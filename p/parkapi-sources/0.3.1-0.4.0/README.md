# Comparing `tmp/parkapi_sources-0.3.1.tar.gz` & `tmp/parkapi_sources-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "parkapi_sources-0.3.1.tar", last modified: Fri May  3 11:23:42 2024, max compression
+gzip compressed data, was "parkapi_sources-0.4.0.tar", last modified: Thu May 16 06:35:38 2024, max compression
```

## Comparing `parkapi_sources-0.3.1.tar` & `parkapi_sources-0.4.0.tar`

### file list

```diff
@@ -1,236 +1,253 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:23:42.152560 parkapi_sources-0.3.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:23:42.116559 parkapi_sources-0.3.1/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:23:42.116559 parkapi_sources-0.3.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2297 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/.github/workflows/build-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1469 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/.github/workflows/lint-test.yml
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      871 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/LICENCE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      381 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)    16246 2024-05-03 11:23:42.152560 parkapi_sources-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    14713 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:23:42.116559 parkapi_sources-0.3.1/data/
--rw-r--r--   0 runner    (1001) docker     (127)    11453 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/data/freiburg.geojson
--rw-r--r--   0 runner    (1001) docker     (127)    11994 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/data/heidelberg.geojson
--rw-r--r--   0 runner    (1001) docker     (127)    10851 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/data/mannheim.geojson
--rw-r--r--   0 runner    (1001) docker     (127)     5300 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/data/ulm.geojson
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:23:42.116559 parkapi_sources-0.3.1/dev/
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/dev/parkapi.py
--rw-r--r--   0 runner    (1001) docker     (127)     3147 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/dev/test-pull-converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     4282 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/dev/test-push-converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3279 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 11:23:42.152560 parkapi_sources-0.3.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:23:42.112559 parkapi_sources-0.3.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:23:42.120559 parkapi_sources-0.3.1/src/parkapi_sources/
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/src/parkapi_sources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-03 11:23:41.000000 parkapi_sources-0.3.1/src/parkapi_sources/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:23:42.120559 parkapi_sources-0.3.1/src/parkapi_sources/converters/
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/src/parkapi_sources/converters/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:23:42.120559 parkapi_sources-0.3.1/src/parkapi_sources/converters/bahn_v2/
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/src/parkapi_sources/converters/bahn_v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3117 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/src/parkapi_sources/converters/bahn_v2/converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1823 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/src/parkapi_sources/converters/bahn_v2/mapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     3885 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/src/parkapi_sources/converters/bahn_v2/validators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:23:42.120559 parkapi_sources-0.3.1/src/parkapi_sources/converters/base_converter/
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/src/parkapi_sources/converters/base_converter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      829 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/src/parkapi_sources/converters/base_converter/base_converter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:23:42.120559 parkapi_sources-0.3.1/src/parkapi_sources/converters/base_converter/pull/
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/src/parkapi_sources/converters/base_converter/pull/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      729 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/src/parkapi_sources/converters/base_converter/pull/pull_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2809 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/src/parkapi_sources/converters/base_converter/pull/pull_scraper_mixin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:23:42.120559 parkapi_sources-0.3.1/src/parkapi_sources/converters/base_converter/pull/static_geojson_data_mixin/
--rw-r--r--   0 runner    (1001) docker     (127)      248 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/src/parkapi_sources/converters/base_converter/pull/static_geojson_data_mixin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3302 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/src/parkapi_sources/converters/base_converter/pull/static_geojson_data_mixin/mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     2207 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/src/parkapi_sources/converters/base_converter/pull/static_geojson_data_mixin/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:23:42.124559 parkapi_sources-0.3.1/src/parkapi_sources/converters/base_converter/push/
--rw-r--r--   0 runner    (1001) docker     (127)      481 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/src/parkapi_sources/converters/base_converter/push/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1478 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/src/parkapi_sources/converters/base_converter/push/csv_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)      649 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/src/parkapi_sources/converters/base_converter/push/json_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     4937 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/src/parkapi_sources/converters/base_converter/push/normalized_xlsx_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3089 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/src/parkapi_sources/converters/base_converter/push/parkapi_json_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/src/parkapi_sources/converters/base_converter/push/push_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1659 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/src/parkapi_sources/converters/base_converter/push/xlsx_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)      725 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/src/parkapi_sources/converters/base_converter/push/xml_converter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:23:42.124559 parkapi_sources-0.3.1/src/parkapi_sources/converters/bfrk_bw/
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/src/parkapi_sources/converters/bfrk_bw/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2061 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/src/parkapi_sources/converters/bfrk_bw/base_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2026 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/src/parkapi_sources/converters/bfrk_bw/base_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     1644 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/src/parkapi_sources/converters/bfrk_bw/bike_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2039 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/src/parkapi_sources/converters/bfrk_bw/bike_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     1628 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/src/parkapi_sources/converters/bfrk_bw/car_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1763 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/src/parkapi_sources/converters/bfrk_bw/car_models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:23:42.124559 parkapi_sources-0.3.1/src/parkapi_sources/converters/freiburg/
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/src/parkapi_sources/converters/freiburg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3061 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/src/parkapi_sources/converters/freiburg/converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1688 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/src/parkapi_sources/converters/freiburg/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:23:42.124559 parkapi_sources-0.3.1/src/parkapi_sources/converters/heidelberg/
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/src/parkapi_sources/converters/heidelberg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3458 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/src/parkapi_sources/converters/heidelberg/converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1970 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/src/parkapi_sources/converters/heidelberg/validators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:23:42.124559 parkapi_sources-0.3.1/src/parkapi_sources/converters/karlsruhe/
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/src/parkapi_sources/converters/karlsruhe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4312 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/src/parkapi_sources/converters/karlsruhe/converter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:23:42.124559 parkapi_sources-0.3.1/src/parkapi_sources/converters/karlsruhe/files/
--rw-r--r--   0 runner    (1001) docker     (127)     2933 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/src/parkapi_sources/converters/karlsruhe/files/ca.crt.pem
--rw-r--r--   0 runner    (1001) docker     (127)     4253 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/src/parkapi_sources/converters/karlsruhe/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:23:42.124559 parkapi_sources-0.3.1/src/parkapi_sources/converters/kienzler/
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/src/parkapi_sources/converters/kienzler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3531 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/src/parkapi_sources/converters/kienzler/converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1607 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/src/parkapi_sources/converters/kienzler/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:23:42.128559 parkapi_sources-0.3.1/src/parkapi_sources/converters/mannheim_buchen/
--rw-r--r--   0 runner    (1001) docker     (127)      210 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/src/parkapi_sources/converters/mannheim_buchen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2855 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/src/parkapi_sources/converters/mannheim_buchen/converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3452 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/src/parkapi_sources/converters/mannheim_buchen/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:23:42.128559 parkapi_sources-0.3.1/src/parkapi_sources/converters/neckarsulm/
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/src/parkapi_sources/converters/neckarsulm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2715 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/src/parkapi_sources/converters/neckarsulm/converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3263 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/src/parkapi_sources/converters/neckarsulm/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:23:42.128559 parkapi_sources-0.3.1/src/parkapi_sources/converters/neckarsulm_bike/
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/src/parkapi_sources/converters/neckarsulm_bike/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3333 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/src/parkapi_sources/converters/neckarsulm_bike/converter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:23:42.128559 parkapi_sources-0.3.1/src/parkapi_sources/converters/pbw/
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/src/parkapi_sources/converters/pbw/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4889 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/src/parkapi_sources/converters/pbw/converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2554 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/src/parkapi_sources/converters/pbw/mapper.py
--rw-r--r--   0 runner    (1001) docker     (127)    11699 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/src/parkapi_sources/converters/pbw/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:23:42.128559 parkapi_sources-0.3.1/src/parkapi_sources/converters/pforzheim/
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/src/parkapi_sources/converters/pforzheim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2669 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/src/parkapi_sources/converters/pforzheim/converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1836 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/src/parkapi_sources/converters/pforzheim/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:23:42.128559 parkapi_sources-0.3.1/src/parkapi_sources/converters/pum_bw/
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/src/parkapi_sources/converters/pum_bw/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2970 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/src/parkapi_sources/converters/pum_bw/converter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:23:42.128559 parkapi_sources-0.3.1/src/parkapi_sources/converters/reutlingen/
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/src/parkapi_sources/converters/reutlingen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2573 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/src/parkapi_sources/converters/reutlingen/converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1805 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/src/parkapi_sources/converters/reutlingen/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:23:42.128559 parkapi_sources-0.3.1/src/parkapi_sources/converters/reutlingen_bike/
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/src/parkapi_sources/converters/reutlingen_bike/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2825 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/src/parkapi_sources/converters/reutlingen_bike/converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/src/parkapi_sources/converters/reutlingen_bike/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:23:42.128559 parkapi_sources-0.3.1/src/parkapi_sources/converters/stuttgart/
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/src/parkapi_sources/converters/stuttgart/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6424 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/src/parkapi_sources/converters/stuttgart/converter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:23:42.132559 parkapi_sources-0.3.1/src/parkapi_sources/converters/ulm/
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/src/parkapi_sources/converters/ulm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2316 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/src/parkapi_sources/converters/ulm/converter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:23:42.132559 parkapi_sources-0.3.1/src/parkapi_sources/converters/vrs_p_r/
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/src/parkapi_sources/converters/vrs_p_r/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2276 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/src/parkapi_sources/converters/vrs_p_r/vrs_p_r.py
--rw-r--r--   0 runner    (1001) docker     (127)     1288 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/src/parkapi_sources/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:23:42.132559 parkapi_sources-0.3.1/src/parkapi_sources/models/
--rw-r--r--   0 runner    (1001) docker     (127)      338 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/src/parkapi_sources/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/src/parkapi_sources/models/enums.py
--rw-r--r--   0 runner    (1001) docker     (127)     7717 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/src/parkapi_sources/models/parking_site_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)      661 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/src/parkapi_sources/models/source_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     4413 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/src/parkapi_sources/models/xlsx_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     3392 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/src/parkapi_sources/parkapi_sources.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:23:42.132559 parkapi_sources-0.3.1/src/parkapi_sources/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)     9093 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/src/parkapi_sources/scripts/parkapi.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:23:42.132559 parkapi_sources-0.3.1/src/parkapi_sources/util/
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/src/parkapi_sources/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/src/parkapi_sources/util/config_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/src/parkapi_sources/util/encoding.py
--rw-r--r--   0 runner    (1001) docker     (127)    10420 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/src/parkapi_sources/util/xml_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:23:42.132559 parkapi_sources-0.3.1/src/parkapi_sources/validators/
--rw-r--r--   0 runner    (1001) docker     (127)      675 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/src/parkapi_sources/validators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      704 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/src/parkapi_sources/validators/boolean_validators.py
--rw-r--r--   0 runner    (1001) docker     (127)      899 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/src/parkapi_sources/validators/date_validator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/src/parkapi_sources/validators/datetime_validator.py
--rw-r--r--   0 runner    (1001) docker     (127)      511 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/src/parkapi_sources/validators/decimal_validators.py
--rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/src/parkapi_sources/validators/integer_validators.py
--rw-r--r--   0 runner    (1001) docker     (127)      831 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/src/parkapi_sources/validators/list_validator.py
--rw-r--r--   0 runner    (1001) docker     (127)      743 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/src/parkapi_sources/validators/noneable.py
--rw-r--r--   0 runner    (1001) docker     (127)      994 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/src/parkapi_sources/validators/string_validators.py
--rw-r--r--   0 runner    (1001) docker     (127)      473 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/src/parkapi_sources/validators/time_validators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:23:42.148559 parkapi_sources-0.3.1/src/parkapi_sources.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    16246 2024-05-03 11:23:42.000000 parkapi_sources-0.3.1/src/parkapi_sources.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8603 2024-05-03 11:23:42.000000 parkapi_sources-0.3.1/src/parkapi_sources.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 11:23:42.000000 parkapi_sources-0.3.1/src/parkapi_sources.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-03 11:23:42.000000 parkapi_sources-0.3.1/src/parkapi_sources.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-03 11:23:42.000000 parkapi_sources-0.3.1/src/parkapi_sources.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:23:42.136559 parkapi_sources-0.3.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      320 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:23:42.136559 parkapi_sources-0.3.1/tests/converters/
--rw-r--r--   0 runner    (1001) docker     (127)     1744 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/tests/converters/bahn_v2_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2053 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/tests/converters/bfrk_bw_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      823 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/tests/converters/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:23:42.144559 parkapi_sources-0.3.1/tests/converters/data/
--rw-r--r--   0 runner    (1001) docker     (127)   947589 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/tests/converters/data/bahn_v2.json
--rw-r--r--   0 runner    (1001) docker     (127)   552854 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/tests/converters/data/bfrk_bw_bike.csv
--rw-r--r--   0 runner    (1001) docker     (127)   617384 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/tests/converters/data/bfrk_bw_car.csv
--rw-r--r--   0 runner    (1001) docker     (127)      802 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/tests/converters/data/buchen.json
--rw-r--r--   0 runner    (1001) docker     (127)    12651 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/tests/converters/data/freiburg.json
--rw-r--r--   0 runner    (1001) docker     (127)     3681 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/tests/converters/data/heidelberg.json
--rw-r--r--   0 runner    (1001) docker     (127)    63706 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/tests/converters/data/karlsruhe.json
--rw-r--r--   0 runner    (1001) docker     (127)     3477 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/tests/converters/data/kienzler.json
--rw-r--r--   0 runner    (1001) docker     (127)    18474 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/tests/converters/data/mannheim.json
--rw-r--r--   0 runner    (1001) docker     (127)    20667 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/tests/converters/data/neckarsulm.csv
--rw-r--r--   0 runner    (1001) docker     (127)    18115 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/tests/converters/data/neckarsulm_bike.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:23:42.148559 parkapi_sources-0.3.1/tests/converters/data/pbw/
--rw-r--r--   0 runner    (1001) docker     (127)     1251 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/tests/converters/data/pbw/catalog-city.json
--rw-r--r--   0 runner    (1001) docker     (127)   114816 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/tests/converters/data/pbw/object-by-city-10.json
--rw-r--r--   0 runner    (1001) docker     (127)     5061 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/tests/converters/data/pbw/object-by-city-11.json
--rw-r--r--   0 runner    (1001) docker     (127)    36083 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/tests/converters/data/pbw/object-by-city-12.json
--rw-r--r--   0 runner    (1001) docker     (127)     1784 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/tests/converters/data/pbw/object-by-city-15.json
--rw-r--r--   0 runner    (1001) docker     (127)     6859 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/tests/converters/data/pbw/object-by-city-17.json
--rw-r--r--   0 runner    (1001) docker     (127)     7122 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/tests/converters/data/pbw/object-by-city-18.json
--rw-r--r--   0 runner    (1001) docker     (127)     5812 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/tests/converters/data/pbw/object-by-city-19.json
--rw-r--r--   0 runner    (1001) docker     (127)     5795 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/tests/converters/data/pbw/object-by-city-31.json
--rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/tests/converters/data/pbw/object-by-city-32.json
--rw-r--r--   0 runner    (1001) docker     (127)     6650 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/tests/converters/data/pbw/object-by-city-33.json
--rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/tests/converters/data/pbw/object-by-city-34.json
--rw-r--r--   0 runner    (1001) docker     (127)     3225 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/tests/converters/data/pbw/object-by-city-4.json
--rw-r--r--   0 runner    (1001) docker     (127)     3187 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/tests/converters/data/pbw/object-by-city-42.json
--rw-r--r--   0 runner    (1001) docker     (127)     3296 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/tests/converters/data/pbw/object-by-city-48.json
--rw-r--r--   0 runner    (1001) docker     (127)     1597 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/tests/converters/data/pbw/object-by-city-49.json
--rw-r--r--   0 runner    (1001) docker     (127)     3241 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/tests/converters/data/pbw/object-by-city-51.json
--rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/tests/converters/data/pbw/object-by-city-52.json
--rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/tests/converters/data/pbw/object-by-city-60.json
--rw-r--r--   0 runner    (1001) docker     (127)     1557 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/tests/converters/data/pbw/object-by-city-61.json
--rw-r--r--   0 runner    (1001) docker     (127)    14227 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/tests/converters/data/pbw/object-by-city-7.json
--rw-r--r--   0 runner    (1001) docker     (127)     3149 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/tests/converters/data/pbw/object-by-city-71.json
--rw-r--r--   0 runner    (1001) docker     (127)     7071 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/tests/converters/data/pbw/object-by-city-9.json
--rw-r--r--   0 runner    (1001) docker     (127)     6685 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/tests/converters/data/pbw/object-dynamic-all.json
--rw-r--r--   0 runner    (1001) docker     (127)    18956 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/tests/converters/data/pforzheim.json
--rw-r--r--   0 runner    (1001) docker     (127)    30849 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/tests/converters/data/pum_bw.xlsx
--rw-r--r--   0 runner    (1001) docker     (127)     9387 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/tests/converters/data/reutlingen.csv
--rw-r--r--   0 runner    (1001) docker     (127)    27295 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/tests/converters/data/reutlingen_bike.csv
--rw-r--r--   0 runner    (1001) docker     (127)    35423 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/tests/converters/data/stuttgart-realtime.xml
--rw-r--r--   0 runner    (1001) docker     (127)   218959 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/tests/converters/data/stuttgart-static.xml
--rw-r--r--   0 runner    (1001) docker     (127)    62841 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/tests/converters/data/ulm.html
--rw-r--r--   0 runner    (1001) docker     (127)   136171 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/tests/converters/data/vrs_p_r.xlsx
--rw-r--r--   0 runner    (1001) docker     (127)     1859 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/tests/converters/freiburg_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2226 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/tests/converters/heidelberg_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2439 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/tests/converters/helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     1926 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/tests/converters/karlsruhe_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/tests/converters/kienzler_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2523 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/tests/converters/mannheim_buchen_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/tests/converters/neckarsulm_bike_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/tests/converters/neckarsulm_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2880 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/tests/converters/pbw_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/tests/converters/pforzheim_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/tests/converters/pum_bw_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1246 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/tests/converters/reutlingen_bike_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/tests/converters/reutlingen_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1949 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/tests/converters/stuttgart_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1777 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/tests/converters/ulm_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/tests/converters/vrs_p_r_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:23:42.148559 parkapi_sources-0.3.1/tests/models/
--rw-r--r--   0 runner    (1001) docker     (127)     2183 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/tests/models/xlsx_inputs_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:23:42.148559 parkapi_sources-0.3.1/tests/util/
--rw-r--r--   0 runner    (1001) docker     (127)     4105 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/tests/util/data_xml_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     1706 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/tests/util/encoding_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     4039 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/tests/util/xml_helper_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:23:42.148559 parkapi_sources-0.3.1/tests/validators/
--rw-r--r--   0 runner    (1001) docker     (127)     1255 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/tests/validators/boolean_validators_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/tests/validators/date_validators_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2108 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/tests/validators/datetime_validators_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/tests/validators/integer_validators_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/tests/validators/noneable_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/tests/validators/string_validators_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      567 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/tests/validators/time_validators_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-03 11:23:36.000000 parkapi_sources-0.3.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 06:35:38.151497 parkapi_sources-0.4.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 06:35:38.107496 parkapi_sources-0.4.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 06:35:38.107496 parkapi_sources-0.4.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2297 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/.github/workflows/build-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1469 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/.github/workflows/lint-test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1589 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/LICENCE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      381 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)    16681 2024-05-16 06:35:38.151497 parkapi_sources-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    15147 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 06:35:38.107496 parkapi_sources-0.4.0/data/
+-rw-r--r--   0 runner    (1001) docker     (127)    11453 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/data/freiburg.geojson
+-rw-r--r--   0 runner    (1001) docker     (127)    11994 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/data/heidelberg.geojson
+-rw-r--r--   0 runner    (1001) docker     (127)    10851 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/data/mannheim.geojson
+-rw-r--r--   0 runner    (1001) docker     (127)     5300 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/data/ulm.geojson
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 06:35:38.107496 parkapi_sources-0.4.0/dev/
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/dev/parkapi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3147 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/dev/test-pull-converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4282 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/dev/test-push-converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3280 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 06:35:38.151497 parkapi_sources-0.4.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 06:35:38.099496 parkapi_sources-0.4.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 06:35:38.111496 parkapi_sources-0.4.0/src/parkapi_sources/
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/src/parkapi_sources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-16 06:35:37.000000 parkapi_sources-0.4.0/src/parkapi_sources/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 06:35:38.111496 parkapi_sources-0.4.0/src/parkapi_sources/converters/
+-rw-r--r--   0 runner    (1001) docker     (127)     1247 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/src/parkapi_sources/converters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 06:35:38.111496 parkapi_sources-0.4.0/src/parkapi_sources/converters/bahn_v2/
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/src/parkapi_sources/converters/bahn_v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3117 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/src/parkapi_sources/converters/bahn_v2/converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1823 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/src/parkapi_sources/converters/bahn_v2/mapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3885 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/src/parkapi_sources/converters/bahn_v2/validators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 06:35:38.111496 parkapi_sources-0.4.0/src/parkapi_sources/converters/base_converter/
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/src/parkapi_sources/converters/base_converter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      829 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/src/parkapi_sources/converters/base_converter/base_converter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 06:35:38.111496 parkapi_sources-0.4.0/src/parkapi_sources/converters/base_converter/pull/
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/src/parkapi_sources/converters/base_converter/pull/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      729 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/src/parkapi_sources/converters/base_converter/pull/pull_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2809 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/src/parkapi_sources/converters/base_converter/pull/pull_scraper_mixin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 06:35:38.111496 parkapi_sources-0.4.0/src/parkapi_sources/converters/base_converter/pull/static_geojson_data_mixin/
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/src/parkapi_sources/converters/base_converter/pull/static_geojson_data_mixin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3302 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/src/parkapi_sources/converters/base_converter/pull/static_geojson_data_mixin/mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2207 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/src/parkapi_sources/converters/base_converter/pull/static_geojson_data_mixin/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 06:35:38.115496 parkapi_sources-0.4.0/src/parkapi_sources/converters/base_converter/push/
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/src/parkapi_sources/converters/base_converter/push/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1518 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/src/parkapi_sources/converters/base_converter/push/csv_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/src/parkapi_sources/converters/base_converter/push/json_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4937 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/src/parkapi_sources/converters/base_converter/push/normalized_xlsx_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3089 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/src/parkapi_sources/converters/base_converter/push/parkapi_json_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/src/parkapi_sources/converters/base_converter/push/push_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1659 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/src/parkapi_sources/converters/base_converter/push/xlsx_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      725 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/src/parkapi_sources/converters/base_converter/push/xml_converter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 06:35:38.115496 parkapi_sources-0.4.0/src/parkapi_sources/converters/bfrk_bw/
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/src/parkapi_sources/converters/bfrk_bw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2061 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/src/parkapi_sources/converters/bfrk_bw/base_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2026 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/src/parkapi_sources/converters/bfrk_bw/base_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1644 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/src/parkapi_sources/converters/bfrk_bw/bike_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2039 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/src/parkapi_sources/converters/bfrk_bw/bike_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1628 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/src/parkapi_sources/converters/bfrk_bw/car_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1763 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/src/parkapi_sources/converters/bfrk_bw/car_models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 06:35:38.115496 parkapi_sources-0.4.0/src/parkapi_sources/converters/ellwangen/
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/src/parkapi_sources/converters/ellwangen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2102 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/src/parkapi_sources/converters/ellwangen/converter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 06:35:38.115496 parkapi_sources-0.4.0/src/parkapi_sources/converters/freiburg/
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/src/parkapi_sources/converters/freiburg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3061 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/src/parkapi_sources/converters/freiburg/converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1688 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/src/parkapi_sources/converters/freiburg/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 06:35:38.115496 parkapi_sources-0.4.0/src/parkapi_sources/converters/heidelberg/
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/src/parkapi_sources/converters/heidelberg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3458 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/src/parkapi_sources/converters/heidelberg/converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1970 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/src/parkapi_sources/converters/heidelberg/validators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 06:35:38.119496 parkapi_sources-0.4.0/src/parkapi_sources/converters/karlsruhe/
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/src/parkapi_sources/converters/karlsruhe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5434 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/src/parkapi_sources/converters/karlsruhe/converter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 06:35:38.119496 parkapi_sources-0.4.0/src/parkapi_sources/converters/karlsruhe/files/
+-rw-r--r--   0 runner    (1001) docker     (127)     2933 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/src/parkapi_sources/converters/karlsruhe/files/ca.crt.pem
+-rw-r--r--   0 runner    (1001) docker     (127)     6626 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/src/parkapi_sources/converters/karlsruhe/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 06:35:38.119496 parkapi_sources-0.4.0/src/parkapi_sources/converters/kienzler/
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/src/parkapi_sources/converters/kienzler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3531 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/src/parkapi_sources/converters/kienzler/converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1607 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/src/parkapi_sources/converters/kienzler/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 06:35:38.119496 parkapi_sources-0.4.0/src/parkapi_sources/converters/konstanz_bike/
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/src/parkapi_sources/converters/konstanz_bike/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2540 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/src/parkapi_sources/converters/konstanz_bike/converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3521 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/src/parkapi_sources/converters/konstanz_bike/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 06:35:38.119496 parkapi_sources-0.4.0/src/parkapi_sources/converters/mannheim_buchen/
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/src/parkapi_sources/converters/mannheim_buchen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/src/parkapi_sources/converters/mannheim_buchen/converter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 06:35:38.119496 parkapi_sources-0.4.0/src/parkapi_sources/converters/neckarsulm/
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/src/parkapi_sources/converters/neckarsulm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2715 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/src/parkapi_sources/converters/neckarsulm/converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3263 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/src/parkapi_sources/converters/neckarsulm/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 06:35:38.119496 parkapi_sources-0.4.0/src/parkapi_sources/converters/neckarsulm_bike/
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/src/parkapi_sources/converters/neckarsulm_bike/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3333 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/src/parkapi_sources/converters/neckarsulm_bike/converter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 06:35:38.119496 parkapi_sources-0.4.0/src/parkapi_sources/converters/pbw/
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/src/parkapi_sources/converters/pbw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4889 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/src/parkapi_sources/converters/pbw/converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2554 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/src/parkapi_sources/converters/pbw/mapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11699 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/src/parkapi_sources/converters/pbw/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 06:35:38.123496 parkapi_sources-0.4.0/src/parkapi_sources/converters/pforzheim/
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/src/parkapi_sources/converters/pforzheim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2744 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/src/parkapi_sources/converters/pforzheim/converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1836 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/src/parkapi_sources/converters/pforzheim/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 06:35:38.123496 parkapi_sources-0.4.0/src/parkapi_sources/converters/pum_bw/
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/src/parkapi_sources/converters/pum_bw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3096 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/src/parkapi_sources/converters/pum_bw/converter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 06:35:38.123496 parkapi_sources-0.4.0/src/parkapi_sources/converters/radvis_bw/
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/src/parkapi_sources/converters/radvis_bw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3558 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/src/parkapi_sources/converters/radvis_bw/converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5678 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/src/parkapi_sources/converters/radvis_bw/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 06:35:38.123496 parkapi_sources-0.4.0/src/parkapi_sources/converters/reutlingen/
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/src/parkapi_sources/converters/reutlingen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2573 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/src/parkapi_sources/converters/reutlingen/converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1805 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/src/parkapi_sources/converters/reutlingen/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 06:35:38.123496 parkapi_sources-0.4.0/src/parkapi_sources/converters/reutlingen_bike/
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/src/parkapi_sources/converters/reutlingen_bike/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2825 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/src/parkapi_sources/converters/reutlingen_bike/converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/src/parkapi_sources/converters/reutlingen_bike/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 06:35:38.123496 parkapi_sources-0.4.0/src/parkapi_sources/converters/stuttgart/
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/src/parkapi_sources/converters/stuttgart/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6424 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/src/parkapi_sources/converters/stuttgart/converter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 06:35:38.123496 parkapi_sources-0.4.0/src/parkapi_sources/converters/ulm/
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/src/parkapi_sources/converters/ulm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2316 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/src/parkapi_sources/converters/ulm/converter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 06:35:38.123496 parkapi_sources-0.4.0/src/parkapi_sources/converters/vrs_p_r/
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/src/parkapi_sources/converters/vrs_p_r/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2276 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/src/parkapi_sources/converters/vrs_p_r/vrs_p_r.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1288 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/src/parkapi_sources/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 06:35:38.127496 parkapi_sources-0.4.0/src/parkapi_sources/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/src/parkapi_sources/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/src/parkapi_sources/models/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8380 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/src/parkapi_sources/models/parking_site_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      661 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/src/parkapi_sources/models/source_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4332 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/src/parkapi_sources/models/xlsx_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3644 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/src/parkapi_sources/parkapi_sources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 06:35:38.127496 parkapi_sources-0.4.0/src/parkapi_sources/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)     9093 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/src/parkapi_sources/scripts/parkapi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 06:35:38.127496 parkapi_sources-0.4.0/src/parkapi_sources/util/
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/src/parkapi_sources/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/src/parkapi_sources/util/config_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/src/parkapi_sources/util/encoding.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10420 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/src/parkapi_sources/util/xml_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 06:35:38.127496 parkapi_sources-0.4.0/src/parkapi_sources/validators/
+-rw-r--r--   0 runner    (1001) docker     (127)      675 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/src/parkapi_sources/validators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      704 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/src/parkapi_sources/validators/boolean_validators.py
+-rw-r--r--   0 runner    (1001) docker     (127)      899 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/src/parkapi_sources/validators/date_validator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/src/parkapi_sources/validators/datetime_validator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      511 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/src/parkapi_sources/validators/decimal_validators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/src/parkapi_sources/validators/integer_validators.py
+-rw-r--r--   0 runner    (1001) docker     (127)      831 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/src/parkapi_sources/validators/list_validator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      743 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/src/parkapi_sources/validators/noneable.py
+-rw-r--r--   0 runner    (1001) docker     (127)      994 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/src/parkapi_sources/validators/string_validators.py
+-rw-r--r--   0 runner    (1001) docker     (127)      473 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/src/parkapi_sources/validators/time_validators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 06:35:38.151497 parkapi_sources-0.4.0/src/parkapi_sources.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    16681 2024-05-16 06:35:38.000000 parkapi_sources-0.4.0/src/parkapi_sources.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9252 2024-05-16 06:35:38.000000 parkapi_sources-0.4.0/src/parkapi_sources.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 06:35:38.000000 parkapi_sources-0.4.0/src/parkapi_sources.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-05-16 06:35:38.000000 parkapi_sources-0.4.0/src/parkapi_sources.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-16 06:35:38.000000 parkapi_sources-0.4.0/src/parkapi_sources.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 06:35:38.127496 parkapi_sources-0.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 06:35:38.131496 parkapi_sources-0.4.0/tests/converters/
+-rw-r--r--   0 runner    (1001) docker     (127)     1744 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/tests/converters/bahn_v2_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2053 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/tests/converters/bfrk_bw_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      823 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/tests/converters/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 06:35:38.143496 parkapi_sources-0.4.0/tests/converters/data/
+-rw-r--r--   0 runner    (1001) docker     (127)   947589 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/tests/converters/data/bahn_v2.json
+-rw-r--r--   0 runner    (1001) docker     (127)   552854 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/tests/converters/data/bfrk_bw_bike.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   617384 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/tests/converters/data/bfrk_bw_car.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    41226 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/tests/converters/data/ellwangen.xlsx
+-rw-r--r--   0 runner    (1001) docker     (127)    12651 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/tests/converters/data/freiburg.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3681 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/tests/converters/data/heidelberg.json
+-rw-r--r--   0 runner    (1001) docker     (127)    63706 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/tests/converters/data/karlsruhe.json
+-rw-r--r--   0 runner    (1001) docker     (127)   252177 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/tests/converters/data/karlsruhe_bike.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3477 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/tests/converters/data/kienzler.json
+-rw-r--r--   0 runner    (1001) docker     (127)    59377 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/tests/converters/data/konstanz_bike.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      666 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/tests/converters/data/mannheim.json
+-rw-r--r--   0 runner    (1001) docker     (127)    20667 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/tests/converters/data/neckarsulm.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    18115 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/tests/converters/data/neckarsulm_bike.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 06:35:38.147496 parkapi_sources-0.4.0/tests/converters/data/pbw/
+-rw-r--r--   0 runner    (1001) docker     (127)     1251 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/tests/converters/data/pbw/catalog-city.json
+-rw-r--r--   0 runner    (1001) docker     (127)   114816 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/tests/converters/data/pbw/object-by-city-10.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5061 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/tests/converters/data/pbw/object-by-city-11.json
+-rw-r--r--   0 runner    (1001) docker     (127)    36083 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/tests/converters/data/pbw/object-by-city-12.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1784 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/tests/converters/data/pbw/object-by-city-15.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6859 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/tests/converters/data/pbw/object-by-city-17.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7122 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/tests/converters/data/pbw/object-by-city-18.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5812 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/tests/converters/data/pbw/object-by-city-19.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5795 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/tests/converters/data/pbw/object-by-city-31.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/tests/converters/data/pbw/object-by-city-32.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6650 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/tests/converters/data/pbw/object-by-city-33.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/tests/converters/data/pbw/object-by-city-34.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3225 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/tests/converters/data/pbw/object-by-city-4.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3187 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/tests/converters/data/pbw/object-by-city-42.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3296 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/tests/converters/data/pbw/object-by-city-48.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1597 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/tests/converters/data/pbw/object-by-city-49.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3241 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/tests/converters/data/pbw/object-by-city-51.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/tests/converters/data/pbw/object-by-city-52.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/tests/converters/data/pbw/object-by-city-60.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1557 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/tests/converters/data/pbw/object-by-city-61.json
+-rw-r--r--   0 runner    (1001) docker     (127)    14227 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/tests/converters/data/pbw/object-by-city-7.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3149 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/tests/converters/data/pbw/object-by-city-71.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7071 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/tests/converters/data/pbw/object-by-city-9.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6685 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/tests/converters/data/pbw/object-dynamic-all.json
+-rw-r--r--   0 runner    (1001) docker     (127)    18956 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/tests/converters/data/pforzheim.json
+-rw-r--r--   0 runner    (1001) docker     (127)    30849 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/tests/converters/data/pum_bw.xlsx
+-rw-r--r--   0 runner    (1001) docker     (127)   526873 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/tests/converters/data/radvis_bw.json
+-rw-r--r--   0 runner    (1001) docker     (127)     9387 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/tests/converters/data/reutlingen.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    27295 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/tests/converters/data/reutlingen_bike.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    35423 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/tests/converters/data/stuttgart-realtime.xml
+-rw-r--r--   0 runner    (1001) docker     (127)   218959 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/tests/converters/data/stuttgart-static.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    62841 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/tests/converters/data/ulm.html
+-rw-r--r--   0 runner    (1001) docker     (127)   136171 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/tests/converters/data/vrs_p_r.xlsx
+-rw-r--r--   0 runner    (1001) docker     (127)     1149 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/tests/converters/ellwangen_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1859 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/tests/converters/freiburg_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2226 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/tests/converters/heidelberg_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2439 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/tests/converters/helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1979 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/tests/converters/karlsruhe_bike_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1926 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/tests/converters/karlsruhe_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/tests/converters/kienzler_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/tests/converters/konstanz_bike_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1546 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/tests/converters/mannheim_buchen_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/tests/converters/neckarsulm_bike_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/tests/converters/neckarsulm_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2880 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/tests/converters/pbw_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/tests/converters/pforzheim_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/tests/converters/pum_bw_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1705 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/tests/converters/radvis_bw_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1246 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/tests/converters/reutlingen_bike_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/tests/converters/reutlingen_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1949 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/tests/converters/stuttgart_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1777 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/tests/converters/ulm_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/tests/converters/vrs_p_r_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 06:35:38.147496 parkapi_sources-0.4.0/tests/models/
+-rw-r--r--   0 runner    (1001) docker     (127)     2183 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/tests/models/xlsx_inputs_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 06:35:38.147496 parkapi_sources-0.4.0/tests/util/
+-rw-r--r--   0 runner    (1001) docker     (127)     4105 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/tests/util/data_xml_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1706 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/tests/util/encoding_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4039 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/tests/util/xml_helper_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 06:35:38.151497 parkapi_sources-0.4.0/tests/validators/
+-rw-r--r--   0 runner    (1001) docker     (127)     1255 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/tests/validators/boolean_validators_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/tests/validators/date_validators_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2108 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/tests/validators/datetime_validators_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/tests/validators/integer_validators_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/tests/validators/noneable_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/tests/validators/string_validators_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      567 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/tests/validators/time_validators_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/tox.ini
```

### Comparing `parkapi_sources-0.3.1/.github/workflows/build-publish.yml` & `parkapi_sources-0.4.0/.github/workflows/build-publish.yml`

 * *Files 2% similar despite different names*

```diff
@@ -39,20 +39,20 @@
     needs: build
     runs-on: ubuntu-latest
 
     steps:
       - uses: actions/checkout@v4
 
       - name: Set timezone to Europe/Berlin
-        uses: szenius/set-timezone@v1.2
+        uses: szenius/set-timezone@v2.0
         with:
           timezoneLinux: "Europe/Berlin"
 
       - name: Setup Python 3.10
-        uses: actions/setup-python@v4
+        uses: actions/setup-python@v5
         with:
           python-version: '3.10'
 
       - name: Download build artifacts
         uses: actions/download-artifact@v4
         with:
           name: dist_packages
```

### Comparing `parkapi_sources-0.3.1/.github/workflows/lint-test.yml` & `parkapi_sources-0.4.0/.github/workflows/lint-test.yml`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.1/LICENCE.txt` & `parkapi_sources-0.4.0/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.1/PKG-INFO` & `parkapi_sources-0.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: parkapi_sources
-Version: 0.3.1
+Version: 0.4.0
 Summary: ParkAPI Sources is a collection of converters from several different data sources to normalized ParkAPI data.
 Author-email: "Ernesto Ruge, binary butterfly GmbH" <ernesto.ruge@binary-butterfly.de>
 Maintainer-email: "Ernesto Ruge, binary butterfly GmbH" <ernesto.ruge@binary-butterfly.de>
 Keywords: data,parking,converter,mobility,car,bike
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -15,24 +15,24 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Utilities
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENCE.txt
-Requires-Dist: validataclass~=0.9.0
+Requires-Dist: validataclass~=0.10.0
 Requires-Dist: pyproj~=3.6.1
 Requires-Dist: lxml~=5.2.1
 Requires-Dist: openpyxl~=3.1.2
 Requires-Dist: requests~=2.31.0
 Requires-Dist: beautifulsoup4~=4.12.3
 Provides-Extra: testing
-Requires-Dist: black~=24.3.0; extra == "testing"
-Requires-Dist: ruff~=0.3.5; extra == "testing"
-Requires-Dist: pytest~=8.1.1; extra == "testing"
+Requires-Dist: black~=24.4.2; extra == "testing"
+Requires-Dist: ruff~=0.4.1; extra == "testing"
+Requires-Dist: pytest~=8.2.0; extra == "testing"
 Requires-Dist: pytest-cov~=5.0.0; extra == "testing"
 Requires-Dist: requests-mock~=1.12.1; extra == "testing"
 
 # ParkAPI Sources
 
 ParkAPI Sources is a collection of converters from several different data sources to normalized ParkAPI data. ParkAPI does support parking
 for cars, for bikes and lockers. The data model is based on the original ParkAPI project and tries to stay compatible to DATEX II Parking
@@ -43,31 +43,34 @@
 | name                                                                              | purpose | type        | uid                  | realtime |
 |-----------------------------------------------------------------------------------|---------|-------------|----------------------|----------|
 | Deutsche Bahn                                                                     | car     | pull        | `bahn_v2`            | no       |
 | Barrierefreie Reisekette Baden-Württemberg: PKW-Parkplätze an Bahnhöfen           | car     | push (csv)  | `bfrk_bw_oepnv_car`  | no       |
 | Barrierefreie Reisekette Baden-Württemberg: PKW-Parkplätze an Bushaltestellen     | car     | push (csv)  | `bfrk_bw_spnv_car`   | no       |
 | Barrierefreie Reisekette Baden-Württemberg: Fahrrad-Parkplätze an Bahnhöfen       | bike    | push (csv)  | `bfrk_bw_oepnv_bike` | no       |
 | Barrierefreie Reisekette Baden-Württemberg: Fahrrad-Parkplätze an Bushaltestellen | bike    | push (csv)  | `bfrk_bw_spnv_bike`  | no       |
+| Stadt Ellwangen                                                                   | car     | push (xlsx) | `ellwangen`          | no       |
 | Stadt Buchen                                                                      | car     | push (json) | `buchen`             | yes      |
 | Stadt Freiburg                                                                    | car     | pull        | `freiburg`           | yes      |
 | Stadt Heidelberg                                                                  | car     | pull        | `heidelberg`         | yes      |
-| Stadt Karlsruhe                                                                   | car     | pull        | `karlsruhe`          | yes      |
+| Stadt Karlsruhe: PKW-Parkplätze                                                   | car     | pull        | `karlsruhe`          | yes      |
+| Stadt Karlsruhe: Fahhrrad-Abstellangen                                            | bike    | pull        | `karlsruhe_bike`     | no       |
 | Kienzler                                                                          | bike    | pull        | `kienzler`           | yes      |
+| Stadt Konstanz: Fahrrad-Abstellanlagen                                            | bike    | push        | `konstanz_bike`      | no       |
 | Stadt Mannheim                                                                    | car     | push (json) | `mannheim`           | yes      |
 | Stadt Neckarsulm: PKW-Parkplätze                                                  | car     | pull        | `neckarsulm`         | no       |
 | Stadt Neckarsulm: Fahrrad-Abstellanlagen                                          | bike    | pull        | `neckarsulm_bike`    | no       |
-| Stadt Karlsruhe                                                                   | car     | push (csv)  | `neckarsulm`         | no       |
 | Baden-Württemberg: Parken und Mitfahren                                           | car     | push (xlsx) | `pum_bw`             | no       |
+| RadVIS Baden-Württemberg (experimental)                                           | bike    | pull        | `radvis_bw`          | no       |
 | Parkraumgesellschaft Baden-Württemberg                                            | car     | pull        | `pbw`                | yes      |
 | Stadt Pforzheim                                                                   | car     | push (csv)  | `pforzheim`          | no       |
 | Stadt Reutlingen: PKW-Parkplätze                                                  | car     | push (csv)  | `reutlingen`         | no       |
 | Stadt Reutlingen: Fahrrad-Abstellanlagen                                          | bike    | push (csv)  | `reutlingen_bike`    | no       |
 | Stadt Stuttgart                                                                   | car     | push (json) | `stuttgart`          | yes      |
 | Stadt Ulm                                                                         | car     | pull        | `ulm`                | yes      |
-| Verband Region Stuttgart: Park and Ride                                           | car     | pull        | `vrs_p_r`            | yes      |
+| Verband Region Stuttgart: Park and Ride                                           | car     | push (xlsx) | `vrs_p_r`            | no       |
 
 New converters for new sources are always welcome, please have a look at "Contribute" below.
 
 
 ## Install
 
 ParkAPI Sources is a python module published at [PyPI](https://pypi.org/project/parkapi-sources/). Therefore, you can install it by
```

### Comparing `parkapi_sources-0.3.1/README.md` & `parkapi_sources-0.4.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -9,31 +9,34 @@
 | name                                                                              | purpose | type        | uid                  | realtime |
 |-----------------------------------------------------------------------------------|---------|-------------|----------------------|----------|
 | Deutsche Bahn                                                                     | car     | pull        | `bahn_v2`            | no       |
 | Barrierefreie Reisekette Baden-Württemberg: PKW-Parkplätze an Bahnhöfen           | car     | push (csv)  | `bfrk_bw_oepnv_car`  | no       |
 | Barrierefreie Reisekette Baden-Württemberg: PKW-Parkplätze an Bushaltestellen     | car     | push (csv)  | `bfrk_bw_spnv_car`   | no       |
 | Barrierefreie Reisekette Baden-Württemberg: Fahrrad-Parkplätze an Bahnhöfen       | bike    | push (csv)  | `bfrk_bw_oepnv_bike` | no       |
 | Barrierefreie Reisekette Baden-Württemberg: Fahrrad-Parkplätze an Bushaltestellen | bike    | push (csv)  | `bfrk_bw_spnv_bike`  | no       |
+| Stadt Ellwangen                                                                   | car     | push (xlsx) | `ellwangen`          | no       |
 | Stadt Buchen                                                                      | car     | push (json) | `buchen`             | yes      |
 | Stadt Freiburg                                                                    | car     | pull        | `freiburg`           | yes      |
 | Stadt Heidelberg                                                                  | car     | pull        | `heidelberg`         | yes      |
-| Stadt Karlsruhe                                                                   | car     | pull        | `karlsruhe`          | yes      |
+| Stadt Karlsruhe: PKW-Parkplätze                                                   | car     | pull        | `karlsruhe`          | yes      |
+| Stadt Karlsruhe: Fahhrrad-Abstellangen                                            | bike    | pull        | `karlsruhe_bike`     | no       |
 | Kienzler                                                                          | bike    | pull        | `kienzler`           | yes      |
+| Stadt Konstanz: Fahrrad-Abstellanlagen                                            | bike    | push        | `konstanz_bike`      | no       |
 | Stadt Mannheim                                                                    | car     | push (json) | `mannheim`           | yes      |
 | Stadt Neckarsulm: PKW-Parkplätze                                                  | car     | pull        | `neckarsulm`         | no       |
 | Stadt Neckarsulm: Fahrrad-Abstellanlagen                                          | bike    | pull        | `neckarsulm_bike`    | no       |
-| Stadt Karlsruhe                                                                   | car     | push (csv)  | `neckarsulm`         | no       |
 | Baden-Württemberg: Parken und Mitfahren                                           | car     | push (xlsx) | `pum_bw`             | no       |
+| RadVIS Baden-Württemberg (experimental)                                           | bike    | pull        | `radvis_bw`          | no       |
 | Parkraumgesellschaft Baden-Württemberg                                            | car     | pull        | `pbw`                | yes      |
 | Stadt Pforzheim                                                                   | car     | push (csv)  | `pforzheim`          | no       |
 | Stadt Reutlingen: PKW-Parkplätze                                                  | car     | push (csv)  | `reutlingen`         | no       |
 | Stadt Reutlingen: Fahrrad-Abstellanlagen                                          | bike    | push (csv)  | `reutlingen_bike`    | no       |
 | Stadt Stuttgart                                                                   | car     | push (json) | `stuttgart`          | yes      |
 | Stadt Ulm                                                                         | car     | pull        | `ulm`                | yes      |
-| Verband Region Stuttgart: Park and Ride                                           | car     | pull        | `vrs_p_r`            | yes      |
+| Verband Region Stuttgart: Park and Ride                                           | car     | push (xlsx) | `vrs_p_r`            | no       |
 
 New converters for new sources are always welcome, please have a look at "Contribute" below.
 
 
 ## Install
 
 ParkAPI Sources is a python module published at [PyPI](https://pypi.org/project/parkapi-sources/). Therefore, you can install it by
```

### Comparing `parkapi_sources-0.3.1/data/freiburg.geojson` & `parkapi_sources-0.4.0/data/freiburg.geojson`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.1/data/heidelberg.geojson` & `parkapi_sources-0.4.0/data/heidelberg.geojson`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.1/data/mannheim.geojson` & `parkapi_sources-0.4.0/data/mannheim.geojson`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.1/data/ulm.geojson` & `parkapi_sources-0.4.0/data/ulm.geojson`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.1/dev/test-pull-converter.py` & `parkapi_sources-0.4.0/dev/test-pull-converter.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.1/dev/test-push-converter.py` & `parkapi_sources-0.4.0/dev/test-push-converter.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.1/pyproject.toml` & `parkapi_sources-0.4.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -30,27 +30,27 @@
     "Programming Language :: Python :: 3.12",
     "Programming Language :: Python :: Implementation :: CPython",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Topic :: Utilities",
 ]
 
 dependencies = [
-    "validataclass~=0.9.0",
+    "validataclass~=0.10.0",
     "pyproj~=3.6.1",
     "lxml~=5.2.1",
     "openpyxl~=3.1.2",
     "requests~=2.31.0",
     "beautifulsoup4~=4.12.3",
 ]
 
 [project.optional-dependencies]
 testing = [
-    "black~=24.3.0",
-    "ruff~=0.3.5",
-    "pytest~=8.1.1",
+    "black~=24.4.2",
+    "ruff~=0.4.1",
+    "pytest~=8.2.0",
     "pytest-cov~=5.0.0",
     "requests-mock~=1.12.1",
 ]
 
 [build-system]
 requires = [
     "setuptools",
```

### Comparing `parkapi_sources-0.3.1/src/parkapi_sources/converters/__init__.py` & `parkapi_sources-0.4.0/src/parkapi_sources/converters/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,22 +2,25 @@
 Copyright 2024 binary butterfly GmbH
 Use of this source code is governed by an MIT-style license that can be found in the LICENSE.txt.
 """
 
 from .bahn_v2 import BahnV2PullConverter
 from .base_converter import BaseConverter
 from .bfrk_bw import BfrkBwOepnvBikePushConverter, BfrkBwOepnvCarPushConverter, BfrkBwSpnvBikePushConverter, BfrkBwSpnvCarPushConverter
+from .ellwangen import EllwangenPushConverter
 from .freiburg import FreiburgPullConverter
 from .heidelberg import HeidelbergPullConverter
-from .karlsruhe import KarlsruhePullConverter
+from .karlsruhe import KarlsruheBikePullConverter, KarlsruhePullConverter
 from .kienzler import KienzlerPullConverter
+from .konstanz_bike import KonstanzBikePushConverter
 from .mannheim_buchen import BuchenPushConverter, MannheimPushConverter
 from .neckarsulm import NeckarsulmPushConverter
 from .neckarsulm_bike import NeckarsulmBikePushConverter
 from .pbw import PbwPullConverter
 from .pforzheim import PforzheimPushConverter
 from .pum_bw import PumBwPushConverter
+from .radvis_bw import RadvisBwPullConverter
 from .reutlingen import ReutlingenPushConverter
 from .reutlingen_bike import ReutlingenBikePushConverter
 from .stuttgart import StuttgartPushConverter
 from .ulm import UlmPullConverter
 from .vrs_p_r import VrsParkAndRidePushConverter
```

### Comparing `parkapi_sources-0.3.1/src/parkapi_sources/converters/bahn_v2/converter.py` & `parkapi_sources-0.4.0/src/parkapi_sources/converters/bahn_v2/converter.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.1/src/parkapi_sources/converters/bahn_v2/mapper.py` & `parkapi_sources-0.4.0/src/parkapi_sources/converters/bahn_v2/mapper.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.1/src/parkapi_sources/converters/bahn_v2/validators.py` & `parkapi_sources-0.4.0/src/parkapi_sources/converters/bahn_v2/validators.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.1/src/parkapi_sources/converters/base_converter/base_converter.py` & `parkapi_sources-0.4.0/src/parkapi_sources/converters/base_converter/base_converter.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.1/src/parkapi_sources/converters/base_converter/pull/pull_converter.py` & `parkapi_sources-0.4.0/src/parkapi_sources/converters/base_converter/pull/pull_converter.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.1/src/parkapi_sources/converters/base_converter/pull/pull_scraper_mixin.py` & `parkapi_sources-0.4.0/src/parkapi_sources/converters/base_converter/pull/pull_scraper_mixin.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.1/src/parkapi_sources/converters/base_converter/pull/static_geojson_data_mixin/mixin.py` & `parkapi_sources-0.4.0/src/parkapi_sources/converters/base_converter/pull/static_geojson_data_mixin/mixin.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.1/src/parkapi_sources/converters/base_converter/pull/static_geojson_data_mixin/models.py` & `parkapi_sources-0.4.0/src/parkapi_sources/converters/base_converter/pull/static_geojson_data_mixin/models.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.1/src/parkapi_sources/converters/base_converter/push/csv_converter.py` & `parkapi_sources-0.4.0/src/parkapi_sources/converters/base_converter/push/csv_converter.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,19 +10,21 @@
 
 from parkapi_sources.converters.base_converter.push import PushConverter
 from parkapi_sources.exceptions import ImportParkingSiteException, ImportSourceException
 from parkapi_sources.models import RealtimeParkingSiteInput, StaticParkingSiteInput
 
 
 class CsvConverter(PushConverter, ABC):
+    csv_delimiter = ';'
+
     def handle_csv_string(
         self,
         data: StringIO,
     ) -> tuple[list[StaticParkingSiteInput | RealtimeParkingSiteInput], list[ImportParkingSiteException]]:
-        return self.handle_csv(list(csv.reader(data, delimiter=';')))
+        return self.handle_csv(list(csv.reader(data, delimiter=self.csv_delimiter)))
 
     def get_mapping_by_header(self, header_row: dict[str, str], row: list[Any]) -> dict[str, int]:
         mapping: dict[str, int] = {}
         for header_field, target_field in header_row.items():
             if header_field not in row:
                 raise ImportSourceException(
                     source_uid=self.source_info.uid,
```

### Comparing `parkapi_sources-0.3.1/src/parkapi_sources/converters/base_converter/push/json_converter.py` & `parkapi_sources-0.4.0/src/parkapi_sources/converters/base_converter/push/json_converter.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.1/src/parkapi_sources/converters/base_converter/push/normalized_xlsx_converter.py` & `parkapi_sources-0.4.0/src/parkapi_sources/converters/base_converter/push/normalized_xlsx_converter.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.1/src/parkapi_sources/converters/base_converter/push/parkapi_json_converter.py` & `parkapi_sources-0.4.0/src/parkapi_sources/converters/base_converter/push/parkapi_json_converter.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.1/src/parkapi_sources/converters/base_converter/push/xlsx_converter.py` & `parkapi_sources-0.4.0/src/parkapi_sources/converters/base_converter/push/xlsx_converter.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.1/src/parkapi_sources/converters/base_converter/push/xml_converter.py` & `parkapi_sources-0.4.0/src/parkapi_sources/converters/base_converter/push/xml_converter.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.1/src/parkapi_sources/converters/bfrk_bw/base_converter.py` & `parkapi_sources-0.4.0/src/parkapi_sources/converters/bfrk_bw/base_converter.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.1/src/parkapi_sources/converters/bfrk_bw/base_models.py` & `parkapi_sources-0.4.0/src/parkapi_sources/converters/bfrk_bw/base_models.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.1/src/parkapi_sources/converters/bfrk_bw/bike_converter.py` & `parkapi_sources-0.4.0/src/parkapi_sources/converters/bfrk_bw/bike_converter.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.1/src/parkapi_sources/converters/bfrk_bw/bike_models.py` & `parkapi_sources-0.4.0/src/parkapi_sources/converters/bfrk_bw/bike_models.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.1/src/parkapi_sources/converters/bfrk_bw/car_converter.py` & `parkapi_sources-0.4.0/src/parkapi_sources/converters/bfrk_bw/car_converter.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.1/src/parkapi_sources/converters/bfrk_bw/car_models.py` & `parkapi_sources-0.4.0/src/parkapi_sources/converters/bfrk_bw/car_models.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.1/src/parkapi_sources/converters/freiburg/converter.py` & `parkapi_sources-0.4.0/src/parkapi_sources/converters/freiburg/converter.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.1/src/parkapi_sources/converters/freiburg/models.py` & `parkapi_sources-0.4.0/src/parkapi_sources/converters/freiburg/models.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.1/src/parkapi_sources/converters/heidelberg/converter.py` & `parkapi_sources-0.4.0/src/parkapi_sources/converters/heidelberg/converter.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.1/src/parkapi_sources/converters/heidelberg/validators.py` & `parkapi_sources-0.4.0/src/parkapi_sources/converters/heidelberg/validators.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.1/src/parkapi_sources/converters/karlsruhe/converter.py` & `parkapi_sources-0.4.0/src/parkapi_sources/converters/karlsruhe/converter.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,42 +1,31 @@
 """
 Copyright 2024 binary butterfly GmbH
 Use of this source code is governed by an MIT-style license that can be found in the LICENSE.txt.
 """
 
+from abc import ABC
 from pathlib import Path
 
 import pyproj
 import requests
 from validataclass.exceptions import ValidationError
 from validataclass.validators import DataclassValidator
 
 from parkapi_sources.converters.base_converter.pull import GeojsonInput, PullConverter
 from parkapi_sources.exceptions import ImportParkingSiteException, ImportSourceException
 from parkapi_sources.models import RealtimeParkingSiteInput, SourceInfo, StaticParkingSiteInput
 
-from .models import KarlsruheFeatureInput
+from .models import KarlsruheBikeFeatureInput, KarlsruheFeatureInput
 
 
-class KarlsruhePullConverter(PullConverter):
+class KarlsruheBasePullConverter(PullConverter, ABC):
     proj: pyproj.Proj = pyproj.Proj(proj='utm', zone=32, ellps='WGS84', preserve_units=True)
     geojson_validator = DataclassValidator(GeojsonInput)
-    karlsruhe_feature_validator = DataclassValidator(KarlsruheFeatureInput)
-    source_info = SourceInfo(
-        uid='karlsruhe',
-        name='Stadt Karlsruhe',
-        public_url='https://web1.karlsruhe.de/service/Parken/',
-        source_url='https://mobil.trk.de:8443/geoserver/TBA/ows?service=WFS&version=1.0.0&request=GetFeature&typeName=TBA%3Aparkhaeuser'
-        '&outputFormat=application%2Fjson',
-        timezone='Europe/Berlin',
-        attribution_contributor='Stadt Karlsruhe',
-        attribution_license='Creative Commons Namensnennung - 4.0 International (CC-BY 4.0)',
-        attribution_url='http://creativecommons.org/licenses/by/4.0/',
-        has_realtime_data=True,
-    )
+    karlsruhe_feature_validator: DataclassValidator
 
     def _get_feature_inputs(self) -> tuple[list[KarlsruheFeatureInput], list[ImportParkingSiteException]]:
         feature_inputs: list[KarlsruheFeatureInput] = []
         import_parking_site_exceptions: list[ImportParkingSiteException] = []
 
         # Karlsruhes http-server config misses the intermediate cert GeoTrust TLS RSA CA G1, so we add it here manually.
         ca_path = Path(Path(__file__).parent, 'files', 'ca.crt.pem')
@@ -73,17 +62,54 @@
 
         static_parking_site_inputs: list[StaticParkingSiteInput] = []
         for feature_input in feature_inputs:
             static_parking_site_inputs.append(feature_input.to_static_parking_site_input(self.proj))
 
         return static_parking_site_inputs, import_parking_site_exceptions
 
+
+class KarlsruhePullConverter(KarlsruheBasePullConverter):
+    karlsruhe_feature_validator = DataclassValidator(KarlsruheFeatureInput)
+
+    source_info = SourceInfo(
+        uid='karlsruhe',
+        name='Stadt Karlsruhe: PKW-Parkplätze',
+        public_url='https://web1.karlsruhe.de/service/Parken/',
+        source_url='https://mobil.trk.de:8443/geoserver/TBA/ows?service=WFS&version=1.0.0&request=GetFeature&typeName=TBA%3Aparkhaeuser'
+        '&outputFormat=application%2Fjson',
+        timezone='Europe/Berlin',
+        attribution_contributor='Stadt Karlsruhe',
+        attribution_license='Creative Commons Namensnennung - 4.0 International (CC-BY 4.0)',
+        attribution_url='http://creativecommons.org/licenses/by/4.0/',
+        has_realtime_data=True,
+    )
+
     def get_realtime_parking_sites(self) -> tuple[list[RealtimeParkingSiteInput], list[ImportParkingSiteException]]:
         feature_inputs, import_parking_site_exceptions = self._get_feature_inputs()
 
         realtime_parking_site_inputs: list[RealtimeParkingSiteInput] = []
         for feature_input in feature_inputs:
             realtime_parking_site_input = feature_input.to_realtime_parking_site_input()
             if realtime_parking_site_input is not None:
                 realtime_parking_site_inputs.append(realtime_parking_site_input)
 
         return realtime_parking_site_inputs, import_parking_site_exceptions
+
+
+class KarlsruheBikePullConverter(KarlsruheBasePullConverter):
+    karlsruhe_feature_validator = DataclassValidator(KarlsruheBikeFeatureInput)
+
+    source_info = SourceInfo(
+        uid='karlsruhe',
+        name='Stadt Karlsruhe: Fahrrad-Abstellanlagen',
+        public_url='https://web1.karlsruhe.de/service/Parken/',
+        source_url='https://mobil.trk.de:8443/geoserver/TBA/ows?service=WFS&version=1.0.0&request=GetFeature'
+        '&typeName=TBA%3Aka_fahrradanlagen&outputFormat=application%2Fjson',
+        timezone='Europe/Berlin',
+        attribution_contributor='Stadt Karlsruhe',
+        attribution_license='Creative Commons Namensnennung - 4.0 International (CC-BY 4.0)',
+        attribution_url='http://creativecommons.org/licenses/by/4.0/',
+        has_realtime_data=False,
+    )
+
+    def get_realtime_parking_sites(self) -> tuple[list[RealtimeParkingSiteInput], list[ImportParkingSiteException]]:
+        return [], []
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `parkapi_sources-0.3.1/src/parkapi_sources/converters/karlsruhe/files/ca.crt.pem` & `parkapi_sources-0.4.0/src/parkapi_sources/converters/karlsruhe/files/ca.crt.pem`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.1/src/parkapi_sources/converters/kienzler/converter.py` & `parkapi_sources-0.4.0/src/parkapi_sources/converters/kienzler/converter.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.1/src/parkapi_sources/converters/kienzler/models.py` & `parkapi_sources-0.4.0/src/parkapi_sources/converters/kienzler/models.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.1/src/parkapi_sources/converters/mannheim_buchen/converter.py` & `parkapi_sources-0.4.0/src/parkapi_sources/converters/reutlingen_bike/converter.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,68 +1,69 @@
 """
 Copyright 2024 binary butterfly GmbH
 Use of this source code is governed by an MIT-style license that can be found in the LICENSE.txt.
 """
 
-from abc import ABC
+import csv
+from io import StringIO
 
+import pyproj
 from validataclass.exceptions import ValidationError
-from validataclass.validators import AnythingValidator, DataclassValidator, ListValidator
+from validataclass.validators import DataclassValidator
 
-from parkapi_sources.converters.base_converter.push import JsonConverter
-from parkapi_sources.converters.mannheim_buchen.models import MannheimBuchenInput
-from parkapi_sources.exceptions import ImportParkingSiteException, ImportSourceException
+from parkapi_sources.converters.base_converter.push import CsvConverter
+from parkapi_sources.converters.reutlingen_bike.validation import ReutlingenBikeRowInput
+from parkapi_sources.exceptions import ImportParkingSiteException
 from parkapi_sources.models import RealtimeParkingSiteInput, SourceInfo, StaticParkingSiteInput
 
 
-class MannheimBuchenBaseConverter(JsonConverter, ABC):
-    mannheim_buchen_list_validator = ListValidator(AnythingValidator(allowed_types=[dict]))
-    mannheim_buchen_validator = DataclassValidator(MannheimBuchenInput)
+class ReutlingenBikePushConverter(CsvConverter):
+    proj: pyproj.Proj = pyproj.Proj(proj='utm', zone=32, ellps='WGS84', preserve_units=True)
+    reutlingen_bike_row_validator = DataclassValidator(ReutlingenBikeRowInput)
 
-    def handle_json(
+    source_info = SourceInfo(
+        uid='reutlingen_bike',
+        name='Stadt Reutlingen: Fahrrad-Abstellanlagen',
+        public_url='https://www.reutlingen.de',
+        has_realtime_data=False,
+    )
+
+    header_mapping: dict[str, str] = {
+        '\ufeffSTANDORT': 'name',
+        'ANZAHL': 'capacity',
+        'ANLAGE': 'additional_name',
+        'GEOM': 'coordinates',
+    }
+
+    def handle_csv_string(
         self,
-        data: dict | list,
+        data: StringIO,
     ) -> tuple[list[StaticParkingSiteInput | RealtimeParkingSiteInput], list[ImportParkingSiteException]]:
-        parking_site_inputs: list[StaticParkingSiteInput | RealtimeParkingSiteInput] = []
-        parking_site_errors: list[ImportParkingSiteException] = []
+        return self.handle_csv(list(csv.reader(data, dialect='unix', delimiter=',')))
 
-        try:
-            parking_site_dicts = self.mannheim_buchen_list_validator.validate(data)
-        except ValidationError as e:
-            raise ImportSourceException(source_uid=self.source_info.uid, message=f'Invalid data {e.to_dict()}') from e
+    def handle_csv(self, data: list[list]) -> tuple[list[StaticParkingSiteInput], list[ImportParkingSiteException]]:
+        static_parking_site_inputs: list[StaticParkingSiteInput] = []
+        static_parking_site_errors: list[ImportParkingSiteException] = []
+
+        mapping: dict[str, int] = self.get_mapping_by_header(self.header_mapping, data[0])
+
+        # We start at row 2, as the first one is our header
+        for row in data[1:]:
+            input_dict: dict[str, str] = {}
+            for field in self.header_mapping.values():
+                input_dict[field] = row[mapping[field]]
 
-        for parking_site_dict in parking_site_dicts:
             try:
-                parking_site_input: MannheimBuchenInput = self.mannheim_buchen_validator.validate(parking_site_dict)
-
-                parking_site_inputs.append(parking_site_input.to_static_parking_site(city=self.source_info.name))
-                parking_site_inputs.append(parking_site_input.to_realtime_parking_site())
-
+                reutlingen_bike_row_input: ReutlingenBikeRowInput = self.reutlingen_bike_row_validator.validate(input_dict)
             except ValidationError as e:
-                parking_site_errors.append(
+                static_parking_site_errors.append(
                     ImportParkingSiteException(
                         source_uid=self.source_info.uid,
-                        parking_site_uid=parking_site_dict.get('uid'),
-                        message=f'validation error for {parking_site_dict}: {e.to_dict()}',
+                        parking_site_uid=input_dict.get('name'),
+                        message=f'validation error for {input_dict}: {e.to_dict()}',
                     ),
                 )
-        return parking_site_inputs, parking_site_errors
+                continue
 
+            static_parking_site_inputs.append(reutlingen_bike_row_input.to_parking_site_input(self.proj))
 
-class MannheimPushConverter(MannheimBuchenBaseConverter):
-    source_info = SourceInfo(
-        uid='mannheim',
-        name='Stadt Mannheim',
-        public_url='https://www.parken-mannheim.de',
-        timezone='Europe/Berlin',
-        has_realtime_data=True,
-    )
-
-
-class BuchenPushConverter(MannheimBuchenBaseConverter):
-    source_info = SourceInfo(
-        uid='buchen',
-        name='Stadt Buchen',
-        public_url='https://www.buchen.de/ueber-buchen/kostenlos-parken.html',
-        timezone='Europe/Berlin',
-        has_realtime_data=True,
-    )
+        return static_parking_site_inputs, static_parking_site_errors
```

### Comparing `parkapi_sources-0.3.1/src/parkapi_sources/converters/neckarsulm/converter.py` & `parkapi_sources-0.4.0/src/parkapi_sources/converters/neckarsulm/converter.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.1/src/parkapi_sources/converters/neckarsulm/models.py` & `parkapi_sources-0.4.0/src/parkapi_sources/converters/neckarsulm/models.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.1/src/parkapi_sources/converters/neckarsulm_bike/converter.py` & `parkapi_sources-0.4.0/src/parkapi_sources/converters/neckarsulm_bike/converter.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.1/src/parkapi_sources/converters/pbw/converter.py` & `parkapi_sources-0.4.0/src/parkapi_sources/converters/pbw/converter.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.1/src/parkapi_sources/converters/pbw/mapper.py` & `parkapi_sources-0.4.0/src/parkapi_sources/converters/pbw/mapper.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.1/src/parkapi_sources/converters/pbw/validation.py` & `parkapi_sources-0.4.0/src/parkapi_sources/converters/pbw/validation.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.1/src/parkapi_sources/converters/pforzheim/converter.py` & `parkapi_sources-0.4.0/src/parkapi_sources/converters/pforzheim/converter.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 
 from validataclass.exceptions import ValidationError
 from validataclass.validators import DataclassValidator
 
 from parkapi_sources.converters.base_converter.push import JsonConverter
 from parkapi_sources.exceptions import ImportParkingSiteException
 from parkapi_sources.models import SourceInfo, StaticParkingSiteInput
+from parkapi_sources.models.enums import SupervisionType
 
 from .validation import PforzheimInput
 
 
 class PforzheimPushConverter(JsonConverter):
     pforzheim_validator = DataclassValidator(PforzheimInput)
 
@@ -49,14 +50,14 @@
                 lon=input_data.lon,
                 address=input_data.address.replace('\n', ', '),
                 description=input_data.description.replace('\n', ', '),
                 capacity=input_data.capacity,
                 capacity_woman=input_data.quantitySpacesReservedForWomen,
                 capacity_disabled=input_data.quantitySpacesReservedForMobilityImpededPerson,
                 fee_description=input_data.feeInformation.replace('\n', ', '),
-                is_supervised=True if 'ja' in input_data.securityInformation.lower() else False,
+                supervision_type=SupervisionType.YES if 'ja' in input_data.securityInformation.lower() else False,
                 opening_hours='24/7' if input_data.hasOpeningHours24h else None,
                 static_data_updated_at=datetime.now(tz=timezone.utc),
             )
             static_parking_site_inputs.append(parking_site_input)
 
         return static_parking_site_inputs, static_parking_site_errors
```

### Comparing `parkapi_sources-0.3.1/src/parkapi_sources/converters/pforzheim/validation.py` & `parkapi_sources-0.4.0/src/parkapi_sources/converters/pforzheim/validation.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.1/src/parkapi_sources/converters/pum_bw/converter.py` & `parkapi_sources-0.4.0/src/parkapi_sources/converters/pum_bw/converter.py`

 * *Files 4% similar despite different names*

```diff
@@ -58,16 +58,18 @@
                 )
                 continue
 
         return static_parking_site_inputs, static_parking_site_errors
 
     @staticmethod
     def map_row_to_parking_site_dict(mapping: dict[str, int], row: list[Cell]) -> dict[str, Any]:
-        parking_site_dict: dict[str, str] = {}
+        parking_site_dict: dict[str, Any] = {}
         for field in mapping.keys():
             parking_site_dict[field] = row[mapping[field]].value
 
         parking_site_dict['uid'] = f"{parking_site_dict['uid']}-{parking_site_dict['name']}"
         parking_site_dict['name'] = f"{parking_site_dict['street']} {parking_site_dict['name']}"
+        parking_site_dict['type'] = 'OFF_STREET_PARKING_GROUND'
+        parking_site_dict['park_and_ride_type'] = ['CARPOOL']
         parking_site_dict['static_data_updated_at'] = datetime.now(tz=timezone.utc).isoformat()
 
         return parking_site_dict
```

### Comparing `parkapi_sources-0.3.1/src/parkapi_sources/converters/reutlingen/converter.py` & `parkapi_sources-0.4.0/src/parkapi_sources/converters/reutlingen/converter.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.1/src/parkapi_sources/converters/reutlingen/validation.py` & `parkapi_sources-0.4.0/src/parkapi_sources/converters/reutlingen/validation.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.1/src/parkapi_sources/converters/reutlingen_bike/converter.py` & `parkapi_sources-0.4.0/src/parkapi_sources/converters/konstanz_bike/converter.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,69 +1,66 @@
 """
 Copyright 2024 binary butterfly GmbH
 Use of this source code is governed by an MIT-style license that can be found in the LICENSE.txt.
 """
 
-import csv
-from io import StringIO
-
-import pyproj
 from validataclass.exceptions import ValidationError
 from validataclass.validators import DataclassValidator
 
 from parkapi_sources.converters.base_converter.push import CsvConverter
-from parkapi_sources.converters.reutlingen_bike.validation import ReutlingenBikeRowInput
 from parkapi_sources.exceptions import ImportParkingSiteException
-from parkapi_sources.models import RealtimeParkingSiteInput, SourceInfo, StaticParkingSiteInput
+from parkapi_sources.models import SourceInfo, StaticParkingSiteInput
+
+from .models import KonstanzRowInput
 
 
-class ReutlingenBikePushConverter(CsvConverter):
-    proj: pyproj.Proj = pyproj.Proj(proj='utm', zone=32, ellps='WGS84', preserve_units=True)
-    reutlingen_bike_row_validator = DataclassValidator(ReutlingenBikeRowInput)
+class KonstanzBikePushConverter(CsvConverter):
+    konstanz_bike_row_validator = DataclassValidator(KonstanzRowInput)
+    csv_delimiter = ','
 
     source_info = SourceInfo(
-        uid='reutlingen_bike',
-        name='Stadt Reutlingen: Fahrrad-Abstellanlagen',
-        public_url='https://www.reutlingen.de',
+        uid='konstanz_bike',
+        name='Stadt Konstanz: Fahrrad-Abstellanlagen',
+        public_url='https://www.konstanz.de/',
         has_realtime_data=False,
     )
 
     header_mapping: dict[str, str] = {
-        '\ufeffSTANDORT': 'name',
-        'ANZAHL': 'capacity',
-        'ANLAGE': 'additional_name',
-        'GEOM': 'coordinates',
+        'ABSTELL_NR': 'uid',
+        'Lagebezeichnung': 'address',
+        'Art': 'type',
+        'Ueberdachung': 'is_covered',
+        'Beleuchtung': 'has_lighting',
+        'Eigentuemer_Baulasttraeger': 'operator_name',
+        'Stadtteil': 'district',
+        'Kapazitaet': 'capacity',
+        'coordinates': 'coordinates',
+        'geometry': 'geometry',
     }
 
-    def handle_csv_string(
-        self,
-        data: StringIO,
-    ) -> tuple[list[StaticParkingSiteInput | RealtimeParkingSiteInput], list[ImportParkingSiteException]]:
-        return self.handle_csv(list(csv.reader(data, dialect='unix', delimiter=',')))
-
     def handle_csv(self, data: list[list]) -> tuple[list[StaticParkingSiteInput], list[ImportParkingSiteException]]:
         static_parking_site_inputs: list[StaticParkingSiteInput] = []
         static_parking_site_errors: list[ImportParkingSiteException] = []
 
         mapping: dict[str, int] = self.get_mapping_by_header(self.header_mapping, data[0])
 
         # We start at row 2, as the first one is our header
         for row in data[1:]:
             input_dict: dict[str, str] = {}
             for field in self.header_mapping.values():
                 input_dict[field] = row[mapping[field]]
 
             try:
-                reutlingen_bike_row_input: ReutlingenBikeRowInput = self.reutlingen_bike_row_validator.validate(input_dict)
+                input_data: KonstanzRowInput = self.konstanz_bike_row_validator.validate(input_dict)
             except ValidationError as e:
                 static_parking_site_errors.append(
                     ImportParkingSiteException(
                         source_uid=self.source_info.uid,
-                        parking_site_uid=input_dict.get('name'),
+                        parking_site_uid=input_dict.get('id'),
                         message=f'validation error for {input_dict}: {e.to_dict()}',
                     ),
                 )
                 continue
 
-            static_parking_site_inputs.append(reutlingen_bike_row_input.to_parking_site_input(self.proj))
+            static_parking_site_inputs.append(input_data.to_static_parking_site_input())
 
         return static_parking_site_inputs, static_parking_site_errors
```

### Comparing `parkapi_sources-0.3.1/src/parkapi_sources/converters/reutlingen_bike/validation.py` & `parkapi_sources-0.4.0/src/parkapi_sources/converters/reutlingen_bike/validation.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.1/src/parkapi_sources/converters/stuttgart/converter.py` & `parkapi_sources-0.4.0/src/parkapi_sources/converters/stuttgart/converter.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.1/src/parkapi_sources/converters/ulm/converter.py` & `parkapi_sources-0.4.0/src/parkapi_sources/converters/ulm/converter.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.1/src/parkapi_sources/converters/vrs_p_r/vrs_p_r.py` & `parkapi_sources-0.4.0/src/parkapi_sources/converters/vrs_p_r/vrs_p_r.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.1/src/parkapi_sources/exceptions.py` & `parkapi_sources-0.4.0/src/parkapi_sources/exceptions.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.1/src/parkapi_sources/models/parking_site_inputs.py` & `parkapi_sources-0.4.0/src/parkapi_sources/models/parking_site_inputs.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """
 Copyright 2023 binary butterfly GmbH
 Use of this source code is governed by an MIT-style license that can be found in the LICENSE.txt.
 """
 
 from datetime import datetime, timezone
 from decimal import Decimal
+from typing import Optional
 
 from validataclass.dataclasses import Default, DefaultUnset, ValidataclassMixin, validataclass
 from validataclass.exceptions import DataclassPostValidationError, ValidationError
 from validataclass.helpers import OptionalUnsetNone
 from validataclass.validators import (
     BooleanValidator,
     DataclassValidator,
@@ -18,15 +19,15 @@
     ListValidator,
     Noneable,
     NumericValidator,
     StringValidator,
     UrlValidator,
 )
 
-from .enums import ExternalIdentifierType, OpeningStatus, ParkAndRideType, ParkingSiteType, PurposeType
+from .enums import ExternalIdentifierType, OpeningStatus, ParkAndRideType, ParkingSiteType, PurposeType, SupervisionType
 
 
 @validataclass
 class BaseParkingSiteInput(ValidataclassMixin):
     uid: str = StringValidator(min_length=1, max_length=256)
 
 
@@ -45,24 +46,27 @@
     address: OptionalUnsetNone[str] = Noneable(StringValidator(max_length=512)), DefaultUnset
     description: OptionalUnsetNone[str] = Noneable(StringValidator(max_length=4096)), DefaultUnset
     type: OptionalUnsetNone[ParkingSiteType] = Noneable(EnumValidator(ParkingSiteType)), DefaultUnset
 
     max_stay: OptionalUnsetNone[int] = Noneable(IntegerValidator(min_value=0, allow_strings=True)), DefaultUnset
     max_height: OptionalUnsetNone[int] = Noneable(IntegerValidator(min_value=0, allow_strings=True)), DefaultUnset
     has_lighting: OptionalUnsetNone[bool] = Noneable(BooleanValidator()), DefaultUnset
+    is_covered: OptionalUnsetNone[bool] = Noneable(BooleanValidator()), DefaultUnset
     fee_description: OptionalUnsetNone[str] = Noneable(StringValidator(max_length=4096)), DefaultUnset
     has_fee: OptionalUnsetNone[bool] = Noneable(BooleanValidator()), DefaultUnset
     park_and_ride_type: OptionalUnsetNone[list[ParkAndRideType]] = (
         Noneable(
             ListValidator(EnumValidator(ParkAndRideType)),
         ),
         DefaultUnset,
     )
-    is_supervised: OptionalUnsetNone[bool] = Noneable(BooleanValidator()), DefaultUnset
+    supervision_type: OptionalUnsetNone[SupervisionType] = Noneable(EnumValidator(SupervisionType)), DefaultUnset
+    is_covered: OptionalUnsetNone[bool] = Noneable(BooleanValidator()), DefaultUnset
     photo_url: OptionalUnsetNone[str] = Noneable(UrlValidator(max_length=4096)), DefaultUnset
+    related_location: OptionalUnsetNone[str] = Noneable(StringValidator(max_length=256)), DefaultUnset
 
     has_realtime_data: OptionalUnsetNone[bool] = Noneable(BooleanValidator(), default=False), DefaultUnset
     static_data_updated_at: OptionalUnsetNone[datetime] = (
         DateTimeValidator(
             local_timezone=timezone.utc,
             target_timezone=timezone.utc,
             discard_milliseconds=True,
@@ -84,14 +88,21 @@
 
     opening_hours: OptionalUnsetNone[str] = Noneable(StringValidator(max_length=512)), DefaultUnset
 
     external_identifiers: OptionalUnsetNone[list[ExternalIdentifierInput]] = (
         Noneable(ListValidator(DataclassValidator(ExternalIdentifierInput))),
         DefaultUnset,
     )
+    tags: list[str] = ListValidator(StringValidator(min_length=1)), Default([])
+
+    @property
+    def is_supervised(self) -> Optional[bool]:
+        if self.supervision_type is None:
+            return None
+        return self.supervision_type in [SupervisionType.YES, SupervisionType.VIDEO, SupervisionType.ATTENDED]
 
     def __post_init__(self):
         if self.lat == 0 and self.lon == 0:
             raise DataclassPostValidationError(error=ValidationError(code='lat_lon_zero', reason='Latitude and longitude are both zero.'))
 
         if self.park_and_ride_type:
             if (ParkAndRideType.NO in self.park_and_ride_type or ParkAndRideType.YES in self.park_and_ride_type) and len(
```

### Comparing `parkapi_sources-0.3.1/src/parkapi_sources/models/source_info.py` & `parkapi_sources-0.4.0/src/parkapi_sources/models/source_info.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.1/src/parkapi_sources/models/xlsx_inputs.py` & `parkapi_sources-0.4.0/src/parkapi_sources/models/xlsx_inputs.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,14 @@
 
 @validataclass
 class ExcelStaticParkingSiteInput(StaticParkingSiteInput):
     operator_name: Optional[str] = ExcelNoneable(StringValidator(max_length=256))
     uid: str = NumberCastingStringValidator(min_length=1, max_length=256)
     has_lighting: Optional[bool] = ExcelNoneable(ExcelMappedBooleanValidator())
     has_fee: Optional[bool] = ExcelNoneable(ExcelMappedBooleanValidator())
-    is_supervised: Optional[bool] = ExcelNoneable(ExcelMappedBooleanValidator())
     has_realtime_data: Optional[bool] = ExcelNoneable(ExcelMappedBooleanValidator(), default=False)
     max_stay: Optional[int] = ExcelNoneable(GermanDurationIntegerValidator()), Default(None)
 
     capacity: Optional[int] = ExcelNoneable(IntegerValidator(min_value=0))
     capacity_disabled: Optional[int] = ExcelNoneable(IntegerValidator(min_value=0))
     capacity_woman: Optional[int] = ExcelNoneable(IntegerValidator(min_value=0))
     capacity_family: Optional[int] = ExcelNoneable(IntegerValidator(min_value=0))
```

### Comparing `parkapi_sources-0.3.1/src/parkapi_sources/parkapi_sources.py` & `parkapi_sources-0.4.0/src/parkapi_sources/parkapi_sources.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,24 +9,28 @@
     BahnV2PullConverter,
     BaseConverter,
     BfrkBwOepnvBikePushConverter,
     BfrkBwOepnvCarPushConverter,
     BfrkBwSpnvBikePushConverter,
     BfrkBwSpnvCarPushConverter,
     BuchenPushConverter,
+    EllwangenPushConverter,
     FreiburgPullConverter,
     HeidelbergPullConverter,
+    KarlsruheBikePullConverter,
     KarlsruhePullConverter,
     KienzlerPullConverter,
+    KonstanzBikePushConverter,
     MannheimPushConverter,
     NeckarsulmBikePushConverter,
     NeckarsulmPushConverter,
     PbwPullConverter,
     PforzheimPushConverter,
     PumBwPushConverter,
+    RadvisBwPullConverter,
     ReutlingenBikePushConverter,
     ReutlingenPushConverter,
     StuttgartPushConverter,
     UlmPullConverter,
     VrsParkAndRidePushConverter,
 )
 from .converters.base_converter.pull import PullConverter
@@ -38,25 +42,29 @@
 class ParkAPISources:
     converter_classes: list[Type[BaseConverter]] = [
         BahnV2PullConverter,
         BfrkBwOepnvBikePushConverter,
         BfrkBwOepnvCarPushConverter,
         BfrkBwSpnvBikePushConverter,
         BfrkBwSpnvCarPushConverter,
+        EllwangenPushConverter,
         BuchenPushConverter,
         FreiburgPullConverter,
         HeidelbergPullConverter,
+        KarlsruheBikePullConverter,
         KarlsruhePullConverter,
         KienzlerPullConverter,
+        KonstanzBikePushConverter,
         MannheimPushConverter,
         NeckarsulmBikePushConverter,
         NeckarsulmPushConverter,
         PbwPullConverter,
         PforzheimPushConverter,
         PumBwPushConverter,
+        RadvisBwPullConverter,
         ReutlingenPushConverter,
         ReutlingenBikePushConverter,
         StuttgartPushConverter,
         UlmPullConverter,
         VrsParkAndRidePushConverter,
     ]
     config_helper: ConfigHelper
```

### Comparing `parkapi_sources-0.3.1/src/parkapi_sources/scripts/parkapi.py` & `parkapi_sources-0.4.0/src/parkapi_sources/scripts/parkapi.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.1/src/parkapi_sources/util/encoding.py` & `parkapi_sources-0.4.0/src/parkapi_sources/util/encoding.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.1/src/parkapi_sources/util/xml_helper.py` & `parkapi_sources-0.4.0/src/parkapi_sources/util/xml_helper.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.1/src/parkapi_sources/validators/__init__.py` & `parkapi_sources-0.4.0/src/parkapi_sources/validators/__init__.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.1/src/parkapi_sources/validators/boolean_validators.py` & `parkapi_sources-0.4.0/src/parkapi_sources/validators/boolean_validators.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.1/src/parkapi_sources/validators/date_validator.py` & `parkapi_sources-0.4.0/src/parkapi_sources/validators/date_validator.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.1/src/parkapi_sources/validators/datetime_validator.py` & `parkapi_sources-0.4.0/src/parkapi_sources/validators/datetime_validator.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.1/src/parkapi_sources/validators/integer_validators.py` & `parkapi_sources-0.4.0/src/parkapi_sources/validators/integer_validators.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.1/src/parkapi_sources/validators/list_validator.py` & `parkapi_sources-0.4.0/src/parkapi_sources/validators/list_validator.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.1/src/parkapi_sources/validators/noneable.py` & `parkapi_sources-0.4.0/src/parkapi_sources/validators/noneable.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.1/src/parkapi_sources/validators/string_validators.py` & `parkapi_sources-0.4.0/src/parkapi_sources/validators/string_validators.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.1/src/parkapi_sources.egg-info/PKG-INFO` & `parkapi_sources-0.4.0/src/parkapi_sources.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: parkapi_sources
-Version: 0.3.1
+Version: 0.4.0
 Summary: ParkAPI Sources is a collection of converters from several different data sources to normalized ParkAPI data.
 Author-email: "Ernesto Ruge, binary butterfly GmbH" <ernesto.ruge@binary-butterfly.de>
 Maintainer-email: "Ernesto Ruge, binary butterfly GmbH" <ernesto.ruge@binary-butterfly.de>
 Keywords: data,parking,converter,mobility,car,bike
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -15,24 +15,24 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Utilities
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENCE.txt
-Requires-Dist: validataclass~=0.9.0
+Requires-Dist: validataclass~=0.10.0
 Requires-Dist: pyproj~=3.6.1
 Requires-Dist: lxml~=5.2.1
 Requires-Dist: openpyxl~=3.1.2
 Requires-Dist: requests~=2.31.0
 Requires-Dist: beautifulsoup4~=4.12.3
 Provides-Extra: testing
-Requires-Dist: black~=24.3.0; extra == "testing"
-Requires-Dist: ruff~=0.3.5; extra == "testing"
-Requires-Dist: pytest~=8.1.1; extra == "testing"
+Requires-Dist: black~=24.4.2; extra == "testing"
+Requires-Dist: ruff~=0.4.1; extra == "testing"
+Requires-Dist: pytest~=8.2.0; extra == "testing"
 Requires-Dist: pytest-cov~=5.0.0; extra == "testing"
 Requires-Dist: requests-mock~=1.12.1; extra == "testing"
 
 # ParkAPI Sources
 
 ParkAPI Sources is a collection of converters from several different data sources to normalized ParkAPI data. ParkAPI does support parking
 for cars, for bikes and lockers. The data model is based on the original ParkAPI project and tries to stay compatible to DATEX II Parking
@@ -43,31 +43,34 @@
 | name                                                                              | purpose | type        | uid                  | realtime |
 |-----------------------------------------------------------------------------------|---------|-------------|----------------------|----------|
 | Deutsche Bahn                                                                     | car     | pull        | `bahn_v2`            | no       |
 | Barrierefreie Reisekette Baden-Württemberg: PKW-Parkplätze an Bahnhöfen           | car     | push (csv)  | `bfrk_bw_oepnv_car`  | no       |
 | Barrierefreie Reisekette Baden-Württemberg: PKW-Parkplätze an Bushaltestellen     | car     | push (csv)  | `bfrk_bw_spnv_car`   | no       |
 | Barrierefreie Reisekette Baden-Württemberg: Fahrrad-Parkplätze an Bahnhöfen       | bike    | push (csv)  | `bfrk_bw_oepnv_bike` | no       |
 | Barrierefreie Reisekette Baden-Württemberg: Fahrrad-Parkplätze an Bushaltestellen | bike    | push (csv)  | `bfrk_bw_spnv_bike`  | no       |
+| Stadt Ellwangen                                                                   | car     | push (xlsx) | `ellwangen`          | no       |
 | Stadt Buchen                                                                      | car     | push (json) | `buchen`             | yes      |
 | Stadt Freiburg                                                                    | car     | pull        | `freiburg`           | yes      |
 | Stadt Heidelberg                                                                  | car     | pull        | `heidelberg`         | yes      |
-| Stadt Karlsruhe                                                                   | car     | pull        | `karlsruhe`          | yes      |
+| Stadt Karlsruhe: PKW-Parkplätze                                                   | car     | pull        | `karlsruhe`          | yes      |
+| Stadt Karlsruhe: Fahhrrad-Abstellangen                                            | bike    | pull        | `karlsruhe_bike`     | no       |
 | Kienzler                                                                          | bike    | pull        | `kienzler`           | yes      |
+| Stadt Konstanz: Fahrrad-Abstellanlagen                                            | bike    | push        | `konstanz_bike`      | no       |
 | Stadt Mannheim                                                                    | car     | push (json) | `mannheim`           | yes      |
 | Stadt Neckarsulm: PKW-Parkplätze                                                  | car     | pull        | `neckarsulm`         | no       |
 | Stadt Neckarsulm: Fahrrad-Abstellanlagen                                          | bike    | pull        | `neckarsulm_bike`    | no       |
-| Stadt Karlsruhe                                                                   | car     | push (csv)  | `neckarsulm`         | no       |
 | Baden-Württemberg: Parken und Mitfahren                                           | car     | push (xlsx) | `pum_bw`             | no       |
+| RadVIS Baden-Württemberg (experimental)                                           | bike    | pull        | `radvis_bw`          | no       |
 | Parkraumgesellschaft Baden-Württemberg                                            | car     | pull        | `pbw`                | yes      |
 | Stadt Pforzheim                                                                   | car     | push (csv)  | `pforzheim`          | no       |
 | Stadt Reutlingen: PKW-Parkplätze                                                  | car     | push (csv)  | `reutlingen`         | no       |
 | Stadt Reutlingen: Fahrrad-Abstellanlagen                                          | bike    | push (csv)  | `reutlingen_bike`    | no       |
 | Stadt Stuttgart                                                                   | car     | push (json) | `stuttgart`          | yes      |
 | Stadt Ulm                                                                         | car     | pull        | `ulm`                | yes      |
-| Verband Region Stuttgart: Park and Ride                                           | car     | pull        | `vrs_p_r`            | yes      |
+| Verband Region Stuttgart: Park and Ride                                           | car     | push (xlsx) | `vrs_p_r`            | no       |
 
 New converters for new sources are always welcome, please have a look at "Contribute" below.
 
 
 ## Install
 
 ParkAPI Sources is a python module published at [PyPI](https://pypi.org/project/parkapi-sources/). Therefore, you can install it by
```

### Comparing `parkapi_sources-0.3.1/src/parkapi_sources.egg-info/SOURCES.txt` & `parkapi_sources-0.4.0/src/parkapi_sources.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -50,44 +50,51 @@
 src/parkapi_sources/converters/bfrk_bw/__init__.py
 src/parkapi_sources/converters/bfrk_bw/base_converter.py
 src/parkapi_sources/converters/bfrk_bw/base_models.py
 src/parkapi_sources/converters/bfrk_bw/bike_converter.py
 src/parkapi_sources/converters/bfrk_bw/bike_models.py
 src/parkapi_sources/converters/bfrk_bw/car_converter.py
 src/parkapi_sources/converters/bfrk_bw/car_models.py
+src/parkapi_sources/converters/ellwangen/__init__.py
+src/parkapi_sources/converters/ellwangen/converter.py
 src/parkapi_sources/converters/freiburg/__init__.py
 src/parkapi_sources/converters/freiburg/converter.py
 src/parkapi_sources/converters/freiburg/models.py
 src/parkapi_sources/converters/heidelberg/__init__.py
 src/parkapi_sources/converters/heidelberg/converter.py
 src/parkapi_sources/converters/heidelberg/validators.py
 src/parkapi_sources/converters/karlsruhe/__init__.py
 src/parkapi_sources/converters/karlsruhe/converter.py
 src/parkapi_sources/converters/karlsruhe/models.py
 src/parkapi_sources/converters/karlsruhe/files/ca.crt.pem
 src/parkapi_sources/converters/kienzler/__init__.py
 src/parkapi_sources/converters/kienzler/converter.py
 src/parkapi_sources/converters/kienzler/models.py
+src/parkapi_sources/converters/konstanz_bike/__init__.py
+src/parkapi_sources/converters/konstanz_bike/converter.py
+src/parkapi_sources/converters/konstanz_bike/models.py
 src/parkapi_sources/converters/mannheim_buchen/__init__.py
 src/parkapi_sources/converters/mannheim_buchen/converter.py
-src/parkapi_sources/converters/mannheim_buchen/models.py
 src/parkapi_sources/converters/neckarsulm/__init__.py
 src/parkapi_sources/converters/neckarsulm/converter.py
 src/parkapi_sources/converters/neckarsulm/models.py
 src/parkapi_sources/converters/neckarsulm_bike/__init__.py
 src/parkapi_sources/converters/neckarsulm_bike/converter.py
 src/parkapi_sources/converters/pbw/__init__.py
 src/parkapi_sources/converters/pbw/converter.py
 src/parkapi_sources/converters/pbw/mapper.py
 src/parkapi_sources/converters/pbw/validation.py
 src/parkapi_sources/converters/pforzheim/__init__.py
 src/parkapi_sources/converters/pforzheim/converter.py
 src/parkapi_sources/converters/pforzheim/validation.py
 src/parkapi_sources/converters/pum_bw/__init__.py
 src/parkapi_sources/converters/pum_bw/converter.py
+src/parkapi_sources/converters/radvis_bw/__init__.py
+src/parkapi_sources/converters/radvis_bw/converter.py
+src/parkapi_sources/converters/radvis_bw/models.py
 src/parkapi_sources/converters/reutlingen/__init__.py
 src/parkapi_sources/converters/reutlingen/converter.py
 src/parkapi_sources/converters/reutlingen/validation.py
 src/parkapi_sources/converters/reutlingen_bike/__init__.py
 src/parkapi_sources/converters/reutlingen_bike/converter.py
 src/parkapi_sources/converters/reutlingen_bike/validation.py
 src/parkapi_sources/converters/stuttgart/__init__.py
@@ -116,43 +123,50 @@
 src/parkapi_sources/validators/noneable.py
 src/parkapi_sources/validators/string_validators.py
 src/parkapi_sources/validators/time_validators.py
 tests/conftest.py
 tests/converters/bahn_v2_test.py
 tests/converters/bfrk_bw_test.py
 tests/converters/conftest.py
+tests/converters/ellwangen_test.py
 tests/converters/freiburg_test.py
 tests/converters/heidelberg_test.py
 tests/converters/helper.py
+tests/converters/karlsruhe_bike_test.py
 tests/converters/karlsruhe_test.py
 tests/converters/kienzler_test.py
+tests/converters/konstanz_bike_test.py
 tests/converters/mannheim_buchen_test.py
 tests/converters/neckarsulm_bike_test.py
 tests/converters/neckarsulm_test.py
 tests/converters/pbw_test.py
 tests/converters/pforzheim_test.py
 tests/converters/pum_bw_test.py
+tests/converters/radvis_bw_test.py
 tests/converters/reutlingen_bike_test.py
 tests/converters/reutlingen_test.py
 tests/converters/stuttgart_test.py
 tests/converters/ulm_test.py
 tests/converters/vrs_p_r_test.py
 tests/converters/data/bahn_v2.json
 tests/converters/data/bfrk_bw_bike.csv
 tests/converters/data/bfrk_bw_car.csv
-tests/converters/data/buchen.json
+tests/converters/data/ellwangen.xlsx
 tests/converters/data/freiburg.json
 tests/converters/data/heidelberg.json
 tests/converters/data/karlsruhe.json
+tests/converters/data/karlsruhe_bike.json
 tests/converters/data/kienzler.json
+tests/converters/data/konstanz_bike.csv
 tests/converters/data/mannheim.json
 tests/converters/data/neckarsulm.csv
 tests/converters/data/neckarsulm_bike.csv
 tests/converters/data/pforzheim.json
 tests/converters/data/pum_bw.xlsx
+tests/converters/data/radvis_bw.json
 tests/converters/data/reutlingen.csv
 tests/converters/data/reutlingen_bike.csv
 tests/converters/data/stuttgart-realtime.xml
 tests/converters/data/stuttgart-static.xml
 tests/converters/data/ulm.html
 tests/converters/data/vrs_p_r.xlsx
 tests/converters/data/pbw/catalog-city.json
```

### Comparing `parkapi_sources-0.3.1/tests/converters/bahn_v2_test.py` & `parkapi_sources-0.4.0/tests/converters/bahn_v2_test.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.1/tests/converters/bfrk_bw_test.py` & `parkapi_sources-0.4.0/tests/converters/bfrk_bw_test.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.1/tests/converters/conftest.py` & `parkapi_sources-0.4.0/tests/converters/conftest.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.1/tests/converters/data/bahn_v2.json` & `parkapi_sources-0.4.0/tests/converters/data/bahn_v2.json`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.1/tests/converters/data/bfrk_bw_bike.csv` & `parkapi_sources-0.4.0/tests/converters/data/bfrk_bw_bike.csv`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.1/tests/converters/data/bfrk_bw_car.csv` & `parkapi_sources-0.4.0/tests/converters/data/bfrk_bw_car.csv`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.1/tests/converters/data/buchen.json` & `parkapi_sources-0.4.0/tests/converters/data/mannheim.json`

 * *Files 26% similar despite different names*

#### Pretty-printed

 * *Differences: {'replace': "OrderedDict([('items', [OrderedDict([('uid', 'P8_Parkdeck_Altstadt_Haagstrasse'), "*

 * *            "('name', 'P8 Parkdeck Altstadt Haagstraße'), ('operator_name', 'Stadt Buchen'), "*

 * *            "('lat', '49.52211082686668'), ('lon', '9.326514294042138'), ('address', 'Haagstraße, "*

 * *            "74722 Buchen'), ('has_realtime_data', True), ('description', 'Parkhaus Haagstrasse'), "*

 * *            "('type', 'CAR_PARK'), ('realtime_opening_status', 'UNKNOWN'), ('capacity', 60), "*

 * *            "('realtime_ […]*

```diff
@@ -1,34 +1,21 @@
-[
-    {
-        "address": {
-            "city": "Buchen",
-            "country": "Deutschland",
-            "countryCode": "de",
-            "houseNo": "",
-            "postalCode": "74722",
-            "state": "Baden-W\u00fcrttemberg",
-            "street": "Haagstra\u00dfe"
-        },
-        "capacity": 60,
-        "dataType": "parkingCar",
-        "description": "Parkhaus Haagstrasse",
-        "free": 2,
-        "id": "P8_Parkdeck_Altstadt_Haagstrasse",
-        "location": {
-            "coordinates": [
-                9.326514294042138,
-                49.52211082686668
-            ],
-            "type": "Point"
-        },
-        "name": "P8 Parkdeck Altstadt Haagstra\u00dfe",
-        "networkId": "Mobidata",
-        "operatorId": "stadt_buchen",
-        "properties": [
-            "carPark"
-        ],
-        "timestamp": "2023-12-04T11:02:00+01:00",
-        "trafficType": "car",
-        "type": "carPark"
-    }
-]
+{
+    "items": [
+        {
+            "address": "Haagstra\u00dfe, 74722 Buchen",
+            "capacity": 60,
+            "description": "Parkhaus Haagstrasse",
+            "has_realtime_data": true,
+            "lat": "49.52211082686668",
+            "lon": "9.326514294042138",
+            "name": "P8 Parkdeck Altstadt Haagstra\u00dfe",
+            "operator_name": "Stadt Buchen",
+            "realtime_capacity": 60,
+            "realtime_data_updated_at": "2024-02-20T17:05:33+01:00",
+            "realtime_free_capacity": 27,
+            "realtime_opening_status": "UNKNOWN",
+            "static_data_updated_at": "2024-02-20T17:05:33+01:00",
+            "type": "CAR_PARK",
+            "uid": "P8_Parkdeck_Altstadt_Haagstrasse"
+        }
+    ]
+}
```

### Comparing `parkapi_sources-0.3.1/tests/converters/data/freiburg.json` & `parkapi_sources-0.4.0/tests/converters/data/freiburg.json`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.1/tests/converters/data/heidelberg.json` & `parkapi_sources-0.4.0/tests/converters/data/heidelberg.json`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.1/tests/converters/data/karlsruhe.json` & `parkapi_sources-0.4.0/tests/converters/data/karlsruhe.json`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.1/tests/converters/data/kienzler.json` & `parkapi_sources-0.4.0/tests/converters/data/kienzler.json`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.1/tests/converters/data/neckarsulm.csv` & `parkapi_sources-0.4.0/tests/converters/data/neckarsulm.csv`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.1/tests/converters/data/neckarsulm_bike.csv` & `parkapi_sources-0.4.0/tests/converters/data/neckarsulm_bike.csv`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.1/tests/converters/data/pbw/catalog-city.json` & `parkapi_sources-0.4.0/tests/converters/data/pbw/catalog-city.json`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.1/tests/converters/data/pbw/object-by-city-10.json` & `parkapi_sources-0.4.0/tests/converters/data/pbw/object-by-city-10.json`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.1/tests/converters/data/pbw/object-by-city-11.json` & `parkapi_sources-0.4.0/tests/converters/data/pbw/object-by-city-11.json`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.1/tests/converters/data/pbw/object-by-city-12.json` & `parkapi_sources-0.4.0/tests/converters/data/pbw/object-by-city-12.json`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.1/tests/converters/data/pbw/object-by-city-15.json` & `parkapi_sources-0.4.0/tests/converters/data/pbw/object-by-city-15.json`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.1/tests/converters/data/pbw/object-by-city-17.json` & `parkapi_sources-0.4.0/tests/converters/data/pbw/object-by-city-17.json`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.1/tests/converters/data/pbw/object-by-city-18.json` & `parkapi_sources-0.4.0/tests/converters/data/pbw/object-by-city-18.json`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.1/tests/converters/data/pbw/object-by-city-19.json` & `parkapi_sources-0.4.0/tests/converters/data/pbw/object-by-city-19.json`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.1/tests/converters/data/pbw/object-by-city-31.json` & `parkapi_sources-0.4.0/tests/converters/data/pbw/object-by-city-31.json`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.1/tests/converters/data/pbw/object-by-city-32.json` & `parkapi_sources-0.4.0/tests/converters/data/pbw/object-by-city-32.json`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.1/tests/converters/data/pbw/object-by-city-33.json` & `parkapi_sources-0.4.0/tests/converters/data/pbw/object-by-city-33.json`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.1/tests/converters/data/pbw/object-by-city-34.json` & `parkapi_sources-0.4.0/tests/converters/data/pbw/object-by-city-34.json`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.1/tests/converters/data/pbw/object-by-city-4.json` & `parkapi_sources-0.4.0/tests/converters/data/pbw/object-by-city-4.json`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.1/tests/converters/data/pbw/object-by-city-42.json` & `parkapi_sources-0.4.0/tests/converters/data/pbw/object-by-city-42.json`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.1/tests/converters/data/pbw/object-by-city-48.json` & `parkapi_sources-0.4.0/tests/converters/data/pbw/object-by-city-48.json`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.1/tests/converters/data/pbw/object-by-city-49.json` & `parkapi_sources-0.4.0/tests/converters/data/pbw/object-by-city-49.json`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.1/tests/converters/data/pbw/object-by-city-51.json` & `parkapi_sources-0.4.0/tests/converters/data/pbw/object-by-city-51.json`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.1/tests/converters/data/pbw/object-by-city-52.json` & `parkapi_sources-0.4.0/tests/converters/data/pbw/object-by-city-52.json`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.1/tests/converters/data/pbw/object-by-city-60.json` & `parkapi_sources-0.4.0/tests/converters/data/pbw/object-by-city-60.json`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.1/tests/converters/data/pbw/object-by-city-61.json` & `parkapi_sources-0.4.0/tests/converters/data/pbw/object-by-city-61.json`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.1/tests/converters/data/pbw/object-by-city-7.json` & `parkapi_sources-0.4.0/tests/converters/data/pbw/object-by-city-7.json`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.1/tests/converters/data/pbw/object-by-city-71.json` & `parkapi_sources-0.4.0/tests/converters/data/pbw/object-by-city-71.json`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.1/tests/converters/data/pbw/object-by-city-9.json` & `parkapi_sources-0.4.0/tests/converters/data/pbw/object-by-city-9.json`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.1/tests/converters/data/pbw/object-dynamic-all.json` & `parkapi_sources-0.4.0/tests/converters/data/pbw/object-dynamic-all.json`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.1/tests/converters/data/pforzheim.json` & `parkapi_sources-0.4.0/tests/converters/data/pforzheim.json`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.1/tests/converters/data/pum_bw.xlsx` & `parkapi_sources-0.4.0/tests/converters/data/pum_bw.xlsx`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.1/tests/converters/data/reutlingen.csv` & `parkapi_sources-0.4.0/tests/converters/data/reutlingen.csv`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.1/tests/converters/data/reutlingen_bike.csv` & `parkapi_sources-0.4.0/tests/converters/data/reutlingen_bike.csv`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.1/tests/converters/data/stuttgart-realtime.xml` & `parkapi_sources-0.4.0/tests/converters/data/stuttgart-realtime.xml`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.1/tests/converters/data/stuttgart-static.xml` & `parkapi_sources-0.4.0/tests/converters/data/stuttgart-static.xml`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.1/tests/converters/data/ulm.html` & `parkapi_sources-0.4.0/tests/converters/data/ulm.html`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.1/tests/converters/data/vrs_p_r.xlsx` & `parkapi_sources-0.4.0/tests/converters/data/vrs_p_r.xlsx`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.1/tests/converters/freiburg_test.py` & `parkapi_sources-0.4.0/tests/converters/freiburg_test.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.1/tests/converters/heidelberg_test.py` & `parkapi_sources-0.4.0/tests/converters/heidelberg_test.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.1/tests/converters/helper.py` & `parkapi_sources-0.4.0/tests/converters/helper.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.1/tests/converters/karlsruhe_test.py` & `parkapi_sources-0.4.0/tests/converters/karlsruhe_test.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.1/tests/converters/kienzler_test.py` & `parkapi_sources-0.4.0/tests/converters/kienzler_test.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.1/tests/converters/mannheim_buchen_test.py` & `parkapi_sources-0.4.0/tests/converters/stuttgart_test.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,54 +1,45 @@
 """
 Copyright 2024 binary butterfly GmbH
 Use of this source code is governed by an MIT-style license that can be found in the LICENSE.txt.
 """
 
-import json
 from unittest.mock import Mock
 
 import pytest
-from parkapi_sources.converters import BuchenPushConverter
-from parkapi_sources.converters.mannheim_buchen import MannheimPushConverter
-from parkapi_sources.models import RealtimeParkingSiteInput, StaticParkingSiteInput
+from lxml import etree
+from parkapi_sources.converters import StuttgartPushConverter
 
 from tests.converters.helper import get_data_path, validate_realtime_parking_site_inputs, validate_static_parking_site_inputs
 
 
 @pytest.fixture
-def mannheim_push_converter(mocked_config_helper: Mock) -> MannheimPushConverter:
-    return MannheimPushConverter(config_helper=mocked_config_helper)
+def stuttgart_push_converter(mocked_config_helper: Mock) -> StuttgartPushConverter:
+    return StuttgartPushConverter(config_helper=mocked_config_helper)
 
 
-class MannheimPullConverterTest:
+class StuttgartPullConverterTest:
     @staticmethod
-    def test_get_parking_sites(mannheim_push_converter: MannheimPushConverter):
-        with get_data_path('mannheim.json').open('br') as json_file:
-            json_data = json.load(json_file)
+    def test_get_static_parking_sites(stuttgart_push_converter: StuttgartPushConverter):
+        with get_data_path('stuttgart-static.xml').open('br') as xml_file:
+            root_element = etree.fromstring(xml_file.read(), parser=etree.XMLParser(resolve_entities=False))  # noqa: S320
 
-        parking_site_inputs, import_parking_site_exceptions = mannheim_push_converter.handle_json(json_data)
+        static_parking_site_inputs, import_parking_site_exceptions = stuttgart_push_converter.handle_xml(root_element)
 
-        assert len(parking_site_inputs) == len(json_data) * 2, 'There should be two parking sites per input dataset.'
-        assert len(import_parking_site_exceptions) == 0, 'There should be no exceptions'
+        assert len(static_parking_site_inputs) > len(
+            import_parking_site_exceptions
+        ), 'There should be more valid then invalid parking sites'
 
-        validate_static_parking_site_inputs([item for item in parking_site_inputs if isinstance(item, StaticParkingSiteInput)])
-        validate_realtime_parking_site_inputs([item for item in parking_site_inputs if isinstance(item, RealtimeParkingSiteInput)])
+        validate_static_parking_site_inputs(static_parking_site_inputs)
 
-
-@pytest.fixture
-def buchen_push_converter(mocked_config_helper: Mock) -> BuchenPushConverter:
-    return BuchenPushConverter(config_helper=mocked_config_helper)
-
-
-class BuchenPushConverterTest:
     @staticmethod
-    def test_get_parking_sites(buchen_push_converter: BuchenPushConverter):
-        with get_data_path('buchen.json').open('br') as json_file:
-            json_data = json.load(json_file)
+    def test_get_realtime_parking_sites(stuttgart_push_converter: StuttgartPushConverter):
+        with get_data_path('stuttgart-realtime.xml').open('br') as xml_file:
+            root_element = etree.fromstring(xml_file.read(), parser=etree.XMLParser(resolve_entities=False))  # noqa: S320
 
-        parking_site_inputs, import_parking_site_exceptions = buchen_push_converter.handle_json(json_data)
+        realtime_parking_site_inputs, import_parking_site_exceptions = stuttgart_push_converter.handle_xml(root_element)
 
-        assert len(parking_site_inputs) == len(json_data) * 2, 'There should be two parking sites per input dataset.'
-        assert len(import_parking_site_exceptions) == 0, 'There should be no exceptions'
+        assert len(realtime_parking_site_inputs) > len(
+            import_parking_site_exceptions
+        ), 'There should be more valid then invalid parking sites'
 
-        validate_static_parking_site_inputs([item for item in parking_site_inputs if isinstance(item, StaticParkingSiteInput)])
-        validate_realtime_parking_site_inputs([item for item in parking_site_inputs if isinstance(item, RealtimeParkingSiteInput)])
+        validate_realtime_parking_site_inputs(realtime_parking_site_inputs)
```

### Comparing `parkapi_sources-0.3.1/tests/converters/neckarsulm_bike_test.py` & `parkapi_sources-0.4.0/tests/converters/neckarsulm_bike_test.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.1/tests/converters/neckarsulm_test.py` & `parkapi_sources-0.4.0/tests/converters/neckarsulm_test.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.1/tests/converters/pbw_test.py` & `parkapi_sources-0.4.0/tests/converters/pbw_test.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.1/tests/converters/pforzheim_test.py` & `parkapi_sources-0.4.0/tests/converters/pforzheim_test.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.1/tests/converters/pum_bw_test.py` & `parkapi_sources-0.4.0/tests/converters/pum_bw_test.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.1/tests/converters/reutlingen_bike_test.py` & `parkapi_sources-0.4.0/tests/converters/reutlingen_bike_test.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.1/tests/converters/reutlingen_test.py` & `parkapi_sources-0.4.0/tests/converters/reutlingen_test.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.1/tests/converters/ulm_test.py` & `parkapi_sources-0.4.0/tests/converters/ulm_test.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.1/tests/converters/vrs_p_r_test.py` & `parkapi_sources-0.4.0/tests/converters/vrs_p_r_test.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.1/tests/models/xlsx_inputs_test.py` & `parkapi_sources-0.4.0/tests/models/xlsx_inputs_test.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.1/tests/util/data_xml_helper.py` & `parkapi_sources-0.4.0/tests/util/data_xml_helper.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.1/tests/util/encoding_test.py` & `parkapi_sources-0.4.0/tests/util/encoding_test.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.1/tests/util/xml_helper_test.py` & `parkapi_sources-0.4.0/tests/util/xml_helper_test.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.1/tests/validators/boolean_validators_test.py` & `parkapi_sources-0.4.0/tests/validators/boolean_validators_test.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.1/tests/validators/date_validators_test.py` & `parkapi_sources-0.4.0/tests/validators/date_validators_test.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.1/tests/validators/datetime_validators_test.py` & `parkapi_sources-0.4.0/tests/validators/datetime_validators_test.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.1/tests/validators/integer_validators_test.py` & `parkapi_sources-0.4.0/tests/validators/integer_validators_test.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.1/tests/validators/noneable_tests.py` & `parkapi_sources-0.4.0/tests/validators/noneable_tests.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.1/tests/validators/string_validators_test.py` & `parkapi_sources-0.4.0/tests/validators/string_validators_test.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.1/tests/validators/time_validators_test.py` & `parkapi_sources-0.4.0/tests/validators/time_validators_test.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.3.1/tox.ini` & `parkapi_sources-0.4.0/tox.ini`

 * *Files identical despite different names*

