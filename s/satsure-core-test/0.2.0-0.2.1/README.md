# Comparing `tmp/satsure_core_test-0.2.0.tar.gz` & `tmp/satsure-core-test-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "satsure_core_test-0.2.0.tar", last modified: Wed May 15 16:11:12 2024, max compression
+gzip compressed data, was "satsure-core-test-0.2.1.tar", last modified: Thu May 16 05:32:43 2024, max compression
```

## Comparing `satsure_core_test-0.2.0.tar` & `satsure-core-test-0.2.1.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-15 16:11:12.816816 satsure_core_test-0.2.0/
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-04-25 07:48:02.000000 satsure_core_test-0.2.0/LICENCE.txt
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      510 2024-05-15 16:11:12.816576 satsure_core_test-0.2.0/PKG-INFO
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-04-25 07:48:18.000000 satsure_core_test-0.2.0/README.md
-drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-15 16:11:12.807892 satsure_core_test-0.2.0/satelite/
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-06 07:15:52.000000 satsure_core_test-0.2.0/satelite/__init__.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      976 2024-05-14 12:00:39.000000 satsure_core_test-0.2.0/satelite/config.py
-drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-15 16:11:12.808537 satsure_core_test-0.2.0/satelite/core/
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-13 07:33:26.000000 satsure_core_test-0.2.0/satelite/core/__init__.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     4955 2024-05-15 15:15:22.000000 satsure_core_test-0.2.0/satelite/core/downloader.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      733 2024-05-15 14:34:53.000000 satsure_core_test-0.2.0/satelite/core/uploader.py
-drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-15 16:11:12.808917 satsure_core_test-0.2.0/satelite/gdal/
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-13 07:33:26.000000 satsure_core_test-0.2.0/satelite/gdal/__init__.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     2511 2024-05-14 15:24:54.000000 satsure_core_test-0.2.0/satelite/gdal/gdal_commands.py
-drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-15 16:11:12.809245 satsure_core_test-0.2.0/satelite/models/
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-13 07:33:26.000000 satsure_core_test-0.2.0/satelite/models/__init__.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      372 2024-05-13 07:33:26.000000 satsure_core_test-0.2.0/satelite/models/s2_enum.py
-drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-15 16:11:12.809553 satsure_core_test-0.2.0/satelite/raster/
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-13 07:33:26.000000 satsure_core_test-0.2.0/satelite/raster/__init__.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     8913 2024-05-13 07:51:34.000000 satsure_core_test-0.2.0/satelite/raster/raster.py
-drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-15 16:11:12.811916 satsure_core_test-0.2.0/satelite/sentinel2/
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      499 2024-05-15 14:34:51.000000 satsure_core_test-0.2.0/satelite/sentinel2/__init__.py
-drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-15 16:11:12.812259 satsure_core_test-0.2.0/satelite/sentinel2/band_stack/
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-13 07:33:26.000000 satsure_core_test-0.2.0/satelite/sentinel2/band_stack/__init__.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     2834 2024-05-15 12:28:03.000000 satsure_core_test-0.2.0/satelite/sentinel2/band_stack/generate_band_stack.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     2429 2024-05-13 07:33:26.000000 satsure_core_test-0.2.0/satelite/sentinel2/fetch_unique_tile_date.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1634 2024-05-06 07:15:52.000000 satsure_core_test-0.2.0/satelite/sentinel2/fetch_unique_tile_date_pystac.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     3204 2024-05-14 12:04:20.000000 satsure_core_test-0.2.0/satelite/sentinel2/get_tiles.py
-drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-15 16:11:12.812566 satsure_core_test-0.2.0/satelite/sentinel2/indices/
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-13 07:33:26.000000 satsure_core_test-0.2.0/satelite/sentinel2/indices/__init__.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     3975 2024-05-15 12:01:41.000000 satsure_core_test-0.2.0/satelite/sentinel2/indices/general_indices.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      835 2024-05-15 14:22:44.000000 satsure_core_test-0.2.0/satelite/sentinel2/mosaic_custom_bands.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     2362 2024-05-15 14:15:25.000000 satsure_core_test-0.2.0/satelite/sentinel2/mosaic_same_bands.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1502 2024-05-13 07:51:34.000000 satsure_core_test-0.2.0/satelite/sentinel2/path_row_from_shp.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     3250 2024-05-13 07:33:26.000000 satsure_core_test-0.2.0/satelite/sentinel2/s2_l1c_urls.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     2912 2024-05-13 07:33:26.000000 satsure_core_test-0.2.0/satelite/sentinel2/s2_l2a_urls.py
-drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-15 16:11:12.812863 satsure_core_test-0.2.0/satelite/tests/
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-11 07:35:59.000000 satsure_core_test-0.2.0/satelite/tests/__init__.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1004 2024-05-14 12:00:39.000000 satsure_core_test-0.2.0/satelite/tests/conftest.py
-drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-15 16:11:12.815326 satsure_core_test-0.2.0/satelite/tests/sentinel2/
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-11 07:35:59.000000 satsure_core_test-0.2.0/satelite/tests/sentinel2/__init__.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      384 2024-05-13 07:58:31.000000 satsure_core_test-0.2.0/satelite/tests/sentinel2/test_fetch_unique_tile_date.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      430 2024-05-06 07:34:13.000000 satsure_core_test-0.2.0/satelite/tests/sentinel2/test_fetch_unique_tile_date_pystac.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1176 2024-05-15 12:53:42.000000 satsure_core_test-0.2.0/satelite/tests/sentinel2/test_genarate_band_stack.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1305 2024-05-15 12:55:00.000000 satsure_core_test-0.2.0/satelite/tests/sentinel2/test_general_indices.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1326 2024-05-14 12:00:39.000000 satsure_core_test-0.2.0/satelite/tests/sentinel2/test_get_tile.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      322 2024-05-13 07:33:26.000000 satsure_core_test-0.2.0/satelite/tests/sentinel2/test_mosaic_same_bands.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      871 2024-05-13 07:33:26.000000 satsure_core_test-0.2.0/satelite/tests/sentinel2/test_s2_l1c_urls.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      898 2024-05-13 07:33:26.000000 satsure_core_test-0.2.0/satelite/tests/sentinel2/test_s2_l2a_urls.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1543 2024-05-13 07:33:26.000000 satsure_core_test-0.2.0/satelite/tests/sentinel2/test_validate.py
-drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-15 16:11:12.815546 satsure_core_test-0.2.0/satelite/validators/
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-13 07:51:34.000000 satsure_core_test-0.2.0/satelite/validators/__init__.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     2381 2024-05-13 07:51:34.000000 satsure_core_test-0.2.0/satelite/validators/check_shape_of_rid.py
-drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-15 16:11:12.816353 satsure_core_test-0.2.0/satsure_core_test.egg-info/
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      510 2024-05-15 16:11:12.000000 satsure_core_test-0.2.0/satsure_core_test.egg-info/PKG-INFO
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1661 2024-05-15 16:11:12.000000 satsure_core_test-0.2.0/satsure_core_test.egg-info/SOURCES.txt
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)        1 2024-05-15 16:11:12.000000 satsure_core_test-0.2.0/satsure_core_test.egg-info/dependency_links.txt
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      136 2024-05-15 16:11:12.000000 satsure_core_test-0.2.0/satsure_core_test.egg-info/requires.txt
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)        9 2024-05-15 16:11:12.000000 satsure_core_test-0.2.0/satsure_core_test.egg-info/top_level.txt
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)       38 2024-05-15 16:11:12.816856 satsure_core_test-0.2.0/setup.cfg
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      521 2024-05-15 16:11:08.000000 satsure_core_test-0.2.0/setup.py
+drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-16 05:32:43.644914 satsure-core-test-0.2.1/
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-04-25 07:48:02.000000 satsure-core-test-0.2.1/LICENCE.txt
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      515 2024-05-16 05:32:43.644672 satsure-core-test-0.2.1/PKG-INFO
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-04-25 07:48:18.000000 satsure-core-test-0.2.1/README.md
+drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-16 05:32:43.634975 satsure-core-test-0.2.1/satelite/
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-06 07:15:52.000000 satsure-core-test-0.2.1/satelite/__init__.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      976 2024-05-14 12:00:39.000000 satsure-core-test-0.2.1/satelite/config.py
+drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-16 05:32:43.635612 satsure-core-test-0.2.1/satelite/core/
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-13 07:33:26.000000 satsure-core-test-0.2.1/satelite/core/__init__.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     4877 2024-05-16 02:50:40.000000 satsure-core-test-0.2.1/satelite/core/downloader.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      825 2024-05-16 05:29:12.000000 satsure-core-test-0.2.1/satelite/core/uploader.py
+drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-16 05:32:43.636010 satsure-core-test-0.2.1/satelite/gdal/
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-13 07:33:26.000000 satsure-core-test-0.2.1/satelite/gdal/__init__.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     2511 2024-05-14 15:24:54.000000 satsure-core-test-0.2.1/satelite/gdal/gdal_commands.py
+drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-16 05:32:43.636336 satsure-core-test-0.2.1/satelite/models/
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-13 07:33:26.000000 satsure-core-test-0.2.1/satelite/models/__init__.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      372 2024-05-13 07:33:26.000000 satsure-core-test-0.2.1/satelite/models/s2_enum.py
+drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-16 05:32:43.636655 satsure-core-test-0.2.1/satelite/raster/
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-13 07:33:26.000000 satsure-core-test-0.2.1/satelite/raster/__init__.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     8913 2024-05-13 07:51:34.000000 satsure-core-test-0.2.1/satelite/raster/raster.py
+drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-16 05:32:43.638943 satsure-core-test-0.2.1/satelite/sentinel2/
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      499 2024-05-15 14:34:51.000000 satsure-core-test-0.2.1/satelite/sentinel2/__init__.py
+drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-16 05:32:43.639218 satsure-core-test-0.2.1/satelite/sentinel2/band_stack/
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-13 07:33:26.000000 satsure-core-test-0.2.1/satelite/sentinel2/band_stack/__init__.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     2834 2024-05-15 12:28:03.000000 satsure-core-test-0.2.1/satelite/sentinel2/band_stack/generate_band_stack.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     2429 2024-05-13 07:33:26.000000 satsure-core-test-0.2.1/satelite/sentinel2/fetch_unique_tile_date.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1634 2024-05-06 07:15:52.000000 satsure-core-test-0.2.1/satelite/sentinel2/fetch_unique_tile_date_pystac.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     3204 2024-05-14 12:04:20.000000 satsure-core-test-0.2.1/satelite/sentinel2/get_tiles.py
+drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-16 05:32:43.639666 satsure-core-test-0.2.1/satelite/sentinel2/indices/
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-13 07:33:26.000000 satsure-core-test-0.2.1/satelite/sentinel2/indices/__init__.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     3975 2024-05-15 12:01:41.000000 satsure-core-test-0.2.1/satelite/sentinel2/indices/general_indices.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      835 2024-05-15 14:22:44.000000 satsure-core-test-0.2.1/satelite/sentinel2/mosaic_custom_bands.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     2362 2024-05-15 14:15:25.000000 satsure-core-test-0.2.1/satelite/sentinel2/mosaic_same_bands.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1502 2024-05-13 07:51:34.000000 satsure-core-test-0.2.1/satelite/sentinel2/path_row_from_shp.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     3250 2024-05-13 07:33:26.000000 satsure-core-test-0.2.1/satelite/sentinel2/s2_l1c_urls.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     2912 2024-05-13 07:33:26.000000 satsure-core-test-0.2.1/satelite/sentinel2/s2_l2a_urls.py
+drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-16 05:32:43.640017 satsure-core-test-0.2.1/satelite/tests/
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-11 07:35:59.000000 satsure-core-test-0.2.1/satelite/tests/__init__.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1004 2024-05-14 12:00:39.000000 satsure-core-test-0.2.1/satelite/tests/conftest.py
+drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-16 05:32:43.642917 satsure-core-test-0.2.1/satelite/tests/sentinel2/
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-11 07:35:59.000000 satsure-core-test-0.2.1/satelite/tests/sentinel2/__init__.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      384 2024-05-13 07:58:31.000000 satsure-core-test-0.2.1/satelite/tests/sentinel2/test_fetch_unique_tile_date.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      430 2024-05-06 07:34:13.000000 satsure-core-test-0.2.1/satelite/tests/sentinel2/test_fetch_unique_tile_date_pystac.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1176 2024-05-15 12:53:42.000000 satsure-core-test-0.2.1/satelite/tests/sentinel2/test_genarate_band_stack.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1318 2024-05-16 03:04:58.000000 satsure-core-test-0.2.1/satelite/tests/sentinel2/test_general_indices.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1326 2024-05-14 12:00:39.000000 satsure-core-test-0.2.1/satelite/tests/sentinel2/test_get_tile.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      322 2024-05-13 07:33:26.000000 satsure-core-test-0.2.1/satelite/tests/sentinel2/test_mosaic_same_bands.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      871 2024-05-13 07:33:26.000000 satsure-core-test-0.2.1/satelite/tests/sentinel2/test_s2_l1c_urls.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      898 2024-05-13 07:33:26.000000 satsure-core-test-0.2.1/satelite/tests/sentinel2/test_s2_l2a_urls.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1543 2024-05-13 07:33:26.000000 satsure-core-test-0.2.1/satelite/tests/sentinel2/test_validate.py
+drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-16 05:32:43.643170 satsure-core-test-0.2.1/satelite/validators/
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-13 07:51:34.000000 satsure-core-test-0.2.1/satelite/validators/__init__.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     2381 2024-05-13 07:51:34.000000 satsure-core-test-0.2.1/satelite/validators/check_shape_of_rid.py
+drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-16 05:32:43.644292 satsure-core-test-0.2.1/satsure_core_test.egg-info/
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      515 2024-05-16 05:32:43.000000 satsure-core-test-0.2.1/satsure_core_test.egg-info/PKG-INFO
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1661 2024-05-16 05:32:43.000000 satsure-core-test-0.2.1/satsure_core_test.egg-info/SOURCES.txt
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)        1 2024-05-16 05:32:43.000000 satsure-core-test-0.2.1/satsure_core_test.egg-info/dependency_links.txt
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      141 2024-05-16 05:32:43.000000 satsure-core-test-0.2.1/satsure_core_test.egg-info/requires.txt
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)        9 2024-05-16 05:32:43.000000 satsure-core-test-0.2.1/satsure_core_test.egg-info/top_level.txt
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)       38 2024-05-16 05:32:43.644955 satsure-core-test-0.2.1/setup.cfg
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      493 2024-05-16 05:32:34.000000 satsure-core-test-0.2.1/setup.py
```

### Comparing `satsure_core_test-0.2.0/satelite/config.py` & `satsure-core-test-0.2.1/satelite/config.py`

 * *Files identical despite different names*

### Comparing `satsure_core_test-0.2.0/satelite/core/downloader.py` & `satsure-core-test-0.2.1/satelite/core/downloader.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import re
 from datetime import datetime, timedelta
 from pathlib import PosixPath
 from subprocess import Popen, PIPE
 from typing import Tuple, List
 
 import requests
-from logger import logger
 from requests.adapters import HTTPAdapter
 from urllib3.util.retry import Retry
 
 
 class Downloader:
     """
        Common downloader for all request methods
@@ -103,15 +102,14 @@
         :return:
         """
 
         command = f"""aws s3 cp "s3://{bucket_name}/{prefix}" "." --recursive --request-payer --dryrun"""
         command += f""" {' '.join([f'--exclude "{exclude_}"' for exclude_ in exclude])}"""
         command += f""" {' '.join([f'--include "{include_}"' for include_ in include])}"""
 
-        logger.debug(f"AWS CLI Command: {command}")
         process = Popen(command, shell=True, stdout=PIPE)
         stdout, _ = process.communicate()
         pattern = r"(?<=download: ).+?(?= to)"
 
         return re.findall(pattern, stdout.decode("utf-8"))
 
     def list_filenames_with_date(self, bucket_name: str, prefix: str,
```

### Comparing `satsure_core_test-0.2.0/satelite/core/uploader.py` & `satsure-core-test-0.2.1/satelite/core/uploader.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 import shutil
 from pathlib import Path, PosixPath
 from subprocess import Popen, PIPE
 
 
-def upload_folder(
-        local_folder: PosixPath, bucket_name: str, prefix: str,
-        exclude: str = "*", include: str = "*", delete_local: bool = False):
-    """
-        to upload file in AWS
-    :param local_folder:
-    :param bucket_name:
-    :param prefix:
-    :param exclude:
-    :param include:
-    :param delete_local:
-    :return:
-    """
-    command = f"""aws s3 cp "{local_folder}" "s3://{bucket_name}/{prefix}" --recursive --exclude "{exclude}" --include "{include}" --request-payer"""
-    process = Popen(command, shell=True, stdout=PIPE)
-    process.communicate()
+class UpLoader:
 
-    if delete_local:
-        shutil.rmtree(Path(local_folder))
+    def upload_folder(self, local_folder: PosixPath, bucket_name: str, prefix: str,
+                      exclude: str = "*", include: str = "*", delete_local: bool = False):
+        """
+            to upload file in AWS
+        :param local_folder:
+        :param bucket_name:
+        :param prefix:
+        :param exclude:
+        :param include:
+        :param delete_local:
+        :return:
+        """
+        command = f"""aws s3 cp "{local_folder}" "s3://{bucket_name}/{prefix}" --recursive --exclude "{exclude}" --include "{include}" --request-payer"""
+        process = Popen(command, shell=True, stdout=PIPE)
+        process.communicate()
+
+        if delete_local:
+            shutil.rmtree(Path(local_folder))
```

### Comparing `satsure_core_test-0.2.0/satelite/gdal/gdal_commands.py` & `satsure-core-test-0.2.1/satelite/gdal/gdal_commands.py`

 * *Files identical despite different names*

### Comparing `satsure_core_test-0.2.0/satelite/raster/raster.py` & `satsure-core-test-0.2.1/satelite/raster/raster.py`

 * *Files identical despite different names*

### Comparing `satsure_core_test-0.2.0/satelite/sentinel2/band_stack/generate_band_stack.py` & `satsure-core-test-0.2.1/satelite/sentinel2/band_stack/generate_band_stack.py`

 * *Files identical despite different names*

### Comparing `satsure_core_test-0.2.0/satelite/sentinel2/fetch_unique_tile_date.py` & `satsure-core-test-0.2.1/satelite/sentinel2/fetch_unique_tile_date.py`

 * *Files identical despite different names*

### Comparing `satsure_core_test-0.2.0/satelite/sentinel2/fetch_unique_tile_date_pystac.py` & `satsure-core-test-0.2.1/satelite/sentinel2/fetch_unique_tile_date_pystac.py`

 * *Files identical despite different names*

### Comparing `satsure_core_test-0.2.0/satelite/sentinel2/get_tiles.py` & `satsure-core-test-0.2.1/satelite/sentinel2/get_tiles.py`

 * *Files identical despite different names*

### Comparing `satsure_core_test-0.2.0/satelite/sentinel2/indices/general_indices.py` & `satsure-core-test-0.2.1/satelite/sentinel2/indices/general_indices.py`

 * *Files identical despite different names*

### Comparing `satsure_core_test-0.2.0/satelite/sentinel2/mosaic_custom_bands.py` & `satsure-core-test-0.2.1/satelite/sentinel2/mosaic_custom_bands.py`

 * *Files identical despite different names*

### Comparing `satsure_core_test-0.2.0/satelite/sentinel2/mosaic_same_bands.py` & `satsure-core-test-0.2.1/satelite/sentinel2/mosaic_same_bands.py`

 * *Files identical despite different names*

### Comparing `satsure_core_test-0.2.0/satelite/sentinel2/path_row_from_shp.py` & `satsure-core-test-0.2.1/satelite/sentinel2/path_row_from_shp.py`

 * *Files identical despite different names*

### Comparing `satsure_core_test-0.2.0/satelite/sentinel2/s2_l1c_urls.py` & `satsure-core-test-0.2.1/satelite/sentinel2/s2_l1c_urls.py`

 * *Files identical despite different names*

### Comparing `satsure_core_test-0.2.0/satelite/sentinel2/s2_l2a_urls.py` & `satsure-core-test-0.2.1/satelite/sentinel2/s2_l2a_urls.py`

 * *Files identical despite different names*

### Comparing `satsure_core_test-0.2.0/satelite/tests/conftest.py` & `satsure-core-test-0.2.1/satelite/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `satsure_core_test-0.2.0/satelite/tests/sentinel2/test_genarate_band_stack.py` & `satsure-core-test-0.2.1/satelite/tests/sentinel2/test_genarate_band_stack.py`

 * *Files identical despite different names*

### Comparing `satsure_core_test-0.2.0/satelite/tests/sentinel2/test_general_indices.py` & `satsure-core-test-0.2.1/satelite/tests/sentinel2/test_general_indices.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     """Testcase for General Indices """
 
     def test_general_indices(self):
         """ test
 
         :return:
         """
-        base_path = "/Users/meenakshisundaram/Documents/airflow-dags-file"
+        base_path = "/Users/meenakshisundaram/Documents/airflow-dags-file/L2A/20240329"
         input_folder = Path(base_path)
         product_code = "IS18021"
         params = {'band_A_identifier': 'B04', 'band_B_identifier': 'B08',
                   'tile_identifier_position': 1, 'file_name_delimiter': '_',
                   'date_identifier_position': 0, 'band_combination_id': '8',
                   'input_file_format': 'tif',
                   'cloud_mask_bands': ('B02', 'B03'),
```

### Comparing `satsure_core_test-0.2.0/satelite/tests/sentinel2/test_get_tile.py` & `satsure-core-test-0.2.1/satelite/tests/sentinel2/test_get_tile.py`

 * *Files identical despite different names*

### Comparing `satsure_core_test-0.2.0/satelite/tests/sentinel2/test_s2_l1c_urls.py` & `satsure-core-test-0.2.1/satelite/tests/sentinel2/test_s2_l1c_urls.py`

 * *Files identical despite different names*

### Comparing `satsure_core_test-0.2.0/satelite/tests/sentinel2/test_s2_l2a_urls.py` & `satsure-core-test-0.2.1/satelite/tests/sentinel2/test_s2_l2a_urls.py`

 * *Files identical despite different names*

### Comparing `satsure_core_test-0.2.0/satelite/tests/sentinel2/test_validate.py` & `satsure-core-test-0.2.1/satelite/tests/sentinel2/test_validate.py`

 * *Files identical despite different names*

### Comparing `satsure_core_test-0.2.0/satelite/validators/check_shape_of_rid.py` & `satsure-core-test-0.2.1/satelite/validators/check_shape_of_rid.py`

 * *Files identical despite different names*

### Comparing `satsure_core_test-0.2.0/satsure_core_test.egg-info/SOURCES.txt` & `satsure-core-test-0.2.1/satsure_core_test.egg-info/SOURCES.txt`

 * *Files identical despite different names*

