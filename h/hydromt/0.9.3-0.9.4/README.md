# Comparing `tmp/hydromt-0.9.3.tar.gz` & `tmp/hydromt-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hydromt-0.9.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "hydromt-0.9.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `hydromt-0.9.3.tar` & `hydromt-0.9.4.tar`

### file list

```diff
@@ -1,82 +1,81 @@
--rw-r--r--   0        0        0       18 2024-02-08 10:42:17.987605 hydromt-0.9.3/.act_event.json
--rw-r--r--   0        0        0      164 2024-02-08 10:42:17.987605 hydromt-0.9.3/.actrc
--rw-r--r--   0        0        0      626 2024-02-08 10:42:17.987605 hydromt-0.9.3/.binder/Dockerfile
--rw-r--r--   0        0        0       12 2024-02-08 10:42:17.987605 hydromt-0.9.3/.dockerignore
--rw-r--r--   0        0        0       62 2024-02-08 10:42:17.987605 hydromt-0.9.3/.gitattributes
--rw-r--r--   0        0        0     1507 2024-02-08 10:42:17.987605 hydromt-0.9.3/.gitignore
--rw-r--r--   0        0        0      658 2024-02-08 10:42:17.987605 hydromt-0.9.3/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1833 2024-02-08 10:42:17.987605 hydromt-0.9.3/.zenodo.json
--rw-r--r--   0        0        0     5216 2024-02-08 10:42:17.987605 hydromt-0.9.3/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0      190 2024-02-08 10:42:17.987605 hydromt-0.9.3/CONTRIBUTING.rst
--rw-r--r--   0        0        0     2987 2024-02-08 10:42:17.987605 hydromt-0.9.3/Dockerfile
--rw-r--r--   0        0        0     1075 2024-02-08 10:42:17.987605 hydromt-0.9.3/LICENSE
--rw-r--r--   0        0        0     2049 2024-02-08 10:42:17.987605 hydromt-0.9.3/Makefile
--rw-r--r--   0        0        0     6083 2024-02-08 10:42:17.987605 hydromt-0.9.3/README.rst
--rw-r--r--   0        0        0     2642 2024-02-08 10:42:17.987605 hydromt-0.9.3/data/catalogs/README.rst
--rw-r--r--   0        0        0    22265 2024-02-08 10:42:17.987605 hydromt-0.9.3/data/catalogs/artifact_data.yml
--rw-r--r--   0        0        0      478 2024-02-08 10:42:17.987605 hydromt-0.9.3/data/catalogs/aws_data.yml
--rw-r--r--   0        0        0     2046 2024-02-08 10:42:17.987605 hydromt-0.9.3/data/catalogs/changelog.rst
--rw-r--r--   0        0        0    50664 2024-02-08 10:42:17.987605 hydromt-0.9.3/data/catalogs/deltares_data.yml
--rw-r--r--   0        0        0    11316 2024-02-08 10:42:17.987605 hydromt-0.9.3/data/catalogs/gcs_cmip6_data.yml
--rw-r--r--   0        0        0     4686 2024-02-08 10:42:17.987605 hydromt-0.9.3/data/catalogs/test_data_catalog.py
--rw-r--r--   0        0        0     2039 2024-02-08 10:42:17.987605 hydromt-0.9.3/data/predefined_catalogs.yml
--rw-r--r--   0        0        0     5241 2024-02-08 10:42:17.987605 hydromt-0.9.3/data/src/chirps_download_convert.py
--rw-r--r--   0        0        0    25042 2024-02-08 10:42:17.987605 hydromt-0.9.3/data/src/era5_download_resample_convert.py
--rw-r--r--   0        0        0       59 2024-02-08 10:42:17.987605 hydromt-0.9.3/diff_latest_release.sh
--rw-r--r--   0        0        0      592 2024-02-08 10:42:18.027606 hydromt-0.9.3/hydromt/__init__.py
--rw-r--r--   0        0        0     1190 2024-02-08 10:42:18.027606 hydromt-0.9.3/hydromt/_compat.py
--rw-r--r--   0        0        0       71 2024-02-08 10:42:18.027606 hydromt-0.9.3/hydromt/cli/__init__.py
--rw-r--r--   0        0        0     6092 2024-02-08 10:42:18.027606 hydromt-0.9.3/hydromt/cli/api.py
--rw-r--r--   0        0        0     3839 2024-02-08 10:42:18.027606 hydromt-0.9.3/hydromt/cli/cli_utils.py
--rw-r--r--   0        0        0    18768 2024-02-08 10:42:18.027606 hydromt-0.9.3/hydromt/cli/main.py
--rw-r--r--   0        0        0     9836 2024-02-08 10:42:18.027606 hydromt-0.9.3/hydromt/config.py
--rw-r--r--   0        0        0      463 2024-02-08 10:42:18.027606 hydromt-0.9.3/hydromt/data_adapter/__init__.py
--rw-r--r--   0        0        0     3805 2024-02-08 10:42:18.027606 hydromt-0.9.3/hydromt/data_adapter/caching.py
--rw-r--r--   0        0        0    16035 2024-02-08 10:42:18.027606 hydromt-0.9.3/hydromt/data_adapter/data_adapter.py
--rw-r--r--   0        0        0    15573 2024-02-08 10:42:18.027606 hydromt-0.9.3/hydromt/data_adapter/dataframe.py
--rw-r--r--   0        0        0    17157 2024-02-08 10:42:18.027606 hydromt-0.9.3/hydromt/data_adapter/dataset.py
--rw-r--r--   0        0        0    22424 2024-02-08 10:42:18.027606 hydromt-0.9.3/hydromt/data_adapter/geodataframe.py
--rw-r--r--   0        0        0    26407 2024-02-08 10:42:18.027606 hydromt-0.9.3/hydromt/data_adapter/geodataset.py
--rw-r--r--   0        0        0    37395 2024-02-08 10:42:18.027606 hydromt-0.9.3/hydromt/data_adapter/rasterdataset.py
--rw-r--r--   0        0        0     2938 2024-02-08 10:42:18.027606 hydromt-0.9.3/hydromt/data_adapter/utils.py
--rw-r--r--   0        0        0    76290 2024-02-08 10:42:18.027606 hydromt-0.9.3/hydromt/data_catalog.py
--rw-r--r--   0        0        0      375 2024-02-08 10:42:18.027606 hydromt-0.9.3/hydromt/error.py
--rw-r--r--   0        0        0      318 2024-02-08 10:42:18.027606 hydromt-0.9.3/hydromt/exceptions.py
--rw-r--r--   0        0        0    30036 2024-02-08 10:42:18.027606 hydromt-0.9.3/hydromt/flw.py
--rw-r--r--   0        0        0    21092 2024-02-08 10:42:18.027606 hydromt-0.9.3/hydromt/gis_utils.py
--rw-r--r--   0        0        0    29003 2024-02-08 10:42:18.027606 hydromt-0.9.3/hydromt/io.py
--rw-r--r--   0        0        0     3131 2024-02-08 10:42:18.027606 hydromt-0.9.3/hydromt/log.py
--rw-r--r--   0        0        0     8282 2024-02-08 10:42:18.027606 hydromt-0.9.3/hydromt/merge.py
--rw-r--r--   0        0        0      410 2024-02-08 10:42:18.027606 hydromt-0.9.3/hydromt/models/__init__.py
--rw-r--r--   0        0        0    77011 2024-02-08 10:42:18.027606 hydromt-0.9.3/hydromt/models/model_api.py
--rw-r--r--   0        0        0    29650 2024-02-08 10:42:18.027606 hydromt-0.9.3/hydromt/models/model_grid.py
--rw-r--r--   0        0        0    26907 2024-02-08 10:42:18.027606 hydromt-0.9.3/hydromt/models/model_mesh.py
--rw-r--r--   0        0        0     2732 2024-02-08 10:42:18.027606 hydromt-0.9.3/hydromt/models/model_network.py
--rw-r--r--   0        0        0     5623 2024-02-08 10:42:18.027606 hydromt-0.9.3/hydromt/models/model_plugins.py
--rw-r--r--   0        0        0    15985 2024-02-08 10:42:18.027606 hydromt-0.9.3/hydromt/models/model_vector.py
--rw-r--r--   0        0        0      610 2024-02-08 10:42:18.031606 hydromt-0.9.3/hydromt/nodata.py
--rw-r--r--   0        0        0   123464 2024-02-08 10:42:18.031606 hydromt-0.9.3/hydromt/raster.py
--rw-r--r--   0        0        0      126 2024-02-08 10:42:18.031606 hydromt-0.9.3/hydromt/stats/__init__.py
--rw-r--r--   0        0        0     3974 2024-02-08 10:42:18.031606 hydromt-0.9.3/hydromt/stats/design_events.py
--rw-r--r--   0        0        0    30672 2024-02-08 10:42:18.031606 hydromt-0.9.3/hydromt/stats/extremes.py
--rw-r--r--   0        0        0    15597 2024-02-08 10:42:18.031606 hydromt-0.9.3/hydromt/stats/skills.py
--rw-r--r--   0        0        0     1347 2024-02-08 10:42:18.031606 hydromt-0.9.3/hydromt/typing.py
--rw-r--r--   0        0        0     2659 2024-02-08 10:42:18.031606 hydromt-0.9.3/hydromt/utils.py
--rw-r--r--   0        0        0      620 2024-02-08 10:42:18.031606 hydromt-0.9.3/hydromt/validators/__init__.py
--rw-r--r--   0        0        0     6570 2024-02-08 10:42:18.031606 hydromt-0.9.3/hydromt/validators/data_catalog.py
--rw-r--r--   0        0        0     2427 2024-02-08 10:42:18.031606 hydromt-0.9.3/hydromt/validators/model_config.py
--rw-r--r--   0        0        0     2990 2024-02-08 10:42:18.031606 hydromt-0.9.3/hydromt/validators/region.py
--rw-r--r--   0        0        0    36705 2024-02-08 10:42:18.031606 hydromt-0.9.3/hydromt/vector.py
--rw-r--r--   0        0        0      211 2024-02-08 10:42:18.031606 hydromt-0.9.3/hydromt/workflows/__init__.py
--rw-r--r--   0        0        0    19973 2024-02-08 10:42:18.031606 hydromt-0.9.3/hydromt/workflows/basin_mask.py
--rw-r--r--   0        0        0    27154 2024-02-08 10:42:18.031606 hydromt-0.9.3/hydromt/workflows/forcing.py
--rw-r--r--   0        0        0    13880 2024-02-08 10:42:18.031606 hydromt-0.9.3/hydromt/workflows/grid.py
--rw-r--r--   0        0        0    15606 2024-02-08 10:42:18.031606 hydromt-0.9.3/hydromt/workflows/mesh.py
--rw-r--r--   0        0        0     6708 2024-02-08 10:42:18.031606 hydromt-0.9.3/hydromt/workflows/rivers.py
--rw-r--r--   0        0        0      582 2024-02-08 10:42:18.031606 hydromt-0.9.3/joss_paper/citation.bib
--rw-r--r--   0        0        0    15299 2024-02-08 10:42:18.031606 hydromt-0.9.3/joss_paper/paper.bib
--rw-r--r--   0        0        0    12867 2024-02-08 10:42:18.031606 hydromt-0.9.3/joss_paper/paper.md
--rw-r--r--   0        0        0     3602 2024-02-08 10:42:18.031606 hydromt-0.9.3/make_env.py
--rw-r--r--   0        0        0     3307 2024-02-08 10:42:18.031606 hydromt-0.9.3/pixi.toml
--rw-r--r--   0        0        0     5804 2024-02-08 10:42:18.031606 hydromt-0.9.3/pyproject.toml
--rw-r--r--   0        0        0     9169 1970-01-01 00:00:00.000000 hydromt-0.9.3/PKG-INFO
+-rw-r--r--   0        0        0       18 2024-02-26 14:00:57.853769 hydromt-0.9.4/.act_event.json
+-rw-r--r--   0        0        0      164 2024-02-26 14:00:57.853769 hydromt-0.9.4/.actrc
+-rw-r--r--   0        0        0      626 2024-02-26 14:00:57.853769 hydromt-0.9.4/.binder/Dockerfile
+-rw-r--r--   0        0        0       12 2024-02-26 14:00:57.853769 hydromt-0.9.4/.dockerignore
+-rw-r--r--   0        0        0       62 2024-02-26 14:00:57.853769 hydromt-0.9.4/.gitattributes
+-rw-r--r--   0        0        0     1507 2024-02-26 14:00:57.857769 hydromt-0.9.4/.gitignore
+-rw-r--r--   0        0        0      658 2024-02-26 14:00:57.857769 hydromt-0.9.4/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1833 2024-02-26 14:00:57.857769 hydromt-0.9.4/.zenodo.json
+-rw-r--r--   0        0        0     5216 2024-02-26 14:00:57.857769 hydromt-0.9.4/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0      190 2024-02-26 14:00:57.857769 hydromt-0.9.4/CONTRIBUTING.rst
+-rw-r--r--   0        0        0     2987 2024-02-26 14:00:57.857769 hydromt-0.9.4/Dockerfile
+-rw-r--r--   0        0        0     1075 2024-02-26 14:00:57.857769 hydromt-0.9.4/LICENSE
+-rw-r--r--   0        0        0     2049 2024-02-26 14:00:57.857769 hydromt-0.9.4/Makefile
+-rw-r--r--   0        0        0     6083 2024-02-26 14:00:57.857769 hydromt-0.9.4/README.rst
+-rw-r--r--   0        0        0     2642 2024-02-26 14:00:57.857769 hydromt-0.9.4/data/catalogs/README.rst
+-rw-r--r--   0        0        0    22265 2024-02-26 14:00:57.857769 hydromt-0.9.4/data/catalogs/artifact_data.yml
+-rw-r--r--   0        0        0      478 2024-02-26 14:00:57.857769 hydromt-0.9.4/data/catalogs/aws_data.yml
+-rw-r--r--   0        0        0     2046 2024-02-26 14:00:57.857769 hydromt-0.9.4/data/catalogs/changelog.rst
+-rw-r--r--   0        0        0    50664 2024-02-26 14:00:57.857769 hydromt-0.9.4/data/catalogs/deltares_data.yml
+-rw-r--r--   0        0        0    11316 2024-02-26 14:00:57.857769 hydromt-0.9.4/data/catalogs/gcs_cmip6_data.yml
+-rw-r--r--   0        0        0     4686 2024-02-26 14:00:57.857769 hydromt-0.9.4/data/catalogs/test_data_catalog.py
+-rw-r--r--   0        0        0     2039 2024-02-26 14:00:57.857769 hydromt-0.9.4/data/predefined_catalogs.yml
+-rw-r--r--   0        0        0     5241 2024-02-26 14:00:57.857769 hydromt-0.9.4/data/src/chirps_download_convert.py
+-rw-r--r--   0        0        0    25042 2024-02-26 14:00:57.857769 hydromt-0.9.4/data/src/era5_download_resample_convert.py
+-rw-r--r--   0        0        0      592 2024-02-26 14:00:57.897769 hydromt-0.9.4/hydromt/__init__.py
+-rw-r--r--   0        0        0     1190 2024-02-26 14:00:57.897769 hydromt-0.9.4/hydromt/_compat.py
+-rw-r--r--   0        0        0       71 2024-02-26 14:00:57.897769 hydromt-0.9.4/hydromt/cli/__init__.py
+-rw-r--r--   0        0        0     6092 2024-02-26 14:00:57.897769 hydromt-0.9.4/hydromt/cli/api.py
+-rw-r--r--   0        0        0     3839 2024-02-26 14:00:57.897769 hydromt-0.9.4/hydromt/cli/cli_utils.py
+-rw-r--r--   0        0        0    18765 2024-02-26 14:00:57.897769 hydromt-0.9.4/hydromt/cli/main.py
+-rw-r--r--   0        0        0     9836 2024-02-26 14:00:57.897769 hydromt-0.9.4/hydromt/config.py
+-rw-r--r--   0        0        0      463 2024-02-26 14:00:57.897769 hydromt-0.9.4/hydromt/data_adapter/__init__.py
+-rw-r--r--   0        0        0     3805 2024-02-26 14:00:57.897769 hydromt-0.9.4/hydromt/data_adapter/caching.py
+-rw-r--r--   0        0        0    16035 2024-02-26 14:00:57.897769 hydromt-0.9.4/hydromt/data_adapter/data_adapter.py
+-rw-r--r--   0        0        0    15573 2024-02-26 14:00:57.897769 hydromt-0.9.4/hydromt/data_adapter/dataframe.py
+-rw-r--r--   0        0        0    17157 2024-02-26 14:00:57.897769 hydromt-0.9.4/hydromt/data_adapter/dataset.py
+-rw-r--r--   0        0        0    22424 2024-02-26 14:00:57.897769 hydromt-0.9.4/hydromt/data_adapter/geodataframe.py
+-rw-r--r--   0        0        0    26407 2024-02-26 14:00:57.897769 hydromt-0.9.4/hydromt/data_adapter/geodataset.py
+-rw-r--r--   0        0        0    37484 2024-02-26 14:00:57.897769 hydromt-0.9.4/hydromt/data_adapter/rasterdataset.py
+-rw-r--r--   0        0        0     2938 2024-02-26 14:00:57.897769 hydromt-0.9.4/hydromt/data_adapter/utils.py
+-rw-r--r--   0        0        0    76290 2024-02-26 14:00:57.897769 hydromt-0.9.4/hydromt/data_catalog.py
+-rw-r--r--   0        0        0      375 2024-02-26 14:00:57.897769 hydromt-0.9.4/hydromt/error.py
+-rw-r--r--   0        0        0      318 2024-02-26 14:00:57.897769 hydromt-0.9.4/hydromt/exceptions.py
+-rw-r--r--   0        0        0    30036 2024-02-26 14:00:57.897769 hydromt-0.9.4/hydromt/flw.py
+-rw-r--r--   0        0        0    21092 2024-02-26 14:00:57.897769 hydromt-0.9.4/hydromt/gis_utils.py
+-rw-r--r--   0        0        0    29014 2024-02-26 14:00:57.897769 hydromt-0.9.4/hydromt/io.py
+-rw-r--r--   0        0        0     3131 2024-02-26 14:00:57.897769 hydromt-0.9.4/hydromt/log.py
+-rw-r--r--   0        0        0     8282 2024-02-26 14:00:57.897769 hydromt-0.9.4/hydromt/merge.py
+-rw-r--r--   0        0        0      410 2024-02-26 14:00:57.897769 hydromt-0.9.4/hydromt/models/__init__.py
+-rw-r--r--   0        0        0    77011 2024-02-26 14:00:57.897769 hydromt-0.9.4/hydromt/models/model_api.py
+-rw-r--r--   0        0        0    29650 2024-02-26 14:00:57.897769 hydromt-0.9.4/hydromt/models/model_grid.py
+-rw-r--r--   0        0        0    26907 2024-02-26 14:00:57.897769 hydromt-0.9.4/hydromt/models/model_mesh.py
+-rw-r--r--   0        0        0     2732 2024-02-26 14:00:57.897769 hydromt-0.9.4/hydromt/models/model_network.py
+-rw-r--r--   0        0        0     5623 2024-02-26 14:00:57.897769 hydromt-0.9.4/hydromt/models/model_plugins.py
+-rw-r--r--   0        0        0    15985 2024-02-26 14:00:57.901769 hydromt-0.9.4/hydromt/models/model_vector.py
+-rw-r--r--   0        0        0      610 2024-02-26 14:00:57.901769 hydromt-0.9.4/hydromt/nodata.py
+-rw-r--r--   0        0        0   123464 2024-02-26 14:00:57.901769 hydromt-0.9.4/hydromt/raster.py
+-rw-r--r--   0        0        0      126 2024-02-26 14:00:57.901769 hydromt-0.9.4/hydromt/stats/__init__.py
+-rw-r--r--   0        0        0     3974 2024-02-26 14:00:57.901769 hydromt-0.9.4/hydromt/stats/design_events.py
+-rw-r--r--   0        0        0    30672 2024-02-26 14:00:57.901769 hydromt-0.9.4/hydromt/stats/extremes.py
+-rw-r--r--   0        0        0    15597 2024-02-26 14:00:57.901769 hydromt-0.9.4/hydromt/stats/skills.py
+-rw-r--r--   0        0        0     1347 2024-02-26 14:00:57.901769 hydromt-0.9.4/hydromt/typing.py
+-rw-r--r--   0        0        0     2659 2024-02-26 14:00:57.901769 hydromt-0.9.4/hydromt/utils.py
+-rw-r--r--   0        0        0      620 2024-02-26 14:00:57.901769 hydromt-0.9.4/hydromt/validators/__init__.py
+-rw-r--r--   0        0        0     6570 2024-02-26 14:00:57.901769 hydromt-0.9.4/hydromt/validators/data_catalog.py
+-rw-r--r--   0        0        0     2427 2024-02-26 14:00:57.901769 hydromt-0.9.4/hydromt/validators/model_config.py
+-rw-r--r--   0        0        0     2990 2024-02-26 14:00:57.901769 hydromt-0.9.4/hydromt/validators/region.py
+-rw-r--r--   0        0        0    36705 2024-02-26 14:00:57.901769 hydromt-0.9.4/hydromt/vector.py
+-rw-r--r--   0        0        0      211 2024-02-26 14:00:57.901769 hydromt-0.9.4/hydromt/workflows/__init__.py
+-rw-r--r--   0        0        0    19973 2024-02-26 14:00:57.901769 hydromt-0.9.4/hydromt/workflows/basin_mask.py
+-rw-r--r--   0        0        0    27154 2024-02-26 14:00:57.901769 hydromt-0.9.4/hydromt/workflows/forcing.py
+-rw-r--r--   0        0        0    13880 2024-02-26 14:00:57.901769 hydromt-0.9.4/hydromt/workflows/grid.py
+-rw-r--r--   0        0        0    15606 2024-02-26 14:00:57.901769 hydromt-0.9.4/hydromt/workflows/mesh.py
+-rw-r--r--   0        0        0     6708 2024-02-26 14:00:57.901769 hydromt-0.9.4/hydromt/workflows/rivers.py
+-rw-r--r--   0        0        0      582 2024-02-26 14:00:57.901769 hydromt-0.9.4/joss_paper/citation.bib
+-rw-r--r--   0        0        0    15299 2024-02-26 14:00:57.901769 hydromt-0.9.4/joss_paper/paper.bib
+-rw-r--r--   0        0        0    12867 2024-02-26 14:00:57.901769 hydromt-0.9.4/joss_paper/paper.md
+-rw-r--r--   0        0        0     3602 2024-02-26 14:00:57.901769 hydromt-0.9.4/make_env.py
+-rw-r--r--   0        0        0     3307 2024-02-26 14:00:57.901769 hydromt-0.9.4/pixi.toml
+-rw-r--r--   0        0        0     5864 2024-02-26 14:00:57.901769 hydromt-0.9.4/pyproject.toml
+-rw-r--r--   0        0        0     9214 1970-01-01 00:00:00.000000 hydromt-0.9.4/PKG-INFO
```

### Comparing `hydromt-0.9.3/.binder/Dockerfile` & `hydromt-0.9.4/.binder/Dockerfile`

 * *Files identical despite different names*

### Comparing `hydromt-0.9.3/.gitignore` & `hydromt-0.9.4/.gitignore`

 * *Files identical despite different names*

### Comparing `hydromt-0.9.3/.pre-commit-config.yaml` & `hydromt-0.9.4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `hydromt-0.9.3/.zenodo.json` & `hydromt-0.9.4/.zenodo.json`

 * *Files identical despite different names*

### Comparing `hydromt-0.9.3/CODE_OF_CONDUCT.md` & `hydromt-0.9.4/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `hydromt-0.9.3/Dockerfile` & `hydromt-0.9.4/Dockerfile`

 * *Files identical despite different names*

### Comparing `hydromt-0.9.3/LICENSE` & `hydromt-0.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `hydromt-0.9.3/Makefile` & `hydromt-0.9.4/Makefile`

 * *Files identical despite different names*

### Comparing `hydromt-0.9.3/README.rst` & `hydromt-0.9.4/README.rst`

 * *Files identical despite different names*

### Comparing `hydromt-0.9.3/data/catalogs/README.rst` & `hydromt-0.9.4/data/catalogs/README.rst`

 * *Files identical despite different names*

### Comparing `hydromt-0.9.3/data/catalogs/artifact_data.yml` & `hydromt-0.9.4/data/catalogs/artifact_data.yml`

 * *Files identical despite different names*

### Comparing `hydromt-0.9.3/data/catalogs/changelog.rst` & `hydromt-0.9.4/data/catalogs/changelog.rst`

 * *Files identical despite different names*

### Comparing `hydromt-0.9.3/data/catalogs/deltares_data.yml` & `hydromt-0.9.4/data/catalogs/deltares_data.yml`

 * *Files identical despite different names*

### Comparing `hydromt-0.9.3/data/catalogs/gcs_cmip6_data.yml` & `hydromt-0.9.4/data/catalogs/gcs_cmip6_data.yml`

 * *Files identical despite different names*

### Comparing `hydromt-0.9.3/data/catalogs/test_data_catalog.py` & `hydromt-0.9.4/data/catalogs/test_data_catalog.py`

 * *Files identical despite different names*

### Comparing `hydromt-0.9.3/data/predefined_catalogs.yml` & `hydromt-0.9.4/data/predefined_catalogs.yml`

 * *Files identical despite different names*

### Comparing `hydromt-0.9.3/data/src/chirps_download_convert.py` & `hydromt-0.9.4/data/src/chirps_download_convert.py`

 * *Files identical despite different names*

### Comparing `hydromt-0.9.3/data/src/era5_download_resample_convert.py` & `hydromt-0.9.4/data/src/era5_download_resample_convert.py`

 * *Files identical despite different names*

### Comparing `hydromt-0.9.3/hydromt/__init__.py` & `hydromt-0.9.4/hydromt/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """HydroMT: Automated and reproducible model building and analysis."""
 
 # version number without 'v' at start
-__version__ = "0.9.3"
+__version__ = "0.9.4"
 
 # pkg_resource deprication warnings originate from dependencies
 # so silence them for now
 import warnings
 
 warnings.filterwarnings("ignore", category=DeprecationWarning)
```

### Comparing `hydromt-0.9.3/hydromt/_compat.py` & `hydromt-0.9.4/hydromt/_compat.py`

 * *Files identical despite different names*

### Comparing `hydromt-0.9.3/hydromt/cli/api.py` & `hydromt-0.9.4/hydromt/cli/api.py`

 * *Files identical despite different names*

### Comparing `hydromt-0.9.3/hydromt/cli/cli_utils.py` & `hydromt-0.9.4/hydromt/cli/cli_utils.py`

 * *Files identical despite different names*

### Comparing `hydromt-0.9.3/hydromt/cli/main.py` & `hydromt-0.9.4/hydromt/cli/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -66,18 +66,14 @@
     "export_dest_path",
     type=click.Path(resolve_path=True, dir_okay=True, file_okay=False),
 )
 arg_root = click.argument(
     "MODEL_ROOT",
     type=click.Path(resolve_path=True, dir_okay=True, file_okay=False),
 )
-arg_baseroot = click.argument(
-    "BASEMODEL_ROOT",
-    type=click.Path(resolve_path=True, dir_okay=True, file_okay=False),
-)
 
 region_opt = click.option(
     "-r",
     "--region",
     type=str,
     default="{}",
     callback=cli_utils.parse_json,
@@ -133,21 +129,21 @@
     help="Flag: If provided cache tiled rasterdatasets",
 )
 
 ## MAIN
 
 
 @click.group()
-@click.version_option(__version__, message="hydroMT version: %(version)s")
+@click.version_option(__version__, message="HydroMT version: %(version)s")
 @click.option(
     "--models",
     default=False,
     is_flag=True,
     is_eager=True,
-    help="Print availabe model plugins and exit.",
+    help="Print available model plugins and exit.",
     callback=print_models,
 )
 @click.pass_context
 def main(ctx, models):  # , quiet, verbose):
     """Command line interface for hydromt models."""
     if ctx.obj is None:
         ctx.obj = {}
@@ -187,18 +183,18 @@
     """Build models from scratch.
 
     Example usage:
     --------------
 
     To build a wflow model for a subbasin using a point coordinates snapped to cells
     with upstream area >= 50 km2
-    hydromt build wflow /path/to/model_root -i /path/to/wflow_config.ini  -r "{'subbasin': [-7.24, 62.09], 'uparea': 50}" -d deltares_data -d /path/to/data_catalog.yml -v
+    hydromt build wflow /path/to/model_root -i /path/to/wflow_config.yml  -r "{'subbasin': [-7.24, 62.09], 'uparea': 50}" -d deltares_data -d /path/to/data_catalog.yml -v
 
     To build a sfincs model based on a bbox
-    hydromt build sfincs /path/to/model_root  -i /path/to/sfincs_config.ini  -r "{'bbox': [4.6891,52.9750,4.9576,53.1994]}"  -d /path/to/data_catalog.yml -v
+    hydromt build sfincs /path/to/model_root  -i /path/to/sfincs_config.yml  -r "{'bbox': [4.6891,52.9750,4.9576,53.1994]}"  -d /path/to/data_catalog.yml -v
 
     """  # noqa: E501
     log_level = max(10, 30 - 10 * (verbose - quiet))
     logger = log.setuplog(
         "build", join(model_root, "hydromt.log"), log_level=log_level, append=False
     )
     logger.info(f"Building instance of {model} model at {model_root}.")
@@ -253,15 +249,15 @@
     callback=lambda c, p, v: v if v else c.params["model_root"],
 )
 @opt_config
 @click.option(
     "-c",
     "--components",
     multiple=True,
-    help="Model methods from ini file to run",
+    help="Model methods from configuration file to run",
 )
 @opt_cli
 @data_opt
 @deltares_data_opt
 @overwrite_opt
 @cache_opt
 @quiet_opt
@@ -289,17 +285,17 @@
 
     Example usage:
     --------------
 
     Update (overwrite!) landuse-landcover based maps in a Wflow model:
     hydromt update wflow /path/to/model_root -c setup_lulcmaps --opt lulc_fn=vito -d /path/to/data_catalog.yml -v
 
-    Update Wflow model components outlined in an .ini configuration file and
+    Update Wflow model components outlined in an .yml configuration file and
     write the model to a directory:
-    hydromt update wflow /path/to/model_root  -o /path/to/model_out  -i /path/to/wflow_config.ini  -d /path/to/data_catalog.yml -v
+    hydromt update wflow /path/to/model_root  -o /path/to/model_out  -i /path/to/wflow_config.yml  -d /path/to/data_catalog.yml -v
     """  # noqa: E501
     # logger
     mode = "r+" if model_root == model_out else "r"
     log_level = max(10, 30 - 10 * (verbose - quiet))
     logger = log.setuplog("update", join(model_out, "hydromt.log"), log_level=log_level)
     logger.info(f"Updating {model} model at {model_root} ({mode}).")
     logger.info(f"Output dir: {model_out}")
@@ -363,15 +359,15 @@
     region: Optional[Dict[Any, Any]],
     quiet: int,
     verbose: int,
 ):
     """
     Verify that provided data catalog and config files are in the correct format.
 
-    Additionnaly region bbox and geom can also be validated.
+    Additionally region bbox and geom can also be validated.
 
     Example usage:
     --------------
 
     Check data catalog file:
     hydromt check -d /path/to/data_catalog.yml -v
 
@@ -436,18 +432,20 @@
 @main.command(
     short_help="Export data",
 )
 @click.option(
     "-s",
     "--source",
     multiple=True,
+    help="Name of the data source to export.",
 )
 @click.option(
     "-t",
     "--time-tuple",
+    help="Time tuple as a list of two strings, e.g. ['2010-01-01', '2022-12-31']",
 )
 @region_opt
 @export_dest_path
 @opt_config
 @data_opt
 @deltares_data_opt
 @overwrite_opt
@@ -604,27 +602,28 @@
 @verbose_opt
 @click.pass_context
 def clip(ctx, model, model_root, model_destination, region, quiet, verbose):
     """Create a new model based on clipped region of an existing model.
 
     If the existing model contains forcing, they will also be clipped to the new model.
 
-    For options to build wflow models see:
+    Example usage:
+    --------------
 
     Example usage to clip a wflow model for a subbasin derived from point coordinates
     snapped to cells with upstream area >= 50 km2
     hydromt clip wflow /path/to/model_root /path/to/model_destination "{'subbasin': [-7.24, 62.09], 'wflow_uparea': 50}"
 
     Example usage basin based on ID from model_root basins map
     hydromt clip wflow /path/to/model_root /path/to/model_destination "{'basin': 1}"
 
     Example usage basins whose outlets are inside a geometry
     hydromt clip wflow /path/to/model_root /path/to/model_destination "{'outlet': 'geometry.geojson'}"
 
-    All available option in the clip_staticmaps function help.
+    All available option in the clip_grid function help.
 
     """  # noqa: E501
     log_level = max(10, 30 - 10 * (verbose - quiet))
     logger = log.setuplog(
         "clip", join(model_destination, "hydromt-clip.log"), log_level=log_level
     )
     logger.info(f"Clipping instance of {model} model.")
@@ -633,15 +632,15 @@
     if model != "wflow":
         raise NotImplementedError("Clip function only implemented for wflow model.")
     try:
         mod = MODELS.load(model)(root=model_root, mode="r", logger=logger)
         logger.info("Reading model to clip")
         mod.read()
         mod.set_root(model_destination, mode="w")
-        logger.info("Clipping staticmaps")
+        logger.info("Clipping grid")
         mod.clip_grid(region)
         logger.info("Clipping forcing")
         mod.clip_forcing()
         logger.info("Writting clipped model")
         mod.write()
     except Exception as e:
         logger.exception(e)  # catch and log errors
```

### Comparing `hydromt-0.9.3/hydromt/config.py` & `hydromt-0.9.4/hydromt/config.py`

 * *Files identical despite different names*

### Comparing `hydromt-0.9.3/hydromt/data_adapter/caching.py` & `hydromt-0.9.4/hydromt/data_adapter/caching.py`

 * *Files identical despite different names*

### Comparing `hydromt-0.9.3/hydromt/data_adapter/data_adapter.py` & `hydromt-0.9.4/hydromt/data_adapter/data_adapter.py`

 * *Files identical despite different names*

### Comparing `hydromt-0.9.3/hydromt/data_adapter/dataframe.py` & `hydromt-0.9.4/hydromt/data_adapter/dataframe.py`

 * *Files identical despite different names*

### Comparing `hydromt-0.9.3/hydromt/data_adapter/dataset.py` & `hydromt-0.9.4/hydromt/data_adapter/dataset.py`

 * *Files identical despite different names*

### Comparing `hydromt-0.9.3/hydromt/data_adapter/geodataframe.py` & `hydromt-0.9.4/hydromt/data_adapter/geodataframe.py`

 * *Files identical despite different names*

### Comparing `hydromt-0.9.3/hydromt/data_adapter/geodataset.py` & `hydromt-0.9.4/hydromt/data_adapter/geodataset.py`

 * *Files identical despite different names*

### Comparing `hydromt-0.9.3/hydromt/data_adapter/rasterdataset.py` & `hydromt-0.9.4/hydromt/data_adapter/rasterdataset.py`

 * *Files 0% similar despite different names*

```diff
@@ -590,25 +590,32 @@
         # work with 4326 data that is defined at 0-360 degrees longtitude
         w, _, e, _ = ds.raster.bounds
         if epsg == 4326 and np.isclose(e - w, 360):  # allow for rounding errors
             ds = gis_utils.meridian_offset(ds, bbox)
 
         # clip with bbox
         if bbox is not None:
-            bbox_str = ", ".join([f"{c:.3f}" for c in bbox])
-            logger.debug(f"Clip to [{bbox_str}] (epsg:{epsg}))")
-            ds = ds.raster.clip_bbox(bbox, buffer=buffer, align=align)
-            # if np.any(np.array(ds.raster.shape) < 2):
             # check if bbox is fully covered
+            bbox_str = ", ".join([f"{c:.3f}" for c in bbox])
+
+            def _lt_or_close(a: float, b: float) -> bool:
+                return np.isclose(a, b) or a < b
+
             w, s, e, n = ds.raster.bounds
-            if not (w <= bbox[0] and s <= bbox[1] and e >= bbox[2] and n >= bbox[3]):
+
+            if not any(
+                map(_lt_or_close, (w, s, bbox[2], bbox[3]), (bbox[0], bbox[1], e, n))
+            ):
                 logger.warning(
-                    f"Dataset does [{w}, {s}, {e}, {n}] does not fully cover bbox [{bbox_str}]"
+                    f"Dataset [{w}, {s}, {e}, {n}] does not fully cover bbox [{bbox_str}]"
                 )
 
+            logger.debug(f"Clip to [{bbox_str}] (epsg:{epsg}))")
+            ds = ds.raster.clip_bbox(bbox, buffer=buffer, align=align)
+
         if has_no_data(ds):
             return None
         else:
             return ds
 
     def _apply_unit_conversions(self, ds: Data, logger=logger):
         unit_names = list(self.unit_mult.keys()) + list(self.unit_add.keys())
```

### Comparing `hydromt-0.9.3/hydromt/data_adapter/utils.py` & `hydromt-0.9.4/hydromt/data_adapter/utils.py`

 * *Files identical despite different names*

### Comparing `hydromt-0.9.3/hydromt/data_catalog.py` & `hydromt-0.9.4/hydromt/data_catalog.py`

 * *Files identical despite different names*

### Comparing `hydromt-0.9.3/hydromt/flw.py` & `hydromt-0.9.4/hydromt/flw.py`

 * *Files identical despite different names*

### Comparing `hydromt-0.9.3/hydromt/gis_utils.py` & `hydromt-0.9.4/hydromt/gis_utils.py`

 * *Files identical despite different names*

### Comparing `hydromt-0.9.3/hydromt/io.py` & `hydromt-0.9.4/hydromt/io.py`

 * *Files 1% similar despite different names*

```diff
@@ -629,15 +629,15 @@
             else:
                 bbox_shapely = None
             bbox_reader = gis_utils.bbox_from_file_and_filters(
                 str(fn), bbox_shapely, geom, crs
             )
             gdf = read_dataframe(str(fn), bbox=bbox_reader, mode=mode, **kwargs)
         else:
-            gdf = gpd.read_file(str(fn), bbox=bbox, mode=mode, **kwargs)
+            gdf = gpd.read_file(str(fn), bbox=bbox, mask=geom, mode=mode, **kwargs)
 
     # check geometry type
     if assert_gtype is not None:
         assert_gtype = np.atleast_1d(assert_gtype)
         if not np.all(np.isin(assert_gtype, GEOMETRY_TYPES)):
             gtype_err = assert_gtype[~np.isin(assert_gtype, GEOMETRY_TYPES)]
             raise ValueError(
```

### Comparing `hydromt-0.9.3/hydromt/log.py` & `hydromt-0.9.4/hydromt/log.py`

 * *Files identical despite different names*

### Comparing `hydromt-0.9.3/hydromt/merge.py` & `hydromt-0.9.4/hydromt/merge.py`

 * *Files identical despite different names*

### Comparing `hydromt-0.9.3/hydromt/models/model_api.py` & `hydromt-0.9.4/hydromt/models/model_api.py`

 * *Files identical despite different names*

### Comparing `hydromt-0.9.3/hydromt/models/model_grid.py` & `hydromt-0.9.4/hydromt/models/model_grid.py`

 * *Files identical despite different names*

### Comparing `hydromt-0.9.3/hydromt/models/model_mesh.py` & `hydromt-0.9.4/hydromt/models/model_mesh.py`

 * *Files identical despite different names*

### Comparing `hydromt-0.9.3/hydromt/models/model_network.py` & `hydromt-0.9.4/hydromt/models/model_network.py`

 * *Files identical despite different names*

### Comparing `hydromt-0.9.3/hydromt/models/model_plugins.py` & `hydromt-0.9.4/hydromt/models/model_plugins.py`

 * *Files identical despite different names*

### Comparing `hydromt-0.9.3/hydromt/models/model_vector.py` & `hydromt-0.9.4/hydromt/models/model_vector.py`

 * *Files identical despite different names*

### Comparing `hydromt-0.9.3/hydromt/nodata.py` & `hydromt-0.9.4/hydromt/nodata.py`

 * *Files identical despite different names*

### Comparing `hydromt-0.9.3/hydromt/raster.py` & `hydromt-0.9.4/hydromt/raster.py`

 * *Files identical despite different names*

### Comparing `hydromt-0.9.3/hydromt/stats/design_events.py` & `hydromt-0.9.4/hydromt/stats/design_events.py`

 * *Files identical despite different names*

### Comparing `hydromt-0.9.3/hydromt/stats/extremes.py` & `hydromt-0.9.4/hydromt/stats/extremes.py`

 * *Files identical despite different names*

### Comparing `hydromt-0.9.3/hydromt/stats/skills.py` & `hydromt-0.9.4/hydromt/stats/skills.py`

 * *Files identical despite different names*

### Comparing `hydromt-0.9.3/hydromt/typing.py` & `hydromt-0.9.4/hydromt/typing.py`

 * *Files identical despite different names*

### Comparing `hydromt-0.9.3/hydromt/utils.py` & `hydromt-0.9.4/hydromt/utils.py`

 * *Files identical despite different names*

### Comparing `hydromt-0.9.3/hydromt/validators/__init__.py` & `hydromt-0.9.4/hydromt/validators/__init__.py`

 * *Files identical despite different names*

### Comparing `hydromt-0.9.3/hydromt/validators/data_catalog.py` & `hydromt-0.9.4/hydromt/validators/data_catalog.py`

 * *Files identical despite different names*

### Comparing `hydromt-0.9.3/hydromt/validators/model_config.py` & `hydromt-0.9.4/hydromt/validators/model_config.py`

 * *Files identical despite different names*

### Comparing `hydromt-0.9.3/hydromt/validators/region.py` & `hydromt-0.9.4/hydromt/validators/region.py`

 * *Files identical despite different names*

### Comparing `hydromt-0.9.3/hydromt/vector.py` & `hydromt-0.9.4/hydromt/vector.py`

 * *Files identical despite different names*

### Comparing `hydromt-0.9.3/hydromt/workflows/basin_mask.py` & `hydromt-0.9.4/hydromt/workflows/basin_mask.py`

 * *Files identical despite different names*

### Comparing `hydromt-0.9.3/hydromt/workflows/forcing.py` & `hydromt-0.9.4/hydromt/workflows/forcing.py`

 * *Files identical despite different names*

### Comparing `hydromt-0.9.3/hydromt/workflows/grid.py` & `hydromt-0.9.4/hydromt/workflows/grid.py`

 * *Files identical despite different names*

### Comparing `hydromt-0.9.3/hydromt/workflows/mesh.py` & `hydromt-0.9.4/hydromt/workflows/mesh.py`

 * *Files identical despite different names*

### Comparing `hydromt-0.9.3/hydromt/workflows/rivers.py` & `hydromt-0.9.4/hydromt/workflows/rivers.py`

 * *Files identical despite different names*

### Comparing `hydromt-0.9.3/joss_paper/citation.bib` & `hydromt-0.9.4/joss_paper/citation.bib`

 * *Files identical despite different names*

### Comparing `hydromt-0.9.3/joss_paper/paper.bib` & `hydromt-0.9.4/joss_paper/paper.bib`

 * *Files identical despite different names*

### Comparing `hydromt-0.9.3/joss_paper/paper.md` & `hydromt-0.9.4/joss_paper/paper.md`

 * *Files identical despite different names*

### Comparing `hydromt-0.9.3/make_env.py` & `hydromt-0.9.4/make_env.py`

 * *Files identical despite different names*

### Comparing `hydromt-0.9.3/pixi.toml` & `hydromt-0.9.4/pixi.toml`

 * *Files identical despite different names*

### Comparing `hydromt-0.9.3/pyproject.toml` & `hydromt-0.9.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -86,14 +86,15 @@
 doc = [
   "hydromt[examples,extra]",      # examples are included in the docs
   "nbsphinx",                     # build notebooks in docs
   "pydata-sphinx-theme>=0.15.2",  # theme
   "sphinx_autosummary_accessors", # doc layout
   "sphinx",                       # build docks
   "sphinx_design",                # doc layout
+  "sphinx-click",       # click integration
 ]
 examples = [
   "cartopy",    # plotting examples
   "jupyterlab", # run examples in jupyter notebook
   "notebook",   # jupyter integration
 ]
 
@@ -105,15 +106,15 @@
 Source = "https://github.com/Deltares/hydromt"
 
 [project.scripts]
 hydromt = "hydromt.cli.main:main"
 
 [tool.make_env]
 channels = ["conda-forge"]
-deps_not_in_conda = ["sphinx_autosummary_accessors", "sphinx_design"]
+deps_not_in_conda = ["sphinx_autosummary_accessors", "sphinx_design", "sphinx-click"]
 
 
 [tool.ruff]
 line-length = 88
 target-version = "py39"
 
 # enable pydocstyle (E), pyflake (F) and isort (I), pytest-style (PT), bugbear (B)
```

### Comparing `hydromt-0.9.3/PKG-INFO` & `hydromt-0.9.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hydromt
-Version: 0.9.3
+Version: 0.9.4
 Summary: HydroMT: Automated and reproducible model building and analysis.
 Author-email: Dirk Eilander <dirk.eilander@deltares.nl>, Hélène Boisgontier <helene.boisgontier@deltares.nl>, Sam Vente <sam.vente@deltares.nl>
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
@@ -49,14 +49,15 @@
 Requires-Dist: twine ; extra == "dev"
 Requires-Dist: hydromt[examples,extra] ; extra == "doc"
 Requires-Dist: nbsphinx ; extra == "doc"
 Requires-Dist: pydata-sphinx-theme>=0.15.2 ; extra == "doc"
 Requires-Dist: sphinx_autosummary_accessors ; extra == "doc"
 Requires-Dist: sphinx ; extra == "doc"
 Requires-Dist: sphinx_design ; extra == "doc"
+Requires-Dist: sphinx-click ; extra == "doc"
 Requires-Dist: cartopy ; extra == "examples"
 Requires-Dist: jupyterlab ; extra == "examples"
 Requires-Dist: notebook ; extra == "examples"
 Requires-Dist: matplotlib ; extra == "extra"
 Requires-Dist: pyet ; extra == "extra"
 Requires-Dist: xugrid>=0.6.5 ; extra == "extra"
 Requires-Dist: hydromt[io,extra,dev,test,doc,examples] ; extra == "full"
```

