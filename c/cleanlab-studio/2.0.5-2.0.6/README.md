# Comparing `tmp/cleanlab_studio-2.0.5.tar.gz` & `tmp/cleanlab_studio-2.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cleanlab_studio-2.0.5.tar", last modified: Wed May 22 16:42:39 2024, max compression
+gzip compressed data, was "cleanlab_studio-2.0.6.tar", last modified: Thu May 30 23:13:06 2024, max compression
```

## Comparing `cleanlab_studio-2.0.5.tar` & `cleanlab_studio-2.0.6.tar`

### file list

```diff
@@ -1,84 +1,84 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:42:39.289073 cleanlab_studio-2.0.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-22 16:42:28.000000 cleanlab_studio-2.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    10562 2024-05-22 16:42:39.289073 cleanlab_studio-2.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8784 2024-05-22 16:42:28.000000 cleanlab_studio-2.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:42:39.277073 cleanlab_studio-2.0.5/cleanlab_studio/
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-22 16:42:28.000000 cleanlab_studio-2.0.5/cleanlab_studio/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:42:39.277073 cleanlab_studio-2.0.5/cleanlab_studio/cli/
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-22 16:42:28.000000 cleanlab_studio-2.0.5/cleanlab_studio/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4591 2024-05-22 16:42:28.000000 cleanlab_studio-2.0.5/cleanlab_studio/cli/api_service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:42:39.277073 cleanlab_studio-2.0.5/cleanlab_studio/cli/classes/
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-22 16:42:28.000000 cleanlab_studio-2.0.5/cleanlab_studio/cli/classes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-05-22 16:42:28.000000 cleanlab_studio-2.0.5/cleanlab_studio/cli/classes/csv_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     2134 2024-05-22 16:42:28.000000 cleanlab_studio-2.0.5/cleanlab_studio/cli/classes/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     2429 2024-05-22 16:42:28.000000 cleanlab_studio-2.0.5/cleanlab_studio/cli/classes/excel_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)      886 2024-05-22 16:42:28.000000 cleanlab_studio-2.0.5/cleanlab_studio/cli/classes/json_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:42:39.281072 cleanlab_studio-2.0.5/cleanlab_studio/cli/cleanset/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 16:42:28.000000 cleanlab_studio-2.0.5/cleanlab_studio/cli/cleanset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-05-22 16:42:28.000000 cleanlab_studio-2.0.5/cleanlab_studio/cli/cleanset/commands.py
--rw-r--r--   0 runner    (1001) docker     (127)     4362 2024-05-22 16:42:28.000000 cleanlab_studio-2.0.5/cleanlab_studio/cli/cleanset/download.py
--rw-r--r--   0 runner    (1001) docker     (127)     1430 2024-05-22 16:42:28.000000 cleanlab_studio-2.0.5/cleanlab_studio/cli/cleanset/download_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1853 2024-05-22 16:42:28.000000 cleanlab_studio-2.0.5/cleanlab_studio/cli/click_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:42:39.281072 cleanlab_studio-2.0.5/cleanlab_studio/cli/dataset/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 16:42:28.000000 cleanlab_studio-2.0.5/cleanlab_studio/cli/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-05-22 16:42:28.000000 cleanlab_studio-2.0.5/cleanlab_studio/cli/dataset/commands.py
--rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-05-22 16:42:28.000000 cleanlab_studio-2.0.5/cleanlab_studio/cli/dataset/schema_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1806 2024-05-22 16:42:28.000000 cleanlab_studio-2.0.5/cleanlab_studio/cli/dataset/upload.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:42:39.281072 cleanlab_studio-2.0.5/cleanlab_studio/cli/decorators/
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-22 16:42:28.000000 cleanlab_studio-2.0.5/cleanlab_studio/cli/decorators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      974 2024-05-22 16:42:28.000000 cleanlab_studio-2.0.5/cleanlab_studio/cli/decorators/auth_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1805 2024-05-22 16:42:28.000000 cleanlab_studio-2.0.5/cleanlab_studio/cli/decorators/previous_state.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:42:39.281072 cleanlab_studio-2.0.5/cleanlab_studio/cli/login/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 16:42:28.000000 cleanlab_studio-2.0.5/cleanlab_studio/cli/login/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1891 2024-05-22 16:42:28.000000 cleanlab_studio-2.0.5/cleanlab_studio/cli/login/login.py
--rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-05-22 16:42:28.000000 cleanlab_studio-2.0.5/cleanlab_studio/cli/main.py
--rw-r--r--   0 runner    (1001) docker     (127)      694 2024-05-22 16:42:28.000000 cleanlab_studio-2.0.5/cleanlab_studio/cli/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     4870 2024-05-22 16:42:28.000000 cleanlab_studio-2.0.5/cleanlab_studio/cli/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     2619 2024-05-22 16:42:28.000000 cleanlab_studio-2.0.5/cleanlab_studio/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:42:39.281072 cleanlab_studio-2.0.5/cleanlab_studio/internal/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 16:42:28.000000 cleanlab_studio-2.0.5/cleanlab_studio/internal/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:42:39.285072 cleanlab_studio-2.0.5/cleanlab_studio/internal/api/
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-22 16:42:28.000000 cleanlab_studio-2.0.5/cleanlab_studio/internal/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24527 2024-05-22 16:42:28.000000 cleanlab_studio-2.0.5/cleanlab_studio/internal/api/api.py
--rw-r--r--   0 runner    (1001) docker     (127)      336 2024-05-22 16:42:28.000000 cleanlab_studio-2.0.5/cleanlab_studio/internal/api/api_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     4297 2024-05-22 16:42:28.000000 cleanlab_studio-2.0.5/cleanlab_studio/internal/clean_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-22 16:42:28.000000 cleanlab_studio-2.0.5/cleanlab_studio/internal/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:42:39.285072 cleanlab_studio-2.0.5/cleanlab_studio/internal/dataset_source/
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-22 16:42:28.000000 cleanlab_studio-2.0.5/cleanlab_studio/internal/dataset_source/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1215 2024-05-22 16:42:28.000000 cleanlab_studio-2.0.5/cleanlab_studio/internal/dataset_source/dataframe_dataset_source.py
--rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-05-22 16:42:28.000000 cleanlab_studio-2.0.5/cleanlab_studio/internal/dataset_source/dataset_source.py
--rw-r--r--   0 runner    (1001) docker     (127)      989 2024-05-22 16:42:28.000000 cleanlab_studio-2.0.5/cleanlab_studio/internal/dataset_source/filepath_dataset_source.py
--rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-22 16:42:28.000000 cleanlab_studio-2.0.5/cleanlab_studio/internal/dataset_source/pandas_dataset_source.py
--rw-r--r--   0 runner    (1001) docker     (127)      668 2024-05-22 16:42:28.000000 cleanlab_studio-2.0.5/cleanlab_studio/internal/dataset_source/pyspark_dataset_source.py
--rw-r--r--   0 runner    (1001) docker     (127)      717 2024-05-22 16:42:28.000000 cleanlab_studio-2.0.5/cleanlab_studio/internal/dataset_source/snowpark_dataset_source.py
--rw-r--r--   0 runner    (1001) docker     (127)     5144 2024-05-22 16:42:28.000000 cleanlab_studio-2.0.5/cleanlab_studio/internal/enrichment_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3359 2024-05-22 16:42:28.000000 cleanlab_studio-2.0.5/cleanlab_studio/internal/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:42:39.285072 cleanlab_studio-2.0.5/cleanlab_studio/internal/tlm/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 16:42:28.000000 cleanlab_studio-2.0.5/cleanlab_studio/internal/tlm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4083 2024-05-22 16:42:28.000000 cleanlab_studio-2.0.5/cleanlab_studio/internal/tlm/concurrency.py
--rw-r--r--   0 runner    (1001) docker     (127)     6977 2024-05-22 16:42:28.000000 cleanlab_studio-2.0.5/cleanlab_studio/internal/tlm/validation.py
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-22 16:42:28.000000 cleanlab_studio-2.0.5/cleanlab_studio/internal/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     6141 2024-05-22 16:42:28.000000 cleanlab_studio-2.0.5/cleanlab_studio/internal/upload_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)    11629 2024-05-22 16:42:28.000000 cleanlab_studio-2.0.5/cleanlab_studio/internal/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:42:39.285072 cleanlab_studio-2.0.5/cleanlab_studio/studio/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 16:42:28.000000 cleanlab_studio-2.0.5/cleanlab_studio/studio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7396 2024-05-22 16:42:28.000000 cleanlab_studio-2.0.5/cleanlab_studio/studio/inference.py
--rw-r--r--   0 runner    (1001) docker     (127)    25333 2024-05-22 16:42:28.000000 cleanlab_studio-2.0.5/cleanlab_studio/studio/studio.py
--rw-r--r--   0 runner    (1001) docker     (127)    30336 2024-05-22 16:42:28.000000 cleanlab_studio-2.0.5/cleanlab_studio/studio/trustworthy_language_model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:42:39.285072 cleanlab_studio-2.0.5/cleanlab_studio/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 16:42:28.000000 cleanlab_studio-2.0.5/cleanlab_studio/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:42:39.285072 cleanlab_studio-2.0.5/cleanlab_studio/utils/data_enrichment/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 16:42:28.000000 cleanlab_studio-2.0.5/cleanlab_studio/utils/data_enrichment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9778 2024-05-22 16:42:28.000000 cleanlab_studio-2.0.5/cleanlab_studio/utils/data_enrichment/enrich.py
--rw-r--r--   0 runner    (1001) docker     (127)     7793 2024-05-22 16:42:28.000000 cleanlab_studio-2.0.5/cleanlab_studio/utils/synthetic.py
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-22 16:42:28.000000 cleanlab_studio-2.0.5/cleanlab_studio/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:42:39.289073 cleanlab_studio-2.0.5/cleanlab_studio.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10562 2024-05-22 16:42:39.000000 cleanlab_studio-2.0.5/cleanlab_studio.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2629 2024-05-22 16:42:39.000000 cleanlab_studio-2.0.5/cleanlab_studio.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 16:42:39.000000 cleanlab_studio-2.0.5/cleanlab_studio.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-22 16:42:39.000000 cleanlab_studio-2.0.5/cleanlab_studio.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      304 2024-05-22 16:42:39.000000 cleanlab_studio-2.0.5/cleanlab_studio.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-22 16:42:39.000000 cleanlab_studio-2.0.5/cleanlab_studio.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-05-22 16:42:28.000000 cleanlab_studio-2.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 16:42:39.289073 cleanlab_studio-2.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2314 2024-05-22 16:42:28.000000 cleanlab_studio-2.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 23:13:06.907467 cleanlab_studio-2.0.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-30 23:12:57.000000 cleanlab_studio-2.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    10562 2024-05-30 23:13:06.903467 cleanlab_studio-2.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8784 2024-05-30 23:12:57.000000 cleanlab_studio-2.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 23:13:06.895466 cleanlab_studio-2.0.6/cleanlab_studio/
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-30 23:12:57.000000 cleanlab_studio-2.0.6/cleanlab_studio/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 23:13:06.899467 cleanlab_studio-2.0.6/cleanlab_studio/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-30 23:12:57.000000 cleanlab_studio-2.0.6/cleanlab_studio/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4591 2024-05-30 23:12:57.000000 cleanlab_studio-2.0.6/cleanlab_studio/cli/api_service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 23:13:06.899467 cleanlab_studio-2.0.6/cleanlab_studio/cli/classes/
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-30 23:12:57.000000 cleanlab_studio-2.0.6/cleanlab_studio/cli/classes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-05-30 23:12:57.000000 cleanlab_studio-2.0.6/cleanlab_studio/cli/classes/csv_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2134 2024-05-30 23:12:57.000000 cleanlab_studio-2.0.6/cleanlab_studio/cli/classes/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2429 2024-05-30 23:12:57.000000 cleanlab_studio-2.0.6/cleanlab_studio/cli/classes/excel_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)      886 2024-05-30 23:12:57.000000 cleanlab_studio-2.0.6/cleanlab_studio/cli/classes/json_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 23:13:06.899467 cleanlab_studio-2.0.6/cleanlab_studio/cli/cleanset/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 23:12:57.000000 cleanlab_studio-2.0.6/cleanlab_studio/cli/cleanset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-05-30 23:12:57.000000 cleanlab_studio-2.0.6/cleanlab_studio/cli/cleanset/commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4362 2024-05-30 23:12:57.000000 cleanlab_studio-2.0.6/cleanlab_studio/cli/cleanset/download.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1430 2024-05-30 23:12:57.000000 cleanlab_studio-2.0.6/cleanlab_studio/cli/cleanset/download_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1853 2024-05-30 23:12:57.000000 cleanlab_studio-2.0.6/cleanlab_studio/cli/click_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 23:13:06.899467 cleanlab_studio-2.0.6/cleanlab_studio/cli/dataset/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 23:12:57.000000 cleanlab_studio-2.0.6/cleanlab_studio/cli/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-05-30 23:12:57.000000 cleanlab_studio-2.0.6/cleanlab_studio/cli/dataset/commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-05-30 23:12:57.000000 cleanlab_studio-2.0.6/cleanlab_studio/cli/dataset/schema_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1806 2024-05-30 23:12:57.000000 cleanlab_studio-2.0.6/cleanlab_studio/cli/dataset/upload.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 23:13:06.899467 cleanlab_studio-2.0.6/cleanlab_studio/cli/decorators/
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-30 23:12:57.000000 cleanlab_studio-2.0.6/cleanlab_studio/cli/decorators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      974 2024-05-30 23:12:57.000000 cleanlab_studio-2.0.6/cleanlab_studio/cli/decorators/auth_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1805 2024-05-30 23:12:57.000000 cleanlab_studio-2.0.6/cleanlab_studio/cli/decorators/previous_state.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 23:13:06.899467 cleanlab_studio-2.0.6/cleanlab_studio/cli/login/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 23:12:57.000000 cleanlab_studio-2.0.6/cleanlab_studio/cli/login/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1891 2024-05-30 23:12:57.000000 cleanlab_studio-2.0.6/cleanlab_studio/cli/login/login.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-05-30 23:12:57.000000 cleanlab_studio-2.0.6/cleanlab_studio/cli/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-05-30 23:12:57.000000 cleanlab_studio-2.0.6/cleanlab_studio/cli/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4870 2024-05-30 23:12:57.000000 cleanlab_studio-2.0.6/cleanlab_studio/cli/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2739 2024-05-30 23:12:57.000000 cleanlab_studio-2.0.6/cleanlab_studio/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 23:13:06.903467 cleanlab_studio-2.0.6/cleanlab_studio/internal/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 23:12:57.000000 cleanlab_studio-2.0.6/cleanlab_studio/internal/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 23:13:06.903467 cleanlab_studio-2.0.6/cleanlab_studio/internal/api/
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-30 23:12:57.000000 cleanlab_studio-2.0.6/cleanlab_studio/internal/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24710 2024-05-30 23:12:57.000000 cleanlab_studio-2.0.6/cleanlab_studio/internal/api/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-05-30 23:12:57.000000 cleanlab_studio-2.0.6/cleanlab_studio/internal/api/api_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4297 2024-05-30 23:12:57.000000 cleanlab_studio-2.0.6/cleanlab_studio/internal/clean_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-30 23:12:57.000000 cleanlab_studio-2.0.6/cleanlab_studio/internal/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 23:13:06.903467 cleanlab_studio-2.0.6/cleanlab_studio/internal/dataset_source/
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-30 23:12:57.000000 cleanlab_studio-2.0.6/cleanlab_studio/internal/dataset_source/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1215 2024-05-30 23:12:57.000000 cleanlab_studio-2.0.6/cleanlab_studio/internal/dataset_source/dataframe_dataset_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-05-30 23:12:57.000000 cleanlab_studio-2.0.6/cleanlab_studio/internal/dataset_source/dataset_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)      989 2024-05-30 23:12:57.000000 cleanlab_studio-2.0.6/cleanlab_studio/internal/dataset_source/filepath_dataset_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-30 23:12:57.000000 cleanlab_studio-2.0.6/cleanlab_studio/internal/dataset_source/pandas_dataset_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2024-05-30 23:12:57.000000 cleanlab_studio-2.0.6/cleanlab_studio/internal/dataset_source/pyspark_dataset_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)      717 2024-05-30 23:12:57.000000 cleanlab_studio-2.0.6/cleanlab_studio/internal/dataset_source/snowpark_dataset_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5144 2024-05-30 23:12:57.000000 cleanlab_studio-2.0.6/cleanlab_studio/internal/enrichment_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3359 2024-05-30 23:12:57.000000 cleanlab_studio-2.0.6/cleanlab_studio/internal/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 23:13:06.903467 cleanlab_studio-2.0.6/cleanlab_studio/internal/tlm/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 23:12:57.000000 cleanlab_studio-2.0.6/cleanlab_studio/internal/tlm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4295 2024-05-30 23:12:57.000000 cleanlab_studio-2.0.6/cleanlab_studio/internal/tlm/concurrency.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6977 2024-05-30 23:12:57.000000 cleanlab_studio-2.0.6/cleanlab_studio/internal/tlm/validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-30 23:12:57.000000 cleanlab_studio-2.0.6/cleanlab_studio/internal/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6141 2024-05-30 23:12:57.000000 cleanlab_studio-2.0.6/cleanlab_studio/internal/upload_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11629 2024-05-30 23:12:57.000000 cleanlab_studio-2.0.6/cleanlab_studio/internal/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 23:13:06.903467 cleanlab_studio-2.0.6/cleanlab_studio/studio/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 23:12:57.000000 cleanlab_studio-2.0.6/cleanlab_studio/studio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7396 2024-05-30 23:12:57.000000 cleanlab_studio-2.0.6/cleanlab_studio/studio/inference.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25333 2024-05-30 23:12:57.000000 cleanlab_studio-2.0.6/cleanlab_studio/studio/studio.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30336 2024-05-30 23:12:57.000000 cleanlab_studio-2.0.6/cleanlab_studio/studio/trustworthy_language_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 23:13:06.903467 cleanlab_studio-2.0.6/cleanlab_studio/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 23:12:57.000000 cleanlab_studio-2.0.6/cleanlab_studio/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 23:13:06.903467 cleanlab_studio-2.0.6/cleanlab_studio/utils/data_enrichment/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 23:12:57.000000 cleanlab_studio-2.0.6/cleanlab_studio/utils/data_enrichment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9778 2024-05-30 23:12:57.000000 cleanlab_studio-2.0.6/cleanlab_studio/utils/data_enrichment/enrich.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7793 2024-05-30 23:12:57.000000 cleanlab_studio-2.0.6/cleanlab_studio/utils/synthetic.py
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-30 23:12:57.000000 cleanlab_studio-2.0.6/cleanlab_studio/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 23:13:06.903467 cleanlab_studio-2.0.6/cleanlab_studio.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10562 2024-05-30 23:13:06.000000 cleanlab_studio-2.0.6/cleanlab_studio.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2629 2024-05-30 23:13:06.000000 cleanlab_studio-2.0.6/cleanlab_studio.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 23:13:06.000000 cleanlab_studio-2.0.6/cleanlab_studio.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-30 23:13:06.000000 cleanlab_studio-2.0.6/cleanlab_studio.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-05-30 23:13:06.000000 cleanlab_studio-2.0.6/cleanlab_studio.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-30 23:13:06.000000 cleanlab_studio-2.0.6/cleanlab_studio.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-05-30 23:12:57.000000 cleanlab_studio-2.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 23:13:06.907467 cleanlab_studio-2.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2314 2024-05-30 23:12:57.000000 cleanlab_studio-2.0.6/setup.py
```

### Comparing `cleanlab_studio-2.0.5/LICENSE` & `cleanlab_studio-2.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `cleanlab_studio-2.0.5/PKG-INFO` & `cleanlab_studio-2.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cleanlab-studio
-Version: 2.0.5
+Version: 2.0.6
 Summary: Client interface for all things Cleanlab Studio
 Home-page: https://github.com/cleanlab/cleanlab-studio
 Author: Cleanlab Inc
 Author-email: team@cleanlab.ai
 License: MIT
 Project-URL: Bug Tracker, https://github.com/cleanlab/cleanlab-studio/issues
 Project-URL: Documentation, https://help.cleanlab.ai
```

### Comparing `cleanlab_studio-2.0.5/README.md` & `cleanlab_studio-2.0.6/README.md`

 * *Files identical despite different names*

### Comparing `cleanlab_studio-2.0.5/cleanlab_studio/cli/api_service.py` & `cleanlab_studio-2.0.6/cleanlab_studio/cli/api_service.py`

 * *Files identical despite different names*

### Comparing `cleanlab_studio-2.0.5/cleanlab_studio/cli/classes/csv_dataset.py` & `cleanlab_studio-2.0.6/cleanlab_studio/cli/classes/csv_dataset.py`

 * *Files identical despite different names*

### Comparing `cleanlab_studio-2.0.5/cleanlab_studio/cli/classes/dataset.py` & `cleanlab_studio-2.0.6/cleanlab_studio/cli/classes/dataset.py`

 * *Files identical despite different names*

### Comparing `cleanlab_studio-2.0.5/cleanlab_studio/cli/classes/excel_dataset.py` & `cleanlab_studio-2.0.6/cleanlab_studio/cli/classes/excel_dataset.py`

 * *Files identical despite different names*

### Comparing `cleanlab_studio-2.0.5/cleanlab_studio/cli/classes/json_dataset.py` & `cleanlab_studio-2.0.6/cleanlab_studio/cli/classes/json_dataset.py`

 * *Files identical despite different names*

### Comparing `cleanlab_studio-2.0.5/cleanlab_studio/cli/cleanset/download.py` & `cleanlab_studio-2.0.6/cleanlab_studio/cli/cleanset/download.py`

 * *Files identical despite different names*

### Comparing `cleanlab_studio-2.0.5/cleanlab_studio/cli/cleanset/download_helpers.py` & `cleanlab_studio-2.0.6/cleanlab_studio/cli/cleanset/download_helpers.py`

 * *Files identical despite different names*

### Comparing `cleanlab_studio-2.0.5/cleanlab_studio/cli/click_helpers.py` & `cleanlab_studio-2.0.6/cleanlab_studio/cli/click_helpers.py`

 * *Files identical despite different names*

### Comparing `cleanlab_studio-2.0.5/cleanlab_studio/cli/dataset/schema_helpers.py` & `cleanlab_studio-2.0.6/cleanlab_studio/cli/dataset/schema_helpers.py`

 * *Files identical despite different names*

### Comparing `cleanlab_studio-2.0.5/cleanlab_studio/cli/dataset/upload.py` & `cleanlab_studio-2.0.6/cleanlab_studio/cli/dataset/upload.py`

 * *Files identical despite different names*

### Comparing `cleanlab_studio-2.0.5/cleanlab_studio/cli/decorators/auth_config.py` & `cleanlab_studio-2.0.6/cleanlab_studio/cli/decorators/auth_config.py`

 * *Files identical despite different names*

### Comparing `cleanlab_studio-2.0.5/cleanlab_studio/cli/decorators/previous_state.py` & `cleanlab_studio-2.0.6/cleanlab_studio/cli/decorators/previous_state.py`

 * *Files identical despite different names*

### Comparing `cleanlab_studio-2.0.5/cleanlab_studio/cli/login/login.py` & `cleanlab_studio-2.0.6/cleanlab_studio/cli/login/login.py`

 * *Files identical despite different names*

### Comparing `cleanlab_studio-2.0.5/cleanlab_studio/cli/main.py` & `cleanlab_studio-2.0.6/cleanlab_studio/cli/main.py`

 * *Files identical despite different names*

### Comparing `cleanlab_studio-2.0.5/cleanlab_studio/cli/types.py` & `cleanlab_studio-2.0.6/cleanlab_studio/cli/types.py`

 * *Files identical despite different names*

### Comparing `cleanlab_studio-2.0.5/cleanlab_studio/cli/util.py` & `cleanlab_studio-2.0.6/cleanlab_studio/cli/util.py`

 * *Files identical despite different names*

### Comparing `cleanlab_studio-2.0.5/cleanlab_studio/errors.py` & `cleanlab_studio-2.0.6/cleanlab_studio/errors.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,14 +82,20 @@
 
 class TlmServerError(APIError):
     def __init__(self, message: str, status_code: int) -> None:
         self.message = message
         self.status_code = status_code
 
 
+class TlmPartialSuccess(APIError):
+    """TLM request partially succeeded. Still returns result to user."""
+
+    pass
+
+
 class UnsupportedVersionError(HandledError):
     def __init__(self) -> None:
         super().__init__(
             "cleanlab-studio is out of date and must be upgraded. Run 'pip install --upgrade cleanlab-studio'."
         )
```

### Comparing `cleanlab_studio-2.0.5/cleanlab_studio/internal/api/api.py` & `cleanlab_studio-2.0.6/cleanlab_studio/internal/api/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 from cleanlab_studio.errors import (
     APIError,
     IngestionError,
     InvalidProjectConfiguration,
     RateLimitError,
     TlmBadRequest,
+    TlmPartialSuccess,
     TlmServerError,
 )
 from cleanlab_studio.internal.tlm.concurrency import TlmRateHandler
 
 import aiohttp
 import aiohttp.client_exceptions
 import requests
@@ -647,14 +648,17 @@
 
             res_json = await res.json()
 
             handle_rate_limit_error_from_resp(res)
             await handle_tlm_client_error_from_resp(res, batch_index)
             await handle_tlm_api_error_from_resp(res, batch_index)
 
+            if not res_json.get("deberta_success", True):
+                raise TlmPartialSuccess("Partial failure on deberta call -- slowdown request rate.")
+
     finally:
         if local_scoped_client:
             await client_session.close()
 
     return cast(JSONDict, res_json)
```

### Comparing `cleanlab_studio-2.0.5/cleanlab_studio/internal/clean_helpers.py` & `cleanlab_studio-2.0.6/cleanlab_studio/internal/clean_helpers.py`

 * *Files identical despite different names*

### Comparing `cleanlab_studio-2.0.5/cleanlab_studio/internal/constants.py` & `cleanlab_studio-2.0.6/cleanlab_studio/internal/constants.py`

 * *Files identical despite different names*

### Comparing `cleanlab_studio-2.0.5/cleanlab_studio/internal/dataset_source/__init__.py` & `cleanlab_studio-2.0.6/cleanlab_studio/internal/dataset_source/__init__.py`

 * *Files identical despite different names*

### Comparing `cleanlab_studio-2.0.5/cleanlab_studio/internal/dataset_source/dataframe_dataset_source.py` & `cleanlab_studio-2.0.6/cleanlab_studio/internal/dataset_source/dataframe_dataset_source.py`

 * *Files identical despite different names*

### Comparing `cleanlab_studio-2.0.5/cleanlab_studio/internal/dataset_source/dataset_source.py` & `cleanlab_studio-2.0.6/cleanlab_studio/internal/dataset_source/dataset_source.py`

 * *Files identical despite different names*

### Comparing `cleanlab_studio-2.0.5/cleanlab_studio/internal/dataset_source/filepath_dataset_source.py` & `cleanlab_studio-2.0.6/cleanlab_studio/internal/dataset_source/filepath_dataset_source.py`

 * *Files identical despite different names*

### Comparing `cleanlab_studio-2.0.5/cleanlab_studio/internal/dataset_source/pyspark_dataset_source.py` & `cleanlab_studio-2.0.6/cleanlab_studio/internal/dataset_source/pyspark_dataset_source.py`

 * *Files identical despite different names*

### Comparing `cleanlab_studio-2.0.5/cleanlab_studio/internal/dataset_source/snowpark_dataset_source.py` & `cleanlab_studio-2.0.6/cleanlab_studio/internal/dataset_source/snowpark_dataset_source.py`

 * *Files identical despite different names*

### Comparing `cleanlab_studio-2.0.5/cleanlab_studio/internal/enrichment_utils.py` & `cleanlab_studio-2.0.6/cleanlab_studio/internal/enrichment_utils.py`

 * *Files identical despite different names*

### Comparing `cleanlab_studio-2.0.5/cleanlab_studio/internal/settings.py` & `cleanlab_studio-2.0.6/cleanlab_studio/internal/settings.py`

 * *Files identical despite different names*

### Comparing `cleanlab_studio-2.0.5/cleanlab_studio/internal/tlm/concurrency.py` & `cleanlab_studio-2.0.6/cleanlab_studio/internal/tlm/concurrency.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import asyncio
 from types import TracebackType
 from typing import Optional, Type
 
-from cleanlab_studio.errors import RateLimitError, TlmServerError
+from cleanlab_studio.errors import RateLimitError, TlmPartialSuccess, TlmServerError
 
 
 class TlmRateHandler:
     """Concurrency handler for TLM queries.
 
     Implements additive increase / multiplicative decrease congestion control algorithm.
     """
@@ -46,28 +46,34 @@
         """Handles exiting from rate limit context. Never suppresses exceptions.
 
         If request succeeded, increase congestion window.
         If request failed due to rate limit error, decrease congestion window.
         If request failed due to 503, decrease congestion window.
         Else if request failed for other reason, don't change congestion window, just exit.
         """
+        swallow_exception: bool = False
+
         if exc_type is None:
             await self._increase_congestion_window()
 
         elif (
             isinstance(exc, RateLimitError)
             or isinstance(exc, TlmServerError)
             and exc.status_code == 503
         ):
             await self._decrease_congestion_window()
 
+        elif isinstance(exc, TlmPartialSuccess):
+            await self._decrease_congestion_window()
+            swallow_exception = True
+
         # release acquired send semaphore from aenter
         self._send_semaphore.release()
 
-        return False
+        return swallow_exception
 
     async def _increase_congestion_window(
         self,
         slow_start_increase_factor: int = SLOW_START_INCREASE_FACTOR,
         additive_increment: int = ADDITIVE_INCREMENT,
         max_concurrent_requests: int = MAX_CONCURRENT_REQUESTS,
     ) -> None:
```

### Comparing `cleanlab_studio-2.0.5/cleanlab_studio/internal/tlm/validation.py` & `cleanlab_studio-2.0.6/cleanlab_studio/internal/tlm/validation.py`

 * *Files identical despite different names*

### Comparing `cleanlab_studio-2.0.5/cleanlab_studio/internal/upload_helpers.py` & `cleanlab_studio-2.0.6/cleanlab_studio/internal/upload_helpers.py`

 * *Files identical despite different names*

### Comparing `cleanlab_studio-2.0.5/cleanlab_studio/internal/util.py` & `cleanlab_studio-2.0.6/cleanlab_studio/internal/util.py`

 * *Files identical despite different names*

### Comparing `cleanlab_studio-2.0.5/cleanlab_studio/studio/inference.py` & `cleanlab_studio-2.0.6/cleanlab_studio/studio/inference.py`

 * *Files identical despite different names*

### Comparing `cleanlab_studio-2.0.5/cleanlab_studio/studio/studio.py` & `cleanlab_studio-2.0.6/cleanlab_studio/studio/studio.py`

 * *Files identical despite different names*

### Comparing `cleanlab_studio-2.0.5/cleanlab_studio/studio/trustworthy_language_model.py` & `cleanlab_studio-2.0.6/cleanlab_studio/studio/trustworthy_language_model.py`

 * *Files identical despite different names*

### Comparing `cleanlab_studio-2.0.5/cleanlab_studio/utils/data_enrichment/enrich.py` & `cleanlab_studio-2.0.6/cleanlab_studio/utils/data_enrichment/enrich.py`

 * *Files identical despite different names*

### Comparing `cleanlab_studio-2.0.5/cleanlab_studio/utils/synthetic.py` & `cleanlab_studio-2.0.6/cleanlab_studio/utils/synthetic.py`

 * *Files identical despite different names*

### Comparing `cleanlab_studio-2.0.5/cleanlab_studio.egg-info/PKG-INFO` & `cleanlab_studio-2.0.6/cleanlab_studio.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cleanlab-studio
-Version: 2.0.5
+Version: 2.0.6
 Summary: Client interface for all things Cleanlab Studio
 Home-page: https://github.com/cleanlab/cleanlab-studio
 Author: Cleanlab Inc
 Author-email: team@cleanlab.ai
 License: MIT
 Project-URL: Bug Tracker, https://github.com/cleanlab/cleanlab-studio/issues
 Project-URL: Documentation, https://help.cleanlab.ai
```

### Comparing `cleanlab_studio-2.0.5/cleanlab_studio.egg-info/SOURCES.txt` & `cleanlab_studio-2.0.6/cleanlab_studio.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cleanlab_studio-2.0.5/setup.py` & `cleanlab_studio-2.0.6/setup.py`

 * *Files identical despite different names*

