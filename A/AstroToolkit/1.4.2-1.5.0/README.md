# Comparing `tmp/astrotoolkit-1.4.2.tar.gz` & `tmp/astrotoolkit-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "astrotoolkit-1.4.2.tar", last modified: Sat Apr 13 21:48:09 2024, max compression
+gzip compressed data, was "astrotoolkit-1.5.0.tar", last modified: Fri May 31 11:22:24 2024, max compression
```

## Comparing `astrotoolkit-1.4.2.tar` & `astrotoolkit-1.5.0.tar`

### file list

```diff
@@ -1,50 +1,69 @@
-drwxrwxrwx   0        0        0        0 2024-04-13 21:48:09.777568 astrotoolkit-1.4.2/
--rw-rw-rw-   0        0        0        0 2024-01-11 16:40:26.000000 astrotoolkit-1.4.2/LICENSE
--rw-rw-rw-   0        0        0      297 2024-02-04 17:52:40.000000 astrotoolkit-1.4.2/MANIFEST.in
--rw-rw-rw-   0        0        0    37829 2024-04-13 21:48:09.775567 astrotoolkit-1.4.2/PKG-INFO
--rw-rw-rw-   0        0        0    36909 2024-04-13 21:47:31.000000 astrotoolkit-1.4.2/README.md
--rw-rw-rw-   0        0        0      967 2024-04-13 21:48:02.000000 astrotoolkit-1.4.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-13 21:48:09.777568 astrotoolkit-1.4.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-13 21:48:09.669545 astrotoolkit-1.4.2/src/
-drwxrwxrwx   0        0        0        0 2024-04-13 21:48:09.677545 astrotoolkit-1.4.2/src/AstroToolkit/
-drwxrwxrwx   0        0        0        0 2024-04-13 21:48:09.748561 astrotoolkit-1.4.2/src/AstroToolkit/Data/
--rw-rw-rw-   0        0        0    14934 2024-04-13 19:49:21.000000 astrotoolkit-1.4.2/src/AstroToolkit/Data/data.py
--rw-rw-rw-   0        0        0     6345 2024-04-13 19:48:56.000000 astrotoolkit-1.4.2/src/AstroToolkit/Data/imaging.py
--rw-rw-rw-   0        0        0     3489 2024-03-15 17:17:57.000000 astrotoolkit-1.4.2/src/AstroToolkit/Data/lightcurve_sigma_clip.py
--rw-rw-rw-   0        0        0    23062 2024-04-05 17:22:00.000000 astrotoolkit-1.4.2/src/AstroToolkit/Data/lightcurves.py
--rw-rw-rw-   0        0        0    10513 2024-04-13 19:53:03.000000 astrotoolkit-1.4.2/src/AstroToolkit/Data/overlays.py
--rw-rw-rw-   0        0        0     2763 2024-01-17 19:10:24.000000 astrotoolkit-1.4.2/src/AstroToolkit/Data/photometry.py
--rw-rw-rw-   0        0        0     2618 2024-04-05 17:44:53.000000 astrotoolkit-1.4.2/src/AstroToolkit/Data/reddening.py
--rw-rw-rw-   0        0        0     4282 2024-04-13 19:53:18.000000 astrotoolkit-1.4.2/src/AstroToolkit/Data/sed.py
--rw-rw-rw-   0        0        0     1978 2024-04-05 17:27:41.000000 astrotoolkit-1.4.2/src/AstroToolkit/Data/spectra.py
-drwxrwxrwx   0        0        0        0 2024-04-13 21:48:09.751561 astrotoolkit-1.4.2/src/AstroToolkit/Datapages/
--rw-rw-rw-   0        0        0     2751 2024-04-05 17:28:09.000000 astrotoolkit-1.4.2/src/AstroToolkit/Datapages/buttons.py
--rw-rw-rw-   0        0        0     3771 2024-04-13 19:53:32.000000 astrotoolkit-1.4.2/src/AstroToolkit/Datapages/grid.py
--rw-rw-rw-   0        0        0     8223 2024-04-13 19:53:36.000000 astrotoolkit-1.4.2/src/AstroToolkit/Datapages/metadata.py
-drwxrwxrwx   0        0        0        0 2024-04-13 21:48:09.752561 astrotoolkit-1.4.2/src/AstroToolkit/Examples/
--rw-rw-rw-   0        0        0     2844 2024-04-13 21:06:25.000000 astrotoolkit-1.4.2/src/AstroToolkit/Examples/datapage_creation.py
-drwxrwxrwx   0        0        0        0 2024-04-13 21:48:09.762564 astrotoolkit-1.4.2/src/AstroToolkit/Misc/
--rw-rw-rw-   0        0        0     2364 2024-04-13 19:54:09.000000 astrotoolkit-1.4.2/src/AstroToolkit/Misc/ProperMotionCorrection.py
--rw-rw-rw-   0        0        0     2540 2024-02-21 13:02:49.000000 astrotoolkit-1.4.2/src/AstroToolkit/Misc/coord_conversion.py
--rw-rw-rw-   0        0        0     1625 2024-04-05 17:29:14.000000 astrotoolkit-1.4.2/src/AstroToolkit/Misc/database_queries.py
--rw-rw-rw-   0        0        0    18188 2024-03-28 16:04:31.000000 astrotoolkit-1.4.2/src/AstroToolkit/Misc/file_handling.py
--rw-rw-rw-   0        0        0     4308 2024-04-05 22:43:02.000000 astrotoolkit-1.4.2/src/AstroToolkit/Misc/file_naming.py
--rw-rw-rw-   0        0        0     2937 2024-04-05 17:40:17.000000 astrotoolkit-1.4.2/src/AstroToolkit/Misc/input_validation.py
--rw-rw-rw-   0        0        0     3244 2024-03-15 18:39:31.000000 astrotoolkit-1.4.2/src/AstroToolkit/Misc/read_fits.py
-drwxrwxrwx   0        0        0        0 2024-04-13 21:48:09.771566 astrotoolkit-1.4.2/src/AstroToolkit/Plotting/
--rw-rw-rw-   0        0        0     4489 2024-04-13 19:54:26.000000 astrotoolkit-1.4.2/src/AstroToolkit/Plotting/HRD.py
--rw-rw-rw-   0        0        0  1224000 2024-01-11 16:40:26.000000 astrotoolkit-1.4.2/src/AstroToolkit/Plotting/backdrop_hrd_allmags.fits
--rw-rw-rw-   0        0        0     4547 2024-04-13 19:55:04.000000 astrotoolkit-1.4.2/src/AstroToolkit/Plotting/imaging.py
--rw-rw-rw-   0        0        0     5617 2024-04-13 20:13:26.000000 astrotoolkit-1.4.2/src/AstroToolkit/Plotting/lightcurves.py
--rw-rw-rw-   0        0        0     2647 2024-03-23 23:44:35.000000 astrotoolkit-1.4.2/src/AstroToolkit/Plotting/powspec.py
--rw-rw-rw-   0        0        0     2636 2024-04-13 20:14:08.000000 astrotoolkit-1.4.2/src/AstroToolkit/Plotting/sed.py
--rw-rw-rw-   0        0        0     3635 2024-04-13 19:55:43.000000 astrotoolkit-1.4.2/src/AstroToolkit/Plotting/spectra.py
-drwxrwxrwx   0        0        0        0 2024-04-13 21:48:09.772568 astrotoolkit-1.4.2/src/AstroToolkit/Settings/
--rw-rw-rw-   0        0        0        0 2024-02-04 19:17:29.000000 astrotoolkit-1.4.2/src/AstroToolkit/Settings/__init__.py
--rw-rw-rw-   0        0        0    32053 2024-04-13 20:28:43.000000 astrotoolkit-1.4.2/src/AstroToolkit/Tools.py
-drwxrwxrwx   0        0        0        0 2024-04-13 21:48:09.774567 astrotoolkit-1.4.2/src/AstroToolkit.egg-info/
--rw-rw-rw-   0        0        0    37829 2024-04-13 21:48:09.000000 astrotoolkit-1.4.2/src/AstroToolkit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1335 2024-04-13 21:48:09.000000 astrotoolkit-1.4.2/src/AstroToolkit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-13 21:48:09.000000 astrotoolkit-1.4.2/src/AstroToolkit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      205 2024-04-13 21:48:09.000000 astrotoolkit-1.4.2/src/AstroToolkit.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-04-13 21:48:09.000000 astrotoolkit-1.4.2/src/AstroToolkit.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-31 11:22:24.669930 astrotoolkit-1.5.0/
+-rw-rw-rw-   0        0        0        0 2024-01-11 16:40:26.000000 astrotoolkit-1.5.0/LICENSE
+-rw-rw-rw-   0        0        0      297 2024-02-04 17:52:40.000000 astrotoolkit-1.5.0/MANIFEST.in
+-rw-rw-rw-   0        0        0    41557 2024-05-31 11:22:24.669930 astrotoolkit-1.5.0/PKG-INFO
+-rw-rw-rw-   0        0        0    40672 2024-05-31 11:19:09.000000 astrotoolkit-1.5.0/README.md
+-rw-rw-rw-   0        0        0      944 2024-05-31 11:21:48.000000 astrotoolkit-1.5.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-31 11:22:24.669930 astrotoolkit-1.5.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-31 11:22:24.619580 astrotoolkit-1.5.0/src/
+drwxrwxrwx   0        0        0        0 2024-05-31 11:22:24.627611 astrotoolkit-1.5.0/src/AstroToolkit/
+-rw-rw-rw-   0        0        0      802 2024-05-30 23:24:18.000000 astrotoolkit-1.5.0/src/AstroToolkit/Config.py
+drwxrwxrwx   0        0        0        0 2024-05-31 11:22:24.642196 astrotoolkit-1.5.0/src/AstroToolkit/Configuration/
+-rw-rw-rw-   0        0        0     6324 2024-05-29 11:30:03.000000 astrotoolkit-1.5.0/src/AstroToolkit/Configuration/baseconfig.py
+drwxrwxrwx   0        0        0        0 2024-05-31 11:22:24.649706 astrotoolkit-1.5.0/src/AstroToolkit/Data/
+-rw-rw-rw-   0        0        0    18394 2024-05-30 23:34:31.000000 astrotoolkit-1.5.0/src/AstroToolkit/Data/dataquery.py
+-rw-rw-rw-   0        0        0     4318 2024-05-31 01:57:18.000000 astrotoolkit-1.5.0/src/AstroToolkit/Data/fetch_crts.py
+-rw-rw-rw-   0        0        0     1485 2024-05-31 01:38:24.000000 astrotoolkit-1.5.0/src/AstroToolkit/Data/hrdquery.py
+-rw-rw-rw-   0        0        0    10391 2024-05-31 01:22:50.000000 astrotoolkit-1.5.0/src/AstroToolkit/Data/imageoverlay.py
+-rw-rw-rw-   0        0        0     7341 2024-05-31 01:38:44.000000 astrotoolkit-1.5.0/src/AstroToolkit/Data/imagequery.py
+-rw-rw-rw-   0        0        0    22828 2024-05-31 01:38:48.000000 astrotoolkit-1.5.0/src/AstroToolkit/Data/lightcurvequery.py
+-rw-rw-rw-   0        0        0     5062 2024-05-30 23:34:08.000000 astrotoolkit-1.5.0/src/AstroToolkit/Data/photquery.py
+-rw-rw-rw-   0        0        0    12435 2024-05-23 23:55:37.000000 astrotoolkit-1.5.0/src/AstroToolkit/Data/reddeningquery.py
+-rw-rw-rw-   0        0        0    10458 2024-05-01 16:56:16.000000 astrotoolkit-1.5.0/src/AstroToolkit/Data/rename_headers.py
+-rw-rw-rw-   0        0        0     3090 2024-05-31 01:38:54.000000 astrotoolkit-1.5.0/src/AstroToolkit/Data/sedquery.py
+-rw-rw-rw-   0        0        0     3715 2024-05-20 10:52:42.000000 astrotoolkit-1.5.0/src/AstroToolkit/Data/sigmaclip.py
+-rw-rw-rw-   0        0        0     1951 2024-05-31 01:38:58.000000 astrotoolkit-1.5.0/src/AstroToolkit/Data/spectrumquery.py
+drwxrwxrwx   0        0        0        0 2024-05-31 11:22:24.650705 astrotoolkit-1.5.0/src/AstroToolkit/DatapageElements/
+-rw-rw-rw-   0        0        0     2433 2024-05-30 01:10:43.000000 astrotoolkit-1.5.0/src/AstroToolkit/DatapageElements/datapage_buttons.py
+-rw-rw-rw-   0        0        0     4667 2024-05-29 15:21:17.000000 astrotoolkit-1.5.0/src/AstroToolkit/DatapageElements/metadata_table.py
+-rw-rw-rw-   0        0        0     2184 2024-05-30 00:59:32.000000 astrotoolkit-1.5.0/src/AstroToolkit/Datapages.py
+drwxrwxrwx   0        0        0        0 2024-05-31 11:22:24.655705 astrotoolkit-1.5.0/src/AstroToolkit/Examples/
+-rw-rw-rw-   0        0        0     2666 2024-05-30 01:12:51.000000 astrotoolkit-1.5.0/src/AstroToolkit/Examples/datapage.py
+-rw-rw-rw-   0        0        0      367 2024-05-31 10:30:32.000000 astrotoolkit-1.5.0/src/AstroToolkit/Examples/hrd.py
+-rw-rw-rw-   0        0        0     1490 2024-05-31 02:03:24.000000 astrotoolkit-1.5.0/src/AstroToolkit/Examples/image.py
+-rw-rw-rw-   0        0        0      444 2024-05-31 02:03:12.000000 astrotoolkit-1.5.0/src/AstroToolkit/Examples/lightcurve.py
+-rw-rw-rw-   0        0        0      573 2024-05-31 10:41:22.000000 astrotoolkit-1.5.0/src/AstroToolkit/Examples/localfiles.py
+-rw-rw-rw-   0        0        0      323 2024-05-31 10:27:55.000000 astrotoolkit-1.5.0/src/AstroToolkit/Examples/sed.py
+-rw-rw-rw-   0        0        0      313 2024-05-31 10:20:02.000000 astrotoolkit-1.5.0/src/AstroToolkit/Examples/spectrum.py
+-rw-rw-rw-   0        0        0      449 2024-05-31 11:12:44.000000 astrotoolkit-1.5.0/src/AstroToolkit/Examples/timeseries.py
+drwxrwxrwx   0        0        0        0 2024-05-31 11:22:24.657706 astrotoolkit-1.5.0/src/AstroToolkit/FileHandling/
+-rw-rw-rw-   0        0        0      602 2024-05-22 16:08:46.000000 astrotoolkit-1.5.0/src/AstroToolkit/FileHandling/file_naming.py
+-rw-rw-rw-   0        0        0    10841 2024-05-22 16:17:49.000000 astrotoolkit-1.5.0/src/AstroToolkit/FileHandling/file_reading.py
+-rw-rw-rw-   0        0        0     6216 2024-05-22 16:18:27.000000 astrotoolkit-1.5.0/src/AstroToolkit/FileHandling/file_writing.py
+drwxrwxrwx   0        0        0        0 2024-05-31 11:22:24.657706 astrotoolkit-1.5.0/src/AstroToolkit/Input/
+-rw-rw-rw-   0        0        0    24436 2024-05-31 00:51:32.000000 astrotoolkit-1.5.0/src/AstroToolkit/Input/input_validation.py
+drwxrwxrwx   0        0        0        0 2024-05-31 11:22:24.661734 astrotoolkit-1.5.0/src/AstroToolkit/Misc/
+-rw-rw-rw-   0        0        0      485 2024-05-23 22:35:50.000000 astrotoolkit-1.5.0/src/AstroToolkit/Misc/coordinate_conversions.py
+-rw-rw-rw-   0        0        0     1071 2024-05-23 22:06:16.000000 astrotoolkit-1.5.0/src/AstroToolkit/Misc/fitsfiles.py
+-rw-rw-rw-   0        0        0     3682 2024-05-31 10:48:39.000000 astrotoolkit-1.5.0/src/AstroToolkit/Misc/gridsetup.py
+-rw-rw-rw-   0        0        0     1950 2024-05-23 22:21:31.000000 astrotoolkit-1.5.0/src/AstroToolkit/Misc/identifier_generation.py
+-rw-rw-rw-   0        0        0     5262 2024-05-23 23:54:34.000000 astrotoolkit-1.5.0/src/AstroToolkit/Misc/pmcorrection.py
+-rw-rw-rw-   0        0        0     2230 2024-05-23 23:53:18.000000 astrotoolkit-1.5.0/src/AstroToolkit/Misc/search.py
+drwxrwxrwx   0        0        0        0 2024-05-31 11:22:24.666729 astrotoolkit-1.5.0/src/AstroToolkit/Plotting/
+-rw-rw-rw-   0        0        0  1224000 2024-01-11 16:40:26.000000 astrotoolkit-1.5.0/src/AstroToolkit/Plotting/backdrop_hrd_allmags.fits
+-rw-rw-rw-   0        0        0     4209 2024-05-30 00:49:01.000000 astrotoolkit-1.5.0/src/AstroToolkit/Plotting/hrdplotting.py
+-rw-rw-rw-   0        0        0     4067 2024-05-31 01:11:09.000000 astrotoolkit-1.5.0/src/AstroToolkit/Plotting/imageplotting.py
+-rw-rw-rw-   0        0        0     5133 2024-05-26 20:36:23.000000 astrotoolkit-1.5.0/src/AstroToolkit/Plotting/lightcurveplotting.py
+-rw-rw-rw-   0        0        0     4439 2024-05-31 10:12:30.000000 astrotoolkit-1.5.0/src/AstroToolkit/Plotting/plotmap.py
+-rw-rw-rw-   0        0        0     3050 2024-05-29 17:25:56.000000 astrotoolkit-1.5.0/src/AstroToolkit/Plotting/sedplotting.py
+-rw-rw-rw-   0        0        0     3989 2024-05-22 12:51:38.000000 astrotoolkit-1.5.0/src/AstroToolkit/Plotting/spectrumplotting.py
+drwxrwxrwx   0        0        0        0 2024-05-31 11:22:24.667731 astrotoolkit-1.5.0/src/AstroToolkit/Timeseries/
+-rw-rw-rw-   0        0        0     4246 2024-05-28 16:18:21.000000 astrotoolkit-1.5.0/src/AstroToolkit/Timeseries/lomb_scargle.py
+-rw-rw-rw-   0        0        0     1113 2024-05-21 15:50:52.000000 astrotoolkit-1.5.0/src/AstroToolkit/Timeseries/timeseries_formatting.py
+-rw-rw-rw-   0        0        0    12135 2024-05-31 10:24:36.000000 astrotoolkit-1.5.0/src/AstroToolkit/Tools.py
+drwxrwxrwx   0        0        0        0 2024-05-31 11:22:24.668730 astrotoolkit-1.5.0/src/AstroToolkit.egg-info/
+-rw-rw-rw-   0        0        0    41557 2024-05-31 11:22:24.000000 astrotoolkit-1.5.0/src/AstroToolkit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2037 2024-05-31 11:22:24.000000 astrotoolkit-1.5.0/src/AstroToolkit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-31 11:22:24.000000 astrotoolkit-1.5.0/src/AstroToolkit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      188 2024-05-31 11:22:24.000000 astrotoolkit-1.5.0/src/AstroToolkit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-05-31 11:22:24.000000 astrotoolkit-1.5.0/src/AstroToolkit.egg-info/top_level.txt
```

### Comparing `astrotoolkit-1.4.2/pyproject.toml` & `astrotoolkit-1.5.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools]
 include-package-data = true
 
 [project]
 name = "AstroToolkit"
-version = "1.4.2"
+version = "1.5.0"
 authors = [
   { name="Ethan Moorfield", email="ethan.moorfield@hotmail.co.uk"},
 ]
 description = "A package for the gathering and plotting of astronomical data."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
@@ -24,15 +24,14 @@
     "bokeh==3.4.1",
     "cmasher==1.8.0",
     "matplotlib==3.8.4",
     "importlib_resources==6.4.0",
     "numpy==1.26.4",
     "pandas==2.2.2",
     "Requests==2.31.0",
-    "selenium==4.17.2",
     "beautifulsoup4==4.12.3",
     "scipy==1.13.0",
 ]
 
 [project.urls]
 Homepage = "https://github.com/WD-planets/AstroToolkit"
-Issues = "https://github.com/WD-planets/AstroToolkit/issues"
+Issues = "https://github.com/WD-planets/AstroToolkit/issues"
```

### Comparing `astrotoolkit-1.4.2/src/AstroToolkit/Plotting/backdrop_hrd_allmags.fits` & `astrotoolkit-1.5.0/src/AstroToolkit/Plotting/backdrop_hrd_allmags.fits`

 * *Files identical despite different names*

