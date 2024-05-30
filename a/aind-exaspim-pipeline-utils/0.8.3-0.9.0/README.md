# Comparing `tmp/aind_exaspim_pipeline_utils-0.8.3.tar.gz` & `tmp/aind_exaspim_pipeline_utils-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aind_exaspim_pipeline_utils-0.8.3.tar", last modified: Thu May 16 03:26:27 2024, max compression
+gzip compressed data, was "aind_exaspim_pipeline_utils-0.9.0.tar", last modified: Fri May 17 23:03:20 2024, max compression
```

## Comparing `aind_exaspim_pipeline_utils-0.8.3.tar` & `aind_exaspim_pipeline_utils-0.9.0.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 03:26:27.445949 aind_exaspim_pipeline_utils-0.8.3/
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-16 03:26:17.000000 aind_exaspim_pipeline_utils-0.8.3/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 03:26:27.433949 aind_exaspim_pipeline_utils-0.8.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 03:26:27.437949 aind_exaspim_pipeline_utils-0.8.3/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      834 2024-05-16 03:26:17.000000 aind_exaspim_pipeline_utils-0.8.3/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-16 03:26:17.000000 aind_exaspim_pipeline_utils-0.8.3/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (127)      772 2024-05-16 03:26:17.000000 aind_exaspim_pipeline_utils-0.8.3/.github/ISSUE_TEMPLATE/user-story.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 03:26:27.437949 aind_exaspim_pipeline_utils-0.8.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      800 2024-05-16 03:26:17.000000 aind_exaspim_pipeline_utils-0.8.3/.github/workflows/lint_and_test.yml
--rw-r--r--   0 runner    (1001) docker     (127)      812 2024-05-16 03:26:17.000000 aind_exaspim_pipeline_utils-0.8.3/.github/workflows/tag_and_publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2199 2024-05-16 03:26:17.000000 aind_exaspim_pipeline_utils-0.8.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-16 03:26:17.000000 aind_exaspim_pipeline_utils-0.8.3/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-16 03:26:17.000000 aind_exaspim_pipeline_utils-0.8.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4947 2024-05-16 03:26:27.445949 aind_exaspim_pipeline_utils-0.8.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3815 2024-05-16 03:26:17.000000 aind_exaspim_pipeline_utils-0.8.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 03:26:27.437949 aind_exaspim_pipeline_utils-0.8.3/capsule_scripts/
--rw-r--r--   0 runner    (1001) docker     (127)      476 2024-05-16 03:26:17.000000 aind_exaspim_pipeline_utils-0.8.3/capsule_scripts/imagej_postInstall
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-16 03:26:17.000000 aind_exaspim_pipeline_utils-0.8.3/capsule_scripts/imagej_run.sh
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-05-16 03:26:17.000000 aind_exaspim_pipeline_utils-0.8.3/capsule_scripts/n5tozarr_postInstall
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-16 03:26:17.000000 aind_exaspim_pipeline_utils-0.8.3/capsule_scripts/n5tozarr_run.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 03:26:27.437949 aind_exaspim_pipeline_utils-0.8.3/doc/
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-16 03:26:17.000000 aind_exaspim_pipeline_utils-0.8.3/doc/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-05-16 03:26:17.000000 aind_exaspim_pipeline_utils-0.8.3/doc/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 03:26:27.437949 aind_exaspim_pipeline_utils-0.8.3/doc/source/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 03:26:27.437949 aind_exaspim_pipeline_utils-0.8.3/doc/source/_static/
--rw-r--r--   0 runner    (1001) docker     (127)     8733 2024-05-16 03:26:17.000000 aind_exaspim_pipeline_utils-0.8.3/doc/source/_static/dark-logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)   259838 2024-05-16 03:26:17.000000 aind_exaspim_pipeline_utils-0.8.3/doc/source/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)     8712 2024-05-16 03:26:17.000000 aind_exaspim_pipeline_utils-0.8.3/doc/source/_static/light-logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1769 2024-05-16 03:26:17.000000 aind_exaspim_pipeline_utils-0.8.3/doc/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      420 2024-05-16 03:26:17.000000 aind_exaspim_pipeline_utils-0.8.3/doc/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2594 2024-05-16 03:26:17.000000 aind_exaspim_pipeline_utils-0.8.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 03:26:27.445949 aind_exaspim_pipeline_utils-0.8.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-16 03:26:17.000000 aind_exaspim_pipeline_utils-0.8.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 03:26:27.433949 aind_exaspim_pipeline_utils-0.8.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 03:26:27.441949 aind_exaspim_pipeline_utils-0.8.3/src/aind_exaspim_pipeline_utils/
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-16 03:26:17.000000 aind_exaspim_pipeline_utils-0.8.3/src/aind_exaspim_pipeline_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23464 2024-05-16 03:26:17.000000 aind_exaspim_pipeline_utils-0.8.3/src/aind_exaspim_pipeline_utils/exaspim_manifest.py
--rw-r--r--   0 runner    (1001) docker     (127)     7057 2024-05-16 03:26:17.000000 aind_exaspim_pipeline_utils-0.8.3/src/aind_exaspim_pipeline_utils/imagej_macros.py
--rw-r--r--   0 runner    (1001) docker     (127)    24060 2024-05-16 03:26:17.000000 aind_exaspim_pipeline_utils-0.8.3/src/aind_exaspim_pipeline_utils/imagej_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     3114 2024-05-16 03:26:17.000000 aind_exaspim_pipeline_utils-0.8.3/src/aind_exaspim_pipeline_utils/java_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 03:26:27.441949 aind_exaspim_pipeline_utils-0.8.3/src/aind_exaspim_pipeline_utils/n5tozarr/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-16 03:26:17.000000 aind_exaspim_pipeline_utils-0.8.3/src/aind_exaspim_pipeline_utils/n5tozarr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18825 2024-05-16 03:26:17.000000 aind_exaspim_pipeline_utils-0.8.3/src/aind_exaspim_pipeline_utils/n5tozarr/n5tozarr_da.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 03:26:27.441949 aind_exaspim_pipeline_utils-0.8.3/src/aind_exaspim_pipeline_utils/qc/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-16 03:26:17.000000 aind_exaspim_pipeline_utils-0.8.3/src/aind_exaspim_pipeline_utils/qc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3516 2024-05-16 03:26:17.000000 aind_exaspim_pipeline_utils-0.8.3/src/aind_exaspim_pipeline_utils/qc/bigstitcher_log_edge_analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)     6987 2024-05-16 03:26:17.000000 aind_exaspim_pipeline_utils-0.8.3/src/aind_exaspim_pipeline_utils/qc/create_ng_link.py
--rw-r--r--   0 runner    (1001) docker     (127)     9689 2024-05-16 03:26:17.000000 aind_exaspim_pipeline_utils-0.8.3/src/aind_exaspim_pipeline_utils/qc/ng_ip_visualization.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 03:26:27.441949 aind_exaspim_pipeline_utils-0.8.3/src/aind_exaspim_pipeline_utils/trigger/
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-16 03:26:17.000000 aind_exaspim_pipeline_utils-0.8.3/src/aind_exaspim_pipeline_utils/trigger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    28937 2024-05-16 03:26:17.000000 aind_exaspim_pipeline_utils-0.8.3/src/aind_exaspim_pipeline_utils/trigger/capsule.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 03:26:27.445949 aind_exaspim_pipeline_utils-0.8.3/src/aind_exaspim_pipeline_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4947 2024-05-16 03:26:27.000000 aind_exaspim_pipeline_utils-0.8.3/src/aind_exaspim_pipeline_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1743 2024-05-16 03:26:27.000000 aind_exaspim_pipeline_utils-0.8.3/src/aind_exaspim_pipeline_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 03:26:27.000000 aind_exaspim_pipeline_utils-0.8.3/src/aind_exaspim_pipeline_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      736 2024-05-16 03:26:27.000000 aind_exaspim_pipeline_utils-0.8.3/src/aind_exaspim_pipeline_utils.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-05-16 03:26:27.000000 aind_exaspim_pipeline_utils-0.8.3/src/aind_exaspim_pipeline_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-16 03:26:27.000000 aind_exaspim_pipeline_utils-0.8.3/src/aind_exaspim_pipeline_utils.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 03:26:27.441949 aind_exaspim_pipeline_utils-0.8.3/src/aind_trigger_codeocean/
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-16 03:26:17.000000 aind_exaspim_pipeline_utils-0.8.3/src/aind_trigger_codeocean/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    51638 2024-05-16 03:26:17.000000 aind_exaspim_pipeline_utils-0.8.3/src/aind_trigger_codeocean/pipelines.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 03:26:27.445949 aind_exaspim_pipeline_utils-0.8.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-16 03:26:17.000000 aind_exaspim_pipeline_utils-0.8.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1258 2024-05-16 03:26:17.000000 aind_exaspim_pipeline_utils-0.8.3/tests/test_capsule.py
--rw-r--r--   0 runner    (1001) docker     (127)     5059 2024-05-16 03:26:17.000000 aind_exaspim_pipeline_utils-0.8.3/tests/test_imagej_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)      517 2024-05-16 03:26:17.000000 aind_exaspim_pipeline_utils-0.8.3/tests/test_n5tozarr.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 23:03:20.298424 aind_exaspim_pipeline_utils-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-17 23:03:07.000000 aind_exaspim_pipeline_utils-0.9.0/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 23:03:20.290424 aind_exaspim_pipeline_utils-0.9.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 23:03:20.290424 aind_exaspim_pipeline_utils-0.9.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      834 2024-05-17 23:03:07.000000 aind_exaspim_pipeline_utils-0.9.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-17 23:03:07.000000 aind_exaspim_pipeline_utils-0.9.0/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-05-17 23:03:07.000000 aind_exaspim_pipeline_utils-0.9.0/.github/ISSUE_TEMPLATE/user-story.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 23:03:20.290424 aind_exaspim_pipeline_utils-0.9.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-05-17 23:03:07.000000 aind_exaspim_pipeline_utils-0.9.0/.github/workflows/lint_and_test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      812 2024-05-17 23:03:07.000000 aind_exaspim_pipeline_utils-0.9.0/.github/workflows/tag_and_publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2199 2024-05-17 23:03:07.000000 aind_exaspim_pipeline_utils-0.9.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-17 23:03:07.000000 aind_exaspim_pipeline_utils-0.9.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-17 23:03:07.000000 aind_exaspim_pipeline_utils-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4947 2024-05-17 23:03:20.298424 aind_exaspim_pipeline_utils-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3815 2024-05-17 23:03:07.000000 aind_exaspim_pipeline_utils-0.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 23:03:20.294424 aind_exaspim_pipeline_utils-0.9.0/capsule_scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)      476 2024-05-17 23:03:07.000000 aind_exaspim_pipeline_utils-0.9.0/capsule_scripts/imagej_postInstall
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-17 23:03:07.000000 aind_exaspim_pipeline_utils-0.9.0/capsule_scripts/imagej_run.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-05-17 23:03:07.000000 aind_exaspim_pipeline_utils-0.9.0/capsule_scripts/n5tozarr_postInstall
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-17 23:03:07.000000 aind_exaspim_pipeline_utils-0.9.0/capsule_scripts/n5tozarr_run.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 23:03:20.294424 aind_exaspim_pipeline_utils-0.9.0/doc/
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-17 23:03:07.000000 aind_exaspim_pipeline_utils-0.9.0/doc/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-05-17 23:03:07.000000 aind_exaspim_pipeline_utils-0.9.0/doc/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 23:03:20.294424 aind_exaspim_pipeline_utils-0.9.0/doc/source/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 23:03:20.294424 aind_exaspim_pipeline_utils-0.9.0/doc/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)     8733 2024-05-17 23:03:07.000000 aind_exaspim_pipeline_utils-0.9.0/doc/source/_static/dark-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)   259838 2024-05-17 23:03:07.000000 aind_exaspim_pipeline_utils-0.9.0/doc/source/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)     8712 2024-05-17 23:03:07.000000 aind_exaspim_pipeline_utils-0.9.0/doc/source/_static/light-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1769 2024-05-17 23:03:07.000000 aind_exaspim_pipeline_utils-0.9.0/doc/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      420 2024-05-17 23:03:07.000000 aind_exaspim_pipeline_utils-0.9.0/doc/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2594 2024-05-17 23:03:07.000000 aind_exaspim_pipeline_utils-0.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 23:03:20.298424 aind_exaspim_pipeline_utils-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-17 23:03:07.000000 aind_exaspim_pipeline_utils-0.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 23:03:20.290424 aind_exaspim_pipeline_utils-0.9.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 23:03:20.294424 aind_exaspim_pipeline_utils-0.9.0/src/aind_exaspim_pipeline_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-17 23:03:08.000000 aind_exaspim_pipeline_utils-0.9.0/src/aind_exaspim_pipeline_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23464 2024-05-17 23:03:07.000000 aind_exaspim_pipeline_utils-0.9.0/src/aind_exaspim_pipeline_utils/exaspim_manifest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9154 2024-05-17 23:03:07.000000 aind_exaspim_pipeline_utils-0.9.0/src/aind_exaspim_pipeline_utils/imagej_macros.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26218 2024-05-17 23:03:07.000000 aind_exaspim_pipeline_utils-0.9.0/src/aind_exaspim_pipeline_utils/imagej_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3114 2024-05-17 23:03:07.000000 aind_exaspim_pipeline_utils-0.9.0/src/aind_exaspim_pipeline_utils/java_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 23:03:20.294424 aind_exaspim_pipeline_utils-0.9.0/src/aind_exaspim_pipeline_utils/n5tozarr/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-17 23:03:07.000000 aind_exaspim_pipeline_utils-0.9.0/src/aind_exaspim_pipeline_utils/n5tozarr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18825 2024-05-17 23:03:07.000000 aind_exaspim_pipeline_utils-0.9.0/src/aind_exaspim_pipeline_utils/n5tozarr/n5tozarr_da.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 23:03:20.298424 aind_exaspim_pipeline_utils-0.9.0/src/aind_exaspim_pipeline_utils/qc/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-17 23:03:07.000000 aind_exaspim_pipeline_utils-0.9.0/src/aind_exaspim_pipeline_utils/qc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3516 2024-05-17 23:03:07.000000 aind_exaspim_pipeline_utils-0.9.0/src/aind_exaspim_pipeline_utils/qc/bigstitcher_log_edge_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6987 2024-05-17 23:03:07.000000 aind_exaspim_pipeline_utils-0.9.0/src/aind_exaspim_pipeline_utils/qc/create_ng_link.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9689 2024-05-17 23:03:07.000000 aind_exaspim_pipeline_utils-0.9.0/src/aind_exaspim_pipeline_utils/qc/ng_ip_visualization.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 23:03:20.298424 aind_exaspim_pipeline_utils-0.9.0/src/aind_exaspim_pipeline_utils/trigger/
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-17 23:03:07.000000 aind_exaspim_pipeline_utils-0.9.0/src/aind_exaspim_pipeline_utils/trigger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28937 2024-05-17 23:03:07.000000 aind_exaspim_pipeline_utils-0.9.0/src/aind_exaspim_pipeline_utils/trigger/capsule.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 23:03:20.298424 aind_exaspim_pipeline_utils-0.9.0/src/aind_exaspim_pipeline_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4947 2024-05-17 23:03:20.000000 aind_exaspim_pipeline_utils-0.9.0/src/aind_exaspim_pipeline_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1743 2024-05-17 23:03:20.000000 aind_exaspim_pipeline_utils-0.9.0/src/aind_exaspim_pipeline_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 23:03:20.000000 aind_exaspim_pipeline_utils-0.9.0/src/aind_exaspim_pipeline_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-05-17 23:03:20.000000 aind_exaspim_pipeline_utils-0.9.0/src/aind_exaspim_pipeline_utils.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-05-17 23:03:20.000000 aind_exaspim_pipeline_utils-0.9.0/src/aind_exaspim_pipeline_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-17 23:03:20.000000 aind_exaspim_pipeline_utils-0.9.0/src/aind_exaspim_pipeline_utils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 23:03:20.298424 aind_exaspim_pipeline_utils-0.9.0/src/aind_trigger_codeocean/
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-17 23:03:07.000000 aind_exaspim_pipeline_utils-0.9.0/src/aind_trigger_codeocean/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51638 2024-05-17 23:03:07.000000 aind_exaspim_pipeline_utils-0.9.0/src/aind_trigger_codeocean/pipelines.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 23:03:20.298424 aind_exaspim_pipeline_utils-0.9.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-17 23:03:07.000000 aind_exaspim_pipeline_utils-0.9.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1258 2024-05-17 23:03:07.000000 aind_exaspim_pipeline_utils-0.9.0/tests/test_capsule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6290 2024-05-17 23:03:07.000000 aind_exaspim_pipeline_utils-0.9.0/tests/test_imagej_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)      517 2024-05-17 23:03:07.000000 aind_exaspim_pipeline_utils-0.9.0/tests/test_n5tozarr.py
```

### Comparing `aind_exaspim_pipeline_utils-0.8.3/.github/ISSUE_TEMPLATE/bug_report.md` & `aind_exaspim_pipeline_utils-0.9.0/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `aind_exaspim_pipeline_utils-0.8.3/.github/ISSUE_TEMPLATE/feature_request.md` & `aind_exaspim_pipeline_utils-0.9.0/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `aind_exaspim_pipeline_utils-0.8.3/.github/ISSUE_TEMPLATE/user-story.md` & `aind_exaspim_pipeline_utils-0.9.0/.github/ISSUE_TEMPLATE/user-story.md`

 * *Files identical despite different names*

### Comparing `aind_exaspim_pipeline_utils-0.8.3/.github/workflows/lint_and_test.yml` & `aind_exaspim_pipeline_utils-0.9.0/.github/workflows/lint_and_test.yml`

 * *Files identical despite different names*

### Comparing `aind_exaspim_pipeline_utils-0.8.3/.github/workflows/tag_and_publish.yml` & `aind_exaspim_pipeline_utils-0.9.0/.github/workflows/tag_and_publish.yml`

 * *Files identical despite different names*

### Comparing `aind_exaspim_pipeline_utils-0.8.3/.gitignore` & `aind_exaspim_pipeline_utils-0.9.0/.gitignore`

 * *Files identical despite different names*

### Comparing `aind_exaspim_pipeline_utils-0.8.3/LICENSE` & `aind_exaspim_pipeline_utils-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aind_exaspim_pipeline_utils-0.8.3/PKG-INFO` & `aind_exaspim_pipeline_utils-0.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aind_exaspim_pipeline_utils
-Version: 0.8.3
+Version: 0.9.0
 Summary: AIND exaSPIM pipeline utilities.
 Author: Allen Institute for Neural Dynamics
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `aind_exaspim_pipeline_utils-0.8.3/README.md` & `aind_exaspim_pipeline_utils-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `aind_exaspim_pipeline_utils-0.8.3/doc/Makefile` & `aind_exaspim_pipeline_utils-0.9.0/doc/Makefile`

 * *Files identical despite different names*

### Comparing `aind_exaspim_pipeline_utils-0.8.3/doc/make.bat` & `aind_exaspim_pipeline_utils-0.9.0/doc/make.bat`

 * *Files identical despite different names*

### Comparing `aind_exaspim_pipeline_utils-0.8.3/doc/source/_static/dark-logo.svg` & `aind_exaspim_pipeline_utils-0.9.0/doc/source/_static/dark-logo.svg`

 * *Files identical despite different names*

### Comparing `aind_exaspim_pipeline_utils-0.8.3/doc/source/_static/favicon.ico` & `aind_exaspim_pipeline_utils-0.9.0/doc/source/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `aind_exaspim_pipeline_utils-0.8.3/doc/source/_static/light-logo.svg` & `aind_exaspim_pipeline_utils-0.9.0/doc/source/_static/light-logo.svg`

 * *Files identical despite different names*

### Comparing `aind_exaspim_pipeline_utils-0.8.3/doc/source/conf.py` & `aind_exaspim_pipeline_utils-0.9.0/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `aind_exaspim_pipeline_utils-0.8.3/pyproject.toml` & `aind_exaspim_pipeline_utils-0.9.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `aind_exaspim_pipeline_utils-0.8.3/src/aind_exaspim_pipeline_utils/exaspim_manifest.py` & `aind_exaspim_pipeline_utils-0.9.0/src/aind_exaspim_pipeline_utils/exaspim_manifest.py`

 * *Files identical despite different names*

### Comparing `aind_exaspim_pipeline_utils-0.8.3/src/aind_exaspim_pipeline_utils/imagej_macros.py` & `aind_exaspim_pipeline_utils-0.9.0/src/aind_exaspim_pipeline_utils/imagej_macros.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,14 +8,42 @@
     This class does not check substitution values and expects that all values are valid.
     """
 
     # Fiji macro allows new line at , separated arguments
     # strings can be added " " + " "
     # within strings, [ ] can be used for spaces, for file names? TBC
 
+    MACRO_PHASE_CORRELATION = """
+run("Memory & Threads...", "parallel={parallel:d}");
+run("Calculate pairwise shifts ...",
+    " select={process_xml}" +
+    " process_angle=[All angles] process_channel=[All channels]" +
+    " process_illumination=[All illuminations] process_tile=[All tiles] process_timepoint=[All Timepoints]" +
+    " method=[Phase Correlation] show_expert_grouping_options" +
+    " how_to_treat_timepoints=group how_to_treat_channels=group how_to_treat_illuminations=group" +
+    " how_to_treat_angles=group how_to_treat_tiles=compare" +
+    " channels=[Average Channels]" +
+    " downsample_in_x={downsample} downsample_in_y={downsample} downsample_in_z={downsample}");
+
+run("Filter pairwise shifts ...",
+"select={process_xml} filter_by_link_quality min_r={min_correlation}" +
+" max_r=1 max_shift_in_x={max_shift_in_x} max_shift_in_y={max_shift_in_y}" +
+" max_shift_in_z={max_shift_in_z}");
+
+// do global optimization
+run("Optimize globally and apply shifts ...",
+    "select={process_xml} process_angle=[All angles] process_channel=[All channels] " +
+    "process_illumination=[All illuminations] process_tile=[All tiles]" +
+    " process_timepoint=[All Timepoints]" +
+    " relative=2.500 absolute=3.500 global_optimization_strategy=" +
+    "[Two-Round using Metadata to align unconnected Tiles] fix_group_0-0,");
+
+eval("script", "System.exit(0);");
+"""
+
     MACRO_IP_DET = """
 run("Memory & Threads...", "parallel={parallel:d}");
 run("Detect Interest Points for Registration",
 "select={process_xml} process_angle=[All angles] process_channel=[All channels] " +
 "process_illumination=[All illuminations] process_tile=[All tiles] process_timepoint=[All Timepoints] " +
 "type_of_interest_point_detection=Difference-of-Gaussian label_interest_points=beads " +
 "subpixel_localization=[3-dimensional quadratic fit] " +
@@ -153,7 +181,26 @@
             )
         fparams["select_reference_views"] = ""
         if P["map_back_views_choice"] in ("selected_translation", "selected_rigid"):
             fparams[
                 "select_reference_views"
             ] = " select_reference_views=[ViewSetupId:{:d} Timepoint:0]".format(P["map_back_reference_view"])
         return ImagejMacros.MACRO_IP_REG.format(**fparams)
+
+    @staticmethod
+    def get_macro_phase_correlation(P: Dict[str, Any]) -> str:
+        """ Get a parameter formatted phase correlation macro.
+
+        Parameters
+        ----------
+        P : `dict`
+          Parameter dictionary for macro formatting.
+            Note: Will already have
+                process_xml: path to xml to process
+                downsample: pyramid level to use
+                min_correlation: minimum correlation to consider
+                max_shift_in_x: maximum shift in x
+                max_shift_in_y: maximum shift in y
+                max_shift_in_z: maximum shift in z
+        """
+        fparams = dict(P)
+        return ImagejMacros.MACRO_PHASE_CORRELATION.format(**fparams)
```

### Comparing `aind_exaspim_pipeline_utils-0.8.3/src/aind_exaspim_pipeline_utils/imagej_wrapper.py` & `aind_exaspim_pipeline_utils-0.9.0/src/aind_exaspim_pipeline_utils/imagej_wrapper.py`

 * *Files 9% similar despite different names*

```diff
@@ -18,23 +18,45 @@
 import s3fs
 from aind_data_schema.processing import DataProcess, ProcessName
 import xml.etree.ElementTree as ET
 
 # from aind_data_schema import DataProcess
 # from aind_data_schema.processing import ProcessName
 
-
 from . import __version__
 from .imagej_macros import ImagejMacros
 from .exaspim_manifest import get_capsule_manifest, write_process_metadata, ExaspimProcessingPipeline
 from .qc import bigstitcher_log_edge_analysis
 from .qc.create_ng_link import create_ng_link
 
 
+class PhaseCorrelationSchema(argschema.ArgSchema):  # pragma: no cover
+
+    """Adjustable parameters for phase correlation."""
+
+    downsample = fld.Int(
+        required=True,
+        metadata={"description": "Downsampling factor. Use the one that is available in the dataset."},
+    )
+    min_correlation = fld.Float(
+        load_default=0.6, metadata={"description": "Minimum correlation value for phase correlation."},
+    )
+    max_shift_in_x = fld.Int(
+        load_default=0, metadata={"description": "Maximum displacement in x direction."},
+    )
+    max_shift_in_y = fld.Int(
+        load_default=0, metadata={"description": "Maximum displacement in y direction."},
+    )
+    max_shift_in_z = fld.Int(
+        load_default=0, metadata={"description": "Maximum displacement in z direction."},
+    )
+
+
 class IPDetectionSchema(argschema.ArgSchema):  # pragma: no cover
+
     """Adjustable parameters to detect IP."""
 
     downsample = fld.Int(
         required=True,
         metadata={"description": "Downsampling factor. Use the one that is available in the dataset."},
     )
     bead_choice = fld.String(
@@ -148,28 +170,35 @@
     )
     parallel = fld.Int(
         required=True,
         metadata={"description": "Number of parallel Java worker threads."},
         validate=mm.validate.Range(min=1, max=128),
     )
     dataset_xml = fld.String(required=True, metadata={"description": "Input xml dataset definition"})
+    phase_correlation_params = fld.Nested(
+        PhaseCorrelationSchema, required=False, metadata={"description": "Phase correlation parameters"}
+    )
     do_detection = fld.Boolean(required=True, metadata={"description": "Do interest point detection?"})
     ip_detection_params = fld.Nested(
         IPDetectionSchema, required=False, metadata={"description": "Interest point detection parameters"}
     )
     do_registrations = fld.Boolean(
         required=True,
         metadata={"description": "Do first transformation fitting ?"},
     )
     ip_registrations_params = fld.Nested(
         IPRegistrationSchema,
         required=False,
         metadata={"description": "Registration parameters (do_registrations==True only)"},
         many=True,
     )
+    do_phase_correlation = fld.Boolean(
+        required=False,
+        metadata={"description": "Do phase correlation for affine only?"},
+    )
 
 
 def print_output(data, f, stderr=False) -> None:  # pragma: no cover
     """Print output to stdout or stderr and to a file if specified."""
     if stderr:
         print(data, end="", file=sys.stderr, flush=True)
     else:
@@ -275,20 +304,23 @@
         d = 5
     mem_GB -= d
     if mem_GB < 10:
         raise ValueError("Too little memory available")
 
     process_xml = "../results/bigstitcher.xml"
     macro_ip_det = "../results/macro_ip_det.ijm"
+    macro_phase_corr = "../results/macro_phase_corr.ijm"
+
     return {
         "process_xml": process_xml,
         # Do not use, this is the whole VM at the moment, not what is available for the capsule
         "auto_ncpu": ncpu,
         "auto_memgb": mem_GB,
         "macro_ip_det": macro_ip_det,
+        "macro_phase_corr": macro_phase_corr,
     }
 
 
 def main():  # pragma: no cover
     """Entry point if run as a standalone program. This uses the old-style config."""
     logging.basicConfig(format="%(asctime)s %(levelname)-7s %(message)s")
 
@@ -303,14 +335,40 @@
     logger.info("Writing out config.json")
     with open("/results/config.json", "w") as f:
         json.dump(args, f, indent=2)
 
     logger.info("Copying input xml %s -> %s", args["dataset_xml"], args["process_xml"])
     shutil.copy(args["dataset_xml"], args["process_xml"])
 
+    if args['do_phase_correlation']:
+        # logger.info("Creating macro for phase correlation", args["do_phase_correlation"])
+        det_params = dict(args["phase_correlation_params"])
+        det_params["process_xml"] = args["process_xml"]
+        det_params["parallel"] = args["parallel"]
+
+        # write phase correlation macro
+        with open(args["macro_phase_corr"], "w") as f:
+            f.write(ImagejMacros.get_macro_phase_correlation(det_params))
+        # run phase correlation
+        r = wrapper_cmd_run(
+            [
+                "ImageJ",
+                "-Dimagej.updater.disableAutocheck=true",
+                "--headless",
+                "--memory",
+                "{memgb}G".format(**args),
+                "--console",
+                "--run",
+                args["macro_phase_corr"]
+            ],
+            logger,
+        )
+    if r != 0:
+        raise RuntimeError("Phase Correlation command failed.")
+
     if args["do_detection"]:
         det_params = dict(args["ip_detection_params"])
         det_params["parallel"] = args["parallel"]
         det_params["process_xml"] = args["process_xml"]
         logger.info("Creating macro %s", args["macro_ip_det"])
         with open(args["macro_ip_det"], "w") as f:
             f.write(ImagejMacros.get_macro_ip_det(det_params))
```

### Comparing `aind_exaspim_pipeline_utils-0.8.3/src/aind_exaspim_pipeline_utils/java_utils.py` & `aind_exaspim_pipeline_utils-0.9.0/src/aind_exaspim_pipeline_utils/java_utils.py`

 * *Files identical despite different names*

### Comparing `aind_exaspim_pipeline_utils-0.8.3/src/aind_exaspim_pipeline_utils/n5tozarr/n5tozarr_da.py` & `aind_exaspim_pipeline_utils-0.9.0/src/aind_exaspim_pipeline_utils/n5tozarr/n5tozarr_da.py`

 * *Files identical despite different names*

### Comparing `aind_exaspim_pipeline_utils-0.8.3/src/aind_exaspim_pipeline_utils/qc/bigstitcher_log_edge_analysis.py` & `aind_exaspim_pipeline_utils-0.9.0/src/aind_exaspim_pipeline_utils/qc/bigstitcher_log_edge_analysis.py`

 * *Files identical despite different names*

### Comparing `aind_exaspim_pipeline_utils-0.8.3/src/aind_exaspim_pipeline_utils/qc/create_ng_link.py` & `aind_exaspim_pipeline_utils-0.9.0/src/aind_exaspim_pipeline_utils/qc/create_ng_link.py`

 * *Files identical despite different names*

### Comparing `aind_exaspim_pipeline_utils-0.8.3/src/aind_exaspim_pipeline_utils/qc/ng_ip_visualization.py` & `aind_exaspim_pipeline_utils-0.9.0/src/aind_exaspim_pipeline_utils/qc/ng_ip_visualization.py`

 * *Files identical despite different names*

### Comparing `aind_exaspim_pipeline_utils-0.8.3/src/aind_exaspim_pipeline_utils/trigger/capsule.py` & `aind_exaspim_pipeline_utils-0.9.0/src/aind_exaspim_pipeline_utils/trigger/capsule.py`

 * *Files identical despite different names*

### Comparing `aind_exaspim_pipeline_utils-0.8.3/src/aind_exaspim_pipeline_utils.egg-info/PKG-INFO` & `aind_exaspim_pipeline_utils-0.9.0/src/aind_exaspim_pipeline_utils.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aind_exaspim_pipeline_utils
-Version: 0.8.3
+Version: 0.9.0
 Summary: AIND exaSPIM pipeline utilities.
 Author: Allen Institute for Neural Dynamics
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `aind_exaspim_pipeline_utils-0.8.3/src/aind_exaspim_pipeline_utils.egg-info/SOURCES.txt` & `aind_exaspim_pipeline_utils-0.9.0/src/aind_exaspim_pipeline_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aind_exaspim_pipeline_utils-0.8.3/src/aind_exaspim_pipeline_utils.egg-info/entry_points.txt` & `aind_exaspim_pipeline_utils-0.9.0/src/aind_exaspim_pipeline_utils.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `aind_exaspim_pipeline_utils-0.8.3/src/aind_trigger_codeocean/pipelines.py` & `aind_exaspim_pipeline_utils-0.9.0/src/aind_trigger_codeocean/pipelines.py`

 * *Files identical despite different names*

### Comparing `aind_exaspim_pipeline_utils-0.8.3/tests/test_capsule.py` & `aind_exaspim_pipeline_utils-0.9.0/tests/test_capsule.py`

 * *Files identical despite different names*

### Comparing `aind_exaspim_pipeline_utils-0.8.3/tests/test_imagej_wrapper.py` & `aind_exaspim_pipeline_utils-0.9.0/tests/test_imagej_wrapper.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 """Tests for ImageJ wrapper functions and macro creator class"""
+import argschema
 import contextlib
 import io
 import logging
 import unittest
 from unittest import mock
 
-import argschema
-
 from aind_exaspim_pipeline_utils.imagej_macros import ImagejMacros
 from aind_exaspim_pipeline_utils.imagej_wrapper import (
     ImageJWrapperSchema,
     get_auto_parameters,
     wrapper_cmd_run,
 )
 
@@ -88,20 +87,42 @@
                     "map_back_views_choice": "no_mapback",
                     "map_back_reference_view": 5,
                     "do_regularize": True,
                     "regularize_with_choice": "rigid",
                 }
             ],
         }
+        example_params_phase_correlation_default = {
+            "session_id": "2023-02-22",
+            "memgb": 55,
+            "parallel": 8,
+            "dataset_xml": "test_dataset.xml",
+            "do_phase_correlation": True,
+            "do_detection": False,
+            "do_registrations": False,
+            "phase_correlation_params": {
+                "downsample": 2,
+                "min_correlation": 0.6,
+                "max_shift_in_x": 10,
+                "max_shift_in_y": 10,
+                "max_shift_in_z": 10,
+                },
+        }
         parser = argschema.ArgSchemaParser(
             schema_type=ImageJWrapperSchema, input_data=example_params_default, args=[]
         )
         self.args = parser.args
 
+        phase_parser = argschema.ArgSchemaParser(
+            schema_type=ImageJWrapperSchema, input_data=example_params_phase_correlation_default, args=[]
+        )
+        self.phase_args = phase_parser.args
+
     def testMacroIPDet(self):
+
         """Test IP Detection macro"""
 
         det_params = dict(self.args["ip_detection_params"])
         det_params["process_xml"] = self.args["dataset_xml"]
         det_params["parallel"] = self.args["parallel"]
 
         m = ImagejMacros.get_macro_ip_det(det_params)
@@ -125,7 +146,17 @@
         reg_params["fix_views_choice"] = "select_fixed"
         m = ImagejMacros.get_macro_ip_reg(reg_params)
         self.assertRegex(m, "viewsetupid_10_timepoint_0")
 
         reg_params["map_back_views_choice"] = "selected_translation"
         m = ImagejMacros.get_macro_ip_reg(reg_params)
         self.assertRegex(m, "ViewSetupId:5")
+
+    def testMacroPhaseCorrelation(self):
+        """Test Phase Correlation macro"""
+        phase_params = dict(self.phase_args["phase_correlation_params"])
+        phase_params["process_xml"] = self.phase_args["dataset_xml"]
+        phase_params["parallel"] = self.args["parallel"]
+
+        m = ImagejMacros.get_macro_phase_correlation(phase_params)
+        self.assertRegex(m, "select=test_dataset.xml")
+        self.assertNotRegex(m, "viewsetupid_")
```

### Comparing `aind_exaspim_pipeline_utils-0.8.3/tests/test_n5tozarr.py` & `aind_exaspim_pipeline_utils-0.9.0/tests/test_n5tozarr.py`

 * *Files identical despite different names*

