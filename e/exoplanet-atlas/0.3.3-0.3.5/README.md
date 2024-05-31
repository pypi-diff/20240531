# Comparing `tmp/exoplanet_atlas-0.3.3.tar.gz` & `tmp/exoplanet_atlas-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "exoplanet_atlas-0.3.3.tar", last modified: Thu May 23 06:46:05 2024, max compression
+gzip compressed data, was "exoplanet_atlas-0.3.5.tar", last modified: Fri May 31 20:21:31 2024, max compression
```

## Comparing `exoplanet_atlas-0.3.3.tar` & `exoplanet_atlas-0.3.5.tar`

### file list

```diff
@@ -1,82 +1,82 @@
-drwxr-xr-x   0 zach       (502) staff       (20)        0 2024-05-23 06:46:05.430907 exoplanet_atlas-0.3.3/
--rw-r--r--   0 zach       (502) staff       (20)     1091 2024-05-20 20:56:00.000000 exoplanet_atlas-0.3.3/LICENSE
--rw-r--r--   0 zach       (502) staff       (20)     1533 2024-05-23 06:46:05.430569 exoplanet_atlas-0.3.3/PKG-INFO
--rw-r--r--   0 zach       (502) staff       (20)     1921 2024-05-20 18:20:59.000000 exoplanet_atlas-0.3.3/README.md
-drwxr-xr-x   0 zach       (502) staff       (20)        0 2024-05-23 06:46:05.408072 exoplanet_atlas-0.3.3/exoatlas/
--rw-r--r--   0 zach       (502) staff       (20)      179 2024-05-20 20:56:00.000000 exoplanet_atlas-0.3.3/exoatlas/__init__.py
--rw-r--r--   0 zach       (502) staff       (20)     4483 2024-05-23 06:36:30.000000 exoplanet_atlas-0.3.3/exoatlas/imports.py
-drwxr-xr-x   0 zach       (502) staff       (20)        0 2024-05-23 06:46:05.410150 exoplanet_atlas-0.3.3/exoatlas/models/
--rw-r--r--   0 zach       (502) staff       (20)       87 2024-05-20 18:20:59.000000 exoplanet_atlas-0.3.3/exoatlas/models/__init__.py
--rw-r--r--   0 zach       (502) staff       (20)     2084 2024-05-20 18:20:59.000000 exoplanet_atlas-0.3.3/exoatlas/models/chen.py
--rw-r--r--   0 zach       (502) staff       (20)     1541 2024-05-20 20:56:00.000000 exoplanet_atlas-0.3.3/exoatlas/models/kopparapu.py
--rw-r--r--   0 zach       (502) staff       (20)     1171 2024-05-20 20:56:00.000000 exoplanet_atlas-0.3.3/exoatlas/models/seager.py
--rw-r--r--   0 zach       (502) staff       (20)      963 2024-05-20 20:56:00.000000 exoplanet_atlas-0.3.3/exoatlas/models/zeng.py
-drwxr-xr-x   0 zach       (502) staff       (20)        0 2024-05-23 06:46:05.415813 exoplanet_atlas-0.3.3/exoatlas/populations/
--rw-r--r--   0 zach       (502) staff       (20)    13402 2024-05-20 20:56:00.000000 exoplanet_atlas-0.3.3/exoatlas/populations/Exoplanets.py
--rw-r--r--   0 zach       (502) staff       (20)    51413 2024-05-23 06:36:30.000000 exoplanet_atlas-0.3.3/exoatlas/populations/Population.py
--rw-r--r--   0 zach       (502) staff       (20)     3598 2024-05-23 06:36:30.000000 exoplanet_atlas-0.3.3/exoatlas/populations/SolarSystem.py
--rw-r--r--   0 zach       (502) staff       (20)       62 2024-05-20 18:20:59.000000 exoplanet_atlas-0.3.3/exoatlas/populations/TESS.py
--rw-r--r--   0 zach       (502) staff       (20)     7538 2024-05-20 20:56:00.000000 exoplanet_atlas-0.3.3/exoatlas/populations/TOI.py
--rw-r--r--   0 zach       (502) staff       (20)     3485 2024-05-20 18:20:59.000000 exoplanet_atlas-0.3.3/exoatlas/populations/TOISubsets.py
--rw-r--r--   0 zach       (502) staff       (20)     3351 2024-05-20 18:20:59.000000 exoplanet_atlas-0.3.3/exoatlas/populations/TransitingExoplanets.py
--rw-r--r--   0 zach       (502) staff       (20)     5718 2024-05-20 20:56:00.000000 exoplanet_atlas-0.3.3/exoatlas/populations/TransitingExoplanetsSubsets.py
--rw-r--r--   0 zach       (502) staff       (20)      416 2024-05-20 18:20:59.000000 exoplanet_atlas-0.3.3/exoatlas/populations/__init__.py
--rw-r--r--   0 zach       (502) staff       (20)      716 2024-05-20 18:20:59.000000 exoplanet_atlas-0.3.3/exoatlas/populations/collections.py
--rw-r--r--   0 zach       (502) staff       (20)     2258 2024-05-20 20:56:00.000000 exoplanet_atlas-0.3.3/exoatlas/populations/column_descriptions.py
-drwxr-xr-x   0 zach       (502) staff       (20)        0 2024-05-23 06:46:05.416800 exoplanet_atlas-0.3.3/exoatlas/populations/curation/
--rw-r--r--   0 zach       (502) staff       (20)     7747 2024-05-20 20:56:00.000000 exoplanet_atlas-0.3.3/exoatlas/populations/curation/Confirmed.py
--rw-r--r--   0 zach       (502) staff       (20)       26 2024-05-20 18:20:59.000000 exoplanet_atlas-0.3.3/exoatlas/populations/curation/TransitingExoplanets.py
--rw-r--r--   0 zach       (502) staff       (20)        0 2024-05-20 18:20:59.000000 exoplanet_atlas-0.3.3/exoatlas/populations/curation/__init__.py
--rw-r--r--   0 zach       (502) staff       (20)     8991 2024-05-20 20:56:00.000000 exoplanet_atlas-0.3.3/exoatlas/populations/downloaders.py
--rw-r--r--   0 zach       (502) staff       (20)     1963 2024-05-20 20:56:00.000000 exoplanet_atlas-0.3.3/exoatlas/populations/summary.py
--rw-r--r--   0 zach       (502) staff       (20)     2735 2024-05-20 20:56:00.000000 exoplanet_atlas-0.3.3/exoatlas/talker.py
-drwxr-xr-x   0 zach       (502) staff       (20)        0 2024-05-23 06:46:05.417321 exoplanet_atlas-0.3.3/exoatlas/telescopes/
--rw-r--r--   0 zach       (502) staff       (20)       23 2024-05-20 18:20:59.000000 exoplanet_atlas-0.3.3/exoatlas/telescopes/__init__.py
--rw-r--r--   0 zach       (502) staff       (20)     6048 2024-05-23 06:36:30.000000 exoplanet_atlas-0.3.3/exoatlas/telescopes/buckets.py
-drwxr-xr-x   0 zach       (502) staff       (20)        0 2024-05-23 06:46:05.420467 exoplanet_atlas-0.3.3/exoatlas/tests/
--rw-r--r--   0 zach       (502) staff       (20)      268 2024-05-20 18:20:59.000000 exoplanet_atlas-0.3.3/exoatlas/tests/__init__.py
--rw-r--r--   0 zach       (502) staff       (20)       40 2024-05-20 20:56:00.000000 exoplanet_atlas-0.3.3/exoatlas/tests/setup_tests.py
--rw-r--r--   0 zach       (502) staff       (20)     1070 2024-05-20 20:56:00.000000 exoplanet_atlas-0.3.3/exoatlas/tests/test_buckets.py
--rw-r--r--   0 zach       (502) staff       (20)      578 2024-05-20 20:56:00.000000 exoplanet_atlas-0.3.3/exoatlas/tests/test_downloaders.py
--rw-r--r--   0 zach       (502) staff       (20)      363 2024-05-20 20:56:00.000000 exoplanet_atlas-0.3.3/exoatlas/tests/test_imports.py
--rw-r--r--   0 zach       (502) staff       (20)      675 2024-05-20 20:56:00.000000 exoplanet_atlas-0.3.3/exoatlas/tests/test_models.py
--rw-r--r--   0 zach       (502) staff       (20)     3284 2024-05-20 20:56:00.000000 exoplanet_atlas-0.3.3/exoatlas/tests/test_populations.py
--rw-r--r--   0 zach       (502) staff       (20)     2489 2024-05-20 20:56:00.000000 exoplanet_atlas-0.3.3/exoatlas/tests/test_snr.py
--rw-r--r--   0 zach       (502) staff       (20)      612 2024-05-20 20:56:00.000000 exoplanet_atlas-0.3.3/exoatlas/tests/test_uncertainties.py
--rw-r--r--   0 zach       (502) staff       (20)     1390 2024-05-20 20:56:00.000000 exoplanet_atlas-0.3.3/exoatlas/tests/test_visualizations.py
--rw-r--r--   0 zach       (502) staff       (20)      701 2024-05-20 20:56:00.000000 exoplanet_atlas-0.3.3/exoatlas/tests/test_whatsup.py
--rw-r--r--   0 zach       (502) staff       (20)       62 2024-05-23 06:36:30.000000 exoplanet_atlas-0.3.3/exoatlas/version.py
-drwxr-xr-x   0 zach       (502) staff       (20)        0 2024-05-23 06:46:05.422507 exoplanet_atlas-0.3.3/exoatlas/visualizations/
--rw-r--r--   0 zach       (502) staff       (20)     4131 2024-05-20 18:20:59.000000 exoplanet_atlas-0.3.3/exoatlas/visualizations/MultiPanel.py
--rw-r--r--   0 zach       (502) staff       (20)      790 2024-05-20 18:20:59.000000 exoplanet_atlas-0.3.3/exoatlas/visualizations/ThumbtackMovie.py
--rw-r--r--   0 zach       (502) staff       (20)    14017 2024-05-20 18:20:59.000000 exoplanet_atlas-0.3.3/exoatlas/visualizations/ThumbtackPlot.py
--rw-r--r--   0 zach       (502) staff       (20)       95 2024-05-20 18:20:59.000000 exoplanet_atlas-0.3.3/exoatlas/visualizations/__init__.py
-drwxr-xr-x   0 zach       (502) staff       (20)        0 2024-05-23 06:46:05.423253 exoplanet_atlas-0.3.3/exoatlas/visualizations/axes/
--rw-r--r--   0 zach       (502) staff       (20)       58 2024-05-20 18:20:59.000000 exoplanet_atlas-0.3.3/exoatlas/visualizations/axes/__init__.py
--rw-r--r--   0 zach       (502) staff       (20)     4309 2024-05-20 18:20:59.000000 exoplanet_atlas-0.3.3/exoatlas/visualizations/axes/plottable.py
--rw-r--r--   0 zach       (502) staff       (20)    13910 2024-05-23 06:36:30.000000 exoplanet_atlas-0.3.3/exoatlas/visualizations/axes/preset_plottables.py
--rw-r--r--   0 zach       (502) staff       (20)     8240 2024-05-23 06:36:30.000000 exoplanet_atlas-0.3.3/exoatlas/visualizations/buildable.py
--rw-r--r--   0 zach       (502) staff       (20)     2846 2024-05-20 20:56:00.000000 exoplanet_atlas-0.3.3/exoatlas/visualizations/ink_errorbar.py
-drwxr-xr-x   0 zach       (502) staff       (20)        0 2024-05-23 06:46:05.424922 exoplanet_atlas-0.3.3/exoatlas/visualizations/panels/
--rw-r--r--   0 zach       (502) staff       (20)     9710 2024-05-20 20:56:00.000000 exoplanet_atlas-0.3.3/exoatlas/visualizations/panels/BubblePanel.py
--rw-r--r--   0 zach       (502) staff       (20)     7716 2024-05-23 06:36:30.000000 exoplanet_atlas-0.3.3/exoatlas/visualizations/panels/ErrorPanel.py
--rw-r--r--   0 zach       (502) staff       (20)    12096 2024-05-20 18:20:59.000000 exoplanet_atlas-0.3.3/exoatlas/visualizations/panels/Panel.py
--rw-r--r--   0 zach       (502) staff       (20)      103 2024-05-20 18:20:59.000000 exoplanet_atlas-0.3.3/exoatlas/visualizations/panels/__init__.py
--rw-r--r--   0 zach       (502) staff       (20)     9782 2024-05-20 18:20:59.000000 exoplanet_atlas-0.3.3/exoatlas/visualizations/panels/preset_panels.py
--rw-r--r--   0 zach       (502) staff       (20)      858 2024-05-20 18:20:59.000000 exoplanet_atlas-0.3.3/exoatlas/visualizations/tweaks.py
-drwxr-xr-x   0 zach       (502) staff       (20)        0 2024-05-23 06:46:05.427521 exoplanet_atlas-0.3.3/exoatlas/whatsup/
--rw-r--r--   0 zach       (502) staff       (20)      164 2024-05-20 18:20:59.000000 exoplanet_atlas-0.3.3/exoatlas/whatsup/__init__.py
--rw-r--r--   0 zach       (502) staff       (20)     2073 2024-05-20 18:20:59.000000 exoplanet_atlas-0.3.3/exoatlas/whatsup/block.py
--rw-r--r--   0 zach       (502) staff       (20)      111 2024-05-20 18:20:59.000000 exoplanet_atlas-0.3.3/exoatlas/whatsup/night.py
--rw-r--r--   0 zach       (502) staff       (20)     6515 2024-05-20 18:20:59.000000 exoplanet_atlas-0.3.3/exoatlas/whatsup/observatory.py
--rw-r--r--   0 zach       (502) staff       (20)    11246 2024-05-20 20:56:00.000000 exoplanet_atlas-0.3.3/exoatlas/whatsup/plan.py
--rw-r--r--   0 zach       (502) staff       (20)     5940 2024-05-20 20:56:00.000000 exoplanet_atlas-0.3.3/exoatlas/whatsup/transit.py
-drwxr-xr-x   0 zach       (502) staff       (20)        0 2024-05-23 06:46:05.429070 exoplanet_atlas-0.3.3/exoplanet_atlas.egg-info/
--rw-r--r--   0 zach       (502) staff       (20)     1533 2024-05-23 06:46:05.000000 exoplanet_atlas-0.3.3/exoplanet_atlas.egg-info/PKG-INFO
--rw-r--r--   0 zach       (502) staff       (20)     2288 2024-05-23 06:46:05.000000 exoplanet_atlas-0.3.3/exoplanet_atlas.egg-info/SOURCES.txt
--rw-r--r--   0 zach       (502) staff       (20)        1 2024-05-23 06:46:05.000000 exoplanet_atlas-0.3.3/exoplanet_atlas.egg-info/dependency_links.txt
--rw-r--r--   0 zach       (502) staff       (20)        1 2024-05-20 18:33:32.000000 exoplanet_atlas-0.3.3/exoplanet_atlas.egg-info/not-zip-safe
--rw-r--r--   0 zach       (502) staff       (20)      300 2024-05-23 06:46:05.000000 exoplanet_atlas-0.3.3/exoplanet_atlas.egg-info/requires.txt
--rw-r--r--   0 zach       (502) staff       (20)        9 2024-05-23 06:46:05.000000 exoplanet_atlas-0.3.3/exoplanet_atlas.egg-info/top_level.txt
--rw-r--r--   0 zach       (502) staff       (20)       38 2024-05-23 06:46:05.430973 exoplanet_atlas-0.3.3/setup.cfg
--rw-r--r--   0 zach       (502) staff       (20)     4028 2024-05-23 06:36:30.000000 exoplanet_atlas-0.3.3/setup.py
+drwxr-xr-x   0 zach       (502) staff       (20)        0 2024-05-31 20:21:31.520286 exoplanet_atlas-0.3.5/
+-rw-r--r--   0 zach       (502) staff       (20)     1091 2024-05-20 20:56:00.000000 exoplanet_atlas-0.3.5/LICENSE
+-rw-r--r--   0 zach       (502) staff       (20)     1533 2024-05-31 20:21:31.520050 exoplanet_atlas-0.3.5/PKG-INFO
+-rw-r--r--   0 zach       (502) staff       (20)     1942 2024-05-31 20:01:26.000000 exoplanet_atlas-0.3.5/README.md
+drwxr-xr-x   0 zach       (502) staff       (20)        0 2024-05-31 20:21:31.497843 exoplanet_atlas-0.3.5/exoplanet_atlas/
+-rw-r--r--   0 zach       (502) staff       (20)      179 2024-05-20 20:56:00.000000 exoplanet_atlas-0.3.5/exoplanet_atlas/__init__.py
+-rw-r--r--   0 zach       (502) staff       (20)     4742 2024-05-31 20:09:38.000000 exoplanet_atlas-0.3.5/exoplanet_atlas/imports.py
+drwxr-xr-x   0 zach       (502) staff       (20)        0 2024-05-31 20:21:31.501981 exoplanet_atlas-0.3.5/exoplanet_atlas/models/
+-rw-r--r--   0 zach       (502) staff       (20)       87 2024-05-20 18:20:59.000000 exoplanet_atlas-0.3.5/exoplanet_atlas/models/__init__.py
+-rw-r--r--   0 zach       (502) staff       (20)     2084 2024-05-20 18:20:59.000000 exoplanet_atlas-0.3.5/exoplanet_atlas/models/chen.py
+-rw-r--r--   0 zach       (502) staff       (20)     1541 2024-05-20 20:56:00.000000 exoplanet_atlas-0.3.5/exoplanet_atlas/models/kopparapu.py
+-rw-r--r--   0 zach       (502) staff       (20)     1171 2024-05-20 20:56:00.000000 exoplanet_atlas-0.3.5/exoplanet_atlas/models/seager.py
+-rw-r--r--   0 zach       (502) staff       (20)      963 2024-05-20 20:56:00.000000 exoplanet_atlas-0.3.5/exoplanet_atlas/models/zeng.py
+drwxr-xr-x   0 zach       (502) staff       (20)        0 2024-05-31 20:21:31.505835 exoplanet_atlas-0.3.5/exoplanet_atlas/populations/
+-rw-r--r--   0 zach       (502) staff       (20)    13402 2024-05-20 20:56:00.000000 exoplanet_atlas-0.3.5/exoplanet_atlas/populations/Exoplanets.py
+-rw-r--r--   0 zach       (502) staff       (20)    51427 2024-05-31 20:01:16.000000 exoplanet_atlas-0.3.5/exoplanet_atlas/populations/Population.py
+-rw-r--r--   0 zach       (502) staff       (20)     3598 2024-05-23 06:36:30.000000 exoplanet_atlas-0.3.5/exoplanet_atlas/populations/SolarSystem.py
+-rw-r--r--   0 zach       (502) staff       (20)       62 2024-05-20 18:20:59.000000 exoplanet_atlas-0.3.5/exoplanet_atlas/populations/TESS.py
+-rw-r--r--   0 zach       (502) staff       (20)     7538 2024-05-20 20:56:00.000000 exoplanet_atlas-0.3.5/exoplanet_atlas/populations/TOI.py
+-rw-r--r--   0 zach       (502) staff       (20)     3485 2024-05-20 18:20:59.000000 exoplanet_atlas-0.3.5/exoplanet_atlas/populations/TOISubsets.py
+-rw-r--r--   0 zach       (502) staff       (20)     3351 2024-05-20 18:20:59.000000 exoplanet_atlas-0.3.5/exoplanet_atlas/populations/TransitingExoplanets.py
+-rw-r--r--   0 zach       (502) staff       (20)     5718 2024-05-20 20:56:00.000000 exoplanet_atlas-0.3.5/exoplanet_atlas/populations/TransitingExoplanetsSubsets.py
+-rw-r--r--   0 zach       (502) staff       (20)      416 2024-05-20 18:20:59.000000 exoplanet_atlas-0.3.5/exoplanet_atlas/populations/__init__.py
+-rw-r--r--   0 zach       (502) staff       (20)      716 2024-05-20 18:20:59.000000 exoplanet_atlas-0.3.5/exoplanet_atlas/populations/collections.py
+-rw-r--r--   0 zach       (502) staff       (20)     2258 2024-05-20 20:56:00.000000 exoplanet_atlas-0.3.5/exoplanet_atlas/populations/column_descriptions.py
+drwxr-xr-x   0 zach       (502) staff       (20)        0 2024-05-31 20:21:31.506271 exoplanet_atlas-0.3.5/exoplanet_atlas/populations/curation/
+-rw-r--r--   0 zach       (502) staff       (20)     7747 2024-05-20 20:56:00.000000 exoplanet_atlas-0.3.5/exoplanet_atlas/populations/curation/Confirmed.py
+-rw-r--r--   0 zach       (502) staff       (20)       26 2024-05-20 18:20:59.000000 exoplanet_atlas-0.3.5/exoplanet_atlas/populations/curation/TransitingExoplanets.py
+-rw-r--r--   0 zach       (502) staff       (20)        0 2024-05-20 18:20:59.000000 exoplanet_atlas-0.3.5/exoplanet_atlas/populations/curation/__init__.py
+-rw-r--r--   0 zach       (502) staff       (20)     9005 2024-05-31 20:01:16.000000 exoplanet_atlas-0.3.5/exoplanet_atlas/populations/downloaders.py
+-rw-r--r--   0 zach       (502) staff       (20)     1963 2024-05-20 20:56:00.000000 exoplanet_atlas-0.3.5/exoplanet_atlas/populations/summary.py
+-rw-r--r--   0 zach       (502) staff       (20)     2735 2024-05-20 20:56:00.000000 exoplanet_atlas-0.3.5/exoplanet_atlas/talker.py
+drwxr-xr-x   0 zach       (502) staff       (20)        0 2024-05-31 20:21:31.506642 exoplanet_atlas-0.3.5/exoplanet_atlas/telescopes/
+-rw-r--r--   0 zach       (502) staff       (20)       23 2024-05-20 18:20:59.000000 exoplanet_atlas-0.3.5/exoplanet_atlas/telescopes/__init__.py
+-rw-r--r--   0 zach       (502) staff       (20)     6048 2024-05-23 06:36:30.000000 exoplanet_atlas-0.3.5/exoplanet_atlas/telescopes/buckets.py
+drwxr-xr-x   0 zach       (502) staff       (20)        0 2024-05-31 20:21:31.509121 exoplanet_atlas-0.3.5/exoplanet_atlas/tests/
+-rw-r--r--   0 zach       (502) staff       (20)      268 2024-05-20 18:20:59.000000 exoplanet_atlas-0.3.5/exoplanet_atlas/tests/__init__.py
+-rw-r--r--   0 zach       (502) staff       (20)       40 2024-05-20 20:56:00.000000 exoplanet_atlas-0.3.5/exoplanet_atlas/tests/setup_tests.py
+-rw-r--r--   0 zach       (502) staff       (20)     1084 2024-05-31 20:01:16.000000 exoplanet_atlas-0.3.5/exoplanet_atlas/tests/test_buckets.py
+-rw-r--r--   0 zach       (502) staff       (20)      592 2024-05-31 20:01:16.000000 exoplanet_atlas-0.3.5/exoplanet_atlas/tests/test_downloaders.py
+-rw-r--r--   0 zach       (502) staff       (20)      370 2024-05-31 20:01:16.000000 exoplanet_atlas-0.3.5/exoplanet_atlas/tests/test_imports.py
+-rw-r--r--   0 zach       (502) staff       (20)      689 2024-05-31 20:01:16.000000 exoplanet_atlas-0.3.5/exoplanet_atlas/tests/test_models.py
+-rw-r--r--   0 zach       (502) staff       (20)     3298 2024-05-31 20:01:16.000000 exoplanet_atlas-0.3.5/exoplanet_atlas/tests/test_populations.py
+-rw-r--r--   0 zach       (502) staff       (20)     2496 2024-05-31 20:01:16.000000 exoplanet_atlas-0.3.5/exoplanet_atlas/tests/test_snr.py
+-rw-r--r--   0 zach       (502) staff       (20)      626 2024-05-31 20:01:16.000000 exoplanet_atlas-0.3.5/exoplanet_atlas/tests/test_uncertainties.py
+-rw-r--r--   0 zach       (502) staff       (20)     1411 2024-05-31 20:01:16.000000 exoplanet_atlas-0.3.5/exoplanet_atlas/tests/test_visualizations.py
+-rw-r--r--   0 zach       (502) staff       (20)      722 2024-05-31 20:01:16.000000 exoplanet_atlas-0.3.5/exoplanet_atlas/tests/test_whatsup.py
+-rw-r--r--   0 zach       (502) staff       (20)      197 2024-05-31 20:19:27.000000 exoplanet_atlas-0.3.5/exoplanet_atlas/version.py
+drwxr-xr-x   0 zach       (502) staff       (20)        0 2024-05-31 20:21:31.511017 exoplanet_atlas-0.3.5/exoplanet_atlas/visualizations/
+-rw-r--r--   0 zach       (502) staff       (20)     4138 2024-05-31 20:01:16.000000 exoplanet_atlas-0.3.5/exoplanet_atlas/visualizations/MultiPanel.py
+-rw-r--r--   0 zach       (502) staff       (20)      818 2024-05-31 20:01:16.000000 exoplanet_atlas-0.3.5/exoplanet_atlas/visualizations/ThumbtackMovie.py
+-rw-r--r--   0 zach       (502) staff       (20)    14017 2024-05-20 18:20:59.000000 exoplanet_atlas-0.3.5/exoplanet_atlas/visualizations/ThumbtackPlot.py
+-rw-r--r--   0 zach       (502) staff       (20)       95 2024-05-20 18:20:59.000000 exoplanet_atlas-0.3.5/exoplanet_atlas/visualizations/__init__.py
+drwxr-xr-x   0 zach       (502) staff       (20)        0 2024-05-31 20:21:31.511810 exoplanet_atlas-0.3.5/exoplanet_atlas/visualizations/axes/
+-rw-r--r--   0 zach       (502) staff       (20)       58 2024-05-20 18:20:59.000000 exoplanet_atlas-0.3.5/exoplanet_atlas/visualizations/axes/__init__.py
+-rw-r--r--   0 zach       (502) staff       (20)     4309 2024-05-20 18:20:59.000000 exoplanet_atlas-0.3.5/exoplanet_atlas/visualizations/axes/plottable.py
+-rw-r--r--   0 zach       (502) staff       (20)    13910 2024-05-23 06:36:30.000000 exoplanet_atlas-0.3.5/exoplanet_atlas/visualizations/axes/preset_plottables.py
+-rw-r--r--   0 zach       (502) staff       (20)     8240 2024-05-23 06:36:30.000000 exoplanet_atlas-0.3.5/exoplanet_atlas/visualizations/buildable.py
+-rw-r--r--   0 zach       (502) staff       (20)     2846 2024-05-20 20:56:00.000000 exoplanet_atlas-0.3.5/exoplanet_atlas/visualizations/ink_errorbar.py
+drwxr-xr-x   0 zach       (502) staff       (20)        0 2024-05-31 20:21:31.517186 exoplanet_atlas-0.3.5/exoplanet_atlas/visualizations/panels/
+-rw-r--r--   0 zach       (502) staff       (20)     9710 2024-05-20 20:56:00.000000 exoplanet_atlas-0.3.5/exoplanet_atlas/visualizations/panels/BubblePanel.py
+-rw-r--r--   0 zach       (502) staff       (20)     7716 2024-05-23 06:36:30.000000 exoplanet_atlas-0.3.5/exoplanet_atlas/visualizations/panels/ErrorPanel.py
+-rw-r--r--   0 zach       (502) staff       (20)    12096 2024-05-20 18:20:59.000000 exoplanet_atlas-0.3.5/exoplanet_atlas/visualizations/panels/Panel.py
+-rw-r--r--   0 zach       (502) staff       (20)      103 2024-05-20 18:20:59.000000 exoplanet_atlas-0.3.5/exoplanet_atlas/visualizations/panels/__init__.py
+-rw-r--r--   0 zach       (502) staff       (20)     9782 2024-05-20 18:20:59.000000 exoplanet_atlas-0.3.5/exoplanet_atlas/visualizations/panels/preset_panels.py
+-rw-r--r--   0 zach       (502) staff       (20)      858 2024-05-20 18:20:59.000000 exoplanet_atlas-0.3.5/exoplanet_atlas/visualizations/tweaks.py
+drwxr-xr-x   0 zach       (502) staff       (20)        0 2024-05-31 20:21:31.518845 exoplanet_atlas-0.3.5/exoplanet_atlas/whatsup/
+-rw-r--r--   0 zach       (502) staff       (20)      164 2024-05-20 18:20:59.000000 exoplanet_atlas-0.3.5/exoplanet_atlas/whatsup/__init__.py
+-rw-r--r--   0 zach       (502) staff       (20)     2073 2024-05-20 18:20:59.000000 exoplanet_atlas-0.3.5/exoplanet_atlas/whatsup/block.py
+-rw-r--r--   0 zach       (502) staff       (20)      111 2024-05-20 18:20:59.000000 exoplanet_atlas-0.3.5/exoplanet_atlas/whatsup/night.py
+-rw-r--r--   0 zach       (502) staff       (20)     6515 2024-05-20 18:20:59.000000 exoplanet_atlas-0.3.5/exoplanet_atlas/whatsup/observatory.py
+-rw-r--r--   0 zach       (502) staff       (20)    11246 2024-05-20 20:56:00.000000 exoplanet_atlas-0.3.5/exoplanet_atlas/whatsup/plan.py
+-rw-r--r--   0 zach       (502) staff       (20)     5940 2024-05-20 20:56:00.000000 exoplanet_atlas-0.3.5/exoplanet_atlas/whatsup/transit.py
+drwxr-xr-x   0 zach       (502) staff       (20)        0 2024-05-31 20:21:31.519052 exoplanet_atlas-0.3.5/exoplanet_atlas.egg-info/
+-rw-r--r--   0 zach       (502) staff       (20)     1533 2024-05-31 20:21:31.000000 exoplanet_atlas-0.3.5/exoplanet_atlas.egg-info/PKG-INFO
+-rw-r--r--   0 zach       (502) staff       (20)     2701 2024-05-31 20:21:31.000000 exoplanet_atlas-0.3.5/exoplanet_atlas.egg-info/SOURCES.txt
+-rw-r--r--   0 zach       (502) staff       (20)        1 2024-05-31 20:21:31.000000 exoplanet_atlas-0.3.5/exoplanet_atlas.egg-info/dependency_links.txt
+-rw-r--r--   0 zach       (502) staff       (20)        1 2024-05-20 18:33:32.000000 exoplanet_atlas-0.3.5/exoplanet_atlas.egg-info/not-zip-safe
+-rw-r--r--   0 zach       (502) staff       (20)      300 2024-05-31 20:21:31.000000 exoplanet_atlas-0.3.5/exoplanet_atlas.egg-info/requires.txt
+-rw-r--r--   0 zach       (502) staff       (20)       16 2024-05-31 20:21:31.000000 exoplanet_atlas-0.3.5/exoplanet_atlas.egg-info/top_level.txt
+-rw-r--r--   0 zach       (502) staff       (20)       38 2024-05-31 20:21:31.520335 exoplanet_atlas-0.3.5/setup.cfg
+-rw-r--r--   0 zach       (502) staff       (20)     4035 2024-05-31 20:01:26.000000 exoplanet_atlas-0.3.5/setup.py
```

### Comparing `exoplanet_atlas-0.3.3/LICENSE` & `exoplanet_atlas-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `exoplanet_atlas-0.3.3/PKG-INFO` & `exoplanet_atlas-0.3.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
-Name: exoplanet-atlas
-Version: 0.3.3
+Name: exoplanet_atlas
+Version: 0.3.5
 Summary: Tools for working with transiting exoplanet populations.
-Home-page: https://github.com/zkbt/exoplanet-atlas
+Home-page: https://github.com/zkbt/exoplanet_atlas
 Author: Zach Berta-Thompson
 Author-email: zach.bertathompson@colorado.edu
 License: MIT
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python
 Classifier: Topic :: Scientific/Engineering :: Astronomy
@@ -33,8 +33,8 @@
 Requires-Dist: mkdocstrings-python; extra == "develop"
 Requires-Dist: pytkdocs[numpy-style]; extra == "develop"
 Requires-Dist: mkdocs-jupyter; extra == "develop"
 Requires-Dist: mkdocs-exclude; extra == "develop"
 Requires-Dist: twine; extra == "develop"
 Requires-Dist: pre-commit; extra == "develop"
 
-For detailed usage, please read the documentation at https://zkbt.github.io/exoplanet-atlas/
+For detailed usage, please read the documentation at https://zkbt.github.io/exoplanet_atlas/
```

### Comparing `exoplanet_atlas-0.3.3/README.md` & `exoplanet_atlas-0.3.5/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,36 +1,36 @@
-# exoplanet-atlas
-Tools for compiling and plotting populations of transiting exoplanets. This package still a bit of a work in progress, but can be generally useful for downloading and working with exoplanet populations. For draft documentation explaing how to use `exoatlas`, please [read the documentation](https://zkbt.github.io/exoplanet-atlas/build/html/index.html).
+# exoplanet_atlas
+Tools for compiling and plotting populations of transiting exoplanets. This package still a bit of a work in progress, but can be generally useful for downloading and working with exoplanet populations. For draft documentation explaing how to use `exoplanet_atlas`, please [read the documentation](https://zkbt.github.io/exoplanet_atlas/build/html/index.html).
 
 ### Installation
 If you want the most recent stable version, the simplest way is to install it from PyPI directly via `pip` from any UNIX prompt:
 ```bash
-pip install exoplanet-atlas
+pip install exoplanet_atlas
 ```
 
 Or, if you want the very-most-up-to-date version, you can install directly from this repository via:
 ```bash
-pip install git+https://github.com/zkbt/exoplanet-atlas
+pip install git+https://github.com/zkbt/exoplanet_atlas
 ```
 
 Or, if you want to be able to modify the code yourself, please also feel free to fork/clone this repository onto your own computer and install directly from that editable package. For example, this might look like:
 ```bash
-git clone https://github.com/zkbt/exoplanet-atlas.git
-cd exoplanet-atlas
+git clone https://github.com/zkbt/exoplanet_atlas.git
+cd exoplanet_atlas
 pip install -e .
 ```
-The `pip install -e .` command will link the installed version of the package to the directory of your local repository. Changes you make to the code in that directory should be reflected in the version Python sees when it tries to `import exoatlas`.
+The `pip install -e .` command will link the installed version of the package to the directory of your local repository. Changes you make to the code in that directory should be reflected in the version Python sees when it tries to `import exoplanet_atlas`.
 
 ### Usage
 Here's a quick preview:
 
 
 ```python
 # import some population definitions and plotting tool
-from exoatlas import *
+from exoplanet_atlas import *
 
 # create a dictionary of populations
 exo = TransitingExoplanets()
 solar = SolarSystem()
 pops = {'solar':solar,
         'exo':exo}
```

### Comparing `exoplanet_atlas-0.3.3/exoatlas/imports.py` & `exoplanet_atlas-0.3.5/exoplanet_atlas/imports.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,19 @@
-# imports that are need by many exoatlas subsections
-import os, sys, time, shutil, warnings, copy, importlib
+# imports that are need by many exoplanet_atlas subsections
+from ast import Import
+import os, sys, time, shutil, warnings, copy
 from tqdm import tqdm
 
-code_directory = importlib.resources.files(__name__)
+# (possibly different on Mac, Linux, Windows, even for Python versions 3.8-3.12)
+try:
+    from importlib.resources import files
+except (ModuleNotFoundError, AttributeError, ImportError):
+    from importlib_resources import files
+
+code_directory = files("exoplanet_atlas")
 
 
 import numpy as np, matplotlib.pyplot as plt, matplotlib.animation as animation
 from matplotlib.ticker import ScalarFormatter, FormatStrFormatter, LogLocator
 
 
 from astropy.utils.exceptions import AstropyDeprecationWarning
@@ -63,36 +70,36 @@
         h = co.cnames[name].lower()
     return co.hex2color(h)
 
 
 # create a directory structure ()
 try:
     # search for an environment variable
-    base = os.getenv("EXOATLAS_DATA")
+    base = os.getenv("exoplanet_atlas_DATA")
     assert base is not None
 except AssertionError:
     # otherwise put it in the local directory
     cwd = os.getcwd()
-    base = os.path.join(cwd, "exoatlas-downloads")
+    base = os.path.join(cwd, "exoplanet_atlas-downloads")
 mkdir(base)
 
 
 def locate_local_data():
-    print("💾 `exoatlas` archive data will be stored in:")
+    print("💾 `exoplanet_atlas` archive data will be stored in:")
     print(base)
 
 
 directories = dict(data=os.path.join(base, "data/"))
 for k in directories.keys():
     mkdir(directories[k])
 
 
 def reset_local_data():
     if "y" in input(
-        "Are you sure you want to wipe all " "local exoplanet-atlas data files? [y/N]"
+        "Are you sure you want to wipe all " "local exoplanet_atlas data files? [y/N]"
     ):
         shutil.rmtree(directories["data"])
         mkdir(directories["data"])
         print(f"Removed all local data from {directories['data']}")
 
 
 # some kludge for dealing with Python 3 vs 2?
```

### Comparing `exoplanet_atlas-0.3.3/exoatlas/models/chen.py` & `exoplanet_atlas-0.3.5/exoplanet_atlas/models/chen.py`

 * *Files identical despite different names*

### Comparing `exoplanet_atlas-0.3.3/exoatlas/models/kopparapu.py` & `exoplanet_atlas-0.3.5/exoplanet_atlas/models/kopparapu.py`

 * *Files identical despite different names*

### Comparing `exoplanet_atlas-0.3.3/exoatlas/models/seager.py` & `exoplanet_atlas-0.3.5/exoplanet_atlas/models/seager.py`

 * *Files identical despite different names*

### Comparing `exoplanet_atlas-0.3.3/exoatlas/models/zeng.py` & `exoplanet_atlas-0.3.5/exoplanet_atlas/models/zeng.py`

 * *Files identical despite different names*

### Comparing `exoplanet_atlas-0.3.3/exoatlas/populations/Exoplanets.py` & `exoplanet_atlas-0.3.5/exoplanet_atlas/populations/Exoplanets.py`

 * *Files identical despite different names*

### Comparing `exoplanet_atlas-0.3.3/exoatlas/populations/Population.py` & `exoplanet_atlas-0.3.5/exoplanet_atlas/populations/Population.py`

 * *Files 0% similar despite different names*

```diff
@@ -1605,15 +1605,15 @@
 
         # a trimmed table
         return self._trimmed
 
     def load_standard(self, skip_update=False):
         """
         Load a standardized population table. Generally this
-        will be from a file like ~/.exoatlas/standardized-*.txt
+        will be from a file like ~/.exoplanet_atlas/standardized-*.txt
 
         Returns
         -------
 
         standard : astropy.table.Table
             A table of planet properties,
             with a minimal set of columns.
@@ -1636,13 +1636,13 @@
         # masked = np.ma.filled(standard, fill_value = np.nan)
 
         return standard
 
     def save_standard(self, standard):
         """
         Save the standardized table out to a text file
-        like ~/exoatlas/standardized-*.txt
+        like ~/exoplanet_atlas/standardized-*.txt
         """
 
         # save it as an ascii table for humans to read
         standard.write(self.standard_path, format="ascii.ecsv", overwrite=True)
         self.speak(f"Saved a standardized text table to {self.standard_path}")
```

### Comparing `exoplanet_atlas-0.3.3/exoatlas/populations/SolarSystem.py` & `exoplanet_atlas-0.3.5/exoplanet_atlas/populations/SolarSystem.py`

 * *Files identical despite different names*

### Comparing `exoplanet_atlas-0.3.3/exoatlas/populations/TOI.py` & `exoplanet_atlas-0.3.5/exoplanet_atlas/populations/TOI.py`

 * *Files identical despite different names*

### Comparing `exoplanet_atlas-0.3.3/exoatlas/populations/TOISubsets.py` & `exoplanet_atlas-0.3.5/exoplanet_atlas/populations/TOISubsets.py`

 * *Files identical despite different names*

### Comparing `exoplanet_atlas-0.3.3/exoatlas/populations/TransitingExoplanets.py` & `exoplanet_atlas-0.3.5/exoplanet_atlas/populations/TransitingExoplanets.py`

 * *Files identical despite different names*

### Comparing `exoplanet_atlas-0.3.3/exoatlas/populations/TransitingExoplanetsSubsets.py` & `exoplanet_atlas-0.3.5/exoplanet_atlas/populations/TransitingExoplanetsSubsets.py`

 * *Files identical despite different names*

### Comparing `exoplanet_atlas-0.3.3/exoatlas/populations/collections.py` & `exoplanet_atlas-0.3.5/exoplanet_atlas/populations/collections.py`

 * *Files identical despite different names*

### Comparing `exoplanet_atlas-0.3.3/exoatlas/populations/column_descriptions.py` & `exoplanet_atlas-0.3.5/exoplanet_atlas/populations/column_descriptions.py`

 * *Files identical despite different names*

### Comparing `exoplanet_atlas-0.3.3/exoatlas/populations/curation/Confirmed.py` & `exoplanet_atlas-0.3.5/exoplanet_atlas/populations/curation/Confirmed.py`

 * *Files identical despite different names*

### Comparing `exoplanet_atlas-0.3.3/exoatlas/populations/downloaders.py` & `exoplanet_atlas-0.3.5/exoplanet_atlas/populations/downloaders.py`

 * *Files 1% similar despite different names*

```diff
@@ -225,15 +225,15 @@
 
 
 toi_exofop = ExoFOPDownloader()
 
 
 class MergedTOIDownloader(ExoFOPDownloader):
     """
-    Download the TOIs from the exoatlas table, but also search the MAST
+    Download the TOIs from the exoplanet_atlas table, but also search the MAST
     archive to pull out extra parameters for each star from the TIC.
     """
 
     @property
     def path(self):
         """
         Where should the local copy of this file be stored?
@@ -252,15 +252,15 @@
         self.speak("Downloading TOIs from ExoFOP.")
         t = toi_exofop.get(remake=True)
 
         # download the TIC entries for these stars
         self.speak(f"Searching for {len(t)} stars in the TIC on the MAST.")
 
         # import Catalogs only when we need it
-        # (otherwise, we'll need the internet to ever run exoatlas)
+        # (otherwise, we'll need the internet to ever run exoplanet_atlas)
         from astroquery.mast import Catalogs
 
         tic_table = Catalogs.query_criteria(catalog="Tic", ID=np.unique(t["TIC ID"]))
 
         # preface all the columns with TIC so we can keep them straight
         for k in tic_table.colnames:
             tic_table[k].name = f"TIC {k}"
```

### Comparing `exoplanet_atlas-0.3.3/exoatlas/populations/summary.py` & `exoplanet_atlas-0.3.5/exoplanet_atlas/populations/summary.py`

 * *Files identical despite different names*

### Comparing `exoplanet_atlas-0.3.3/exoatlas/talker.py` & `exoplanet_atlas-0.3.5/exoplanet_atlas/talker.py`

 * *Files identical despite different names*

### Comparing `exoplanet_atlas-0.3.3/exoatlas/telescopes/buckets.py` & `exoplanet_atlas-0.3.5/exoplanet_atlas/telescopes/buckets.py`

 * *Files identical despite different names*

### Comparing `exoplanet_atlas-0.3.3/exoatlas/tests/test_buckets.py` & `exoplanet_atlas-0.3.5/exoplanet_atlas/tests/test_buckets.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from .setup_tests import *
-from exoatlas.imports import *
-from exoatlas import *
+from exoplanet_atlas.imports import *
+from exoplanet_atlas import *
 
 
 def test_telescope_units():
     for t in ["Kepler", "TESS", "JWST", "HST"]:
         define_telescope_unit_by_name(t)
         define_telescope_unit_by_name(t, wavelength=0.7 * u.micron)
```

### Comparing `exoplanet_atlas-0.3.3/exoatlas/tests/test_downloaders.py` & `exoplanet_atlas-0.3.5/exoplanet_atlas/tests/test_downloaders.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from .setup_tests import *
 
-from exoatlas.imports import *
-from exoatlas.populations.downloaders import *
+from exoplanet_atlas.imports import *
+from exoplanet_atlas.populations.downloaders import *
 
 
 def test_exoplanets():
     with mock.patch("builtins.input", return_value=""):
         exoplanets_downloader.get()
```

### Comparing `exoplanet_atlas-0.3.3/exoatlas/tests/test_models.py` & `exoplanet_atlas-0.3.5/exoplanet_atlas/tests/test_models.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from .setup_tests import *
 
-from exoatlas.models import *
-from exoatlas.imports import *
+from exoplanet_atlas.models import *
+from exoplanet_atlas.imports import *
 
 
 def test_seager():
     """
     Test the Seager mass-radius relations.
     """
     plt.cla()
```

### Comparing `exoplanet_atlas-0.3.3/exoatlas/tests/test_populations.py` & `exoplanet_atlas-0.3.5/exoplanet_atlas/tests/test_populations.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from .setup_tests import *
 
-from exoatlas.imports import *
-from exoatlas.populations import *
+from exoplanet_atlas.imports import *
+from exoplanet_atlas.populations import *
 
 
 def test_population():
     """
     Can we make a population from scratch from a table?
     """
```

### Comparing `exoplanet_atlas-0.3.3/exoatlas/tests/test_snr.py` & `exoplanet_atlas-0.3.5/exoplanet_atlas/tests/test_snr.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from .setup_tests import *
 
-from exoatlas import *
+from exoplanet_atlas import *
 
 
 def test_reflection(telescope_name="JWST", wavelength=1 * u.micron):
     with mock.patch("builtins.input", return_value=""):
         t = TransitingExoplanets()
 
     w = 1 * u.micron
```

### Comparing `exoplanet_atlas-0.3.3/exoatlas/tests/test_uncertainties.py` & `exoplanet_atlas-0.3.5/exoplanet_atlas/tests/test_uncertainties.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from .setup_tests import *
 
-from exoatlas.imports import *
-from exoatlas.populations import *
+from exoplanet_atlas.imports import *
+from exoplanet_atlas.populations import *
 
 
 def test_uncertainties():
     """
     Can we pull out c
     """
```

### Comparing `exoplanet_atlas-0.3.3/exoatlas/tests/test_visualizations.py` & `exoplanet_atlas-0.3.5/exoplanet_atlas/tests/test_visualizations.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from .setup_tests import *
 
-from exoatlas.imports import *
+from exoplanet_atlas.imports import *
 
-import exoatlas as ex
+import exoplanet_atlas as ex
 import matplotlib.pyplot as plt
-from exoatlas.visualizations.panels.preset_panels import predefined_panels
+from exoplanet_atlas.visualizations.panels.preset_panels import predefined_panels
 
 
 def test_panels():
     pops = {}
     pops["solarsystem"] = ex.SolarSystem()
     for p in predefined_panels:
         print(p)
```

### Comparing `exoplanet_atlas-0.3.3/exoatlas/tests/test_whatsup.py` & `exoplanet_atlas-0.3.5/exoplanet_atlas/tests/test_whatsup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from .setup_tests import *
 
-from exoatlas.imports import *
-from exoatlas.populations import TransitingExoplanets
-from exoatlas.whatsup import Plan
+from exoplanet_atlas.imports import *
+from exoplanet_atlas.populations import TransitingExoplanets
+from exoplanet_atlas.whatsup import Plan
 
 
 def test_whatsup():
     with mock.patch("builtins.input", return_value=""):
         planets = TransitingExoplanets()
 
     p = Plan(
```

### Comparing `exoplanet_atlas-0.3.3/exoatlas/visualizations/MultiPanel.py` & `exoplanet_atlas-0.3.5/exoplanet_atlas/visualizations/MultiPanel.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
         return x
     else:
         return x(**kw)
 
 
 class MultiPanelPlot(Talker):
     """
-    Make and modify row or a column of connected exoatlas plot panels.
+    Make and modify row or a column of connected exoplanet_atlas plot panels.
     """
 
     def __init__(
         self,
         panels=[MassRadius, FluxRadius, StellarRadiusPlanetRadius, DistanceRadius],
         horizontal=True,
         figsize=(8, 6),
```

### Comparing `exoplanet_atlas-0.3.3/exoatlas/visualizations/ThumbtackMovie.py` & `exoplanet_atlas-0.3.5/exoplanet_atlas/visualizations/ThumbtackMovie.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-from exoatlas.ThumbtackPlot import ThumbtackPlot
-from exoatlas.TransitingExoplanets import GoodMass, BadMass, Kepler, NonKepler
-from exoatlas.KOI import UnconfirmedKepler
-from exoatlas.TESS import TESS
+from exoplanet_atlas.ThumbtackPlot import ThumbtackPlot
+from exoplanet_atlas.TransitingExoplanets import GoodMass, BadMass, Kepler, NonKepler
+from exoplanet_atlas.KOI import UnconfirmedKepler
+from exoplanet_atlas.TESS import TESS
 
 pops = dict(
     kepler=Kepler(), candidates=UnconfirmedKepler(), nonkepler=NonKepler(), new=TESS()
 )
 
 
 t = ThumbtackPlot(pops=pops, lightyears=False)
```

### Comparing `exoplanet_atlas-0.3.3/exoatlas/visualizations/ThumbtackPlot.py` & `exoplanet_atlas-0.3.5/exoplanet_atlas/visualizations/ThumbtackPlot.py`

 * *Files identical despite different names*

### Comparing `exoplanet_atlas-0.3.3/exoatlas/visualizations/axes/plottable.py` & `exoplanet_atlas-0.3.5/exoplanet_atlas/visualizations/axes/plottable.py`

 * *Files identical despite different names*

### Comparing `exoplanet_atlas-0.3.3/exoatlas/visualizations/axes/preset_plottables.py` & `exoplanet_atlas-0.3.5/exoplanet_atlas/visualizations/axes/preset_plottables.py`

 * *Files identical despite different names*

### Comparing `exoplanet_atlas-0.3.3/exoatlas/visualizations/buildable.py` & `exoplanet_atlas-0.3.5/exoplanet_atlas/visualizations/buildable.py`

 * *Files identical despite different names*

### Comparing `exoplanet_atlas-0.3.3/exoatlas/visualizations/ink_errorbar.py` & `exoplanet_atlas-0.3.5/exoplanet_atlas/visualizations/ink_errorbar.py`

 * *Files identical despite different names*

### Comparing `exoplanet_atlas-0.3.3/exoatlas/visualizations/panels/BubblePanel.py` & `exoplanet_atlas-0.3.5/exoplanet_atlas/visualizations/panels/BubblePanel.py`

 * *Files identical despite different names*

### Comparing `exoplanet_atlas-0.3.3/exoatlas/visualizations/panels/ErrorPanel.py` & `exoplanet_atlas-0.3.5/exoplanet_atlas/visualizations/panels/ErrorPanel.py`

 * *Files identical despite different names*

### Comparing `exoplanet_atlas-0.3.3/exoatlas/visualizations/panels/Panel.py` & `exoplanet_atlas-0.3.5/exoplanet_atlas/visualizations/panels/Panel.py`

 * *Files identical despite different names*

### Comparing `exoplanet_atlas-0.3.3/exoatlas/visualizations/panels/preset_panels.py` & `exoplanet_atlas-0.3.5/exoplanet_atlas/visualizations/panels/preset_panels.py`

 * *Files identical despite different names*

### Comparing `exoplanet_atlas-0.3.3/exoatlas/visualizations/tweaks.py` & `exoplanet_atlas-0.3.5/exoplanet_atlas/visualizations/tweaks.py`

 * *Files identical despite different names*

### Comparing `exoplanet_atlas-0.3.3/exoatlas/whatsup/block.py` & `exoplanet_atlas-0.3.5/exoplanet_atlas/whatsup/block.py`

 * *Files identical despite different names*

### Comparing `exoplanet_atlas-0.3.3/exoatlas/whatsup/observatory.py` & `exoplanet_atlas-0.3.5/exoplanet_atlas/whatsup/observatory.py`

 * *Files identical despite different names*

### Comparing `exoplanet_atlas-0.3.3/exoatlas/whatsup/plan.py` & `exoplanet_atlas-0.3.5/exoplanet_atlas/whatsup/plan.py`

 * *Files identical despite different names*

### Comparing `exoplanet_atlas-0.3.3/exoatlas/whatsup/transit.py` & `exoplanet_atlas-0.3.5/exoplanet_atlas/whatsup/transit.py`

 * *Files identical despite different names*

### Comparing `exoplanet_atlas-0.3.3/exoplanet_atlas.egg-info/PKG-INFO` & `exoplanet_atlas-0.3.5/exoplanet_atlas.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
-Name: exoplanet-atlas
-Version: 0.3.3
+Name: exoplanet_atlas
+Version: 0.3.5
 Summary: Tools for working with transiting exoplanet populations.
-Home-page: https://github.com/zkbt/exoplanet-atlas
+Home-page: https://github.com/zkbt/exoplanet_atlas
 Author: Zach Berta-Thompson
 Author-email: zach.bertathompson@colorado.edu
 License: MIT
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python
 Classifier: Topic :: Scientific/Engineering :: Astronomy
@@ -33,8 +33,8 @@
 Requires-Dist: mkdocstrings-python; extra == "develop"
 Requires-Dist: pytkdocs[numpy-style]; extra == "develop"
 Requires-Dist: mkdocs-jupyter; extra == "develop"
 Requires-Dist: mkdocs-exclude; extra == "develop"
 Requires-Dist: twine; extra == "develop"
 Requires-Dist: pre-commit; extra == "develop"
 
-For detailed usage, please read the documentation at https://zkbt.github.io/exoplanet-atlas/
+For detailed usage, please read the documentation at https://zkbt.github.io/exoplanet_atlas/
```

### Comparing `exoplanet_atlas-0.3.3/exoplanet_atlas.egg-info/SOURCES.txt` & `exoplanet_atlas-0.3.5/exoplanet_atlas.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,68 +1,68 @@
 LICENSE
 README.md
 setup.py
-exoatlas/__init__.py
-exoatlas/imports.py
-exoatlas/talker.py
-exoatlas/version.py
-exoatlas/models/__init__.py
-exoatlas/models/chen.py
-exoatlas/models/kopparapu.py
-exoatlas/models/seager.py
-exoatlas/models/zeng.py
-exoatlas/populations/Exoplanets.py
-exoatlas/populations/Population.py
-exoatlas/populations/SolarSystem.py
-exoatlas/populations/TESS.py
-exoatlas/populations/TOI.py
-exoatlas/populations/TOISubsets.py
-exoatlas/populations/TransitingExoplanets.py
-exoatlas/populations/TransitingExoplanetsSubsets.py
-exoatlas/populations/__init__.py
-exoatlas/populations/collections.py
-exoatlas/populations/column_descriptions.py
-exoatlas/populations/downloaders.py
-exoatlas/populations/summary.py
-exoatlas/populations/curation/Confirmed.py
-exoatlas/populations/curation/TransitingExoplanets.py
-exoatlas/populations/curation/__init__.py
-exoatlas/telescopes/__init__.py
-exoatlas/telescopes/buckets.py
-exoatlas/tests/__init__.py
-exoatlas/tests/setup_tests.py
-exoatlas/tests/test_buckets.py
-exoatlas/tests/test_downloaders.py
-exoatlas/tests/test_imports.py
-exoatlas/tests/test_models.py
-exoatlas/tests/test_populations.py
-exoatlas/tests/test_snr.py
-exoatlas/tests/test_uncertainties.py
-exoatlas/tests/test_visualizations.py
-exoatlas/tests/test_whatsup.py
-exoatlas/visualizations/MultiPanel.py
-exoatlas/visualizations/ThumbtackMovie.py
-exoatlas/visualizations/ThumbtackPlot.py
-exoatlas/visualizations/__init__.py
-exoatlas/visualizations/buildable.py
-exoatlas/visualizations/ink_errorbar.py
-exoatlas/visualizations/tweaks.py
-exoatlas/visualizations/axes/__init__.py
-exoatlas/visualizations/axes/plottable.py
-exoatlas/visualizations/axes/preset_plottables.py
-exoatlas/visualizations/panels/BubblePanel.py
-exoatlas/visualizations/panels/ErrorPanel.py
-exoatlas/visualizations/panels/Panel.py
-exoatlas/visualizations/panels/__init__.py
-exoatlas/visualizations/panels/preset_panels.py
-exoatlas/whatsup/__init__.py
-exoatlas/whatsup/block.py
-exoatlas/whatsup/night.py
-exoatlas/whatsup/observatory.py
-exoatlas/whatsup/plan.py
-exoatlas/whatsup/transit.py
+exoplanet_atlas/__init__.py
+exoplanet_atlas/imports.py
+exoplanet_atlas/talker.py
+exoplanet_atlas/version.py
 exoplanet_atlas.egg-info/PKG-INFO
 exoplanet_atlas.egg-info/SOURCES.txt
 exoplanet_atlas.egg-info/dependency_links.txt
 exoplanet_atlas.egg-info/not-zip-safe
 exoplanet_atlas.egg-info/requires.txt
-exoplanet_atlas.egg-info/top_level.txt
+exoplanet_atlas.egg-info/top_level.txt
+exoplanet_atlas/models/__init__.py
+exoplanet_atlas/models/chen.py
+exoplanet_atlas/models/kopparapu.py
+exoplanet_atlas/models/seager.py
+exoplanet_atlas/models/zeng.py
+exoplanet_atlas/populations/Exoplanets.py
+exoplanet_atlas/populations/Population.py
+exoplanet_atlas/populations/SolarSystem.py
+exoplanet_atlas/populations/TESS.py
+exoplanet_atlas/populations/TOI.py
+exoplanet_atlas/populations/TOISubsets.py
+exoplanet_atlas/populations/TransitingExoplanets.py
+exoplanet_atlas/populations/TransitingExoplanetsSubsets.py
+exoplanet_atlas/populations/__init__.py
+exoplanet_atlas/populations/collections.py
+exoplanet_atlas/populations/column_descriptions.py
+exoplanet_atlas/populations/downloaders.py
+exoplanet_atlas/populations/summary.py
+exoplanet_atlas/populations/curation/Confirmed.py
+exoplanet_atlas/populations/curation/TransitingExoplanets.py
+exoplanet_atlas/populations/curation/__init__.py
+exoplanet_atlas/telescopes/__init__.py
+exoplanet_atlas/telescopes/buckets.py
+exoplanet_atlas/tests/__init__.py
+exoplanet_atlas/tests/setup_tests.py
+exoplanet_atlas/tests/test_buckets.py
+exoplanet_atlas/tests/test_downloaders.py
+exoplanet_atlas/tests/test_imports.py
+exoplanet_atlas/tests/test_models.py
+exoplanet_atlas/tests/test_populations.py
+exoplanet_atlas/tests/test_snr.py
+exoplanet_atlas/tests/test_uncertainties.py
+exoplanet_atlas/tests/test_visualizations.py
+exoplanet_atlas/tests/test_whatsup.py
+exoplanet_atlas/visualizations/MultiPanel.py
+exoplanet_atlas/visualizations/ThumbtackMovie.py
+exoplanet_atlas/visualizations/ThumbtackPlot.py
+exoplanet_atlas/visualizations/__init__.py
+exoplanet_atlas/visualizations/buildable.py
+exoplanet_atlas/visualizations/ink_errorbar.py
+exoplanet_atlas/visualizations/tweaks.py
+exoplanet_atlas/visualizations/axes/__init__.py
+exoplanet_atlas/visualizations/axes/plottable.py
+exoplanet_atlas/visualizations/axes/preset_plottables.py
+exoplanet_atlas/visualizations/panels/BubblePanel.py
+exoplanet_atlas/visualizations/panels/ErrorPanel.py
+exoplanet_atlas/visualizations/panels/Panel.py
+exoplanet_atlas/visualizations/panels/__init__.py
+exoplanet_atlas/visualizations/panels/preset_panels.py
+exoplanet_atlas/whatsup/__init__.py
+exoplanet_atlas/whatsup/block.py
+exoplanet_atlas/whatsup/night.py
+exoplanet_atlas/whatsup/observatory.py
+exoplanet_atlas/whatsup/plan.py
+exoplanet_atlas/whatsup/transit.py
```

### Comparing `exoplanet_atlas-0.3.3/setup.py` & `exoplanet_atlas-0.3.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,32 +41,32 @@
     # uncomment the next line to test out on test.pypi.com/project/tess-zap
     # os.system("twine upload --repository-url https://test.pypi.org/legacy/ dist/*")
     os.system("twine upload dist/*")
     os.system("rm -rf dist/rainbow-connection*")
     sys.exit()
 
 # a little kludge to get the version number from __version__
-exec(open("exoatlas/version.py").read())
+exec(open("exoplanet_atlas/version.py").read())
 
 # run the setup function
 setup(
     # the name folks can use to search for this with pip
-    name="exoplanet-atlas",
+    name="exoplanet_atlas",
     # this package will only be installed if the current version doesn't exist
     version=__version__,
     # what's a short description of the package?
     description="Tools for working with transiting exoplanet populations.",
     # what's a more detailed description?
-    long_description="For detailed usage, please read the documentation at https://zkbt.github.io/exoplanet-atlas/",
+    long_description="For detailed usage, please read the documentation at https://zkbt.github.io/exoplanet_atlas/",
     # who's the main author?
     author="Zach Berta-Thompson",
     # what's the main author's email?
     author_email="zach.bertathompson@colorado.edu",
     # what's the URL for the repository?
-    url="https://github.com/zkbt/exoplanet-atlas",
+    url="https://github.com/zkbt/exoplanet_atlas",
     # this figures out what subdirectories to include
     packages=find_packages(),
     # are there directories of data that should be accessible when installed?
     include_package_data=True,
     # where are those data directories?
     package_data={},
     # any scripts will be copied into your $PATH, to run from the command line
```

