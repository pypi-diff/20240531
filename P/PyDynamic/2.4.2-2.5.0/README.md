# Comparing `tmp/PyDynamic-2.4.2.tar.gz` & `tmp/PyDynamic-2.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyDynamic-2.4.2.tar", last modified: Fri Aug 11 07:27:09 2023, max compression
+gzip compressed data, was "PyDynamic-2.5.0.tar", last modified: Fri May 31 13:48:19 2024, max compression
```

## Comparing `PyDynamic-2.4.2.tar` & `PyDynamic-2.5.0.tar`

### file list

```diff
@@ -1,74 +1,166 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-11 07:27:09.139603 PyDynamic-2.4.2/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       98 2023-08-11 07:26:02.000000 PyDynamic-2.4.2/MANIFEST.in
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12023 2023-08-11 07:27:09.139603 PyDynamic-2.4.2/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10499 2023-08-11 07:26:02.000000 PyDynamic-2.4.2/README.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7650 2023-08-11 07:26:02.000000 PyDynamic-2.4.2/licence.txt
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-11 07:27:09.135603 PyDynamic-2.4.2/requirements/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       50 2023-08-11 07:26:02.000000 PyDynamic-2.4.2/requirements/dev-requirements-py310.in
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11281 2023-08-11 07:26:02.000000 PyDynamic-2.4.2/requirements/dev-requirements-py310.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       50 2023-08-11 07:26:02.000000 PyDynamic-2.4.2/requirements/dev-requirements-py311.in
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11034 2023-08-11 07:26:02.000000 PyDynamic-2.4.2/requirements/dev-requirements-py311.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       49 2023-08-11 07:26:02.000000 PyDynamic-2.4.2/requirements/dev-requirements-py38.in
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11769 2023-08-11 07:26:02.000000 PyDynamic-2.4.2/requirements/dev-requirements-py38.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       49 2023-08-11 07:26:02.000000 PyDynamic-2.4.2/requirements/dev-requirements-py39.in
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11600 2023-08-11 07:26:02.000000 PyDynamic-2.4.2/requirements/dev-requirements-py39.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       24 2023-08-11 07:26:02.000000 PyDynamic-2.4.2/requirements/dev-requirements.in
--rw-r--r--   0 circleci  (1001) circleci  (1002)       93 2023-08-11 07:26:02.000000 PyDynamic-2.4.2/requirements/dev-requirements.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      191 2023-08-11 07:26:02.000000 PyDynamic-2.4.2/requirements/environment.yml
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1166 2023-08-11 07:26:02.000000 PyDynamic-2.4.2/requirements/requirements-py310.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1166 2023-08-11 07:26:02.000000 PyDynamic-2.4.2/requirements/requirements-py311.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1255 2023-08-11 07:26:02.000000 PyDynamic-2.4.2/requirements/requirements-py38.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1255 2023-08-11 07:26:02.000000 PyDynamic-2.4.2/requirements/requirements-py39.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       77 2023-08-11 07:26:02.000000 PyDynamic-2.4.2/requirements/requirements.txt
--rwxr-xr-x   0 circleci  (1001) circleci  (1002)     2312 2023-08-11 07:26:02.000000 PyDynamic-2.4.2/requirements/upgrade_dependencies.sh
--rw-r--r--   0 circleci  (1001) circleci  (1002)      642 2023-08-11 07:27:09.139603 PyDynamic-2.4.2/setup.cfg
--rwxr-xr-x   0 circleci  (1001) circleci  (1002)     6234 2023-08-11 07:26:02.000000 PyDynamic-2.4.2/setup.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-11 07:27:09.131603 PyDynamic-2.4.2/src/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-11 07:27:09.135603 PyDynamic-2.4.2/src/PyDynamic/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1644 2023-08-11 07:27:07.000000 PyDynamic-2.4.2/src/PyDynamic/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-11 07:27:09.135603 PyDynamic-2.4.2/src/PyDynamic/deconvolution/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      763 2023-08-11 07:26:02.000000 PyDynamic-2.4.2/src/PyDynamic/deconvolution/__init__.py
--rwxr-xr-x   0 circleci  (1001) circleci  (1002)     2422 2023-08-11 07:26:02.000000 PyDynamic-2.4.2/src/PyDynamic/deconvolution/fit_filter.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-11 07:27:09.135603 PyDynamic-2.4.2/src/PyDynamic/examples/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-08-11 07:26:02.000000 PyDynamic-2.4.2/src/PyDynamic/examples/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1785 2023-08-11 07:26:02.000000 PyDynamic-2.4.2/src/PyDynamic/examples/demonstrate_fit_som.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-11 07:27:09.139603 PyDynamic-2.4.2/src/PyDynamic/examples/uncertainty_for_dft/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3457 2023-08-11 07:26:02.000000 PyDynamic-2.4.2/src/PyDynamic/examples/uncertainty_for_dft/DFT_amplitude_phase.py
--rwxr-xr-x   0 circleci  (1001) circleci  (1002)   256616 2023-08-11 07:26:02.000000 PyDynamic-2.4.2/src/PyDynamic/examples/uncertainty_for_dft/DFTdeconv calibration.dat
--rwxr-xr-x   0 circleci  (1001) circleci  (1002)    50594 2023-08-11 07:26:02.000000 PyDynamic-2.4.2/src/PyDynamic/examples/uncertainty_for_dft/DFTdeconv measured_signal.dat
--rwxr-xr-x   0 circleci  (1001) circleci  (1002)    50623 2023-08-11 07:26:02.000000 PyDynamic-2.4.2/src/PyDynamic/examples/uncertainty_for_dft/DFTdeconv reference_signal.dat
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-08-11 07:26:02.000000 PyDynamic-2.4.2/src/PyDynamic/examples/uncertainty_for_dft/__init__.py
--rwxr-xr-x   0 circleci  (1001) circleci  (1002)     6197 2023-08-11 07:26:02.000000 PyDynamic-2.4.2/src/PyDynamic/examples/uncertainty_for_dft/deconv_DFT.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1268 2023-08-11 07:26:02.000000 PyDynamic-2.4.2/src/PyDynamic/examples/working_with_signals.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-11 07:27:09.139603 PyDynamic-2.4.2/src/PyDynamic/identification/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      409 2023-08-11 07:26:02.000000 PyDynamic-2.4.2/src/PyDynamic/identification/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1034 2023-08-11 07:26:02.000000 PyDynamic-2.4.2/src/PyDynamic/identification/fit_filter.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      847 2023-08-11 07:26:02.000000 PyDynamic-2.4.2/src/PyDynamic/identification/fit_transfer.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-11 07:27:09.139603 PyDynamic-2.4.2/src/PyDynamic/misc/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5838 2023-08-11 07:26:02.000000 PyDynamic-2.4.2/src/PyDynamic/misc/SecondOrderSystem.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1884 2023-08-11 07:26:02.000000 PyDynamic-2.4.2/src/PyDynamic/misc/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7936 2023-08-11 07:26:02.000000 PyDynamic-2.4.2/src/PyDynamic/misc/filterstuff.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7847 2023-08-11 07:26:02.000000 PyDynamic-2.4.2/src/PyDynamic/misc/impinvar.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7217 2023-08-11 07:26:02.000000 PyDynamic-2.4.2/src/PyDynamic/misc/noise.py
--rwxr-xr-x   0 circleci  (1001) circleci  (1002)     8724 2023-08-11 07:26:02.000000 PyDynamic-2.4.2/src/PyDynamic/misc/testsignals.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    23151 2023-08-11 07:26:02.000000 PyDynamic-2.4.2/src/PyDynamic/misc/tools.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-11 07:27:09.139603 PyDynamic-2.4.2/src/PyDynamic/model_estimation/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      710 2023-08-11 07:26:02.000000 PyDynamic-2.4.2/src/PyDynamic/model_estimation/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    39343 2023-08-11 07:26:02.000000 PyDynamic-2.4.2/src/PyDynamic/model_estimation/fit_filter.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9530 2023-08-11 07:26:02.000000 PyDynamic-2.4.2/src/PyDynamic/model_estimation/fit_transfer.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9972 2023-08-11 07:26:02.000000 PyDynamic-2.4.2/src/PyDynamic/signals.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-11 07:27:09.139603 PyDynamic-2.4.2/src/PyDynamic/uncertainty/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1582 2023-08-11 07:26:02.000000 PyDynamic-2.4.2/src/PyDynamic/uncertainty/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    17787 2023-08-11 07:26:02.000000 PyDynamic-2.4.2/src/PyDynamic/uncertainty/interpolate.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      773 2023-08-11 07:26:02.000000 PyDynamic-2.4.2/src/PyDynamic/uncertainty/interpolation.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    39847 2023-08-11 07:26:02.000000 PyDynamic-2.4.2/src/PyDynamic/uncertainty/propagate_DFT.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14351 2023-08-11 07:26:02.000000 PyDynamic-2.4.2/src/PyDynamic/uncertainty/propagate_DWT.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    27932 2023-08-11 07:26:02.000000 PyDynamic-2.4.2/src/PyDynamic/uncertainty/propagate_MonteCarlo.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6282 2023-08-11 07:26:02.000000 PyDynamic-2.4.2/src/PyDynamic/uncertainty/propagate_convolution.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    26281 2023-08-11 07:26:02.000000 PyDynamic-2.4.2/src/PyDynamic/uncertainty/propagate_filter.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-11 07:27:09.135603 PyDynamic-2.4.2/src/PyDynamic.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12023 2023-08-11 07:27:09.000000 PyDynamic-2.4.2/src/PyDynamic.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2353 2023-08-11 07:27:09.000000 PyDynamic-2.4.2/src/PyDynamic.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-08-11 07:27:09.000000 PyDynamic-2.4.2/src/PyDynamic.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      262 2023-08-11 07:27:09.000000 PyDynamic-2.4.2/src/PyDynamic.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       10 2023-08-11 07:27:09.000000 PyDynamic-2.4.2/src/PyDynamic.egg-info/top_level.txt
+drwxr-xr-x   0 ludwig10  (1000) ludwig10  (1001)        0 2024-05-31 13:48:19.371653 PyDynamic-2.5.0/
+drwxr-xr-x   0 ludwig10  (1000) ludwig10  (1001)        0 2024-05-31 13:48:19.298319 PyDynamic-2.5.0/.circleci/
+-rw-r--r--   0 ludwig10  (1000) ludwig10  (1001)    19008 2024-04-17 09:43:43.000000 PyDynamic-2.5.0/.circleci/config.yml
+-rw-r--r--   0 ludwig10  (1000) ludwig10  (1001)      265 2021-11-07 11:41:25.000000 PyDynamic-2.5.0/.coveragerc
+drwxr-xr-x   0 ludwig10  (1000) ludwig10  (1001)        0 2024-05-31 13:48:19.291653 PyDynamic-2.5.0/.github/
+drwxr-xr-x   0 ludwig10  (1000) ludwig10  (1001)        0 2024-05-31 13:48:19.301653 PyDynamic-2.5.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 ludwig10  (1000) ludwig10  (1001)      684 2021-09-21 16:11:46.000000 PyDynamic-2.5.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 ludwig10  (1000) ludwig10  (1001)       27 2021-09-21 16:11:46.000000 PyDynamic-2.5.0/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 ludwig10  (1000) ludwig10  (1001)      614 2021-09-21 16:11:46.000000 PyDynamic-2.5.0/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 ludwig10  (1000) ludwig10  (1001)      497 2022-01-31 21:20:02.000000 PyDynamic-2.5.0/.gitignore
+-rw-r--r--   0 ludwig10  (1000) ludwig10  (1001)      510 2023-11-01 16:14:37.000000 PyDynamic-2.5.0/.readthedocs.yaml
+-rw-r--r--   0 ludwig10  (1000) ludwig10  (1001)     1418 2022-02-06 15:49:00.000000 PyDynamic-2.5.0/.zenodo.json
+-rw-r--r--   0 ludwig10  (1000) ludwig10  (1001)    20501 2024-05-24 10:33:22.000000 PyDynamic-2.5.0/CHANGELOG.md
+-rw-r--r--   0 ludwig10  (1000) ludwig10  (1001)     5261 2021-11-07 03:02:34.000000 PyDynamic-2.5.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 ludwig10  (1000) ludwig10  (1001)    12455 2023-08-01 08:11:44.000000 PyDynamic-2.5.0/CONTRIBUTING.md
+-rw-r--r--   0 ludwig10  (1000) ludwig10  (1001)     4800 2023-08-01 16:34:37.000000 PyDynamic-2.5.0/INSTALL.md
+-rw-r--r--   0 ludwig10  (1000) ludwig10  (1001)       98 2021-11-04 12:22:54.000000 PyDynamic-2.5.0/MANIFEST.in
+-rw-r--r--   0 ludwig10  (1000) ludwig10  (1001)    12023 2024-05-31 13:48:19.371653 PyDynamic-2.5.0/PKG-INFO
+-rw-r--r--   0 ludwig10  (1000) ludwig10  (1001)    10499 2024-05-31 10:26:12.000000 PyDynamic-2.5.0/README.md
+-rw-r--r--   0 ludwig10  (1000) ludwig10  (1001)       91 2021-11-04 12:22:54.000000 PyDynamic-2.5.0/_config.yml
+drwxr-xr-x   0 ludwig10  (1000) ludwig10  (1001)        0 2024-05-31 13:48:19.334986 PyDynamic-2.5.0/docs/
+-rw-r--r--   0 ludwig10  (1000) ludwig10  (1001)    40026 2021-09-21 16:11:46.000000 PyDynamic-2.5.0/docs/DFT_13_0.png
+-rw-r--r--   0 ludwig10  (1000) ludwig10  (1001)    88856 2021-09-21 16:11:46.000000 PyDynamic-2.5.0/docs/DFT_16_0.png
+-rw-r--r--   0 ludwig10  (1000) ludwig10  (1001)    46825 2021-09-21 16:11:46.000000 PyDynamic-2.5.0/docs/DFT_22_0.png
+-rw-r--r--   0 ludwig10  (1000) ludwig10  (1001)    66029 2021-09-21 16:11:46.000000 PyDynamic-2.5.0/docs/DFT_26_0.png
+-rw-r--r--   0 ludwig10  (1000) ludwig10  (1001)    41400 2021-09-21 16:11:46.000000 PyDynamic-2.5.0/docs/DFT_27_0.png
+-rw-r--r--   0 ludwig10  (1000) ludwig10  (1001)    56576 2021-09-21 16:11:46.000000 PyDynamic-2.5.0/docs/DFT_5_0.png
+-rw-r--r--   0 ludwig10  (1000) ludwig10  (1001)    22081 2021-09-21 16:11:46.000000 PyDynamic-2.5.0/docs/DFT_6_0.png
+-rw-r--r--   0 ludwig10  (1000) ludwig10  (1001)     9072 2021-11-07 03:02:34.000000 PyDynamic-2.5.0/docs/Deconvolution by FIR.rst
+-rw-r--r--   0 ludwig10  (1000) ludwig10  (1001)    10659 2021-09-21 16:11:46.000000 PyDynamic-2.5.0/docs/Deconvolution in the DFT domain.rst
+-rw-r--r--   0 ludwig10  (1000) ludwig10  (1001)    92929 2021-11-04 12:22:54.000000 PyDynamic-2.5.0/docs/Deconvolution.png
+-rw-r--r--   0 ludwig10  (1000) ludwig10  (1001)     2515 2021-11-07 03:02:34.000000 PyDynamic-2.5.0/docs/Examples.rst
+-rw-r--r--   0 ludwig10  (1000) ludwig10  (1001)    13780 2021-09-21 16:11:46.000000 PyDynamic-2.5.0/docs/FIR_16_0.png
+-rw-r--r--   0 ludwig10  (1000) ludwig10  (1001)    57468 2021-09-21 16:11:46.000000 PyDynamic-2.5.0/docs/FIR_20_0.png
+-rw-r--r--   0 ludwig10  (1000) ludwig10  (1001)    63274 2021-09-21 16:11:46.000000 PyDynamic-2.5.0/docs/FIR_22_0.png
+-rw-r--r--   0 ludwig10  (1000) ludwig10  (1001)    56136 2021-09-21 16:11:46.000000 PyDynamic-2.5.0/docs/FIR_23_0.png
+-rw-r--r--   0 ludwig10  (1000) ludwig10  (1001)    16272 2021-09-21 16:11:46.000000 PyDynamic-2.5.0/docs/FIR_5_0.png
+-rw-r--r--   0 ludwig10  (1000) ludwig10  (1001)    16790 2021-09-21 16:11:46.000000 PyDynamic-2.5.0/docs/FIR_6_0.png
+-rw-r--r--   0 ludwig10  (1000) ludwig10  (1001)    66073 2021-09-21 16:11:46.000000 PyDynamic-2.5.0/docs/FIR_9_0.png
+-rw-r--r--   0 ludwig10  (1000) ludwig10  (1001)    35450 2021-09-21 16:11:46.000000 PyDynamic-2.5.0/docs/IIR_16_0.png
+-rw-r--r--   0 ludwig10  (1000) ludwig10  (1001)    20477 2021-09-21 16:11:46.000000 PyDynamic-2.5.0/docs/IIR_18_0.png
+-rw-r--r--   0 ludwig10  (1000) ludwig10  (1001)    11772 2021-09-21 16:11:46.000000 PyDynamic-2.5.0/docs/IIR_21_0.png
+-rw-r--r--   0 ludwig10  (1000) ludwig10  (1001)    28842 2021-09-21 16:11:46.000000 PyDynamic-2.5.0/docs/IIR_23_0.png
+-rw-r--r--   0 ludwig10  (1000) ludwig10  (1001)    25474 2021-09-21 16:11:46.000000 PyDynamic-2.5.0/docs/IIR_24_0.png
+-rw-r--r--   0 ludwig10  (1000) ludwig10  (1001)    42787 2021-09-21 16:11:46.000000 PyDynamic-2.5.0/docs/IIR_28_1.png
+-rw-r--r--   0 ludwig10  (1000) ludwig10  (1001)     1081 2021-09-21 16:11:46.000000 PyDynamic-2.5.0/docs/PyDynamic.misc.rst
+-rw-r--r--   0 ludwig10  (1000) ludwig10  (1001)     1269 2021-09-21 16:11:46.000000 PyDynamic-2.5.0/docs/PyDynamic.model_estimation.rst
+-rw-r--r--   0 ludwig10  (1000) ludwig10  (1001)       62 2022-01-31 11:49:22.000000 PyDynamic-2.5.0/docs/PyDynamic.signals.rst
+-rw-r--r--   0 ludwig10  (1000) ludwig10  (1001)     2304 2024-05-24 10:33:22.000000 PyDynamic-2.5.0/docs/PyDynamic.uncertainty.rst
+-rw-r--r--   0 ludwig10  (1000) ludwig10  (1001)    28678 2023-11-01 16:14:37.000000 PyDynamic-2.5.0/docs/PyDynamic_logo.png
+-rw-r--r--   0 ludwig10  (1000) ludwig10  (1001)     3252 2021-11-07 03:02:34.000000 PyDynamic-2.5.0/docs/PyDynamic_logo.svg
+-rw-r--r--   0 ludwig10  (1000) ludwig10  (1001)     2975 2023-03-14 16:07:08.000000 PyDynamic-2.5.0/docs/PyDynamic_module_diagram.drawio
+-rw-r--r--   0 ludwig10  (1000) ludwig10  (1001)    46611 2023-03-14 16:07:08.000000 PyDynamic-2.5.0/docs/PyDynamic_module_diagram.png
+-rw-r--r--   0 ludwig10  (1000) ludwig10  (1001)     2116 2022-04-22 12:51:57.000000 PyDynamic-2.5.0/docs/Tutorials.rst
+-rw-r--r--   0 ludwig10  (1000) ludwig10  (1001)     7410 2021-09-21 16:11:46.000000 PyDynamic-2.5.0/docs/Uncertainty propagation for IIR filters.rst
+-rw-r--r--   0 ludwig10  (1000) ludwig10  (1001)    13391 2024-05-24 10:33:22.000000 PyDynamic-2.5.0/docs/conf.py
+-rw-r--r--   0 ludwig10  (1000) ludwig10  (1001)     3559 2024-05-31 10:26:12.000000 PyDynamic-2.5.0/docs/index.rst
+-rw-r--r--   0 ludwig10  (1000) ludwig10  (1001)  3457110 2021-11-04 12:22:54.000000 PyDynamic-2.5.0/docs/numpy-intersphinx-mappings.txt
+-rw-r--r--   0 ludwig10  (1000) ludwig10  (1001)    33709 2021-11-04 12:20:45.000000 PyDynamic-2.5.0/docs/pydynamic-intersphinx-mappings.txt
+-rw-r--r--   0 ludwig10  (1000) ludwig10  (1001)    24596 2021-11-04 12:20:45.000000 PyDynamic-2.5.0/docs/pydynamic_tutorials-intersphinx-mappings.txt
+-rw-r--r--   0 ludwig10  (1000) ludwig10  (1001)    47676 2022-02-06 15:42:34.000000 PyDynamic-2.5.0/docs/pywavelets-intersphinx-mappings.txt
+-rw-r--r--   0 ludwig10  (1000) ludwig10  (1001)  1290523 2022-02-06 15:40:22.000000 PyDynamic-2.5.0/docs/scipy-intersphinx-mappings.txt
+-rw-r--r--   0 ludwig10  (1000) ludwig10  (1001)     7650 2020-09-29 10:24:27.000000 PyDynamic-2.5.0/licence.txt
+-rw-r--r--   0 ludwig10  (1000) ludwig10  (1001)      451 2022-01-31 21:20:02.000000 PyDynamic-2.5.0/pytest.ini
+drwxr-xr-x   0 ludwig10  (1000) ludwig10  (1001)        0 2024-05-31 13:48:19.344986 PyDynamic-2.5.0/requirements/
+-rw-r--r--   0 ludwig10  (1000) ludwig10  (1001)       50 2022-01-30 23:44:49.000000 PyDynamic-2.5.0/requirements/dev-requirements-py310.in
+-rw-r--r--   0 ludwig10  (1000) ludwig10  (1001)    11635 2024-05-31 10:26:12.000000 PyDynamic-2.5.0/requirements/dev-requirements-py310.txt
+-rw-r--r--   0 ludwig10  (1000) ludwig10  (1001)       50 2023-08-01 16:34:37.000000 PyDynamic-2.5.0/requirements/dev-requirements-py311.in
+-rw-r--r--   0 ludwig10  (1000) ludwig10  (1001)    11363 2024-05-31 10:26:12.000000 PyDynamic-2.5.0/requirements/dev-requirements-py311.txt
+-rw-r--r--   0 ludwig10  (1000) ludwig10  (1001)       49 2021-11-04 12:20:34.000000 PyDynamic-2.5.0/requirements/dev-requirements-py38.in
+-rw-r--r--   0 ludwig10  (1000) ludwig10  (1001)    12122 2024-05-31 10:26:12.000000 PyDynamic-2.5.0/requirements/dev-requirements-py38.txt
+-rw-r--r--   0 ludwig10  (1000) ludwig10  (1001)       49 2021-11-04 12:22:54.000000 PyDynamic-2.5.0/requirements/dev-requirements-py39.in
+-rw-r--r--   0 ludwig10  (1000) ludwig10  (1001)    11916 2024-05-31 10:26:12.000000 PyDynamic-2.5.0/requirements/dev-requirements-py39.txt
+-rw-r--r--   0 ludwig10  (1000) ludwig10  (1001)       24 2023-08-01 16:34:37.000000 PyDynamic-2.5.0/requirements/dev-requirements.in
+-rw-r--r--   0 ludwig10  (1000) ludwig10  (1001)       93 2022-01-31 21:20:02.000000 PyDynamic-2.5.0/requirements/dev-requirements.txt
+-rw-r--r--   0 ludwig10  (1000) ludwig10  (1001)      191 2022-01-31 21:20:02.000000 PyDynamic-2.5.0/requirements/environment.yml
+-rw-r--r--   0 ludwig10  (1000) ludwig10  (1001)     1171 2024-05-31 10:26:12.000000 PyDynamic-2.5.0/requirements/requirements-py310.txt
+-rw-r--r--   0 ludwig10  (1000) ludwig10  (1001)     1171 2024-05-31 10:26:12.000000 PyDynamic-2.5.0/requirements/requirements-py311.txt
+-rw-r--r--   0 ludwig10  (1000) ludwig10  (1001)     1260 2024-05-31 10:26:12.000000 PyDynamic-2.5.0/requirements/requirements-py38.txt
+-rw-r--r--   0 ludwig10  (1000) ludwig10  (1001)     1260 2024-05-31 10:26:12.000000 PyDynamic-2.5.0/requirements/requirements-py39.txt
+-rw-r--r--   0 ludwig10  (1000) ludwig10  (1001)       77 2022-01-31 21:20:02.000000 PyDynamic-2.5.0/requirements/requirements.txt
+-rwxr-xr-x   0 ludwig10  (1000) ludwig10  (1001)     2312 2023-08-01 16:34:37.000000 PyDynamic-2.5.0/requirements/upgrade_dependencies.sh
+-rw-r--r--   0 ludwig10  (1000) ludwig10  (1001)      642 2024-05-31 13:48:19.371653 PyDynamic-2.5.0/setup.cfg
+-rwxr-xr-x   0 ludwig10  (1000) ludwig10  (1001)     6234 2024-05-31 10:26:12.000000 PyDynamic-2.5.0/setup.py
+drwxr-xr-x   0 ludwig10  (1000) ludwig10  (1001)        0 2024-05-31 13:48:19.291653 PyDynamic-2.5.0/src/
+drwxr-xr-x   0 ludwig10  (1000) ludwig10  (1001)        0 2024-05-31 13:48:19.344986 PyDynamic-2.5.0/src/PyDynamic/
+-rw-r--r--   0 ludwig10  (1000) ludwig10  (1001)     1693 2024-05-31 10:26:12.000000 PyDynamic-2.5.0/src/PyDynamic/__init__.py
+drwxr-xr-x   0 ludwig10  (1000) ludwig10  (1001)        0 2024-05-31 13:48:19.344986 PyDynamic-2.5.0/src/PyDynamic/deconvolution/
+-rw-r--r--   0 ludwig10  (1000) ludwig10  (1001)      763 2021-11-07 03:02:34.000000 PyDynamic-2.5.0/src/PyDynamic/deconvolution/__init__.py
+-rwxr-xr-x   0 ludwig10  (1000) ludwig10  (1001)     2422 2021-11-08 21:32:42.000000 PyDynamic-2.5.0/src/PyDynamic/deconvolution/fit_filter.py
+drwxr-xr-x   0 ludwig10  (1000) ludwig10  (1001)        0 2024-05-31 13:48:19.348320 PyDynamic-2.5.0/src/PyDynamic/examples/
+-rw-r--r--   0 ludwig10  (1000) ludwig10  (1001)  1200883 2024-05-31 10:26:12.000000 PyDynamic-2.5.0/src/PyDynamic/examples/DFT and iDFT with PyDynamic - best practice guide and use cases.ipynb
+drwxr-xr-x   0 ludwig10  (1000) ludwig10  (1001)        0 2024-05-31 13:48:19.348320 PyDynamic-2.5.0/src/PyDynamic/examples/Interpolating/
+-rw-r--r--   0 ludwig10  (1000) ludwig10  (1001)     1343 2021-11-08 21:32:42.000000 PyDynamic-2.5.0/src/PyDynamic/examples/Interpolating/validation_spline_interp_with_MC.py
+drwxr-xr-x   0 ludwig10  (1000) ludwig10  (1001)        0 2024-05-31 13:48:19.351653 PyDynamic-2.5.0/src/PyDynamic/examples/Shock calibration/
+-rw-r--r--   0 ludwig10  (1000) ludwig10  (1001)   165874 2023-03-14 16:07:08.000000 PyDynamic-2.5.0/src/PyDynamic/examples/Shock calibration/Input estimation for shock acceleration example.ipynb
+-rwxr-xr-x   0 ludwig10  (1000) ludwig10  (1001)   324000 2021-11-04 12:22:54.000000 PyDynamic-2.5.0/src/PyDynamic/examples/Shock calibration/measured_input_accel.txt
+-rwxr-xr-x   0 ludwig10  (1000) ludwig10  (1001)   324000 2021-11-04 12:22:54.000000 PyDynamic-2.5.0/src/PyDynamic/examples/Shock calibration/measured_output_accel.txt
+-rw-r--r--   0 ludwig10  (1000) ludwig10  (1001)     3724 2021-11-04 12:22:54.000000 PyDynamic-2.5.0/src/PyDynamic/examples/Shock calibration/sinusoidal_calibration_values.txt
+-rw-r--r--   0 ludwig10  (1000) ludwig10  (1001)        0 2021-11-04 12:22:54.000000 PyDynamic-2.5.0/src/PyDynamic/examples/__init__.py
+-rw-r--r--   0 ludwig10  (1000) ludwig10  (1001)     1785 2021-11-08 16:08:31.000000 PyDynamic-2.5.0/src/PyDynamic/examples/demonstrate_fit_som.py
+drwxr-xr-x   0 ludwig10  (1000) ludwig10  (1001)        0 2024-05-31 13:48:19.358320 PyDynamic-2.5.0/src/PyDynamic/examples/digital_filtering/
+-rw-r--r--   0 ludwig10  (1000) ludwig10  (1001)   730515 2023-03-14 16:07:08.000000 PyDynamic-2.5.0/src/PyDynamic/examples/digital_filtering/Design of a digital deconvolution filter (FIR type).ipynb
+-rw-r--r--   0 ludwig10  (1000) ludwig10  (1001)     1996 2021-11-08 21:32:42.000000 PyDynamic-2.5.0/src/PyDynamic/examples/digital_filtering/FIRuncFilter_runtime_comparison.py
+-rw-r--r--   0 ludwig10  (1000) ludwig10  (1001)     5084 2021-11-08 21:32:42.000000 PyDynamic-2.5.0/src/PyDynamic/examples/digital_filtering/deconv_FIR.py
+-rw-r--r--   0 ludwig10  (1000) ludwig10  (1001)     1871 2021-11-12 07:01:40.000000 PyDynamic-2.5.0/src/PyDynamic/examples/digital_filtering/identify_IIR.py
+-rw-r--r--   0 ludwig10  (1000) ludwig10  (1001)     5971 2023-03-14 16:07:08.000000 PyDynamic-2.5.0/src/PyDynamic/examples/digital_filtering/realtime_dwt.py
+-rw-r--r--   0 ludwig10  (1000) ludwig10  (1001)     1899 2023-03-14 16:07:08.000000 PyDynamic-2.5.0/src/PyDynamic/examples/digital_filtering/speed_comparison_filter.py
+-rw-r--r--   0 ludwig10  (1000) ludwig10  (1001)     1813 2021-11-08 21:32:42.000000 PyDynamic-2.5.0/src/PyDynamic/examples/digital_filtering/uncpropagation_FIR.py
+-rw-r--r--   0 ludwig10  (1000) ludwig10  (1001)     2207 2021-11-08 21:32:42.000000 PyDynamic-2.5.0/src/PyDynamic/examples/digital_filtering/uncpropagation_IIR.py
+-rw-r--r--   0 ludwig10  (1000) ludwig10  (1001)     3105 2021-11-07 03:02:34.000000 PyDynamic-2.5.0/src/PyDynamic/examples/digital_filtering/validate_DWT_monte_carlo.py
+-rw-r--r--   0 ludwig10  (1000) ludwig10  (1001)     2470 2021-11-08 21:32:42.000000 PyDynamic-2.5.0/src/PyDynamic/examples/digital_filtering/validate_FIR_IIR_MC.py
+-rw-r--r--   0 ludwig10  (1000) ludwig10  (1001)     4470 2021-11-08 21:32:42.000000 PyDynamic-2.5.0/src/PyDynamic/examples/digital_filtering/validate_FIRuncFilter.py
+drwxr-xr-x   0 ludwig10  (1000) ludwig10  (1001)        0 2024-05-31 13:48:19.361653 PyDynamic-2.5.0/src/PyDynamic/examples/uncertainty_for_dft/
+-rw-r--r--   0 ludwig10  (1000) ludwig10  (1001)     3457 2023-03-14 16:07:08.000000 PyDynamic-2.5.0/src/PyDynamic/examples/uncertainty_for_dft/DFT_amplitude_phase.py
+-rwxr-xr-x   0 ludwig10  (1000) ludwig10  (1001)   256616 2021-11-04 12:22:54.000000 PyDynamic-2.5.0/src/PyDynamic/examples/uncertainty_for_dft/DFTdeconv calibration.dat
+-rwxr-xr-x   0 ludwig10  (1000) ludwig10  (1001)    50594 2021-11-04 12:22:54.000000 PyDynamic-2.5.0/src/PyDynamic/examples/uncertainty_for_dft/DFTdeconv measured_signal.dat
+-rwxr-xr-x   0 ludwig10  (1000) ludwig10  (1001)    50623 2021-11-04 12:22:54.000000 PyDynamic-2.5.0/src/PyDynamic/examples/uncertainty_for_dft/DFTdeconv reference_signal.dat
+-rw-r--r--   0 ludwig10  (1000) ludwig10  (1001)        0 2021-11-04 12:22:54.000000 PyDynamic-2.5.0/src/PyDynamic/examples/uncertainty_for_dft/__init__.py
+drwxr-xr-x   0 ludwig10  (1000) ludwig10  (1001)        0 2024-05-31 13:48:19.364987 PyDynamic-2.5.0/src/PyDynamic/examples/uncertainty_for_dft/__pycache__/
+-rw-r--r--   0 ludwig10  (1000) ludwig10  (1001)     2751 2024-05-24 11:46:45.000000 PyDynamic-2.5.0/src/PyDynamic/examples/uncertainty_for_dft/__pycache__/DFT_amplitude_phase.cpython-310.pyc
+-rw-r--r--   0 ludwig10  (1000) ludwig10  (1001)     2759 2021-11-26 16:47:08.000000 PyDynamic-2.5.0/src/PyDynamic/examples/uncertainty_for_dft/__pycache__/DFT_amplitude_phase.cpython-38.pyc
+-rw-r--r--   0 ludwig10  (1000) ludwig10  (1001)     2743 2021-12-15 18:43:24.000000 PyDynamic-2.5.0/src/PyDynamic/examples/uncertainty_for_dft/__pycache__/DFT_amplitude_phase.cpython-39.pyc
+-rw-r--r--   0 ludwig10  (1000) ludwig10  (1001)      177 2024-05-24 11:46:45.000000 PyDynamic-2.5.0/src/PyDynamic/examples/uncertainty_for_dft/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 ludwig10  (1000) ludwig10  (1001)      175 2021-11-26 16:47:08.000000 PyDynamic-2.5.0/src/PyDynamic/examples/uncertainty_for_dft/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 ludwig10  (1000) ludwig10  (1001)      175 2021-11-07 05:04:07.000000 PyDynamic-2.5.0/src/PyDynamic/examples/uncertainty_for_dft/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 ludwig10  (1000) ludwig10  (1001)     5822 2024-05-24 11:46:45.000000 PyDynamic-2.5.0/src/PyDynamic/examples/uncertainty_for_dft/__pycache__/deconv_DFT.cpython-310.pyc
+-rw-r--r--   0 ludwig10  (1000) ludwig10  (1001)     5798 2021-11-26 16:47:08.000000 PyDynamic-2.5.0/src/PyDynamic/examples/uncertainty_for_dft/__pycache__/deconv_DFT.cpython-38.pyc
+-rw-r--r--   0 ludwig10  (1000) ludwig10  (1001)     5812 2021-12-15 18:43:24.000000 PyDynamic-2.5.0/src/PyDynamic/examples/uncertainty_for_dft/__pycache__/deconv_DFT.cpython-39.pyc
+-rwxr-xr-x   0 ludwig10  (1000) ludwig10  (1001)     6197 2023-03-14 16:07:08.000000 PyDynamic-2.5.0/src/PyDynamic/examples/uncertainty_for_dft/deconv_DFT.py
+-rw-r--r--   0 ludwig10  (1000) ludwig10  (1001)     1268 2022-01-31 11:49:22.000000 PyDynamic-2.5.0/src/PyDynamic/examples/working_with_signals.py
+drwxr-xr-x   0 ludwig10  (1000) ludwig10  (1001)        0 2024-05-31 13:48:19.364987 PyDynamic-2.5.0/src/PyDynamic/identification/
+-rw-r--r--   0 ludwig10  (1000) ludwig10  (1001)      409 2021-11-08 21:32:42.000000 PyDynamic-2.5.0/src/PyDynamic/identification/__init__.py
+-rw-r--r--   0 ludwig10  (1000) ludwig10  (1001)     1034 2021-11-08 21:32:42.000000 PyDynamic-2.5.0/src/PyDynamic/identification/fit_filter.py
+-rw-r--r--   0 ludwig10  (1000) ludwig10  (1001)      847 2021-11-08 21:32:42.000000 PyDynamic-2.5.0/src/PyDynamic/identification/fit_transfer.py
+drwxr-xr-x   0 ludwig10  (1000) ludwig10  (1001)        0 2024-05-31 13:48:19.368320 PyDynamic-2.5.0/src/PyDynamic/misc/
+-rw-r--r--   0 ludwig10  (1000) ludwig10  (1001)     5838 2023-03-14 16:07:08.000000 PyDynamic-2.5.0/src/PyDynamic/misc/SecondOrderSystem.py
+-rw-r--r--   0 ludwig10  (1000) ludwig10  (1001)     1884 2021-12-16 20:44:39.000000 PyDynamic-2.5.0/src/PyDynamic/misc/__init__.py
+-rw-r--r--   0 ludwig10  (1000) ludwig10  (1001)     7936 2023-03-14 16:07:08.000000 PyDynamic-2.5.0/src/PyDynamic/misc/filterstuff.py
+-rw-r--r--   0 ludwig10  (1000) ludwig10  (1001)     7847 2021-11-08 21:32:42.000000 PyDynamic-2.5.0/src/PyDynamic/misc/impinvar.py
+-rw-r--r--   0 ludwig10  (1000) ludwig10  (1001)    31963 2021-11-04 12:22:54.000000 PyDynamic-2.5.0/src/PyDynamic/misc/impinvar_license.txt
+-rw-r--r--   0 ludwig10  (1000) ludwig10  (1001)     7217 2023-03-14 16:07:08.000000 PyDynamic-2.5.0/src/PyDynamic/misc/noise.py
+-rwxr-xr-x   0 ludwig10  (1000) ludwig10  (1001)     8724 2023-03-14 16:07:08.000000 PyDynamic-2.5.0/src/PyDynamic/misc/testsignals.py
+-rw-r--r--   0 ludwig10  (1000) ludwig10  (1001)    23151 2023-08-01 07:36:41.000000 PyDynamic-2.5.0/src/PyDynamic/misc/tools.py
+drwxr-xr-x   0 ludwig10  (1000) ludwig10  (1001)        0 2024-05-31 13:48:19.368320 PyDynamic-2.5.0/src/PyDynamic/model_estimation/
+-rw-r--r--   0 ludwig10  (1000) ludwig10  (1001)      710 2021-11-08 21:32:42.000000 PyDynamic-2.5.0/src/PyDynamic/model_estimation/__init__.py
+-rw-r--r--   0 ludwig10  (1000) ludwig10  (1001)    39343 2022-08-19 07:00:31.000000 PyDynamic-2.5.0/src/PyDynamic/model_estimation/fit_filter.py
+-rw-r--r--   0 ludwig10  (1000) ludwig10  (1001)     9530 2023-03-14 16:07:08.000000 PyDynamic-2.5.0/src/PyDynamic/model_estimation/fit_transfer.py
+-rw-r--r--   0 ludwig10  (1000) ludwig10  (1001)     9972 2022-01-31 11:49:22.000000 PyDynamic-2.5.0/src/PyDynamic/signals.py
+drwxr-xr-x   0 ludwig10  (1000) ludwig10  (1001)        0 2024-05-31 13:48:19.371653 PyDynamic-2.5.0/src/PyDynamic/uncertainty/
+-rw-r--r--   0 ludwig10  (1000) ludwig10  (1001)     1705 2024-05-24 10:33:22.000000 PyDynamic-2.5.0/src/PyDynamic/uncertainty/__init__.py
+-rw-r--r--   0 ludwig10  (1000) ludwig10  (1001)    17787 2023-03-14 16:07:08.000000 PyDynamic-2.5.0/src/PyDynamic/uncertainty/interpolate.py
+-rw-r--r--   0 ludwig10  (1000) ludwig10  (1001)      773 2021-11-07 03:02:34.000000 PyDynamic-2.5.0/src/PyDynamic/uncertainty/interpolation.py
+-rw-r--r--   0 ludwig10  (1000) ludwig10  (1001)    39847 2023-08-01 07:36:41.000000 PyDynamic-2.5.0/src/PyDynamic/uncertainty/propagate_DFT.py
+-rw-r--r--   0 ludwig10  (1000) ludwig10  (1001)    14351 2023-03-14 16:07:08.000000 PyDynamic-2.5.0/src/PyDynamic/uncertainty/propagate_DWT.py
+-rw-r--r--   0 ludwig10  (1000) ludwig10  (1001)    27932 2023-08-01 07:36:41.000000 PyDynamic-2.5.0/src/PyDynamic/uncertainty/propagate_MonteCarlo.py
+-rw-r--r--   0 ludwig10  (1000) ludwig10  (1001)     6282 2022-04-22 15:01:32.000000 PyDynamic-2.5.0/src/PyDynamic/uncertainty/propagate_convolution.py
+-rw-r--r--   0 ludwig10  (1000) ludwig10  (1001)    26281 2023-03-14 16:07:08.000000 PyDynamic-2.5.0/src/PyDynamic/uncertainty/propagate_filter.py
+-rw-r--r--   0 ludwig10  (1000) ludwig10  (1001)     6743 2024-05-24 10:33:22.000000 PyDynamic-2.5.0/src/PyDynamic/uncertainty/propagate_multiplication.py
+drwxr-xr-x   0 ludwig10  (1000) ludwig10  (1001)        0 2024-05-31 13:48:19.344986 PyDynamic-2.5.0/src/PyDynamic.egg-info/
+-rw-r--r--   0 ludwig10  (1000) ludwig10  (1001)    12023 2024-05-31 13:48:19.000000 PyDynamic-2.5.0/src/PyDynamic.egg-info/PKG-INFO
+-rw-r--r--   0 ludwig10  (1000) ludwig10  (1001)     5687 2024-05-31 13:48:19.000000 PyDynamic-2.5.0/src/PyDynamic.egg-info/SOURCES.txt
+-rw-r--r--   0 ludwig10  (1000) ludwig10  (1001)        1 2024-05-31 13:48:19.000000 PyDynamic-2.5.0/src/PyDynamic.egg-info/dependency_links.txt
+-rw-r--r--   0 ludwig10  (1000) ludwig10  (1001)      262 2024-05-31 13:48:19.000000 PyDynamic-2.5.0/src/PyDynamic.egg-info/requires.txt
+-rw-r--r--   0 ludwig10  (1000) ludwig10  (1001)       10 2024-05-31 13:48:19.000000 PyDynamic-2.5.0/src/PyDynamic.egg-info/top_level.txt
+-rw-r--r--   0 ludwig10  (1000) ludwig10  (1001)      536 2023-08-01 16:34:37.000000 PyDynamic-2.5.0/tox.ini
```

### Comparing `PyDynamic-2.4.2/PKG-INFO` & `PyDynamic-2.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: PyDynamic
-Version: 2.4.2
+Version: 2.5.0
 Summary: A software package for the analysis of dynamic measurements
 Home-page: https://ptb-m4d.github.io/PyDynamic/
+Download-URL: https://github.com/PTB-M4D/PyDynamic/releases/download/v2.5.0/PyDynamic-2.5.0.tar.gz
 Author: Sascha Eichstädt, Maximilian Gruber, Björn Ludwig, Thomas Bruns, Martin Weber
 Author-email: sascha.eichstaedt@ptb.de
 License: UNKNOWN
-Download-URL: https://github.com/PTB-M4D/PyDynamic/releases/download/v2.4.2/PyDynamic-2.4.2.tar.gz
-Project-URL: Documentation, https://pydynamic.readthedocs.io/en/v2.4.2/
-Project-URL: Source, https://github.com/PTB-M4D/PyDynamic/tree/v2.4.2/
+Project-URL: Documentation, https://pydynamic.readthedocs.io/en/v2.5.0/
+Project-URL: Source, https://github.com/PTB-M4D/PyDynamic/tree/v2.5.0/
 Project-URL: Tracker, https://github.com/PTB-M4D/PyDynamic/issues
 Keywords: measurement uncertainty,dynamic measurements,metrology,GUM
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Topic :: Utilities
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
```

#### html2text {}

```diff
@@ -1,15 +1,15 @@
-Metadata-Version: 2.1 Name: PyDynamic Version: 2.4.2 Summary: A software
+Metadata-Version: 2.1 Name: PyDynamic Version: 2.5.0 Summary: A software
 package for the analysis of dynamic measurements Home-page: https://ptb-
-m4d.github.io/PyDynamic/ Author: Sascha EichstÃ¤dt, Maximilian Gruber, BjÃ¶rn
-Ludwig, Thomas Bruns, Martin Weber Author-email: sascha.eichstaedt@ptb.de
-License: UNKNOWN Download-URL: https://github.com/PTB-M4D/PyDynamic/releases/
-download/v2.4.2/PyDynamic-2.4.2.tar.gz Project-URL: Documentation, https://
-pydynamic.readthedocs.io/en/v2.4.2/ Project-URL: Source, https://github.com/
-PTB-M4D/PyDynamic/tree/v2.4.2/ Project-URL: Tracker, https://github.com/PTB-
+m4d.github.io/PyDynamic/ Download-URL: https://github.com/PTB-M4D/PyDynamic/
+releases/download/v2.5.0/PyDynamic-2.5.0.tar.gz Author: Sascha EichstÃ¤dt,
+Maximilian Gruber, BjÃ¶rn Ludwig, Thomas Bruns, Martin Weber Author-email:
+sascha.eichstaedt@ptb.de License: UNKNOWN Project-URL: Documentation, https://
+pydynamic.readthedocs.io/en/v2.5.0/ Project-URL: Source, https://github.com/
+PTB-M4D/PyDynamic/tree/v2.5.0/ Project-URL: Tracker, https://github.com/PTB-
 M4D/PyDynamic/issues Keywords: measurement uncertainty,dynamic
 measurements,metrology,GUM Platform: UNKNOWN Classifier: Development Status ::
 4 - Beta Classifier: Topic :: Utilities Classifier: Topic :: Scientific/
 Engineering Classifier: Topic :: Software Development :: Libraries :: Python
 Modules Classifier: Intended Audience :: Education Classifier: Intended
 Audience :: Science/Research Classifier: License :: OSI Approved :: GNU Lesser
 General Public License v3 or later (LGPLv3+) Classifier: Programming Language
```

### Comparing `PyDynamic-2.4.2/README.md` & `PyDynamic-2.5.0/README.md`

 * *Files identical despite different names*

### Comparing `PyDynamic-2.4.2/licence.txt` & `PyDynamic-2.5.0/licence.txt`

 * *Files identical despite different names*

### Comparing `PyDynamic-2.4.2/requirements/dev-requirements-py310.txt` & `PyDynamic-2.5.0/requirements/dev-requirements-py310.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,409 +1,424 @@
 #
 # This file is autogenerated by pip-compile with Python 3.10
 # by the following command:
 #
 #    pip-compile --output-file=requirements/dev-requirements-py310.txt requirements/dev-requirements-py310.in
 #
 -e file:.
-    # via -r requirements/dev-requirements.in
-alabaster==0.7.13
+    # via file:///-
+alabaster==0.7.16
     # via sphinx
-anyio==3.7.1
-    # via jupyter-server
-argon2-cffi==21.3.0
+anyio==4.3.0
+    # via
+    #   httpx
+    #   jupyter-server
+argon2-cffi==23.1.0
     # via jupyter-server
 argon2-cffi-bindings==21.2.0
     # via argon2-cffi
-arrow==1.2.3
+arrow==1.3.0
     # via isoduration
-asttokens==2.2.1
+asttokens==2.4.1
     # via stack-data
 async-lru==2.0.4
     # via jupyterlab
-attrs==23.1.0
+attrs==23.2.0
     # via
     #   hypothesis
     #   jsonschema
     #   referencing
-babel==2.12.1
+babel==2.14.0
     # via
     #   jupyterlab-server
     #   sphinx
-backcall==0.2.0
-    # via ipython
-beautifulsoup4==4.12.2
+beautifulsoup4==4.12.3
     # via nbconvert
-black[jupyter]==23.7.0
+black[jupyter]==24.3.0
     # via pydynamic
-bleach==6.0.0
-    # via
-    #   nbconvert
-    #   readme-renderer
-cachetools==5.3.1
+bleach==6.1.0
+    # via nbconvert
+cachetools==5.3.3
     # via tox
-certifi==2023.7.22
-    # via requests
-cffi==1.15.1
+certifi==2024.2.2
+    # via
+    #   httpcore
+    #   httpx
+    #   requests
+cffi==1.16.0
     # via
     #   argon2-cffi-bindings
     #   cryptography
-chardet==5.1.0
+chardet==5.2.0
     # via tox
-charset-normalizer==3.2.0
+charset-normalizer==3.3.2
     # via requests
-click==8.1.6
+click==8.1.7
     # via
     #   black
     #   click-log
     #   python-semantic-release
 click-log==0.4.0
     # via python-semantic-release
 colorama==0.4.6
     # via
     #   tox
     #   twine
-comm==0.1.3
+comm==0.2.2
     # via ipykernel
-contourpy==1.1.0
+contourpy==1.2.0
     # via
     #   -c requirements/requirements-py310.txt
     #   matplotlib
-coverage[toml]==7.2.7
+coverage[toml]==7.4.4
     # via pytest-cov
-cryptography==41.0.2
+cryptography==42.0.5
     # via secretstorage
-cycler==0.11.0
+cycler==0.12.1
     # via
     #   -c requirements/requirements-py310.txt
     #   matplotlib
-debugpy==1.6.7
+debugpy==1.8.1
     # via ipykernel
 decorator==5.1.1
     # via ipython
 defusedxml==0.7.1
     # via nbconvert
-distlib==0.3.7
+distlib==0.3.8
     # via virtualenv
-docutils==0.18.1
+docutils==0.20.1
     # via
     #   myst-parser
     #   nbsphinx
     #   readme-renderer
     #   sphinx
     #   sphinx-rtd-theme
 dotty-dict==1.3.1
     # via python-semantic-release
-exceptiongroup==1.1.2
+exceptiongroup==1.2.0
     # via
     #   anyio
     #   hypothesis
+    #   ipython
     #   pytest
-executing==1.2.0
+executing==2.0.1
     # via stack-data
-fastjsonschema==2.18.0
+fastjsonschema==2.19.1
     # via nbformat
-filelock==3.12.2
+filelock==3.13.3
     # via
     #   tox
     #   virtualenv
-fonttools==4.41.1
+fonttools==4.50.0
     # via
     #   -c requirements/requirements-py310.txt
     #   matplotlib
 fqdn==1.5.1
     # via jsonschema
-future==0.18.3
+future==1.0.0
     # via
     #   -c requirements/requirements-py310.txt
     #   uncertainties
-gitdb==4.0.10
+gitdb==4.0.11
     # via gitpython
-gitpython==3.1.32
+gitpython==3.1.43
     # via python-semantic-release
-hypothesis==6.82.0
+h11==0.14.0
+    # via httpcore
+httpcore==1.0.5
+    # via httpx
+httpx==0.27.0
+    # via jupyterlab
+hypothesis==6.100.0
     # via pydynamic
-idna==3.4
+idna==3.6
     # via
     #   anyio
+    #   httpx
     #   jsonschema
     #   requests
 imagesize==1.4.1
     # via sphinx
-importlib-metadata==6.8.0
+importlib-metadata==7.1.0
     # via
     #   keyring
     #   twine
 iniconfig==2.0.0
     # via pytest
 invoke==2.2.0
     # via python-semantic-release
-ipykernel==6.25.0
+ipykernel==6.29.4
     # via
     #   jupyterlab
     #   pydynamic
-ipython==8.14.0
+ipython==8.23.0
     # via
     #   black
     #   ipykernel
     #   pydynamic
 isoduration==20.11.0
     # via jsonschema
-jaraco-classes==3.3.0
+jaraco-classes==3.4.0
+    # via keyring
+jaraco-context==4.3.0
+    # via keyring
+jaraco-functools==4.0.0
     # via keyring
-jedi==0.19.0
+jedi==0.19.1
     # via ipython
 jeepney==0.8.0
     # via
     #   keyring
     #   secretstorage
-jinja2==3.1.2
+jinja2==3.1.3
     # via
     #   jupyter-server
     #   jupyterlab
     #   jupyterlab-server
     #   myst-parser
     #   nbconvert
     #   nbsphinx
     #   sphinx
-json5==0.9.14
+json5==0.9.24
     # via jupyterlab-server
 jsonpointer==2.4
     # via jsonschema
-jsonschema[format-nongpl]==4.18.4
+jsonschema[format-nongpl]==4.21.1
     # via
     #   jupyter-events
     #   jupyterlab-server
     #   nbformat
-jsonschema-specifications==2023.7.1
+jsonschema-specifications==2023.12.1
     # via jsonschema
-jupyter-client==8.3.0
+jupyter-client==8.6.1
     # via
     #   ipykernel
     #   jupyter-server
     #   nbclient
-jupyter-core==5.3.1
+jupyter-core==5.7.2
     # via
     #   ipykernel
     #   jupyter-client
     #   jupyter-server
     #   jupyterlab
     #   nbclient
     #   nbconvert
     #   nbformat
-jupyter-events==0.7.0
+jupyter-events==0.10.0
     # via jupyter-server
-jupyter-lsp==2.2.0
+jupyter-lsp==2.2.4
     # via jupyterlab
-jupyter-server==2.7.0
+jupyter-server==2.13.0
     # via
     #   jupyter-lsp
     #   jupyterlab
     #   jupyterlab-server
     #   notebook
     #   notebook-shim
-jupyter-server-terminals==0.4.4
+jupyter-server-terminals==0.5.3
     # via jupyter-server
-jupyterlab==4.0.3
+jupyterlab==4.1.5
     # via notebook
-jupyterlab-pygments==0.2.2
+jupyterlab-pygments==0.3.0
     # via nbconvert
-jupyterlab-server==2.24.0
+jupyterlab-server==2.25.4
     # via
     #   jupyterlab
     #   notebook
-keyring==24.2.0
+keyring==25.0.0
     # via twine
-kiwisolver==1.4.4
+kiwisolver==1.4.5
     # via
     #   -c requirements/requirements-py310.txt
     #   matplotlib
 markdown-it-py==3.0.0
     # via
     #   mdit-py-plugins
     #   myst-parser
-markupsafe==2.1.3
+markupsafe==2.1.5
     # via
     #   jinja2
     #   nbconvert
-matplotlib==3.7.2
+matplotlib==3.8.3
     # via
     #   -c requirements/requirements-py310.txt
     #   pydynamic
 matplotlib-inline==0.1.6
     # via
     #   ipykernel
     #   ipython
 mdit-py-plugins==0.4.0
     # via myst-parser
 mdurl==0.1.2
     # via markdown-it-py
-mistune==3.0.1
+mistune==3.0.2
     # via nbconvert
-more-itertools==10.0.0
-    # via jaraco-classes
+more-itertools==10.2.0
+    # via
+    #   jaraco-classes
+    #   jaraco-functools
 mpmath==1.3.0
     # via
     #   -c requirements/requirements-py310.txt
     #   sympy
 mypy-extensions==1.0.0
     # via black
 myst-parser==2.0.0
     # via pydynamic
-nbclient==0.8.0
+nbclient==0.10.0
     # via nbconvert
-nbconvert==7.7.3
+nbconvert==7.16.3
     # via
     #   jupyter-server
     #   nbsphinx
-nbformat==5.9.2
+nbformat==5.10.3
     # via
     #   jupyter-server
     #   nbclient
     #   nbconvert
     #   nbsphinx
-nbsphinx==0.9.2
+nbsphinx==0.9.3
     # via pydynamic
-nest-asyncio==1.5.7
+nest-asyncio==1.6.0
     # via ipykernel
-notebook==7.0.1
+nh3==0.2.17
+    # via readme-renderer
+notebook==7.1.2
     # via pydynamic
-notebook-shim==0.2.3
+notebook-shim==0.2.4
     # via
     #   jupyterlab
     #   notebook
-numpy==1.25.2
+numpy==1.26.4
     # via
     #   -c requirements/requirements-py310.txt
     #   contourpy
     #   matplotlib
     #   pandas
     #   pydynamic
     #   pywavelets
     #   scipy
     #   time-series-buffer
 oauthlib==3.2.2
     # via
     #   requests-oauthlib
     #   tweepy
-overrides==7.3.1
+overrides==7.7.0
     # via jupyter-server
-packaging==23.1
+packaging==24.0
     # via
     #   -c requirements/requirements-py310.txt
     #   black
     #   ipykernel
     #   jupyter-server
     #   jupyterlab
     #   jupyterlab-server
     #   matplotlib
     #   nbconvert
     #   pyproject-api
     #   pytest
     #   python-semantic-release
     #   sphinx
     #   tox
-pandas==2.0.3
+pandas==2.2.1
     # via
     #   -c requirements/requirements-py310.txt
     #   pydynamic
-pandocfilters==1.5.0
+pandocfilters==1.5.1
     # via nbconvert
 parso==0.8.3
     # via jedi
-pathspec==0.11.2
+pathspec==0.12.1
     # via black
-pexpect==4.8.0
-    # via ipython
-pickleshare==0.7.5
+pexpect==4.9.0
     # via ipython
-pillow==10.0.0
+pillow==10.2.0
     # via
     #   -c requirements/requirements-py310.txt
     #   matplotlib
-pkginfo==1.9.6
+pkginfo==1.10.0
     # via twine
-platformdirs==3.10.0
+platformdirs==4.2.0
     # via
     #   black
     #   jupyter-core
     #   tox
     #   virtualenv
-pluggy==1.2.0
+pluggy==1.4.0
     # via
     #   pytest
     #   tox
-prometheus-client==0.17.1
+prometheus-client==0.20.0
     # via jupyter-server
-prompt-toolkit==3.0.39
+prompt-toolkit==3.0.43
     # via ipython
-psutil==5.9.5
+psutil==5.9.8
     # via ipykernel
 ptyprocess==0.7.0
     # via
     #   pexpect
     #   terminado
 pure-eval==0.2.2
     # via stack-data
-pycparser==2.21
+pycparser==2.22
     # via cffi
-pygments==2.15.1
+pygments==2.17.2
     # via
     #   ipython
     #   nbconvert
     #   readme-renderer
     #   sphinx
-pyparsing==3.0.9
+pyparsing==3.1.2
     # via
     #   -c requirements/requirements-py310.txt
     #   matplotlib
-pyproject-api==1.5.3
+pyproject-api==1.6.1
     # via tox
-pytest==7.4.0
+pytest==8.1.1
     # via
     #   pydynamic
     #   pytest-cov
     #   pytest-custom-exit-code
-pytest-cov==4.1.0
+pytest-cov==5.0.0
     # via pydynamic
 pytest-custom-exit-code==0.3.0
     # via pydynamic
-python-dateutil==2.8.2
+python-dateutil==2.9.0.post0
     # via
     #   -c requirements/requirements-py310.txt
     #   arrow
     #   jupyter-client
     #   matplotlib
     #   pandas
 python-gitlab==3.15.0
     # via python-semantic-release
 python-json-logger==2.0.7
     # via jupyter-events
 python-semantic-release==7.34.6
     # via pydynamic
-pytz==2023.3
+pytz==2024.1
     # via
     #   -c requirements/requirements-py310.txt
     #   pandas
-pywavelets==1.4.1
+pywavelets==1.5.0
     # via
     #   -c requirements/requirements-py310.txt
     #   pydynamic
 pyyaml==6.0.1
     # via
     #   jupyter-events
     #   myst-parser
-pyzmq==25.1.0
+pyzmq==25.1.2
     # via
     #   ipykernel
     #   jupyter-client
     #   jupyter-server
-readme-renderer==40.0
+readme-renderer==43.0
     # via twine
-referencing==0.30.0
+referencing==0.34.0
     # via
     #   jsonschema
     #   jsonschema-specifications
     #   jupyter-events
 requests==2.31.0
     # via
     #   jupyterlab-server
@@ -426,19 +441,19 @@
     #   jupyter-events
 rfc3986==2.0.0
     # via twine
 rfc3986-validator==0.1.1
     # via
     #   jsonschema
     #   jupyter-events
-rpds-py==0.9.2
+rpds-py==0.18.0
     # via
     #   jsonschema
     #   referencing
-scipy==1.11.1
+scipy==1.12.0
     # via
     #   -c requirements/requirements-py310.txt
     #   pydynamic
 secretstorage==3.3.3
     # via keyring
 semver==2.13.0
     # via python-semantic-release
@@ -447,54 +462,56 @@
 six==1.16.0
     # via
     #   -c requirements/requirements-py310.txt
     #   asttokens
     #   bleach
     #   python-dateutil
     #   rfc3339-validator
-smmap==5.0.0
+smmap==5.0.1
     # via gitdb
-sniffio==1.3.0
-    # via anyio
+sniffio==1.3.1
+    # via
+    #   anyio
+    #   httpx
 snowballstemmer==2.2.0
     # via sphinx
 sortedcontainers==2.4.0
     # via hypothesis
-soupsieve==2.4.1
+soupsieve==2.5
     # via beautifulsoup4
-sphinx==6.2.1
+sphinx==7.2.6
     # via
     #   myst-parser
     #   nbsphinx
     #   pydynamic
     #   sphinx-rtd-theme
     #   sphinxcontrib-jquery
-sphinx-rtd-theme==1.2.2
+sphinx-rtd-theme==2.0.0
     # via pydynamic
-sphinxcontrib-applehelp==1.0.4
+sphinxcontrib-applehelp==1.0.8
     # via sphinx
-sphinxcontrib-devhelp==1.0.2
+sphinxcontrib-devhelp==1.0.6
     # via sphinx
-sphinxcontrib-htmlhelp==2.0.1
+sphinxcontrib-htmlhelp==2.0.5
     # via sphinx
 sphinxcontrib-jquery==4.1
     # via sphinx-rtd-theme
 sphinxcontrib-jsmath==1.0.1
     # via sphinx
-sphinxcontrib-qthelp==1.0.3
+sphinxcontrib-qthelp==1.0.7
     # via sphinx
-sphinxcontrib-serializinghtml==1.1.5
+sphinxcontrib-serializinghtml==1.1.10
     # via sphinx
-stack-data==0.6.2
+stack-data==0.6.3
     # via ipython
 sympy==1.12
     # via
     #   -c requirements/requirements-py310.txt
     #   pydynamic
-terminado==0.17.1
+terminado==0.18.1
     # via
     #   jupyter-server
     #   jupyter-server-terminals
 time-series-buffer==0.1.4b0
     # via
     #   -c requirements/requirements-py310.txt
     #   pydynamic
@@ -506,29 +523,29 @@
     # via
     #   black
     #   coverage
     #   jupyterlab
     #   pyproject-api
     #   pytest
     #   tox
-tomlkit==0.12.1
+tomlkit==0.12.4
     # via python-semantic-release
-tornado==6.3.2
+tornado==6.4
     # via
     #   ipykernel
     #   jupyter-client
     #   jupyter-server
     #   jupyterlab
     #   notebook
     #   terminado
-tox==4.6.4
+tox==4.14.2
     # via pydynamic
-tqdm==4.65.0
+tqdm==4.66.2
     # via twine
-traitlets==5.9.0
+traitlets==5.14.2
     # via
     #   comm
     #   ipykernel
     #   ipython
     #   jupyter-client
     #   jupyter-core
     #   jupyter-events
@@ -539,39 +556,45 @@
     #   nbconvert
     #   nbformat
     #   nbsphinx
 tweepy==4.14.0
     # via pydynamic
 twine==3.8.0
     # via python-semantic-release
-typing-extensions==4.7.1
-    # via async-lru
-tzdata==2023.3
+types-python-dateutil==2.9.0.20240316
+    # via arrow
+typing-extensions==4.10.0
+    # via
+    #   anyio
+    #   async-lru
+    #   black
+    #   ipython
+tzdata==2024.1
     # via
     #   -c requirements/requirements-py310.txt
     #   pandas
 uncertainties==3.1.7
     # via
     #   -c requirements/requirements-py310.txt
     #   time-series-buffer
 uri-template==1.3.0
     # via jsonschema
-urllib3==2.0.4
+urllib3==2.2.1
     # via
     #   requests
     #   twine
-virtualenv==20.24.2
+virtualenv==20.25.1
     # via tox
-wcwidth==0.2.6
+wcwidth==0.2.13
     # via prompt-toolkit
 webcolors==1.13
     # via jsonschema
 webencodings==0.5.1
     # via
     #   bleach
     #   tinycss2
-websocket-client==1.6.1
+websocket-client==1.7.0
     # via jupyter-server
-wheel==0.41.0
+wheel==0.43.0
     # via python-semantic-release
-zipp==3.16.2
+zipp==3.18.1
     # via importlib-metadata
```

### Comparing `PyDynamic-2.4.2/requirements/dev-requirements-py311.txt` & `PyDynamic-2.5.0/requirements/dev-requirements-py311.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,404 +1,418 @@
 #
 # This file is autogenerated by pip-compile with Python 3.11
 # by the following command:
 #
 #    pip-compile --output-file=requirements/dev-requirements-py311.txt requirements/dev-requirements-py311.in
 #
 -e file:.
-    # via -r requirements/dev-requirements.in
-alabaster==0.7.13
+    # via file:///-
+alabaster==0.7.16
     # via sphinx
-anyio==3.7.1
-    # via jupyter-server
-argon2-cffi==21.3.0
+anyio==4.3.0
+    # via
+    #   httpx
+    #   jupyter-server
+argon2-cffi==23.1.0
     # via jupyter-server
 argon2-cffi-bindings==21.2.0
     # via argon2-cffi
-arrow==1.2.3
+arrow==1.3.0
     # via isoduration
-asttokens==2.2.1
+asttokens==2.4.1
     # via stack-data
 async-lru==2.0.4
     # via jupyterlab
-attrs==23.1.0
+attrs==23.2.0
     # via
     #   hypothesis
     #   jsonschema
     #   referencing
-babel==2.12.1
+babel==2.14.0
     # via
     #   jupyterlab-server
     #   sphinx
-backcall==0.2.0
-    # via ipython
-beautifulsoup4==4.12.2
+beautifulsoup4==4.12.3
     # via nbconvert
-black[jupyter]==23.7.0
+black[jupyter]==24.3.0
     # via pydynamic
-bleach==6.0.0
-    # via
-    #   nbconvert
-    #   readme-renderer
-cachetools==5.3.1
+bleach==6.1.0
+    # via nbconvert
+cachetools==5.3.3
     # via tox
-certifi==2023.7.22
-    # via requests
-cffi==1.15.1
+certifi==2024.2.2
+    # via
+    #   httpcore
+    #   httpx
+    #   requests
+cffi==1.16.0
     # via
     #   argon2-cffi-bindings
     #   cryptography
-chardet==5.1.0
+chardet==5.2.0
     # via tox
-charset-normalizer==3.2.0
+charset-normalizer==3.3.2
     # via requests
-click==8.1.6
+click==8.1.7
     # via
     #   black
     #   click-log
     #   python-semantic-release
 click-log==0.4.0
     # via python-semantic-release
 colorama==0.4.6
     # via
     #   tox
     #   twine
-comm==0.1.3
+comm==0.2.2
     # via ipykernel
-contourpy==1.1.0
+contourpy==1.2.0
     # via
     #   -c requirements/requirements-py311.txt
     #   matplotlib
-coverage[toml]==7.2.7
+coverage[toml]==7.4.4
     # via pytest-cov
-cryptography==41.0.2
+cryptography==42.0.5
     # via secretstorage
-cycler==0.11.0
+cycler==0.12.1
     # via
     #   -c requirements/requirements-py311.txt
     #   matplotlib
-debugpy==1.6.7
+debugpy==1.8.1
     # via ipykernel
 decorator==5.1.1
     # via ipython
 defusedxml==0.7.1
     # via nbconvert
-distlib==0.3.7
+distlib==0.3.8
     # via virtualenv
-docutils==0.18.1
+docutils==0.20.1
     # via
     #   myst-parser
     #   nbsphinx
     #   readme-renderer
     #   sphinx
     #   sphinx-rtd-theme
 dotty-dict==1.3.1
     # via python-semantic-release
-executing==1.2.0
+executing==2.0.1
     # via stack-data
-fastjsonschema==2.18.0
+fastjsonschema==2.19.1
     # via nbformat
-filelock==3.12.2
+filelock==3.13.3
     # via
     #   tox
     #   virtualenv
-fonttools==4.41.1
+fonttools==4.50.0
     # via
     #   -c requirements/requirements-py311.txt
     #   matplotlib
 fqdn==1.5.1
     # via jsonschema
-future==0.18.3
+future==1.0.0
     # via
     #   -c requirements/requirements-py311.txt
     #   uncertainties
-gitdb==4.0.10
+gitdb==4.0.11
     # via gitpython
-gitpython==3.1.32
+gitpython==3.1.43
     # via python-semantic-release
-hypothesis==6.82.0
+h11==0.14.0
+    # via httpcore
+httpcore==1.0.5
+    # via httpx
+httpx==0.27.0
+    # via jupyterlab
+hypothesis==6.100.0
     # via pydynamic
-idna==3.4
+idna==3.6
     # via
     #   anyio
+    #   httpx
     #   jsonschema
     #   requests
 imagesize==1.4.1
     # via sphinx
-importlib-metadata==6.8.0
+importlib-metadata==7.1.0
     # via
     #   keyring
     #   twine
 iniconfig==2.0.0
     # via pytest
 invoke==2.2.0
     # via python-semantic-release
-ipykernel==6.25.0
+ipykernel==6.29.4
     # via
     #   jupyterlab
     #   pydynamic
-ipython==8.14.0
+ipython==8.23.0
     # via
     #   black
     #   ipykernel
     #   pydynamic
 isoduration==20.11.0
     # via jsonschema
-jaraco-classes==3.3.0
+jaraco-classes==3.4.0
+    # via keyring
+jaraco-context==4.3.0
     # via keyring
-jedi==0.19.0
+jaraco-functools==4.0.0
+    # via keyring
+jedi==0.19.1
     # via ipython
 jeepney==0.8.0
     # via
     #   keyring
     #   secretstorage
-jinja2==3.1.2
+jinja2==3.1.3
     # via
     #   jupyter-server
     #   jupyterlab
     #   jupyterlab-server
     #   myst-parser
     #   nbconvert
     #   nbsphinx
     #   sphinx
-json5==0.9.14
+json5==0.9.24
     # via jupyterlab-server
 jsonpointer==2.4
     # via jsonschema
-jsonschema[format-nongpl]==4.18.4
+jsonschema[format-nongpl]==4.21.1
     # via
     #   jupyter-events
     #   jupyterlab-server
     #   nbformat
-jsonschema-specifications==2023.7.1
+jsonschema-specifications==2023.12.1
     # via jsonschema
-jupyter-client==8.3.0
+jupyter-client==8.6.1
     # via
     #   ipykernel
     #   jupyter-server
     #   nbclient
-jupyter-core==5.3.1
+jupyter-core==5.7.2
     # via
     #   ipykernel
     #   jupyter-client
     #   jupyter-server
     #   jupyterlab
     #   nbclient
     #   nbconvert
     #   nbformat
-jupyter-events==0.7.0
+jupyter-events==0.10.0
     # via jupyter-server
-jupyter-lsp==2.2.0
+jupyter-lsp==2.2.4
     # via jupyterlab
-jupyter-server==2.7.0
+jupyter-server==2.13.0
     # via
     #   jupyter-lsp
     #   jupyterlab
     #   jupyterlab-server
     #   notebook
     #   notebook-shim
-jupyter-server-terminals==0.4.4
+jupyter-server-terminals==0.5.3
     # via jupyter-server
-jupyterlab==4.0.3
+jupyterlab==4.1.5
     # via notebook
-jupyterlab-pygments==0.2.2
+jupyterlab-pygments==0.3.0
     # via nbconvert
-jupyterlab-server==2.24.0
+jupyterlab-server==2.25.4
     # via
     #   jupyterlab
     #   notebook
-keyring==24.2.0
+keyring==25.0.0
     # via twine
-kiwisolver==1.4.4
+kiwisolver==1.4.5
     # via
     #   -c requirements/requirements-py311.txt
     #   matplotlib
 markdown-it-py==3.0.0
     # via
     #   mdit-py-plugins
     #   myst-parser
-markupsafe==2.1.3
+markupsafe==2.1.5
     # via
     #   jinja2
     #   nbconvert
-matplotlib==3.7.2
+matplotlib==3.8.3
     # via
     #   -c requirements/requirements-py311.txt
     #   pydynamic
 matplotlib-inline==0.1.6
     # via
     #   ipykernel
     #   ipython
 mdit-py-plugins==0.4.0
     # via myst-parser
 mdurl==0.1.2
     # via markdown-it-py
-mistune==3.0.1
+mistune==3.0.2
     # via nbconvert
-more-itertools==10.0.0
-    # via jaraco-classes
+more-itertools==10.2.0
+    # via
+    #   jaraco-classes
+    #   jaraco-functools
 mpmath==1.3.0
     # via
     #   -c requirements/requirements-py311.txt
     #   sympy
 mypy-extensions==1.0.0
     # via black
 myst-parser==2.0.0
     # via pydynamic
-nbclient==0.8.0
+nbclient==0.10.0
     # via nbconvert
-nbconvert==7.7.3
+nbconvert==7.16.3
     # via
     #   jupyter-server
     #   nbsphinx
-nbformat==5.9.2
+nbformat==5.10.3
     # via
     #   jupyter-server
     #   nbclient
     #   nbconvert
     #   nbsphinx
-nbsphinx==0.9.2
+nbsphinx==0.9.3
     # via pydynamic
-nest-asyncio==1.5.7
+nest-asyncio==1.6.0
     # via ipykernel
-notebook==7.0.1
+nh3==0.2.17
+    # via readme-renderer
+notebook==7.1.2
     # via pydynamic
-notebook-shim==0.2.3
+notebook-shim==0.2.4
     # via
     #   jupyterlab
     #   notebook
-numpy==1.25.2
+numpy==1.26.4
     # via
     #   -c requirements/requirements-py311.txt
     #   contourpy
     #   matplotlib
     #   pandas
     #   pydynamic
     #   pywavelets
     #   scipy
     #   time-series-buffer
 oauthlib==3.2.2
     # via
     #   requests-oauthlib
     #   tweepy
-overrides==7.3.1
+overrides==7.7.0
     # via jupyter-server
-packaging==23.1
+packaging==24.0
     # via
     #   -c requirements/requirements-py311.txt
     #   black
     #   ipykernel
     #   jupyter-server
     #   jupyterlab
     #   jupyterlab-server
     #   matplotlib
     #   nbconvert
     #   pyproject-api
     #   pytest
     #   python-semantic-release
     #   sphinx
     #   tox
-pandas==2.0.3
+pandas==2.2.1
     # via
     #   -c requirements/requirements-py311.txt
     #   pydynamic
-pandocfilters==1.5.0
+pandocfilters==1.5.1
     # via nbconvert
 parso==0.8.3
     # via jedi
-pathspec==0.11.2
+pathspec==0.12.1
     # via black
-pexpect==4.8.0
+pexpect==4.9.0
     # via ipython
-pickleshare==0.7.5
-    # via ipython
-pillow==10.0.0
+pillow==10.2.0
     # via
     #   -c requirements/requirements-py311.txt
     #   matplotlib
-pkginfo==1.9.6
+pkginfo==1.10.0
     # via twine
-platformdirs==3.10.0
+platformdirs==4.2.0
     # via
     #   black
     #   jupyter-core
     #   tox
     #   virtualenv
-pluggy==1.2.0
+pluggy==1.4.0
     # via
     #   pytest
     #   tox
-prometheus-client==0.17.1
+prometheus-client==0.20.0
     # via jupyter-server
-prompt-toolkit==3.0.39
+prompt-toolkit==3.0.43
     # via ipython
-psutil==5.9.5
+psutil==5.9.8
     # via ipykernel
 ptyprocess==0.7.0
     # via
     #   pexpect
     #   terminado
 pure-eval==0.2.2
     # via stack-data
-pycparser==2.21
+pycparser==2.22
     # via cffi
-pygments==2.15.1
+pygments==2.17.2
     # via
     #   ipython
     #   nbconvert
     #   readme-renderer
     #   sphinx
-pyparsing==3.0.9
+pyparsing==3.1.2
     # via
     #   -c requirements/requirements-py311.txt
     #   matplotlib
-pyproject-api==1.5.3
+pyproject-api==1.6.1
     # via tox
-pytest==7.4.0
+pytest==8.1.1
     # via
     #   pydynamic
     #   pytest-cov
     #   pytest-custom-exit-code
-pytest-cov==4.1.0
+pytest-cov==5.0.0
     # via pydynamic
 pytest-custom-exit-code==0.3.0
     # via pydynamic
-python-dateutil==2.8.2
+python-dateutil==2.9.0.post0
     # via
     #   -c requirements/requirements-py311.txt
     #   arrow
     #   jupyter-client
     #   matplotlib
     #   pandas
 python-gitlab==3.15.0
     # via python-semantic-release
 python-json-logger==2.0.7
     # via jupyter-events
 python-semantic-release==7.34.6
     # via pydynamic
-pytz==2023.3
+pytz==2024.1
     # via
     #   -c requirements/requirements-py311.txt
     #   pandas
-pywavelets==1.4.1
+pywavelets==1.5.0
     # via
     #   -c requirements/requirements-py311.txt
     #   pydynamic
 pyyaml==6.0.1
     # via
     #   jupyter-events
     #   myst-parser
-pyzmq==25.1.0
+pyzmq==25.1.2
     # via
     #   ipykernel
     #   jupyter-client
     #   jupyter-server
-readme-renderer==40.0
+readme-renderer==43.0
     # via twine
-referencing==0.30.0
+referencing==0.34.0
     # via
     #   jsonschema
     #   jsonschema-specifications
     #   jupyter-events
 requests==2.31.0
     # via
     #   jupyterlab-server
@@ -421,19 +435,19 @@
     #   jupyter-events
 rfc3986==2.0.0
     # via twine
 rfc3986-validator==0.1.1
     # via
     #   jsonschema
     #   jupyter-events
-rpds-py==0.9.2
+rpds-py==0.18.0
     # via
     #   jsonschema
     #   referencing
-scipy==1.11.1
+scipy==1.12.0
     # via
     #   -c requirements/requirements-py311.txt
     #   pydynamic
 secretstorage==3.3.3
     # via keyring
 semver==2.13.0
     # via python-semantic-release
@@ -442,80 +456,82 @@
 six==1.16.0
     # via
     #   -c requirements/requirements-py311.txt
     #   asttokens
     #   bleach
     #   python-dateutil
     #   rfc3339-validator
-smmap==5.0.0
+smmap==5.0.1
     # via gitdb
-sniffio==1.3.0
-    # via anyio
+sniffio==1.3.1
+    # via
+    #   anyio
+    #   httpx
 snowballstemmer==2.2.0
     # via sphinx
 sortedcontainers==2.4.0
     # via hypothesis
-soupsieve==2.4.1
+soupsieve==2.5
     # via beautifulsoup4
-sphinx==6.2.1
+sphinx==7.2.6
     # via
     #   myst-parser
     #   nbsphinx
     #   pydynamic
     #   sphinx-rtd-theme
     #   sphinxcontrib-jquery
-sphinx-rtd-theme==1.2.2
+sphinx-rtd-theme==2.0.0
     # via pydynamic
-sphinxcontrib-applehelp==1.0.4
+sphinxcontrib-applehelp==1.0.8
     # via sphinx
-sphinxcontrib-devhelp==1.0.2
+sphinxcontrib-devhelp==1.0.6
     # via sphinx
-sphinxcontrib-htmlhelp==2.0.1
+sphinxcontrib-htmlhelp==2.0.5
     # via sphinx
 sphinxcontrib-jquery==4.1
     # via sphinx-rtd-theme
 sphinxcontrib-jsmath==1.0.1
     # via sphinx
-sphinxcontrib-qthelp==1.0.3
+sphinxcontrib-qthelp==1.0.7
     # via sphinx
-sphinxcontrib-serializinghtml==1.1.5
+sphinxcontrib-serializinghtml==1.1.10
     # via sphinx
-stack-data==0.6.2
+stack-data==0.6.3
     # via ipython
 sympy==1.12
     # via
     #   -c requirements/requirements-py311.txt
     #   pydynamic
-terminado==0.17.1
+terminado==0.18.1
     # via
     #   jupyter-server
     #   jupyter-server-terminals
 time-series-buffer==0.1.4b0
     # via
     #   -c requirements/requirements-py311.txt
     #   pydynamic
 tinycss2==1.2.1
     # via nbconvert
 tokenize-rt==5.2.0
     # via black
-tomlkit==0.12.1
+tomlkit==0.12.4
     # via python-semantic-release
-tornado==6.3.2
+tornado==6.4
     # via
     #   ipykernel
     #   jupyter-client
     #   jupyter-server
     #   jupyterlab
     #   notebook
     #   terminado
-tox==4.6.4
+tox==4.14.2
     # via pydynamic
-tqdm==4.65.0
+tqdm==4.66.2
     # via twine
-traitlets==5.9.0
+traitlets==5.14.2
     # via
     #   comm
     #   ipykernel
     #   ipython
     #   jupyter-client
     #   jupyter-core
     #   jupyter-events
@@ -526,37 +542,41 @@
     #   nbconvert
     #   nbformat
     #   nbsphinx
 tweepy==4.14.0
     # via pydynamic
 twine==3.8.0
     # via python-semantic-release
-tzdata==2023.3
+types-python-dateutil==2.9.0.20240316
+    # via arrow
+typing-extensions==4.10.0
+    # via ipython
+tzdata==2024.1
     # via
     #   -c requirements/requirements-py311.txt
     #   pandas
 uncertainties==3.1.7
     # via
     #   -c requirements/requirements-py311.txt
     #   time-series-buffer
 uri-template==1.3.0
     # via jsonschema
-urllib3==2.0.4
+urllib3==2.2.1
     # via
     #   requests
     #   twine
-virtualenv==20.24.2
+virtualenv==20.25.1
     # via tox
-wcwidth==0.2.6
+wcwidth==0.2.13
     # via prompt-toolkit
 webcolors==1.13
     # via jsonschema
 webencodings==0.5.1
     # via
     #   bleach
     #   tinycss2
-websocket-client==1.6.1
+websocket-client==1.7.0
     # via jupyter-server
-wheel==0.41.0
+wheel==0.43.0
     # via python-semantic-release
-zipp==3.16.2
+zipp==3.18.1
     # via importlib-metadata
```

### Comparing `PyDynamic-2.4.2/requirements/dev-requirements-py38.txt` & `PyDynamic-2.5.0/requirements/dev-requirements-py38.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,292 +1,309 @@
 #
 # This file is autogenerated by pip-compile with Python 3.8
 # by the following command:
 #
 #    pip-compile --output-file=requirements/dev-requirements-py38.txt requirements/dev-requirements-py38.in
 #
 -e file:.
-    # via -r requirements/dev-requirements.in
+    # via file:///-
 alabaster==0.7.13
     # via sphinx
-anyio==3.7.1
-    # via jupyter-server
-argon2-cffi==21.3.0
+anyio==4.3.0
+    # via
+    #   httpx
+    #   jupyter-server
+argon2-cffi==23.1.0
     # via jupyter-server
 argon2-cffi-bindings==21.2.0
     # via argon2-cffi
-arrow==1.2.3
+arrow==1.3.0
     # via isoduration
-asttokens==2.2.1
+asttokens==2.4.1
     # via stack-data
 async-lru==2.0.4
     # via jupyterlab
-attrs==23.1.0
+attrs==23.2.0
     # via
     #   hypothesis
     #   jsonschema
     #   referencing
-babel==2.12.1
+babel==2.14.0
     # via
     #   jupyterlab-server
     #   sphinx
 backcall==0.2.0
     # via ipython
-beautifulsoup4==4.12.2
+beautifulsoup4==4.12.3
     # via nbconvert
-black[jupyter]==23.7.0
+black[jupyter]==24.3.0
     # via pydynamic
-bleach==6.0.0
-    # via
-    #   nbconvert
-    #   readme-renderer
-cachetools==5.3.1
+bleach==6.1.0
+    # via nbconvert
+cachetools==5.3.3
     # via tox
-certifi==2023.7.22
-    # via requests
-cffi==1.15.1
+certifi==2024.2.2
+    # via
+    #   httpcore
+    #   httpx
+    #   requests
+cffi==1.16.0
     # via
     #   argon2-cffi-bindings
     #   cryptography
-chardet==5.1.0
+chardet==5.2.0
     # via tox
-charset-normalizer==3.2.0
+charset-normalizer==3.3.2
     # via requests
-click==8.1.6
+click==8.1.7
     # via
     #   black
     #   click-log
     #   python-semantic-release
 click-log==0.4.0
     # via python-semantic-release
 colorama==0.4.6
     # via
     #   tox
     #   twine
-comm==0.1.3
+comm==0.2.2
     # via ipykernel
-contourpy==1.1.0
+contourpy==1.1.1
     # via
     #   -c requirements/requirements-py38.txt
     #   matplotlib
-coverage[toml]==7.2.7
+coverage[toml]==7.4.4
     # via pytest-cov
-cryptography==41.0.2
+cryptography==42.0.5
     # via secretstorage
-cycler==0.11.0
+cycler==0.12.1
     # via
     #   -c requirements/requirements-py38.txt
     #   matplotlib
-debugpy==1.6.7
+debugpy==1.8.1
     # via ipykernel
 decorator==5.1.1
     # via ipython
 defusedxml==0.7.1
     # via nbconvert
-distlib==0.3.7
+distlib==0.3.8
     # via virtualenv
-docutils==0.18.1
+docutils==0.20.1
     # via
     #   myst-parser
     #   nbsphinx
     #   readme-renderer
     #   sphinx
     #   sphinx-rtd-theme
 dotty-dict==1.3.1
     # via python-semantic-release
-exceptiongroup==1.1.2
+exceptiongroup==1.2.0
     # via
     #   anyio
     #   hypothesis
     #   pytest
-executing==1.2.0
+executing==2.0.1
     # via stack-data
-fastjsonschema==2.18.0
+fastjsonschema==2.19.1
     # via nbformat
-filelock==3.12.2
+filelock==3.13.3
     # via
     #   tox
     #   virtualenv
-fonttools==4.41.1
+fonttools==4.50.0
     # via
     #   -c requirements/requirements-py38.txt
     #   matplotlib
 fqdn==1.5.1
     # via jsonschema
-future==0.18.3
+future==1.0.0
     # via
     #   -c requirements/requirements-py38.txt
     #   uncertainties
-gitdb==4.0.10
+gitdb==4.0.11
     # via gitpython
-gitpython==3.1.32
+gitpython==3.1.43
     # via python-semantic-release
-hypothesis==6.82.0
+h11==0.14.0
+    # via httpcore
+httpcore==1.0.5
+    # via httpx
+httpx==0.27.0
+    # via jupyterlab
+hypothesis==6.100.0
     # via pydynamic
-idna==3.4
+idna==3.6
     # via
     #   anyio
+    #   httpx
     #   jsonschema
     #   requests
 imagesize==1.4.1
     # via sphinx
-importlib-metadata==6.8.0
+importlib-metadata==7.1.0
     # via
     #   jupyter-client
     #   jupyter-lsp
     #   jupyterlab
     #   jupyterlab-server
     #   keyring
     #   nbconvert
     #   sphinx
     #   twine
-importlib-resources==6.0.0
+importlib-resources==6.4.0
     # via
     #   -c requirements/requirements-py38.txt
     #   jsonschema
     #   jsonschema-specifications
     #   jupyterlab
     #   keyring
     #   matplotlib
-    #   notebook
 iniconfig==2.0.0
     # via pytest
 invoke==2.2.0
     # via python-semantic-release
-ipykernel==6.25.0
+ipykernel==6.29.4
     # via
     #   jupyterlab
     #   pydynamic
-ipython==8.12.2
+ipython==8.12.3
     # via
     #   black
     #   ipykernel
     #   pydynamic
 isoduration==20.11.0
     # via jsonschema
-jaraco-classes==3.3.0
+jaraco-classes==3.4.0
+    # via keyring
+jaraco-context==4.3.0
+    # via keyring
+jaraco-functools==4.0.0
     # via keyring
-jedi==0.19.0
+jedi==0.19.1
     # via ipython
 jeepney==0.8.0
     # via
     #   keyring
     #   secretstorage
-jinja2==3.1.2
+jinja2==3.1.3
     # via
     #   jupyter-server
     #   jupyterlab
     #   jupyterlab-server
     #   myst-parser
     #   nbconvert
     #   nbsphinx
     #   sphinx
-json5==0.9.14
+json5==0.9.24
     # via jupyterlab-server
 jsonpointer==2.4
     # via jsonschema
-jsonschema[format-nongpl]==4.18.4
+jsonschema[format-nongpl]==4.21.1
     # via
     #   jupyter-events
     #   jupyterlab-server
     #   nbformat
-jsonschema-specifications==2023.7.1
+jsonschema-specifications==2023.12.1
     # via jsonschema
-jupyter-client==8.3.0
+jupyter-client==8.6.1
     # via
     #   ipykernel
     #   jupyter-server
     #   nbclient
-jupyter-core==5.3.1
+jupyter-core==5.7.2
     # via
     #   ipykernel
     #   jupyter-client
     #   jupyter-server
     #   jupyterlab
     #   nbclient
     #   nbconvert
     #   nbformat
-jupyter-events==0.7.0
+jupyter-events==0.10.0
     # via jupyter-server
-jupyter-lsp==2.2.0
+jupyter-lsp==2.2.4
     # via jupyterlab
-jupyter-server==2.7.0
+jupyter-server==2.13.0
     # via
     #   jupyter-lsp
     #   jupyterlab
     #   jupyterlab-server
     #   notebook
     #   notebook-shim
-jupyter-server-terminals==0.4.4
+jupyter-server-terminals==0.5.3
     # via jupyter-server
-jupyterlab==4.0.3
+jupyterlab==4.1.5
     # via notebook
-jupyterlab-pygments==0.2.2
+jupyterlab-pygments==0.3.0
     # via nbconvert
-jupyterlab-server==2.24.0
+jupyterlab-server==2.25.4
     # via
     #   jupyterlab
     #   notebook
-keyring==24.2.0
+keyring==25.0.0
     # via twine
-kiwisolver==1.4.4
+kiwisolver==1.4.5
     # via
     #   -c requirements/requirements-py38.txt
     #   matplotlib
 markdown-it-py==3.0.0
     # via
     #   mdit-py-plugins
     #   myst-parser
-markupsafe==2.1.3
+markupsafe==2.1.5
     # via
     #   jinja2
     #   nbconvert
-matplotlib==3.7.2
+matplotlib==3.7.5
     # via
     #   -c requirements/requirements-py38.txt
     #   pydynamic
 matplotlib-inline==0.1.6
     # via
     #   ipykernel
     #   ipython
 mdit-py-plugins==0.4.0
     # via myst-parser
 mdurl==0.1.2
     # via markdown-it-py
-mistune==3.0.1
+mistune==3.0.2
     # via nbconvert
-more-itertools==10.0.0
-    # via jaraco-classes
+more-itertools==10.2.0
+    # via
+    #   jaraco-classes
+    #   jaraco-functools
 mpmath==1.3.0
     # via
     #   -c requirements/requirements-py38.txt
     #   sympy
 mypy-extensions==1.0.0
     # via black
 myst-parser==2.0.0
     # via pydynamic
-nbclient==0.8.0
+nbclient==0.10.0
     # via nbconvert
-nbconvert==7.7.3
+nbconvert==7.16.3
     # via
     #   jupyter-server
     #   nbsphinx
-nbformat==5.9.2
+nbformat==5.10.3
     # via
     #   jupyter-server
     #   nbclient
     #   nbconvert
     #   nbsphinx
-nbsphinx==0.9.2
+nbsphinx==0.9.3
     # via pydynamic
-nest-asyncio==1.5.7
+nest-asyncio==1.6.0
     # via ipykernel
-notebook==7.0.1
+nh3==0.2.17
+    # via readme-renderer
+notebook==7.1.2
     # via pydynamic
-notebook-shim==0.2.3
+notebook-shim==0.2.4
     # via
     #   jupyterlab
     #   notebook
 numpy==1.24.4
     # via
     #   -c requirements/requirements-py38.txt
     #   contourpy
@@ -296,17 +313,17 @@
     #   pywavelets
     #   scipy
     #   time-series-buffer
 oauthlib==3.2.2
     # via
     #   requests-oauthlib
     #   tweepy
-overrides==7.3.1
+overrides==7.7.0
     # via jupyter-server
-packaging==23.1
+packaging==24.0
     # via
     #   -c requirements/requirements-py38.txt
     #   black
     #   ipykernel
     #   jupyter-server
     #   jupyterlab
     #   jupyterlab-server
@@ -317,111 +334,111 @@
     #   python-semantic-release
     #   sphinx
     #   tox
 pandas==2.0.3
     # via
     #   -c requirements/requirements-py38.txt
     #   pydynamic
-pandocfilters==1.5.0
+pandocfilters==1.5.1
     # via nbconvert
 parso==0.8.3
     # via jedi
-pathspec==0.11.2
+pathspec==0.12.1
     # via black
-pexpect==4.8.0
+pexpect==4.9.0
     # via ipython
 pickleshare==0.7.5
     # via ipython
-pillow==10.0.0
+pillow==10.2.0
     # via
     #   -c requirements/requirements-py38.txt
     #   matplotlib
-pkginfo==1.9.6
+pkginfo==1.10.0
     # via twine
 pkgutil-resolve-name==1.3.10
     # via jsonschema
-platformdirs==3.10.0
+platformdirs==4.2.0
     # via
     #   black
     #   jupyter-core
     #   tox
     #   virtualenv
-pluggy==1.2.0
+pluggy==1.4.0
     # via
     #   pytest
     #   tox
-prometheus-client==0.17.1
+prometheus-client==0.20.0
     # via jupyter-server
-prompt-toolkit==3.0.39
+prompt-toolkit==3.0.43
     # via ipython
-psutil==5.9.5
+psutil==5.9.8
     # via ipykernel
 ptyprocess==0.7.0
     # via
     #   pexpect
     #   terminado
 pure-eval==0.2.2
     # via stack-data
-pycparser==2.21
+pycparser==2.22
     # via cffi
-pygments==2.15.1
+pygments==2.17.2
     # via
     #   ipython
     #   nbconvert
     #   readme-renderer
     #   sphinx
-pyparsing==3.0.9
+pyparsing==3.1.2
     # via
     #   -c requirements/requirements-py38.txt
     #   matplotlib
-pyproject-api==1.5.3
+pyproject-api==1.6.1
     # via tox
-pytest==7.4.0
+pytest==8.1.1
     # via
     #   pydynamic
     #   pytest-cov
     #   pytest-custom-exit-code
-pytest-cov==4.1.0
+pytest-cov==5.0.0
     # via pydynamic
 pytest-custom-exit-code==0.3.0
     # via pydynamic
-python-dateutil==2.8.2
+python-dateutil==2.9.0.post0
     # via
     #   -c requirements/requirements-py38.txt
     #   arrow
     #   jupyter-client
     #   matplotlib
     #   pandas
 python-gitlab==3.15.0
     # via python-semantic-release
 python-json-logger==2.0.7
     # via jupyter-events
 python-semantic-release==7.34.6
     # via pydynamic
-pytz==2023.3
+pytz==2024.1
     # via
     #   -c requirements/requirements-py38.txt
     #   babel
     #   pandas
 pywavelets==1.4.1
     # via
     #   -c requirements/requirements-py38.txt
     #   pydynamic
 pyyaml==6.0.1
     # via
     #   jupyter-events
     #   myst-parser
-pyzmq==25.1.0
+pyzmq==25.1.2
     # via
     #   ipykernel
     #   jupyter-client
     #   jupyter-server
-readme-renderer==40.0
+readme-renderer==43.0
     # via twine
-referencing==0.30.0
+referencing==0.34.0
     # via
     #   jsonschema
     #   jsonschema-specifications
     #   jupyter-events
 requests==2.31.0
     # via
     #   jupyterlab-server
@@ -444,15 +461,15 @@
     #   jupyter-events
 rfc3986==2.0.0
     # via twine
 rfc3986-validator==0.1.1
     # via
     #   jsonschema
     #   jupyter-events
-rpds-py==0.9.2
+rpds-py==0.18.0
     # via
     #   jsonschema
     #   referencing
 scipy==1.10.1
     # via
     #   -c requirements/requirements-py38.txt
     #   pydynamic
@@ -465,32 +482,34 @@
 six==1.16.0
     # via
     #   -c requirements/requirements-py38.txt
     #   asttokens
     #   bleach
     #   python-dateutil
     #   rfc3339-validator
-smmap==5.0.0
+smmap==5.0.1
     # via gitdb
-sniffio==1.3.0
-    # via anyio
+sniffio==1.3.1
+    # via
+    #   anyio
+    #   httpx
 snowballstemmer==2.2.0
     # via sphinx
 sortedcontainers==2.4.0
     # via hypothesis
-soupsieve==2.4.1
+soupsieve==2.5
     # via beautifulsoup4
-sphinx==6.2.1
+sphinx==7.1.2
     # via
     #   myst-parser
     #   nbsphinx
     #   pydynamic
     #   sphinx-rtd-theme
     #   sphinxcontrib-jquery
-sphinx-rtd-theme==1.2.2
+sphinx-rtd-theme==2.0.0
     # via pydynamic
 sphinxcontrib-applehelp==1.0.4
     # via sphinx
 sphinxcontrib-devhelp==1.0.2
     # via sphinx
 sphinxcontrib-htmlhelp==2.0.1
     # via sphinx
@@ -498,21 +517,21 @@
     # via sphinx-rtd-theme
 sphinxcontrib-jsmath==1.0.1
     # via sphinx
 sphinxcontrib-qthelp==1.0.3
     # via sphinx
 sphinxcontrib-serializinghtml==1.1.5
     # via sphinx
-stack-data==0.6.2
+stack-data==0.6.3
     # via ipython
 sympy==1.12
     # via
     #   -c requirements/requirements-py38.txt
     #   pydynamic
-terminado==0.17.1
+terminado==0.18.1
     # via
     #   jupyter-server
     #   jupyter-server-terminals
 time-series-buffer==0.1.4b0
     # via
     #   -c requirements/requirements-py38.txt
     #   pydynamic
@@ -524,29 +543,29 @@
     # via
     #   black
     #   coverage
     #   jupyterlab
     #   pyproject-api
     #   pytest
     #   tox
-tomlkit==0.12.1
+tomlkit==0.12.4
     # via python-semantic-release
-tornado==6.3.2
+tornado==6.4
     # via
     #   ipykernel
     #   jupyter-client
     #   jupyter-server
     #   jupyterlab
     #   notebook
     #   terminado
-tox==4.6.4
+tox==4.14.2
     # via pydynamic
-tqdm==4.65.0
+tqdm==4.66.2
     # via twine
-traitlets==5.9.0
+traitlets==5.14.2
     # via
     #   comm
     #   ipykernel
     #   ipython
     #   jupyter-client
     #   jupyter-core
     #   jupyter-events
@@ -557,45 +576,48 @@
     #   nbconvert
     #   nbformat
     #   nbsphinx
 tweepy==4.14.0
     # via pydynamic
 twine==3.8.0
     # via python-semantic-release
-typing-extensions==4.7.1
+types-python-dateutil==2.9.0.20240316
+    # via arrow
+typing-extensions==4.10.0
     # via
+    #   anyio
     #   async-lru
     #   black
     #   ipython
-tzdata==2023.3
+tzdata==2024.1
     # via
     #   -c requirements/requirements-py38.txt
     #   pandas
 uncertainties==3.1.7
     # via
     #   -c requirements/requirements-py38.txt
     #   time-series-buffer
 uri-template==1.3.0
     # via jsonschema
-urllib3==2.0.4
+urllib3==2.2.1
     # via
     #   requests
     #   twine
-virtualenv==20.24.2
+virtualenv==20.25.1
     # via tox
-wcwidth==0.2.6
+wcwidth==0.2.13
     # via prompt-toolkit
 webcolors==1.13
     # via jsonschema
 webencodings==0.5.1
     # via
     #   bleach
     #   tinycss2
-websocket-client==1.6.1
+websocket-client==1.7.0
     # via jupyter-server
-wheel==0.41.0
+wheel==0.43.0
     # via python-semantic-release
-zipp==3.16.2
+zipp==3.18.1
     # via
     #   -c requirements/requirements-py38.txt
     #   importlib-metadata
     #   importlib-resources
```

### Comparing `PyDynamic-2.4.2/requirements/dev-requirements-py39.txt` & `PyDynamic-2.5.0/requirements/dev-requirements-py39.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,419 +1,434 @@
 #
 # This file is autogenerated by pip-compile with Python 3.9
 # by the following command:
 #
 #    pip-compile --output-file=requirements/dev-requirements-py39.txt requirements/dev-requirements-py39.in
 #
 -e file:.
-    # via -r requirements/dev-requirements.in
-alabaster==0.7.13
+    # via file:///-
+alabaster==0.7.16
     # via sphinx
-anyio==3.7.1
-    # via jupyter-server
-argon2-cffi==21.3.0
+anyio==4.3.0
+    # via
+    #   httpx
+    #   jupyter-server
+argon2-cffi==23.1.0
     # via jupyter-server
 argon2-cffi-bindings==21.2.0
     # via argon2-cffi
-arrow==1.2.3
+arrow==1.3.0
     # via isoduration
-asttokens==2.2.1
+asttokens==2.4.1
     # via stack-data
 async-lru==2.0.4
     # via jupyterlab
-attrs==23.1.0
+attrs==23.2.0
     # via
     #   hypothesis
     #   jsonschema
     #   referencing
-babel==2.12.1
+babel==2.14.0
     # via
     #   jupyterlab-server
     #   sphinx
-backcall==0.2.0
-    # via ipython
-beautifulsoup4==4.12.2
+beautifulsoup4==4.12.3
     # via nbconvert
-black[jupyter]==23.7.0
+black[jupyter]==24.3.0
     # via pydynamic
-bleach==6.0.0
-    # via
-    #   nbconvert
-    #   readme-renderer
-cachetools==5.3.1
+bleach==6.1.0
+    # via nbconvert
+cachetools==5.3.3
     # via tox
-certifi==2023.7.22
-    # via requests
-cffi==1.15.1
+certifi==2024.2.2
+    # via
+    #   httpcore
+    #   httpx
+    #   requests
+cffi==1.16.0
     # via
     #   argon2-cffi-bindings
     #   cryptography
-chardet==5.1.0
+chardet==5.2.0
     # via tox
-charset-normalizer==3.2.0
+charset-normalizer==3.3.2
     # via requests
-click==8.1.6
+click==8.1.7
     # via
     #   black
     #   click-log
     #   python-semantic-release
 click-log==0.4.0
     # via python-semantic-release
 colorama==0.4.6
     # via
     #   tox
     #   twine
-comm==0.1.3
+comm==0.2.2
     # via ipykernel
-contourpy==1.1.0
+contourpy==1.2.0
     # via
     #   -c requirements/requirements-py39.txt
     #   matplotlib
-coverage[toml]==7.2.7
+coverage[toml]==7.4.4
     # via pytest-cov
-cryptography==41.0.2
+cryptography==42.0.5
     # via secretstorage
-cycler==0.11.0
+cycler==0.12.1
     # via
     #   -c requirements/requirements-py39.txt
     #   matplotlib
-debugpy==1.6.7
+debugpy==1.8.1
     # via ipykernel
 decorator==5.1.1
     # via ipython
 defusedxml==0.7.1
     # via nbconvert
-distlib==0.3.7
+distlib==0.3.8
     # via virtualenv
-docutils==0.18.1
+docutils==0.20.1
     # via
     #   myst-parser
     #   nbsphinx
     #   readme-renderer
     #   sphinx
     #   sphinx-rtd-theme
 dotty-dict==1.3.1
     # via python-semantic-release
-exceptiongroup==1.1.2
+exceptiongroup==1.2.0
     # via
     #   anyio
     #   hypothesis
+    #   ipython
     #   pytest
-executing==1.2.0
+executing==2.0.1
     # via stack-data
-fastjsonschema==2.18.0
+fastjsonschema==2.19.1
     # via nbformat
-filelock==3.12.2
+filelock==3.13.3
     # via
     #   tox
     #   virtualenv
-fonttools==4.41.1
+fonttools==4.50.0
     # via
     #   -c requirements/requirements-py39.txt
     #   matplotlib
 fqdn==1.5.1
     # via jsonschema
-future==0.18.3
+future==1.0.0
     # via
     #   -c requirements/requirements-py39.txt
     #   uncertainties
-gitdb==4.0.10
+gitdb==4.0.11
     # via gitpython
-gitpython==3.1.32
+gitpython==3.1.43
     # via python-semantic-release
-hypothesis==6.82.0
+h11==0.14.0
+    # via httpcore
+httpcore==1.0.5
+    # via httpx
+httpx==0.27.0
+    # via jupyterlab
+hypothesis==6.100.0
     # via pydynamic
-idna==3.4
+idna==3.6
     # via
     #   anyio
+    #   httpx
     #   jsonschema
     #   requests
 imagesize==1.4.1
     # via sphinx
-importlib-metadata==6.8.0
+importlib-metadata==7.1.0
     # via
     #   jupyter-client
     #   jupyter-lsp
     #   jupyterlab
     #   jupyterlab-server
     #   keyring
     #   nbconvert
     #   sphinx
     #   twine
-importlib-resources==6.0.0
+importlib-resources==6.4.0
     # via
     #   -c requirements/requirements-py39.txt
     #   matplotlib
 iniconfig==2.0.0
     # via pytest
 invoke==2.2.0
     # via python-semantic-release
-ipykernel==6.25.0
+ipykernel==6.29.4
     # via
     #   jupyterlab
     #   pydynamic
-ipython==8.14.0
+ipython==8.18.1
     # via
     #   black
     #   ipykernel
     #   pydynamic
 isoduration==20.11.0
     # via jsonschema
-jaraco-classes==3.3.0
+jaraco-classes==3.4.0
+    # via keyring
+jaraco-context==4.3.0
+    # via keyring
+jaraco-functools==4.0.0
     # via keyring
-jedi==0.19.0
+jedi==0.19.1
     # via ipython
 jeepney==0.8.0
     # via
     #   keyring
     #   secretstorage
-jinja2==3.1.2
+jinja2==3.1.3
     # via
     #   jupyter-server
     #   jupyterlab
     #   jupyterlab-server
     #   myst-parser
     #   nbconvert
     #   nbsphinx
     #   sphinx
-json5==0.9.14
+json5==0.9.24
     # via jupyterlab-server
 jsonpointer==2.4
     # via jsonschema
-jsonschema[format-nongpl]==4.18.4
+jsonschema[format-nongpl]==4.21.1
     # via
     #   jupyter-events
     #   jupyterlab-server
     #   nbformat
-jsonschema-specifications==2023.7.1
+jsonschema-specifications==2023.12.1
     # via jsonschema
-jupyter-client==8.3.0
+jupyter-client==8.6.1
     # via
     #   ipykernel
     #   jupyter-server
     #   nbclient
-jupyter-core==5.3.1
+jupyter-core==5.7.2
     # via
     #   ipykernel
     #   jupyter-client
     #   jupyter-server
     #   jupyterlab
     #   nbclient
     #   nbconvert
     #   nbformat
-jupyter-events==0.7.0
+jupyter-events==0.10.0
     # via jupyter-server
-jupyter-lsp==2.2.0
+jupyter-lsp==2.2.4
     # via jupyterlab
-jupyter-server==2.7.0
+jupyter-server==2.13.0
     # via
     #   jupyter-lsp
     #   jupyterlab
     #   jupyterlab-server
     #   notebook
     #   notebook-shim
-jupyter-server-terminals==0.4.4
+jupyter-server-terminals==0.5.3
     # via jupyter-server
-jupyterlab==4.0.3
+jupyterlab==4.1.5
     # via notebook
-jupyterlab-pygments==0.2.2
+jupyterlab-pygments==0.3.0
     # via nbconvert
-jupyterlab-server==2.24.0
+jupyterlab-server==2.25.4
     # via
     #   jupyterlab
     #   notebook
-keyring==24.2.0
+keyring==25.0.0
     # via twine
-kiwisolver==1.4.4
+kiwisolver==1.4.5
     # via
     #   -c requirements/requirements-py39.txt
     #   matplotlib
 markdown-it-py==3.0.0
     # via
     #   mdit-py-plugins
     #   myst-parser
-markupsafe==2.1.3
+markupsafe==2.1.5
     # via
     #   jinja2
     #   nbconvert
-matplotlib==3.7.2
+matplotlib==3.8.3
     # via
     #   -c requirements/requirements-py39.txt
     #   pydynamic
 matplotlib-inline==0.1.6
     # via
     #   ipykernel
     #   ipython
 mdit-py-plugins==0.4.0
     # via myst-parser
 mdurl==0.1.2
     # via markdown-it-py
-mistune==3.0.1
+mistune==3.0.2
     # via nbconvert
-more-itertools==10.0.0
-    # via jaraco-classes
+more-itertools==10.2.0
+    # via
+    #   jaraco-classes
+    #   jaraco-functools
 mpmath==1.3.0
     # via
     #   -c requirements/requirements-py39.txt
     #   sympy
 mypy-extensions==1.0.0
     # via black
 myst-parser==2.0.0
     # via pydynamic
-nbclient==0.8.0
+nbclient==0.10.0
     # via nbconvert
-nbconvert==7.7.3
+nbconvert==7.16.3
     # via
     #   jupyter-server
     #   nbsphinx
-nbformat==5.9.2
+nbformat==5.10.3
     # via
     #   jupyter-server
     #   nbclient
     #   nbconvert
     #   nbsphinx
-nbsphinx==0.9.2
+nbsphinx==0.9.3
     # via pydynamic
-nest-asyncio==1.5.7
+nest-asyncio==1.6.0
     # via ipykernel
-notebook==7.0.1
+nh3==0.2.17
+    # via readme-renderer
+notebook==7.1.2
     # via pydynamic
-notebook-shim==0.2.3
+notebook-shim==0.2.4
     # via
     #   jupyterlab
     #   notebook
-numpy==1.25.2
+numpy==1.26.4
     # via
     #   -c requirements/requirements-py39.txt
     #   contourpy
     #   matplotlib
     #   pandas
     #   pydynamic
     #   pywavelets
     #   scipy
     #   time-series-buffer
 oauthlib==3.2.2
     # via
     #   requests-oauthlib
     #   tweepy
-overrides==7.3.1
+overrides==7.7.0
     # via jupyter-server
-packaging==23.1
+packaging==24.0
     # via
     #   -c requirements/requirements-py39.txt
     #   black
     #   ipykernel
     #   jupyter-server
     #   jupyterlab
     #   jupyterlab-server
     #   matplotlib
     #   nbconvert
     #   pyproject-api
     #   pytest
     #   python-semantic-release
     #   sphinx
     #   tox
-pandas==2.0.3
+pandas==2.2.1
     # via
     #   -c requirements/requirements-py39.txt
     #   pydynamic
-pandocfilters==1.5.0
+pandocfilters==1.5.1
     # via nbconvert
 parso==0.8.3
     # via jedi
-pathspec==0.11.2
+pathspec==0.12.1
     # via black
-pexpect==4.8.0
-    # via ipython
-pickleshare==0.7.5
+pexpect==4.9.0
     # via ipython
-pillow==10.0.0
+pillow==10.2.0
     # via
     #   -c requirements/requirements-py39.txt
     #   matplotlib
-pkginfo==1.9.6
+pkginfo==1.10.0
     # via twine
-platformdirs==3.10.0
+platformdirs==4.2.0
     # via
     #   black
     #   jupyter-core
     #   tox
     #   virtualenv
-pluggy==1.2.0
+pluggy==1.4.0
     # via
     #   pytest
     #   tox
-prometheus-client==0.17.1
+prometheus-client==0.20.0
     # via jupyter-server
-prompt-toolkit==3.0.39
+prompt-toolkit==3.0.43
     # via ipython
-psutil==5.9.5
+psutil==5.9.8
     # via ipykernel
 ptyprocess==0.7.0
     # via
     #   pexpect
     #   terminado
 pure-eval==0.2.2
     # via stack-data
-pycparser==2.21
+pycparser==2.22
     # via cffi
-pygments==2.15.1
+pygments==2.17.2
     # via
     #   ipython
     #   nbconvert
     #   readme-renderer
     #   sphinx
-pyparsing==3.0.9
+pyparsing==3.1.2
     # via
     #   -c requirements/requirements-py39.txt
     #   matplotlib
-pyproject-api==1.5.3
+pyproject-api==1.6.1
     # via tox
-pytest==7.4.0
+pytest==8.1.1
     # via
     #   pydynamic
     #   pytest-cov
     #   pytest-custom-exit-code
-pytest-cov==4.1.0
+pytest-cov==5.0.0
     # via pydynamic
 pytest-custom-exit-code==0.3.0
     # via pydynamic
-python-dateutil==2.8.2
+python-dateutil==2.9.0.post0
     # via
     #   -c requirements/requirements-py39.txt
     #   arrow
     #   jupyter-client
     #   matplotlib
     #   pandas
 python-gitlab==3.15.0
     # via python-semantic-release
 python-json-logger==2.0.7
     # via jupyter-events
 python-semantic-release==7.34.6
     # via pydynamic
-pytz==2023.3
+pytz==2024.1
     # via
     #   -c requirements/requirements-py39.txt
     #   pandas
-pywavelets==1.4.1
+pywavelets==1.5.0
     # via
     #   -c requirements/requirements-py39.txt
     #   pydynamic
 pyyaml==6.0.1
     # via
     #   jupyter-events
     #   myst-parser
-pyzmq==25.1.0
+pyzmq==25.1.2
     # via
     #   ipykernel
     #   jupyter-client
     #   jupyter-server
-readme-renderer==40.0
+readme-renderer==43.0
     # via twine
-referencing==0.30.0
+referencing==0.34.0
     # via
     #   jsonschema
     #   jsonschema-specifications
     #   jupyter-events
 requests==2.31.0
     # via
     #   jupyterlab-server
@@ -436,19 +451,19 @@
     #   jupyter-events
 rfc3986==2.0.0
     # via twine
 rfc3986-validator==0.1.1
     # via
     #   jsonschema
     #   jupyter-events
-rpds-py==0.9.2
+rpds-py==0.18.0
     # via
     #   jsonschema
     #   referencing
-scipy==1.11.1
+scipy==1.12.0
     # via
     #   -c requirements/requirements-py39.txt
     #   pydynamic
 secretstorage==3.3.3
     # via keyring
 semver==2.13.0
     # via python-semantic-release
@@ -457,54 +472,56 @@
 six==1.16.0
     # via
     #   -c requirements/requirements-py39.txt
     #   asttokens
     #   bleach
     #   python-dateutil
     #   rfc3339-validator
-smmap==5.0.0
+smmap==5.0.1
     # via gitdb
-sniffio==1.3.0
-    # via anyio
+sniffio==1.3.1
+    # via
+    #   anyio
+    #   httpx
 snowballstemmer==2.2.0
     # via sphinx
 sortedcontainers==2.4.0
     # via hypothesis
-soupsieve==2.4.1
+soupsieve==2.5
     # via beautifulsoup4
-sphinx==6.2.1
+sphinx==7.2.6
     # via
     #   myst-parser
     #   nbsphinx
     #   pydynamic
     #   sphinx-rtd-theme
     #   sphinxcontrib-jquery
-sphinx-rtd-theme==1.2.2
+sphinx-rtd-theme==2.0.0
     # via pydynamic
-sphinxcontrib-applehelp==1.0.4
+sphinxcontrib-applehelp==1.0.8
     # via sphinx
-sphinxcontrib-devhelp==1.0.2
+sphinxcontrib-devhelp==1.0.6
     # via sphinx
-sphinxcontrib-htmlhelp==2.0.1
+sphinxcontrib-htmlhelp==2.0.5
     # via sphinx
 sphinxcontrib-jquery==4.1
     # via sphinx-rtd-theme
 sphinxcontrib-jsmath==1.0.1
     # via sphinx
-sphinxcontrib-qthelp==1.0.3
+sphinxcontrib-qthelp==1.0.7
     # via sphinx
-sphinxcontrib-serializinghtml==1.1.5
+sphinxcontrib-serializinghtml==1.1.10
     # via sphinx
-stack-data==0.6.2
+stack-data==0.6.3
     # via ipython
 sympy==1.12
     # via
     #   -c requirements/requirements-py39.txt
     #   pydynamic
-terminado==0.17.1
+terminado==0.18.1
     # via
     #   jupyter-server
     #   jupyter-server-terminals
 time-series-buffer==0.1.4b0
     # via
     #   -c requirements/requirements-py39.txt
     #   pydynamic
@@ -516,29 +533,29 @@
     # via
     #   black
     #   coverage
     #   jupyterlab
     #   pyproject-api
     #   pytest
     #   tox
-tomlkit==0.12.1
+tomlkit==0.12.4
     # via python-semantic-release
-tornado==6.3.2
+tornado==6.4
     # via
     #   ipykernel
     #   jupyter-client
     #   jupyter-server
     #   jupyterlab
     #   notebook
     #   terminado
-tox==4.6.4
+tox==4.14.2
     # via pydynamic
-tqdm==4.65.0
+tqdm==4.66.2
     # via twine
-traitlets==5.9.0
+traitlets==5.14.2
     # via
     #   comm
     #   ipykernel
     #   ipython
     #   jupyter-client
     #   jupyter-core
     #   jupyter-events
@@ -549,45 +566,48 @@
     #   nbconvert
     #   nbformat
     #   nbsphinx
 tweepy==4.14.0
     # via pydynamic
 twine==3.8.0
     # via python-semantic-release
-typing-extensions==4.7.1
+types-python-dateutil==2.9.0.20240316
+    # via arrow
+typing-extensions==4.10.0
     # via
+    #   anyio
     #   async-lru
     #   black
     #   ipython
-tzdata==2023.3
+tzdata==2024.1
     # via
     #   -c requirements/requirements-py39.txt
     #   pandas
 uncertainties==3.1.7
     # via
     #   -c requirements/requirements-py39.txt
     #   time-series-buffer
 uri-template==1.3.0
     # via jsonschema
-urllib3==2.0.4
+urllib3==2.2.1
     # via
     #   requests
     #   twine
-virtualenv==20.24.2
+virtualenv==20.25.1
     # via tox
-wcwidth==0.2.6
+wcwidth==0.2.13
     # via prompt-toolkit
 webcolors==1.13
     # via jsonschema
 webencodings==0.5.1
     # via
     #   bleach
     #   tinycss2
-websocket-client==1.6.1
+websocket-client==1.7.0
     # via jupyter-server
-wheel==0.41.0
+wheel==0.43.0
     # via python-semantic-release
-zipp==3.16.2
+zipp==3.18.1
     # via
     #   -c requirements/requirements-py39.txt
     #   importlib-metadata
     #   importlib-resources
```

### Comparing `PyDynamic-2.4.2/requirements/requirements-py310.txt` & `PyDynamic-2.5.0/requirements/requirements-py310.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,57 +1,57 @@
 #
 # This file is autogenerated by pip-compile with Python 3.10
 # by the following command:
 #
 #    pip-compile --output-file=requirements/requirements-py310.txt
 #
-contourpy==1.1.0
+contourpy==1.2.0
     # via matplotlib
-cycler==0.11.0
+cycler==0.12.1
     # via matplotlib
-fonttools==4.41.1
+fonttools==4.50.0
     # via matplotlib
-future==0.18.3
+future==1.0.0
     # via uncertainties
-kiwisolver==1.4.4
+kiwisolver==1.4.5
     # via matplotlib
-matplotlib==3.7.2
+matplotlib==3.8.3
     # via PyDynamic (setup.py)
 mpmath==1.3.0
     # via sympy
-numpy==1.25.2
+numpy==1.26.4
     # via
     #   PyDynamic (setup.py)
     #   contourpy
     #   matplotlib
     #   pandas
     #   pywavelets
     #   scipy
     #   time-series-buffer
-packaging==23.1
+packaging==24.0
     # via matplotlib
-pandas==2.0.3
+pandas==2.2.1
     # via PyDynamic (setup.py)
-pillow==10.0.0
+pillow==10.2.0
     # via matplotlib
-pyparsing==3.0.9
+pyparsing==3.1.2
     # via matplotlib
-python-dateutil==2.8.2
+python-dateutil==2.9.0.post0
     # via
     #   matplotlib
     #   pandas
-pytz==2023.3
+pytz==2024.1
     # via pandas
-pywavelets==1.4.1
+pywavelets==1.5.0
     # via PyDynamic (setup.py)
-scipy==1.11.1
+scipy==1.12.0
     # via PyDynamic (setup.py)
 six==1.16.0
     # via python-dateutil
 sympy==1.12
     # via PyDynamic (setup.py)
 time-series-buffer==0.1.4b0
     # via PyDynamic (setup.py)
-tzdata==2023.3
+tzdata==2024.1
     # via pandas
 uncertainties==3.1.7
     # via time-series-buffer
```

### Comparing `PyDynamic-2.4.2/requirements/requirements-py311.txt` & `PyDynamic-2.5.0/requirements/requirements-py311.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,57 +1,57 @@
 #
 # This file is autogenerated by pip-compile with Python 3.11
 # by the following command:
 #
 #    pip-compile --output-file=requirements/requirements-py311.txt
 #
-contourpy==1.1.0
+contourpy==1.2.0
     # via matplotlib
-cycler==0.11.0
+cycler==0.12.1
     # via matplotlib
-fonttools==4.41.1
+fonttools==4.50.0
     # via matplotlib
-future==0.18.3
+future==1.0.0
     # via uncertainties
-kiwisolver==1.4.4
+kiwisolver==1.4.5
     # via matplotlib
-matplotlib==3.7.2
+matplotlib==3.8.3
     # via PyDynamic (setup.py)
 mpmath==1.3.0
     # via sympy
-numpy==1.25.2
+numpy==1.26.4
     # via
     #   PyDynamic (setup.py)
     #   contourpy
     #   matplotlib
     #   pandas
     #   pywavelets
     #   scipy
     #   time-series-buffer
-packaging==23.1
+packaging==24.0
     # via matplotlib
-pandas==2.0.3
+pandas==2.2.1
     # via PyDynamic (setup.py)
-pillow==10.0.0
+pillow==10.2.0
     # via matplotlib
-pyparsing==3.0.9
+pyparsing==3.1.2
     # via matplotlib
-python-dateutil==2.8.2
+python-dateutil==2.9.0.post0
     # via
     #   matplotlib
     #   pandas
-pytz==2023.3
+pytz==2024.1
     # via pandas
-pywavelets==1.4.1
+pywavelets==1.5.0
     # via PyDynamic (setup.py)
-scipy==1.11.1
+scipy==1.12.0
     # via PyDynamic (setup.py)
 six==1.16.0
     # via python-dateutil
 sympy==1.12
     # via PyDynamic (setup.py)
 time-series-buffer==0.1.4b0
     # via PyDynamic (setup.py)
-tzdata==2023.3
+tzdata==2024.1
     # via pandas
 uncertainties==3.1.7
     # via time-series-buffer
```

### Comparing `PyDynamic-2.4.2/requirements/requirements-py38.txt` & `PyDynamic-2.5.0/requirements/requirements-py38.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,61 +1,61 @@
 #
 # This file is autogenerated by pip-compile with Python 3.8
 # by the following command:
 #
 #    pip-compile --output-file=requirements/requirements-py38.txt
 #
-contourpy==1.1.0
+contourpy==1.1.1
     # via matplotlib
-cycler==0.11.0
+cycler==0.12.1
     # via matplotlib
-fonttools==4.41.1
+fonttools==4.50.0
     # via matplotlib
-future==0.18.3
+future==1.0.0
     # via uncertainties
-importlib-resources==6.0.0
+importlib-resources==6.4.0
     # via matplotlib
-kiwisolver==1.4.4
+kiwisolver==1.4.5
     # via matplotlib
-matplotlib==3.7.2
+matplotlib==3.7.5
     # via PyDynamic (setup.py)
 mpmath==1.3.0
     # via sympy
 numpy==1.24.4
     # via
     #   PyDynamic (setup.py)
     #   contourpy
     #   matplotlib
     #   pandas
     #   pywavelets
     #   scipy
     #   time-series-buffer
-packaging==23.1
+packaging==24.0
     # via matplotlib
 pandas==2.0.3
     # via PyDynamic (setup.py)
-pillow==10.0.0
+pillow==10.2.0
     # via matplotlib
-pyparsing==3.0.9
+pyparsing==3.1.2
     # via matplotlib
-python-dateutil==2.8.2
+python-dateutil==2.9.0.post0
     # via
     #   matplotlib
     #   pandas
-pytz==2023.3
+pytz==2024.1
     # via pandas
 pywavelets==1.4.1
     # via PyDynamic (setup.py)
 scipy==1.10.1
     # via PyDynamic (setup.py)
 six==1.16.0
     # via python-dateutil
 sympy==1.12
     # via PyDynamic (setup.py)
 time-series-buffer==0.1.4b0
     # via PyDynamic (setup.py)
-tzdata==2023.3
+tzdata==2024.1
     # via pandas
 uncertainties==3.1.7
     # via time-series-buffer
-zipp==3.16.2
+zipp==3.18.1
     # via importlib-resources
```

### Comparing `PyDynamic-2.4.2/requirements/requirements-py39.txt` & `PyDynamic-2.5.0/requirements/requirements-py39.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,61 +1,61 @@
 #
 # This file is autogenerated by pip-compile with Python 3.9
 # by the following command:
 #
 #    pip-compile --output-file=requirements/requirements-py39.txt
 #
-contourpy==1.1.0
+contourpy==1.2.0
     # via matplotlib
-cycler==0.11.0
+cycler==0.12.1
     # via matplotlib
-fonttools==4.41.1
+fonttools==4.50.0
     # via matplotlib
-future==0.18.3
+future==1.0.0
     # via uncertainties
-importlib-resources==6.0.0
+importlib-resources==6.4.0
     # via matplotlib
-kiwisolver==1.4.4
+kiwisolver==1.4.5
     # via matplotlib
-matplotlib==3.7.2
+matplotlib==3.8.3
     # via PyDynamic (setup.py)
 mpmath==1.3.0
     # via sympy
-numpy==1.25.2
+numpy==1.26.4
     # via
     #   PyDynamic (setup.py)
     #   contourpy
     #   matplotlib
     #   pandas
     #   pywavelets
     #   scipy
     #   time-series-buffer
-packaging==23.1
+packaging==24.0
     # via matplotlib
-pandas==2.0.3
+pandas==2.2.1
     # via PyDynamic (setup.py)
-pillow==10.0.0
+pillow==10.2.0
     # via matplotlib
-pyparsing==3.0.9
+pyparsing==3.1.2
     # via matplotlib
-python-dateutil==2.8.2
+python-dateutil==2.9.0.post0
     # via
     #   matplotlib
     #   pandas
-pytz==2023.3
+pytz==2024.1
     # via pandas
-pywavelets==1.4.1
+pywavelets==1.5.0
     # via PyDynamic (setup.py)
-scipy==1.11.1
+scipy==1.12.0
     # via PyDynamic (setup.py)
 six==1.16.0
     # via python-dateutil
 sympy==1.12
     # via PyDynamic (setup.py)
 time-series-buffer==0.1.4b0
     # via PyDynamic (setup.py)
-tzdata==2023.3
+tzdata==2024.1
     # via pandas
 uncertainties==3.1.7
     # via time-series-buffer
-zipp==3.16.2
+zipp==3.18.1
     # via importlib-resources
```

### Comparing `PyDynamic-2.4.2/requirements/upgrade_dependencies.sh` & `PyDynamic-2.5.0/requirements/upgrade_dependencies.sh`

 * *Files identical despite different names*

### Comparing `PyDynamic-2.4.2/setup.cfg` & `PyDynamic-2.5.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `PyDynamic-2.4.2/setup.py` & `PyDynamic-2.5.0/setup.py`

 * *Files identical despite different names*

### Comparing `PyDynamic-2.4.2/src/PyDynamic/__init__.py` & `PyDynamic-2.5.0/src/PyDynamic/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 .. seealso::
 
    - `initial project website <https://www.euramet.org/research-innovation/search
      -research-projects/details/project/standards-and-software-to-maximise-end-user
      -uptake-of-nmi-calibrations-of-dynamic-force-torque-and/>`_
    - `GitHub website <https://www.github.com/PTB-M4D/PyDynamic>`_
 """
-__version__ = "2.4.2"
+__version__ = "2.5.0"
 
 __all__ = [
     "LSFIR",
     "LSIIR",
     "fit_som",
     "FreqResp2RealImag",
     "GUM_DFT",
@@ -67,12 +67,14 @@
     "is_vector",
     "is_2d_matrix",
     "number_of_rows_equals_vector_dim",
     "real_imag_2_complex",
     "separate_real_imag_of_mc_samples",
     "separate_real_imag_of_vector",
     "complex_2_real_imag",
+    "hadamar_product",
+    "window_application",
 ]
 
 from .misc import *
 from .model_estimation import *
 from .uncertainty import *
```

### Comparing `PyDynamic-2.4.2/src/PyDynamic/deconvolution/__init__.py` & `PyDynamic-2.5.0/src/PyDynamic/deconvolution/__init__.py`

 * *Files identical despite different names*

### Comparing `PyDynamic-2.4.2/src/PyDynamic/deconvolution/fit_filter.py` & `PyDynamic-2.5.0/src/PyDynamic/deconvolution/fit_filter.py`

 * *Files identical despite different names*

### Comparing `PyDynamic-2.4.2/src/PyDynamic/examples/demonstrate_fit_som.py` & `PyDynamic-2.5.0/src/PyDynamic/examples/demonstrate_fit_som.py`

 * *Files identical despite different names*

### Comparing `PyDynamic-2.4.2/src/PyDynamic/examples/uncertainty_for_dft/DFT_amplitude_phase.py` & `PyDynamic-2.5.0/src/PyDynamic/examples/uncertainty_for_dft/DFT_amplitude_phase.py`

 * *Files identical despite different names*

### Comparing `PyDynamic-2.4.2/src/PyDynamic/examples/uncertainty_for_dft/DFTdeconv calibration.dat` & `PyDynamic-2.5.0/src/PyDynamic/examples/uncertainty_for_dft/DFTdeconv calibration.dat`

 * *Files identical despite different names*

### Comparing `PyDynamic-2.4.2/src/PyDynamic/examples/uncertainty_for_dft/DFTdeconv measured_signal.dat` & `PyDynamic-2.5.0/src/PyDynamic/examples/uncertainty_for_dft/DFTdeconv measured_signal.dat`

 * *Files identical despite different names*

### Comparing `PyDynamic-2.4.2/src/PyDynamic/examples/uncertainty_for_dft/DFTdeconv reference_signal.dat` & `PyDynamic-2.5.0/src/PyDynamic/examples/uncertainty_for_dft/DFTdeconv reference_signal.dat`

 * *Files identical despite different names*

### Comparing `PyDynamic-2.4.2/src/PyDynamic/examples/uncertainty_for_dft/deconv_DFT.py` & `PyDynamic-2.5.0/src/PyDynamic/examples/uncertainty_for_dft/deconv_DFT.py`

 * *Files identical despite different names*

### Comparing `PyDynamic-2.4.2/src/PyDynamic/examples/working_with_signals.py` & `PyDynamic-2.5.0/src/PyDynamic/examples/working_with_signals.py`

 * *Files identical despite different names*

### Comparing `PyDynamic-2.4.2/src/PyDynamic/identification/fit_filter.py` & `PyDynamic-2.5.0/src/PyDynamic/identification/fit_filter.py`

 * *Files identical despite different names*

### Comparing `PyDynamic-2.4.2/src/PyDynamic/identification/fit_transfer.py` & `PyDynamic-2.5.0/src/PyDynamic/identification/fit_transfer.py`

 * *Files identical despite different names*

### Comparing `PyDynamic-2.4.2/src/PyDynamic/misc/SecondOrderSystem.py` & `PyDynamic-2.5.0/src/PyDynamic/misc/SecondOrderSystem.py`

 * *Files identical despite different names*

### Comparing `PyDynamic-2.4.2/src/PyDynamic/misc/__init__.py` & `PyDynamic-2.5.0/src/PyDynamic/misc/__init__.py`

 * *Files identical despite different names*

### Comparing `PyDynamic-2.4.2/src/PyDynamic/misc/filterstuff.py` & `PyDynamic-2.5.0/src/PyDynamic/misc/filterstuff.py`

 * *Files identical despite different names*

### Comparing `PyDynamic-2.4.2/src/PyDynamic/misc/impinvar.py` & `PyDynamic-2.5.0/src/PyDynamic/misc/impinvar.py`

 * *Files identical despite different names*

### Comparing `PyDynamic-2.4.2/src/PyDynamic/misc/noise.py` & `PyDynamic-2.5.0/src/PyDynamic/misc/noise.py`

 * *Files identical despite different names*

### Comparing `PyDynamic-2.4.2/src/PyDynamic/misc/testsignals.py` & `PyDynamic-2.5.0/src/PyDynamic/misc/testsignals.py`

 * *Files identical despite different names*

### Comparing `PyDynamic-2.4.2/src/PyDynamic/misc/tools.py` & `PyDynamic-2.5.0/src/PyDynamic/misc/tools.py`

 * *Files identical despite different names*

### Comparing `PyDynamic-2.4.2/src/PyDynamic/model_estimation/__init__.py` & `PyDynamic-2.5.0/src/PyDynamic/model_estimation/__init__.py`

 * *Files identical despite different names*

### Comparing `PyDynamic-2.4.2/src/PyDynamic/model_estimation/fit_filter.py` & `PyDynamic-2.5.0/src/PyDynamic/model_estimation/fit_filter.py`

 * *Files identical despite different names*

### Comparing `PyDynamic-2.4.2/src/PyDynamic/model_estimation/fit_transfer.py` & `PyDynamic-2.5.0/src/PyDynamic/model_estimation/fit_transfer.py`

 * *Files identical despite different names*

### Comparing `PyDynamic-2.4.2/src/PyDynamic/signals.py` & `PyDynamic-2.5.0/src/PyDynamic/signals.py`

 * *Files identical despite different names*

### Comparing `PyDynamic-2.4.2/src/PyDynamic/uncertainty/__init__.py` & `PyDynamic-2.5.0/src/PyDynamic/uncertainty/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -34,14 +34,16 @@
     "dwt",
     "wave_dec",
     "wave_dec_realtime",
     "inv_dwt",
     "wave_rec",
     "filter_design",
     "dwt_max_level",
+    "hadamar_product",
+    "window_application",
 ]
 
 from .interpolate import interp1d_unc
 from .propagate_DFT import (
     AmpPhase2DFT,
     AmpPhase2Time,
     DFT2AmpPhase,
@@ -58,8 +60,9 @@
     inv_dwt,
     wave_dec,
     wave_dec_realtime,
     wave_rec,
 )
 from .propagate_filter import FIRuncFilter, IIR_get_initial_state, IIRuncFilter
 from .propagate_MonteCarlo import MC, SMC, UMC, UMC_generic
+from .propagate_multiplication import hadamar_product, window_application
 from ..misc.noise import ARMA
```

### Comparing `PyDynamic-2.4.2/src/PyDynamic/uncertainty/interpolate.py` & `PyDynamic-2.5.0/src/PyDynamic/uncertainty/interpolate.py`

 * *Files identical despite different names*

### Comparing `PyDynamic-2.4.2/src/PyDynamic/uncertainty/interpolation.py` & `PyDynamic-2.5.0/src/PyDynamic/uncertainty/interpolation.py`

 * *Files identical despite different names*

### Comparing `PyDynamic-2.4.2/src/PyDynamic/uncertainty/propagate_DFT.py` & `PyDynamic-2.5.0/src/PyDynamic/uncertainty/propagate_DFT.py`

 * *Files identical despite different names*

### Comparing `PyDynamic-2.4.2/src/PyDynamic/uncertainty/propagate_DWT.py` & `PyDynamic-2.5.0/src/PyDynamic/uncertainty/propagate_DWT.py`

 * *Files identical despite different names*

### Comparing `PyDynamic-2.4.2/src/PyDynamic/uncertainty/propagate_MonteCarlo.py` & `PyDynamic-2.5.0/src/PyDynamic/uncertainty/propagate_MonteCarlo.py`

 * *Files identical despite different names*

### Comparing `PyDynamic-2.4.2/src/PyDynamic/uncertainty/propagate_convolution.py` & `PyDynamic-2.5.0/src/PyDynamic/uncertainty/propagate_convolution.py`

 * *Files identical despite different names*

### Comparing `PyDynamic-2.4.2/src/PyDynamic/uncertainty/propagate_filter.py` & `PyDynamic-2.5.0/src/PyDynamic/uncertainty/propagate_filter.py`

 * *Files identical despite different names*

### Comparing `PyDynamic-2.4.2/src/PyDynamic.egg-info/PKG-INFO` & `PyDynamic-2.5.0/src/PyDynamic.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: PyDynamic
-Version: 2.4.2
+Version: 2.5.0
 Summary: A software package for the analysis of dynamic measurements
 Home-page: https://ptb-m4d.github.io/PyDynamic/
+Download-URL: https://github.com/PTB-M4D/PyDynamic/releases/download/v2.5.0/PyDynamic-2.5.0.tar.gz
 Author: Sascha Eichstädt, Maximilian Gruber, Björn Ludwig, Thomas Bruns, Martin Weber
 Author-email: sascha.eichstaedt@ptb.de
 License: UNKNOWN
-Download-URL: https://github.com/PTB-M4D/PyDynamic/releases/download/v2.4.2/PyDynamic-2.4.2.tar.gz
-Project-URL: Documentation, https://pydynamic.readthedocs.io/en/v2.4.2/
-Project-URL: Source, https://github.com/PTB-M4D/PyDynamic/tree/v2.4.2/
+Project-URL: Documentation, https://pydynamic.readthedocs.io/en/v2.5.0/
+Project-URL: Source, https://github.com/PTB-M4D/PyDynamic/tree/v2.5.0/
 Project-URL: Tracker, https://github.com/PTB-M4D/PyDynamic/issues
 Keywords: measurement uncertainty,dynamic measurements,metrology,GUM
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Topic :: Utilities
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
```

#### html2text {}

```diff
@@ -1,15 +1,15 @@
-Metadata-Version: 2.1 Name: PyDynamic Version: 2.4.2 Summary: A software
+Metadata-Version: 2.1 Name: PyDynamic Version: 2.5.0 Summary: A software
 package for the analysis of dynamic measurements Home-page: https://ptb-
-m4d.github.io/PyDynamic/ Author: Sascha EichstÃ¤dt, Maximilian Gruber, BjÃ¶rn
-Ludwig, Thomas Bruns, Martin Weber Author-email: sascha.eichstaedt@ptb.de
-License: UNKNOWN Download-URL: https://github.com/PTB-M4D/PyDynamic/releases/
-download/v2.4.2/PyDynamic-2.4.2.tar.gz Project-URL: Documentation, https://
-pydynamic.readthedocs.io/en/v2.4.2/ Project-URL: Source, https://github.com/
-PTB-M4D/PyDynamic/tree/v2.4.2/ Project-URL: Tracker, https://github.com/PTB-
+m4d.github.io/PyDynamic/ Download-URL: https://github.com/PTB-M4D/PyDynamic/
+releases/download/v2.5.0/PyDynamic-2.5.0.tar.gz Author: Sascha EichstÃ¤dt,
+Maximilian Gruber, BjÃ¶rn Ludwig, Thomas Bruns, Martin Weber Author-email:
+sascha.eichstaedt@ptb.de License: UNKNOWN Project-URL: Documentation, https://
+pydynamic.readthedocs.io/en/v2.5.0/ Project-URL: Source, https://github.com/
+PTB-M4D/PyDynamic/tree/v2.5.0/ Project-URL: Tracker, https://github.com/PTB-
 M4D/PyDynamic/issues Keywords: measurement uncertainty,dynamic
 measurements,metrology,GUM Platform: UNKNOWN Classifier: Development Status ::
 4 - Beta Classifier: Topic :: Utilities Classifier: Topic :: Scientific/
 Engineering Classifier: Topic :: Software Development :: Libraries :: Python
 Modules Classifier: Intended Audience :: Education Classifier: Intended
 Audience :: Science/Research Classifier: License :: OSI Approved :: GNU Lesser
 General Public License v3 or later (LGPLv3+) Classifier: Programming Language
```

