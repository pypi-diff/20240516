# Comparing `tmp/parkapi_sources-0.4.0.tar.gz` & `tmp/parkapi_sources-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "parkapi_sources-0.4.0.tar", last modified: Thu May 16 06:35:38 2024, max compression
+gzip compressed data, was "parkapi_sources-0.4.1.tar", last modified: Thu May 16 11:32:12 2024, max compression
```

## Comparing `parkapi_sources-0.4.0.tar` & `parkapi_sources-0.4.1.tar`

### file list

```diff
@@ -1,253 +1,253 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 06:35:38.151497 parkapi_sources-0.4.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 06:35:38.107496 parkapi_sources-0.4.0/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 06:35:38.107496 parkapi_sources-0.4.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2297 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/.github/workflows/build-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1469 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/.github/workflows/lint-test.yml
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1589 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/LICENCE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      381 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)    16681 2024-05-16 06:35:38.151497 parkapi_sources-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    15147 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 06:35:38.107496 parkapi_sources-0.4.0/data/
--rw-r--r--   0 runner    (1001) docker     (127)    11453 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/data/freiburg.geojson
--rw-r--r--   0 runner    (1001) docker     (127)    11994 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/data/heidelberg.geojson
--rw-r--r--   0 runner    (1001) docker     (127)    10851 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/data/mannheim.geojson
--rw-r--r--   0 runner    (1001) docker     (127)     5300 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/data/ulm.geojson
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 06:35:38.107496 parkapi_sources-0.4.0/dev/
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/dev/parkapi.py
--rw-r--r--   0 runner    (1001) docker     (127)     3147 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/dev/test-pull-converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     4282 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/dev/test-push-converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3280 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 06:35:38.151497 parkapi_sources-0.4.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 06:35:38.099496 parkapi_sources-0.4.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 06:35:38.111496 parkapi_sources-0.4.0/src/parkapi_sources/
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/src/parkapi_sources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-16 06:35:37.000000 parkapi_sources-0.4.0/src/parkapi_sources/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 06:35:38.111496 parkapi_sources-0.4.0/src/parkapi_sources/converters/
--rw-r--r--   0 runner    (1001) docker     (127)     1247 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/src/parkapi_sources/converters/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 06:35:38.111496 parkapi_sources-0.4.0/src/parkapi_sources/converters/bahn_v2/
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/src/parkapi_sources/converters/bahn_v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3117 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/src/parkapi_sources/converters/bahn_v2/converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1823 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/src/parkapi_sources/converters/bahn_v2/mapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     3885 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/src/parkapi_sources/converters/bahn_v2/validators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 06:35:38.111496 parkapi_sources-0.4.0/src/parkapi_sources/converters/base_converter/
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/src/parkapi_sources/converters/base_converter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      829 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/src/parkapi_sources/converters/base_converter/base_converter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 06:35:38.111496 parkapi_sources-0.4.0/src/parkapi_sources/converters/base_converter/pull/
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/src/parkapi_sources/converters/base_converter/pull/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      729 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/src/parkapi_sources/converters/base_converter/pull/pull_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2809 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/src/parkapi_sources/converters/base_converter/pull/pull_scraper_mixin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 06:35:38.111496 parkapi_sources-0.4.0/src/parkapi_sources/converters/base_converter/pull/static_geojson_data_mixin/
--rw-r--r--   0 runner    (1001) docker     (127)      248 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/src/parkapi_sources/converters/base_converter/pull/static_geojson_data_mixin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3302 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/src/parkapi_sources/converters/base_converter/pull/static_geojson_data_mixin/mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     2207 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/src/parkapi_sources/converters/base_converter/pull/static_geojson_data_mixin/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 06:35:38.115496 parkapi_sources-0.4.0/src/parkapi_sources/converters/base_converter/push/
--rw-r--r--   0 runner    (1001) docker     (127)      481 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/src/parkapi_sources/converters/base_converter/push/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1518 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/src/parkapi_sources/converters/base_converter/push/csv_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)      649 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/src/parkapi_sources/converters/base_converter/push/json_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     4937 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/src/parkapi_sources/converters/base_converter/push/normalized_xlsx_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3089 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/src/parkapi_sources/converters/base_converter/push/parkapi_json_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/src/parkapi_sources/converters/base_converter/push/push_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1659 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/src/parkapi_sources/converters/base_converter/push/xlsx_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)      725 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/src/parkapi_sources/converters/base_converter/push/xml_converter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 06:35:38.115496 parkapi_sources-0.4.0/src/parkapi_sources/converters/bfrk_bw/
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/src/parkapi_sources/converters/bfrk_bw/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2061 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/src/parkapi_sources/converters/bfrk_bw/base_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2026 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/src/parkapi_sources/converters/bfrk_bw/base_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     1644 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/src/parkapi_sources/converters/bfrk_bw/bike_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2039 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/src/parkapi_sources/converters/bfrk_bw/bike_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     1628 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/src/parkapi_sources/converters/bfrk_bw/car_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1763 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/src/parkapi_sources/converters/bfrk_bw/car_models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 06:35:38.115496 parkapi_sources-0.4.0/src/parkapi_sources/converters/ellwangen/
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/src/parkapi_sources/converters/ellwangen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2102 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/src/parkapi_sources/converters/ellwangen/converter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 06:35:38.115496 parkapi_sources-0.4.0/src/parkapi_sources/converters/freiburg/
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/src/parkapi_sources/converters/freiburg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3061 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/src/parkapi_sources/converters/freiburg/converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1688 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/src/parkapi_sources/converters/freiburg/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 06:35:38.115496 parkapi_sources-0.4.0/src/parkapi_sources/converters/heidelberg/
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/src/parkapi_sources/converters/heidelberg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3458 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/src/parkapi_sources/converters/heidelberg/converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1970 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/src/parkapi_sources/converters/heidelberg/validators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 06:35:38.119496 parkapi_sources-0.4.0/src/parkapi_sources/converters/karlsruhe/
--rw-r--r--   0 runner    (1001) docker     (127)      218 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/src/parkapi_sources/converters/karlsruhe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5434 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/src/parkapi_sources/converters/karlsruhe/converter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 06:35:38.119496 parkapi_sources-0.4.0/src/parkapi_sources/converters/karlsruhe/files/
--rw-r--r--   0 runner    (1001) docker     (127)     2933 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/src/parkapi_sources/converters/karlsruhe/files/ca.crt.pem
--rw-r--r--   0 runner    (1001) docker     (127)     6626 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/src/parkapi_sources/converters/karlsruhe/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 06:35:38.119496 parkapi_sources-0.4.0/src/parkapi_sources/converters/kienzler/
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/src/parkapi_sources/converters/kienzler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3531 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/src/parkapi_sources/converters/kienzler/converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1607 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/src/parkapi_sources/converters/kienzler/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 06:35:38.119496 parkapi_sources-0.4.0/src/parkapi_sources/converters/konstanz_bike/
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/src/parkapi_sources/converters/konstanz_bike/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2540 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/src/parkapi_sources/converters/konstanz_bike/converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3521 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/src/parkapi_sources/converters/konstanz_bike/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 06:35:38.119496 parkapi_sources-0.4.0/src/parkapi_sources/converters/mannheim_buchen/
--rw-r--r--   0 runner    (1001) docker     (127)      210 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/src/parkapi_sources/converters/mannheim_buchen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      804 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/src/parkapi_sources/converters/mannheim_buchen/converter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 06:35:38.119496 parkapi_sources-0.4.0/src/parkapi_sources/converters/neckarsulm/
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/src/parkapi_sources/converters/neckarsulm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2715 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/src/parkapi_sources/converters/neckarsulm/converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3263 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/src/parkapi_sources/converters/neckarsulm/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 06:35:38.119496 parkapi_sources-0.4.0/src/parkapi_sources/converters/neckarsulm_bike/
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/src/parkapi_sources/converters/neckarsulm_bike/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3333 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/src/parkapi_sources/converters/neckarsulm_bike/converter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 06:35:38.119496 parkapi_sources-0.4.0/src/parkapi_sources/converters/pbw/
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/src/parkapi_sources/converters/pbw/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4889 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/src/parkapi_sources/converters/pbw/converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2554 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/src/parkapi_sources/converters/pbw/mapper.py
--rw-r--r--   0 runner    (1001) docker     (127)    11699 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/src/parkapi_sources/converters/pbw/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 06:35:38.123496 parkapi_sources-0.4.0/src/parkapi_sources/converters/pforzheim/
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/src/parkapi_sources/converters/pforzheim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2744 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/src/parkapi_sources/converters/pforzheim/converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1836 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/src/parkapi_sources/converters/pforzheim/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 06:35:38.123496 parkapi_sources-0.4.0/src/parkapi_sources/converters/pum_bw/
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/src/parkapi_sources/converters/pum_bw/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3096 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/src/parkapi_sources/converters/pum_bw/converter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 06:35:38.123496 parkapi_sources-0.4.0/src/parkapi_sources/converters/radvis_bw/
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/src/parkapi_sources/converters/radvis_bw/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3558 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/src/parkapi_sources/converters/radvis_bw/converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     5678 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/src/parkapi_sources/converters/radvis_bw/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 06:35:38.123496 parkapi_sources-0.4.0/src/parkapi_sources/converters/reutlingen/
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/src/parkapi_sources/converters/reutlingen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2573 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/src/parkapi_sources/converters/reutlingen/converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1805 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/src/parkapi_sources/converters/reutlingen/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 06:35:38.123496 parkapi_sources-0.4.0/src/parkapi_sources/converters/reutlingen_bike/
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/src/parkapi_sources/converters/reutlingen_bike/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2825 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/src/parkapi_sources/converters/reutlingen_bike/converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/src/parkapi_sources/converters/reutlingen_bike/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 06:35:38.123496 parkapi_sources-0.4.0/src/parkapi_sources/converters/stuttgart/
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/src/parkapi_sources/converters/stuttgart/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6424 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/src/parkapi_sources/converters/stuttgart/converter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 06:35:38.123496 parkapi_sources-0.4.0/src/parkapi_sources/converters/ulm/
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/src/parkapi_sources/converters/ulm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2316 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/src/parkapi_sources/converters/ulm/converter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 06:35:38.123496 parkapi_sources-0.4.0/src/parkapi_sources/converters/vrs_p_r/
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/src/parkapi_sources/converters/vrs_p_r/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2276 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/src/parkapi_sources/converters/vrs_p_r/vrs_p_r.py
--rw-r--r--   0 runner    (1001) docker     (127)     1288 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/src/parkapi_sources/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 06:35:38.127496 parkapi_sources-0.4.0/src/parkapi_sources/models/
--rw-r--r--   0 runner    (1001) docker     (127)      338 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/src/parkapi_sources/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/src/parkapi_sources/models/enums.py
--rw-r--r--   0 runner    (1001) docker     (127)     8380 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/src/parkapi_sources/models/parking_site_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)      661 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/src/parkapi_sources/models/source_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     4332 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/src/parkapi_sources/models/xlsx_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     3644 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/src/parkapi_sources/parkapi_sources.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 06:35:38.127496 parkapi_sources-0.4.0/src/parkapi_sources/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)     9093 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/src/parkapi_sources/scripts/parkapi.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 06:35:38.127496 parkapi_sources-0.4.0/src/parkapi_sources/util/
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/src/parkapi_sources/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/src/parkapi_sources/util/config_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/src/parkapi_sources/util/encoding.py
--rw-r--r--   0 runner    (1001) docker     (127)    10420 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/src/parkapi_sources/util/xml_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 06:35:38.127496 parkapi_sources-0.4.0/src/parkapi_sources/validators/
--rw-r--r--   0 runner    (1001) docker     (127)      675 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/src/parkapi_sources/validators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      704 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/src/parkapi_sources/validators/boolean_validators.py
--rw-r--r--   0 runner    (1001) docker     (127)      899 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/src/parkapi_sources/validators/date_validator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/src/parkapi_sources/validators/datetime_validator.py
--rw-r--r--   0 runner    (1001) docker     (127)      511 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/src/parkapi_sources/validators/decimal_validators.py
--rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/src/parkapi_sources/validators/integer_validators.py
--rw-r--r--   0 runner    (1001) docker     (127)      831 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/src/parkapi_sources/validators/list_validator.py
--rw-r--r--   0 runner    (1001) docker     (127)      743 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/src/parkapi_sources/validators/noneable.py
--rw-r--r--   0 runner    (1001) docker     (127)      994 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/src/parkapi_sources/validators/string_validators.py
--rw-r--r--   0 runner    (1001) docker     (127)      473 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/src/parkapi_sources/validators/time_validators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 06:35:38.151497 parkapi_sources-0.4.0/src/parkapi_sources.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    16681 2024-05-16 06:35:38.000000 parkapi_sources-0.4.0/src/parkapi_sources.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9252 2024-05-16 06:35:38.000000 parkapi_sources-0.4.0/src/parkapi_sources.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 06:35:38.000000 parkapi_sources-0.4.0/src/parkapi_sources.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-05-16 06:35:38.000000 parkapi_sources-0.4.0/src/parkapi_sources.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-16 06:35:38.000000 parkapi_sources-0.4.0/src/parkapi_sources.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 06:35:38.127496 parkapi_sources-0.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      320 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 06:35:38.131496 parkapi_sources-0.4.0/tests/converters/
--rw-r--r--   0 runner    (1001) docker     (127)     1744 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/tests/converters/bahn_v2_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2053 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/tests/converters/bfrk_bw_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      823 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/tests/converters/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 06:35:38.143496 parkapi_sources-0.4.0/tests/converters/data/
--rw-r--r--   0 runner    (1001) docker     (127)   947589 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/tests/converters/data/bahn_v2.json
--rw-r--r--   0 runner    (1001) docker     (127)   552854 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/tests/converters/data/bfrk_bw_bike.csv
--rw-r--r--   0 runner    (1001) docker     (127)   617384 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/tests/converters/data/bfrk_bw_car.csv
--rw-r--r--   0 runner    (1001) docker     (127)    41226 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/tests/converters/data/ellwangen.xlsx
--rw-r--r--   0 runner    (1001) docker     (127)    12651 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/tests/converters/data/freiburg.json
--rw-r--r--   0 runner    (1001) docker     (127)     3681 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/tests/converters/data/heidelberg.json
--rw-r--r--   0 runner    (1001) docker     (127)    63706 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/tests/converters/data/karlsruhe.json
--rw-r--r--   0 runner    (1001) docker     (127)   252177 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/tests/converters/data/karlsruhe_bike.json
--rw-r--r--   0 runner    (1001) docker     (127)     3477 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/tests/converters/data/kienzler.json
--rw-r--r--   0 runner    (1001) docker     (127)    59377 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/tests/converters/data/konstanz_bike.csv
--rw-r--r--   0 runner    (1001) docker     (127)      666 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/tests/converters/data/mannheim.json
--rw-r--r--   0 runner    (1001) docker     (127)    20667 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/tests/converters/data/neckarsulm.csv
--rw-r--r--   0 runner    (1001) docker     (127)    18115 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/tests/converters/data/neckarsulm_bike.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 06:35:38.147496 parkapi_sources-0.4.0/tests/converters/data/pbw/
--rw-r--r--   0 runner    (1001) docker     (127)     1251 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/tests/converters/data/pbw/catalog-city.json
--rw-r--r--   0 runner    (1001) docker     (127)   114816 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/tests/converters/data/pbw/object-by-city-10.json
--rw-r--r--   0 runner    (1001) docker     (127)     5061 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/tests/converters/data/pbw/object-by-city-11.json
--rw-r--r--   0 runner    (1001) docker     (127)    36083 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/tests/converters/data/pbw/object-by-city-12.json
--rw-r--r--   0 runner    (1001) docker     (127)     1784 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/tests/converters/data/pbw/object-by-city-15.json
--rw-r--r--   0 runner    (1001) docker     (127)     6859 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/tests/converters/data/pbw/object-by-city-17.json
--rw-r--r--   0 runner    (1001) docker     (127)     7122 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/tests/converters/data/pbw/object-by-city-18.json
--rw-r--r--   0 runner    (1001) docker     (127)     5812 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/tests/converters/data/pbw/object-by-city-19.json
--rw-r--r--   0 runner    (1001) docker     (127)     5795 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/tests/converters/data/pbw/object-by-city-31.json
--rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/tests/converters/data/pbw/object-by-city-32.json
--rw-r--r--   0 runner    (1001) docker     (127)     6650 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/tests/converters/data/pbw/object-by-city-33.json
--rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/tests/converters/data/pbw/object-by-city-34.json
--rw-r--r--   0 runner    (1001) docker     (127)     3225 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/tests/converters/data/pbw/object-by-city-4.json
--rw-r--r--   0 runner    (1001) docker     (127)     3187 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/tests/converters/data/pbw/object-by-city-42.json
--rw-r--r--   0 runner    (1001) docker     (127)     3296 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/tests/converters/data/pbw/object-by-city-48.json
--rw-r--r--   0 runner    (1001) docker     (127)     1597 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/tests/converters/data/pbw/object-by-city-49.json
--rw-r--r--   0 runner    (1001) docker     (127)     3241 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/tests/converters/data/pbw/object-by-city-51.json
--rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/tests/converters/data/pbw/object-by-city-52.json
--rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/tests/converters/data/pbw/object-by-city-60.json
--rw-r--r--   0 runner    (1001) docker     (127)     1557 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/tests/converters/data/pbw/object-by-city-61.json
--rw-r--r--   0 runner    (1001) docker     (127)    14227 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/tests/converters/data/pbw/object-by-city-7.json
--rw-r--r--   0 runner    (1001) docker     (127)     3149 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/tests/converters/data/pbw/object-by-city-71.json
--rw-r--r--   0 runner    (1001) docker     (127)     7071 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/tests/converters/data/pbw/object-by-city-9.json
--rw-r--r--   0 runner    (1001) docker     (127)     6685 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/tests/converters/data/pbw/object-dynamic-all.json
--rw-r--r--   0 runner    (1001) docker     (127)    18956 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/tests/converters/data/pforzheim.json
--rw-r--r--   0 runner    (1001) docker     (127)    30849 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/tests/converters/data/pum_bw.xlsx
--rw-r--r--   0 runner    (1001) docker     (127)   526873 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/tests/converters/data/radvis_bw.json
--rw-r--r--   0 runner    (1001) docker     (127)     9387 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/tests/converters/data/reutlingen.csv
--rw-r--r--   0 runner    (1001) docker     (127)    27295 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/tests/converters/data/reutlingen_bike.csv
--rw-r--r--   0 runner    (1001) docker     (127)    35423 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/tests/converters/data/stuttgart-realtime.xml
--rw-r--r--   0 runner    (1001) docker     (127)   218959 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/tests/converters/data/stuttgart-static.xml
--rw-r--r--   0 runner    (1001) docker     (127)    62841 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/tests/converters/data/ulm.html
--rw-r--r--   0 runner    (1001) docker     (127)   136171 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/tests/converters/data/vrs_p_r.xlsx
--rw-r--r--   0 runner    (1001) docker     (127)     1149 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/tests/converters/ellwangen_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1859 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/tests/converters/freiburg_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2226 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/tests/converters/heidelberg_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2439 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/tests/converters/helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     1979 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/tests/converters/karlsruhe_bike_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1926 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/tests/converters/karlsruhe_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/tests/converters/kienzler_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/tests/converters/konstanz_bike_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1546 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/tests/converters/mannheim_buchen_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/tests/converters/neckarsulm_bike_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/tests/converters/neckarsulm_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2880 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/tests/converters/pbw_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/tests/converters/pforzheim_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/tests/converters/pum_bw_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1705 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/tests/converters/radvis_bw_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1246 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/tests/converters/reutlingen_bike_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/tests/converters/reutlingen_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1949 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/tests/converters/stuttgart_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1777 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/tests/converters/ulm_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/tests/converters/vrs_p_r_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 06:35:38.147496 parkapi_sources-0.4.0/tests/models/
--rw-r--r--   0 runner    (1001) docker     (127)     2183 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/tests/models/xlsx_inputs_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 06:35:38.147496 parkapi_sources-0.4.0/tests/util/
--rw-r--r--   0 runner    (1001) docker     (127)     4105 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/tests/util/data_xml_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     1706 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/tests/util/encoding_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     4039 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/tests/util/xml_helper_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 06:35:38.151497 parkapi_sources-0.4.0/tests/validators/
--rw-r--r--   0 runner    (1001) docker     (127)     1255 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/tests/validators/boolean_validators_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/tests/validators/date_validators_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2108 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/tests/validators/datetime_validators_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/tests/validators/integer_validators_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/tests/validators/noneable_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/tests/validators/string_validators_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      567 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/tests/validators/time_validators_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-16 06:35:33.000000 parkapi_sources-0.4.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:32:12.636774 parkapi_sources-0.4.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:32:12.600774 parkapi_sources-0.4.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-05-16 11:32:08.000000 parkapi_sources-0.4.1/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:32:12.600774 parkapi_sources-0.4.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2297 2024-05-16 11:32:08.000000 parkapi_sources-0.4.1/.github/workflows/build-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1469 2024-05-16 11:32:08.000000 parkapi_sources-0.4.1/.github/workflows/lint-test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-16 11:32:08.000000 parkapi_sources-0.4.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-05-16 11:32:08.000000 parkapi_sources-0.4.1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-05-16 11:32:08.000000 parkapi_sources-0.4.1/LICENCE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      381 2024-05-16 11:32:08.000000 parkapi_sources-0.4.1/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)    16681 2024-05-16 11:32:12.636774 parkapi_sources-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    15147 2024-05-16 11:32:08.000000 parkapi_sources-0.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:32:12.600774 parkapi_sources-0.4.1/data/
+-rw-r--r--   0 runner    (1001) docker     (127)    11453 2024-05-16 11:32:08.000000 parkapi_sources-0.4.1/data/freiburg.geojson
+-rw-r--r--   0 runner    (1001) docker     (127)    11994 2024-05-16 11:32:08.000000 parkapi_sources-0.4.1/data/heidelberg.geojson
+-rw-r--r--   0 runner    (1001) docker     (127)    10851 2024-05-16 11:32:08.000000 parkapi_sources-0.4.1/data/mannheim.geojson
+-rw-r--r--   0 runner    (1001) docker     (127)     5300 2024-05-16 11:32:08.000000 parkapi_sources-0.4.1/data/ulm.geojson
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:32:12.600774 parkapi_sources-0.4.1/dev/
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-16 11:32:08.000000 parkapi_sources-0.4.1/dev/parkapi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3147 2024-05-16 11:32:08.000000 parkapi_sources-0.4.1/dev/test-pull-converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4282 2024-05-16 11:32:08.000000 parkapi_sources-0.4.1/dev/test-push-converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3280 2024-05-16 11:32:08.000000 parkapi_sources-0.4.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-16 11:32:08.000000 parkapi_sources-0.4.1/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-16 11:32:08.000000 parkapi_sources-0.4.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 11:32:12.636774 parkapi_sources-0.4.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:32:12.592774 parkapi_sources-0.4.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:32:12.600774 parkapi_sources-0.4.1/src/parkapi_sources/
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-05-16 11:32:08.000000 parkapi_sources-0.4.1/src/parkapi_sources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-16 11:32:12.000000 parkapi_sources-0.4.1/src/parkapi_sources/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:32:12.600774 parkapi_sources-0.4.1/src/parkapi_sources/converters/
+-rw-r--r--   0 runner    (1001) docker     (127)     1247 2024-05-16 11:32:08.000000 parkapi_sources-0.4.1/src/parkapi_sources/converters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:32:12.604774 parkapi_sources-0.4.1/src/parkapi_sources/converters/bahn_v2/
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-16 11:32:08.000000 parkapi_sources-0.4.1/src/parkapi_sources/converters/bahn_v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3117 2024-05-16 11:32:08.000000 parkapi_sources-0.4.1/src/parkapi_sources/converters/bahn_v2/converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1823 2024-05-16 11:32:08.000000 parkapi_sources-0.4.1/src/parkapi_sources/converters/bahn_v2/mapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3885 2024-05-16 11:32:08.000000 parkapi_sources-0.4.1/src/parkapi_sources/converters/bahn_v2/validators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:32:12.604774 parkapi_sources-0.4.1/src/parkapi_sources/converters/base_converter/
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-16 11:32:08.000000 parkapi_sources-0.4.1/src/parkapi_sources/converters/base_converter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      829 2024-05-16 11:32:08.000000 parkapi_sources-0.4.1/src/parkapi_sources/converters/base_converter/base_converter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:32:12.604774 parkapi_sources-0.4.1/src/parkapi_sources/converters/base_converter/pull/
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-05-16 11:32:08.000000 parkapi_sources-0.4.1/src/parkapi_sources/converters/base_converter/pull/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      729 2024-05-16 11:32:08.000000 parkapi_sources-0.4.1/src/parkapi_sources/converters/base_converter/pull/pull_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2809 2024-05-16 11:32:08.000000 parkapi_sources-0.4.1/src/parkapi_sources/converters/base_converter/pull/pull_scraper_mixin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:32:12.604774 parkapi_sources-0.4.1/src/parkapi_sources/converters/base_converter/pull/static_geojson_data_mixin/
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-05-16 11:32:08.000000 parkapi_sources-0.4.1/src/parkapi_sources/converters/base_converter/pull/static_geojson_data_mixin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3302 2024-05-16 11:32:08.000000 parkapi_sources-0.4.1/src/parkapi_sources/converters/base_converter/pull/static_geojson_data_mixin/mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2207 2024-05-16 11:32:08.000000 parkapi_sources-0.4.1/src/parkapi_sources/converters/base_converter/pull/static_geojson_data_mixin/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:32:12.604774 parkapi_sources-0.4.1/src/parkapi_sources/converters/base_converter/push/
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-05-16 11:32:08.000000 parkapi_sources-0.4.1/src/parkapi_sources/converters/base_converter/push/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1518 2024-05-16 11:32:08.000000 parkapi_sources-0.4.1/src/parkapi_sources/converters/base_converter/push/csv_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2024-05-16 11:32:08.000000 parkapi_sources-0.4.1/src/parkapi_sources/converters/base_converter/push/json_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4937 2024-05-16 11:32:08.000000 parkapi_sources-0.4.1/src/parkapi_sources/converters/base_converter/push/normalized_xlsx_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3089 2024-05-16 11:32:08.000000 parkapi_sources-0.4.1/src/parkapi_sources/converters/base_converter/push/parkapi_json_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-05-16 11:32:08.000000 parkapi_sources-0.4.1/src/parkapi_sources/converters/base_converter/push/push_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1659 2024-05-16 11:32:08.000000 parkapi_sources-0.4.1/src/parkapi_sources/converters/base_converter/push/xlsx_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      725 2024-05-16 11:32:08.000000 parkapi_sources-0.4.1/src/parkapi_sources/converters/base_converter/push/xml_converter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:32:12.608774 parkapi_sources-0.4.1/src/parkapi_sources/converters/bfrk_bw/
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-16 11:32:08.000000 parkapi_sources-0.4.1/src/parkapi_sources/converters/bfrk_bw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2061 2024-05-16 11:32:08.000000 parkapi_sources-0.4.1/src/parkapi_sources/converters/bfrk_bw/base_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2026 2024-05-16 11:32:08.000000 parkapi_sources-0.4.1/src/parkapi_sources/converters/bfrk_bw/base_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1644 2024-05-16 11:32:08.000000 parkapi_sources-0.4.1/src/parkapi_sources/converters/bfrk_bw/bike_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2039 2024-05-16 11:32:08.000000 parkapi_sources-0.4.1/src/parkapi_sources/converters/bfrk_bw/bike_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1628 2024-05-16 11:32:08.000000 parkapi_sources-0.4.1/src/parkapi_sources/converters/bfrk_bw/car_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1763 2024-05-16 11:32:08.000000 parkapi_sources-0.4.1/src/parkapi_sources/converters/bfrk_bw/car_models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:32:12.608774 parkapi_sources-0.4.1/src/parkapi_sources/converters/ellwangen/
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-16 11:32:08.000000 parkapi_sources-0.4.1/src/parkapi_sources/converters/ellwangen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2102 2024-05-16 11:32:08.000000 parkapi_sources-0.4.1/src/parkapi_sources/converters/ellwangen/converter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:32:12.608774 parkapi_sources-0.4.1/src/parkapi_sources/converters/freiburg/
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-16 11:32:08.000000 parkapi_sources-0.4.1/src/parkapi_sources/converters/freiburg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3061 2024-05-16 11:32:08.000000 parkapi_sources-0.4.1/src/parkapi_sources/converters/freiburg/converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1688 2024-05-16 11:32:08.000000 parkapi_sources-0.4.1/src/parkapi_sources/converters/freiburg/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:32:12.608774 parkapi_sources-0.4.1/src/parkapi_sources/converters/heidelberg/
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-16 11:32:08.000000 parkapi_sources-0.4.1/src/parkapi_sources/converters/heidelberg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3458 2024-05-16 11:32:08.000000 parkapi_sources-0.4.1/src/parkapi_sources/converters/heidelberg/converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1970 2024-05-16 11:32:08.000000 parkapi_sources-0.4.1/src/parkapi_sources/converters/heidelberg/validators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:32:12.608774 parkapi_sources-0.4.1/src/parkapi_sources/converters/karlsruhe/
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-05-16 11:32:08.000000 parkapi_sources-0.4.1/src/parkapi_sources/converters/karlsruhe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5439 2024-05-16 11:32:08.000000 parkapi_sources-0.4.1/src/parkapi_sources/converters/karlsruhe/converter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:32:12.608774 parkapi_sources-0.4.1/src/parkapi_sources/converters/karlsruhe/files/
+-rw-r--r--   0 runner    (1001) docker     (127)     2933 2024-05-16 11:32:08.000000 parkapi_sources-0.4.1/src/parkapi_sources/converters/karlsruhe/files/ca.crt.pem
+-rw-r--r--   0 runner    (1001) docker     (127)     6678 2024-05-16 11:32:08.000000 parkapi_sources-0.4.1/src/parkapi_sources/converters/karlsruhe/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:32:12.608774 parkapi_sources-0.4.1/src/parkapi_sources/converters/kienzler/
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-16 11:32:08.000000 parkapi_sources-0.4.1/src/parkapi_sources/converters/kienzler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3531 2024-05-16 11:32:08.000000 parkapi_sources-0.4.1/src/parkapi_sources/converters/kienzler/converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1607 2024-05-16 11:32:08.000000 parkapi_sources-0.4.1/src/parkapi_sources/converters/kienzler/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:32:12.608774 parkapi_sources-0.4.1/src/parkapi_sources/converters/konstanz_bike/
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-16 11:32:08.000000 parkapi_sources-0.4.1/src/parkapi_sources/converters/konstanz_bike/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2540 2024-05-16 11:32:08.000000 parkapi_sources-0.4.1/src/parkapi_sources/converters/konstanz_bike/converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3572 2024-05-16 11:32:08.000000 parkapi_sources-0.4.1/src/parkapi_sources/converters/konstanz_bike/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:32:12.608774 parkapi_sources-0.4.1/src/parkapi_sources/converters/mannheim_buchen/
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-05-16 11:32:08.000000 parkapi_sources-0.4.1/src/parkapi_sources/converters/mannheim_buchen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2024-05-16 11:32:08.000000 parkapi_sources-0.4.1/src/parkapi_sources/converters/mannheim_buchen/converter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:32:12.608774 parkapi_sources-0.4.1/src/parkapi_sources/converters/neckarsulm/
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-16 11:32:08.000000 parkapi_sources-0.4.1/src/parkapi_sources/converters/neckarsulm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2715 2024-05-16 11:32:08.000000 parkapi_sources-0.4.1/src/parkapi_sources/converters/neckarsulm/converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3263 2024-05-16 11:32:08.000000 parkapi_sources-0.4.1/src/parkapi_sources/converters/neckarsulm/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:32:12.608774 parkapi_sources-0.4.1/src/parkapi_sources/converters/neckarsulm_bike/
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-05-16 11:32:08.000000 parkapi_sources-0.4.1/src/parkapi_sources/converters/neckarsulm_bike/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3333 2024-05-16 11:32:08.000000 parkapi_sources-0.4.1/src/parkapi_sources/converters/neckarsulm_bike/converter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:32:12.612774 parkapi_sources-0.4.1/src/parkapi_sources/converters/pbw/
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-16 11:32:08.000000 parkapi_sources-0.4.1/src/parkapi_sources/converters/pbw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4889 2024-05-16 11:32:08.000000 parkapi_sources-0.4.1/src/parkapi_sources/converters/pbw/converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2554 2024-05-16 11:32:08.000000 parkapi_sources-0.4.1/src/parkapi_sources/converters/pbw/mapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11699 2024-05-16 11:32:08.000000 parkapi_sources-0.4.1/src/parkapi_sources/converters/pbw/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:32:12.612774 parkapi_sources-0.4.1/src/parkapi_sources/converters/pforzheim/
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-16 11:32:08.000000 parkapi_sources-0.4.1/src/parkapi_sources/converters/pforzheim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2744 2024-05-16 11:32:08.000000 parkapi_sources-0.4.1/src/parkapi_sources/converters/pforzheim/converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1836 2024-05-16 11:32:08.000000 parkapi_sources-0.4.1/src/parkapi_sources/converters/pforzheim/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:32:12.612774 parkapi_sources-0.4.1/src/parkapi_sources/converters/pum_bw/
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-16 11:32:08.000000 parkapi_sources-0.4.1/src/parkapi_sources/converters/pum_bw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3096 2024-05-16 11:32:08.000000 parkapi_sources-0.4.1/src/parkapi_sources/converters/pum_bw/converter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:32:12.612774 parkapi_sources-0.4.1/src/parkapi_sources/converters/radvis_bw/
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-16 11:32:08.000000 parkapi_sources-0.4.1/src/parkapi_sources/converters/radvis_bw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3680 2024-05-16 11:32:08.000000 parkapi_sources-0.4.1/src/parkapi_sources/converters/radvis_bw/converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5678 2024-05-16 11:32:08.000000 parkapi_sources-0.4.1/src/parkapi_sources/converters/radvis_bw/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:32:12.612774 parkapi_sources-0.4.1/src/parkapi_sources/converters/reutlingen/
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-16 11:32:08.000000 parkapi_sources-0.4.1/src/parkapi_sources/converters/reutlingen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2573 2024-05-16 11:32:08.000000 parkapi_sources-0.4.1/src/parkapi_sources/converters/reutlingen/converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1805 2024-05-16 11:32:08.000000 parkapi_sources-0.4.1/src/parkapi_sources/converters/reutlingen/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:32:12.612774 parkapi_sources-0.4.1/src/parkapi_sources/converters/reutlingen_bike/
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-05-16 11:32:08.000000 parkapi_sources-0.4.1/src/parkapi_sources/converters/reutlingen_bike/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2825 2024-05-16 11:32:08.000000 parkapi_sources-0.4.1/src/parkapi_sources/converters/reutlingen_bike/converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-05-16 11:32:08.000000 parkapi_sources-0.4.1/src/parkapi_sources/converters/reutlingen_bike/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:32:12.612774 parkapi_sources-0.4.1/src/parkapi_sources/converters/stuttgart/
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-16 11:32:08.000000 parkapi_sources-0.4.1/src/parkapi_sources/converters/stuttgart/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6424 2024-05-16 11:32:08.000000 parkapi_sources-0.4.1/src/parkapi_sources/converters/stuttgart/converter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:32:12.612774 parkapi_sources-0.4.1/src/parkapi_sources/converters/ulm/
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-16 11:32:08.000000 parkapi_sources-0.4.1/src/parkapi_sources/converters/ulm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2316 2024-05-16 11:32:08.000000 parkapi_sources-0.4.1/src/parkapi_sources/converters/ulm/converter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:32:12.612774 parkapi_sources-0.4.1/src/parkapi_sources/converters/vrs_p_r/
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-16 11:32:08.000000 parkapi_sources-0.4.1/src/parkapi_sources/converters/vrs_p_r/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2276 2024-05-16 11:32:08.000000 parkapi_sources-0.4.1/src/parkapi_sources/converters/vrs_p_r/vrs_p_r.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1288 2024-05-16 11:32:08.000000 parkapi_sources-0.4.1/src/parkapi_sources/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:32:12.616774 parkapi_sources-0.4.1/src/parkapi_sources/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2024-05-16 11:32:08.000000 parkapi_sources-0.4.1/src/parkapi_sources/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-05-16 11:32:08.000000 parkapi_sources-0.4.1/src/parkapi_sources/models/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8295 2024-05-16 11:32:08.000000 parkapi_sources-0.4.1/src/parkapi_sources/models/parking_site_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      661 2024-05-16 11:32:08.000000 parkapi_sources-0.4.1/src/parkapi_sources/models/source_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4332 2024-05-16 11:32:08.000000 parkapi_sources-0.4.1/src/parkapi_sources/models/xlsx_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3644 2024-05-16 11:32:08.000000 parkapi_sources-0.4.1/src/parkapi_sources/parkapi_sources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:32:12.616774 parkapi_sources-0.4.1/src/parkapi_sources/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)     9093 2024-05-16 11:32:08.000000 parkapi_sources-0.4.1/src/parkapi_sources/scripts/parkapi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:32:12.616774 parkapi_sources-0.4.1/src/parkapi_sources/util/
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-05-16 11:32:08.000000 parkapi_sources-0.4.1/src/parkapi_sources/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-16 11:32:08.000000 parkapi_sources-0.4.1/src/parkapi_sources/util/config_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-05-16 11:32:08.000000 parkapi_sources-0.4.1/src/parkapi_sources/util/encoding.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10420 2024-05-16 11:32:08.000000 parkapi_sources-0.4.1/src/parkapi_sources/util/xml_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:32:12.616774 parkapi_sources-0.4.1/src/parkapi_sources/validators/
+-rw-r--r--   0 runner    (1001) docker     (127)      675 2024-05-16 11:32:08.000000 parkapi_sources-0.4.1/src/parkapi_sources/validators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      704 2024-05-16 11:32:08.000000 parkapi_sources-0.4.1/src/parkapi_sources/validators/boolean_validators.py
+-rw-r--r--   0 runner    (1001) docker     (127)      899 2024-05-16 11:32:08.000000 parkapi_sources-0.4.1/src/parkapi_sources/validators/date_validator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-05-16 11:32:08.000000 parkapi_sources-0.4.1/src/parkapi_sources/validators/datetime_validator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      511 2024-05-16 11:32:08.000000 parkapi_sources-0.4.1/src/parkapi_sources/validators/decimal_validators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-05-16 11:32:08.000000 parkapi_sources-0.4.1/src/parkapi_sources/validators/integer_validators.py
+-rw-r--r--   0 runner    (1001) docker     (127)      831 2024-05-16 11:32:08.000000 parkapi_sources-0.4.1/src/parkapi_sources/validators/list_validator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      743 2024-05-16 11:32:08.000000 parkapi_sources-0.4.1/src/parkapi_sources/validators/noneable.py
+-rw-r--r--   0 runner    (1001) docker     (127)      994 2024-05-16 11:32:08.000000 parkapi_sources-0.4.1/src/parkapi_sources/validators/string_validators.py
+-rw-r--r--   0 runner    (1001) docker     (127)      473 2024-05-16 11:32:08.000000 parkapi_sources-0.4.1/src/parkapi_sources/validators/time_validators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:32:12.636774 parkapi_sources-0.4.1/src/parkapi_sources.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    16681 2024-05-16 11:32:12.000000 parkapi_sources-0.4.1/src/parkapi_sources.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9252 2024-05-16 11:32:12.000000 parkapi_sources-0.4.1/src/parkapi_sources.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 11:32:12.000000 parkapi_sources-0.4.1/src/parkapi_sources.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-05-16 11:32:12.000000 parkapi_sources-0.4.1/src/parkapi_sources.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-16 11:32:12.000000 parkapi_sources-0.4.1/src/parkapi_sources.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:32:12.616774 parkapi_sources-0.4.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-05-16 11:32:08.000000 parkapi_sources-0.4.1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:32:12.620774 parkapi_sources-0.4.1/tests/converters/
+-rw-r--r--   0 runner    (1001) docker     (127)     1744 2024-05-16 11:32:08.000000 parkapi_sources-0.4.1/tests/converters/bahn_v2_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2053 2024-05-16 11:32:08.000000 parkapi_sources-0.4.1/tests/converters/bfrk_bw_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      823 2024-05-16 11:32:08.000000 parkapi_sources-0.4.1/tests/converters/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:32:12.628774 parkapi_sources-0.4.1/tests/converters/data/
+-rw-r--r--   0 runner    (1001) docker     (127)   947589 2024-05-16 11:32:08.000000 parkapi_sources-0.4.1/tests/converters/data/bahn_v2.json
+-rw-r--r--   0 runner    (1001) docker     (127)   552854 2024-05-16 11:32:08.000000 parkapi_sources-0.4.1/tests/converters/data/bfrk_bw_bike.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   617384 2024-05-16 11:32:08.000000 parkapi_sources-0.4.1/tests/converters/data/bfrk_bw_car.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    41226 2024-05-16 11:32:08.000000 parkapi_sources-0.4.1/tests/converters/data/ellwangen.xlsx
+-rw-r--r--   0 runner    (1001) docker     (127)    12651 2024-05-16 11:32:08.000000 parkapi_sources-0.4.1/tests/converters/data/freiburg.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3681 2024-05-16 11:32:08.000000 parkapi_sources-0.4.1/tests/converters/data/heidelberg.json
+-rw-r--r--   0 runner    (1001) docker     (127)    45865 2024-05-16 11:32:08.000000 parkapi_sources-0.4.1/tests/converters/data/karlsruhe.json
+-rw-r--r--   0 runner    (1001) docker     (127)   252177 2024-05-16 11:32:08.000000 parkapi_sources-0.4.1/tests/converters/data/karlsruhe_bike.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3477 2024-05-16 11:32:08.000000 parkapi_sources-0.4.1/tests/converters/data/kienzler.json
+-rw-r--r--   0 runner    (1001) docker     (127)    59377 2024-05-16 11:32:08.000000 parkapi_sources-0.4.1/tests/converters/data/konstanz_bike.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      666 2024-05-16 11:32:08.000000 parkapi_sources-0.4.1/tests/converters/data/mannheim.json
+-rw-r--r--   0 runner    (1001) docker     (127)    20667 2024-05-16 11:32:08.000000 parkapi_sources-0.4.1/tests/converters/data/neckarsulm.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    18115 2024-05-16 11:32:08.000000 parkapi_sources-0.4.1/tests/converters/data/neckarsulm_bike.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:32:12.632774 parkapi_sources-0.4.1/tests/converters/data/pbw/
+-rw-r--r--   0 runner    (1001) docker     (127)     1251 2024-05-16 11:32:08.000000 parkapi_sources-0.4.1/tests/converters/data/pbw/catalog-city.json
+-rw-r--r--   0 runner    (1001) docker     (127)   114816 2024-05-16 11:32:08.000000 parkapi_sources-0.4.1/tests/converters/data/pbw/object-by-city-10.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5061 2024-05-16 11:32:08.000000 parkapi_sources-0.4.1/tests/converters/data/pbw/object-by-city-11.json
+-rw-r--r--   0 runner    (1001) docker     (127)    36083 2024-05-16 11:32:08.000000 parkapi_sources-0.4.1/tests/converters/data/pbw/object-by-city-12.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1784 2024-05-16 11:32:08.000000 parkapi_sources-0.4.1/tests/converters/data/pbw/object-by-city-15.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6859 2024-05-16 11:32:08.000000 parkapi_sources-0.4.1/tests/converters/data/pbw/object-by-city-17.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7122 2024-05-16 11:32:08.000000 parkapi_sources-0.4.1/tests/converters/data/pbw/object-by-city-18.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5812 2024-05-16 11:32:08.000000 parkapi_sources-0.4.1/tests/converters/data/pbw/object-by-city-19.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5795 2024-05-16 11:32:08.000000 parkapi_sources-0.4.1/tests/converters/data/pbw/object-by-city-31.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-05-16 11:32:08.000000 parkapi_sources-0.4.1/tests/converters/data/pbw/object-by-city-32.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6650 2024-05-16 11:32:08.000000 parkapi_sources-0.4.1/tests/converters/data/pbw/object-by-city-33.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-05-16 11:32:08.000000 parkapi_sources-0.4.1/tests/converters/data/pbw/object-by-city-34.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3225 2024-05-16 11:32:08.000000 parkapi_sources-0.4.1/tests/converters/data/pbw/object-by-city-4.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3187 2024-05-16 11:32:08.000000 parkapi_sources-0.4.1/tests/converters/data/pbw/object-by-city-42.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3296 2024-05-16 11:32:08.000000 parkapi_sources-0.4.1/tests/converters/data/pbw/object-by-city-48.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1597 2024-05-16 11:32:08.000000 parkapi_sources-0.4.1/tests/converters/data/pbw/object-by-city-49.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3241 2024-05-16 11:32:08.000000 parkapi_sources-0.4.1/tests/converters/data/pbw/object-by-city-51.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-05-16 11:32:08.000000 parkapi_sources-0.4.1/tests/converters/data/pbw/object-by-city-52.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-05-16 11:32:08.000000 parkapi_sources-0.4.1/tests/converters/data/pbw/object-by-city-60.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1557 2024-05-16 11:32:08.000000 parkapi_sources-0.4.1/tests/converters/data/pbw/object-by-city-61.json
+-rw-r--r--   0 runner    (1001) docker     (127)    14227 2024-05-16 11:32:08.000000 parkapi_sources-0.4.1/tests/converters/data/pbw/object-by-city-7.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3149 2024-05-16 11:32:08.000000 parkapi_sources-0.4.1/tests/converters/data/pbw/object-by-city-71.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7071 2024-05-16 11:32:08.000000 parkapi_sources-0.4.1/tests/converters/data/pbw/object-by-city-9.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6685 2024-05-16 11:32:08.000000 parkapi_sources-0.4.1/tests/converters/data/pbw/object-dynamic-all.json
+-rw-r--r--   0 runner    (1001) docker     (127)    18956 2024-05-16 11:32:08.000000 parkapi_sources-0.4.1/tests/converters/data/pforzheim.json
+-rw-r--r--   0 runner    (1001) docker     (127)    30849 2024-05-16 11:32:08.000000 parkapi_sources-0.4.1/tests/converters/data/pum_bw.xlsx
+-rw-r--r--   0 runner    (1001) docker     (127)   526873 2024-05-16 11:32:08.000000 parkapi_sources-0.4.1/tests/converters/data/radvis_bw.json
+-rw-r--r--   0 runner    (1001) docker     (127)     9387 2024-05-16 11:32:08.000000 parkapi_sources-0.4.1/tests/converters/data/reutlingen.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    27295 2024-05-16 11:32:08.000000 parkapi_sources-0.4.1/tests/converters/data/reutlingen_bike.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    35423 2024-05-16 11:32:08.000000 parkapi_sources-0.4.1/tests/converters/data/stuttgart-realtime.xml
+-rw-r--r--   0 runner    (1001) docker     (127)   218959 2024-05-16 11:32:08.000000 parkapi_sources-0.4.1/tests/converters/data/stuttgart-static.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    62841 2024-05-16 11:32:08.000000 parkapi_sources-0.4.1/tests/converters/data/ulm.html
+-rw-r--r--   0 runner    (1001) docker     (127)   136171 2024-05-16 11:32:08.000000 parkapi_sources-0.4.1/tests/converters/data/vrs_p_r.xlsx
+-rw-r--r--   0 runner    (1001) docker     (127)     1149 2024-05-16 11:32:08.000000 parkapi_sources-0.4.1/tests/converters/ellwangen_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1859 2024-05-16 11:32:08.000000 parkapi_sources-0.4.1/tests/converters/freiburg_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2226 2024-05-16 11:32:08.000000 parkapi_sources-0.4.1/tests/converters/heidelberg_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2439 2024-05-16 11:32:08.000000 parkapi_sources-0.4.1/tests/converters/helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1979 2024-05-16 11:32:08.000000 parkapi_sources-0.4.1/tests/converters/karlsruhe_bike_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1926 2024-05-16 11:32:08.000000 parkapi_sources-0.4.1/tests/converters/karlsruhe_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-05-16 11:32:08.000000 parkapi_sources-0.4.1/tests/converters/kienzler_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-05-16 11:32:08.000000 parkapi_sources-0.4.1/tests/converters/konstanz_bike_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1546 2024-05-16 11:32:08.000000 parkapi_sources-0.4.1/tests/converters/mannheim_buchen_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-05-16 11:32:08.000000 parkapi_sources-0.4.1/tests/converters/neckarsulm_bike_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-05-16 11:32:08.000000 parkapi_sources-0.4.1/tests/converters/neckarsulm_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2880 2024-05-16 11:32:08.000000 parkapi_sources-0.4.1/tests/converters/pbw_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-05-16 11:32:08.000000 parkapi_sources-0.4.1/tests/converters/pforzheim_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-05-16 11:32:08.000000 parkapi_sources-0.4.1/tests/converters/pum_bw_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1705 2024-05-16 11:32:08.000000 parkapi_sources-0.4.1/tests/converters/radvis_bw_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1246 2024-05-16 11:32:08.000000 parkapi_sources-0.4.1/tests/converters/reutlingen_bike_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-05-16 11:32:08.000000 parkapi_sources-0.4.1/tests/converters/reutlingen_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1949 2024-05-16 11:32:08.000000 parkapi_sources-0.4.1/tests/converters/stuttgart_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1777 2024-05-16 11:32:08.000000 parkapi_sources-0.4.1/tests/converters/ulm_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-05-16 11:32:08.000000 parkapi_sources-0.4.1/tests/converters/vrs_p_r_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:32:12.632774 parkapi_sources-0.4.1/tests/models/
+-rw-r--r--   0 runner    (1001) docker     (127)     2183 2024-05-16 11:32:08.000000 parkapi_sources-0.4.1/tests/models/xlsx_inputs_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:32:12.632774 parkapi_sources-0.4.1/tests/util/
+-rw-r--r--   0 runner    (1001) docker     (127)     4105 2024-05-16 11:32:08.000000 parkapi_sources-0.4.1/tests/util/data_xml_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1706 2024-05-16 11:32:08.000000 parkapi_sources-0.4.1/tests/util/encoding_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4039 2024-05-16 11:32:08.000000 parkapi_sources-0.4.1/tests/util/xml_helper_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:32:12.636774 parkapi_sources-0.4.1/tests/validators/
+-rw-r--r--   0 runner    (1001) docker     (127)     1255 2024-05-16 11:32:08.000000 parkapi_sources-0.4.1/tests/validators/boolean_validators_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-16 11:32:08.000000 parkapi_sources-0.4.1/tests/validators/date_validators_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2108 2024-05-16 11:32:08.000000 parkapi_sources-0.4.1/tests/validators/datetime_validators_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-05-16 11:32:08.000000 parkapi_sources-0.4.1/tests/validators/integer_validators_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-05-16 11:32:08.000000 parkapi_sources-0.4.1/tests/validators/noneable_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-05-16 11:32:08.000000 parkapi_sources-0.4.1/tests/validators/string_validators_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      567 2024-05-16 11:32:08.000000 parkapi_sources-0.4.1/tests/validators/time_validators_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-16 11:32:08.000000 parkapi_sources-0.4.1/tox.ini
```

### Comparing `parkapi_sources-0.4.0/.github/workflows/build-publish.yml` & `parkapi_sources-0.4.1/.github/workflows/build-publish.yml`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.4.0/.github/workflows/lint-test.yml` & `parkapi_sources-0.4.1/.github/workflows/lint-test.yml`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.4.0/CHANGELOG.md` & `parkapi_sources-0.4.1/CHANGELOG.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,20 @@
 # Changelog
 
+## 0.4.1
+
+Released 2024-05-16
+
+### Fixes:
+
+* Fixes purpose to BIKE at Konstanz, Karlsruhe and RadVIS bike converters
+* Fixes Karlsruhe bike converter uid
+* Fixes Karlsruhe converter because data source changed date format
+
+
 ## 0.4.0
 
 Released 2024-05-16
 
 ### Features
 
 * Converter: [Konstanz Bike](https://github.com/ParkenDD/parkapi-sources-v3/pull/36), including some enumeration enhancements
```

### Comparing `parkapi_sources-0.4.0/LICENCE.txt` & `parkapi_sources-0.4.1/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.4.0/PKG-INFO` & `parkapi_sources-0.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: parkapi_sources
-Version: 0.4.0
+Version: 0.4.1
 Summary: ParkAPI Sources is a collection of converters from several different data sources to normalized ParkAPI data.
 Author-email: "Ernesto Ruge, binary butterfly GmbH" <ernesto.ruge@binary-butterfly.de>
 Maintainer-email: "Ernesto Ruge, binary butterfly GmbH" <ernesto.ruge@binary-butterfly.de>
 Keywords: data,parking,converter,mobility,car,bike
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `parkapi_sources-0.4.0/README.md` & `parkapi_sources-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.4.0/data/freiburg.geojson` & `parkapi_sources-0.4.1/data/freiburg.geojson`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.4.0/data/heidelberg.geojson` & `parkapi_sources-0.4.1/data/heidelberg.geojson`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.4.0/data/mannheim.geojson` & `parkapi_sources-0.4.1/data/mannheim.geojson`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.4.0/data/ulm.geojson` & `parkapi_sources-0.4.1/data/ulm.geojson`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.4.0/dev/test-pull-converter.py` & `parkapi_sources-0.4.1/dev/test-pull-converter.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.4.0/dev/test-push-converter.py` & `parkapi_sources-0.4.1/dev/test-push-converter.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.4.0/pyproject.toml` & `parkapi_sources-0.4.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.4.0/src/parkapi_sources/converters/__init__.py` & `parkapi_sources-0.4.1/src/parkapi_sources/converters/__init__.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.4.0/src/parkapi_sources/converters/bahn_v2/converter.py` & `parkapi_sources-0.4.1/src/parkapi_sources/converters/bahn_v2/converter.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.4.0/src/parkapi_sources/converters/bahn_v2/mapper.py` & `parkapi_sources-0.4.1/src/parkapi_sources/converters/bahn_v2/mapper.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.4.0/src/parkapi_sources/converters/bahn_v2/validators.py` & `parkapi_sources-0.4.1/src/parkapi_sources/converters/bahn_v2/validators.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.4.0/src/parkapi_sources/converters/base_converter/base_converter.py` & `parkapi_sources-0.4.1/src/parkapi_sources/converters/base_converter/base_converter.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.4.0/src/parkapi_sources/converters/base_converter/pull/pull_converter.py` & `parkapi_sources-0.4.1/src/parkapi_sources/converters/base_converter/pull/pull_converter.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.4.0/src/parkapi_sources/converters/base_converter/pull/pull_scraper_mixin.py` & `parkapi_sources-0.4.1/src/parkapi_sources/converters/base_converter/pull/pull_scraper_mixin.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.4.0/src/parkapi_sources/converters/base_converter/pull/static_geojson_data_mixin/mixin.py` & `parkapi_sources-0.4.1/src/parkapi_sources/converters/base_converter/pull/static_geojson_data_mixin/mixin.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.4.0/src/parkapi_sources/converters/base_converter/pull/static_geojson_data_mixin/models.py` & `parkapi_sources-0.4.1/src/parkapi_sources/converters/base_converter/pull/static_geojson_data_mixin/models.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.4.0/src/parkapi_sources/converters/base_converter/push/csv_converter.py` & `parkapi_sources-0.4.1/src/parkapi_sources/converters/base_converter/push/csv_converter.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.4.0/src/parkapi_sources/converters/base_converter/push/json_converter.py` & `parkapi_sources-0.4.1/src/parkapi_sources/converters/base_converter/push/json_converter.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.4.0/src/parkapi_sources/converters/base_converter/push/normalized_xlsx_converter.py` & `parkapi_sources-0.4.1/src/parkapi_sources/converters/base_converter/push/normalized_xlsx_converter.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.4.0/src/parkapi_sources/converters/base_converter/push/parkapi_json_converter.py` & `parkapi_sources-0.4.1/src/parkapi_sources/converters/base_converter/push/parkapi_json_converter.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.4.0/src/parkapi_sources/converters/base_converter/push/xlsx_converter.py` & `parkapi_sources-0.4.1/src/parkapi_sources/converters/base_converter/push/xlsx_converter.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.4.0/src/parkapi_sources/converters/base_converter/push/xml_converter.py` & `parkapi_sources-0.4.1/src/parkapi_sources/converters/base_converter/push/xml_converter.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.4.0/src/parkapi_sources/converters/bfrk_bw/base_converter.py` & `parkapi_sources-0.4.1/src/parkapi_sources/converters/bfrk_bw/base_converter.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.4.0/src/parkapi_sources/converters/bfrk_bw/base_models.py` & `parkapi_sources-0.4.1/src/parkapi_sources/converters/bfrk_bw/base_models.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.4.0/src/parkapi_sources/converters/bfrk_bw/bike_converter.py` & `parkapi_sources-0.4.1/src/parkapi_sources/converters/bfrk_bw/bike_converter.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.4.0/src/parkapi_sources/converters/bfrk_bw/bike_models.py` & `parkapi_sources-0.4.1/src/parkapi_sources/converters/bfrk_bw/bike_models.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.4.0/src/parkapi_sources/converters/bfrk_bw/car_converter.py` & `parkapi_sources-0.4.1/src/parkapi_sources/converters/bfrk_bw/car_converter.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.4.0/src/parkapi_sources/converters/bfrk_bw/car_models.py` & `parkapi_sources-0.4.1/src/parkapi_sources/converters/bfrk_bw/car_models.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.4.0/src/parkapi_sources/converters/ellwangen/converter.py` & `parkapi_sources-0.4.1/src/parkapi_sources/converters/ellwangen/converter.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.4.0/src/parkapi_sources/converters/freiburg/converter.py` & `parkapi_sources-0.4.1/src/parkapi_sources/converters/freiburg/converter.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.4.0/src/parkapi_sources/converters/freiburg/models.py` & `parkapi_sources-0.4.1/src/parkapi_sources/converters/freiburg/models.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.4.0/src/parkapi_sources/converters/heidelberg/converter.py` & `parkapi_sources-0.4.1/src/parkapi_sources/converters/heidelberg/converter.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.4.0/src/parkapi_sources/converters/heidelberg/validators.py` & `parkapi_sources-0.4.1/src/parkapi_sources/converters/heidelberg/validators.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.4.0/src/parkapi_sources/converters/karlsruhe/converter.py` & `parkapi_sources-0.4.1/src/parkapi_sources/converters/karlsruhe/converter.py`

 * *Files 0% similar despite different names*

```diff
@@ -95,15 +95,15 @@
         return realtime_parking_site_inputs, import_parking_site_exceptions
 
 
 class KarlsruheBikePullConverter(KarlsruheBasePullConverter):
     karlsruhe_feature_validator = DataclassValidator(KarlsruheBikeFeatureInput)
 
     source_info = SourceInfo(
-        uid='karlsruhe',
+        uid='karlsruhe_bike',
         name='Stadt Karlsruhe: Fahrrad-Abstellanlagen',
         public_url='https://web1.karlsruhe.de/service/Parken/',
         source_url='https://mobil.trk.de:8443/geoserver/TBA/ows?service=WFS&version=1.0.0&request=GetFeature'
         '&typeName=TBA%3Aka_fahrradanlagen&outputFormat=application%2Fjson',
         timezone='Europe/Berlin',
         attribution_contributor='Stadt Karlsruhe',
         attribution_license='Creative Commons Namensnennung - 4.0 International (CC-BY 4.0)',
```

### Comparing `parkapi_sources-0.4.0/src/parkapi_sources/converters/karlsruhe/files/ca.crt.pem` & `parkapi_sources-0.4.1/src/parkapi_sources/converters/karlsruhe/files/ca.crt.pem`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.4.0/src/parkapi_sources/converters/karlsruhe/models.py` & `parkapi_sources-0.4.1/src/parkapi_sources/converters/karlsruhe/models.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     NumericValidator,
     StringValidator,
     UrlValidator,
 )
 
 from parkapi_sources.converters.base_converter.pull import GeojsonFeatureGeometryInput
 from parkapi_sources.models import RealtimeParkingSiteInput, StaticParkingSiteInput
-from parkapi_sources.models.enums import OpeningStatus, ParkingSiteType
+from parkapi_sources.models.enums import OpeningStatus, ParkingSiteType, PurposeType
 from parkapi_sources.validators import ParsedDateValidator
 
 
 class KarlsruheOpeningStatus(Enum):
     OPEN = 'Geöffnet'
     CLOSED = 'Geschlossen'
 
@@ -56,15 +56,15 @@
     bemerkung: Optional[str] = Noneable(StringValidator())
     parkhaus_internet: Optional[str] = Noneable(UrlValidator())
     parkhaus_telefon: Optional[str] = Noneable(StringValidator())
     parkhaus_email: Optional[str] = Noneable(EmailValidator())
     betreiber_internet: Optional[str] = Noneable(UrlValidator())
     betreiber_email: Optional[str] = Noneable(EmailValidator())
     betreiber_telefon: Optional[str] = Noneable(StringValidator())
-    stand_parkhausdaten: date = ParsedDateValidator(date_format='%d.%m.%Y')
+    stand_parkhausdaten: date = ParsedDateValidator(date_format='%Y-%m-%dZ')
 
     def __post_init__(self):
         if self.max_durchfahrtshoehe == 0:  # 0 is used as None
             self.max_durchfahrtshoehe = None
 
 
 @validataclass
@@ -150,8 +150,9 @@
             capacity=self.properties.stellplaetze,
             address=address,
             public_url=self.properties.link,
             is_covered=self.properties.art == KarlsruheBikeType.STANDS_WITH_ROOF or UnsetValue,
             description=self.properties.bemerkung,
             static_data_updated_at=datetime.now(timezone.utc),
             type=self.properties.art.to_parking_site_type(),
+            purpose=PurposeType.BIKE,
         )
```

### Comparing `parkapi_sources-0.4.0/src/parkapi_sources/converters/kienzler/converter.py` & `parkapi_sources-0.4.1/src/parkapi_sources/converters/kienzler/converter.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.4.0/src/parkapi_sources/converters/kienzler/models.py` & `parkapi_sources-0.4.1/src/parkapi_sources/converters/kienzler/models.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.4.0/src/parkapi_sources/converters/konstanz_bike/converter.py` & `parkapi_sources-0.4.1/src/parkapi_sources/converters/konstanz_bike/converter.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.4.0/src/parkapi_sources/converters/konstanz_bike/models.py` & `parkapi_sources-0.4.1/src/parkapi_sources/converters/konstanz_bike/models.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from typing import Any, Optional
 
 from validataclass.dataclasses import validataclass
 from validataclass.exceptions import ValidationError
 from validataclass.validators import EnumValidator, IntegerValidator, StringValidator
 
 from parkapi_sources.models import StaticParkingSiteInput
-from parkapi_sources.models.enums import ParkingSiteType
+from parkapi_sources.models.enums import ParkingSiteType, PurposeType
 from parkapi_sources.validators import ExcelNoneable
 from parkapi_sources.validators.boolean_validators import MappedBooleanValidator
 
 
 @validataclass
 class PolygonListValidator(StringValidator):
     def validate(self, input_data: Any, **kwargs) -> list[tuple[Decimal, Decimal]]:
@@ -76,8 +76,9 @@
             lon=sum([coordinate[0] for coordinate in self.coordinates]) / len(self.coordinates),
             type=self.type.to_parking_site_type_input(),
             address=f'{self.address}, Konstanz',
             capacity=self.capacity,
             has_lighting=self.has_lighting,
             is_covered=self.is_covered,
             static_data_updated_at=datetime.now(tz=timezone.utc),
+            purpose=PurposeType.BIKE,
         )
```

### Comparing `parkapi_sources-0.4.0/src/parkapi_sources/converters/mannheim_buchen/converter.py` & `parkapi_sources-0.4.1/src/parkapi_sources/converters/mannheim_buchen/converter.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.4.0/src/parkapi_sources/converters/neckarsulm/converter.py` & `parkapi_sources-0.4.1/src/parkapi_sources/converters/neckarsulm/converter.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.4.0/src/parkapi_sources/converters/neckarsulm/models.py` & `parkapi_sources-0.4.1/src/parkapi_sources/converters/neckarsulm/models.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.4.0/src/parkapi_sources/converters/neckarsulm_bike/converter.py` & `parkapi_sources-0.4.1/src/parkapi_sources/converters/neckarsulm_bike/converter.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.4.0/src/parkapi_sources/converters/pbw/converter.py` & `parkapi_sources-0.4.1/src/parkapi_sources/converters/pbw/converter.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.4.0/src/parkapi_sources/converters/pbw/mapper.py` & `parkapi_sources-0.4.1/src/parkapi_sources/converters/pbw/mapper.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.4.0/src/parkapi_sources/converters/pbw/validation.py` & `parkapi_sources-0.4.1/src/parkapi_sources/converters/pbw/validation.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.4.0/src/parkapi_sources/converters/pforzheim/converter.py` & `parkapi_sources-0.4.1/src/parkapi_sources/converters/pforzheim/converter.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.4.0/src/parkapi_sources/converters/pforzheim/validation.py` & `parkapi_sources-0.4.1/src/parkapi_sources/converters/pforzheim/validation.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.4.0/src/parkapi_sources/converters/pum_bw/converter.py` & `parkapi_sources-0.4.1/src/parkapi_sources/converters/pum_bw/converter.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.4.0/src/parkapi_sources/converters/radvis_bw/converter.py` & `parkapi_sources-0.4.1/src/parkapi_sources/converters/radvis_bw/converter.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 import requests
 from validataclass.exceptions import ValidationError
 from validataclass.validators import DataclassValidator
 
 from parkapi_sources.converters.base_converter.pull import GeojsonInput, PullConverter
 from parkapi_sources.exceptions import ImportParkingSiteException
 from parkapi_sources.models import RealtimeParkingSiteInput, SourceInfo, StaticParkingSiteInput
+from parkapi_sources.models.enums import PurposeType
 
 from .models import RadvisFeatureInput
 
 
 class RadvisBwPullConverter(PullConverter):
     proj: pyproj.Proj = pyproj.Proj(proj='utm', zone=32, ellps='WGS84', preserve_units=True)
     _base_url = (
@@ -54,14 +55,15 @@
 
                 static_parking_site_inputs.append(
                     radvis_parking_site_input.to_static_parking_site_input_with_proj(
                         static_data_updated_at=datetime.now(tz=timezone.utc),
                         proj=self.proj,
                     ),
                 )
+                radvis_parking_site_input.purpose = PurposeType.BIKE
             except ValidationError as e:
                 static_parking_site_errors.append(
                     ImportParkingSiteException(
                         source_uid=self.source_info.uid,
                         parking_site_uid=feature_dict.get('properties', {}).get('id'),
                         message=f'validation error for data {feature_dict}: {e.to_dict()}',
                     ),
```

### Comparing `parkapi_sources-0.4.0/src/parkapi_sources/converters/radvis_bw/models.py` & `parkapi_sources-0.4.1/src/parkapi_sources/converters/radvis_bw/models.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.4.0/src/parkapi_sources/converters/reutlingen/converter.py` & `parkapi_sources-0.4.1/src/parkapi_sources/converters/reutlingen/converter.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.4.0/src/parkapi_sources/converters/reutlingen/validation.py` & `parkapi_sources-0.4.1/src/parkapi_sources/converters/reutlingen/validation.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.4.0/src/parkapi_sources/converters/reutlingen_bike/converter.py` & `parkapi_sources-0.4.1/src/parkapi_sources/converters/reutlingen_bike/converter.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.4.0/src/parkapi_sources/converters/reutlingen_bike/validation.py` & `parkapi_sources-0.4.1/src/parkapi_sources/converters/reutlingen_bike/validation.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.4.0/src/parkapi_sources/converters/stuttgart/converter.py` & `parkapi_sources-0.4.1/src/parkapi_sources/converters/stuttgart/converter.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.4.0/src/parkapi_sources/converters/ulm/converter.py` & `parkapi_sources-0.4.1/src/parkapi_sources/converters/ulm/converter.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.4.0/src/parkapi_sources/converters/vrs_p_r/vrs_p_r.py` & `parkapi_sources-0.4.1/src/parkapi_sources/converters/vrs_p_r/vrs_p_r.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.4.0/src/parkapi_sources/exceptions.py` & `parkapi_sources-0.4.1/src/parkapi_sources/exceptions.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.4.0/src/parkapi_sources/models/enums.py` & `parkapi_sources-0.4.1/src/parkapi_sources/models/enums.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.4.0/src/parkapi_sources/models/parking_site_inputs.py` & `parkapi_sources-0.4.1/src/parkapi_sources/models/parking_site_inputs.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,15 +56,14 @@
     park_and_ride_type: OptionalUnsetNone[list[ParkAndRideType]] = (
         Noneable(
             ListValidator(EnumValidator(ParkAndRideType)),
         ),
         DefaultUnset,
     )
     supervision_type: OptionalUnsetNone[SupervisionType] = Noneable(EnumValidator(SupervisionType)), DefaultUnset
-    is_covered: OptionalUnsetNone[bool] = Noneable(BooleanValidator()), DefaultUnset
     photo_url: OptionalUnsetNone[str] = Noneable(UrlValidator(max_length=4096)), DefaultUnset
     related_location: OptionalUnsetNone[str] = Noneable(StringValidator(max_length=256)), DefaultUnset
 
     has_realtime_data: OptionalUnsetNone[bool] = Noneable(BooleanValidator(), default=False), DefaultUnset
     static_data_updated_at: OptionalUnsetNone[datetime] = (
         DateTimeValidator(
             local_timezone=timezone.utc,
```

### Comparing `parkapi_sources-0.4.0/src/parkapi_sources/models/source_info.py` & `parkapi_sources-0.4.1/src/parkapi_sources/models/source_info.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.4.0/src/parkapi_sources/models/xlsx_inputs.py` & `parkapi_sources-0.4.1/src/parkapi_sources/models/xlsx_inputs.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.4.0/src/parkapi_sources/parkapi_sources.py` & `parkapi_sources-0.4.1/src/parkapi_sources/parkapi_sources.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.4.0/src/parkapi_sources/scripts/parkapi.py` & `parkapi_sources-0.4.1/src/parkapi_sources/scripts/parkapi.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.4.0/src/parkapi_sources/util/encoding.py` & `parkapi_sources-0.4.1/src/parkapi_sources/util/encoding.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.4.0/src/parkapi_sources/util/xml_helper.py` & `parkapi_sources-0.4.1/src/parkapi_sources/util/xml_helper.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.4.0/src/parkapi_sources/validators/__init__.py` & `parkapi_sources-0.4.1/src/parkapi_sources/validators/__init__.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.4.0/src/parkapi_sources/validators/boolean_validators.py` & `parkapi_sources-0.4.1/src/parkapi_sources/validators/boolean_validators.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.4.0/src/parkapi_sources/validators/date_validator.py` & `parkapi_sources-0.4.1/src/parkapi_sources/validators/date_validator.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.4.0/src/parkapi_sources/validators/datetime_validator.py` & `parkapi_sources-0.4.1/src/parkapi_sources/validators/datetime_validator.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.4.0/src/parkapi_sources/validators/integer_validators.py` & `parkapi_sources-0.4.1/src/parkapi_sources/validators/integer_validators.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.4.0/src/parkapi_sources/validators/list_validator.py` & `parkapi_sources-0.4.1/src/parkapi_sources/validators/list_validator.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.4.0/src/parkapi_sources/validators/noneable.py` & `parkapi_sources-0.4.1/src/parkapi_sources/validators/noneable.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.4.0/src/parkapi_sources/validators/string_validators.py` & `parkapi_sources-0.4.1/src/parkapi_sources/validators/string_validators.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.4.0/src/parkapi_sources.egg-info/PKG-INFO` & `parkapi_sources-0.4.1/src/parkapi_sources.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: parkapi_sources
-Version: 0.4.0
+Version: 0.4.1
 Summary: ParkAPI Sources is a collection of converters from several different data sources to normalized ParkAPI data.
 Author-email: "Ernesto Ruge, binary butterfly GmbH" <ernesto.ruge@binary-butterfly.de>
 Maintainer-email: "Ernesto Ruge, binary butterfly GmbH" <ernesto.ruge@binary-butterfly.de>
 Keywords: data,parking,converter,mobility,car,bike
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `parkapi_sources-0.4.0/src/parkapi_sources.egg-info/SOURCES.txt` & `parkapi_sources-0.4.1/src/parkapi_sources.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.4.0/tests/converters/bahn_v2_test.py` & `parkapi_sources-0.4.1/tests/converters/bahn_v2_test.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.4.0/tests/converters/bfrk_bw_test.py` & `parkapi_sources-0.4.1/tests/converters/bfrk_bw_test.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.4.0/tests/converters/conftest.py` & `parkapi_sources-0.4.1/tests/converters/conftest.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.4.0/tests/converters/data/bahn_v2.json` & `parkapi_sources-0.4.1/tests/converters/data/bahn_v2.json`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.4.0/tests/converters/data/bfrk_bw_bike.csv` & `parkapi_sources-0.4.1/tests/converters/data/bfrk_bw_bike.csv`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.4.0/tests/converters/data/bfrk_bw_car.csv` & `parkapi_sources-0.4.1/tests/converters/data/bfrk_bw_car.csv`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.4.0/tests/converters/data/ellwangen.xlsx` & `parkapi_sources-0.4.1/tests/converters/data/ellwangen.xlsx`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.4.0/tests/converters/data/freiburg.json` & `parkapi_sources-0.4.1/tests/converters/data/freiburg.json`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.4.0/tests/converters/data/heidelberg.json` & `parkapi_sources-0.4.1/tests/converters/data/heidelberg.json`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.4.0/tests/converters/data/karlsruhe_bike.json` & `parkapi_sources-0.4.1/tests/converters/data/karlsruhe_bike.json`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.4.0/tests/converters/data/kienzler.json` & `parkapi_sources-0.4.1/tests/converters/data/kienzler.json`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.4.0/tests/converters/data/konstanz_bike.csv` & `parkapi_sources-0.4.1/tests/converters/data/konstanz_bike.csv`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.4.0/tests/converters/data/mannheim.json` & `parkapi_sources-0.4.1/tests/converters/data/mannheim.json`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.4.0/tests/converters/data/neckarsulm.csv` & `parkapi_sources-0.4.1/tests/converters/data/neckarsulm.csv`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.4.0/tests/converters/data/neckarsulm_bike.csv` & `parkapi_sources-0.4.1/tests/converters/data/neckarsulm_bike.csv`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.4.0/tests/converters/data/pbw/catalog-city.json` & `parkapi_sources-0.4.1/tests/converters/data/pbw/catalog-city.json`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.4.0/tests/converters/data/pbw/object-by-city-10.json` & `parkapi_sources-0.4.1/tests/converters/data/pbw/object-by-city-10.json`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.4.0/tests/converters/data/pbw/object-by-city-11.json` & `parkapi_sources-0.4.1/tests/converters/data/pbw/object-by-city-11.json`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.4.0/tests/converters/data/pbw/object-by-city-12.json` & `parkapi_sources-0.4.1/tests/converters/data/pbw/object-by-city-12.json`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.4.0/tests/converters/data/pbw/object-by-city-15.json` & `parkapi_sources-0.4.1/tests/converters/data/pbw/object-by-city-15.json`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.4.0/tests/converters/data/pbw/object-by-city-17.json` & `parkapi_sources-0.4.1/tests/converters/data/pbw/object-by-city-17.json`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.4.0/tests/converters/data/pbw/object-by-city-18.json` & `parkapi_sources-0.4.1/tests/converters/data/pbw/object-by-city-18.json`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.4.0/tests/converters/data/pbw/object-by-city-19.json` & `parkapi_sources-0.4.1/tests/converters/data/pbw/object-by-city-19.json`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.4.0/tests/converters/data/pbw/object-by-city-31.json` & `parkapi_sources-0.4.1/tests/converters/data/pbw/object-by-city-31.json`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.4.0/tests/converters/data/pbw/object-by-city-32.json` & `parkapi_sources-0.4.1/tests/converters/data/pbw/object-by-city-32.json`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.4.0/tests/converters/data/pbw/object-by-city-33.json` & `parkapi_sources-0.4.1/tests/converters/data/pbw/object-by-city-33.json`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.4.0/tests/converters/data/pbw/object-by-city-34.json` & `parkapi_sources-0.4.1/tests/converters/data/pbw/object-by-city-34.json`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.4.0/tests/converters/data/pbw/object-by-city-4.json` & `parkapi_sources-0.4.1/tests/converters/data/pbw/object-by-city-4.json`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.4.0/tests/converters/data/pbw/object-by-city-42.json` & `parkapi_sources-0.4.1/tests/converters/data/pbw/object-by-city-42.json`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.4.0/tests/converters/data/pbw/object-by-city-48.json` & `parkapi_sources-0.4.1/tests/converters/data/pbw/object-by-city-48.json`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.4.0/tests/converters/data/pbw/object-by-city-49.json` & `parkapi_sources-0.4.1/tests/converters/data/pbw/object-by-city-49.json`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.4.0/tests/converters/data/pbw/object-by-city-51.json` & `parkapi_sources-0.4.1/tests/converters/data/pbw/object-by-city-51.json`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.4.0/tests/converters/data/pbw/object-by-city-52.json` & `parkapi_sources-0.4.1/tests/converters/data/pbw/object-by-city-52.json`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.4.0/tests/converters/data/pbw/object-by-city-60.json` & `parkapi_sources-0.4.1/tests/converters/data/pbw/object-by-city-60.json`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.4.0/tests/converters/data/pbw/object-by-city-61.json` & `parkapi_sources-0.4.1/tests/converters/data/pbw/object-by-city-61.json`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.4.0/tests/converters/data/pbw/object-by-city-7.json` & `parkapi_sources-0.4.1/tests/converters/data/pbw/object-by-city-7.json`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.4.0/tests/converters/data/pbw/object-by-city-71.json` & `parkapi_sources-0.4.1/tests/converters/data/pbw/object-by-city-71.json`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.4.0/tests/converters/data/pbw/object-by-city-9.json` & `parkapi_sources-0.4.1/tests/converters/data/pbw/object-by-city-9.json`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.4.0/tests/converters/data/pbw/object-dynamic-all.json` & `parkapi_sources-0.4.1/tests/converters/data/pbw/object-dynamic-all.json`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.4.0/tests/converters/data/pforzheim.json` & `parkapi_sources-0.4.1/tests/converters/data/pforzheim.json`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.4.0/tests/converters/data/pum_bw.xlsx` & `parkapi_sources-0.4.1/tests/converters/data/pum_bw.xlsx`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.4.0/tests/converters/data/radvis_bw.json` & `parkapi_sources-0.4.1/tests/converters/data/radvis_bw.json`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.4.0/tests/converters/data/reutlingen.csv` & `parkapi_sources-0.4.1/tests/converters/data/reutlingen.csv`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.4.0/tests/converters/data/reutlingen_bike.csv` & `parkapi_sources-0.4.1/tests/converters/data/reutlingen_bike.csv`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.4.0/tests/converters/data/stuttgart-realtime.xml` & `parkapi_sources-0.4.1/tests/converters/data/stuttgart-realtime.xml`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.4.0/tests/converters/data/stuttgart-static.xml` & `parkapi_sources-0.4.1/tests/converters/data/stuttgart-static.xml`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.4.0/tests/converters/data/ulm.html` & `parkapi_sources-0.4.1/tests/converters/data/ulm.html`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.4.0/tests/converters/data/vrs_p_r.xlsx` & `parkapi_sources-0.4.1/tests/converters/data/vrs_p_r.xlsx`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.4.0/tests/converters/ellwangen_test.py` & `parkapi_sources-0.4.1/tests/converters/ellwangen_test.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.4.0/tests/converters/freiburg_test.py` & `parkapi_sources-0.4.1/tests/converters/freiburg_test.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.4.0/tests/converters/heidelberg_test.py` & `parkapi_sources-0.4.1/tests/converters/heidelberg_test.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.4.0/tests/converters/helper.py` & `parkapi_sources-0.4.1/tests/converters/helper.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.4.0/tests/converters/karlsruhe_bike_test.py` & `parkapi_sources-0.4.1/tests/converters/karlsruhe_bike_test.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.4.0/tests/converters/karlsruhe_test.py` & `parkapi_sources-0.4.1/tests/converters/karlsruhe_test.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.4.0/tests/converters/kienzler_test.py` & `parkapi_sources-0.4.1/tests/converters/kienzler_test.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.4.0/tests/converters/konstanz_bike_test.py` & `parkapi_sources-0.4.1/tests/converters/konstanz_bike_test.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.4.0/tests/converters/mannheim_buchen_test.py` & `parkapi_sources-0.4.1/tests/converters/mannheim_buchen_test.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.4.0/tests/converters/neckarsulm_bike_test.py` & `parkapi_sources-0.4.1/tests/converters/neckarsulm_bike_test.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.4.0/tests/converters/neckarsulm_test.py` & `parkapi_sources-0.4.1/tests/converters/neckarsulm_test.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.4.0/tests/converters/pbw_test.py` & `parkapi_sources-0.4.1/tests/converters/pbw_test.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.4.0/tests/converters/pforzheim_test.py` & `parkapi_sources-0.4.1/tests/converters/pforzheim_test.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.4.0/tests/converters/pum_bw_test.py` & `parkapi_sources-0.4.1/tests/converters/pum_bw_test.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.4.0/tests/converters/radvis_bw_test.py` & `parkapi_sources-0.4.1/tests/converters/radvis_bw_test.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.4.0/tests/converters/reutlingen_bike_test.py` & `parkapi_sources-0.4.1/tests/converters/reutlingen_bike_test.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.4.0/tests/converters/reutlingen_test.py` & `parkapi_sources-0.4.1/tests/converters/reutlingen_test.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.4.0/tests/converters/stuttgart_test.py` & `parkapi_sources-0.4.1/tests/converters/stuttgart_test.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.4.0/tests/converters/ulm_test.py` & `parkapi_sources-0.4.1/tests/converters/ulm_test.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.4.0/tests/converters/vrs_p_r_test.py` & `parkapi_sources-0.4.1/tests/converters/vrs_p_r_test.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.4.0/tests/models/xlsx_inputs_test.py` & `parkapi_sources-0.4.1/tests/models/xlsx_inputs_test.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.4.0/tests/util/data_xml_helper.py` & `parkapi_sources-0.4.1/tests/util/data_xml_helper.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.4.0/tests/util/encoding_test.py` & `parkapi_sources-0.4.1/tests/util/encoding_test.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.4.0/tests/util/xml_helper_test.py` & `parkapi_sources-0.4.1/tests/util/xml_helper_test.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.4.0/tests/validators/boolean_validators_test.py` & `parkapi_sources-0.4.1/tests/validators/boolean_validators_test.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.4.0/tests/validators/date_validators_test.py` & `parkapi_sources-0.4.1/tests/validators/date_validators_test.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.4.0/tests/validators/datetime_validators_test.py` & `parkapi_sources-0.4.1/tests/validators/datetime_validators_test.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.4.0/tests/validators/integer_validators_test.py` & `parkapi_sources-0.4.1/tests/validators/integer_validators_test.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.4.0/tests/validators/noneable_tests.py` & `parkapi_sources-0.4.1/tests/validators/noneable_tests.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.4.0/tests/validators/string_validators_test.py` & `parkapi_sources-0.4.1/tests/validators/string_validators_test.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.4.0/tests/validators/time_validators_test.py` & `parkapi_sources-0.4.1/tests/validators/time_validators_test.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.4.0/tox.ini` & `parkapi_sources-0.4.1/tox.ini`

 * *Files identical despite different names*

