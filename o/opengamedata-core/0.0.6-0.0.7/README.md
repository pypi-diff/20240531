# Comparing `tmp/opengamedata_core-0.0.6.tar.gz` & `tmp/opengamedata_core-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opengamedata_core-0.0.6.tar", last modified: Thu May 30 18:05:05 2024, max compression
+gzip compressed data, was "opengamedata_core-0.0.7.tar", last modified: Thu May 30 22:40:41 2024, max compression
```

## Comparing `opengamedata_core-0.0.6.tar` & `opengamedata_core-0.0.7.tar`

### file list

```diff
@@ -1,560 +1,560 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:05:05.067022 opengamedata_core-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4796 2024-05-30 18:05:05.067022 opengamedata_core-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3900 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 18:05:05.067022 opengamedata_core-0.0.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:05:04.983023 opengamedata_core-0.0.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:05:04.983023 opengamedata_core-0.0.6/src/ogd/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:05:04.983023 opengamedata_core-0.0.6/src/ogd/core/
--rw-r--r--   0 runner    (1001) docker     (127)      265 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:05:04.983023 opengamedata_core-0.0.6/src/ogd/core/exec/
--rw-r--r--   0 runner    (1001) docker     (127)     9579 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/core/exec/Commands.py
--rw-r--r--   0 runner    (1001) docker     (127)     3903 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/core/exec/Generators.py
--rw-r--r--   0 runner    (1001) docker     (127)     4858 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/core/exec/Parsers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:05:04.971023 opengamedata_core-0.0.6/src/ogd/core/games/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:05:04.971023 opengamedata_core-0.0.6/src/ogd/core/games/AQUALAB/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:05:04.983023 opengamedata_core-0.0.6/src/ogd/core/games/AQUALAB/features/
--rw-r--r--   0 runner    (1001) docker     (127)     4259 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/core/games/AQUALAB/features/PlayLocations.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:05:04.987023 opengamedata_core-0.0.6/src/ogd/core/generators/
--rw-r--r--   0 runner    (1001) docker     (127)     7945 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/core/generators/Generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     5140 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/core/generators/GeneratorLoader.py
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/core/generators/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:05:04.987023 opengamedata_core-0.0.6/src/ogd/core/generators/detectors/
--rw-r--r--   0 runner    (1001) docker     (127)     4355 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/core/generators/detectors/Detector.py
--rw-r--r--   0 runner    (1001) docker     (127)     2299 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/core/generators/detectors/DetectorEvent.py
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/core/generators/detectors/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:05:04.987023 opengamedata_core-0.0.6/src/ogd/core/generators/extractors/
--rw-r--r--   0 runner    (1001) docker     (127)     6502 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/core/generators/extractors/Extractor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/core/generators/extractors/Feature.py
--rw-r--r--   0 runner    (1001) docker     (127)     1584 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/core/generators/extractors/PerCountFeature.py
--rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/core/generators/extractors/PerLevelFeature.py
--rw-r--r--   0 runner    (1001) docker     (127)      804 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/core/generators/extractors/SessionFeature.py
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/core/generators/extractors/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:05:04.987023 opengamedata_core-0.0.6/src/ogd/core/generators/legacy/
--rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/core/generators/legacy/LegacyDetector.py
--rw-r--r--   0 runner    (1001) docker     (127)    14636 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/core/generators/legacy/LegacyFeature.py
--rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/core/generators/legacy/LegacyLoader.py
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/core/generators/legacy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:05:04.987023 opengamedata_core-0.0.6/src/ogd/core/generators/registries/
--rw-r--r--   0 runner    (1001) docker     (127)     8372 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/core/generators/registries/DetectorRegistry.py
--rw-r--r--   0 runner    (1001) docker     (127)    13807 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/core/generators/registries/ExtractorRegistry.py
--rw-r--r--   0 runner    (1001) docker     (127)     5284 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/core/generators/registries/GeneratorRegistry.py
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/core/generators/registries/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:05:04.991023 opengamedata_core-0.0.6/src/ogd/core/interfaces/
--rw-r--r--   0 runner    (1001) docker     (127)    10837 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/core/interfaces/BQFirebaseInterface.py
--rw-r--r--   0 runner    (1001) docker     (127)     9704 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/core/interfaces/BigQueryCodingInterface.py
--rw-r--r--   0 runner    (1001) docker     (127)    11862 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/core/interfaces/BigQueryInterface.py
--rw-r--r--   0 runner    (1001) docker     (127)     4908 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/core/interfaces/CSVInterface.py
--rw-r--r--   0 runner    (1001) docker     (127)     3524 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/core/interfaces/CodingInterface.py
--rw-r--r--   0 runner    (1001) docker     (127)     5436 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/core/interfaces/DataInterface.py
--rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/core/interfaces/Interface.py
--rw-r--r--   0 runner    (1001) docker     (127)    23923 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/core/interfaces/MySQLInterface.py
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/core/interfaces/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:05:04.991023 opengamedata_core-0.0.6/src/ogd/core/interfaces/outerfaces/
--rw-r--r--   0 runner    (1001) docker     (127)     5834 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/core/interfaces/outerfaces/DataOuterface.py
--rw-r--r--   0 runner    (1001) docker     (127)     4200 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/core/interfaces/outerfaces/DebugOuterface.py
--rw-r--r--   0 runner    (1001) docker     (127)     4907 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/core/interfaces/outerfaces/DictionaryOuterface.py
--rw-r--r--   0 runner    (1001) docker     (127)    33767 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/core/interfaces/outerfaces/TSVOuterface.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:05:04.991023 opengamedata_core-0.0.6/src/ogd/core/managers/
--rw-r--r--   0 runner    (1001) docker     (127)     3512 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/core/managers/EventManager.py
--rw-r--r--   0 runner    (1001) docker     (127)    19016 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/core/managers/ExportManager.py
--rw-r--r--   0 runner    (1001) docker     (127)    12107 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/core/managers/FeatureManager.py
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/core/managers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:05:04.991023 opengamedata_core-0.0.6/src/ogd/core/models/
--rw-r--r--   0 runner    (1001) docker     (127)    14401 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/core/models/Event.py
--rw-r--r--   0 runner    (1001) docker     (127)     1431 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/core/models/FeatureData.py
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/core/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:05:04.995023 opengamedata_core-0.0.6/src/ogd/core/models/enums/
--rw-r--r--   0 runner    (1001) docker     (127)      213 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/core/models/enums/ExportMode.py
--rw-r--r--   0 runner    (1001) docker     (127)      364 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/core/models/enums/ExtractionMode.py
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/core/models/enums/IDMode.py
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/core/models/enums/IterationMode.py
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/core/models/enums/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:05:04.995023 opengamedata_core-0.0.6/src/ogd/core/processors/
--rw-r--r--   0 runner    (1001) docker     (127)     6040 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/core/processors/ClassroomDetector.py
--rw-r--r--   0 runner    (1001) docker     (127)     2242 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/core/processors/DetectorProcessor.py
--rw-r--r--   0 runner    (1001) docker     (127)      963 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/core/processors/EventProcessor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1658 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/core/processors/ExtractorProcessor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2637 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/core/processors/GeneratorProcessor.py
--rw-r--r--   0 runner    (1001) docker     (127)     4610 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/core/processors/PlayerProcessor.py
--rw-r--r--   0 runner    (1001) docker     (127)     4218 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/core/processors/PopulationProcessor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1876 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/core/processors/Processor.py
--rw-r--r--   0 runner    (1001) docker     (127)     4275 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/core/processors/SessionProcessor.py
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/core/processors/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:05:04.995023 opengamedata_core-0.0.6/src/ogd/core/requests/
--rw-r--r--   0 runner    (1001) docker     (127)     5311 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/core/requests/Request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2062 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/core/requests/RequestResult.py
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/core/requests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:05:04.995023 opengamedata_core-0.0.6/src/ogd/core/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)     1427 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/core/schemas/Schema.py
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/core/schemas/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:05:04.999023 opengamedata_core-0.0.6/src/ogd/core/schemas/configs/
--rw-r--r--   0 runner    (1001) docker     (127)    10898 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/core/schemas/configs/ConfigSchema.py
--rw-r--r--   0 runner    (1001) docker     (127)     5835 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/core/schemas/configs/GameSourceSchema.py
--rw-r--r--   0 runner    (1001) docker     (127)     3452 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/core/schemas/configs/IndexingSchema.py
--rw-r--r--   0 runner    (1001) docker     (127)     2593 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/core/schemas/configs/LegacyConfigSchema.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:05:04.999023 opengamedata_core-0.0.6/src/ogd/core/schemas/configs/data_sources/
--rw-r--r--   0 runner    (1001) docker     (127)     3048 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/core/schemas/configs/data_sources/BigQuerySourceSchema.py
--rw-r--r--   0 runner    (1001) docker     (127)     1806 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/core/schemas/configs/data_sources/DataSourceSchema.py
--rw-r--r--   0 runner    (1001) docker     (127)      577 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/core/schemas/configs/data_sources/FileSourceSchema.py
--rw-r--r--   0 runner    (1001) docker     (127)    10140 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/core/schemas/configs/data_sources/MySQLSourceSchema.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:05:04.999023 opengamedata_core-0.0.6/src/ogd/core/schemas/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)    20326 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/core/schemas/datasets/DatasetSchema.py
--rw-r--r--   0 runner    (1001) docker     (127)     6410 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/core/schemas/datasets/FileListSchema.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:05:05.003023 opengamedata_core-0.0.6/src/ogd/core/schemas/games/
--rw-r--r--   0 runner    (1001) docker     (127)      922 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/core/schemas/games/AggregateSchema.py
--rw-r--r--   0 runner    (1001) docker     (127)     5168 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/core/schemas/games/DataElementSchema.py
--rw-r--r--   0 runner    (1001) docker     (127)     5045 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/core/schemas/games/DetectorMapSchema.py
--rw-r--r--   0 runner    (1001) docker     (127)      806 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/core/schemas/games/DetectorSchema.py
--rw-r--r--   0 runner    (1001) docker     (127)     3996 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/core/schemas/games/EventSchema.py
--rw-r--r--   0 runner    (1001) docker     (127)     4011 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/core/schemas/games/ExtractorSchema.py
--rw-r--r--   0 runner    (1001) docker     (127)     5656 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/core/schemas/games/FeatureMapSchema.py
--rw-r--r--   0 runner    (1001) docker     (127)     4869 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/core/schemas/games/FeatureSchema.py
--rw-r--r--   0 runner    (1001) docker     (127)    26736 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/core/schemas/games/GameSchema.py
--rw-r--r--   0 runner    (1001) docker     (127)     2652 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/core/schemas/games/GameStateSchema.py
--rw-r--r--   0 runner    (1001) docker     (127)     2831 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/core/schemas/games/PerCountSchema.py
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/core/schemas/games/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:05:05.003023 opengamedata_core-0.0.6/src/ogd/core/schemas/table_schemas/
--rw-r--r--   0 runner    (1001) docker     (127)     3615 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/core/schemas/table_schemas/BIGQUERY.json
--rw-r--r--   0 runner    (1001) docker     (127)     4890 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/core/schemas/table_schemas/FIELDDAY_MYSQL.json
--rw-r--r--   0 runner    (1001) docker     (127)     2390 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/core/schemas/table_schemas/FIREBASE.json
--rw-r--r--   0 runner    (1001) docker     (127)     4430 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/core/schemas/table_schemas/MASHOPOLIS_MYSQL.json
--rw-r--r--   0 runner    (1001) docker     (127)     3685 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/core/schemas/table_schemas/OGD_EVENT_FILE.json
--rw-r--r--   0 runner    (1001) docker     (127)     4077 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/core/schemas/table_schemas/OPENGAMEDATA_BIGQUERY.json
--rw-r--r--   0 runner    (1001) docker     (127)     4477 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/core/schemas/table_schemas/OPENGAMEDATA_MYSQL.json
--rw-r--r--   0 runner    (1001) docker     (127)     1920 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/core/schemas/table_schemas/SHIPWRECKS.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:05:05.003023 opengamedata_core-0.0.6/src/ogd/core/schemas/tables/
--rw-r--r--   0 runner    (1001) docker     (127)     6782 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/core/schemas/tables/ColumnMapSchema.py
--rw-r--r--   0 runner    (1001) docker     (127)     4179 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/core/schemas/tables/ColumnSchema.py
--rw-r--r--   0 runner    (1001) docker     (127)    23083 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/core/schemas/tables/TableSchema.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:05:05.003023 opengamedata_core-0.0.6/src/ogd/core/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     4573 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/core/utils/Logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     4361 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/core/utils/Readme.py
--rw-r--r--   0 runner    (1001) docker     (127)    14950 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/core/utils/SemanticVersion.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/core/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/core/utils/typing.py
--rw-r--r--   0 runner    (1001) docker     (127)     2692 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/core/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:05:05.003023 opengamedata_core-0.0.6/src/ogd/games/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:05:04.975023 opengamedata_core-0.0.6/src/ogd/games/ALL_YOU_CAN_ET/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:05:05.007023 opengamedata_core-0.0.6/src/ogd/games/ALL_YOU_CAN_ET/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)    20816 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/games/ALL_YOU_CAN_ET/schemas/ALL_YOU_CAN_ET.json.template
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:05:05.007023 opengamedata_core-0.0.6/src/ogd/games/AQUALAB/
--rw-r--r--   0 runner    (1001) docker     (127)    13547 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/games/AQUALAB/AqualabLoader.py
--rw-r--r--   0 runner    (1001) docker     (127)   278275 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/games/AQUALAB/DBExport.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/games/AQUALAB/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:05:05.007023 opengamedata_core-0.0.6/src/ogd/games/AQUALAB/detectors/
--rw-r--r--   0 runner    (1001) docker     (127)     2324 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/games/AQUALAB/detectors/CollectFactNoJob.py
--rw-r--r--   0 runner    (1001) docker     (127)     3558 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/games/AQUALAB/detectors/DiveSiteNoEvidence.py
--rw-r--r--   0 runner    (1001) docker     (127)     1729 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/games/AQUALAB/detectors/EchoRoomChange.py
--rw-r--r--   0 runner    (1001) docker     (127)     4509 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/games/AQUALAB/detectors/HintAndLeave.py
--rw-r--r--   0 runner    (1001) docker     (127)     3470 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/games/AQUALAB/detectors/Idle.py
--rw-r--r--   0 runner    (1001) docker     (127)     3905 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/games/AQUALAB/detectors/SceneChangeFrequently.py
--rw-r--r--   0 runner    (1001) docker     (127)     3800 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/games/AQUALAB/detectors/TwoHints.py
--rw-r--r--   0 runner    (1001) docker     (127)      361 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/games/AQUALAB/detectors/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:05:05.019023 opengamedata_core-0.0.6/src/ogd/games/AQUALAB/features/
--rw-r--r--   0 runner    (1001) docker     (127)     2755 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/games/AQUALAB/features/ActiveJobs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2335 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/games/AQUALAB/features/ActiveTime.py
--rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/games/AQUALAB/features/AppVersions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1752 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/games/AQUALAB/features/AverageSessionTime.py
--rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/games/AQUALAB/features/EchoSessionID.py
--rw-r--r--   0 runner    (1001) docker     (127)     5321 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/games/AQUALAB/features/EventList.py
--rw-r--r--   0 runner    (1001) docker     (127)     9516 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/games/AQUALAB/features/JobActiveTime.py
--rw-r--r--   0 runner    (1001) docker     (127)     2463 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/games/AQUALAB/features/JobArgumentation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2711 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/games/AQUALAB/features/JobCompletionTime.py
--rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/games/AQUALAB/features/JobDiveSitesCount.py
--rw-r--r--   0 runner    (1001) docker     (127)     2141 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/games/AQUALAB/features/JobDiveTime.py
--rw-r--r--   0 runner    (1001) docker     (127)     2411 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/games/AQUALAB/features/JobExperimentation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1247 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/games/AQUALAB/features/JobGuideCount.py
--rw-r--r--   0 runner    (1001) docker     (127)     1761 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/games/AQUALAB/features/JobHelpCount.py
--rw-r--r--   0 runner    (1001) docker     (127)     3955 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/games/AQUALAB/features/JobLocationChanges.py
--rw-r--r--   0 runner    (1001) docker     (127)     2282 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/games/AQUALAB/features/JobModeling.py
--rw-r--r--   0 runner    (1001) docker     (127)     2347 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/games/AQUALAB/features/JobPlayTime.py
--rw-r--r--   0 runner    (1001) docker     (127)     2122 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/games/AQUALAB/features/JobPriorAttempt.py
--rw-r--r--   0 runner    (1001) docker     (127)     1946 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/games/AQUALAB/features/JobPriorComplete.py
--rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/games/AQUALAB/features/JobStartCount.py
--rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/games/AQUALAB/features/JobTasksCompleted.py
--rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/games/AQUALAB/features/JobTriesInArgument.py
--rw-r--r--   0 runner    (1001) docker     (127)     6200 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/games/AQUALAB/features/JobsAttempted.py
--rw-r--r--   0 runner    (1001) docker     (127)     1532 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/games/AQUALAB/features/JobsCompleted.py
--rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/games/AQUALAB/features/ModelExportCount.py
--rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/games/AQUALAB/features/ModelInterveneCount.py
--rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/games/AQUALAB/features/ModelPredictCount.py
--rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/games/AQUALAB/features/PerJobFeature.py
--rw-r--r--   0 runner    (1001) docker     (127)     3022 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/games/AQUALAB/features/PlayerSummary.py
--rw-r--r--   0 runner    (1001) docker     (127)     3354 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/games/AQUALAB/features/PopulationSummary.py
--rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/games/AQUALAB/features/RegionJobCount.py
--rw-r--r--   0 runner    (1001) docker     (127)     1292 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/games/AQUALAB/features/RegionName.py
--rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/games/AQUALAB/features/SessionDiveSitesCount.py
--rw-r--r--   0 runner    (1001) docker     (127)     3953 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/games/AQUALAB/features/SessionDuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/games/AQUALAB/features/SessionGuideCount.py
--rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/games/AQUALAB/features/SessionHelpCount.py
--rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/games/AQUALAB/features/SessionID.py
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/games/AQUALAB/features/SessionJobsCompleted.py
--rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/games/AQUALAB/features/SwitchJobsCount.py
--rw-r--r--   0 runner    (1001) docker     (127)     2524 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/games/AQUALAB/features/SyncCompletionTime.py
--rw-r--r--   0 runner    (1001) docker     (127)     1736 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/games/AQUALAB/features/TankRulesCount.py
--rw-r--r--   0 runner    (1001) docker     (127)     3461 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/games/AQUALAB/features/TopJobCompletionDestinations.py
--rw-r--r--   0 runner    (1001) docker     (127)     3447 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/games/AQUALAB/features/TopJobSwitchDestinations.py
--rw-r--r--   0 runner    (1001) docker     (127)     3342 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/games/AQUALAB/features/TotalArcticTime.py
--rw-r--r--   0 runner    (1001) docker     (127)     2196 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/games/AQUALAB/features/TotalArgumentationTime.py
--rw-r--r--   0 runner    (1001) docker     (127)     3335 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/games/AQUALAB/features/TotalBayouTime.py
--rw-r--r--   0 runner    (1001) docker     (127)     3335 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/games/AQUALAB/features/TotalCoralTime.py
--rw-r--r--   0 runner    (1001) docker     (127)     2797 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/games/AQUALAB/features/TotalDiveTime.py
--rw-r--r--   0 runner    (1001) docker     (127)     2139 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/games/AQUALAB/features/TotalExperimentationTime.py
--rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/games/AQUALAB/features/TotalGuideCount.py
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/games/AQUALAB/features/TotalHelpCount.py
--rw-r--r--   0 runner    (1001) docker     (127)     3328 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/games/AQUALAB/features/TotalKelpTime.py
--rw-r--r--   0 runner    (1001) docker     (127)     2124 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/games/AQUALAB/features/TotalModelingTime.py
--rw-r--r--   0 runner    (1001) docker     (127)     2496 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/games/AQUALAB/features/TotalPlayTime.py
--rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/games/AQUALAB/features/UserAvgActiveTime.py
--rw-r--r--   0 runner    (1001) docker     (127)     1415 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/games/AQUALAB/features/UserAvgSessionDuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1447 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/games/AQUALAB/features/UserTotalSessionDuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     3093 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/games/AQUALAB/features/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:05:05.019023 opengamedata_core-0.0.6/src/ogd/games/AQUALAB/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)    32117 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/games/AQUALAB/schemas/AQUALAB.json.template
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:05:04.975023 opengamedata_core-0.0.6/src/ogd/games/BACTERIA/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:05:05.019023 opengamedata_core-0.0.6/src/ogd/games/BACTERIA/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/games/BACTERIA/schemas/BACTERIA.json.template
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:05:04.975023 opengamedata_core-0.0.6/src/ogd/games/BALLOON/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:05:05.019023 opengamedata_core-0.0.6/src/ogd/games/BALLOON/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/games/BALLOON/schemas/BALLOON.json.template
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:05:04.975023 opengamedata_core-0.0.6/src/ogd/games/BLOOM/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:05:05.019023 opengamedata_core-0.0.6/src/ogd/games/BLOOM/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)    21554 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/games/BLOOM/schemas/BLOOM.json.template
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:05:04.975023 opengamedata_core-0.0.6/src/ogd/games/CENSIO_SLIDE/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:05:05.019023 opengamedata_core-0.0.6/src/ogd/games/CENSIO_SLIDE/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)    11446 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/games/CENSIO_SLIDE/schemas/CENSIO_SLIDE.json.template
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:05:04.975023 opengamedata_core-0.0.6/src/ogd/games/CENSIO_STACK/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:05:05.019023 opengamedata_core-0.0.6/src/ogd/games/CENSIO_STACK/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)    21742 2024-05-30 18:04:24.000000 opengamedata_core-0.0.6/src/ogd/games/CENSIO_STACK/schemas/CENSIO_STACK.json.template
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:05:04.975023 opengamedata_core-0.0.6/src/ogd/games/CRUSH_STATION/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:05:05.019023 opengamedata_core-0.0.6/src/ogd/games/CRUSH_STATION/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)    11756 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/CRUSH_STATION/schemas/CRUSH_STATION.json.template
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:05:05.019023 opengamedata_core-0.0.6/src/ogd/games/CRYSTAL/
--rw-r--r--   0 runner    (1001) docker     (127)     2384 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/CRYSTAL/CrystalLoader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:05:05.019023 opengamedata_core-0.0.6/src/ogd/games/CRYSTAL/features/
--rw-r--r--   0 runner    (1001) docker     (127)    14127 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/CRYSTAL/features/CrystalExtractor.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/CRYSTAL/features/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:05:05.019023 opengamedata_core-0.0.6/src/ogd/games/CRYSTAL/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)    14066 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/CRYSTAL/schemas/CRYSTAL.json.template
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:05:04.975023 opengamedata_core-0.0.6/src/ogd/games/CYCLE_CARBON/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:05:05.019023 opengamedata_core-0.0.6/src/ogd/games/CYCLE_CARBON/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/CYCLE_CARBON/schemas/CYCLE_CARBON.json.template
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:05:04.975023 opengamedata_core-0.0.6/src/ogd/games/CYCLE_NITROGEN/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:05:05.019023 opengamedata_core-0.0.6/src/ogd/games/CYCLE_NITROGEN/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/CYCLE_NITROGEN/schemas/CYCLE_NITROGEN.json.template
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:05:04.975023 opengamedata_core-0.0.6/src/ogd/games/CYCLE_WATER/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:05:05.023023 opengamedata_core-0.0.6/src/ogd/games/CYCLE_WATER/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/CYCLE_WATER/schemas/CYCLE_WATER.json.template
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:05:04.975023 opengamedata_core-0.0.6/src/ogd/games/EARTHQUAKE/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:05:05.023023 opengamedata_core-0.0.6/src/ogd/games/EARTHQUAKE/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/EARTHQUAKE/schemas/EARTHQUAKE.json.template
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:05:04.975023 opengamedata_core-0.0.6/src/ogd/games/GWAKKAMOLE/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:05:05.023023 opengamedata_core-0.0.6/src/ogd/games/GWAKKAMOLE/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)    12879 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/GWAKKAMOLE/schemas/GWAKKAMOLE.json.template
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:05:05.023023 opengamedata_core-0.0.6/src/ogd/games/ICECUBE/
--rw-r--r--   0 runner    (1001) docker     (127)     1883 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/ICECUBE/DBExport.json
--rw-r--r--   0 runner    (1001) docker     (127)      803 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/ICECUBE/DBExport.py
--rw-r--r--   0 runner    (1001) docker     (127)     4859 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/ICECUBE/IcecubeLoader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:05:05.023023 opengamedata_core-0.0.6/src/ogd/games/ICECUBE/features/
--rw-r--r--   0 runner    (1001) docker     (127)     1281 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/ICECUBE/features/HeadsetOnCount.py
--rw-r--r--   0 runner    (1001) docker     (127)     1894 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/ICECUBE/features/ObjectSelectionsDuringVoiceover.py
--rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/ICECUBE/features/PerSceneFeature.py
--rw-r--r--   0 runner    (1001) docker     (127)     2893 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/ICECUBE/features/SceneDuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1944 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/ICECUBE/features/SceneFailureCount.py
--rw-r--r--   0 runner    (1001) docker     (127)     2723 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/ICECUBE/features/SceneFailures.py
--rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/ICECUBE/features/ScenesEncountered.py
--rw-r--r--   0 runner    (1001) docker     (127)     3472 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/ICECUBE/features/SessionDuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/ICECUBE/features/Session_Language.py
--rw-r--r--   0 runner    (1001) docker     (127)     2392 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/ICECUBE/features/TaskTimeToComplete.py
--rw-r--r--   0 runner    (1001) docker     (127)     1783 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/ICECUBE/features/ViewportCountPerScene.py
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/ICECUBE/features/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:05:05.023023 opengamedata_core-0.0.6/src/ogd/games/ICECUBE/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)     7292 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/ICECUBE/schemas/ICECUBE.json.template
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:05:05.023023 opengamedata_core-0.0.6/src/ogd/games/JOURNALISM/
--rw-r--r--   0 runner    (1001) docker     (127)     7981 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/JOURNALISM/JournalismLoader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:05:05.031023 opengamedata_core-0.0.6/src/ogd/games/JOURNALISM/features/
--rw-r--r--   0 runner    (1001) docker     (127)     4549 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/JOURNALISM/features/AttributeView.py
--rw-r--r--   0 runner    (1001) docker     (127)     4976 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/JOURNALISM/features/ChoiceClickCount.py
--rw-r--r--   0 runner    (1001) docker     (127)     2236 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/JOURNALISM/features/ContinuesOnFail.py
--rw-r--r--   0 runner    (1001) docker     (127)     4552 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/JOURNALISM/features/EditorNoteOpen.py
--rw-r--r--   0 runner    (1001) docker     (127)     2971 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/JOURNALISM/features/FailureAttributes.py
--rw-r--r--   0 runner    (1001) docker     (127)     4997 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/JOURNALISM/features/FailureCount.py
--rw-r--r--   0 runner    (1001) docker     (127)     1942 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/JOURNALISM/features/FinalAttributes.py
--rw-r--r--   0 runner    (1001) docker     (127)     3971 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/JOURNALISM/features/GameComplete.py
--rw-r--r--   0 runner    (1001) docker     (127)     4862 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/JOURNALISM/features/LevelCompleteCount.py
--rw-r--r--   0 runner    (1001) docker     (127)     4869 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/JOURNALISM/features/LevelCompleted.py
--rw-r--r--   0 runner    (1001) docker     (127)     2826 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/JOURNALISM/features/LevelTime.py
--rw-r--r--   0 runner    (1001) docker     (127)     2342 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/JOURNALISM/features/MaxedPlayerAttribute.py
--rw-r--r--   0 runner    (1001) docker     (127)     5258 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/JOURNALISM/features/MeanSnippetTime.py
--rw-r--r--   0 runner    (1001) docker     (127)     4462 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/JOURNALISM/features/PlayTime.py
--rw-r--r--   0 runner    (1001) docker     (127)     4387 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/JOURNALISM/features/PlayerAttributes.py
--rw-r--r--   0 runner    (1001) docker     (127)     4471 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/JOURNALISM/features/QuitLevel.py
--rw-r--r--   0 runner    (1001) docker     (127)     4145 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/JOURNALISM/features/QuitNode.py
--rw-r--r--   0 runner    (1001) docker     (127)     7637 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/JOURNALISM/features/QuitType.py
--rw-r--r--   0 runner    (1001) docker     (127)     6948 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/JOURNALISM/features/QuitTypePerLevel.py
--rw-r--r--   0 runner    (1001) docker     (127)     5905 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/JOURNALISM/features/SessionPlayTime.py
--rw-r--r--   0 runner    (1001) docker     (127)     5066 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/JOURNALISM/features/SkillSequenceCount.py
--rw-r--r--   0 runner    (1001) docker     (127)     3748 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/JOURNALISM/features/SnippetReceivedCount.py
--rw-r--r--   0 runner    (1001) docker     (127)     5007 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/JOURNALISM/features/SnippetReplace.py
--rw-r--r--   0 runner    (1001) docker     (127)     2080 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/JOURNALISM/features/SnippetsCollected.py
--rw-r--r--   0 runner    (1001) docker     (127)     1780 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/JOURNALISM/features/SnippetsSubmitted.py
--rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/JOURNALISM/features/StoryAlignment.py
--rw-r--r--   0 runner    (1001) docker     (127)     2219 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/JOURNALISM/features/StoryAlignmentSequence.py
--rw-r--r--   0 runner    (1001) docker     (127)     5476 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/JOURNALISM/features/StoryCompleteTime.py
--rw-r--r--   0 runner    (1001) docker     (127)     6579 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/JOURNALISM/features/StoryEditorTime.py
--rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/JOURNALISM/features/StoryScore.py
--rw-r--r--   0 runner    (1001) docker     (127)     2192 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/JOURNALISM/features/StoryScoreSequence.py
--rw-r--r--   0 runner    (1001) docker     (127)     4776 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/JOURNALISM/features/TextClickCount.py
--rw-r--r--   0 runner    (1001) docker     (127)     4723 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/JOURNALISM/features/TopAttribute.py
--rw-r--r--   0 runner    (1001) docker     (127)     2230 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/JOURNALISM/features/TopPlayerAttribute.py
--rw-r--r--   0 runner    (1001) docker     (127)     2274 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/JOURNALISM/features/TopPlayerQuitType.py
--rw-r--r--   0 runner    (1001) docker     (127)     4478 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/JOURNALISM/features/TotalFails.py
--rw-r--r--   0 runner    (1001) docker     (127)     2088 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/JOURNALISM/features/TotalLevelTime.py
--rw-r--r--   0 runner    (1001) docker     (127)     3951 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/JOURNALISM/features/UserPlayTime.py
--rw-r--r--   0 runner    (1001) docker     (127)     4732 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/JOURNALISM/features/WorstAttribute.py
--rw-r--r--   0 runner    (1001) docker     (127)     2244 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/JOURNALISM/features/WorstPlayerAttribute.py
--rw-r--r--   0 runner    (1001) docker     (127)     2048 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/JOURNALISM/features/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:05:05.031023 opengamedata_core-0.0.6/src/ogd/games/JOURNALISM/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)    45415 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/JOURNALISM/schemas/JOURNALISM.json.template
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:05:05.031023 opengamedata_core-0.0.6/src/ogd/games/JOWILDER/
--rw-r--r--   0 runner    (1001) docker     (127)     5210 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/JOWILDER/JowilderLoader.py
--rw-r--r--   0 runner    (1001) docker     (127)    16451 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/JOWILDER/Jowilder_Enumerators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:05:05.035023 opengamedata_core-0.0.6/src/ogd/games/JOWILDER/features/
--rw-r--r--   0 runner    (1001) docker     (127)     3092 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/JOWILDER/features/ActiveStateTime.py
--rw-r--r--   0 runner    (1001) docker     (127)     1841 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/JOWILDER/features/Clicks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1441 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/JOWILDER/features/EventCount.py
--rw-r--r--   0 runner    (1001) docker     (127)     1739 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/JOWILDER/features/FirstInteraction.py
--rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/JOWILDER/features/GameScript.py
--rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/JOWILDER/features/GameVersion.py
--rw-r--r--   0 runner    (1001) docker     (127)     1362 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/JOWILDER/features/Hovers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2461 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/JOWILDER/features/IdleState.py
--rw-r--r--   0 runner    (1001) docker     (127)     7612 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/JOWILDER/features/Interaction.py
--rw-r--r--   0 runner    (1001) docker     (127)     2341 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/JOWILDER/features/InteractionName.py
--rw-r--r--   0 runner    (1001) docker     (127)     4595 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/JOWILDER/features/InteractionTextBoxesPerSecond.py
--rw-r--r--   0 runner    (1001) docker     (127)     4590 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/JOWILDER/features/InteractionWordsPerSecond.py
--rw-r--r--   0 runner    (1001) docker     (127)     1687 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/JOWILDER/features/LastInteraction.py
--rw-r--r--   0 runner    (1001) docker     (127)     1723 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/JOWILDER/features/MeaningfulActions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2003 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/JOWILDER/features/NotebookUses.py
--rw-r--r--   0 runner    (1001) docker     (127)     3214 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/JOWILDER/features/QuestionAnswers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1773 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/JOWILDER/features/SessionDuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1890 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/JOWILDER/features/SessionStart.py
--rw-r--r--   0 runner    (1001) docker     (127)     5107 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/JOWILDER/features/SurveyItem.py
--rw-r--r--   0 runner    (1001) docker     (127)     2794 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/JOWILDER/features/SurveyTime.py
--rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/JOWILDER/features/UsedContinue.py
--rw-r--r--   0 runner    (1001) docker     (127)     1327 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/JOWILDER/features/UsedSaveCode.py
--rw-r--r--   0 runner    (1001) docker     (127)     2154 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/JOWILDER/features/UserEnabled.py
--rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/JOWILDER/features/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1925 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/JOWILDER/get_jowilder_all_items.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:05:05.035023 opengamedata_core-0.0.6/src/ogd/games/JOWILDER/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)    35912 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/JOWILDER/schemas/JOWILDER.json.template
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:05:05.039023 opengamedata_core-0.0.6/src/ogd/games/LAKELAND/
--rw-r--r--   0 runner    (1001) docker     (127)     2361 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/LAKELAND/LakelandLoader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:05:05.043022 opengamedata_core-0.0.6/src/ogd/games/LAKELAND/features/
--rw-r--r--   0 runner    (1001) docker     (127)     2039 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/LAKELAND/features/ActionsLastXSecondsModel.py
--rw-r--r--   0 runner    (1001) docker     (127)      607 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/LAKELAND/features/DeathCountModel.py
--rw-r--r--   0 runner    (1001) docker     (127)    11750 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/LAKELAND/features/DeathPredModel.py
--rw-r--r--   0 runner    (1001) docker     (127)     8664 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/LAKELAND/features/DeathThresholdModel.py
--rw-r--r--   0 runner    (1001) docker     (127)     4916 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/LAKELAND/features/DiagonalFarmDetectorModel.py
--rw-r--r--   0 runner    (1001) docker     (127)     7995 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/LAKELAND/features/FeatSeqPercent.py
--rw-r--r--   0 runner    (1001) docker     (127)     2294 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/LAKELAND/features/FeatVelocity.py
--rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/LAKELAND/features/FeatureModel.py
--rw-r--r--   0 runner    (1001) docker     (127)     8478 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/LAKELAND/features/LAKELAND_models.json
--rw-r--r--   0 runner    (1001) docker     (127)     4415 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/LAKELAND/features/LakelandEnumerators.json
--rw-r--r--   0 runner    (1001) docker     (127)    69736 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/LAKELAND/features/LakelandExtractor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2639 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/LAKELAND/features/LinearModel.py
--rw-r--r--   0 runner    (1001) docker     (127)     2701 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/LAKELAND/features/LogisticModel.py
--rw-r--r--   0 runner    (1001) docker     (127)     3353 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/LAKELAND/features/MapSummaryModel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/LAKELAND/features/Model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2574 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/LAKELAND/features/MoneyAccumulationModel.py
--rw-r--r--   0 runner    (1001) docker     (127)      444 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/LAKELAND/features/NthEventModel.py
--rw-r--r--   0 runner    (1001) docker     (127)      496 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/LAKELAND/features/PlayingTimeModel.py
--rw-r--r--   0 runner    (1001) docker     (127)     3287 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/LAKELAND/features/PopulationModel.py
--rw-r--r--   0 runner    (1001) docker     (127)     4813 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/LAKELAND/features/RecentPurchasesModel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1264 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/LAKELAND/features/SequenceModel.py
--rw-r--r--   0 runner    (1001) docker     (127)     4909 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/LAKELAND/features/SimpleFarmAbandonmentModel.py
--rw-r--r--   0 runner    (1001) docker     (127)      850 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/LAKELAND/features/SingleFeatureModel.py
--rw-r--r--   0 runner    (1001) docker     (127)     6060 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/LAKELAND/features/TimeSinceEventTypes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/LAKELAND/features/TimeSinceLastSaleModel.py
--rw-r--r--   0 runner    (1001) docker     (127)      507 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/LAKELAND/features/TownCompositionFeatureModel.py
--rw-r--r--   0 runner    (1001) docker     (127)     2026 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/LAKELAND/features/TownCompositionModel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/LAKELAND/features/TutorialProgressionModel.py
--rw-r--r--   0 runner    (1001) docker     (127)    82382 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/LAKELAND/features/WAVES_models.json
--rw-r--r--   0 runner    (1001) docker     (127)    82382 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/LAKELAND/features/WAVES_models_L8_Q0_Q1.json
--rw-r--r--   0 runner    (1001) docker     (127)    49819 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/LAKELAND/features/WAVES_models_L8_and_Q0.json
--rw-r--r--   0 runner    (1001) docker     (127)    28429 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/LAKELAND/features/WAVES_models_L8_complete_and_current.json
--rw-r--r--   0 runner    (1001) docker     (127)    21021 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/LAKELAND/features/WAVES_models_L8_only_complete.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/LAKELAND/features/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2331 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/LAKELAND/produce_lakeland_enumerators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:05:05.043022 opengamedata_core-0.0.6/src/ogd/games/LAKELAND/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)   115553 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/LAKELAND/schemas/LAKELAND.json.template
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:05:05.043022 opengamedata_core-0.0.6/src/ogd/games/MAGNET/
--rw-r--r--   0 runner    (1001) docker     (127)     2350 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/MAGNET/MagnetLoader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:05:05.043022 opengamedata_core-0.0.6/src/ogd/games/MAGNET/features/
--rw-r--r--   0 runner    (1001) docker     (127)     8600 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/MAGNET/features/MagnetExtractor.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/MAGNET/features/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:05:05.043022 opengamedata_core-0.0.6/src/ogd/games/MAGNET/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)     7887 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/MAGNET/schemas/MAGNET.json.template
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:05:04.979023 opengamedata_core-0.0.6/src/ogd/games/MASHOPOLIS/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:05:05.043022 opengamedata_core-0.0.6/src/ogd/games/MASHOPOLIS/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)    10063 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/MASHOPOLIS/schemas/MASHOPOLIS.json.template
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:05:05.047022 opengamedata_core-0.0.6/src/ogd/games/PENGUINS/
--rw-r--r--   0 runner    (1001) docker     (127)     2970 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/PENGUINS/DBExport.json
--rw-r--r--   0 runner    (1001) docker     (127)     8007 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/PENGUINS/PenguinsLoader.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/PENGUINS/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:05:05.047022 opengamedata_core-0.0.6/src/ogd/games/PENGUINS/detectors/
--rw-r--r--   0 runner    (1001) docker     (127)     5164 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/PENGUINS/detectors/RegionEnter.py
--rw-r--r--   0 runner    (1001) docker     (127)     6271 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/PENGUINS/detectors/RegionExit.py
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/PENGUINS/detectors/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:05:05.051023 opengamedata_core-0.0.6/src/ogd/games/PENGUINS/features/
--rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/PENGUINS/features/ActivityCompleted.py
--rw-r--r--   0 runner    (1001) docker     (127)     2723 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/PENGUINS/features/ActivityDuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/PENGUINS/features/BuiltNestCount.py
--rw-r--r--   0 runner    (1001) docker     (127)     1445 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/PENGUINS/features/BuiltWrongNestCount.py
--rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/PENGUINS/features/EatFishCount.py
--rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/PENGUINS/features/EggLostCount.py
--rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/PENGUINS/features/EggRecoverTime.py
--rw-r--r--   0 runner    (1001) docker     (127)     1662 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/PENGUINS/features/GazeCount.py
--rw-r--r--   0 runner    (1001) docker     (127)     2666 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/PENGUINS/features/GazeDuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/PENGUINS/features/LogVersion.py
--rw-r--r--   0 runner    (1001) docker     (127)     4231 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/PENGUINS/features/MirrorWaddleDuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/PENGUINS/features/PenguinInteractCount.py
--rw-r--r--   0 runner    (1001) docker     (127)     2508 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/PENGUINS/features/PlayerInactiveAvgDuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     2299 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/PENGUINS/features/RegionDuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1797 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/PENGUINS/features/RegionEnterCount.py
--rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/PENGUINS/features/RegionsEncountered.py
--rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/PENGUINS/features/RingChimesCount.py
--rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/PENGUINS/features/RockBashCount.py
--rw-r--r--   0 runner    (1001) docker     (127)     1419 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/PENGUINS/features/RockMultiplePickupCount.py
--rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/PENGUINS/features/RockPickupCount.py
--rw-r--r--   0 runner    (1001) docker     (127)     3212 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/PENGUINS/features/SessionDuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/PENGUINS/features/SkuaBashCount.py
--rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/PENGUINS/features/SkuaPeckCount.py
--rw-r--r--   0 runner    (1001) docker     (127)     1971 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/PENGUINS/features/SnowBallDuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/PENGUINS/features/WaddleCount.py
--rw-r--r--   0 runner    (1001) docker     (127)     1698 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/PENGUINS/features/WaddlePerRegion.py
--rw-r--r--   0 runner    (1001) docker     (127)     1474 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/PENGUINS/features/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:05:05.051023 opengamedata_core-0.0.6/src/ogd/games/PENGUINS/features/bases/
--rw-r--r--   0 runner    (1001) docker     (127)     3507 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/PENGUINS/features/bases/PerRegionFeature.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:05:05.051023 opengamedata_core-0.0.6/src/ogd/games/PENGUINS/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)    30981 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/PENGUINS/schemas/PENGUINS.json.template
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:05:05.051023 opengamedata_core-0.0.6/src/ogd/games/SHADOWSPECT/
--rw-r--r--   0 runner    (1001) docker     (127)     3373 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/SHADOWSPECT/ShadowspectLoader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:05:05.051023 opengamedata_core-0.0.6/src/ogd/games/SHADOWSPECT/features/
--rw-r--r--   0 runner    (1001) docker     (127)     2951 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/SHADOWSPECT/features/FunnelByUser.py
--rw-r--r--   0 runner    (1001) docker     (127)     7674 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/SHADOWSPECT/features/LevelsOfDifficulty.py
--rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/SHADOWSPECT/features/MoveShapeCount.py
--rw-r--r--   0 runner    (1001) docker     (127)     3916 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/SHADOWSPECT/features/SequenceBetweenPuzzles.py
--rw-r--r--   0 runner    (1001) docker     (127)     8242 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/SHADOWSPECT/features/SequenceWithinPuzzles.py
--rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/SHADOWSPECT/features/SessionID.py
--rw-r--r--   0 runner    (1001) docker     (127)      344 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/SHADOWSPECT/features/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:05:05.051023 opengamedata_core-0.0.6/src/ogd/games/SHADOWSPECT/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)    29173 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/SHADOWSPECT/schemas/SHADOWSPECT.json.template
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:05:05.051023 opengamedata_core-0.0.6/src/ogd/games/SHIPWRECKS/
--rw-r--r--   0 runner    (1001) docker     (127)     4681 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/SHIPWRECKS/ShipwrecksLoader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:05:05.055023 opengamedata_core-0.0.6/src/ogd/games/SHIPWRECKS/features/
--rw-r--r--   0 runner    (1001) docker     (127)     2167 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/SHIPWRECKS/features/ActiveJobs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2336 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/SHIPWRECKS/features/EventList.py
--rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/SHIPWRECKS/features/EvidenceBoardCompleteCount.py
--rw-r--r--   0 runner    (1001) docker     (127)     3548 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/SHIPWRECKS/features/JobsAttempted.py
--rw-r--r--   0 runner    (1001) docker     (127)     1225 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/SHIPWRECKS/features/JobsCompleted.py
--rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/SHIPWRECKS/features/MissionDiveTime.py
--rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/SHIPWRECKS/features/MissionSonarTimeToComplete.py
--rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/SHIPWRECKS/features/PlayerSummary.py
--rw-r--r--   0 runner    (1001) docker     (127)     1948 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/SHIPWRECKS/features/PopulationSummary.py
--rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/SHIPWRECKS/features/SessionDuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/SHIPWRECKS/features/SessionID.py
--rw-r--r--   0 runner    (1001) docker     (127)     2995 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/SHIPWRECKS/features/TopJobCompletionDestinations.py
--rw-r--r--   0 runner    (1001) docker     (127)     2739 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/SHIPWRECKS/features/TopJobSwitchDestinations.py
--rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/SHIPWRECKS/features/TotalDiveTime.py
--rw-r--r--   0 runner    (1001) docker     (127)      798 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/SHIPWRECKS/features/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:05:05.055023 opengamedata_core-0.0.6/src/ogd/games/SHIPWRECKS/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)    10509 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/SHIPWRECKS/schemas/SHIPWRECKS.json.template
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:05:05.055023 opengamedata_core-0.0.6/src/ogd/games/THERMOVR/
--rw-r--r--   0 runner    (1001) docker     (127)        3 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/THERMOVR/DBExport.json
--rw-r--r--   0 runner    (1001) docker     (127)     5667 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/THERMOVR/ThermoVRLoader.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/THERMOVR/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:05:05.055023 opengamedata_core-0.0.6/src/ogd/games/THERMOVR/detectors/
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/THERMOVR/detectors/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:05:05.059023 opengamedata_core-0.0.6/src/ogd/games/THERMOVR/features/
--rw-r--r--   0 runner    (1001) docker     (127)      302 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/THERMOVR/features/LabCompleteCount.py
--rw-r--r--   0 runner    (1001) docker     (127)     1891 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/THERMOVR/features/LeftHandMoves.py
--rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/THERMOVR/features/PhasesReached.py
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/THERMOVR/features/PlayMode.py
--rw-r--r--   0 runner    (1001) docker     (127)     1896 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/THERMOVR/features/RightHandMoves.py
--rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/THERMOVR/features/TaskCompleteCount.py
--rw-r--r--   0 runner    (1001) docker     (127)     1760 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/THERMOVR/features/ToolNudgeCount.py
--rw-r--r--   0 runner    (1001) docker     (127)     1700 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/THERMOVR/features/ToolSliderTime.py
--rw-r--r--   0 runner    (1001) docker     (127)      503 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/THERMOVR/features/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:05:05.059023 opengamedata_core-0.0.6/src/ogd/games/THERMOVR/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)    51378 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/THERMOVR/schemas/THERMOVR.json.template
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:05:05.059023 opengamedata_core-0.0.6/src/ogd/games/TRANSFORMATION_QUEST/
--rw-r--r--   0 runner    (1001) docker     (127)      777 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/TRANSFORMATION_QUEST/DBExport.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:05:05.059023 opengamedata_core-0.0.6/src/ogd/games/TRANSFORMATION_QUEST/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)    25177 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/TRANSFORMATION_QUEST/schemas/TRANSFORMATION_QUEST.json.template
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:05:05.059023 opengamedata_core-0.0.6/src/ogd/games/WAVES/
--rw-r--r--   0 runner    (1001) docker     (127)    37336 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/WAVES/WaveLoader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:05:05.067022 opengamedata_core-0.0.6/src/ogd/games/WAVES/features/
--rw-r--r--   0 runner    (1001) docker     (127)     1710 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/WAVES/features/AmplitudeGoodMoveCount.py
--rw-r--r--   0 runner    (1001) docker     (127)     1425 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/WAVES/features/AverageFails.py
--rw-r--r--   0 runner    (1001) docker     (127)     3489 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/WAVES/features/AverageLevelTime.py
--rw-r--r--   0 runner    (1001) docker     (127)     1876 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/WAVES/features/AverageMoveTypeChanges.py
--rw-r--r--   0 runner    (1001) docker     (127)     1478 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/WAVES/features/AverageSliderMoves.py
--rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/WAVES/features/BeginCount.py
--rw-r--r--   0 runner    (1001) docker     (127)     2014 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/WAVES/features/ClosenessIntercept.py
--rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/WAVES/features/ClosenessR2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/WAVES/features/ClosenessSlope.py
--rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/WAVES/features/Completed.py
--rw-r--r--   0 runner    (1001) docker     (127)     1194 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/WAVES/features/FirstMoveType.py
--rw-r--r--   0 runner    (1001) docker     (127)     1168 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/WAVES/features/MenuButtonCount.py
--rw-r--r--   0 runner    (1001) docker     (127)     1704 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/WAVES/features/OffsetGoodMoveCount.py
--rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/WAVES/features/OverallPercentAmplitudeMoves.py
--rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/WAVES/features/OverallPercentOffsetMoves.py
--rw-r--r--   0 runner    (1001) docker     (127)     1451 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/WAVES/features/OverallPercentWavelengthMoves.py
--rw-r--r--   0 runner    (1001) docker     (127)     1319 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/WAVES/features/OverallSliderAverageRange.py
--rw-r--r--   0 runner    (1001) docker     (127)     1315 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/WAVES/features/OverallSliderAverageStandardDeviations.py
--rw-r--r--   0 runner    (1001) docker     (127)     1921 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/WAVES/features/PercentAmplitudeGoodMoves.py
--rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/WAVES/features/PercentAmplitudeMoves.py
--rw-r--r--   0 runner    (1001) docker     (127)     1903 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/WAVES/features/PercentOffsetGoodMoves.py
--rw-r--r--   0 runner    (1001) docker     (127)     1327 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/WAVES/features/PercentOffsetMoves.py
--rw-r--r--   0 runner    (1001) docker     (127)     1845 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/WAVES/features/PercentWavelengthGoodMoves.py
--rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/WAVES/features/PercentWavelengthMoves.py
--rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/WAVES/features/PersistentSessionID.py
--rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/WAVES/features/QuestionAnswered.py
--rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/WAVES/features/QuestionCorrect.py
--rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/WAVES/features/RangeIntercept.py
--rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/WAVES/features/RangeR2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/WAVES/features/RangeSlope.py
--rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/WAVES/features/SequenceLevel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/WAVES/features/SessionID.py
--rw-r--r--   0 runner    (1001) docker     (127)     1328 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/WAVES/features/SliderAverageRange.py
--rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/WAVES/features/SliderAverageStandardDeviations.py
--rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/WAVES/features/SucceedCount.py
--rw-r--r--   0 runner    (1001) docker     (127)     2597 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/WAVES/features/TimeToAnswerMS.py
--rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/WAVES/features/TotalArrowMoves.py
--rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/WAVES/features/TotalFails.py
--rw-r--r--   0 runner    (1001) docker     (127)     1986 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/WAVES/features/TotalLevelTime.py
--rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/WAVES/features/TotalMoveTypeChanges.py
--rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/WAVES/features/TotalResets.py
--rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/WAVES/features/TotalSkips.py
--rw-r--r--   0 runner    (1001) docker     (127)     1192 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/WAVES/features/TotalSliderMoves.py
--rw-r--r--   0 runner    (1001) docker     (127)     1726 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/WAVES/features/WavelengthGoodMoveCount.py
--rw-r--r--   0 runner    (1001) docker     (127)     2575 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/WAVES/features/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:05:05.067022 opengamedata_core-0.0.6/src/ogd/games/WAVES/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)    21383 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/WAVES/schemas/WAVES.json.template
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:05:04.983023 opengamedata_core-0.0.6/src/ogd/games/WEATHER_STATION/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:05:05.067022 opengamedata_core-0.0.6/src/ogd/games/WEATHER_STATION/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)    34344 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/WEATHER_STATION/schemas/WEATHER_STATION.json.template
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:05:04.983023 opengamedata_core-0.0.6/src/ogd/games/WIND/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:05:05.067022 opengamedata_core-0.0.6/src/ogd/games/WIND/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/WIND/schemas/WIND.json.template
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/src/ogd/games/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:05:05.067022 opengamedata_core-0.0.6/src/opengamedata_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4796 2024-05-30 18:05:04.000000 opengamedata_core-0.0.6/src/opengamedata_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    22284 2024-05-30 18:05:04.000000 opengamedata_core-0.0.6/src/opengamedata_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 18:05:04.000000 opengamedata_core-0.0.6/src/opengamedata_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-30 18:05:04.000000 opengamedata_core-0.0.6/src/opengamedata_core.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 18:05:05.067022 opengamedata_core-0.0.6/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3113 2024-05-30 18:04:25.000000 opengamedata_core-0.0.6/tests/test_lakeland_models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:40:41.280908 opengamedata_core-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4796 2024-05-30 22:40:41.280908 opengamedata_core-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3900 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 22:40:41.280908 opengamedata_core-0.0.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:40:41.204908 opengamedata_core-0.0.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:40:41.208908 opengamedata_core-0.0.7/src/ogd/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:40:41.208908 opengamedata_core-0.0.7/src/ogd/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:40:41.208908 opengamedata_core-0.0.7/src/ogd/core/exec/
+-rw-r--r--   0 runner    (1001) docker     (127)     9579 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/core/exec/Commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3903 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/core/exec/Generators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4858 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/core/exec/Parsers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:40:41.196909 opengamedata_core-0.0.7/src/ogd/core/games/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:40:41.196909 opengamedata_core-0.0.7/src/ogd/core/games/AQUALAB/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:40:41.208908 opengamedata_core-0.0.7/src/ogd/core/games/AQUALAB/features/
+-rw-r--r--   0 runner    (1001) docker     (127)     4259 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/core/games/AQUALAB/features/PlayLocations.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:40:41.208908 opengamedata_core-0.0.7/src/ogd/core/generators/
+-rw-r--r--   0 runner    (1001) docker     (127)     7945 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/core/generators/Generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5140 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/core/generators/GeneratorLoader.py
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/core/generators/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:40:41.208908 opengamedata_core-0.0.7/src/ogd/core/generators/detectors/
+-rw-r--r--   0 runner    (1001) docker     (127)     4355 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/core/generators/detectors/Detector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2299 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/core/generators/detectors/DetectorEvent.py
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/core/generators/detectors/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:40:41.208908 opengamedata_core-0.0.7/src/ogd/core/generators/extractors/
+-rw-r--r--   0 runner    (1001) docker     (127)     6502 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/core/generators/extractors/Extractor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/core/generators/extractors/Feature.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1584 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/core/generators/extractors/PerCountFeature.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/core/generators/extractors/PerLevelFeature.py
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/core/generators/extractors/SessionFeature.py
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/core/generators/extractors/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:40:41.208908 opengamedata_core-0.0.7/src/ogd/core/generators/legacy/
+-rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/core/generators/legacy/LegacyDetector.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14636 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/core/generators/legacy/LegacyFeature.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/core/generators/legacy/LegacyLoader.py
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/core/generators/legacy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:40:41.212909 opengamedata_core-0.0.7/src/ogd/core/generators/registries/
+-rw-r--r--   0 runner    (1001) docker     (127)     8372 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/core/generators/registries/DetectorRegistry.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13807 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/core/generators/registries/ExtractorRegistry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5284 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/core/generators/registries/GeneratorRegistry.py
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/core/generators/registries/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:40:41.212909 opengamedata_core-0.0.7/src/ogd/core/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (127)    10837 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/core/interfaces/BQFirebaseInterface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9704 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/core/interfaces/BigQueryCodingInterface.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11862 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/core/interfaces/BigQueryInterface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4908 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/core/interfaces/CSVInterface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3524 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/core/interfaces/CodingInterface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5436 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/core/interfaces/DataInterface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/core/interfaces/Interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23923 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/core/interfaces/MySQLInterface.py
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/core/interfaces/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:40:41.212909 opengamedata_core-0.0.7/src/ogd/core/interfaces/outerfaces/
+-rw-r--r--   0 runner    (1001) docker     (127)     5834 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/core/interfaces/outerfaces/DataOuterface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4200 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/core/interfaces/outerfaces/DebugOuterface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4907 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/core/interfaces/outerfaces/DictionaryOuterface.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33767 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/core/interfaces/outerfaces/TSVOuterface.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:40:41.212909 opengamedata_core-0.0.7/src/ogd/core/managers/
+-rw-r--r--   0 runner    (1001) docker     (127)     3512 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/core/managers/EventManager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19016 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/core/managers/ExportManager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12107 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/core/managers/FeatureManager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/core/managers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:40:41.212909 opengamedata_core-0.0.7/src/ogd/core/models/
+-rw-r--r--   0 runner    (1001) docker     (127)    14401 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/core/models/Event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1431 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/core/models/FeatureData.py
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/core/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:40:41.216909 opengamedata_core-0.0.7/src/ogd/core/models/enums/
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/core/models/enums/ExportMode.py
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/core/models/enums/ExtractionMode.py
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/core/models/enums/IDMode.py
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/core/models/enums/IterationMode.py
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/core/models/enums/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:40:41.216909 opengamedata_core-0.0.7/src/ogd/core/processors/
+-rw-r--r--   0 runner    (1001) docker     (127)     6040 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/core/processors/ClassroomDetector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2242 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/core/processors/DetectorProcessor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      963 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/core/processors/EventProcessor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1658 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/core/processors/ExtractorProcessor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2637 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/core/processors/GeneratorProcessor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4610 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/core/processors/PlayerProcessor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4218 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/core/processors/PopulationProcessor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1876 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/core/processors/Processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4275 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/core/processors/SessionProcessor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/core/processors/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:40:41.216909 opengamedata_core-0.0.7/src/ogd/core/requests/
+-rw-r--r--   0 runner    (1001) docker     (127)     5311 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/core/requests/Request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2062 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/core/requests/RequestResult.py
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/core/requests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:40:41.216909 opengamedata_core-0.0.7/src/ogd/core/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)     1427 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/core/schemas/Schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/core/schemas/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:40:41.216909 opengamedata_core-0.0.7/src/ogd/core/schemas/configs/
+-rw-r--r--   0 runner    (1001) docker     (127)    10898 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/core/schemas/configs/ConfigSchema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5835 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/core/schemas/configs/GameSourceSchema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3452 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/core/schemas/configs/IndexingSchema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2593 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/core/schemas/configs/LegacyConfigSchema.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:40:41.220908 opengamedata_core-0.0.7/src/ogd/core/schemas/configs/data_sources/
+-rw-r--r--   0 runner    (1001) docker     (127)     3048 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/core/schemas/configs/data_sources/BigQuerySourceSchema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1806 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/core/schemas/configs/data_sources/DataSourceSchema.py
+-rw-r--r--   0 runner    (1001) docker     (127)      577 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/core/schemas/configs/data_sources/FileSourceSchema.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10140 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/core/schemas/configs/data_sources/MySQLSourceSchema.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:40:41.220908 opengamedata_core-0.0.7/src/ogd/core/schemas/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)    20326 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/core/schemas/datasets/DatasetSchema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6410 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/core/schemas/datasets/FileListSchema.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:40:41.220908 opengamedata_core-0.0.7/src/ogd/core/schemas/games/
+-rw-r--r--   0 runner    (1001) docker     (127)      922 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/core/schemas/games/AggregateSchema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5168 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/core/schemas/games/DataElementSchema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5045 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/core/schemas/games/DetectorMapSchema.py
+-rw-r--r--   0 runner    (1001) docker     (127)      806 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/core/schemas/games/DetectorSchema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3996 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/core/schemas/games/EventSchema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4011 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/core/schemas/games/ExtractorSchema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5656 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/core/schemas/games/FeatureMapSchema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4869 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/core/schemas/games/FeatureSchema.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26736 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/core/schemas/games/GameSchema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2652 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/core/schemas/games/GameStateSchema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2831 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/core/schemas/games/PerCountSchema.py
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/core/schemas/games/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:40:41.220908 opengamedata_core-0.0.7/src/ogd/core/schemas/table_schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)     3615 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/core/schemas/table_schemas/BIGQUERY.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4890 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/core/schemas/table_schemas/FIELDDAY_MYSQL.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2390 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/core/schemas/table_schemas/FIREBASE.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4430 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/core/schemas/table_schemas/MASHOPOLIS_MYSQL.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3685 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/core/schemas/table_schemas/OGD_EVENT_FILE.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4077 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/core/schemas/table_schemas/OPENGAMEDATA_BIGQUERY.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4477 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/core/schemas/table_schemas/OPENGAMEDATA_MYSQL.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1920 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/core/schemas/table_schemas/SHIPWRECKS.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:40:41.224908 opengamedata_core-0.0.7/src/ogd/core/schemas/tables/
+-rw-r--r--   0 runner    (1001) docker     (127)     6782 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/core/schemas/tables/ColumnMapSchema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4179 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/core/schemas/tables/ColumnSchema.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23083 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/core/schemas/tables/TableSchema.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:40:41.224908 opengamedata_core-0.0.7/src/ogd/core/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     4573 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/core/utils/Logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4361 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/core/utils/Readme.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14950 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/core/utils/SemanticVersion.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/core/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/core/utils/typing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2692 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/core/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:40:41.224908 opengamedata_core-0.0.7/src/ogd/games/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:40:41.196909 opengamedata_core-0.0.7/src/ogd/games/ALL_YOU_CAN_ET/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:40:41.224908 opengamedata_core-0.0.7/src/ogd/games/ALL_YOU_CAN_ET/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)    20816 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/ALL_YOU_CAN_ET/schemas/ALL_YOU_CAN_ET.json.template
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:40:41.224908 opengamedata_core-0.0.7/src/ogd/games/AQUALAB/
+-rw-r--r--   0 runner    (1001) docker     (127)    13547 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/AQUALAB/AqualabLoader.py
+-rw-r--r--   0 runner    (1001) docker     (127)   278275 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/AQUALAB/DBExport.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/AQUALAB/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:40:41.224908 opengamedata_core-0.0.7/src/ogd/games/AQUALAB/detectors/
+-rw-r--r--   0 runner    (1001) docker     (127)     2324 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/AQUALAB/detectors/CollectFactNoJob.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3558 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/AQUALAB/detectors/DiveSiteNoEvidence.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1729 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/AQUALAB/detectors/EchoRoomChange.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4509 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/AQUALAB/detectors/HintAndLeave.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3470 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/AQUALAB/detectors/Idle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3905 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/AQUALAB/detectors/SceneChangeFrequently.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3800 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/AQUALAB/detectors/TwoHints.py
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/AQUALAB/detectors/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:40:41.236908 opengamedata_core-0.0.7/src/ogd/games/AQUALAB/features/
+-rw-r--r--   0 runner    (1001) docker     (127)     2755 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/AQUALAB/features/ActiveJobs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2335 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/AQUALAB/features/ActiveTime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/AQUALAB/features/AppVersions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1752 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/AQUALAB/features/AverageSessionTime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/AQUALAB/features/EchoSessionID.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5321 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/AQUALAB/features/EventList.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9516 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/AQUALAB/features/JobActiveTime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2463 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/AQUALAB/features/JobArgumentation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2711 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/AQUALAB/features/JobCompletionTime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/AQUALAB/features/JobDiveSitesCount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2141 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/AQUALAB/features/JobDiveTime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2411 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/AQUALAB/features/JobExperimentation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1247 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/AQUALAB/features/JobGuideCount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1761 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/AQUALAB/features/JobHelpCount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3955 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/AQUALAB/features/JobLocationChanges.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2282 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/AQUALAB/features/JobModeling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2347 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/AQUALAB/features/JobPlayTime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2122 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/AQUALAB/features/JobPriorAttempt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1946 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/AQUALAB/features/JobPriorComplete.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/AQUALAB/features/JobStartCount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/AQUALAB/features/JobTasksCompleted.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/AQUALAB/features/JobTriesInArgument.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6200 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/AQUALAB/features/JobsAttempted.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1532 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/AQUALAB/features/JobsCompleted.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/AQUALAB/features/ModelExportCount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/AQUALAB/features/ModelInterveneCount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/AQUALAB/features/ModelPredictCount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/AQUALAB/features/PerJobFeature.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3022 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/AQUALAB/features/PlayerSummary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3354 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/AQUALAB/features/PopulationSummary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/AQUALAB/features/RegionJobCount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1292 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/AQUALAB/features/RegionName.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/AQUALAB/features/SessionDiveSitesCount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3953 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/AQUALAB/features/SessionDuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/AQUALAB/features/SessionGuideCount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/AQUALAB/features/SessionHelpCount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/AQUALAB/features/SessionID.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/AQUALAB/features/SessionJobsCompleted.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/AQUALAB/features/SwitchJobsCount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2524 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/AQUALAB/features/SyncCompletionTime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1736 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/AQUALAB/features/TankRulesCount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3461 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/AQUALAB/features/TopJobCompletionDestinations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3447 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/AQUALAB/features/TopJobSwitchDestinations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3342 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/AQUALAB/features/TotalArcticTime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2196 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/AQUALAB/features/TotalArgumentationTime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3335 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/AQUALAB/features/TotalBayouTime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3335 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/AQUALAB/features/TotalCoralTime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2797 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/AQUALAB/features/TotalDiveTime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2139 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/AQUALAB/features/TotalExperimentationTime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/AQUALAB/features/TotalGuideCount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/AQUALAB/features/TotalHelpCount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3328 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/AQUALAB/features/TotalKelpTime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2124 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/AQUALAB/features/TotalModelingTime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2496 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/AQUALAB/features/TotalPlayTime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/AQUALAB/features/UserAvgActiveTime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1415 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/AQUALAB/features/UserAvgSessionDuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1447 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/AQUALAB/features/UserTotalSessionDuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3093 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/AQUALAB/features/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:40:41.236908 opengamedata_core-0.0.7/src/ogd/games/AQUALAB/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)    32117 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/AQUALAB/schemas/AQUALAB.json.template
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:40:41.200909 opengamedata_core-0.0.7/src/ogd/games/BACTERIA/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:40:41.236908 opengamedata_core-0.0.7/src/ogd/games/BACTERIA/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/BACTERIA/schemas/BACTERIA.json.template
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:40:41.200909 opengamedata_core-0.0.7/src/ogd/games/BALLOON/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:40:41.236908 opengamedata_core-0.0.7/src/ogd/games/BALLOON/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/BALLOON/schemas/BALLOON.json.template
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:40:41.200909 opengamedata_core-0.0.7/src/ogd/games/BLOOM/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:40:41.236908 opengamedata_core-0.0.7/src/ogd/games/BLOOM/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)    21554 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/BLOOM/schemas/BLOOM.json.template
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:40:41.200909 opengamedata_core-0.0.7/src/ogd/games/CENSIO_SLIDE/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:40:41.236908 opengamedata_core-0.0.7/src/ogd/games/CENSIO_SLIDE/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)    11446 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/CENSIO_SLIDE/schemas/CENSIO_SLIDE.json.template
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:40:41.200909 opengamedata_core-0.0.7/src/ogd/games/CENSIO_STACK/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:40:41.236908 opengamedata_core-0.0.7/src/ogd/games/CENSIO_STACK/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)    21742 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/CENSIO_STACK/schemas/CENSIO_STACK.json.template
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:40:41.200909 opengamedata_core-0.0.7/src/ogd/games/CRUSH_STATION/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:40:41.236908 opengamedata_core-0.0.7/src/ogd/games/CRUSH_STATION/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)    11756 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/CRUSH_STATION/schemas/CRUSH_STATION.json.template
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:40:41.236908 opengamedata_core-0.0.7/src/ogd/games/CRYSTAL/
+-rw-r--r--   0 runner    (1001) docker     (127)     2384 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/CRYSTAL/CrystalLoader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:40:41.236908 opengamedata_core-0.0.7/src/ogd/games/CRYSTAL/features/
+-rw-r--r--   0 runner    (1001) docker     (127)    14127 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/CRYSTAL/features/CrystalExtractor.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/CRYSTAL/features/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:40:41.236908 opengamedata_core-0.0.7/src/ogd/games/CRYSTAL/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)    14066 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/CRYSTAL/schemas/CRYSTAL.json.template
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:40:41.200909 opengamedata_core-0.0.7/src/ogd/games/CYCLE_CARBON/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:40:41.236908 opengamedata_core-0.0.7/src/ogd/games/CYCLE_CARBON/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/CYCLE_CARBON/schemas/CYCLE_CARBON.json.template
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:40:41.200909 opengamedata_core-0.0.7/src/ogd/games/CYCLE_NITROGEN/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:40:41.236908 opengamedata_core-0.0.7/src/ogd/games/CYCLE_NITROGEN/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/CYCLE_NITROGEN/schemas/CYCLE_NITROGEN.json.template
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:40:41.200909 opengamedata_core-0.0.7/src/ogd/games/CYCLE_WATER/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:40:41.236908 opengamedata_core-0.0.7/src/ogd/games/CYCLE_WATER/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/CYCLE_WATER/schemas/CYCLE_WATER.json.template
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:40:41.200909 opengamedata_core-0.0.7/src/ogd/games/EARTHQUAKE/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:40:41.236908 opengamedata_core-0.0.7/src/ogd/games/EARTHQUAKE/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/EARTHQUAKE/schemas/EARTHQUAKE.json.template
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:40:41.200909 opengamedata_core-0.0.7/src/ogd/games/GWAKKAMOLE/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:40:41.236908 opengamedata_core-0.0.7/src/ogd/games/GWAKKAMOLE/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)    12879 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/GWAKKAMOLE/schemas/GWAKKAMOLE.json.template
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:40:41.240908 opengamedata_core-0.0.7/src/ogd/games/ICECUBE/
+-rw-r--r--   0 runner    (1001) docker     (127)     1883 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/ICECUBE/DBExport.json
+-rw-r--r--   0 runner    (1001) docker     (127)      803 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/ICECUBE/DBExport.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4859 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/ICECUBE/IcecubeLoader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:40:41.240908 opengamedata_core-0.0.7/src/ogd/games/ICECUBE/features/
+-rw-r--r--   0 runner    (1001) docker     (127)     1281 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/ICECUBE/features/HeadsetOnCount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1894 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/ICECUBE/features/ObjectSelectionsDuringVoiceover.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/ICECUBE/features/PerSceneFeature.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2893 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/ICECUBE/features/SceneDuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1944 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/ICECUBE/features/SceneFailureCount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2723 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/ICECUBE/features/SceneFailures.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/ICECUBE/features/ScenesEncountered.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3472 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/ICECUBE/features/SessionDuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/ICECUBE/features/Session_Language.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2392 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/ICECUBE/features/TaskTimeToComplete.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1783 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/ICECUBE/features/ViewportCountPerScene.py
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/ICECUBE/features/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:40:41.240908 opengamedata_core-0.0.7/src/ogd/games/ICECUBE/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)     7292 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/ICECUBE/schemas/ICECUBE.json.template
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:40:41.240908 opengamedata_core-0.0.7/src/ogd/games/JOURNALISM/
+-rw-r--r--   0 runner    (1001) docker     (127)     7981 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/JOURNALISM/JournalismLoader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:40:41.248908 opengamedata_core-0.0.7/src/ogd/games/JOURNALISM/features/
+-rw-r--r--   0 runner    (1001) docker     (127)     4549 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/JOURNALISM/features/AttributeView.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4976 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/JOURNALISM/features/ChoiceClickCount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2236 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/JOURNALISM/features/ContinuesOnFail.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4552 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/JOURNALISM/features/EditorNoteOpen.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2971 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/JOURNALISM/features/FailureAttributes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4997 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/JOURNALISM/features/FailureCount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1942 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/JOURNALISM/features/FinalAttributes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3971 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/JOURNALISM/features/GameComplete.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4862 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/JOURNALISM/features/LevelCompleteCount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4869 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/JOURNALISM/features/LevelCompleted.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2826 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/JOURNALISM/features/LevelTime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2342 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/JOURNALISM/features/MaxedPlayerAttribute.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5258 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/JOURNALISM/features/MeanSnippetTime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4462 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/JOURNALISM/features/PlayTime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4387 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/JOURNALISM/features/PlayerAttributes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4471 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/JOURNALISM/features/QuitLevel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4145 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/JOURNALISM/features/QuitNode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7637 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/JOURNALISM/features/QuitType.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6948 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/JOURNALISM/features/QuitTypePerLevel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5905 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/JOURNALISM/features/SessionPlayTime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5066 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/JOURNALISM/features/SkillSequenceCount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3748 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/JOURNALISM/features/SnippetReceivedCount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5007 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/JOURNALISM/features/SnippetReplace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2080 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/JOURNALISM/features/SnippetsCollected.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1780 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/JOURNALISM/features/SnippetsSubmitted.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/JOURNALISM/features/StoryAlignment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2219 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/JOURNALISM/features/StoryAlignmentSequence.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5476 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/JOURNALISM/features/StoryCompleteTime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6579 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/JOURNALISM/features/StoryEditorTime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/JOURNALISM/features/StoryScore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2192 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/JOURNALISM/features/StoryScoreSequence.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4776 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/JOURNALISM/features/TextClickCount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4723 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/JOURNALISM/features/TopAttribute.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2230 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/JOURNALISM/features/TopPlayerAttribute.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2274 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/JOURNALISM/features/TopPlayerQuitType.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4478 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/JOURNALISM/features/TotalFails.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2088 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/JOURNALISM/features/TotalLevelTime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3951 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/JOURNALISM/features/UserPlayTime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4732 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/JOURNALISM/features/WorstAttribute.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2244 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/JOURNALISM/features/WorstPlayerAttribute.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2048 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/JOURNALISM/features/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:40:41.248908 opengamedata_core-0.0.7/src/ogd/games/JOURNALISM/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)    45415 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/JOURNALISM/schemas/JOURNALISM.json.template
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:40:41.248908 opengamedata_core-0.0.7/src/ogd/games/JOWILDER/
+-rw-r--r--   0 runner    (1001) docker     (127)     5210 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/JOWILDER/JowilderLoader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16451 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/JOWILDER/Jowilder_Enumerators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:40:41.252908 opengamedata_core-0.0.7/src/ogd/games/JOWILDER/features/
+-rw-r--r--   0 runner    (1001) docker     (127)     3092 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/JOWILDER/features/ActiveStateTime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1841 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/JOWILDER/features/Clicks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1441 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/JOWILDER/features/EventCount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1739 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/JOWILDER/features/FirstInteraction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/JOWILDER/features/GameScript.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/JOWILDER/features/GameVersion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1362 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/JOWILDER/features/Hovers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2461 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/JOWILDER/features/IdleState.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7612 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/JOWILDER/features/Interaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2341 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/JOWILDER/features/InteractionName.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4595 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/JOWILDER/features/InteractionTextBoxesPerSecond.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4590 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/JOWILDER/features/InteractionWordsPerSecond.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1687 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/JOWILDER/features/LastInteraction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1723 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/JOWILDER/features/MeaningfulActions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2003 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/JOWILDER/features/NotebookUses.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3214 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/JOWILDER/features/QuestionAnswers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1773 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/JOWILDER/features/SessionDuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1890 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/JOWILDER/features/SessionStart.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5107 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/JOWILDER/features/SurveyItem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2794 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/JOWILDER/features/SurveyTime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/JOWILDER/features/UsedContinue.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1327 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/JOWILDER/features/UsedSaveCode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2154 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/JOWILDER/features/UserEnabled.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/JOWILDER/features/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1925 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/JOWILDER/get_jowilder_all_items.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:40:41.252908 opengamedata_core-0.0.7/src/ogd/games/JOWILDER/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)    35912 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/JOWILDER/schemas/JOWILDER.json.template
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:40:41.252908 opengamedata_core-0.0.7/src/ogd/games/LAKELAND/
+-rw-r--r--   0 runner    (1001) docker     (127)     2361 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/LAKELAND/LakelandLoader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:40:41.260908 opengamedata_core-0.0.7/src/ogd/games/LAKELAND/features/
+-rw-r--r--   0 runner    (1001) docker     (127)     2039 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/LAKELAND/features/ActionsLastXSecondsModel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      607 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/LAKELAND/features/DeathCountModel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11750 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/LAKELAND/features/DeathPredModel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8664 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/LAKELAND/features/DeathThresholdModel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4916 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/LAKELAND/features/DiagonalFarmDetectorModel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7995 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/LAKELAND/features/FeatSeqPercent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2294 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/LAKELAND/features/FeatVelocity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/LAKELAND/features/FeatureModel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8478 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/LAKELAND/features/LAKELAND_models.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4415 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/LAKELAND/features/LakelandEnumerators.json
+-rw-r--r--   0 runner    (1001) docker     (127)    69736 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/LAKELAND/features/LakelandExtractor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2639 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/LAKELAND/features/LinearModel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2701 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/LAKELAND/features/LogisticModel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3353 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/LAKELAND/features/MapSummaryModel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/LAKELAND/features/Model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2574 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/LAKELAND/features/MoneyAccumulationModel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      444 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/LAKELAND/features/NthEventModel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      496 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/LAKELAND/features/PlayingTimeModel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3287 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/LAKELAND/features/PopulationModel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4813 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/LAKELAND/features/RecentPurchasesModel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1264 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/LAKELAND/features/SequenceModel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4909 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/LAKELAND/features/SimpleFarmAbandonmentModel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      850 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/LAKELAND/features/SingleFeatureModel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6060 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/LAKELAND/features/TimeSinceEventTypes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/LAKELAND/features/TimeSinceLastSaleModel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      507 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/LAKELAND/features/TownCompositionFeatureModel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2026 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/LAKELAND/features/TownCompositionModel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/LAKELAND/features/TutorialProgressionModel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    82382 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/LAKELAND/features/WAVES_models.json
+-rw-r--r--   0 runner    (1001) docker     (127)    82382 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/LAKELAND/features/WAVES_models_L8_Q0_Q1.json
+-rw-r--r--   0 runner    (1001) docker     (127)    49819 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/LAKELAND/features/WAVES_models_L8_and_Q0.json
+-rw-r--r--   0 runner    (1001) docker     (127)    28429 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/LAKELAND/features/WAVES_models_L8_complete_and_current.json
+-rw-r--r--   0 runner    (1001) docker     (127)    21021 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/LAKELAND/features/WAVES_models_L8_only_complete.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/LAKELAND/features/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2331 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/LAKELAND/produce_lakeland_enumerators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:40:41.260908 opengamedata_core-0.0.7/src/ogd/games/LAKELAND/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)   115553 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/LAKELAND/schemas/LAKELAND.json.template
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:40:41.260908 opengamedata_core-0.0.7/src/ogd/games/MAGNET/
+-rw-r--r--   0 runner    (1001) docker     (127)     2350 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/MAGNET/MagnetLoader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:40:41.260908 opengamedata_core-0.0.7/src/ogd/games/MAGNET/features/
+-rw-r--r--   0 runner    (1001) docker     (127)     8600 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/MAGNET/features/MagnetExtractor.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/MAGNET/features/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:40:41.260908 opengamedata_core-0.0.7/src/ogd/games/MAGNET/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)     7887 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/MAGNET/schemas/MAGNET.json.template
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:40:41.204908 opengamedata_core-0.0.7/src/ogd/games/MASHOPOLIS/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:40:41.260908 opengamedata_core-0.0.7/src/ogd/games/MASHOPOLIS/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)    10063 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/MASHOPOLIS/schemas/MASHOPOLIS.json.template
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:40:41.260908 opengamedata_core-0.0.7/src/ogd/games/PENGUINS/
+-rw-r--r--   0 runner    (1001) docker     (127)     2970 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/PENGUINS/DBExport.json
+-rw-r--r--   0 runner    (1001) docker     (127)     8007 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/PENGUINS/PenguinsLoader.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/PENGUINS/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:40:41.260908 opengamedata_core-0.0.7/src/ogd/games/PENGUINS/detectors/
+-rw-r--r--   0 runner    (1001) docker     (127)     5164 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/PENGUINS/detectors/RegionEnter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6271 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/PENGUINS/detectors/RegionExit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/PENGUINS/detectors/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:40:41.264908 opengamedata_core-0.0.7/src/ogd/games/PENGUINS/features/
+-rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/PENGUINS/features/ActivityCompleted.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2723 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/PENGUINS/features/ActivityDuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/PENGUINS/features/BuiltNestCount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1445 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/PENGUINS/features/BuiltWrongNestCount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/PENGUINS/features/EatFishCount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/PENGUINS/features/EggLostCount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/PENGUINS/features/EggRecoverTime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1662 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/PENGUINS/features/GazeCount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2666 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/PENGUINS/features/GazeDuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/PENGUINS/features/LogVersion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4231 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/PENGUINS/features/MirrorWaddleDuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/PENGUINS/features/PenguinInteractCount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2508 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/PENGUINS/features/PlayerInactiveAvgDuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2299 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/PENGUINS/features/RegionDuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1797 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/PENGUINS/features/RegionEnterCount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/PENGUINS/features/RegionsEncountered.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/PENGUINS/features/RingChimesCount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/PENGUINS/features/RockBashCount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1419 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/PENGUINS/features/RockMultiplePickupCount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/PENGUINS/features/RockPickupCount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3212 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/PENGUINS/features/SessionDuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/PENGUINS/features/SkuaBashCount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/PENGUINS/features/SkuaPeckCount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1971 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/PENGUINS/features/SnowBallDuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/PENGUINS/features/WaddleCount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1698 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/PENGUINS/features/WaddlePerRegion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1474 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/PENGUINS/features/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:40:41.264908 opengamedata_core-0.0.7/src/ogd/games/PENGUINS/features/bases/
+-rw-r--r--   0 runner    (1001) docker     (127)     3507 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/PENGUINS/features/bases/PerRegionFeature.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:40:41.264908 opengamedata_core-0.0.7/src/ogd/games/PENGUINS/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)    30981 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/PENGUINS/schemas/PENGUINS.json.template
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:40:41.264908 opengamedata_core-0.0.7/src/ogd/games/SHADOWSPECT/
+-rw-r--r--   0 runner    (1001) docker     (127)     3373 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/SHADOWSPECT/ShadowspectLoader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:40:41.268908 opengamedata_core-0.0.7/src/ogd/games/SHADOWSPECT/features/
+-rw-r--r--   0 runner    (1001) docker     (127)     2951 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/SHADOWSPECT/features/FunnelByUser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7674 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/SHADOWSPECT/features/LevelsOfDifficulty.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/SHADOWSPECT/features/MoveShapeCount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3916 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/SHADOWSPECT/features/SequenceBetweenPuzzles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8242 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/SHADOWSPECT/features/SequenceWithinPuzzles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/SHADOWSPECT/features/SessionID.py
+-rw-r--r--   0 runner    (1001) docker     (127)      344 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/SHADOWSPECT/features/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:40:41.268908 opengamedata_core-0.0.7/src/ogd/games/SHADOWSPECT/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)    29173 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/SHADOWSPECT/schemas/SHADOWSPECT.json.template
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:40:41.268908 opengamedata_core-0.0.7/src/ogd/games/SHIPWRECKS/
+-rw-r--r--   0 runner    (1001) docker     (127)     4681 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/SHIPWRECKS/ShipwrecksLoader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:40:41.268908 opengamedata_core-0.0.7/src/ogd/games/SHIPWRECKS/features/
+-rw-r--r--   0 runner    (1001) docker     (127)     2167 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/SHIPWRECKS/features/ActiveJobs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2336 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/SHIPWRECKS/features/EventList.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/SHIPWRECKS/features/EvidenceBoardCompleteCount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3548 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/SHIPWRECKS/features/JobsAttempted.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1225 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/SHIPWRECKS/features/JobsCompleted.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/SHIPWRECKS/features/MissionDiveTime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/SHIPWRECKS/features/MissionSonarTimeToComplete.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/SHIPWRECKS/features/PlayerSummary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1948 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/SHIPWRECKS/features/PopulationSummary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/SHIPWRECKS/features/SessionDuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/SHIPWRECKS/features/SessionID.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2995 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/SHIPWRECKS/features/TopJobCompletionDestinations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2739 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/SHIPWRECKS/features/TopJobSwitchDestinations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/SHIPWRECKS/features/TotalDiveTime.py
+-rw-r--r--   0 runner    (1001) docker     (127)      798 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/SHIPWRECKS/features/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:40:41.268908 opengamedata_core-0.0.7/src/ogd/games/SHIPWRECKS/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)    10509 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/SHIPWRECKS/schemas/SHIPWRECKS.json.template
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:40:41.268908 opengamedata_core-0.0.7/src/ogd/games/THERMOVR/
+-rw-r--r--   0 runner    (1001) docker     (127)        3 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/THERMOVR/DBExport.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5667 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/THERMOVR/ThermoVRLoader.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/THERMOVR/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:40:41.268908 opengamedata_core-0.0.7/src/ogd/games/THERMOVR/detectors/
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/THERMOVR/detectors/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:40:41.272908 opengamedata_core-0.0.7/src/ogd/games/THERMOVR/features/
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/THERMOVR/features/LabCompleteCount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1891 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/THERMOVR/features/LeftHandMoves.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/THERMOVR/features/PhasesReached.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/THERMOVR/features/PlayMode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1896 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/THERMOVR/features/RightHandMoves.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/THERMOVR/features/TaskCompleteCount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1760 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/THERMOVR/features/ToolNudgeCount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1700 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/THERMOVR/features/ToolSliderTime.py
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/THERMOVR/features/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:40:41.272908 opengamedata_core-0.0.7/src/ogd/games/THERMOVR/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)    51378 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/THERMOVR/schemas/THERMOVR.json.template
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:40:41.272908 opengamedata_core-0.0.7/src/ogd/games/TRANSFORMATION_QUEST/
+-rw-r--r--   0 runner    (1001) docker     (127)      777 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/TRANSFORMATION_QUEST/DBExport.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:40:41.272908 opengamedata_core-0.0.7/src/ogd/games/TRANSFORMATION_QUEST/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)    25177 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/TRANSFORMATION_QUEST/schemas/TRANSFORMATION_QUEST.json.template
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:40:41.272908 opengamedata_core-0.0.7/src/ogd/games/WAVES/
+-rw-r--r--   0 runner    (1001) docker     (127)    37336 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/WAVES/WaveLoader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:40:41.280908 opengamedata_core-0.0.7/src/ogd/games/WAVES/features/
+-rw-r--r--   0 runner    (1001) docker     (127)     1710 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/WAVES/features/AmplitudeGoodMoveCount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1425 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/WAVES/features/AverageFails.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3489 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/WAVES/features/AverageLevelTime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1876 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/WAVES/features/AverageMoveTypeChanges.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1478 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/WAVES/features/AverageSliderMoves.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/WAVES/features/BeginCount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2014 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/WAVES/features/ClosenessIntercept.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/WAVES/features/ClosenessR2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/WAVES/features/ClosenessSlope.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/WAVES/features/Completed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1194 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/WAVES/features/FirstMoveType.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1168 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/WAVES/features/MenuButtonCount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1704 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/WAVES/features/OffsetGoodMoveCount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/WAVES/features/OverallPercentAmplitudeMoves.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/WAVES/features/OverallPercentOffsetMoves.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1451 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/WAVES/features/OverallPercentWavelengthMoves.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1319 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/WAVES/features/OverallSliderAverageRange.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1315 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/WAVES/features/OverallSliderAverageStandardDeviations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1921 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/WAVES/features/PercentAmplitudeGoodMoves.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/WAVES/features/PercentAmplitudeMoves.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1903 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/WAVES/features/PercentOffsetGoodMoves.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1327 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/WAVES/features/PercentOffsetMoves.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1845 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/WAVES/features/PercentWavelengthGoodMoves.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/WAVES/features/PercentWavelengthMoves.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/WAVES/features/PersistentSessionID.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/WAVES/features/QuestionAnswered.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/WAVES/features/QuestionCorrect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/WAVES/features/RangeIntercept.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/WAVES/features/RangeR2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/WAVES/features/RangeSlope.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/WAVES/features/SequenceLevel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/WAVES/features/SessionID.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1328 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/WAVES/features/SliderAverageRange.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/WAVES/features/SliderAverageStandardDeviations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/WAVES/features/SucceedCount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2597 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/WAVES/features/TimeToAnswerMS.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/WAVES/features/TotalArrowMoves.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/WAVES/features/TotalFails.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1986 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/WAVES/features/TotalLevelTime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/WAVES/features/TotalMoveTypeChanges.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/WAVES/features/TotalResets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/WAVES/features/TotalSkips.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1192 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/WAVES/features/TotalSliderMoves.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1726 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/WAVES/features/WavelengthGoodMoveCount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2575 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/WAVES/features/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:40:41.280908 opengamedata_core-0.0.7/src/ogd/games/WAVES/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)    21383 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/WAVES/schemas/WAVES.json.template
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:40:41.204908 opengamedata_core-0.0.7/src/ogd/games/WEATHER_STATION/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:40:41.280908 opengamedata_core-0.0.7/src/ogd/games/WEATHER_STATION/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)    34344 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/WEATHER_STATION/schemas/WEATHER_STATION.json.template
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:40:41.204908 opengamedata_core-0.0.7/src/ogd/games/WIND/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:40:41.280908 opengamedata_core-0.0.7/src/ogd/games/WIND/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/WIND/schemas/WIND.json.template
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 22:39:59.000000 opengamedata_core-0.0.7/src/ogd/games/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:40:41.280908 opengamedata_core-0.0.7/src/opengamedata_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4796 2024-05-30 22:40:41.000000 opengamedata_core-0.0.7/src/opengamedata_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    22284 2024-05-30 22:40:41.000000 opengamedata_core-0.0.7/src/opengamedata_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 22:40:41.000000 opengamedata_core-0.0.7/src/opengamedata_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-30 22:40:41.000000 opengamedata_core-0.0.7/src/opengamedata_core.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:40:41.280908 opengamedata_core-0.0.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3113 2024-05-30 22:40:00.000000 opengamedata_core-0.0.7/tests/test_lakeland_models.py
```

### Comparing `opengamedata_core-0.0.6/LICENSE` & `opengamedata_core-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/PKG-INFO` & `opengamedata_core-0.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opengamedata-core
-Version: 0.0.6
+Version: 0.0.7
 Summary: A package for retrieving and processing event-based video game data. Additional authors: Nick Spevacek, Renee Li, John McCloskey, Zach Studdiford, Glenn Palmer, Haishuo Chen, Daus, Ameya Kshirsagar, Yunqing Xiao, Erik Harpstead, Manuel Jesus Gomez Moratilla
 Author-email: Luke Swanson <superscription58@gmail.com>, David Gagnon <djgagnon@wisc.edu>
 Project-URL: Homepage, https://github.com/opengamedata/opengamedata-core
 Project-URL: Bug Tracker, https://github.com/opengamedata/opengamedata-core/issues
 Project-URL: Documentation, https://opengamedata-doc.readthedocs.io/en/latest/index.html
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `opengamedata_core-0.0.6/README.md` & `opengamedata_core-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/pyproject.toml` & `opengamedata_core-0.0.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/core/exec/Commands.py` & `opengamedata_core-0.0.7/src/ogd/core/exec/Commands.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/core/exec/Generators.py` & `opengamedata_core-0.0.7/src/ogd/core/exec/Generators.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/core/exec/Parsers.py` & `opengamedata_core-0.0.7/src/ogd/core/exec/Parsers.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/core/games/AQUALAB/features/PlayLocations.py` & `opengamedata_core-0.0.7/src/ogd/core/games/AQUALAB/features/PlayLocations.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/core/generators/Generator.py` & `opengamedata_core-0.0.7/src/ogd/core/generators/Generator.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/core/generators/GeneratorLoader.py` & `opengamedata_core-0.0.7/src/ogd/core/generators/GeneratorLoader.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/core/generators/detectors/Detector.py` & `opengamedata_core-0.0.7/src/ogd/core/generators/detectors/Detector.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/core/generators/detectors/DetectorEvent.py` & `opengamedata_core-0.0.7/src/ogd/core/generators/detectors/DetectorEvent.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/core/generators/extractors/Extractor.py` & `opengamedata_core-0.0.7/src/ogd/core/generators/extractors/Extractor.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/core/generators/extractors/Feature.py` & `opengamedata_core-0.0.7/src/ogd/core/generators/extractors/Feature.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/core/generators/extractors/PerCountFeature.py` & `opengamedata_core-0.0.7/src/ogd/core/generators/extractors/PerCountFeature.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/core/generators/extractors/PerLevelFeature.py` & `opengamedata_core-0.0.7/src/ogd/core/generators/extractors/PerLevelFeature.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/core/generators/extractors/SessionFeature.py` & `opengamedata_core-0.0.7/src/ogd/core/generators/extractors/SessionFeature.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/core/generators/legacy/LegacyDetector.py` & `opengamedata_core-0.0.7/src/ogd/core/generators/legacy/LegacyDetector.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/core/generators/legacy/LegacyFeature.py` & `opengamedata_core-0.0.7/src/ogd/core/generators/legacy/LegacyFeature.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/core/generators/legacy/LegacyLoader.py` & `opengamedata_core-0.0.7/src/ogd/core/generators/legacy/LegacyLoader.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/core/generators/registries/DetectorRegistry.py` & `opengamedata_core-0.0.7/src/ogd/core/generators/registries/DetectorRegistry.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/core/generators/registries/ExtractorRegistry.py` & `opengamedata_core-0.0.7/src/ogd/core/generators/registries/ExtractorRegistry.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/core/generators/registries/GeneratorRegistry.py` & `opengamedata_core-0.0.7/src/ogd/core/generators/registries/GeneratorRegistry.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/core/interfaces/BQFirebaseInterface.py` & `opengamedata_core-0.0.7/src/ogd/core/interfaces/BQFirebaseInterface.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/core/interfaces/BigQueryCodingInterface.py` & `opengamedata_core-0.0.7/src/ogd/core/interfaces/BigQueryCodingInterface.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/core/interfaces/BigQueryInterface.py` & `opengamedata_core-0.0.7/src/ogd/core/interfaces/BigQueryInterface.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/core/interfaces/CSVInterface.py` & `opengamedata_core-0.0.7/src/ogd/core/interfaces/CSVInterface.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/core/interfaces/CodingInterface.py` & `opengamedata_core-0.0.7/src/ogd/core/interfaces/CodingInterface.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/core/interfaces/DataInterface.py` & `opengamedata_core-0.0.7/src/ogd/core/interfaces/DataInterface.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/core/interfaces/Interface.py` & `opengamedata_core-0.0.7/src/ogd/core/interfaces/Interface.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/core/interfaces/MySQLInterface.py` & `opengamedata_core-0.0.7/src/ogd/core/interfaces/MySQLInterface.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/core/interfaces/outerfaces/DataOuterface.py` & `opengamedata_core-0.0.7/src/ogd/core/interfaces/outerfaces/DataOuterface.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/core/interfaces/outerfaces/DebugOuterface.py` & `opengamedata_core-0.0.7/src/ogd/core/interfaces/outerfaces/DebugOuterface.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/core/interfaces/outerfaces/DictionaryOuterface.py` & `opengamedata_core-0.0.7/src/ogd/core/interfaces/outerfaces/DictionaryOuterface.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/core/interfaces/outerfaces/TSVOuterface.py` & `opengamedata_core-0.0.7/src/ogd/core/interfaces/outerfaces/TSVOuterface.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/core/managers/EventManager.py` & `opengamedata_core-0.0.7/src/ogd/core/managers/EventManager.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/core/managers/ExportManager.py` & `opengamedata_core-0.0.7/src/ogd/core/managers/ExportManager.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/core/managers/FeatureManager.py` & `opengamedata_core-0.0.7/src/ogd/core/managers/FeatureManager.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/core/models/Event.py` & `opengamedata_core-0.0.7/src/ogd/core/models/Event.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/core/models/FeatureData.py` & `opengamedata_core-0.0.7/src/ogd/core/models/FeatureData.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/core/processors/ClassroomDetector.py` & `opengamedata_core-0.0.7/src/ogd/core/processors/ClassroomDetector.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/core/processors/DetectorProcessor.py` & `opengamedata_core-0.0.7/src/ogd/core/processors/DetectorProcessor.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/core/processors/EventProcessor.py` & `opengamedata_core-0.0.7/src/ogd/core/processors/EventProcessor.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/core/processors/ExtractorProcessor.py` & `opengamedata_core-0.0.7/src/ogd/core/processors/ExtractorProcessor.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/core/processors/GeneratorProcessor.py` & `opengamedata_core-0.0.7/src/ogd/core/processors/GeneratorProcessor.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/core/processors/PlayerProcessor.py` & `opengamedata_core-0.0.7/src/ogd/core/processors/PlayerProcessor.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/core/processors/PopulationProcessor.py` & `opengamedata_core-0.0.7/src/ogd/core/processors/PopulationProcessor.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/core/processors/Processor.py` & `opengamedata_core-0.0.7/src/ogd/core/processors/Processor.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/core/processors/SessionProcessor.py` & `opengamedata_core-0.0.7/src/ogd/core/processors/SessionProcessor.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/core/requests/Request.py` & `opengamedata_core-0.0.7/src/ogd/core/requests/Request.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/core/requests/RequestResult.py` & `opengamedata_core-0.0.7/src/ogd/core/requests/RequestResult.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/core/schemas/Schema.py` & `opengamedata_core-0.0.7/src/ogd/core/schemas/Schema.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/core/schemas/configs/ConfigSchema.py` & `opengamedata_core-0.0.7/src/ogd/core/schemas/configs/ConfigSchema.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/core/schemas/configs/GameSourceSchema.py` & `opengamedata_core-0.0.7/src/ogd/core/schemas/configs/GameSourceSchema.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/core/schemas/configs/IndexingSchema.py` & `opengamedata_core-0.0.7/src/ogd/core/schemas/configs/IndexingSchema.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/core/schemas/configs/LegacyConfigSchema.py` & `opengamedata_core-0.0.7/src/ogd/core/schemas/configs/LegacyConfigSchema.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/core/schemas/configs/data_sources/BigQuerySourceSchema.py` & `opengamedata_core-0.0.7/src/ogd/core/schemas/configs/data_sources/BigQuerySourceSchema.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/core/schemas/configs/data_sources/DataSourceSchema.py` & `opengamedata_core-0.0.7/src/ogd/core/schemas/configs/data_sources/DataSourceSchema.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/core/schemas/configs/data_sources/FileSourceSchema.py` & `opengamedata_core-0.0.7/src/ogd/core/schemas/configs/data_sources/FileSourceSchema.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/core/schemas/configs/data_sources/MySQLSourceSchema.py` & `opengamedata_core-0.0.7/src/ogd/core/schemas/configs/data_sources/MySQLSourceSchema.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/core/schemas/datasets/DatasetSchema.py` & `opengamedata_core-0.0.7/src/ogd/core/schemas/datasets/DatasetSchema.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/core/schemas/datasets/FileListSchema.py` & `opengamedata_core-0.0.7/src/ogd/core/schemas/datasets/FileListSchema.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/core/schemas/games/AggregateSchema.py` & `opengamedata_core-0.0.7/src/ogd/core/schemas/games/AggregateSchema.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/core/schemas/games/DataElementSchema.py` & `opengamedata_core-0.0.7/src/ogd/core/schemas/games/DataElementSchema.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/core/schemas/games/DetectorMapSchema.py` & `opengamedata_core-0.0.7/src/ogd/core/schemas/games/DetectorMapSchema.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/core/schemas/games/DetectorSchema.py` & `opengamedata_core-0.0.7/src/ogd/core/schemas/games/DetectorSchema.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/core/schemas/games/EventSchema.py` & `opengamedata_core-0.0.7/src/ogd/core/schemas/games/EventSchema.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/core/schemas/games/ExtractorSchema.py` & `opengamedata_core-0.0.7/src/ogd/core/schemas/games/ExtractorSchema.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/core/schemas/games/FeatureMapSchema.py` & `opengamedata_core-0.0.7/src/ogd/core/schemas/games/FeatureMapSchema.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/core/schemas/games/FeatureSchema.py` & `opengamedata_core-0.0.7/src/ogd/core/schemas/games/FeatureSchema.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/core/schemas/games/GameSchema.py` & `opengamedata_core-0.0.7/src/ogd/core/schemas/games/GameSchema.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/core/schemas/games/GameStateSchema.py` & `opengamedata_core-0.0.7/src/ogd/core/schemas/games/GameStateSchema.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/core/schemas/games/PerCountSchema.py` & `opengamedata_core-0.0.7/src/ogd/core/schemas/games/PerCountSchema.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/core/schemas/table_schemas/BIGQUERY.json` & `opengamedata_core-0.0.7/src/ogd/core/schemas/table_schemas/BIGQUERY.json`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/core/schemas/table_schemas/FIELDDAY_MYSQL.json` & `opengamedata_core-0.0.7/src/ogd/core/schemas/table_schemas/FIELDDAY_MYSQL.json`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/core/schemas/table_schemas/FIREBASE.json` & `opengamedata_core-0.0.7/src/ogd/core/schemas/table_schemas/FIREBASE.json`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/core/schemas/table_schemas/MASHOPOLIS_MYSQL.json` & `opengamedata_core-0.0.7/src/ogd/core/schemas/table_schemas/MASHOPOLIS_MYSQL.json`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/core/schemas/table_schemas/OGD_EVENT_FILE.json` & `opengamedata_core-0.0.7/src/ogd/core/schemas/table_schemas/OGD_EVENT_FILE.json`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/core/schemas/table_schemas/OPENGAMEDATA_BIGQUERY.json` & `opengamedata_core-0.0.7/src/ogd/core/schemas/table_schemas/OPENGAMEDATA_BIGQUERY.json`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/core/schemas/table_schemas/OPENGAMEDATA_MYSQL.json` & `opengamedata_core-0.0.7/src/ogd/core/schemas/table_schemas/OPENGAMEDATA_MYSQL.json`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/core/schemas/table_schemas/SHIPWRECKS.json` & `opengamedata_core-0.0.7/src/ogd/core/schemas/table_schemas/SHIPWRECKS.json`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/core/schemas/tables/ColumnMapSchema.py` & `opengamedata_core-0.0.7/src/ogd/core/schemas/tables/ColumnMapSchema.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/core/schemas/tables/ColumnSchema.py` & `opengamedata_core-0.0.7/src/ogd/core/schemas/tables/ColumnSchema.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/core/schemas/tables/TableSchema.py` & `opengamedata_core-0.0.7/src/ogd/core/schemas/tables/TableSchema.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/core/utils/Logger.py` & `opengamedata_core-0.0.7/src/ogd/core/utils/Logger.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/core/utils/Readme.py` & `opengamedata_core-0.0.7/src/ogd/core/utils/Readme.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/core/utils/SemanticVersion.py` & `opengamedata_core-0.0.7/src/ogd/core/utils/SemanticVersion.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/core/utils/utils.py` & `opengamedata_core-0.0.7/src/ogd/core/utils/utils.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/ALL_YOU_CAN_ET/schemas/ALL_YOU_CAN_ET.json.template` & `opengamedata_core-0.0.7/src/ogd/games/ALL_YOU_CAN_ET/schemas/ALL_YOU_CAN_ET.json.template`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/AQUALAB/AqualabLoader.py` & `opengamedata_core-0.0.7/src/ogd/games/AQUALAB/AqualabLoader.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/AQUALAB/DBExport.json` & `opengamedata_core-0.0.7/src/ogd/games/AQUALAB/DBExport.json`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/AQUALAB/detectors/CollectFactNoJob.py` & `opengamedata_core-0.0.7/src/ogd/games/AQUALAB/detectors/CollectFactNoJob.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/AQUALAB/detectors/DiveSiteNoEvidence.py` & `opengamedata_core-0.0.7/src/ogd/games/AQUALAB/detectors/DiveSiteNoEvidence.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/AQUALAB/detectors/EchoRoomChange.py` & `opengamedata_core-0.0.7/src/ogd/games/AQUALAB/detectors/EchoRoomChange.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/AQUALAB/detectors/HintAndLeave.py` & `opengamedata_core-0.0.7/src/ogd/games/AQUALAB/detectors/HintAndLeave.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/AQUALAB/detectors/Idle.py` & `opengamedata_core-0.0.7/src/ogd/games/AQUALAB/detectors/Idle.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/AQUALAB/detectors/SceneChangeFrequently.py` & `opengamedata_core-0.0.7/src/ogd/games/AQUALAB/detectors/SceneChangeFrequently.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/AQUALAB/detectors/TwoHints.py` & `opengamedata_core-0.0.7/src/ogd/games/AQUALAB/detectors/TwoHints.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/AQUALAB/features/ActiveJobs.py` & `opengamedata_core-0.0.7/src/ogd/games/AQUALAB/features/ActiveJobs.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/AQUALAB/features/ActiveTime.py` & `opengamedata_core-0.0.7/src/ogd/games/AQUALAB/features/ActiveTime.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/AQUALAB/features/AppVersions.py` & `opengamedata_core-0.0.7/src/ogd/games/AQUALAB/features/AppVersions.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/AQUALAB/features/AverageSessionTime.py` & `opengamedata_core-0.0.7/src/ogd/games/AQUALAB/features/AverageSessionTime.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/AQUALAB/features/EchoSessionID.py` & `opengamedata_core-0.0.7/src/ogd/games/AQUALAB/features/EchoSessionID.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/AQUALAB/features/EventList.py` & `opengamedata_core-0.0.7/src/ogd/games/AQUALAB/features/EventList.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/AQUALAB/features/JobActiveTime.py` & `opengamedata_core-0.0.7/src/ogd/games/AQUALAB/features/JobActiveTime.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/AQUALAB/features/JobArgumentation.py` & `opengamedata_core-0.0.7/src/ogd/games/AQUALAB/features/JobArgumentation.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/AQUALAB/features/JobCompletionTime.py` & `opengamedata_core-0.0.7/src/ogd/games/AQUALAB/features/JobCompletionTime.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/AQUALAB/features/JobDiveSitesCount.py` & `opengamedata_core-0.0.7/src/ogd/games/AQUALAB/features/JobDiveSitesCount.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/AQUALAB/features/JobDiveTime.py` & `opengamedata_core-0.0.7/src/ogd/games/AQUALAB/features/JobDiveTime.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/AQUALAB/features/JobExperimentation.py` & `opengamedata_core-0.0.7/src/ogd/games/AQUALAB/features/JobExperimentation.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/AQUALAB/features/JobGuideCount.py` & `opengamedata_core-0.0.7/src/ogd/games/AQUALAB/features/JobGuideCount.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/AQUALAB/features/JobHelpCount.py` & `opengamedata_core-0.0.7/src/ogd/games/AQUALAB/features/JobHelpCount.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/AQUALAB/features/JobLocationChanges.py` & `opengamedata_core-0.0.7/src/ogd/games/AQUALAB/features/JobLocationChanges.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/AQUALAB/features/JobModeling.py` & `opengamedata_core-0.0.7/src/ogd/games/AQUALAB/features/JobModeling.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/AQUALAB/features/JobPlayTime.py` & `opengamedata_core-0.0.7/src/ogd/games/AQUALAB/features/JobPlayTime.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/AQUALAB/features/JobPriorAttempt.py` & `opengamedata_core-0.0.7/src/ogd/games/AQUALAB/features/JobPriorAttempt.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/AQUALAB/features/JobPriorComplete.py` & `opengamedata_core-0.0.7/src/ogd/games/AQUALAB/features/JobPriorComplete.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/AQUALAB/features/JobStartCount.py` & `opengamedata_core-0.0.7/src/ogd/games/AQUALAB/features/JobStartCount.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/AQUALAB/features/JobTasksCompleted.py` & `opengamedata_core-0.0.7/src/ogd/games/AQUALAB/features/JobTasksCompleted.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/AQUALAB/features/JobTriesInArgument.py` & `opengamedata_core-0.0.7/src/ogd/games/AQUALAB/features/JobTriesInArgument.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/AQUALAB/features/JobsAttempted.py` & `opengamedata_core-0.0.7/src/ogd/games/AQUALAB/features/JobsAttempted.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/AQUALAB/features/JobsCompleted.py` & `opengamedata_core-0.0.7/src/ogd/games/AQUALAB/features/JobsCompleted.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/AQUALAB/features/ModelExportCount.py` & `opengamedata_core-0.0.7/src/ogd/games/AQUALAB/features/ModelExportCount.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/AQUALAB/features/ModelInterveneCount.py` & `opengamedata_core-0.0.7/src/ogd/games/AQUALAB/features/ModelInterveneCount.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/AQUALAB/features/ModelPredictCount.py` & `opengamedata_core-0.0.7/src/ogd/games/AQUALAB/features/ModelPredictCount.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/AQUALAB/features/PerJobFeature.py` & `opengamedata_core-0.0.7/src/ogd/games/AQUALAB/features/PerJobFeature.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/AQUALAB/features/PlayerSummary.py` & `opengamedata_core-0.0.7/src/ogd/games/AQUALAB/features/PlayerSummary.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/AQUALAB/features/PopulationSummary.py` & `opengamedata_core-0.0.7/src/ogd/games/AQUALAB/features/PopulationSummary.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/AQUALAB/features/RegionJobCount.py` & `opengamedata_core-0.0.7/src/ogd/games/AQUALAB/features/RegionJobCount.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/AQUALAB/features/RegionName.py` & `opengamedata_core-0.0.7/src/ogd/games/AQUALAB/features/RegionName.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/AQUALAB/features/SessionDiveSitesCount.py` & `opengamedata_core-0.0.7/src/ogd/games/AQUALAB/features/SessionDiveSitesCount.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/AQUALAB/features/SessionDuration.py` & `opengamedata_core-0.0.7/src/ogd/games/AQUALAB/features/SessionDuration.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/AQUALAB/features/SessionGuideCount.py` & `opengamedata_core-0.0.7/src/ogd/games/AQUALAB/features/SessionGuideCount.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/AQUALAB/features/SessionHelpCount.py` & `opengamedata_core-0.0.7/src/ogd/games/AQUALAB/features/SessionHelpCount.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/AQUALAB/features/SessionID.py` & `opengamedata_core-0.0.7/src/ogd/games/AQUALAB/features/SessionID.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/AQUALAB/features/SessionJobsCompleted.py` & `opengamedata_core-0.0.7/src/ogd/games/AQUALAB/features/SessionJobsCompleted.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/AQUALAB/features/SwitchJobsCount.py` & `opengamedata_core-0.0.7/src/ogd/games/AQUALAB/features/SwitchJobsCount.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/AQUALAB/features/SyncCompletionTime.py` & `opengamedata_core-0.0.7/src/ogd/games/AQUALAB/features/SyncCompletionTime.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/AQUALAB/features/TankRulesCount.py` & `opengamedata_core-0.0.7/src/ogd/games/AQUALAB/features/TankRulesCount.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/AQUALAB/features/TopJobCompletionDestinations.py` & `opengamedata_core-0.0.7/src/ogd/games/AQUALAB/features/TopJobCompletionDestinations.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/AQUALAB/features/TopJobSwitchDestinations.py` & `opengamedata_core-0.0.7/src/ogd/games/AQUALAB/features/TopJobSwitchDestinations.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/AQUALAB/features/TotalArcticTime.py` & `opengamedata_core-0.0.7/src/ogd/games/AQUALAB/features/TotalArcticTime.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/AQUALAB/features/TotalArgumentationTime.py` & `opengamedata_core-0.0.7/src/ogd/games/AQUALAB/features/TotalArgumentationTime.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/AQUALAB/features/TotalBayouTime.py` & `opengamedata_core-0.0.7/src/ogd/games/AQUALAB/features/TotalBayouTime.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/AQUALAB/features/TotalCoralTime.py` & `opengamedata_core-0.0.7/src/ogd/games/AQUALAB/features/TotalCoralTime.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/AQUALAB/features/TotalDiveTime.py` & `opengamedata_core-0.0.7/src/ogd/games/AQUALAB/features/TotalDiveTime.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/AQUALAB/features/TotalExperimentationTime.py` & `opengamedata_core-0.0.7/src/ogd/games/AQUALAB/features/TotalExperimentationTime.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/AQUALAB/features/TotalGuideCount.py` & `opengamedata_core-0.0.7/src/ogd/games/AQUALAB/features/TotalGuideCount.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/AQUALAB/features/TotalHelpCount.py` & `opengamedata_core-0.0.7/src/ogd/games/AQUALAB/features/TotalHelpCount.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/AQUALAB/features/TotalKelpTime.py` & `opengamedata_core-0.0.7/src/ogd/games/AQUALAB/features/TotalKelpTime.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/AQUALAB/features/TotalModelingTime.py` & `opengamedata_core-0.0.7/src/ogd/games/AQUALAB/features/TotalModelingTime.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/AQUALAB/features/TotalPlayTime.py` & `opengamedata_core-0.0.7/src/ogd/games/AQUALAB/features/TotalPlayTime.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/AQUALAB/features/UserAvgActiveTime.py` & `opengamedata_core-0.0.7/src/ogd/games/AQUALAB/features/UserAvgActiveTime.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/AQUALAB/features/UserAvgSessionDuration.py` & `opengamedata_core-0.0.7/src/ogd/games/AQUALAB/features/UserAvgSessionDuration.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/AQUALAB/features/UserTotalSessionDuration.py` & `opengamedata_core-0.0.7/src/ogd/games/AQUALAB/features/UserTotalSessionDuration.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/AQUALAB/features/__init__.py` & `opengamedata_core-0.0.7/src/ogd/games/AQUALAB/features/__init__.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/AQUALAB/schemas/AQUALAB.json.template` & `opengamedata_core-0.0.7/src/ogd/games/AQUALAB/schemas/AQUALAB.json.template`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/BLOOM/schemas/BLOOM.json.template` & `opengamedata_core-0.0.7/src/ogd/games/BLOOM/schemas/BLOOM.json.template`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/CENSIO_SLIDE/schemas/CENSIO_SLIDE.json.template` & `opengamedata_core-0.0.7/src/ogd/games/CENSIO_SLIDE/schemas/CENSIO_SLIDE.json.template`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/CENSIO_STACK/schemas/CENSIO_STACK.json.template` & `opengamedata_core-0.0.7/src/ogd/games/CENSIO_STACK/schemas/CENSIO_STACK.json.template`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/CRUSH_STATION/schemas/CRUSH_STATION.json.template` & `opengamedata_core-0.0.7/src/ogd/games/CRUSH_STATION/schemas/CRUSH_STATION.json.template`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/CRYSTAL/CrystalLoader.py` & `opengamedata_core-0.0.7/src/ogd/games/CRYSTAL/CrystalLoader.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/CRYSTAL/features/CrystalExtractor.py` & `opengamedata_core-0.0.7/src/ogd/games/CRYSTAL/features/CrystalExtractor.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/CRYSTAL/schemas/CRYSTAL.json.template` & `opengamedata_core-0.0.7/src/ogd/games/CRYSTAL/schemas/CRYSTAL.json.template`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/GWAKKAMOLE/schemas/GWAKKAMOLE.json.template` & `opengamedata_core-0.0.7/src/ogd/games/GWAKKAMOLE/schemas/GWAKKAMOLE.json.template`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/ICECUBE/DBExport.json` & `opengamedata_core-0.0.7/src/ogd/games/ICECUBE/DBExport.json`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/ICECUBE/DBExport.py` & `opengamedata_core-0.0.7/src/ogd/games/ICECUBE/DBExport.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/ICECUBE/IcecubeLoader.py` & `opengamedata_core-0.0.7/src/ogd/games/ICECUBE/IcecubeLoader.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/ICECUBE/features/HeadsetOnCount.py` & `opengamedata_core-0.0.7/src/ogd/games/ICECUBE/features/HeadsetOnCount.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/ICECUBE/features/ObjectSelectionsDuringVoiceover.py` & `opengamedata_core-0.0.7/src/ogd/games/ICECUBE/features/ObjectSelectionsDuringVoiceover.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/ICECUBE/features/PerSceneFeature.py` & `opengamedata_core-0.0.7/src/ogd/games/ICECUBE/features/PerSceneFeature.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/ICECUBE/features/SceneDuration.py` & `opengamedata_core-0.0.7/src/ogd/games/ICECUBE/features/SceneDuration.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/ICECUBE/features/SceneFailureCount.py` & `opengamedata_core-0.0.7/src/ogd/games/ICECUBE/features/SceneFailureCount.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/ICECUBE/features/SceneFailures.py` & `opengamedata_core-0.0.7/src/ogd/games/ICECUBE/features/SceneFailures.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/ICECUBE/features/ScenesEncountered.py` & `opengamedata_core-0.0.7/src/ogd/games/ICECUBE/features/ScenesEncountered.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/ICECUBE/features/SessionDuration.py` & `opengamedata_core-0.0.7/src/ogd/games/ICECUBE/features/SessionDuration.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/ICECUBE/features/Session_Language.py` & `opengamedata_core-0.0.7/src/ogd/games/ICECUBE/features/Session_Language.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/ICECUBE/features/TaskTimeToComplete.py` & `opengamedata_core-0.0.7/src/ogd/games/ICECUBE/features/TaskTimeToComplete.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/ICECUBE/features/ViewportCountPerScene.py` & `opengamedata_core-0.0.7/src/ogd/games/ICECUBE/features/ViewportCountPerScene.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/ICECUBE/features/__init__.py` & `opengamedata_core-0.0.7/src/ogd/games/ICECUBE/features/__init__.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/ICECUBE/schemas/ICECUBE.json.template` & `opengamedata_core-0.0.7/src/ogd/games/ICECUBE/schemas/ICECUBE.json.template`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/JOURNALISM/JournalismLoader.py` & `opengamedata_core-0.0.7/src/ogd/games/JOURNALISM/JournalismLoader.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/JOURNALISM/features/AttributeView.py` & `opengamedata_core-0.0.7/src/ogd/games/JOURNALISM/features/AttributeView.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/JOURNALISM/features/ChoiceClickCount.py` & `opengamedata_core-0.0.7/src/ogd/games/JOURNALISM/features/ChoiceClickCount.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/JOURNALISM/features/ContinuesOnFail.py` & `opengamedata_core-0.0.7/src/ogd/games/JOURNALISM/features/ContinuesOnFail.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/JOURNALISM/features/EditorNoteOpen.py` & `opengamedata_core-0.0.7/src/ogd/games/JOURNALISM/features/EditorNoteOpen.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/JOURNALISM/features/FailureAttributes.py` & `opengamedata_core-0.0.7/src/ogd/games/JOURNALISM/features/FailureAttributes.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/JOURNALISM/features/FailureCount.py` & `opengamedata_core-0.0.7/src/ogd/games/JOURNALISM/features/FailureCount.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/JOURNALISM/features/FinalAttributes.py` & `opengamedata_core-0.0.7/src/ogd/games/JOURNALISM/features/FinalAttributes.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/JOURNALISM/features/GameComplete.py` & `opengamedata_core-0.0.7/src/ogd/games/JOURNALISM/features/GameComplete.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/JOURNALISM/features/LevelCompleteCount.py` & `opengamedata_core-0.0.7/src/ogd/games/JOURNALISM/features/LevelCompleteCount.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/JOURNALISM/features/LevelCompleted.py` & `opengamedata_core-0.0.7/src/ogd/games/JOURNALISM/features/LevelCompleted.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/JOURNALISM/features/LevelTime.py` & `opengamedata_core-0.0.7/src/ogd/games/JOURNALISM/features/LevelTime.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/JOURNALISM/features/MaxedPlayerAttribute.py` & `opengamedata_core-0.0.7/src/ogd/games/JOURNALISM/features/MaxedPlayerAttribute.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/JOURNALISM/features/MeanSnippetTime.py` & `opengamedata_core-0.0.7/src/ogd/games/JOURNALISM/features/MeanSnippetTime.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/JOURNALISM/features/PlayTime.py` & `opengamedata_core-0.0.7/src/ogd/games/JOURNALISM/features/PlayTime.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/JOURNALISM/features/PlayerAttributes.py` & `opengamedata_core-0.0.7/src/ogd/games/JOURNALISM/features/PlayerAttributes.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/JOURNALISM/features/QuitLevel.py` & `opengamedata_core-0.0.7/src/ogd/games/JOURNALISM/features/QuitLevel.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/JOURNALISM/features/QuitNode.py` & `opengamedata_core-0.0.7/src/ogd/games/JOURNALISM/features/QuitNode.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/JOURNALISM/features/QuitType.py` & `opengamedata_core-0.0.7/src/ogd/games/JOURNALISM/features/QuitType.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/JOURNALISM/features/QuitTypePerLevel.py` & `opengamedata_core-0.0.7/src/ogd/games/JOURNALISM/features/QuitTypePerLevel.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/JOURNALISM/features/SessionPlayTime.py` & `opengamedata_core-0.0.7/src/ogd/games/JOURNALISM/features/SessionPlayTime.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/JOURNALISM/features/SkillSequenceCount.py` & `opengamedata_core-0.0.7/src/ogd/games/JOURNALISM/features/SkillSequenceCount.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/JOURNALISM/features/SnippetReceivedCount.py` & `opengamedata_core-0.0.7/src/ogd/games/JOURNALISM/features/SnippetReceivedCount.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/JOURNALISM/features/SnippetReplace.py` & `opengamedata_core-0.0.7/src/ogd/games/JOURNALISM/features/SnippetReplace.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/JOURNALISM/features/SnippetsCollected.py` & `opengamedata_core-0.0.7/src/ogd/games/JOURNALISM/features/SnippetsCollected.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/JOURNALISM/features/SnippetsSubmitted.py` & `opengamedata_core-0.0.7/src/ogd/games/JOURNALISM/features/SnippetsSubmitted.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/JOURNALISM/features/StoryAlignment.py` & `opengamedata_core-0.0.7/src/ogd/games/JOURNALISM/features/StoryAlignment.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/JOURNALISM/features/StoryAlignmentSequence.py` & `opengamedata_core-0.0.7/src/ogd/games/JOURNALISM/features/StoryAlignmentSequence.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/JOURNALISM/features/StoryCompleteTime.py` & `opengamedata_core-0.0.7/src/ogd/games/JOURNALISM/features/StoryCompleteTime.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/JOURNALISM/features/StoryEditorTime.py` & `opengamedata_core-0.0.7/src/ogd/games/JOURNALISM/features/StoryEditorTime.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/JOURNALISM/features/StoryScore.py` & `opengamedata_core-0.0.7/src/ogd/games/JOURNALISM/features/StoryScore.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/JOURNALISM/features/StoryScoreSequence.py` & `opengamedata_core-0.0.7/src/ogd/games/JOURNALISM/features/StoryScoreSequence.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/JOURNALISM/features/TextClickCount.py` & `opengamedata_core-0.0.7/src/ogd/games/JOURNALISM/features/TextClickCount.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/JOURNALISM/features/TopAttribute.py` & `opengamedata_core-0.0.7/src/ogd/games/JOURNALISM/features/TopAttribute.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/JOURNALISM/features/TopPlayerAttribute.py` & `opengamedata_core-0.0.7/src/ogd/games/JOURNALISM/features/TopPlayerAttribute.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/JOURNALISM/features/TopPlayerQuitType.py` & `opengamedata_core-0.0.7/src/ogd/games/JOURNALISM/features/TopPlayerQuitType.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/JOURNALISM/features/TotalFails.py` & `opengamedata_core-0.0.7/src/ogd/games/JOURNALISM/features/TotalFails.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/JOURNALISM/features/TotalLevelTime.py` & `opengamedata_core-0.0.7/src/ogd/games/JOURNALISM/features/TotalLevelTime.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/JOURNALISM/features/UserPlayTime.py` & `opengamedata_core-0.0.7/src/ogd/games/JOURNALISM/features/UserPlayTime.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/JOURNALISM/features/WorstAttribute.py` & `opengamedata_core-0.0.7/src/ogd/games/JOURNALISM/features/WorstAttribute.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/JOURNALISM/features/WorstPlayerAttribute.py` & `opengamedata_core-0.0.7/src/ogd/games/JOURNALISM/features/WorstPlayerAttribute.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/JOURNALISM/features/__init__.py` & `opengamedata_core-0.0.7/src/ogd/games/JOURNALISM/features/__init__.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/JOURNALISM/schemas/JOURNALISM.json.template` & `opengamedata_core-0.0.7/src/ogd/games/JOURNALISM/schemas/JOURNALISM.json.template`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/JOWILDER/JowilderLoader.py` & `opengamedata_core-0.0.7/src/ogd/games/JOWILDER/JowilderLoader.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/JOWILDER/Jowilder_Enumerators.py` & `opengamedata_core-0.0.7/src/ogd/games/JOWILDER/Jowilder_Enumerators.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/JOWILDER/features/ActiveStateTime.py` & `opengamedata_core-0.0.7/src/ogd/games/JOWILDER/features/ActiveStateTime.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/JOWILDER/features/Clicks.py` & `opengamedata_core-0.0.7/src/ogd/games/JOWILDER/features/Clicks.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/JOWILDER/features/EventCount.py` & `opengamedata_core-0.0.7/src/ogd/games/JOWILDER/features/EventCount.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/JOWILDER/features/FirstInteraction.py` & `opengamedata_core-0.0.7/src/ogd/games/JOWILDER/features/FirstInteraction.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/JOWILDER/features/GameScript.py` & `opengamedata_core-0.0.7/src/ogd/games/JOWILDER/features/GameScript.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/JOWILDER/features/GameVersion.py` & `opengamedata_core-0.0.7/src/ogd/games/JOWILDER/features/GameVersion.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/JOWILDER/features/Hovers.py` & `opengamedata_core-0.0.7/src/ogd/games/JOWILDER/features/Hovers.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/JOWILDER/features/IdleState.py` & `opengamedata_core-0.0.7/src/ogd/games/JOWILDER/features/IdleState.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/JOWILDER/features/Interaction.py` & `opengamedata_core-0.0.7/src/ogd/games/JOWILDER/features/Interaction.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/JOWILDER/features/InteractionName.py` & `opengamedata_core-0.0.7/src/ogd/games/JOWILDER/features/InteractionName.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/JOWILDER/features/InteractionTextBoxesPerSecond.py` & `opengamedata_core-0.0.7/src/ogd/games/JOWILDER/features/InteractionTextBoxesPerSecond.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/JOWILDER/features/InteractionWordsPerSecond.py` & `opengamedata_core-0.0.7/src/ogd/games/JOWILDER/features/InteractionWordsPerSecond.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/JOWILDER/features/LastInteraction.py` & `opengamedata_core-0.0.7/src/ogd/games/JOWILDER/features/LastInteraction.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/JOWILDER/features/MeaningfulActions.py` & `opengamedata_core-0.0.7/src/ogd/games/JOWILDER/features/MeaningfulActions.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/JOWILDER/features/NotebookUses.py` & `opengamedata_core-0.0.7/src/ogd/games/JOWILDER/features/NotebookUses.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/JOWILDER/features/QuestionAnswers.py` & `opengamedata_core-0.0.7/src/ogd/games/JOWILDER/features/QuestionAnswers.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/JOWILDER/features/SessionDuration.py` & `opengamedata_core-0.0.7/src/ogd/games/JOWILDER/features/SessionDuration.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/JOWILDER/features/SessionStart.py` & `opengamedata_core-0.0.7/src/ogd/games/JOWILDER/features/SessionStart.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/JOWILDER/features/SurveyItem.py` & `opengamedata_core-0.0.7/src/ogd/games/JOWILDER/features/SurveyItem.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/JOWILDER/features/SurveyTime.py` & `opengamedata_core-0.0.7/src/ogd/games/JOWILDER/features/SurveyTime.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/JOWILDER/features/UsedContinue.py` & `opengamedata_core-0.0.7/src/ogd/games/JOWILDER/features/UsedContinue.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/JOWILDER/features/UsedSaveCode.py` & `opengamedata_core-0.0.7/src/ogd/games/JOWILDER/features/UsedSaveCode.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/JOWILDER/features/UserEnabled.py` & `opengamedata_core-0.0.7/src/ogd/games/JOWILDER/features/UserEnabled.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/JOWILDER/features/__init__.py` & `opengamedata_core-0.0.7/src/ogd/games/JOWILDER/features/__init__.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/JOWILDER/get_jowilder_all_items.py` & `opengamedata_core-0.0.7/src/ogd/games/JOWILDER/get_jowilder_all_items.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/JOWILDER/schemas/JOWILDER.json.template` & `opengamedata_core-0.0.7/src/ogd/games/JOWILDER/schemas/JOWILDER.json.template`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/LAKELAND/LakelandLoader.py` & `opengamedata_core-0.0.7/src/ogd/games/LAKELAND/LakelandLoader.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/LAKELAND/features/ActionsLastXSecondsModel.py` & `opengamedata_core-0.0.7/src/ogd/games/LAKELAND/features/ActionsLastXSecondsModel.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/LAKELAND/features/DeathCountModel.py` & `opengamedata_core-0.0.7/src/ogd/games/LAKELAND/features/DeathCountModel.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/LAKELAND/features/DeathPredModel.py` & `opengamedata_core-0.0.7/src/ogd/games/LAKELAND/features/DeathPredModel.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/LAKELAND/features/DeathThresholdModel.py` & `opengamedata_core-0.0.7/src/ogd/games/LAKELAND/features/DeathThresholdModel.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/LAKELAND/features/DiagonalFarmDetectorModel.py` & `opengamedata_core-0.0.7/src/ogd/games/LAKELAND/features/DiagonalFarmDetectorModel.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/LAKELAND/features/FeatSeqPercent.py` & `opengamedata_core-0.0.7/src/ogd/games/LAKELAND/features/FeatSeqPercent.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/LAKELAND/features/FeatVelocity.py` & `opengamedata_core-0.0.7/src/ogd/games/LAKELAND/features/FeatVelocity.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/LAKELAND/features/FeatureModel.py` & `opengamedata_core-0.0.7/src/ogd/games/LAKELAND/features/FeatureModel.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/LAKELAND/features/LAKELAND_models.json` & `opengamedata_core-0.0.7/src/ogd/games/LAKELAND/features/LAKELAND_models.json`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/LAKELAND/features/LakelandEnumerators.json` & `opengamedata_core-0.0.7/src/ogd/games/LAKELAND/features/LakelandEnumerators.json`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/LAKELAND/features/LakelandExtractor.py` & `opengamedata_core-0.0.7/src/ogd/games/LAKELAND/features/LakelandExtractor.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/LAKELAND/features/LinearModel.py` & `opengamedata_core-0.0.7/src/ogd/games/LAKELAND/features/LinearModel.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/LAKELAND/features/LogisticModel.py` & `opengamedata_core-0.0.7/src/ogd/games/LAKELAND/features/LogisticModel.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/LAKELAND/features/MapSummaryModel.py` & `opengamedata_core-0.0.7/src/ogd/games/LAKELAND/features/MapSummaryModel.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/LAKELAND/features/Model.py` & `opengamedata_core-0.0.7/src/ogd/games/LAKELAND/features/Model.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/LAKELAND/features/MoneyAccumulationModel.py` & `opengamedata_core-0.0.7/src/ogd/games/LAKELAND/features/MoneyAccumulationModel.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/LAKELAND/features/PopulationModel.py` & `opengamedata_core-0.0.7/src/ogd/games/LAKELAND/features/PopulationModel.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/LAKELAND/features/RecentPurchasesModel.py` & `opengamedata_core-0.0.7/src/ogd/games/LAKELAND/features/RecentPurchasesModel.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/LAKELAND/features/SequenceModel.py` & `opengamedata_core-0.0.7/src/ogd/games/LAKELAND/features/SequenceModel.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/LAKELAND/features/SimpleFarmAbandonmentModel.py` & `opengamedata_core-0.0.7/src/ogd/games/LAKELAND/features/SimpleFarmAbandonmentModel.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/LAKELAND/features/SingleFeatureModel.py` & `opengamedata_core-0.0.7/src/ogd/games/LAKELAND/features/SingleFeatureModel.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/LAKELAND/features/TimeSinceEventTypes.py` & `opengamedata_core-0.0.7/src/ogd/games/LAKELAND/features/TimeSinceEventTypes.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/LAKELAND/features/TimeSinceLastSaleModel.py` & `opengamedata_core-0.0.7/src/ogd/games/LAKELAND/features/TimeSinceLastSaleModel.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/LAKELAND/features/TownCompositionModel.py` & `opengamedata_core-0.0.7/src/ogd/games/LAKELAND/features/TownCompositionModel.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/LAKELAND/features/TutorialProgressionModel.py` & `opengamedata_core-0.0.7/src/ogd/games/LAKELAND/features/TutorialProgressionModel.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/LAKELAND/features/WAVES_models.json` & `opengamedata_core-0.0.7/src/ogd/games/LAKELAND/features/WAVES_models.json`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/LAKELAND/features/WAVES_models_L8_Q0_Q1.json` & `opengamedata_core-0.0.7/src/ogd/games/LAKELAND/features/WAVES_models_L8_Q0_Q1.json`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/LAKELAND/features/WAVES_models_L8_and_Q0.json` & `opengamedata_core-0.0.7/src/ogd/games/LAKELAND/features/WAVES_models_L8_and_Q0.json`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/LAKELAND/features/WAVES_models_L8_complete_and_current.json` & `opengamedata_core-0.0.7/src/ogd/games/LAKELAND/features/WAVES_models_L8_complete_and_current.json`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/LAKELAND/features/WAVES_models_L8_only_complete.json` & `opengamedata_core-0.0.7/src/ogd/games/LAKELAND/features/WAVES_models_L8_only_complete.json`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/LAKELAND/produce_lakeland_enumerators.py` & `opengamedata_core-0.0.7/src/ogd/games/LAKELAND/produce_lakeland_enumerators.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/LAKELAND/schemas/LAKELAND.json.template` & `opengamedata_core-0.0.7/src/ogd/games/LAKELAND/schemas/LAKELAND.json.template`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/MAGNET/MagnetLoader.py` & `opengamedata_core-0.0.7/src/ogd/games/MAGNET/MagnetLoader.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/MAGNET/features/MagnetExtractor.py` & `opengamedata_core-0.0.7/src/ogd/games/MAGNET/features/MagnetExtractor.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/MAGNET/schemas/MAGNET.json.template` & `opengamedata_core-0.0.7/src/ogd/games/MAGNET/schemas/MAGNET.json.template`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/MASHOPOLIS/schemas/MASHOPOLIS.json.template` & `opengamedata_core-0.0.7/src/ogd/games/MASHOPOLIS/schemas/MASHOPOLIS.json.template`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/PENGUINS/DBExport.json` & `opengamedata_core-0.0.7/src/ogd/games/PENGUINS/DBExport.json`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/PENGUINS/PenguinsLoader.py` & `opengamedata_core-0.0.7/src/ogd/games/PENGUINS/PenguinsLoader.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/PENGUINS/detectors/RegionEnter.py` & `opengamedata_core-0.0.7/src/ogd/games/PENGUINS/detectors/RegionEnter.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/PENGUINS/detectors/RegionExit.py` & `opengamedata_core-0.0.7/src/ogd/games/PENGUINS/detectors/RegionExit.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/PENGUINS/features/ActivityCompleted.py` & `opengamedata_core-0.0.7/src/ogd/games/PENGUINS/features/ActivityCompleted.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/PENGUINS/features/ActivityDuration.py` & `opengamedata_core-0.0.7/src/ogd/games/PENGUINS/features/ActivityDuration.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/PENGUINS/features/BuiltNestCount.py` & `opengamedata_core-0.0.7/src/ogd/games/PENGUINS/features/BuiltNestCount.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/PENGUINS/features/BuiltWrongNestCount.py` & `opengamedata_core-0.0.7/src/ogd/games/PENGUINS/features/BuiltWrongNestCount.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/PENGUINS/features/EatFishCount.py` & `opengamedata_core-0.0.7/src/ogd/games/PENGUINS/features/EatFishCount.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/PENGUINS/features/EggLostCount.py` & `opengamedata_core-0.0.7/src/ogd/games/PENGUINS/features/EggLostCount.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/PENGUINS/features/EggRecoverTime.py` & `opengamedata_core-0.0.7/src/ogd/games/PENGUINS/features/EggRecoverTime.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/PENGUINS/features/GazeCount.py` & `opengamedata_core-0.0.7/src/ogd/games/PENGUINS/features/GazeCount.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/PENGUINS/features/GazeDuration.py` & `opengamedata_core-0.0.7/src/ogd/games/PENGUINS/features/GazeDuration.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/PENGUINS/features/LogVersion.py` & `opengamedata_core-0.0.7/src/ogd/games/PENGUINS/features/LogVersion.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/PENGUINS/features/MirrorWaddleDuration.py` & `opengamedata_core-0.0.7/src/ogd/games/PENGUINS/features/MirrorWaddleDuration.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/PENGUINS/features/PenguinInteractCount.py` & `opengamedata_core-0.0.7/src/ogd/games/PENGUINS/features/PenguinInteractCount.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/PENGUINS/features/PlayerInactiveAvgDuration.py` & `opengamedata_core-0.0.7/src/ogd/games/PENGUINS/features/PlayerInactiveAvgDuration.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/PENGUINS/features/RegionDuration.py` & `opengamedata_core-0.0.7/src/ogd/games/PENGUINS/features/RegionDuration.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/PENGUINS/features/RegionEnterCount.py` & `opengamedata_core-0.0.7/src/ogd/games/PENGUINS/features/RegionEnterCount.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/PENGUINS/features/RegionsEncountered.py` & `opengamedata_core-0.0.7/src/ogd/games/PENGUINS/features/RegionsEncountered.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/PENGUINS/features/RingChimesCount.py` & `opengamedata_core-0.0.7/src/ogd/games/PENGUINS/features/RingChimesCount.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/PENGUINS/features/RockBashCount.py` & `opengamedata_core-0.0.7/src/ogd/games/PENGUINS/features/RockBashCount.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/PENGUINS/features/RockMultiplePickupCount.py` & `opengamedata_core-0.0.7/src/ogd/games/PENGUINS/features/RockMultiplePickupCount.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/PENGUINS/features/RockPickupCount.py` & `opengamedata_core-0.0.7/src/ogd/games/PENGUINS/features/RockPickupCount.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/PENGUINS/features/SessionDuration.py` & `opengamedata_core-0.0.7/src/ogd/games/PENGUINS/features/SessionDuration.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/PENGUINS/features/SkuaBashCount.py` & `opengamedata_core-0.0.7/src/ogd/games/PENGUINS/features/SkuaBashCount.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/PENGUINS/features/SkuaPeckCount.py` & `opengamedata_core-0.0.7/src/ogd/games/PENGUINS/features/SkuaPeckCount.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/PENGUINS/features/SnowBallDuration.py` & `opengamedata_core-0.0.7/src/ogd/games/PENGUINS/features/SnowBallDuration.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/PENGUINS/features/WaddleCount.py` & `opengamedata_core-0.0.7/src/ogd/games/PENGUINS/features/WaddleCount.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/PENGUINS/features/WaddlePerRegion.py` & `opengamedata_core-0.0.7/src/ogd/games/PENGUINS/features/WaddlePerRegion.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/PENGUINS/features/__init__.py` & `opengamedata_core-0.0.7/src/ogd/games/PENGUINS/features/__init__.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/PENGUINS/features/bases/PerRegionFeature.py` & `opengamedata_core-0.0.7/src/ogd/games/PENGUINS/features/bases/PerRegionFeature.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/PENGUINS/schemas/PENGUINS.json.template` & `opengamedata_core-0.0.7/src/ogd/games/PENGUINS/schemas/PENGUINS.json.template`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/SHADOWSPECT/ShadowspectLoader.py` & `opengamedata_core-0.0.7/src/ogd/games/SHADOWSPECT/ShadowspectLoader.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/SHADOWSPECT/features/FunnelByUser.py` & `opengamedata_core-0.0.7/src/ogd/games/SHADOWSPECT/features/FunnelByUser.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/SHADOWSPECT/features/LevelsOfDifficulty.py` & `opengamedata_core-0.0.7/src/ogd/games/SHADOWSPECT/features/LevelsOfDifficulty.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/SHADOWSPECT/features/MoveShapeCount.py` & `opengamedata_core-0.0.7/src/ogd/games/SHADOWSPECT/features/MoveShapeCount.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/SHADOWSPECT/features/SequenceBetweenPuzzles.py` & `opengamedata_core-0.0.7/src/ogd/games/SHADOWSPECT/features/SequenceBetweenPuzzles.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/SHADOWSPECT/features/SequenceWithinPuzzles.py` & `opengamedata_core-0.0.7/src/ogd/games/SHADOWSPECT/features/SequenceWithinPuzzles.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/SHADOWSPECT/features/SessionID.py` & `opengamedata_core-0.0.7/src/ogd/games/SHADOWSPECT/features/SessionID.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/SHADOWSPECT/schemas/SHADOWSPECT.json.template` & `opengamedata_core-0.0.7/src/ogd/games/SHADOWSPECT/schemas/SHADOWSPECT.json.template`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/SHIPWRECKS/ShipwrecksLoader.py` & `opengamedata_core-0.0.7/src/ogd/games/SHIPWRECKS/ShipwrecksLoader.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/SHIPWRECKS/features/ActiveJobs.py` & `opengamedata_core-0.0.7/src/ogd/games/SHIPWRECKS/features/ActiveJobs.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/SHIPWRECKS/features/EventList.py` & `opengamedata_core-0.0.7/src/ogd/games/SHIPWRECKS/features/EventList.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/SHIPWRECKS/features/EvidenceBoardCompleteCount.py` & `opengamedata_core-0.0.7/src/ogd/games/SHIPWRECKS/features/EvidenceBoardCompleteCount.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/SHIPWRECKS/features/JobsAttempted.py` & `opengamedata_core-0.0.7/src/ogd/games/SHIPWRECKS/features/JobsAttempted.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/SHIPWRECKS/features/JobsCompleted.py` & `opengamedata_core-0.0.7/src/ogd/games/SHIPWRECKS/features/JobsCompleted.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/SHIPWRECKS/features/MissionDiveTime.py` & `opengamedata_core-0.0.7/src/ogd/games/SHIPWRECKS/features/MissionDiveTime.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/SHIPWRECKS/features/MissionSonarTimeToComplete.py` & `opengamedata_core-0.0.7/src/ogd/games/SHIPWRECKS/features/MissionSonarTimeToComplete.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/SHIPWRECKS/features/PlayerSummary.py` & `opengamedata_core-0.0.7/src/ogd/games/SHIPWRECKS/features/PlayerSummary.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/SHIPWRECKS/features/PopulationSummary.py` & `opengamedata_core-0.0.7/src/ogd/games/SHIPWRECKS/features/PopulationSummary.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/SHIPWRECKS/features/SessionDuration.py` & `opengamedata_core-0.0.7/src/ogd/games/SHIPWRECKS/features/SessionDuration.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/SHIPWRECKS/features/SessionID.py` & `opengamedata_core-0.0.7/src/ogd/games/SHIPWRECKS/features/SessionID.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/SHIPWRECKS/features/TopJobCompletionDestinations.py` & `opengamedata_core-0.0.7/src/ogd/games/SHIPWRECKS/features/TopJobCompletionDestinations.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/SHIPWRECKS/features/TopJobSwitchDestinations.py` & `opengamedata_core-0.0.7/src/ogd/games/SHIPWRECKS/features/TopJobSwitchDestinations.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/SHIPWRECKS/features/TotalDiveTime.py` & `opengamedata_core-0.0.7/src/ogd/games/SHIPWRECKS/features/TotalDiveTime.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/SHIPWRECKS/features/__init__.py` & `opengamedata_core-0.0.7/src/ogd/games/SHIPWRECKS/features/__init__.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/SHIPWRECKS/schemas/SHIPWRECKS.json.template` & `opengamedata_core-0.0.7/src/ogd/games/SHIPWRECKS/schemas/SHIPWRECKS.json.template`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/THERMOVR/ThermoVRLoader.py` & `opengamedata_core-0.0.7/src/ogd/games/THERMOVR/ThermoVRLoader.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/THERMOVR/features/LeftHandMoves.py` & `opengamedata_core-0.0.7/src/ogd/games/THERMOVR/features/LeftHandMoves.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/THERMOVR/features/PhasesReached.py` & `opengamedata_core-0.0.7/src/ogd/games/THERMOVR/features/PhasesReached.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/THERMOVR/features/PlayMode.py` & `opengamedata_core-0.0.7/src/ogd/games/THERMOVR/features/PlayMode.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/THERMOVR/features/RightHandMoves.py` & `opengamedata_core-0.0.7/src/ogd/games/THERMOVR/features/RightHandMoves.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/THERMOVR/features/TaskCompleteCount.py` & `opengamedata_core-0.0.7/src/ogd/games/THERMOVR/features/TaskCompleteCount.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/THERMOVR/features/ToolNudgeCount.py` & `opengamedata_core-0.0.7/src/ogd/games/THERMOVR/features/ToolNudgeCount.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/THERMOVR/features/ToolSliderTime.py` & `opengamedata_core-0.0.7/src/ogd/games/THERMOVR/features/ToolSliderTime.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/THERMOVR/schemas/THERMOVR.json.template` & `opengamedata_core-0.0.7/src/ogd/games/THERMOVR/schemas/THERMOVR.json.template`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/TRANSFORMATION_QUEST/DBExport.json` & `opengamedata_core-0.0.7/src/ogd/games/TRANSFORMATION_QUEST/DBExport.json`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/TRANSFORMATION_QUEST/schemas/TRANSFORMATION_QUEST.json.template` & `opengamedata_core-0.0.7/src/ogd/games/TRANSFORMATION_QUEST/schemas/TRANSFORMATION_QUEST.json.template`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/WAVES/WaveLoader.py` & `opengamedata_core-0.0.7/src/ogd/games/WAVES/WaveLoader.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/WAVES/features/AmplitudeGoodMoveCount.py` & `opengamedata_core-0.0.7/src/ogd/games/WAVES/features/AmplitudeGoodMoveCount.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/WAVES/features/AverageFails.py` & `opengamedata_core-0.0.7/src/ogd/games/WAVES/features/AverageFails.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/WAVES/features/AverageLevelTime.py` & `opengamedata_core-0.0.7/src/ogd/games/WAVES/features/AverageLevelTime.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/WAVES/features/AverageMoveTypeChanges.py` & `opengamedata_core-0.0.7/src/ogd/games/WAVES/features/AverageMoveTypeChanges.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/WAVES/features/AverageSliderMoves.py` & `opengamedata_core-0.0.7/src/ogd/games/WAVES/features/AverageSliderMoves.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/WAVES/features/BeginCount.py` & `opengamedata_core-0.0.7/src/ogd/games/WAVES/features/BeginCount.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/WAVES/features/ClosenessIntercept.py` & `opengamedata_core-0.0.7/src/ogd/games/WAVES/features/ClosenessIntercept.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/WAVES/features/ClosenessR2.py` & `opengamedata_core-0.0.7/src/ogd/games/WAVES/features/ClosenessR2.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/WAVES/features/ClosenessSlope.py` & `opengamedata_core-0.0.7/src/ogd/games/WAVES/features/ClosenessSlope.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/WAVES/features/Completed.py` & `opengamedata_core-0.0.7/src/ogd/games/WAVES/features/Completed.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/WAVES/features/FirstMoveType.py` & `opengamedata_core-0.0.7/src/ogd/games/WAVES/features/FirstMoveType.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/WAVES/features/MenuButtonCount.py` & `opengamedata_core-0.0.7/src/ogd/games/WAVES/features/MenuButtonCount.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/WAVES/features/OffsetGoodMoveCount.py` & `opengamedata_core-0.0.7/src/ogd/games/WAVES/features/OffsetGoodMoveCount.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/WAVES/features/OverallPercentAmplitudeMoves.py` & `opengamedata_core-0.0.7/src/ogd/games/WAVES/features/OverallPercentAmplitudeMoves.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/WAVES/features/OverallPercentOffsetMoves.py` & `opengamedata_core-0.0.7/src/ogd/games/WAVES/features/OverallPercentOffsetMoves.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/WAVES/features/OverallPercentWavelengthMoves.py` & `opengamedata_core-0.0.7/src/ogd/games/WAVES/features/OverallPercentWavelengthMoves.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/WAVES/features/OverallSliderAverageRange.py` & `opengamedata_core-0.0.7/src/ogd/games/WAVES/features/OverallSliderAverageRange.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/WAVES/features/OverallSliderAverageStandardDeviations.py` & `opengamedata_core-0.0.7/src/ogd/games/WAVES/features/OverallSliderAverageStandardDeviations.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/WAVES/features/PercentAmplitudeGoodMoves.py` & `opengamedata_core-0.0.7/src/ogd/games/WAVES/features/PercentAmplitudeGoodMoves.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/WAVES/features/PercentAmplitudeMoves.py` & `opengamedata_core-0.0.7/src/ogd/games/WAVES/features/PercentAmplitudeMoves.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/WAVES/features/PercentOffsetGoodMoves.py` & `opengamedata_core-0.0.7/src/ogd/games/WAVES/features/PercentOffsetGoodMoves.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/WAVES/features/PercentOffsetMoves.py` & `opengamedata_core-0.0.7/src/ogd/games/WAVES/features/PercentOffsetMoves.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/WAVES/features/PercentWavelengthGoodMoves.py` & `opengamedata_core-0.0.7/src/ogd/games/WAVES/features/PercentWavelengthGoodMoves.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/WAVES/features/PercentWavelengthMoves.py` & `opengamedata_core-0.0.7/src/ogd/games/WAVES/features/PercentWavelengthMoves.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/WAVES/features/PersistentSessionID.py` & `opengamedata_core-0.0.7/src/ogd/games/WAVES/features/PersistentSessionID.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/WAVES/features/QuestionAnswered.py` & `opengamedata_core-0.0.7/src/ogd/games/WAVES/features/QuestionAnswered.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/WAVES/features/QuestionCorrect.py` & `opengamedata_core-0.0.7/src/ogd/games/WAVES/features/QuestionCorrect.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/WAVES/features/RangeIntercept.py` & `opengamedata_core-0.0.7/src/ogd/games/WAVES/features/RangeIntercept.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/WAVES/features/RangeR2.py` & `opengamedata_core-0.0.7/src/ogd/games/WAVES/features/RangeR2.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/WAVES/features/RangeSlope.py` & `opengamedata_core-0.0.7/src/ogd/games/WAVES/features/RangeSlope.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/WAVES/features/SequenceLevel.py` & `opengamedata_core-0.0.7/src/ogd/games/WAVES/features/SequenceLevel.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/WAVES/features/SessionID.py` & `opengamedata_core-0.0.7/src/ogd/games/WAVES/features/SessionID.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/WAVES/features/SliderAverageRange.py` & `opengamedata_core-0.0.7/src/ogd/games/WAVES/features/SliderAverageRange.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/WAVES/features/SliderAverageStandardDeviations.py` & `opengamedata_core-0.0.7/src/ogd/games/WAVES/features/SliderAverageStandardDeviations.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/WAVES/features/SucceedCount.py` & `opengamedata_core-0.0.7/src/ogd/games/WAVES/features/SucceedCount.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/WAVES/features/TimeToAnswerMS.py` & `opengamedata_core-0.0.7/src/ogd/games/WAVES/features/TimeToAnswerMS.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/WAVES/features/TotalArrowMoves.py` & `opengamedata_core-0.0.7/src/ogd/games/WAVES/features/TotalArrowMoves.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/WAVES/features/TotalFails.py` & `opengamedata_core-0.0.7/src/ogd/games/WAVES/features/TotalFails.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/WAVES/features/TotalLevelTime.py` & `opengamedata_core-0.0.7/src/ogd/games/WAVES/features/TotalLevelTime.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/WAVES/features/TotalMoveTypeChanges.py` & `opengamedata_core-0.0.7/src/ogd/games/WAVES/features/TotalMoveTypeChanges.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/WAVES/features/TotalResets.py` & `opengamedata_core-0.0.7/src/ogd/games/WAVES/features/TotalResets.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/WAVES/features/TotalSkips.py` & `opengamedata_core-0.0.7/src/ogd/games/WAVES/features/TotalSkips.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/WAVES/features/TotalSliderMoves.py` & `opengamedata_core-0.0.7/src/ogd/games/WAVES/features/TotalSliderMoves.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/WAVES/features/WavelengthGoodMoveCount.py` & `opengamedata_core-0.0.7/src/ogd/games/WAVES/features/WavelengthGoodMoveCount.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/WAVES/features/__init__.py` & `opengamedata_core-0.0.7/src/ogd/games/WAVES/features/__init__.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/WAVES/schemas/WAVES.json.template` & `opengamedata_core-0.0.7/src/ogd/games/WAVES/schemas/WAVES.json.template`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/ogd/games/WEATHER_STATION/schemas/WEATHER_STATION.json.template` & `opengamedata_core-0.0.7/src/ogd/games/WEATHER_STATION/schemas/WEATHER_STATION.json.template`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/src/opengamedata_core.egg-info/PKG-INFO` & `opengamedata_core-0.0.7/src/opengamedata_core.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opengamedata-core
-Version: 0.0.6
+Version: 0.0.7
 Summary: A package for retrieving and processing event-based video game data. Additional authors: Nick Spevacek, Renee Li, John McCloskey, Zach Studdiford, Glenn Palmer, Haishuo Chen, Daus, Ameya Kshirsagar, Yunqing Xiao, Erik Harpstead, Manuel Jesus Gomez Moratilla
 Author-email: Luke Swanson <superscription58@gmail.com>, David Gagnon <djgagnon@wisc.edu>
 Project-URL: Homepage, https://github.com/opengamedata/opengamedata-core
 Project-URL: Bug Tracker, https://github.com/opengamedata/opengamedata-core/issues
 Project-URL: Documentation, https://opengamedata-doc.readthedocs.io/en/latest/index.html
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `opengamedata_core-0.0.6/src/opengamedata_core.egg-info/SOURCES.txt` & `opengamedata_core-0.0.7/src/opengamedata_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.6/tests/test_lakeland_models.py` & `opengamedata_core-0.0.7/tests/test_lakeland_models.py`

 * *Files identical despite different names*

