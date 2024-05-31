# Comparing `tmp/asf_search-7.1.1.tar.gz` & `tmp/asf_search-7.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asf_search-7.1.1.tar", last modified: Thu Apr 25 18:54:17 2024, max compression
+gzip compressed data, was "asf_search-7.1.2.tar", last modified: Fri May 31 19:38:07 2024, max compression
```

## Comparing `asf_search-7.1.1.tar` & `asf_search-7.1.2.tar`

### file list

```diff
@@ -1,192 +1,192 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:54:17.182212 asf_search-7.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-25 18:54:12.000000 asf_search-7.1.1/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:54:17.150212 asf_search-7.1.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:54:17.154212 asf_search-7.1.1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      706 2024-04-25 18:54:12.000000 asf_search-7.1.1/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      306 2024-04-25 18:54:12.000000 asf_search-7.1.1/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 runner    (1001) docker     (127)      604 2024-04-25 18:54:12.000000 asf_search-7.1.1/.github/ISSUE_TEMPLATE/feature_request.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:54:17.154212 asf_search-7.1.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      490 2024-04-25 18:54:12.000000 asf_search-7.1.1/.github/workflows/changelog.yml
--rw-r--r--   0 runner    (1001) docker     (127)      493 2024-04-25 18:54:12.000000 asf_search-7.1.1/.github/workflows/label-prod-pr.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1873 2024-04-25 18:54:12.000000 asf_search-7.1.1/.github/workflows/prod-request-merged.yml
--rw-r--r--   0 runner    (1001) docker     (127)      786 2024-04-25 18:54:12.000000 asf_search-7.1.1/.github/workflows/pypi-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      654 2024-04-25 18:54:12.000000 asf_search-7.1.1/.github/workflows/run-pytest.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1862 2024-04-25 18:54:12.000000 asf_search-7.1.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)    29667 2024-04-25 18:54:12.000000 asf_search-7.1.1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-04-25 18:54:12.000000 asf_search-7.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7950 2024-04-25 18:54:17.182212 asf_search-7.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5967 2024-04-25 18:54:12.000000 asf_search-7.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:54:17.154212 asf_search-7.1.1/asf_search/
--rw-r--r--   0 runner    (1001) docker     (127)    17769 2024-04-25 18:54:12.000000 asf_search-7.1.1/asf_search/ASFProduct.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:54:17.154212 asf_search-7.1.1/asf_search/ASFSearchOptions/
--rw-r--r--   0 runner    (1001) docker     (127)     4709 2024-04-25 18:54:12.000000 asf_search-7.1.1/asf_search/ASFSearchOptions/ASFSearchOptions.py
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-25 18:54:12.000000 asf_search-7.1.1/asf_search/ASFSearchOptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-25 18:54:12.000000 asf_search-7.1.1/asf_search/ASFSearchOptions/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2931 2024-04-25 18:54:12.000000 asf_search-7.1.1/asf_search/ASFSearchOptions/validator_map.py
--rw-r--r--   0 runner    (1001) docker     (127)     8829 2024-04-25 18:54:12.000000 asf_search-7.1.1/asf_search/ASFSearchOptions/validators.py
--rw-r--r--   0 runner    (1001) docker     (127)     3771 2024-04-25 18:54:12.000000 asf_search-7.1.1/asf_search/ASFSearchResults.py
--rw-r--r--   0 runner    (1001) docker     (127)    10680 2024-04-25 18:54:12.000000 asf_search-7.1.1/asf_search/ASFSession.py
--rw-r--r--   0 runner    (1001) docker     (127)     2782 2024-04-25 18:54:12.000000 asf_search-7.1.1/asf_search/ASFStackableProduct.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:54:17.158212 asf_search-7.1.1/asf_search/CMR/
--rw-r--r--   0 runner    (1001) docker     (127)      874 2024-04-25 18:54:12.000000 asf_search-7.1.1/asf_search/CMR/MissionList.py
--rw-r--r--   0 runner    (1001) docker     (127)      297 2024-04-25 18:54:12.000000 asf_search-7.1.1/asf_search/CMR/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    44421 2024-04-25 18:54:12.000000 asf_search-7.1.1/asf_search/CMR/datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)     3912 2024-04-25 18:54:12.000000 asf_search-7.1.1/asf_search/CMR/field_map.py
--rw-r--r--   0 runner    (1001) docker     (127)     5654 2024-04-25 18:54:12.000000 asf_search-7.1.1/asf_search/CMR/subquery.py
--rw-r--r--   0 runner    (1001) docker     (127)     7616 2024-04-25 18:54:12.000000 asf_search-7.1.1/asf_search/CMR/translate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:54:17.158212 asf_search-7.1.1/asf_search/Products/
--rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-04-25 18:54:12.000000 asf_search-7.1.1/asf_search/Products/AIRSARProduct.py
--rw-r--r--   0 runner    (1001) docker     (127)     1709 2024-04-25 18:54:12.000000 asf_search-7.1.1/asf_search/Products/ALOSProduct.py
--rw-r--r--   0 runner    (1001) docker     (127)     2604 2024-04-25 18:54:12.000000 asf_search-7.1.1/asf_search/Products/ARIAS1GUNWProduct.py
--rw-r--r--   0 runner    (1001) docker     (127)     1628 2024-04-25 18:54:12.000000 asf_search-7.1.1/asf_search/Products/ERSProduct.py
--rw-r--r--   0 runner    (1001) docker     (127)     1325 2024-04-25 18:54:12.000000 asf_search-7.1.1/asf_search/Products/JERSProduct.py
--rw-r--r--   0 runner    (1001) docker     (127)     1858 2024-04-25 18:54:12.000000 asf_search-7.1.1/asf_search/Products/NISARProduct.py
--rw-r--r--   0 runner    (1001) docker     (127)     3482 2024-04-25 18:54:12.000000 asf_search-7.1.1/asf_search/Products/OPERAS1Product.py
--rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-04-25 18:54:12.000000 asf_search-7.1.1/asf_search/Products/RADARSATProduct.py
--rw-r--r--   0 runner    (1001) docker     (127)     4538 2024-04-25 18:54:12.000000 asf_search-7.1.1/asf_search/Products/S1BurstProduct.py
--rw-r--r--   0 runner    (1001) docker     (127)     5796 2024-04-25 18:54:12.000000 asf_search-7.1.1/asf_search/Products/S1Product.py
--rw-r--r--   0 runner    (1001) docker     (127)      908 2024-04-25 18:54:12.000000 asf_search-7.1.1/asf_search/Products/SEASATProduct.py
--rw-r--r--   0 runner    (1001) docker     (127)      881 2024-04-25 18:54:12.000000 asf_search-7.1.1/asf_search/Products/SIRCProduct.py
--rw-r--r--   0 runner    (1001) docker     (127)      913 2024-04-25 18:54:12.000000 asf_search-7.1.1/asf_search/Products/SMAPProduct.py
--rw-r--r--   0 runner    (1001) docker     (127)      872 2024-04-25 18:54:12.000000 asf_search-7.1.1/asf_search/Products/UAVSARProduct.py
--rw-r--r--   0 runner    (1001) docker     (127)      557 2024-04-25 18:54:12.000000 asf_search-7.1.1/asf_search/Products/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:54:17.158212 asf_search-7.1.1/asf_search/WKT/
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-25 18:54:12.000000 asf_search-7.1.1/asf_search/WKT/RepairEntry.py
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-25 18:54:12.000000 asf_search-7.1.1/asf_search/WKT/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13339 2024-04-25 18:54:12.000000 asf_search-7.1.1/asf_search/WKT/validate_wkt.py
--rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-04-25 18:54:12.000000 asf_search-7.1.1/asf_search/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:54:17.158212 asf_search-7.1.1/asf_search/baseline/
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-25 18:54:12.000000 asf_search-7.1.1/asf_search/baseline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8424 2024-04-25 18:54:12.000000 asf_search-7.1.1/asf_search/baseline/calc.py
--rw-r--r--   0 runner    (1001) docker     (127)     3771 2024-04-25 18:54:12.000000 asf_search-7.1.1/asf_search/baseline/stack.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:54:17.162212 asf_search-7.1.1/asf_search/constants/
--rw-r--r--   0 runner    (1001) docker     (127)      554 2024-04-25 18:54:12.000000 asf_search-7.1.1/asf_search/constants/BEAMMODE.py
--rw-r--r--   0 runner    (1001) docker     (127)      350 2024-04-25 18:54:12.000000 asf_search-7.1.1/asf_search/constants/DATASET.py
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-25 18:54:12.000000 asf_search-7.1.1/asf_search/constants/FLIGHT_DIRECTION.py
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-25 18:54:12.000000 asf_search-7.1.1/asf_search/constants/INSTRUMENT.py
--rw-r--r--   0 runner    (1001) docker     (127)      633 2024-04-25 18:54:12.000000 asf_search-7.1.1/asf_search/constants/INTERNAL.py
--rw-r--r--   0 runner    (1001) docker     (127)      276 2024-04-25 18:54:12.000000 asf_search-7.1.1/asf_search/constants/PLATFORM.py
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-04-25 18:54:12.000000 asf_search-7.1.1/asf_search/constants/POLARIZATION.py
--rw-r--r--   0 runner    (1001) docker     (127)     2086 2024-04-25 18:54:12.000000 asf_search-7.1.1/asf_search/constants/PRODUCT_TYPE.py
--rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-25 18:54:12.000000 asf_search-7.1.1/asf_search/constants/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:54:17.162212 asf_search-7.1.1/asf_search/download/
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-25 18:54:12.000000 asf_search-7.1.1/asf_search/download/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4248 2024-04-25 18:54:12.000000 asf_search-7.1.1/asf_search/download/download.py
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-25 18:54:12.000000 asf_search-7.1.1/asf_search/download/file_download_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-04-25 18:54:12.000000 asf_search-7.1.1/asf_search/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:54:17.162212 asf_search-7.1.1/asf_search/export/
--rw-r--r--   0 runner    (1001) docker     (127)      300 2024-04-25 18:54:12.000000 asf_search-7.1.1/asf_search/export/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6802 2024-04-25 18:54:12.000000 asf_search-7.1.1/asf_search/export/csv.py
--rw-r--r--   0 runner    (1001) docker     (127)     1421 2024-04-25 18:54:12.000000 asf_search-7.1.1/asf_search/export/export_translators.py
--rw-r--r--   0 runner    (1001) docker     (127)     1441 2024-04-25 18:54:12.000000 asf_search-7.1.1/asf_search/export/geojson.py
--rw-r--r--   0 runner    (1001) docker     (127)     6839 2024-04-25 18:54:12.000000 asf_search-7.1.1/asf_search/export/jsonlite.py
--rw-r--r--   0 runner    (1001) docker     (127)     2583 2024-04-25 18:54:12.000000 asf_search-7.1.1/asf_search/export/jsonlite2.py
--rw-r--r--   0 runner    (1001) docker     (127)     6888 2024-04-25 18:54:12.000000 asf_search-7.1.1/asf_search/export/kml.py
--rw-r--r--   0 runner    (1001) docker     (127)     3301 2024-04-25 18:54:12.000000 asf_search-7.1.1/asf_search/export/metalink.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:54:17.162212 asf_search-7.1.1/asf_search/health/
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-25 18:54:12.000000 asf_search-7.1.1/asf_search/health/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      539 2024-04-25 18:54:12.000000 asf_search-7.1.1/asf_search/health/health.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:54:17.166212 asf_search-7.1.1/asf_search/search/
--rw-r--r--   0 runner    (1001) docker     (127)      309 2024-04-25 18:54:12.000000 asf_search-7.1.1/asf_search/search/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4605 2024-04-25 18:54:12.000000 asf_search-7.1.1/asf_search/search/baseline_search.py
--rw-r--r--   0 runner    (1001) docker     (127)     1845 2024-04-25 18:54:12.000000 asf_search-7.1.1/asf_search/search/campaigns.py
--rw-r--r--   0 runner    (1001) docker     (127)     1753 2024-04-25 18:54:12.000000 asf_search-7.1.1/asf_search/search/error_reporting.py
--rw-r--r--   0 runner    (1001) docker     (127)     5256 2024-04-25 18:54:12.000000 asf_search-7.1.1/asf_search/search/geo_search.py
--rw-r--r--   0 runner    (1001) docker     (127)      886 2024-04-25 18:54:12.000000 asf_search-7.1.1/asf_search/search/granule_search.py
--rw-r--r--   0 runner    (1001) docker     (127)      888 2024-04-25 18:54:12.000000 asf_search-7.1.1/asf_search/search/product_search.py
--rw-r--r--   0 runner    (1001) docker     (127)     7493 2024-04-25 18:54:12.000000 asf_search-7.1.1/asf_search/search/search.py
--rw-r--r--   0 runner    (1001) docker     (127)     3559 2024-04-25 18:54:12.000000 asf_search-7.1.1/asf_search/search/search_count.py
--rw-r--r--   0 runner    (1001) docker     (127)    15751 2024-04-25 18:54:12.000000 asf_search-7.1.1/asf_search/search/search_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:54:17.182212 asf_search-7.1.1/asf_search.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7950 2024-04-25 18:54:17.000000 asf_search-7.1.1/asf_search.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5772 2024-04-25 18:54:17.000000 asf_search-7.1.1/asf_search.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 18:54:17.000000 asf_search-7.1.1/asf_search.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-25 18:54:17.000000 asf_search-7.1.1/asf_search.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-25 18:54:17.000000 asf_search-7.1.1/asf_search.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:54:17.166212 asf_search-7.1.1/examples/
--rw-r--r--   0 runner    (1001) docker     (127)     2679 2024-04-25 18:54:12.000000 asf_search-7.1.1/examples/0-Intro.md
--rw-r--r--   0 runner    (1001) docker     (127)    13465 2024-04-25 18:54:12.000000 asf_search-7.1.1/examples/1-Basic_Overview.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     6816 2024-04-25 18:54:12.000000 asf_search-7.1.1/examples/2-Geographic_Search.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    10801 2024-04-25 18:54:12.000000 asf_search-7.1.1/examples/3-Granule_Search.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     7312 2024-04-25 18:54:12.000000 asf_search-7.1.1/examples/4-Baseline_Search.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    14428 2024-04-25 18:54:12.000000 asf_search-7.1.1/examples/5-Download.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)      783 2024-04-25 18:54:12.000000 asf_search-7.1.1/examples/6-Outro.md
--rw-r--r--   0 runner    (1001) docker     (127)    14687 2024-04-25 18:54:12.000000 asf_search-7.1.1/examples/Advanced-Custom-ASFProduct-Subclassing.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     3630 2024-04-25 18:54:12.000000 asf_search-7.1.1/examples/hello_world.py
--rw-r--r--   0 runner    (1001) docker     (127)      345 2024-04-25 18:54:12.000000 asf_search-7.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 18:54:17.182212 asf_search-7.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2301 2024-04-25 18:54:12.000000 asf_search-7.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:54:17.166212 asf_search-7.1.1/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:54:17.166212 asf_search-7.1.1/tests/ASFProduct/
--rw-r--r--   0 runner    (1001) docker     (127)     3569 2024-04-25 18:54:12.000000 asf_search-7.1.1/tests/ASFProduct/test_ASFProduct.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:54:17.166212 asf_search-7.1.1/tests/ASFSearchOptions/
--rw-r--r--   0 runner    (1001) docker     (127)     2661 2024-04-25 18:54:12.000000 asf_search-7.1.1/tests/ASFSearchOptions/test_ASFSearchOptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:54:17.166212 asf_search-7.1.1/tests/ASFSearchResults/
--rw-r--r--   0 runner    (1001) docker     (127)     9303 2024-04-25 18:54:12.000000 asf_search-7.1.1/tests/ASFSearchResults/test_ASFSearchResults.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:54:17.166212 asf_search-7.1.1/tests/ASFSession/
--rw-r--r--   0 runner    (1001) docker     (127)     7472 2024-04-25 18:54:12.000000 asf_search-7.1.1/tests/ASFSession/test_ASFSession.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:54:17.166212 asf_search-7.1.1/tests/BaselineSearch/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:54:17.166212 asf_search-7.1.1/tests/BaselineSearch/Stack/
--rw-r--r--   0 runner    (1001) docker     (127)     2639 2024-04-25 18:54:12.000000 asf_search-7.1.1/tests/BaselineSearch/Stack/test_stack.py
--rw-r--r--   0 runner    (1001) docker     (127)     3767 2024-04-25 18:54:12.000000 asf_search-7.1.1/tests/BaselineSearch/test_baseline_search.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:54:17.166212 asf_search-7.1.1/tests/CMR/
--rw-r--r--   0 runner    (1001) docker     (127)      883 2024-04-25 18:54:12.000000 asf_search-7.1.1/tests/CMR/test_MissionList.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:54:17.166212 asf_search-7.1.1/tests/Search/
--rw-r--r--   0 runner    (1001) docker     (127)     7429 2024-04-25 18:54:12.000000 asf_search-7.1.1/tests/Search/test_search.py
--rw-r--r--   0 runner    (1001) docker     (127)     2456 2024-04-25 18:54:12.000000 asf_search-7.1.1/tests/Search/test_search_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:54:17.170212 asf_search-7.1.1/tests/Serialization/
--rw-r--r--   0 runner    (1001) docker     (127)     1566 2024-04-25 18:54:12.000000 asf_search-7.1.1/tests/Serialization/test_serialization.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:54:17.170212 asf_search-7.1.1/tests/WKT/
--rw-r--r--   0 runner    (1001) docker     (127)     2958 2024-04-25 18:54:12.000000 asf_search-7.1.1/tests/WKT/test_validate_wkt.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:54:17.170212 asf_search-7.1.1/tests/download/
--rw-r--r--   0 runner    (1001) docker     (127)     2405 2024-04-25 18:54:12.000000 asf_search-7.1.1/tests/download/test_download.py
--rw-r--r--   0 runner    (1001) docker     (127)     7386 2024-04-25 18:54:12.000000 asf_search-7.1.1/tests/pytest-config.yml
--rw-r--r--   0 runner    (1001) docker     (127)    18837 2024-04-25 18:54:12.000000 asf_search-7.1.1/tests/pytest-managers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:54:17.170212 asf_search-7.1.1/tests/yml_tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 18:54:17.182212 asf_search-7.1.1/tests/yml_tests/Resources/
--rw-r--r--   0 runner    (1001) docker     (127)    11951 2024-04-25 18:54:12.000000 asf_search-7.1.1/tests/yml_tests/Resources/Alos_response.yml
--rw-r--r--   0 runner    (1001) docker     (127)    23351 2024-04-25 18:54:12.000000 asf_search-7.1.1/tests/yml_tests/Resources/Alos_response_maxResults3.yml
--rw-r--r--   0 runner    (1001) docker     (127)    11957 2024-04-25 18:54:12.000000 asf_search-7.1.1/tests/yml_tests/Resources/Alos_response_missing_baseline.yml
--rw-r--r--   0 runner    (1001) docker     (127)    10954 2024-04-25 18:54:12.000000 asf_search-7.1.1/tests/yml_tests/Resources/Fairbanks_L1.yml
--rw-r--r--   0 runner    (1001) docker     (127)    31136 2024-04-25 18:54:12.000000 asf_search-7.1.1/tests/yml_tests/Resources/Fairbanks_S1_stack incomplete.yml
--rw-r--r--   0 runner    (1001) docker     (127)    48181 2024-04-25 18:54:12.000000 asf_search-7.1.1/tests/yml_tests/Resources/Fairbanks_S1_stack.yml
--rw-r--r--   0 runner    (1001) docker     (127)    46473 2024-04-25 18:54:12.000000 asf_search-7.1.1/tests/yml_tests/Resources/Fairbanks_S1_stack_preprocessed.yml
--rw-r--r--   0 runner    (1001) docker     (127)    44452 2024-04-25 18:54:12.000000 asf_search-7.1.1/tests/yml_tests/Resources/Fairbanks_S1_stack_preprocessed_incomplete.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-04-25 18:54:12.000000 asf_search-7.1.1/tests/yml_tests/Resources/Fairbanks_SLC.csv
--rw-r--r--   0 runner    (1001) docker     (127)     2336 2024-04-25 18:54:12.000000 asf_search-7.1.1/tests/yml_tests/Resources/Fairbanks_SLC.kml
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-25 18:54:12.000000 asf_search-7.1.1/tests/yml_tests/Resources/Fairbanks_SLC.metalink
--rw-r--r--   0 runner    (1001) docker     (127)    14418 2024-04-25 18:54:12.000000 asf_search-7.1.1/tests/yml_tests/Resources/Fairbanks_SLC.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3011 2024-04-25 18:54:12.000000 asf_search-7.1.1/tests/yml_tests/Resources/Fairbanks_SLC_Incomplete_Meta.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1472 2024-04-25 18:54:12.000000 asf_search-7.1.1/tests/yml_tests/Resources/Fairbanks_SLC_jsonlite.json
--rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-04-25 18:54:12.000000 asf_search-7.1.1/tests/yml_tests/Resources/Fairbanks_SLC_jsonlite2.json
--rw-r--r--   0 runner    (1001) docker     (127)    12816 2024-04-25 18:54:12.000000 asf_search-7.1.1/tests/yml_tests/Resources/Fairbanks_SLC_no_stateVectors.yml
--rw-r--r--   0 runner    (1001) docker     (127)    11560 2024-04-25 18:54:12.000000 asf_search-7.1.1/tests/yml_tests/Resources/Fairbanks_ers_reference.yml
--rw-r--r--   0 runner    (1001) docker     (127)    52821 2024-04-25 18:54:12.000000 asf_search-7.1.1/tests/yml_tests/Resources/Fairbanks_ers_stack preprocessed.yml
--rw-r--r--   0 runner    (1001) docker     (127)    53132 2024-04-25 18:54:12.000000 asf_search-7.1.1/tests/yml_tests/Resources/Fairbanks_ers_stack.yml
--rw-r--r--   0 runner    (1001) docker     (127)     7766 2024-04-25 18:54:12.000000 asf_search-7.1.1/tests/yml_tests/Resources/JERS.yml
--rw-r--r--   0 runner    (1001) docker     (127)    83735 2024-04-25 18:54:12.000000 asf_search-7.1.1/tests/yml_tests/Resources/JERS_stack.yml
--rw-r--r--   0 runner    (1001) docker     (127)    63985 2024-04-25 18:54:12.000000 asf_search-7.1.1/tests/yml_tests/Resources/OPERA_Products.yml
--rw-r--r--   0 runner    (1001) docker     (127)     4671 2024-04-25 18:54:12.000000 asf_search-7.1.1/tests/yml_tests/Resources/RADARSAT.yml
--rw-r--r--   0 runner    (1001) docker     (127)   308082 2024-04-25 18:54:12.000000 asf_search-7.1.1/tests/yml_tests/Resources/RADARSAT_stack.yml
--rw-r--r--   0 runner    (1001) docker     (127)   376802 2024-04-25 18:54:12.000000 asf_search-7.1.1/tests/yml_tests/Resources/S1_Interferogram_(beta)_cmr_ummjson.yml
--rw-r--r--   0 runner    (1001) docker     (127)    38828 2024-04-25 18:54:12.000000 asf_search-7.1.1/tests/yml_tests/Resources/S1_baseline_stack.yml
--rw-r--r--   0 runner    (1001) docker     (127)     9091 2024-04-25 18:54:12.000000 asf_search-7.1.1/tests/yml_tests/Resources/S1_response.yml
--rw-r--r--   0 runner    (1001) docker     (127)    18407 2024-04-25 18:54:12.000000 asf_search-7.1.1/tests/yml_tests/Resources/SLC_BURST.yml
--rw-r--r--   0 runner    (1001) docker     (127)  1807159 2024-04-25 18:54:12.000000 asf_search-7.1.1/tests/yml_tests/Resources/SLC_BURST_stack.yml
--rw-r--r--   0 runner    (1001) docker     (127)    16602 2024-04-25 18:54:12.000000 asf_search-7.1.1/tests/yml_tests/Resources/SMAP_response.yml
--rw-r--r--   0 runner    (1001) docker     (127)   600436 2024-04-25 18:54:12.000000 asf_search-7.1.1/tests/yml_tests/Resources/ShorelineMask26.shp
--rw-r--r--   0 runner    (1001) docker     (127)    20991 2024-04-25 18:54:12.000000 asf_search-7.1.1/tests/yml_tests/Resources/Shovel_Creek_many_points.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3692 2024-04-25 18:54:12.000000 asf_search-7.1.1/tests/yml_tests/test_ASFProduct.yml
--rw-r--r--   0 runner    (1001) docker     (127)     4106 2024-04-25 18:54:12.000000 asf_search-7.1.1/tests/yml_tests/test_ASFSearchOptions.yml
--rw-r--r--   0 runner    (1001) docker     (127)    22399 2024-04-25 18:54:12.000000 asf_search-7.1.1/tests/yml_tests/test_ASFSearchResults.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-04-25 18:54:12.000000 asf_search-7.1.1/tests/yml_tests/test_ASFSession.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-04-25 18:54:12.000000 asf_search-7.1.1/tests/yml_tests/test_baseline_search.yml
--rw-r--r--   0 runner    (1001) docker     (127)      349 2024-04-25 18:54:12.000000 asf_search-7.1.1/tests/yml_tests/test_campaigns.yml
--rw-r--r--   0 runner    (1001) docker     (127)      605 2024-04-25 18:54:12.000000 asf_search-7.1.1/tests/yml_tests/test_download.yml
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-25 18:54:12.000000 asf_search-7.1.1/tests/yml_tests/test_known_bugs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      459 2024-04-25 18:54:12.000000 asf_search-7.1.1/tests/yml_tests/test_notebooks.yml
--rw-r--r--   0 runner    (1001) docker     (127)    20759 2024-04-25 18:54:12.000000 asf_search-7.1.1/tests/yml_tests/test_search.yml
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-04-25 18:54:12.000000 asf_search-7.1.1/tests/yml_tests/test_search_generator.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-04-25 18:54:12.000000 asf_search-7.1.1/tests/yml_tests/test_serialization.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1766 2024-04-25 18:54:12.000000 asf_search-7.1.1/tests/yml_tests/test_stack.yml
--rw-r--r--   0 runner    (1001) docker     (127)    30725 2024-04-25 18:54:12.000000 asf_search-7.1.1/tests/yml_tests/test_validate_wkt.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 19:38:07.852380 asf_search-7.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-31 19:38:03.000000 asf_search-7.1.2/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 19:38:07.816380 asf_search-7.1.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 19:38:07.820380 asf_search-7.1.2/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      706 2024-05-31 19:38:03.000000 asf_search-7.1.2/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      306 2024-05-31 19:38:03.000000 asf_search-7.1.2/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      604 2024-05-31 19:38:03.000000 asf_search-7.1.2/.github/ISSUE_TEMPLATE/feature_request.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 19:38:07.820380 asf_search-7.1.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2024-05-31 19:38:03.000000 asf_search-7.1.2/.github/workflows/changelog.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      493 2024-05-31 19:38:03.000000 asf_search-7.1.2/.github/workflows/label-prod-pr.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1873 2024-05-31 19:38:03.000000 asf_search-7.1.2/.github/workflows/prod-request-merged.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      786 2024-05-31 19:38:03.000000 asf_search-7.1.2/.github/workflows/pypi-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      654 2024-05-31 19:38:03.000000 asf_search-7.1.2/.github/workflows/run-pytest.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1862 2024-05-31 19:38:03.000000 asf_search-7.1.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)    29966 2024-05-31 19:38:03.000000 asf_search-7.1.2/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-05-31 19:38:03.000000 asf_search-7.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7950 2024-05-31 19:38:07.852380 asf_search-7.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5967 2024-05-31 19:38:03.000000 asf_search-7.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 19:38:07.824380 asf_search-7.1.2/asf_search/
+-rw-r--r--   0 runner    (1001) docker     (127)    18136 2024-05-31 19:38:03.000000 asf_search-7.1.2/asf_search/ASFProduct.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 19:38:07.824380 asf_search-7.1.2/asf_search/ASFSearchOptions/
+-rw-r--r--   0 runner    (1001) docker     (127)     4709 2024-05-31 19:38:03.000000 asf_search-7.1.2/asf_search/ASFSearchOptions/ASFSearchOptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-31 19:38:03.000000 asf_search-7.1.2/asf_search/ASFSearchOptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-05-31 19:38:03.000000 asf_search-7.1.2/asf_search/ASFSearchOptions/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2931 2024-05-31 19:38:03.000000 asf_search-7.1.2/asf_search/ASFSearchOptions/validator_map.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8829 2024-05-31 19:38:03.000000 asf_search-7.1.2/asf_search/ASFSearchOptions/validators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3771 2024-05-31 19:38:03.000000 asf_search-7.1.2/asf_search/ASFSearchResults.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10680 2024-05-31 19:38:03.000000 asf_search-7.1.2/asf_search/ASFSession.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2782 2024-05-31 19:38:03.000000 asf_search-7.1.2/asf_search/ASFStackableProduct.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 19:38:07.824380 asf_search-7.1.2/asf_search/CMR/
+-rw-r--r--   0 runner    (1001) docker     (127)      874 2024-05-31 19:38:03.000000 asf_search-7.1.2/asf_search/CMR/MissionList.py
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2024-05-31 19:38:03.000000 asf_search-7.1.2/asf_search/CMR/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44421 2024-05-31 19:38:03.000000 asf_search-7.1.2/asf_search/CMR/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3912 2024-05-31 19:38:03.000000 asf_search-7.1.2/asf_search/CMR/field_map.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5654 2024-05-31 19:38:03.000000 asf_search-7.1.2/asf_search/CMR/subquery.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7616 2024-05-31 19:38:03.000000 asf_search-7.1.2/asf_search/CMR/translate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 19:38:07.828380 asf_search-7.1.2/asf_search/Products/
+-rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-05-31 19:38:03.000000 asf_search-7.1.2/asf_search/Products/AIRSARProduct.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1709 2024-05-31 19:38:03.000000 asf_search-7.1.2/asf_search/Products/ALOSProduct.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2596 2024-05-31 19:38:03.000000 asf_search-7.1.2/asf_search/Products/ARIAS1GUNWProduct.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1628 2024-05-31 19:38:03.000000 asf_search-7.1.2/asf_search/Products/ERSProduct.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1325 2024-05-31 19:38:03.000000 asf_search-7.1.2/asf_search/Products/JERSProduct.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1858 2024-05-31 19:38:03.000000 asf_search-7.1.2/asf_search/Products/NISARProduct.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4128 2024-05-31 19:38:03.000000 asf_search-7.1.2/asf_search/Products/OPERAS1Product.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-05-31 19:38:03.000000 asf_search-7.1.2/asf_search/Products/RADARSATProduct.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4538 2024-05-31 19:38:03.000000 asf_search-7.1.2/asf_search/Products/S1BurstProduct.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5796 2024-05-31 19:38:03.000000 asf_search-7.1.2/asf_search/Products/S1Product.py
+-rw-r--r--   0 runner    (1001) docker     (127)      908 2024-05-31 19:38:03.000000 asf_search-7.1.2/asf_search/Products/SEASATProduct.py
+-rw-r--r--   0 runner    (1001) docker     (127)      881 2024-05-31 19:38:03.000000 asf_search-7.1.2/asf_search/Products/SIRCProduct.py
+-rw-r--r--   0 runner    (1001) docker     (127)      913 2024-05-31 19:38:03.000000 asf_search-7.1.2/asf_search/Products/SMAPProduct.py
+-rw-r--r--   0 runner    (1001) docker     (127)      872 2024-05-31 19:38:03.000000 asf_search-7.1.2/asf_search/Products/UAVSARProduct.py
+-rw-r--r--   0 runner    (1001) docker     (127)      557 2024-05-31 19:38:03.000000 asf_search-7.1.2/asf_search/Products/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 19:38:07.828380 asf_search-7.1.2/asf_search/WKT/
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-05-31 19:38:03.000000 asf_search-7.1.2/asf_search/WKT/RepairEntry.py
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-31 19:38:03.000000 asf_search-7.1.2/asf_search/WKT/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13339 2024-05-31 19:38:03.000000 asf_search-7.1.2/asf_search/WKT/validate_wkt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-05-31 19:38:03.000000 asf_search-7.1.2/asf_search/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 19:38:07.828380 asf_search-7.1.2/asf_search/baseline/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-31 19:38:03.000000 asf_search-7.1.2/asf_search/baseline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8424 2024-05-31 19:38:03.000000 asf_search-7.1.2/asf_search/baseline/calc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3771 2024-05-31 19:38:03.000000 asf_search-7.1.2/asf_search/baseline/stack.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 19:38:07.828380 asf_search-7.1.2/asf_search/constants/
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-05-31 19:38:03.000000 asf_search-7.1.2/asf_search/constants/BEAMMODE.py
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-05-31 19:38:03.000000 asf_search-7.1.2/asf_search/constants/DATASET.py
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-31 19:38:03.000000 asf_search-7.1.2/asf_search/constants/FLIGHT_DIRECTION.py
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-31 19:38:03.000000 asf_search-7.1.2/asf_search/constants/INSTRUMENT.py
+-rw-r--r--   0 runner    (1001) docker     (127)      633 2024-05-31 19:38:03.000000 asf_search-7.1.2/asf_search/constants/INTERNAL.py
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-05-31 19:38:03.000000 asf_search-7.1.2/asf_search/constants/PLATFORM.py
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-05-31 19:38:03.000000 asf_search-7.1.2/asf_search/constants/POLARIZATION.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2086 2024-05-31 19:38:03.000000 asf_search-7.1.2/asf_search/constants/PRODUCT_TYPE.py
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-05-31 19:38:03.000000 asf_search-7.1.2/asf_search/constants/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 19:38:07.832380 asf_search-7.1.2/asf_search/download/
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-05-31 19:38:03.000000 asf_search-7.1.2/asf_search/download/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4248 2024-05-31 19:38:03.000000 asf_search-7.1.2/asf_search/download/download.py
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-31 19:38:03.000000 asf_search-7.1.2/asf_search/download/file_download_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-05-31 19:38:03.000000 asf_search-7.1.2/asf_search/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 19:38:07.832380 asf_search-7.1.2/asf_search/export/
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2024-05-31 19:38:03.000000 asf_search-7.1.2/asf_search/export/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6802 2024-05-31 19:38:03.000000 asf_search-7.1.2/asf_search/export/csv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1421 2024-05-31 19:38:03.000000 asf_search-7.1.2/asf_search/export/export_translators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1441 2024-05-31 19:38:03.000000 asf_search-7.1.2/asf_search/export/geojson.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6839 2024-05-31 19:38:03.000000 asf_search-7.1.2/asf_search/export/jsonlite.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2583 2024-05-31 19:38:03.000000 asf_search-7.1.2/asf_search/export/jsonlite2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6888 2024-05-31 19:38:03.000000 asf_search-7.1.2/asf_search/export/kml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3301 2024-05-31 19:38:03.000000 asf_search-7.1.2/asf_search/export/metalink.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 19:38:07.832380 asf_search-7.1.2/asf_search/health/
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-31 19:38:03.000000 asf_search-7.1.2/asf_search/health/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      539 2024-05-31 19:38:03.000000 asf_search-7.1.2/asf_search/health/health.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 19:38:07.832380 asf_search-7.1.2/asf_search/search/
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-05-31 19:38:03.000000 asf_search-7.1.2/asf_search/search/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4608 2024-05-31 19:38:03.000000 asf_search-7.1.2/asf_search/search/baseline_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1845 2024-05-31 19:38:03.000000 asf_search-7.1.2/asf_search/search/campaigns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1753 2024-05-31 19:38:03.000000 asf_search-7.1.2/asf_search/search/error_reporting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5256 2024-05-31 19:38:03.000000 asf_search-7.1.2/asf_search/search/geo_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)      886 2024-05-31 19:38:03.000000 asf_search-7.1.2/asf_search/search/granule_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)      888 2024-05-31 19:38:03.000000 asf_search-7.1.2/asf_search/search/product_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7493 2024-05-31 19:38:03.000000 asf_search-7.1.2/asf_search/search/search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3559 2024-05-31 19:38:03.000000 asf_search-7.1.2/asf_search/search/search_count.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15861 2024-05-31 19:38:03.000000 asf_search-7.1.2/asf_search/search/search_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 19:38:07.848380 asf_search-7.1.2/asf_search.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7950 2024-05-31 19:38:07.000000 asf_search-7.1.2/asf_search.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5772 2024-05-31 19:38:07.000000 asf_search-7.1.2/asf_search.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 19:38:07.000000 asf_search-7.1.2/asf_search.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-31 19:38:07.000000 asf_search-7.1.2/asf_search.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-31 19:38:07.000000 asf_search-7.1.2/asf_search.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 19:38:07.836380 asf_search-7.1.2/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     2679 2024-05-31 19:38:03.000000 asf_search-7.1.2/examples/0-Intro.md
+-rw-r--r--   0 runner    (1001) docker     (127)    13465 2024-05-31 19:38:03.000000 asf_search-7.1.2/examples/1-Basic_Overview.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     6816 2024-05-31 19:38:03.000000 asf_search-7.1.2/examples/2-Geographic_Search.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    10801 2024-05-31 19:38:03.000000 asf_search-7.1.2/examples/3-Granule_Search.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     7312 2024-05-31 19:38:03.000000 asf_search-7.1.2/examples/4-Baseline_Search.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    14428 2024-05-31 19:38:03.000000 asf_search-7.1.2/examples/5-Download.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)      783 2024-05-31 19:38:03.000000 asf_search-7.1.2/examples/6-Outro.md
+-rw-r--r--   0 runner    (1001) docker     (127)    14687 2024-05-31 19:38:03.000000 asf_search-7.1.2/examples/Advanced-Custom-ASFProduct-Subclassing.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     3630 2024-05-31 19:38:03.000000 asf_search-7.1.2/examples/hello_world.py
+-rw-r--r--   0 runner    (1001) docker     (127)      345 2024-05-31 19:38:03.000000 asf_search-7.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 19:38:07.852380 asf_search-7.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2301 2024-05-31 19:38:03.000000 asf_search-7.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 19:38:07.836380 asf_search-7.1.2/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 19:38:07.836380 asf_search-7.1.2/tests/ASFProduct/
+-rw-r--r--   0 runner    (1001) docker     (127)     3569 2024-05-31 19:38:03.000000 asf_search-7.1.2/tests/ASFProduct/test_ASFProduct.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 19:38:07.836380 asf_search-7.1.2/tests/ASFSearchOptions/
+-rw-r--r--   0 runner    (1001) docker     (127)     2661 2024-05-31 19:38:03.000000 asf_search-7.1.2/tests/ASFSearchOptions/test_ASFSearchOptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 19:38:07.836380 asf_search-7.1.2/tests/ASFSearchResults/
+-rw-r--r--   0 runner    (1001) docker     (127)     9303 2024-05-31 19:38:03.000000 asf_search-7.1.2/tests/ASFSearchResults/test_ASFSearchResults.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 19:38:07.836380 asf_search-7.1.2/tests/ASFSession/
+-rw-r--r--   0 runner    (1001) docker     (127)     7472 2024-05-31 19:38:03.000000 asf_search-7.1.2/tests/ASFSession/test_ASFSession.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 19:38:07.836380 asf_search-7.1.2/tests/BaselineSearch/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 19:38:07.836380 asf_search-7.1.2/tests/BaselineSearch/Stack/
+-rw-r--r--   0 runner    (1001) docker     (127)     2639 2024-05-31 19:38:03.000000 asf_search-7.1.2/tests/BaselineSearch/Stack/test_stack.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3767 2024-05-31 19:38:03.000000 asf_search-7.1.2/tests/BaselineSearch/test_baseline_search.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 19:38:07.836380 asf_search-7.1.2/tests/CMR/
+-rw-r--r--   0 runner    (1001) docker     (127)      883 2024-05-31 19:38:03.000000 asf_search-7.1.2/tests/CMR/test_MissionList.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 19:38:07.836380 asf_search-7.1.2/tests/Search/
+-rw-r--r--   0 runner    (1001) docker     (127)     7429 2024-05-31 19:38:03.000000 asf_search-7.1.2/tests/Search/test_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2456 2024-05-31 19:38:03.000000 asf_search-7.1.2/tests/Search/test_search_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 19:38:07.836380 asf_search-7.1.2/tests/Serialization/
+-rw-r--r--   0 runner    (1001) docker     (127)     1566 2024-05-31 19:38:03.000000 asf_search-7.1.2/tests/Serialization/test_serialization.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 19:38:07.836380 asf_search-7.1.2/tests/WKT/
+-rw-r--r--   0 runner    (1001) docker     (127)     2958 2024-05-31 19:38:03.000000 asf_search-7.1.2/tests/WKT/test_validate_wkt.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 19:38:07.836380 asf_search-7.1.2/tests/download/
+-rw-r--r--   0 runner    (1001) docker     (127)     2405 2024-05-31 19:38:03.000000 asf_search-7.1.2/tests/download/test_download.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7386 2024-05-31 19:38:03.000000 asf_search-7.1.2/tests/pytest-config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    18837 2024-05-31 19:38:03.000000 asf_search-7.1.2/tests/pytest-managers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 19:38:07.840380 asf_search-7.1.2/tests/yml_tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 19:38:07.848380 asf_search-7.1.2/tests/yml_tests/Resources/
+-rw-r--r--   0 runner    (1001) docker     (127)    11951 2024-05-31 19:38:03.000000 asf_search-7.1.2/tests/yml_tests/Resources/Alos_response.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    23351 2024-05-31 19:38:03.000000 asf_search-7.1.2/tests/yml_tests/Resources/Alos_response_maxResults3.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    11957 2024-05-31 19:38:03.000000 asf_search-7.1.2/tests/yml_tests/Resources/Alos_response_missing_baseline.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    10954 2024-05-31 19:38:03.000000 asf_search-7.1.2/tests/yml_tests/Resources/Fairbanks_L1.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    31136 2024-05-31 19:38:03.000000 asf_search-7.1.2/tests/yml_tests/Resources/Fairbanks_S1_stack incomplete.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    48181 2024-05-31 19:38:03.000000 asf_search-7.1.2/tests/yml_tests/Resources/Fairbanks_S1_stack.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    46473 2024-05-31 19:38:03.000000 asf_search-7.1.2/tests/yml_tests/Resources/Fairbanks_S1_stack_preprocessed.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    44452 2024-05-31 19:38:03.000000 asf_search-7.1.2/tests/yml_tests/Resources/Fairbanks_S1_stack_preprocessed_incomplete.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-05-31 19:38:03.000000 asf_search-7.1.2/tests/yml_tests/Resources/Fairbanks_SLC.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     2336 2024-05-31 19:38:03.000000 asf_search-7.1.2/tests/yml_tests/Resources/Fairbanks_SLC.kml
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-05-31 19:38:03.000000 asf_search-7.1.2/tests/yml_tests/Resources/Fairbanks_SLC.metalink
+-rw-r--r--   0 runner    (1001) docker     (127)    14418 2024-05-31 19:38:03.000000 asf_search-7.1.2/tests/yml_tests/Resources/Fairbanks_SLC.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3011 2024-05-31 19:38:03.000000 asf_search-7.1.2/tests/yml_tests/Resources/Fairbanks_SLC_Incomplete_Meta.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1472 2024-05-31 19:38:03.000000 asf_search-7.1.2/tests/yml_tests/Resources/Fairbanks_SLC_jsonlite.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-05-31 19:38:03.000000 asf_search-7.1.2/tests/yml_tests/Resources/Fairbanks_SLC_jsonlite2.json
+-rw-r--r--   0 runner    (1001) docker     (127)    12816 2024-05-31 19:38:03.000000 asf_search-7.1.2/tests/yml_tests/Resources/Fairbanks_SLC_no_stateVectors.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    11560 2024-05-31 19:38:03.000000 asf_search-7.1.2/tests/yml_tests/Resources/Fairbanks_ers_reference.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    52821 2024-05-31 19:38:03.000000 asf_search-7.1.2/tests/yml_tests/Resources/Fairbanks_ers_stack preprocessed.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    53132 2024-05-31 19:38:03.000000 asf_search-7.1.2/tests/yml_tests/Resources/Fairbanks_ers_stack.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     7766 2024-05-31 19:38:03.000000 asf_search-7.1.2/tests/yml_tests/Resources/JERS.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    83735 2024-05-31 19:38:03.000000 asf_search-7.1.2/tests/yml_tests/Resources/JERS_stack.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    63985 2024-05-31 19:38:03.000000 asf_search-7.1.2/tests/yml_tests/Resources/OPERA_Products.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     4671 2024-05-31 19:38:03.000000 asf_search-7.1.2/tests/yml_tests/Resources/RADARSAT.yml
+-rw-r--r--   0 runner    (1001) docker     (127)   308082 2024-05-31 19:38:03.000000 asf_search-7.1.2/tests/yml_tests/Resources/RADARSAT_stack.yml
+-rw-r--r--   0 runner    (1001) docker     (127)   376802 2024-05-31 19:38:03.000000 asf_search-7.1.2/tests/yml_tests/Resources/S1_Interferogram_(beta)_cmr_ummjson.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    38828 2024-05-31 19:38:03.000000 asf_search-7.1.2/tests/yml_tests/Resources/S1_baseline_stack.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     9091 2024-05-31 19:38:03.000000 asf_search-7.1.2/tests/yml_tests/Resources/S1_response.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    18407 2024-05-31 19:38:03.000000 asf_search-7.1.2/tests/yml_tests/Resources/SLC_BURST.yml
+-rw-r--r--   0 runner    (1001) docker     (127)  1807159 2024-05-31 19:38:03.000000 asf_search-7.1.2/tests/yml_tests/Resources/SLC_BURST_stack.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    16602 2024-05-31 19:38:03.000000 asf_search-7.1.2/tests/yml_tests/Resources/SMAP_response.yml
+-rw-r--r--   0 runner    (1001) docker     (127)   600436 2024-05-31 19:38:03.000000 asf_search-7.1.2/tests/yml_tests/Resources/ShorelineMask26.shp
+-rw-r--r--   0 runner    (1001) docker     (127)    20991 2024-05-31 19:38:03.000000 asf_search-7.1.2/tests/yml_tests/Resources/Shovel_Creek_many_points.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3692 2024-05-31 19:38:03.000000 asf_search-7.1.2/tests/yml_tests/test_ASFProduct.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     4106 2024-05-31 19:38:03.000000 asf_search-7.1.2/tests/yml_tests/test_ASFSearchOptions.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    22399 2024-05-31 19:38:03.000000 asf_search-7.1.2/tests/yml_tests/test_ASFSearchResults.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-05-31 19:38:03.000000 asf_search-7.1.2/tests/yml_tests/test_ASFSession.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-05-31 19:38:03.000000 asf_search-7.1.2/tests/yml_tests/test_baseline_search.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-05-31 19:38:03.000000 asf_search-7.1.2/tests/yml_tests/test_campaigns.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      605 2024-05-31 19:38:03.000000 asf_search-7.1.2/tests/yml_tests/test_download.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-31 19:38:03.000000 asf_search-7.1.2/tests/yml_tests/test_known_bugs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-05-31 19:38:03.000000 asf_search-7.1.2/tests/yml_tests/test_notebooks.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    20759 2024-05-31 19:38:03.000000 asf_search-7.1.2/tests/yml_tests/test_search.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-05-31 19:38:03.000000 asf_search-7.1.2/tests/yml_tests/test_search_generator.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-05-31 19:38:03.000000 asf_search-7.1.2/tests/yml_tests/test_serialization.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1766 2024-05-31 19:38:03.000000 asf_search-7.1.2/tests/yml_tests/test_stack.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    30725 2024-05-31 19:38:03.000000 asf_search-7.1.2/tests/yml_tests/test_validate_wkt.yml
```

### Comparing `asf_search-7.1.1/.github/ISSUE_TEMPLATE/bug_report.md` & `asf_search-7.1.2/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `asf_search-7.1.1/.github/ISSUE_TEMPLATE/feature_request.md` & `asf_search-7.1.2/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `asf_search-7.1.1/.github/workflows/prod-request-merged.yml` & `asf_search-7.1.2/.github/workflows/prod-request-merged.yml`

 * *Files identical despite different names*

### Comparing `asf_search-7.1.1/.github/workflows/pypi-publish.yml` & `asf_search-7.1.2/.github/workflows/pypi-publish.yml`

 * *Files identical despite different names*

### Comparing `asf_search-7.1.1/.github/workflows/run-pytest.yml` & `asf_search-7.1.2/.github/workflows/run-pytest.yml`

 * *Files identical despite different names*

### Comparing `asf_search-7.1.1/.gitignore` & `asf_search-7.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `asf_search-7.1.1/CHANGELOG.md` & `asf_search-7.1.2/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -22,14 +22,21 @@
 - 
 
 ### Removed:
 -
 
 -->
 ------
+## [v7.1.2](https://github.com/asfadmin/Discovery-asf_search/compare/v7.1.1...v7.1.2)
+### Fixed
+- `OPERAS1Product` subclass now properly assigned to PGE v2.0.1 results
+### Changed
+- `ARIAS1GUNWProduct.is_ARIAS1GUNWProduct()` removed, replaced with `ASFProduct._is_subclass()` implementation
+
+------
 ## [v7.1.1](https://github.com/asfadmin/Discovery-asf_search/compare/v7.1.0...v7.1.1)
 ### Changed
 - Uses `ciso8601.parse_datetime()` in baseline calculations, speeds up calculations on larger stacks
 ### Added
 - Adds `ASF_LOGGER` logging in `search_generator()` and related methods
 ### Fixed
 - `ASFProduct.get_sort_keys()` will no longer returns `None` if missing sort key, defaults to empty string
```

### Comparing `asf_search-7.1.1/LICENSE` & `asf_search-7.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `asf_search-7.1.1/PKG-INFO` & `asf_search-7.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asf_search
-Version: 7.1.1
+Version: 7.1.2
 Summary: Python wrapper for ASF's SearchAPI
 Home-page: https://github.com/asfadmin/Discovery-asf_search.git
 Author: Alaska Satellite Facility Discovery Team
 Author-email: uaf-asf-discovery@alaska.edu
 License: BSD
 Project-URL: Documentation, https://docs.asf.alaska.edu/asf_search/basics/
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `asf_search-7.1.1/README.md` & `asf_search-7.1.2/README.md`

 * *Files identical despite different names*

### Comparing `asf_search-7.1.1/asf_search/ASFProduct.py` & `asf_search-7.1.2/asf_search/ASFProduct.py`

 * *Files 2% similar despite different names*

```diff
@@ -420,7 +420,18 @@
     @staticmethod
     def umm_cast(f, v):
         """Tries to cast value v by callable f, returns None if it fails"""
         try:
             return f(v)
         except TypeError:
             return None
+
+    @staticmethod
+    def _is_subclass(item: Dict) -> bool:
+        """
+        Used to determine which subclass to use for specific edge-cases when parsing results in search methods
+        (Currently implemented for ARIA and OPERA subclasses).
+
+        params:
+        - item (dict): the CMR UMM-G item to read from
+        """
+        raise NotImplementedError()
```

### Comparing `asf_search-7.1.1/asf_search/ASFSearchOptions/ASFSearchOptions.py` & `asf_search-7.1.2/asf_search/ASFSearchOptions/ASFSearchOptions.py`

 * *Files identical despite different names*

### Comparing `asf_search-7.1.1/asf_search/ASFSearchOptions/validator_map.py` & `asf_search-7.1.2/asf_search/ASFSearchOptions/validator_map.py`

 * *Files identical despite different names*

### Comparing `asf_search-7.1.1/asf_search/ASFSearchOptions/validators.py` & `asf_search-7.1.2/asf_search/ASFSearchOptions/validators.py`

 * *Files identical despite different names*

### Comparing `asf_search-7.1.1/asf_search/ASFSearchResults.py` & `asf_search-7.1.2/asf_search/ASFSearchResults.py`

 * *Files identical despite different names*

### Comparing `asf_search-7.1.1/asf_search/ASFSession.py` & `asf_search-7.1.2/asf_search/ASFSession.py`

 * *Files identical despite different names*

### Comparing `asf_search-7.1.1/asf_search/ASFStackableProduct.py` & `asf_search-7.1.2/asf_search/ASFStackableProduct.py`

 * *Files identical despite different names*

### Comparing `asf_search-7.1.1/asf_search/CMR/MissionList.py` & `asf_search-7.1.2/asf_search/CMR/MissionList.py`

 * *Files identical despite different names*

### Comparing `asf_search-7.1.1/asf_search/CMR/datasets.py` & `asf_search-7.1.2/asf_search/CMR/datasets.py`

 * *Files identical despite different names*

### Comparing `asf_search-7.1.1/asf_search/CMR/field_map.py` & `asf_search-7.1.2/asf_search/CMR/field_map.py`

 * *Files identical despite different names*

### Comparing `asf_search-7.1.1/asf_search/CMR/subquery.py` & `asf_search-7.1.2/asf_search/CMR/subquery.py`

 * *Files identical despite different names*

### Comparing `asf_search-7.1.1/asf_search/CMR/translate.py` & `asf_search-7.1.2/asf_search/CMR/translate.py`

 * *Files identical despite different names*

### Comparing `asf_search-7.1.1/asf_search/Products/AIRSARProduct.py` & `asf_search-7.1.2/asf_search/Products/AIRSARProduct.py`

 * *Files identical despite different names*

### Comparing `asf_search-7.1.1/asf_search/Products/ALOSProduct.py` & `asf_search-7.1.2/asf_search/Products/ALOSProduct.py`

 * *Files identical despite different names*

### Comparing `asf_search-7.1.1/asf_search/Products/ARIAS1GUNWProduct.py` & `asf_search-7.1.2/asf_search/Products/ARIAS1GUNWProduct.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,14 +54,14 @@
     def get_default_baseline_product_type() -> None:
         """
         Returns the product type to search for when building a baseline stack.
         """
         return None
 
     @staticmethod
-    def is_ARIAS1GUNWProduct(item: Dict) -> bool:
+    def _is_subclass(item: Dict) -> bool:
         platform = ASFProduct.umm_get(item['umm'], 'Platforms', 0, 'ShortName')
         if platform in ['SENTINEL-1A', 'SENTINEL-1B']:
             asf_platform = ASFProduct.umm_get(item['umm'], 'AdditionalAttributes', ('Name', 'ASF_PLATFORM'), 'Values', 0)
             return 'Sentinel-1 Interferogram' in asf_platform
 
         return False
```

### Comparing `asf_search-7.1.1/asf_search/Products/ERSProduct.py` & `asf_search-7.1.2/asf_search/Products/ERSProduct.py`

 * *Files identical despite different names*

### Comparing `asf_search-7.1.1/asf_search/Products/JERSProduct.py` & `asf_search-7.1.2/asf_search/Products/JERSProduct.py`

 * *Files identical despite different names*

### Comparing `asf_search-7.1.1/asf_search/Products/NISARProduct.py` & `asf_search-7.1.2/asf_search/Products/NISARProduct.py`

 * *Files identical despite different names*

### Comparing `asf_search-7.1.1/asf_search/Products/OPERAS1Product.py` & `asf_search-7.1.2/asf_search/Products/OPERAS1Product.py`

 * *Files 21% similar despite different names*

```diff
@@ -15,14 +15,16 @@
         'operaBurstID': {'path': ['AdditionalAttributes', ('Name', 'OPERA_BURST_ID'), 'Values', 0]},
         'validityStartDate': {'path': ['TemporalExtent', 'SingleDateTime'], 'cast': try_parse_date},
         'bytes': {'path': ['DataGranule', 'ArchiveAndDistributionInformation']},
         'subswath': {'path': ['AdditionalAttributes', ('Name', 'SUBSWATH_NAME'), 'Values', 0]},
         'polarization': {'path': ['AdditionalAttributes', ('Name', 'POLARIZATION'), 'Values']} # dual polarization is in list rather than a 'VV+VH' style format
     }
 
+    _subclass_concept_ids = { 'C1257995185-ASF', 'C1257995186-ASF', 'C1258354200-ASF', 'C1258354201-ASF', 'C1259974840-ASF', 'C1259976861-ASF', 'C1259981910-ASF', 'C1259982010-ASF', 'C2777436413-ASF', 'C2777443834-ASF', 'C2795135174-ASF', 'C2795135668-ASF','C1260721853-ASF', 'C1260721945-ASF', 'C2803501097-ASF', 'C2803501758-ASF' }
+
     def __init__(self, args: Dict = {}, session: ASFSession = ASFSession()):
         super().__init__(args, session)
 
         self.baseline = None
 
         self.properties['beamMode'] = self.umm_get(self.umm, 'AdditionalAttributes', ('Name', 'BEAM_MODE'), 'Values', 0)
 
@@ -74,7 +76,14 @@
     def get_sort_keys(self) -> Tuple[str, str]:
         keys = super().get_sort_keys()
 
         if keys[0] == '':
             return (self._read_property('validityStartDate', ''), keys[1])
 
         return keys
+
+    @staticmethod
+    def _is_subclass(item: Dict) -> bool:
+        # not all umm products have this field set, 
+        # but when it's available it's convenient for fast matching
+        concept_id = item['meta'].get('collection-concept-id')
+        return concept_id in OPERAS1Product._subclass_concept_ids
```

### Comparing `asf_search-7.1.1/asf_search/Products/RADARSATProduct.py` & `asf_search-7.1.2/asf_search/Products/RADARSATProduct.py`

 * *Files identical despite different names*

### Comparing `asf_search-7.1.1/asf_search/Products/S1BurstProduct.py` & `asf_search-7.1.2/asf_search/Products/S1BurstProduct.py`

 * *Files identical despite different names*

### Comparing `asf_search-7.1.1/asf_search/Products/S1Product.py` & `asf_search-7.1.2/asf_search/Products/S1Product.py`

 * *Files identical despite different names*

### Comparing `asf_search-7.1.1/asf_search/Products/SEASATProduct.py` & `asf_search-7.1.2/asf_search/Products/SEASATProduct.py`

 * *Files identical despite different names*

### Comparing `asf_search-7.1.1/asf_search/Products/SIRCProduct.py` & `asf_search-7.1.2/asf_search/Products/SIRCProduct.py`

 * *Files identical despite different names*

### Comparing `asf_search-7.1.1/asf_search/Products/SMAPProduct.py` & `asf_search-7.1.2/asf_search/Products/SMAPProduct.py`

 * *Files identical despite different names*

### Comparing `asf_search-7.1.1/asf_search/Products/UAVSARProduct.py` & `asf_search-7.1.2/asf_search/Products/UAVSARProduct.py`

 * *Files identical despite different names*

### Comparing `asf_search-7.1.1/asf_search/Products/__init__.py` & `asf_search-7.1.2/asf_search/Products/__init__.py`

 * *Files identical despite different names*

### Comparing `asf_search-7.1.1/asf_search/WKT/validate_wkt.py` & `asf_search-7.1.2/asf_search/WKT/validate_wkt.py`

 * *Files identical despite different names*

### Comparing `asf_search-7.1.1/asf_search/__init__.py` & `asf_search-7.1.2/asf_search/__init__.py`

 * *Files identical despite different names*

### Comparing `asf_search-7.1.1/asf_search/baseline/calc.py` & `asf_search-7.1.2/asf_search/baseline/calc.py`

 * *Files identical despite different names*

### Comparing `asf_search-7.1.1/asf_search/baseline/stack.py` & `asf_search-7.1.2/asf_search/baseline/stack.py`

 * *Files identical despite different names*

### Comparing `asf_search-7.1.1/asf_search/constants/BEAMMODE.py` & `asf_search-7.1.2/asf_search/constants/BEAMMODE.py`

 * *Files identical despite different names*

### Comparing `asf_search-7.1.1/asf_search/constants/INTERNAL.py` & `asf_search-7.1.2/asf_search/constants/INTERNAL.py`

 * *Files identical despite different names*

### Comparing `asf_search-7.1.1/asf_search/constants/PRODUCT_TYPE.py` & `asf_search-7.1.2/asf_search/constants/PRODUCT_TYPE.py`

 * *Files identical despite different names*

### Comparing `asf_search-7.1.1/asf_search/download/download.py` & `asf_search-7.1.2/asf_search/download/download.py`

 * *Files identical despite different names*

### Comparing `asf_search-7.1.1/asf_search/exceptions.py` & `asf_search-7.1.2/asf_search/exceptions.py`

 * *Files identical despite different names*

### Comparing `asf_search-7.1.1/asf_search/export/csv.py` & `asf_search-7.1.2/asf_search/export/csv.py`

 * *Files identical despite different names*

### Comparing `asf_search-7.1.1/asf_search/export/export_translators.py` & `asf_search-7.1.2/asf_search/export/export_translators.py`

 * *Files identical despite different names*

### Comparing `asf_search-7.1.1/asf_search/export/geojson.py` & `asf_search-7.1.2/asf_search/export/geojson.py`

 * *Files identical despite different names*

### Comparing `asf_search-7.1.1/asf_search/export/jsonlite.py` & `asf_search-7.1.2/asf_search/export/jsonlite.py`

 * *Files identical despite different names*

### Comparing `asf_search-7.1.1/asf_search/export/jsonlite2.py` & `asf_search-7.1.2/asf_search/export/jsonlite2.py`

 * *Files identical despite different names*

### Comparing `asf_search-7.1.1/asf_search/export/kml.py` & `asf_search-7.1.2/asf_search/export/kml.py`

 * *Files identical despite different names*

### Comparing `asf_search-7.1.1/asf_search/export/metalink.py` & `asf_search-7.1.2/asf_search/export/metalink.py`

 * *Files identical despite different names*

### Comparing `asf_search-7.1.1/asf_search/health/health.py` & `asf_search-7.1.2/asf_search/health/health.py`

 * *Files identical despite different names*

### Comparing `asf_search-7.1.1/asf_search/search/baseline_search.py` & `asf_search-7.1.2/asf_search/search/baseline_search.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 
     stack, warnings = get_baseline_from_stack(reference=reference, stack=stack)
     stack.searchComplete = is_complete # preserve final outcome of earlier search()
 
     stack.sort(key=lambda product: product.properties['temporalBaseline'])
 
     for warning in warnings:
-        ASF_LOGGER.warn(f'{warning}')
+        ASF_LOGGER.warning(f'{warning}')
     
     return stack
 
 
 def stack_from_id(
         reference_id: str,
         opts: ASFSearchOptions = None,
```

### Comparing `asf_search-7.1.1/asf_search/search/campaigns.py` & `asf_search-7.1.2/asf_search/search/campaigns.py`

 * *Files identical despite different names*

### Comparing `asf_search-7.1.1/asf_search/search/error_reporting.py` & `asf_search-7.1.2/asf_search/search/error_reporting.py`

 * *Files identical despite different names*

### Comparing `asf_search-7.1.1/asf_search/search/geo_search.py` & `asf_search-7.1.2/asf_search/search/geo_search.py`

 * *Files identical despite different names*

### Comparing `asf_search-7.1.1/asf_search/search/granule_search.py` & `asf_search-7.1.2/asf_search/search/granule_search.py`

 * *Files identical despite different names*

### Comparing `asf_search-7.1.1/asf_search/search/product_search.py` & `asf_search-7.1.2/asf_search/search/product_search.py`

 * *Files identical despite different names*

### Comparing `asf_search-7.1.1/asf_search/search/search.py` & `asf_search-7.1.2/asf_search/search/search.py`

 * *Files identical despite different names*

### Comparing `asf_search-7.1.1/asf_search/search/search_count.py` & `asf_search-7.1.2/asf_search/search/search_count.py`

 * *Files identical despite different names*

### Comparing `asf_search-7.1.1/asf_search/search/search_generator.py` & `asf_search-7.1.2/asf_search/search/search_generator.py`

 * *Files 2% similar despite different names*

```diff
@@ -262,14 +262,17 @@
     or ASFProduct if no equivalent is found
 
     :param item: the granule umm json
     :param session: the session used to query CMR for the product
 
     :returns the granule as an object of type ASFProduct
     """
+    if ASFProductType.OPERAS1Product._is_subclass(item):
+        return ASFProductType.OPERAS1Product(item, session=session)
+
     product_type_key = _get_product_type_key(item)
 
     # if there's a direct entry in our dataset to product type dict
     subclass = dataset_to_product_types.get(product_type_key)
     if subclass is not None:
         return subclass(item, session=session)
 
@@ -279,15 +282,15 @@
             subclass = dataset_to_product_types.get(dataset)
             if subclass is not None:
                 return subclass(item, session=session)
             break # dataset exists, but is not in dataset_to_product_types yet
 
     # If the platform exists, try to match it
     platform = _get_platform(item=item)
-    if ASFProductType.ARIAS1GUNWProduct.is_ARIAS1GUNWProduct(item=item):
+    if ASFProductType.ARIAS1GUNWProduct._is_subclass(item=item):
         return dataset_to_product_types.get('ARIA S1 GUNW')(item, session=session)
     elif (subclass := dataset_to_product_types.get(platform)) is not None:
         return subclass(item, session=session)
     
     output = ASFProduct(item, session=session)
     
     granule_concept_id = output.meta.get('concept-id', 'Missing Granule Concept ID')
@@ -302,18 +305,18 @@
         1. collection shortName (Ideal case)
         2. platform_shortName (Fallback)
             - special case: Aria S1 GUNW
     """
     collection_shortName = ASFProduct.umm_get(item['umm'], 'CollectionReference', 'ShortName')
 
     if collection_shortName is None:
-        platform = _get_platform(item=item)
-        if ASFProductType.ARIAS1GUNWProduct.is_ARIAS1GUNWProduct(item=item):
+        if ASFProductType.ARIAS1GUNWProduct._is_subclass(item=item):
             return 'ARIA S1 GUNW'
 
+        platform = _get_platform(item=item)
         return platform
 
     return collection_shortName
 
 def _get_platform(item: Dict):
     return ASFProduct.umm_get(item['umm'], 'Platforms', 0, 'ShortName')
```

### Comparing `asf_search-7.1.1/asf_search.egg-info/PKG-INFO` & `asf_search-7.1.2/asf_search.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asf_search
-Version: 7.1.1
+Version: 7.1.2
 Summary: Python wrapper for ASF's SearchAPI
 Home-page: https://github.com/asfadmin/Discovery-asf_search.git
 Author: Alaska Satellite Facility Discovery Team
 Author-email: uaf-asf-discovery@alaska.edu
 License: BSD
 Project-URL: Documentation, https://docs.asf.alaska.edu/asf_search/basics/
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `asf_search-7.1.1/asf_search.egg-info/SOURCES.txt` & `asf_search-7.1.2/asf_search.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `asf_search-7.1.1/examples/0-Intro.md` & `asf_search-7.1.2/examples/0-Intro.md`

 * *Files identical despite different names*

### Comparing `asf_search-7.1.1/examples/1-Basic_Overview.ipynb` & `asf_search-7.1.2/examples/1-Basic_Overview.ipynb`

 * *Files identical despite different names*

### Comparing `asf_search-7.1.1/examples/2-Geographic_Search.ipynb` & `asf_search-7.1.2/examples/2-Geographic_Search.ipynb`

 * *Files identical despite different names*

### Comparing `asf_search-7.1.1/examples/3-Granule_Search.ipynb` & `asf_search-7.1.2/examples/3-Granule_Search.ipynb`

 * *Files identical despite different names*

### Comparing `asf_search-7.1.1/examples/4-Baseline_Search.ipynb` & `asf_search-7.1.2/examples/4-Baseline_Search.ipynb`

 * *Files identical despite different names*

### Comparing `asf_search-7.1.1/examples/5-Download.ipynb` & `asf_search-7.1.2/examples/5-Download.ipynb`

 * *Files identical despite different names*

### Comparing `asf_search-7.1.1/examples/6-Outro.md` & `asf_search-7.1.2/examples/6-Outro.md`

 * *Files identical despite different names*

### Comparing `asf_search-7.1.1/examples/Advanced-Custom-ASFProduct-Subclassing.ipynb` & `asf_search-7.1.2/examples/Advanced-Custom-ASFProduct-Subclassing.ipynb`

 * *Files identical despite different names*

### Comparing `asf_search-7.1.1/examples/hello_world.py` & `asf_search-7.1.2/examples/hello_world.py`

 * *Files identical despite different names*

### Comparing `asf_search-7.1.1/setup.py` & `asf_search-7.1.2/setup.py`

 * *Files identical despite different names*

### Comparing `asf_search-7.1.1/tests/ASFProduct/test_ASFProduct.py` & `asf_search-7.1.2/tests/ASFProduct/test_ASFProduct.py`

 * *Files identical despite different names*

### Comparing `asf_search-7.1.1/tests/ASFSearchOptions/test_ASFSearchOptions.py` & `asf_search-7.1.2/tests/ASFSearchOptions/test_ASFSearchOptions.py`

 * *Files identical despite different names*

### Comparing `asf_search-7.1.1/tests/ASFSearchResults/test_ASFSearchResults.py` & `asf_search-7.1.2/tests/ASFSearchResults/test_ASFSearchResults.py`

 * *Files identical despite different names*

### Comparing `asf_search-7.1.1/tests/ASFSession/test_ASFSession.py` & `asf_search-7.1.2/tests/ASFSession/test_ASFSession.py`

 * *Files identical despite different names*

### Comparing `asf_search-7.1.1/tests/BaselineSearch/Stack/test_stack.py` & `asf_search-7.1.2/tests/BaselineSearch/Stack/test_stack.py`

 * *Files identical despite different names*

### Comparing `asf_search-7.1.1/tests/BaselineSearch/test_baseline_search.py` & `asf_search-7.1.2/tests/BaselineSearch/test_baseline_search.py`

 * *Files identical despite different names*

### Comparing `asf_search-7.1.1/tests/CMR/test_MissionList.py` & `asf_search-7.1.2/tests/CMR/test_MissionList.py`

 * *Files identical despite different names*

### Comparing `asf_search-7.1.1/tests/Search/test_search.py` & `asf_search-7.1.2/tests/Search/test_search.py`

 * *Files identical despite different names*

### Comparing `asf_search-7.1.1/tests/Search/test_search_generator.py` & `asf_search-7.1.2/tests/Search/test_search_generator.py`

 * *Files identical despite different names*

### Comparing `asf_search-7.1.1/tests/Serialization/test_serialization.py` & `asf_search-7.1.2/tests/Serialization/test_serialization.py`

 * *Files identical despite different names*

### Comparing `asf_search-7.1.1/tests/WKT/test_validate_wkt.py` & `asf_search-7.1.2/tests/WKT/test_validate_wkt.py`

 * *Files identical despite different names*

### Comparing `asf_search-7.1.1/tests/download/test_download.py` & `asf_search-7.1.2/tests/download/test_download.py`

 * *Files identical despite different names*

### Comparing `asf_search-7.1.1/tests/pytest-config.yml` & `asf_search-7.1.2/tests/pytest-config.yml`

 * *Files identical despite different names*

### Comparing `asf_search-7.1.1/tests/pytest-managers.py` & `asf_search-7.1.2/tests/pytest-managers.py`

 * *Files identical despite different names*

### Comparing `asf_search-7.1.1/tests/yml_tests/Resources/Alos_response.yml` & `asf_search-7.1.2/tests/yml_tests/Resources/Alos_response.yml`

 * *Files identical despite different names*

### Comparing `asf_search-7.1.1/tests/yml_tests/Resources/Alos_response_maxResults3.yml` & `asf_search-7.1.2/tests/yml_tests/Resources/Alos_response_maxResults3.yml`

 * *Files identical despite different names*

### Comparing `asf_search-7.1.1/tests/yml_tests/Resources/Alos_response_missing_baseline.yml` & `asf_search-7.1.2/tests/yml_tests/Resources/Alos_response_missing_baseline.yml`

 * *Files identical despite different names*

### Comparing `asf_search-7.1.1/tests/yml_tests/Resources/Fairbanks_L1.yml` & `asf_search-7.1.2/tests/yml_tests/Resources/Fairbanks_L1.yml`

 * *Files identical despite different names*

### Comparing `asf_search-7.1.1/tests/yml_tests/Resources/Fairbanks_S1_stack incomplete.yml` & `asf_search-7.1.2/tests/yml_tests/Resources/Fairbanks_S1_stack incomplete.yml`

 * *Files identical despite different names*

### Comparing `asf_search-7.1.1/tests/yml_tests/Resources/Fairbanks_S1_stack.yml` & `asf_search-7.1.2/tests/yml_tests/Resources/Fairbanks_S1_stack.yml`

 * *Files identical despite different names*

### Comparing `asf_search-7.1.1/tests/yml_tests/Resources/Fairbanks_S1_stack_preprocessed.yml` & `asf_search-7.1.2/tests/yml_tests/Resources/Fairbanks_S1_stack_preprocessed.yml`

 * *Files identical despite different names*

### Comparing `asf_search-7.1.1/tests/yml_tests/Resources/Fairbanks_S1_stack_preprocessed_incomplete.yml` & `asf_search-7.1.2/tests/yml_tests/Resources/Fairbanks_S1_stack_preprocessed_incomplete.yml`

 * *Files identical despite different names*

### Comparing `asf_search-7.1.1/tests/yml_tests/Resources/Fairbanks_SLC.csv` & `asf_search-7.1.2/tests/yml_tests/Resources/Fairbanks_SLC.csv`

 * *Files identical despite different names*

### Comparing `asf_search-7.1.1/tests/yml_tests/Resources/Fairbanks_SLC.kml` & `asf_search-7.1.2/tests/yml_tests/Resources/Fairbanks_SLC.kml`

 * *Files identical despite different names*

### Comparing `asf_search-7.1.1/tests/yml_tests/Resources/Fairbanks_SLC.metalink` & `asf_search-7.1.2/tests/yml_tests/Resources/Fairbanks_SLC.metalink`

 * *Files identical despite different names*

### Comparing `asf_search-7.1.1/tests/yml_tests/Resources/Fairbanks_SLC.yml` & `asf_search-7.1.2/tests/yml_tests/Resources/Fairbanks_SLC.yml`

 * *Files identical despite different names*

### Comparing `asf_search-7.1.1/tests/yml_tests/Resources/Fairbanks_SLC_Incomplete_Meta.yml` & `asf_search-7.1.2/tests/yml_tests/Resources/Fairbanks_SLC_Incomplete_Meta.yml`

 * *Files identical despite different names*

### Comparing `asf_search-7.1.1/tests/yml_tests/Resources/Fairbanks_SLC_jsonlite.json` & `asf_search-7.1.2/tests/yml_tests/Resources/Fairbanks_SLC_jsonlite.json`

 * *Files identical despite different names*

### Comparing `asf_search-7.1.1/tests/yml_tests/Resources/Fairbanks_SLC_jsonlite2.json` & `asf_search-7.1.2/tests/yml_tests/Resources/Fairbanks_SLC_jsonlite2.json`

 * *Files identical despite different names*

### Comparing `asf_search-7.1.1/tests/yml_tests/Resources/Fairbanks_SLC_no_stateVectors.yml` & `asf_search-7.1.2/tests/yml_tests/Resources/Fairbanks_SLC_no_stateVectors.yml`

 * *Files identical despite different names*

### Comparing `asf_search-7.1.1/tests/yml_tests/Resources/Fairbanks_ers_reference.yml` & `asf_search-7.1.2/tests/yml_tests/Resources/Fairbanks_ers_reference.yml`

 * *Files identical despite different names*

### Comparing `asf_search-7.1.1/tests/yml_tests/Resources/Fairbanks_ers_stack preprocessed.yml` & `asf_search-7.1.2/tests/yml_tests/Resources/Fairbanks_ers_stack preprocessed.yml`

 * *Files identical despite different names*

### Comparing `asf_search-7.1.1/tests/yml_tests/Resources/Fairbanks_ers_stack.yml` & `asf_search-7.1.2/tests/yml_tests/Resources/Fairbanks_ers_stack.yml`

 * *Files identical despite different names*

### Comparing `asf_search-7.1.1/tests/yml_tests/Resources/JERS.yml` & `asf_search-7.1.2/tests/yml_tests/Resources/JERS.yml`

 * *Files identical despite different names*

### Comparing `asf_search-7.1.1/tests/yml_tests/Resources/JERS_stack.yml` & `asf_search-7.1.2/tests/yml_tests/Resources/JERS_stack.yml`

 * *Files identical despite different names*

### Comparing `asf_search-7.1.1/tests/yml_tests/Resources/OPERA_Products.yml` & `asf_search-7.1.2/tests/yml_tests/Resources/OPERA_Products.yml`

 * *Files identical despite different names*

### Comparing `asf_search-7.1.1/tests/yml_tests/Resources/RADARSAT.yml` & `asf_search-7.1.2/tests/yml_tests/Resources/RADARSAT.yml`

 * *Files identical despite different names*

### Comparing `asf_search-7.1.1/tests/yml_tests/Resources/RADARSAT_stack.yml` & `asf_search-7.1.2/tests/yml_tests/Resources/RADARSAT_stack.yml`

 * *Files identical despite different names*

### Comparing `asf_search-7.1.1/tests/yml_tests/Resources/S1_Interferogram_(beta)_cmr_ummjson.yml` & `asf_search-7.1.2/tests/yml_tests/Resources/S1_Interferogram_(beta)_cmr_ummjson.yml`

 * *Files identical despite different names*

### Comparing `asf_search-7.1.1/tests/yml_tests/Resources/S1_baseline_stack.yml` & `asf_search-7.1.2/tests/yml_tests/Resources/S1_baseline_stack.yml`

 * *Files identical despite different names*

### Comparing `asf_search-7.1.1/tests/yml_tests/Resources/S1_response.yml` & `asf_search-7.1.2/tests/yml_tests/Resources/S1_response.yml`

 * *Files identical despite different names*

### Comparing `asf_search-7.1.1/tests/yml_tests/Resources/SLC_BURST.yml` & `asf_search-7.1.2/tests/yml_tests/Resources/SLC_BURST.yml`

 * *Files identical despite different names*

### Comparing `asf_search-7.1.1/tests/yml_tests/Resources/SLC_BURST_stack.yml` & `asf_search-7.1.2/tests/yml_tests/Resources/SLC_BURST_stack.yml`

 * *Files identical despite different names*

### Comparing `asf_search-7.1.1/tests/yml_tests/Resources/SMAP_response.yml` & `asf_search-7.1.2/tests/yml_tests/Resources/SMAP_response.yml`

 * *Files identical despite different names*

### Comparing `asf_search-7.1.1/tests/yml_tests/Resources/ShorelineMask26.shp` & `asf_search-7.1.2/tests/yml_tests/Resources/ShorelineMask26.shp`

 * *Files identical despite different names*

### Comparing `asf_search-7.1.1/tests/yml_tests/Resources/Shovel_Creek_many_points.yml` & `asf_search-7.1.2/tests/yml_tests/Resources/Shovel_Creek_many_points.yml`

 * *Files identical despite different names*

### Comparing `asf_search-7.1.1/tests/yml_tests/test_ASFProduct.yml` & `asf_search-7.1.2/tests/yml_tests/test_ASFProduct.yml`

 * *Files identical despite different names*

### Comparing `asf_search-7.1.1/tests/yml_tests/test_ASFSearchOptions.yml` & `asf_search-7.1.2/tests/yml_tests/test_ASFSearchOptions.yml`

 * *Files identical despite different names*

### Comparing `asf_search-7.1.1/tests/yml_tests/test_ASFSearchResults.yml` & `asf_search-7.1.2/tests/yml_tests/test_ASFSearchResults.yml`

 * *Files identical despite different names*

### Comparing `asf_search-7.1.1/tests/yml_tests/test_ASFSession.yml` & `asf_search-7.1.2/tests/yml_tests/test_ASFSession.yml`

 * *Files identical despite different names*

### Comparing `asf_search-7.1.1/tests/yml_tests/test_baseline_search.yml` & `asf_search-7.1.2/tests/yml_tests/test_baseline_search.yml`

 * *Files identical despite different names*

### Comparing `asf_search-7.1.1/tests/yml_tests/test_download.yml` & `asf_search-7.1.2/tests/yml_tests/test_download.yml`

 * *Files identical despite different names*

### Comparing `asf_search-7.1.1/tests/yml_tests/test_search.yml` & `asf_search-7.1.2/tests/yml_tests/test_search.yml`

 * *Files identical despite different names*

### Comparing `asf_search-7.1.1/tests/yml_tests/test_serialization.yml` & `asf_search-7.1.2/tests/yml_tests/test_serialization.yml`

 * *Files identical despite different names*

### Comparing `asf_search-7.1.1/tests/yml_tests/test_stack.yml` & `asf_search-7.1.2/tests/yml_tests/test_stack.yml`

 * *Files identical despite different names*

### Comparing `asf_search-7.1.1/tests/yml_tests/test_validate_wkt.yml` & `asf_search-7.1.2/tests/yml_tests/test_validate_wkt.yml`

 * *Files identical despite different names*

