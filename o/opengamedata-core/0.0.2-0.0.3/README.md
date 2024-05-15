# Comparing `tmp/opengamedata_core-0.0.2.tar.gz` & `tmp/opengamedata_core-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opengamedata_core-0.0.2.tar", last modified: Mon May  6 17:29:13 2024, max compression
+gzip compressed data, was "opengamedata_core-0.0.3.tar", last modified: Wed May 15 21:05:19 2024, max compression
```

## Comparing `opengamedata_core-0.0.2.tar` & `opengamedata_core-0.0.3.tar`

### file list

```diff
@@ -1,522 +1,547 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:29:13.802339 opengamedata_core-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4796 2024-05-06 17:29:13.802339 opengamedata_core-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3900 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 17:29:13.802339 opengamedata_core-0.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:29:13.726339 opengamedata_core-0.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:29:13.726339 opengamedata_core-0.0.2/src/ogd/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:29:13.726339 opengamedata_core-0.0.2/src/ogd/core/
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:29:13.726339 opengamedata_core-0.0.2/src/ogd/core/exec/
--rw-r--r--   0 runner    (1001) docker     (127)     9329 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/core/exec/Commands.py
--rw-r--r--   0 runner    (1001) docker     (127)     3763 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/core/exec/Generators.py
--rw-r--r--   0 runner    (1001) docker     (127)     4858 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/core/exec/Parsers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:29:13.730339 opengamedata_core-0.0.2/src/ogd/core/generators/
--rw-r--r--   0 runner    (1001) docker     (127)     7753 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/core/generators/Generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     5136 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/core/generators/GeneratorLoader.py
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/core/generators/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:29:13.730339 opengamedata_core-0.0.2/src/ogd/core/generators/detectors/
--rw-r--r--   0 runner    (1001) docker     (127)     4351 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/core/generators/detectors/Detector.py
--rw-r--r--   0 runner    (1001) docker     (127)     2300 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/core/generators/detectors/DetectorEvent.py
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/core/generators/detectors/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:29:13.730339 opengamedata_core-0.0.2/src/ogd/core/generators/extractors/
--rw-r--r--   0 runner    (1001) docker     (127)     6499 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/core/generators/extractors/Extractor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/core/generators/extractors/Feature.py
--rw-r--r--   0 runner    (1001) docker     (127)     1585 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/core/generators/extractors/PerCountFeature.py
--rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/core/generators/extractors/PerLevelFeature.py
--rw-r--r--   0 runner    (1001) docker     (127)      804 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/core/generators/extractors/SessionFeature.py
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/core/generators/extractors/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:29:13.730339 opengamedata_core-0.0.2/src/ogd/core/generators/legacy/
--rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/core/generators/legacy/LegacyDetector.py
--rw-r--r--   0 runner    (1001) docker     (127)    14632 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/core/generators/legacy/LegacyFeature.py
--rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/core/generators/legacy/LegacyLoader.py
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/core/generators/legacy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:29:13.730339 opengamedata_core-0.0.2/src/ogd/core/generators/registries/
--rw-r--r--   0 runner    (1001) docker     (127)     8364 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/core/generators/registries/DetectorRegistry.py
--rw-r--r--   0 runner    (1001) docker     (127)    13575 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/core/generators/registries/ExtractorRegistry.py
--rw-r--r--   0 runner    (1001) docker     (127)     5276 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/core/generators/registries/GeneratorRegistry.py
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/core/generators/registries/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:29:13.734340 opengamedata_core-0.0.2/src/ogd/core/interfaces/
--rw-r--r--   0 runner    (1001) docker     (127)    10850 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/core/interfaces/BQFirebaseInterface.py
--rw-r--r--   0 runner    (1001) docker     (127)     9699 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/core/interfaces/BigQueryCodingInterface.py
--rw-r--r--   0 runner    (1001) docker     (127)    11865 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/core/interfaces/BigQueryInterface.py
--rw-r--r--   0 runner    (1001) docker     (127)     4903 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/core/interfaces/CSVInterface.py
--rw-r--r--   0 runner    (1001) docker     (127)     3519 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/core/interfaces/CodingInterface.py
--rw-r--r--   0 runner    (1001) docker     (127)     5432 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/core/interfaces/DataInterface.py
--rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/core/interfaces/Interface.py
--rw-r--r--   0 runner    (1001) docker     (127)    23918 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/core/interfaces/MySQLInterface.py
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/core/interfaces/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:29:13.734340 opengamedata_core-0.0.2/src/ogd/core/interfaces/outerfaces/
--rw-r--r--   0 runner    (1001) docker     (127)     5824 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/core/interfaces/outerfaces/DataOuterface.py
--rw-r--r--   0 runner    (1001) docker     (127)     4195 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/core/interfaces/outerfaces/DebugOuterface.py
--rw-r--r--   0 runner    (1001) docker     (127)     4902 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/core/interfaces/outerfaces/DictionaryOuterface.py
--rw-r--r--   0 runner    (1001) docker     (127)    33757 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/core/interfaces/outerfaces/TSVOuterface.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:29:13.734340 opengamedata_core-0.0.2/src/ogd/core/managers/
--rw-r--r--   0 runner    (1001) docker     (127)     3513 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/core/managers/EventManager.py
--rw-r--r--   0 runner    (1001) docker     (127)    18830 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/core/managers/ExportManager.py
--rw-r--r--   0 runner    (1001) docker     (127)    12108 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/core/managers/FeatureManager.py
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/core/managers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:29:13.734340 opengamedata_core-0.0.2/src/ogd/core/processors/
--rw-r--r--   0 runner    (1001) docker     (127)     6040 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/core/processors/ClassroomDetector.py
--rw-r--r--   0 runner    (1001) docker     (127)     2239 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/core/processors/DetectorProcessor.py
--rw-r--r--   0 runner    (1001) docker     (127)      964 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/core/processors/EventProcessor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/core/processors/ExtractorProcessor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2628 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/core/processors/GeneratorProcessor.py
--rw-r--r--   0 runner    (1001) docker     (127)     4602 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/core/processors/PlayerProcessor.py
--rw-r--r--   0 runner    (1001) docker     (127)     4215 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/core/processors/PopulationProcessor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1878 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/core/processors/Processor.py
--rw-r--r--   0 runner    (1001) docker     (127)     4267 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/core/processors/SessionProcessor.py
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/core/processors/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:29:13.738340 opengamedata_core-0.0.2/src/ogd/core/requests/
--rw-r--r--   0 runner    (1001) docker     (127)     5301 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/core/requests/Request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2062 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/core/requests/RequestResult.py
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/core/requests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:29:13.738340 opengamedata_core-0.0.2/src/ogd/core/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)    14401 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/core/schemas/Event.py
--rw-r--r--   0 runner    (1001) docker     (127)      213 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/core/schemas/ExportMode.py
--rw-r--r--   0 runner    (1001) docker     (127)      364 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/core/schemas/ExtractionMode.py
--rw-r--r--   0 runner    (1001) docker     (127)     1426 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/core/schemas/FeatureData.py
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/core/schemas/IDMode.py
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/core/schemas/IterationMode.py
--rw-r--r--   0 runner    (1001) docker     (127)     1427 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/core/schemas/Schema.py
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/core/schemas/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:29:13.738340 opengamedata_core-0.0.2/src/ogd/core/schemas/configs/
--rw-r--r--   0 runner    (1001) docker     (127)    10898 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/core/schemas/configs/ConfigSchema.py
--rw-r--r--   0 runner    (1001) docker     (127)     5835 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/core/schemas/configs/GameSourceSchema.py
--rw-r--r--   0 runner    (1001) docker     (127)     3452 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/core/schemas/configs/IndexingSchema.py
--rw-r--r--   0 runner    (1001) docker     (127)     2593 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/core/schemas/configs/LegacyConfigSchema.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:29:13.738340 opengamedata_core-0.0.2/src/ogd/core/schemas/configs/data_sources/
--rw-r--r--   0 runner    (1001) docker     (127)     3048 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/core/schemas/configs/data_sources/BigQuerySourceSchema.py
--rw-r--r--   0 runner    (1001) docker     (127)     1806 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/core/schemas/configs/data_sources/DataSourceSchema.py
--rw-r--r--   0 runner    (1001) docker     (127)      577 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/core/schemas/configs/data_sources/FileSourceSchema.py
--rw-r--r--   0 runner    (1001) docker     (127)    10140 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/core/schemas/configs/data_sources/MySQLSourceSchema.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:29:13.742339 opengamedata_core-0.0.2/src/ogd/core/schemas/games/
--rw-r--r--   0 runner    (1001) docker     (127)      922 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/core/schemas/games/AggregateSchema.py
--rw-r--r--   0 runner    (1001) docker     (127)     5168 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/core/schemas/games/DataElementSchema.py
--rw-r--r--   0 runner    (1001) docker     (127)     5045 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/core/schemas/games/DetectorMapSchema.py
--rw-r--r--   0 runner    (1001) docker     (127)      801 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/core/schemas/games/DetectorSchema.py
--rw-r--r--   0 runner    (1001) docker     (127)     3996 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/core/schemas/games/EventSchema.py
--rw-r--r--   0 runner    (1001) docker     (127)     4006 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/core/schemas/games/ExtractorSchema.py
--rw-r--r--   0 runner    (1001) docker     (127)     5656 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/core/schemas/games/FeatureMapSchema.py
--rw-r--r--   0 runner    (1001) docker     (127)     4869 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/core/schemas/games/FeatureSchema.py
--rw-r--r--   0 runner    (1001) docker     (127)    26726 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/core/schemas/games/GameSchema.py
--rw-r--r--   0 runner    (1001) docker     (127)     2652 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/core/schemas/games/GameStateSchema.py
--rw-r--r--   0 runner    (1001) docker     (127)     2831 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/core/schemas/games/PerCountSchema.py
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/core/schemas/games/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:29:13.742339 opengamedata_core-0.0.2/src/ogd/core/schemas/table_schemas/
--rw-r--r--   0 runner    (1001) docker     (127)     3615 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/core/schemas/table_schemas/BIGQUERY.json
--rw-r--r--   0 runner    (1001) docker     (127)     4890 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/core/schemas/table_schemas/FIELDDAY_MYSQL.json
--rw-r--r--   0 runner    (1001) docker     (127)     2572 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/core/schemas/table_schemas/FIREBASE.json
--rw-r--r--   0 runner    (1001) docker     (127)     4430 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/core/schemas/table_schemas/MASHOPOLIS_MYSQL.json
--rw-r--r--   0 runner    (1001) docker     (127)     3685 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/core/schemas/table_schemas/OGD_EVENT_FILE.json
--rw-r--r--   0 runner    (1001) docker     (127)     4077 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/core/schemas/table_schemas/OPENGAMEDATA_BIGQUERY.json
--rw-r--r--   0 runner    (1001) docker     (127)     4477 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/core/schemas/table_schemas/OPENGAMEDATA_MYSQL.json
--rw-r--r--   0 runner    (1001) docker     (127)     1920 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/core/schemas/table_schemas/SHIPWRECKS.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:29:13.742339 opengamedata_core-0.0.2/src/ogd/core/schemas/tables/
--rw-r--r--   0 runner    (1001) docker     (127)     6782 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/core/schemas/tables/ColumnMapSchema.py
--rw-r--r--   0 runner    (1001) docker     (127)     4174 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/core/schemas/tables/ColumnSchema.py
--rw-r--r--   0 runner    (1001) docker     (127)    23084 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/core/schemas/tables/TableSchema.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:29:13.742339 opengamedata_core-0.0.2/src/ogd/core/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     4567 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/core/utils/Logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     4361 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/core/utils/Readme.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/core/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/core/utils/typing.py
--rw-r--r--   0 runner    (1001) docker     (127)     2692 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/core/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:29:13.742339 opengamedata_core-0.0.2/src/ogd/games/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:29:13.718340 opengamedata_core-0.0.2/src/ogd/games/ALL_YOU_CAN_ET/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:29:13.746339 opengamedata_core-0.0.2/src/ogd/games/ALL_YOU_CAN_ET/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)    20816 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/ALL_YOU_CAN_ET/schemas/ALL_YOU_CAN_ET.json.template
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:29:13.746339 opengamedata_core-0.0.2/src/ogd/games/AQUALAB/
--rw-r--r--   0 runner    (1001) docker     (127)    12275 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/AQUALAB/AqualabLoader.py
--rw-r--r--   0 runner    (1001) docker     (127)   278275 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/AQUALAB/DBExport.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/AQUALAB/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:29:13.746339 opengamedata_core-0.0.2/src/ogd/games/AQUALAB/detectors/
--rw-r--r--   0 runner    (1001) docker     (127)     2320 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/AQUALAB/detectors/CollectFactNoJob.py
--rw-r--r--   0 runner    (1001) docker     (127)     3554 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/AQUALAB/detectors/DiveSiteNoEvidence.py
--rw-r--r--   0 runner    (1001) docker     (127)     1725 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/AQUALAB/detectors/EchoRoomChange.py
--rw-r--r--   0 runner    (1001) docker     (127)     4505 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/AQUALAB/detectors/HintAndLeave.py
--rw-r--r--   0 runner    (1001) docker     (127)     3466 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/AQUALAB/detectors/Idle.py
--rw-r--r--   0 runner    (1001) docker     (127)     3901 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/AQUALAB/detectors/SceneChangeFrequently.py
--rw-r--r--   0 runner    (1001) docker     (127)     3796 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/AQUALAB/detectors/TwoHints.py
--rw-r--r--   0 runner    (1001) docker     (127)      361 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/AQUALAB/detectors/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:29:13.754339 opengamedata_core-0.0.2/src/ogd/games/AQUALAB/features/
--rw-r--r--   0 runner    (1001) docker     (127)     2752 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/AQUALAB/features/ActiveJobs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2328 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/AQUALAB/features/ActiveTime.py
--rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/AQUALAB/features/EchoSessionID.py
--rw-r--r--   0 runner    (1001) docker     (127)     5318 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/AQUALAB/features/EventList.py
--rw-r--r--   0 runner    (1001) docker     (127)     9386 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/AQUALAB/features/JobActiveTime.py
--rw-r--r--   0 runner    (1001) docker     (127)     2205 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/AQUALAB/features/JobArgumentationTime.py
--rw-r--r--   0 runner    (1001) docker     (127)     2708 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/AQUALAB/features/JobCompletionTime.py
--rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/AQUALAB/features/JobDiveSitesCount.py
--rw-r--r--   0 runner    (1001) docker     (127)     2138 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/AQUALAB/features/JobDiveTime.py
--rw-r--r--   0 runner    (1001) docker     (127)     2203 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/AQUALAB/features/JobExperimentationTime.py
--rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/AQUALAB/features/JobGuideCount.py
--rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/AQUALAB/features/JobHelpCount.py
--rw-r--r--   0 runner    (1001) docker     (127)     3952 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/AQUALAB/features/JobLocationChanges.py
--rw-r--r--   0 runner    (1001) docker     (127)     2076 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/AQUALAB/features/JobModelingTime.py
--rw-r--r--   0 runner    (1001) docker     (127)     2344 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/AQUALAB/features/JobPlayTime.py
--rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/AQUALAB/features/JobStartCount.py
--rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/AQUALAB/features/JobTasksCompleted.py
--rw-r--r--   0 runner    (1001) docker     (127)     1600 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/AQUALAB/features/JobTriesInArgument.py
--rw-r--r--   0 runner    (1001) docker     (127)     6192 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/AQUALAB/features/JobsAttempted.py
--rw-r--r--   0 runner    (1001) docker     (127)     1261 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/AQUALAB/features/JobsCompleted.py
--rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/AQUALAB/features/ModelExportCount.py
--rw-r--r--   0 runner    (1001) docker     (127)     1299 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/AQUALAB/features/ModelInterveneCount.py
--rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/AQUALAB/features/ModelPredictCount.py
--rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/AQUALAB/features/PerJobFeature.py
--rw-r--r--   0 runner    (1001) docker     (127)     3014 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/AQUALAB/features/PlayerSummary.py
--rw-r--r--   0 runner    (1001) docker     (127)     3351 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/AQUALAB/features/PopulationSummary.py
--rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/AQUALAB/features/SessionDiveSitesCount.py
--rw-r--r--   0 runner    (1001) docker     (127)     3020 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/AQUALAB/features/SessionDuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/AQUALAB/features/SessionGuideCount.py
--rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/AQUALAB/features/SessionHelpCount.py
--rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/AQUALAB/features/SessionID.py
--rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/AQUALAB/features/SessionJobsCompleted.py
--rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/AQUALAB/features/SwitchJobsCount.py
--rw-r--r--   0 runner    (1001) docker     (127)     2521 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/AQUALAB/features/SyncCompletionTime.py
--rw-r--r--   0 runner    (1001) docker     (127)     1733 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/AQUALAB/features/TankRulesCount.py
--rw-r--r--   0 runner    (1001) docker     (127)     3458 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/AQUALAB/features/TopJobCompletionDestinations.py
--rw-r--r--   0 runner    (1001) docker     (127)     3444 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/AQUALAB/features/TopJobSwitchDestinations.py
--rw-r--r--   0 runner    (1001) docker     (127)     1852 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/AQUALAB/features/TotalArgumentationTime.py
--rw-r--r--   0 runner    (1001) docker     (127)     1829 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/AQUALAB/features/TotalDiveTime.py
--rw-r--r--   0 runner    (1001) docker     (127)     1894 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/AQUALAB/features/TotalExperimentationTime.py
--rw-r--r--   0 runner    (1001) docker     (127)     1440 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/AQUALAB/features/UserAvgActiveTime.py
--rw-r--r--   0 runner    (1001) docker     (127)     1412 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/AQUALAB/features/UserAvgSessionDuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/AQUALAB/features/UserTotalSessionDuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     2307 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/AQUALAB/features/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:29:13.754339 opengamedata_core-0.0.2/src/ogd/games/AQUALAB/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)    29283 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/AQUALAB/schemas/AQUALAB.json.template
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:29:13.718340 opengamedata_core-0.0.2/src/ogd/games/BACTERIA/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:29:13.754339 opengamedata_core-0.0.2/src/ogd/games/BACTERIA/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/BACTERIA/schemas/BACTERIA.json.template
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:29:13.718340 opengamedata_core-0.0.2/src/ogd/games/BALLOON/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:29:13.754339 opengamedata_core-0.0.2/src/ogd/games/BALLOON/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/BALLOON/schemas/BALLOON.json.template
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:29:13.718340 opengamedata_core-0.0.2/src/ogd/games/BLOOM/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:29:13.754339 opengamedata_core-0.0.2/src/ogd/games/BLOOM/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)    20765 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/BLOOM/schemas/BLOOM.json.template
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:29:13.718340 opengamedata_core-0.0.2/src/ogd/games/CENSIO_SLIDE/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:29:13.754339 opengamedata_core-0.0.2/src/ogd/games/CENSIO_SLIDE/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)    11446 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/CENSIO_SLIDE/schemas/CENSIO_SLIDE.json.template
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:29:13.718340 opengamedata_core-0.0.2/src/ogd/games/CENSIO_STACK/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:29:13.754339 opengamedata_core-0.0.2/src/ogd/games/CENSIO_STACK/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)    21742 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/CENSIO_STACK/schemas/CENSIO_STACK.json.template
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:29:13.722339 opengamedata_core-0.0.2/src/ogd/games/CRUSH_STATION/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:29:13.754339 opengamedata_core-0.0.2/src/ogd/games/CRUSH_STATION/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)    11756 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/CRUSH_STATION/schemas/CRUSH_STATION.json.template
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:29:13.754339 opengamedata_core-0.0.2/src/ogd/games/CRYSTAL/
--rw-r--r--   0 runner    (1001) docker     (127)     2380 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/CRYSTAL/CrystalLoader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:29:13.754339 opengamedata_core-0.0.2/src/ogd/games/CRYSTAL/features/
--rw-r--r--   0 runner    (1001) docker     (127)    14123 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/CRYSTAL/features/CrystalExtractor.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/CRYSTAL/features/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:29:13.754339 opengamedata_core-0.0.2/src/ogd/games/CRYSTAL/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)    14066 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/CRYSTAL/schemas/CRYSTAL.json.template
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:29:13.722339 opengamedata_core-0.0.2/src/ogd/games/CYCLE_CARBON/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:29:13.754339 opengamedata_core-0.0.2/src/ogd/games/CYCLE_CARBON/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/CYCLE_CARBON/schemas/CYCLE_CARBON.json.template
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:29:13.722339 opengamedata_core-0.0.2/src/ogd/games/CYCLE_NITROGEN/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:29:13.758339 opengamedata_core-0.0.2/src/ogd/games/CYCLE_NITROGEN/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/CYCLE_NITROGEN/schemas/CYCLE_NITROGEN.json.template
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:29:13.722339 opengamedata_core-0.0.2/src/ogd/games/CYCLE_WATER/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:29:13.758339 opengamedata_core-0.0.2/src/ogd/games/CYCLE_WATER/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/CYCLE_WATER/schemas/CYCLE_WATER.json.template
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:29:13.722339 opengamedata_core-0.0.2/src/ogd/games/EARTHQUAKE/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:29:13.758339 opengamedata_core-0.0.2/src/ogd/games/EARTHQUAKE/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/EARTHQUAKE/schemas/EARTHQUAKE.json.template
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:29:13.722339 opengamedata_core-0.0.2/src/ogd/games/GWAKKAMOLE/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:29:13.758339 opengamedata_core-0.0.2/src/ogd/games/GWAKKAMOLE/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)    12879 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/GWAKKAMOLE/schemas/GWAKKAMOLE.json.template
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:29:13.758339 opengamedata_core-0.0.2/src/ogd/games/ICECUBE/
--rw-r--r--   0 runner    (1001) docker     (127)     1883 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/ICECUBE/DBExport.json
--rw-r--r--   0 runner    (1001) docker     (127)      803 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/ICECUBE/DBExport.py
--rw-r--r--   0 runner    (1001) docker     (127)     4855 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/ICECUBE/IcecubeLoader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:29:13.758339 opengamedata_core-0.0.2/src/ogd/games/ICECUBE/features/
--rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/ICECUBE/features/HeadsetOnCount.py
--rw-r--r--   0 runner    (1001) docker     (127)     1891 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/ICECUBE/features/ObjectSelectionsDuringVoiceover.py
--rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/ICECUBE/features/PerSceneFeature.py
--rw-r--r--   0 runner    (1001) docker     (127)     2890 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/ICECUBE/features/SceneDuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1941 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/ICECUBE/features/SceneFailureCount.py
--rw-r--r--   0 runner    (1001) docker     (127)     2720 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/ICECUBE/features/SceneFailures.py
--rw-r--r--   0 runner    (1001) docker     (127)     1380 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/ICECUBE/features/ScenesEncountered.py
--rw-r--r--   0 runner    (1001) docker     (127)     3466 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/ICECUBE/features/SessionDuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/ICECUBE/features/Session_Language.py
--rw-r--r--   0 runner    (1001) docker     (127)     2389 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/ICECUBE/features/TaskTimeToComplete.py
--rw-r--r--   0 runner    (1001) docker     (127)     1780 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/ICECUBE/features/ViewportCountPerScene.py
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/ICECUBE/features/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:29:13.758339 opengamedata_core-0.0.2/src/ogd/games/ICECUBE/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)     7292 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/ICECUBE/schemas/ICECUBE.json.template
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:29:13.758339 opengamedata_core-0.0.2/src/ogd/games/JOURNALISM/
--rw-r--r--   0 runner    (1001) docker     (127)     7717 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/JOURNALISM/JournalismLoader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:29:13.766339 opengamedata_core-0.0.2/src/ogd/games/JOURNALISM/features/
--rw-r--r--   0 runner    (1001) docker     (127)     4546 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/JOURNALISM/features/AttributeView.py
--rw-r--r--   0 runner    (1001) docker     (127)     4973 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/JOURNALISM/features/ChoiceClickCount.py
--rw-r--r--   0 runner    (1001) docker     (127)     2234 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/JOURNALISM/features/ContinuesOnFail.py
--rw-r--r--   0 runner    (1001) docker     (127)     4549 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/JOURNALISM/features/EditorNoteOpen.py
--rw-r--r--   0 runner    (1001) docker     (127)     4994 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/JOURNALISM/features/FailureCount.py
--rw-r--r--   0 runner    (1001) docker     (127)     3968 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/JOURNALISM/features/GameComplete.py
--rw-r--r--   0 runner    (1001) docker     (127)     4859 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/JOURNALISM/features/LevelCompleteCount.py
--rw-r--r--   0 runner    (1001) docker     (127)     4866 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/JOURNALISM/features/LevelCompleted.py
--rw-r--r--   0 runner    (1001) docker     (127)     2824 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/JOURNALISM/features/LevelTime.py
--rw-r--r--   0 runner    (1001) docker     (127)     2340 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/JOURNALISM/features/MaxedPlayerAttribute.py
--rw-r--r--   0 runner    (1001) docker     (127)     5255 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/JOURNALISM/features/MeanSnippetTime.py
--rw-r--r--   0 runner    (1001) docker     (127)     4437 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/JOURNALISM/features/PlayTime.py
--rw-r--r--   0 runner    (1001) docker     (127)     4384 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/JOURNALISM/features/PlayerAttributes.py
--rw-r--r--   0 runner    (1001) docker     (127)     4468 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/JOURNALISM/features/QuitLevel.py
--rw-r--r--   0 runner    (1001) docker     (127)     4142 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/JOURNALISM/features/QuitNode.py
--rw-r--r--   0 runner    (1001) docker     (127)     7634 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/JOURNALISM/features/QuitType.py
--rw-r--r--   0 runner    (1001) docker     (127)     6945 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/JOURNALISM/features/QuitTypePerLevel.py
--rw-r--r--   0 runner    (1001) docker     (127)     5902 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/JOURNALISM/features/SessionPlayTime.py
--rw-r--r--   0 runner    (1001) docker     (127)     5049 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/JOURNALISM/features/SkillSequenceCount.py
--rw-r--r--   0 runner    (1001) docker     (127)     4786 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/JOURNALISM/features/SnippetReceivedCount.py
--rw-r--r--   0 runner    (1001) docker     (127)     5004 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/JOURNALISM/features/SnippetReplace.py
--rw-r--r--   0 runner    (1001) docker     (127)     1542 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/JOURNALISM/features/SnippetsCollected.py
--rw-r--r--   0 runner    (1001) docker     (127)     1772 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/JOURNALISM/features/SnippetsSubmitted.py
--rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/JOURNALISM/features/StoryAlignment.py
--rw-r--r--   0 runner    (1001) docker     (127)     2217 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/JOURNALISM/features/StoryAlignmentSequence.py
--rw-r--r--   0 runner    (1001) docker     (127)     5473 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/JOURNALISM/features/StoryCompleteTime.py
--rw-r--r--   0 runner    (1001) docker     (127)     6576 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/JOURNALISM/features/StoryEditorTime.py
--rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/JOURNALISM/features/StoryScore.py
--rw-r--r--   0 runner    (1001) docker     (127)     2190 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/JOURNALISM/features/StoryScoreSequence.py
--rw-r--r--   0 runner    (1001) docker     (127)     4773 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/JOURNALISM/features/TextClickCount.py
--rw-r--r--   0 runner    (1001) docker     (127)     4720 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/JOURNALISM/features/TopAttribute.py
--rw-r--r--   0 runner    (1001) docker     (127)     2228 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/JOURNALISM/features/TopPlayerAttribute.py
--rw-r--r--   0 runner    (1001) docker     (127)     2272 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/JOURNALISM/features/TopPlayerQuitType.py
--rw-r--r--   0 runner    (1001) docker     (127)     4475 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/JOURNALISM/features/TotalFails.py
--rw-r--r--   0 runner    (1001) docker     (127)     2086 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/JOURNALISM/features/TotalLevelTime.py
--rw-r--r--   0 runner    (1001) docker     (127)     3928 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/JOURNALISM/features/UserPlayTime.py
--rw-r--r--   0 runner    (1001) docker     (127)     4729 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/JOURNALISM/features/WorstAttribute.py
--rw-r--r--   0 runner    (1001) docker     (127)     2242 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/JOURNALISM/features/WorstPlayerAttribute.py
--rw-r--r--   0 runner    (1001) docker     (127)     1938 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/JOURNALISM/features/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:29:13.766339 opengamedata_core-0.0.2/src/ogd/games/JOURNALISM/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)    45415 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/JOURNALISM/schemas/JOURNALISM.json.template
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:29:13.766339 opengamedata_core-0.0.2/src/ogd/games/JOWILDER/
--rw-r--r--   0 runner    (1001) docker     (127)     5206 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/JOWILDER/JowilderLoader.py
--rw-r--r--   0 runner    (1001) docker     (127)    16451 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/JOWILDER/Jowilder_Enumerators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:29:13.770339 opengamedata_core-0.0.2/src/ogd/games/JOWILDER/features/
--rw-r--r--   0 runner    (1001) docker     (127)     3089 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/JOWILDER/features/ActiveStateTime.py
--rw-r--r--   0 runner    (1001) docker     (127)     1838 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/JOWILDER/features/Clicks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1438 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/JOWILDER/features/EventCount.py
--rw-r--r--   0 runner    (1001) docker     (127)     1736 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/JOWILDER/features/FirstInteraction.py
--rw-r--r--   0 runner    (1001) docker     (127)     1822 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/JOWILDER/features/GameScript.py
--rw-r--r--   0 runner    (1001) docker     (127)     1439 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/JOWILDER/features/GameVersion.py
--rw-r--r--   0 runner    (1001) docker     (127)     1359 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/JOWILDER/features/Hovers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2458 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/JOWILDER/features/IdleState.py
--rw-r--r--   0 runner    (1001) docker     (127)     7609 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/JOWILDER/features/Interaction.py
--rw-r--r--   0 runner    (1001) docker     (127)     2338 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/JOWILDER/features/InteractionName.py
--rw-r--r--   0 runner    (1001) docker     (127)     4592 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/JOWILDER/features/InteractionTextBoxesPerSecond.py
--rw-r--r--   0 runner    (1001) docker     (127)     4587 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/JOWILDER/features/InteractionWordsPerSecond.py
--rw-r--r--   0 runner    (1001) docker     (127)     1684 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/JOWILDER/features/LastInteraction.py
--rw-r--r--   0 runner    (1001) docker     (127)     1720 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/JOWILDER/features/MeaningfulActions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2000 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/JOWILDER/features/NotebookUses.py
--rw-r--r--   0 runner    (1001) docker     (127)     3211 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/JOWILDER/features/QuestionAnswers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1770 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/JOWILDER/features/SessionDuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1887 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/JOWILDER/features/SessionStart.py
--rw-r--r--   0 runner    (1001) docker     (127)     5104 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/JOWILDER/features/SurveyItem.py
--rw-r--r--   0 runner    (1001) docker     (127)     2791 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/JOWILDER/features/SurveyTime.py
--rw-r--r--   0 runner    (1001) docker     (127)     1631 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/JOWILDER/features/UsedContinue.py
--rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/JOWILDER/features/UsedSaveCode.py
--rw-r--r--   0 runner    (1001) docker     (127)     2151 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/JOWILDER/features/UserEnabled.py
--rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/JOWILDER/features/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1925 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/JOWILDER/get_jowilder_all_items.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:29:13.770339 opengamedata_core-0.0.2/src/ogd/games/JOWILDER/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)    35912 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/JOWILDER/schemas/JOWILDER.json.template
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:29:13.774339 opengamedata_core-0.0.2/src/ogd/games/LAKELAND/
--rw-r--r--   0 runner    (1001) docker     (127)     2357 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/LAKELAND/LakelandLoader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:29:13.778339 opengamedata_core-0.0.2/src/ogd/games/LAKELAND/features/
--rw-r--r--   0 runner    (1001) docker     (127)     2039 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/LAKELAND/features/ActionsLastXSecondsModel.py
--rw-r--r--   0 runner    (1001) docker     (127)      607 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/LAKELAND/features/DeathCountModel.py
--rw-r--r--   0 runner    (1001) docker     (127)    11750 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/LAKELAND/features/DeathPredModel.py
--rw-r--r--   0 runner    (1001) docker     (127)     8664 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/LAKELAND/features/DeathThresholdModel.py
--rw-r--r--   0 runner    (1001) docker     (127)     4916 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/LAKELAND/features/DiagonalFarmDetectorModel.py
--rw-r--r--   0 runner    (1001) docker     (127)     7995 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/LAKELAND/features/FeatSeqPercent.py
--rw-r--r--   0 runner    (1001) docker     (127)     2294 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/LAKELAND/features/FeatVelocity.py
--rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/LAKELAND/features/FeatureModel.py
--rw-r--r--   0 runner    (1001) docker     (127)     8478 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/LAKELAND/features/LAKELAND_models.json
--rw-r--r--   0 runner    (1001) docker     (127)     4415 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/LAKELAND/features/LakelandEnumerators.json
--rw-r--r--   0 runner    (1001) docker     (127)    69732 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/LAKELAND/features/LakelandExtractor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2639 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/LAKELAND/features/LinearModel.py
--rw-r--r--   0 runner    (1001) docker     (127)     2701 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/LAKELAND/features/LogisticModel.py
--rw-r--r--   0 runner    (1001) docker     (127)     3353 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/LAKELAND/features/MapSummaryModel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/LAKELAND/features/Model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2574 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/LAKELAND/features/MoneyAccumulationModel.py
--rw-r--r--   0 runner    (1001) docker     (127)      444 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/LAKELAND/features/NthEventModel.py
--rw-r--r--   0 runner    (1001) docker     (127)      496 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/LAKELAND/features/PlayingTimeModel.py
--rw-r--r--   0 runner    (1001) docker     (127)     3287 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/LAKELAND/features/PopulationModel.py
--rw-r--r--   0 runner    (1001) docker     (127)     4813 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/LAKELAND/features/RecentPurchasesModel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1264 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/LAKELAND/features/SequenceModel.py
--rw-r--r--   0 runner    (1001) docker     (127)     4909 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/LAKELAND/features/SimpleFarmAbandonmentModel.py
--rw-r--r--   0 runner    (1001) docker     (127)      850 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/LAKELAND/features/SingleFeatureModel.py
--rw-r--r--   0 runner    (1001) docker     (127)     6060 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/LAKELAND/features/TimeSinceEventTypes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/LAKELAND/features/TimeSinceLastSaleModel.py
--rw-r--r--   0 runner    (1001) docker     (127)      507 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/LAKELAND/features/TownCompositionFeatureModel.py
--rw-r--r--   0 runner    (1001) docker     (127)     2026 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/LAKELAND/features/TownCompositionModel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/LAKELAND/features/TutorialProgressionModel.py
--rw-r--r--   0 runner    (1001) docker     (127)    82382 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/LAKELAND/features/WAVES_models.json
--rw-r--r--   0 runner    (1001) docker     (127)    82382 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/LAKELAND/features/WAVES_models_L8_Q0_Q1.json
--rw-r--r--   0 runner    (1001) docker     (127)    49819 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/LAKELAND/features/WAVES_models_L8_and_Q0.json
--rw-r--r--   0 runner    (1001) docker     (127)    28429 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/LAKELAND/features/WAVES_models_L8_complete_and_current.json
--rw-r--r--   0 runner    (1001) docker     (127)    21021 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/LAKELAND/features/WAVES_models_L8_only_complete.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/LAKELAND/features/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2331 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/LAKELAND/produce_lakeland_enumerators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:29:13.778339 opengamedata_core-0.0.2/src/ogd/games/LAKELAND/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)   115553 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/LAKELAND/schemas/LAKELAND.json.template
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:29:13.778339 opengamedata_core-0.0.2/src/ogd/games/MAGNET/
--rw-r--r--   0 runner    (1001) docker     (127)     2346 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/MAGNET/MagnetLoader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:29:13.778339 opengamedata_core-0.0.2/src/ogd/games/MAGNET/features/
--rw-r--r--   0 runner    (1001) docker     (127)     8596 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/MAGNET/features/MagnetExtractor.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/MAGNET/features/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:29:13.778339 opengamedata_core-0.0.2/src/ogd/games/MAGNET/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)     7887 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/MAGNET/schemas/MAGNET.json.template
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:29:13.722339 opengamedata_core-0.0.2/src/ogd/games/MASHOPOLIS/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:29:13.778339 opengamedata_core-0.0.2/src/ogd/games/MASHOPOLIS/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)    10063 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/MASHOPOLIS/schemas/MASHOPOLIS.json.template
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:29:13.782339 opengamedata_core-0.0.2/src/ogd/games/PENGUINS/
--rw-r--r--   0 runner    (1001) docker     (127)     2970 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/PENGUINS/DBExport.json
--rw-r--r--   0 runner    (1001) docker     (127)     7109 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/PENGUINS/PenguinsLoader.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/PENGUINS/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:29:13.782339 opengamedata_core-0.0.2/src/ogd/games/PENGUINS/detectors/
--rw-r--r--   0 runner    (1001) docker     (127)     3747 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/PENGUINS/detectors/RegionEnter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3966 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/PENGUINS/detectors/RegionExit.py
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/PENGUINS/detectors/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:29:13.786339 opengamedata_core-0.0.2/src/ogd/games/PENGUINS/features/
--rw-r--r--   0 runner    (1001) docker     (127)     1691 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/PENGUINS/features/ActivityCompleted.py
--rw-r--r--   0 runner    (1001) docker     (127)     2720 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/PENGUINS/features/ActivityDuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/PENGUINS/features/EatFishCount.py
--rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/PENGUINS/features/EggLostCount.py
--rw-r--r--   0 runner    (1001) docker     (127)     2401 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/PENGUINS/features/EggRecoverTime.py
--rw-r--r--   0 runner    (1001) docker     (127)     1792 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/PENGUINS/features/GazeCount.py
--rw-r--r--   0 runner    (1001) docker     (127)     2663 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/PENGUINS/features/GazeDuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     4361 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/PENGUINS/features/MirrorWaddleDuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1901 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/PENGUINS/features/PerRegionFeature.py
--rw-r--r--   0 runner    (1001) docker     (127)     1232 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/PENGUINS/features/PickupRockCount.py
--rw-r--r--   0 runner    (1001) docker     (127)     2636 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/PENGUINS/features/PlayerInactiveAvgDuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/PENGUINS/features/PlayerWaddleCount.py
--rw-r--r--   0 runner    (1001) docker     (127)     2290 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/PENGUINS/features/RegionDuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/PENGUINS/features/RegionEnterCount.py
--rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/PENGUINS/features/RegionsEncountered.py
--rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/PENGUINS/features/RingChimesCount.py
--rw-r--r--   0 runner    (1001) docker     (127)     3599 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/PENGUINS/features/SessionDuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     2101 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/PENGUINS/features/SnowBallDuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1689 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/PENGUINS/features/WaddlePerRegion.py
--rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/PENGUINS/features/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:29:13.786339 opengamedata_core-0.0.2/src/ogd/games/PENGUINS/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)    24103 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/PENGUINS/schemas/PENGUINS.json.template
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:29:13.786339 opengamedata_core-0.0.2/src/ogd/games/SHADOWSPECT/
--rw-r--r--   0 runner    (1001) docker     (127)     3232 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/SHADOWSPECT/ShadowspectLoader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:29:13.786339 opengamedata_core-0.0.2/src/ogd/games/SHADOWSPECT/features/
--rw-r--r--   0 runner    (1001) docker     (127)     2789 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/SHADOWSPECT/features/FunnelByUser.py
--rw-r--r--   0 runner    (1001) docker     (127)     7671 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/SHADOWSPECT/features/LevelsOfDifficulty.py
--rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/SHADOWSPECT/features/MoveShapeCount.py
--rw-r--r--   0 runner    (1001) docker     (127)     3897 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/SHADOWSPECT/features/SequenceBetweenPuzzles.py
--rw-r--r--   0 runner    (1001) docker     (127)     1050 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/SHADOWSPECT/features/SessionID.py
--rw-r--r--   0 runner    (1001) docker     (127)      279 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/SHADOWSPECT/features/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:29:13.786339 opengamedata_core-0.0.2/src/ogd/games/SHADOWSPECT/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)    29173 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/SHADOWSPECT/schemas/SHADOWSPECT.json.template
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:29:13.786339 opengamedata_core-0.0.2/src/ogd/games/SHIPWRECKS/
--rw-r--r--   0 runner    (1001) docker     (127)     4677 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/SHIPWRECKS/ShipwrecksLoader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:29:13.790339 opengamedata_core-0.0.2/src/ogd/games/SHIPWRECKS/features/
--rw-r--r--   0 runner    (1001) docker     (127)     2164 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/SHIPWRECKS/features/ActiveJobs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2333 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/SHIPWRECKS/features/EventList.py
--rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/SHIPWRECKS/features/EvidenceBoardCompleteCount.py
--rw-r--r--   0 runner    (1001) docker     (127)     3545 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/SHIPWRECKS/features/JobsAttempted.py
--rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/SHIPWRECKS/features/JobsCompleted.py
--rw-r--r--   0 runner    (1001) docker     (127)     1426 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/SHIPWRECKS/features/MissionDiveTime.py
--rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/SHIPWRECKS/features/MissionSonarTimeToComplete.py
--rw-r--r--   0 runner    (1001) docker     (127)     1526 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/SHIPWRECKS/features/PlayerSummary.py
--rw-r--r--   0 runner    (1001) docker     (127)     1945 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/SHIPWRECKS/features/PopulationSummary.py
--rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/SHIPWRECKS/features/SessionDuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/SHIPWRECKS/features/SessionID.py
--rw-r--r--   0 runner    (1001) docker     (127)     2992 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/SHIPWRECKS/features/TopJobCompletionDestinations.py
--rw-r--r--   0 runner    (1001) docker     (127)     2736 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/SHIPWRECKS/features/TopJobSwitchDestinations.py
--rw-r--r--   0 runner    (1001) docker     (127)     1392 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/SHIPWRECKS/features/TotalDiveTime.py
--rw-r--r--   0 runner    (1001) docker     (127)      798 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/SHIPWRECKS/features/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:29:13.790339 opengamedata_core-0.0.2/src/ogd/games/SHIPWRECKS/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)    10509 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/SHIPWRECKS/schemas/SHIPWRECKS.json.template
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:29:13.790339 opengamedata_core-0.0.2/src/ogd/games/THERMOVR/
--rw-r--r--   0 runner    (1001) docker     (127)        3 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/THERMOVR/DBExport.json
--rw-r--r--   0 runner    (1001) docker     (127)     5663 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/THERMOVR/ThermoVRLoader.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/THERMOVR/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:29:13.790339 opengamedata_core-0.0.2/src/ogd/games/THERMOVR/detectors/
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/THERMOVR/detectors/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:29:13.790339 opengamedata_core-0.0.2/src/ogd/games/THERMOVR/features/
--rw-r--r--   0 runner    (1001) docker     (127)      302 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/THERMOVR/features/LabCompleteCount.py
--rw-r--r--   0 runner    (1001) docker     (127)     1888 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/THERMOVR/features/LeftHandMoves.py
--rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/THERMOVR/features/PhasesReached.py
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/THERMOVR/features/PlayMode.py
--rw-r--r--   0 runner    (1001) docker     (127)     1893 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/THERMOVR/features/RightHandMoves.py
--rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/THERMOVR/features/TaskCompleteCount.py
--rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/THERMOVR/features/ToolNudgeCount.py
--rw-r--r--   0 runner    (1001) docker     (127)     1697 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/THERMOVR/features/ToolSliderTime.py
--rw-r--r--   0 runner    (1001) docker     (127)      503 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/THERMOVR/features/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:29:13.790339 opengamedata_core-0.0.2/src/ogd/games/THERMOVR/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)    51378 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/THERMOVR/schemas/THERMOVR.json.template
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:29:13.790339 opengamedata_core-0.0.2/src/ogd/games/TRANSFORMATION_QUEST/
--rw-r--r--   0 runner    (1001) docker     (127)      777 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/TRANSFORMATION_QUEST/DBExport.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:29:13.790339 opengamedata_core-0.0.2/src/ogd/games/TRANSFORMATION_QUEST/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)    25177 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/TRANSFORMATION_QUEST/schemas/TRANSFORMATION_QUEST.json.template
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:29:13.790339 opengamedata_core-0.0.2/src/ogd/games/WAVES/
--rw-r--r--   0 runner    (1001) docker     (127)    37332 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/WAVES/WaveLoader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:29:13.802339 opengamedata_core-0.0.2/src/ogd/games/WAVES/features/
--rw-r--r--   0 runner    (1001) docker     (127)     1708 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/WAVES/features/AmplitudeGoodMoveCount.py
--rw-r--r--   0 runner    (1001) docker     (127)     1423 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/WAVES/features/AverageFails.py
--rw-r--r--   0 runner    (1001) docker     (127)     3487 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/WAVES/features/AverageLevelTime.py
--rw-r--r--   0 runner    (1001) docker     (127)     1874 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/WAVES/features/AverageMoveTypeChanges.py
--rw-r--r--   0 runner    (1001) docker     (127)     1476 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/WAVES/features/AverageSliderMoves.py
--rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/WAVES/features/BeginCount.py
--rw-r--r--   0 runner    (1001) docker     (127)     2012 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/WAVES/features/ClosenessIntercept.py
--rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/WAVES/features/ClosenessR2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/WAVES/features/ClosenessSlope.py
--rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/WAVES/features/Completed.py
--rw-r--r--   0 runner    (1001) docker     (127)     1192 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/WAVES/features/FirstMoveType.py
--rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/WAVES/features/MenuButtonCount.py
--rw-r--r--   0 runner    (1001) docker     (127)     1702 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/WAVES/features/OffsetGoodMoveCount.py
--rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/WAVES/features/OverallPercentAmplitudeMoves.py
--rw-r--r--   0 runner    (1001) docker     (127)     1427 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/WAVES/features/OverallPercentOffsetMoves.py
--rw-r--r--   0 runner    (1001) docker     (127)     1449 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/WAVES/features/OverallPercentWavelengthMoves.py
--rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/WAVES/features/OverallSliderAverageRange.py
--rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/WAVES/features/OverallSliderAverageStandardDeviations.py
--rw-r--r--   0 runner    (1001) docker     (127)     1919 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/WAVES/features/PercentAmplitudeGoodMoves.py
--rw-r--r--   0 runner    (1001) docker     (127)     1422 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/WAVES/features/PercentAmplitudeMoves.py
--rw-r--r--   0 runner    (1001) docker     (127)     1901 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/WAVES/features/PercentOffsetGoodMoves.py
--rw-r--r--   0 runner    (1001) docker     (127)     1325 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/WAVES/features/PercentOffsetMoves.py
--rw-r--r--   0 runner    (1001) docker     (127)     1843 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/WAVES/features/PercentWavelengthGoodMoves.py
--rw-r--r--   0 runner    (1001) docker     (127)     1345 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/WAVES/features/PercentWavelengthMoves.py
--rw-r--r--   0 runner    (1001) docker     (127)     1227 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/WAVES/features/PersistentSessionID.py
--rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/WAVES/features/QuestionAnswered.py
--rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/WAVES/features/QuestionCorrect.py
--rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/WAVES/features/RangeIntercept.py
--rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/WAVES/features/RangeR2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/WAVES/features/RangeSlope.py
--rw-r--r--   0 runner    (1001) docker     (127)     1627 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/WAVES/features/SequenceLevel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/WAVES/features/SessionID.py
--rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/WAVES/features/SliderAverageRange.py
--rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/WAVES/features/SliderAverageStandardDeviations.py
--rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/WAVES/features/SucceedCount.py
--rw-r--r--   0 runner    (1001) docker     (127)     2595 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/WAVES/features/TimeToAnswerMS.py
--rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/WAVES/features/TotalArrowMoves.py
--rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/WAVES/features/TotalFails.py
--rw-r--r--   0 runner    (1001) docker     (127)     1984 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/WAVES/features/TotalLevelTime.py
--rw-r--r--   0 runner    (1001) docker     (127)     1341 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/WAVES/features/TotalMoveTypeChanges.py
--rw-r--r--   0 runner    (1001) docker     (127)     1171 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/WAVES/features/TotalResets.py
--rw-r--r--   0 runner    (1001) docker     (127)     1163 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/WAVES/features/TotalSkips.py
--rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/WAVES/features/TotalSliderMoves.py
--rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/WAVES/features/WavelengthGoodMoveCount.py
--rw-r--r--   0 runner    (1001) docker     (127)     2575 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/WAVES/features/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:29:13.802339 opengamedata_core-0.0.2/src/ogd/games/WAVES/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)    21383 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/WAVES/schemas/WAVES.json.template
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:29:13.726339 opengamedata_core-0.0.2/src/ogd/games/WEATHER_STATION/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:29:13.802339 opengamedata_core-0.0.2/src/ogd/games/WEATHER_STATION/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)    34344 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/WEATHER_STATION/schemas/WEATHER_STATION.json.template
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:29:13.726339 opengamedata_core-0.0.2/src/ogd/games/WIND/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:29:13.802339 opengamedata_core-0.0.2/src/ogd/games/WIND/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/WIND/schemas/WIND.json.template
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 17:28:32.000000 opengamedata_core-0.0.2/src/ogd/games/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:29:13.802339 opengamedata_core-0.0.2/src/opengamedata_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4796 2024-05-06 17:29:13.000000 opengamedata_core-0.0.2/src/opengamedata_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    20752 2024-05-06 17:29:13.000000 opengamedata_core-0.0.2/src/opengamedata_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 17:29:13.000000 opengamedata_core-0.0.2/src/opengamedata_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-06 17:29:13.000000 opengamedata_core-0.0.2/src/opengamedata_core.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 17:29:13.802339 opengamedata_core-0.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3113 2024-05-06 17:28:33.000000 opengamedata_core-0.0.2/tests/test_lakeland_models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:05:19.896207 opengamedata_core-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4796 2024-05-15 21:05:19.896207 opengamedata_core-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3900 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 21:05:19.896207 opengamedata_core-0.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:05:19.812207 opengamedata_core-0.0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:05:19.816207 opengamedata_core-0.0.3/src/ogd/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:05:19.816207 opengamedata_core-0.0.3/src/ogd/core/
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:05:19.816207 opengamedata_core-0.0.3/src/ogd/core/exec/
+-rw-r--r--   0 runner    (1001) docker     (127)     9329 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/core/exec/Commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3763 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/core/exec/Generators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4858 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/core/exec/Parsers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:05:19.804207 opengamedata_core-0.0.3/src/ogd/core/games/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:05:19.804207 opengamedata_core-0.0.3/src/ogd/core/games/AQUALAB/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:05:19.816207 opengamedata_core-0.0.3/src/ogd/core/games/AQUALAB/features/
+-rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/core/games/AQUALAB/features/AppVersions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4209 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/core/games/AQUALAB/features/PlayLocations.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:05:19.804207 opengamedata_core-0.0.3/src/ogd/core/games/JOURNALISM/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:05:19.816207 opengamedata_core-0.0.3/src/ogd/core/games/JOURNALISM/features/
+-rw-r--r--   0 runner    (1001) docker     (127)     2899 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/core/games/JOURNALISM/features/FailureAttributes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1907 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/core/games/JOURNALISM/features/FinalAttributes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:05:19.816207 opengamedata_core-0.0.3/src/ogd/core/generators/
+-rw-r--r--   0 runner    (1001) docker     (127)     7941 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/core/generators/Generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5136 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/core/generators/GeneratorLoader.py
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/core/generators/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:05:19.816207 opengamedata_core-0.0.3/src/ogd/core/generators/detectors/
+-rw-r--r--   0 runner    (1001) docker     (127)     4351 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/core/generators/detectors/Detector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2300 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/core/generators/detectors/DetectorEvent.py
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/core/generators/detectors/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:05:19.816207 opengamedata_core-0.0.3/src/ogd/core/generators/extractors/
+-rw-r--r--   0 runner    (1001) docker     (127)     6499 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/core/generators/extractors/Extractor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/core/generators/extractors/Feature.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1585 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/core/generators/extractors/PerCountFeature.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/core/generators/extractors/PerLevelFeature.py
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/core/generators/extractors/SessionFeature.py
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/core/generators/extractors/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:05:19.820207 opengamedata_core-0.0.3/src/ogd/core/generators/legacy/
+-rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/core/generators/legacy/LegacyDetector.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14632 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/core/generators/legacy/LegacyFeature.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/core/generators/legacy/LegacyLoader.py
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/core/generators/legacy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:05:19.820207 opengamedata_core-0.0.3/src/ogd/core/generators/registries/
+-rw-r--r--   0 runner    (1001) docker     (127)     8364 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/core/generators/registries/DetectorRegistry.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13799 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/core/generators/registries/ExtractorRegistry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5276 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/core/generators/registries/GeneratorRegistry.py
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/core/generators/registries/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:05:19.820207 opengamedata_core-0.0.3/src/ogd/core/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (127)    10850 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/core/interfaces/BQFirebaseInterface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9699 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/core/interfaces/BigQueryCodingInterface.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11865 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/core/interfaces/BigQueryInterface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4903 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/core/interfaces/CSVInterface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3519 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/core/interfaces/CodingInterface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5432 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/core/interfaces/DataInterface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/core/interfaces/Interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23918 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/core/interfaces/MySQLInterface.py
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/core/interfaces/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:05:19.820207 opengamedata_core-0.0.3/src/ogd/core/interfaces/outerfaces/
+-rw-r--r--   0 runner    (1001) docker     (127)     5824 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/core/interfaces/outerfaces/DataOuterface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4195 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/core/interfaces/outerfaces/DebugOuterface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4902 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/core/interfaces/outerfaces/DictionaryOuterface.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33757 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/core/interfaces/outerfaces/TSVOuterface.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:05:19.820207 opengamedata_core-0.0.3/src/ogd/core/managers/
+-rw-r--r--   0 runner    (1001) docker     (127)     3513 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/core/managers/EventManager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19007 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/core/managers/ExportManager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12108 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/core/managers/FeatureManager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/core/managers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:05:19.824207 opengamedata_core-0.0.3/src/ogd/core/processors/
+-rw-r--r--   0 runner    (1001) docker     (127)     6040 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/core/processors/ClassroomDetector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2239 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/core/processors/DetectorProcessor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      964 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/core/processors/EventProcessor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/core/processors/ExtractorProcessor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2628 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/core/processors/GeneratorProcessor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4602 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/core/processors/PlayerProcessor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4215 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/core/processors/PopulationProcessor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1878 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/core/processors/Processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4267 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/core/processors/SessionProcessor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/core/processors/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:05:19.824207 opengamedata_core-0.0.3/src/ogd/core/requests/
+-rw-r--r--   0 runner    (1001) docker     (127)     5301 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/core/requests/Request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2062 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/core/requests/RequestResult.py
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/core/requests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:05:19.824207 opengamedata_core-0.0.3/src/ogd/core/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)    14401 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/core/schemas/Event.py
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/core/schemas/ExportMode.py
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/core/schemas/ExtractionMode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1426 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/core/schemas/FeatureData.py
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/core/schemas/IDMode.py
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/core/schemas/IterationMode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1427 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/core/schemas/Schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/core/schemas/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:05:19.824207 opengamedata_core-0.0.3/src/ogd/core/schemas/configs/
+-rw-r--r--   0 runner    (1001) docker     (127)    10898 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/core/schemas/configs/ConfigSchema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5835 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/core/schemas/configs/GameSourceSchema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3452 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/core/schemas/configs/IndexingSchema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2593 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/core/schemas/configs/LegacyConfigSchema.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:05:19.828207 opengamedata_core-0.0.3/src/ogd/core/schemas/configs/data_sources/
+-rw-r--r--   0 runner    (1001) docker     (127)     3048 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/core/schemas/configs/data_sources/BigQuerySourceSchema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1806 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/core/schemas/configs/data_sources/DataSourceSchema.py
+-rw-r--r--   0 runner    (1001) docker     (127)      577 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/core/schemas/configs/data_sources/FileSourceSchema.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10140 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/core/schemas/configs/data_sources/MySQLSourceSchema.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:05:19.828207 opengamedata_core-0.0.3/src/ogd/core/schemas/games/
+-rw-r--r--   0 runner    (1001) docker     (127)      922 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/core/schemas/games/AggregateSchema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5168 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/core/schemas/games/DataElementSchema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5045 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/core/schemas/games/DetectorMapSchema.py
+-rw-r--r--   0 runner    (1001) docker     (127)      801 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/core/schemas/games/DetectorSchema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3996 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/core/schemas/games/EventSchema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4006 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/core/schemas/games/ExtractorSchema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5656 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/core/schemas/games/FeatureMapSchema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4869 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/core/schemas/games/FeatureSchema.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26726 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/core/schemas/games/GameSchema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2652 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/core/schemas/games/GameStateSchema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2831 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/core/schemas/games/PerCountSchema.py
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/core/schemas/games/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:05:19.828207 opengamedata_core-0.0.3/src/ogd/core/schemas/table_schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)     3615 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/core/schemas/table_schemas/BIGQUERY.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4890 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/core/schemas/table_schemas/FIELDDAY_MYSQL.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2573 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/core/schemas/table_schemas/FIREBASE.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4430 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/core/schemas/table_schemas/MASHOPOLIS_MYSQL.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3685 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/core/schemas/table_schemas/OGD_EVENT_FILE.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4077 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/core/schemas/table_schemas/OPENGAMEDATA_BIGQUERY.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4477 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/core/schemas/table_schemas/OPENGAMEDATA_MYSQL.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1920 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/core/schemas/table_schemas/SHIPWRECKS.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:05:19.832207 opengamedata_core-0.0.3/src/ogd/core/schemas/tables/
+-rw-r--r--   0 runner    (1001) docker     (127)     6782 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/core/schemas/tables/ColumnMapSchema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4174 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/core/schemas/tables/ColumnSchema.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23084 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/core/schemas/tables/TableSchema.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:05:19.832207 opengamedata_core-0.0.3/src/ogd/core/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     4567 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/core/utils/Logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4361 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/core/utils/Readme.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6145 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/core/utils/SemanticVersion.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/core/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/core/utils/typing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2692 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/core/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:05:19.832207 opengamedata_core-0.0.3/src/ogd/games/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:05:19.808207 opengamedata_core-0.0.3/src/ogd/games/ALL_YOU_CAN_ET/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:05:19.832207 opengamedata_core-0.0.3/src/ogd/games/ALL_YOU_CAN_ET/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)    20816 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/ALL_YOU_CAN_ET/schemas/ALL_YOU_CAN_ET.json.template
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:05:19.832207 opengamedata_core-0.0.3/src/ogd/games/AQUALAB/
+-rw-r--r--   0 runner    (1001) docker     (127)    13543 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/AQUALAB/AqualabLoader.py
+-rw-r--r--   0 runner    (1001) docker     (127)   278275 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/AQUALAB/DBExport.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/AQUALAB/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:05:19.832207 opengamedata_core-0.0.3/src/ogd/games/AQUALAB/detectors/
+-rw-r--r--   0 runner    (1001) docker     (127)     2320 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/AQUALAB/detectors/CollectFactNoJob.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3554 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/AQUALAB/detectors/DiveSiteNoEvidence.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1725 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/AQUALAB/detectors/EchoRoomChange.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4505 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/AQUALAB/detectors/HintAndLeave.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3466 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/AQUALAB/detectors/Idle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3901 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/AQUALAB/detectors/SceneChangeFrequently.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3796 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/AQUALAB/detectors/TwoHints.py
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/AQUALAB/detectors/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:05:19.844207 opengamedata_core-0.0.3/src/ogd/games/AQUALAB/features/
+-rw-r--r--   0 runner    (1001) docker     (127)     2752 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/AQUALAB/features/ActiveJobs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2332 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/AQUALAB/features/ActiveTime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/AQUALAB/features/AppVersions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/AQUALAB/features/AverageSessionTime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/AQUALAB/features/EchoSessionID.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5318 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/AQUALAB/features/EventList.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9513 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/AQUALAB/features/JobActiveTime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2460 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/AQUALAB/features/JobArgumentation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2708 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/AQUALAB/features/JobCompletionTime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/AQUALAB/features/JobDiveSitesCount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2138 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/AQUALAB/features/JobDiveTime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2408 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/AQUALAB/features/JobExperimentation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/AQUALAB/features/JobGuideCount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/AQUALAB/features/JobHelpCount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3952 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/AQUALAB/features/JobLocationChanges.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2279 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/AQUALAB/features/JobModeling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2344 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/AQUALAB/features/JobPlayTime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2119 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/AQUALAB/features/JobPriorAttempt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1943 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/AQUALAB/features/JobPriorComplete.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/AQUALAB/features/JobStartCount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/AQUALAB/features/JobTasksCompleted.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1600 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/AQUALAB/features/JobTriesInArgument.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6192 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/AQUALAB/features/JobsAttempted.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/AQUALAB/features/JobsCompleted.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/AQUALAB/features/ModelExportCount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1299 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/AQUALAB/features/ModelInterveneCount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/AQUALAB/features/ModelPredictCount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/AQUALAB/features/PerJobFeature.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4256 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/AQUALAB/features/PlayLocations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3014 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/AQUALAB/features/PlayerSummary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3351 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/AQUALAB/features/PopulationSummary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/AQUALAB/features/RegionJobCount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/AQUALAB/features/RegionName.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/AQUALAB/features/SessionDiveSitesCount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3950 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/AQUALAB/features/SessionDuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/AQUALAB/features/SessionGuideCount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/AQUALAB/features/SessionHelpCount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/AQUALAB/features/SessionID.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/AQUALAB/features/SessionJobsCompleted.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/AQUALAB/features/SwitchJobsCount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2521 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/AQUALAB/features/SyncCompletionTime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1733 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/AQUALAB/features/TankRulesCount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3458 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/AQUALAB/features/TopJobCompletionDestinations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3444 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/AQUALAB/features/TopJobSwitchDestinations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3339 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/AQUALAB/features/TotalArcticTime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2193 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/AQUALAB/features/TotalArgumentationTime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3332 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/AQUALAB/features/TotalBayouTime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3332 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/AQUALAB/features/TotalCoralTime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2794 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/AQUALAB/features/TotalDiveTime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2136 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/AQUALAB/features/TotalExperimentationTime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/AQUALAB/features/TotalGuideCount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/AQUALAB/features/TotalHelpCount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3325 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/AQUALAB/features/TotalKelpTime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2121 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/AQUALAB/features/TotalModelingTime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2493 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/AQUALAB/features/TotalPlayTime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1440 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/AQUALAB/features/UserAvgActiveTime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1412 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/AQUALAB/features/UserAvgSessionDuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/AQUALAB/features/UserTotalSessionDuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3191 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/AQUALAB/features/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:05:19.844207 opengamedata_core-0.0.3/src/ogd/games/AQUALAB/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)    32600 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/AQUALAB/schemas/AQUALAB.json.template
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:05:19.808207 opengamedata_core-0.0.3/src/ogd/games/BACTERIA/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:05:19.844207 opengamedata_core-0.0.3/src/ogd/games/BACTERIA/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/BACTERIA/schemas/BACTERIA.json.template
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:05:19.808207 opengamedata_core-0.0.3/src/ogd/games/BALLOON/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:05:19.844207 opengamedata_core-0.0.3/src/ogd/games/BALLOON/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/BALLOON/schemas/BALLOON.json.template
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:05:19.808207 opengamedata_core-0.0.3/src/ogd/games/BLOOM/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:05:19.844207 opengamedata_core-0.0.3/src/ogd/games/BLOOM/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)    21554 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/BLOOM/schemas/BLOOM.json.template
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:05:19.808207 opengamedata_core-0.0.3/src/ogd/games/CENSIO_SLIDE/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:05:19.844207 opengamedata_core-0.0.3/src/ogd/games/CENSIO_SLIDE/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)    11446 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/CENSIO_SLIDE/schemas/CENSIO_SLIDE.json.template
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:05:19.808207 opengamedata_core-0.0.3/src/ogd/games/CENSIO_STACK/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:05:19.844207 opengamedata_core-0.0.3/src/ogd/games/CENSIO_STACK/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)    21742 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/CENSIO_STACK/schemas/CENSIO_STACK.json.template
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:05:19.808207 opengamedata_core-0.0.3/src/ogd/games/CRUSH_STATION/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:05:19.844207 opengamedata_core-0.0.3/src/ogd/games/CRUSH_STATION/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)    11756 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/CRUSH_STATION/schemas/CRUSH_STATION.json.template
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:05:19.844207 opengamedata_core-0.0.3/src/ogd/games/CRYSTAL/
+-rw-r--r--   0 runner    (1001) docker     (127)     2380 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/CRYSTAL/CrystalLoader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:05:19.848207 opengamedata_core-0.0.3/src/ogd/games/CRYSTAL/features/
+-rw-r--r--   0 runner    (1001) docker     (127)    14123 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/CRYSTAL/features/CrystalExtractor.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/CRYSTAL/features/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:05:19.848207 opengamedata_core-0.0.3/src/ogd/games/CRYSTAL/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)    14066 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/CRYSTAL/schemas/CRYSTAL.json.template
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:05:19.808207 opengamedata_core-0.0.3/src/ogd/games/CYCLE_CARBON/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:05:19.848207 opengamedata_core-0.0.3/src/ogd/games/CYCLE_CARBON/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/CYCLE_CARBON/schemas/CYCLE_CARBON.json.template
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:05:19.808207 opengamedata_core-0.0.3/src/ogd/games/CYCLE_NITROGEN/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:05:19.848207 opengamedata_core-0.0.3/src/ogd/games/CYCLE_NITROGEN/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/CYCLE_NITROGEN/schemas/CYCLE_NITROGEN.json.template
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:05:19.808207 opengamedata_core-0.0.3/src/ogd/games/CYCLE_WATER/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:05:19.848207 opengamedata_core-0.0.3/src/ogd/games/CYCLE_WATER/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/CYCLE_WATER/schemas/CYCLE_WATER.json.template
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:05:19.808207 opengamedata_core-0.0.3/src/ogd/games/EARTHQUAKE/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:05:19.848207 opengamedata_core-0.0.3/src/ogd/games/EARTHQUAKE/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/EARTHQUAKE/schemas/EARTHQUAKE.json.template
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:05:19.808207 opengamedata_core-0.0.3/src/ogd/games/GWAKKAMOLE/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:05:19.848207 opengamedata_core-0.0.3/src/ogd/games/GWAKKAMOLE/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)    12879 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/GWAKKAMOLE/schemas/GWAKKAMOLE.json.template
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:05:19.848207 opengamedata_core-0.0.3/src/ogd/games/ICECUBE/
+-rw-r--r--   0 runner    (1001) docker     (127)     1883 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/ICECUBE/DBExport.json
+-rw-r--r--   0 runner    (1001) docker     (127)      803 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/ICECUBE/DBExport.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4855 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/ICECUBE/IcecubeLoader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:05:19.848207 opengamedata_core-0.0.3/src/ogd/games/ICECUBE/features/
+-rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/ICECUBE/features/HeadsetOnCount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1891 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/ICECUBE/features/ObjectSelectionsDuringVoiceover.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/ICECUBE/features/PerSceneFeature.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2890 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/ICECUBE/features/SceneDuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1941 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/ICECUBE/features/SceneFailureCount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2720 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/ICECUBE/features/SceneFailures.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1380 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/ICECUBE/features/ScenesEncountered.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3466 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/ICECUBE/features/SessionDuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/ICECUBE/features/Session_Language.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2389 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/ICECUBE/features/TaskTimeToComplete.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1780 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/ICECUBE/features/ViewportCountPerScene.py
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/ICECUBE/features/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:05:19.852207 opengamedata_core-0.0.3/src/ogd/games/ICECUBE/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)     7292 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/ICECUBE/schemas/ICECUBE.json.template
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:05:19.852207 opengamedata_core-0.0.3/src/ogd/games/JOURNALISM/
+-rw-r--r--   0 runner    (1001) docker     (127)     7977 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/JOURNALISM/JournalismLoader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:05:19.856207 opengamedata_core-0.0.3/src/ogd/games/JOURNALISM/features/
+-rw-r--r--   0 runner    (1001) docker     (127)     4546 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/JOURNALISM/features/AttributeView.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4973 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/JOURNALISM/features/ChoiceClickCount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2234 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/JOURNALISM/features/ContinuesOnFail.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4549 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/JOURNALISM/features/EditorNoteOpen.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4994 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/JOURNALISM/features/FailureCount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3968 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/JOURNALISM/features/GameComplete.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4859 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/JOURNALISM/features/LevelCompleteCount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4866 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/JOURNALISM/features/LevelCompleted.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2824 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/JOURNALISM/features/LevelTime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2340 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/JOURNALISM/features/MaxedPlayerAttribute.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5255 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/JOURNALISM/features/MeanSnippetTime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4459 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/JOURNALISM/features/PlayTime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4384 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/JOURNALISM/features/PlayerAttributes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4468 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/JOURNALISM/features/QuitLevel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4142 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/JOURNALISM/features/QuitNode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7634 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/JOURNALISM/features/QuitType.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6945 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/JOURNALISM/features/QuitTypePerLevel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5902 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/JOURNALISM/features/SessionPlayTime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5063 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/JOURNALISM/features/SkillSequenceCount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3745 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/JOURNALISM/features/SnippetReceivedCount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5004 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/JOURNALISM/features/SnippetReplace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2078 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/JOURNALISM/features/SnippetsCollected.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1778 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/JOURNALISM/features/SnippetsSubmitted.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/JOURNALISM/features/StoryAlignment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2217 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/JOURNALISM/features/StoryAlignmentSequence.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5473 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/JOURNALISM/features/StoryCompleteTime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6576 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/JOURNALISM/features/StoryEditorTime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/JOURNALISM/features/StoryScore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2190 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/JOURNALISM/features/StoryScoreSequence.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4773 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/JOURNALISM/features/TextClickCount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4720 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/JOURNALISM/features/TopAttribute.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2228 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/JOURNALISM/features/TopPlayerAttribute.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2272 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/JOURNALISM/features/TopPlayerQuitType.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4475 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/JOURNALISM/features/TotalFails.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2086 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/JOURNALISM/features/TotalLevelTime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3948 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/JOURNALISM/features/UserPlayTime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4729 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/JOURNALISM/features/WorstAttribute.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2242 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/JOURNALISM/features/WorstPlayerAttribute.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2048 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/JOURNALISM/features/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:05:19.856207 opengamedata_core-0.0.3/src/ogd/games/JOURNALISM/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)    45415 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/JOURNALISM/schemas/JOURNALISM.json.template
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:05:19.860207 opengamedata_core-0.0.3/src/ogd/games/JOWILDER/
+-rw-r--r--   0 runner    (1001) docker     (127)     5206 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/JOWILDER/JowilderLoader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16451 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/JOWILDER/Jowilder_Enumerators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:05:19.864207 opengamedata_core-0.0.3/src/ogd/games/JOWILDER/features/
+-rw-r--r--   0 runner    (1001) docker     (127)     3089 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/JOWILDER/features/ActiveStateTime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1838 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/JOWILDER/features/Clicks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1438 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/JOWILDER/features/EventCount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1736 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/JOWILDER/features/FirstInteraction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1822 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/JOWILDER/features/GameScript.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1439 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/JOWILDER/features/GameVersion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1359 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/JOWILDER/features/Hovers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2458 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/JOWILDER/features/IdleState.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7609 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/JOWILDER/features/Interaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2338 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/JOWILDER/features/InteractionName.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4592 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/JOWILDER/features/InteractionTextBoxesPerSecond.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4587 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/JOWILDER/features/InteractionWordsPerSecond.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1684 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/JOWILDER/features/LastInteraction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1720 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/JOWILDER/features/MeaningfulActions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2000 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/JOWILDER/features/NotebookUses.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3211 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/JOWILDER/features/QuestionAnswers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1770 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/JOWILDER/features/SessionDuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1887 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/JOWILDER/features/SessionStart.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5104 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/JOWILDER/features/SurveyItem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2791 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/JOWILDER/features/SurveyTime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1631 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/JOWILDER/features/UsedContinue.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/JOWILDER/features/UsedSaveCode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2151 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/JOWILDER/features/UserEnabled.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/JOWILDER/features/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1925 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/JOWILDER/get_jowilder_all_items.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:05:19.864207 opengamedata_core-0.0.3/src/ogd/games/JOWILDER/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)    35912 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/JOWILDER/schemas/JOWILDER.json.template
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:05:19.864207 opengamedata_core-0.0.3/src/ogd/games/LAKELAND/
+-rw-r--r--   0 runner    (1001) docker     (127)     2357 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/LAKELAND/LakelandLoader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:05:19.872207 opengamedata_core-0.0.3/src/ogd/games/LAKELAND/features/
+-rw-r--r--   0 runner    (1001) docker     (127)     2039 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/LAKELAND/features/ActionsLastXSecondsModel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      607 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/LAKELAND/features/DeathCountModel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11750 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/LAKELAND/features/DeathPredModel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8664 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/LAKELAND/features/DeathThresholdModel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4916 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/LAKELAND/features/DiagonalFarmDetectorModel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7995 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/LAKELAND/features/FeatSeqPercent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2294 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/LAKELAND/features/FeatVelocity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/LAKELAND/features/FeatureModel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8478 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/LAKELAND/features/LAKELAND_models.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4415 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/LAKELAND/features/LakelandEnumerators.json
+-rw-r--r--   0 runner    (1001) docker     (127)    69732 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/LAKELAND/features/LakelandExtractor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2639 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/LAKELAND/features/LinearModel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2701 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/LAKELAND/features/LogisticModel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3353 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/LAKELAND/features/MapSummaryModel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/LAKELAND/features/Model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2574 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/LAKELAND/features/MoneyAccumulationModel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      444 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/LAKELAND/features/NthEventModel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      496 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/LAKELAND/features/PlayingTimeModel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3287 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/LAKELAND/features/PopulationModel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4813 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/LAKELAND/features/RecentPurchasesModel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1264 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/LAKELAND/features/SequenceModel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4909 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/LAKELAND/features/SimpleFarmAbandonmentModel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      850 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/LAKELAND/features/SingleFeatureModel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6060 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/LAKELAND/features/TimeSinceEventTypes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/LAKELAND/features/TimeSinceLastSaleModel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      507 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/LAKELAND/features/TownCompositionFeatureModel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2026 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/LAKELAND/features/TownCompositionModel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/LAKELAND/features/TutorialProgressionModel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    82382 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/LAKELAND/features/WAVES_models.json
+-rw-r--r--   0 runner    (1001) docker     (127)    82382 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/LAKELAND/features/WAVES_models_L8_Q0_Q1.json
+-rw-r--r--   0 runner    (1001) docker     (127)    49819 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/LAKELAND/features/WAVES_models_L8_and_Q0.json
+-rw-r--r--   0 runner    (1001) docker     (127)    28429 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/LAKELAND/features/WAVES_models_L8_complete_and_current.json
+-rw-r--r--   0 runner    (1001) docker     (127)    21021 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/LAKELAND/features/WAVES_models_L8_only_complete.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/LAKELAND/features/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2331 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/LAKELAND/produce_lakeland_enumerators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:05:19.872207 opengamedata_core-0.0.3/src/ogd/games/LAKELAND/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)   115553 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/LAKELAND/schemas/LAKELAND.json.template
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:05:19.872207 opengamedata_core-0.0.3/src/ogd/games/MAGNET/
+-rw-r--r--   0 runner    (1001) docker     (127)     2346 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/MAGNET/MagnetLoader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:05:19.872207 opengamedata_core-0.0.3/src/ogd/games/MAGNET/features/
+-rw-r--r--   0 runner    (1001) docker     (127)     8596 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/MAGNET/features/MagnetExtractor.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/MAGNET/features/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:05:19.872207 opengamedata_core-0.0.3/src/ogd/games/MAGNET/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)     7887 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/MAGNET/schemas/MAGNET.json.template
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:05:19.812207 opengamedata_core-0.0.3/src/ogd/games/MASHOPOLIS/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:05:19.872207 opengamedata_core-0.0.3/src/ogd/games/MASHOPOLIS/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)    10063 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/MASHOPOLIS/schemas/MASHOPOLIS.json.template
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:05:19.872207 opengamedata_core-0.0.3/src/ogd/games/PENGUINS/
+-rw-r--r--   0 runner    (1001) docker     (127)     2970 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/PENGUINS/DBExport.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7109 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/PENGUINS/PenguinsLoader.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/PENGUINS/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:05:19.872207 opengamedata_core-0.0.3/src/ogd/games/PENGUINS/detectors/
+-rw-r--r--   0 runner    (1001) docker     (127)     3747 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/PENGUINS/detectors/RegionEnter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3966 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/PENGUINS/detectors/RegionExit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/PENGUINS/detectors/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:05:19.876207 opengamedata_core-0.0.3/src/ogd/games/PENGUINS/features/
+-rw-r--r--   0 runner    (1001) docker     (127)     1691 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/PENGUINS/features/ActivityCompleted.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2720 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/PENGUINS/features/ActivityDuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/PENGUINS/features/EatFishCount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/PENGUINS/features/EggLostCount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2401 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/PENGUINS/features/EggRecoverTime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1792 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/PENGUINS/features/GazeCount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2663 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/PENGUINS/features/GazeDuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4361 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/PENGUINS/features/MirrorWaddleDuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1901 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/PENGUINS/features/PerRegionFeature.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1232 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/PENGUINS/features/PickupRockCount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2636 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/PENGUINS/features/PlayerInactiveAvgDuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/PENGUINS/features/PlayerWaddleCount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2290 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/PENGUINS/features/RegionDuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/PENGUINS/features/RegionEnterCount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/PENGUINS/features/RegionsEncountered.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/PENGUINS/features/RingChimesCount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3599 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/PENGUINS/features/SessionDuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2101 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/PENGUINS/features/SnowBallDuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1689 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/PENGUINS/features/WaddlePerRegion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/PENGUINS/features/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:05:19.876207 opengamedata_core-0.0.3/src/ogd/games/PENGUINS/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)    28356 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/PENGUINS/schemas/PENGUINS.json.template
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:05:19.876207 opengamedata_core-0.0.3/src/ogd/games/SHADOWSPECT/
+-rw-r--r--   0 runner    (1001) docker     (127)     3232 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/SHADOWSPECT/ShadowspectLoader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:05:19.880207 opengamedata_core-0.0.3/src/ogd/games/SHADOWSPECT/features/
+-rw-r--r--   0 runner    (1001) docker     (127)     2789 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/SHADOWSPECT/features/FunnelByUser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7671 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/SHADOWSPECT/features/LevelsOfDifficulty.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/SHADOWSPECT/features/MoveShapeCount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3897 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/SHADOWSPECT/features/SequenceBetweenPuzzles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1050 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/SHADOWSPECT/features/SessionID.py
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/SHADOWSPECT/features/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:05:19.880207 opengamedata_core-0.0.3/src/ogd/games/SHADOWSPECT/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)    29173 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/SHADOWSPECT/schemas/SHADOWSPECT.json.template
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:05:19.880207 opengamedata_core-0.0.3/src/ogd/games/SHIPWRECKS/
+-rw-r--r--   0 runner    (1001) docker     (127)     4677 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/SHIPWRECKS/ShipwrecksLoader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:05:19.880207 opengamedata_core-0.0.3/src/ogd/games/SHIPWRECKS/features/
+-rw-r--r--   0 runner    (1001) docker     (127)     2164 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/SHIPWRECKS/features/ActiveJobs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2333 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/SHIPWRECKS/features/EventList.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/SHIPWRECKS/features/EvidenceBoardCompleteCount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3545 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/SHIPWRECKS/features/JobsAttempted.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/SHIPWRECKS/features/JobsCompleted.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1426 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/SHIPWRECKS/features/MissionDiveTime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/SHIPWRECKS/features/MissionSonarTimeToComplete.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1526 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/SHIPWRECKS/features/PlayerSummary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1945 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/SHIPWRECKS/features/PopulationSummary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/SHIPWRECKS/features/SessionDuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/SHIPWRECKS/features/SessionID.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2992 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/SHIPWRECKS/features/TopJobCompletionDestinations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2736 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/SHIPWRECKS/features/TopJobSwitchDestinations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1392 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/SHIPWRECKS/features/TotalDiveTime.py
+-rw-r--r--   0 runner    (1001) docker     (127)      798 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/SHIPWRECKS/features/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:05:19.884207 opengamedata_core-0.0.3/src/ogd/games/SHIPWRECKS/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)    10509 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/SHIPWRECKS/schemas/SHIPWRECKS.json.template
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:05:19.884207 opengamedata_core-0.0.3/src/ogd/games/THERMOVR/
+-rw-r--r--   0 runner    (1001) docker     (127)        3 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/THERMOVR/DBExport.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5663 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/THERMOVR/ThermoVRLoader.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/THERMOVR/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:05:19.884207 opengamedata_core-0.0.3/src/ogd/games/THERMOVR/detectors/
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/THERMOVR/detectors/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:05:19.884207 opengamedata_core-0.0.3/src/ogd/games/THERMOVR/features/
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/THERMOVR/features/LabCompleteCount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1888 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/THERMOVR/features/LeftHandMoves.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/THERMOVR/features/PhasesReached.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/THERMOVR/features/PlayMode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1893 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/THERMOVR/features/RightHandMoves.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/THERMOVR/features/TaskCompleteCount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/THERMOVR/features/ToolNudgeCount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1697 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/THERMOVR/features/ToolSliderTime.py
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/THERMOVR/features/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:05:19.884207 opengamedata_core-0.0.3/src/ogd/games/THERMOVR/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)    51378 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/THERMOVR/schemas/THERMOVR.json.template
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:05:19.884207 opengamedata_core-0.0.3/src/ogd/games/TRANSFORMATION_QUEST/
+-rw-r--r--   0 runner    (1001) docker     (127)      777 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/TRANSFORMATION_QUEST/DBExport.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:05:19.884207 opengamedata_core-0.0.3/src/ogd/games/TRANSFORMATION_QUEST/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)    25177 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/TRANSFORMATION_QUEST/schemas/TRANSFORMATION_QUEST.json.template
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:05:19.884207 opengamedata_core-0.0.3/src/ogd/games/WAVES/
+-rw-r--r--   0 runner    (1001) docker     (127)    37332 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/WAVES/WaveLoader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:05:19.896207 opengamedata_core-0.0.3/src/ogd/games/WAVES/features/
+-rw-r--r--   0 runner    (1001) docker     (127)     1708 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/WAVES/features/AmplitudeGoodMoveCount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1423 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/WAVES/features/AverageFails.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3487 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/WAVES/features/AverageLevelTime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1874 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/WAVES/features/AverageMoveTypeChanges.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1476 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/WAVES/features/AverageSliderMoves.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/WAVES/features/BeginCount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2012 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/WAVES/features/ClosenessIntercept.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/WAVES/features/ClosenessR2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/WAVES/features/ClosenessSlope.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/WAVES/features/Completed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1192 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/WAVES/features/FirstMoveType.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/WAVES/features/MenuButtonCount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1702 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/WAVES/features/OffsetGoodMoveCount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/WAVES/features/OverallPercentAmplitudeMoves.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1427 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/WAVES/features/OverallPercentOffsetMoves.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1449 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/WAVES/features/OverallPercentWavelengthMoves.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/WAVES/features/OverallSliderAverageRange.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/WAVES/features/OverallSliderAverageStandardDeviations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1919 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/WAVES/features/PercentAmplitudeGoodMoves.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1422 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/WAVES/features/PercentAmplitudeMoves.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1901 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/WAVES/features/PercentOffsetGoodMoves.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1325 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/WAVES/features/PercentOffsetMoves.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1843 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/WAVES/features/PercentWavelengthGoodMoves.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1345 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/WAVES/features/PercentWavelengthMoves.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1227 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/WAVES/features/PersistentSessionID.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/WAVES/features/QuestionAnswered.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/WAVES/features/QuestionCorrect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/WAVES/features/RangeIntercept.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/WAVES/features/RangeR2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/WAVES/features/RangeSlope.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1627 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/WAVES/features/SequenceLevel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/WAVES/features/SessionID.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/WAVES/features/SliderAverageRange.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/WAVES/features/SliderAverageStandardDeviations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/WAVES/features/SucceedCount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2595 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/WAVES/features/TimeToAnswerMS.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/WAVES/features/TotalArrowMoves.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/WAVES/features/TotalFails.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1984 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/WAVES/features/TotalLevelTime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1341 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/WAVES/features/TotalMoveTypeChanges.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1171 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/WAVES/features/TotalResets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1163 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/WAVES/features/TotalSkips.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/WAVES/features/TotalSliderMoves.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/WAVES/features/WavelengthGoodMoveCount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2575 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/WAVES/features/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:05:19.896207 opengamedata_core-0.0.3/src/ogd/games/WAVES/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)    21383 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/WAVES/schemas/WAVES.json.template
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:05:19.812207 opengamedata_core-0.0.3/src/ogd/games/WEATHER_STATION/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:05:19.896207 opengamedata_core-0.0.3/src/ogd/games/WEATHER_STATION/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)    34344 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/WEATHER_STATION/schemas/WEATHER_STATION.json.template
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:05:19.812207 opengamedata_core-0.0.3/src/ogd/games/WIND/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:05:19.896207 opengamedata_core-0.0.3/src/ogd/games/WIND/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/WIND/schemas/WIND.json.template
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/src/ogd/games/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:05:19.896207 opengamedata_core-0.0.3/src/opengamedata_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4796 2024-05-15 21:05:19.000000 opengamedata_core-0.0.3/src/opengamedata_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    21737 2024-05-15 21:05:19.000000 opengamedata_core-0.0.3/src/opengamedata_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 21:05:19.000000 opengamedata_core-0.0.3/src/opengamedata_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-15 21:05:19.000000 opengamedata_core-0.0.3/src/opengamedata_core.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:05:19.896207 opengamedata_core-0.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3113 2024-05-15 21:04:34.000000 opengamedata_core-0.0.3/tests/test_lakeland_models.py
```

### Comparing `opengamedata_core-0.0.2/LICENSE` & `opengamedata_core-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/PKG-INFO` & `opengamedata_core-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opengamedata-core
-Version: 0.0.2
+Version: 0.0.3
 Summary: A package for retrieving and processing event-based video game data. Additional authors: Nick Spevacek, Renee Li, John McCloskey, Zach Studdiford, Glenn Palmer, Haishuo Chen, Daus, Ameya Kshirsagar, Yunqing Xiao, Erik Harpstead, Manuel Jesus Gomez Moratilla
 Author-email: Luke Swanson <superscription58@gmail.com>, David Gagnon <djgagnon@wisc.edu>
 Project-URL: Homepage, https://github.com/opengamedata/opengamedata-core
 Project-URL: Bug Tracker, https://github.com/opengamedata/opengamedata-core/issues
 Project-URL: Documentation, https://opengamedata-doc.readthedocs.io/en/latest/index.html
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `opengamedata_core-0.0.2/README.md` & `opengamedata_core-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/pyproject.toml` & `opengamedata_core-0.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/core/exec/Commands.py` & `opengamedata_core-0.0.3/src/ogd/core/exec/Commands.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/core/exec/Generators.py` & `opengamedata_core-0.0.3/src/ogd/core/exec/Generators.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/core/exec/Parsers.py` & `opengamedata_core-0.0.3/src/ogd/core/exec/Parsers.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/core/generators/Generator.py` & `opengamedata_core-0.0.3/src/ogd/core/generators/Generator.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,27 +34,27 @@
         """ Abstract function to get a list of event types the Feature wants.
             The types of event accepted by a feature are a responsibility of the Feature's developer,
             so this is a required part of interface instead of a config item in the schema.
 
         :return: [description]
         :rtype: List[str]
         """
-        pass
+        raise TypeError(f"Can't call function on class {cls.__name__} with abstract method _eventFilter")
 
     @classmethod
     @abc.abstractmethod
     def _featureFilter(cls, mode:ExtractionMode) -> List[str]:
         """Base function for getting any features a second-order feature depends upon.
         By default, no dependencies.
         Any feature intented to be second-order should override this function.
 
         :return: _description_
         :rtype: List[str]
         """
-        pass
+        raise TypeError(f"Can't call function on class {cls.__name__} with abstract method _featureFilter")
 
     ## Abstract declaration of a function to perform update of a feature from a row.
     @abc.abstractmethod
     def _updateFromEvent(self, event:Event):
         """Abstract declaration of a function to perform update of a feature from a row.
 
         :param event: An event, used to update the feature's data.
```

### Comparing `opengamedata_core-0.0.2/src/ogd/core/generators/GeneratorLoader.py` & `opengamedata_core-0.0.3/src/ogd/core/generators/GeneratorLoader.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/core/generators/detectors/Detector.py` & `opengamedata_core-0.0.3/src/ogd/core/generators/detectors/Detector.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/core/generators/detectors/DetectorEvent.py` & `opengamedata_core-0.0.3/src/ogd/core/generators/detectors/DetectorEvent.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/core/generators/extractors/Extractor.py` & `opengamedata_core-0.0.3/src/ogd/core/generators/extractors/Extractor.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/core/generators/extractors/Feature.py` & `opengamedata_core-0.0.3/src/ogd/core/generators/extractors/Feature.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/core/generators/extractors/PerCountFeature.py` & `opengamedata_core-0.0.3/src/ogd/core/generators/extractors/PerCountFeature.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/core/generators/extractors/PerLevelFeature.py` & `opengamedata_core-0.0.3/src/ogd/core/generators/extractors/PerLevelFeature.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/core/generators/extractors/SessionFeature.py` & `opengamedata_core-0.0.3/src/ogd/core/generators/extractors/SessionFeature.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/core/generators/legacy/LegacyDetector.py` & `opengamedata_core-0.0.3/src/ogd/core/generators/legacy/LegacyDetector.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/core/generators/legacy/LegacyFeature.py` & `opengamedata_core-0.0.3/src/ogd/core/generators/legacy/LegacyFeature.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/core/generators/legacy/LegacyLoader.py` & `opengamedata_core-0.0.3/src/ogd/core/generators/legacy/LegacyLoader.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/core/generators/registries/DetectorRegistry.py` & `opengamedata_core-0.0.3/src/ogd/core/generators/registries/DetectorRegistry.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/core/generators/registries/ExtractorRegistry.py` & `opengamedata_core-0.0.3/src/ogd/core/generators/registries/ExtractorRegistry.py`

 * *Files 2% similar despite different names*

```diff
@@ -233,14 +233,16 @@
         return ret_val
 
     def GetFeatureValues(self) -> List[Any]:
         ret_val : List[Any] = []
         for order in self._features:
             for feature in order.values():
                 next_vals = feature.GetFeatureValues()
+                if len(next_vals) != len(feature.GetFeatureNames()):
+                    raise ValueError(f"Feature {feature.Name} lists {len(feature.GetFeatureNames())} feature names, but returns {len(next_vals)} values!")
                 ret_val += next_vals if next_vals != [] else [None]
         return ret_val
 
     def GetFeatureStringValues(self) -> List[str]:
         ret_val : List[str] = []
         _vals   : List[Any] = self.GetFeatureValues()
```

### Comparing `opengamedata_core-0.0.2/src/ogd/core/generators/registries/GeneratorRegistry.py` & `opengamedata_core-0.0.3/src/ogd/core/generators/registries/GeneratorRegistry.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/core/interfaces/BQFirebaseInterface.py` & `opengamedata_core-0.0.3/src/ogd/core/interfaces/BQFirebaseInterface.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/core/interfaces/BigQueryCodingInterface.py` & `opengamedata_core-0.0.3/src/ogd/core/interfaces/BigQueryCodingInterface.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/core/interfaces/BigQueryInterface.py` & `opengamedata_core-0.0.3/src/ogd/core/interfaces/BigQueryInterface.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/core/interfaces/CSVInterface.py` & `opengamedata_core-0.0.3/src/ogd/core/interfaces/CSVInterface.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/core/interfaces/CodingInterface.py` & `opengamedata_core-0.0.3/src/ogd/core/interfaces/CodingInterface.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/core/interfaces/DataInterface.py` & `opengamedata_core-0.0.3/src/ogd/core/interfaces/DataInterface.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/core/interfaces/Interface.py` & `opengamedata_core-0.0.3/src/ogd/core/interfaces/Interface.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/core/interfaces/MySQLInterface.py` & `opengamedata_core-0.0.3/src/ogd/core/interfaces/MySQLInterface.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/core/interfaces/outerfaces/DataOuterface.py` & `opengamedata_core-0.0.3/src/ogd/core/interfaces/outerfaces/DataOuterface.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/core/interfaces/outerfaces/DebugOuterface.py` & `opengamedata_core-0.0.3/src/ogd/core/interfaces/outerfaces/DebugOuterface.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/core/interfaces/outerfaces/DictionaryOuterface.py` & `opengamedata_core-0.0.3/src/ogd/core/interfaces/outerfaces/DictionaryOuterface.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/core/interfaces/outerfaces/TSVOuterface.py` & `opengamedata_core-0.0.3/src/ogd/core/interfaces/outerfaces/TSVOuterface.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/core/managers/EventManager.py` & `opengamedata_core-0.0.3/src/ogd/core/managers/EventManager.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/core/managers/ExportManager.py` & `opengamedata_core-0.0.3/src/ogd/core/managers/ExportManager.py`

 * *Files 2% similar despite different names*

```diff
@@ -87,15 +87,15 @@
             Logger.Log(f"Outputting post-process data...", logging.INFO, depth=2)
             self._postProcess(request=request)
             Logger.Log(f"Done", logging.INFO)
 
             ret_val.SessionCount = len(_sess_ids)
             ret_val.RequestSucceeded(msg=f"Successfully executed data request {request}.")
         except ValueError as err:
-            msg = f"Failed to execute data request {str(request)}, an invalid value was found:\n{str(err)}"
+            msg = f"Failed to execute data request {str(request)}, an invalid value was found:\n{str(err)}\n{traceback.format_exc()}"
             ret_val.RequestErrored(msg=msg)
         except Exception as err:
             msg = f"Failed to execute data request {str(request)}, an unexpected error occurred:\n{type(err)} {str(err)}\n{traceback.format_exc()}"
             ret_val.RequestErrored(msg=msg)
         finally:
             time_delta = datetime.now() - start
             ret_val.Duration = time_delta
@@ -225,15 +225,16 @@
                              for j in range( 0, math.ceil(_num_sess / _slice_size) )]
 
     def _loadSlice(self, request:Request, next_slice_ids:List[str], slice_num:int, slice_count:int) -> Optional[List[Event]]:
         ret_val : Optional[List[Event]]
 
         Logger.Log(f"Retrieving slice [{slice_num}/{slice_count}]...", logging.INFO, depth=2)
         start : datetime = datetime.now()
-        ret_val = request.Interface.EventsFromIDs(id_list=next_slice_ids, id_mode=request.Range.IDMode)
+        # TODO : Add a way to configure what to exclude at higher level, here. So we can easily choose to leave out certain events.
+        ret_val = request.Interface.EventsFromIDs(id_list=next_slice_ids, id_mode=request.Range.IDMode, exclude_rows=None)
         time_delta = datetime.now() - start
         if ret_val is not None:
             Logger.Log(f"Retrieval time for slice [{slice_num}/{slice_count}]: {time_delta} to get {len(ret_val)} events", logging.INFO, depth=2)
         else:
             Logger.Log(f"Could not retrieve data set for slice [{slice_num}/{slice_count}].", logging.WARN, depth=2)
         return ret_val
```

### Comparing `opengamedata_core-0.0.2/src/ogd/core/managers/FeatureManager.py` & `opengamedata_core-0.0.3/src/ogd/core/managers/FeatureManager.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/core/processors/ClassroomDetector.py` & `opengamedata_core-0.0.3/src/ogd/core/processors/ClassroomDetector.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/core/processors/DetectorProcessor.py` & `opengamedata_core-0.0.3/src/ogd/core/processors/DetectorProcessor.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/core/processors/EventProcessor.py` & `opengamedata_core-0.0.3/src/ogd/core/processors/EventProcessor.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/core/processors/ExtractorProcessor.py` & `opengamedata_core-0.0.3/src/ogd/core/processors/ExtractorProcessor.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/core/processors/GeneratorProcessor.py` & `opengamedata_core-0.0.3/src/ogd/core/processors/GeneratorProcessor.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/core/processors/PlayerProcessor.py` & `opengamedata_core-0.0.3/src/ogd/core/processors/PlayerProcessor.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/core/processors/PopulationProcessor.py` & `opengamedata_core-0.0.3/src/ogd/core/processors/PopulationProcessor.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/core/processors/Processor.py` & `opengamedata_core-0.0.3/src/ogd/core/processors/Processor.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/core/processors/SessionProcessor.py` & `opengamedata_core-0.0.3/src/ogd/core/processors/SessionProcessor.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/core/requests/Request.py` & `opengamedata_core-0.0.3/src/ogd/core/requests/Request.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/core/requests/RequestResult.py` & `opengamedata_core-0.0.3/src/ogd/core/requests/RequestResult.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/core/schemas/Event.py` & `opengamedata_core-0.0.3/src/ogd/core/schemas/Event.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/core/schemas/FeatureData.py` & `opengamedata_core-0.0.3/src/ogd/core/schemas/FeatureData.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/core/schemas/Schema.py` & `opengamedata_core-0.0.3/src/ogd/core/schemas/Schema.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/core/schemas/configs/ConfigSchema.py` & `opengamedata_core-0.0.3/src/ogd/core/schemas/configs/ConfigSchema.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/core/schemas/configs/GameSourceSchema.py` & `opengamedata_core-0.0.3/src/ogd/core/schemas/configs/GameSourceSchema.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/core/schemas/configs/IndexingSchema.py` & `opengamedata_core-0.0.3/src/ogd/core/schemas/configs/IndexingSchema.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/core/schemas/configs/LegacyConfigSchema.py` & `opengamedata_core-0.0.3/src/ogd/core/schemas/configs/LegacyConfigSchema.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/core/schemas/configs/data_sources/BigQuerySourceSchema.py` & `opengamedata_core-0.0.3/src/ogd/core/schemas/configs/data_sources/BigQuerySourceSchema.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/core/schemas/configs/data_sources/DataSourceSchema.py` & `opengamedata_core-0.0.3/src/ogd/core/schemas/configs/data_sources/DataSourceSchema.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/core/schemas/configs/data_sources/FileSourceSchema.py` & `opengamedata_core-0.0.3/src/ogd/core/schemas/configs/data_sources/FileSourceSchema.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/core/schemas/configs/data_sources/MySQLSourceSchema.py` & `opengamedata_core-0.0.3/src/ogd/core/schemas/configs/data_sources/MySQLSourceSchema.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/core/schemas/games/AggregateSchema.py` & `opengamedata_core-0.0.3/src/ogd/core/schemas/games/AggregateSchema.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/core/schemas/games/DataElementSchema.py` & `opengamedata_core-0.0.3/src/ogd/core/schemas/games/DataElementSchema.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/core/schemas/games/DetectorMapSchema.py` & `opengamedata_core-0.0.3/src/ogd/core/schemas/games/DetectorMapSchema.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/core/schemas/games/DetectorSchema.py` & `opengamedata_core-0.0.3/src/ogd/core/schemas/games/DetectorSchema.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/core/schemas/games/EventSchema.py` & `opengamedata_core-0.0.3/src/ogd/core/schemas/games/EventSchema.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/core/schemas/games/ExtractorSchema.py` & `opengamedata_core-0.0.3/src/ogd/core/schemas/games/ExtractorSchema.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/core/schemas/games/FeatureMapSchema.py` & `opengamedata_core-0.0.3/src/ogd/core/schemas/games/FeatureMapSchema.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/core/schemas/games/FeatureSchema.py` & `opengamedata_core-0.0.3/src/ogd/core/schemas/games/FeatureSchema.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/core/schemas/games/GameSchema.py` & `opengamedata_core-0.0.3/src/ogd/core/schemas/games/GameSchema.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/core/schemas/games/GameStateSchema.py` & `opengamedata_core-0.0.3/src/ogd/core/schemas/games/GameStateSchema.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/core/schemas/games/PerCountSchema.py` & `opengamedata_core-0.0.3/src/ogd/core/schemas/games/PerCountSchema.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/core/schemas/table_schemas/BIGQUERY.json` & `opengamedata_core-0.0.3/src/ogd/core/schemas/table_schemas/BIGQUERY.json`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/core/schemas/table_schemas/FIELDDAY_MYSQL.json` & `opengamedata_core-0.0.3/src/ogd/core/schemas/table_schemas/FIELDDAY_MYSQL.json`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/core/schemas/table_schemas/FIREBASE.json` & `opengamedata_core-0.0.3/src/ogd/core/schemas/table_schemas/FIREBASE.json`

 * *Files 14% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9910714285714286%*

 * *Differences: {"'column_map'": "{'user_data': 'geo'}"}*

```diff
@@ -8,15 +8,15 @@
         "event_sequence_index": null,
         "event_source": null,
         "game_state": null,
         "log_version": "log_version",
         "session_id": "session_id",
         "time_offset": null,
         "timestamp": "timestamp",
-        "user_data": null,
+        "user_data": "geo",
         "user_id": "fd_user_id"
     },
     "columns": [
         {
             "description": "The name of the event",
             "name": "event_name",
             "readable": "Event Name",
```

### Comparing `opengamedata_core-0.0.2/src/ogd/core/schemas/table_schemas/MASHOPOLIS_MYSQL.json` & `opengamedata_core-0.0.3/src/ogd/core/schemas/table_schemas/MASHOPOLIS_MYSQL.json`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/core/schemas/table_schemas/OGD_EVENT_FILE.json` & `opengamedata_core-0.0.3/src/ogd/core/schemas/table_schemas/OGD_EVENT_FILE.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9955357142857143%*

 * *Differences: {"'columns'": "{6: {'type': 'str'}, 8: {'type': 'str'}}"}*

```diff
@@ -52,27 +52,27 @@
             "readable": "Event Source",
             "type": "enum('GAME', 'GENERATED')"
         },
         {
             "description": "The version of the game from which the event came",
             "name": "app_version",
             "readable": "App Version",
-            "type": "int"
+            "type": "str"
         },
         {
             "description": "The branch of the game from which the event came",
             "name": "app_branch",
             "readable": "App Branch",
             "type": "str"
         },
         {
             "description": "The version of the logging code for the game from which the event came",
             "name": "log_version",
             "readable": "Log Version",
-            "type": "int"
+            "type": "str"
         },
         {
             "description": "The local offset of the event time from GMT",
             "name": "offset",
             "readable": "Time Offset",
             "type": "timedelta"
         },
```

### Comparing `opengamedata_core-0.0.2/src/ogd/core/schemas/table_schemas/OPENGAMEDATA_BIGQUERY.json` & `opengamedata_core-0.0.3/src/ogd/core/schemas/table_schemas/OPENGAMEDATA_BIGQUERY.json`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/core/schemas/table_schemas/OPENGAMEDATA_MYSQL.json` & `opengamedata_core-0.0.3/src/ogd/core/schemas/table_schemas/OPENGAMEDATA_MYSQL.json`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/core/schemas/table_schemas/SHIPWRECKS.json` & `opengamedata_core-0.0.3/src/ogd/core/schemas/table_schemas/SHIPWRECKS.json`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/core/schemas/tables/ColumnMapSchema.py` & `opengamedata_core-0.0.3/src/ogd/core/schemas/tables/ColumnMapSchema.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/core/schemas/tables/ColumnSchema.py` & `opengamedata_core-0.0.3/src/ogd/core/schemas/tables/ColumnSchema.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/core/schemas/tables/TableSchema.py` & `opengamedata_core-0.0.3/src/ogd/core/schemas/tables/TableSchema.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/core/utils/Logger.py` & `opengamedata_core-0.0.3/src/ogd/core/utils/Logger.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/core/utils/Readme.py` & `opengamedata_core-0.0.3/src/ogd/core/utils/Readme.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/core/utils/utils.py` & `opengamedata_core-0.0.3/src/ogd/core/utils/utils.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/ALL_YOU_CAN_ET/schemas/ALL_YOU_CAN_ET.json.template` & `opengamedata_core-0.0.3/src/ogd/games/ALL_YOU_CAN_ET/schemas/ALL_YOU_CAN_ET.json.template`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/AQUALAB/AqualabLoader.py` & `opengamedata_core-0.0.3/src/ogd/games/AQUALAB/AqualabLoader.py`

 * *Files 7% similar despite different names*

```diff
@@ -70,97 +70,117 @@
     def _loadFeature(self, feature_type:str, extractor_params:GeneratorParameters, schema_args:Dict[str,Any]) -> Feature:
         ret_val : Feature
         # First run through aggregate features
         if extractor_params._count_index == None:
             match feature_type:
                 case "ActiveTime":
                     ret_val = ActiveTime.ActiveTime(params=extractor_params, job_map=self._job_map, active_threads=schema_args.get("Active_threshold"))
-                case "JobTriesInArgument":
-                    ret_val = JobTriesInArgument.JobTriesInArgument(params=extractor_params, job_map=self._job_map)
-                case "ModelInterveneCount":
-                    ret_val = ModelInterveneCount.ModelInterveneCount(params=extractor_params, job_map=self._job_map)
-                case "TankRulesCount":
-                    ret_val = TankRulesCount.TankRulesCount(params=extractor_params)
-                case "ModelExportCount":
-                    ret_val = ModelExportCount.ModelExportCount(params=extractor_params, job_map=self._job_map)
-                case "ModelPredictCount":
-                    ret_val = ModelPredictCount.ModelPredictCount(params=extractor_params, job_map=self._job_map)
-                case "UserAvgActiveTime":
-                    ret_val = UserAvgActiveTime.UserAvgActiveTime(params=extractor_params, player_id=self._player_id)
                 case "ActiveJobs":
                     ret_val = ActiveJobs.ActiveJobs(params=extractor_params, job_map=self._job_map)
+                case "AppVersions":
+                    ret_val = AppVersions.AppVersions(params=extractor_params)
                 case "EchoSessionID":
                     ret_val = EchoSessionID.EchoSessionID(params=extractor_params)
                 case "EventList":
                     ret_val = EventList.EventList(params=extractor_params)
                 case "JobsCompleted":
                     ret_val = JobsCompleted.JobsCompleted(params=extractor_params, player_id=self._player_id)
+                case "JobTriesInArgument":
+                    ret_val = JobTriesInArgument.JobTriesInArgument(params=extractor_params, job_map=self._job_map)
+                case "ModelExportCount":
+                    ret_val = ModelExportCount.ModelExportCount(params=extractor_params, job_map=self._job_map)
+                case "ModelInterveneCount":
+                    ret_val = ModelInterveneCount.ModelInterveneCount(params=extractor_params, job_map=self._job_map)
+                case "ModelPredictCount":
+                    ret_val = ModelPredictCount.ModelPredictCount(params=extractor_params, job_map=self._job_map)
+                # case "PlayLocations":
+                #     ret_val = PlayLocations.PlayLocations(params=extractor_params)
                 case "PlayerSummary":
                     ret_val = PlayerSummary.PlayerSummary(params=extractor_params)
                 case "PopulationSummary":
                     ret_val = PopulationSummary.PopulationSummary(params=extractor_params)
                 case "SessionDiveSitesCount":
                     ret_val = SessionDiveSitesCount.SessionDiveSitesCount(params=extractor_params)
                 case "SessionDuration":
-                    ret_val = SessionDuration.SessionDuration(params=extractor_params, session_id=self._session_id)
+                    ret_val = SessionDuration.SessionDuration(params=extractor_params, threshold=int(schema_args.get("threshold", 60)))
                 case "SessionGuideCount":
                     ret_val = SessionGuideCount.SessionGuideCount(params=extractor_params)
                 case "SessionHelpCount":
                     ret_val = SessionHelpCount.SessionHelpCount(params=extractor_params)
                 case "SessionID":
                     ret_val = SessionID.SessionID(params=extractor_params, session_id=self._session_id)
                 case "SessionJobsCompleted":
                     ret_val = SessionJobsCompleted.SessionJobsCompleted(params=extractor_params)
                 case "SwitchJobsCount":
                     ret_val = SwitchJobsCount.SwitchJobsCount(params=extractor_params)
+                case "TankRulesCount":
+                    ret_val = TankRulesCount.TankRulesCount(params=extractor_params)
                 case "TopJobCompletionDestinations":
                     ret_val = TopJobCompletionDestinations.TopJobCompletionDestinations(params=extractor_params, job_map=self._job_map)
                 case "TopJobSwitchDestinations":
                     ret_val = TopJobSwitchDestinations.TopJobSwitchDestinations(params=extractor_params, job_map=self._job_map)
                 case "TotalArgumentationTime":
                     ret_val = TotalArgumentationTime.TotalArgumentationTime(params=extractor_params)
                 case "TotalDiveTime":
                     ret_val = TotalDiveTime.TotalDiveTime(params=extractor_params)
                 case "TotalExperimentationTime":
                     ret_val = TotalExperimentationTime.TotalExperimentationTime(params=extractor_params)
+                case "TotalGuideCount":
+                    ret_val = TotalGuideCount.TotalGuideCount(params=extractor_params)
+                case "TotalHelpCount":
+                    ret_val = TotalHelpCount.TotalHelpCount(params=extractor_params)
+                case "TotalModelingTime":
+                    ret_val = TotalModelingTime.TotalModelingTime(params=extractor_params)
+                case "TotalPlayTime":
+                    ret_val = TotalPlayTime.TotalPlayTime(params=extractor_params)
+                case "UserAvgActiveTime":
+                    ret_val = UserAvgActiveTime.UserAvgActiveTime(params=extractor_params, player_id=self._player_id)
                 case "UserAvgSessionDuration":
                     ret_val = UserAvgSessionDuration.UserAvgSessionDuration(params=extractor_params, player_id=self._player_id)
                 case "UserTotalSessionDuration":
                     ret_val = UserTotalSessionDuration.UserTotalSessionDuration(params=extractor_params, player_id=self._player_id)
                 case _:
                     raise NotImplementedError(f"'{feature_type}' is not a valid aggregate feature type for Aqualab.")
         # then run through per-count features.
         else:
             match feature_type:
                 case "JobActiveTime":
                     ret_val = JobActiveTime.JobActiveTime(params=extractor_params, job_map=self._job_map)
-                case "JobArgumentationTime":
-                    ret_val = JobArgumentationTime.JobArgumentationTime(params=extractor_params, job_map=self._job_map)
+                case "JobArgumentation":
+                    ret_val = JobArgumentation.JobArgumentation(params=extractor_params, job_map=self._job_map)
                 case "JobCompletionTime":
                     ret_val = JobCompletionTime.JobCompletionTime(params=extractor_params, job_map=self._job_map)
                 case "JobDiveSitesCount":
                     ret_val = JobDiveSitesCount.JobDiveSitesCount(params=extractor_params, job_map=self._job_map)
                 case "JobDiveTime":
                     ret_val = JobDiveTime.JobDiveTime(params=extractor_params, job_map=self._job_map)
-                case "JobExperimentationTime":
-                    ret_val = JobExperimentationTime.JobExperimentationTime(params=extractor_params, job_map=self._job_map)
+                case "JobExperimentation":
+                    ret_val = JobExperimentation.JobExperimentation(params=extractor_params, job_map=self._job_map)
                 case "JobGuideCount":
                     ret_val = JobGuideCount.JobGuideCount(params=extractor_params, job_map=self._job_map)
                 case "JobHelpCount":
                     ret_val = JobHelpCount.JobHelpCount(params=extractor_params, job_map=self._job_map)
                 case "JobLocationChanges":
                     ret_val = JobLocationChanges.JobLocationChanges(params=extractor_params, job_map=self._job_map)
-                case "JobModelingTime":
-                    ret_val = JobModelingTime.JobModelingTime(params=extractor_params, job_map=self._job_map)
+                case "JobModeling":
+                    ret_val = JobModeling.JobModeling(params=extractor_params, job_map=self._job_map)
+                case "JobPriorAttempt":
+                    ret_val = JobPriorAttempt.JobPriorAttempt(params=extractor_params, job_map=self._job_map)
+                case "JobPriorComplete":
+                    ret_val = JobPriorComplete.JobPriorComplete(params=extractor_params, job_map=self._job_map)
                 case "JobStartCount":
                     ret_val = JobStartCount.JobStartCount(params=extractor_params, job_map=self._job_map)
                 case "JobTasksCompleted":
                     ret_val = JobTasksCompleted.JobTasksCompleted(params=extractor_params, job_map=self._job_map)
                 case "JobsAttempted":
                     ret_val = JobsAttempted.JobsAttempted(params=extractor_params, job_map=self._job_map, diff_map=self._diff_map)
+                case "RegionName":
+                    ret_val = RegionName.RegionName(params=extractor_params)
+                case "RegionJobCount":
+                    ret_val = RegionJobCount.RegionJobCount(params=extractor_params)
                 case "SyncCompletionTime":
                     ret_val = SyncCompletionTime.SyncCompletionTime(params=extractor_params)
                 case _:
                     raise NotImplementedError(f"'{feature_type}' is not a valid per-count feature type for Aqualab.")
         return ret_val
 
     def _loadDetector(self, detector_type:str, extractor_params:GeneratorParameters, schema_args:Dict[str,Any], trigger_callback:Callable[[Event], None]) -> Detector:
```

### Comparing `opengamedata_core-0.0.2/src/ogd/games/AQUALAB/DBExport.json` & `opengamedata_core-0.0.3/src/ogd/games/AQUALAB/DBExport.json`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/AQUALAB/detectors/CollectFactNoJob.py` & `opengamedata_core-0.0.3/src/ogd/games/AQUALAB/detectors/CollectFactNoJob.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/AQUALAB/detectors/DiveSiteNoEvidence.py` & `opengamedata_core-0.0.3/src/ogd/games/AQUALAB/detectors/DiveSiteNoEvidence.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/AQUALAB/detectors/EchoRoomChange.py` & `opengamedata_core-0.0.3/src/ogd/games/AQUALAB/detectors/EchoRoomChange.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/AQUALAB/detectors/HintAndLeave.py` & `opengamedata_core-0.0.3/src/ogd/games/AQUALAB/detectors/HintAndLeave.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/AQUALAB/detectors/Idle.py` & `opengamedata_core-0.0.3/src/ogd/games/AQUALAB/detectors/Idle.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/AQUALAB/detectors/SceneChangeFrequently.py` & `opengamedata_core-0.0.3/src/ogd/games/AQUALAB/detectors/SceneChangeFrequently.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/AQUALAB/detectors/TwoHints.py` & `opengamedata_core-0.0.3/src/ogd/games/AQUALAB/detectors/TwoHints.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/AQUALAB/features/ActiveJobs.py` & `opengamedata_core-0.0.3/src/ogd/games/AQUALAB/features/ActiveJobs.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/AQUALAB/features/ActiveTime.py` & `opengamedata_core-0.0.3/src/ogd/games/AQUALAB/features/ActiveTime.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,16 +33,16 @@
         return []
 
     def _updateFromEvent(self, event:Event) -> None:
         if not self._client_start_time:
             self._client_start_time = event.Timestamp
         self._client_end_time = event.Timestamp
         
-        if event.EventName != "Idle":
-            return
+        # if event.EventName != "Idle":
+        #     return
 
         if not self.active_level:
             self.active_level = event.EventData.get("level")
         else:
             if self.active_level != event.EventData.get("level"):
                 warnings.warn("The idle event has a different threshold!")
                 return
```

### Comparing `opengamedata_core-0.0.2/src/ogd/games/AQUALAB/features/EchoSessionID.py` & `opengamedata_core-0.0.3/src/ogd/games/AQUALAB/features/EchoSessionID.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/AQUALAB/features/EventList.py` & `opengamedata_core-0.0.3/src/ogd/games/AQUALAB/features/EventList.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/AQUALAB/features/JobActiveTime.py` & `opengamedata_core-0.0.3/src/ogd/games/AQUALAB/features/JobActiveTime.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,14 +18,17 @@
         if self.ExtractionMode == ExtractionMode.PLAYER:
             self._session_id      = None
             self._last_start_time = None
             self._last_event_time = None
             self._last_event_session = None
             self._last_event_name = None
             self._last_event_index = None
+            self._last_event_session = None
+            self._last_event_name = None
+            self._last_event_index = None
         else:
             raise NotImplementedError(f"Got invalid export mode of {self.ExtractionMode.name} in JobActiveTime!")
 
     # *** IMPLEMENT ABSTRACT FUNCTIONS ***
     @classmethod
     def _eventFilter(cls, mode:ExtractionMode) -> List[str]:
         return ["all_events"]
```

### Comparing `opengamedata_core-0.0.2/src/ogd/games/AQUALAB/features/JobArgumentationTime.py` & `opengamedata_core-0.0.3/src/ogd/games/AQUALAB/features/JobArgumentation.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,19 +6,20 @@
 from ogd.core.utils.Logger import Logger
 from ogd.core.generators.Generator import GeneratorParameters
 from ogd.games.AQUALAB.features.PerJobFeature import PerJobFeature
 from ogd.core.schemas.Event import Event
 from ogd.core.schemas.ExtractionMode import ExtractionMode
 from ogd.core.schemas.FeatureData import FeatureData
 
-class JobArgumentationTime(PerJobFeature):
+class JobArgumentation(PerJobFeature):
 
     def __init__(self, params:GeneratorParameters, job_map:dict):
         super().__init__(params=params, job_map=job_map)
         self._session_id = None
+        self._argumentation_start_count : int = 0
         self._argument_start_time : Optional[datetime] = None
         self._prev_timestamp = None
         self._time = 0
 
     # *** IMPLEMENT ABSTRACT FUNCTIONS ***
     @classmethod
     def _eventFilter(cls, mode:ExtractionMode) -> List[str]:
@@ -33,24 +34,30 @@
             self._session_id = event.SessionID
             # if we jumped to a new session, we only want to count time up to last event, not the time between sessions.
             if self._argument_start_time and self._prev_timestamp:
                 self._time += (self._prev_timestamp - self._argument_start_time).total_seconds()
                 self._argument_start_time = event.Timestamp
 
         if event.EventName == "begin_argument":
+            self._argumentation_start_count += 1
             self._argument_start_time = event.Timestamp
-        elif event.EventName == "room_changed" and self._argument_start_time is not None:
-            self._time += (event.Timestamp - self._argument_start_time).total_seconds()
-            self._argument_start_time = None
+        elif event.EventName in ["room_changed", "leave_argument", "complete_argument"]:
+            if self._argument_start_time is not None:
+                self._time += (event.Timestamp - self._argument_start_time).total_seconds()
+                self._argument_start_time = None
         
         self._prev_timestamp = event.Timestamp
     
     def _updateFromFeatureData(self, feature:FeatureData):
         return
 
     def _getFeatureValues(self) -> List[Any]:
-        return [timedelta(seconds=self._time)]
+        return [self._argumentation_start_count, timedelta(seconds=self._time)]
 
     # *** Optionally override public functions. ***
+
+    def Subfeatures(self) -> List[str]:
+        return ["Time"]
+
     @staticmethod
     def MinVersion() -> Optional[str]:
         return "1"
```

### Comparing `opengamedata_core-0.0.2/src/ogd/games/AQUALAB/features/JobCompletionTime.py` & `opengamedata_core-0.0.3/src/ogd/games/AQUALAB/features/JobCompletionTime.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/AQUALAB/features/JobDiveSitesCount.py` & `opengamedata_core-0.0.3/src/ogd/games/AQUALAB/features/JobDiveSitesCount.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/AQUALAB/features/JobDiveTime.py` & `opengamedata_core-0.0.3/src/ogd/games/AQUALAB/features/JobDiveTime.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/AQUALAB/features/JobExperimentationTime.py` & `opengamedata_core-0.0.3/src/ogd/games/AQUALAB/features/JobExperimentation.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,19 +7,20 @@
 from ogd.core.utils.Logger import Logger
 from ogd.core.generators.Generator import GeneratorParameters
 from ogd.games.AQUALAB.features.PerJobFeature import PerJobFeature
 from ogd.core.schemas.Event import Event
 from ogd.core.schemas.ExtractionMode import ExtractionMode
 from ogd.core.schemas.FeatureData import FeatureData
 
-class JobExperimentationTime(PerJobFeature):
+class JobExperimentation(PerJobFeature):
 
     def __init__(self, params:GeneratorParameters, job_map:dict):
         super().__init__(params=params, job_map=job_map)
         self._session_id = None
+        self._experiment_start_count : int = 0
         self._experiment_start_time = None
         self._prev_timestamp = None
         self._time = 0
 
     # *** IMPLEMENT ABSTRACT FUNCTIONS ***
     @classmethod
     def _eventFilter(cls, mode:ExtractionMode) -> List[str]:
@@ -34,25 +35,30 @@
             self._session_id = event.SessionID
             # if we jumped to a new session, we only want to count time up to last event, not the time between sessions.
             if self._experiment_start_time and self._prev_timestamp:
                 self._time += (self._prev_timestamp - self._experiment_start_time).total_seconds()
                 self._experiment_start_time = event.Timestamp
 
         if event.EventName == "begin_experiment":
+            self._experiment_start_count += 1
             self._experiment_start_time = event.Timestamp
-        elif event.EventName == "room_changed":
+        elif event.EventName in ["room_changed", "end_experiment"]:
             if self._experiment_start_time is not None:
                 self._time += (event.Timestamp - self._experiment_start_time).total_seconds()
                 self._experiment_start_time = None
 
         self._prev_timestamp = event.Timestamp
 
     def _updateFromFeatureData(self, feature:FeatureData):
         return
 
     def _getFeatureValues(self) -> List[Any]:
-        return [timedelta(seconds=self._time)]
+        return [self._experiment_start_count, timedelta(seconds=self._time)]
 
     # *** Optionally override public functions. ***
+
+    def Subfeatures(self) -> List[str]:
+        return ["Time"]
+
     @staticmethod
     def MinVersion() -> Optional[str]:
         return "1"
```

### Comparing `opengamedata_core-0.0.2/src/ogd/games/AQUALAB/features/JobGuideCount.py` & `opengamedata_core-0.0.3/src/ogd/games/AQUALAB/features/JobGuideCount.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/AQUALAB/features/JobHelpCount.py` & `opengamedata_core-0.0.3/src/ogd/games/AQUALAB/features/JobHelpCount.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/AQUALAB/features/JobLocationChanges.py` & `opengamedata_core-0.0.3/src/ogd/games/AQUALAB/features/JobLocationChanges.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/AQUALAB/features/JobModelingTime.py` & `opengamedata_core-0.0.3/src/ogd/games/AQUALAB/features/JobModeling.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,52 +6,58 @@
 from ogd.core.utils.Logger import Logger
 from ogd.core.generators.Generator import GeneratorParameters
 from ogd.games.AQUALAB.features.PerJobFeature import PerJobFeature
 from ogd.core.schemas.Event import Event
 from ogd.core.schemas.ExtractionMode import ExtractionMode
 from ogd.core.schemas.FeatureData import FeatureData
 
-class JobModelingTime(PerJobFeature):
+class JobModeling(PerJobFeature):
     def __init__(self, params:GeneratorParameters, job_map:dict):
         self._job_map = job_map
         super().__init__(params=params, job_map=job_map)
         self._session_id = None
+        self._modeling_start_count : int = 0
         self._modeling_start_time = None
         self._prev_timestamp = None
         self._time = 0
 
     # *** IMPLEMENT ABSTRACT FUNCTIONS ***
     @classmethod
     def _eventFilter(cls, mode:ExtractionMode) -> List[str]:
-        return []
+        return ["all_events"]
 
     @classmethod
     def _featureFilter(cls, mode:ExtractionMode) -> List[str]:
         return []
 
     def _updateFromEvent(self, event:Event) -> None:
         if event.SessionID != self._session_id:
             self._session_id = event.SessionID
 
             if self._modeling_start_time and self._prev_timestamp:
                 self._time += (self._prev_timestamp - self._modeling_start_time).total_seconds()
                 self._modeling_start_time = event.Timestamp
 
-        if event.EventName == "begin_modeling":
+        if event.EventName == "begin_model":
+            self._modeling_start_count += 1
             self._modeling_start_time = event.Timestamp
-        elif event.EventName == "room_changed":
+        elif event.EventName in ["room_changed", "end_model"]:
             if self._modeling_start_time is not None:
                 self._time += (event.Timestamp - self._modeling_start_time).total_seconds()
                 self._modeling_start_time = None
 
         self._prev_timestamp = event.Timestamp
 
     def _updateFromFeatureData(self, feature:FeatureData):
         return
 
     def _getFeatureValues(self) -> List[Any]:
-        return [timedelta(seconds=self._time)]
+        return [self._modeling_start_count, timedelta(seconds=self._time)]
 
     # *** Optionally override public functions. ***
+
+    def Subfeatures(self) -> List[str]:
+        return ["Time"]
+
     @staticmethod
     def MinVersion() -> Optional[str]:
         return "1"
```

### Comparing `opengamedata_core-0.0.2/src/ogd/games/AQUALAB/features/JobPlayTime.py` & `opengamedata_core-0.0.3/src/ogd/games/AQUALAB/features/JobPlayTime.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/AQUALAB/features/JobStartCount.py` & `opengamedata_core-0.0.3/src/ogd/games/AQUALAB/features/JobStartCount.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/AQUALAB/features/JobTasksCompleted.py` & `opengamedata_core-0.0.3/src/ogd/games/AQUALAB/features/JobTasksCompleted.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/AQUALAB/features/JobTriesInArgument.py` & `opengamedata_core-0.0.3/src/ogd/games/AQUALAB/features/JobTriesInArgument.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/AQUALAB/features/JobsAttempted.py` & `opengamedata_core-0.0.3/src/ogd/games/AQUALAB/features/JobsAttempted.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/AQUALAB/features/JobsCompleted.py` & `opengamedata_core-0.0.3/src/ogd/games/AQUALAB/features/UserAvgSessionDuration.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,36 +1,42 @@
+# import libraries
 from typing import Any, List
-
+# import locals
 from ogd.core.generators.Generator import GeneratorParameters
 from ogd.core.generators.extractors.SessionFeature import SessionFeature
 from ogd.core.schemas.Event import Event
 from ogd.core.schemas.ExtractionMode import ExtractionMode
 from ogd.core.schemas.FeatureData import FeatureData
 
-class JobsCompleted(SessionFeature):
+class UserAvgSessionDuration(SessionFeature):
 
     def __init__(self, params:GeneratorParameters, player_id:str):
         self._player_id = player_id
         super().__init__(params=params)
-        self._jobs_completed = []
+        self._times : List[int] = []
 
     # *** IMPLEMENT ABSTRACT FUNCTIONS ***
     @classmethod
     def _eventFilter(cls, mode:ExtractionMode) -> List[str]:
-        return ["complete_job"]
+        return []
 
     @classmethod
     def _featureFilter(cls, mode:ExtractionMode) -> List[str]:
-        return []
+        return ["SessionDuration"]
 
-    def _updateFromEvent(self, event: Event) -> None:
-        if event.UserID == self._player_id:
-            _job_name = event.GameState.get('job_name', event.EventData.get('job_name', "JOB NAME NOT FOUND"))
-            self._jobs_completed.append(_job_name)
+    def _updateFromEvent(self, event:Event) -> None:
+        return
 
     def _updateFromFeatureData(self, feature:FeatureData):
-        return
+        if feature.PlayerID == self._player_id:
+            if feature.FeatureValues[0] == "No events":
+                pass
+            else:
+                self._times.append(feature.FeatureValues[0].total_seconds())
 
     def _getFeatureValues(self) -> List[Any]:
-        return [self._jobs_completed]
+        if len(self._times) > 0:
+            return [sum(self._times) / len(self._times)]
+        else:
+            return [0]
 
     # *** Optionally override public functions. ***
```

### Comparing `opengamedata_core-0.0.2/src/ogd/games/AQUALAB/features/ModelExportCount.py` & `opengamedata_core-0.0.3/src/ogd/games/AQUALAB/features/ModelExportCount.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/AQUALAB/features/ModelInterveneCount.py` & `opengamedata_core-0.0.3/src/ogd/games/AQUALAB/features/ModelInterveneCount.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/AQUALAB/features/ModelPredictCount.py` & `opengamedata_core-0.0.3/src/ogd/games/AQUALAB/features/ModelPredictCount.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/AQUALAB/features/PerJobFeature.py` & `opengamedata_core-0.0.3/src/ogd/games/AQUALAB/features/PerJobFeature.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/AQUALAB/features/PlayerSummary.py` & `opengamedata_core-0.0.3/src/ogd/games/AQUALAB/features/PlayerSummary.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/AQUALAB/features/PopulationSummary.py` & `opengamedata_core-0.0.3/src/ogd/games/AQUALAB/features/PopulationSummary.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/AQUALAB/features/SessionDiveSitesCount.py` & `opengamedata_core-0.0.3/src/ogd/games/AQUALAB/features/SessionDiveSitesCount.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/AQUALAB/features/SessionGuideCount.py` & `opengamedata_core-0.0.3/src/ogd/games/AQUALAB/features/SessionGuideCount.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/AQUALAB/features/SessionHelpCount.py` & `opengamedata_core-0.0.3/src/ogd/games/AQUALAB/features/SessionHelpCount.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/AQUALAB/features/SessionID.py` & `opengamedata_core-0.0.3/src/ogd/games/AQUALAB/features/SessionID.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/AQUALAB/features/SessionJobsCompleted.py` & `opengamedata_core-0.0.3/src/ogd/games/AQUALAB/features/SessionJobsCompleted.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/AQUALAB/features/SwitchJobsCount.py` & `opengamedata_core-0.0.3/src/ogd/games/AQUALAB/features/SwitchJobsCount.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/AQUALAB/features/SyncCompletionTime.py` & `opengamedata_core-0.0.3/src/ogd/games/AQUALAB/features/SyncCompletionTime.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/AQUALAB/features/TankRulesCount.py` & `opengamedata_core-0.0.3/src/ogd/games/AQUALAB/features/TankRulesCount.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/AQUALAB/features/TopJobCompletionDestinations.py` & `opengamedata_core-0.0.3/src/ogd/games/AQUALAB/features/TopJobCompletionDestinations.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/AQUALAB/features/TopJobSwitchDestinations.py` & `opengamedata_core-0.0.3/src/ogd/games/AQUALAB/features/TopJobSwitchDestinations.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/AQUALAB/features/TotalArgumentationTime.py` & `opengamedata_core-0.0.3/src/ogd/games/PENGUINS/features/SnowBallDuration.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,52 +1,53 @@
 # import libraries
-from datetime import timedelta
-from typing import Any, List
+import logging
+from typing import Any, Dict, List, Optional
 # import locals
+from ogd.core.utils.Logger import Logger
+from datetime import datetime, timedelta
 from ogd.core.generators.Generator import GeneratorParameters
 from ogd.core.generators.extractors.Feature import Feature
+from ogd.games.PENGUINS.features.PerRegionFeature import PerRegionFeature
 from ogd.core.schemas.Event import Event
 from ogd.core.schemas.ExtractionMode import ExtractionMode
 from ogd.core.schemas.FeatureData import FeatureData
+from ogd.core.generators.extractors.SessionFeature import SessionFeature
+
+class SnowBallDuration(SessionFeature):
 
-class TotalArgumentationTime(Feature):
-    
     def __init__(self, params:GeneratorParameters):
         super().__init__(params=params)
         self._session_id = None
-        self._argue_start_time = None
+        self._argument_start_time : Optional[datetime] = None
         self._prev_timestamp = None
         self._time = 0
 
     # *** IMPLEMENT ABSTRACT FUNCTIONS ***
     @classmethod
     def _eventFilter(cls, mode:ExtractionMode) -> List[str]:
-        return ["begin_argument", "room_changed"]
+        return ["push_snowball"]
 
     @classmethod
     def _featureFilter(cls, mode:ExtractionMode) -> List[str]:
         return []
 
     def _updateFromEvent(self, event:Event) -> None:
         if event.SessionID != self._session_id:
             self._session_id = event.SessionID
-
-            if self._argue_start_time:
-                self._time += (self._prev_timestamp - self._argue_start_time).total_seconds()
-                self._argue_start_time = event.Timestamp
-
-        if event.EventName == "begin_argument":
-            self._argue_start_time = event.Timestamp
-        elif event.EventName == "room_changed":
-            if self._argue_start_time is not None:
-                self._time += (event.Timestamp - self._argue_start_time).total_seconds()
-                self._argue_start_time = None
-
+            # if we jumped to a new session, we only want to count time up to last event, not the time between sessions.
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
+
```

### Comparing `opengamedata_core-0.0.2/src/ogd/games/AQUALAB/features/TotalDiveTime.py` & `opengamedata_core-0.0.3/src/ogd/games/JOWILDER/features/SessionStart.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,52 +1,58 @@
 # import libraries
-from datetime import timedelta
-from typing import Any, List
-# import locals
+from typing import Any, List, Optional
 from ogd.core.generators.Generator import GeneratorParameters
-from ogd.core.generators.extractors.Feature import Feature
-from ogd.core.schemas.Event import Event
+from datetime import date, datetime, time
+# import local files
+from ogd.core.generators.extractors.SessionFeature import SessionFeature
 from ogd.core.schemas.ExtractionMode import ExtractionMode
 from ogd.core.schemas.FeatureData import FeatureData
+from ogd.core.schemas.Event import Event
 
-class TotalDiveTime(Feature):
-    
+class SessionStart(SessionFeature):
+    """Template file to serve as a guide for creating custom Feature subclasses for games.
+
+    :param Feature: Base class for a Custom Feature class.
+    :type Feature: _type_
+    """
     def __init__(self, params:GeneratorParameters):
         super().__init__(params=params)
-        self._session_id = None
-        self._dive_start_time = None
-        self._prev_timestamp = None
-        self._time = 0
+        self._date : Optional[date] = None
+        self._time : Optional[time] = None
+        self._year : Optional[int] = None
+        self._month : Optional[int] = None
+        self._hour : Optional[int] = None
 
     # *** IMPLEMENT ABSTRACT FUNCTIONS ***
+
     @classmethod
     def _eventFilter(cls, mode:ExtractionMode) -> List[str]:
-        return ["begin_dive", "scene_changed"]
+        return ["CUSTOM.1"]
 
     @classmethod
     def _featureFilter(cls, mode:ExtractionMode) -> List[str]:
-        return []
+        return [] 
 
     def _updateFromEvent(self, event:Event) -> None:
-        if event.SessionID != self._session_id:
-            self._session_id = event.SessionID
+        event_time = event.Timestamp
+        if not self._date:
+            self._date = event_time.date()
+            self._time = event_time.time()
+            self._hour = event_time.hour
+            self._year = event_time.year
+            self._month = event_time.month
 
-            if self._dive_start_time:
-                self._time += (self._prev_timestamp - self._dive_start_time).total_seconds()
-                self._dive_start_time = event.Timestamp
-
-        if event.EventName == "begin_dive":
-            self._dive_start_time = event.Timestamp
-        elif event.EventName == "scene_changed":
-            if self._dive_start_time is not None:
-                self._time += (event.Timestamp - self._dive_start_time).total_seconds()
-                self._dive_start_time = None
 
-        self._prev_timestamp = event.Timestamp
+        return
 
-    def _updateFromFeatureData(self, feature:FeatureData):
+    def _updateFromFeatureData(self, feature: FeatureData):
         return
 
     def _getFeatureValues(self) -> List[Any]:
-        return [timedelta(seconds=self._time)]
+        return [self._date, self._time, self._year, self._month, self._hour]
+
+    def Subfeatures(self) -> List[str]:
+        return ["Time", "Year", "Month", "Hour"]
+
+    def BaseFeatureSuffix(self) -> str:
+        return "Date"
 
-    # *** Optionally override public functions. ***
```

### Comparing `opengamedata_core-0.0.2/src/ogd/games/AQUALAB/features/TotalExperimentationTime.py` & `opengamedata_core-0.0.3/src/ogd/games/AQUALAB/features/TotalDiveTime.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,52 +1,69 @@
 # import libraries
 from datetime import timedelta
 from typing import Any, List
 # import locals
 from ogd.core.generators.Generator import GeneratorParameters
 from ogd.core.generators.extractors.Feature import Feature
-from ogd.core.schemas.Event import Event
+from ogd.core.schemas.Event import Event, EventSource
 from ogd.core.schemas.ExtractionMode import ExtractionMode
 from ogd.core.schemas.FeatureData import FeatureData
 
-class TotalExperimentationTime(Feature):
-
+class TotalDiveTime(Feature):
+    
     def __init__(self, params:GeneratorParameters):
         super().__init__(params=params)
-        self._session_id = None
-        self._experiment_start_time = None
-        self._prev_timestamp = None
-        self._time = 0
+        self.prev_time = timedelta(0)
+        self.total_time = timedelta(0)
+        self.idle_time = timedelta(0)
+        self.on = False
 
+    def Subfeatures(self) -> List[str]: 
+        return ["Seconds", "Active", "Active-Seconds", "Idle", "Idle-Seconds"]
     # *** IMPLEMENT ABSTRACT FUNCTIONS ***
     @classmethod
     def _eventFilter(cls, mode:ExtractionMode) -> List[str]:
-        return ["begin_experiment", "room_changed"]
+        return ["begin_dive", "scene_changed", "end_dive"]
 
     @classmethod
     def _featureFilter(cls, mode:ExtractionMode) -> List[str]:
         return []
 
     def _updateFromEvent(self, event:Event) -> None:
-        if event.SessionID != self._session_id:
-            self._session_id = event.SessionID
-
-            if self._experiment_start_time:
-                self._time += (self._prev_timestamp - self._experiment_start_time).total_seconds()
-                self._experiment_start_time = event.Timestamp
-
-        if event.EventName == "begin_experiment":
-            self._experiment_start_time = event.Timestamp
-        elif event.EventName == "room_changed":
-            if self._experiment_start_time is not None:
-                self._time += (event.Timestamp - self._experiment_start_time).total_seconds()
-                self._experiment_start_time = None
+        if event.EventSource == EventSource.GAME:
+            if self.on:
+                self.total_time += (event.Timestamp - self.prev_time)
+                if (event.Timestamp - self.prev_time) > timedelta(minutes=1):
+                    self.idle_time += (event.Timestamp - self.prev_time)
+                if event.EventName == 'end_dive':
+                    self.on = False
+            else:
+                if event.EventName == "begin_dive":
+                    self.on = True
+            self.prev_time = event.Timestamp
+       
+        # if event.SessionID != self._session_id:
+        #     self._session_id = event.SessionID
+
+        #     if self._dive_start_time:
+        #         self._time += (self._prev_timestamp - self._dive_start_time).total_seconds()
+        #         self._dive_start_time = event.Timestamp
+
+        # if event.EventName == "begin_dive":
+        #     self._dive_start_time = event.Timestamp
+        # elif event.EventName == "scene_changed":
+        #     if self._dive_start_time is not None:
+        #         self._time += (event.Timestamp - self._dive_start_time).total_seconds()
+        #         self._dive_start_time = None
 
-        self._prev_timestamp = event.Timestamp
+        # self._prev_timestamp = event.Timestamp
 
     def _updateFromFeatureData(self, feature:FeatureData):
         return
 
     def _getFeatureValues(self) -> List[Any]:
-        return [timedelta(seconds=self._time)]
+        if self.total_time is not None:
+            return [self.total_time, self.total_time.total_seconds(), (self.total_time - self.idle_time), (self.total_time - self.idle_time).total_seconds(), self.idle_time, self.idle_time.total_seconds()]
+        else:
+            return ["No events"]
 
     # *** Optionally override public functions. ***
```

### Comparing `opengamedata_core-0.0.2/src/ogd/games/AQUALAB/features/UserAvgActiveTime.py` & `opengamedata_core-0.0.3/src/ogd/games/AQUALAB/features/UserAvgActiveTime.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/AQUALAB/features/UserAvgSessionDuration.py` & `opengamedata_core-0.0.3/src/ogd/games/AQUALAB/features/AppVersions.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,42 +1,37 @@
-# import libraries
 from typing import Any, List
-# import locals
+
 from ogd.core.generators.Generator import GeneratorParameters
 from ogd.core.generators.extractors.SessionFeature import SessionFeature
 from ogd.core.schemas.Event import Event
 from ogd.core.schemas.ExtractionMode import ExtractionMode
 from ogd.core.schemas.FeatureData import FeatureData
 
-class UserAvgSessionDuration(SessionFeature):
+class AppVersions(SessionFeature):
+    """_summary_
 
-    def __init__(self, params:GeneratorParameters, player_id:str):
-        self._player_id = player_id
+    :param SessionFeature: _description_
+    :type SessionFeature: _type_
+    """
+    def __init__(self, params:GeneratorParameters):
         super().__init__(params=params)
-        self._times : List[int] = []
+        self._versions = set()
 
     # *** IMPLEMENT ABSTRACT FUNCTIONS ***
     @classmethod
     def _eventFilter(cls, mode:ExtractionMode) -> List[str]:
-        return []
+        return ["all_events"]
 
     @classmethod
     def _featureFilter(cls, mode:ExtractionMode) -> List[str]:
-        return ["SessionDuration"]
+        return []
 
     def _updateFromEvent(self, event:Event) -> None:
-        return
+        self._versions.add(event.AppVersion)
 
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
+        return [list(self._versions)]
 
-    # *** Optionally override public functions. ***
+    # *** Optionally override public functions. ***
```

### Comparing `opengamedata_core-0.0.2/src/ogd/games/AQUALAB/features/UserTotalSessionDuration.py` & `opengamedata_core-0.0.3/src/ogd/games/AQUALAB/features/UserTotalSessionDuration.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/AQUALAB/features/__init__.py` & `opengamedata_core-0.0.3/src/ogd/games/AQUALAB/features/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,85 +1,121 @@
 __all__ = [
-    "JobTriesInArgument",
-    "TankRulesCount",
-    "ModelExportCount",
-    "ModelPredictCount",
-    "UserAvgActiveTime",
-    "ModelInterveneCount",
-    "ActiveTime",
     "ActiveJobs",
+    "ActiveTime",
+    "AppVersions",
+    "AverageSessionTime",
     "EchoSessionID",
     "EventList",
     "JobActiveTime",
-    "JobArgumentationTime",
+    "JobArgumentation",
     "JobCompletionTime",
     "JobDiveSitesCount",
     "JobDiveTime",
-    "JobExperimentationTime",
+    "JobExperimentation",
     "JobGuideCount",
     "JobHelpCount",
     "JobLocationChanges",
-    "JobModelingTime",
-    "JobStartCount",
-    "JobTasksCompleted",
+    "JobModeling",
+    "JobPlayTime",
+    "JobPriorAttempt",
+    "JobPriorComplete",
     "JobsAttempted",
     "JobsCompleted",
+    "JobStartCount",
+    "JobTasksCompleted",
+    "JobTriesInArgument",
+    "ModelExportCount",
+    "ModelInterveneCount",
+    "ModelPredictCount",
     "PlayerSummary",
+    "PlayLocations",
     "PopulationSummary",
+    "RegionJobCount",
+    "RegionName",
     "SessionDiveSitesCount",
     "SessionDuration",
     "SessionGuideCount",
     "SessionHelpCount",
     "SessionID",
     "SessionJobsCompleted",
     "SwitchJobsCount",
     "SyncCompletionTime",
+    "TankRulesCount",
     "TopJobCompletionDestinations",
     "TopJobSwitchDestinations",
+    "TotalArcticTime",
     "TotalArgumentationTime",
+    "TotalBayouTime",
+    "TotalCoralTime",
     "TotalDiveTime",
     "TotalExperimentationTime",
+    "TotalGuideCount",
+    "TotalHelpCount",
+    "TotalKelpTime",
+    "TotalModelingTime",
+    "TotalPlayTime",
+    "UserAvgActiveTime",
     "UserAvgSessionDuration",
-    "UserTotalSessionDuration"
+    "UserTotalSessionDuration",
+    "PlayLocations",
+    "AppVersions"
 ]
 
-from . import JobTriesInArgument
-from . import TankRulesCount
-from . import UserAvgActiveTime
-from . import ModelInterveneCount
-from . import ModelPredictCount
-from . import ModelExportCount
-from . import ActiveTime
 from . import ActiveJobs
+from . import ActiveTime
+from . import AppVersions
+from . import AverageSessionTime
 from . import EchoSessionID
 from . import EventList
 from . import JobActiveTime
-from . import JobArgumentationTime
+from . import JobArgumentation
 from . import JobCompletionTime
 from . import JobDiveSitesCount
 from . import JobDiveTime
-from . import JobExperimentationTime
+from . import JobExperimentation
 from . import JobGuideCount
 from . import JobHelpCount
 from . import JobLocationChanges
-from . import JobModelingTime
-from . import JobStartCount
-from . import JobTasksCompleted
+from . import JobModeling
+from . import JobPlayTime
+from . import JobPriorAttempt
+from . import JobPriorComplete
 from . import JobsAttempted
 from . import JobsCompleted
+from . import JobStartCount
+from . import JobTasksCompleted
+from . import JobTriesInArgument
+from . import ModelExportCount
+from . import ModelInterveneCount
+from . import ModelPredictCount
 from . import PlayerSummary
+from . import PlayLocations
 from . import PopulationSummary
+from . import RegionJobCount
+from . import RegionName
 from . import SessionDiveSitesCount
 from . import SessionDuration
 from . import SessionGuideCount
 from . import SessionHelpCount
 from . import SessionID
 from . import SessionJobsCompleted
 from . import SwitchJobsCount
 from . import SyncCompletionTime
+from . import TankRulesCount
 from . import TopJobCompletionDestinations
 from . import TopJobSwitchDestinations
+from . import TotalArcticTime
 from . import TotalArgumentationTime
+from . import TotalBayouTime
+from . import TotalCoralTime
 from . import TotalDiveTime
 from . import TotalExperimentationTime
+from . import TotalGuideCount
+from . import TotalHelpCount
+from . import TotalKelpTime
+from . import TotalModelingTime
+from . import TotalPlayTime
+from . import UserAvgActiveTime
 from . import UserAvgSessionDuration
 from . import UserTotalSessionDuration
+from . import PlayLocations
+from . import AppVersions
```

### Comparing `opengamedata_core-0.0.2/src/ogd/games/AQUALAB/schemas/AQUALAB.json.template` & `opengamedata_core-0.0.3/src/ogd/games/AQUALAB/schemas/AQUALAB.json.template`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.982954223356009%*

 * *Differences: {"'detectors'": "{'aggregate': {'CollectFactNoJob': {'enabled': False}, 'DiveSiteNoEvidence': "*

 * *                "{'enabled': False}, 'HintAndLeave': {'enabled': False}, 'Idle': {'enabled': "*

 * *                "False}, 'SceneChangeFrequently': {'enabled': False}, 'TwoHints': {'enabled': "*

 * *                'False}}}',*

 * * "'features'": "{'per_count': {'JobGuideCount': {'enabled': False}, 'JobHelpCount': {'enabled': "*

 * *               "False}, 'JobLocationChanges': {'enabled': False}, 'JobsAttempted': {'enabled': "*

 * *   […]*

```diff
@@ -4,49 +4,49 @@
             1
         ]
     },
     "detectors": {
         "aggregate": {
             "CollectFactNoJob": {
                 "description": "Triggers an event when a player collects a fact while not actively working on a job",
-                "enabled": true,
+                "enabled": false,
                 "type": "CollectFactNoJob"
             },
             "DiveSiteNoEvidence": {
                 "description": "Triggers an event when a player has gone sufficiently long at a dive site without uncovering new evidence",
-                "enabled": true,
+                "enabled": false,
                 "threshold": 30,
                 "type": "DiveSiteNoEvidence"
             },
             "EchoRoomChange": {
                 "description": "Triggers an event when a player changes rooms.",
                 "enabled": false,
                 "type": "EchoRoomChange"
             },
             "HintAndLeave": {
                 "description": "",
-                "enabled": true,
+                "enabled": false,
                 "threshold": 30,
                 "type": "HintAndLeave"
             },
             "Idle": {
                 "description": "",
-                "enabled": true,
+                "enabled": false,
                 "idle_level": 30,
                 "type": "Idle"
             },
             "SceneChangeFrequently": {
                 "description": "",
-                "enabled": true,
+                "enabled": false,
                 "threshold": 30,
                 "type": "SceneChangeFrequently"
             },
             "TwoHints": {
                 "description": "",
-                "enabled": true,
+                "enabled": false,
                 "threshold": 30,
                 "type": "TwoHints"
             }
         },
         "per_count": {}
     },
     "events": {
@@ -544,41 +544,54 @@
             "event_data": {}
         }
     },
     "features": {
         "aggregate": {
             "ActiveJobs": {
                 "description": "Count of players who left off on each job.",
-                "enabled": false,
+                "enabled": true,
                 "return_type": "dict",
                 "type": "ActiveJobs"
             },
             "ActiveTime": {
-                "enabled": true,
+                "description": "Total time spent actively playing",
+                "enabled": false,
                 "return_type": "timedelta",
                 "type": "ActiveTime"
             },
-            "EchoSessionID": {
-                "description": "Test of second-order features.",
-                "enabled": false,
-                "return_type": "str",
-                "type": "EchoSessionID"
+            "AppVersions": {
+                "description": "List of all app versions encountered.",
+                "enabled": true,
+                "return_type": "list",
+                "type": "AppVersions"
             },
             "EventList": {
                 "description": "List of key events that happened in a player's session(s)",
                 "enabled": false,
                 "return_type": "list",
                 "type": "EventList"
             },
             "JobsCompleted": {
                 "description": "List of completed jobs for a player",
                 "enabled": true,
                 "return_type": "list[str]",
                 "type": "JobsCompleted"
             },
+            "PlayLocations": {
+                "description": "An indicator of whether play happened during normal school hours or not",
+                "enabled": false,
+                "return_type": "List[bool]",
+                "subfeatures": {
+                    "LocalTime": {
+                        "description": "The actual local time when each session started",
+                        "return_type": "datetime"
+                    }
+                },
+                "type": "PlayLocations"
+            },
             "PlayerSummary": {
                 "description": "Summary of player statistics (active session time, jobs completed, number of sessions)",
                 "enabled": false,
                 "return_type": "dict",
                 "type": "PlayerSummary"
             },
             "PopulationSummary": {
@@ -593,55 +606,38 @@
                 "return_type": "int",
                 "type": "SessionDiveSitesCount"
             },
             "SessionDuration": {
                 "description": "Time spent playing in a given session",
                 "enabled": true,
                 "return_type": "timedelta",
+                "threshold": 60,
                 "type": "SessionDuration"
             },
-            "SessionGuideCount": {
-                "description": "Number of times player talked with the guide throughout the session",
-                "enabled": true,
-                "return_type": "int",
-                "type": "SessionGuideCount"
-            },
-            "SessionHelpCount": {
-                "description": "Number of times player clicked the help button throughout the session",
-                "enabled": true,
-                "return_type": "int",
-                "type": "SessionHelpCount"
-            },
             "SessionID": {
                 "description": "The player's session ID number for this play session",
-                "enabled": true,
+                "enabled": false,
                 "return_type": "str",
                 "type": "SessionID"
             },
-            "SessionJobsCompleted": {
-                "description": "Number of jobs completed in a given session",
-                "enabled": true,
-                "return_type": "int",
-                "type": "SessionJobsCompleted"
-            },
             "SwitchJobsCount": {
                 "description": "Number of times player switched jobs before completion",
                 "enabled": true,
                 "return_type": "int",
                 "type": "SwitchJobsCount"
             },
             "TopJobCompletionDestinations": {
                 "description": "Top five most accepted jobs after previously completing a given job",
-                "enabled": true,
+                "enabled": false,
                 "return_type": "str",
                 "type": "TopJobCompletionDestinations"
             },
             "TopJobSwitchDestinations": {
                 "description": "Top five most accepted jobs after switching away from a given job",
-                "enabled": true,
+                "enabled": false,
                 "return_type": "str",
                 "type": "TopJobSwitchDestinations"
             },
             "TotalArgumentationTime": {
                 "description": "Total time spent in argumentation",
                 "enabled": true,
                 "return_type": "timedelta",
@@ -655,14 +651,38 @@
             },
             "TotalExperimentationTime": {
                 "description": "Total time spent in experimentation",
                 "enabled": true,
                 "return_type": "timedelta",
                 "type": "TotalExperimentationTime"
             },
+            "TotalGuideCount": {
+                "description": "Number of times player talked with the guide throughout the session",
+                "enabled": true,
+                "return_type": "int",
+                "type": "TotalGuideCount"
+            },
+            "TotalHelpCount": {
+                "description": "Number of times player clicked the help button throughout the session",
+                "enabled": true,
+                "return_type": "int",
+                "type": "TotalHelpCount"
+            },
+            "TotalModelingTime": {
+                "description": "Total time spent in modeling",
+                "enabled": true,
+                "return_type": "timedelta",
+                "type": "TotalModelingTime"
+            },
+            "TotalPlayTime": {
+                "description": "Total time the player had the game open, based on sum total of SessionDurations.",
+                "enabled": true,
+                "return_type": "timedelta",
+                "type": "TotalPlayTime"
+            },
             "UserAvgSessionDuration": {
                 "description": "Average session duration for a user.",
                 "enabled": true,
                 "return_type": "float",
                 "type": "UserAvgSessionDuration"
             },
             "UserTotalSessionDuration": {
@@ -677,21 +697,27 @@
                 "count": "level_range",
                 "description": "Time spent with job as the active job",
                 "enabled": true,
                 "prefix": "job",
                 "return_type": "timedelta",
                 "type": "JobActiveTime"
             },
-            "JobArgumentationTime": {
+            "JobArgumentation": {
                 "count": "level_range",
-                "description": "Time spent in argumentation during a job",
+                "description": "Number of times the player entered the argumentation mechanic during a job",
                 "enabled": true,
                 "prefix": "job",
                 "return_type": "timedelta",
-                "type": "JobArgumentationTime"
+                "subfeatures": {
+                    "Time": {
+                        "description": "Time spent in argumentation during a job",
+                        "return_type": "timedelta"
+                    }
+                },
+                "type": "JobArgumentation"
             },
             "JobCompletionTime": {
                 "count": "level_range",
                 "description": "Time taken to complete a given job",
                 "enabled": true,
                 "prefix": "job",
                 "return_type": "timedelta",
@@ -709,78 +735,106 @@
                 "count": "level_range",
                 "description": "Time spent diving during a job",
                 "enabled": true,
                 "prefix": "job",
                 "return_type": "timedelta",
                 "type": "JobDiveTime"
             },
-            "JobExperimentationTime": {
+            "JobExperimentation": {
                 "count": "level_range",
-                "description": "Time spent in experimentation during a job",
+                "description": "Number of times the player entered the experimentation mechanic during a job",
                 "enabled": true,
                 "prefix": "job",
                 "return_type": "timedelta",
-                "type": "JobExperimentationTime"
+                "subfeatures": {
+                    "Time": {
+                        "description": "Time spent in experimentation during a job",
+                        "return_type": "timedelta"
+                    }
+                },
+                "type": "JobExperimentation"
             },
             "JobGuideCount": {
                 "count": "level_range",
                 "description": "Number of times player talked with guide during a job",
-                "enabled": true,
+                "enabled": false,
                 "prefix": "job",
                 "return_type": "int",
                 "type": "JobGuideCount"
             },
             "JobHelpCount": {
                 "count": "level_range",
                 "description": "Number of times player asked for help during a job",
-                "enabled": true,
+                "enabled": false,
                 "prefix": "job",
                 "return_type": "int",
                 "subfeatures": {
                     "ByTask": {
                         "description": "Help counts leading up to each completed task",
                         "return_type": "int"
                     }
                 },
                 "type": "JobHelpCount"
             },
             "JobLocationChanges": {
                 "count": "level_range",
                 "description": "Number of times player changed scenes or rooms",
-                "enabled": true,
+                "enabled": false,
                 "prefix": "job",
                 "return_type": "int",
                 "subfeatures": {
                     "ByTask": {
                         "description": "Change counts leading up to each completed task",
                         "return_type": "int"
                     }
                 },
                 "type": "JobLocationChanges"
             },
-            "JobModelingTime": {
+            "JobModeling": {
                 "count": "level_range",
-                "description": "Time spent in modeling during a job",
+                "description": "Number of times the player entered the modeling mechanic during a job",
                 "enabled": true,
                 "prefix": "job",
                 "return_type": "timedelta",
-                "type": "JobModelingTime"
+                "subfeatures": {
+                    "Time": {
+                        "description": "Time spent in modeling during a job",
+                        "return_type": "timedelta"
+                    }
+                },
+                "type": "JobModeling"
+            },
+            "JobPriorAttempt": {
+                "count": "level_range",
+                "description": "",
+                "enabled": true,
+                "prefix": "job",
+                "return_type": "list",
+                "type": "JobPriorAttempt"
+            },
+            "JobPriorComplete": {
+                "count": "level_range",
+                "description": "",
+                "enabled": true,
+                "prefix": "job",
+                "return_type": "list",
+                "type": "JobPriorComplete"
             },
             "JobTasksCompleted": {
                 "count": "level_range",
                 "description": "Number of tasks completed for a given job",
                 "enabled": true,
                 "prefix": "job",
                 "return_type": "int",
                 "type": "JobTasksCompleted"
             },
             "JobsAttempted": {
                 "count": "level_range",
                 "description": "Subfeatures for number of job starts and completes, percent complete, and avg/std time to complete",
-                "enabled": true,
+                "enabled": false,
                 "prefix": "job",
                 "subfeatures": {
                     "avg-time-per-attempt": {
                         "description": "Average time taken from accepting to completing/leaving a job",
                         "return_type": "float"
                     },
                     "job-difficulties": {
@@ -806,14 +860,30 @@
                     "std-dev-per-attempt": {
                         "description": "Standard deviation of time taken on a job",
                         "return_type": "float"
                     }
                 },
                 "type": "JobsAttempted"
             },
+            "RegionJobCount": {
+                "count": 5,
+                "description": "The number of jobs completed in a given region",
+                "enabled": true,
+                "prefix": "region",
+                "return_type": "int",
+                "type": "RegionJobCount"
+            },
+            "RegionName": {
+                "count": 5,
+                "description": "The human-readable version of the name for a given region",
+                "enabled": true,
+                "prefix": "region",
+                "return_type": "str",
+                "type": "RegionName"
+            },
             "SyncCompletionTime": {
                 "count": "level_range",
                 "description": "Time taken to achieve 100% sync in a simulation",
                 "enabled": true,
                 "prefix": "job",
                 "return_type": "timedelta",
                 "type": "SyncCompletionTime"
```

### Comparing `opengamedata_core-0.0.2/src/ogd/games/BLOOM/schemas/BLOOM.json.template` & `opengamedata_core-0.0.3/src/ogd/games/BLOOM/schemas/BLOOM.json.template`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9882051282051283%*

 * *Differences: {"'enums'": "{'LossType': ['CityFailed', 'TooManyBlooms', 'OutOfMoney']}",*

 * * "'events'": '{\'win_game\': OrderedDict([(\'description\', "When the player enters the game win '*

 * *             'state, and is shown the \'you win\' cutscene"), (\'event_data\', '*

 * *             "OrderedDict([('map_state', OrderedDict([('type', 'TODO : BuildMap'), ('description', "*

 * *             "'The state of the build map when the player entered the win state.')]))]))]), "*

 * *             "'lose_game': OrderedDict([('description', 'When  […]*

```diff
@@ -39,14 +39,19 @@
         "ImportPolicy": [
             "NOT_SET",
             "NONE",
             "MILK",
             "GRAIN",
             "FERTILIZER"
         ],
+        "LossType": [
+            "CityFailed",
+            "TooManyBlooms",
+            "OutOfMoney"
+        ],
         "MapMode": [
             "VIEW",
             "BUILD",
             "DESTROY"
         ],
         "PolicyCategory": [
             "ECONOMY",
@@ -408,14 +413,23 @@
                 },
                 "policy": {
                     "description": "The specific policy whose cards are displayed, i.e. sales tax, import subsidy, runoff fine, or cleanup initiative.",
                     "type": "PolicyType"
                 }
             }
         },
+        "lose_game": {
+            "description": "When the player enters the game lose state, and is taken back to a checkpoint to try again.",
+            "event_data": {
+                "lose_condition": {
+                    "description": "The state of the build map when the player entered the win state.",
+                    "type": "LossType"
+                }
+            }
+        },
         "open_economy_view": {
             "description": "When the player clicks to open the economy breakdown view",
             "event_data": {}
         },
         "pause_game": {
             "description": "When the player presses the spacebar or escape key to pause the game",
             "event_data": {}
@@ -488,14 +502,23 @@
                     "type": "MapMode"
                 }
             }
         },
         "unpause_game": {
             "description": "When the player presses the spacebar or escape key to un-pause the game",
             "event_data": {}
+        },
+        "win_game": {
+            "description": "When the player enters the game win state, and is shown the 'you win' cutscene",
+            "event_data": {
+                "map_state": {
+                    "description": "The state of the build map when the player entered the win state.",
+                    "type": "TODO : BuildMap"
+                }
+            }
         }
     },
     "features": {
         "aggregate": {},
         "per_count": {}
     },
     "game_state": {
```

### Comparing `opengamedata_core-0.0.2/src/ogd/games/CENSIO_SLIDE/schemas/CENSIO_SLIDE.json.template` & `opengamedata_core-0.0.3/src/ogd/games/CENSIO_SLIDE/schemas/CENSIO_SLIDE.json.template`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/CENSIO_STACK/schemas/CENSIO_STACK.json.template` & `opengamedata_core-0.0.3/src/ogd/games/CENSIO_STACK/schemas/CENSIO_STACK.json.template`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/CRUSH_STATION/schemas/CRUSH_STATION.json.template` & `opengamedata_core-0.0.3/src/ogd/games/CRUSH_STATION/schemas/CRUSH_STATION.json.template`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/CRYSTAL/CrystalLoader.py` & `opengamedata_core-0.0.3/src/ogd/games/CRYSTAL/CrystalLoader.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/CRYSTAL/features/CrystalExtractor.py` & `opengamedata_core-0.0.3/src/ogd/games/CRYSTAL/features/CrystalExtractor.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/CRYSTAL/schemas/CRYSTAL.json.template` & `opengamedata_core-0.0.3/src/ogd/games/CRYSTAL/schemas/CRYSTAL.json.template`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/GWAKKAMOLE/schemas/GWAKKAMOLE.json.template` & `opengamedata_core-0.0.3/src/ogd/games/GWAKKAMOLE/schemas/GWAKKAMOLE.json.template`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/ICECUBE/DBExport.json` & `opengamedata_core-0.0.3/src/ogd/games/ICECUBE/DBExport.json`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/ICECUBE/DBExport.py` & `opengamedata_core-0.0.3/src/ogd/games/ICECUBE/DBExport.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/ICECUBE/IcecubeLoader.py` & `opengamedata_core-0.0.3/src/ogd/games/ICECUBE/IcecubeLoader.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/ICECUBE/features/HeadsetOnCount.py` & `opengamedata_core-0.0.3/src/ogd/games/ICECUBE/features/HeadsetOnCount.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/ICECUBE/features/ObjectSelectionsDuringVoiceover.py` & `opengamedata_core-0.0.3/src/ogd/games/ICECUBE/features/ObjectSelectionsDuringVoiceover.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/ICECUBE/features/PerSceneFeature.py` & `opengamedata_core-0.0.3/src/ogd/games/ICECUBE/features/PerSceneFeature.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/ICECUBE/features/SceneDuration.py` & `opengamedata_core-0.0.3/src/ogd/games/ICECUBE/features/SceneDuration.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/ICECUBE/features/SceneFailureCount.py` & `opengamedata_core-0.0.3/src/ogd/games/ICECUBE/features/SceneFailureCount.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/ICECUBE/features/SceneFailures.py` & `opengamedata_core-0.0.3/src/ogd/games/ICECUBE/features/SceneFailures.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/ICECUBE/features/ScenesEncountered.py` & `opengamedata_core-0.0.3/src/ogd/games/ICECUBE/features/ScenesEncountered.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/ICECUBE/features/SessionDuration.py` & `opengamedata_core-0.0.3/src/ogd/games/ICECUBE/features/SessionDuration.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/ICECUBE/features/Session_Language.py` & `opengamedata_core-0.0.3/src/ogd/games/ICECUBE/features/Session_Language.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/ICECUBE/features/TaskTimeToComplete.py` & `opengamedata_core-0.0.3/src/ogd/games/ICECUBE/features/TaskTimeToComplete.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/ICECUBE/features/ViewportCountPerScene.py` & `opengamedata_core-0.0.3/src/ogd/games/ICECUBE/features/ViewportCountPerScene.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/ICECUBE/features/__init__.py` & `opengamedata_core-0.0.3/src/ogd/games/ICECUBE/features/__init__.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/ICECUBE/schemas/ICECUBE.json.template` & `opengamedata_core-0.0.3/src/ogd/games/ICECUBE/schemas/ICECUBE.json.template`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/JOURNALISM/JournalismLoader.py` & `opengamedata_core-0.0.3/src/ogd/games/JOURNALISM/JournalismLoader.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,14 +28,18 @@
         ret_val : Feature
         if extractor_params._count_index == None:
             match feature_type:
                 case "ChoiceClickCount":
                     ret_val = ChoiceClickCount.ChoiceClickCount(params=extractor_params)
                 case "SessionPlayTime":
                     ret_val = SessionPlayTime.SessionPlayTime(params=extractor_params, threshold=schema_args.get("IDLE_THRESH_SECONDS", SessionPlayTime.SessionPlayTime.IDLE_TIME_THRESHOLD))
+                case "FinalAttributes":
+                    ret_val = FinalAttributes.FinalAttributes(params=extractor_params)
+                case "FailureAttributes":
+                    ret_val = FailureAttributes.FailureAttributes(params=extractor_params)
                 case "SkillSequenceCount":
                     ret_val = SkillSequenceCount.SkillSequenceCount(params = extractor_params)
                 case "MeanSnippetTime":
                     ret_val = MeanSnippetTime.MeanSnippetTime(params = extractor_params)
                 case "TextClickCount":
                     ret_val = TextClickCount.TextClickCount(params=extractor_params)
                 case "SnippetReceivedCount":
```

### Comparing `opengamedata_core-0.0.2/src/ogd/games/JOURNALISM/features/AttributeView.py` & `opengamedata_core-0.0.3/src/ogd/games/JOURNALISM/features/AttributeView.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/JOURNALISM/features/ChoiceClickCount.py` & `opengamedata_core-0.0.3/src/ogd/games/JOURNALISM/features/ChoiceClickCount.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/JOURNALISM/features/ContinuesOnFail.py` & `opengamedata_core-0.0.3/src/ogd/games/JOURNALISM/features/ContinuesOnFail.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/JOURNALISM/features/EditorNoteOpen.py` & `opengamedata_core-0.0.3/src/ogd/games/JOURNALISM/features/EditorNoteOpen.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/JOURNALISM/features/FailureCount.py` & `opengamedata_core-0.0.3/src/ogd/games/JOURNALISM/features/FailureCount.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/JOURNALISM/features/GameComplete.py` & `opengamedata_core-0.0.3/src/ogd/games/JOURNALISM/features/GameComplete.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/JOURNALISM/features/LevelCompleteCount.py` & `opengamedata_core-0.0.3/src/ogd/games/JOURNALISM/features/LevelCompleteCount.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/JOURNALISM/features/LevelCompleted.py` & `opengamedata_core-0.0.3/src/ogd/games/JOURNALISM/features/LevelCompleted.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/JOURNALISM/features/LevelTime.py` & `opengamedata_core-0.0.3/src/ogd/games/JOURNALISM/features/LevelTime.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/JOURNALISM/features/MaxedPlayerAttribute.py` & `opengamedata_core-0.0.3/src/ogd/games/JOURNALISM/features/MaxedPlayerAttribute.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/JOURNALISM/features/MeanSnippetTime.py` & `opengamedata_core-0.0.3/src/ogd/games/JOURNALISM/features/MeanSnippetTime.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/JOURNALISM/features/PlayTime.py` & `opengamedata_core-0.0.3/src/ogd/games/JOURNALISM/features/PlayTime.py`

 * *Files 1% similar despite different names*

```diff
@@ -107,18 +107,17 @@
         """
 
         #exception handling for empty sessions
 
         try:
             total_time : timedelta = self._last_event_timestamp - self._first_event_timestamp
             play_time : timedelta = total_time - self._idle_time
-
         except:
-            total_time = 0
-            play_time = 0
+            total_time = timedelta(0)
+            play_time  = timedelta(0)
 
 
         return [total_time, play_time, self._idle_time]
 
 
     # *** Optionally override public functions. ***
     def Subfeatures(self) -> List[str]:
```

### Comparing `opengamedata_core-0.0.2/src/ogd/games/JOURNALISM/features/PlayerAttributes.py` & `opengamedata_core-0.0.3/src/ogd/games/JOURNALISM/features/PlayerAttributes.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/JOURNALISM/features/QuitLevel.py` & `opengamedata_core-0.0.3/src/ogd/games/JOURNALISM/features/QuitLevel.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/JOURNALISM/features/QuitNode.py` & `opengamedata_core-0.0.3/src/ogd/games/JOURNALISM/features/QuitNode.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/JOURNALISM/features/QuitType.py` & `opengamedata_core-0.0.3/src/ogd/games/JOURNALISM/features/QuitType.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/JOURNALISM/features/QuitTypePerLevel.py` & `opengamedata_core-0.0.3/src/ogd/games/JOURNALISM/features/QuitTypePerLevel.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/JOURNALISM/features/SessionPlayTime.py` & `opengamedata_core-0.0.3/src/ogd/games/JOURNALISM/features/SessionPlayTime.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/JOURNALISM/features/SkillSequenceCount.py` & `opengamedata_core-0.0.3/src/ogd/games/JOURNALISM/features/SkillSequenceCount.py`

 * *Files 1% similar despite different names*

```diff
@@ -99,15 +99,15 @@
         #
         # note the code above is redundant, we could just return [self._found_click] to get the same result;
         # the more-verbose code is here for illustrative purposes.
         event_string = json.dumps(self._skill_event_sequence)
 
         # print("TOTAL DEBUG: " + self._total_upgrades)
         # print(self._total_upgrades)
-        return [self._total_upgrades, event_string]
+        return [self._total_upgrades, self._skill_event_sequence]
 
 
     # *** Optionally override public functions. ***
     def Subfeatures(self) -> List[str]:
         return ["Event Sequence"] # >>> fill in names of Subfeatures for which this Feature should extract values. <<<
     
     @staticmethod
```

### Comparing `opengamedata_core-0.0.2/src/ogd/games/JOURNALISM/features/SnippetReceivedCount.py` & `opengamedata_core-0.0.3/src/ogd/games/JOURNALISM/features/TotalFails.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,37 +8,37 @@
 from ogd.core.schemas.FeatureData import FeatureData
 from ogd.core.generators.Generator import GeneratorParameters
 from ogd.core.generators.extractors.SessionFeature import SessionFeature
 
 
 
 
-class SnippetReceivedCount(SessionFeature):
+class TotalFails(SessionFeature):
     """Template file to serve as a guide for creating custom Feature subclasses for games.
 
     :param Feature: Base class for a Custom Feature class.
     :type Feature: _type_
     """
     def __init__(self, params:GeneratorParameters):
         super().__init__(params=params)
-        choice_type_names = ["BAD", "GOOD", "GREAT"]
-        self._init_vals = {name: 0 for name in choice_type_names}
-
-        self._snippet_receive_count : int = 0;
-        
+        self._fail_count : int = 0;
+        # >>> create/initialize any variables to track feature extractor state <<<
+        #
+        # e.g. To track whether extractor found a click event yet:
+        # self._found_click : bool = False
 
     # *** IMPLEMENT ABSTRACT FUNCTIONS ***
     @classmethod
     def _eventFilter(cls, mode:ExtractionMode) -> List[str]:
         """_summary_
 
         :return: _description_
         :rtype: List[str]
         """
-        return ["snippet_received"] # >>> fill in names of events this Feature should use for extraction. <<<
+        return ["level_fail"] # >>> fill in names of events this Feature should use for extraction. <<<
 
     @classmethod
     def _featureFilter(cls, mode:ExtractionMode) -> List[str]:
         """_summary_
 
         :return: _description_
         :rtype: List[str]
@@ -52,20 +52,15 @@
         :type event: Event
         """
         # >>> use the data in the Event object to update state variables as needed. <<<
         # Note that this function runs once on each Event whose name matches one of the strings returned by _eventFilter()
         #
         # e.g. check if the event name contains the substring "Click," and if so set self._found_click to True
         
-        
-        self._choice_click_count += 1
-        for key in self._init_vals:
-            if key in event.event_data.snippet_quality:
-                self._init_vals[key] +=1
-
+        self._fail_count +=1
         
         
         return
 
     def _updateFromFeatureData(self, feature: FeatureData):
         """_summary_
 
@@ -94,22 +89,20 @@
         # else:
         #     ret_val = [False]
         # return ret_val
         #
         # note the code above is redundant, we could just return [self._found_click] to get the same result;
         # the more-verbose code is here for illustrative purposes.
         
-        return [self._snippet_receive_count, self._init_vals["BAD"],
-        self._init_vals["GOOD"], self._init_vals["GREAT"]]
+        return [self._fail_count]
 
 
     # *** Optionally override public functions. ***
     def Subfeatures(self) -> List[str]:
-        return ["Bad", "Good", "Great"] # >>> fill in names of Subfeatures for which this Feature should extract values. <<<
-    
+        return []
     @staticmethod
     def AvailableModes() -> List[ExtractionMode]:
         return [ExtractionMode.POPULATION, ExtractionMode.PLAYER, ExtractionMode.SESSION] # >>> delete any modes you don't want run for your Feature. <<<
     
     # @staticmethod
     # def MinVersion() -> Optional[str]:
     #     # >>> replace return statement below with a string defining the minimum logging version for events to be processed by this Feature. <<<
```

### Comparing `opengamedata_core-0.0.2/src/ogd/games/JOURNALISM/features/SnippetReplace.py` & `opengamedata_core-0.0.3/src/ogd/games/JOURNALISM/features/SnippetReplace.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/JOURNALISM/features/SnippetsCollected.py` & `opengamedata_core-0.0.3/src/ogd/games/WAVES/features/TotalArrowMoves.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,47 +1,35 @@
-import logging
-from datetime import datetime
+# import libraries
 from ogd.core.schemas import Event
 from typing import Any, List, Optional
 # import locals
-from ogd.core.utils.Logger import Logger
 from ogd.core.generators.extractors.PerLevelFeature import PerLevelFeature
 from ogd.core.generators.Generator import GeneratorParameters
 from ogd.core.schemas.Event import Event
 from ogd.core.schemas.ExtractionMode import ExtractionMode
 from ogd.core.schemas.FeatureData import FeatureData
 
-class SnippetsCollected(PerLevelFeature):
+class TotalArrowMoves(PerLevelFeature):
     def __init__(self, params:GeneratorParameters):
         PerLevelFeature.__init__(self, params=params)
-        self._snippet_ids : List[str] = []
-
+        self._arrow_move_count : int = 0
 
     # *** IMPLEMENT ABSTRACT FUNCTIONS ***
     @classmethod
     def _eventFilter(cls, mode:ExtractionMode) -> List[str]:
-        return ["snippet_received"]
+        return ["CUSTOM.2"]
+        # return ["ARROW_MOVE_RELEASE"]
 
     @classmethod
     def _featureFilter(cls, mode:ExtractionMode) -> List[str]:
         return []
 
     def _updateFromEvent(self, event:Event) -> None:
-        if event.EventName == "snippet_received":
-            self._snippet_ids.append(event.EventData["snippet_id"])
-
-    def _updateFromFeatureData(self, feature: FeatureData):
-        """_summary_
+        self._arrow_move_count += 1
 
-        :param feature: _description_
-        :type feature: FeatureData
-        """
+    def _updateFromFeatureData(self, feature:FeatureData):
         return
 
     def _getFeatureValues(self) -> List[Any]:
-        return [self._snippet_ids]
+        return [self._arrow_move_count]
 
     # *** Optionally override public functions. ***
-    
-    @staticmethod
-    def AvailableModes() -> List[ExtractionMode]:
-        return [ExtractionMode.PLAYER, ExtractionMode.SESSION]
```

### Comparing `opengamedata_core-0.0.2/src/ogd/games/JOURNALISM/features/SnippetsSubmitted.py` & `opengamedata_core-0.0.3/src/ogd/games/JOURNALISM/features/SnippetsSubmitted.py`

 * *Files 8% similar despite different names*

```diff
@@ -27,17 +27,17 @@
     def _featureFilter(cls, mode:ExtractionMode) -> List[str]:
         return []
 
     def _updateFromEvent(self, event:Event) -> None:
         if event.EventName == "story_click":
             snippet_list = json.loads( event.EventData["snippet_list"] )
             for snippet in snippet_list:
-                if not SnippetsSubmitted.has_printed:
-                    print(f"snippet: {snippet} of type {type(snippet)}")
-                    SnippetsSubmitted.has_printed = True
+                # if not SnippetsSubmitted.has_printed:
+                #     print(f"snippet: {snippet} of type {type(snippet)}")
+                #     SnippetsSubmitted.has_printed = True
                 self._snippet_ids.append(snippet.get("SnippetId", "NOT FOUND"))
 
     def _updateFromFeatureData(self, feature: FeatureData):
         return
 
     def _getFeatureValues(self) -> List[Any]:
         return [self._snippet_ids]
```

### Comparing `opengamedata_core-0.0.2/src/ogd/games/JOURNALISM/features/StoryAlignment.py` & `opengamedata_core-0.0.3/src/ogd/games/JOURNALISM/features/StoryAlignment.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/JOURNALISM/features/StoryAlignmentSequence.py` & `opengamedata_core-0.0.3/src/ogd/games/JOURNALISM/features/StoryAlignmentSequence.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/JOURNALISM/features/StoryCompleteTime.py` & `opengamedata_core-0.0.3/src/ogd/games/JOURNALISM/features/StoryCompleteTime.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/JOURNALISM/features/StoryEditorTime.py` & `opengamedata_core-0.0.3/src/ogd/games/JOURNALISM/features/StoryEditorTime.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/JOURNALISM/features/StoryScore.py` & `opengamedata_core-0.0.3/src/ogd/games/JOURNALISM/features/StoryScore.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from ogd.core.schemas import Event
 from ogd.core.generators.extractors.PerLevelFeature import PerLevelFeature
 from ogd.core.generators.Generator import GeneratorParameters
 from ogd.core.schemas.Event import Event
 from ogd.core.schemas.ExtractionMode import ExtractionMode
 from ogd.core.schemas.FeatureData import FeatureData
 
+
 class StoryScore(PerLevelFeature):
     def __init__(self, params: GeneratorParameters):
         PerLevelFeature.__init__(self, params=params)
         self._story_score = 0
 
     @classmethod
     def _eventFilter(cls, mode: ExtractionMode) -> List[str]:
```

### Comparing `opengamedata_core-0.0.2/src/ogd/games/JOURNALISM/features/StoryScoreSequence.py` & `opengamedata_core-0.0.3/src/ogd/games/JOURNALISM/features/StoryScoreSequence.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/JOURNALISM/features/TextClickCount.py` & `opengamedata_core-0.0.3/src/ogd/games/JOURNALISM/features/TextClickCount.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/JOURNALISM/features/TopAttribute.py` & `opengamedata_core-0.0.3/src/ogd/games/JOURNALISM/features/TopAttribute.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/JOURNALISM/features/TopPlayerAttribute.py` & `opengamedata_core-0.0.3/src/ogd/games/JOURNALISM/features/TopPlayerAttribute.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/JOURNALISM/features/TopPlayerQuitType.py` & `opengamedata_core-0.0.3/src/ogd/games/JOURNALISM/features/TopPlayerQuitType.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/JOURNALISM/features/TotalFails.py` & `opengamedata_core-0.0.3/src/ogd/games/JOURNALISM/features/WorstAttribute.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,44 +1,44 @@
 # import libraries
 import json
-from typing import Any, List, Optional
+from typing import Any, Final, List, Optional
 # import local files
 from ogd.core.generators.extractors.Feature import Feature
 from ogd.core.schemas.Event import Event
 from ogd.core.schemas.ExtractionMode import ExtractionMode
 from ogd.core.schemas.FeatureData import FeatureData
 from ogd.core.generators.Generator import GeneratorParameters
 from ogd.core.generators.extractors.SessionFeature import SessionFeature
 
-
-
-
-class TotalFails(SessionFeature):
+class WorstAttribute(SessionFeature):
     """Template file to serve as a guide for creating custom Feature subclasses for games.
 
     :param Feature: Base class for a Custom Feature class.
     :type Feature: _type_
     """
     def __init__(self, params:GeneratorParameters):
         super().__init__(params=params)
-        self._fail_count : int = 0;
+        self._min_value : int = 0
+        self._min_names : List[str] = []
+        self._ATTRIBUTE_ENUM : Final[List[str]] = ["endurance", "resourceful", "tech","social","trust","research"]
+        #self._text_click_count : int = 0;
         # >>> create/initialize any variables to track feature extractor state <<<
         #
         # e.g. To track whether extractor found a click event yet:
         # self._found_click : bool = False
 
     # *** IMPLEMENT ABSTRACT FUNCTIONS ***
     @classmethod
     def _eventFilter(cls, mode:ExtractionMode) -> List[str]:
         """_summary_
 
         :return: _description_
         :rtype: List[str]
         """
-        return ["level_fail"] # >>> fill in names of events this Feature should use for extraction. <<<
+        return ["stat_update"] # >>> fill in names of events this Feature should use for extraction. <<<
 
     @classmethod
     def _featureFilter(cls, mode:ExtractionMode) -> List[str]:
         """_summary_
 
         :return: _description_
         :rtype: List[str]
@@ -47,22 +47,27 @@
 
     def _updateFromEvent(self, event:Event) -> None:
         """_summary_
 
         :param event: _description_
         :type event: Event
         """
-        # >>> use the data in the Event object to update state variables as needed. <<<
-        # Note that this function runs once on each Event whose name matches one of the strings returned by _eventFilter()
-        #
-        # e.g. check if the event name contains the substring "Click," and if so set self._found_click to True
-        
-        self._fail_count +=1
-        
+
+        self._min_names = []
         
+        skill_vals = eval(event.GameState["current_stats"])
+        self._min_value = min(skill_vals)
+        #get lowest val in list 
+        res_list = [i for i in range(len(skill_vals)) if skill_vals[i] == self._min_value]
+
+        for val in res_list:
+            self._min_names.append(self._ATTRIBUTE_ENUM[val])
+
+
+
         return
 
     def _updateFromFeatureData(self, feature: FeatureData):
         """_summary_
 
         :param feature: _description_
         :type feature: FeatureData
@@ -88,24 +93,24 @@
         #     ret_val = [True]
         # else:
         #     ret_val = [False]
         # return ret_val
         #
         # note the code above is redundant, we could just return [self._found_click] to get the same result;
         # the more-verbose code is here for illustrative purposes.
-        
-        return [self._fail_count]
+        return [self._min_value,self._min_names]
 
 
     # *** Optionally override public functions. ***
     def Subfeatures(self) -> List[str]:
-        return []
+        return ["Names"] # >>> fill in names of Subfeatures for which this Feature should extract values. <<<
+    
     @staticmethod
     def AvailableModes() -> List[ExtractionMode]:
-        return [ExtractionMode.POPULATION, ExtractionMode.PLAYER, ExtractionMode.SESSION] # >>> delete any modes you don't want run for your Feature. <<<
+        return [ExtractionMode.PLAYER, ExtractionMode.SESSION] # >>> delete any modes you don't want run for your Feature. <<<
     
     # @staticmethod
     # def MinVersion() -> Optional[str]:
     #     # >>> replace return statement below with a string defining the minimum logging version for events to be processed by this Feature. <<<
     #     return super().MinVersion()
 
     # @staticmethod
```

### Comparing `opengamedata_core-0.0.2/src/ogd/games/JOURNALISM/features/TotalLevelTime.py` & `opengamedata_core-0.0.3/src/ogd/games/JOURNALISM/features/TotalLevelTime.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/JOURNALISM/features/UserPlayTime.py` & `opengamedata_core-0.0.3/src/ogd/games/JOURNALISM/features/UserPlayTime.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     :param Feature: Base class for a Custom Feature class.
     :type Feature: _type_
     """
 
     def __init__(self, params:GeneratorParameters):
         super().__init__(params=params)
         self._cumulative_play_time : Optional[timedelta] = None 
-        self._cumulative_total_time : Optional[timedelta] = None
+        self._cumulative_active_time : Optional[timedelta] = None
         
 
 
     # *** IMPLEMENT ABSTRACT FUNCTIONS ***
     @classmethod
     def _eventFilter(cls, mode:ExtractionMode) -> List[str]:
         """_summary_
@@ -68,45 +68,45 @@
         # >>> use data in the FeatureData object to update state variables as needed. <<<
         # Note: This function runs on data from each Feature whose name matches one of the strings returned by _featureFilter().
         #       The number of instances of each Feature may vary, depending on the configuration and the unit of analysis at which this CustomFeature is run.
     
         # Exception handling for empty sessions
         if(not self._cumulative_play_time):
             self._cumulative_play_time = feature._vals[0]
-        if(not self._cumulative_total_time):
-            self._cumulative_total_time = feature._vals[1]
+        if(not self._cumulative_active_time):
+            self._cumulative_active_time = feature._vals[1]
 
         try:
-            self._cumulative_play_time+=feature._vals[0]
-            self._cumulative_total_time+= feature._vals[1]
+            self._cumulative_play_time  += feature.FeatureValues[0]
+            self._cumulative_active_time += feature.FeatureValues[1]
         except:
-            self._cumulative_play_time += 0
-            self._cumulative_total_time += 0
+            self._cumulative_play_time += timedelta(0)
+            self._cumulative_active_time += timedelta(0)
 
         
         
         return
 
     def _getFeatureValues(self) -> List[Any]:
         """_summary_
 
         :return: _description_
         :rtype: List[Any]
         """
 
-        return [self._cumulative_play_time, self._cumulative_total_time]
+        return [self._cumulative_play_time, self._cumulative_active_time]
 
 
     # *** Optionally override public functions. ***
     def Subfeatures(self) -> List[str]:
-        return ["Total Time"] # >>> fill in names of Subfeatures for which this Feature should extract values. <<<
+        return ["Active"] # >>> fill in names of Subfeatures for which this Feature should extract values. <<<
     
     @staticmethod
     def AvailableModes() -> List[ExtractionMode]:
-        return [ExtractionMode.PLAYER,ExtractionMode.DETECTOR] # >>> delete any modes you don't want run for your Feature. <<<
+        return [ExtractionMode.PLAYER] # >>> delete any modes you don't want run for your Feature. <<<
     
     # @staticmethod
     # def MinVersion() -> Optional[str]:
     #     # >>> replace return statement below with a string defining the minimum logging version for events to be processed by this Feature. <<<
     #     return super().MinVersion()
 
     # @staticmethod
```

### Comparing `opengamedata_core-0.0.2/src/ogd/games/JOURNALISM/features/WorstAttribute.py` & `opengamedata_core-0.0.3/src/ogd/games/JOURNALISM/features/SnippetReceivedCount.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,44 +1,43 @@
 # import libraries
 import json
-from typing import Any, Final, List, Optional
+from typing import Any, List, Optional
 # import local files
 from ogd.core.generators.extractors.Feature import Feature
 from ogd.core.schemas.Event import Event
 from ogd.core.schemas.ExtractionMode import ExtractionMode
 from ogd.core.schemas.FeatureData import FeatureData
 from ogd.core.generators.Generator import GeneratorParameters
 from ogd.core.generators.extractors.SessionFeature import SessionFeature
 
-class WorstAttribute(SessionFeature):
+
+
+
+class SnippetReceivedCount(SessionFeature):
     """Template file to serve as a guide for creating custom Feature subclasses for games.
 
     :param Feature: Base class for a Custom Feature class.
     :type Feature: _type_
     """
     def __init__(self, params:GeneratorParameters):
         super().__init__(params=params)
-        self._min_value : int = 0
-        self._min_names : List[str] = []
-        self._ATTRIBUTE_ENUM : Final[List[str]] = ["endurance", "resourceful", "tech","social","trust","research"]
-        #self._text_click_count : int = 0;
-        # >>> create/initialize any variables to track feature extractor state <<<
-        #
-        # e.g. To track whether extractor found a click event yet:
-        # self._found_click : bool = False
+        choice_type_names = ["BAD", "GOOD", "GREAT"]
+        self._quality_counts = {name: 0 for name in choice_type_names}
+        self._snippet_receive_count : int = 0
+        
 
     # *** IMPLEMENT ABSTRACT FUNCTIONS ***
     @classmethod
     def _eventFilter(cls, mode:ExtractionMode) -> List[str]:
         """_summary_
 
         :return: _description_
         :rtype: List[str]
         """
-        return ["stat_update"] # >>> fill in names of events this Feature should use for extraction. <<<
+        return ["snippet_received"] # >>> fill in names of events this Feature should use for extraction. <<<
 
     @classmethod
     def _featureFilter(cls, mode:ExtractionMode) -> List[str]:
         """_summary_
 
         :return: _description_
         :rtype: List[str]
@@ -47,27 +46,18 @@
 
     def _updateFromEvent(self, event:Event) -> None:
         """_summary_
 
         :param event: _description_
         :type event: Event
         """
-
-        self._min_names = []
-        
-        skill_vals = eval(event.GameState["current_stats"])
-        self._min_value = min(skill_vals)
-        #get lowest val in list 
-        res_list = [i for i in range(len(skill_vals)) if skill_vals[i] == self._min_value]
-
-        for val in res_list:
-            self._min_names.append(self._ATTRIBUTE_ENUM[val])
-
-
-
+        self._snippet_receive_count += 1
+        _quality = event.EventData.get("snippet_quality", "QUALITY NOT FOUND").upper()
+        if _quality is not None and _quality in self._quality_counts.keys():
+            self._quality_counts[_quality] += 1
         return
 
     def _updateFromFeatureData(self, feature: FeatureData):
         """_summary_
 
         :param feature: _description_
         :type feature: FeatureData
@@ -79,38 +69,25 @@
 
     def _getFeatureValues(self) -> List[Any]:
         """_summary_
 
         :return: _description_
         :rtype: List[Any]
         """
-        
-        # >>> use state variables to calculate the return value(s) of the base Feature and any Subfeatures. <<<
-        # >>> put the calculated value(s) into a list as the function return value. <<<
-        # >>> definitely don't return ["template"], unless you really find that useful... <<<
-        #
-        # e.g. use the self._found_click, which was created/initialized in __init__(...), and updated in _updateFromEvent(...):
-        # if self._found_click:
-        #     ret_val = [True]
-        # else:
-        #     ret_val = [False]
-        # return ret_val
-        #
-        # note the code above is redundant, we could just return [self._found_click] to get the same result;
-        # the more-verbose code is here for illustrative purposes.
-        return [self._min_value,self._min_names]
+        return [self._snippet_receive_count, self._quality_counts["BAD"],
+        self._quality_counts["GOOD"], self._quality_counts["GREAT"]]
 
 
     # *** Optionally override public functions. ***
     def Subfeatures(self) -> List[str]:
-        return ["Names"] # >>> fill in names of Subfeatures for which this Feature should extract values. <<<
+        return ["Bad", "Good", "Great"] # >>> fill in names of Subfeatures for which this Feature should extract values. <<<
     
     @staticmethod
     def AvailableModes() -> List[ExtractionMode]:
-        return [ExtractionMode.PLAYER, ExtractionMode.SESSION] # >>> delete any modes you don't want run for your Feature. <<<
+        return [ExtractionMode.POPULATION, ExtractionMode.PLAYER, ExtractionMode.SESSION] # >>> delete any modes you don't want run for your Feature. <<<
     
     # @staticmethod
     # def MinVersion() -> Optional[str]:
     #     # >>> replace return statement below with a string defining the minimum logging version for events to be processed by this Feature. <<<
     #     return super().MinVersion()
 
     # @staticmethod
```

### Comparing `opengamedata_core-0.0.2/src/ogd/games/JOURNALISM/features/WorstPlayerAttribute.py` & `opengamedata_core-0.0.3/src/ogd/games/JOURNALISM/features/WorstPlayerAttribute.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/JOURNALISM/features/__init__.py` & `opengamedata_core-0.0.3/src/ogd/games/JOURNALISM/features/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,25 +4,27 @@
     "SessionPlayTime",
     "SnippetReceivedCount",
     "MeanSnippetTime",
     "StoryCompleteTime",
     "SkillSequenceCount",
     "TotalLevelTime",
     "PlayerAttributes",
+    "FinalAttributes",
     "StoryAlignment",
     "QuitLevel",
     "QuitType",
     "WorstAttribute",
     "WorstPlayerAttribute",
     "TopAttribute",
     "TopPlayerAttribute",
     "MaxedPlayerAttribute",
     "LevelCompleteCount",
     "LevelCompleted",
     "TotalFails",
+    "FailureAttributes",
     "FailureCount",
     "ContinuesOnFail",
     "PlayTime",
     "UserPlayTime",
     "GameComplete",
     "QuitNode",
     "SnippetReplace",
@@ -45,26 +47,28 @@
 from . import ChoiceClickCount
 from . import SessionPlayTime
 from . import SnippetReceivedCount
 from . import MeanSnippetTime
 from . import StoryCompleteTime
 from . import SkillSequenceCount
 from . import TotalLevelTime
+from . import FinalAttributes
 from . import PlayerAttributes
 from . import StoryAlignment
 from . import QuitLevel
 from . import QuitType
 from . import WorstAttribute
 from . import WorstPlayerAttribute
 from . import TopAttribute
 from . import TopPlayerAttribute
 from . import MaxedPlayerAttribute
 from . import LevelCompleteCount
 from . import LevelCompleted
 from . import TotalFails
+from . import FailureAttributes
 from . import FailureCount
 from . import ContinuesOnFail
 from . import PlayTime
 from . import UserPlayTime
 from . import GameComplete
 from . import QuitNode
 from . import SnippetReplace
```

### Comparing `opengamedata_core-0.0.2/src/ogd/games/JOURNALISM/schemas/JOURNALISM.json.template` & `opengamedata_core-0.0.3/src/ogd/games/JOURNALISM/schemas/JOURNALISM.json.template`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/JOWILDER/JowilderLoader.py` & `opengamedata_core-0.0.3/src/ogd/games/JOWILDER/JowilderLoader.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/JOWILDER/Jowilder_Enumerators.py` & `opengamedata_core-0.0.3/src/ogd/games/JOWILDER/Jowilder_Enumerators.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/JOWILDER/features/ActiveStateTime.py` & `opengamedata_core-0.0.3/src/ogd/games/JOWILDER/features/ActiveStateTime.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/JOWILDER/features/Clicks.py` & `opengamedata_core-0.0.3/src/ogd/games/JOWILDER/features/Clicks.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/JOWILDER/features/EventCount.py` & `opengamedata_core-0.0.3/src/ogd/games/JOWILDER/features/EventCount.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/JOWILDER/features/FirstInteraction.py` & `opengamedata_core-0.0.3/src/ogd/games/JOWILDER/features/FirstInteraction.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/JOWILDER/features/GameScript.py` & `opengamedata_core-0.0.3/src/ogd/games/JOWILDER/features/GameScript.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/JOWILDER/features/GameVersion.py` & `opengamedata_core-0.0.3/src/ogd/games/JOWILDER/features/GameVersion.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/JOWILDER/features/Hovers.py` & `opengamedata_core-0.0.3/src/ogd/games/JOWILDER/features/Hovers.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/JOWILDER/features/IdleState.py` & `opengamedata_core-0.0.3/src/ogd/games/JOWILDER/features/IdleState.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/JOWILDER/features/Interaction.py` & `opengamedata_core-0.0.3/src/ogd/games/JOWILDER/features/Interaction.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/JOWILDER/features/InteractionName.py` & `opengamedata_core-0.0.3/src/ogd/games/JOWILDER/features/InteractionName.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/JOWILDER/features/InteractionTextBoxesPerSecond.py` & `opengamedata_core-0.0.3/src/ogd/games/JOWILDER/features/InteractionTextBoxesPerSecond.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/JOWILDER/features/InteractionWordsPerSecond.py` & `opengamedata_core-0.0.3/src/ogd/games/JOWILDER/features/InteractionWordsPerSecond.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/JOWILDER/features/LastInteraction.py` & `opengamedata_core-0.0.3/src/ogd/games/JOWILDER/features/LastInteraction.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/JOWILDER/features/MeaningfulActions.py` & `opengamedata_core-0.0.3/src/ogd/games/JOWILDER/features/MeaningfulActions.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/JOWILDER/features/NotebookUses.py` & `opengamedata_core-0.0.3/src/ogd/games/JOWILDER/features/NotebookUses.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/JOWILDER/features/QuestionAnswers.py` & `opengamedata_core-0.0.3/src/ogd/games/JOWILDER/features/QuestionAnswers.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/JOWILDER/features/SessionDuration.py` & `opengamedata_core-0.0.3/src/ogd/games/JOWILDER/features/SessionDuration.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/JOWILDER/features/SessionStart.py` & `opengamedata_core-0.0.3/src/ogd/games/JOWILDER/features/UsedContinue.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,58 +1,46 @@
 # import libraries
-from typing import Any, List, Optional
+from typing import Any, Final, List, Optional
 from ogd.core.generators.Generator import GeneratorParameters
-from datetime import date, datetime, time
 # import local files
 from ogd.core.generators.extractors.SessionFeature import SessionFeature
 from ogd.core.schemas.ExtractionMode import ExtractionMode
 from ogd.core.schemas.FeatureData import FeatureData
 from ogd.core.schemas.Event import Event
 
-class SessionStart(SessionFeature):
+class UsedContinue(SessionFeature):
     """Template file to serve as a guide for creating custom Feature subclasses for games.
 
     :param Feature: Base class for a Custom Feature class.
     :type Feature: _type_
     """
+
+    START_SIGN : Final[str] = "tunic.historicalsociety.closet.gramps.intro_0_cs_0"
+
     def __init__(self, params:GeneratorParameters):
         super().__init__(params=params)
-        self._date : Optional[date] = None
-        self._time : Optional[time] = None
-        self._year : Optional[int] = None
-        self._month : Optional[int] = None
-        self._hour : Optional[int] = None
+        self._continue : int = 0
 
     # *** IMPLEMENT ABSTRACT FUNCTIONS ***
 
     @classmethod
     def _eventFilter(cls, mode:ExtractionMode) -> List[str]:
-        return ["CUSTOM.1"]
+        return []
 
     @classmethod
     def _featureFilter(cls, mode:ExtractionMode) -> List[str]:
-        return [] 
+        return ["FirstInteraction", "UsedSaveCode"] 
 
     def _updateFromEvent(self, event:Event) -> None:
-        event_time = event.Timestamp
-        if not self._date:
-            self._date = event_time.date()
-            self._time = event_time.time()
-            self._hour = event_time.hour
-            self._year = event_time.year
-            self._month = event_time.month
-
-
         return
 
     def _updateFromFeatureData(self, feature: FeatureData):
+        if feature.FeatureType == "UsedSaveCode":
+            self._save_code = feature.FeatureValues[0]
+        elif feature.FeatureType == "FirstInteraction":
+            self._first_inc = feature.FeatureValues[0]
         return
 
     def _getFeatureValues(self) -> List[Any]:
-        return [self._date, self._time, self._year, self._month, self._hour]
-
-    def Subfeatures(self) -> List[str]:
-        return ["Time", "Year", "Month", "Hour"]
-
-    def BaseFeatureSuffix(self) -> str:
-        return "Date"
-
+        if not self._save_code and self._first_inc != UsedContinue.START_SIGN:
+            self._continue = 1
+        return [self._continue]
```

### Comparing `opengamedata_core-0.0.2/src/ogd/games/JOWILDER/features/SurveyItem.py` & `opengamedata_core-0.0.3/src/ogd/games/JOWILDER/features/SurveyItem.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/JOWILDER/features/SurveyTime.py` & `opengamedata_core-0.0.3/src/ogd/games/JOWILDER/features/SurveyTime.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/JOWILDER/features/UsedContinue.py` & `opengamedata_core-0.0.3/src/ogd/games/AQUALAB/features/RegionName.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,46 +1,40 @@
 # import libraries
-from typing import Any, Final, List, Optional
-from ogd.core.generators.Generator import GeneratorParameters
-# import local files
-from ogd.core.generators.extractors.SessionFeature import SessionFeature
+from typing import Any, List, Optional
+# import locals
+from ogd.core.generators.extractors.Extractor import GeneratorParameters
+from ogd.core.schemas.Event import Event
 from ogd.core.schemas.ExtractionMode import ExtractionMode
 from ogd.core.schemas.FeatureData import FeatureData
-from ogd.core.schemas.Event import Event
-
-class UsedContinue(SessionFeature):
-    """Template file to serve as a guide for creating custom Feature subclasses for games.
-
-    :param Feature: Base class for a Custom Feature class.
-    :type Feature: _type_
-    """
-
-    START_SIGN : Final[str] = "tunic.historicalsociety.closet.gramps.intro_0_cs_0"
+from ogd.core.generators.extractors.PerCountFeature import PerCountFeature
 
+class RegionName(PerCountFeature):
     def __init__(self, params:GeneratorParameters):
         super().__init__(params=params)
-        self._continue : int = 0
-
+        regions = ['arctic', 'coral', 'bayou', 'kelp', 'other']
+        self.count = 0
+        self.region = regions[self.CountIndex]
     # *** IMPLEMENT ABSTRACT FUNCTIONS ***
-
     @classmethod
     def _eventFilter(cls, mode:ExtractionMode) -> List[str]:
         return []
 
     @classmethod
     def _featureFilter(cls, mode:ExtractionMode) -> List[str]:
-        return ["FirstInteraction", "UsedSaveCode"] 
+        return []
+
+    def _validateEventCountIndex(self, event:Event):
+        pass
 
     def _updateFromEvent(self, event:Event) -> None:
-        return
+        pass
 
-    def _updateFromFeatureData(self, feature: FeatureData):
-        if feature.FeatureType == "UsedSaveCode":
-            self._save_code = feature.FeatureValues[0]
-        elif feature.FeatureType == "FirstInteraction":
-            self._first_inc = feature.FeatureValues[0]
+    def _updateFromFeatureData(self, feature:FeatureData):
         return
 
     def _getFeatureValues(self) -> List[Any]:
-        if not self._save_code and self._first_inc != UsedContinue.START_SIGN:
-            self._continue = 1
-        return [self._continue]
+        return [self.region]
+
+    # *** Optionally override public functions. ***
+    @staticmethod
+    def MinVersion() -> Optional[str]:
+        return "1"
```

### Comparing `opengamedata_core-0.0.2/src/ogd/games/JOWILDER/features/UsedSaveCode.py` & `opengamedata_core-0.0.3/src/ogd/games/JOWILDER/features/UsedSaveCode.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/JOWILDER/features/UserEnabled.py` & `opengamedata_core-0.0.3/src/ogd/games/JOWILDER/features/UserEnabled.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/JOWILDER/features/__init__.py` & `opengamedata_core-0.0.3/src/ogd/games/JOWILDER/features/__init__.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/JOWILDER/get_jowilder_all_items.py` & `opengamedata_core-0.0.3/src/ogd/games/JOWILDER/get_jowilder_all_items.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/JOWILDER/schemas/JOWILDER.json.template` & `opengamedata_core-0.0.3/src/ogd/games/JOWILDER/schemas/JOWILDER.json.template`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/LAKELAND/LakelandLoader.py` & `opengamedata_core-0.0.3/src/ogd/games/LAKELAND/LakelandLoader.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/LAKELAND/features/ActionsLastXSecondsModel.py` & `opengamedata_core-0.0.3/src/ogd/games/LAKELAND/features/ActionsLastXSecondsModel.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/LAKELAND/features/DeathCountModel.py` & `opengamedata_core-0.0.3/src/ogd/games/LAKELAND/features/DeathCountModel.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/LAKELAND/features/DeathPredModel.py` & `opengamedata_core-0.0.3/src/ogd/games/LAKELAND/features/DeathPredModel.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/LAKELAND/features/DeathThresholdModel.py` & `opengamedata_core-0.0.3/src/ogd/games/LAKELAND/features/DeathThresholdModel.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/LAKELAND/features/DiagonalFarmDetectorModel.py` & `opengamedata_core-0.0.3/src/ogd/games/LAKELAND/features/DiagonalFarmDetectorModel.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/LAKELAND/features/FeatSeqPercent.py` & `opengamedata_core-0.0.3/src/ogd/games/LAKELAND/features/FeatSeqPercent.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/LAKELAND/features/FeatVelocity.py` & `opengamedata_core-0.0.3/src/ogd/games/LAKELAND/features/FeatVelocity.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/LAKELAND/features/FeatureModel.py` & `opengamedata_core-0.0.3/src/ogd/games/LAKELAND/features/FeatureModel.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/LAKELAND/features/LAKELAND_models.json` & `opengamedata_core-0.0.3/src/ogd/games/LAKELAND/features/LAKELAND_models.json`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/LAKELAND/features/LakelandEnumerators.json` & `opengamedata_core-0.0.3/src/ogd/games/LAKELAND/features/LakelandEnumerators.json`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/LAKELAND/features/LakelandExtractor.py` & `opengamedata_core-0.0.3/src/ogd/games/LAKELAND/features/LakelandExtractor.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/LAKELAND/features/LinearModel.py` & `opengamedata_core-0.0.3/src/ogd/games/LAKELAND/features/LinearModel.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/LAKELAND/features/LogisticModel.py` & `opengamedata_core-0.0.3/src/ogd/games/LAKELAND/features/LogisticModel.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/LAKELAND/features/MapSummaryModel.py` & `opengamedata_core-0.0.3/src/ogd/games/LAKELAND/features/MapSummaryModel.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/LAKELAND/features/Model.py` & `opengamedata_core-0.0.3/src/ogd/games/LAKELAND/features/Model.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/LAKELAND/features/MoneyAccumulationModel.py` & `opengamedata_core-0.0.3/src/ogd/games/LAKELAND/features/MoneyAccumulationModel.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/LAKELAND/features/PopulationModel.py` & `opengamedata_core-0.0.3/src/ogd/games/LAKELAND/features/PopulationModel.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/LAKELAND/features/RecentPurchasesModel.py` & `opengamedata_core-0.0.3/src/ogd/games/LAKELAND/features/RecentPurchasesModel.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/LAKELAND/features/SequenceModel.py` & `opengamedata_core-0.0.3/src/ogd/games/LAKELAND/features/SequenceModel.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/LAKELAND/features/SimpleFarmAbandonmentModel.py` & `opengamedata_core-0.0.3/src/ogd/games/LAKELAND/features/SimpleFarmAbandonmentModel.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/LAKELAND/features/SingleFeatureModel.py` & `opengamedata_core-0.0.3/src/ogd/games/LAKELAND/features/SingleFeatureModel.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/LAKELAND/features/TimeSinceEventTypes.py` & `opengamedata_core-0.0.3/src/ogd/games/LAKELAND/features/TimeSinceEventTypes.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/LAKELAND/features/TimeSinceLastSaleModel.py` & `opengamedata_core-0.0.3/src/ogd/games/LAKELAND/features/TimeSinceLastSaleModel.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/LAKELAND/features/TownCompositionModel.py` & `opengamedata_core-0.0.3/src/ogd/games/LAKELAND/features/TownCompositionModel.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/LAKELAND/features/TutorialProgressionModel.py` & `opengamedata_core-0.0.3/src/ogd/games/LAKELAND/features/TutorialProgressionModel.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/LAKELAND/features/WAVES_models.json` & `opengamedata_core-0.0.3/src/ogd/games/LAKELAND/features/WAVES_models.json`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/LAKELAND/features/WAVES_models_L8_Q0_Q1.json` & `opengamedata_core-0.0.3/src/ogd/games/LAKELAND/features/WAVES_models_L8_Q0_Q1.json`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/LAKELAND/features/WAVES_models_L8_and_Q0.json` & `opengamedata_core-0.0.3/src/ogd/games/LAKELAND/features/WAVES_models_L8_and_Q0.json`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/LAKELAND/features/WAVES_models_L8_complete_and_current.json` & `opengamedata_core-0.0.3/src/ogd/games/LAKELAND/features/WAVES_models_L8_complete_and_current.json`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/LAKELAND/features/WAVES_models_L8_only_complete.json` & `opengamedata_core-0.0.3/src/ogd/games/LAKELAND/features/WAVES_models_L8_only_complete.json`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/LAKELAND/produce_lakeland_enumerators.py` & `opengamedata_core-0.0.3/src/ogd/games/LAKELAND/produce_lakeland_enumerators.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/LAKELAND/schemas/LAKELAND.json.template` & `opengamedata_core-0.0.3/src/ogd/games/LAKELAND/schemas/LAKELAND.json.template`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/MAGNET/MagnetLoader.py` & `opengamedata_core-0.0.3/src/ogd/games/MAGNET/MagnetLoader.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/MAGNET/features/MagnetExtractor.py` & `opengamedata_core-0.0.3/src/ogd/games/MAGNET/features/MagnetExtractor.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/MAGNET/schemas/MAGNET.json.template` & `opengamedata_core-0.0.3/src/ogd/games/MAGNET/schemas/MAGNET.json.template`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/MASHOPOLIS/schemas/MASHOPOLIS.json.template` & `opengamedata_core-0.0.3/src/ogd/games/MASHOPOLIS/schemas/MASHOPOLIS.json.template`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/PENGUINS/DBExport.json` & `opengamedata_core-0.0.3/src/ogd/games/PENGUINS/DBExport.json`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/PENGUINS/PenguinsLoader.py` & `opengamedata_core-0.0.3/src/ogd/games/PENGUINS/PenguinsLoader.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/PENGUINS/detectors/RegionEnter.py` & `opengamedata_core-0.0.3/src/ogd/games/PENGUINS/detectors/RegionEnter.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/PENGUINS/detectors/RegionExit.py` & `opengamedata_core-0.0.3/src/ogd/games/PENGUINS/detectors/RegionExit.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/PENGUINS/features/ActivityCompleted.py` & `opengamedata_core-0.0.3/src/ogd/games/PENGUINS/features/ActivityCompleted.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/PENGUINS/features/ActivityDuration.py` & `opengamedata_core-0.0.3/src/ogd/games/PENGUINS/features/ActivityDuration.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/PENGUINS/features/EatFishCount.py` & `opengamedata_core-0.0.3/src/ogd/games/PENGUINS/features/EatFishCount.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/PENGUINS/features/EggLostCount.py` & `opengamedata_core-0.0.3/src/ogd/games/PENGUINS/features/EggLostCount.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/PENGUINS/features/EggRecoverTime.py` & `opengamedata_core-0.0.3/src/ogd/games/PENGUINS/features/EggRecoverTime.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/PENGUINS/features/GazeCount.py` & `opengamedata_core-0.0.3/src/ogd/games/PENGUINS/features/GazeCount.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/PENGUINS/features/GazeDuration.py` & `opengamedata_core-0.0.3/src/ogd/games/PENGUINS/features/GazeDuration.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/PENGUINS/features/MirrorWaddleDuration.py` & `opengamedata_core-0.0.3/src/ogd/games/PENGUINS/features/MirrorWaddleDuration.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/PENGUINS/features/PerRegionFeature.py` & `opengamedata_core-0.0.3/src/ogd/games/PENGUINS/features/PerRegionFeature.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/PENGUINS/features/PickupRockCount.py` & `opengamedata_core-0.0.3/src/ogd/games/PENGUINS/features/PickupRockCount.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/PENGUINS/features/PlayerInactiveAvgDuration.py` & `opengamedata_core-0.0.3/src/ogd/games/PENGUINS/features/PlayerInactiveAvgDuration.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/PENGUINS/features/PlayerWaddleCount.py` & `opengamedata_core-0.0.3/src/ogd/games/PENGUINS/features/PlayerWaddleCount.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/PENGUINS/features/RegionDuration.py` & `opengamedata_core-0.0.3/src/ogd/games/PENGUINS/features/RegionDuration.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/PENGUINS/features/RegionEnterCount.py` & `opengamedata_core-0.0.3/src/ogd/games/PENGUINS/features/RegionEnterCount.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/PENGUINS/features/RegionsEncountered.py` & `opengamedata_core-0.0.3/src/ogd/games/PENGUINS/features/RegionsEncountered.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/PENGUINS/features/RingChimesCount.py` & `opengamedata_core-0.0.3/src/ogd/games/PENGUINS/features/RingChimesCount.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/PENGUINS/features/SessionDuration.py` & `opengamedata_core-0.0.3/src/ogd/games/PENGUINS/features/SessionDuration.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/PENGUINS/features/WaddlePerRegion.py` & `opengamedata_core-0.0.3/src/ogd/games/PENGUINS/features/WaddlePerRegion.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/PENGUINS/features/__init__.py` & `opengamedata_core-0.0.3/src/ogd/games/PENGUINS/features/__init__.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/PENGUINS/schemas/PENGUINS.json.template` & `opengamedata_core-0.0.3/src/ogd/games/PENGUINS/schemas/PENGUINS.json.template`

 * *Files 10% similar despite different names*

```diff
@@ -1,1507 +1,1773 @@
 00000000: 7b0a 2020 2020 226c 6576 656c 5f72 616e  {.    "level_ran
 00000010: 6765 223a 207b 0a20 2020 2020 2020 2022  ge": {.        "
 00000020: 6d69 6e22 3a20 312c 0a20 2020 2020 2020  min": 1,.       
 00000030: 2022 6d61 7822 3a20 360a 2020 2020 7d2c   "max": 6.    },
-00000040: 0a20 2020 2022 6761 6d65 5f73 7461 7465  .    "game_state
-00000050: 223a 207b 0a20 2020 2020 2020 2022 7365  ": {.        "se
-00000060: 636f 6e64 735f 6672 6f6d 5f6c 6175 6e63  conds_from_launc
-00000070: 6822 3a20 7b0a 2020 2020 2020 2020 2020  h": {.          
-00000080: 2020 2274 7970 6522 3a20 2266 6c6f 6174    "type": "float
-00000090: 222c 0a20 2020 2020 2020 2020 2020 2022  ",.            "
-000000a0: 6465 7363 7269 7074 696f 6e22 3a20 2254  description": "T
-000000b0: 6865 206e 756d 6265 7220 6f66 2073 6563  he number of sec
-000000c0: 6f6e 6473 206f 6620 6761 6d65 2074 696d  onds of game tim
-000000d0: 6520 656c 6170 7365 6420 7369 6e63 6520  e elapsed since 
-000000e0: 7468 6520 6761 6d65 2077 6173 206c 6175  the game was lau
-000000f0: 6e63 6865 642c 202a 6e6f 7420 696e 636c  nched, *not incl
-00000100: 7564 696e 6720 7469 6d65 2077 6865 6e20  uding time when 
-00000110: 7468 6520 6761 6d65 2077 6173 2070 6175  the game was pau
-00000120: 7365 642a 2e22 0a20 2020 2020 2020 207d  sed*.".        }
-00000130: 2c0a 2020 2020 2020 2020 2270 6f73 223a  ,.        "pos":
-00000140: 207b 0a20 2020 2020 2020 2020 2020 2022   {.            "
-00000150: 7479 7065 223a 2022 4c69 7374 5b66 6c6f  type": "List[flo
-00000160: 6174 5d22 2c0a 2020 2020 2020 2020 2020  at]",.          
-00000170: 2020 2264 6573 6372 6970 7469 6f6e 223a    "description":
-00000180: 2022 5468 6520 6375 7272 656e 7420 706f   "The current po
-00000190: 7369 7469 6f6e 206f 6620 7468 6520 706c  sition of the pl
-000001a0: 6179 6572 2068 6561 6473 6574 2061 7420  ayer headset at 
-000001b0: 7468 6520 6d6f 6d65 6e74 2074 6865 2065  the moment the e
-000001c0: 7665 6e74 206f 6363 7572 7265 642c 2066  vent occurred, f
-000001d0: 6f72 6d61 7474 6564 2061 7320 5b78 2c20  ormatted as [x, 
-000001e0: 792c 207a 5d22 0a20 2020 2020 2020 207d  y, z]".        }
-000001f0: 2c0a 2020 2020 2020 2020 2272 6f74 223a  ,.        "rot":
-00000200: 207b 0a20 2020 2020 2020 2020 2020 2022   {.            "
-00000210: 7479 7065 223a 2022 4c69 7374 5b66 6c6f  type": "List[flo
-00000220: 6174 5d22 2c0a 2020 2020 2020 2020 2020  at]",.          
-00000230: 2020 2264 6573 6372 6970 7469 6f6e 223a    "description":
-00000240: 2022 5468 6520 6375 7272 656e 7420 6f72   "The current or
-00000250: 6965 6e74 6174 696f 6e20 6f66 2074 6865  ientation of the
-00000260: 2070 6c61 7965 7220 6865 6164 7365 7420   player headset 
-00000270: 6174 2074 6865 206d 6f6d 656e 7420 7468  at the moment th
-00000280: 6520 6576 656e 7420 6f63 6375 7272 6564  e event occurred
-00000290: 2c20 666f 726d 6174 7465 6420 6173 205b  , formatted as [
-000002a0: 782c 2079 2c20 7a2c 2077 5d22 0a20 2020  x, y, z, w]".   
-000002b0: 2020 2020 207d 2c0a 2020 2020 2020 2020       },.        
-000002c0: 2268 6173 5f72 6f63 6b22 3a20 7b0a 2020  "has_rock": {.  
-000002d0: 2020 2020 2020 2020 2020 2274 7970 6522            "type"
-000002e0: 3a20 2262 6f6f 6c22 2c0a 2020 2020 2020  : "bool",.      
-000002f0: 2020 2020 2020 2264 6573 6372 6970 7469        "descripti
-00000300: 6f6e 223a 2022 5768 6574 6865 7220 7468  on": "Whether th
-00000310: 6520 706c 6179 6572 2077 6173 2068 6f6c  e player was hol
-00000320: 6469 6e67 2061 2072 6f63 6b20 696e 2074  ding a rock in t
-00000330: 6865 6972 2062 6561 6b20 6174 2074 6865  heir beak at the
-00000340: 2074 696d 6520 7468 6520 6576 656e 7420   time the event 
-00000350: 6f63 6375 7272 6564 2e22 0a20 2020 2020  occurred.".     
-00000360: 2020 207d 0a20 2020 207d 2c0a 2020 2020     }.    },.    
-00000370: 2265 7665 6e74 7322 3a20 7b0a 2020 2020  "events": {.    
-00000380: 2020 2020 2273 6573 7369 6f6e 5f73 7461      "session_sta
-00000390: 7274 223a 207b 0a20 2020 2020 2020 2020  rt": {.         
-000003a0: 2020 2022 6465 7363 7269 7074 696f 6e22     "description"
-000003b0: 3a20 2257 6865 6e20 7468 6520 6170 7020  : "When the app 
-000003c0: 6973 2073 7461 7274 6564 2061 6e64 2074  is started and t
-000003d0: 6865 2067 616d 6570 6c61 7920 7365 7373  he gameplay sess
-000003e0: 696f 6e20 6973 2061 7373 6967 6e65 6420  ion is assigned 
-000003f0: 6120 7365 7373 696f 6e20 4944 2e20 5468  a session ID. Th
-00000400: 6520 706c 6179 6572 2068 6173 206e 6f74  e player has not
-00000410: 206e 6563 6573 7361 7269 6c79 2062 6567   necessarily beg
-00000420: 756e 2074 6865 2067 616d 6520 6974 7365  un the game itse
-00000430: 6c66 2079 6574 2e22 2c0a 2020 2020 2020  lf yet.",.      
-00000440: 2020 2020 2020 2265 7665 6e74 5f64 6174        "event_dat
-00000450: 6122 3a20 7b0a 2020 2020 2020 2020 2020  a": {.          
-00000460: 2020 2020 2020 2272 616e 646f 6d5f 7365        "random_se
-00000470: 6564 223a 2022 5468 6520 7261 6e64 6f6d  ed": "The random
-00000480: 2073 6565 6420 7573 6564 2066 6f72 2061   seed used for a
-00000490: 6c6c 2072 616e 646f 6d20 6e75 6d62 6572  ll random number
-000004a0: 2f70 6f73 6974 696f 6e2f 726f 7461 7469  /position/rotati
-000004b0: 6f6e 2067 656e 6572 6174 696f 6e20 696e  on generation in
-000004c0: 2074 6865 2067 616d 652e 220a 2020 2020   the game.".    
-000004d0: 2020 2020 2020 2020 7d0a 2020 2020 2020          }.      
-000004e0: 2020 7d2c 0a20 2020 2020 2020 2022 6761    },.        "ga
-000004f0: 6d65 5f73 7461 7274 223a 207b 0a20 2020  me_start": {.   
-00000500: 2020 2020 2020 2020 2022 6465 7363 7269           "descri
-00000510: 7074 696f 6e22 3a20 2257 6865 6e20 6120  ption": "When a 
-00000520: 6e65 7720 6761 6d65 2069 7320 7374 6172  new game is star
-00000530: 7465 6422 2c0a 2020 2020 2020 2020 2020  ted",.          
-00000540: 2020 2265 7665 6e74 5f64 6174 6122 3a20    "event_data": 
-00000550: 7b0a 2020 2020 2020 2020 2020 2020 2020  {.              
-00000560: 2020 226d 6f64 6522 3a20 7b0a 2020 2020    "mode": {.    
+00000040: 0a20 2020 2022 656e 756d 7322 203a 207b  .    "enums" : {
+00000050: 0a20 2020 2020 2020 2022 4761 6d65 4d6f  .        "GameMo
+00000060: 6465 2220 3a20 5b22 484f 4d45 5f4d 4f44  de" : ["HOME_MOD
+00000070: 4522 2c20 222e 2e2e 225d 2c0a 2020 2020  E", "..."],.    
+00000080: 2020 2020 224d 6f76 6554 7970 6522 203a      "MoveType" :
+00000090: 205b 2242 5554 544f 4e22 2c20 2257 4144   ["BUTTON", "WAD
+000000a0: 444c 4522 5d2c 0a20 2020 2020 2020 2022  DLE"],.        "
+000000b0: 4163 7469 7669 7479 2220 3a20 5b22 736b  Activity" : ["sk
+000000c0: 7561 7322 2c20 226d 6174 696e 675f 6461  uas", "mating_da
+000000d0: 6e63 6522 2c20 226e 6573 7422 2c20 222e  nce", "nest", ".
+000000e0: 2e2e 225d 2c0a 2020 2020 2020 2020 2248  .."],.        "H
+000000f0: 616e 6422 2020 2020 203a 205b 224c 4546  and"     : ["LEF
+00000100: 5422 2c20 2252 4947 4854 225d 0a20 2020  T", "RIGHT"].   
+00000110: 207d 2c0a 2020 2020 2267 616d 655f 7374   },.    "game_st
+00000120: 6174 6522 3a20 7b0a 2020 2020 2020 2020  ate": {.        
+00000130: 2268 6173 5f72 6f63 6b22 3a20 7b0a 2020  "has_rock": {.  
+00000140: 2020 2020 2020 2020 2020 2274 7970 6522            "type"
+00000150: 3a20 2262 6f6f 6c22 2c0a 2020 2020 2020  : "bool",.      
+00000160: 2020 2020 2020 2264 6573 6372 6970 7469        "descripti
+00000170: 6f6e 223a 2022 5768 6574 6865 7220 7468  on": "Whether th
+00000180: 6520 706c 6179 6572 2077 6173 2068 6f6c  e player was hol
+00000190: 6469 6e67 2061 2072 6f63 6b20 696e 2074  ding a rock in t
+000001a0: 6865 6972 2062 6561 6b20 6174 2074 6865  heir beak at the
+000001b0: 2074 696d 6520 7468 6520 6576 656e 7420   time the event 
+000001c0: 6f63 6375 7272 6564 2e22 0a20 2020 2020  occurred.".     
+000001d0: 2020 207d 2c0a 2020 2020 2020 2020 2270     },.        "p
+000001e0: 6f73 223a 207b 0a20 2020 2020 2020 2020  os": {.         
+000001f0: 2020 2022 7479 7065 223a 2022 4c69 7374     "type": "List
+00000200: 5b66 6c6f 6174 5d22 2c0a 2020 2020 2020  [float]",.      
+00000210: 2020 2020 2020 2264 6573 6372 6970 7469        "descripti
+00000220: 6f6e 223a 2022 5468 6520 6375 7272 656e  on": "The curren
+00000230: 7420 706f 7369 7469 6f6e 206f 6620 7468  t position of th
+00000240: 6520 706c 6179 6572 2068 6561 6473 6574  e player headset
+00000250: 2061 7420 7468 6520 6d6f 6d65 6e74 2074   at the moment t
+00000260: 6865 2065 7665 6e74 206f 6363 7572 7265  he event occurre
+00000270: 642c 2066 6f72 6d61 7474 6564 2061 7320  d, formatted as 
+00000280: 5b78 2c20 792c 207a 5d22 0a20 2020 2020  [x, y, z]".     
+00000290: 2020 207d 2c0a 2020 2020 2020 2020 2272     },.        "r
+000002a0: 6f74 223a 207b 0a20 2020 2020 2020 2020  ot": {.         
+000002b0: 2020 2022 7479 7065 223a 2022 4c69 7374     "type": "List
+000002c0: 5b66 6c6f 6174 5d22 2c0a 2020 2020 2020  [float]",.      
+000002d0: 2020 2020 2020 2264 6573 6372 6970 7469        "descripti
+000002e0: 6f6e 223a 2022 5468 6520 6375 7272 656e  on": "The curren
+000002f0: 7420 6f72 6965 6e74 6174 696f 6e20 6f66  t orientation of
+00000300: 2074 6865 2070 6c61 7965 7220 6865 6164   the player head
+00000310: 7365 7420 6174 2074 6865 206d 6f6d 656e  set at the momen
+00000320: 7420 7468 6520 6576 656e 7420 6f63 6375  t the event occu
+00000330: 7272 6564 2c20 666f 726d 6174 7465 6420  rred, formatted 
+00000340: 6173 205b 782c 2079 2c20 7a2c 2077 5d22  as [x, y, z, w]"
+00000350: 0a20 2020 2020 2020 207d 2c0a 2020 2020  .        },.    
+00000360: 2020 2020 2273 6563 6f6e 6473 5f66 726f      "seconds_fro
+00000370: 6d5f 6c61 756e 6368 223a 207b 0a20 2020  m_launch": {.   
+00000380: 2020 2020 2020 2020 2022 7479 7065 223a           "type":
+00000390: 2022 666c 6f61 7422 2c0a 2020 2020 2020   "float",.      
+000003a0: 2020 2020 2020 2264 6573 6372 6970 7469        "descripti
+000003b0: 6f6e 223a 2022 5468 6520 6e75 6d62 6572  on": "The number
+000003c0: 206f 6620 7365 636f 6e64 7320 6f66 2067   of seconds of g
+000003d0: 616d 6520 7469 6d65 2065 6c61 7073 6564  ame time elapsed
+000003e0: 2073 696e 6365 2074 6865 2067 616d 6520   since the game 
+000003f0: 7761 7320 6c61 756e 6368 6564 2c20 2a6e  was launched, *n
+00000400: 6f74 2069 6e63 6c75 6469 6e67 2074 696d  ot including tim
+00000410: 6520 7768 656e 2074 6865 2067 616d 6520  e when the game 
+00000420: 7761 7320 7061 7573 6564 2a2e 220a 2020  was paused*.".  
+00000430: 2020 2020 2020 7d0a 2020 2020 7d2c 0a20        }.    },. 
+00000440: 2020 2022 6576 656e 7473 223a 207b 0a20     "events": {. 
+00000450: 2020 2020 2020 2022 7365 7373 696f 6e5f         "session_
+00000460: 7374 6172 7422 3a20 7b0a 2020 2020 2020  start": {.      
+00000470: 2020 2020 2020 2264 6573 6372 6970 7469        "descripti
+00000480: 6f6e 223a 2022 5768 656e 2074 6865 2061  on": "When the a
+00000490: 7070 2069 7320 7374 6172 7465 6420 616e  pp is started an
+000004a0: 6420 7468 6520 6761 6d65 706c 6179 2073  d the gameplay s
+000004b0: 6573 7369 6f6e 2069 7320 6173 7369 676e  ession is assign
+000004c0: 6564 2061 2073 6573 7369 6f6e 2049 442e  ed a session ID.
+000004d0: 2054 6865 2070 6c61 7965 7220 6861 7320   The player has 
+000004e0: 6e6f 7420 6e65 6365 7373 6172 696c 7920  not necessarily 
+000004f0: 6265 6775 6e20 7468 6520 6761 6d65 2069  begun the game i
+00000500: 7473 656c 6620 7965 742e 222c 0a20 2020  tself yet.",.   
+00000510: 2020 2020 2020 2020 2022 6576 656e 745f           "event_
+00000520: 6461 7461 223a 207b 0a20 2020 2020 2020  data": {.       
+00000530: 2020 2020 2020 2020 2022 7261 6e64 6f6d           "random
+00000540: 5f73 6565 6422 3a20 7b0a 2020 2020 2020  _seed": {.      
+00000550: 2020 2020 2020 2020 2020 2020 2020 2274                "t
+00000560: 7970 6522 3a20 2269 6e74 222c 0a20 2020  ype": "int",.   
 00000570: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000580: 2274 7970 6522 3a20 2265 6e75 6d28 484f  "type": "enum(HO
-00000590: 4d45 5f4d 4f44 452c 202e 2e2e 2922 2c0a  ME_MODE, ...)",.
-000005a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000005b0: 2020 2020 2264 6573 6372 6970 7469 6f6e      "description
-000005c0: 223a 2022 5468 6520 6761 6d65 206d 6f64  ": "The game mod
-000005d0: 6520 7468 6174 2074 6865 2070 6c61 7965  e that the playe
-000005e0: 7220 6c61 756e 6368 6564 220a 2020 2020  r launched".    
-000005f0: 2020 2020 2020 2020 2020 2020 7d0a 2020              }.  
-00000600: 2020 2020 2020 2020 2020 7d0a 2020 2020            }.    
-00000610: 2020 2020 7d2c 0a20 2020 2020 2020 2022      },.        "
-00000620: 6f70 656e 5f6d 656e 7522 3a20 7b0a 2020  open_menu": {.  
-00000630: 2020 2020 2020 2020 2020 2264 6573 6372            "descr
-00000640: 6970 7469 6f6e 223a 2022 5768 656e 2074  iption": "When t
-00000650: 6865 2070 6c61 7965 7220 6f70 656e 7320  he player opens 
-00000660: 7468 6520 6761 6d65 206d 656e 7522 2c0a  the game menu",.
-00000670: 2020 2020 2020 2020 2020 2020 2265 7665              "eve
-00000680: 6e74 5f64 6174 6122 3a20 7b7d 0a20 2020  nt_data": {}.   
-00000690: 2020 2020 207d 2c0a 2020 2020 2020 2020       },.        
-000006a0: 2263 6c6f 7365 5f6d 656e 7522 3a20 7b0a  "close_menu": {.
-000006b0: 2020 2020 2020 2020 2020 2020 2264 6573              "des
-000006c0: 6372 6970 7469 6f6e 223a 2022 5768 656e  cription": "When
-000006d0: 2074 6865 2070 6c61 7965 7220 636c 6f73   the player clos
-000006e0: 6573 2074 6865 2067 616d 6520 6d65 6e75  es the game menu
-000006f0: 222c 0a20 2020 2020 2020 2020 2020 2022  ",.            "
-00000700: 6576 656e 745f 6461 7461 223a 207b 7d0a  event_data": {}.
-00000710: 2020 2020 2020 2020 7d2c 0a20 2020 2020          },.     
-00000720: 2020 2022 7365 6c65 6374 5f6d 656e 755f     "select_menu_
-00000730: 6974 656d 223a 207b 0a20 2020 2020 2020  item": {.       
-00000740: 2020 2020 2022 6465 7363 7269 7074 696f       "descriptio
-00000750: 6e22 3a20 2257 6865 6e20 7468 6520 706c  n": "When the pl
-00000760: 6179 6572 2063 6c69 636b 7320 616e 6420  ayer clicks and 
-00000770: 6974 656d 2069 6e20 7468 6520 6d65 6e75  item in the menu
-00000780: 222c 0a20 2020 2020 2020 2020 2020 2022  ",.            "
-00000790: 6576 656e 745f 6461 7461 223a 207b 0a20  event_data": {. 
-000007a0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-000007b0: 6974 656d 223a 207b 0a20 2020 2020 2020  item": {.       
-000007c0: 2020 2020 2020 2020 2020 2020 2022 7479               "ty
-000007d0: 7065 223a 2022 7374 7222 2c0a 2020 2020  pe": "str",.    
-000007e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000007f0: 2264 6573 6372 6970 7469 6f6e 223a 2022  "description": "
-00000800: 5468 6520 6e61 6d65 206f 6620 7468 6520  The name of the 
-00000810: 6d65 6e75 2069 7465 6d20 7468 6520 706c  menu item the pl
-00000820: 6179 6572 2073 656c 6563 7465 6422 0a20  ayer selected". 
-00000830: 2020 2020 2020 2020 2020 2020 2020 207d                 }
-00000840: 0a20 2020 2020 2020 2020 2020 207d 0a20  .            }. 
-00000850: 2020 2020 2020 207d 2c0a 2020 2020 2020         },.      
-00000860: 2020 2268 6561 6473 6574 5f6f 6e22 3a20    "headset_on": 
-00000870: 7b0a 2020 2020 2020 2020 2020 2020 2264  {.            "d
-00000880: 6573 6372 6970 7469 6f6e 223a 2022 5768  escription": "Wh
-00000890: 656e 2074 6865 2070 6c61 7965 7220 7075  en the player pu
-000008a0: 7473 2074 6865 2068 6561 6473 6574 206f  ts the headset o
-000008b0: 6e2c 2072 6573 756d 696e 6720 7468 6520  n, resuming the 
-000008c0: 6761 6d65 222c 0a20 2020 2020 2020 2020  game",.         
-000008d0: 2020 2022 6576 656e 745f 6461 7461 223a     "event_data":
-000008e0: 207b 7d0a 2020 2020 2020 2020 7d2c 0a20   {}.        },. 
-000008f0: 2020 2020 2020 2022 6865 6164 7365 745f         "headset_
-00000900: 6f66 6622 3a20 7b0a 2020 2020 2020 2020  off": {.        
-00000910: 2020 2020 2264 6573 6372 6970 7469 6f6e      "description
-00000920: 223a 2022 5768 656e 2074 6865 2070 6c61  ": "When the pla
-00000930: 7965 7220 7265 6d6f 7665 7320 7468 6520  yer removes the 
-00000940: 6865 6164 7365 7420 6672 6f6d 2074 6865  headset from the
-00000950: 6972 2068 6561 642c 2070 6175 7369 6e67  ir head, pausing
-00000960: 2074 6865 2067 616d 6522 2c0a 2020 2020   the game",.    
-00000970: 2020 2020 2020 2020 2265 7665 6e74 5f64          "event_d
-00000980: 6174 6122 3a20 7b7d 0a20 2020 2020 2020  ata": {}.       
-00000990: 207d 2c0a 2020 2020 2020 2020 2276 6965   },.        "vie
-000009a0: 7770 6f72 745f 6461 7461 223a 207b 0a20  wport_data": {. 
-000009b0: 2020 2020 2020 2020 2020 2022 6465 7363             "desc
-000009c0: 7269 7074 696f 6e22 3a20 2241 6e20 6576  ription": "An ev
-000009d0: 656e 7420 7365 6e74 2061 7070 726f 7869  ent sent approxi
-000009e0: 6d61 7465 6c79 206f 6e63 6520 7065 7220  mately once per 
-000009f0: 7365 636f 6e64 2c20 636f 6e74 6169 6e69  second, containi
-00000a00: 6e67 2074 6865 2069 6e2d 6761 6d65 2070  ng the in-game p
-00000a10: 6f73 6974 696f 6e20 616e 6420 6f72 6965  osition and orie
-00000a20: 6e74 6174 696f 6e20 6f66 2074 6865 2070  ntation of the p
-00000a30: 6c61 7965 7220 6865 6164 7365 7420 666f  layer headset fo
-00000a40: 7220 6561 6368 2066 7261 6d65 2069 6e20  r each frame in 
-00000a50: 7468 6520 7061 7374 2073 6563 6f6e 6422  the past second"
-00000a60: 2c0a 2020 2020 2020 2020 2020 2020 2265  ,.            "e
-00000a70: 7665 6e74 5f64 6174 6122 3a20 7b0a 2020  vent_data": {.  
-00000a80: 2020 2020 2020 2020 2020 2020 2020 2267                "g
-00000a90: 617a 655f 6461 7461 5f70 6163 6b61 6765  aze_data_package
-00000aa0: 223a 207b 0a20 2020 2020 2020 2020 2020  ": {.           
-00000ab0: 2020 2020 2020 2020 2022 7479 7065 223a           "type":
-00000ac0: 2022 4c69 7374 5b44 6963 745d 222c 0a20   "List[Dict]",. 
-00000ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000ae0: 2020 2022 6465 7461 696c 7322 3a20 7b0a     "details": {.
-00000af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000b00: 2020 2020 2020 2020 2270 6f73 223a 2022          "pos": "
-00000b10: 4c69 7374 5b66 6c6f 6174 5d22 2c0a 2020  List[float]",.  
-00000b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000b30: 2020 2020 2020 2272 6f74 223a 2022 4c69        "rot": "Li
-00000b40: 7374 5b66 6c6f 6174 5d22 0a20 2020 2020  st[float]".     
-00000b50: 2020 2020 2020 2020 2020 2020 2020 207d                 }
-00000b60: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00000b70: 2020 2020 2020 2264 6573 6372 6970 7469        "descripti
-00000b80: 6f6e 223a 2022 4120 6c69 7374 206f 6620  on": "A list of 
-00000b90: 6469 6374 732c 2077 6865 7265 2065 6163  dicts, where eac
-00000ba0: 6820 6469 6374 2069 7320 6f6e 6520 6672  h dict is one fr
-00000bb0: 616d 6520 6f66 2068 6561 6473 6574 2064  ame of headset d
-00000bc0: 6174 612c 2063 6f6e 7461 696e 696e 6720  ata, containing 
-00000bd0: 6120 706f 7369 7469 6f6e 2061 6e64 2072  a position and r
-00000be0: 6f74 6174 696f 6e20 7665 6374 6f72 2c20  otation vector, 
-00000bf0: 652e 672e 207b 5c22 706f 735c 223a 5b31  e.g. {\"pos\":[1
-00000c00: 2c32 2c33 5d2c 205c 2272 6f74 5c22 3a5b  ,2,3], \"rot\":[
-00000c10: 342c 352c 362c 375d 7d2e 220a 2020 2020  4,5,6,7]}.".    
-00000c20: 2020 2020 2020 2020 2020 2020 7d0a 2020              }.  
-00000c30: 2020 2020 2020 2020 2020 7d0a 2020 2020            }.    
-00000c40: 2020 2020 7d2c 0a20 2020 2020 2020 2022      },.        "
-00000c50: 6c65 6674 5f68 616e 645f 6461 7461 223a  left_hand_data":
-00000c60: 207b 0a20 2020 2020 2020 2020 2020 2022   {.            "
-00000c70: 6465 7363 7269 7074 696f 6e22 3a20 2241  description": "A
-00000c80: 6e20 6576 656e 7420 7365 6e74 2061 7070  n event sent app
-00000c90: 726f 7869 6d61 7465 6c79 206f 6e63 6520  roximately once 
-00000ca0: 7065 7220 7365 636f 6e64 2c20 636f 6e74  per second, cont
-00000cb0: 6169 6e69 6e67 2074 6865 2069 6e2d 6761  aining the in-ga
-00000cc0: 6d65 2070 6f73 6974 696f 6e20 616e 6420  me position and 
-00000cd0: 6f72 6965 6e74 6174 696f 6e20 6f66 2074  orientation of t
-00000ce0: 6865 2070 6c61 7965 7227 7320 6c65 6674  he player's left
-00000cf0: 2068 616e 6420 666f 7220 6561 6368 2066   hand for each f
-00000d00: 7261 6d65 2069 6e20 7468 6520 7061 7374  rame in the past
-00000d10: 2073 6563 6f6e 6422 2c0a 2020 2020 2020   second",.      
-00000d20: 2020 2020 2020 2265 7665 6e74 5f64 6174        "event_dat
-00000d30: 6122 3a20 7b0a 2020 2020 2020 2020 2020  a": {.          
-00000d40: 2020 2020 2020 226c 6566 745f 6861 6e64        "left_hand
-00000d50: 5f64 6174 615f 7061 636b 6167 6522 3a20  _data_package": 
-00000d60: 7b0a 2020 2020 2020 2020 2020 2020 2020  {.              
-00000d70: 2020 2020 2020 2274 7970 6522 3a20 224c        "type": "L
-00000d80: 6973 745b 4469 6374 5d22 2c0a 2020 2020  ist[Dict]",.    
-00000d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000da0: 2264 6574 6169 6c73 223a 207b 0a20 2020  "details": {.   
-00000db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000dc0: 2020 2020 2022 706f 7322 3a20 224c 6973       "pos": "Lis
-00000dd0: 745b 666c 6f61 745d 222c 0a20 2020 2020  t[float]",.     
+00000580: 2022 6465 7363 7269 7074 696f 6e22 3a20   "description": 
+00000590: 2254 6865 2072 616e 646f 6d20 7365 6564  "The random seed
+000005a0: 2075 7365 6420 666f 7220 616c 6c20 7261   used for all ra
+000005b0: 6e64 6f6d 206e 756d 6265 722f 706f 7369  ndom number/posi
+000005c0: 7469 6f6e 2f72 6f74 6174 696f 6e20 6765  tion/rotation ge
+000005d0: 6e65 7261 7469 6f6e 2069 6e20 7468 6520  neration in the 
+000005e0: 6761 6d65 2e22 0a20 2020 2020 2020 2020  game.".         
+000005f0: 2020 2020 2020 207d 0a20 2020 2020 2020         }.       
+00000600: 2020 2020 207d 0a20 2020 2020 2020 207d       }.        }
+00000610: 2c0a 2020 2020 2020 2020 2267 616d 655f  ,.        "game_
+00000620: 7374 6172 7422 3a20 7b0a 2020 2020 2020  start": {.      
+00000630: 2020 2020 2020 2264 6573 6372 6970 7469        "descripti
+00000640: 6f6e 223a 2022 5768 656e 2061 206e 6577  on": "When a new
+00000650: 2067 616d 6520 6973 2073 7461 7274 6564   game is started
+00000660: 222c 0a20 2020 2020 2020 2020 2020 2022  ",.            "
+00000670: 6576 656e 745f 6461 7461 223a 207b 0a20  event_data": {. 
+00000680: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00000690: 6d6f 6465 223a 207b 0a20 2020 2020 2020  mode": {.       
+000006a0: 2020 2020 2020 2020 2020 2020 2022 7479               "ty
+000006b0: 7065 223a 2022 4761 6d65 4d6f 6465 222c  pe": "GameMode",
+000006c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000006d0: 2020 2020 2022 6465 7363 7269 7074 696f       "descriptio
+000006e0: 6e22 3a20 2254 6865 2067 616d 6520 6d6f  n": "The game mo
+000006f0: 6465 2074 6861 7420 7468 6520 706c 6179  de that the play
+00000700: 6572 206c 6175 6e63 6865 6422 0a20 2020  er launched".   
+00000710: 2020 2020 2020 2020 2020 2020 207d 0a20               }. 
+00000720: 2020 2020 2020 2020 2020 207d 0a20 2020             }.   
+00000730: 2020 2020 207d 2c0a 2020 2020 2020 2020       },.        
+00000740: 2264 6576 6963 655f 6964 656e 7469 6669  "device_identifi
+00000750: 6572 2220 3a20 7b0a 2020 2020 2020 2020  er" : {.        
+00000760: 2020 2020 2264 6573 6372 6970 7469 6f6e      "description
+00000770: 223a 2022 4576 656e 7420 746f 2072 6563  ": "Event to rec
+00000780: 6f72 6420 6120 6861 7264 7761 7265 2049  ord a hardware I
+00000790: 442c 2066 6f72 2063 726f 7373 2d72 6566  D, for cross-ref
+000007a0: 6572 656e 6369 6e67 2061 6761 696e 7374  erencing against
+000007b0: 2073 7572 7665 7920 6461 7461 2061 7420   survey data at 
+000007c0: 6761 6d65 706c 6179 2065 7665 6e74 732e  gameplay events.
+000007d0: 222c 0a20 2020 2020 2020 2020 2020 2022  ",.            "
+000007e0: 6576 656e 745f 6461 7461 223a 207b 0a20  event_data": {. 
+000007f0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00000800: 6861 7264 7761 7265 5f75 7569 6422 3a20  hardware_uuid": 
+00000810: 7b0a 2020 2020 2020 2020 2020 2020 2020  {.              
+00000820: 2020 2020 2020 2274 7970 6522 3a20 2273        "type": "s
+00000830: 7472 222c 0a20 2020 2020 2020 2020 2020  tr",.           
+00000840: 2020 2020 2020 2020 2022 6465 7363 7269           "descri
+00000850: 7074 696f 6e22 3a20 2254 6865 2064 6576  ption": "The dev
+00000860: 6963 6520 5555 4944 220a 2020 2020 2020  ice UUID".      
+00000870: 2020 2020 2020 2020 2020 7d0a 2020 2020            }.    
+00000880: 2020 2020 2020 2020 7d0a 2020 2020 2020          }.      
+00000890: 2020 7d2c 0a20 2020 2020 2020 2022 6f70    },.        "op
+000008a0: 656e 5f6d 656e 7522 3a20 7b0a 2020 2020  en_menu": {.    
+000008b0: 2020 2020 2020 2020 2264 6573 6372 6970          "descrip
+000008c0: 7469 6f6e 223a 2022 5768 656e 2074 6865  tion": "When the
+000008d0: 2070 6c61 7965 7220 6f70 656e 7320 7468   player opens th
+000008e0: 6520 6761 6d65 206d 656e 7522 2c0a 2020  e game menu",.  
+000008f0: 2020 2020 2020 2020 2020 2265 7665 6e74            "event
+00000900: 5f64 6174 6122 3a20 7b7d 0a20 2020 2020  _data": {}.     
+00000910: 2020 207d 2c0a 2020 2020 2020 2020 2263     },.        "c
+00000920: 6c6f 7365 5f6d 656e 7522 3a20 7b0a 2020  lose_menu": {.  
+00000930: 2020 2020 2020 2020 2020 2264 6573 6372            "descr
+00000940: 6970 7469 6f6e 223a 2022 5768 656e 2074  iption": "When t
+00000950: 6865 2070 6c61 7965 7220 636c 6f73 6573  he player closes
+00000960: 2074 6865 2067 616d 6520 6d65 6e75 222c   the game menu",
+00000970: 0a20 2020 2020 2020 2020 2020 2022 6576  .            "ev
+00000980: 656e 745f 6461 7461 223a 207b 7d0a 2020  ent_data": {}.  
+00000990: 2020 2020 2020 7d2c 0a20 2020 2020 2020        },.       
+000009a0: 2022 7365 6c65 6374 5f6d 656e 755f 6974   "select_menu_it
+000009b0: 656d 223a 207b 0a20 2020 2020 2020 2020  em": {.         
+000009c0: 2020 2022 6465 7363 7269 7074 696f 6e22     "description"
+000009d0: 3a20 2257 6865 6e20 7468 6520 706c 6179  : "When the play
+000009e0: 6572 2063 6c69 636b 7320 616e 6420 6974  er clicks and it
+000009f0: 656d 2069 6e20 7468 6520 6d65 6e75 222c  em in the menu",
+00000a00: 0a20 2020 2020 2020 2020 2020 2022 6576  .            "ev
+00000a10: 656e 745f 6461 7461 223a 207b 0a20 2020  ent_data": {.   
+00000a20: 2020 2020 2020 2020 2020 2020 2022 6974               "it
+00000a30: 656d 223a 207b 0a20 2020 2020 2020 2020  em": {.         
+00000a40: 2020 2020 2020 2020 2020 2022 7479 7065             "type
+00000a50: 223a 2022 7374 7222 2c0a 2020 2020 2020  ": "str",.      
+00000a60: 2020 2020 2020 2020 2020 2020 2020 2264                "d
+00000a70: 6573 6372 6970 7469 6f6e 223a 2022 5468  escription": "Th
+00000a80: 6520 6e61 6d65 206f 6620 7468 6520 6d65  e name of the me
+00000a90: 6e75 2069 7465 6d20 7468 6520 706c 6179  nu item the play
+00000aa0: 6572 2073 656c 6563 7465 6422 0a20 2020  er selected".   
+00000ab0: 2020 2020 2020 2020 2020 2020 207d 0a20               }. 
+00000ac0: 2020 2020 2020 2020 2020 207d 0a20 2020             }.   
+00000ad0: 2020 2020 207d 2c0a 2020 2020 2020 2020       },.        
+00000ae0: 2268 6561 6473 6574 5f6f 6e22 3a20 7b0a  "headset_on": {.
+00000af0: 2020 2020 2020 2020 2020 2020 2264 6573              "des
+00000b00: 6372 6970 7469 6f6e 223a 2022 5768 656e  cription": "When
+00000b10: 2074 6865 2070 6c61 7965 7220 7075 7473   the player puts
+00000b20: 2074 6865 2068 6561 6473 6574 206f 6e2c   the headset on,
+00000b30: 2072 6573 756d 696e 6720 7468 6520 6761   resuming the ga
+00000b40: 6d65 222c 0a20 2020 2020 2020 2020 2020  me",.           
+00000b50: 2022 6576 656e 745f 6461 7461 223a 207b   "event_data": {
+00000b60: 7d0a 2020 2020 2020 2020 7d2c 0a20 2020  }.        },.   
+00000b70: 2020 2020 2022 6865 6164 7365 745f 6f66       "headset_of
+00000b80: 6622 3a20 7b0a 2020 2020 2020 2020 2020  f": {.          
+00000b90: 2020 2264 6573 6372 6970 7469 6f6e 223a    "description":
+00000ba0: 2022 5768 656e 2074 6865 2070 6c61 7965   "When the playe
+00000bb0: 7220 7265 6d6f 7665 7320 7468 6520 6865  r removes the he
+00000bc0: 6164 7365 7420 6672 6f6d 2074 6865 6972  adset from their
+00000bd0: 2068 6561 642c 2070 6175 7369 6e67 2074   head, pausing t
+00000be0: 6865 2067 616d 6522 2c0a 2020 2020 2020  he game",.      
+00000bf0: 2020 2020 2020 2265 7665 6e74 5f64 6174        "event_dat
+00000c00: 6122 3a20 7b7d 0a20 2020 2020 2020 207d  a": {}.        }
+00000c10: 2c0a 2020 2020 2020 2020 2276 6965 7770  ,.        "viewp
+00000c20: 6f72 745f 6461 7461 223a 207b 0a20 2020  ort_data": {.   
+00000c30: 2020 2020 2020 2020 2022 6465 7363 7269           "descri
+00000c40: 7074 696f 6e22 3a20 2241 6e20 6576 656e  ption": "An even
+00000c50: 7420 7365 6e74 2061 7070 726f 7869 6d61  t sent approxima
+00000c60: 7465 6c79 206f 6e63 6520 7065 7220 7365  tely once per se
+00000c70: 636f 6e64 2c20 636f 6e74 6169 6e69 6e67  cond, containing
+00000c80: 2074 6865 2069 6e2d 6761 6d65 2070 6f73   the in-game pos
+00000c90: 6974 696f 6e20 616e 6420 6f72 6965 6e74  ition and orient
+00000ca0: 6174 696f 6e20 6f66 2074 6865 2070 6c61  ation of the pla
+00000cb0: 7965 7220 6865 6164 7365 7420 666f 7220  yer headset for 
+00000cc0: 6561 6368 2066 7261 6d65 2069 6e20 7468  each frame in th
+00000cd0: 6520 7061 7374 2073 6563 6f6e 6422 2c0a  e past second",.
+00000ce0: 2020 2020 2020 2020 2020 2020 2265 7665              "eve
+00000cf0: 6e74 5f64 6174 6122 3a20 7b0a 2020 2020  nt_data": {.    
+00000d00: 2020 2020 2020 2020 2020 2020 2267 617a              "gaz
+00000d10: 655f 6461 7461 5f70 6163 6b61 6765 223a  e_data_package":
+00000d20: 207b 0a20 2020 2020 2020 2020 2020 2020   {.             
+00000d30: 2020 2020 2020 2022 7479 7065 223a 2022         "type": "
+00000d40: 4c69 7374 5b44 6963 745d 222c 0a20 2020  List[Dict]",.   
+00000d50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000d60: 2022 6465 7461 696c 7322 3a20 7b0a 2020   "details": {.  
+00000d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000d80: 2020 2020 2020 2270 6f73 223a 2022 4c69        "pos": "Li
+00000d90: 7374 5b66 6c6f 6174 5d22 2c0a 2020 2020  st[float]",.    
+00000da0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000db0: 2020 2020 2272 6f74 223a 2022 4c69 7374      "rot": "List
+00000dc0: 5b66 6c6f 6174 5d22 0a20 2020 2020 2020  [float]".       
+00000dd0: 2020 2020 2020 2020 2020 2020 207d 2c0a               },.
 00000de0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000df0: 2020 2022 726f 7422 3a20 224c 6973 745b     "rot": "List[
-00000e00: 666c 6f61 745d 220a 2020 2020 2020 2020  float]".        
-00000e10: 2020 2020 2020 2020 2020 2020 7d2c 0a20              },. 
-00000e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000e30: 2020 2022 6465 7363 7269 7074 696f 6e22     "description"
-00000e40: 3a20 2241 206c 6973 7420 6f66 2064 6963  : "A list of dic
-00000e50: 7473 2c20 7768 6572 6520 6561 6368 2064  ts, where each d
-00000e60: 6963 7420 6973 206f 6e65 2066 7261 6d65  ict is one frame
-00000e70: 206f 6620 6c65 6674 2d68 616e 6420 6461   of left-hand da
-00000e80: 7461 2c20 636f 6e74 6169 6e69 6e67 2061  ta, containing a
-00000e90: 2070 6f73 6974 696f 6e20 616e 6420 726f   position and ro
-00000ea0: 7461 7469 6f6e 2076 6563 746f 722c 2065  tation vector, e
-00000eb0: 2e67 2e20 7b5c 2270 6f73 5c22 3a5b 312c  .g. {\"pos\":[1,
-00000ec0: 322c 335d 2c20 5c22 726f 745c 223a 5b34  2,3], \"rot\":[4
-00000ed0: 2c35 2c36 2c37 5d7d 2e22 0a20 2020 2020  ,5,6,7]}.".     
-00000ee0: 2020 2020 2020 2020 2020 207d 0a20 2020             }.   
-00000ef0: 2020 2020 2020 2020 207d 0a20 2020 2020           }.     
-00000f00: 2020 207d 2c0a 2020 2020 2020 2020 2272     },.        "r
-00000f10: 6967 6874 5f68 616e 645f 6461 7461 223a  ight_hand_data":
-00000f20: 207b 0a20 2020 2020 2020 2020 2020 2022   {.            "
-00000f30: 6465 7363 7269 7074 696f 6e22 3a20 2241  description": "A
-00000f40: 6e20 6576 656e 7420 7365 6e74 2061 7070  n event sent app
-00000f50: 726f 7869 6d61 7465 6c79 206f 6e63 6520  roximately once 
-00000f60: 7065 7220 7365 636f 6e64 2c20 636f 6e74  per second, cont
-00000f70: 6169 6e69 6e67 2074 6865 2069 6e2d 6761  aining the in-ga
-00000f80: 6d65 2070 6f73 6974 696f 6e20 616e 6420  me position and 
-00000f90: 6f72 6965 6e74 6174 696f 6e20 6f66 2074  orientation of t
-00000fa0: 6865 2070 6c61 7965 7227 7320 7269 6768  he player's righ
-00000fb0: 7420 6861 6e64 2066 6f72 2065 6163 6820  t hand for each 
-00000fc0: 6672 616d 6520 696e 2074 6865 2070 6173  frame in the pas
-00000fd0: 7420 7365 636f 6e64 222c 0a20 2020 2020  t second",.     
-00000fe0: 2020 2020 2020 2022 6576 656e 745f 6461         "event_da
-00000ff0: 7461 223a 207b 0a20 2020 2020 2020 2020  ta": {.         
-00001000: 2020 2020 2020 2022 7269 6768 745f 6861         "right_ha
-00001010: 6e64 5f64 6174 615f 7061 636b 6167 6522  nd_data_package"
-00001020: 3a20 7b0a 2020 2020 2020 2020 2020 2020  : {.            
-00001030: 2020 2020 2020 2020 2274 7970 6522 3a20          "type": 
-00001040: 224c 6973 745b 4469 6374 5d22 2c0a 2020  "List[Dict]",.  
-00001050: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001060: 2020 2264 6574 6169 6c73 223a 207b 0a20    "details": {. 
-00001070: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001080: 2020 2020 2020 2022 706f 7322 3a20 224c         "pos": "L
-00001090: 6973 745b 666c 6f61 745d 222c 0a20 2020  ist[float]",.   
+00000df0: 2020 2020 2264 6573 6372 6970 7469 6f6e      "description
+00000e00: 223a 2022 4120 6c69 7374 206f 6620 6469  ": "A list of di
+00000e10: 6374 732c 2077 6865 7265 2065 6163 6820  cts, where each 
+00000e20: 6469 6374 2069 7320 6f6e 6520 6672 616d  dict is one fram
+00000e30: 6520 6f66 2068 6561 6473 6574 2064 6174  e of headset dat
+00000e40: 612c 2063 6f6e 7461 696e 696e 6720 6120  a, containing a 
+00000e50: 706f 7369 7469 6f6e 2061 6e64 2072 6f74  position and rot
+00000e60: 6174 696f 6e20 7665 6374 6f72 2c20 652e  ation vector, e.
+00000e70: 672e 207b 5c22 706f 735c 223a 5b31 2c32  g. {\"pos\":[1,2
+00000e80: 2c33 5d2c 205c 2272 6f74 5c22 3a5b 342c  ,3], \"rot\":[4,
+00000e90: 352c 362c 375d 7d2e 220a 2020 2020 2020  5,6,7]}.".      
+00000ea0: 2020 2020 2020 2020 2020 7d0a 2020 2020            }.    
+00000eb0: 2020 2020 2020 2020 7d0a 2020 2020 2020          }.      
+00000ec0: 2020 7d2c 0a20 2020 2020 2020 2022 6c65    },.        "le
+00000ed0: 6674 5f68 616e 645f 6461 7461 223a 207b  ft_hand_data": {
+00000ee0: 0a20 2020 2020 2020 2020 2020 2022 6465  .            "de
+00000ef0: 7363 7269 7074 696f 6e22 3a20 2241 6e20  scription": "An 
+00000f00: 6576 656e 7420 7365 6e74 2061 7070 726f  event sent appro
+00000f10: 7869 6d61 7465 6c79 206f 6e63 6520 7065  ximately once pe
+00000f20: 7220 7365 636f 6e64 2c20 636f 6e74 6169  r second, contai
+00000f30: 6e69 6e67 2074 6865 2069 6e2d 6761 6d65  ning the in-game
+00000f40: 2070 6f73 6974 696f 6e20 616e 6420 6f72   position and or
+00000f50: 6965 6e74 6174 696f 6e20 6f66 2074 6865  ientation of the
+00000f60: 2070 6c61 7965 7227 7320 6c65 6674 2068   player's left h
+00000f70: 616e 6420 666f 7220 6561 6368 2066 7261  and for each fra
+00000f80: 6d65 2069 6e20 7468 6520 7061 7374 2073  me in the past s
+00000f90: 6563 6f6e 6422 2c0a 2020 2020 2020 2020  econd",.        
+00000fa0: 2020 2020 2265 7665 6e74 5f64 6174 6122      "event_data"
+00000fb0: 3a20 7b0a 2020 2020 2020 2020 2020 2020  : {.            
+00000fc0: 2020 2020 226c 6566 745f 6861 6e64 5f64      "left_hand_d
+00000fd0: 6174 615f 7061 636b 6167 6522 3a20 7b0a  ata_package": {.
+00000fe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000ff0: 2020 2020 2274 7970 6522 3a20 224c 6973      "type": "Lis
+00001000: 745b 4469 6374 5d22 2c0a 2020 2020 2020  t[Dict]",.      
+00001010: 2020 2020 2020 2020 2020 2020 2020 2264                "d
+00001020: 6574 6169 6c73 223a 207b 0a20 2020 2020  etails": {.     
+00001030: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001040: 2020 2022 706f 7322 3a20 224c 6973 745b     "pos": "List[
+00001050: 666c 6f61 745d 222c 0a20 2020 2020 2020  float]",.       
+00001060: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001070: 2022 726f 7422 3a20 224c 6973 745b 666c   "rot": "List[fl
+00001080: 6f61 745d 220a 2020 2020 2020 2020 2020  oat]".          
+00001090: 2020 2020 2020 2020 2020 7d2c 0a20 2020            },.   
 000010a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000010b0: 2020 2020 2022 726f 7422 3a20 224c 6973       "rot": "Lis
-000010c0: 745b 666c 6f61 745d 220a 2020 2020 2020  t[float]".      
-000010d0: 2020 2020 2020 2020 2020 2020 2020 7d2c                },
-000010e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000010f0: 2020 2020 2022 6465 7363 7269 7074 696f       "descriptio
-00001100: 6e22 3a20 2241 206c 6973 7420 6f66 2064  n": "A list of d
-00001110: 6963 7473 2c20 7768 6572 6520 6561 6368  icts, where each
-00001120: 2064 6963 7420 6973 206f 6e65 2066 7261   dict is one fra
-00001130: 6d65 206f 6620 7269 6768 742d 6861 6e64  me of right-hand
-00001140: 2064 6174 612c 2063 6f6e 7461 696e 696e   data, containin
-00001150: 6720 6120 706f 7369 7469 6f6e 2061 6e64  g a position and
-00001160: 2072 6f74 6174 696f 6e20 7665 6374 6f72   rotation vector
-00001170: 2c20 652e 672e 207b 5c22 706f 735c 223a  , e.g. {\"pos\":
-00001180: 5b31 2c32 2c33 5d2c 205c 2272 6f74 5c22  [1,2,3], \"rot\"
-00001190: 3a5b 342c 352c 362c 375d 7d2e 220a 2020  :[4,5,6,7]}.".  
-000011a0: 2020 2020 2020 2020 2020 2020 2020 7d0a                }.
-000011b0: 2020 2020 2020 2020 2020 2020 7d0a 2020              }.  
-000011c0: 2020 2020 2020 7d2c 0a20 2020 2020 2020        },.       
-000011d0: 2022 706c 6179 6572 5f77 6164 646c 6522   "player_waddle"
-000011e0: 3a20 7b0a 2020 2020 2020 2020 2020 2020  : {.            
-000011f0: 2264 6573 6372 6970 7469 6f6e 223a 2022  "description": "
-00001200: 5768 656e 2061 2070 6c61 7965 7220 7065  When a player pe
-00001210: 7266 6f72 6d73 2061 2077 6164 646c 6520  rforms a waddle 
-00001220: 6d6f 7665 6d65 6e74 2074 6f20 6d6f 7665  movement to move
-00001230: 2074 6865 6972 2070 656e 6775 696e 2061   their penguin a
-00001240: 7661 7461 7220 666f 7277 6172 6422 2c0a  vatar forward",.
-00001250: 2020 2020 2020 2020 2020 2020 2265 7665              "eve
-00001260: 6e74 5f64 6174 6122 3a20 7b0a 2020 2020  nt_data": {.    
-00001270: 2020 2020 2020 2020 2020 2020 226f 626a              "obj
-00001280: 6563 745f 6964 223a 207b 0a20 2020 2020  ect_id": {.     
-00001290: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-000012a0: 7479 7065 223a 2022 7374 7222 2c0a 2020  type": "str",.  
-000012b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000012c0: 2020 2264 6573 6372 6970 7469 6f6e 223a    "description":
-000012d0: 2022 5468 6520 6e61 6d65 206f 662e 2e2e   "The name of...
-000012e0: 2073 6f6d 6520 6f62 6a65 6374 220a 2020   some object".  
-000012f0: 2020 2020 2020 2020 2020 2020 2020 7d2c                },
-00001300: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001310: 2022 706f 735f 6f6c 6422 3a20 7b0a 2020   "pos_old": {.  
+000010b0: 2022 6465 7363 7269 7074 696f 6e22 3a20   "description": 
+000010c0: 2241 206c 6973 7420 6f66 2064 6963 7473  "A list of dicts
+000010d0: 2c20 7768 6572 6520 6561 6368 2064 6963  , where each dic
+000010e0: 7420 6973 206f 6e65 2066 7261 6d65 206f  t is one frame o
+000010f0: 6620 6c65 6674 2d68 616e 6420 6461 7461  f left-hand data
+00001100: 2c20 636f 6e74 6169 6e69 6e67 2061 2070  , containing a p
+00001110: 6f73 6974 696f 6e20 616e 6420 726f 7461  osition and rota
+00001120: 7469 6f6e 2076 6563 746f 722c 2065 2e67  tion vector, e.g
+00001130: 2e20 7b5c 2270 6f73 5c22 3a5b 312c 322c  . {\"pos\":[1,2,
+00001140: 335d 2c20 5c22 726f 745c 223a 5b34 2c35  3], \"rot\":[4,5
+00001150: 2c36 2c37 5d7d 2e22 0a20 2020 2020 2020  ,6,7]}.".       
+00001160: 2020 2020 2020 2020 207d 0a20 2020 2020           }.     
+00001170: 2020 2020 2020 207d 0a20 2020 2020 2020         }.       
+00001180: 207d 2c0a 2020 2020 2020 2020 2272 6967   },.        "rig
+00001190: 6874 5f68 616e 645f 6461 7461 223a 207b  ht_hand_data": {
+000011a0: 0a20 2020 2020 2020 2020 2020 2022 6465  .            "de
+000011b0: 7363 7269 7074 696f 6e22 3a20 2241 6e20  scription": "An 
+000011c0: 6576 656e 7420 7365 6e74 2061 7070 726f  event sent appro
+000011d0: 7869 6d61 7465 6c79 206f 6e63 6520 7065  ximately once pe
+000011e0: 7220 7365 636f 6e64 2c20 636f 6e74 6169  r second, contai
+000011f0: 6e69 6e67 2074 6865 2069 6e2d 6761 6d65  ning the in-game
+00001200: 2070 6f73 6974 696f 6e20 616e 6420 6f72   position and or
+00001210: 6965 6e74 6174 696f 6e20 6f66 2074 6865  ientation of the
+00001220: 2070 6c61 7965 7227 7320 7269 6768 7420   player's right 
+00001230: 6861 6e64 2066 6f72 2065 6163 6820 6672  hand for each fr
+00001240: 616d 6520 696e 2074 6865 2070 6173 7420  ame in the past 
+00001250: 7365 636f 6e64 222c 0a20 2020 2020 2020  second",.       
+00001260: 2020 2020 2022 6576 656e 745f 6461 7461       "event_data
+00001270: 223a 207b 0a20 2020 2020 2020 2020 2020  ": {.           
+00001280: 2020 2020 2022 7269 6768 745f 6861 6e64       "right_hand
+00001290: 5f64 6174 615f 7061 636b 6167 6522 3a20  _data_package": 
+000012a0: 7b0a 2020 2020 2020 2020 2020 2020 2020  {.              
+000012b0: 2020 2020 2020 2274 7970 6522 3a20 224c        "type": "L
+000012c0: 6973 745b 4469 6374 5d22 2c0a 2020 2020  ist[Dict]",.    
+000012d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000012e0: 2264 6574 6169 6c73 223a 207b 0a20 2020  "details": {.   
+000012f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001300: 2020 2020 2022 706f 7322 3a20 224c 6973       "pos": "Lis
+00001310: 745b 666c 6f61 745d 222c 0a20 2020 2020  t[float]",.     
 00001320: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001330: 2020 2274 7970 6522 3a20 224c 6973 745b    "type": "List[
-00001340: 666c 6f61 745d 222c 0a20 2020 2020 2020  float]",.       
-00001350: 2020 2020 2020 2020 2020 2020 2022 6465               "de
-00001360: 7363 7269 7074 696f 6e22 3a20 2254 6865  scription": "The
-00001370: 2070 7265 7669 6f75 7320 706f 7369 7469   previous positi
-00001380: 6f6e 206f 6620 7468 6520 706c 6179 6572  on of the player
-00001390: 2061 7661 7461 7227 7320 6665 6574 2c20   avatar's feet, 
-000013a0: 696e 205b 782c 2079 2c20 7a5d 2066 6f72  in [x, y, z] for
-000013b0: 6d2c 2069 2e65 2e20 7768 6572 6520 7468  m, i.e. where th
-000013c0: 6520 7761 6464 6c65 2073 7461 7274 6564  e waddle started
-000013d0: 2e22 0a20 2020 2020 2020 2020 2020 2020  .".             
-000013e0: 2020 207d 2c0a 2020 2020 2020 2020 2020     },.          
-000013f0: 2020 2020 2020 2270 6f73 5f6e 6577 223a        "pos_new":
-00001400: 207b 0a20 2020 2020 2020 2020 2020 2020   {.             
-00001410: 2020 2020 2020 2022 7479 7065 223a 2022         "type": "
-00001420: 4c69 7374 5b66 6c6f 6174 5d22 2c0a 2020  List[float]",.  
-00001430: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001440: 2020 2264 6573 6372 6970 7469 6f6e 223a    "description":
-00001450: 2022 5468 6520 7265 7375 6c74 696e 6720   "The resulting 
-00001460: 706f 7369 7469 6f6e 206f 6620 7468 6520  position of the 
-00001470: 706c 6179 6572 2061 7661 7461 7227 7320  player avatar's 
-00001480: 6665 6574 2c20 696e 205b 782c 2079 2c20  feet, in [x, y, 
-00001490: 7a5d 2066 6f72 6d2c 2069 2e65 2e20 7768  z] form, i.e. wh
-000014a0: 6572 6520 7468 6520 7761 6464 6c65 2065  ere the waddle e
-000014b0: 6e64 6564 2e22 0a20 2020 2020 2020 2020  nded.".         
-000014c0: 2020 2020 2020 207d 2c0a 2020 2020 2020         },.      
-000014d0: 2020 2020 2020 2020 2020 2273 6f75 7263            "sourc
-000014e0: 6522 3a20 7b0a 2020 2020 2020 2020 2020  e": {.          
-000014f0: 2020 2020 2020 2020 2020 2274 7970 6522            "type"
-00001500: 3a20 2265 6e75 6d28 4255 5454 4f4e 2c20  : "enum(BUTTON, 
-00001510: 5741 4444 4c45 2922 2c0a 2020 2020 2020  WADDLE)",.      
-00001520: 2020 2020 2020 2020 2020 2020 2020 2264                "d
-00001530: 6573 6372 6970 7469 6f6e 223a 2022 496e  escription": "In
-00001540: 6469 6361 746f 7220 666f 7220 7768 6574  dicator for whet
-00001550: 6865 7220 7468 6520 706c 6179 6572 2077  her the player w
-00001560: 6164 646c 6564 2062 7920 7072 6573 7369  addled by pressi
-00001570: 6e67 2061 2062 7574 746f 6e2c 206f 7220  ng a button, or 
-00001580: 6279 206d 616b 696e 6720 7468 6520 2777  by making the 'w
-00001590: 6164 646c 6527 2067 6573 7475 7265 2077  addle' gesture w
-000015a0: 6974 6820 7468 6569 7220 6865 6164 2e22  ith their head."
-000015b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000015c0: 207d 0a20 2020 2020 2020 2020 2020 207d   }.            }
-000015d0: 0a20 2020 2020 2020 207d 2c0a 2020 2020  .        },.    
-000015e0: 2020 2020 2267 617a 655f 6f62 6a65 6374      "gaze_object
-000015f0: 5f62 6567 696e 223a 207b 0a20 2020 2020  _begin": {.     
-00001600: 2020 2020 2020 2022 6465 7363 7269 7074         "descript
-00001610: 696f 6e22 3a20 2241 6e20 6576 656e 7420  ion": "An event 
-00001620: 7472 6967 6765 7265 6420 7768 656e 2074  triggered when t
-00001630: 6865 2070 6c61 7965 7220 6861 7320 6761  he player has ga
-00001640: 7a65 6420 6174 2061 6e20 6f62 6a65 6374  zed at an object
-00001650: 2066 6f72 2061 7420 6c65 6173 7420 302e   for at least 0.
-00001660: 3235 2073 6563 6f6e 6473 2c20 7768 6572  25 seconds, wher
-00001670: 6520 2767 617a 6564 2061 7427 206d 6561  e 'gazed at' mea
-00001680: 6e73 2074 6865 206f 626a 6563 7420 6973  ns the object is
-00001690: 2074 6865 206e 6561 7265 7374 206f 6e20   the nearest on 
-000016a0: 6120 7261 7963 6173 7420 6672 6f6d 2074  a raycast from t
-000016b0: 6865 2076 6965 7770 6f72 7420 6365 6e74  he viewport cent
-000016c0: 6572 222c 0a20 2020 2020 2020 2020 2020  er",.           
-000016d0: 2022 6576 656e 745f 6461 7461 223a 207b   "event_data": {
-000016e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000016f0: 2022 6f62 6a65 6374 5f69 6422 3a20 7b0a   "object_id": {.
-00001700: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001710: 2020 2020 2274 7970 6522 3a20 2273 7472      "type": "str
-00001720: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
-00001730: 2020 2020 2020 2022 6465 7363 7269 7074         "descript
-00001740: 696f 6e22 3a20 2254 6865 206e 616d 6520  ion": "The name 
-00001750: 6f66 2074 6865 206f 626a 6563 7420 7468  of the object th
-00001760: 6520 706c 6179 6572 2069 7320 6761 7a69  e player is gazi
-00001770: 6e67 2061 7422 0a20 2020 2020 2020 2020  ng at".         
-00001780: 2020 2020 2020 207d 0a20 2020 2020 2020         }.       
-00001790: 2020 2020 207d 0a20 2020 2020 2020 207d       }.        }
-000017a0: 2c0a 2020 2020 2020 2020 2267 617a 655f  ,.        "gaze_
-000017b0: 6f62 6a65 6374 5f65 6e64 223a 207b 0a20  object_end": {. 
-000017c0: 2020 2020 2020 2020 2020 2022 6465 7363             "desc
-000017d0: 7269 7074 696f 6e22 3a20 2241 6e20 6576  ription": "An ev
-000017e0: 656e 7420 7472 6967 6765 7265 6420 7768  ent triggered wh
-000017f0: 656e 2074 6865 2070 6c61 7965 7220 7475  en the player tu
-00001800: 726e 7320 6177 6179 2066 726f 6d20 616e  rns away from an
-00001810: 206f 626a 6563 7420 7468 6579 2764 2067   object they'd g
-00001820: 617a 6564 2061 742c 2073 6f20 7468 6520  azed at, so the 
-00001830: 6f62 6a65 6374 2069 7320 6e6f 206c 6f6e  object is no lon
-00001840: 6765 7220 6e65 6172 6573 7420 6f6e 2061  ger nearest on a
-00001850: 2072 6179 6361 7374 2066 726f 6d20 7468   raycast from th
-00001860: 6520 7669 6577 706f 7274 2063 656e 7465  e viewport cente
-00001870: 722e 204e 6f74 6520 7468 6572 6520 6d61  r. Note there ma
-00001880: 7920 6265 2061 2073 6d61 6c6c 2062 7566  y be a small buf
-00001890: 6665 7220 6172 6f75 6e64 2074 6865 206f  fer around the o
-000018a0: 626a 6563 7420 666f 7220 7468 6520 7261  bject for the ra
-000018b0: 7963 6173 742e 222c 0a20 2020 2020 2020  ycast.",.       
-000018c0: 2020 2020 2022 6576 656e 745f 6461 7461       "event_data
-000018d0: 223a 207b 0a20 2020 2020 2020 2020 2020  ": {.           
-000018e0: 2020 2020 2022 6f62 6a65 6374 5f69 6422       "object_id"
-000018f0: 3a20 7b0a 2020 2020 2020 2020 2020 2020  : {.            
-00001900: 2020 2020 2020 2020 2274 7970 6522 3a20          "type": 
-00001910: 2273 7472 222c 0a20 2020 2020 2020 2020  "str",.         
-00001920: 2020 2020 2020 2020 2020 2022 6465 7363             "desc
-00001930: 7269 7074 696f 6e22 3a20 2254 6865 206e  ription": "The n
-00001940: 616d 6520 6f66 2074 6865 206f 626a 6563  ame of the objec
-00001950: 7420 7468 6520 706c 6179 6572 2068 6164  t the player had
-00001960: 2070 7265 7669 6f75 736c 7920 6761 7a65   previously gaze
-00001970: 6420 6174 220a 2020 2020 2020 2020 2020  d at".          
-00001980: 2020 2020 2020 7d0a 2020 2020 2020 2020        }.        
-00001990: 2020 2020 7d0a 2020 2020 2020 2020 7d2c      }.        },
-000019a0: 0a20 2020 2020 2020 2022 6275 6262 6c65  .        "bubble
-000019b0: 5f70 6f70 223a 207b 0a20 2020 2020 2020  _pop": {.       
-000019c0: 2020 2020 2022 6465 7363 7269 7074 696f       "descriptio
-000019d0: 6e22 3a20 2241 6e20 6576 656e 7420 7472  n": "An event tr
-000019e0: 6967 6765 7265 6420 7768 656e 2074 6865  iggered when the
-000019f0: 2070 6c61 7965 7220 706f 7073 2061 2062   player pops a b
-00001a00: 7562 626c 6520 696e 2074 6865 2062 7562  ubble in the bub
-00001a10: 626c 652d 706f 7070 696e 6720 6d69 6e69  ble-popping mini
-00001a20: 2d67 616d 652e 2041 2062 7562 626c 6520  -game. A bubble 
-00001a30: 7368 6f75 6c64 2062 6520 706f 7070 6564  should be popped
-00001a40: 206f 6e20 6120 2762 6561 7427 206f 6620   on a 'beat' of 
-00001a50: 7468 6520 6d75 7369 632c 2062 7574 2063  the music, but c
-00001a60: 616e 2062 6520 706f 7070 6564 2075 7020  an be popped up 
-00001a70: 746f 2030 2e35 2073 6563 6f6e 6473 2062  to 0.5 seconds b
-00001a80: 6566 6f72 6520 6f72 2061 6674 6572 2074  efore or after t
-00001a90: 6865 2027 6265 6174 2e27 222c 0a20 2020  he 'beat.'",.   
-00001aa0: 2020 2020 2020 2020 2022 6576 656e 745f           "event_
-00001ab0: 6461 7461 223a 207b 0a20 2020 2020 2020  data": {.       
-00001ac0: 2020 2020 2020 2020 2022 6f62 6a65 6374           "object
-00001ad0: 5f69 6422 3a20 7b0a 2020 2020 2020 2020  _id": {.        
-00001ae0: 2020 2020 2020 2020 2020 2020 2274 7970              "typ
-00001af0: 6522 3a20 2273 7472 222c 0a20 2020 2020  e": "str",.     
-00001b00: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00001b10: 6465 7363 7269 7074 696f 6e22 3a20 2254  description": "T
-00001b20: 6865 206e 616d 6520 6f66 2074 6865 2062  he name of the b
-00001b30: 7562 626c 6520 6f62 6a65 6374 2074 6865  ubble object the
-00001b40: 2070 6c61 7965 7220 706f 7070 6564 220a   player popped".
-00001b50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001b60: 7d2c 0a20 2020 2020 2020 2020 2020 2020  },.             
-00001b70: 2020 2022 7469 6d69 6e67 5f65 7272 6f72     "timing_error
-00001b80: 223a 207b 0a20 2020 2020 2020 2020 2020  ": {.           
-00001b90: 2020 2020 2020 2020 2022 7479 7065 223a           "type":
-00001ba0: 2022 666c 6f61 7422 2c0a 2020 2020 2020   "float",.      
-00001bb0: 2020 2020 2020 2020 2020 2020 2020 2264                "d
-00001bc0: 6573 6372 6970 7469 6f6e 223a 2022 5468  escription": "Th
-00001bd0: 6520 7469 6d69 6e67 2064 6966 6665 7265  e timing differe
-00001be0: 6e63 6520 6265 7477 6565 6e20 7468 6520  nce between the 
-00001bf0: 706f 7020 6576 656e 7420 616e 6420 7468  pop event and th
-00001c00: 6520 6d75 7369 6320 2762 6561 742e 2720  e music 'beat.' 
-00001c10: 5468 6973 2076 616c 7565 2069 7320 696e  This value is in
-00001c20: 2074 6865 2072 616e 6765 205b 2d30 2e35   the range [-0.5
-00001c30: 2c20 302e 355d 2c20 7768 6572 6520 6120  , 0.5], where a 
-00001c40: 6e65 6761 7469 7665 2069 6e64 6963 6174  negative indicat
-00001c50: 6573 2074 6865 2062 7562 626c 6520 7761  es the bubble wa
-00001c60: 7320 706f 7070 6564 2062 6566 6f72 6520  s popped before 
-00001c70: 7468 6520 2762 6561 742c 2720 616e 6420  the 'beat,' and 
-00001c80: 706f 7369 7469 7665 2069 6e64 6963 6174  positive indicat
-00001c90: 6573 2070 6f70 7069 6e67 2061 6674 6572  es popping after
-00001ca0: 2074 6865 2027 6265 6174 2e27 220a 2020   the 'beat.'".  
-00001cb0: 2020 2020 2020 2020 2020 2020 2020 7d0a                }.
-00001cc0: 2020 2020 2020 2020 2020 2020 7d0a 2020              }.  
-00001cd0: 2020 2020 2020 7d2c 0a20 2020 2020 2020        },.       
-00001ce0: 2022 6561 745f 6669 7368 223a 207b 0a20   "eat_fish": {. 
-00001cf0: 2020 2020 2020 2020 2020 2022 6465 7363             "desc
-00001d00: 7269 7074 696f 6e22 3a20 2241 6e20 6576  ription": "An ev
-00001d10: 656e 7420 7472 6967 6765 7265 6420 7768  ent triggered wh
-00001d20: 656e 2074 6865 2070 6c61 7965 7220 6561  en the player ea
-00001d30: 7473 2061 2066 6973 682e 222c 0a20 2020  ts a fish.",.   
-00001d40: 2020 2020 2020 2020 2022 6576 656e 745f           "event_
-00001d50: 6461 7461 223a 207b 0a20 2020 2020 2020  data": {.       
-00001d60: 2020 2020 2020 2020 2022 6f62 6a65 6374           "object
-00001d70: 5f69 6422 3a20 7b0a 2020 2020 2020 2020  _id": {.        
-00001d80: 2020 2020 2020 2020 2020 2020 2274 7970              "typ
-00001d90: 6522 3a20 2273 7472 222c 0a20 2020 2020  e": "str",.     
-00001da0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00001db0: 6465 7363 7269 7074 696f 6e22 3a20 2254  description": "T
-00001dc0: 6865 206e 616d 6520 6f66 2074 6865 2066  he name of the f
-00001dd0: 6973 6820 6f62 6a65 6374 2074 6865 2070  ish object the p
-00001de0: 6c61 7965 7220 6174 6522 0a20 2020 2020  layer ate".     
-00001df0: 2020 2020 2020 2020 2020 207d 0a20 2020             }.   
-00001e00: 2020 2020 2020 2020 207d 0a20 2020 2020           }.     
-00001e10: 2020 207d 2c0a 2020 2020 2020 2020 2266     },.        "f
-00001e20: 6c69 7070 6572 5f62 6173 685f 6e65 7374  lipper_bash_nest
-00001e30: 223a 207b 0a20 2020 2020 2020 2020 2020  ": {.           
-00001e40: 2022 6465 7363 7269 7074 696f 6e22 3a20   "description": 
-00001e50: 2241 6e20 6576 656e 7420 7472 6967 6765  "An event trigge
-00001e60: 7265 6420 7768 656e 2074 6865 2070 6c61  red when the pla
-00001e70: 7965 7220 6d61 6b65 7320 6120 666c 6970  yer makes a flip
-00001e80: 7065 722d 6261 7368 696e 6720 6d6f 7665  per-bashing move
-00001e90: 2061 6e64 206d 616b 6573 2063 6f6e 7461   and makes conta
-00001ea0: 6374 2077 6974 6820 6120 6e65 7374 2e22  ct with a nest."
-00001eb0: 2c0a 2020 2020 2020 2020 2020 2020 2265  ,.            "e
-00001ec0: 7665 6e74 5f64 6174 6122 3a20 7b0a 2020  vent_data": {.  
-00001ed0: 2020 2020 2020 2020 2020 2020 2020 226e                "n
-00001ee0: 6573 745f 6964 223a 207b 0a20 2020 2020  est_id": {.     
-00001ef0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00001f00: 7479 7065 223a 2022 7374 7222 2c0a 2020  type": "str",.  
-00001f10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001f20: 2020 2264 6573 6372 6970 7469 6f6e 223a    "description":
-00001f30: 2022 5468 6520 6e61 6d65 206f 6620 7468   "The name of th
-00001f40: 6520 6e65 7374 206f 626a 6563 7420 7468  e nest object th
-00001f50: 6520 706c 6179 6572 2062 6173 6865 6422  e player bashed"
-00001f60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001f70: 207d 2c0a 2020 2020 2020 2020 2020 2020   },.            
-00001f80: 2020 2020 226e 6573 745f 706f 7322 3a20      "nest_pos": 
-00001f90: 7b0a 2020 2020 2020 2020 2020 2020 2020  {.              
-00001fa0: 2020 2020 2020 2274 7970 6522 3a20 224c        "type": "L
-00001fb0: 6973 745b 666c 6f61 745d 222c 0a20 2020  ist[float]",.   
-00001fc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001fd0: 2022 6465 7363 7269 7074 696f 6e22 3a20   "description": 
-00001fe0: 2254 6865 2070 6f73 6974 696f 6e20 6f66  "The position of
-00001ff0: 2074 6865 206e 6573 7420 7468 6520 706c   the nest the pl
-00002000: 6179 6572 2062 6173 6865 6422 0a20 2020  ayer bashed".   
-00002010: 2020 2020 2020 2020 2020 2020 207d 2c0a               },.
-00002020: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002030: 2268 616e 6422 3a20 7b0a 2020 2020 2020  "hand": {.      
-00002040: 2020 2020 2020 2020 2020 2020 2020 2274                "t
-00002050: 7970 6522 3a20 224c 6973 745b 666c 6f61  ype": "List[floa
-00002060: 745d 222c 0a20 2020 2020 2020 2020 2020  t]",.           
-00002070: 2020 2020 2020 2020 2022 6465 7363 7269           "descri
-00002080: 7074 696f 6e22 3a20 2254 6865 2070 6f73  ption": "The pos
-00002090: 6974 696f 6e20 6f66 2074 6865 206e 6573  ition of the nes
-000020a0: 7420 7468 6520 706c 6179 6572 2062 6173  t the player bas
-000020b0: 6865 6422 0a20 2020 2020 2020 2020 2020  hed".           
-000020c0: 2020 2020 207d 2c0a 2020 2020 2020 2020       },.        
-000020d0: 2020 2020 7d0a 2020 2020 2020 2020 7d2c      }.        },
-000020e0: 0a20 2020 2020 2020 2022 666c 6970 7065  .        "flippe
-000020f0: 725f 6261 7368 5f70 656e 6775 696e 223a  r_bash_penguin":
-00002100: 207b 0a20 2020 2020 2020 2020 2020 2022   {.            "
-00002110: 6465 7363 7269 7074 696f 6e22 3a20 2241  description": "A
-00002120: 6e20 6576 656e 7420 7472 6967 6765 7265  n event triggere
-00002130: 6420 7768 656e 2074 6865 2070 6c61 7965  d when the playe
-00002140: 7220 6d61 6b65 7320 6120 666c 6970 7065  r makes a flippe
-00002150: 722d 6261 7368 696e 6720 6d6f 7665 2061  r-bashing move a
-00002160: 6e64 206d 616b 6573 2063 6f6e 7461 6374  nd makes contact
-00002170: 2077 6974 6820 616e 6f74 6865 7220 7065   with another pe
-00002180: 6e67 7569 6e2e 222c 0a20 2020 2020 2020  nguin.",.       
-00002190: 2020 2020 2022 6576 656e 745f 6461 7461       "event_data
-000021a0: 223a 207b 0a20 2020 2020 2020 2020 2020  ": {.           
-000021b0: 2020 2020 2022 7065 6e67 7569 6e5f 6964       "penguin_id
-000021c0: 223a 207b 0a20 2020 2020 2020 2020 2020  ": {.           
-000021d0: 2020 2020 2020 2020 2022 7479 7065 223a           "type":
-000021e0: 2022 7374 7222 2c0a 2020 2020 2020 2020   "str",.        
-000021f0: 2020 2020 2020 2020 2020 2020 2264 6573              "des
-00002200: 6372 6970 7469 6f6e 223a 2022 5468 6520  cription": "The 
-00002210: 6e61 6d65 206f 6620 7468 6520 7065 6e67  name of the peng
-00002220: 7569 6e20 6f62 6a65 6374 2074 6865 2070  uin object the p
-00002230: 6c61 7965 7220 6261 7368 6564 220a 2020  layer bashed".  
-00002240: 2020 2020 2020 2020 2020 2020 2020 7d2c                },
-00002250: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002260: 2022 7065 6e67 7569 6e5f 706f 7322 3a20   "penguin_pos": 
-00002270: 7b0a 2020 2020 2020 2020 2020 2020 2020  {.              
-00002280: 2020 2020 2020 2274 7970 6522 3a20 224c        "type": "L
-00002290: 6973 745b 666c 6f61 745d 222c 0a20 2020  ist[float]",.   
-000022a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000022b0: 2022 6465 7363 7269 7074 696f 6e22 3a20   "description": 
-000022c0: 2254 6865 2070 6f73 6974 696f 6e20 6f66  "The position of
-000022d0: 2074 6865 206f 7468 6572 2070 656e 6775   the other pengu
-000022e0: 696e 2077 6865 6e20 6974 2067 6f74 2062  in when it got b
-000022f0: 6173 6865 6422 0a20 2020 2020 2020 2020  ashed".         
-00002300: 2020 2020 2020 207d 0a20 2020 2020 2020         }.       
-00002310: 2020 2020 207d 0a20 2020 2020 2020 207d       }.        }
-00002320: 2c0a 2020 2020 2020 2020 2266 6c69 7070  ,.        "flipp
-00002330: 6572 5f62 6173 685f 736b 7561 223a 207b  er_bash_skua": {
-00002340: 0a20 2020 2020 2020 2020 2020 2022 6465  .            "de
-00002350: 7363 7269 7074 696f 6e22 3a20 2241 6e20  scription": "An 
-00002360: 6576 656e 7420 7472 6967 6765 7265 6420  event triggered 
-00002370: 7768 656e 2074 6865 2070 6c61 7965 7220  when the player 
-00002380: 6d61 6b65 7320 6120 666c 6970 7065 722d  makes a flipper-
-00002390: 6261 7368 696e 6720 6d6f 7665 2074 6f20  bashing move to 
-000023a0: 7368 6f6f 2061 2073 6b75 6120 6177 6179  shoo a skua away
-000023b0: 2066 726f 6d20 7468 6569 7220 6e65 7374   from their nest
-000023c0: 2f65 6767 2e22 2c0a 2020 2020 2020 2020  /egg.",.        
-000023d0: 2020 2020 2265 7665 6e74 5f64 6174 6122      "event_data"
-000023e0: 3a20 7b0a 2020 2020 2020 2020 2020 2020  : {.            
-000023f0: 2020 2020 2273 6b75 615f 6964 223a 207b      "skua_id": {
-00002400: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002410: 2020 2020 2022 7479 7065 223a 2022 7374       "type": "st
-00002420: 7222 2c0a 2020 2020 2020 2020 2020 2020  r",.            
-00002430: 2020 2020 2020 2020 2264 6573 6372 6970          "descrip
-00002440: 7469 6f6e 223a 2022 5468 6520 6e61 6d65  tion": "The name
-00002450: 206f 6620 7468 6520 736b 7561 206f 626a   of the skua obj
-00002460: 6563 7420 7468 6520 706c 6179 6572 2062  ect the player b
-00002470: 6173 6865 6422 0a20 2020 2020 2020 2020  ashed".         
-00002480: 2020 2020 2020 207d 2c0a 2020 2020 2020         },.      
-00002490: 2020 2020 2020 2020 2020 2273 6b75 615f            "skua_
-000024a0: 706f 7322 3a20 7b0a 2020 2020 2020 2020  pos": {.        
-000024b0: 2020 2020 2020 2020 2020 2020 2274 7970              "typ
-000024c0: 6522 3a20 224c 6973 745b 666c 6f61 745d  e": "List[float]
-000024d0: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
-000024e0: 2020 2020 2020 2022 6465 7363 7269 7074         "descript
-000024f0: 696f 6e22 3a20 2254 6865 2070 6f73 6974  ion": "The posit
-00002500: 696f 6e20 6f66 2068 7420 6573 6b75 6120  ion of ht eskua 
-00002510: 7768 656e 2069 7420 676f 7420 6261 7368  when it got bash
-00002520: 6564 220a 2020 2020 2020 2020 2020 2020  ed".            
-00002530: 2020 2020 7d2c 0a20 2020 2020 2020 2020      },.         
-00002540: 2020 2020 2020 2022 7065 6e67 7569 6e5f         "penguin_
-00002550: 706f 7322 3a20 7b0a 2020 2020 2020 2020  pos": {.        
-00002560: 2020 2020 2020 2020 2020 2020 2274 7970              "typ
-00002570: 6522 3a20 2273 7472 222c 0a20 2020 2020  e": "str",.     
-00002580: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00002590: 6465 7363 7269 7074 696f 6e22 3a20 2254  description": "T
-000025a0: 6865 2070 6f73 6974 696f 6e20 6f66 2074  he position of t
-000025b0: 6865 2070 6c61 7965 7220 7768 656e 2074  he player when t
-000025c0: 6865 7920 736c 6170 7065 6420 7468 6520  hey slapped the 
-000025d0: 736b 7561 2e20 4e4f 5445 203a 2054 6869  skua. NOTE : Thi
-000025e0: 7320 7761 7320 6164 6465 6420 6475 6520  s was added due 
-000025f0: 746f 2061 206d 6973 7461 6b65 2069 6e20  to a mistake in 
-00002600: 7370 6563 6966 6963 6174 696f 6e2c 2061  specification, a
-00002610: 6e64 2069 7320 7265 6475 6e64 616e 7420  nd is redundant 
-00002620: 7769 7468 2074 6865 2070 6f73 6974 696f  with the positio
-00002630: 6e20 656c 656d 656e 7420 696e 2067 616d  n element in gam
-00002640: 655f 7374 6174 652e 220a 2020 2020 2020  e_state.".      
-00002650: 2020 2020 2020 2020 2020 7d0a 2020 2020            }.    
-00002660: 2020 2020 2020 2020 7d0a 2020 2020 2020          }.      
-00002670: 2020 7d2c 0a20 2020 2020 2020 2022 7069    },.        "pi
-00002680: 636b 7570 5f72 6f63 6b22 3a20 7b0a 2020  ckup_rock": {.  
-00002690: 2020 2020 2020 2020 2020 2264 6573 6372            "descr
-000026a0: 6970 7469 6f6e 223a 2022 416e 2065 7665  iption": "An eve
-000026b0: 6e74 2074 7269 6767 6572 6564 2077 6865  nt triggered whe
-000026c0: 6e20 7468 6520 706c 6179 6572 2070 6963  n the player pic
-000026d0: 6b73 2075 7020 6120 726f 636b 206c 7969  ks up a rock lyi
-000026e0: 6e67 206f 6e20 7468 6520 6772 6f75 6e64  ng on the ground
-000026f0: 2c20 7768 6963 6820 636f 6e74 7269 6275  , which contribu
-00002700: 7465 7320 746f 2074 6865 2062 7569 6c64  tes to the build
-00002710: 696e 6720 6f66 2074 6865 6972 206e 6573  ing of their nes
-00002720: 742e 222c 0a20 2020 2020 2020 2020 2020  t.",.           
-00002730: 2022 6576 656e 745f 6461 7461 223a 207b   "event_data": {
-00002740: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002750: 2022 746f 7461 6c5f 7069 636b 6564 5f75   "total_picked_u
-00002760: 7022 3a20 7b0a 2020 2020 2020 2020 2020  p": {.          
-00002770: 2020 2020 2020 2020 2020 2274 7970 6522            "type"
-00002780: 3a20 2269 6e74 222c 0a20 2020 2020 2020  : "int",.       
-00002790: 2020 2020 2020 2020 2020 2020 2022 6465               "de
-000027a0: 7363 7269 7074 696f 6e22 3a20 2254 6865  scription": "The
-000027b0: 2072 756e 6e69 6e67 2074 6f74 616c 206f   running total o
-000027c0: 6620 726f 636b 7320 7468 6520 706c 6179  f rocks the play
-000027d0: 6572 2068 6173 2070 6963 6b65 6420 7570  er has picked up
-000027e0: 2e22 0a20 2020 2020 2020 2020 2020 2020  .".             
-000027f0: 2020 207d 2c0a 2020 2020 2020 2020 2020     },.          
-00002800: 2020 2020 2020 2270 7822 3a20 7b0a 2020        "px": {.  
-00002810: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002820: 2020 2274 7970 6522 3a20 2266 6c6f 6174    "type": "float
-00002830: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
-00002840: 2020 2020 2020 2022 6465 7363 7269 7074         "descript
-00002850: 696f 6e22 3a20 2254 6865 2078 2d70 6f73  ion": "The x-pos
-00002860: 6974 696f 6e20 6f66 2074 6865 2070 6c61  ition of the pla
-00002870: 7965 7220 7768 656e 2074 6865 2065 7665  yer when the eve
-00002880: 6e74 2068 6170 7065 6e65 6422 0a20 2020  nt happened".   
-00002890: 2020 2020 2020 2020 2020 2020 207d 2c0a               },.
-000028a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000028b0: 2270 7922 3a20 7b0a 2020 2020 2020 2020  "py": {.        
-000028c0: 2020 2020 2020 2020 2020 2020 2274 7970              "typ
-000028d0: 6522 3a20 2266 6c6f 6174 222c 0a20 2020  e": "float",.   
-000028e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000028f0: 2022 6465 7363 7269 7074 696f 6e22 3a20   "description": 
-00002900: 2254 6865 2079 2d70 6f73 6974 696f 6e20  "The y-position 
-00002910: 6f66 2074 6865 2070 6c61 7965 7220 7768  of the player wh
-00002920: 656e 2074 6865 2065 7665 6e74 2068 6170  en the event hap
-00002930: 7065 6e65 6422 0a20 2020 2020 2020 2020  pened".         
-00002940: 2020 2020 2020 207d 2c0a 2020 2020 2020         },.      
-00002950: 2020 2020 2020 2020 2020 2270 7a22 3a20            "pz": 
-00002960: 7b0a 2020 2020 2020 2020 2020 2020 2020  {.              
-00002970: 2020 2020 2020 2274 7970 6522 3a20 2266        "type": "f
-00002980: 6c6f 6174 222c 0a20 2020 2020 2020 2020  loat",.         
-00002990: 2020 2020 2020 2020 2020 2022 6465 7363             "desc
-000029a0: 7269 7074 696f 6e22 3a20 2254 6865 207a  ription": "The z
-000029b0: 2d70 6f73 6974 696f 6e20 6f66 2074 6865  -position of the
-000029c0: 2070 6c61 7965 7220 7768 656e 2074 6865   player when the
-000029d0: 2065 7665 6e74 2068 6170 7065 6e65 6422   event happened"
-000029e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000029f0: 207d 2c0a 2020 2020 2020 2020 2020 2020   },.            
-00002a00: 2020 2020 2271 7822 3a20 7b0a 2020 2020      "qx": {.    
-00002a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002a20: 2274 7970 6522 3a20 2266 6c6f 6174 222c  "type": "float",
-00002a30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002a40: 2020 2020 2022 6465 7363 7269 7074 696f       "descriptio
-00002a50: 6e22 3a20 2254 6865 2078 2d63 6f6d 706f  n": "The x-compo
-00002a60: 6e65 6e74 206f 6620 7468 6520 7175 6174  nent of the quat
-00002a70: 6572 6e69 6f6e 2066 6f72 2074 6865 2070  ernion for the p
-00002a80: 6c61 7965 7227 7320 6f72 6965 6e74 6174  layer's orientat
-00002a90: 696f 6e20 7768 656e 2074 6865 2065 7665  ion when the eve
-00002aa0: 6e74 2068 6170 7065 6e65 6422 0a20 2020  nt happened".   
-00002ab0: 2020 2020 2020 2020 2020 2020 207d 2c0a               },.
-00002ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002ad0: 2271 7922 3a20 7b0a 2020 2020 2020 2020  "qy": {.        
-00002ae0: 2020 2020 2020 2020 2020 2020 2274 7970              "typ
-00002af0: 6522 3a20 2266 6c6f 6174 222c 0a20 2020  e": "float",.   
-00002b00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002b10: 2022 6465 7363 7269 7074 696f 6e22 3a20   "description": 
-00002b20: 2254 6865 2079 2d63 6f6d 706f 6e65 6e74  "The y-component
-00002b30: 206f 6620 7468 6520 7175 6174 6572 6e69   of the quaterni
-00002b40: 6f6e 2066 6f72 2074 6865 2070 6c61 7965  on for the playe
-00002b50: 7227 7320 6f72 6965 6e74 6174 696f 6e20  r's orientation 
-00002b60: 7768 656e 2074 6865 2065 7665 6e74 2068  when the event h
-00002b70: 6170 7065 6e65 6422 0a20 2020 2020 2020  appened".       
-00002b80: 2020 2020 2020 2020 207d 2c0a 2020 2020           },.    
-00002b90: 2020 2020 2020 2020 2020 2020 2271 7a22              "qz"
-00002ba0: 3a20 7b0a 2020 2020 2020 2020 2020 2020  : {.            
-00002bb0: 2020 2020 2020 2020 2274 7970 6522 3a20          "type": 
-00002bc0: 2266 6c6f 6174 222c 0a20 2020 2020 2020  "float",.       
-00002bd0: 2020 2020 2020 2020 2020 2020 2022 6465               "de
-00002be0: 7363 7269 7074 696f 6e22 3a20 2254 6865  scription": "The
-00002bf0: 207a 2d63 6f6d 706f 6e65 6e74 206f 6620   z-component of 
-00002c00: 7468 6520 7175 6174 6572 6e69 6f6e 2066  the quaternion f
-00002c10: 6f72 2074 6865 2070 6c61 7965 7227 7320  or the player's 
-00002c20: 6f72 6965 6e74 6174 696f 6e20 7768 656e  orientation when
-00002c30: 2074 6865 2065 7665 6e74 2068 6170 7065   the event happe
-00002c40: 6e65 6422 0a20 2020 2020 2020 2020 2020  ned".           
-00002c50: 2020 2020 207d 2c0a 2020 2020 2020 2020       },.        
-00002c60: 2020 2020 2020 2020 2271 7722 3a20 7b0a          "qw": {.
-00002c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002c80: 2020 2020 2274 7970 6522 3a20 2266 6c6f      "type": "flo
-00002c90: 6174 222c 0a20 2020 2020 2020 2020 2020  at",.           
-00002ca0: 2020 2020 2020 2020 2022 6465 7363 7269           "descri
-00002cb0: 7074 696f 6e22 3a20 2254 6865 2077 2d63  ption": "The w-c
-00002cc0: 6f6d 706f 6e65 6e74 206f 6620 7468 6520  omponent of the 
-00002cd0: 7175 6174 6572 6e69 6f6e 2066 6f72 2074  quaternion for t
-00002ce0: 6865 2070 6c61 7965 7227 7320 6f72 6965  he player's orie
-00002cf0: 6e74 6174 696f 6e20 7768 656e 2074 6865  ntation when the
-00002d00: 2065 7665 6e74 2068 6170 7065 6e65 6422   event happened"
-00002d10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002d20: 207d 0a20 2020 2020 2020 2020 2020 207d   }.            }
-00002d30: 0a20 2020 2020 2020 207d 2c0a 2020 2020  .        },.    
-00002d40: 2020 2020 2270 7573 685f 736e 6f77 6261      "push_snowba
-00002d50: 6c6c 223a 207b 0a20 2020 2020 2020 2020  ll": {.         
-00002d60: 2020 2022 6465 7363 7269 7074 696f 6e22     "description"
-00002d70: 3a20 2241 6e20 6576 656e 7420 7472 6967  : "An event trig
-00002d80: 6765 7265 6420 7768 656e 2074 6865 2070  gered when the p
-00002d90: 6c61 7965 7220 7075 7368 6573 2061 2073  layer pushes a s
-00002da0: 6e6f 7762 616c 6c20 646f 776e 2074 6865  nowball down the
-00002db0: 2068 696c 6c2e 222c 0a20 2020 2020 2020   hill.",.       
-00002dc0: 2020 2020 2022 6576 656e 745f 6461 7461       "event_data
-00002dd0: 223a 207b 0a20 2020 2020 2020 2020 2020  ": {.           
-00002de0: 2020 2020 2022 6f62 6a65 6374 5f69 6422       "object_id"
-00002df0: 3a20 7b0a 2020 2020 2020 2020 2020 2020  : {.            
-00002e00: 2020 2020 2020 2020 2274 7970 6522 3a20          "type": 
-00002e10: 2273 7472 222c 0a20 2020 2020 2020 2020  "str",.         
-00002e20: 2020 2020 2020 2020 2020 2022 6465 7363             "desc
-00002e30: 7269 7074 696f 6e22 3a20 2254 6865 206e  ription": "The n
-00002e40: 616d 6520 6f66 2074 6865 2073 6e6f 7762  ame of the snowb
-00002e50: 616c 6c20 6f62 6a65 6374 2074 6865 2070  all object the p
-00002e60: 6c61 7965 7220 7075 7368 6564 220a 2020  layer pushed".  
-00002e70: 2020 2020 2020 2020 2020 2020 2020 7d2c                },
-00002e80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002e90: 2022 7078 223a 207b 0a20 2020 2020 2020   "px": {.       
-00002ea0: 2020 2020 2020 2020 2020 2020 2022 7479               "ty
-00002eb0: 7065 223a 2022 666c 6f61 7422 2c0a 2020  pe": "float",.  
-00002ec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002ed0: 2020 2264 6573 6372 6970 7469 6f6e 223a    "description":
-00002ee0: 2022 5468 6520 782d 706f 7369 7469 6f6e   "The x-position
-00002ef0: 206f 6620 7468 6520 706c 6179 6572 2077   of the player w
-00002f00: 6865 6e20 7468 6520 6576 656e 7420 6861  hen the event ha
-00002f10: 7070 656e 6564 220a 2020 2020 2020 2020  ppened".        
-00002f20: 2020 2020 2020 2020 7d2c 0a20 2020 2020          },.     
-00002f30: 2020 2020 2020 2020 2020 2022 7079 223a             "py":
-00002f40: 207b 0a20 2020 2020 2020 2020 2020 2020   {.             
-00002f50: 2020 2020 2020 2022 7479 7065 223a 2022         "type": "
-00002f60: 666c 6f61 7422 2c0a 2020 2020 2020 2020  float",.        
-00002f70: 2020 2020 2020 2020 2020 2020 2264 6573              "des
-00002f80: 6372 6970 7469 6f6e 223a 2022 5468 6520  cription": "The 
-00002f90: 792d 706f 7369 7469 6f6e 206f 6620 7468  y-position of th
-00002fa0: 6520 706c 6179 6572 2077 6865 6e20 7468  e player when th
-00002fb0: 6520 6576 656e 7420 6861 7070 656e 6564  e event happened
-00002fc0: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
-00002fd0: 2020 7d2c 0a20 2020 2020 2020 2020 2020    },.           
-00002fe0: 2020 2020 2022 707a 223a 207b 0a20 2020       "pz": {.   
-00002ff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003000: 2022 7479 7065 223a 2022 666c 6f61 7422   "type": "float"
-00003010: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00003020: 2020 2020 2020 2264 6573 6372 6970 7469        "descripti
-00003030: 6f6e 223a 2022 5468 6520 7a2d 706f 7369  on": "The z-posi
-00003040: 7469 6f6e 206f 6620 7468 6520 706c 6179  tion of the play
-00003050: 6572 2077 6865 6e20 7468 6520 6576 656e  er when the even
-00003060: 7420 6861 7070 656e 6564 220a 2020 2020  t happened".    
-00003070: 2020 2020 2020 2020 2020 2020 7d2c 0a20              },. 
-00003080: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00003090: 7178 223a 207b 0a20 2020 2020 2020 2020  qx": {.         
-000030a0: 2020 2020 2020 2020 2020 2022 7479 7065             "type
-000030b0: 223a 2022 666c 6f61 7422 2c0a 2020 2020  ": "float",.    
-000030c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000030d0: 2264 6573 6372 6970 7469 6f6e 223a 2022  "description": "
-000030e0: 5468 6520 782d 636f 6d70 6f6e 656e 7420  The x-component 
-000030f0: 6f66 2074 6865 2071 7561 7465 726e 696f  of the quaternio
-00003100: 6e20 666f 7220 7468 6520 706c 6179 6572  n for the player
-00003110: 2773 206f 7269 656e 7461 7469 6f6e 2077  's orientation w
-00003120: 6865 6e20 7468 6520 6576 656e 7420 6861  hen the event ha
-00003130: 7070 656e 6564 220a 2020 2020 2020 2020  ppened".        
-00003140: 2020 2020 2020 2020 7d2c 0a20 2020 2020          },.     
-00003150: 2020 2020 2020 2020 2020 2022 7179 223a             "qy":
-00003160: 207b 0a20 2020 2020 2020 2020 2020 2020   {.             
-00003170: 2020 2020 2020 2022 7479 7065 223a 2022         "type": "
-00003180: 666c 6f61 7422 2c0a 2020 2020 2020 2020  float",.        
-00003190: 2020 2020 2020 2020 2020 2020 2264 6573              "des
-000031a0: 6372 6970 7469 6f6e 223a 2022 5468 6520  cription": "The 
-000031b0: 792d 636f 6d70 6f6e 656e 7420 6f66 2074  y-component of t
-000031c0: 6865 2071 7561 7465 726e 696f 6e20 666f  he quaternion fo
-000031d0: 7220 7468 6520 706c 6179 6572 2773 206f  r the player's o
-000031e0: 7269 656e 7461 7469 6f6e 2077 6865 6e20  rientation when 
-000031f0: 7468 6520 6576 656e 7420 6861 7070 656e  the event happen
-00003200: 6564 220a 2020 2020 2020 2020 2020 2020  ed".            
-00003210: 2020 2020 7d2c 0a20 2020 2020 2020 2020      },.         
-00003220: 2020 2020 2020 2022 717a 223a 207b 0a20         "qz": {. 
-00003230: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003240: 2020 2022 7479 7065 223a 2022 666c 6f61     "type": "floa
-00003250: 7422 2c0a 2020 2020 2020 2020 2020 2020  t",.            
-00003260: 2020 2020 2020 2020 2264 6573 6372 6970          "descrip
-00003270: 7469 6f6e 223a 2022 5468 6520 7a2d 636f  tion": "The z-co
-00003280: 6d70 6f6e 656e 7420 6f66 2074 6865 2071  mponent of the q
-00003290: 7561 7465 726e 696f 6e20 666f 7220 7468  uaternion for th
-000032a0: 6520 706c 6179 6572 2773 206f 7269 656e  e player's orien
-000032b0: 7461 7469 6f6e 2077 6865 6e20 7468 6520  tation when the 
-000032c0: 6576 656e 7420 6861 7070 656e 6564 220a  event happened".
-000032d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000032e0: 7d2c 0a20 2020 2020 2020 2020 2020 2020  },.             
-000032f0: 2020 2022 7177 223a 207b 0a20 2020 2020     "qw": {.     
-00003300: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00003310: 7479 7065 223a 2022 666c 6f61 7422 2c0a  type": "float",.
-00003320: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003330: 2020 2020 2264 6573 6372 6970 7469 6f6e      "description
-00003340: 223a 2022 5468 6520 772d 636f 6d70 6f6e  ": "The w-compon
-00003350: 656e 7420 6f66 2074 6865 2071 7561 7465  ent of the quate
-00003360: 726e 696f 6e20 666f 7220 7468 6520 706c  rnion for the pl
-00003370: 6179 6572 2773 206f 7269 656e 7461 7469  ayer's orientati
-00003380: 6f6e 2077 6865 6e20 7468 6520 6576 656e  on when the even
-00003390: 7420 6861 7070 656e 6564 220a 2020 2020  t happened".    
-000033a0: 2020 2020 2020 2020 2020 2020 7d0a 2020              }.  
-000033b0: 2020 2020 2020 2020 2020 7d0a 2020 2020            }.    
-000033c0: 2020 2020 7d2c 0a20 2020 2020 2020 2022      },.        "
-000033d0: 7269 6e67 5f63 6869 6d65 223a 207b 0a20  ring_chime": {. 
-000033e0: 2020 2020 2020 2020 2020 2022 6465 7363             "desc
-000033f0: 7269 7074 696f 6e22 3a20 2241 6e20 6576  ription": "An ev
-00003400: 656e 7420 7768 656e 2074 6865 2070 6c61  ent when the pla
-00003410: 7965 7220 7269 6e67 7320 6f6e 6520 6f66  yer rings one of
-00003420: 2074 6865 2063 6869 6d65 7320 696e 2074   the chimes in t
-00003430: 6865 2063 6869 6d65 206d 696e 692d 6761  he chime mini-ga
-00003440: 6d65 2e22 2c0a 2020 2020 2020 2020 2020  me.",.          
-00003450: 2020 2265 7665 6e74 5f64 6174 6122 3a20    "event_data": 
-00003460: 7b0a 2020 2020 2020 2020 2020 2020 2020  {.              
-00003470: 2020 226e 6f74 655f 706c 6179 6564 223a    "note_played":
-00003480: 207b 0a20 2020 2020 2020 2020 2020 2020   {.             
-00003490: 2020 2020 2020 2022 7479 7065 223a 2022         "type": "
-000034a0: 7374 7222 2c0a 2020 2020 2020 2020 2020  str",.          
-000034b0: 2020 2020 2020 2020 2020 2264 6573 6372            "descr
-000034c0: 6970 7469 6f6e 223a 2022 5468 6520 6e61  iption": "The na
-000034d0: 6d65 206f 6620 7468 6520 6368 696d 6520  me of the chime 
-000034e0: 7468 6520 706c 6179 6572 2072 616e 6722  the player rang"
-000034f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00003500: 207d 0a20 2020 2020 2020 2020 2020 207d   }.            }
-00003510: 0a20 2020 2020 2020 207d 2c0a 2020 2020  .        },.    
-00003520: 2020 2020 2262 7562 626c 655f 6170 7065      "bubble_appe
-00003530: 6172 6564 223a 207b 0a20 2020 2020 2020  ared": {.       
-00003540: 2020 2020 2022 6465 7363 7269 7074 696f       "descriptio
-00003550: 6e22 3a20 2245 7665 6e74 2077 6865 6e20  n": "Event when 
-00003560: 6120 6e65 7720 6275 6262 6c65 2061 7070  a new bubble app
-00003570: 6561 7273 2069 6e20 7468 6520 6d61 7469  ears in the mati
-00003580: 6e67 2064 616e 6365 206d 696e 6967 616d  ng dance minigam
-00003590: 652e 222c 0a20 2020 2020 2020 2020 2020  e.",.           
-000035a0: 2022 6576 656e 745f 6461 7461 223a 207b   "event_data": {
-000035b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000035c0: 2022 6f62 6a65 6374 5f69 6422 3a20 7b0a   "object_id": {.
-000035d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000035e0: 2020 2020 2274 7970 6522 3a20 2273 7472      "type": "str
-000035f0: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
-00003600: 2020 2020 2020 2022 6465 7363 7269 7074         "descript
-00003610: 696f 6e22 3a20 2254 6865 206e 616d 6520  ion": "The name 
-00003620: 6f66 2074 6865 2062 7562 626c 6520 6f62  of the bubble ob
-00003630: 6a65 6374 2074 6861 7420 6170 7065 6172  ject that appear
-00003640: 6564 220a 2020 2020 2020 2020 2020 2020  ed".            
-00003650: 2020 2020 7d2c 0a20 2020 2020 2020 2020      },.         
-00003660: 2020 2020 2020 2022 706f 7358 223a 207b         "posX": {
-00003670: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00003680: 2020 2020 2022 7479 7065 223a 2022 666c       "type": "fl
-00003690: 6f61 7422 2c0a 2020 2020 2020 2020 2020  oat",.          
-000036a0: 2020 2020 2020 2020 2020 2264 6573 6372            "descr
-000036b0: 6970 7469 6f6e 223a 2022 5468 6520 782d  iption": "The x-
-000036c0: 706f 7369 7469 6f6e 206f 6620 7468 6520  position of the 
-000036d0: 6275 6262 6c65 2074 6861 7420 6170 7065  bubble that appe
-000036e0: 6172 6564 220a 2020 2020 2020 2020 2020  ared".          
-000036f0: 2020 2020 2020 7d2c 0a20 2020 2020 2020        },.       
-00003700: 2020 2020 2020 2020 2022 706f 7359 223a           "posY":
-00003710: 207b 0a20 2020 2020 2020 2020 2020 2020   {.             
-00003720: 2020 2020 2020 2022 7479 7065 223a 2022         "type": "
-00003730: 666c 6f61 7422 2c0a 2020 2020 2020 2020  float",.        
-00003740: 2020 2020 2020 2020 2020 2020 2264 6573              "des
-00003750: 6372 6970 7469 6f6e 223a 2022 5468 6520  cription": "The 
-00003760: 792d 706f 7369 7469 6f6e 206f 6620 7468  y-position of th
-00003770: 6520 6275 6262 6c65 2074 6861 7420 6170  e bubble that ap
-00003780: 7065 6172 6564 220a 2020 2020 2020 2020  peared".        
-00003790: 2020 2020 2020 2020 7d2c 0a20 2020 2020          },.     
-000037a0: 2020 2020 2020 2020 2020 2022 706f 735a             "posZ
-000037b0: 223a 207b 0a20 2020 2020 2020 2020 2020  ": {.           
-000037c0: 2020 2020 2020 2020 2022 7479 7065 223a           "type":
-000037d0: 2022 666c 6f61 7422 2c0a 2020 2020 2020   "float",.      
-000037e0: 2020 2020 2020 2020 2020 2020 2020 2264                "d
-000037f0: 6573 6372 6970 7469 6f6e 223a 2022 5468  escription": "Th
-00003800: 6520 7a2d 706f 7369 7469 6f6e 206f 6620  e z-position of 
-00003810: 7468 6520 6275 6262 6c65 2074 6861 7420  the bubble that 
-00003820: 6170 7065 6172 6564 220a 2020 2020 2020  appeared".      
-00003830: 2020 2020 2020 2020 2020 7d0a 2020 2020            }.    
-00003840: 2020 2020 2020 2020 7d0a 2020 2020 2020          }.      
-00003850: 2020 7d2c 0a20 2020 2020 2020 2022 6275    },.        "bu
-00003860: 6262 6c65 5f65 7870 6972 6564 223a 207b  bble_expired": {
-00003870: 0a20 2020 2020 2020 2020 2020 2022 6465  .            "de
-00003880: 7363 7269 7074 696f 6e22 3a20 2245 7665  scription": "Eve
-00003890: 6e74 2077 6865 6e20 6120 6275 6262 6c65  nt when a bubble
-000038a0: 2773 2070 6f70 2d61 626c 6520 7469 6d65  's pop-able time
-000038b0: 2065 6e64 7320 616e 6420 7468 6520 6275   ends and the bu
-000038c0: 6262 6c65 2064 6973 6170 7065 6172 732e  bble disappears.
-000038d0: 222c 0a20 2020 2020 2020 2020 2020 2022  ",.            "
-000038e0: 6576 656e 745f 6461 7461 223a 207b 0a20  event_data": {. 
-000038f0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00003900: 6f62 6a65 6374 5f69 6422 3a20 7b0a 2020  object_id": {.  
-00003910: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003920: 2020 2274 7970 6522 3a20 2273 7472 222c    "type": "str",
-00003930: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00003940: 2020 2020 2022 6465 7363 7269 7074 696f       "descriptio
-00003950: 6e22 3a20 2254 6865 206e 616d 6520 6f66  n": "The name of
-00003960: 2074 6865 2062 7562 626c 6520 6f62 6a65   the bubble obje
-00003970: 6374 2074 6861 7420 6469 7361 7070 6561  ct that disappea
-00003980: 7265 6422 0a20 2020 2020 2020 2020 2020  red".           
-00003990: 2020 2020 207d 0a20 2020 2020 2020 2020       }.         
-000039a0: 2020 207d 0a20 2020 2020 2020 207d 2c0a     }.        },.
-000039b0: 2020 2020 2020 2020 2265 6767 5f68 6174          "egg_hat
-000039c0: 6368 5f69 6e64 6963 6174 6f72 5f75 7064  ch_indicator_upd
-000039d0: 6174 6564 223a 207b 0a20 2020 2020 2020  ated": {.       
-000039e0: 2020 2020 2022 6465 7363 7269 7074 696f       "descriptio
-000039f0: 6e22 3a20 224e 4f54 2059 4554 2044 4f43  n": "NOT YET DOC
-00003a00: 554d 454e 5445 4422 2c0a 2020 2020 2020  UMENTED",.      
-00003a10: 2020 2020 2020 2265 7665 6e74 5f64 6174        "event_dat
-00003a20: 6122 3a20 7b0a 2020 2020 2020 2020 2020  a": {.          
-00003a30: 2020 2020 2020 2274 696d 655f 7265 6d61        "time_rema
-00003a40: 696e 696e 6722 3a20 7b0a 2020 2020 2020  ining": {.      
-00003a50: 2020 2020 2020 2020 2020 2020 2020 2274                "t
-00003a60: 7970 6522 3a20 2269 6e74 222c 0a20 2020  ype": "int",.   
-00003a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003a80: 2022 6465 7363 7269 7074 696f 6e22 3a20   "description": 
-00003a90: 2254 6865 2074 696d 6520 6c65 6674 2075  "The time left u
-00003aa0: 6e74 696c 2074 6865 2065 6767 2077 696c  ntil the egg wil
-00003ab0: 6c20 6861 7463 6822 0a20 2020 2020 2020  l hatch".       
-00003ac0: 2020 2020 2020 2020 207d 0a20 2020 2020           }.     
-00003ad0: 2020 2020 2020 207d 0a20 2020 2020 2020         }.       
-00003ae0: 207d 2c0a 2020 2020 2020 2020 2265 6767   },.        "egg
-00003af0: 5f68 6174 6368 6564 223a 207b 0a20 2020  _hatched": {.   
-00003b00: 2020 2020 2020 2020 2022 6465 7363 7269           "descri
-00003b10: 7074 696f 6e22 3a20 2245 7665 6e74 2077  ption": "Event w
-00003b20: 6865 6e20 7468 6520 6567 6720 6861 7463  hen the egg hatc
-00003b30: 6865 7322 2c0a 2020 2020 2020 2020 2020  hes",.          
-00003b40: 2020 2265 7665 6e74 5f64 6174 6122 3a20    "event_data": 
-00003b50: 7b7d 0a20 2020 2020 2020 207d 2c0a 2020  {}.        },.  
-00003b60: 2020 2020 2020 2265 6767 5f6c 6f73 7422        "egg_lost"
-00003b70: 3a20 7b0a 2020 2020 2020 2020 2020 2020  : {.            
-00003b80: 2264 6573 6372 6970 7469 6f6e 223a 2022  "description": "
-00003b90: 4576 656e 7420 7768 656e 2074 6865 2070  Event when the p
-00003ba0: 6c61 7965 7227 7320 6567 6720 6973 2073  layer's egg is s
-00003bb0: 746f 6c65 6e20 6279 2061 2073 6b75 612e  tolen by a skua.
-00003bc0: 222c 0a20 2020 2020 2020 2020 2020 2022  ",.            "
-00003bd0: 6576 656e 745f 6461 7461 223a 207b 0a20  event_data": {. 
-00003be0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00003bf0: 6f62 6a65 6374 5f69 6422 3a20 7b0a 2020  object_id": {.  
-00003c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003c10: 2020 2274 7970 6522 3a20 2273 7472 222c    "type": "str",
-00003c20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00003c30: 2020 2020 2022 6465 7363 7269 7074 696f       "descriptio
-00003c40: 6e22 3a20 2254 6865 206e 616d 6520 6f66  n": "The name of
-00003c50: 2074 6865 2073 6b75 6120 7468 6174 2073   the skua that s
-00003c60: 746f 6c65 2074 6865 2065 6767 220a 2020  tole the egg".  
-00003c70: 2020 2020 2020 2020 2020 2020 2020 7d0a                }.
-00003c80: 2020 2020 2020 2020 2020 2020 7d0a 2020              }.  
-00003c90: 2020 2020 2020 7d2c 0a20 2020 2020 2020        },.       
-00003ca0: 2022 6567 675f 7265 636f 7665 7265 6422   "egg_recovered"
-00003cb0: 3a20 7b0a 2020 2020 2020 2020 2020 2020  : {.            
-00003cc0: 2264 6573 6372 6970 7469 6f6e 223a 2022  "description": "
-00003cd0: 4576 656e 7420 7768 656e 2074 6865 2070  Event when the p
-00003ce0: 6c61 7965 7220 7265 636f 7665 7273 2074  layer recovers t
-00003cf0: 6865 2065 6767 2066 726f 6d20 7468 6520  he egg from the 
-00003d00: 736b 7561 732e 222c 0a20 2020 2020 2020  skuas.",.       
-00003d10: 2020 2020 2022 6576 656e 745f 6461 7461       "event_data
-00003d20: 223a 207b 7d0a 2020 2020 2020 2020 7d2c  ": {}.        },
-00003d30: 0a20 2020 2020 2020 2022 6d61 7469 6e67  .        "mating
-00003d40: 5f64 616e 6365 5f69 6e64 6963 6174 6f72  _dance_indicator
-00003d50: 5f75 7064 6174 6564 223a 207b 0a20 2020  _updated": {.   
-00003d60: 2020 2020 2020 2020 2022 6465 7363 7269           "descri
-00003d70: 7074 696f 6e22 3a20 2245 7665 6e74 2077  ption": "Event w
-00003d80: 6865 6e20 6120 6275 6262 6c65 2069 7320  hen a bubble is 
-00003d90: 706f 7070 6564 2061 6e64 2074 6865 2069  popped and the i
-00003da0: 6e64 6963 6174 6f72 2066 6f72 2070 726f  ndicator for pro
-00003db0: 6772 6573 7320 746f 2063 6f6d 706c 6574  gress to complet
-00003dc0: 696f 6e20 6f66 2074 6865 206d 6174 696e  ion of the matin
-00003dd0: 6720 6461 6e63 6520 7570 6461 7465 732e  g dance updates.
-00003de0: 222c 0a20 2020 2020 2020 2020 2020 2022  ",.            "
-00003df0: 6576 656e 745f 6461 7461 223a 207b 0a20  event_data": {. 
-00003e00: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00003e10: 7065 7263 656e 745f 6675 6c6c 223a 207b  percent_full": {
-00003e20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00003e30: 2020 2020 2022 7479 7065 223a 2022 696e       "type": "in
-00003e40: 7422 2c0a 2020 2020 2020 2020 2020 2020  t",.            
-00003e50: 2020 2020 2020 2020 2264 6573 6372 6970          "descrip
-00003e60: 7469 6f6e 223a 2022 5468 6520 6e65 7720  tion": "The new 
-00003e70: 7065 7263 656e 7420 746f 2077 6869 6368  percent to which
-00003e80: 2074 6865 2064 616e 6365 2063 6f6d 706c   the dance compl
-00003e90: 6574 696f 6e20 696e 6469 6361 746f 7220  etion indicator 
-00003ea0: 6973 2066 696c 6c65 6422 0a20 2020 2020  is filled".     
-00003eb0: 2020 2020 2020 2020 2020 207d 0a20 2020             }.   
-00003ec0: 2020 2020 2020 2020 207d 0a20 2020 2020           }.     
-00003ed0: 2020 207d 2c0a 2020 2020 2020 2020 226e     },.        "n
-00003ee0: 6573 745f 636f 6d70 6c65 7465 223a 207b  est_complete": {
-00003ef0: 0a20 2020 2020 2020 2020 2020 2022 6465  .            "de
-00003f00: 7363 7269 7074 696f 6e22 3a20 2245 7665  scription": "Eve
-00003f10: 6e74 2077 6865 6e20 7468 6520 706c 6179  nt when the play
-00003f20: 6572 2063 6f6d 706c 6574 6573 2074 6865  er completes the
-00003f30: 2062 7569 6c64 696e 6720 6f66 2074 6865   building of the
-00003f40: 6972 206e 6573 742e 222c 0a20 2020 2020  ir nest.",.     
-00003f50: 2020 2020 2020 2022 6576 656e 745f 6461         "event_da
-00003f60: 7461 223a 207b 7d0a 2020 2020 2020 2020  ta": {}.        
-00003f70: 7d2c 0a20 2020 2020 2020 2022 7065 6e67  },.        "peng
-00003f80: 7569 6e5f 7069 6e5f 6665 6c6c 223a 207b  uin_pin_fell": {
-00003f90: 0a20 2020 2020 2020 2020 2020 2022 6465  .            "de
-00003fa0: 7363 7269 7074 696f 6e22 3a20 2257 6865  scription": "Whe
-00003fb0: 6e20 6f6e 6520 6f66 2074 6865 2070 696e  n one of the pin
-00003fc0: 7320 6665 6c6c 2069 6e20 7468 6520 626f  s fell in the bo
-00003fd0: 776c 696e 6720 6172 6561 2e22 2c0a 2020  wling area.",.  
-00003fe0: 2020 2020 2020 2020 2020 2265 7665 6e74            "event
-00003ff0: 5f64 6174 6122 3a20 7b7d 0a20 2020 2020  _data": {}.     
-00004000: 2020 207d 2c0a 2020 2020 2020 2020 2273     },.        "s
-00004010: 6b75 615f 7370 6177 6e22 3a20 7b0a 2020  kua_spawn": {.  
-00004020: 2020 2020 2020 2020 2020 2264 6573 6372            "descr
-00004030: 6970 7469 6f6e 223a 2022 4576 656e 7420  iption": "Event 
-00004040: 7768 656e 2061 206e 6577 2073 6b75 6120  when a new skua 
-00004050: 6973 2061 6464 6564 2069 6e20 7468 6520  is added in the 
-00004060: 6e65 7374 2f65 6767 2064 6566 656e 7365  nest/egg defense
-00004070: 206d 696e 692d 6761 6d65 2e22 2c0a 2020   mini-game.",.  
-00004080: 2020 2020 2020 2020 2020 2265 7665 6e74            "event
-00004090: 5f64 6174 6122 3a20 7b0a 2020 2020 2020  _data": {.      
-000040a0: 2020 2020 2020 2020 2020 226f 626a 6563            "objec
-000040b0: 745f 6964 223a 207b 0a20 2020 2020 2020  t_id": {.       
-000040c0: 2020 2020 2020 2020 2020 2020 2022 7479               "ty
-000040d0: 7065 223a 2022 7374 7222 2c0a 2020 2020  pe": "str",.    
-000040e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000040f0: 2264 6573 6372 6970 7469 6f6e 223a 2022  "description": "
-00004100: 5468 6520 6e61 6d65 206f 6620 7468 6520  The name of the 
-00004110: 736b 7561 206f 626a 6563 7420 7468 6174  skua object that
-00004120: 2061 7070 6561 7265 6422 0a20 2020 2020   appeared".     
-00004130: 2020 2020 2020 2020 2020 207d 2c0a 2020             },.  
-00004140: 2020 2020 2020 2020 2020 2020 2020 2270                "p
-00004150: 6f73 5822 3a20 7b0a 2020 2020 2020 2020  osX": {.        
-00004160: 2020 2020 2020 2020 2020 2020 2274 7970              "typ
-00004170: 6522 3a20 2266 6c6f 6174 222c 0a20 2020  e": "float",.   
-00004180: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004190: 2022 6465 7363 7269 7074 696f 6e22 3a20   "description": 
-000041a0: 2254 6865 2078 2d70 6f73 6974 696f 6e20  "The x-position 
-000041b0: 6f66 2074 6865 2073 6b75 6120 7468 6174  of the skua that
-000041c0: 2061 7070 6561 7265 6422 0a20 2020 2020   appeared".     
-000041d0: 2020 2020 2020 2020 2020 207d 2c0a 2020             },.  
-000041e0: 2020 2020 2020 2020 2020 2020 2020 2270                "p
-000041f0: 6f73 5922 3a20 7b0a 2020 2020 2020 2020  osY": {.        
-00004200: 2020 2020 2020 2020 2020 2020 2274 7970              "typ
-00004210: 6522 3a20 2266 6c6f 6174 222c 0a20 2020  e": "float",.   
-00004220: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004230: 2022 6465 7363 7269 7074 696f 6e22 3a20   "description": 
-00004240: 2254 6865 2079 2d70 6f73 6974 696f 6e20  "The y-position 
-00004250: 6f66 2074 6865 2073 6b75 6120 7468 6174  of the skua that
-00004260: 2061 7070 6561 7265 6422 0a20 2020 2020   appeared".     
-00004270: 2020 2020 2020 2020 2020 207d 2c0a 2020             },.  
-00004280: 2020 2020 2020 2020 2020 2020 2020 2270                "p
-00004290: 6f73 5a22 3a20 7b0a 2020 2020 2020 2020  osZ": {.        
-000042a0: 2020 2020 2020 2020 2020 2020 2274 7970              "typ
-000042b0: 6522 3a20 2266 6c6f 6174 222c 0a20 2020  e": "float",.   
-000042c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000042d0: 2022 6465 7363 7269 7074 696f 6e22 3a20   "description": 
-000042e0: 2254 6865 207a 2d70 6f73 6974 696f 6e20  "The z-position 
-000042f0: 6f66 2074 6865 2073 6b75 6120 7468 6174  of the skua that
-00004300: 2061 7070 6561 7265 6422 0a20 2020 2020   appeared".     
-00004310: 2020 2020 2020 2020 2020 207d 0a20 2020             }.   
-00004320: 2020 2020 2020 2020 207d 0a20 2020 2020           }.     
-00004330: 2020 207d 2c0a 2020 2020 2020 2020 2273     },.        "s
-00004340: 6b75 615f 6d6f 7665 223a 207b 0a20 2020  kua_move": {.   
-00004350: 2020 2020 2020 2020 2022 6465 7363 7269           "descri
-00004360: 7074 696f 6e22 3a20 2245 7665 6e74 2077  ption": "Event w
-00004370: 6865 6e20 6120 736b 7561 206d 6f76 6573  hen a skua moves
-00004380: 2074 6f20 6120 6e65 7720 6c6f 6361 7469   to a new locati
-00004390: 6f6e 2069 6e20 7468 6520 6e65 7374 2f65  on in the nest/e
-000043a0: 6767 2064 6566 656e 7365 206d 696e 692d  gg defense mini-
-000043b0: 6761 6d65 2e22 2c0a 2020 2020 2020 2020  game.",.        
-000043c0: 2020 2020 2265 7665 6e74 5f64 6174 6122      "event_data"
-000043d0: 3a20 7b0a 2020 2020 2020 2020 2020 2020  : {.            
-000043e0: 2020 2020 226f 626a 6563 745f 6964 223a      "object_id":
-000043f0: 207b 0a20 2020 2020 2020 2020 2020 2020   {.             
-00004400: 2020 2020 2020 2022 7479 7065 223a 2022         "type": "
-00004410: 7374 7222 2c0a 2020 2020 2020 2020 2020  str",.          
-00004420: 2020 2020 2020 2020 2020 2264 6573 6372            "descr
-00004430: 6970 7469 6f6e 223a 2022 5468 6520 6e61  iption": "The na
-00004440: 6d65 206f 6620 7468 6520 736b 7561 206f  me of the skua o
-00004450: 626a 6563 7420 7468 6174 206d 6f76 6564  bject that moved
-00004460: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
-00004470: 2020 7d2c 0a20 2020 2020 2020 2020 2020    },.           
-00004480: 2020 2020 2022 6672 6f6d 5f70 6f73 6974       "from_posit
-00004490: 696f 6e5f 7822 3a20 7b0a 2020 2020 2020  ion_x": {.      
-000044a0: 2020 2020 2020 2020 2020 2020 2020 2274                "t
-000044b0: 7970 6522 3a20 2266 6c6f 6174 222c 0a20  ype": "float",. 
-000044c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000044d0: 2020 2022 6465 7363 7269 7074 696f 6e22     "description"
-000044e0: 3a20 2254 6865 2069 6e69 7469 616c 2078  : "The initial x
-000044f0: 2d70 6f73 6974 696f 6e20 6f66 2074 6865  -position of the
-00004500: 2073 6b75 6120 7468 6174 206d 6f76 6564   skua that moved
-00004510: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
-00004520: 2020 7d2c 0a20 2020 2020 2020 2020 2020    },.           
-00004530: 2020 2020 2022 6672 6f6d 5f70 6f73 6974       "from_posit
-00004540: 696f 6e5f 7922 3a20 7b0a 2020 2020 2020  ion_y": {.      
-00004550: 2020 2020 2020 2020 2020 2020 2020 2274                "t
-00004560: 7970 6522 3a20 2266 6c6f 6174 222c 0a20  ype": "float",. 
-00004570: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004580: 2020 2022 6465 7363 7269 7074 696f 6e22     "description"
-00004590: 3a20 2254 6865 2069 6e69 7469 616c 2079  : "The initial y
-000045a0: 2d70 6f73 6974 696f 6e20 6f66 2074 6865  -position of the
-000045b0: 2073 6b75 6120 7468 6174 206d 6f76 6564   skua that moved
-000045c0: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
-000045d0: 2020 7d2c 0a20 2020 2020 2020 2020 2020    },.           
-000045e0: 2020 2020 2022 6672 6f6d 5f70 6f73 6974       "from_posit
-000045f0: 696f 6e5f 7a22 3a20 7b0a 2020 2020 2020  ion_z": {.      
-00004600: 2020 2020 2020 2020 2020 2020 2020 2274                "t
-00004610: 7970 6522 3a20 2266 6c6f 6174 222c 0a20  ype": "float",. 
-00004620: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004630: 2020 2022 6465 7363 7269 7074 696f 6e22     "description"
-00004640: 3a20 2254 6865 2069 6e69 7469 616c 207a  : "The initial z
-00004650: 2d70 6f73 6974 696f 6e20 6f66 2074 6865  -position of the
-00004660: 2073 6b75 6120 7468 6174 206d 6f76 6564   skua that moved
-00004670: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
-00004680: 2020 7d2c 0a20 2020 2020 2020 2020 2020    },.           
-00004690: 2020 2020 2022 746f 5f70 6f73 6974 696f       "to_positio
-000046a0: 6e5f 7822 3a20 7b0a 2020 2020 2020 2020  n_x": {.        
-000046b0: 2020 2020 2020 2020 2020 2020 2274 7970              "typ
-000046c0: 6522 3a20 2266 6c6f 6174 222c 0a20 2020  e": "float",.   
-000046d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000046e0: 2022 6465 7363 7269 7074 696f 6e22 3a20   "description": 
-000046f0: 2254 6865 206e 6577 2078 2d70 6f73 6974  "The new x-posit
-00004700: 696f 6e20 6f66 2074 6865 2073 6b75 6120  ion of the skua 
-00004710: 7468 6174 206d 6f76 6564 220a 2020 2020  that moved".    
-00004720: 2020 2020 2020 2020 2020 2020 7d2c 0a20              },. 
-00004730: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00004740: 746f 5f70 6f73 6974 696f 6e5f 7922 3a20  to_position_y": 
-00004750: 7b0a 2020 2020 2020 2020 2020 2020 2020  {.              
-00004760: 2020 2020 2020 2274 7970 6522 3a20 2266        "type": "f
-00004770: 6c6f 6174 222c 0a20 2020 2020 2020 2020  loat",.         
-00004780: 2020 2020 2020 2020 2020 2022 6465 7363             "desc
-00004790: 7269 7074 696f 6e22 3a20 2254 6865 206e  ription": "The n
-000047a0: 6577 2079 2d70 6f73 6974 696f 6e20 6f66  ew y-position of
-000047b0: 2074 6865 2073 6b75 6120 7468 6174 206d   the skua that m
-000047c0: 6f76 6564 220a 2020 2020 2020 2020 2020  oved".          
-000047d0: 2020 2020 2020 7d2c 0a20 2020 2020 2020        },.       
-000047e0: 2020 2020 2020 2020 2022 746f 5f70 6f73           "to_pos
-000047f0: 6974 696f 6e5f 7a22 3a20 7b0a 2020 2020  ition_z": {.    
-00004800: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004810: 2274 7970 6522 3a20 2266 6c6f 6174 222c  "type": "float",
-00004820: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00004830: 2020 2020 2022 6465 7363 7269 7074 696f       "descriptio
-00004840: 6e22 3a20 2254 6865 206e 6577 207a 2d70  n": "The new z-p
-00004850: 6f73 6974 696f 6e20 6f66 2074 6865 2073  osition of the s
-00004860: 6b75 6120 7468 6174 206d 6f76 6564 220a  kua that moved".
-00004870: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004880: 7d0a 2020 2020 2020 2020 2020 2020 7d0a  }.            }.
-00004890: 2020 2020 2020 2020 7d2c 0a20 2020 2020          },.     
-000048a0: 2020 2022 656e 7465 725f 7265 6769 6f6e     "enter_region
-000048b0: 223a 207b 0a20 2020 2020 2020 2020 2020  ": {.           
-000048c0: 2022 6465 7363 7269 7074 696f 6e22 3a20   "description": 
-000048d0: 2245 7665 6e74 2077 6865 6e20 7468 6520  "Event when the 
-000048e0: 706c 6179 6572 206d 6f76 6573 2069 6e74  player moves int
-000048f0: 6f20 6f6e 6520 6f66 2074 6865 2072 6567  o one of the reg
-00004900: 696f 6e73 2063 6f6e 7461 696e 696e 6720  ions containing 
-00004910: 6120 6d69 6e69 2d67 616d 6520 6f72 206f  a mini-game or o
-00004920: 7468 6572 2066 6561 7475 7265 2e22 2c0a  ther feature.",.
-00004930: 2020 2020 2020 2020 2020 2020 2265 7665              "eve
-00004940: 6e74 5f64 6174 6122 3a20 7b0a 2020 2020  nt_data": {.    
-00004950: 2020 2020 2020 2020 2020 2020 2272 6567              "reg
-00004960: 696f 6e5f 6e61 6d65 223a 207b 0a20 2020  ion_name": {.   
-00004970: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004980: 2022 7479 7065 223a 2022 7374 7222 2c0a   "type": "str",.
-00004990: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000049a0: 2020 2020 2264 6573 6372 6970 7469 6f6e      "description
-000049b0: 223a 2022 5468 6520 6e61 6d65 206f 6620  ": "The name of 
-000049c0: 7468 6520 7265 6769 6f6e 2074 6865 2070  the region the p
-000049d0: 6c61 7965 7220 656e 7465 7265 6422 0a20  layer entered". 
-000049e0: 2020 2020 2020 2020 2020 2020 2020 207d                 }
-000049f0: 0a20 2020 2020 2020 2020 2020 207d 0a20  .            }. 
-00004a00: 2020 2020 2020 207d 2c0a 2020 2020 2020         },.      
-00004a10: 2020 2265 7869 745f 7265 6769 6f6e 223a    "exit_region":
-00004a20: 207b 0a20 2020 2020 2020 2020 2020 2022   {.            "
-00004a30: 6465 7363 7269 7074 696f 6e22 3a20 2245  description": "E
-00004a40: 7665 6e74 2077 6865 6e20 6120 6d6f 7665  vent when a move
-00004a50: 7320 6f75 7420 6f66 206f 6e65 206f 6620  s out of one of 
-00004a60: 7468 6520 7265 6769 6f6e 7320 636f 6e74  the regions cont
-00004a70: 6169 6e69 6e67 2061 206d 696e 692d 6761  aining a mini-ga
-00004a80: 6d65 206f 7220 6f74 6865 7220 6665 6174  me or other feat
-00004a90: 7572 652e 222c 0a20 2020 2020 2020 2020  ure.",.         
-00004aa0: 2020 2022 6576 656e 745f 6461 7461 223a     "event_data":
-00004ab0: 207b 0a20 2020 2020 2020 2020 2020 2020   {.             
-00004ac0: 2020 2022 7265 6769 6f6e 5f6e 616d 6522     "region_name"
-00004ad0: 3a20 7b0a 2020 2020 2020 2020 2020 2020  : {.            
-00004ae0: 2020 2020 2020 2020 2274 7970 6522 3a20          "type": 
-00004af0: 2273 7472 222c 0a20 2020 2020 2020 2020  "str",.         
-00004b00: 2020 2020 2020 2020 2020 2022 6465 7363             "desc
-00004b10: 7269 7074 696f 6e22 3a20 2254 6865 206e  ription": "The n
-00004b20: 616d 6520 6f66 2074 6865 2072 6567 696f  ame of the regio
-00004b30: 6e20 7468 6520 706c 6179 6572 206c 6566  n the player lef
-00004b40: 7422 0a20 2020 2020 2020 2020 2020 2020  t".             
-00004b50: 2020 207d 0a20 2020 2020 2020 2020 2020     }.           
-00004b60: 207d 0a20 2020 2020 2020 207d 2c0a 2020   }.        },.  
-00004b70: 2020 2020 2020 2261 6374 6976 6974 795f        "activity_
-00004b80: 6265 6769 6e22 3a20 7b0a 2020 2020 2020  begin": {.      
-00004b90: 2020 2020 2020 2264 6573 6372 6970 7469        "descripti
-00004ba0: 6f6e 223a 2022 4576 656e 7420 7768 656e  on": "Event when
-00004bb0: 2074 6865 2070 6c61 7965 7220 6265 6769   the player begi
-00004bc0: 6e73 2074 6f20 656e 6761 6765 2077 6974  ns to engage wit
-00004bd0: 6820 6120 6d69 6e69 2d67 616d 652e 222c  h a mini-game.",
-00004be0: 0a20 2020 2020 2020 2020 2020 2022 6576  .            "ev
-00004bf0: 656e 745f 6461 7461 223a 207b 0a20 2020  ent_data": {.   
-00004c00: 2020 2020 2020 2020 2020 2020 2022 6163               "ac
-00004c10: 7469 7669 7479 5f6e 616d 6522 3a20 7b0a  tivity_name": {.
-00004c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004c30: 2020 2020 2274 7970 6522 3a20 2265 6e75      "type": "enu
-00004c40: 6d28 736b 7561 732c 206d 6174 696e 675f  m(skuas, mating_
-00004c50: 6461 6e63 652c 202e 2e2e 2922 2c0a 2020  dance, ...)",.  
-00004c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004c70: 2020 2264 6573 6372 6970 7469 6f6e 223a    "description":
-00004c80: 2022 5468 6520 6e61 6d65 206f 6620 7468   "The name of th
-00004c90: 6520 6d69 6e69 2d67 616d 652f 6163 7469  e mini-game/acti
-00004ca0: 7669 7479 2077 6974 6820 7768 6963 6820  vity with which 
-00004cb0: 7468 6520 706c 6179 6572 2062 6567 616e  the player began
-00004cc0: 2074 6f20 656e 6761 6765 220a 2020 2020   to engage".    
-00004cd0: 2020 2020 2020 2020 2020 2020 7d0a 2020              }.  
-00004ce0: 2020 2020 2020 2020 2020 7d0a 2020 2020            }.    
-00004cf0: 2020 2020 7d2c 0a20 2020 2020 2020 2022      },.        "
-00004d00: 6163 7469 7669 7479 5f65 6e64 223a 207b  activity_end": {
-00004d10: 0a20 2020 2020 2020 2020 2020 2022 6465  .            "de
-00004d20: 7363 7269 7074 696f 6e22 3a20 224e 4f54  scription": "NOT
-00004d30: 2059 4554 2044 4f43 554d 454e 5445 4422   YET DOCUMENTED"
-00004d40: 2c0a 2020 2020 2020 2020 2020 2020 2265  ,.            "e
-00004d50: 7665 6e74 5f64 6174 6122 3a20 7b0a 2020  vent_data": {.  
-00004d60: 2020 2020 2020 2020 2020 2020 2020 2261                "a
-00004d70: 6374 6976 6974 795f 6e61 6d65 223a 207b  ctivity_name": {
-00004d80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00004d90: 2020 2020 2022 7479 7065 223a 2022 656e       "type": "en
-00004da0: 756d 2873 6b75 6173 2c20 6d61 7469 6e67  um(skuas, mating
-00004db0: 5f64 616e 6365 2c20 2e2e 2e29 222c 0a20  _dance, ...)",. 
-00004dc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004dd0: 2020 2022 6465 7363 7269 7074 696f 6e22     "description"
-00004de0: 3a20 224e 4f54 2059 4554 2044 4f43 554d  : "NOT YET DOCUM
-00004df0: 454e 5445 4422 0a20 2020 2020 2020 2020  ENTED".         
-00004e00: 2020 2020 2020 207d 0a20 2020 2020 2020         }.       
-00004e10: 2020 2020 207d 0a20 2020 2020 2020 207d       }.        }
-00004e20: 2c0a 2020 2020 2020 2020 2267 6c6f 6261  ,.        "globa
-00004e30: 6c5f 7469 6d65 725f 6265 6769 6e22 3a20  l_timer_begin": 
-00004e40: 7b0a 2020 2020 2020 2020 2020 2020 2264  {.            "d
-00004e50: 6573 6372 6970 7469 6f6e 223a 2022 4e4f  escription": "NO
-00004e60: 5420 5945 5420 444f 4355 4d45 4e54 4544  T YET DOCUMENTED
-00004e70: 222c 0a20 2020 2020 2020 2020 2020 2022  ",.            "
-00004e80: 6576 656e 745f 6461 7461 223a 207b 0a20  event_data": {. 
-00004e90: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00004ea0: 7469 6d65 5f72 656d 6169 6e69 6e67 223a  time_remaining":
-00004eb0: 207b 0a20 2020 2020 2020 2020 2020 2020   {.             
-00004ec0: 2020 2020 2020 2022 7479 7065 223a 2022         "type": "
-00004ed0: 696e 7422 2c0a 2020 2020 2020 2020 2020  int",.          
-00004ee0: 2020 2020 2020 2020 2020 2264 6573 6372            "descr
-00004ef0: 6970 7469 6f6e 223a 2022 5468 6520 6c65  iption": "The le
-00004f00: 6674 206f 6e20 7468 6520 676c 6f62 616c  ft on the global
-00004f10: 2074 696d 6572 220a 2020 2020 2020 2020   timer".        
-00004f20: 2020 2020 2020 2020 7d0a 2020 2020 2020          }.      
-00004f30: 2020 2020 2020 7d0a 2020 2020 2020 2020        }.        
-00004f40: 7d2c 0a20 2020 2020 2020 2022 676c 6f62  },.        "glob
-00004f50: 616c 5f74 696d 6572 5f70 6175 7365 223a  al_timer_pause":
-00004f60: 207b 0a20 2020 2020 2020 2020 2020 2022   {.            "
-00004f70: 6465 7363 7269 7074 696f 6e22 3a20 224e  description": "N
-00004f80: 4f54 2059 4554 2044 4f43 554d 454e 5445  OT YET DOCUMENTE
-00004f90: 4422 2c0a 2020 2020 2020 2020 2020 2020  D",.            
-00004fa0: 2265 7665 6e74 5f64 6174 6122 3a20 7b0a  "event_data": {.
-00004fb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004fc0: 2264 6174 6122 3a20 224e 4f54 2059 4554  "data": "NOT YET
-00004fd0: 2044 4f43 554d 454e 5445 4422 0a20 2020   DOCUMENTED".   
-00004fe0: 2020 2020 2020 2020 207d 0a20 2020 2020           }.     
-00004ff0: 2020 207d 2c0a 2020 2020 2020 2020 2267     },.        "g
-00005000: 6c6f 6261 6c5f 7469 6d65 725f 6578 7069  lobal_timer_expi
-00005010: 7265 6422 3a20 7b0a 2020 2020 2020 2020  red": {.        
-00005020: 2020 2020 2264 6573 6372 6970 7469 6f6e      "description
-00005030: 223a 2022 4e4f 5420 5945 5420 444f 4355  ": "NOT YET DOCU
-00005040: 4d45 4e54 4544 222c 0a20 2020 2020 2020  MENTED",.       
-00005050: 2020 2020 2022 6576 656e 745f 6461 7461       "event_data
-00005060: 223a 207b 0a20 2020 2020 2020 2020 2020  ": {.           
-00005070: 2020 2020 2022 6461 7461 223a 2022 4e4f       "data": "NO
-00005080: 5420 5945 5420 444f 4355 4d45 4e54 4544  T YET DOCUMENTED
-00005090: 220a 2020 2020 2020 2020 2020 2020 7d0a  ".            }.
-000050a0: 2020 2020 2020 2020 7d0a 2020 2020 7d2c          }.    },
-000050b0: 0a20 2020 2022 6465 7465 6374 6f72 7322  .    "detectors"
-000050c0: 3a20 7b0a 2020 2020 2020 2020 2270 6572  : {.        "per
-000050d0: 5f63 6f75 6e74 223a 207b 0a20 2020 2020  _count": {.     
-000050e0: 2020 2020 2020 2022 5265 6769 6f6e 456e         "RegionEn
-000050f0: 7465 7222 3a20 7b0a 2020 2020 2020 2020  ter": {.        
-00005100: 2020 2020 2020 2020 2274 7970 6522 3a20          "type": 
-00005110: 2252 6567 696f 6e45 6e74 6572 222c 0a20  "RegionEnter",. 
-00005120: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00005130: 656e 6162 6c65 6422 3a20 7472 7565 2c0a  enabled": true,.
-00005140: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005150: 2264 6573 6372 6970 7469 6f6e 223a 2022  "description": "
-00005160: 5472 6967 6765 7273 2061 6e20 6576 656e  Triggers an even
-00005170: 7420 7768 656e 2061 2070 6c61 7965 7220  t when a player 
-00005180: 656e 7465 7220 6120 7265 6769 6f6e 220a  enter a region".
-00005190: 2020 2020 2020 2020 2020 2020 7d2c 0a20              },. 
-000051a0: 2020 2020 2020 2020 2020 2022 5265 6769             "Regi
-000051b0: 6f6e 4578 6974 223a 207b 0a20 2020 2020  onExit": {.     
-000051c0: 2020 2020 2020 2020 2020 2022 7479 7065             "type
-000051d0: 223a 2022 5265 6769 6f6e 4578 6974 222c  ": "RegionExit",
-000051e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000051f0: 2022 656e 6162 6c65 6422 3a20 7472 7565   "enabled": true
-00005200: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00005210: 2020 2264 6573 6372 6970 7469 6f6e 223a    "description":
-00005220: 2022 5472 6967 6765 7273 2061 6e20 6576   "Triggers an ev
-00005230: 656e 7420 7768 656e 2061 2070 6c61 7965  ent when a playe
-00005240: 7220 6578 6974 2061 2072 6567 696f 6e22  r exit a region"
-00005250: 0a20 2020 2020 2020 2020 2020 207d 0a20  .            }. 
-00005260: 2020 2020 2020 207d 2c0a 2020 2020 2020         },.      
-00005270: 2020 2261 6767 7265 6761 7465 223a 207b    "aggregate": {
-00005280: 7d0a 2020 2020 7d2c 0a20 2020 2022 6665  }.    },.    "fe
-00005290: 6174 7572 6573 223a 207b 0a20 2020 2020  atures": {.     
-000052a0: 2020 2022 7065 725f 636f 756e 7422 3a20     "per_count": 
-000052b0: 7b0a 2020 2020 2020 2020 2020 2020 2252  {.            "R
-000052c0: 6567 696f 6e44 7572 6174 696f 6e22 3a20  egionDuration": 
-000052d0: 7b0a 2020 2020 2020 2020 2020 2020 2020  {.              
-000052e0: 2020 2274 7970 6522 3a20 2252 6567 696f    "type": "Regio
-000052f0: 6e44 7572 6174 696f 6e22 2c0a 2020 2020  nDuration",.    
-00005300: 2020 2020 2020 2020 2020 2020 2265 6e61              "ena
-00005310: 626c 6564 223a 2074 7275 652c 0a20 2020  bled": true,.   
-00005320: 2020 2020 2020 2020 2020 2020 2022 636f               "co
-00005330: 756e 7422 3a20 3131 2c0a 2020 2020 2020  unt": 11,.      
-00005340: 2020 2020 2020 2020 2020 2270 7265 6669            "prefi
-00005350: 7822 3a20 2272 6567 696f 6e22 2c0a 2020  x": "region",.  
-00005360: 2020 2020 2020 2020 2020 2020 2020 2264                "d
-00005370: 6573 6372 6970 7469 6f6e 223a 2022 5468  escription": "Th
-00005380: 6520 6475 7261 7469 6f6e 206f 6620 7469  e duration of ti
-00005390: 6d65 2061 2070 6c61 7965 7220 706c 6179  me a player play
-000053a0: 6564 2069 6e20 6120 6769 7665 6e20 7265  ed in a given re
-000053b0: 6769 6f6e 206f 6620 7468 6520 6761 6d65  gion of the game
-000053c0: 2e22 2c0a 2020 2020 2020 2020 2020 2020  .",.            
-000053d0: 2020 2020 2272 6574 7572 6e5f 7479 7065      "return_type
-000053e0: 223a 2022 7469 6d65 6465 6c74 6122 0a20  ": "timedelta". 
-000053f0: 2020 2020 2020 2020 2020 207d 2c0a 2020             },.  
-00005400: 2020 2020 2020 2020 2020 2257 6164 646c            "Waddl
-00005410: 6550 6572 5265 6769 6f6e 223a 207b 0a20  ePerRegion": {. 
-00005420: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00005430: 7479 7065 223a 2022 5761 6464 6c65 5065  type": "WaddlePe
-00005440: 7252 6567 696f 6e22 2c0a 2020 2020 2020  rRegion",.      
-00005450: 2020 2020 2020 2020 2020 2265 6e61 626c            "enabl
-00005460: 6564 223a 2074 7275 652c 0a20 2020 2020  ed": true,.     
-00005470: 2020 2020 2020 2020 2020 2022 636f 756e             "coun
-00005480: 7422 3a20 3131 2c0a 2020 2020 2020 2020  t": 11,.        
-00005490: 2020 2020 2020 2020 2270 7265 6669 7822          "prefix"
-000054a0: 3a20 2272 6567 696f 6e22 2c0a 2020 2020  : "region",.    
-000054b0: 2020 2020 2020 2020 2020 2020 2264 6573              "des
-000054c0: 6372 6970 7469 6f6e 223a 2022 5468 6520  cription": "The 
-000054d0: 6e75 6d62 6572 206f 6620 7469 6d65 7320  number of times 
-000054e0: 6120 706c 6179 6572 2077 6164 646c 6564  a player waddled
-000054f0: 2069 6e20 6120 6769 7665 6e20 7265 6769   in a given regi
-00005500: 6f6e 206f 6620 7468 6520 6761 6d65 2e22  on of the game."
-00005510: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00005520: 2020 2272 6574 7572 6e5f 7479 7065 223a    "return_type":
-00005530: 2022 696e 7422 0a20 2020 2020 2020 2020   "int".         
-00005540: 2020 207d 0a20 2020 2020 2020 207d 2c0a     }.        },.
-00005550: 2020 2020 2020 2020 2261 6767 7265 6761          "aggrega
-00005560: 7465 223a 207b 0a20 2020 2020 2020 2020  te": {.         
-00005570: 2020 2022 4761 7a65 436f 756e 7422 3a20     "GazeCount": 
-00005580: 7b0a 2020 2020 2020 2020 2020 2020 2020  {.              
-00005590: 2020 2274 7970 6522 3a20 2247 617a 6543    "type": "GazeC
-000055a0: 6f75 6e74 222c 0a20 2020 2020 2020 2020  ount",.         
-000055b0: 2020 2020 2020 2022 656e 6162 6c65 6422         "enabled"
-000055c0: 3a20 7472 7565 2c0a 2020 2020 2020 2020  : true,.        
-000055d0: 2020 2020 2020 2020 2264 6573 6372 6970          "descrip
-000055e0: 7469 6f6e 223a 2022 5468 6520 6e75 6d62  tion": "The numb
-000055f0: 6572 206f 6620 7469 6d65 7320 6120 706c  er of times a pl
-00005600: 6179 6572 2077 6164 646c 6564 2069 6e20  ayer waddled in 
-00005610: 6120 6769 7665 6e20 7265 6769 6f6e 206f  a given region o
-00005620: 6620 7468 6520 6761 6d65 2e22 2c0a 2020  f the game.",.  
-00005630: 2020 2020 2020 2020 2020 2020 2020 2272                "r
-00005640: 6574 7572 6e5f 7479 7065 223a 2022 696e  eturn_type": "in
-00005650: 7422 0a20 2020 2020 2020 2020 2020 207d  t".            }
-00005660: 2c0a 2020 2020 2020 2020 2020 2020 2250  ,.            "P
-00005670: 6963 6b75 7052 6f63 6b43 6f75 6e74 223a  ickupRockCount":
-00005680: 207b 0a20 2020 2020 2020 2020 2020 2020   {.             
-00005690: 2020 2022 7479 7065 223a 2022 5069 636b     "type": "Pick
-000056a0: 7570 526f 636b 436f 756e 7422 2c0a 2020  upRockCount",.  
-000056b0: 2020 2020 2020 2020 2020 2020 2020 2265                "e
-000056c0: 6e61 626c 6564 223a 2074 7275 652c 0a20  nabled": true,. 
-000056d0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-000056e0: 6465 7363 7269 7074 696f 6e22 3a20 2254  description": "T
-000056f0: 6865 2064 7572 6174 696f 6e20 6561 6368  he duration each
-00005700: 2073 6573 7369 6f6e 2074 6f6f 6b2e 222c   session took.",
-00005710: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00005720: 2022 7265 7475 726e 5f74 7970 6522 3a20   "return_type": 
-00005730: 2269 6e74 220a 2020 2020 2020 2020 2020  "int".          
-00005740: 2020 7d2c 0a20 2020 2020 2020 2020 2020    },.           
-00005750: 2022 506c 6179 6572 5761 6464 6c65 436f   "PlayerWaddleCo
-00005760: 756e 7422 3a20 7b0a 2020 2020 2020 2020  unt": {.        
-00005770: 2020 2020 2020 2020 2274 7970 6522 3a20          "type": 
-00005780: 2250 6c61 7965 7257 6164 646c 6543 6f75  "PlayerWaddleCou
-00005790: 6e74 222c 0a20 2020 2020 2020 2020 2020  nt",.           
-000057a0: 2020 2020 2022 656e 6162 6c65 6422 3a20       "enabled": 
-000057b0: 7472 7565 2c0a 2020 2020 2020 2020 2020  true,.          
-000057c0: 2020 2020 2020 2264 6573 6372 6970 7469        "descripti
-000057d0: 6f6e 223a 2022 5468 6520 6e75 6d62 6572  on": "The number
-000057e0: 206f 6620 7469 6d65 7320 6120 706c 6179   of times a play
-000057f0: 6572 2077 6164 646c 6564 2e22 2c0a 2020  er waddled.",.  
-00005800: 2020 2020 2020 2020 2020 2020 2020 2272                "r
-00005810: 6574 7572 6e5f 7479 7065 223a 2022 696e  eturn_type": "in
-00005820: 7422 0a20 2020 2020 2020 2020 2020 207d  t".            }
-00005830: 2c0a 2020 2020 2020 2020 2020 2020 2253  ,.            "S
-00005840: 6573 7369 6f6e 4475 7261 7469 6f6e 223a  essionDuration":
-00005850: 207b 0a20 2020 2020 2020 2020 2020 2020   {.             
-00005860: 2020 2022 7479 7065 223a 2022 5365 7373     "type": "Sess
-00005870: 696f 6e44 7572 6174 696f 6e22 2c0a 2020  ionDuration",.  
-00005880: 2020 2020 2020 2020 2020 2020 2020 2265                "e
-00005890: 6e61 626c 6564 223a 2074 7275 652c 0a20  nabled": true,. 
-000058a0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-000058b0: 6465 7363 7269 7074 696f 6e22 3a20 2254  description": "T
-000058c0: 6865 2064 7572 6174 696f 6e20 6561 6368  he duration each
-000058d0: 2073 6573 7369 6f6e 2074 6f6f 6b2e 222c   session took.",
-000058e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000058f0: 2022 7265 7475 726e 5f74 7970 6522 3a20   "return_type": 
-00005900: 2274 696d 6564 656c 7461 220a 2020 2020  "timedelta".    
-00005910: 2020 2020 2020 2020 7d2c 0a20 2020 2020          },.     
-00005920: 2020 2020 2020 2022 4761 7a65 4475 7261         "GazeDura
-00005930: 7469 6f6e 223a 207b 0a20 2020 2020 2020  tion": {.       
-00005940: 2020 2020 2020 2020 2022 7479 7065 223a           "type":
-00005950: 2022 4761 7a65 4475 7261 7469 6f6e 222c   "GazeDuration",
-00005960: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00005970: 2022 656e 6162 6c65 6422 3a20 7472 7565   "enabled": true
-00005980: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00005990: 2020 2264 6573 6372 6970 7469 6f6e 223a    "description":
-000059a0: 2022 486f 7720 6c6f 6e67 2067 617a 6520   "How long gaze 
-000059b0: 6576 656e 7420 6c61 7374 2066 6f72 2e22  event last for."
-000059c0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-000059d0: 2020 2272 6574 7572 6e5f 7479 7065 223a    "return_type":
-000059e0: 2022 7469 6d65 6465 6c74 6122 0a20 2020   "timedelta".   
-000059f0: 2020 2020 2020 2020 207d 2c0a 2020 2020           },.    
-00005a00: 2020 2020 2020 2020 2252 6567 696f 6e45          "RegionE
-00005a10: 6e74 6572 436f 756e 7422 3a20 7b0a 2020  nterCount": {.  
-00005a20: 2020 2020 2020 2020 2020 2020 2020 2274                "t
-00005a30: 7970 6522 3a20 2252 6567 696f 6e45 6e74  ype": "RegionEnt
-00005a40: 6572 436f 756e 7422 2c0a 2020 2020 2020  erCount",.      
-00005a50: 2020 2020 2020 2020 2020 2265 6e61 626c            "enabl
-00005a60: 6564 223a 2066 616c 7365 2c0a 2020 2020  ed": false,.    
-00005a70: 2020 2020 2020 2020 2020 2020 2264 6573              "des
-00005a80: 6372 6970 7469 6f6e 223a 2022 5468 6520  cription": "The 
-00005a90: 6e75 6d62 6572 206f 6620 7469 6d65 7320  number of times 
-00005aa0: 6120 706c 6179 6572 2065 6e74 6572 6420  a player enterd 
-00005ab0: 666f 7220 6120 6769 7665 6e20 7265 6769  for a given regi
-00005ac0: 6f6e 206f 6620 7468 6520 6761 6d65 2e22  on of the game."
-00005ad0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00005ae0: 2020 2272 6574 7572 6e5f 7479 7065 223a    "return_type":
-00005af0: 2022 696e 7422 0a20 2020 2020 2020 2020   "int".         
-00005b00: 2020 207d 2c0a 2020 2020 2020 2020 2020     },.          
-00005b10: 2020 2241 6374 6976 6974 7943 6f6d 706c    "ActivityCompl
-00005b20: 6574 6564 223a 207b 0a20 2020 2020 2020  eted": {.       
-00005b30: 2020 2020 2020 2020 2022 7479 7065 223a           "type":
-00005b40: 2022 4163 7469 7669 7479 436f 6d70 6c65   "ActivityComple
-00005b50: 7465 6422 2c0a 2020 2020 2020 2020 2020  ted",.          
-00005b60: 2020 2020 2020 2265 6e61 626c 6564 223a        "enabled":
-00005b70: 2074 7275 652c 0a20 2020 2020 2020 2020   true,.         
-00005b80: 2020 2020 2020 2022 6465 7363 7269 7074         "descript
-00005b90: 696f 6e22 3a20 2254 6865 2061 6374 6976  ion": "The activ
-00005ba0: 6974 6965 7320 636f 6d70 6c65 7465 6420  ities completed 
-00005bb0: 696e 2061 2067 6976 656e 2073 6573 7369  in a given sessi
-00005bc0: 6f6e 2e22 2c0a 2020 2020 2020 2020 2020  on.",.          
-00005bd0: 2020 2020 2020 2272 6574 7572 6e5f 7479        "return_ty
-00005be0: 7065 223a 2022 696e 7422 0a20 2020 2020  pe": "int".     
-00005bf0: 2020 2020 2020 207d 2c0a 2020 2020 2020         },.      
-00005c00: 2020 2020 2020 2241 6374 6976 6974 7944        "ActivityD
-00005c10: 7572 6174 696f 6e22 3a20 7b0a 2020 2020  uration": {.    
-00005c20: 2020 2020 2020 2020 2020 2020 2274 7970              "typ
-00005c30: 6522 3a20 2241 6374 6976 6974 7944 7572  e": "ActivityDur
-00005c40: 6174 696f 6e22 2c0a 2020 2020 2020 2020  ation",.        
-00005c50: 2020 2020 2020 2020 2265 6e61 626c 6564          "enabled
-00005c60: 223a 2074 7275 652c 0a20 2020 2020 2020  ": true,.       
-00005c70: 2020 2020 2020 2020 2022 6465 7363 7269           "descri
-00005c80: 7074 696f 6e22 3a20 2248 6f77 206c 6f6e  ption": "How lon
-00005c90: 6720 6163 7469 7669 7479 206c 6173 7420  g activity last 
-00005ca0: 666f 722e 222c 0a20 2020 2020 2020 2020  for.",.         
-00005cb0: 2020 2020 2020 2022 7265 7475 726e 5f74         "return_t
-00005cc0: 7970 6522 3a20 2269 6e74 220a 2020 2020  ype": "int".    
-00005cd0: 2020 2020 2020 2020 7d2c 0a20 2020 2020          },.     
-00005ce0: 2020 2020 2020 2022 5265 6769 6f6e 7345         "RegionsE
-00005cf0: 6e63 6f75 6e74 6572 6564 223a 207b 0a20  ncountered": {. 
-00005d00: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00005d10: 7479 7065 223a 2022 5265 6769 6f6e 7345  type": "RegionsE
-00005d20: 6e63 6f75 6e74 6572 6564 222c 0a20 2020  ncountered",.   
-00005d30: 2020 2020 2020 2020 2020 2020 2022 656e               "en
-00005d40: 6162 6c65 6422 3a20 7472 7565 2c0a 2020  abled": true,.  
-00005d50: 2020 2020 2020 2020 2020 2020 2020 2264                "d
-00005d60: 6573 6372 6970 7469 6f6e 223a 2022 5468  escription": "Th
-00005d70: 6520 7265 6769 6f6e 7320 656e 7465 7265  e regions entere
-00005d80: 6420 696e 2061 2067 6976 656e 2073 6573  d in a given ses
-00005d90: 7369 6f6e 2e22 2c0a 2020 2020 2020 2020  sion.",.        
-00005da0: 2020 2020 2020 2020 2272 6574 7572 6e5f          "return_
-00005db0: 7479 7065 223a 2022 696e 7422 0a20 2020  type": "int".   
-00005dc0: 2020 2020 2020 2020 207d 0a20 2020 2020           }.     
-00005dd0: 2020 207d 0a20 2020 207d 2c0a 2020 2020     }.    },.    
-00005de0: 2263 6f6e 6669 6722 3a20 7b0a 2020 2020  "config": {.    
-00005df0: 2020 2020 2253 5550 504f 5254 4544 5f56      "SUPPORTED_V
-00005e00: 4552 5322 3a20 5b0a 2020 2020 2020 2020  ERS": [.        
-00005e10: 2020 2020 310a 2020 2020 2020 2020 5d0a      1.        ].
-00005e20: 2020 2020 7d0a 7d                            }.}
+00001330: 2020 2022 726f 7422 3a20 224c 6973 745b     "rot": "List[
+00001340: 666c 6f61 745d 220a 2020 2020 2020 2020  float]".        
+00001350: 2020 2020 2020 2020 2020 2020 7d2c 0a20              },. 
+00001360: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001370: 2020 2022 6465 7363 7269 7074 696f 6e22     "description"
+00001380: 3a20 2241 206c 6973 7420 6f66 2064 6963  : "A list of dic
+00001390: 7473 2c20 7768 6572 6520 6561 6368 2064  ts, where each d
+000013a0: 6963 7420 6973 206f 6e65 2066 7261 6d65  ict is one frame
+000013b0: 206f 6620 7269 6768 742d 6861 6e64 2064   of right-hand d
+000013c0: 6174 612c 2063 6f6e 7461 696e 696e 6720  ata, containing 
+000013d0: 6120 706f 7369 7469 6f6e 2061 6e64 2072  a position and r
+000013e0: 6f74 6174 696f 6e20 7665 6374 6f72 2c20  otation vector, 
+000013f0: 652e 672e 207b 5c22 706f 735c 223a 5b31  e.g. {\"pos\":[1
+00001400: 2c32 2c33 5d2c 205c 2272 6f74 5c22 3a5b  ,2,3], \"rot\":[
+00001410: 342c 352c 362c 375d 7d2e 220a 2020 2020  4,5,6,7]}.".    
+00001420: 2020 2020 2020 2020 2020 2020 7d0a 2020              }.  
+00001430: 2020 2020 2020 2020 2020 7d0a 2020 2020            }.    
+00001440: 2020 2020 7d2c 0a20 2020 2020 2020 2022      },.        "
+00001450: 706c 6179 6572 5f77 6164 646c 6522 3a20  player_waddle": 
+00001460: 7b0a 2020 2020 2020 2020 2020 2020 2264  {.            "d
+00001470: 6573 6372 6970 7469 6f6e 223a 2022 5768  escription": "Wh
+00001480: 656e 2061 2070 6c61 7965 7220 7065 7266  en a player perf
+00001490: 6f72 6d73 2061 2077 6164 646c 6520 6d6f  orms a waddle mo
+000014a0: 7665 6d65 6e74 2074 6f20 6d6f 7665 2074  vement to move t
+000014b0: 6865 6972 2070 656e 6775 696e 2061 7661  heir penguin ava
+000014c0: 7461 7220 666f 7277 6172 6422 2c0a 2020  tar forward",.  
+000014d0: 2020 2020 2020 2020 2020 2265 7665 6e74            "event
+000014e0: 5f64 6174 6122 3a20 7b0a 2020 2020 2020  _data": {.      
+000014f0: 2020 2020 2020 2020 2020 226f 626a 6563            "objec
+00001500: 745f 6964 223a 207b 0a20 2020 2020 2020  t_id": {.       
+00001510: 2020 2020 2020 2020 2020 2020 2022 7479               "ty
+00001520: 7065 223a 2022 7374 7222 2c0a 2020 2020  pe": "str",.    
+00001530: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001540: 2264 6573 6372 6970 7469 6f6e 223a 2022  "description": "
+00001550: 5468 6520 6e61 6d65 206f 662e 2e2e 2073  The name of... s
+00001560: 6f6d 6520 6f62 6a65 6374 220a 2020 2020  ome object".    
+00001570: 2020 2020 2020 2020 2020 2020 7d2c 0a20              },. 
+00001580: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00001590: 706f 735f 6f6c 6422 3a20 7b0a 2020 2020  pos_old": {.    
+000015a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000015b0: 2274 7970 6522 3a20 224c 6973 745b 666c  "type": "List[fl
+000015c0: 6f61 745d 222c 0a20 2020 2020 2020 2020  oat]",.         
+000015d0: 2020 2020 2020 2020 2020 2022 6465 7363             "desc
+000015e0: 7269 7074 696f 6e22 3a20 2254 6865 2070  ription": "The p
+000015f0: 7265 7669 6f75 7320 706f 7369 7469 6f6e  revious position
+00001600: 206f 6620 7468 6520 706c 6179 6572 2061   of the player a
+00001610: 7661 7461 7227 7320 6665 6574 2c20 696e  vatar's feet, in
+00001620: 205b 782c 2079 2c20 7a5d 2066 6f72 6d2c   [x, y, z] form,
+00001630: 2069 2e65 2e20 7768 6572 6520 7468 6520   i.e. where the 
+00001640: 7761 6464 6c65 2073 7461 7274 6564 2e22  waddle started."
+00001650: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00001660: 207d 2c0a 2020 2020 2020 2020 2020 2020   },.            
+00001670: 2020 2020 2270 6f73 5f6e 6577 223a 207b      "pos_new": {
+00001680: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00001690: 2020 2020 2022 7479 7065 223a 2022 4c69       "type": "Li
+000016a0: 7374 5b66 6c6f 6174 5d22 2c0a 2020 2020  st[float]",.    
+000016b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000016c0: 2264 6573 6372 6970 7469 6f6e 223a 2022  "description": "
+000016d0: 5468 6520 7265 7375 6c74 696e 6720 706f  The resulting po
+000016e0: 7369 7469 6f6e 206f 6620 7468 6520 706c  sition of the pl
+000016f0: 6179 6572 2061 7661 7461 7227 7320 6665  ayer avatar's fe
+00001700: 6574 2c20 696e 205b 782c 2079 2c20 7a5d  et, in [x, y, z]
+00001710: 2066 6f72 6d2c 2069 2e65 2e20 7768 6572   form, i.e. wher
+00001720: 6520 7468 6520 7761 6464 6c65 2065 6e64  e the waddle end
+00001730: 6564 2e22 0a20 2020 2020 2020 2020 2020  ed.".           
+00001740: 2020 2020 207d 2c0a 2020 2020 2020 2020       },.        
+00001750: 2020 2020 2020 2020 2273 6f75 7263 6522          "source"
+00001760: 3a20 7b0a 2020 2020 2020 2020 2020 2020  : {.            
+00001770: 2020 2020 2020 2020 2274 7970 6522 3a20          "type": 
+00001780: 224d 6f76 6554 7970 6522 2c0a 2020 2020  "MoveType",.    
+00001790: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000017a0: 2264 6573 6372 6970 7469 6f6e 223a 2022  "description": "
+000017b0: 496e 6469 6361 746f 7220 666f 7220 7768  Indicator for wh
+000017c0: 6574 6865 7220 7468 6520 706c 6179 6572  ether the player
+000017d0: 2077 6164 646c 6564 2062 7920 7072 6573   waddled by pres
+000017e0: 7369 6e67 2061 2062 7574 746f 6e2c 206f  sing a button, o
+000017f0: 7220 6279 206d 616b 696e 6720 7468 6520  r by making the 
+00001800: 2777 6164 646c 6527 2067 6573 7475 7265  'waddle' gesture
+00001810: 2077 6974 6820 7468 6569 7220 6865 6164   with their head
+00001820: 2e22 0a20 2020 2020 2020 2020 2020 2020  .".             
+00001830: 2020 207d 0a20 2020 2020 2020 2020 2020     }.           
+00001840: 207d 0a20 2020 2020 2020 207d 2c0a 2020   }.        },.  
+00001850: 2020 2020 2020 2267 617a 655f 6f62 6a65        "gaze_obje
+00001860: 6374 5f62 6567 696e 223a 207b 0a20 2020  ct_begin": {.   
+00001870: 2020 2020 2020 2020 2022 6465 7363 7269           "descri
+00001880: 7074 696f 6e22 3a20 2241 6e20 6576 656e  ption": "An even
+00001890: 7420 7472 6967 6765 7265 6420 7768 656e  t triggered when
+000018a0: 2074 6865 2070 6c61 7965 7220 6861 7320   the player has 
+000018b0: 6761 7a65 6420 6174 2061 6e20 6f62 6a65  gazed at an obje
+000018c0: 6374 2066 6f72 2061 7420 6c65 6173 7420  ct for at least 
+000018d0: 302e 3235 2073 6563 6f6e 6473 2c20 7768  0.25 seconds, wh
+000018e0: 6572 6520 2767 617a 6564 2061 7427 206d  ere 'gazed at' m
+000018f0: 6561 6e73 2074 6865 206f 626a 6563 7420  eans the object 
+00001900: 6973 2074 6865 206e 6561 7265 7374 206f  is the nearest o
+00001910: 6e20 6120 7261 7963 6173 7420 6672 6f6d  n a raycast from
+00001920: 2074 6865 2076 6965 7770 6f72 7420 6365   the viewport ce
+00001930: 6e74 6572 222c 0a20 2020 2020 2020 2020  nter",.         
+00001940: 2020 2022 6576 656e 745f 6461 7461 223a     "event_data":
+00001950: 207b 0a20 2020 2020 2020 2020 2020 2020   {.             
+00001960: 2020 2022 6f62 6a65 6374 5f69 6422 3a20     "object_id": 
+00001970: 7b0a 2020 2020 2020 2020 2020 2020 2020  {.              
+00001980: 2020 2020 2020 2274 7970 6522 3a20 2273        "type": "s
+00001990: 7472 222c 0a20 2020 2020 2020 2020 2020  tr",.           
+000019a0: 2020 2020 2020 2020 2022 6465 7363 7269           "descri
+000019b0: 7074 696f 6e22 3a20 2254 6865 206e 616d  ption": "The nam
+000019c0: 6520 6f66 2074 6865 206f 626a 6563 7420  e of the object 
+000019d0: 7468 6520 706c 6179 6572 2069 7320 6761  the player is ga
+000019e0: 7a69 6e67 2061 7422 0a20 2020 2020 2020  zing at".       
+000019f0: 2020 2020 2020 2020 207d 0a20 2020 2020           }.     
+00001a00: 2020 2020 2020 207d 0a20 2020 2020 2020         }.       
+00001a10: 207d 2c0a 2020 2020 2020 2020 2267 617a   },.        "gaz
+00001a20: 655f 6f62 6a65 6374 5f65 6e64 223a 207b  e_object_end": {
+00001a30: 0a20 2020 2020 2020 2020 2020 2022 6465  .            "de
+00001a40: 7363 7269 7074 696f 6e22 3a20 2241 6e20  scription": "An 
+00001a50: 6576 656e 7420 7472 6967 6765 7265 6420  event triggered 
+00001a60: 7768 656e 2074 6865 2070 6c61 7965 7220  when the player 
+00001a70: 7475 726e 7320 6177 6179 2066 726f 6d20  turns away from 
+00001a80: 616e 206f 626a 6563 7420 7468 6579 2764  an object they'd
+00001a90: 2067 617a 6564 2061 742c 2073 6f20 7468   gazed at, so th
+00001aa0: 6520 6f62 6a65 6374 2069 7320 6e6f 206c  e object is no l
+00001ab0: 6f6e 6765 7220 6e65 6172 6573 7420 6f6e  onger nearest on
+00001ac0: 2061 2072 6179 6361 7374 2066 726f 6d20   a raycast from 
+00001ad0: 7468 6520 7669 6577 706f 7274 2063 656e  the viewport cen
+00001ae0: 7465 722e 204e 6f74 6520 7468 6572 6520  ter. Note there 
+00001af0: 6d61 7920 6265 2061 2073 6d61 6c6c 2062  may be a small b
+00001b00: 7566 6665 7220 6172 6f75 6e64 2074 6865  uffer around the
+00001b10: 206f 626a 6563 7420 666f 7220 7468 6520   object for the 
+00001b20: 7261 7963 6173 742e 222c 0a20 2020 2020  raycast.",.     
+00001b30: 2020 2020 2020 2022 6576 656e 745f 6461         "event_da
+00001b40: 7461 223a 207b 0a20 2020 2020 2020 2020  ta": {.         
+00001b50: 2020 2020 2020 2022 6f62 6a65 6374 5f69         "object_i
+00001b60: 6422 3a20 7b0a 2020 2020 2020 2020 2020  d": {.          
+00001b70: 2020 2020 2020 2020 2020 2274 7970 6522            "type"
+00001b80: 3a20 2273 7472 222c 0a20 2020 2020 2020  : "str",.       
+00001b90: 2020 2020 2020 2020 2020 2020 2022 6465               "de
+00001ba0: 7363 7269 7074 696f 6e22 3a20 2254 6865  scription": "The
+00001bb0: 206e 616d 6520 6f66 2074 6865 206f 626a   name of the obj
+00001bc0: 6563 7420 7468 6520 706c 6179 6572 2068  ect the player h
+00001bd0: 6164 2070 7265 7669 6f75 736c 7920 6761  ad previously ga
+00001be0: 7a65 6420 6174 220a 2020 2020 2020 2020  zed at".        
+00001bf0: 2020 2020 2020 2020 7d0a 2020 2020 2020          }.      
+00001c00: 2020 2020 2020 7d0a 2020 2020 2020 2020        }.        
+00001c10: 7d2c 0a20 2020 2020 2020 2022 6275 6262  },.        "bubb
+00001c20: 6c65 5f70 6f70 223a 207b 0a20 2020 2020  le_pop": {.     
+00001c30: 2020 2020 2020 2022 6465 7363 7269 7074         "descript
+00001c40: 696f 6e22 3a20 2241 6e20 6576 656e 7420  ion": "An event 
+00001c50: 7472 6967 6765 7265 6420 7768 656e 2074  triggered when t
+00001c60: 6865 2070 6c61 7965 7220 706f 7073 2061  he player pops a
+00001c70: 2062 7562 626c 6520 696e 2074 6865 2062   bubble in the b
+00001c80: 7562 626c 652d 706f 7070 696e 6720 6d69  ubble-popping mi
+00001c90: 6e69 2d67 616d 652e 2041 2062 7562 626c  ni-game. A bubbl
+00001ca0: 6520 7368 6f75 6c64 2062 6520 706f 7070  e should be popp
+00001cb0: 6564 206f 6e20 6120 2762 6561 7427 206f  ed on a 'beat' o
+00001cc0: 6620 7468 6520 6d75 7369 632c 2062 7574  f the music, but
+00001cd0: 2063 616e 2062 6520 706f 7070 6564 2075   can be popped u
+00001ce0: 7020 746f 2030 2e35 2073 6563 6f6e 6473  p to 0.5 seconds
+00001cf0: 2062 6566 6f72 6520 6f72 2061 6674 6572   before or after
+00001d00: 2074 6865 2027 6265 6174 2e27 222c 0a20   the 'beat.'",. 
+00001d10: 2020 2020 2020 2020 2020 2022 6576 656e             "even
+00001d20: 745f 6461 7461 223a 207b 0a20 2020 2020  t_data": {.     
+00001d30: 2020 2020 2020 2020 2020 2022 6f62 6a65             "obje
+00001d40: 6374 5f69 6422 3a20 7b0a 2020 2020 2020  ct_id": {.      
+00001d50: 2020 2020 2020 2020 2020 2020 2020 2274                "t
+00001d60: 7970 6522 3a20 2273 7472 222c 0a20 2020  ype": "str",.   
+00001d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001d80: 2022 6465 7363 7269 7074 696f 6e22 3a20   "description": 
+00001d90: 2254 6865 206e 616d 6520 6f66 2074 6865  "The name of the
+00001da0: 2062 7562 626c 6520 6f62 6a65 6374 2074   bubble object t
+00001db0: 6865 2070 6c61 7965 7220 706f 7070 6564  he player popped
+00001dc0: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
+00001dd0: 2020 7d2c 0a20 2020 2020 2020 2020 2020    },.           
+00001de0: 2020 2020 2022 7469 6d69 6e67 5f65 7272       "timing_err
+00001df0: 6f72 223a 207b 0a20 2020 2020 2020 2020  or": {.         
+00001e00: 2020 2020 2020 2020 2020 2022 7479 7065             "type
+00001e10: 223a 2022 666c 6f61 7422 2c0a 2020 2020  ": "float",.    
+00001e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001e30: 2264 6573 6372 6970 7469 6f6e 223a 2022  "description": "
+00001e40: 5468 6520 7469 6d69 6e67 2064 6966 6665  The timing diffe
+00001e50: 7265 6e63 6520 6265 7477 6565 6e20 7468  rence between th
+00001e60: 6520 706f 7020 6576 656e 7420 616e 6420  e pop event and 
+00001e70: 7468 6520 6d75 7369 6320 2762 6561 742e  the music 'beat.
+00001e80: 2720 5468 6973 2076 616c 7565 2069 7320  ' This value is 
+00001e90: 696e 2074 6865 2072 616e 6765 205b 2d30  in the range [-0
+00001ea0: 2e35 2c20 302e 355d 2c20 7768 6572 6520  .5, 0.5], where 
+00001eb0: 6120 6e65 6761 7469 7665 2069 6e64 6963  a negative indic
+00001ec0: 6174 6573 2074 6865 2062 7562 626c 6520  ates the bubble 
+00001ed0: 7761 7320 706f 7070 6564 2062 6566 6f72  was popped befor
+00001ee0: 6520 7468 6520 2762 6561 742c 2720 616e  e the 'beat,' an
+00001ef0: 6420 706f 7369 7469 7665 2069 6e64 6963  d positive indic
+00001f00: 6174 6573 2070 6f70 7069 6e67 2061 6674  ates popping aft
+00001f10: 6572 2074 6865 2027 6265 6174 2e27 220a  er the 'beat.'".
+00001f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001f30: 7d0a 2020 2020 2020 2020 2020 2020 7d0a  }.            }.
+00001f40: 2020 2020 2020 2020 7d2c 0a20 2020 2020          },.     
+00001f50: 2020 2022 6561 745f 6669 7368 223a 207b     "eat_fish": {
+00001f60: 0a20 2020 2020 2020 2020 2020 2022 6465  .            "de
+00001f70: 7363 7269 7074 696f 6e22 3a20 2241 6e20  scription": "An 
+00001f80: 6576 656e 7420 7472 6967 6765 7265 6420  event triggered 
+00001f90: 7768 656e 2074 6865 2070 6c61 7965 7220  when the player 
+00001fa0: 6561 7473 2061 2066 6973 682e 222c 0a20  eats a fish.",. 
+00001fb0: 2020 2020 2020 2020 2020 2022 6576 656e             "even
+00001fc0: 745f 6461 7461 223a 207b 0a20 2020 2020  t_data": {.     
+00001fd0: 2020 2020 2020 2020 2020 2022 6f62 6a65             "obje
+00001fe0: 6374 5f69 6422 3a20 7b0a 2020 2020 2020  ct_id": {.      
+00001ff0: 2020 2020 2020 2020 2020 2020 2020 2274                "t
+00002000: 7970 6522 3a20 2273 7472 222c 0a20 2020  ype": "str",.   
+00002010: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002020: 2022 6465 7363 7269 7074 696f 6e22 3a20   "description": 
+00002030: 2254 6865 206e 616d 6520 6f66 2074 6865  "The name of the
+00002040: 2066 6973 6820 6f62 6a65 6374 2074 6865   fish object the
+00002050: 2070 6c61 7965 7220 6174 6522 0a20 2020   player ate".   
+00002060: 2020 2020 2020 2020 2020 2020 207d 0a20               }. 
+00002070: 2020 2020 2020 2020 2020 207d 0a20 2020             }.   
+00002080: 2020 2020 207d 2c0a 2020 2020 2020 2020       },.        
+00002090: 2273 7461 6e64 5f6f 6e5f 6e65 7374 223a  "stand_on_nest":
+000020a0: 207b 0a20 2020 2020 2020 2020 2020 2022   {.            "
+000020b0: 6465 7363 7269 7074 696f 6e22 3a20 2241  description": "A
+000020c0: 6e20 6576 656e 7420 7472 6967 6765 7265  n event triggere
+000020d0: 6420 7768 656e 2074 6865 2070 6c61 7965  d when the playe
+000020e0: 7220 7374 616e 6473 2061 746f 7020 6120  r stands atop a 
+000020f0: 6e65 7374 2e22 2c0a 2020 2020 2020 2020  nest.",.        
+00002100: 2020 2020 2265 7665 6e74 5f64 6174 6122      "event_data"
+00002110: 3a20 7b0a 2020 2020 2020 2020 2020 2020  : {.            
+00002120: 2020 2020 226e 6573 745f 6964 223a 207b      "nest_id": {
+00002130: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002140: 2020 2020 2022 7479 7065 223a 2022 7374       "type": "st
+00002150: 7222 2c0a 2020 2020 2020 2020 2020 2020  r",.            
+00002160: 2020 2020 2020 2020 2264 6573 6372 6970          "descrip
+00002170: 7469 6f6e 223a 2022 5468 6520 6e61 6d65  tion": "The name
+00002180: 206f 6620 7468 6520 6e65 7374 206f 626a   of the nest obj
+00002190: 6563 7420 7468 6520 706c 6179 6572 2073  ect the player s
+000021a0: 746f 6f64 206f 6e22 0a20 2020 2020 2020  tood on".       
+000021b0: 2020 2020 2020 2020 207d 2c0a 2020 2020           },.    
+000021c0: 2020 2020 2020 2020 2020 2020 226e 6573              "nes
+000021d0: 745f 706f 7322 3a20 7b0a 2020 2020 2020  t_pos": {.      
+000021e0: 2020 2020 2020 2020 2020 2020 2020 2274                "t
+000021f0: 7970 6522 3a20 224c 6973 745b 666c 6f61  ype": "List[floa
+00002200: 745d 222c 0a20 2020 2020 2020 2020 2020  t]",.           
+00002210: 2020 2020 2020 2020 2022 6465 7363 7269           "descri
+00002220: 7074 696f 6e22 3a20 2254 6865 2070 6f73  ption": "The pos
+00002230: 6974 696f 6e20 6f66 2074 6865 206e 6573  ition of the nes
+00002240: 7420 7468 6520 706c 6179 6572 2073 746f  t the player sto
+00002250: 6f64 206f 6e22 0a20 2020 2020 2020 2020  od on".         
+00002260: 2020 2020 2020 207d 0a20 2020 2020 2020         }.       
+00002270: 2020 2020 207d 0a20 2020 2020 2020 207d       }.        }
+00002280: 2c0a 2020 2020 2020 2020 2273 7461 6e64  ,.        "stand
+00002290: 5f6f 6e5f 726f 636b 223a 207b 0a20 2020  _on_rock": {.   
+000022a0: 2020 2020 2020 2020 2022 6465 7363 7269           "descri
+000022b0: 7074 696f 6e22 3a20 2241 6e20 6576 656e  ption": "An even
+000022c0: 7420 7472 6967 6765 7265 6420 7768 656e  t triggered when
+000022d0: 2074 6865 2070 6c61 7965 7220 7374 616e   the player stan
+000022e0: 6473 2061 746f 7020 6120 726f 636b 2e22  ds atop a rock."
+000022f0: 2c0a 2020 2020 2020 2020 2020 2020 2265  ,.            "e
+00002300: 7665 6e74 5f64 6174 6122 3a20 7b0a 2020  vent_data": {.  
+00002310: 2020 2020 2020 2020 2020 2020 2020 2272                "r
+00002320: 6f63 6b5f 6964 223a 207b 0a20 2020 2020  ock_id": {.     
+00002330: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00002340: 7479 7065 223a 2022 7374 7222 2c0a 2020  type": "str",.  
+00002350: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002360: 2020 2264 6573 6372 6970 7469 6f6e 223a    "description":
+00002370: 2022 5468 6520 6e61 6d65 206f 6620 7468   "The name of th
+00002380: 6520 726f 636b 206f 626a 6563 7420 7468  e rock object th
+00002390: 6520 706c 6179 6572 2073 746f 6f64 206f  e player stood o
+000023a0: 6e22 0a20 2020 2020 2020 2020 2020 2020  n".             
+000023b0: 2020 207d 2c0a 2020 2020 2020 2020 2020     },.          
+000023c0: 2020 2020 2020 2272 6f63 6b5f 706f 7322        "rock_pos"
+000023d0: 3a20 7b0a 2020 2020 2020 2020 2020 2020  : {.            
+000023e0: 2020 2020 2020 2020 2274 7970 6522 3a20          "type": 
+000023f0: 224c 6973 745b 666c 6f61 745d 222c 0a20  "List[float]",. 
+00002400: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002410: 2020 2022 6465 7363 7269 7074 696f 6e22     "description"
+00002420: 3a20 2254 6865 2070 6f73 6974 696f 6e20  : "The position 
+00002430: 6f66 2074 6865 2072 6f63 6b20 7768 656e  of the rock when
+00002440: 2069 7420 676f 7420 7374 6f6f 6420 6f6e   it got stood on
+00002450: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
+00002460: 2020 7d0a 2020 2020 2020 2020 2020 2020    }.            
+00002470: 7d0a 2020 2020 2020 2020 7d2c 0a20 2020  }.        },.   
+00002480: 2020 2020 2022 666c 6970 7065 725f 6261       "flipper_ba
+00002490: 7368 5f6e 6573 7422 3a20 7b0a 2020 2020  sh_nest": {.    
+000024a0: 2020 2020 2020 2020 2264 6573 6372 6970          "descrip
+000024b0: 7469 6f6e 223a 2022 416e 2065 7665 6e74  tion": "An event
+000024c0: 2074 7269 6767 6572 6564 2077 6865 6e20   triggered when 
+000024d0: 7468 6520 706c 6179 6572 206d 616b 6573  the player makes
+000024e0: 2061 2066 6c69 7070 6572 2d62 6173 6869   a flipper-bashi
+000024f0: 6e67 206d 6f76 6520 616e 6420 6d61 6b65  ng move and make
+00002500: 7320 636f 6e74 6163 7420 7769 7468 2061  s contact with a
+00002510: 206e 6573 742e 222c 0a20 2020 2020 2020   nest.",.       
+00002520: 2020 2020 2022 6576 656e 745f 6461 7461       "event_data
+00002530: 223a 207b 0a20 2020 2020 2020 2020 2020  ": {.           
+00002540: 2020 2020 2022 6e65 7374 5f69 6422 3a20       "nest_id": 
+00002550: 7b0a 2020 2020 2020 2020 2020 2020 2020  {.              
+00002560: 2020 2020 2020 2274 7970 6522 3a20 2273        "type": "s
+00002570: 7472 222c 0a20 2020 2020 2020 2020 2020  tr",.           
+00002580: 2020 2020 2020 2020 2022 6465 7363 7269           "descri
+00002590: 7074 696f 6e22 3a20 2254 6865 206e 616d  ption": "The nam
+000025a0: 6520 6f66 2074 6865 206e 6573 7420 6f62  e of the nest ob
+000025b0: 6a65 6374 2074 6865 2070 6c61 7965 7220  ject the player 
+000025c0: 6261 7368 6564 220a 2020 2020 2020 2020  bashed".        
+000025d0: 2020 2020 2020 2020 7d2c 0a20 2020 2020          },.     
+000025e0: 2020 2020 2020 2020 2020 2022 6e65 7374             "nest
+000025f0: 5f70 6f73 223a 207b 0a20 2020 2020 2020  _pos": {.       
+00002600: 2020 2020 2020 2020 2020 2020 2022 7479               "ty
+00002610: 7065 223a 2022 4c69 7374 5b66 6c6f 6174  pe": "List[float
+00002620: 5d22 2c0a 2020 2020 2020 2020 2020 2020  ]",.            
+00002630: 2020 2020 2020 2020 2264 6573 6372 6970          "descrip
+00002640: 7469 6f6e 223a 2022 5468 6520 706f 7369  tion": "The posi
+00002650: 7469 6f6e 206f 6620 7468 6520 6e65 7374  tion of the nest
+00002660: 2074 6865 2070 6c61 7965 7220 6261 7368   the player bash
+00002670: 6564 220a 2020 2020 2020 2020 2020 2020  ed".            
+00002680: 2020 2020 7d2c 0a20 2020 2020 2020 2020      },.         
+00002690: 2020 2020 2020 2022 6861 6e64 223a 207b         "hand": {
+000026a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000026b0: 2020 2020 2022 7479 7065 223a 2022 4861       "type": "Ha
+000026c0: 6e64 222c 0a20 2020 2020 2020 2020 2020  nd",.           
+000026d0: 2020 2020 2020 2020 2022 6465 7363 7269           "descri
+000026e0: 7074 696f 6e22 3a20 2257 6865 7468 6572  ption": "Whether
+000026f0: 2074 6865 2070 6c61 7965 7220 7065 7266   the player perf
+00002700: 6f72 6d65 6420 7468 6520 6261 7368 2077  ormed the bash w
+00002710: 6974 6820 7468 6569 7220 7269 6768 7420  ith their right 
+00002720: 6f72 206c 6566 7420 6861 6e64 2e22 0a20  or left hand.". 
+00002730: 2020 2020 2020 2020 2020 2020 2020 207d                 }
+00002740: 0a20 2020 2020 2020 2020 2020 207d 0a20  .            }. 
+00002750: 2020 2020 2020 207d 2c0a 2020 2020 2020         },.      
+00002760: 2020 2266 6c69 7070 6572 5f62 6173 685f    "flipper_bash_
+00002770: 7065 6e67 7569 6e22 3a20 7b0a 2020 2020  penguin": {.    
+00002780: 2020 2020 2020 2020 2264 6573 6372 6970          "descrip
+00002790: 7469 6f6e 223a 2022 416e 2065 7665 6e74  tion": "An event
+000027a0: 2074 7269 6767 6572 6564 2077 6865 6e20   triggered when 
+000027b0: 7468 6520 706c 6179 6572 206d 616b 6573  the player makes
+000027c0: 2061 2066 6c69 7070 6572 2d62 6173 6869   a flipper-bashi
+000027d0: 6e67 206d 6f76 6520 616e 6420 6d61 6b65  ng move and make
+000027e0: 7320 636f 6e74 6163 7420 7769 7468 2061  s contact with a
+000027f0: 6e6f 7468 6572 2070 656e 6775 696e 2e22  nother penguin."
+00002800: 2c0a 2020 2020 2020 2020 2020 2020 2265  ,.            "e
+00002810: 7665 6e74 5f64 6174 6122 3a20 7b0a 2020  vent_data": {.  
+00002820: 2020 2020 2020 2020 2020 2020 2020 2270                "p
+00002830: 656e 6775 696e 5f69 6422 3a20 7b0a 2020  enguin_id": {.  
+00002840: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002850: 2020 2274 7970 6522 3a20 2273 7472 222c    "type": "str",
+00002860: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002870: 2020 2020 2022 6465 7363 7269 7074 696f       "descriptio
+00002880: 6e22 3a20 2254 6865 206e 616d 6520 6f66  n": "The name of
+00002890: 2074 6865 2070 656e 6775 696e 206f 626a   the penguin obj
+000028a0: 6563 7420 7468 6520 706c 6179 6572 2062  ect the player b
+000028b0: 6173 6865 6422 0a20 2020 2020 2020 2020  ashed".         
+000028c0: 2020 2020 2020 207d 2c0a 2020 2020 2020         },.      
+000028d0: 2020 2020 2020 2020 2020 2270 656e 6775            "pengu
+000028e0: 696e 5f70 6f73 223a 207b 0a20 2020 2020  in_pos": {.     
+000028f0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00002900: 7479 7065 223a 2022 4c69 7374 5b66 6c6f  type": "List[flo
+00002910: 6174 5d22 2c0a 2020 2020 2020 2020 2020  at]",.          
+00002920: 2020 2020 2020 2020 2020 2264 6573 6372            "descr
+00002930: 6970 7469 6f6e 223a 2022 5468 6520 706f  iption": "The po
+00002940: 7369 7469 6f6e 206f 6620 7468 6520 6f74  sition of the ot
+00002950: 6865 7220 7065 6e67 7569 6e20 7768 656e  her penguin when
+00002960: 2069 7420 676f 7420 6261 7368 6564 220a   it got bashed".
+00002970: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002980: 7d2c 0a20 2020 2020 2020 2020 2020 2020  },.             
+00002990: 2020 2022 6861 6e64 223a 207b 0a20 2020     "hand": {.   
+000029a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000029b0: 2022 7479 7065 223a 2022 4861 6e64 222c   "type": "Hand",
+000029c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000029d0: 2020 2020 2022 6465 7363 7269 7074 696f       "descriptio
+000029e0: 6e22 3a20 2257 6865 7468 6572 2074 6865  n": "Whether the
+000029f0: 2070 6c61 7965 7220 7065 7266 6f72 6d65   player performe
+00002a00: 6420 7468 6520 6261 7368 2077 6974 6820  d the bash with 
+00002a10: 7468 6569 7220 7269 6768 7420 6f72 206c  their right or l
+00002a20: 6566 7420 6861 6e64 2e22 0a20 2020 2020  eft hand.".     
+00002a30: 2020 2020 2020 2020 2020 207d 0a20 2020             }.   
+00002a40: 2020 2020 2020 2020 207d 0a20 2020 2020           }.     
+00002a50: 2020 207d 2c0a 2020 2020 2020 2020 2266     },.        "f
+00002a60: 6c69 7070 6572 5f62 6173 685f 726f 636b  lipper_bash_rock
+00002a70: 223a 207b 0a20 2020 2020 2020 2020 2020  ": {.           
+00002a80: 2022 6465 7363 7269 7074 696f 6e22 3a20   "description": 
+00002a90: 2241 6e20 6576 656e 7420 7472 6967 6765  "An event trigge
+00002aa0: 7265 6420 7768 656e 2074 6865 2070 6c61  red when the pla
+00002ab0: 7965 7220 6d61 6b65 7320 6120 666c 6970  yer makes a flip
+00002ac0: 7065 722d 6261 7368 696e 6720 6d6f 7665  per-bashing move
+00002ad0: 2061 6e64 206d 616b 6573 2063 6f6e 7461   and makes conta
+00002ae0: 6374 2077 6974 6820 6120 726f 636b 2e22  ct with a rock."
+00002af0: 2c0a 2020 2020 2020 2020 2020 2020 2265  ,.            "e
+00002b00: 7665 6e74 5f64 6174 6122 3a20 7b0a 2020  vent_data": {.  
+00002b10: 2020 2020 2020 2020 2020 2020 2020 2272                "r
+00002b20: 6f63 6b5f 6964 223a 207b 0a20 2020 2020  ock_id": {.     
+00002b30: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00002b40: 7479 7065 223a 2022 7374 7222 2c0a 2020  type": "str",.  
+00002b50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002b60: 2020 2264 6573 6372 6970 7469 6f6e 223a    "description":
+00002b70: 2022 5468 6520 6e61 6d65 206f 6620 7468   "The name of th
+00002b80: 6520 726f 636b 206f 626a 6563 7420 7468  e rock object th
+00002b90: 6520 706c 6179 6572 2062 6173 6865 6422  e player bashed"
+00002ba0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002bb0: 207d 2c0a 2020 2020 2020 2020 2020 2020   },.            
+00002bc0: 2020 2020 2272 6f63 6b5f 706f 7322 3a20      "rock_pos": 
+00002bd0: 7b0a 2020 2020 2020 2020 2020 2020 2020  {.              
+00002be0: 2020 2020 2020 2274 7970 6522 3a20 224c        "type": "L
+00002bf0: 6973 745b 666c 6f61 745d 222c 0a20 2020  ist[float]",.   
+00002c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002c10: 2022 6465 7363 7269 7074 696f 6e22 3a20   "description": 
+00002c20: 2254 6865 2070 6f73 6974 696f 6e20 6f66  "The position of
+00002c30: 2074 6865 2072 6f63 6b20 7768 656e 2069   the rock when i
+00002c40: 7420 676f 7420 6261 7368 6564 220a 2020  t got bashed".  
+00002c50: 2020 2020 2020 2020 2020 2020 2020 7d2c                },
+00002c60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002c70: 2022 6861 6e64 223a 207b 0a20 2020 2020   "hand": {.     
+00002c80: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00002c90: 7479 7065 223a 2022 4861 6e64 222c 0a20  type": "Hand",. 
+00002ca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002cb0: 2020 2022 6465 7363 7269 7074 696f 6e22     "description"
+00002cc0: 3a20 2257 6865 7468 6572 2074 6865 2070  : "Whether the p
+00002cd0: 6c61 7965 7220 7065 7266 6f72 6d65 6420  layer performed 
+00002ce0: 7468 6520 6261 7368 2077 6974 6820 7468  the bash with th
+00002cf0: 6569 7220 7269 6768 7420 6f72 206c 6566  eir right or lef
+00002d00: 7420 6861 6e64 2e22 0a20 2020 2020 2020  t hand.".       
+00002d10: 2020 2020 2020 2020 207d 0a20 2020 2020           }.     
+00002d20: 2020 2020 2020 207d 0a20 2020 2020 2020         }.       
+00002d30: 207d 2c0a 2020 2020 2020 2020 2266 6c69   },.        "fli
+00002d40: 7070 6572 5f62 6173 685f 736b 7561 223a  pper_bash_skua":
+00002d50: 207b 0a20 2020 2020 2020 2020 2020 2022   {.            "
+00002d60: 6465 7363 7269 7074 696f 6e22 3a20 2241  description": "A
+00002d70: 6e20 6576 656e 7420 7472 6967 6765 7265  n event triggere
+00002d80: 6420 7768 656e 2074 6865 2070 6c61 7965  d when the playe
+00002d90: 7220 6d61 6b65 7320 6120 666c 6970 7065  r makes a flippe
+00002da0: 722d 6261 7368 696e 6720 6d6f 7665 2074  r-bashing move t
+00002db0: 6f20 7368 6f6f 2061 2073 6b75 6120 6177  o shoo a skua aw
+00002dc0: 6179 2066 726f 6d20 7468 6569 7220 6e65  ay from their ne
+00002dd0: 7374 2f65 6767 2e22 2c0a 2020 2020 2020  st/egg.",.      
+00002de0: 2020 2020 2020 2265 7665 6e74 5f64 6174        "event_dat
+00002df0: 6122 3a20 7b0a 2020 2020 2020 2020 2020  a": {.          
+00002e00: 2020 2020 2020 2273 6b75 615f 6964 223a        "skua_id":
+00002e10: 207b 0a20 2020 2020 2020 2020 2020 2020   {.             
+00002e20: 2020 2020 2020 2022 7479 7065 223a 2022         "type": "
+00002e30: 7374 7222 2c0a 2020 2020 2020 2020 2020  str",.          
+00002e40: 2020 2020 2020 2020 2020 2264 6573 6372            "descr
+00002e50: 6970 7469 6f6e 223a 2022 5468 6520 6e61  iption": "The na
+00002e60: 6d65 206f 6620 7468 6520 736b 7561 206f  me of the skua o
+00002e70: 626a 6563 7420 7468 6520 706c 6179 6572  bject the player
+00002e80: 2062 6173 6865 6422 0a20 2020 2020 2020   bashed".       
+00002e90: 2020 2020 2020 2020 207d 2c0a 2020 2020           },.    
+00002ea0: 2020 2020 2020 2020 2020 2020 2273 6b75              "sku
+00002eb0: 615f 706f 7322 3a20 7b0a 2020 2020 2020  a_pos": {.      
+00002ec0: 2020 2020 2020 2020 2020 2020 2020 2274                "t
+00002ed0: 7970 6522 3a20 224c 6973 745b 666c 6f61  ype": "List[floa
+00002ee0: 745d 222c 0a20 2020 2020 2020 2020 2020  t]",.           
+00002ef0: 2020 2020 2020 2020 2022 6465 7363 7269           "descri
+00002f00: 7074 696f 6e22 3a20 2254 6865 2070 6f73  ption": "The pos
+00002f10: 6974 696f 6e20 6f66 2074 6865 2073 6b75  ition of the sku
+00002f20: 6120 7768 656e 2069 7420 676f 7420 6261  a when it got ba
+00002f30: 7368 6564 220a 2020 2020 2020 2020 2020  shed".          
+00002f40: 2020 2020 2020 7d2c 0a20 2020 2020 2020        },.       
+00002f50: 2020 2020 2020 2020 2022 7065 6e67 7569           "pengui
+00002f60: 6e5f 706f 7322 3a20 7b0a 2020 2020 2020  n_pos": {.      
+00002f70: 2020 2020 2020 2020 2020 2020 2020 2274                "t
+00002f80: 7970 6522 3a20 2273 7472 222c 0a20 2020  ype": "str",.   
+00002f90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002fa0: 2022 6465 7363 7269 7074 696f 6e22 3a20   "description": 
+00002fb0: 2254 6865 2070 6f73 6974 696f 6e20 6f66  "The position of
+00002fc0: 2074 6865 2070 6c61 7965 7220 7768 656e   the player when
+00002fd0: 2074 6865 7920 736c 6170 7065 6420 7468   they slapped th
+00002fe0: 6520 736b 7561 2e20 4e4f 5445 203a 2054  e skua. NOTE : T
+00002ff0: 6869 7320 7761 7320 6164 6465 6420 6475  his was added du
+00003000: 6520 746f 2061 206d 6973 7461 6b65 2069  e to a mistake i
+00003010: 6e20 7370 6563 6966 6963 6174 696f 6e2c  n specification,
+00003020: 2061 6e64 2069 7320 7265 6475 6e64 616e   and is redundan
+00003030: 7420 7769 7468 2074 6865 2070 6f73 6974  t with the posit
+00003040: 696f 6e20 656c 656d 656e 7420 696e 2067  ion element in g
+00003050: 616d 655f 7374 6174 652e 220a 2020 2020  ame_state.".    
+00003060: 2020 2020 2020 2020 2020 2020 7d2c 0a20              },. 
+00003070: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00003080: 6861 6e64 223a 207b 0a20 2020 2020 2020  hand": {.       
+00003090: 2020 2020 2020 2020 2020 2020 2022 7479               "ty
+000030a0: 7065 223a 2022 4861 6e64 222c 0a20 2020  pe": "Hand",.   
+000030b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000030c0: 2022 6465 7363 7269 7074 696f 6e22 3a20   "description": 
+000030d0: 2257 6865 7468 6572 2074 6865 2070 6c61  "Whether the pla
+000030e0: 7965 7220 7065 7266 6f72 6d65 6420 7468  yer performed th
+000030f0: 6520 6261 7368 2077 6974 6820 7468 6569  e bash with thei
+00003100: 7220 7269 6768 7420 6f72 206c 6566 7420  r right or left 
+00003110: 6861 6e64 2e22 0a20 2020 2020 2020 2020  hand.".         
+00003120: 2020 2020 2020 207d 0a20 2020 2020 2020         }.       
+00003130: 2020 2020 207d 0a20 2020 2020 2020 207d       }.        }
+00003140: 2c0a 2020 2020 2020 2020 2270 6563 6b5f  ,.        "peck_
+00003150: 6e65 7374 223a 207b 0a20 2020 2020 2020  nest": {.       
+00003160: 2020 2020 2022 6465 7363 7269 7074 696f       "descriptio
+00003170: 6e22 3a20 2241 6e20 6576 656e 7420 7472  n": "An event tr
+00003180: 6967 6765 7265 6420 7768 656e 2074 6865  iggered when the
+00003190: 2070 6c61 7965 7227 7320 6265 616b 206d   player's beak m
+000031a0: 616b 6573 2063 6f6e 7461 6374 2077 6974  akes contact wit
+000031b0: 6820 6120 6e65 7374 2e22 2c0a 2020 2020  h a nest.",.    
+000031c0: 2020 2020 2020 2020 2265 7665 6e74 5f64          "event_d
+000031d0: 6174 6122 3a20 7b0a 2020 2020 2020 2020  ata": {.        
+000031e0: 2020 2020 2020 2020 226e 6573 745f 6964          "nest_id
+000031f0: 223a 207b 0a20 2020 2020 2020 2020 2020  ": {.           
+00003200: 2020 2020 2020 2020 2022 7479 7065 223a           "type":
+00003210: 2022 7374 7222 2c0a 2020 2020 2020 2020   "str",.        
+00003220: 2020 2020 2020 2020 2020 2020 2264 6573              "des
+00003230: 6372 6970 7469 6f6e 223a 2022 5468 6520  cription": "The 
+00003240: 6e61 6d65 206f 6620 7468 6520 6e65 7374  name of the nest
+00003250: 206f 626a 6563 7420 7468 6520 706c 6179   object the play
+00003260: 6572 2070 6563 6b65 6422 0a20 2020 2020  er pecked".     
+00003270: 2020 2020 2020 2020 2020 207d 2c0a 2020             },.  
+00003280: 2020 2020 2020 2020 2020 2020 2020 226e                "n
+00003290: 6573 745f 706f 7322 3a20 7b0a 2020 2020  est_pos": {.    
+000032a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000032b0: 2274 7970 6522 3a20 224c 6973 745b 666c  "type": "List[fl
+000032c0: 6f61 745d 222c 0a20 2020 2020 2020 2020  oat]",.         
+000032d0: 2020 2020 2020 2020 2020 2022 6465 7363             "desc
+000032e0: 7269 7074 696f 6e22 3a20 2254 6865 2070  ription": "The p
+000032f0: 6f73 6974 696f 6e20 6f66 2074 6865 206e  osition of the n
+00003300: 6573 7420 7468 6520 706c 6179 6572 2070  est the player p
+00003310: 6563 6b65 6422 0a20 2020 2020 2020 2020  ecked".         
+00003320: 2020 2020 2020 207d 0a20 2020 2020 2020         }.       
+00003330: 2020 2020 207d 0a20 2020 2020 2020 207d       }.        }
+00003340: 2c0a 2020 2020 2020 2020 2270 6563 6b5f  ,.        "peck_
+00003350: 7065 6e67 7569 6e22 3a20 7b0a 2020 2020  penguin": {.    
+00003360: 2020 2020 2020 2020 2264 6573 6372 6970          "descrip
+00003370: 7469 6f6e 223a 2022 416e 2065 7665 6e74  tion": "An event
+00003380: 2074 7269 6767 6572 6564 2077 6865 6e20   triggered when 
+00003390: 7468 6520 706c 6179 6572 2773 2062 6561  the player's bea
+000033a0: 6b20 6d61 6b65 7320 636f 6e74 6163 7420  k makes contact 
+000033b0: 7769 7468 2061 6e6f 7468 6572 2070 656e  with another pen
+000033c0: 6775 696e 2e22 2c0a 2020 2020 2020 2020  guin.",.        
+000033d0: 2020 2020 2265 7665 6e74 5f64 6174 6122      "event_data"
+000033e0: 3a20 7b0a 2020 2020 2020 2020 2020 2020  : {.            
+000033f0: 2020 2020 2270 656e 6775 696e 5f69 6422      "penguin_id"
+00003400: 3a20 7b0a 2020 2020 2020 2020 2020 2020  : {.            
+00003410: 2020 2020 2020 2020 2274 7970 6522 3a20          "type": 
+00003420: 2273 7472 222c 0a20 2020 2020 2020 2020  "str",.         
+00003430: 2020 2020 2020 2020 2020 2022 6465 7363             "desc
+00003440: 7269 7074 696f 6e22 3a20 2254 6865 206e  ription": "The n
+00003450: 616d 6520 6f66 2074 6865 2070 656e 6775  ame of the pengu
+00003460: 696e 206f 626a 6563 7420 7468 6520 706c  in object the pl
+00003470: 6179 6572 2070 6563 6b65 6422 0a20 2020  ayer pecked".   
+00003480: 2020 2020 2020 2020 2020 2020 207d 2c0a               },.
+00003490: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000034a0: 2270 656e 6775 696e 5f70 6f73 223a 207b  "penguin_pos": {
+000034b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000034c0: 2020 2020 2022 7479 7065 223a 2022 4c69       "type": "Li
+000034d0: 7374 5b66 6c6f 6174 5d22 2c0a 2020 2020  st[float]",.    
+000034e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000034f0: 2264 6573 6372 6970 7469 6f6e 223a 2022  "description": "
+00003500: 5468 6520 706f 7369 7469 6f6e 206f 6620  The position of 
+00003510: 7468 6520 6f74 6865 7220 7065 6e67 7569  the other pengui
+00003520: 6e20 7768 656e 2069 7420 676f 7420 7065  n when it got pe
+00003530: 636b 6564 220a 2020 2020 2020 2020 2020  cked".          
+00003540: 2020 2020 2020 7d0a 2020 2020 2020 2020        }.        
+00003550: 2020 2020 7d0a 2020 2020 2020 2020 7d2c      }.        },
+00003560: 0a20 2020 2020 2020 2022 7065 636b 5f72  .        "peck_r
+00003570: 6f63 6b22 3a20 7b0a 2020 2020 2020 2020  ock": {.        
+00003580: 2020 2020 2264 6573 6372 6970 7469 6f6e      "description
+00003590: 223a 2022 416e 2065 7665 6e74 2074 7269  ": "An event tri
+000035a0: 6767 6572 6564 2077 6865 6e20 7468 6520  ggered when the 
+000035b0: 706c 6179 6572 2773 2062 6561 6b20 6d61  player's beak ma
+000035c0: 6b65 7320 636f 6e74 6163 7420 7769 7468  kes contact with
+000035d0: 2061 2072 6f63 6b2e 222c 0a20 2020 2020   a rock.",.     
+000035e0: 2020 2020 2020 2022 6576 656e 745f 6461         "event_da
+000035f0: 7461 223a 207b 0a20 2020 2020 2020 2020  ta": {.         
+00003600: 2020 2020 2020 2022 726f 636b 5f69 6422         "rock_id"
+00003610: 3a20 7b0a 2020 2020 2020 2020 2020 2020  : {.            
+00003620: 2020 2020 2020 2020 2274 7970 6522 3a20          "type": 
+00003630: 2273 7472 222c 0a20 2020 2020 2020 2020  "str",.         
+00003640: 2020 2020 2020 2020 2020 2022 6465 7363             "desc
+00003650: 7269 7074 696f 6e22 3a20 2254 6865 206e  ription": "The n
+00003660: 616d 6520 6f66 2074 6865 2072 6f63 6b20  ame of the rock 
+00003670: 6f62 6a65 6374 2074 6865 2070 6c61 7965  object the playe
+00003680: 7220 7065 636b 6564 220a 2020 2020 2020  r pecked".      
+00003690: 2020 2020 2020 2020 2020 7d2c 0a20 2020            },.   
+000036a0: 2020 2020 2020 2020 2020 2020 2022 726f               "ro
+000036b0: 636b 5f70 6f73 223a 207b 0a20 2020 2020  ck_pos": {.     
+000036c0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+000036d0: 7479 7065 223a 2022 4c69 7374 5b66 6c6f  type": "List[flo
+000036e0: 6174 5d22 2c0a 2020 2020 2020 2020 2020  at]",.          
+000036f0: 2020 2020 2020 2020 2020 2264 6573 6372            "descr
+00003700: 6970 7469 6f6e 223a 2022 5468 6520 706f  iption": "The po
+00003710: 7369 7469 6f6e 206f 6620 7468 6520 726f  sition of the ro
+00003720: 636b 2077 6865 6e20 6974 2067 6f74 2070  ck when it got p
+00003730: 6563 6b65 6422 0a20 2020 2020 2020 2020  ecked".         
+00003740: 2020 2020 2020 207d 0a20 2020 2020 2020         }.       
+00003750: 2020 2020 207d 0a20 2020 2020 2020 207d       }.        }
+00003760: 2c0a 2020 2020 2020 2020 2270 6563 6b5f  ,.        "peck_
+00003770: 736b 7561 223a 207b 0a20 2020 2020 2020  skua": {.       
+00003780: 2020 2020 2022 6465 7363 7269 7074 696f       "descriptio
+00003790: 6e22 3a20 2241 6e20 6576 656e 7420 7472  n": "An event tr
+000037a0: 6967 6765 7265 6420 7768 656e 2074 6865  iggered when the
+000037b0: 2070 6c61 7965 7227 7320 6265 616b 206d   player's beak m
+000037c0: 616b 6573 2063 6f6e 7461 6374 2077 6974  akes contact wit
+000037d0: 6820 6120 736b 7561 2e22 2c0a 2020 2020  h a skua.",.    
+000037e0: 2020 2020 2020 2020 2265 7665 6e74 5f64          "event_d
+000037f0: 6174 6122 3a20 7b0a 2020 2020 2020 2020  ata": {.        
+00003800: 2020 2020 2020 2020 2273 6b75 615f 6964          "skua_id
+00003810: 223a 207b 0a20 2020 2020 2020 2020 2020  ": {.           
+00003820: 2020 2020 2020 2020 2022 7479 7065 223a           "type":
+00003830: 2022 7374 7222 2c0a 2020 2020 2020 2020   "str",.        
+00003840: 2020 2020 2020 2020 2020 2020 2264 6573              "des
+00003850: 6372 6970 7469 6f6e 223a 2022 5468 6520  cription": "The 
+00003860: 6e61 6d65 206f 6620 7468 6520 736b 7561  name of the skua
+00003870: 206f 626a 6563 7420 7468 6520 706c 6179   object the play
+00003880: 6572 2070 6563 6b65 6422 0a20 2020 2020  er pecked".     
+00003890: 2020 2020 2020 2020 2020 207d 2c0a 2020             },.  
+000038a0: 2020 2020 2020 2020 2020 2020 2020 2273                "s
+000038b0: 6b75 615f 706f 7322 3a20 7b0a 2020 2020  kua_pos": {.    
+000038c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000038d0: 2274 7970 6522 3a20 224c 6973 745b 666c  "type": "List[fl
+000038e0: 6f61 745d 222c 0a20 2020 2020 2020 2020  oat]",.         
+000038f0: 2020 2020 2020 2020 2020 2022 6465 7363             "desc
+00003900: 7269 7074 696f 6e22 3a20 2254 6865 2070  ription": "The p
+00003910: 6f73 6974 696f 6e20 6f66 2074 6865 2073  osition of the s
+00003920: 6b75 6120 7768 656e 2069 7420 676f 7420  kua when it got 
+00003930: 7065 636b 6564 220a 2020 2020 2020 2020  pecked".        
+00003940: 2020 2020 2020 2020 7d0a 2020 2020 2020          }.      
+00003950: 2020 2020 2020 7d0a 2020 2020 2020 2020        }.        
+00003960: 7d2c 0a20 2020 2020 2020 2022 7069 636b  },.        "pick
+00003970: 7570 5f72 6f63 6b22 3a20 7b0a 2020 2020  up_rock": {.    
+00003980: 2020 2020 2020 2020 2264 6573 6372 6970          "descrip
+00003990: 7469 6f6e 223a 2022 416e 2065 7665 6e74  tion": "An event
+000039a0: 2074 7269 6767 6572 6564 2077 6865 6e20   triggered when 
+000039b0: 7468 6520 706c 6179 6572 2070 6963 6b73  the player picks
+000039c0: 2075 7020 6120 726f 636b 206c 7969 6e67   up a rock lying
+000039d0: 206f 6e20 7468 6520 6772 6f75 6e64 2c20   on the ground, 
+000039e0: 7768 6963 6820 636f 6e74 7269 6275 7465  which contribute
+000039f0: 7320 746f 2074 6865 2062 7569 6c64 696e  s to the buildin
+00003a00: 6720 6f66 2074 6865 6972 206e 6573 742e  g of their nest.
+00003a10: 222c 0a20 2020 2020 2020 2020 2020 2022  ",.            "
+00003a20: 6576 656e 745f 6461 7461 223a 207b 0a20  event_data": {. 
+00003a30: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00003a40: 746f 7461 6c5f 7069 636b 6564 5f75 7022  total_picked_up"
+00003a50: 3a20 7b0a 2020 2020 2020 2020 2020 2020  : {.            
+00003a60: 2020 2020 2020 2020 2274 7970 6522 3a20          "type": 
+00003a70: 2269 6e74 222c 0a20 2020 2020 2020 2020  "int",.         
+00003a80: 2020 2020 2020 2020 2020 2022 6465 7363             "desc
+00003a90: 7269 7074 696f 6e22 3a20 2254 6865 2072  ription": "The r
+00003aa0: 756e 6e69 6e67 2074 6f74 616c 206f 6620  unning total of 
+00003ab0: 726f 636b 7320 7468 6520 706c 6179 6572  rocks the player
+00003ac0: 2068 6173 2070 6963 6b65 6420 7570 2e22   has picked up."
+00003ad0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00003ae0: 207d 0a20 2020 2020 2020 2020 2020 207d   }.            }
+00003af0: 0a20 2020 2020 2020 207d 2c0a 2020 2020  .        },.    
+00003b00: 2020 2020 2270 6c61 6365 5f72 6f63 6b22      "place_rock"
+00003b10: 3a20 7b0a 2020 2020 2020 2020 2020 2020  : {.            
+00003b20: 2264 6573 6372 6970 7469 6f6e 223a 2022  "description": "
+00003b30: 416e 2065 7665 6e74 2074 7269 6767 6572  An event trigger
+00003b40: 6564 2077 6865 6e20 7468 6520 706c 6179  ed when the play
+00003b50: 6572 2070 6c61 6365 7320 7468 6520 726f  er places the ro
+00003b60: 636b 2069 6e74 6f20 7468 6569 7220 6e65  ck into their ne
+00003b70: 7374 2e22 2c0a 2020 2020 2020 2020 2020  st.",.          
+00003b80: 2020 2265 7665 6e74 5f64 6174 6122 3a20    "event_data": 
+00003b90: 7b0a 2020 2020 2020 2020 2020 2020 2020  {.              
+00003ba0: 2020 2270 6572 6365 6e74 5f63 6f6d 706c    "percent_compl
+00003bb0: 6574 6522 3a20 7b0a 2020 2020 2020 2020  ete": {.        
+00003bc0: 2020 2020 2020 2020 2020 2020 2274 7970              "typ
+00003bd0: 6522 3a20 2266 6c6f 6174 222c 0a20 2020  e": "float",.   
+00003be0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003bf0: 2022 6465 7363 7269 7074 696f 6e22 3a20   "description": 
+00003c00: 2254 6865 2070 726f 706f 7274 696f 6e20  "The proportion 
+00003c10: 696e 6469 6361 7469 6e67 2074 6865 2070  indicating the p
+00003c20: 6c61 7965 7227 7320 7072 6f67 7265 7373  layer's progress
+00003c30: 2074 6f77 6172 6473 2063 6f6d 706c 6574   towards complet
+00003c40: 696e 6720 7468 6520 6e65 7374 2e20 536f  ing the nest. So
+00003c50: 2066 6172 2c20 7468 6520 6761 6d65 2068   far, the game h
+00003c60: 6173 2061 6c77 6179 7320 6265 656e 2073  as always been s
+00003c70: 6574 2074 6f20 7265 7175 6972 6520 3420  et to require 4 
+00003c80: 726f 636b 732e 220a 2020 2020 2020 2020  rocks.".        
+00003c90: 2020 2020 2020 2020 7d2c 0a20 2020 2020          },.     
+00003ca0: 2020 2020 2020 2020 2020 2022 726f 636b             "rock
+00003cb0: 5f63 6f75 6e74 223a 207b 0a20 2020 2020  _count": {.     
+00003cc0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00003cd0: 7479 7065 223a 2022 696e 7422 2c0a 2020  type": "int",.  
+00003ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003cf0: 2020 2264 6573 6372 6970 7469 6f6e 223a    "description":
+00003d00: 2022 5468 6520 746f 7461 6c20 6e75 6d62   "The total numb
+00003d10: 6572 206f 6620 726f 636b 7320 7468 6520  er of rocks the 
+00003d20: 706c 6179 6572 2068 6173 2070 6c61 6365  player has place
+00003d30: 6420 696e 2074 6865 6972 206e 6573 742e  d in their nest.
+00003d40: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
+00003d50: 2020 7d0a 2020 2020 2020 2020 2020 2020    }.            
+00003d60: 7d0a 2020 2020 2020 2020 7d2c 0a20 2020  }.        },.   
+00003d70: 2020 2020 2022 7075 7368 5f73 6e6f 7762       "push_snowb
+00003d80: 616c 6c22 3a20 7b0a 2020 2020 2020 2020  all": {.        
+00003d90: 2020 2020 2264 6573 6372 6970 7469 6f6e      "description
+00003da0: 223a 2022 416e 2065 7665 6e74 2074 7269  ": "An event tri
+00003db0: 6767 6572 6564 2077 6865 6e20 7468 6520  ggered when the 
+00003dc0: 706c 6179 6572 2070 7573 6865 7320 6120  player pushes a 
+00003dd0: 736e 6f77 6261 6c6c 2064 6f77 6e20 7468  snowball down th
+00003de0: 6520 6869 6c6c 2e22 2c0a 2020 2020 2020  e hill.",.      
+00003df0: 2020 2020 2020 2265 7665 6e74 5f64 6174        "event_dat
+00003e00: 6122 3a20 7b0a 2020 2020 2020 2020 2020  a": {.          
+00003e10: 2020 2020 2020 226f 626a 6563 745f 6964        "object_id
+00003e20: 223a 207b 0a20 2020 2020 2020 2020 2020  ": {.           
+00003e30: 2020 2020 2020 2020 2022 7479 7065 223a           "type":
+00003e40: 2022 7374 7222 2c0a 2020 2020 2020 2020   "str",.        
+00003e50: 2020 2020 2020 2020 2020 2020 2264 6573              "des
+00003e60: 6372 6970 7469 6f6e 223a 2022 5468 6520  cription": "The 
+00003e70: 6e61 6d65 206f 6620 7468 6520 736e 6f77  name of the snow
+00003e80: 6261 6c6c 206f 626a 6563 7420 7468 6520  ball object the 
+00003e90: 706c 6179 6572 2070 7573 6865 6422 0a20  player pushed". 
+00003ea0: 2020 2020 2020 2020 2020 2020 2020 207d                 }
+00003eb0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00003ec0: 2020 2270 7822 3a20 7b0a 2020 2020 2020    "px": {.      
+00003ed0: 2020 2020 2020 2020 2020 2020 2020 2274                "t
+00003ee0: 7970 6522 3a20 2266 6c6f 6174 222c 0a20  ype": "float",. 
+00003ef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003f00: 2020 2022 6465 7363 7269 7074 696f 6e22     "description"
+00003f10: 3a20 2254 6865 2078 2d70 6f73 6974 696f  : "The x-positio
+00003f20: 6e20 6f66 2074 6865 2070 6c61 7965 7220  n of the player 
+00003f30: 7768 656e 2074 6865 2065 7665 6e74 2068  when the event h
+00003f40: 6170 7065 6e65 6422 0a20 2020 2020 2020  appened".       
+00003f50: 2020 2020 2020 2020 207d 2c0a 2020 2020           },.    
+00003f60: 2020 2020 2020 2020 2020 2020 2270 7922              "py"
+00003f70: 3a20 7b0a 2020 2020 2020 2020 2020 2020  : {.            
+00003f80: 2020 2020 2020 2020 2274 7970 6522 3a20          "type": 
+00003f90: 2266 6c6f 6174 222c 0a20 2020 2020 2020  "float",.       
+00003fa0: 2020 2020 2020 2020 2020 2020 2022 6465               "de
+00003fb0: 7363 7269 7074 696f 6e22 3a20 2254 6865  scription": "The
+00003fc0: 2079 2d70 6f73 6974 696f 6e20 6f66 2074   y-position of t
+00003fd0: 6865 2070 6c61 7965 7220 7768 656e 2074  he player when t
+00003fe0: 6865 2065 7665 6e74 2068 6170 7065 6e65  he event happene
+00003ff0: 6422 0a20 2020 2020 2020 2020 2020 2020  d".             
+00004000: 2020 207d 2c0a 2020 2020 2020 2020 2020     },.          
+00004010: 2020 2020 2020 2270 7a22 3a20 7b0a 2020        "pz": {.  
+00004020: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004030: 2020 2274 7970 6522 3a20 2266 6c6f 6174    "type": "float
+00004040: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
+00004050: 2020 2020 2020 2022 6465 7363 7269 7074         "descript
+00004060: 696f 6e22 3a20 2254 6865 207a 2d70 6f73  ion": "The z-pos
+00004070: 6974 696f 6e20 6f66 2074 6865 2070 6c61  ition of the pla
+00004080: 7965 7220 7768 656e 2074 6865 2065 7665  yer when the eve
+00004090: 6e74 2068 6170 7065 6e65 6422 0a20 2020  nt happened".   
+000040a0: 2020 2020 2020 2020 2020 2020 207d 2c0a               },.
+000040b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000040c0: 2271 7822 3a20 7b0a 2020 2020 2020 2020  "qx": {.        
+000040d0: 2020 2020 2020 2020 2020 2020 2274 7970              "typ
+000040e0: 6522 3a20 2266 6c6f 6174 222c 0a20 2020  e": "float",.   
+000040f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004100: 2022 6465 7363 7269 7074 696f 6e22 3a20   "description": 
+00004110: 2254 6865 2078 2d63 6f6d 706f 6e65 6e74  "The x-component
+00004120: 206f 6620 7468 6520 7175 6174 6572 6e69   of the quaterni
+00004130: 6f6e 2066 6f72 2074 6865 2070 6c61 7965  on for the playe
+00004140: 7227 7320 6f72 6965 6e74 6174 696f 6e20  r's orientation 
+00004150: 7768 656e 2074 6865 2065 7665 6e74 2068  when the event h
+00004160: 6170 7065 6e65 6422 0a20 2020 2020 2020  appened".       
+00004170: 2020 2020 2020 2020 207d 2c0a 2020 2020           },.    
+00004180: 2020 2020 2020 2020 2020 2020 2271 7922              "qy"
+00004190: 3a20 7b0a 2020 2020 2020 2020 2020 2020  : {.            
+000041a0: 2020 2020 2020 2020 2274 7970 6522 3a20          "type": 
+000041b0: 2266 6c6f 6174 222c 0a20 2020 2020 2020  "float",.       
+000041c0: 2020 2020 2020 2020 2020 2020 2022 6465               "de
+000041d0: 7363 7269 7074 696f 6e22 3a20 2254 6865  scription": "The
+000041e0: 2079 2d63 6f6d 706f 6e65 6e74 206f 6620   y-component of 
+000041f0: 7468 6520 7175 6174 6572 6e69 6f6e 2066  the quaternion f
+00004200: 6f72 2074 6865 2070 6c61 7965 7227 7320  or the player's 
+00004210: 6f72 6965 6e74 6174 696f 6e20 7768 656e  orientation when
+00004220: 2074 6865 2065 7665 6e74 2068 6170 7065   the event happe
+00004230: 6e65 6422 0a20 2020 2020 2020 2020 2020  ned".           
+00004240: 2020 2020 207d 2c0a 2020 2020 2020 2020       },.        
+00004250: 2020 2020 2020 2020 2271 7a22 3a20 7b0a          "qz": {.
+00004260: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004270: 2020 2020 2274 7970 6522 3a20 2266 6c6f      "type": "flo
+00004280: 6174 222c 0a20 2020 2020 2020 2020 2020  at",.           
+00004290: 2020 2020 2020 2020 2022 6465 7363 7269           "descri
+000042a0: 7074 696f 6e22 3a20 2254 6865 207a 2d63  ption": "The z-c
+000042b0: 6f6d 706f 6e65 6e74 206f 6620 7468 6520  omponent of the 
+000042c0: 7175 6174 6572 6e69 6f6e 2066 6f72 2074  quaternion for t
+000042d0: 6865 2070 6c61 7965 7227 7320 6f72 6965  he player's orie
+000042e0: 6e74 6174 696f 6e20 7768 656e 2074 6865  ntation when the
+000042f0: 2065 7665 6e74 2068 6170 7065 6e65 6422   event happened"
+00004300: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00004310: 207d 2c0a 2020 2020 2020 2020 2020 2020   },.            
+00004320: 2020 2020 2271 7722 3a20 7b0a 2020 2020      "qw": {.    
+00004330: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004340: 2274 7970 6522 3a20 2266 6c6f 6174 222c  "type": "float",
+00004350: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00004360: 2020 2020 2022 6465 7363 7269 7074 696f       "descriptio
+00004370: 6e22 3a20 2254 6865 2077 2d63 6f6d 706f  n": "The w-compo
+00004380: 6e65 6e74 206f 6620 7468 6520 7175 6174  nent of the quat
+00004390: 6572 6e69 6f6e 2066 6f72 2074 6865 2070  ernion for the p
+000043a0: 6c61 7965 7227 7320 6f72 6965 6e74 6174  layer's orientat
+000043b0: 696f 6e20 7768 656e 2074 6865 2065 7665  ion when the eve
+000043c0: 6e74 2068 6170 7065 6e65 6422 0a20 2020  nt happened".   
+000043d0: 2020 2020 2020 2020 2020 2020 207d 0a20               }. 
+000043e0: 2020 2020 2020 2020 2020 207d 0a20 2020             }.   
+000043f0: 2020 2020 207d 2c0a 2020 2020 2020 2020       },.        
+00004400: 2272 696e 675f 6368 696d 6522 3a20 7b0a  "ring_chime": {.
+00004410: 2020 2020 2020 2020 2020 2020 2264 6573              "des
+00004420: 6372 6970 7469 6f6e 223a 2022 416e 2065  cription": "An e
+00004430: 7665 6e74 2077 6865 6e20 7468 6520 706c  vent when the pl
+00004440: 6179 6572 2072 696e 6773 206f 6e65 206f  ayer rings one o
+00004450: 6620 7468 6520 6368 696d 6573 2069 6e20  f the chimes in 
+00004460: 7468 6520 6368 696d 6520 6d69 6e69 2d67  the chime mini-g
+00004470: 616d 652e 222c 0a20 2020 2020 2020 2020  ame.",.         
+00004480: 2020 2022 6576 656e 745f 6461 7461 223a     "event_data":
+00004490: 207b 0a20 2020 2020 2020 2020 2020 2020   {.             
+000044a0: 2020 2022 6e6f 7465 5f70 6c61 7965 6422     "note_played"
+000044b0: 3a20 7b0a 2020 2020 2020 2020 2020 2020  : {.            
+000044c0: 2020 2020 2020 2020 2274 7970 6522 3a20          "type": 
+000044d0: 2273 7472 222c 0a20 2020 2020 2020 2020  "str",.         
+000044e0: 2020 2020 2020 2020 2020 2022 6465 7363             "desc
+000044f0: 7269 7074 696f 6e22 3a20 2254 6865 206e  ription": "The n
+00004500: 616d 6520 6f66 2074 6865 2063 6869 6d65  ame of the chime
+00004510: 2074 6865 2070 6c61 7965 7220 7261 6e67   the player rang
+00004520: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
+00004530: 2020 7d0a 2020 2020 2020 2020 2020 2020    }.            
+00004540: 7d0a 2020 2020 2020 2020 7d2c 0a20 2020  }.        },.   
+00004550: 2020 2020 2022 6275 6262 6c65 5f61 7070       "bubble_app
+00004560: 6561 7265 6422 3a20 7b0a 2020 2020 2020  eared": {.      
+00004570: 2020 2020 2020 2264 6573 6372 6970 7469        "descripti
+00004580: 6f6e 223a 2022 4576 656e 7420 7768 656e  on": "Event when
+00004590: 2061 206e 6577 2062 7562 626c 6520 6170   a new bubble ap
+000045a0: 7065 6172 7320 696e 2074 6865 206d 6174  pears in the mat
+000045b0: 696e 6720 6461 6e63 6520 6d69 6e69 6761  ing dance miniga
+000045c0: 6d65 2e22 2c0a 2020 2020 2020 2020 2020  me.",.          
+000045d0: 2020 2265 7665 6e74 5f64 6174 6122 3a20    "event_data": 
+000045e0: 7b0a 2020 2020 2020 2020 2020 2020 2020  {.              
+000045f0: 2020 226f 626a 6563 745f 6964 223a 207b    "object_id": {
+00004600: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00004610: 2020 2020 2022 7479 7065 223a 2022 7374       "type": "st
+00004620: 7222 2c0a 2020 2020 2020 2020 2020 2020  r",.            
+00004630: 2020 2020 2020 2020 2264 6573 6372 6970          "descrip
+00004640: 7469 6f6e 223a 2022 5468 6520 6e61 6d65  tion": "The name
+00004650: 206f 6620 7468 6520 6275 6262 6c65 206f   of the bubble o
+00004660: 626a 6563 7420 7468 6174 2061 7070 6561  bject that appea
+00004670: 7265 6422 0a20 2020 2020 2020 2020 2020  red".           
+00004680: 2020 2020 207d 2c0a 2020 2020 2020 2020       },.        
+00004690: 2020 2020 2020 2020 2270 6f73 5822 3a20          "posX": 
+000046a0: 7b0a 2020 2020 2020 2020 2020 2020 2020  {.              
+000046b0: 2020 2020 2020 2274 7970 6522 3a20 2266        "type": "f
+000046c0: 6c6f 6174 222c 0a20 2020 2020 2020 2020  loat",.         
+000046d0: 2020 2020 2020 2020 2020 2022 6465 7363             "desc
+000046e0: 7269 7074 696f 6e22 3a20 2254 6865 2078  ription": "The x
+000046f0: 2d70 6f73 6974 696f 6e20 6f66 2074 6865  -position of the
+00004700: 2062 7562 626c 6520 7468 6174 2061 7070   bubble that app
+00004710: 6561 7265 6422 0a20 2020 2020 2020 2020  eared".         
+00004720: 2020 2020 2020 207d 2c0a 2020 2020 2020         },.      
+00004730: 2020 2020 2020 2020 2020 2270 6f73 5922            "posY"
+00004740: 3a20 7b0a 2020 2020 2020 2020 2020 2020  : {.            
+00004750: 2020 2020 2020 2020 2274 7970 6522 3a20          "type": 
+00004760: 2266 6c6f 6174 222c 0a20 2020 2020 2020  "float",.       
+00004770: 2020 2020 2020 2020 2020 2020 2022 6465               "de
+00004780: 7363 7269 7074 696f 6e22 3a20 2254 6865  scription": "The
+00004790: 2079 2d70 6f73 6974 696f 6e20 6f66 2074   y-position of t
+000047a0: 6865 2062 7562 626c 6520 7468 6174 2061  he bubble that a
+000047b0: 7070 6561 7265 6422 0a20 2020 2020 2020  ppeared".       
+000047c0: 2020 2020 2020 2020 207d 2c0a 2020 2020           },.    
+000047d0: 2020 2020 2020 2020 2020 2020 2270 6f73              "pos
+000047e0: 5a22 3a20 7b0a 2020 2020 2020 2020 2020  Z": {.          
+000047f0: 2020 2020 2020 2020 2020 2274 7970 6522            "type"
+00004800: 3a20 2266 6c6f 6174 222c 0a20 2020 2020  : "float",.     
+00004810: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00004820: 6465 7363 7269 7074 696f 6e22 3a20 2254  description": "T
+00004830: 6865 207a 2d70 6f73 6974 696f 6e20 6f66  he z-position of
+00004840: 2074 6865 2062 7562 626c 6520 7468 6174   the bubble that
+00004850: 2061 7070 6561 7265 6422 0a20 2020 2020   appeared".     
+00004860: 2020 2020 2020 2020 2020 207d 0a20 2020             }.   
+00004870: 2020 2020 2020 2020 207d 0a20 2020 2020           }.     
+00004880: 2020 207d 2c0a 2020 2020 2020 2020 2262     },.        "b
+00004890: 7562 626c 655f 6578 7069 7265 6422 3a20  ubble_expired": 
+000048a0: 7b0a 2020 2020 2020 2020 2020 2020 2264  {.            "d
+000048b0: 6573 6372 6970 7469 6f6e 223a 2022 4576  escription": "Ev
+000048c0: 656e 7420 7768 656e 2061 2062 7562 626c  ent when a bubbl
+000048d0: 6527 7320 706f 702d 6162 6c65 2074 696d  e's pop-able tim
+000048e0: 6520 656e 6473 2061 6e64 2074 6865 2062  e ends and the b
+000048f0: 7562 626c 6520 6469 7361 7070 6561 7273  ubble disappears
+00004900: 2e22 2c0a 2020 2020 2020 2020 2020 2020  .",.            
+00004910: 2265 7665 6e74 5f64 6174 6122 3a20 7b0a  "event_data": {.
+00004920: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004930: 226f 626a 6563 745f 6964 223a 207b 0a20  "object_id": {. 
+00004940: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004950: 2020 2022 7479 7065 223a 2022 7374 7222     "type": "str"
+00004960: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00004970: 2020 2020 2020 2264 6573 6372 6970 7469        "descripti
+00004980: 6f6e 223a 2022 5468 6520 6e61 6d65 206f  on": "The name o
+00004990: 6620 7468 6520 6275 6262 6c65 206f 626a  f the bubble obj
+000049a0: 6563 7420 7468 6174 2064 6973 6170 7065  ect that disappe
+000049b0: 6172 6564 220a 2020 2020 2020 2020 2020  ared".          
+000049c0: 2020 2020 2020 7d0a 2020 2020 2020 2020        }.        
+000049d0: 2020 2020 7d0a 2020 2020 2020 2020 7d2c      }.        },
+000049e0: 0a20 2020 2020 2020 2022 6567 675f 6861  .        "egg_ha
+000049f0: 7463 685f 696e 6469 6361 746f 725f 7570  tch_indicator_up
+00004a00: 6461 7465 6422 3a20 7b0a 2020 2020 2020  dated": {.      
+00004a10: 2020 2020 2020 2264 6573 6372 6970 7469        "descripti
+00004a20: 6f6e 223a 2022 4e4f 5420 5945 5420 444f  on": "NOT YET DO
+00004a30: 4355 4d45 4e54 4544 222c 0a20 2020 2020  CUMENTED",.     
+00004a40: 2020 2020 2020 2022 6576 656e 745f 6461         "event_da
+00004a50: 7461 223a 207b 0a20 2020 2020 2020 2020  ta": {.         
+00004a60: 2020 2020 2020 2022 7469 6d65 5f72 656d         "time_rem
+00004a70: 6169 6e69 6e67 223a 207b 0a20 2020 2020  aining": {.     
+00004a80: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00004a90: 7479 7065 223a 2022 666c 6f61 7422 2c0a  type": "float",.
+00004aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004ab0: 2020 2020 2264 6573 6372 6970 7469 6f6e      "description
+00004ac0: 223a 2022 5468 6520 7469 6d65 206c 6566  ": "The time lef
+00004ad0: 7420 756e 7469 6c20 7468 6520 6567 6720  t until the egg 
+00004ae0: 7769 6c6c 2068 6174 6368 220a 2020 2020  will hatch".    
+00004af0: 2020 2020 2020 2020 2020 2020 7d0a 2020              }.  
+00004b00: 2020 2020 2020 2020 2020 7d0a 2020 2020            }.    
+00004b10: 2020 2020 7d2c 0a20 2020 2020 2020 2022      },.        "
+00004b20: 6567 675f 6861 7463 6865 6422 3a20 7b0a  egg_hatched": {.
+00004b30: 2020 2020 2020 2020 2020 2020 2264 6573              "des
+00004b40: 6372 6970 7469 6f6e 223a 2022 4576 656e  cription": "Even
+00004b50: 7420 7768 656e 2074 6865 2065 6767 2068  t when the egg h
+00004b60: 6174 6368 6573 222c 0a20 2020 2020 2020  atches",.       
+00004b70: 2020 2020 2022 6576 656e 745f 6461 7461       "event_data
+00004b80: 223a 207b 7d0a 2020 2020 2020 2020 7d2c  ": {}.        },
+00004b90: 0a20 2020 2020 2020 2022 6567 675f 6c6f  .        "egg_lo
+00004ba0: 7374 223a 207b 0a20 2020 2020 2020 2020  st": {.         
+00004bb0: 2020 2022 6465 7363 7269 7074 696f 6e22     "description"
+00004bc0: 3a20 2245 7665 6e74 2077 6865 6e20 7468  : "Event when th
+00004bd0: 6520 706c 6179 6572 2773 2065 6767 2069  e player's egg i
+00004be0: 7320 7374 6f6c 656e 2062 7920 6120 736b  s stolen by a sk
+00004bf0: 7561 2e22 2c0a 2020 2020 2020 2020 2020  ua.",.          
+00004c00: 2020 2265 7665 6e74 5f64 6174 6122 3a20    "event_data": 
+00004c10: 7b0a 2020 2020 2020 2020 2020 2020 2020  {.              
+00004c20: 2020 226f 626a 6563 745f 6964 223a 207b    "object_id": {
+00004c30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00004c40: 2020 2020 2022 7479 7065 223a 2022 7374       "type": "st
+00004c50: 7222 2c0a 2020 2020 2020 2020 2020 2020  r",.            
+00004c60: 2020 2020 2020 2020 2264 6573 6372 6970          "descrip
+00004c70: 7469 6f6e 223a 2022 5468 6520 6e61 6d65  tion": "The name
+00004c80: 206f 6620 7468 6520 736b 7561 2074 6861   of the skua tha
+00004c90: 7420 7374 6f6c 6520 7468 6520 6567 6722  t stole the egg"
+00004ca0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00004cb0: 207d 0a20 2020 2020 2020 2020 2020 207d   }.            }
+00004cc0: 0a20 2020 2020 2020 207d 2c0a 2020 2020  .        },.    
+00004cd0: 2020 2020 2265 6767 5f72 6563 6f76 6572      "egg_recover
+00004ce0: 6564 223a 207b 0a20 2020 2020 2020 2020  ed": {.         
+00004cf0: 2020 2022 6465 7363 7269 7074 696f 6e22     "description"
+00004d00: 3a20 2245 7665 6e74 2077 6865 6e20 7468  : "Event when th
+00004d10: 6520 706c 6179 6572 2072 6563 6f76 6572  e player recover
+00004d20: 7320 7468 6520 6567 6720 6672 6f6d 2074  s the egg from t
+00004d30: 6865 2073 6b75 6173 2e22 2c0a 2020 2020  he skuas.",.    
+00004d40: 2020 2020 2020 2020 2265 7665 6e74 5f64          "event_d
+00004d50: 6174 6122 3a20 7b7d 0a20 2020 2020 2020  ata": {}.       
+00004d60: 207d 2c0a 2020 2020 2020 2020 226d 6174   },.        "mat
+00004d70: 696e 675f 6461 6e63 655f 696e 6469 6361  ing_dance_indica
+00004d80: 746f 725f 7570 6461 7465 6422 3a20 7b0a  tor_updated": {.
+00004d90: 2020 2020 2020 2020 2020 2020 2264 6573              "des
+00004da0: 6372 6970 7469 6f6e 223a 2022 4576 656e  cription": "Even
+00004db0: 7420 7768 656e 2061 2062 7562 626c 6520  t when a bubble 
+00004dc0: 6973 2070 6f70 7065 6420 616e 6420 7468  is popped and th
+00004dd0: 6520 696e 6469 6361 746f 7220 666f 7220  e indicator for 
+00004de0: 7072 6f67 7265 7373 2074 6f20 636f 6d70  progress to comp
+00004df0: 6c65 7469 6f6e 206f 6620 7468 6520 6d61  letion of the ma
+00004e00: 7469 6e67 2064 616e 6365 2075 7064 6174  ting dance updat
+00004e10: 6573 2e22 2c0a 2020 2020 2020 2020 2020  es.",.          
+00004e20: 2020 2265 7665 6e74 5f64 6174 6122 3a20    "event_data": 
+00004e30: 7b0a 2020 2020 2020 2020 2020 2020 2020  {.              
+00004e40: 2020 2270 6572 6365 6e74 5f66 756c 6c22    "percent_full"
+00004e50: 3a20 7b0a 2020 2020 2020 2020 2020 2020  : {.            
+00004e60: 2020 2020 2020 2020 2274 7970 6522 3a20          "type": 
+00004e70: 2269 6e74 222c 0a20 2020 2020 2020 2020  "int",.         
+00004e80: 2020 2020 2020 2020 2020 2022 6465 7363             "desc
+00004e90: 7269 7074 696f 6e22 3a20 2254 6865 206e  ription": "The n
+00004ea0: 6577 2070 6572 6365 6e74 2074 6f20 7768  ew percent to wh
+00004eb0: 6963 6820 7468 6520 6461 6e63 6520 636f  ich the dance co
+00004ec0: 6d70 6c65 7469 6f6e 2069 6e64 6963 6174  mpletion indicat
+00004ed0: 6f72 2069 7320 6669 6c6c 6564 220a 2020  or is filled".  
+00004ee0: 2020 2020 2020 2020 2020 2020 2020 7d0a                }.
+00004ef0: 2020 2020 2020 2020 2020 2020 7d0a 2020              }.  
+00004f00: 2020 2020 2020 7d2c 0a20 2020 2020 2020        },.       
+00004f10: 2022 6e65 7374 5f63 6f6d 706c 6574 6522   "nest_complete"
+00004f20: 3a20 7b0a 2020 2020 2020 2020 2020 2020  : {.            
+00004f30: 2264 6573 6372 6970 7469 6f6e 223a 2022  "description": "
+00004f40: 4576 656e 7420 7768 656e 2074 6865 2070  Event when the p
+00004f50: 6c61 7965 7220 636f 6d70 6c65 7465 7320  layer completes 
+00004f60: 7468 6520 6275 696c 6469 6e67 206f 6620  the building of 
+00004f70: 7468 6569 7220 6e65 7374 2e22 2c0a 2020  their nest.",.  
+00004f80: 2020 2020 2020 2020 2020 2265 7665 6e74            "event
+00004f90: 5f64 6174 6122 3a20 7b7d 0a20 2020 2020  _data": {}.     
+00004fa0: 2020 207d 2c0a 2020 2020 2020 2020 2270     },.        "p
+00004fb0: 656e 6775 696e 5f70 696e 5f66 656c 6c22  enguin_pin_fell"
+00004fc0: 3a20 7b0a 2020 2020 2020 2020 2020 2020  : {.            
+00004fd0: 2264 6573 6372 6970 7469 6f6e 223a 2022  "description": "
+00004fe0: 5768 656e 206f 6e65 206f 6620 7468 6520  When one of the 
+00004ff0: 7069 6e73 2066 656c 6c20 696e 2074 6865  pins fell in the
+00005000: 2062 6f77 6c69 6e67 2061 7265 612e 222c   bowling area.",
+00005010: 0a20 2020 2020 2020 2020 2020 2022 6576  .            "ev
+00005020: 656e 745f 6461 7461 223a 207b 7d0a 2020  ent_data": {}.  
+00005030: 2020 2020 2020 7d2c 0a20 2020 2020 2020        },.       
+00005040: 2022 736b 7561 5f73 7061 776e 223a 207b   "skua_spawn": {
+00005050: 0a20 2020 2020 2020 2020 2020 2022 6465  .            "de
+00005060: 7363 7269 7074 696f 6e22 3a20 2245 7665  scription": "Eve
+00005070: 6e74 2077 6865 6e20 6120 6e65 7720 736b  nt when a new sk
+00005080: 7561 2069 7320 6164 6465 6420 696e 2074  ua is added in t
+00005090: 6865 206e 6573 742f 6567 6720 6465 6665  he nest/egg defe
+000050a0: 6e73 6520 6d69 6e69 2d67 616d 652e 222c  nse mini-game.",
+000050b0: 0a20 2020 2020 2020 2020 2020 2022 6576  .            "ev
+000050c0: 656e 745f 6461 7461 223a 207b 0a20 2020  ent_data": {.   
+000050d0: 2020 2020 2020 2020 2020 2020 2022 6f62               "ob
+000050e0: 6a65 6374 5f69 6422 3a20 7b0a 2020 2020  ject_id": {.    
+000050f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005100: 2274 7970 6522 3a20 2273 7472 222c 0a20  "type": "str",. 
+00005110: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005120: 2020 2022 6465 7363 7269 7074 696f 6e22     "description"
+00005130: 3a20 2254 6865 206e 616d 6520 6f66 2074  : "The name of t
+00005140: 6865 2073 6b75 6120 6f62 6a65 6374 2074  he skua object t
+00005150: 6861 7420 6170 7065 6172 6564 220a 2020  hat appeared".  
+00005160: 2020 2020 2020 2020 2020 2020 2020 7d2c                },
+00005170: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00005180: 2022 706f 7358 223a 207b 0a20 2020 2020   "posX": {.     
+00005190: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+000051a0: 7479 7065 223a 2022 666c 6f61 7422 2c0a  type": "float",.
+000051b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000051c0: 2020 2020 2264 6573 6372 6970 7469 6f6e      "description
+000051d0: 223a 2022 5468 6520 782d 706f 7369 7469  ": "The x-positi
+000051e0: 6f6e 206f 6620 7468 6520 736b 7561 2074  on of the skua t
+000051f0: 6861 7420 6170 7065 6172 6564 220a 2020  hat appeared".  
+00005200: 2020 2020 2020 2020 2020 2020 2020 7d2c                },
+00005210: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00005220: 2022 706f 7359 223a 207b 0a20 2020 2020   "posY": {.     
+00005230: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00005240: 7479 7065 223a 2022 666c 6f61 7422 2c0a  type": "float",.
+00005250: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005260: 2020 2020 2264 6573 6372 6970 7469 6f6e      "description
+00005270: 223a 2022 5468 6520 792d 706f 7369 7469  ": "The y-positi
+00005280: 6f6e 206f 6620 7468 6520 736b 7561 2074  on of the skua t
+00005290: 6861 7420 6170 7065 6172 6564 220a 2020  hat appeared".  
+000052a0: 2020 2020 2020 2020 2020 2020 2020 7d2c                },
+000052b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000052c0: 2022 706f 735a 223a 207b 0a20 2020 2020   "posZ": {.     
+000052d0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+000052e0: 7479 7065 223a 2022 666c 6f61 7422 2c0a  type": "float",.
+000052f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005300: 2020 2020 2264 6573 6372 6970 7469 6f6e      "description
+00005310: 223a 2022 5468 6520 7a2d 706f 7369 7469  ": "The z-positi
+00005320: 6f6e 206f 6620 7468 6520 736b 7561 2074  on of the skua t
+00005330: 6861 7420 6170 7065 6172 6564 220a 2020  hat appeared".  
+00005340: 2020 2020 2020 2020 2020 2020 2020 7d0a                }.
+00005350: 2020 2020 2020 2020 2020 2020 7d0a 2020              }.  
+00005360: 2020 2020 2020 7d2c 0a20 2020 2020 2020        },.       
+00005370: 2022 736b 7561 5f6d 6f76 6522 3a20 7b0a   "skua_move": {.
+00005380: 2020 2020 2020 2020 2020 2020 2264 6573              "des
+00005390: 6372 6970 7469 6f6e 223a 2022 4576 656e  cription": "Even
+000053a0: 7420 7768 656e 2061 2073 6b75 6120 6d6f  t when a skua mo
+000053b0: 7665 7320 746f 2061 206e 6577 206c 6f63  ves to a new loc
+000053c0: 6174 696f 6e20 696e 2074 6865 206e 6573  ation in the nes
+000053d0: 742f 6567 6720 6465 6665 6e73 6520 6d69  t/egg defense mi
+000053e0: 6e69 2d67 616d 652e 222c 0a20 2020 2020  ni-game.",.     
+000053f0: 2020 2020 2020 2022 6576 656e 745f 6461         "event_da
+00005400: 7461 223a 207b 0a20 2020 2020 2020 2020  ta": {.         
+00005410: 2020 2020 2020 2022 6f62 6a65 6374 5f69         "object_i
+00005420: 6422 3a20 7b0a 2020 2020 2020 2020 2020  d": {.          
+00005430: 2020 2020 2020 2020 2020 2274 7970 6522            "type"
+00005440: 3a20 2273 7472 222c 0a20 2020 2020 2020  : "str",.       
+00005450: 2020 2020 2020 2020 2020 2020 2022 6465               "de
+00005460: 7363 7269 7074 696f 6e22 3a20 2254 6865  scription": "The
+00005470: 206e 616d 6520 6f66 2074 6865 2073 6b75   name of the sku
+00005480: 6120 6f62 6a65 6374 2074 6861 7420 6d6f  a object that mo
+00005490: 7665 6422 0a20 2020 2020 2020 2020 2020  ved".           
+000054a0: 2020 2020 207d 2c0a 2020 2020 2020 2020       },.        
+000054b0: 2020 2020 2020 2020 2266 726f 6d5f 706f          "from_po
+000054c0: 7369 7469 6f6e 5f78 223a 207b 0a20 2020  sition_x": {.   
+000054d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000054e0: 2022 7479 7065 223a 2022 666c 6f61 7422   "type": "float"
+000054f0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00005500: 2020 2020 2020 2264 6573 6372 6970 7469        "descripti
+00005510: 6f6e 223a 2022 5468 6520 696e 6974 6961  on": "The initia
+00005520: 6c20 782d 706f 7369 7469 6f6e 206f 6620  l x-position of 
+00005530: 7468 6520 736b 7561 2074 6861 7420 6d6f  the skua that mo
+00005540: 7665 6422 0a20 2020 2020 2020 2020 2020  ved".           
+00005550: 2020 2020 207d 2c0a 2020 2020 2020 2020       },.        
+00005560: 2020 2020 2020 2020 2266 726f 6d5f 706f          "from_po
+00005570: 7369 7469 6f6e 5f79 223a 207b 0a20 2020  sition_y": {.   
+00005580: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005590: 2022 7479 7065 223a 2022 666c 6f61 7422   "type": "float"
+000055a0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+000055b0: 2020 2020 2020 2264 6573 6372 6970 7469        "descripti
+000055c0: 6f6e 223a 2022 5468 6520 696e 6974 6961  on": "The initia
+000055d0: 6c20 792d 706f 7369 7469 6f6e 206f 6620  l y-position of 
+000055e0: 7468 6520 736b 7561 2074 6861 7420 6d6f  the skua that mo
+000055f0: 7665 6422 0a20 2020 2020 2020 2020 2020  ved".           
+00005600: 2020 2020 207d 2c0a 2020 2020 2020 2020       },.        
+00005610: 2020 2020 2020 2020 2266 726f 6d5f 706f          "from_po
+00005620: 7369 7469 6f6e 5f7a 223a 207b 0a20 2020  sition_z": {.   
+00005630: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005640: 2022 7479 7065 223a 2022 666c 6f61 7422   "type": "float"
+00005650: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00005660: 2020 2020 2020 2264 6573 6372 6970 7469        "descripti
+00005670: 6f6e 223a 2022 5468 6520 696e 6974 6961  on": "The initia
+00005680: 6c20 7a2d 706f 7369 7469 6f6e 206f 6620  l z-position of 
+00005690: 7468 6520 736b 7561 2074 6861 7420 6d6f  the skua that mo
+000056a0: 7665 6422 0a20 2020 2020 2020 2020 2020  ved".           
+000056b0: 2020 2020 207d 2c0a 2020 2020 2020 2020       },.        
+000056c0: 2020 2020 2020 2020 2274 6f5f 706f 7369          "to_posi
+000056d0: 7469 6f6e 5f78 223a 207b 0a20 2020 2020  tion_x": {.     
+000056e0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+000056f0: 7479 7065 223a 2022 666c 6f61 7422 2c0a  type": "float",.
+00005700: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005710: 2020 2020 2264 6573 6372 6970 7469 6f6e      "description
+00005720: 223a 2022 5468 6520 6e65 7720 782d 706f  ": "The new x-po
+00005730: 7369 7469 6f6e 206f 6620 7468 6520 736b  sition of the sk
+00005740: 7561 2074 6861 7420 6d6f 7665 6422 0a20  ua that moved". 
+00005750: 2020 2020 2020 2020 2020 2020 2020 207d                 }
+00005760: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00005770: 2020 2274 6f5f 706f 7369 7469 6f6e 5f79    "to_position_y
+00005780: 223a 207b 0a20 2020 2020 2020 2020 2020  ": {.           
+00005790: 2020 2020 2020 2020 2022 7479 7065 223a           "type":
+000057a0: 2022 666c 6f61 7422 2c0a 2020 2020 2020   "float",.      
+000057b0: 2020 2020 2020 2020 2020 2020 2020 2264                "d
+000057c0: 6573 6372 6970 7469 6f6e 223a 2022 5468  escription": "Th
+000057d0: 6520 6e65 7720 792d 706f 7369 7469 6f6e  e new y-position
+000057e0: 206f 6620 7468 6520 736b 7561 2074 6861   of the skua tha
+000057f0: 7420 6d6f 7665 6422 0a20 2020 2020 2020  t moved".       
+00005800: 2020 2020 2020 2020 207d 2c0a 2020 2020           },.    
+00005810: 2020 2020 2020 2020 2020 2020 2274 6f5f              "to_
+00005820: 706f 7369 7469 6f6e 5f7a 223a 207b 0a20  position_z": {. 
+00005830: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005840: 2020 2022 7479 7065 223a 2022 666c 6f61     "type": "floa
+00005850: 7422 2c0a 2020 2020 2020 2020 2020 2020  t",.            
+00005860: 2020 2020 2020 2020 2264 6573 6372 6970          "descrip
+00005870: 7469 6f6e 223a 2022 5468 6520 6e65 7720  tion": "The new 
+00005880: 7a2d 706f 7369 7469 6f6e 206f 6620 7468  z-position of th
+00005890: 6520 736b 7561 2074 6861 7420 6d6f 7665  e skua that move
+000058a0: 6422 0a20 2020 2020 2020 2020 2020 2020  d".             
+000058b0: 2020 207d 0a20 2020 2020 2020 2020 2020     }.           
+000058c0: 207d 0a20 2020 2020 2020 207d 2c0a 2020   }.        },.  
+000058d0: 2020 2020 2020 2265 6e74 6572 5f72 6567        "enter_reg
+000058e0: 696f 6e22 3a20 7b0a 2020 2020 2020 2020  ion": {.        
+000058f0: 2020 2020 2264 6573 6372 6970 7469 6f6e      "description
+00005900: 223a 2022 4576 656e 7420 7768 656e 2074  ": "Event when t
+00005910: 6865 2070 6c61 7965 7220 6d6f 7665 7320  he player moves 
+00005920: 696e 746f 206f 6e65 206f 6620 7468 6520  into one of the 
+00005930: 7265 6769 6f6e 7320 636f 6e74 6169 6e69  regions containi
+00005940: 6e67 2061 206d 696e 692d 6761 6d65 206f  ng a mini-game o
+00005950: 7220 6f74 6865 7220 6665 6174 7572 652e  r other feature.
+00005960: 222c 0a20 2020 2020 2020 2020 2020 2022  ",.            "
+00005970: 6576 656e 745f 6461 7461 223a 207b 0a20  event_data": {. 
+00005980: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00005990: 7265 6769 6f6e 5f6e 616d 6522 3a20 7b0a  region_name": {.
+000059a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000059b0: 2020 2020 2274 7970 6522 3a20 2273 7472      "type": "str
+000059c0: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
+000059d0: 2020 2020 2020 2022 6465 7363 7269 7074         "descript
+000059e0: 696f 6e22 3a20 2254 6865 206e 616d 6520  ion": "The name 
+000059f0: 6f66 2074 6865 2072 6567 696f 6e20 7468  of the region th
+00005a00: 6520 706c 6179 6572 2065 6e74 6572 6564  e player entered
+00005a10: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
+00005a20: 2020 7d0a 2020 2020 2020 2020 2020 2020    }.            
+00005a30: 7d0a 2020 2020 2020 2020 7d2c 0a20 2020  }.        },.   
+00005a40: 2020 2020 2022 6578 6974 5f72 6567 696f       "exit_regio
+00005a50: 6e22 3a20 7b0a 2020 2020 2020 2020 2020  n": {.          
+00005a60: 2020 2264 6573 6372 6970 7469 6f6e 223a    "description":
+00005a70: 2022 4576 656e 7420 7768 656e 2061 206d   "Event when a m
+00005a80: 6f76 6573 206f 7574 206f 6620 6f6e 6520  oves out of one 
+00005a90: 6f66 2074 6865 2072 6567 696f 6e73 2063  of the regions c
+00005aa0: 6f6e 7461 696e 696e 6720 6120 6d69 6e69  ontaining a mini
+00005ab0: 2d67 616d 6520 6f72 206f 7468 6572 2066  -game or other f
+00005ac0: 6561 7475 7265 2e22 2c0a 2020 2020 2020  eature.",.      
+00005ad0: 2020 2020 2020 2265 7665 6e74 5f64 6174        "event_dat
+00005ae0: 6122 3a20 7b0a 2020 2020 2020 2020 2020  a": {.          
+00005af0: 2020 2020 2020 2272 6567 696f 6e5f 6e61        "region_na
+00005b00: 6d65 223a 207b 0a20 2020 2020 2020 2020  me": {.         
+00005b10: 2020 2020 2020 2020 2020 2022 7479 7065             "type
+00005b20: 223a 2022 7374 7222 2c0a 2020 2020 2020  ": "str",.      
+00005b30: 2020 2020 2020 2020 2020 2020 2020 2264                "d
+00005b40: 6573 6372 6970 7469 6f6e 223a 2022 5468  escription": "Th
+00005b50: 6520 6e61 6d65 206f 6620 7468 6520 7265  e name of the re
+00005b60: 6769 6f6e 2074 6865 2070 6c61 7965 7220  gion the player 
+00005b70: 6c65 6674 220a 2020 2020 2020 2020 2020  left".          
+00005b80: 2020 2020 2020 7d0a 2020 2020 2020 2020        }.        
+00005b90: 2020 2020 7d0a 2020 2020 2020 2020 7d2c      }.        },
+00005ba0: 0a20 2020 2020 2020 2022 6163 7469 7669  .        "activi
+00005bb0: 7479 5f62 6567 696e 223a 207b 0a20 2020  ty_begin": {.   
+00005bc0: 2020 2020 2020 2020 2022 6465 7363 7269           "descri
+00005bd0: 7074 696f 6e22 3a20 2245 7665 6e74 2077  ption": "Event w
+00005be0: 6865 6e20 7468 6520 706c 6179 6572 2062  hen the player b
+00005bf0: 6567 696e 7320 746f 2065 6e67 6167 6520  egins to engage 
+00005c00: 7769 7468 2061 206d 696e 692d 6761 6d65  with a mini-game
+00005c10: 2061 6374 6976 6974 792e 2045 7861 6374   activity. Exact
+00005c20: 2074 7269 6767 6572 2076 6172 6965 7320   trigger varies 
+00005c30: 6279 2061 6374 6976 6974 792e 222c 0a20  by activity.",. 
+00005c40: 2020 2020 2020 2020 2020 2022 6576 656e             "even
+00005c50: 745f 6461 7461 223a 207b 0a20 2020 2020  t_data": {.     
+00005c60: 2020 2020 2020 2020 2020 2022 6163 7469             "acti
+00005c70: 7669 7479 5f6e 616d 6522 3a20 7b0a 2020  vity_name": {.  
+00005c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005c90: 2020 2274 7970 6522 3a20 2241 6374 6976    "type": "Activ
+00005ca0: 6974 7922 2c0a 2020 2020 2020 2020 2020  ity",.          
+00005cb0: 2020 2020 2020 2020 2020 2264 6573 6372            "descr
+00005cc0: 6970 7469 6f6e 223a 2022 5468 6520 6e61  iption": "The na
+00005cd0: 6d65 206f 6620 7468 6520 6d69 6e69 2d67  me of the mini-g
+00005ce0: 616d 652f 6163 7469 7669 7479 2077 6974  ame/activity wit
+00005cf0: 6820 7768 6963 6820 7468 6520 706c 6179  h which the play
+00005d00: 6572 2062 6567 616e 2074 6f20 656e 6761  er began to enga
+00005d10: 6765 220a 2020 2020 2020 2020 2020 2020  ge".            
+00005d20: 2020 2020 7d0a 2020 2020 2020 2020 2020      }.          
+00005d30: 2020 7d0a 2020 2020 2020 2020 7d2c 0a20    }.        },. 
+00005d40: 2020 2020 2020 2022 6163 7469 7669 7479         "activity
+00005d50: 5f65 6e64 223a 207b 0a20 2020 2020 2020  _end": {.       
+00005d60: 2020 2020 2022 6465 7363 7269 7074 696f       "descriptio
+00005d70: 6e22 3a20 2245 7665 6e74 2077 6865 6e20  n": "Event when 
+00005d80: 7468 6520 706c 6179 6572 2063 6f6d 706c  the player compl
+00005d90: 6574 6573 2061 206d 696e 692d 6761 6d65  etes a mini-game
+00005da0: 2061 6374 6976 6974 792e 2045 7861 6374   activity. Exact
+00005db0: 2074 7269 6767 6572 2076 6172 6965 7320   trigger varies 
+00005dc0: 6279 2061 6374 6976 6974 792e 222c 0a20  by activity.",. 
+00005dd0: 2020 2020 2020 2020 2020 2022 6576 656e             "even
+00005de0: 745f 6461 7461 223a 207b 0a20 2020 2020  t_data": {.     
+00005df0: 2020 2020 2020 2020 2020 2022 6163 7469             "acti
+00005e00: 7669 7479 5f6e 616d 6522 3a20 7b0a 2020  vity_name": {.  
+00005e10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005e20: 2020 2274 7970 6522 3a20 2241 6374 6976    "type": "Activ
+00005e30: 6974 7922 2c0a 2020 2020 2020 2020 2020  ity",.          
+00005e40: 2020 2020 2020 2020 2020 2264 6573 6372            "descr
+00005e50: 6970 7469 6f6e 223a 2022 5468 6520 6e61  iption": "The na
+00005e60: 6d65 206f 6620 7468 6520 6d69 6e69 2d67  me of the mini-g
+00005e70: 616d 652f 6163 7469 7669 7479 2074 6865  ame/activity the
+00005e80: 2070 6c61 7965 7220 636f 6d70 6c65 7465   player complete
+00005e90: 642e 220a 2020 2020 2020 2020 2020 2020  d.".            
+00005ea0: 2020 2020 7d0a 2020 2020 2020 2020 2020      }.          
+00005eb0: 2020 7d0a 2020 2020 2020 2020 7d2c 0a20    }.        },. 
+00005ec0: 2020 2020 2020 2022 676c 6f62 616c 5f74         "global_t
+00005ed0: 696d 6572 5f62 6567 696e 223a 207b 0a20  imer_begin": {. 
+00005ee0: 2020 2020 2020 2020 2020 2022 6465 7363             "desc
+00005ef0: 7269 7074 696f 6e22 3a20 224e 4f54 2059  ription": "NOT Y
+00005f00: 4554 2044 4f43 554d 454e 5445 4422 2c0a  ET DOCUMENTED",.
+00005f10: 2020 2020 2020 2020 2020 2020 2265 7665              "eve
+00005f20: 6e74 5f64 6174 6122 3a20 7b0a 2020 2020  nt_data": {.    
+00005f30: 2020 2020 2020 2020 2020 2020 2274 696d              "tim
+00005f40: 655f 7265 6d61 696e 696e 6722 3a20 7b0a  e_remaining": {.
+00005f50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005f60: 2020 2020 2274 7970 6522 3a20 2269 6e74      "type": "int
+00005f70: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
+00005f80: 2020 2020 2020 2022 6465 7363 7269 7074         "descript
+00005f90: 696f 6e22 3a20 2254 6865 206c 6566 7420  ion": "The left 
+00005fa0: 6f6e 2074 6865 2067 6c6f 6261 6c20 7469  on the global ti
+00005fb0: 6d65 7222 0a20 2020 2020 2020 2020 2020  mer".           
+00005fc0: 2020 2020 207d 0a20 2020 2020 2020 2020       }.         
+00005fd0: 2020 207d 0a20 2020 2020 2020 207d 2c0a     }.        },.
+00005fe0: 2020 2020 2020 2020 2267 6c6f 6261 6c5f          "global_
+00005ff0: 7469 6d65 725f 7061 7573 6522 3a20 7b0a  timer_pause": {.
+00006000: 2020 2020 2020 2020 2020 2020 2264 6573              "des
+00006010: 6372 6970 7469 6f6e 223a 2022 4e4f 5420  cription": "NOT 
+00006020: 5945 5420 444f 4355 4d45 4e54 4544 222c  YET DOCUMENTED",
+00006030: 0a20 2020 2020 2020 2020 2020 2022 6576  .            "ev
+00006040: 656e 745f 6461 7461 223a 207b 0a20 2020  ent_data": {.   
+00006050: 2020 2020 2020 2020 2020 2020 2022 6461               "da
+00006060: 7461 223a 2022 4e4f 5420 5945 5420 444f  ta": "NOT YET DO
+00006070: 4355 4d45 4e54 4544 220a 2020 2020 2020  CUMENTED".      
+00006080: 2020 2020 2020 7d0a 2020 2020 2020 2020        }.        
+00006090: 7d2c 0a20 2020 2020 2020 2022 676c 6f62  },.        "glob
+000060a0: 616c 5f74 696d 6572 5f65 7870 6972 6564  al_timer_expired
+000060b0: 223a 207b 0a20 2020 2020 2020 2020 2020  ": {.           
+000060c0: 2022 6465 7363 7269 7074 696f 6e22 3a20   "description": 
+000060d0: 224e 4f54 2059 4554 2044 4f43 554d 454e  "NOT YET DOCUMEN
+000060e0: 5445 4422 2c0a 2020 2020 2020 2020 2020  TED",.          
+000060f0: 2020 2265 7665 6e74 5f64 6174 6122 3a20    "event_data": 
+00006100: 7b0a 2020 2020 2020 2020 2020 2020 2020  {.              
+00006110: 2020 2264 6174 6122 3a20 224e 4f54 2059    "data": "NOT Y
+00006120: 4554 2044 4f43 554d 454e 5445 4422 0a20  ET DOCUMENTED". 
+00006130: 2020 2020 2020 2020 2020 207d 0a20 2020             }.   
+00006140: 2020 2020 207d 0a20 2020 207d 2c0a 2020       }.    },.  
+00006150: 2020 2264 6574 6563 746f 7273 223a 207b    "detectors": {
+00006160: 0a20 2020 2020 2020 2022 7065 725f 636f  .        "per_co
+00006170: 756e 7422 3a20 7b0a 2020 2020 2020 2020  unt": {.        
+00006180: 2020 2020 2252 6567 696f 6e45 6e74 6572      "RegionEnter
+00006190: 223a 207b 0a20 2020 2020 2020 2020 2020  ": {.           
+000061a0: 2020 2020 2022 7479 7065 223a 2022 5265       "type": "Re
+000061b0: 6769 6f6e 456e 7465 7222 2c0a 2020 2020  gionEnter",.    
+000061c0: 2020 2020 2020 2020 2020 2020 2265 6e61              "ena
+000061d0: 626c 6564 223a 2074 7275 652c 0a20 2020  bled": true,.   
+000061e0: 2020 2020 2020 2020 2020 2020 2022 6465               "de
+000061f0: 7363 7269 7074 696f 6e22 3a20 2254 7269  scription": "Tri
+00006200: 6767 6572 7320 616e 2065 7665 6e74 2077  ggers an event w
+00006210: 6865 6e20 6120 706c 6179 6572 2065 6e74  hen a player ent
+00006220: 6572 2061 2072 6567 696f 6e22 0a20 2020  er a region".   
+00006230: 2020 2020 2020 2020 207d 2c0a 2020 2020           },.    
+00006240: 2020 2020 2020 2020 2252 6567 696f 6e45          "RegionE
+00006250: 7869 7422 3a20 7b0a 2020 2020 2020 2020  xit": {.        
+00006260: 2020 2020 2020 2020 2274 7970 6522 3a20          "type": 
+00006270: 2252 6567 696f 6e45 7869 7422 2c0a 2020  "RegionExit",.  
+00006280: 2020 2020 2020 2020 2020 2020 2020 2265                "e
+00006290: 6e61 626c 6564 223a 2074 7275 652c 0a20  nabled": true,. 
+000062a0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+000062b0: 6465 7363 7269 7074 696f 6e22 3a20 2254  description": "T
+000062c0: 7269 6767 6572 7320 616e 2065 7665 6e74  riggers an event
+000062d0: 2077 6865 6e20 6120 706c 6179 6572 2065   when a player e
+000062e0: 7869 7420 6120 7265 6769 6f6e 220a 2020  xit a region".  
+000062f0: 2020 2020 2020 2020 2020 7d0a 2020 2020            }.    
+00006300: 2020 2020 7d2c 0a20 2020 2020 2020 2022      },.        "
+00006310: 6167 6772 6567 6174 6522 3a20 7b7d 0a20  aggregate": {}. 
+00006320: 2020 207d 2c0a 2020 2020 2266 6561 7475     },.    "featu
+00006330: 7265 7322 3a20 7b0a 2020 2020 2020 2020  res": {.        
+00006340: 2270 6572 5f63 6f75 6e74 223a 207b 0a20  "per_count": {. 
+00006350: 2020 2020 2020 2020 2020 2022 5265 6769             "Regi
+00006360: 6f6e 4475 7261 7469 6f6e 223a 207b 0a20  onDuration": {. 
+00006370: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00006380: 7479 7065 223a 2022 5265 6769 6f6e 4475  type": "RegionDu
+00006390: 7261 7469 6f6e 222c 0a20 2020 2020 2020  ration",.       
+000063a0: 2020 2020 2020 2020 2022 656e 6162 6c65           "enable
+000063b0: 6422 3a20 7472 7565 2c0a 2020 2020 2020  d": true,.      
+000063c0: 2020 2020 2020 2020 2020 2263 6f75 6e74            "count
+000063d0: 223a 2031 312c 0a20 2020 2020 2020 2020  ": 11,.         
+000063e0: 2020 2020 2020 2022 7072 6566 6978 223a         "prefix":
+000063f0: 2022 7265 6769 6f6e 222c 0a20 2020 2020   "region",.     
+00006400: 2020 2020 2020 2020 2020 2022 6465 7363             "desc
+00006410: 7269 7074 696f 6e22 3a20 2254 6865 2064  ription": "The d
+00006420: 7572 6174 696f 6e20 6f66 2074 696d 6520  uration of time 
+00006430: 6120 706c 6179 6572 2070 6c61 7965 6420  a player played 
+00006440: 696e 2061 2067 6976 656e 2072 6567 696f  in a given regio
+00006450: 6e20 6f66 2074 6865 2067 616d 652e 222c  n of the game.",
+00006460: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00006470: 2022 7265 7475 726e 5f74 7970 6522 3a20   "return_type": 
+00006480: 2274 696d 6564 656c 7461 220a 2020 2020  "timedelta".    
+00006490: 2020 2020 2020 2020 7d2c 0a20 2020 2020          },.     
+000064a0: 2020 2020 2020 2022 5761 6464 6c65 5065         "WaddlePe
+000064b0: 7252 6567 696f 6e22 3a20 7b0a 2020 2020  rRegion": {.    
+000064c0: 2020 2020 2020 2020 2020 2020 2274 7970              "typ
+000064d0: 6522 3a20 2257 6164 646c 6550 6572 5265  e": "WaddlePerRe
+000064e0: 6769 6f6e 222c 0a20 2020 2020 2020 2020  gion",.         
+000064f0: 2020 2020 2020 2022 656e 6162 6c65 6422         "enabled"
+00006500: 3a20 7472 7565 2c0a 2020 2020 2020 2020  : true,.        
+00006510: 2020 2020 2020 2020 2263 6f75 6e74 223a          "count":
+00006520: 2031 312c 0a20 2020 2020 2020 2020 2020   11,.           
+00006530: 2020 2020 2022 7072 6566 6978 223a 2022       "prefix": "
+00006540: 7265 6769 6f6e 222c 0a20 2020 2020 2020  region",.       
+00006550: 2020 2020 2020 2020 2022 6465 7363 7269           "descri
+00006560: 7074 696f 6e22 3a20 2254 6865 206e 756d  ption": "The num
+00006570: 6265 7220 6f66 2074 696d 6573 2061 2070  ber of times a p
+00006580: 6c61 7965 7220 7761 6464 6c65 6420 696e  layer waddled in
+00006590: 2061 2067 6976 656e 2072 6567 696f 6e20   a given region 
+000065a0: 6f66 2074 6865 2067 616d 652e 222c 0a20  of the game.",. 
+000065b0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+000065c0: 7265 7475 726e 5f74 7970 6522 3a20 2269  return_type": "i
+000065d0: 6e74 220a 2020 2020 2020 2020 2020 2020  nt".            
+000065e0: 7d0a 2020 2020 2020 2020 7d2c 0a20 2020  }.        },.   
+000065f0: 2020 2020 2022 6167 6772 6567 6174 6522       "aggregate"
+00006600: 3a20 7b0a 2020 2020 2020 2020 2020 2020  : {.            
+00006610: 2247 617a 6543 6f75 6e74 223a 207b 0a20  "GazeCount": {. 
+00006620: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00006630: 7479 7065 223a 2022 4761 7a65 436f 756e  type": "GazeCoun
+00006640: 7422 2c0a 2020 2020 2020 2020 2020 2020  t",.            
+00006650: 2020 2020 2265 6e61 626c 6564 223a 2074      "enabled": t
+00006660: 7275 652c 0a20 2020 2020 2020 2020 2020  rue,.           
+00006670: 2020 2020 2022 6465 7363 7269 7074 696f       "descriptio
+00006680: 6e22 3a20 2254 6865 206e 756d 6265 7220  n": "The number 
+00006690: 6f66 2074 696d 6573 2061 2070 6c61 7965  of times a playe
+000066a0: 7220 7761 6464 6c65 6420 696e 2061 2067  r waddled in a g
+000066b0: 6976 656e 2072 6567 696f 6e20 6f66 2074  iven region of t
+000066c0: 6865 2067 616d 652e 222c 0a20 2020 2020  he game.",.     
+000066d0: 2020 2020 2020 2020 2020 2022 7265 7475             "retu
+000066e0: 726e 5f74 7970 6522 3a20 2269 6e74 220a  rn_type": "int".
+000066f0: 2020 2020 2020 2020 2020 2020 7d2c 0a20              },. 
+00006700: 2020 2020 2020 2020 2020 2022 5069 636b             "Pick
+00006710: 7570 526f 636b 436f 756e 7422 3a20 7b0a  upRockCount": {.
+00006720: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006730: 2274 7970 6522 3a20 2250 6963 6b75 7052  "type": "PickupR
+00006740: 6f63 6b43 6f75 6e74 222c 0a20 2020 2020  ockCount",.     
+00006750: 2020 2020 2020 2020 2020 2022 656e 6162             "enab
+00006760: 6c65 6422 3a20 7472 7565 2c0a 2020 2020  led": true,.    
+00006770: 2020 2020 2020 2020 2020 2020 2264 6573              "des
+00006780: 6372 6970 7469 6f6e 223a 2022 5468 6520  cription": "The 
+00006790: 6475 7261 7469 6f6e 2065 6163 6820 7365  duration each se
+000067a0: 7373 696f 6e20 746f 6f6b 2e22 2c0a 2020  ssion took.",.  
+000067b0: 2020 2020 2020 2020 2020 2020 2020 2272                "r
+000067c0: 6574 7572 6e5f 7479 7065 223a 2022 696e  eturn_type": "in
+000067d0: 7422 0a20 2020 2020 2020 2020 2020 207d  t".            }
+000067e0: 2c0a 2020 2020 2020 2020 2020 2020 2250  ,.            "P
+000067f0: 6c61 7965 7257 6164 646c 6543 6f75 6e74  layerWaddleCount
+00006800: 223a 207b 0a20 2020 2020 2020 2020 2020  ": {.           
+00006810: 2020 2020 2022 7479 7065 223a 2022 506c       "type": "Pl
+00006820: 6179 6572 5761 6464 6c65 436f 756e 7422  ayerWaddleCount"
+00006830: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00006840: 2020 2265 6e61 626c 6564 223a 2074 7275    "enabled": tru
+00006850: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
+00006860: 2020 2022 6465 7363 7269 7074 696f 6e22     "description"
+00006870: 3a20 2254 6865 206e 756d 6265 7220 6f66  : "The number of
+00006880: 2074 696d 6573 2061 2070 6c61 7965 7220   times a player 
+00006890: 7761 6464 6c65 642e 222c 0a20 2020 2020  waddled.",.     
+000068a0: 2020 2020 2020 2020 2020 2022 7265 7475             "retu
+000068b0: 726e 5f74 7970 6522 3a20 2269 6e74 220a  rn_type": "int".
+000068c0: 2020 2020 2020 2020 2020 2020 7d2c 0a20              },. 
+000068d0: 2020 2020 2020 2020 2020 2022 5365 7373             "Sess
+000068e0: 696f 6e44 7572 6174 696f 6e22 3a20 7b0a  ionDuration": {.
+000068f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006900: 2274 7970 6522 3a20 2253 6573 7369 6f6e  "type": "Session
+00006910: 4475 7261 7469 6f6e 222c 0a20 2020 2020  Duration",.     
+00006920: 2020 2020 2020 2020 2020 2022 656e 6162             "enab
+00006930: 6c65 6422 3a20 7472 7565 2c0a 2020 2020  led": true,.    
+00006940: 2020 2020 2020 2020 2020 2020 2264 6573              "des
+00006950: 6372 6970 7469 6f6e 223a 2022 5468 6520  cription": "The 
+00006960: 6475 7261 7469 6f6e 2065 6163 6820 7365  duration each se
+00006970: 7373 696f 6e20 746f 6f6b 2e22 2c0a 2020  ssion took.",.  
+00006980: 2020 2020 2020 2020 2020 2020 2020 2272                "r
+00006990: 6574 7572 6e5f 7479 7065 223a 2022 7469  eturn_type": "ti
+000069a0: 6d65 6465 6c74 6122 0a20 2020 2020 2020  medelta".       
+000069b0: 2020 2020 207d 2c0a 2020 2020 2020 2020       },.        
+000069c0: 2020 2020 2247 617a 6544 7572 6174 696f      "GazeDuratio
+000069d0: 6e22 3a20 7b0a 2020 2020 2020 2020 2020  n": {.          
+000069e0: 2020 2020 2020 2274 7970 6522 3a20 2247        "type": "G
+000069f0: 617a 6544 7572 6174 696f 6e22 2c0a 2020  azeDuration",.  
+00006a00: 2020 2020 2020 2020 2020 2020 2020 2265                "e
+00006a10: 6e61 626c 6564 223a 2074 7275 652c 0a20  nabled": true,. 
+00006a20: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00006a30: 6465 7363 7269 7074 696f 6e22 3a20 2248  description": "H
+00006a40: 6f77 206c 6f6e 6720 6761 7a65 2065 7665  ow long gaze eve
+00006a50: 6e74 206c 6173 7420 666f 722e 222c 0a20  nt last for.",. 
+00006a60: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00006a70: 7265 7475 726e 5f74 7970 6522 3a20 2274  return_type": "t
+00006a80: 696d 6564 656c 7461 220a 2020 2020 2020  imedelta".      
+00006a90: 2020 2020 2020 7d2c 0a20 2020 2020 2020        },.       
+00006aa0: 2020 2020 2022 5265 6769 6f6e 456e 7465       "RegionEnte
+00006ab0: 7243 6f75 6e74 223a 207b 0a20 2020 2020  rCount": {.     
+00006ac0: 2020 2020 2020 2020 2020 2022 7479 7065             "type
+00006ad0: 223a 2022 5265 6769 6f6e 456e 7465 7243  ": "RegionEnterC
+00006ae0: 6f75 6e74 222c 0a20 2020 2020 2020 2020  ount",.         
+00006af0: 2020 2020 2020 2022 656e 6162 6c65 6422         "enabled"
+00006b00: 3a20 6661 6c73 652c 0a20 2020 2020 2020  : false,.       
+00006b10: 2020 2020 2020 2020 2022 6465 7363 7269           "descri
+00006b20: 7074 696f 6e22 3a20 2254 6865 206e 756d  ption": "The num
+00006b30: 6265 7220 6f66 2074 696d 6573 2061 2070  ber of times a p
+00006b40: 6c61 7965 7220 656e 7465 7264 2066 6f72  layer enterd for
+00006b50: 2061 2067 6976 656e 2072 6567 696f 6e20   a given region 
+00006b60: 6f66 2074 6865 2067 616d 652e 222c 0a20  of the game.",. 
+00006b70: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00006b80: 7265 7475 726e 5f74 7970 6522 3a20 2269  return_type": "i
+00006b90: 6e74 220a 2020 2020 2020 2020 2020 2020  nt".            
+00006ba0: 7d2c 0a20 2020 2020 2020 2020 2020 2022  },.            "
+00006bb0: 4163 7469 7669 7479 436f 6d70 6c65 7465  ActivityComplete
+00006bc0: 6422 3a20 7b0a 2020 2020 2020 2020 2020  d": {.          
+00006bd0: 2020 2020 2020 2274 7970 6522 3a20 2241        "type": "A
+00006be0: 6374 6976 6974 7943 6f6d 706c 6574 6564  ctivityCompleted
+00006bf0: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
+00006c00: 2020 2022 656e 6162 6c65 6422 3a20 7472     "enabled": tr
+00006c10: 7565 2c0a 2020 2020 2020 2020 2020 2020  ue,.            
+00006c20: 2020 2020 2264 6573 6372 6970 7469 6f6e      "description
+00006c30: 223a 2022 5468 6520 6163 7469 7669 7469  ": "The activiti
+00006c40: 6573 2063 6f6d 706c 6574 6564 2069 6e20  es completed in 
+00006c50: 6120 6769 7665 6e20 7365 7373 696f 6e2e  a given session.
+00006c60: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
+00006c70: 2020 2022 7265 7475 726e 5f74 7970 6522     "return_type"
+00006c80: 3a20 2269 6e74 220a 2020 2020 2020 2020  : "int".        
+00006c90: 2020 2020 7d2c 0a20 2020 2020 2020 2020      },.         
+00006ca0: 2020 2022 4163 7469 7669 7479 4475 7261     "ActivityDura
+00006cb0: 7469 6f6e 223a 207b 0a20 2020 2020 2020  tion": {.       
+00006cc0: 2020 2020 2020 2020 2022 7479 7065 223a           "type":
+00006cd0: 2022 4163 7469 7669 7479 4475 7261 7469   "ActivityDurati
+00006ce0: 6f6e 222c 0a20 2020 2020 2020 2020 2020  on",.           
+00006cf0: 2020 2020 2022 656e 6162 6c65 6422 3a20       "enabled": 
+00006d00: 7472 7565 2c0a 2020 2020 2020 2020 2020  true,.          
+00006d10: 2020 2020 2020 2264 6573 6372 6970 7469        "descripti
+00006d20: 6f6e 223a 2022 486f 7720 6c6f 6e67 2061  on": "How long a
+00006d30: 6374 6976 6974 7920 6c61 7374 2066 6f72  ctivity last for
+00006d40: 2e22 2c0a 2020 2020 2020 2020 2020 2020  .",.            
+00006d50: 2020 2020 2272 6574 7572 6e5f 7479 7065      "return_type
+00006d60: 223a 2022 696e 7422 0a20 2020 2020 2020  ": "int".       
+00006d70: 2020 2020 207d 2c0a 2020 2020 2020 2020       },.        
+00006d80: 2020 2020 2252 6567 696f 6e73 456e 636f      "RegionsEnco
+00006d90: 756e 7465 7265 6422 3a20 7b0a 2020 2020  untered": {.    
+00006da0: 2020 2020 2020 2020 2020 2020 2274 7970              "typ
+00006db0: 6522 3a20 2252 6567 696f 6e73 456e 636f  e": "RegionsEnco
+00006dc0: 756e 7465 7265 6422 2c0a 2020 2020 2020  untered",.      
+00006dd0: 2020 2020 2020 2020 2020 2265 6e61 626c            "enabl
+00006de0: 6564 223a 2074 7275 652c 0a20 2020 2020  ed": true,.     
+00006df0: 2020 2020 2020 2020 2020 2022 6465 7363             "desc
+00006e00: 7269 7074 696f 6e22 3a20 2254 6865 2072  ription": "The r
+00006e10: 6567 696f 6e73 2065 6e74 6572 6564 2069  egions entered i
+00006e20: 6e20 6120 6769 7665 6e20 7365 7373 696f  n a given sessio
+00006e30: 6e2e 222c 0a20 2020 2020 2020 2020 2020  n.",.           
+00006e40: 2020 2020 2022 7265 7475 726e 5f74 7970       "return_typ
+00006e50: 6522 3a20 2269 6e74 220a 2020 2020 2020  e": "int".      
+00006e60: 2020 2020 2020 7d0a 2020 2020 2020 2020        }.        
+00006e70: 7d0a 2020 2020 7d2c 0a20 2020 2022 636f  }.    },.    "co
+00006e80: 6e66 6967 223a 207b 0a20 2020 2020 2020  nfig": {.       
+00006e90: 2022 5355 5050 4f52 5445 445f 5645 5253   "SUPPORTED_VERS
+00006ea0: 223a 205b 0a20 2020 2020 2020 2020 2020  ": [.           
+00006eb0: 2031 0a20 2020 2020 2020 205d 0a20 2020   1.        ].   
+00006ec0: 207d 0a7d                                 }.}
```

### Comparing `opengamedata_core-0.0.2/src/ogd/games/SHADOWSPECT/ShadowspectLoader.py` & `opengamedata_core-0.0.3/src/ogd/games/SHADOWSPECT/ShadowspectLoader.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/SHADOWSPECT/features/FunnelByUser.py` & `opengamedata_core-0.0.3/src/ogd/games/SHADOWSPECT/features/FunnelByUser.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/SHADOWSPECT/features/LevelsOfDifficulty.py` & `opengamedata_core-0.0.3/src/ogd/games/SHADOWSPECT/features/LevelsOfDifficulty.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/SHADOWSPECT/features/MoveShapeCount.py` & `opengamedata_core-0.0.3/src/ogd/games/SHADOWSPECT/features/MoveShapeCount.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/SHADOWSPECT/features/SequenceBetweenPuzzles.py` & `opengamedata_core-0.0.3/src/ogd/games/SHADOWSPECT/features/SequenceBetweenPuzzles.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/SHADOWSPECT/features/SessionID.py` & `opengamedata_core-0.0.3/src/ogd/games/SHADOWSPECT/features/SessionID.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/SHADOWSPECT/schemas/SHADOWSPECT.json.template` & `opengamedata_core-0.0.3/src/ogd/games/SHADOWSPECT/schemas/SHADOWSPECT.json.template`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/SHIPWRECKS/ShipwrecksLoader.py` & `opengamedata_core-0.0.3/src/ogd/games/SHIPWRECKS/ShipwrecksLoader.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/SHIPWRECKS/features/ActiveJobs.py` & `opengamedata_core-0.0.3/src/ogd/games/SHIPWRECKS/features/ActiveJobs.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/SHIPWRECKS/features/EventList.py` & `opengamedata_core-0.0.3/src/ogd/games/SHIPWRECKS/features/EventList.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/SHIPWRECKS/features/EvidenceBoardCompleteCount.py` & `opengamedata_core-0.0.3/src/ogd/games/SHIPWRECKS/features/EvidenceBoardCompleteCount.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/SHIPWRECKS/features/JobsAttempted.py` & `opengamedata_core-0.0.3/src/ogd/games/SHIPWRECKS/features/JobsAttempted.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/SHIPWRECKS/features/JobsCompleted.py` & `opengamedata_core-0.0.3/src/ogd/games/SHIPWRECKS/features/JobsCompleted.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/SHIPWRECKS/features/MissionDiveTime.py` & `opengamedata_core-0.0.3/src/ogd/games/SHIPWRECKS/features/MissionDiveTime.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/SHIPWRECKS/features/MissionSonarTimeToComplete.py` & `opengamedata_core-0.0.3/src/ogd/games/SHIPWRECKS/features/MissionSonarTimeToComplete.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/SHIPWRECKS/features/PlayerSummary.py` & `opengamedata_core-0.0.3/src/ogd/games/SHIPWRECKS/features/PlayerSummary.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/SHIPWRECKS/features/PopulationSummary.py` & `opengamedata_core-0.0.3/src/ogd/games/SHIPWRECKS/features/PopulationSummary.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/SHIPWRECKS/features/SessionDuration.py` & `opengamedata_core-0.0.3/src/ogd/games/SHIPWRECKS/features/SessionDuration.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/SHIPWRECKS/features/SessionID.py` & `opengamedata_core-0.0.3/src/ogd/games/SHIPWRECKS/features/SessionID.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/SHIPWRECKS/features/TopJobCompletionDestinations.py` & `opengamedata_core-0.0.3/src/ogd/games/SHIPWRECKS/features/TopJobCompletionDestinations.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/SHIPWRECKS/features/TopJobSwitchDestinations.py` & `opengamedata_core-0.0.3/src/ogd/games/SHIPWRECKS/features/TopJobSwitchDestinations.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/SHIPWRECKS/features/TotalDiveTime.py` & `opengamedata_core-0.0.3/src/ogd/games/SHIPWRECKS/features/TotalDiveTime.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/SHIPWRECKS/features/__init__.py` & `opengamedata_core-0.0.3/src/ogd/games/SHIPWRECKS/features/__init__.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/SHIPWRECKS/schemas/SHIPWRECKS.json.template` & `opengamedata_core-0.0.3/src/ogd/games/SHIPWRECKS/schemas/SHIPWRECKS.json.template`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/THERMOVR/ThermoVRLoader.py` & `opengamedata_core-0.0.3/src/ogd/games/THERMOVR/ThermoVRLoader.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/THERMOVR/features/LeftHandMoves.py` & `opengamedata_core-0.0.3/src/ogd/games/THERMOVR/features/LeftHandMoves.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/THERMOVR/features/PhasesReached.py` & `opengamedata_core-0.0.3/src/ogd/games/THERMOVR/features/PhasesReached.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/THERMOVR/features/PlayMode.py` & `opengamedata_core-0.0.3/src/ogd/games/THERMOVR/features/PlayMode.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/THERMOVR/features/RightHandMoves.py` & `opengamedata_core-0.0.3/src/ogd/games/THERMOVR/features/RightHandMoves.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/THERMOVR/features/TaskCompleteCount.py` & `opengamedata_core-0.0.3/src/ogd/games/THERMOVR/features/TaskCompleteCount.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/THERMOVR/features/ToolNudgeCount.py` & `opengamedata_core-0.0.3/src/ogd/games/THERMOVR/features/ToolNudgeCount.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/THERMOVR/features/ToolSliderTime.py` & `opengamedata_core-0.0.3/src/ogd/games/THERMOVR/features/ToolSliderTime.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/THERMOVR/schemas/THERMOVR.json.template` & `opengamedata_core-0.0.3/src/ogd/games/THERMOVR/schemas/THERMOVR.json.template`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/TRANSFORMATION_QUEST/DBExport.json` & `opengamedata_core-0.0.3/src/ogd/games/TRANSFORMATION_QUEST/DBExport.json`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/TRANSFORMATION_QUEST/schemas/TRANSFORMATION_QUEST.json.template` & `opengamedata_core-0.0.3/src/ogd/games/TRANSFORMATION_QUEST/schemas/TRANSFORMATION_QUEST.json.template`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/WAVES/WaveLoader.py` & `opengamedata_core-0.0.3/src/ogd/games/WAVES/WaveLoader.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/WAVES/features/AmplitudeGoodMoveCount.py` & `opengamedata_core-0.0.3/src/ogd/games/WAVES/features/AmplitudeGoodMoveCount.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/WAVES/features/AverageFails.py` & `opengamedata_core-0.0.3/src/ogd/games/WAVES/features/AverageFails.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/WAVES/features/AverageLevelTime.py` & `opengamedata_core-0.0.3/src/ogd/games/WAVES/features/AverageLevelTime.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/WAVES/features/AverageMoveTypeChanges.py` & `opengamedata_core-0.0.3/src/ogd/games/WAVES/features/AverageMoveTypeChanges.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/WAVES/features/AverageSliderMoves.py` & `opengamedata_core-0.0.3/src/ogd/games/WAVES/features/AverageSliderMoves.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/WAVES/features/BeginCount.py` & `opengamedata_core-0.0.3/src/ogd/games/WAVES/features/BeginCount.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/WAVES/features/ClosenessIntercept.py` & `opengamedata_core-0.0.3/src/ogd/games/WAVES/features/ClosenessIntercept.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/WAVES/features/ClosenessR2.py` & `opengamedata_core-0.0.3/src/ogd/games/WAVES/features/ClosenessR2.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/WAVES/features/ClosenessSlope.py` & `opengamedata_core-0.0.3/src/ogd/games/WAVES/features/ClosenessSlope.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/WAVES/features/Completed.py` & `opengamedata_core-0.0.3/src/ogd/games/WAVES/features/Completed.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/WAVES/features/FirstMoveType.py` & `opengamedata_core-0.0.3/src/ogd/games/WAVES/features/FirstMoveType.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/WAVES/features/MenuButtonCount.py` & `opengamedata_core-0.0.3/src/ogd/games/WAVES/features/MenuButtonCount.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/WAVES/features/OffsetGoodMoveCount.py` & `opengamedata_core-0.0.3/src/ogd/games/WAVES/features/OffsetGoodMoveCount.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/WAVES/features/OverallPercentAmplitudeMoves.py` & `opengamedata_core-0.0.3/src/ogd/games/WAVES/features/OverallPercentAmplitudeMoves.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/WAVES/features/OverallPercentOffsetMoves.py` & `opengamedata_core-0.0.3/src/ogd/games/WAVES/features/OverallPercentOffsetMoves.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/WAVES/features/OverallPercentWavelengthMoves.py` & `opengamedata_core-0.0.3/src/ogd/games/WAVES/features/OverallPercentWavelengthMoves.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/WAVES/features/OverallSliderAverageRange.py` & `opengamedata_core-0.0.3/src/ogd/games/WAVES/features/OverallSliderAverageRange.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/WAVES/features/OverallSliderAverageStandardDeviations.py` & `opengamedata_core-0.0.3/src/ogd/games/WAVES/features/OverallSliderAverageStandardDeviations.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/WAVES/features/PercentAmplitudeGoodMoves.py` & `opengamedata_core-0.0.3/src/ogd/games/WAVES/features/PercentAmplitudeGoodMoves.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/WAVES/features/PercentAmplitudeMoves.py` & `opengamedata_core-0.0.3/src/ogd/games/WAVES/features/PercentAmplitudeMoves.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/WAVES/features/PercentOffsetGoodMoves.py` & `opengamedata_core-0.0.3/src/ogd/games/WAVES/features/PercentOffsetGoodMoves.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/WAVES/features/PercentOffsetMoves.py` & `opengamedata_core-0.0.3/src/ogd/games/WAVES/features/PercentOffsetMoves.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/WAVES/features/PercentWavelengthGoodMoves.py` & `opengamedata_core-0.0.3/src/ogd/games/WAVES/features/PercentWavelengthGoodMoves.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/WAVES/features/PercentWavelengthMoves.py` & `opengamedata_core-0.0.3/src/ogd/games/WAVES/features/PercentWavelengthMoves.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/WAVES/features/PersistentSessionID.py` & `opengamedata_core-0.0.3/src/ogd/games/WAVES/features/PersistentSessionID.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/WAVES/features/QuestionAnswered.py` & `opengamedata_core-0.0.3/src/ogd/games/WAVES/features/QuestionAnswered.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/WAVES/features/QuestionCorrect.py` & `opengamedata_core-0.0.3/src/ogd/games/WAVES/features/QuestionCorrect.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/WAVES/features/RangeIntercept.py` & `opengamedata_core-0.0.3/src/ogd/games/WAVES/features/RangeIntercept.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/WAVES/features/RangeR2.py` & `opengamedata_core-0.0.3/src/ogd/games/WAVES/features/RangeR2.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/WAVES/features/RangeSlope.py` & `opengamedata_core-0.0.3/src/ogd/games/WAVES/features/RangeSlope.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/WAVES/features/SequenceLevel.py` & `opengamedata_core-0.0.3/src/ogd/games/WAVES/features/SequenceLevel.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/WAVES/features/SessionID.py` & `opengamedata_core-0.0.3/src/ogd/games/WAVES/features/SessionID.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/WAVES/features/SliderAverageRange.py` & `opengamedata_core-0.0.3/src/ogd/games/WAVES/features/SliderAverageRange.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/WAVES/features/SliderAverageStandardDeviations.py` & `opengamedata_core-0.0.3/src/ogd/games/WAVES/features/SliderAverageStandardDeviations.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/WAVES/features/SucceedCount.py` & `opengamedata_core-0.0.3/src/ogd/games/WAVES/features/SucceedCount.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/WAVES/features/TimeToAnswerMS.py` & `opengamedata_core-0.0.3/src/ogd/games/WAVES/features/TimeToAnswerMS.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/WAVES/features/TotalArrowMoves.py` & `opengamedata_core-0.0.3/src/ogd/games/AQUALAB/features/TotalHelpCount.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,35 +1,37 @@
-# import libraries
-from ogd.core.schemas import Event
-from typing import Any, List, Optional
+from typing import Any, List
 # import locals
-from ogd.core.generators.extractors.PerLevelFeature import PerLevelFeature
 from ogd.core.generators.Generator import GeneratorParameters
+from ogd.core.generators.extractors.Feature import Feature
 from ogd.core.schemas.Event import Event
 from ogd.core.schemas.ExtractionMode import ExtractionMode
 from ogd.core.schemas.FeatureData import FeatureData
 
-class TotalArrowMoves(PerLevelFeature):
+class TotalHelpCount(Feature):
+    """_summary_
+
+    :param Feature: _description_
+    :type Feature: _type_
+    """
     def __init__(self, params:GeneratorParameters):
-        PerLevelFeature.__init__(self, params=params)
-        self._arrow_move_count : int = 0
+        super().__init__(params=params)
+        self._count = 0
 
     # *** IMPLEMENT ABSTRACT FUNCTIONS ***
     @classmethod
     def _eventFilter(cls, mode:ExtractionMode) -> List[str]:
-        return ["CUSTOM.2"]
-        # return ["ARROW_MOVE_RELEASE"]
+        return ["ask_for_help"]
 
     @classmethod
     def _featureFilter(cls, mode:ExtractionMode) -> List[str]:
         return []
 
     def _updateFromEvent(self, event:Event) -> None:
-        self._arrow_move_count += 1
+        self._count += 1
 
     def _updateFromFeatureData(self, feature:FeatureData):
         return
 
     def _getFeatureValues(self) -> List[Any]:
-        return [self._arrow_move_count]
+        return [self._count]
 
     # *** Optionally override public functions. ***
```

### Comparing `opengamedata_core-0.0.2/src/ogd/games/WAVES/features/TotalFails.py` & `opengamedata_core-0.0.3/src/ogd/games/WAVES/features/TotalFails.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/WAVES/features/TotalLevelTime.py` & `opengamedata_core-0.0.3/src/ogd/games/WAVES/features/TotalLevelTime.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/WAVES/features/TotalMoveTypeChanges.py` & `opengamedata_core-0.0.3/src/ogd/games/WAVES/features/TotalMoveTypeChanges.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/WAVES/features/TotalResets.py` & `opengamedata_core-0.0.3/src/ogd/games/WAVES/features/TotalResets.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/WAVES/features/TotalSkips.py` & `opengamedata_core-0.0.3/src/ogd/games/WAVES/features/TotalSkips.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/WAVES/features/TotalSliderMoves.py` & `opengamedata_core-0.0.3/src/ogd/games/WAVES/features/TotalSliderMoves.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/WAVES/features/WavelengthGoodMoveCount.py` & `opengamedata_core-0.0.3/src/ogd/games/WAVES/features/WavelengthGoodMoveCount.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/WAVES/features/__init__.py` & `opengamedata_core-0.0.3/src/ogd/games/WAVES/features/__init__.py`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/WAVES/schemas/WAVES.json.template` & `opengamedata_core-0.0.3/src/ogd/games/WAVES/schemas/WAVES.json.template`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/ogd/games/WEATHER_STATION/schemas/WEATHER_STATION.json.template` & `opengamedata_core-0.0.3/src/ogd/games/WEATHER_STATION/schemas/WEATHER_STATION.json.template`

 * *Files identical despite different names*

### Comparing `opengamedata_core-0.0.2/src/opengamedata_core.egg-info/PKG-INFO` & `opengamedata_core-0.0.3/src/opengamedata_core.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opengamedata-core
-Version: 0.0.2
+Version: 0.0.3
 Summary: A package for retrieving and processing event-based video game data. Additional authors: Nick Spevacek, Renee Li, John McCloskey, Zach Studdiford, Glenn Palmer, Haishuo Chen, Daus, Ameya Kshirsagar, Yunqing Xiao, Erik Harpstead, Manuel Jesus Gomez Moratilla
 Author-email: Luke Swanson <superscription58@gmail.com>, David Gagnon <djgagnon@wisc.edu>
 Project-URL: Homepage, https://github.com/opengamedata/opengamedata-core
 Project-URL: Bug Tracker, https://github.com/opengamedata/opengamedata-core/issues
 Project-URL: Documentation, https://opengamedata-doc.readthedocs.io/en/latest/index.html
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `opengamedata_core-0.0.2/src/opengamedata_core.egg-info/SOURCES.txt` & `opengamedata_core-0.0.3/src/opengamedata_core.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -2,14 +2,18 @@
 README.md
 pyproject.toml
 src/ogd/__init__.py
 src/ogd/core/__init__.py
 src/ogd/core/exec/Commands.py
 src/ogd/core/exec/Generators.py
 src/ogd/core/exec/Parsers.py
+src/ogd/core/games/AQUALAB/features/AppVersions.py
+src/ogd/core/games/AQUALAB/features/PlayLocations.py
+src/ogd/core/games/JOURNALISM/features/FailureAttributes.py
+src/ogd/core/games/JOURNALISM/features/FinalAttributes.py
 src/ogd/core/generators/Generator.py
 src/ogd/core/generators/GeneratorLoader.py
 src/ogd/core/generators/__init__.py
 src/ogd/core/generators/detectors/Detector.py
 src/ogd/core/generators/detectors/DetectorEvent.py
 src/ogd/core/generators/detectors/__init__.py
 src/ogd/core/generators/extractors/Extractor.py
@@ -93,14 +97,15 @@
 src/ogd/core/schemas/table_schemas/OPENGAMEDATA_MYSQL.json
 src/ogd/core/schemas/table_schemas/SHIPWRECKS.json
 src/ogd/core/schemas/tables/ColumnMapSchema.py
 src/ogd/core/schemas/tables/ColumnSchema.py
 src/ogd/core/schemas/tables/TableSchema.py
 src/ogd/core/utils/Logger.py
 src/ogd/core/utils/Readme.py
+src/ogd/core/utils/SemanticVersion.py
 src/ogd/core/utils/__init__.py
 src/ogd/core/utils/typing.py
 src/ogd/core/utils/utils.py
 src/ogd/games/__init__.py
 src/ogd/games/ALL_YOU_CAN_ET/schemas/ALL_YOU_CAN_ET.json.template
 src/ogd/games/AQUALAB/AqualabLoader.py
 src/ogd/games/AQUALAB/DBExport.json
@@ -111,52 +116,67 @@
 src/ogd/games/AQUALAB/detectors/HintAndLeave.py
 src/ogd/games/AQUALAB/detectors/Idle.py
 src/ogd/games/AQUALAB/detectors/SceneChangeFrequently.py
 src/ogd/games/AQUALAB/detectors/TwoHints.py
 src/ogd/games/AQUALAB/detectors/__init__.py
 src/ogd/games/AQUALAB/features/ActiveJobs.py
 src/ogd/games/AQUALAB/features/ActiveTime.py
+src/ogd/games/AQUALAB/features/AppVersions.py
+src/ogd/games/AQUALAB/features/AverageSessionTime.py
 src/ogd/games/AQUALAB/features/EchoSessionID.py
 src/ogd/games/AQUALAB/features/EventList.py
 src/ogd/games/AQUALAB/features/JobActiveTime.py
-src/ogd/games/AQUALAB/features/JobArgumentationTime.py
+src/ogd/games/AQUALAB/features/JobArgumentation.py
 src/ogd/games/AQUALAB/features/JobCompletionTime.py
 src/ogd/games/AQUALAB/features/JobDiveSitesCount.py
 src/ogd/games/AQUALAB/features/JobDiveTime.py
-src/ogd/games/AQUALAB/features/JobExperimentationTime.py
+src/ogd/games/AQUALAB/features/JobExperimentation.py
 src/ogd/games/AQUALAB/features/JobGuideCount.py
 src/ogd/games/AQUALAB/features/JobHelpCount.py
 src/ogd/games/AQUALAB/features/JobLocationChanges.py
-src/ogd/games/AQUALAB/features/JobModelingTime.py
+src/ogd/games/AQUALAB/features/JobModeling.py
 src/ogd/games/AQUALAB/features/JobPlayTime.py
+src/ogd/games/AQUALAB/features/JobPriorAttempt.py
+src/ogd/games/AQUALAB/features/JobPriorComplete.py
 src/ogd/games/AQUALAB/features/JobStartCount.py
 src/ogd/games/AQUALAB/features/JobTasksCompleted.py
 src/ogd/games/AQUALAB/features/JobTriesInArgument.py
 src/ogd/games/AQUALAB/features/JobsAttempted.py
 src/ogd/games/AQUALAB/features/JobsCompleted.py
 src/ogd/games/AQUALAB/features/ModelExportCount.py
 src/ogd/games/AQUALAB/features/ModelInterveneCount.py
 src/ogd/games/AQUALAB/features/ModelPredictCount.py
 src/ogd/games/AQUALAB/features/PerJobFeature.py
+src/ogd/games/AQUALAB/features/PlayLocations.py
 src/ogd/games/AQUALAB/features/PlayerSummary.py
 src/ogd/games/AQUALAB/features/PopulationSummary.py
+src/ogd/games/AQUALAB/features/RegionJobCount.py
+src/ogd/games/AQUALAB/features/RegionName.py
 src/ogd/games/AQUALAB/features/SessionDiveSitesCount.py
 src/ogd/games/AQUALAB/features/SessionDuration.py
 src/ogd/games/AQUALAB/features/SessionGuideCount.py
 src/ogd/games/AQUALAB/features/SessionHelpCount.py
 src/ogd/games/AQUALAB/features/SessionID.py
 src/ogd/games/AQUALAB/features/SessionJobsCompleted.py
 src/ogd/games/AQUALAB/features/SwitchJobsCount.py
 src/ogd/games/AQUALAB/features/SyncCompletionTime.py
 src/ogd/games/AQUALAB/features/TankRulesCount.py
 src/ogd/games/AQUALAB/features/TopJobCompletionDestinations.py
 src/ogd/games/AQUALAB/features/TopJobSwitchDestinations.py
+src/ogd/games/AQUALAB/features/TotalArcticTime.py
 src/ogd/games/AQUALAB/features/TotalArgumentationTime.py
+src/ogd/games/AQUALAB/features/TotalBayouTime.py
+src/ogd/games/AQUALAB/features/TotalCoralTime.py
 src/ogd/games/AQUALAB/features/TotalDiveTime.py
 src/ogd/games/AQUALAB/features/TotalExperimentationTime.py
+src/ogd/games/AQUALAB/features/TotalGuideCount.py
+src/ogd/games/AQUALAB/features/TotalHelpCount.py
+src/ogd/games/AQUALAB/features/TotalKelpTime.py
+src/ogd/games/AQUALAB/features/TotalModelingTime.py
+src/ogd/games/AQUALAB/features/TotalPlayTime.py
 src/ogd/games/AQUALAB/features/UserAvgActiveTime.py
 src/ogd/games/AQUALAB/features/UserAvgSessionDuration.py
 src/ogd/games/AQUALAB/features/UserTotalSessionDuration.py
 src/ogd/games/AQUALAB/features/__init__.py
 src/ogd/games/AQUALAB/schemas/AQUALAB.json.template
 src/ogd/games/BACTERIA/schemas/BACTERIA.json.template
 src/ogd/games/BALLOON/schemas/BALLOON.json.template
```

### Comparing `opengamedata_core-0.0.2/tests/test_lakeland_models.py` & `opengamedata_core-0.0.3/tests/test_lakeland_models.py`

 * *Files identical despite different names*

