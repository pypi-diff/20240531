# Comparing `tmp/gis-conflation-toolchain-0.7.1.tar.gz` & `tmp/gis_conflation_toolchain-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gis-conflation-toolchain-0.7.1.tar", last modified: Thu Jun  1 03:56:34 2023, max compression
+gzip compressed data, was "gis_conflation_toolchain-0.7.2.tar", last modified: Thu May 30 23:25:09 2024, max compression
```

## Comparing `gis-conflation-toolchain-0.7.1.tar` & `gis_conflation_toolchain-0.7.2.tar`

### file list

```diff
@@ -1,41 +1,39 @@
-drwxrwxr-x   0 fititnt   (1000) fititnt   (1000)        0 2023-06-01 03:56:34.955835 gis-conflation-toolchain-0.7.1/
--rw-rw-r--   0 fititnt   (1000) fititnt   (1000)    34522 2023-05-06 01:44:35.000000 gis-conflation-toolchain-0.7.1/LICENSE
--rw-rw-r--   0 fititnt   (1000) fititnt   (1000)     3173 2023-06-01 03:56:34.955835 gis-conflation-toolchain-0.7.1/PKG-INFO
--rw-rw-r--   0 fititnt   (1000) fititnt   (1000)     2486 2023-06-01 03:52:52.000000 gis-conflation-toolchain-0.7.1/README.md
--rw-rw-r--   0 fititnt   (1000) fititnt   (1000)      104 2023-05-06 19:31:41.000000 gis-conflation-toolchain-0.7.1/pyproject.toml
--rw-rw-r--   0 fititnt   (1000) fititnt   (1000)     1739 2023-06-01 03:56:34.955835 gis-conflation-toolchain-0.7.1/setup.cfg
-drwxrwxr-x   0 fititnt   (1000) fititnt   (1000)        0 2023-06-01 03:56:34.951835 gis-conflation-toolchain-0.7.1/src/
-drwxrwxr-x   0 fititnt   (1000) fititnt   (1000)        0 2023-06-01 03:56:34.951835 gis-conflation-toolchain-0.7.1/src/csv2excel/
--rw-rw-r--   0 fititnt   (1000) fititnt   (1000)        0 2023-04-25 07:23:36.000000 gis-conflation-toolchain-0.7.1/src/csv2excel/__init__.py
--rw-rw-r--   0 fititnt   (1000) fititnt   (1000)     5490 2023-04-26 12:06:05.000000 gis-conflation-toolchain-0.7.1/src/csv2excel/csv2excel.py
-drwxrwxr-x   0 fititnt   (1000) fititnt   (1000)        0 2023-06-01 03:56:34.951835 gis-conflation-toolchain-0.7.1/src/csv2geojson/
--rw-rw-r--   0 fititnt   (1000) fititnt   (1000)        0 2023-04-25 07:17:51.000000 gis-conflation-toolchain-0.7.1/src/csv2geojson/__init__.py
--rw-rw-r--   0 fititnt   (1000) fititnt   (1000)    26048 2023-05-09 03:45:20.000000 gis-conflation-toolchain-0.7.1/src/csv2geojson/csv2geojson.py
-drwxrwxr-x   0 fititnt   (1000) fititnt   (1000)        0 2023-06-01 03:56:34.951835 gis-conflation-toolchain-0.7.1/src/geojsondiff/
--rw-rw-r--   0 fititnt   (1000) fititnt   (1000)      168 2023-04-25 05:57:16.000000 gis-conflation-toolchain-0.7.1/src/geojsondiff/__init__.py
--rwxrwxr-x   0 fititnt   (1000) fititnt   (1000)    44861 2023-05-07 23:02:01.000000 gis-conflation-toolchain-0.7.1/src/geojsondiff/geojsondiff.py
-drwxrwxr-x   0 fititnt   (1000) fititnt   (1000)        0 2023-06-01 03:56:34.955835 gis-conflation-toolchain-0.7.1/src/gis_conflation_toolchain.egg-info/
--rw-rw-r--   0 fititnt   (1000) fititnt   (1000)     3173 2023-06-01 03:56:34.000000 gis-conflation-toolchain-0.7.1/src/gis_conflation_toolchain.egg-info/PKG-INFO
--rw-rw-r--   0 fititnt   (1000) fititnt   (1000)     1016 2023-06-01 03:56:34.000000 gis-conflation-toolchain-0.7.1/src/gis_conflation_toolchain.egg-info/SOURCES.txt
--rw-rw-r--   0 fititnt   (1000) fititnt   (1000)        1 2023-06-01 03:56:34.000000 gis-conflation-toolchain-0.7.1/src/gis_conflation_toolchain.egg-info/dependency_links.txt
--rw-rw-r--   0 fititnt   (1000) fititnt   (1000)      828 2023-06-01 03:56:34.000000 gis-conflation-toolchain-0.7.1/src/gis_conflation_toolchain.egg-info/entry_points.txt
--rw-rw-r--   0 fititnt   (1000) fititnt   (1000)       56 2023-06-01 03:56:34.000000 gis-conflation-toolchain-0.7.1/src/gis_conflation_toolchain.egg-info/requires.txt
--rw-rw-r--   0 fititnt   (1000) fititnt   (1000)       48 2023-06-01 03:56:34.000000 gis-conflation-toolchain-0.7.1/src/gis_conflation_toolchain.egg-info/top_level.txt
-drwxrwxr-x   0 fititnt   (1000) fititnt   (1000)        0 2023-06-01 03:56:34.955835 gis-conflation-toolchain-0.7.1/src/gisconflation/
--rw-rw-r--   0 fititnt   (1000) fititnt   (1000)        0 2023-04-25 09:07:58.000000 gis-conflation-toolchain-0.7.1/src/gisconflation/__init__.py
--rw-rw-r--   0 fititnt   (1000) fititnt   (1000)    24308 2023-05-06 22:34:03.000000 gis-conflation-toolchain-0.7.1/src/gisconflation/csv2gecodedcsv.py
--rw-rw-r--   0 fititnt   (1000) fititnt   (1000)    14609 2023-05-09 05:18:51.000000 gis-conflation-toolchain-0.7.1/src/gisconflation/csvedit.py
--rw-rw-r--   0 fititnt   (1000) fititnt   (1000)    10344 2023-05-08 21:49:46.000000 gis-conflation-toolchain-0.7.1/src/gisconflation/dictionarybuilder.py
--rw-rw-r--   0 fititnt   (1000) fititnt   (1000)     5727 2023-05-08 21:50:20.000000 gis-conflation-toolchain-0.7.1/src/gisconflation/dictionarymerger.py
--rwxrwxr-x   0 fititnt   (1000) fititnt   (1000)     7111 2023-06-01 03:54:51.000000 gis-conflation-toolchain-0.7.1/src/gisconflation/geojsonconcat.py
--rwxrwxr-x   0 fititnt   (1000) fititnt   (1000)    10629 2023-05-07 01:45:11.000000 gis-conflation-toolchain-0.7.1/src/gisconflation/geojsonedit.py
--rwxrwxr-x   0 fititnt   (1000) fititnt   (1000)    14364 2023-06-01 02:16:30.000000 gis-conflation-toolchain-0.7.1/src/gisconflation/geojsonmerger.py
--rw-rw-r--   0 fititnt   (1000) fititnt   (1000)     6639 2023-05-07 00:35:41.000000 gis-conflation-toolchain-0.7.1/src/gisconflation/json2csv.py
-drwxrwxr-x   0 fititnt   (1000) fititnt   (1000)        0 2023-06-01 03:56:34.955835 gis-conflation-toolchain-0.7.1/src/gisconflation/lib/
--rw-rw-r--   0 fititnt   (1000) fititnt   (1000)        0 2023-04-29 17:52:00.000000 gis-conflation-toolchain-0.7.1/src/gisconflation/lib/__init__.py
--rw-rw-r--   0 fititnt   (1000) fititnt   (1000)      503 2023-04-29 18:03:53.000000 gis-conflation-toolchain-0.7.1/src/gisconflation/lib/language.py
--rw-rw-r--   0 fititnt   (1000) fititnt   (1000)     2511 2023-04-28 09:55:54.000000 gis-conflation-toolchain-0.7.1/src/gisconflation/osmf2geojson.py
--rwxrwxr-x   0 fititnt   (1000) fititnt   (1000)     5820 2023-05-08 01:21:04.000000 gis-conflation-toolchain-0.7.1/src/gisconflation/overpassql2osmf.py
--rw-rw-r--   0 fititnt   (1000) fititnt   (1000)     8661 2023-05-06 22:48:52.000000 gis-conflation-toolchain-0.7.1/src/gisconflation/util.py
-drwxrwxr-x   0 fititnt   (1000) fititnt   (1000)        0 2023-06-01 03:56:34.955835 gis-conflation-toolchain-0.7.1/tests/
--rw-rw-r--   0 fititnt   (1000) fititnt   (1000)      580 2023-04-25 08:13:46.000000 gis-conflation-toolchain-0.7.1/tests/test_main.py
+drwxrwxr-x   0 fititnt   (1000) fititnt   (1000)        0 2024-05-30 23:25:09.739396 gis_conflation_toolchain-0.7.2/
+-rw-rw-r--   0 fititnt   (1000) fititnt   (1000)    34522 2023-05-06 01:44:35.000000 gis_conflation_toolchain-0.7.2/LICENSE
+-rw-r--r--   0 fititnt   (1000) fititnt   (1000)     3311 2024-05-30 23:25:09.739396 gis_conflation_toolchain-0.7.2/PKG-INFO
+-rw-rw-r--   0 fititnt   (1000) fititnt   (1000)     2484 2023-06-01 03:59:50.000000 gis_conflation_toolchain-0.7.2/README.md
+-rw-rw-r--   0 fititnt   (1000) fititnt   (1000)      104 2023-05-06 19:31:41.000000 gis_conflation_toolchain-0.7.2/pyproject.toml
+-rw-rw-r--   0 fititnt   (1000) fititnt   (1000)     1741 2024-05-30 23:25:09.739396 gis_conflation_toolchain-0.7.2/setup.cfg
+drwxrwxr-x   0 fititnt   (1000) fititnt   (1000)        0 2024-05-30 23:25:09.739396 gis_conflation_toolchain-0.7.2/src/
+drwxrwxr-x   0 fititnt   (1000) fititnt   (1000)        0 2024-05-30 23:25:09.739396 gis_conflation_toolchain-0.7.2/src/csv2excel/
+-rw-rw-r--   0 fititnt   (1000) fititnt   (1000)        0 2023-04-25 07:23:36.000000 gis_conflation_toolchain-0.7.2/src/csv2excel/__init__.py
+-rw-rw-r--   0 fititnt   (1000) fititnt   (1000)     5490 2023-04-26 12:06:05.000000 gis_conflation_toolchain-0.7.2/src/csv2excel/csv2excel.py
+drwxrwxr-x   0 fititnt   (1000) fititnt   (1000)        0 2024-05-30 23:25:09.739396 gis_conflation_toolchain-0.7.2/src/csv2geojson/
+-rw-rw-r--   0 fititnt   (1000) fititnt   (1000)        0 2023-04-25 07:17:51.000000 gis_conflation_toolchain-0.7.2/src/csv2geojson/__init__.py
+-rw-rw-r--   0 fititnt   (1000) fititnt   (1000)    40130 2024-05-30 22:54:11.000000 gis_conflation_toolchain-0.7.2/src/csv2geojson/csv2geojson.py
+drwxrwxr-x   0 fititnt   (1000) fititnt   (1000)        0 2024-05-30 23:25:09.739396 gis_conflation_toolchain-0.7.2/src/gis_conflation_toolchain.egg-info/
+-rw-r--r--   0 fititnt   (1000) fititnt   (1000)     3311 2024-05-30 23:25:09.000000 gis_conflation_toolchain-0.7.2/src/gis_conflation_toolchain.egg-info/PKG-INFO
+-rw-rw-r--   0 fititnt   (1000) fititnt   (1000)      990 2024-05-30 23:25:09.000000 gis_conflation_toolchain-0.7.2/src/gis_conflation_toolchain.egg-info/SOURCES.txt
+-rw-rw-r--   0 fititnt   (1000) fititnt   (1000)        1 2024-05-30 23:25:09.000000 gis_conflation_toolchain-0.7.2/src/gis_conflation_toolchain.egg-info/dependency_links.txt
+-rw-rw-r--   0 fititnt   (1000) fititnt   (1000)      830 2024-05-30 23:25:09.000000 gis_conflation_toolchain-0.7.2/src/gis_conflation_toolchain.egg-info/entry_points.txt
+-rw-rw-r--   0 fititnt   (1000) fititnt   (1000)       56 2024-05-30 23:25:09.000000 gis_conflation_toolchain-0.7.2/src/gis_conflation_toolchain.egg-info/requires.txt
+-rw-rw-r--   0 fititnt   (1000) fititnt   (1000)       36 2024-05-30 23:25:09.000000 gis_conflation_toolchain-0.7.2/src/gis_conflation_toolchain.egg-info/top_level.txt
+drwxrwxr-x   0 fititnt   (1000) fititnt   (1000)        0 2024-05-30 23:25:09.739396 gis_conflation_toolchain-0.7.2/src/gisconflation/
+-rw-rw-r--   0 fititnt   (1000) fititnt   (1000)        0 2023-04-25 09:07:58.000000 gis_conflation_toolchain-0.7.2/src/gisconflation/__init__.py
+-rw-rw-r--   0 fititnt   (1000) fititnt   (1000)    24308 2023-05-06 22:34:03.000000 gis_conflation_toolchain-0.7.2/src/gisconflation/csv2gecodedcsv.py
+-rw-rw-r--   0 fititnt   (1000) fititnt   (1000)    16044 2024-05-29 18:14:24.000000 gis_conflation_toolchain-0.7.2/src/gisconflation/csvedit.py
+-rw-rw-r--   0 fititnt   (1000) fititnt   (1000)    10344 2023-05-08 21:49:46.000000 gis_conflation_toolchain-0.7.2/src/gisconflation/dictionarybuilder.py
+-rw-rw-r--   0 fititnt   (1000) fititnt   (1000)     5727 2023-05-08 21:50:20.000000 gis_conflation_toolchain-0.7.2/src/gisconflation/dictionarymerger.py
+-rwxrwxr-x   0 fititnt   (1000) fititnt   (1000)     7111 2023-06-01 22:54:35.000000 gis_conflation_toolchain-0.7.2/src/gisconflation/geojsonconcat.py
+-rwxrwxr-x   0 fititnt   (1000) fititnt   (1000)    45337 2023-06-03 07:08:13.000000 gis_conflation_toolchain-0.7.2/src/gisconflation/geojsondiff.py
+-rwxrwxr-x   0 fititnt   (1000) fititnt   (1000)    10629 2023-05-07 01:45:11.000000 gis_conflation_toolchain-0.7.2/src/gisconflation/geojsonedit.py
+-rwxrwxr-x   0 fititnt   (1000) fititnt   (1000)    14364 2023-06-01 02:16:30.000000 gis_conflation_toolchain-0.7.2/src/gisconflation/geojsonmerger.py
+-rw-rw-r--   0 fititnt   (1000) fititnt   (1000)     6639 2023-05-07 00:35:41.000000 gis_conflation_toolchain-0.7.2/src/gisconflation/json2csv.py
+drwxrwxr-x   0 fititnt   (1000) fititnt   (1000)        0 2024-05-30 23:25:09.739396 gis_conflation_toolchain-0.7.2/src/gisconflation/lib/
+-rw-rw-r--   0 fititnt   (1000) fititnt   (1000)        0 2023-04-29 17:52:00.000000 gis_conflation_toolchain-0.7.2/src/gisconflation/lib/__init__.py
+-rw-rw-r--   0 fititnt   (1000) fititnt   (1000)      503 2023-04-29 18:03:53.000000 gis_conflation_toolchain-0.7.2/src/gisconflation/lib/language.py
+-rw-rw-r--   0 fititnt   (1000) fititnt   (1000)     2511 2023-04-28 09:55:54.000000 gis_conflation_toolchain-0.7.2/src/gisconflation/osmf2geojson.py
+-rwxrwxr-x   0 fititnt   (1000) fititnt   (1000)     5820 2023-05-08 01:21:04.000000 gis_conflation_toolchain-0.7.2/src/gisconflation/overpassql2osmf.py
+-rw-rw-r--   0 fititnt   (1000) fititnt   (1000)     8661 2023-05-06 22:48:52.000000 gis_conflation_toolchain-0.7.2/src/gisconflation/util.py
+drwxrwxr-x   0 fititnt   (1000) fititnt   (1000)        0 2024-05-30 23:25:09.739396 gis_conflation_toolchain-0.7.2/tests/
+-rw-rw-r--   0 fititnt   (1000) fititnt   (1000)      580 2023-04-25 08:13:46.000000 gis_conflation_toolchain-0.7.2/tests/test_main.py
```

### Comparing `gis-conflation-toolchain-0.7.1/LICENSE` & `gis_conflation_toolchain-0.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `gis-conflation-toolchain-0.7.1/PKG-INFO` & `gis_conflation_toolchain-0.7.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,33 +1,36 @@
 Metadata-Version: 2.1
 Name: gis-conflation-toolchain
-Version: 0.7.1
+Version: 0.7.2
 Summary: gis-conflation-toolchain
 Home-page: https://github.com/fititnt/spatial-data-conflation-open-toolchain
 Author: Emerson Rocha
 Author-email: rocha@ieee.org
 Project-URL: Bug Tracker, https://github.com/fititnt/spatial-data-conflation-open-toolchain/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Operating System :: OS Independent
 Classifier: Typing :: Typed
 Classifier: Topic :: Utilities
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Provides-Extra: extras
 License-File: LICENSE
+Requires-Dist: shapely
+Requires-Dist: haversine
+Requires-Dist: pandas
+Requires-Dist: levenshtein
+Provides-Extra: extras
+Requires-Dist: geocoder; extra == "extras"
 
 # spatial-data-conflation-open-toolchain
-**[EARLY DRAFT] Open, free to use, toolchain for geospatial data conflation. Command-line interface for file manipulation.** _See geojson-diff.py from <https://github.com/fititnt/openstreetmap-vs-dados-abertos-brasil>._
-
 [![GitHub](https://img.shields.io/badge/GitHub-fititnt%20spatial--data--conflation--open--toolchain-lightgrey?logo=github&style=social[fititnt/geojson-diff] "GitHub")](https://github.com/fititnt/spatial-data-conflation-open-toolchain)
-
 [![Pypi: gis-conflation-toolchain](https://img.shields.io/badge/python%20pypi-gis--conflation--toolchain-brightgreen[Python] 
  "Pypi: gis-conflation-toolchain")](https://pypi.org/project/gis-conflation-toolchain)
 
+**[EARLY DRAFT] Open, free to use, toolchain for geospatial data conflation. Command-line interface for file manipulation.** _See geojson-diff.py from <https://github.com/fititnt/openstreetmap-vs-dados-abertos-brasil>._
 
 ## Installing
 
 ```bash
 pip install --upgrade gis-conflation-toolchain
 ```
```

### Comparing `gis-conflation-toolchain-0.7.1/README.md` & `gis_conflation_toolchain-0.7.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 # spatial-data-conflation-open-toolchain
-**[EARLY DRAFT] Open, free to use, toolchain for geospatial data conflation. Command-line interface for file manipulation.** _See geojson-diff.py from <https://github.com/fititnt/openstreetmap-vs-dados-abertos-brasil>._
-
 [![GitHub](https://img.shields.io/badge/GitHub-fititnt%20spatial--data--conflation--open--toolchain-lightgrey?logo=github&style=social[fititnt/geojson-diff] "GitHub")](https://github.com/fititnt/spatial-data-conflation-open-toolchain)
-
 [![Pypi: gis-conflation-toolchain](https://img.shields.io/badge/python%20pypi-gis--conflation--toolchain-brightgreen[Python] 
  "Pypi: gis-conflation-toolchain")](https://pypi.org/project/gis-conflation-toolchain)
 
+**[EARLY DRAFT] Open, free to use, toolchain for geospatial data conflation. Command-line interface for file manipulation.** _See geojson-diff.py from <https://github.com/fititnt/openstreetmap-vs-dados-abertos-brasil>._
 
 ## Installing
 
 ```bash
 pip install --upgrade gis-conflation-toolchain
 ```
```

### Comparing `gis-conflation-toolchain-0.7.1/setup.cfg` & `gis_conflation_toolchain-0.7.2/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = gis-conflation-toolchain
-version = 0.7.1
+version = 0.7.2
 author = Emerson Rocha
 author_email = rocha@ieee.org
 description = gis-conflation-toolchain
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/fititnt/spatial-data-conflation-open-toolchain
 project_urls = 
@@ -39,15 +39,15 @@
 	csv2excel = csv2excel.csv2excel:exec_from_console_scripts
 	csv2gecodedcsv = gisconflation.csv2gecodedcsv:exec_from_console_scripts
 	csv2geojson = csv2geojson.csv2geojson:exec_from_console_scripts
 	csvedit = gisconflation.csvedit:exec_from_console_scripts
 	dictionarybuilder = gisconflation.dictionarybuilder:exec_from_console_scripts
 	dictionarymerger = gisconflation.dictionarymerger:exec_from_console_scripts
 	geojsonconcat = gisconflation.geojsonconcat:exec_from_console_scripts
-	geojsondiff = geojsondiff.geojsondiff:exec_from_console_scripts
+	geojsondiff = gisconflation.geojsondiff:exec_from_console_scripts
 	geojsonedit = gisconflation.geojsonedit:exec_from_console_scripts
 	geojsonmerger = gisconflation.geojsonmerger:exec_from_console_scripts
 	json2csv = gisconflation.json2csv:exec_from_console_scripts
 	overpassql2osmf = gisconflation.overpassql2osmf:exec_from_console_scripts
 
 [egg_info]
 tag_build =
```

### Comparing `gis-conflation-toolchain-0.7.1/src/csv2excel/csv2excel.py` & `gis_conflation_toolchain-0.7.2/src/csv2excel/csv2excel.py`

 * *Files identical despite different names*

### Comparing `gis-conflation-toolchain-0.7.1/src/csv2geojson/csv2geojson.py` & `gis_conflation_toolchain-0.7.2/src/gisconflation/csv2gecodedcsv.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,51 +1,60 @@
 #!/usr/bin/env python3
 # ==============================================================================
 #
-#          FILE:  csv2geojson.py
+#          FILE:  csv2gecodedcsv.py
 #
-#         USAGE:  ./scripts/csv2geojson.py
-#                 ./scripts/csv2geojson.py --help
+#         USAGE:  ./scripts/csv2gecodedcsv.py
+#                 ./scripts/csv2gecodedcsv.py --help
 #
-#   DESCRIPTION:  ---
+#   DESCRIPTION:  [DRAFT, not usable yet]
 #
 #       OPTIONS:  ---
 #
 #  REQUIREMENTS:  - python3
 #          BUGS:  ---
 #         NOTES:  ---
 #       AUTHORS:  Emerson Rocha <rocha[at]ieee.org>
 # COLLABORATORS:  ---
 #
 #       COMPANY:  EticaAI
-#       LICENSE:  Public Domain dedication or Zero-Clause BSD
-#                 SPDX-License-Identifier: Unlicense OR 0BSD
-#       VERSION:  v1.1.0
-#       CREATED:  2023-04-11 18:13 BRT
-#      REVISION:  2023-04-20 01:20 BRT v1.1 --contain-and-in
+#       LICENSE:  GNU Affero General Public License v3.0 or later
+#                 SPDX-License-Identifier: AGPL-3.0-or-later
+#       VERSION:  v0.5.0
+#       CREATED:  2023-05-06 16:54 BRT started, based on csv2geojson.py
+#      REVISION:  --
 # ==============================================================================
 
 
 # import geopandas
 # import os
 import argparse
 import csv
 import json
 import re
 import sys
 import string
 
 from gisconflation.util import parse_argument_values
 
+try:
+    import geocoder
+except ImportError:
+    raise ImportError("Dependency not found. Please: pip install geocoder")
 
-__VERSION__ = "1.1.0"
-PROGRAM = "csv2geojson"
+# https://geocoder.readthedocs.io/providers/OpenStreetMap.html
+print(geocoder.osm('Mountain View, CA'))
+
+# geocode 'New York city' --provider osm --out geojson | jq .
+
+__VERSION__ = "0.5.0"
+PROGRAM = "csv2gecodedcsv"
 DESCRIPTION = """
 ------------------------------------------------------------------------------
-CSV to GeoJSON
+[DRAFT, not usable yet] CSV to Geocoded CSV
 
 ------------------------------------------------------------------------------
 """.format(
     PROGRAM, __VERSION__
 )
 
 # https://www.rfc-editor.org/rfc/rfc7946
@@ -332,24 +341,14 @@
             "(Locale BR, 'logradouro') ",
             dest="value_name_street_br",
             nargs="?",
             type=lambda x: x.split("|"),
             default=None,
         )
 
-        custom_group = parser.add_argument_group("Other")
-
-        custom_group.add_argument(
-            "--preprocessor-item-custom-inep",
-            help="Custom feature not yet documented",
-            dest="prepitem_custom_inep",
-            required=False,
-            nargs="?",
-        )
-
         return parser.parse_args()
 
     def execute_cli(self, pyargs, stdin=STDIN, stdout=sys.stdout, stderr=sys.stderr):
         # input_file = STDIN if pyargs.input == "-" else pyargs.input
 
         _contain_or = {}
         _contain_and = {}
@@ -411,20 +410,14 @@
                     row,
                     line_num=line_num,
                     cast_integer=pyargs.cast_integer,
                     cast_float=pyargs.cast_float,
                     ignore_warnings=pyargs.ignore_warnings,
                 )
 
-                if pyargs.prepitem_custom_inep:
-                    formated_row = _zzz_format_custom_inep(
-                        formated_row, pyargs.prepitem_custom_inep
-                    )
-                    # raise ValueError(pyargs.prepitem_custom_inep)
-
                 row_v2 = row_item_column_add(
                     formated_row,
                     column_copy=pyargs.column_copy,
                     ignore_warnings=pyargs.ignore_warnings,
                 )
                 row_v3 = row_item_values(
                     row_v2,
@@ -738,40 +731,27 @@
 
 
 def _zzz_format_name_place_br(value: str):
     if not value or not isinstance(value, str):
         return value
 
     term = string.capwords(value.strip())
-    term2 = re.sub("\\s\\s+", " ", term)
+    term2 = re.sub("\s\s+", " ", term)
 
     # @TODO deal with Do Da De
 
     return term2
 
 
 def _zzz_format_name_street_br(value: str):
     if not value or not isinstance(value, str):
         return value
 
     term = string.capwords(value.strip())
-    term2 = re.sub("\\s\\s+", " ", term)
-
-    # @TODO deal with Do Da De
-    # @TODO deal with abbreviations
-
-    return term2
-
-
-def _zzz_format_name_school_br(value: str):
-    if not value or not isinstance(value, str):
-        return value
-
-    term = string.capwords(value.strip())
-    term2 = re.sub("\\s\\s+", " ", term)
+    term2 = re.sub("\s\s+", " ", term)
 
     # @TODO deal with Do Da De
     # @TODO deal with abbreviations
 
     return term2
 
 
@@ -795,59 +775,14 @@
         return "+55 " + _regiao + " " + _num_loc_p1 + " " + _num_loc_p2
 
     # if value.isnumeric():
     #     if len(value) == 8:
     #         return re.sub(r"(\d{5})(\d{3})", r"\1-\2", value)
     return False
 
-escolas_dict = {
-    'ESC EST ENS FUN': 'Escola Estadual Ensino Fundamental'
-}
-
-# pytest -vv src/csv2geojson/csv2geojson.py --doctest-modules
-def _zzz_format_custom_inep(item: dict, source_column: str = "Endereço") -> dict:
-    """_summary_
-
-    Args:
-        item (dict): _description_
-        source_column (str, optional): _description_. Defaults to "Endereço".
-
-    Returns:
-        dict: _description_
-
-    >>> d1 = "RUA LEONILLA HANSEN, 182 JOANETA. 95166-000 Picada Café - RS."
-    >>> item1 = {"Endereço": d1}
-    >>> r1 = _zzz_format_custom_inep(item1)
-    >>> r1['addr:city']
-    'Picada'
-    >>> r1['addr:postcode']
-    '95166-000'
-    """
-    result = item
-    addr_raw = item[source_column]
-
-    logradouro_arr = []
-    parts = addr_raw.split(" ")
-    while len(parts) > 0:
-        token = parts.pop(0)
-        # @TODO do the regex
-        if len(token) == 9 and token[5] == "-":
-            result["addr:postcode"] = token
-            result["addr:city"] = parts.pop(0)
-            break
-
-        logradouro_arr.append(token)
-
-    result["__addr:street"] = _zzz_format_name_street_br(
-        " ".join(logradouro_arr).strip(".")
-    )
-    # result["__addr:street"] = result["__addr:street"]p('.')
-
-    return result
-
 
 def exec_from_console_scripts():
     main = Cli()
     args = main.make_args()
     main.execute_cli(args)
```

### Comparing `gis-conflation-toolchain-0.7.1/src/geojsondiff/geojsondiff.py` & `gis_conflation_toolchain-0.7.2/src/gisconflation/geojsondiff.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python3
 # ==============================================================================
 #
-#          FILE:  geojson-diff.py
+#          FILE:  geojsondiff.py
 #
-#         USAGE:  ./scripts/geojson-diff.py
-#                 ./scripts/geojson-diff.py --help
+#         USAGE:  geojsondiff --help
+#                 ./src/gisconflation/geojsondiff.py --help
 #
 #   DESCRIPTION:  ---
 #
 #       OPTIONS:  ---
 #
 #  REQUIREMENTS:  - python3
 #                   - haversine (pip install haversine)
@@ -17,20 +17,21 @@
 #         NOTES:  ---
 #       AUTHORS:  Emerson Rocha <rocha[at]ieee.org>
 # COLLABORATORS:  ---
 #
 #       COMPANY:  EticaAI
 #       LICENSE:  Public Domain dedication or Zero-Clause BSD
 #                 SPDX-License-Identifier: Unlicense OR 0BSD
-#       VERSION:  v0.6.1
+#       VERSION:  v0.6.2
 #       CREATED:  2023-04-16 22:36 BRT
 #      REVISION:  2023-04-17 02:32 BRT v0.4.0 accept Overpas GeoJSON flavor
 #                 2023-04-18 00:25 BRT v0.5.0 supports Polygon (not just Point)
 #                 2023-04-19 21:52 BRT v0.6.0 draft of diff GeoJSON and JOSM
 #                 2023-04-25 03:58 BRT v0.6.1 miggrade as pip package
+#                 2023-06-03 03:16 BRT v0.6.2 moved to ./src/gisconflation
 # ==============================================================================
 
 import argparse
 import csv
 import dataclasses
 import json
 import sys
@@ -42,24 +43,25 @@
 # from shapely.geometry import Polygon, Point
 from shapely.geometry import Polygon
 from xml.sax.saxutils import escape
 
 from gisconflation.util import LevenshteinHelper
 
 
-__VERSION__ = "0.6.1"
+__VERSION__ = "0.6.2"
+# VERSION = "0.6.2"
 
 PROGRAM = "geojsondiff"
 DESCRIPTION = """
 ------------------------------------------------------------------------------
-GeoJSON++ diff
+GeoJSON++ diff v{1}
 
 ------------------------------------------------------------------------------
 """.format(
-    __file__
+    __file__, __VERSION__
 )
 
 # https://www.rfc-editor.org/rfc/rfc7946
 # The GeoJSON Format
 # https://www.rfc-editor.org/rfc/rfc8142
 # GeoJSON Text Sequences
 
@@ -159,14 +161,24 @@
             nargs="?",
         )
 
         pivot = parser.add_argument_group(
             "Parameters used to know how to conflate A and B"
         )
 
+        parser.add_argument(
+            "--conflation-strategy",
+            help="Conflation strategy.",
+            dest="strategy",
+            default="distance",
+            required=False,
+            choices=["distance", "addr"],
+            nargs="?",
+        )
+
         pivot.add_argument(
             "--tolerate-distance",
             help="Typical maximum distance for features match if not "
             "exact same point. In meters. Default to 100",
             dest="tdist",
             default="100",
             required=False,
@@ -346,14 +358,15 @@
             prefilter_a_contain=parse_argument_values(pyargs.prefilter_a_contain),
             prefilter_b_contain=parse_argument_values(pyargs.prefilter_b_contain),
         )
 
         geodiff = GeojsonCompare(
             pyargs.geodataset_a,
             pyargs.geodataset_b,
+            pyargs.strategy,
             crules,
             cprefilters=cprefilters,
             cfilters=cfilters,
             logger=logger,
         )
 
         if pyargs.outosc:
@@ -656,19 +669,21 @@
     @TODO optimize for very large files
     """
 
     def __init__(
         self,
         geodataset_a: str,
         geodataset_b: str,
+        strategy: str,
         crules: Type["ConflationRules"],
         cprefilters: Type["ConflationPrefilters"],
         cfilters: Type["ConflationFilters"],
-        logger,
+        logger=None,
     ) -> None:
+        self.strategy = strategy
         self.distance_okay = crules.distance_okay
         self.crules = crules
         self.cfilters = cfilters
         self.cprefilters = cprefilters
         self.a_is_osm = None
         self.b_is_osm = None
```

### Comparing `gis-conflation-toolchain-0.7.1/src/gis_conflation_toolchain.egg-info/PKG-INFO` & `gis_conflation_toolchain-0.7.2/src/gis_conflation_toolchain.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,33 +1,36 @@
 Metadata-Version: 2.1
 Name: gis-conflation-toolchain
-Version: 0.7.1
+Version: 0.7.2
 Summary: gis-conflation-toolchain
 Home-page: https://github.com/fititnt/spatial-data-conflation-open-toolchain
 Author: Emerson Rocha
 Author-email: rocha@ieee.org
 Project-URL: Bug Tracker, https://github.com/fititnt/spatial-data-conflation-open-toolchain/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Operating System :: OS Independent
 Classifier: Typing :: Typed
 Classifier: Topic :: Utilities
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Provides-Extra: extras
 License-File: LICENSE
+Requires-Dist: shapely
+Requires-Dist: haversine
+Requires-Dist: pandas
+Requires-Dist: levenshtein
+Provides-Extra: extras
+Requires-Dist: geocoder; extra == "extras"
 
 # spatial-data-conflation-open-toolchain
-**[EARLY DRAFT] Open, free to use, toolchain for geospatial data conflation. Command-line interface for file manipulation.** _See geojson-diff.py from <https://github.com/fititnt/openstreetmap-vs-dados-abertos-brasil>._
-
 [![GitHub](https://img.shields.io/badge/GitHub-fititnt%20spatial--data--conflation--open--toolchain-lightgrey?logo=github&style=social[fititnt/geojson-diff] "GitHub")](https://github.com/fititnt/spatial-data-conflation-open-toolchain)
-
 [![Pypi: gis-conflation-toolchain](https://img.shields.io/badge/python%20pypi-gis--conflation--toolchain-brightgreen[Python] 
  "Pypi: gis-conflation-toolchain")](https://pypi.org/project/gis-conflation-toolchain)
 
+**[EARLY DRAFT] Open, free to use, toolchain for geospatial data conflation. Command-line interface for file manipulation.** _See geojson-diff.py from <https://github.com/fititnt/openstreetmap-vs-dados-abertos-brasil>._
 
 ## Installing
 
 ```bash
 pip install --upgrade gis-conflation-toolchain
 ```
```

### Comparing `gis-conflation-toolchain-0.7.1/src/gis_conflation_toolchain.egg-info/SOURCES.txt` & `gis_conflation_toolchain-0.7.2/src/gis_conflation_toolchain.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -2,28 +2,27 @@
 README.md
 pyproject.toml
 setup.cfg
 src/csv2excel/__init__.py
 src/csv2excel/csv2excel.py
 src/csv2geojson/__init__.py
 src/csv2geojson/csv2geojson.py
-src/geojsondiff/__init__.py
-src/geojsondiff/geojsondiff.py
 src/gis_conflation_toolchain.egg-info/PKG-INFO
 src/gis_conflation_toolchain.egg-info/SOURCES.txt
 src/gis_conflation_toolchain.egg-info/dependency_links.txt
 src/gis_conflation_toolchain.egg-info/entry_points.txt
 src/gis_conflation_toolchain.egg-info/requires.txt
 src/gis_conflation_toolchain.egg-info/top_level.txt
 src/gisconflation/__init__.py
 src/gisconflation/csv2gecodedcsv.py
 src/gisconflation/csvedit.py
 src/gisconflation/dictionarybuilder.py
 src/gisconflation/dictionarymerger.py
 src/gisconflation/geojsonconcat.py
+src/gisconflation/geojsondiff.py
 src/gisconflation/geojsonedit.py
 src/gisconflation/geojsonmerger.py
 src/gisconflation/json2csv.py
 src/gisconflation/osmf2geojson.py
 src/gisconflation/overpassql2osmf.py
 src/gisconflation/util.py
 src/gisconflation/lib/__init__.py
```

### Comparing `gis-conflation-toolchain-0.7.1/src/gis_conflation_toolchain.egg-info/entry_points.txt` & `gis_conflation_toolchain-0.7.2/src/gis_conflation_toolchain.egg-info/entry_points.txt`

 * *Files 2% similar despite different names*

```diff
@@ -2,12 +2,12 @@
 csv2excel = csv2excel.csv2excel:exec_from_console_scripts
 csv2gecodedcsv = gisconflation.csv2gecodedcsv:exec_from_console_scripts
 csv2geojson = csv2geojson.csv2geojson:exec_from_console_scripts
 csvedit = gisconflation.csvedit:exec_from_console_scripts
 dictionarybuilder = gisconflation.dictionarybuilder:exec_from_console_scripts
 dictionarymerger = gisconflation.dictionarymerger:exec_from_console_scripts
 geojsonconcat = gisconflation.geojsonconcat:exec_from_console_scripts
-geojsondiff = geojsondiff.geojsondiff:exec_from_console_scripts
+geojsondiff = gisconflation.geojsondiff:exec_from_console_scripts
 geojsonedit = gisconflation.geojsonedit:exec_from_console_scripts
 geojsonmerger = gisconflation.geojsonmerger:exec_from_console_scripts
 json2csv = gisconflation.json2csv:exec_from_console_scripts
 overpassql2osmf = gisconflation.overpassql2osmf:exec_from_console_scripts
```

### Comparing `gis-conflation-toolchain-0.7.1/src/gisconflation/csvedit.py` & `gis_conflation_toolchain-0.7.2/src/gisconflation/csvedit.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,19 +25,21 @@
 # ==============================================================================
 
 
 # import geopandas
 # import os
 import argparse
 import csv
+
 # import json
 import re
 import sys
 
 from gisconflation.util import parse_argument_values
+
 # import string
 
 # from gisconflation.util import parse_argument_values
 
 # try:
 #     import geocoder
 # except ImportError:
@@ -198,29 +200,39 @@
             help="The output delimiter",
             dest="out_delimiter",
             default=",",
             required=False,
             nargs="?",
         )
 
-        filter_group = parser.add_argument_group(
-            "Filter rows"
-        )
+        filter_group = parser.add_argument_group("Filter rows")
 
         filter_group.add_argument(
             "--contain-and",
             help="If defined, only results that match all clauses"
             " will appear on output. Accept multiple values."
             "--contain-and=tag1=value1 --contain-and=tag2=value2",
             dest="contain_and",
             nargs="?",
             action="append",
         )
 
         filter_group.add_argument(
+            "--contain-and-regex",
+            help="If defined, only results that match all clauses"
+            " will appear on output. Accept multiple values."
+            "Syntax is python regex. https://docs.python.org/3/library/re.html"
+            "Example: "
+            "--contain-and-regex='name|||hospital.+'",
+            dest="contain_and_regex",
+            nargs="?",
+            action="append",
+        )
+
+        filter_group.add_argument(
             "--filter-contain",
             help="Filter one or more fields for contain a string"
             "Use '|||' to divide the field and the string. "
             "Accept multiple values. "
             "Example: "
             "--filter-contain='name|||hospital'",
             dest="filter_contain",
@@ -367,15 +379,16 @@
                 if item:
                     if item.find("="):
                         _key, _val = item.split("=")
                         _contain_and[_key] = _val
                     else:
                         _contain_and[_key] = True
 
-        filter_contain=parse_argument_values(pyargs.filter_contain)
+        filter_contain = parse_argument_values(pyargs.filter_contain)
+        contain_and_regex = parse_argument_values(pyargs.contain_and_regex)
 
         # @TODO stdin does not yet allow non UTF8 customization (will pass as it is)
         # @see https://stackoverflow.com/questions/5004687
         with open(pyargs.input, "r", encoding=pyargs.in_encoding) if len(
             pyargs.input
         ) > 1 else sys.stdin as csvfile:
             if pyargs.in_fieldnames:
@@ -395,20 +408,23 @@
 
             _fieldnames = firstline.keys()
             writer = csv.DictWriter(
                 sys.stdout, fieldnames=_fieldnames, delimiter=pyargs.out_delimiter
             )
 
             writer.writeheader()
-            writer.writerow(firstline)
+            # writer.writerow(firstline)
 
-            # @TODO bug with both conditions must be fixed.
+            reader2 = list(reader)
+            reader2.insert(0, firstline)
 
-            for row in reader:
+            # @TODO bug with both conditions must be fixed.
 
+            # for row in reader:
+            for row in reader2:
                 # @TODO move out of here
                 if _contain_and:
                     _count = len(_contain_and.keys())
 
                     for _key, _val in _contain_and.items():
                         if _key not in row:
                             raise SyntaxError(f"key {_key} not in {row}")
@@ -416,33 +432,54 @@
                         # print(item)
                         if _val is not True and _val != row[_key]:
                             continue
                         _count -= 1
 
                     if _count > 0:
                         continue
-                
+
                 if filter_contain:
                     # raise ValueError(filter_contain)
                     _count2 = len(filter_contain.keys())
 
                     for _key, _val in filter_contain.items():
-                        _val = _val.lower()
+                        if not isinstance(_val, bool):
+                            _val = _val.lower()
 
                         if _key not in row:
                             raise SyntaxError(f"key {_key} not in {row}")
                             # return False
 
                         if _val is not True and row[_key].lower().find(_val) == -1:
                             continue
                         _count2 -= 1
 
                     if _count2 > 0:
                         continue
 
+                if contain_and_regex:
+                    # raise ValueError(filter_contain)
+                    _count3 = len(contain_and_regex.keys())
+
+                    for _key, _regex in contain_and_regex.items():
+                        # _val = _val.lower()
+
+                        if _key not in row:
+                            raise SyntaxError(f"key {_key} not in {row}")
+                            # return False
+                        _result = re.match(_regex, row[_key])
+
+                        # if _val is not True and row[_key].lower().find(_val) == -1:
+                        if not _result:
+                            continue
+                        _count3 -= 1
+
+                    if _count3 > 0:
+                        continue
+
                 writer.writerow(row)
 
         return self.EXIT_OK
 
 
 def exec_from_console_scripts():
     main = Cli()
```

### Comparing `gis-conflation-toolchain-0.7.1/src/gisconflation/dictionarybuilder.py` & `gis_conflation_toolchain-0.7.2/src/gisconflation/dictionarybuilder.py`

 * *Files identical despite different names*

### Comparing `gis-conflation-toolchain-0.7.1/src/gisconflation/dictionarymerger.py` & `gis_conflation_toolchain-0.7.2/src/gisconflation/dictionarymerger.py`

 * *Files identical despite different names*

### Comparing `gis-conflation-toolchain-0.7.1/src/gisconflation/geojsonconcat.py` & `gis_conflation_toolchain-0.7.2/src/gisconflation/geojsonconcat.py`

 * *Files identical despite different names*

### Comparing `gis-conflation-toolchain-0.7.1/src/gisconflation/geojsonedit.py` & `gis_conflation_toolchain-0.7.2/src/gisconflation/geojsonedit.py`

 * *Files identical despite different names*

### Comparing `gis-conflation-toolchain-0.7.1/src/gisconflation/geojsonmerger.py` & `gis_conflation_toolchain-0.7.2/src/gisconflation/geojsonmerger.py`

 * *Files identical despite different names*

### Comparing `gis-conflation-toolchain-0.7.1/src/gisconflation/json2csv.py` & `gis_conflation_toolchain-0.7.2/src/gisconflation/json2csv.py`

 * *Files identical despite different names*

### Comparing `gis-conflation-toolchain-0.7.1/src/gisconflation/osmf2geojson.py` & `gis_conflation_toolchain-0.7.2/src/gisconflation/osmf2geojson.py`

 * *Files identical despite different names*

### Comparing `gis-conflation-toolchain-0.7.1/src/gisconflation/overpassql2osmf.py` & `gis_conflation_toolchain-0.7.2/src/gisconflation/overpassql2osmf.py`

 * *Files identical despite different names*

### Comparing `gis-conflation-toolchain-0.7.1/src/gisconflation/util.py` & `gis_conflation_toolchain-0.7.2/src/gisconflation/util.py`

 * *Files identical despite different names*

### Comparing `gis-conflation-toolchain-0.7.1/tests/test_main.py` & `gis_conflation_toolchain-0.7.2/tests/test_main.py`

 * *Files identical despite different names*

