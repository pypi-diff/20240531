# Comparing `tmp/niamoto-0.0.2a1.tar.gz` & `tmp/niamoto-0.0.3a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "niamoto-0.0.2a1.tar", max compression
+gzip compressed data, was "niamoto-0.0.3a1.tar", max compression
```

## Comparing `niamoto-0.0.2a1.tar` & `niamoto-0.0.3a1.tar`

### file list

```diff
@@ -1,60 +1,60 @@
--rw-r--r--   0        0        0    35149 2023-12-18 18:49:51.068568 niamoto-0.0.2a1/LICENSE
--rw-r--r--   0        0        0    12572 2024-04-29 09:35:50.501361 niamoto-0.0.2a1/README.md
--rw-r--r--   0        0        0     7608 2024-04-26 16:21:56.378658 niamoto-0.0.2a1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-12-18 18:47:14.899456 niamoto-0.0.2a1/src/niamoto/__init__.py
--rw-r--r--   0        0        0      176 2024-03-17 11:30:55.790624 niamoto-0.0.2a1/src/niamoto/api/__init__.py
--rw-r--r--   0        0        0      638 2024-04-29 08:55:57.427623 niamoto-0.0.2a1/src/niamoto/api/generator.py
--rw-r--r--   0        0        0     3404 2024-04-26 16:01:49.245020 niamoto-0.0.2a1/src/niamoto/api/importer.py
--rw-r--r--   0        0        0     2172 2024-04-26 16:01:49.248356 niamoto-0.0.2a1/src/niamoto/api/mapper.py
--rw-r--r--   0        0        0     2994 2024-04-29 08:38:58.672070 niamoto-0.0.2a1/src/niamoto/api/statistics.py
--rw-r--r--   0        0        0        0 2023-12-18 18:47:14.900005 niamoto-0.0.2a1/src/niamoto/cli/__init__.py
--rw-r--r--   0        0        0    23392 2024-04-29 08:55:57.428067 niamoto-0.0.2a1/src/niamoto/cli/commands.py
--rw-r--r--   0        0        0        0 2023-12-18 18:47:14.900231 niamoto-0.0.2a1/src/niamoto/common/__init__.py
--rw-r--r--   0        0        0     6722 2024-04-26 16:01:49.247937 niamoto-0.0.2a1/src/niamoto/common/config.py
--rw-r--r--   0        0        0     7679 2024-04-26 16:01:49.246735 niamoto-0.0.2a1/src/niamoto/common/database.py
--rw-r--r--   0        0        0     1419 2024-03-17 11:30:55.792426 niamoto-0.0.2a1/src/niamoto/common/environment.py
--rw-r--r--   0        0        0     1422 2024-03-17 11:30:55.791898 niamoto-0.0.2a1/src/niamoto/common/exceptions.py
--rw-r--r--   0        0        0        0 2024-03-14 20:33:15.957328 niamoto-0.0.2a1/src/niamoto/core/__init__.py
--rw-r--r--   0        0        0        0 2024-02-26 16:56:57.129500 niamoto-0.0.2a1/src/niamoto/core/components/__init__.py
--rw-r--r--   0        0        0        0 2024-02-26 16:56:57.125946 niamoto-0.0.2a1/src/niamoto/core/components/importers/__init__.py
--rw-r--r--   0        0        0     9811 2024-04-26 16:01:49.248390 niamoto-0.0.2a1/src/niamoto/core/components/importers/occurrences.py
--rw-r--r--   0        0        0     1608 2024-04-26 15:09:01.953631 niamoto-0.0.2a1/src/niamoto/core/components/importers/plots.py
--rw-r--r--   0        0        0     3900 2024-04-26 16:01:49.246868 niamoto-0.0.2a1/src/niamoto/core/components/importers/taxonomy.py
--rw-r--r--   0        0        0        0 2024-02-26 16:58:28.941202 niamoto-0.0.2a1/src/niamoto/core/components/mappers/__init__.py
--rw-r--r--   0        0        0    12822 2024-04-29 08:55:57.427862 niamoto-0.0.2a1/src/niamoto/core/components/mappers/mapping_manager.py
--rw-r--r--   0        0        0        0 2024-04-02 13:26:08.724363 niamoto-0.0.2a1/src/niamoto/core/components/statistics/__init__.py
--rw-r--r--   0        0        0     2312 2024-04-29 08:45:10.824735 niamoto-0.0.2a1/src/niamoto/core/components/statistics/plot_stats_calculator.py
--rw-r--r--   0        0        0    11234 2024-04-29 08:55:57.428251 niamoto-0.0.2a1/src/niamoto/core/components/statistics/statistics_calculator.py
--rw-r--r--   0        0        0     3637 2024-04-26 16:01:49.245261 niamoto-0.0.2a1/src/niamoto/core/components/statistics/taxonomy_stats_calculator.py
--rw-r--r--   0        0        0      107 2024-04-29 08:58:01.228690 niamoto-0.0.2a1/src/niamoto/core/models/__init__.py
--rw-r--r--   0        0        0     3094 2024-04-29 08:55:57.427544 niamoto-0.0.2a1/src/niamoto/core/models/models.py
--rw-r--r--   0        0        0        0 2024-02-26 09:35:39.100463 niamoto-0.0.2a1/src/niamoto/core/repositories/__init__.py
--rw-r--r--   0        0        0     2729 2024-04-26 16:16:39.970756 niamoto-0.0.2a1/src/niamoto/core/repositories/niamoto_repository.py
--rw-r--r--   0        0        0        0 2024-02-26 16:59:11.340255 niamoto-0.0.2a1/src/niamoto/core/services/__init__.py
--rw-r--r--   0        0        0     1556 2024-03-22 10:17:01.014526 niamoto-0.0.2a1/src/niamoto/core/services/importer.py
--rw-r--r--   0        0        0     1083 2024-04-26 16:01:49.247159 niamoto-0.0.2a1/src/niamoto/core/services/mapper.py
--rw-r--r--   0        0        0    23730 2024-04-29 09:04:50.758432 niamoto-0.0.2a1/src/niamoto/core/services/processor.py
--rw-r--r--   0        0        0     1899 2024-04-26 16:01:49.245968 niamoto-0.0.2a1/src/niamoto/core/services/statistics.py
--rw-r--r--   0        0        0        0 2024-02-26 09:35:12.975166 niamoto-0.0.2a1/src/niamoto/core/utils/__init__.py
--rw-r--r--   0        0        0     1440 2024-04-26 16:01:49.176772 niamoto-0.0.2a1/src/niamoto/core/utils/csv_utils.py
--rw-r--r--   0        0        0      174 2024-03-17 09:40:18.006381 niamoto-0.0.2a1/src/niamoto/main.py
--rw-r--r--   0        0        0       78 2024-03-14 22:19:33.109529 niamoto-0.0.2a1/src/niamoto/publish/__init__.py
--rw-r--r--   0        0        0        0 2023-12-18 18:47:14.899932 niamoto-0.0.2a1/src/niamoto/publish/api_creator/__init__.py
--rw-r--r--   0        0        0       71 2024-03-14 21:27:58.003471 niamoto-0.0.2a1/src/niamoto/publish/static_site_generator/__init__.py
--rw-r--r--   0        0        0     5997 2024-04-29 09:12:19.969907 niamoto-0.0.2a1/src/niamoto/publish/static_site_generator/page_generator.py
--rw-r--r--   0        0        0     8892 2024-04-28 21:29:58.212701 niamoto-0.0.2a1/src/niamoto/publish/static_site_generator/static/js/index.js
--rw-r--r--   0        0        0   205488 2024-04-26 17:33:58.572179 niamoto-0.0.2a1/src/niamoto/publish/static_site_generator/static/js/vendor/chart/4.4.2_chart.js
--rw-r--r--   0        0        0   586923 2024-04-26 17:34:20.924377 niamoto-0.0.2a1/src/niamoto/publish/static_site_generator/static/js/vendor/d3/7.8.5_d3.js
--rw-r--r--   0        0        0   288580 2024-04-26 17:34:26.124154 niamoto-0.0.2a1/src/niamoto/publish/static_site_generator/static/js/vendor/jquery/3.6.0_jquery.js
--rw-r--r--   0        0        0    47635 2024-04-26 17:34:15.492610 niamoto-0.0.2a1/src/niamoto/publish/static_site_generator/static/js/vendor/justgage/1.6.1_justgage.js
--rw-r--r--   0        0        0    14806 2024-04-26 17:32:44.478066 niamoto-0.0.2a1/src/niamoto/publish/static_site_generator/static/js/vendor/leaflet/1.9.4_leaflet.css
--rw-r--r--   0        0        0   147552 2024-04-26 17:34:31.191623 niamoto-0.0.2a1/src/niamoto/publish/static_site_generator/static/js/vendor/leaflet/1.9.4_leaflet.js
--rw-r--r--   0        0        0     1259 2023-05-18 11:01:45.000000 niamoto-0.0.2a1/src/niamoto/publish/static_site_generator/static/js/vendor/leaflet/images/layers-2x.png
--rw-r--r--   0        0        0      696 2023-05-18 11:01:45.000000 niamoto-0.0.2a1/src/niamoto/publish/static_site_generator/static/js/vendor/leaflet/images/layers.png
--rw-r--r--   0        0        0     2464 2023-05-18 11:01:45.000000 niamoto-0.0.2a1/src/niamoto/publish/static_site_generator/static/js/vendor/leaflet/images/marker-icon-2x.png
--rw-r--r--   0        0        0     1466 2023-05-18 11:01:45.000000 niamoto-0.0.2a1/src/niamoto/publish/static_site_generator/static/js/vendor/leaflet/images/marker-icon.png
--rw-r--r--   0        0        0      618 2023-05-18 11:01:45.000000 niamoto-0.0.2a1/src/niamoto/publish/static_site_generator/static/js/vendor/leaflet/images/marker-shadow.png
--rw-r--r--   0        0        0   310628 2024-04-26 17:34:08.014141 niamoto-0.0.2a1/src/niamoto/publish/static_site_generator/static/js/vendor/raphael/2.3.0_raphael.js
--rw-r--r--   0        0        0  3642321 2024-04-26 17:26:39.465386 niamoto-0.0.2a1/src/niamoto/publish/static_site_generator/static/js/vendor/tailwindcss/2.2.19_dist_tailwind.css
--rw-r--r--   0        0        0     5514 2024-04-29 07:50:15.272656 niamoto-0.0.2a1/src/niamoto/publish/static_site_generator/templates/taxon_template.html
--rw-r--r--   0        0        0    14692 1970-01-01 00:00:00.000000 niamoto-0.0.2a1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-12-18 18:49:51.068568 niamoto-0.0.3a1/LICENSE
+-rw-r--r--   0        0        0    11283 2024-05-31 10:01:30.813822 niamoto-0.0.3a1/README.md
+-rw-r--r--   0        0        0     7698 2024-05-31 10:02:38.037014 niamoto-0.0.3a1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-12-18 18:47:14.899456 niamoto-0.0.3a1/src/niamoto/__init__.py
+-rw-r--r--   0        0        0      176 2024-03-17 11:30:55.790624 niamoto-0.0.3a1/src/niamoto/api/__init__.py
+-rw-r--r--   0        0        0     1633 2024-05-09 10:08:03.981764 niamoto-0.0.3a1/src/niamoto/api/generator.py
+-rw-r--r--   0        0        0     3828 2024-05-31 09:17:03.015413 niamoto-0.0.3a1/src/niamoto/api/importer.py
+-rw-r--r--   0        0        0     2389 2024-05-09 10:08:03.982562 niamoto-0.0.3a1/src/niamoto/api/mapper.py
+-rw-r--r--   0        0        0     4736 2024-05-09 10:08:03.981816 niamoto-0.0.3a1/src/niamoto/api/statistics.py
+-rw-r--r--   0        0        0        0 2023-12-18 18:47:14.900005 niamoto-0.0.3a1/src/niamoto/cli/__init__.py
+-rw-r--r--   0        0        0    30728 2024-05-31 10:07:56.569740 niamoto-0.0.3a1/src/niamoto/cli/commands.py
+-rw-r--r--   0        0        0        0 2023-12-18 18:47:14.900231 niamoto-0.0.3a1/src/niamoto/common/__init__.py
+-rw-r--r--   0        0        0     7835 2024-05-31 10:03:51.829555 niamoto-0.0.3a1/src/niamoto/common/config.py
+-rw-r--r--   0        0        0     7920 2024-05-09 09:20:29.453660 niamoto-0.0.3a1/src/niamoto/common/database.py
+-rw-r--r--   0        0        0     1990 2024-05-31 10:03:51.791151 niamoto-0.0.3a1/src/niamoto/common/environment.py
+-rw-r--r--   0        0        0     3274 2024-05-09 09:20:29.466938 niamoto-0.0.3a1/src/niamoto/common/exceptions.py
+-rw-r--r--   0        0        0        0 2024-03-14 20:33:15.957328 niamoto-0.0.3a1/src/niamoto/core/__init__.py
+-rw-r--r--   0        0        0        0 2024-02-26 16:56:57.129500 niamoto-0.0.3a1/src/niamoto/core/components/__init__.py
+-rw-r--r--   0        0        0        0 2024-02-26 16:56:57.125946 niamoto-0.0.3a1/src/niamoto/core/components/importers/__init__.py
+-rw-r--r--   0        0        0    10457 2024-05-31 10:03:51.828915 niamoto-0.0.3a1/src/niamoto/core/components/importers/occurrences.py
+-rw-r--r--   0        0        0     2094 2024-05-09 10:08:03.983376 niamoto-0.0.3a1/src/niamoto/core/components/importers/plots.py
+-rw-r--r--   0        0        0     5888 2024-05-09 10:08:03.982214 niamoto-0.0.3a1/src/niamoto/core/components/importers/taxonomy.py
+-rw-r--r--   0        0        0        0 2024-02-26 16:58:28.941202 niamoto-0.0.3a1/src/niamoto/core/components/mappers/__init__.py
+-rw-r--r--   0        0        0    16087 2024-05-31 10:03:51.829754 niamoto-0.0.3a1/src/niamoto/core/components/mappers/mapping_manager.py
+-rw-r--r--   0        0        0        0 2024-04-02 13:26:08.724363 niamoto-0.0.3a1/src/niamoto/core/components/statistics/__init__.py
+-rw-r--r--   0        0        0     3458 2024-05-09 10:08:03.983406 niamoto-0.0.3a1/src/niamoto/core/components/statistics/plot_stats_calculator.py
+-rw-r--r--   0        0        0    13312 2024-05-09 10:08:03.982456 niamoto-0.0.3a1/src/niamoto/core/components/statistics/statistics_calculator.py
+-rw-r--r--   0        0        0     5002 2024-05-09 10:08:03.981148 niamoto-0.0.3a1/src/niamoto/core/components/statistics/taxonomy_stats_calculator.py
+-rw-r--r--   0        0        0      107 2024-04-29 08:58:01.228690 niamoto-0.0.3a1/src/niamoto/core/models/__init__.py
+-rw-r--r--   0        0        0     4508 2024-05-09 10:08:03.980053 niamoto-0.0.3a1/src/niamoto/core/models/models.py
+-rw-r--r--   0        0        0        0 2024-02-26 09:35:39.100463 niamoto-0.0.3a1/src/niamoto/core/repositories/__init__.py
+-rw-r--r--   0        0        0     3250 2024-05-09 09:20:29.493819 niamoto-0.0.3a1/src/niamoto/core/repositories/niamoto_repository.py
+-rw-r--r--   0        0        0        0 2024-02-26 16:59:11.340255 niamoto-0.0.3a1/src/niamoto/core/services/__init__.py
+-rw-r--r--   0        0        0     2629 2024-05-09 10:08:03.983410 niamoto-0.0.3a1/src/niamoto/core/services/importer.py
+-rw-r--r--   0        0        0     2370 2024-05-09 10:08:03.983290 niamoto-0.0.3a1/src/niamoto/core/services/mapper.py
+-rw-r--r--   0        0        0    25820 2024-05-09 10:08:33.454541 niamoto-0.0.3a1/src/niamoto/core/services/processor.py
+-rw-r--r--   0        0        0     2689 2024-05-09 10:08:03.983209 niamoto-0.0.3a1/src/niamoto/core/services/statistics.py
+-rw-r--r--   0        0        0        0 2024-02-26 09:35:12.975166 niamoto-0.0.3a1/src/niamoto/core/utils/__init__.py
+-rw-r--r--   0        0        0     1444 2024-05-09 09:20:29.413414 niamoto-0.0.3a1/src/niamoto/core/utils/csv_utils.py
+-rw-r--r--   0        0        0      174 2024-03-17 09:40:18.006381 niamoto-0.0.3a1/src/niamoto/main.py
+-rw-r--r--   0        0        0       78 2024-03-14 22:19:33.109529 niamoto-0.0.3a1/src/niamoto/publish/__init__.py
+-rw-r--r--   0        0        0        0 2023-12-18 18:47:14.899932 niamoto-0.0.3a1/src/niamoto/publish/api_creator/__init__.py
+-rw-r--r--   0        0        0       71 2024-03-14 21:27:58.003471 niamoto-0.0.3a1/src/niamoto/publish/static_site_generator/__init__.py
+-rw-r--r--   0        0        0     6990 2024-05-31 08:51:11.178609 niamoto-0.0.3a1/src/niamoto/publish/static_site_generator/page_generator.py
+-rw-r--r--   0        0        0     8892 2024-04-28 21:29:58.212701 niamoto-0.0.3a1/src/niamoto/publish/static_site_generator/static/js/index.js
+-rw-r--r--   0        0        0   205488 2024-04-26 17:33:58.572179 niamoto-0.0.3a1/src/niamoto/publish/static_site_generator/static/js/vendor/chart/4.4.2_chart.js
+-rw-r--r--   0        0        0   586923 2024-04-26 17:34:20.924377 niamoto-0.0.3a1/src/niamoto/publish/static_site_generator/static/js/vendor/d3/7.8.5_d3.js
+-rw-r--r--   0        0        0   288580 2024-04-26 17:34:26.124154 niamoto-0.0.3a1/src/niamoto/publish/static_site_generator/static/js/vendor/jquery/3.6.0_jquery.js
+-rw-r--r--   0        0        0    47635 2024-04-26 17:34:15.492610 niamoto-0.0.3a1/src/niamoto/publish/static_site_generator/static/js/vendor/justgage/1.6.1_justgage.js
+-rw-r--r--   0        0        0    14806 2024-04-26 17:32:44.478066 niamoto-0.0.3a1/src/niamoto/publish/static_site_generator/static/js/vendor/leaflet/1.9.4_leaflet.css
+-rw-r--r--   0        0        0   147552 2024-04-26 17:34:31.191623 niamoto-0.0.3a1/src/niamoto/publish/static_site_generator/static/js/vendor/leaflet/1.9.4_leaflet.js
+-rw-r--r--   0        0        0     1259 2023-05-18 11:01:45.000000 niamoto-0.0.3a1/src/niamoto/publish/static_site_generator/static/js/vendor/leaflet/images/layers-2x.png
+-rw-r--r--   0        0        0      696 2023-05-18 11:01:45.000000 niamoto-0.0.3a1/src/niamoto/publish/static_site_generator/static/js/vendor/leaflet/images/layers.png
+-rw-r--r--   0        0        0     2464 2023-05-18 11:01:45.000000 niamoto-0.0.3a1/src/niamoto/publish/static_site_generator/static/js/vendor/leaflet/images/marker-icon-2x.png
+-rw-r--r--   0        0        0     1466 2023-05-18 11:01:45.000000 niamoto-0.0.3a1/src/niamoto/publish/static_site_generator/static/js/vendor/leaflet/images/marker-icon.png
+-rw-r--r--   0        0        0      618 2023-05-18 11:01:45.000000 niamoto-0.0.3a1/src/niamoto/publish/static_site_generator/static/js/vendor/leaflet/images/marker-shadow.png
+-rw-r--r--   0        0        0   310628 2024-04-26 17:34:08.014141 niamoto-0.0.3a1/src/niamoto/publish/static_site_generator/static/js/vendor/raphael/2.3.0_raphael.js
+-rw-r--r--   0        0        0  3642321 2024-04-26 17:26:39.465386 niamoto-0.0.3a1/src/niamoto/publish/static_site_generator/static/js/vendor/tailwindcss/2.2.19_dist_tailwind.css
+-rw-r--r--   0        0        0     5514 2024-04-29 07:50:15.272656 niamoto-0.0.3a1/src/niamoto/publish/static_site_generator/templates/taxon_template.html
+-rw-r--r--   0        0        0    13554 1970-01-01 00:00:00.000000 niamoto-0.0.3a1/PKG-INFO
```

### Comparing `niamoto-0.0.2a1/LICENSE` & `niamoto-0.0.3a1/LICENSE`

 * *Files identical despite different names*

### Comparing `niamoto-0.0.2a1/README.md` & `niamoto-0.0.3a1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -46,54 +46,45 @@
 
 ```
 niamoto init
 ```
 
 This command will create the default configuration necessary for Niamoto to operate. Use the `--reset` option to reset the environment if it already exists.
 
-## Available Commands
-
-| Command                 | Description                                                                                                             |
-|-------------------------|-------------------------------------------------------------------------------------------------------------------------|
-| init                    | Initialize or reset the Niamoto environment.                                                                            |
-| import-taxonomy         | Import taxonomy data from a CSV file into the database.                                                                 |
-| import-plots            | Import plot data from a GeoPackage file into the plot_ref table.                                                        |
-| import-occurrences      | Import occurrence data from a CSV file, analyze it to update the 'mapping' table, and link occurrences to their taxons. |
-| import-occurrence-plots | Import occurrence-plot links from a CSV file.                                                                           |
-| generate-mapping        | Generate a mapping from a CSV file based on the specified grouping criteria.                                            |
-| calculate-statistics    | Calculate statistics based on the mapping file specified in the configuration.                                          |
-| generate-static-site    | Generate static web pages for each taxon in the database.                                                               |
-| generate-taxonomy-stats | Generate a taxonomy tree, calculate statistics, and write the taxon table from a CSV file.                              |
-
 
 ## Development Environment Configuration
 
 To set up a development environment for Niamoto, you must have `Poetry` installed on your system. Poetry is a dependency management and packaging tool for Python.
 
 1. **Poetry Installation**:
-   To install Poetry, run the following command:
-   ```bash
-   curl -sSL https://raw.githubusercontent.com/python-poetry/poetry/master/get-poetry.py | python -
-   ```
 
+  To install Poetry, run the following command:
+
+  ```bash
+  curl -sSL https://raw.githubusercontent.com/python-poetry/poetry/master/get-poetry.py | python -
+  ```
 
 2. **Clone the Niamoto repository**:
+
   Clone the Niamoto repository on your system using `git`:
+
   ```bash
   git clone https://github.com/niamoto/niamoto.git
   ```
 
 3. **Configure the development environment with Poetry**:
+
   Move into the cloned directory and install the dependencies with Poetry:
   ```bash
   cd niamoto
   poetry install
   ```
 
 4. **Activate the virtual environment**:
+
   Activate the virtual environment created by Poetry:
   ```bash
   poetry shell
   ```
 
 5. **Editable Installation**:
 
@@ -127,63 +118,73 @@
 **Command:**
 ```bash
 $ niamoto init [--reset]
 ```
 **Explanation:**
 Initializes or resets the Niamoto environment. Use the `--reset` option to reset the environment if it already exists, clearing all data and configurations to start fresh.
 
-#### 2. Import Taxonomy Data
+#### 2. Import All Data
+**Command:**
+```bash
+$ niamoto import-all
+```
+
+**Explanation:**
+Imports all data from CSV files and GeoPackage files into the database. This command is a shortcut to import taxonomy, plot, occurrences, and occurrence-plot links data in one go.
+Assuming the following files are present in the current source directory and specified in the configuration file
+
+#### 3. Import Taxonomy Data
 **Command:**
 ```bash
 $ niamoto import-taxonomy <csvfile> [--ranks <ranks>]
 ```
 **Explanation:**
 Imports taxonomy data from a specified CSV file. The `--ranks` option allows specifying the order of taxonomic ranks as they appear in the CSV file.
 
-#### 3. Import Plot Data
+#### 4. Import Plot Data
 **Command:**
 ```bash
 $ niamoto import-plots <gpkg_file>
 ```
 **Explanation:**
 Imports plot data from a GeoPackage file into the database, which should contain plot geometries and associated attributes.
 
-#### 4. Import Occurrences Data
+#### 5. Import Occurrences Data
 **Command:**
 ```bash
 $ niamoto import-occurrences <csvfile> --taxon-id-column <column_name>
 ```
 **Explanation:**
 Imports occurrences data from a CSV file. The `--taxon-id-column` option specifies the CSV column containing the taxon IDs needed to link occurrences to taxons.
 
-#### 5. Import Occurrence-Plot Links
+#### 6. Import Occurrence-Plot Links
 **Command:**
 ```bash
 $ niamoto import-occurrence-plots <csvfile>
 ```
 **Explanation:**
 Imports links between occurrences and plots from a CSV file, establishing relational data within the database.
 
-#### 6. Generate Mapping
+#### 7. Generate Mapping
 **Command:**
 ```bash
 $ niamoto generate-mapping --data-source <csv_file> --mapping-group <group> [--reference-table-name <table_name> --reference-data-path <path>]
 ```
 **Explanation:**
 Generates mappings from a CSV file based on specified grouping criteria. Optional parameters allow linking to reference data for enhanced mapping accuracy.
 
-#### 7. Calculate Statistics
+#### 8. Calculate Statistics
 **Command:**
 ```bash
 $ niamoto calculate-statistics [--mapping-group <group> --csv-file <file>]
 ```
 **Explanation:**
 Calculates statistics based on the provided mapping file and optional group or CSV file specifics.
 
-#### 8. Generate Static Site
+#### 9. Generate Static Site
 **Command:**
 ```bash
 $ niamoto generate-static-site
 ```
 **Explanation:**
 Generates a static website for each taxon in the database, providing a visual and informational representation of taxonomic data.
 
@@ -217,14 +218,15 @@
   - `chart_type`: The type of chart to generate for the bins (e.g., "bar").
   - `chart_options`: Specific options for the bin chart (e.g., "title", "color").
 - `is_identifier`: Indicates whether the field is an identifier (boolean value).
 - `display_order`: The display order of the field in the interface.
 
 #### Special Fields
 Some fields may have specific configurations depending on their `target_field` and `field_type`:
+
 - **Calculated field** (e.g., total number of occurrences):
   - `target_field`: null
   - `field_type`: "INTEGER"
   - `transformations`: Must contain a "count" type transformation
 - **Boolean field** (e.g., occurrence on a particular substrate):
   - `target_field`: The name of the boolean field in the occurrences table
   - `field_type`: "BOOLEAN"
@@ -238,14 +240,15 @@
 
 #### 1. **JSON Style Notation:**
 
 ```yaml
 transformations:
   - {"name": "max", "chart_type": "gauge", "chart_options": {"max": 40, "title": "Maximum", "label": "units"}}
 ```
+
 #### 1. **Standard YAML Style Notation:**
 This format will display both YAML notations under a single Markdown box, keeping the explanation compact and the code examples clear and easy to compare.
 
 ```yaml
 transformations:
   - name: max
     chart_type: gauge
```

### Comparing `niamoto-0.0.2a1/pyproject.toml` & `niamoto-0.0.3a1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "niamoto"
-version = "0.0.2a1"
+version = "0.0.3a1"
 description = ""
 authors = ["Julien Barbe <julien.barbe@me.com>"]
 readme = "README.md"
 license= "GPL-3.0-or-later"
 packages = [{include = "niamoto", from = "src"}]
 homepage = "https://github.com/niamoto/niamoto"
 repository= "https://github.com/niamoto/niamoto"
@@ -136,14 +136,17 @@
 pyproj = "^3.6.1"
 
 # rjsmin - JavaScript minifier written in Python.
 rjsmin = "^1.2.2"
 
 # prompt-toolkit - Library for building powerful interactive command line applications in Python.
 prompt-toolkit = "^3.0.43"
+sphinxcontrib-napoleon = "^0.7"
+myst-parser = "^3.0.1"
+sphinx-markdown-builder = "^0.6.6"
 
 
 [tool.poetry.group.dev.dependencies]
 # -------------
 # Testing Tools
 # -------------
```

### Comparing `niamoto-0.0.2a1/src/niamoto/api/importer.py` & `niamoto-0.0.3a1/src/niamoto/api/importer.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,51 +1,62 @@
 from loguru import logger
 from typing import Any, Tuple
 from niamoto.core.services.importer import ImporterService
 from niamoto.common.config import Config
 
 
 class ApiImporter:
+    """
+    A class used to import data for the Niamoto project.
+
+    Attributes:
+        config (Config): The configuration settings for the Niamoto project.
+        db_path (str): The path to the database.
+    """
+
     def __init__(self) -> None:
         """
-        Initialize the ImportAPI with the database path.
-
-        Parameters:
-        - db_path (str): The path to the database.
+        Initializes the ApiImporter with the database path.
         """
         self.config = Config()
         self.db_path = self.config.get("database", "path")
 
-    def import_taxononomy(self, csvfile: str, ranks: Tuple[str, ...]) -> Any:
+    def import_taxonomy(self, csvfile: str, ranks: Tuple[str, ...]) -> Any:
         """
-        Import taxonomu data using DataImportService.
+        Imports taxonomy data using DataImportService.
 
-        Parameters:
+        Args:
             csvfile (str): Path to the CSV file to be imported.
-            ranks (tuple): The ranks to be imported.
+            ranks (Tuple[str, ...]): The ranks to be imported.
+
+        Returns:
+            Any: The results of the import operation.
         """
         try:
             # Initialize the data import service
             data_import_service = ImporterService(self.db_path)
 
             # Call the service to import the taxonomy
             import_tax_results = data_import_service.import_taxonomy(csvfile, ranks)
 
             # Confirmation message
             return import_tax_results
 
         except Exception as e:
-            logger.exception(f"Error importing 'occurrences' data: {e}")
+            logger.error(f"Error during taxonomy data import: {e}")
 
     def import_plots(self, gpkg_path: str) -> Any:
         """
-        Import plot data from the provided GeoPackage file path.
+        Imports plot data from the provided GeoPackage file path.
 
-        Parameters:
-        - gpkg_path (str): Path to the GeoPackage file to be imported.
+        Args:
+            gpkg_path (str): Path to the GeoPackage file to be imported.
+
+        Returns:
+            Any: The results of the import operation.
         """
         try:
             # Initialize the data import service
             data_import_service = ImporterService(self.db_path)
 
             # Call the service to import the plots
             import_plot_results = data_import_service.import_plots(gpkg_path)
@@ -54,49 +65,55 @@
             return import_plot_results
 
         except Exception as e:
             logger.error(f"Error during plot data import: {e}")
 
     def import_occurrences(self, csvfile: str, taxon_id_column: str) -> Any:
         """
-        Import occurrences data using DataImportService.
+        Imports occurrences data using DataImportService.
 
-        Parameters:
-            taxon_id_column: Name of the column in the CSV that corresponds to the taxon ID.
+        Args:
             csvfile (str): Path to the CSV file to be imported.
+            taxon_id_column (str): Name of the column in the CSV that corresponds to the taxon ID.
+
+        Returns:
+            Any: The results of the import operation.
         """
         try:
             # Initialize the data import service
             data_import_service = ImporterService(self.db_path)
 
             # Call the service to import the occurrences
             import_occ_result = data_import_service.import_occurrences(
                 csvfile, taxon_id_column
             )
 
             # Confirmation message
             return import_occ_result
 
         except Exception as e:
-            logger.exception(f"Error importing 'occurrences' data: {e}")
+            logger.error(f"Error during occurrences data import: {e}")
 
     def import_occurrence_plot_links(self, csvfile: str) -> Any:
         """
-        Import occurrence-plot links from a CSV file.
+        Imports occurrence-plot links from a CSV file.
+
+        Args:
+            csvfile (str): Path to the CSV file to be imported.
 
-        Parameters:
-        - csvfile (str): Path to the CSV file to be imported.
+        Returns:
+            Any: The results of the import operation.
         """
         try:
             # Initialize the data import service
             data_import_service = ImporterService(self.db_path)
 
             # Call the service to import the occurrence-plot links
             import_opl_results = data_import_service.import_occurrence_plot_links(
                 csvfile
             )
 
             # Confirmation message
             return import_opl_results
 
         except Exception as e:
-            logger.exception(f"Error importing 'occurrence-plot' links: {e}")
+            logger.error(f"Error during occurrence-plot data import: {e}")
```

### Comparing `niamoto-0.0.2a1/src/niamoto/api/mapper.py` & `niamoto-0.0.3a1/src/niamoto/api/mapper.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,43 +3,47 @@
 from loguru import logger
 
 from niamoto.common.config import Config
 from niamoto.core.services.mapper import MapperService
 
 
 class ApiMapper:
+    """
+    A class used to map data for the Niamoto project.
+
+    Attributes:
+        config (Config): The configuration settings for the Niamoto project.
+        db_path (str): The path to the database.
+    """
+
     def __init__(self) -> None:
         """
-        Initialize the ImportAPI with the database path.
-
-        Parameters:
-        - db_path (str): The path to the database.
+        Initializes the ApiMapper with the database path.
         """
         self.config = Config()
         self.db_path = self.config.get("database", "path")
 
     def generate_mapping_from_csv(
         self,
         csvfile: str,
         group_by: str,
         reference_table_name: Optional[str],
         reference_data_path: Optional[str],
     ) -> Any:
         """
-        Generate mapping from the CSV file.
+        Generates a mapping from a CSV file.
 
         Args:
-            csvfile: Path to the CSV file to generate mapping from.
-            group_by: The type of grouping to generate the mapping for (e.g., taxon, plot, commune).
-            reference_table_name: The name of the reference table in the database.
-            reference_data_path: The path to the reference table file (e.g., GeoPackage).
+            csvfile (str): Path to the CSV file to generate mapping from.
+            group_by (str): The type of grouping to generate the mapping for (e.g., taxon, plot, commune).
+            reference_table_name (Optional[str]): The name of the reference table in the database.
+            reference_data_path (Optional[str]): The path to the reference table file (e.g., GeoPackage).
 
         Returns:
-            str: Confirmation message.
-
+            Any: Confirmation message.
         """
         try:
             # Initialize the data import service
             mapper_service = MapperService(self.db_path)
 
             # Call the service to import the taxonomy
             mapper_service.generate_mapping(
@@ -49,22 +53,21 @@
             return "Mapping generated"
 
         except Exception as e:
             logger.exception(f"Error importing 'occurrences' data: {e}")
 
     def add_new_mapping(self, field: str) -> Any:
         """
-        Add new mapping to the database.
+        Adds a new mapping to the database.
 
         Args:
-            field: New field to be added to the mapping.
+            field (str): New field to be added to the mapping.
 
         Returns:
-            str:
-
+            Any: Confirmation message.
         """
         try:
             # Initialize the data import service
             mapper_service = MapperService(self.db_path)
 
             # Call the service to import the taxonomy
             mapper_service.add_mapping(field)
```

### Comparing `niamoto-0.0.2a1/src/niamoto/cli/commands.py` & `niamoto-0.0.3a1/src/niamoto/cli/commands.py`

 * *Files 15% similar despite different names*

```diff
@@ -9,25 +9,27 @@
 """
 
 import os
 import time
 from typing import Optional, List
 
 import click
+import duckdb
 from loguru import logger
 from rich.console import Console
 from rich.progress import track
 from rich.table import Table
 from sqlalchemy import asc, text
 
 from niamoto.api import StaticContentGenerator, ApiImporter, ApiMapper
 from niamoto.api.statistics import ApiStatistics
 from niamoto.common.config import Config
+from niamoto.common.database import Database
 from niamoto.common.environment import Environment
-from niamoto.core.models import TaxonRef
+from niamoto.core.models import TaxonRef, Base
 from niamoto.core.repositories.niamoto_repository import NiamotoRepository
 from niamoto.core.services.mapper import MapperService
 
 
 class RichCLI(click.Group):
     def list_commands(self, ctx: click.Context) -> List[str]:
         """
@@ -166,28 +168,28 @@
     """
     console = Console()
     niamoto_home = Config.get_niamoto_home()
     config_path = os.path.join(niamoto_home, "config.yml")
 
     if os.path.exists(config_path):
         config_manager = Config(config_path)
-        environment = Environment(config_manager.config)
+        environment = Environment(config_manager)
 
         if reset:
             click.secho("Resetting the Niamoto environment...", fg="red")
             environment.reset()
         else:
             click.secho(
-                "Niamoto environment already exists. Use --reset to remove existing files",
+                "Niamoto environment already exists. Use --reset to remove existing files.",
                 fg="yellow",
             )
             return
     else:
         config_manager = Config(config_path, create_default=True)
-        environment = Environment(config_manager.config)
+        environment = Environment(config_manager)
         environment.initialize()
 
     console.print("🌱 Niamoto initialized.", style="italic green")
     console.rule()
 
     list_commands(cli)
 
@@ -235,174 +237,346 @@
         table.add_row(command.name, description)
 
     console.print("Available Commands:", style="italic underline")
     console.print(table)
 
 
 @cli.command(name="import-taxonomy")
-@click.argument("csvfile")
+@click.argument("csvfile", required=False)
 @click.option("--ranks", help="Comma-separated list of ranks in the hierarchy.")
 def import_taxonomy(csvfile: str, ranks: str) -> None:
     """
     Import taxonomy data from a CSV file into the database.
 
     This command reads taxonomic data from the specified CSV file and imports it into the database.
     The CSV file should contain columns corresponding to the taxonomic ranks, such as family, genus, species, etc.
     The `--ranks` option allows you to specify the order of the ranks in the CSV file.
 
+    If the `csvfile` argument is not provided, the command will use the path specified in the configuration file.
+
     Args:
-        csvfile (str): Path to the CSV file containing the taxonomic data to be imported.
-        ranks (str): Comma-separated list of ranks in the hierarchy, in the order they appear in the CSV file.
-                     If not provided, the command will attempt to infer the ranks from the CSV file headers.
+        csvfile (str, optional): Path to the CSV file containing the taxonomic data to be imported.
+                                 If not provided, the path specified in the configuration file will be used.
+        ranks (str, optional): Comma-separated list of ranks in the hierarchy, in the order they appear in the CSV file.
+                               If not provided, the command will attempt to infer the ranks from the CSV file headers
+                               or use the ranks specified in the configuration file.
 
     Examples:
         $ niamoto import-taxonomy taxonomy.csv
         $ niamoto import-taxonomy taxonomy.csv --ranks=id_family,id_genus,id_species,id_infra
+        $ niamoto import-taxonomy
 
     Returns:
         None
 
     Raises:
-        FileNotFoundError: If the specified CSV file does not exist.
+        FileNotFoundError: If the specified CSV file does not exist and no default path is provided in the configuration.
         ValueError: If the provided ranks do not match the columns in the CSV file.
 
     Note:
         The CSV file should have a header row specifying the column names.
         The column names should match the ranks specified in the `--ranks` option, if provided.
     """
+    config = Config()
+    taxonomy_config = config.get("sources", "taxonomy")
+    ranks_from_config = taxonomy_config.get("ranks")
+    default_csvfile = taxonomy_config.get("path")
+
+    if not csvfile and default_csvfile and os.path.exists(default_csvfile):
+        csvfile = default_csvfile
+
+    if not csvfile or not os.path.exists(csvfile):
+        raise FileNotFoundError("CSV file not specified or does not exist.")
+
+    ranks = ranks or ranks_from_config
     ranks_tuple = tuple(ranks.split(",")) if ranks else ()
+
     data_importer = ApiImporter()
-    import_tax_result = data_importer.import_taxononomy(csvfile, ranks_tuple)
+    import_tax_result = data_importer.import_taxonomy(csvfile, ranks_tuple)
     console = Console()
     console.print(import_tax_result, style="italic green")
 
 
 @cli.command(name="import-plots")
-@click.argument("gpkg_file")
-def import_plots(gpkg_file: str) -> None:
+@click.argument("csvfile", required=False)
+def import_plots(csvfile: str) -> None:
     """
-    Import plot data from a GeoPackage file into the plot_ref table.
+    Import plot data from a CSV file into the database.
+
+    This command reads plot data from the specified CSV file and imports it into the database.
+    The CSV file should contain columns corresponding to the plot data.
 
-    This command reads plot data from the specified GeoPackage file and imports it into the plot_ref table in the database.
-    The GeoPackage file should contain a layer with plot geometries and associated attributes.
+    If the `csvfile` argument is not provided, the command will use the path specified in the configuration file.
 
     Args:
-        gpkg_file (str): Path to the GeoPackage file containing the plot data.
+        csvfile (str, optional): Path to the CSV file containing the plot data to be imported.
+                                 If not provided, the path specified in the configuration file will be used.
 
     Examples:
-        $ niamoto import-plots plots.gpkg
+        $ niamoto import-plots plots.csv
+        $ niamoto import-plots
 
     Returns:
         None
 
     Raises:
-        FileNotFoundError: If the specified GeoPackage file does not exist.
-        ValueError: If the GeoPackage file does not contain a valid plot layer.
-        Exception: If an error occurs during the import process.
+        FileNotFoundError: If the specified CSV file does not exist and no default path is provided in the configuration.
 
     Note:
-        The plot layer in the GeoPackage file should have a specific structure and attributes.
-        Refer to the documentation for the required structure of the plot layer.
+        The CSV file should have a header row specifying the column names.
     """
-    try:
-        api_importer = ApiImporter()
-        import_plot_results = api_importer.import_plots(gpkg_file)
-        console = Console()
-        console.print(import_plot_results, style="italic green")
-    except FileNotFoundError as e:
-        logger.exception(f"GeoPackage file not found: {e}")
-    except ValueError as e:
-        logger.exception(f"Invalid GeoPackage file: {e}")
-    except Exception as e:
-        logger.exception(f"Import failed: {e}")
+    config = Config()
+    plots_config = config.get("sources", "plots")
+    default_csvfile = plots_config.get("path")
+
+    if not csvfile and default_csvfile and os.path.exists(default_csvfile):
+        csvfile = default_csvfile
+
+    if not csvfile or not os.path.exists(csvfile):
+        raise FileNotFoundError("CSV file not specified or does not exist.")
+
+    data_importer = ApiImporter()
+    import_plots_result = data_importer.import_plots(csvfile)
+    console = Console()
+    console.print(import_plots_result, style="italic green")
 
 
 @cli.command(name="import-occurrences")
-@click.argument("csvfile")
+@click.argument("csvfile", required=False)
 @click.option(
-    "--taxon-id-column",
+    "--taxon-identifier",
     "-t",
-    required=True,
     help="Name of the column in the CSV that corresponds to the taxon ID.",
 )
-def import_occurrences(csvfile: str, taxon_id_column: str) -> None:
+def import_occurrences(csvfile: str, taxon_identifier: str) -> None:
     """
     Import occurrence data from a CSV file, analyze it to update the 'mapping' table, and link occurrences to their taxons.
 
     This command reads occurrence data from the specified CSV file, performs an analysis to update the 'mapping' table,
-    and establishes links between occurrences and their corresponding taxons based on the provided taxon ID column.
+    and establishes links between occurrences and their corresponding taxons based on the provided taxon identifier column.
+
+    If the `csvfile` argument is not provided, the command will use the path specified in the configuration file.
+    If the `--taxon-identifier` option is not provided, the command will use the taxon identifier specified in the configuration file.
 
     Args:
-        csvfile (str): Path to the CSV file containing the occurrence data to be imported and analyzed.
-        taxon_id_column (str): Name of the column in the CSV file that contains the taxon IDs.
+        csvfile (str, optional): Path to the CSV file containing the occurrence data to be imported and analyzed.
+                                 If not provided, the path specified in the configuration file will be used.
+        taxon_identifier (str, optional): Name of the column in the CSV file that contains the taxon IDs.
+                                          If not provided, the identifier specified in the configuration file will be used.
 
     Examples:
-        $ niamoto import-occurrences occurrences.csv --taxon-id-column=id_taxonref
-        $ niamoto import-occurrences occurrences.csv -t taxon_id
+        $ niamoto import-occurrences occurrences.csv --taxon-identifier=id_taxonref
+        $ niamoto import-occurrences occurrences.csv -t id_taxon
+        $ niamoto import-occurrences -t id_taxon
+        $ niamoto import-occurrences
 
     Returns:
         None
 
     Raises:
-        FileNotFoundError: If the specified CSV file does not exist.
-        ValueError: If the specified taxon ID column is not found in the CSV file.
+        FileNotFoundError: If the specified CSV file does not exist and no default path is provided in the configuration.
+        ValueError: If the specified taxon identifier column is not found in the CSV file.
         Exception: If an error occurs during the import process.
 
     Note:
         - The CSV file should have a header row specifying the column names.
-        - The taxon ID column should contain valid taxon identifiers that match the taxons in the database.
+        - The taxon identifier column should contain valid taxon identifiers that match the taxons in the database.
         - The 'mapping' table will be updated based on the analysis of the occurrence data.
     """
+    config = Config()
+    occurrences_config = config.get("sources", "occurrences")
+    default_csvfile = occurrences_config.get("path")
+    default_taxon_identifier = occurrences_config.get("taxon_identifier")
+
+    if not csvfile and default_csvfile and os.path.exists(default_csvfile):
+        csvfile = default_csvfile
+
+    if not csvfile or not os.path.exists(csvfile):
+        raise FileNotFoundError("CSV file not specified or does not exist.")
+
+    taxon_identifier = taxon_identifier or default_taxon_identifier
+    if not taxon_identifier:
+        raise ValueError("Taxon identifier column not specified.")
+
     data_importer = ApiImporter()
-    import_occ_result = data_importer.import_occurrences(csvfile, taxon_id_column)
+    import_occ_result = data_importer.import_occurrences(csvfile, taxon_identifier)
     console = Console()
     console.print(import_occ_result, style="italic green")
 
 
 @cli.command(name="import-occurrence-plots")
-@click.argument("csvfile")
+@click.argument("csvfile", required=False)
 def import_occurrence_plot_links(csvfile: str) -> None:
     """
     Import occurrence-plot links from a CSV file.
 
     This command reads occurrence-plot links from the specified CSV file and imports them into the database.
     The CSV file should contain columns representing the occurrence ID and the corresponding plot ID.
 
+    If the `csvfile` argument is not provided, the command will use the path specified in the configuration file.
+
     Args:
-        csvfile (str): Path to the CSV file containing the occurrence-plot links.
+        csvfile (str, optional): Path to the CSV file containing the occurrence-plot links.
+                                 If not provided, the path specified in the configuration file will be used.
 
     Examples:
         $ niamoto import-occurrence-plots occurrence_plots.csv
+        $ niamoto import-occurrence-plots
 
     Returns:
         None
 
     Raises:
-        FileNotFoundError: If the specified CSV file does not exist.
+        FileNotFoundError: If the specified CSV file does not exist and no default path is provided in the configuration.
         ValueError: If the CSV file does not contain the required columns for occurrence-plot links.
         Exception: If an error occurs during the import process.
 
     Note:
         - The CSV file should have a header row specifying the column names.
         - The required columns in the CSV file are:
             - 'occurrence_id': The ID of the occurrence.
             - 'plot_id': The ID of the plot associated with the occurrence.
         - The occurrence IDs and plot IDs should match the existing occurrences and plots in the database.
     """
+    config = Config()
+    occurrence_plots_config = config.get("sources", "occurrence-plots")
+    default_csvfile = occurrence_plots_config.get("path")
+
+    if not csvfile and default_csvfile and os.path.exists(default_csvfile):
+        csvfile = default_csvfile
+
+    if not csvfile or not os.path.exists(csvfile):
+        raise FileNotFoundError("CSV file not specified or does not exist.")
+
     try:
         api_importer = ApiImporter()
         import_occ_plot_results = api_importer.import_occurrence_plot_links(csvfile)
         console = Console()
         console.print(import_occ_plot_results, style="italic green")
     except FileNotFoundError as e:
         logger.exception(f"CSV file not found: {e}")
+        raise
     except ValueError as e:
         logger.exception(f"Invalid CSV file format: {e}")
+        raise
     except Exception as e:
         logger.exception(f"Import failed: {e}")
+        raise
+
+
+@cli.command(name="import-all")
+def import_all() -> None:
+    """
+    Import all data sources as specified in the configuration file.
+
+    This command reads the paths for taxonomy, plots, occurrences, and occurrence-plot links
+    from the configuration file, resets the relevant tables, and imports the data into the database.
+
+    Returns:
+        None
+
+    Raises:
+        FileNotFoundError: If any of the specified CSV files do not exist.
+        ValueError: If any required configurations are missing.
+    """
+    console = Console()
+    config = Config()
+    db_path = config.get("database", "path")
+
+    # Reset the tables
+    reset_tables(db_path)
+
+    # Import taxonomy
+    taxonomy_config = config.get("sources", "taxonomy")
+    taxonomy_csvfile = taxonomy_config.get("path")
+    taxonomy_ranks = taxonomy_config.get("ranks")
+    if not taxonomy_csvfile or not os.path.exists(taxonomy_csvfile):
+        raise FileNotFoundError(f"Taxonomy CSV file not found: {taxonomy_csvfile}")
+    data_importer = ApiImporter()
+    console.print(f"Importing taxonomy from {taxonomy_csvfile}", style="italic green")
+    data_importer.import_taxonomy(taxonomy_csvfile, tuple(taxonomy_ranks.split(",")))
+
+    # Import plots
+    plots_config = config.get("sources", "plots")
+    plots_csvfile = plots_config.get("path")
+    if not plots_csvfile or not os.path.exists(plots_csvfile):
+        raise FileNotFoundError(f"Plots CSV file not found: {plots_csvfile}")
+    console.print(f"Importing plots from {plots_csvfile}", style="italic green")
+    data_importer.import_plots(plots_csvfile)
+
+    # Import occurrences
+    occurrences_config = config.get("sources", "occurrences")
+    occurrences_csvfile = occurrences_config.get("path")
+    occurrences_taxon_identifier = occurrences_config.get("taxon_identifier")
+    if not occurrences_csvfile or not os.path.exists(occurrences_csvfile):
+        raise FileNotFoundError(
+            f"Occurrences CSV file not found: {occurrences_csvfile}"
+        )
+    console.print(
+        f"Importing occurrences from {occurrences_csvfile}", style="italic green"
+    )
+    data_importer.import_occurrences(occurrences_csvfile, occurrences_taxon_identifier)
+
+    # Import occurrence plots
+    occurrence_plots_config = config.get("sources", "occurrence-plots")
+    occurrence_plots_csvfile = occurrence_plots_config.get("path")
+    if not occurrence_plots_csvfile or not os.path.exists(occurrence_plots_csvfile):
+        raise FileNotFoundError(
+            f"Occurrence plots CSV file not found: {occurrence_plots_csvfile}"
+        )
+    console.print(
+        f"Importing occurrence plots from {occurrence_plots_csvfile}",
+        style="italic green",
+    )
+    data_importer.import_occurrence_plot_links(occurrence_plots_csvfile)
+
+    console.print("All data sources imported successfully.", style="bold green")
+
+
+def reset_tables(db_path: str) -> None:
+    """
+    Reset the tables using DuckDB and recreate them using SQLAlchemy models.
+
+    Args:
+        db_path (str): The path to the DuckDB database file.
+
+    Returns:
+        None
+
+    Raises:
+        Exception: If an error occurs during the reset process.
+    """
+    console = Console()
+    duckdb_connection = duckdb.connect(db_path)  # Connect directly to DuckDB
+
+    try:
+        console.print("Resetting tables...", style="bold yellow")
+
+        # Drop tables
+        duckdb_connection.execute("DROP TABLE IF EXISTS occurrences_plots")
+        duckdb_connection.execute("DROP TABLE IF EXISTS occurrences")
+        duckdb_connection.execute("DROP TABLE IF EXISTS plot_ref")
+        duckdb_connection.execute("DROP TABLE IF EXISTS taxon_ref")
+
+        console.print("Tables dropped successfully.", style="italic green")
+    except Exception as e:
+        console.print(f"Error resetting tables: {e}", style="bold red")
+        raise
+    finally:
+        duckdb_connection.close()
+
+    # Recreate tables using SQLAlchemy models
+    try:
+        db = Database(db_path)
+        engine = db.engine
+        Base.metadata.create_all(engine)
+        console.print("Tables recreated successfully.", style="italic green")
+    except Exception as e:
+        console.print(f"Error recreating tables: {e}", style="bold red")
+        raise
 
 
 @cli.command(name="generate-mapping")
 @click.option(
     "--data-source",
     type=str,
     help="Path to the CSV file to generate mapping from.",
```

### Comparing `niamoto-0.0.2a1/src/niamoto/common/config.py` & `niamoto-0.0.3a1/src/niamoto/common/config.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,126 +1,138 @@
 import os
 from typing import Any, Dict, Optional
-
 import yaml
 
 
 class Config:
     """
     Class to manage the configuration settings for Niamoto application.
 
     Attributes:
-        config (Dict[str, Any]): Configuration dictionary loaded from TOML file.
+        config (Dict[str, Any]): Configuration dictionary loaded from YAML file.
     """
 
     def __init__(
         self, config_path: Optional[str] = None, create_default: bool = True
     ) -> None:
         """
         Initializes the ConfigManager and loads the configuration file.
 
         Args:
             config_path (Optional[str]): Custom path to the configuration file.
                                          If None, default path is used.
+            create_default (bool): If True, creates a default configuration file if none exists.
         """
         niamoto_home = self.get_niamoto_home()
         self.config_path = config_path or os.path.join(niamoto_home, "config.yml")
         self.config: Dict[str, Any] = self.load_config(create_default)
 
     @property
     def database_path(self) -> Any:
+        """
+        Retrieves the database path from the configuration.
+
+        Returns:
+            Any: The database path.
+        """
         return self.get("database", "path")
 
     @property
-    def taxonomy_source(self) -> Any:
-        return self.get("sources", "taxonomy")
+    def logs_path(self) -> Any:
+        """
+        Retrieves the logs path from the configuration.
 
-    @property
-    def plots_source(self) -> Any:
-        return self.get("sources", "plots")
+        Returns:
+            Any: The logs path.
+        """
+        return self.get("logs", "path")
 
     @property
-    def occurrences_source(self) -> Any:
-        return self.get("sources", "occurrences")
+    def data_sources(self) -> Dict[str, Any]:
+        """
+        Retrieves the data sources section from the configuration.
 
-    @property
-    def occurrence_plots_source(self) -> Any:
-        return self.get("sources", "occurrence-plots")
+        Returns:
+            Dict[str, Any]: The data sources section.
+        """
+        return self.get_section("sources")
 
     @property
-    def raster_source(self) -> Any:
-        return self.get("sources", "raster")
+    def output_paths(self) -> Dict[str, Any]:
+        """
+        Retrieves the output paths section from the configuration.
 
-    @property
-    def static_pages_path(self) -> Any:
-        return self.get("web", "static_pages")
+        Returns:
+            Dict[str, Any]: The output paths section.
+        """
+        return self.get_section("outputs")
 
-    @property
-    def api_path(self) -> Any:
-        return self.get("web", "api")
+    def get_section(self, section: str) -> Dict[str, Any]:
+        """
+        Retrieves a specific section from the configuration.
 
-    @property
-    def logs_path(self) -> Any:
-        return self.get("logs", "path")
+        Args:
+            section (str): The configuration section to retrieve.
+
+        Returns:
+            Dict[str, Any]: The configuration section.
+        """
+        return self.config.get(section, {})
 
     def get(self, section: str, key: Optional[str] = None) -> Any:
         """
         Retrieves a specific configuration value or a whole section.
 
         Args:
             section (str): The configuration section to retrieve.
             key (Optional[str]): The specific key in the section to retrieve.
                                  If None, returns the whole section.
 
         Returns:
             Any: The configuration value or section.
         """
+        section_data = self.get_section(section)
         if key:
-            return self.config[section].get(key)
-        else:
-            return self.config.get(section)
+            return section_data.get(key)
+        return section_data
 
     @staticmethod
-    def get_niamoto_home() -> str:
+    def create_default_config() -> Dict[str, Any]:
         """
-        Get the Niamoto home directory.
+        Create a default configuration dictionary.
 
         Returns:
-            str: The Niamoto home directory.
-        """
-        niamoto_home = os.environ.get("NIAMOTO_HOME")
-        if niamoto_home:
-            return niamoto_home
-        else:
-            return os.path.join(os.getcwd(), "config")
-
-    @staticmethod
-    def create_default_config() -> Dict[Any, Any]:
-        """
-        Create a default configuration dictionary.
+            Dict[str, Any]: The default configuration dictionary.
         """
         return {
             "database": {"path": "data/db/niamoto.db"},
+            "logs": {"path": "logs"},
             "sources": {
-                "taxonomy": "data/sources/taxonomy.csv",
-                "plots": "data/sources/plots.gpkg",
-                "occurrences": "data/sources/occurrences.csv",
-                "occurrence-plots": "data/sources/occurrence-plots.csv",
-                "raster": "data/sources/raster",
+                "taxonomy": {
+                    "path": "data/sources/taxonomy.csv",
+                    "ranks": "id_family,id_genus,id_species,id_infra",
+                },
+                "plots": {"path": "data/sources/plots.gpkg"},
+                "occurrences": {
+                    "path": "data/sources/occurrences.csv",
+                    "taxon_identifier": "id_taxonref",
+                },
+                "occurrence-plots": {"path": "data/sources/occurrence-plots.csv"},
+                "raster": {"path": "data/sources/raster"},
             },
-            "web": {
-                "static_pages": "web/static",
-                "api": "web/api",
+            "outputs": {
+                "static_pages": "outputs/static",
+                "api": "outputs/api",
             },
-            "logs": {"path": "logs"},
+            "aggregations": [],
         }
 
     def create_config_file(self, config: Dict[str, Any]) -> None:
         """
-        Create or overwrite the TOML configuration file with the provided configuration.
+        Create or overwrite the YAML configuration file with the provided configuration.
 
         Args:
             config (Dict[str, Any]): Configuration to write to the file.
         """
         os.makedirs(os.path.dirname(self.config_path), exist_ok=True)
         with open(self.config_path, "w") as config_file:
             yaml.dump(config, config_file, default_flow_style=False, sort_keys=False)
@@ -151,27 +163,28 @@
             )
 
     def validate_config(self) -> Optional[Dict[Any, Any]]:
         """
         Validate the currently loaded configuration.
 
         Returns:
-            bool: True if the configuration is valid, False otherwise.
+            Optional[Dict[Any, Any]]: The validated configuration dictionary if the configuration is valid, None otherwise.
         """
         expected_keys = {
             "database": ["path"],
+            "logs": ["path"],
             "sources": [
                 "taxonomy",
                 "plots",
                 "occurrences",
                 "occurrence-plots",
                 "raster",
             ],
-            "web": ["static_pages", "api"],
-            "logs": ["path"],
+            "outputs": ["static_pages", "api"],
+            "aggregations": [],
         }
 
         try:
             with open(self.config_path, "r") as config_file:
                 config: Dict[Any, Any] = yaml.safe_load(config_file)
 
             for section, keys in expected_keys.items():
@@ -187,17 +200,20 @@
             return config
 
         except Exception as e:
             raise ValueError(f"Error validating configuration file: {e}")
 
     def load_config(self, create_default: bool = True) -> Any:
         """
-        Loads the configuration from the Yaml file. If the file does not exist,
+        Loads the configuration from the YAML file. If the file does not exist,
         creates a default configuration file.
 
+        Args:
+            create_default (bool): If True, creates a default configuration file if none exists.
+
         Returns:
             Dict[str, Any]: Configuration dictionary.
         """
         if os.path.exists(self.config_path):
             with open(self.config_path, "r") as config_file:
                 return yaml.safe_load(config_file)
         else:
@@ -205,7 +221,21 @@
                 config = self.create_default_config()
                 self.create_config_file(config)
                 return config
             else:
                 raise FileNotFoundError(
                     f"Configuration file not found: {self.config_path}"
                 )
+
+    @staticmethod
+    def get_niamoto_home() -> str:
+        """
+        Get the Niamoto home directory.
+
+        Returns:
+            str: The Niamoto home directory.
+        """
+        niamoto_home = os.environ.get("NIAMOTO_HOME")
+        if niamoto_home:
+            return niamoto_home
+        else:
+            return os.getcwd()
```

### Comparing `niamoto-0.0.2a1/src/niamoto/common/database.py` & `niamoto-0.0.3a1/src/niamoto/common/database.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,29 +16,25 @@
     """
     A class that provides a connection to a database and offers methods
     to interact with it.
 
     Attributes:
     - engine: The database engine connection.
     - session: A scoped session for creating new database sessions.
-
-    Methods:
-    - get_new_session: Returns a new session.
-    - add_instance_and_commit: Adds an instance to the session and commits it.
-    - close_db_session: Closes the database session.
     """
 
     def __init__(
         self,
         db_path: str,
     ) -> None:
         """
         Initialize the Database class with given parameters.
 
-        :param db_path: Path to the database file.
+        Args:
+            db_path (str): Path to the database file.
         """
 
         try:
             self.db_path = db_path
             self.connection_string = f"duckdb:///{db_path}"
             self.engine = create_engine(self.connection_string, echo=False)
             self.session_factory = sessionmaker(bind=self.engine)
@@ -49,75 +45,91 @@
                 f"SQLAlchemy error during database initialization: {e}"
             ) from e
 
     def has_table(self, table_name: str) -> bool:
         """
         Check if a table exists in the database.
 
-        :param table_name: The name of the table to check.
-        :return: True if the table exists, False otherwise.
+        Args:
+            table_name (str): The name of the table to check.
+
+        Returns:
+            bool: True if the table exists, False otherwise.
         """
         inspector = inspect(self.engine)
         return table_name in inspector.get_table_names()
 
     def get_new_session(self) -> scoped_session[Session]:
         """
         Get a new session from the session factory.
 
-        :return: A new session.
+        Returns:
+            scoped_session[Session]: A new session.
         """
         return self.session
 
     def add_instance_and_commit(self, instance: Any) -> None:
         """
         Add an instance to the session and commit.
 
-        :param instance: The instance to be added.
+        Args:
+            instance (Any): The instance to be added.
         """
         try:
             self.session.add(instance)
             self.session.commit()
         except exc.SQLAlchemyError as e:
             self.session.rollback()
             print(f"Error while adding and committing: {e}")
 
     @staticmethod
     def execute_query(query: Query[T]) -> Optional[List[Any]]:
         """
         Execute a given query and handle any database-related exceptions.
 
-        :param query: A SQLAlchemy query object.
-        :return: The result of the query if successful, None otherwise.
+        Args:
+            query (Query[T]): A SQLAlchemy query object.
+
+        Returns:
+            Optional[List[Any]]: The result of the query if successful, None otherwise.
         """
         try:
             return query.all()
         except (duckdb.duckdb.IOException, exc.SQLAlchemyError) as e:  # type: ignore
             Database.__handle_db_errors(e)
             return None
 
     def execute_select(self, sql: str) -> Optional[Any]:
         """
         Execute a SELECT query using the database engine.
 
-        :param sql: A string containing the SELECT query to be executed.
+        Args:
+            sql (str): A string containing the SELECT query to be executed.
+
+        Returns:
+            Optional[Any]: The result of the query if successful, None otherwise.
         """
         try:
             with self.engine.connect() as connection:
                 result = connection.execute(text(sql))
                 return result
         except (duckdb.duckdb.IOException, exc.SQLAlchemyError) as e:  # type: ignore
             print(f"Exception occurred: {e}")
             self.__handle_db_errors(e)
             return None
 
     def execute_sql(self, sql: str) -> Optional[Any]:
         """
         Execute a raw SQL query using the database engine.
 
-        :param sql: A string containing the SQL query to be executed.
+        Args:
+            sql (str): A string containing the SQL query to be executed.
+
+        Returns:
+            Optional[Any]: The result of the query if successful, None otherwise.
         """
         try:
             with self.engine.connect() as connection:
                 result = connection.execute(text(sql))
                 connection.commit()
                 return result
         except (duckdb.duckdb.IOException, exc.SQLAlchemyError) as e:  # type: ignore
@@ -194,16 +206,19 @@
             raise Exception("No active transaction to rollback.")
 
     @staticmethod
     def __handle_db_errors(error: Exception) -> None:
         """
         Private helper method to handle database-related errors.
 
-        :param error: The exception object that was raised.
-        :raises Exception: Raises an appropriate exception based on the error type.
+        Args:
+            error (Exception): The exception object that was raised.
+
+        Raises:
+            Exception: Raises an appropriate exception based on the error type.
         """
         if isinstance(error, duckdb.duckdb.IOException):  # type: ignore
             if "Resource temporarily unavailable" in str(error):
                 raise Exception(
                     "Database is currently in use by another application. Please try again later."
                 ) from error
             else:
```

### Comparing `niamoto-0.0.2a1/src/niamoto/core/components/importers/occurrences.py` & `niamoto-0.0.3a1/src/niamoto/core/components/importers/occurrences.py`

 * *Files 15% similar despite different names*

```diff
@@ -12,17 +12,17 @@
     def __init__(self, db_path: str):
         self.db_path = db_path
         self.con = duckdb.connect(self.db_path)
 
     @staticmethod
     def analyze_data(csvfile: str) -> Any:
         """
-        Analyze the data types of columns in a CSV file.
+        Analyzes the data types of columns in a CSV file.
 
-        Parameters:
+        Args:
             csvfile (str): Path to the CSV file to be analyzed.
 
         Returns:
             List[Tuple[str, str]]: A list of tuples with column names and types.
         """
         con = duckdb.connect()
         con.execute(
@@ -31,19 +31,22 @@
         types_info = con.execute("DESCRIBE temp_csv").fetchall()
         con.close()
 
         return [(col_info[0], col_info[1]) for col_info in types_info]
 
     def import_occurrences(self, csvfile: str, taxon_id_column: str) -> str:
         """
-        Create the 'occurrences' table based on the CSV file schema and import the data.
+        Creates the 'occurrences' table based on the CSV file schema and imports the data.
 
-        Parameters:
+        Args:
             csvfile (str): Path to the CSV file to be imported.
             taxon_id_column (str): Name of the column in the CSV that corresponds to the taxon ID.
+
+        Returns:
+            str: A message indicating the number of imported occurrences.
         """
         try:
             # Analyse the CSV file to get the schema
             column_schema = self.analyze_data(csvfile)
 
             # Ensure the taxon_id_column exists in the schema
             if taxon_id_column not in [
@@ -114,26 +117,38 @@
 
     def import_valid_occurrences(
         self, csvfile: str, taxon_id_column: str, only_existing_taxons: bool = True
     ) -> str:
         """
         Import occurrences from a CSV file. Optionally, only import occurrences with existing taxons.
 
-        Parameters:
+        Args:
             csvfile (str): Path to the CSV file to be imported.
             taxon_id_column (str): Name of the column in the CSV that corresponds to the taxon ID.
             only_existing_taxons (bool): If True, only import occurrences for existing taxons.
+
+        Returns:
+            str: A message indicating the number of valid occurrences imported.
+
+        Raises:
+            ValueError: If the specified taxon ID column is not found in the CSV file.
         """
         try:
             # Analyse the CSV file to get the schema
             column_schema = self.analyze_data(csvfile)
 
             # Check if 'id' column exists in the CSV schema
             id_column_exists = any(col_name == "id" for col_name, _ in column_schema)
 
+            # Verify that the taxon_id_column exists in the CSV schema
+            if not any(col_name == taxon_id_column for col_name, _ in column_schema):
+                raise ValueError(
+                    f"The specified taxon ID column '{taxon_id_column}' is not found in the CSV file."
+                )
+
             # Create the 'occurrences' table
             columns_sql = ", ".join(
                 [f"{col_name} {col_type}" for col_name, col_type in column_schema]
             )
             if not id_column_exists:
                 columns_sql = f"id BIGINT PRIMARY KEY, {columns_sql}"
             columns_sql += ", taxon_ref_id BIGINT REFERENCES taxon_ref(id)"
@@ -185,14 +200,16 @@
             if result is not None:
                 imported_count = result[0]
             else:
                 imported_count = 0
 
             return f"Total valid occurrences imported: {imported_count}"
 
+        except ValueError as ve:
+            raise ve
         except Exception as e:
             raise e
 
     def import_occurrence_plot_links(self, csvfile: str) -> str:
         try:
             # Analyse the CSV file to get the schema
             column_schema = self.analyze_data(csvfile)
```

### Comparing `niamoto-0.0.2a1/src/niamoto/core/components/importers/plots.py` & `niamoto-0.0.3a1/src/niamoto/core/components/importers/plots.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,26 +2,42 @@
 from shapely.wkt import dumps  # type: ignore
 
 from niamoto.core.models import PlotRef
 from niamoto.common.database import Database
 
 
 class PlotImporter:
+    """
+    A class used to import plot data from a GeoPackage file into the database.
+
+    Attributes:
+        db (Database): The database connection.
+    """
+
     def __init__(self, db: Database):
+        """
+        Initializes the PlotImporter with the database connection.
+
+        Args:
+            db (Database): The database connection.
+        """
         self.db = db
 
     def import_from_gpkg(self, file_path: str) -> str:
         """
         Import plot data from a GeoPackage file.
 
         Args:
-            file_path:  The path to the GeoPackage file to be imported.
+            file_path (str): The path to the GeoPackage file to be imported.
 
         Returns:
+            str: A message indicating the success of the import operation.
 
+        Raises:
+            Exception: If an error occurs during the import operation.
         """
         plots_data = gpd.read_file(file_path)
 
         try:
             for index, row in plots_data.iterrows():
                 # Convert Shapely geometry to WKT
                 wkt_geometry = dumps(row["geometry"]) if row["geometry"] else None
```

### Comparing `niamoto-0.0.2a1/src/niamoto/core/components/mappers/mapping_manager.py` & `niamoto-0.0.3a1/src/niamoto/core/components/mappers/mapping_manager.py`

 * *Files 20% similar despite different names*

```diff
@@ -13,24 +13,46 @@
 
 from niamoto.common.database import Database
 from niamoto.core.models import Mapping
 from niamoto.core.utils.csv_utils import analyze_csv_data_types, is_duckdb_type_numeric
 
 
 class MappingManager:
+    """
+    A class used to manage the mapping of data.
+
+    Attributes:
+        db (Database): The database connection.
+    """
+
     def __init__(self, db: Database):
+        """
+        Initializes the MappingManager with the database connection.
+
+        Args:
+            db (Database): The database connection.
+        """
         self.db = db
 
     def generate_mapping(
         self,
         csvfile: str,
         group_by: str,
         reference_table_name: Optional[str] = None,
         reference_data_path: Optional[str] = None,
     ) -> None:
+        """
+        Generate a mapping from a CSV file.
+
+        Args:
+            csvfile (str): The path to the CSV file.
+            group_by (str): The group by field.
+            reference_table_name (Optional[str], optional): The reference table name. Defaults to None.
+            reference_data_path (Optional[str], optional): The reference data path. Defaults to None.
+        """
         console = Console()
         try:
             con = duckdb.connect()
             con.execute(
                 f"CREATE TEMPORARY TABLE temp_csv AS SELECT * FROM READ_CSV_AUTO('{csvfile}')"
             )
             session = self.db.get_new_session()
@@ -100,29 +122,28 @@
                 }
                 if column_name == identifier_field:
                     column_mapping_data["is_identifier"] = True
                 mapping_data[column_name] = column_mapping_data
             self.db.commit_session()
             console.print(f"Mapping table updated for {csvfile}", style="italic green")
 
-            # Write the mapping data to the mapping file
-            mapping_path = os.path.join(os.getcwd(), "config", "mapping.yml")
-
-            # Load the existing mapping data if the file exists
-            if os.path.exists(mapping_path):
-                with open(mapping_path, "r") as mapping_file:
-                    existing_mapping_data = yaml.safe_load(mapping_file) or []
-            else:
-                existing_mapping_data = []
+            # Load the existing configuration data
+            config_path = os.path.join(os.getcwd(), "config.yml")
+            with open(config_path, "r") as config_file:
+                config_data = yaml.safe_load(config_file) or {}
+
+            # Ensure 'aggregations' section exists
+            if "aggregations" not in config_data:
+                config_data["aggregations"] = []
 
             # Check if an entry with the same 'group_by' value already exists
             existing_entry = next(
                 (
                     entry
-                    for entry in existing_mapping_data
+                    for entry in config_data["aggregations"]
                     if entry["group_by"] == group_by
                 ),
                 None,
             )
 
             if existing_entry:
                 # Update the existing entry with the new mapping data
@@ -136,36 +157,45 @@
                     "group_by": group_by,
                     "identifier": identifier_field,
                     "target_table_name": "occurrences",
                     "reference_table_name": reference_table_name,
                     "reference_data_path": reference_data_path,
                     "fields": mapping_data,
                 }
-                existing_mapping_data.append(new_mapping_entry)
+                config_data["aggregations"].append(new_mapping_entry)
 
-            # Write the updated mapping data to the file
-            with open(mapping_path, "w") as mapping_file:
+            # Write the updated configuration data to the file
+            with open(config_path, "w") as config_file:
                 yaml.safe_dump(
-                    existing_mapping_data,
-                    mapping_file,
+                    config_data,
+                    config_file,
                     default_flow_style=None,
                     sort_keys=False,
                 )
             console.print(
-                f"Mapping data written to {mapping_path}", style="italic green"
+                f"Mapping data written to {config_path}", style="italic green"
             )
 
         except Exception as e:
             console.print(f"Error while generating mapping: {e}", style="bold red")
 
         finally:
             self.db.close_db_session()
 
     @staticmethod
     def add_mapping(field: str) -> str:
+        """
+        Add a new field to the mapping.
+
+        Args:
+            field (str): The field to be added.
+
+        Returns:
+            str: A message indicating the field has been added.
+        """
         return f"Adding new field {field} to the mapping"
         # Implement the logic to add a new field to the existing mapping
 
     @staticmethod
     def add_mapping_entry(
         session: Any,
         column_name: str,
@@ -173,14 +203,28 @@
         group_by: str,
         reference_table_name: Optional[str],
         reference_data_path: Optional[str],
         transforms: Optional[List[Dict[str, str]]] = None,
         bins: Optional[Collection[str]] = None,
         is_identifier: bool = False,
     ) -> None:
+        """
+        Add a mapping entry.
+
+        Args:
+            session (Any): The session to use.
+            column_name (str): The column name.
+            column_schema (List[Tuple[str, str]]): The column schema.
+            group_by (str): The group by field.
+            reference_table_name (Optional[str]): The reference table name. Defaults to None.
+            reference_data_path (Optional[str]): The reference data path. Defaults to None.
+            transforms (Optional[List[Dict[str, str]]] optional): The transforms. Defaults to None.
+            bins (Optional[Collection[str]], optional): The bins. Defaults to None.
+            is_identifier (bool, optional): Whether the field is an identifier. Defaults to False.
+        """
         field_type = next((ct for cn, ct in column_schema if cn == column_name), None)
         mapping_entry = (
             session.query(Mapping)
             .filter_by(target_field=column_name, group_by=group_by)
             .first()
         )
         if mapping_entry:
@@ -213,14 +257,25 @@
                 bins=",".join(map(str, bins)) if bins else None,
             )
             session.add(new_entry)
 
     def get_transforms_and_bins(
         self, con: DuckDBPyConnection, column_name: str, column_type: Any
     ) -> tuple[list[dict[str, str]], Collection[str]]:
+        """
+        Get the transforms and bins for a column.
+
+        Args:
+            con (DuckDBPyConnection): The connection to use.
+            column_name (str): The column name.
+            column_type (Any): The column type.
+
+        Returns:
+            tuple[list[dict[str, str]], Collection[str]]: The transforms and bins.
+        """
         apply_transforms = self.custom_confirm(
             f"Apply transformations for [bold]{column_name}[/bold]?", default=True
         )
         transforms = (
             self.determine_transformations(column_type) if apply_transforms else []
         )
         calculate_bins = self.custom_confirm(
@@ -231,14 +286,24 @@
             if calculate_bins
             else []
         )
         return transforms, bins
 
     @staticmethod
     def custom_confirm(question: str, default: bool = False) -> bool:
+        """
+        Custom confirm prompt.
+
+        Args:
+            question (str): The question to ask.
+            default (bool, optional): The default answer. Defaults to False.
+
+        Returns:
+            bool: The user's answer.
+        """
         console = Console()
         while True:
             console.print(question, end=" ")
             response = click.prompt(
                 "(Y/n)" if default else "(y/N)", default="", show_default=False
             ).lower()
             if not response:
@@ -248,14 +313,23 @@
             elif response in ["n", "no"]:
                 return False
             else:
                 console.print("Invalid input. Please enter 'y' or 'n'.")
 
     @staticmethod
     def determine_transformations(data_type: str) -> List[Dict[str, str]]:
+        """
+        Determine the transformations for a data type.
+
+        Args:
+            data_type (str): The data type.
+
+        Returns:
+            List[Dict[str, str]]: The transformations.
+        """
         if is_duckdb_type_numeric(data_type):
             return [
                 {"name": "mean"},
                 {"name": "max"},
                 {"name": "median"},
                 {"name": "min"},
             ]
@@ -264,14 +338,26 @@
     @staticmethod
     def calculate_default_bins(
         con: DuckDBPyConnection,
         column_name: str,
         column_type: str,
         num_intervals: int = 6,
     ) -> Dict[str, Any]:
+        """
+        Calculate the default bins for a column.
+
+        Args:
+            con (DuckDBPyConnection): The connection to use.
+            column_name (str): The column name.
+            column_type (str): The column type.
+            num_intervals (int, optional): The number of intervals. Defaults to 6.
+
+        Returns:
+            Dict[str, Any]: The default bins.
+        """
         if is_duckdb_type_numeric(column_type):
             if column_type == "BOOLEAN":
                 return {}
 
             min_query = f"SELECT MIN({column_name}) FROM temp_csv"
             max_query = f"SELECT MAX({column_name}) FROM temp_csv"
 
@@ -312,31 +398,54 @@
                     "title": f"{column_name.capitalize()} Distribution",
                     "color": "blue",
                 },
             }
 
         return {}
 
-    @staticmethod
-    def get_mapping() -> List[Dict[str, Any]]:
-        mapping_path = os.path.join(os.getcwd(), "config", "mapping.yml")
-        if os.path.exists(mapping_path):
-            with open(mapping_path, "r") as mapping_file:
-                mapping_data = yaml.safe_load(mapping_file) or []
+    def get_mapping(self) -> List[Dict[str, Any]]:
+        """
+        Get the mapping.
+
+        Returns:
+            List[Dict[str, Any]]: The mapping.
+        """
+        config_path = os.path.join(os.getcwd(), "config.yml")
+        if os.path.exists(config_path):
+            with open(config_path, "r") as config_file:
+                config_data = yaml.safe_load(config_file) or {}
+                return config_data.get("aggregations", [])
         else:
-            mapping_data = []
-        return mapping_data
+            return []
 
     def get_group_config(self, group_by: str) -> Dict[str, Any]:
+        """
+        Get the group config for a group.
+
+        Args:
+            group_by (str): The group by field.
+
+        Returns:
+            Dict[str, Any]: The group config.
+        """
         mapping_data = self.get_mapping()
         group_config = next(
             (entry for entry in mapping_data if entry["group_by"] == group_by), None
         )
         return group_config if group_config is not None else {}
 
     def get_fields(self, group_by: str) -> Dict[str, Any]:
+        """
+        Get the fields for a group.
+
+        Args:
+            group_by (str): The group by field.
+
+        Returns:
+            Dict[str, Any]: The fields.
+        """
         group_config: Optional[Dict[str, Any]] = self.get_group_config(group_by)
         if group_config:
             fields: Dict[str, Any] = group_config["fields"]
             return fields
         else:
             return {}
```

### Comparing `niamoto-0.0.2a1/src/niamoto/core/components/statistics/plot_stats_calculator.py` & `niamoto-0.0.3a1/src/niamoto/core/components/statistics/plot_stats_calculator.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,21 +1,37 @@
 from typing import List, Dict, Any, Hashable
 from .statistics_calculator import StatisticsCalculator
 from ...models import PlotRef
 
 
 class PlotStatsCalculator(StatisticsCalculator):
+    """
+    A class used to calculate statistics for plots.
+
+    Inherits from:
+        StatisticsCalculator
+    """
+
     def calculate_plot_stats(self) -> None:
+        """
+        Calculate statistics for all plots.
+        """
         # Retrieve the unique identifiers of the plots from PlotRef
         plot_ids = self.get_unique_plot_ids()
 
         for plot_id in plot_ids:
             self.process_group(plot_id)
 
     def process_group(self, plot_id: int) -> None:
+        """
+        Process a group of plots.
+
+        Args:
+            plot_id (int): The plot id.
+        """
         # Filter the occurrences related to the current plot from the occurrences_plots table
         plot_occurrences = self.get_plot_occurrences(plot_id)
 
         # Calculate the general statistics for each field of the mapping
         stats = self.calculate_stats(plot_id, plot_occurrences)
 
         # Calculate the specific statistics for the plots
@@ -24,31 +40,66 @@
 
         # Create or update the entry in the plot_stats table
         self.create_or_update_stats_entry(plot_id, stats)
 
     def calculate_specific_stats(
         self, plot_id: int, plot_occurrences: list[dict[Hashable, Any]]
     ) -> Dict[str, Any]:
+        """
+        Calculate specific statistics for a plot.
+
+        Args:
+            plot_id (int): The plot id.
+            plot_occurrences (list[dict[Hashable, Any]]): The plot occurrences.
+
+        Returns:
+            Dict[str, Any]: The specific statistics.
+        """
         frequencies = self.calculate_frequencies(plot_id, plot_occurrences)
         return frequencies
 
     def calculate_frequencies(
         self, plot_id: int, plot_occurrences: list[dict[Hashable, Any]]
     ) -> Dict[str, Any]:
+        """
+        Calculate frequencies for a plot.
+
+        Args:
+            plot_id (int): The plot id.
+            plot_occurrences (list[dict[Hashable, Any]]): The plot occurrences.
+
+        Returns:
+            Dict[str, Any]: The frequencies.
+        """
         frequencies: Dict[str, Any] = {}
         # Calculate the specific frequencies for the plots (altitude, rainfall, etc.)
         # ...
         return frequencies
 
     def get_unique_plot_ids(self) -> List[int]:
+        """
+        Get unique plot ids.
+
+        Returns:
+            List[int]: The unique plot ids.
+        """
         # Retrieve the unique identifiers of the plots from PlotRef
         plot_ids = self.db.session.query(PlotRef.id).all()
         return [plot_id[0] for plot_id in plot_ids]
 
     def get_plot_occurrences(self, plot_id: int) -> list[dict[Hashable, Any]]:
+        """
+        Get plot occurrences.
+
+        Args:
+            plot_id (int): The plot id.
+
+        Returns:
+            list[dict[Hashable, Any]]: The plot occurrences.
+        """
         occurrence_identifier = self.identifier
         query = f"""
             SELECT o.*
             FROM occurrences o
             JOIN occurrences_plots op ON o.{occurrence_identifier} = op.occurrence_id
             WHERE op.plot_id = {plot_id}
         """
```

### Comparing `niamoto-0.0.2a1/src/niamoto/core/components/statistics/statistics_calculator.py` & `niamoto-0.0.3a1/src/niamoto/core/components/statistics/statistics_calculator.py`

 * *Files 17% similar despite different names*

```diff
@@ -7,21 +7,46 @@
 import pandas as pd
 
 from niamoto.common.database import Database
 from niamoto.core.services.mapper import MapperService
 
 
 class StatisticsCalculator(ABC):
+    """
+    An abstract base class for calculating statistics.
+
+    Attributes:
+        db (Database): The database connection.
+        con (duckdb.DuckDBPyConnection): The DuckDB connection.
+        mapper_service (MapperService): The mapper service.
+        occurrences (list[dict[Hashable, Any]]): The occurrences.
+        group_by (str): The group by field.
+        group_config (dict[str, Any]): The group configuration.
+        identifier (str): The identifier.
+        reference_table_name (str): The reference table name.
+        reference_data_path (str): The reference data path.
+        fields (dict[str, Any]): The fields.
+    """
+
     def __init__(
         self,
         db: Database,
         mapper_service: MapperService,
         occurrences: list[dict[Hashable, Any]],
         group_by: str,
     ):
+        """
+        Initializes the StatisticsCalculator with the database connection, mapper service, occurrences, and group by field.
+
+        Args:
+            db (Database): The database connection.
+            mapper_service (MapperService): The mapper service.
+            occurrences (list[dict[Hashable, Any]]): The occurrences.
+            group_by (str): The group by field.
+        """
         self.db = db
         self.con = duckdb.connect(self.db.db_path)
         self.mapper_service = mapper_service
         self.occurrences = occurrences
         self.group_by = group_by
         self.group_config = self.mapper_service.get_group_config(group_by)
         self.identifier = self.group_config.get("identifier")
@@ -29,19 +54,39 @@
         self.reference_data_path = self.group_config.get("reference_data_path")
         self.fields = self.mapper_service.get_fields(group_by)
 
     @abstractmethod
     def calculate_specific_stats(
         self, group_id: int, group_occurrences: list[dict[Hashable, Any]]
     ) -> Dict[str, Any]:
+        """
+        Abstract method to calculate specific statistics for a group.
+
+        Args:
+            group_id (int): The group id.
+            group_occurrences (list[dict[Hashable, Any]]): The group occurrences.
+
+        Returns:
+            Dict[str, Any]: The specific statistics.
+        """
         pass
 
     def calculate_stats(
         self, group_id: int, group_occurrences: list[dict[Hashable, Any]]
     ) -> Dict[str, Any]:
+        """
+        Calculate statistics for a group.
+
+        Args:
+            group_id (int): The group id.
+            group_occurrences (list[dict[Hashable, Any]]): The group occurrences.
+
+        Returns:
+            Dict[str, Any]: The statistics.
+        """
         stats: Dict[str, Union[int, Dict[str, Any], pd.Series[Any], float]] = {}
 
         # Convert occurrences to pandas DataFrame
         df_occurrences = pd.DataFrame(group_occurrences)
 
         # Iterate over fields in the mapping
         for field, field_config in self.fields.items():
@@ -108,26 +153,36 @@
         # Add group-specific stats
         specific_stats = self.calculate_specific_stats(group_id, group_occurrences)
         stats.update(specific_stats)
 
         return stats
 
     def initialize_stats_table(self) -> None:
+        """
+        Initialize the statistics table.
+        """
         # Construct the name of the statistics table by appending "_stats" to the group name
         table_name = f"{self.group_by}_stats"
 
         # Call the create_stats_table method with the constructed table name
         # and initialize parameter set to True. This will create a new table in the database
         # with the given name. If a table with the same name already exists, it will be dropped
         # and a new one will be created.
         self.create_stats_table(table_name, initialize=True)
 
     def create_or_update_stats_entry(
         self, group_id: int, stats: Dict[str, Any]
     ) -> None:
+        """
+        Create or update a statistics entry.
+
+        Args:
+            group_id (int): The group id.
+            stats (Dict[str, Any]): The statistics.
+        """
         table_name = f"{self.group_by}_stats"
         # Check if the table exists, otherwise create it
         if not self.db.has_table(table_name):
             self.create_stats_table(table_name)
 
         # Check if an entry exists for this group
         query = f"""
@@ -150,14 +205,21 @@
                 insert_query = f"""
                         INSERT INTO {table_name} ({self.group_by}_id, {', '.join(stats.keys())})
                         VALUES ({group_id}, {', '.join(f"'{json.dumps(value)}'" if isinstance(value, dict) else f"'{value}'" for value in stats.values())})
                     """
                 self.db.execute_sql(insert_query)
 
     def create_stats_table(self, table_name: str, initialize: bool = False) -> None:
+        """
+        Create a statistics table.
+
+        Args:
+            table_name (str): The table name.
+            initialize (bool, optional): Whether to initialize the table. Defaults to False.
+        """
         if initialize:
             drop_query = f"DROP TABLE IF EXISTS {table_name}"
             self.con.execute(drop_query)
 
         fields_sql = [f"{self.group_by}_id INTEGER PRIMARY KEY"]
 
         for field, config in self.fields.items():
@@ -232,19 +294,19 @@
         }
 
     @staticmethod
     def extract_coordinates(filtered_data: Any) -> List[Dict[str, Any]]:
         """
         Extract unique geographic coordinates and their occurrence counts from the filtered data.
 
-        Parameters:
+        Args:
             filtered_data (pd.DataFrame): The DataFrame containing the filtered data.
 
         Returns:
-            list: A list of dictionaries containing unique coordinates and their occurrence counts.
+            List[Dict[str, int]]: A list of dictionaries containing unique coordinates and their occurrence counts.
         """
         coordinate_counts: defaultdict[Tuple[float, ...], int] = defaultdict(int)
 
         for point in filtered_data["geo_pt"]:
             if pd.notna(point):  # Check that the point is not NaN
                 coordinates = tuple(
                     map(
```

### Comparing `niamoto-0.0.2a1/src/niamoto/core/components/statistics/taxonomy_stats_calculator.py` & `niamoto-0.0.3a1/src/niamoto/core/components/statistics/taxonomy_stats_calculator.py`

 * *Files 26% similar despite different names*

```diff
@@ -7,15 +7,25 @@
 from sqlalchemy import select
 
 from .statistics_calculator import StatisticsCalculator
 from niamoto.core.models import TaxonRef
 
 
 class TaxonomyStatsCalculator(StatisticsCalculator):
+    """
+    A class used to calculate statistics for taxonomies.
+
+    Inherits from:
+        StatisticsCalculator
+    """
+
     def calculate_taxonomy_stats(self) -> None:
+        """
+        Calculate statistics for all taxonomies.
+        """
         start_time = time.time()
 
         # Retrieve all taxons from the TaxonRef table in the database
         taxons = self.db.session.query(TaxonRef).all()
 
         # Initialize the statistics table for storing the calculated statistics for each taxon
         self.initialize_stats_table()
@@ -30,14 +40,20 @@
 
         console = Console()
         console.print(
             f"Total processing time: {total_time:.2f} seconds", style="italic blue"
         )
 
     def process_taxon(self, taxon: TaxonRef) -> None:
+        """
+        Process a taxon.
+
+        Args:
+            taxon (niamoto.core.models.models.TaxonRef): The taxon to process.
+        """
         # Extract the taxon ID value from the Column[int]
         taxon_id = self.db.session.execute(select(taxon.id)).scalar()
 
         # Check if taxon_id is None
         if taxon_id is None:
             # Handle the case when taxon_id is None
             # You can choose to return or use a default value
@@ -58,41 +74,79 @@
         specific_stats = self.calculate_specific_stats(taxon_id, taxon_occurrences)
         stats.update(specific_stats)
 
         # Create or update the entry in the taxonomy_stats table
         self.create_or_update_stats_entry(taxon_id, stats)
 
     def get_taxon_occurrences(self, taxon: TaxonRef) -> list[dict[Hashable, Any]]:
+        """
+        Get taxon occurrences.
+
+        Args:
+            taxon (niamoto.core.models.models.TaxonRef): The taxon to get occurrences for.
+
+        Returns:
+            list[dict[Hashable, Any]]: The taxon occurrences.
+        """
         # Retrieve the identifiers of the taxon and its descendants
         taxon_ids = self.get_taxon_and_descendant_ids(taxon)
 
         # Filter the occurrences for the taxon and its descendants
         taxon_occurrences = [
             occ for occ in self.occurrences if occ[self.identifier] in taxon_ids
         ]
 
         # Return the filtered occurrences
         return taxon_occurrences
 
     def get_taxon_and_descendant_ids(self, taxon: TaxonRef) -> List[int]:
+        """
+        Get taxon and descendant ids.
+
+        Args:
+            taxon (niamoto.core.models.models.TaxonRef): The taxon to get ids for.
+
+        Returns:
+            List[int]: The taxon and descendant ids.
+        """
         # Retrieve the identifiers of the taxon and its descendants using the lft and rght fields
         taxon_ids = (
             self.db.session.query(TaxonRef.id)
             .filter(TaxonRef.lft >= taxon.lft, TaxonRef.rght <= taxon.rght)
             .all()
         )
 
         # Return a list of taxon identifiers
         return [taxon_id[0] for taxon_id in taxon_ids]
 
     def calculate_specific_stats(
         self, taxon_id: int, taxon_occurrences: list[dict[Hashable, Any]]
     ) -> Dict[str, Any]:
+        """
+        Calculate specific statistics for a taxon.
+
+        Args:
+            taxon_id (int): The taxon id.
+            taxon_occurrences (list[dict[Hashable, Any]]): The taxon occurrences.
+
+        Returns:
+            Dict[str, Any]: The specific statistics.
+        """
         frequencies = self.calculate_frequencies(taxon_id, taxon_occurrences)
         return frequencies
 
     def calculate_frequencies(
         self, taxon_id: int, taxon_occurrences: list[dict[Hashable, Any]]
     ) -> Dict[str, Any]:
+        """
+        Calculate frequencies for a taxon.
+
+        Args:
+            taxon_id (int): The taxon id.
+            taxon_occurrences (list[dict[Hashable, Any]]): The taxon occurrences.
+
+        Returns:
+            Dict[str, Any]: The frequencies.
+        """
         frequencies: Dict[str, Any] = {}
 
         return frequencies
```

### Comparing `niamoto-0.0.2a1/src/niamoto/core/repositories/niamoto_repository.py` & `niamoto-0.0.3a1/src/niamoto/core/repositories/niamoto_repository.py`

 * *Files 12% similar despite different names*

```diff
@@ -42,14 +42,23 @@
         query = self.session.query(entity_class)
         if order_by is not None:
             query = query.order_by(order_by)
         return query.all()
 
     @staticmethod
     def build_taxonomy_tree(taxons: Any) -> Any:
+        """
+        Builds a taxonomy tree from a list of taxons.
+
+        Args:
+            taxons (list): The list of taxons to build the tree from.
+
+        Returns:
+            list: A list of root nodes of the taxonomy tree.
+        """
         rank_order = {"Famille": 1, "Genus": 2, "Species": 3, "Variety": 4}
 
         sorted_taxons = sorted(taxons, key=lambda x: rank_order.get(x.rank_name, 5))
 
         tree = {}
         for taxon in sorted_taxons:
             tree[taxon.id] = {
@@ -71,15 +80,23 @@
         Closes the database session.
         """
         self.db.close_db_session()
 
     def __enter__(self) -> "NiamotoRepository":
         """
         Enters the context manager and opens the database session.
+
+        Returns:
+            NiamotoRepository: The current instance of the NiamotoRepository.
         """
         return self
 
     def __exit__(self, exc_type: Any, exc_val: Any, exc_tb: Any) -> None:
         """
         Exits the context manager and closes the database session.
+
+        Args:
+            exc_type (Any): The type of the exception.
+            exc_val (Any): The value of the exception.
+            exc_tb (Any): The traceback of the exception.
         """
         self.close_session()
```

### Comparing `niamoto-0.0.2a1/src/niamoto/core/services/processor.py` & `niamoto-0.0.3a1/src/niamoto/core/services/processor.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,21 +20,28 @@
 class TaxonDataProcessor:
     """
     Processor for handling taxon data operations, including reading from a DataFrame,
     processing data, and writing to a database.
     """
 
     def __init__(self, db_path: str):
-        """Initialize the processor with a database name."""
+        """
+        Initialize the processor with a database name.
+
+        Args:
+            db_path (str): The path to the database file.
+        """
         self.db = Database(db_path)
         self.console = Console()
         self.config = Config()
 
     def process_and_write_taxon_data(self, data: Any) -> None:
-        """Process the provided taxon data and write it to the database."""
+        """
+        Process the provided taxon data and write it to the database.
+        """
         start_time = time.time()
         # Sort the DataFrame for easier processing
 
         taxonomy_config = {
             "Family": {"field": "id_family", "parent": ""},
             "Genus": {"field": "id_genus", "parent": "Family"},
             "Species": {"field": "id_species", "parent": "Genus"},
@@ -71,15 +78,15 @@
 
     def generate_taxonomy_from_occurrences(
         self, data: Any, model: Any, config: Dict[str, Any]
     ) -> None:
         """
         Generate the taxonomy hierarchy from occurrence data.
 
-        Parameters:
+        Args:
             data: DataFrame containing the occurrence data.
             model: The SQLAlchemy model to use for the taxon hierarchy.
             config: Configuration defining the taxonomic ranks and their hierarchy.
         """
         sorted_df = data.sort_values(
             by=["id_family", "id_genus", "id_species", "id_infra"]
         )
@@ -88,20 +95,19 @@
 
     def create_taxonomic_hierarchy(
         self, data: Any, session: Any, model: Any, taxonomy_config: Dict[str, Any]
     ) -> None:
         """
         Creates a taxonomic hierarchy based on a given configuration.
 
-        Parameters:
+        Args:
             data: DataFrame containing the taxonomic data.
             session: Database session.
             model: The SQLAlchemy model to use for the taxonomic hierarchy.
             taxonomy_config: Configuration defining the taxonomic ranks and their hierarchy.
-
         """
 
         for rank in taxonomy_config:
             self.create_taxons_for_rank(
                 data, session, model, rank, taxonomy_config[rank], taxonomy_config
             )
 
@@ -113,15 +119,15 @@
         rank_name: str,
         rank_config: Dict[str, Any],
         taxonomy_config: Dict[str, Any],
     ) -> None:
         """
         Creates taxons for a specific rank based on the configuration.
 
-        Parameters:
+        Args:
             data: DataFrame containing the taxonomic data.
             session: Database session.
             model: The SQLAlchemy model to use for the taxonomic hierarchy.
             rank_name: The name of the taxonomic rank.
             rank_config: Configuration for the taxonomic rank.
             taxonomy_config: Configuration defining the taxonomic ranks and their hierarchy.
         """
@@ -157,17 +163,15 @@
                 parent_id = (
                     int(row[parent_id_field])
                     if parent_id_field and pd.notna(row[parent_id_field])
                     else None
                 )
                 if parent_id:
                     parent_taxon = (
-                        session.query(TaxonRef)
-                        .filter(TaxonRef.id == parent_id)
-                        .first()
+                        session.query(TaxonRef).filter(TaxonRef.id == parent_id).first()
                     )
                     parent_id = parent_taxon.id if parent_taxon else None
 
                 full_name = self.determine_full_name(row, rank_name)
                 taxon = model(
                     id_taxonref=id_native,
                     id_family=int(taxon_ids["id_family"])
@@ -191,15 +195,15 @@
         session.commit()
 
     @staticmethod
     def determine_full_name(row: Any, rank_name: str) -> Any:
         """
         Determine the full name for a given taxon rank.
 
-        Parameters:
+        Args:
             row (pd.Series): Data row containing taxon information.
             rank_name (str): The rank name of the taxon.
 
         Returns:
             str: The full name of the taxon.
         """
         if rank_name == "Family":
@@ -208,15 +212,15 @@
             return row["taxaname"].split()[0] if "taxaname" in row else ""
         return row.get("taxaname", "")
 
     def perform_calculations(self, data: Any, taxonomy_config: Dict[str, Any]) -> None:
         """
         Perform calculations for each taxonomic level and update the Taxon objects in the database.
 
-        Parameters:
+        Args:
             data (pd.DataFrame): The DataFrame containing occurrence data.
             taxonomy_config (dict): The configuration defining the taxonomic ranks and their hierarchy.
         """
 
         processed_ranks = set()
 
         # Perform calculations for each taxonomic level
@@ -229,15 +233,15 @@
         # Commit the changes to the database in one transaction
         self.db.commit_session()
 
     def process_group(self, data: Any, group_by_rank: str, rank_name: str) -> None:
         """
         Process a group of data for a given taxonomic level and update the database.
 
-        Parameters:
+        Args:
             data (pd.DataFrame): The DataFrame containing the data to process.
             group_by_rank (str): The field to group the data by.
             rank_name (str): The name of the taxonomic rank to process.
         """
         # Define the calculations to perform for each field
         calculations: Dict[
             str,
@@ -293,24 +297,31 @@
             ].apply(lambda x: (x.astype(str).str.lower() == "true").sum())
 
             # Process and update Taxon objects with the calculated metrics
             for taxon_id, metrics in grouped_data.iterrows():
                 self.update_taxon(taxon_id, metrics)
 
             # Extract the coordinates from the filtered data
-            coordinates = self.extract_coordinates(filtered_data)
-
-            geo_json = {"type": "MultiPoint", "coordinates": coordinates}
+            # coordinates = self.extract_coordinates(filtered_data)
 
+            # geo_json = {"type": "MultiPoint", "coordinates": coordinates}
 
     def calculate_frequencies(
         self, taxon_id: int, group_data: Any
     ) -> dict[str, dict[str, float]]:
         """
         Calculate the frequencies for various measurements for a given taxon.
+
+        Args:
+            taxon_id (int): The identifier of the Taxon to be updated.
+            group_data (Any): The dataset containing the group data.
+
+        Returns:
+            dict[str, dict[str, float]]: A dictionary containing the frequencies of the field data categories as percentages.
+            The keys are the left endpoints of the intervals and the values are the percentages.
         """
         frequencies = {}
 
         dbh_bins = [10, 20, 30, 40, 50, 75, 100, 200, 300, 400, 500]
         elevation_bins = [
             100,
             200,
@@ -380,15 +391,15 @@
 
         return frequencies
 
     def update_taxon(self, taxon_id: int, update_data: Dict[str, Any]) -> None:
         """
         Update a Taxon object in the database with provided data.
 
-        Parameters:
+        Args:
             taxon_id (int): The identifier of the Taxon to be updated.
             update_data (dict): The data to update the Taxon with.
         """
         # Fetch the Taxon object from the database
         taxon = self.db.session.query(TaxonRef).filter_by(id_taxonref=taxon_id).first()
 
         if taxon:
@@ -402,15 +413,15 @@
             logger.error(f"Taxon with id {taxon_id} not found in the database.")
 
     @staticmethod
     def extract_coordinates(filtered_data: Any) -> List[List[float]]:
         """
         Extract geographic coordinates from the filtered data.
 
-        Parameters:
+        Args:
             filtered_data (pd.DataFrame): The DataFrame containing the filtered data.
 
         Returns:
             list: A list of coordinates.
         """
 
         # This code returns a list of coordinates. For each point in the 'geo_pt' column of the filtered_data DataFrame,
@@ -423,15 +434,15 @@
             if pd.notna(point)  # Check that the point is not NaN
         ]
 
     def get_unique_ids(self, field_name: str) -> List[int]:
         """
         Retrieve unique identifiers for a specified field from the database.
 
-        Parameters:
+        Args:
             field_name (str): The field name to retrieve unique identifiers for.
 
         Returns:
             List[int]: A list of unique identifiers.
         """
         query = self.db.session.query(getattr(TaxonRef, field_name)).distinct()
         unique_ids = [record[0] for record in query.all() if record[0] is not None]
@@ -516,29 +527,63 @@
                 pheno_fruit[month] = round(fruit_count / total_count * 100)
 
         return pheno_flower, pheno_fruit
 
     def calculate_direct_distribution(
         self, data: Any, value_bins: List[int]
     ) -> dict[str, float]:
+        """
+        Calculate the distribution of values directly from the data.
+
+        Args:
+            data (Any): The dataset containing the data.
+            value_bins (List[int]): The list of bins to categorize the data.
+
+        Returns:
+            dict[str, float]: A dictionary containing the distribution of values as percentages.
+            The keys are the left endpoints of the intervals and the values are the percentages.
+        """
         filtered_values = data.dropna().tolist()
 
         return self.calculate_distribution(filtered_values, value_bins)
 
     def calculate_raster_distribution(
         self, geo_points: Any, value_bins: List[int], raster_path: str
     ) -> dict[str, float]:
+        """
+        Calculate the distribution of values from a raster file.
+
+        Args:
+            geo_points (Any): The geographic points to extract the values from.
+            value_bins (List[int]): The list of bins to categorize the data.
+            raster_path (str): The path to the raster file.
+
+        Returns:
+            dict[str, float]: A dictionary containing the distribution of values as percentages.
+            The keys are the left endpoints of the intervals and the values are the percentages.
+        """
         raster_values = self.extract_raster_values(geo_points, raster_path)
         filtered_values = [value for value in raster_values if value is not None]
 
         return self.calculate_distribution(filtered_values, value_bins)
 
     def calculate_distribution(
         self, values: List[float], value_bins: List[int]
     ) -> dict[str, float]:
+        """
+        Calculate the distribution of values.
+
+        Args:
+            values (List[float]): The list of values.
+            value_bins (List[int]): The list of bins to categorize the values.
+
+        Returns:
+            dict[str, float]: A dictionary containing the distribution of values as percentages.
+            The keys are the left endpoints of the intervals and the values are the percentages.
+        """
         total_count = len(values)
         percentages_per_interval = {}
 
         previous_bin_edge = 0
         for bin_edge in value_bins:
             count_in_interval = sum(
                 previous_bin_edge < value <= bin_edge for value in values
@@ -553,15 +598,24 @@
 
             previous_bin_edge = bin_edge
 
         return percentages_per_interval
 
     @staticmethod
     def extract_raster_values(geo_points: Any, raster_path: str) -> Any:
-        """Extract values for given geo points from a raster file."""
+        """
+        Extract values for given geo points from a raster file.
+
+        Args:
+            geo_points (Any): The geographic points to extract the values from.
+            raster_path (str): The path to the raster file.
+
+        Returns:
+            pd.Series: A pandas Series containing the extracted raster values.
+        """
         raster_values = pd.Series([None] * len(geo_points))
 
         try:
             with rasterio.open(raster_path) as raster:
                 transformer = Transformer.from_crs(
                     "epsg:4326", raster.crs, always_xy=True
                 )
```

### Comparing `niamoto-0.0.2a1/src/niamoto/core/utils/csv_utils.py` & `niamoto-0.0.3a1/src/niamoto/core/utils/csv_utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,19 +3,19 @@
 from loguru import logger
 
 
 def analyze_csv_data_types(csv_file: str) -> List[Tuple[str, str]]:
     """
     Analyze the data types of columns in a CSV file.
 
-    Parameters:
-    csv_file (str): Path to the CSV file to be analyzed.
+    Args:
+        csv_file (str): Path to the CSV file to be analyzed.
 
     Returns:
-    List[Tuple[str, str]]: A list of tuples with column names and types.
+        List[Tuple[str, str]]: A list of tuples with column names and types.
     """
 
     try:
         con = duckdb.connect()
         con.execute(
             f"CREATE TEMPORARY TABLE temp_csv AS SELECT * FROM READ_CSV_AUTO('{csv_file}')"
         )
@@ -27,19 +27,19 @@
         raise ValueError("Unable to analyze CSV file") from e
 
 
 def is_duckdb_type_numeric(duckdb_type: str) -> bool:
     """
     Check if a DuckDB data type is numeric.
 
-    Parameters:
-    duckdb_type (str): The data type of the column in DuckDB.
+    Args:
+        duckdb_type (str): The data type of the column in DuckDB.
 
     Returns:
-    bool: True if the type is numeric, False otherwise.
+        bool: True if the type is numeric, False otherwise.
     """
     numeric_types = [
         "TINYINT",
         "SMALLINT",
         "INTEGER",
         "BIGINT",
         "HUGEINT",
```

### Comparing `niamoto-0.0.2a1/src/niamoto/publish/static_site_generator/page_generator.py` & `niamoto-0.0.3a1/src/niamoto/publish/static_site_generator/page_generator.py`

 * *Files 20% similar despite different names*

```diff
@@ -7,14 +7,18 @@
 import rjsmin  # type: ignore
 
 from niamoto.core.models import TaxonRef
 from niamoto.common.config import Config
 
 
 class PageGenerator:
+    """
+    The PageGenerator class provides methods to generate static webpages for taxons.
+    """
+
     def __init__(self, config: Config) -> None:
         """
         Initializes the PageGenerator class with configuration settings.
 
         Args:
              config (Config): An instance of ConfigManager containing configuration settings.
 
@@ -29,27 +33,27 @@
 
         self.template_dir = os.path.join(
             os.path.dirname(os.path.abspath(__file__)), "templates"
         )
         self.static_src_dir = os.path.join(
             os.path.dirname(os.path.abspath(__file__)), "static"
         )
-        self.output_dir = self.config.get("web", "static_pages")
+        self.output_dir = self.config.get("outputs", "static_pages")
 
         template_loader = jinja2.FileSystemLoader(searchpath=self.template_dir)
         self.template_env = jinja2.Environment(loader=template_loader)
 
     def generate_taxon_page(
         self, taxon: TaxonRef, stats: Optional[Any], mapping: Dict[Any, Any]
     ) -> str:
         """
         Generates a webpage for a given taxon object.
 
         Args:
-            taxon (TaxonRef): The taxon object for which the webpage is generated.
+            taxon (niamoto.core.models.models.TaxonRef): The taxon object for which the webpage is generated.
             stats (dict, optional): A dictionary containing statistics for the taxon.
             mapping (dict): The mapping dictionary containing the configuration for generating the webpage.
 
         Returns:
             str: The path of the generated webpage.
         """
         template = self.template_env.get_template("taxon_template.html")
@@ -61,35 +65,60 @@
         output_path = os.path.join(taxon_output_dir, f"{taxon.id}.html")
         with open(output_path, "w") as file:
             file.write(html_output)
         self.copy_static_files()
         return output_path
 
     def generate_taxonomy_tree_js(self, taxons: List[TaxonRef]) -> None:
+        """
+        Generates a JavaScript file containing the taxonomy tree data.
+
+        Args:
+            taxons (List[niamoto.core.models.models.TaxonRef]): A list of taxon objects.
+        """
         tree = self.build_taxonomy_tree(taxons)
         js_content = "const taxonomyData = " + json.dumps(tree, indent=4) + ";"
         minified_js = rjsmin.jsmin(js_content)
 
         js_path = os.path.join(self.output_dir, "js", "taxonomy_tree.js")
         with open(js_path, "w") as file:
             file.write(minified_js)
 
     def build_taxonomy_tree(self, taxons: List[TaxonRef]) -> List[Dict[Any, Any]]:
+        """
+        Builds a taxonomy tree from a list of taxon objects.
+
+        Args:
+            taxons (List[niamoto.core.models.models.TaxonRef]): A list of taxon objects.
+
+        Returns:
+            List[Dict[Any, Any]]: A list of dictionaries representing the taxonomy tree.
+        """
         taxons_by_id = {int(taxon.id): taxon for taxon in taxons}
         tree = []
 
         for taxon in taxons:
             if taxon.parent_id is None:
                 tree.append(self.build_subtree(taxon, taxons_by_id))
 
         return tree
 
     def build_subtree(
         self, taxon: TaxonRef, taxons_by_id: Dict[int, TaxonRef]
     ) -> Dict[str, Any]:
+        """
+        Builds a subtree for a given taxon object.
+
+        Args:
+            taxon (niamoto.core.models.models.TaxonRef): The taxon object for which the subtree is built.
+            taxons_by_id (Dict[int, niamoto.core.models.models.TaxonRef]): A dictionary mapping taxon IDs to taxon objects.
+
+        Returns:
+            Dict[str, Any]: A dictionary representing the subtree.
+        """
         node: Dict[str, Any] = {
             "id": taxon.id,
             "name": taxon.full_name,
             "children": [],
         }
 
         left = taxon.lft
@@ -103,16 +132,14 @@
                 node["children"].append(self.build_subtree(child_taxon, taxons_by_id))
 
         return node
 
     def copy_static_files(self) -> None:
         """
         Copies static files to the destination directory, overwriting existing files.
-
-        The destination directory is created if it doesn't exist.
         """
         # Create the destination directory if it does not exist
         os.makedirs(self.output_dir, exist_ok=True)
 
         # Copy each item in the source directory
         for item in os.listdir(self.static_src_dir):
             src_path = os.path.join(self.static_src_dir, item)
@@ -125,15 +152,15 @@
                 shutil.copy2(src_path, dest_path)
 
     def taxon_to_dict(self, taxon: TaxonRef, stats: Optional[Any]) -> dict[str, Any]:
         """
         Converts a TaxonRef object and its associated statistics to a dictionary.
 
         Args:
-            taxon (TaxonRef): A TaxonRef object.
+            taxon (niamoto.core.models.models.TaxonRef): A TaxonRef object.
             stats (dict, optional): A dictionary containing statistics for the taxon.
 
         Returns:
             dict[str, Any]: A dictionary representing the taxon data and its statistics.
         """
         taxon_dict = {
             "id": taxon.id,
```

### Comparing `niamoto-0.0.2a1/src/niamoto/publish/static_site_generator/static/js/index.js` & `niamoto-0.0.3a1/src/niamoto/publish/static_site_generator/static/js/index.js`

 * *Files identical despite different names*

### Comparing `niamoto-0.0.2a1/src/niamoto/publish/static_site_generator/static/js/vendor/chart/4.4.2_chart.js` & `niamoto-0.0.3a1/src/niamoto/publish/static_site_generator/static/js/vendor/chart/4.4.2_chart.js`

 * *Files identical despite different names*

### Comparing `niamoto-0.0.2a1/src/niamoto/publish/static_site_generator/static/js/vendor/d3/7.8.5_d3.js` & `niamoto-0.0.3a1/src/niamoto/publish/static_site_generator/static/js/vendor/d3/7.8.5_d3.js`

 * *Files identical despite different names*

### Comparing `niamoto-0.0.2a1/src/niamoto/publish/static_site_generator/static/js/vendor/jquery/3.6.0_jquery.js` & `niamoto-0.0.3a1/src/niamoto/publish/static_site_generator/static/js/vendor/jquery/3.6.0_jquery.js`

 * *Files identical despite different names*

### Comparing `niamoto-0.0.2a1/src/niamoto/publish/static_site_generator/static/js/vendor/justgage/1.6.1_justgage.js` & `niamoto-0.0.3a1/src/niamoto/publish/static_site_generator/static/js/vendor/justgage/1.6.1_justgage.js`

 * *Files identical despite different names*

### Comparing `niamoto-0.0.2a1/src/niamoto/publish/static_site_generator/static/js/vendor/leaflet/1.9.4_leaflet.css` & `niamoto-0.0.3a1/src/niamoto/publish/static_site_generator/static/js/vendor/leaflet/1.9.4_leaflet.css`

 * *Files identical despite different names*

### Comparing `niamoto-0.0.2a1/src/niamoto/publish/static_site_generator/static/js/vendor/leaflet/1.9.4_leaflet.js` & `niamoto-0.0.3a1/src/niamoto/publish/static_site_generator/static/js/vendor/leaflet/1.9.4_leaflet.js`

 * *Files identical despite different names*

### Comparing `niamoto-0.0.2a1/src/niamoto/publish/static_site_generator/static/js/vendor/leaflet/images/layers-2x.png` & `niamoto-0.0.3a1/src/niamoto/publish/static_site_generator/static/js/vendor/leaflet/images/layers-2x.png`

 * *Files identical despite different names*

### Comparing `niamoto-0.0.2a1/src/niamoto/publish/static_site_generator/static/js/vendor/leaflet/images/layers.png` & `niamoto-0.0.3a1/src/niamoto/publish/static_site_generator/static/js/vendor/leaflet/images/layers.png`

 * *Files identical despite different names*

### Comparing `niamoto-0.0.2a1/src/niamoto/publish/static_site_generator/static/js/vendor/leaflet/images/marker-icon-2x.png` & `niamoto-0.0.3a1/src/niamoto/publish/static_site_generator/static/js/vendor/leaflet/images/marker-icon-2x.png`

 * *Files identical despite different names*

### Comparing `niamoto-0.0.2a1/src/niamoto/publish/static_site_generator/static/js/vendor/leaflet/images/marker-icon.png` & `niamoto-0.0.3a1/src/niamoto/publish/static_site_generator/static/js/vendor/leaflet/images/marker-icon.png`

 * *Files identical despite different names*

### Comparing `niamoto-0.0.2a1/src/niamoto/publish/static_site_generator/static/js/vendor/leaflet/images/marker-shadow.png` & `niamoto-0.0.3a1/src/niamoto/publish/static_site_generator/static/js/vendor/leaflet/images/marker-shadow.png`

 * *Files identical despite different names*

### Comparing `niamoto-0.0.2a1/src/niamoto/publish/static_site_generator/static/js/vendor/raphael/2.3.0_raphael.js` & `niamoto-0.0.3a1/src/niamoto/publish/static_site_generator/static/js/vendor/raphael/2.3.0_raphael.js`

 * *Files identical despite different names*

### Comparing `niamoto-0.0.2a1/src/niamoto/publish/static_site_generator/static/js/vendor/tailwindcss/2.2.19_dist_tailwind.css` & `niamoto-0.0.3a1/src/niamoto/publish/static_site_generator/static/js/vendor/tailwindcss/2.2.19_dist_tailwind.css`

 * *Files identical despite different names*

### Comparing `niamoto-0.0.2a1/src/niamoto/publish/static_site_generator/templates/taxon_template.html` & `niamoto-0.0.3a1/src/niamoto/publish/static_site_generator/templates/taxon_template.html`

 * *Files identical despite different names*

### Comparing `niamoto-0.0.2a1/PKG-INFO` & `niamoto-0.0.3a1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: niamoto
-Version: 0.0.2a1
+Version: 0.0.3a1
 Summary: 
 Home-page: https://github.com/niamoto/niamoto
 License: GPL-3.0-or-later
 Keywords: niamoto
 Author: Julien Barbe
 Author-email: julien.barbe@me.com
 Requires-Python: >=3.9,<3.12
@@ -29,24 +29,27 @@
 Requires-Dist: duckdb (>=0.10.1,<0.11.0)
 Requires-Dist: duckdb-engine (>=0.12.0,<0.13.0)
 Requires-Dist: flask (>=3.0.0,<4.0.0)
 Requires-Dist: geoalchemy2 (>=0.15.0,<0.16.0)
 Requires-Dist: geopandas (>=0.14.1,<0.15.0)
 Requires-Dist: leafmap (>=0.31.5,<0.32.0)
 Requires-Dist: loguru (>=0.7.2,<0.8.0)
+Requires-Dist: myst-parser (>=3.0.1,<4.0.0)
 Requires-Dist: numpy (>=1.26.1,<2.0.0)
 Requires-Dist: pandas (>=2.2.1,<3.0.0)
 Requires-Dist: prompt-toolkit (>=3.0.43,<4.0.0)
 Requires-Dist: pyarrow (==16.0.0)
 Requires-Dist: pyproj (>=3.6.1,<4.0.0)
 Requires-Dist: pyyaml (>=6.0.1,<7.0.0)
 Requires-Dist: rasterio (>=1.3.9,<2.0.0)
 Requires-Dist: rich (>=13.7.1,<14.0.0)
 Requires-Dist: rjsmin (>=1.2.2,<2.0.0)
 Requires-Dist: shapely (>=2.0.3,<3.0.0)
+Requires-Dist: sphinx-markdown-builder (>=0.6.6,<0.7.0)
+Requires-Dist: sphinxcontrib-napoleon (>=0.7,<0.8)
 Requires-Dist: sqlalchemy[mypy] (>=2.0.29,<3.0.0)
 Requires-Dist: tabulate (>=0.9.0,<0.10.0)
 Project-URL: Documentation, https://github.com/niamoto/niamoto#readme
 Project-URL: Repository, https://github.com/niamoto/niamoto
 Description-Content-Type: text/markdown
 
 
@@ -97,54 +100,45 @@
 
 ```
 niamoto init
 ```
 
 This command will create the default configuration necessary for Niamoto to operate. Use the `--reset` option to reset the environment if it already exists.
 
-## Available Commands
-
-| Command                 | Description                                                                                                             |
-|-------------------------|-------------------------------------------------------------------------------------------------------------------------|
-| init                    | Initialize or reset the Niamoto environment.                                                                            |
-| import-taxonomy         | Import taxonomy data from a CSV file into the database.                                                                 |
-| import-plots            | Import plot data from a GeoPackage file into the plot_ref table.                                                        |
-| import-occurrences      | Import occurrence data from a CSV file, analyze it to update the 'mapping' table, and link occurrences to their taxons. |
-| import-occurrence-plots | Import occurrence-plot links from a CSV file.                                                                           |
-| generate-mapping        | Generate a mapping from a CSV file based on the specified grouping criteria.                                            |
-| calculate-statistics    | Calculate statistics based on the mapping file specified in the configuration.                                          |
-| generate-static-site    | Generate static web pages for each taxon in the database.                                                               |
-| generate-taxonomy-stats | Generate a taxonomy tree, calculate statistics, and write the taxon table from a CSV file.                              |
-
 
 ## Development Environment Configuration
 
 To set up a development environment for Niamoto, you must have `Poetry` installed on your system. Poetry is a dependency management and packaging tool for Python.
 
 1. **Poetry Installation**:
-   To install Poetry, run the following command:
-   ```bash
-   curl -sSL https://raw.githubusercontent.com/python-poetry/poetry/master/get-poetry.py | python -
-   ```
 
+  To install Poetry, run the following command:
+
+  ```bash
+  curl -sSL https://raw.githubusercontent.com/python-poetry/poetry/master/get-poetry.py | python -
+  ```
 
 2. **Clone the Niamoto repository**:
+
   Clone the Niamoto repository on your system using `git`:
+
   ```bash
   git clone https://github.com/niamoto/niamoto.git
   ```
 
 3. **Configure the development environment with Poetry**:
+
   Move into the cloned directory and install the dependencies with Poetry:
   ```bash
   cd niamoto
   poetry install
   ```
 
 4. **Activate the virtual environment**:
+
   Activate the virtual environment created by Poetry:
   ```bash
   poetry shell
   ```
 
 5. **Editable Installation**:
 
@@ -178,63 +172,73 @@
 **Command:**
 ```bash
 $ niamoto init [--reset]
 ```
 **Explanation:**
 Initializes or resets the Niamoto environment. Use the `--reset` option to reset the environment if it already exists, clearing all data and configurations to start fresh.
 
-#### 2. Import Taxonomy Data
+#### 2. Import All Data
+**Command:**
+```bash
+$ niamoto import-all
+```
+
+**Explanation:**
+Imports all data from CSV files and GeoPackage files into the database. This command is a shortcut to import taxonomy, plot, occurrences, and occurrence-plot links data in one go.
+Assuming the following files are present in the current source directory and specified in the configuration file
+
+#### 3. Import Taxonomy Data
 **Command:**
 ```bash
 $ niamoto import-taxonomy <csvfile> [--ranks <ranks>]
 ```
 **Explanation:**
 Imports taxonomy data from a specified CSV file. The `--ranks` option allows specifying the order of taxonomic ranks as they appear in the CSV file.
 
-#### 3. Import Plot Data
+#### 4. Import Plot Data
 **Command:**
 ```bash
 $ niamoto import-plots <gpkg_file>
 ```
 **Explanation:**
 Imports plot data from a GeoPackage file into the database, which should contain plot geometries and associated attributes.
 
-#### 4. Import Occurrences Data
+#### 5. Import Occurrences Data
 **Command:**
 ```bash
 $ niamoto import-occurrences <csvfile> --taxon-id-column <column_name>
 ```
 **Explanation:**
 Imports occurrences data from a CSV file. The `--taxon-id-column` option specifies the CSV column containing the taxon IDs needed to link occurrences to taxons.
 
-#### 5. Import Occurrence-Plot Links
+#### 6. Import Occurrence-Plot Links
 **Command:**
 ```bash
 $ niamoto import-occurrence-plots <csvfile>
 ```
 **Explanation:**
 Imports links between occurrences and plots from a CSV file, establishing relational data within the database.
 
-#### 6. Generate Mapping
+#### 7. Generate Mapping
 **Command:**
 ```bash
 $ niamoto generate-mapping --data-source <csv_file> --mapping-group <group> [--reference-table-name <table_name> --reference-data-path <path>]
 ```
 **Explanation:**
 Generates mappings from a CSV file based on specified grouping criteria. Optional parameters allow linking to reference data for enhanced mapping accuracy.
 
-#### 7. Calculate Statistics
+#### 8. Calculate Statistics
 **Command:**
 ```bash
 $ niamoto calculate-statistics [--mapping-group <group> --csv-file <file>]
 ```
 **Explanation:**
 Calculates statistics based on the provided mapping file and optional group or CSV file specifics.
 
-#### 8. Generate Static Site
+#### 9. Generate Static Site
 **Command:**
 ```bash
 $ niamoto generate-static-site
 ```
 **Explanation:**
 Generates a static website for each taxon in the database, providing a visual and informational representation of taxonomic data.
 
@@ -268,14 +272,15 @@
   - `chart_type`: The type of chart to generate for the bins (e.g., "bar").
   - `chart_options`: Specific options for the bin chart (e.g., "title", "color").
 - `is_identifier`: Indicates whether the field is an identifier (boolean value).
 - `display_order`: The display order of the field in the interface.
 
 #### Special Fields
 Some fields may have specific configurations depending on their `target_field` and `field_type`:
+
 - **Calculated field** (e.g., total number of occurrences):
   - `target_field`: null
   - `field_type`: "INTEGER"
   - `transformations`: Must contain a "count" type transformation
 - **Boolean field** (e.g., occurrence on a particular substrate):
   - `target_field`: The name of the boolean field in the occurrences table
   - `field_type`: "BOOLEAN"
@@ -289,14 +294,15 @@
 
 #### 1. **JSON Style Notation:**
 
 ```yaml
 transformations:
   - {"name": "max", "chart_type": "gauge", "chart_options": {"max": 40, "title": "Maximum", "label": "units"}}
 ```
+
 #### 1. **Standard YAML Style Notation:**
 This format will display both YAML notations under a single Markdown box, keeping the explanation compact and the code examples clear and easy to compare.
 
 ```yaml
 transformations:
   - name: max
     chart_type: gauge
```

