# Comparing `tmp/exoplanet_atlas-0.3.5.tar.gz` & `tmp/exoplanet_atlas-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "exoplanet_atlas-0.3.5.tar", last modified: Fri May 31 20:21:31 2024, max compression
+gzip compressed data, was "exoplanet_atlas-0.3.6.tar", last modified: Fri May 31 20:40:23 2024, max compression
```

## Comparing `exoplanet_atlas-0.3.5.tar` & `exoplanet_atlas-0.3.6.tar`

### file list

```diff
@@ -1,82 +1,82 @@
-drwxr-xr-x   0 zach       (502) staff       (20)        0 2024-05-31 20:21:31.520286 exoplanet_atlas-0.3.5/
--rw-r--r--   0 zach       (502) staff       (20)     1091 2024-05-20 20:56:00.000000 exoplanet_atlas-0.3.5/LICENSE
--rw-r--r--   0 zach       (502) staff       (20)     1533 2024-05-31 20:21:31.520050 exoplanet_atlas-0.3.5/PKG-INFO
--rw-r--r--   0 zach       (502) staff       (20)     1942 2024-05-31 20:01:26.000000 exoplanet_atlas-0.3.5/README.md
-drwxr-xr-x   0 zach       (502) staff       (20)        0 2024-05-31 20:21:31.497843 exoplanet_atlas-0.3.5/exoplanet_atlas/
--rw-r--r--   0 zach       (502) staff       (20)      179 2024-05-20 20:56:00.000000 exoplanet_atlas-0.3.5/exoplanet_atlas/__init__.py
--rw-r--r--   0 zach       (502) staff       (20)     4742 2024-05-31 20:09:38.000000 exoplanet_atlas-0.3.5/exoplanet_atlas/imports.py
-drwxr-xr-x   0 zach       (502) staff       (20)        0 2024-05-31 20:21:31.501981 exoplanet_atlas-0.3.5/exoplanet_atlas/models/
--rw-r--r--   0 zach       (502) staff       (20)       87 2024-05-20 18:20:59.000000 exoplanet_atlas-0.3.5/exoplanet_atlas/models/__init__.py
--rw-r--r--   0 zach       (502) staff       (20)     2084 2024-05-20 18:20:59.000000 exoplanet_atlas-0.3.5/exoplanet_atlas/models/chen.py
--rw-r--r--   0 zach       (502) staff       (20)     1541 2024-05-20 20:56:00.000000 exoplanet_atlas-0.3.5/exoplanet_atlas/models/kopparapu.py
--rw-r--r--   0 zach       (502) staff       (20)     1171 2024-05-20 20:56:00.000000 exoplanet_atlas-0.3.5/exoplanet_atlas/models/seager.py
--rw-r--r--   0 zach       (502) staff       (20)      963 2024-05-20 20:56:00.000000 exoplanet_atlas-0.3.5/exoplanet_atlas/models/zeng.py
-drwxr-xr-x   0 zach       (502) staff       (20)        0 2024-05-31 20:21:31.505835 exoplanet_atlas-0.3.5/exoplanet_atlas/populations/
--rw-r--r--   0 zach       (502) staff       (20)    13402 2024-05-20 20:56:00.000000 exoplanet_atlas-0.3.5/exoplanet_atlas/populations/Exoplanets.py
--rw-r--r--   0 zach       (502) staff       (20)    51427 2024-05-31 20:01:16.000000 exoplanet_atlas-0.3.5/exoplanet_atlas/populations/Population.py
--rw-r--r--   0 zach       (502) staff       (20)     3598 2024-05-23 06:36:30.000000 exoplanet_atlas-0.3.5/exoplanet_atlas/populations/SolarSystem.py
--rw-r--r--   0 zach       (502) staff       (20)       62 2024-05-20 18:20:59.000000 exoplanet_atlas-0.3.5/exoplanet_atlas/populations/TESS.py
--rw-r--r--   0 zach       (502) staff       (20)     7538 2024-05-20 20:56:00.000000 exoplanet_atlas-0.3.5/exoplanet_atlas/populations/TOI.py
--rw-r--r--   0 zach       (502) staff       (20)     3485 2024-05-20 18:20:59.000000 exoplanet_atlas-0.3.5/exoplanet_atlas/populations/TOISubsets.py
--rw-r--r--   0 zach       (502) staff       (20)     3351 2024-05-20 18:20:59.000000 exoplanet_atlas-0.3.5/exoplanet_atlas/populations/TransitingExoplanets.py
--rw-r--r--   0 zach       (502) staff       (20)     5718 2024-05-20 20:56:00.000000 exoplanet_atlas-0.3.5/exoplanet_atlas/populations/TransitingExoplanetsSubsets.py
--rw-r--r--   0 zach       (502) staff       (20)      416 2024-05-20 18:20:59.000000 exoplanet_atlas-0.3.5/exoplanet_atlas/populations/__init__.py
--rw-r--r--   0 zach       (502) staff       (20)      716 2024-05-20 18:20:59.000000 exoplanet_atlas-0.3.5/exoplanet_atlas/populations/collections.py
--rw-r--r--   0 zach       (502) staff       (20)     2258 2024-05-20 20:56:00.000000 exoplanet_atlas-0.3.5/exoplanet_atlas/populations/column_descriptions.py
-drwxr-xr-x   0 zach       (502) staff       (20)        0 2024-05-31 20:21:31.506271 exoplanet_atlas-0.3.5/exoplanet_atlas/populations/curation/
--rw-r--r--   0 zach       (502) staff       (20)     7747 2024-05-20 20:56:00.000000 exoplanet_atlas-0.3.5/exoplanet_atlas/populations/curation/Confirmed.py
--rw-r--r--   0 zach       (502) staff       (20)       26 2024-05-20 18:20:59.000000 exoplanet_atlas-0.3.5/exoplanet_atlas/populations/curation/TransitingExoplanets.py
--rw-r--r--   0 zach       (502) staff       (20)        0 2024-05-20 18:20:59.000000 exoplanet_atlas-0.3.5/exoplanet_atlas/populations/curation/__init__.py
--rw-r--r--   0 zach       (502) staff       (20)     9005 2024-05-31 20:01:16.000000 exoplanet_atlas-0.3.5/exoplanet_atlas/populations/downloaders.py
--rw-r--r--   0 zach       (502) staff       (20)     1963 2024-05-20 20:56:00.000000 exoplanet_atlas-0.3.5/exoplanet_atlas/populations/summary.py
--rw-r--r--   0 zach       (502) staff       (20)     2735 2024-05-20 20:56:00.000000 exoplanet_atlas-0.3.5/exoplanet_atlas/talker.py
-drwxr-xr-x   0 zach       (502) staff       (20)        0 2024-05-31 20:21:31.506642 exoplanet_atlas-0.3.5/exoplanet_atlas/telescopes/
--rw-r--r--   0 zach       (502) staff       (20)       23 2024-05-20 18:20:59.000000 exoplanet_atlas-0.3.5/exoplanet_atlas/telescopes/__init__.py
--rw-r--r--   0 zach       (502) staff       (20)     6048 2024-05-23 06:36:30.000000 exoplanet_atlas-0.3.5/exoplanet_atlas/telescopes/buckets.py
-drwxr-xr-x   0 zach       (502) staff       (20)        0 2024-05-31 20:21:31.509121 exoplanet_atlas-0.3.5/exoplanet_atlas/tests/
--rw-r--r--   0 zach       (502) staff       (20)      268 2024-05-20 18:20:59.000000 exoplanet_atlas-0.3.5/exoplanet_atlas/tests/__init__.py
--rw-r--r--   0 zach       (502) staff       (20)       40 2024-05-20 20:56:00.000000 exoplanet_atlas-0.3.5/exoplanet_atlas/tests/setup_tests.py
--rw-r--r--   0 zach       (502) staff       (20)     1084 2024-05-31 20:01:16.000000 exoplanet_atlas-0.3.5/exoplanet_atlas/tests/test_buckets.py
--rw-r--r--   0 zach       (502) staff       (20)      592 2024-05-31 20:01:16.000000 exoplanet_atlas-0.3.5/exoplanet_atlas/tests/test_downloaders.py
--rw-r--r--   0 zach       (502) staff       (20)      370 2024-05-31 20:01:16.000000 exoplanet_atlas-0.3.5/exoplanet_atlas/tests/test_imports.py
--rw-r--r--   0 zach       (502) staff       (20)      689 2024-05-31 20:01:16.000000 exoplanet_atlas-0.3.5/exoplanet_atlas/tests/test_models.py
--rw-r--r--   0 zach       (502) staff       (20)     3298 2024-05-31 20:01:16.000000 exoplanet_atlas-0.3.5/exoplanet_atlas/tests/test_populations.py
--rw-r--r--   0 zach       (502) staff       (20)     2496 2024-05-31 20:01:16.000000 exoplanet_atlas-0.3.5/exoplanet_atlas/tests/test_snr.py
--rw-r--r--   0 zach       (502) staff       (20)      626 2024-05-31 20:01:16.000000 exoplanet_atlas-0.3.5/exoplanet_atlas/tests/test_uncertainties.py
--rw-r--r--   0 zach       (502) staff       (20)     1411 2024-05-31 20:01:16.000000 exoplanet_atlas-0.3.5/exoplanet_atlas/tests/test_visualizations.py
--rw-r--r--   0 zach       (502) staff       (20)      722 2024-05-31 20:01:16.000000 exoplanet_atlas-0.3.5/exoplanet_atlas/tests/test_whatsup.py
--rw-r--r--   0 zach       (502) staff       (20)      197 2024-05-31 20:19:27.000000 exoplanet_atlas-0.3.5/exoplanet_atlas/version.py
-drwxr-xr-x   0 zach       (502) staff       (20)        0 2024-05-31 20:21:31.511017 exoplanet_atlas-0.3.5/exoplanet_atlas/visualizations/
--rw-r--r--   0 zach       (502) staff       (20)     4138 2024-05-31 20:01:16.000000 exoplanet_atlas-0.3.5/exoplanet_atlas/visualizations/MultiPanel.py
--rw-r--r--   0 zach       (502) staff       (20)      818 2024-05-31 20:01:16.000000 exoplanet_atlas-0.3.5/exoplanet_atlas/visualizations/ThumbtackMovie.py
--rw-r--r--   0 zach       (502) staff       (20)    14017 2024-05-20 18:20:59.000000 exoplanet_atlas-0.3.5/exoplanet_atlas/visualizations/ThumbtackPlot.py
--rw-r--r--   0 zach       (502) staff       (20)       95 2024-05-20 18:20:59.000000 exoplanet_atlas-0.3.5/exoplanet_atlas/visualizations/__init__.py
-drwxr-xr-x   0 zach       (502) staff       (20)        0 2024-05-31 20:21:31.511810 exoplanet_atlas-0.3.5/exoplanet_atlas/visualizations/axes/
--rw-r--r--   0 zach       (502) staff       (20)       58 2024-05-20 18:20:59.000000 exoplanet_atlas-0.3.5/exoplanet_atlas/visualizations/axes/__init__.py
--rw-r--r--   0 zach       (502) staff       (20)     4309 2024-05-20 18:20:59.000000 exoplanet_atlas-0.3.5/exoplanet_atlas/visualizations/axes/plottable.py
--rw-r--r--   0 zach       (502) staff       (20)    13910 2024-05-23 06:36:30.000000 exoplanet_atlas-0.3.5/exoplanet_atlas/visualizations/axes/preset_plottables.py
--rw-r--r--   0 zach       (502) staff       (20)     8240 2024-05-23 06:36:30.000000 exoplanet_atlas-0.3.5/exoplanet_atlas/visualizations/buildable.py
--rw-r--r--   0 zach       (502) staff       (20)     2846 2024-05-20 20:56:00.000000 exoplanet_atlas-0.3.5/exoplanet_atlas/visualizations/ink_errorbar.py
-drwxr-xr-x   0 zach       (502) staff       (20)        0 2024-05-31 20:21:31.517186 exoplanet_atlas-0.3.5/exoplanet_atlas/visualizations/panels/
--rw-r--r--   0 zach       (502) staff       (20)     9710 2024-05-20 20:56:00.000000 exoplanet_atlas-0.3.5/exoplanet_atlas/visualizations/panels/BubblePanel.py
--rw-r--r--   0 zach       (502) staff       (20)     7716 2024-05-23 06:36:30.000000 exoplanet_atlas-0.3.5/exoplanet_atlas/visualizations/panels/ErrorPanel.py
--rw-r--r--   0 zach       (502) staff       (20)    12096 2024-05-20 18:20:59.000000 exoplanet_atlas-0.3.5/exoplanet_atlas/visualizations/panels/Panel.py
--rw-r--r--   0 zach       (502) staff       (20)      103 2024-05-20 18:20:59.000000 exoplanet_atlas-0.3.5/exoplanet_atlas/visualizations/panels/__init__.py
--rw-r--r--   0 zach       (502) staff       (20)     9782 2024-05-20 18:20:59.000000 exoplanet_atlas-0.3.5/exoplanet_atlas/visualizations/panels/preset_panels.py
--rw-r--r--   0 zach       (502) staff       (20)      858 2024-05-20 18:20:59.000000 exoplanet_atlas-0.3.5/exoplanet_atlas/visualizations/tweaks.py
-drwxr-xr-x   0 zach       (502) staff       (20)        0 2024-05-31 20:21:31.518845 exoplanet_atlas-0.3.5/exoplanet_atlas/whatsup/
--rw-r--r--   0 zach       (502) staff       (20)      164 2024-05-20 18:20:59.000000 exoplanet_atlas-0.3.5/exoplanet_atlas/whatsup/__init__.py
--rw-r--r--   0 zach       (502) staff       (20)     2073 2024-05-20 18:20:59.000000 exoplanet_atlas-0.3.5/exoplanet_atlas/whatsup/block.py
--rw-r--r--   0 zach       (502) staff       (20)      111 2024-05-20 18:20:59.000000 exoplanet_atlas-0.3.5/exoplanet_atlas/whatsup/night.py
--rw-r--r--   0 zach       (502) staff       (20)     6515 2024-05-20 18:20:59.000000 exoplanet_atlas-0.3.5/exoplanet_atlas/whatsup/observatory.py
--rw-r--r--   0 zach       (502) staff       (20)    11246 2024-05-20 20:56:00.000000 exoplanet_atlas-0.3.5/exoplanet_atlas/whatsup/plan.py
--rw-r--r--   0 zach       (502) staff       (20)     5940 2024-05-20 20:56:00.000000 exoplanet_atlas-0.3.5/exoplanet_atlas/whatsup/transit.py
-drwxr-xr-x   0 zach       (502) staff       (20)        0 2024-05-31 20:21:31.519052 exoplanet_atlas-0.3.5/exoplanet_atlas.egg-info/
--rw-r--r--   0 zach       (502) staff       (20)     1533 2024-05-31 20:21:31.000000 exoplanet_atlas-0.3.5/exoplanet_atlas.egg-info/PKG-INFO
--rw-r--r--   0 zach       (502) staff       (20)     2701 2024-05-31 20:21:31.000000 exoplanet_atlas-0.3.5/exoplanet_atlas.egg-info/SOURCES.txt
--rw-r--r--   0 zach       (502) staff       (20)        1 2024-05-31 20:21:31.000000 exoplanet_atlas-0.3.5/exoplanet_atlas.egg-info/dependency_links.txt
--rw-r--r--   0 zach       (502) staff       (20)        1 2024-05-20 18:33:32.000000 exoplanet_atlas-0.3.5/exoplanet_atlas.egg-info/not-zip-safe
--rw-r--r--   0 zach       (502) staff       (20)      300 2024-05-31 20:21:31.000000 exoplanet_atlas-0.3.5/exoplanet_atlas.egg-info/requires.txt
--rw-r--r--   0 zach       (502) staff       (20)       16 2024-05-31 20:21:31.000000 exoplanet_atlas-0.3.5/exoplanet_atlas.egg-info/top_level.txt
--rw-r--r--   0 zach       (502) staff       (20)       38 2024-05-31 20:21:31.520335 exoplanet_atlas-0.3.5/setup.cfg
--rw-r--r--   0 zach       (502) staff       (20)     4035 2024-05-31 20:01:26.000000 exoplanet_atlas-0.3.5/setup.py
+drwxr-xr-x   0 zach       (502) staff       (20)        0 2024-05-31 20:40:23.326010 exoplanet_atlas-0.3.6/
+-rw-r--r--   0 zach       (502) staff       (20)     1091 2024-05-20 20:56:00.000000 exoplanet_atlas-0.3.6/LICENSE
+-rw-r--r--   0 zach       (502) staff       (20)     1533 2024-05-31 20:40:23.325805 exoplanet_atlas-0.3.6/PKG-INFO
+-rw-r--r--   0 zach       (502) staff       (20)     1942 2024-05-31 20:01:26.000000 exoplanet_atlas-0.3.6/README.md
+drwxr-xr-x   0 zach       (502) staff       (20)        0 2024-05-31 20:40:23.311414 exoplanet_atlas-0.3.6/exoplanet_atlas/
+-rw-r--r--   0 zach       (502) staff       (20)      179 2024-05-20 20:56:00.000000 exoplanet_atlas-0.3.6/exoplanet_atlas/__init__.py
+-rw-r--r--   0 zach       (502) staff       (20)     4760 2024-05-31 20:32:08.000000 exoplanet_atlas-0.3.6/exoplanet_atlas/imports.py
+drwxr-xr-x   0 zach       (502) staff       (20)        0 2024-05-31 20:40:23.312888 exoplanet_atlas-0.3.6/exoplanet_atlas/models/
+-rw-r--r--   0 zach       (502) staff       (20)       87 2024-05-20 18:20:59.000000 exoplanet_atlas-0.3.6/exoplanet_atlas/models/__init__.py
+-rw-r--r--   0 zach       (502) staff       (20)     2084 2024-05-20 18:20:59.000000 exoplanet_atlas-0.3.6/exoplanet_atlas/models/chen.py
+-rw-r--r--   0 zach       (502) staff       (20)     1541 2024-05-20 20:56:00.000000 exoplanet_atlas-0.3.6/exoplanet_atlas/models/kopparapu.py
+-rw-r--r--   0 zach       (502) staff       (20)     1171 2024-05-20 20:56:00.000000 exoplanet_atlas-0.3.6/exoplanet_atlas/models/seager.py
+-rw-r--r--   0 zach       (502) staff       (20)      963 2024-05-20 20:56:00.000000 exoplanet_atlas-0.3.6/exoplanet_atlas/models/zeng.py
+drwxr-xr-x   0 zach       (502) staff       (20)        0 2024-05-31 20:40:23.315590 exoplanet_atlas-0.3.6/exoplanet_atlas/populations/
+-rw-r--r--   0 zach       (502) staff       (20)    13402 2024-05-20 20:56:00.000000 exoplanet_atlas-0.3.6/exoplanet_atlas/populations/Exoplanets.py
+-rw-r--r--   0 zach       (502) staff       (20)    51427 2024-05-31 20:01:16.000000 exoplanet_atlas-0.3.6/exoplanet_atlas/populations/Population.py
+-rw-r--r--   0 zach       (502) staff       (20)     3598 2024-05-23 06:36:30.000000 exoplanet_atlas-0.3.6/exoplanet_atlas/populations/SolarSystem.py
+-rw-r--r--   0 zach       (502) staff       (20)       62 2024-05-20 18:20:59.000000 exoplanet_atlas-0.3.6/exoplanet_atlas/populations/TESS.py
+-rw-r--r--   0 zach       (502) staff       (20)     7538 2024-05-20 20:56:00.000000 exoplanet_atlas-0.3.6/exoplanet_atlas/populations/TOI.py
+-rw-r--r--   0 zach       (502) staff       (20)     3485 2024-05-20 18:20:59.000000 exoplanet_atlas-0.3.6/exoplanet_atlas/populations/TOISubsets.py
+-rw-r--r--   0 zach       (502) staff       (20)     3351 2024-05-20 18:20:59.000000 exoplanet_atlas-0.3.6/exoplanet_atlas/populations/TransitingExoplanets.py
+-rw-r--r--   0 zach       (502) staff       (20)     5718 2024-05-20 20:56:00.000000 exoplanet_atlas-0.3.6/exoplanet_atlas/populations/TransitingExoplanetsSubsets.py
+-rw-r--r--   0 zach       (502) staff       (20)      416 2024-05-20 18:20:59.000000 exoplanet_atlas-0.3.6/exoplanet_atlas/populations/__init__.py
+-rw-r--r--   0 zach       (502) staff       (20)      716 2024-05-20 18:20:59.000000 exoplanet_atlas-0.3.6/exoplanet_atlas/populations/collections.py
+-rw-r--r--   0 zach       (502) staff       (20)     2258 2024-05-20 20:56:00.000000 exoplanet_atlas-0.3.6/exoplanet_atlas/populations/column_descriptions.py
+drwxr-xr-x   0 zach       (502) staff       (20)        0 2024-05-31 20:40:23.316202 exoplanet_atlas-0.3.6/exoplanet_atlas/populations/curation/
+-rw-r--r--   0 zach       (502) staff       (20)     7747 2024-05-20 20:56:00.000000 exoplanet_atlas-0.3.6/exoplanet_atlas/populations/curation/Confirmed.py
+-rw-r--r--   0 zach       (502) staff       (20)       26 2024-05-20 18:20:59.000000 exoplanet_atlas-0.3.6/exoplanet_atlas/populations/curation/TransitingExoplanets.py
+-rw-r--r--   0 zach       (502) staff       (20)        0 2024-05-20 18:20:59.000000 exoplanet_atlas-0.3.6/exoplanet_atlas/populations/curation/__init__.py
+-rw-r--r--   0 zach       (502) staff       (20)     9005 2024-05-31 20:01:16.000000 exoplanet_atlas-0.3.6/exoplanet_atlas/populations/downloaders.py
+-rw-r--r--   0 zach       (502) staff       (20)     1963 2024-05-20 20:56:00.000000 exoplanet_atlas-0.3.6/exoplanet_atlas/populations/summary.py
+-rw-r--r--   0 zach       (502) staff       (20)     2735 2024-05-20 20:56:00.000000 exoplanet_atlas-0.3.6/exoplanet_atlas/talker.py
+drwxr-xr-x   0 zach       (502) staff       (20)        0 2024-05-31 20:40:23.316410 exoplanet_atlas-0.3.6/exoplanet_atlas/telescopes/
+-rw-r--r--   0 zach       (502) staff       (20)       23 2024-05-20 18:20:59.000000 exoplanet_atlas-0.3.6/exoplanet_atlas/telescopes/__init__.py
+-rw-r--r--   0 zach       (502) staff       (20)     6048 2024-05-23 06:36:30.000000 exoplanet_atlas-0.3.6/exoplanet_atlas/telescopes/buckets.py
+drwxr-xr-x   0 zach       (502) staff       (20)        0 2024-05-31 20:40:23.319293 exoplanet_atlas-0.3.6/exoplanet_atlas/tests/
+-rw-r--r--   0 zach       (502) staff       (20)      268 2024-05-20 18:20:59.000000 exoplanet_atlas-0.3.6/exoplanet_atlas/tests/__init__.py
+-rw-r--r--   0 zach       (502) staff       (20)       40 2024-05-20 20:56:00.000000 exoplanet_atlas-0.3.6/exoplanet_atlas/tests/setup_tests.py
+-rw-r--r--   0 zach       (502) staff       (20)     1084 2024-05-31 20:01:16.000000 exoplanet_atlas-0.3.6/exoplanet_atlas/tests/test_buckets.py
+-rw-r--r--   0 zach       (502) staff       (20)      592 2024-05-31 20:01:16.000000 exoplanet_atlas-0.3.6/exoplanet_atlas/tests/test_downloaders.py
+-rw-r--r--   0 zach       (502) staff       (20)      370 2024-05-31 20:01:16.000000 exoplanet_atlas-0.3.6/exoplanet_atlas/tests/test_imports.py
+-rw-r--r--   0 zach       (502) staff       (20)      689 2024-05-31 20:01:16.000000 exoplanet_atlas-0.3.6/exoplanet_atlas/tests/test_models.py
+-rw-r--r--   0 zach       (502) staff       (20)     3298 2024-05-31 20:01:16.000000 exoplanet_atlas-0.3.6/exoplanet_atlas/tests/test_populations.py
+-rw-r--r--   0 zach       (502) staff       (20)     2496 2024-05-31 20:01:16.000000 exoplanet_atlas-0.3.6/exoplanet_atlas/tests/test_snr.py
+-rw-r--r--   0 zach       (502) staff       (20)      626 2024-05-31 20:01:16.000000 exoplanet_atlas-0.3.6/exoplanet_atlas/tests/test_uncertainties.py
+-rw-r--r--   0 zach       (502) staff       (20)     1411 2024-05-31 20:01:16.000000 exoplanet_atlas-0.3.6/exoplanet_atlas/tests/test_visualizations.py
+-rw-r--r--   0 zach       (502) staff       (20)      722 2024-05-31 20:01:16.000000 exoplanet_atlas-0.3.6/exoplanet_atlas/tests/test_whatsup.py
+-rw-r--r--   0 zach       (502) staff       (20)      193 2024-05-31 20:40:16.000000 exoplanet_atlas-0.3.6/exoplanet_atlas/version.py
+drwxr-xr-x   0 zach       (502) staff       (20)        0 2024-05-31 20:40:23.320531 exoplanet_atlas-0.3.6/exoplanet_atlas/visualizations/
+-rw-r--r--   0 zach       (502) staff       (20)     4138 2024-05-31 20:01:16.000000 exoplanet_atlas-0.3.6/exoplanet_atlas/visualizations/MultiPanel.py
+-rw-r--r--   0 zach       (502) staff       (20)      818 2024-05-31 20:01:16.000000 exoplanet_atlas-0.3.6/exoplanet_atlas/visualizations/ThumbtackMovie.py
+-rw-r--r--   0 zach       (502) staff       (20)    14017 2024-05-20 18:20:59.000000 exoplanet_atlas-0.3.6/exoplanet_atlas/visualizations/ThumbtackPlot.py
+-rw-r--r--   0 zach       (502) staff       (20)       95 2024-05-20 18:20:59.000000 exoplanet_atlas-0.3.6/exoplanet_atlas/visualizations/__init__.py
+drwxr-xr-x   0 zach       (502) staff       (20)        0 2024-05-31 20:40:23.320922 exoplanet_atlas-0.3.6/exoplanet_atlas/visualizations/axes/
+-rw-r--r--   0 zach       (502) staff       (20)       58 2024-05-20 18:20:59.000000 exoplanet_atlas-0.3.6/exoplanet_atlas/visualizations/axes/__init__.py
+-rw-r--r--   0 zach       (502) staff       (20)     4309 2024-05-20 18:20:59.000000 exoplanet_atlas-0.3.6/exoplanet_atlas/visualizations/axes/plottable.py
+-rw-r--r--   0 zach       (502) staff       (20)    13910 2024-05-23 06:36:30.000000 exoplanet_atlas-0.3.6/exoplanet_atlas/visualizations/axes/preset_plottables.py
+-rw-r--r--   0 zach       (502) staff       (20)     8240 2024-05-23 06:36:30.000000 exoplanet_atlas-0.3.6/exoplanet_atlas/visualizations/buildable.py
+-rw-r--r--   0 zach       (502) staff       (20)     2846 2024-05-20 20:56:00.000000 exoplanet_atlas-0.3.6/exoplanet_atlas/visualizations/ink_errorbar.py
+drwxr-xr-x   0 zach       (502) staff       (20)        0 2024-05-31 20:40:23.321681 exoplanet_atlas-0.3.6/exoplanet_atlas/visualizations/panels/
+-rw-r--r--   0 zach       (502) staff       (20)     9710 2024-05-20 20:56:00.000000 exoplanet_atlas-0.3.6/exoplanet_atlas/visualizations/panels/BubblePanel.py
+-rw-r--r--   0 zach       (502) staff       (20)     7716 2024-05-23 06:36:30.000000 exoplanet_atlas-0.3.6/exoplanet_atlas/visualizations/panels/ErrorPanel.py
+-rw-r--r--   0 zach       (502) staff       (20)    12096 2024-05-20 18:20:59.000000 exoplanet_atlas-0.3.6/exoplanet_atlas/visualizations/panels/Panel.py
+-rw-r--r--   0 zach       (502) staff       (20)      103 2024-05-20 18:20:59.000000 exoplanet_atlas-0.3.6/exoplanet_atlas/visualizations/panels/__init__.py
+-rw-r--r--   0 zach       (502) staff       (20)     9782 2024-05-20 18:20:59.000000 exoplanet_atlas-0.3.6/exoplanet_atlas/visualizations/panels/preset_panels.py
+-rw-r--r--   0 zach       (502) staff       (20)      858 2024-05-20 18:20:59.000000 exoplanet_atlas-0.3.6/exoplanet_atlas/visualizations/tweaks.py
+drwxr-xr-x   0 zach       (502) staff       (20)        0 2024-05-31 20:40:23.324619 exoplanet_atlas-0.3.6/exoplanet_atlas/whatsup/
+-rw-r--r--   0 zach       (502) staff       (20)      164 2024-05-20 18:20:59.000000 exoplanet_atlas-0.3.6/exoplanet_atlas/whatsup/__init__.py
+-rw-r--r--   0 zach       (502) staff       (20)     2073 2024-05-20 18:20:59.000000 exoplanet_atlas-0.3.6/exoplanet_atlas/whatsup/block.py
+-rw-r--r--   0 zach       (502) staff       (20)      111 2024-05-20 18:20:59.000000 exoplanet_atlas-0.3.6/exoplanet_atlas/whatsup/night.py
+-rw-r--r--   0 zach       (502) staff       (20)     6515 2024-05-20 18:20:59.000000 exoplanet_atlas-0.3.6/exoplanet_atlas/whatsup/observatory.py
+-rw-r--r--   0 zach       (502) staff       (20)    11246 2024-05-20 20:56:00.000000 exoplanet_atlas-0.3.6/exoplanet_atlas/whatsup/plan.py
+-rw-r--r--   0 zach       (502) staff       (20)     5940 2024-05-20 20:56:00.000000 exoplanet_atlas-0.3.6/exoplanet_atlas/whatsup/transit.py
+drwxr-xr-x   0 zach       (502) staff       (20)        0 2024-05-31 20:40:23.324930 exoplanet_atlas-0.3.6/exoplanet_atlas.egg-info/
+-rw-r--r--   0 zach       (502) staff       (20)     1533 2024-05-31 20:40:23.000000 exoplanet_atlas-0.3.6/exoplanet_atlas.egg-info/PKG-INFO
+-rw-r--r--   0 zach       (502) staff       (20)     2701 2024-05-31 20:40:23.000000 exoplanet_atlas-0.3.6/exoplanet_atlas.egg-info/SOURCES.txt
+-rw-r--r--   0 zach       (502) staff       (20)        1 2024-05-31 20:40:23.000000 exoplanet_atlas-0.3.6/exoplanet_atlas.egg-info/dependency_links.txt
+-rw-r--r--   0 zach       (502) staff       (20)        1 2024-05-20 18:33:32.000000 exoplanet_atlas-0.3.6/exoplanet_atlas.egg-info/not-zip-safe
+-rw-r--r--   0 zach       (502) staff       (20)      300 2024-05-31 20:40:23.000000 exoplanet_atlas-0.3.6/exoplanet_atlas.egg-info/requires.txt
+-rw-r--r--   0 zach       (502) staff       (20)       16 2024-05-31 20:40:23.000000 exoplanet_atlas-0.3.6/exoplanet_atlas.egg-info/top_level.txt
+-rw-r--r--   0 zach       (502) staff       (20)       38 2024-05-31 20:40:23.326048 exoplanet_atlas-0.3.6/setup.cfg
+-rw-r--r--   0 zach       (502) staff       (20)     4032 2024-05-31 20:40:01.000000 exoplanet_atlas-0.3.6/setup.py
```

### Comparing `exoplanet_atlas-0.3.5/LICENSE` & `exoplanet_atlas-0.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `exoplanet_atlas-0.3.5/PKG-INFO` & `exoplanet_atlas-0.3.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: exoplanet_atlas
-Version: 0.3.5
+Version: 0.3.6
 Summary: Tools for working with transiting exoplanet populations.
 Home-page: https://github.com/zkbt/exoplanet_atlas
 Author: Zach Berta-Thompson
 Author-email: zach.bertathompson@colorado.edu
 License: MIT
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python
 Classifier: Topic :: Scientific/Engineering :: Astronomy
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 License-File: LICENSE
 Requires-Dist: numpy>=1.13
 Requires-Dist: matplotlib>=2.0
 Requires-Dist: astropy>=3.2.3
 Requires-Dist: astroquery>=0.3.9
 Requires-Dist: astroplan>=0.10
 Requires-Dist: rainbow-connection>=0.0.1
```

### Comparing `exoplanet_atlas-0.3.5/README.md` & `exoplanet_atlas-0.3.6/README.md`

 * *Files identical despite different names*

### Comparing `exoplanet_atlas-0.3.5/exoplanet_atlas/imports.py` & `exoplanet_atlas-0.3.6/exoplanet_atlas/imports.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,21 @@
+from .version import *
+
 # imports that are need by many exoplanet_atlas subsections
 from ast import Import
 import os, sys, time, shutil, warnings, copy
 from tqdm import tqdm
 
 # (possibly different on Mac, Linux, Windows, even for Python versions 3.8-3.12)
 try:
     from importlib.resources import files
 except (ModuleNotFoundError, AttributeError, ImportError):
     from importlib_resources import files
 
-code_directory = files("exoplanet_atlas")
+code_directory = files(import_name)
 
 
 import numpy as np, matplotlib.pyplot as plt, matplotlib.animation as animation
 from matplotlib.ticker import ScalarFormatter, FormatStrFormatter, LogLocator
 
 
 from astropy.utils.exceptions import AstropyDeprecationWarning
```

### Comparing `exoplanet_atlas-0.3.5/exoplanet_atlas/models/chen.py` & `exoplanet_atlas-0.3.6/exoplanet_atlas/models/chen.py`

 * *Files identical despite different names*

### Comparing `exoplanet_atlas-0.3.5/exoplanet_atlas/models/kopparapu.py` & `exoplanet_atlas-0.3.6/exoplanet_atlas/models/kopparapu.py`

 * *Files identical despite different names*

### Comparing `exoplanet_atlas-0.3.5/exoplanet_atlas/models/seager.py` & `exoplanet_atlas-0.3.6/exoplanet_atlas/models/seager.py`

 * *Files identical despite different names*

### Comparing `exoplanet_atlas-0.3.5/exoplanet_atlas/models/zeng.py` & `exoplanet_atlas-0.3.6/exoplanet_atlas/models/zeng.py`

 * *Files identical despite different names*

### Comparing `exoplanet_atlas-0.3.5/exoplanet_atlas/populations/Exoplanets.py` & `exoplanet_atlas-0.3.6/exoplanet_atlas/populations/Exoplanets.py`

 * *Files identical despite different names*

### Comparing `exoplanet_atlas-0.3.5/exoplanet_atlas/populations/Population.py` & `exoplanet_atlas-0.3.6/exoplanet_atlas/populations/Population.py`

 * *Files identical despite different names*

### Comparing `exoplanet_atlas-0.3.5/exoplanet_atlas/populations/SolarSystem.py` & `exoplanet_atlas-0.3.6/exoplanet_atlas/populations/SolarSystem.py`

 * *Files identical despite different names*

### Comparing `exoplanet_atlas-0.3.5/exoplanet_atlas/populations/TOI.py` & `exoplanet_atlas-0.3.6/exoplanet_atlas/populations/TOI.py`

 * *Files identical despite different names*

### Comparing `exoplanet_atlas-0.3.5/exoplanet_atlas/populations/TOISubsets.py` & `exoplanet_atlas-0.3.6/exoplanet_atlas/populations/TOISubsets.py`

 * *Files identical despite different names*

### Comparing `exoplanet_atlas-0.3.5/exoplanet_atlas/populations/TransitingExoplanets.py` & `exoplanet_atlas-0.3.6/exoplanet_atlas/populations/TransitingExoplanets.py`

 * *Files identical despite different names*

### Comparing `exoplanet_atlas-0.3.5/exoplanet_atlas/populations/TransitingExoplanetsSubsets.py` & `exoplanet_atlas-0.3.6/exoplanet_atlas/populations/TransitingExoplanetsSubsets.py`

 * *Files identical despite different names*

### Comparing `exoplanet_atlas-0.3.5/exoplanet_atlas/populations/collections.py` & `exoplanet_atlas-0.3.6/exoplanet_atlas/populations/collections.py`

 * *Files identical despite different names*

### Comparing `exoplanet_atlas-0.3.5/exoplanet_atlas/populations/column_descriptions.py` & `exoplanet_atlas-0.3.6/exoplanet_atlas/populations/column_descriptions.py`

 * *Files identical despite different names*

### Comparing `exoplanet_atlas-0.3.5/exoplanet_atlas/populations/curation/Confirmed.py` & `exoplanet_atlas-0.3.6/exoplanet_atlas/populations/curation/Confirmed.py`

 * *Files identical despite different names*

### Comparing `exoplanet_atlas-0.3.5/exoplanet_atlas/populations/downloaders.py` & `exoplanet_atlas-0.3.6/exoplanet_atlas/populations/downloaders.py`

 * *Files identical despite different names*

### Comparing `exoplanet_atlas-0.3.5/exoplanet_atlas/populations/summary.py` & `exoplanet_atlas-0.3.6/exoplanet_atlas/populations/summary.py`

 * *Files identical despite different names*

### Comparing `exoplanet_atlas-0.3.5/exoplanet_atlas/talker.py` & `exoplanet_atlas-0.3.6/exoplanet_atlas/talker.py`

 * *Files identical despite different names*

### Comparing `exoplanet_atlas-0.3.5/exoplanet_atlas/telescopes/buckets.py` & `exoplanet_atlas-0.3.6/exoplanet_atlas/telescopes/buckets.py`

 * *Files identical despite different names*

### Comparing `exoplanet_atlas-0.3.5/exoplanet_atlas/tests/test_buckets.py` & `exoplanet_atlas-0.3.6/exoplanet_atlas/tests/test_buckets.py`

 * *Files identical despite different names*

### Comparing `exoplanet_atlas-0.3.5/exoplanet_atlas/tests/test_downloaders.py` & `exoplanet_atlas-0.3.6/exoplanet_atlas/tests/test_downloaders.py`

 * *Files identical despite different names*

### Comparing `exoplanet_atlas-0.3.5/exoplanet_atlas/tests/test_models.py` & `exoplanet_atlas-0.3.6/exoplanet_atlas/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `exoplanet_atlas-0.3.5/exoplanet_atlas/tests/test_populations.py` & `exoplanet_atlas-0.3.6/exoplanet_atlas/tests/test_populations.py`

 * *Files identical despite different names*

### Comparing `exoplanet_atlas-0.3.5/exoplanet_atlas/tests/test_snr.py` & `exoplanet_atlas-0.3.6/exoplanet_atlas/tests/test_snr.py`

 * *Files identical despite different names*

### Comparing `exoplanet_atlas-0.3.5/exoplanet_atlas/tests/test_uncertainties.py` & `exoplanet_atlas-0.3.6/exoplanet_atlas/tests/test_uncertainties.py`

 * *Files identical despite different names*

### Comparing `exoplanet_atlas-0.3.5/exoplanet_atlas/tests/test_visualizations.py` & `exoplanet_atlas-0.3.6/exoplanet_atlas/tests/test_visualizations.py`

 * *Files identical despite different names*

### Comparing `exoplanet_atlas-0.3.5/exoplanet_atlas/tests/test_whatsup.py` & `exoplanet_atlas-0.3.6/exoplanet_atlas/tests/test_whatsup.py`

 * *Files identical despite different names*

### Comparing `exoplanet_atlas-0.3.5/exoplanet_atlas/visualizations/MultiPanel.py` & `exoplanet_atlas-0.3.6/exoplanet_atlas/visualizations/MultiPanel.py`

 * *Files identical despite different names*

### Comparing `exoplanet_atlas-0.3.5/exoplanet_atlas/visualizations/ThumbtackMovie.py` & `exoplanet_atlas-0.3.6/exoplanet_atlas/visualizations/ThumbtackMovie.py`

 * *Files identical despite different names*

### Comparing `exoplanet_atlas-0.3.5/exoplanet_atlas/visualizations/ThumbtackPlot.py` & `exoplanet_atlas-0.3.6/exoplanet_atlas/visualizations/ThumbtackPlot.py`

 * *Files identical despite different names*

### Comparing `exoplanet_atlas-0.3.5/exoplanet_atlas/visualizations/axes/plottable.py` & `exoplanet_atlas-0.3.6/exoplanet_atlas/visualizations/axes/plottable.py`

 * *Files identical despite different names*

### Comparing `exoplanet_atlas-0.3.5/exoplanet_atlas/visualizations/axes/preset_plottables.py` & `exoplanet_atlas-0.3.6/exoplanet_atlas/visualizations/axes/preset_plottables.py`

 * *Files identical despite different names*

### Comparing `exoplanet_atlas-0.3.5/exoplanet_atlas/visualizations/buildable.py` & `exoplanet_atlas-0.3.6/exoplanet_atlas/visualizations/buildable.py`

 * *Files identical despite different names*

### Comparing `exoplanet_atlas-0.3.5/exoplanet_atlas/visualizations/ink_errorbar.py` & `exoplanet_atlas-0.3.6/exoplanet_atlas/visualizations/ink_errorbar.py`

 * *Files identical despite different names*

### Comparing `exoplanet_atlas-0.3.5/exoplanet_atlas/visualizations/panels/BubblePanel.py` & `exoplanet_atlas-0.3.6/exoplanet_atlas/visualizations/panels/BubblePanel.py`

 * *Files identical despite different names*

### Comparing `exoplanet_atlas-0.3.5/exoplanet_atlas/visualizations/panels/ErrorPanel.py` & `exoplanet_atlas-0.3.6/exoplanet_atlas/visualizations/panels/ErrorPanel.py`

 * *Files identical despite different names*

### Comparing `exoplanet_atlas-0.3.5/exoplanet_atlas/visualizations/panels/Panel.py` & `exoplanet_atlas-0.3.6/exoplanet_atlas/visualizations/panels/Panel.py`

 * *Files identical despite different names*

### Comparing `exoplanet_atlas-0.3.5/exoplanet_atlas/visualizations/panels/preset_panels.py` & `exoplanet_atlas-0.3.6/exoplanet_atlas/visualizations/panels/preset_panels.py`

 * *Files identical despite different names*

### Comparing `exoplanet_atlas-0.3.5/exoplanet_atlas/visualizations/tweaks.py` & `exoplanet_atlas-0.3.6/exoplanet_atlas/visualizations/tweaks.py`

 * *Files identical despite different names*

### Comparing `exoplanet_atlas-0.3.5/exoplanet_atlas/whatsup/block.py` & `exoplanet_atlas-0.3.6/exoplanet_atlas/whatsup/block.py`

 * *Files identical despite different names*

### Comparing `exoplanet_atlas-0.3.5/exoplanet_atlas/whatsup/observatory.py` & `exoplanet_atlas-0.3.6/exoplanet_atlas/whatsup/observatory.py`

 * *Files identical despite different names*

### Comparing `exoplanet_atlas-0.3.5/exoplanet_atlas/whatsup/plan.py` & `exoplanet_atlas-0.3.6/exoplanet_atlas/whatsup/plan.py`

 * *Files identical despite different names*

### Comparing `exoplanet_atlas-0.3.5/exoplanet_atlas/whatsup/transit.py` & `exoplanet_atlas-0.3.6/exoplanet_atlas/whatsup/transit.py`

 * *Files identical despite different names*

### Comparing `exoplanet_atlas-0.3.5/exoplanet_atlas.egg-info/PKG-INFO` & `exoplanet_atlas-0.3.6/exoplanet_atlas.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: exoplanet_atlas
-Version: 0.3.5
+Version: 0.3.6
 Summary: Tools for working with transiting exoplanet populations.
 Home-page: https://github.com/zkbt/exoplanet_atlas
 Author: Zach Berta-Thompson
 Author-email: zach.bertathompson@colorado.edu
 License: MIT
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python
 Classifier: Topic :: Scientific/Engineering :: Astronomy
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 License-File: LICENSE
 Requires-Dist: numpy>=1.13
 Requires-Dist: matplotlib>=2.0
 Requires-Dist: astropy>=3.2.3
 Requires-Dist: astroquery>=0.3.9
 Requires-Dist: astroplan>=0.10
 Requires-Dist: rainbow-connection>=0.0.1
```

### Comparing `exoplanet_atlas-0.3.5/exoplanet_atlas.egg-info/SOURCES.txt` & `exoplanet_atlas-0.3.6/exoplanet_atlas.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `exoplanet_atlas-0.3.5/setup.py` & `exoplanet_atlas-0.3.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 
 # running `python setup.py release` from the command line will post to PyPI
 if "release" in sys.argv[-1]:
     os.system("python setup.py sdist")
     # uncomment the next line to test out on test.pypi.com/project/tess-zap
     # os.system("twine upload --repository-url https://test.pypi.org/legacy/ dist/*")
     os.system("twine upload dist/*")
-    os.system("rm -rf dist/rainbow-connection*")
+    os.system("rm -rf dist/exoplanet_atlas*")
     sys.exit()
 
 # a little kludge to get the version number from __version__
 exec(open("exoplanet_atlas/version.py").read())
 
 # run the setup function
 setup(
@@ -105,13 +105,13 @@
             "mkdocs-jupyter",
             "mkdocs-exclude",
             "twine",
             "pre-commit",
         ]
     },
     # what version of Python is required?
-    python_requires=">=3.8",
+    python_requires=">=3.9",
     # (I think just leave this set to False)
     zip_safe=False,
     # under what license is this code released?
     license="MIT",
 )
```

