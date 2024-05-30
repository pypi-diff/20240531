# Comparing `tmp/opengamedata_core-0.0.5.tar.gz` & `tmp/opengamedata_core-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opengamedata_core-0.0.5.tar", last modified: Fri May 17 03:40:41 2024, max compression
+gzip compressed data, was "opengamedata_core-0.0.6.tar", last modified: Thu May 30 18:05:05 2024, max compression
```

## Comparing `opengamedata_core-0.0.5.tar` & `opengamedata_core-0.0.6.tar`

### file list

```diff
@@ -1,546 +1,560 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:40:41.360147 opengamedata_core-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4796 2024-05-17 03:40:41.360147 opengamedata_core-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3900 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 03:40:41.360147 opengamedata_core-0.0.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:40:41.268148 opengamedata_core-0.0.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:40:41.272148 opengamedata_core-0.0.5/src/ogd/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:40:41.272148 opengamedata_core-0.0.5/src/ogd/core/
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:40:41.272148 opengamedata_core-0.0.5/src/ogd/core/exec/
--rw-r--r--   0 runner    (1001) docker     (127)     9329 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/core/exec/Commands.py
--rw-r--r--   0 runner    (1001) docker     (127)     3763 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/core/exec/Generators.py
--rw-r--r--   0 runner    (1001) docker     (127)     4858 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/core/exec/Parsers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:40:41.260148 opengamedata_core-0.0.5/src/ogd/core/games/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:40:41.260148 opengamedata_core-0.0.5/src/ogd/core/games/AQUALAB/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:40:41.272148 opengamedata_core-0.0.5/src/ogd/core/games/AQUALAB/features/
--rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/core/games/AQUALAB/features/AppVersions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4209 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/core/games/AQUALAB/features/PlayLocations.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:40:41.260148 opengamedata_core-0.0.5/src/ogd/core/games/JOURNALISM/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:40:41.272148 opengamedata_core-0.0.5/src/ogd/core/games/JOURNALISM/features/
--rw-r--r--   0 runner    (1001) docker     (127)     2899 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/core/games/JOURNALISM/features/FailureAttributes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1907 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/core/games/JOURNALISM/features/FinalAttributes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:40:41.272148 opengamedata_core-0.0.5/src/ogd/core/generators/
--rw-r--r--   0 runner    (1001) docker     (127)     7941 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/core/generators/Generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     5136 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/core/generators/GeneratorLoader.py
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/core/generators/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:40:41.272148 opengamedata_core-0.0.5/src/ogd/core/generators/detectors/
--rw-r--r--   0 runner    (1001) docker     (127)     4351 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/core/generators/detectors/Detector.py
--rw-r--r--   0 runner    (1001) docker     (127)     2300 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/core/generators/detectors/DetectorEvent.py
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/core/generators/detectors/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:40:41.276148 opengamedata_core-0.0.5/src/ogd/core/generators/extractors/
--rw-r--r--   0 runner    (1001) docker     (127)     6499 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/core/generators/extractors/Extractor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/core/generators/extractors/Feature.py
--rw-r--r--   0 runner    (1001) docker     (127)     1585 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/core/generators/extractors/PerCountFeature.py
--rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/core/generators/extractors/PerLevelFeature.py
--rw-r--r--   0 runner    (1001) docker     (127)      804 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/core/generators/extractors/SessionFeature.py
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/core/generators/extractors/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:40:41.276148 opengamedata_core-0.0.5/src/ogd/core/generators/legacy/
--rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/core/generators/legacy/LegacyDetector.py
--rw-r--r--   0 runner    (1001) docker     (127)    14632 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/core/generators/legacy/LegacyFeature.py
--rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/core/generators/legacy/LegacyLoader.py
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/core/generators/legacy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:40:41.276148 opengamedata_core-0.0.5/src/ogd/core/generators/registries/
--rw-r--r--   0 runner    (1001) docker     (127)     8364 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/core/generators/registries/DetectorRegistry.py
--rw-r--r--   0 runner    (1001) docker     (127)    13799 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/core/generators/registries/ExtractorRegistry.py
--rw-r--r--   0 runner    (1001) docker     (127)     5276 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/core/generators/registries/GeneratorRegistry.py
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/core/generators/registries/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:40:41.280148 opengamedata_core-0.0.5/src/ogd/core/interfaces/
--rw-r--r--   0 runner    (1001) docker     (127)    10850 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/core/interfaces/BQFirebaseInterface.py
--rw-r--r--   0 runner    (1001) docker     (127)     9699 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/core/interfaces/BigQueryCodingInterface.py
--rw-r--r--   0 runner    (1001) docker     (127)    11865 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/core/interfaces/BigQueryInterface.py
--rw-r--r--   0 runner    (1001) docker     (127)     4903 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/core/interfaces/CSVInterface.py
--rw-r--r--   0 runner    (1001) docker     (127)     3519 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/core/interfaces/CodingInterface.py
--rw-r--r--   0 runner    (1001) docker     (127)     5432 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/core/interfaces/DataInterface.py
--rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/core/interfaces/Interface.py
--rw-r--r--   0 runner    (1001) docker     (127)    23918 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/core/interfaces/MySQLInterface.py
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/core/interfaces/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:40:41.280148 opengamedata_core-0.0.5/src/ogd/core/interfaces/outerfaces/
--rw-r--r--   0 runner    (1001) docker     (127)     5824 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/core/interfaces/outerfaces/DataOuterface.py
--rw-r--r--   0 runner    (1001) docker     (127)     4195 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/core/interfaces/outerfaces/DebugOuterface.py
--rw-r--r--   0 runner    (1001) docker     (127)     4902 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/core/interfaces/outerfaces/DictionaryOuterface.py
--rw-r--r--   0 runner    (1001) docker     (127)    33757 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/core/interfaces/outerfaces/TSVOuterface.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:40:41.280148 opengamedata_core-0.0.5/src/ogd/core/managers/
--rw-r--r--   0 runner    (1001) docker     (127)     3513 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/core/managers/EventManager.py
--rw-r--r--   0 runner    (1001) docker     (127)    19007 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/core/managers/ExportManager.py
--rw-r--r--   0 runner    (1001) docker     (127)    12108 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/core/managers/FeatureManager.py
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/core/managers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:40:41.284148 opengamedata_core-0.0.5/src/ogd/core/processors/
--rw-r--r--   0 runner    (1001) docker     (127)     6040 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/core/processors/ClassroomDetector.py
--rw-r--r--   0 runner    (1001) docker     (127)     2239 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/core/processors/DetectorProcessor.py
--rw-r--r--   0 runner    (1001) docker     (127)      964 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/core/processors/EventProcessor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/core/processors/ExtractorProcessor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2628 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/core/processors/GeneratorProcessor.py
--rw-r--r--   0 runner    (1001) docker     (127)     4602 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/core/processors/PlayerProcessor.py
--rw-r--r--   0 runner    (1001) docker     (127)     4215 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/core/processors/PopulationProcessor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1878 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/core/processors/Processor.py
--rw-r--r--   0 runner    (1001) docker     (127)     4267 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/core/processors/SessionProcessor.py
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/core/processors/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:40:41.284148 opengamedata_core-0.0.5/src/ogd/core/requests/
--rw-r--r--   0 runner    (1001) docker     (127)     5301 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/core/requests/Request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2062 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/core/requests/RequestResult.py
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/core/requests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:40:41.284148 opengamedata_core-0.0.5/src/ogd/core/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)    14401 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/core/schemas/Event.py
--rw-r--r--   0 runner    (1001) docker     (127)      213 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/core/schemas/ExportMode.py
--rw-r--r--   0 runner    (1001) docker     (127)      364 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/core/schemas/ExtractionMode.py
--rw-r--r--   0 runner    (1001) docker     (127)     1426 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/core/schemas/FeatureData.py
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/core/schemas/IDMode.py
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/core/schemas/IterationMode.py
--rw-r--r--   0 runner    (1001) docker     (127)     1427 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/core/schemas/Schema.py
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/core/schemas/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:40:41.284148 opengamedata_core-0.0.5/src/ogd/core/schemas/configs/
--rw-r--r--   0 runner    (1001) docker     (127)    10898 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/core/schemas/configs/ConfigSchema.py
--rw-r--r--   0 runner    (1001) docker     (127)     5835 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/core/schemas/configs/GameSourceSchema.py
--rw-r--r--   0 runner    (1001) docker     (127)     3452 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/core/schemas/configs/IndexingSchema.py
--rw-r--r--   0 runner    (1001) docker     (127)     2593 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/core/schemas/configs/LegacyConfigSchema.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:40:41.284148 opengamedata_core-0.0.5/src/ogd/core/schemas/configs/data_sources/
--rw-r--r--   0 runner    (1001) docker     (127)     3048 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/core/schemas/configs/data_sources/BigQuerySourceSchema.py
--rw-r--r--   0 runner    (1001) docker     (127)     1806 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/core/schemas/configs/data_sources/DataSourceSchema.py
--rw-r--r--   0 runner    (1001) docker     (127)      577 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/core/schemas/configs/data_sources/FileSourceSchema.py
--rw-r--r--   0 runner    (1001) docker     (127)    10140 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/core/schemas/configs/data_sources/MySQLSourceSchema.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:40:41.288148 opengamedata_core-0.0.5/src/ogd/core/schemas/games/
--rw-r--r--   0 runner    (1001) docker     (127)      922 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/core/schemas/games/AggregateSchema.py
--rw-r--r--   0 runner    (1001) docker     (127)     5168 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/core/schemas/games/DataElementSchema.py
--rw-r--r--   0 runner    (1001) docker     (127)     5045 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/core/schemas/games/DetectorMapSchema.py
--rw-r--r--   0 runner    (1001) docker     (127)      801 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/core/schemas/games/DetectorSchema.py
--rw-r--r--   0 runner    (1001) docker     (127)     3996 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/core/schemas/games/EventSchema.py
--rw-r--r--   0 runner    (1001) docker     (127)     4006 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/core/schemas/games/ExtractorSchema.py
--rw-r--r--   0 runner    (1001) docker     (127)     5656 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/core/schemas/games/FeatureMapSchema.py
--rw-r--r--   0 runner    (1001) docker     (127)     4869 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/core/schemas/games/FeatureSchema.py
--rw-r--r--   0 runner    (1001) docker     (127)    26726 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/core/schemas/games/GameSchema.py
--rw-r--r--   0 runner    (1001) docker     (127)     2652 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/core/schemas/games/GameStateSchema.py
--rw-r--r--   0 runner    (1001) docker     (127)     2831 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/core/schemas/games/PerCountSchema.py
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/core/schemas/games/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:40:41.288148 opengamedata_core-0.0.5/src/ogd/core/schemas/table_schemas/
--rw-r--r--   0 runner    (1001) docker     (127)     3615 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/core/schemas/table_schemas/BIGQUERY.json
--rw-r--r--   0 runner    (1001) docker     (127)     4890 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/core/schemas/table_schemas/FIELDDAY_MYSQL.json
--rw-r--r--   0 runner    (1001) docker     (127)     2573 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/core/schemas/table_schemas/FIREBASE.json
--rw-r--r--   0 runner    (1001) docker     (127)     4430 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/core/schemas/table_schemas/MASHOPOLIS_MYSQL.json
--rw-r--r--   0 runner    (1001) docker     (127)     3685 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/core/schemas/table_schemas/OGD_EVENT_FILE.json
--rw-r--r--   0 runner    (1001) docker     (127)     4077 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/core/schemas/table_schemas/OPENGAMEDATA_BIGQUERY.json
--rw-r--r--   0 runner    (1001) docker     (127)     4477 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/core/schemas/table_schemas/OPENGAMEDATA_MYSQL.json
--rw-r--r--   0 runner    (1001) docker     (127)     1920 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/core/schemas/table_schemas/SHIPWRECKS.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:40:41.292148 opengamedata_core-0.0.5/src/ogd/core/schemas/tables/
--rw-r--r--   0 runner    (1001) docker     (127)     6782 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/core/schemas/tables/ColumnMapSchema.py
--rw-r--r--   0 runner    (1001) docker     (127)     4174 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/core/schemas/tables/ColumnSchema.py
--rw-r--r--   0 runner    (1001) docker     (127)    23084 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/core/schemas/tables/TableSchema.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:40:41.292148 opengamedata_core-0.0.5/src/ogd/core/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     4567 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/core/utils/Logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     4361 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/core/utils/Readme.py
--rw-r--r--   0 runner    (1001) docker     (127)     6477 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/core/utils/SemanticVersion.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/core/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/core/utils/typing.py
--rw-r--r--   0 runner    (1001) docker     (127)     2692 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/core/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:40:41.292148 opengamedata_core-0.0.5/src/ogd/games/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:40:41.260148 opengamedata_core-0.0.5/src/ogd/games/ALL_YOU_CAN_ET/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:40:41.292148 opengamedata_core-0.0.5/src/ogd/games/ALL_YOU_CAN_ET/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)    20816 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/ALL_YOU_CAN_ET/schemas/ALL_YOU_CAN_ET.json.template
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:40:41.292148 opengamedata_core-0.0.5/src/ogd/games/AQUALAB/
--rw-r--r--   0 runner    (1001) docker     (127)    13543 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/AQUALAB/AqualabLoader.py
--rw-r--r--   0 runner    (1001) docker     (127)   278275 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/AQUALAB/DBExport.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/AQUALAB/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:40:41.296148 opengamedata_core-0.0.5/src/ogd/games/AQUALAB/detectors/
--rw-r--r--   0 runner    (1001) docker     (127)     2320 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/AQUALAB/detectors/CollectFactNoJob.py
--rw-r--r--   0 runner    (1001) docker     (127)     3554 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/AQUALAB/detectors/DiveSiteNoEvidence.py
--rw-r--r--   0 runner    (1001) docker     (127)     1725 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/AQUALAB/detectors/EchoRoomChange.py
--rw-r--r--   0 runner    (1001) docker     (127)     4505 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/AQUALAB/detectors/HintAndLeave.py
--rw-r--r--   0 runner    (1001) docker     (127)     3466 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/AQUALAB/detectors/Idle.py
--rw-r--r--   0 runner    (1001) docker     (127)     3901 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/AQUALAB/detectors/SceneChangeFrequently.py
--rw-r--r--   0 runner    (1001) docker     (127)     3796 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/AQUALAB/detectors/TwoHints.py
--rw-r--r--   0 runner    (1001) docker     (127)      361 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/AQUALAB/detectors/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:40:41.308148 opengamedata_core-0.0.5/src/ogd/games/AQUALAB/features/
--rw-r--r--   0 runner    (1001) docker     (127)     2752 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/AQUALAB/features/ActiveJobs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2332 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/AQUALAB/features/ActiveTime.py
--rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/AQUALAB/features/AppVersions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/AQUALAB/features/AverageSessionTime.py
--rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/AQUALAB/features/EchoSessionID.py
--rw-r--r--   0 runner    (1001) docker     (127)     5318 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/AQUALAB/features/EventList.py
--rw-r--r--   0 runner    (1001) docker     (127)     9513 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/AQUALAB/features/JobActiveTime.py
--rw-r--r--   0 runner    (1001) docker     (127)     2460 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/AQUALAB/features/JobArgumentation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2708 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/AQUALAB/features/JobCompletionTime.py
--rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/AQUALAB/features/JobDiveSitesCount.py
--rw-r--r--   0 runner    (1001) docker     (127)     2138 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/AQUALAB/features/JobDiveTime.py
--rw-r--r--   0 runner    (1001) docker     (127)     2408 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/AQUALAB/features/JobExperimentation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/AQUALAB/features/JobGuideCount.py
--rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/AQUALAB/features/JobHelpCount.py
--rw-r--r--   0 runner    (1001) docker     (127)     3952 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/AQUALAB/features/JobLocationChanges.py
--rw-r--r--   0 runner    (1001) docker     (127)     2279 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/AQUALAB/features/JobModeling.py
--rw-r--r--   0 runner    (1001) docker     (127)     2344 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/AQUALAB/features/JobPlayTime.py
--rw-r--r--   0 runner    (1001) docker     (127)     2119 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/AQUALAB/features/JobPriorAttempt.py
--rw-r--r--   0 runner    (1001) docker     (127)     1943 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/AQUALAB/features/JobPriorComplete.py
--rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/AQUALAB/features/JobStartCount.py
--rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/AQUALAB/features/JobTasksCompleted.py
--rw-r--r--   0 runner    (1001) docker     (127)     1600 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/AQUALAB/features/JobTriesInArgument.py
--rw-r--r--   0 runner    (1001) docker     (127)     6192 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/AQUALAB/features/JobsAttempted.py
--rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/AQUALAB/features/JobsCompleted.py
--rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/AQUALAB/features/ModelExportCount.py
--rw-r--r--   0 runner    (1001) docker     (127)     1299 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/AQUALAB/features/ModelInterveneCount.py
--rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/AQUALAB/features/ModelPredictCount.py
--rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/AQUALAB/features/PerJobFeature.py
--rw-r--r--   0 runner    (1001) docker     (127)     3014 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/AQUALAB/features/PlayerSummary.py
--rw-r--r--   0 runner    (1001) docker     (127)     3351 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/AQUALAB/features/PopulationSummary.py
--rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/AQUALAB/features/RegionJobCount.py
--rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/AQUALAB/features/RegionName.py
--rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/AQUALAB/features/SessionDiveSitesCount.py
--rw-r--r--   0 runner    (1001) docker     (127)     3950 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/AQUALAB/features/SessionDuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/AQUALAB/features/SessionGuideCount.py
--rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/AQUALAB/features/SessionHelpCount.py
--rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/AQUALAB/features/SessionID.py
--rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/AQUALAB/features/SessionJobsCompleted.py
--rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/AQUALAB/features/SwitchJobsCount.py
--rw-r--r--   0 runner    (1001) docker     (127)     2521 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/AQUALAB/features/SyncCompletionTime.py
--rw-r--r--   0 runner    (1001) docker     (127)     1733 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/AQUALAB/features/TankRulesCount.py
--rw-r--r--   0 runner    (1001) docker     (127)     3458 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/AQUALAB/features/TopJobCompletionDestinations.py
--rw-r--r--   0 runner    (1001) docker     (127)     3444 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/AQUALAB/features/TopJobSwitchDestinations.py
--rw-r--r--   0 runner    (1001) docker     (127)     3339 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/AQUALAB/features/TotalArcticTime.py
--rw-r--r--   0 runner    (1001) docker     (127)     2193 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/AQUALAB/features/TotalArgumentationTime.py
--rw-r--r--   0 runner    (1001) docker     (127)     3332 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/AQUALAB/features/TotalBayouTime.py
--rw-r--r--   0 runner    (1001) docker     (127)     3332 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/AQUALAB/features/TotalCoralTime.py
--rw-r--r--   0 runner    (1001) docker     (127)     2794 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/AQUALAB/features/TotalDiveTime.py
--rw-r--r--   0 runner    (1001) docker     (127)     2136 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/AQUALAB/features/TotalExperimentationTime.py
--rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/AQUALAB/features/TotalGuideCount.py
--rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/AQUALAB/features/TotalHelpCount.py
--rw-r--r--   0 runner    (1001) docker     (127)     3325 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/AQUALAB/features/TotalKelpTime.py
--rw-r--r--   0 runner    (1001) docker     (127)     2121 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/AQUALAB/features/TotalModelingTime.py
--rw-r--r--   0 runner    (1001) docker     (127)     2493 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/AQUALAB/features/TotalPlayTime.py
--rw-r--r--   0 runner    (1001) docker     (127)     1440 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/AQUALAB/features/UserAvgActiveTime.py
--rw-r--r--   0 runner    (1001) docker     (127)     1412 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/AQUALAB/features/UserAvgSessionDuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/AQUALAB/features/UserTotalSessionDuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     3093 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/AQUALAB/features/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:40:41.308148 opengamedata_core-0.0.5/src/ogd/games/AQUALAB/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)    32117 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/AQUALAB/schemas/AQUALAB.json.template
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:40:41.260148 opengamedata_core-0.0.5/src/ogd/games/BACTERIA/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:40:41.308148 opengamedata_core-0.0.5/src/ogd/games/BACTERIA/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/BACTERIA/schemas/BACTERIA.json.template
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:40:41.264148 opengamedata_core-0.0.5/src/ogd/games/BALLOON/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:40:41.308148 opengamedata_core-0.0.5/src/ogd/games/BALLOON/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/BALLOON/schemas/BALLOON.json.template
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:40:41.264148 opengamedata_core-0.0.5/src/ogd/games/BLOOM/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:40:41.308148 opengamedata_core-0.0.5/src/ogd/games/BLOOM/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)    21554 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/BLOOM/schemas/BLOOM.json.template
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:40:41.264148 opengamedata_core-0.0.5/src/ogd/games/CENSIO_SLIDE/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:40:41.308148 opengamedata_core-0.0.5/src/ogd/games/CENSIO_SLIDE/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)    11446 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/CENSIO_SLIDE/schemas/CENSIO_SLIDE.json.template
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:40:41.264148 opengamedata_core-0.0.5/src/ogd/games/CENSIO_STACK/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:40:41.308148 opengamedata_core-0.0.5/src/ogd/games/CENSIO_STACK/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)    21742 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/CENSIO_STACK/schemas/CENSIO_STACK.json.template
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:40:41.264148 opengamedata_core-0.0.5/src/ogd/games/CRUSH_STATION/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:40:41.308148 opengamedata_core-0.0.5/src/ogd/games/CRUSH_STATION/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)    11756 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/CRUSH_STATION/schemas/CRUSH_STATION.json.template
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:40:41.308148 opengamedata_core-0.0.5/src/ogd/games/CRYSTAL/
--rw-r--r--   0 runner    (1001) docker     (127)     2380 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/CRYSTAL/CrystalLoader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:40:41.308148 opengamedata_core-0.0.5/src/ogd/games/CRYSTAL/features/
--rw-r--r--   0 runner    (1001) docker     (127)    14123 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/CRYSTAL/features/CrystalExtractor.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/CRYSTAL/features/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:40:41.308148 opengamedata_core-0.0.5/src/ogd/games/CRYSTAL/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)    14066 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/CRYSTAL/schemas/CRYSTAL.json.template
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:40:41.264148 opengamedata_core-0.0.5/src/ogd/games/CYCLE_CARBON/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:40:41.308148 opengamedata_core-0.0.5/src/ogd/games/CYCLE_CARBON/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/CYCLE_CARBON/schemas/CYCLE_CARBON.json.template
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:40:41.264148 opengamedata_core-0.0.5/src/ogd/games/CYCLE_NITROGEN/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:40:41.308148 opengamedata_core-0.0.5/src/ogd/games/CYCLE_NITROGEN/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/CYCLE_NITROGEN/schemas/CYCLE_NITROGEN.json.template
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:40:41.264148 opengamedata_core-0.0.5/src/ogd/games/CYCLE_WATER/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:40:41.308148 opengamedata_core-0.0.5/src/ogd/games/CYCLE_WATER/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/CYCLE_WATER/schemas/CYCLE_WATER.json.template
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:40:41.264148 opengamedata_core-0.0.5/src/ogd/games/EARTHQUAKE/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:40:41.308148 opengamedata_core-0.0.5/src/ogd/games/EARTHQUAKE/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/EARTHQUAKE/schemas/EARTHQUAKE.json.template
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:40:41.264148 opengamedata_core-0.0.5/src/ogd/games/GWAKKAMOLE/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:40:41.308148 opengamedata_core-0.0.5/src/ogd/games/GWAKKAMOLE/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)    12879 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/GWAKKAMOLE/schemas/GWAKKAMOLE.json.template
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:40:41.312148 opengamedata_core-0.0.5/src/ogd/games/ICECUBE/
--rw-r--r--   0 runner    (1001) docker     (127)     1883 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/ICECUBE/DBExport.json
--rw-r--r--   0 runner    (1001) docker     (127)      803 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/ICECUBE/DBExport.py
--rw-r--r--   0 runner    (1001) docker     (127)     4855 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/ICECUBE/IcecubeLoader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:40:41.312148 opengamedata_core-0.0.5/src/ogd/games/ICECUBE/features/
--rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/ICECUBE/features/HeadsetOnCount.py
--rw-r--r--   0 runner    (1001) docker     (127)     1891 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/ICECUBE/features/ObjectSelectionsDuringVoiceover.py
--rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/ICECUBE/features/PerSceneFeature.py
--rw-r--r--   0 runner    (1001) docker     (127)     2890 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/ICECUBE/features/SceneDuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1941 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/ICECUBE/features/SceneFailureCount.py
--rw-r--r--   0 runner    (1001) docker     (127)     2720 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/ICECUBE/features/SceneFailures.py
--rw-r--r--   0 runner    (1001) docker     (127)     1380 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/ICECUBE/features/ScenesEncountered.py
--rw-r--r--   0 runner    (1001) docker     (127)     3466 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/ICECUBE/features/SessionDuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/ICECUBE/features/Session_Language.py
--rw-r--r--   0 runner    (1001) docker     (127)     2389 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/ICECUBE/features/TaskTimeToComplete.py
--rw-r--r--   0 runner    (1001) docker     (127)     1780 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/ICECUBE/features/ViewportCountPerScene.py
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/ICECUBE/features/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:40:41.312148 opengamedata_core-0.0.5/src/ogd/games/ICECUBE/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)     7292 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/ICECUBE/schemas/ICECUBE.json.template
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:40:41.312148 opengamedata_core-0.0.5/src/ogd/games/JOURNALISM/
--rw-r--r--   0 runner    (1001) docker     (127)     7977 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/JOURNALISM/JournalismLoader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:40:41.320148 opengamedata_core-0.0.5/src/ogd/games/JOURNALISM/features/
--rw-r--r--   0 runner    (1001) docker     (127)     4546 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/JOURNALISM/features/AttributeView.py
--rw-r--r--   0 runner    (1001) docker     (127)     4973 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/JOURNALISM/features/ChoiceClickCount.py
--rw-r--r--   0 runner    (1001) docker     (127)     2234 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/JOURNALISM/features/ContinuesOnFail.py
--rw-r--r--   0 runner    (1001) docker     (127)     4549 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/JOURNALISM/features/EditorNoteOpen.py
--rw-r--r--   0 runner    (1001) docker     (127)     4994 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/JOURNALISM/features/FailureCount.py
--rw-r--r--   0 runner    (1001) docker     (127)     3968 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/JOURNALISM/features/GameComplete.py
--rw-r--r--   0 runner    (1001) docker     (127)     4859 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/JOURNALISM/features/LevelCompleteCount.py
--rw-r--r--   0 runner    (1001) docker     (127)     4866 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/JOURNALISM/features/LevelCompleted.py
--rw-r--r--   0 runner    (1001) docker     (127)     2824 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/JOURNALISM/features/LevelTime.py
--rw-r--r--   0 runner    (1001) docker     (127)     2340 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/JOURNALISM/features/MaxedPlayerAttribute.py
--rw-r--r--   0 runner    (1001) docker     (127)     5255 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/JOURNALISM/features/MeanSnippetTime.py
--rw-r--r--   0 runner    (1001) docker     (127)     4459 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/JOURNALISM/features/PlayTime.py
--rw-r--r--   0 runner    (1001) docker     (127)     4384 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/JOURNALISM/features/PlayerAttributes.py
--rw-r--r--   0 runner    (1001) docker     (127)     4468 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/JOURNALISM/features/QuitLevel.py
--rw-r--r--   0 runner    (1001) docker     (127)     4142 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/JOURNALISM/features/QuitNode.py
--rw-r--r--   0 runner    (1001) docker     (127)     7634 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/JOURNALISM/features/QuitType.py
--rw-r--r--   0 runner    (1001) docker     (127)     6945 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/JOURNALISM/features/QuitTypePerLevel.py
--rw-r--r--   0 runner    (1001) docker     (127)     5902 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/JOURNALISM/features/SessionPlayTime.py
--rw-r--r--   0 runner    (1001) docker     (127)     5063 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/JOURNALISM/features/SkillSequenceCount.py
--rw-r--r--   0 runner    (1001) docker     (127)     3745 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/JOURNALISM/features/SnippetReceivedCount.py
--rw-r--r--   0 runner    (1001) docker     (127)     5004 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/JOURNALISM/features/SnippetReplace.py
--rw-r--r--   0 runner    (1001) docker     (127)     2078 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/JOURNALISM/features/SnippetsCollected.py
--rw-r--r--   0 runner    (1001) docker     (127)     1778 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/JOURNALISM/features/SnippetsSubmitted.py
--rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/JOURNALISM/features/StoryAlignment.py
--rw-r--r--   0 runner    (1001) docker     (127)     2217 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/JOURNALISM/features/StoryAlignmentSequence.py
--rw-r--r--   0 runner    (1001) docker     (127)     5473 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/JOURNALISM/features/StoryCompleteTime.py
--rw-r--r--   0 runner    (1001) docker     (127)     6576 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/JOURNALISM/features/StoryEditorTime.py
--rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/JOURNALISM/features/StoryScore.py
--rw-r--r--   0 runner    (1001) docker     (127)     2190 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/JOURNALISM/features/StoryScoreSequence.py
--rw-r--r--   0 runner    (1001) docker     (127)     4773 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/JOURNALISM/features/TextClickCount.py
--rw-r--r--   0 runner    (1001) docker     (127)     4720 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/JOURNALISM/features/TopAttribute.py
--rw-r--r--   0 runner    (1001) docker     (127)     2228 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/JOURNALISM/features/TopPlayerAttribute.py
--rw-r--r--   0 runner    (1001) docker     (127)     2272 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/JOURNALISM/features/TopPlayerQuitType.py
--rw-r--r--   0 runner    (1001) docker     (127)     4475 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/JOURNALISM/features/TotalFails.py
--rw-r--r--   0 runner    (1001) docker     (127)     2086 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/JOURNALISM/features/TotalLevelTime.py
--rw-r--r--   0 runner    (1001) docker     (127)     3948 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/JOURNALISM/features/UserPlayTime.py
--rw-r--r--   0 runner    (1001) docker     (127)     4729 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/JOURNALISM/features/WorstAttribute.py
--rw-r--r--   0 runner    (1001) docker     (127)     2242 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/JOURNALISM/features/WorstPlayerAttribute.py
--rw-r--r--   0 runner    (1001) docker     (127)     2048 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/JOURNALISM/features/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:40:41.320148 opengamedata_core-0.0.5/src/ogd/games/JOURNALISM/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)    45415 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/JOURNALISM/schemas/JOURNALISM.json.template
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:40:41.324148 opengamedata_core-0.0.5/src/ogd/games/JOWILDER/
--rw-r--r--   0 runner    (1001) docker     (127)     5206 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/JOWILDER/JowilderLoader.py
--rw-r--r--   0 runner    (1001) docker     (127)    16451 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/JOWILDER/Jowilder_Enumerators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:40:41.328148 opengamedata_core-0.0.5/src/ogd/games/JOWILDER/features/
--rw-r--r--   0 runner    (1001) docker     (127)     3089 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/JOWILDER/features/ActiveStateTime.py
--rw-r--r--   0 runner    (1001) docker     (127)     1838 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/JOWILDER/features/Clicks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1438 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/JOWILDER/features/EventCount.py
--rw-r--r--   0 runner    (1001) docker     (127)     1736 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/JOWILDER/features/FirstInteraction.py
--rw-r--r--   0 runner    (1001) docker     (127)     1822 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/JOWILDER/features/GameScript.py
--rw-r--r--   0 runner    (1001) docker     (127)     1439 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/JOWILDER/features/GameVersion.py
--rw-r--r--   0 runner    (1001) docker     (127)     1359 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/JOWILDER/features/Hovers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2458 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/JOWILDER/features/IdleState.py
--rw-r--r--   0 runner    (1001) docker     (127)     7609 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/JOWILDER/features/Interaction.py
--rw-r--r--   0 runner    (1001) docker     (127)     2338 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/JOWILDER/features/InteractionName.py
--rw-r--r--   0 runner    (1001) docker     (127)     4592 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/JOWILDER/features/InteractionTextBoxesPerSecond.py
--rw-r--r--   0 runner    (1001) docker     (127)     4587 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/JOWILDER/features/InteractionWordsPerSecond.py
--rw-r--r--   0 runner    (1001) docker     (127)     1684 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/JOWILDER/features/LastInteraction.py
--rw-r--r--   0 runner    (1001) docker     (127)     1720 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/JOWILDER/features/MeaningfulActions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2000 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/JOWILDER/features/NotebookUses.py
--rw-r--r--   0 runner    (1001) docker     (127)     3211 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/JOWILDER/features/QuestionAnswers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1770 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/JOWILDER/features/SessionDuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1887 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/JOWILDER/features/SessionStart.py
--rw-r--r--   0 runner    (1001) docker     (127)     5104 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/JOWILDER/features/SurveyItem.py
--rw-r--r--   0 runner    (1001) docker     (127)     2791 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/JOWILDER/features/SurveyTime.py
--rw-r--r--   0 runner    (1001) docker     (127)     1631 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/JOWILDER/features/UsedContinue.py
--rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/JOWILDER/features/UsedSaveCode.py
--rw-r--r--   0 runner    (1001) docker     (127)     2151 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/JOWILDER/features/UserEnabled.py
--rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/JOWILDER/features/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1925 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/JOWILDER/get_jowilder_all_items.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:40:41.328148 opengamedata_core-0.0.5/src/ogd/games/JOWILDER/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)    35912 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/JOWILDER/schemas/JOWILDER.json.template
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:40:41.328148 opengamedata_core-0.0.5/src/ogd/games/LAKELAND/
--rw-r--r--   0 runner    (1001) docker     (127)     2357 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/LAKELAND/LakelandLoader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:40:41.336147 opengamedata_core-0.0.5/src/ogd/games/LAKELAND/features/
--rw-r--r--   0 runner    (1001) docker     (127)     2039 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/LAKELAND/features/ActionsLastXSecondsModel.py
--rw-r--r--   0 runner    (1001) docker     (127)      607 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/LAKELAND/features/DeathCountModel.py
--rw-r--r--   0 runner    (1001) docker     (127)    11750 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/LAKELAND/features/DeathPredModel.py
--rw-r--r--   0 runner    (1001) docker     (127)     8664 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/LAKELAND/features/DeathThresholdModel.py
--rw-r--r--   0 runner    (1001) docker     (127)     4916 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/LAKELAND/features/DiagonalFarmDetectorModel.py
--rw-r--r--   0 runner    (1001) docker     (127)     7995 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/LAKELAND/features/FeatSeqPercent.py
--rw-r--r--   0 runner    (1001) docker     (127)     2294 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/LAKELAND/features/FeatVelocity.py
--rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/LAKELAND/features/FeatureModel.py
--rw-r--r--   0 runner    (1001) docker     (127)     8478 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/LAKELAND/features/LAKELAND_models.json
--rw-r--r--   0 runner    (1001) docker     (127)     4415 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/LAKELAND/features/LakelandEnumerators.json
--rw-r--r--   0 runner    (1001) docker     (127)    69732 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/LAKELAND/features/LakelandExtractor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2639 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/LAKELAND/features/LinearModel.py
--rw-r--r--   0 runner    (1001) docker     (127)     2701 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/LAKELAND/features/LogisticModel.py
--rw-r--r--   0 runner    (1001) docker     (127)     3353 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/LAKELAND/features/MapSummaryModel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/LAKELAND/features/Model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2574 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/LAKELAND/features/MoneyAccumulationModel.py
--rw-r--r--   0 runner    (1001) docker     (127)      444 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/LAKELAND/features/NthEventModel.py
--rw-r--r--   0 runner    (1001) docker     (127)      496 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/LAKELAND/features/PlayingTimeModel.py
--rw-r--r--   0 runner    (1001) docker     (127)     3287 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/LAKELAND/features/PopulationModel.py
--rw-r--r--   0 runner    (1001) docker     (127)     4813 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/LAKELAND/features/RecentPurchasesModel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1264 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/LAKELAND/features/SequenceModel.py
--rw-r--r--   0 runner    (1001) docker     (127)     4909 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/LAKELAND/features/SimpleFarmAbandonmentModel.py
--rw-r--r--   0 runner    (1001) docker     (127)      850 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/LAKELAND/features/SingleFeatureModel.py
--rw-r--r--   0 runner    (1001) docker     (127)     6060 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/LAKELAND/features/TimeSinceEventTypes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/LAKELAND/features/TimeSinceLastSaleModel.py
--rw-r--r--   0 runner    (1001) docker     (127)      507 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/LAKELAND/features/TownCompositionFeatureModel.py
--rw-r--r--   0 runner    (1001) docker     (127)     2026 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/LAKELAND/features/TownCompositionModel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/LAKELAND/features/TutorialProgressionModel.py
--rw-r--r--   0 runner    (1001) docker     (127)    82382 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/LAKELAND/features/WAVES_models.json
--rw-r--r--   0 runner    (1001) docker     (127)    82382 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/LAKELAND/features/WAVES_models_L8_Q0_Q1.json
--rw-r--r--   0 runner    (1001) docker     (127)    49819 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/LAKELAND/features/WAVES_models_L8_and_Q0.json
--rw-r--r--   0 runner    (1001) docker     (127)    28429 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/LAKELAND/features/WAVES_models_L8_complete_and_current.json
--rw-r--r--   0 runner    (1001) docker     (127)    21021 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/LAKELAND/features/WAVES_models_L8_only_complete.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/LAKELAND/features/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2331 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/LAKELAND/produce_lakeland_enumerators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:40:41.336147 opengamedata_core-0.0.5/src/ogd/games/LAKELAND/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)   115553 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/LAKELAND/schemas/LAKELAND.json.template
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:40:41.336147 opengamedata_core-0.0.5/src/ogd/games/MAGNET/
--rw-r--r--   0 runner    (1001) docker     (127)     2346 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/MAGNET/MagnetLoader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:40:41.336147 opengamedata_core-0.0.5/src/ogd/games/MAGNET/features/
--rw-r--r--   0 runner    (1001) docker     (127)     8596 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/MAGNET/features/MagnetExtractor.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/MAGNET/features/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:40:41.336147 opengamedata_core-0.0.5/src/ogd/games/MAGNET/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)     7887 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/MAGNET/schemas/MAGNET.json.template
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:40:41.268148 opengamedata_core-0.0.5/src/ogd/games/MASHOPOLIS/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:40:41.336147 opengamedata_core-0.0.5/src/ogd/games/MASHOPOLIS/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)    10063 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/MASHOPOLIS/schemas/MASHOPOLIS.json.template
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:40:41.336147 opengamedata_core-0.0.5/src/ogd/games/PENGUINS/
--rw-r--r--   0 runner    (1001) docker     (127)     2970 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/PENGUINS/DBExport.json
--rw-r--r--   0 runner    (1001) docker     (127)     7109 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/PENGUINS/PenguinsLoader.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/PENGUINS/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:40:41.336147 opengamedata_core-0.0.5/src/ogd/games/PENGUINS/detectors/
--rw-r--r--   0 runner    (1001) docker     (127)     3747 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/PENGUINS/detectors/RegionEnter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3966 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/PENGUINS/detectors/RegionExit.py
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/PENGUINS/detectors/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:40:41.340147 opengamedata_core-0.0.5/src/ogd/games/PENGUINS/features/
--rw-r--r--   0 runner    (1001) docker     (127)     1691 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/PENGUINS/features/ActivityCompleted.py
--rw-r--r--   0 runner    (1001) docker     (127)     2720 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/PENGUINS/features/ActivityDuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/PENGUINS/features/EatFishCount.py
--rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/PENGUINS/features/EggLostCount.py
--rw-r--r--   0 runner    (1001) docker     (127)     2401 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/PENGUINS/features/EggRecoverTime.py
--rw-r--r--   0 runner    (1001) docker     (127)     1792 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/PENGUINS/features/GazeCount.py
--rw-r--r--   0 runner    (1001) docker     (127)     2663 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/PENGUINS/features/GazeDuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     4361 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/PENGUINS/features/MirrorWaddleDuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1901 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/PENGUINS/features/PerRegionFeature.py
--rw-r--r--   0 runner    (1001) docker     (127)     1232 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/PENGUINS/features/PickupRockCount.py
--rw-r--r--   0 runner    (1001) docker     (127)     2636 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/PENGUINS/features/PlayerInactiveAvgDuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/PENGUINS/features/PlayerWaddleCount.py
--rw-r--r--   0 runner    (1001) docker     (127)     2290 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/PENGUINS/features/RegionDuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/PENGUINS/features/RegionEnterCount.py
--rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/PENGUINS/features/RegionsEncountered.py
--rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/PENGUINS/features/RingChimesCount.py
--rw-r--r--   0 runner    (1001) docker     (127)     3599 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/PENGUINS/features/SessionDuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     2101 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/PENGUINS/features/SnowBallDuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1689 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/PENGUINS/features/WaddlePerRegion.py
--rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/PENGUINS/features/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:40:41.340147 opengamedata_core-0.0.5/src/ogd/games/PENGUINS/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)    28356 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/PENGUINS/schemas/PENGUINS.json.template
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:40:41.340147 opengamedata_core-0.0.5/src/ogd/games/SHADOWSPECT/
--rw-r--r--   0 runner    (1001) docker     (127)     3232 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/SHADOWSPECT/ShadowspectLoader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:40:41.344147 opengamedata_core-0.0.5/src/ogd/games/SHADOWSPECT/features/
--rw-r--r--   0 runner    (1001) docker     (127)     2789 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/SHADOWSPECT/features/FunnelByUser.py
--rw-r--r--   0 runner    (1001) docker     (127)     7671 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/SHADOWSPECT/features/LevelsOfDifficulty.py
--rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/SHADOWSPECT/features/MoveShapeCount.py
--rw-r--r--   0 runner    (1001) docker     (127)     3897 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/SHADOWSPECT/features/SequenceBetweenPuzzles.py
--rw-r--r--   0 runner    (1001) docker     (127)     1050 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/SHADOWSPECT/features/SessionID.py
--rw-r--r--   0 runner    (1001) docker     (127)      279 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/SHADOWSPECT/features/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:40:41.344147 opengamedata_core-0.0.5/src/ogd/games/SHADOWSPECT/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)    29173 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/SHADOWSPECT/schemas/SHADOWSPECT.json.template
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:40:41.344147 opengamedata_core-0.0.5/src/ogd/games/SHIPWRECKS/
--rw-r--r--   0 runner    (1001) docker     (127)     4677 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/SHIPWRECKS/ShipwrecksLoader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:40:41.348147 opengamedata_core-0.0.5/src/ogd/games/SHIPWRECKS/features/
--rw-r--r--   0 runner    (1001) docker     (127)     2164 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/SHIPWRECKS/features/ActiveJobs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2333 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/SHIPWRECKS/features/EventList.py
--rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/SHIPWRECKS/features/EvidenceBoardCompleteCount.py
--rw-r--r--   0 runner    (1001) docker     (127)     3545 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/SHIPWRECKS/features/JobsAttempted.py
--rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/SHIPWRECKS/features/JobsCompleted.py
--rw-r--r--   0 runner    (1001) docker     (127)     1426 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/SHIPWRECKS/features/MissionDiveTime.py
--rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/SHIPWRECKS/features/MissionSonarTimeToComplete.py
--rw-r--r--   0 runner    (1001) docker     (127)     1526 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/SHIPWRECKS/features/PlayerSummary.py
--rw-r--r--   0 runner    (1001) docker     (127)     1945 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/SHIPWRECKS/features/PopulationSummary.py
--rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/SHIPWRECKS/features/SessionDuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/SHIPWRECKS/features/SessionID.py
--rw-r--r--   0 runner    (1001) docker     (127)     2992 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/SHIPWRECKS/features/TopJobCompletionDestinations.py
--rw-r--r--   0 runner    (1001) docker     (127)     2736 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/SHIPWRECKS/features/TopJobSwitchDestinations.py
--rw-r--r--   0 runner    (1001) docker     (127)     1392 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/SHIPWRECKS/features/TotalDiveTime.py
--rw-r--r--   0 runner    (1001) docker     (127)      798 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/SHIPWRECKS/features/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:40:41.348147 opengamedata_core-0.0.5/src/ogd/games/SHIPWRECKS/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)    10509 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/SHIPWRECKS/schemas/SHIPWRECKS.json.template
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:40:41.348147 opengamedata_core-0.0.5/src/ogd/games/THERMOVR/
--rw-r--r--   0 runner    (1001) docker     (127)        3 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/THERMOVR/DBExport.json
--rw-r--r--   0 runner    (1001) docker     (127)     5663 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/THERMOVR/ThermoVRLoader.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/THERMOVR/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:40:41.348147 opengamedata_core-0.0.5/src/ogd/games/THERMOVR/detectors/
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/THERMOVR/detectors/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:40:41.348147 opengamedata_core-0.0.5/src/ogd/games/THERMOVR/features/
--rw-r--r--   0 runner    (1001) docker     (127)      302 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/THERMOVR/features/LabCompleteCount.py
--rw-r--r--   0 runner    (1001) docker     (127)     1888 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/THERMOVR/features/LeftHandMoves.py
--rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/THERMOVR/features/PhasesReached.py
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/THERMOVR/features/PlayMode.py
--rw-r--r--   0 runner    (1001) docker     (127)     1893 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/THERMOVR/features/RightHandMoves.py
--rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/THERMOVR/features/TaskCompleteCount.py
--rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/THERMOVR/features/ToolNudgeCount.py
--rw-r--r--   0 runner    (1001) docker     (127)     1697 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/THERMOVR/features/ToolSliderTime.py
--rw-r--r--   0 runner    (1001) docker     (127)      503 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/THERMOVR/features/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:40:41.348147 opengamedata_core-0.0.5/src/ogd/games/THERMOVR/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)    51378 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/THERMOVR/schemas/THERMOVR.json.template
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:40:41.348147 opengamedata_core-0.0.5/src/ogd/games/TRANSFORMATION_QUEST/
--rw-r--r--   0 runner    (1001) docker     (127)      777 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/TRANSFORMATION_QUEST/DBExport.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:40:41.348147 opengamedata_core-0.0.5/src/ogd/games/TRANSFORMATION_QUEST/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)    25177 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/TRANSFORMATION_QUEST/schemas/TRANSFORMATION_QUEST.json.template
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:40:41.348147 opengamedata_core-0.0.5/src/ogd/games/WAVES/
--rw-r--r--   0 runner    (1001) docker     (127)    37332 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/WAVES/WaveLoader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:40:41.360147 opengamedata_core-0.0.5/src/ogd/games/WAVES/features/
--rw-r--r--   0 runner    (1001) docker     (127)     1708 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/WAVES/features/AmplitudeGoodMoveCount.py
--rw-r--r--   0 runner    (1001) docker     (127)     1423 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/WAVES/features/AverageFails.py
--rw-r--r--   0 runner    (1001) docker     (127)     3487 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/WAVES/features/AverageLevelTime.py
--rw-r--r--   0 runner    (1001) docker     (127)     1874 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/WAVES/features/AverageMoveTypeChanges.py
--rw-r--r--   0 runner    (1001) docker     (127)     1476 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/WAVES/features/AverageSliderMoves.py
--rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/WAVES/features/BeginCount.py
--rw-r--r--   0 runner    (1001) docker     (127)     2012 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/WAVES/features/ClosenessIntercept.py
--rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/WAVES/features/ClosenessR2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/WAVES/features/ClosenessSlope.py
--rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/WAVES/features/Completed.py
--rw-r--r--   0 runner    (1001) docker     (127)     1192 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/WAVES/features/FirstMoveType.py
--rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/WAVES/features/MenuButtonCount.py
--rw-r--r--   0 runner    (1001) docker     (127)     1702 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/WAVES/features/OffsetGoodMoveCount.py
--rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/WAVES/features/OverallPercentAmplitudeMoves.py
--rw-r--r--   0 runner    (1001) docker     (127)     1427 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/WAVES/features/OverallPercentOffsetMoves.py
--rw-r--r--   0 runner    (1001) docker     (127)     1449 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/WAVES/features/OverallPercentWavelengthMoves.py
--rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/WAVES/features/OverallSliderAverageRange.py
--rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/WAVES/features/OverallSliderAverageStandardDeviations.py
--rw-r--r--   0 runner    (1001) docker     (127)     1919 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/WAVES/features/PercentAmplitudeGoodMoves.py
--rw-r--r--   0 runner    (1001) docker     (127)     1422 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/WAVES/features/PercentAmplitudeMoves.py
--rw-r--r--   0 runner    (1001) docker     (127)     1901 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/WAVES/features/PercentOffsetGoodMoves.py
--rw-r--r--   0 runner    (1001) docker     (127)     1325 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/WAVES/features/PercentOffsetMoves.py
--rw-r--r--   0 runner    (1001) docker     (127)     1843 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/WAVES/features/PercentWavelengthGoodMoves.py
--rw-r--r--   0 runner    (1001) docker     (127)     1345 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/WAVES/features/PercentWavelengthMoves.py
--rw-r--r--   0 runner    (1001) docker     (127)     1227 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/WAVES/features/PersistentSessionID.py
--rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/WAVES/features/QuestionAnswered.py
--rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/WAVES/features/QuestionCorrect.py
--rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/WAVES/features/RangeIntercept.py
--rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/WAVES/features/RangeR2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/WAVES/features/RangeSlope.py
--rw-r--r--   0 runner    (1001) docker     (127)     1627 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/WAVES/features/SequenceLevel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/WAVES/features/SessionID.py
--rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/WAVES/features/SliderAverageRange.py
--rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/WAVES/features/SliderAverageStandardDeviations.py
--rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/WAVES/features/SucceedCount.py
--rw-r--r--   0 runner    (1001) docker     (127)     2595 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/WAVES/features/TimeToAnswerMS.py
--rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/WAVES/features/TotalArrowMoves.py
--rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/WAVES/features/TotalFails.py
--rw-r--r--   0 runner    (1001) docker     (127)     1984 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/WAVES/features/TotalLevelTime.py
--rw-r--r--   0 runner    (1001) docker     (127)     1341 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/WAVES/features/TotalMoveTypeChanges.py
--rw-r--r--   0 runner    (1001) docker     (127)     1171 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/WAVES/features/TotalResets.py
--rw-r--r--   0 runner    (1001) docker     (127)     1163 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/WAVES/features/TotalSkips.py
--rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/WAVES/features/TotalSliderMoves.py
--rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/WAVES/features/WavelengthGoodMoveCount.py
--rw-r--r--   0 runner    (1001) docker     (127)     2575 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/WAVES/features/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:40:41.360147 opengamedata_core-0.0.5/src/ogd/games/WAVES/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)    21383 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/WAVES/schemas/WAVES.json.template
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:40:41.268148 opengamedata_core-0.0.5/src/ogd/games/WEATHER_STATION/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:40:41.360147 opengamedata_core-0.0.5/src/ogd/games/WEATHER_STATION/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)    34344 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/WEATHER_STATION/schemas/WEATHER_STATION.json.template
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:40:41.268148 opengamedata_core-0.0.5/src/ogd/games/WIND/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:40:41.360147 opengamedata_core-0.0.5/src/ogd/games/WIND/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/WIND/schemas/WIND.json.template
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 03:39:52.000000 opengamedata_core-0.0.5/src/ogd/games/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:40:41.360147 opengamedata_core-0.0.5/src/opengamedata_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4796 2024-05-17 03:40:41.000000 opengamedata_core-0.0.5/src/opengamedata_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    21689 2024-05-17 03:40:41.000000 opengamedata_core-0.0.5/src/opengamedata_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 03:40:41.000000 opengamedata_core-0.0.5/src/opengamedata_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-17 03:40:41.000000 opengamedata_core-0.0.5/src/opengamedata_core.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:40:41.360147 opengamedata_core-0.0.5/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3113 2024-05-17 03:39:53.000000 opengamedata_core-0.0.5/tests/test_lakeland_models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:05:05.067022 opengamedata_core-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4796 2024-05-30 18:05:05.067022 opengamedata_core-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3900 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 18:05:05.067022 opengamedata_core-0.0.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:05:04.983023 opengamedata_core-0.0.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:05:04.983023 opengamedata_core-0.0.6/src/ogd/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:05:04.983023 opengamedata_core-0.0.6/src/ogd/core/
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:05:04.983023 opengamedata_core-0.0.6/src/ogd/core/exec/
+-rw-r--r--   0 runner    (1001) docker     (127)     9579 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/core/exec/Commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3903 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/core/exec/Generators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4858 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/core/exec/Parsers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:05:04.971023 opengamedata_core-0.0.6/src/ogd/core/games/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:05:04.971023 opengamedata_core-0.0.6/src/ogd/core/games/AQUALAB/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:05:04.983023 opengamedata_core-0.0.6/src/ogd/core/games/AQUALAB/features/
+-rw-r--r--   0 runner    (1001) docker     (127)     4259 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/core/games/AQUALAB/features/PlayLocations.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:05:04.987023 opengamedata_core-0.0.6/src/ogd/core/generators/
+-rw-r--r--   0 runner    (1001) docker     (127)     7945 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/core/generators/Generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5140 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/core/generators/GeneratorLoader.py
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/core/generators/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:05:04.987023 opengamedata_core-0.0.6/src/ogd/core/generators/detectors/
+-rw-r--r--   0 runner    (1001) docker     (127)     4355 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/core/generators/detectors/Detector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2299 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/core/generators/detectors/DetectorEvent.py
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/core/generators/detectors/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:05:04.987023 opengamedata_core-0.0.6/src/ogd/core/generators/extractors/
+-rw-r--r--   0 runner    (1001) docker     (127)     6502 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/core/generators/extractors/Extractor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/core/generators/extractors/Feature.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1584 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/core/generators/extractors/PerCountFeature.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/core/generators/extractors/PerLevelFeature.py
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/core/generators/extractors/SessionFeature.py
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/core/generators/extractors/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:05:04.987023 opengamedata_core-0.0.6/src/ogd/core/generators/legacy/
+-rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/core/generators/legacy/LegacyDetector.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14636 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/core/generators/legacy/LegacyFeature.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/core/generators/legacy/LegacyLoader.py
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/core/generators/legacy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:05:04.987023 opengamedata_core-0.0.6/src/ogd/core/generators/registries/
+-rw-r--r--   0 runner    (1001) docker     (127)     8372 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/core/generators/registries/DetectorRegistry.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13807 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/core/generators/registries/ExtractorRegistry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5284 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/core/generators/registries/GeneratorRegistry.py
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/core/generators/registries/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:05:04.991023 opengamedata_core-0.0.6/src/ogd/core/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (127)    10837 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/core/interfaces/BQFirebaseInterface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9704 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/core/interfaces/BigQueryCodingInterface.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11862 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/core/interfaces/BigQueryInterface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4908 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/core/interfaces/CSVInterface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3524 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/core/interfaces/CodingInterface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5436 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/core/interfaces/DataInterface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/core/interfaces/Interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23923 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/core/interfaces/MySQLInterface.py
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/core/interfaces/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:05:04.991023 opengamedata_core-0.0.6/src/ogd/core/interfaces/outerfaces/
+-rw-r--r--   0 runner    (1001) docker     (127)     5834 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/core/interfaces/outerfaces/DataOuterface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4200 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/core/interfaces/outerfaces/DebugOuterface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4907 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/core/interfaces/outerfaces/DictionaryOuterface.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33767 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/core/interfaces/outerfaces/TSVOuterface.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:05:04.991023 opengamedata_core-0.0.6/src/ogd/core/managers/
+-rw-r--r--   0 runner    (1001) docker     (127)     3512 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/core/managers/EventManager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19016 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/core/managers/ExportManager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12107 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/core/managers/FeatureManager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/core/managers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:05:04.991023 opengamedata_core-0.0.6/src/ogd/core/models/
+-rw-r--r--   0 runner    (1001) docker     (127)    14401 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/core/models/Event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1431 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/core/models/FeatureData.py
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/core/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:05:04.995023 opengamedata_core-0.0.6/src/ogd/core/models/enums/
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/core/models/enums/ExportMode.py
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/core/models/enums/ExtractionMode.py
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/core/models/enums/IDMode.py
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/core/models/enums/IterationMode.py
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/core/models/enums/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:05:04.995023 opengamedata_core-0.0.6/src/ogd/core/processors/
+-rw-r--r--   0 runner    (1001) docker     (127)     6040 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/core/processors/ClassroomDetector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2242 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/core/processors/DetectorProcessor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      963 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/core/processors/EventProcessor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1658 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/core/processors/ExtractorProcessor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2637 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/core/processors/GeneratorProcessor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4610 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/core/processors/PlayerProcessor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4218 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/core/processors/PopulationProcessor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1876 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/core/processors/Processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4275 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/core/processors/SessionProcessor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/core/processors/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:05:04.995023 opengamedata_core-0.0.6/src/ogd/core/requests/
+-rw-r--r--   0 runner    (1001) docker     (127)     5311 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/core/requests/Request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2062 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/core/requests/RequestResult.py
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/core/requests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:05:04.995023 opengamedata_core-0.0.6/src/ogd/core/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)     1427 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/core/schemas/Schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/core/schemas/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:05:04.999023 opengamedata_core-0.0.6/src/ogd/core/schemas/configs/
+-rw-r--r--   0 runner    (1001) docker     (127)    10898 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/core/schemas/configs/ConfigSchema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5835 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/core/schemas/configs/GameSourceSchema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3452 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/core/schemas/configs/IndexingSchema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2593 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/core/schemas/configs/LegacyConfigSchema.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:05:04.999023 opengamedata_core-0.0.6/src/ogd/core/schemas/configs/data_sources/
+-rw-r--r--   0 runner    (1001) docker     (127)     3048 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/core/schemas/configs/data_sources/BigQuerySourceSchema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1806 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/core/schemas/configs/data_sources/DataSourceSchema.py
+-rw-r--r--   0 runner    (1001) docker     (127)      577 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/core/schemas/configs/data_sources/FileSourceSchema.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10140 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/core/schemas/configs/data_sources/MySQLSourceSchema.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:05:04.999023 opengamedata_core-0.0.6/src/ogd/core/schemas/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)    20326 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/core/schemas/datasets/DatasetSchema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6410 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/core/schemas/datasets/FileListSchema.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:05:05.003023 opengamedata_core-0.0.6/src/ogd/core/schemas/games/
+-rw-r--r--   0 runner    (1001) docker     (127)      922 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/core/schemas/games/AggregateSchema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5168 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/core/schemas/games/DataElementSchema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5045 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/core/schemas/games/DetectorMapSchema.py
+-rw-r--r--   0 runner    (1001) docker     (127)      806 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/core/schemas/games/DetectorSchema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3996 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/core/schemas/games/EventSchema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4011 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/core/schemas/games/ExtractorSchema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5656 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/core/schemas/games/FeatureMapSchema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4869 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/core/schemas/games/FeatureSchema.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26736 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/core/schemas/games/GameSchema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2652 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/core/schemas/games/GameStateSchema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2831 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/core/schemas/games/PerCountSchema.py
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/core/schemas/games/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:05:05.003023 opengamedata_core-0.0.6/src/ogd/core/schemas/table_schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)     3615 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/core/schemas/table_schemas/BIGQUERY.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4890 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/core/schemas/table_schemas/FIELDDAY_MYSQL.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2390 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/core/schemas/table_schemas/FIREBASE.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4430 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/core/schemas/table_schemas/MASHOPOLIS_MYSQL.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3685 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/core/schemas/table_schemas/OGD_EVENT_FILE.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4077 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/core/schemas/table_schemas/OPENGAMEDATA_BIGQUERY.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4477 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/core/schemas/table_schemas/OPENGAMEDATA_MYSQL.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1920 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/core/schemas/table_schemas/SHIPWRECKS.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:05:05.003023 opengamedata_core-0.0.6/src/ogd/core/schemas/tables/
+-rw-r--r--   0 runner    (1001) docker     (127)     6782 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/core/schemas/tables/ColumnMapSchema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4179 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/core/schemas/tables/ColumnSchema.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23083 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/core/schemas/tables/TableSchema.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:05:05.003023 opengamedata_core-0.0.6/src/ogd/core/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     4573 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/core/utils/Logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4361 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/core/utils/Readme.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14950 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/core/utils/SemanticVersion.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/core/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/core/utils/typing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2692 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/core/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:05:05.003023 opengamedata_core-0.0.6/src/ogd/games/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:05:04.975023 opengamedata_core-0.0.6/src/ogd/games/ALL_YOU_CAN_ET/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:05:05.007023 opengamedata_core-0.0.6/src/ogd/games/ALL_YOU_CAN_ET/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)    20816 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/games/ALL_YOU_CAN_ET/schemas/ALL_YOU_CAN_ET.json.template
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:05:05.007023 opengamedata_core-0.0.6/src/ogd/games/AQUALAB/
+-rw-r--r--   0 runner    (1001) docker     (127)    13547 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/games/AQUALAB/AqualabLoader.py
+-rw-r--r--   0 runner    (1001) docker     (127)   278275 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/games/AQUALAB/DBExport.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/games/AQUALAB/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:05:05.007023 opengamedata_core-0.0.6/src/ogd/games/AQUALAB/detectors/
+-rw-r--r--   0 runner    (1001) docker     (127)     2324 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/games/AQUALAB/detectors/CollectFactNoJob.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3558 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/games/AQUALAB/detectors/DiveSiteNoEvidence.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1729 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/games/AQUALAB/detectors/EchoRoomChange.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4509 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/games/AQUALAB/detectors/HintAndLeave.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3470 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/games/AQUALAB/detectors/Idle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3905 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/games/AQUALAB/detectors/SceneChangeFrequently.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3800 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/games/AQUALAB/detectors/TwoHints.py
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/games/AQUALAB/detectors/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:05:05.019023 opengamedata_core-0.0.6/src/ogd/games/AQUALAB/features/
+-rw-r--r--   0 runner    (1001) docker     (127)     2755 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/games/AQUALAB/features/ActiveJobs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2335 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/games/AQUALAB/features/ActiveTime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/games/AQUALAB/features/AppVersions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1752 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/games/AQUALAB/features/AverageSessionTime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/games/AQUALAB/features/EchoSessionID.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5321 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/games/AQUALAB/features/EventList.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9516 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/games/AQUALAB/features/JobActiveTime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2463 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/games/AQUALAB/features/JobArgumentation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2711 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/games/AQUALAB/features/JobCompletionTime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/games/AQUALAB/features/JobDiveSitesCount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2141 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/games/AQUALAB/features/JobDiveTime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2411 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/games/AQUALAB/features/JobExperimentation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1247 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/games/AQUALAB/features/JobGuideCount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1761 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/games/AQUALAB/features/JobHelpCount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3955 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/games/AQUALAB/features/JobLocationChanges.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2282 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/games/AQUALAB/features/JobModeling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2347 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/games/AQUALAB/features/JobPlayTime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2122 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/games/AQUALAB/features/JobPriorAttempt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1946 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/games/AQUALAB/features/JobPriorComplete.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/games/AQUALAB/features/JobStartCount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/games/AQUALAB/features/JobTasksCompleted.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/games/AQUALAB/features/JobTriesInArgument.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6200 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/games/AQUALAB/features/JobsAttempted.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1532 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/games/AQUALAB/features/JobsCompleted.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/games/AQUALAB/features/ModelExportCount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/games/AQUALAB/features/ModelInterveneCount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/games/AQUALAB/features/ModelPredictCount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/games/AQUALAB/features/PerJobFeature.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3022 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/games/AQUALAB/features/PlayerSummary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3354 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/games/AQUALAB/features/PopulationSummary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/games/AQUALAB/features/RegionJobCount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1292 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/games/AQUALAB/features/RegionName.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/games/AQUALAB/features/SessionDiveSitesCount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3953 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/games/AQUALAB/features/SessionDuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/games/AQUALAB/features/SessionGuideCount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/games/AQUALAB/features/SessionHelpCount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/games/AQUALAB/features/SessionID.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/games/AQUALAB/features/SessionJobsCompleted.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/games/AQUALAB/features/SwitchJobsCount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2524 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/games/AQUALAB/features/SyncCompletionTime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1736 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/games/AQUALAB/features/TankRulesCount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3461 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/games/AQUALAB/features/TopJobCompletionDestinations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3447 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/games/AQUALAB/features/TopJobSwitchDestinations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3342 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/games/AQUALAB/features/TotalArcticTime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2196 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/games/AQUALAB/features/TotalArgumentationTime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3335 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/games/AQUALAB/features/TotalBayouTime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3335 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/games/AQUALAB/features/TotalCoralTime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2797 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/games/AQUALAB/features/TotalDiveTime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2139 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/games/AQUALAB/features/TotalExperimentationTime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/games/AQUALAB/features/TotalGuideCount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/games/AQUALAB/features/TotalHelpCount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3328 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/games/AQUALAB/features/TotalKelpTime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2124 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/games/AQUALAB/features/TotalModelingTime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2496 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/games/AQUALAB/features/TotalPlayTime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/games/AQUALAB/features/UserAvgActiveTime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1415 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/games/AQUALAB/features/UserAvgSessionDuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1447 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/games/AQUALAB/features/UserTotalSessionDuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3093 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/games/AQUALAB/features/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:05:05.019023 opengamedata_core-0.0.6/src/ogd/games/AQUALAB/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)    32117 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/games/AQUALAB/schemas/AQUALAB.json.template
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:05:04.975023 opengamedata_core-0.0.6/src/ogd/games/BACTERIA/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:05:05.019023 opengamedata_core-0.0.6/src/ogd/games/BACTERIA/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/games/BACTERIA/schemas/BACTERIA.json.template
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:05:04.975023 opengamedata_core-0.0.6/src/ogd/games/BALLOON/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:05:05.019023 opengamedata_core-0.0.6/src/ogd/games/BALLOON/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/games/BALLOON/schemas/BALLOON.json.template
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:05:04.975023 opengamedata_core-0.0.6/src/ogd/games/BLOOM/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:05:05.019023 opengamedata_core-0.0.6/src/ogd/games/BLOOM/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)    21554 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/games/BLOOM/schemas/BLOOM.json.template
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:05:04.975023 opengamedata_core-0.0.6/src/ogd/games/CENSIO_SLIDE/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:05:05.019023 opengamedata_core-0.0.6/src/ogd/games/CENSIO_SLIDE/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)    11446 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/games/CENSIO_SLIDE/schemas/CENSIO_SLIDE.json.template
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:05:04.975023 opengamedata_core-0.0.6/src/ogd/games/CENSIO_STACK/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:05:05.019023 opengamedata_core-0.0.6/src/ogd/games/CENSIO_STACK/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)    21742 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/games/CENSIO_STACK/schemas/CENSIO_STACK.json.template
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:05:04.975023 opengamedata_core-0.0.6/src/ogd/games/CRUSH_STATION/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:05:05.019023 opengamedata_core-0.0.6/src/ogd/games/CRUSH_STATION/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)    11756 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/CRUSH_STATION/schemas/CRUSH_STATION.json.template
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:05:05.019023 opengamedata_core-0.0.6/src/ogd/games/CRYSTAL/
+-rw-r--r--   0 runner    (1001) docker     (127)     2384 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/CRYSTAL/CrystalLoader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:05:05.019023 opengamedata_core-0.0.6/src/ogd/games/CRYSTAL/features/
+-rw-r--r--   0 runner    (1001) docker     (127)    14127 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/CRYSTAL/features/CrystalExtractor.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/CRYSTAL/features/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:05:05.019023 opengamedata_core-0.0.6/src/ogd/games/CRYSTAL/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)    14066 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/CRYSTAL/schemas/CRYSTAL.json.template
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:05:04.975023 opengamedata_core-0.0.6/src/ogd/games/CYCLE_CARBON/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:05:05.019023 opengamedata_core-0.0.6/src/ogd/games/CYCLE_CARBON/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/CYCLE_CARBON/schemas/CYCLE_CARBON.json.template
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:05:04.975023 opengamedata_core-0.0.6/src/ogd/games/CYCLE_NITROGEN/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:05:05.019023 opengamedata_core-0.0.6/src/ogd/games/CYCLE_NITROGEN/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/CYCLE_NITROGEN/schemas/CYCLE_NITROGEN.json.template
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:05:04.975023 opengamedata_core-0.0.6/src/ogd/games/CYCLE_WATER/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:05:05.023023 opengamedata_core-0.0.6/src/ogd/games/CYCLE_WATER/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/CYCLE_WATER/schemas/CYCLE_WATER.json.template
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:05:04.975023 opengamedata_core-0.0.6/src/ogd/games/EARTHQUAKE/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:05:05.023023 opengamedata_core-0.0.6/src/ogd/games/EARTHQUAKE/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/EARTHQUAKE/schemas/EARTHQUAKE.json.template
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:05:04.975023 opengamedata_core-0.0.6/src/ogd/games/GWAKKAMOLE/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:05:05.023023 opengamedata_core-0.0.6/src/ogd/games/GWAKKAMOLE/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)    12879 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/GWAKKAMOLE/schemas/GWAKKAMOLE.json.template
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:05:05.023023 opengamedata_core-0.0.6/src/ogd/games/ICECUBE/
+-rw-r--r--   0 runner    (1001) docker     (127)     1883 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/ICECUBE/DBExport.json
+-rw-r--r--   0 runner    (1001) docker     (127)      803 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/ICECUBE/DBExport.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4859 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/ICECUBE/IcecubeLoader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:05:05.023023 opengamedata_core-0.0.6/src/ogd/games/ICECUBE/features/
+-rw-r--r--   0 runner    (1001) docker     (127)     1281 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/ICECUBE/features/HeadsetOnCount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1894 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/ICECUBE/features/ObjectSelectionsDuringVoiceover.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/ICECUBE/features/PerSceneFeature.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2893 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/ICECUBE/features/SceneDuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1944 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/ICECUBE/features/SceneFailureCount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2723 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/ICECUBE/features/SceneFailures.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/ICECUBE/features/ScenesEncountered.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3472 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/ICECUBE/features/SessionDuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/ICECUBE/features/Session_Language.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2392 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/ICECUBE/features/TaskTimeToComplete.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1783 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/ICECUBE/features/ViewportCountPerScene.py
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/ICECUBE/features/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:05:05.023023 opengamedata_core-0.0.6/src/ogd/games/ICECUBE/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)     7292 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/ICECUBE/schemas/ICECUBE.json.template
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:05:05.023023 opengamedata_core-0.0.6/src/ogd/games/JOURNALISM/
+-rw-r--r--   0 runner    (1001) docker     (127)     7981 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/JOURNALISM/JournalismLoader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:05:05.031023 opengamedata_core-0.0.6/src/ogd/games/JOURNALISM/features/
+-rw-r--r--   0 runner    (1001) docker     (127)     4549 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/JOURNALISM/features/AttributeView.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4976 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/JOURNALISM/features/ChoiceClickCount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2236 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/JOURNALISM/features/ContinuesOnFail.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4552 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/JOURNALISM/features/EditorNoteOpen.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2971 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/JOURNALISM/features/FailureAttributes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4997 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/JOURNALISM/features/FailureCount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1942 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/JOURNALISM/features/FinalAttributes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3971 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/JOURNALISM/features/GameComplete.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4862 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/JOURNALISM/features/LevelCompleteCount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4869 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/JOURNALISM/features/LevelCompleted.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2826 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/JOURNALISM/features/LevelTime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2342 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/JOURNALISM/features/MaxedPlayerAttribute.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5258 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/JOURNALISM/features/MeanSnippetTime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4462 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/JOURNALISM/features/PlayTime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4387 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/JOURNALISM/features/PlayerAttributes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4471 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/JOURNALISM/features/QuitLevel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4145 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/JOURNALISM/features/QuitNode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7637 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/JOURNALISM/features/QuitType.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6948 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/JOURNALISM/features/QuitTypePerLevel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5905 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/JOURNALISM/features/SessionPlayTime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5066 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/JOURNALISM/features/SkillSequenceCount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3748 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/JOURNALISM/features/SnippetReceivedCount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5007 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/JOURNALISM/features/SnippetReplace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2080 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/JOURNALISM/features/SnippetsCollected.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1780 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/JOURNALISM/features/SnippetsSubmitted.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/JOURNALISM/features/StoryAlignment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2219 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/JOURNALISM/features/StoryAlignmentSequence.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5476 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/JOURNALISM/features/StoryCompleteTime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6579 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/JOURNALISM/features/StoryEditorTime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/JOURNALISM/features/StoryScore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2192 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/JOURNALISM/features/StoryScoreSequence.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4776 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/JOURNALISM/features/TextClickCount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4723 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/JOURNALISM/features/TopAttribute.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2230 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/JOURNALISM/features/TopPlayerAttribute.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2274 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/JOURNALISM/features/TopPlayerQuitType.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4478 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/JOURNALISM/features/TotalFails.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2088 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/JOURNALISM/features/TotalLevelTime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3951 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/JOURNALISM/features/UserPlayTime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4732 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/JOURNALISM/features/WorstAttribute.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2244 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/JOURNALISM/features/WorstPlayerAttribute.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2048 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/JOURNALISM/features/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:05:05.031023 opengamedata_core-0.0.6/src/ogd/games/JOURNALISM/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)    45415 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/JOURNALISM/schemas/JOURNALISM.json.template
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:05:05.031023 opengamedata_core-0.0.6/src/ogd/games/JOWILDER/
+-rw-r--r--   0 runner    (1001) docker     (127)     5210 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/JOWILDER/JowilderLoader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16451 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/JOWILDER/Jowilder_Enumerators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:05:05.035023 opengamedata_core-0.0.6/src/ogd/games/JOWILDER/features/
+-rw-r--r--   0 runner    (1001) docker     (127)     3092 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/JOWILDER/features/ActiveStateTime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1841 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/JOWILDER/features/Clicks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1441 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/JOWILDER/features/EventCount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1739 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/JOWILDER/features/FirstInteraction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/JOWILDER/features/GameScript.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/JOWILDER/features/GameVersion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1362 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/JOWILDER/features/Hovers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2461 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/JOWILDER/features/IdleState.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7612 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/JOWILDER/features/Interaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2341 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/JOWILDER/features/InteractionName.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4595 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/JOWILDER/features/InteractionTextBoxesPerSecond.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4590 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/JOWILDER/features/InteractionWordsPerSecond.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1687 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/JOWILDER/features/LastInteraction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1723 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/JOWILDER/features/MeaningfulActions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2003 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/JOWILDER/features/NotebookUses.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3214 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/JOWILDER/features/QuestionAnswers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1773 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/JOWILDER/features/SessionDuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1890 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/JOWILDER/features/SessionStart.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5107 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/JOWILDER/features/SurveyItem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2794 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/JOWILDER/features/SurveyTime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/JOWILDER/features/UsedContinue.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1327 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/JOWILDER/features/UsedSaveCode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2154 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/JOWILDER/features/UserEnabled.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/JOWILDER/features/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1925 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/JOWILDER/get_jowilder_all_items.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:05:05.035023 opengamedata_core-0.0.6/src/ogd/games/JOWILDER/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)    35912 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/JOWILDER/schemas/JOWILDER.json.template
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:05:05.039023 opengamedata_core-0.0.6/src/ogd/games/LAKELAND/
+-rw-r--r--   0 runner    (1001) docker     (127)     2361 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/LAKELAND/LakelandLoader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:05:05.043022 opengamedata_core-0.0.6/src/ogd/games/LAKELAND/features/
+-rw-r--r--   0 runner    (1001) docker     (127)     2039 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/LAKELAND/features/ActionsLastXSecondsModel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      607 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/LAKELAND/features/DeathCountModel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11750 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/LAKELAND/features/DeathPredModel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8664 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/LAKELAND/features/DeathThresholdModel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4916 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/LAKELAND/features/DiagonalFarmDetectorModel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7995 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/LAKELAND/features/FeatSeqPercent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2294 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/LAKELAND/features/FeatVelocity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/LAKELAND/features/FeatureModel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8478 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/LAKELAND/features/LAKELAND_models.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4415 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/LAKELAND/features/LakelandEnumerators.json
+-rw-r--r--   0 runner    (1001) docker     (127)    69736 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/LAKELAND/features/LakelandExtractor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2639 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/LAKELAND/features/LinearModel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2701 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/LAKELAND/features/LogisticModel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3353 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/LAKELAND/features/MapSummaryModel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/LAKELAND/features/Model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2574 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/LAKELAND/features/MoneyAccumulationModel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      444 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/LAKELAND/features/NthEventModel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      496 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/LAKELAND/features/PlayingTimeModel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3287 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/LAKELAND/features/PopulationModel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4813 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/LAKELAND/features/RecentPurchasesModel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1264 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/LAKELAND/features/SequenceModel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4909 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/LAKELAND/features/SimpleFarmAbandonmentModel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      850 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/LAKELAND/features/SingleFeatureModel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6060 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/LAKELAND/features/TimeSinceEventTypes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/LAKELAND/features/TimeSinceLastSaleModel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      507 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/LAKELAND/features/TownCompositionFeatureModel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2026 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/LAKELAND/features/TownCompositionModel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/LAKELAND/features/TutorialProgressionModel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    82382 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/LAKELAND/features/WAVES_models.json
+-rw-r--r--   0 runner    (1001) docker     (127)    82382 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/LAKELAND/features/WAVES_models_L8_Q0_Q1.json
+-rw-r--r--   0 runner    (1001) docker     (127)    49819 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/LAKELAND/features/WAVES_models_L8_and_Q0.json
+-rw-r--r--   0 runner    (1001) docker     (127)    28429 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/LAKELAND/features/WAVES_models_L8_complete_and_current.json
+-rw-r--r--   0 runner    (1001) docker     (127)    21021 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/LAKELAND/features/WAVES_models_L8_only_complete.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/LAKELAND/features/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2331 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/LAKELAND/produce_lakeland_enumerators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:05:05.043022 opengamedata_core-0.0.6/src/ogd/games/LAKELAND/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)   115553 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/LAKELAND/schemas/LAKELAND.json.template
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:05:05.043022 opengamedata_core-0.0.6/src/ogd/games/MAGNET/
+-rw-r--r--   0 runner    (1001) docker     (127)     2350 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/MAGNET/MagnetLoader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:05:05.043022 opengamedata_core-0.0.6/src/ogd/games/MAGNET/features/
+-rw-r--r--   0 runner    (1001) docker     (127)     8600 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/MAGNET/features/MagnetExtractor.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/MAGNET/features/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:05:05.043022 opengamedata_core-0.0.6/src/ogd/games/MAGNET/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)     7887 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/MAGNET/schemas/MAGNET.json.template
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:05:04.979023 opengamedata_core-0.0.6/src/ogd/games/MASHOPOLIS/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:05:05.043022 opengamedata_core-0.0.6/src/ogd/games/MASHOPOLIS/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)    10063 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/MASHOPOLIS/schemas/MASHOPOLIS.json.template
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:05:05.047022 opengamedata_core-0.0.6/src/ogd/games/PENGUINS/
+-rw-r--r--   0 runner    (1001) docker     (127)     2970 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/PENGUINS/DBExport.json
+-rw-r--r--   0 runner    (1001) docker     (127)     8007 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/PENGUINS/PenguinsLoader.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/PENGUINS/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:05:05.047022 opengamedata_core-0.0.6/src/ogd/games/PENGUINS/detectors/
+-rw-r--r--   0 runner    (1001) docker     (127)     5164 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/PENGUINS/detectors/RegionEnter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6271 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/PENGUINS/detectors/RegionExit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/PENGUINS/detectors/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:05:05.051023 opengamedata_core-0.0.6/src/ogd/games/PENGUINS/features/
+-rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/PENGUINS/features/ActivityCompleted.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2723 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/PENGUINS/features/ActivityDuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/PENGUINS/features/BuiltNestCount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1445 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/PENGUINS/features/BuiltWrongNestCount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/PENGUINS/features/EatFishCount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/PENGUINS/features/EggLostCount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/PENGUINS/features/EggRecoverTime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1662 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/PENGUINS/features/GazeCount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2666 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/PENGUINS/features/GazeDuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/PENGUINS/features/LogVersion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4231 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/PENGUINS/features/MirrorWaddleDuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/PENGUINS/features/PenguinInteractCount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2508 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/PENGUINS/features/PlayerInactiveAvgDuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2299 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/PENGUINS/features/RegionDuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1797 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/PENGUINS/features/RegionEnterCount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/PENGUINS/features/RegionsEncountered.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/PENGUINS/features/RingChimesCount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/PENGUINS/features/RockBashCount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1419 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/PENGUINS/features/RockMultiplePickupCount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/PENGUINS/features/RockPickupCount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3212 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/PENGUINS/features/SessionDuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/PENGUINS/features/SkuaBashCount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/PENGUINS/features/SkuaPeckCount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1971 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/PENGUINS/features/SnowBallDuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/PENGUINS/features/WaddleCount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1698 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/PENGUINS/features/WaddlePerRegion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1474 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/PENGUINS/features/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:05:05.051023 opengamedata_core-0.0.6/src/ogd/games/PENGUINS/features/bases/
+-rw-r--r--   0 runner    (1001) docker     (127)     3507 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/PENGUINS/features/bases/PerRegionFeature.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:05:05.051023 opengamedata_core-0.0.6/src/ogd/games/PENGUINS/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)    30981 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/PENGUINS/schemas/PENGUINS.json.template
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:05:05.051023 opengamedata_core-0.0.6/src/ogd/games/SHADOWSPECT/
+-rw-r--r--   0 runner    (1001) docker     (127)     3373 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/SHADOWSPECT/ShadowspectLoader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:05:05.051023 opengamedata_core-0.0.6/src/ogd/games/SHADOWSPECT/features/
+-rw-r--r--   0 runner    (1001) docker     (127)     2951 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/SHADOWSPECT/features/FunnelByUser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7674 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/SHADOWSPECT/features/LevelsOfDifficulty.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/SHADOWSPECT/features/MoveShapeCount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3916 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/SHADOWSPECT/features/SequenceBetweenPuzzles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8242 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/SHADOWSPECT/features/SequenceWithinPuzzles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/SHADOWSPECT/features/SessionID.py
+-rw-r--r--   0 runner    (1001) docker     (127)      344 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/SHADOWSPECT/features/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:05:05.051023 opengamedata_core-0.0.6/src/ogd/games/SHADOWSPECT/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)    29173 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/SHADOWSPECT/schemas/SHADOWSPECT.json.template
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:05:05.051023 opengamedata_core-0.0.6/src/ogd/games/SHIPWRECKS/
+-rw-r--r--   0 runner    (1001) docker     (127)     4681 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/SHIPWRECKS/ShipwrecksLoader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:05:05.055023 opengamedata_core-0.0.6/src/ogd/games/SHIPWRECKS/features/
+-rw-r--r--   0 runner    (1001) docker     (127)     2167 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/SHIPWRECKS/features/ActiveJobs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2336 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/SHIPWRECKS/features/EventList.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/SHIPWRECKS/features/EvidenceBoardCompleteCount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3548 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/SHIPWRECKS/features/JobsAttempted.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1225 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/SHIPWRECKS/features/JobsCompleted.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/SHIPWRECKS/features/MissionDiveTime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/SHIPWRECKS/features/MissionSonarTimeToComplete.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/SHIPWRECKS/features/PlayerSummary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1948 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/SHIPWRECKS/features/PopulationSummary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/SHIPWRECKS/features/SessionDuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/SHIPWRECKS/features/SessionID.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2995 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/SHIPWRECKS/features/TopJobCompletionDestinations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2739 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/SHIPWRECKS/features/TopJobSwitchDestinations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/SHIPWRECKS/features/TotalDiveTime.py
+-rw-r--r--   0 runner    (1001) docker     (127)      798 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/SHIPWRECKS/features/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:05:05.055023 opengamedata_core-0.0.6/src/ogd/games/SHIPWRECKS/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)    10509 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/SHIPWRECKS/schemas/SHIPWRECKS.json.template
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:05:05.055023 opengamedata_core-0.0.6/src/ogd/games/THERMOVR/
+-rw-r--r--   0 runner    (1001) docker     (127)        3 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/THERMOVR/DBExport.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5667 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/THERMOVR/ThermoVRLoader.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/THERMOVR/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:05:05.055023 opengamedata_core-0.0.6/src/ogd/games/THERMOVR/detectors/
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/THERMOVR/detectors/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:05:05.059023 opengamedata_core-0.0.6/src/ogd/games/THERMOVR/features/
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/THERMOVR/features/LabCompleteCount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1891 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/THERMOVR/features/LeftHandMoves.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/THERMOVR/features/PhasesReached.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/THERMOVR/features/PlayMode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1896 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/THERMOVR/features/RightHandMoves.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/THERMOVR/features/TaskCompleteCount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1760 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/THERMOVR/features/ToolNudgeCount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1700 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/THERMOVR/features/ToolSliderTime.py
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/THERMOVR/features/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:05:05.059023 opengamedata_core-0.0.6/src/ogd/games/THERMOVR/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)    51378 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/THERMOVR/schemas/THERMOVR.json.template
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:05:05.059023 opengamedata_core-0.0.6/src/ogd/games/TRANSFORMATION_QUEST/
+-rw-r--r--   0 runner    (1001) docker     (127)      777 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/TRANSFORMATION_QUEST/DBExport.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:05:05.059023 opengamedata_core-0.0.6/src/ogd/games/TRANSFORMATION_QUEST/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)    25177 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/TRANSFORMATION_QUEST/schemas/TRANSFORMATION_QUEST.json.template
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:05:05.059023 opengamedata_core-0.0.6/src/ogd/games/WAVES/
+-rw-r--r--   0 runner    (1001) docker     (127)    37336 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/WAVES/WaveLoader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:05:05.067022 opengamedata_core-0.0.6/src/ogd/games/WAVES/features/
+-rw-r--r--   0 runner    (1001) docker     (127)     1710 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/WAVES/features/AmplitudeGoodMoveCount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1425 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/WAVES/features/AverageFails.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3489 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/WAVES/features/AverageLevelTime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1876 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/WAVES/features/AverageMoveTypeChanges.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1478 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/WAVES/features/AverageSliderMoves.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/WAVES/features/BeginCount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2014 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/WAVES/features/ClosenessIntercept.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/WAVES/features/ClosenessR2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/WAVES/features/ClosenessSlope.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/WAVES/features/Completed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1194 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/WAVES/features/FirstMoveType.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1168 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/WAVES/features/MenuButtonCount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1704 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/WAVES/features/OffsetGoodMoveCount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/WAVES/features/OverallPercentAmplitudeMoves.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/WAVES/features/OverallPercentOffsetMoves.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1451 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/WAVES/features/OverallPercentWavelengthMoves.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1319 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/WAVES/features/OverallSliderAverageRange.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1315 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/WAVES/features/OverallSliderAverageStandardDeviations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1921 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/WAVES/features/PercentAmplitudeGoodMoves.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/WAVES/features/PercentAmplitudeMoves.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1903 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/WAVES/features/PercentOffsetGoodMoves.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1327 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/WAVES/features/PercentOffsetMoves.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1845 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/WAVES/features/PercentWavelengthGoodMoves.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/WAVES/features/PercentWavelengthMoves.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/WAVES/features/PersistentSessionID.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/WAVES/features/QuestionAnswered.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/WAVES/features/QuestionCorrect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/WAVES/features/RangeIntercept.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/WAVES/features/RangeR2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/WAVES/features/RangeSlope.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/WAVES/features/SequenceLevel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/WAVES/features/SessionID.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1328 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/WAVES/features/SliderAverageRange.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/WAVES/features/SliderAverageStandardDeviations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/WAVES/features/SucceedCount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2597 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/WAVES/features/TimeToAnswerMS.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/WAVES/features/TotalArrowMoves.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/WAVES/features/TotalFails.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1986 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/WAVES/features/TotalLevelTime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/WAVES/features/TotalMoveTypeChanges.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/WAVES/features/TotalResets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/WAVES/features/TotalSkips.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1192 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/WAVES/features/TotalSliderMoves.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1726 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/WAVES/features/WavelengthGoodMoveCount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2575 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/WAVES/features/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:05:05.067022 opengamedata_core-0.0.6/src/ogd/games/WAVES/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)    21383 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/WAVES/schemas/WAVES.json.template
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:05:04.983023 opengamedata_core-0.0.6/src/ogd/games/WEATHER_STATION/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:05:05.067022 opengamedata_core-0.0.6/src/ogd/games/WEATHER_STATION/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)    34344 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/WEATHER_STATION/schemas/WEATHER_STATION.json.template
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:05:04.983023 opengamedata_core-0.0.6/src/ogd/games/WIND/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:05:05.067022 opengamedata_core-0.0.6/src/ogd/games/WIND/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/WIND/schemas/WIND.json.template
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:05:05.067022 opengamedata_core-0.0.6/src/opengamedata_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4796 2024-05-30 18:05:04.000000 opengamedata_core-0.0.6/src/opengamedata_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    22284 2024-05-30 18:05:04.000000 opengamedata_core-0.0.6/src/opengamedata_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 18:05:04.000000 opengamedata_core-0.0.6/src/opengamedata_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-30 18:05:04.000000 opengamedata_core-0.0.6/src/opengamedata_core.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:05:05.067022 opengamedata_core-0.0.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3113 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/tests/test_lakeland_models.py
```

### Comparing `opengamedata_core-0.0.5/LICENSE` & `opengamedata_core-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.5/PKG-INFO` & `opengamedata_core-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opengamedata-core
-Version: 0.0.5
+Version: 0.0.6
 Summary: A package for retrieving and processing event-based video game data. Additional authors: Nick Spevacek, Renee Li, John McCloskey, Zach Studdiford, Glenn Palmer, Haishuo Chen, Daus, Ameya Kshirsagar, Yunqing Xiao, Erik Harpstead, Manuel Jesus Gomez Moratilla
 Author-email: Luke Swanson <superscription58@gmail.com>, David Gagnon <djgagnon@wisc.edu>
 Project-URL: Homepage, https://github.com/opengamedata/opengamedata-core
 Project-URL: Bug Tracker, https://github.com/opengamedata/opengamedata-core/issues
 Project-URL: Documentation, https://opengamedata-doc.readthedocs.io/en/latest/index.html
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `opengamedata_core-0.0.5/README.md` & `opengamedata_core-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.5/pyproject.toml` & `opengamedata_core-0.0.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.5/src/ogd/core/exec/Commands.py` & `opengamedata_core-0.0.6/src/ogd/core/exec/Commands.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,17 +17,17 @@
 from ogd.core.interfaces.outerfaces.TSVOuterface import TSVOuterface
 from ogd.core.interfaces.outerfaces.DebugOuterface import DebugOuterface
 from ogd.core.managers.ExportManager import ExportManager
 from ogd.core.requests.RequestResult import RequestResult, ResultStatus
 from ogd.core.requests.Request import Request, ExporterRange
 from ogd.core.schemas.configs.ConfigSchema import ConfigSchema
 from ogd.core.schemas.configs.GameSourceSchema import GameSourceSchema
-from ogd.core.schemas.ExportMode import ExportMode
+from ogd.core.models.enums.ExportMode import ExportMode
 from ogd.core.schemas.games.GameSchema import GameSchema
-from ogd.core.schemas.IDMode import IDMode
+from ogd.core.models.enums.IDMode import IDMode
 from ogd.core.schemas.tables.TableSchema import TableSchema
 from ogd.core.utils.Logger import Logger
 from ogd.core.utils.Readme import Readme
 
 class OGDCommands:
     """Utility class to collect functions for each of the commands that can be run when executing ogd-core as a module.
     """
@@ -100,63 +100,68 @@
 
         export_modes   : Set[ExportMode]
         interface      : DataInterface
         range          : ExporterRange
         file_outerface : DataOuterface
         dataset_id     : Optional[str] = None
 
-        # 1. get exporter modes to run
+    # 1. get exporter modes to run
         export_modes = OGDGenerators.genModes(with_events=with_events, with_features=with_features,
                                               no_session_file=args.no_session_file, no_player_file=args.no_player_file, no_pop_file=args.no_pop_file)
-        # 2. figure out the interface and range; optionally set a different dataset_id
+    # 2. figure out the interface and range; optionally set a different dataset_id
         if args.file is not None and args.file != "":
             # raise NotImplementedError("Sorry, exports with file inputs are currently broken.")
             _ext = str(args.file).split('.')[-1]
             _cfg = GameSourceSchema(name="FILE SOURCE", all_elements={"schema":"OGD_EVENT_FILE"}, data_sources={})
             interface = CSVInterface(game_id=args.game, config=_cfg, fail_fast=config.FailFast, filepath=Path(args.file), delim="\t" if _ext == 'tsv' else ',')
             # retrieve/calculate id range.
             ids = interface.AllIDs()
             range = ExporterRange.FromIDs(source=interface, ids=ids if ids is not None else [])
         else:
             interface = OGDGenerators.genDBInterface(config=config, game=args.game)
+        # a. Case where specific player ID was given
             if args.player is not None and args.player != "":
                 range = ExporterRange.FromIDs(source=interface, ids=[args.player], id_mode=IDMode.USER)
                 dataset_id = f"{args.game}_{args.player}"
+        # b. Case where player ID file was given
             elif args.player_id_file is not None and args.player_id_file != "":
                 file_path = Path(args.player_id_file)
                 with open(file_path) as player_file:
                     reader = csv.reader(player_file)
                     file_contents = list(reader) # this gives list of lines, each line a list
                     names = list(chain.from_iterable(file_contents)) # so, convert to single list
                     print(f"list of names: {list(names)}")
                     range = ExporterRange.FromIDs(source=interface, ids=names, id_mode=IDMode.USER)
+        # c. Case where specific session ID was given
             elif args.session is not None and args.session != "":
                 range = ExporterRange.FromIDs(source=interface, ids=[args.session], id_mode=IDMode.SESSION)
                 dataset_id = f"{args.game}_{args.session}"
+        # d. Case where session ID file was given
             elif args.session_id_file is not None and args.session_id_file != "":
                 file_path = Path(args.session_id_file)
                 with open(file_path) as session_file:
                     reader = csv.reader(session_file)
                     file_contents = list(reader) # this gives list of lines, each line a list
                     names = list(chain.from_iterable(file_contents)) # so, convert to single list
                     print(f"list of sessions: {list(names)}")
                     range = ExporterRange.FromIDs(source=interface, ids=names, id_mode=IDMode.SESSION)
+        # e. Default case where we use date range
             else:
                 range = OGDGenerators.genDateRange(game=args.game, interface=interface, monthly=args.monthly, start_date=args.start_date, end_date=args.end_date)
-        # 3. set up the outerface, based on the range and dataset_id.
+    # 3. set up the outerface, based on the range and dataset_id.
         _cfg = GameSourceSchema(name="FILE DEST", all_elements={"database":"FILE", "table":"DEBUG", "schema":"OGD_EVENT_FILE"}, data_sources={})
         file_outerface = TSVOuterface(game_id=args.game, config=_cfg, export_modes=export_modes, date_range=range.DateRange,
                                     file_indexing=config.FileIndexConfig, dataset_id=dataset_id)
         outerfaces : Set[DataOuterface] = {file_outerface}
         # If we're in debug level of output, include a debug outerface, so we know what is *supposed* to go through the outerfaces.
         if config.DebugLevel == "DEBUG":
             _cfg = GameSourceSchema(name="DEBUG", all_elements={"database":"DEBUG", "table":"DEBUG", "schema":"OGD_EVENT_FILE"}, data_sources={})
             outerfaces.add(DebugOuterface(game_id=args.game, config=_cfg, export_modes=export_modes))
 
-        # 4. Once we have the parameters parsed out, construct the request.
+    # 4. Once we have the parameters parsed out, construct the request.
         req = Request(range=range, exporter_modes=export_modes, interface=interface, outerfaces=outerfaces)
         if req.Interface.IsOpen():
             export_manager : ExportManager = ExportManager(config=config)
             result         : RequestResult = export_manager.ExecuteRequest(request=req)
             success = result.Status == ResultStatus.SUCCESS
             level = logging.INFO if success else logging.ERROR
             Logger.Log(message=result.Message, level=level)
```

### Comparing `opengamedata_core-0.0.5/src/ogd/core/exec/Generators.py` & `opengamedata_core-0.0.6/src/ogd/core/exec/Generators.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # import local files
 from ogd.core.interfaces.DataInterface import DataInterface
 from ogd.core.interfaces.MySQLInterface import MySQLInterface
 from ogd.core.interfaces.BigQueryInterface import BigQueryInterface
 from ogd.core.interfaces.BQFirebaseInterface import BQFirebaseInterface
 from ogd.core.requests.Request import ExporterRange
 from ogd.core.schemas.configs.ConfigSchema import ConfigSchema
-from ogd.core.schemas.ExportMode import ExportMode
+from ogd.core.models.enums.ExportMode import ExportMode
 from ogd.core.utils.Logger import Logger
 
 class OGDGenerators:
     @staticmethod
     def genDBInterface(config:ConfigSchema, game:str) -> DataInterface:
         ret_val : DataInterface
         _game_cfg = config.GameSourceMap.get(game)
@@ -72,9 +72,11 @@
             Logger.Log(f"Exporting {month}/{year} data for {game}...", logging.DEBUG)
         # Otherwise, create date range from given pair of dates.
         else:
             _from = datetime.strptime(start_date, "%m/%d/%Y") if start_date is not None else today
             _from = _from.replace(hour=0, minute=0, second=0)
             _to   = datetime.strptime(end_date, "%m/%d/%Y") if end_date is not None else _from
             _to = _to.replace(hour=23, minute=59, second=59)
+            if _from > _to:
+                raise ValueError(f"Invalid date range, start date of {_from} is after end date of {_to}!")
             Logger.Log(f"Exporting from {str(_from)} to {str(_to)} of data for {game}...", logging.INFO)
         return ExporterRange.FromDateRange(source=interface, date_min=_from, date_max=_to)
```

### Comparing `opengamedata_core-0.0.5/src/ogd/core/exec/Parsers.py` & `opengamedata_core-0.0.6/src/ogd/core/exec/Parsers.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.5/src/ogd/core/games/AQUALAB/features/AppVersions.py` & `opengamedata_core-0.0.6/src/ogd/games/AQUALAB/features/AppVersions.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 from typing import Any, List
 
-from extractors.Extractor import ExtractorParameters
-from extractors.features.SessionFeature import SessionFeature
-from schemas.Event import Event
-from schemas.ExtractionMode import ExtractionMode
-from schemas.FeatureData import FeatureData
+from ogd.core.generators.Generator import GeneratorParameters
+from ogd.core.generators.extractors.SessionFeature import SessionFeature
+from ogd.core.models.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
+from ogd.core.models.FeatureData import FeatureData
 
 class AppVersions(SessionFeature):
     """_summary_
 
     :param SessionFeature: _description_
     :type SessionFeature: _type_
     """
-    def __init__(self, params:ExtractorParameters):
+    def __init__(self, params:GeneratorParameters):
         super().__init__(params=params)
         self._versions = set()
 
     # *** IMPLEMENT ABSTRACT FUNCTIONS ***
     @classmethod
-    def _getEventDependencies(cls, mode:ExtractionMode) -> List[str]:
+    def _eventFilter(cls, mode:ExtractionMode) -> List[str]:
         return ["all_events"]
 
     @classmethod
-    def _getFeatureDependencies(cls, mode:ExtractionMode) -> List[str]:
+    def _featureFilter(cls, mode:ExtractionMode) -> List[str]:
         return []
 
-    def _extractFromEvent(self, event:Event) -> None:
+    def _updateFromEvent(self, event:Event) -> None:
         self._versions.add(event.AppVersion)
 
-    def _extractFromFeatureData(self, feature:FeatureData):
+    def _updateFromFeatureData(self, feature:FeatureData):
         return
 
     def _getFeatureValues(self) -> List[Any]:
         return [list(self._versions)]
 
-    # *** Optionally override public functions. ***
+    # *** Optionally override public functions. ***
```

### Comparing `opengamedata_core-0.0.5/src/ogd/core/games/AQUALAB/features/PlayLocations.py` & `opengamedata_core-0.0.6/src/ogd/core/games/AQUALAB/features/PlayLocations.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import logging
 from typing import Any, List
 
-from extractors.Extractor import ExtractorParameters
-from extractors.features.SessionFeature import SessionFeature
-from schemas.Event import Event
-from schemas.ExtractionMode import ExtractionMode
-from schemas.FeatureData import FeatureData
+from ogd.core.generators.Generator import GeneratorParameters
+from ogd.core.generators.extractors.SessionFeature import SessionFeature
+from ogd.core.models.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
+from ogd.core.models.FeatureData import FeatureData
 from utils.Logger import Logger
 
 
 
 class InSchoolSessions(SessionFeature):
     """A feature that determines whether a session started in school or not."""
 
@@ -57,15 +57,15 @@
             self._in_school_sessions.append(in_school)
 
             
     def _getFeatureValues(self) -> List[Any]:
         # Sessions that started in school
         return [self._in_school_sessions, self._session_times]
 
-    def __init__(self, params: ExtractorParameters):
+    def __init__(self, params: GeneratorParameters):
         super().__init__(params=params)
 
         # sessions that have been seen before.
         self._seen_sessions = set()
         # sessions that started in school.
         self._in_school_sessions = []
         self._session_times = []
```

### Comparing `opengamedata_core-0.0.5/src/ogd/core/games/JOURNALISM/features/FailureAttributes.py` & `opengamedata_core-0.0.6/src/ogd/games/JOURNALISM/features/FailureAttributes.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 # import libraries
 import json
 from typing import Any, Dict, List, Optional
 # import local files
-from extractors.features.Feature import Feature
-from extractors.features.PerLevelFeature import PerLevelFeature
-from schemas.Event import Event
-from schemas.ExtractionMode import ExtractionMode
-from schemas.FeatureData import FeatureData
-from extractors.Extractor import ExtractorParameters
-from extractors.features.SessionFeature import SessionFeature
+from ogd.core.generators.extractors.Feature import Feature
+from ogd.core.generators.extractors.PerLevelFeature import PerLevelFeature
+from ogd.core.models.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
+from ogd.core.models.FeatureData import FeatureData
+from ogd.core.generators.Generator import GeneratorParameters
+from ogd.core.generators.extractors.SessionFeature import SessionFeature
 
 
 
 
 class FailureAttributes(PerLevelFeature):
     """Per-level feature to generate a list of failures, where each failure in the list is the set of player attributes
 
     :param PerLevelFeature: Base class for a Custom Feature class.
     :type PerLevelFeature: _type_
     """
-    def __init__(self, params:ExtractorParameters):
+    def __init__(self, params:GeneratorParameters):
         super().__init__(params=params)
         PerLevelFeature.__init__(self, params=params)
 
         self._fails : List[Dict[str, int]] = []
 
     # *** IMPLEMENT ABSTRACT FUNCTIONS ***
     @classmethod
```

### Comparing `opengamedata_core-0.0.5/src/ogd/core/games/JOURNALISM/features/FinalAttributes.py` & `opengamedata_core-0.0.6/src/ogd/games/JOURNALISM/features/FinalAttributes.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 # import libraries
 import json
-from extractors.features.PerCountFeature import PerCountFeature
-from schemas import Event
 from typing import Any, Dict, List, Optional
 # import locals
-from extractors.features.PerLevelFeature import PerLevelFeature
-from extractors.Extractor import ExtractorParameters
-from schemas.Event import Event
-from schemas.ExtractionMode import ExtractionMode
-from schemas.FeatureData import FeatureData
+from ogd.core.generators.extractors.PerLevelFeature import PerLevelFeature
+from ogd.core.generators.Generator import GeneratorParameters
+from ogd.core.generators.extractors.PerCountFeature import PerCountFeature
+from ogd.core.models.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
+from ogd.core.models.FeatureData import FeatureData
 
 class FinalAttributes(PerLevelFeature):
-    def __init__(self, params:ExtractorParameters):
+    def __init__(self, params:GeneratorParameters):
         PerCountFeature.__init__(self, params=params)
         self._ATTRIBUTE_ENUM : List[str] = ["endurance", "resourceful", "tech","social","trust","research"]
         self._last_attribs : Dict[str, Optional[int]] = dict(zip(self._ATTRIBUTE_ENUM, [None]*len(self._ATTRIBUTE_ENUM)))
 
 
     # *** IMPLEMENT ABSTRACT FUNCTIONS ***
```

### Comparing `opengamedata_core-0.0.5/src/ogd/core/generators/Generator.py` & `opengamedata_core-0.0.6/src/ogd/core/generators/Generator.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 ## import standard libraries
 import abc
 import logging
 from typing import List, Optional
 # import locals
-from ogd.core.schemas.Event import Event
-from ogd.core.schemas.ExtractionMode import ExtractionMode
+from ogd.core.models.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
 from ogd.core.utils.Logger import Logger
 
 ## @class ExtractorParams
 class GeneratorParameters:
     """Dumb struct to hold the data that should be available to every Generator.
     This just makes it easier to add/manage any new params,
     so that we don't need to change the param list for hundreds of individual
```

### Comparing `opengamedata_core-0.0.5/src/ogd/core/generators/GeneratorLoader.py` & `opengamedata_core-0.0.6/src/ogd/core/generators/GeneratorLoader.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 import logging
 from importlib import import_module
 from typing import Any, Callable, Dict, List, Optional, Type
 # import locals
 from ogd.core.generators.Generator import Generator, GeneratorParameters
 from ogd.core.generators.detectors.Detector import Detector
 from ogd.core.generators.extractors.Extractor import Extractor
-from ogd.core.schemas.Event import Event
-from ogd.core.schemas.ExtractionMode import ExtractionMode
+from ogd.core.models.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
 from ogd.core.schemas.games.GameSchema import GameSchema
 from ogd.core.utils.Logger import Logger
 
 class GeneratorLoader(abc.ABC):
 
     # *** ABSTRACTS ***
```

### Comparing `opengamedata_core-0.0.5/src/ogd/core/generators/detectors/Detector.py` & `opengamedata_core-0.0.6/src/ogd/core/generators/detectors/Detector.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 ## import standard libraries
 import abc
 from datetime import datetime, timedelta
 from typing import Any, Callable, Dict, List, Optional
 # import locals
 from ogd.core.generators.Generator import Generator, GeneratorParameters
 from ogd.core.generators.detectors.DetectorEvent import DetectorEvent
-from ogd.core.schemas.Event import Event
-from ogd.core.schemas.ExtractionMode import ExtractionMode
+from ogd.core.models.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
 from ogd.core.utils.typing import Map
 
 ## @class Model
 #  Abstract base class for session-level Wave Detectors.
 #  Models only have one public function, called Eval.
 #  The Eval function takes a list of row data, computes some statistic, and returns a list of results.
 #  If the model works on Detectors from session data, it should calculate one result for each row (each row being a session).
```

### Comparing `opengamedata_core-0.0.5/src/ogd/core/generators/detectors/DetectorEvent.py` & `opengamedata_core-0.0.6/src/ogd/core/generators/detectors/DetectorEvent.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # import libraries
 import abc
 from datetime import datetime, timedelta
 from typing import Any, Dict, Optional
 # import locals
-from ogd.core.schemas.Event import Event, EventSource
+from ogd.core.models.Event import Event, EventSource
 from ogd.core.utils.typing import Map
 
 class DetectorEvent(Event):
    def __init__(self, session_id:str,      app_id:str,
                 event_name:str,            event_data:Map,
                 timestamp:datetime,        time_offset:Optional[timedelta],
                 app_version:Optional[str], log_version:Optional[str],
```

### Comparing `opengamedata_core-0.0.5/src/ogd/core/generators/extractors/Extractor.py` & `opengamedata_core-0.0.6/src/ogd/core/generators/extractors/Extractor.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 ## import standard libraries
 import abc
 from typing import Any, Dict, List, Optional
 # import locals
 from ogd.core.generators.Generator import Generator, GeneratorParameters
-from ogd.core.schemas.Event import Event
-from ogd.core.schemas.ExtractionMode import ExtractionMode
-from ogd.core.schemas.FeatureData import FeatureData
+from ogd.core.models.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
+from ogd.core.models.FeatureData import FeatureData
 
 class Extractor(Generator):
     """
     Base class for feature extractors.
 
     In addition to event/feature filters and an update-from-event rule,
     the Feature base class requires subclasses to implement an update-from-feature rule and a calculate rule.
```

### Comparing `opengamedata_core-0.0.5/src/ogd/core/generators/extractors/Feature.py` & `opengamedata_core-0.0.6/src/ogd/core/generators/extractors/Feature.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.5/src/ogd/core/generators/extractors/PerCountFeature.py` & `opengamedata_core-0.0.6/src/ogd/core/generators/extractors/PerCountFeature.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # import standard libraries
 import abc
 from multiprocessing.sharedctypes import Value
 # import locals
 from ogd.core.generators.Generator import GeneratorParameters
 from ogd.core.generators.extractors.Feature import Feature
-from ogd.core.schemas.Event import Event
+from ogd.core.models.Event import Event
 
 ## @class PerLevelFeature
 class PerCountFeature(Feature):
     """PerLevelFeature
     Abstract base class for per-level game features.
     Works like a normal Feature, but checks if the given event has right "level"
     before attempting to extract from event.
```

### Comparing `opengamedata_core-0.0.5/src/ogd/core/generators/extractors/PerLevelFeature.py` & `opengamedata_core-0.0.6/src/ogd/core/generators/extractors/PerLevelFeature.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # import locals
 from ogd.core.generators.Generator import GeneratorParameters
 from ogd.core.generators.extractors.PerCountFeature import PerCountFeature
-from ogd.core.schemas.Event import Event
-from ogd.core.schemas.ExtractionMode import ExtractionMode
+from ogd.core.models.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
 
 ## @class PerLevelFeature
 class PerLevelFeature(PerCountFeature):
     """PerLevelFeature
     Abstract base class for per-level game features.
     Works like a normal Feature, but checks if the given event has right "level"
     before attempting to extract from event.
```

### Comparing `opengamedata_core-0.0.5/src/ogd/core/generators/extractors/SessionFeature.py` & `opengamedata_core-0.0.6/src/ogd/core/generators/extractors/SessionFeature.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.5/src/ogd/core/generators/legacy/LegacyDetector.py` & `opengamedata_core-0.0.6/src/ogd/core/generators/legacy/LegacyDetector.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # import standard libraries
 from datetime import datetime
 from typing import Any, List, Optional
 # import local files
 from ogd.core.generators.detectors.Detector import Detector
 from ogd.core.generators.Generator import GeneratorParameters
-from ogd.core.schemas.Event import EventSource
-from ogd.core.schemas.Event import Event
-from ogd.core.schemas.ExtractionMode import ExtractionMode
+from ogd.core.models.Event import EventSource
+from ogd.core.models.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
 
 class LegacyDetector(Detector):
     """Dummy version of a detector, so that LegacyLoader can return something that's not None.
     """
 
     # *** IMPLEMENT ABSTRACT FUNCTIONS ***
```

### Comparing `opengamedata_core-0.0.5/src/ogd/core/generators/legacy/LegacyFeature.py` & `opengamedata_core-0.0.6/src/ogd/core/generators/legacy/LegacyFeature.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 from collections import defaultdict
 from datetime import timedelta
 from typing import Any, Dict, List, Optional, Union
 ## import local files
 from ogd.core.utils.Logger import Logger
 from ogd.core.generators.Generator import GeneratorParameters
 from ogd.core.generators.extractors.Feature import Feature
-from ogd.core.schemas.ExtractionMode import ExtractionMode
-from ogd.core.schemas.FeatureData import FeatureData
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
+from ogd.core.models.FeatureData import FeatureData
 from ogd.core.schemas.games.GameSchema import GameSchema
 
 LegacyFeatureType = Union[int,float,timedelta,Dict[int,Dict[str,Any]]]
 
 ## @class LegacyFeature
 #  Abstract base class for game feature extractors.
 #  Gives a few static functions to be used across all extractor classes,
```

### Comparing `opengamedata_core-0.0.5/src/ogd/core/generators/legacy/LegacyLoader.py` & `opengamedata_core-0.0.6/src/ogd/core/generators/legacy/LegacyLoader.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # import libraries
 from typing import List, Optional, Type
 # import locals
 from ogd.core.generators.GeneratorLoader import GeneratorLoader
 from ogd.core.generators.extractors.Feature import Feature
-from ogd.core.schemas.ExtractionMode import ExtractionMode
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
 from ogd.core.schemas.games.GameSchema import GameSchema
 
 class LegacyLoader(GeneratorLoader):
     def __init__(self, player_id:str, session_id:str, game_schema:GameSchema, mode:ExtractionMode, feature_overrides:Optional[List[str]]):
         super().__init__(player_id=player_id, session_id=session_id, game_schema=game_schema, mode=mode, feature_overrides=feature_overrides)
 
     def GetFeatureClass(self, feature_type:str) -> Optional[Type[Feature]]:
```

### Comparing `opengamedata_core-0.0.5/src/ogd/core/generators/registries/DetectorRegistry.py` & `opengamedata_core-0.0.6/src/ogd/core/generators/registries/DetectorRegistry.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,20 +3,20 @@
 from collections import OrderedDict
 from typing import Any, Callable, List, Optional, Set
 ## import local files
 from ogd.core.generators.detectors.Detector import Detector
 from ogd.core.generators.Generator import Generator
 from ogd.core.generators.GeneratorLoader import GeneratorLoader
 from ogd.core.generators.registries.GeneratorRegistry import GeneratorRegistry
-from ogd.core.schemas.Event import Event
-from ogd.core.schemas.ExtractionMode import ExtractionMode
-from ogd.core.schemas.FeatureData import FeatureData
+from ogd.core.models.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
+from ogd.core.models.FeatureData import FeatureData
 from ogd.core.schemas.games.DetectorSchema import DetectorSchema
 from ogd.core.schemas.games.GameSchema import GameSchema
-from ogd.core.schemas.IterationMode import IterationMode
+from ogd.core.models.enums.IterationMode import IterationMode
 
 ## @class Extractor
 #  Abstract base class for game feature extractors.
 #  Gives a few static functions to be used across all extractor classes,
 #  and defines an interface that the SessionProcessor can use.
 class DetectorRegistry(GeneratorRegistry):
     """Class for registering features to listen for events.
```

### Comparing `opengamedata_core-0.0.5/src/ogd/core/generators/registries/ExtractorRegistry.py` & `opengamedata_core-0.0.6/src/ogd/core/generators/registries/ExtractorRegistry.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,19 +7,19 @@
 from typing import Any, Dict, List, Optional, Set
 ## import local files
 from ogd.core.generators.Generator import Generator
 from ogd.core.generators.GeneratorLoader import GeneratorLoader
 from ogd.core.generators.extractors.PerCountFeature import PerCountFeature
 from ogd.core.generators.registries.GeneratorRegistry import GeneratorRegistry
 from ogd.core.generators.extractors.Feature import Feature
-from ogd.core.schemas.Event import Event
-from ogd.core.schemas.ExtractionMode import ExtractionMode
-from ogd.core.schemas.FeatureData import FeatureData
+from ogd.core.models.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
+from ogd.core.models.FeatureData import FeatureData
 from ogd.core.schemas.games.GameSchema import GameSchema
-from ogd.core.schemas.IterationMode import IterationMode
+from ogd.core.models.enums.IterationMode import IterationMode
 from ogd.core.schemas.games.AggregateSchema import AggregateSchema
 from ogd.core.schemas.games.PerCountSchema import PerCountSchema
 from ogd.core.utils.Logger import Logger
 
 ## @class Extractor
 #  Abstract base class for game feature extractors.
 #  Gives a few static functions to be used across all extractor classes,
```

### Comparing `opengamedata_core-0.0.5/src/ogd/core/generators/registries/GeneratorRegistry.py` & `opengamedata_core-0.0.6/src/ogd/core/generators/registries/GeneratorRegistry.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 import abc
 import logging
 from typing import Any, Dict, List, Optional
 from ogd.core.generators.GeneratorLoader import GeneratorLoader
 ## import local files
 from ogd.core.utils.Logger import Logger
 from ogd.core.generators.Generator import Generator
-from ogd.core.schemas.Event import Event
-from ogd.core.schemas.ExtractionMode import ExtractionMode
-from ogd.core.schemas.FeatureData import FeatureData
+from ogd.core.models.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
+from ogd.core.models.FeatureData import FeatureData
 from ogd.core.schemas.games.GameSchema import GameSchema
-from ogd.core.schemas.IterationMode import IterationMode
+from ogd.core.models.enums.IterationMode import IterationMode
 
 ## @class Extractor
 #  Abstract base class for game feature extractors.
 #  Gives a few static functions to be used across all extractor classes,
 #  and defines an interface that the SessionProcessor can use.
 class GeneratorRegistry(abc.ABC):
     """Class for registering features to listen for events.
```

### Comparing `opengamedata_core-0.0.5/src/ogd/core/interfaces/BQFirebaseInterface.py` & `opengamedata_core-0.0.6/src/ogd/core/interfaces/BQFirebaseInterface.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import logging
 import os
 from datetime import datetime
 from typing import Dict, Final, List, Tuple, Optional
 # import locals
 from ogd.core.interfaces.BigQueryInterface import BigQueryInterface
-from ogd.core.schemas.IDMode import IDMode
+from ogd.core.models.enums.IDMode import IDMode
 from ogd.core.schemas.configs.GameSourceSchema import GameSourceSchema
 from ogd.core.utils.Logger import Logger
 
 AQUALAB_MIN_VERSION : Final[float] = 6.2
 
 class BQFirebaseInterface(BigQueryInterface):
     """Subclass of the general BigQueryInterface, with re-implemented queries to handle old Firebase unnest bullshit.
@@ -62,15 +62,15 @@
                 items = tuple(row.items())
                 event = []
                 for item in items:
                     match item[0]:
                         case "event_params":
                             _params = {param['key']:param['value'] for param in item[1]}
                             event.append(json.dumps(_params, sort_keys=True))
-                        case "device" | "geo":
+                        case "device":
                             event.append(json.dumps(item[1], sort_keys=True))
                         case _:
                             event.append(item[1])
                 events.append(tuple(event))
         return events if events != None else []
 
     def _IDsFromDates(self, min:datetime, max:datetime, versions:Optional[List[int]] = None) -> List[str]:
@@ -179,15 +179,15 @@
                     AND   {session_clause}
                     AND   {player_clause}"""
     # 4) Set up actual query
         query = ""
         match self._game_id:
             case "SHADOWSPECT" | "SHIPWRECKS":
                 query = f"""
-                    SELECT event_name, event_params, device, geo, platform,
+                    SELECT event_name, event_params, device, platform,
                     concat(FORMAT_DATE('%Y-%m-%d', PARSE_DATE('%Y%m%d', event_date)), FORMAT_TIME('T%H:%M:%S.00', TIME(TIMESTAMP_MICROS(event_timestamp)))) AS timestamp,
                     null as app_version,
                     null as log_version,
                     param_session.value.int_value as session_id,
                     null as fd_user_id
                     FROM `{self.DBPath()}`
                     CROSS JOIN UNNEST(event_params) AS param_session
@@ -196,15 +196,15 @@
                 """
             case _:
                 # TODO Order by user_id, and by timestamp within that.
                 # Note that this could prove to be wonky when we have more games without user ids,
                 # will need to really rethink this when we start using new system.
                 # Still, not a huge deal because most of these will be rewritten at that time anyway.
                 query = f"""
-                    SELECT event_name, event_params, device, geo, platform,
+                    SELECT event_name, event_params, device, platform,
                     concat(FORMAT_DATE('%Y-%m-%d', PARSE_DATE('%Y%m%d', event_date)), FORMAT_TIME('T%H:%M:%S.00', TIME(TIMESTAMP_MICROS(event_timestamp)))) AS timestamp,
                     param_app_version.value.string_value as app_version,
                     param_log_version.value.int_value as log_version,
                     param_session.value.int_value as session_id,
                     param_user.value.string_value as fd_user_id
                     FROM `{self.DBPath()}`
                     CROSS JOIN UNNEST(event_params) AS param_app_version
```

### Comparing `opengamedata_core-0.0.5/src/ogd/core/interfaces/BigQueryCodingInterface.py` & `opengamedata_core-0.0.6/src/ogd/core/interfaces/BigQueryCodingInterface.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from datetime import datetime
 from google.cloud import bigquery
 from typing import Dict, List, Tuple, Optional
 # import locals
 from coding.Code import Code
 from coding.Coder import Coder
 from ogd.core.interfaces.CodingInterface import CodingInterface
-from ogd.core.schemas.IDMode import IDMode
+from ogd.core.models.enums.IDMode import IDMode
 from ogd.core.schemas.configs.ConfigSchema import ConfigSchema
 from ogd.core.utils.Logger import Logger
 
 # TODO: see about merging this back into BigQueryInterface for a unified interface.
 
 class BigQueryCodingInterface(CodingInterface):
```

### Comparing `opengamedata_core-0.0.5/src/ogd/core/interfaces/BigQueryInterface.py` & `opengamedata_core-0.0.6/src/ogd/core/interfaces/BigQueryInterface.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 from datetime import datetime, date
 from google.cloud import bigquery
 from google.api_core.exceptions import BadRequest
 from typing import Dict, Final, List, Tuple, Optional
 # import locals
 from ogd.core.interfaces.DataInterface import DataInterface
-from ogd.core.schemas.IDMode import IDMode
+from ogd.core.models.enums.IDMode import IDMode
 from ogd.core.schemas.configs.GameSourceSchema import GameSourceSchema
 from ogd.core.schemas.configs.data_sources.BigQuerySourceSchema import BigQuerySchema
 from ogd.core.utils.Logger import Logger
 
 AQUALAB_MIN_VERSION : Final[float] = 6.2
 
 class BigQueryInterface(DataInterface):
@@ -102,15 +102,15 @@
                     items = tuple(row.items())
                     event = []
                     for item in items:
                         match item[0]:
                             case "event_params":
                                 _params = {param['key']:param['value'] for param in item[1]}
                                 event.append(json.dumps(_params, sort_keys=True))
-                            case "device" | "geo":
+                            case "device":
                                 event.append(json.dumps(item[1], sort_keys=True))
                             case _:
                                 event.append(item[1])
                     ret_val.append(tuple(event))
         return ret_val
 
     def _IDsFromDates(self, min:datetime, max:datetime, versions:Optional[List[int]] = None) -> List[str]:
```

### Comparing `opengamedata_core-0.0.5/src/ogd/core/interfaces/CSVInterface.py` & `opengamedata_core-0.0.6/src/ogd/core/interfaces/CSVInterface.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import pandas as pd
 from datetime import datetime
 from pandas.io.parsers import TextFileReader
 from pathlib import Path
 from typing import Any, Dict, IO, List, Tuple, Optional
 ## import local files
 from ogd.core.interfaces.DataInterface import DataInterface
-from ogd.core.schemas.IDMode import IDMode
+from ogd.core.models.enums.IDMode import IDMode
 from ogd.core.schemas.configs.GameSourceSchema import GameSourceSchema
 from ogd.core.schemas.tables.TableSchema import TableSchema
 from ogd.core.utils.Logger import Logger
 
 class CSVInterface(DataInterface):
 
     # *** BUILT-INS & PROPERTIES ***
```

### Comparing `opengamedata_core-0.0.5/src/ogd/core/interfaces/CodingInterface.py` & `opengamedata_core-0.0.6/src/ogd/core/interfaces/CodingInterface.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from enum import IntEnum
 from typing import Dict, List, Tuple, Optional
 
 # import local files
 from coding.Code import Code
 from coding.Coder import Coder
 from ogd.core.interfaces.Interface import Interface
-from ogd.core.schemas.IDMode import IDMode
+from ogd.core.models.enums.IDMode import IDMode
 from ogd.core.utils.Logger import Logger
 
 class CodingInterface(Interface):
 
     # *** ABSTRACTS ***
 
     @abc.abstractmethod
```

### Comparing `opengamedata_core-0.0.5/src/ogd/core/interfaces/DataInterface.py` & `opengamedata_core-0.0.6/src/ogd/core/interfaces/DataInterface.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 import logging
 from datetime import datetime
 from pprint import pformat
 from typing import Any, Dict, List, Tuple, Optional, Union
 
 # import local files
 from ogd.core.interfaces.Interface import Interface
-from ogd.core.schemas.Event import Event
-from ogd.core.schemas.IDMode import IDMode
+from ogd.core.models.Event import Event
+from ogd.core.models.enums.IDMode import IDMode
 from ogd.core.schemas.tables.TableSchema import TableSchema
 from ogd.core.schemas.configs.GameSourceSchema import GameSourceSchema
 from ogd.core.utils.Logger import Logger
 
 class DataInterface(Interface):
 
     # *** ABSTRACTS ***
```

### Comparing `opengamedata_core-0.0.5/src/ogd/core/interfaces/Interface.py` & `opengamedata_core-0.0.6/src/ogd/core/interfaces/Interface.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.5/src/ogd/core/interfaces/MySQLInterface.py` & `opengamedata_core-0.0.6/src/ogd/core/interfaces/MySQLInterface.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import logging
 import sshtunnel
 import traceback
 from datetime import datetime
 from typing import Dict, Final, List, Tuple, Optional
 # import locals
 from ogd.core.interfaces.DataInterface import DataInterface
-from ogd.core.schemas.IDMode import IDMode
+from ogd.core.models.enums.IDMode import IDMode
 from ogd.core.schemas.configs.GameSourceSchema import GameSourceSchema
 from ogd.core.schemas.configs.data_sources.MySQLSourceSchema import MySQLSchema
 from ogd.core.utils.Logger import Logger
 
 
 ## @class SQL
 #  A utility class containing some functions to assist in retrieving from a database.
```

### Comparing `opengamedata_core-0.0.5/src/ogd/core/interfaces/outerfaces/DataOuterface.py` & `opengamedata_core-0.0.6/src/ogd/core/interfaces/outerfaces/DataOuterface.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 ## import standard libraries
 import abc
 import logging
 from typing import Any, Dict, List, Set
 
 # import local files
 from ogd.core.interfaces.Interface import Interface
-from ogd.core.schemas.IDMode import IDMode
-from ogd.core.schemas.ExportMode import ExportMode
+from ogd.core.models.enums.IDMode import IDMode
+from ogd.core.models.enums.ExportMode import ExportMode
 from ogd.core.schemas.configs.GameSourceSchema import GameSourceSchema
 from ogd.core.utils.Logger import Logger
 from ogd.core.utils.utils import ExportRow
 
 class DataOuterface(Interface):
     """Base class for feature and event output.
```

### Comparing `opengamedata_core-0.0.5/src/ogd/core/interfaces/outerfaces/DebugOuterface.py` & `opengamedata_core-0.0.6/src/ogd/core/interfaces/outerfaces/DebugOuterface.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 ## import standard libraries
 import logging
 from typing import List, Set
 
 # import local files
 from ogd.core.interfaces.outerfaces.DataOuterface import DataOuterface
-from ogd.core.schemas.ExportMode import ExportMode
+from ogd.core.models.enums.ExportMode import ExportMode
 from ogd.core.schemas.configs.GameSourceSchema import GameSourceSchema
 from ogd.core.utils.Logger import Logger
 from ogd.core.utils.utils import ExportRow
 
 class DebugOuterface(DataOuterface):
 
     # *** BUILT-INS & PROPERTIES ***
```

### Comparing `opengamedata_core-0.0.5/src/ogd/core/interfaces/outerfaces/DictionaryOuterface.py` & `opengamedata_core-0.0.6/src/ogd/core/interfaces/outerfaces/DictionaryOuterface.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 ## import standard libraries
 import logging
 from typing import Dict, List, Set, Union
 
 # import local files
 from ogd.core.interfaces.outerfaces.DataOuterface import DataOuterface
-from ogd.core.schemas.ExportMode import ExportMode
+from ogd.core.models.enums.ExportMode import ExportMode
 from ogd.core.schemas.configs.GameSourceSchema import GameSourceSchema
 from ogd.core.utils.Logger import Logger
 from ogd.core.utils.utils import ExportRow
 
 class DictionaryOuterface(DataOuterface):
 
     # *** BUILT-INS & PROPERTIES ***
```

### Comparing `opengamedata_core-0.0.5/src/ogd/core/interfaces/outerfaces/TSVOuterface.py` & `opengamedata_core-0.0.6/src/ogd/core/interfaces/outerfaces/TSVOuterface.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,16 +12,16 @@
 from git.exc import InvalidGitRepositoryError, NoSuchPathError
 from pathlib import Path
 from typing import Any, Dict, IO, List, Optional, Set
 
 # import local files
 from ogd import games
 from ogd.core.interfaces.outerfaces.DataOuterface import DataOuterface
-from ogd.core.schemas.ExtractionMode import ExtractionMode
-from ogd.core.schemas.ExportMode import ExportMode
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
+from ogd.core.models.enums.ExportMode import ExportMode
 from ogd.core.schemas.configs.GameSourceSchema import GameSourceSchema
 from ogd.core.schemas.games.GameSchema import GameSchema
 from ogd.core.schemas.tables.TableSchema import TableSchema
 from ogd.core.schemas.configs.IndexingSchema import FileIndexingSchema
 from ogd.core.utils import utils
 from ogd.core.utils.Logger import Logger
 from ogd.core.utils.utils import ExportRow
```

### Comparing `opengamedata_core-0.0.5/src/ogd/core/managers/EventManager.py` & `opengamedata_core-0.0.6/src/ogd/core/managers/EventManager.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from datetime import datetime
 from typing import Any, Callable, List, Type, Optional, Set
 ## import local files
 from ogd.core.generators.registries.DetectorRegistry import DetectorRegistry
 from ogd.core.generators.GeneratorLoader import GeneratorLoader
 from ogd.core.processors.DetectorProcessor import DetectorProcessor
 from ogd.core.processors.EventProcessor import EventProcessor
-from ogd.core.schemas.Event import Event, EventSource
+from ogd.core.models.Event import Event, EventSource
 from ogd.core.schemas.games.GameSchema import GameSchema
 from ogd.core.utils import utils
 from ogd.core.utils.Logger import Logger
 from ogd.core.utils.utils import ExportRow
 
 ## @class EventProcessor
 #  Class to manage data for a csv events file.
```

### Comparing `opengamedata_core-0.0.5/src/ogd/core/managers/ExportManager.py` & `opengamedata_core-0.0.6/src/ogd/core/managers/ExportManager.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,17 +12,17 @@
 from typing import Any, Dict, List, Tuple, Type, Optional
 
 ## import local files
 from ogd import games
 from ogd.core.generators.GeneratorLoader import GeneratorLoader
 from ogd.core.managers.EventManager import EventManager
 from ogd.core.managers.FeatureManager import FeatureManager
-from ogd.core.schemas.Event import Event
-from ogd.core.schemas.ExportMode import ExportMode
-from ogd.core.schemas.IDMode import IDMode
+from ogd.core.models.Event import Event
+from ogd.core.models.enums.ExportMode import ExportMode
+from ogd.core.models.enums.IDMode import IDMode
 from ogd.core.schemas.games.GameSchema import GameSchema
 from ogd.core.schemas.configs.ConfigSchema import ConfigSchema
 from ogd.core.requests.Request import Request
 from ogd.core.requests.RequestResult import RequestResult
 from ogd.core.utils.Logger import Logger
 
 ## @class ExportManager
```

### Comparing `opengamedata_core-0.0.5/src/ogd/core/managers/FeatureManager.py` & `opengamedata_core-0.0.6/src/ogd/core/managers/FeatureManager.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 ## import local files
 from ogd.core.generators.GeneratorLoader import GeneratorLoader
 from ogd.core.processors.ExtractorProcessor import ExtractorProcessor
 from ogd.core.processors.PopulationProcessor import PopulationProcessor
 from ogd.core.processors.PlayerProcessor import PlayerProcessor
 from ogd.core.processors.SessionProcessor import SessionProcessor
 from ogd.core.schemas.games.GameSchema import GameSchema
-from ogd.core.schemas.Event import Event
+from ogd.core.models.Event import Event
 from ogd.core.utils.Logger import Logger
 from ogd.core.utils.utils import ExportRow
 
 class FeatureManager:
     def __init__(self, game_schema:GameSchema, LoaderClass:Optional[Type[GeneratorLoader]], feature_overrides:Optional[List[str]]):
         self._LoaderClass    : Optional[Type[GeneratorLoader]] = LoaderClass
         self._game_schema    : GameSchema                 = game_schema
```

### Comparing `opengamedata_core-0.0.5/src/ogd/core/processors/ClassroomDetector.py` & `opengamedata_core-0.0.6/src/ogd/core/processors/ClassroomDetector.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.5/src/ogd/core/processors/DetectorProcessor.py` & `opengamedata_core-0.0.6/src/ogd/core/processors/DetectorProcessor.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # import libraries
 from typing import Any, Callable, Dict, List, Type, Optional
 # import locals
 from ogd.core.generators.registries.DetectorRegistry import DetectorRegistry
-from ogd.core.schemas.FeatureData import FeatureData
+from ogd.core.models.FeatureData import FeatureData
 from ogd.core.generators.GeneratorLoader import GeneratorLoader
 from ogd.core.processors.GeneratorProcessor import GeneratorProcessor
-from ogd.core.schemas.Event import Event
-from ogd.core.schemas.ExtractionMode import ExtractionMode
+from ogd.core.models.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
 from ogd.core.schemas.games.GameSchema import GameSchema
 from ogd.core.utils.utils import ExportRow
 
 class DetectorProcessor(GeneratorProcessor):
 
     # *** BUILT-INS & PROPERTIES ***
```

### Comparing `opengamedata_core-0.0.5/src/ogd/core/processors/EventProcessor.py` & `opengamedata_core-0.0.6/src/ogd/core/processors/EventProcessor.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # import libraries
 import json
 from datetime import datetime
 from typing import List, Type, Optional
 # import locals
 from ogd.core.processors.Processor import Processor
-from ogd.core.schemas.Event import Event
+from ogd.core.models.Event import Event
 from ogd.core.schemas.games.GameSchema import GameSchema
 from ogd.core.utils.utils import ExportRow
 
 class EventProcessor(Processor):
 
     # *** BUILT-INS & PROPERTIES ***
```

### Comparing `opengamedata_core-0.0.5/src/ogd/core/processors/ExtractorProcessor.py` & `opengamedata_core-0.0.6/src/ogd/core/processors/ExtractorProcessor.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 ## import standard libraries
 import abc
 from typing import Dict, List, Type, Optional, Set
 
 # import locals
-from ogd.core.schemas.FeatureData import FeatureData
+from ogd.core.models.FeatureData import FeatureData
 from ogd.core.generators.GeneratorLoader import GeneratorLoader
 from ogd.core.generators.registries.ExtractorRegistry import ExtractorRegistry
 from ogd.core.processors.GeneratorProcessor import GeneratorProcessor
 from ogd.core.schemas.games.GameSchema import GameSchema
-from ogd.core.schemas.ExportMode import ExportMode
+from ogd.core.models.enums.ExportMode import ExportMode
 from ogd.core.utils.utils import ExportRow
 
 ## @class Processor
 class ExtractorProcessor(GeneratorProcessor):
 
     # *** ABSTRACTS ***
```

### Comparing `opengamedata_core-0.0.5/src/ogd/core/processors/GeneratorProcessor.py` & `opengamedata_core-0.0.6/src/ogd/core/processors/GeneratorProcessor.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 ## import standard libraries
 import abc
 import logging
 from typing import Dict, List, Type, Optional, Set
 # import locals
 from ogd.core.generators.registries.GeneratorRegistry import GeneratorRegistry
 from ogd.core.generators.GeneratorLoader import GeneratorLoader
-from ogd.core.schemas.FeatureData import FeatureData
+from ogd.core.models.FeatureData import FeatureData
 from ogd.core.generators.GeneratorLoader import GeneratorLoader
 from ogd.core.processors.Processor import Processor
-from ogd.core.schemas.ExtractionMode import ExtractionMode
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
 from ogd.core.schemas.games.GameSchema import GameSchema
-from ogd.core.schemas.ExportMode import ExportMode
+from ogd.core.models.enums.ExportMode import ExportMode
 from ogd.core.utils.Logger import Logger
 from ogd.core.utils.utils import ExportRow
 
 ## @class Processor
 class GeneratorProcessor(Processor):
 
     # *** ABSTRACTS ***
```

### Comparing `opengamedata_core-0.0.5/src/ogd/core/processors/PlayerProcessor.py` & `opengamedata_core-0.0.6/src/ogd/core/processors/PlayerProcessor.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 import traceback
 from typing import List, Dict, Type, Optional, Set
 # import local files
 from ogd.core.generators.GeneratorLoader import GeneratorLoader
 from ogd.core.generators.registries.ExtractorRegistry import ExtractorRegistry
 from ogd.core.processors.ExtractorProcessor import ExtractorProcessor
 from ogd.core.processors.SessionProcessor import SessionProcessor
-from ogd.core.schemas.Event import Event
-from ogd.core.schemas.ExportMode import ExportMode
-from ogd.core.schemas.ExtractionMode import ExtractionMode
-from ogd.core.schemas.FeatureData import FeatureData
+from ogd.core.models.Event import Event
+from ogd.core.models.enums.ExportMode import ExportMode
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
+from ogd.core.models.FeatureData import FeatureData
 from ogd.core.schemas.games.GameSchema import GameSchema
 from ogd.core.utils.Logger import Logger
 from ogd.core.utils.utils import ExportRow
 
 ## @class PlayerProcessor
 #  Class to extract and manage features for a processed csv file.
 class PlayerProcessor(ExtractorProcessor):
```

### Comparing `opengamedata_core-0.0.5/src/ogd/core/processors/PopulationProcessor.py` & `opengamedata_core-0.0.6/src/ogd/core/processors/PopulationProcessor.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # import standard libraries
 import logging
 from typing import List, Type, Optional, Set
 # import local files
-from ogd.core.schemas.FeatureData import FeatureData
+from ogd.core.models.FeatureData import FeatureData
 from ogd.core.generators.GeneratorLoader import GeneratorLoader
 from ogd.core.generators.registries.ExtractorRegistry import ExtractorRegistry
 from ogd.core.processors.ExtractorProcessor import ExtractorProcessor
-from ogd.core.schemas.Event import Event
-from ogd.core.schemas.ExtractionMode import ExtractionMode
+from ogd.core.models.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
 from ogd.core.schemas.games.GameSchema import GameSchema
 from ogd.core.utils.Logger import Logger
 from ogd.core.utils.utils import ExportRow
 
 ## @class PopulationProcessor
 #  Class to extract and manage features for a processed csv file.
 class PopulationProcessor(ExtractorProcessor):
```

### Comparing `opengamedata_core-0.0.5/src/ogd/core/processors/Processor.py` & `opengamedata_core-0.0.6/src/ogd/core/processors/Processor.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 ## import standard libraries
 import abc
 import json
 import logging
 from datetime import datetime
 from typing import Any, Dict, List, Type, Optional
 # import locals
-from ogd.core.schemas.FeatureData import FeatureData
+from ogd.core.models.FeatureData import FeatureData
 from ogd.core.schemas.games.GameSchema import GameSchema
-from ogd.core.schemas.Event import Event
+from ogd.core.models.Event import Event
 from ogd.core.utils.utils import ExportRow, Logger
 
 ## @class Processor
 class Processor(abc.ABC):
 
     # *** ABSTRACTS ***
```

### Comparing `opengamedata_core-0.0.5/src/ogd/core/processors/SessionProcessor.py` & `opengamedata_core-0.0.6/src/ogd/core/processors/SessionProcessor.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 # import standard libraries
 import logging
 import traceback
 from typing import List, Dict, Type, Optional, Set
 # import local files
-from ogd.core.schemas.FeatureData import FeatureData
+from ogd.core.models.FeatureData import FeatureData
 from ogd.core.generators.GeneratorLoader import GeneratorLoader
 from ogd.core.generators.registries.ExtractorRegistry import ExtractorRegistry
 from ogd.core.processors.ExtractorProcessor import ExtractorProcessor
-from ogd.core.schemas.Event import Event
-from ogd.core.schemas.ExportMode import ExportMode
-from ogd.core.schemas.ExtractionMode import ExtractionMode
+from ogd.core.models.Event import Event
+from ogd.core.models.enums.ExportMode import ExportMode
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
 from ogd.core.schemas.games.GameSchema import GameSchema
 from ogd.core.utils.Logger import Logger
 from ogd.core.utils.utils import ExportRow
 
 ## @class SessionProcessor
 #  Class to extract and manage features for a processed csv file.
 class SessionProcessor(ExtractorProcessor):
```

### Comparing `opengamedata_core-0.0.5/src/ogd/core/requests/Request.py` & `opengamedata_core-0.0.6/src/ogd/core/requests/Request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # import standard libraries
 import abc
 from datetime import datetime
 from typing import Dict, List, Optional, Set
 # import local files
 from ogd.core.interfaces.DataInterface import DataInterface
 from ogd.core.interfaces.outerfaces.DataOuterface import DataOuterface
-from ogd.core.schemas.IDMode import IDMode
-from ogd.core.schemas.ExportMode import ExportMode
+from ogd.core.models.enums.IDMode import IDMode
+from ogd.core.models.enums.ExportMode import ExportMode
 from ogd.core.utils.Logger import Logger
 
 class ExporterRange:
     """
     Simple class to define a range of data for export.
     """
     def __init__(self, date_min:Optional[datetime], date_max:Optional[datetime], ids:Optional[List[str]], id_mode:IDMode=IDMode.SESSION, versions:Optional[List[int]]=None):
```

### Comparing `opengamedata_core-0.0.5/src/ogd/core/requests/RequestResult.py` & `opengamedata_core-0.0.6/src/ogd/core/requests/RequestResult.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.5/src/ogd/core/schemas/Event.py` & `opengamedata_core-0.0.6/src/ogd/core/models/Event.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.5/src/ogd/core/schemas/FeatureData.py` & `opengamedata_core-0.0.6/src/ogd/core/models/FeatureData.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Any, List, Optional
 
-from ogd.core.schemas.ExtractionMode import ExtractionMode
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
 
 class FeatureData:
    def __init__(self, name:str, feature_type:str, count_index:Optional[int],
                 cols:List[str], vals:List[Any],   mode:ExtractionMode,
                 player_id:Optional[str]=None,     sess_id:Optional[str]=None):
       self._name = name
       self._feature_type = feature_type
```

### Comparing `opengamedata_core-0.0.5/src/ogd/core/schemas/Schema.py` & `opengamedata_core-0.0.6/src/ogd/core/schemas/Schema.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.5/src/ogd/core/schemas/configs/ConfigSchema.py` & `opengamedata_core-0.0.6/src/ogd/core/schemas/configs/ConfigSchema.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.5/src/ogd/core/schemas/configs/GameSourceSchema.py` & `opengamedata_core-0.0.6/src/ogd/core/schemas/configs/GameSourceSchema.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.5/src/ogd/core/schemas/configs/IndexingSchema.py` & `opengamedata_core-0.0.6/src/ogd/core/schemas/configs/IndexingSchema.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.5/src/ogd/core/schemas/configs/LegacyConfigSchema.py` & `opengamedata_core-0.0.6/src/ogd/core/schemas/configs/LegacyConfigSchema.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.5/src/ogd/core/schemas/configs/data_sources/BigQuerySourceSchema.py` & `opengamedata_core-0.0.6/src/ogd/core/schemas/configs/data_sources/BigQuerySourceSchema.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.5/src/ogd/core/schemas/configs/data_sources/DataSourceSchema.py` & `opengamedata_core-0.0.6/src/ogd/core/schemas/configs/data_sources/DataSourceSchema.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.5/src/ogd/core/schemas/configs/data_sources/FileSourceSchema.py` & `opengamedata_core-0.0.6/src/ogd/core/schemas/configs/data_sources/FileSourceSchema.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.5/src/ogd/core/schemas/configs/data_sources/MySQLSourceSchema.py` & `opengamedata_core-0.0.6/src/ogd/core/schemas/configs/data_sources/MySQLSourceSchema.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.5/src/ogd/core/schemas/games/AggregateSchema.py` & `opengamedata_core-0.0.6/src/ogd/core/schemas/games/AggregateSchema.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.5/src/ogd/core/schemas/games/DataElementSchema.py` & `opengamedata_core-0.0.6/src/ogd/core/schemas/games/DataElementSchema.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.5/src/ogd/core/schemas/games/DetectorMapSchema.py` & `opengamedata_core-0.0.6/src/ogd/core/schemas/games/DetectorMapSchema.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.5/src/ogd/core/schemas/games/DetectorSchema.py` & `opengamedata_core-0.0.6/src/ogd/core/schemas/games/DetectorSchema.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # import standard libraries
 from typing import Any, Dict
 # import local files
-from ogd.core.schemas.ExtractionMode import ExtractionMode
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
 from ogd.core.schemas.games.ExtractorSchema import ExtractorSchema
 
 class DetectorSchema(ExtractorSchema):
     def __init__(self, name:str, all_elements:Dict[str, Any]):
         super().__init__(name=name, all_elements=all_elements)
 
     @property
```

### Comparing `opengamedata_core-0.0.5/src/ogd/core/schemas/games/EventSchema.py` & `opengamedata_core-0.0.6/src/ogd/core/schemas/games/EventSchema.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.5/src/ogd/core/schemas/games/ExtractorSchema.py` & `opengamedata_core-0.0.6/src/ogd/core/schemas/games/ExtractorSchema.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # import standard libraries
 import abc
 import logging
 from typing import Any, Dict, List, Set
 # import local files
-from ogd.core.schemas.ExtractionMode import ExtractionMode
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
 from ogd.core.schemas.Schema import Schema
 from ogd.core.utils.Logger import Logger
 
 class ExtractorSchema(Schema):
     def __init__(self, name:str, all_elements:Dict[str, Any]):
         self._enabled     : Set[ExtractionMode]
         self._type_name   : str
```

### Comparing `opengamedata_core-0.0.5/src/ogd/core/schemas/games/FeatureMapSchema.py` & `opengamedata_core-0.0.6/src/ogd/core/schemas/games/FeatureMapSchema.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.5/src/ogd/core/schemas/games/FeatureSchema.py` & `opengamedata_core-0.0.6/src/ogd/core/schemas/games/FeatureSchema.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.5/src/ogd/core/schemas/games/GameSchema.py` & `opengamedata_core-0.0.6/src/ogd/core/schemas/games/GameSchema.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,16 +10,16 @@
 from ogd.core.schemas.games.DetectorSchema import DetectorSchema
 from ogd.core.schemas.games.DetectorMapSchema import DetectorMapSchema
 from ogd.core.schemas.games.DataElementSchema import DataElementSchema
 from ogd.core.schemas.games.EventSchema import EventSchema
 from ogd.core.schemas.games.PerCountSchema import PerCountSchema
 from ogd.core.schemas.games.FeatureSchema import FeatureSchema
 from ogd.core.schemas.games.FeatureMapSchema import FeatureMapSchema
-from ogd.core.schemas.IterationMode import IterationMode
-from ogd.core.schemas.ExtractionMode import ExtractionMode
+from ogd.core.models.enums.IterationMode import IterationMode
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
 from ogd.core.utils import utils
 from ogd.core.utils.utils import loadJSONFile
 from ogd.core.utils.Logger import Logger
 
 ## @class GameSchema
 #  A fairly simple class that reads a JSON schema with information on how a given
 #  game's data is structured in the database, and the features we want to extract
```

### Comparing `opengamedata_core-0.0.5/src/ogd/core/schemas/games/GameStateSchema.py` & `opengamedata_core-0.0.6/src/ogd/core/schemas/games/GameStateSchema.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.5/src/ogd/core/schemas/games/PerCountSchema.py` & `opengamedata_core-0.0.6/src/ogd/core/schemas/games/PerCountSchema.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.5/src/ogd/core/schemas/table_schemas/BIGQUERY.json` & `opengamedata_core-0.0.6/src/ogd/core/schemas/table_schemas/BIGQUERY.json`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.5/src/ogd/core/schemas/table_schemas/FIELDDAY_MYSQL.json` & `opengamedata_core-0.0.6/src/ogd/core/schemas/table_schemas/FIELDDAY_MYSQL.json`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.5/src/ogd/core/schemas/table_schemas/FIREBASE.json` & `opengamedata_core-0.0.6/src/ogd/core/schemas/table_schemas/FIREBASE.json`

 * *Files 18% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9660714285714286%*

 * *Differences: {"'column_map'": "{'user_data': None}", "'columns'": '{delete: [3]}'}*

```diff
@@ -8,15 +8,15 @@
         "event_sequence_index": null,
         "event_source": null,
         "game_state": null,
         "log_version": "log_version",
         "session_id": "session_id",
         "time_offset": null,
         "timestamp": "timestamp",
-        "user_data": "geo",
+        "user_data": null,
         "user_id": "fd_user_id"
     },
     "columns": [
         {
             "description": "The name of the event",
             "name": "event_name",
             "readable": "Event Name",
@@ -31,20 +31,14 @@
         {
             "description": "A record of device information",
             "name": "device",
             "readable": "Device",
             "type": "json"
         },
         {
-            "description": "A record of the user's geographic information",
-            "name": "geo",
-            "readable": "Geo",
-            "type": "json"
-        },
-        {
             "description": "The platform on which the app was built",
             "name": "platform",
             "readable": "Platform",
             "type": "str"
         },
         {
             "description": "Datetime when event was logged",
```

### Comparing `opengamedata_core-0.0.5/src/ogd/core/schemas/table_schemas/MASHOPOLIS_MYSQL.json` & `opengamedata_core-0.0.6/src/ogd/core/schemas/table_schemas/MASHOPOLIS_MYSQL.json`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.5/src/ogd/core/schemas/table_schemas/OGD_EVENT_FILE.json` & `opengamedata_core-0.0.6/src/ogd/core/schemas/table_schemas/OGD_EVENT_FILE.json`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.5/src/ogd/core/schemas/table_schemas/OPENGAMEDATA_BIGQUERY.json` & `opengamedata_core-0.0.6/src/ogd/core/schemas/table_schemas/OPENGAMEDATA_BIGQUERY.json`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.5/src/ogd/core/schemas/table_schemas/OPENGAMEDATA_MYSQL.json` & `opengamedata_core-0.0.6/src/ogd/core/schemas/table_schemas/OPENGAMEDATA_MYSQL.json`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.5/src/ogd/core/schemas/table_schemas/SHIPWRECKS.json` & `opengamedata_core-0.0.6/src/ogd/core/schemas/table_schemas/SHIPWRECKS.json`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.5/src/ogd/core/schemas/tables/ColumnMapSchema.py` & `opengamedata_core-0.0.6/src/ogd/core/schemas/tables/ColumnMapSchema.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.5/src/ogd/core/schemas/tables/ColumnSchema.py` & `opengamedata_core-0.0.6/src/ogd/core/schemas/tables/ColumnSchema.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # import standard libraries
 import logging
 from typing import Any, Dict, List, Set
 # import local files
-from ogd.core.schemas.ExtractionMode import ExtractionMode
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
 from ogd.core.schemas.Schema import Schema
 from ogd.core.utils.Logger import Logger
 
 class ColumnSchema(Schema):
     def __init__(self, all_elements:Dict[str, Any]):
         self._readable    : str
         self._value_type  : str
```

### Comparing `opengamedata_core-0.0.5/src/ogd/core/schemas/tables/TableSchema.py` & `opengamedata_core-0.0.6/src/ogd/core/schemas/tables/TableSchema.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from dateutil import parser
 from datetime import datetime, time, timedelta
 from json.decoder import JSONDecodeError
 from pathlib import Path
 from typing import Any, Dict, Final, List, Tuple, Optional, Union
 ## import local files
 from ogd.core import schemas
-from ogd.core.schemas.Event import Event, EventSource
+from ogd.core.models.Event import Event, EventSource
 from ogd.core.schemas.tables.ColumnMapSchema import ColumnMapSchema
 from ogd.core.schemas.tables.ColumnSchema import ColumnSchema
 from ogd.core.utils import utils
 from ogd.core.utils.Logger import Logger
 from ogd.core.utils.typing import Map
 
 ## @class TableSchema
```

### Comparing `opengamedata_core-0.0.5/src/ogd/core/utils/Logger.py` & `opengamedata_core-0.0.6/src/ogd/core/utils/Logger.py`

 * *Files 0% similar despite different names*

```diff
@@ -62,25 +62,25 @@
         if Logger.file_logger is not None:
             match level:
                 case logging.DEBUG:
                     Logger.file_logger.debug(f"DEBUG:   {now} {indent}{_idt_msg}")
                 case logging.INFO:
                     Logger.file_logger.info( f"INFO:    {now} {indent}{_idt_msg}")
                 case logging.WARNING:
-                    Logger.file_logger.warn( f"WARNING: {now} {indent}{_idt_msg}")
+                    Logger.file_logger.warning( f"WARNING: {now} {indent}{_idt_msg}")
                 case logging.ERROR:
                     Logger.file_logger.error(f"ERROR:   {now} {indent}{_idt_msg}")
         if Logger.std_logger is not None:
             match level:
                 case logging.DEBUG:
                     Logger.std_logger.debug(f"DEBUG:   {indent}{_idt_msg}")
                 case logging.INFO:
                     Logger.std_logger.info( f"INFO:    {indent}{_idt_msg}")
                 case logging.WARNING:
-                    Logger.std_logger.warn( f"WARNING: {indent}{_idt_msg}")
+                    Logger.std_logger.warning( f"WARNING: {indent}{_idt_msg}")
                 case logging.ERROR:
                     Logger.std_logger.error(f"ERROR:   {indent}{_idt_msg}")
 
     @staticmethod
     def Print(message:str, level=logging.DEBUG) -> None:
         match level:
             case logging.DEBUG:
```

### Comparing `opengamedata_core-0.0.5/src/ogd/core/utils/Readme.py` & `opengamedata_core-0.0.6/src/ogd/core/utils/Readme.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.5/src/ogd/core/utils/utils.py` & `opengamedata_core-0.0.6/src/ogd/core/utils/utils.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.5/src/ogd/games/ALL_YOU_CAN_ET/schemas/ALL_YOU_CAN_ET.json.template` & `opengamedata_core-0.0.6/src/ogd/games/ALL_YOU_CAN_ET/schemas/ALL_YOU_CAN_ET.json.template`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.5/src/ogd/games/AQUALAB/AqualabLoader.py` & `opengamedata_core-0.0.6/src/ogd/games/AQUALAB/AqualabLoader.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,16 +8,16 @@
 from ogd.games import AQUALAB
 from ogd.core.generators.detectors.Detector import Detector
 from ogd.core.generators.Generator import GeneratorParameters
 from ogd.core.generators.GeneratorLoader import GeneratorLoader
 from ogd.core.generators.extractors.Feature import Feature
 from ogd.games.AQUALAB.detectors import *
 from ogd.games.AQUALAB.features import *
-from ogd.core.schemas.Event import Event
-from ogd.core.schemas.ExtractionMode import ExtractionMode
+from ogd.core.models.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
 from ogd.core.schemas.games.GameSchema import GameSchema
 from ogd.core.utils.utils import loadJSONFile
 
 EXPORT_PATH : Final[str] = "games/AQUALAB/DBExport.json"
 
 ## @class AqualabLoader
 #  Extractor subclass for extracting features from Aqualab game data.
```

### Comparing `opengamedata_core-0.0.5/src/ogd/games/AQUALAB/DBExport.json` & `opengamedata_core-0.0.6/src/ogd/games/AQUALAB/DBExport.json`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.5/src/ogd/games/AQUALAB/detectors/CollectFactNoJob.py` & `opengamedata_core-0.0.6/src/ogd/games/AQUALAB/detectors/CollectFactNoJob.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 from datetime import datetime
 from typing import Callable, List
 
 # import local files
 from ogd.core.generators.detectors.Detector import Detector
 from ogd.core.generators.detectors.DetectorEvent import DetectorEvent
 from ogd.core.generators.Generator import GeneratorParameters
-from ogd.core.schemas.Event import Event
-from ogd.core.schemas.ExtractionMode import ExtractionMode
+from ogd.core.models.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
 
 class CollectFactNoJob(Detector):
     """Template file to serve as a guide for creating custom Feature subclasses for games.
 
     :param Feature: Base class for a Custom Feature class.
     :type Feature: _type_
     """
```

### Comparing `opengamedata_core-0.0.5/src/ogd/games/AQUALAB/detectors/DiveSiteNoEvidence.py` & `opengamedata_core-0.0.6/src/ogd/games/AQUALAB/detectors/DiveSiteNoEvidence.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # import standard libraries
 from datetime import datetime, timedelta
 from typing import Any, Callable, List, Optional
 # import local files
 from ogd.core.generators.detectors.Detector import Detector
 from ogd.core.generators.detectors.DetectorEvent import DetectorEvent
 from ogd.core.generators.Generator import GeneratorParameters
-from ogd.core.schemas.Event import Event
-from ogd.core.schemas.ExtractionMode import ExtractionMode
+from ogd.core.models.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
 
 class DiveSiteNoEvidence(Detector):
     """Template file to serve as a guide for creating custom Feature subclasses for games.
 
     :param Feature: Base class for a Custom Feature class.
     :type Feature: _type_
     """
```

### Comparing `opengamedata_core-0.0.5/src/ogd/games/AQUALAB/detectors/EchoRoomChange.py` & `opengamedata_core-0.0.6/src/ogd/games/AQUALAB/detectors/EchoRoomChange.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # import standard libraries
 from datetime import datetime
 from typing import Callable, List
 # import local files
 from ogd.core.generators.detectors.Detector import Detector
 from ogd.core.generators.detectors.DetectorEvent import DetectorEvent
 from ogd.core.generators.Generator import GeneratorParameters
-from ogd.core.schemas.Event import Event
-from ogd.core.schemas.ExtractionMode import ExtractionMode
+from ogd.core.models.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
 
 class EchoRoomChange(Detector):
     """Template file to serve as a guide for creating custom Feature subclasses for games.
 
     :param Feature: Base class for a Custom Feature class.
     :type Feature: _type_
     """
```

### Comparing `opengamedata_core-0.0.5/src/ogd/games/AQUALAB/detectors/HintAndLeave.py` & `opengamedata_core-0.0.6/src/ogd/games/AQUALAB/detectors/HintAndLeave.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # import standard libraries
 from datetime import datetime, timedelta
 from typing import Callable, Final, List, Optional, Union
 # import local files
 from ogd.core.generators.detectors.Detector import Detector
 from ogd.core.generators.detectors.DetectorEvent import DetectorEvent
 from ogd.core.generators.Generator import GeneratorParameters
-from ogd.core.schemas.Event import Event
-from ogd.core.schemas.ExtractionMode import ExtractionMode
+from ogd.core.models.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
 from ogd.core.utils.typing import Map
 
 
 class HintAndLeave(Detector):
     """Template file to serve as a guide for creating custom Feature subclasses for games.
 
     :param Feature: Base class for a Custom Feature class.
```

### Comparing `opengamedata_core-0.0.5/src/ogd/games/AQUALAB/detectors/Idle.py` & `opengamedata_core-0.0.6/src/ogd/games/AQUALAB/detectors/Idle.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 from datetime import datetime, timedelta
 from time import time
 from typing import Callable, Final, List, Optional, Union
 # import local files
 from ogd.core.generators.detectors.Detector import Detector
 from ogd.core.generators.detectors.DetectorEvent import DetectorEvent
 from ogd.core.generators.Generator import GeneratorParameters
-from ogd.core.schemas.Event import Event
-from ogd.core.schemas.ExtractionMode import ExtractionMode
+from ogd.core.models.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
 
 class Idle(Detector):
     """Template file to serve as a guide for creating custom Feature subclasses for games.
 
     :param Feature: Base class for a Custom Feature class.
     :type Feature: _type_
     """
```

### Comparing `opengamedata_core-0.0.5/src/ogd/games/AQUALAB/detectors/SceneChangeFrequently.py` & `opengamedata_core-0.0.6/src/ogd/games/AQUALAB/detectors/SceneChangeFrequently.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 from datetime import datetime, timedelta
 from time import time
 from typing import Callable, Final, List, Optional, Union
 # import local files
 from ogd.core.generators.detectors.Detector import Detector
 from ogd.core.generators.detectors.DetectorEvent import DetectorEvent
 from ogd.core.generators.Generator import GeneratorParameters
-from ogd.core.schemas.Event import Event
-from ogd.core.schemas.ExtractionMode import ExtractionMode
+from ogd.core.models.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
 
 
 class SceneChangeFrequently(Detector):
     """Template file to serve as a guide for creating custom Feature subclasses for games.
 
     :param Feature: Base class for a Custom Feature class.
     :type Feature: _type_
```

### Comparing `opengamedata_core-0.0.5/src/ogd/games/AQUALAB/detectors/TwoHints.py` & `opengamedata_core-0.0.6/src/ogd/games/AQUALAB/detectors/TwoHints.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 from datetime import datetime, timedelta
 from time import time
 from typing import Callable, Final, List, Optional, Union
 # import local files
 from ogd.core.generators.detectors.Detector import Detector
 from ogd.core.generators.detectors.DetectorEvent import DetectorEvent
 from ogd.core.generators.Generator import GeneratorParameters
-from ogd.core.schemas.Event import Event
-from ogd.core.schemas.ExtractionMode import ExtractionMode
+from ogd.core.models.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
 from ogd.core.utils.typing import Map
 
 
 class TwoHints(Detector):
     """Template file to serve as a guide for creating custom Feature subclasses for games.
 
     :param Feature: Base class for a Custom Feature class.
```

### Comparing `opengamedata_core-0.0.5/src/ogd/games/AQUALAB/features/ActiveJobs.py` & `opengamedata_core-0.0.6/src/ogd/games/AQUALAB/features/ActiveJobs.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 import logging
 from collections import defaultdict
 from typing import Any, List, Optional
 # import locals
 from ogd.core.utils.Logger import Logger
 from ogd.core.generators.Generator import GeneratorParameters
 from ogd.core.generators.extractors.Feature import Feature
-from ogd.core.schemas.Event import Event
-from ogd.core.schemas.ExtractionMode import ExtractionMode
-from ogd.core.schemas.FeatureData import FeatureData
+from ogd.core.models.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
+from ogd.core.models.FeatureData import FeatureData
 
 class ActiveJobs(Feature):
 
     def __init__(self, params:GeneratorParameters, job_map:dict):
         self._job_map = job_map
         super().__init__(params=params)
         self._current_user_code = None
```

### Comparing `opengamedata_core-0.0.5/src/ogd/games/AQUALAB/features/ActiveTime.py` & `opengamedata_core-0.0.6/src/ogd/games/AQUALAB/features/ActiveTime.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 from datetime import datetime, timedelta
 import logging, warnings
 from typing import Any, Final, List, Optional
 # import locals
 from ogd.core.utils.Logger import Logger
 from ogd.core.generators.Generator import GeneratorParameters
 from ogd.core.generators.extractors.Feature import Feature
-from ogd.core.schemas.Event import Event
-from ogd.core.schemas.ExtractionMode import ExtractionMode
-from ogd.core.schemas.FeatureData import FeatureData
+from ogd.core.models.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
+from ogd.core.models.FeatureData import FeatureData
 
 class ActiveTime(Feature):
     IDLE_LEVEL : Final[int] = 30
 
     def __init__(self, params:GeneratorParameters, job_map:dict, active_threads:Optional[float] = None):
         self._job_map = job_map
         super().__init__(params=params)
```

### Comparing `opengamedata_core-0.0.5/src/ogd/games/AQUALAB/features/AppVersions.py` & `opengamedata_core-0.0.6/src/ogd/games/AQUALAB/features/SessionJobsCompleted.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 from typing import Any, List
 
 from ogd.core.generators.Generator import GeneratorParameters
-from ogd.core.generators.extractors.SessionFeature import SessionFeature
-from ogd.core.schemas.Event import Event
-from ogd.core.schemas.ExtractionMode import ExtractionMode
-from ogd.core.schemas.FeatureData import FeatureData
+from ogd.core.generators.extractors.Feature import Feature
+from ogd.core.models.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
+from ogd.core.models.FeatureData import FeatureData
 
-class AppVersions(SessionFeature):
+class SessionJobsCompleted(Feature):
     """_summary_
 
-    :param SessionFeature: _description_
-    :type SessionFeature: _type_
+    :param Feature: _description_
+    :type Feature: _type_
     """
     def __init__(self, params:GeneratorParameters):
         super().__init__(params=params)
-        self._versions = set()
+        self._count = 0
 
     # *** IMPLEMENT ABSTRACT FUNCTIONS ***
     @classmethod
     def _eventFilter(cls, mode:ExtractionMode) -> List[str]:
-        return ["all_events"]
+        return ["complete_job"]
 
     @classmethod
     def _featureFilter(cls, mode:ExtractionMode) -> List[str]:
         return []
 
     def _updateFromEvent(self, event:Event) -> None:
-        self._versions.add(event.AppVersion)
+        self._count += 1
 
     def _updateFromFeatureData(self, feature:FeatureData):
         return
 
     def _getFeatureValues(self) -> List[Any]:
-        return [list(self._versions)]
+        return [self._count]
 
-    # *** Optionally override public functions. ***
+    # *** Optionally override public functions. ***
```

### Comparing `opengamedata_core-0.0.5/src/ogd/games/AQUALAB/features/AverageSessionTime.py` & `opengamedata_core-0.0.6/src/ogd/games/AQUALAB/features/AverageSessionTime.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 from datetime import datetime, timedelta
 import logging, warnings
 from typing import Any, List, Optional
 # import locals
 from ogd.core.utils.Logger import Logger
 from ogd.core.generators.extractors.Extractor import GeneratorParameters
 from ogd.core.generators.extractors.Feature import Feature
-from ogd.core.schemas.Event import Event
-from ogd.core.schemas.ExtractionMode import ExtractionMode
-from ogd.core.schemas.FeatureData import FeatureData
+from ogd.core.models.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
+from ogd.core.models.FeatureData import FeatureData
 
 class AverageSessionTime(Feature):
     def __init__(self, params:GeneratorParameters):
         super().__init__(params=params)
         self._play_time: timedelta = timedelta(0)
         self._session_count = 0
```

### Comparing `opengamedata_core-0.0.5/src/ogd/games/AQUALAB/features/EchoSessionID.py` & `opengamedata_core-0.0.6/src/ogd/games/SHADOWSPECT/features/SessionID.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 # import libraries
 from typing import Any, List
 # import locals
 from ogd.core.generators.Generator import GeneratorParameters
 from ogd.core.generators.extractors.SessionFeature import SessionFeature
-from ogd.core.schemas.Event import Event
-from ogd.core.schemas.ExtractionMode import ExtractionMode
-from ogd.core.schemas.FeatureData import FeatureData
+from ogd.core.models.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
+from ogd.core.models.FeatureData import FeatureData
 
-class EchoSessionID(SessionFeature):
 
-    def __init__(self, params:GeneratorParameters):
+class SessionID(SessionFeature):
+    def __init__(self, params:GeneratorParameters, session_id:str):
+        self._session_id = session_id
         super().__init__(params=params)
-        self._session_id = None
 
     # *** IMPLEMENT ABSTRACT FUNCTIONS ***
     @classmethod
     def _eventFilter(cls, mode:ExtractionMode) -> List[str]:
         return []
 
     @classmethod
     def _featureFilter(cls, mode:ExtractionMode) -> List[str]:
-        return ["SessionID"]
+        return []
 
     def _updateFromEvent(self, event:Event) -> None:
         return
 
     def _updateFromFeatureData(self, feature:FeatureData):
-        self._session_id = feature.FeatureValues[0]
+        return
 
     def _getFeatureValues(self) -> List[Any]:
-        return [f"The sess ID is: {self._session_id}"]
+        return [self._session_id]
 
     # *** Optionally override public functions. ***
```

### Comparing `opengamedata_core-0.0.5/src/ogd/games/AQUALAB/features/EventList.py` & `opengamedata_core-0.0.6/src/ogd/games/AQUALAB/features/EventList.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # import libraries
 import json
 from typing import Any, List, Optional
 
 # import locals
 from ogd.core.generators.extractors.Feature import Feature
 from ogd.core.generators.Generator import GeneratorParameters
-from ogd.core.schemas.Event import Event
-from ogd.core.schemas.ExtractionMode import ExtractionMode
-from ogd.core.schemas.FeatureData import FeatureData
+from ogd.core.models.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
+from ogd.core.models.FeatureData import FeatureData
 
 class EventList(Feature):
 
     def __init__(self, params:GeneratorParameters):
         super().__init__(params=params)
         self._event_list = []
```

### Comparing `opengamedata_core-0.0.5/src/ogd/games/AQUALAB/features/JobActiveTime.py` & `opengamedata_core-0.0.6/src/ogd/games/AQUALAB/features/JobActiveTime.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 import logging
 from datetime import timedelta
 from typing import Any, List, Optional
 # import locals
 from ogd.core.utils.Logger import Logger
 from ogd.core.generators.Generator import GeneratorParameters
 from ogd.games.AQUALAB.features.PerJobFeature import PerJobFeature
-from ogd.core.schemas.Event import Event
-from ogd.core.schemas.ExtractionMode import ExtractionMode
-from ogd.core.schemas.FeatureData import FeatureData
+from ogd.core.models.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
+from ogd.core.models.FeatureData import FeatureData
 
 class JobActiveTime(PerJobFeature):
 
     def __init__(self, params:GeneratorParameters, job_map:dict):
         super().__init__(params=params, job_map=job_map)
         self._total_time = timedelta(0)
         if self.ExtractionMode == ExtractionMode.PLAYER:
```

### Comparing `opengamedata_core-0.0.5/src/ogd/games/AQUALAB/features/JobArgumentation.py` & `opengamedata_core-0.0.6/src/ogd/games/AQUALAB/features/JobArgumentation.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 import logging
 from datetime import datetime, timedelta
 from typing import Any, List, Optional
 # import locals
 from ogd.core.utils.Logger import Logger
 from ogd.core.generators.Generator import GeneratorParameters
 from ogd.games.AQUALAB.features.PerJobFeature import PerJobFeature
-from ogd.core.schemas.Event import Event
-from ogd.core.schemas.ExtractionMode import ExtractionMode
-from ogd.core.schemas.FeatureData import FeatureData
+from ogd.core.models.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
+from ogd.core.models.FeatureData import FeatureData
 
 class JobArgumentation(PerJobFeature):
 
     def __init__(self, params:GeneratorParameters, job_map:dict):
         super().__init__(params=params, job_map=job_map)
         self._session_id = None
         self._argumentation_start_count : int = 0
```

### Comparing `opengamedata_core-0.0.5/src/ogd/games/AQUALAB/features/JobCompletionTime.py` & `opengamedata_core-0.0.6/src/ogd/games/AQUALAB/features/JobCompletionTime.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 import logging
 from datetime import timedelta
 from typing import Any, List, Optional
 # import locals
 from ogd.core.utils.Logger import Logger
 from ogd.core.generators.Generator import GeneratorParameters
 from ogd.games.AQUALAB.features.PerJobFeature import PerJobFeature
-from ogd.core.schemas.Event import Event
-from ogd.core.schemas.ExtractionMode import ExtractionMode
-from ogd.core.schemas.FeatureData import FeatureData
+from ogd.core.models.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
+from ogd.core.models.FeatureData import FeatureData
 
 class JobCompletionTime(PerJobFeature):
 
     def __init__(self, params:GeneratorParameters, job_map:dict):
         super().__init__(params=params, job_map=job_map)
         self._session_id = None
         self._job_start_time = None
```

### Comparing `opengamedata_core-0.0.5/src/ogd/games/AQUALAB/features/JobDiveSitesCount.py` & `opengamedata_core-0.0.6/src/ogd/games/AQUALAB/features/JobDiveSitesCount.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # import libraries
 import logging
 from typing import Any, List, Optional
 # import locals
 from ogd.core.utils.Logger import Logger
 from ogd.core.generators.Generator import GeneratorParameters
 from ogd.games.AQUALAB.features.PerJobFeature import PerJobFeature
-from ogd.core.schemas.Event import Event
-from ogd.core.schemas.ExtractionMode import ExtractionMode
-from ogd.core.schemas.FeatureData import FeatureData
+from ogd.core.models.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
+from ogd.core.models.FeatureData import FeatureData
 
 class JobDiveSitesCount(PerJobFeature):
     def __init__(self, params:GeneratorParameters, job_map:dict):
         super().__init__(params=params, job_map=job_map)
         self._count = 0
 
     # *** IMPLEMENT ABSTRACT FUNCTIONS ***
```

### Comparing `opengamedata_core-0.0.5/src/ogd/games/AQUALAB/features/JobDiveTime.py` & `opengamedata_core-0.0.6/src/ogd/games/PENGUINS/features/SnowBallDuration.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,57 +1,51 @@
 # import libraries
 import logging
-from datetime import timedelta
-from typing import Any, List, Optional
+from typing import Any, Dict, List, Optional
 # import locals
 from ogd.core.utils.Logger import Logger
+from datetime import datetime, timedelta
 from ogd.core.generators.Generator import GeneratorParameters
-from ogd.games.AQUALAB.features.PerJobFeature import PerJobFeature
-from ogd.core.schemas.Event import Event
-from ogd.core.schemas.ExtractionMode import ExtractionMode
-from ogd.core.schemas.FeatureData import FeatureData
+from ogd.core.models.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
+from ogd.core.models.FeatureData import FeatureData
+from ogd.core.generators.extractors.SessionFeature import SessionFeature
 
-class JobDiveTime(PerJobFeature):
+class SnowBallDuration(SessionFeature):
 
-    def __init__(self, params:GeneratorParameters, job_map:dict):
-        super().__init__(params=params, job_map=job_map)
+    def __init__(self, params:GeneratorParameters):
+        super().__init__(params=params)
         self._session_id = None
-        self._dive_start_time = None
+        self._argument_start_time : Optional[datetime] = None
         self._prev_timestamp = None
         self._time = 0
 
     # *** IMPLEMENT ABSTRACT FUNCTIONS ***
     @classmethod
     def _eventFilter(cls, mode:ExtractionMode) -> List[str]:
-        return ["all_events"]
+        return ["push_snowball"]
 
     @classmethod
     def _featureFilter(cls, mode:ExtractionMode) -> List[str]:
         return []
 
     def _updateFromEvent(self, event:Event) -> None:
         if event.SessionID != self._session_id:
             self._session_id = event.SessionID
             # if we jumped to a new session, we only want to count time up to last event, not the time between sessions.
-            if self._dive_start_time and self._prev_timestamp:
-                self._time += (self._prev_timestamp - self._dive_start_time).total_seconds()
-                self._dive_start_time = event.Timestamp
-
-        if event.EventName == "begin_dive":
-            self._dive_start_time = event.Timestamp
-        elif event.EventName == "scene_changed":
-            if self._dive_start_time is not None:
-                self._time += (event.Timestamp - self._dive_start_time).total_seconds()
-                self._dive_start_time = None
-
+            if self._argument_start_time and self._prev_timestamp:
+                self._time += (self._prev_timestamp - self._argument_start_time).total_seconds()
+                self._argument_start_time = event.Timestamp
+
+        elif event.EventName == "push_snowball" and self._argument_start_time is not None:
+            self._time = (event.Timestamp - self._argument_start_time).total_seconds()
+            self._argument_start_time = None
+            return
         self._prev_timestamp = event.Timestamp
-
+    
     def _updateFromFeatureData(self, feature:FeatureData):
         return
 
     def _getFeatureValues(self) -> List[Any]:
         return [timedelta(seconds=self._time)]
 
-    # *** Optionally override public functions. ***
-    @staticmethod
-    def MinVersion() -> Optional[str]:
-        return "1"
+
```

### Comparing `opengamedata_core-0.0.5/src/ogd/games/AQUALAB/features/JobExperimentation.py` & `opengamedata_core-0.0.6/src/ogd/games/AQUALAB/features/JobExperimentation.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 from datetime import timedelta
 from typing import Any, List, Optional
 
 # import locals
 from ogd.core.utils.Logger import Logger
 from ogd.core.generators.Generator import GeneratorParameters
 from ogd.games.AQUALAB.features.PerJobFeature import PerJobFeature
-from ogd.core.schemas.Event import Event
-from ogd.core.schemas.ExtractionMode import ExtractionMode
-from ogd.core.schemas.FeatureData import FeatureData
+from ogd.core.models.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
+from ogd.core.models.FeatureData import FeatureData
 
 class JobExperimentation(PerJobFeature):
 
     def __init__(self, params:GeneratorParameters, job_map:dict):
         super().__init__(params=params, job_map=job_map)
         self._session_id = None
         self._experiment_start_count : int = 0
```

### Comparing `opengamedata_core-0.0.5/src/ogd/games/AQUALAB/features/JobGuideCount.py` & `opengamedata_core-0.0.6/src/ogd/games/AQUALAB/features/JobTasksCompleted.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 # import libraries
 import logging
 from typing import Any, List, Optional
 # import locals
 from ogd.core.utils.Logger import Logger
 from ogd.core.generators.Generator import GeneratorParameters
 from ogd.games.AQUALAB.features.PerJobFeature import PerJobFeature
-from ogd.core.schemas.Event import Event
-from ogd.core.schemas.ExtractionMode import ExtractionMode
-from ogd.core.schemas.FeatureData import FeatureData
-
-class JobGuideCount(PerJobFeature):
+from ogd.core.models.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
+from ogd.core.models.FeatureData import FeatureData
 
+class JobTasksCompleted(PerJobFeature):
+    
     def __init__(self, params:GeneratorParameters, job_map:dict):
-        self._job_map = job_map
         super().__init__(params=params, job_map=job_map)
         self._count = 0
 
     # *** IMPLEMENT ABSTRACT FUNCTIONS ***
     @classmethod
     def _eventFilter(cls, mode:ExtractionMode) -> List[str]:
-        return ["guide_triggered"]
+        return ["complete_task"]
 
     @classmethod
     def _featureFilter(cls, mode:ExtractionMode) -> List[str]:
         return []
 
     def _updateFromEvent(self, event:Event) -> None:
         self._count += 1
@@ -33,8 +32,8 @@
 
     def _getFeatureValues(self) -> List[Any]:
         return [self._count]
 
     # *** Optionally override public functions. ***
     @staticmethod
     def MinVersion() -> Optional[str]:
-        return "1"
+        return "1"
```

### Comparing `opengamedata_core-0.0.5/src/ogd/games/AQUALAB/features/JobHelpCount.py` & `opengamedata_core-0.0.6/src/ogd/games/AQUALAB/features/JobHelpCount.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # import libraries
 import logging
 from typing import Any, Dict, List, Optional
 # import locals
 from ogd.core.utils.Logger import Logger
 from ogd.core.generators.Generator import GeneratorParameters
 from ogd.games.AQUALAB.features.PerJobFeature import PerJobFeature
-from ogd.core.schemas.Event import Event
-from ogd.core.schemas.ExtractionMode import ExtractionMode
-from ogd.core.schemas.FeatureData import FeatureData
+from ogd.core.models.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
+from ogd.core.models.FeatureData import FeatureData
 
 class JobHelpCount(PerJobFeature):
 
     def __init__(self, params:GeneratorParameters, job_map:dict):
         self._job_map = job_map
         super().__init__(params=params, job_map=job_map)
         self._by_task       : Dict[str, int] = {}
```

### Comparing `opengamedata_core-0.0.5/src/ogd/games/AQUALAB/features/JobLocationChanges.py` & `opengamedata_core-0.0.6/src/ogd/games/AQUALAB/features/JobLocationChanges.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # import libraries
 from datetime import datetime
 from typing import Any, Dict, List, Optional
 # import locals
 from ogd.core.utils.Logger import Logger
 from ogd.core.generators.Generator import GeneratorParameters
 from ogd.games.AQUALAB.features.PerJobFeature import PerJobFeature
-from ogd.core.schemas.Event import Event
-from ogd.core.schemas.ExtractionMode import ExtractionMode
-from ogd.core.schemas.FeatureData import FeatureData
+from ogd.core.models.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
+from ogd.core.models.FeatureData import FeatureData
 
 class JobLocationChanges(PerJobFeature):
 
     def __init__(self, params:GeneratorParameters, job_map:dict):
         self._job_map = job_map
         super().__init__(params=params, job_map=job_map)
         self._by_task       : Dict[str, int] = {}
```

### Comparing `opengamedata_core-0.0.5/src/ogd/games/AQUALAB/features/JobModeling.py` & `opengamedata_core-0.0.6/src/ogd/games/AQUALAB/features/JobModeling.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 import logging
 from datetime import timedelta
 from typing import Any, List, Optional
 # import locals
 from ogd.core.utils.Logger import Logger
 from ogd.core.generators.Generator import GeneratorParameters
 from ogd.games.AQUALAB.features.PerJobFeature import PerJobFeature
-from ogd.core.schemas.Event import Event
-from ogd.core.schemas.ExtractionMode import ExtractionMode
-from ogd.core.schemas.FeatureData import FeatureData
+from ogd.core.models.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
+from ogd.core.models.FeatureData import FeatureData
 
 class JobModeling(PerJobFeature):
     def __init__(self, params:GeneratorParameters, job_map:dict):
         self._job_map = job_map
         super().__init__(params=params, job_map=job_map)
         self._session_id = None
         self._modeling_start_count : int = 0
```

### Comparing `opengamedata_core-0.0.5/src/ogd/games/AQUALAB/features/JobPlayTime.py` & `opengamedata_core-0.0.6/src/ogd/games/AQUALAB/features/JobPlayTime.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 from datetime import datetime, timedelta
 import logging, warnings
 from typing import Any, Final, List, Optional
 # import locals
 from ogd.core.utils.Logger import Logger
 from ogd.core.generators.extractors.Extractor import GeneratorParameters
 from ogd.core.generators.extractors.Feature import Feature
-from ogd.core.schemas.Event import Event
-from ogd.core.schemas.ExtractionMode import ExtractionMode
-from ogd.core.schemas.FeatureData import FeatureData
+from ogd.core.models.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
+from ogd.core.models.FeatureData import FeatureData
 
 class JobPlayTime(Feature):
     IDLE_LEVEL : Final[int] = 30
 
     def __init__(self, params:GeneratorParameters, job_map:dict, active_threads:Optional[float] = None):
         self._job_map = job_map
         super().__init__(params=params)
```

### Comparing `opengamedata_core-0.0.5/src/ogd/games/AQUALAB/features/JobPriorAttempt.py` & `opengamedata_core-0.0.6/src/ogd/games/AQUALAB/features/JobPriorAttempt.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # import libraries
 import logging
 from typing import Any, Dict, List, Optional
 # import locals
 from ogd.core.utils.Logger import Logger
 from ogd.core.generators.extractors.Extractor import GeneratorParameters
 from ogd.core.generators.extractors.PerCountFeature import PerCountFeature
-from ogd.core.schemas.Event import Event
-from ogd.core.schemas.ExtractionMode import ExtractionMode
-from ogd.core.schemas.FeatureData import FeatureData
+from ogd.core.models.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
+from ogd.core.models.FeatureData import FeatureData
 
 class JobPriorAttempt(PerCountFeature):
 
     def __init__(self, params:GeneratorParameters, job_map:dict):
         self._job_map = job_map
         super().__init__(params=params)
         self._prior_list = set()
```

### Comparing `opengamedata_core-0.0.5/src/ogd/games/AQUALAB/features/JobPriorComplete.py` & `opengamedata_core-0.0.6/src/ogd/games/AQUALAB/features/JobPriorComplete.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # import libraries
 import logging
 from typing import Any, Dict, List, Optional
 # import locals
 from ogd.core.utils.Logger import Logger
 from ogd.core.generators.extractors.Extractor import GeneratorParameters
 from ogd.core.generators.extractors.PerCountFeature import PerCountFeature
-from ogd.core.schemas.Event import Event
-from ogd.core.schemas.ExtractionMode import ExtractionMode
-from ogd.core.schemas.FeatureData import FeatureData
+from ogd.core.models.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
+from ogd.core.models.FeatureData import FeatureData
 
 class JobPriorComplete(PerCountFeature):
 
     def __init__(self, params:GeneratorParameters, job_map:dict):
         self._job_map = job_map
         super().__init__(params=params)
         self._prior_list = set()
```

### Comparing `opengamedata_core-0.0.5/src/ogd/games/AQUALAB/features/JobStartCount.py` & `opengamedata_core-0.0.6/src/ogd/games/AQUALAB/features/JobStartCount.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 import logging
 from typing import Any, Dict, List, Optional
 # import locals
 from ogd.core.utils.Logger import Logger
 from ogd.core.generators.Generator import GeneratorParameters
 from ogd.core.generators.extractors.Feature import Feature
 from ogd.games.AQUALAB.features.PerJobFeature import PerJobFeature
-from ogd.core.schemas.Event import Event
-from ogd.core.schemas.ExtractionMode import ExtractionMode
-from ogd.core.schemas.FeatureData import FeatureData
+from ogd.core.models.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
+from ogd.core.models.FeatureData import FeatureData
 
 class JobStartCount(PerJobFeature):
 
     def __init__(self, params:GeneratorParameters, job_map:dict):
         self._job_map = job_map
         super().__init__(params=params, job_map=job_map)
         self._current_count : int = 0
```

### Comparing `opengamedata_core-0.0.5/src/ogd/games/AQUALAB/features/JobTasksCompleted.py` & `opengamedata_core-0.0.6/src/ogd/games/ICECUBE/features/ScenesEncountered.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,39 +1,42 @@
 # import libraries
 import logging
-from typing import Any, List, Optional
+from typing import Any, Dict, List, Optional
 # import locals
 from ogd.core.utils.Logger import Logger
 from ogd.core.generators.Generator import GeneratorParameters
-from ogd.games.AQUALAB.features.PerJobFeature import PerJobFeature
-from ogd.core.schemas.Event import Event
-from ogd.core.schemas.ExtractionMode import ExtractionMode
-from ogd.core.schemas.FeatureData import FeatureData
-
-class JobTasksCompleted(PerJobFeature):
-    
-    def __init__(self, params:GeneratorParameters, job_map:dict):
-        super().__init__(params=params, job_map=job_map)
-        self._count = 0
+from ogd.core.generators.extractors.Feature import Feature
+from ogd.core.generators.extractors.SessionFeature import SessionFeature
+from ogd.core.models.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
+from ogd.core.models.FeatureData import FeatureData
+
+class ScenesEncountered(SessionFeature):
+
+    def __init__(self, params:GeneratorParameters):
+        super().__init__(params=params)
+        self._scene_name = None
+        self._cnt_list = list()
 
     # *** IMPLEMENT ABSTRACT FUNCTIONS ***
     @classmethod
     def _eventFilter(cls, mode:ExtractionMode) -> List[str]:
-        return ["complete_task"]
+        return ["scene_change"]
 
     @classmethod
     def _featureFilter(cls, mode:ExtractionMode) -> List[str]:
         return []
 
     def _updateFromEvent(self, event:Event) -> None:
-        self._count += 1
+        self._scene_name = event.EventData.get("scene_name")
+        self._cnt_list.append(self._scene_name)
 
     def _updateFromFeatureData(self, feature:FeatureData):
         return
 
     def _getFeatureValues(self) -> List[Any]:
-        return [self._count]
+        return [self._cnt_list]
 
     # *** Optionally override public functions. ***
     @staticmethod
     def MinVersion() -> Optional[str]:
-        return "1"
+        return "2"
```

### Comparing `opengamedata_core-0.0.5/src/ogd/games/AQUALAB/features/JobTriesInArgument.py` & `opengamedata_core-0.0.6/src/ogd/games/AQUALAB/features/JobTriesInArgument.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # import libraries
 import logging
 from typing import Any, List, Optional
 # import locals
 from ogd.core.utils.Logger import Logger
 from ogd.core.generators.Generator import GeneratorParameters
 from ogd.games.AQUALAB.features.PerJobFeature import PerJobFeature
-from ogd.core.schemas.Event import Event
-from ogd.core.schemas.ExtractionMode import ExtractionMode
-from ogd.core.schemas.FeatureData import FeatureData
+from ogd.core.models.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
+from ogd.core.models.FeatureData import FeatureData
 
 
 class JobTriesInArgument(PerJobFeature):
     
     def __init__(self, params:GeneratorParameters, job_map:dict):
         super().__init__(params=params, job_map=job_map)
         self._count = 0
```

### Comparing `opengamedata_core-0.0.5/src/ogd/games/AQUALAB/features/JobsAttempted.py` & `opengamedata_core-0.0.6/src/ogd/games/AQUALAB/features/JobsAttempted.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 # import libraries
 import logging
 from datetime import datetime, timedelta
 from statistics import stdev
 from typing import Any, List, Optional
-from ogd.core.schemas.ExtractionMode import ExtractionMode
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
 # import locals
 from ogd.core.utils.Logger import Logger
 from ogd.core.generators.Generator import GeneratorParameters
 from ogd.core.generators.extractors.Feature import Feature
-from ogd.core.schemas.Event import Event
-from ogd.core.schemas.ExtractionMode import ExtractionMode
-from ogd.core.schemas.FeatureData import FeatureData
+from ogd.core.models.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
+from ogd.core.models.FeatureData import FeatureData
 
 class JobsAttempted(Feature):
 
     def __init__(self, params:GeneratorParameters, job_map:dict, diff_map: dict):
         self._player_id = None
 
         self._job_map = job_map
```

### Comparing `opengamedata_core-0.0.5/src/ogd/games/AQUALAB/features/JobsCompleted.py` & `opengamedata_core-0.0.6/src/ogd/games/AQUALAB/features/JobsCompleted.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Any, List
 
 from ogd.core.generators.Generator import GeneratorParameters
 from ogd.core.generators.extractors.SessionFeature import SessionFeature
-from ogd.core.schemas.Event import Event
-from ogd.core.schemas.ExtractionMode import ExtractionMode
-from ogd.core.schemas.FeatureData import FeatureData
+from ogd.core.models.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
+from ogd.core.models.FeatureData import FeatureData
 
 class JobsCompleted(SessionFeature):
 
     def __init__(self, params:GeneratorParameters, player_id:str):
         self._player_id = player_id
         super().__init__(params=params)
         self._jobs_completed = []
```

### Comparing `opengamedata_core-0.0.5/src/ogd/games/AQUALAB/features/ModelExportCount.py` & `opengamedata_core-0.0.6/src/ogd/games/AQUALAB/features/ModelExportCount.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 from datetime import datetime, timedelta
 import logging, warnings
 from typing import Any, List, Optional
 # import locals
 from ogd.core.utils.Logger import Logger
 from ogd.core.generators.Generator import GeneratorParameters
 from ogd.core.generators.extractors.Feature import Feature
-from ogd.core.schemas.Event import Event
-from ogd.core.schemas.ExtractionMode import ExtractionMode
-from ogd.core.schemas.FeatureData import FeatureData
+from ogd.core.models.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
+from ogd.core.models.FeatureData import FeatureData
 
 
 class ModelExportCount(Feature):
 
     def __init__(self, params:GeneratorParameters, job_map:dict):
         self._job_map = job_map
         super().__init__(params=params)
```

### Comparing `opengamedata_core-0.0.5/src/ogd/games/AQUALAB/features/ModelInterveneCount.py` & `opengamedata_core-0.0.6/src/ogd/games/AQUALAB/features/ModelInterveneCount.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 from datetime import datetime, timedelta
 import logging, warnings
 from typing import Any, List, Optional
 # import locals
 from ogd.core.utils.Logger import Logger
 from ogd.core.generators.Generator import GeneratorParameters
 from ogd.core.generators.extractors.Feature import Feature
-from ogd.core.schemas.Event import Event
-from ogd.core.schemas.ExtractionMode import ExtractionMode
-from ogd.core.schemas.FeatureData import FeatureData
+from ogd.core.models.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
+from ogd.core.models.FeatureData import FeatureData
 
 
 class ModelInterveneCount(Feature):
 
     def __init__(self, params:GeneratorParameters, job_map:dict):
         self._job_map = job_map
         super().__init__(params=params)
```

### Comparing `opengamedata_core-0.0.5/src/ogd/games/AQUALAB/features/ModelPredictCount.py` & `opengamedata_core-0.0.6/src/ogd/games/AQUALAB/features/ModelPredictCount.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 from datetime import datetime, timedelta
 import logging, warnings
 from typing import Any, List, Optional
 # import locals
 from ogd.core.utils.Logger import Logger
 from ogd.core.generators.Generator import GeneratorParameters
 from ogd.core.generators.extractors.Feature import Feature
-from ogd.core.schemas.Event import Event
-from ogd.core.schemas.ExtractionMode import ExtractionMode
-from ogd.core.schemas.FeatureData import FeatureData
+from ogd.core.models.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
+from ogd.core.models.FeatureData import FeatureData
 
 
 class ModelPredictCount(Feature):
 
     def __init__(self, params:GeneratorParameters, job_map:dict):
         self._job_map = job_map
         super().__init__(params=params)
```

### Comparing `opengamedata_core-0.0.5/src/ogd/games/AQUALAB/features/PerJobFeature.py` & `opengamedata_core-0.0.6/src/ogd/games/AQUALAB/features/PerJobFeature.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # import libraries
 import logging
 from typing import Optional
 # import locals
 from ogd.core.utils.Logger import Logger
 from ogd.core.generators.Generator import GeneratorParameters
 from ogd.core.generators.extractors.PerCountFeature import PerCountFeature
-from ogd.core.schemas.Event import Event
+from ogd.core.models.Event import Event
 
 class PerJobFeature(PerCountFeature):
     def __init__(self, params:GeneratorParameters, job_map:dict):
         super().__init__(params=params,)
         self._job_map = job_map
 
     # *** IMPLEMENT ABSTRACT FUNCTIONS ***
```

### Comparing `opengamedata_core-0.0.5/src/ogd/games/AQUALAB/features/PlayerSummary.py` & `opengamedata_core-0.0.6/src/ogd/games/AQUALAB/features/PlayerSummary.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import logging
 from datetime import timedelta
 from multiprocessing.sharedctypes import Value
 from typing import Any, List
 
 from ogd.core.generators.Generator import GeneratorParameters
 from ogd.core.generators.extractors.SessionFeature import SessionFeature
-from ogd.core.schemas.Event import Event
-from ogd.core.schemas.ExtractionMode import ExtractionMode
-from ogd.core.schemas.FeatureData import FeatureData
-from ogd.core.schemas.ExtractionMode import ExtractionMode
+from ogd.core.models.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
+from ogd.core.models.FeatureData import FeatureData
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
 from ogd.core.utils.Logger import Logger
 
 class PlayerSummary(SessionFeature):
 
     def __init__(self, params:GeneratorParameters):
         super().__init__(params=params)
         self._summary = {}
```

### Comparing `opengamedata_core-0.0.5/src/ogd/games/AQUALAB/features/PopulationSummary.py` & `opengamedata_core-0.0.6/src/ogd/games/AQUALAB/features/PopulationSummary.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from collections import defaultdict
 from datetime import timedelta
 from typing import Any, Dict, List
 
 from ogd.core.generators.Generator import GeneratorParameters
 from ogd.core.generators.extractors.SessionFeature import SessionFeature
-from ogd.core.schemas.Event import Event
-from ogd.core.schemas.ExtractionMode import ExtractionMode
-from ogd.core.schemas.FeatureData import FeatureData
+from ogd.core.models.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
+from ogd.core.models.FeatureData import FeatureData
 
 class PopulationSummary(SessionFeature):
 
     def __init__(self, params:GeneratorParameters):
         super().__init__(params=params)
         self._user_sessions = defaultdict(list)
         self._user_completions = defaultdict(list)
```

### Comparing `opengamedata_core-0.0.5/src/ogd/games/AQUALAB/features/RegionJobCount.py` & `opengamedata_core-0.0.6/src/ogd/games/AQUALAB/features/RegionJobCount.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 import logging
 from datetime import timedelta
 from typing import Any, List, Optional
 # import locals
 from ogd.core.utils.Logger import Logger
 from ogd.core.generators.extractors.Extractor import GeneratorParameters
 from ogd.games.AQUALAB.features.PerJobFeature import PerJobFeature
-from ogd.core.schemas.Event import Event
-from ogd.core.schemas.ExtractionMode import ExtractionMode
-from ogd.core.schemas.FeatureData import FeatureData
+from ogd.core.models.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
+from ogd.core.models.FeatureData import FeatureData
 from ogd.core.generators.extractors.PerCountFeature import PerCountFeature
 
 class RegionJobCount(PerCountFeature):
     def __init__(self, params:GeneratorParameters):
         super().__init__(params=params)
         regions = ['arctic', 'coral', 'bayou', 'kelp', 'other']
         self.count = 0
```

### Comparing `opengamedata_core-0.0.5/src/ogd/games/AQUALAB/features/RegionName.py` & `opengamedata_core-0.0.6/src/ogd/games/ICECUBE/features/HeadsetOnCount.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 # import libraries
-from typing import Any, List, Optional
+import logging
+from typing import Any, Dict, List, Optional
 # import locals
-from ogd.core.generators.extractors.Extractor import GeneratorParameters
-from ogd.core.schemas.Event import Event
-from ogd.core.schemas.ExtractionMode import ExtractionMode
-from ogd.core.schemas.FeatureData import FeatureData
-from ogd.core.generators.extractors.PerCountFeature import PerCountFeature
+from ogd.core.utils.Logger import Logger
+from ogd.core.generators.Generator import GeneratorParameters
+from ogd.core.generators.extractors.Feature import Feature
+from ogd.core.generators.extractors.SessionFeature import SessionFeature
+from ogd.core.models.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
+from ogd.core.models.FeatureData import FeatureData
+
+class HeadsetOnCount(SessionFeature):
 
-class RegionName(PerCountFeature):
     def __init__(self, params:GeneratorParameters):
         super().__init__(params=params)
-        regions = ['arctic', 'coral', 'bayou', 'kelp', 'other']
-        self.count = 0
-        self.region = regions[self.CountIndex]
+        self._headset_count : int = 0
+
     # *** IMPLEMENT ABSTRACT FUNCTIONS ***
     @classmethod
     def _eventFilter(cls, mode:ExtractionMode) -> List[str]:
-        return []
+        return ["headset_on"]
 
     @classmethod
     def _featureFilter(cls, mode:ExtractionMode) -> List[str]:
         return []
 
-    def _validateEventCountIndex(self, event:Event):
-        pass
-
     def _updateFromEvent(self, event:Event) -> None:
-        pass
+        self._headset_count += 1
 
     def _updateFromFeatureData(self, feature:FeatureData):
         return
 
     def _getFeatureValues(self) -> List[Any]:
-        return [self.region]
+        return [self._headset_count]
 
     # *** Optionally override public functions. ***
     @staticmethod
     def MinVersion() -> Optional[str]:
-        return "1"
+        return "2"
```

### Comparing `opengamedata_core-0.0.5/src/ogd/games/AQUALAB/features/SessionDiveSitesCount.py` & `opengamedata_core-0.0.6/src/ogd/games/AQUALAB/features/SessionDiveSitesCount.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # import libraries
 from typing import Any, List
 # import locals
 from ogd.core.generators.Generator import GeneratorParameters
 from ogd.core.generators.extractors.Feature import Feature
-from ogd.core.schemas.Event import Event
-from ogd.core.schemas.ExtractionMode import ExtractionMode
-from ogd.core.schemas.FeatureData import FeatureData
+from ogd.core.models.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
+from ogd.core.models.FeatureData import FeatureData
 
 class SessionDiveSitesCount(Feature):
     
     def __init__(self, params:GeneratorParameters):
         super().__init__(params=params)
         self._count = 0
         self._visited_sites = []
```

### Comparing `opengamedata_core-0.0.5/src/ogd/games/AQUALAB/features/SessionDuration.py` & `opengamedata_core-0.0.6/src/ogd/games/AQUALAB/features/SessionDuration.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # import libraries
 import logging
 from datetime import timedelta
 from typing import Any, List
 # import locals
 from ogd.core.generators.Generator import GeneratorParameters
 from ogd.core.generators.extractors.SessionFeature import SessionFeature
-from ogd.core.schemas.Event import Event, EventSource
-from ogd.core.schemas.ExtractionMode import ExtractionMode
-from ogd.core.schemas.FeatureData import FeatureData
+from ogd.core.models.Event import Event, EventSource
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
+from ogd.core.models.FeatureData import FeatureData
 from ogd.core.utils.Logger import Logger
 
 class SessionDuration(SessionFeature):
 
     def __init__(self, params:GeneratorParameters, threshold:int):
         self.threshold = threshold
         super().__init__(params=params)
```

### Comparing `opengamedata_core-0.0.5/src/ogd/games/AQUALAB/features/SessionGuideCount.py` & `opengamedata_core-0.0.6/src/ogd/games/WAVES/features/ClosenessSlope.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 # import libraries
-from typing import Any, List
+from ogd.core.models import Event
+from typing import Any, List, Optional
 # import locals
-from ogd.core.generators.Generator import GeneratorParameters
 from ogd.core.generators.extractors.Feature import Feature
-from ogd.core.schemas.Event import Event
-from ogd.core.schemas.ExtractionMode import ExtractionMode
-from ogd.core.schemas.FeatureData import FeatureData
+from ogd.core.generators.Generator import GeneratorParameters
+from ogd.core.models.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
+from ogd.core.models.FeatureData import FeatureData
 
-class SessionGuideCount(Feature):
 
+class ClosenessSlope(Feature):
     def __init__(self, params:GeneratorParameters):
-        super().__init__(params=params)
-        self._count = 0
+        Feature.__init__(self, params=params)
 
     # *** IMPLEMENT ABSTRACT FUNCTIONS ***
     @classmethod
     def _eventFilter(cls, mode:ExtractionMode) -> List[str]:
-        return ["guide_triggered"]
+        return []
 
     @classmethod
     def _featureFilter(cls, mode:ExtractionMode) -> List[str]:
         return []
 
     def _updateFromEvent(self, event:Event) -> None:
-        self._count += 1
+        return
 
     def _updateFromFeatureData(self, feature:FeatureData):
         return
 
     def _getFeatureValues(self) -> List[Any]:
-        return [self._count]
+        return ["Not Implemented"]
 
     # *** Optionally override public functions. ***
```

### Comparing `opengamedata_core-0.0.5/src/ogd/games/AQUALAB/features/SessionHelpCount.py` & `opengamedata_core-0.0.6/src/ogd/games/PENGUINS/features/LogVersion.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,37 +1,44 @@
-from typing import Any, List
+# import libraries
+import logging
+from typing import Any, Dict, List, Optional
 # import locals
+from ogd.core.utils.Logger import Logger
 from ogd.core.generators.Generator import GeneratorParameters
-from ogd.core.generators.extractors.Feature import Feature
-from ogd.core.schemas.Event import Event
-from ogd.core.schemas.ExtractionMode import ExtractionMode
-from ogd.core.schemas.FeatureData import FeatureData
-
-class SessionHelpCount(Feature):
-    """_summary_
-
-    :param Feature: _description_
-    :type Feature: _type_
-    """
+from ogd.core.models.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
+from ogd.core.models.FeatureData import FeatureData
+from ogd.core.generators.extractors.SessionFeature import SessionFeature
+
+
+class LogVersion(SessionFeature):
+
     def __init__(self, params:GeneratorParameters):
         super().__init__(params=params)
-        self._count = 0
+        self._current_log : str = "UNKNOWN LOG VERSION"
 
     # *** IMPLEMENT ABSTRACT FUNCTIONS ***
     @classmethod
     def _eventFilter(cls, mode:ExtractionMode) -> List[str]:
-        return ["ask_for_help"]
+        return ["all_events"]
 
     @classmethod
     def _featureFilter(cls, mode:ExtractionMode) -> List[str]:
         return []
 
     def _updateFromEvent(self, event:Event) -> None:
-        self._count += 1
+        self._current_log = event.LogVersion
+
 
     def _updateFromFeatureData(self, feature:FeatureData):
         return
 
     def _getFeatureValues(self) -> List[Any]:
-        return [self._count]
-
+        return [self._current_log]
+    
     # *** Optionally override public functions. ***
+
+    @staticmethod
+    def AvailableModes() -> List[ExtractionMode]:
+        return [ExtractionMode.SESSION]
+
+
```

### Comparing `opengamedata_core-0.0.5/src/ogd/games/AQUALAB/features/SessionID.py` & `opengamedata_core-0.0.6/src/ogd/games/AQUALAB/features/SessionID.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Any, List
 
 from ogd.core.generators.Generator import GeneratorParameters
 from ogd.core.generators.extractors.SessionFeature import SessionFeature
-from ogd.core.schemas.Event import Event
-from ogd.core.schemas.ExtractionMode import ExtractionMode
-from ogd.core.schemas.FeatureData import FeatureData
+from ogd.core.models.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
+from ogd.core.models.FeatureData import FeatureData
 
 class SessionID(SessionFeature):
     """_summary_
 
     :param SessionFeature: _description_
     :type SessionFeature: _type_
     """
```

### Comparing `opengamedata_core-0.0.5/src/ogd/games/AQUALAB/features/SessionJobsCompleted.py` & `opengamedata_core-0.0.6/src/ogd/games/AQUALAB/features/SessionHelpCount.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 from typing import Any, List
-
+# import locals
 from ogd.core.generators.Generator import GeneratorParameters
 from ogd.core.generators.extractors.Feature import Feature
-from ogd.core.schemas.Event import Event
-from ogd.core.schemas.ExtractionMode import ExtractionMode
-from ogd.core.schemas.FeatureData import FeatureData
+from ogd.core.models.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
+from ogd.core.models.FeatureData import FeatureData
 
-class SessionJobsCompleted(Feature):
+class SessionHelpCount(Feature):
     """_summary_
 
     :param Feature: _description_
     :type Feature: _type_
     """
     def __init__(self, params:GeneratorParameters):
         super().__init__(params=params)
         self._count = 0
 
     # *** IMPLEMENT ABSTRACT FUNCTIONS ***
     @classmethod
     def _eventFilter(cls, mode:ExtractionMode) -> List[str]:
-        return ["complete_job"]
+        return ["ask_for_help"]
 
     @classmethod
     def _featureFilter(cls, mode:ExtractionMode) -> List[str]:
         return []
 
     def _updateFromEvent(self, event:Event) -> None:
         self._count += 1
```

### Comparing `opengamedata_core-0.0.5/src/ogd/games/AQUALAB/features/SwitchJobsCount.py` & `opengamedata_core-0.0.6/src/ogd/games/AQUALAB/features/SwitchJobsCount.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # import libraries
 from typing import Any, List
 # import locals
 from ogd.core.generators.Generator import GeneratorParameters
 from ogd.core.generators.extractors.Feature import Feature
-from ogd.core.schemas.Event import Event
-from ogd.core.schemas.ExtractionMode import ExtractionMode
-from ogd.core.schemas.FeatureData import FeatureData
+from ogd.core.models.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
+from ogd.core.models.FeatureData import FeatureData
 
 class SwitchJobsCount(Feature):
     
     def __init__(self, params:GeneratorParameters):
         super().__init__(params=params)
         self._count = 0
```

### Comparing `opengamedata_core-0.0.5/src/ogd/games/AQUALAB/features/SyncCompletionTime.py` & `opengamedata_core-0.0.6/src/ogd/games/AQUALAB/features/SyncCompletionTime.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 import logging
 from datetime import datetime, timedelta
 from typing import Any, List, Optional
 # import locals
 from ogd.core.utils.Logger import Logger
 from ogd.core.generators.Generator import GeneratorParameters
 from ogd.core.generators.extractors.Feature import Feature
-from ogd.core.schemas.Event import Event
-from ogd.core.schemas.ExtractionMode import ExtractionMode
-from ogd.core.schemas.FeatureData import FeatureData
+from ogd.core.models.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
+from ogd.core.models.FeatureData import FeatureData
 
 class SyncCompletionTime(Feature):
 
     def __init__(self, params:GeneratorParameters):
         super().__init__(params=params)
         self._session_id = None
         self._sim_start_time : Optional[datetime] = None
```

### Comparing `opengamedata_core-0.0.5/src/ogd/games/AQUALAB/features/TankRulesCount.py` & `opengamedata_core-0.0.6/src/ogd/games/AQUALAB/features/TankRulesCount.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # import libraries
 from datetime import timedelta
 from typing import Any, Final, List
 # import locals
 from ogd.core.generators.Generator import GeneratorParameters
 from ogd.core.generators.extractors.PerCountFeature import PerCountFeature
-from ogd.core.schemas.Event import Event
-from ogd.core.schemas.ExtractionMode import ExtractionMode
-from ogd.core.schemas.FeatureData import FeatureData
+from ogd.core.models.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
+from ogd.core.models.FeatureData import FeatureData
 
 TANK_TYPE : Final[List[str]] = [
     "Observation",
     "Stress",
     "Measurement"]
 
 class TankRulesCount(PerCountFeature):
```

### Comparing `opengamedata_core-0.0.5/src/ogd/games/AQUALAB/features/TopJobCompletionDestinations.py` & `opengamedata_core-0.0.6/src/ogd/games/AQUALAB/features/TopJobCompletionDestinations.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 import logging
 from collections import defaultdict
 from typing import Any, List, Optional
 # import locals
 from ogd.core.utils.Logger import Logger
 from ogd.core.generators.Generator import GeneratorParameters
 from ogd.core.generators.extractors.Feature import Feature
-from ogd.core.schemas.Event import Event
-from ogd.core.schemas.ExtractionMode import ExtractionMode
-from ogd.core.schemas.FeatureData import FeatureData
+from ogd.core.models.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
+from ogd.core.models.FeatureData import FeatureData
 
 class TopJobCompletionDestinations(Feature):
 
     def __init__(self, params:GeneratorParameters, job_map:dict):
         self._job_map = job_map
         super().__init__(params=params)
         self._current_user_code = None
```

### Comparing `opengamedata_core-0.0.5/src/ogd/games/AQUALAB/features/TopJobSwitchDestinations.py` & `opengamedata_core-0.0.6/src/ogd/games/AQUALAB/features/TopJobSwitchDestinations.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 import logging
 from collections import defaultdict
 from typing import Any, List, Optional
 # import locals
 from ogd.core.utils.Logger import Logger
 from ogd.core.generators.extractors.Feature import Feature
 from ogd.core.generators.Generator import GeneratorParameters
-from ogd.core.schemas.Event import Event
-from ogd.core.schemas.ExtractionMode import ExtractionMode
-from ogd.core.schemas.FeatureData import FeatureData
+from ogd.core.models.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
+from ogd.core.models.FeatureData import FeatureData
 
 class TopJobSwitchDestinations(Feature):
 
     def __init__(self, params:GeneratorParameters, job_map:dict):
         self._job_map = job_map
         super().__init__(params=params)
         self._current_user_code = None
```

### Comparing `opengamedata_core-0.0.5/src/ogd/games/AQUALAB/features/TotalArcticTime.py` & `opengamedata_core-0.0.6/src/ogd/games/AQUALAB/features/TotalArcticTime.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # import libraries
 from datetime import timedelta
 from typing import Any, List
 # import locals
 from ogd.core.generators.extractors.Extractor import GeneratorParameters
 from ogd.core.generators.extractors.Feature import Feature
-from ogd.core.schemas.Event import Event, EventSource
-from ogd.core.schemas.ExtractionMode import ExtractionMode
-from ogd.core.schemas.FeatureData import FeatureData
+from ogd.core.models.Event import Event, EventSource
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
+from ogd.core.models.FeatureData import FeatureData
 from ogd.core.utils.Logger import Logger
 from ogd.games.AQUALAB.features.PerJobFeature import PerJobFeature
 from ogd.core.generators.extractors.PerCountFeature import PerCountFeature
 
 class TotalArcticTime(Feature):
     def __init__(self, params:GeneratorParameters):
         super().__init__(params=params)
```

### Comparing `opengamedata_core-0.0.5/src/ogd/games/AQUALAB/features/TotalArgumentationTime.py` & `opengamedata_core-0.0.6/src/ogd/games/AQUALAB/features/TotalArgumentationTime.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # import libraries
 from datetime import timedelta
 from typing import Any, List
 # import locals
 from ogd.core.generators.Generator import GeneratorParameters
 from ogd.core.generators.extractors.Feature import Feature
-from ogd.core.schemas.Event import Event, EventSource
-from ogd.core.schemas.ExtractionMode import ExtractionMode
-from ogd.core.schemas.FeatureData import FeatureData
+from ogd.core.models.Event import Event, EventSource
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
+from ogd.core.models.FeatureData import FeatureData
 
 class TotalArgumentationTime(Feature):
     
     def __init__(self, params:GeneratorParameters):
         super().__init__(params=params)
         self.prev_time = timedelta(0)
         self.total_time = timedelta(0)
```

### Comparing `opengamedata_core-0.0.5/src/ogd/games/AQUALAB/features/TotalBayouTime.py` & `opengamedata_core-0.0.6/src/ogd/games/AQUALAB/features/TotalBayouTime.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # import libraries
 from datetime import timedelta
 from typing import Any, List
 # import locals
 from ogd.core.generators.extractors.Extractor import GeneratorParameters
 from ogd.core.generators.extractors.Feature import Feature
-from ogd.core.schemas.Event import Event, EventSource
-from ogd.core.schemas.ExtractionMode import ExtractionMode
-from ogd.core.schemas.FeatureData import FeatureData
+from ogd.core.models.Event import Event, EventSource
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
+from ogd.core.models.FeatureData import FeatureData
 from ogd.core.utils.Logger import Logger
 from ogd.games.AQUALAB.features.PerJobFeature import PerJobFeature
 from ogd.core.generators.extractors.PerCountFeature import PerCountFeature
 
 class TotalBayouTime(Feature):
     def __init__(self, params:GeneratorParameters):
         super().__init__(params=params)
```

### Comparing `opengamedata_core-0.0.5/src/ogd/games/AQUALAB/features/TotalCoralTime.py` & `opengamedata_core-0.0.6/src/ogd/games/AQUALAB/features/TotalCoralTime.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # import libraries
 from datetime import timedelta
 from typing import Any, List
 # import locals
 from ogd.core.generators.extractors.Extractor import GeneratorParameters
 from ogd.core.generators.extractors.Feature import Feature
-from ogd.core.schemas.Event import Event, EventSource
-from ogd.core.schemas.ExtractionMode import ExtractionMode
-from ogd.core.schemas.FeatureData import FeatureData
+from ogd.core.models.Event import Event, EventSource
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
+from ogd.core.models.FeatureData import FeatureData
 from ogd.core.utils.Logger import Logger
 from ogd.games.AQUALAB.features.PerJobFeature import PerJobFeature
 from ogd.core.generators.extractors.PerCountFeature import PerCountFeature
 
 class TotalCoralTime(Feature):
     def __init__(self, params:GeneratorParameters):
         super().__init__(params=params)
```

### Comparing `opengamedata_core-0.0.5/src/ogd/games/AQUALAB/features/TotalDiveTime.py` & `opengamedata_core-0.0.6/src/ogd/games/AQUALAB/features/TotalDiveTime.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # import libraries
 from datetime import timedelta
 from typing import Any, List
 # import locals
 from ogd.core.generators.Generator import GeneratorParameters
 from ogd.core.generators.extractors.Feature import Feature
-from ogd.core.schemas.Event import Event, EventSource
-from ogd.core.schemas.ExtractionMode import ExtractionMode
-from ogd.core.schemas.FeatureData import FeatureData
+from ogd.core.models.Event import Event, EventSource
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
+from ogd.core.models.FeatureData import FeatureData
 
 class TotalDiveTime(Feature):
     
     def __init__(self, params:GeneratorParameters):
         super().__init__(params=params)
         self.prev_time = timedelta(0)
         self.total_time = timedelta(0)
```

### Comparing `opengamedata_core-0.0.5/src/ogd/games/AQUALAB/features/TotalExperimentationTime.py` & `opengamedata_core-0.0.6/src/ogd/games/AQUALAB/features/TotalExperimentationTime.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # import libraries
 from datetime import timedelta
 from typing import Any, List
 # import locals
 from ogd.core.generators.Generator import GeneratorParameters
 from ogd.core.generators.extractors.Feature import Feature
-from ogd.core.schemas.Event import Event, EventSource
-from ogd.core.schemas.ExtractionMode import ExtractionMode
-from ogd.core.schemas.FeatureData import FeatureData
+from ogd.core.models.Event import Event, EventSource
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
+from ogd.core.models.FeatureData import FeatureData
 
 class TotalExperimentationTime(Feature):
 
     def __init__(self, params:GeneratorParameters):
         super().__init__(params=params)
         self.prev_time = timedelta(0)
         self.total_time = timedelta(0)
```

### Comparing `opengamedata_core-0.0.5/src/ogd/games/AQUALAB/features/TotalGuideCount.py` & `opengamedata_core-0.0.6/src/ogd/games/AQUALAB/features/SessionGuideCount.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # import libraries
 from typing import Any, List
 # import locals
 from ogd.core.generators.Generator import GeneratorParameters
 from ogd.core.generators.extractors.Feature import Feature
-from ogd.core.schemas.Event import Event
-from ogd.core.schemas.ExtractionMode import ExtractionMode
-from ogd.core.schemas.FeatureData import FeatureData
+from ogd.core.models.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
+from ogd.core.models.FeatureData import FeatureData
 
-class TotalGuideCount(Feature):
+class SessionGuideCount(Feature):
 
     def __init__(self, params:GeneratorParameters):
         super().__init__(params=params)
         self._count = 0
 
     # *** IMPLEMENT ABSTRACT FUNCTIONS ***
     @classmethod
```

### Comparing `opengamedata_core-0.0.5/src/ogd/games/AQUALAB/features/TotalHelpCount.py` & `opengamedata_core-0.0.6/src/ogd/games/SHADOWSPECT/features/MoveShapeCount.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,26 @@
+# import libraries
 from typing import Any, List
 # import locals
-from ogd.core.generators.Generator import GeneratorParameters
 from ogd.core.generators.extractors.Feature import Feature
-from ogd.core.schemas.Event import Event
-from ogd.core.schemas.ExtractionMode import ExtractionMode
-from ogd.core.schemas.FeatureData import FeatureData
+from ogd.core.generators.Generator import GeneratorParameters
+from ogd.core.models.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
+from ogd.core.models.FeatureData import FeatureData
 
-class TotalHelpCount(Feature):
-    """_summary_
 
-    :param Feature: _description_
-    :type Feature: _type_
-    """
+class MoveShapeCount(Feature):
     def __init__(self, params:GeneratorParameters):
         super().__init__(params=params)
         self._count = 0
 
     # *** IMPLEMENT ABSTRACT FUNCTIONS ***
     @classmethod
     def _eventFilter(cls, mode:ExtractionMode) -> List[str]:
-        return ["ask_for_help"]
+        return ["move_shape"]
 
     @classmethod
     def _featureFilter(cls, mode:ExtractionMode) -> List[str]:
         return []
 
     def _updateFromEvent(self, event:Event) -> None:
         self._count += 1
```

### Comparing `opengamedata_core-0.0.5/src/ogd/games/AQUALAB/features/TotalKelpTime.py` & `opengamedata_core-0.0.6/src/ogd/games/AQUALAB/features/TotalKelpTime.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # import libraries
 from datetime import timedelta
 from typing import Any, List
 # import locals
 from ogd.core.generators.extractors.Extractor import GeneratorParameters
 from ogd.core.generators.extractors.Feature import Feature
-from ogd.core.schemas.Event import Event, EventSource
-from ogd.core.schemas.ExtractionMode import ExtractionMode
-from ogd.core.schemas.FeatureData import FeatureData
+from ogd.core.models.Event import Event, EventSource
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
+from ogd.core.models.FeatureData import FeatureData
 from ogd.core.utils.Logger import Logger
 from ogd.games.AQUALAB.features.PerJobFeature import PerJobFeature
 from ogd.core.generators.extractors.PerCountFeature import PerCountFeature
 
 class TotalKelpTime(Feature):
     def __init__(self, params:GeneratorParameters):
         super().__init__(params=params)
```

### Comparing `opengamedata_core-0.0.5/src/ogd/games/AQUALAB/features/TotalModelingTime.py` & `opengamedata_core-0.0.6/src/ogd/games/AQUALAB/features/TotalModelingTime.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # import libraries
 from datetime import timedelta
 from typing import Any, List
 # import locals
 from ogd.core.generators.extractors.Extractor import GeneratorParameters
 from ogd.core.generators.extractors.Feature import Feature
-from ogd.core.schemas.Event import Event, EventSource
-from ogd.core.schemas.ExtractionMode import ExtractionMode
-from ogd.core.schemas.FeatureData import FeatureData
+from ogd.core.models.Event import Event, EventSource
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
+from ogd.core.models.FeatureData import FeatureData
 
 class TotalModelingTime(Feature):
 
     def __init__(self, params:GeneratorParameters):
         super().__init__(params=params)
         self.prev_time = timedelta(0)
         self.total_time = timedelta(0)
```

### Comparing `opengamedata_core-0.0.5/src/ogd/games/AQUALAB/features/TotalPlayTime.py` & `opengamedata_core-0.0.6/src/ogd/games/AQUALAB/features/TotalPlayTime.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 from datetime import datetime, timedelta
 import logging, warnings
 from typing import Any, List, Optional
 # import locals
 from ogd.core.utils.Logger import Logger
 from ogd.core.generators.extractors.Extractor import GeneratorParameters
 from ogd.core.generators.extractors.Feature import Feature
-from ogd.core.schemas.Event import Event
-from ogd.core.schemas.ExtractionMode import ExtractionMode
-from ogd.core.schemas.FeatureData import FeatureData
+from ogd.core.models.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
+from ogd.core.models.FeatureData import FeatureData
 
 class TotalPlayTime(Feature):
     def __init__(self, params:GeneratorParameters, ):
         super().__init__(params=params)
         self._play_time: timedelta = timedelta(0)
         self._play_time_seconds: timedelta = timedelta(0)
         self._idle_time: timedelta = timedelta(0)
```

### Comparing `opengamedata_core-0.0.5/src/ogd/games/AQUALAB/features/UserAvgActiveTime.py` & `opengamedata_core-0.0.6/src/ogd/games/WAVES/features/MenuButtonCount.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,43 +1,35 @@
 # import libraries
-from datetime import timedelta
-from typing import Any, List
+from ogd.core.models import Event
+from typing import Any, List, Optional
 # import locals
+from ogd.core.generators.extractors.PerLevelFeature import PerLevelFeature
 from ogd.core.generators.Generator import GeneratorParameters
-from ogd.core.generators.extractors.SessionFeature import SessionFeature
-from ogd.core.schemas.Event import Event
-from ogd.core.schemas.ExtractionMode import ExtractionMode
-from ogd.core.schemas.FeatureData import FeatureData
-
-class UserAvgActiveTime(SessionFeature):
-
-    def __init__(self, params:GeneratorParameters, player_id:str):
-        self._player_id = player_id
-        super().__init__(params=params)
-        self._times : List[float] = []
+from ogd.core.models.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
+from ogd.core.models.FeatureData import FeatureData
+
+class MenuButtonCount(PerLevelFeature):
+    def __init__(self, params:GeneratorParameters):
+        PerLevelFeature.__init__(self, params=params)
+        self._menu_btn_count = 0
 
     # *** IMPLEMENT ABSTRACT FUNCTIONS ***
     @classmethod
     def _eventFilter(cls, mode:ExtractionMode) -> List[str]:
-        return []
+        return ["CUSTOM.5"]
+        # "events": ["MENU_BUTTON"],
 
     @classmethod
     def _featureFilter(cls, mode:ExtractionMode) -> List[str]:
-        return ["ActiveTime"]
+        return []
 
     def _updateFromEvent(self, event:Event) -> None:
-        return
+        self._menu_btn_count += 1
 
     def _updateFromFeatureData(self, feature:FeatureData):
-        if feature.PlayerID == self._player_id:
-            if feature.FeatureValues[0] == "No events":
-                pass
-            else:
-                self._times.append(feature.FeatureValues[0]/timedelta(seconds=1))
+        return
 
     def _getFeatureValues(self) -> List[Any]:
-        if len(self._times) > 0:
-            return [sum(self._times) / len(self._times)]
-        else:
-            return [0]
+        return [self._menu_btn_count]
 
     # *** Optionally override public functions. ***
```

### Comparing `opengamedata_core-0.0.5/src/ogd/games/AQUALAB/features/UserAvgSessionDuration.py` & `opengamedata_core-0.0.6/src/ogd/games/SHIPWRECKS/features/SessionID.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,42 +1,34 @@
 # import libraries
-from typing import Any, List
+from typing import Any, List, Optional
 # import locals
-from ogd.core.generators.Generator import GeneratorParameters
 from ogd.core.generators.extractors.SessionFeature import SessionFeature
-from ogd.core.schemas.Event import Event
-from ogd.core.schemas.ExtractionMode import ExtractionMode
-from ogd.core.schemas.FeatureData import FeatureData
+from ogd.core.generators.Generator import GeneratorParameters
+from ogd.core.models.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
+from ogd.core.models.FeatureData import FeatureData
 
-class UserAvgSessionDuration(SessionFeature):
+class SessionID(SessionFeature):
 
-    def __init__(self, params:GeneratorParameters, player_id:str):
-        self._player_id = player_id
+    def __init__(self, params:GeneratorParameters, session_id:str):
+        self._session_id = session_id
         super().__init__(params=params)
-        self._times : List[int] = []
 
     # *** IMPLEMENT ABSTRACT FUNCTIONS ***
     @classmethod
     def _eventFilter(cls, mode:ExtractionMode) -> List[str]:
         return []
 
     @classmethod
     def _featureFilter(cls, mode:ExtractionMode) -> List[str]:
-        return ["SessionDuration"]
+        return []
 
     def _updateFromEvent(self, event:Event) -> None:
         return
 
     def _updateFromFeatureData(self, feature:FeatureData):
-        if feature.PlayerID == self._player_id:
-            if feature.FeatureValues[0] == "No events":
-                pass
-            else:
-                self._times.append(feature.FeatureValues[0].total_seconds())
+        return
 
     def _getFeatureValues(self) -> List[Any]:
-        if len(self._times) > 0:
-            return [sum(self._times) / len(self._times)]
-        else:
-            return [0]
+        return [self._session_id]
 
-    # *** Optionally override public functions. ***
+    # *** Optionally override public functions. ***
```

### Comparing `opengamedata_core-0.0.5/src/ogd/games/AQUALAB/features/UserTotalSessionDuration.py` & `opengamedata_core-0.0.6/src/ogd/games/AQUALAB/features/UserTotalSessionDuration.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from datetime import timedelta
 from typing import Any, List
 
 from ogd.core.generators.Generator import GeneratorParameters
 from ogd.core.generators.extractors.SessionFeature import SessionFeature
-from ogd.core.schemas.Event import Event
-from ogd.core.schemas.ExtractionMode import ExtractionMode
-from ogd.core.schemas.FeatureData import FeatureData
+from ogd.core.models.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
+from ogd.core.models.FeatureData import FeatureData
 
 class UserTotalSessionDuration(SessionFeature):
     """_summary_
 
     :param SessionFeature: _description_
     :type SessionFeature: _type_
     """
```

### Comparing `opengamedata_core-0.0.5/src/ogd/games/AQUALAB/features/__init__.py` & `opengamedata_core-0.0.6/src/ogd/games/AQUALAB/features/__init__.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.5/src/ogd/games/AQUALAB/schemas/AQUALAB.json.template` & `opengamedata_core-0.0.6/src/ogd/games/AQUALAB/schemas/AQUALAB.json.template`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.5/src/ogd/games/BLOOM/schemas/BLOOM.json.template` & `opengamedata_core-0.0.6/src/ogd/games/BLOOM/schemas/BLOOM.json.template`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.5/src/ogd/games/CENSIO_SLIDE/schemas/CENSIO_SLIDE.json.template` & `opengamedata_core-0.0.6/src/ogd/games/CENSIO_SLIDE/schemas/CENSIO_SLIDE.json.template`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.5/src/ogd/games/CENSIO_STACK/schemas/CENSIO_STACK.json.template` & `opengamedata_core-0.0.6/src/ogd/games/CENSIO_STACK/schemas/CENSIO_STACK.json.template`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.5/src/ogd/games/CRUSH_STATION/schemas/CRUSH_STATION.json.template` & `opengamedata_core-0.0.6/src/ogd/games/CRUSH_STATION/schemas/CRUSH_STATION.json.template`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.5/src/ogd/games/CRYSTAL/CrystalLoader.py` & `opengamedata_core-0.0.6/src/ogd/games/CRYSTAL/CrystalLoader.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 ## import local files
 import ogd.games.CRYSTAL.features
 from ogd.core.generators.detectors.Detector import Detector
 from ogd.core.generators.Generator import GeneratorParameters
 from ogd.core.generators.extractors.Feature import Feature
 from ogd.core.generators.legacy.LegacyLoader import LegacyLoader
 from ogd.games.CRYSTAL.features.CrystalExtractor import CrystalExtractor
-from ogd.core.schemas.Event import Event
-from ogd.core.schemas.ExtractionMode import ExtractionMode
+from ogd.core.models.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
 from ogd.core.schemas.games.GameSchema import GameSchema
 
 class CrystalLoader(LegacyLoader):
 
     # *** IMPLEMENT ABSTRACT FUNCTIONS ***
 
     @staticmethod
```

### Comparing `opengamedata_core-0.0.5/src/ogd/games/CRYSTAL/features/CrystalExtractor.py` & `opengamedata_core-0.0.6/src/ogd/games/CRYSTAL/features/CrystalExtractor.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 import typing
 from datetime import datetime
 from typing import Any, Dict, List, Optional
 ## import local files
 from ogd.core.utils.Logger import Logger
 from ogd.core.generators.Generator import GeneratorParameters
 from ogd.core.generators.legacy.LegacyFeature import LegacyFeature
-from ogd.core.schemas.Event import Event
-from ogd.core.schemas.ExtractionMode import ExtractionMode
+from ogd.core.models.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
 from ogd.core.schemas.games.GameSchema import GameSchema
 
 # temp comment
 
 ## @class CrystalExtractor
 #  Extractor subclass for extracting features from Crystal game data.
 class CrystalExtractor(LegacyFeature):
```

### Comparing `opengamedata_core-0.0.5/src/ogd/games/CRYSTAL/schemas/CRYSTAL.json.template` & `opengamedata_core-0.0.6/src/ogd/games/CRYSTAL/schemas/CRYSTAL.json.template`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.5/src/ogd/games/GWAKKAMOLE/schemas/GWAKKAMOLE.json.template` & `opengamedata_core-0.0.6/src/ogd/games/GWAKKAMOLE/schemas/GWAKKAMOLE.json.template`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.5/src/ogd/games/ICECUBE/DBExport.json` & `opengamedata_core-0.0.6/src/ogd/games/ICECUBE/DBExport.json`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.5/src/ogd/games/ICECUBE/DBExport.py` & `opengamedata_core-0.0.6/src/ogd/games/ICECUBE/DBExport.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.5/src/ogd/games/ICECUBE/IcecubeLoader.py` & `opengamedata_core-0.0.6/src/ogd/games/ICECUBE/IcecubeLoader.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 from . import features
 from ogd.core.generators.detectors.Detector import Detector
 from ogd.core.generators.Generator import GeneratorParameters
 from ogd.core.generators.GeneratorLoader import GeneratorLoader
 from ogd.core.generators.extractors.Feature import Feature
 from ogd.games.ICECUBE.features import *
 from ogd.core.generators.Generator import GeneratorParameters
-from ogd.core.schemas.Event import Event
-from ogd.core.schemas.ExtractionMode import ExtractionMode
+from ogd.core.models.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
 from ogd.core.schemas.games.GameSchema import GameSchema
 # from ogd.games.ICECUBE.DBExport import scene_map
 
 ## @class WaveExtractor
 #  Extractor subclass for extracting features from Waves game data.
 
 EXPORT_PATH : Final[str] = "games/ICECUBE/DBExport.json"
```

### Comparing `opengamedata_core-0.0.5/src/ogd/games/ICECUBE/features/HeadsetOnCount.py` & `opengamedata_core-0.0.6/src/ogd/games/PENGUINS/features/RockPickupCount.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,40 +1,37 @@
 # import libraries
 import logging
 from typing import Any, Dict, List, Optional
 # import locals
 from ogd.core.utils.Logger import Logger
 from ogd.core.generators.Generator import GeneratorParameters
-from ogd.core.generators.extractors.Feature import Feature
+from ogd.core.models.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
+from ogd.core.models.FeatureData import FeatureData
 from ogd.core.generators.extractors.SessionFeature import SessionFeature
-from ogd.core.schemas.Event import Event
-from ogd.core.schemas.ExtractionMode import ExtractionMode
-from ogd.core.schemas.FeatureData import FeatureData
 
-class HeadsetOnCount(SessionFeature):
+
+class RockPickupCount(SessionFeature):
 
     def __init__(self, params:GeneratorParameters):
         super().__init__(params=params)
-        self._headset_count : int = 0
+        self._current_count : int = 0
 
     # *** IMPLEMENT ABSTRACT FUNCTIONS ***
     @classmethod
     def _eventFilter(cls, mode:ExtractionMode) -> List[str]:
-        return ["headset_on"]
+        return ["pickup_rock"]
 
     @classmethod
     def _featureFilter(cls, mode:ExtractionMode) -> List[str]:
         return []
 
     def _updateFromEvent(self, event:Event) -> None:
-        self._headset_count += 1
+        self._current_count += 1
 
     def _updateFromFeatureData(self, feature:FeatureData):
         return
 
     def _getFeatureValues(self) -> List[Any]:
-        return [self._headset_count]
+        return [self._current_count]
 
-    # *** Optionally override public functions. ***
-    @staticmethod
-    def MinVersion() -> Optional[str]:
-        return "2"
+
```

### Comparing `opengamedata_core-0.0.5/src/ogd/games/ICECUBE/features/ObjectSelectionsDuringVoiceover.py` & `opengamedata_core-0.0.6/src/ogd/games/ICECUBE/features/ObjectSelectionsDuringVoiceover.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 import logging
 from typing import Any, Dict, List, Optional
 # import locals
 from ogd.core.utils.Logger import Logger
 from ogd.core.generators.Generator import GeneratorParameters
 from ogd.core.generators.extractors.Feature import Feature
 from ogd.core.generators.extractors.SessionFeature import SessionFeature
-from ogd.core.schemas.Event import Event
-from ogd.core.schemas.ExtractionMode import ExtractionMode
-from ogd.core.schemas.FeatureData import FeatureData
+from ogd.core.models.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
+from ogd.core.models.FeatureData import FeatureData
 # count of object_selected 
 # between script_audio_started and script_audio_complete
 # return the # of object_selected during audio playing
 class ObjectSelectionsDuringVoiceover (SessionFeature):
 
     def __init__(self, params:GeneratorParameters):
         super().__init__(params=params)
```

### Comparing `opengamedata_core-0.0.5/src/ogd/games/ICECUBE/features/PerSceneFeature.py` & `opengamedata_core-0.0.6/src/ogd/games/ICECUBE/features/PerSceneFeature.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # import locals
 from ogd.core.generators.Generator import GeneratorParameters
 from ogd.core.generators.extractors.PerCountFeature import PerCountFeature
-from ogd.core.schemas.Event import Event
-from ogd.core.schemas.ExtractionMode import ExtractionMode
+from ogd.core.models.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
 from ogd.games.ICECUBE.DBExport import scenes_list
 ## @class PerLevelFeature
 class PerSceneFeature(PerCountFeature):
     """PerLevelFeature
     Abstract base class for per-level game features.
     Works like a normal Feature, but checks if the given event has right "level"
     before attempting to extract from event.
```

### Comparing `opengamedata_core-0.0.5/src/ogd/games/ICECUBE/features/SceneDuration.py` & `opengamedata_core-0.0.6/src/ogd/games/ICECUBE/features/SceneDuration.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # import libraries
 import json
 from typing import Any, List, Optional
 # import local files
 from ogd.core.generators.Generator import GeneratorParameters
 from ogd.core.generators.extractors.PerCountFeature import PerCountFeature
-from ogd.core.schemas.Event import Event
-from ogd.core.schemas.ExtractionMode import ExtractionMode
-from ogd.core.schemas.FeatureData import FeatureData
+from ogd.core.models.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
+from ogd.core.models.FeatureData import FeatureData
 from ogd.games.ICECUBE.DBExport import scene_map
 from ogd.games.ICECUBE.features.PerSceneFeature import PerSceneFeature
 from ogd.games.ICECUBE.DBExport import scenes_list
 from ogd.core.utils.Logger import Logger
 from datetime import timedelta
 
 # import libraries
```

### Comparing `opengamedata_core-0.0.5/src/ogd/games/ICECUBE/features/SceneFailureCount.py` & `opengamedata_core-0.0.6/src/ogd/games/ICECUBE/features/SceneFailureCount.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 import logging
 from typing import Any, Dict, List, Optional
 # import locals
 from ogd.core.utils.Logger import Logger
 from ogd.core.generators.Generator import GeneratorParameters
 from ogd.core.generators.extractors.Feature import Feature
 from ogd.core.generators.extractors.SessionFeature import SessionFeature
-from ogd.core.schemas.Event import Event
-from ogd.core.schemas.ExtractionMode import ExtractionMode
-from ogd.core.schemas.FeatureData import FeatureData
+from ogd.core.models.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
+from ogd.core.models.FeatureData import FeatureData
 scenes_map = {"ICE":0, "VOYAGER":0, "NOTHING":0, "EXTREME":0, "EARTH":0, "CREDITS":0}
 
 class SceneFailureCount(SessionFeature):
 
     def __init__(self, params:GeneratorParameters):
         super().__init__(params=params)
         self._failure_count : int = 0
```

### Comparing `opengamedata_core-0.0.5/src/ogd/games/ICECUBE/features/SceneFailures.py` & `opengamedata_core-0.0.6/src/ogd/games/ICECUBE/features/SceneFailures.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # import libraries
 import json
 from typing import Any, List, Optional
 # import local files
 from ogd.core.generators.Generator import GeneratorParameters
 from ogd.core.generators.extractors.PerCountFeature import PerCountFeature
-from ogd.core.schemas.Event import Event
-from ogd.core.schemas.ExtractionMode import ExtractionMode
-from ogd.core.schemas.FeatureData import FeatureData
+from ogd.core.models.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
+from ogd.core.models.FeatureData import FeatureData
 from ogd.games.ICECUBE.DBExport import scene_map
 from ogd.games.ICECUBE.features.PerSceneFeature import PerSceneFeature
 from ogd.games.ICECUBE.DBExport import scenes_list
 from ogd.core.utils.Logger import Logger
 
 # import libraries
 import logging
```

### Comparing `opengamedata_core-0.0.5/src/ogd/games/ICECUBE/features/ScenesEncountered.py` & `opengamedata_core-0.0.6/src/ogd/games/PENGUINS/features/RegionsEncountered.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,41 +2,38 @@
 import logging
 from typing import Any, Dict, List, Optional
 # import locals
 from ogd.core.utils.Logger import Logger
 from ogd.core.generators.Generator import GeneratorParameters
 from ogd.core.generators.extractors.Feature import Feature
 from ogd.core.generators.extractors.SessionFeature import SessionFeature
-from ogd.core.schemas.Event import Event
-from ogd.core.schemas.ExtractionMode import ExtractionMode
-from ogd.core.schemas.FeatureData import FeatureData
+from ogd.core.models.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
+from ogd.core.models.FeatureData import FeatureData
 
-class ScenesEncountered(SessionFeature):
+class RegionsEncountered(SessionFeature):
 
     def __init__(self, params:GeneratorParameters):
         super().__init__(params=params)
-        self._scene_name = None
+        #self._scene_name = None
         self._cnt_list = list()
 
     # *** IMPLEMENT ABSTRACT FUNCTIONS ***
     @classmethod
     def _eventFilter(cls, mode:ExtractionMode) -> List[str]:
-        return ["scene_change"]
+        return ["region_enter"]
 
     @classmethod
     def _featureFilter(cls, mode:ExtractionMode) -> List[str]:
         return []
 
     def _updateFromEvent(self, event:Event) -> None:
-        self._scene_name = event.EventData.get("scene_name")
-        self._cnt_list.append(self._scene_name)
+        self._object_id = event.event_data.get("region")
+        self._cnt_list.append(self._object_id)
 
     def _updateFromFeatureData(self, feature:FeatureData):
         return
 
     def _getFeatureValues(self) -> List[Any]:
         return [self._cnt_list]
 
     # *** Optionally override public functions. ***
-    @staticmethod
-    def MinVersion() -> Optional[str]:
-        return "2"
```

### Comparing `opengamedata_core-0.0.5/src/ogd/games/ICECUBE/features/SessionDuration.py` & `opengamedata_core-0.0.6/src/ogd/games/ICECUBE/features/SessionDuration.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 # import libraries
 import logging
 from typing import Any, List
 # import locals
 from ogd.core.generators.Generator import GeneratorParameters
 from ogd.core.generators.extractors.SessionFeature import SessionFeature
-from ogd.core.schemas.Event import Event
-from ogd.core.schemas.ExtractionMode import ExtractionMode
-from ogd.core.schemas.FeatureData import FeatureData
+from ogd.core.models.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
+from ogd.core.models.FeatureData import FeatureData
 from ogd.core.utils.Logger import Logger
 
 # import libraries
 import logging
 from typing import Any, List, Optional
 from datetime import datetime, timedelta
 # import locals
 from ogd.core.generators.Generator import GeneratorParameters
 from ogd.core.generators.extractors.SessionFeature import SessionFeature
-from ogd.core.schemas.Event import Event
-from ogd.core.schemas.ExtractionMode import ExtractionMode
-from ogd.core.schemas.FeatureData import FeatureData
+from ogd.core.models.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
+from ogd.core.models.FeatureData import FeatureData
 from ogd.core.utils.Logger import Logger
 
 class SessionDuration(SessionFeature):
     """Template file to serve as a guide for creating custom Feature subclasses for games.
 
     :param Feature: Base class for a Custom Feature class.
     :type Feature: _type_
```

### Comparing `opengamedata_core-0.0.5/src/ogd/games/ICECUBE/features/Session_Language.py` & `opengamedata_core-0.0.6/src/ogd/games/ICECUBE/features/Session_Language.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import Any, List
 
 from typing import Any, Dict, List, Optional
 from ogd.core.generators.Generator import GeneratorParameters
 from ogd.core.generators.extractors.SessionFeature import SessionFeature
-from ogd.core.schemas.Event import Event
-from ogd.core.schemas.ExtractionMode import ExtractionMode
-from ogd.core.schemas.FeatureData import FeatureData
+from ogd.core.models.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
+from ogd.core.models.FeatureData import FeatureData
 
 class Session_Language(SessionFeature):
     """_summary_
 
     :param SessionFeature: _description_
     :type SessionFeature: _type_
     """
```

### Comparing `opengamedata_core-0.0.5/src/ogd/games/ICECUBE/features/TaskTimeToComplete.py` & `opengamedata_core-0.0.6/src/ogd/games/ICECUBE/features/TaskTimeToComplete.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 from typing import Any, Dict, List, Optional
 # import locals
 from datetime import datetime, timedelta
 from ogd.core.utils.Logger import Logger
 from ogd.core.generators.Generator import GeneratorParameters
 from ogd.core.generators.extractors.Feature import Feature
 from ogd.core.generators.extractors.SessionFeature import SessionFeature
-from ogd.core.schemas.Event import Event
-from ogd.core.schemas.ExtractionMode import ExtractionMode
-from ogd.core.schemas.FeatureData import FeatureData
+from ogd.core.models.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
+from ogd.core.models.FeatureData import FeatureData
 scenes_map = {"ICE":0, "VOYAGER":0, "NOTHING":0, "EXTREME":0, "EARTH":0, "CREDITS":0}
 
 class TaskTimeToComplete(SessionFeature):
     
     def __init__(self, params:GeneratorParameters):
         super().__init__(params=params)
         self._session_id = None
```

### Comparing `opengamedata_core-0.0.5/src/ogd/games/ICECUBE/features/ViewportCountPerScene.py` & `opengamedata_core-0.0.6/src/ogd/games/ICECUBE/features/ViewportCountPerScene.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 import logging
 from typing import Any, Dict, List, Optional
 # import locals
 from ogd.core.utils.Logger import Logger
 from ogd.core.generators.Generator import GeneratorParameters
 from ogd.core.generators.extractors.Feature import Feature
 from ogd.core.generators.extractors.SessionFeature import SessionFeature
-from ogd.core.schemas.Event import Event
-from ogd.core.schemas.ExtractionMode import ExtractionMode
-from ogd.core.schemas.FeatureData import FeatureData
+from ogd.core.models.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
+from ogd.core.models.FeatureData import FeatureData
 scenes_map = {"ICE":0, "VOYAGER":0, "NOTHING":0, "EXTREME":0, "EARTH":0, "CREDITS":0}
 
 class ViewportCountPerScene(SessionFeature):
 
     def __init__(self, params:GeneratorParameters):
         super().__init__(params=params)
         self._failure_count : int = 0
```

### Comparing `opengamedata_core-0.0.5/src/ogd/games/ICECUBE/features/__init__.py` & `opengamedata_core-0.0.6/src/ogd/games/ICECUBE/features/__init__.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.5/src/ogd/games/ICECUBE/schemas/ICECUBE.json.template` & `opengamedata_core-0.0.6/src/ogd/games/ICECUBE/schemas/ICECUBE.json.template`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.5/src/ogd/games/JOURNALISM/JournalismLoader.py` & `opengamedata_core-0.0.6/src/ogd/games/JOURNALISM/JournalismLoader.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 from . import features
 from ogd.games.JOURNALISM.features import *
 from ogd.core.generators.detectors.Detector import Detector
 from ogd.core.generators.Generator import GeneratorParameters
 from ogd.core.generators.extractors.Feature import Feature
 from ogd.core.generators.GeneratorLoader import GeneratorLoader
 from ogd.games.JOURNALISM.features import StoryScoreSequence
-from ogd.core.schemas.Event import Event
-from ogd.core.schemas.ExtractionMode import ExtractionMode
+from ogd.core.models.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
 from ogd.core.schemas.games.GameSchema import GameSchema
 
 
 
 class JournalismLoader(GeneratorLoader):
 
     # *** IMPLEMENT ABSTRACT FUNCTIONS ***
```

### Comparing `opengamedata_core-0.0.5/src/ogd/games/JOURNALISM/features/AttributeView.py` & `opengamedata_core-0.0.6/src/ogd/games/JOURNALISM/features/AttributeView.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # import libraries
 import json
 from typing import Any, List, Optional
 # import local files
 from ogd.core.generators.extractors.Feature import Feature
 from ogd.core.generators.extractors.PerLevelFeature import PerLevelFeature
-from ogd.core.schemas.Event import Event
-from ogd.core.schemas.ExtractionMode import ExtractionMode
-from ogd.core.schemas.FeatureData import FeatureData
+from ogd.core.models.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
+from ogd.core.models.FeatureData import FeatureData
 from ogd.core.generators.Generator import GeneratorParameters
 from ogd.core.generators.extractors.SessionFeature import SessionFeature
 
 
 
 
 class AttributeView(PerLevelFeature):
```

### Comparing `opengamedata_core-0.0.5/src/ogd/games/JOURNALISM/features/ChoiceClickCount.py` & `opengamedata_core-0.0.6/src/ogd/games/JOURNALISM/features/ChoiceClickCount.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # import libraries
 import json
 from typing import Any, List, Optional
 # import local files
 from ogd.core.generators.extractors.Feature import Feature
-from ogd.core.schemas.Event import Event
-from ogd.core.schemas.ExtractionMode import ExtractionMode
-from ogd.core.schemas.FeatureData import FeatureData
+from ogd.core.models.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
+from ogd.core.models.FeatureData import FeatureData
 from ogd.core.generators.Generator import GeneratorParameters
 from ogd.core.generators.extractors.SessionFeature import SessionFeature
 
 
 
 
 class ChoiceClickCount(SessionFeature):
```

### Comparing `opengamedata_core-0.0.5/src/ogd/games/JOURNALISM/features/ContinuesOnFail.py` & `opengamedata_core-0.0.6/src/ogd/games/JOURNALISM/features/ContinuesOnFail.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 # import libraries
 from os import truncate
 from ogd.core.generators.extractors.PerCountFeature import PerCountFeature
 from ogd.core.generators.extractors.SessionFeature import SessionFeature
-from ogd.core.schemas import Event
+from ogd.core.models import Event
 from typing import Any, List, Optional
 # import locals
 from ogd.core.generators.extractors.PerLevelFeature import PerLevelFeature
 from ogd.core.generators.Generator import GeneratorParameters
-from ogd.core.schemas.Event import Event
-from ogd.core.schemas.ExtractionMode import ExtractionMode
-from ogd.core.schemas.FeatureData import FeatureData
+from ogd.core.models.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
+from ogd.core.models.FeatureData import FeatureData
 
 class ContinuesOnFail(SessionFeature):
     def __init__(self, params:GeneratorParameters):
         super().__init__(params=params)
         self._quit_type : Optional[bool] = None
         self._total_fails : Optional[int] = None
```

### Comparing `opengamedata_core-0.0.5/src/ogd/games/JOURNALISM/features/EditorNoteOpen.py` & `opengamedata_core-0.0.6/src/ogd/games/JOURNALISM/features/EditorNoteOpen.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # import libraries
 import json
 from typing import Any, List, Optional
 # import local files
 from ogd.core.generators.extractors.Feature import Feature
 from ogd.core.generators.extractors.PerLevelFeature import PerLevelFeature
-from ogd.core.schemas.Event import Event
-from ogd.core.schemas.ExtractionMode import ExtractionMode
-from ogd.core.schemas.FeatureData import FeatureData
+from ogd.core.models.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
+from ogd.core.models.FeatureData import FeatureData
 from ogd.core.generators.Generator import GeneratorParameters
 from ogd.core.generators.extractors.SessionFeature import SessionFeature
 
 
 
 
 class EditorNoteOpen(PerLevelFeature):
```

### Comparing `opengamedata_core-0.0.5/src/ogd/games/JOURNALISM/features/FailureCount.py` & `opengamedata_core-0.0.6/src/ogd/games/JOURNALISM/features/FailureCount.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # import libraries
 import json
 from typing import Any, List, Optional
 # import local files
 from ogd.core.generators.extractors.Feature import Feature
 from ogd.core.generators.extractors.PerLevelFeature import PerLevelFeature
-from ogd.core.schemas.Event import Event
-from ogd.core.schemas.ExtractionMode import ExtractionMode
-from ogd.core.schemas.FeatureData import FeatureData
+from ogd.core.models.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
+from ogd.core.models.FeatureData import FeatureData
 from ogd.core.generators.Generator import GeneratorParameters
 from ogd.core.generators.extractors.SessionFeature import SessionFeature
 
 
 
 
 class FailureCount(PerLevelFeature):
```

### Comparing `opengamedata_core-0.0.5/src/ogd/games/JOURNALISM/features/GameComplete.py` & `opengamedata_core-0.0.6/src/ogd/games/JOURNALISM/features/GameComplete.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 import json
 from typing import Any, List, Optional
 import json
 from time import time
 from datetime  import timedelta, datetime
 # import local files
 from ogd.core.generators.extractors.Feature import Feature
-from ogd.core.schemas.Event import Event
-from ogd.core.schemas.ExtractionMode import ExtractionMode
-from ogd.core.schemas.FeatureData import FeatureData
+from ogd.core.models.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
+from ogd.core.models.FeatureData import FeatureData
 from ogd.core.generators.Generator import GeneratorParameters
 from ogd.core.generators.extractors.SessionFeature import SessionFeature
```

### Comparing `opengamedata_core-0.0.5/src/ogd/games/JOURNALISM/features/LevelCompleteCount.py` & `opengamedata_core-0.0.6/src/ogd/games/JOURNALISM/features/LevelCompleteCount.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # import libraries
 import json
 from typing import Any, List, Optional
 # import local files
 from ogd.core.generators.extractors.Feature import Feature
 from ogd.core.generators.extractors.PerLevelFeature import PerLevelFeature
-from ogd.core.schemas.Event import Event
-from ogd.core.schemas.ExtractionMode import ExtractionMode
-from ogd.core.schemas.FeatureData import FeatureData
+from ogd.core.models.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
+from ogd.core.models.FeatureData import FeatureData
 from ogd.core.generators.Generator import GeneratorParameters
 from ogd.core.generators.extractors.SessionFeature import SessionFeature
 
 
 
 
 class LevelCompleteCount(PerLevelFeature):
```

### Comparing `opengamedata_core-0.0.5/src/ogd/games/JOURNALISM/features/LevelCompleted.py` & `opengamedata_core-0.0.6/src/ogd/games/JOURNALISM/features/LevelCompleted.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # import libraries
 import json
 from typing import Any, List, Optional
 # import local files
 from ogd.core.generators.extractors.Feature import Feature
 from ogd.core.generators.extractors.PerLevelFeature import PerLevelFeature
-from ogd.core.schemas.Event import Event
-from ogd.core.schemas.ExtractionMode import ExtractionMode
-from ogd.core.schemas.FeatureData import FeatureData
+from ogd.core.models.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
+from ogd.core.models.FeatureData import FeatureData
 from ogd.core.generators.Generator import GeneratorParameters
 from ogd.core.generators.extractors.SessionFeature import SessionFeature
 
 
 
 
 class LevelCompleted(PerLevelFeature):
```

### Comparing `opengamedata_core-0.0.5/src/ogd/games/JOURNALISM/features/LevelTime.py` & `opengamedata_core-0.0.6/src/ogd/games/JOURNALISM/features/LevelTime.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import logging
 from datetime import datetime, timedelta
 from ogd.games.JOURNALISM.features import PlayTime
-from ogd.core.schemas import Event
+from ogd.core.models import Event
 from typing import Any, Final, List, Optional
 # import locals
 from ogd.core.utils.Logger import Logger
 from ogd.core.generators.extractors.PerLevelFeature import PerLevelFeature
 from ogd.core.generators.Generator import GeneratorParameters
-from ogd.core.schemas.Event import Event
-from ogd.core.schemas.ExtractionMode import ExtractionMode
-from ogd.core.schemas.FeatureData import FeatureData
+from ogd.core.models.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
+from ogd.core.models.FeatureData import FeatureData
 
 class LevelTime(PerLevelFeature):
     def __init__(self, params:GeneratorParameters):
         PerLevelFeature.__init__(self, params=params)
         self._begin_times    : List[datetime] = []
         self._complete_times : List[datetime] = []
         self._idle_time  : Optional[timedelta] = None
```

### Comparing `opengamedata_core-0.0.5/src/ogd/games/JOURNALISM/features/MaxedPlayerAttribute.py` & `opengamedata_core-0.0.6/src/ogd/games/JOURNALISM/features/WorstPlayerAttribute.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 # import libraries
 from os import truncate
 from ogd.core.generators.extractors.PerCountFeature import PerCountFeature
-from ogd.core.schemas import Event
+from ogd.core.models import Event
 from typing import Any, Final, List, Optional
 # import locals
 from ogd.core.generators.extractors.PerLevelFeature import PerLevelFeature
 from ogd.core.generators.Generator import GeneratorParameters
-from ogd.core.schemas.Event import Event
-from ogd.core.schemas.ExtractionMode import ExtractionMode
-from ogd.core.schemas.FeatureData import FeatureData
+from ogd.core.models.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
+from ogd.core.models.FeatureData import FeatureData
 
-class MaxedPlayerAttribute(PerCountFeature):
+class WorstPlayerAttribute(PerCountFeature):
     def __init__(self, params:GeneratorParameters):
         PerCountFeature.__init__(self, params=params)
-        self._attr_count     : int              = 0
+        self._attr_count = 0
         self._ATTRIBUTE_ENUM : Final[List[str]] = ["endurance", "resourceful", "tech","social","trust","research"]
-        self._attr_name      : str              = self._ATTRIBUTE_ENUM[self.CountIndex]
+        self._attr_name = self._ATTRIBUTE_ENUM[self.CountIndex]
 
 
     # *** IMPLEMENT ABSTRACT FUNCTIONS ***
     def _validateEventCountIndex(self, event:Event):
         
         return False
         #return int(event.GameState['att']) == self.CountIndex
@@ -28,33 +28,29 @@
 
     @classmethod
     def _eventFilter(cls, mode:ExtractionMode) -> List[str]:
         return [""]
 
     @classmethod
     def _featureFilter(cls, mode:ExtractionMode) -> List[str]:
-        return ["TopAttribute"]
+        return ["WorstAttribute"]
 
     def _updateFromEvent(self, event:Event) -> None:
         #self._story_alignment = event.EventData["story_alignment"]
 
         pass
 
 
     def _updateFromFeatureData(self, feature:FeatureData):
         #add logic to make sure that MODE is session, not player so we don't get duplicates
         if(feature._mode == ExtractionMode.SESSION):
             attribute_list = feature._vals[1]
             for attr in attribute_list:
                 if(self._ATTRIBUTE_ENUM.index(attr) == self.CountIndex):
-                    if(feature._vals[0]>=10):
-                        self._attr_count+=1
-
-
-
+                    self._attr_count+=1
             
         return
 
     def _getFeatureValues(self) -> List[Any]:
         return [self._attr_name, self._attr_count]
 
     # *** Optionally override public functions. ***
```

### Comparing `opengamedata_core-0.0.5/src/ogd/games/JOURNALISM/features/MeanSnippetTime.py` & `opengamedata_core-0.0.6/src/ogd/games/JOURNALISM/features/MeanSnippetTime.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # import libraries
 import json
 from typing import Any, List, Optional
 # import local files
 from ogd.core.generators.extractors.Feature import Feature
-from ogd.core.schemas.Event import Event
-from ogd.core.schemas.ExtractionMode import ExtractionMode
-from ogd.core.schemas.FeatureData import FeatureData
+from ogd.core.models.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
+from ogd.core.models.FeatureData import FeatureData
 from ogd.core.generators.Generator import GeneratorParameters
 from ogd.core.generators.extractors.SessionFeature import SessionFeature
 from time import time
 from datetime  import timedelta, datetime
```

### Comparing `opengamedata_core-0.0.5/src/ogd/games/JOURNALISM/features/PlayTime.py` & `opengamedata_core-0.0.6/src/ogd/games/JOURNALISM/features/PlayTime.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # import libraries
 import json
 from typing import Any, Final, List, Optional
 import json
 from datetime  import timedelta, datetime
 # import local files
-from ogd.core.schemas.Event import Event
-from ogd.core.schemas.ExtractionMode import ExtractionMode
-from ogd.core.schemas.FeatureData import FeatureData
+from ogd.core.models.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
+from ogd.core.models.FeatureData import FeatureData
 from ogd.core.generators.Generator import GeneratorParameters
 from ogd.core.generators.extractors.SessionFeature import SessionFeature
```

### Comparing `opengamedata_core-0.0.5/src/ogd/games/JOURNALISM/features/PlayerAttributes.py` & `opengamedata_core-0.0.6/src/ogd/games/JOURNALISM/features/PlayerAttributes.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # import libraries
 import json
 from typing import Any, List, Optional
 # import local files
 from ogd.core.generators.extractors.Feature import Feature
-from ogd.core.schemas.Event import Event
-from ogd.core.schemas.ExtractionMode import ExtractionMode
-from ogd.core.schemas.FeatureData import FeatureData
+from ogd.core.models.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
+from ogd.core.models.FeatureData import FeatureData
 from ogd.core.generators.Generator import GeneratorParameters
 from ogd.core.generators.extractors.SessionFeature import SessionFeature
 
 
 
 
 class PlayerAttributes(SessionFeature):
```

### Comparing `opengamedata_core-0.0.5/src/ogd/games/JOURNALISM/features/QuitLevel.py` & `opengamedata_core-0.0.6/src/ogd/games/JOURNALISM/features/QuitLevel.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 import json
 from typing import Any, List, Optional
 import json
 from time import time
 from datetime  import timedelta, datetime
 # import local files
 from ogd.core.generators.extractors.Feature import Feature
-from ogd.core.schemas.Event import Event
-from ogd.core.schemas.ExtractionMode import ExtractionMode
-from ogd.core.schemas.FeatureData import FeatureData
+from ogd.core.models.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
+from ogd.core.models.FeatureData import FeatureData
 from ogd.core.generators.Generator import GeneratorParameters
 from ogd.core.generators.extractors.SessionFeature import SessionFeature
```

### Comparing `opengamedata_core-0.0.5/src/ogd/games/JOURNALISM/features/QuitNode.py` & `opengamedata_core-0.0.6/src/ogd/games/JOURNALISM/features/QuitNode.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 import operator
 import logging
 from collections import Counter
 from typing import Any, Final, List, Optional
 # import local files
 from ogd.core.generators.extractors.Feature import Feature
 from ogd.core.generators.extractors.PerLevelFeature import PerLevelFeature
-from ogd.core.schemas.Event import Event
-from ogd.core.schemas.ExtractionMode import ExtractionMode
-from ogd.core.schemas.FeatureData import FeatureData
+from ogd.core.models.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
+from ogd.core.models.FeatureData import FeatureData
 from ogd.core.generators.Generator import GeneratorParameters
 from ogd.core.generators.extractors.SessionFeature import SessionFeature
 from ogd.core.utils.Logger import Logger
```

### Comparing `opengamedata_core-0.0.5/src/ogd/games/JOURNALISM/features/QuitType.py` & `opengamedata_core-0.0.6/src/ogd/games/JOURNALISM/features/QuitType.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # import libraries
 import json
 from typing import Any, Final, List, Optional
 import json
 # import local files
-from ogd.core.schemas.Event import Event
-from ogd.core.schemas.ExtractionMode import ExtractionMode
-from ogd.core.schemas.FeatureData import FeatureData
+from ogd.core.models.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
+from ogd.core.models.FeatureData import FeatureData
 from ogd.core.generators.Generator import GeneratorParameters
 from ogd.core.generators.extractors.SessionFeature import SessionFeature
 
 
 """
 QuitType logic:
 -"complete_level", "display_feedback", "resumed_checkpoint", "level_fail" all denote certain breakpoints in quit types
```

### Comparing `opengamedata_core-0.0.5/src/ogd/games/JOURNALISM/features/QuitTypePerLevel.py` & `opengamedata_core-0.0.6/src/ogd/games/JOURNALISM/features/QuitTypePerLevel.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # import libraries
 import json
 from typing import Any, Final, List, Optional
 import json
 # import local files
 from ogd.core.generators.extractors.PerLevelFeature import PerLevelFeature
-from ogd.core.schemas.Event import Event
-from ogd.core.schemas.ExtractionMode import ExtractionMode
-from ogd.core.schemas.FeatureData import FeatureData
+from ogd.core.models.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
+from ogd.core.models.FeatureData import FeatureData
 from ogd.core.generators.Generator import GeneratorParameters
 
 
 """
 
 """
```

### Comparing `opengamedata_core-0.0.5/src/ogd/games/JOURNALISM/features/SessionPlayTime.py` & `opengamedata_core-0.0.6/src/ogd/games/JOURNALISM/features/StoryEditorTime.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,34 +1,41 @@
 # import libraries
 import json
 from typing import Any, Final, List, Optional
 import json
 from datetime  import timedelta, datetime
 # import local files
 from ogd.core.generators.extractors.Feature import Feature
-from ogd.core.schemas.Event import Event
-from ogd.core.schemas.ExtractionMode import ExtractionMode
-from ogd.core.schemas.FeatureData import FeatureData
+from ogd.core.generators.extractors.PerLevelFeature import PerLevelFeature
+from ogd.core.models.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
+from ogd.core.models.FeatureData import FeatureData
 from ogd.core.generators.Generator import GeneratorParameters
 from ogd.core.generators.extractors.SessionFeature import SessionFeature
 
 
 
 
 
-class SessionPlayTime(SessionFeature):
+class StoryEditorTime(PerLevelFeature):
     """Template file to serve as a guide for creating custom Feature subclasses for games.
 
     :param Feature: Base class for a Custom Feature class.
     :type Feature: _type_
     """
     IDLE_TIME_THRESHOLD : Final[timedelta] = timedelta(seconds=60)
 
     def __init__(self, params:GeneratorParameters, threshold: int):
         super().__init__(params=params)
+        PerLevelFeature.__init__(self, params=params)
+
+
+        ##enable feature logic only when in the story editor
+        self._editor_watch_enabled: bool = False
+
         self._first_event_timestamp : Optional[datetime] = None
         self._last_event_timestamp : Optional[datetime] = None
 
         self._idle_time : Optional[timedelta] = None
         self._time : timedelta = timedelta(0)
         self._count : int = 0
         self._last_timestamp : Optional[datetime] = None
@@ -38,15 +45,15 @@
         # >>> create/initialize any variables to track feature extractor state <<<
         #
         # e.g. To track whether extractor found a click event yet:
         # self._found_click : bool = False
     
     @staticmethod
     def defaultThreshold():
-        return SessionPlayTime.IDLE_TIME_THRESHOLD
+        return StoryEditorTime.IDLE_TIME_THRESHOLD
 
     # *** IMPLEMENT ABSTRACT FUNCTIONS ***
     @classmethod
     def _eventFilter(cls, mode:ExtractionMode) -> List[str]:
         """_summary_
 
         :return: _description_
@@ -69,34 +76,43 @@
         :param event: _description_
         :type event: Event
         """
         # >>> use the data in the Event object to update state variables as needed. <<<
         # Note that this function runs once on each Event whose name matches one of the strings returned by _eventFilter()
         #
         # e.g. check if the event name contains the substring "Click," and if so set self._found_click to True
-        if not self._first_event_timestamp:
-            self._first_event_timestamp = event.Timestamp
+        if event.EventName == "open_notebook":
+            self._editor_watch_enabled = True
+        
+        if self._editor_watch_enabled == True:
+        
+            if not self._first_event_timestamp:
+                self._first_event_timestamp = event.Timestamp
 
-        if not self._last_timestamp:
+            if not self._last_timestamp:
+                self._last_timestamp = event.Timestamp
+                print("set self._last!")
+                return
+            if self._last_timestamp is not None:
+                time_since_last = event.Timestamp - self._last_timestamp
+                if time_since_last > StoryEditorTime.IDLE_TIME_THRESHOLD:
+                    self._time += time_since_last
+                    self._count += 1
+            else:
+                raise ValueError("In IdleState, last timestamp is None!")
             self._last_timestamp = event.Timestamp
-            print("set self._last!")
-            return
-        if self._last_timestamp is not None:
-            time_since_last = event.Timestamp - self._last_timestamp
-            if time_since_last > SessionPlayTime.IDLE_TIME_THRESHOLD:
-                self._time += time_since_last
-                self._count += 1
-        else:
-            raise ValueError("In IdleState, last timestamp is None!")
-        self._last_timestamp = event.Timestamp
 
-        if(not self._first_event_timestamp):
-            self._first_event_timestamp = event.Timestamp
+            if(not self._first_event_timestamp):
+                self._first_event_timestamp = event.Timestamp
+            
+            self._last_event_timestamp = event.Timestamp
         
-        self._last_event_timestamp = event.Timestamp
+        ##check to see if editor_watch should be disabled 
+        if event.EventName =="close_notebook" and self._editor_watch_enabled == True:
+            self._editor_watch_enabled = False
 
 
         return
 
     def _updateFromFeatureData(self, feature: FeatureData):
         """_summary_
```

### Comparing `opengamedata_core-0.0.5/src/ogd/games/JOURNALISM/features/SkillSequenceCount.py` & `opengamedata_core-0.0.6/src/ogd/games/JOURNALISM/features/SkillSequenceCount.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # import libraries
 import json
 from typing import Any, List, Optional
 # import local files
 from ogd.core.generators.extractors.Feature import Feature
-from ogd.core.schemas.Event import Event
-from ogd.core.schemas.ExtractionMode import ExtractionMode
-from ogd.core.schemas.FeatureData import FeatureData
+from ogd.core.models.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
+from ogd.core.models.FeatureData import FeatureData
 from ogd.core.generators.Generator import GeneratorParameters
 from ogd.core.generators.extractors.SessionFeature import SessionFeature
 
 
 
 
 class SkillSequenceCount(SessionFeature):
```

### Comparing `opengamedata_core-0.0.5/src/ogd/games/JOURNALISM/features/SnippetReceivedCount.py` & `opengamedata_core-0.0.6/src/ogd/games/JOURNALISM/features/SnippetReceivedCount.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # import libraries
 import json
 from typing import Any, List, Optional
 # import local files
 from ogd.core.generators.extractors.Feature import Feature
-from ogd.core.schemas.Event import Event
-from ogd.core.schemas.ExtractionMode import ExtractionMode
-from ogd.core.schemas.FeatureData import FeatureData
+from ogd.core.models.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
+from ogd.core.models.FeatureData import FeatureData
 from ogd.core.generators.Generator import GeneratorParameters
 from ogd.core.generators.extractors.SessionFeature import SessionFeature
 
 
 
 
 class SnippetReceivedCount(SessionFeature):
```

### Comparing `opengamedata_core-0.0.5/src/ogd/games/JOURNALISM/features/SnippetReplace.py` & `opengamedata_core-0.0.6/src/ogd/games/JOURNALISM/features/SnippetReplace.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # import libraries
 import json
 from typing import Any, List, Optional
 # import local files
 from ogd.core.generators.extractors.Feature import Feature
 from ogd.core.generators.extractors.PerLevelFeature import PerLevelFeature
-from ogd.core.schemas.Event import Event
-from ogd.core.schemas.ExtractionMode import ExtractionMode
-from ogd.core.schemas.FeatureData import FeatureData
+from ogd.core.models.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
+from ogd.core.models.FeatureData import FeatureData
 from ogd.core.generators.Generator import GeneratorParameters
 from ogd.core.generators.extractors.SessionFeature import SessionFeature
 
 
 
 
 class SnippetReplace(PerLevelFeature):
```

### Comparing `opengamedata_core-0.0.5/src/ogd/games/JOURNALISM/features/SnippetsCollected.py` & `opengamedata_core-0.0.6/src/ogd/games/JOURNALISM/features/SnippetsCollected.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import logging
 from datetime import datetime
-from ogd.core.schemas import Event
+from ogd.core.models import Event
 from typing import Any, List, Optional
 # import locals
 from ogd.core.utils.Logger import Logger
 from ogd.core.generators.extractors.PerLevelFeature import PerLevelFeature
 from ogd.core.generators.Generator import GeneratorParameters
-from ogd.core.schemas.Event import Event
-from ogd.core.schemas.ExtractionMode import ExtractionMode
-from ogd.core.schemas.FeatureData import FeatureData
+from ogd.core.models.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
+from ogd.core.models.FeatureData import FeatureData
 
 class SnippetsCollected(PerLevelFeature):
     def __init__(self, params:GeneratorParameters):
         PerLevelFeature.__init__(self, params=params)
         self._snippet_ids   : List[str] = []
         self._snippet_quals : List[str] = []
         self._snippet_types : List[str] = []
```

### Comparing `opengamedata_core-0.0.5/src/ogd/games/JOURNALISM/features/SnippetsSubmitted.py` & `opengamedata_core-0.0.6/src/ogd/games/JOURNALISM/features/SnippetsSubmitted.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import logging
 import json
 from datetime import datetime
-from ogd.core.schemas import Event
+from ogd.core.models import Event
 from typing import Any, List, Optional
 # import locals
 from ogd.core.utils.Logger import Logger
 from ogd.core.generators.extractors.PerLevelFeature import PerLevelFeature
 from ogd.core.generators.Generator import GeneratorParameters
-from ogd.core.schemas.Event import Event
-from ogd.core.schemas.ExtractionMode import ExtractionMode
-from ogd.core.schemas.FeatureData import FeatureData
+from ogd.core.models.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
+from ogd.core.models.FeatureData import FeatureData
 
 class SnippetsSubmitted(PerLevelFeature):
     has_printed = False
     def __init__(self, params:GeneratorParameters):
         PerLevelFeature.__init__(self, params=params)
         self._snippet_ids : List[str] = []
```

### Comparing `opengamedata_core-0.0.5/src/ogd/games/JOURNALISM/features/StoryAlignment.py` & `opengamedata_core-0.0.6/src/ogd/games/JOURNALISM/features/StoryAlignment.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # import libraries
 from os import truncate
-from ogd.core.schemas import Event
+from ogd.core.models import Event
 from typing import Any, List, Optional
 # import locals
 from ogd.core.generators.extractors.PerLevelFeature import PerLevelFeature
 from ogd.core.generators.Generator import GeneratorParameters
-from ogd.core.schemas.Event import Event
-from ogd.core.schemas.ExtractionMode import ExtractionMode
-from ogd.core.schemas.FeatureData import FeatureData
+from ogd.core.models.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
+from ogd.core.models.FeatureData import FeatureData
 
 class StoryAlignment(PerLevelFeature):
     def __init__(self, params:GeneratorParameters):
         PerLevelFeature.__init__(self, params=params)
         self._story_alignment = 0
         ##print("working!")
```

### Comparing `opengamedata_core-0.0.5/src/ogd/games/JOURNALISM/features/StoryAlignmentSequence.py` & `opengamedata_core-0.0.6/src/ogd/games/JOURNALISM/features/StoryAlignmentSequence.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # import libraries
 from typing import Any, List
-from ogd.core.schemas import Event
+from ogd.core.models import Event
 from ogd.core.generators.extractors.PerLevelFeature import PerLevelFeature
 from ogd.core.generators.Generator import GeneratorParameters
-from ogd.core.schemas.Event import Event
-from ogd.core.schemas.ExtractionMode import ExtractionMode
-from ogd.core.schemas.FeatureData import FeatureData
+from ogd.core.models.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
+from ogd.core.models.FeatureData import FeatureData
 
 """
 class StoryAlignmentSequence(PerLevelFeature):
     def __init__(self, params: GeneratorParameters):
         PerLevelFeature.__init__(self, params=params)
         self._story_alignment_sequence = []
```

### Comparing `opengamedata_core-0.0.5/src/ogd/games/JOURNALISM/features/StoryCompleteTime.py` & `opengamedata_core-0.0.6/src/ogd/games/JOURNALISM/features/StoryCompleteTime.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # import libraries
 import json
 from typing import Any, List, Optional
 # import local files
 from ogd.core.generators.extractors.Feature import Feature
-from ogd.core.schemas.Event import Event
-from ogd.core.schemas.ExtractionMode import ExtractionMode
-from ogd.core.schemas.FeatureData import FeatureData
+from ogd.core.models.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
+from ogd.core.models.FeatureData import FeatureData
 from ogd.core.generators.Generator import GeneratorParameters
 from ogd.core.generators.extractors.SessionFeature import SessionFeature
 from time import time
 from datetime  import timedelta, datetime
```

### Comparing `opengamedata_core-0.0.5/src/ogd/games/JOURNALISM/features/StoryEditorTime.py` & `opengamedata_core-0.0.6/src/ogd/games/JOURNALISM/features/SessionPlayTime.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,41 +1,34 @@
 # import libraries
 import json
 from typing import Any, Final, List, Optional
 import json
 from datetime  import timedelta, datetime
 # import local files
 from ogd.core.generators.extractors.Feature import Feature
-from ogd.core.generators.extractors.PerLevelFeature import PerLevelFeature
-from ogd.core.schemas.Event import Event
-from ogd.core.schemas.ExtractionMode import ExtractionMode
-from ogd.core.schemas.FeatureData import FeatureData
+from ogd.core.models.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
+from ogd.core.models.FeatureData import FeatureData
 from ogd.core.generators.Generator import GeneratorParameters
 from ogd.core.generators.extractors.SessionFeature import SessionFeature
 
 
 
 
 
-class StoryEditorTime(PerLevelFeature):
+class SessionPlayTime(SessionFeature):
     """Template file to serve as a guide for creating custom Feature subclasses for games.
 
     :param Feature: Base class for a Custom Feature class.
     :type Feature: _type_
     """
     IDLE_TIME_THRESHOLD : Final[timedelta] = timedelta(seconds=60)
 
     def __init__(self, params:GeneratorParameters, threshold: int):
         super().__init__(params=params)
-        PerLevelFeature.__init__(self, params=params)
-
-
-        ##enable feature logic only when in the story editor
-        self._editor_watch_enabled: bool = False
-
         self._first_event_timestamp : Optional[datetime] = None
         self._last_event_timestamp : Optional[datetime] = None
 
         self._idle_time : Optional[timedelta] = None
         self._time : timedelta = timedelta(0)
         self._count : int = 0
         self._last_timestamp : Optional[datetime] = None
@@ -45,15 +38,15 @@
         # >>> create/initialize any variables to track feature extractor state <<<
         #
         # e.g. To track whether extractor found a click event yet:
         # self._found_click : bool = False
     
     @staticmethod
     def defaultThreshold():
-        return StoryEditorTime.IDLE_TIME_THRESHOLD
+        return SessionPlayTime.IDLE_TIME_THRESHOLD
 
     # *** IMPLEMENT ABSTRACT FUNCTIONS ***
     @classmethod
     def _eventFilter(cls, mode:ExtractionMode) -> List[str]:
         """_summary_
 
         :return: _description_
@@ -76,43 +69,34 @@
         :param event: _description_
         :type event: Event
         """
         # >>> use the data in the Event object to update state variables as needed. <<<
         # Note that this function runs once on each Event whose name matches one of the strings returned by _eventFilter()
         #
         # e.g. check if the event name contains the substring "Click," and if so set self._found_click to True
-        if event.EventName == "open_notebook":
-            self._editor_watch_enabled = True
-        
-        if self._editor_watch_enabled == True:
-        
-            if not self._first_event_timestamp:
-                self._first_event_timestamp = event.Timestamp
+        if not self._first_event_timestamp:
+            self._first_event_timestamp = event.Timestamp
 
-            if not self._last_timestamp:
-                self._last_timestamp = event.Timestamp
-                print("set self._last!")
-                return
-            if self._last_timestamp is not None:
-                time_since_last = event.Timestamp - self._last_timestamp
-                if time_since_last > StoryEditorTime.IDLE_TIME_THRESHOLD:
-                    self._time += time_since_last
-                    self._count += 1
-            else:
-                raise ValueError("In IdleState, last timestamp is None!")
+        if not self._last_timestamp:
             self._last_timestamp = event.Timestamp
+            print("set self._last!")
+            return
+        if self._last_timestamp is not None:
+            time_since_last = event.Timestamp - self._last_timestamp
+            if time_since_last > SessionPlayTime.IDLE_TIME_THRESHOLD:
+                self._time += time_since_last
+                self._count += 1
+        else:
+            raise ValueError("In IdleState, last timestamp is None!")
+        self._last_timestamp = event.Timestamp
 
-            if(not self._first_event_timestamp):
-                self._first_event_timestamp = event.Timestamp
-            
-            self._last_event_timestamp = event.Timestamp
+        if(not self._first_event_timestamp):
+            self._first_event_timestamp = event.Timestamp
         
-        ##check to see if editor_watch should be disabled 
-        if event.EventName =="close_notebook" and self._editor_watch_enabled == True:
-            self._editor_watch_enabled = False
+        self._last_event_timestamp = event.Timestamp
 
 
         return
 
     def _updateFromFeatureData(self, feature: FeatureData):
         """_summary_
```

### Comparing `opengamedata_core-0.0.5/src/ogd/games/JOURNALISM/features/StoryScore.py` & `opengamedata_core-0.0.6/src/ogd/games/JOURNALISM/features/StoryScore.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # import libraries
 from typing import Any, List
-from ogd.core.schemas import Event
+from ogd.core.models import Event
 from ogd.core.generators.extractors.PerLevelFeature import PerLevelFeature
 from ogd.core.generators.Generator import GeneratorParameters
-from ogd.core.schemas.Event import Event
-from ogd.core.schemas.ExtractionMode import ExtractionMode
-from ogd.core.schemas.FeatureData import FeatureData
+from ogd.core.models.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
+from ogd.core.models.FeatureData import FeatureData
 
 
 class StoryScore(PerLevelFeature):
     def __init__(self, params: GeneratorParameters):
         PerLevelFeature.__init__(self, params=params)
         self._story_score = 0
```

### Comparing `opengamedata_core-0.0.5/src/ogd/games/JOURNALISM/features/StoryScoreSequence.py` & `opengamedata_core-0.0.6/src/ogd/games/JOURNALISM/features/StoryScoreSequence.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # import libraries
 from typing import Any, List
-from ogd.core.schemas import Event
+from ogd.core.models import Event
 from ogd.core.generators.extractors.PerLevelFeature import PerLevelFeature
 from ogd.core.generators.Generator import GeneratorParameters
-from ogd.core.schemas.Event import Event
-from ogd.core.schemas.ExtractionMode import ExtractionMode
-from ogd.core.schemas.FeatureData import FeatureData
+from ogd.core.models.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
+from ogd.core.models.FeatureData import FeatureData
 
 
 """class StoryAlignmentSequence(PerLevelFeature):
     def __init__(self, params: GeneratorParameters):
         PerLevelFeature.__init__(self, params=params)
         self._story_alignment_sequence = []
```

### Comparing `opengamedata_core-0.0.5/src/ogd/games/JOURNALISM/features/TextClickCount.py` & `opengamedata_core-0.0.6/src/ogd/games/JOURNALISM/features/TextClickCount.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # import libraries
 import json
 from typing import Any, List, Optional
 # import local files
 from ogd.core.generators.extractors.Feature import Feature
-from ogd.core.schemas.Event import Event
-from ogd.core.schemas.ExtractionMode import ExtractionMode
-from ogd.core.schemas.FeatureData import FeatureData
+from ogd.core.models.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
+from ogd.core.models.FeatureData import FeatureData
 from ogd.core.generators.Generator import GeneratorParameters
 from ogd.core.generators.extractors.SessionFeature import SessionFeature
 
 
 
 
 class TextClickCount(SessionFeature):
```

### Comparing `opengamedata_core-0.0.5/src/ogd/games/JOURNALISM/features/TopAttribute.py` & `opengamedata_core-0.0.6/src/ogd/games/JOURNALISM/features/TopAttribute.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # import libraries
 import json
 from typing import Any, Final, List
 # import local files
 from ogd.core.generators.extractors.Feature import Feature
-from ogd.core.schemas.Event import Event
-from ogd.core.schemas.ExtractionMode import ExtractionMode
-from ogd.core.schemas.FeatureData import FeatureData
+from ogd.core.models.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
+from ogd.core.models.FeatureData import FeatureData
 from ogd.core.generators.Generator import GeneratorParameters
 from ogd.core.generators.extractors.SessionFeature import SessionFeature
 
 
 
 
 class TopAttribute(SessionFeature):
```

### Comparing `opengamedata_core-0.0.5/src/ogd/games/JOURNALISM/features/TopPlayerAttribute.py` & `opengamedata_core-0.0.6/src/ogd/games/JOURNALISM/features/TopPlayerAttribute.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 # import libraries
 from os import truncate
 from ogd.core.generators.extractors.PerCountFeature import PerCountFeature
-from ogd.core.schemas import Event
+from ogd.core.models import Event
 from typing import Any, Final, List
 # import locals
 from ogd.core.generators.extractors.PerLevelFeature import PerLevelFeature
 from ogd.core.generators.Generator import GeneratorParameters
-from ogd.core.schemas.Event import Event
-from ogd.core.schemas.ExtractionMode import ExtractionMode
-from ogd.core.schemas.FeatureData import FeatureData
+from ogd.core.models.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
+from ogd.core.models.FeatureData import FeatureData
 
 class TopPlayerAttribute(PerCountFeature):
     def __init__(self, params:GeneratorParameters):
         PerCountFeature.__init__(self, params=params)
         self._attr_count = 0
         self._ATTRIBUTE_ENUM : Final[List[str]] = ["endurance", "resourceful", "tech","social","trust","research"]
         self._attr_name = self._ATTRIBUTE_ENUM[self.CountIndex]
```

### Comparing `opengamedata_core-0.0.5/src/ogd/games/JOURNALISM/features/TopPlayerQuitType.py` & `opengamedata_core-0.0.6/src/ogd/games/JOURNALISM/features/TopPlayerQuitType.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 # import libraries
 from os import truncate
 from ogd.core.generators.extractors.PerCountFeature import PerCountFeature
-from ogd.core.schemas import Event
+from ogd.core.models import Event
 from typing import Any, Final, List, Optional
 # import locals
 from ogd.core.generators.extractors.PerLevelFeature import PerLevelFeature
 from ogd.core.generators.Generator import GeneratorParameters
-from ogd.core.schemas.Event import Event
-from ogd.core.schemas.ExtractionMode import ExtractionMode
-from ogd.core.schemas.FeatureData import FeatureData
+from ogd.core.models.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
+from ogd.core.models.FeatureData import FeatureData
 
 class TopPlayerQuitType(PerCountFeature):
     def __init__(self, params:GeneratorParameters):
         PerCountFeature.__init__(self, params=params)
         self._attr_count = 0
         self._ATTRIBUTE_ENUM : Final[List[str]] = ["BetweenLevels", "OnFail", "OnCheckpoint","Other"]
         self._attr_name = self._ATTRIBUTE_ENUM[self.CountIndex]
```

### Comparing `opengamedata_core-0.0.5/src/ogd/games/JOURNALISM/features/TotalFails.py` & `opengamedata_core-0.0.6/src/ogd/games/JOURNALISM/features/TotalFails.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # import libraries
 import json
 from typing import Any, List, Optional
 # import local files
 from ogd.core.generators.extractors.Feature import Feature
-from ogd.core.schemas.Event import Event
-from ogd.core.schemas.ExtractionMode import ExtractionMode
-from ogd.core.schemas.FeatureData import FeatureData
+from ogd.core.models.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
+from ogd.core.models.FeatureData import FeatureData
 from ogd.core.generators.Generator import GeneratorParameters
 from ogd.core.generators.extractors.SessionFeature import SessionFeature
 
 
 
 
 class TotalFails(SessionFeature):
```

### Comparing `opengamedata_core-0.0.5/src/ogd/games/JOURNALISM/features/TotalLevelTime.py` & `opengamedata_core-0.0.6/src/ogd/games/JOURNALISM/features/TotalLevelTime.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 # import libraries
 import logging
 from datetime import datetime
-from ogd.core.schemas import Event
+from ogd.core.models import Event
 from typing import Any, List, Optional
 # import locals
 from ogd.core.utils.Logger import Logger
 from ogd.core.generators.extractors.PerLevelFeature import PerLevelFeature
 from ogd.core.generators.Generator import GeneratorParameters
-from ogd.core.schemas.Event import Event
-from ogd.core.schemas.ExtractionMode import ExtractionMode
-from ogd.core.schemas.FeatureData import FeatureData
+from ogd.core.models.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
+from ogd.core.models.FeatureData import FeatureData
 
 class TotalLevelTime(PerLevelFeature):
     def __init__(self, params:GeneratorParameters):
         PerLevelFeature.__init__(self, params=params)
         self._begin_times    : List[datetime] = []
         self._complete_times : List[datetime] = []
```

### Comparing `opengamedata_core-0.0.5/src/ogd/games/JOURNALISM/features/UserPlayTime.py` & `opengamedata_core-0.0.6/src/ogd/games/JOURNALISM/features/UserPlayTime.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 import json
 from typing import Any, List, Optional
 import json
 from time import time
 from datetime  import timedelta, datetime
 # import local files
 from ogd.core.generators.extractors.Feature import Feature
-from ogd.core.schemas.Event import Event
-from ogd.core.schemas.ExtractionMode import ExtractionMode
-from ogd.core.schemas.FeatureData import FeatureData
+from ogd.core.models.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
+from ogd.core.models.FeatureData import FeatureData
 from ogd.core.generators.Generator import GeneratorParameters
 from ogd.core.generators.extractors.SessionFeature import SessionFeature
```

### Comparing `opengamedata_core-0.0.5/src/ogd/games/JOURNALISM/features/WorstAttribute.py` & `opengamedata_core-0.0.6/src/ogd/games/JOURNALISM/features/WorstAttribute.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # import libraries
 import json
 from typing import Any, Final, List, Optional
 # import local files
 from ogd.core.generators.extractors.Feature import Feature
-from ogd.core.schemas.Event import Event
-from ogd.core.schemas.ExtractionMode import ExtractionMode
-from ogd.core.schemas.FeatureData import FeatureData
+from ogd.core.models.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
+from ogd.core.models.FeatureData import FeatureData
 from ogd.core.generators.Generator import GeneratorParameters
 from ogd.core.generators.extractors.SessionFeature import SessionFeature
 
 class WorstAttribute(SessionFeature):
     """Template file to serve as a guide for creating custom Feature subclasses for games.
 
     :param Feature: Base class for a Custom Feature class.
```

### Comparing `opengamedata_core-0.0.5/src/ogd/games/JOURNALISM/features/WorstPlayerAttribute.py` & `opengamedata_core-0.0.6/src/ogd/games/JOURNALISM/features/MaxedPlayerAttribute.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 # import libraries
 from os import truncate
 from ogd.core.generators.extractors.PerCountFeature import PerCountFeature
-from ogd.core.schemas import Event
+from ogd.core.models import Event
 from typing import Any, Final, List, Optional
 # import locals
 from ogd.core.generators.extractors.PerLevelFeature import PerLevelFeature
 from ogd.core.generators.Generator import GeneratorParameters
-from ogd.core.schemas.Event import Event
-from ogd.core.schemas.ExtractionMode import ExtractionMode
-from ogd.core.schemas.FeatureData import FeatureData
+from ogd.core.models.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
+from ogd.core.models.FeatureData import FeatureData
 
-class WorstPlayerAttribute(PerCountFeature):
+class MaxedPlayerAttribute(PerCountFeature):
     def __init__(self, params:GeneratorParameters):
         PerCountFeature.__init__(self, params=params)
-        self._attr_count = 0
+        self._attr_count     : int              = 0
         self._ATTRIBUTE_ENUM : Final[List[str]] = ["endurance", "resourceful", "tech","social","trust","research"]
-        self._attr_name = self._ATTRIBUTE_ENUM[self.CountIndex]
+        self._attr_name      : str              = self._ATTRIBUTE_ENUM[self.CountIndex]
 
 
     # *** IMPLEMENT ABSTRACT FUNCTIONS ***
     def _validateEventCountIndex(self, event:Event):
         
         return False
         #return int(event.GameState['att']) == self.CountIndex
@@ -28,29 +28,33 @@
 
     @classmethod
     def _eventFilter(cls, mode:ExtractionMode) -> List[str]:
         return [""]
 
     @classmethod
     def _featureFilter(cls, mode:ExtractionMode) -> List[str]:
-        return ["WorstAttribute"]
+        return ["TopAttribute"]
 
     def _updateFromEvent(self, event:Event) -> None:
         #self._story_alignment = event.EventData["story_alignment"]
 
         pass
 
 
     def _updateFromFeatureData(self, feature:FeatureData):
         #add logic to make sure that MODE is session, not player so we don't get duplicates
         if(feature._mode == ExtractionMode.SESSION):
             attribute_list = feature._vals[1]
             for attr in attribute_list:
                 if(self._ATTRIBUTE_ENUM.index(attr) == self.CountIndex):
-                    self._attr_count+=1
+                    if(feature._vals[0]>=10):
+                        self._attr_count+=1
+
+
+
             
         return
 
     def _getFeatureValues(self) -> List[Any]:
         return [self._attr_name, self._attr_count]
 
     # *** Optionally override public functions. ***
```

### Comparing `opengamedata_core-0.0.5/src/ogd/games/JOURNALISM/features/__init__.py` & `opengamedata_core-0.0.6/src/ogd/games/JOURNALISM/features/__init__.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.5/src/ogd/games/JOURNALISM/schemas/JOURNALISM.json.template` & `opengamedata_core-0.0.6/src/ogd/games/JOURNALISM/schemas/JOURNALISM.json.template`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.5/src/ogd/games/JOWILDER/JowilderLoader.py` & `opengamedata_core-0.0.6/src/ogd/games/JOWILDER/JowilderLoader.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 ## import local files
 from . import features
 from ogd.core.generators.detectors.Detector import Detector
 from ogd.core.generators.Generator import GeneratorParameters
 from ogd.core.generators.extractors.Feature import Feature
 from ogd.core.generators.GeneratorLoader import GeneratorLoader
 from ogd.games.JOWILDER.features.UsedContinue import UsedContinue
-from ogd.core.schemas.Event import Event
-from ogd.core.schemas.ExtractionMode import ExtractionMode
+from ogd.core.models.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
 from ogd.core.schemas.games.GameSchema import GameSchema
 from ogd.games.JOWILDER.features import *
 
 
 
 class JowilderLoader(GeneratorLoader):
```

### Comparing `opengamedata_core-0.0.5/src/ogd/games/JOWILDER/Jowilder_Enumerators.py` & `opengamedata_core-0.0.6/src/ogd/games/JOWILDER/Jowilder_Enumerators.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.5/src/ogd/games/JOWILDER/features/ActiveStateTime.py` & `opengamedata_core-0.0.6/src/ogd/games/JOWILDER/features/ActiveStateTime.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # import libraries
 import json
 from typing import Any, Final, List, Optional
 from datetime  import timedelta, datetime
 # import local files
 from ogd.core.generators.Generator import GeneratorParameters
 from ogd.core.generators.extractors.SessionFeature import SessionFeature
-from ogd.core.schemas.ExtractionMode import ExtractionMode
-from ogd.core.schemas.FeatureData import FeatureData
-from ogd.core.schemas.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
+from ogd.core.models.FeatureData import FeatureData
+from ogd.core.models.Event import Event
 
 class ActiveStateTime(SessionFeature):
     """Template file to serve as a guide for creating custom Feature subclasses for games.
 
     :param Feature: Base class for a Custom Feature class.
     :type Feature: _type_
     """
```

### Comparing `opengamedata_core-0.0.5/src/ogd/games/JOWILDER/features/Clicks.py` & `opengamedata_core-0.0.6/src/ogd/games/JOWILDER/features/Clicks.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # import libraries
 import logging
 from typing import Any, List, Optional
 from ogd.core.generators.Generator import GeneratorParameters
 # import local files
 from ogd.core.generators.extractors.SessionFeature import SessionFeature
-from ogd.core.schemas.ExtractionMode import ExtractionMode
-from ogd.core.schemas.FeatureData import FeatureData
-from ogd.core.schemas.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
+from ogd.core.models.FeatureData import FeatureData
+from ogd.core.models.Event import Event
 from ogd.core.utils.Logger import Logger
 
 class Clicks(SessionFeature):
     """Template file to serve as a guide for creating custom Feature subclasses for games.
 
     :param Feature: Base class for a Custom Feature class.
     :type Feature: _type_
```

### Comparing `opengamedata_core-0.0.5/src/ogd/games/JOWILDER/features/EventCount.py` & `opengamedata_core-0.0.6/src/ogd/games/JOWILDER/features/EventCount.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # import libraries
 import json
 from typing import Any, List, Optional
 # import local files
 from ogd.core.generators.Generator import GeneratorParameters
 from ogd.core.generators.extractors.SessionFeature import SessionFeature
-from ogd.core.schemas.ExtractionMode import ExtractionMode
-from ogd.core.schemas.FeatureData import FeatureData
-from ogd.core.schemas.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
+from ogd.core.models.FeatureData import FeatureData
+from ogd.core.models.Event import Event
 
 class EventCount(SessionFeature):
     """Template file to serve as a guide for creating custom Feature subclasses for games.
 
     :param Feature: Base class for a Custom Feature class.
     :type Feature: _type_
     """
```

### Comparing `opengamedata_core-0.0.5/src/ogd/games/JOWILDER/features/FirstInteraction.py` & `opengamedata_core-0.0.6/src/ogd/games/JOWILDER/features/LastInteraction.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 # import libraries
 import json
 from typing import Any, Final, List, Optional
 # import local files
 from ogd.core.generators.Generator import GeneratorParameters
 from ogd.core.generators.extractors.SessionFeature import SessionFeature
-from ogd.core.schemas.ExtractionMode import ExtractionMode
-from ogd.core.schemas.FeatureData import FeatureData
-from ogd.core.schemas.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
+from ogd.core.models.FeatureData import FeatureData
+from ogd.core.models.Event import Event
 
-class FirstInteraction(SessionFeature):
+class LastInteraction(SessionFeature):
     """Template file to serve as a guide for creating custom Feature subclasses for games.
 
     :param Feature: Base class for a Custom Feature class.
     :type Feature: _type_
     """
     NO_SENSE : Final[str] = 'tunic.historicalsociety.closet.intro'
 
@@ -27,16 +27,16 @@
 
     @classmethod
     def _featureFilter(cls, mode:ExtractionMode) -> List[str]:
         return []
 
     def _updateFromEvent(self, event:Event) -> None:
         _interaction = event.EventData.get("text_fqid")
-        if _interaction is not None and _interaction != FirstInteraction.NO_SENSE and self._interaction is None:
-            self._interaction = event.EventData.get("text_fqid")
+        if _interaction is not None and _interaction != LastInteraction.NO_SENSE:
+            self._interaction = _interaction
 
         return
 
     def _updateFromFeatureData(self, feature: FeatureData):
         return
 
     def _getFeatureValues(self) -> List[Any]:
```

### Comparing `opengamedata_core-0.0.5/src/ogd/games/JOWILDER/features/GameScript.py` & `opengamedata_core-0.0.6/src/ogd/games/JOWILDER/features/GameScript.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # import libraries
 from typing import Any, Dict, Final, List, Optional
 from ogd.core.generators.Generator import GeneratorParameters
 # import local files
 from ogd.core.generators.extractors.SessionFeature import SessionFeature
-from ogd.core.schemas.ExtractionMode import ExtractionMode
-from ogd.core.schemas.FeatureData import FeatureData
-from ogd.core.schemas.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
+from ogd.core.models.FeatureData import FeatureData
+from ogd.core.models.Event import Event
 
 class GameScript(SessionFeature):
     """Template file to serve as a guide for creating custom Feature subclasses for games.
 
     :param Feature: Base class for a Custom Feature class.
     :type Feature: _type_
     """
```

### Comparing `opengamedata_core-0.0.5/src/ogd/games/JOWILDER/features/GameVersion.py` & `opengamedata_core-0.0.6/src/ogd/games/WAVES/features/TotalArrowMoves.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,44 +1,35 @@
 # import libraries
-from typing import Any, List, Optional, Union
+from ogd.core.models import Event
+from typing import Any, List, Optional
+# import locals
+from ogd.core.generators.extractors.PerLevelFeature import PerLevelFeature
 from ogd.core.generators.Generator import GeneratorParameters
-# import local files
-from ogd.core.generators.extractors.SessionFeature import SessionFeature
-from ogd.core.schemas.ExtractionMode import ExtractionMode
-from ogd.core.schemas.FeatureData import FeatureData
-from ogd.core.schemas.Event import Event
-
-class GameVersion(SessionFeature):
-    """Template file to serve as a guide for creating custom Feature subclasses for games.
-
-    :param Feature: Base class for a Custom Feature class.
-    :type Feature: _type_
-    """
+from ogd.core.models.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
+from ogd.core.models.FeatureData import FeatureData
+
+class TotalArrowMoves(PerLevelFeature):
     def __init__(self, params:GeneratorParameters):
-        super().__init__(params=params)
-        self._version    : Union[str,int,None] = None
-        self._log_version: Union[str,int,None] = None
+        PerLevelFeature.__init__(self, params=params)
+        self._arrow_move_count : int = 0
 
     # *** IMPLEMENT ABSTRACT FUNCTIONS ***
-
     @classmethod
     def _eventFilter(cls, mode:ExtractionMode) -> List[str]:
-        return ["CUSTOM.1"]
+        return ["CUSTOM.2"]
+        # return ["ARROW_MOVE_RELEASE"]
 
     @classmethod
     def _featureFilter(cls, mode:ExtractionMode) -> List[str]:
-        return [] 
+        return []
 
     def _updateFromEvent(self, event:Event) -> None:
-        self._version = event.AppVersion
-        self._log_version = event.LogVersion
-        return
+        self._arrow_move_count += 1
 
-    def _updateFromFeatureData(self, feature: FeatureData):
+    def _updateFromFeatureData(self, feature:FeatureData):
         return
 
     def _getFeatureValues(self) -> List[Any]:
-        return [self._version, self._log_version]
-
-    def Subfeatures(self) -> List[str]:
-        return ["Log"]
+        return [self._arrow_move_count]
 
+    # *** Optionally override public functions. ***
```

### Comparing `opengamedata_core-0.0.5/src/ogd/games/JOWILDER/features/Hovers.py` & `opengamedata_core-0.0.6/src/ogd/games/JOWILDER/features/Hovers.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # import libraries
 from typing import Any, List, Optional
 from ogd.core.generators.Generator import GeneratorParameters
 # import local files
 from ogd.core.generators.extractors.SessionFeature import SessionFeature
-from ogd.core.schemas.ExtractionMode import ExtractionMode
-from ogd.core.schemas.FeatureData import FeatureData
-from ogd.core.schemas.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
+from ogd.core.models.FeatureData import FeatureData
+from ogd.core.models.Event import Event
 
 class Hovers(SessionFeature):
     """Template file to serve as a guide for creating custom Feature subclasses for games.
 
     :param Feature: Base class for a Custom Feature class.
     :type Feature: _type_
     """
```

### Comparing `opengamedata_core-0.0.5/src/ogd/games/JOWILDER/features/IdleState.py` & `opengamedata_core-0.0.6/src/ogd/games/JOWILDER/features/IdleState.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 import json
 from time import time
 from typing import Any, Final, List, Optional
 from datetime  import timedelta, datetime
 # import local files
 from ogd.core.generators.Generator import GeneratorParameters
 from ogd.core.generators.extractors.SessionFeature import SessionFeature
-from ogd.core.schemas.ExtractionMode import ExtractionMode
-from ogd.core.schemas.FeatureData import FeatureData
-from ogd.core.schemas.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
+from ogd.core.models.FeatureData import FeatureData
+from ogd.core.models.Event import Event
 
 class IdleState(SessionFeature):
     """Template file to serve as a guide for creating custom Feature subclasses for games.
 
     :param Feature: Base class for a Custom Feature class.
     :type Feature: _type_
     """
```

### Comparing `opengamedata_core-0.0.5/src/ogd/games/JOWILDER/features/Interaction.py` & `opengamedata_core-0.0.6/src/ogd/games/JOWILDER/features/Interaction.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 from os import environ
 from sqlite3 import Timestamp
 from typing import Any, List, Optional
 from ogd.core.generators.Generator import GeneratorParameters
 # import local files
 from ogd.core.generators.extractors.PerCountFeature import PerCountFeature
 from ogd.games.JOWILDER import Jowilder_Enumerators as je
-from ogd.core.schemas.ExtractionMode import ExtractionMode
-from ogd.core.schemas.FeatureData import FeatureData
-from ogd.core.schemas.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
+from ogd.core.models.FeatureData import FeatureData
+from ogd.core.models.Event import Event
 
 # NOTE: Assumptions are: 1. All click events occured in the order like xxxx111xx222x1x3. 2. Use "text_fqid" to identify interactions. 3. The first interaction "tunic.historicalsociety.closet.intro" makes no sense so we don't need to consider it. That is, there are 190 interactions in total, but we only count 189. And we should confirm that, this tunic.historicalsociety.closet.intro doesn't occur anywhere else.
 
 
 class ClickTrack:
     def __init__(self, start_time:Optional[datetime] = None, game_start: bool = False, this_click:Optional[Event]=None, last_click:Optional[Event]=None) -> None:
         self._game_start : bool = game_start
```

### Comparing `opengamedata_core-0.0.5/src/ogd/games/JOWILDER/features/InteractionName.py` & `opengamedata_core-0.0.6/src/ogd/games/JOWILDER/features/InteractionName.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 import json
 import logging
 from pathlib import Path
 from typing import Any, Dict, List, Optional
 # import local files
 from ogd.core.generators.Generator import GeneratorParameters
 from ogd.core.generators.extractors.PerCountFeature import PerCountFeature
-from ogd.core.schemas.ExtractionMode import ExtractionMode
-from ogd.core.schemas.FeatureData import FeatureData
-from ogd.core.schemas.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
+from ogd.core.models.FeatureData import FeatureData
+from ogd.core.models.Event import Event
 from ogd.games.JOWILDER import Jowilder_Enumerators as je
 from ogd.core.utils.utils import loadJSONFile
 from ogd.core.utils.Logger import Logger
 
 interaction_path = Path('.') / "ogd" / "games" / "JOWILDER"
 METADATA_RAW : Dict[str, Dict[str, Any]] = loadJSONFile(filename="interaction_metadata.json", path=interaction_path, search_in_src=True)
 METADATA     : Dict[int, Dict[str, Any]] = {je.fqid_to_enum.get(v.get("fqid", "FQID NOT FOUND"), -1): v for v in METADATA_RAW.values()}
```

### Comparing `opengamedata_core-0.0.5/src/ogd/games/JOWILDER/features/InteractionTextBoxesPerSecond.py` & `opengamedata_core-0.0.6/src/ogd/games/JOWILDER/features/InteractionTextBoxesPerSecond.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 from typing import Any, List, Optional
 import numpy as np
 from ogd.core.generators.Generator import GeneratorParameters
 # import local files
 from ogd.core.generators.extractors.PerCountFeature import PerCountFeature
 from ogd.games.JOWILDER import Jowilder_Enumerators as je
 from ogd.games.JOWILDER.features.Interaction import clicks_track
-from ogd.core.schemas.ExtractionMode import ExtractionMode
-from ogd.core.schemas.FeatureData import FeatureData
-from ogd.core.schemas.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
+from ogd.core.models.FeatureData import FeatureData
+from ogd.core.models.Event import Event
 
 # NOTE: Assumptions are: 1. All click events occured in the order like xxxx111xx222x1x3. 2. Use "text_fqid" to identify interactions. 3. The first interaction "tunic.historicalsociety.closet.intro" makes no sense so we don't need to consider it. That is, there are 190 interactions in total, but we only count 189. And we should confirm that, this tunic.historicalsociety.closet.intro doesn't occur anywhere else.
 
 class InteractionTextBoxesPerSecond(PerCountFeature):
     """Template file to serve as a guide for creating custom Feature subclasses for games.
 
     :param Feature: Base class for a Custom Feature class.
```

### Comparing `opengamedata_core-0.0.5/src/ogd/games/JOWILDER/features/InteractionWordsPerSecond.py` & `opengamedata_core-0.0.6/src/ogd/games/JOWILDER/features/InteractionWordsPerSecond.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 import json
 from os import environ
 from typing import Any, List, Optional
 import numpy as np
 from ogd.core.generators.Generator import GeneratorParameters
 # import local files
 from ogd.core.generators.extractors.PerCountFeature import PerCountFeature
-from ogd.core.schemas.ExtractionMode import ExtractionMode
-from ogd.core.schemas.FeatureData import FeatureData
-from ogd.core.schemas.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
+from ogd.core.models.FeatureData import FeatureData
+from ogd.core.models.Event import Event
 from datetime import datetime, timedelta
 from ogd.games.JOWILDER import Jowilder_Enumerators as je
 from ogd.games.JOWILDER.features.Interaction import clicks_track
 
 # NOTE: Assumptions are: 1. All click events occured in the order like xxxx111xx222x1x3. 2. Use "text_fqid" to identify interactions. 3. The first interaction "tunic.historicalsociety.closet.intro" makes no sense so we don't need to consider it. That is, there are 190 interactions in total, but we only count 189. And we should confirm that, this tunic.historicalsociety.closet.intro doesn't occur anywhere else.
 
 class InteractionWordsPerSecond(PerCountFeature):
```

### Comparing `opengamedata_core-0.0.5/src/ogd/games/JOWILDER/features/LastInteraction.py` & `opengamedata_core-0.0.6/src/ogd/games/JOWILDER/features/FirstInteraction.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 # import libraries
 import json
 from typing import Any, Final, List, Optional
 # import local files
 from ogd.core.generators.Generator import GeneratorParameters
 from ogd.core.generators.extractors.SessionFeature import SessionFeature
-from ogd.core.schemas.ExtractionMode import ExtractionMode
-from ogd.core.schemas.FeatureData import FeatureData
-from ogd.core.schemas.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
+from ogd.core.models.FeatureData import FeatureData
+from ogd.core.models.Event import Event
 
-class LastInteraction(SessionFeature):
+class FirstInteraction(SessionFeature):
     """Template file to serve as a guide for creating custom Feature subclasses for games.
 
     :param Feature: Base class for a Custom Feature class.
     :type Feature: _type_
     """
     NO_SENSE : Final[str] = 'tunic.historicalsociety.closet.intro'
 
@@ -27,16 +27,16 @@
 
     @classmethod
     def _featureFilter(cls, mode:ExtractionMode) -> List[str]:
         return []
 
     def _updateFromEvent(self, event:Event) -> None:
         _interaction = event.EventData.get("text_fqid")
-        if _interaction is not None and _interaction != LastInteraction.NO_SENSE:
-            self._interaction = _interaction
+        if _interaction is not None and _interaction != FirstInteraction.NO_SENSE and self._interaction is None:
+            self._interaction = event.EventData.get("text_fqid")
 
         return
 
     def _updateFromFeatureData(self, feature: FeatureData):
         return
 
     def _getFeatureValues(self) -> List[Any]:
```

### Comparing `opengamedata_core-0.0.5/src/ogd/games/JOWILDER/features/MeaningfulActions.py` & `opengamedata_core-0.0.6/src/ogd/games/JOWILDER/features/MeaningfulActions.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # import libraries
 from typing import Any, List, Optional
 from ogd.core.generators.Generator import GeneratorParameters
 # import local files
 from ogd.core.generators.extractors.SessionFeature import SessionFeature
-from ogd.core.schemas.ExtractionMode import ExtractionMode
-from ogd.core.schemas.FeatureData import FeatureData
-from ogd.core.schemas.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
+from ogd.core.models.FeatureData import FeatureData
+from ogd.core.models.Event import Event
 
 
 # regexpr to test num: "fqid": ".{1,800}"(navigate|map)", "type": "click"
 
 class MeaningfulActions(SessionFeature):
     """Template file to serve as a guide for creating custom Feature subclasses for games.
```

### Comparing `opengamedata_core-0.0.5/src/ogd/games/JOWILDER/features/NotebookUses.py` & `opengamedata_core-0.0.6/src/ogd/games/JOWILDER/features/NotebookUses.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # import libraries
 import json
 from typing import Any, List, Optional
 # import local files
 from ogd.core.generators.Generator import GeneratorParameters
 from ogd.core.generators.extractors.SessionFeature import SessionFeature
-from ogd.core.schemas.ExtractionMode import ExtractionMode
-from ogd.core.schemas.FeatureData import FeatureData
-from ogd.core.schemas.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
+from ogd.core.models.FeatureData import FeatureData
+from ogd.core.models.Event import Event
 
 class NotebookUses(SessionFeature):
     """Template file to serve as a guide for creating custom Feature subclasses for games.
 
     :param Feature: Base class for a Custom Feature class.
     :type Feature: _type_
     """
```

### Comparing `opengamedata_core-0.0.5/src/ogd/games/JOWILDER/features/QuestionAnswers.py` & `opengamedata_core-0.0.6/src/ogd/games/JOWILDER/features/QuestionAnswers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # import libraries
 from typing import Any, List, Optional
 # import locals
 from ogd.core.generators.extractors.PerCountFeature import PerCountFeature
 from ogd.core.generators.Generator import GeneratorParameters
-from ogd.core.schemas.ExtractionMode import ExtractionMode
-from ogd.core.schemas.FeatureData import FeatureData
-from ogd.core.schemas.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
+from ogd.core.models.FeatureData import FeatureData
+from ogd.core.models.Event import Event
 from .. import Jowilder_Enumerators as je
 
 
 
 # NOTE: Assumption is that in question 10 and qustion 16, we will have hover events which indicates new answer
 
 class QuestionAnswers(PerCountFeature):
```

### Comparing `opengamedata_core-0.0.5/src/ogd/games/JOWILDER/features/SessionDuration.py` & `opengamedata_core-0.0.6/src/ogd/games/JOWILDER/features/SessionDuration.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # import libraries
 from typing import Any, List, Optional
 from datetime import datetime, timedelta
 from ogd.core.generators.Generator import GeneratorParameters
 # import local files
 from ogd.core.generators.extractors.SessionFeature import SessionFeature
-from ogd.core.schemas.ExtractionMode import ExtractionMode
-from ogd.core.schemas.FeatureData import FeatureData
-from ogd.core.schemas.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
+from ogd.core.models.FeatureData import FeatureData
+from ogd.core.models.Event import Event
 
 # BUG: There may be multiple endgame events with only one startgame event
 
 class SessionDuration(SessionFeature):
     """Template file to serve as a guide for creating custom Feature subclasses for games.
 
     :param Feature: Base class for a Custom Feature class.
```

### Comparing `opengamedata_core-0.0.5/src/ogd/games/JOWILDER/features/SessionStart.py` & `opengamedata_core-0.0.6/src/ogd/games/JOWILDER/features/SessionStart.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # import libraries
 from typing import Any, List, Optional
 from ogd.core.generators.Generator import GeneratorParameters
 from datetime import date, datetime, time
 # import local files
 from ogd.core.generators.extractors.SessionFeature import SessionFeature
-from ogd.core.schemas.ExtractionMode import ExtractionMode
-from ogd.core.schemas.FeatureData import FeatureData
-from ogd.core.schemas.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
+from ogd.core.models.FeatureData import FeatureData
+from ogd.core.models.Event import Event
 
 class SessionStart(SessionFeature):
     """Template file to serve as a guide for creating custom Feature subclasses for games.
 
     :param Feature: Base class for a Custom Feature class.
     :type Feature: _type_
     """
```

### Comparing `opengamedata_core-0.0.5/src/ogd/games/JOWILDER/features/SurveyItem.py` & `opengamedata_core-0.0.6/src/ogd/games/JOWILDER/features/SurveyItem.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 import json
 import logging
 from datetime import datetime, timedelta
 from typing import Any, Dict, Final, List, Optional
 # import local files
 from ogd.core.generators.Generator import GeneratorParameters
 from ogd.core.generators.extractors.PerCountFeature import PerCountFeature
-from ogd.core.schemas.ExtractionMode import ExtractionMode
-from ogd.core.schemas.FeatureData import FeatureData
-from ogd.core.schemas.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
+from ogd.core.models.FeatureData import FeatureData
+from ogd.core.models.Event import Event
 from ogd.core.utils.Logger import Logger
 
 # BUG: Question0 and quiz 0 don't have start time
 # NOTE: Assumptions are: Every quiz should have a quizstart.
 
 QUIZ_INDEXES : Final[Dict[int, Dict[int, int]]] = {
     0: {0: 0, 1: 1},
```

### Comparing `opengamedata_core-0.0.5/src/ogd/games/JOWILDER/features/SurveyTime.py` & `opengamedata_core-0.0.6/src/ogd/games/JOWILDER/features/SurveyTime.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # import libraries
 from datetime import datetime, timedelta
 import json
 from typing import Any, List, Optional
 from ogd.core.generators.Generator import GeneratorParameters
 # import local files
 from ogd.core.generators.extractors.PerCountFeature import PerCountFeature
-from ogd.core.schemas.ExtractionMode import ExtractionMode
-from ogd.core.schemas.FeatureData import FeatureData
-from ogd.core.schemas.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
+from ogd.core.models.FeatureData import FeatureData
+from ogd.core.models.Event import Event
 
 # BUG: quizstart and quizend don't match. Using "wellsdidit" save code to inspect it.
 
 class SurveyTime(PerCountFeature):
     """Template file to serve as a guide for creating custom Feature subclasses for games.
 
     :param Feature: Base class for a Custom Feature class.
```

### Comparing `opengamedata_core-0.0.5/src/ogd/games/JOWILDER/features/UsedContinue.py` & `opengamedata_core-0.0.6/src/ogd/games/JOWILDER/features/UsedContinue.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # import libraries
 from typing import Any, Final, List, Optional
 from ogd.core.generators.Generator import GeneratorParameters
 # import local files
 from ogd.core.generators.extractors.SessionFeature import SessionFeature
-from ogd.core.schemas.ExtractionMode import ExtractionMode
-from ogd.core.schemas.FeatureData import FeatureData
-from ogd.core.schemas.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
+from ogd.core.models.FeatureData import FeatureData
+from ogd.core.models.Event import Event
 
 class UsedContinue(SessionFeature):
     """Template file to serve as a guide for creating custom Feature subclasses for games.
 
     :param Feature: Base class for a Custom Feature class.
     :type Feature: _type_
     """
```

### Comparing `opengamedata_core-0.0.5/src/ogd/games/JOWILDER/features/UsedSaveCode.py` & `opengamedata_core-0.0.6/src/ogd/games/JOWILDER/features/UsedSaveCode.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # import libraries
 from typing import Any, List, Optional
 from ogd.core.generators.Generator import GeneratorParameters
 # import local files
 from ogd.core.generators.extractors.SessionFeature import SessionFeature
-from ogd.core.schemas.ExtractionMode import ExtractionMode
-from ogd.core.schemas.FeatureData import FeatureData
-from ogd.core.schemas.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
+from ogd.core.models.FeatureData import FeatureData
+from ogd.core.models.Event import Event
 
 class UsedSaveCode(SessionFeature):
     """Template file to serve as a guide for creating custom Feature subclasses for games.
 
     :param Feature: Base class for a Custom Feature class.
     :type Feature: _type_
     """
```

### Comparing `opengamedata_core-0.0.5/src/ogd/games/JOWILDER/features/UserEnabled.py` & `opengamedata_core-0.0.6/src/ogd/games/JOWILDER/features/UserEnabled.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # import libraries
 from typing import Any, List, Optional
 from ogd.core.generators.Generator import GeneratorParameters
 # import local files
 from ogd.core.generators.extractors.SessionFeature import SessionFeature
-from ogd.core.schemas.ExtractionMode import ExtractionMode
-from ogd.core.schemas.FeatureData import FeatureData
-from ogd.core.schemas.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
+from ogd.core.models.FeatureData import FeatureData
+from ogd.core.models.Event import Event
 
 class UserEnabled(SessionFeature):
     """Template file to serve as a guide for creating custom Feature subclasses for games.
 
     :param Feature: Base class for a Custom Feature class.
     :type Feature: _type_
     """
```

### Comparing `opengamedata_core-0.0.5/src/ogd/games/JOWILDER/features/__init__.py` & `opengamedata_core-0.0.6/src/ogd/games/JOWILDER/features/__init__.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.5/src/ogd/games/JOWILDER/get_jowilder_all_items.py` & `opengamedata_core-0.0.6/src/ogd/games/JOWILDER/get_jowilder_all_items.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.5/src/ogd/games/JOWILDER/schemas/JOWILDER.json.template` & `opengamedata_core-0.0.6/src/ogd/games/JOWILDER/schemas/JOWILDER.json.template`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.5/src/ogd/games/LAKELAND/LakelandLoader.py` & `opengamedata_core-0.0.6/src/ogd/games/LAKELAND/LakelandLoader.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 ## import local files
 from . import features
 from ogd.core.generators.detectors.Detector import Detector
 from ogd.core.generators.Generator import GeneratorParameters
 from ogd.core.generators.legacy.LegacyLoader import LegacyLoader
 from ogd.core.generators.extractors.Feature import Feature
 from ogd.games.LAKELAND.features.LakelandExtractor import LakelandExtractor
-from ogd.core.schemas.Event import Event
-from ogd.core.schemas.ExtractionMode import ExtractionMode
+from ogd.core.models.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
 from ogd.core.schemas.games.GameSchema import GameSchema
 
 class LakelandLoader(LegacyLoader):
 
     # *** IMPLEMENT ABSTRACT FUNCTIONS ***
 
     def _loadFeature(self, feature_type:str, extractor_params:GeneratorParameters, schema_args:Dict[str,Any]) -> Feature:
```

### Comparing `opengamedata_core-0.0.5/src/ogd/games/LAKELAND/features/ActionsLastXSecondsModel.py` & `opengamedata_core-0.0.6/src/ogd/games/LAKELAND/features/ActionsLastXSecondsModel.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.5/src/ogd/games/LAKELAND/features/DeathCountModel.py` & `opengamedata_core-0.0.6/src/ogd/games/LAKELAND/features/DeathCountModel.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.5/src/ogd/games/LAKELAND/features/DeathPredModel.py` & `opengamedata_core-0.0.6/src/ogd/games/LAKELAND/features/DeathPredModel.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.5/src/ogd/games/LAKELAND/features/DeathThresholdModel.py` & `opengamedata_core-0.0.6/src/ogd/games/LAKELAND/features/DeathThresholdModel.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.5/src/ogd/games/LAKELAND/features/DiagonalFarmDetectorModel.py` & `opengamedata_core-0.0.6/src/ogd/games/LAKELAND/features/DiagonalFarmDetectorModel.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.5/src/ogd/games/LAKELAND/features/FeatSeqPercent.py` & `opengamedata_core-0.0.6/src/ogd/games/LAKELAND/features/FeatSeqPercent.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.5/src/ogd/games/LAKELAND/features/FeatVelocity.py` & `opengamedata_core-0.0.6/src/ogd/games/LAKELAND/features/FeatVelocity.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.5/src/ogd/games/LAKELAND/features/FeatureModel.py` & `opengamedata_core-0.0.6/src/ogd/games/LAKELAND/features/FeatureModel.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.5/src/ogd/games/LAKELAND/features/LAKELAND_models.json` & `opengamedata_core-0.0.6/src/ogd/games/LAKELAND/features/LAKELAND_models.json`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.5/src/ogd/games/LAKELAND/features/LakelandEnumerators.json` & `opengamedata_core-0.0.6/src/ogd/games/LAKELAND/features/LakelandEnumerators.json`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.5/src/ogd/games/LAKELAND/features/LakelandExtractor.py` & `opengamedata_core-0.0.6/src/ogd/games/LAKELAND/features/LakelandExtractor.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,16 +19,16 @@
 from datetime import datetime, timedelta
 from math import sqrt
 from pathlib import Path
 from typing import Any, Dict, List, Optional
 ## import local files
 from ogd.core.generators.Generator import GeneratorParameters
 from ogd.core.generators.legacy.LegacyFeature import LegacyFeature
-from ogd.core.schemas.Event import Event
-from ogd.core.schemas.ExtractionMode import ExtractionMode
+from ogd.core.models.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
 from ogd.core.schemas.games.GameSchema import GameSchema
 from ogd.core.utils import utils
 from ogd.core.utils.Logger import Logger
 
 # temp comment
 
 ## @class LakelandExtractor
```

### Comparing `opengamedata_core-0.0.5/src/ogd/games/LAKELAND/features/LinearModel.py` & `opengamedata_core-0.0.6/src/ogd/games/LAKELAND/features/LinearModel.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.5/src/ogd/games/LAKELAND/features/LogisticModel.py` & `opengamedata_core-0.0.6/src/ogd/games/LAKELAND/features/LogisticModel.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.5/src/ogd/games/LAKELAND/features/MapSummaryModel.py` & `opengamedata_core-0.0.6/src/ogd/games/LAKELAND/features/MapSummaryModel.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.5/src/ogd/games/LAKELAND/features/Model.py` & `opengamedata_core-0.0.6/src/ogd/games/LAKELAND/features/Model.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.5/src/ogd/games/LAKELAND/features/MoneyAccumulationModel.py` & `opengamedata_core-0.0.6/src/ogd/games/LAKELAND/features/MoneyAccumulationModel.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.5/src/ogd/games/LAKELAND/features/PopulationModel.py` & `opengamedata_core-0.0.6/src/ogd/games/LAKELAND/features/PopulationModel.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.5/src/ogd/games/LAKELAND/features/RecentPurchasesModel.py` & `opengamedata_core-0.0.6/src/ogd/games/LAKELAND/features/RecentPurchasesModel.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.5/src/ogd/games/LAKELAND/features/SequenceModel.py` & `opengamedata_core-0.0.6/src/ogd/games/LAKELAND/features/SequenceModel.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.5/src/ogd/games/LAKELAND/features/SimpleFarmAbandonmentModel.py` & `opengamedata_core-0.0.6/src/ogd/games/LAKELAND/features/SimpleFarmAbandonmentModel.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.5/src/ogd/games/LAKELAND/features/SingleFeatureModel.py` & `opengamedata_core-0.0.6/src/ogd/games/LAKELAND/features/SingleFeatureModel.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.5/src/ogd/games/LAKELAND/features/TimeSinceEventTypes.py` & `opengamedata_core-0.0.6/src/ogd/games/LAKELAND/features/TimeSinceEventTypes.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.5/src/ogd/games/LAKELAND/features/TimeSinceLastSaleModel.py` & `opengamedata_core-0.0.6/src/ogd/games/LAKELAND/features/TimeSinceLastSaleModel.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.5/src/ogd/games/LAKELAND/features/TownCompositionModel.py` & `opengamedata_core-0.0.6/src/ogd/games/LAKELAND/features/TownCompositionModel.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.5/src/ogd/games/LAKELAND/features/TutorialProgressionModel.py` & `opengamedata_core-0.0.6/src/ogd/games/LAKELAND/features/TutorialProgressionModel.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.5/src/ogd/games/LAKELAND/features/WAVES_models.json` & `opengamedata_core-0.0.6/src/ogd/games/LAKELAND/features/WAVES_models.json`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.5/src/ogd/games/LAKELAND/features/WAVES_models_L8_Q0_Q1.json` & `opengamedata_core-0.0.6/src/ogd/games/LAKELAND/features/WAVES_models_L8_Q0_Q1.json`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.5/src/ogd/games/LAKELAND/features/WAVES_models_L8_and_Q0.json` & `opengamedata_core-0.0.6/src/ogd/games/LAKELAND/features/WAVES_models_L8_and_Q0.json`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.5/src/ogd/games/LAKELAND/features/WAVES_models_L8_complete_and_current.json` & `opengamedata_core-0.0.6/src/ogd/games/LAKELAND/features/WAVES_models_L8_complete_and_current.json`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.5/src/ogd/games/LAKELAND/features/WAVES_models_L8_only_complete.json` & `opengamedata_core-0.0.6/src/ogd/games/LAKELAND/features/WAVES_models_L8_only_complete.json`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.5/src/ogd/games/LAKELAND/produce_lakeland_enumerators.py` & `opengamedata_core-0.0.6/src/ogd/games/LAKELAND/produce_lakeland_enumerators.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.5/src/ogd/games/LAKELAND/schemas/LAKELAND.json.template` & `opengamedata_core-0.0.6/src/ogd/games/LAKELAND/schemas/LAKELAND.json.template`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.5/src/ogd/games/MAGNET/MagnetLoader.py` & `opengamedata_core-0.0.6/src/ogd/games/MAGNET/MagnetLoader.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 ## import local files
 from . import features
 from ogd.core.generators.detectors.Detector import Detector
 from ogd.core.generators.Generator import GeneratorParameters
 from ogd.core.generators.extractors.Feature import Feature
 from ogd.core.generators.legacy.LegacyLoader import LegacyLoader
 from ogd.games.MAGNET.features.MagnetExtractor import MagnetExtractor
-from ogd.core.schemas.Event import Event
-from ogd.core.schemas.ExtractionMode import ExtractionMode
+from ogd.core.models.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
 from ogd.core.schemas.games.GameSchema import GameSchema
 
 class MagnetLoader(LegacyLoader):
 
     # *** IMPLEMENT ABSTRACT FUNCTIONS ***
 
     def _loadFeature(self, feature_type:str, extractor_params:GeneratorParameters, schema_args:Dict[str,Any]) -> Feature:
```

### Comparing `opengamedata_core-0.0.5/src/ogd/games/MAGNET/features/MagnetExtractor.py` & `opengamedata_core-0.0.6/src/ogd/games/MAGNET/features/MagnetExtractor.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 import logging
 from datetime import datetime
 from typing import Any, Dict, List, Optional
 ## import local files
 from ogd.core.utils.Logger import Logger
 from ogd.core.generators.Generator import GeneratorParameters
 from ogd.core.generators.legacy.LegacyFeature import LegacyFeature
-from ogd.core.schemas.Event import Event
-from ogd.core.schemas.ExtractionMode import ExtractionMode
+from ogd.core.models.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
 from ogd.core.schemas.games.GameSchema import GameSchema
 
 ## @class MagnetExtractor
 #  Extractor subclass for extracting features from Magnet game data.
 class MagnetExtractor(LegacyFeature):
     ## Constructor for the MagnetExtractor class.
     #  Initializes some custom private data (not present in base class) for use
```

### Comparing `opengamedata_core-0.0.5/src/ogd/games/MAGNET/schemas/MAGNET.json.template` & `opengamedata_core-0.0.6/src/ogd/games/MAGNET/schemas/MAGNET.json.template`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.5/src/ogd/games/MASHOPOLIS/schemas/MASHOPOLIS.json.template` & `opengamedata_core-0.0.6/src/ogd/games/MASHOPOLIS/schemas/MASHOPOLIS.json.template`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.5/src/ogd/games/PENGUINS/DBExport.json` & `opengamedata_core-0.0.6/src/ogd/games/PENGUINS/DBExport.json`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.5/src/ogd/games/PENGUINS/PenguinsLoader.py` & `opengamedata_core-0.0.6/src/ogd/games/PENGUINS/PenguinsLoader.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,16 +8,16 @@
 from ogd.core.generators.detectors.Detector import Detector
 from ogd.core.generators.Generator import GeneratorParameters
 from ogd.core.generators.GeneratorLoader import GeneratorLoader
 from ogd.core.generators.extractors.Feature import Feature
 from ogd.games.PENGUINS.detectors import *
 from ogd.games.PENGUINS.features import *
 from ogd.core.generators.Generator import GeneratorParameters
-from ogd.core.schemas.Event import Event
-from ogd.core.schemas.ExtractionMode import ExtractionMode
+from ogd.core.models.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
 from ogd.core.schemas.games.GameSchema import GameSchema
 # from ogd.games.PENGUINS.DBExport import scene_map
 
 ## @class WaveExtractor
 #  Extractor subclass for extracting features from Waves game data.
 
 EXPORT_PATH : Final[str] = "games/PENGUINS/DBExport.json"
@@ -54,58 +54,72 @@
     def _getFeaturesModule():
         return features
     
     def _loadFeature(self, feature_type:str, extractor_params:GeneratorParameters, schema_args:Dict[str,Any]) -> Feature:
         ret_val : Feature
         if extractor_params._count_index == None:
             match feature_type:
-                case "SessionDuration":
-                    ret_val = SessionDuration.SessionDuration(params=extractor_params, session_id=self._session_id)
-                case "RegionsEncountered":
-                    ret_val = RegionsEncountered.RegionsEncountered(params=extractor_params)
-                case "PlayerWaddleCount":
-                    ret_val = PlayerWaddleCount.PlayerWaddleCount(params=extractor_params)
-                case "GazeDuration":
-                    ret_val = GazeDuration.GazeDuration(params=extractor_params)
-                case "GazeCount":
-                    ret_val = GazeCount.GazeCount(params=extractor_params)
-                case "SnowBallDuration":
-                    ret_val = SnowBallDuration.SnowBallDuration(params=extractor_params)
-                # case "RingChimesCount":
-                    # ret_val = RingChimesCount.RingChimesCount(params=extractor_params)
-                case "WaddlePerRegion":
-                    ret_val = WaddlePerRegion.WaddlePerRegion(params=extractor_params, region_map=self._region_map)
+                case "ActivityCompleted":
+                    ret_val = ActivityCompleted.ActivityCompleted(params=extractor_params)
+                case "ActivityDuration":
+                    ret_val = ActivityDuration.ActivityDuration(params=extractor_params)       
+                case "BuiltNestCount":
+                    ret_val = BuiltNestCount.BuiltNestCount(params=extractor_params)
+                case "BuiltWrongNestCount":
+                    ret_val = BuiltWrongNestCount.BuiltWrongNestCount(params=extractor_params)
                 case "EatFishCount":
                     ret_val = EatFishCount.EatFishCount(params=extractor_params)
-                case "PickupRockCount":
-                    ret_val = PickupRockCount.PickupRockCount(params=extractor_params)
                 case "EggLostCount":
                     ret_val = EggLostCount.EggLostCount(params=extractor_params)
                 case "EggRecoverTime":
                     ret_val = EggRecoverTime.EggRecoverTime(params=extractor_params)
-                # case "PlayerInactiveAvgDuration":
-                #     ret_val = PlayerInactiveAvgDuration.PlayerInactiveAvgDuration(params=extractor_params)
+                case "GazeCount":
+                    ret_val = GazeCount.GazeCount(params=extractor_params)
+                case "GazeDuration":
+                    ret_val = GazeDuration.GazeDuration(params=extractor_params)
+                case "LogVersion":
+                    ret_val = LogVersion.LogVersion(params=extractor_params)
                 case "MirrorWaddleDuration":
                     ret_val = MirrorWaddleDuration.MirrorWaddleDuration(params=extractor_params)
-                case "ActivityCompleted":
-                    ret_val = ActivityCompleted.ActivityCompleted(params=extractor_params)
-                case "ActivityDuration":
-                    ret_val = ActivityDuration.ActivityDuration(params=extractor_params)       
+                case "PenguinInteractCount":
+                    ret_val = PenguinInteractCount.PenguinInteractCount(params=extractor_params)
+                # case "PlayerInactiveAvgDuration":
+                #     ret_val = PlayerInactiveAvgDuration.PlayerInactiveAvgDuration(params=extractor_params)
+                case "RegionsEncountered":
+                    ret_val = RegionsEncountered.RegionsEncountered(params=extractor_params)
+                case "RingChimesCount":
+                    ret_val = RingChimesCount.RingChimesCount(params=extractor_params)
+                case "RockBashCount":
+                    ret_val = RockBashCount.RockBashCount(params=extractor_params) 
+                case "RockPickupCount":
+                    ret_val = RockPickupCount.RockPickupCount(params=extractor_params)
+                case "RockMultiplePickupCount":
+                        ret_val = RockMultiplePickupCount.RockMultiplePickupCount(params=extractor_params)      
+                case "SessionDuration":
+                    ret_val = SessionDuration.SessionDuration(params=extractor_params, session_id=self._session_id)
+                case "SkuaBashCount":
+                        ret_val = SkuaBashCount.SkuaBashCount(params=extractor_params)
+                case "SkuaPeckCount":
+                        ret_val = SkuaPeckCount.SkuaPeckCount(params=extractor_params)
+                case "SnowBallDuration":
+                    ret_val = SnowBallDuration.SnowBallDuration(params=extractor_params)
+                case "WaddleCount":
+                    ret_val = WaddleCount.WaddleCount(params=extractor_params)
                 case _:
                     raise NotImplementedError(f"'{feature_type}' is not a valid aggregate feature for Penguins.")
         # Per-count features
         # level attempt features
         else:
             match feature_type:
-                case "RegionEnterCount":
-                        ret_val = RegionEnterCount.RegionEnterCount(params=extractor_params, region_map=self._region_map)
-                # case "WaddlePerRegion":
-                        #ret_val = WaddlePerRegion.WaddlePerRegion(params=extractor_params)
                 case "RegionDuration":
                             ret_val = RegionDuration.RegionDuration(params=extractor_params, region_map=self._region_map)
+                case "RegionEnterCount":
+                        ret_val = RegionEnterCount.RegionEnterCount(params=extractor_params, region_map=self._region_map)
+                case "WaddlePerRegion":
+                    ret_val = WaddlePerRegion.WaddlePerRegion(params=extractor_params, region_map=self._region_map)
                 case _:
                     raise NotImplementedError(f"'{feature_type}' is not a valid per-count feature for Penguins.")
         return ret_val
 
     def _loadDetector(self, detector_type:str, extractor_params:GeneratorParameters, schema_args:Dict[str,Any], trigger_callback:Callable[[Event], None]) -> Detector:
         ret_val : Detector
```

### Comparing `opengamedata_core-0.0.5/src/ogd/games/PENGUINS/features/ActivityCompleted.py` & `opengamedata_core-0.0.6/src/ogd/games/PENGUINS/features/ActivityCompleted.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 # import libraries
 import logging
 from typing import Any, Dict, List, Optional
 # import locals
 from ogd.core.utils.Logger import Logger
 from ogd.core.generators.Generator import GeneratorParameters
 from ogd.core.generators.extractors.Feature import Feature
-from ogd.games.PENGUINS.features.PerRegionFeature import PerRegionFeature
-from ogd.core.schemas.Event import Event
-from ogd.core.schemas.ExtractionMode import ExtractionMode
-from ogd.core.schemas.FeatureData import FeatureData
+from ogd.core.models.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
+from ogd.core.models.FeatureData import FeatureData
 from ogd.core.generators.extractors.SessionFeature import SessionFeature
 
 
 class ActivityCompleted(SessionFeature):
     """Template file to serve as a guide for creating custom Feature subclasses for games.
 
     :param Feature: Base class for a Custom Feature class.
```

### Comparing `opengamedata_core-0.0.5/src/ogd/games/PENGUINS/features/ActivityDuration.py` & `opengamedata_core-0.0.6/src/ogd/games/PENGUINS/features/ActivityDuration.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # import libraries
 import logging
 from typing import Any, List, Optional
 from datetime import datetime, timedelta
 # import locals
 from ogd.core.generators.Generator import GeneratorParameters
 from ogd.core.generators.extractors.SessionFeature import SessionFeature
-from ogd.core.schemas.Event import Event
-from ogd.core.schemas.ExtractionMode import ExtractionMode
-from ogd.core.schemas.FeatureData import FeatureData
+from ogd.core.models.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
+from ogd.core.models.FeatureData import FeatureData
 from ogd.core.utils.Logger import Logger
 
 class ActivityDuration(SessionFeature):
     """Template file to serve as a guide for creating custom Feature subclasses for games.
 
     :param Feature: Base class for a Custom Feature class.
     :type Feature: _type_
```

### Comparing `opengamedata_core-0.0.5/src/ogd/games/PENGUINS/features/EatFishCount.py` & `opengamedata_core-0.0.6/src/ogd/games/PENGUINS/features/RockBashCount.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,39 +1,35 @@
 # import libraries
 import logging
 from typing import Any, Dict, List, Optional
 # import locals
 from ogd.core.utils.Logger import Logger
 from ogd.core.generators.Generator import GeneratorParameters
-from ogd.core.generators.extractors.Feature import Feature
-from ogd.games.PENGUINS.features.PerRegionFeature import PerRegionFeature
-from ogd.core.schemas.Event import Event
-from ogd.core.schemas.ExtractionMode import ExtractionMode
-from ogd.core.schemas.FeatureData import FeatureData
+from ogd.core.models.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
+from ogd.core.models.FeatureData import FeatureData
 from ogd.core.generators.extractors.SessionFeature import SessionFeature
 
 
-class EatFishCount(SessionFeature):
+class RockBashCount(SessionFeature):
 
     def __init__(self, params:GeneratorParameters):
         super().__init__(params=params)
         self._current_count : int = 0
 
     # *** IMPLEMENT ABSTRACT FUNCTIONS ***
     @classmethod
     def _eventFilter(cls, mode:ExtractionMode) -> List[str]:
-        return ["eat_fish"]
+        return ["flipper_bash_rock"]
 
     @classmethod
     def _featureFilter(cls, mode:ExtractionMode) -> List[str]:
         return []
 
     def _updateFromEvent(self, event:Event) -> None:
         self._current_count += 1
 
     def _updateFromFeatureData(self, feature:FeatureData):
         return
 
     def _getFeatureValues(self) -> List[Any]:
         return [self._current_count]
-
-
```

### Comparing `opengamedata_core-0.0.5/src/ogd/games/PENGUINS/features/EggLostCount.py` & `opengamedata_core-0.0.6/src/ogd/games/PENGUINS/features/EatFishCount.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,31 +1,29 @@
 # import libraries
 import logging
 from typing import Any, Dict, List, Optional
 # import locals
 from ogd.core.utils.Logger import Logger
 from ogd.core.generators.Generator import GeneratorParameters
-from ogd.core.generators.extractors.Feature import Feature
-from ogd.games.PENGUINS.features.PerRegionFeature import PerRegionFeature
-from ogd.core.schemas.Event import Event
-from ogd.core.schemas.ExtractionMode import ExtractionMode
-from ogd.core.schemas.FeatureData import FeatureData
+from ogd.core.models.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
+from ogd.core.models.FeatureData import FeatureData
 from ogd.core.generators.extractors.SessionFeature import SessionFeature
 
 
-class EggLostCount(SessionFeature):
+class EatFishCount(SessionFeature):
 
     def __init__(self, params:GeneratorParameters):
         super().__init__(params=params)
         self._current_count : int = 0
 
     # *** IMPLEMENT ABSTRACT FUNCTIONS ***
     @classmethod
     def _eventFilter(cls, mode:ExtractionMode) -> List[str]:
-        return ["egg_lost"]
+        return ["eat_fish"]
 
     @classmethod
     def _featureFilter(cls, mode:ExtractionMode) -> List[str]:
         return []
 
     def _updateFromEvent(self, event:Event) -> None:
         self._current_count += 1
```

### Comparing `opengamedata_core-0.0.5/src/ogd/games/PENGUINS/features/EggRecoverTime.py` & `opengamedata_core-0.0.6/src/ogd/games/SHIPWRECKS/features/MissionSonarTimeToComplete.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,59 +1,42 @@
 # import libraries
-import logging
-from typing import Any, Dict, List, Optional
+from datetime import timedelta
+from typing import Any, List, Optional
 # import locals
-from ogd.core.utils.Logger import Logger
-from datetime import datetime, timedelta
-from ogd.core.generators.Generator import GeneratorParameters
 from ogd.core.generators.extractors.Feature import Feature
-from ogd.games.PENGUINS.features.PerRegionFeature import PerRegionFeature
-from ogd.core.schemas.Event import Event
-from ogd.core.schemas.ExtractionMode import ExtractionMode
-from ogd.core.schemas.FeatureData import FeatureData
-from ogd.core.generators.extractors.SessionFeature import SessionFeature
+from ogd.core.generators.Generator import GeneratorParameters
+from ogd.core.models.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
+from ogd.core.models.FeatureData import FeatureData
 
-class EggRecoverTime(SessionFeature):
 
+class MissionSonarTimeToComplete(Feature):
+    
+    # *** IMPLEMENT ABSTRACT FUNCTIONS ***
     def __init__(self, params:GeneratorParameters):
         super().__init__(params=params)
-        self._session_id = None
-        self._argument_start_time : Optional[datetime] = None
-        self._prev_timestamp = None
-        self._time = 0
-        self._skua_id = None
+        self._sonar_start_time = None
+        self._time = timedelta(0)
 
-    # *** IMPLEMENT ABSTRACT FUNCTIONS ***
     @classmethod
     def _eventFilter(cls, mode:ExtractionMode) -> List[str]:
-        return ["egg_lost", "egg_recovered"]
+        return ["sonar_start", "sonar_exit"]
 
     @classmethod
     def _featureFilter(cls, mode:ExtractionMode) -> List[str]:
         return []
 
     def _updateFromEvent(self, event:Event) -> None:
-        Logger.Log(f"triggered")
-        if event.SessionID != self._session_id:
-            self._session_id = event.SessionID
-            # if we jumped to a new session, we only want to count time up to last event, not the time between sessions.
-            if self._argument_start_time and self._prev_timestamp:
-                self._time += (self._prev_timestamp - self._argument_start_time).total_seconds()
-                self._argument_start_time = event.Timestamp
-
-        if event.EventName == "egg_lost":
-            self._skua_id = event.event_data.get("object_id")
-            self._argument_start_time = event.Timestamp
-            Logger.Log(f"lost time is {self._argument_start_time}")
-        elif event.EventName == "egg_recovered" and self._argument_start_time is not None:
-            self._time = (event.Timestamp - self._argument_start_time).total_seconds()
-            self._argument_start_time = None
-            return
-        self._prev_timestamp = event.Timestamp
-    
+        if event.EventName == "sonar_start":
+            self._sonar_start_time = event.Timestamp
+        elif event.EventName == "sonar_complete":
+            if self._sonar_start_time is not None:
+                self._time += (event.Timestamp - self._sonar_start_time).total_seconds() # TODO : maybe see if we should add timedeltas and convert to float at end?
+                self._sonar_start_time = None
+
     def _updateFromFeatureData(self, feature:FeatureData):
         return
 
     def _getFeatureValues(self) -> List[Any]:
-        return [timedelta(seconds=self._time)]
+        return [self._time]
 
-    
+    # *** Optionally override public functions. ***
```

### Comparing `opengamedata_core-0.0.5/src/ogd/games/PENGUINS/features/GazeCount.py` & `opengamedata_core-0.0.6/src/ogd/games/PENGUINS/features/GazeCount.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 # import libraries
 import logging
 from typing import Any, Dict, List, Optional
 # import locals
 from ogd.core.utils.Logger import Logger
 from ogd.core.generators.Generator import GeneratorParameters
-from ogd.core.generators.extractors.Feature import Feature
-from ogd.games.PENGUINS.features.PerRegionFeature import PerRegionFeature
-from ogd.core.schemas.Event import Event
-from ogd.core.schemas.ExtractionMode import ExtractionMode
-from ogd.core.schemas.FeatureData import FeatureData
+from ogd.core.models.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
+from ogd.core.models.FeatureData import FeatureData
 from ogd.core.generators.extractors.SessionFeature import SessionFeature
 
 # gaze_dict = { 'BigRock00': 0, 'Bridge': 0, 'Bridge2': 0, 'BigRock01': 0, 'River3': 0, 'Inland2': 0, 'Sea4': 0, 'River2': 0,'Inland1': 0, 'Sea5': 0, 'Sea3': 0, 'River5': 0, 'River4': 0, 'Inland5': 0, 'Inland4': 0, 'Inland3': 0,'River1': 0, 'Sea2': 0, 'Sea1': 0}
 class GazeCount(SessionFeature):
 
     def __init__(self, params:GeneratorParameters):
         super().__init__(params=params)
```

### Comparing `opengamedata_core-0.0.5/src/ogd/games/PENGUINS/features/GazeDuration.py` & `opengamedata_core-0.0.6/src/ogd/games/PENGUINS/features/GazeDuration.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # import libraries
 import logging
 from typing import Any, List, Optional
 from datetime import datetime, timedelta
 # import locals
 from ogd.core.generators.Generator import GeneratorParameters
 from ogd.core.generators.extractors.SessionFeature import SessionFeature
-from ogd.core.schemas.Event import Event
-from ogd.core.schemas.ExtractionMode import ExtractionMode
-from ogd.core.schemas.FeatureData import FeatureData
+from ogd.core.models.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
+from ogd.core.models.FeatureData import FeatureData
 from ogd.core.utils.Logger import Logger
 
 class GazeDuration(SessionFeature):
     """Template file to serve as a guide for creating custom Feature subclasses for games.
 
     :param Feature: Base class for a Custom Feature class.
     :type Feature: _type_
```

### Comparing `opengamedata_core-0.0.5/src/ogd/games/PENGUINS/features/MirrorWaddleDuration.py` & `opengamedata_core-0.0.6/src/ogd/games/PENGUINS/features/MirrorWaddleDuration.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 # import libraries
 import logging
 from typing import Any, Dict, List, Optional
 # import locals
 from ogd.core.utils.Logger import Logger
 from datetime import datetime, timedelta
 from ogd.core.generators.Generator import GeneratorParameters
-from ogd.core.generators.extractors.Feature import Feature
-from ogd.games.PENGUINS.features.PerRegionFeature import PerRegionFeature
-from ogd.core.schemas.Event import Event
-from ogd.core.schemas.ExtractionMode import ExtractionMode
-from ogd.core.schemas.FeatureData import FeatureData
+from ogd.core.models.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
+from ogd.core.models.FeatureData import FeatureData
 from ogd.core.generators.extractors.SessionFeature import SessionFeature
 
 class MirrorWaddleDuration(SessionFeature):
     def __init__(self, params:GeneratorParameters):
         super().__init__(params=params)
         self._session_id = None
         self._argument_start_time : Optional[datetime] = None
```

### Comparing `opengamedata_core-0.0.5/src/ogd/games/PENGUINS/features/PickupRockCount.py` & `opengamedata_core-0.0.6/src/ogd/games/AQUALAB/features/TotalGuideCount.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,39 +1,34 @@
 # import libraries
-import logging
-from typing import Any, Dict, List, Optional
+from typing import Any, List
 # import locals
-from ogd.core.utils.Logger import Logger
 from ogd.core.generators.Generator import GeneratorParameters
 from ogd.core.generators.extractors.Feature import Feature
-from ogd.games.PENGUINS.features.PerRegionFeature import PerRegionFeature
-from ogd.core.schemas.Event import Event
-from ogd.core.schemas.ExtractionMode import ExtractionMode
-from ogd.core.schemas.FeatureData import FeatureData
-from ogd.core.generators.extractors.SessionFeature import SessionFeature
+from ogd.core.models.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
+from ogd.core.models.FeatureData import FeatureData
 
-
-class PickupRockCount(SessionFeature):
+class TotalGuideCount(Feature):
 
     def __init__(self, params:GeneratorParameters):
         super().__init__(params=params)
-        self._current_count : int = 0
+        self._count = 0
 
     # *** IMPLEMENT ABSTRACT FUNCTIONS ***
     @classmethod
     def _eventFilter(cls, mode:ExtractionMode) -> List[str]:
-        return ["pickup_rock"]
+        return ["guide_triggered"]
 
     @classmethod
     def _featureFilter(cls, mode:ExtractionMode) -> List[str]:
         return []
 
     def _updateFromEvent(self, event:Event) -> None:
-        self._current_count += 1
+        self._count += 1
 
     def _updateFromFeatureData(self, feature:FeatureData):
         return
 
     def _getFeatureValues(self) -> List[Any]:
-        return [self._current_count]
+        return [self._count]
 
-    
+    # *** Optionally override public functions. ***
```

### Comparing `opengamedata_core-0.0.5/src/ogd/games/PENGUINS/features/PlayerInactiveAvgDuration.py` & `opengamedata_core-0.0.6/src/ogd/games/AQUALAB/features/JobDiveTime.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,64 +1,57 @@
 # import libraries
 import logging
-from typing import Any, Dict, List, Optional
+from datetime import timedelta
+from typing import Any, List, Optional
 # import locals
 from ogd.core.utils.Logger import Logger
-from datetime import datetime, timedelta
 from ogd.core.generators.Generator import GeneratorParameters
-from ogd.core.generators.extractors.Feature import Feature
-from ogd.games.PENGUINS.features.PerRegionFeature import PerRegionFeature
-from ogd.core.schemas.Event import Event
-from ogd.core.schemas.ExtractionMode import ExtractionMode
-from ogd.core.schemas.FeatureData import FeatureData
-from ogd.core.generators.extractors.SessionFeature import SessionFeature
+from ogd.games.AQUALAB.features.PerJobFeature import PerJobFeature
+from ogd.core.models.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
+from ogd.core.models.FeatureData import FeatureData
 
-class PlayerInactiveAvgDuration(SessionFeature):
+class JobDiveTime(PerJobFeature):
 
-    def __init__(self, params:GeneratorParameters):
-        super().__init__(params=params)
+    def __init__(self, params:GeneratorParameters, job_map:dict):
+        super().__init__(params=params, job_map=job_map)
         self._session_id = None
-        self._argument_start_time : Optional[datetime] = None
+        self._dive_start_time = None
         self._prev_timestamp = None
         self._time = 0
-        self._inactive_count = 0
-        self._evt_name = None
-        self._inactive_time_lst = list()
 
     # *** IMPLEMENT ABSTRACT FUNCTIONS ***
     @classmethod
     def _eventFilter(cls, mode:ExtractionMode) -> List[str]:
         return ["all_events"]
 
     @classmethod
     def _featureFilter(cls, mode:ExtractionMode) -> List[str]:
         return []
 
     def _updateFromEvent(self, event:Event) -> None:
         if event.SessionID != self._session_id:
             self._session_id = event.SessionID
             # if we jumped to a new session, we only want to count time up to last event, not the time between sessions.
-            if self._argument_start_time and self._prev_timestamp:
-                self._time += (self._prev_timestamp - self._argument_start_time).total_seconds()
-                self._argument_start_time = event.Timestamp
-        if event.EventName != "viewport_data":
-            if  self._argument_start_time is None :
-                self._evt_name = event.EventName
-                self._argument_start_time = event.Timestamp
-            else:
-                self._time = (event.Timestamp - self._argument_start_time).total_seconds()
-                self._inactive_time_lst.append(self._time)
-                self._argument_start_time = None
+            if self._dive_start_time and self._prev_timestamp:
+                self._time += (self._prev_timestamp - self._dive_start_time).total_seconds()
+                self._dive_start_time = event.Timestamp
+
+        if event.EventName == "begin_dive":
+            self._dive_start_time = event.Timestamp
+        elif event.EventName == "scene_changed":
+            if self._dive_start_time is not None:
+                self._time += (event.Timestamp - self._dive_start_time).total_seconds()
+                self._dive_start_time = None
+
         self._prev_timestamp = event.Timestamp
-    
+
     def _updateFromFeatureData(self, feature:FeatureData):
         return
 
     def _getFeatureValues(self) -> List[Any]:
-        Logger.Log(f"sum is {sum(self._inactive_time_lst)}")
-        Logger.Log(f"length is {len(self._inactive_time_lst)}")
-        if (len(self._inactive_time_lst) != 0):
-            return [sum(self._inactive_time_lst)/len(self._inactive_time_lst)]
-        else:
-            return None
+        return [timedelta(seconds=self._time)]
 
-    
+    # *** Optionally override public functions. ***
+    @staticmethod
+    def MinVersion() -> Optional[str]:
+        return "1"
```

### Comparing `opengamedata_core-0.0.5/src/ogd/games/PENGUINS/features/PlayerWaddleCount.py` & `opengamedata_core-0.0.6/src/ogd/games/PENGUINS/features/SkuaBashCount.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,39 +1,35 @@
 # import libraries
 import logging
 from typing import Any, Dict, List, Optional
 # import locals
 from ogd.core.utils.Logger import Logger
 from ogd.core.generators.Generator import GeneratorParameters
-from ogd.core.generators.extractors.Feature import Feature
-from ogd.games.PENGUINS.features.PerRegionFeature import PerRegionFeature
-from ogd.core.schemas.Event import Event
-from ogd.core.schemas.ExtractionMode import ExtractionMode
-from ogd.core.schemas.FeatureData import FeatureData
+from ogd.core.models.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
+from ogd.core.models.FeatureData import FeatureData
 from ogd.core.generators.extractors.SessionFeature import SessionFeature
 
 
-class PlayerWaddleCount(SessionFeature):
+class SkuaBashCount(SessionFeature):
 
     def __init__(self, params:GeneratorParameters):
         super().__init__(params=params)
         self._current_count : int = 0
 
     # *** IMPLEMENT ABSTRACT FUNCTIONS ***
     @classmethod
     def _eventFilter(cls, mode:ExtractionMode) -> List[str]:
-        return ["player_waddle"]
+        return ["flipper_bash_skua"]
 
     @classmethod
     def _featureFilter(cls, mode:ExtractionMode) -> List[str]:
         return []
 
     def _updateFromEvent(self, event:Event) -> None:
         self._current_count += 1
 
     def _updateFromFeatureData(self, feature:FeatureData):
         return
 
     def _getFeatureValues(self) -> List[Any]:
         return [self._current_count]
-
-
```

### Comparing `opengamedata_core-0.0.5/src/ogd/games/PENGUINS/features/RegionDuration.py` & `opengamedata_core-0.0.6/src/ogd/games/PENGUINS/features/RegionDuration.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 # import libraries
 import json
 from typing import Any, Dict, List
 from datetime import timedelta
 # import local files
 from ogd.core.generators.Generator import GeneratorParameters
 from ogd.core.generators.extractors.PerCountFeature import PerCountFeature
-from ogd.core.schemas.Event import Event
-from ogd.core.schemas.ExtractionMode import ExtractionMode
-from ogd.core.schemas.FeatureData import FeatureData
+from ogd.core.models.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
+from ogd.core.models.FeatureData import FeatureData
 from ogd.core.utils.Logger import Logger
 # import libraries
 import logging
-from ogd.games.PENGUINS.features.PerRegionFeature import PerRegionFeature
+from ogd.games.PENGUINS.features.bases.PerRegionFeature import PerRegionFeature
     
 class RegionDuration(PerRegionFeature):
     
     def __init__(self, params:GeneratorParameters, region_map:List[Dict[str, Any]]):
         super().__init__(params=params,region_map = region_map)
         self._region_start_time = None
         self._time = timedelta(0)
```

### Comparing `opengamedata_core-0.0.5/src/ogd/games/PENGUINS/features/RegionEnterCount.py` & `opengamedata_core-0.0.6/src/ogd/games/WAVES/features/PercentAmplitudeMoves.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,50 +1,39 @@
 # import libraries
-import logging
-from typing import Any, Dict, List, Optional
+from ogd.core.models import Event
+from typing import Any, List, Optional
 # import locals
-from ogd.core.utils.Logger import Logger
-from ogd.core.generators.Generator import GeneratorParameters
 from ogd.core.generators.extractors.Feature import Feature
-from ogd.games.PENGUINS.features.PerRegionFeature import PerRegionFeature
-from ogd.core.schemas.Event import Event
-from ogd.core.schemas.ExtractionMode import ExtractionMode
-from ogd.core.schemas.FeatureData import FeatureData
-from ogd.core.generators.extractors.PerCountFeature import PerCountFeature
-
-
-class RegionEnterCount(PerCountFeature):
-
-    def __init__(self, params:GeneratorParameters, region_map:List[Dict[str, Any]]):
-        super().__init__(params=params)
-        self._region_map = region_map
-        self._current_count : int = 0
+from ogd.core.generators.extractors.PerLevelFeature import PerLevelFeature
+from ogd.core.generators.Generator import GeneratorParameters
+from ogd.core.models.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
+from ogd.core.models.FeatureData import FeatureData
+
+class PercentAmplitudeMoves(PerLevelFeature):
+    def __init__(self, params:GeneratorParameters):
+        Feature.__init__(self, params=params)
+        self._amplitude_count = 0
+        self._count = 0
 
     # *** IMPLEMENT ABSTRACT FUNCTIONS ***
     @classmethod
     def _eventFilter(cls, mode:ExtractionMode) -> List[str]:
-        return ["enter_region"]
+        return ["CUSTOM.1", "CUSTOM.2"]
+        # return ["SLIDER_MOVE_RELEASE", "ARROW_MOVE_RELEASE"]
 
     @classmethod
     def _featureFilter(cls, mode:ExtractionMode) -> List[str]:
         return []
 
     def _updateFromEvent(self, event:Event) -> None:
-        self._current_count += 1
+        self._count += 1
+        if event.EventData['slider'].upper() == 'AMPLITUDE':
+            self._amplitude_count += 1
 
     def _updateFromFeatureData(self, feature:FeatureData):
         return
 
     def _getFeatureValues(self) -> List[Any]:
-        return [self._current_count]
+        return [self._amplitude_count / self._count if self._count != 0 else None]
 
     # *** Optionally override public functions. ***
-    def _validateEventCountIndex(self, event: Event):
-        ret_val : bool = False
-        region_data = event.EventData.get("region_name")
-        if region_data is not None:
-            if region_data in region_map and region_map[region_data] == self.CountIndex:
-                ret_val = True
-        else:
-            self.WarningMessage(f"Got invalid region data in {type(self).__name__}")
-
-        return ret_val
```

### Comparing `opengamedata_core-0.0.5/src/ogd/games/PENGUINS/features/RegionsEncountered.py` & `opengamedata_core-0.0.6/src/ogd/games/WAVES/features/PersistentSessionID.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,39 +1,37 @@
 # import libraries
-import logging
-from typing import Any, Dict, List, Optional
+from ogd.core.models import Event
+from typing import Any, List, Optional
 # import locals
-from ogd.core.utils.Logger import Logger
-from ogd.core.generators.Generator import GeneratorParameters
-from ogd.core.generators.extractors.Feature import Feature
 from ogd.core.generators.extractors.SessionFeature import SessionFeature
-from ogd.core.schemas.Event import Event
-from ogd.core.schemas.ExtractionMode import ExtractionMode
-from ogd.core.schemas.FeatureData import FeatureData
-
-class RegionsEncountered(SessionFeature):
+from ogd.core.generators.Generator import GeneratorParameters
+from ogd.core.models.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
+from ogd.core.models.FeatureData import FeatureData
 
+class PersistentSessionID(SessionFeature):
     def __init__(self, params:GeneratorParameters):
-        super().__init__(params=params)
-        #self._scene_name = None
-        self._cnt_list = list()
+        SessionFeature.__init__(self, params=params)
+        self._persistent_id : Optional[int] = None
 
     # *** IMPLEMENT ABSTRACT FUNCTIONS ***
     @classmethod
     def _eventFilter(cls, mode:ExtractionMode) -> List[str]:
-        return ["region_enter"]
+        return ["BEGIN.0"]
 
     @classmethod
     def _featureFilter(cls, mode:ExtractionMode) -> List[str]:
         return []
 
     def _updateFromEvent(self, event:Event) -> None:
-        self._object_id = event.event_data.get("region")
-        self._cnt_list.append(self._object_id)
+        if self._persistent_id is None:
+            self._persistent_id = event.UserData['persistent_session_id']
 
     def _updateFromFeatureData(self, feature:FeatureData):
         return
 
     def _getFeatureValues(self) -> List[Any]:
-        return [self._cnt_list]
+        return [self._persistent_id]
 
     # *** Optionally override public functions. ***
+
+
```

### Comparing `opengamedata_core-0.0.5/src/ogd/games/PENGUINS/features/RingChimesCount.py` & `opengamedata_core-0.0.6/src/ogd/games/PENGUINS/features/RingChimesCount.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 # import libraries
 import logging
 from typing import Any, Dict, List, Optional
 # import locals
 from ogd.core.utils.Logger import Logger
 from ogd.core.generators.Generator import GeneratorParameters
-from ogd.core.generators.extractors.Feature import Feature
-from ogd.games.PENGUINS.features.PerRegionFeature import PerRegionFeature
-from ogd.core.schemas.Event import Event
-from ogd.core.schemas.ExtractionMode import ExtractionMode
-from ogd.core.schemas.FeatureData import FeatureData
+from ogd.core.models.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
+from ogd.core.models.FeatureData import FeatureData
 from ogd.core.generators.extractors.SessionFeature import SessionFeature
 
-chime_dict = {'chime 1':0, 'chime 2':0, 'chime 3':0, 'chime 4':0, 'chime 5':0, 'chime 6':0}
+chime_dict = {'chime 1':0, 'chime 2':0, 'chime 3':0, 'chime 4':0, 'chime 5':0, 'chime 6':0, 'unknown chime':0}
 class RingChimesCount(SessionFeature):
 
     def __init__(self, params:GeneratorParameters):
         super().__init__(params=params)
         self._current_count : int = 0
         self._object_id = None
         self._chime_dict = chime_dict.copy()
@@ -28,16 +26,16 @@
 
     @classmethod
     def _featureFilter(cls, mode:ExtractionMode) -> List[str]:
         return []
 
     def _updateFromEvent(self, event:Event) -> None:
         # self._current_count += 1
-        self._object_id = event.event_data.get("note_played")
-        self._chime_dict[self._object_id]+=1
+        self._object_id = event.event_data.get("note_played", "unknown chime")
+        self._chime_dict[self._object_id] += 1
         
     def _updateFromFeatureData(self, feature:FeatureData):
         return
 
     def _getFeatureValues(self) -> List[Any]:
         return [self._chime_dict]
```

### Comparing `opengamedata_core-0.0.5/src/ogd/games/PENGUINS/features/SnowBallDuration.py` & `opengamedata_core-0.0.6/src/ogd/games/PENGUINS/features/PlayerInactiveAvgDuration.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,53 +1,62 @@
 # import libraries
 import logging
 from typing import Any, Dict, List, Optional
 # import locals
 from ogd.core.utils.Logger import Logger
 from datetime import datetime, timedelta
 from ogd.core.generators.Generator import GeneratorParameters
-from ogd.core.generators.extractors.Feature import Feature
-from ogd.games.PENGUINS.features.PerRegionFeature import PerRegionFeature
-from ogd.core.schemas.Event import Event
-from ogd.core.schemas.ExtractionMode import ExtractionMode
-from ogd.core.schemas.FeatureData import FeatureData
+from ogd.core.models.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
+from ogd.core.models.FeatureData import FeatureData
 from ogd.core.generators.extractors.SessionFeature import SessionFeature
 
-class SnowBallDuration(SessionFeature):
+class PlayerInactiveAvgDuration(SessionFeature):
 
     def __init__(self, params:GeneratorParameters):
         super().__init__(params=params)
         self._session_id = None
         self._argument_start_time : Optional[datetime] = None
         self._prev_timestamp = None
         self._time = 0
+        self._inactive_count = 0
+        self._evt_name = None
+        self._inactive_time_lst = list()
 
     # *** IMPLEMENT ABSTRACT FUNCTIONS ***
     @classmethod
     def _eventFilter(cls, mode:ExtractionMode) -> List[str]:
-        return ["push_snowball"]
+        return ["all_events"]
 
     @classmethod
     def _featureFilter(cls, mode:ExtractionMode) -> List[str]:
         return []
 
     def _updateFromEvent(self, event:Event) -> None:
         if event.SessionID != self._session_id:
             self._session_id = event.SessionID
             # if we jumped to a new session, we only want to count time up to last event, not the time between sessions.
             if self._argument_start_time and self._prev_timestamp:
                 self._time += (self._prev_timestamp - self._argument_start_time).total_seconds()
                 self._argument_start_time = event.Timestamp
-
-        elif event.EventName == "push_snowball" and self._argument_start_time is not None:
-            self._time = (event.Timestamp - self._argument_start_time).total_seconds()
-            self._argument_start_time = None
-            return
+        if event.EventName != "viewport_data":
+            if  self._argument_start_time is None :
+                self._evt_name = event.EventName
+                self._argument_start_time = event.Timestamp
+            else:
+                self._time = (event.Timestamp - self._argument_start_time).total_seconds()
+                self._inactive_time_lst.append(self._time)
+                self._argument_start_time = None
         self._prev_timestamp = event.Timestamp
     
     def _updateFromFeatureData(self, feature:FeatureData):
         return
 
     def _getFeatureValues(self) -> List[Any]:
-        return [timedelta(seconds=self._time)]
+        Logger.Log(f"sum is {sum(self._inactive_time_lst)}")
+        Logger.Log(f"length is {len(self._inactive_time_lst)}")
+        if (len(self._inactive_time_lst) != 0):
+            return [sum(self._inactive_time_lst)/len(self._inactive_time_lst)]
+        else:
+            return [None]
```

### Comparing `opengamedata_core-0.0.5/src/ogd/games/PENGUINS/features/WaddlePerRegion.py` & `opengamedata_core-0.0.6/src/ogd/games/PENGUINS/features/WaddlePerRegion.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 # import libraries
 import logging
 from typing import Any, Dict, List, Optional
 # import locals
 from ogd.core.utils.Logger import Logger
 from ogd.core.generators.Generator import GeneratorParameters
 from ogd.core.generators.extractors.Feature import Feature
-from ogd.games.PENGUINS.features.PerRegionFeature import PerRegionFeature
-from ogd.core.schemas.Event import Event
-from ogd.core.schemas.ExtractionMode import ExtractionMode
-from ogd.core.schemas.FeatureData import FeatureData
+from ogd.games.PENGUINS.features.bases.PerRegionFeature import PerRegionFeature
+from ogd.core.models.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
+from ogd.core.models.FeatureData import FeatureData
 from ogd.core.generators.extractors.SessionFeature import SessionFeature
 
 class WaddlePerRegion(PerRegionFeature):
 
     def __init__(self, params:GeneratorParameters, region_map:List[Dict[str, Any]]):
         super().__init__(params=params, region_map = region_map)
         self._waddle_count : int = 0
```

### Comparing `opengamedata_core-0.0.5/src/ogd/games/PENGUINS/features/__init__.py` & `opengamedata_core-0.0.6/src/ogd/games/PENGUINS/features/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,43 +1,61 @@
 __all__ = [
-    "SessionDuration",
-    "RegionsEncountered",
-    "RegionEnterCount",
-    "PlayerWaddleCount",
-    "GazeDuration",
-    "GazeCount",
-    "SnowBallDuration",
-    # "RingChimesCount",
-    "WaddlePerRegion",
+    "ActivityCompleted",
+    "ActivityDuration",
+    "BuiltNestCount",
+    "BuiltWrongNestCount",
     "EatFishCount",
-    "PickupRockCount",
     "EggLostCount",
     "EggRecoverTime",
-    "PlayerInactiveAvgDuration",
+    "GazeCount",
+    "GazeDuration",
+    "LogVersion",
     "MirrorWaddleDuration",
-    "WaddlePerRegion",
+    "PenguinInteractCount",
+    "PlayerInactiveAvgDuration",
     "RegionDuration",
-    "ActivityCompleted",
-    "ActivityDuration"
+    "RegionEnterCount",
+    "RegionsEncountered",
+    "RingChimesCount",
+    "RockBashCount",
+    "RockMultiplePickupCount",
+    "RockPickupCount",
+    "SessionDuration",
+    "SkuaBashCount",
+    "SkuaPeckCount",
+    "SnowBallDuration",
+    "WaddleCount",
+    "WaddlePerRegion",
+    "WaddlePerRegion"
 ]
 # aggregated features
 
-from . import SessionDuration
-from . import RegionsEncountered
-from . import PlayerWaddleCount
-from . import GazeDuration
-from . import GazeCount
-from . import SnowBallDuration
-from . import RingChimesCount
+from . import BuiltNestCount
+from . import BuiltWrongNestCount
 from . import EatFishCount
-from . import PickupRockCount
 from . import EggLostCount
 from . import EggRecoverTime
-from . import PlayerInactiveAvgDuration
+from . import GazeCount
+from . import GazeDuration
+from . import LogVersion
 from . import MirrorWaddleDuration
+from . import PenguinInteractCount
+from . import PlayerInactiveAvgDuration
+from . import RegionsEncountered
+from . import RingChimesCount
+from . import RockBashCount
+from . import RockMultiplePickupCount
+from . import RockPickupCount
+from . import SessionDuration
+from . import SkuaBashCount
+from . import SkuaPeckCount
+from . import SnowBallDuration
+from . import WaddleCount
+
 # percount features
-from . import RegionEnterCount
-from . import WaddlePerRegion
-from . import RegionDuration
 from . import ActivityCompleted
 from . import ActivityDuration
+from . import RegionDuration
+from . import RegionEnterCount
+from . import WaddlePerRegion
+
```

### Comparing `opengamedata_core-0.0.5/src/ogd/games/PENGUINS/schemas/PENGUINS.json.template` & `opengamedata_core-0.0.6/src/ogd/games/PENGUINS/schemas/PENGUINS.json.template`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9812770160147392%*

 * *Differences: {"'events'": "{'flipper_bash_nest': {'event_data': {'hand': {'type': 'List[float]', 'description': "*

 * *             "'The position of the nest the player bashed'}}}}",*

 * * "'features'": "{'per_count': {'RegionEnterCount': OrderedDict([('type', 'RegionEnterCount'), "*

 * *               "('enabled', False), ('description', 'The number of times a player enterd for a "*

 * *               "given region of the game.'), ('return_type', 'int')])}, 'aggregate': "*

 * *               "{'LogVersion': OrderedDict([('type', 'LogVersion') […]*

```diff
@@ -167,16 +167,16 @@
                 }
             }
         },
         "flipper_bash_nest": {
             "description": "An event triggered when the player makes a flipper-bashing move and makes contact with a nest.",
             "event_data": {
                 "hand": {
-                    "description": "Whether the player performed the bash with their right or left hand.",
-                    "type": "Hand"
+                    "description": "The position of the nest the player bashed",
+                    "type": "List[float]"
                 },
                 "nest_id": {
                     "description": "The name of the nest object the player bashed",
                     "type": "str"
                 },
                 "nest_pos": {
                     "description": "The position of the nest the player bashed",
@@ -605,66 +605,126 @@
             },
             "ActivityDuration": {
                 "description": "How long activity last for.",
                 "enabled": true,
                 "return_type": "int",
                 "type": "ActivityDuration"
             },
+            "BuiltNestCount": {
+                "description": "The number of times a player with a rock placed the rock on the correct nest.",
+                "enabled": true,
+                "return_type": "int",
+                "type": "BuiltNestCount"
+            },
+            "BuiltWrongNestCount": {
+                "description": "The number of times a player with a rock that has a peck_nest event, where nest_id does not equal to player nest_id.",
+                "enabled": true,
+                "return_type": "int",
+                "type": "BuiltWrongNestCount"
+            },
+            "EggLostCount": {
+                "description": "The number of times a player's egg was stolen by skuas",
+                "enabled": true,
+                "return_type": "int",
+                "type": "EggLostCount"
+            },
+            "EggRecoverTime": {
+                "description": "The amount of time the egg spent stolen, with the player trying to recover it",
+                "enabled": true,
+                "return_type": "int",
+                "type": "EggRecoverTime"
+            },
             "GazeCount": {
                 "description": "The number of times a player waddled in a given region of the game.",
                 "enabled": true,
                 "return_type": "int",
                 "type": "GazeCount"
             },
             "GazeDuration": {
                 "description": "How long gaze event last for.",
                 "enabled": true,
                 "return_type": "timedelta",
                 "type": "GazeDuration"
             },
-            "PickupRockCount": {
-                "description": "The duration each session took.",
+            "LogVersion": {
+                "description": "The version of game the player use.",
                 "enabled": true,
                 "return_type": "int",
-                "type": "PickupRockCount"
+                "type": "LogVersion"
             },
-            "PlayerWaddleCount": {
-                "description": "The number of times a player waddled.",
+            "PenguinInteractCount": {
+                "description": "The number of times a player interacted with another penguin via pecks and/or flipper bashes",
                 "enabled": true,
                 "return_type": "int",
-                "type": "PlayerWaddleCount"
-            },
-            "RegionEnterCount": {
-                "description": "The number of times a player enterd for a given region of the game.",
-                "enabled": false,
-                "return_type": "int",
-                "type": "RegionEnterCount"
+                "type": "PenguinInteractCount"
             },
             "RegionsEncountered": {
                 "description": "The regions entered in a given session.",
                 "enabled": true,
                 "return_type": "int",
                 "type": "RegionsEncountered"
             },
+            "RockBashCount": {
+                "description": "he number of times a player had a flipper_bash_rock event.",
+                "enabled": true,
+                "return_type": "int",
+                "type": "RockBashCount"
+            },
+            "RockMultiplePickupCount": {
+                "description": "The number of times a player with a rock has peck_rock event.",
+                "enabled": true,
+                "return_type": "int",
+                "type": "RockMultiplePickupCount"
+            },
+            "RockPickupCount": {
+                "description": "The duration each session took.",
+                "enabled": true,
+                "return_type": "int",
+                "type": "RockPickupCount"
+            },
             "SessionDuration": {
                 "description": "The duration each session took.",
                 "enabled": true,
                 "return_type": "timedelta",
                 "type": "SessionDuration"
+            },
+            "SkuaBashCount": {
+                "description": "The number of times a player bashed skuas",
+                "enabled": true,
+                "return_type": "int",
+                "type": "SkuaBashCount"
+            },
+            "SkuaPeckCount": {
+                "description": "The number of times a player pecked skuas, which does not actually affect the skuas",
+                "enabled": true,
+                "return_type": "int",
+                "type": "SkuaPeckCount"
+            },
+            "WaddleCount": {
+                "description": "The number of times a player waddled.",
+                "enabled": true,
+                "return_type": "int",
+                "type": "WaddleCount"
             }
         },
         "per_count": {
             "RegionDuration": {
                 "count": 11,
                 "description": "The duration of time a player played in a given region of the game.",
                 "enabled": true,
                 "prefix": "region",
                 "return_type": "timedelta",
                 "type": "RegionDuration"
             },
+            "RegionEnterCount": {
+                "description": "The number of times a player enterd for a given region of the game.",
+                "enabled": false,
+                "return_type": "int",
+                "type": "RegionEnterCount"
+            },
             "WaddlePerRegion": {
                 "count": 11,
                 "description": "The number of times a player waddled in a given region of the game.",
                 "enabled": true,
                 "prefix": "region",
                 "return_type": "int",
                 "type": "WaddlePerRegion"
```

### Comparing `opengamedata_core-0.0.5/src/ogd/games/SHADOWSPECT/ShadowspectLoader.py` & `opengamedata_core-0.0.6/src/ogd/games/SHADOWSPECT/ShadowspectLoader.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 from . import features
 from ogd.core.generators.detectors.Detector import Detector
 from ogd.core.generators.Generator import GeneratorParameters
 from ogd.core.generators.GeneratorLoader import GeneratorLoader
 from ogd.core.generators.extractors.Feature import Feature
 from ogd.core.generators.Generator import GeneratorParameters
 from ogd.games.SHADOWSPECT.features import *
-from ogd.core.schemas.Event import Event
-from ogd.core.schemas.ExtractionMode import ExtractionMode
+from ogd.core.models.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
 from ogd.core.schemas.games.GameSchema import GameSchema
 
 ## @class ShadowspectExtractor
 #  Extractor subclass for extracting features from Shadowspects game data.
 class ShadowspectLoader(GeneratorLoader):
 
     # *** IMPLEMENT ABSTRACT FUNCTIONS ***
@@ -31,14 +31,16 @@
                 ret_val = SessionID.SessionID(params=extractor_params, session_id=self._session_id)
             case "FunnelByUser":
                 ret_val = FunnelByUser.FunnelByUser(params=extractor_params)
             case "LevelsOfDifficulty":
                 ret_val = LevelsOfDifficulty.LevelsOfDifficulty(params=extractor_params)
             case "SequenceBetweenPuzzles":
                 ret_val = SequenceBetweenPuzzles.SequenceBetweenPuzzles(params=extractor_params)
+            case "SequenceWithinPuzzles":
+                ret_val = SequenceWithinPuzzles.SequenceWithinPuzzles(params=extractor_params)
             case _:
                 raise NotImplementedError(f"'{feature_type}' is not a valid feature for Shadowspect.")
         return ret_val
 
     def _loadDetector(self, detector_type:str, name:str, detector_args:Dict[str,Any], trigger_callback:Callable[[Event], None], count_index:Optional[int] = None) -> Detector:
         raise NotImplementedError(f"'{detector_type}' is not a valid detector for Shadowspect.")
```

### Comparing `opengamedata_core-0.0.5/src/ogd/games/SHADOWSPECT/features/FunnelByUser.py` & `opengamedata_core-0.0.6/src/ogd/games/SHADOWSPECT/features/FunnelByUser.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # import libraries
 from typing import Any, List
 import json
 # import locals
 from ogd.core.generators.Generator import GeneratorParameters
 from ogd.core.generators.extractors.SessionFeature import SessionFeature
-from ogd.core.schemas.Event import Event
-from ogd.core.schemas.ExtractionMode import ExtractionMode
-from ogd.core.schemas.FeatureData import FeatureData
+from ogd.core.models.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
+from ogd.core.models.FeatureData import FeatureData
 
 class FunnelByUser(SessionFeature):
     def __init__(self, params:GeneratorParameters):
         super().__init__(params=params)
         self._count = 0
         self._level = None
         self._userFunnelDict = dict()
@@ -22,30 +22,33 @@
 
     @classmethod
     def _featureFilter(cls, mode:ExtractionMode) -> List[str]:
         return []
 
     def _updateFromEvent(self, event:Event) -> None:
         if event.EventName in ["start_level", "puzzle_started"]:
-            self._level = event.EventData["task_id"]
+            self._level = event.EventData.get("task_id")
+            if isinstance(self._level, dict):
+                self._level = self._level["string_value"]
 
             if self._level not in self._userFunnelDict.keys():
-                self._userFunnelDict[self._level] = json.loads('{"started": 0, "create_shape": 0, "submitted": 0, "completed": 0}')
+                self._userFunnelDict[self._level] = {"started": 0, "create_shape": 0, "submitted": 0, "completed": 0}
 
-        if event.EventName == "puzzle_started":
-            self._userFunnelDict[self._level]["started"] = 1
+        if self._level != None:
+            if event.EventName == "puzzle_started":
+                self._userFunnelDict[self._level]["started"] = 1
 
-        elif event.EventName == "create_shape":
-            self._userFunnelDict[self._level]["create_shape"] = 1
+            elif event.EventName == "create_shape":
+                self._userFunnelDict[self._level]["create_shape"] = 1
 
-        elif event.EventName == "check_solution":
-            self._userFunnelDict[self._level]["submitted"] = 1
+            elif event.EventName == "check_solution":
+                self._userFunnelDict[self._level]["submitted"] = 1
 
-        elif event.EventName == "puzzle_complete":
-            self._userFunnelDict[self._level]["completed"] = 1
+            elif event.EventName == "puzzle_complete":
+                self._userFunnelDict[self._level]["completed"] = 1
 
     def _updateFromFeatureData(self, feature:FeatureData):
         return
 
     def _getFeatureValues(self) -> List[Any]:
         count = 0
         finalList = []
@@ -60,7 +63,8 @@
         listReturn.append(sum([x[2] for x in finalList]))
         listReturn.append(sum([x[3] for x in finalList]))
         return listReturn
         
     # *** Optionally override public functions. ***
     def Subfeatures(self) -> List[str]:
         return ["started", "create_shape", "submitted", "completed"]
+
```

### Comparing `opengamedata_core-0.0.5/src/ogd/games/SHADOWSPECT/features/LevelsOfDifficulty.py` & `opengamedata_core-0.0.6/src/ogd/games/SHADOWSPECT/features/LevelsOfDifficulty.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,18 +6,18 @@
 import json
 import hashlib
 from datetime import datetime
 from datetime import timedelta
 from collections import OrderedDict
 # import locals
 from ogd.core.generators.Generator import GeneratorParameters
-from ogd.core.schemas.FeatureData import FeatureData
 from ogd.core.generators.extractors.SessionFeature import SessionFeature
-from ogd.core.schemas.Event import Event
-from ogd.core.schemas.ExtractionMode import ExtractionMode
+from ogd.core.models.FeatureData import FeatureData
+from ogd.core.models.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
 
 pd.options.mode.chained_assignment = None  # default='warn'
     
 listActionEvents = ['move_shape', 'rotate_shape', 'scale_shape',
                     'check_solution', 'undo_action', 'redo_action',
                     'rotate_view', 'snapshot', 'mode_change',
                     'create_shape', 'select_shape', 'delete_shape', 'select_shape_add']
```

### Comparing `opengamedata_core-0.0.5/src/ogd/games/SHADOWSPECT/features/MoveShapeCount.py` & `opengamedata_core-0.0.6/src/ogd/games/SHIPWRECKS/features/EvidenceBoardCompleteCount.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 # import libraries
-from typing import Any, List
+from typing import Any, List, Optional
 # import locals
 from ogd.core.generators.extractors.Feature import Feature
 from ogd.core.generators.Generator import GeneratorParameters
-from ogd.core.schemas.Event import Event
-from ogd.core.schemas.ExtractionMode import ExtractionMode
-from ogd.core.schemas.FeatureData import FeatureData
+from ogd.core.models.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
+from ogd.core.models.FeatureData import FeatureData
 
+class EvidenceBoardCompleteCount(Feature):
 
-class MoveShapeCount(Feature):
     def __init__(self, params:GeneratorParameters):
         super().__init__(params=params)
         self._count = 0
 
     # *** IMPLEMENT ABSTRACT FUNCTIONS ***
     @classmethod
     def _eventFilter(cls, mode:ExtractionMode) -> List[str]:
-        return ["move_shape"]
+        return ["evidence_board_complete"]
 
     @classmethod
     def _featureFilter(cls, mode:ExtractionMode) -> List[str]:
         return []
 
     def _updateFromEvent(self, event:Event) -> None:
         self._count += 1
 
     def _updateFromFeatureData(self, feature:FeatureData):
         return
 
     def _getFeatureValues(self) -> List[Any]:
         return [self._count]
 
-    # *** Optionally override public functions. ***
+    # *** Optionally override public functions. ***
```

### Comparing `opengamedata_core-0.0.5/src/ogd/games/SHADOWSPECT/features/SequenceBetweenPuzzles.py` & `opengamedata_core-0.0.6/src/ogd/games/SHADOWSPECT/features/SequenceBetweenPuzzles.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # import libraries
 from typing import Any, List
 import json
 # import locals
 from ogd.core.generators.Generator import GeneratorParameters
 from ogd.core.generators.extractors.SessionFeature import SessionFeature
-from ogd.core.schemas.Event import Event
-from ogd.core.schemas.ExtractionMode import ExtractionMode
-from ogd.core.schemas.FeatureData import FeatureData
+from ogd.core.models.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
+from ogd.core.models.FeatureData import FeatureData
 
 
 orderMapping = {'1. One Box': 1, '2. Separated Boxes': 2, '3. Rotate a Pyramid': 3, '4. Match Silhouettes': 4, '5. Removing Objects': 5, '6. Stretch a Ramp': 6, '7. Max 2 Boxes': 7, '8. Combine 2 Ramps': 8, '9. Scaling Round Objects': 9,
                 'Square Cross-Sections': 10, 'Bird Fez': 11, 'Pi Henge': 12, '45-Degree Rotations': 13,  'Pyramids are Strange': 14, 'Boxes Obscure Spheres': 15, 'Object Limits': 16, 'Warm Up': 17, 'Angled Silhouette': 18,
                 'Sugar Cones': 19,'Stranger Shapes': 20, 'Tall and Small': 21, 'Ramp Up and Can It': 22, 'More Than Meets Your Eye': 23, 'Not Bird': 24, 'Unnecesary': 25, 'Zzz': 26, 'Bull Market': 27, 'Few Clues': 28, 'Orange Dance': 29, 'Bear Market': 30}
 listPuzzles = list(orderMapping.keys())
 
@@ -59,16 +59,16 @@
                 self._currentPuzzle["funnel"] = "shape_created"
 
             elif event.EventName == "check_solution":
                 self._currentPuzzle["funnel"] = "submitted"
 
             elif event.EventName == "puzzle_complete":
                 self._currentPuzzle["funnel"] = "completed"
-                
-            elif event.EventName in ["disconnect", "login_user", "exit_to_menu"]:
+
+            elif event.event_name in ["disconnect", "login_user", "exit_to_menu"] and self._activePuzzle != None:
                 #Add current data
                 self._userPuzzleDict[self._activePuzzle].append(json.dumps(self._currentPuzzle))
                 self._currentPuzzle = {}
                 self._numPuzzles += 1
 
     def _updateFromFeatureData(self, feature:FeatureData):
         return
```

### Comparing `opengamedata_core-0.0.5/src/ogd/games/SHADOWSPECT/features/SessionID.py` & `opengamedata_core-0.0.6/src/ogd/games/AQUALAB/features/EchoSessionID.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 # import libraries
 from typing import Any, List
 # import locals
 from ogd.core.generators.Generator import GeneratorParameters
 from ogd.core.generators.extractors.SessionFeature import SessionFeature
-from ogd.core.schemas.Event import Event
-from ogd.core.schemas.ExtractionMode import ExtractionMode
-from ogd.core.schemas.FeatureData import FeatureData
+from ogd.core.models.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
+from ogd.core.models.FeatureData import FeatureData
 
+class EchoSessionID(SessionFeature):
 
-class SessionID(SessionFeature):
-    def __init__(self, params:GeneratorParameters, session_id:str):
-        self._session_id = session_id
+    def __init__(self, params:GeneratorParameters):
         super().__init__(params=params)
+        self._session_id = None
 
     # *** IMPLEMENT ABSTRACT FUNCTIONS ***
     @classmethod
     def _eventFilter(cls, mode:ExtractionMode) -> List[str]:
         return []
 
     @classmethod
     def _featureFilter(cls, mode:ExtractionMode) -> List[str]:
-        return []
+        return ["SessionID"]
 
     def _updateFromEvent(self, event:Event) -> None:
         return
 
     def _updateFromFeatureData(self, feature:FeatureData):
-        return
+        self._session_id = feature.FeatureValues[0]
 
     def _getFeatureValues(self) -> List[Any]:
-        return [self._session_id]
+        return [f"The sess ID is: {self._session_id}"]
 
     # *** Optionally override public functions. ***
```

### Comparing `opengamedata_core-0.0.5/src/ogd/games/SHADOWSPECT/schemas/SHADOWSPECT.json.template` & `opengamedata_core-0.0.6/src/ogd/games/SHADOWSPECT/schemas/SHADOWSPECT.json.template`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.5/src/ogd/games/SHIPWRECKS/ShipwrecksLoader.py` & `opengamedata_core-0.0.6/src/ogd/games/SHIPWRECKS/ShipwrecksLoader.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 from . import features
 from ogd.core.generators.detectors.Detector import Detector
 from ogd.core.generators.Generator import GeneratorParameters
 from ogd.core.generators.GeneratorLoader import GeneratorLoader
 from ogd.core.generators.extractors.Feature import Feature
 from ogd.games.SHIPWRECKS.features import *
 from ogd.core.generators.Generator import GeneratorParameters
-from ogd.core.schemas.Event import Event
-from ogd.core.schemas.ExtractionMode import ExtractionMode
+from ogd.core.models.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
 from ogd.core.schemas.games.GameSchema import GameSchema
 
 ## @class ShipwrecksLoader
 #  Extractor subclass for extracting features from Shipwrecks game data.
 class ShipwrecksLoader(GeneratorLoader):
     ## Constructor for the ShipwrecksLoader class.
     #  Initializes some custom private data (not present in base class) for use
```

### Comparing `opengamedata_core-0.0.5/src/ogd/games/SHIPWRECKS/features/ActiveJobs.py` & `opengamedata_core-0.0.6/src/ogd/games/SHIPWRECKS/features/ActiveJobs.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # import libraries
 import json
 from collections import defaultdict
 from typing import Any, List, Optional
 # import locals
 from ogd.core.generators.extractors.Feature import Feature
 from ogd.core.generators.Generator import GeneratorParameters
-from ogd.core.schemas.Event import Event
-from ogd.core.schemas.ExtractionMode import ExtractionMode
-from ogd.core.schemas.FeatureData import FeatureData
+from ogd.core.models.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
+from ogd.core.models.FeatureData import FeatureData
 
 
 class ActiveJobs(Feature):
 
     def __init__(self, params:GeneratorParameters):
         super().__init__(params=params)
         self._current_session_id = None
```

### Comparing `opengamedata_core-0.0.5/src/ogd/games/SHIPWRECKS/features/EventList.py` & `opengamedata_core-0.0.6/src/ogd/games/SHIPWRECKS/features/EventList.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # import libraries
 import json
 from typing import Any, List
 # import locals
 from ogd.core.generators.extractors.Feature import Feature
 from ogd.core.generators.Generator import GeneratorParameters
-from ogd.core.schemas.Event import Event
-from ogd.core.schemas.ExtractionMode import ExtractionMode
-from ogd.core.schemas.FeatureData import FeatureData
+from ogd.core.models.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
+from ogd.core.models.FeatureData import FeatureData
 
 
 class EventList(Feature):
 
     def __init__(self, params:GeneratorParameters):
         super().__init__(params=params)
         self._event_list = []
```

### Comparing `opengamedata_core-0.0.5/src/ogd/games/SHIPWRECKS/features/EvidenceBoardCompleteCount.py` & `opengamedata_core-0.0.6/src/ogd/games/PENGUINS/features/WaddleCount.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,34 +1,37 @@
 # import libraries
-from typing import Any, List, Optional
+import logging
+from typing import Any, Dict, List, Optional
 # import locals
-from ogd.core.generators.extractors.Feature import Feature
+from ogd.core.utils.Logger import Logger
 from ogd.core.generators.Generator import GeneratorParameters
-from ogd.core.schemas.Event import Event
-from ogd.core.schemas.ExtractionMode import ExtractionMode
-from ogd.core.schemas.FeatureData import FeatureData
+from ogd.core.models.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
+from ogd.core.models.FeatureData import FeatureData
+from ogd.core.generators.extractors.SessionFeature import SessionFeature
 
-class EvidenceBoardCompleteCount(Feature):
+
+class WaddleCount(SessionFeature):
 
     def __init__(self, params:GeneratorParameters):
         super().__init__(params=params)
-        self._count = 0
+        self._current_count : int = 0
 
     # *** IMPLEMENT ABSTRACT FUNCTIONS ***
     @classmethod
     def _eventFilter(cls, mode:ExtractionMode) -> List[str]:
-        return ["evidence_board_complete"]
+        return ["player_waddle"]
 
     @classmethod
     def _featureFilter(cls, mode:ExtractionMode) -> List[str]:
         return []
 
     def _updateFromEvent(self, event:Event) -> None:
-        self._count += 1
+        self._current_count += 1
 
     def _updateFromFeatureData(self, feature:FeatureData):
         return
 
     def _getFeatureValues(self) -> List[Any]:
-        return [self._count]
+        return [self._current_count]
 
-    # *** Optionally override public functions. ***
+
```

### Comparing `opengamedata_core-0.0.5/src/ogd/games/SHIPWRECKS/features/JobsAttempted.py` & `opengamedata_core-0.0.6/src/ogd/games/SHIPWRECKS/features/JobsAttempted.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # import libraries
 from collections import defaultdict
 from statistics import stdev
 from typing import Any, List
 # import locals
 from ogd.core.generators.extractors.Feature import Feature
 from ogd.core.generators.Generator import GeneratorParameters
-from ogd.core.schemas.Event import Event
-from ogd.core.schemas.ExtractionMode import ExtractionMode
-from ogd.core.schemas.FeatureData import FeatureData
+from ogd.core.models.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
+from ogd.core.models.FeatureData import FeatureData
 
 
 class JobsAttempted(Feature):
 
     def __init__(self, params:GeneratorParameters, mission_map:dict):
         self._mission_map = mission_map
         super().__init__(params=params)
```

### Comparing `opengamedata_core-0.0.5/src/ogd/games/SHIPWRECKS/features/JobsCompleted.py` & `opengamedata_core-0.0.6/src/ogd/games/SHIPWRECKS/features/JobsCompleted.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Any, List
 
 from ogd.core.generators.extractors.SessionFeature import SessionFeature
 from ogd.core.generators.Generator import GeneratorParameters
-from ogd.core.schemas.Event import Event
-from ogd.core.schemas.ExtractionMode import ExtractionMode
-from ogd.core.schemas.FeatureData import FeatureData
+from ogd.core.models.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
+from ogd.core.models.FeatureData import FeatureData
 
 class JobsCompleted(SessionFeature):
 
     def __init__(self, params:GeneratorParameters, session_id:str):
         self._session_id = session_id
         super().__init__(params=params)
         self._jobs_completed = []
```

### Comparing `opengamedata_core-0.0.5/src/ogd/games/SHIPWRECKS/features/MissionDiveTime.py` & `opengamedata_core-0.0.6/src/ogd/games/SHIPWRECKS/features/MissionDiveTime.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # import libraries
 from datetime import timedelta
 from typing import Any, List, Optional
 # import locals
 from ogd.core.generators.extractors.Feature import Feature
 from ogd.core.generators.Generator import GeneratorParameters
-from ogd.core.schemas.Event import Event
-from ogd.core.schemas.ExtractionMode import ExtractionMode
-from ogd.core.schemas.FeatureData import FeatureData
+from ogd.core.models.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
+from ogd.core.models.FeatureData import FeatureData
 
 
 class MissionDiveTime(Feature):
     
     def __init__(self, params:GeneratorParameters):
         super().__init__(params=params)
         self._dive_start_time = None
```

### Comparing `opengamedata_core-0.0.5/src/ogd/games/SHIPWRECKS/features/MissionSonarTimeToComplete.py` & `opengamedata_core-0.0.6/src/ogd/games/PENGUINS/features/RegionEnterCount.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,42 +1,50 @@
 # import libraries
-from datetime import timedelta
-from typing import Any, List, Optional
+import logging
+from typing import Any, Dict, List, Optional
 # import locals
-from ogd.core.generators.extractors.Feature import Feature
+from ogd.core.utils.Logger import Logger
 from ogd.core.generators.Generator import GeneratorParameters
-from ogd.core.schemas.Event import Event
-from ogd.core.schemas.ExtractionMode import ExtractionMode
-from ogd.core.schemas.FeatureData import FeatureData
+from ogd.core.generators.extractors.Feature import Feature
+from ogd.games.PENGUINS.features.bases.PerRegionFeature import PerRegionFeature
+from ogd.core.models.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
+from ogd.core.models.FeatureData import FeatureData
+from ogd.core.generators.extractors.PerCountFeature import PerCountFeature
 
 
-class MissionSonarTimeToComplete(Feature):
-    
-    # *** IMPLEMENT ABSTRACT FUNCTIONS ***
-    def __init__(self, params:GeneratorParameters):
+class RegionEnterCount(PerCountFeature):
+
+    def __init__(self, params:GeneratorParameters, region_map:List[Dict[str, Any]]):
         super().__init__(params=params)
-        self._sonar_start_time = None
-        self._time = timedelta(0)
+        self._region_map = region_map
+        self._current_count : int = 0
 
+    # *** IMPLEMENT ABSTRACT FUNCTIONS ***
     @classmethod
     def _eventFilter(cls, mode:ExtractionMode) -> List[str]:
-        return ["sonar_start", "sonar_exit"]
+        return ["enter_region"]
 
     @classmethod
     def _featureFilter(cls, mode:ExtractionMode) -> List[str]:
         return []
 
     def _updateFromEvent(self, event:Event) -> None:
-        if event.EventName == "sonar_start":
-            self._sonar_start_time = event.Timestamp
-        elif event.EventName == "sonar_complete":
-            if self._sonar_start_time is not None:
-                self._time += (event.Timestamp - self._sonar_start_time).total_seconds() # TODO : maybe see if we should add timedeltas and convert to float at end?
-                self._sonar_start_time = None
+        self._current_count += 1
 
     def _updateFromFeatureData(self, feature:FeatureData):
         return
 
     def _getFeatureValues(self) -> List[Any]:
-        return [self._time]
+        return [self._current_count]
+
+    # *** Optionally override public functions. ***
+    def _validateEventCountIndex(self, event: Event):
+        ret_val : bool = False
+        region_name = event.EventData.get("region_name")
+        if region_name is not None:
+            if region_name in self._region_map and self._region_map[region_name] == self.CountIndex:
+                ret_val = True
+        else:
+            self.WarningMessage(f"Got invalid region data in {type(self).__name__}")
 
-    # *** Optionally override public functions. ***
+        return ret_val
```

### Comparing `opengamedata_core-0.0.5/src/ogd/games/SHIPWRECKS/features/PlayerSummary.py` & `opengamedata_core-0.0.6/src/ogd/games/SHIPWRECKS/features/PlayerSummary.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Any, List
 
 from ogd.core.generators.extractors.SessionFeature import SessionFeature
 from ogd.core.generators.Generator import GeneratorParameters
-from ogd.core.schemas.Event import Event
-from ogd.core.schemas.ExtractionMode import ExtractionMode
-from ogd.core.schemas.FeatureData import FeatureData
+from ogd.core.models.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
+from ogd.core.models.FeatureData import FeatureData
 
 class PlayerSummary(SessionFeature):
 
     def __init__(self, params:GeneratorParameters):
         super().__init__(params=params)
         self._summary = {}
```

### Comparing `opengamedata_core-0.0.5/src/ogd/games/SHIPWRECKS/features/PopulationSummary.py` & `opengamedata_core-0.0.6/src/ogd/games/SHIPWRECKS/features/PopulationSummary.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from collections import defaultdict
 from typing import Any, Dict, List, Union
 from unicodedata import numeric
 
 from ogd.core.generators.extractors.SessionFeature import SessionFeature
 from ogd.core.generators.Generator import GeneratorParameters
-from ogd.core.schemas.Event import Event
-from ogd.core.schemas.ExtractionMode import ExtractionMode
-from ogd.core.schemas.FeatureData import FeatureData
+from ogd.core.models.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
+from ogd.core.models.FeatureData import FeatureData
 
 class PopulationSummary(SessionFeature):
 
     def __init__(self, params:GeneratorParameters):
         super().__init__(params=params)
         self._session_completions = defaultdict(list)
         self._session_times = []
```

### Comparing `opengamedata_core-0.0.5/src/ogd/games/SHIPWRECKS/features/SessionDuration.py` & `opengamedata_core-0.0.6/src/ogd/games/SHIPWRECKS/features/SessionDuration.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # import libraries
 from typing import Any, List
 # import locals
 from ogd.core.generators.extractors.SessionFeature import SessionFeature
 from ogd.core.generators.Generator import GeneratorParameters
-from ogd.core.schemas.Event import Event
-from ogd.core.schemas.ExtractionMode import ExtractionMode
-from ogd.core.schemas.FeatureData import FeatureData
+from ogd.core.models.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
+from ogd.core.models.FeatureData import FeatureData
 
 
 class SessionDuration(SessionFeature):
 
     def __init__(self, params:GeneratorParameters, session_id:str):
         self._session_id = session_id
         super().__init__(params=params)
```

### Comparing `opengamedata_core-0.0.5/src/ogd/games/SHIPWRECKS/features/SessionID.py` & `opengamedata_core-0.0.6/src/ogd/games/PENGUINS/features/PenguinInteractCount.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,34 +1,35 @@
 # import libraries
-from typing import Any, List, Optional
+import logging
+from typing import Any, Dict, List, Optional
 # import locals
-from ogd.core.generators.extractors.SessionFeature import SessionFeature
+from ogd.core.utils.Logger import Logger
 from ogd.core.generators.Generator import GeneratorParameters
-from ogd.core.schemas.Event import Event
-from ogd.core.schemas.ExtractionMode import ExtractionMode
-from ogd.core.schemas.FeatureData import FeatureData
+from ogd.core.models.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
+from ogd.core.models.FeatureData import FeatureData
+from ogd.core.generators.extractors.SessionFeature import SessionFeature
+
 
-class SessionID(SessionFeature):
+class PenguinInteractCount(SessionFeature):
 
-    def __init__(self, params:GeneratorParameters, session_id:str):
-        self._session_id = session_id
+    def __init__(self, params:GeneratorParameters):
         super().__init__(params=params)
+        self._current_count : int = 0
 
     # *** IMPLEMENT ABSTRACT FUNCTIONS ***
     @classmethod
     def _eventFilter(cls, mode:ExtractionMode) -> List[str]:
-        return []
+        return ["peck_penguin", "flipper_bash_penguin"]
 
     @classmethod
     def _featureFilter(cls, mode:ExtractionMode) -> List[str]:
         return []
 
     def _updateFromEvent(self, event:Event) -> None:
-        return
+        self._current_count += 1
 
     def _updateFromFeatureData(self, feature:FeatureData):
         return
 
     def _getFeatureValues(self) -> List[Any]:
-        return [self._session_id]
-
-    # *** Optionally override public functions. ***
+        return [self._current_count]
```

### Comparing `opengamedata_core-0.0.5/src/ogd/games/SHIPWRECKS/features/TopJobCompletionDestinations.py` & `opengamedata_core-0.0.6/src/ogd/games/SHIPWRECKS/features/TopJobCompletionDestinations.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 import json
 from collections import defaultdict
 from typing import Any, List
 # import locals
 from ogd.core.utils.Logger import Logger
 from ogd.core.generators.extractors.Feature import Feature
 from ogd.core.generators.Generator import GeneratorParameters
-from ogd.core.schemas.Event import Event
-from ogd.core.schemas.ExtractionMode import ExtractionMode
-from ogd.core.schemas.FeatureData import FeatureData
+from ogd.core.models.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
+from ogd.core.models.FeatureData import FeatureData
 
 
 class TopJobCompletionDestinations(Feature):
 
     def __init__(self, params:GeneratorParameters):
         super().__init__(params=params)
         self._current_session_id = None
```

### Comparing `opengamedata_core-0.0.5/src/ogd/games/SHIPWRECKS/features/TopJobSwitchDestinations.py` & `opengamedata_core-0.0.6/src/ogd/games/SHIPWRECKS/features/TopJobSwitchDestinations.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 import json
 from collections import defaultdict
 from typing import Any, List
 # import locals
 from ogd.core.utils.Logger import Logger
 from ogd.core.generators.extractors.Feature import Feature
 from ogd.core.generators.Generator import GeneratorParameters
-from ogd.core.schemas.Event import Event
-from ogd.core.schemas.ExtractionMode import ExtractionMode
-from ogd.core.schemas.FeatureData import FeatureData
+from ogd.core.models.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
+from ogd.core.models.FeatureData import FeatureData
 
 
 class TopJobSwitchDestinations(Feature):
 
     def __init__(self, params:GeneratorParameters):
         super().__init__(params=params)
         self._current_session_id = None
```

### Comparing `opengamedata_core-0.0.5/src/ogd/games/SHIPWRECKS/features/TotalDiveTime.py` & `opengamedata_core-0.0.6/src/ogd/games/SHIPWRECKS/features/TotalDiveTime.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # import libraries
 from typing import Any, List, Optional
 from datetime import timedelta
 # import locals
 from ogd.core.generators.extractors.SessionFeature import SessionFeature
 from ogd.core.generators.Generator import GeneratorParameters
-from ogd.core.schemas.Event import Event
-from ogd.core.schemas.ExtractionMode import ExtractionMode
-from ogd.core.schemas.FeatureData import FeatureData
+from ogd.core.models.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
+from ogd.core.models.FeatureData import FeatureData
 
 class TotalDiveTime(SessionFeature):
 
     def __init__(self, params:GeneratorParameters):
         super().__init__(params=params)
         self._time = 0
```

### Comparing `opengamedata_core-0.0.5/src/ogd/games/SHIPWRECKS/features/__init__.py` & `opengamedata_core-0.0.6/src/ogd/games/SHIPWRECKS/features/__init__.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.5/src/ogd/games/SHIPWRECKS/schemas/SHIPWRECKS.json.template` & `opengamedata_core-0.0.6/src/ogd/games/SHIPWRECKS/schemas/SHIPWRECKS.json.template`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.5/src/ogd/games/THERMOVR/ThermoVRLoader.py` & `opengamedata_core-0.0.6/src/ogd/games/THERMOVR/ThermoVRLoader.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,16 +8,16 @@
 from ogd.games import THERMOVR
 from ogd.core.generators.detectors.Detector import Detector
 from ogd.core.generators.Generator import GeneratorParameters
 from ogd.core.generators.GeneratorLoader import GeneratorLoader
 from ogd.core.generators.extractors.Feature import Feature
 from ogd.games.THERMOVR.detectors import *
 from ogd.games.THERMOVR.features import *
-from ogd.core.schemas.Event import Event
-from ogd.core.schemas.ExtractionMode import ExtractionMode
+from ogd.core.models.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
 from ogd.core.schemas.games.GameSchema import GameSchema
 from ogd.core.utils.utils import loadJSONFile
 
 EXPORT_PATH = "games/THERMOVR/DBExport.json"
 
 ## @class ThermoVRLoader
 #  Extractor subclass for extracting features from ThermoVR game data.
```

### Comparing `opengamedata_core-0.0.5/src/ogd/games/THERMOVR/features/LeftHandMoves.py` & `opengamedata_core-0.0.6/src/ogd/games/THERMOVR/features/LeftHandMoves.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Any, Dict, List
 
 from ogd.core.generators.Generator import GeneratorParameters
 from ogd.core.generators.extractors.SessionFeature import SessionFeature
-from ogd.core.schemas.Event import Event
-from ogd.core.schemas.ExtractionMode import ExtractionMode
-from ogd.core.schemas.FeatureData import FeatureData
+from ogd.core.models.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
+from ogd.core.models.FeatureData import FeatureData
 
 class LeftHandMovesCount(SessionFeature):
 
     def __init__(self, params: GeneratorParameters):
         self._left_hand_move_count = 0
         self._last_hand_action = None
         super().__init__(params=params)
```

### Comparing `opengamedata_core-0.0.5/src/ogd/games/THERMOVR/features/PhasesReached.py` & `opengamedata_core-0.0.6/src/ogd/games/WAVES/features/PercentOffsetMoves.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,31 +1,39 @@
-from typing import Any, List
+# import libraries
+from ogd.core.models import Event
+from typing import Any, List, Optional
+# import locals
+from ogd.core.generators.extractors.Feature import Feature
 from ogd.core.generators.Generator import GeneratorParameters
-from ogd.core.generators.extractors.SessionFeature import SessionFeature
-from ogd.core.schemas.Event import Event
-from ogd.core.schemas.ExtractionMode import ExtractionMode
-from ogd.core.schemas.FeatureData import FeatureData
-
-class PhasesReached(SessionFeature):
-
-    def __init__(self, params: GeneratorParameters):
-        self.phases_reached = set()
-        super().__init__(params=params)
+from ogd.core.models.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
+from ogd.core.models.FeatureData import FeatureData
 
+
+class PercentOffsetMoves(Feature):
+    def __init__(self, params:GeneratorParameters):
+        Feature.__init__(self, params=params)
+        self._offset_count = 0
+        self._count = 0
+
+    # *** IMPLEMENT ABSTRACT FUNCTIONS ***
     @classmethod
-    def _getEventDependencies(cls, mode: ExtractionMode) -> List[str]:
-        return ["all_events"]
+    def _eventFilter(cls, mode:ExtractionMode) -> List[str]:
+        return ["CUSTOM.1", "CUSTOM.2"]
+        # return ["SLIDER_MOVE_RELEASE", "ARROW_MOVE_RELEASE"]
 
     @classmethod
-    def _getFeatureDependencies(cls, mode: ExtractionMode) -> List[str]:
+    def _featureFilter(cls, mode:ExtractionMode) -> List[str]:
         return []
 
-    def _extractFromEvent(self, event: Event) -> None:
-        region = event.GameState.get("region")
-        if region:
-            self.phases_reached.add(region)
+    def _updateFromEvent(self, event:Event) -> None:
+        self._count += 1
+        if event.EventData['slider'].upper() == 'OFFSET':
+            self._offset_count += 1
 
-    def _extractFromFeatureData(self, feature: FeatureData):
+    def _updateFromFeatureData(self, feature:FeatureData):
         return
 
     def _getFeatureValues(self) -> List[Any]:
-        return [list(self.phases_reached)]
+        return [self._offset_count / self._count if self._count != 0 else None]
+
+    # *** Optionally override public functions. ***
```

### Comparing `opengamedata_core-0.0.5/src/ogd/games/THERMOVR/features/PlayMode.py` & `opengamedata_core-0.0.6/src/ogd/games/WAVES/features/RangeR2.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,32 +1,33 @@
-from typing import Any, List
+# import libraries
+from ogd.core.models import Event
+from typing import Any, List, Optional
+# import locals
+from ogd.core.generators.extractors.Feature import Feature
 from ogd.core.generators.Generator import GeneratorParameters
-from ogd.core.generators.extractors.SessionFeature import SessionFeature
-from ogd.core.schemas.Event import Event
-from ogd.core.schemas.ExtractionMode import ExtractionMode
-from ogd.core.schemas.FeatureData import FeatureData
-
-class PlayMode(SessionFeature):
-
-    def __init__(self, params: GeneratorParameters):
-        self.play_mode = None
-        super().__init__(params=params)
+from ogd.core.models.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
+from ogd.core.models.FeatureData import FeatureData
+
+class RangeR2(Feature):
+    def __init__(self, params:GeneratorParameters):
+        Feature.__init__(self, params=params)
 
+    # *** IMPLEMENT ABSTRACT FUNCTIONS ***
     @classmethod
-    def _getEventDependencies(cls, mode: ExtractionMode) -> List[str]:
-        return ["game_start"]
+    def _eventFilter(cls, mode:ExtractionMode) -> List[str]:
+        return []
 
     @classmethod
-    def _getFeatureDependencies(cls, mode: ExtractionMode) -> List[str]:
+    def _featureFilter(cls, mode:ExtractionMode) -> List[str]:
         return []
 
-    def _extractFromEvent(self, event: Event) -> None:
-        if event.EventName == "game_start":
-            mode = event.EventData.get("mode")
-            if mode:
-                self.play_mode = mode
+    def _updateFromEvent(self, event:Event) -> None:
+        return
 
-    def _extractFromFeatureData(self, feature: FeatureData):
+    def _updateFromFeatureData(self, feature:FeatureData):
         return
 
     def _getFeatureValues(self) -> List[Any]:
-        return [self.play_mode]
+        return ["Not Implemented"]
+
+    # *** Optionally override public functions. ***
```

### Comparing `opengamedata_core-0.0.5/src/ogd/games/THERMOVR/features/RightHandMoves.py` & `opengamedata_core-0.0.6/src/ogd/games/THERMOVR/features/RightHandMoves.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Any, Dict, List
 
 from ogd.core.generators.Generator import GeneratorParameters
 from ogd.core.generators.extractors.SessionFeature import SessionFeature
-from ogd.core.schemas.Event import Event
-from ogd.core.schemas.ExtractionMode import ExtractionMode
-from ogd.core.schemas.FeatureData import FeatureData
+from ogd.core.models.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
+from ogd.core.models.FeatureData import FeatureData
 
 class RightHandMovesCount(SessionFeature):
 
     def __init__(self, params: GeneratorParameters):
         self._right_hand_move_count = 0
         self._last_hand_action = None
         super().__init__(params=params)
```

### Comparing `opengamedata_core-0.0.5/src/ogd/games/THERMOVR/features/TaskCompleteCount.py` & `opengamedata_core-0.0.6/src/ogd/games/THERMOVR/features/TaskCompleteCount.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import Any, List, Set
 from ogd.core.generators.Generator import GeneratorParameters
 from ogd.core.generators.extractors.SessionFeature import SessionFeature
-from ogd.core.schemas.Event import Event
-from ogd.core.schemas.ExtractionMode import ExtractionMode
-from ogd.core.schemas.FeatureData import FeatureData
+from ogd.core.models.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
+from ogd.core.models.FeatureData import FeatureData
 import json
 
 class TaskCompleteCount(SessionFeature):
 
     def __init__(self, params: GeneratorParameters):
         self.completed_tasks: Set[str] = set()
         super().__init__(params=params)
```

### Comparing `opengamedata_core-0.0.5/src/ogd/games/THERMOVR/features/ToolNudgeCount.py` & `opengamedata_core-0.0.6/src/ogd/games/THERMOVR/features/ToolNudgeCount.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Any, Final, List
 from enum import Enum
 from ogd.core.generators.Generator import GeneratorParameters
 from ogd.core.generators.extractors.SessionFeature import SessionFeature
-from ogd.core.schemas.Event import Event
-from ogd.core.schemas.ExtractionMode import ExtractionMode
-from ogd.core.schemas.FeatureData import FeatureData
+from ogd.core.models.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
+from ogd.core.models.FeatureData import FeatureData
 
 class Thermotool(Enum):
     INSULATION          = "insulation"
     LOWER_STOP          = "lower_stop"
     UPPER_STOP          = "upper_stop"
     INCREASE_WEIGHT     = "increase_weight"
     DECREASE_WEIGHT     = "decrease_weight"
```

### Comparing `opengamedata_core-0.0.5/src/ogd/games/THERMOVR/features/ToolSliderTime.py` & `opengamedata_core-0.0.6/src/ogd/games/THERMOVR/features/ToolSliderTime.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Any, Dict, List
 
 from ogd.core.generators.Generator import GeneratorParameters
 from ogd.core.generators.extractors.SessionFeature import SessionFeature
-from ogd.core.schemas.Event import Event
-from ogd.core.schemas.ExtractionMode import ExtractionMode
-from ogd.core.schemas.FeatureData import FeatureData
+from ogd.core.models.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
+from ogd.core.models.FeatureData import FeatureData
 
 class ToolSliderTime(SessionFeature):
 
     def __init__(self, params: GeneratorParameters):
         self._slider_start_time = {}
         self._slider_times = {}
         super().__init__(params=params)
```

### Comparing `opengamedata_core-0.0.5/src/ogd/games/THERMOVR/schemas/THERMOVR.json.template` & `opengamedata_core-0.0.6/src/ogd/games/THERMOVR/schemas/THERMOVR.json.template`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.5/src/ogd/games/TRANSFORMATION_QUEST/DBExport.json` & `opengamedata_core-0.0.6/src/ogd/games/TRANSFORMATION_QUEST/DBExport.json`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.5/src/ogd/games/TRANSFORMATION_QUEST/schemas/TRANSFORMATION_QUEST.json.template` & `opengamedata_core-0.0.6/src/ogd/games/TRANSFORMATION_QUEST/schemas/TRANSFORMATION_QUEST.json.template`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.5/src/ogd/games/WAVES/WaveLoader.py` & `opengamedata_core-0.0.6/src/ogd/games/WAVES/WaveLoader.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 from . import features
 from ogd.core.generators.detectors.Detector import Detector
 from ogd.core.generators.Generator import GeneratorParameters
 from ogd.core.generators.GeneratorLoader import GeneratorLoader
 from ogd.core.generators.extractors.Feature import Feature
 from ogd.games.WAVES.features import *
 from ogd.core.generators.Generator import GeneratorParameters
-from ogd.core.schemas.Event import Event
-from ogd.core.schemas.ExtractionMode import ExtractionMode
+from ogd.core.models.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
 from ogd.core.schemas.games.GameSchema import GameSchema
 
 ## @class WaveExtractor
 #  Extractor subclass for extracting features from Waves game data.
 class WaveLoader(GeneratorLoader):
 
     # *** IMPLEMENT ABSTRACT FUNCTIONS ***
```

### Comparing `opengamedata_core-0.0.5/src/ogd/games/WAVES/features/AmplitudeGoodMoveCount.py` & `opengamedata_core-0.0.6/src/ogd/games/WAVES/features/OffsetGoodMoveCount.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 # import libraries
-from ogd.core.schemas import Event
+from ogd.core.models import Event
 from typing import Any, List, Optional
 # import locals
 from ogd.core.generators.extractors.PerLevelFeature import PerLevelFeature
 from ogd.core.generators.Generator import GeneratorParameters
-from ogd.core.schemas.Event import Event
-from ogd.core.schemas.ExtractionMode import ExtractionMode
-from ogd.core.schemas.FeatureData import FeatureData
+from ogd.core.models.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
+from ogd.core.models.FeatureData import FeatureData
 
-class AmplitudeGoodMoveCount(PerLevelFeature):
+class OffsetGoodMoveCount(PerLevelFeature):
     def __init__(self, params:GeneratorParameters):
         PerLevelFeature.__init__(self, params=params)
         self._count = 0
 
     # *** IMPLEMENT ABSTRACT FUNCTIONS ***
     @classmethod
     def _eventFilter(cls, mode:ExtractionMode) -> List[str]:
@@ -20,15 +20,15 @@
         # return ["SLIDER_MOVE_RELEASE", "ARROW_MOVE_RELEASE"]
 
     @classmethod
     def _featureFilter(cls, mode:ExtractionMode) -> List[str]:
         return []
 
     def _updateFromEvent(self, event:Event) -> None:
-        if event.EventData['slider'].upper() == 'AMPLITUDE':
+        if event.EventData['slider'].upper() == 'OFFSET':
             if event.EventName == "CUSTOM.1":
                 if event.EventData['end_closeness'] > event.EventData['begin_closeness']:
                     self._count += 1
             elif event.EventName == "CUSTOM.2":
                 start_dist = event.EventData['correct_val'] - event.EventData['begin_val']
                 end_dist = event.EventData['correct_val'] - event.EventData['end_val']
                 if abs(end_dist) < abs(start_dist):
```

### Comparing `opengamedata_core-0.0.5/src/ogd/games/WAVES/features/AverageFails.py` & `opengamedata_core-0.0.6/src/ogd/games/WAVES/features/AverageFails.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # import libraries
-from ogd.core.schemas import Event
+from ogd.core.models import Event
 from typing import Any, List, Optional
 # import locals
 from ogd.core.generators.extractors.SessionFeature import SessionFeature
 from ogd.core.generators.Generator import GeneratorParameters
-from ogd.core.schemas.Event import Event
-from ogd.core.schemas.ExtractionMode import ExtractionMode
-from ogd.core.schemas.FeatureData import FeatureData
+from ogd.core.models.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
+from ogd.core.models.FeatureData import FeatureData
 
 class AverageFails(SessionFeature):
     def __init__(self, params:GeneratorParameters):
         SessionFeature.__init__(self, params=params)
         self._levels_encountered : set = set()
         self._fail_count         : int = 0
```

### Comparing `opengamedata_core-0.0.5/src/ogd/games/WAVES/features/AverageLevelTime.py` & `opengamedata_core-0.0.6/src/ogd/games/WAVES/features/AverageLevelTime.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 # import libraries
 import logging
 from datetime import datetime
-from ogd.core.schemas import Event
+from ogd.core.models import Event
 from typing import Any, Dict, List, Optional
 # import locals
 from ogd.core.utils.Logger import Logger
 from ogd.core.generators.extractors.SessionFeature import SessionFeature
 from ogd.core.generators.Generator import GeneratorParameters
-from ogd.core.schemas.Event import Event
-from ogd.core.schemas.ExtractionMode import ExtractionMode
-from ogd.core.schemas.FeatureData import FeatureData
+from ogd.core.models.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
+from ogd.core.models.FeatureData import FeatureData
 
 class AverageLevelTime(SessionFeature):
     def __init__(self, params:GeneratorParameters):
         SessionFeature.__init__(self, params=params)
         self._levels_encountered : set                      = set()
         self._begin_times        : Dict[int,List[datetime]] = {}
         self._complete_times     : Dict[int,List[datetime]] = {}
```

### Comparing `opengamedata_core-0.0.5/src/ogd/games/WAVES/features/AverageMoveTypeChanges.py` & `opengamedata_core-0.0.6/src/ogd/games/WAVES/features/AverageMoveTypeChanges.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # import libraries
-from ogd.core.schemas import Event
+from ogd.core.models import Event
 from typing import Any, List, Optional
 # import locals
 from ogd.core.generators.extractors.SessionFeature import SessionFeature
 from ogd.core.generators.Generator import GeneratorParameters
-from ogd.core.schemas.Event import Event
-from ogd.core.schemas.ExtractionMode import ExtractionMode
-from ogd.core.schemas.FeatureData import FeatureData
+from ogd.core.models.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
+from ogd.core.models.FeatureData import FeatureData
 
 class AverageMoveTypeChanges(SessionFeature):
     def __init__(self, params:GeneratorParameters):
         SessionFeature.__init__(self, params=params)
         self._levels_encountered : set = set()
         self._last_move = {}
         self._change_count = {}
```

### Comparing `opengamedata_core-0.0.5/src/ogd/games/WAVES/features/AverageSliderMoves.py` & `opengamedata_core-0.0.6/src/ogd/games/WAVES/features/AverageSliderMoves.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # import libraries
-from ogd.core.schemas import Event
+from ogd.core.models import Event
 from typing import Any, List, Optional
 # import locals
 from ogd.core.generators.extractors.SessionFeature import SessionFeature
 from ogd.core.generators.Generator import GeneratorParameters
-from ogd.core.schemas.Event import Event
-from ogd.core.schemas.ExtractionMode import ExtractionMode
-from ogd.core.schemas.FeatureData import FeatureData
+from ogd.core.models.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
+from ogd.core.models.FeatureData import FeatureData
 
 class AverageSliderMoves(SessionFeature):
     def __init__(self, params:GeneratorParameters):
         SessionFeature.__init__(self, params=params)
         self._levels_encountered : set = set()
         self._slider_count       : int = 0
```

### Comparing `opengamedata_core-0.0.5/src/ogd/games/WAVES/features/BeginCount.py` & `opengamedata_core-0.0.6/src/ogd/games/WAVES/features/BeginCount.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # import libraries
-from ogd.core.schemas import Event
+from ogd.core.models import Event
 from typing import Any, List, Optional
 # import locals
 from ogd.core.generators.extractors.PerLevelFeature import PerLevelFeature
 from ogd.core.generators.Generator import GeneratorParameters
-from ogd.core.schemas.Event import Event
-from ogd.core.schemas.ExtractionMode import ExtractionMode
-from ogd.core.schemas.FeatureData import FeatureData
+from ogd.core.models.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
+from ogd.core.models.FeatureData import FeatureData
 
 class BeginCount(PerLevelFeature):
     def __init__(self, params:GeneratorParameters):
         PerLevelFeature.__init__(self, params=params)
         self._num_begins = 0
 
     # *** IMPLEMENT ABSTRACT FUNCTIONS ***
```

### Comparing `opengamedata_core-0.0.5/src/ogd/games/WAVES/features/ClosenessIntercept.py` & `opengamedata_core-0.0.6/src/ogd/games/WAVES/features/ClosenessIntercept.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # import libraries
-from ogd.core.schemas import Event
+from ogd.core.models import Event
 from typing import Any, List, Optional
 # import locals
 from ogd.core.generators.extractors.Feature import Feature
 from ogd.core.generators.Generator import GeneratorParameters
-from ogd.core.schemas.Event import Event
-from ogd.core.schemas.ExtractionMode import ExtractionMode
-from ogd.core.schemas.FeatureData import FeatureData
+from ogd.core.models.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
+from ogd.core.models.FeatureData import FeatureData
 
 
 class ClosenessIntercept(Feature):
     def __init__(self, params:GeneratorParameters):
         Feature.__init__(self, params=params)
 
     # *** IMPLEMENT ABSTRACT FUNCTIONS ***
```

### Comparing `opengamedata_core-0.0.5/src/ogd/games/WAVES/features/ClosenessR2.py` & `opengamedata_core-0.0.6/src/ogd/games/WAVES/features/SessionID.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 # import libraries
-from ogd.core.schemas import Event
+from ogd.core.models import Event
 from typing import Any, List, Optional
 # import locals
-from ogd.core.generators.extractors.Feature import Feature
+from ogd.core.generators.extractors.SessionFeature import SessionFeature
 from ogd.core.generators.Generator import GeneratorParameters
-from ogd.core.schemas.Event import Event
-from ogd.core.schemas.ExtractionMode import ExtractionMode
-from ogd.core.schemas.FeatureData import FeatureData
-
-class ClosenessR2(Feature):
-    def __init__(self, params:GeneratorParameters):
-        Feature.__init__(self, params=params)
+from ogd.core.models.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
+from ogd.core.models.FeatureData import FeatureData
+
+class SessionID(SessionFeature):
+    def __init__(self, params:GeneratorParameters, sessionID:str):
+        SessionFeature.__init__(self, params=params)
+        self._sessionID = sessionID
 
     # *** IMPLEMENT ABSTRACT FUNCTIONS ***
     @classmethod
     def _eventFilter(cls, mode:ExtractionMode) -> List[str]:
         return []
 
     @classmethod
@@ -24,10 +25,11 @@
     def _updateFromEvent(self, event:Event) -> None:
         return
 
     def _updateFromFeatureData(self, feature:FeatureData):
         return
 
     def _getFeatureValues(self) -> List[Any]:
-        return ["Not Implemented"]
+        return [self._sessionID]
 
     # *** Optionally override public functions. ***
+
```

### Comparing `opengamedata_core-0.0.5/src/ogd/games/WAVES/features/ClosenessSlope.py` & `opengamedata_core-0.0.6/src/ogd/games/WAVES/features/RangeIntercept.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 # import libraries
-from ogd.core.schemas import Event
+from ogd.core.models import Event
 from typing import Any, List, Optional
 # import locals
 from ogd.core.generators.extractors.Feature import Feature
 from ogd.core.generators.Generator import GeneratorParameters
-from ogd.core.schemas.Event import Event
-from ogd.core.schemas.ExtractionMode import ExtractionMode
-from ogd.core.schemas.FeatureData import FeatureData
+from ogd.core.models.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
+from ogd.core.models.FeatureData import FeatureData
 
-
-class ClosenessSlope(Feature):
+class RangeIntercept(Feature):
     def __init__(self, params:GeneratorParameters):
         Feature.__init__(self, params=params)
 
     # *** IMPLEMENT ABSTRACT FUNCTIONS ***
     @classmethod
     def _eventFilter(cls, mode:ExtractionMode) -> List[str]:
         return []
```

### Comparing `opengamedata_core-0.0.5/src/ogd/games/WAVES/features/Completed.py` & `opengamedata_core-0.0.6/src/ogd/games/WAVES/features/Completed.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # import libraries
 from os import truncate
-from ogd.core.schemas import Event
+from ogd.core.models import Event
 from typing import Any, List, Optional
 # import locals
 from ogd.core.generators.extractors.PerLevelFeature import PerLevelFeature
 from ogd.core.generators.Generator import GeneratorParameters
-from ogd.core.schemas.Event import Event
-from ogd.core.schemas.ExtractionMode import ExtractionMode
-from ogd.core.schemas.FeatureData import FeatureData
+from ogd.core.models.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
+from ogd.core.models.FeatureData import FeatureData
 
 class Completed(PerLevelFeature):
     def __init__(self, params:GeneratorParameters):
         PerLevelFeature.__init__(self, params=params)
         self._num_completes = 0
 
     # *** IMPLEMENT ABSTRACT FUNCTIONS ***
```

### Comparing `opengamedata_core-0.0.5/src/ogd/games/WAVES/features/FirstMoveType.py` & `opengamedata_core-0.0.6/src/ogd/games/WAVES/features/FirstMoveType.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # import libraries
-from ogd.core.schemas import Event
+from ogd.core.models import Event
 from typing import Any, List, Optional
 # import locals
 from ogd.core.generators.extractors.Feature import Feature
 from ogd.core.generators.Generator import GeneratorParameters
-from ogd.core.schemas.Event import Event
-from ogd.core.schemas.ExtractionMode import ExtractionMode
-from ogd.core.schemas.FeatureData import FeatureData
+from ogd.core.models.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
+from ogd.core.models.FeatureData import FeatureData
 
 
 class FirstMoveType(Feature):
     def __init__(self, params:GeneratorParameters):
         Feature.__init__(self, params=params)
         self._first_move = None
```

### Comparing `opengamedata_core-0.0.5/src/ogd/games/WAVES/features/MenuButtonCount.py` & `opengamedata_core-0.0.6/src/ogd/games/WAVES/features/TotalResets.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,35 +1,36 @@
 # import libraries
-from ogd.core.schemas import Event
+from ogd.core.models import Event
+import typing
 from typing import Any, List, Optional
 # import locals
 from ogd.core.generators.extractors.PerLevelFeature import PerLevelFeature
 from ogd.core.generators.Generator import GeneratorParameters
-from ogd.core.schemas.Event import Event
-from ogd.core.schemas.ExtractionMode import ExtractionMode
-from ogd.core.schemas.FeatureData import FeatureData
+from ogd.core.models.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
+from ogd.core.models.FeatureData import FeatureData
 
-class MenuButtonCount(PerLevelFeature):
+class TotalResets(PerLevelFeature):
     def __init__(self, params:GeneratorParameters):
         PerLevelFeature.__init__(self, params=params)
-        self._menu_btn_count = 0
+        self._reset_count = 0
 
     # *** IMPLEMENT ABSTRACT FUNCTIONS ***
     @classmethod
     def _eventFilter(cls, mode:ExtractionMode) -> List[str]:
-        return ["CUSTOM.5"]
-        # "events": ["MENU_BUTTON"],
+        return ["CUSTOM.4"]
+        # "events": ["RESET_BTN_PRESS"],
 
     @classmethod
     def _featureFilter(cls, mode:ExtractionMode) -> List[str]:
         return []
 
     def _updateFromEvent(self, event:Event) -> None:
-        self._menu_btn_count += 1
+        self._reset_count += 1
 
     def _updateFromFeatureData(self, feature:FeatureData):
         return
 
     def _getFeatureValues(self) -> List[Any]:
-        return [self._menu_btn_count]
+        return [self._reset_count]
 
     # *** Optionally override public functions. ***
```

### Comparing `opengamedata_core-0.0.5/src/ogd/games/WAVES/features/OffsetGoodMoveCount.py` & `opengamedata_core-0.0.6/src/ogd/games/WAVES/features/WavelengthGoodMoveCount.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 # import libraries
-from ogd.core.schemas import Event
+from ogd.core.models import Event
+import typing
 from typing import Any, List, Optional
 # import locals
 from ogd.core.generators.extractors.PerLevelFeature import PerLevelFeature
 from ogd.core.generators.Generator import GeneratorParameters
-from ogd.core.schemas.Event import Event
-from ogd.core.schemas.ExtractionMode import ExtractionMode
-from ogd.core.schemas.FeatureData import FeatureData
+from ogd.core.models.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
+from ogd.core.models.FeatureData import FeatureData
 
-class OffsetGoodMoveCount(PerLevelFeature):
+class WavelengthGoodMoveCount(PerLevelFeature):
     def __init__(self, params:GeneratorParameters):
         PerLevelFeature.__init__(self, params=params)
         self._count = 0
 
     # *** IMPLEMENT ABSTRACT FUNCTIONS ***
     @classmethod
     def _eventFilter(cls, mode:ExtractionMode) -> List[str]:
@@ -20,15 +21,15 @@
         # return ["SLIDER_MOVE_RELEASE", "ARROW_MOVE_RELEASE"]
 
     @classmethod
     def _featureFilter(cls, mode:ExtractionMode) -> List[str]:
         return []
 
     def _updateFromEvent(self, event:Event) -> None:
-        if event.EventData['slider'].upper() == 'OFFSET':
+        if event.EventData['slider'].upper() == 'WAVELENGTH':
             if event.EventName == "CUSTOM.1":
                 if event.EventData['end_closeness'] > event.EventData['begin_closeness']:
                     self._count += 1
             elif event.EventName == "CUSTOM.2":
                 start_dist = event.EventData['correct_val'] - event.EventData['begin_val']
                 end_dist = event.EventData['correct_val'] - event.EventData['end_val']
                 if abs(end_dist) < abs(start_dist):
```

### Comparing `opengamedata_core-0.0.5/src/ogd/games/WAVES/features/OverallPercentAmplitudeMoves.py` & `opengamedata_core-0.0.6/src/ogd/games/WAVES/features/OverallPercentAmplitudeMoves.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # import libraries
-from ogd.core.schemas import Event
+from ogd.core.models import Event
 from typing import Any, List, Optional
 # import locals
 from ogd.core.generators.extractors.SessionFeature import SessionFeature
 from ogd.core.generators.Generator import GeneratorParameters
-from ogd.core.schemas.Event import Event
-from ogd.core.schemas.ExtractionMode import ExtractionMode
-from ogd.core.schemas.FeatureData import FeatureData
+from ogd.core.models.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
+from ogd.core.models.FeatureData import FeatureData
 
 class OverallPercentAmplitudeMoves(SessionFeature):
     def __init__(self, params:GeneratorParameters):
         SessionFeature.__init__(self, params=params)
         self._amplitude_count = 0
         self._move_count = 0
```

### Comparing `opengamedata_core-0.0.5/src/ogd/games/WAVES/features/OverallPercentOffsetMoves.py` & `opengamedata_core-0.0.6/src/ogd/games/WAVES/features/OverallPercentOffsetMoves.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # import libraries
-from ogd.core.schemas import Event
+from ogd.core.models import Event
 from typing import Any, List, Optional
 # import locals
 from ogd.core.generators.extractors.SessionFeature import SessionFeature
 from ogd.core.generators.Generator import GeneratorParameters
-from ogd.core.schemas.Event import Event
-from ogd.core.schemas.ExtractionMode import ExtractionMode
-from ogd.core.schemas.FeatureData import FeatureData
+from ogd.core.models.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
+from ogd.core.models.FeatureData import FeatureData
 
 class OverallPercentOffsetMoves(SessionFeature):
     def __init__(self, params:GeneratorParameters):
         SessionFeature.__init__(self, params=params)
         self._offset_count = 0
         self._move_count = 0
```

### Comparing `opengamedata_core-0.0.5/src/ogd/games/WAVES/features/OverallPercentWavelengthMoves.py` & `opengamedata_core-0.0.6/src/ogd/games/WAVES/features/TotalMoveTypeChanges.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,43 +1,39 @@
 # import libraries
-from ogd.core.schemas import Event
+from ogd.core.models import Event
+import typing
 from typing import Any, List, Optional
 # import locals
-from ogd.core.generators.extractors.SessionFeature import SessionFeature
+from ogd.core.generators.extractors.PerLevelFeature import PerLevelFeature
 from ogd.core.generators.Generator import GeneratorParameters
-from ogd.core.schemas.Event import Event
-from ogd.core.schemas.ExtractionMode import ExtractionMode
-from ogd.core.schemas.FeatureData import FeatureData
+from ogd.core.models.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
+from ogd.core.models.FeatureData import FeatureData
 
-class OverallPercentWavelengthMoves(SessionFeature):
+class TotalMoveTypeChanges(PerLevelFeature):
     def __init__(self, params:GeneratorParameters):
-        SessionFeature.__init__(self, params=params)
-        self._wavelength_count = 0
-        self._move_count = 0
+        PerLevelFeature.__init__(self, params=params)
+        self._last_move = None
+        self._change_count = 0
 
     # *** IMPLEMENT ABSTRACT FUNCTIONS ***
     @classmethod
     def _eventFilter(cls, mode:ExtractionMode) -> List[str]:
         return ["CUSTOM.1", "CUSTOM.2"]
         # return ["SLIDER_MOVE_RELEASE", "ARROW_MOVE_RELEASE"]
 
     @classmethod
     def _featureFilter(cls, mode:ExtractionMode) -> List[str]:
         return []
 
     def _updateFromEvent(self, event:Event) -> None:
-        self._move_count += 1
-        if event.EventData["slider"].upper() == "WAVELENGTH":
-            self._wavelength_count += 1
+        if self._last_move != event.EventName:
+            self._change_count += 1
+        self._last_move = event.EventName
 
     def _updateFromFeatureData(self, feature:FeatureData):
         return
 
     def _getFeatureValues(self) -> List[Any]:
-        if self._move_count > 0:
-            return [self._wavelength_count / self._move_count * 100]
-        else:
-            return [None]
+        return [self._change_count]
 
     # *** Optionally override public functions. ***
-
-
```

### Comparing `opengamedata_core-0.0.5/src/ogd/games/WAVES/features/OverallSliderAverageRange.py` & `opengamedata_core-0.0.6/src/ogd/games/WAVES/features/OverallSliderAverageStandardDeviations.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 # import libraries
-from ogd.core.schemas import Event
+from ogd.core.models import Event
 from typing import Any, List, Optional
 # import locals
 from ogd.core.generators.extractors.SessionFeature import SessionFeature
 from ogd.core.generators.Generator import GeneratorParameters
-from ogd.core.schemas.Event import Event
-from ogd.core.schemas.ExtractionMode import ExtractionMode
-from ogd.core.schemas.FeatureData import FeatureData
+from ogd.core.models.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
+from ogd.core.models.FeatureData import FeatureData
 
-class OverallSliderAverageRange(SessionFeature):
+class OverallSliderAverageStandardDeviations(SessionFeature):
     def __init__(self, params:GeneratorParameters):
         SessionFeature.__init__(self, params=params)
-        self._ranges = []
+        self._std_devs = []
 
     # *** IMPLEMENT ABSTRACT FUNCTIONS ***
     @classmethod
     def _eventFilter(cls, mode:ExtractionMode) -> List[str]:
         return ["CUSTOM.1"]
         # return ["SLIDER_MOVE_RELEASE"]
 
     @classmethod
     def _featureFilter(cls, mode:ExtractionMode) -> List[str]:
         return []
 
     def _updateFromEvent(self, event:Event) -> None:
-        self._ranges.append(event.EventData["max_val"] - event.EventData["min_val"])
+        self._std_devs.append(event.EventData["stdev_val"])
 
     def _updateFromFeatureData(self, feature:FeatureData):
         return
 
     def _getFeatureValues(self) -> List[Any]:
-        if len(self._ranges) > 0:
-            return [sum(self._ranges) / len(self._ranges)]
+        if len(self._std_devs) > 0:
+            return [sum(self._std_devs) / len(self._std_devs)]
         else:
             return [None]
 
     # *** Optionally override public functions. ***
```

### Comparing `opengamedata_core-0.0.5/src/ogd/games/WAVES/features/OverallSliderAverageStandardDeviations.py` & `opengamedata_core-0.0.6/src/ogd/games/WAVES/features/OverallSliderAverageRange.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 # import libraries
-from ogd.core.schemas import Event
+from ogd.core.models import Event
 from typing import Any, List, Optional
 # import locals
 from ogd.core.generators.extractors.SessionFeature import SessionFeature
 from ogd.core.generators.Generator import GeneratorParameters
-from ogd.core.schemas.Event import Event
-from ogd.core.schemas.ExtractionMode import ExtractionMode
-from ogd.core.schemas.FeatureData import FeatureData
+from ogd.core.models.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
+from ogd.core.models.FeatureData import FeatureData
 
-class OverallSliderAverageStandardDeviations(SessionFeature):
+class OverallSliderAverageRange(SessionFeature):
     def __init__(self, params:GeneratorParameters):
         SessionFeature.__init__(self, params=params)
-        self._std_devs = []
+        self._ranges = []
 
     # *** IMPLEMENT ABSTRACT FUNCTIONS ***
     @classmethod
     def _eventFilter(cls, mode:ExtractionMode) -> List[str]:
         return ["CUSTOM.1"]
         # return ["SLIDER_MOVE_RELEASE"]
 
     @classmethod
     def _featureFilter(cls, mode:ExtractionMode) -> List[str]:
         return []
 
     def _updateFromEvent(self, event:Event) -> None:
-        self._std_devs.append(event.EventData["stdev_val"])
+        self._ranges.append(event.EventData["max_val"] - event.EventData["min_val"])
 
     def _updateFromFeatureData(self, feature:FeatureData):
         return
 
     def _getFeatureValues(self) -> List[Any]:
-        if len(self._std_devs) > 0:
-            return [sum(self._std_devs) / len(self._std_devs)]
+        if len(self._ranges) > 0:
+            return [sum(self._ranges) / len(self._ranges)]
         else:
             return [None]
 
     # *** Optionally override public functions. ***
```

### Comparing `opengamedata_core-0.0.5/src/ogd/games/WAVES/features/PercentAmplitudeGoodMoves.py` & `opengamedata_core-0.0.6/src/ogd/games/WAVES/features/AmplitudeGoodMoveCount.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,46 +1,43 @@
 # import libraries
-from ogd.core.schemas import Event
+from ogd.core.models import Event
 from typing import Any, List, Optional
 # import locals
-from ogd.core.generators.extractors.Feature import Feature
 from ogd.core.generators.extractors.PerLevelFeature import PerLevelFeature
 from ogd.core.generators.Generator import GeneratorParameters
-from ogd.core.schemas.Event import Event
-from ogd.core.schemas.ExtractionMode import ExtractionMode
-from ogd.core.schemas.FeatureData import FeatureData
+from ogd.core.models.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
+from ogd.core.models.FeatureData import FeatureData
 
-class PercentAmplitudeGoodMoves(PerLevelFeature):
+class AmplitudeGoodMoveCount(PerLevelFeature):
     def __init__(self, params:GeneratorParameters):
-        Feature.__init__(self, params=params)
-        self._amplitude_count = 0
-        self._good_count = 0
+        PerLevelFeature.__init__(self, params=params)
+        self._count = 0
 
     # *** IMPLEMENT ABSTRACT FUNCTIONS ***
     @classmethod
     def _eventFilter(cls, mode:ExtractionMode) -> List[str]:
         return ["CUSTOM.1", "CUSTOM.2"]
         # return ["SLIDER_MOVE_RELEASE", "ARROW_MOVE_RELEASE"]
 
     @classmethod
     def _featureFilter(cls, mode:ExtractionMode) -> List[str]:
         return []
 
     def _updateFromEvent(self, event:Event) -> None:
         if event.EventData['slider'].upper() == 'AMPLITUDE':
-            self._amplitude_count += 1
             if event.EventName == "CUSTOM.1":
                 if event.EventData['end_closeness'] > event.EventData['begin_closeness']:
-                    self._good_count += 1
+                    self._count += 1
             elif event.EventName == "CUSTOM.2":
                 start_dist = event.EventData['correct_val'] - event.EventData['begin_val']
                 end_dist = event.EventData['correct_val'] - event.EventData['end_val']
                 if abs(end_dist) < abs(start_dist):
-                    self._good_count += 1
+                    self._count += 1
 
     def _updateFromFeatureData(self, feature:FeatureData):
         return
 
     def _getFeatureValues(self) -> List[Any]:
-        return [self._good_count / self._amplitude_count if self._amplitude_count != 0 else None]
+        return [self._count]
 
     # *** Optionally override public functions. ***
```

### Comparing `opengamedata_core-0.0.5/src/ogd/games/WAVES/features/PercentAmplitudeMoves.py` & `opengamedata_core-0.0.6/src/ogd/games/WAVES/features/SliderAverageStandardDeviations.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,39 +1,38 @@
-# import libraries
-from ogd.core.schemas import Event
+# import locals
+import typing
 from typing import Any, List, Optional
 # import locals
-from ogd.core.generators.extractors.Feature import Feature
 from ogd.core.generators.extractors.PerLevelFeature import PerLevelFeature
 from ogd.core.generators.Generator import GeneratorParameters
-from ogd.core.schemas.Event import Event
-from ogd.core.schemas.ExtractionMode import ExtractionMode
-from ogd.core.schemas.FeatureData import FeatureData
+from ogd.core.models.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
+from ogd.core.models.FeatureData import FeatureData
 
-class PercentAmplitudeMoves(PerLevelFeature):
+class SliderAverageStandardDeviations(PerLevelFeature):
     def __init__(self, params:GeneratorParameters):
-        Feature.__init__(self, params=params)
-        self._amplitude_count = 0
-        self._count = 0
+        PerLevelFeature.__init__(self, params=params)
+        self._std_devs = []
 
     # *** IMPLEMENT ABSTRACT FUNCTIONS ***
     @classmethod
     def _eventFilter(cls, mode:ExtractionMode) -> List[str]:
-        return ["CUSTOM.1", "CUSTOM.2"]
-        # return ["SLIDER_MOVE_RELEASE", "ARROW_MOVE_RELEASE"]
+        return ["CUSTOM.1"]
+        # return ["SLIDER_MOVE_RELEASE"]
 
     @classmethod
     def _featureFilter(cls, mode:ExtractionMode) -> List[str]:
         return []
 
     def _updateFromEvent(self, event:Event) -> None:
-        self._count += 1
-        if event.EventData['slider'].upper() == 'AMPLITUDE':
-            self._amplitude_count += 1
+        self._std_devs.append(event.EventData["stdev_val"])
 
     def _updateFromFeatureData(self, feature:FeatureData):
         return
 
     def _getFeatureValues(self) -> List[Any]:
-        return [self._amplitude_count / self._count if self._count != 0 else None]
+        if len(self._std_devs) > 0:
+            return [sum(self._std_devs) / len(self._std_devs)]
+        else:
+            return [None]
 
     # *** Optionally override public functions. ***
```

### Comparing `opengamedata_core-0.0.5/src/ogd/games/WAVES/features/PercentOffsetGoodMoves.py` & `opengamedata_core-0.0.6/src/ogd/games/WAVES/features/PercentWavelengthGoodMoves.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,46 +1,46 @@
 # import libraries
-from ogd.core.schemas import Event
+from ogd.core.models import Event
 from typing import Any, List, Optional
 # import locals
 from ogd.core.generators.extractors.Feature import Feature
-from ogd.core.generators.extractors.PerLevelFeature import PerLevelFeature
 from ogd.core.generators.Generator import GeneratorParameters
-from ogd.core.schemas.Event import Event
-from ogd.core.schemas.ExtractionMode import ExtractionMode
-from ogd.core.schemas.FeatureData import FeatureData
+from ogd.core.models.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
+from ogd.core.models.FeatureData import FeatureData
 
-class PercentOffsetGoodMoves(PerLevelFeature):
+
+class PercentWavelengthGoodMoves(Feature):
     def __init__(self, params:GeneratorParameters):
         Feature.__init__(self, params=params)
-        self._offset_count = 0
+        self._wavelength_count = 0
         self._good_count = 0
 
     # *** IMPLEMENT ABSTRACT FUNCTIONS ***
     @classmethod
     def _eventFilter(cls, mode:ExtractionMode) -> List[str]:
         return ["CUSTOM.1", "CUSTOM.2"]
         # return ["SLIDER_MOVE_RELEASE", "ARROW_MOVE_RELEASE"]
 
     @classmethod
     def _featureFilter(cls, mode:ExtractionMode) -> List[str]:
         return []
 
     def _updateFromEvent(self, event:Event) -> None:
-        if event.EventData['slider'].upper() == 'OFFSET':
-            self._offset_count += 1
+        if event.EventData['slider'].upper() == 'WAVELENGTH':
+            self._wavelength_count += 1
             if event.EventName == "CUSTOM.1":
                 if event.EventData['end_closeness'] > event.EventData['begin_closeness']:
                     self._good_count += 1
             elif event.EventName == "CUSTOM.2":
                 start_dist = event.EventData['correct_val'] - event.EventData['begin_val']
                 end_dist = event.EventData['correct_val'] - event.EventData['end_val']
                 if abs(end_dist) < abs(start_dist):
                     self._good_count += 1
 
     def _updateFromFeatureData(self, feature:FeatureData):
         return
 
     def _getFeatureValues(self) -> List[Any]:
-        return [self._good_count / self._offset_count if self._offset_count != 0 else None]
+        return [self._good_count / self._wavelength_count if self._wavelength_count != 0 else None]
 
     # *** Optionally override public functions. ***
```

### Comparing `opengamedata_core-0.0.5/src/ogd/games/WAVES/features/PercentOffsetMoves.py` & `opengamedata_core-0.0.6/src/ogd/games/WAVES/features/PercentWavelengthMoves.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 # import libraries
-from ogd.core.schemas import Event
+from ogd.core.models import Event
 from typing import Any, List, Optional
 # import locals
 from ogd.core.generators.extractors.Feature import Feature
 from ogd.core.generators.Generator import GeneratorParameters
-from ogd.core.schemas.Event import Event
-from ogd.core.schemas.ExtractionMode import ExtractionMode
-from ogd.core.schemas.FeatureData import FeatureData
+from ogd.core.models.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
+from ogd.core.models.FeatureData import FeatureData
 
 
-class PercentOffsetMoves(Feature):
+class PercentWavelengthMoves(Feature):
     def __init__(self, params:GeneratorParameters):
         Feature.__init__(self, params=params)
-        self._offset_count = 0
+        self._wavelength_count = 0
         self._count = 0
 
     # *** IMPLEMENT ABSTRACT FUNCTIONS ***
     @classmethod
     def _eventFilter(cls, mode:ExtractionMode) -> List[str]:
         return ["CUSTOM.1", "CUSTOM.2"]
         # return ["SLIDER_MOVE_RELEASE", "ARROW_MOVE_RELEASE"]
 
     @classmethod
     def _featureFilter(cls, mode:ExtractionMode) -> List[str]:
         return []
 
     def _updateFromEvent(self, event:Event) -> None:
         self._count += 1
-        if event.EventData['slider'].upper() == 'OFFSET':
-            self._offset_count += 1
+        if event.EventData['slider'].upper() == 'WAVELENGTH':
+            self._wavelength_count += 1
 
     def _updateFromFeatureData(self, feature:FeatureData):
         return
 
     def _getFeatureValues(self) -> List[Any]:
-        return [self._offset_count / self._count if self._count != 0 else None]
+        return [self._wavelength_count / self._count if self._count != 0 else None]
 
     # *** Optionally override public functions. ***
```

### Comparing `opengamedata_core-0.0.5/src/ogd/games/WAVES/features/PercentWavelengthGoodMoves.py` & `opengamedata_core-0.0.6/src/ogd/games/WAVES/features/OverallPercentWavelengthMoves.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,46 +1,43 @@
 # import libraries
-from ogd.core.schemas import Event
+from ogd.core.models import Event
 from typing import Any, List, Optional
 # import locals
-from ogd.core.generators.extractors.Feature import Feature
+from ogd.core.generators.extractors.SessionFeature import SessionFeature
 from ogd.core.generators.Generator import GeneratorParameters
-from ogd.core.schemas.Event import Event
-from ogd.core.schemas.ExtractionMode import ExtractionMode
-from ogd.core.schemas.FeatureData import FeatureData
+from ogd.core.models.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
+from ogd.core.models.FeatureData import FeatureData
 
-
-class PercentWavelengthGoodMoves(Feature):
+class OverallPercentWavelengthMoves(SessionFeature):
     def __init__(self, params:GeneratorParameters):
-        Feature.__init__(self, params=params)
+        SessionFeature.__init__(self, params=params)
         self._wavelength_count = 0
-        self._good_count = 0
+        self._move_count = 0
 
     # *** IMPLEMENT ABSTRACT FUNCTIONS ***
     @classmethod
     def _eventFilter(cls, mode:ExtractionMode) -> List[str]:
         return ["CUSTOM.1", "CUSTOM.2"]
         # return ["SLIDER_MOVE_RELEASE", "ARROW_MOVE_RELEASE"]
 
     @classmethod
     def _featureFilter(cls, mode:ExtractionMode) -> List[str]:
         return []
 
     def _updateFromEvent(self, event:Event) -> None:
-        if event.EventData['slider'].upper() == 'WAVELENGTH':
+        self._move_count += 1
+        if event.EventData["slider"].upper() == "WAVELENGTH":
             self._wavelength_count += 1
-            if event.EventName == "CUSTOM.1":
-                if event.EventData['end_closeness'] > event.EventData['begin_closeness']:
-                    self._good_count += 1
-            elif event.EventName == "CUSTOM.2":
-                start_dist = event.EventData['correct_val'] - event.EventData['begin_val']
-                end_dist = event.EventData['correct_val'] - event.EventData['end_val']
-                if abs(end_dist) < abs(start_dist):
-                    self._good_count += 1
 
     def _updateFromFeatureData(self, feature:FeatureData):
         return
 
     def _getFeatureValues(self) -> List[Any]:
-        return [self._good_count / self._wavelength_count if self._wavelength_count != 0 else None]
+        if self._move_count > 0:
+            return [self._wavelength_count / self._move_count * 100]
+        else:
+            return [None]
 
     # *** Optionally override public functions. ***
+
+
```

### Comparing `opengamedata_core-0.0.5/src/ogd/games/WAVES/features/PercentWavelengthMoves.py` & `opengamedata_core-0.0.6/src/ogd/games/WAVES/features/TotalSliderMoves.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,39 +1,35 @@
 # import libraries
-from ogd.core.schemas import Event
+from ogd.core.models import Event
 from typing import Any, List, Optional
 # import locals
-from ogd.core.generators.extractors.Feature import Feature
+from ogd.core.generators.extractors.PerLevelFeature import PerLevelFeature
 from ogd.core.generators.Generator import GeneratorParameters
-from ogd.core.schemas.Event import Event
-from ogd.core.schemas.ExtractionMode import ExtractionMode
-from ogd.core.schemas.FeatureData import FeatureData
+from ogd.core.models.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
+from ogd.core.models.FeatureData import FeatureData
 
-
-class PercentWavelengthMoves(Feature):
+class TotalSliderMoves(PerLevelFeature):
     def __init__(self, params:GeneratorParameters):
-        Feature.__init__(self, params=params)
-        self._wavelength_count = 0
-        self._count = 0
+        PerLevelFeature.__init__(self, params=params)
+        self._slider_move_count : int = 0
 
     # *** IMPLEMENT ABSTRACT FUNCTIONS ***
     @classmethod
     def _eventFilter(cls, mode:ExtractionMode) -> List[str]:
-        return ["CUSTOM.1", "CUSTOM.2"]
-        # return ["SLIDER_MOVE_RELEASE", "ARROW_MOVE_RELEASE"]
+        return ["CUSTOM.1"]
+        # return ["SLIDER_MOVE_RELEASE"]
 
     @classmethod
     def _featureFilter(cls, mode:ExtractionMode) -> List[str]:
         return []
 
     def _updateFromEvent(self, event:Event) -> None:
-        self._count += 1
-        if event.EventData['slider'].upper() == 'WAVELENGTH':
-            self._wavelength_count += 1
+            self._slider_move_count += 1
 
     def _updateFromFeatureData(self, feature:FeatureData):
         return
 
     def _getFeatureValues(self) -> List[Any]:
-        return [self._wavelength_count / self._count if self._count != 0 else None]
+        return [self._slider_move_count]
 
     # *** Optionally override public functions. ***
```

### Comparing `opengamedata_core-0.0.5/src/ogd/games/WAVES/features/PersistentSessionID.py` & `opengamedata_core-0.0.6/src/ogd/games/AQUALAB/features/UserAvgSessionDuration.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,37 +1,42 @@
 # import libraries
-from ogd.core.schemas import Event
-from typing import Any, List, Optional
+from typing import Any, List
 # import locals
-from ogd.core.generators.extractors.SessionFeature import SessionFeature
 from ogd.core.generators.Generator import GeneratorParameters
-from ogd.core.schemas.Event import Event
-from ogd.core.schemas.ExtractionMode import ExtractionMode
-from ogd.core.schemas.FeatureData import FeatureData
-
-class PersistentSessionID(SessionFeature):
-    def __init__(self, params:GeneratorParameters):
-        SessionFeature.__init__(self, params=params)
-        self._persistent_id : Optional[int] = None
+from ogd.core.generators.extractors.SessionFeature import SessionFeature
+from ogd.core.models.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
+from ogd.core.models.FeatureData import FeatureData
+
+class UserAvgSessionDuration(SessionFeature):
+
+    def __init__(self, params:GeneratorParameters, player_id:str):
+        self._player_id = player_id
+        super().__init__(params=params)
+        self._times : List[int] = []
 
     # *** IMPLEMENT ABSTRACT FUNCTIONS ***
     @classmethod
     def _eventFilter(cls, mode:ExtractionMode) -> List[str]:
-        return ["BEGIN.0"]
+        return []
 
     @classmethod
     def _featureFilter(cls, mode:ExtractionMode) -> List[str]:
-        return []
+        return ["SessionDuration"]
 
     def _updateFromEvent(self, event:Event) -> None:
-        if self._persistent_id is None:
-            self._persistent_id = event.UserData['persistent_session_id']
+        return
 
     def _updateFromFeatureData(self, feature:FeatureData):
-        return
+        if feature.PlayerID == self._player_id:
+            if feature.FeatureValues[0] == "No events":
+                pass
+            else:
+                self._times.append(feature.FeatureValues[0].total_seconds())
 
     def _getFeatureValues(self) -> List[Any]:
-        return [self._persistent_id]
+        if len(self._times) > 0:
+            return [sum(self._times) / len(self._times)]
+        else:
+            return [0]
 
     # *** Optionally override public functions. ***
-
-
```

### Comparing `opengamedata_core-0.0.5/src/ogd/games/WAVES/features/QuestionAnswered.py` & `opengamedata_core-0.0.6/src/ogd/games/WAVES/features/QuestionAnswered.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # import libraries
-from ogd.core.schemas import Event
+from ogd.core.models import Event
 from typing import Any, List, Optional
 # import locals
 from ogd.core.generators.extractors.Feature import Feature
 from ogd.core.generators.Generator import GeneratorParameters
-from ogd.core.schemas.Event import Event
-from ogd.core.schemas.ExtractionMode import ExtractionMode
-from ogd.core.schemas.FeatureData import FeatureData
+from ogd.core.models.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
+from ogd.core.models.FeatureData import FeatureData
 
 
 class QuestionAnswered(Feature):
     def __init__(self, params:GeneratorParameters):
         Feature.__init__(self, params=params)
         self._answer = None
```

### Comparing `opengamedata_core-0.0.5/src/ogd/games/WAVES/features/QuestionCorrect.py` & `opengamedata_core-0.0.6/src/ogd/games/WAVES/features/QuestionCorrect.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # import libraries
-from ogd.core.schemas import Event
+from ogd.core.models import Event
 from typing import Any, List, Optional
 # import locals
 from ogd.core.generators.extractors.Feature import Feature
 from ogd.core.generators.Generator import GeneratorParameters
-from ogd.core.schemas.Event import Event
-from ogd.core.schemas.ExtractionMode import ExtractionMode
-from ogd.core.schemas.FeatureData import FeatureData
+from ogd.core.models.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
+from ogd.core.models.FeatureData import FeatureData
 
 
 class QuestionCorrect(Feature):
     def __init__(self, params:GeneratorParameters):
         Feature.__init__(self, params=params)
         self._correct = None
```

### Comparing `opengamedata_core-0.0.5/src/ogd/games/WAVES/features/RangeIntercept.py` & `opengamedata_core-0.0.6/src/ogd/games/AQUALAB/features/TotalHelpCount.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,33 +1,37 @@
-# import libraries
-from ogd.core.schemas import Event
-from typing import Any, List, Optional
+from typing import Any, List
 # import locals
-from ogd.core.generators.extractors.Feature import Feature
 from ogd.core.generators.Generator import GeneratorParameters
-from ogd.core.schemas.Event import Event
-from ogd.core.schemas.ExtractionMode import ExtractionMode
-from ogd.core.schemas.FeatureData import FeatureData
-
-class RangeIntercept(Feature):
+from ogd.core.generators.extractors.Feature import Feature
+from ogd.core.models.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
+from ogd.core.models.FeatureData import FeatureData
+
+class TotalHelpCount(Feature):
+    """_summary_
+
+    :param Feature: _description_
+    :type Feature: _type_
+    """
     def __init__(self, params:GeneratorParameters):
-        Feature.__init__(self, params=params)
+        super().__init__(params=params)
+        self._count = 0
 
     # *** IMPLEMENT ABSTRACT FUNCTIONS ***
     @classmethod
     def _eventFilter(cls, mode:ExtractionMode) -> List[str]:
-        return []
+        return ["ask_for_help"]
 
     @classmethod
     def _featureFilter(cls, mode:ExtractionMode) -> List[str]:
         return []
 
     def _updateFromEvent(self, event:Event) -> None:
-        return
+        self._count += 1
 
     def _updateFromFeatureData(self, feature:FeatureData):
         return
 
     def _getFeatureValues(self) -> List[Any]:
-        return ["Not Implemented"]
+        return [self._count]
 
     # *** Optionally override public functions. ***
```

### Comparing `opengamedata_core-0.0.5/src/ogd/games/WAVES/features/RangeR2.py` & `opengamedata_core-0.0.6/src/ogd/games/WAVES/features/ClosenessR2.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 # import libraries
-from ogd.core.schemas import Event
+from ogd.core.models import Event
 from typing import Any, List, Optional
 # import locals
 from ogd.core.generators.extractors.Feature import Feature
 from ogd.core.generators.Generator import GeneratorParameters
-from ogd.core.schemas.Event import Event
-from ogd.core.schemas.ExtractionMode import ExtractionMode
-from ogd.core.schemas.FeatureData import FeatureData
+from ogd.core.models.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
+from ogd.core.models.FeatureData import FeatureData
 
-class RangeR2(Feature):
+class ClosenessR2(Feature):
     def __init__(self, params:GeneratorParameters):
         Feature.__init__(self, params=params)
 
     # *** IMPLEMENT ABSTRACT FUNCTIONS ***
     @classmethod
     def _eventFilter(cls, mode:ExtractionMode) -> List[str]:
         return []
```

### Comparing `opengamedata_core-0.0.5/src/ogd/games/WAVES/features/RangeSlope.py` & `opengamedata_core-0.0.6/src/ogd/games/WAVES/features/RangeSlope.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # import libraries
-from ogd.core.schemas import Event
+from ogd.core.models import Event
 from typing import Any, List, Optional
 # import locals
 from ogd.core.generators.extractors.Feature import Feature
 from ogd.core.generators.Generator import GeneratorParameters
-from ogd.core.schemas.Event import Event
-from ogd.core.schemas.ExtractionMode import ExtractionMode
-from ogd.core.schemas.FeatureData import FeatureData
+from ogd.core.models.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
+from ogd.core.models.FeatureData import FeatureData
 
 class RangeSlope(Feature):
     def __init__(self, params:GeneratorParameters):
         Feature.__init__(self, params=params)
 
     # *** IMPLEMENT ABSTRACT FUNCTIONS ***
     @classmethod
```

### Comparing `opengamedata_core-0.0.5/src/ogd/games/WAVES/features/SequenceLevel.py` & `opengamedata_core-0.0.6/src/ogd/games/WAVES/features/SequenceLevel.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # import libraries
-from ogd.core.schemas import Event
+from ogd.core.models import Event
 from typing import Any, List, Optional
 # import locals
 from ogd.core.generators.extractors.PerLevelFeature import PerLevelFeature
 from ogd.core.generators.Generator import GeneratorParameters
-from ogd.core.schemas.Event import Event
-from ogd.core.schemas.ExtractionMode import ExtractionMode
-from ogd.core.schemas.FeatureData import FeatureData
+from ogd.core.models.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
+from ogd.core.models.FeatureData import FeatureData
 
 class SequenceLevel(PerLevelFeature):
     def __init__(self, params:GeneratorParameters):
         PerLevelFeature.__init__(self, params=params)
         self._seq = ''
         self._lastSliderType = ''
```

### Comparing `opengamedata_core-0.0.5/src/ogd/games/WAVES/features/SessionID.py` & `opengamedata_core-0.0.6/src/ogd/games/PENGUINS/features/SkuaPeckCount.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 # import libraries
-from ogd.core.schemas import Event
-from typing import Any, List, Optional
+import logging
+from typing import Any, Dict, List, Optional
 # import locals
-from ogd.core.generators.extractors.SessionFeature import SessionFeature
+from ogd.core.utils.Logger import Logger
 from ogd.core.generators.Generator import GeneratorParameters
-from ogd.core.schemas.Event import Event
-from ogd.core.schemas.ExtractionMode import ExtractionMode
-from ogd.core.schemas.FeatureData import FeatureData
-
-class SessionID(SessionFeature):
-    def __init__(self, params:GeneratorParameters, sessionID:str):
-        SessionFeature.__init__(self, params=params)
-        self._sessionID = sessionID
+from ogd.core.models.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
+from ogd.core.models.FeatureData import FeatureData
+from ogd.core.generators.extractors.SessionFeature import SessionFeature
+
+
+class SkuaPeckCount(SessionFeature):
+
+    def __init__(self, params:GeneratorParameters):
+        super().__init__(params=params)
+        self._current_count : int = 0
 
     # *** IMPLEMENT ABSTRACT FUNCTIONS ***
     @classmethod
     def _eventFilter(cls, mode:ExtractionMode) -> List[str]:
-        return []
+        return ["peck_skua"]
 
     @classmethod
     def _featureFilter(cls, mode:ExtractionMode) -> List[str]:
         return []
 
     def _updateFromEvent(self, event:Event) -> None:
-        return
+        self._current_count += 1
 
     def _updateFromFeatureData(self, feature:FeatureData):
         return
 
     def _getFeatureValues(self) -> List[Any]:
-        return [self._sessionID]
-
-    # *** Optionally override public functions. ***
-
+        return [self._current_count]
```

### Comparing `opengamedata_core-0.0.5/src/ogd/games/WAVES/features/SliderAverageRange.py` & `opengamedata_core-0.0.6/src/ogd/games/WAVES/features/SliderAverageRange.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # import libraries
-from ogd.core.schemas import Event
+from ogd.core.models import Event
 import typing
 from typing import Any, List, Optional
 # import locals
 from ogd.core.generators.extractors.PerLevelFeature import PerLevelFeature
 from ogd.core.generators.Generator import GeneratorParameters
-from ogd.core.schemas.Event import Event
-from ogd.core.schemas.ExtractionMode import ExtractionMode
-from ogd.core.schemas.FeatureData import FeatureData
+from ogd.core.models.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
+from ogd.core.models.FeatureData import FeatureData
 
 class SliderAverageRange(PerLevelFeature):
     def __init__(self, params:GeneratorParameters):
         PerLevelFeature.__init__(self, params=params)
         self._ranges = []
 
     # *** IMPLEMENT ABSTRACT FUNCTIONS ***
```

### Comparing `opengamedata_core-0.0.5/src/ogd/games/WAVES/features/SliderAverageStandardDeviations.py` & `opengamedata_core-0.0.6/src/ogd/games/PENGUINS/features/EggLostCount.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,38 +1,37 @@
+# import libraries
+import logging
+from typing import Any, Dict, List, Optional
 # import locals
-import typing
-from typing import Any, List, Optional
-# import locals
-from ogd.core.generators.extractors.PerLevelFeature import PerLevelFeature
+from ogd.core.utils.Logger import Logger
 from ogd.core.generators.Generator import GeneratorParameters
-from ogd.core.schemas.Event import Event
-from ogd.core.schemas.ExtractionMode import ExtractionMode
-from ogd.core.schemas.FeatureData import FeatureData
+from ogd.core.models.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
+from ogd.core.models.FeatureData import FeatureData
+from ogd.core.generators.extractors.SessionFeature import SessionFeature
+
+
+class EggLostCount(SessionFeature):
 
-class SliderAverageStandardDeviations(PerLevelFeature):
     def __init__(self, params:GeneratorParameters):
-        PerLevelFeature.__init__(self, params=params)
-        self._std_devs = []
+        super().__init__(params=params)
+        self._current_count : int = 0
 
     # *** IMPLEMENT ABSTRACT FUNCTIONS ***
     @classmethod
     def _eventFilter(cls, mode:ExtractionMode) -> List[str]:
-        return ["CUSTOM.1"]
-        # return ["SLIDER_MOVE_RELEASE"]
+        return ["egg_lost"]
 
     @classmethod
     def _featureFilter(cls, mode:ExtractionMode) -> List[str]:
         return []
 
     def _updateFromEvent(self, event:Event) -> None:
-        self._std_devs.append(event.EventData["stdev_val"])
+        self._current_count += 1
 
     def _updateFromFeatureData(self, feature:FeatureData):
         return
 
     def _getFeatureValues(self) -> List[Any]:
-        if len(self._std_devs) > 0:
-            return [sum(self._std_devs) / len(self._std_devs)]
-        else:
-            return [None]
+        return [self._current_count]
 
-    # *** Optionally override public functions. ***
+
```

### Comparing `opengamedata_core-0.0.5/src/ogd/games/WAVES/features/SucceedCount.py` & `opengamedata_core-0.0.6/src/ogd/games/WAVES/features/SucceedCount.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # import libraries
 import typing
 from typing import Any, List, Optional
 # import locals
 from ogd.core.generators.extractors.PerLevelFeature import PerLevelFeature
 from ogd.core.generators.Generator import GeneratorParameters
-from ogd.core.schemas.Event import Event
-from ogd.core.schemas.ExtractionMode import ExtractionMode
-from ogd.core.schemas.FeatureData import FeatureData
+from ogd.core.models.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
+from ogd.core.models.FeatureData import FeatureData
 
 class SucceedCount(PerLevelFeature):
     def __init__(self, params:GeneratorParameters):
         PerLevelFeature.__init__(self, params=params)
         self._succeed_count = 0
 
     # *** IMPLEMENT ABSTRACT FUNCTIONS ***
```

### Comparing `opengamedata_core-0.0.5/src/ogd/games/WAVES/features/TimeToAnswerMS.py` & `opengamedata_core-0.0.6/src/ogd/games/WAVES/features/TimeToAnswerMS.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # import libraries
-from ogd.core.schemas import Event
+from ogd.core.models import Event
 import typing
 from typing import Any, List, Optional
 # import locals
 from ogd.core.generators.extractors.Feature import Feature
 from ogd.core.generators.Generator import GeneratorParameters
-from ogd.core.schemas.Event import Event
-from ogd.core.schemas.ExtractionMode import ExtractionMode
-from ogd.core.schemas.FeatureData import FeatureData
+from ogd.core.models.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
+from ogd.core.models.FeatureData import FeatureData
 
 class TimeToAnswerMS(Feature):
     def __init__(self, params:GeneratorParameters):
         Feature.__init__(self, params=params)
         self._latest_complete_lvl8  = None
         self._latest_complete_lvl16 = None
         self._latest_answer_Q0 = None
```

### Comparing `opengamedata_core-0.0.5/src/ogd/games/WAVES/features/TotalArrowMoves.py` & `opengamedata_core-0.0.6/src/ogd/games/PENGUINS/features/RockMultiplePickupCount.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,35 +1,43 @@
 # import libraries
-from ogd.core.schemas import Event
-from typing import Any, List, Optional
+import logging
+from typing import Any, Dict, List, Optional
 # import locals
-from ogd.core.generators.extractors.PerLevelFeature import PerLevelFeature
+from ogd.core.utils.Logger import Logger
 from ogd.core.generators.Generator import GeneratorParameters
-from ogd.core.schemas.Event import Event
-from ogd.core.schemas.ExtractionMode import ExtractionMode
-from ogd.core.schemas.FeatureData import FeatureData
+from ogd.core.models.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
+from ogd.core.models.FeatureData import FeatureData
+from ogd.core.generators.extractors.SessionFeature import SessionFeature
 
-class TotalArrowMoves(PerLevelFeature):
+
+class RockMultiplePickupCount(SessionFeature):
+    """Template file to serve as a guide for creating custom Feature subclasses for games.
+
+    :param Feature: Base class for a Custom Feature class.
+    :type Feature: _type_
+    """
     def __init__(self, params:GeneratorParameters):
-        PerLevelFeature.__init__(self, params=params)
-        self._arrow_move_count : int = 0
+        super().__init__(params=params)
+        self._current_count : int = 0
 
     # *** IMPLEMENT ABSTRACT FUNCTIONS ***
+
     @classmethod
     def _eventFilter(cls, mode:ExtractionMode) -> List[str]:
-        return ["CUSTOM.2"]
-        # return ["ARROW_MOVE_RELEASE"]
+        return ["peck_rock"]
 
     @classmethod
     def _featureFilter(cls, mode:ExtractionMode) -> List[str]:
-        return []
+        return [] 
 
     def _updateFromEvent(self, event:Event) -> None:
-        self._arrow_move_count += 1
+        # if has_rock does not exit it will return false as well
+        if event.game_state.get("has_rock", False):
+            self._current_count += 1
+        
 
-    def _updateFromFeatureData(self, feature:FeatureData):
+    def _updateFromFeatureData(self, feature: FeatureData):
         return
 
     def _getFeatureValues(self) -> List[Any]:
-        return [self._arrow_move_count]
-
-    # *** Optionally override public functions. ***
+        return [self._current_count]
```

### Comparing `opengamedata_core-0.0.5/src/ogd/games/WAVES/features/TotalFails.py` & `opengamedata_core-0.0.6/src/ogd/games/WAVES/features/TotalSkips.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,34 +1,36 @@
-from ogd.core.schemas import Event
+# import libraries
+from ogd.core.models import Event
 import typing
 from typing import Any, List, Optional
 # import locals
 from ogd.core.generators.extractors.PerLevelFeature import PerLevelFeature
 from ogd.core.generators.Generator import GeneratorParameters
-from ogd.core.schemas.Event import Event
-from ogd.core.schemas.ExtractionMode import ExtractionMode
-from ogd.core.schemas.FeatureData import FeatureData
+from ogd.core.models.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
+from ogd.core.models.FeatureData import FeatureData
 
-class TotalFails(PerLevelFeature):
+class TotalSkips(PerLevelFeature):
     def __init__(self, params:GeneratorParameters):
         PerLevelFeature.__init__(self, params=params)
-        self._fail_count = 0
+        self._skip_count = 0
 
     # *** IMPLEMENT ABSTRACT FUNCTIONS ***
     @classmethod
     def _eventFilter(cls, mode:ExtractionMode) -> List[str]:
-        return ["FAIL.0"]
+        return ["CUSTOM.6"]
+        # "events": ["SKIP_BUTTON"],
 
     @classmethod
     def _featureFilter(cls, mode:ExtractionMode) -> List[str]:
         return []
 
     def _updateFromEvent(self, event:Event) -> None:
-        self._fail_count += 1
+        self._skip_count += 1
 
     def _updateFromFeatureData(self, feature:FeatureData):
         return
 
     def _getFeatureValues(self) -> List[Any]:
-        return [self._fail_count]
+        return [self._skip_count]
 
     # *** Optionally override public functions. ***
```

### Comparing `opengamedata_core-0.0.5/src/ogd/games/WAVES/features/TotalLevelTime.py` & `opengamedata_core-0.0.6/src/ogd/games/WAVES/features/TotalLevelTime.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 # import libraries
 import logging
 from datetime import datetime
-from ogd.core.schemas import Event
+from ogd.core.models import Event
 from typing import Any, List, Optional
 # import locals
 from ogd.core.utils.Logger import Logger
 from ogd.core.generators.extractors.PerLevelFeature import PerLevelFeature
 from ogd.core.generators.Generator import GeneratorParameters
-from ogd.core.schemas.Event import Event
-from ogd.core.schemas.ExtractionMode import ExtractionMode
-from ogd.core.schemas.FeatureData import FeatureData
+from ogd.core.models.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
+from ogd.core.models.FeatureData import FeatureData
 
 class TotalLevelTime(PerLevelFeature):
     def __init__(self, params:GeneratorParameters):
         PerLevelFeature.__init__(self, params=params)
         self._begin_times    : List[datetime] = []
         self._complete_times : List[datetime] = []
```

### Comparing `opengamedata_core-0.0.5/src/ogd/games/WAVES/features/TotalMoveTypeChanges.py` & `opengamedata_core-0.0.6/src/ogd/games/WAVES/features/TotalFails.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,39 +1,34 @@
-# import libraries
-from ogd.core.schemas import Event
+from ogd.core.models import Event
 import typing
 from typing import Any, List, Optional
 # import locals
 from ogd.core.generators.extractors.PerLevelFeature import PerLevelFeature
 from ogd.core.generators.Generator import GeneratorParameters
-from ogd.core.schemas.Event import Event
-from ogd.core.schemas.ExtractionMode import ExtractionMode
-from ogd.core.schemas.FeatureData import FeatureData
+from ogd.core.models.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
+from ogd.core.models.FeatureData import FeatureData
 
-class TotalMoveTypeChanges(PerLevelFeature):
+class TotalFails(PerLevelFeature):
     def __init__(self, params:GeneratorParameters):
         PerLevelFeature.__init__(self, params=params)
-        self._last_move = None
-        self._change_count = 0
+        self._fail_count = 0
 
     # *** IMPLEMENT ABSTRACT FUNCTIONS ***
     @classmethod
     def _eventFilter(cls, mode:ExtractionMode) -> List[str]:
-        return ["CUSTOM.1", "CUSTOM.2"]
-        # return ["SLIDER_MOVE_RELEASE", "ARROW_MOVE_RELEASE"]
+        return ["FAIL.0"]
 
     @classmethod
     def _featureFilter(cls, mode:ExtractionMode) -> List[str]:
         return []
 
     def _updateFromEvent(self, event:Event) -> None:
-        if self._last_move != event.EventName:
-            self._change_count += 1
-        self._last_move = event.EventName
+        self._fail_count += 1
 
     def _updateFromFeatureData(self, feature:FeatureData):
         return
 
     def _getFeatureValues(self) -> List[Any]:
-        return [self._change_count]
+        return [self._fail_count]
 
     # *** Optionally override public functions. ***
```

### Comparing `opengamedata_core-0.0.5/src/ogd/games/WAVES/features/TotalResets.py` & `opengamedata_core-0.0.6/src/ogd/games/JOWILDER/features/GameVersion.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,36 +1,44 @@
 # import libraries
-from ogd.core.schemas import Event
-import typing
-from typing import Any, List, Optional
-# import locals
-from ogd.core.generators.extractors.PerLevelFeature import PerLevelFeature
+from typing import Any, List, Optional, Union
 from ogd.core.generators.Generator import GeneratorParameters
-from ogd.core.schemas.Event import Event
-from ogd.core.schemas.ExtractionMode import ExtractionMode
-from ogd.core.schemas.FeatureData import FeatureData
-
-class TotalResets(PerLevelFeature):
+# import local files
+from ogd.core.generators.extractors.SessionFeature import SessionFeature
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
+from ogd.core.models.FeatureData import FeatureData
+from ogd.core.models.Event import Event
+
+class GameVersion(SessionFeature):
+    """Template file to serve as a guide for creating custom Feature subclasses for games.
+
+    :param Feature: Base class for a Custom Feature class.
+    :type Feature: _type_
+    """
     def __init__(self, params:GeneratorParameters):
-        PerLevelFeature.__init__(self, params=params)
-        self._reset_count = 0
+        super().__init__(params=params)
+        self._version    : Union[str,int,None] = None
+        self._log_version: Union[str,int,None] = None
 
     # *** IMPLEMENT ABSTRACT FUNCTIONS ***
+
     @classmethod
     def _eventFilter(cls, mode:ExtractionMode) -> List[str]:
-        return ["CUSTOM.4"]
-        # "events": ["RESET_BTN_PRESS"],
+        return ["CUSTOM.1"]
 
     @classmethod
     def _featureFilter(cls, mode:ExtractionMode) -> List[str]:
-        return []
+        return [] 
 
     def _updateFromEvent(self, event:Event) -> None:
-        self._reset_count += 1
+        self._version = event.AppVersion
+        self._log_version = event.LogVersion
+        return
 
-    def _updateFromFeatureData(self, feature:FeatureData):
+    def _updateFromFeatureData(self, feature: FeatureData):
         return
 
     def _getFeatureValues(self) -> List[Any]:
-        return [self._reset_count]
+        return [self._version, self._log_version]
+
+    def Subfeatures(self) -> List[str]:
+        return ["Log"]
 
-    # *** Optionally override public functions. ***
```

### Comparing `opengamedata_core-0.0.5/src/ogd/games/WAVES/features/TotalSkips.py` & `opengamedata_core-0.0.6/src/ogd/games/AQUALAB/features/JobGuideCount.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,36 +1,40 @@
 # import libraries
-from ogd.core.schemas import Event
-import typing
+import logging
 from typing import Any, List, Optional
 # import locals
-from ogd.core.generators.extractors.PerLevelFeature import PerLevelFeature
+from ogd.core.utils.Logger import Logger
 from ogd.core.generators.Generator import GeneratorParameters
-from ogd.core.schemas.Event import Event
-from ogd.core.schemas.ExtractionMode import ExtractionMode
-from ogd.core.schemas.FeatureData import FeatureData
-
-class TotalSkips(PerLevelFeature):
-    def __init__(self, params:GeneratorParameters):
-        PerLevelFeature.__init__(self, params=params)
-        self._skip_count = 0
+from ogd.games.AQUALAB.features.PerJobFeature import PerJobFeature
+from ogd.core.models.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
+from ogd.core.models.FeatureData import FeatureData
+
+class JobGuideCount(PerJobFeature):
+
+    def __init__(self, params:GeneratorParameters, job_map:dict):
+        self._job_map = job_map
+        super().__init__(params=params, job_map=job_map)
+        self._count = 0
 
     # *** IMPLEMENT ABSTRACT FUNCTIONS ***
     @classmethod
     def _eventFilter(cls, mode:ExtractionMode) -> List[str]:
-        return ["CUSTOM.6"]
-        # "events": ["SKIP_BUTTON"],
+        return ["guide_triggered"]
 
     @classmethod
     def _featureFilter(cls, mode:ExtractionMode) -> List[str]:
         return []
 
     def _updateFromEvent(self, event:Event) -> None:
-        self._skip_count += 1
+        self._count += 1
 
     def _updateFromFeatureData(self, feature:FeatureData):
         return
 
     def _getFeatureValues(self) -> List[Any]:
-        return [self._skip_count]
+        return [self._count]
 
     # *** Optionally override public functions. ***
+    @staticmethod
+    def MinVersion() -> Optional[str]:
+        return "1"
```

### Comparing `opengamedata_core-0.0.5/src/ogd/games/WAVES/features/TotalSliderMoves.py` & `opengamedata_core-0.0.6/src/ogd/games/PENGUINS/features/BuiltWrongNestCount.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,35 +1,41 @@
 # import libraries
-from ogd.core.schemas import Event
-from typing import Any, List, Optional
+import logging
+import re
+from typing import Any, Dict, List, Optional
 # import locals
-from ogd.core.generators.extractors.PerLevelFeature import PerLevelFeature
+from ogd.core.utils.Logger import Logger
 from ogd.core.generators.Generator import GeneratorParameters
-from ogd.core.schemas.Event import Event
-from ogd.core.schemas.ExtractionMode import ExtractionMode
-from ogd.core.schemas.FeatureData import FeatureData
+from ogd.core.models.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
+from ogd.core.models.FeatureData import FeatureData
+from ogd.core.generators.extractors.SessionFeature import SessionFeature
+
+
+class BuiltWrongNestCount(SessionFeature):
 
-class TotalSliderMoves(PerLevelFeature):
     def __init__(self, params:GeneratorParameters):
-        PerLevelFeature.__init__(self, params=params)
-        self._slider_move_count : int = 0
+        super().__init__(params=params)
+        self._current_count : int = 0
 
     # *** IMPLEMENT ABSTRACT FUNCTIONS ***
     @classmethod
     def _eventFilter(cls, mode:ExtractionMode) -> List[str]:
-        return ["CUSTOM.1"]
-        # return ["SLIDER_MOVE_RELEASE"]
+        return ["peck_nest"]
 
     @classmethod
     def _featureFilter(cls, mode:ExtractionMode) -> List[str]:
         return []
 
     def _updateFromEvent(self, event:Event) -> None:
-            self._slider_move_count += 1
+        # if has_rock does not exit it will return false as well
+        
+        # TODO : account for newer versions having peck_nest co-occurring with place_rock when building correct nest
+        if event.game_state.get("has_rock", False):
+            # if (event.log_version) < 11 and (event.game_state.get("has_rock", False)):
+            self._current_count += 1
 
     def _updateFromFeatureData(self, feature:FeatureData):
         return
 
     def _getFeatureValues(self) -> List[Any]:
-        return [self._slider_move_count]
-
-    # *** Optionally override public functions. ***
+        return [self._current_count]
```

### Comparing `opengamedata_core-0.0.5/src/ogd/games/WAVES/features/WavelengthGoodMoveCount.py` & `opengamedata_core-0.0.6/src/ogd/games/WAVES/features/PercentOffsetGoodMoves.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,44 +1,46 @@
 # import libraries
-from ogd.core.schemas import Event
-import typing
+from ogd.core.models import Event
 from typing import Any, List, Optional
 # import locals
+from ogd.core.generators.extractors.Feature import Feature
 from ogd.core.generators.extractors.PerLevelFeature import PerLevelFeature
 from ogd.core.generators.Generator import GeneratorParameters
-from ogd.core.schemas.Event import Event
-from ogd.core.schemas.ExtractionMode import ExtractionMode
-from ogd.core.schemas.FeatureData import FeatureData
+from ogd.core.models.Event import Event
+from ogd.core.models.enums.ExtractionMode import ExtractionMode
+from ogd.core.models.FeatureData import FeatureData
 
-class WavelengthGoodMoveCount(PerLevelFeature):
+class PercentOffsetGoodMoves(PerLevelFeature):
     def __init__(self, params:GeneratorParameters):
-        PerLevelFeature.__init__(self, params=params)
-        self._count = 0
+        Feature.__init__(self, params=params)
+        self._offset_count = 0
+        self._good_count = 0
 
     # *** IMPLEMENT ABSTRACT FUNCTIONS ***
     @classmethod
     def _eventFilter(cls, mode:ExtractionMode) -> List[str]:
         return ["CUSTOM.1", "CUSTOM.2"]
         # return ["SLIDER_MOVE_RELEASE", "ARROW_MOVE_RELEASE"]
 
     @classmethod
     def _featureFilter(cls, mode:ExtractionMode) -> List[str]:
         return []
 
     def _updateFromEvent(self, event:Event) -> None:
-        if event.EventData['slider'].upper() == 'WAVELENGTH':
+        if event.EventData['slider'].upper() == 'OFFSET':
+            self._offset_count += 1
             if event.EventName == "CUSTOM.1":
                 if event.EventData['end_closeness'] > event.EventData['begin_closeness']:
-                    self._count += 1
+                    self._good_count += 1
             elif event.EventName == "CUSTOM.2":
                 start_dist = event.EventData['correct_val'] - event.EventData['begin_val']
                 end_dist = event.EventData['correct_val'] - event.EventData['end_val']
                 if abs(end_dist) < abs(start_dist):
-                    self._count += 1
+                    self._good_count += 1
 
     def _updateFromFeatureData(self, feature:FeatureData):
         return
 
     def _getFeatureValues(self) -> List[Any]:
-        return [self._count]
+        return [self._good_count / self._offset_count if self._offset_count != 0 else None]
 
     # *** Optionally override public functions. ***
```

### Comparing `opengamedata_core-0.0.5/src/ogd/games/WAVES/features/__init__.py` & `opengamedata_core-0.0.6/src/ogd/games/WAVES/features/__init__.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.5/src/ogd/games/WAVES/schemas/WAVES.json.template` & `opengamedata_core-0.0.6/src/ogd/games/WAVES/schemas/WAVES.json.template`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.5/src/ogd/games/WEATHER_STATION/schemas/WEATHER_STATION.json.template` & `opengamedata_core-0.0.6/src/ogd/games/WEATHER_STATION/schemas/WEATHER_STATION.json.template`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.5/src/opengamedata_core.egg-info/PKG-INFO` & `opengamedata_core-0.0.6/src/opengamedata_core.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opengamedata-core
-Version: 0.0.5
+Version: 0.0.6
 Summary: A package for retrieving and processing event-based video game data. Additional authors: Nick Spevacek, Renee Li, John McCloskey, Zach Studdiford, Glenn Palmer, Haishuo Chen, Daus, Ameya Kshirsagar, Yunqing Xiao, Erik Harpstead, Manuel Jesus Gomez Moratilla
 Author-email: Luke Swanson <superscription58@gmail.com>, David Gagnon <djgagnon@wisc.edu>
 Project-URL: Homepage, https://github.com/opengamedata/opengamedata-core
 Project-URL: Bug Tracker, https://github.com/opengamedata/opengamedata-core/issues
 Project-URL: Documentation, https://opengamedata-doc.readthedocs.io/en/latest/index.html
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `opengamedata_core-0.0.5/src/opengamedata_core.egg-info/SOURCES.txt` & `opengamedata_core-0.0.6/src/opengamedata_core.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -2,18 +2,15 @@
 README.md
 pyproject.toml
 src/ogd/__init__.py
 src/ogd/core/__init__.py
 src/ogd/core/exec/Commands.py
 src/ogd/core/exec/Generators.py
 src/ogd/core/exec/Parsers.py
-src/ogd/core/games/AQUALAB/features/AppVersions.py
 src/ogd/core/games/AQUALAB/features/PlayLocations.py
-src/ogd/core/games/JOURNALISM/features/FailureAttributes.py
-src/ogd/core/games/JOURNALISM/features/FinalAttributes.py
 src/ogd/core/generators/Generator.py
 src/ogd/core/generators/GeneratorLoader.py
 src/ogd/core/generators/__init__.py
 src/ogd/core/generators/detectors/Detector.py
 src/ogd/core/generators/detectors/DetectorEvent.py
 src/ogd/core/generators/detectors/__init__.py
 src/ogd/core/generators/extractors/Extractor.py
@@ -43,43 +40,47 @@
 src/ogd/core/interfaces/outerfaces/DebugOuterface.py
 src/ogd/core/interfaces/outerfaces/DictionaryOuterface.py
 src/ogd/core/interfaces/outerfaces/TSVOuterface.py
 src/ogd/core/managers/EventManager.py
 src/ogd/core/managers/ExportManager.py
 src/ogd/core/managers/FeatureManager.py
 src/ogd/core/managers/__init__.py
+src/ogd/core/models/Event.py
+src/ogd/core/models/FeatureData.py
+src/ogd/core/models/__init__.py
+src/ogd/core/models/enums/ExportMode.py
+src/ogd/core/models/enums/ExtractionMode.py
+src/ogd/core/models/enums/IDMode.py
+src/ogd/core/models/enums/IterationMode.py
+src/ogd/core/models/enums/__init__.py
 src/ogd/core/processors/ClassroomDetector.py
 src/ogd/core/processors/DetectorProcessor.py
 src/ogd/core/processors/EventProcessor.py
 src/ogd/core/processors/ExtractorProcessor.py
 src/ogd/core/processors/GeneratorProcessor.py
 src/ogd/core/processors/PlayerProcessor.py
 src/ogd/core/processors/PopulationProcessor.py
 src/ogd/core/processors/Processor.py
 src/ogd/core/processors/SessionProcessor.py
 src/ogd/core/processors/__init__.py
 src/ogd/core/requests/Request.py
 src/ogd/core/requests/RequestResult.py
 src/ogd/core/requests/__init__.py
-src/ogd/core/schemas/Event.py
-src/ogd/core/schemas/ExportMode.py
-src/ogd/core/schemas/ExtractionMode.py
-src/ogd/core/schemas/FeatureData.py
-src/ogd/core/schemas/IDMode.py
-src/ogd/core/schemas/IterationMode.py
 src/ogd/core/schemas/Schema.py
 src/ogd/core/schemas/__init__.py
 src/ogd/core/schemas/configs/ConfigSchema.py
 src/ogd/core/schemas/configs/GameSourceSchema.py
 src/ogd/core/schemas/configs/IndexingSchema.py
 src/ogd/core/schemas/configs/LegacyConfigSchema.py
 src/ogd/core/schemas/configs/data_sources/BigQuerySourceSchema.py
 src/ogd/core/schemas/configs/data_sources/DataSourceSchema.py
 src/ogd/core/schemas/configs/data_sources/FileSourceSchema.py
 src/ogd/core/schemas/configs/data_sources/MySQLSourceSchema.py
+src/ogd/core/schemas/datasets/DatasetSchema.py
+src/ogd/core/schemas/datasets/FileListSchema.py
 src/ogd/core/schemas/games/AggregateSchema.py
 src/ogd/core/schemas/games/DataElementSchema.py
 src/ogd/core/schemas/games/DetectorMapSchema.py
 src/ogd/core/schemas/games/DetectorSchema.py
 src/ogd/core/schemas/games/EventSchema.py
 src/ogd/core/schemas/games/ExtractorSchema.py
 src/ogd/core/schemas/games/FeatureMapSchema.py
@@ -209,15 +210,17 @@
 src/ogd/games/ICECUBE/features/__init__.py
 src/ogd/games/ICECUBE/schemas/ICECUBE.json.template
 src/ogd/games/JOURNALISM/JournalismLoader.py
 src/ogd/games/JOURNALISM/features/AttributeView.py
 src/ogd/games/JOURNALISM/features/ChoiceClickCount.py
 src/ogd/games/JOURNALISM/features/ContinuesOnFail.py
 src/ogd/games/JOURNALISM/features/EditorNoteOpen.py
+src/ogd/games/JOURNALISM/features/FailureAttributes.py
 src/ogd/games/JOURNALISM/features/FailureCount.py
+src/ogd/games/JOURNALISM/features/FinalAttributes.py
 src/ogd/games/JOURNALISM/features/GameComplete.py
 src/ogd/games/JOURNALISM/features/LevelCompleteCount.py
 src/ogd/games/JOURNALISM/features/LevelCompleted.py
 src/ogd/games/JOURNALISM/features/LevelTime.py
 src/ogd/games/JOURNALISM/features/MaxedPlayerAttribute.py
 src/ogd/games/JOURNALISM/features/MeanSnippetTime.py
 src/ogd/games/JOURNALISM/features/PlayTime.py
@@ -323,38 +326,47 @@
 src/ogd/games/PENGUINS/PenguinsLoader.py
 src/ogd/games/PENGUINS/__init__.py
 src/ogd/games/PENGUINS/detectors/RegionEnter.py
 src/ogd/games/PENGUINS/detectors/RegionExit.py
 src/ogd/games/PENGUINS/detectors/__init__.py
 src/ogd/games/PENGUINS/features/ActivityCompleted.py
 src/ogd/games/PENGUINS/features/ActivityDuration.py
+src/ogd/games/PENGUINS/features/BuiltNestCount.py
+src/ogd/games/PENGUINS/features/BuiltWrongNestCount.py
 src/ogd/games/PENGUINS/features/EatFishCount.py
 src/ogd/games/PENGUINS/features/EggLostCount.py
 src/ogd/games/PENGUINS/features/EggRecoverTime.py
 src/ogd/games/PENGUINS/features/GazeCount.py
 src/ogd/games/PENGUINS/features/GazeDuration.py
+src/ogd/games/PENGUINS/features/LogVersion.py
 src/ogd/games/PENGUINS/features/MirrorWaddleDuration.py
-src/ogd/games/PENGUINS/features/PerRegionFeature.py
-src/ogd/games/PENGUINS/features/PickupRockCount.py
+src/ogd/games/PENGUINS/features/PenguinInteractCount.py
 src/ogd/games/PENGUINS/features/PlayerInactiveAvgDuration.py
-src/ogd/games/PENGUINS/features/PlayerWaddleCount.py
 src/ogd/games/PENGUINS/features/RegionDuration.py
 src/ogd/games/PENGUINS/features/RegionEnterCount.py
 src/ogd/games/PENGUINS/features/RegionsEncountered.py
 src/ogd/games/PENGUINS/features/RingChimesCount.py
+src/ogd/games/PENGUINS/features/RockBashCount.py
+src/ogd/games/PENGUINS/features/RockMultiplePickupCount.py
+src/ogd/games/PENGUINS/features/RockPickupCount.py
 src/ogd/games/PENGUINS/features/SessionDuration.py
+src/ogd/games/PENGUINS/features/SkuaBashCount.py
+src/ogd/games/PENGUINS/features/SkuaPeckCount.py
 src/ogd/games/PENGUINS/features/SnowBallDuration.py
+src/ogd/games/PENGUINS/features/WaddleCount.py
 src/ogd/games/PENGUINS/features/WaddlePerRegion.py
 src/ogd/games/PENGUINS/features/__init__.py
+src/ogd/games/PENGUINS/features/bases/PerRegionFeature.py
 src/ogd/games/PENGUINS/schemas/PENGUINS.json.template
 src/ogd/games/SHADOWSPECT/ShadowspectLoader.py
 src/ogd/games/SHADOWSPECT/features/FunnelByUser.py
 src/ogd/games/SHADOWSPECT/features/LevelsOfDifficulty.py
 src/ogd/games/SHADOWSPECT/features/MoveShapeCount.py
 src/ogd/games/SHADOWSPECT/features/SequenceBetweenPuzzles.py
+src/ogd/games/SHADOWSPECT/features/SequenceWithinPuzzles.py
 src/ogd/games/SHADOWSPECT/features/SessionID.py
 src/ogd/games/SHADOWSPECT/features/__init__.py
 src/ogd/games/SHADOWSPECT/schemas/SHADOWSPECT.json.template
 src/ogd/games/SHIPWRECKS/ShipwrecksLoader.py
 src/ogd/games/SHIPWRECKS/features/ActiveJobs.py
 src/ogd/games/SHIPWRECKS/features/EventList.py
 src/ogd/games/SHIPWRECKS/features/EvidenceBoardCompleteCount.py
```

### Comparing `opengamedata_core-0.0.5/tests/test_lakeland_models.py` & `opengamedata_core-0.0.6/tests/test_lakeland_models.py`

 * *Files identical despite different names*

