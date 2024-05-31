# Comparing `tmp/hipscat-0.3.3.tar.gz` & `tmp/hipscat-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hipscat-0.3.3.tar", last modified: Tue May 21 17:30:14 2024, max compression
+gzip compressed data, was "hipscat-0.3.4.tar", last modified: Fri May 31 17:26:02 2024, max compression
```

## Comparing `hipscat-0.3.3.tar` & `hipscat-0.3.4.tar`

### file list

```diff
@@ -1,304 +1,305 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:30:14.900486 hipscat-0.3.3/
--rw-r--r--   0 runner    (1001) docker     (127)      558 2024-05-21 17:30:10.000000 hipscat-0.3.3/.copier-answers.yml
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-21 17:30:10.000000 hipscat-0.3.3/.git_archival.txt
--rw-r--r--   0 runner    (1001) docker     (127)      747 2024-05-21 17:30:10.000000 hipscat-0.3.3/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:30:14.860486 hipscat-0.3.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:30:14.860486 hipscat-0.3.3/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-21 17:30:10.000000 hipscat-0.3.3/.github/ISSUE_TEMPLATE/0-general_issue.md
--rw-r--r--   0 runner    (1001) docker     (127)      660 2024-05-21 17:30:10.000000 hipscat-0.3.3/.github/ISSUE_TEMPLATE/1-bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      706 2024-05-21 17:30:10.000000 hipscat-0.3.3/.github/ISSUE_TEMPLATE/2-feature_request.md
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-21 17:30:10.000000 hipscat-0.3.3/.github/dependabot.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3329 2024-05-21 17:30:10.000000 hipscat-0.3.3/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:30:14.860486 hipscat-0.3.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      358 2024-05-21 17:30:10.000000 hipscat-0.3.3/.github/workflows/add-issue-to-project-tracker.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2697 2024-05-21 17:30:10.000000 hipscat-0.3.3/.github/workflows/asv-main.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2839 2024-05-21 17:30:10.000000 hipscat-0.3.3/.github/workflows/asv-nightly.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3057 2024-05-21 17:30:10.000000 hipscat-0.3.3/.github/workflows/asv-pr.yml
--rw-r--r--   0 runner    (1001) docker     (127)      929 2024-05-21 17:30:10.000000 hipscat-0.3.3/.github/workflows/build-documentation.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-05-21 17:30:10.000000 hipscat-0.3.3/.github/workflows/pre-commit-ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2065 2024-05-21 17:30:10.000000 hipscat-0.3.3/.github/workflows/publish-benchmarks-pr.yml
--rw-r--r--   0 runner    (1001) docker     (127)      951 2024-05-21 17:30:10.000000 hipscat-0.3.3/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2359 2024-05-21 17:30:10.000000 hipscat-0.3.3/.github/workflows/smoke-test.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-05-21 17:30:10.000000 hipscat-0.3.3/.github/workflows/testing-and-coverage.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-05-21 17:30:10.000000 hipscat-0.3.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     5366 2024-05-21 17:30:10.000000 hipscat-0.3.3/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-05-21 17:30:10.000000 hipscat-0.3.3/.prepare_project.sh
--rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-21 17:30:10.000000 hipscat-0.3.3/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1539 2024-05-21 17:30:10.000000 hipscat-0.3.3/.setup_dev.sh
--rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-05-21 17:30:10.000000 hipscat-0.3.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5975 2024-05-21 17:30:14.900486 hipscat-0.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2860 2024-05-21 17:30:10.000000 hipscat-0.3.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:30:14.860486 hipscat-0.3.3/benchmarks/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 17:30:10.000000 hipscat-0.3.3/benchmarks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3597 2024-05-21 17:30:10.000000 hipscat-0.3.3/benchmarks/asv.conf.json
--rw-r--r--   0 runner    (1001) docker     (127)     4950 2024-05-21 17:30:10.000000 hipscat-0.3.3/benchmarks/benchmarks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:30:14.860486 hipscat-0.3.3/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-05-21 17:30:10.000000 hipscat-0.3.3/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:30:14.860486 hipscat-0.3.3/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-21 17:30:10.000000 hipscat-0.3.3/docs/_static/custom.css
--rw-r--r--   0 runner    (1001) docker     (127)     2151 2024-05-21 17:30:10.000000 hipscat-0.3.3/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:30:14.864486 hipscat-0.3.3/docs/guide/
--rw-r--r--   0 runner    (1001) docker     (127)     4409 2024-05-21 17:30:10.000000 hipscat-0.3.3/docs/guide/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-05-21 17:30:10.000000 hipscat-0.3.3/docs/guide/directory_scheme.rst
--rw-r--r--   0 runner    (1001) docker     (127)    17649 2024-05-21 17:30:10.000000 hipscat-0.3.3/docs/guide/margin_cache_diagram.png
--rw-r--r--   0 runner    (1001) docker     (127)    12890 2024-05-21 17:30:10.000000 hipscat-0.3.3/docs/guide/pixel_math.md
--rw-r--r--   0 runner    (1001) docker     (127)      923 2024-05-21 17:30:10.000000 hipscat-0.3.3/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:30:14.864486 hipscat-0.3.3/docs/notebooks/
--rw-r--r--   0 runner    (1001) docker     (127)     4988 2024-05-21 17:30:10.000000 hipscat-0.3.3/docs/notebooks/catalog_size_inspection.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     2303 2024-05-21 17:30:10.000000 hipscat-0.3.3/docs/notebooks/cone_search.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-21 17:30:10.000000 hipscat-0.3.3/docs/notebooks.rst
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-21 17:30:10.000000 hipscat-0.3.3/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2839 2024-05-21 17:30:10.000000 hipscat-0.3.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 17:30:14.900486 hipscat-0.3.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:30:14.864486 hipscat-0.3.3/src/
--rw-r--r--   0 runner    (1001) docker     (127)    20811 2024-05-21 17:30:10.000000 hipscat-0.3.3/src/.pylintrc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:30:14.864486 hipscat-0.3.3/src/hipscat/
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-21 17:30:10.000000 hipscat-0.3.3/src/hipscat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-21 17:30:14.000000 hipscat-0.3.3/src/hipscat/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:30:14.864486 hipscat-0.3.3/src/hipscat/catalog/
--rw-r--r--   0 runner    (1001) docker     (127)      302 2024-05-21 17:30:10.000000 hipscat-0.3.3/src/hipscat/catalog/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:30:14.864486 hipscat-0.3.3/src/hipscat/catalog/association_catalog/
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-05-21 17:30:10.000000 hipscat-0.3.3/src/hipscat/catalog/association_catalog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3883 2024-05-21 17:30:10.000000 hipscat-0.3.3/src/hipscat/catalog/association_catalog/association_catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-05-21 17:30:10.000000 hipscat-0.3.3/src/hipscat/catalog/association_catalog/association_catalog_info.py
--rw-r--r--   0 runner    (1001) docker     (127)    13211 2024-05-21 17:30:10.000000 hipscat-0.3.3/src/hipscat/catalog/association_catalog/partition_join_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     6029 2024-05-21 17:30:10.000000 hipscat-0.3.3/src/hipscat/catalog/catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)      513 2024-05-21 17:30:10.000000 hipscat-0.3.3/src/hipscat/catalog/catalog_info.py
--rw-r--r--   0 runner    (1001) docker     (127)      346 2024-05-21 17:30:10.000000 hipscat-0.3.3/src/hipscat/catalog/catalog_type.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:30:14.868486 hipscat-0.3.3/src/hipscat/catalog/dataset/
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-21 17:30:10.000000 hipscat-0.3.3/src/hipscat/catalog/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2768 2024-05-21 17:30:10.000000 hipscat-0.3.3/src/hipscat/catalog/dataset/base_catalog_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     3318 2024-05-21 17:30:10.000000 hipscat-0.3.3/src/hipscat/catalog/dataset/catalog_info_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     3512 2024-05-21 17:30:10.000000 hipscat-0.3.3/src/hipscat/catalog/dataset/dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:30:14.868486 hipscat-0.3.3/src/hipscat/catalog/healpix_dataset/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 17:30:10.000000 hipscat-0.3.3/src/hipscat/catalog/healpix_dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8107 2024-05-21 17:30:10.000000 hipscat-0.3.3/src/hipscat/catalog/healpix_dataset/healpix_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:30:14.868486 hipscat-0.3.3/src/hipscat/catalog/index/
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-21 17:30:10.000000 hipscat-0.3.3/src/hipscat/catalog/index/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2758 2024-05-21 17:30:10.000000 hipscat-0.3.3/src/hipscat/catalog/index/index_catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)      813 2024-05-21 17:30:10.000000 hipscat-0.3.3/src/hipscat/catalog/index/index_catalog_info.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:30:14.868486 hipscat-0.3.3/src/hipscat/catalog/margin_cache/
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-21 17:30:10.000000 hipscat-0.3.3/src/hipscat/catalog/margin_cache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      710 2024-05-21 17:30:10.000000 hipscat-0.3.3/src/hipscat/catalog/margin_cache/margin_cache_catalog_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     2170 2024-05-21 17:30:10.000000 hipscat-0.3.3/src/hipscat/catalog/margin_cache/margin_catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)    11819 2024-05-21 17:30:10.000000 hipscat-0.3.3/src/hipscat/catalog/partition_info.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:30:14.868486 hipscat-0.3.3/src/hipscat/catalog/source_catalog/
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-21 17:30:10.000000 hipscat-0.3.3/src/hipscat/catalog/source_catalog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      906 2024-05-21 17:30:10.000000 hipscat-0.3.3/src/hipscat/catalog/source_catalog/source_catalog_info.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:30:14.868486 hipscat-0.3.3/src/hipscat/inspection/
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-21 17:30:10.000000 hipscat-0.3.3/src/hipscat/inspection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11751 2024-05-21 17:30:10.000000 hipscat-0.3.3/src/hipscat/inspection/almanac.py
--rw-r--r--   0 runner    (1001) docker     (127)     5457 2024-05-21 17:30:10.000000 hipscat-0.3.3/src/hipscat/inspection/almanac_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     5462 2024-05-21 17:30:10.000000 hipscat-0.3.3/src/hipscat/inspection/visualize_catalog.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:30:14.868486 hipscat-0.3.3/src/hipscat/io/
--rw-r--r--   0 runner    (1001) docker     (127)      714 2024-05-21 17:30:10.000000 hipscat-0.3.3/src/hipscat/io/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:30:14.868486 hipscat-0.3.3/src/hipscat/io/file_io/
--rw-r--r--   0 runner    (1001) docker     (127)      815 2024-05-21 17:30:10.000000 hipscat-0.3.3/src/hipscat/io/file_io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12699 2024-05-21 17:30:10.000000 hipscat-0.3.3/src/hipscat/io/file_io/file_io.py
--rw-r--r--   0 runner    (1001) docker     (127)     8215 2024-05-21 17:30:10.000000 hipscat-0.3.3/src/hipscat/io/file_io/file_pointer.py
--rw-r--r--   0 runner    (1001) docker     (127)     7498 2024-05-21 17:30:10.000000 hipscat-0.3.3/src/hipscat/io/parquet_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     9634 2024-05-21 17:30:10.000000 hipscat-0.3.3/src/hipscat/io/paths.py
--rw-r--r--   0 runner    (1001) docker     (127)     2855 2024-05-21 17:30:10.000000 hipscat-0.3.3/src/hipscat/io/validation.py
--rw-r--r--   0 runner    (1001) docker     (127)     5839 2024-05-21 17:30:10.000000 hipscat-0.3.3/src/hipscat/io/write_metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:30:14.872486 hipscat-0.3.3/src/hipscat/loaders/
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-21 17:30:10.000000 hipscat-0.3.3/src/hipscat/loaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2404 2024-05-21 17:30:10.000000 hipscat-0.3.3/src/hipscat/loaders/read_from_hipscat.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:30:14.872486 hipscat-0.3.3/src/hipscat/pixel_math/
--rw-r--r--   0 runner    (1001) docker     (127)      546 2024-05-21 17:30:10.000000 hipscat-0.3.3/src/hipscat/pixel_math/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5533 2024-05-21 17:30:10.000000 hipscat-0.3.3/src/hipscat/pixel_math/box_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1543 2024-05-21 17:30:10.000000 hipscat-0.3.3/src/hipscat/pixel_math/cone_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-05-21 17:30:10.000000 hipscat-0.3.3/src/hipscat/pixel_math/filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     4979 2024-05-21 17:30:10.000000 hipscat-0.3.3/src/hipscat/pixel_math/healpix_pixel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-05-21 17:30:10.000000 hipscat-0.3.3/src/hipscat/pixel_math/healpix_pixel_convertor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2203 2024-05-21 17:30:10.000000 hipscat-0.3.3/src/hipscat/pixel_math/healpix_pixel_function.py
--rw-r--r--   0 runner    (1001) docker     (127)     4311 2024-05-21 17:30:10.000000 hipscat-0.3.3/src/hipscat/pixel_math/hipscat_id.py
--rw-r--r--   0 runner    (1001) docker     (127)     5651 2024-05-21 17:30:10.000000 hipscat-0.3.3/src/hipscat/pixel_math/margin_bounding.py
--rw-r--r--   0 runner    (1001) docker     (127)    12354 2024-05-21 17:30:10.000000 hipscat-0.3.3/src/hipscat/pixel_math/partition_stats.py
--rw-r--r--   0 runner    (1001) docker     (127)     4807 2024-05-21 17:30:10.000000 hipscat-0.3.3/src/hipscat/pixel_math/pixel_margins.py
--rw-r--r--   0 runner    (1001) docker     (127)     1942 2024-05-21 17:30:10.000000 hipscat-0.3.3/src/hipscat/pixel_math/polygon_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     4185 2024-05-21 17:30:10.000000 hipscat-0.3.3/src/hipscat/pixel_math/validators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:30:14.872486 hipscat-0.3.3/src/hipscat/pixel_tree/
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-21 17:30:10.000000 hipscat-0.3.3/src/hipscat/pixel_tree/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2153 2024-05-21 17:30:10.000000 hipscat-0.3.3/src/hipscat/pixel_tree/moc_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)      961 2024-05-21 17:30:10.000000 hipscat-0.3.3/src/hipscat/pixel_tree/negative_tree.py
--rw-r--r--   0 runner    (1001) docker     (127)    19695 2024-05-21 17:30:10.000000 hipscat-0.3.3/src/hipscat/pixel_tree/pixel_alignment.py
--rw-r--r--   0 runner    (1001) docker     (127)      302 2024-05-21 17:30:10.000000 hipscat-0.3.3/src/hipscat/pixel_tree/pixel_alignment_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     4367 2024-05-21 17:30:10.000000 hipscat-0.3.3/src/hipscat/pixel_tree/pixel_tree.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 17:30:10.000000 hipscat-0.3.3/src/hipscat/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:30:14.900486 hipscat-0.3.3/src/hipscat.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5975 2024-05-21 17:30:14.000000 hipscat-0.3.3/src/hipscat.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10075 2024-05-21 17:30:14.000000 hipscat-0.3.3/src/hipscat.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 17:30:14.000000 hipscat-0.3.3/src/hipscat.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-05-21 17:30:14.000000 hipscat-0.3.3/src/hipscat.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-21 17:30:14.000000 hipscat-0.3.3/src/hipscat.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:30:14.872486 hipscat-0.3.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    20972 2024-05-21 17:30:10.000000 hipscat-0.3.3/tests/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (127)     8358 2024-05-21 17:30:10.000000 hipscat-0.3.3/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:30:14.872486 hipscat-0.3.3/tests/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:30:14.876486 hipscat-0.3.3/tests/data/almanac/
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-21 17:30:10.000000 hipscat-0.3.3/tests/data/almanac/deprecated.yml
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-05-21 17:30:10.000000 hipscat-0.3.3/tests/data/almanac/small_sky.yml
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-21 17:30:10.000000 hipscat-0.3.3/tests/data/almanac/small_sky_order1.yml
--rw-r--r--   0 runner    (1001) docker     (127)      336 2024-05-21 17:30:10.000000 hipscat-0.3.3/tests/data/almanac/small_sky_order1_id_index.yml
--rw-r--r--   0 runner    (1001) docker     (127)      328 2024-05-21 17:30:10.000000 hipscat-0.3.3/tests/data/almanac/small_sky_order1_margin.yml
--rw-r--r--   0 runner    (1001) docker     (127)      363 2024-05-21 17:30:10.000000 hipscat-0.3.3/tests/data/almanac/small_sky_source.yml
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-21 17:30:10.000000 hipscat-0.3.3/tests/data/almanac/small_sky_source_object_index.yml
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-05-21 17:30:10.000000 hipscat-0.3.3/tests/data/almanac/small_sky_to_small_sky_order1.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:30:14.876486 hipscat-0.3.3/tests/data/almanac_exception/
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-05-21 17:30:10.000000 hipscat-0.3.3/tests/data/almanac_exception/association_missing_join.yml
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-21 17:30:10.000000 hipscat-0.3.3/tests/data/almanac_exception/association_missing_primary.yml
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-21 17:30:10.000000 hipscat-0.3.3/tests/data/almanac_exception/bad_catalog_path.yml
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-21 17:30:10.000000 hipscat-0.3.3/tests/data/almanac_exception/bad_primary_path.yml
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-21 17:30:10.000000 hipscat-0.3.3/tests/data/almanac_exception/bad_type.yml
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-05-21 17:30:10.000000 hipscat-0.3.3/tests/data/almanac_exception/index_missing_primary.yml
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-21 17:30:10.000000 hipscat-0.3.3/tests/data/almanac_exception/margin_missing_primary.yml
--rw-r--r--   0 runner    (1001) docker     (127)      343 2024-05-21 17:30:10.000000 hipscat-0.3.3/tests/data/almanac_exception/standalone_source_catalog.yml
--rw-r--r--   0 runner    (1001) docker     (127)    10017 2024-05-21 17:30:10.000000 hipscat-0.3.3/tests/data/generate_data.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:30:14.852486 hipscat-0.3.3/tests/data/info_only/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:30:14.876486 hipscat-0.3.3/tests/data/info_only/catalog/
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-05-21 17:30:10.000000 hipscat-0.3.3/tests/data/info_only/catalog/catalog_info.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:30:14.876486 hipscat-0.3.3/tests/data/info_only/dataset/
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-21 17:30:10.000000 hipscat-0.3.3/tests/data/info_only/dataset/catalog_info.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:30:14.876486 hipscat-0.3.3/tests/data/info_only/index_catalog/
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-21 17:30:10.000000 hipscat-0.3.3/tests/data/info_only/index_catalog/catalog_info.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:30:14.876486 hipscat-0.3.3/tests/data/info_only/margin_cache/
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-21 17:30:10.000000 hipscat-0.3.3/tests/data/info_only/margin_cache/catalog_info.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:30:14.880486 hipscat-0.3.3/tests/data/small_sky/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:30:14.852486 hipscat-0.3.3/tests/data/small_sky/Norder=0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:30:14.880486 hipscat-0.3.3/tests/data/small_sky/Norder=0/Dir=0/
--rw-r--r--   0 runner    (1001) docker     (127)     8880 2024-05-21 17:30:10.000000 hipscat-0.3.3/tests/data/small_sky/Norder=0/Dir=0/Npix=11.parquet
--rw-r--r--   0 runner    (1001) docker     (127)     4018 2024-05-21 17:30:10.000000 hipscat-0.3.3/tests/data/small_sky/_common_metadata
--rw-r--r--   0 runner    (1001) docker     (127)     5130 2024-05-21 17:30:10.000000 hipscat-0.3.3/tests/data/small_sky/_metadata
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-21 17:30:10.000000 hipscat-0.3.3/tests/data/small_sky/catalog_info.json
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-21 17:30:10.000000 hipscat-0.3.3/tests/data/small_sky/partition_info.csv
--rw-r--r--   0 runner    (1001) docker     (127)  1581120 2024-05-21 17:30:10.000000 hipscat-0.3.3/tests/data/small_sky/point_map.fits
--rw-r--r--   0 runner    (1001) docker     (127)     1873 2024-05-21 17:30:10.000000 hipscat-0.3.3/tests/data/small_sky/provenance_info.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:30:14.880486 hipscat-0.3.3/tests/data/small_sky_order1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:30:14.852486 hipscat-0.3.3/tests/data/small_sky_order1/Norder=1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:30:14.880486 hipscat-0.3.3/tests/data/small_sky_order1/Norder=1/Dir=0/
--rw-r--r--   0 runner    (1001) docker     (127)     7210 2024-05-21 17:30:10.000000 hipscat-0.3.3/tests/data/small_sky_order1/Norder=1/Dir=0/Npix=44.parquet
--rw-r--r--   0 runner    (1001) docker     (127)     6973 2024-05-21 17:30:10.000000 hipscat-0.3.3/tests/data/small_sky_order1/Norder=1/Dir=0/Npix=45.parquet
--rw-r--r--   0 runner    (1001) docker     (127)     7216 2024-05-21 17:30:10.000000 hipscat-0.3.3/tests/data/small_sky_order1/Norder=1/Dir=0/Npix=46.parquet
--rw-r--r--   0 runner    (1001) docker     (127)     6741 2024-05-21 17:30:10.000000 hipscat-0.3.3/tests/data/small_sky_order1/Norder=1/Dir=0/Npix=47.parquet
--rw-r--r--   0 runner    (1001) docker     (127)      936 2024-05-21 17:30:10.000000 hipscat-0.3.3/tests/data/small_sky_order1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     4018 2024-05-21 17:30:10.000000 hipscat-0.3.3/tests/data/small_sky_order1/_common_metadata
--rw-r--r--   0 runner    (1001) docker     (127)     8423 2024-05-21 17:30:10.000000 hipscat-0.3.3/tests/data/small_sky_order1/_metadata
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-21 17:30:10.000000 hipscat-0.3.3/tests/data/small_sky_order1/catalog_info.json
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-21 17:30:10.000000 hipscat-0.3.3/tests/data/small_sky_order1/partition_info.csv
--rw-r--r--   0 runner    (1001) docker     (127)     8640 2024-05-21 17:30:10.000000 hipscat-0.3.3/tests/data/small_sky_order1/point_map.fits
--rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-05-21 17:30:10.000000 hipscat-0.3.3/tests/data/small_sky_order1/provenance_info.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:30:14.884486 hipscat-0.3.3/tests/data/small_sky_order1_id_index/
--rw-r--r--   0 runner    (1001) docker     (127)     2224 2024-05-21 17:30:10.000000 hipscat-0.3.3/tests/data/small_sky_order1_id_index/_common_metadata
--rw-r--r--   0 runner    (1001) docker     (127)     2649 2024-05-21 17:30:10.000000 hipscat-0.3.3/tests/data/small_sky_order1_id_index/_metadata
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-21 17:30:10.000000 hipscat-0.3.3/tests/data/small_sky_order1_id_index/catalog_info.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:30:14.884486 hipscat-0.3.3/tests/data/small_sky_order1_id_index/index/
--rw-r--r--   0 runner    (1001) docker     (127)     3867 2024-05-21 17:30:10.000000 hipscat-0.3.3/tests/data/small_sky_order1_id_index/index/part.0.parquet
--rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-05-21 17:30:10.000000 hipscat-0.3.3/tests/data/small_sky_order1_id_index/provenance_info.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:30:14.884486 hipscat-0.3.3/tests/data/small_sky_order1_margin/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:30:14.852486 hipscat-0.3.3/tests/data/small_sky_order1_margin/Norder=0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:30:14.884486 hipscat-0.3.3/tests/data/small_sky_order1_margin/Norder=0/Dir=0/
--rw-r--r--   0 runner    (1001) docker     (127)     8255 2024-05-21 17:30:10.000000 hipscat-0.3.3/tests/data/small_sky_order1_margin/Norder=0/Dir=0/Npix=4.parquet
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:30:14.852486 hipscat-0.3.3/tests/data/small_sky_order1_margin/Norder=1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:30:14.884486 hipscat-0.3.3/tests/data/small_sky_order1_margin/Norder=1/Dir=0/
--rw-r--r--   0 runner    (1001) docker     (127)     8434 2024-05-21 17:30:10.000000 hipscat-0.3.3/tests/data/small_sky_order1_margin/Norder=1/Dir=0/Npix=44.parquet
--rw-r--r--   0 runner    (1001) docker     (127)     8476 2024-05-21 17:30:10.000000 hipscat-0.3.3/tests/data/small_sky_order1_margin/Norder=1/Dir=0/Npix=45.parquet
--rw-r--r--   0 runner    (1001) docker     (127)     8378 2024-05-21 17:30:10.000000 hipscat-0.3.3/tests/data/small_sky_order1_margin/Norder=1/Dir=0/Npix=46.parquet
--rw-r--r--   0 runner    (1001) docker     (127)     8344 2024-05-21 17:30:10.000000 hipscat-0.3.3/tests/data/small_sky_order1_margin/Norder=1/Dir=0/Npix=47.parquet
--rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-05-21 17:30:10.000000 hipscat-0.3.3/tests/data/small_sky_order1_margin/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     5194 2024-05-21 17:30:10.000000 hipscat-0.3.3/tests/data/small_sky_order1_margin/_common_metadata
--rw-r--r--   0 runner    (1001) docker     (127)    12384 2024-05-21 17:30:10.000000 hipscat-0.3.3/tests/data/small_sky_order1_margin/_metadata
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-21 17:30:10.000000 hipscat-0.3.3/tests/data/small_sky_order1_margin/catalog_info.json
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-21 17:30:10.000000 hipscat-0.3.3/tests/data/small_sky_order1_margin/partition_info.csv
--rw-r--r--   0 runner    (1001) docker     (127)      942 2024-05-21 17:30:10.000000 hipscat-0.3.3/tests/data/small_sky_order1_margin/provenance_info.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:30:14.888486 hipscat-0.3.3/tests/data/small_sky_source/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:30:14.852486 hipscat-0.3.3/tests/data/small_sky_source/Norder=0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:30:14.888486 hipscat-0.3.3/tests/data/small_sky_source/Norder=0/Dir=0/
--rw-r--r--   0 runner    (1001) docker     (127)    11421 2024-05-21 17:30:10.000000 hipscat-0.3.3/tests/data/small_sky_source/Norder=0/Dir=0/Npix=4.parquet
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:30:14.852486 hipscat-0.3.3/tests/data/small_sky_source/Norder=1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:30:14.888486 hipscat-0.3.3/tests/data/small_sky_source/Norder=1/Dir=0/
--rw-r--r--   0 runner    (1001) docker     (127)   133671 2024-05-21 17:30:10.000000 hipscat-0.3.3/tests/data/small_sky_source/Norder=1/Dir=0/Npix=47.parquet
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:30:14.856486 hipscat-0.3.3/tests/data/small_sky_source/Norder=2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:30:14.892486 hipscat-0.3.3/tests/data/small_sky_source/Norder=2/Dir=0/
--rw-r--r--   0 runner    (1001) docker     (127)    28346 2024-05-21 17:30:10.000000 hipscat-0.3.3/tests/data/small_sky_source/Norder=2/Dir=0/Npix=176.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    86262 2024-05-21 17:30:10.000000 hipscat-0.3.3/tests/data/small_sky_source/Norder=2/Dir=0/Npix=177.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    92634 2024-05-21 17:30:10.000000 hipscat-0.3.3/tests/data/small_sky_source/Norder=2/Dir=0/Npix=178.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    99874 2024-05-21 17:30:10.000000 hipscat-0.3.3/tests/data/small_sky_source/Norder=2/Dir=0/Npix=179.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    42177 2024-05-21 17:30:10.000000 hipscat-0.3.3/tests/data/small_sky_source/Norder=2/Dir=0/Npix=180.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    54742 2024-05-21 17:30:10.000000 hipscat-0.3.3/tests/data/small_sky_source/Norder=2/Dir=0/Npix=181.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    72960 2024-05-21 17:30:10.000000 hipscat-0.3.3/tests/data/small_sky_source/Norder=2/Dir=0/Npix=182.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    67771 2024-05-21 17:30:10.000000 hipscat-0.3.3/tests/data/small_sky_source/Norder=2/Dir=0/Npix=183.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    80265 2024-05-21 17:30:10.000000 hipscat-0.3.3/tests/data/small_sky_source/Norder=2/Dir=0/Npix=184.parquet
--rw-r--r--   0 runner    (1001) docker     (127)   162064 2024-05-21 17:30:10.000000 hipscat-0.3.3/tests/data/small_sky_source/Norder=2/Dir=0/Npix=185.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    31761 2024-05-21 17:30:10.000000 hipscat-0.3.3/tests/data/small_sky_source/Norder=2/Dir=0/Npix=186.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    43705 2024-05-21 17:30:10.000000 hipscat-0.3.3/tests/data/small_sky_source/Norder=2/Dir=0/Npix=187.parquet
--rw-r--r--   0 runner    (1001) docker     (127)     5525 2024-05-21 17:30:10.000000 hipscat-0.3.3/tests/data/small_sky_source/_common_metadata
--rw-r--r--   0 runner    (1001) docker     (127)    28968 2024-05-21 17:30:10.000000 hipscat-0.3.3/tests/data/small_sky_source/_metadata
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-21 17:30:10.000000 hipscat-0.3.3/tests/data/small_sky_source/catalog_info.json
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-21 17:30:10.000000 hipscat-0.3.3/tests/data/small_sky_source/partition_info.csv
--rw-r--r--   0 runner    (1001) docker     (127)  1581120 2024-05-21 17:30:10.000000 hipscat-0.3.3/tests/data/small_sky_source/point_map.fits
--rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-05-21 17:30:10.000000 hipscat-0.3.3/tests/data/small_sky_source/provenance_info.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:30:14.892486 hipscat-0.3.3/tests/data/small_sky_source_object_index/
--rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-05-21 17:30:10.000000 hipscat-0.3.3/tests/data/small_sky_source_object_index/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2296 2024-05-21 17:30:10.000000 hipscat-0.3.3/tests/data/small_sky_source_object_index/_common_metadata
--rw-r--r--   0 runner    (1001) docker     (127)     2729 2024-05-21 17:30:10.000000 hipscat-0.3.3/tests/data/small_sky_source_object_index/_metadata
--rw-r--r--   0 runner    (1001) docker     (127)      212 2024-05-21 17:30:10.000000 hipscat-0.3.3/tests/data/small_sky_source_object_index/catalog_info.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:30:14.892486 hipscat-0.3.3/tests/data/small_sky_source_object_index/index/
--rw-r--r--   0 runner    (1001) docker     (127)     4153 2024-05-21 17:30:10.000000 hipscat-0.3.3/tests/data/small_sky_source_object_index/index/part.0.parquet
--rw-r--r--   0 runner    (1001) docker     (127)     1156 2024-05-21 17:30:10.000000 hipscat-0.3.3/tests/data/small_sky_source_object_index/provenance_info.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:30:14.892486 hipscat-0.3.3/tests/data/small_sky_to_small_sky_order1/
--rw-r--r--   0 runner    (1001) docker     (127)      556 2024-05-21 17:30:10.000000 hipscat-0.3.3/tests/data/small_sky_to_small_sky_order1/_common_metadata
--rw-r--r--   0 runner    (1001) docker     (127)     2929 2024-05-21 17:30:10.000000 hipscat-0.3.3/tests/data/small_sky_to_small_sky_order1/_metadata
--rw-r--r--   0 runner    (1001) docker     (127)      360 2024-05-21 17:30:10.000000 hipscat-0.3.3/tests/data/small_sky_to_small_sky_order1/catalog_info.json
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-21 17:30:10.000000 hipscat-0.3.3/tests/data/small_sky_to_small_sky_order1/partition_info.csv
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-21 17:30:10.000000 hipscat-0.3.3/tests/data/small_sky_to_small_sky_order1/partition_join_info.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:30:14.892486 hipscat-0.3.3/tests/hipscat/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:30:14.892486 hipscat-0.3.3/tests/hipscat/catalog/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:30:14.892486 hipscat-0.3.3/tests/hipscat/catalog/association_catalog/
--rw-r--r--   0 runner    (1001) docker     (127)     5552 2024-05-21 17:30:10.000000 hipscat-0.3.3/tests/hipscat/catalog/association_catalog/test_association_catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     2627 2024-05-21 17:30:10.000000 hipscat-0.3.3/tests/hipscat/catalog/association_catalog/test_association_catalog_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     6156 2024-05-21 17:30:10.000000 hipscat-0.3.3/tests/hipscat/catalog/association_catalog/test_partition_join_info.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:30:14.896486 hipscat-0.3.3/tests/hipscat/catalog/dataset/
--rw-r--r--   0 runner    (1001) docker     (127)     1595 2024-05-21 17:30:10.000000 hipscat-0.3.3/tests/hipscat/catalog/dataset/test_base_catalog_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     4896 2024-05-21 17:30:10.000000 hipscat-0.3.3/tests/hipscat/catalog/dataset/test_catalog_info_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-05-21 17:30:10.000000 hipscat-0.3.3/tests/hipscat/catalog/dataset/test_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:30:14.896486 hipscat-0.3.3/tests/hipscat/catalog/index/
--rw-r--r--   0 runner    (1001) docker     (127)      699 2024-05-21 17:30:10.000000 hipscat-0.3.3/tests/hipscat/catalog/index/test_index_catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     2636 2024-05-21 17:30:10.000000 hipscat-0.3.3/tests/hipscat/catalog/index/test_index_catalog_info.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:30:14.896486 hipscat-0.3.3/tests/hipscat/catalog/loaders/
--rw-r--r--   0 runner    (1001) docker     (127)      444 2024-05-21 17:30:10.000000 hipscat-0.3.3/tests/hipscat/catalog/loaders/test_read_from_hipscat.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:30:14.896486 hipscat-0.3.3/tests/hipscat/catalog/margin_cache/
--rw-r--r--   0 runner    (1001) docker     (127)     2586 2024-05-21 17:30:10.000000 hipscat-0.3.3/tests/hipscat/catalog/margin_cache/test_margin_cache_catalog_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     3115 2024-05-21 17:30:10.000000 hipscat-0.3.3/tests/hipscat/catalog/margin_cache/test_margin_catalog.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:30:14.896486 hipscat-0.3.3/tests/hipscat/catalog/source_catalog/
--rw-r--r--   0 runner    (1001) docker     (127)     2645 2024-05-21 17:30:10.000000 hipscat-0.3.3/tests/hipscat/catalog/source_catalog/test_source_catalog_info.py
--rw-r--r--   0 runner    (1001) docker     (127)    22579 2024-05-21 17:30:10.000000 hipscat-0.3.3/tests/hipscat/catalog/test_catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     1579 2024-05-21 17:30:10.000000 hipscat-0.3.3/tests/hipscat/catalog/test_catalog_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     6742 2024-05-21 17:30:10.000000 hipscat-0.3.3/tests/hipscat/catalog/test_partition_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     1986 2024-05-21 17:30:10.000000 hipscat-0.3.3/tests/hipscat/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:30:14.896486 hipscat-0.3.3/tests/hipscat/inspection/
--rw-r--r--   0 runner    (1001) docker     (127)     7492 2024-05-21 17:30:10.000000 hipscat-0.3.3/tests/hipscat/inspection/test_almanac.py
--rw-r--r--   0 runner    (1001) docker     (127)     3550 2024-05-21 17:30:10.000000 hipscat-0.3.3/tests/hipscat/inspection/test_almanac_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     2775 2024-05-21 17:30:10.000000 hipscat-0.3.3/tests/hipscat/inspection/test_visualize_catalog.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:30:14.896486 hipscat-0.3.3/tests/hipscat/io/
--rw-r--r--   0 runner    (1001) docker     (127)     3654 2024-05-21 17:30:10.000000 hipscat-0.3.3/tests/hipscat/io/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:30:14.896486 hipscat-0.3.3/tests/hipscat/io/file_io/
--rw-r--r--   0 runner    (1001) docker     (127)     4488 2024-05-21 17:30:10.000000 hipscat-0.3.3/tests/hipscat/io/file_io/test_file_io.py
--rw-r--r--   0 runner    (1001) docker     (127)     5396 2024-05-21 17:30:10.000000 hipscat-0.3.3/tests/hipscat/io/file_io/test_file_pointers.py
--rw-r--r--   0 runner    (1001) docker     (127)     8508 2024-05-21 17:30:10.000000 hipscat-0.3.3/tests/hipscat/io/test_parquet_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     2290 2024-05-21 17:30:10.000000 hipscat-0.3.3/tests/hipscat/io/test_paths.py
--rw-r--r--   0 runner    (1001) docker     (127)     1459 2024-05-21 17:30:10.000000 hipscat-0.3.3/tests/hipscat/io/test_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)     7326 2024-05-21 17:30:10.000000 hipscat-0.3.3/tests/hipscat/io/test_write_metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:30:14.896486 hipscat-0.3.3/tests/hipscat/pixel_math/
--rw-r--r--   0 runner    (1001) docker     (127)     3203 2024-05-21 17:30:10.000000 hipscat-0.3.3/tests/hipscat/pixel_math/test_healpix_pixel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-05-21 17:30:10.000000 hipscat-0.3.3/tests/hipscat/pixel_math/test_healpix_pixel_convertor.py
--rw-r--r--   0 runner    (1001) docker     (127)      739 2024-05-21 17:30:10.000000 hipscat-0.3.3/tests/hipscat/pixel_math/test_healpix_pixel_function.py
--rw-r--r--   0 runner    (1001) docker     (127)     5361 2024-05-21 17:30:10.000000 hipscat-0.3.3/tests/hipscat/pixel_math/test_hipscat_id.py
--rw-r--r--   0 runner    (1001) docker     (127)     2745 2024-05-21 17:30:10.000000 hipscat-0.3.3/tests/hipscat/pixel_math/test_margin_bounding.py
--rw-r--r--   0 runner    (1001) docker     (127)    10360 2024-05-21 17:30:10.000000 hipscat-0.3.3/tests/hipscat/pixel_math/test_partition_stats.py
--rw-r--r--   0 runner    (1001) docker     (127)     3789 2024-05-21 17:30:10.000000 hipscat-0.3.3/tests/hipscat/pixel_math/test_pixel_margins.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:30:14.900486 hipscat-0.3.3/tests/hipscat/pixel_tree/
--rw-r--r--   0 runner    (1001) docker     (127)     3395 2024-05-21 17:30:10.000000 hipscat-0.3.3/tests/hipscat/pixel_tree/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1800 2024-05-21 17:30:10.000000 hipscat-0.3.3/tests/hipscat/pixel_tree/test_moc_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)    12040 2024-05-21 17:30:10.000000 hipscat-0.3.3/tests/hipscat/pixel_tree/test_pixel_alignment.py
--rw-r--r--   0 runner    (1001) docker     (127)     1917 2024-05-21 17:30:10.000000 hipscat-0.3.3/tests/hipscat/pixel_tree/test_pixel_tree.py
--rw-r--r--   0 runner    (1001) docker     (127)     2265 2024-05-21 17:30:10.000000 hipscat-0.3.3/tests/hipscat/pixel_tree/test_pixel_tree_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:26:02.384830 hipscat-0.3.4/
+-rw-r--r--   0 runner    (1001) docker     (127)      558 2024-05-31 17:25:57.000000 hipscat-0.3.4/.copier-answers.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-31 17:25:57.000000 hipscat-0.3.4/.git_archival.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      747 2024-05-31 17:25:57.000000 hipscat-0.3.4/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:26:02.336830 hipscat-0.3.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:26:02.336830 hipscat-0.3.4/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-31 17:25:57.000000 hipscat-0.3.4/.github/ISSUE_TEMPLATE/0-general_issue.md
+-rw-r--r--   0 runner    (1001) docker     (127)      660 2024-05-31 17:25:57.000000 hipscat-0.3.4/.github/ISSUE_TEMPLATE/1-bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      706 2024-05-31 17:25:57.000000 hipscat-0.3.4/.github/ISSUE_TEMPLATE/2-feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-31 17:25:57.000000 hipscat-0.3.4/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3329 2024-05-31 17:25:57.000000 hipscat-0.3.4/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:26:02.340829 hipscat-0.3.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2024-05-31 17:25:57.000000 hipscat-0.3.4/.github/workflows/add-issue-to-project-tracker.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2697 2024-05-31 17:25:57.000000 hipscat-0.3.4/.github/workflows/asv-main.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2839 2024-05-31 17:25:57.000000 hipscat-0.3.4/.github/workflows/asv-nightly.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3057 2024-05-31 17:25:57.000000 hipscat-0.3.4/.github/workflows/asv-pr.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      929 2024-05-31 17:25:57.000000 hipscat-0.3.4/.github/workflows/build-documentation.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-05-31 17:25:57.000000 hipscat-0.3.4/.github/workflows/pre-commit-ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2065 2024-05-31 17:25:57.000000 hipscat-0.3.4/.github/workflows/publish-benchmarks-pr.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      951 2024-05-31 17:25:57.000000 hipscat-0.3.4/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2359 2024-05-31 17:25:57.000000 hipscat-0.3.4/.github/workflows/smoke-test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-05-31 17:25:57.000000 hipscat-0.3.4/.github/workflows/testing-and-coverage.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-05-31 17:25:57.000000 hipscat-0.3.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     5366 2024-05-31 17:25:57.000000 hipscat-0.3.4/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-05-31 17:25:57.000000 hipscat-0.3.4/.prepare_project.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-31 17:25:57.000000 hipscat-0.3.4/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1539 2024-05-31 17:25:57.000000 hipscat-0.3.4/.setup_dev.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-05-31 17:25:57.000000 hipscat-0.3.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5975 2024-05-31 17:26:02.384830 hipscat-0.3.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2860 2024-05-31 17:25:57.000000 hipscat-0.3.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:26:02.340829 hipscat-0.3.4/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 17:25:57.000000 hipscat-0.3.4/benchmarks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3597 2024-05-31 17:25:57.000000 hipscat-0.3.4/benchmarks/asv.conf.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4950 2024-05-31 17:25:57.000000 hipscat-0.3.4/benchmarks/benchmarks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:26:02.340829 hipscat-0.3.4/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-05-31 17:25:57.000000 hipscat-0.3.4/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:26:02.340829 hipscat-0.3.4/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-31 17:25:57.000000 hipscat-0.3.4/docs/_static/custom.css
+-rw-r--r--   0 runner    (1001) docker     (127)     2151 2024-05-31 17:25:57.000000 hipscat-0.3.4/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:26:02.340829 hipscat-0.3.4/docs/guide/
+-rw-r--r--   0 runner    (1001) docker     (127)     4409 2024-05-31 17:25:57.000000 hipscat-0.3.4/docs/guide/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-05-31 17:25:57.000000 hipscat-0.3.4/docs/guide/directory_scheme.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    17649 2024-05-31 17:25:57.000000 hipscat-0.3.4/docs/guide/margin_cache_diagram.png
+-rw-r--r--   0 runner    (1001) docker     (127)    12890 2024-05-31 17:25:57.000000 hipscat-0.3.4/docs/guide/pixel_math.md
+-rw-r--r--   0 runner    (1001) docker     (127)      923 2024-05-31 17:25:57.000000 hipscat-0.3.4/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:26:02.340829 hipscat-0.3.4/docs/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (127)     4988 2024-05-31 17:25:57.000000 hipscat-0.3.4/docs/notebooks/catalog_size_inspection.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     2303 2024-05-31 17:25:57.000000 hipscat-0.3.4/docs/notebooks/cone_search.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-31 17:25:57.000000 hipscat-0.3.4/docs/notebooks.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-31 17:25:57.000000 hipscat-0.3.4/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2839 2024-05-31 17:25:57.000000 hipscat-0.3.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 17:26:02.384830 hipscat-0.3.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:26:02.340829 hipscat-0.3.4/src/
+-rw-r--r--   0 runner    (1001) docker     (127)    20824 2024-05-31 17:25:57.000000 hipscat-0.3.4/src/.pylintrc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:26:02.344829 hipscat-0.3.4/src/hipscat/
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-31 17:25:57.000000 hipscat-0.3.4/src/hipscat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-31 17:26:02.000000 hipscat-0.3.4/src/hipscat/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:26:02.344829 hipscat-0.3.4/src/hipscat/catalog/
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-05-31 17:25:57.000000 hipscat-0.3.4/src/hipscat/catalog/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:26:02.344829 hipscat-0.3.4/src/hipscat/catalog/association_catalog/
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-05-31 17:25:57.000000 hipscat-0.3.4/src/hipscat/catalog/association_catalog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3883 2024-05-31 17:25:57.000000 hipscat-0.3.4/src/hipscat/catalog/association_catalog/association_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-05-31 17:25:57.000000 hipscat-0.3.4/src/hipscat/catalog/association_catalog/association_catalog_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13211 2024-05-31 17:25:57.000000 hipscat-0.3.4/src/hipscat/catalog/association_catalog/partition_join_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6069 2024-05-31 17:25:57.000000 hipscat-0.3.4/src/hipscat/catalog/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2024-05-31 17:25:57.000000 hipscat-0.3.4/src/hipscat/catalog/catalog_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-05-31 17:25:57.000000 hipscat-0.3.4/src/hipscat/catalog/catalog_type.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:26:02.344829 hipscat-0.3.4/src/hipscat/catalog/dataset/
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-31 17:25:57.000000 hipscat-0.3.4/src/hipscat/catalog/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2768 2024-05-31 17:25:57.000000 hipscat-0.3.4/src/hipscat/catalog/dataset/base_catalog_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3318 2024-05-31 17:25:57.000000 hipscat-0.3.4/src/hipscat/catalog/dataset/catalog_info_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3512 2024-05-31 17:25:57.000000 hipscat-0.3.4/src/hipscat/catalog/dataset/dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:26:02.348830 hipscat-0.3.4/src/hipscat/catalog/healpix_dataset/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 17:25:57.000000 hipscat-0.3.4/src/hipscat/catalog/healpix_dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9517 2024-05-31 17:25:57.000000 hipscat-0.3.4/src/hipscat/catalog/healpix_dataset/healpix_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:26:02.348830 hipscat-0.3.4/src/hipscat/catalog/index/
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-31 17:25:57.000000 hipscat-0.3.4/src/hipscat/catalog/index/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2758 2024-05-31 17:25:57.000000 hipscat-0.3.4/src/hipscat/catalog/index/index_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-05-31 17:25:57.000000 hipscat-0.3.4/src/hipscat/catalog/index/index_catalog_info.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:26:02.348830 hipscat-0.3.4/src/hipscat/catalog/margin_cache/
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-31 17:25:57.000000 hipscat-0.3.4/src/hipscat/catalog/margin_cache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      710 2024-05-31 17:25:57.000000 hipscat-0.3.4/src/hipscat/catalog/margin_cache/margin_cache_catalog_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3499 2024-05-31 17:25:57.000000 hipscat-0.3.4/src/hipscat/catalog/margin_cache/margin_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11819 2024-05-31 17:25:57.000000 hipscat-0.3.4/src/hipscat/catalog/partition_info.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:26:02.348830 hipscat-0.3.4/src/hipscat/catalog/source_catalog/
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-31 17:25:57.000000 hipscat-0.3.4/src/hipscat/catalog/source_catalog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      906 2024-05-31 17:25:57.000000 hipscat-0.3.4/src/hipscat/catalog/source_catalog/source_catalog_info.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:26:02.348830 hipscat-0.3.4/src/hipscat/inspection/
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-31 17:25:57.000000 hipscat-0.3.4/src/hipscat/inspection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11751 2024-05-31 17:25:57.000000 hipscat-0.3.4/src/hipscat/inspection/almanac.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5457 2024-05-31 17:25:57.000000 hipscat-0.3.4/src/hipscat/inspection/almanac_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5462 2024-05-31 17:25:57.000000 hipscat-0.3.4/src/hipscat/inspection/visualize_catalog.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:26:02.348830 hipscat-0.3.4/src/hipscat/io/
+-rw-r--r--   0 runner    (1001) docker     (127)      714 2024-05-31 17:25:57.000000 hipscat-0.3.4/src/hipscat/io/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:26:02.348830 hipscat-0.3.4/src/hipscat/io/file_io/
+-rw-r--r--   0 runner    (1001) docker     (127)      815 2024-05-31 17:25:57.000000 hipscat-0.3.4/src/hipscat/io/file_io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13206 2024-05-31 17:25:57.000000 hipscat-0.3.4/src/hipscat/io/file_io/file_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8215 2024-05-31 17:25:57.000000 hipscat-0.3.4/src/hipscat/io/file_io/file_pointer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7498 2024-05-31 17:25:57.000000 hipscat-0.3.4/src/hipscat/io/parquet_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9634 2024-05-31 17:25:57.000000 hipscat-0.3.4/src/hipscat/io/paths.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2855 2024-05-31 17:25:57.000000 hipscat-0.3.4/src/hipscat/io/validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6104 2024-05-31 17:25:57.000000 hipscat-0.3.4/src/hipscat/io/write_metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:26:02.352830 hipscat-0.3.4/src/hipscat/loaders/
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-31 17:25:57.000000 hipscat-0.3.4/src/hipscat/loaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2404 2024-05-31 17:25:57.000000 hipscat-0.3.4/src/hipscat/loaders/read_from_hipscat.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:26:02.352830 hipscat-0.3.4/src/hipscat/pixel_math/
+-rw-r--r--   0 runner    (1001) docker     (127)      546 2024-05-31 17:25:57.000000 hipscat-0.3.4/src/hipscat/pixel_math/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4890 2024-05-31 17:25:57.000000 hipscat-0.3.4/src/hipscat/pixel_math/box_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-05-31 17:25:57.000000 hipscat-0.3.4/src/hipscat/pixel_math/cone_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-05-31 17:25:57.000000 hipscat-0.3.4/src/hipscat/pixel_math/filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4979 2024-05-31 17:25:57.000000 hipscat-0.3.4/src/hipscat/pixel_math/healpix_pixel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-05-31 17:25:57.000000 hipscat-0.3.4/src/hipscat/pixel_math/healpix_pixel_convertor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2203 2024-05-31 17:25:57.000000 hipscat-0.3.4/src/hipscat/pixel_math/healpix_pixel_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4311 2024-05-31 17:25:57.000000 hipscat-0.3.4/src/hipscat/pixel_math/hipscat_id.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5651 2024-05-31 17:25:57.000000 hipscat-0.3.4/src/hipscat/pixel_math/margin_bounding.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12354 2024-05-31 17:25:57.000000 hipscat-0.3.4/src/hipscat/pixel_math/partition_stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4807 2024-05-31 17:25:57.000000 hipscat-0.3.4/src/hipscat/pixel_math/pixel_margins.py
+-rw-r--r--   0 runner    (1001) docker     (127)      976 2024-05-31 17:25:57.000000 hipscat-0.3.4/src/hipscat/pixel_math/polygon_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4185 2024-05-31 17:25:57.000000 hipscat-0.3.4/src/hipscat/pixel_math/validators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:26:02.356830 hipscat-0.3.4/src/hipscat/pixel_tree/
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-31 17:25:57.000000 hipscat-0.3.4/src/hipscat/pixel_tree/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2153 2024-05-31 17:25:57.000000 hipscat-0.3.4/src/hipscat/pixel_tree/moc_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-05-31 17:25:57.000000 hipscat-0.3.4/src/hipscat/pixel_tree/moc_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      961 2024-05-31 17:25:57.000000 hipscat-0.3.4/src/hipscat/pixel_tree/negative_tree.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19695 2024-05-31 17:25:57.000000 hipscat-0.3.4/src/hipscat/pixel_tree/pixel_alignment.py
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-05-31 17:25:57.000000 hipscat-0.3.4/src/hipscat/pixel_tree/pixel_alignment_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4367 2024-05-31 17:25:57.000000 hipscat-0.3.4/src/hipscat/pixel_tree/pixel_tree.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 17:25:57.000000 hipscat-0.3.4/src/hipscat/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:26:02.380830 hipscat-0.3.4/src/hipscat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5975 2024-05-31 17:26:02.000000 hipscat-0.3.4/src/hipscat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10111 2024-05-31 17:26:02.000000 hipscat-0.3.4/src/hipscat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 17:26:02.000000 hipscat-0.3.4/src/hipscat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-05-31 17:26:02.000000 hipscat-0.3.4/src/hipscat.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-31 17:26:02.000000 hipscat-0.3.4/src/hipscat.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:26:02.356830 hipscat-0.3.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    20985 2024-05-31 17:25:57.000000 hipscat-0.3.4/tests/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (127)     8358 2024-05-31 17:25:57.000000 hipscat-0.3.4/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:26:02.356830 hipscat-0.3.4/tests/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:26:02.356830 hipscat-0.3.4/tests/data/almanac/
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-31 17:25:57.000000 hipscat-0.3.4/tests/data/almanac/deprecated.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-05-31 17:25:57.000000 hipscat-0.3.4/tests/data/almanac/small_sky.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-31 17:25:57.000000 hipscat-0.3.4/tests/data/almanac/small_sky_order1.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-05-31 17:25:57.000000 hipscat-0.3.4/tests/data/almanac/small_sky_order1_id_index.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      328 2024-05-31 17:25:57.000000 hipscat-0.3.4/tests/data/almanac/small_sky_order1_margin.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-05-31 17:25:57.000000 hipscat-0.3.4/tests/data/almanac/small_sky_source.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-31 17:25:57.000000 hipscat-0.3.4/tests/data/almanac/small_sky_source_object_index.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-05-31 17:25:57.000000 hipscat-0.3.4/tests/data/almanac/small_sky_to_small_sky_order1.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:26:02.356830 hipscat-0.3.4/tests/data/almanac_exception/
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-05-31 17:25:57.000000 hipscat-0.3.4/tests/data/almanac_exception/association_missing_join.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-31 17:25:57.000000 hipscat-0.3.4/tests/data/almanac_exception/association_missing_primary.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-31 17:25:57.000000 hipscat-0.3.4/tests/data/almanac_exception/bad_catalog_path.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-31 17:25:57.000000 hipscat-0.3.4/tests/data/almanac_exception/bad_primary_path.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-31 17:25:57.000000 hipscat-0.3.4/tests/data/almanac_exception/bad_type.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-05-31 17:25:57.000000 hipscat-0.3.4/tests/data/almanac_exception/index_missing_primary.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-31 17:25:57.000000 hipscat-0.3.4/tests/data/almanac_exception/margin_missing_primary.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-05-31 17:25:57.000000 hipscat-0.3.4/tests/data/almanac_exception/standalone_source_catalog.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    10110 2024-05-31 17:25:57.000000 hipscat-0.3.4/tests/data/generate_data.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:26:02.328829 hipscat-0.3.4/tests/data/info_only/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:26:02.356830 hipscat-0.3.4/tests/data/info_only/catalog/
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-05-31 17:25:57.000000 hipscat-0.3.4/tests/data/info_only/catalog/catalog_info.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:26:02.360829 hipscat-0.3.4/tests/data/info_only/dataset/
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-31 17:25:57.000000 hipscat-0.3.4/tests/data/info_only/dataset/catalog_info.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:26:02.360829 hipscat-0.3.4/tests/data/info_only/index_catalog/
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-31 17:25:57.000000 hipscat-0.3.4/tests/data/info_only/index_catalog/catalog_info.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:26:02.360829 hipscat-0.3.4/tests/data/info_only/margin_cache/
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-31 17:25:57.000000 hipscat-0.3.4/tests/data/info_only/margin_cache/catalog_info.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:26:02.360829 hipscat-0.3.4/tests/data/small_sky/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:26:02.328829 hipscat-0.3.4/tests/data/small_sky/Norder=0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:26:02.360829 hipscat-0.3.4/tests/data/small_sky/Norder=0/Dir=0/
+-rw-r--r--   0 runner    (1001) docker     (127)     8880 2024-05-31 17:25:57.000000 hipscat-0.3.4/tests/data/small_sky/Norder=0/Dir=0/Npix=11.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)     4018 2024-05-31 17:25:57.000000 hipscat-0.3.4/tests/data/small_sky/_common_metadata
+-rw-r--r--   0 runner    (1001) docker     (127)     5130 2024-05-31 17:25:57.000000 hipscat-0.3.4/tests/data/small_sky/_metadata
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-31 17:25:57.000000 hipscat-0.3.4/tests/data/small_sky/catalog_info.json
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-31 17:25:57.000000 hipscat-0.3.4/tests/data/small_sky/partition_info.csv
+-rw-r--r--   0 runner    (1001) docker     (127)  1581120 2024-05-31 17:25:57.000000 hipscat-0.3.4/tests/data/small_sky/point_map.fits
+-rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-05-31 17:25:57.000000 hipscat-0.3.4/tests/data/small_sky/provenance_info.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:26:02.364830 hipscat-0.3.4/tests/data/small_sky_order1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:26:02.328829 hipscat-0.3.4/tests/data/small_sky_order1/Norder=1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:26:02.364830 hipscat-0.3.4/tests/data/small_sky_order1/Norder=1/Dir=0/
+-rw-r--r--   0 runner    (1001) docker     (127)     7210 2024-05-31 17:25:57.000000 hipscat-0.3.4/tests/data/small_sky_order1/Norder=1/Dir=0/Npix=44.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)     6973 2024-05-31 17:25:57.000000 hipscat-0.3.4/tests/data/small_sky_order1/Norder=1/Dir=0/Npix=45.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)     7216 2024-05-31 17:25:57.000000 hipscat-0.3.4/tests/data/small_sky_order1/Norder=1/Dir=0/Npix=46.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)     6741 2024-05-31 17:25:57.000000 hipscat-0.3.4/tests/data/small_sky_order1/Norder=1/Dir=0/Npix=47.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)      936 2024-05-31 17:25:57.000000 hipscat-0.3.4/tests/data/small_sky_order1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4018 2024-05-31 17:25:57.000000 hipscat-0.3.4/tests/data/small_sky_order1/_common_metadata
+-rw-r--r--   0 runner    (1001) docker     (127)     8423 2024-05-31 17:25:57.000000 hipscat-0.3.4/tests/data/small_sky_order1/_metadata
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-31 17:25:57.000000 hipscat-0.3.4/tests/data/small_sky_order1/catalog_info.json
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-31 17:25:57.000000 hipscat-0.3.4/tests/data/small_sky_order1/partition_info.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     8640 2024-05-31 17:25:57.000000 hipscat-0.3.4/tests/data/small_sky_order1/point_map.fits
+-rw-r--r--   0 runner    (1001) docker     (127)     1895 2024-05-31 17:25:57.000000 hipscat-0.3.4/tests/data/small_sky_order1/provenance_info.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:26:02.364830 hipscat-0.3.4/tests/data/small_sky_order1_id_index/
+-rw-r--r--   0 runner    (1001) docker     (127)     2224 2024-05-31 17:25:57.000000 hipscat-0.3.4/tests/data/small_sky_order1_id_index/_common_metadata
+-rw-r--r--   0 runner    (1001) docker     (127)     2649 2024-05-31 17:25:57.000000 hipscat-0.3.4/tests/data/small_sky_order1_id_index/_metadata
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-31 17:25:57.000000 hipscat-0.3.4/tests/data/small_sky_order1_id_index/catalog_info.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:26:02.364830 hipscat-0.3.4/tests/data/small_sky_order1_id_index/index/
+-rw-r--r--   0 runner    (1001) docker     (127)     3867 2024-05-31 17:25:57.000000 hipscat-0.3.4/tests/data/small_sky_order1_id_index/index/part.0.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-31 17:25:57.000000 hipscat-0.3.4/tests/data/small_sky_order1_id_index/provenance_info.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:26:02.364830 hipscat-0.3.4/tests/data/small_sky_order1_margin/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:26:02.332829 hipscat-0.3.4/tests/data/small_sky_order1_margin/Norder=0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:26:02.364830 hipscat-0.3.4/tests/data/small_sky_order1_margin/Norder=0/Dir=0/
+-rw-r--r--   0 runner    (1001) docker     (127)     8255 2024-05-31 17:25:57.000000 hipscat-0.3.4/tests/data/small_sky_order1_margin/Norder=0/Dir=0/Npix=4.parquet
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:26:02.332829 hipscat-0.3.4/tests/data/small_sky_order1_margin/Norder=1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:26:02.368830 hipscat-0.3.4/tests/data/small_sky_order1_margin/Norder=1/Dir=0/
+-rw-r--r--   0 runner    (1001) docker     (127)     8434 2024-05-31 17:25:57.000000 hipscat-0.3.4/tests/data/small_sky_order1_margin/Norder=1/Dir=0/Npix=44.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)     8476 2024-05-31 17:25:57.000000 hipscat-0.3.4/tests/data/small_sky_order1_margin/Norder=1/Dir=0/Npix=45.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)     8378 2024-05-31 17:25:57.000000 hipscat-0.3.4/tests/data/small_sky_order1_margin/Norder=1/Dir=0/Npix=46.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)     8344 2024-05-31 17:25:57.000000 hipscat-0.3.4/tests/data/small_sky_order1_margin/Norder=1/Dir=0/Npix=47.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-05-31 17:25:57.000000 hipscat-0.3.4/tests/data/small_sky_order1_margin/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5194 2024-05-31 17:25:57.000000 hipscat-0.3.4/tests/data/small_sky_order1_margin/_common_metadata
+-rw-r--r--   0 runner    (1001) docker     (127)    12384 2024-05-31 17:25:57.000000 hipscat-0.3.4/tests/data/small_sky_order1_margin/_metadata
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-31 17:25:57.000000 hipscat-0.3.4/tests/data/small_sky_order1_margin/catalog_info.json
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-31 17:25:57.000000 hipscat-0.3.4/tests/data/small_sky_order1_margin/partition_info.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      961 2024-05-31 17:25:57.000000 hipscat-0.3.4/tests/data/small_sky_order1_margin/provenance_info.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:26:02.368830 hipscat-0.3.4/tests/data/small_sky_source/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:26:02.332829 hipscat-0.3.4/tests/data/small_sky_source/Norder=0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:26:02.368830 hipscat-0.3.4/tests/data/small_sky_source/Norder=0/Dir=0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11421 2024-05-31 17:25:57.000000 hipscat-0.3.4/tests/data/small_sky_source/Norder=0/Dir=0/Npix=4.parquet
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:26:02.332829 hipscat-0.3.4/tests/data/small_sky_source/Norder=1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:26:02.368830 hipscat-0.3.4/tests/data/small_sky_source/Norder=1/Dir=0/
+-rw-r--r--   0 runner    (1001) docker     (127)   133671 2024-05-31 17:25:57.000000 hipscat-0.3.4/tests/data/small_sky_source/Norder=1/Dir=0/Npix=47.parquet
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:26:02.332829 hipscat-0.3.4/tests/data/small_sky_source/Norder=2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:26:02.372830 hipscat-0.3.4/tests/data/small_sky_source/Norder=2/Dir=0/
+-rw-r--r--   0 runner    (1001) docker     (127)    28346 2024-05-31 17:25:57.000000 hipscat-0.3.4/tests/data/small_sky_source/Norder=2/Dir=0/Npix=176.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    86262 2024-05-31 17:25:57.000000 hipscat-0.3.4/tests/data/small_sky_source/Norder=2/Dir=0/Npix=177.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    92634 2024-05-31 17:25:57.000000 hipscat-0.3.4/tests/data/small_sky_source/Norder=2/Dir=0/Npix=178.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    99874 2024-05-31 17:25:57.000000 hipscat-0.3.4/tests/data/small_sky_source/Norder=2/Dir=0/Npix=179.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    42177 2024-05-31 17:25:57.000000 hipscat-0.3.4/tests/data/small_sky_source/Norder=2/Dir=0/Npix=180.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    54742 2024-05-31 17:25:57.000000 hipscat-0.3.4/tests/data/small_sky_source/Norder=2/Dir=0/Npix=181.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    72960 2024-05-31 17:25:57.000000 hipscat-0.3.4/tests/data/small_sky_source/Norder=2/Dir=0/Npix=182.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    67771 2024-05-31 17:25:57.000000 hipscat-0.3.4/tests/data/small_sky_source/Norder=2/Dir=0/Npix=183.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    80265 2024-05-31 17:25:57.000000 hipscat-0.3.4/tests/data/small_sky_source/Norder=2/Dir=0/Npix=184.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)   162064 2024-05-31 17:25:57.000000 hipscat-0.3.4/tests/data/small_sky_source/Norder=2/Dir=0/Npix=185.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    31761 2024-05-31 17:25:57.000000 hipscat-0.3.4/tests/data/small_sky_source/Norder=2/Dir=0/Npix=186.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    43705 2024-05-31 17:25:57.000000 hipscat-0.3.4/tests/data/small_sky_source/Norder=2/Dir=0/Npix=187.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)     5525 2024-05-31 17:25:57.000000 hipscat-0.3.4/tests/data/small_sky_source/_common_metadata
+-rw-r--r--   0 runner    (1001) docker     (127)    28968 2024-05-31 17:25:57.000000 hipscat-0.3.4/tests/data/small_sky_source/_metadata
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-31 17:25:57.000000 hipscat-0.3.4/tests/data/small_sky_source/catalog_info.json
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-31 17:25:57.000000 hipscat-0.3.4/tests/data/small_sky_source/partition_info.csv
+-rw-r--r--   0 runner    (1001) docker     (127)  1581120 2024-05-31 17:25:57.000000 hipscat-0.3.4/tests/data/small_sky_source/point_map.fits
+-rw-r--r--   0 runner    (1001) docker     (127)     1946 2024-05-31 17:25:57.000000 hipscat-0.3.4/tests/data/small_sky_source/provenance_info.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:26:02.372830 hipscat-0.3.4/tests/data/small_sky_source_object_index/
+-rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-05-31 17:25:57.000000 hipscat-0.3.4/tests/data/small_sky_source_object_index/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2296 2024-05-31 17:25:57.000000 hipscat-0.3.4/tests/data/small_sky_source_object_index/_common_metadata
+-rw-r--r--   0 runner    (1001) docker     (127)     2729 2024-05-31 17:25:57.000000 hipscat-0.3.4/tests/data/small_sky_source_object_index/_metadata
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-05-31 17:25:57.000000 hipscat-0.3.4/tests/data/small_sky_source_object_index/catalog_info.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:26:02.372830 hipscat-0.3.4/tests/data/small_sky_source_object_index/index/
+-rw-r--r--   0 runner    (1001) docker     (127)     4153 2024-05-31 17:25:57.000000 hipscat-0.3.4/tests/data/small_sky_source_object_index/index/part.0.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-05-31 17:25:57.000000 hipscat-0.3.4/tests/data/small_sky_source_object_index/provenance_info.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:26:02.376829 hipscat-0.3.4/tests/data/small_sky_to_small_sky_order1/
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-05-31 17:25:57.000000 hipscat-0.3.4/tests/data/small_sky_to_small_sky_order1/_common_metadata
+-rw-r--r--   0 runner    (1001) docker     (127)     2929 2024-05-31 17:25:57.000000 hipscat-0.3.4/tests/data/small_sky_to_small_sky_order1/_metadata
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-05-31 17:25:57.000000 hipscat-0.3.4/tests/data/small_sky_to_small_sky_order1/catalog_info.json
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-31 17:25:57.000000 hipscat-0.3.4/tests/data/small_sky_to_small_sky_order1/partition_info.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-31 17:25:57.000000 hipscat-0.3.4/tests/data/small_sky_to_small_sky_order1/partition_join_info.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:26:02.376829 hipscat-0.3.4/tests/hipscat/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:26:02.376829 hipscat-0.3.4/tests/hipscat/catalog/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:26:02.376829 hipscat-0.3.4/tests/hipscat/catalog/association_catalog/
+-rw-r--r--   0 runner    (1001) docker     (127)     5552 2024-05-31 17:25:57.000000 hipscat-0.3.4/tests/hipscat/catalog/association_catalog/test_association_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2627 2024-05-31 17:25:57.000000 hipscat-0.3.4/tests/hipscat/catalog/association_catalog/test_association_catalog_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6156 2024-05-31 17:25:57.000000 hipscat-0.3.4/tests/hipscat/catalog/association_catalog/test_partition_join_info.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:26:02.376829 hipscat-0.3.4/tests/hipscat/catalog/dataset/
+-rw-r--r--   0 runner    (1001) docker     (127)     1595 2024-05-31 17:25:57.000000 hipscat-0.3.4/tests/hipscat/catalog/dataset/test_base_catalog_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4896 2024-05-31 17:25:57.000000 hipscat-0.3.4/tests/hipscat/catalog/dataset/test_catalog_info_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-05-31 17:25:57.000000 hipscat-0.3.4/tests/hipscat/catalog/dataset/test_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:26:02.376829 hipscat-0.3.4/tests/hipscat/catalog/index/
+-rw-r--r--   0 runner    (1001) docker     (127)      699 2024-05-31 17:25:57.000000 hipscat-0.3.4/tests/hipscat/catalog/index/test_index_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2636 2024-05-31 17:25:57.000000 hipscat-0.3.4/tests/hipscat/catalog/index/test_index_catalog_info.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:26:02.376829 hipscat-0.3.4/tests/hipscat/catalog/loaders/
+-rw-r--r--   0 runner    (1001) docker     (127)      444 2024-05-31 17:25:57.000000 hipscat-0.3.4/tests/hipscat/catalog/loaders/test_read_from_hipscat.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:26:02.376829 hipscat-0.3.4/tests/hipscat/catalog/margin_cache/
+-rw-r--r--   0 runner    (1001) docker     (127)     2586 2024-05-31 17:25:57.000000 hipscat-0.3.4/tests/hipscat/catalog/margin_cache/test_margin_cache_catalog_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3941 2024-05-31 17:25:57.000000 hipscat-0.3.4/tests/hipscat/catalog/margin_cache/test_margin_catalog.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:26:02.376829 hipscat-0.3.4/tests/hipscat/catalog/source_catalog/
+-rw-r--r--   0 runner    (1001) docker     (127)     2645 2024-05-31 17:25:57.000000 hipscat-0.3.4/tests/hipscat/catalog/source_catalog/test_source_catalog_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24240 2024-05-31 17:25:57.000000 hipscat-0.3.4/tests/hipscat/catalog/test_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1579 2024-05-31 17:25:57.000000 hipscat-0.3.4/tests/hipscat/catalog/test_catalog_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6742 2024-05-31 17:25:57.000000 hipscat-0.3.4/tests/hipscat/catalog/test_partition_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1986 2024-05-31 17:25:57.000000 hipscat-0.3.4/tests/hipscat/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:26:02.376829 hipscat-0.3.4/tests/hipscat/inspection/
+-rw-r--r--   0 runner    (1001) docker     (127)     7492 2024-05-31 17:25:57.000000 hipscat-0.3.4/tests/hipscat/inspection/test_almanac.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3550 2024-05-31 17:25:57.000000 hipscat-0.3.4/tests/hipscat/inspection/test_almanac_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2775 2024-05-31 17:25:57.000000 hipscat-0.3.4/tests/hipscat/inspection/test_visualize_catalog.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:26:02.380830 hipscat-0.3.4/tests/hipscat/io/
+-rw-r--r--   0 runner    (1001) docker     (127)     3654 2024-05-31 17:25:57.000000 hipscat-0.3.4/tests/hipscat/io/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:26:02.380830 hipscat-0.3.4/tests/hipscat/io/file_io/
+-rw-r--r--   0 runner    (1001) docker     (127)     4488 2024-05-31 17:25:57.000000 hipscat-0.3.4/tests/hipscat/io/file_io/test_file_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5396 2024-05-31 17:25:57.000000 hipscat-0.3.4/tests/hipscat/io/file_io/test_file_pointers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8508 2024-05-31 17:25:57.000000 hipscat-0.3.4/tests/hipscat/io/test_parquet_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2290 2024-05-31 17:25:57.000000 hipscat-0.3.4/tests/hipscat/io/test_paths.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1459 2024-05-31 17:25:57.000000 hipscat-0.3.4/tests/hipscat/io/test_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8769 2024-05-31 17:25:57.000000 hipscat-0.3.4/tests/hipscat/io/test_write_metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:26:02.380830 hipscat-0.3.4/tests/hipscat/pixel_math/
+-rw-r--r--   0 runner    (1001) docker     (127)     3203 2024-05-31 17:25:57.000000 hipscat-0.3.4/tests/hipscat/pixel_math/test_healpix_pixel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-05-31 17:25:57.000000 hipscat-0.3.4/tests/hipscat/pixel_math/test_healpix_pixel_convertor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      739 2024-05-31 17:25:57.000000 hipscat-0.3.4/tests/hipscat/pixel_math/test_healpix_pixel_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5361 2024-05-31 17:25:57.000000 hipscat-0.3.4/tests/hipscat/pixel_math/test_hipscat_id.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2745 2024-05-31 17:25:57.000000 hipscat-0.3.4/tests/hipscat/pixel_math/test_margin_bounding.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10360 2024-05-31 17:25:57.000000 hipscat-0.3.4/tests/hipscat/pixel_math/test_partition_stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3789 2024-05-31 17:25:57.000000 hipscat-0.3.4/tests/hipscat/pixel_math/test_pixel_margins.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:26:02.380830 hipscat-0.3.4/tests/hipscat/pixel_tree/
+-rw-r--r--   0 runner    (1001) docker     (127)     3395 2024-05-31 17:25:57.000000 hipscat-0.3.4/tests/hipscat/pixel_tree/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1800 2024-05-31 17:25:57.000000 hipscat-0.3.4/tests/hipscat/pixel_tree/test_moc_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12040 2024-05-31 17:25:57.000000 hipscat-0.3.4/tests/hipscat/pixel_tree/test_pixel_alignment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1917 2024-05-31 17:25:57.000000 hipscat-0.3.4/tests/hipscat/pixel_tree/test_pixel_tree.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2265 2024-05-31 17:25:57.000000 hipscat-0.3.4/tests/hipscat/pixel_tree/test_pixel_tree_builder.py
```

### Comparing `hipscat-0.3.3/.copier-answers.yml` & `hipscat-0.3.4/.copier-answers.yml`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.3/.gitattributes` & `hipscat-0.3.4/.gitattributes`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.3/.github/ISSUE_TEMPLATE/1-bug_report.md` & `hipscat-0.3.4/.github/ISSUE_TEMPLATE/1-bug_report.md`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.3/.github/ISSUE_TEMPLATE/2-feature_request.md` & `hipscat-0.3.4/.github/ISSUE_TEMPLATE/2-feature_request.md`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.3/.github/pull_request_template.md` & `hipscat-0.3.4/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.3/.github/workflows/asv-main.yml` & `hipscat-0.3.4/.github/workflows/asv-main.yml`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.3/.github/workflows/asv-nightly.yml` & `hipscat-0.3.4/.github/workflows/asv-nightly.yml`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.3/.github/workflows/asv-pr.yml` & `hipscat-0.3.4/.github/workflows/asv-pr.yml`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.3/.github/workflows/build-documentation.yml` & `hipscat-0.3.4/.github/workflows/build-documentation.yml`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.3/.github/workflows/pre-commit-ci.yml` & `hipscat-0.3.4/.github/workflows/pre-commit-ci.yml`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.3/.github/workflows/publish-benchmarks-pr.yml` & `hipscat-0.3.4/.github/workflows/publish-benchmarks-pr.yml`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.3/.github/workflows/publish-to-pypi.yml` & `hipscat-0.3.4/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.3/.github/workflows/smoke-test.yml` & `hipscat-0.3.4/.github/workflows/smoke-test.yml`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.3/.github/workflows/testing-and-coverage.yml` & `hipscat-0.3.4/.github/workflows/testing-and-coverage.yml`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.3/.gitignore` & `hipscat-0.3.4/.gitignore`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.3/.pre-commit-config.yaml` & `hipscat-0.3.4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.3/.prepare_project.sh` & `hipscat-0.3.4/.prepare_project.sh`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.3/.setup_dev.sh` & `hipscat-0.3.4/.setup_dev.sh`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.3/LICENSE` & `hipscat-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.3/PKG-INFO` & `hipscat-0.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hipscat
-Version: 0.3.3
+Version: 0.3.4
 Summary: Hierarchical Progressive Survey Catalog
 Author-email: LINCC Frameworks <lincc-frameworks-team@lists.lsst.org>
 License: BSD 3-Clause License
         
         Copyright (c) 2023, LINCC Frameworks
         
         Redistribution and use in source and binary forms, with or without
```

### Comparing `hipscat-0.3.3/README.md` & `hipscat-0.3.4/README.md`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.3/benchmarks/asv.conf.json` & `hipscat-0.3.4/benchmarks/asv.conf.json`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.3/benchmarks/benchmarks.py` & `hipscat-0.3.4/benchmarks/benchmarks.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.3/docs/Makefile` & `hipscat-0.3.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.3/docs/conf.py` & `hipscat-0.3.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.3/docs/guide/contributing.rst` & `hipscat-0.3.4/docs/guide/contributing.rst`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.3/docs/guide/directory_scheme.rst` & `hipscat-0.3.4/docs/guide/directory_scheme.rst`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.3/docs/guide/margin_cache_diagram.png` & `hipscat-0.3.4/docs/guide/margin_cache_diagram.png`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.3/docs/guide/pixel_math.md` & `hipscat-0.3.4/docs/guide/pixel_math.md`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.3/docs/index.rst` & `hipscat-0.3.4/docs/index.rst`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.3/docs/notebooks/catalog_size_inspection.ipynb` & `hipscat-0.3.4/docs/notebooks/catalog_size_inspection.ipynb`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.3/docs/notebooks/cone_search.ipynb` & `hipscat-0.3.4/docs/notebooks/cone_search.ipynb`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.3/pyproject.toml` & `hipscat-0.3.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.3/src/.pylintrc` & `hipscat-0.3.4/src/.pylintrc`

 * *Files 0% similar despite different names*

```diff
@@ -58,15 +58,15 @@
 # The regex matches against base names, not paths.
 ignore-patterns=_version.py
 
 # List of module names for which member attributes should not be checked
 # (useful for modules/projects where namespaces are manipulated during runtime
 # and thus existing member attributes cannot be deduced by static analysis). It
 # supports qualified module names, as well as Unix pattern matching.
-ignored-modules=
+ignored-modules=astropy.units
 
 # Python code to execute, usually for sys.path manipulation such as
 # pygtk.require().
 #init-hook=
 
 # Use multiple processes to speed up Pylint. Specifying 0 will auto-detect the
 # number of processors available to use, and will cap the count on Windows to
```

### Comparing `hipscat-0.3.3/src/hipscat/catalog/association_catalog/association_catalog.py` & `hipscat-0.3.4/src/hipscat/catalog/association_catalog/association_catalog.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.3/src/hipscat/catalog/association_catalog/association_catalog_info.py` & `hipscat-0.3.4/src/hipscat/catalog/association_catalog/association_catalog_info.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.3/src/hipscat/catalog/association_catalog/partition_join_info.py` & `hipscat-0.3.4/src/hipscat/catalog/association_catalog/partition_join_info.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.3/src/hipscat/catalog/catalog.py` & `hipscat-0.3.4/src/hipscat/catalog/catalog.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,21 +9,17 @@
 from mocpy import MOC
 from typing_extensions import TypeAlias
 
 from hipscat.catalog.catalog_info import CatalogInfo
 from hipscat.catalog.catalog_type import CatalogType
 from hipscat.catalog.healpix_dataset.healpix_dataset import HealpixDataset, PixelInputTypes
 from hipscat.pixel_math import HealpixPixel
-from hipscat.pixel_math.box_filter import filter_pixels_by_box, wrap_ra_angles
-from hipscat.pixel_math.cone_filter import filter_pixels_by_cone
-from hipscat.pixel_math.polygon_filter import (
-    CartesianCoordinates,
-    SphericalCoordinates,
-    filter_pixels_by_polygon,
-)
+from hipscat.pixel_math.box_filter import generate_box_moc, wrap_ra_angles
+from hipscat.pixel_math.cone_filter import generate_cone_moc
+from hipscat.pixel_math.polygon_filter import CartesianCoordinates, SphericalCoordinates, generate_polygon_moc
 from hipscat.pixel_math.validators import (
     validate_box_search,
     validate_declination_values,
     validate_polygon,
     validate_radius,
 )
 from hipscat.pixel_tree.negative_tree import compute_negative_tree_pixels
@@ -81,15 +77,15 @@
             radius_arcsec (float): Radius of the cone in arcseconds
 
         Returns:
             A new catalog with only the pixels that overlap with the specified cone
         """
         validate_radius(radius_arcsec)
         validate_declination_values(dec)
-        return self.filter_from_pixel_list(filter_pixels_by_cone(self.pixel_tree, ra, dec, radius_arcsec))
+        return self.filter_by_moc(generate_cone_moc(ra, dec, radius_arcsec, self.get_max_coverage_order()))
 
     def filter_by_box(
         self, ra: Tuple[float, float] | None = None, dec: Tuple[float, float] | None = None
     ) -> Catalog:
         """Filter the pixels in the catalog to only include the pixels that overlap with a
         right ascension or declination range. In case both ranges are provided, filtering
         is performed using a polygon.
@@ -99,15 +95,15 @@
             dec (Tuple[float, float]): Declination range, in degrees
 
         Returns:
             A new catalog with only the pixels that overlap with the specified region
         """
         ra = tuple(wrap_ra_angles(ra)) if ra else None
         validate_box_search(ra, dec)
-        return self.filter_from_pixel_list(filter_pixels_by_box(self.pixel_tree, ra, dec))
+        return self.filter_by_moc(generate_box_moc(ra, dec, self.get_max_coverage_order()))
 
     def filter_by_polygon(self, vertices: List[SphericalCoordinates] | List[CartesianCoordinates]) -> Catalog:
         """Filter the pixels in the catalog to only include the pixels that overlap
         with a polygonal sky region.
 
         Args:
             vertices (List[SphericalCoordinates] | List[CartesianCoordinates]): The vertices
@@ -118,17 +114,19 @@
             A new catalog with only the pixels that overlap with the specified polygon.
         """
         if all(len(vertex) == 2 for vertex in vertices):
             ra, dec = np.array(vertices).T
             validate_declination_values(dec)
             # Get the coordinates vector on the unit sphere if we were provided
             # with polygon spherical coordinates of ra and dec
-            vertices = hp.ang2vec(ra, dec, lonlat=True)
-        validate_polygon(vertices)
-        return self.filter_from_pixel_list(filter_pixels_by_polygon(self.pixel_tree, vertices))
+            cart_vertices = hp.ang2vec(ra, dec, lonlat=True)
+        else:
+            cart_vertices = vertices
+        validate_polygon(cart_vertices)
+        return self.filter_by_moc(generate_polygon_moc(cart_vertices, self.get_max_coverage_order()))
 
     def generate_negative_tree_pixels(self) -> List[HealpixPixel]:
         """Get the leaf nodes at each healpix order that have zero catalog data.
 
         For example, if an example catalog only had data points in pixel 0 at
         order 0, then this method would return order 0's pixels 1 through 11.
         Used for getting full coverage on margin caches.
```

### Comparing `hipscat-0.3.3/src/hipscat/catalog/catalog_info.py` & `hipscat-0.3.4/src/hipscat/catalog/catalog_info.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.3/src/hipscat/catalog/dataset/base_catalog_info.py` & `hipscat-0.3.4/src/hipscat/catalog/dataset/base_catalog_info.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.3/src/hipscat/catalog/dataset/catalog_info_factory.py` & `hipscat-0.3.4/src/hipscat/catalog/dataset/catalog_info_factory.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.3/src/hipscat/catalog/dataset/dataset.py` & `hipscat-0.3.4/src/hipscat/catalog/dataset/dataset.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.3/src/hipscat/catalog/healpix_dataset/healpix_dataset.py` & `hipscat-0.3.4/src/hipscat/catalog/healpix_dataset/healpix_dataset.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from typing_extensions import Self, TypeAlias
 
 from hipscat.catalog.dataset import BaseCatalogInfo, Dataset
 from hipscat.catalog.partition_info import PartitionInfo
 from hipscat.io import FilePointer, file_io, paths
 from hipscat.pixel_math import HealpixPixel
 from hipscat.pixel_tree import PixelAlignment, PixelAlignmentType
+from hipscat.pixel_tree.moc_filter import filter_by_moc
 from hipscat.pixel_tree.pixel_alignment import align_with_mocs
 from hipscat.pixel_tree.pixel_tree import PixelTree
 
 PixelInputTypes = Union[PartitionInfo, PixelTree, List[HealpixPixel]]
 
 
 class HealpixDataset(Dataset):
@@ -127,26 +128,53 @@
             file_io.does_file_or_directory_exist(partition_info_file, storage_options=storage_options)
             or file_io.does_file_or_directory_exist(metadata_file, storage_options=storage_options)
         ):
             raise FileNotFoundError(
                 f"_metadata or partition info file is required in catalog directory {catalog_base_dir}"
             )
 
+    def get_max_coverage_order(self) -> int:
+        """Gets the maximum HEALPix order for which the coverage of the catalog is known from the pixel
+        tree and moc if it exists"""
+        max_order = (
+            max(self.moc.max_order, self.pixel_tree.get_max_depth())
+            if self.moc is not None
+            else self.pixel_tree.get_max_depth()
+        )
+        return max_order
+
     def filter_from_pixel_list(self, pixels: List[HealpixPixel]) -> Self:
-        """Filter the pixels in the catalog to only include the requested pixels.
+        """Filter the pixels in the catalog to only include any that overlap with the requested pixels.
 
         Args:
             pixels (List[HealpixPixels]): the pixels to include
 
         Returns:
-            A new catalog with only those pixels. Note that we reset the total_rows
-            to None, instead of performing a scan over the new pixel sizes.
+            A new catalog with only the pixels that overlap with the given pixels. Note that we reset the
+            total_rows to None, as updating would require a scan over the new pixel sizes.
         """
+        orders = np.array([p.order for p in pixels])
+        pixel_inds = np.array([p.pixel for p in pixels])
+        max_order = np.max(orders) if len(orders) > 0 else 0
+        moc = MOC.from_healpix_cells(ipix=pixel_inds, depth=orders, max_depth=max_order)
+        return self.filter_by_moc(moc)
+
+    def filter_by_moc(self, moc: MOC) -> Self:
+        """Filter the pixels in the catalog to only include the pixels that overlap with the moc provided.
+
+        Args:
+            moc (mocpy.MOC): the moc to filter by
+
+        Returns:
+            A new catalog with only the pixels that overlap with the moc. Note that we reset the total_rows
+            to None, as updating would require a scan over the new pixel sizes."""
+        filtered_tree = filter_by_moc(self.pixel_tree, moc)
+        filtered_moc = self.moc.intersection(moc) if self.moc is not None else None
         filtered_catalog_info = dataclasses.replace(self.catalog_info, total_rows=None)
-        return self.__class__(filtered_catalog_info, pixels)
+        return self.__class__(filtered_catalog_info, filtered_tree, moc=filtered_moc)
 
     def align(
         self, other_cat: Self, alignment_type: PixelAlignmentType = PixelAlignmentType.INNER
     ) -> PixelAlignment:
         """Performs an alignment to another catalog, using the pixel tree and mocs if available
 
         An alignment compares the pixel structures of the two catalogs, checking which pixels overlap.
```

### Comparing `hipscat-0.3.3/src/hipscat/catalog/index/index_catalog.py` & `hipscat-0.3.4/src/hipscat/catalog/index/index_catalog.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.3/src/hipscat/catalog/index/index_catalog_info.py` & `hipscat-0.3.4/src/hipscat/catalog/index/index_catalog_info.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.3/src/hipscat/catalog/margin_cache/margin_cache_catalog_info.py` & `hipscat-0.3.4/src/hipscat/catalog/margin_cache/margin_cache_catalog_info.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.3/src/hipscat/catalog/margin_cache/margin_catalog.py` & `hipscat-0.3.4/src/hipscat/loaders/read_from_hipscat.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,48 +1,59 @@
 from __future__ import annotations
 
-from mocpy import MOC
-from typing_extensions import TypeAlias
+from typing import Type
 
-from hipscat.catalog.catalog_type import CatalogType
-from hipscat.catalog.healpix_dataset.healpix_dataset import HealpixDataset, PixelInputTypes
-from hipscat.catalog.margin_cache import MarginCacheCatalogInfo
+from hipscat import io
+from hipscat.catalog import AssociationCatalog, Catalog, CatalogType, Dataset, MarginCatalog
+from hipscat.catalog.dataset import BaseCatalogInfo
+from hipscat.catalog.index.index_catalog import IndexCatalog
+
+CATALOG_TYPE_TO_CLASS = {
+    CatalogType.OBJECT: Catalog,
+    CatalogType.SOURCE: Catalog,
+    CatalogType.ASSOCIATION: AssociationCatalog,
+    CatalogType.INDEX: IndexCatalog,
+    CatalogType.MARGIN: MarginCatalog,
+}
+
+
+def read_from_hipscat(
+    catalog_path: str,
+    catalog_type: CatalogType | None = None,
+    storage_options: dict | None = None,
+) -> Dataset:
+    """Reads a HiPSCat Catalog from a HiPSCat directory
+
+    Args:
+        catalog_path (str): path to the root directory of the catalog
+        catalog_type (CatalogType): Default `None`. By default, the type of the catalog is loaded
+            from the catalog info and the corresponding object type is returned. Python's type hints
+            cannot allow a return type specified by a loaded value, so to use the correct return
+            type for type checking, the type of the catalog can be specified here. Use by specifying
+            the hipscat class for that catalog.
+        storage_options (dict): dictionary that contains abstract filesystem credentials
 
-
-class MarginCatalog(HealpixDataset):
-    """A HiPSCat Catalog used to contain the 'margin' of another HiPSCat catalog.
-
-    Catalogs of this type are used alongside a primary catalog, and contains the margin points for each
-    HEALPix pixel - any points that are within a certain distance from the HEALPix pixel boundary. This is
-    used to ensure spatial operations such as crossmatching can be performed efficiently while maintaining
-    accuracy.
+    Returns:
+        The initialized catalog object
     """
-
-    # Update CatalogInfoClass, used to check if the catalog_info is the correct type, and
-    # set the catalog info to the correct type
-    CatalogInfoClass: TypeAlias = MarginCacheCatalogInfo
-    catalog_info: CatalogInfoClass
-
-    def __init__(
-        self,
-        catalog_info: CatalogInfoClass,
-        pixels: PixelInputTypes,
-        catalog_path: str = None,
-        moc: MOC | None = None,
-        storage_options: dict | None = None,
-    ) -> None:
-        """Initializes a Margin Catalog
-
-        Args:
-            catalog_info: CatalogInfo object with catalog metadata
-            pixels: Specifies the pixels contained in the catalog. Can be either a
-                list of HealpixPixel, `PartitionInfo object`, or a `PixelTree` object
-            catalog_path: If the catalog is stored on disk, specify the location of the catalog
-                Does not load the catalog from this path, only store as metadata
-            storage_options: dictionary that contains abstract filesystem credentials
-            moc (mocpy.MOC): MOC object representing the coverage of the catalog
-        """
-        if catalog_info.catalog_type != CatalogType.MARGIN:
-            raise ValueError(f"Catalog info `catalog_type` must equal {CatalogType.MARGIN}")
-        super().__init__(
-            catalog_info, pixels, catalog_path=catalog_path, moc=moc, storage_options=storage_options
-        )
+    catalog_type_to_use = (
+        _read_dataset_class_from_metadata(catalog_path, storage_options=storage_options)
+        if catalog_type is None
+        else catalog_type
+    )
+    loader = _get_loader_from_catalog_type(catalog_type_to_use)
+    return loader.read_from_hipscat(catalog_path, storage_options=storage_options)
+
+
+def _read_dataset_class_from_metadata(
+    catalog_base_path: str, storage_options: dict | None = None
+) -> CatalogType:
+    catalog_base_dir = io.file_io.get_file_pointer_from_path(catalog_base_path)
+    catalog_info_path = io.paths.get_catalog_info_pointer(catalog_base_dir)
+    catalog_info = BaseCatalogInfo.read_from_metadata_file(catalog_info_path, storage_options=storage_options)
+    return catalog_info.catalog_type
+
+
+def _get_loader_from_catalog_type(catalog_type: CatalogType) -> Type[Dataset]:
+    if catalog_type not in CATALOG_TYPE_TO_CLASS:
+        raise NotImplementedError(f"Cannot load catalog of type {catalog_type}")
+    return CATALOG_TYPE_TO_CLASS[catalog_type]
```

### Comparing `hipscat-0.3.3/src/hipscat/catalog/partition_info.py` & `hipscat-0.3.4/src/hipscat/catalog/partition_info.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.3/src/hipscat/catalog/source_catalog/source_catalog_info.py` & `hipscat-0.3.4/src/hipscat/catalog/source_catalog/source_catalog_info.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.3/src/hipscat/inspection/almanac.py` & `hipscat-0.3.4/src/hipscat/inspection/almanac.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.3/src/hipscat/inspection/almanac_info.py` & `hipscat-0.3.4/src/hipscat/inspection/almanac_info.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.3/src/hipscat/inspection/visualize_catalog.py` & `hipscat-0.3.4/src/hipscat/inspection/visualize_catalog.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.3/src/hipscat/io/__init__.py` & `hipscat-0.3.4/src/hipscat/io/__init__.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.3/src/hipscat/io/file_io/__init__.py` & `hipscat-0.3.4/src/hipscat/io/file_io/__init__.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.3/src/hipscat/io/file_io/file_io.py` & `hipscat-0.3.4/src/hipscat/io/file_io/file_io.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from __future__ import annotations
 
 import json
 import tempfile
+import warnings
 from typing import Any, Dict, Tuple, Union
 
 import healpy as hp
 import numpy as np
 import pandas as pd
 import pyarrow.dataset as pds
 import pyarrow.parquet as pq
@@ -274,16 +275,25 @@
         value at each index corresponds to the number of objects found at the healpix pixel.
     """
     file_system, map_file_pointer = get_fs(file_pointer=map_file_pointer, storage_options=storage_options)
     with tempfile.NamedTemporaryFile() as _tmp_file:
         with file_system.open(map_file_pointer, "rb") as _map_file:
             map_data = _map_file.read()
             _tmp_file.write(map_data)
-            map_fits_image = hp.read_map(_tmp_file.name)
-    return map_fits_image
+            map_fits_image = hp.read_map(_tmp_file.name, nest=True, h=True)
+            header_dict = dict(map_fits_image[1])
+            if header_dict["ORDERING"] != "NESTED":
+                warnings.warn(
+                    "point_map.fits file written in RING ordering, due to "
+                    "https://github.com/astronomy-commons/hipscat/issues/271. "
+                    "Converting to NESTED."
+                )
+                map_fits_image = hp.read_map(_tmp_file.name)
+                return map_fits_image
+            return map_fits_image[0]
 
 
 def write_fits_image(
     histogram: np.ndarray, map_file_pointer: FilePointer, storage_options: Union[Dict[Any, Any], None] = None
 ):
     """Write the object spatial distribution information to a healpix FITS file.
 
@@ -292,15 +302,15 @@
             value at each index corresponds to the number of objects found at the healpix pixel.
         file_pointer: location of file to be written
         storage_options: dictionary that contains abstract filesystem credentials
     """
     file_system, map_file_pointer = get_fs(file_pointer=map_file_pointer, storage_options=storage_options)
     with tempfile.NamedTemporaryFile() as _tmp_file:
         with file_system.open(map_file_pointer, "wb") as _map_file:
-            hp.write_map(_tmp_file.name, histogram, overwrite=True, dtype=np.int64)
+            hp.write_map(_tmp_file.name, histogram, overwrite=True, dtype=np.int64, nest=True)
             _map_file.write(_tmp_file.read())
 
 
 def read_yaml(file_handle: FilePointer, storage_options: Union[Dict[Any, Any], None] = None):
     """Reads yaml file from filesystem.
 
     Args:
```

### Comparing `hipscat-0.3.3/src/hipscat/io/file_io/file_pointer.py` & `hipscat-0.3.4/src/hipscat/io/file_io/file_pointer.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.3/src/hipscat/io/parquet_metadata.py` & `hipscat-0.3.4/src/hipscat/io/parquet_metadata.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.3/src/hipscat/io/paths.py` & `hipscat-0.3.4/src/hipscat/io/paths.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.3/src/hipscat/io/validation.py` & `hipscat-0.3.4/src/hipscat/io/validation.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.3/src/hipscat/io/write_metadata.py` & `hipscat-0.3.4/src/hipscat/io/write_metadata.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,28 +8,35 @@
 from typing import Any, Dict, Union
 
 import numpy as np
 import pandas as pd
 
 from hipscat.io import file_io, paths
 from hipscat.io.parquet_metadata import write_parquet_metadata as wpm
+from hipscat.pixel_math.healpix_pixel import HealpixPixel
 
 
 class HipscatEncoder(json.JSONEncoder):
     """Special json encoder for types commonly encountered with hipscat.
 
     NB: This will only be used by JSON encoding when encountering a type
     that is unhandled by the default encoder.
     """
 
     def default(self, o):
         if isinstance(o, Path):
             return str(o)
         if isinstance(o, (type, np.dtype, pd.core.dtypes.base.ExtensionDtype)):
             return str(o)
+        if isinstance(o, HealpixPixel):
+            return str(o)
+        if np.issubdtype(o.dtype, np.integer):
+            return int(o)
+        if isinstance(o, np.ndarray):
+            return o.tolist()
         return super().default(o)  # pragma: no cover
 
 
 def write_json_file(
     metadata_dictionary: dict,
     file_pointer: file_io.FilePointer,
     storage_options: Union[Dict[Any, Any], None] = None,
```

### Comparing `hipscat-0.3.3/src/hipscat/pixel_math/__init__.py` & `hipscat-0.3.4/src/hipscat/pixel_math/__init__.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.3/src/hipscat/pixel_math/box_filter.py` & `hipscat-0.3.4/src/hipscat/pixel_math/box_filter.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,70 +1,56 @@
 from __future__ import annotations
 
 from typing import Iterable, List, Tuple
 
 import healpy as hp
 import numpy as np
+from mocpy import MOC
 
-from hipscat.pixel_math import HealpixPixel
-from hipscat.pixel_math.filter import get_filtered_pixel_list
 from hipscat.pixel_math.polygon_filter import SphericalCoordinates
-from hipscat.pixel_tree import PixelAlignmentType, align_trees
-from hipscat.pixel_tree.pixel_tree import PixelTree
 
 
-def filter_pixels_by_box(
-    pixel_tree: PixelTree, ra: Tuple[float, float] | None, dec: Tuple[float, float] | None
-) -> List[HealpixPixel]:
-    """Filter the leaf pixels in a pixel tree to return a partition_info dataframe
-    with the pixels that overlap with a right ascension and/or declination region.
+def generate_box_moc(ra: Tuple[float, float] | None, dec: Tuple[float, float] | None, order: int) -> MOC:
+    """Generates a MOC object that covers the specified box area
 
     Args:
-        pixel_tree (PixelTree): The catalog tree to filter pixels from
         ra (Tuple[float, float]): Right ascension range, in [0,360] degrees
         dec (Tuple[float, float]): Declination range, in [-90,90] degrees
+        order (int): Maximum order of the moc to generate the box at
 
     Returns:
-        List of HEALPix representing only the pixels that overlap with the right
-        ascension and/or declination region.
+        a MOC object that covers the specified box
     """
-    max_order = pixel_tree.get_max_depth()
-
-    filter_tree = None
-    ra_search_tree, dec_search_tree = None, None
+    filter_moc = None
+    ra_search_moc, dec_search_moc = None, None
 
     if ra is not None:
-        ra_search_tree = _generate_ra_strip_pixel_tree(ra, max_order)
-        filter_tree = ra_search_tree
+        ra_search_moc = _generate_ra_strip_moc(ra, order)
+        filter_moc = ra_search_moc
     if dec is not None:
-        dec_search_tree = _generate_dec_strip_pixel_tree(dec, max_order)
-        filter_tree = dec_search_tree
-    if ra_search_tree is not None and dec_search_tree is not None:
-        filter_tree = align_trees(
-            ra_search_tree, dec_search_tree, alignment_type=PixelAlignmentType.INNER
-        ).pixel_tree
-
-    result_pixels = get_filtered_pixel_list(pixel_tree, filter_tree)
-
-    return result_pixels
+        dec_search_moc = _generate_dec_strip_moc(dec, order)
+        filter_moc = dec_search_moc
+    if ra_search_moc is not None and dec_search_moc is not None:
+        filter_moc = ra_search_moc.intersection(dec_search_moc)
+    return filter_moc
 
 
 def wrap_ra_angles(ra: np.ndarray | Iterable | int | float) -> np.ndarray:
     """Wraps angles to the [0,360] degree range.
 
     Args:
         ra (ndarray | Iterable | int | float): Right ascension values, in degrees
 
     Returns:
         A numpy array of right ascension values, wrapped to the [0,360] degree range.
     """
     return np.asarray(ra, dtype=float) % 360
 
 
-def _generate_ra_strip_pixel_tree(ra_range: Tuple[float, float], order: int) -> PixelTree:
+def _generate_ra_strip_moc(ra_range: Tuple[float, float], order: int) -> MOC:
     """Generates a pixel_tree filled with leaf nodes at a given order that overlap with the ra region."""
     # Subdivide polygons (if needed) in two smaller polygons of at most 180 degrees
     division_ra = _get_division_ra(ra_range)
 
     if division_ra is not None:
         pixels_in_range = _get_pixels_for_subpolygons(
             [
@@ -86,29 +72,29 @@
                 [(0, 90), (ra_range[0], 0), (ra_range[1], 0)],
                 # South Pole
                 [(ra_range[0], 0), (0, -90), (ra_range[1], 0)],
             ],
             order,
         )
 
-    pixel_list = [HealpixPixel(order, polygon_pixel) for polygon_pixel in pixels_in_range]
-    return PixelTree.from_healpix(pixel_list)
+    orders = np.full(pixels_in_range.shape, fill_value=order)
+    return MOC.from_healpix_cells(ipix=pixels_in_range, depth=orders, max_depth=order)
 
 
-def _generate_dec_strip_pixel_tree(dec_range: Tuple[float, float], order: int) -> PixelTree:
+def _generate_dec_strip_moc(dec_range: Tuple[float, float], order: int) -> MOC:
     """Generates a pixel_tree filled with leaf nodes at a given order that overlap with the dec region."""
     nside = hp.order2nside(order)
     # Convert declination values to colatitudes, in radians, and revert their order
     colat_rad = np.sort(np.radians([90 - dec if dec > 0 else 90 + abs(dec) for dec in dec_range]))
     # Figure out which pixels in nested order are contained in the declination band
     pixels_in_range = hp.ring2nest(
         nside, hp.query_strip(nside, theta1=colat_rad[0], theta2=colat_rad[1], inclusive=True)
     )
-    pixel_list = [HealpixPixel(order, polygon_pixel) for polygon_pixel in pixels_in_range]
-    return PixelTree.from_healpix(pixel_list)
+    orders = np.full(pixels_in_range.shape, fill_value=order)
+    return MOC.from_healpix_cells(ipix=pixels_in_range, depth=orders, max_depth=order)
 
 
 def _get_division_ra(ra_range: Tuple[float, float]) -> float | None:
     """Gets the division angle for the right ascension region. This is crucial for the edge
     cases where we need to split up polygons wider than 180 degrees into smaller polygons."""
     division_ra = None
     if ra_range[0] > ra_range[1] and 360 - ra_range[0] + ra_range[1] >= 180:
```

### Comparing `hipscat-0.3.3/src/hipscat/pixel_math/filter.py` & `hipscat-0.3.4/src/hipscat/pixel_math/filter.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.3/src/hipscat/pixel_math/healpix_pixel.py` & `hipscat-0.3.4/src/hipscat/pixel_math/healpix_pixel.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.3/src/hipscat/pixel_math/healpix_pixel_convertor.py` & `hipscat-0.3.4/src/hipscat/pixel_math/healpix_pixel_convertor.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.3/src/hipscat/pixel_math/healpix_pixel_function.py` & `hipscat-0.3.4/src/hipscat/pixel_math/healpix_pixel_function.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.3/src/hipscat/pixel_math/hipscat_id.py` & `hipscat-0.3.4/src/hipscat/pixel_math/hipscat_id.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.3/src/hipscat/pixel_math/margin_bounding.py` & `hipscat-0.3.4/src/hipscat/pixel_math/margin_bounding.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.3/src/hipscat/pixel_math/partition_stats.py` & `hipscat-0.3.4/src/hipscat/pixel_math/partition_stats.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.3/src/hipscat/pixel_math/pixel_margins.py` & `hipscat-0.3.4/src/hipscat/pixel_math/pixel_margins.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.3/src/hipscat/pixel_math/validators.py` & `hipscat-0.3.4/src/hipscat/pixel_math/validators.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.3/src/hipscat/pixel_tree/moc_filter.py` & `hipscat-0.3.4/src/hipscat/pixel_tree/moc_filter.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.3/src/hipscat/pixel_tree/negative_tree.py` & `hipscat-0.3.4/src/hipscat/pixel_tree/negative_tree.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.3/src/hipscat/pixel_tree/pixel_alignment.py` & `hipscat-0.3.4/src/hipscat/pixel_tree/pixel_alignment.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.3/src/hipscat/pixel_tree/pixel_tree.py` & `hipscat-0.3.4/src/hipscat/pixel_tree/pixel_tree.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.3/src/hipscat.egg-info/PKG-INFO` & `hipscat-0.3.4/src/hipscat.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hipscat
-Version: 0.3.3
+Version: 0.3.4
 Summary: Hierarchical Progressive Survey Catalog
 Author-email: LINCC Frameworks <lincc-frameworks-team@lists.lsst.org>
 License: BSD 3-Clause License
         
         Copyright (c) 2023, LINCC Frameworks
         
         Redistribution and use in source and binary forms, with or without
```

### Comparing `hipscat-0.3.3/src/hipscat.egg-info/SOURCES.txt` & `hipscat-0.3.4/src/hipscat.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -96,14 +96,15 @@
 src/hipscat/pixel_math/margin_bounding.py
 src/hipscat/pixel_math/partition_stats.py
 src/hipscat/pixel_math/pixel_margins.py
 src/hipscat/pixel_math/polygon_filter.py
 src/hipscat/pixel_math/validators.py
 src/hipscat/pixel_tree/__init__.py
 src/hipscat/pixel_tree/moc_filter.py
+src/hipscat/pixel_tree/moc_utils.py
 src/hipscat/pixel_tree/negative_tree.py
 src/hipscat/pixel_tree/pixel_alignment.py
 src/hipscat/pixel_tree/pixel_alignment_types.py
 src/hipscat/pixel_tree/pixel_tree.py
 tests/.pylintrc
 tests/conftest.py
 tests/data/generate_data.ipynb
```

### Comparing `hipscat-0.3.3/tests/.pylintrc` & `hipscat-0.3.4/tests/.pylintrc`

 * *Files 0% similar despite different names*

```diff
@@ -58,15 +58,15 @@
 # The regex matches against base names, not paths.
 ignore-patterns=_version.py
 
 # List of module names for which member attributes should not be checked
 # (useful for modules/projects where namespaces are manipulated during runtime
 # and thus existing member attributes cannot be deduced by static analysis). It
 # supports qualified module names, as well as Unix pattern matching.
-ignored-modules=
+ignored-modules=astropy.units
 
 # Python code to execute, usually for sys.path manipulation such as
 # pygtk.require().
 #init-hook=
 
 # Use multiple processes to speed up Pylint. Specifying 0 will auto-detect the
 # number of processors available to use, and will cap the count on Windows to
```

### Comparing `hipscat-0.3.3/tests/conftest.py` & `hipscat-0.3.4/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.3/tests/data/generate_data.ipynb` & `hipscat-0.3.4/tests/data/generate_data.ipynb`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.99602320473644%*

 * *Differences: {"'cells'": "{1: {'source': {insert: [(6, 'from dask.distributed import Client\\n'), (11, "*

 * *            '\'hipscat_import_dir = "../../../hipscat-import/tests/hipscat_import/data/"\\n\'), '*

 * *            "(12, 'client = Client(n_workers=1, threads_per_worker=1, local_directory=tmp_dir)')], "*

 * *            "delete: [10]}}, 3: {'source': {insert: [(7, 'runner.pipeline_with_client(args, "*

 * *            "client)')], delete: [8, 5]}}, 5: {'source': {insert: [(8, "*

 * *            "'runner.pipeline_with_client(args, client […]*

```diff
@@ -27,19 +27,21 @@
             "source": [
                 "import hipscat_import.pipeline as runner\n",
                 "from hipscat_import.catalog.arguments import ImportArguments\n",
                 "from hipscat_import.index.arguments import IndexArguments\n",
                 "from hipscat_import.margin_cache.margin_cache_arguments import MarginCacheArguments\n",
                 "import tempfile\n",
                 "from pathlib import Path\n",
+                "from dask.distributed import Client\n",
                 "\n",
                 "tmp_path = tempfile.TemporaryDirectory()\n",
                 "tmp_dir = tmp_path.name\n",
                 "\n",
-                "hipscat_import_dir = \"../../../hipscat-import/tests/hipscat_import/data/\""
+                "hipscat_import_dir = \"../../../hipscat-import/tests/hipscat_import/data/\"\n",
+                "client = Client(n_workers=1, threads_per_worker=1, local_directory=tmp_dir)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "### small_sky\n",
@@ -59,18 +61,17 @@
             "outputs": [],
             "source": [
                 "args = ImportArguments(\n",
                 "    input_path=Path(hipscat_import_dir) / \"small_sky\",\n",
                 "    output_path=\".\",\n",
                 "    file_reader=\"csv\",\n",
                 "    output_artifact_name=\"small_sky\",\n",
-                "    overwrite=True,\n",
                 "    tmp_dir=tmp_dir,\n",
                 ")\n",
-                "runner.pipeline(args)"
+                "runner.pipeline_with_client(args, client)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "### small_sky_order1\n",
@@ -96,18 +97,17 @@
             "source": [
                 "args = ImportArguments(\n",
                 "    input_path=Path(hipscat_import_dir) / \"small_sky\",\n",
                 "    output_path=\".\",\n",
                 "    file_reader=\"csv\",\n",
                 "    output_artifact_name=\"small_sky_order1\",\n",
                 "    constant_healpix_order=1,\n",
-                "    overwrite=True,\n",
                 "    tmp_dir=tmp_dir,\n",
                 ")\n",
-                "runner.pipeline(args)"
+                "runner.pipeline_with_client(args, client)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "### small_sky_order1_id_index\n",
@@ -126,18 +126,17 @@
                 "args = IndexArguments(\n",
                 "    input_catalog_path=\"small_sky\",\n",
                 "    indexing_column=\"id\",\n",
                 "    output_path=\".\",\n",
                 "    output_artifact_name=\"small_sky_order1_id_index\",\n",
                 "    include_hipscat_index=False,\n",
                 "    compute_partition_size=200_000,\n",
-                "    overwrite=True,\n",
                 "    tmp_dir=tmp_dir,\n",
                 ")\n",
-                "runner.pipeline(args)"
+                "runner.pipeline_with_client(args, client)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "### small_sky_order1_margin\n",
@@ -163,18 +162,17 @@
             "outputs": [],
             "source": [
                 "margin_args = MarginCacheArguments(\n",
                 "    margin_threshold=7200,\n",
                 "    input_catalog_path=\"small_sky_order1\",\n",
                 "    output_path=\".\",\n",
                 "    output_artifact_name=\"small_sky_order1_margin\",\n",
-                "    overwrite=True,\n",
                 "    tmp_dir=tmp_dir,\n",
                 ")\n",
-                "runner.pipeline(margin_args)"
+                "runner.pipeline_with_client(args, client)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "### small_sky_to_small_sky_order1\n",
@@ -237,18 +235,17 @@
                 "    output_path=\".\",\n",
                 "    file_reader=\"csv\",\n",
                 "    ra_column=\"source_ra\",\n",
                 "    dec_column=\"source_dec\",\n",
                 "    catalog_type=\"source\",\n",
                 "    pixel_threshold=3000,\n",
                 "    output_artifact_name=\"small_sky_source\",\n",
-                "    overwrite=True,\n",
                 "    tmp_dir=tmp_dir,\n",
                 ")\n",
-                "runner.pipeline(args)"
+                "runner.pipeline_with_client(args, client)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "### small_sky_source_object_index\n",
@@ -278,26 +275,26 @@
                 "args = IndexArguments(\n",
                 "    input_catalog_path=\"small_sky_source\",\n",
                 "    indexing_column=\"object_id\",\n",
                 "    output_path=\".\",\n",
                 "    output_artifact_name=\"small_sky_source_object_index\",\n",
                 "    include_hipscat_index=False,\n",
                 "    compute_partition_size=200_000,\n",
-                "    overwrite=True,\n",
                 "    tmp_dir=tmp_dir,\n",
                 ")\n",
-                "runner.pipeline(args)"
+                "runner.pipeline_with_client(args, client)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
+                "client.close()\n",
                 "tmp_path.cleanup()"
             ]
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "hipscatenv",
@@ -310,13 +307,13 @@
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

### Comparing `hipscat-0.3.3/tests/data/small_sky/Norder=0/Dir=0/Npix=11.parquet` & `hipscat-0.3.4/tests/data/small_sky/Norder=0/Dir=0/Npix=11.parquet`

 * *Files 1% similar despite different names*

```diff
@@ -386,17 +386,17 @@
 00001810: 2c20 2270 616e 6461 735f 7479 7065 223a  , "pandas_type":
 00001820: 2022 7569 6e74 3634 222c 2022 6e75 6d70   "uint64", "nump
 00001830: 795f 7479 7065 223a 2022 7569 6e74 3634  y_type": "uint64
 00001840: 222c 2022 6d65 7461 6461 7461 223a 206e  ", "metadata": n
 00001850: 756c 6c7d 5d2c 2022 6372 6561 746f 7222  ull}], "creator"
 00001860: 3a20 7b22 6c69 6272 6172 7922 3a20 2270  : {"library": "p
 00001870: 7961 7272 6f77 222c 2022 7665 7273 696f  yarrow", "versio
-00001880: 6e22 3a20 2231 342e 302e 3122 7d2c 2022  n": "14.0.1"}, "
+00001880: 6e22 3a20 2231 362e 302e 3022 7d2c 2022  n": "16.0.0"}, "
 00001890: 7061 6e64 6173 5f76 6572 7369 6f6e 223a  pandas_version":
-000018a0: 2022 322e 302e 3322 7d00 180c 4152 524f   "2.0.3"}...ARRO
+000018a0: 2022 322e 322e 3222 7d00 180c 4152 524f   "2.2.2"}...ARRO
 000018b0: 573a 7363 6865 6d61 18ac 132f 2f2f 2f2f  W:schema.../////
 000018c0: 7a67 4841 4141 5141 4141 4141 4141 4b41  zgHAAAQAAAAAAAKA
 000018d0: 4134 4142 6741 4641 4167 4143 6741 4141  A4ABgAFAAgACgAAA
 000018e0: 4141 4242 4141 5141 4141 4141 4141 4b41  AABBAAQAAAAAAAKA
 000018f0: 4177 4141 4141 4541 4167 4143 6741 4141  AwAAAAEAAgACgAAA
 00001900: 4351 4641 4141 4541 4141 4141 5141 4141  CQFAAAEAAAAAQAAA
 00001910: 4177 4141 4141 4941 4177 4142 4141 4941  AwAAAAIAAwABAAIA
@@ -500,18 +500,18 @@
 00001f30: 4341 6962 6e56 7463 486c 6664 486c 775a  CAibnVtcHlfdHlwZ
 00001f40: 5349 3649 434a 3161 5735 304e 6a51 694c  SI6ICJ1aW50NjQiL
 00001f50: 4341 6962 5756 3059 5752 6864 4745 694f  CAibWV0YWRhdGEiO
 00001f60: 6942 7564 5778 7366 5630 7349 434a 6a63  iBudWxsfV0sICJjc
 00001f70: 6d56 6864 4739 7949 6a6f 6765 794a 7361  mVhdG9yIjogeyJsa
 00001f80: 574a 7959 584a 3549 6a6f 6749 6e42 3559  WJyYXJ5IjogInB5Y
 00001f90: 584a 7962 3363 694c 4341 6964 6d56 7963  XJyb3ciLCAidmVyc
-00001fa0: 326c 7662 6949 3649 4349 784e 4334 774c  2lvbiI6ICIxNC4wL
-00001fb0: 6a45 6966 5377 6749 6e42 6862 6d52 6863  jEifSwgInBhbmRhc
+00001fa0: 326c 7662 6949 3649 4349 784e 6934 774c  2lvbiI6ICIxNi4wL
+00001fb0: 6a41 6966 5377 6749 6e42 6862 6d52 6863  jAifSwgInBhbmRhc
 00001fc0: 3139 325a 584a 7a61 5739 7549 6a6f 6749  192ZXJzaW9uIjogI
-00001fd0: 6a49 754d 4334 7a49 6e30 4143 5141 4141  jIuMC4zIn0ACQAAA
+00001fd0: 6a49 754d 6934 7949 6e30 4143 5141 4141  jIuMi4yIn0ACQAAA
 00001fe0: 4c41 4241 4142 7341 5141 4151 4145 4141  LABAABsAQAAQAEAA
 00001ff0: 4167 4241 4144 5141 4141 416d 4141 4141  AgBAADQAAAAmAAAA
 00002000: 4777 4141 4141 3841 4141 4142 4141 4141  GwAAAA8AAAABAAAA
 00002010: 4954 2b2f 2f38 4141 4145 4345 4141 4141  IT+//8AAAECEAAAA
 00002020: 4341 4141 4141 4541 4141 4141 4141 4141  CAAAAAEAAAAAAAAA
 00002030: 4134 4141 4142 6661 476c 7763 324e 6864  A4AAABfaGlwc2Nhd
 00002040: 4639 7062 6d52 6c65 4141 4166 762f 2f2f  F9pbmRleAAAfv///
@@ -546,10 +546,10 @@
 00002210: 4167 4142 6741 4841 4177 4141 4141 5141  AgABgAHAAwAAAAQA
 00002220: 4241 4141 4141 4141 4145 4345 4141 4141  BAAAAAAAAECEAAAA
 00002230: 4277 4141 4141 4541 4141 4141 4141 4141  BwAAAAEAAAAAAAAA
 00002240: 4149 4141 4142 705a 4141 4143 4141 4d41  AIAAABpZAAACAAMA
 00002250: 4167 4142 7741 4941 4141 4141 4141 4141  AgABwAIAAAAAAAAA
 00002260: 5541 4141 4141 3d00 1820 7061 7271 7565  UAAAAA=.. parque
 00002270: 742d 6370 702d 6172 726f 7720 7665 7273  t-cpp-arrow vers
-00002280: 696f 6e20 3134 2e30 2e31 199c 1c00 001c  ion 14.0.1......
+00002280: 696f 6e20 3136 2e30 2e30 199c 1c00 001c  ion 16.0.0......
 00002290: 0000 1c00 001c 0000 1c00 001c 0000 1c00  ................
 000022a0: 001c 0000 1c00 0000 d512 0000 5041 5231  ............PAR1
```

### Comparing `hipscat-0.3.3/tests/data/small_sky/_common_metadata` & `hipscat-0.3.4/tests/data/small_sky/_common_metadata`

 * *Files 2% similar despite different names*

```diff
@@ -82,17 +82,17 @@
 00000510: 7822 2c20 2270 616e 6461 735f 7479 7065  x", "pandas_type
 00000520: 223a 2022 7569 6e74 3634 222c 2022 6e75  ": "uint64", "nu
 00000530: 6d70 795f 7479 7065 223a 2022 7569 6e74  mpy_type": "uint
 00000540: 3634 222c 2022 6d65 7461 6461 7461 223a  64", "metadata":
 00000550: 206e 756c 6c7d 5d2c 2022 6372 6561 746f   null}], "creato
 00000560: 7222 3a20 7b22 6c69 6272 6172 7922 3a20  r": {"library": 
 00000570: 2270 7961 7272 6f77 222c 2022 7665 7273  "pyarrow", "vers
-00000580: 696f 6e22 3a20 2231 342e 302e 3122 7d2c  ion": "14.0.1"},
+00000580: 696f 6e22 3a20 2231 362e 302e 3022 7d2c  ion": "16.0.0"},
 00000590: 2022 7061 6e64 6173 5f76 6572 7369 6f6e   "pandas_version
-000005a0: 223a 2022 322e 302e 3322 7d00 180c 4152  ": "2.0.3"}...AR
+000005a0: 223a 2022 322e 322e 3222 7d00 180c 4152  ": "2.2.2"}...AR
 000005b0: 524f 573a 7363 6865 6d61 18ac 132f 2f2f  ROW:schema...///
 000005c0: 2f2f 7a67 4841 4141 5141 4141 4141 4141  //zgHAAAQAAAAAAA
 000005d0: 4b41 4134 4142 6741 4641 4167 4143 6741  KAA4ABgAFAAgACgA
 000005e0: 4141 4141 4242 4141 5141 4141 4141 4141  AAAABBAAQAAAAAAA
 000005f0: 4b41 4177 4141 4141 4541 4167 4143 6741  KAAwAAAAEAAgACgA
 00000600: 4141 4351 4641 4141 4541 4141 4141 5141  AACQFAAAEAAAAAQA
 00000610: 4141 4177 4141 4141 4941 4177 4142 4141  AAAwAAAAIAAwABAA
@@ -196,18 +196,18 @@
 00000c30: 694c 4341 6962 6e56 7463 486c 6664 486c  iLCAibnVtcHlfdHl
 00000c40: 775a 5349 3649 434a 3161 5735 304e 6a51  wZSI6ICJ1aW50NjQ
 00000c50: 694c 4341 6962 5756 3059 5752 6864 4745  iLCAibWV0YWRhdGE
 00000c60: 694f 6942 7564 5778 7366 5630 7349 434a  iOiBudWxsfV0sICJ
 00000c70: 6a63 6d56 6864 4739 7949 6a6f 6765 794a  jcmVhdG9yIjogeyJ
 00000c80: 7361 574a 7959 584a 3549 6a6f 6749 6e42  saWJyYXJ5IjogInB
 00000c90: 3559 584a 7962 3363 694c 4341 6964 6d56  5YXJyb3ciLCAidmV
-00000ca0: 7963 326c 7662 6949 3649 4349 784e 4334  yc2lvbiI6ICIxNC4
-00000cb0: 774c 6a45 6966 5377 6749 6e42 6862 6d52  wLjEifSwgInBhbmR
+00000ca0: 7963 326c 7662 6949 3649 4349 784e 6934  yc2lvbiI6ICIxNi4
+00000cb0: 774c 6a41 6966 5377 6749 6e42 6862 6d52  wLjAifSwgInBhbmR
 00000cc0: 6863 3139 325a 584a 7a61 5739 7549 6a6f  hc192ZXJzaW9uIjo
-00000cd0: 6749 6a49 754d 4334 7a49 6e30 4143 5141  gIjIuMC4zIn0ACQA
+00000cd0: 6749 6a49 754d 6934 7949 6e30 4143 5141  gIjIuMi4yIn0ACQA
 00000ce0: 4141 4c41 4241 4142 7341 5141 4151 4145  AALABAABsAQAAQAE
 00000cf0: 4141 4167 4241 4144 5141 4141 416d 4141  AAAgBAADQAAAAmAA
 00000d00: 4141 4777 4141 4141 3841 4141 4142 4141  AAGwAAAA8AAAABAA
 00000d10: 4141 4954 2b2f 2f38 4141 4145 4345 4141  AAIT+//8AAAECEAA
 00000d20: 4141 4341 4141 4141 4541 4141 4141 4141  AACAAAAAEAAAAAAA
 00000d30: 4141 4134 4141 4142 6661 476c 7763 324e  AAA4AAABfaGlwc2N
 00000d40: 6864 4639 7062 6d52 6c65 4141 4166 762f  hdF9pbmRleAAAfv/
@@ -242,11 +242,11 @@
 00000f10: 5541 4167 4142 6741 4841 4177 4141 4141  UAAgABgAHAAwAAAA
 00000f20: 5141 4241 4141 4141 4141 4145 4345 4141  QABAAAAAAAAECEAA
 00000f30: 4141 4277 4141 4141 4541 4141 4141 4141  AABwAAAAEAAAAAAA
 00000f40: 4141 4149 4141 4142 705a 4141 4143 4141  AAAIAAABpZAAACAA
 00000f50: 4d41 4167 4142 7741 4941 4141 4141 4141  MAAgABwAIAAAAAAA
 00000f60: 4141 5541 4141 4141 3d00 1820 7061 7271  AAUAAAAA=.. parq
 00000f70: 7565 742d 6370 702d 6172 726f 7720 7665  uet-cpp-arrow ve
-00000f80: 7273 696f 6e20 3134 2e30 2e31 199c 1c00  rsion 14.0.1....
+00000f80: 7273 696f 6e20 3136 2e30 2e30 199c 1c00  rsion 16.0.0....
 00000f90: 001c 0000 1c00 001c 0000 1c00 001c 0000  ................
 00000fa0: 1c00 001c 0000 1c00 0000 a60f 0000 5041  ..............PA
 00000fb0: 5231                                     R1
```

### Comparing `hipscat-0.3.3/tests/data/small_sky/_metadata` & `hipscat-0.3.4/tests/data/small_sky/_metadata`

 * *Files 1% similar despite different names*

```diff
@@ -152,17 +152,17 @@
 00000970: 6461 735f 7479 7065 223a 2022 7569 6e74  das_type": "uint
 00000980: 3634 222c 2022 6e75 6d70 795f 7479 7065  64", "numpy_type
 00000990: 223a 2022 7569 6e74 3634 222c 2022 6d65  ": "uint64", "me
 000009a0: 7461 6461 7461 223a 206e 756c 6c7d 5d2c  tadata": null}],
 000009b0: 2022 6372 6561 746f 7222 3a20 7b22 6c69   "creator": {"li
 000009c0: 6272 6172 7922 3a20 2270 7961 7272 6f77  brary": "pyarrow
 000009d0: 222c 2022 7665 7273 696f 6e22 3a20 2231  ", "version": "1
-000009e0: 342e 302e 3122 7d2c 2022 7061 6e64 6173  4.0.1"}, "pandas
-000009f0: 5f76 6572 7369 6f6e 223a 2022 322e 302e  _version": "2.0.
-00000a00: 3322 7d00 180c 4152 524f 573a 7363 6865  3"}...ARROW:sche
+000009e0: 362e 302e 3022 7d2c 2022 7061 6e64 6173  6.0.0"}, "pandas
+000009f0: 5f76 6572 7369 6f6e 223a 2022 322e 322e  _version": "2.2.
+00000a00: 3222 7d00 180c 4152 524f 573a 7363 6865  2"}...ARROW:sche
 00000a10: 6d61 18ac 132f 2f2f 2f2f 7a67 4841 4141  ma.../////zgHAAA
 00000a20: 5141 4141 4141 4141 4b41 4134 4142 6741  QAAAAAAAKAA4ABgA
 00000a30: 4641 4167 4143 6741 4141 4141 4242 4141  FAAgACgAAAAABBAA
 00000a40: 5141 4141 4141 4141 4b41 4177 4141 4141  QAAAAAAAKAAwAAAA
 00000a50: 4541 4167 4143 6741 4141 4351 4641 4141  EAAgACgAAACQFAAA
 00000a60: 4541 4141 4141 5141 4141 4177 4141 4141  EAAAAAQAAAAwAAAA
 00000a70: 4941 4177 4142 4141 4941 4167 4141 4141  IAAwABAAIAAgAAAA
@@ -266,18 +266,18 @@
 00001090: 7463 486c 6664 486c 775a 5349 3649 434a  tcHlfdHlwZSI6ICJ
 000010a0: 3161 5735 304e 6a51 694c 4341 6962 5756  1aW50NjQiLCAibWV
 000010b0: 3059 5752 6864 4745 694f 6942 7564 5778  0YWRhdGEiOiBudWx
 000010c0: 7366 5630 7349 434a 6a63 6d56 6864 4739  sfV0sICJjcmVhdG9
 000010d0: 7949 6a6f 6765 794a 7361 574a 7959 584a  yIjogeyJsaWJyYXJ
 000010e0: 3549 6a6f 6749 6e42 3559 584a 7962 3363  5IjogInB5YXJyb3c
 000010f0: 694c 4341 6964 6d56 7963 326c 7662 6949  iLCAidmVyc2lvbiI
-00001100: 3649 4349 784e 4334 774c 6a45 6966 5377  6ICIxNC4wLjEifSw
+00001100: 3649 4349 784e 6934 774c 6a41 6966 5377  6ICIxNi4wLjAifSw
 00001110: 6749 6e42 6862 6d52 6863 3139 325a 584a  gInBhbmRhc192ZXJ
-00001120: 7a61 5739 7549 6a6f 6749 6a49 754d 4334  zaW9uIjogIjIuMC4
-00001130: 7a49 6e30 4143 5141 4141 4c41 4241 4142  zIn0ACQAAALABAAB
+00001120: 7a61 5739 7549 6a6f 6749 6a49 754d 6934  zaW9uIjogIjIuMi4
+00001130: 7949 6e30 4143 5141 4141 4c41 4241 4142  yIn0ACQAAALABAAB
 00001140: 7341 5141 4151 4145 4141 4167 4241 4144  sAQAAQAEAAAgBAAD
 00001150: 5141 4141 416d 4141 4141 4777 4141 4141  QAAAAmAAAAGwAAAA
 00001160: 3841 4141 4142 4141 4141 4954 2b2f 2f38  8AAAABAAAAIT+//8
 00001170: 4141 4145 4345 4141 4141 4341 4141 4141  AAAECEAAAACAAAAA
 00001180: 4541 4141 4141 4141 4141 4134 4141 4142  EAAAAAAAAAA4AAAB
 00001190: 6661 476c 7763 324e 6864 4639 7062 6d52  faGlwc2NhdF9pbmR
 000011a0: 6c65 4141 4166 762f 2f2f 3041 4141 4143  leAAAfv///0AAAAC
@@ -311,11 +311,11 @@
 00001360: 4141 4149 4145 4141 5541 4167 4142 6741  AAAIAEAAUAAgABgA
 00001370: 4841 4177 4141 4141 5141 4241 4141 4141  HAAwAAAAQABAAAAA
 00001380: 4141 4145 4345 4141 4141 4277 4141 4141  AAAECEAAAABwAAAA
 00001390: 4541 4141 4141 4141 4141 4149 4141 4142  EAAAAAAAAAAIAAAB
 000013a0: 705a 4141 4143 4141 4d41 4167 4142 7741  pZAAACAAMAAgABwA
 000013b0: 4941 4141 4141 4141 4141 5541 4141 4141  IAAAAAAAAAUAAAAA
 000013c0: 3d00 1820 7061 7271 7565 742d 6370 702d  =.. parquet-cpp-
-000013d0: 6172 726f 7720 7665 7273 696f 6e20 3134  arrow version 14
-000013e0: 2e30 2e31 199c 1c00 001c 0000 1c00 001c  .0.1............
+000013d0: 6172 726f 7720 7665 7273 696f 6e20 3136  arrow version 16
+000013e0: 2e30 2e30 199c 1c00 001c 0000 1c00 001c  .0.0............
 000013f0: 0000 1c00 001c 0000 1c00 001c 0000 1c00  ................
 00001400: 0000 fe13 0000 5041 5231                 ......PAR1
```

### Comparing `hipscat-0.3.3/tests/data/small_sky/point_map.fits` & `hipscat-0.3.4/tests/data/small_sky/point_map.fits`

 * *Files 2% similar despite different names*

```diff
@@ -229,16 +229,16 @@
 00000e40: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00000e50: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00000e60: 5049 5854 5950 4520 3d20 2748 4541 4c50  PIXTYPE = 'HEALP
 00000e70: 4958 2027 2020 2020 2020 2020 2020 202f  IX '           /
 00000e80: 2048 4541 4c50 4958 2070 6978 656c 6973   HEALPIX pixelis
 00000e90: 6174 696f 6e20 2020 2020 2020 2020 2020  ation           
 00000ea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000eb0: 4f52 4445 5249 4e47 3d20 2752 494e 4720  ORDERING= 'RING 
-00000ec0: 2020 2027 2020 2020 2020 2020 2020 202f     '           /
+00000eb0: 4f52 4445 5249 4e47 3d20 274e 4553 5445  ORDERING= 'NESTE
+00000ec0: 4420 2027 2020 2020 2020 2020 2020 202f  D  '           /
 00000ed0: 2050 6978 656c 206f 7264 6572 696e 6720   Pixel ordering 
 00000ee0: 7363 6865 6d65 2c20 6569 7468 6572 2052  scheme, either R
 00000ef0: 494e 4720 6f72 204e 4553 5445 4420 2020  ING or NESTED   
 00000f00: 4558 544e 414d 4520 3d20 2778 7465 6e73  EXTNAME = 'xtens
 00000f10: 696f 6e27 2020 2020 2020 2020 2020 202f  ion'           /
 00000f20: 206e 616d 6520 6f66 2074 6869 7320 6269   name of this bi
 00000f30: 6e61 7279 2074 6162 6c65 2065 7874 656e  nary table exten
```

### Comparing `hipscat-0.3.3/tests/data/small_sky/provenance_info.json` & `hipscat-0.3.4/tests/data/small_sky_order1/provenance_info.json`

 * *Files 24% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8212639079408627%*

 * *Differences: {"'catalog_name'": "'small_sky_order1'",*

 * * "'generation_date'": "'2024.05.29'",*

 * * "'tool_args'": "{'version': '0.3.3.dev10+gd573bcd', 'runtime_args': {'catalog_name': "*

 * *                "'small_sky_order1', 'output_path': '.', 'output_artifact_name': "*

 * *                "'small_sky_order1', 'tmp_dir': '/tmp/tmpgasth6x_', 'catalog_path': "*

 * *                "'./small_sky_order1', 'tmp_path': "*

 * *                "'/tmp/tmpgasth6x_/small_sky_order1/intermediate', 'input_path': "*

 * *                "'../../../hipscat-impor […]*

```diff
@@ -1,52 +1,52 @@
 {
-    "catalog_name": "small_sky",
+    "catalog_name": "small_sky_order1",
     "catalog_type": "object",
     "dec_column": "dec",
     "epoch": "J2000",
-    "generation_date": "2024.01.09",
+    "generation_date": "2024.05.29",
     "ra_column": "ra",
     "tool_args": {
         "runtime_args": {
-            "catalog_name": "small_sky",
-            "catalog_path": "/home/delucchi/git/hipscat/tests/data/small_sky",
+            "catalog_name": "small_sky_order1",
+            "catalog_path": "./small_sky_order1",
             "catalog_type": "object",
-            "constant_healpix_order": -1,
+            "constant_healpix_order": 1,
             "dask_n_workers": 1,
             "dask_threads_per_worker": 1,
             "dask_tmp": "",
             "debug_stats_only": false,
             "dec_column": "dec",
             "epoch": "J2000",
             "file_reader_info": {
                 "chunksize": 500000,
                 "column_names": null,
                 "header": "infer",
                 "input_reader_type": "CsvReader",
+                "kwargs": {},
+                "parquet_kwargs": null,
                 "schema_file": null,
-                "separator": ",",
-                "type_map": {}
+                "type_map": null
             },
             "highest_healpix_order": 7,
             "input_file_list": [],
-            "input_format": "csv",
-            "input_path": "/home/delucchi/git/hipscat-import/tests/hipscat_import/data/small_sky",
+            "input_path": "../../../hipscat-import/tests/hipscat_import/data/small_sky",
             "input_paths": [
-                "file:///home/delucchi/git/hipscat-import/tests/hipscat_import/data/small_sky/catalog.csv"
+                "file:///home/delucchi/git/fits/tests/data/../../../hipscat-import/tests/hipscat_import/data/small_sky/catalog.csv"
             ],
-            "mapping_healpix_order": 7,
-            "output_artifact_name": "small_sky",
-            "output_path": "/home/delucchi/git/hipscat/tests/data/",
-            "overwrite": true,
+            "lowest_healpix_order": 0,
+            "mapping_healpix_order": 1,
+            "output_artifact_name": "small_sky_order1",
+            "output_path": ".",
             "pixel_threshold": 1000000,
             "ra_column": "ra",
             "sort_columns": null,
-            "tmp_dir": "",
-            "tmp_path": "/home/delucchi/git/hipscat/tests/data/small_sky/intermediate",
+            "tmp_dir": "/tmp/tmpgasth6x_",
+            "tmp_path": "/tmp/tmpgasth6x_/small_sky_order1/intermediate",
             "use_hipscat_index": false
         },
         "tool_name": "hipscat_import",
-        "version": "0.2.1"
+        "version": "0.3.3.dev10+gd573bcd"
     },
     "total_rows": 131,
-    "version": "0.2.1"
+    "version": "0.3.4.dev17+g922a4b7.d20240529"
 }
```

### Comparing `hipscat-0.3.3/tests/data/small_sky_order1/Norder=1/Dir=0/Npix=44.parquet` & `hipscat-0.3.4/tests/data/small_sky_order1/Norder=1/Dir=0/Npix=44.parquet`

 * *Files 4% similar despite different names*

```diff
@@ -282,17 +282,17 @@
 00001190: 6461 735f 7479 7065 223a 2022 7569 6e74  das_type": "uint
 000011a0: 3634 222c 2022 6e75 6d70 795f 7479 7065  64", "numpy_type
 000011b0: 223a 2022 7569 6e74 3634 222c 2022 6d65  ": "uint64", "me
 000011c0: 7461 6461 7461 223a 206e 756c 6c7d 5d2c  tadata": null}],
 000011d0: 2022 6372 6561 746f 7222 3a20 7b22 6c69   "creator": {"li
 000011e0: 6272 6172 7922 3a20 2270 7961 7272 6f77  brary": "pyarrow
 000011f0: 222c 2022 7665 7273 696f 6e22 3a20 2231  ", "version": "1
-00001200: 342e 302e 3122 7d2c 2022 7061 6e64 6173  4.0.1"}, "pandas
-00001210: 5f76 6572 7369 6f6e 223a 2022 322e 302e  _version": "2.0.
-00001220: 3322 7d00 180c 4152 524f 573a 7363 6865  3"}...ARROW:sche
+00001200: 362e 302e 3022 7d2c 2022 7061 6e64 6173  6.0.0"}, "pandas
+00001210: 5f76 6572 7369 6f6e 223a 2022 322e 322e  _version": "2.2.
+00001220: 3222 7d00 180c 4152 524f 573a 7363 6865  2"}...ARROW:sche
 00001230: 6d61 18ac 132f 2f2f 2f2f 7a67 4841 4141  ma.../////zgHAAA
 00001240: 5141 4141 4141 4141 4b41 4134 4142 6741  QAAAAAAAKAA4ABgA
 00001250: 4641 4167 4143 6741 4141 4141 4242 4141  FAAgACgAAAAABBAA
 00001260: 5141 4141 4141 4141 4b41 4177 4141 4141  QAAAAAAAKAAwAAAA
 00001270: 4541 4167 4143 6741 4141 4351 4641 4141  EAAgACgAAACQFAAA
 00001280: 4541 4141 4141 5141 4141 4177 4141 4141  EAAAAAQAAAAwAAAA
 00001290: 4941 4177 4142 4141 4941 4167 4141 4141  IAAwABAAIAAgAAAA
@@ -396,18 +396,18 @@
 000018b0: 7463 486c 6664 486c 775a 5349 3649 434a  tcHlfdHlwZSI6ICJ
 000018c0: 3161 5735 304e 6a51 694c 4341 6962 5756  1aW50NjQiLCAibWV
 000018d0: 3059 5752 6864 4745 694f 6942 7564 5778  0YWRhdGEiOiBudWx
 000018e0: 7366 5630 7349 434a 6a63 6d56 6864 4739  sfV0sICJjcmVhdG9
 000018f0: 7949 6a6f 6765 794a 7361 574a 7959 584a  yIjogeyJsaWJyYXJ
 00001900: 3549 6a6f 6749 6e42 3559 584a 7962 3363  5IjogInB5YXJyb3c
 00001910: 694c 4341 6964 6d56 7963 326c 7662 6949  iLCAidmVyc2lvbiI
-00001920: 3649 4349 784e 4334 774c 6a45 6966 5377  6ICIxNC4wLjEifSw
+00001920: 3649 4349 784e 6934 774c 6a41 6966 5377  6ICIxNi4wLjAifSw
 00001930: 6749 6e42 6862 6d52 6863 3139 325a 584a  gInBhbmRhc192ZXJ
-00001940: 7a61 5739 7549 6a6f 6749 6a49 754d 4334  zaW9uIjogIjIuMC4
-00001950: 7a49 6e30 4143 5141 4141 4c41 4241 4142  zIn0ACQAAALABAAB
+00001940: 7a61 5739 7549 6a6f 6749 6a49 754d 6934  zaW9uIjogIjIuMi4
+00001950: 7949 6e30 4143 5141 4141 4c41 4241 4142  yIn0ACQAAALABAAB
 00001960: 7341 5141 4151 4145 4141 4167 4241 4144  sAQAAQAEAAAgBAAD
 00001970: 5141 4141 416d 4141 4141 4777 4141 4141  QAAAAmAAAAGwAAAA
 00001980: 3841 4141 4142 4141 4141 4954 2b2f 2f38  8AAAABAAAAIT+//8
 00001990: 4141 4145 4345 4141 4141 4341 4141 4141  AAAECEAAAACAAAAA
 000019a0: 4541 4141 4141 4141 4141 4134 4141 4142  EAAAAAAAAAA4AAAB
 000019b0: 6661 476c 7763 324e 6864 4639 7062 6d52  faGlwc2NhdF9pbmR
 000019c0: 6c65 4141 4166 762f 2f2f 3041 4141 4143  leAAAfv///0AAAAC
@@ -441,11 +441,11 @@
 00001b80: 4141 4149 4145 4141 5541 4167 4142 6741  AAAIAEAAUAAgABgA
 00001b90: 4841 4177 4141 4141 5141 4241 4141 4141  HAAwAAAAQABAAAAA
 00001ba0: 4141 4145 4345 4141 4141 4277 4141 4141  AAAECEAAAABwAAAA
 00001bb0: 4541 4141 4141 4141 4141 4149 4141 4142  EAAAAAAAAAAIAAAB
 00001bc0: 705a 4141 4143 4141 4d41 4167 4142 7741  pZAAACAAMAAgABwA
 00001bd0: 4941 4141 4141 4141 4141 5541 4141 4141  IAAAAAAAAAUAAAAA
 00001be0: 3d00 1820 7061 7271 7565 742d 6370 702d  =.. parquet-cpp-
-00001bf0: 6172 726f 7720 7665 7273 696f 6e20 3134  arrow version 14
-00001c00: 2e30 2e31 199c 1c00 001c 0000 1c00 001c  .0.1............
+00001bf0: 6172 726f 7720 7665 7273 696f 6e20 3136  arrow version 16
+00001c00: 2e30 2e30 199c 1c00 001c 0000 1c00 001c  .0.0............
 00001c10: 0000 1c00 001c 0000 1c00 001c 0000 1c00  ................
 00001c20: 0000 ca12 0000 5041 5231                 ......PAR1
```

### Comparing `hipscat-0.3.3/tests/data/small_sky_order1/Norder=1/Dir=0/Npix=45.parquet` & `hipscat-0.3.4/tests/data/small_sky_order1/Norder=1/Dir=0/Npix=45.parquet`

 * *Files 1% similar despite different names*

```diff
@@ -267,17 +267,17 @@
 000010a0: 7061 6e64 6173 5f74 7970 6522 3a20 2275  pandas_type": "u
 000010b0: 696e 7436 3422 2c20 226e 756d 7079 5f74  int64", "numpy_t
 000010c0: 7970 6522 3a20 2275 696e 7436 3422 2c20  ype": "uint64", 
 000010d0: 226d 6574 6164 6174 6122 3a20 6e75 6c6c  "metadata": null
 000010e0: 7d5d 2c20 2263 7265 6174 6f72 223a 207b  }], "creator": {
 000010f0: 226c 6962 7261 7279 223a 2022 7079 6172  "library": "pyar
 00001100: 726f 7722 2c20 2276 6572 7369 6f6e 223a  row", "version":
-00001110: 2022 3134 2e30 2e31 227d 2c20 2270 616e   "14.0.1"}, "pan
+00001110: 2022 3136 2e30 2e30 227d 2c20 2270 616e   "16.0.0"}, "pan
 00001120: 6461 735f 7665 7273 696f 6e22 3a20 2232  das_version": "2
-00001130: 2e30 2e33 227d 0018 0c41 5252 4f57 3a73  .0.3"}...ARROW:s
+00001130: 2e32 2e32 227d 0018 0c41 5252 4f57 3a73  .2.2"}...ARROW:s
 00001140: 6368 656d 6118 ac13 2f2f 2f2f 2f7a 6748  chema.../////zgH
 00001150: 4141 4151 4141 4141 4141 414b 4141 3441  AAAQAAAAAAAKAA4A
 00001160: 4267 4146 4141 6741 4367 4141 4141 4142  BgAFAAgACgAAAAAB
 00001170: 4241 4151 4141 4141 4141 414b 4141 7741  BAAQAAAAAAAKAAwA
 00001180: 4141 4145 4141 6741 4367 4141 4143 5146  AAAEAAgACgAAACQF
 00001190: 4141 4145 4141 4141 4151 4141 4141 7741  AAAEAAAAAQAAAAwA
 000011a0: 4141 4149 4141 7741 4241 4149 4141 6741  AAAIAAwABAAIAAgA
@@ -381,18 +381,18 @@
 000017c0: 626e 5674 6348 6c66 6448 6c77 5a53 4936  bnVtcHlfdHlwZSI6
 000017d0: 4943 4a31 6157 3530 4e6a 5169 4c43 4169  ICJ1aW50NjQiLCAi
 000017e0: 6257 5630 5957 5268 6447 4569 4f69 4275  bWV0YWRhdGEiOiBu
 000017f0: 6457 7873 6656 3073 4943 4a6a 636d 5668  dWxsfV0sICJjcmVh
 00001800: 6447 3979 496a 6f67 6579 4a73 6157 4a79  dG9yIjogeyJsaWJy
 00001810: 5958 4a35 496a 6f67 496e 4235 5958 4a79  YXJ5IjogInB5YXJy
 00001820: 6233 6369 4c43 4169 646d 5679 6332 6c76  b3ciLCAidmVyc2lv
-00001830: 6269 4936 4943 4978 4e43 3477 4c6a 4569  biI6ICIxNC4wLjEi
+00001830: 6269 4936 4943 4978 4e69 3477 4c6a 4169  biI6ICIxNi4wLjAi
 00001840: 6653 7767 496e 4268 626d 5268 6331 3932  fSwgInBhbmRhc192
 00001850: 5a58 4a7a 6157 3975 496a 6f67 496a 4975  ZXJzaW9uIjogIjIu
-00001860: 4d43 347a 496e 3041 4351 4141 414c 4142  MC4zIn0ACQAAALAB
+00001860: 4d69 3479 496e 3041 4351 4141 414c 4142  Mi4yIn0ACQAAALAB
 00001870: 4141 4273 4151 4141 5141 4541 4141 6742  AABsAQAAQAEAAAgB
 00001880: 4141 4451 4141 4141 6d41 4141 4147 7741  AADQAAAAmAAAAGwA
 00001890: 4141 4138 4141 4141 4241 4141 4149 542b  AAA8AAAABAAAAIT+
 000018a0: 2f2f 3841 4141 4543 4541 4141 4143 4141  //8AAAECEAAAACAA
 000018b0: 4141 4145 4141 4141 4141 4141 4141 3441  AAAEAAAAAAAAAA4A
 000018c0: 4141 4266 6147 6c77 6332 4e68 6446 3970  AABfaGlwc2NhdF9p
 000018d0: 626d 526c 6541 4141 6676 2f2f 2f30 4141  bmRleAAAfv///0AA
@@ -427,10 +427,10 @@
 00001aa0: 4267 4148 4141 7741 4141 4151 4142 4141  BgAHAAwAAAAQABAA
 00001ab0: 4141 4141 4141 4543 4541 4141 4142 7741  AAAAAAECEAAAABwA
 00001ac0: 4141 4145 4141 4141 4141 4141 4141 4941  AAAEAAAAAAAAAAIA
 00001ad0: 4141 4270 5a41 4141 4341 414d 4141 6741  AABpZAAACAAMAAgA
 00001ae0: 4277 4149 4141 4141 4141 4141 4155 4141  BwAIAAAAAAAAAUAA
 00001af0: 4141 413d 0018 2070 6172 7175 6574 2d63  AAA=.. parquet-c
 00001b00: 7070 2d61 7272 6f77 2076 6572 7369 6f6e  pp-arrow version
-00001b10: 2031 342e 302e 3119 9c1c 0000 1c00 001c   14.0.1.........
+00001b10: 2031 362e 302e 3019 9c1c 0000 1c00 001c   16.0.0.........
 00001b20: 0000 1c00 001c 0000 1c00 001c 0000 1c00  ................
 00001b30: 001c 0000 00ca 1200 0050 4152 31         .........PAR1
```

### Comparing `hipscat-0.3.3/tests/data/small_sky_order1/Norder=1/Dir=0/Npix=46.parquet` & `hipscat-0.3.4/tests/data/small_sky_order1/Norder=1/Dir=0/Npix=46.parquet`

 * *Files 2% similar despite different names*

```diff
@@ -282,17 +282,17 @@
 00001190: 2c20 2270 616e 6461 735f 7479 7065 223a  , "pandas_type":
 000011a0: 2022 7569 6e74 3634 222c 2022 6e75 6d70   "uint64", "nump
 000011b0: 795f 7479 7065 223a 2022 7569 6e74 3634  y_type": "uint64
 000011c0: 222c 2022 6d65 7461 6461 7461 223a 206e  ", "metadata": n
 000011d0: 756c 6c7d 5d2c 2022 6372 6561 746f 7222  ull}], "creator"
 000011e0: 3a20 7b22 6c69 6272 6172 7922 3a20 2270  : {"library": "p
 000011f0: 7961 7272 6f77 222c 2022 7665 7273 696f  yarrow", "versio
-00001200: 6e22 3a20 2231 342e 302e 3122 7d2c 2022  n": "14.0.1"}, "
+00001200: 6e22 3a20 2231 362e 302e 3022 7d2c 2022  n": "16.0.0"}, "
 00001210: 7061 6e64 6173 5f76 6572 7369 6f6e 223a  pandas_version":
-00001220: 2022 322e 302e 3322 7d00 180c 4152 524f   "2.0.3"}...ARRO
+00001220: 2022 322e 322e 3222 7d00 180c 4152 524f   "2.2.2"}...ARRO
 00001230: 573a 7363 6865 6d61 18ac 132f 2f2f 2f2f  W:schema.../////
 00001240: 7a67 4841 4141 5141 4141 4141 4141 4b41  zgHAAAQAAAAAAAKA
 00001250: 4134 4142 6741 4641 4167 4143 6741 4141  A4ABgAFAAgACgAAA
 00001260: 4141 4242 4141 5141 4141 4141 4141 4b41  AABBAAQAAAAAAAKA
 00001270: 4177 4141 4141 4541 4167 4143 6741 4141  AwAAAAEAAgACgAAA
 00001280: 4351 4641 4141 4541 4141 4141 5141 4141  CQFAAAEAAAAAQAAA
 00001290: 4177 4141 4141 4941 4177 4142 4141 4941  AwAAAAIAAwABAAIA
@@ -396,18 +396,18 @@
 000018b0: 4341 6962 6e56 7463 486c 6664 486c 775a  CAibnVtcHlfdHlwZ
 000018c0: 5349 3649 434a 3161 5735 304e 6a51 694c  SI6ICJ1aW50NjQiL
 000018d0: 4341 6962 5756 3059 5752 6864 4745 694f  CAibWV0YWRhdGEiO
 000018e0: 6942 7564 5778 7366 5630 7349 434a 6a63  iBudWxsfV0sICJjc
 000018f0: 6d56 6864 4739 7949 6a6f 6765 794a 7361  mVhdG9yIjogeyJsa
 00001900: 574a 7959 584a 3549 6a6f 6749 6e42 3559  WJyYXJ5IjogInB5Y
 00001910: 584a 7962 3363 694c 4341 6964 6d56 7963  XJyb3ciLCAidmVyc
-00001920: 326c 7662 6949 3649 4349 784e 4334 774c  2lvbiI6ICIxNC4wL
-00001930: 6a45 6966 5377 6749 6e42 6862 6d52 6863  jEifSwgInBhbmRhc
+00001920: 326c 7662 6949 3649 4349 784e 6934 774c  2lvbiI6ICIxNi4wL
+00001930: 6a41 6966 5377 6749 6e42 6862 6d52 6863  jAifSwgInBhbmRhc
 00001940: 3139 325a 584a 7a61 5739 7549 6a6f 6749  192ZXJzaW9uIjogI
-00001950: 6a49 754d 4334 7a49 6e30 4143 5141 4141  jIuMC4zIn0ACQAAA
+00001950: 6a49 754d 6934 7949 6e30 4143 5141 4141  jIuMi4yIn0ACQAAA
 00001960: 4c41 4241 4142 7341 5141 4151 4145 4141  LABAABsAQAAQAEAA
 00001970: 4167 4241 4144 5141 4141 416d 4141 4141  AgBAADQAAAAmAAAA
 00001980: 4777 4141 4141 3841 4141 4142 4141 4141  GwAAAA8AAAABAAAA
 00001990: 4954 2b2f 2f38 4141 4145 4345 4141 4141  IT+//8AAAECEAAAA
 000019a0: 4341 4141 4141 4541 4141 4141 4141 4141  CAAAAAEAAAAAAAAA
 000019b0: 4134 4141 4142 6661 476c 7763 324e 6864  A4AAABfaGlwc2Nhd
 000019c0: 4639 7062 6d52 6c65 4141 4166 762f 2f2f  F9pbmRleAAAfv///
@@ -442,10 +442,10 @@
 00001b90: 4167 4142 6741 4841 4177 4141 4141 5141  AgABgAHAAwAAAAQA
 00001ba0: 4241 4141 4141 4141 4145 4345 4141 4141  BAAAAAAAAECEAAAA
 00001bb0: 4277 4141 4141 4541 4141 4141 4141 4141  BwAAAAEAAAAAAAAA
 00001bc0: 4149 4141 4142 705a 4141 4143 4141 4d41  AIAAABpZAAACAAMA
 00001bd0: 4167 4142 7741 4941 4141 4141 4141 4141  AgABwAIAAAAAAAAA
 00001be0: 5541 4141 4141 3d00 1820 7061 7271 7565  UAAAAA=.. parque
 00001bf0: 742d 6370 702d 6172 726f 7720 7665 7273  t-cpp-arrow vers
-00001c00: 696f 6e20 3134 2e30 2e31 199c 1c00 001c  ion 14.0.1......
+00001c00: 696f 6e20 3136 2e30 2e30 199c 1c00 001c  ion 16.0.0......
 00001c10: 0000 1c00 001c 0000 1c00 001c 0000 1c00  ................
 00001c20: 001c 0000 1c00 0000 ca12 0000 5041 5231  ............PAR1
```

### Comparing `hipscat-0.3.3/tests/data/small_sky_order1/Norder=1/Dir=0/Npix=47.parquet` & `hipscat-0.3.4/tests/data/small_sky_order1/Norder=1/Dir=0/Npix=47.parquet`

 * *Files 1% similar despite different names*

```diff
@@ -252,17 +252,17 @@
 00000fb0: 6e64 6578 222c 2022 7061 6e64 6173 5f74  ndex", "pandas_t
 00000fc0: 7970 6522 3a20 2275 696e 7436 3422 2c20  ype": "uint64", 
 00000fd0: 226e 756d 7079 5f74 7970 6522 3a20 2275  "numpy_type": "u
 00000fe0: 696e 7436 3422 2c20 226d 6574 6164 6174  int64", "metadat
 00000ff0: 6122 3a20 6e75 6c6c 7d5d 2c20 2263 7265  a": null}], "cre
 00001000: 6174 6f72 223a 207b 226c 6962 7261 7279  ator": {"library
 00001010: 223a 2022 7079 6172 726f 7722 2c20 2276  ": "pyarrow", "v
-00001020: 6572 7369 6f6e 223a 2022 3134 2e30 2e31  ersion": "14.0.1
+00001020: 6572 7369 6f6e 223a 2022 3136 2e30 2e30  ersion": "16.0.0
 00001030: 227d 2c20 2270 616e 6461 735f 7665 7273  "}, "pandas_vers
-00001040: 696f 6e22 3a20 2232 2e30 2e33 227d 0018  ion": "2.0.3"}..
+00001040: 696f 6e22 3a20 2232 2e32 2e32 227d 0018  ion": "2.2.2"}..
 00001050: 0c41 5252 4f57 3a73 6368 656d 6118 ac13  .ARROW:schema...
 00001060: 2f2f 2f2f 2f7a 6748 4141 4151 4141 4141  /////zgHAAAQAAAA
 00001070: 4141 414b 4141 3441 4267 4146 4141 6741  AAAKAA4ABgAFAAgA
 00001080: 4367 4141 4141 4142 4241 4151 4141 4141  CgAAAAABBAAQAAAA
 00001090: 4141 414b 4141 7741 4141 4145 4141 6741  AAAKAAwAAAAEAAgA
 000010a0: 4367 4141 4143 5146 4141 4145 4141 4141  CgAAACQFAAAEAAAA
 000010b0: 4151 4141 4141 7741 4141 4149 4141 7741  AQAAAAwAAAAIAAwA
@@ -367,17 +367,17 @@
 000016e0: 6448 6c77 5a53 4936 4943 4a31 6157 3530  dHlwZSI6ICJ1aW50
 000016f0: 4e6a 5169 4c43 4169 6257 5630 5957 5268  NjQiLCAibWV0YWRh
 00001700: 6447 4569 4f69 4275 6457 7873 6656 3073  dGEiOiBudWxsfV0s
 00001710: 4943 4a6a 636d 5668 6447 3979 496a 6f67  ICJjcmVhdG9yIjog
 00001720: 6579 4a73 6157 4a79 5958 4a35 496a 6f67  eyJsaWJyYXJ5Ijog
 00001730: 496e 4235 5958 4a79 6233 6369 4c43 4169  InB5YXJyb3ciLCAi
 00001740: 646d 5679 6332 6c76 6269 4936 4943 4978  dmVyc2lvbiI6ICIx
-00001750: 4e43 3477 4c6a 4569 6653 7767 496e 4268  NC4wLjEifSwgInBh
+00001750: 4e69 3477 4c6a 4169 6653 7767 496e 4268  Ni4wLjAifSwgInBh
 00001760: 626d 5268 6331 3932 5a58 4a7a 6157 3975  bmRhc192ZXJzaW9u
-00001770: 496a 6f67 496a 4975 4d43 347a 496e 3041  IjogIjIuMC4zIn0A
+00001770: 496a 6f67 496a 4975 4d69 3479 496e 3041  IjogIjIuMi4yIn0A
 00001780: 4351 4141 414c 4142 4141 4273 4151 4141  CQAAALABAABsAQAA
 00001790: 5141 4541 4141 6742 4141 4451 4141 4141  QAEAAAgBAADQAAAA
 000017a0: 6d41 4141 4147 7741 4141 4138 4141 4141  mAAAAGwAAAA8AAAA
 000017b0: 4241 4141 4149 542b 2f2f 3841 4141 4543  BAAAAIT+//8AAAEC
 000017c0: 4541 4141 4143 4141 4141 4145 4141 4141  EAAAACAAAAAEAAAA
 000017d0: 4141 4141 4141 3441 4141 4266 6147 6c77  AAAAAA4AAABfaGlw
 000017e0: 6332 4e68 6446 3970 626d 526c 6541 4141  c2NhdF9pbmRleAAA
@@ -412,11 +412,11 @@
 000019b0: 4541 4155 4141 6741 4267 4148 4141 7741  EAAUAAgABgAHAAwA
 000019c0: 4141 4151 4142 4141 4141 4141 4141 4543  AAAQABAAAAAAAAEC
 000019d0: 4541 4141 4142 7741 4141 4145 4141 4141  EAAAABwAAAAEAAAA
 000019e0: 4141 4141 4141 4941 4141 4270 5a41 4141  AAAAAAIAAABpZAAA
 000019f0: 4341 414d 4141 6741 4277 4149 4141 4141  CAAMAAgABwAIAAAA
 00001a00: 4141 4141 4155 4141 4141 413d 0018 2070  AAAAAUAAAAA=.. p
 00001a10: 6172 7175 6574 2d63 7070 2d61 7272 6f77  arquet-cpp-arrow
-00001a20: 2076 6572 7369 6f6e 2031 342e 302e 3119   version 14.0.1.
+00001a20: 2076 6572 7369 6f6e 2031 362e 302e 3019   version 16.0.0.
 00001a30: 9c1c 0000 1c00 001c 0000 1c00 001c 0000  ................
 00001a40: 1c00 001c 0000 1c00 001c 0000 00ca 1200  ................
 00001a50: 0050 4152 31                             .PAR1
```

### Comparing `hipscat-0.3.3/tests/data/small_sky_order1/README.md` & `hipscat-0.3.4/tests/data/small_sky_order1/README.md`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.3/tests/data/small_sky_order1/_common_metadata` & `hipscat-0.3.4/tests/data/small_sky_order1/_common_metadata`

 * *Files 2% similar despite different names*

```diff
@@ -82,17 +82,17 @@
 00000510: 7822 2c20 2270 616e 6461 735f 7479 7065  x", "pandas_type
 00000520: 223a 2022 7569 6e74 3634 222c 2022 6e75  ": "uint64", "nu
 00000530: 6d70 795f 7479 7065 223a 2022 7569 6e74  mpy_type": "uint
 00000540: 3634 222c 2022 6d65 7461 6461 7461 223a  64", "metadata":
 00000550: 206e 756c 6c7d 5d2c 2022 6372 6561 746f   null}], "creato
 00000560: 7222 3a20 7b22 6c69 6272 6172 7922 3a20  r": {"library": 
 00000570: 2270 7961 7272 6f77 222c 2022 7665 7273  "pyarrow", "vers
-00000580: 696f 6e22 3a20 2231 342e 302e 3122 7d2c  ion": "14.0.1"},
+00000580: 696f 6e22 3a20 2231 362e 302e 3022 7d2c  ion": "16.0.0"},
 00000590: 2022 7061 6e64 6173 5f76 6572 7369 6f6e   "pandas_version
-000005a0: 223a 2022 322e 302e 3322 7d00 180c 4152  ": "2.0.3"}...AR
+000005a0: 223a 2022 322e 322e 3222 7d00 180c 4152  ": "2.2.2"}...AR
 000005b0: 524f 573a 7363 6865 6d61 18ac 132f 2f2f  ROW:schema...///
 000005c0: 2f2f 7a67 4841 4141 5141 4141 4141 4141  //zgHAAAQAAAAAAA
 000005d0: 4b41 4134 4142 6741 4641 4167 4143 6741  KAA4ABgAFAAgACgA
 000005e0: 4141 4141 4242 4141 5141 4141 4141 4141  AAAABBAAQAAAAAAA
 000005f0: 4b41 4177 4141 4141 4541 4167 4143 6741  KAAwAAAAEAAgACgA
 00000600: 4141 4351 4641 4141 4541 4141 4141 5141  AACQFAAAEAAAAAQA
 00000610: 4141 4177 4141 4141 4941 4177 4142 4141  AAAwAAAAIAAwABAA
@@ -196,18 +196,18 @@
 00000c30: 694c 4341 6962 6e56 7463 486c 6664 486c  iLCAibnVtcHlfdHl
 00000c40: 775a 5349 3649 434a 3161 5735 304e 6a51  wZSI6ICJ1aW50NjQ
 00000c50: 694c 4341 6962 5756 3059 5752 6864 4745  iLCAibWV0YWRhdGE
 00000c60: 694f 6942 7564 5778 7366 5630 7349 434a  iOiBudWxsfV0sICJ
 00000c70: 6a63 6d56 6864 4739 7949 6a6f 6765 794a  jcmVhdG9yIjogeyJ
 00000c80: 7361 574a 7959 584a 3549 6a6f 6749 6e42  saWJyYXJ5IjogInB
 00000c90: 3559 584a 7962 3363 694c 4341 6964 6d56  5YXJyb3ciLCAidmV
-00000ca0: 7963 326c 7662 6949 3649 4349 784e 4334  yc2lvbiI6ICIxNC4
-00000cb0: 774c 6a45 6966 5377 6749 6e42 6862 6d52  wLjEifSwgInBhbmR
+00000ca0: 7963 326c 7662 6949 3649 4349 784e 6934  yc2lvbiI6ICIxNi4
+00000cb0: 774c 6a41 6966 5377 6749 6e42 6862 6d52  wLjAifSwgInBhbmR
 00000cc0: 6863 3139 325a 584a 7a61 5739 7549 6a6f  hc192ZXJzaW9uIjo
-00000cd0: 6749 6a49 754d 4334 7a49 6e30 4143 5141  gIjIuMC4zIn0ACQA
+00000cd0: 6749 6a49 754d 6934 7949 6e30 4143 5141  gIjIuMi4yIn0ACQA
 00000ce0: 4141 4c41 4241 4142 7341 5141 4151 4145  AALABAABsAQAAQAE
 00000cf0: 4141 4167 4241 4144 5141 4141 416d 4141  AAAgBAADQAAAAmAA
 00000d00: 4141 4777 4141 4141 3841 4141 4142 4141  AAGwAAAA8AAAABAA
 00000d10: 4141 4954 2b2f 2f38 4141 4145 4345 4141  AAIT+//8AAAECEAA
 00000d20: 4141 4341 4141 4141 4541 4141 4141 4141  AACAAAAAEAAAAAAA
 00000d30: 4141 4134 4141 4142 6661 476c 7763 324e  AAA4AAABfaGlwc2N
 00000d40: 6864 4639 7062 6d52 6c65 4141 4166 762f  hdF9pbmRleAAAfv/
@@ -242,11 +242,11 @@
 00000f10: 5541 4167 4142 6741 4841 4177 4141 4141  UAAgABgAHAAwAAAA
 00000f20: 5141 4241 4141 4141 4141 4145 4345 4141  QABAAAAAAAAECEAA
 00000f30: 4141 4277 4141 4141 4541 4141 4141 4141  AABwAAAAEAAAAAAA
 00000f40: 4141 4149 4141 4142 705a 4141 4143 4141  AAAIAAABpZAAACAA
 00000f50: 4d41 4167 4142 7741 4941 4141 4141 4141  MAAgABwAIAAAAAAA
 00000f60: 4141 5541 4141 4141 3d00 1820 7061 7271  AAUAAAAA=.. parq
 00000f70: 7565 742d 6370 702d 6172 726f 7720 7665  uet-cpp-arrow ve
-00000f80: 7273 696f 6e20 3134 2e30 2e31 199c 1c00  rsion 14.0.1....
+00000f80: 7273 696f 6e20 3136 2e30 2e30 199c 1c00  rsion 16.0.0....
 00000f90: 001c 0000 1c00 001c 0000 1c00 001c 0000  ................
 00000fa0: 1c00 001c 0000 1c00 0000 a60f 0000 5041  ..............PA
 00000fb0: 5231                                     R1
```

### Comparing `hipscat-0.3.3/tests/data/small_sky_order1/_metadata` & `hipscat-0.3.4/tests/data/small_sky_order1/_metadata`

 * *Files 1% similar despite different names*

```diff
@@ -357,17 +357,17 @@
 00001640: 5f69 6e64 6578 222c 2022 7061 6e64 6173  _index", "pandas
 00001650: 5f74 7970 6522 3a20 2275 696e 7436 3422  _type": "uint64"
 00001660: 2c20 226e 756d 7079 5f74 7970 6522 3a20  , "numpy_type": 
 00001670: 2275 696e 7436 3422 2c20 226d 6574 6164  "uint64", "metad
 00001680: 6174 6122 3a20 6e75 6c6c 7d5d 2c20 2263  ata": null}], "c
 00001690: 7265 6174 6f72 223a 207b 226c 6962 7261  reator": {"libra
 000016a0: 7279 223a 2022 7079 6172 726f 7722 2c20  ry": "pyarrow", 
-000016b0: 2276 6572 7369 6f6e 223a 2022 3134 2e30  "version": "14.0
-000016c0: 2e31 227d 2c20 2270 616e 6461 735f 7665  .1"}, "pandas_ve
-000016d0: 7273 696f 6e22 3a20 2232 2e30 2e33 227d  rsion": "2.0.3"}
+000016b0: 2276 6572 7369 6f6e 223a 2022 3136 2e30  "version": "16.0
+000016c0: 2e30 227d 2c20 2270 616e 6461 735f 7665  .0"}, "pandas_ve
+000016d0: 7273 696f 6e22 3a20 2232 2e32 2e32 227d  rsion": "2.2.2"}
 000016e0: 0018 0c41 5252 4f57 3a73 6368 656d 6118  ...ARROW:schema.
 000016f0: ac13 2f2f 2f2f 2f7a 6748 4141 4151 4141  ../////zgHAAAQAA
 00001700: 4141 4141 414b 4141 3441 4267 4146 4141  AAAAAKAA4ABgAFAA
 00001710: 6741 4367 4141 4141 4142 4241 4151 4141  gACgAAAAABBAAQAA
 00001720: 4141 4141 414b 4141 7741 4141 4145 4141  AAAAAKAAwAAAAEAA
 00001730: 6741 4367 4141 4143 5146 4141 4145 4141  gACgAAACQFAAAEAA
 00001740: 4141 4151 4141 4141 7741 4141 4149 4141  AAAQAAAAwAAAAIAA
@@ -472,17 +472,17 @@
 00001d70: 6c66 6448 6c77 5a53 4936 4943 4a31 6157  lfdHlwZSI6ICJ1aW
 00001d80: 3530 4e6a 5169 4c43 4169 6257 5630 5957  50NjQiLCAibWV0YW
 00001d90: 5268 6447 4569 4f69 4275 6457 7873 6656  RhdGEiOiBudWxsfV
 00001da0: 3073 4943 4a6a 636d 5668 6447 3979 496a  0sICJjcmVhdG9yIj
 00001db0: 6f67 6579 4a73 6157 4a79 5958 4a35 496a  ogeyJsaWJyYXJ5Ij
 00001dc0: 6f67 496e 4235 5958 4a79 6233 6369 4c43  ogInB5YXJyb3ciLC
 00001dd0: 4169 646d 5679 6332 6c76 6269 4936 4943  AidmVyc2lvbiI6IC
-00001de0: 4978 4e43 3477 4c6a 4569 6653 7767 496e  IxNC4wLjEifSwgIn
+00001de0: 4978 4e69 3477 4c6a 4169 6653 7767 496e  IxNi4wLjAifSwgIn
 00001df0: 4268 626d 5268 6331 3932 5a58 4a7a 6157  BhbmRhc192ZXJzaW
-00001e00: 3975 496a 6f67 496a 4975 4d43 347a 496e  9uIjogIjIuMC4zIn
+00001e00: 3975 496a 6f67 496a 4975 4d69 3479 496e  9uIjogIjIuMi4yIn
 00001e10: 3041 4351 4141 414c 4142 4141 4273 4151  0ACQAAALABAABsAQ
 00001e20: 4141 5141 4541 4141 6742 4141 4451 4141  AAQAEAAAgBAADQAA
 00001e30: 4141 6d41 4141 4147 7741 4141 4138 4141  AAmAAAAGwAAAA8AA
 00001e40: 4141 4241 4141 4149 542b 2f2f 3841 4141  AABAAAAIT+//8AAA
 00001e50: 4543 4541 4141 4143 4141 4141 4145 4141  ECEAAAACAAAAAEAA
 00001e60: 4141 4141 4141 4141 3441 4141 4266 6147  AAAAAAAA4AAABfaG
 00001e70: 6c77 6332 4e68 6446 3970 626d 526c 6541  lwc2NhdF9pbmRleA
@@ -517,11 +517,11 @@
 00002040: 4941 4541 4155 4141 6741 4267 4148 4141  IAEAAUAAgABgAHAA
 00002050: 7741 4141 4151 4142 4141 4141 4141 4141  wAAAAQABAAAAAAAA
 00002060: 4543 4541 4141 4142 7741 4141 4145 4141  ECEAAAABwAAAAEAA
 00002070: 4141 4141 4141 4141 4941 4141 4270 5a41  AAAAAAAAIAAABpZA
 00002080: 4141 4341 414d 4141 6741 4277 4149 4141  AACAAMAAgABwAIAA
 00002090: 4141 4141 4141 4155 4141 4141 413d 0018  AAAAAAAUAAAAA=..
 000020a0: 2070 6172 7175 6574 2d63 7070 2d61 7272   parquet-cpp-arr
-000020b0: 6f77 2076 6572 7369 6f6e 2031 342e 302e  ow version 14.0.
-000020c0: 3119 9c1c 0000 1c00 001c 0000 1c00 001c  1...............
+000020b0: 6f77 2076 6572 7369 6f6e 2031 362e 302e  ow version 16.0.
+000020c0: 3019 9c1c 0000 1c00 001c 0000 1c00 001c  0...............
 000020d0: 0000 1c00 001c 0000 1c00 001c 0000 00db  ................
 000020e0: 2000 0050 4152 31                         ..PAR1
```

### Comparing `hipscat-0.3.3/tests/data/small_sky_order1/point_map.fits` & `hipscat-0.3.4/tests/data/small_sky_order1/point_map.fits`

 * *Files 2% similar despite different names*

```diff
@@ -229,16 +229,16 @@
 00000e40: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00000e50: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00000e60: 5049 5854 5950 4520 3d20 2748 4541 4c50  PIXTYPE = 'HEALP
 00000e70: 4958 2027 2020 2020 2020 2020 2020 202f  IX '           /
 00000e80: 2048 4541 4c50 4958 2070 6978 656c 6973   HEALPIX pixelis
 00000e90: 6174 696f 6e20 2020 2020 2020 2020 2020  ation           
 00000ea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000eb0: 4f52 4445 5249 4e47 3d20 2752 494e 4720  ORDERING= 'RING 
-00000ec0: 2020 2027 2020 2020 2020 2020 2020 202f     '           /
+00000eb0: 4f52 4445 5249 4e47 3d20 274e 4553 5445  ORDERING= 'NESTE
+00000ec0: 4420 2027 2020 2020 2020 2020 2020 202f  D  '           /
 00000ed0: 2050 6978 656c 206f 7264 6572 696e 6720   Pixel ordering 
 00000ee0: 7363 6865 6d65 2c20 6569 7468 6572 2052  scheme, either R
 00000ef0: 494e 4720 6f72 204e 4553 5445 4420 2020  ING or NESTED   
 00000f00: 4558 544e 414d 4520 3d20 2778 7465 6e73  EXTNAME = 'xtens
 00000f10: 696f 6e27 2020 2020 2020 2020 2020 202f  ion'           /
 00000f20: 206e 616d 6520 6f66 2074 6869 7320 6269   name of this bi
 00000f30: 6e61 7279 2074 6162 6c65 2065 7874 656e  nary table exten
```

### Comparing `hipscat-0.3.3/tests/data/small_sky_order1/provenance_info.json` & `hipscat-0.3.4/tests/data/small_sky/provenance_info.json`

 * *Files 12% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8212639079408627%*

 * *Differences: {"'catalog_name'": "'small_sky'",*

 * * "'generation_date'": "'2024.05.29'",*

 * * "'tool_args'": "{'version': '0.3.3.dev10+gd573bcd', 'runtime_args': {'catalog_name': 'small_sky', "*

 * *                "'output_path': '.', 'output_artifact_name': 'small_sky', 'tmp_dir': "*

 * *                "'/tmp/tmpgasth6x_', 'catalog_path': './small_sky', 'tmp_path': "*

 * *                "'/tmp/tmpgasth6x_/small_sky/intermediate', 'input_path': "*

 * *                "'../../../hipscat-import/tests/hipscat_import/data/small_sky', 'input_paths': […]*

```diff
@@ -1,52 +1,52 @@
 {
-    "catalog_name": "small_sky_order1",
+    "catalog_name": "small_sky",
     "catalog_type": "object",
     "dec_column": "dec",
     "epoch": "J2000",
-    "generation_date": "2024.01.09",
+    "generation_date": "2024.05.29",
     "ra_column": "ra",
     "tool_args": {
         "runtime_args": {
-            "catalog_name": "small_sky_order1",
-            "catalog_path": "tests/data/small_sky_order1",
+            "catalog_name": "small_sky",
+            "catalog_path": "./small_sky",
             "catalog_type": "object",
-            "constant_healpix_order": 1,
+            "constant_healpix_order": -1,
             "dask_n_workers": 1,
             "dask_threads_per_worker": 1,
             "dask_tmp": "",
             "debug_stats_only": false,
             "dec_column": "dec",
             "epoch": "J2000",
             "file_reader_info": {
                 "chunksize": 500000,
                 "column_names": null,
                 "header": "infer",
                 "input_reader_type": "CsvReader",
+                "kwargs": {},
+                "parquet_kwargs": null,
                 "schema_file": null,
-                "separator": ",",
-                "type_map": {}
+                "type_map": null
             },
             "highest_healpix_order": 7,
             "input_file_list": [],
-            "input_format": "csv",
-            "input_path": "/home/delucchi/git/hipscat-import/tests/hipscat_import/data/small_sky",
+            "input_path": "../../../hipscat-import/tests/hipscat_import/data/small_sky",
             "input_paths": [
-                "file:///home/delucchi/git/hipscat-import/tests/hipscat_import/data/small_sky/catalog.csv"
+                "file:///home/delucchi/git/fits/tests/data/../../../hipscat-import/tests/hipscat_import/data/small_sky/catalog.csv"
             ],
-            "mapping_healpix_order": 1,
-            "output_artifact_name": "small_sky_order1",
-            "output_path": "tests/data",
-            "overwrite": true,
+            "lowest_healpix_order": 0,
+            "mapping_healpix_order": 7,
+            "output_artifact_name": "small_sky",
+            "output_path": ".",
             "pixel_threshold": 1000000,
             "ra_column": "ra",
             "sort_columns": null,
-            "tmp_dir": "",
-            "tmp_path": "tests/data/small_sky_order1/intermediate",
+            "tmp_dir": "/tmp/tmpgasth6x_",
+            "tmp_path": "/tmp/tmpgasth6x_/small_sky/intermediate",
             "use_hipscat_index": false
         },
         "tool_name": "hipscat_import",
-        "version": "0.2.1"
+        "version": "0.3.3.dev10+gd573bcd"
     },
     "total_rows": 131,
-    "version": "0.2.1"
+    "version": "0.3.4.dev17+g922a4b7.d20240529"
 }
```

### Comparing `hipscat-0.3.3/tests/data/small_sky_order1_id_index/_common_metadata` & `hipscat-0.3.4/tests/data/small_sky_order1_id_index/_common_metadata`

 * *Files 2% similar despite different names*

```diff
@@ -41,17 +41,17 @@
 00000280: 222c 2022 7061 6e64 6173 5f74 7970 6522  ", "pandas_type"
 00000290: 3a20 2269 6e74 3634 222c 2022 6e75 6d70  : "int64", "nump
 000002a0: 795f 7479 7065 223a 2022 696e 7436 3422  y_type": "int64"
 000002b0: 2c20 226d 6574 6164 6174 6122 3a20 6e75  , "metadata": nu
 000002c0: 6c6c 7d5d 2c20 2263 7265 6174 6f72 223a  ll}], "creator":
 000002d0: 207b 226c 6962 7261 7279 223a 2022 7079   {"library": "py
 000002e0: 6172 726f 7722 2c20 2276 6572 7369 6f6e  arrow", "version
-000002f0: 223a 2022 3134 2e30 2e31 227d 2c20 2270  ": "14.0.1"}, "p
+000002f0: 223a 2022 3136 2e30 2e30 227d 2c20 2270  ": "16.0.0"}, "p
 00000300: 616e 6461 735f 7665 7273 696f 6e22 3a20  andas_version": 
-00000310: 2232 2e30 2e33 227d 0018 0c41 5252 4f57  "2.0.3"}...ARROW
+00000310: 2232 2e32 2e32 227d 0018 0c41 5252 4f57  "2.2.2"}...ARROW
 00000320: 3a73 6368 656d 6118 cc0a 2f2f 2f2f 2f2f  :schema...//////
 00000330: 4144 4141 4151 4141 4141 4141 414b 4141  ADAAAQAAAAAAAKAA
 00000340: 3441 4267 4146 4141 6741 4367 4141 4141  4ABgAFAAgACgAAAA
 00000350: 4142 4241 4151 4141 4141 4141 414b 4141  ABBAAQAAAAAAAKAA
 00000360: 7741 4141 4145 4141 6741 4367 4141 414f  wAAAAEAAgACgAAAO
 00000370: 5143 4141 4145 4141 4141 4151 4141 4141  QCAAAEAAAAAQAAAA
 00000380: 7741 4141 4149 4141 7741 4241 4149 4141  wAAAAIAAwABAAIAA
@@ -107,18 +107,18 @@
 000006a0: 3531 6258 4235 5833 5235 6347 5569 4f69  51bXB5X3R5cGUiOi
 000006b0: 4169 6157 3530 4e6a 5169 4c43 4169 6257  AiaW50NjQiLCAibW
 000006c0: 5630 5957 5268 6447 4569 4f69 4275 6457  V0YWRhdGEiOiBudW
 000006d0: 7873 6656 3073 4943 4a6a 636d 5668 6447  xsfV0sICJjcmVhdG
 000006e0: 3979 496a 6f67 6579 4a73 6157 4a79 5958  9yIjogeyJsaWJyYX
 000006f0: 4a35 496a 6f67 496e 4235 5958 4a79 6233  J5IjogInB5YXJyb3
 00000700: 6369 4c43 4169 646d 5679 6332 6c76 6269  ciLCAidmVyc2lvbi
-00000710: 4936 4943 4978 4e43 3477 4c6a 4569 6653  I6ICIxNC4wLjEifS
+00000710: 4936 4943 4978 4e69 3477 4c6a 4169 6653  I6ICIxNi4wLjAifS
 00000720: 7767 496e 4268 626d 5268 6331 3932 5a58  wgInBhbmRhc192ZX
-00000730: 4a7a 6157 3975 496a 6f67 496a 4975 4d43  JzaW9uIjogIjIuMC
-00000740: 347a 496e 3041 4141 4141 4241 4141 414b  4zIn0AAAAABAAAAK
+00000730: 4a7a 6157 3975 496a 6f67 496a 4975 4d69  JzaW9uIjogIjIuMi
+00000740: 3479 496e 3041 4141 4141 4241 4141 414b  4yIn0AAAAABAAAAK
 00000750: 6741 4141 4273 4141 4141 5041 4141 4141  gAAABsAAAAPAAAAA
 00000760: 5141 4141 4234 2f2f 2f2f 4141 4142 4168  QAAAB4////AAABAh
 00000770: 4141 4141 4163 4141 4141 4241 4141 4141  AAAAAcAAAABAAAAA
 00000780: 4141 4141 4143 4141 4141 6157 5141 4141  AAAAACAAAAaWQAAA
 00000790: 6741 4441 4149 4141 6341 4341 4141 4141  gADAAIAAcACAAAAA
 000007a0: 4141 4141 4641 4141 4141 7250 2f2f 2f77  AAAAFAAAAArP///w
 000007b0: 4141 4151 4951 4141 4141 4741 4141 4141  AAAQIQAAAAGAAAAA
@@ -131,9 +131,9 @@
 00000820: 6741 4267 4148 4141 7741 4141 4151 4142  gABgAHAAwAAAAQAB
 00000830: 4141 4141 4141 4141 4543 4541 4141 4143  AAAAAAAAECEAAAAC
 00000840: 4141 4141 4145 4141 4141 4141 4141 4141  AAAAAEAAAAAAAAAA
 00000850: 5941 4141 424f 6233 4a6b 5a58 4941 4141  YAAABOb3JkZXIAAA
 00000860: 4141 4267 4149 4141 5141 4267 4141 4141  AABgAIAAQABgAAAA
 00000870: 6741 4141 413d 0018 2070 6172 7175 6574  gAAAA=.. parquet
 00000880: 2d63 7070 2d61 7272 6f77 2076 6572 7369  -cpp-arrow versi
-00000890: 6f6e 2031 342e 302e 3119 4c1c 0000 1c00  on 14.0.1.L.....
+00000890: 6f6e 2031 362e 302e 3019 4c1c 0000 1c00  on 16.0.0.L.....
 000008a0: 001c 0000 1c00 0000 a408 0000 5041 5231  ............PAR1
```

### Comparing `hipscat-0.3.3/tests/data/small_sky_order1_id_index/_metadata` & `hipscat-0.3.4/tests/data/small_sky_order1_id_index/_metadata`

 * *Files 2% similar despite different names*

```diff
@@ -67,17 +67,17 @@
 00000420: 616d 6522 3a20 2269 6422 2c20 2270 616e  ame": "id", "pan
 00000430: 6461 735f 7479 7065 223a 2022 696e 7436  das_type": "int6
 00000440: 3422 2c20 226e 756d 7079 5f74 7970 6522  4", "numpy_type"
 00000450: 3a20 2269 6e74 3634 222c 2022 6d65 7461  : "int64", "meta
 00000460: 6461 7461 223a 206e 756c 6c7d 5d2c 2022  data": null}], "
 00000470: 6372 6561 746f 7222 3a20 7b22 6c69 6272  creator": {"libr
 00000480: 6172 7922 3a20 2270 7961 7272 6f77 222c  ary": "pyarrow",
-00000490: 2022 7665 7273 696f 6e22 3a20 2231 342e   "version": "14.
-000004a0: 302e 3122 7d2c 2022 7061 6e64 6173 5f76  0.1"}, "pandas_v
-000004b0: 6572 7369 6f6e 223a 2022 322e 302e 3322  ersion": "2.0.3"
+00000490: 2022 7665 7273 696f 6e22 3a20 2231 362e   "version": "16.
+000004a0: 302e 3022 7d2c 2022 7061 6e64 6173 5f76  0.0"}, "pandas_v
+000004b0: 6572 7369 6f6e 223a 2022 322e 322e 3222  ersion": "2.2.2"
 000004c0: 7d00 180c 4152 524f 573a 7363 6865 6d61  }...ARROW:schema
 000004d0: 18cc 0a2f 2f2f 2f2f 2f41 4441 4141 5141  ...//////ADAAAQA
 000004e0: 4141 4141 4141 4b41 4134 4142 6741 4641  AAAAAAKAA4ABgAFA
 000004f0: 4167 4143 6741 4141 4141 4242 4141 5141  AgACgAAAAABBAAQA
 00000500: 4141 4141 4141 4b41 4177 4141 4141 4541  AAAAAAKAAwAAAAEA
 00000510: 4167 4143 6741 4141 4f51 4341 4141 4541  AgACgAAAOQCAAAEA
 00000520: 4141 4141 5141 4141 4177 4141 4141 4941  AAAAQAAAAwAAAAIA
@@ -134,17 +134,17 @@
 00000850: 3352 3563 4755 694f 6941 6961 5735 304e  3R5cGUiOiAiaW50N
 00000860: 6a51 694c 4341 6962 5756 3059 5752 6864  jQiLCAibWV0YWRhd
 00000870: 4745 694f 6942 7564 5778 7366 5630 7349  GEiOiBudWxsfV0sI
 00000880: 434a 6a63 6d56 6864 4739 7949 6a6f 6765  CJjcmVhdG9yIjoge
 00000890: 794a 7361 574a 7959 584a 3549 6a6f 6749  yJsaWJyYXJ5IjogI
 000008a0: 6e42 3559 584a 7962 3363 694c 4341 6964  nB5YXJyb3ciLCAid
 000008b0: 6d56 7963 326c 7662 6949 3649 4349 784e  mVyc2lvbiI6ICIxN
-000008c0: 4334 774c 6a45 6966 5377 6749 6e42 6862  C4wLjEifSwgInBhb
+000008c0: 6934 774c 6a41 6966 5377 6749 6e42 6862  i4wLjAifSwgInBhb
 000008d0: 6d52 6863 3139 325a 584a 7a61 5739 7549  mRhc192ZXJzaW9uI
-000008e0: 6a6f 6749 6a49 754d 4334 7a49 6e30 4141  jogIjIuMC4zIn0AA
+000008e0: 6a6f 6749 6a49 754d 6934 7949 6e30 4141  jogIjIuMi4yIn0AA
 000008f0: 4141 4142 4141 4141 4b67 4141 4142 7341  AAABAAAAKgAAABsA
 00000900: 4141 4150 4141 4141 4151 4141 4142 342f  AAAPAAAAAQAAAB4/
 00000910: 2f2f 2f41 4141 4241 6841 4141 4141 6341  ///AAABAhAAAAAcA
 00000920: 4141 4142 4141 4141 4141 4141 4141 4341  AAABAAAAAAAAAACA
 00000930: 4141 4161 5751 4141 4167 4144 4141 4941  AAAaWQAAAgADAAIA
 00000940: 4163 4143 4141 4141 4141 4141 4146 4141  AcACAAAAAAAAAFAA
 00000950: 4141 4172 502f 2f2f 7741 4141 5149 5141  AAArP///wAAAQIQA
@@ -157,10 +157,10 @@
 000009c0: 4141 4145 4141 5541 4167 4142 6741 4841  AAAEAAUAAgABgAHA
 000009d0: 4177 4141 4141 5141 4241 4141 4141 4141  AwAAAAQABAAAAAAA
 000009e0: 4145 4345 4141 4141 4341 4141 4141 4541  AECEAAAACAAAAAEA
 000009f0: 4141 4141 4141 4141 4159 4141 4142 4f62  AAAAAAAAAYAAABOb
 00000a00: 334a 6b5a 5849 4141 4141 4142 6741 4941  3JkZXIAAAAABgAIA
 00000a10: 4151 4142 6741 4141 4167 4141 4141 3d00  AQABgAAAAgAAAA=.
 00000a20: 1820 7061 7271 7565 742d 6370 702d 6172  . parquet-cpp-ar
-00000a30: 726f 7720 7665 7273 696f 6e20 3134 2e30  row version 14.0
-00000a40: 2e31 194c 1c00 001c 0000 1c00 001c 0000  .1.L............
+00000a30: 726f 7720 7665 7273 696f 6e20 3136 2e30  row version 16.0
+00000a40: 2e30 194c 1c00 001c 0000 1c00 001c 0000  .0.L............
 00000a50: 004d 0a00 0050 4152 31                   .M...PAR1
```

### Comparing `hipscat-0.3.3/tests/data/small_sky_order1_id_index/index/part.0.parquet` & `hipscat-0.3.4/tests/data/small_sky_order1_id_index/index/part.0.parquet`

 * *Files 2% similar despite different names*

```diff
@@ -144,17 +144,17 @@
 000008f0: 616e 6461 735f 7479 7065 223a 2022 696e  andas_type": "in
 00000900: 7436 3422 2c20 226e 756d 7079 5f74 7970  t64", "numpy_typ
 00000910: 6522 3a20 2269 6e74 3634 222c 2022 6d65  e": "int64", "me
 00000920: 7461 6461 7461 223a 206e 756c 6c7d 5d2c  tadata": null}],
 00000930: 2022 6372 6561 746f 7222 3a20 7b22 6c69   "creator": {"li
 00000940: 6272 6172 7922 3a20 2270 7961 7272 6f77  brary": "pyarrow
 00000950: 222c 2022 7665 7273 696f 6e22 3a20 2231  ", "version": "1
-00000960: 342e 302e 3122 7d2c 2022 7061 6e64 6173  4.0.1"}, "pandas
-00000970: 5f76 6572 7369 6f6e 223a 2022 322e 302e  _version": "2.0.
-00000980: 3322 7d00 180c 4152 524f 573a 7363 6865  3"}...ARROW:sche
+00000960: 362e 302e 3022 7d2c 2022 7061 6e64 6173  6.0.0"}, "pandas
+00000970: 5f76 6572 7369 6f6e 223a 2022 322e 322e  _version": "2.2.
+00000980: 3222 7d00 180c 4152 524f 573a 7363 6865  2"}...ARROW:sche
 00000990: 6d61 18cc 0a2f 2f2f 2f2f 2f41 4441 4141  ma...//////ADAAA
 000009a0: 5141 4141 4141 4141 4b41 4134 4142 6741  QAAAAAAAKAA4ABgA
 000009b0: 4641 4167 4143 6741 4141 4141 4242 4141  FAAgACgAAAAABBAA
 000009c0: 5141 4141 4141 4141 4b41 4177 4141 4141  QAAAAAAAKAAwAAAA
 000009d0: 4541 4167 4143 6741 4141 4f51 4341 4141  EAAgACgAAAOQCAAA
 000009e0: 4541 4141 4141 5141 4141 4177 4141 4141  EAAAAAQAAAAwAAAA
 000009f0: 4941 4177 4142 4141 4941 4167 4141 4141  IAAwABAAIAAgAAAA
@@ -210,17 +210,17 @@
 00000d10: 3558 3352 3563 4755 694f 6941 6961 5735  5X3R5cGUiOiAiaW5
 00000d20: 304e 6a51 694c 4341 6962 5756 3059 5752  0NjQiLCAibWV0YWR
 00000d30: 6864 4745 694f 6942 7564 5778 7366 5630  hdGEiOiBudWxsfV0
 00000d40: 7349 434a 6a63 6d56 6864 4739 7949 6a6f  sICJjcmVhdG9yIjo
 00000d50: 6765 794a 7361 574a 7959 584a 3549 6a6f  geyJsaWJyYXJ5Ijo
 00000d60: 6749 6e42 3559 584a 7962 3363 694c 4341  gInB5YXJyb3ciLCA
 00000d70: 6964 6d56 7963 326c 7662 6949 3649 4349  idmVyc2lvbiI6ICI
-00000d80: 784e 4334 774c 6a45 6966 5377 6749 6e42  xNC4wLjEifSwgInB
+00000d80: 784e 6934 774c 6a41 6966 5377 6749 6e42  xNi4wLjAifSwgInB
 00000d90: 6862 6d52 6863 3139 325a 584a 7a61 5739  hbmRhc192ZXJzaW9
-00000da0: 7549 6a6f 6749 6a49 754d 4334 7a49 6e30  uIjogIjIuMC4zIn0
+00000da0: 7549 6a6f 6749 6a49 754d 6934 7949 6e30  uIjogIjIuMi4yIn0
 00000db0: 4141 4141 4142 4141 4141 4b67 4141 4142  AAAAABAAAAKgAAAB
 00000dc0: 7341 4141 4150 4141 4141 4151 4141 4142  sAAAAPAAAAAQAAAB
 00000dd0: 342f 2f2f 2f41 4141 4241 6841 4141 4141  4////AAABAhAAAAA
 00000de0: 6341 4141 4142 4141 4141 4141 4141 4141  cAAAABAAAAAAAAAA
 00000df0: 4341 4141 4161 5751 4141 4167 4144 4141  CAAAAaWQAAAgADAA
 00000e00: 4941 4163 4143 4141 4141 4141 4141 4146  IAAcACAAAAAAAAAF
 00000e10: 4141 4141 4172 502f 2f2f 7741 4141 5149  AAAAArP///wAAAQI
@@ -233,10 +233,10 @@
 00000e80: 4141 4141 4145 4141 5541 4167 4142 6741  AAAAAEAAUAAgABgA
 00000e90: 4841 4177 4141 4141 5141 4241 4141 4141  HAAwAAAAQABAAAAA
 00000ea0: 4141 4145 4345 4141 4141 4341 4141 4141  AAAECEAAAACAAAAA
 00000eb0: 4541 4141 4141 4141 4141 4159 4141 4142  EAAAAAAAAAAYAAAB
 00000ec0: 4f62 334a 6b5a 5849 4141 4141 4142 6741  Ob3JkZXIAAAAABgA
 00000ed0: 4941 4151 4142 6741 4141 4167 4141 4141  IAAQABgAAAAgAAAA
 00000ee0: 3d00 1820 7061 7271 7565 742d 6370 702d  =.. parquet-cpp-
-00000ef0: 6172 726f 7720 7665 7273 696f 6e20 3134  arrow version 14
-00000f00: 2e30 2e31 194c 1c00 001c 0000 1c00 001c  .0.1.L..........
+00000ef0: 6172 726f 7720 7665 7273 696f 6e20 3136  arrow version 16
+00000f00: 2e30 2e30 194c 1c00 001c 0000 1c00 001c  .0.0.L..........
 00000f10: 0000 00f1 0900 0050 4152 31              .......PAR1
```

### Comparing `hipscat-0.3.3/tests/data/small_sky_order1_id_index/provenance_info.json` & `hipscat-0.3.4/tests/data/small_sky_source_object_index/provenance_info.json`

 * *Files 22% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6540123456790123%*

 * *Differences: {"'catalog_name'": "'small_sky_source_object_index'",*

 * * "'generation_date'": "'2024.05.29'",*

 * * "'indexing_column'": "'object_id'",*

 * * "'primary_catalog'": "'small_sky_source'",*

 * * "'tool_args'": "{'version': '0.3.3.dev10+gd573bcd', 'runtime_args': {'catalog_name': "*

 * *                "'small_sky_source_object_index', 'output_path': '.', 'output_artifact_name': "*

 * *                "'small_sky_source_object_index', 'tmp_dir': '/tmp/tmpgasth6x_', 'catalog_path': "*

 * *                "'./small_sky_source_object_index', 'tmp […]*

```diff
@@ -1,31 +1,30 @@
 {
-    "catalog_name": "small_sky_order1_id_index",
+    "catalog_name": "small_sky_source_object_index",
     "catalog_type": "index",
     "extra_columns": [],
-    "generation_date": "2024.01.09",
-    "indexing_column": "id",
-    "primary_catalog": "/home/delucchi/git/hipscat/tests/data/small_sky_order1",
+    "generation_date": "2024.05.29",
+    "indexing_column": "object_id",
+    "primary_catalog": "small_sky_source",
     "tool_args": {
         "runtime_args": {
-            "catalog_name": "small_sky_order1_id_index",
-            "catalog_path": "/home/delucchi/git/hipscat/tests/data/small_sky_order1_id_index",
+            "catalog_name": "small_sky_source_object_index",
+            "catalog_path": "./small_sky_source_object_index",
             "dask_n_workers": 1,
             "dask_threads_per_worker": 1,
             "dask_tmp": "",
             "extra_columns": [],
-            "include_hipscat_index": "False",
+            "include_hipscat_index": false,
             "include_order_pixel": true,
-            "indexing_column": "id",
-            "input_catalog_path": "/home/delucchi/git/hipscat/tests/data/small_sky_order1",
-            "output_artifact_name": "small_sky_order1_id_index",
-            "output_path": "/home/delucchi/git/hipscat/tests/data/",
-            "overwrite": true,
-            "tmp_dir": "",
-            "tmp_path": "/home/delucchi/git/hipscat/tests/data/small_sky_order1_id_index/intermediate"
+            "indexing_column": "object_id",
+            "input_catalog_path": "small_sky_source",
+            "output_artifact_name": "small_sky_source_object_index",
+            "output_path": ".",
+            "tmp_dir": "/tmp/tmpgasth6x_",
+            "tmp_path": "/tmp/tmpgasth6x_/small_sky_source_object_index/intermediate"
         },
         "tool_name": "hipscat_import",
-        "version": "0.2.1"
+        "version": "0.3.3.dev10+gd573bcd"
     },
-    "total_rows": 131,
-    "version": "0.2.1"
+    "total_rows": 148,
+    "version": "0.3.4.dev17+g922a4b7.d20240529"
 }
```

### Comparing `hipscat-0.3.3/tests/data/small_sky_order1_margin/Norder=0/Dir=0/Npix=4.parquet` & `hipscat-0.3.4/tests/data/small_sky_order1_margin/Norder=0/Dir=0/Npix=4.parquet`

 * *Files 2% similar despite different names*

```diff
@@ -302,17 +302,17 @@
 000012d0: 6461 735f 7479 7065 223a 2022 7569 6e74  das_type": "uint
 000012e0: 3634 222c 2022 6e75 6d70 795f 7479 7065  64", "numpy_type
 000012f0: 223a 2022 7569 6e74 3634 222c 2022 6d65  ": "uint64", "me
 00001300: 7461 6461 7461 223a 206e 756c 6c7d 5d2c  tadata": null}],
 00001310: 2022 6372 6561 746f 7222 3a20 7b22 6c69   "creator": {"li
 00001320: 6272 6172 7922 3a20 2270 7961 7272 6f77  brary": "pyarrow
 00001330: 222c 2022 7665 7273 696f 6e22 3a20 2231  ", "version": "1
-00001340: 342e 302e 3122 7d2c 2022 7061 6e64 6173  4.0.1"}, "pandas
-00001350: 5f76 6572 7369 6f6e 223a 2022 322e 302e  _version": "2.0.
-00001360: 3322 7d00 180c 4152 524f 573a 7363 6865  3"}...ARROW:sche
+00001340: 362e 302e 3022 7d2c 2022 7061 6e64 6173  6.0.0"}, "pandas
+00001350: 5f76 6572 7369 6f6e 223a 2022 322e 322e  _version": "2.2.
+00001360: 3222 7d00 180c 4152 524f 573a 7363 6865  2"}...ARROW:sche
 00001370: 6d61 18f8 182f 2f2f 2f2f 3141 4a41 4141  ma.../////1AJAAA
 00001380: 5141 4141 4141 4141 4b41 4134 4142 6741  QAAAAAAAKAA4ABgA
 00001390: 4641 4167 4143 6741 4141 4141 4242 4141  FAAgACgAAAAABBAA
 000013a0: 5141 4141 4141 4141 4b41 4177 4141 4141  QAAAAAAAKAAwAAAA
 000013b0: 4541 4167 4143 6741 4141 4a67 4741 4141  EAAgACgAAAJgGAAA
 000013c0: 4541 4141 4141 5141 4141 4177 4141 4141  EAAAAAQAAAAwAAAA
 000013d0: 4941 4177 4142 4141 4941 4167 4141 4141  IAAwABAAIAAgAAAA
@@ -447,17 +447,17 @@
 00001be0: 6664 486c 775a 5349 3649 434a 3161 5735  fdHlwZSI6ICJ1aW5
 00001bf0: 304e 6a51 694c 4341 6962 5756 3059 5752  0NjQiLCAibWV0YWR
 00001c00: 6864 4745 694f 6942 7564 5778 7366 5630  hdGEiOiBudWxsfV0
 00001c10: 7349 434a 6a63 6d56 6864 4739 7949 6a6f  sICJjcmVhdG9yIjo
 00001c20: 6765 794a 7361 574a 7959 584a 3549 6a6f  geyJsaWJyYXJ5Ijo
 00001c30: 6749 6e42 3559 584a 7962 3363 694c 4341  gInB5YXJyb3ciLCA
 00001c40: 6964 6d56 7963 326c 7662 6949 3649 4349  idmVyc2lvbiI6ICI
-00001c50: 784e 4334 774c 6a45 6966 5377 6749 6e42  xNC4wLjEifSwgInB
+00001c50: 784e 6934 774c 6a41 6966 5377 6749 6e42  xNi4wLjAifSwgInB
 00001c60: 6862 6d52 6863 3139 325a 584a 7a61 5739  hbmRhc192ZXJzaW9
-00001c70: 7549 6a6f 6749 6a49 754d 4334 7a49 6e30  uIjogIjIuMC4zIn0
+00001c70: 7549 6a6f 6749 6a49 754d 6934 7949 6e30  uIjogIjIuMi4yIn0
 00001c80: 4141 4141 4144 4141 4141 4641 4341 4141  AAAAADAAAAFACAAA
 00001c90: 4d41 6741 4134 4145 4141 4b67 4241 4142  MAgAA4AEAAKgBAAB
 00001ca0: 7741 5141 414f 4145 4141 4177 4241 4144  wAQAAOAEAAAwBAAD
 00001cb0: 6341 4141 4170 4141 4141 4777 4141 4141  cAAAApAAAAGwAAAA
 00001cc0: 3441 4141 4142 4141 4141 5044 392f 2f38  4AAAABAAAAPD9//8
 00001cd0: 4141 4145 4345 4141 4141 4277 4141 4141  AAAECEAAAABwAAAA
 00001ce0: 4541 4141 4141 4141 4141 4173 4141 4142  EAAAAAAAAAAsAAAB
@@ -506,11 +506,11 @@
 00001f90: 4941 4159 4142 7741 4d41 4141 4145 4141  IAAYABwAMAAAAEAA
 00001fa0: 5141 4141 4141 4141 4241 6841 4141 4141  QAAAAAAABAhAAAAA
 00001fb0: 6341 4141 4142 4141 4141 4141 4141 4141  cAAAABAAAAAAAAAA
 00001fc0: 4341 4141 4161 5751 4141 4167 4144 4141  CAAAAaWQAAAgADAA
 00001fd0: 4941 4163 4143 4141 4141 4141 4141 4146  IAAcACAAAAAAAAAF
 00001fe0: 4141 4141 4141 4141 4141 413d 3d00 1820  AAAAAAAAAAA==.. 
 00001ff0: 7061 7271 7565 742d 6370 702d 6172 726f  parquet-cpp-arro
-00002000: 7720 7665 7273 696f 6e20 3134 2e30 2e31  w version 14.0.1
+00002000: 7720 7665 7273 696f 6e20 3136 2e30 2e30  w version 16.0.0
 00002010: 19cc 1c00 001c 0000 1c00 001c 0000 1c00  ................
 00002020: 001c 0000 1c00 001c 0000 1c00 001c 0000  ................
 00002030: 1c00 001c 0000 0052 1800 0050 4152 31    .......R...PAR1
```

### Comparing `hipscat-0.3.3/tests/data/small_sky_order1_margin/Norder=1/Dir=0/Npix=44.parquet` & `hipscat-0.3.4/tests/data/small_sky_order1_margin/Norder=1/Dir=0/Npix=44.parquet`

 * *Files 1% similar despite different names*

```diff
@@ -313,17 +313,17 @@
 00001380: 7061 6e64 6173 5f74 7970 6522 3a20 2275  pandas_type": "u
 00001390: 696e 7436 3422 2c20 226e 756d 7079 5f74  int64", "numpy_t
 000013a0: 7970 6522 3a20 2275 696e 7436 3422 2c20  ype": "uint64", 
 000013b0: 226d 6574 6164 6174 6122 3a20 6e75 6c6c  "metadata": null
 000013c0: 7d5d 2c20 2263 7265 6174 6f72 223a 207b  }], "creator": {
 000013d0: 226c 6962 7261 7279 223a 2022 7079 6172  "library": "pyar
 000013e0: 726f 7722 2c20 2276 6572 7369 6f6e 223a  row", "version":
-000013f0: 2022 3134 2e30 2e31 227d 2c20 2270 616e   "14.0.1"}, "pan
+000013f0: 2022 3136 2e30 2e30 227d 2c20 2270 616e   "16.0.0"}, "pan
 00001400: 6461 735f 7665 7273 696f 6e22 3a20 2232  das_version": "2
-00001410: 2e30 2e33 227d 0018 0c41 5252 4f57 3a73  .0.3"}...ARROW:s
+00001410: 2e32 2e32 227d 0018 0c41 5252 4f57 3a73  .2.2"}...ARROW:s
 00001420: 6368 656d 6118 f818 2f2f 2f2f 2f31 414a  chema.../////1AJ
 00001430: 4141 4151 4141 4141 4141 414b 4141 3441  AAAQAAAAAAAKAA4A
 00001440: 4267 4146 4141 6741 4367 4141 4141 4142  BgAFAAgACgAAAAAB
 00001450: 4241 4151 4141 4141 4141 414b 4141 7741  BAAQAAAAAAAKAAwA
 00001460: 4141 4145 4141 6741 4367 4141 414a 6747  AAAEAAgACgAAAJgG
 00001470: 4141 4145 4141 4141 4151 4141 4141 7741  AAAEAAAAAQAAAAwA
 00001480: 4141 4149 4141 7741 4241 4149 4141 6741  AAAIAAwABAAIAAgA
@@ -458,17 +458,17 @@
 00001c90: 6348 6c66 6448 6c77 5a53 4936 4943 4a31  cHlfdHlwZSI6ICJ1
 00001ca0: 6157 3530 4e6a 5169 4c43 4169 6257 5630  aW50NjQiLCAibWV0
 00001cb0: 5957 5268 6447 4569 4f69 4275 6457 7873  YWRhdGEiOiBudWxs
 00001cc0: 6656 3073 4943 4a6a 636d 5668 6447 3979  fV0sICJjcmVhdG9y
 00001cd0: 496a 6f67 6579 4a73 6157 4a79 5958 4a35  IjogeyJsaWJyYXJ5
 00001ce0: 496a 6f67 496e 4235 5958 4a79 6233 6369  IjogInB5YXJyb3ci
 00001cf0: 4c43 4169 646d 5679 6332 6c76 6269 4936  LCAidmVyc2lvbiI6
-00001d00: 4943 4978 4e43 3477 4c6a 4569 6653 7767  ICIxNC4wLjEifSwg
+00001d00: 4943 4978 4e69 3477 4c6a 4169 6653 7767  ICIxNi4wLjAifSwg
 00001d10: 496e 4268 626d 5268 6331 3932 5a58 4a7a  InBhbmRhc192ZXJz
-00001d20: 6157 3975 496a 6f67 496a 4975 4d43 347a  aW9uIjogIjIuMC4z
+00001d20: 6157 3975 496a 6f67 496a 4975 4d69 3479  aW9uIjogIjIuMi4y
 00001d30: 496e 3041 4141 4141 4441 4141 4146 4143  In0AAAAADAAAAFAC
 00001d40: 4141 414d 4167 4141 3441 4541 414b 6742  AAAMAgAA4AEAAKgB
 00001d50: 4141 4277 4151 4141 4f41 4541 4141 7742  AABwAQAAOAEAAAwB
 00001d60: 4141 4463 4141 4141 7041 4141 4147 7741  AADcAAAApAAAAGwA
 00001d70: 4141 4134 4141 4141 4241 4141 4150 4439  AAA4AAAABAAAAPD9
 00001d80: 2f2f 3841 4141 4543 4541 4141 4142 7741  //8AAAECEAAAABwA
 00001d90: 4141 4145 4141 4141 4141 4141 4141 7341  AAAEAAAAAAAAAAsA
@@ -517,12 +517,12 @@
 00002040: 4641 4149 4141 5941 4277 414d 4141 4141  FAAIAAYABwAMAAAA
 00002050: 4541 4151 4141 4141 4141 4142 4168 4141  EAAQAAAAAAABAhAA
 00002060: 4141 4163 4141 4141 4241 4141 4141 4141  AAAcAAAABAAAAAAA
 00002070: 4141 4143 4141 4141 6157 5141 4141 6741  AAACAAAAaWQAAAgA
 00002080: 4441 4149 4141 6341 4341 4141 4141 4141  DAAIAAcACAAAAAAA
 00002090: 4141 4641 4141 4141 4141 4141 4141 3d3d  AAFAAAAAAAAAAA==
 000020a0: 0018 2070 6172 7175 6574 2d63 7070 2d61  .. parquet-cpp-a
-000020b0: 7272 6f77 2076 6572 7369 6f6e 2031 342e  rrow version 14.
-000020c0: 302e 3119 cc1c 0000 1c00 001c 0000 1c00  0.1.............
+000020b0: 7272 6f77 2076 6572 7369 6f6e 2031 362e  rrow version 16.
+000020c0: 302e 3019 cc1c 0000 1c00 001c 0000 1c00  0.0.............
 000020d0: 001c 0000 1c00 001c 0000 1c00 001c 0000  ................
 000020e0: 1c00 001c 0000 1c00 0000 5318 0000 5041  ..........S...PA
 000020f0: 5231                                     R1
```

### Comparing `hipscat-0.3.3/tests/data/small_sky_order1_margin/Norder=1/Dir=0/Npix=45.parquet` & `hipscat-0.3.4/tests/data/small_sky_order1_margin/Norder=1/Dir=0/Npix=45.parquet`

 * *Files 1% similar despite different names*

```diff
@@ -315,17 +315,17 @@
 000013a0: 5f69 6e64 6578 222c 2022 7061 6e64 6173  _index", "pandas
 000013b0: 5f74 7970 6522 3a20 2275 696e 7436 3422  _type": "uint64"
 000013c0: 2c20 226e 756d 7079 5f74 7970 6522 3a20  , "numpy_type": 
 000013d0: 2275 696e 7436 3422 2c20 226d 6574 6164  "uint64", "metad
 000013e0: 6174 6122 3a20 6e75 6c6c 7d5d 2c20 2263  ata": null}], "c
 000013f0: 7265 6174 6f72 223a 207b 226c 6962 7261  reator": {"libra
 00001400: 7279 223a 2022 7079 6172 726f 7722 2c20  ry": "pyarrow", 
-00001410: 2276 6572 7369 6f6e 223a 2022 3134 2e30  "version": "14.0
-00001420: 2e31 227d 2c20 2270 616e 6461 735f 7665  .1"}, "pandas_ve
-00001430: 7273 696f 6e22 3a20 2232 2e30 2e33 227d  rsion": "2.0.3"}
+00001410: 2276 6572 7369 6f6e 223a 2022 3136 2e30  "version": "16.0
+00001420: 2e30 227d 2c20 2270 616e 6461 735f 7665  .0"}, "pandas_ve
+00001430: 7273 696f 6e22 3a20 2232 2e32 2e32 227d  rsion": "2.2.2"}
 00001440: 0018 0c41 5252 4f57 3a73 6368 656d 6118  ...ARROW:schema.
 00001450: f818 2f2f 2f2f 2f31 414a 4141 4151 4141  ../////1AJAAAQAA
 00001460: 4141 4141 414b 4141 3441 4267 4146 4141  AAAAAKAA4ABgAFAA
 00001470: 6741 4367 4141 4141 4142 4241 4151 4141  gACgAAAAABBAAQAA
 00001480: 4141 4141 414b 4141 7741 4141 4145 4141  AAAAAKAAwAAAAEAA
 00001490: 6741 4367 4141 414a 6747 4141 4145 4141  gACgAAAJgGAAAEAA
 000014a0: 4141 4151 4141 4141 7741 4141 4149 4141  AAAQAAAAwAAAAIAA
@@ -460,18 +460,18 @@
 00001cb0: 5169 4c43 4169 626e 5674 6348 6c66 6448  QiLCAibnVtcHlfdH
 00001cc0: 6c77 5a53 4936 4943 4a31 6157 3530 4e6a  lwZSI6ICJ1aW50Nj
 00001cd0: 5169 4c43 4169 6257 5630 5957 5268 6447  QiLCAibWV0YWRhdG
 00001ce0: 4569 4f69 4275 6457 7873 6656 3073 4943  EiOiBudWxsfV0sIC
 00001cf0: 4a6a 636d 5668 6447 3979 496a 6f67 6579  JjcmVhdG9yIjogey
 00001d00: 4a73 6157 4a79 5958 4a35 496a 6f67 496e  JsaWJyYXJ5IjogIn
 00001d10: 4235 5958 4a79 6233 6369 4c43 4169 646d  B5YXJyb3ciLCAidm
-00001d20: 5679 6332 6c76 6269 4936 4943 4978 4e43  Vyc2lvbiI6ICIxNC
-00001d30: 3477 4c6a 4569 6653 7767 496e 4268 626d  4wLjEifSwgInBhbm
+00001d20: 5679 6332 6c76 6269 4936 4943 4978 4e69  Vyc2lvbiI6ICIxNi
+00001d30: 3477 4c6a 4169 6653 7767 496e 4268 626d  4wLjAifSwgInBhbm
 00001d40: 5268 6331 3932 5a58 4a7a 6157 3975 496a  Rhc192ZXJzaW9uIj
-00001d50: 6f67 496a 4975 4d43 347a 496e 3041 4141  ogIjIuMC4zIn0AAA
+00001d50: 6f67 496a 4975 4d69 3479 496e 3041 4141  ogIjIuMi4yIn0AAA
 00001d60: 4141 4441 4141 4146 4143 4141 414d 4167  AADAAAAFACAAAMAg
 00001d70: 4141 3441 4541 414b 6742 4141 4277 4151  AA4AEAAKgBAABwAQ
 00001d80: 4141 4f41 4541 4141 7742 4141 4463 4141  AAOAEAAAwBAADcAA
 00001d90: 4141 7041 4141 4147 7741 4141 4134 4141  AApAAAAGwAAAA4AA
 00001da0: 4141 4241 4141 4150 4439 2f2f 3841 4141  AABAAAAPD9//8AAA
 00001db0: 4543 4541 4141 4142 7741 4141 4145 4141  ECEAAAABwAAAAEAA
 00001dc0: 4141 4141 4141 4141 7341 4141 4274 5958  AAAAAAAAsAAABtYX
@@ -520,11 +520,11 @@
 00002070: 5941 4277 414d 4141 4141 4541 4151 4141  YABwAMAAAAEAAQAA
 00002080: 4141 4141 4142 4168 4141 4141 4163 4141  AAAAABAhAAAAAcAA
 00002090: 4141 4241 4141 4141 4141 4141 4143 4141  AABAAAAAAAAAACAA
 000020a0: 4141 6157 5141 4141 6741 4441 4149 4141  AAaWQAAAgADAAIAA
 000020b0: 6341 4341 4141 4141 4141 4141 4641 4141  cACAAAAAAAAAFAAA
 000020c0: 4141 4141 4141 4141 3d3d 0018 2070 6172  AAAAAAAA==.. par
 000020d0: 7175 6574 2d63 7070 2d61 7272 6f77 2076  quet-cpp-arrow v
-000020e0: 6572 7369 6f6e 2031 342e 302e 3119 cc1c  ersion 14.0.1...
+000020e0: 6572 7369 6f6e 2031 362e 302e 3019 cc1c  ersion 16.0.0...
 000020f0: 0000 1c00 001c 0000 1c00 001c 0000 1c00  ................
 00002100: 001c 0000 1c00 001c 0000 1c00 001c 0000  ................
 00002110: 1c00 0000 5318 0000 5041 5231            ....S...PAR1
```

### Comparing `hipscat-0.3.3/tests/data/small_sky_order1_margin/Norder=1/Dir=0/Npix=46.parquet` & `hipscat-0.3.4/tests/data/small_sky_order1_margin/Norder=1/Dir=0/Npix=46.parquet`

 * *Files 1% similar despite different names*

```diff
@@ -309,17 +309,17 @@
 00001340: 6e64 6578 222c 2022 7061 6e64 6173 5f74  ndex", "pandas_t
 00001350: 7970 6522 3a20 2275 696e 7436 3422 2c20  ype": "uint64", 
 00001360: 226e 756d 7079 5f74 7970 6522 3a20 2275  "numpy_type": "u
 00001370: 696e 7436 3422 2c20 226d 6574 6164 6174  int64", "metadat
 00001380: 6122 3a20 6e75 6c6c 7d5d 2c20 2263 7265  a": null}], "cre
 00001390: 6174 6f72 223a 207b 226c 6962 7261 7279  ator": {"library
 000013a0: 223a 2022 7079 6172 726f 7722 2c20 2276  ": "pyarrow", "v
-000013b0: 6572 7369 6f6e 223a 2022 3134 2e30 2e31  ersion": "14.0.1
+000013b0: 6572 7369 6f6e 223a 2022 3136 2e30 2e30  ersion": "16.0.0
 000013c0: 227d 2c20 2270 616e 6461 735f 7665 7273  "}, "pandas_vers
-000013d0: 696f 6e22 3a20 2232 2e30 2e33 227d 0018  ion": "2.0.3"}..
+000013d0: 696f 6e22 3a20 2232 2e32 2e32 227d 0018  ion": "2.2.2"}..
 000013e0: 0c41 5252 4f57 3a73 6368 656d 6118 f818  .ARROW:schema...
 000013f0: 2f2f 2f2f 2f31 414a 4141 4151 4141 4141  /////1AJAAAQAAAA
 00001400: 4141 414b 4141 3441 4267 4146 4141 6741  AAAKAA4ABgAFAAgA
 00001410: 4367 4141 4141 4142 4241 4151 4141 4141  CgAAAAABBAAQAAAA
 00001420: 4141 414b 4141 7741 4141 4145 4141 6741  AAAKAAwAAAAEAAgA
 00001430: 4367 4141 414a 6747 4141 4145 4141 4141  CgAAAJgGAAAEAAAA
 00001440: 4151 4141 4141 7741 4141 4149 4141 7741  AQAAAAwAAAAIAAwA
@@ -454,18 +454,18 @@
 00001c50: 4c43 4169 626e 5674 6348 6c66 6448 6c77  LCAibnVtcHlfdHlw
 00001c60: 5a53 4936 4943 4a31 6157 3530 4e6a 5169  ZSI6ICJ1aW50NjQi
 00001c70: 4c43 4169 6257 5630 5957 5268 6447 4569  LCAibWV0YWRhdGEi
 00001c80: 4f69 4275 6457 7873 6656 3073 4943 4a6a  OiBudWxsfV0sICJj
 00001c90: 636d 5668 6447 3979 496a 6f67 6579 4a73  cmVhdG9yIjogeyJs
 00001ca0: 6157 4a79 5958 4a35 496a 6f67 496e 4235  aWJyYXJ5IjogInB5
 00001cb0: 5958 4a79 6233 6369 4c43 4169 646d 5679  YXJyb3ciLCAidmVy
-00001cc0: 6332 6c76 6269 4936 4943 4978 4e43 3477  c2lvbiI6ICIxNC4w
-00001cd0: 4c6a 4569 6653 7767 496e 4268 626d 5268  LjEifSwgInBhbmRh
+00001cc0: 6332 6c76 6269 4936 4943 4978 4e69 3477  c2lvbiI6ICIxNi4w
+00001cd0: 4c6a 4169 6653 7767 496e 4268 626d 5268  LjAifSwgInBhbmRh
 00001ce0: 6331 3932 5a58 4a7a 6157 3975 496a 6f67  c192ZXJzaW9uIjog
-00001cf0: 496a 4975 4d43 347a 496e 3041 4141 4141  IjIuMC4zIn0AAAAA
+00001cf0: 496a 4975 4d69 3479 496e 3041 4141 4141  IjIuMi4yIn0AAAAA
 00001d00: 4441 4141 4146 4143 4141 414d 4167 4141  DAAAAFACAAAMAgAA
 00001d10: 3441 4541 414b 6742 4141 4277 4151 4141  4AEAAKgBAABwAQAA
 00001d20: 4f41 4541 4141 7742 4141 4463 4141 4141  OAEAAAwBAADcAAAA
 00001d30: 7041 4141 4147 7741 4141 4134 4141 4141  pAAAAGwAAAA4AAAA
 00001d40: 4241 4141 4150 4439 2f2f 3841 4141 4543  BAAAAPD9//8AAAEC
 00001d50: 4541 4141 4142 7741 4141 4145 4141 4141  EAAAABwAAAAEAAAA
 00001d60: 4141 4141 4141 7341 4141 4274 5958 4a6e  AAAAAAsAAABtYXJn
@@ -514,11 +514,11 @@
 00002010: 4277 414d 4141 4141 4541 4151 4141 4141  BwAMAAAAEAAQAAAA
 00002020: 4141 4142 4168 4141 4141 4163 4141 4141  AAABAhAAAAAcAAAA
 00002030: 4241 4141 4141 4141 4141 4143 4141 4141  BAAAAAAAAAACAAAA
 00002040: 6157 5141 4141 6741 4441 4149 4141 6341  aWQAAAgADAAIAAcA
 00002050: 4341 4141 4141 4141 4141 4641 4141 4141  CAAAAAAAAAFAAAAA
 00002060: 4141 4141 4141 3d3d 0018 2070 6172 7175  AAAAAA==.. parqu
 00002070: 6574 2d63 7070 2d61 7272 6f77 2076 6572  et-cpp-arrow ver
-00002080: 7369 6f6e 2031 342e 302e 3119 cc1c 0000  sion 14.0.1.....
+00002080: 7369 6f6e 2031 362e 302e 3019 cc1c 0000  sion 16.0.0.....
 00002090: 1c00 001c 0000 1c00 001c 0000 1c00 001c  ................
 000020a0: 0000 1c00 001c 0000 1c00 001c 0000 1c00  ................
 000020b0: 0000 5218 0000 5041 5231                 ..R...PAR1
```

### Comparing `hipscat-0.3.3/tests/data/small_sky_order1_margin/Norder=1/Dir=0/Npix=47.parquet` & `hipscat-0.3.4/tests/data/small_sky_order1_margin/Norder=1/Dir=0/Npix=47.parquet`

 * *Files 1% similar despite different names*

```diff
@@ -307,17 +307,17 @@
 00001320: 6578 222c 2022 7061 6e64 6173 5f74 7970  ex", "pandas_typ
 00001330: 6522 3a20 2275 696e 7436 3422 2c20 226e  e": "uint64", "n
 00001340: 756d 7079 5f74 7970 6522 3a20 2275 696e  umpy_type": "uin
 00001350: 7436 3422 2c20 226d 6574 6164 6174 6122  t64", "metadata"
 00001360: 3a20 6e75 6c6c 7d5d 2c20 2263 7265 6174  : null}], "creat
 00001370: 6f72 223a 207b 226c 6962 7261 7279 223a  or": {"library":
 00001380: 2022 7079 6172 726f 7722 2c20 2276 6572   "pyarrow", "ver
-00001390: 7369 6f6e 223a 2022 3134 2e30 2e31 227d  sion": "14.0.1"}
+00001390: 7369 6f6e 223a 2022 3136 2e30 2e30 227d  sion": "16.0.0"}
 000013a0: 2c20 2270 616e 6461 735f 7665 7273 696f  , "pandas_versio
-000013b0: 6e22 3a20 2232 2e30 2e33 227d 0018 0c41  n": "2.0.3"}...A
+000013b0: 6e22 3a20 2232 2e32 2e32 227d 0018 0c41  n": "2.2.2"}...A
 000013c0: 5252 4f57 3a73 6368 656d 6118 f818 2f2f  RROW:schema...//
 000013d0: 2f2f 2f31 414a 4141 4151 4141 4141 4141  ///1AJAAAQAAAAAA
 000013e0: 414b 4141 3441 4267 4146 4141 6741 4367  AKAA4ABgAFAAgACg
 000013f0: 4141 4141 4142 4241 4151 4141 4141 4141  AAAAABBAAQAAAAAA
 00001400: 414b 4141 7741 4141 4145 4141 6741 4367  AKAAwAAAAEAAgACg
 00001410: 4141 414a 6747 4141 4145 4141 4141 4151  AAAJgGAAAEAAAAAQ
 00001420: 4141 4141 7741 4141 4149 4141 7741 4241  AAAAwAAAAIAAwABA
@@ -452,18 +452,18 @@
 00001c30: 4169 626e 5674 6348 6c66 6448 6c77 5a53  AibnVtcHlfdHlwZS
 00001c40: 4936 4943 4a31 6157 3530 4e6a 5169 4c43  I6ICJ1aW50NjQiLC
 00001c50: 4169 6257 5630 5957 5268 6447 4569 4f69  AibWV0YWRhdGEiOi
 00001c60: 4275 6457 7873 6656 3073 4943 4a6a 636d  BudWxsfV0sICJjcm
 00001c70: 5668 6447 3979 496a 6f67 6579 4a73 6157  VhdG9yIjogeyJsaW
 00001c80: 4a79 5958 4a35 496a 6f67 496e 4235 5958  JyYXJ5IjogInB5YX
 00001c90: 4a79 6233 6369 4c43 4169 646d 5679 6332  Jyb3ciLCAidmVyc2
-00001ca0: 6c76 6269 4936 4943 4978 4e43 3477 4c6a  lvbiI6ICIxNC4wLj
-00001cb0: 4569 6653 7767 496e 4268 626d 5268 6331  EifSwgInBhbmRhc1
+00001ca0: 6c76 6269 4936 4943 4978 4e69 3477 4c6a  lvbiI6ICIxNi4wLj
+00001cb0: 4169 6653 7767 496e 4268 626d 5268 6331  AifSwgInBhbmRhc1
 00001cc0: 3932 5a58 4a7a 6157 3975 496a 6f67 496a  92ZXJzaW9uIjogIj
-00001cd0: 4975 4d43 347a 496e 3041 4141 4141 4441  IuMC4zIn0AAAAADA
+00001cd0: 4975 4d69 3479 496e 3041 4141 4141 4441  IuMi4yIn0AAAAADA
 00001ce0: 4141 4146 4143 4141 414d 4167 4141 3441  AAAFACAAAMAgAA4A
 00001cf0: 4541 414b 6742 4141 4277 4151 4141 4f41  EAAKgBAABwAQAAOA
 00001d00: 4541 4141 7742 4141 4463 4141 4141 7041  EAAAwBAADcAAAApA
 00001d10: 4141 4147 7741 4141 4134 4141 4141 4241  AAAGwAAAA4AAAABA
 00001d20: 4141 4150 4439 2f2f 3841 4141 4543 4541  AAAPD9//8AAAECEA
 00001d30: 4141 4142 7741 4141 4145 4141 4141 4141  AAABwAAAAEAAAAAA
 00001d40: 4141 4141 7341 4141 4274 5958 4a6e 6157  AAAAsAAABtYXJnaW
@@ -512,11 +512,11 @@
 00001ff0: 414d 4141 4141 4541 4151 4141 4141 4141  AMAAAAEAAQAAAAAA
 00002000: 4142 4168 4141 4141 4163 4141 4141 4241  ABAhAAAAAcAAAABA
 00002010: 4141 4141 4141 4141 4143 4141 4141 6157  AAAAAAAAACAAAAaW
 00002020: 5141 4141 6741 4441 4149 4141 6341 4341  QAAAgADAAIAAcACA
 00002030: 4141 4141 4141 4141 4641 4141 4141 4141  AAAAAAAAFAAAAAAA
 00002040: 4141 4141 3d3d 0018 2070 6172 7175 6574  AAAA==.. parquet
 00002050: 2d63 7070 2d61 7272 6f77 2076 6572 7369  -cpp-arrow versi
-00002060: 6f6e 2031 342e 302e 3119 cc1c 0000 1c00  on 14.0.1.......
+00002060: 6f6e 2031 362e 302e 3019 cc1c 0000 1c00  on 16.0.0.......
 00002070: 001c 0000 1c00 001c 0000 1c00 001c 0000  ................
 00002080: 1c00 001c 0000 1c00 001c 0000 1c00 0000  ................
 00002090: 5218 0000 5041 5231                      R...PAR1
```

### Comparing `hipscat-0.3.3/tests/data/small_sky_order1_margin/README.md` & `hipscat-0.3.4/tests/data/small_sky_order1_margin/README.md`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.3/tests/data/small_sky_order1_margin/_common_metadata` & `hipscat-0.3.4/tests/data/small_sky_order1_margin/_common_metadata`

 * *Files 1% similar despite different names*

```diff
@@ -110,17 +110,17 @@
 000006d0: 6e64 6578 222c 2022 7061 6e64 6173 5f74  ndex", "pandas_t
 000006e0: 7970 6522 3a20 2275 696e 7436 3422 2c20  ype": "uint64", 
 000006f0: 226e 756d 7079 5f74 7970 6522 3a20 2275  "numpy_type": "u
 00000700: 696e 7436 3422 2c20 226d 6574 6164 6174  int64", "metadat
 00000710: 6122 3a20 6e75 6c6c 7d5d 2c20 2263 7265  a": null}], "cre
 00000720: 6174 6f72 223a 207b 226c 6962 7261 7279  ator": {"library
 00000730: 223a 2022 7079 6172 726f 7722 2c20 2276  ": "pyarrow", "v
-00000740: 6572 7369 6f6e 223a 2022 3134 2e30 2e31  ersion": "14.0.1
+00000740: 6572 7369 6f6e 223a 2022 3136 2e30 2e30  ersion": "16.0.0
 00000750: 227d 2c20 2270 616e 6461 735f 7665 7273  "}, "pandas_vers
-00000760: 696f 6e22 3a20 2232 2e30 2e33 227d 0018  ion": "2.0.3"}..
+00000760: 696f 6e22 3a20 2232 2e32 2e32 227d 0018  ion": "2.2.2"}..
 00000770: 0c41 5252 4f57 3a73 6368 656d 6118 f818  .ARROW:schema...
 00000780: 2f2f 2f2f 2f31 414a 4141 4151 4141 4141  /////1AJAAAQAAAA
 00000790: 4141 414b 4141 3441 4267 4146 4141 6741  AAAKAA4ABgAFAAgA
 000007a0: 4367 4141 4141 4142 4241 4151 4141 4141  CgAAAAABBAAQAAAA
 000007b0: 4141 414b 4141 7741 4141 4145 4141 6741  AAAKAAwAAAAEAAgA
 000007c0: 4367 4141 414a 6747 4141 4145 4141 4141  CgAAAJgGAAAEAAAA
 000007d0: 4151 4141 4141 7741 4141 4149 4141 7741  AQAAAAwAAAAIAAwA
@@ -255,18 +255,18 @@
 00000fe0: 4c43 4169 626e 5674 6348 6c66 6448 6c77  LCAibnVtcHlfdHlw
 00000ff0: 5a53 4936 4943 4a31 6157 3530 4e6a 5169  ZSI6ICJ1aW50NjQi
 00001000: 4c43 4169 6257 5630 5957 5268 6447 4569  LCAibWV0YWRhdGEi
 00001010: 4f69 4275 6457 7873 6656 3073 4943 4a6a  OiBudWxsfV0sICJj
 00001020: 636d 5668 6447 3979 496a 6f67 6579 4a73  cmVhdG9yIjogeyJs
 00001030: 6157 4a79 5958 4a35 496a 6f67 496e 4235  aWJyYXJ5IjogInB5
 00001040: 5958 4a79 6233 6369 4c43 4169 646d 5679  YXJyb3ciLCAidmVy
-00001050: 6332 6c76 6269 4936 4943 4978 4e43 3477  c2lvbiI6ICIxNC4w
-00001060: 4c6a 4569 6653 7767 496e 4268 626d 5268  LjEifSwgInBhbmRh
+00001050: 6332 6c76 6269 4936 4943 4978 4e69 3477  c2lvbiI6ICIxNi4w
+00001060: 4c6a 4169 6653 7767 496e 4268 626d 5268  LjAifSwgInBhbmRh
 00001070: 6331 3932 5a58 4a7a 6157 3975 496a 6f67  c192ZXJzaW9uIjog
-00001080: 496a 4975 4d43 347a 496e 3041 4141 4141  IjIuMC4zIn0AAAAA
+00001080: 496a 4975 4d69 3479 496e 3041 4141 4141  IjIuMi4yIn0AAAAA
 00001090: 4441 4141 4146 4143 4141 414d 4167 4141  DAAAAFACAAAMAgAA
 000010a0: 3441 4541 414b 6742 4141 4277 4151 4141  4AEAAKgBAABwAQAA
 000010b0: 4f41 4541 4141 7742 4141 4463 4141 4141  OAEAAAwBAADcAAAA
 000010c0: 7041 4141 4147 7741 4141 4134 4141 4141  pAAAAGwAAAA4AAAA
 000010d0: 4241 4141 4150 4439 2f2f 3841 4141 4543  BAAAAPD9//8AAAEC
 000010e0: 4541 4141 4142 7741 4141 4145 4141 4141  EAAAABwAAAAEAAAA
 000010f0: 4141 4141 4141 7341 4141 4274 5958 4a6e  AAAAAAsAAABtYXJn
@@ -315,11 +315,11 @@
 000013a0: 4277 414d 4141 4141 4541 4151 4141 4141  BwAMAAAAEAAQAAAA
 000013b0: 4141 4142 4168 4141 4141 4163 4141 4141  AAABAhAAAAAcAAAA
 000013c0: 4241 4141 4141 4141 4141 4143 4141 4141  BAAAAAAAAAACAAAA
 000013d0: 6157 5141 4141 6741 4441 4149 4141 6341  aWQAAAgADAAIAAcA
 000013e0: 4341 4141 4141 4141 4141 4641 4141 4141  CAAAAAAAAAFAAAAA
 000013f0: 4141 4141 4141 3d3d 0018 2070 6172 7175  AAAAAA==.. parqu
 00001400: 6574 2d63 7070 2d61 7272 6f77 2076 6572  et-cpp-arrow ver
-00001410: 7369 6f6e 2031 342e 302e 3119 cc1c 0000  sion 14.0.1.....
+00001410: 7369 6f6e 2031 362e 302e 3019 cc1c 0000  sion 16.0.0.....
 00001420: 1c00 001c 0000 1c00 001c 0000 1c00 001c  ................
 00001430: 0000 1c00 001c 0000 1c00 001c 0000 1c00  ................
 00001440: 0000 3e14 0000 5041 5231                 ..>...PAR1
```

### Comparing `hipscat-0.3.3/tests/data/small_sky_order1_margin/_metadata` & `hipscat-0.3.4/tests/data/small_sky_order1_margin/_metadata`

 * *Files 1% similar despite different names*

```diff
@@ -560,17 +560,17 @@
 000022f0: 6e64 6173 5f74 7970 6522 3a20 2275 696e  ndas_type": "uin
 00002300: 7436 3422 2c20 226e 756d 7079 5f74 7970  t64", "numpy_typ
 00002310: 6522 3a20 2275 696e 7436 3422 2c20 226d  e": "uint64", "m
 00002320: 6574 6164 6174 6122 3a20 6e75 6c6c 7d5d  etadata": null}]
 00002330: 2c20 2263 7265 6174 6f72 223a 207b 226c  , "creator": {"l
 00002340: 6962 7261 7279 223a 2022 7079 6172 726f  ibrary": "pyarro
 00002350: 7722 2c20 2276 6572 7369 6f6e 223a 2022  w", "version": "
-00002360: 3134 2e30 2e31 227d 2c20 2270 616e 6461  14.0.1"}, "panda
-00002370: 735f 7665 7273 696f 6e22 3a20 2232 2e30  s_version": "2.0
-00002380: 2e33 227d 0018 0c41 5252 4f57 3a73 6368  .3"}...ARROW:sch
+00002360: 3136 2e30 2e30 227d 2c20 2270 616e 6461  16.0.0"}, "panda
+00002370: 735f 7665 7273 696f 6e22 3a20 2232 2e32  s_version": "2.2
+00002380: 2e32 227d 0018 0c41 5252 4f57 3a73 6368  .2"}...ARROW:sch
 00002390: 656d 6118 f818 2f2f 2f2f 2f31 414a 4141  ema.../////1AJAA
 000023a0: 4151 4141 4141 4141 414b 4141 3441 4267  AQAAAAAAAKAA4ABg
 000023b0: 4146 4141 6741 4367 4141 4141 4142 4241  AFAAgACgAAAAABBA
 000023c0: 4151 4141 4141 4141 414b 4141 7741 4141  AQAAAAAAAKAAwAAA
 000023d0: 4145 4141 6741 4367 4141 414a 6747 4141  AEAAgACgAAAJgGAA
 000023e0: 4145 4141 4141 4151 4141 4141 7741 4141  AEAAAAAQAAAAwAAA
 000023f0: 4149 4141 7741 4241 4149 4141 6741 4141  AIAAwABAAIAAgAAA
@@ -705,17 +705,17 @@
 00002c00: 6c66 6448 6c77 5a53 4936 4943 4a31 6157  lfdHlwZSI6ICJ1aW
 00002c10: 3530 4e6a 5169 4c43 4169 6257 5630 5957  50NjQiLCAibWV0YW
 00002c20: 5268 6447 4569 4f69 4275 6457 7873 6656  RhdGEiOiBudWxsfV
 00002c30: 3073 4943 4a6a 636d 5668 6447 3979 496a  0sICJjcmVhdG9yIj
 00002c40: 6f67 6579 4a73 6157 4a79 5958 4a35 496a  ogeyJsaWJyYXJ5Ij
 00002c50: 6f67 496e 4235 5958 4a79 6233 6369 4c43  ogInB5YXJyb3ciLC
 00002c60: 4169 646d 5679 6332 6c76 6269 4936 4943  AidmVyc2lvbiI6IC
-00002c70: 4978 4e43 3477 4c6a 4569 6653 7767 496e  IxNC4wLjEifSwgIn
+00002c70: 4978 4e69 3477 4c6a 4169 6653 7767 496e  IxNi4wLjAifSwgIn
 00002c80: 4268 626d 5268 6331 3932 5a58 4a7a 6157  BhbmRhc192ZXJzaW
-00002c90: 3975 496a 6f67 496a 4975 4d43 347a 496e  9uIjogIjIuMC4zIn
+00002c90: 3975 496a 6f67 496a 4975 4d69 3479 496e  9uIjogIjIuMi4yIn
 00002ca0: 3041 4141 4141 4441 4141 4146 4143 4141  0AAAAADAAAAFACAA
 00002cb0: 414d 4167 4141 3441 4541 414b 6742 4141  AMAgAA4AEAAKgBAA
 00002cc0: 4277 4151 4141 4f41 4541 4141 7742 4141  BwAQAAOAEAAAwBAA
 00002cd0: 4463 4141 4141 7041 4141 4147 7741 4141  DcAAAApAAAAGwAAA
 00002ce0: 4134 4141 4141 4241 4141 4150 4439 2f2f  A4AAAABAAAAPD9//
 00002cf0: 3841 4141 4543 4541 4141 4142 7741 4141  8AAAECEAAAABwAAA
 00002d00: 4145 4141 4141 4141 4141 4141 7341 4141  AEAAAAAAAAAAsAAA
@@ -764,11 +764,11 @@
 00002fb0: 4149 4141 5941 4277 414d 4141 4141 4541  AIAAYABwAMAAAAEA
 00002fc0: 4151 4141 4141 4141 4142 4168 4141 4141  AQAAAAAAABAhAAAA
 00002fd0: 4163 4141 4141 4241 4141 4141 4141 4141  AcAAAABAAAAAAAAA
 00002fe0: 4143 4141 4141 6157 5141 4141 6741 4441  ACAAAAaWQAAAgADA
 00002ff0: 4149 4141 6341 4341 4141 4141 4141 4141  AIAAcACAAAAAAAAA
 00003000: 4641 4141 4141 4141 4141 4141 3d3d 0018  FAAAAAAAAAAA==..
 00003010: 2070 6172 7175 6574 2d63 7070 2d61 7272   parquet-cpp-arr
-00003020: 6f77 2076 6572 7369 6f6e 2031 342e 302e  ow version 14.0.
-00003030: 3119 cc1c 0000 1c00 001c 0000 1c00 001c  1...............
+00003020: 6f77 2076 6572 7369 6f6e 2031 362e 302e  ow version 16.0.
+00003030: 3019 cc1c 0000 1c00 001c 0000 1c00 001c  0...............
 00003040: 0000 1c00 001c 0000 1c00 001c 0000 1c00  ................
 00003050: 001c 0000 1c00 0000 5430 0000 5041 5231  ........T0..PAR1
```

### Comparing `hipscat-0.3.3/tests/data/small_sky_order1_margin/provenance_info.json` & `hipscat-0.3.4/tests/data/small_sky_order1_margin/provenance_info.json`

 * *Files 26% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7992788461538461%*

 * *Differences: {"'generation_date'": "'2024.05.29'",*

 * * "'primary_catalog'": "'small_sky_order1'",*

 * * "'tool_args'": "{'version': '0.3.3.dev10+gd573bcd', 'runtime_args': {'output_path': '.', "*

 * *                "'tmp_dir': '/tmp/tmp8j6vsyq2', 'catalog_path': './small_sky_order1_margin', "*

 * *                "'tmp_path': '/tmp/tmp8j6vsyq2/small_sky_order1_margin/intermediate', "*

 * *                "'input_catalog_path': 'small_sky_order1', delete: ['overwrite']}}",*

 * * "'version'": "'0.3.4.dev17+g922a4b7.d20240529'"}*

```diff
@@ -1,28 +1,27 @@
 {
     "catalog_name": "small_sky_order1_margin",
     "catalog_type": "margin",
-    "generation_date": "2024.01.30",
+    "generation_date": "2024.05.29",
     "margin_threshold": 7200,
-    "primary_catalog": "data/small_sky_order1",
+    "primary_catalog": "small_sky_order1",
     "tool_args": {
         "runtime_args": {
             "catalog_name": "small_sky_order1_margin",
-            "catalog_path": "data/small_sky_order1_margin",
+            "catalog_path": "./small_sky_order1_margin",
             "dask_n_workers": 1,
             "dask_threads_per_worker": 1,
             "dask_tmp": "",
-            "input_catalog_path": "data/small_sky_order1",
+            "input_catalog_path": "small_sky_order1",
             "margin_order": 2,
             "margin_threshold": 7200,
             "output_artifact_name": "small_sky_order1_margin",
-            "output_path": "data/",
-            "overwrite": false,
-            "tmp_dir": "",
-            "tmp_path": "data/small_sky_order1_margin/intermediate"
+            "output_path": ".",
+            "tmp_dir": "/tmp/tmp8j6vsyq2",
+            "tmp_path": "/tmp/tmp8j6vsyq2/small_sky_order1_margin/intermediate"
         },
         "tool_name": "hipscat_import",
-        "version": "0.2.2"
+        "version": "0.3.3.dev10+gd573bcd"
     },
     "total_rows": 28,
-    "version": "0.2.3"
+    "version": "0.3.4.dev17+g922a4b7.d20240529"
 }
```

### Comparing `hipscat-0.3.3/tests/data/small_sky_source/Norder=0/Dir=0/Npix=4.parquet` & `hipscat-0.3.4/tests/data/small_sky_source/Norder=0/Dir=0/Npix=4.parquet`

 * *Files 0% similar despite different names*

```diff
@@ -486,17 +486,17 @@
 00001e50: 222c 2022 7061 6e64 6173 5f74 7970 6522  ", "pandas_type"
 00001e60: 3a20 2275 696e 7436 3422 2c20 226e 756d  : "uint64", "num
 00001e70: 7079 5f74 7970 6522 3a20 2275 696e 7436  py_type": "uint6
 00001e80: 3422 2c20 226d 6574 6164 6174 6122 3a20  4", "metadata": 
 00001e90: 6e75 6c6c 7d5d 2c20 2263 7265 6174 6f72  null}], "creator
 00001ea0: 223a 207b 226c 6962 7261 7279 223a 2022  ": {"library": "
 00001eb0: 7079 6172 726f 7722 2c20 2276 6572 7369  pyarrow", "versi
-00001ec0: 6f6e 223a 2022 3134 2e30 2e31 227d 2c20  on": "14.0.1"}, 
+00001ec0: 6f6e 223a 2022 3136 2e30 2e30 227d 2c20  on": "16.0.0"}, 
 00001ed0: 2270 616e 6461 735f 7665 7273 696f 6e22  "pandas_version"
-00001ee0: 3a20 2232 2e30 2e33 227d 0018 0c41 5252  : "2.0.3"}...ARR
+00001ee0: 3a20 2232 2e32 2e32 227d 0018 0c41 5252  : "2.2.2"}...ARR
 00001ef0: 4f57 3a73 6368 656d 6118 cc1a 2f2f 2f2f  OW:schema...////
 00001f00: 2f2f 414a 4141 4151 4141 4141 4141 414b  //AJAAAQAAAAAAAK
 00001f10: 4141 3441 4267 4146 4141 6741 4367 4141  AA4ABgAFAAgACgAA
 00001f20: 4141 4142 4241 4151 4141 4141 4141 414b  AAABBAAQAAAAAAAK
 00001f30: 4141 7741 4141 4145 4141 6741 4367 4141  AAwAAAAEAAgACgAA
 00001f40: 4142 4148 4141 4145 4141 4141 4151 4141  ABAHAAAEAAAAAQAA
 00001f50: 4141 7741 4141 4149 4141 7741 4241 4149  AAwAAAAIAAwABAAI
@@ -641,18 +641,18 @@
 00002800: 4943 4a75 6457 3177 6556 3930 6558 426c  ICJudW1weV90eXBl
 00002810: 496a 6f67 496e 5670 626e 5132 4e43 4973  IjogInVpbnQ2NCIs
 00002820: 4943 4a74 5a58 5268 5a47 4630 5953 4936  ICJtZXRhZGF0YSI6
 00002830: 4947 3531 6247 7839 5853 7767 496d 4e79  IG51bGx9XSwgImNy
 00002840: 5a57 4630 6233 4969 4f69 4237 496d 7870  ZWF0b3IiOiB7Imxp
 00002850: 596e 4a68 636e 6b69 4f69 4169 6348 6c68  YnJhcnkiOiAicHlh
 00002860: 636e 4a76 6479 4973 4943 4a32 5a58 4a7a  cnJvdyIsICJ2ZXJz
-00002870: 6157 3975 496a 6f67 496a 4530 4c6a 4175  aW9uIjogIjE0LjAu
-00002880: 4d53 4a39 4c43 4169 6347 4675 5a47 467a  MSJ9LCAicGFuZGFz
+00002870: 6157 3975 496a 6f67 496a 4532 4c6a 4175  aW9uIjogIjE2LjAu
+00002880: 4d43 4a39 4c43 4169 6347 4675 5a47 467a  MCJ9LCAicGFuZGFz
 00002890: 5833 5a6c 636e 4e70 6232 3469 4f69 4169  X3ZlcnNpb24iOiAi
-000028a0: 4d69 3477 4c6a 4d69 6651 4141 4451 4141  Mi4wLjMifQAADQAA
+000028a0: 4d69 3479 4c6a 4969 6651 4141 4451 4141  Mi4yLjIifQAADQAA
 000028b0: 4148 5143 4141 4173 4167 4141 2b41 4541  AHQCAAAsAgAA+AEA
 000028c0: 414d 7742 4141 4367 4151 4141 6341 4541  AMwBAACgAQAAcAEA
 000028d0: 4144 6742 4141 4145 4151 4141 3041 4141  ADgBAAAEAQAA0AAA
 000028e0: 414a 6741 4141 4273 4141 4141 5041 4141  AJgAAABsAAAAPAAA
 000028f0: 4141 5141 4141 4451 2f66 2f2f 4141 4142  AAQAAADQ/f//AAAB
 00002900: 4168 4141 4141 4167 4141 4141 4241 4141  AhAAAAAgAAAABAAA
 00002910: 4141 4141 4141 414f 4141 4141 5832 6870  AAAAAAAOAAAAX2hp
@@ -704,11 +704,11 @@
 00002bf0: 4141 4141 4541 4151 4141 4141 4141 4142  AAAAEAAQAAAAAAAB
 00002c00: 4168 4141 4141 416b 4141 4141 4241 4141  AhAAAAAkAAAABAAA
 00002c10: 4141 4141 4141 414a 4141 4141 6332 3931  AAAAAAAJAAAAc291
 00002c20: 636d 4e6c 5832 6c6b 4141 4141 4341 414d  cmNlX2lkAAAACAAM
 00002c30: 4141 6741 4277 4149 4141 4141 4141 4141  AAgABwAIAAAAAAAA
 00002c40: 4155 4141 4141 413d 0018 2070 6172 7175  AUAAAAA=.. parqu
 00002c50: 6574 2d63 7070 2d61 7272 6f77 2076 6572  et-cpp-arrow ver
-00002c60: 7369 6f6e 2031 342e 302e 3119 dc1c 0000  sion 14.0.1.....
+00002c60: 7369 6f6e 2031 362e 302e 3019 dc1c 0000  sion 16.0.0.....
 00002c70: 1c00 001c 0000 1c00 001c 0000 1c00 001c  ................
 00002c80: 0000 1c00 001c 0000 1c00 001c 0000 1c00  ................
 00002c90: 001c 0000 0025 1a00 0050 4152 31         .....%...PAR1
```

### Comparing `hipscat-0.3.3/tests/data/small_sky_source/Norder=1/Dir=0/Npix=47.parquet` & `hipscat-0.3.4/tests/data/small_sky_source/Norder=1/Dir=0/Npix=47.parquet`

 * *Files 0% similar despite different names*

```diff
@@ -8127,17 +8127,17 @@
 0001fbe0: 6e64 6173 5f74 7970 6522 3a20 2275 696e  ndas_type": "uin
 0001fbf0: 7436 3422 2c20 226e 756d 7079 5f74 7970  t64", "numpy_typ
 0001fc00: 6522 3a20 2275 696e 7436 3422 2c20 226d  e": "uint64", "m
 0001fc10: 6574 6164 6174 6122 3a20 6e75 6c6c 7d5d  etadata": null}]
 0001fc20: 2c20 2263 7265 6174 6f72 223a 207b 226c  , "creator": {"l
 0001fc30: 6962 7261 7279 223a 2022 7079 6172 726f  ibrary": "pyarro
 0001fc40: 7722 2c20 2276 6572 7369 6f6e 223a 2022  w", "version": "
-0001fc50: 3134 2e30 2e31 227d 2c20 2270 616e 6461  14.0.1"}, "panda
-0001fc60: 735f 7665 7273 696f 6e22 3a20 2232 2e30  s_version": "2.0
-0001fc70: 2e33 227d 0018 0c41 5252 4f57 3a73 6368  .3"}...ARROW:sch
+0001fc50: 3136 2e30 2e30 227d 2c20 2270 616e 6461  16.0.0"}, "panda
+0001fc60: 735f 7665 7273 696f 6e22 3a20 2232 2e32  s_version": "2.2
+0001fc70: 2e32 227d 0018 0c41 5252 4f57 3a73 6368  .2"}...ARROW:sch
 0001fc80: 656d 6118 cc1a 2f2f 2f2f 2f2f 414a 4141  ema...//////AJAA
 0001fc90: 4151 4141 4141 4141 414b 4141 3441 4267  AQAAAAAAAKAA4ABg
 0001fca0: 4146 4141 6741 4367 4141 4141 4142 4241  AFAAgACgAAAAABBA
 0001fcb0: 4151 4141 4141 4141 414b 4141 7741 4141  AQAAAAAAAKAAwAAA
 0001fcc0: 4145 4141 6741 4367 4141 4142 4148 4141  AEAAgACgAAABAHAA
 0001fcd0: 4145 4141 4141 4151 4141 4141 7741 4141  AEAAAAAQAAAAwAAA
 0001fce0: 4149 4141 7741 4241 4149 4141 6741 4141  AIAAwABAAIAAgAAA
@@ -8282,18 +8282,18 @@
 00020590: 3177 6556 3930 6558 426c 496a 6f67 496e  1weV90eXBlIjogIn
 000205a0: 5670 626e 5132 4e43 4973 4943 4a74 5a58  VpbnQ2NCIsICJtZX
 000205b0: 5268 5a47 4630 5953 4936 4947 3531 6247  RhZGF0YSI6IG51bG
 000205c0: 7839 5853 7767 496d 4e79 5a57 4630 6233  x9XSwgImNyZWF0b3
 000205d0: 4969 4f69 4237 496d 7870 596e 4a68 636e  IiOiB7ImxpYnJhcn
 000205e0: 6b69 4f69 4169 6348 6c68 636e 4a76 6479  kiOiAicHlhcnJvdy
 000205f0: 4973 4943 4a32 5a58 4a7a 6157 3975 496a  IsICJ2ZXJzaW9uIj
-00020600: 6f67 496a 4530 4c6a 4175 4d53 4a39 4c43  ogIjE0LjAuMSJ9LC
+00020600: 6f67 496a 4532 4c6a 4175 4d43 4a39 4c43  ogIjE2LjAuMCJ9LC
 00020610: 4169 6347 4675 5a47 467a 5833 5a6c 636e  AicGFuZGFzX3Zlcn
-00020620: 4e70 6232 3469 4f69 4169 4d69 3477 4c6a  Npb24iOiAiMi4wLj
-00020630: 4d69 6651 4141 4451 4141 4148 5143 4141  MifQAADQAAAHQCAA
+00020620: 4e70 6232 3469 4f69 4169 4d69 3479 4c6a  Npb24iOiAiMi4yLj
+00020630: 4969 6651 4141 4451 4141 4148 5143 4141  IifQAADQAAAHQCAA
 00020640: 4173 4167 4141 2b41 4541 414d 7742 4141  AsAgAA+AEAAMwBAA
 00020650: 4367 4151 4141 6341 4541 4144 6742 4141  CgAQAAcAEAADgBAA
 00020660: 4145 4151 4141 3041 4141 414a 6741 4141  AEAQAA0AAAAJgAAA
 00020670: 4273 4141 4141 5041 4141 4141 5141 4141  BsAAAAPAAAAAQAAA
 00020680: 4451 2f66 2f2f 4141 4142 4168 4141 4141  DQ/f//AAABAhAAAA
 00020690: 4167 4141 4141 4241 4141 4141 4141 4141  AgAAAABAAAAAAAAA
 000206a0: 414f 4141 4141 5832 6870 6348 4e6a 5958  AOAAAAX2hpcHNjYX
@@ -8345,11 +8345,11 @@
 00020980: 4151 4141 4141 4141 4142 4168 4141 4141  AQAAAAAAABAhAAAA
 00020990: 416b 4141 4141 4241 4141 4141 4141 4141  AkAAAABAAAAAAAAA
 000209a0: 414a 4141 4141 6332 3931 636d 4e6c 5832  AJAAAAc291cmNlX2
 000209b0: 6c6b 4141 4141 4341 414d 4141 6741 4277  lkAAAACAAMAAgABw
 000209c0: 4149 4141 4141 4141 4141 4155 4141 4141  AIAAAAAAAAAUAAAA
 000209d0: 413d 0018 2070 6172 7175 6574 2d63 7070  A=.. parquet-cpp
 000209e0: 2d61 7272 6f77 2076 6572 7369 6f6e 2031  -arrow version 1
-000209f0: 342e 302e 3119 dc1c 0000 1c00 001c 0000  4.0.1...........
+000209f0: 362e 302e 3019 dc1c 0000 1c00 001c 0000  6.0.0...........
 00020a00: 1c00 001c 0000 1c00 001c 0000 1c00 001c  ................
 00020a10: 0000 1c00 001c 0000 1c00 001c 0000 0068  ...............h
 00020a20: 1a00 0050 4152 31                        ...PAR1
```

### Comparing `hipscat-0.3.3/tests/data/small_sky_source/Norder=2/Dir=0/Npix=176.parquet` & `hipscat-0.3.4/tests/data/small_sky_source/Norder=2/Dir=0/Npix=176.parquet`

 * *Files 1% similar despite different names*

```diff
@@ -1544,17 +1544,17 @@
 00006070: 2270 616e 6461 735f 7479 7065 223a 2022  "pandas_type": "
 00006080: 7569 6e74 3634 222c 2022 6e75 6d70 795f  uint64", "numpy_
 00006090: 7479 7065 223a 2022 7569 6e74 3634 222c  type": "uint64",
 000060a0: 2022 6d65 7461 6461 7461 223a 206e 756c   "metadata": nul
 000060b0: 6c7d 5d2c 2022 6372 6561 746f 7222 3a20  l}], "creator": 
 000060c0: 7b22 6c69 6272 6172 7922 3a20 2270 7961  {"library": "pya
 000060d0: 7272 6f77 222c 2022 7665 7273 696f 6e22  rrow", "version"
-000060e0: 3a20 2231 342e 302e 3122 7d2c 2022 7061  : "14.0.1"}, "pa
+000060e0: 3a20 2231 362e 302e 3022 7d2c 2022 7061  : "16.0.0"}, "pa
 000060f0: 6e64 6173 5f76 6572 7369 6f6e 223a 2022  ndas_version": "
-00006100: 322e 302e 3322 7d00 180c 4152 524f 573a  2.0.3"}...ARROW:
+00006100: 322e 322e 3222 7d00 180c 4152 524f 573a  2.2.2"}...ARROW:
 00006110: 7363 6865 6d61 18cc 1a2f 2f2f 2f2f 2f41  schema...//////A
 00006120: 4a41 4141 5141 4141 4141 4141 4b41 4134  JAAAQAAAAAAAKAA4
 00006130: 4142 6741 4641 4167 4143 6741 4141 4141  ABgAFAAgACgAAAAA
 00006140: 4242 4141 5141 4141 4141 4141 4b41 4177  BBAAQAAAAAAAKAAw
 00006150: 4141 4141 4541 4167 4143 6741 4141 4241  AAAAEAAgACgAAABA
 00006160: 4841 4141 4541 4141 4141 5141 4141 4177  HAAAEAAAAAQAAAAw
 00006170: 4141 4141 4941 4177 4142 4141 4941 4167  AAAAIAAwABAAIAAg
@@ -1699,18 +1699,18 @@
 00006a20: 7564 5731 7765 5639 3065 5842 6c49 6a6f  udW1weV90eXBlIjo
 00006a30: 6749 6e56 7062 6e51 324e 4349 7349 434a  gInVpbnQ2NCIsICJ
 00006a40: 745a 5852 685a 4746 3059 5349 3649 4735  tZXRhZGF0YSI6IG5
 00006a50: 3162 4778 3958 5377 6749 6d4e 795a 5746  1bGx9XSwgImNyZWF
 00006a60: 3062 3349 694f 6942 3749 6d78 7059 6e4a  0b3IiOiB7ImxpYnJ
 00006a70: 6863 6e6b 694f 6941 6963 486c 6863 6e4a  hcnkiOiAicHlhcnJ
 00006a80: 7664 7949 7349 434a 325a 584a 7a61 5739  vdyIsICJ2ZXJzaW9
-00006a90: 7549 6a6f 6749 6a45 304c 6a41 754d 534a  uIjogIjE0LjAuMSJ
+00006a90: 7549 6a6f 6749 6a45 324c 6a41 754d 434a  uIjogIjE2LjAuMCJ
 00006aa0: 394c 4341 6963 4746 755a 4746 7a58 335a  9LCAicGFuZGFzX3Z
 00006ab0: 6c63 6e4e 7062 3234 694f 6941 694d 6934  lcnNpb24iOiAiMi4
-00006ac0: 774c 6a4d 6966 5141 4144 5141 4141 4851  wLjMifQAADQAAAHQ
+00006ac0: 794c 6a49 6966 5141 4144 5141 4141 4851  yLjIifQAADQAAAHQ
 00006ad0: 4341 4141 7341 6741 412b 4145 4141 4d77  CAAAsAgAA+AEAAMw
 00006ae0: 4241 4143 6741 5141 4163 4145 4141 4467  BAACgAQAAcAEAADg
 00006af0: 4241 4141 4541 5141 4130 4141 4141 4a67  BAAAEAQAA0AAAAJg
 00006b00: 4141 4142 7341 4141 4150 4141 4141 4151  AAABsAAAAPAAAAAQ
 00006b10: 4141 4144 512f 662f 2f41 4141 4241 6841  AAADQ/f//AAABAhA
 00006b20: 4141 4141 6741 4141 4142 4141 4141 4141  AAAAgAAAABAAAAAA
 00006b30: 4141 4141 4f41 4141 4158 3268 7063 484e  AAAAOAAAAX2hpcHN
@@ -1762,11 +1762,11 @@
 00006e10: 4145 4141 5141 4141 4141 4141 4241 6841  AEAAQAAAAAAABAhA
 00006e20: 4141 4141 6b41 4141 4142 4141 4141 4141  AAAAkAAAABAAAAAA
 00006e30: 4141 4141 4a41 4141 4163 3239 3163 6d4e  AAAAJAAAAc291cmN
 00006e40: 6c58 326c 6b41 4141 4143 4141 4d41 4167  lX2lkAAAACAAMAAg
 00006e50: 4142 7741 4941 4141 4141 4141 4141 5541  ABwAIAAAAAAAAAUA
 00006e60: 4141 4141 3d00 1820 7061 7271 7565 742d  AAAA=.. parquet-
 00006e70: 6370 702d 6172 726f 7720 7665 7273 696f  cpp-arrow versio
-00006e80: 6e20 3134 2e30 2e31 19dc 1c00 001c 0000  n 14.0.1........
+00006e80: 6e20 3136 2e30 2e30 19dc 1c00 001c 0000  n 16.0.0........
 00006e90: 1c00 001c 0000 1c00 001c 0000 1c00 001c  ................
 00006ea0: 0000 1c00 001c 0000 1c00 001c 0000 1c00  ................
 00006eb0: 0000 561a 0000 5041 5231                 ..V...PAR1
```

### Comparing `hipscat-0.3.3/tests/data/small_sky_source/Norder=2/Dir=0/Npix=177.parquet` & `hipscat-0.3.4/tests/data/small_sky_source/Norder=2/Dir=0/Npix=177.parquet`

 * *Files 0% similar despite different names*

```diff
@@ -5164,17 +5164,17 @@
 000142b0: 6461 735f 7479 7065 223a 2022 7569 6e74  das_type": "uint
 000142c0: 3634 222c 2022 6e75 6d70 795f 7479 7065  64", "numpy_type
 000142d0: 223a 2022 7569 6e74 3634 222c 2022 6d65  ": "uint64", "me
 000142e0: 7461 6461 7461 223a 206e 756c 6c7d 5d2c  tadata": null}],
 000142f0: 2022 6372 6561 746f 7222 3a20 7b22 6c69   "creator": {"li
 00014300: 6272 6172 7922 3a20 2270 7961 7272 6f77  brary": "pyarrow
 00014310: 222c 2022 7665 7273 696f 6e22 3a20 2231  ", "version": "1
-00014320: 342e 302e 3122 7d2c 2022 7061 6e64 6173  4.0.1"}, "pandas
-00014330: 5f76 6572 7369 6f6e 223a 2022 322e 302e  _version": "2.0.
-00014340: 3322 7d00 180c 4152 524f 573a 7363 6865  3"}...ARROW:sche
+00014320: 362e 302e 3022 7d2c 2022 7061 6e64 6173  6.0.0"}, "pandas
+00014330: 5f76 6572 7369 6f6e 223a 2022 322e 322e  _version": "2.2.
+00014340: 3222 7d00 180c 4152 524f 573a 7363 6865  2"}...ARROW:sche
 00014350: 6d61 18cc 1a2f 2f2f 2f2f 2f41 4a41 4141  ma...//////AJAAA
 00014360: 5141 4141 4141 4141 4b41 4134 4142 6741  QAAAAAAAKAA4ABgA
 00014370: 4641 4167 4143 6741 4141 4141 4242 4141  FAAgACgAAAAABBAA
 00014380: 5141 4141 4141 4141 4b41 4177 4141 4141  QAAAAAAAKAAwAAAA
 00014390: 4541 4167 4143 6741 4141 4241 4841 4141  EAAgACgAAABAHAAA
 000143a0: 4541 4141 4141 5141 4141 4177 4141 4141  EAAAAAQAAAAwAAAA
 000143b0: 4941 4177 4142 4141 4941 4167 4141 4141  IAAwABAAIAAgAAAA
@@ -5319,17 +5319,17 @@
 00014c60: 7765 5639 3065 5842 6c49 6a6f 6749 6e56  weV90eXBlIjogInV
 00014c70: 7062 6e51 324e 4349 7349 434a 745a 5852  pbnQ2NCIsICJtZXR
 00014c80: 685a 4746 3059 5349 3649 4735 3162 4778  hZGF0YSI6IG51bGx
 00014c90: 3958 5377 6749 6d4e 795a 5746 3062 3349  9XSwgImNyZWF0b3I
 00014ca0: 694f 6942 3749 6d78 7059 6e4a 6863 6e6b  iOiB7ImxpYnJhcnk
 00014cb0: 694f 6941 6963 486c 6863 6e4a 7664 7949  iOiAicHlhcnJvdyI
 00014cc0: 7349 434a 325a 584a 7a61 5739 7549 6a6f  sICJ2ZXJzaW9uIjo
-00014cd0: 6749 6a45 304c 6a41 754d 534a 394c 4341  gIjE0LjAuMSJ9LCA
+00014cd0: 6749 6a45 324c 6a41 754d 434a 394c 4341  gIjE2LjAuMCJ9LCA
 00014ce0: 6963 4746 755a 4746 7a58 335a 6c63 6e4e  icGFuZGFzX3ZlcnN
-00014cf0: 7062 3234 694f 6941 694d 6934 774c 6a4d  pb24iOiAiMi4wLjM
+00014cf0: 7062 3234 694f 6941 694d 6934 794c 6a49  pb24iOiAiMi4yLjI
 00014d00: 6966 5141 4144 5141 4141 4851 4341 4141  ifQAADQAAAHQCAAA
 00014d10: 7341 6741 412b 4145 4141 4d77 4241 4143  sAgAA+AEAAMwBAAC
 00014d20: 6741 5141 4163 4145 4141 4467 4241 4141  gAQAAcAEAADgBAAA
 00014d30: 4541 5141 4130 4141 4141 4a67 4141 4142  EAQAA0AAAAJgAAAB
 00014d40: 7341 4141 4150 4141 4141 4151 4141 4144  sAAAAPAAAAAQAAAD
 00014d50: 512f 662f 2f41 4141 4241 6841 4141 4141  Q/f//AAABAhAAAAA
 00014d60: 6741 4141 4142 4141 4141 4141 4141 4141  gAAAABAAAAAAAAAA
@@ -5381,12 +5381,12 @@
 00015040: 4941 4159 4142 7741 4d41 4141 4145 4141  IAAYABwAMAAAAEAA
 00015050: 5141 4141 4141 4141 4241 6841 4141 4141  QAAAAAAABAhAAAAA
 00015060: 6b41 4141 4142 4141 4141 4141 4141 4141  kAAAABAAAAAAAAAA
 00015070: 4a41 4141 4163 3239 3163 6d4e 6c58 326c  JAAAAc291cmNlX2l
 00015080: 6b41 4141 4143 4141 4d41 4167 4142 7741  kAAAACAAMAAgABwA
 00015090: 4941 4141 4141 4141 4141 5541 4141 4141  IAAAAAAAAAUAAAAA
 000150a0: 3d00 1820 7061 7271 7565 742d 6370 702d  =.. parquet-cpp-
-000150b0: 6172 726f 7720 7665 7273 696f 6e20 3134  arrow version 14
-000150c0: 2e30 2e31 19dc 1c00 001c 0000 1c00 001c  .0.1............
+000150b0: 6172 726f 7720 7665 7273 696f 6e20 3136  arrow version 16
+000150c0: 2e30 2e30 19dc 1c00 001c 0000 1c00 001c  .0.0............
 000150d0: 0000 1c00 001c 0000 1c00 001c 0000 1c00  ................
 000150e0: 001c 0000 1c00 001c 0000 1c00 0000 671a  ..............g.
 000150f0: 0000 5041 5231                           ..PAR1
```

### Comparing `hipscat-0.3.3/tests/data/small_sky_source/Norder=2/Dir=0/Npix=178.parquet` & `hipscat-0.3.4/tests/data/small_sky_source/Norder=2/Dir=0/Npix=178.parquet`

 * *Files 1% similar despite different names*

```diff
@@ -5562,17 +5562,17 @@
 00015b90: 2270 616e 6461 735f 7479 7065 223a 2022  "pandas_type": "
 00015ba0: 7569 6e74 3634 222c 2022 6e75 6d70 795f  uint64", "numpy_
 00015bb0: 7479 7065 223a 2022 7569 6e74 3634 222c  type": "uint64",
 00015bc0: 2022 6d65 7461 6461 7461 223a 206e 756c   "metadata": nul
 00015bd0: 6c7d 5d2c 2022 6372 6561 746f 7222 3a20  l}], "creator": 
 00015be0: 7b22 6c69 6272 6172 7922 3a20 2270 7961  {"library": "pya
 00015bf0: 7272 6f77 222c 2022 7665 7273 696f 6e22  rrow", "version"
-00015c00: 3a20 2231 342e 302e 3122 7d2c 2022 7061  : "14.0.1"}, "pa
+00015c00: 3a20 2231 362e 302e 3022 7d2c 2022 7061  : "16.0.0"}, "pa
 00015c10: 6e64 6173 5f76 6572 7369 6f6e 223a 2022  ndas_version": "
-00015c20: 322e 302e 3322 7d00 180c 4152 524f 573a  2.0.3"}...ARROW:
+00015c20: 322e 322e 3222 7d00 180c 4152 524f 573a  2.2.2"}...ARROW:
 00015c30: 7363 6865 6d61 18cc 1a2f 2f2f 2f2f 2f41  schema...//////A
 00015c40: 4a41 4141 5141 4141 4141 4141 4b41 4134  JAAAQAAAAAAAKAA4
 00015c50: 4142 6741 4641 4167 4143 6741 4141 4141  ABgAFAAgACgAAAAA
 00015c60: 4242 4141 5141 4141 4141 4141 4b41 4177  BBAAQAAAAAAAKAAw
 00015c70: 4141 4141 4541 4167 4143 6741 4141 4241  AAAAEAAgACgAAABA
 00015c80: 4841 4141 4541 4141 4141 5141 4141 4177  HAAAEAAAAAQAAAAw
 00015c90: 4141 4141 4941 4177 4142 4141 4941 4167  AAAAIAAwABAAIAAg
@@ -5717,18 +5717,18 @@
 00016540: 7564 5731 7765 5639 3065 5842 6c49 6a6f  udW1weV90eXBlIjo
 00016550: 6749 6e56 7062 6e51 324e 4349 7349 434a  gInVpbnQ2NCIsICJ
 00016560: 745a 5852 685a 4746 3059 5349 3649 4735  tZXRhZGF0YSI6IG5
 00016570: 3162 4778 3958 5377 6749 6d4e 795a 5746  1bGx9XSwgImNyZWF
 00016580: 3062 3349 694f 6942 3749 6d78 7059 6e4a  0b3IiOiB7ImxpYnJ
 00016590: 6863 6e6b 694f 6941 6963 486c 6863 6e4a  hcnkiOiAicHlhcnJ
 000165a0: 7664 7949 7349 434a 325a 584a 7a61 5739  vdyIsICJ2ZXJzaW9
-000165b0: 7549 6a6f 6749 6a45 304c 6a41 754d 534a  uIjogIjE0LjAuMSJ
+000165b0: 7549 6a6f 6749 6a45 324c 6a41 754d 434a  uIjogIjE2LjAuMCJ
 000165c0: 394c 4341 6963 4746 755a 4746 7a58 335a  9LCAicGFuZGFzX3Z
 000165d0: 6c63 6e4e 7062 3234 694f 6941 694d 6934  lcnNpb24iOiAiMi4
-000165e0: 774c 6a4d 6966 5141 4144 5141 4141 4851  wLjMifQAADQAAAHQ
+000165e0: 794c 6a49 6966 5141 4144 5141 4141 4851  yLjIifQAADQAAAHQ
 000165f0: 4341 4141 7341 6741 412b 4145 4141 4d77  CAAAsAgAA+AEAAMw
 00016600: 4241 4143 6741 5141 4163 4145 4141 4467  BAACgAQAAcAEAADg
 00016610: 4241 4141 4541 5141 4130 4141 4141 4a67  BAAAEAQAA0AAAAJg
 00016620: 4141 4142 7341 4141 4150 4141 4141 4151  AAABsAAAAPAAAAAQ
 00016630: 4141 4144 512f 662f 2f41 4141 4241 6841  AAADQ/f//AAABAhA
 00016640: 4141 4141 6741 4141 4142 4141 4141 4141  AAAAgAAAABAAAAAA
 00016650: 4141 4141 4f41 4141 4158 3268 7063 484e  AAAAOAAAAX2hpcHN
@@ -5780,11 +5780,11 @@
 00016930: 4145 4141 5141 4141 4141 4141 4241 6841  AEAAQAAAAAAABAhA
 00016940: 4141 4141 6b41 4141 4142 4141 4141 4141  AAAAkAAAABAAAAAA
 00016950: 4141 4141 4a41 4141 4163 3239 3163 6d4e  AAAAJAAAAc291cmN
 00016960: 6c58 326c 6b41 4141 4143 4141 4d41 4167  lX2lkAAAACAAMAAg
 00016970: 4142 7741 4941 4141 4141 4141 4141 5541  ABwAIAAAAAAAAAUA
 00016980: 4141 4141 3d00 1820 7061 7271 7565 742d  AAAA=.. parquet-
 00016990: 6370 702d 6172 726f 7720 7665 7273 696f  cpp-arrow versio
-000169a0: 6e20 3134 2e30 2e31 19dc 1c00 001c 0000  n 14.0.1........
+000169a0: 6e20 3136 2e30 2e30 19dc 1c00 001c 0000  n 16.0.0........
 000169b0: 1c00 001c 0000 1c00 001c 0000 1c00 001c  ................
 000169c0: 0000 1c00 001c 0000 1c00 001c 0000 1c00  ................
 000169d0: 0000 671a 0000 5041 5231                 ..g...PAR1
```

### Comparing `hipscat-0.3.3/tests/data/small_sky_source/Norder=2/Dir=0/Npix=179.parquet` & `hipscat-0.3.4/tests/data/small_sky_source/Norder=2/Dir=0/Npix=179.parquet`

 * *Files 1% similar despite different names*

```diff
@@ -6014,17 +6014,17 @@
 000177d0: 696e 6465 7822 2c20 2270 616e 6461 735f  index", "pandas_
 000177e0: 7479 7065 223a 2022 7569 6e74 3634 222c  type": "uint64",
 000177f0: 2022 6e75 6d70 795f 7479 7065 223a 2022   "numpy_type": "
 00017800: 7569 6e74 3634 222c 2022 6d65 7461 6461  uint64", "metada
 00017810: 7461 223a 206e 756c 6c7d 5d2c 2022 6372  ta": null}], "cr
 00017820: 6561 746f 7222 3a20 7b22 6c69 6272 6172  eator": {"librar
 00017830: 7922 3a20 2270 7961 7272 6f77 222c 2022  y": "pyarrow", "
-00017840: 7665 7273 696f 6e22 3a20 2231 342e 302e  version": "14.0.
-00017850: 3122 7d2c 2022 7061 6e64 6173 5f76 6572  1"}, "pandas_ver
-00017860: 7369 6f6e 223a 2022 322e 302e 3322 7d00  sion": "2.0.3"}.
+00017840: 7665 7273 696f 6e22 3a20 2231 362e 302e  version": "16.0.
+00017850: 3022 7d2c 2022 7061 6e64 6173 5f76 6572  0"}, "pandas_ver
+00017860: 7369 6f6e 223a 2022 322e 322e 3222 7d00  sion": "2.2.2"}.
 00017870: 180c 4152 524f 573a 7363 6865 6d61 18cc  ..ARROW:schema..
 00017880: 1a2f 2f2f 2f2f 2f41 4a41 4141 5141 4141  .//////AJAAAQAAA
 00017890: 4141 4141 4b41 4134 4142 6741 4641 4167  AAAAKAA4ABgAFAAg
 000178a0: 4143 6741 4141 4141 4242 4141 5141 4141  ACgAAAAABBAAQAAA
 000178b0: 4141 4141 4b41 4177 4141 4141 4541 4167  AAAAKAAwAAAAEAAg
 000178c0: 4143 6741 4141 4241 4841 4141 4541 4141  ACgAAABAHAAAEAAA
 000178d0: 4141 5141 4141 4177 4141 4141 4941 4177  AAQAAAAwAAAAIAAw
@@ -6170,17 +6170,17 @@
 00018190: 3065 5842 6c49 6a6f 6749 6e56 7062 6e51  0eXBlIjogInVpbnQ
 000181a0: 324e 4349 7349 434a 745a 5852 685a 4746  2NCIsICJtZXRhZGF
 000181b0: 3059 5349 3649 4735 3162 4778 3958 5377  0YSI6IG51bGx9XSw
 000181c0: 6749 6d4e 795a 5746 3062 3349 694f 6942  gImNyZWF0b3IiOiB
 000181d0: 3749 6d78 7059 6e4a 6863 6e6b 694f 6941  7ImxpYnJhcnkiOiA
 000181e0: 6963 486c 6863 6e4a 7664 7949 7349 434a  icHlhcnJvdyIsICJ
 000181f0: 325a 584a 7a61 5739 7549 6a6f 6749 6a45  2ZXJzaW9uIjogIjE
-00018200: 304c 6a41 754d 534a 394c 4341 6963 4746  0LjAuMSJ9LCAicGF
+00018200: 324c 6a41 754d 434a 394c 4341 6963 4746  2LjAuMCJ9LCAicGF
 00018210: 755a 4746 7a58 335a 6c63 6e4e 7062 3234  uZGFzX3ZlcnNpb24
-00018220: 694f 6941 694d 6934 774c 6a4d 6966 5141  iOiAiMi4wLjMifQA
+00018220: 694f 6941 694d 6934 794c 6a49 6966 5141  iOiAiMi4yLjIifQA
 00018230: 4144 5141 4141 4851 4341 4141 7341 6741  ADQAAAHQCAAAsAgA
 00018240: 412b 4145 4141 4d77 4241 4143 6741 5141  A+AEAAMwBAACgAQA
 00018250: 4163 4145 4141 4467 4241 4141 4541 5141  AcAEAADgBAAAEAQA
 00018260: 4130 4141 4141 4a67 4141 4142 7341 4141  A0AAAAJgAAABsAAA
 00018270: 4150 4141 4141 4151 4141 4144 512f 662f  APAAAAAQAAADQ/f/
 00018280: 2f41 4141 4241 6841 4141 4141 6741 4141  /AAABAhAAAAAgAAA
 00018290: 4142 4141 4141 4141 4141 4141 4f41 4141  ABAAAAAAAAAAOAAA
@@ -6232,12 +6232,12 @@
 00018570: 4142 7741 4d41 4141 4145 4141 5141 4141  ABwAMAAAAEAAQAAA
 00018580: 4141 4141 4241 6841 4141 4141 6b41 4141  AAAABAhAAAAAkAAA
 00018590: 4142 4141 4141 4141 4141 4141 4a41 4141  ABAAAAAAAAAAJAAA
 000185a0: 4163 3239 3163 6d4e 6c58 326c 6b41 4141  Ac291cmNlX2lkAAA
 000185b0: 4143 4141 4d41 4167 4142 7741 4941 4141  ACAAMAAgABwAIAAA
 000185c0: 4141 4141 4141 5541 4141 4141 3d00 1820  AAAAAAUAAAAA=.. 
 000185d0: 7061 7271 7565 742d 6370 702d 6172 726f  parquet-cpp-arro
-000185e0: 7720 7665 7273 696f 6e20 3134 2e30 2e31  w version 14.0.1
+000185e0: 7720 7665 7273 696f 6e20 3136 2e30 2e30  w version 16.0.0
 000185f0: 19dc 1c00 001c 0000 1c00 001c 0000 1c00  ................
 00018600: 001c 0000 1c00 001c 0000 1c00 001c 0000  ................
 00018610: 1c00 001c 0000 1c00 0000 671a 0000 5041  ..........g...PA
 00018620: 5231                                     R1
```

### Comparing `hipscat-0.3.3/tests/data/small_sky_source/Norder=2/Dir=0/Npix=180.parquet` & `hipscat-0.3.4/tests/data/small_sky_source/Norder=2/Dir=0/Npix=180.parquet`

 * *Files 2% similar despite different names*

```diff
@@ -2408,17 +2408,17 @@
 00009670: 6e64 6578 222c 2022 7061 6e64 6173 5f74  ndex", "pandas_t
 00009680: 7970 6522 3a20 2275 696e 7436 3422 2c20  ype": "uint64", 
 00009690: 226e 756d 7079 5f74 7970 6522 3a20 2275  "numpy_type": "u
 000096a0: 696e 7436 3422 2c20 226d 6574 6164 6174  int64", "metadat
 000096b0: 6122 3a20 6e75 6c6c 7d5d 2c20 2263 7265  a": null}], "cre
 000096c0: 6174 6f72 223a 207b 226c 6962 7261 7279  ator": {"library
 000096d0: 223a 2022 7079 6172 726f 7722 2c20 2276  ": "pyarrow", "v
-000096e0: 6572 7369 6f6e 223a 2022 3134 2e30 2e31  ersion": "14.0.1
+000096e0: 6572 7369 6f6e 223a 2022 3136 2e30 2e30  ersion": "16.0.0
 000096f0: 227d 2c20 2270 616e 6461 735f 7665 7273  "}, "pandas_vers
-00009700: 696f 6e22 3a20 2232 2e30 2e33 227d 0018  ion": "2.0.3"}..
+00009700: 696f 6e22 3a20 2232 2e32 2e32 227d 0018  ion": "2.2.2"}..
 00009710: 0c41 5252 4f57 3a73 6368 656d 6118 cc1a  .ARROW:schema...
 00009720: 2f2f 2f2f 2f2f 414a 4141 4151 4141 4141  //////AJAAAQAAAA
 00009730: 4141 414b 4141 3441 4267 4146 4141 6741  AAAKAA4ABgAFAAgA
 00009740: 4367 4141 4141 4142 4241 4151 4141 4141  CgAAAAABBAAQAAAA
 00009750: 4141 414b 4141 7741 4141 4145 4141 6741  AAAKAAwAAAAEAAgA
 00009760: 4367 4141 4142 4148 4141 4145 4141 4141  CgAAABAHAAAEAAAA
 00009770: 4151 4141 4141 7741 4141 4149 4141 7741  AQAAAAwAAAAIAAwA
@@ -2563,18 +2563,18 @@
 0000a020: 4e43 4973 4943 4a75 6457 3177 6556 3930  NCIsICJudW1weV90
 0000a030: 6558 426c 496a 6f67 496e 5670 626e 5132  eXBlIjogInVpbnQ2
 0000a040: 4e43 4973 4943 4a74 5a58 5268 5a47 4630  NCIsICJtZXRhZGF0
 0000a050: 5953 4936 4947 3531 6247 7839 5853 7767  YSI6IG51bGx9XSwg
 0000a060: 496d 4e79 5a57 4630 6233 4969 4f69 4237  ImNyZWF0b3IiOiB7
 0000a070: 496d 7870 596e 4a68 636e 6b69 4f69 4169  ImxpYnJhcnkiOiAi
 0000a080: 6348 6c68 636e 4a76 6479 4973 4943 4a32  cHlhcnJvdyIsICJ2
-0000a090: 5a58 4a7a 6157 3975 496a 6f67 496a 4530  ZXJzaW9uIjogIjE0
-0000a0a0: 4c6a 4175 4d53 4a39 4c43 4169 6347 4675  LjAuMSJ9LCAicGFu
+0000a090: 5a58 4a7a 6157 3975 496a 6f67 496a 4532  ZXJzaW9uIjogIjE2
+0000a0a0: 4c6a 4175 4d43 4a39 4c43 4169 6347 4675  LjAuMCJ9LCAicGFu
 0000a0b0: 5a47 467a 5833 5a6c 636e 4e70 6232 3469  ZGFzX3ZlcnNpb24i
-0000a0c0: 4f69 4169 4d69 3477 4c6a 4d69 6651 4141  OiAiMi4wLjMifQAA
+0000a0c0: 4f69 4169 4d69 3479 4c6a 4969 6651 4141  OiAiMi4yLjIifQAA
 0000a0d0: 4451 4141 4148 5143 4141 4173 4167 4141  DQAAAHQCAAAsAgAA
 0000a0e0: 2b41 4541 414d 7742 4141 4367 4151 4141  +AEAAMwBAACgAQAA
 0000a0f0: 6341 4541 4144 6742 4141 4145 4151 4141  cAEAADgBAAAEAQAA
 0000a100: 3041 4141 414a 6741 4141 4273 4141 4141  0AAAAJgAAABsAAAA
 0000a110: 5041 4141 4141 5141 4141 4451 2f66 2f2f  PAAAAAQAAADQ/f//
 0000a120: 4141 4142 4168 4141 4141 4167 4141 4141  AAABAhAAAAAgAAAA
 0000a130: 4241 4141 4141 4141 4141 414f 4141 4141  BAAAAAAAAAAOAAAA
@@ -2626,12 +2626,12 @@
 0000a410: 4277 414d 4141 4141 4541 4151 4141 4141  BwAMAAAAEAAQAAAA
 0000a420: 4141 4142 4168 4141 4141 416b 4141 4141  AAABAhAAAAAkAAAA
 0000a430: 4241 4141 4141 4141 4141 414a 4141 4141  BAAAAAAAAAAJAAAA
 0000a440: 6332 3931 636d 4e6c 5832 6c6b 4141 4141  c291cmNlX2lkAAAA
 0000a450: 4341 414d 4141 6741 4277 4149 4141 4141  CAAMAAgABwAIAAAA
 0000a460: 4141 4141 4155 4141 4141 413d 0018 2070  AAAAAUAAAAA=.. p
 0000a470: 6172 7175 6574 2d63 7070 2d61 7272 6f77  arquet-cpp-arrow
-0000a480: 2076 6572 7369 6f6e 2031 342e 302e 3119   version 14.0.1.
+0000a480: 2076 6572 7369 6f6e 2031 362e 302e 3019   version 16.0.0.
 0000a490: dc1c 0000 1c00 001c 0000 1c00 001c 0000  ................
 0000a4a0: 1c00 001c 0000 1c00 001c 0000 1c00 001c  ................
 0000a4b0: 0000 1c00 001c 0000 0059 1a00 0050 4152  .........Y...PAR
 0000a4c0: 31                                       1
```

### Comparing `hipscat-0.3.3/tests/data/small_sky_source/Norder=2/Dir=0/Npix=181.parquet` & `hipscat-0.3.4/tests/data/small_sky_source/Norder=2/Dir=0/Npix=181.parquet`

 * *Files 1% similar despite different names*

```diff
@@ -3194,17 +3194,17 @@
 0000c790: 6461 735f 7479 7065 223a 2022 7569 6e74  das_type": "uint
 0000c7a0: 3634 222c 2022 6e75 6d70 795f 7479 7065  64", "numpy_type
 0000c7b0: 223a 2022 7569 6e74 3634 222c 2022 6d65  ": "uint64", "me
 0000c7c0: 7461 6461 7461 223a 206e 756c 6c7d 5d2c  tadata": null}],
 0000c7d0: 2022 6372 6561 746f 7222 3a20 7b22 6c69   "creator": {"li
 0000c7e0: 6272 6172 7922 3a20 2270 7961 7272 6f77  brary": "pyarrow
 0000c7f0: 222c 2022 7665 7273 696f 6e22 3a20 2231  ", "version": "1
-0000c800: 342e 302e 3122 7d2c 2022 7061 6e64 6173  4.0.1"}, "pandas
-0000c810: 5f76 6572 7369 6f6e 223a 2022 322e 302e  _version": "2.0.
-0000c820: 3322 7d00 180c 4152 524f 573a 7363 6865  3"}...ARROW:sche
+0000c800: 362e 302e 3022 7d2c 2022 7061 6e64 6173  6.0.0"}, "pandas
+0000c810: 5f76 6572 7369 6f6e 223a 2022 322e 322e  _version": "2.2.
+0000c820: 3222 7d00 180c 4152 524f 573a 7363 6865  2"}...ARROW:sche
 0000c830: 6d61 18cc 1a2f 2f2f 2f2f 2f41 4a41 4141  ma...//////AJAAA
 0000c840: 5141 4141 4141 4141 4b41 4134 4142 6741  QAAAAAAAKAA4ABgA
 0000c850: 4641 4167 4143 6741 4141 4141 4242 4141  FAAgACgAAAAABBAA
 0000c860: 5141 4141 4141 4141 4b41 4177 4141 4141  QAAAAAAAKAAwAAAA
 0000c870: 4541 4167 4143 6741 4141 4241 4841 4141  EAAgACgAAABAHAAA
 0000c880: 4541 4141 4141 5141 4141 4177 4141 4141  EAAAAAQAAAAwAAAA
 0000c890: 4941 4177 4142 4141 4941 4167 4141 4141  IAAwABAAIAAgAAAA
@@ -3349,17 +3349,17 @@
 0000d140: 7765 5639 3065 5842 6c49 6a6f 6749 6e56  weV90eXBlIjogInV
 0000d150: 7062 6e51 324e 4349 7349 434a 745a 5852  pbnQ2NCIsICJtZXR
 0000d160: 685a 4746 3059 5349 3649 4735 3162 4778  hZGF0YSI6IG51bGx
 0000d170: 3958 5377 6749 6d4e 795a 5746 3062 3349  9XSwgImNyZWF0b3I
 0000d180: 694f 6942 3749 6d78 7059 6e4a 6863 6e6b  iOiB7ImxpYnJhcnk
 0000d190: 694f 6941 6963 486c 6863 6e4a 7664 7949  iOiAicHlhcnJvdyI
 0000d1a0: 7349 434a 325a 584a 7a61 5739 7549 6a6f  sICJ2ZXJzaW9uIjo
-0000d1b0: 6749 6a45 304c 6a41 754d 534a 394c 4341  gIjE0LjAuMSJ9LCA
+0000d1b0: 6749 6a45 324c 6a41 754d 434a 394c 4341  gIjE2LjAuMCJ9LCA
 0000d1c0: 6963 4746 755a 4746 7a58 335a 6c63 6e4e  icGFuZGFzX3ZlcnN
-0000d1d0: 7062 3234 694f 6941 694d 6934 774c 6a4d  pb24iOiAiMi4wLjM
+0000d1d0: 7062 3234 694f 6941 694d 6934 794c 6a49  pb24iOiAiMi4yLjI
 0000d1e0: 6966 5141 4144 5141 4141 4851 4341 4141  ifQAADQAAAHQCAAA
 0000d1f0: 7341 6741 412b 4145 4141 4d77 4241 4143  sAgAA+AEAAMwBAAC
 0000d200: 6741 5141 4163 4145 4141 4467 4241 4141  gAQAAcAEAADgBAAA
 0000d210: 4541 5141 4130 4141 4141 4a67 4141 4142  EAQAA0AAAAJgAAAB
 0000d220: 7341 4141 4150 4141 4141 4151 4141 4144  sAAAAPAAAAAQAAAD
 0000d230: 512f 662f 2f41 4141 4241 6841 4141 4141  Q/f//AAABAhAAAAA
 0000d240: 6741 4141 4142 4141 4141 4141 4141 4141  gAAAABAAAAAAAAAA
@@ -3411,12 +3411,12 @@
 0000d520: 4941 4159 4142 7741 4d41 4141 4145 4141  IAAYABwAMAAAAEAA
 0000d530: 5141 4141 4141 4141 4241 6841 4141 4141  QAAAAAAABAhAAAAA
 0000d540: 6b41 4141 4142 4141 4141 4141 4141 4141  kAAAABAAAAAAAAAA
 0000d550: 4a41 4141 4163 3239 3163 6d4e 6c58 326c  JAAAAc291cmNlX2l
 0000d560: 6b41 4141 4143 4141 4d41 4167 4142 7741  kAAAACAAMAAgABwA
 0000d570: 4941 4141 4141 4141 4141 5541 4141 4141  IAAAAAAAAAUAAAAA
 0000d580: 3d00 1820 7061 7271 7565 742d 6370 702d  =.. parquet-cpp-
-0000d590: 6172 726f 7720 7665 7273 696f 6e20 3134  arrow version 14
-0000d5a0: 2e30 2e31 19dc 1c00 001c 0000 1c00 001c  .0.1............
+0000d590: 6172 726f 7720 7665 7273 696f 6e20 3136  arrow version 16
+0000d5a0: 2e30 2e30 19dc 1c00 001c 0000 1c00 001c  .0.0............
 0000d5b0: 0000 1c00 001c 0000 1c00 001c 0000 1c00  ................
 0000d5c0: 001c 0000 1c00 001c 0000 1c00 0000 631a  ..............c.
 0000d5d0: 0000 5041 5231                           ..PAR1
```

### Comparing `hipscat-0.3.3/tests/data/small_sky_source/Norder=2/Dir=0/Npix=182.parquet` & `hipscat-0.3.4/tests/data/small_sky_source/Norder=2/Dir=0/Npix=182.parquet`

 * *Files 0% similar despite different names*

```diff
@@ -4332,17 +4332,17 @@
 00010eb0: 6465 7822 2c20 2270 616e 6461 735f 7479  dex", "pandas_ty
 00010ec0: 7065 223a 2022 7569 6e74 3634 222c 2022  pe": "uint64", "
 00010ed0: 6e75 6d70 795f 7479 7065 223a 2022 7569  numpy_type": "ui
 00010ee0: 6e74 3634 222c 2022 6d65 7461 6461 7461  nt64", "metadata
 00010ef0: 223a 206e 756c 6c7d 5d2c 2022 6372 6561  ": null}], "crea
 00010f00: 746f 7222 3a20 7b22 6c69 6272 6172 7922  tor": {"library"
 00010f10: 3a20 2270 7961 7272 6f77 222c 2022 7665  : "pyarrow", "ve
-00010f20: 7273 696f 6e22 3a20 2231 342e 302e 3122  rsion": "14.0.1"
+00010f20: 7273 696f 6e22 3a20 2231 362e 302e 3022  rsion": "16.0.0"
 00010f30: 7d2c 2022 7061 6e64 6173 5f76 6572 7369  }, "pandas_versi
-00010f40: 6f6e 223a 2022 322e 302e 3322 7d00 180c  on": "2.0.3"}...
+00010f40: 6f6e 223a 2022 322e 322e 3222 7d00 180c  on": "2.2.2"}...
 00010f50: 4152 524f 573a 7363 6865 6d61 18cc 1a2f  ARROW:schema.../
 00010f60: 2f2f 2f2f 2f41 4a41 4141 5141 4141 4141  /////AJAAAQAAAAA
 00010f70: 4141 4b41 4134 4142 6741 4641 4167 4143  AAKAA4ABgAFAAgAC
 00010f80: 6741 4141 4141 4242 4141 5141 4141 4141  gAAAAABBAAQAAAAA
 00010f90: 4141 4b41 4177 4141 4141 4541 4167 4143  AAKAAwAAAAEAAgAC
 00010fa0: 6741 4141 4241 4841 4141 4541 4141 4141  gAAABAHAAAEAAAAA
 00010fb0: 5141 4141 4177 4141 4141 4941 4177 4142  QAAAAwAAAAIAAwAB
@@ -4487,18 +4487,18 @@
 00011860: 4349 7349 434a 7564 5731 7765 5639 3065  CIsICJudW1weV90e
 00011870: 5842 6c49 6a6f 6749 6e56 7062 6e51 324e  XBlIjogInVpbnQ2N
 00011880: 4349 7349 434a 745a 5852 685a 4746 3059  CIsICJtZXRhZGF0Y
 00011890: 5349 3649 4735 3162 4778 3958 5377 6749  SI6IG51bGx9XSwgI
 000118a0: 6d4e 795a 5746 3062 3349 694f 6942 3749  mNyZWF0b3IiOiB7I
 000118b0: 6d78 7059 6e4a 6863 6e6b 694f 6941 6963  mxpYnJhcnkiOiAic
 000118c0: 486c 6863 6e4a 7664 7949 7349 434a 325a  HlhcnJvdyIsICJ2Z
-000118d0: 584a 7a61 5739 7549 6a6f 6749 6a45 304c  XJzaW9uIjogIjE0L
-000118e0: 6a41 754d 534a 394c 4341 6963 4746 755a  jAuMSJ9LCAicGFuZ
+000118d0: 584a 7a61 5739 7549 6a6f 6749 6a45 324c  XJzaW9uIjogIjE2L
+000118e0: 6a41 754d 434a 394c 4341 6963 4746 755a  jAuMCJ9LCAicGFuZ
 000118f0: 4746 7a58 335a 6c63 6e4e 7062 3234 694f  GFzX3ZlcnNpb24iO
-00011900: 6941 694d 6934 774c 6a4d 6966 5141 4144  iAiMi4wLjMifQAAD
+00011900: 6941 694d 6934 794c 6a49 6966 5141 4144  iAiMi4yLjIifQAAD
 00011910: 5141 4141 4851 4341 4141 7341 6741 412b  QAAAHQCAAAsAgAA+
 00011920: 4145 4141 4d77 4241 4143 6741 5141 4163  AEAAMwBAACgAQAAc
 00011930: 4145 4141 4467 4241 4141 4541 5141 4130  AEAADgBAAAEAQAA0
 00011940: 4141 4141 4a67 4141 4142 7341 4141 4150  AAAAJgAAABsAAAAP
 00011950: 4141 4141 4151 4141 4144 512f 662f 2f41  AAAAAQAAADQ/f//A
 00011960: 4141 4241 6841 4141 4141 6741 4141 4142  AABAhAAAAAgAAAAB
 00011970: 4141 4141 4141 4141 4141 4f41 4141 4158  AAAAAAAAAAOAAAAX
@@ -4550,11 +4550,11 @@
 00011c50: 7741 4d41 4141 4145 4141 5141 4141 4141  wAMAAAAEAAQAAAAA
 00011c60: 4141 4241 6841 4141 4141 6b41 4141 4142  AABAhAAAAAkAAAAB
 00011c70: 4141 4141 4141 4141 4141 4a41 4141 4163  AAAAAAAAAAJAAAAc
 00011c80: 3239 3163 6d4e 6c58 326c 6b41 4141 4143  291cmNlX2lkAAAAC
 00011c90: 4141 4d41 4167 4142 7741 4941 4141 4141  AAMAAgABwAIAAAAA
 00011ca0: 4141 4141 5541 4141 4141 3d00 1820 7061  AAAAUAAAAA=.. pa
 00011cb0: 7271 7565 742d 6370 702d 6172 726f 7720  rquet-cpp-arrow 
-00011cc0: 7665 7273 696f 6e20 3134 2e30 2e31 19dc  version 14.0.1..
+00011cc0: 7665 7273 696f 6e20 3136 2e30 2e30 19dc  version 16.0.0..
 00011cd0: 1c00 001c 0000 1c00 001c 0000 1c00 001c  ................
 00011ce0: 0000 1c00 001c 0000 1c00 001c 0000 1c00  ................
 00011cf0: 001c 0000 1c00 0000 641a 0000 5041 5231  ........d...PAR1
```

### Comparing `hipscat-0.3.3/tests/data/small_sky_source/Norder=2/Dir=0/Npix=183.parquet` & `hipscat-0.3.4/tests/data/small_sky_source/Norder=2/Dir=0/Npix=183.parquet`

 * *Files 1% similar despite different names*

```diff
@@ -4008,17 +4008,17 @@
 0000fa70: 2022 7061 6e64 6173 5f74 7970 6522 3a20   "pandas_type": 
 0000fa80: 2275 696e 7436 3422 2c20 226e 756d 7079  "uint64", "numpy
 0000fa90: 5f74 7970 6522 3a20 2275 696e 7436 3422  _type": "uint64"
 0000faa0: 2c20 226d 6574 6164 6174 6122 3a20 6e75  , "metadata": nu
 0000fab0: 6c6c 7d5d 2c20 2263 7265 6174 6f72 223a  ll}], "creator":
 0000fac0: 207b 226c 6962 7261 7279 223a 2022 7079   {"library": "py
 0000fad0: 6172 726f 7722 2c20 2276 6572 7369 6f6e  arrow", "version
-0000fae0: 223a 2022 3134 2e30 2e31 227d 2c20 2270  ": "14.0.1"}, "p
+0000fae0: 223a 2022 3136 2e30 2e30 227d 2c20 2270  ": "16.0.0"}, "p
 0000faf0: 616e 6461 735f 7665 7273 696f 6e22 3a20  andas_version": 
-0000fb00: 2232 2e30 2e33 227d 0018 0c41 5252 4f57  "2.0.3"}...ARROW
+0000fb00: 2232 2e32 2e32 227d 0018 0c41 5252 4f57  "2.2.2"}...ARROW
 0000fb10: 3a73 6368 656d 6118 cc1a 2f2f 2f2f 2f2f  :schema...//////
 0000fb20: 414a 4141 4151 4141 4141 4141 414b 4141  AJAAAQAAAAAAAKAA
 0000fb30: 3441 4267 4146 4141 6741 4367 4141 4141  4ABgAFAAgACgAAAA
 0000fb40: 4142 4241 4151 4141 4141 4141 414b 4141  ABBAAQAAAAAAAKAA
 0000fb50: 7741 4141 4145 4141 6741 4367 4141 4142  wAAAAEAAgACgAAAB
 0000fb60: 4148 4141 4145 4141 4141 4151 4141 4141  AHAAAEAAAAAQAAAA
 0000fb70: 7741 4141 4149 4141 7741 4241 4149 4141  wAAAAIAAwABAAIAA
@@ -4163,18 +4163,18 @@
 00010420: 4a75 6457 3177 6556 3930 6558 426c 496a  JudW1weV90eXBlIj
 00010430: 6f67 496e 5670 626e 5132 4e43 4973 4943  ogInVpbnQ2NCIsIC
 00010440: 4a74 5a58 5268 5a47 4630 5953 4936 4947  JtZXRhZGF0YSI6IG
 00010450: 3531 6247 7839 5853 7767 496d 4e79 5a57  51bGx9XSwgImNyZW
 00010460: 4630 6233 4969 4f69 4237 496d 7870 596e  F0b3IiOiB7ImxpYn
 00010470: 4a68 636e 6b69 4f69 4169 6348 6c68 636e  JhcnkiOiAicHlhcn
 00010480: 4a76 6479 4973 4943 4a32 5a58 4a7a 6157  JvdyIsICJ2ZXJzaW
-00010490: 3975 496a 6f67 496a 4530 4c6a 4175 4d53  9uIjogIjE0LjAuMS
+00010490: 3975 496a 6f67 496a 4532 4c6a 4175 4d43  9uIjogIjE2LjAuMC
 000104a0: 4a39 4c43 4169 6347 4675 5a47 467a 5833  J9LCAicGFuZGFzX3
 000104b0: 5a6c 636e 4e70 6232 3469 4f69 4169 4d69  ZlcnNpb24iOiAiMi
-000104c0: 3477 4c6a 4d69 6651 4141 4451 4141 4148  4wLjMifQAADQAAAH
+000104c0: 3479 4c6a 4969 6651 4141 4451 4141 4148  4yLjIifQAADQAAAH
 000104d0: 5143 4141 4173 4167 4141 2b41 4541 414d  QCAAAsAgAA+AEAAM
 000104e0: 7742 4141 4367 4151 4141 6341 4541 4144  wBAACgAQAAcAEAAD
 000104f0: 6742 4141 4145 4151 4141 3041 4141 414a  gBAAAEAQAA0AAAAJ
 00010500: 6741 4141 4273 4141 4141 5041 4141 4141  gAAABsAAAAPAAAAA
 00010510: 5141 4141 4451 2f66 2f2f 4141 4142 4168  QAAADQ/f//AAABAh
 00010520: 4141 4141 4167 4141 4141 4241 4141 4141  AAAAAgAAAABAAAAA
 00010530: 4141 4141 414f 4141 4141 5832 6870 6348  AAAAAOAAAAX2hpcH
@@ -4226,11 +4226,11 @@
 00010810: 4141 4541 4151 4141 4141 4141 4142 4168  AAEAAQAAAAAAABAh
 00010820: 4141 4141 416b 4141 4141 4241 4141 4141  AAAAAkAAAABAAAAA
 00010830: 4141 4141 414a 4141 4141 6332 3931 636d  AAAAAJAAAAc291cm
 00010840: 4e6c 5832 6c6b 4141 4141 4341 414d 4141  NlX2lkAAAACAAMAA
 00010850: 6741 4277 4149 4141 4141 4141 4141 4155  gABwAIAAAAAAAAAU
 00010860: 4141 4141 413d 0018 2070 6172 7175 6574  AAAAA=.. parquet
 00010870: 2d63 7070 2d61 7272 6f77 2076 6572 7369  -cpp-arrow versi
-00010880: 6f6e 2031 342e 302e 3119 dc1c 0000 1c00  on 14.0.1.......
+00010880: 6f6e 2031 362e 302e 3019 dc1c 0000 1c00  on 16.0.0.......
 00010890: 001c 0000 1c00 001c 0000 1c00 001c 0000  ................
 000108a0: 1c00 001c 0000 1c00 001c 0000 1c00 001c  ................
 000108b0: 0000 0064 1a00 0050 4152 31              ...d...PAR1
```

### Comparing `hipscat-0.3.3/tests/data/small_sky_source/Norder=2/Dir=0/Npix=184.parquet` & `hipscat-0.3.4/tests/data/small_sky_source/Norder=2/Dir=0/Npix=184.parquet`

 * *Files 0% similar despite different names*

```diff
@@ -4789,17 +4789,17 @@
 00012b40: 7061 6e64 6173 5f74 7970 6522 3a20 2275  pandas_type": "u
 00012b50: 696e 7436 3422 2c20 226e 756d 7079 5f74  int64", "numpy_t
 00012b60: 7970 6522 3a20 2275 696e 7436 3422 2c20  ype": "uint64", 
 00012b70: 226d 6574 6164 6174 6122 3a20 6e75 6c6c  "metadata": null
 00012b80: 7d5d 2c20 2263 7265 6174 6f72 223a 207b  }], "creator": {
 00012b90: 226c 6962 7261 7279 223a 2022 7079 6172  "library": "pyar
 00012ba0: 726f 7722 2c20 2276 6572 7369 6f6e 223a  row", "version":
-00012bb0: 2022 3134 2e30 2e31 227d 2c20 2270 616e   "14.0.1"}, "pan
+00012bb0: 2022 3136 2e30 2e30 227d 2c20 2270 616e   "16.0.0"}, "pan
 00012bc0: 6461 735f 7665 7273 696f 6e22 3a20 2232  das_version": "2
-00012bd0: 2e30 2e33 227d 0018 0c41 5252 4f57 3a73  .0.3"}...ARROW:s
+00012bd0: 2e32 2e32 227d 0018 0c41 5252 4f57 3a73  .2.2"}...ARROW:s
 00012be0: 6368 656d 6118 cc1a 2f2f 2f2f 2f2f 414a  chema...//////AJ
 00012bf0: 4141 4151 4141 4141 4141 414b 4141 3441  AAAQAAAAAAAKAA4A
 00012c00: 4267 4146 4141 6741 4367 4141 4141 4142  BgAFAAgACgAAAAAB
 00012c10: 4241 4151 4141 4141 4141 414b 4141 7741  BAAQAAAAAAAKAAwA
 00012c20: 4141 4145 4141 6741 4367 4141 4142 4148  AAAEAAgACgAAABAH
 00012c30: 4141 4145 4141 4141 4151 4141 4141 7741  AAAEAAAAAQAAAAwA
 00012c40: 4141 4149 4141 7741 4241 4149 4141 6741  AAAIAAwABAAIAAgA
@@ -4944,18 +4944,18 @@
 000134f0: 6457 3177 6556 3930 6558 426c 496a 6f67  dW1weV90eXBlIjog
 00013500: 496e 5670 626e 5132 4e43 4973 4943 4a74  InVpbnQ2NCIsICJt
 00013510: 5a58 5268 5a47 4630 5953 4936 4947 3531  ZXRhZGF0YSI6IG51
 00013520: 6247 7839 5853 7767 496d 4e79 5a57 4630  bGx9XSwgImNyZWF0
 00013530: 6233 4969 4f69 4237 496d 7870 596e 4a68  b3IiOiB7ImxpYnJh
 00013540: 636e 6b69 4f69 4169 6348 6c68 636e 4a76  cnkiOiAicHlhcnJv
 00013550: 6479 4973 4943 4a32 5a58 4a7a 6157 3975  dyIsICJ2ZXJzaW9u
-00013560: 496a 6f67 496a 4530 4c6a 4175 4d53 4a39  IjogIjE0LjAuMSJ9
+00013560: 496a 6f67 496a 4532 4c6a 4175 4d43 4a39  IjogIjE2LjAuMCJ9
 00013570: 4c43 4169 6347 4675 5a47 467a 5833 5a6c  LCAicGFuZGFzX3Zl
-00013580: 636e 4e70 6232 3469 4f69 4169 4d69 3477  cnNpb24iOiAiMi4w
-00013590: 4c6a 4d69 6651 4141 4451 4141 4148 5143  LjMifQAADQAAAHQC
+00013580: 636e 4e70 6232 3469 4f69 4169 4d69 3479  cnNpb24iOiAiMi4y
+00013590: 4c6a 4969 6651 4141 4451 4141 4148 5143  LjIifQAADQAAAHQC
 000135a0: 4141 4173 4167 4141 2b41 4541 414d 7742  AAAsAgAA+AEAAMwB
 000135b0: 4141 4367 4151 4141 6341 4541 4144 6742  AACgAQAAcAEAADgB
 000135c0: 4141 4145 4151 4141 3041 4141 414a 6741  AAAEAQAA0AAAAJgA
 000135d0: 4141 4273 4141 4141 5041 4141 4141 5141  AABsAAAAPAAAAAQA
 000135e0: 4141 4451 2f66 2f2f 4141 4142 4168 4141  AADQ/f//AAABAhAA
 000135f0: 4141 4167 4141 4141 4241 4141 4141 4141  AAAgAAAABAAAAAAA
 00013600: 4141 414f 4141 4141 5832 6870 6348 4e6a  AAAOAAAAX2hpcHNj
@@ -5007,11 +5007,11 @@
 000138e0: 4541 4151 4141 4141 4141 4142 4168 4141  EAAQAAAAAAABAhAA
 000138f0: 4141 416b 4141 4141 4241 4141 4141 4141  AAAkAAAABAAAAAAA
 00013900: 4141 414a 4141 4141 6332 3931 636d 4e6c  AAAJAAAAc291cmNl
 00013910: 5832 6c6b 4141 4141 4341 414d 4141 6741  X2lkAAAACAAMAAgA
 00013920: 4277 4149 4141 4141 4141 4141 4155 4141  BwAIAAAAAAAAAUAA
 00013930: 4141 413d 0018 2070 6172 7175 6574 2d63  AAA=.. parquet-c
 00013940: 7070 2d61 7272 6f77 2076 6572 7369 6f6e  pp-arrow version
-00013950: 2031 342e 302e 3119 dc1c 0000 1c00 001c   14.0.1.........
+00013950: 2031 362e 302e 3019 dc1c 0000 1c00 001c   16.0.0.........
 00013960: 0000 1c00 001c 0000 1c00 001c 0000 1c00  ................
 00013970: 001c 0000 1c00 001c 0000 1c00 001c 0000  ................
 00013980: 0064 1a00 0050 4152 31                   .d...PAR1
```

### Comparing `hipscat-0.3.3/tests/data/small_sky_source/Norder=2/Dir=0/Npix=185.parquet` & `hipscat-0.3.4/tests/data/small_sky_source/Norder=2/Dir=0/Npix=185.parquet`

 * *Files 0% similar despite different names*

```diff
@@ -9901,17 +9901,17 @@
 00026ac0: 6465 7822 2c20 2270 616e 6461 735f 7479  dex", "pandas_ty
 00026ad0: 7065 223a 2022 7569 6e74 3634 222c 2022  pe": "uint64", "
 00026ae0: 6e75 6d70 795f 7479 7065 223a 2022 7569  numpy_type": "ui
 00026af0: 6e74 3634 222c 2022 6d65 7461 6461 7461  nt64", "metadata
 00026b00: 223a 206e 756c 6c7d 5d2c 2022 6372 6561  ": null}], "crea
 00026b10: 746f 7222 3a20 7b22 6c69 6272 6172 7922  tor": {"library"
 00026b20: 3a20 2270 7961 7272 6f77 222c 2022 7665  : "pyarrow", "ve
-00026b30: 7273 696f 6e22 3a20 2231 342e 302e 3122  rsion": "14.0.1"
+00026b30: 7273 696f 6e22 3a20 2231 362e 302e 3022  rsion": "16.0.0"
 00026b40: 7d2c 2022 7061 6e64 6173 5f76 6572 7369  }, "pandas_versi
-00026b50: 6f6e 223a 2022 322e 302e 3322 7d00 180c  on": "2.0.3"}...
+00026b50: 6f6e 223a 2022 322e 322e 3222 7d00 180c  on": "2.2.2"}...
 00026b60: 4152 524f 573a 7363 6865 6d61 18cc 1a2f  ARROW:schema.../
 00026b70: 2f2f 2f2f 2f41 4a41 4141 5141 4141 4141  /////AJAAAQAAAAA
 00026b80: 4141 4b41 4134 4142 6741 4641 4167 4143  AAKAA4ABgAFAAgAC
 00026b90: 6741 4141 4141 4242 4141 5141 4141 4141  gAAAAABBAAQAAAAA
 00026ba0: 4141 4b41 4177 4141 4141 4541 4167 4143  AAKAAwAAAAEAAgAC
 00026bb0: 6741 4141 4241 4841 4141 4541 4141 4141  gAAABAHAAAEAAAAA
 00026bc0: 5141 4141 4177 4141 4141 4941 4177 4142  QAAAAwAAAAIAAwAB
@@ -10056,18 +10056,18 @@
 00027470: 4349 7349 434a 7564 5731 7765 5639 3065  CIsICJudW1weV90e
 00027480: 5842 6c49 6a6f 6749 6e56 7062 6e51 324e  XBlIjogInVpbnQ2N
 00027490: 4349 7349 434a 745a 5852 685a 4746 3059  CIsICJtZXRhZGF0Y
 000274a0: 5349 3649 4735 3162 4778 3958 5377 6749  SI6IG51bGx9XSwgI
 000274b0: 6d4e 795a 5746 3062 3349 694f 6942 3749  mNyZWF0b3IiOiB7I
 000274c0: 6d78 7059 6e4a 6863 6e6b 694f 6941 6963  mxpYnJhcnkiOiAic
 000274d0: 486c 6863 6e4a 7664 7949 7349 434a 325a  HlhcnJvdyIsICJ2Z
-000274e0: 584a 7a61 5739 7549 6a6f 6749 6a45 304c  XJzaW9uIjogIjE0L
-000274f0: 6a41 754d 534a 394c 4341 6963 4746 755a  jAuMSJ9LCAicGFuZ
+000274e0: 584a 7a61 5739 7549 6a6f 6749 6a45 324c  XJzaW9uIjogIjE2L
+000274f0: 6a41 754d 434a 394c 4341 6963 4746 755a  jAuMCJ9LCAicGFuZ
 00027500: 4746 7a58 335a 6c63 6e4e 7062 3234 694f  GFzX3ZlcnNpb24iO
-00027510: 6941 694d 6934 774c 6a4d 6966 5141 4144  iAiMi4wLjMifQAAD
+00027510: 6941 694d 6934 794c 6a49 6966 5141 4144  iAiMi4yLjIifQAAD
 00027520: 5141 4141 4851 4341 4141 7341 6741 412b  QAAAHQCAAAsAgAA+
 00027530: 4145 4141 4d77 4241 4143 6741 5141 4163  AEAAMwBAACgAQAAc
 00027540: 4145 4141 4467 4241 4141 4541 5141 4130  AEAADgBAAAEAQAA0
 00027550: 4141 4141 4a67 4141 4142 7341 4141 4150  AAAAJgAAABsAAAAP
 00027560: 4141 4141 4151 4141 4144 512f 662f 2f41  AAAAAQAAADQ/f//A
 00027570: 4141 4241 6841 4141 4141 6741 4141 4142  AABAhAAAAAgAAAAB
 00027580: 4141 4141 4141 4141 4141 4f41 4141 4158  AAAAAAAAAAOAAAAX
@@ -10119,11 +10119,11 @@
 00027860: 7741 4d41 4141 4145 4141 5141 4141 4141  wAMAAAAEAAQAAAAA
 00027870: 4141 4241 6841 4141 4141 6b41 4141 4142  AABAhAAAAAkAAAAB
 00027880: 4141 4141 4141 4141 4141 4a41 4141 4163  AAAAAAAAAAJAAAAc
 00027890: 3239 3163 6d4e 6c58 326c 6b41 4141 4143  291cmNlX2lkAAAAC
 000278a0: 4141 4d41 4167 4142 7741 4941 4141 4141  AAMAAgABwAIAAAAA
 000278b0: 4141 4141 5541 4141 4141 3d00 1820 7061  AAAAUAAAAA=.. pa
 000278c0: 7271 7565 742d 6370 702d 6172 726f 7720  rquet-cpp-arrow 
-000278d0: 7665 7273 696f 6e20 3134 2e30 2e31 19dc  version 14.0.1..
+000278d0: 7665 7273 696f 6e20 3136 2e30 2e30 19dc  version 16.0.0..
 000278e0: 1c00 001c 0000 1c00 001c 0000 1c00 001c  ................
 000278f0: 0000 1c00 001c 0000 1c00 001c 0000 1c00  ................
 00027900: 001c 0000 1c00 0000 681a 0000 5041 5231  ........h...PAR1
```

### Comparing `hipscat-0.3.3/tests/data/small_sky_source/Norder=2/Dir=0/Npix=186.parquet` & `hipscat-0.3.4/tests/data/small_sky_source/Norder=2/Dir=0/Npix=186.parquet`

 * *Files 0% similar despite different names*

```diff
@@ -1757,17 +1757,17 @@
 00006dc0: 6e64 6578 222c 2022 7061 6e64 6173 5f74  ndex", "pandas_t
 00006dd0: 7970 6522 3a20 2275 696e 7436 3422 2c20  ype": "uint64", 
 00006de0: 226e 756d 7079 5f74 7970 6522 3a20 2275  "numpy_type": "u
 00006df0: 696e 7436 3422 2c20 226d 6574 6164 6174  int64", "metadat
 00006e00: 6122 3a20 6e75 6c6c 7d5d 2c20 2263 7265  a": null}], "cre
 00006e10: 6174 6f72 223a 207b 226c 6962 7261 7279  ator": {"library
 00006e20: 223a 2022 7079 6172 726f 7722 2c20 2276  ": "pyarrow", "v
-00006e30: 6572 7369 6f6e 223a 2022 3134 2e30 2e31  ersion": "14.0.1
+00006e30: 6572 7369 6f6e 223a 2022 3136 2e30 2e30  ersion": "16.0.0
 00006e40: 227d 2c20 2270 616e 6461 735f 7665 7273  "}, "pandas_vers
-00006e50: 696f 6e22 3a20 2232 2e30 2e33 227d 0018  ion": "2.0.3"}..
+00006e50: 696f 6e22 3a20 2232 2e32 2e32 227d 0018  ion": "2.2.2"}..
 00006e60: 0c41 5252 4f57 3a73 6368 656d 6118 cc1a  .ARROW:schema...
 00006e70: 2f2f 2f2f 2f2f 414a 4141 4151 4141 4141  //////AJAAAQAAAA
 00006e80: 4141 414b 4141 3441 4267 4146 4141 6741  AAAKAA4ABgAFAAgA
 00006e90: 4367 4141 4141 4142 4241 4151 4141 4141  CgAAAAABBAAQAAAA
 00006ea0: 4141 414b 4141 7741 4141 4145 4141 6741  AAAKAAwAAAAEAAgA
 00006eb0: 4367 4141 4142 4148 4141 4145 4141 4141  CgAAABAHAAAEAAAA
 00006ec0: 4151 4141 4141 7741 4141 4149 4141 7741  AQAAAAwAAAAIAAwA
@@ -1912,18 +1912,18 @@
 00007770: 4e43 4973 4943 4a75 6457 3177 6556 3930  NCIsICJudW1weV90
 00007780: 6558 426c 496a 6f67 496e 5670 626e 5132  eXBlIjogInVpbnQ2
 00007790: 4e43 4973 4943 4a74 5a58 5268 5a47 4630  NCIsICJtZXRhZGF0
 000077a0: 5953 4936 4947 3531 6247 7839 5853 7767  YSI6IG51bGx9XSwg
 000077b0: 496d 4e79 5a57 4630 6233 4969 4f69 4237  ImNyZWF0b3IiOiB7
 000077c0: 496d 7870 596e 4a68 636e 6b69 4f69 4169  ImxpYnJhcnkiOiAi
 000077d0: 6348 6c68 636e 4a76 6479 4973 4943 4a32  cHlhcnJvdyIsICJ2
-000077e0: 5a58 4a7a 6157 3975 496a 6f67 496a 4530  ZXJzaW9uIjogIjE0
-000077f0: 4c6a 4175 4d53 4a39 4c43 4169 6347 4675  LjAuMSJ9LCAicGFu
+000077e0: 5a58 4a7a 6157 3975 496a 6f67 496a 4532  ZXJzaW9uIjogIjE2
+000077f0: 4c6a 4175 4d43 4a39 4c43 4169 6347 4675  LjAuMCJ9LCAicGFu
 00007800: 5a47 467a 5833 5a6c 636e 4e70 6232 3469  ZGFzX3ZlcnNpb24i
-00007810: 4f69 4169 4d69 3477 4c6a 4d69 6651 4141  OiAiMi4wLjMifQAA
+00007810: 4f69 4169 4d69 3479 4c6a 4969 6651 4141  OiAiMi4yLjIifQAA
 00007820: 4451 4141 4148 5143 4141 4173 4167 4141  DQAAAHQCAAAsAgAA
 00007830: 2b41 4541 414d 7742 4141 4367 4151 4141  +AEAAMwBAACgAQAA
 00007840: 6341 4541 4144 6742 4141 4145 4151 4141  cAEAADgBAAAEAQAA
 00007850: 3041 4141 414a 6741 4141 4273 4141 4141  0AAAAJgAAABsAAAA
 00007860: 5041 4141 4141 5141 4141 4451 2f66 2f2f  PAAAAAQAAADQ/f//
 00007870: 4141 4142 4168 4141 4141 4167 4141 4141  AAABAhAAAAAgAAAA
 00007880: 4241 4141 4141 4141 4141 414f 4141 4141  BAAAAAAAAAAOAAAA
@@ -1975,12 +1975,12 @@
 00007b60: 4277 414d 4141 4141 4541 4151 4141 4141  BwAMAAAAEAAQAAAA
 00007b70: 4141 4142 4168 4141 4141 416b 4141 4141  AAABAhAAAAAkAAAA
 00007b80: 4241 4141 4141 4141 4141 414a 4141 4141  BAAAAAAAAAAJAAAA
 00007b90: 6332 3931 636d 4e6c 5832 6c6b 4141 4141  c291cmNlX2lkAAAA
 00007ba0: 4341 414d 4141 6741 4277 4149 4141 4141  CAAMAAgABwAIAAAA
 00007bb0: 4141 4141 4155 4141 4141 413d 0018 2070  AAAAAUAAAAA=.. p
 00007bc0: 6172 7175 6574 2d63 7070 2d61 7272 6f77  arquet-cpp-arrow
-00007bd0: 2076 6572 7369 6f6e 2031 342e 302e 3119   version 14.0.1.
+00007bd0: 2076 6572 7369 6f6e 2031 362e 302e 3019   version 16.0.0.
 00007be0: dc1c 0000 1c00 001c 0000 1c00 001c 0000  ................
 00007bf0: 1c00 001c 0000 1c00 001c 0000 1c00 001c  ................
 00007c00: 0000 1c00 001c 0000 0056 1a00 0050 4152  .........V...PAR
 00007c10: 31                                       1
```

### Comparing `hipscat-0.3.3/tests/data/small_sky_source/Norder=2/Dir=0/Npix=187.parquet` & `hipscat-0.3.4/tests/data/small_sky_source/Norder=2/Dir=0/Npix=187.parquet`

 * *Files 2% similar despite different names*

```diff
@@ -2504,17 +2504,17 @@
 00009c70: 7061 6e64 6173 5f74 7970 6522 3a20 2275  pandas_type": "u
 00009c80: 696e 7436 3422 2c20 226e 756d 7079 5f74  int64", "numpy_t
 00009c90: 7970 6522 3a20 2275 696e 7436 3422 2c20  ype": "uint64", 
 00009ca0: 226d 6574 6164 6174 6122 3a20 6e75 6c6c  "metadata": null
 00009cb0: 7d5d 2c20 2263 7265 6174 6f72 223a 207b  }], "creator": {
 00009cc0: 226c 6962 7261 7279 223a 2022 7079 6172  "library": "pyar
 00009cd0: 726f 7722 2c20 2276 6572 7369 6f6e 223a  row", "version":
-00009ce0: 2022 3134 2e30 2e31 227d 2c20 2270 616e   "14.0.1"}, "pan
+00009ce0: 2022 3136 2e30 2e30 227d 2c20 2270 616e   "16.0.0"}, "pan
 00009cf0: 6461 735f 7665 7273 696f 6e22 3a20 2232  das_version": "2
-00009d00: 2e30 2e33 227d 0018 0c41 5252 4f57 3a73  .0.3"}...ARROW:s
+00009d00: 2e32 2e32 227d 0018 0c41 5252 4f57 3a73  .2.2"}...ARROW:s
 00009d10: 6368 656d 6118 cc1a 2f2f 2f2f 2f2f 414a  chema...//////AJ
 00009d20: 4141 4151 4141 4141 4141 414b 4141 3441  AAAQAAAAAAAKAA4A
 00009d30: 4267 4146 4141 6741 4367 4141 4141 4142  BgAFAAgACgAAAAAB
 00009d40: 4241 4151 4141 4141 4141 414b 4141 7741  BAAQAAAAAAAKAAwA
 00009d50: 4141 4145 4141 6741 4367 4141 4142 4148  AAAEAAgACgAAABAH
 00009d60: 4141 4145 4141 4141 4151 4141 4141 7741  AAAEAAAAAQAAAAwA
 00009d70: 4141 4149 4141 7741 4241 4149 4141 6741  AAAIAAwABAAIAAgA
@@ -2659,18 +2659,18 @@
 0000a620: 6457 3177 6556 3930 6558 426c 496a 6f67  dW1weV90eXBlIjog
 0000a630: 496e 5670 626e 5132 4e43 4973 4943 4a74  InVpbnQ2NCIsICJt
 0000a640: 5a58 5268 5a47 4630 5953 4936 4947 3531  ZXRhZGF0YSI6IG51
 0000a650: 6247 7839 5853 7767 496d 4e79 5a57 4630  bGx9XSwgImNyZWF0
 0000a660: 6233 4969 4f69 4237 496d 7870 596e 4a68  b3IiOiB7ImxpYnJh
 0000a670: 636e 6b69 4f69 4169 6348 6c68 636e 4a76  cnkiOiAicHlhcnJv
 0000a680: 6479 4973 4943 4a32 5a58 4a7a 6157 3975  dyIsICJ2ZXJzaW9u
-0000a690: 496a 6f67 496a 4530 4c6a 4175 4d53 4a39  IjogIjE0LjAuMSJ9
+0000a690: 496a 6f67 496a 4532 4c6a 4175 4d43 4a39  IjogIjE2LjAuMCJ9
 0000a6a0: 4c43 4169 6347 4675 5a47 467a 5833 5a6c  LCAicGFuZGFzX3Zl
-0000a6b0: 636e 4e70 6232 3469 4f69 4169 4d69 3477  cnNpb24iOiAiMi4w
-0000a6c0: 4c6a 4d69 6651 4141 4451 4141 4148 5143  LjMifQAADQAAAHQC
+0000a6b0: 636e 4e70 6232 3469 4f69 4169 4d69 3479  cnNpb24iOiAiMi4y
+0000a6c0: 4c6a 4969 6651 4141 4451 4141 4148 5143  LjIifQAADQAAAHQC
 0000a6d0: 4141 4173 4167 4141 2b41 4541 414d 7742  AAAsAgAA+AEAAMwB
 0000a6e0: 4141 4367 4151 4141 6341 4541 4144 6742  AACgAQAAcAEAADgB
 0000a6f0: 4141 4145 4151 4141 3041 4141 414a 6741  AAAEAQAA0AAAAJgA
 0000a700: 4141 4273 4141 4141 5041 4141 4141 5141  AABsAAAAPAAAAAQA
 0000a710: 4141 4451 2f66 2f2f 4141 4142 4168 4141  AADQ/f//AAABAhAA
 0000a720: 4141 4167 4141 4141 4241 4141 4141 4141  AAAgAAAABAAAAAAA
 0000a730: 4141 414f 4141 4141 5832 6870 6348 4e6a  AAAOAAAAX2hpcHNj
@@ -2722,11 +2722,11 @@
 0000aa10: 4541 4151 4141 4141 4141 4142 4168 4141  EAAQAAAAAAABAhAA
 0000aa20: 4141 416b 4141 4141 4241 4141 4141 4141  AAAkAAAABAAAAAAA
 0000aa30: 4141 414a 4141 4141 6332 3931 636d 4e6c  AAAJAAAAc291cmNl
 0000aa40: 5832 6c6b 4141 4141 4341 414d 4141 6741  X2lkAAAACAAMAAgA
 0000aa50: 4277 4149 4141 4141 4141 4141 4155 4141  BwAIAAAAAAAAAUAA
 0000aa60: 4141 413d 0018 2070 6172 7175 6574 2d63  AAA=.. parquet-c
 0000aa70: 7070 2d61 7272 6f77 2076 6572 7369 6f6e  pp-arrow version
-0000aa80: 2031 342e 302e 3119 dc1c 0000 1c00 001c   14.0.1.........
+0000aa80: 2031 362e 302e 3019 dc1c 0000 1c00 001c   16.0.0.........
 0000aa90: 0000 1c00 001c 0000 1c00 001c 0000 1c00  ................
 0000aaa0: 001c 0000 1c00 001c 0000 1c00 001c 0000  ................
 0000aab0: 0059 1a00 0050 4152 31                   .Y...PAR1
```

### Comparing `hipscat-0.3.3/tests/data/small_sky_source/_common_metadata` & `hipscat-0.3.4/tests/data/small_sky_source/_common_metadata`

 * *Files 2% similar despite different names*

```diff
@@ -117,17 +117,17 @@
 00000740: 6174 5f69 6e64 6578 222c 2022 7061 6e64  at_index", "pand
 00000750: 6173 5f74 7970 6522 3a20 2275 696e 7436  as_type": "uint6
 00000760: 3422 2c20 226e 756d 7079 5f74 7970 6522  4", "numpy_type"
 00000770: 3a20 2275 696e 7436 3422 2c20 226d 6574  : "uint64", "met
 00000780: 6164 6174 6122 3a20 6e75 6c6c 7d5d 2c20  adata": null}], 
 00000790: 2263 7265 6174 6f72 223a 207b 226c 6962  "creator": {"lib
 000007a0: 7261 7279 223a 2022 7079 6172 726f 7722  rary": "pyarrow"
-000007b0: 2c20 2276 6572 7369 6f6e 223a 2022 3134  , "version": "14
-000007c0: 2e30 2e31 227d 2c20 2270 616e 6461 735f  .0.1"}, "pandas_
-000007d0: 7665 7273 696f 6e22 3a20 2232 2e30 2e33  version": "2.0.3
+000007b0: 2c20 2276 6572 7369 6f6e 223a 2022 3136  , "version": "16
+000007c0: 2e30 2e30 227d 2c20 2270 616e 6461 735f  .0.0"}, "pandas_
+000007d0: 7665 7273 696f 6e22 3a20 2232 2e32 2e32  version": "2.2.2
 000007e0: 227d 0018 0c41 5252 4f57 3a73 6368 656d  "}...ARROW:schem
 000007f0: 6118 cc1a 2f2f 2f2f 2f2f 414a 4141 4151  a...//////AJAAAQ
 00000800: 4141 4141 4141 414b 4141 3441 4267 4146  AAAAAAAKAA4ABgAF
 00000810: 4141 6741 4367 4141 4141 4142 4241 4151  AAgACgAAAAABBAAQ
 00000820: 4141 4141 4141 414b 4141 7741 4141 4145  AAAAAAAKAAwAAAAE
 00000830: 4141 6741 4367 4141 4142 4148 4141 4145  AAgACgAAABAHAAAE
 00000840: 4141 4141 4151 4141 4141 7741 4141 4149  AAAAAQAAAAwAAAAI
@@ -273,17 +273,17 @@
 00001100: 6556 3930 6558 426c 496a 6f67 496e 5670  eV90eXBlIjogInVp
 00001110: 626e 5132 4e43 4973 4943 4a74 5a58 5268  bnQ2NCIsICJtZXRh
 00001120: 5a47 4630 5953 4936 4947 3531 6247 7839  ZGF0YSI6IG51bGx9
 00001130: 5853 7767 496d 4e79 5a57 4630 6233 4969  XSwgImNyZWF0b3Ii
 00001140: 4f69 4237 496d 7870 596e 4a68 636e 6b69  OiB7ImxpYnJhcnki
 00001150: 4f69 4169 6348 6c68 636e 4a76 6479 4973  OiAicHlhcnJvdyIs
 00001160: 4943 4a32 5a58 4a7a 6157 3975 496a 6f67  ICJ2ZXJzaW9uIjog
-00001170: 496a 4530 4c6a 4175 4d53 4a39 4c43 4169  IjE0LjAuMSJ9LCAi
+00001170: 496a 4532 4c6a 4175 4d43 4a39 4c43 4169  IjE2LjAuMCJ9LCAi
 00001180: 6347 4675 5a47 467a 5833 5a6c 636e 4e70  cGFuZGFzX3ZlcnNp
-00001190: 6232 3469 4f69 4169 4d69 3477 4c6a 4d69  b24iOiAiMi4wLjMi
+00001190: 6232 3469 4f69 4169 4d69 3479 4c6a 4969  b24iOiAiMi4yLjIi
 000011a0: 6651 4141 4451 4141 4148 5143 4141 4173  fQAADQAAAHQCAAAs
 000011b0: 4167 4141 2b41 4541 414d 7742 4141 4367  AgAA+AEAAMwBAACg
 000011c0: 4151 4141 6341 4541 4144 6742 4141 4145  AQAAcAEAADgBAAAE
 000011d0: 4151 4141 3041 4141 414a 6741 4141 4273  AQAA0AAAAJgAAABs
 000011e0: 4141 4141 5041 4141 4141 5141 4141 4451  AAAAPAAAAAQAAADQ
 000011f0: 2f66 2f2f 4141 4142 4168 4141 4141 4167  /f//AAABAhAAAAAg
 00001200: 4141 4141 4241 4141 4141 4141 4141 414f  AAAABAAAAAAAAAAO
@@ -335,12 +335,12 @@
 000014e0: 4141 5941 4277 414d 4141 4141 4541 4151  AAYABwAMAAAAEAAQ
 000014f0: 4141 4141 4141 4142 4168 4141 4141 416b  AAAAAAABAhAAAAAk
 00001500: 4141 4141 4241 4141 4141 4141 4141 414a  AAAABAAAAAAAAAAJ
 00001510: 4141 4141 6332 3931 636d 4e6c 5832 6c6b  AAAAc291cmNlX2lk
 00001520: 4141 4141 4341 414d 4141 6741 4277 4149  AAAACAAMAAgABwAI
 00001530: 4141 4141 4141 4141 4155 4141 4141 413d  AAAAAAAAAUAAAAA=
 00001540: 0018 2070 6172 7175 6574 2d63 7070 2d61  .. parquet-cpp-a
-00001550: 7272 6f77 2076 6572 7369 6f6e 2031 342e  rrow version 14.
-00001560: 302e 3119 dc1c 0000 1c00 001c 0000 1c00  0.1.............
+00001550: 7272 6f77 2076 6572 7369 6f6e 2031 362e  rrow version 16.
+00001560: 302e 3019 dc1c 0000 1c00 001c 0000 1c00  0.0.............
 00001570: 001c 0000 1c00 001c 0000 1c00 001c 0000  ................
 00001580: 1c00 001c 0000 1c00 001c 0000 0089 1500  ................
 00001590: 0050 4152 31                             .PAR1
```

### Comparing `hipscat-0.3.3/tests/data/small_sky_source/_metadata` & `hipscat-0.3.4/tests/data/small_sky_source/_metadata`

 * *Files 0% similar despite different names*

```diff
@@ -1583,17 +1583,17 @@
 000062e0: 616e 6461 735f 7479 7065 223a 2022 7569  andas_type": "ui
 000062f0: 6e74 3634 222c 2022 6e75 6d70 795f 7479  nt64", "numpy_ty
 00006300: 7065 223a 2022 7569 6e74 3634 222c 2022  pe": "uint64", "
 00006310: 6d65 7461 6461 7461 223a 206e 756c 6c7d  metadata": null}
 00006320: 5d2c 2022 6372 6561 746f 7222 3a20 7b22  ], "creator": {"
 00006330: 6c69 6272 6172 7922 3a20 2270 7961 7272  library": "pyarr
 00006340: 6f77 222c 2022 7665 7273 696f 6e22 3a20  ow", "version": 
-00006350: 2231 342e 302e 3122 7d2c 2022 7061 6e64  "14.0.1"}, "pand
+00006350: 2231 362e 302e 3022 7d2c 2022 7061 6e64  "16.0.0"}, "pand
 00006360: 6173 5f76 6572 7369 6f6e 223a 2022 322e  as_version": "2.
-00006370: 302e 3322 7d00 180c 4152 524f 573a 7363  0.3"}...ARROW:sc
+00006370: 322e 3222 7d00 180c 4152 524f 573a 7363  2.2"}...ARROW:sc
 00006380: 6865 6d61 18cc 1a2f 2f2f 2f2f 2f41 4a41  hema...//////AJA
 00006390: 4141 5141 4141 4141 4141 4b41 4134 4142  AAQAAAAAAAKAA4AB
 000063a0: 6741 4641 4167 4143 6741 4141 4141 4242  gAFAAgACgAAAAABB
 000063b0: 4141 5141 4141 4141 4141 4b41 4177 4141  AAQAAAAAAAKAAwAA
 000063c0: 4141 4541 4167 4143 6741 4141 4241 4841  AAEAAgACgAAABAHA
 000063d0: 4141 4541 4141 4141 5141 4141 4177 4141  AAEAAAAAQAAAAwAA
 000063e0: 4141 4941 4177 4142 4141 4941 4167 4141  AAIAAwABAAIAAgAA
@@ -1738,18 +1738,18 @@
 00006c90: 5731 7765 5639 3065 5842 6c49 6a6f 6749  W1weV90eXBlIjogI
 00006ca0: 6e56 7062 6e51 324e 4349 7349 434a 745a  nVpbnQ2NCIsICJtZ
 00006cb0: 5852 685a 4746 3059 5349 3649 4735 3162  XRhZGF0YSI6IG51b
 00006cc0: 4778 3958 5377 6749 6d4e 795a 5746 3062  Gx9XSwgImNyZWF0b
 00006cd0: 3349 694f 6942 3749 6d78 7059 6e4a 6863  3IiOiB7ImxpYnJhc
 00006ce0: 6e6b 694f 6941 6963 486c 6863 6e4a 7664  nkiOiAicHlhcnJvd
 00006cf0: 7949 7349 434a 325a 584a 7a61 5739 7549  yIsICJ2ZXJzaW9uI
-00006d00: 6a6f 6749 6a45 304c 6a41 754d 534a 394c  jogIjE0LjAuMSJ9L
+00006d00: 6a6f 6749 6a45 324c 6a41 754d 434a 394c  jogIjE2LjAuMCJ9L
 00006d10: 4341 6963 4746 755a 4746 7a58 335a 6c63  CAicGFuZGFzX3Zlc
-00006d20: 6e4e 7062 3234 694f 6941 694d 6934 774c  nNpb24iOiAiMi4wL
-00006d30: 6a4d 6966 5141 4144 5141 4141 4851 4341  jMifQAADQAAAHQCA
+00006d20: 6e4e 7062 3234 694f 6941 694d 6934 794c  nNpb24iOiAiMi4yL
+00006d30: 6a49 6966 5141 4144 5141 4141 4851 4341  jIifQAADQAAAHQCA
 00006d40: 4141 7341 6741 412b 4145 4141 4d77 4241  AAsAgAA+AEAAMwBA
 00006d50: 4143 6741 5141 4163 4145 4141 4467 4241  ACgAQAAcAEAADgBA
 00006d60: 4141 4541 5141 4130 4141 4141 4a67 4141  AAEAQAA0AAAAJgAA
 00006d70: 4142 7341 4141 4150 4141 4141 4151 4141  ABsAAAAPAAAAAQAA
 00006d80: 4144 512f 662f 2f41 4141 4241 6841 4141  ADQ/f//AAABAhAAA
 00006d90: 4141 6741 4141 4142 4141 4141 4141 4141  AAgAAAABAAAAAAAA
 00006da0: 4141 4f41 4141 4158 3268 7063 484e 6a59  AAOAAAAX2hpcHNjY
@@ -1801,11 +1801,11 @@
 00007080: 4141 5141 4141 4141 4141 4241 6841 4141  AAQAAAAAAABAhAAA
 00007090: 4141 6b41 4141 4142 4141 4141 4141 4141  AAkAAAABAAAAAAAA
 000070a0: 4141 4a41 4141 4163 3239 3163 6d4e 6c58  AAJAAAAc291cmNlX
 000070b0: 326c 6b41 4141 4143 4141 4d41 4167 4142  2lkAAAACAAMAAgAB
 000070c0: 7741 4941 4141 4141 4141 4141 5541 4141  wAIAAAAAAAAAUAAA
 000070d0: 4141 3d00 1820 7061 7271 7565 742d 6370  AA=.. parquet-cp
 000070e0: 702d 6172 726f 7720 7665 7273 696f 6e20  p-arrow version 
-000070f0: 3134 2e30 2e31 19dc 1c00 001c 0000 1c00  14.0.1..........
+000070f0: 3136 2e30 2e30 19dc 1c00 001c 0000 1c00  16.0.0..........
 00007100: 001c 0000 1c00 001c 0000 1c00 001c 0000  ................
 00007110: 1c00 001c 0000 1c00 001c 0000 1c00 0000  ................
 00007120: 1c71 0000 5041 5231                      .q..PAR1
```

### Comparing `hipscat-0.3.3/tests/data/small_sky_source/point_map.fits` & `hipscat-0.3.4/tests/data/small_sky_source/point_map.fits`

 * *Files 2% similar despite different names*

```diff
@@ -229,16 +229,16 @@
 00000e40: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00000e50: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00000e60: 5049 5854 5950 4520 3d20 2748 4541 4c50  PIXTYPE = 'HEALP
 00000e70: 4958 2027 2020 2020 2020 2020 2020 202f  IX '           /
 00000e80: 2048 4541 4c50 4958 2070 6978 656c 6973   HEALPIX pixelis
 00000e90: 6174 696f 6e20 2020 2020 2020 2020 2020  ation           
 00000ea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000eb0: 4f52 4445 5249 4e47 3d20 2752 494e 4720  ORDERING= 'RING 
-00000ec0: 2020 2027 2020 2020 2020 2020 2020 202f     '           /
+00000eb0: 4f52 4445 5249 4e47 3d20 274e 4553 5445  ORDERING= 'NESTE
+00000ec0: 4420 2027 2020 2020 2020 2020 2020 202f  D  '           /
 00000ed0: 2050 6978 656c 206f 7264 6572 696e 6720   Pixel ordering 
 00000ee0: 7363 6865 6d65 2c20 6569 7468 6572 2052  scheme, either R
 00000ef0: 494e 4720 6f72 204e 4553 5445 4420 2020  ING or NESTED   
 00000f00: 4558 544e 414d 4520 3d20 2778 7465 6e73  EXTNAME = 'xtens
 00000f10: 696f 6e27 2020 2020 2020 2020 2020 202f  ion'           /
 00000f20: 206e 616d 6520 6f66 2074 6869 7320 6269   name of this bi
 00000f30: 6e61 7279 2074 6162 6c65 2065 7874 656e  nary table exten
```

### Comparing `hipscat-0.3.3/tests/data/small_sky_source/provenance_info.json` & `hipscat-0.3.4/tests/data/small_sky_source/provenance_info.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8783139442861665%*

 * *Differences: {"'generation_date'": "'2024.05.29'",*

 * * "'tool_args'": "{'version': '0.3.3.dev10+gd573bcd', 'runtime_args': {'tmp_dir': "*

 * *                "'/tmp/tmpgasth6x_', 'tmp_path': '/tmp/tmpgasth6x_/small_sky_source/intermediate', "*

 * *                "'input_paths': "*

 * *                "['file:///home/delucchi/git/fits/tests/data/../../../hipscat-import/tests/hipscat_import/data/small_sky_source/small_sky_source.csv'], "*

 * *                "'file_reader_info': {'type_map': None, 'parquet_kwargs': None, 'kwargs': "*

 * *           […]*

```diff
@@ -1,13 +1,13 @@
 {
     "catalog_name": "small_sky_source",
     "catalog_type": "source",
     "dec_column": "source_dec",
     "epoch": "J2000",
-    "generation_date": "2024.03.01",
+    "generation_date": "2024.05.29",
     "ra_column": "source_ra",
     "tool_args": {
         "runtime_args": {
             "catalog_name": "small_sky_source",
             "catalog_path": "./small_sky_source",
             "catalog_type": "source",
             "constant_healpix_order": -1,
@@ -18,34 +18,35 @@
             "dec_column": "source_dec",
             "epoch": "J2000",
             "file_reader_info": {
                 "chunksize": 500000,
                 "column_names": null,
                 "header": "infer",
                 "input_reader_type": "CsvReader",
+                "kwargs": {},
+                "parquet_kwargs": null,
                 "schema_file": null,
-                "separator": ",",
-                "type_map": {}
+                "type_map": null
             },
             "highest_healpix_order": 7,
             "input_file_list": [],
             "input_path": "../../../hipscat-import/tests/hipscat_import/data/small_sky_source",
             "input_paths": [
-                "file:///home/delucchi/git/hipscat/tests/data/../../../hipscat-import/tests/hipscat_import/data/small_sky_source/small_sky_source.csv"
+                "file:///home/delucchi/git/fits/tests/data/../../../hipscat-import/tests/hipscat_import/data/small_sky_source/small_sky_source.csv"
             ],
+            "lowest_healpix_order": 0,
             "mapping_healpix_order": 7,
             "output_artifact_name": "small_sky_source",
             "output_path": ".",
-            "overwrite": true,
             "pixel_threshold": 3000,
             "ra_column": "source_ra",
             "sort_columns": null,
-            "tmp_dir": "/tmp/user/11115/tmp2vluzdw5",
-            "tmp_path": "/tmp/user/11115/tmp2vluzdw5/small_sky_source/intermediate",
+            "tmp_dir": "/tmp/tmpgasth6x_",
+            "tmp_path": "/tmp/tmpgasth6x_/small_sky_source/intermediate",
             "use_hipscat_index": false
         },
         "tool_name": "hipscat_import",
-        "version": "0.2.5.dev5+g0733afb"
+        "version": "0.3.3.dev10+gd573bcd"
     },
     "total_rows": 17161,
-    "version": "0.2.7.dev5+gde86705"
+    "version": "0.3.4.dev17+g922a4b7.d20240529"
 }
```

### Comparing `hipscat-0.3.3/tests/data/small_sky_source_object_index/README.md` & `hipscat-0.3.4/tests/data/small_sky_source_object_index/README.md`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.3/tests/data/small_sky_source_object_index/_common_metadata` & `hipscat-0.3.4/tests/data/small_sky_source_object_index/_common_metadata`

 * *Files 3% similar despite different names*

```diff
@@ -43,17 +43,17 @@
 000002a0: 7061 6e64 6173 5f74 7970 6522 3a20 2269  pandas_type": "i
 000002b0: 6e74 3634 222c 2022 6e75 6d70 795f 7479  nt64", "numpy_ty
 000002c0: 7065 223a 2022 696e 7436 3422 2c20 226d  pe": "int64", "m
 000002d0: 6574 6164 6174 6122 3a20 6e75 6c6c 7d5d  etadata": null}]
 000002e0: 2c20 2263 7265 6174 6f72 223a 207b 226c  , "creator": {"l
 000002f0: 6962 7261 7279 223a 2022 7079 6172 726f  ibrary": "pyarro
 00000300: 7722 2c20 2276 6572 7369 6f6e 223a 2022  w", "version": "
-00000310: 3134 2e30 2e31 227d 2c20 2270 616e 6461  14.0.1"}, "panda
-00000320: 735f 7665 7273 696f 6e22 3a20 2232 2e30  s_version": "2.0
-00000330: 2e33 227d 0018 0c41 5252 4f57 3a73 6368  .3"}...ARROW:sch
+00000310: 3136 2e30 2e30 227d 2c20 2270 616e 6461  16.0.0"}, "panda
+00000320: 735f 7665 7273 696f 6e22 3a20 2232 2e32  s_version": "2.2
+00000330: 2e32 227d 0018 0c41 5252 4f57 3a73 6368  .2"}...ARROW:sch
 00000340: 656d 6118 f80a 2f2f 2f2f 2f78 4145 4141  ema.../////xAEAA
 00000350: 4151 4141 4141 4141 414b 4141 3441 4267  AQAAAAAAAKAA4ABg
 00000360: 4146 4141 6741 4367 4141 4141 4142 4241  AFAAgACgAAAAABBA
 00000370: 4151 4141 4141 4141 414b 4141 7741 4141  AQAAAAAAAKAAwAAA
 00000380: 4145 4141 6741 4367 4141 4150 6743 4141  AEAAgACgAAAPgCAA
 00000390: 4145 4141 4141 4151 4141 4141 7741 4141  AEAAAAAQAAAAwAAA
 000003a0: 4149 4141 7741 4241 4149 4141 6741 4141  AIAAwABAAIAAgAAA
@@ -110,18 +110,18 @@
 000006d0: 5930 4969 7767 496d 3531 6258 4235 5833  Y0IiwgIm51bXB5X3
 000006e0: 5235 6347 5569 4f69 4169 6157 3530 4e6a  R5cGUiOiAiaW50Nj
 000006f0: 5169 4c43 4169 6257 5630 5957 5268 6447  QiLCAibWV0YWRhdG
 00000700: 4569 4f69 4275 6457 7873 6656 3073 4943  EiOiBudWxsfV0sIC
 00000710: 4a6a 636d 5668 6447 3979 496a 6f67 6579  JjcmVhdG9yIjogey
 00000720: 4a73 6157 4a79 5958 4a35 496a 6f67 496e  JsaWJyYXJ5IjogIn
 00000730: 4235 5958 4a79 6233 6369 4c43 4169 646d  B5YXJyb3ciLCAidm
-00000740: 5679 6332 6c76 6269 4936 4943 4978 4e43  Vyc2lvbiI6ICIxNC
-00000750: 3477 4c6a 4569 6653 7767 496e 4268 626d  4wLjEifSwgInBhbm
+00000740: 5679 6332 6c76 6269 4936 4943 4978 4e69  Vyc2lvbiI6ICIxNi
+00000750: 3477 4c6a 4169 6653 7767 496e 4268 626d  4wLjAifSwgInBhbm
 00000760: 5268 6331 3932 5a58 4a7a 6157 3975 496a  Rhc192ZXJzaW9uIj
-00000770: 6f67 496a 4975 4d43 347a 496e 3041 4141  ogIjIuMC4zIn0AAA
+00000770: 6f67 496a 4975 4d69 3479 496e 3041 4141  ogIjIuMi4yIn0AAA
 00000780: 4145 4141 4141 7341 4141 4148 5141 4141  AEAAAAsAAAAHQAAA
 00000790: 4245 4141 4141 4241 4141 4148 442f 2f2f  BEAAAABAAAAHD///
 000007a0: 3841 4141 4543 4541 4141 4143 5141 4141  8AAAECEAAAACQAAA
 000007b0: 4145 4141 4141 4141 4141 4141 6b41 4141  AEAAAAAAAAAAkAAA
 000007c0: 4276 596d 706c 5933 5266 6157 5141 4141  BvYmplY3RfaWQAAA
 000007d0: 4149 4141 7741 4341 4148 4141 6741 4141  AIAAwACAAHAAgAAA
 000007e0: 4141 4141 4142 5141 4141 414b 7a2f 2f2f  AAAAABQAAAAKz///
@@ -135,10 +135,10 @@
 00000860: 4149 4141 5941 4277 414d 4141 4141 4541  AIAAYABwAMAAAAEA
 00000870: 4151 4141 4141 4141 4142 4168 4141 4141  AQAAAAAAABAhAAAA
 00000880: 4167 4141 4141 4241 4141 4141 4141 4141  AgAAAABAAAAAAAAA
 00000890: 4147 4141 4141 546d 3979 5a47 5679 4141  AGAAAATm9yZGVyAA
 000008a0: 4141 4141 5941 4341 4145 4141 5941 4141  AAAAYACAAEAAYAAA
 000008b0: 4149 4141 4141 4141 4141 4141 3d3d 0018  AIAAAAAAAAAA==..
 000008c0: 2070 6172 7175 6574 2d63 7070 2d61 7272   parquet-cpp-arr
-000008d0: 6f77 2076 6572 7369 6f6e 2031 342e 302e  ow version 14.0.
-000008e0: 3119 4c1c 0000 1c00 001c 0000 1c00 0000  1.L.............
+000008d0: 6f77 2076 6572 7369 6f6e 2031 362e 302e  ow version 16.0.
+000008e0: 3019 4c1c 0000 1c00 001c 0000 1c00 0000  0.L.............
 000008f0: ec08 0000 5041 5231                      ....PAR1
```

### Comparing `hipscat-0.3.3/tests/data/small_sky_source_object_index/_metadata` & `hipscat-0.3.4/tests/data/small_sky_source_object_index/_metadata`

 * *Files 3% similar despite different names*

```diff
@@ -70,17 +70,17 @@
 00000450: 2270 616e 6461 735f 7479 7065 223a 2022  "pandas_type": "
 00000460: 696e 7436 3422 2c20 226e 756d 7079 5f74  int64", "numpy_t
 00000470: 7970 6522 3a20 2269 6e74 3634 222c 2022  ype": "int64", "
 00000480: 6d65 7461 6461 7461 223a 206e 756c 6c7d  metadata": null}
 00000490: 5d2c 2022 6372 6561 746f 7222 3a20 7b22  ], "creator": {"
 000004a0: 6c69 6272 6172 7922 3a20 2270 7961 7272  library": "pyarr
 000004b0: 6f77 222c 2022 7665 7273 696f 6e22 3a20  ow", "version": 
-000004c0: 2231 342e 302e 3122 7d2c 2022 7061 6e64  "14.0.1"}, "pand
+000004c0: 2231 362e 302e 3022 7d2c 2022 7061 6e64  "16.0.0"}, "pand
 000004d0: 6173 5f76 6572 7369 6f6e 223a 2022 322e  as_version": "2.
-000004e0: 302e 3322 7d00 180c 4152 524f 573a 7363  0.3"}...ARROW:sc
+000004e0: 322e 3222 7d00 180c 4152 524f 573a 7363  2.2"}...ARROW:sc
 000004f0: 6865 6d61 18f8 0a2f 2f2f 2f2f 7841 4541  hema.../////xAEA
 00000500: 4141 5141 4141 4141 4141 4b41 4134 4142  AAQAAAAAAAKAA4AB
 00000510: 6741 4641 4167 4143 6741 4141 4141 4242  gAFAAgACgAAAAABB
 00000520: 4141 5141 4141 4141 4141 4b41 4177 4141  AAQAAAAAAAKAAwAA
 00000530: 4141 4541 4167 4143 6741 4141 5067 4341  AAEAAgACgAAAPgCA
 00000540: 4141 4541 4141 4141 5141 4141 4177 4141  AAEAAAAAQAAAAwAA
 00000550: 4141 4941 4177 4142 4141 4941 4167 4141  AAIAAwABAAIAAgAA
@@ -138,17 +138,17 @@
 00000890: 3352 3563 4755 694f 6941 6961 5735 304e  3R5cGUiOiAiaW50N
 000008a0: 6a51 694c 4341 6962 5756 3059 5752 6864  jQiLCAibWV0YWRhd
 000008b0: 4745 694f 6942 7564 5778 7366 5630 7349  GEiOiBudWxsfV0sI
 000008c0: 434a 6a63 6d56 6864 4739 7949 6a6f 6765  CJjcmVhdG9yIjoge
 000008d0: 794a 7361 574a 7959 584a 3549 6a6f 6749  yJsaWJyYXJ5IjogI
 000008e0: 6e42 3559 584a 7962 3363 694c 4341 6964  nB5YXJyb3ciLCAid
 000008f0: 6d56 7963 326c 7662 6949 3649 4349 784e  mVyc2lvbiI6ICIxN
-00000900: 4334 774c 6a45 6966 5377 6749 6e42 6862  C4wLjEifSwgInBhb
+00000900: 6934 774c 6a41 6966 5377 6749 6e42 6862  i4wLjAifSwgInBhb
 00000910: 6d52 6863 3139 325a 584a 7a61 5739 7549  mRhc192ZXJzaW9uI
-00000920: 6a6f 6749 6a49 754d 4334 7a49 6e30 4141  jogIjIuMC4zIn0AA
+00000920: 6a6f 6749 6a49 754d 6934 7949 6e30 4141  jogIjIuMi4yIn0AA
 00000930: 4141 4541 4141 4173 4141 4141 4851 4141  AAEAAAAsAAAAHQAA
 00000940: 4142 4541 4141 4142 4141 4141 4844 2f2f  ABEAAAABAAAAHD//
 00000950: 2f38 4141 4145 4345 4141 4141 4351 4141  /8AAAECEAAAACQAA
 00000960: 4141 4541 4141 4141 4141 4141 416b 4141  AAEAAAAAAAAAAkAA
 00000970: 4142 7659 6d70 6c59 3352 6661 5751 4141  ABvYmplY3RfaWQAA
 00000980: 4141 4941 4177 4143 4141 4841 4167 4141  AAIAAwACAAHAAgAA
 00000990: 4141 4141 4141 4251 4141 4141 4b7a 2f2f  AAAAAABQAAAAKz//
@@ -162,10 +162,10 @@
 00000a10: 4141 4941 4159 4142 7741 4d41 4141 4145  AAIAAYABwAMAAAAE
 00000a20: 4141 5141 4141 4141 4141 4241 6841 4141  AAQAAAAAAABAhAAA
 00000a30: 4141 6741 4141 4142 4141 4141 4141 4141  AAgAAAABAAAAAAAA
 00000a40: 4141 4741 4141 4154 6d39 795a 4756 7941  AAGAAAATm9yZGVyA
 00000a50: 4141 4141 4159 4143 4141 4541 4159 4141  AAAAAYACAAEAAYAA
 00000a60: 4141 4941 4141 4141 4141 4141 413d 3d00  AAIAAAAAAAAAA==.
 00000a70: 1820 7061 7271 7565 742d 6370 702d 6172  . parquet-cpp-ar
-00000a80: 726f 7720 7665 7273 696f 6e20 3134 2e30  row version 14.0
-00000a90: 2e31 194c 1c00 001c 0000 1c00 001c 0000  .1.L............
+00000a80: 726f 7720 7665 7273 696f 6e20 3136 2e30  row version 16.0
+00000a90: 2e30 194c 1c00 001c 0000 1c00 001c 0000  .0.L............
 00000aa0: 009d 0a00 0050 4152 31                   .....PAR1
```

### Comparing `hipscat-0.3.3/tests/data/small_sky_source_object_index/index/part.0.parquet` & `hipscat-0.3.4/tests/data/small_sky_source_object_index/index/part.0.parquet`

 * *Files 2% similar despite different names*

```diff
@@ -159,17 +159,17 @@
 000009e0: 2270 616e 6461 735f 7479 7065 223a 2022  "pandas_type": "
 000009f0: 696e 7436 3422 2c20 226e 756d 7079 5f74  int64", "numpy_t
 00000a00: 7970 6522 3a20 2269 6e74 3634 222c 2022  ype": "int64", "
 00000a10: 6d65 7461 6461 7461 223a 206e 756c 6c7d  metadata": null}
 00000a20: 5d2c 2022 6372 6561 746f 7222 3a20 7b22  ], "creator": {"
 00000a30: 6c69 6272 6172 7922 3a20 2270 7961 7272  library": "pyarr
 00000a40: 6f77 222c 2022 7665 7273 696f 6e22 3a20  ow", "version": 
-00000a50: 2231 342e 302e 3122 7d2c 2022 7061 6e64  "14.0.1"}, "pand
+00000a50: 2231 362e 302e 3022 7d2c 2022 7061 6e64  "16.0.0"}, "pand
 00000a60: 6173 5f76 6572 7369 6f6e 223a 2022 322e  as_version": "2.
-00000a70: 302e 3322 7d00 180c 4152 524f 573a 7363  0.3"}...ARROW:sc
+00000a70: 322e 3222 7d00 180c 4152 524f 573a 7363  2.2"}...ARROW:sc
 00000a80: 6865 6d61 18f8 0a2f 2f2f 2f2f 7841 4541  hema.../////xAEA
 00000a90: 4141 5141 4141 4141 4141 4b41 4134 4142  AAQAAAAAAAKAA4AB
 00000aa0: 6741 4641 4167 4143 6741 4141 4141 4242  gAFAAgACgAAAAABB
 00000ab0: 4141 5141 4141 4141 4141 4b41 4177 4141  AAQAAAAAAAKAAwAA
 00000ac0: 4141 4541 4167 4143 6741 4141 5067 4341  AAEAAgACgAAAPgCA
 00000ad0: 4141 4541 4141 4141 5141 4141 4177 4141  AAEAAAAAQAAAAwAA
 00000ae0: 4141 4941 4177 4142 4141 4941 4167 4141  AAIAAwABAAIAAgAA
@@ -227,17 +227,17 @@
 00000e20: 3352 3563 4755 694f 6941 6961 5735 304e  3R5cGUiOiAiaW50N
 00000e30: 6a51 694c 4341 6962 5756 3059 5752 6864  jQiLCAibWV0YWRhd
 00000e40: 4745 694f 6942 7564 5778 7366 5630 7349  GEiOiBudWxsfV0sI
 00000e50: 434a 6a63 6d56 6864 4739 7949 6a6f 6765  CJjcmVhdG9yIjoge
 00000e60: 794a 7361 574a 7959 584a 3549 6a6f 6749  yJsaWJyYXJ5IjogI
 00000e70: 6e42 3559 584a 7962 3363 694c 4341 6964  nB5YXJyb3ciLCAid
 00000e80: 6d56 7963 326c 7662 6949 3649 4349 784e  mVyc2lvbiI6ICIxN
-00000e90: 4334 774c 6a45 6966 5377 6749 6e42 6862  C4wLjEifSwgInBhb
+00000e90: 6934 774c 6a41 6966 5377 6749 6e42 6862  i4wLjAifSwgInBhb
 00000ea0: 6d52 6863 3139 325a 584a 7a61 5739 7549  mRhc192ZXJzaW9uI
-00000eb0: 6a6f 6749 6a49 754d 4334 7a49 6e30 4141  jogIjIuMC4zIn0AA
+00000eb0: 6a6f 6749 6a49 754d 6934 7949 6e30 4141  jogIjIuMi4yIn0AA
 00000ec0: 4141 4541 4141 4173 4141 4141 4851 4141  AAEAAAAsAAAAHQAA
 00000ed0: 4142 4541 4141 4142 4141 4141 4844 2f2f  ABEAAAABAAAAHD//
 00000ee0: 2f38 4141 4145 4345 4141 4141 4351 4141  /8AAAECEAAAACQAA
 00000ef0: 4141 4541 4141 4141 4141 4141 416b 4141  AAEAAAAAAAAAAkAA
 00000f00: 4142 7659 6d70 6c59 3352 6661 5751 4141  ABvYmplY3RfaWQAA
 00000f10: 4141 4941 4177 4143 4141 4841 4167 4141  AAIAAwACAAHAAgAA
 00000f20: 4141 4141 4141 4251 4141 4141 4b7a 2f2f  AAAAAABQAAAAKz//
@@ -251,10 +251,10 @@
 00000fa0: 4141 4941 4159 4142 7741 4d41 4141 4145  AAIAAYABwAMAAAAE
 00000fb0: 4141 5141 4141 4141 4141 4241 6841 4141  AAQAAAAAAABAhAAA
 00000fc0: 4141 6741 4141 4142 4141 4141 4141 4141  AAgAAAABAAAAAAAA
 00000fd0: 4141 4741 4141 4154 6d39 795a 4756 7941  AAGAAAATm9yZGVyA
 00000fe0: 4141 4141 4159 4143 4141 4541 4159 4141  AAAAAYACAAEAAYAA
 00000ff0: 4141 4941 4141 4141 4141 4141 413d 3d00  AAIAAAAAAAAAA==.
 00001000: 1820 7061 7271 7565 742d 6370 702d 6172  . parquet-cpp-ar
-00001010: 726f 7720 7665 7273 696f 6e20 3134 2e30  row version 14.0
-00001020: 2e31 194c 1c00 001c 0000 1c00 001c 0000  .1.L............
+00001010: 726f 7720 7665 7273 696f 6e20 3136 2e30  row version 16.0
+00001020: 2e30 194c 1c00 001c 0000 1c00 001c 0000  .0.L............
 00001030: 0041 0a00 0050 4152 31                   .A...PAR1
```

### Comparing `hipscat-0.3.3/tests/data/small_sky_source_object_index/provenance_info.json` & `hipscat-0.3.4/tests/data/small_sky_order1_id_index/provenance_info.json`

 * *Files 21% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6546296296296297%*

 * *Differences: {"'catalog_name'": "'small_sky_order1_id_index'",*

 * * "'generation_date'": "'2024.05.29'",*

 * * "'indexing_column'": "'id'",*

 * * "'primary_catalog'": "'small_sky'",*

 * * "'tool_args'": "{'version': '0.3.3.dev10+gd573bcd', 'runtime_args': {'catalog_name': "*

 * *                "'small_sky_order1_id_index', 'output_artifact_name': 'small_sky_order1_id_index', "*

 * *                "'tmp_dir': '/tmp/tmpgasth6x_', 'catalog_path': './small_sky_order1_id_index', "*

 * *                "'tmp_path': '/tmp/tmpgasth6x_/small_sky_order1_id_inde […]*

```diff
@@ -1,31 +1,30 @@
 {
-    "catalog_name": "small_sky_source_object_index",
+    "catalog_name": "small_sky_order1_id_index",
     "catalog_type": "index",
     "extra_columns": [],
-    "generation_date": "2024.03.01",
-    "indexing_column": "object_id",
-    "primary_catalog": "small_sky_source",
+    "generation_date": "2024.05.29",
+    "indexing_column": "id",
+    "primary_catalog": "small_sky",
     "tool_args": {
         "runtime_args": {
-            "catalog_name": "small_sky_source_object_index",
-            "catalog_path": "./small_sky_source_object_index",
+            "catalog_name": "small_sky_order1_id_index",
+            "catalog_path": "./small_sky_order1_id_index",
             "dask_n_workers": 1,
             "dask_threads_per_worker": 1,
             "dask_tmp": "",
             "extra_columns": [],
             "include_hipscat_index": false,
             "include_order_pixel": true,
-            "indexing_column": "object_id",
-            "input_catalog_path": "small_sky_source",
-            "output_artifact_name": "small_sky_source_object_index",
+            "indexing_column": "id",
+            "input_catalog_path": "small_sky",
+            "output_artifact_name": "small_sky_order1_id_index",
             "output_path": ".",
-            "overwrite": true,
-            "tmp_dir": "/tmp/user/11115/tmp2vluzdw5",
-            "tmp_path": "/tmp/user/11115/tmp2vluzdw5/small_sky_source_object_index/intermediate"
+            "tmp_dir": "/tmp/tmpgasth6x_",
+            "tmp_path": "/tmp/tmpgasth6x_/small_sky_order1_id_index/intermediate"
         },
         "tool_name": "hipscat_import",
-        "version": "0.2.5.dev5+g0733afb"
+        "version": "0.3.3.dev10+gd573bcd"
     },
-    "total_rows": 148,
-    "version": "0.2.7.dev5+gde86705"
+    "total_rows": 131,
+    "version": "0.3.4.dev17+g922a4b7.d20240529"
 }
```

### Comparing `hipscat-0.3.3/tests/data/small_sky_to_small_sky_order1/_common_metadata` & `hipscat-0.3.4/tests/data/small_sky_to_small_sky_order1/_common_metadata`

 * *Files 2% similar despite different names*

```diff
@@ -27,9 +27,9 @@
 000001a0: 4141 4142 4141 4541 4141 4141 4141 4151  AAABAAEAAAAAAAAQ
 000001b0: 4951 4141 4141 4941 4141 4141 5141 4141  IQAAAAIAAAAAQAAA
 000001c0: 4141 4141 4141 4267 4141 4145 3576 636d  AAAAAABgAAAE5vcm
 000001d0: 526c 6367 4141 4341 414d 4141 6741 4277  RlcgAACAAMAAgABw
 000001e0: 4149 4141 4141 4141 4141 4155 4141 4141  AIAAAAAAAAAUAAAA
 000001f0: 413d 0018 2070 6172 7175 6574 2d63 7070  A=.. parquet-cpp
 00000200: 2d61 7272 6f77 2076 6572 7369 6f6e 2031  -arrow version 1
-00000210: 342e 302e 3119 4c1c 0000 1c00 001c 0000  4.0.1.L.........
+00000210: 362e 302e 3019 4c1c 0000 1c00 001c 0000  6.0.0.L.........
 00000220: 1c00 0000 2002 0000 5041 5231            .... ...PAR1
```

### Comparing `hipscat-0.3.3/tests/hipscat/catalog/association_catalog/test_association_catalog.py` & `hipscat-0.3.4/tests/hipscat/catalog/association_catalog/test_association_catalog.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.3/tests/hipscat/catalog/association_catalog/test_association_catalog_info.py` & `hipscat-0.3.4/tests/hipscat/catalog/association_catalog/test_association_catalog_info.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.3/tests/hipscat/catalog/association_catalog/test_partition_join_info.py` & `hipscat-0.3.4/tests/hipscat/catalog/association_catalog/test_partition_join_info.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.3/tests/hipscat/catalog/dataset/test_base_catalog_info.py` & `hipscat-0.3.4/tests/hipscat/catalog/dataset/test_base_catalog_info.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.3/tests/hipscat/catalog/dataset/test_catalog_info_factory.py` & `hipscat-0.3.4/tests/hipscat/catalog/dataset/test_catalog_info_factory.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.3/tests/hipscat/catalog/dataset/test_dataset.py` & `hipscat-0.3.4/tests/hipscat/catalog/dataset/test_dataset.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.3/tests/hipscat/catalog/index/test_index_catalog.py` & `hipscat-0.3.4/tests/hipscat/catalog/index/test_index_catalog.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.3/tests/hipscat/catalog/index/test_index_catalog_info.py` & `hipscat-0.3.4/tests/hipscat/catalog/index/test_index_catalog_info.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.3/tests/hipscat/catalog/margin_cache/test_margin_cache_catalog_info.py` & `hipscat-0.3.4/tests/hipscat/catalog/margin_cache/test_margin_cache_catalog_info.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.3/tests/hipscat/catalog/margin_cache/test_margin_catalog.py` & `hipscat-0.3.4/tests/hipscat/catalog/margin_cache/test_margin_catalog.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import json
 import os
 
 import pytest
 
 from hipscat.catalog import CatalogType, MarginCatalog, PartitionInfo
 from hipscat.loaders import read_from_hipscat
+from hipscat.pixel_math import HealpixPixel
 
 
 def test_init_catalog(margin_catalog_info, margin_catalog_pixels):
     catalog = MarginCatalog(margin_catalog_info, margin_catalog_pixels)
     assert catalog.catalog_name == margin_catalog_info.catalog_name
     assert catalog.get_healpix_pixels() == margin_catalog_pixels
     assert catalog.catalog_info == margin_catalog_info
@@ -72,7 +73,27 @@
     ## Now we create the needed _metadata and everything is right.
     part_info = PartitionInfo.from_healpix(margin_catalog_pixels)
     part_info.write_to_metadata_files(catalog_path=catalog_path)
 
     with pytest.warns(UserWarning, match="slow"):
         catalog = read_from_hipscat(catalog_path)
     assert catalog.catalog_name == margin_cache_catalog_info_data["catalog_name"]
+
+
+def test_margin_filter(margin_catalog_info, margin_catalog_pixels):
+    catalog = MarginCatalog(margin_catalog_info, margin_catalog_pixels)
+    pixels = [HealpixPixel(1, 44)]
+    filtered_catalog = catalog.filter_from_pixel_list(pixels)
+    assert filtered_catalog.get_healpix_pixels() == [
+        HealpixPixel(1, 44),
+        HealpixPixel(1, 45),
+        HealpixPixel(1, 46),
+        HealpixPixel(1, 47),
+    ]
+
+
+def test_margin_filter_invalid_size(margin_catalog_info, margin_catalog_pixels):
+    margin_catalog_info.margin_threshold = 10000000
+    catalog = MarginCatalog(margin_catalog_info, margin_catalog_pixels)
+    pixels = [HealpixPixel(1, 44)]
+    with pytest.raises(ValueError, match="greater than the size of a pixel"):
+        catalog.filter_from_pixel_list(pixels)
```

### Comparing `hipscat-0.3.3/tests/hipscat/catalog/source_catalog/test_source_catalog_info.py` & `hipscat-0.3.4/tests/hipscat/catalog/source_catalog/test_source_catalog_info.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.3/tests/hipscat/catalog/test_catalog.py` & `hipscat-0.3.4/tests/hipscat/catalog/test_catalog.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 """Tests of catalog functionality"""
 
 import os
 
+import astropy.units as u
 import healpy as hp
 import numpy as np
 import pytest
+from mocpy import MOC
 
 from hipscat.catalog import Catalog, CatalogType, PartitionInfo
 from hipscat.io import paths
 from hipscat.io.file_io import read_fits_image
 from hipscat.loaders import read_from_hipscat
 from hipscat.pixel_math import HealpixPixel
-from hipscat.pixel_math.box_filter import _generate_ra_strip_pixel_tree
+from hipscat.pixel_math.box_filter import _generate_ra_strip_moc, generate_box_moc
 from hipscat.pixel_math.validators import ValidatorsErrors
 from hipscat.pixel_tree.pixel_tree import PixelTree
 
 
 def test_catalog_load(catalog_info, catalog_pixels):
     catalog = Catalog(catalog_info, catalog_pixels)
     assert catalog.get_healpix_pixels() == catalog_pixels
@@ -112,24 +114,56 @@
     cat = read_from_hipscat(small_sky_source_dir)
 
     assert isinstance(cat, Catalog)
     assert cat.catalog_name == "small_sky_source"
     assert len(cat.get_healpix_pixels()) == 14
 
 
+def test_max_coverage_order(small_sky_order1_catalog):
+    assert small_sky_order1_catalog.get_max_coverage_order() >= small_sky_order1_catalog.moc.max_order
+    assert (
+        small_sky_order1_catalog.get_max_coverage_order()
+        >= small_sky_order1_catalog.pixel_tree.get_max_depth()
+    )
+    high_moc_order = 8
+    test_moc = MOC.from_depth29_ranges(
+        max_depth=high_moc_order, ranges=small_sky_order1_catalog.moc.to_depth29_ranges
+    )
+    small_sky_order1_catalog.moc = test_moc
+    assert small_sky_order1_catalog.get_max_coverage_order() == high_moc_order
+    small_sky_order1_catalog.moc = None
+    assert (
+        small_sky_order1_catalog.get_max_coverage_order()
+        == small_sky_order1_catalog.pixel_tree.get_max_depth()
+    )
+
+
 def test_cone_filter(small_sky_order1_catalog):
-    filtered_catalog = small_sky_order1_catalog.filter_by_cone(315, -66.443, 0.1)
+    ra = 315
+    dec = -66.443
+    radius = 0.1
+
+    filtered_catalog = small_sky_order1_catalog.filter_by_cone(ra, dec, radius)
     filtered_pixels = filtered_catalog.get_healpix_pixels()
 
     assert len(filtered_pixels) == 1
     assert filtered_pixels == [HealpixPixel(1, 44)]
 
     assert (1, 44) in filtered_catalog.pixel_tree
     assert filtered_catalog.catalog_info.total_rows is None
 
+    assert filtered_catalog.moc is not None
+    cone_moc = MOC.from_cone(
+        lon=ra * u.deg,
+        lat=dec * u.deg,
+        radius=radius * u.arcsec,
+        max_depth=small_sky_order1_catalog.get_max_coverage_order(),
+    )
+    assert filtered_catalog.moc == cone_moc.intersection(small_sky_order1_catalog.moc)
+
 
 def test_cone_filter_big(small_sky_order1_catalog):
     filtered_catalog = small_sky_order1_catalog.filter_by_cone(315, -66.443, 30 * 3600)
     assert len(filtered_catalog.get_healpix_pixels()) == 4
     assert (1, 44) in filtered_catalog.pixel_tree
     assert (1, 45) in filtered_catalog.pixel_tree
     assert (1, 46) in filtered_catalog.pixel_tree
@@ -167,14 +201,22 @@
     polygon_vertices = [(282, -58), (282, -55), (272, -55), (272, -58)]
     filtered_catalog = small_sky_order1_catalog.filter_by_polygon(polygon_vertices)
     filtered_pixels = filtered_catalog.get_healpix_pixels()
     assert len(filtered_pixels) == 1
     assert filtered_pixels == [HealpixPixel(1, 46)]
     assert (1, 46) in filtered_catalog.pixel_tree
     assert filtered_catalog.catalog_info.total_rows is None
+    assert filtered_catalog.moc is not None
+    ra, dec = np.array(polygon_vertices).T
+    polygon_moc = MOC.from_polygon(
+        lon=ra * u.deg,
+        lat=dec * u.deg,
+        max_depth=small_sky_order1_catalog.get_max_coverage_order(),
+    )
+    assert filtered_catalog.moc == polygon_moc.intersection(small_sky_order1_catalog.moc)
 
 
 def test_polygonal_filter_with_cartesian_coordinates(small_sky_order1_catalog):
     sky_vertices = [(282, -58), (282, -55), (272, -55), (272, -58)]
     cartesian_vertices = hp.ang2vec(*np.array(sky_vertices).T, lonlat=True)
     filtered_catalog_1 = small_sky_order1_catalog.filter_by_polygon(sky_vertices)
     filtered_catalog_2 = small_sky_order1_catalog.filter_by_polygon(cartesian_vertices)
@@ -237,27 +279,32 @@
         small_sky_order1_catalog.filter_by_polygon(vertices)
     with pytest.raises(ValueError, match=ValidatorsErrors.DEGENERATE_POLYGON):
         vertices = [(50.1, 0), (100.1, 0), (150.1, 0), (200.1, 0)]
         small_sky_order1_catalog.filter_by_polygon(vertices)
 
 
 def test_box_filter_ra(small_sky_order1_catalog):
+    ra = (280, 290)
     # The catalog pixels are distributed around the [270,0] degree range.
-    filtered_catalog = small_sky_order1_catalog.filter_by_box(ra=(280, 290))
+    filtered_catalog = small_sky_order1_catalog.filter_by_box(ra=ra)
 
     filtered_pixels = filtered_catalog.get_healpix_pixels()
 
     assert len(filtered_pixels) == 2
     assert filtered_pixels == [HealpixPixel(1, 44), HealpixPixel(1, 46)]
 
     assert (1, 44) in filtered_catalog.pixel_tree
     assert (1, 46) in filtered_catalog.pixel_tree
     assert len(filtered_catalog.pixel_tree.pixels[1]) == 2
     assert filtered_catalog.catalog_info.total_rows is None
 
+    assert filtered_catalog.moc is not None
+    box_moc = generate_box_moc(ra=ra, dec=None, order=small_sky_order1_catalog.get_max_coverage_order())
+    assert filtered_catalog.moc == box_moc.intersection(small_sky_order1_catalog.moc)
+
 
 def test_box_filter_wrapped_ra(small_sky_order1_catalog):
     # The catalog pixels are distributed around the [270,0] degree range.
     filtered_catalog = small_sky_order1_catalog.filter_by_box(ra=(-10, 10))
 
     filtered_pixels = filtered_catalog.get_healpix_pixels()
 
@@ -304,33 +351,33 @@
     filtered_catalog_complement = small_sky_order1_catalog.filter_by_box(ra=(200, 50))
     assert_is_subset_of(filtered_catalog, filtered_catalog_complement)
 
 
 def test_box_filter_ra_pixel_tree_generation():
     """This method tests the pixel tree generation for the ra filter"""
     # The catalog pixels are distributed around the [270,0] degree range.
-    pixel_tree = _generate_ra_strip_pixel_tree(ra_range=(0, 180), order=1)
-    pixel_tree_complement = _generate_ra_strip_pixel_tree(ra_range=(180, 0), order=1)
-    assert len(pixel_tree) == len(pixel_tree_complement)
-
-    pixel_tree = _generate_ra_strip_pixel_tree(ra_range=(10, 50), order=1)
-    pixel_tree_complement = _generate_ra_strip_pixel_tree(ra_range=(50, 10), order=1)
-    assert len(pixel_tree) < len(pixel_tree_complement)
-
-    pixel_tree = _generate_ra_strip_pixel_tree(ra_range=(10, 220), order=1)
-    pixel_tree_complement = _generate_ra_strip_pixel_tree(ra_range=(220, 10), order=1)
-    assert len(pixel_tree_complement) < len(pixel_tree)
-
-    pixel_tree = _generate_ra_strip_pixel_tree(ra_range=(200, 350), order=1)
-    pixel_tree_complement = _generate_ra_strip_pixel_tree(ra_range=(350, 200), order=1)
-    assert len(pixel_tree) < len(pixel_tree_complement)
-
-    pixel_tree = _generate_ra_strip_pixel_tree(ra_range=(200, 50), order=1)
-    pixel_tree_complement = _generate_ra_strip_pixel_tree(ra_range=(50, 200), order=1)
-    assert len(pixel_tree_complement) < len(pixel_tree)
+    moc = _generate_ra_strip_moc(ra_range=(0, 180), order=1)
+    moc_complement = _generate_ra_strip_moc(ra_range=(180, 0), order=1)
+    assert len(moc.flatten()) == len(moc_complement.flatten())
+
+    moc = _generate_ra_strip_moc(ra_range=(10, 50), order=1)
+    moc_complement = _generate_ra_strip_moc(ra_range=(50, 10), order=1)
+    assert len(moc.flatten()) < len(moc_complement.flatten())
+
+    moc = _generate_ra_strip_moc(ra_range=(10, 220), order=1)
+    moc_complement = _generate_ra_strip_moc(ra_range=(220, 10), order=1)
+    assert len(moc_complement.flatten()) < len(moc.flatten())
+
+    moc = _generate_ra_strip_moc(ra_range=(200, 350), order=1)
+    moc_complement = _generate_ra_strip_moc(ra_range=(350, 200), order=1)
+    assert len(moc.flatten()) < len(moc_complement.flatten())
+
+    moc = _generate_ra_strip_moc(ra_range=(200, 50), order=1)
+    moc_complement = _generate_ra_strip_moc(ra_range=(50, 200), order=1)
+    assert len(moc_complement.flatten()) < len(moc.flatten())
 
 
 def test_box_filter_dec(small_sky_order1_catalog):
     # The catalog pixels are distributed around the [-90,0] degree range.
     filtered_catalog = small_sky_order1_catalog.filter_by_box(dec=(10, 20))
     assert len(filtered_catalog.get_healpix_pixels()) == 0
     assert len(filtered_catalog.pixel_tree) == 0
```

### Comparing `hipscat-0.3.3/tests/hipscat/catalog/test_catalog_info.py` & `hipscat-0.3.4/tests/hipscat/catalog/test_catalog_info.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.3/tests/hipscat/catalog/test_partition_info.py` & `hipscat-0.3.4/tests/hipscat/catalog/test_partition_info.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.3/tests/hipscat/conftest.py` & `hipscat-0.3.4/tests/hipscat/conftest.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.3/tests/hipscat/inspection/test_almanac.py` & `hipscat-0.3.4/tests/hipscat/inspection/test_almanac.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.3/tests/hipscat/inspection/test_almanac_info.py` & `hipscat-0.3.4/tests/hipscat/inspection/test_almanac_info.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.3/tests/hipscat/inspection/test_visualize_catalog.py` & `hipscat-0.3.4/tests/hipscat/inspection/test_visualize_catalog.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.3/tests/hipscat/io/conftest.py` & `hipscat-0.3.4/tests/hipscat/io/conftest.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.3/tests/hipscat/io/file_io/test_file_io.py` & `hipscat-0.3.4/tests/hipscat/io/file_io/test_file_io.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.3/tests/hipscat/io/file_io/test_file_pointers.py` & `hipscat-0.3.4/tests/hipscat/io/file_io/test_file_pointers.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.3/tests/hipscat/io/test_parquet_metadata.py` & `hipscat-0.3.4/tests/hipscat/io/test_parquet_metadata.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.3/tests/hipscat/io/test_paths.py` & `hipscat-0.3.4/tests/hipscat/io/test_paths.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.3/tests/hipscat/io/test_validation.py` & `hipscat-0.3.4/tests/hipscat/io/test_validation.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.3/tests/hipscat/io/test_write_metadata.py` & `hipscat-0.3.4/tests/hipscat/io/test_write_metadata.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 """Tests of file IO (reads and writes)"""
 
 import os
 import shutil
 from pathlib import Path
 
+import healpy as hp
+import numpy as np
 import numpy.testing as npt
+import pytest
 
 import hipscat.io.write_metadata as io
 import hipscat.pixel_math as hist
 from hipscat.io import file_io
 from hipscat.pixel_math.healpix_pixel import HealpixPixel
 
 
@@ -23,24 +26,35 @@
         r'    "first_five_fib": \[',
         "        1,",
         "        1,",
         "        2,",
         "        3,",
         "        5",
         "    ]",
-        r'    "integer_type": "<class \'int\'>"',
+        r'    "integer_type": "<class \'int\'>",',
+        '    "np_int": 5000000,',
+        '    "np_float": 1.618,',
+        '    "pixel": "Order: 5, Pixel: 9000",',
+        r'    "pixels": \[',
+        '        "Order: 5, Pixel: 9000",',
+        '        "Order: 5, Pixel: 9001"',
+        "    ]",
         "}",
     ]
 
     dictionary = {}
     dictionary["first_english"] = "a"
     dictionary["first_greek"] = "alpha"
     dictionary["first_number"] = 1
     dictionary["first_five_fib"] = [1, 1, 2, 3, 5]
     dictionary["integer_type"] = int
+    dictionary["np_int"] = np.uint64(5_000_000)
+    dictionary["np_float"] = np.float64(1.618)
+    dictionary["pixel"] = HealpixPixel(5, 9_000)
+    dictionary["pixels"] = np.array([HealpixPixel(5, 9_000), HealpixPixel(5, 9_001)])
 
     json_filename = os.path.join(tmp_path, "dictionary.json")
     io.write_json_file(dictionary, json_filename)
     assert_text_file_matches(expected_lines, json_filename)
 
 
 def test_write_json_paths(assert_text_file_matches, tmp_path):
@@ -200,7 +214,30 @@
     initial_histogram[44:] = filled_pixels[:]
     io.write_fits_map(tmp_path, initial_histogram)
 
     output_file = os.path.join(tmp_path, "point_map.fits")
 
     output = file_io.read_fits_image(output_file)
     npt.assert_array_equal(output, initial_histogram)
+
+    # Check the metadata of the fits file:
+    map_fits_image = hp.read_map(output_file, nest=True, h=True)
+
+    header_dict = dict(map_fits_image[1])
+    assert header_dict["ORDERING"] == "NESTED"
+    assert header_dict["PIXTYPE"] == "HEALPIX"
+    assert header_dict["NSIDE"] == 2
+
+    npt.assert_array_equal(initial_histogram, map_fits_image[0])
+
+
+def test_read_ring_fits_point_map(tmp_path):
+    """Check that we write and can read a FITS file for spatial distribution."""
+    output_file = os.path.join(tmp_path, "point_map.fits")
+    initial_histogram = hist.empty_histogram(1)
+    filled_pixels = [51, 29, 51, 0]
+    initial_histogram[44:] = filled_pixels[:]
+    hp.write_map(output_file, initial_histogram, dtype=np.int64)
+
+    with pytest.warns(UserWarning, match="/hipscat/issues/271"):
+        output = file_io.read_fits_image(output_file)
+        npt.assert_array_equal(output, initial_histogram)
```

### Comparing `hipscat-0.3.3/tests/hipscat/pixel_math/test_healpix_pixel.py` & `hipscat-0.3.4/tests/hipscat/pixel_math/test_healpix_pixel.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.3/tests/hipscat/pixel_math/test_healpix_pixel_convertor.py` & `hipscat-0.3.4/tests/hipscat/pixel_math/test_healpix_pixel_convertor.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.3/tests/hipscat/pixel_math/test_healpix_pixel_function.py` & `hipscat-0.3.4/tests/hipscat/pixel_math/test_healpix_pixel_function.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.3/tests/hipscat/pixel_math/test_hipscat_id.py` & `hipscat-0.3.4/tests/hipscat/pixel_math/test_hipscat_id.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.3/tests/hipscat/pixel_math/test_margin_bounding.py` & `hipscat-0.3.4/tests/hipscat/pixel_math/test_margin_bounding.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.3/tests/hipscat/pixel_math/test_partition_stats.py` & `hipscat-0.3.4/tests/hipscat/pixel_math/test_partition_stats.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.3/tests/hipscat/pixel_math/test_pixel_margins.py` & `hipscat-0.3.4/tests/hipscat/pixel_math/test_pixel_margins.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.3/tests/hipscat/pixel_tree/conftest.py` & `hipscat-0.3.4/tests/hipscat/pixel_tree/conftest.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.3/tests/hipscat/pixel_tree/test_moc_filter.py` & `hipscat-0.3.4/tests/hipscat/pixel_tree/test_moc_filter.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.3/tests/hipscat/pixel_tree/test_pixel_alignment.py` & `hipscat-0.3.4/tests/hipscat/pixel_tree/test_pixel_alignment.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.3/tests/hipscat/pixel_tree/test_pixel_tree.py` & `hipscat-0.3.4/tests/hipscat/pixel_tree/test_pixel_tree.py`

 * *Files identical despite different names*

### Comparing `hipscat-0.3.3/tests/hipscat/pixel_tree/test_pixel_tree_builder.py` & `hipscat-0.3.4/tests/hipscat/pixel_tree/test_pixel_tree_builder.py`

 * *Files identical despite different names*

