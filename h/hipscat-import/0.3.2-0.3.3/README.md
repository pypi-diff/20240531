# Comparing `tmp/hipscat_import-0.3.2.tar.gz` & `tmp/hipscat_import-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hipscat_import-0.3.2.tar", last modified: Wed May 15 19:40:07 2024, max compression
+gzip compressed data, was "hipscat_import-0.3.3.tar", last modified: Fri May 31 20:05:56 2024, max compression
```

## Comparing `hipscat_import-0.3.2.tar` & `hipscat_import-0.3.3.tar`

### file list

```diff
@@ -1,287 +1,289 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:40:07.394019 hipscat_import-0.3.2/
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/.copier-answers.yml
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/.git_archival.txt
--rw-r--r--   0 runner    (1001) docker     (127)      747 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:40:07.346019 hipscat_import-0.3.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:40:07.346019 hipscat_import-0.3.2/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/.github/ISSUE_TEMPLATE/0-general_issue.md
--rw-r--r--   0 runner    (1001) docker     (127)      660 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/.github/ISSUE_TEMPLATE/1-bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      706 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/.github/ISSUE_TEMPLATE/2-feature_request.md
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/.github/dependabot.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3329 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:40:07.346019 hipscat_import-0.3.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      358 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/.github/workflows/add-issue-to-project-tracker.yml
--rw-r--r--   0 runner    (1001) docker     (127)      929 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/.github/workflows/build-documentation.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/.github/workflows/pre-commit-ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)      951 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2423 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/.github/workflows/smoke-test.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1258 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/.github/workflows/testing-and-coverage.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     5719 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1539 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/.setup_dev.sh
--rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5495 2024-05-15 19:40:07.394019 hipscat_import-0.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2585 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:40:07.350019 hipscat_import-0.3.2/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:40:07.350019 hipscat_import-0.3.2/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/docs/_static/custom.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:40:07.350019 hipscat_import-0.3.2/docs/catalogs/
--rw-r--r--   0 runner    (1001) docker     (127)    13620 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/docs/catalogs/arguments.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:40:07.350019 hipscat_import-0.3.2/docs/catalogs/public/
--rw-r--r--   0 runner    (1001) docker     (127)     2252 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/docs/catalogs/public/allwise.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/docs/catalogs/public/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2545 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/docs/catalogs/public/neowise.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3050 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/docs/catalogs/public/panstarrs.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2794 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/docs/catalogs/public/sdss.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1948 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/docs/catalogs/public/tic.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3544 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/docs/catalogs/public/zubercal.rst
--rw-r--r--   0 runner    (1001) docker     (127)    10736 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/docs/catalogs/temp_files.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2454 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:40:07.350019 hipscat_import-0.3.2/docs/guide/
--rw-r--r--   0 runner    (1001) docker     (127)      536 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/docs/guide/contact.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5302 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/docs/guide/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/docs/guide/dask_on_ray.rst
--rw-r--r--   0 runner    (1001) docker     (127)    12082 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/docs/guide/index_table.rst
--rw-r--r--   0 runner    (1001) docker     (127)     6496 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/docs/guide/margin_cache.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2966 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:40:07.354019 hipscat_import-0.3.2/docs/notebooks/
--rwxr-xr-x   0 runner    (1001) docker     (127)     7615 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/docs/notebooks/estimate_pixel_threshold.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    10364 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/docs/notebooks/unequal_schema.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)      241 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/docs/notebooks.rst
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:40:07.354019 hipscat_import-0.3.2/docs/static/
--rw-r--r--   0 runner    (1001) docker     (127)   136863 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/docs/static/allwise_schema.parquet
--rw-r--r--   0 runner    (1001) docker     (127)     4576 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/docs/static/allwise_types.csv
--rw-r--r--   0 runner    (1001) docker     (127)    66486 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/docs/static/neowise_schema.parquet
--rw-r--r--   0 runner    (1001) docker     (127)     2224 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/docs/static/neowise_types.csv
--rw-r--r--   0 runner    (1001) docker     (127)      971 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/docs/static/ps1_detections_types.csv
--rw-r--r--   0 runner    (1001) docker     (127)     2503 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/docs/static/ps1_otmo_types.csv
--rw-r--r--   0 runner    (1001) docker     (127)   412559 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/docs/static/sdss_wget.bash
--rw-r--r--   0 runner    (1001) docker     (127)    57050 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/docs/static/tic_schema.parquet
--rw-r--r--   0 runner    (1001) docker     (127)     1781 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/docs/static/tic_types.csv
--rw-r--r--   0 runner    (1001) docker     (127)     2250 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 19:40:07.394019 hipscat_import-0.3.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:40:07.354019 hipscat_import-0.3.2/src/
--rw-r--r--   0 runner    (1001) docker     (127)    20810 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/src/.pylintrc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:40:07.354019 hipscat_import-0.3.2/src/hipscat_import/
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/src/hipscat_import/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-15 19:40:07.000000 hipscat_import-0.3.2/src/hipscat_import/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:40:07.358019 hipscat_import-0.3.2/src/hipscat_import/catalog/
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/src/hipscat_import/catalog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8559 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/src/hipscat_import/catalog/arguments.py
--rw-r--r--   0 runner    (1001) docker     (127)    11014 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/src/hipscat_import/catalog/file_readers.py
--rw-r--r--   0 runner    (1001) docker     (127)    12421 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/src/hipscat_import/catalog/map_reduce.py
--rw-r--r--   0 runner    (1001) docker     (127)    10600 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/src/hipscat_import/catalog/resume_plan.py
--rw-r--r--   0 runner    (1001) docker     (127)     7129 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/src/hipscat_import/catalog/run_import.py
--rw-r--r--   0 runner    (1001) docker     (127)     3281 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/src/hipscat_import/catalog/sparse_histogram.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:40:07.358019 hipscat_import-0.3.2/src/hipscat_import/index/
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/src/hipscat_import/index/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3678 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/src/hipscat_import/index/arguments.py
--rw-r--r--   0 runner    (1001) docker     (127)     2837 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/src/hipscat_import/index/map_reduce.py
--rw-r--r--   0 runner    (1001) docker     (127)     1788 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/src/hipscat_import/index/run_index.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:40:07.358019 hipscat_import-0.3.2/src/hipscat_import/margin_cache/
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/src/hipscat_import/margin_cache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6164 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/src/hipscat_import/margin_cache/margin_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     3395 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/src/hipscat_import/margin_cache/margin_cache_arguments.py
--rw-r--r--   0 runner    (1001) docker     (127)     5115 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/src/hipscat_import/margin_cache/margin_cache_map_reduce.py
--rw-r--r--   0 runner    (1001) docker     (127)     3266 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/src/hipscat_import/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     8619 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/src/hipscat_import/pipeline_resume_plan.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/src/hipscat_import/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     6649 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/src/hipscat_import/runtime_arguments.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:40:07.362019 hipscat_import-0.3.2/src/hipscat_import/soap/
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/src/hipscat_import/soap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3613 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/src/hipscat_import/soap/arguments.py
--rw-r--r--   0 runner    (1001) docker     (127)    10151 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/src/hipscat_import/soap/map_reduce.py
--rw-r--r--   0 runner    (1001) docker     (127)     9464 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/src/hipscat_import/soap/resume_plan.py
--rw-r--r--   0 runner    (1001) docker     (127)     3713 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/src/hipscat_import/soap/run_soap.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:40:07.362019 hipscat_import-0.3.2/src/hipscat_import/verification/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/src/hipscat_import/verification/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1863 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/src/hipscat_import/verification/arguments.py
--rw-r--r--   0 runner    (1001) docker     (127)      536 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/src/hipscat_import/verification/run_verification.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:40:07.394019 hipscat_import-0.3.2/src/hipscat_import.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5495 2024-05-15 19:40:07.000000 hipscat_import-0.3.2/src/hipscat_import.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11937 2024-05-15 19:40:07.000000 hipscat_import-0.3.2/src/hipscat_import.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 19:40:07.000000 hipscat_import-0.3.2/src/hipscat_import.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-05-15 19:40:07.000000 hipscat_import-0.3.2/src/hipscat_import.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-15 19:40:07.000000 hipscat_import-0.3.2/src/hipscat_import.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:40:07.362019 hipscat_import-0.3.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    20888 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (127)     1316 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:40:07.362019 hipscat_import-0.3.2/tests/hipscat_import/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:40:07.362019 hipscat_import-0.3.2/tests/hipscat_import/catalog/
--rw-r--r--   0 runner    (1001) docker     (127)     7287 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/catalog/test_argument_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)     9452 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/catalog/test_file_readers.py
--rw-r--r--   0 runner    (1001) docker     (127)    17183 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/catalog/test_map_reduce.py
--rw-r--r--   0 runner    (1001) docker     (127)     8076 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/catalog/test_resume_plan.py
--rw-r--r--   0 runner    (1001) docker     (127)    12967 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/catalog/test_run_import.py
--rw-r--r--   0 runner    (1001) docker     (127)    22142 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/catalog/test_run_round_trip.py
--rw-r--r--   0 runner    (1001) docker     (127)     2391 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/catalog/test_sparse_histogram.py
--rw-r--r--   0 runner    (1001) docker     (127)     9441 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:40:07.342018 hipscat_import-0.3.2/tests/hipscat_import/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:40:07.362019 hipscat_import-0.3.2/tests/hipscat_import/data/blank/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/data/blank/blank.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:40:07.362019 hipscat_import-0.3.2/tests/hipscat_import/data/mixed_schema/
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/data/mixed_schema/input_01.csv
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/data/mixed_schema/input_02.csv
--rw-r--r--   0 runner    (1001) docker     (127)     4513 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/data/mixed_schema/schema.parquet
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:40:07.338019 hipscat_import-0.3.2/tests/hipscat_import/data/parquet_shards/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:40:07.338019 hipscat_import-0.3.2/tests/hipscat_import/data/parquet_shards/order_0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:40:07.338019 hipscat_import-0.3.2/tests/hipscat_import/data/parquet_shards/order_0/dir_0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:40:07.366019 hipscat_import-0.3.2/tests/hipscat_import/data/parquet_shards/order_0/dir_0/pixel_11/
--rw-r--r--   0 runner    (1001) docker     (127)     4084 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/data/parquet_shards/order_0/dir_0/pixel_11/shard_0_0.parquet
--rw-r--r--   0 runner    (1001) docker     (127)     4104 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/data/parquet_shards/order_0/dir_0/pixel_11/shard_1_0.parquet
--rw-r--r--   0 runner    (1001) docker     (127)     4090 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/data/parquet_shards/order_0/dir_0/pixel_11/shard_2_0.parquet
--rw-r--r--   0 runner    (1001) docker     (127)     4110 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/data/parquet_shards/order_0/dir_0/pixel_11/shard_3_0.parquet
--rw-r--r--   0 runner    (1001) docker     (127)     4123 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/data/parquet_shards/order_0/dir_0/pixel_11/shard_4_0.parquet
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:40:07.338019 hipscat_import-0.3.2/tests/hipscat_import/data/parquet_shards/order_1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:40:07.342018 hipscat_import-0.3.2/tests/hipscat_import/data/parquet_shards/order_1/dir_0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:40:07.366019 hipscat_import-0.3.2/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_44/
--rw-r--r--   0 runner    (1001) docker     (127)     3809 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_44/shard_0_0.parquet
--rw-r--r--   0 runner    (1001) docker     (127)     3903 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_44/shard_1_0.parquet
--rw-r--r--   0 runner    (1001) docker     (127)     3852 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_44/shard_2_0.parquet
--rw-r--r--   0 runner    (1001) docker     (127)     3842 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_44/shard_3_0.parquet
--rw-r--r--   0 runner    (1001) docker     (127)     3905 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_44/shard_4_0.parquet
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:40:07.366019 hipscat_import-0.3.2/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_45/
--rw-r--r--   0 runner    (1001) docker     (127)     3836 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_45/shard_0_0.parquet
--rw-r--r--   0 runner    (1001) docker     (127)     3836 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_45/shard_1_0.parquet
--rw-r--r--   0 runner    (1001) docker     (127)     3804 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_45/shard_2_0.parquet
--rw-r--r--   0 runner    (1001) docker     (127)     3803 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_45/shard_3_0.parquet
--rw-r--r--   0 runner    (1001) docker     (127)     3841 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_45/shard_4_0.parquet
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:40:07.366019 hipscat_import-0.3.2/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_46/
--rw-r--r--   0 runner    (1001) docker     (127)     3898 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_46/shard_0_0.parquet
--rw-r--r--   0 runner    (1001) docker     (127)     3833 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_46/shard_1_0.parquet
--rw-r--r--   0 runner    (1001) docker     (127)     3899 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_46/shard_2_0.parquet
--rw-r--r--   0 runner    (1001) docker     (127)     3891 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_46/shard_3_0.parquet
--rw-r--r--   0 runner    (1001) docker     (127)     3803 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_46/shard_4_0.parquet
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:40:07.370019 hipscat_import-0.3.2/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_47/
--rw-r--r--   0 runner    (1001) docker     (127)     3769 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_47/shard_0_0.parquet
--rw-r--r--   0 runner    (1001) docker     (127)     3769 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_47/shard_1_0.parquet
--rw-r--r--   0 runner    (1001) docker     (127)     3790 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_47/shard_2_0.parquet
--rw-r--r--   0 runner    (1001) docker     (127)     3808 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_47/shard_3_0.parquet
--rw-r--r--   0 runner    (1001) docker     (127)     3822 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_47/shard_4_0.parquet
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:40:07.342018 hipscat_import-0.3.2/tests/hipscat_import/data/resume/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:40:07.342018 hipscat_import-0.3.2/tests/hipscat_import/data/resume/Norder=0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:40:07.370019 hipscat_import-0.3.2/tests/hipscat_import/data/resume/Norder=0/Dir=0/
--rw-r--r--   0 runner    (1001) docker     (127)     8915 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/data/resume/Norder=0/Dir=0/Npix=11.parquet
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:40:07.342018 hipscat_import-0.3.2/tests/hipscat_import/data/resume/Norder=1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:40:07.370019 hipscat_import-0.3.2/tests/hipscat_import/data/resume/Norder=1/Dir=0/
--rw-r--r--   0 runner    (1001) docker     (127)     7210 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/data/resume/Norder=1/Dir=0/Npix=44.parquet
--rw-r--r--   0 runner    (1001) docker     (127)     6973 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/data/resume/Norder=1/Dir=0/Npix=45.parquet
--rw-r--r--   0 runner    (1001) docker     (127)     7216 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/data/resume/Norder=1/Dir=0/Npix=46.parquet
--rw-r--r--   0 runner    (1001) docker     (127)     6741 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/data/resume/Norder=1/Dir=0/Npix=47.parquet
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:40:07.370019 hipscat_import-0.3.2/tests/hipscat_import/data/resume/intermediate/
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/data/resume/intermediate/mapping_histogram.binary
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:40:07.370019 hipscat_import-0.3.2/tests/hipscat_import/data/small_sky/
--rw-r--r--   0 runner    (1001) docker     (127)     2648 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/data/small_sky/catalog.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:40:07.374019 hipscat_import-0.3.2/tests/hipscat_import/data/small_sky_object_catalog/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:40:07.342018 hipscat_import-0.3.2/tests/hipscat_import/data/small_sky_object_catalog/Norder=0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:40:07.374019 hipscat_import-0.3.2/tests/hipscat_import/data/small_sky_object_catalog/Norder=0/Dir=0/
--rw-r--r--   0 runner    (1001) docker     (127)     8880 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/data/small_sky_object_catalog/Norder=0/Dir=0/Npix=11.parquet
--rw-r--r--   0 runner    (1001) docker     (127)     4018 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/data/small_sky_object_catalog/_common_metadata
--rw-r--r--   0 runner    (1001) docker     (127)     5130 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/data/small_sky_object_catalog/_metadata
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/data/small_sky_object_catalog/catalog_info.json
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/data/small_sky_object_catalog/partition_info.csv
--rw-r--r--   0 runner    (1001) docker     (127)  1581120 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/data/small_sky_object_catalog/point_map.fits
--rw-r--r--   0 runner    (1001) docker     (127)     1979 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/data/small_sky_object_catalog/provenance_info.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:40:07.374019 hipscat_import-0.3.2/tests/hipscat_import/data/small_sky_parts/
--rw-r--r--   0 runner    (1001) docker     (127)      528 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/data/small_sky_parts/catalog_00_of_05.csv
--rw-r--r--   0 runner    (1001) docker     (127)      549 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/data/small_sky_parts/catalog_01_of_05.csv
--rw-r--r--   0 runner    (1001) docker     (127)      549 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/data/small_sky_parts/catalog_02_of_05.csv
--rw-r--r--   0 runner    (1001) docker     (127)      549 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/data/small_sky_parts/catalog_03_of_05.csv
--rw-r--r--   0 runner    (1001) docker     (127)      589 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/data/small_sky_parts/catalog_04_of_05.csv
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/data/small_sky_parts/catalog_10_of_05.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:40:07.374019 hipscat_import-0.3.2/tests/hipscat_import/data/small_sky_source/
--rw-r--r--   0 runner    (1001) docker     (127)  1688789 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/data/small_sky_source/small_sky_source.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:40:07.378019 hipscat_import-0.3.2/tests/hipscat_import/data/small_sky_source_catalog/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:40:07.342018 hipscat_import-0.3.2/tests/hipscat_import/data/small_sky_source_catalog/Norder=0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:40:07.378019 hipscat_import-0.3.2/tests/hipscat_import/data/small_sky_source_catalog/Norder=0/Dir=0/
--rw-r--r--   0 runner    (1001) docker     (127)    11421 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/data/small_sky_source_catalog/Norder=0/Dir=0/Npix=4.parquet
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:40:07.342018 hipscat_import-0.3.2/tests/hipscat_import/data/small_sky_source_catalog/Norder=1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:40:07.378019 hipscat_import-0.3.2/tests/hipscat_import/data/small_sky_source_catalog/Norder=1/Dir=0/
--rw-r--r--   0 runner    (1001) docker     (127)   133671 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/data/small_sky_source_catalog/Norder=1/Dir=0/Npix=47.parquet
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:40:07.342018 hipscat_import-0.3.2/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:40:07.382019 hipscat_import-0.3.2/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/
--rw-r--r--   0 runner    (1001) docker     (127)    28346 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=176.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    86262 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=177.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    92634 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=178.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    99874 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=179.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    42177 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=180.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    54742 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=181.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    72960 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=182.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    67771 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=183.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    80265 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=184.parquet
--rw-r--r--   0 runner    (1001) docker     (127)   162064 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=185.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    31761 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=186.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    43705 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=187.parquet
--rw-r--r--   0 runner    (1001) docker     (127)     5525 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/data/small_sky_source_catalog/_common_metadata
--rw-r--r--   0 runner    (1001) docker     (127)    28968 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/data/small_sky_source_catalog/_metadata
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/data/small_sky_source_catalog/catalog_info.json
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/data/small_sky_source_catalog/partition_info.csv
--rw-r--r--   0 runner    (1001) docker     (127)     8640 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/data/small_sky_source_catalog/point_map.fits
--rw-r--r--   0 runner    (1001) docker     (127)     2146 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/data/small_sky_source_catalog/provenance_info.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:40:07.386019 hipscat_import-0.3.2/tests/hipscat_import/data/soap_intermediate/
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/data/soap_intermediate/0_4.csv
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/data/soap_intermediate/1_47.csv
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/data/soap_intermediate/2_176.csv
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/data/soap_intermediate/2_177.csv
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/data/soap_intermediate/2_178.csv
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/data/soap_intermediate/2_179.csv
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/data/soap_intermediate/2_180.csv
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/data/soap_intermediate/2_181.csv
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/data/soap_intermediate/2_182.csv
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/data/soap_intermediate/2_183.csv
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/data/soap_intermediate/2_184.csv
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/data/soap_intermediate/2_185.csv
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/data/soap_intermediate/2_186.csv
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/data/soap_intermediate/2_187.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:40:07.342018 hipscat_import-0.3.2/tests/hipscat_import/data/soap_intermediate/order_0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:40:07.342018 hipscat_import-0.3.2/tests/hipscat_import/data/soap_intermediate/order_0/dir_0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:40:07.386019 hipscat_import-0.3.2/tests/hipscat_import/data/soap_intermediate/order_0/dir_0/pixel_11/
--rw-r--r--   0 runner    (1001) docker     (127)     6838 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/data/soap_intermediate/order_0/dir_0/pixel_11/source_0_4.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    33062 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/data/soap_intermediate/order_0/dir_0/pixel_11/source_1_47.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    10443 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/data/soap_intermediate/order_0/dir_0/pixel_11/source_2_176.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    22870 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/data/soap_intermediate/order_0/dir_0/pixel_11/source_2_177.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    24239 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/data/soap_intermediate/order_0/dir_0/pixel_11/source_2_178.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    25729 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/data/soap_intermediate/order_0/dir_0/pixel_11/source_2_179.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    13370 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/data/soap_intermediate/order_0/dir_0/pixel_11/source_2_180.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    16010 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/data/soap_intermediate/order_0/dir_0/pixel_11/source_2_181.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    19958 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/data/soap_intermediate/order_0/dir_0/pixel_11/source_2_182.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    18844 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/data/soap_intermediate/order_0/dir_0/pixel_11/source_2_183.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    21542 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/data/soap_intermediate/order_0/dir_0/pixel_11/source_2_184.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    39137 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/data/soap_intermediate/order_0/dir_0/pixel_11/source_2_185.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    11136 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/data/soap_intermediate/order_0/dir_0/pixel_11/source_2_186.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    13692 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/data/soap_intermediate/order_0/dir_0/pixel_11/source_2_187.parquet
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:40:07.390019 hipscat_import-0.3.2/tests/hipscat_import/data/test_formats/
--rw-r--r--   0 runner    (1001) docker     (127)     2648 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/data/test_formats/catalog.starr
--rw-r--r--   0 runner    (1001) docker     (127)    45749 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/data/test_formats/gaia_epoch.ecsv
--rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/data/test_formats/gaia_minimum.csv
--rw-r--r--   0 runner    (1001) docker     (127)     5010 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/data/test_formats/gaia_minimum_schema.parquet
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/data/test_formats/headers.csv
--rw-r--r--   0 runner    (1001) docker     (127)     5394 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/data/test_formats/hipscat_index.csv
--rw-r--r--   0 runner    (1001) docker     (127)     4034 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/data/test_formats/hipscat_index.parquet
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/data/test_formats/macauff_metadata.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     4636 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/data/test_formats/pandasindex.parquet
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/data/test_formats/pipe_delimited.csv
--rw-r--r--   0 runner    (1001) docker     (127)    14400 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/data/test_formats/small_sky.fits
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:40:07.390019 hipscat_import-0.3.2/tests/hipscat_import/index/
--rw-r--r--   0 runner    (1001) docker     (127)     5293 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/index/test_index_argument.py
--rw-r--r--   0 runner    (1001) docker     (127)     7110 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/index/test_index_map_reduce.py
--rw-r--r--   0 runner    (1001) docker     (127)     5501 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/index/test_run_index.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:40:07.390019 hipscat_import-0.3.2/tests/hipscat_import/margin_cache/
--rw-r--r--   0 runner    (1001) docker     (127)     3469 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/margin_cache/test_arguments_margin_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     5505 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/margin_cache/test_margin_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     3664 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/margin_cache/test_margin_cache_map_reduce.py
--rw-r--r--   0 runner    (1001) docker     (127)     4086 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/margin_cache/test_margin_round_trip.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:40:07.394019 hipscat_import-0.3.2/tests/hipscat_import/soap/
--rw-r--r--   0 runner    (1001) docker     (127)     2079 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/soap/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     7832 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/soap/test_run_soap.py
--rw-r--r--   0 runner    (1001) docker     (127)     3242 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/soap/test_soap_arguments.py
--rw-r--r--   0 runner    (1001) docker     (127)     6053 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/soap/test_soap_map_reduce.py
--rw-r--r--   0 runner    (1001) docker     (127)     7052 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/soap/test_soap_resume_plan.py
--rw-r--r--   0 runner    (1001) docker     (127)     4790 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/test_pipeline_resume_plan.py
--rw-r--r--   0 runner    (1001) docker     (127)     4217 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/test_runtime_arguments.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:40:07.394019 hipscat_import-0.3.2/tests/hipscat_import/verification/
--rw-r--r--   0 runner    (1001) docker     (127)      908 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/verification/test_run_verification.py
--rw-r--r--   0 runner    (1001) docker     (127)     3021 2024-05-15 19:40:02.000000 hipscat_import-0.3.2/tests/hipscat_import/verification/test_verification_arguments.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:05:56.823187 hipscat_import-0.3.3/
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-05-31 20:05:51.000000 hipscat_import-0.3.3/.copier-answers.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-31 20:05:51.000000 hipscat_import-0.3.3/.git_archival.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      747 2024-05-31 20:05:51.000000 hipscat_import-0.3.3/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:05:56.779187 hipscat_import-0.3.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:05:56.779187 hipscat_import-0.3.3/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-31 20:05:51.000000 hipscat_import-0.3.3/.github/ISSUE_TEMPLATE/0-general_issue.md
+-rw-r--r--   0 runner    (1001) docker     (127)      660 2024-05-31 20:05:51.000000 hipscat_import-0.3.3/.github/ISSUE_TEMPLATE/1-bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      706 2024-05-31 20:05:51.000000 hipscat_import-0.3.3/.github/ISSUE_TEMPLATE/2-feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-31 20:05:51.000000 hipscat_import-0.3.3/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3518 2024-05-31 20:05:51.000000 hipscat_import-0.3.3/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:05:56.779187 hipscat_import-0.3.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2024-05-31 20:05:51.000000 hipscat_import-0.3.3/.github/workflows/add-issue-to-project-tracker.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      929 2024-05-31 20:05:51.000000 hipscat_import-0.3.3/.github/workflows/build-documentation.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-05-31 20:05:51.000000 hipscat_import-0.3.3/.github/workflows/pre-commit-ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      951 2024-05-31 20:05:51.000000 hipscat_import-0.3.3/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2423 2024-05-31 20:05:51.000000 hipscat_import-0.3.3/.github/workflows/smoke-test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1258 2024-05-31 20:05:51.000000 hipscat_import-0.3.3/.github/workflows/testing-and-coverage.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-05-31 20:05:51.000000 hipscat_import-0.3.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     5719 2024-05-31 20:05:51.000000 hipscat_import-0.3.3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-31 20:05:51.000000 hipscat_import-0.3.3/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1539 2024-05-31 20:05:51.000000 hipscat_import-0.3.3/.setup_dev.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-05-31 20:05:51.000000 hipscat_import-0.3.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5516 2024-05-31 20:05:56.823187 hipscat_import-0.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2585 2024-05-31 20:05:51.000000 hipscat_import-0.3.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:05:56.783187 hipscat_import-0.3.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-05-31 20:05:51.000000 hipscat_import-0.3.3/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:05:56.783187 hipscat_import-0.3.3/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-31 20:05:51.000000 hipscat_import-0.3.3/docs/_static/custom.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:05:56.783187 hipscat_import-0.3.3/docs/catalogs/
+-rw-r--r--   0 runner    (1001) docker     (127)    13638 2024-05-31 20:05:51.000000 hipscat_import-0.3.3/docs/catalogs/arguments.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:05:56.783187 hipscat_import-0.3.3/docs/catalogs/public/
+-rw-r--r--   0 runner    (1001) docker     (127)     2252 2024-05-31 20:05:51.000000 hipscat_import-0.3.3/docs/catalogs/public/allwise.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-05-31 20:05:51.000000 hipscat_import-0.3.3/docs/catalogs/public/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2545 2024-05-31 20:05:51.000000 hipscat_import-0.3.3/docs/catalogs/public/neowise.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3050 2024-05-31 20:05:51.000000 hipscat_import-0.3.3/docs/catalogs/public/panstarrs.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2794 2024-05-31 20:05:51.000000 hipscat_import-0.3.3/docs/catalogs/public/sdss.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1948 2024-05-31 20:05:51.000000 hipscat_import-0.3.3/docs/catalogs/public/tic.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3544 2024-05-31 20:05:51.000000 hipscat_import-0.3.3/docs/catalogs/public/zubercal.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    10736 2024-05-31 20:05:51.000000 hipscat_import-0.3.3/docs/catalogs/temp_files.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2768 2024-05-31 20:05:51.000000 hipscat_import-0.3.3/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:05:56.783187 hipscat_import-0.3.3/docs/guide/
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-05-31 20:05:51.000000 hipscat_import-0.3.3/docs/guide/contact.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4668 2024-05-31 20:05:51.000000 hipscat_import-0.3.3/docs/guide/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-05-31 20:05:51.000000 hipscat_import-0.3.3/docs/guide/dask_on_ray.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    12082 2024-05-31 20:05:51.000000 hipscat_import-0.3.3/docs/guide/index_table.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6496 2024-05-31 20:05:51.000000 hipscat_import-0.3.3/docs/guide/margin_cache.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2966 2024-05-31 20:05:51.000000 hipscat_import-0.3.3/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:05:56.783187 hipscat_import-0.3.3/docs/notebooks/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7717 2024-05-31 20:05:51.000000 hipscat_import-0.3.3/docs/notebooks/estimate_pixel_threshold.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    10364 2024-05-31 20:05:51.000000 hipscat_import-0.3.3/docs/notebooks/unequal_schema.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-05-31 20:05:51.000000 hipscat_import-0.3.3/docs/notebooks.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-31 20:05:51.000000 hipscat_import-0.3.3/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:05:56.787187 hipscat_import-0.3.3/docs/static/
+-rw-r--r--   0 runner    (1001) docker     (127)   136863 2024-05-31 20:05:51.000000 hipscat_import-0.3.3/docs/static/allwise_schema.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)     4576 2024-05-31 20:05:51.000000 hipscat_import-0.3.3/docs/static/allwise_types.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    66486 2024-05-31 20:05:51.000000 hipscat_import-0.3.3/docs/static/neowise_schema.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)     2224 2024-05-31 20:05:51.000000 hipscat_import-0.3.3/docs/static/neowise_types.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      971 2024-05-31 20:05:51.000000 hipscat_import-0.3.3/docs/static/ps1_detections_types.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     2503 2024-05-31 20:05:51.000000 hipscat_import-0.3.3/docs/static/ps1_otmo_types.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   412559 2024-05-31 20:05:51.000000 hipscat_import-0.3.3/docs/static/sdss_wget.bash
+-rw-r--r--   0 runner    (1001) docker     (127)    57050 2024-05-31 20:05:51.000000 hipscat_import-0.3.3/docs/static/tic_schema.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)     1781 2024-05-31 20:05:51.000000 hipscat_import-0.3.3/docs/static/tic_types.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     2263 2024-05-31 20:05:51.000000 hipscat_import-0.3.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 20:05:56.823187 hipscat_import-0.3.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:05:56.787187 hipscat_import-0.3.3/src/
+-rw-r--r--   0 runner    (1001) docker     (127)    20810 2024-05-31 20:05:51.000000 hipscat_import-0.3.3/src/.pylintrc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:05:56.787187 hipscat_import-0.3.3/src/hipscat_import/
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-31 20:05:51.000000 hipscat_import-0.3.3/src/hipscat_import/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-31 20:05:56.000000 hipscat_import-0.3.3/src/hipscat_import/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:05:56.791187 hipscat_import-0.3.3/src/hipscat_import/catalog/
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-31 20:05:51.000000 hipscat_import-0.3.3/src/hipscat_import/catalog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9073 2024-05-31 20:05:51.000000 hipscat_import-0.3.3/src/hipscat_import/catalog/arguments.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11466 2024-05-31 20:05:51.000000 hipscat_import-0.3.3/src/hipscat_import/catalog/file_readers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13622 2024-05-31 20:05:51.000000 hipscat_import-0.3.3/src/hipscat_import/catalog/map_reduce.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10677 2024-05-31 20:05:51.000000 hipscat_import-0.3.3/src/hipscat_import/catalog/resume_plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7204 2024-05-31 20:05:51.000000 hipscat_import-0.3.3/src/hipscat_import/catalog/run_import.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3281 2024-05-31 20:05:51.000000 hipscat_import-0.3.3/src/hipscat_import/catalog/sparse_histogram.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:05:56.791187 hipscat_import-0.3.3/src/hipscat_import/index/
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-31 20:05:51.000000 hipscat_import-0.3.3/src/hipscat_import/index/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3678 2024-05-31 20:05:51.000000 hipscat_import-0.3.3/src/hipscat_import/index/arguments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2837 2024-05-31 20:05:51.000000 hipscat_import-0.3.3/src/hipscat_import/index/map_reduce.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1788 2024-05-31 20:05:51.000000 hipscat_import-0.3.3/src/hipscat_import/index/run_index.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:05:56.791187 hipscat_import-0.3.3/src/hipscat_import/margin_cache/
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-31 20:05:51.000000 hipscat_import-0.3.3/src/hipscat_import/margin_cache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4326 2024-05-31 20:05:51.000000 hipscat_import-0.3.3/src/hipscat_import/margin_cache/margin_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4472 2024-05-31 20:05:51.000000 hipscat_import-0.3.3/src/hipscat_import/margin_cache/margin_cache_arguments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6453 2024-05-31 20:05:51.000000 hipscat_import-0.3.3/src/hipscat_import/margin_cache/margin_cache_map_reduce.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6838 2024-05-31 20:05:51.000000 hipscat_import-0.3.3/src/hipscat_import/margin_cache/margin_cache_resume_plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3266 2024-05-31 20:05:51.000000 hipscat_import-0.3.3/src/hipscat_import/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9055 2024-05-31 20:05:51.000000 hipscat_import-0.3.3/src/hipscat_import/pipeline_resume_plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 20:05:51.000000 hipscat_import-0.3.3/src/hipscat_import/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     6649 2024-05-31 20:05:51.000000 hipscat_import-0.3.3/src/hipscat_import/runtime_arguments.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:05:56.791187 hipscat_import-0.3.3/src/hipscat_import/soap/
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-31 20:05:51.000000 hipscat_import-0.3.3/src/hipscat_import/soap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4008 2024-05-31 20:05:51.000000 hipscat_import-0.3.3/src/hipscat_import/soap/arguments.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10861 2024-05-31 20:05:51.000000 hipscat_import-0.3.3/src/hipscat_import/soap/map_reduce.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9577 2024-05-31 20:05:51.000000 hipscat_import-0.3.3/src/hipscat_import/soap/resume_plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3792 2024-05-31 20:05:51.000000 hipscat_import-0.3.3/src/hipscat_import/soap/run_soap.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:05:56.791187 hipscat_import-0.3.3/src/hipscat_import/verification/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 20:05:51.000000 hipscat_import-0.3.3/src/hipscat_import/verification/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1863 2024-05-31 20:05:51.000000 hipscat_import-0.3.3/src/hipscat_import/verification/arguments.py
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-05-31 20:05:51.000000 hipscat_import-0.3.3/src/hipscat_import/verification/run_verification.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:05:56.819187 hipscat_import-0.3.3/src/hipscat_import.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5516 2024-05-31 20:05:56.000000 hipscat_import-0.3.3/src/hipscat_import.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12064 2024-05-31 20:05:56.000000 hipscat_import-0.3.3/src/hipscat_import.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 20:05:56.000000 hipscat_import-0.3.3/src/hipscat_import.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-05-31 20:05:56.000000 hipscat_import-0.3.3/src/hipscat_import.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-31 20:05:56.000000 hipscat_import-0.3.3/src/hipscat_import.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:05:56.791187 hipscat_import-0.3.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    20888 2024-05-31 20:05:51.000000 hipscat_import-0.3.3/tests/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (127)     1316 2024-05-31 20:05:51.000000 hipscat_import-0.3.3/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:05:56.791187 hipscat_import-0.3.3/tests/hipscat_import/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:05:56.795187 hipscat_import-0.3.3/tests/hipscat_import/catalog/
+-rw-r--r--   0 runner    (1001) docker     (127)     7287 2024-05-31 20:05:51.000000 hipscat_import-0.3.3/tests/hipscat_import/catalog/test_argument_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10293 2024-05-31 20:05:51.000000 hipscat_import-0.3.3/tests/hipscat_import/catalog/test_file_readers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18007 2024-05-31 20:05:51.000000 hipscat_import-0.3.3/tests/hipscat_import/catalog/test_map_reduce.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8076 2024-05-31 20:05:51.000000 hipscat_import-0.3.3/tests/hipscat_import/catalog/test_resume_plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12967 2024-05-31 20:05:51.000000 hipscat_import-0.3.3/tests/hipscat_import/catalog/test_run_import.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25081 2024-05-31 20:05:51.000000 hipscat_import-0.3.3/tests/hipscat_import/catalog/test_run_round_trip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2391 2024-05-31 20:05:51.000000 hipscat_import-0.3.3/tests/hipscat_import/catalog/test_sparse_histogram.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9441 2024-05-31 20:05:51.000000 hipscat_import-0.3.3/tests/hipscat_import/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:05:56.775187 hipscat_import-0.3.3/tests/hipscat_import/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:05:56.795187 hipscat_import-0.3.3/tests/hipscat_import/data/blank/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 20:05:51.000000 hipscat_import-0.3.3/tests/hipscat_import/data/blank/blank.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:05:56.795187 hipscat_import-0.3.3/tests/hipscat_import/data/mixed_schema/
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-31 20:05:51.000000 hipscat_import-0.3.3/tests/hipscat_import/data/mixed_schema/input_01.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-05-31 20:05:51.000000 hipscat_import-0.3.3/tests/hipscat_import/data/mixed_schema/input_02.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     4513 2024-05-31 20:05:51.000000 hipscat_import-0.3.3/tests/hipscat_import/data/mixed_schema/schema.parquet
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:05:56.775187 hipscat_import-0.3.3/tests/hipscat_import/data/parquet_shards/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:05:56.771187 hipscat_import-0.3.3/tests/hipscat_import/data/parquet_shards/order_0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:05:56.771187 hipscat_import-0.3.3/tests/hipscat_import/data/parquet_shards/order_0/dir_0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:05:56.795187 hipscat_import-0.3.3/tests/hipscat_import/data/parquet_shards/order_0/dir_0/pixel_11/
+-rw-r--r--   0 runner    (1001) docker     (127)     4084 2024-05-31 20:05:51.000000 hipscat_import-0.3.3/tests/hipscat_import/data/parquet_shards/order_0/dir_0/pixel_11/shard_0_0.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)     4104 2024-05-31 20:05:51.000000 hipscat_import-0.3.3/tests/hipscat_import/data/parquet_shards/order_0/dir_0/pixel_11/shard_1_0.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)     4090 2024-05-31 20:05:51.000000 hipscat_import-0.3.3/tests/hipscat_import/data/parquet_shards/order_0/dir_0/pixel_11/shard_2_0.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)     4110 2024-05-31 20:05:51.000000 hipscat_import-0.3.3/tests/hipscat_import/data/parquet_shards/order_0/dir_0/pixel_11/shard_3_0.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)     4123 2024-05-31 20:05:51.000000 hipscat_import-0.3.3/tests/hipscat_import/data/parquet_shards/order_0/dir_0/pixel_11/shard_4_0.parquet
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:05:56.775187 hipscat_import-0.3.3/tests/hipscat_import/data/parquet_shards/order_1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:05:56.775187 hipscat_import-0.3.3/tests/hipscat_import/data/parquet_shards/order_1/dir_0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:05:56.795187 hipscat_import-0.3.3/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_44/
+-rw-r--r--   0 runner    (1001) docker     (127)     3809 2024-05-31 20:05:51.000000 hipscat_import-0.3.3/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_44/shard_0_0.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)     3903 2024-05-31 20:05:51.000000 hipscat_import-0.3.3/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_44/shard_1_0.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)     3852 2024-05-31 20:05:51.000000 hipscat_import-0.3.3/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_44/shard_2_0.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)     3842 2024-05-31 20:05:51.000000 hipscat_import-0.3.3/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_44/shard_3_0.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)     3905 2024-05-31 20:05:51.000000 hipscat_import-0.3.3/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_44/shard_4_0.parquet
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:05:56.799187 hipscat_import-0.3.3/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_45/
+-rw-r--r--   0 runner    (1001) docker     (127)     3836 2024-05-31 20:05:51.000000 hipscat_import-0.3.3/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_45/shard_0_0.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)     3836 2024-05-31 20:05:51.000000 hipscat_import-0.3.3/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_45/shard_1_0.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)     3804 2024-05-31 20:05:51.000000 hipscat_import-0.3.3/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_45/shard_2_0.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)     3803 2024-05-31 20:05:51.000000 hipscat_import-0.3.3/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_45/shard_3_0.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)     3841 2024-05-31 20:05:51.000000 hipscat_import-0.3.3/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_45/shard_4_0.parquet
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:05:56.799187 hipscat_import-0.3.3/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_46/
+-rw-r--r--   0 runner    (1001) docker     (127)     3898 2024-05-31 20:05:51.000000 hipscat_import-0.3.3/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_46/shard_0_0.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)     3833 2024-05-31 20:05:51.000000 hipscat_import-0.3.3/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_46/shard_1_0.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)     3899 2024-05-31 20:05:51.000000 hipscat_import-0.3.3/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_46/shard_2_0.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)     3891 2024-05-31 20:05:51.000000 hipscat_import-0.3.3/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_46/shard_3_0.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)     3803 2024-05-31 20:05:51.000000 hipscat_import-0.3.3/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_46/shard_4_0.parquet
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:05:56.799187 hipscat_import-0.3.3/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_47/
+-rw-r--r--   0 runner    (1001) docker     (127)     3769 2024-05-31 20:05:51.000000 hipscat_import-0.3.3/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_47/shard_0_0.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)     3769 2024-05-31 20:05:51.000000 hipscat_import-0.3.3/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_47/shard_1_0.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)     3790 2024-05-31 20:05:51.000000 hipscat_import-0.3.3/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_47/shard_2_0.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)     3808 2024-05-31 20:05:51.000000 hipscat_import-0.3.3/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_47/shard_3_0.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)     3822 2024-05-31 20:05:51.000000 hipscat_import-0.3.3/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_47/shard_4_0.parquet
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:05:56.775187 hipscat_import-0.3.3/tests/hipscat_import/data/resume/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:05:56.775187 hipscat_import-0.3.3/tests/hipscat_import/data/resume/Norder=0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:05:56.799187 hipscat_import-0.3.3/tests/hipscat_import/data/resume/Norder=0/Dir=0/
+-rw-r--r--   0 runner    (1001) docker     (127)     8915 2024-05-31 20:05:51.000000 hipscat_import-0.3.3/tests/hipscat_import/data/resume/Norder=0/Dir=0/Npix=11.parquet
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:05:56.775187 hipscat_import-0.3.3/tests/hipscat_import/data/resume/Norder=1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:05:56.799187 hipscat_import-0.3.3/tests/hipscat_import/data/resume/Norder=1/Dir=0/
+-rw-r--r--   0 runner    (1001) docker     (127)     7210 2024-05-31 20:05:51.000000 hipscat_import-0.3.3/tests/hipscat_import/data/resume/Norder=1/Dir=0/Npix=44.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)     6973 2024-05-31 20:05:51.000000 hipscat_import-0.3.3/tests/hipscat_import/data/resume/Norder=1/Dir=0/Npix=45.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)     7216 2024-05-31 20:05:51.000000 hipscat_import-0.3.3/tests/hipscat_import/data/resume/Norder=1/Dir=0/Npix=46.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)     6741 2024-05-31 20:05:51.000000 hipscat_import-0.3.3/tests/hipscat_import/data/resume/Norder=1/Dir=0/Npix=47.parquet
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:05:56.799187 hipscat_import-0.3.3/tests/hipscat_import/data/resume/intermediate/
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-31 20:05:51.000000 hipscat_import-0.3.3/tests/hipscat_import/data/resume/intermediate/mapping_histogram.binary
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:05:56.799187 hipscat_import-0.3.3/tests/hipscat_import/data/small_sky/
+-rw-r--r--   0 runner    (1001) docker     (127)     2648 2024-05-31 20:05:51.000000 hipscat_import-0.3.3/tests/hipscat_import/data/small_sky/catalog.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:05:56.803187 hipscat_import-0.3.3/tests/hipscat_import/data/small_sky_object_catalog/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:05:56.775187 hipscat_import-0.3.3/tests/hipscat_import/data/small_sky_object_catalog/Norder=0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:05:56.803187 hipscat_import-0.3.3/tests/hipscat_import/data/small_sky_object_catalog/Norder=0/Dir=0/
+-rw-r--r--   0 runner    (1001) docker     (127)     8880 2024-05-31 20:05:51.000000 hipscat_import-0.3.3/tests/hipscat_import/data/small_sky_object_catalog/Norder=0/Dir=0/Npix=11.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)     4018 2024-05-31 20:05:51.000000 hipscat_import-0.3.3/tests/hipscat_import/data/small_sky_object_catalog/_common_metadata
+-rw-r--r--   0 runner    (1001) docker     (127)     5130 2024-05-31 20:05:51.000000 hipscat_import-0.3.3/tests/hipscat_import/data/small_sky_object_catalog/_metadata
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-05-31 20:05:51.000000 hipscat_import-0.3.3/tests/hipscat_import/data/small_sky_object_catalog/catalog_info.json
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-31 20:05:51.000000 hipscat_import-0.3.3/tests/hipscat_import/data/small_sky_object_catalog/partition_info.csv
+-rw-r--r--   0 runner    (1001) docker     (127)  1581120 2024-05-31 20:05:51.000000 hipscat_import-0.3.3/tests/hipscat_import/data/small_sky_object_catalog/point_map.fits
+-rw-r--r--   0 runner    (1001) docker     (127)     1979 2024-05-31 20:05:51.000000 hipscat_import-0.3.3/tests/hipscat_import/data/small_sky_object_catalog/provenance_info.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:05:56.803187 hipscat_import-0.3.3/tests/hipscat_import/data/small_sky_parts/
+-rw-r--r--   0 runner    (1001) docker     (127)      528 2024-05-31 20:05:51.000000 hipscat_import-0.3.3/tests/hipscat_import/data/small_sky_parts/catalog_00_of_05.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      549 2024-05-31 20:05:51.000000 hipscat_import-0.3.3/tests/hipscat_import/data/small_sky_parts/catalog_01_of_05.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      549 2024-05-31 20:05:51.000000 hipscat_import-0.3.3/tests/hipscat_import/data/small_sky_parts/catalog_02_of_05.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      549 2024-05-31 20:05:51.000000 hipscat_import-0.3.3/tests/hipscat_import/data/small_sky_parts/catalog_03_of_05.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      589 2024-05-31 20:05:51.000000 hipscat_import-0.3.3/tests/hipscat_import/data/small_sky_parts/catalog_04_of_05.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-31 20:05:51.000000 hipscat_import-0.3.3/tests/hipscat_import/data/small_sky_parts/catalog_10_of_05.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:05:56.803187 hipscat_import-0.3.3/tests/hipscat_import/data/small_sky_source/
+-rw-r--r--   0 runner    (1001) docker     (127)  1688789 2024-05-31 20:05:51.000000 hipscat_import-0.3.3/tests/hipscat_import/data/small_sky_source/small_sky_source.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:05:56.807187 hipscat_import-0.3.3/tests/hipscat_import/data/small_sky_source_catalog/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:05:56.775187 hipscat_import-0.3.3/tests/hipscat_import/data/small_sky_source_catalog/Norder=0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:05:56.807187 hipscat_import-0.3.3/tests/hipscat_import/data/small_sky_source_catalog/Norder=0/Dir=0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11421 2024-05-31 20:05:51.000000 hipscat_import-0.3.3/tests/hipscat_import/data/small_sky_source_catalog/Norder=0/Dir=0/Npix=4.parquet
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:05:56.775187 hipscat_import-0.3.3/tests/hipscat_import/data/small_sky_source_catalog/Norder=1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:05:56.807187 hipscat_import-0.3.3/tests/hipscat_import/data/small_sky_source_catalog/Norder=1/Dir=0/
+-rw-r--r--   0 runner    (1001) docker     (127)   133671 2024-05-31 20:05:51.000000 hipscat_import-0.3.3/tests/hipscat_import/data/small_sky_source_catalog/Norder=1/Dir=0/Npix=47.parquet
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:05:56.775187 hipscat_import-0.3.3/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:05:56.811187 hipscat_import-0.3.3/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/
+-rw-r--r--   0 runner    (1001) docker     (127)    28346 2024-05-31 20:05:51.000000 hipscat_import-0.3.3/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=176.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    86262 2024-05-31 20:05:51.000000 hipscat_import-0.3.3/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=177.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    92634 2024-05-31 20:05:51.000000 hipscat_import-0.3.3/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=178.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    99874 2024-05-31 20:05:51.000000 hipscat_import-0.3.3/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=179.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    42177 2024-05-31 20:05:51.000000 hipscat_import-0.3.3/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=180.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    54742 2024-05-31 20:05:51.000000 hipscat_import-0.3.3/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=181.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    72960 2024-05-31 20:05:51.000000 hipscat_import-0.3.3/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=182.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    67771 2024-05-31 20:05:51.000000 hipscat_import-0.3.3/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=183.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    80265 2024-05-31 20:05:51.000000 hipscat_import-0.3.3/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=184.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)   162064 2024-05-31 20:05:51.000000 hipscat_import-0.3.3/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=185.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    31761 2024-05-31 20:05:51.000000 hipscat_import-0.3.3/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=186.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    43705 2024-05-31 20:05:51.000000 hipscat_import-0.3.3/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=187.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)     5525 2024-05-31 20:05:51.000000 hipscat_import-0.3.3/tests/hipscat_import/data/small_sky_source_catalog/_common_metadata
+-rw-r--r--   0 runner    (1001) docker     (127)    28968 2024-05-31 20:05:51.000000 hipscat_import-0.3.3/tests/hipscat_import/data/small_sky_source_catalog/_metadata
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-31 20:05:51.000000 hipscat_import-0.3.3/tests/hipscat_import/data/small_sky_source_catalog/catalog_info.json
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-31 20:05:51.000000 hipscat_import-0.3.3/tests/hipscat_import/data/small_sky_source_catalog/partition_info.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     8640 2024-05-31 20:05:51.000000 hipscat_import-0.3.3/tests/hipscat_import/data/small_sky_source_catalog/point_map.fits
+-rw-r--r--   0 runner    (1001) docker     (127)     2146 2024-05-31 20:05:51.000000 hipscat_import-0.3.3/tests/hipscat_import/data/small_sky_source_catalog/provenance_info.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:05:56.811187 hipscat_import-0.3.3/tests/hipscat_import/data/soap_intermediate/
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-31 20:05:51.000000 hipscat_import-0.3.3/tests/hipscat_import/data/soap_intermediate/0_4.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-31 20:05:51.000000 hipscat_import-0.3.3/tests/hipscat_import/data/soap_intermediate/1_47.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-31 20:05:51.000000 hipscat_import-0.3.3/tests/hipscat_import/data/soap_intermediate/2_176.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-31 20:05:51.000000 hipscat_import-0.3.3/tests/hipscat_import/data/soap_intermediate/2_177.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-31 20:05:51.000000 hipscat_import-0.3.3/tests/hipscat_import/data/soap_intermediate/2_178.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-31 20:05:51.000000 hipscat_import-0.3.3/tests/hipscat_import/data/soap_intermediate/2_179.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-31 20:05:51.000000 hipscat_import-0.3.3/tests/hipscat_import/data/soap_intermediate/2_180.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-31 20:05:51.000000 hipscat_import-0.3.3/tests/hipscat_import/data/soap_intermediate/2_181.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-31 20:05:51.000000 hipscat_import-0.3.3/tests/hipscat_import/data/soap_intermediate/2_182.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-31 20:05:51.000000 hipscat_import-0.3.3/tests/hipscat_import/data/soap_intermediate/2_183.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-31 20:05:51.000000 hipscat_import-0.3.3/tests/hipscat_import/data/soap_intermediate/2_184.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-31 20:05:51.000000 hipscat_import-0.3.3/tests/hipscat_import/data/soap_intermediate/2_185.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-31 20:05:51.000000 hipscat_import-0.3.3/tests/hipscat_import/data/soap_intermediate/2_186.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-31 20:05:51.000000 hipscat_import-0.3.3/tests/hipscat_import/data/soap_intermediate/2_187.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:05:56.775187 hipscat_import-0.3.3/tests/hipscat_import/data/soap_intermediate/order_0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:05:56.775187 hipscat_import-0.3.3/tests/hipscat_import/data/soap_intermediate/order_0/dir_0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:05:56.815187 hipscat_import-0.3.3/tests/hipscat_import/data/soap_intermediate/order_0/dir_0/pixel_11/
+-rw-r--r--   0 runner    (1001) docker     (127)     6838 2024-05-31 20:05:51.000000 hipscat_import-0.3.3/tests/hipscat_import/data/soap_intermediate/order_0/dir_0/pixel_11/source_0_4.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    33062 2024-05-31 20:05:51.000000 hipscat_import-0.3.3/tests/hipscat_import/data/soap_intermediate/order_0/dir_0/pixel_11/source_1_47.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    10443 2024-05-31 20:05:51.000000 hipscat_import-0.3.3/tests/hipscat_import/data/soap_intermediate/order_0/dir_0/pixel_11/source_2_176.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    22870 2024-05-31 20:05:51.000000 hipscat_import-0.3.3/tests/hipscat_import/data/soap_intermediate/order_0/dir_0/pixel_11/source_2_177.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    24239 2024-05-31 20:05:51.000000 hipscat_import-0.3.3/tests/hipscat_import/data/soap_intermediate/order_0/dir_0/pixel_11/source_2_178.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    25729 2024-05-31 20:05:51.000000 hipscat_import-0.3.3/tests/hipscat_import/data/soap_intermediate/order_0/dir_0/pixel_11/source_2_179.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    13370 2024-05-31 20:05:51.000000 hipscat_import-0.3.3/tests/hipscat_import/data/soap_intermediate/order_0/dir_0/pixel_11/source_2_180.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    16010 2024-05-31 20:05:51.000000 hipscat_import-0.3.3/tests/hipscat_import/data/soap_intermediate/order_0/dir_0/pixel_11/source_2_181.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    19958 2024-05-31 20:05:51.000000 hipscat_import-0.3.3/tests/hipscat_import/data/soap_intermediate/order_0/dir_0/pixel_11/source_2_182.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    18844 2024-05-31 20:05:51.000000 hipscat_import-0.3.3/tests/hipscat_import/data/soap_intermediate/order_0/dir_0/pixel_11/source_2_183.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    21542 2024-05-31 20:05:51.000000 hipscat_import-0.3.3/tests/hipscat_import/data/soap_intermediate/order_0/dir_0/pixel_11/source_2_184.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    39137 2024-05-31 20:05:51.000000 hipscat_import-0.3.3/tests/hipscat_import/data/soap_intermediate/order_0/dir_0/pixel_11/source_2_185.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    11136 2024-05-31 20:05:51.000000 hipscat_import-0.3.3/tests/hipscat_import/data/soap_intermediate/order_0/dir_0/pixel_11/source_2_186.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    13692 2024-05-31 20:05:51.000000 hipscat_import-0.3.3/tests/hipscat_import/data/soap_intermediate/order_0/dir_0/pixel_11/source_2_187.parquet
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:05:56.819187 hipscat_import-0.3.3/tests/hipscat_import/data/test_formats/
+-rw-r--r--   0 runner    (1001) docker     (127)     2648 2024-05-31 20:05:51.000000 hipscat_import-0.3.3/tests/hipscat_import/data/test_formats/catalog.starr
+-rw-r--r--   0 runner    (1001) docker     (127)    45749 2024-05-31 20:05:51.000000 hipscat_import-0.3.3/tests/hipscat_import/data/test_formats/gaia_epoch.ecsv
+-rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-05-31 20:05:51.000000 hipscat_import-0.3.3/tests/hipscat_import/data/test_formats/gaia_minimum.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     5010 2024-05-31 20:05:51.000000 hipscat_import-0.3.3/tests/hipscat_import/data/test_formats/gaia_minimum_schema.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-05-31 20:05:51.000000 hipscat_import-0.3.3/tests/hipscat_import/data/test_formats/headers.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     5394 2024-05-31 20:05:51.000000 hipscat_import-0.3.3/tests/hipscat_import/data/test_formats/hipscat_index.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     4034 2024-05-31 20:05:51.000000 hipscat_import-0.3.3/tests/hipscat_import/data/test_formats/hipscat_index.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-05-31 20:05:51.000000 hipscat_import-0.3.3/tests/hipscat_import/data/test_formats/macauff_metadata.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     4636 2024-05-31 20:05:51.000000 hipscat_import-0.3.3/tests/hipscat_import/data/test_formats/pandasindex.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-31 20:05:51.000000 hipscat_import-0.3.3/tests/hipscat_import/data/test_formats/pipe_delimited.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    14400 2024-05-31 20:05:51.000000 hipscat_import-0.3.3/tests/hipscat_import/data/test_formats/small_sky.fits
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:05:56.819187 hipscat_import-0.3.3/tests/hipscat_import/index/
+-rw-r--r--   0 runner    (1001) docker     (127)     5293 2024-05-31 20:05:51.000000 hipscat_import-0.3.3/tests/hipscat_import/index/test_index_argument.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7110 2024-05-31 20:05:51.000000 hipscat_import-0.3.3/tests/hipscat_import/index/test_index_map_reduce.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5501 2024-05-31 20:05:51.000000 hipscat_import-0.3.3/tests/hipscat_import/index/test_run_index.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:05:56.819187 hipscat_import-0.3.3/tests/hipscat_import/margin_cache/
+-rw-r--r--   0 runner    (1001) docker     (127)     5008 2024-05-31 20:05:51.000000 hipscat_import-0.3.3/tests/hipscat_import/margin_cache/test_arguments_margin_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3081 2024-05-31 20:05:51.000000 hipscat_import-0.3.3/tests/hipscat_import/margin_cache/test_margin_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6197 2024-05-31 20:05:51.000000 hipscat_import-0.3.3/tests/hipscat_import/margin_cache/test_margin_cache_map_reduce.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4854 2024-05-31 20:05:51.000000 hipscat_import-0.3.3/tests/hipscat_import/margin_cache/test_margin_cache_resume_plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4086 2024-05-31 20:05:51.000000 hipscat_import-0.3.3/tests/hipscat_import/margin_cache/test_margin_round_trip.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:05:56.819187 hipscat_import-0.3.3/tests/hipscat_import/soap/
+-rw-r--r--   0 runner    (1001) docker     (127)     2079 2024-05-31 20:05:51.000000 hipscat_import-0.3.3/tests/hipscat_import/soap/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7832 2024-05-31 20:05:51.000000 hipscat_import-0.3.3/tests/hipscat_import/soap/test_run_soap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3242 2024-05-31 20:05:51.000000 hipscat_import-0.3.3/tests/hipscat_import/soap/test_soap_arguments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6697 2024-05-31 20:05:51.000000 hipscat_import-0.3.3/tests/hipscat_import/soap/test_soap_map_reduce.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7052 2024-05-31 20:05:51.000000 hipscat_import-0.3.3/tests/hipscat_import/soap/test_soap_resume_plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5921 2024-05-31 20:05:51.000000 hipscat_import-0.3.3/tests/hipscat_import/test_pipeline_resume_plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4217 2024-05-31 20:05:51.000000 hipscat_import-0.3.3/tests/hipscat_import/test_runtime_arguments.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:05:56.819187 hipscat_import-0.3.3/tests/hipscat_import/verification/
+-rw-r--r--   0 runner    (1001) docker     (127)      908 2024-05-31 20:05:51.000000 hipscat_import-0.3.3/tests/hipscat_import/verification/test_run_verification.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3021 2024-05-31 20:05:51.000000 hipscat_import-0.3.3/tests/hipscat_import/verification/test_verification_arguments.py
```

### Comparing `hipscat_import-0.3.2/.copier-answers.yml` & `hipscat_import-0.3.3/.copier-answers.yml`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.2/.gitattributes` & `hipscat_import-0.3.3/.gitattributes`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.2/.github/ISSUE_TEMPLATE/1-bug_report.md` & `hipscat_import-0.3.3/.github/ISSUE_TEMPLATE/1-bug_report.md`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.2/.github/ISSUE_TEMPLATE/2-feature_request.md` & `hipscat_import-0.3.3/.github/ISSUE_TEMPLATE/2-feature_request.md`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.2/.github/pull_request_template.md` & `hipscat_import-0.3.3/.github/pull_request_template.md`

 * *Files 10% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 ## Solution Description
 <!-- Please explain the technical solution that I have provided and how it addresses the issue or feature being implemented -->
 
 
 
 ## Code Quality
-- [ ] I have read the Contribution Guide
+- [ ] I have read the [Contribution Guide](https://hipscat-import.readthedocs.io/en/stable/guide/contributing.html) and [LINCC Frameworks Code of Conduct](https://lsstdiscoveryalliance.org/programs/lincc-frameworks/code-conduct/)
 - [ ] My code follows the code style of this project
 - [ ] My code builds (or compiles) cleanly without any errors or warnings
 - [ ] My code contains relevant comments and necessary documentation
 
 ## Project-Specific Pull Request Checklists
 <!--- Please only use the checklist that apply to your change type(s) -->
```

### Comparing `hipscat_import-0.3.2/.github/workflows/build-documentation.yml` & `hipscat_import-0.3.3/.github/workflows/build-documentation.yml`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.2/.github/workflows/pre-commit-ci.yml` & `hipscat_import-0.3.3/.github/workflows/pre-commit-ci.yml`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.2/.github/workflows/publish-to-pypi.yml` & `hipscat_import-0.3.3/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.2/.github/workflows/smoke-test.yml` & `hipscat_import-0.3.3/.github/workflows/smoke-test.yml`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.2/.github/workflows/testing-and-coverage.yml` & `hipscat_import-0.3.3/.github/workflows/testing-and-coverage.yml`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.2/.gitignore` & `hipscat_import-0.3.3/.gitignore`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.2/.pre-commit-config.yaml` & `hipscat_import-0.3.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.2/.setup_dev.sh` & `hipscat_import-0.3.3/.setup_dev.sh`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.2/LICENSE` & `hipscat_import-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.2/PKG-INFO` & `hipscat_import-0.3.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hipscat-import
-Version: 0.3.2
+Version: 0.3.3
 Author-email: LINCC Frameworks <lincc-frameworks-team@lists.lsst.org>
 License: BSD 3-Clause License
         
         Copyright (c) 2023, LINCC Frameworks
         
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met:
@@ -38,21 +38,22 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: dask[complete]>=2024.3.0
 Requires-Dist: deprecated
 Requires-Dist: healpy
-Requires-Dist: hipscat>=0.3.0
+Requires-Dist: hipscat>=0.3.4
 Requires-Dist: ipykernel
+Requires-Dist: numpy
 Requires-Dist: pandas
 Requires-Dist: pyarrow
 Requires-Dist: pyyaml
+Requires-Dist: scipy
 Requires-Dist: tqdm
-Requires-Dist: numpy
 Provides-Extra: dev
 Requires-Dist: black; extra == "dev"
 Requires-Dist: jupyter; extra == "dev"
 Requires-Dist: mypy; extra == "dev"
 Requires-Dist: pre-commit; extra == "dev"
 Requires-Dist: pylint; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
```

### Comparing `hipscat_import-0.3.2/README.md` & `hipscat_import-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.2/docs/Makefile` & `hipscat_import-0.3.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.2/docs/catalogs/arguments.rst` & `hipscat_import-0.3.3/docs/catalogs/arguments.rst`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 At a minimum, you need arguments that include where to find the input files,
 the column names for RA, and DEC, and where to put the output files. 
 A minimal arguments block will look something like:
 
 .. code-block:: python
 
-    from hipscat_import.pipeline import ImportArguments
+    from hipscat_import.pipeline.catalog.arguments import ImportArguments
 
     args = ImportArguments(
         sort_columns="ObjectID",
         ra_column="ObjectRA",
         dec_column="ObjectDec",
         input_path="./my_data",
         file_reader="csv",
```

### Comparing `hipscat_import-0.3.2/docs/catalogs/public/allwise.rst` & `hipscat_import-0.3.3/docs/catalogs/public/allwise.rst`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.2/docs/catalogs/public/index.rst` & `hipscat_import-0.3.3/docs/catalogs/public/index.rst`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.2/docs/catalogs/public/neowise.rst` & `hipscat_import-0.3.3/docs/catalogs/public/neowise.rst`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.2/docs/catalogs/public/panstarrs.rst` & `hipscat_import-0.3.3/docs/catalogs/public/panstarrs.rst`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.2/docs/catalogs/public/sdss.rst` & `hipscat_import-0.3.3/docs/catalogs/public/sdss.rst`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.2/docs/catalogs/public/tic.rst` & `hipscat_import-0.3.3/docs/catalogs/public/tic.rst`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.2/docs/catalogs/public/zubercal.rst` & `hipscat_import-0.3.3/docs/catalogs/public/zubercal.rst`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.2/docs/catalogs/temp_files.rst` & `hipscat_import-0.3.3/docs/catalogs/temp_files.rst`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.2/docs/conf.py` & `hipscat_import-0.3.3/docs/conf.py`

 * *Files 23% similar despite different names*

```diff
@@ -34,15 +34,17 @@
 
 html_static_path = ["_static"]
 html_css_files = ["custom.css"]
 
 extensions = [
     "sphinx.ext.mathjax",
     "sphinx.ext.napoleon",
-    "sphinx.ext.viewcode",
+    # viewcode and autoapi interaction creates some failures. See:
+    # https://github.com/readthedocs/sphinx-autoapi/issues/422
+    # "sphinx.ext.viewcode",
     "sphinx.ext.intersphinx",
     "sphinx_copybutton",
     "autoapi.extension",
     "nbsphinx",
 ]
 
 # -- autoapi configuration ----------------------------------------
@@ -53,14 +55,24 @@
 
 autoapi_type = "python"
 autoapi_dirs = ["../src"]
 autoapi_ignore = ["*/__main__.py", "*/_version.py"]
 autoapi_add_toc_tree_entry = False
 autoapi_member_order = "bysource"
 
+autoapi_options = [
+    "members",
+    "undoc-members",
+    "show-inheritance",
+    "show-module-summary",
+    "special-members",
+    "imported-members",
+    "inherited-members",
+]
+
 napoleon_google_docstring = True
 
 # -- sphinx-copybutton configuration ----------------------------------------
 ## sets up the expected prompt text from console blocks, and excludes it from
 ## the text that goes into the clipboard.
 copybutton_exclude = ".linenos, .gp"
 copybutton_prompt_text = ">> "
```

### Comparing `hipscat_import-0.3.2/docs/guide/contact.rst` & `hipscat_import-0.3.3/docs/guide/contact.rst`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.2/docs/guide/contributing.rst` & `hipscat_import-0.3.3/docs/guide/contributing.rst`

 * *Files 16% similar despite different names*

```diff
@@ -36,58 +36,33 @@
 .. code-block:: console
 
    >> conda create env -n <env_name> python=3.10
    >> conda activate <env_name>
 
 
 Once you have created a new environment, you can install this project for local
-development using the following commands:
+development using the following command:
 
 .. code-block:: console
 
-   >> pip install -e .'[dev]'
-   >> pre-commit install
-   >> conda install pandoc
+   >> source .setup_dev.sh
 
 
 Notes:
 
 1) The single quotes around ``'[dev]'`` may not be required for your operating system.
 2) ``pre-commit install`` will initialize pre-commit for this local repository, so
    that a set of tests will be run prior to completing a local commit. For more
    information, see the Python Project Template documentation on
    `pre-commit <https://lincc-ppt.readthedocs.io/en/stable/practices/precommit.html>`_.
 3) Installing ``pandoc`` allows you to verify that automatic rendering of Jupyter notebooks
    into documentation for ReadTheDocs works as expected. For more information, see
    the Python Project Template documentation on
    `Sphinx and Python Notebooks <https://lincc-ppt.readthedocs.io/en/stable/practices/sphinx.html#python-notebooks>`_.
 
-
-.. tip::
-    Installing on Mac
-
-    ``healpy`` is a very necessary dependency for hipscat libraries at this time, but
-    native prebuilt binaries for healpy on Apple Silicon Macs 
-    `do not yet exist <https://healpy.readthedocs.io/en/latest/install.html#binary-installation-with-pip-recommended-for-most-other-python-users>`_, 
-    so it's recommended to install via conda before proceeding to hipscat-import.
-
-    .. code-block:: console
-
-        >> conda config --add channels conda-forge
-        >> conda install healpy
-        >> git clone https://github.com/astronomy-commons/hipscat-import
-        >> cd hipscat-import
-        >> pip install -e .
-        
-    When installing dev dependencies, make sure to include the single quotes.
-
-    .. code-block:: console
-        
-        >> pip install -e '.[dev]'
-
 Testing
 -------------------------------------------------------------------------------
 
 We use ``pytest`` as our preferred unit test runner engine, in keeping with
 LSST DM style guide. We make heavy use of 
 `pytest fixtures <https://docs.pytest.org/en/7.1.x/explanation/fixtures.html#about-fixtures>`_, 
 which set up various resources used for unit testing, or provide consistent 
@@ -127,7 +102,13 @@
 
 Optional - Release a new version
 -------------------------------------------------------------------------------
 
 Once your PR is merged you can create a new release to make your changes available. 
 GitHub's `instructions <https://docs.github.com/en/repositories/releasing-projects-on-github/managing-releases-in-a-repository>`_ for doing so are here. 
 Use your best judgement when incrementing the version. i.e. is this a major, minor, or patch fix.
+
+Be kind
+-------------------------------------------------------------------------------
+
+You are expected to comply with the 
+`LINCC Frameworks Code of Conduct <https://lsstdiscoveryalliance.org/programs/lincc-frameworks/code-conduct/>`_`.
```

### Comparing `hipscat_import-0.3.2/docs/guide/dask_on_ray.rst` & `hipscat_import-0.3.3/docs/guide/dask_on_ray.rst`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.2/docs/guide/index_table.rst` & `hipscat_import-0.3.3/docs/guide/index_table.rst`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.2/docs/guide/margin_cache.rst` & `hipscat_import-0.3.3/docs/guide/margin_cache.rst`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.2/docs/index.rst` & `hipscat_import-0.3.3/docs/index.rst`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.2/docs/notebooks/estimate_pixel_threshold.ipynb` & `hipscat_import-0.3.3/docs/notebooks/estimate_pixel_threshold.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9345951140873017%*

 * *Differences: {"'cells'": "{1: {'source': {insert: [(3, '- parquet uses compression in various ways, and by "*

 * *            'creating the sample, we can get a sense of both the overall and field-level '*

 * *            "compression with real data\\n')], delete: [3]}}, 5: {'source': {insert: [(7, '## "*

 * *            "300MB\\n'), (8, 'ideal_file_small = 300 * 1024 * 1024\\n'), (9, '## 1G\\n'), (10, "*

 * *            "'ideal_file_large = 1024 * 1024 * 1024\\n')], delete: [10, 9, 8, 7]}}}",*

 * * "'metadata'": "{'language_info': {'version':  […]*

```diff
@@ -28,15 +28,15 @@
             "cell_type": "markdown",
             "id": "eb86458c",
             "metadata": {},
             "source": [
                 "## Create a sample parquet file\n",
                 "\n",
                 "The first step is to read in your survey data in its original form, and convert a sample into parquet. This has a few benefits:\n",
-                "- parquet uses compression in various ways, and by creating the sample, we can get a sense of both the overall and field-level compression with real dat\n",
+                "- parquet uses compression in various ways, and by creating the sample, we can get a sense of both the overall and field-level compression with real data\n",
                 "- using the importer `FileReader` interface now sets you up for more success when you get around to importing!\n",
                 "\n",
                 "If your data is already in parquet format, just change the `sample_parquet_file` path to an existing file, and don't run the second cell."
             ]
         },
         {
             "cell_type": "code",
@@ -92,18 +92,18 @@
                 "import os\n",
                 "import pyarrow.parquet as pq\n",
                 "\n",
                 "sample_file_size = os.path.getsize(sample_parquet_file)\n",
                 "parquet_file = pq.ParquetFile(sample_parquet_file)\n",
                 "num_rows = parquet_file.metadata.num_rows\n",
                 "\n",
-                "## 100MB\n",
-                "ideal_file_small = 100 * 1024 * 1024\n",
-                "## 800MB\n",
-                "ideal_file_large = 800 * 1024 * 1024\n",
+                "## 300MB\n",
+                "ideal_file_small = 300 * 1024 * 1024\n",
+                "## 1G\n",
+                "ideal_file_large = 1024 * 1024 * 1024\n",
                 "\n",
                 "threshold_small = ideal_file_small / sample_file_size * num_rows\n",
                 "threshold_large = ideal_file_large / sample_file_size * num_rows\n",
                 "\n",
                 "print(f\"threshold between {int(threshold_small):_} and {int(threshold_large):_}\")"
             ]
         },
@@ -187,23 +187,28 @@
                 "pd.DataFrame({\"name\": parquet_file.schema.names, \"size\": sizes.astype(int), \"percent\": percents}).sort_values(\n",
                 "    \"size\", ascending=False\n",
                 ")"
             ]
         }
     ],
     "metadata": {
+        "kernelspec": {
+            "display_name": "hipscatenv",
+            "language": "python",
+            "name": "python3"
+        },
         "language_info": {
             "codemirror_mode": {
                 "name": "ipython",
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.9.15"
+            "version": "3.10.14"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 5
 }
```

### Comparing `hipscat_import-0.3.2/docs/notebooks/unequal_schema.ipynb` & `hipscat_import-0.3.3/docs/notebooks/unequal_schema.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9977678571428572%*

 * *Differences: {"'metadata'": "{'language_info': {'version': '3.10.14'}}"}*

```diff
@@ -304,13 +304,13 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.10.13"
+            "version": "3.10.14"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 2
 }
```

### Comparing `hipscat_import-0.3.2/docs/static/allwise_schema.parquet` & `hipscat_import-0.3.3/docs/static/allwise_schema.parquet`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.2/docs/static/allwise_types.csv` & `hipscat_import-0.3.3/docs/static/allwise_types.csv`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.2/docs/static/neowise_schema.parquet` & `hipscat_import-0.3.3/docs/static/neowise_schema.parquet`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.2/docs/static/neowise_types.csv` & `hipscat_import-0.3.3/docs/static/neowise_types.csv`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.2/docs/static/ps1_detections_types.csv` & `hipscat_import-0.3.3/docs/static/ps1_detections_types.csv`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.2/docs/static/ps1_otmo_types.csv` & `hipscat_import-0.3.3/docs/static/ps1_otmo_types.csv`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.2/docs/static/sdss_wget.bash` & `hipscat_import-0.3.3/docs/static/sdss_wget.bash`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.2/docs/static/tic_schema.parquet` & `hipscat_import-0.3.3/docs/static/tic_schema.parquet`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.2/docs/static/tic_types.csv` & `hipscat_import-0.3.3/docs/static/tic_types.csv`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.2/pyproject.toml` & `hipscat_import-0.3.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -14,21 +14,22 @@
     "Programming Language :: Python",
 ]
 dynamic = ["version"]
 dependencies = [
     "dask[complete]>=2024.3.0", # Includes dask expressions.
     "deprecated",
     "healpy",
-    "hipscat >=0.3.0",
+    "hipscat >=0.3.4",
     "ipykernel", # Support for Jupyter notebooks
+    "numpy",
     "pandas",
     "pyarrow",
     "pyyaml",
+    "scipy",
     "tqdm",
-    "numpy",
 ]
 
 # On a mac, install optional dependencies with `pip install '.[dev]'` (include the single quotes)
 [project.optional-dependencies]
 dev = [
     "black", # Used for static linting of files
     "jupyter", # Clears output from Jupyter notebooks
```

### Comparing `hipscat_import-0.3.2/src/.pylintrc` & `hipscat_import-0.3.3/src/.pylintrc`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.2/src/hipscat_import/catalog/arguments.py` & `hipscat_import-0.3.3/src/hipscat_import/catalog/arguments.py`

 * *Files 6% similar despite different names*

```diff
@@ -64,14 +64,21 @@
     pixel_threshold: int = 1_000_000
     """maximum number of rows for a single resulting pixel.
     we may combine hierarchically until we near the ``pixel_threshold``"""
     mapping_healpix_order: int = -1
     """healpix order to use when mapping. will be
     ``highest_healpix_order`` unless a positive value is provided for
     ``constant_healpix_order``"""
+    delete_intermediate_parquet_files: bool = True
+    """should we delete the smaller intermediate parquet files generated in the
+    splitting stage, once the relevant reducing stage is complete?"""
+    delete_resume_log_files: bool = True
+    """should we delete task-level done files once each stage is complete?
+    if False, we will keep all sub-histograms from the mapping stage, and all
+    done marker files at the end of the pipeline."""
     debug_stats_only: bool = False
     """do not perform a map reduce and don't create a new
     catalog. generate the partition info"""
     file_reader: InputReader | str | None = None
     """instance of input reader that specifies arguments necessary for reading
     from your input files"""
     resume_plan: ResumePlan | None = None
@@ -121,14 +128,15 @@
             storage_options=self.input_storage_options,
         )
         self.resume_plan = ResumePlan(
             resume=self.resume,
             progress_bar=self.progress_bar,
             input_paths=self.input_paths,
             tmp_path=self.resume_tmp,
+            delete_resume_log_files=self.delete_resume_log_files,
         )
 
     def to_catalog_info(self, total_rows) -> CatalogInfo:
         """Catalog-type-specific dataset info."""
         info = {
             "catalog_name": self.output_artifact_name,
             "catalog_type": self.catalog_type,
```

### Comparing `hipscat_import-0.3.2/src/hipscat_import/catalog/file_readers.py` & `hipscat_import-0.3.3/src/hipscat_import/catalog/file_readers.py`

 * *Files 10% similar despite different names*

```diff
@@ -34,14 +34,15 @@
         chunksize (int): number of rows to read in a single iteration.
         schema_file (str): path to a parquet schema file. if provided, header names
             and column types will be pulled from the parquet schema metadata.
         column_names (list[str]): for CSV files, the names of columns if no header
             is available. for fits files, a list of columns to *keep*.
         skip_column_names (list[str]): for fits files, a list of columns to remove.
         type_map (dict): for CSV files, the data types to use for columns
+        kwargs: additional keyword arguments to pass to the underlying file reader.
     """
     if file_format == "csv":
         return CsvReader(
             chunksize=chunksize,
             schema_file=schema_file,
             column_names=column_names,
             type_map=type_map,
@@ -73,21 +74,28 @@
             input_file(str): path to the input file.
             read_columns(List[str]): subset of columns to read.
                 if None, all columns are read
         Yields:
             DataFrame containing chunk of file info.
         """
 
-    @abc.abstractmethod
     def provenance_info(self) -> dict:
         """Create dictionary of parameters for provenance tracking.
 
+        If any `storage_options` have been provided as kwargs, we will replace the
+        value with ``REDACTED`` for the purpose of writing to provenance info, as it
+        may contain user names or API keys.
+
         Returns:
             dictionary with all argument_name -> argument_value as key -> value pairs.
         """
+        all_args = vars(self)
+        if "kwargs" in all_args and "storage_options" in all_args["kwargs"]:
+            all_args["kwargs"]["storage_options"] = "REDACTED"
+        return {"input_reader_type": type(self).__name__, **vars(self)}
 
     def regular_file_exists(self, input_file, storage_options: Union[Dict[Any, Any], None] = None, **_kwargs):
         """Check that the `input_file` points to a single regular file
 
         Raises
             FileNotFoundError: if nothing exists at path, or directory found.
         """
@@ -109,17 +117,19 @@
         header (int, list of int, None, default 'infer'): rows to
             use as the header with column names
         schema_file (str): path to a parquet schema file. if provided, header names
             and column types will be pulled from the parquet schema metadata.
         column_names (list[str]): the names of columns if no header is available
         type_map (dict): the data types to use for columns
         parquet_kwargs (dict): additional keyword arguments to use when
-            reading the parquet schema metadata.
+            reading the parquet schema metadata, passed to pandas.read_parquet.
+            See https://pandas.pydata.org/docs/reference/api/pandas.read_parquet.html
         kwargs (dict): additional keyword arguments to use when reading
-            the CSV files.
+            the CSV files with pandas.read_csv.
+            See https://pandas.pydata.org/docs/reference/api/pandas.read_csv.html
     """
 
     def __init__(
         self,
         chunksize=500_000,
         header="infer",
         schema_file=None,
@@ -165,49 +175,37 @@
             FilePointer(input_file),
             chunksize=self.chunksize,
             header=self.header,
             **self.kwargs,
         ) as reader:
             yield from reader
 
-    def provenance_info(self) -> dict:
-        str_kwargs = {}
-        if self.type_map:
-            str_kwargs = {key: str(value) for (key, value) in self.kwargs.items()}
-        provenance_info = {
-            "input_reader_type": "CsvReader",
-            "chunksize": self.chunksize,
-            "schema_file": self.schema_file,
-            "column_names": self.column_names,
-            "parquet_kwargs": self.parquet_kwargs,
-            "kwargs": str_kwargs,
-        }
-        return provenance_info
-
 
 class AstropyEcsvReader(InputReader):
     """Reads astropy ascii .ecsv files.
 
     Note that this is NOT a chunked reader. Use caution when reading
-    large ECSV files with this reader."""
+    large ECSV files with this reader.
+
+    Attributes:
+        kwargs: keyword arguments passed to astropy ascii reader.
+            See https://docs.astropy.org/en/stable/api/astropy.io.ascii.read.html#astropy.io.ascii.read
+    """
 
     def __init__(self, **kwargs):
         self.kwargs = kwargs
 
     def read(self, input_file, read_columns=None):
         self.regular_file_exists(input_file, **self.kwargs)
         if read_columns:
             self.kwargs["include_names"] = read_columns
 
         astropy_table = ascii_reader.read(input_file, format="ecsv", **self.kwargs)
         yield astropy_table.to_pandas()
 
-    def provenance_info(self):
-        return {"input_reader_type": "AstropyEcsvReader"}
-
 
 class FitsReader(InputReader):
     """Chunked FITS file reader.
 
     There are two column-level arguments for reading fits files:
     `column_names` and `skip_column_names`.
 
@@ -224,14 +222,16 @@
         chunksize (int): number of rows of the file to process at once.
             For large files, this can prevent loading the entire file
             into memory at once.
         column_names (list[str]): list of column names to keep. only use
             one of `column_names` or `skip_column_names`
         skip_column_names (list[str]): list of column names to skip. only use
             one of `column_names` or `skip_column_names`
+        kwargs: keyword arguments passed along to astropy.Table.read.
+            See https://docs.astropy.org/en/stable/api/astropy.table.Table.html#astropy.table.Table.read
     """
 
     def __init__(self, chunksize=500_000, column_names=None, skip_column_names=None, **kwargs):
         self.chunksize = chunksize
         self.column_names = column_names
         self.skip_column_names = skip_column_names
         self.kwargs = kwargs
@@ -260,42 +260,34 @@
                         lambda x: x.decode("utf-8") if isinstance(x, bytes) else x
                     )
 
             yield df_chunk
 
             read_rows += self.chunksize
 
-    def provenance_info(self) -> dict:
-        provenance_info = {
-            "input_reader_type": "FitsReader",
-            "chunksize": self.chunksize,
-            "column_names": self.column_names,
-            "skip_column_names": self.skip_column_names,
-        }
-        return provenance_info
-
 
 class ParquetReader(InputReader):
     """Parquet reader for the most common Parquet reading arguments.
 
     Attributes:
         chunksize (int): number of rows of the file to process at once.
             For large files, this can prevent loading the entire file
             into memory at once.
+        column_names (list[str] or None): Names of columns to use from the input dataset.
+            If None, use all columns.
+        kwargs: arguments to pass along to pyarrow.parquet.ParquetFile.
+            See https://arrow.apache.org/docs/python/generated/pyarrow.parquet.ParquetFile.html
     """
 
-    def __init__(self, chunksize=500_000, **kwargs):
+    def __init__(self, chunksize=500_000, column_names=None, **kwargs):
         self.chunksize = chunksize
+        self.column_names = column_names
         self.kwargs = kwargs
 
     def read(self, input_file, read_columns=None):
         self.regular_file_exists(input_file, **self.kwargs)
+        columns = read_columns or self.column_names
         parquet_file = pq.ParquetFile(input_file, **self.kwargs)
-        for smaller_table in parquet_file.iter_batches(batch_size=self.chunksize, use_pandas_metadata=True):
+        for smaller_table in parquet_file.iter_batches(
+            batch_size=self.chunksize, columns=columns, use_pandas_metadata=True
+        ):
             yield smaller_table.to_pandas()
-
-    def provenance_info(self) -> dict:
-        provenance_info = {
-            "input_reader_type": "ParquetReader",
-            "chunksize": self.chunksize,
-        }
-        return provenance_info
```

### Comparing `hipscat_import-0.3.2/src/hipscat_import/catalog/map_reduce.py` & `hipscat_import-0.3.3/src/hipscat_import/catalog/map_reduce.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from hipscat.io import FilePointer, file_io, paths
 from hipscat.pixel_math.healpix_pixel import HealpixPixel
 from hipscat.pixel_math.hipscat_id import HIPSCAT_ID_COLUMN, hipscat_id_to_healpix
 
 from hipscat_import.catalog.file_readers import InputReader
 from hipscat_import.catalog.resume_plan import ResumePlan
 from hipscat_import.catalog.sparse_histogram import SparseHistogram
-from hipscat_import.pipeline_resume_plan import get_pixel_cache_directory
+from hipscat_import.pipeline_resume_plan import get_pixel_cache_directory, print_task_failure
 
 # pylint: disable=too-many-locals,too-many-arguments
 
 
 def _has_named_index(dataframe):
     """Heuristic to determine if a dataframe has some meaningful index.
 
@@ -90,30 +90,36 @@
     Returns:
         one-dimensional numpy array of long integers where the value at each index corresponds
         to the number of objects found at the healpix pixel.
     Raises:
         ValueError: if the `ra_column` or `dec_column` cannot be found in the input file.
         FileNotFoundError: if the file does not exist, or is a directory
     """
-    histo = SparseHistogram.make_empty(highest_order)
+    try:
+        histo = SparseHistogram.make_empty(highest_order)
 
-    if use_hipscat_index:
-        read_columns = [HIPSCAT_ID_COLUMN]
-    else:
-        read_columns = [ra_column, dec_column]
-
-    for _, _, mapped_pixels in _iterate_input_file(
-        input_file, file_reader, highest_order, ra_column, dec_column, use_hipscat_index, read_columns
-    ):
-        mapped_pixel, count_at_pixel = np.unique(mapped_pixels, return_counts=True)
+        if use_hipscat_index:
+            read_columns = [HIPSCAT_ID_COLUMN]
+        else:
+            read_columns = [ra_column, dec_column]
 
-        partial = SparseHistogram.make_from_counts(mapped_pixel, count_at_pixel, healpix_order=highest_order)
-        histo.add(partial)
+        for _, _, mapped_pixels in _iterate_input_file(
+            input_file, file_reader, highest_order, ra_column, dec_column, use_hipscat_index, read_columns
+        ):
+            mapped_pixel, count_at_pixel = np.unique(mapped_pixels, return_counts=True)
 
-    histo.to_file(ResumePlan.partial_histogram_file(tmp_path=resume_path, mapping_key=mapping_key))
+            partial = SparseHistogram.make_from_counts(
+                mapped_pixel, count_at_pixel, healpix_order=highest_order
+            )
+            histo.add(partial)
+
+        histo.to_file(ResumePlan.partial_histogram_file(tmp_path=resume_path, mapping_key=mapping_key))
+    except Exception as exception:  # pylint: disable=broad-exception-caught
+        print_task_failure(f"Failed MAPPING stage with file {input_file}", exception)
+        raise exception
 
 
 def split_pixels(
     input_file: FilePointer,
     file_reader: InputReader,
     splitting_key,
     highest_order,
@@ -138,38 +144,42 @@
         cache_shard_path (FilePointer): where to write intermediate parquet files.
         resume_path (FilePointer): where to write resume files.
 
     Raises:
         ValueError: if the `ra_column` or `dec_column` cannot be found in the input file.
         FileNotFoundError: if the file does not exist, or is a directory
     """
-    for chunk_number, data, mapped_pixels in _iterate_input_file(
-        input_file, file_reader, highest_order, ra_column, dec_column, use_hipscat_index
-    ):
-        aligned_pixels = alignment[mapped_pixels]
-        unique_pixels, unique_inverse = np.unique(aligned_pixels, return_inverse=True)
-
-        for unique_index, [order, pixel, _] in enumerate(unique_pixels):
-            mapped_indexes = np.where(unique_inverse == unique_index)
-            data_indexes = data.index[mapped_indexes[0].tolist()]
-
-            filtered_data = data.filter(items=data_indexes, axis=0)
-
-            pixel_dir = get_pixel_cache_directory(cache_shard_path, HealpixPixel(order, pixel))
-            file_io.make_directory(pixel_dir, exist_ok=True)
-            output_file = file_io.append_paths_to_pointer(
-                pixel_dir, f"shard_{splitting_key}_{chunk_number}.parquet"
-            )
-            if _has_named_index(filtered_data):
-                filtered_data.to_parquet(output_file, index=True)
-            else:
-                filtered_data.to_parquet(output_file, index=False)
-            del filtered_data, data_indexes
-
-    ResumePlan.splitting_key_done(tmp_path=resume_path, splitting_key=splitting_key)
+    try:
+        for chunk_number, data, mapped_pixels in _iterate_input_file(
+            input_file, file_reader, highest_order, ra_column, dec_column, use_hipscat_index
+        ):
+            aligned_pixels = alignment[mapped_pixels]
+            unique_pixels, unique_inverse = np.unique(aligned_pixels, return_inverse=True)
+
+            for unique_index, [order, pixel, _] in enumerate(unique_pixels):
+                mapped_indexes = np.where(unique_inverse == unique_index)
+                data_indexes = data.index[mapped_indexes[0].tolist()]
+
+                filtered_data = data.filter(items=data_indexes, axis=0)
+
+                pixel_dir = get_pixel_cache_directory(cache_shard_path, HealpixPixel(order, pixel))
+                file_io.make_directory(pixel_dir, exist_ok=True)
+                output_file = file_io.append_paths_to_pointer(
+                    pixel_dir, f"shard_{splitting_key}_{chunk_number}.parquet"
+                )
+                if _has_named_index(filtered_data):
+                    filtered_data.to_parquet(output_file, index=True)
+                else:
+                    filtered_data.to_parquet(output_file, index=False)
+                del filtered_data, data_indexes
+
+        ResumePlan.splitting_key_done(tmp_path=resume_path, splitting_key=splitting_key)
+    except Exception as exception:  # pylint: disable=broad-exception-caught
+        print_task_failure(f"Failed SPLITTING stage with file {input_file}", exception)
+        raise exception
 
 
 def reduce_pixel_shards(
     cache_shard_path,
     resume_path,
     reducing_key,
     destination_pixel_order,
@@ -223,88 +233,103 @@
         use_schema_file (str): use the parquet schema from the indicated
             parquet file.
 
     Raises:
         ValueError: if the number of rows written doesn't equal provided
             `destination_pixel_size`
     """
-    destination_dir = paths.pixel_directory(output_path, destination_pixel_order, destination_pixel_number)
-    file_io.make_directory(destination_dir, exist_ok=True, storage_options=storage_options)
-
-    destination_file = paths.pixel_catalog_file(
-        output_path, destination_pixel_order, destination_pixel_number
-    )
-
-    schema = None
-    if use_schema_file:
-        schema = file_io.read_parquet_metadata(
-            use_schema_file, storage_options=storage_options
-        ).schema.to_arrow_schema()
-
-    tables = []
-    healpix_pixel = HealpixPixel(destination_pixel_order, destination_pixel_number)
-    pixel_dir = get_pixel_cache_directory(cache_shard_path, healpix_pixel)
-
-    if schema:
-        tables.append(pq.read_table(pixel_dir, schema=schema))
-    else:
-        tables.append(pq.read_table(pixel_dir))
-
-    merged_table = pa.concat_tables(tables)
-
-    rows_written = len(merged_table)
-
-    if rows_written != destination_pixel_size:
-        raise ValueError(
-            "Unexpected number of objects at pixel "
-            f"({healpix_pixel})."
-            f" Expected {destination_pixel_size}, wrote {rows_written}"
+    try:
+        destination_dir = paths.pixel_directory(
+            output_path, destination_pixel_order, destination_pixel_number
         )
+        file_io.make_directory(destination_dir, exist_ok=True, storage_options=storage_options)
 
-    dataframe = merged_table.to_pandas()
-    if sort_columns:
-        dataframe = dataframe.sort_values(sort_columns.split(","))
-    if add_hipscat_index:
-        ## If we had a meaningful index before, preserve it as a column.
-        if _has_named_index(dataframe):
-            dataframe = dataframe.reset_index()
-
-        dataframe[HIPSCAT_ID_COLUMN] = pixel_math.compute_hipscat_id(
-            dataframe[ra_column].values,
-            dataframe[dec_column].values,
+        destination_file = paths.pixel_catalog_file(
+            output_path, destination_pixel_order, destination_pixel_number
         )
-        dataframe = dataframe.set_index(HIPSCAT_ID_COLUMN).sort_index()
 
-        # Adjust the schema to make sure that the _hipscat_index will
-        # be saved as a uint64
+        schema = None
+        if use_schema_file:
+            schema = file_io.read_parquet_metadata(
+                use_schema_file, storage_options=storage_options
+            ).schema.to_arrow_schema()
+
+        tables = []
+        healpix_pixel = HealpixPixel(destination_pixel_order, destination_pixel_number)
+        pixel_dir = get_pixel_cache_directory(cache_shard_path, healpix_pixel)
+
         if schema:
-            pandas_index_column = schema.get_field_index("__index_level_0__")
-            if pandas_index_column != -1:
-                schema = schema.remove(pandas_index_column)
-            schema = schema.insert(0, pa.field(HIPSCAT_ID_COLUMN, pa.uint64()))
-    elif use_hipscat_index:
-        if dataframe.index.name != HIPSCAT_ID_COLUMN:
-            dataframe = dataframe.set_index(HIPSCAT_ID_COLUMN)
-        dataframe = dataframe.sort_index()
-
-    dataframe["Norder"] = np.full(rows_written, fill_value=healpix_pixel.order, dtype=np.uint8)
-    dataframe["Dir"] = np.full(rows_written, fill_value=healpix_pixel.dir, dtype=np.uint64)
-    dataframe["Npix"] = np.full(rows_written, fill_value=healpix_pixel.pixel, dtype=np.uint64)
-
-    if schema:
-        schema = (
-            schema.append(pa.field("Norder", pa.uint8()))
-            .append(pa.field("Dir", pa.uint64()))
-            .append(pa.field("Npix", pa.uint64()))
-        )
-        dataframe.to_parquet(destination_file, schema=schema, storage_options=storage_options)
-    else:
-        dataframe.to_parquet(destination_file, storage_options=storage_options)
+            tables.append(pq.read_table(pixel_dir, schema=schema))
+        else:
+            tables.append(pq.read_table(pixel_dir))
 
-    del dataframe, merged_table, tables
+        merged_table = pa.concat_tables(tables)
 
-    if delete_input_files:
-        pixel_dir = get_pixel_cache_directory(cache_shard_path, healpix_pixel)
+        rows_written = len(merged_table)
 
-        file_io.remove_directory(pixel_dir, ignore_errors=True, storage_options=storage_options)
+        if rows_written != destination_pixel_size:
+            raise ValueError(
+                "Unexpected number of objects at pixel "
+                f"({healpix_pixel})."
+                f" Expected {destination_pixel_size}, wrote {rows_written}"
+            )
+
+        dataframe = merged_table.to_pandas()
+        if sort_columns:
+            dataframe = dataframe.sort_values(sort_columns.split(","))
+        if add_hipscat_index:
+            ## If we had a meaningful index before, preserve it as a column.
+            if _has_named_index(dataframe):
+                dataframe = dataframe.reset_index()
+
+            dataframe[HIPSCAT_ID_COLUMN] = pixel_math.compute_hipscat_id(
+                dataframe[ra_column].values,
+                dataframe[dec_column].values,
+            )
+            dataframe = dataframe.set_index(HIPSCAT_ID_COLUMN).sort_index()
+
+            # Adjust the schema to make sure that the _hipscat_index will
+            # be saved as a uint64
+        elif use_hipscat_index:
+            if dataframe.index.name != HIPSCAT_ID_COLUMN:
+                dataframe = dataframe.set_index(HIPSCAT_ID_COLUMN)
+            dataframe = dataframe.sort_index()
+
+        dataframe["Norder"] = np.full(rows_written, fill_value=healpix_pixel.order, dtype=np.uint8)
+        dataframe["Dir"] = np.full(rows_written, fill_value=healpix_pixel.dir, dtype=np.uint64)
+        dataframe["Npix"] = np.full(rows_written, fill_value=healpix_pixel.pixel, dtype=np.uint64)
+
+        if schema:
+            schema = _modify_arrow_schema(schema, add_hipscat_index)
+            dataframe.to_parquet(destination_file, schema=schema, storage_options=storage_options)
+        else:
+            dataframe.to_parquet(destination_file, storage_options=storage_options)
+
+        del dataframe, merged_table, tables
+
+        if delete_input_files:
+            pixel_dir = get_pixel_cache_directory(cache_shard_path, healpix_pixel)
+
+            file_io.remove_directory(pixel_dir, ignore_errors=True, storage_options=storage_options)
+
+        ResumePlan.reducing_key_done(tmp_path=resume_path, reducing_key=reducing_key)
+    except Exception as exception:  # pylint: disable=broad-exception-caught
+        print_task_failure(
+            f"Failed REDUCING stage for shard: {destination_pixel_order} {destination_pixel_number}",
+            exception,
+        )
+        raise exception
+
+
+def _modify_arrow_schema(schema, add_hipscat_index):
+    if add_hipscat_index:
+        pandas_index_column = schema.get_field_index("__index_level_0__")
+        if pandas_index_column != -1:
+            schema = schema.remove(pandas_index_column)
+        schema = schema.insert(0, pa.field(HIPSCAT_ID_COLUMN, pa.uint64()))
+    schema = (
+        schema.append(pa.field("Norder", pa.uint8()))
+        .append(pa.field("Dir", pa.uint64()))
+        .append(pa.field("Npix", pa.uint64()))
+    )
 
-    ResumePlan.reducing_key_done(tmp_path=resume_path, reducing_key=reducing_key)
+    return schema
```

### Comparing `hipscat_import-0.3.2/src/hipscat_import/catalog/resume_plan.py` & `hipscat_import-0.3.3/src/hipscat_import/catalog/resume_plan.py`

 * *Files 0% similar despite different names*

```diff
@@ -115,18 +115,19 @@
                 raise RuntimeError(f"{len(remaining_map_files)} map stages did not complete successfully.")
             histogram_files = file_io.find_files_matching_path(self.tmp_path, self.HISTOGRAMS_DIR, "*.npz")
             aggregate_histogram = SparseHistogram.make_empty(healpix_order)
             for partial_file_name in histogram_files:
                 aggregate_histogram.add(SparseHistogram.from_file(partial_file_name))
 
             aggregate_histogram.to_file(file_name)
-            file_io.remove_directory(
-                file_io.append_paths_to_pointer(self.tmp_path, self.HISTOGRAMS_DIR),
-                ignore_errors=True,
-            )
+            if self.delete_resume_log_files:
+                file_io.remove_directory(
+                    file_io.append_paths_to_pointer(self.tmp_path, self.HISTOGRAMS_DIR),
+                    ignore_errors=True,
+                )
 
         full_histogram = SparseHistogram.from_file(file_name).to_array()
 
         if len(full_histogram) != hp.order2npix(healpix_order):
             raise ValueError(
                 "The histogram from the previous execution is incompatible with "
                 + "the highest healpix order. To start the importing pipeline "
@@ -233,12 +234,12 @@
 
     def is_reducing_done(self) -> bool:
         """Are there partitions left to reduce?"""
         return self.done_file_exists(self.REDUCING_STAGE)
 
     def wait_for_reducing(self, futures):
         """Wait for reducing futures to complete."""
-        self.wait_for_futures(futures, self.REDUCING_STAGE)
+        self.wait_for_futures(futures, self.REDUCING_STAGE, fail_fast=True)
         remaining_reduce_items = self.get_reduce_items()
         if len(remaining_reduce_items) > 0:
             raise RuntimeError(f"{len(remaining_reduce_items)} reduce stages did not complete successfully.")
         self.touch_stage_done_file(self.REDUCING_STAGE)
```

### Comparing `hipscat_import-0.3.2/src/hipscat_import/catalog/run_import.py` & `hipscat_import-0.3.3/src/hipscat_import/catalog/run_import.py`

 * *Files 1% similar despite different names*

```diff
@@ -94,14 +94,15 @@
                 output_path=args.catalog_path,
                 ra_column=args.ra_column,
                 dec_column=args.dec_column,
                 sort_columns=args.sort_columns,
                 add_hipscat_index=args.add_hipscat_index,
                 use_schema_file=args.use_schema_file,
                 use_hipscat_index=args.use_hipscat_index,
+                delete_input_files=args.delete_intermediate_parquet_files,
                 storage_options=args.output_storage_options,
             )
         )
 
     args.resume_plan.wait_for_reducing(futures)
```

### Comparing `hipscat_import-0.3.2/src/hipscat_import/catalog/sparse_histogram.py` & `hipscat_import-0.3.3/src/hipscat_import/catalog/sparse_histogram.py`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.2/src/hipscat_import/index/arguments.py` & `hipscat_import-0.3.3/src/hipscat_import/index/arguments.py`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.2/src/hipscat_import/index/map_reduce.py` & `hipscat_import-0.3.3/src/hipscat_import/index/map_reduce.py`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.2/src/hipscat_import/index/run_index.py` & `hipscat_import-0.3.3/src/hipscat_import/index/run_index.py`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.2/src/hipscat_import/margin_cache/margin_cache.py` & `hipscat_import-0.3.3/src/hipscat_import/margin_cache/margin_cache_map_reduce.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,170 +1,167 @@
+import healpy as hp
+import numpy as np
 import pandas as pd
-from dask.distributed import as_completed
+import pyarrow as pa
+import pyarrow.dataset as ds
 from hipscat import pixel_math
-from hipscat.catalog import PartitionInfo
-from hipscat.io import file_io, parquet_metadata, paths, write_metadata
-from tqdm.auto import tqdm
-
-import hipscat_import.margin_cache.margin_cache_map_reduce as mcmr
-
-# pylint: disable=too-many-locals,too-many-arguments
-
-
-def _find_partition_margin_pixel_pairs(stats, margin_order):
-    """Creates a DataFrame filled with many-to-many connections between
-    the catalog partition pixels and the margin pixels at `margin_order`.
-    """
-    norders = []
-    part_pix = []
-    margin_pix = []
-
-    for healpixel in stats:
-        order = healpixel.order
-        pix = healpixel.pixel
+from hipscat.catalog.partition_info import PartitionInfo
+from hipscat.io import file_io, paths
+from hipscat.pixel_math.healpix_pixel import HealpixPixel
+from hipscat.pixel_math.hipscat_id import HIPSCAT_ID_COLUMN
+
+from hipscat_import.margin_cache.margin_cache_resume_plan import MarginCachePlan
+from hipscat_import.pipeline_resume_plan import get_pixel_cache_directory, print_task_failure
+
+
+def map_pixel_shards(
+    partition_file,
+    mapping_key,
+    input_storage_options,
+    original_catalog_metadata,
+    margin_pair_file,
+    margin_threshold,
+    output_path,
+    margin_order,
+    ra_column,
+    dec_column,
+):
+    """Creates margin cache shards from a source partition file."""
+    try:
+        schema = file_io.read_parquet_metadata(
+            original_catalog_metadata, storage_options=input_storage_options
+        ).schema.to_arrow_schema()
+        data = file_io.load_parquet_to_pandas(
+            partition_file, schema=schema, storage_options=input_storage_options
+        )
+
+        data["margin_pixel"] = hp.ang2pix(
+            2**margin_order,
+            data[ra_column].values,
+            data[dec_column].values,
+            lonlat=True,
+            nest=True,
+        )
+
+        margin_pairs = pd.read_csv(margin_pair_file)
+        constrained_data = data.reset_index().merge(margin_pairs, on="margin_pixel")
+
+        if len(constrained_data):
+            constrained_data.groupby(["partition_order", "partition_pixel"]).apply(
+                _to_pixel_shard,
+                margin_threshold=margin_threshold,
+                output_path=output_path,
+                ra_column=ra_column,
+                dec_column=dec_column,
+            )
 
-        d_order = margin_order - order
+        MarginCachePlan.mapping_key_done(output_path, mapping_key)
+    except Exception as exception:  # pylint: disable=broad-exception-caught
+        print_task_failure(f"Failed MAPPING stage for pixel: {mapping_key}", exception)
+        raise exception
 
-        margins = pixel_math.get_margin(order, pix, d_order)
 
-        for m_p in margins:
-            norders.append(order)
-            part_pix.append(pix)
-            margin_pix.append(m_p)
+def _to_pixel_shard(data, margin_threshold, output_path, ra_column, dec_column):
+    """Do boundary checking for the cached partition and then output remaining data."""
+    order, pix = data["partition_order"].iloc[0], data["partition_pixel"].iloc[0]
+    source_order, source_pix = data["Norder"].iloc[0], data["Npix"].iloc[0]
 
-    margin_pairs_df = pd.DataFrame(
-        zip(norders, part_pix, margin_pix),
-        columns=["partition_order", "partition_pixel", "margin_pixel"],
+    data["margin_check"] = pixel_math.check_margin_bounds(
+        data[ra_column].values, data[dec_column].values, order, pix, margin_threshold
     )
-    return margin_pairs_df
 
+    # pylint: disable-next=singleton-comparison
+    margin_data = data.loc[data["margin_check"] == True]
 
-def _create_margin_directory(stats, output_path, storage_options):
-    """Creates directories for all the catalog partitions."""
-    for healpixel in stats:
-        order = healpixel.order
-        pix = healpixel.pixel
-
-        destination_dir = paths.pixel_directory(output_path, order, pix)
-        file_io.make_directory(destination_dir, exist_ok=True, storage_options=storage_options)
-
-
-def _map_to_margin_shards(client, args, partition_pixels, margin_pairs):
-    """Create all the jobs for mapping partition files into the margin cache."""
-    futures = []
-    mp_future = client.scatter(margin_pairs, broadcast=True)
-    for pix in partition_pixels:
-        partition_file = paths.pixel_catalog_file(args.input_catalog_path, pix.order, pix.pixel)
-        futures.append(
-            client.submit(
-                mcmr.map_pixel_shards,
-                partition_file=partition_file,
-                input_storage_options=args.input_storage_options,
-                margin_pairs=mp_future,
-                margin_threshold=args.margin_threshold,
-                output_path=args.tmp_path,
-                margin_order=args.margin_order,
-                ra_column=args.catalog.catalog_info.ra_column,
-                dec_column=args.catalog.catalog_info.dec_column,
+    if len(margin_data):
+        # generate a file name for our margin shard, that uses both sets of Norder/Npix
+        partition_dir = get_pixel_cache_directory(output_path, HealpixPixel(order, pix))
+        shard_dir = paths.pixel_directory(partition_dir, source_order, source_pix)
+
+        file_io.make_directory(shard_dir, exist_ok=True)
+
+        shard_path = paths.pixel_catalog_file(partition_dir, source_order, source_pix)
+
+        final_df = margin_data.drop(
+            columns=[
+                "margin_check",
+                "margin_pixel",
+            ]
+        )
+
+        rename_columns = {
+            PartitionInfo.METADATA_ORDER_COLUMN_NAME: f"margin_{PartitionInfo.METADATA_ORDER_COLUMN_NAME}",
+            PartitionInfo.METADATA_DIR_COLUMN_NAME: f"margin_{PartitionInfo.METADATA_DIR_COLUMN_NAME}",
+            PartitionInfo.METADATA_PIXEL_COLUMN_NAME: f"margin_{PartitionInfo.METADATA_PIXEL_COLUMN_NAME}",
+            "partition_order": PartitionInfo.METADATA_ORDER_COLUMN_NAME,
+            "partition_pixel": PartitionInfo.METADATA_PIXEL_COLUMN_NAME,
+        }
+
+        final_df.rename(columns=rename_columns, inplace=True)
+
+        dir_column = np.floor_divide(final_df[PartitionInfo.METADATA_PIXEL_COLUMN_NAME].values, 10000) * 10000
+
+        final_df[PartitionInfo.METADATA_DIR_COLUMN_NAME] = dir_column
+
+        final_df = final_df.astype(
+            {
+                PartitionInfo.METADATA_ORDER_COLUMN_NAME: np.uint8,
+                PartitionInfo.METADATA_DIR_COLUMN_NAME: np.uint64,
+                PartitionInfo.METADATA_PIXEL_COLUMN_NAME: np.uint64,
+            }
+        )
+        final_df = final_df.set_index(HIPSCAT_ID_COLUMN).sort_index()
+
+        final_df.to_parquet(shard_path)
+
+        del data, margin_data, final_df
+
+
+def reduce_margin_shards(
+    intermediate_directory,
+    reducing_key,
+    output_path,
+    output_storage_options,
+    partition_order,
+    partition_pixel,
+    original_catalog_metadata,
+    delete_intermediate_parquet_files,
+    input_storage_options,
+):
+    """Reduce all partition pixel directories into a single file"""
+    try:
+        shard_dir = get_pixel_cache_directory(
+            intermediate_directory, HealpixPixel(partition_order, partition_pixel)
+        )
+        if file_io.does_file_or_directory_exist(shard_dir):
+            schema = file_io.read_parquet_metadata(
+                original_catalog_metadata, storage_options=input_storage_options
+            ).schema.to_arrow_schema()
+
+            schema = (
+                schema.append(pa.field("margin_Norder", pa.uint8()))
+                .append(pa.field("margin_Dir", pa.uint64()))
+                .append(pa.field("margin_Npix", pa.uint64()))
             )
-        )
-
-    for _ in tqdm(
-        as_completed(futures),
-        desc="Mapping  ",
-        total=len(futures),
-        disable=not args.progress_bar,
-    ):
-        ...
-
-
-def _reduce_margin_shards(client, args, partition_pixels):
-    """Create all the jobs for reducing margin cache shards into singular files"""
-    futures = []
-
-    for pix in partition_pixels:
-        futures.append(
-            client.submit(
-                mcmr.reduce_margin_shards,
-                intermediate_directory=args.tmp_path,
-                output_path=args.catalog_path,
-                output_storage_options=args.output_storage_options,
-                partition_order=pix.order,
-                partition_pixel=pix.pixel,
-                original_catalog_metadata=paths.get_common_metadata_pointer(args.input_catalog_path),
-                input_storage_options=args.input_storage_options,
-            )
-        )
+            data = ds.dataset(shard_dir, format="parquet", schema=schema)
+            full_df = data.to_table().to_pandas()
 
-    for _ in tqdm(
-        as_completed(futures),
-        desc="Reducing ",
-        total=len(futures),
-        disable=not args.progress_bar,
-    ):
-        ...
-
-
-def generate_margin_cache(args, client):
-    """Generate a margin cache for a given input catalog.
-    The input catalog must be in hipscat format.
-
-    Args:
-        args (MarginCacheArguments): A valid `MarginCacheArguments` object.
-        client (dask.distributed.Client): A dask distributed client object.
-    """
-    # determine which order to generate margin pixels for
-    partition_stats = args.catalog.partition_info.get_healpix_pixels()
-
-    # get the negative tree pixels
-    negative_pixels = args.catalog.generate_negative_tree_pixels()
-
-    combined_pixels = partition_stats + negative_pixels
-
-    margin_pairs = _find_partition_margin_pixel_pairs(combined_pixels, args.margin_order)
-
-    _create_margin_directory(combined_pixels, args.catalog_path, args.output_storage_options)
-
-    _map_to_margin_shards(
-        client=client,
-        args=args,
-        partition_pixels=partition_stats,
-        margin_pairs=margin_pairs,
-    )
-
-    _reduce_margin_shards(client=client, args=args, partition_pixels=combined_pixels)
-
-    with tqdm(total=4, desc="Finishing", disable=not args.progress_bar) as step_progress:
-        parquet_metadata.write_parquet_metadata(
-            args.catalog_path, storage_options=args.output_storage_options
-        )
-        step_progress.update(1)
-        total_rows = 0
-        metadata_path = paths.get_parquet_metadata_pointer(args.catalog_path)
-        for row_group in parquet_metadata.read_row_group_fragments(
-            metadata_path, storage_options=args.output_storage_options
-        ):
-            total_rows += row_group.num_rows
-        partition_info = PartitionInfo.read_from_file(
-            metadata_path, storage_options=args.output_storage_options
-        )
-        partition_info_file = paths.get_partition_info_pointer(args.catalog_path)
-        partition_info.write_to_file(partition_info_file, storage_options=args.output_storage_options)
-
-        step_progress.update(1)
-        margin_catalog_info = args.to_catalog_info(int(total_rows))
-        write_metadata.write_provenance_info(
-            catalog_base_dir=args.catalog_path,
-            dataset_info=margin_catalog_info,
-            tool_args=args.provenance_info(),
-            storage_options=args.output_storage_options,
-        )
-        write_metadata.write_catalog_info(
-            catalog_base_dir=args.catalog_path,
-            dataset_info=margin_catalog_info,
-            storage_options=args.output_storage_options,
-        )
-        step_progress.update(1)
-        file_io.remove_directory(
-            args.tmp_path, ignore_errors=True, storage_options=args.output_storage_options
-        )
-        step_progress.update(1)
+            if len(full_df):
+                margin_cache_dir = paths.pixel_directory(output_path, partition_order, partition_pixel)
+                file_io.make_directory(
+                    margin_cache_dir, exist_ok=True, storage_options=output_storage_options
+                )
+
+                margin_cache_file_path = paths.pixel_catalog_file(
+                    output_path, partition_order, partition_pixel
+                )
+
+                full_df.to_parquet(
+                    margin_cache_file_path, schema=schema, storage_options=output_storage_options
+                )
+                if delete_intermediate_parquet_files:
+                    file_io.remove_directory(shard_dir)
+
+        MarginCachePlan.reducing_key_done(intermediate_directory, reducing_key)
+    except Exception as exception:  # pylint: disable=broad-exception-caught
+        print_task_failure(f"Failed REDUCING stage for pixel: {reducing_key}", exception)
+        raise exception
```

### Comparing `hipscat_import-0.3.2/src/hipscat_import/margin_cache/margin_cache_arguments.py` & `hipscat_import-0.3.3/src/hipscat_import/margin_cache/margin_cache_arguments.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import warnings
-from dataclasses import dataclass
-from typing import Any, Dict, Union
+from dataclasses import dataclass, field
+from typing import Any, Dict, List, Union
 
 import healpy as hp
 from hipscat.catalog import Catalog
 from hipscat.catalog.margin_cache.margin_cache_catalog_info import MarginCacheCatalogInfo
 from hipscat.io.validation import is_valid_catalog
+from hipscat.pixel_math.healpix_pixel import HealpixPixel
 
 from hipscat_import.runtime_arguments import RuntimeArguments
 
 
 @dataclass
 class MarginCacheArguments(RuntimeArguments):
     """Container for margin cache generation arguments"""
@@ -20,35 +21,48 @@
     healpixel will result in a warning, as this may lead to data loss."""
     margin_order: int = -1
     """the order of healpixels that will be used to constrain the margin data before
     doing more precise boundary checking. this value must be greater than the highest
     order of healpix partitioning in the source catalog. if `margin_order` is left
     default or set to -1, then the `margin_order` will be set dynamically to the
     highest partition order plus 1."""
+    delete_intermediate_parquet_files: bool = True
+    """should we delete the smaller intermediate parquet files generated in the
+    splitting stage, once the relevant reducing stage is complete?"""
+    delete_resume_log_files: bool = True
+    """should we delete task-level done files once each stage is complete?
+    if False, we will keep all done marker files at the end of the pipeline."""
 
     input_catalog_path: str = ""
     """the path to the hipscat-formatted input catalog."""
     input_storage_options: Union[Dict[Any, Any], None] = None
     """optional dictionary of abstract filesystem credentials for the INPUT."""
+    debug_filter_pixel_list: List[HealpixPixel] = field(default_factory=list)
+    """debug setting. if provided, we will first filter the catalog to the pixels
+    provided. this can be useful for creating a margin over a subset of a catalog."""
 
     def __post_init__(self):
         self._check_arguments()
 
     def _check_arguments(self):
         super()._check_arguments()
         if not self.input_catalog_path:
             raise ValueError("input_catalog_path is required")
         if not is_valid_catalog(self.input_catalog_path, storage_options=self.input_storage_options):
             raise ValueError("input_catalog_path not a valid catalog")
 
         self.catalog = Catalog.read_from_hipscat(
             self.input_catalog_path, storage_options=self.input_storage_options
         )
+        if len(self.debug_filter_pixel_list) > 0:
+            self.catalog = self.catalog.filter_from_pixel_list(self.debug_filter_pixel_list)
+            if len(self.catalog.get_healpix_pixels()) == 0:
+                raise ValueError("debug_filter_pixel_list has created empty catalog")
 
-        highest_order = self.catalog.partition_info.get_highest_order()
+        highest_order = int(self.catalog.partition_info.get_highest_order())
         margin_pixel_k = highest_order + 1
         if self.margin_order > -1:
             if self.margin_order < margin_pixel_k:
                 raise ValueError(
                     "margin_order must be of a higher order "
                     "than the highest order catalog partition pixel."
                 )
@@ -75,8 +89,9 @@
         return MarginCacheCatalogInfo(**info)
 
     def additional_runtime_provenance_info(self) -> dict:
         return {
             "input_catalog_path": self.input_catalog_path,
             "margin_threshold": self.margin_threshold,
             "margin_order": self.margin_order,
+            "debug_filter_pixel_list": self.debug_filter_pixel_list,
         }
```

### Comparing `hipscat_import-0.3.2/src/hipscat_import/pipeline.py` & `hipscat_import-0.3.3/src/hipscat_import/pipeline.py`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.2/src/hipscat_import/pipeline_resume_plan.py` & `hipscat_import-0.3.3/src/hipscat_import/pipeline_resume_plan.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 
 from __future__ import annotations
 
 import re
 from dataclasses import dataclass
 from pathlib import Path
 
-from dask.distributed import as_completed
+from dask.distributed import as_completed, get_worker
+from dask.distributed import print as dask_print
 from hipscat.io import FilePointer, file_io
 from hipscat.pixel_math.healpix_pixel import HealpixPixel
 from tqdm.auto import tqdm
 
 
 @dataclass
 class PipelineResumePlan:
@@ -20,14 +21,18 @@
     """path for any intermediate files"""
     resume: bool = True
     """if there are existing intermediate resume files, should we
     read those and continue to run pipeline where we left off"""
     progress_bar: bool = True
     """if true, a tqdm progress bar will be displayed for user
     feedback of planning progress"""
+    delete_resume_log_files: bool = True
+    """should we delete task-level done files once each stage is complete?
+    if False, we will keep all sub-histograms from the mapping stage, and all
+    done marker files at the end of the pipeline."""
 
     ORIGINAL_INPUT_PATHS = "input_paths.txt"
 
     def safe_to_resume(self):
         """Check that we are ok to resume an in-progress pipeline, if one exists.
 
         Raises:
@@ -104,51 +109,43 @@
             result_file_name = file_io.get_basename_from_filepointer(file_path)
             match = re.match(r"(.*)" + extension, str(result_file_name))
             keys.append(match.group(1))
         return keys
 
     def clean_resume_files(self):
         """Remove all intermediate files created in execution."""
-        file_io.remove_directory(self.tmp_path, ignore_errors=True)
+        if self.delete_resume_log_files:
+            file_io.remove_directory(self.tmp_path, ignore_errors=True)
 
-    def wait_for_futures(self, futures, stage_name):
+    def wait_for_futures(self, futures, stage_name, fail_fast=False):
         """Wait for collected futures to complete.
 
         As each future completes, check the returned status.
 
         Args:
             futures(List[future]): collected futures
             stage_name(str): name of the stage (e.g. mapping, reducing)
+            fail_fast (bool): if True, we will re-raise the first exception
+                encountered and NOT continue. this may lead to unexpected
+                behavior for in-progress tasks.
         Raises:
             RuntimeError: if any future returns an error status.
         """
         some_error = False
         formatted_stage_name = self.get_formatted_stage_name(stage_name)
         for future in tqdm(
             as_completed(futures),
             desc=formatted_stage_name,
             total=len(futures),
             disable=(not self.progress_bar),
         ):
             if future.status == "error":
                 some_error = True
-                exception = future.exception()
-                trace_strs = [
-                    f"{stage_name} task {future.key} failed with message:",
-                    f"  {type(exception).__name__}: {exception}",
-                    "  Traceback (most recent call last):",
-                ]
-                stack_trace = exception.__traceback__
-                while stack_trace is not None:
-                    filename = stack_trace.tb_frame.f_code.co_filename
-                    method_name = stack_trace.tb_frame.f_code.co_name
-                    line_number = stack_trace.tb_lineno
-                    trace_strs.append(f'    File "{filename}", line {line_number}, in {method_name}')
-                    stack_trace = stack_trace.tb_next
-                print("\n".join(trace_strs))
+                if fail_fast:
+                    raise future.exception()
 
         if some_error:
             raise RuntimeError(f"Some {stage_name} stages failed. See logs for details.")
 
     @staticmethod
     def get_formatted_stage_name(stage_name) -> str:
         """Create a stage name of consistent minimum length. Ensures that the tqdm
@@ -168,38 +165,38 @@
 
         Args:
             input_paths (list[str]): input paths that will be processed by a pipeline.
 
         Raises:
             ValueError: if the retrieved file set differs from `input_paths`.
         """
-        unique_file_paths = set(input_paths)
+        input_paths = set(input_paths)
+        input_paths = [str(p) for p in input_paths]
+        input_paths.sort()
 
         original_input_paths = []
 
-        file_path = file_io.append_paths_to_pointer(self.tmp_path, self.ORIGINAL_INPUT_PATHS)
+        log_file_path = file_io.append_paths_to_pointer(self.tmp_path, self.ORIGINAL_INPUT_PATHS)
         try:
-            with open(file_path, "r", encoding="utf-8") as file_handle:
+            with open(log_file_path, "r", encoding="utf-8") as file_handle:
                 contents = file_handle.readlines()
             contents = [path.strip() for path in contents]
-            original_input_paths = set(contents)
+            original_input_paths = list(set(contents))
+            original_input_paths.sort()
         except FileNotFoundError:
             pass
 
         if len(original_input_paths) == 0:
-            file_path = file_io.append_paths_to_pointer(self.tmp_path, self.ORIGINAL_INPUT_PATHS)
-            with open(file_path, "w", encoding="utf-8") as file_handle:
+            with open(log_file_path, "w", encoding="utf-8") as file_handle:
                 for path in input_paths:
                     file_handle.write(f"{path}\n")
         else:
-            if original_input_paths != unique_file_paths:
+            if original_input_paths != input_paths:
                 raise ValueError("Different file set from resumed pipeline execution.")
 
-        input_paths = list(unique_file_paths)
-        input_paths.sort()
         return input_paths
 
 
 def get_pixel_cache_directory(cache_path, pixel: HealpixPixel):
     """Create a path for intermediate pixel data.
 
     You can use this over the paths.get_pixel_directory method, as it will include the pixel
@@ -211,7 +208,25 @@
     Args:
         cache_path (str): root path to cache
         pixel (HealpixPixel): pixel partition data
     """
     return file_io.append_paths_to_pointer(
         cache_path, f"order_{pixel.order}", f"dir_{pixel.dir}", f"pixel_{pixel.pixel}"
     )
+
+
+def print_task_failure(custom_message, exception):
+    """Use dask's distributed print feature to print the exception message to the task's logs
+    and to the controller job's logs.
+
+    Optionally print the worker address if a worker is found.
+
+    Args:
+        custom_message (str): some custom message for the task that might help with debugging
+        exception (Exception): error raised in execution of the task.
+    """
+    dask_print(custom_message)
+    try:
+        dask_print("  worker address:", get_worker().address)
+    except Exception:  # pylint: disable=broad-exception-caught
+        pass
+    dask_print(exception)
```

### Comparing `hipscat_import-0.3.2/src/hipscat_import/runtime_arguments.py` & `hipscat_import-0.3.3/src/hipscat_import/runtime_arguments.py`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.2/src/hipscat_import/soap/arguments.py` & `hipscat_import-0.3.3/src/hipscat_import/soap/arguments.py`

 * *Files 11% similar despite different names*

```diff
@@ -24,17 +24,23 @@
     source_id_column: str = ""
     source_storage_options: Union[Dict[Any, Any], None] = None
     """optional dictionary of abstract filesystem credentials for the SOURCE catalog."""
 
     resume: bool = True
     """if there are existing intermediate resume files, should we
     read those and continue to run the pipeline where we left off"""
+    delete_resume_log_files: bool = True
+    """should we delete task-level done files once each stage is complete?
+    if False, we will keep all done marker files at the end of the pipeline."""
     write_leaf_files: bool = False
     """Should we also write out leaf parquet files (e.g. Norder/Dir/Npix.parquet)
     that represent the full association table"""
+    delete_intermediate_parquet_files: bool = True
+    """should we delete the smaller intermediate parquet files generated in the
+    mapping stage, once the relevant reducing stage is complete?"""
 
     compute_partition_size: int = 1_000_000_000
 
     def __post_init__(self):
         self._check_arguments()
 
     def _check_arguments(self):
```

### Comparing `hipscat_import-0.3.2/src/hipscat_import/soap/map_reduce.py` & `hipscat_import-0.3.3/src/hipscat_import/soap/map_reduce.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from hipscat.catalog.association_catalog.partition_join_info import PartitionJoinInfo
 from hipscat.io import FilePointer, file_io, paths
 from hipscat.io.file_io.file_pointer import get_fs, strip_leading_slash_for_pyarrow
 from hipscat.io.parquet_metadata import get_healpix_pixel_from_metadata
 from hipscat.pixel_math.healpix_pixel import HealpixPixel
 from hipscat.pixel_math.healpix_pixel_function import get_pixel_argsort
 
-from hipscat_import.pipeline_resume_plan import get_pixel_cache_directory
+from hipscat_import.pipeline_resume_plan import get_pixel_cache_directory, print_task_failure
 from hipscat_import.soap.arguments import SoapArguments
 from hipscat_import.soap.resume_plan import SoapPlan
 
 
 def _count_joins_for_object(source_data, source_pixel, object_pixel, soap_args):
     object_path = paths.pixel_catalog_file(
         catalog_base_dir=soap_args.object_catalog_dir,
@@ -90,47 +90,51 @@
 
     Args:
         soap_args(`hipscat_import.soap.SoapArguments`): set of arguments for pipeline execution
         source_pixel(HealpixPixel): order and pixel for the source catalog single pixel.
         object_pixels(List[HealpixPixel]): set of tuples of order and pixel for the partitions
             of the object catalog to be joined.
     """
-    source_path = paths.pixel_catalog_file(
-        catalog_base_dir=file_io.get_file_pointer_from_path(soap_args.source_catalog_dir),
-        pixel_order=source_pixel.order,
-        pixel_number=source_pixel.pixel,
-    )
-    if soap_args.write_leaf_files and soap_args.source_object_id_column != soap_args.source_id_column:
-        read_columns = [soap_args.source_object_id_column, soap_args.source_id_column]
-    else:
-        read_columns = [soap_args.source_object_id_column]
-    source_data = file_io.load_parquet_to_pandas(
-        source_path, columns=read_columns, storage_options=soap_args.source_storage_options
-    ).set_index(soap_args.source_object_id_column)
-
-    remaining_sources = len(source_data)
-    results = []
-
-    for object_pixel in object_pixels:
-        if remaining_sources < 1:
-            break
-        join_count = _count_joins_for_object(
-            source_data,
-            source_pixel,
-            object_pixel,
-            soap_args,
+    try:
+        source_path = paths.pixel_catalog_file(
+            catalog_base_dir=file_io.get_file_pointer_from_path(soap_args.source_catalog_dir),
+            pixel_order=source_pixel.order,
+            pixel_number=source_pixel.pixel,
         )
-        results.append([object_pixel.order, object_pixel.pixel, join_count])
-        remaining_sources -= join_count
-
-    ## mark that some sources were not joined
-    if remaining_sources > 0:
-        results.append([-1, -1, remaining_sources])
-
-    _write_count_results(soap_args.tmp_path, source_pixel, results)
+        if soap_args.write_leaf_files and soap_args.source_object_id_column != soap_args.source_id_column:
+            read_columns = [soap_args.source_object_id_column, soap_args.source_id_column]
+        else:
+            read_columns = [soap_args.source_object_id_column]
+        source_data = file_io.load_parquet_to_pandas(
+            source_path, columns=read_columns, storage_options=soap_args.source_storage_options
+        ).set_index(soap_args.source_object_id_column)
+
+        remaining_sources = len(source_data)
+        results = []
+
+        for object_pixel in object_pixels:
+            if remaining_sources < 1:
+                break
+            join_count = _count_joins_for_object(
+                source_data,
+                source_pixel,
+                object_pixel,
+                soap_args,
+            )
+            results.append([object_pixel.order, object_pixel.pixel, join_count])
+            remaining_sources -= join_count
+
+        ## mark that some sources were not joined
+        if remaining_sources > 0:
+            results.append([-1, -1, remaining_sources])
+
+        _write_count_results(soap_args.tmp_path, source_pixel, results)
+    except Exception as exception:  # pylint: disable=broad-exception-caught
+        print_task_failure(f"Failed COUNTING stage for shard: {source_pixel}", exception)
+        raise exception
 
 
 def combine_partial_results(input_path, output_path, output_storage_options) -> int:
     """Combine many partial CSVs into single partition join info.
     Also write out a debug file with counts of unmatched sources, if any.
 
     Args:
@@ -183,53 +187,59 @@
 
 
 def reduce_joins(
     soap_args: SoapArguments, object_pixel: HealpixPixel, object_key: str, delete_input_files: bool = True
 ):
     """Reduce join tables into one parquet file per object-pixel, with one row-group
     inside per source pixel."""
-    pixel_dir = get_pixel_cache_directory(soap_args.tmp_path, object_pixel)
-    # If there's no directory, this implies there were no matches to this object pixel
-    # earlier in the pipeline. Move on.
-    if not file_io.does_file_or_directory_exist(pixel_dir):
-        return
-    # Find all of the constituent files / source pixels. Create a list of PyArrow Tables from those
-    # parquet files. We need to know the schema before we create the ParquetWriter.
-    shard_file_list = file_io.find_files_matching_path(pixel_dir, "source*.parquet")
-
-    if len(shard_file_list) == 0:
-        return
-
-    ## We want to order the row groups in a "breadth-first" sorting. Determine our sorting
-    ## via the metadata, then read the tables in using that sorting.
-    healpix_pixels = []
-    for shard_file_name in shard_file_list:
-        healpix_pixels.append(
-            get_healpix_pixel_from_metadata(pq.read_metadata(shard_file_name), "join_Norder", "join_Npix")
+    try:
+        pixel_dir = get_pixel_cache_directory(soap_args.tmp_path, object_pixel)
+        # If there's no directory, this implies there were no matches to this object pixel
+        # earlier in the pipeline. Move on.
+        if not file_io.does_file_or_directory_exist(pixel_dir):
+            return
+        # Find all of the constituent files / source pixels. Create a list of PyArrow Tables from those
+        # parquet files. We need to know the schema before we create the ParquetWriter.
+        shard_file_list = file_io.find_files_matching_path(pixel_dir, "source*.parquet")
+
+        if len(shard_file_list) == 0:
+            return
+
+        ## We want to order the row groups in a "breadth-first" sorting. Determine our sorting
+        ## via the metadata, then read the tables in using that sorting.
+        healpix_pixels = []
+        for shard_file_name in shard_file_list:
+            healpix_pixels.append(
+                get_healpix_pixel_from_metadata(pq.read_metadata(shard_file_name), "join_Norder", "join_Npix")
+            )
+
+        argsort = get_pixel_argsort(healpix_pixels)
+        shard_file_list = np.array(shard_file_list)[argsort]
+
+        shards = []
+        for shard_file_name in shard_file_list:
+            shards.append(pq.read_table(shard_file_name))
+
+        # Write all of the shards into a single parquet file, one row-group-per-shard.
+        starting_catalog_path = FilePointer(str(soap_args.catalog_path))
+        destination_dir = paths.pixel_directory(starting_catalog_path, object_pixel.order, object_pixel.pixel)
+        file_io.make_directory(
+            destination_dir, exist_ok=True, storage_options=soap_args.output_storage_options
         )
 
-    argsort = get_pixel_argsort(healpix_pixels)
-    shard_file_list = np.array(shard_file_list)[argsort]
-
-    shards = []
-    for shard_file_name in shard_file_list:
-        shards.append(pq.read_table(shard_file_name))
-
-    # Write all of the shards into a single parquet file, one row-group-per-shard.
-    starting_catalog_path = FilePointer(str(soap_args.catalog_path))
-    destination_dir = paths.pixel_directory(starting_catalog_path, object_pixel.order, object_pixel.pixel)
-    file_io.make_directory(destination_dir, exist_ok=True, storage_options=soap_args.output_storage_options)
-
-    output_file = paths.pixel_catalog_file(starting_catalog_path, object_pixel.order, object_pixel.pixel)
-    file_system, output_file = get_fs(
-        file_pointer=output_file, storage_options=soap_args.output_storage_options
-    )
-    output_file = strip_leading_slash_for_pyarrow(output_file, protocol=file_system.protocol)
-    with pq.ParquetWriter(output_file, shards[0].schema, filesystem=file_system) as writer:
-        for table in shards:
-            writer.write_table(table)
-
-    # Delete the intermediate shards.
-    if delete_input_files:
-        file_io.remove_directory(pixel_dir, ignore_errors=True)
-
-    SoapPlan.reducing_key_done(tmp_path=soap_args.tmp_path, reducing_key=object_key)
+        output_file = paths.pixel_catalog_file(starting_catalog_path, object_pixel.order, object_pixel.pixel)
+        file_system, output_file = get_fs(
+            file_pointer=output_file, storage_options=soap_args.output_storage_options
+        )
+        output_file = strip_leading_slash_for_pyarrow(output_file, protocol=file_system.protocol)
+        with pq.ParquetWriter(output_file, shards[0].schema, filesystem=file_system) as writer:
+            for table in shards:
+                writer.write_table(table)
+
+        # Delete the intermediate shards.
+        if delete_input_files:
+            file_io.remove_directory(pixel_dir, ignore_errors=True)
+
+        SoapPlan.reducing_key_done(tmp_path=soap_args.tmp_path, reducing_key=object_key)
+    except Exception as exception:  # pylint: disable=broad-exception-caught
+        print_task_failure(f"Failed REDUCING stage for shard: {object_pixel}", exception)
+        raise exception
```

### Comparing `hipscat_import-0.3.2/src/hipscat_import/soap/resume_plan.py` & `hipscat_import-0.3.3/src/hipscat_import/soap/resume_plan.py`

 * *Files 5% similar despite different names*

```diff
@@ -32,15 +32,20 @@
     COUNTING_STAGE = "counting"
     REDUCING_STAGE = "reducing"
     SOURCE_MAP_FILE = "source_object_map.npz"
 
     def __init__(self, args: SoapArguments):
         if not args.tmp_path:  # pragma: no cover (not reachable, but required for mypy)
             raise ValueError("tmp_path is required")
-        super().__init__(resume=args.resume, progress_bar=args.progress_bar, tmp_path=args.tmp_path)
+        super().__init__(
+            resume=args.resume,
+            progress_bar=args.progress_bar,
+            tmp_path=args.tmp_path,
+            delete_resume_log_files=args.delete_resume_log_files,
+        )
         self.gather_plan(args)
 
     def gather_plan(self, args):
         """Initialize the plan."""
         with tqdm(
             total=3, desc=self.get_formatted_stage_name("Planning"), disable=not self.progress_bar
         ) as step_progress:
```

### Comparing `hipscat_import-0.3.2/src/hipscat_import/soap/run_soap.py` & `hipscat_import-0.3.3/src/hipscat_import/soap/run_soap.py`

 * *Files 3% similar despite different names*

```diff
@@ -39,14 +39,15 @@
         for object_pixel, object_key in resume_plan.reduce_keys:
             futures.append(
                 client.submit(
                     reduce_joins,
                     soap_args=args,
                     object_pixel=object_pixel,
                     object_key=object_key,
+                    delete_input_files=args.delete_intermediate_parquet_files,
                 )
             )
 
         resume_plan.wait_for_reducing(futures)
 
     # All done - write out the metadata
     with tqdm(
```

### Comparing `hipscat_import-0.3.2/src/hipscat_import/verification/arguments.py` & `hipscat_import-0.3.3/src/hipscat_import/verification/arguments.py`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.2/src/hipscat_import/verification/run_verification.py` & `hipscat_import-0.3.3/src/hipscat_import/verification/run_verification.py`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.2/src/hipscat_import.egg-info/PKG-INFO` & `hipscat_import-0.3.3/src/hipscat_import.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hipscat-import
-Version: 0.3.2
+Version: 0.3.3
 Author-email: LINCC Frameworks <lincc-frameworks-team@lists.lsst.org>
 License: BSD 3-Clause License
         
         Copyright (c) 2023, LINCC Frameworks
         
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met:
@@ -38,21 +38,22 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: dask[complete]>=2024.3.0
 Requires-Dist: deprecated
 Requires-Dist: healpy
-Requires-Dist: hipscat>=0.3.0
+Requires-Dist: hipscat>=0.3.4
 Requires-Dist: ipykernel
+Requires-Dist: numpy
 Requires-Dist: pandas
 Requires-Dist: pyarrow
 Requires-Dist: pyyaml
+Requires-Dist: scipy
 Requires-Dist: tqdm
-Requires-Dist: numpy
 Provides-Extra: dev
 Requires-Dist: black; extra == "dev"
 Requires-Dist: jupyter; extra == "dev"
 Requires-Dist: mypy; extra == "dev"
 Requires-Dist: pre-commit; extra == "dev"
 Requires-Dist: pylint; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
```

### Comparing `hipscat_import-0.3.2/src/hipscat_import.egg-info/SOURCES.txt` & `hipscat_import-0.3.3/src/hipscat_import.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -73,14 +73,15 @@
 src/hipscat_import/index/arguments.py
 src/hipscat_import/index/map_reduce.py
 src/hipscat_import/index/run_index.py
 src/hipscat_import/margin_cache/__init__.py
 src/hipscat_import/margin_cache/margin_cache.py
 src/hipscat_import/margin_cache/margin_cache_arguments.py
 src/hipscat_import/margin_cache/margin_cache_map_reduce.py
+src/hipscat_import/margin_cache/margin_cache_resume_plan.py
 src/hipscat_import/soap/__init__.py
 src/hipscat_import/soap/arguments.py
 src/hipscat_import/soap/map_reduce.py
 src/hipscat_import/soap/resume_plan.py
 src/hipscat_import/soap/run_soap.py
 src/hipscat_import/verification/__init__.py
 src/hipscat_import/verification/arguments.py
@@ -208,14 +209,15 @@
 tests/hipscat_import/data/test_formats/small_sky.fits
 tests/hipscat_import/index/test_index_argument.py
 tests/hipscat_import/index/test_index_map_reduce.py
 tests/hipscat_import/index/test_run_index.py
 tests/hipscat_import/margin_cache/test_arguments_margin_cache.py
 tests/hipscat_import/margin_cache/test_margin_cache.py
 tests/hipscat_import/margin_cache/test_margin_cache_map_reduce.py
+tests/hipscat_import/margin_cache/test_margin_cache_resume_plan.py
 tests/hipscat_import/margin_cache/test_margin_round_trip.py
 tests/hipscat_import/soap/conftest.py
 tests/hipscat_import/soap/test_run_soap.py
 tests/hipscat_import/soap/test_soap_arguments.py
 tests/hipscat_import/soap/test_soap_map_reduce.py
 tests/hipscat_import/soap/test_soap_resume_plan.py
 tests/hipscat_import/verification/test_run_verification.py
```

### Comparing `hipscat_import-0.3.2/tests/.pylintrc` & `hipscat_import-0.3.3/tests/.pylintrc`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.2/tests/conftest.py` & `hipscat_import-0.3.3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.2/tests/hipscat_import/catalog/test_argument_validation.py` & `hipscat_import-0.3.3/tests/hipscat_import/catalog/test_argument_validation.py`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.2/tests/hipscat_import/catalog/test_file_readers.py` & `hipscat_import-0.3.3/tests/hipscat_import/catalog/test_file_readers.py`

 * *Files 4% similar despite different names*

```diff
@@ -216,20 +216,28 @@
         column_names=["letters", "ints", "empty", "numeric"],
         type_map={
             "letters": object,
             "ints": int,
             "empty": "Int64",
             "numeric": int,
         },
+        storage_options={"user_name": "user_pii", "user_key": "SECRETS!"},
     )
     provenance_info = reader.provenance_info()
-    catalog_base_dir = os.path.join(tmp_path, "test_catalog")
+    catalog_base_dir = tmp_path / "test_catalog"
     os.makedirs(catalog_base_dir)
     io.write_provenance_info(catalog_base_dir, basic_catalog_info, provenance_info)
 
+    with open(catalog_base_dir / "provenance_info.json", "r", encoding="utf-8") as file:
+        data = file.read()
+        assert "test_catalog" in data
+        assert "REDACTED" in data
+        assert "user_pii" not in data
+        assert "SECRETS" not in data
+
 
 def test_parquet_reader(parquet_shards_shard_44_0):
     """Verify we can read the parquet file into a single data frame."""
     total_chunks = 0
     for frame in ParquetReader().read(parquet_shards_shard_44_0):
         total_chunks += 1
         assert len(frame) == 7
@@ -251,14 +259,27 @@
     reader = ParquetReader(chunksize=1)
     provenance_info = reader.provenance_info()
     catalog_base_dir = os.path.join(tmp_path, "test_catalog")
     os.makedirs(catalog_base_dir)
     io.write_provenance_info(catalog_base_dir, basic_catalog_info, provenance_info)
 
 
+def test_parquet_reader_columns(parquet_shards_shard_44_0):
+    """Verify we can read a subset of columns."""
+    column_subset = ["id", "dec"]
+
+    # test column_names class property
+    for frame in ParquetReader(column_names=column_subset).read(parquet_shards_shard_44_0):
+        assert set(frame.columns) == set(column_subset)
+
+    # test read_columns kwarg
+    for frame in ParquetReader().read(parquet_shards_shard_44_0, read_columns=column_subset):
+        assert set(frame.columns) == set(column_subset)
+
+
 def test_read_fits(formats_fits):
     """Success case - fits file that exists being read as fits"""
     total_chunks = 0
     for frame in FitsReader().read(formats_fits):
         total_chunks += 1
         assert len(frame) == 131
```

### Comparing `hipscat_import-0.3.2/tests/hipscat_import/catalog/test_map_reduce.py` & `hipscat_import-0.3.3/tests/hipscat_import/catalog/test_map_reduce.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,26 +54,28 @@
             ra_column="ra",
             dec_column="dec",
             resume_path="",
             mapping_key="map_0",
         )
 
 
-def test_read_bad_fileformat(blank_data_file):
+def test_read_bad_fileformat(blank_data_file, capsys):
     """Unsupported file format"""
     with pytest.raises(NotImplementedError):
         mr.map_to_pixels(
             input_file=blank_data_file,
             file_reader=None,
             highest_order=0,
             ra_column="ra",
             dec_column="dec",
             resume_path="",
             mapping_key="map_0",
         )
+    captured = capsys.readouterr()
+    assert "No file reader implemented" in captured.out
 
 
 def read_partial_histogram(tmp_path, mapping_key):
     """Helper to read in the former result of a map operation."""
     histogram_file = os.path.join(tmp_path, "histograms", f"{mapping_key}.npz")
     hist = SparseHistogram.from_file(histogram_file)
     return hist.to_array()
@@ -242,14 +244,35 @@
     expected = hist.empty_histogram(1)
     filled_pixels = [5, 7, 11, 2]
     expected[44:] = filled_pixels[:]
     npt.assert_array_equal(result, expected)
     assert (result == expected).all()
 
 
+def test_split_pixels_bad_format(blank_data_file, tmp_path, capsys):
+    """Test loading the a file with non-default headers"""
+    alignment = np.full(12, None)
+    alignment[11] = (0, 11, 131)
+    with pytest.raises(NotImplementedError):
+        mr.split_pixels(
+            input_file=blank_data_file,
+            file_reader=None,
+            highest_order=0,
+            ra_column="ra_mean",
+            dec_column="dec_mean",
+            splitting_key="0",
+            cache_shard_path=tmp_path,
+            resume_path=tmp_path,
+            alignment=alignment,
+        )
+    captured = capsys.readouterr()
+    assert "No file reader implemented" in captured.out
+    os.makedirs(os.path.join(tmp_path, "splitting"))
+
+
 def test_split_pixels_headers(formats_headers_csv, assert_parquet_file_ids, tmp_path):
     """Test loading the a file with non-default headers"""
     os.makedirs(os.path.join(tmp_path, "splitting"))
     alignment = np.full(12, None)
     alignment[11] = (0, 11, 131)
     mr.split_pixels(
         input_file=formats_headers_csv,
```

### Comparing `hipscat_import-0.3.2/tests/hipscat_import/catalog/test_resume_plan.py` & `hipscat_import-0.3.3/tests/hipscat_import/catalog/test_resume_plan.py`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.2/tests/hipscat_import/catalog/test_run_import.py` & `hipscat_import-0.3.3/tests/hipscat_import/catalog/test_run_import.py`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.2/tests/hipscat_import/catalog/test_run_round_trip.py` & `hipscat_import-0.3.3/tests/hipscat_import/catalog/test_run_round_trip.py`

 * *Files 4% similar despite different names*

```diff
@@ -240,14 +240,93 @@
 
     data_frame = pd.read_parquet(output_file, engine="pyarrow")
     assert len(data_frame) == 14
     ids = data_frame["id"]
     assert np.logical_and(ids >= 700, ids < 832).all()
 
 
+def assert_directory_contains(dir_name, expected_contents):
+    assert os.path.exists(dir_name)
+    actual_contents = os.listdir(dir_name)
+    actual_contents.sort()
+    npt.assert_array_equal(actual_contents, expected_contents)
+
+
+@pytest.mark.dask
+def test_import_keep_intermediate_files(
+    dask_client,
+    small_sky_parts_dir,
+    tmp_path,
+):
+    """Test that ALL intermediate files are still around on-disk after
+    successful import, when setting the appropriate flags.
+    """
+    temp = os.path.join(tmp_path, "intermediate_files")
+    os.makedirs(temp)
+    args = ImportArguments(
+        output_artifact_name="small_sky_object_catalog",
+        input_path=small_sky_parts_dir,
+        file_reader="csv",
+        output_path=tmp_path,
+        tmp_dir=temp,
+        dask_tmp=temp,
+        progress_bar=False,
+        delete_intermediate_parquet_files=False,
+        delete_resume_log_files=False,
+    )
+
+    runner.run(args, dask_client)
+
+    # Check that the catalog metadata file exists
+    catalog = Catalog.read_from_hipscat(args.catalog_path)
+    assert catalog.on_disk
+    assert catalog.catalog_path == args.catalog_path
+
+    ## Check that stage-level done files are still around.
+    base_intermediate_dir = os.path.join(temp, "small_sky_object_catalog", "intermediate")
+    expected_contents = [
+        "histograms",  # directory containing sub-histograms
+        "input_paths.txt",  # original input paths for subsequent comparison
+        "mapping_done",  # stage-level done file
+        "mapping_histogram.npz",  # concatenated histogram file
+        "order_0",  # all intermediate parquet files
+        "reducing",  # directory containing task-level done files
+        "reducing_done",  # stage-level done file
+        "splitting",  # directory containing task-level done files
+        "splitting_done",  # stage-level done file
+    ]
+    assert_directory_contains(base_intermediate_dir, expected_contents)
+
+    checking_dir = os.path.join(base_intermediate_dir, "histograms")
+    assert_directory_contains(
+        checking_dir, ["map_0.npz", "map_1.npz", "map_2.npz", "map_3.npz", "map_4.npz", "map_5.npz"]
+    )
+    checking_dir = os.path.join(base_intermediate_dir, "splitting")
+    assert_directory_contains(
+        checking_dir,
+        ["split_0_done", "split_1_done", "split_2_done", "split_3_done", "split_4_done", "split_5_done"],
+    )
+
+    checking_dir = os.path.join(base_intermediate_dir, "reducing")
+    assert_directory_contains(checking_dir, ["0_11_done"])
+
+    # Check that all of the intermediate parquet shards are still around.
+    checking_dir = os.path.join(base_intermediate_dir, "order_0", "dir_0", "pixel_11")
+    assert_directory_contains(
+        checking_dir,
+        [
+            "shard_split_0_0.parquet",
+            "shard_split_1_0.parquet",
+            "shard_split_2_0.parquet",
+            "shard_split_3_0.parquet",
+            "shard_split_4_0.parquet",
+        ],
+    )
+
+
 @pytest.mark.dask
 def test_import_lowest_healpix_order(
     dask_client,
     small_sky_parts_dir,
     tmp_path,
 ):
     """Test basic execution.
```

### Comparing `hipscat_import-0.3.2/tests/hipscat_import/catalog/test_sparse_histogram.py` & `hipscat_import-0.3.3/tests/hipscat_import/catalog/test_sparse_histogram.py`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.2/tests/hipscat_import/conftest.py` & `hipscat_import-0.3.3/tests/hipscat_import/conftest.py`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.2/tests/hipscat_import/data/mixed_schema/schema.parquet` & `hipscat_import-0.3.3/tests/hipscat_import/data/mixed_schema/schema.parquet`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.2/tests/hipscat_import/data/parquet_shards/order_0/dir_0/pixel_11/shard_0_0.parquet` & `hipscat_import-0.3.3/tests/hipscat_import/data/parquet_shards/order_0/dir_0/pixel_11/shard_0_0.parquet`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.2/tests/hipscat_import/data/parquet_shards/order_0/dir_0/pixel_11/shard_1_0.parquet` & `hipscat_import-0.3.3/tests/hipscat_import/data/parquet_shards/order_0/dir_0/pixel_11/shard_1_0.parquet`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.2/tests/hipscat_import/data/parquet_shards/order_0/dir_0/pixel_11/shard_2_0.parquet` & `hipscat_import-0.3.3/tests/hipscat_import/data/parquet_shards/order_0/dir_0/pixel_11/shard_2_0.parquet`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.2/tests/hipscat_import/data/parquet_shards/order_0/dir_0/pixel_11/shard_3_0.parquet` & `hipscat_import-0.3.3/tests/hipscat_import/data/parquet_shards/order_0/dir_0/pixel_11/shard_3_0.parquet`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.2/tests/hipscat_import/data/parquet_shards/order_0/dir_0/pixel_11/shard_4_0.parquet` & `hipscat_import-0.3.3/tests/hipscat_import/data/parquet_shards/order_0/dir_0/pixel_11/shard_4_0.parquet`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.2/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_44/shard_0_0.parquet` & `hipscat_import-0.3.3/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_44/shard_0_0.parquet`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.2/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_44/shard_1_0.parquet` & `hipscat_import-0.3.3/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_44/shard_1_0.parquet`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.2/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_44/shard_2_0.parquet` & `hipscat_import-0.3.3/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_44/shard_2_0.parquet`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.2/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_44/shard_3_0.parquet` & `hipscat_import-0.3.3/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_44/shard_3_0.parquet`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.2/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_44/shard_4_0.parquet` & `hipscat_import-0.3.3/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_44/shard_4_0.parquet`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.2/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_45/shard_0_0.parquet` & `hipscat_import-0.3.3/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_45/shard_0_0.parquet`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.2/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_45/shard_1_0.parquet` & `hipscat_import-0.3.3/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_45/shard_1_0.parquet`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.2/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_45/shard_2_0.parquet` & `hipscat_import-0.3.3/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_45/shard_2_0.parquet`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.2/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_45/shard_3_0.parquet` & `hipscat_import-0.3.3/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_45/shard_3_0.parquet`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.2/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_45/shard_4_0.parquet` & `hipscat_import-0.3.3/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_45/shard_4_0.parquet`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.2/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_46/shard_0_0.parquet` & `hipscat_import-0.3.3/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_46/shard_0_0.parquet`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.2/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_46/shard_1_0.parquet` & `hipscat_import-0.3.3/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_46/shard_1_0.parquet`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.2/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_46/shard_2_0.parquet` & `hipscat_import-0.3.3/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_46/shard_2_0.parquet`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.2/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_46/shard_3_0.parquet` & `hipscat_import-0.3.3/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_46/shard_3_0.parquet`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.2/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_46/shard_4_0.parquet` & `hipscat_import-0.3.3/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_46/shard_4_0.parquet`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.2/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_47/shard_0_0.parquet` & `hipscat_import-0.3.3/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_47/shard_0_0.parquet`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.2/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_47/shard_1_0.parquet` & `hipscat_import-0.3.3/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_47/shard_1_0.parquet`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.2/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_47/shard_2_0.parquet` & `hipscat_import-0.3.3/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_47/shard_2_0.parquet`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.2/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_47/shard_3_0.parquet` & `hipscat_import-0.3.3/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_47/shard_3_0.parquet`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.2/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_47/shard_4_0.parquet` & `hipscat_import-0.3.3/tests/hipscat_import/data/parquet_shards/order_1/dir_0/pixel_47/shard_4_0.parquet`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.2/tests/hipscat_import/data/resume/Norder=0/Dir=0/Npix=11.parquet` & `hipscat_import-0.3.3/tests/hipscat_import/data/resume/Norder=0/Dir=0/Npix=11.parquet`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.2/tests/hipscat_import/data/resume/Norder=1/Dir=0/Npix=44.parquet` & `hipscat_import-0.3.3/tests/hipscat_import/data/resume/Norder=1/Dir=0/Npix=44.parquet`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.2/tests/hipscat_import/data/resume/Norder=1/Dir=0/Npix=45.parquet` & `hipscat_import-0.3.3/tests/hipscat_import/data/resume/Norder=1/Dir=0/Npix=45.parquet`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.2/tests/hipscat_import/data/resume/Norder=1/Dir=0/Npix=46.parquet` & `hipscat_import-0.3.3/tests/hipscat_import/data/resume/Norder=1/Dir=0/Npix=46.parquet`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.2/tests/hipscat_import/data/resume/Norder=1/Dir=0/Npix=47.parquet` & `hipscat_import-0.3.3/tests/hipscat_import/data/resume/Norder=1/Dir=0/Npix=47.parquet`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.2/tests/hipscat_import/data/small_sky/catalog.csv` & `hipscat_import-0.3.3/tests/hipscat_import/data/small_sky/catalog.csv`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.2/tests/hipscat_import/data/small_sky_object_catalog/Norder=0/Dir=0/Npix=11.parquet` & `hipscat_import-0.3.3/tests/hipscat_import/data/small_sky_object_catalog/Norder=0/Dir=0/Npix=11.parquet`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.2/tests/hipscat_import/data/small_sky_object_catalog/_common_metadata` & `hipscat_import-0.3.3/tests/hipscat_import/data/small_sky_object_catalog/_common_metadata`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.2/tests/hipscat_import/data/small_sky_object_catalog/_metadata` & `hipscat_import-0.3.3/tests/hipscat_import/data/small_sky_object_catalog/_metadata`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.2/tests/hipscat_import/data/small_sky_object_catalog/point_map.fits` & `hipscat_import-0.3.3/tests/hipscat_import/data/small_sky_object_catalog/point_map.fits`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.2/tests/hipscat_import/data/small_sky_object_catalog/provenance_info.json` & `hipscat_import-0.3.3/tests/hipscat_import/data/small_sky_object_catalog/provenance_info.json`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.2/tests/hipscat_import/data/small_sky_parts/catalog_00_of_05.csv` & `hipscat_import-0.3.3/tests/hipscat_import/data/small_sky_parts/catalog_00_of_05.csv`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.2/tests/hipscat_import/data/small_sky_parts/catalog_01_of_05.csv` & `hipscat_import-0.3.3/tests/hipscat_import/data/small_sky_parts/catalog_01_of_05.csv`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.2/tests/hipscat_import/data/small_sky_parts/catalog_02_of_05.csv` & `hipscat_import-0.3.3/tests/hipscat_import/data/small_sky_parts/catalog_02_of_05.csv`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.2/tests/hipscat_import/data/small_sky_parts/catalog_03_of_05.csv` & `hipscat_import-0.3.3/tests/hipscat_import/data/small_sky_parts/catalog_03_of_05.csv`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.2/tests/hipscat_import/data/small_sky_parts/catalog_04_of_05.csv` & `hipscat_import-0.3.3/tests/hipscat_import/data/small_sky_parts/catalog_04_of_05.csv`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.2/tests/hipscat_import/data/small_sky_source/small_sky_source.csv` & `hipscat_import-0.3.3/tests/hipscat_import/data/small_sky_source/small_sky_source.csv`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.2/tests/hipscat_import/data/small_sky_source_catalog/Norder=0/Dir=0/Npix=4.parquet` & `hipscat_import-0.3.3/tests/hipscat_import/data/small_sky_source_catalog/Norder=0/Dir=0/Npix=4.parquet`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.2/tests/hipscat_import/data/small_sky_source_catalog/Norder=1/Dir=0/Npix=47.parquet` & `hipscat_import-0.3.3/tests/hipscat_import/data/small_sky_source_catalog/Norder=1/Dir=0/Npix=47.parquet`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.2/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=176.parquet` & `hipscat_import-0.3.3/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=176.parquet`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.2/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=177.parquet` & `hipscat_import-0.3.3/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=177.parquet`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.2/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=178.parquet` & `hipscat_import-0.3.3/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=178.parquet`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.2/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=179.parquet` & `hipscat_import-0.3.3/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=179.parquet`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.2/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=180.parquet` & `hipscat_import-0.3.3/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=180.parquet`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.2/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=181.parquet` & `hipscat_import-0.3.3/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=181.parquet`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.2/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=182.parquet` & `hipscat_import-0.3.3/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=182.parquet`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.2/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=183.parquet` & `hipscat_import-0.3.3/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=183.parquet`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.2/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=184.parquet` & `hipscat_import-0.3.3/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=184.parquet`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.2/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=185.parquet` & `hipscat_import-0.3.3/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=185.parquet`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.2/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=186.parquet` & `hipscat_import-0.3.3/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=186.parquet`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.2/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=187.parquet` & `hipscat_import-0.3.3/tests/hipscat_import/data/small_sky_source_catalog/Norder=2/Dir=0/Npix=187.parquet`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.2/tests/hipscat_import/data/small_sky_source_catalog/_common_metadata` & `hipscat_import-0.3.3/tests/hipscat_import/data/small_sky_source_catalog/_common_metadata`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.2/tests/hipscat_import/data/small_sky_source_catalog/_metadata` & `hipscat_import-0.3.3/tests/hipscat_import/data/small_sky_source_catalog/_metadata`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.2/tests/hipscat_import/data/small_sky_source_catalog/point_map.fits` & `hipscat_import-0.3.3/tests/hipscat_import/data/small_sky_source_catalog/point_map.fits`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.2/tests/hipscat_import/data/small_sky_source_catalog/provenance_info.json` & `hipscat_import-0.3.3/tests/hipscat_import/data/small_sky_source_catalog/provenance_info.json`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.2/tests/hipscat_import/data/soap_intermediate/order_0/dir_0/pixel_11/source_0_4.parquet` & `hipscat_import-0.3.3/tests/hipscat_import/data/soap_intermediate/order_0/dir_0/pixel_11/source_0_4.parquet`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.2/tests/hipscat_import/data/soap_intermediate/order_0/dir_0/pixel_11/source_1_47.parquet` & `hipscat_import-0.3.3/tests/hipscat_import/data/soap_intermediate/order_0/dir_0/pixel_11/source_1_47.parquet`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.2/tests/hipscat_import/data/soap_intermediate/order_0/dir_0/pixel_11/source_2_176.parquet` & `hipscat_import-0.3.3/tests/hipscat_import/data/soap_intermediate/order_0/dir_0/pixel_11/source_2_176.parquet`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.2/tests/hipscat_import/data/soap_intermediate/order_0/dir_0/pixel_11/source_2_177.parquet` & `hipscat_import-0.3.3/tests/hipscat_import/data/soap_intermediate/order_0/dir_0/pixel_11/source_2_177.parquet`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.2/tests/hipscat_import/data/soap_intermediate/order_0/dir_0/pixel_11/source_2_178.parquet` & `hipscat_import-0.3.3/tests/hipscat_import/data/soap_intermediate/order_0/dir_0/pixel_11/source_2_178.parquet`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.2/tests/hipscat_import/data/soap_intermediate/order_0/dir_0/pixel_11/source_2_179.parquet` & `hipscat_import-0.3.3/tests/hipscat_import/data/soap_intermediate/order_0/dir_0/pixel_11/source_2_179.parquet`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.2/tests/hipscat_import/data/soap_intermediate/order_0/dir_0/pixel_11/source_2_180.parquet` & `hipscat_import-0.3.3/tests/hipscat_import/data/soap_intermediate/order_0/dir_0/pixel_11/source_2_180.parquet`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.2/tests/hipscat_import/data/soap_intermediate/order_0/dir_0/pixel_11/source_2_181.parquet` & `hipscat_import-0.3.3/tests/hipscat_import/data/soap_intermediate/order_0/dir_0/pixel_11/source_2_181.parquet`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.2/tests/hipscat_import/data/soap_intermediate/order_0/dir_0/pixel_11/source_2_182.parquet` & `hipscat_import-0.3.3/tests/hipscat_import/data/soap_intermediate/order_0/dir_0/pixel_11/source_2_182.parquet`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.2/tests/hipscat_import/data/soap_intermediate/order_0/dir_0/pixel_11/source_2_183.parquet` & `hipscat_import-0.3.3/tests/hipscat_import/data/soap_intermediate/order_0/dir_0/pixel_11/source_2_183.parquet`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.2/tests/hipscat_import/data/soap_intermediate/order_0/dir_0/pixel_11/source_2_184.parquet` & `hipscat_import-0.3.3/tests/hipscat_import/data/soap_intermediate/order_0/dir_0/pixel_11/source_2_184.parquet`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.2/tests/hipscat_import/data/soap_intermediate/order_0/dir_0/pixel_11/source_2_185.parquet` & `hipscat_import-0.3.3/tests/hipscat_import/data/soap_intermediate/order_0/dir_0/pixel_11/source_2_185.parquet`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.2/tests/hipscat_import/data/soap_intermediate/order_0/dir_0/pixel_11/source_2_186.parquet` & `hipscat_import-0.3.3/tests/hipscat_import/data/soap_intermediate/order_0/dir_0/pixel_11/source_2_186.parquet`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.2/tests/hipscat_import/data/soap_intermediate/order_0/dir_0/pixel_11/source_2_187.parquet` & `hipscat_import-0.3.3/tests/hipscat_import/data/soap_intermediate/order_0/dir_0/pixel_11/source_2_187.parquet`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.2/tests/hipscat_import/data/test_formats/catalog.starr` & `hipscat_import-0.3.3/tests/hipscat_import/data/test_formats/catalog.starr`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.2/tests/hipscat_import/data/test_formats/gaia_epoch.ecsv` & `hipscat_import-0.3.3/tests/hipscat_import/data/test_formats/gaia_epoch.ecsv`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.2/tests/hipscat_import/data/test_formats/gaia_minimum.csv` & `hipscat_import-0.3.3/tests/hipscat_import/data/test_formats/gaia_minimum.csv`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.2/tests/hipscat_import/data/test_formats/gaia_minimum_schema.parquet` & `hipscat_import-0.3.3/tests/hipscat_import/data/test_formats/gaia_minimum_schema.parquet`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.2/tests/hipscat_import/data/test_formats/hipscat_index.csv` & `hipscat_import-0.3.3/tests/hipscat_import/data/test_formats/hipscat_index.csv`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.2/tests/hipscat_import/data/test_formats/hipscat_index.parquet` & `hipscat_import-0.3.3/tests/hipscat_import/data/test_formats/hipscat_index.parquet`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.2/tests/hipscat_import/data/test_formats/pandasindex.parquet` & `hipscat_import-0.3.3/tests/hipscat_import/data/test_formats/pandasindex.parquet`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.2/tests/hipscat_import/data/test_formats/small_sky.fits` & `hipscat_import-0.3.3/tests/hipscat_import/data/test_formats/small_sky.fits`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.2/tests/hipscat_import/index/test_index_argument.py` & `hipscat_import-0.3.3/tests/hipscat_import/index/test_index_argument.py`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.2/tests/hipscat_import/index/test_index_map_reduce.py` & `hipscat_import-0.3.3/tests/hipscat_import/index/test_index_map_reduce.py`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.2/tests/hipscat_import/index/test_run_index.py` & `hipscat_import-0.3.3/tests/hipscat_import/index/test_run_index.py`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.2/tests/hipscat_import/margin_cache/test_arguments_margin_cache.py` & `hipscat_import-0.3.3/tests/hipscat_import/margin_cache/test_arguments_margin_cache.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Tests of margin cache generation arguments"""
 
 import pytest
+from hipscat.io import write_metadata
+from hipscat.pixel_math.healpix_pixel import HealpixPixel
 
 from hipscat_import.margin_cache.margin_cache_arguments import MarginCacheArguments
 
-# pylint: disable=protected-access
-
 
 def test_empty_required(tmp_path):
     """*Most* required arguments are provided."""
     ## Input catalog path is missing
     with pytest.raises(ValueError, match="input_catalog_path"):
         MarginCacheArguments(
             margin_threshold=5.0,
@@ -60,14 +60,50 @@
             input_catalog_path=small_sky_source_catalog,
             output_path=tmp_path,
             output_artifact_name="catalog_cache",
             margin_order=2,
         )
 
 
+def test_debug_filter_pixel_list(small_sky_source_catalog, tmp_path):
+    """Ensure we can generate catalog with a filtereed list of pixels, and
+    that we raise an exception when the filter results in an empty catalog."""
+    args = MarginCacheArguments(
+        margin_threshold=5.0,
+        input_catalog_path=small_sky_source_catalog,
+        output_path=tmp_path,
+        output_artifact_name="catalog_cache",
+        margin_order=4,
+        debug_filter_pixel_list=[HealpixPixel(0, 11)],
+    )
+
+    assert len(args.catalog.get_healpix_pixels()) == 13
+
+    args = MarginCacheArguments(
+        margin_threshold=5.0,
+        input_catalog_path=small_sky_source_catalog,
+        output_path=tmp_path,
+        output_artifact_name="catalog_cache",
+        margin_order=4,
+        debug_filter_pixel_list=[HealpixPixel(1, 44)],
+    )
+
+    assert len(args.catalog.get_healpix_pixels()) == 4
+
+    with pytest.raises(ValueError, match="debug_filter_pixel_list"):
+        MarginCacheArguments(
+            margin_threshold=5.0,
+            input_catalog_path=small_sky_source_catalog,
+            output_path=tmp_path,
+            output_artifact_name="catalog_cache",
+            margin_order=4,
+            debug_filter_pixel_list=[HealpixPixel(0, 5)],
+        )
+
+
 def test_margin_threshold_warns(small_sky_source_catalog, tmp_path):
     """Ensure we give a warning when margin_threshold is greater than margin_order resolution"""
 
     with pytest.warns(UserWarning, match="margin_threshold"):
         MarginCacheArguments(
             margin_threshold=360.0,
             input_catalog_path=small_sky_source_catalog,
@@ -95,11 +131,16 @@
     """Verify that provenance info includes margin-cache-specific fields."""
     args = MarginCacheArguments(
         margin_threshold=5.0,
         input_catalog_path=small_sky_source_catalog,
         output_path=tmp_path,
         output_artifact_name="catalog_cache",
         margin_order=4,
+        debug_filter_pixel_list=[HealpixPixel(1, 44)],
     )
 
     runtime_args = args.provenance_info()["runtime_args"]
     assert "margin_threshold" in runtime_args
+
+    write_metadata.write_provenance_info(
+        catalog_base_dir=args.catalog_path, dataset_info=args.to_catalog_info(20_000), tool_args=runtime_args
+    )
```

### Comparing `hipscat_import-0.3.2/tests/hipscat_import/margin_cache/test_margin_cache.py` & `hipscat_import-0.3.3/tests/hipscat_import/margin_cache/test_margin_cache_resume_plan.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,164 +1,129 @@
-"""Tests of map reduce operations"""
-
 import numpy as np
 import numpy.testing as npt
-import pandas as pd
 import pytest
-from hipscat.catalog import PartitionInfo
-from hipscat.catalog.healpix_dataset.healpix_dataset import HealpixDataset
-from hipscat.io import file_io, paths
+from hipscat.catalog import Catalog
 
-import hipscat_import.margin_cache.margin_cache as mc
 from hipscat_import.margin_cache.margin_cache_arguments import MarginCacheArguments
+from hipscat_import.margin_cache.margin_cache_resume_plan import (
+    MarginCachePlan,
+    _find_partition_margin_pixel_pairs,
+)
 
 # pylint: disable=protected-access
 
 
-@pytest.mark.dask(timeout=150)
-def test_margin_cache_gen(small_sky_source_catalog, tmp_path, dask_client):
-    """Test that margin cache generation works end to end."""
-    args = MarginCacheArguments(
-        margin_threshold=180.0,
-        input_catalog_path=small_sky_source_catalog,
+@pytest.fixture
+def small_sky_margin_args(tmp_path, small_sky_object_catalog):
+    return MarginCacheArguments(
+        margin_threshold=5.0,
+        input_catalog_path=small_sky_object_catalog,
         output_path=tmp_path,
         output_artifact_name="catalog_cache",
-        margin_order=8,
         progress_bar=False,
+        resume=True,
     )
 
-    assert args.catalog.catalog_info.ra_column == "source_ra"
 
-    mc.generate_margin_cache(args, dask_client)
+def test_done_checks(small_sky_margin_args):
+    """Verify that done files imply correct pipeline execution order:
+    mapping > reducing
+    """
+    plan = MarginCachePlan(small_sky_margin_args)
+    plan.touch_stage_done_file(MarginCachePlan.REDUCING_STAGE)
 
-    norder = 1
-    npix = 47
+    with pytest.raises(ValueError, match="before reducing"):
+        plan._gather_plan(small_sky_margin_args)
 
-    test_file = paths.pixel_catalog_file(args.catalog_path, norder, npix)
+    plan.touch_stage_done_file(MarginCachePlan.MAPPING_STAGE)
+    plan._gather_plan(small_sky_margin_args)
+    assert plan.is_mapping_done()
+    assert plan.is_reducing_done()
 
-    data = pd.read_parquet(test_file)
-
-    assert len(data) == 13
-
-    assert all(data[PartitionInfo.METADATA_ORDER_COLUMN_NAME] == norder)
-    assert all(data[PartitionInfo.METADATA_PIXEL_COLUMN_NAME] == npix)
-    assert all(data[PartitionInfo.METADATA_DIR_COLUMN_NAME] == int(npix / 10000) * 10000)
-
-    assert data.dtypes[PartitionInfo.METADATA_ORDER_COLUMN_NAME] == np.uint8
-    assert data.dtypes[PartitionInfo.METADATA_DIR_COLUMN_NAME] == np.uint64
-    assert data.dtypes[PartitionInfo.METADATA_PIXEL_COLUMN_NAME] == np.uint64
-
-    npt.assert_array_equal(
-        data.columns,
-        [
-            "source_id",
-            "source_ra",
-            "source_dec",
-            "mjd",
-            "mag",
-            "band",
-            "object_id",
-            "object_ra",
-            "object_dec",
-            "Norder",
-            "Dir",
-            "Npix",
-            "margin_Norder",
-            "margin_Dir",
-            "margin_Npix",
-        ],
-    )
-    assert data.index.name == "_hipscat_index"
+    plan.clean_resume_files()
 
-    catalog = HealpixDataset.read_from_hipscat(args.catalog_path)
-    assert catalog.on_disk
-    assert catalog.catalog_path == args.catalog_path
+    plan = MarginCachePlan(small_sky_margin_args)
+    plan.touch_stage_done_file(MarginCachePlan.MAPPING_STAGE)
+    plan._gather_plan(small_sky_margin_args)
 
+    assert plan.is_mapping_done()
+    assert not plan.is_reducing_done()
 
-@pytest.mark.dask(timeout=150)
-def test_margin_cache_gen_negative_pixels(small_sky_source_catalog, tmp_path, dask_client):
-    """Test that margin cache generation can generate a file for a negative pixel."""
-    with pytest.warns(UserWarning, match="smaller resolution"):
-        args = MarginCacheArguments(
-            margin_threshold=36000.0,
-            input_catalog_path=small_sky_source_catalog,
-            output_path=tmp_path,
-            output_artifact_name="catalog_cache",
-            margin_order=4,
-            progress_bar=False,
-        )
 
-    assert args.catalog.catalog_info.ra_column == "source_ra"
+def never_fails():
+    """Method never fails, but never marks intermediate success file."""
+    return
 
-    mc.generate_margin_cache(args, dask_client)
 
-    norder = 0
-    npix = 7
+@pytest.mark.dask
+def test_some_map_task_failures(small_sky_margin_args, dask_client):
+    """Test that we only consider map stage successful if all done files are written"""
+    plan = MarginCachePlan(small_sky_margin_args)
 
-    negative_test_file = paths.pixel_catalog_file(args.catalog_path, norder, npix)
+    ## Method doesn't FAIL, but it doesn't write out the done file either.
+    ## Since the intermediate files aren't found, we throw an error.
+    futures = [dask_client.submit(never_fails)]
+    with pytest.raises(RuntimeError, match="1 mapping stages"):
+        plan.wait_for_mapping(futures)
 
-    negative_data = pd.read_parquet(negative_test_file)
+    MarginCachePlan.touch_key_done_file(plan.tmp_path, MarginCachePlan.MAPPING_STAGE, "0_11")
 
-    assert len(negative_data) > 0
+    ## Method succeeds, *and* done files are present.
+    futures = [dask_client.submit(never_fails)]
+    plan.wait_for_mapping(futures)
 
 
-def test_partition_margin_pixel_pairs(small_sky_source_catalog, tmp_path):
-    """Ensure partition_margin_pixel_pairs can generate main partition pixels."""
-    args = MarginCacheArguments(
-        margin_threshold=5.0,
-        input_catalog_path=small_sky_source_catalog,
-        output_path=tmp_path,
-        output_artifact_name="catalog_cache",
-    )
+@pytest.mark.dask
+def test_some_reducing_task_failures(small_sky_margin_args, dask_client):
+    """Test that we only consider reduce stage successful if all done files are written"""
+    plan = MarginCachePlan(small_sky_margin_args)
 
-    margin_pairs = mc._find_partition_margin_pixel_pairs(
-        args.catalog.partition_info.get_healpix_pixels(), args.margin_order
-    )
+    ## Method doesn't FAIL, but it doesn't write out the done file either.
+    ## Since the intermediate files aren't found, we throw an error.
+    futures = [dask_client.submit(never_fails)]
+    with pytest.raises(RuntimeError, match="12 reducing stages"):
+        plan.wait_for_reducing(futures)
+
+    MarginCachePlan.touch_key_done_file(plan.tmp_path, MarginCachePlan.REDUCING_STAGE, "0_11")
+
+    ## Method succeeds, but only *ONE* done file is present.
+    futures = [dask_client.submit(never_fails)]
+    with pytest.raises(RuntimeError, match="11 reducing stages"):
+        plan.wait_for_reducing(futures)
+
+    for partition in range(0, 12):
+        MarginCachePlan.touch_key_done_file(plan.tmp_path, MarginCachePlan.REDUCING_STAGE, f"0_{partition}")
+
+    ## Method succeeds, *and* done files are present.
+    futures = [dask_client.submit(never_fails)]
+    plan.wait_for_reducing(futures)
+
+
+def test_partition_margin_pixel_pairs(small_sky_source_catalog):
+    """Ensure partition_margin_pixel_pairs can generate main partition pixels."""
+    source_catalog = Catalog.read_from_hipscat(small_sky_source_catalog)
+    margin_pairs = _find_partition_margin_pixel_pairs(source_catalog.get_healpix_pixels(), 3)
 
     expected = np.array([725, 733, 757, 765, 727, 735, 759, 767, 469, 192])
 
     npt.assert_array_equal(margin_pairs.iloc[:10]["margin_pixel"], expected)
     assert len(margin_pairs) == 196
 
 
-def test_partition_margin_pixel_pairs_negative(small_sky_source_catalog, tmp_path):
+def test_partition_margin_pixel_pairs_negative(small_sky_source_catalog):
     """Ensure partition_margin_pixel_pairs can generate negative tree pixels."""
-    args = MarginCacheArguments(
-        margin_threshold=5.0,
-        input_catalog_path=small_sky_source_catalog,
-        output_path=tmp_path,
-        output_artifact_name="catalog_cache",
-    )
+    source_catalog = Catalog.read_from_hipscat(small_sky_source_catalog)
 
-    partition_stats = args.catalog.partition_info.get_healpix_pixels()
-    negative_pixels = args.catalog.generate_negative_tree_pixels()
+    partition_stats = source_catalog.get_healpix_pixels()
+    negative_pixels = source_catalog.generate_negative_tree_pixels()
     combined_pixels = partition_stats + negative_pixels
 
-    margin_pairs = mc._find_partition_margin_pixel_pairs(combined_pixels, args.margin_order)
+    margin_pairs = _find_partition_margin_pixel_pairs(combined_pixels, 3)
 
     expected_order = 0
     expected_pixel = 10
     expected = np.array([490, 704, 712, 736, 744, 706, 714, 738, 746, 512])
 
     assert margin_pairs.iloc[-1]["partition_order"] == expected_order
     assert margin_pairs.iloc[-1]["partition_pixel"] == expected_pixel
     npt.assert_array_equal(margin_pairs.iloc[-10:]["margin_pixel"], expected)
     assert len(margin_pairs) == 536
-
-
-def test_create_margin_directory(small_sky_source_catalog, tmp_path):
-    """Ensure create_margin_directory works on main partition_pixels"""
-    args = MarginCacheArguments(
-        margin_threshold=5.0,
-        input_catalog_path=small_sky_source_catalog,
-        output_path=tmp_path,
-        output_artifact_name="catalog_cache",
-    )
-
-    mc._create_margin_directory(
-        stats=args.catalog.partition_info.get_healpix_pixels(),
-        output_path=args.catalog_path,
-        storage_options=None,
-    )
-
-    output = file_io.append_paths_to_pointer(args.catalog_path, "Norder=0", "Dir=0")
-    assert file_io.does_file_or_directory_exist(output)
```

### Comparing `hipscat_import-0.3.2/tests/hipscat_import/margin_cache/test_margin_cache_map_reduce.py` & `hipscat_import-0.3.3/tests/hipscat_import/margin_cache/test_margin_cache_map_reduce.py`

 * *Files 27% similar despite different names*

```diff
@@ -66,21 +66,42 @@
     path = os.path.join(tmp_path, "order_2", "dir_0", "pixel_15", "Norder=2", "Dir=0", "Npix=0.parquet")
 
     assert os.path.exists(path)
 
     validate_result_dataframe(path, 360)
 
 
-@pytest.mark.dask
-def test_reduce_margin_shards(tmp_path, basic_data_shard_df):
+def test_map_pixel_shards_error(tmp_path, capsys):
+    """Test error behavior on reduce stage. e.g. by not creating the original
+    catalog parquet files."""
+    with pytest.raises(FileNotFoundError):
+        margin_cache_map_reduce.map_pixel_shards(
+            paths.pixel_catalog_file(tmp_path, 1, 0),
+            mapping_key="1_21",
+            input_storage_options=None,
+            original_catalog_metadata="",
+            margin_pair_file="",
+            margin_threshold=10,
+            output_path=tmp_path,
+            margin_order=4,
+            ra_column="ra",
+            dec_column="dec",
+        )
+
+    captured = capsys.readouterr()
+    assert "No such file or directory" in captured.out
+
+
+def test_reduce_margin_shards(tmp_path):
     intermediate_dir = os.path.join(tmp_path, "intermediate")
     partition_dir = get_pixel_cache_directory(intermediate_dir, HealpixPixel(1, 21))
     shard_dir = paths.pixel_directory(partition_dir, 1, 21)
 
     os.makedirs(shard_dir)
+    os.makedirs(os.path.join(intermediate_dir, "reducing"))
 
     first_shard_path = paths.pixel_catalog_file(partition_dir, 1, 0)
     second_shard_path = paths.pixel_catalog_file(partition_dir, 1, 1)
 
     ras = np.arange(0.0, 360.0)
     dec = np.full(360, 0.0)
     norder = np.full(360, 1)
@@ -114,19 +135,71 @@
     basic_data_shard_df = test_df
 
     basic_data_shard_df.to_parquet(first_shard_path)
     basic_data_shard_df.to_parquet(second_shard_path)
 
     margin_cache_map_reduce.reduce_margin_shards(
         intermediate_dir,
+        "1_21",
+        tmp_path,
+        None,
+        1,
+        21,
+        original_catalog_metadata=schema_path,
+        delete_intermediate_parquet_files=False,
+        input_storage_options=None,
+    )
+
+    result_path = paths.pixel_catalog_file(tmp_path, 1, 21)
+
+    validate_result_dataframe(result_path, 720)
+    assert os.path.exists(shard_dir)
+
+    # Run again with delete_intermediate_parquet_files. shard_dir doesn't exist at the end.
+    margin_cache_map_reduce.reduce_margin_shards(
+        intermediate_dir,
+        "1_21",
         tmp_path,
         None,
         1,
         21,
         original_catalog_metadata=schema_path,
+        delete_intermediate_parquet_files=True,
         input_storage_options=None,
     )
 
     result_path = paths.pixel_catalog_file(tmp_path, 1, 21)
 
     validate_result_dataframe(result_path, 720)
     assert not os.path.exists(shard_dir)
+
+
+def test_reduce_margin_shards_error(tmp_path, basic_data_shard_df, capsys):
+    """Test error behavior on reduce stage. e.g. by not creating the original
+    catalog metadata."""
+    intermediate_dir = os.path.join(tmp_path, "intermediate")
+    partition_dir = get_pixel_cache_directory(intermediate_dir, HealpixPixel(1, 21))
+    shard_dir = paths.pixel_directory(partition_dir, 1, 21)
+    os.makedirs(shard_dir)
+    os.makedirs(os.path.join(intermediate_dir, "reducing"))
+
+    # Don't write anything at the metadata path!
+    schema_path = os.path.join(tmp_path, "metadata.parquet")
+
+    basic_data_shard_df.to_parquet(paths.pixel_catalog_file(partition_dir, 1, 0))
+    basic_data_shard_df.to_parquet(paths.pixel_catalog_file(partition_dir, 1, 1))
+
+    with pytest.raises(FileNotFoundError):
+        margin_cache_map_reduce.reduce_margin_shards(
+            intermediate_dir,
+            "1_21",
+            tmp_path,
+            None,
+            1,
+            21,
+            original_catalog_metadata=schema_path,
+            delete_intermediate_parquet_files=True,
+            input_storage_options=None,
+        )
+
+    captured = capsys.readouterr()
+    assert "No such file or directory" in captured.out
```

### Comparing `hipscat_import-0.3.2/tests/hipscat_import/margin_cache/test_margin_round_trip.py` & `hipscat_import-0.3.3/tests/hipscat_import/margin_cache/test_margin_round_trip.py`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.2/tests/hipscat_import/soap/conftest.py` & `hipscat_import-0.3.3/tests/hipscat_import/soap/conftest.py`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.2/tests/hipscat_import/soap/test_run_soap.py` & `hipscat_import-0.3.3/tests/hipscat_import/soap/test_run_soap.py`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.2/tests/hipscat_import/soap/test_soap_arguments.py` & `hipscat_import-0.3.3/tests/hipscat_import/soap/test_soap_arguments.py`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.2/tests/hipscat_import/soap/test_soap_map_reduce.py` & `hipscat_import-0.3.3/tests/hipscat_import/soap/test_soap_map_reduce.py`

 * *Files 6% similar despite different names*

```diff
@@ -155,7 +155,23 @@
         HealpixPixel(
             parquet_file.metadata.row_group(row_index).column(join_order_column).statistics.min,
             parquet_file.metadata.row_group(row_index).column(join_pix_column).statistics.min,
         )
         for row_index in range(14)
     ]
     assert ordered_pixels == list(small_sky_soap_maps.keys())
+
+
+def test_reduce_joins_missing_files(small_sky_soap_args, soap_intermediate_dir, capsys):
+    """Use some previously-computed intermediate files to reduce the joined
+    leaf parquet files into a single parquet file."""
+    temp_path = os.path.join(small_sky_soap_args.tmp_path, "resume", "intermediate")
+    shutil.copytree(
+        soap_intermediate_dir,
+        temp_path,
+    )
+    small_sky_soap_args.tmp_path = temp_path
+
+    with pytest.raises(FileNotFoundError):
+        reduce_joins(small_sky_soap_args, HealpixPixel(0, 11), object_key="0_11")
+    captured = capsys.readouterr()
+    assert "No such file or directory" in captured.out
```

### Comparing `hipscat_import-0.3.2/tests/hipscat_import/soap/test_soap_resume_plan.py` & `hipscat_import-0.3.3/tests/hipscat_import/soap/test_soap_resume_plan.py`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.2/tests/hipscat_import/test_pipeline_resume_plan.py` & `hipscat_import-0.3.3/tests/hipscat_import/test_pipeline_resume_plan.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Test resume file operations"""
 
 import os
 from pathlib import Path
 
+import numpy.testing as npt
 import pytest
 
 from hipscat_import.pipeline_resume_plan import PipelineResumePlan
 
 
 def test_done_key(tmp_path):
     """Verify expected behavior of marking stage progress via done files."""
@@ -93,15 +94,15 @@
 
     ## If there are no more intermediate files, we don't need to set resume.
     plan.clean_resume_files()
     plan.safe_to_resume()
 
 
 @pytest.mark.dask
-def test_wait_for_futures(tmp_path, dask_client, capsys):
+def test_wait_for_futures(tmp_path, dask_client):
     """Test that we can wait around for futures to complete.
 
     Additionally test that relevant parts of the traceback are printed to stdout."""
     plan = PipelineResumePlan(tmp_path=tmp_path, progress_bar=False, resume=False)
 
     def error_on_even(argument):
         """Silly little method used to test futures that fail under predictable conditions"""
@@ -113,17 +114,30 @@
     plan.wait_for_futures(futures, "test")
 
     ## Throw an even in the mix, and we'll see some stages fail. Should cause whole stage to fail.
     futures = [dask_client.submit(error_on_even, 1), dask_client.submit(error_on_even, 2)]
     with pytest.raises(RuntimeError, match="Some test stages failed"):
         plan.wait_for_futures(futures, "test")
 
-        captured = capsys.readouterr()
-        assert "we are at odds with evens" in captured
-        assert "error_on_even" in captured
+
+@pytest.mark.dask
+def test_wait_for_futures_fail_fast(tmp_path, dask_client):
+    """Test that we can wait around for futures to complete.
+
+    Additionally test that relevant parts of the traceback are printed to stdout."""
+    plan = PipelineResumePlan(tmp_path=tmp_path, progress_bar=False, resume=False)
+
+    def error_on_even(argument):
+        """Silly little method used to test futures that fail under predictable conditions"""
+        if argument % 2 == 0:
+            raise RuntimeError("we are at odds with evens")
+
+    futures = [dask_client.submit(error_on_even, 3), dask_client.submit(error_on_even, 4)]
+    with pytest.raises(RuntimeError, match="we are at odds with evens"):
+        plan.wait_for_futures(futures, "test", fail_fast=True)
 
 
 def test_formatted_stage_name():
     """Test that we make pretty stage names for presenting in progress bars"""
     formatted = PipelineResumePlan.get_formatted_stage_name(None)
     assert formatted == "Progress  "
 
@@ -131,7 +145,22 @@
     assert formatted == "Progress  "
 
     formatted = PipelineResumePlan.get_formatted_stage_name("stage")
     assert formatted == "Stage     "
 
     formatted = PipelineResumePlan.get_formatted_stage_name("very long stage name")
     assert formatted == "Very long stage name"
+
+
+def test_check_original_input_paths(tmp_path, mixed_schema_csv_dir):
+    plan = PipelineResumePlan(tmp_path=tmp_path, progress_bar=False, resume=False)
+
+    input_file_list = [
+        Path(mixed_schema_csv_dir) / "input_01.csv",
+        Path(mixed_schema_csv_dir) / "input_02.csv",
+    ]
+
+    checked_files = plan.check_original_input_paths(input_file_list)
+
+    round_trip_files = plan.check_original_input_paths(checked_files)
+
+    npt.assert_array_equal(checked_files, round_trip_files)
```

### Comparing `hipscat_import-0.3.2/tests/hipscat_import/test_runtime_arguments.py` & `hipscat_import-0.3.3/tests/hipscat_import/test_runtime_arguments.py`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.2/tests/hipscat_import/verification/test_run_verification.py` & `hipscat_import-0.3.3/tests/hipscat_import/verification/test_run_verification.py`

 * *Files identical despite different names*

### Comparing `hipscat_import-0.3.2/tests/hipscat_import/verification/test_verification_arguments.py` & `hipscat_import-0.3.3/tests/hipscat_import/verification/test_verification_arguments.py`

 * *Files identical despite different names*

