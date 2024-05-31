# Comparing `tmp/physt-0.6.0a2.tar.gz` & `tmp/physt-0.6.0a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "physt-0.6.0a2.tar", last modified: Thu Jan 18 15:30:30 2024, max compression
+gzip compressed data, was "physt-0.6.0a4.tar", last modified: Tue Jan 30 08:40:43 2024, max compression
```

## Comparing `physt-0.6.0a2.tar` & `physt-0.6.0a4.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxrwxr-x   0 jan       (1000) jan       (1000)        0 2024-01-18 15:30:30.037151 physt-0.6.0a2/
--rw-rw-r--   0 jan       (1000) jan       (1000)    11001 2024-01-18 15:18:24.000000 physt-0.6.0a2/HISTORY.txt
--rw-rw-r--   0 jan       (1000) jan       (1000)     1081 2024-01-18 09:16:51.000000 physt-0.6.0a2/LICENSE
--rw-rw-r--   0 jan       (1000) jan       (1000)      240 2022-11-05 15:01:31.000000 physt-0.6.0a2/MANIFEST.in
--rw-r--r--   0 jan       (1000) jan       (1000)     9955 2024-01-18 15:30:30.036152 physt-0.6.0a2/PKG-INFO
--rw-rw-r--   0 jan       (1000) jan       (1000)     6796 2022-11-28 13:06:35.000000 physt-0.6.0a2/README.md
--rw-rw-r--   0 jan       (1000) jan       (1000)     2280 2024-01-18 15:24:08.000000 physt-0.6.0a2/pyproject.toml
--rw-rw-r--   0 jan       (1000) jan       (1000)       38 2024-01-18 15:30:30.037151 physt-0.6.0a2/setup.cfg
-drwxrwxr-x   0 jan       (1000) jan       (1000)        0 2024-01-18 15:30:29.994152 physt-0.6.0a2/src/
-drwxrwxr-x   0 jan       (1000) jan       (1000)        0 2024-01-18 15:30:30.006152 physt-0.6.0a2/src/physt/
--rw-rw-r--   0 jan       (1000) jan       (1000)      798 2022-11-05 15:01:31.000000 physt-0.6.0a2/src/physt/__init__.py
--rw-rw-r--   0 jan       (1000) jan       (1000)     6483 2024-01-18 08:34:31.000000 physt-0.6.0a2/src/physt/_bin_utils.py
--rw-rw-r--   0 jan       (1000) jan       (1000)    20102 2024-01-18 08:34:31.000000 physt-0.6.0a2/src/physt/_construction.py
--rw-rw-r--   0 jan       (1000) jan       (1000)     8460 2024-01-18 08:34:31.000000 physt-0.6.0a2/src/physt/_facade.py
--rw-rw-r--   0 jan       (1000) jan       (1000)     2415 2024-01-18 08:34:31.000000 physt-0.6.0a2/src/physt/_util.py
--rw-rw-r--   0 jan       (1000) jan       (1000)    35776 2024-01-18 08:34:31.000000 physt-0.6.0a2/src/physt/binnings.py
-drwxrwxr-x   0 jan       (1000) jan       (1000)        0 2024-01-18 15:30:30.011152 physt-0.6.0a2/src/physt/compat/
--rw-rw-r--   0 jan       (1000) jan       (1000)      601 2023-01-30 10:59:27.000000 physt-0.6.0a2/src/physt/compat/__init__.py
--rw-rw-r--   0 jan       (1000) jan       (1000)     5027 2024-01-18 09:16:51.000000 physt-0.6.0a2/src/physt/compat/dask.py
--rw-rw-r--   0 jan       (1000) jan       (1000)     3021 2024-01-18 08:34:31.000000 physt-0.6.0a2/src/physt/compat/geant4.py
--rw-rw-r--   0 jan       (1000) jan       (1000)     9818 2024-01-18 08:34:31.000000 physt-0.6.0a2/src/physt/compat/pandas.py
--rw-rw-r--   0 jan       (1000) jan       (1000)     3545 2024-01-18 15:18:26.000000 physt-0.6.0a2/src/physt/compat/polars.py
--rw-rw-r--   0 jan       (1000) jan       (1000)     1691 2022-11-05 15:01:31.000000 physt-0.6.0a2/src/physt/compat/xarray.py
--rw-rw-r--   0 jan       (1000) jan       (1000)     1705 2024-01-18 08:34:31.000000 physt-0.6.0a2/src/physt/config.py
-drwxrwxr-x   0 jan       (1000) jan       (1000)        0 2024-01-18 15:30:30.012152 physt-0.6.0a2/src/physt/examples/
--rw-rw-r--   0 jan       (1000) jan       (1000)     3423 2024-01-18 08:34:31.000000 physt-0.6.0a2/src/physt/examples/__init__.py
--rw-rw-r--   0 jan       (1000) jan       (1000)    17171 2022-11-05 15:01:31.000000 physt-0.6.0a2/src/physt/examples/munros.csv
-drwxrwxr-x   0 jan       (1000) jan       (1000)        0 2024-01-18 15:30:30.012152 physt-0.6.0a2/src/physt/helpers/
--rw-rw-r--   0 jan       (1000) jan       (1000)        0 2022-11-05 15:01:31.000000 physt-0.6.0a2/src/physt/helpers/__init__.py
--rw-rw-r--   0 jan       (1000) jan       (1000)     1791 2022-11-05 15:01:31.000000 physt-0.6.0a2/src/physt/helpers/db.py
--rw-rw-r--   0 jan       (1000) jan       (1000)    17074 2024-01-18 08:34:31.000000 physt-0.6.0a2/src/physt/histogram1d.py
--rw-rw-r--   0 jan       (1000) jan       (1000)    35753 2024-01-18 09:16:51.000000 physt-0.6.0a2/src/physt/histogram_base.py
--rw-rw-r--   0 jan       (1000) jan       (1000)     7074 2024-01-18 08:34:31.000000 physt-0.6.0a2/src/physt/histogram_collection.py
--rw-rw-r--   0 jan       (1000) jan       (1000)    20641 2024-01-18 09:16:51.000000 physt-0.6.0a2/src/physt/histogram_nd.py
-drwxrwxr-x   0 jan       (1000) jan       (1000)        0 2024-01-18 15:30:30.014152 physt-0.6.0a2/src/physt/io/
--rw-rw-r--   0 jan       (1000) jan       (1000)      649 2024-01-18 15:18:26.000000 physt-0.6.0a2/src/physt/io/__init__.py
--rw-rw-r--   0 jan       (1000) jan       (1000)     1673 2024-01-18 08:34:31.000000 physt-0.6.0a2/src/physt/io/json.py
--rw-rw-r--   0 jan       (1000) jan       (1000)     1346 2024-01-18 15:18:26.000000 physt-0.6.0a2/src/physt/io/root.py
--rw-rw-r--   0 jan       (1000) jan       (1000)     1066 2022-11-05 15:01:31.000000 physt-0.6.0a2/src/physt/io/util.py
--rw-rw-r--   0 jan       (1000) jan       (1000)      784 2022-11-05 15:01:31.000000 physt-0.6.0a2/src/physt/io/version.py
-drwxrwxr-x   0 jan       (1000) jan       (1000)        0 2024-01-18 15:30:30.018152 physt-0.6.0a2/src/physt/plotting/
--rw-rw-r--   0 jan       (1000) jan       (1000)     7516 2024-01-18 08:34:31.000000 physt-0.6.0a2/src/physt/plotting/__init__.py
--rw-rw-r--   0 jan       (1000) jan       (1000)     2915 2024-01-18 08:34:31.000000 physt-0.6.0a2/src/physt/plotting/ascii.py
--rw-rw-r--   0 jan       (1000) jan       (1000)     9717 2024-01-18 08:34:31.000000 physt-0.6.0a2/src/physt/plotting/common.py
--rw-rw-r--   0 jan       (1000) jan       (1000)     3287 2024-01-18 08:34:31.000000 physt-0.6.0a2/src/physt/plotting/folium.py
--rw-rw-r--   0 jan       (1000) jan       (1000)    35888 2024-01-18 09:16:51.000000 physt-0.6.0a2/src/physt/plotting/matplotlib.py
--rw-rw-r--   0 jan       (1000) jan       (1000)     4399 2024-01-18 08:34:31.000000 physt-0.6.0a2/src/physt/plotting/plotly.py
--rw-rw-r--   0 jan       (1000) jan       (1000)    23376 2024-01-18 08:34:31.000000 physt-0.6.0a2/src/physt/plotting/vega.py
--rw-rw-r--   0 jan       (1000) jan       (1000)    24442 2024-01-18 08:34:31.000000 physt-0.6.0a2/src/physt/special_histograms.py
--rw-rw-r--   0 jan       (1000) jan       (1000)     2582 2022-11-05 15:01:31.000000 physt-0.6.0a2/src/physt/statistics.py
-drwxrwxr-x   0 jan       (1000) jan       (1000)        0 2024-01-18 15:30:30.019152 physt-0.6.0a2/src/physt/testing/
--rw-rw-r--   0 jan       (1000) jan       (1000)     1052 2022-11-05 15:01:31.000000 physt-0.6.0a2/src/physt/testing/__init__.py
--rw-rw-r--   0 jan       (1000) jan       (1000)     1775 2024-01-18 08:34:31.000000 physt-0.6.0a2/src/physt/testing/strategies.py
--rw-rw-r--   0 jan       (1000) jan       (1000)      324 2024-01-18 08:34:31.000000 physt-0.6.0a2/src/physt/types.py
--rw-rw-r--   0 jan       (1000) jan       (1000)      299 2022-11-05 15:01:31.000000 physt-0.6.0a2/src/physt/typing_aliases.py
--rw-rw-r--   0 jan       (1000) jan       (1000)      163 2024-01-18 15:24:08.000000 physt-0.6.0a2/src/physt/version.py
-drwxrwxr-x   0 jan       (1000) jan       (1000)        0 2024-01-18 15:30:30.026152 physt-0.6.0a2/src/physt.egg-info/
--rw-r--r--   0 jan       (1000) jan       (1000)     9955 2024-01-18 15:30:29.000000 physt-0.6.0a2/src/physt.egg-info/PKG-INFO
--rw-rw-r--   0 jan       (1000) jan       (1000)     1618 2024-01-18 15:30:29.000000 physt-0.6.0a2/src/physt.egg-info/SOURCES.txt
--rw-rw-r--   0 jan       (1000) jan       (1000)        1 2024-01-18 15:30:29.000000 physt-0.6.0a2/src/physt.egg-info/dependency_links.txt
--rw-rw-r--   0 jan       (1000) jan       (1000)      471 2024-01-18 15:30:29.000000 physt-0.6.0a2/src/physt.egg-info/requires.txt
--rw-rw-r--   0 jan       (1000) jan       (1000)        6 2024-01-18 15:30:29.000000 physt-0.6.0a2/src/physt.egg-info/top_level.txt
-drwxrwxr-x   0 jan       (1000) jan       (1000)        0 2024-01-18 15:30:30.025152 physt-0.6.0a2/tests/
-drwxrwxr-x   0 jan       (1000) jan       (1000)        0 2024-01-18 15:30:30.026152 physt-0.6.0a2/tests/data/
--rw-rw-r--   0 jan       (1000) jan       (1000)     1768 2022-11-05 15:01:31.000000 physt-0.6.0a2/tests/data/geant-h1.csv
--rw-rw-r--   0 jan       (1000) jan       (1000)    38786 2022-11-05 15:01:31.000000 physt-0.6.0a2/tests/data/geant-h2.csv
--rw-rw-r--   0 jan       (1000) jan       (1000)     5251 2022-11-05 15:01:31.000000 physt-0.6.0a2/tests/test_adaptive.py
--rw-rw-r--   0 jan       (1000) jan       (1000)     3049 2024-01-18 08:34:31.000000 physt-0.6.0a2/tests/test_bin_utils.py
--rw-rw-r--   0 jan       (1000) jan       (1000)     7868 2024-01-18 08:34:31.000000 physt-0.6.0a2/tests/test_binning.py
--rw-rw-r--   0 jan       (1000) jan       (1000)    12435 2024-01-18 08:34:31.000000 physt-0.6.0a2/tests/test_construction.py
--rw-rw-r--   0 jan       (1000) jan       (1000)      830 2024-01-18 08:34:31.000000 physt-0.6.0a2/tests/test_examples.py
--rw-rw-r--   0 jan       (1000) jan       (1000)     3763 2024-01-18 15:18:26.000000 physt-0.6.0a2/tests/test_facade.py
--rw-rw-r--   0 jan       (1000) jan       (1000)     1373 2022-11-05 15:01:31.000000 physt-0.6.0a2/tests/test_histogram.py
--rw-rw-r--   0 jan       (1000) jan       (1000)    21010 2024-01-18 08:34:31.000000 physt-0.6.0a2/tests/test_histogram1d.py
--rw-rw-r--   0 jan       (1000) jan       (1000)     6707 2024-01-18 08:34:31.000000 physt-0.6.0a2/tests/test_histogram2d.py
--rw-rw-r--   0 jan       (1000) jan       (1000)     5815 2024-01-18 08:34:31.000000 physt-0.6.0a2/tests/test_histogramnd.py
--rw-rw-r--   0 jan       (1000) jan       (1000)     1679 2024-01-18 09:22:42.000000 physt-0.6.0a2/tests/test_io.py
--rw-rw-r--   0 jan       (1000) jan       (1000)     7451 2024-01-18 08:34:31.000000 physt-0.6.0a2/tests/test_special.py
--rw-rw-r--   0 jan       (1000) jan       (1000)     2344 2024-01-18 08:34:31.000000 physt-0.6.0a2/tests/test_stats.py
+drwxr-xr-x   0 jan       (1000) jan       (1000)        0 2024-01-30 08:40:43.164738 physt-0.6.0a4/
+-rw-r--r--   0 jan       (1000) jan       (1000)    11071 2024-01-26 18:28:39.000000 physt-0.6.0a4/HISTORY.txt
+-rw-r--r--   0 jan       (1000) jan       (1000)     1081 2024-01-26 18:28:39.000000 physt-0.6.0a4/LICENSE
+-rw-r--r--   0 jan       (1000) jan       (1000)      240 2024-01-26 18:28:39.000000 physt-0.6.0a4/MANIFEST.in
+-rw-r--r--   0 jan       (1000) jan       (1000)     9998 2024-01-30 08:40:43.164738 physt-0.6.0a4/PKG-INFO
+-rw-r--r--   0 jan       (1000) jan       (1000)     6862 2024-01-26 18:28:39.000000 physt-0.6.0a4/README.md
+-rw-r--r--   0 jan       (1000) jan       (1000)     2386 2024-01-30 08:38:46.000000 physt-0.6.0a4/pyproject.toml
+-rw-r--r--   0 jan       (1000) jan       (1000)       38 2024-01-30 08:40:43.164738 physt-0.6.0a4/setup.cfg
+drwxr-xr-x   0 jan       (1000) jan       (1000)        0 2024-01-30 08:40:43.154738 physt-0.6.0a4/src/
+drwxr-xr-x   0 jan       (1000) jan       (1000)        0 2024-01-30 08:40:43.157738 physt-0.6.0a4/src/physt/
+-rw-r--r--   0 jan       (1000) jan       (1000)      798 2024-01-26 18:28:39.000000 physt-0.6.0a4/src/physt/__init__.py
+-rw-r--r--   0 jan       (1000) jan       (1000)     6497 2024-01-26 18:28:39.000000 physt-0.6.0a4/src/physt/_bin_utils.py
+-rw-r--r--   0 jan       (1000) jan       (1000)    20102 2024-01-26 18:28:39.000000 physt-0.6.0a4/src/physt/_construction.py
+-rw-r--r--   0 jan       (1000) jan       (1000)     8460 2024-01-26 18:28:39.000000 physt-0.6.0a4/src/physt/_facade.py
+-rw-r--r--   0 jan       (1000) jan       (1000)     2415 2024-01-26 18:28:39.000000 physt-0.6.0a4/src/physt/_util.py
+-rw-r--r--   0 jan       (1000) jan       (1000)    35941 2024-01-26 18:28:39.000000 physt-0.6.0a4/src/physt/binnings.py
+drwxr-xr-x   0 jan       (1000) jan       (1000)        0 2024-01-30 08:40:43.158738 physt-0.6.0a4/src/physt/compat/
+-rw-r--r--   0 jan       (1000) jan       (1000)      601 2024-01-26 18:28:39.000000 physt-0.6.0a4/src/physt/compat/__init__.py
+-rw-r--r--   0 jan       (1000) jan       (1000)     5027 2024-01-26 18:28:39.000000 physt-0.6.0a4/src/physt/compat/dask.py
+-rw-r--r--   0 jan       (1000) jan       (1000)     3093 2024-01-26 18:28:39.000000 physt-0.6.0a4/src/physt/compat/geant4.py
+-rw-r--r--   0 jan       (1000) jan       (1000)     9818 2024-01-26 18:28:39.000000 physt-0.6.0a4/src/physt/compat/pandas.py
+-rw-r--r--   0 jan       (1000) jan       (1000)     3545 2024-01-26 18:28:39.000000 physt-0.6.0a4/src/physt/compat/polars.py
+-rw-r--r--   0 jan       (1000) jan       (1000)     1691 2024-01-26 18:28:39.000000 physt-0.6.0a4/src/physt/compat/xarray.py
+-rw-r--r--   0 jan       (1000) jan       (1000)     1705 2024-01-26 18:28:39.000000 physt-0.6.0a4/src/physt/config.py
+drwxr-xr-x   0 jan       (1000) jan       (1000)        0 2024-01-30 08:40:43.158738 physt-0.6.0a4/src/physt/examples/
+-rw-r--r--   0 jan       (1000) jan       (1000)     3423 2024-01-26 18:28:39.000000 physt-0.6.0a4/src/physt/examples/__init__.py
+-rw-r--r--   0 jan       (1000) jan       (1000)    17171 2024-01-26 18:28:39.000000 physt-0.6.0a4/src/physt/examples/munros.csv
+drwxr-xr-x   0 jan       (1000) jan       (1000)        0 2024-01-30 08:40:43.158738 physt-0.6.0a4/src/physt/helpers/
+-rw-r--r--   0 jan       (1000) jan       (1000)        0 2024-01-26 18:28:39.000000 physt-0.6.0a4/src/physt/helpers/__init__.py
+-rw-r--r--   0 jan       (1000) jan       (1000)     1791 2024-01-26 18:28:39.000000 physt-0.6.0a4/src/physt/helpers/db.py
+-rw-r--r--   0 jan       (1000) jan       (1000)    17074 2024-01-26 18:28:39.000000 physt-0.6.0a4/src/physt/histogram1d.py
+-rw-r--r--   0 jan       (1000) jan       (1000)    35753 2024-01-26 18:28:39.000000 physt-0.6.0a4/src/physt/histogram_base.py
+-rw-r--r--   0 jan       (1000) jan       (1000)     7074 2024-01-26 18:28:39.000000 physt-0.6.0a4/src/physt/histogram_collection.py
+-rw-r--r--   0 jan       (1000) jan       (1000)    20641 2024-01-26 18:28:39.000000 physt-0.6.0a4/src/physt/histogram_nd.py
+drwxr-xr-x   0 jan       (1000) jan       (1000)        0 2024-01-30 08:40:43.159738 physt-0.6.0a4/src/physt/io/
+-rw-r--r--   0 jan       (1000) jan       (1000)      649 2024-01-26 18:28:39.000000 physt-0.6.0a4/src/physt/io/__init__.py
+-rw-r--r--   0 jan       (1000) jan       (1000)     1673 2024-01-26 18:28:39.000000 physt-0.6.0a4/src/physt/io/json.py
+-rw-r--r--   0 jan       (1000) jan       (1000)     1346 2024-01-26 18:28:39.000000 physt-0.6.0a4/src/physt/io/root.py
+-rw-r--r--   0 jan       (1000) jan       (1000)     1066 2024-01-26 18:28:39.000000 physt-0.6.0a4/src/physt/io/util.py
+-rw-r--r--   0 jan       (1000) jan       (1000)      790 2024-01-30 08:38:42.000000 physt-0.6.0a4/src/physt/io/version.py
+drwxr-xr-x   0 jan       (1000) jan       (1000)        0 2024-01-30 08:40:43.160738 physt-0.6.0a4/src/physt/plotting/
+-rw-r--r--   0 jan       (1000) jan       (1000)     7545 2024-01-26 18:28:39.000000 physt-0.6.0a4/src/physt/plotting/__init__.py
+-rw-r--r--   0 jan       (1000) jan       (1000)     2915 2024-01-26 18:28:39.000000 physt-0.6.0a4/src/physt/plotting/ascii.py
+-rw-r--r--   0 jan       (1000) jan       (1000)     9725 2024-01-26 18:28:39.000000 physt-0.6.0a4/src/physt/plotting/common.py
+-rw-r--r--   0 jan       (1000) jan       (1000)     3300 2024-01-26 18:28:39.000000 physt-0.6.0a4/src/physt/plotting/folium.py
+-rw-r--r--   0 jan       (1000) jan       (1000)    35888 2024-01-26 18:28:39.000000 physt-0.6.0a4/src/physt/plotting/matplotlib.py
+-rw-r--r--   0 jan       (1000) jan       (1000)     4399 2024-01-26 18:28:39.000000 physt-0.6.0a4/src/physt/plotting/plotly.py
+-rw-r--r--   0 jan       (1000) jan       (1000)    23376 2024-01-26 18:28:39.000000 physt-0.6.0a4/src/physt/plotting/vega.py
+-rw-r--r--   0 jan       (1000) jan       (1000)    24442 2024-01-26 18:28:39.000000 physt-0.6.0a4/src/physt/special_histograms.py
+-rw-r--r--   0 jan       (1000) jan       (1000)     2582 2024-01-26 18:28:39.000000 physt-0.6.0a4/src/physt/statistics.py
+drwxr-xr-x   0 jan       (1000) jan       (1000)        0 2024-01-30 08:40:43.160738 physt-0.6.0a4/src/physt/testing/
+-rw-r--r--   0 jan       (1000) jan       (1000)     1052 2024-01-26 18:28:39.000000 physt-0.6.0a4/src/physt/testing/__init__.py
+-rw-r--r--   0 jan       (1000) jan       (1000)     1775 2024-01-26 18:28:39.000000 physt-0.6.0a4/src/physt/testing/strategies.py
+-rw-r--r--   0 jan       (1000) jan       (1000)      324 2024-01-26 18:28:39.000000 physt-0.6.0a4/src/physt/types.py
+-rw-r--r--   0 jan       (1000) jan       (1000)      299 2024-01-26 18:28:39.000000 physt-0.6.0a4/src/physt/typing_aliases.py
+-rw-r--r--   0 jan       (1000) jan       (1000)      163 2024-01-30 08:38:46.000000 physt-0.6.0a4/src/physt/version.py
+drwxr-xr-x   0 jan       (1000) jan       (1000)        0 2024-01-30 08:40:43.162738 physt-0.6.0a4/src/physt.egg-info/
+-rw-r--r--   0 jan       (1000) jan       (1000)     9998 2024-01-30 08:40:43.000000 physt-0.6.0a4/src/physt.egg-info/PKG-INFO
+-rw-r--r--   0 jan       (1000) jan       (1000)     1618 2024-01-30 08:40:43.000000 physt-0.6.0a4/src/physt.egg-info/SOURCES.txt
+-rw-r--r--   0 jan       (1000) jan       (1000)        1 2024-01-30 08:40:43.000000 physt-0.6.0a4/src/physt.egg-info/dependency_links.txt
+-rw-r--r--   0 jan       (1000) jan       (1000)      463 2024-01-30 08:40:43.000000 physt-0.6.0a4/src/physt.egg-info/requires.txt
+-rw-r--r--   0 jan       (1000) jan       (1000)        6 2024-01-30 08:40:43.000000 physt-0.6.0a4/src/physt.egg-info/top_level.txt
+drwxr-xr-x   0 jan       (1000) jan       (1000)        0 2024-01-30 08:40:43.161738 physt-0.6.0a4/tests/
+drwxr-xr-x   0 jan       (1000) jan       (1000)        0 2024-01-30 08:40:43.161738 physt-0.6.0a4/tests/data/
+-rw-r--r--   0 jan       (1000) jan       (1000)     1768 2024-01-26 18:28:39.000000 physt-0.6.0a4/tests/data/geant-h1.csv
+-rw-r--r--   0 jan       (1000) jan       (1000)    38786 2024-01-26 18:28:39.000000 physt-0.6.0a4/tests/data/geant-h2.csv
+-rw-r--r--   0 jan       (1000) jan       (1000)     5251 2024-01-26 18:28:39.000000 physt-0.6.0a4/tests/test_adaptive.py
+-rw-r--r--   0 jan       (1000) jan       (1000)     3052 2024-01-26 18:28:39.000000 physt-0.6.0a4/tests/test_bin_utils.py
+-rw-r--r--   0 jan       (1000) jan       (1000)     7874 2024-01-26 18:28:39.000000 physt-0.6.0a4/tests/test_binning.py
+-rw-r--r--   0 jan       (1000) jan       (1000)    12435 2024-01-26 18:28:39.000000 physt-0.6.0a4/tests/test_construction.py
+-rw-r--r--   0 jan       (1000) jan       (1000)      830 2024-01-26 18:28:39.000000 physt-0.6.0a4/tests/test_examples.py
+-rw-r--r--   0 jan       (1000) jan       (1000)     4005 2024-01-26 18:28:39.000000 physt-0.6.0a4/tests/test_facade.py
+-rw-r--r--   0 jan       (1000) jan       (1000)     1373 2024-01-26 18:28:39.000000 physt-0.6.0a4/tests/test_histogram.py
+-rw-r--r--   0 jan       (1000) jan       (1000)    21010 2024-01-26 18:28:39.000000 physt-0.6.0a4/tests/test_histogram1d.py
+-rw-r--r--   0 jan       (1000) jan       (1000)     6707 2024-01-26 18:28:39.000000 physt-0.6.0a4/tests/test_histogram2d.py
+-rw-r--r--   0 jan       (1000) jan       (1000)     5815 2024-01-26 18:28:39.000000 physt-0.6.0a4/tests/test_histogramnd.py
+-rw-r--r--   0 jan       (1000) jan       (1000)     1679 2024-01-26 18:28:39.000000 physt-0.6.0a4/tests/test_io.py
+-rw-r--r--   0 jan       (1000) jan       (1000)     7451 2024-01-26 18:28:39.000000 physt-0.6.0a4/tests/test_special.py
+-rw-r--r--   0 jan       (1000) jan       (1000)     2344 2024-01-26 18:28:39.000000 physt-0.6.0a4/tests/test_stats.py
```

### Comparing `physt-0.6.0a2/HISTORY.txt` & `physt-0.6.0a4/HISTORY.txt`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 - Added: Support for pola.rs series/dataframes
 - Moved: xarray support as a separate module in physt.compat
 - Removed: physt.special (use physt.special_histograms instead)
 - Added: Pretty printing with rich library
 - Changed: Moved most configuration to pyproject.toml
 - Improved: Much more testing and edge-case bug fixes
 - Support: Removed Python 3.7 and numpy <1.22, added 3.11
+- Renamed: human binning => pretty binning (with deprecation warning)
 
 0.5.3 (6 January 2022)
 ----------------------
 - Changed: Distribution to wheels
 - Changed: Statistics have a special class
 - Changed: Statistics are now computed from all values (more options for plot too)
 - Fixed: Sometimes, dtypes were not properly used
```

### Comparing `physt-0.6.0a2/LICENSE` & `physt-0.6.0a4/LICENSE`

 * *Files identical despite different names*

### Comparing `physt-0.6.0a2/PKG-INFO` & `physt-0.6.0a4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: physt
-Version: 0.6.0a2
+Version: 0.6.0a4
 Summary: P(i/y)thon h(i/y)stograms.
 Author-email: Jan Pipek <jan.pipek@gmail.com>
 License: The MIT License (MIT)
         
         Copyright (c) 2016-2024 Jan Pipek
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -31,22 +31,23 @@
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: ~=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: numpy>=1.23
+Requires-Dist: numpy<2.0,>=1.23
 Requires-Dist: packaging
 Requires-Dist: typing_extensions
 Requires-Dist: hypothesis>=6.96.1
 Provides-Extra: dev
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: mypy>=1.8; extra == "dev"
 Requires-Dist: types-setuptools; extra == "dev"
+Requires-Dist: bumpver; extra == "dev"
 Provides-Extra: astropy
 Requires-Dist: astropy; extra == "astropy"
 Provides-Extra: dask
 Requires-Dist: dask[array]>=2023.0; extra == "dask"
 Provides-Extra: pandas
 Requires-Dist: pandas>=1.3; extra == "pandas"
 Provides-Extra: polars
@@ -55,26 +56,24 @@
 Requires-Dist: physt[pandas]; extra == "polars"
 Provides-Extra: xarray
 Requires-Dist: xarray; extra == "xarray"
 Provides-Extra: matplotlib
 Requires-Dist: matplotlib>=3.0; extra == "matplotlib"
 Provides-Extra: plotly
 Requires-Dist: plotly; extra == "plotly"
-Provides-Extra: vega3
-Requires-Dist: vega3; extra == "vega3"
 Provides-Extra: folium
 Requires-Dist: folium; extra == "folium"
 Provides-Extra: root
 Requires-Dist: uproot3; extra == "root"
 Provides-Extra: scipy
 Requires-Dist: scipy; extra == "scipy"
 Provides-Extra: xtermcolor
 Requires-Dist: xtermcolor; extra == "xtermcolor"
 Provides-Extra: all
-Requires-Dist: physt[astropy,dask,dev,folium,matplotlib,pandas,plotly,polars,root,scipy,vega3,xarray,xtermcolor]; extra == "all"
+Requires-Dist: physt[astropy,dask,dev,folium,matplotlib,pandas,plotly,polars,root,scipy,xarray,xtermcolor]; extra == "all"
 
 # physt ![Physt logo](doc/physt-logo64.png)
 
 
 
 P(i/y)thon h(i/y)stograms. Inspired (and based on) numpy.histogram, but designed for humans(TM) on steroids(TM).
 
@@ -113,15 +112,15 @@
 ## 2D example
 
 ```python
 from physt import h2
 import seaborn as sns
 
 iris = sns.load_dataset('iris')
-iris_hist = h2(iris["sepal_length"], iris["sepal_width"], "human", bin_count=[12, 7], name="Iris")
+iris_hist = h2(iris["sepal_length"], iris["sepal_width"], "pretty", bin_count=[12, 7], name="Iris")
 iris_hist.plot(show_zero=False, cmap="gray_r", show_values=True);
 ```
 
 ![Iris 2D plot](doc/iris-2d.png)
 
 ## 3D directional example
 
@@ -189,16 +188,16 @@
 * Plotting with several backends
   - matplotlib (static plots with many options)
   - vega (interactive plots, beta, help wanted!)
   - folium (experimental for geo-data)
   - plotly (very basic, help wanted!)
   - ascii (experimental)
 * Algorithms for optimized binning
-  - human-friendly
-  - mathematical
+  - pretty (nice rounded bin edges)
+  - mathematical (statistical, quantile-based, geometrical, ...)
 * IO, conversions
   - I/O JSON
   - I/O xarray.DataSet (experimental)
   - O ROOT file (experimental)
   - O pandas.DataFrame (basic)
 
 ### Planned
```

### Comparing `physt-0.6.0a2/README.md` & `physt-0.6.0a4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 ## 2D example
 
 ```python
 from physt import h2
 import seaborn as sns
 
 iris = sns.load_dataset('iris')
-iris_hist = h2(iris["sepal_length"], iris["sepal_width"], "human", bin_count=[12, 7], name="Iris")
+iris_hist = h2(iris["sepal_length"], iris["sepal_width"], "pretty", bin_count=[12, 7], name="Iris")
 iris_hist.plot(show_zero=False, cmap="gray_r", show_values=True);
 ```
 
 ![Iris 2D plot](doc/iris-2d.png)
 
 ## 3D directional example
 
@@ -115,16 +115,16 @@
 * Plotting with several backends
   - matplotlib (static plots with many options)
   - vega (interactive plots, beta, help wanted!)
   - folium (experimental for geo-data)
   - plotly (very basic, help wanted!)
   - ascii (experimental)
 * Algorithms for optimized binning
-  - human-friendly
-  - mathematical
+  - pretty (nice rounded bin edges)
+  - mathematical (statistical, quantile-based, geometrical, ...)
 * IO, conversions
   - I/O JSON
   - I/O xarray.DataSet (experimental)
   - O ROOT file (experimental)
   - O pandas.DataFrame (basic)
 
 ### Planned
```

### Comparing `physt-0.6.0a2/pyproject.toml` & `physt-0.6.0a4/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "physt"
-version = "0.6.0a2"
+version = "0.6.0a4"
 description = "P(i/y)thon h(i/y)stograms."
 readme = "README.md"
 requires-python = "~=3.8"
 license = {file = "LICENSE"}
 authors = [
     {name = "Jan Pipek", email="jan.pipek@gmail.com"}
 ]
@@ -14,37 +14,38 @@
         "Intended Audience :: Developers",
         "Intended Audience :: Information Technology",
         "Intended Audience :: Science/Research",
         "Topic :: Scientific/Engineering",
         "Topic :: Software Development :: Libraries :: Python Modules",
 ]
 dependencies = [
-    "numpy>=1.23",
+    "numpy>=1.23,<2.0",
     "packaging",
     "typing_extensions",
     "hypothesis>=6.96.1"
 ]
 
 [project.optional-dependencies]
-dev = ["pytest", "mypy>=1.8", "types-setuptools"]
+dev = ["pytest", "mypy>=1.8", "types-setuptools", "bumpver"]
 # doc = ["sphinx", "sphinx_rtd_theme", "sphixncontrib-apidoc", "nbsphinx"]
 astropy = ["astropy"]
 dask = ["dask[array]>=2023.0"]
 pandas = ["pandas>=1.3"]
 polars = ["polars>=0.20", "pyarrow", "physt[pandas]"]
 xarray = ["xarray"]
 matplotlib = ["matplotlib>=3.0"]
 plotly = ["plotly"]
-vega3 = ["vega3"]
+# TODO: Re-enable vega
+# vega3 = ["vega3"]
 folium = ["folium"]
 root = ["uproot3"]  # TODO: Update to uproot4
 scipy = ["scipy"]
 xtermcolor = ["xtermcolor"]
 all = [
-    "physt[astropy,dev,dask,pandas,polars,xarray,matplotlib,plotly,vega3,folium,root,scipy,xtermcolor]"
+    "physt[astropy,dev,dask,pandas,polars,xarray,matplotlib,plotly,folium,root,scipy,xtermcolor]"
 ]
 
 [build-system]
 requires = ["setuptools>=65.0", "build"]
 build-backend = "setuptools.build_meta"
 
 [tool.black]
@@ -73,20 +74,23 @@
 target-version = "py38"
 
 [tool.ruff.per-file-ignores]
 "tests/*.py" = ["E402"]
 
 
 [tool.bumpver]
-current_version = "0.6.0a2"
-version_pattern = "MAJOR.MINOR.PATCH[PYTAGNUM]"
+current_version = "v0.6.0a4"
+version_pattern = "vMAJOR.MINOR.PATCH[PYTAGNUM]"
 commit_message = "Bump version: {old_version} → {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
 "pyproject.toml" = [
     'current_version = "{version}"',
     'version = "{pep440_version}"']
 "src/physt/version.py" = [
     '__version__ = "{pep440_version}"']
+"conda/meta.yaml" = [
+    '{% set version = "{pep440_version}" %}'
+]
```

### Comparing `physt-0.6.0a2/src/physt/__init__.py` & `physt-0.6.0a4/src/physt/__init__.py`

 * *Files identical despite different names*

### Comparing `physt-0.6.0a2/src/physt/_bin_utils.py` & `physt-0.6.0a4/src/physt/_bin_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -166,45 +166,45 @@
 
 
 def is_bin_superset(sup: ArrayLike, sub: ArrayLike) -> bool:
     """Inverse of is_bin_subset."""
     return is_bin_subset(sub=sub, sup=sup)
 
 
-def find_human_width_decimal(raw_width: float) -> float:
-    """Find the human bin width un decimal scale close to raw_width."""
+def find_pretty_width_decimal(raw_width: float) -> float:
+    """Find the pretty bin width on decimal scale close to raw_width."""
     subscales = np.array([0.5, 1, 2, 2.5, 5, 10])
     power = np.floor(np.log10(raw_width)).astype(int)
     best_index = np.argmin(np.abs(np.log(subscales * (10.0**power) / raw_width)))
     return (10.0**power) * subscales[best_index]
 
 
-def find_human_width_60(raw_width: float) -> int:
-    """Find the best human bin width for seconds and minutes close to raw_width."""
+def find_pretty_width_60(raw_width: float) -> int:
+    """Find the best pretty bin width for seconds and minutes close to raw_width."""
     subscales = np.array([1, 2, 5, 10, 15, 20, 30])
     best_index = np.argmin(np.abs(np.log(subscales / raw_width)))
     return subscales[best_index]
 
 
-def find_human_width_24(raw_width: float) -> int:
-    """Find the best human bin width for hours close to raw_width."""
+def find_pretty_width_24(raw_width: float) -> int:
+    """Find the best pretty bin width for hours close to raw_width."""
     subscales = np.array([1, 2, 3, 4, 6, 12])
     best_index = np.argmin(np.abs(np.log(subscales / raw_width)))
     return subscales[best_index]
 
 
-def find_human_width(raw_width: float, kind: Optional[Literal["time"]] = None) -> float:
-    """Find the best human width close to a given raw_width."""
+def find_pretty_width(raw_width: float, kind: Optional[Literal["time"]] = None) -> float:
+    """Find the best pretty width close to a given raw_width."""
     # TODO: Deal with infinity
     if not kind:
-        return find_human_width_decimal(raw_width)
+        return find_pretty_width_decimal(raw_width)
     if kind == "time":
         if raw_width < 0.8:
-            return find_human_width_decimal(raw_width)
+            return find_pretty_width_decimal(raw_width)
         if raw_width < 50:
-            return find_human_width_60(raw_width)
+            return find_pretty_width_60(raw_width)
         if raw_width < 3000:
-            return find_human_width_60(raw_width / 60) * 60
+            return find_pretty_width_60(raw_width / 60) * 60
         if raw_width < 70000:
-            return find_human_width_24(raw_width / 3600) * 3600
-        return find_human_width_decimal(raw_width / 86400) * 86400
+            return find_pretty_width_24(raw_width / 3600) * 3600
+        return find_pretty_width_decimal(raw_width / 86400) * 86400
     raise ValueError(f"Value of 'kind' not understood: '{kind}'.")
```

### Comparing `physt-0.6.0a2/src/physt/_construction.py` & `physt-0.6.0a4/src/physt/_construction.py`

 * *Files identical despite different names*

### Comparing `physt-0.6.0a2/src/physt/_facade.py` & `physt-0.6.0a4/src/physt/_facade.py`

 * *Files identical despite different names*

### Comparing `physt-0.6.0a2/src/physt/_util.py` & `physt-0.6.0a4/src/physt/_util.py`

 * *Files identical despite different names*

### Comparing `physt-0.6.0a2/src/physt/binnings.py` & `physt-0.6.0a4/src/physt/binnings.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 """Different binning algorithms/schemas for the histograms."""
 from __future__ import annotations
+from functools import wraps
 
 import warnings
 from contextlib import suppress
 from typing import TYPE_CHECKING, cast
 
 import numpy as np
 
 from physt._bin_utils import (
-    find_human_width,
+    find_pretty_width,
     is_bin_subset,
     is_consecutive,
     is_rising,
     make_bin_array,
     to_numpy_bins,
     to_numpy_bins_with_mask,
 )
-from physt._util import find_subclass
+from physt._util import find_subclass, deprecation_alias
 
 if TYPE_CHECKING:
     from typing import (
         Any,
         Callable,
         ClassVar,
         Dict,
@@ -749,15 +750,15 @@
             raise ValueError(
                 f"Range too narrow to split into {bin_count} bins: {start} to {stop}."
             )
     return NumpyBinning(bins)
 
 
 @register_binning()
-def human_binning(
+def pretty_binning(
     data: Optional[np.ndarray],
     bin_count: Optional[int] = None,
     *,
     kind: Optional[Literal["time"]] = None,
     range: Optional[RangeTuple] = None,
     min_bin_width: Optional[float] = None,
     max_bin_width: Optional[float] = None,
@@ -785,24 +786,28 @@
         min_, max_ = range
     if bin_count is None:
         if data is None:
             raise ValueError("Cannot guess optimum bin count without data.")
         bin_count = ideal_bin_count(data)
 
     raw_width = (max_ - min_) / bin_count
-    bin_width = find_human_width(raw_width, kind=kind)
+    bin_width = find_pretty_width(raw_width, kind=kind)
 
     if min_bin_width:
         bin_width = max(bin_width, min_bin_width)
     if max_bin_width:
         bin_width = min(bin_width, max_bin_width)
 
     return fixed_width_binning(bin_width=bin_width, data=data, range=range, **kwargs)
 
 
+human_binning = deprecation_alias(pretty_binning, "human_binning")
+register_binning(name="human")(human_binning)
+
+
 @register_binning()
 def quantile_binning(
     data: Optional[np.ndarray],
     *,
     bin_count: Optional[int] = None,
     q: Optional[Sequence[float]] = None,
     qrange: Optional[RangeTuple] = None,
```

### Comparing `physt-0.6.0a2/src/physt/compat/__init__.py` & `physt-0.6.0a4/src/physt/compat/__init__.py`

 * *Files identical despite different names*

### Comparing `physt-0.6.0a2/src/physt/compat/dask.py` & `physt-0.6.0a4/src/physt/compat/dask.py`

 * *Files identical despite different names*

### Comparing `physt-0.6.0a2/src/physt/compat/geant4.py` & `physt-0.6.0a4/src/physt/compat/geant4.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 """
 import codecs
 from typing import Union
 
 import numpy as np
 
 from physt.binnings import fixed_width_binning
+from physt.statistics import Statistics
 from physt.types import Histogram1D, Histogram2D
 
 
 def load_csv(path: str) -> Union[Histogram1D, Histogram2D]:
     """Loads a histogram as output from Geant4 analysis tools in CSV format.
 
     Parameters
@@ -56,20 +57,25 @@
     _, bin_count, min_, max_ = _get(meta, "axis").split()
     bin_count = int(bin_count)
     min_ = float(min_)
     max_ = float(max_)
     binning = fixed_width_binning(
         bin_width=(max_ - min_) / bin_count, range=(min_, max_)
     )
-    hist = Histogram1D(binning, name=_get(meta, "title"))
-    hist._frequencies = data[1:-1, 1]
-    hist._errors2 = data[1:-1, 2]
-    hist.underflow = data[0, 1]
-    hist.overflow = data[-1, 1]
-    hist._stats = {"sum": data[1:-1, 3].sum(), "sum2": data[1:-1, 4].sum()}
+    stats = Statistics(sum=data[1:-1, 3].sum(), sum2=data[1:-1, 4].sum())
+
+    hist = Histogram1D(
+        binning,
+        frequencies=data[1:-1, 1],
+        errors2=data[1:-1, 2],
+        name=_get(meta, "title"),
+        underflow=data[0, 1],
+        overflow=data[-1, 1],
+        stats=stats
+    )
     return hist
 
 
 def _create_h2(data, meta) -> Histogram2D:
     binnings = []
     axes = _get(meta, "axis", False)
     for axis in axes:
```

### Comparing `physt-0.6.0a2/src/physt/compat/pandas.py` & `physt-0.6.0a4/src/physt/compat/pandas.py`

 * *Files identical despite different names*

### Comparing `physt-0.6.0a2/src/physt/compat/polars.py` & `physt-0.6.0a4/src/physt/compat/polars.py`

 * *Files identical despite different names*

### Comparing `physt-0.6.0a2/src/physt/compat/xarray.py` & `physt-0.6.0a4/src/physt/compat/xarray.py`

 * *Files identical despite different names*

### Comparing `physt-0.6.0a2/src/physt/config.py` & `physt-0.6.0a4/src/physt/config.py`

 * *Files identical despite different names*

### Comparing `physt-0.6.0a2/src/physt/examples/__init__.py` & `physt-0.6.0a4/src/physt/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `physt-0.6.0a2/src/physt/examples/munros.csv` & `physt-0.6.0a4/src/physt/examples/munros.csv`

 * *Files identical despite different names*

### Comparing `physt-0.6.0a2/src/physt/helpers/db.py` & `physt-0.6.0a4/src/physt/helpers/db.py`

 * *Files identical despite different names*

### Comparing `physt-0.6.0a2/src/physt/histogram1d.py` & `physt-0.6.0a4/src/physt/histogram1d.py`

 * *Files identical despite different names*

### Comparing `physt-0.6.0a2/src/physt/histogram_base.py` & `physt-0.6.0a4/src/physt/histogram_base.py`

 * *Files identical despite different names*

### Comparing `physt-0.6.0a2/src/physt/histogram_collection.py` & `physt-0.6.0a4/src/physt/histogram_collection.py`

 * *Files identical despite different names*

### Comparing `physt-0.6.0a2/src/physt/histogram_nd.py` & `physt-0.6.0a4/src/physt/histogram_nd.py`

 * *Files identical despite different names*

### Comparing `physt-0.6.0a2/src/physt/io/__init__.py` & `physt-0.6.0a4/src/physt/io/__init__.py`

 * *Files identical despite different names*

### Comparing `physt-0.6.0a2/src/physt/io/json.py` & `physt-0.6.0a4/src/physt/io/json.py`

 * *Files identical despite different names*

### Comparing `physt-0.6.0a2/src/physt/io/root.py` & `physt-0.6.0a4/src/physt/io/root.py`

 * *Files identical despite different names*

### Comparing `physt-0.6.0a2/src/physt/io/util.py` & `physt-0.6.0a4/src/physt/io/util.py`

 * *Files identical despite different names*

### Comparing `physt-0.6.0a2/src/physt/io/version.py` & `physt-0.6.0a4/src/physt/io/version.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,24 +1,25 @@
-from packaging.version import Version
-from pkg_resources import parse_version
+from typing import Union
+
+from packaging.version import Version, parse
 
 from physt import __version__
 
 CURRENT_VERSION = __version__
 
 
 class VersionError(Exception):
     pass
 
 
-def require_compatible_version(compatible_version, word="File"):
+def require_compatible_version(compatible_version: Union[str, Version], word="File") -> None:
     """Check that compatible version of input data is not too new."""
     if isinstance(compatible_version, str):
-        compatible_version = parse_version(compatible_version)
+        compatible_version = parse(compatible_version)
     elif not isinstance(compatible_version, Version):
         raise ValueError("Type of `compatible_version` not understood.")
 
-    current_version = parse_version(CURRENT_VERSION)
+    current_version = parse(CURRENT_VERSION)
     if current_version < compatible_version:
         raise VersionError(
             f"{word} written for version >= {compatible_version}, this is {CURRENT_VERSION}."
         )
```

### Comparing `physt-0.6.0a2/src/physt/plotting/__init__.py` & `physt-0.6.0a4/src/physt/plotting/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -110,18 +110,19 @@
 
 with suppress(ImportError):
     from . import matplotlib as mpl_backend
 
     backends["matplotlib"] = mpl_backend
 
 
-with suppress(ImportError):
-    from . import vega as vega_backend
+# TODO: Re-enable vega
+# with suppress(ImportError):
+#     from . import vega as vega_backend
 
-    backends["vega"] = vega_backend
+#     backends["vega"] = vega_backend
 
 with suppress(ImportError):
     from . import plotly as plotly_backend
 
     backends["plotly"] = plotly_backend
```

### Comparing `physt-0.6.0a2/src/physt/plotting/ascii.py` & `physt-0.6.0a4/src/physt/plotting/ascii.py`

 * *Files identical despite different names*

### Comparing `physt-0.6.0a2/src/physt/plotting/common.py` & `physt-0.6.0a4/src/physt/plotting/common.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,17 +7,17 @@
 from datetime import timedelta
 from functools import wraps
 from typing import TYPE_CHECKING
 
 import numpy as np
 
 from physt._bin_utils import (
-    find_human_width_24,
-    find_human_width_60,
-    find_human_width_decimal,
+    find_pretty_width_24,
+    find_pretty_width_60,
+    find_pretty_width_decimal,
 )
 
 if TYPE_CHECKING:
     from typing import Any, Callable, Dict, List, Optional, Tuple, Union
 
     from physt.types import Histogram1D, HistogramBase
 
@@ -208,25 +208,25 @@
         raise TypeError(f"Invalid level: {value}")
 
     @classmethod
     def deduce_level(cls, min_: float, max_: float) -> "TimeTickHandler.LevelType":
         """Determine the level of the tick handler from the histogram range."""
         ideal_width = (max_ - min_) / 6
         if ideal_width < 0.8:
-            return ("sec", find_human_width_decimal(ideal_width))
+            return ("sec", find_pretty_width_decimal(ideal_width))
         elif ideal_width < 50:
-            return ("sec", find_human_width_60(ideal_width))
+            return ("sec", find_pretty_width_60(ideal_width))
         elif ideal_width < 3000:
-            return ("min", find_human_width_60(ideal_width / 60))
+            return ("min", find_pretty_width_60(ideal_width / 60))
         elif ideal_width < 70000:
-            return ("hour", find_human_width_24(ideal_width / 3600))
+            return ("hour", find_pretty_width_24(ideal_width / 3600))
         else:
             return (
                 "day",
-                find_human_width_decimal(ideal_width / 86400),
+                find_pretty_width_decimal(ideal_width / 86400),
             )  # # noqa: FURB126
 
     def get_time_ticks(
         self, h1: Histogram1D, level: LevelType, min_: float, max_: float
     ) -> List[float]:
         """Get ticks for a given level."""
         # TODO: Change to class method?
```

### Comparing `physt-0.6.0a2/src/physt/plotting/folium.py` & `physt-0.6.0a4/src/physt/plotting/folium.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,15 +64,15 @@
     }
 
 
 def geo_map(
     h2: Histogram2D,
     *,
     map: Optional[Map] = None,
-    tiles: str = "stamenterrain",
+    tiles: Optional[str] = "cartodb positron",
     cmap="wk",
     alpha: float = 0.5,
     lw=1,
     fit_bounds: Optional[bool] = None,
     layer_name: Optional[str] = None,
 ) -> Map:
     """Show rectangular grid over a map.
```

### Comparing `physt-0.6.0a2/src/physt/plotting/matplotlib.py` & `physt-0.6.0a4/src/physt/plotting/matplotlib.py`

 * *Files identical despite different names*

### Comparing `physt-0.6.0a2/src/physt/plotting/plotly.py` & `physt-0.6.0a4/src/physt/plotting/plotly.py`

 * *Files identical despite different names*

### Comparing `physt-0.6.0a2/src/physt/plotting/vega.py` & `physt-0.6.0a4/src/physt/plotting/vega.py`

 * *Files identical despite different names*

### Comparing `physt-0.6.0a2/src/physt/special_histograms.py` & `physt-0.6.0a4/src/physt/special_histograms.py`

 * *Files identical despite different names*

### Comparing `physt-0.6.0a2/src/physt/statistics.py` & `physt-0.6.0a4/src/physt/statistics.py`

 * *Files identical despite different names*

### Comparing `physt-0.6.0a2/src/physt/testing/__init__.py` & `physt-0.6.0a4/src/physt/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `physt-0.6.0a2/src/physt/testing/strategies.py` & `physt-0.6.0a4/src/physt/testing/strategies.py`

 * *Files identical despite different names*

### Comparing `physt-0.6.0a2/src/physt.egg-info/PKG-INFO` & `physt-0.6.0a4/src/physt.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: physt
-Version: 0.6.0a2
+Version: 0.6.0a4
 Summary: P(i/y)thon h(i/y)stograms.
 Author-email: Jan Pipek <jan.pipek@gmail.com>
 License: The MIT License (MIT)
         
         Copyright (c) 2016-2024 Jan Pipek
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -31,22 +31,23 @@
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: ~=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: numpy>=1.23
+Requires-Dist: numpy<2.0,>=1.23
 Requires-Dist: packaging
 Requires-Dist: typing_extensions
 Requires-Dist: hypothesis>=6.96.1
 Provides-Extra: dev
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: mypy>=1.8; extra == "dev"
 Requires-Dist: types-setuptools; extra == "dev"
+Requires-Dist: bumpver; extra == "dev"
 Provides-Extra: astropy
 Requires-Dist: astropy; extra == "astropy"
 Provides-Extra: dask
 Requires-Dist: dask[array]>=2023.0; extra == "dask"
 Provides-Extra: pandas
 Requires-Dist: pandas>=1.3; extra == "pandas"
 Provides-Extra: polars
@@ -55,26 +56,24 @@
 Requires-Dist: physt[pandas]; extra == "polars"
 Provides-Extra: xarray
 Requires-Dist: xarray; extra == "xarray"
 Provides-Extra: matplotlib
 Requires-Dist: matplotlib>=3.0; extra == "matplotlib"
 Provides-Extra: plotly
 Requires-Dist: plotly; extra == "plotly"
-Provides-Extra: vega3
-Requires-Dist: vega3; extra == "vega3"
 Provides-Extra: folium
 Requires-Dist: folium; extra == "folium"
 Provides-Extra: root
 Requires-Dist: uproot3; extra == "root"
 Provides-Extra: scipy
 Requires-Dist: scipy; extra == "scipy"
 Provides-Extra: xtermcolor
 Requires-Dist: xtermcolor; extra == "xtermcolor"
 Provides-Extra: all
-Requires-Dist: physt[astropy,dask,dev,folium,matplotlib,pandas,plotly,polars,root,scipy,vega3,xarray,xtermcolor]; extra == "all"
+Requires-Dist: physt[astropy,dask,dev,folium,matplotlib,pandas,plotly,polars,root,scipy,xarray,xtermcolor]; extra == "all"
 
 # physt ![Physt logo](doc/physt-logo64.png)
 
 
 
 P(i/y)thon h(i/y)stograms. Inspired (and based on) numpy.histogram, but designed for humans(TM) on steroids(TM).
 
@@ -113,15 +112,15 @@
 ## 2D example
 
 ```python
 from physt import h2
 import seaborn as sns
 
 iris = sns.load_dataset('iris')
-iris_hist = h2(iris["sepal_length"], iris["sepal_width"], "human", bin_count=[12, 7], name="Iris")
+iris_hist = h2(iris["sepal_length"], iris["sepal_width"], "pretty", bin_count=[12, 7], name="Iris")
 iris_hist.plot(show_zero=False, cmap="gray_r", show_values=True);
 ```
 
 ![Iris 2D plot](doc/iris-2d.png)
 
 ## 3D directional example
 
@@ -189,16 +188,16 @@
 * Plotting with several backends
   - matplotlib (static plots with many options)
   - vega (interactive plots, beta, help wanted!)
   - folium (experimental for geo-data)
   - plotly (very basic, help wanted!)
   - ascii (experimental)
 * Algorithms for optimized binning
-  - human-friendly
-  - mathematical
+  - pretty (nice rounded bin edges)
+  - mathematical (statistical, quantile-based, geometrical, ...)
 * IO, conversions
   - I/O JSON
   - I/O xarray.DataSet (experimental)
   - O ROOT file (experimental)
   - O pandas.DataFrame (basic)
 
 ### Planned
```

### Comparing `physt-0.6.0a2/src/physt.egg-info/SOURCES.txt` & `physt-0.6.0a4/src/physt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `physt-0.6.0a2/tests/data/geant-h1.csv` & `physt-0.6.0a4/tests/data/geant-h1.csv`

 * *Files identical despite different names*

### Comparing `physt-0.6.0a2/tests/data/geant-h2.csv` & `physt-0.6.0a4/tests/data/geant-h2.csv`

 * *Files identical despite different names*

### Comparing `physt-0.6.0a2/tests/test_adaptive.py` & `physt-0.6.0a4/tests/test_adaptive.py`

 * *Files identical despite different names*

### Comparing `physt-0.6.0a2/tests/test_bin_utils.py` & `physt-0.6.0a4/tests/test_bin_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import numpy as np
 import pytest
 
 from physt._bin_utils import (
-    find_human_width,
+    find_pretty_width,
     is_consecutive,
     is_rising,
     make_bin_array,
     to_numpy_bins_with_mask,
 )
 
 
@@ -80,15 +80,15 @@
             assert not is_consecutive((np.array(sequence)))
 
 
 class TestFindHumanWidth:
     def test_normal(self):
         invalues = [1.1, 2.4, 32, 57, 2000, 3621, 85000]
         expected = [1.0, 2.5, 25, 50, 2000, 5000, 1e5]
-        result = [find_human_width(x) for x in invalues]
+        result = [find_pretty_width(x) for x in invalues]
         assert np.array_equal(result, expected)
 
     def test_time(self):
         invalues = [1.1, 2.4, 32, 57, 2000, 3621, 85000]
         expected = [1.0, 2.0, 30, 60, 1800, 3600, 86400]
-        result = [find_human_width(x, kind="time") for x in invalues]
+        result = [find_pretty_width(x, kind="time") for x in invalues]
         assert np.array_equal(result, expected)
```

### Comparing `physt-0.6.0a2/tests/test_binning.py` & `physt-0.6.0a4/tests/test_binning.py`

 * *Files 5% similar despite different names*

```diff
@@ -138,33 +138,33 @@
         b3 = binnings.FixedWidthBinning(bin_width=5, bin_count=6, min=0, adaptive=True)
         with pytest.raises(ValueError):
             b1.adapt(b3)
         with pytest.raises(ValueError):
             b3.adapt(b1)
 
 
-class TestHumanBins:
+class TestPrettyBins:
     def test_exact(self):
         data = np.random.rand(1000)
-        the_binning = binnings.human_binning(data, 10)
+        the_binning = binnings.pretty_binning(data, 10)
         assert np.allclose(the_binning.numpy_bins, np.linspace(0, 1, 11))
 
-        the_binning = binnings.human_binning(data, 9)
+        the_binning = binnings.pretty_binning(data, 9)
         assert np.allclose(the_binning.numpy_bins, np.linspace(0, 1, 11))
 
-        the_binning = binnings.human_binning(data, 11)
+        the_binning = binnings.pretty_binning(data, 11)
         assert np.allclose(the_binning.numpy_bins, np.linspace(0, 1, 11))
 
     def test_min_max_bin_width(self):
         data = np.random.rand(1000)
 
-        the_binning = binnings.human_binning(data, min_bin_width=0.3)
+        the_binning = binnings.pretty_binning(data, min_bin_width=0.3)
         assert the_binning.bin_width == 0.3
 
-        the_binning = binnings.human_binning(data, max_bin_width=0.001)
+        the_binning = binnings.pretty_binning(data, max_bin_width=0.001)
         assert the_binning.bin_width == 0.001
 
 
 class TestIntegerBins:
     def test_dice(self):
         data = np.asarray([1, 2, 3, 5, 6, 2, 4, 3, 2, 3, 4, 5, 6, 6, 1, 2, 5])
         the_binning = binnings.integer_binning(data)
```

### Comparing `physt-0.6.0a2/tests/test_construction.py` & `physt-0.6.0a4/tests/test_construction.py`

 * *Files identical despite different names*

### Comparing `physt-0.6.0a2/tests/test_examples.py` & `physt-0.6.0a4/tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `physt-0.6.0a2/tests/test_facade.py` & `physt-0.6.0a4/tests/test_facade.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,25 +15,30 @@
 from physt._facade import h1, h2
 from physt.types import Histogram1D, Histogram2D
 
 
 class TestH1:
     class TestNoArgs:
         @given(
-            array=arrays(
-                dtype=floating_dtypes() | integer_dtypes(),
-                shape=array_shapes(),
-                unique=True,
+            array=st.one_of(
+                arrays(
+                    dtype=floating_dtypes(),
+                    shape=array_shapes(min_side=2),
+                    unique=True,
+                    elements=st.floats(allow_nan=False, allow_infinity=False, allow_subnormal=False),
+                ),
+                arrays(
+                    dtype=integer_dtypes(),
+                    shape=array_shapes(min_side=2),
+                    unique=True,
+                ),
             )
         )
         def test_array_at_least_two_different_values(self, array):
             # Reasonable defaults for at least two different values
-            assume(array.size > 2)
-            assume(np.isfinite(array).all())
-
             # Avoid too narrow ranges in float precision
             array_range = array.max() - array.min()
             assume(array_range > np.spacing(array.min()) * 20)
 
             histogram = h1(array)
             assert isinstance(histogram, Histogram1D)
             assert histogram.bin_right_edges[-1] >= array.max()
```

### Comparing `physt-0.6.0a2/tests/test_histogram.py` & `physt-0.6.0a4/tests/test_histogram.py`

 * *Files identical despite different names*

### Comparing `physt-0.6.0a2/tests/test_histogram1d.py` & `physt-0.6.0a4/tests/test_histogram1d.py`

 * *Files identical despite different names*

### Comparing `physt-0.6.0a2/tests/test_histogram2d.py` & `physt-0.6.0a4/tests/test_histogram2d.py`

 * *Files identical despite different names*

### Comparing `physt-0.6.0a2/tests/test_histogramnd.py` & `physt-0.6.0a4/tests/test_histogramnd.py`

 * *Files identical despite different names*

### Comparing `physt-0.6.0a2/tests/test_io.py` & `physt-0.6.0a4/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `physt-0.6.0a2/tests/test_special.py` & `physt-0.6.0a4/tests/test_special.py`

 * *Files identical despite different names*

### Comparing `physt-0.6.0a2/tests/test_stats.py` & `physt-0.6.0a4/tests/test_stats.py`

 * *Files identical despite different names*

