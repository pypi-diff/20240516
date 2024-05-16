# Comparing `tmp/parkapi_sources-0.3.0.tar.gz` & `tmp/parkapi_sources-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "parkapi_sources-0.3.0.tar", last modified: Thu May  2 13:18:48 2024, max compression
+gzip compressed data, was "parkapi_sources-0.3.1.tar", last modified: Fri May  3 11:23:42 2024, max compression
```

## Comparing `parkapi_sources-0.3.0.tar` & `parkapi_sources-0.3.1.tar`

### file list

```diff
@@ -1,236 +1,236 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:18:48.646194 parkapi_sources-0.3.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:18:48.610194 parkapi_sources-0.3.0/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:18:48.614194 parkapi_sources-0.3.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2297 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/.github/workflows/build-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1469 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/.github/workflows/lint-test.yml
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      776 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/LICENCE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      381 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)    16246 2024-05-02 13:18:48.646194 parkapi_sources-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    14713 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:18:48.614194 parkapi_sources-0.3.0/data/
--rw-r--r--   0 runner    (1001) docker     (127)    11453 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/data/freiburg.geojson
--rw-r--r--   0 runner    (1001) docker     (127)    11994 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/data/heidelberg.geojson
--rw-r--r--   0 runner    (1001) docker     (127)    10851 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/data/mannheim.geojson
--rw-r--r--   0 runner    (1001) docker     (127)     5300 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/data/ulm.geojson
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:18:48.614194 parkapi_sources-0.3.0/dev/
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/dev/parkapi.py
--rw-r--r--   0 runner    (1001) docker     (127)     3147 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/dev/test-pull-converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     4282 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/dev/test-push-converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3279 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 13:18:48.646194 parkapi_sources-0.3.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:18:48.606194 parkapi_sources-0.3.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:18:48.614194 parkapi_sources-0.3.0/src/parkapi_sources/
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/src/parkapi_sources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-02 13:18:48.000000 parkapi_sources-0.3.0/src/parkapi_sources/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:18:48.614194 parkapi_sources-0.3.0/src/parkapi_sources/converters/
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/src/parkapi_sources/converters/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:18:48.614194 parkapi_sources-0.3.0/src/parkapi_sources/converters/bahn_v2/
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/src/parkapi_sources/converters/bahn_v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3117 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/src/parkapi_sources/converters/bahn_v2/converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1823 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/src/parkapi_sources/converters/bahn_v2/mapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     3885 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/src/parkapi_sources/converters/bahn_v2/validators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:18:48.618194 parkapi_sources-0.3.0/src/parkapi_sources/converters/base_converter/
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/src/parkapi_sources/converters/base_converter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      829 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/src/parkapi_sources/converters/base_converter/base_converter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:18:48.618194 parkapi_sources-0.3.0/src/parkapi_sources/converters/base_converter/pull/
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/src/parkapi_sources/converters/base_converter/pull/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      729 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/src/parkapi_sources/converters/base_converter/pull/pull_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2809 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/src/parkapi_sources/converters/base_converter/pull/pull_scraper_mixin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:18:48.618194 parkapi_sources-0.3.0/src/parkapi_sources/converters/base_converter/pull/static_geojson_data_mixin/
--rw-r--r--   0 runner    (1001) docker     (127)      248 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/src/parkapi_sources/converters/base_converter/pull/static_geojson_data_mixin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3302 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/src/parkapi_sources/converters/base_converter/pull/static_geojson_data_mixin/mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     2207 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/src/parkapi_sources/converters/base_converter/pull/static_geojson_data_mixin/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:18:48.618194 parkapi_sources-0.3.0/src/parkapi_sources/converters/base_converter/push/
--rw-r--r--   0 runner    (1001) docker     (127)      481 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/src/parkapi_sources/converters/base_converter/push/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1478 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/src/parkapi_sources/converters/base_converter/push/csv_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)      649 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/src/parkapi_sources/converters/base_converter/push/json_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     4937 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/src/parkapi_sources/converters/base_converter/push/normalized_xlsx_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3089 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/src/parkapi_sources/converters/base_converter/push/parkapi_json_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/src/parkapi_sources/converters/base_converter/push/push_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1659 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/src/parkapi_sources/converters/base_converter/push/xlsx_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)      725 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/src/parkapi_sources/converters/base_converter/push/xml_converter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:18:48.618194 parkapi_sources-0.3.0/src/parkapi_sources/converters/bfrk_bw/
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/src/parkapi_sources/converters/bfrk_bw/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2061 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/src/parkapi_sources/converters/bfrk_bw/base_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2026 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/src/parkapi_sources/converters/bfrk_bw/base_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     1644 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/src/parkapi_sources/converters/bfrk_bw/bike_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2039 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/src/parkapi_sources/converters/bfrk_bw/bike_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     1628 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/src/parkapi_sources/converters/bfrk_bw/car_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1763 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/src/parkapi_sources/converters/bfrk_bw/car_models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:18:48.622194 parkapi_sources-0.3.0/src/parkapi_sources/converters/freiburg/
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/src/parkapi_sources/converters/freiburg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3061 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/src/parkapi_sources/converters/freiburg/converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1688 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/src/parkapi_sources/converters/freiburg/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:18:48.622194 parkapi_sources-0.3.0/src/parkapi_sources/converters/heidelberg/
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/src/parkapi_sources/converters/heidelberg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3458 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/src/parkapi_sources/converters/heidelberg/converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1970 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/src/parkapi_sources/converters/heidelberg/validators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:18:48.622194 parkapi_sources-0.3.0/src/parkapi_sources/converters/karlsruhe/
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/src/parkapi_sources/converters/karlsruhe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4312 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/src/parkapi_sources/converters/karlsruhe/converter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:18:48.622194 parkapi_sources-0.3.0/src/parkapi_sources/converters/karlsruhe/files/
--rw-r--r--   0 runner    (1001) docker     (127)     2933 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/src/parkapi_sources/converters/karlsruhe/files/ca.crt.pem
--rw-r--r--   0 runner    (1001) docker     (127)     4253 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/src/parkapi_sources/converters/karlsruhe/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:18:48.622194 parkapi_sources-0.3.0/src/parkapi_sources/converters/kienzler/
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/src/parkapi_sources/converters/kienzler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3531 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/src/parkapi_sources/converters/kienzler/converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1607 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/src/parkapi_sources/converters/kienzler/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:18:48.622194 parkapi_sources-0.3.0/src/parkapi_sources/converters/mannheim_buchen/
--rw-r--r--   0 runner    (1001) docker     (127)      210 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/src/parkapi_sources/converters/mannheim_buchen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2855 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/src/parkapi_sources/converters/mannheim_buchen/converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3452 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/src/parkapi_sources/converters/mannheim_buchen/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:18:48.622194 parkapi_sources-0.3.0/src/parkapi_sources/converters/neckarsulm/
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/src/parkapi_sources/converters/neckarsulm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2715 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/src/parkapi_sources/converters/neckarsulm/converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3263 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/src/parkapi_sources/converters/neckarsulm/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:18:48.622194 parkapi_sources-0.3.0/src/parkapi_sources/converters/neckarsulm_bike/
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/src/parkapi_sources/converters/neckarsulm_bike/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3328 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/src/parkapi_sources/converters/neckarsulm_bike/converter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:18:48.626194 parkapi_sources-0.3.0/src/parkapi_sources/converters/pbw/
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/src/parkapi_sources/converters/pbw/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4889 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/src/parkapi_sources/converters/pbw/converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2554 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/src/parkapi_sources/converters/pbw/mapper.py
--rw-r--r--   0 runner    (1001) docker     (127)    11699 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/src/parkapi_sources/converters/pbw/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:18:48.626194 parkapi_sources-0.3.0/src/parkapi_sources/converters/pforzheim/
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/src/parkapi_sources/converters/pforzheim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2669 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/src/parkapi_sources/converters/pforzheim/converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1836 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/src/parkapi_sources/converters/pforzheim/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:18:48.626194 parkapi_sources-0.3.0/src/parkapi_sources/converters/pum_bw/
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/src/parkapi_sources/converters/pum_bw/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2970 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/src/parkapi_sources/converters/pum_bw/converter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:18:48.626194 parkapi_sources-0.3.0/src/parkapi_sources/converters/reutlingen/
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/src/parkapi_sources/converters/reutlingen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2573 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/src/parkapi_sources/converters/reutlingen/converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1805 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/src/parkapi_sources/converters/reutlingen/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:18:48.626194 parkapi_sources-0.3.0/src/parkapi_sources/converters/reutlingen_bike/
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/src/parkapi_sources/converters/reutlingen_bike/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2820 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/src/parkapi_sources/converters/reutlingen_bike/converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/src/parkapi_sources/converters/reutlingen_bike/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:18:48.626194 parkapi_sources-0.3.0/src/parkapi_sources/converters/stuttgart/
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/src/parkapi_sources/converters/stuttgart/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6424 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/src/parkapi_sources/converters/stuttgart/converter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:18:48.626194 parkapi_sources-0.3.0/src/parkapi_sources/converters/ulm/
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/src/parkapi_sources/converters/ulm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2316 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/src/parkapi_sources/converters/ulm/converter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:18:48.626194 parkapi_sources-0.3.0/src/parkapi_sources/converters/vrs_p_r/
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/src/parkapi_sources/converters/vrs_p_r/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2276 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/src/parkapi_sources/converters/vrs_p_r/vrs_p_r.py
--rw-r--r--   0 runner    (1001) docker     (127)     1288 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/src/parkapi_sources/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:18:48.626194 parkapi_sources-0.3.0/src/parkapi_sources/models/
--rw-r--r--   0 runner    (1001) docker     (127)      338 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/src/parkapi_sources/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/src/parkapi_sources/models/enums.py
--rw-r--r--   0 runner    (1001) docker     (127)     7717 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/src/parkapi_sources/models/parking_site_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)      661 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/src/parkapi_sources/models/source_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     4413 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/src/parkapi_sources/models/xlsx_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     3322 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/src/parkapi_sources/parkapi_sources.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:18:48.630194 parkapi_sources-0.3.0/src/parkapi_sources/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)     9093 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/src/parkapi_sources/scripts/parkapi.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:18:48.630194 parkapi_sources-0.3.0/src/parkapi_sources/util/
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/src/parkapi_sources/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/src/parkapi_sources/util/config_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/src/parkapi_sources/util/encoding.py
--rw-r--r--   0 runner    (1001) docker     (127)    10420 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/src/parkapi_sources/util/xml_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:18:48.630194 parkapi_sources-0.3.0/src/parkapi_sources/validators/
--rw-r--r--   0 runner    (1001) docker     (127)      675 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/src/parkapi_sources/validators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      704 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/src/parkapi_sources/validators/boolean_validators.py
--rw-r--r--   0 runner    (1001) docker     (127)      899 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/src/parkapi_sources/validators/date_validator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/src/parkapi_sources/validators/datetime_validator.py
--rw-r--r--   0 runner    (1001) docker     (127)      511 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/src/parkapi_sources/validators/decimal_validators.py
--rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/src/parkapi_sources/validators/integer_validators.py
--rw-r--r--   0 runner    (1001) docker     (127)      831 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/src/parkapi_sources/validators/list_validator.py
--rw-r--r--   0 runner    (1001) docker     (127)      743 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/src/parkapi_sources/validators/noneable.py
--rw-r--r--   0 runner    (1001) docker     (127)      994 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/src/parkapi_sources/validators/string_validators.py
--rw-r--r--   0 runner    (1001) docker     (127)      473 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/src/parkapi_sources/validators/time_validators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:18:48.646194 parkapi_sources-0.3.0/src/parkapi_sources.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    16246 2024-05-02 13:18:48.000000 parkapi_sources-0.3.0/src/parkapi_sources.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8603 2024-05-02 13:18:48.000000 parkapi_sources-0.3.0/src/parkapi_sources.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 13:18:48.000000 parkapi_sources-0.3.0/src/parkapi_sources.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-02 13:18:48.000000 parkapi_sources-0.3.0/src/parkapi_sources.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-02 13:18:48.000000 parkapi_sources-0.3.0/src/parkapi_sources.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:18:48.630194 parkapi_sources-0.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      320 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:18:48.634194 parkapi_sources-0.3.0/tests/converters/
--rw-r--r--   0 runner    (1001) docker     (127)     1744 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/tests/converters/bahn_v2_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2053 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/tests/converters/bfrk_bw_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      823 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/tests/converters/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:18:48.638194 parkapi_sources-0.3.0/tests/converters/data/
--rw-r--r--   0 runner    (1001) docker     (127)   947589 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/tests/converters/data/bahn_v2.json
--rw-r--r--   0 runner    (1001) docker     (127)   552854 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/tests/converters/data/bfrk_bw_bike.csv
--rw-r--r--   0 runner    (1001) docker     (127)   617384 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/tests/converters/data/bfrk_bw_car.csv
--rw-r--r--   0 runner    (1001) docker     (127)      802 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/tests/converters/data/buchen.json
--rw-r--r--   0 runner    (1001) docker     (127)    12651 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/tests/converters/data/freiburg.json
--rw-r--r--   0 runner    (1001) docker     (127)     3681 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/tests/converters/data/heidelberg.json
--rw-r--r--   0 runner    (1001) docker     (127)    63706 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/tests/converters/data/karlsruhe.json
--rw-r--r--   0 runner    (1001) docker     (127)     3477 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/tests/converters/data/kienzler.json
--rw-r--r--   0 runner    (1001) docker     (127)    18474 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/tests/converters/data/mannheim.json
--rw-r--r--   0 runner    (1001) docker     (127)    20667 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/tests/converters/data/neckarsulm.csv
--rw-r--r--   0 runner    (1001) docker     (127)    18115 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/tests/converters/data/neckarsulm_bike.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:18:48.642194 parkapi_sources-0.3.0/tests/converters/data/pbw/
--rw-r--r--   0 runner    (1001) docker     (127)     1251 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/tests/converters/data/pbw/catalog-city.json
--rw-r--r--   0 runner    (1001) docker     (127)   114816 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/tests/converters/data/pbw/object-by-city-10.json
--rw-r--r--   0 runner    (1001) docker     (127)     5061 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/tests/converters/data/pbw/object-by-city-11.json
--rw-r--r--   0 runner    (1001) docker     (127)    36083 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/tests/converters/data/pbw/object-by-city-12.json
--rw-r--r--   0 runner    (1001) docker     (127)     1784 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/tests/converters/data/pbw/object-by-city-15.json
--rw-r--r--   0 runner    (1001) docker     (127)     6859 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/tests/converters/data/pbw/object-by-city-17.json
--rw-r--r--   0 runner    (1001) docker     (127)     7122 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/tests/converters/data/pbw/object-by-city-18.json
--rw-r--r--   0 runner    (1001) docker     (127)     5812 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/tests/converters/data/pbw/object-by-city-19.json
--rw-r--r--   0 runner    (1001) docker     (127)     5795 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/tests/converters/data/pbw/object-by-city-31.json
--rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/tests/converters/data/pbw/object-by-city-32.json
--rw-r--r--   0 runner    (1001) docker     (127)     6650 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/tests/converters/data/pbw/object-by-city-33.json
--rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/tests/converters/data/pbw/object-by-city-34.json
--rw-r--r--   0 runner    (1001) docker     (127)     3225 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/tests/converters/data/pbw/object-by-city-4.json
--rw-r--r--   0 runner    (1001) docker     (127)     3187 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/tests/converters/data/pbw/object-by-city-42.json
--rw-r--r--   0 runner    (1001) docker     (127)     3296 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/tests/converters/data/pbw/object-by-city-48.json
--rw-r--r--   0 runner    (1001) docker     (127)     1597 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/tests/converters/data/pbw/object-by-city-49.json
--rw-r--r--   0 runner    (1001) docker     (127)     3241 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/tests/converters/data/pbw/object-by-city-51.json
--rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/tests/converters/data/pbw/object-by-city-52.json
--rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/tests/converters/data/pbw/object-by-city-60.json
--rw-r--r--   0 runner    (1001) docker     (127)     1557 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/tests/converters/data/pbw/object-by-city-61.json
--rw-r--r--   0 runner    (1001) docker     (127)    14227 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/tests/converters/data/pbw/object-by-city-7.json
--rw-r--r--   0 runner    (1001) docker     (127)     3149 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/tests/converters/data/pbw/object-by-city-71.json
--rw-r--r--   0 runner    (1001) docker     (127)     7071 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/tests/converters/data/pbw/object-by-city-9.json
--rw-r--r--   0 runner    (1001) docker     (127)     6685 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/tests/converters/data/pbw/object-dynamic-all.json
--rw-r--r--   0 runner    (1001) docker     (127)    18956 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/tests/converters/data/pforzheim.json
--rw-r--r--   0 runner    (1001) docker     (127)    30849 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/tests/converters/data/pum_bw.xlsx
--rw-r--r--   0 runner    (1001) docker     (127)     9387 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/tests/converters/data/reutlingen.csv
--rw-r--r--   0 runner    (1001) docker     (127)    27295 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/tests/converters/data/reutlingen_bike.csv
--rw-r--r--   0 runner    (1001) docker     (127)    35423 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/tests/converters/data/stuttgart-realtime.xml
--rw-r--r--   0 runner    (1001) docker     (127)   218959 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/tests/converters/data/stuttgart-static.xml
--rw-r--r--   0 runner    (1001) docker     (127)    62841 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/tests/converters/data/ulm.html
--rw-r--r--   0 runner    (1001) docker     (127)   136171 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/tests/converters/data/vrs_p_r.xlsx
--rw-r--r--   0 runner    (1001) docker     (127)     1859 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/tests/converters/freiburg_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2226 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/tests/converters/heidelberg_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2439 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/tests/converters/helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     1926 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/tests/converters/karlsruhe_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/tests/converters/kienzler_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2523 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/tests/converters/mannheim_buchen_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/tests/converters/neckarsulm_bike_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/tests/converters/neckarsulm_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2880 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/tests/converters/pbw_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/tests/converters/pforzheim_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/tests/converters/pum_bw_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1246 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/tests/converters/reutlingen_bike_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/tests/converters/reutlingen_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1949 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/tests/converters/stuttgart_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1777 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/tests/converters/ulm_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/tests/converters/vrs_p_r_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:18:48.642194 parkapi_sources-0.3.0/tests/models/
--rw-r--r--   0 runner    (1001) docker     (127)     2183 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/tests/models/xlsx_inputs_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:18:48.646194 parkapi_sources-0.3.0/tests/util/
--rw-r--r--   0 runner    (1001) docker     (127)     4105 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/tests/util/data_xml_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     1706 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/tests/util/encoding_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     4039 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/tests/util/xml_helper_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:18:48.646194 parkapi_sources-0.3.0/tests/validators/
--rw-r--r--   0 runner    (1001) docker     (127)     1255 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/tests/validators/boolean_validators_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/tests/validators/date_validators_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2108 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/tests/validators/datetime_validators_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/tests/validators/integer_validators_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/tests/validators/noneable_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/tests/validators/string_validators_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      567 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/tests/validators/time_validators_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:23:42.152560 parkapi_sources-0.3.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:23:42.116559 parkapi_sources-0.3.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:23:42.116559 parkapi_sources-0.3.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2297 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/.github/workflows/build-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1469 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/.github/workflows/lint-test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      871 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/LICENCE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      381 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)    16246 2024-05-03 11:23:42.152560 parkapi_sources-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    14713 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:23:42.116559 parkapi_sources-0.3.1/data/
+-rw-r--r--   0 runner    (1001) docker     (127)    11453 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/data/freiburg.geojson
+-rw-r--r--   0 runner    (1001) docker     (127)    11994 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/data/heidelberg.geojson
+-rw-r--r--   0 runner    (1001) docker     (127)    10851 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/data/mannheim.geojson
+-rw-r--r--   0 runner    (1001) docker     (127)     5300 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/data/ulm.geojson
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:23:42.116559 parkapi_sources-0.3.1/dev/
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/dev/parkapi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3147 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/dev/test-pull-converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4282 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/dev/test-push-converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3279 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 11:23:42.152560 parkapi_sources-0.3.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:23:42.112559 parkapi_sources-0.3.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:23:42.120559 parkapi_sources-0.3.1/src/parkapi_sources/
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/src/parkapi_sources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-03 11:23:41.000000 parkapi_sources-0.3.1/src/parkapi_sources/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:23:42.120559 parkapi_sources-0.3.1/src/parkapi_sources/converters/
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/src/parkapi_sources/converters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:23:42.120559 parkapi_sources-0.3.1/src/parkapi_sources/converters/bahn_v2/
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/src/parkapi_sources/converters/bahn_v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3117 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/src/parkapi_sources/converters/bahn_v2/converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1823 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/src/parkapi_sources/converters/bahn_v2/mapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3885 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/src/parkapi_sources/converters/bahn_v2/validators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:23:42.120559 parkapi_sources-0.3.1/src/parkapi_sources/converters/base_converter/
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/src/parkapi_sources/converters/base_converter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      829 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/src/parkapi_sources/converters/base_converter/base_converter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:23:42.120559 parkapi_sources-0.3.1/src/parkapi_sources/converters/base_converter/pull/
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/src/parkapi_sources/converters/base_converter/pull/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      729 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/src/parkapi_sources/converters/base_converter/pull/pull_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2809 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/src/parkapi_sources/converters/base_converter/pull/pull_scraper_mixin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:23:42.120559 parkapi_sources-0.3.1/src/parkapi_sources/converters/base_converter/pull/static_geojson_data_mixin/
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/src/parkapi_sources/converters/base_converter/pull/static_geojson_data_mixin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3302 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/src/parkapi_sources/converters/base_converter/pull/static_geojson_data_mixin/mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2207 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/src/parkapi_sources/converters/base_converter/pull/static_geojson_data_mixin/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:23:42.124559 parkapi_sources-0.3.1/src/parkapi_sources/converters/base_converter/push/
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/src/parkapi_sources/converters/base_converter/push/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1478 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/src/parkapi_sources/converters/base_converter/push/csv_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/src/parkapi_sources/converters/base_converter/push/json_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4937 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/src/parkapi_sources/converters/base_converter/push/normalized_xlsx_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3089 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/src/parkapi_sources/converters/base_converter/push/parkapi_json_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/src/parkapi_sources/converters/base_converter/push/push_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1659 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/src/parkapi_sources/converters/base_converter/push/xlsx_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      725 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/src/parkapi_sources/converters/base_converter/push/xml_converter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:23:42.124559 parkapi_sources-0.3.1/src/parkapi_sources/converters/bfrk_bw/
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/src/parkapi_sources/converters/bfrk_bw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2061 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/src/parkapi_sources/converters/bfrk_bw/base_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2026 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/src/parkapi_sources/converters/bfrk_bw/base_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1644 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/src/parkapi_sources/converters/bfrk_bw/bike_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2039 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/src/parkapi_sources/converters/bfrk_bw/bike_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1628 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/src/parkapi_sources/converters/bfrk_bw/car_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1763 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/src/parkapi_sources/converters/bfrk_bw/car_models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:23:42.124559 parkapi_sources-0.3.1/src/parkapi_sources/converters/freiburg/
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/src/parkapi_sources/converters/freiburg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3061 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/src/parkapi_sources/converters/freiburg/converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1688 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/src/parkapi_sources/converters/freiburg/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:23:42.124559 parkapi_sources-0.3.1/src/parkapi_sources/converters/heidelberg/
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/src/parkapi_sources/converters/heidelberg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3458 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/src/parkapi_sources/converters/heidelberg/converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1970 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/src/parkapi_sources/converters/heidelberg/validators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:23:42.124559 parkapi_sources-0.3.1/src/parkapi_sources/converters/karlsruhe/
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/src/parkapi_sources/converters/karlsruhe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4312 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/src/parkapi_sources/converters/karlsruhe/converter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:23:42.124559 parkapi_sources-0.3.1/src/parkapi_sources/converters/karlsruhe/files/
+-rw-r--r--   0 runner    (1001) docker     (127)     2933 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/src/parkapi_sources/converters/karlsruhe/files/ca.crt.pem
+-rw-r--r--   0 runner    (1001) docker     (127)     4253 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/src/parkapi_sources/converters/karlsruhe/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:23:42.124559 parkapi_sources-0.3.1/src/parkapi_sources/converters/kienzler/
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/src/parkapi_sources/converters/kienzler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3531 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/src/parkapi_sources/converters/kienzler/converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1607 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/src/parkapi_sources/converters/kienzler/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:23:42.128559 parkapi_sources-0.3.1/src/parkapi_sources/converters/mannheim_buchen/
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/src/parkapi_sources/converters/mannheim_buchen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2855 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/src/parkapi_sources/converters/mannheim_buchen/converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3452 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/src/parkapi_sources/converters/mannheim_buchen/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:23:42.128559 parkapi_sources-0.3.1/src/parkapi_sources/converters/neckarsulm/
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/src/parkapi_sources/converters/neckarsulm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2715 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/src/parkapi_sources/converters/neckarsulm/converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3263 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/src/parkapi_sources/converters/neckarsulm/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:23:42.128559 parkapi_sources-0.3.1/src/parkapi_sources/converters/neckarsulm_bike/
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/src/parkapi_sources/converters/neckarsulm_bike/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3333 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/src/parkapi_sources/converters/neckarsulm_bike/converter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:23:42.128559 parkapi_sources-0.3.1/src/parkapi_sources/converters/pbw/
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/src/parkapi_sources/converters/pbw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4889 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/src/parkapi_sources/converters/pbw/converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2554 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/src/parkapi_sources/converters/pbw/mapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11699 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/src/parkapi_sources/converters/pbw/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:23:42.128559 parkapi_sources-0.3.1/src/parkapi_sources/converters/pforzheim/
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/src/parkapi_sources/converters/pforzheim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2669 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/src/parkapi_sources/converters/pforzheim/converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1836 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/src/parkapi_sources/converters/pforzheim/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:23:42.128559 parkapi_sources-0.3.1/src/parkapi_sources/converters/pum_bw/
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/src/parkapi_sources/converters/pum_bw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2970 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/src/parkapi_sources/converters/pum_bw/converter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:23:42.128559 parkapi_sources-0.3.1/src/parkapi_sources/converters/reutlingen/
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/src/parkapi_sources/converters/reutlingen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2573 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/src/parkapi_sources/converters/reutlingen/converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1805 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/src/parkapi_sources/converters/reutlingen/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:23:42.128559 parkapi_sources-0.3.1/src/parkapi_sources/converters/reutlingen_bike/
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/src/parkapi_sources/converters/reutlingen_bike/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2825 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/src/parkapi_sources/converters/reutlingen_bike/converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/src/parkapi_sources/converters/reutlingen_bike/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:23:42.128559 parkapi_sources-0.3.1/src/parkapi_sources/converters/stuttgart/
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/src/parkapi_sources/converters/stuttgart/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6424 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/src/parkapi_sources/converters/stuttgart/converter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:23:42.132559 parkapi_sources-0.3.1/src/parkapi_sources/converters/ulm/
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/src/parkapi_sources/converters/ulm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2316 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/src/parkapi_sources/converters/ulm/converter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:23:42.132559 parkapi_sources-0.3.1/src/parkapi_sources/converters/vrs_p_r/
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/src/parkapi_sources/converters/vrs_p_r/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2276 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/src/parkapi_sources/converters/vrs_p_r/vrs_p_r.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1288 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/src/parkapi_sources/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:23:42.132559 parkapi_sources-0.3.1/src/parkapi_sources/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/src/parkapi_sources/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/src/parkapi_sources/models/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7717 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/src/parkapi_sources/models/parking_site_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      661 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/src/parkapi_sources/models/source_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4413 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/src/parkapi_sources/models/xlsx_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3392 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/src/parkapi_sources/parkapi_sources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:23:42.132559 parkapi_sources-0.3.1/src/parkapi_sources/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)     9093 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/src/parkapi_sources/scripts/parkapi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:23:42.132559 parkapi_sources-0.3.1/src/parkapi_sources/util/
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/src/parkapi_sources/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/src/parkapi_sources/util/config_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/src/parkapi_sources/util/encoding.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10420 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/src/parkapi_sources/util/xml_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:23:42.132559 parkapi_sources-0.3.1/src/parkapi_sources/validators/
+-rw-r--r--   0 runner    (1001) docker     (127)      675 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/src/parkapi_sources/validators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      704 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/src/parkapi_sources/validators/boolean_validators.py
+-rw-r--r--   0 runner    (1001) docker     (127)      899 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/src/parkapi_sources/validators/date_validator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/src/parkapi_sources/validators/datetime_validator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      511 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/src/parkapi_sources/validators/decimal_validators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/src/parkapi_sources/validators/integer_validators.py
+-rw-r--r--   0 runner    (1001) docker     (127)      831 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/src/parkapi_sources/validators/list_validator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      743 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/src/parkapi_sources/validators/noneable.py
+-rw-r--r--   0 runner    (1001) docker     (127)      994 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/src/parkapi_sources/validators/string_validators.py
+-rw-r--r--   0 runner    (1001) docker     (127)      473 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/src/parkapi_sources/validators/time_validators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:23:42.148559 parkapi_sources-0.3.1/src/parkapi_sources.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    16246 2024-05-03 11:23:42.000000 parkapi_sources-0.3.1/src/parkapi_sources.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8603 2024-05-03 11:23:42.000000 parkapi_sources-0.3.1/src/parkapi_sources.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 11:23:42.000000 parkapi_sources-0.3.1/src/parkapi_sources.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-03 11:23:42.000000 parkapi_sources-0.3.1/src/parkapi_sources.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-03 11:23:42.000000 parkapi_sources-0.3.1/src/parkapi_sources.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:23:42.136559 parkapi_sources-0.3.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:23:42.136559 parkapi_sources-0.3.1/tests/converters/
+-rw-r--r--   0 runner    (1001) docker     (127)     1744 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/tests/converters/bahn_v2_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2053 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/tests/converters/bfrk_bw_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      823 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/tests/converters/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:23:42.144559 parkapi_sources-0.3.1/tests/converters/data/
+-rw-r--r--   0 runner    (1001) docker     (127)   947589 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/tests/converters/data/bahn_v2.json
+-rw-r--r--   0 runner    (1001) docker     (127)   552854 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/tests/converters/data/bfrk_bw_bike.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   617384 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/tests/converters/data/bfrk_bw_car.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      802 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/tests/converters/data/buchen.json
+-rw-r--r--   0 runner    (1001) docker     (127)    12651 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/tests/converters/data/freiburg.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3681 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/tests/converters/data/heidelberg.json
+-rw-r--r--   0 runner    (1001) docker     (127)    63706 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/tests/converters/data/karlsruhe.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3477 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/tests/converters/data/kienzler.json
+-rw-r--r--   0 runner    (1001) docker     (127)    18474 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/tests/converters/data/mannheim.json
+-rw-r--r--   0 runner    (1001) docker     (127)    20667 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/tests/converters/data/neckarsulm.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    18115 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/tests/converters/data/neckarsulm_bike.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:23:42.148559 parkapi_sources-0.3.1/tests/converters/data/pbw/
+-rw-r--r--   0 runner    (1001) docker     (127)     1251 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/tests/converters/data/pbw/catalog-city.json
+-rw-r--r--   0 runner    (1001) docker     (127)   114816 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/tests/converters/data/pbw/object-by-city-10.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5061 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/tests/converters/data/pbw/object-by-city-11.json
+-rw-r--r--   0 runner    (1001) docker     (127)    36083 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/tests/converters/data/pbw/object-by-city-12.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1784 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/tests/converters/data/pbw/object-by-city-15.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6859 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/tests/converters/data/pbw/object-by-city-17.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7122 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/tests/converters/data/pbw/object-by-city-18.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5812 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/tests/converters/data/pbw/object-by-city-19.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5795 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/tests/converters/data/pbw/object-by-city-31.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/tests/converters/data/pbw/object-by-city-32.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6650 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/tests/converters/data/pbw/object-by-city-33.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/tests/converters/data/pbw/object-by-city-34.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3225 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/tests/converters/data/pbw/object-by-city-4.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3187 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/tests/converters/data/pbw/object-by-city-42.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3296 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/tests/converters/data/pbw/object-by-city-48.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1597 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/tests/converters/data/pbw/object-by-city-49.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3241 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/tests/converters/data/pbw/object-by-city-51.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/tests/converters/data/pbw/object-by-city-52.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/tests/converters/data/pbw/object-by-city-60.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1557 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/tests/converters/data/pbw/object-by-city-61.json
+-rw-r--r--   0 runner    (1001) docker     (127)    14227 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/tests/converters/data/pbw/object-by-city-7.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3149 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/tests/converters/data/pbw/object-by-city-71.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7071 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/tests/converters/data/pbw/object-by-city-9.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6685 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/tests/converters/data/pbw/object-dynamic-all.json
+-rw-r--r--   0 runner    (1001) docker     (127)    18956 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/tests/converters/data/pforzheim.json
+-rw-r--r--   0 runner    (1001) docker     (127)    30849 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/tests/converters/data/pum_bw.xlsx
+-rw-r--r--   0 runner    (1001) docker     (127)     9387 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/tests/converters/data/reutlingen.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    27295 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/tests/converters/data/reutlingen_bike.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    35423 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/tests/converters/data/stuttgart-realtime.xml
+-rw-r--r--   0 runner    (1001) docker     (127)   218959 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/tests/converters/data/stuttgart-static.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    62841 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/tests/converters/data/ulm.html
+-rw-r--r--   0 runner    (1001) docker     (127)   136171 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/tests/converters/data/vrs_p_r.xlsx
+-rw-r--r--   0 runner    (1001) docker     (127)     1859 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/tests/converters/freiburg_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2226 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/tests/converters/heidelberg_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2439 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/tests/converters/helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1926 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/tests/converters/karlsruhe_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/tests/converters/kienzler_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2523 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/tests/converters/mannheim_buchen_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/tests/converters/neckarsulm_bike_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/tests/converters/neckarsulm_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2880 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/tests/converters/pbw_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/tests/converters/pforzheim_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/tests/converters/pum_bw_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1246 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/tests/converters/reutlingen_bike_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/tests/converters/reutlingen_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1949 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/tests/converters/stuttgart_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1777 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/tests/converters/ulm_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/tests/converters/vrs_p_r_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:23:42.148559 parkapi_sources-0.3.1/tests/models/
+-rw-r--r--   0 runner    (1001) docker     (127)     2183 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/tests/models/xlsx_inputs_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:23:42.148559 parkapi_sources-0.3.1/tests/util/
+-rw-r--r--   0 runner    (1001) docker     (127)     4105 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/tests/util/data_xml_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1706 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/tests/util/encoding_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4039 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/tests/util/xml_helper_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:23:42.148559 parkapi_sources-0.3.1/tests/validators/
+-rw-r--r--   0 runner    (1001) docker     (127)     1255 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/tests/validators/boolean_validators_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/tests/validators/date_validators_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2108 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/tests/validators/datetime_validators_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/tests/validators/integer_validators_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/tests/validators/noneable_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/tests/validators/string_validators_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      567 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/tests/validators/time_validators_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/tox.ini
```

### Comparing `parkapi_sources-0.3.0/.github/workflows/build-publish.yml` & `parkapi_sources-0.3.1/.github/workflows/build-publish.yml`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.0/.github/workflows/lint-test.yml` & `parkapi_sources-0.3.1/.github/workflows/lint-test.yml`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.0/CHANGELOG.md` & `parkapi_sources-0.3.1/CHANGELOG.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,16 @@
 # Changelog
 
+## 0.3.1
+
+Released 2024-05-03
+
+Fixes:
+* Register neckarsulm_bike and reutlingen_bike properly
+
 ## 0.3.0
 
 Released 2024-05-02
 
 Features:
 
 * Automated tests via CI pipeline
```

### Comparing `parkapi_sources-0.3.0/LICENCE.txt` & `parkapi_sources-0.3.1/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.0/PKG-INFO` & `parkapi_sources-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: parkapi_sources
-Version: 0.3.0
+Version: 0.3.1
 Summary: ParkAPI Sources is a collection of converters from several different data sources to normalized ParkAPI data.
 Author-email: "Ernesto Ruge, binary butterfly GmbH" <ernesto.ruge@binary-butterfly.de>
 Maintainer-email: "Ernesto Ruge, binary butterfly GmbH" <ernesto.ruge@binary-butterfly.de>
 Keywords: data,parking,converter,mobility,car,bike
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `parkapi_sources-0.3.0/README.md` & `parkapi_sources-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.0/data/freiburg.geojson` & `parkapi_sources-0.3.1/data/freiburg.geojson`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.0/data/heidelberg.geojson` & `parkapi_sources-0.3.1/data/heidelberg.geojson`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.0/data/mannheim.geojson` & `parkapi_sources-0.3.1/data/mannheim.geojson`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.0/data/ulm.geojson` & `parkapi_sources-0.3.1/data/ulm.geojson`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.0/dev/test-pull-converter.py` & `parkapi_sources-0.3.1/dev/test-pull-converter.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.0/dev/test-push-converter.py` & `parkapi_sources-0.3.1/dev/test-push-converter.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.0/pyproject.toml` & `parkapi_sources-0.3.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.0/src/parkapi_sources/converters/__init__.py` & `parkapi_sources-0.3.1/src/parkapi_sources/converters/__init__.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.0/src/parkapi_sources/converters/bahn_v2/converter.py` & `parkapi_sources-0.3.1/src/parkapi_sources/converters/bahn_v2/converter.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.0/src/parkapi_sources/converters/bahn_v2/mapper.py` & `parkapi_sources-0.3.1/src/parkapi_sources/converters/bahn_v2/mapper.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.0/src/parkapi_sources/converters/bahn_v2/validators.py` & `parkapi_sources-0.3.1/src/parkapi_sources/converters/bahn_v2/validators.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.0/src/parkapi_sources/converters/base_converter/base_converter.py` & `parkapi_sources-0.3.1/src/parkapi_sources/converters/base_converter/base_converter.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.0/src/parkapi_sources/converters/base_converter/pull/pull_converter.py` & `parkapi_sources-0.3.1/src/parkapi_sources/converters/base_converter/pull/pull_converter.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.0/src/parkapi_sources/converters/base_converter/pull/pull_scraper_mixin.py` & `parkapi_sources-0.3.1/src/parkapi_sources/converters/base_converter/pull/pull_scraper_mixin.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.0/src/parkapi_sources/converters/base_converter/pull/static_geojson_data_mixin/mixin.py` & `parkapi_sources-0.3.1/src/parkapi_sources/converters/base_converter/pull/static_geojson_data_mixin/mixin.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.0/src/parkapi_sources/converters/base_converter/pull/static_geojson_data_mixin/models.py` & `parkapi_sources-0.3.1/src/parkapi_sources/converters/base_converter/pull/static_geojson_data_mixin/models.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.0/src/parkapi_sources/converters/base_converter/push/csv_converter.py` & `parkapi_sources-0.3.1/src/parkapi_sources/converters/base_converter/push/csv_converter.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.0/src/parkapi_sources/converters/base_converter/push/json_converter.py` & `parkapi_sources-0.3.1/src/parkapi_sources/converters/base_converter/push/json_converter.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.0/src/parkapi_sources/converters/base_converter/push/normalized_xlsx_converter.py` & `parkapi_sources-0.3.1/src/parkapi_sources/converters/base_converter/push/normalized_xlsx_converter.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.0/src/parkapi_sources/converters/base_converter/push/parkapi_json_converter.py` & `parkapi_sources-0.3.1/src/parkapi_sources/converters/base_converter/push/parkapi_json_converter.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.0/src/parkapi_sources/converters/base_converter/push/xlsx_converter.py` & `parkapi_sources-0.3.1/src/parkapi_sources/converters/base_converter/push/xlsx_converter.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.0/src/parkapi_sources/converters/base_converter/push/xml_converter.py` & `parkapi_sources-0.3.1/src/parkapi_sources/converters/base_converter/push/xml_converter.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.0/src/parkapi_sources/converters/bfrk_bw/base_converter.py` & `parkapi_sources-0.3.1/src/parkapi_sources/converters/bfrk_bw/base_converter.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.0/src/parkapi_sources/converters/bfrk_bw/base_models.py` & `parkapi_sources-0.3.1/src/parkapi_sources/converters/bfrk_bw/base_models.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.0/src/parkapi_sources/converters/bfrk_bw/bike_converter.py` & `parkapi_sources-0.3.1/src/parkapi_sources/converters/bfrk_bw/bike_converter.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.0/src/parkapi_sources/converters/bfrk_bw/bike_models.py` & `parkapi_sources-0.3.1/src/parkapi_sources/converters/bfrk_bw/bike_models.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.0/src/parkapi_sources/converters/bfrk_bw/car_converter.py` & `parkapi_sources-0.3.1/src/parkapi_sources/converters/bfrk_bw/car_converter.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.0/src/parkapi_sources/converters/bfrk_bw/car_models.py` & `parkapi_sources-0.3.1/src/parkapi_sources/converters/bfrk_bw/car_models.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.0/src/parkapi_sources/converters/freiburg/converter.py` & `parkapi_sources-0.3.1/src/parkapi_sources/converters/freiburg/converter.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.0/src/parkapi_sources/converters/freiburg/models.py` & `parkapi_sources-0.3.1/src/parkapi_sources/converters/freiburg/models.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.0/src/parkapi_sources/converters/heidelberg/converter.py` & `parkapi_sources-0.3.1/src/parkapi_sources/converters/heidelberg/converter.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.0/src/parkapi_sources/converters/heidelberg/validators.py` & `parkapi_sources-0.3.1/src/parkapi_sources/converters/heidelberg/validators.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.0/src/parkapi_sources/converters/karlsruhe/converter.py` & `parkapi_sources-0.3.1/src/parkapi_sources/converters/karlsruhe/converter.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.0/src/parkapi_sources/converters/karlsruhe/files/ca.crt.pem` & `parkapi_sources-0.3.1/src/parkapi_sources/converters/karlsruhe/files/ca.crt.pem`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.0/src/parkapi_sources/converters/karlsruhe/models.py` & `parkapi_sources-0.3.1/src/parkapi_sources/converters/karlsruhe/models.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.0/src/parkapi_sources/converters/kienzler/converter.py` & `parkapi_sources-0.3.1/src/parkapi_sources/converters/kienzler/converter.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.0/src/parkapi_sources/converters/kienzler/models.py` & `parkapi_sources-0.3.1/src/parkapi_sources/converters/kienzler/models.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.0/src/parkapi_sources/converters/mannheim_buchen/converter.py` & `parkapi_sources-0.3.1/src/parkapi_sources/converters/mannheim_buchen/converter.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.0/src/parkapi_sources/converters/mannheim_buchen/models.py` & `parkapi_sources-0.3.1/src/parkapi_sources/converters/mannheim_buchen/models.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.0/src/parkapi_sources/converters/neckarsulm/converter.py` & `parkapi_sources-0.3.1/src/parkapi_sources/converters/neckarsulm/converter.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.0/src/parkapi_sources/converters/neckarsulm/models.py` & `parkapi_sources-0.3.1/src/parkapi_sources/converters/neckarsulm/models.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.0/src/parkapi_sources/converters/neckarsulm_bike/converter.py` & `parkapi_sources-0.3.1/src/parkapi_sources/converters/neckarsulm_bike/converter.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from parkapi_sources.models import RealtimeParkingSiteInput, SourceInfo, StaticParkingSiteInput
 
 
 class NeckarsulmBikePushConverter(CsvConverter):
     proj: pyproj.Proj = pyproj.Proj(proj='utm', zone=32, ellps='WGS84', preserve_units=True)
 
     source_info = SourceInfo(
-        uid='neckarsulm',
+        uid='neckarsulm_bike',
         name='Stadt Neckarsulm: Fahrad-Abstellanlagen',
         public_url='https://www.neckarsulm.de',
         has_realtime_data=False,
     )
 
     header_mapping: dict[str, str] = {
         'id': 'uid',
```

### Comparing `parkapi_sources-0.3.0/src/parkapi_sources/converters/pbw/converter.py` & `parkapi_sources-0.3.1/src/parkapi_sources/converters/pbw/converter.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.0/src/parkapi_sources/converters/pbw/mapper.py` & `parkapi_sources-0.3.1/src/parkapi_sources/converters/pbw/mapper.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.0/src/parkapi_sources/converters/pbw/validation.py` & `parkapi_sources-0.3.1/src/parkapi_sources/converters/pbw/validation.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.0/src/parkapi_sources/converters/pforzheim/converter.py` & `parkapi_sources-0.3.1/src/parkapi_sources/converters/pforzheim/converter.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.0/src/parkapi_sources/converters/pforzheim/validation.py` & `parkapi_sources-0.3.1/src/parkapi_sources/converters/pforzheim/validation.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.0/src/parkapi_sources/converters/pum_bw/converter.py` & `parkapi_sources-0.3.1/src/parkapi_sources/converters/pum_bw/converter.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.0/src/parkapi_sources/converters/reutlingen/converter.py` & `parkapi_sources-0.3.1/src/parkapi_sources/converters/reutlingen/converter.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.0/src/parkapi_sources/converters/reutlingen/validation.py` & `parkapi_sources-0.3.1/src/parkapi_sources/converters/reutlingen/validation.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.0/src/parkapi_sources/converters/reutlingen_bike/converter.py` & `parkapi_sources-0.3.1/src/parkapi_sources/converters/reutlingen_bike/converter.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 
 class ReutlingenBikePushConverter(CsvConverter):
     proj: pyproj.Proj = pyproj.Proj(proj='utm', zone=32, ellps='WGS84', preserve_units=True)
     reutlingen_bike_row_validator = DataclassValidator(ReutlingenBikeRowInput)
 
     source_info = SourceInfo(
-        uid='reutlingen',
+        uid='reutlingen_bike',
         name='Stadt Reutlingen: Fahrrad-Abstellanlagen',
         public_url='https://www.reutlingen.de',
         has_realtime_data=False,
     )
 
     header_mapping: dict[str, str] = {
         '\ufeffSTANDORT': 'name',
```

### Comparing `parkapi_sources-0.3.0/src/parkapi_sources/converters/reutlingen_bike/validation.py` & `parkapi_sources-0.3.1/src/parkapi_sources/converters/reutlingen_bike/validation.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.0/src/parkapi_sources/converters/stuttgart/converter.py` & `parkapi_sources-0.3.1/src/parkapi_sources/converters/stuttgart/converter.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.0/src/parkapi_sources/converters/ulm/converter.py` & `parkapi_sources-0.3.1/src/parkapi_sources/converters/ulm/converter.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.0/src/parkapi_sources/converters/vrs_p_r/vrs_p_r.py` & `parkapi_sources-0.3.1/src/parkapi_sources/converters/vrs_p_r/vrs_p_r.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.0/src/parkapi_sources/exceptions.py` & `parkapi_sources-0.3.1/src/parkapi_sources/exceptions.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.0/src/parkapi_sources/models/enums.py` & `parkapi_sources-0.3.1/src/parkapi_sources/models/enums.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.0/src/parkapi_sources/models/parking_site_inputs.py` & `parkapi_sources-0.3.1/src/parkapi_sources/models/parking_site_inputs.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.0/src/parkapi_sources/models/source_info.py` & `parkapi_sources-0.3.1/src/parkapi_sources/models/source_info.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.0/src/parkapi_sources/models/xlsx_inputs.py` & `parkapi_sources-0.3.1/src/parkapi_sources/models/xlsx_inputs.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.0/src/parkapi_sources/parkapi_sources.py` & `parkapi_sources-0.3.1/src/parkapi_sources/parkapi_sources.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,14 +19,15 @@
     KienzlerPullConverter,
     MannheimPushConverter,
     NeckarsulmBikePushConverter,
     NeckarsulmPushConverter,
     PbwPullConverter,
     PforzheimPushConverter,
     PumBwPushConverter,
+    ReutlingenBikePushConverter,
     ReutlingenPushConverter,
     StuttgartPushConverter,
     UlmPullConverter,
     VrsParkAndRidePushConverter,
 )
 from .converters.base_converter.pull import PullConverter
 from .converters.base_converter.push import PushConverter
@@ -49,14 +50,15 @@
         MannheimPushConverter,
         NeckarsulmBikePushConverter,
         NeckarsulmPushConverter,
         PbwPullConverter,
         PforzheimPushConverter,
         PumBwPushConverter,
         ReutlingenPushConverter,
+        ReutlingenBikePushConverter,
         StuttgartPushConverter,
         UlmPullConverter,
         VrsParkAndRidePushConverter,
     ]
     config_helper: ConfigHelper
     converter_by_uid: dict[str, BaseConverter]
```

### Comparing `parkapi_sources-0.3.0/src/parkapi_sources/scripts/parkapi.py` & `parkapi_sources-0.3.1/src/parkapi_sources/scripts/parkapi.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.0/src/parkapi_sources/util/encoding.py` & `parkapi_sources-0.3.1/src/parkapi_sources/util/encoding.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.0/src/parkapi_sources/util/xml_helper.py` & `parkapi_sources-0.3.1/src/parkapi_sources/util/xml_helper.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.0/src/parkapi_sources/validators/__init__.py` & `parkapi_sources-0.3.1/src/parkapi_sources/validators/__init__.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.0/src/parkapi_sources/validators/boolean_validators.py` & `parkapi_sources-0.3.1/src/parkapi_sources/validators/boolean_validators.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.0/src/parkapi_sources/validators/date_validator.py` & `parkapi_sources-0.3.1/src/parkapi_sources/validators/date_validator.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.0/src/parkapi_sources/validators/datetime_validator.py` & `parkapi_sources-0.3.1/src/parkapi_sources/validators/datetime_validator.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.0/src/parkapi_sources/validators/integer_validators.py` & `parkapi_sources-0.3.1/src/parkapi_sources/validators/integer_validators.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.0/src/parkapi_sources/validators/list_validator.py` & `parkapi_sources-0.3.1/src/parkapi_sources/validators/list_validator.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.0/src/parkapi_sources/validators/noneable.py` & `parkapi_sources-0.3.1/src/parkapi_sources/validators/noneable.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.0/src/parkapi_sources/validators/string_validators.py` & `parkapi_sources-0.3.1/src/parkapi_sources/validators/string_validators.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.0/src/parkapi_sources.egg-info/PKG-INFO` & `parkapi_sources-0.3.1/src/parkapi_sources.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: parkapi_sources
-Version: 0.3.0
+Version: 0.3.1
 Summary: ParkAPI Sources is a collection of converters from several different data sources to normalized ParkAPI data.
 Author-email: "Ernesto Ruge, binary butterfly GmbH" <ernesto.ruge@binary-butterfly.de>
 Maintainer-email: "Ernesto Ruge, binary butterfly GmbH" <ernesto.ruge@binary-butterfly.de>
 Keywords: data,parking,converter,mobility,car,bike
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `parkapi_sources-0.3.0/src/parkapi_sources.egg-info/SOURCES.txt` & `parkapi_sources-0.3.1/src/parkapi_sources.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.0/tests/converters/bahn_v2_test.py` & `parkapi_sources-0.3.1/tests/converters/bahn_v2_test.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.0/tests/converters/bfrk_bw_test.py` & `parkapi_sources-0.3.1/tests/converters/bfrk_bw_test.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.0/tests/converters/conftest.py` & `parkapi_sources-0.3.1/tests/converters/conftest.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.0/tests/converters/data/bahn_v2.json` & `parkapi_sources-0.3.1/tests/converters/data/bahn_v2.json`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.0/tests/converters/data/bfrk_bw_bike.csv` & `parkapi_sources-0.3.1/tests/converters/data/bfrk_bw_bike.csv`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.0/tests/converters/data/bfrk_bw_car.csv` & `parkapi_sources-0.3.1/tests/converters/data/bfrk_bw_car.csv`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.0/tests/converters/data/buchen.json` & `parkapi_sources-0.3.1/tests/converters/data/buchen.json`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.0/tests/converters/data/freiburg.json` & `parkapi_sources-0.3.1/tests/converters/data/freiburg.json`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.0/tests/converters/data/heidelberg.json` & `parkapi_sources-0.3.1/tests/converters/data/heidelberg.json`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.0/tests/converters/data/karlsruhe.json` & `parkapi_sources-0.3.1/tests/converters/data/karlsruhe.json`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.0/tests/converters/data/kienzler.json` & `parkapi_sources-0.3.1/tests/converters/data/kienzler.json`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.0/tests/converters/data/mannheim.json` & `parkapi_sources-0.3.1/tests/converters/data/mannheim.json`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.0/tests/converters/data/neckarsulm.csv` & `parkapi_sources-0.3.1/tests/converters/data/neckarsulm.csv`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.0/tests/converters/data/neckarsulm_bike.csv` & `parkapi_sources-0.3.1/tests/converters/data/neckarsulm_bike.csv`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.0/tests/converters/data/pbw/catalog-city.json` & `parkapi_sources-0.3.1/tests/converters/data/pbw/catalog-city.json`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.0/tests/converters/data/pbw/object-by-city-10.json` & `parkapi_sources-0.3.1/tests/converters/data/pbw/object-by-city-10.json`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.0/tests/converters/data/pbw/object-by-city-11.json` & `parkapi_sources-0.3.1/tests/converters/data/pbw/object-by-city-11.json`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.0/tests/converters/data/pbw/object-by-city-12.json` & `parkapi_sources-0.3.1/tests/converters/data/pbw/object-by-city-12.json`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.0/tests/converters/data/pbw/object-by-city-15.json` & `parkapi_sources-0.3.1/tests/converters/data/pbw/object-by-city-15.json`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.0/tests/converters/data/pbw/object-by-city-17.json` & `parkapi_sources-0.3.1/tests/converters/data/pbw/object-by-city-17.json`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.0/tests/converters/data/pbw/object-by-city-18.json` & `parkapi_sources-0.3.1/tests/converters/data/pbw/object-by-city-18.json`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.0/tests/converters/data/pbw/object-by-city-19.json` & `parkapi_sources-0.3.1/tests/converters/data/pbw/object-by-city-19.json`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.0/tests/converters/data/pbw/object-by-city-31.json` & `parkapi_sources-0.3.1/tests/converters/data/pbw/object-by-city-31.json`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.0/tests/converters/data/pbw/object-by-city-32.json` & `parkapi_sources-0.3.1/tests/converters/data/pbw/object-by-city-32.json`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.0/tests/converters/data/pbw/object-by-city-33.json` & `parkapi_sources-0.3.1/tests/converters/data/pbw/object-by-city-33.json`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.0/tests/converters/data/pbw/object-by-city-34.json` & `parkapi_sources-0.3.1/tests/converters/data/pbw/object-by-city-34.json`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.0/tests/converters/data/pbw/object-by-city-4.json` & `parkapi_sources-0.3.1/tests/converters/data/pbw/object-by-city-4.json`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.0/tests/converters/data/pbw/object-by-city-42.json` & `parkapi_sources-0.3.1/tests/converters/data/pbw/object-by-city-42.json`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.0/tests/converters/data/pbw/object-by-city-48.json` & `parkapi_sources-0.3.1/tests/converters/data/pbw/object-by-city-48.json`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.0/tests/converters/data/pbw/object-by-city-49.json` & `parkapi_sources-0.3.1/tests/converters/data/pbw/object-by-city-49.json`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.0/tests/converters/data/pbw/object-by-city-51.json` & `parkapi_sources-0.3.1/tests/converters/data/pbw/object-by-city-51.json`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.0/tests/converters/data/pbw/object-by-city-52.json` & `parkapi_sources-0.3.1/tests/converters/data/pbw/object-by-city-52.json`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.0/tests/converters/data/pbw/object-by-city-60.json` & `parkapi_sources-0.3.1/tests/converters/data/pbw/object-by-city-60.json`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.0/tests/converters/data/pbw/object-by-city-61.json` & `parkapi_sources-0.3.1/tests/converters/data/pbw/object-by-city-61.json`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.0/tests/converters/data/pbw/object-by-city-7.json` & `parkapi_sources-0.3.1/tests/converters/data/pbw/object-by-city-7.json`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.0/tests/converters/data/pbw/object-by-city-71.json` & `parkapi_sources-0.3.1/tests/converters/data/pbw/object-by-city-71.json`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.0/tests/converters/data/pbw/object-by-city-9.json` & `parkapi_sources-0.3.1/tests/converters/data/pbw/object-by-city-9.json`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.0/tests/converters/data/pbw/object-dynamic-all.json` & `parkapi_sources-0.3.1/tests/converters/data/pbw/object-dynamic-all.json`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.0/tests/converters/data/pforzheim.json` & `parkapi_sources-0.3.1/tests/converters/data/pforzheim.json`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.0/tests/converters/data/pum_bw.xlsx` & `parkapi_sources-0.3.1/tests/converters/data/pum_bw.xlsx`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.0/tests/converters/data/reutlingen.csv` & `parkapi_sources-0.3.1/tests/converters/data/reutlingen.csv`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.0/tests/converters/data/reutlingen_bike.csv` & `parkapi_sources-0.3.1/tests/converters/data/reutlingen_bike.csv`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.0/tests/converters/data/stuttgart-realtime.xml` & `parkapi_sources-0.3.1/tests/converters/data/stuttgart-realtime.xml`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.0/tests/converters/data/stuttgart-static.xml` & `parkapi_sources-0.3.1/tests/converters/data/stuttgart-static.xml`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.0/tests/converters/data/ulm.html` & `parkapi_sources-0.3.1/tests/converters/data/ulm.html`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.0/tests/converters/data/vrs_p_r.xlsx` & `parkapi_sources-0.3.1/tests/converters/data/vrs_p_r.xlsx`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.0/tests/converters/freiburg_test.py` & `parkapi_sources-0.3.1/tests/converters/freiburg_test.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.0/tests/converters/heidelberg_test.py` & `parkapi_sources-0.3.1/tests/converters/heidelberg_test.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.0/tests/converters/helper.py` & `parkapi_sources-0.3.1/tests/converters/helper.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.0/tests/converters/karlsruhe_test.py` & `parkapi_sources-0.3.1/tests/converters/karlsruhe_test.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.0/tests/converters/kienzler_test.py` & `parkapi_sources-0.3.1/tests/converters/kienzler_test.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.0/tests/converters/mannheim_buchen_test.py` & `parkapi_sources-0.3.1/tests/converters/mannheim_buchen_test.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.0/tests/converters/neckarsulm_bike_test.py` & `parkapi_sources-0.3.1/tests/converters/neckarsulm_bike_test.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.0/tests/converters/neckarsulm_test.py` & `parkapi_sources-0.3.1/tests/converters/neckarsulm_test.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.0/tests/converters/pbw_test.py` & `parkapi_sources-0.3.1/tests/converters/pbw_test.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.0/tests/converters/pforzheim_test.py` & `parkapi_sources-0.3.1/tests/converters/pforzheim_test.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.0/tests/converters/pum_bw_test.py` & `parkapi_sources-0.3.1/tests/converters/pum_bw_test.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.0/tests/converters/reutlingen_bike_test.py` & `parkapi_sources-0.3.1/tests/converters/reutlingen_bike_test.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.0/tests/converters/reutlingen_test.py` & `parkapi_sources-0.3.1/tests/converters/reutlingen_test.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.0/tests/converters/stuttgart_test.py` & `parkapi_sources-0.3.1/tests/converters/stuttgart_test.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.0/tests/converters/ulm_test.py` & `parkapi_sources-0.3.1/tests/converters/ulm_test.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.0/tests/converters/vrs_p_r_test.py` & `parkapi_sources-0.3.1/tests/converters/vrs_p_r_test.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.0/tests/models/xlsx_inputs_test.py` & `parkapi_sources-0.3.1/tests/models/xlsx_inputs_test.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.0/tests/util/data_xml_helper.py` & `parkapi_sources-0.3.1/tests/util/data_xml_helper.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.0/tests/util/encoding_test.py` & `parkapi_sources-0.3.1/tests/util/encoding_test.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.0/tests/util/xml_helper_test.py` & `parkapi_sources-0.3.1/tests/util/xml_helper_test.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.0/tests/validators/boolean_validators_test.py` & `parkapi_sources-0.3.1/tests/validators/boolean_validators_test.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.0/tests/validators/date_validators_test.py` & `parkapi_sources-0.3.1/tests/validators/date_validators_test.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.0/tests/validators/datetime_validators_test.py` & `parkapi_sources-0.3.1/tests/validators/datetime_validators_test.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.0/tests/validators/integer_validators_test.py` & `parkapi_sources-0.3.1/tests/validators/integer_validators_test.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.0/tests/validators/noneable_tests.py` & `parkapi_sources-0.3.1/tests/validators/noneable_tests.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.0/tests/validators/string_validators_test.py` & `parkapi_sources-0.3.1/tests/validators/string_validators_test.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.0/tests/validators/time_validators_test.py` & `parkapi_sources-0.3.1/tests/validators/time_validators_test.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.0/tox.ini` & `parkapi_sources-0.3.1/tox.ini`

 * *Files identical despite different names*

