# Comparing `tmp/satsure-core-test-0.2.1.tar.gz` & `tmp/satsure-core-test-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "satsure-core-test-0.2.1.tar", last modified: Thu May 16 05:32:43 2024, max compression
+gzip compressed data, was "satsure-core-test-0.2.2.tar", last modified: Thu May 16 05:50:17 2024, max compression
```

## Comparing `satsure-core-test-0.2.1.tar` & `satsure-core-test-0.2.2.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-16 05:32:43.644914 satsure-core-test-0.2.1/
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-04-25 07:48:02.000000 satsure-core-test-0.2.1/LICENCE.txt
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      515 2024-05-16 05:32:43.644672 satsure-core-test-0.2.1/PKG-INFO
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-04-25 07:48:18.000000 satsure-core-test-0.2.1/README.md
-drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-16 05:32:43.634975 satsure-core-test-0.2.1/satelite/
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-06 07:15:52.000000 satsure-core-test-0.2.1/satelite/__init__.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      976 2024-05-14 12:00:39.000000 satsure-core-test-0.2.1/satelite/config.py
-drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-16 05:32:43.635612 satsure-core-test-0.2.1/satelite/core/
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-13 07:33:26.000000 satsure-core-test-0.2.1/satelite/core/__init__.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     4877 2024-05-16 02:50:40.000000 satsure-core-test-0.2.1/satelite/core/downloader.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      825 2024-05-16 05:29:12.000000 satsure-core-test-0.2.1/satelite/core/uploader.py
-drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-16 05:32:43.636010 satsure-core-test-0.2.1/satelite/gdal/
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-13 07:33:26.000000 satsure-core-test-0.2.1/satelite/gdal/__init__.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     2511 2024-05-14 15:24:54.000000 satsure-core-test-0.2.1/satelite/gdal/gdal_commands.py
-drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-16 05:32:43.636336 satsure-core-test-0.2.1/satelite/models/
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-13 07:33:26.000000 satsure-core-test-0.2.1/satelite/models/__init__.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      372 2024-05-13 07:33:26.000000 satsure-core-test-0.2.1/satelite/models/s2_enum.py
-drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-16 05:32:43.636655 satsure-core-test-0.2.1/satelite/raster/
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-13 07:33:26.000000 satsure-core-test-0.2.1/satelite/raster/__init__.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     8913 2024-05-13 07:51:34.000000 satsure-core-test-0.2.1/satelite/raster/raster.py
-drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-16 05:32:43.638943 satsure-core-test-0.2.1/satelite/sentinel2/
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      499 2024-05-15 14:34:51.000000 satsure-core-test-0.2.1/satelite/sentinel2/__init__.py
-drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-16 05:32:43.639218 satsure-core-test-0.2.1/satelite/sentinel2/band_stack/
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-13 07:33:26.000000 satsure-core-test-0.2.1/satelite/sentinel2/band_stack/__init__.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     2834 2024-05-15 12:28:03.000000 satsure-core-test-0.2.1/satelite/sentinel2/band_stack/generate_band_stack.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     2429 2024-05-13 07:33:26.000000 satsure-core-test-0.2.1/satelite/sentinel2/fetch_unique_tile_date.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1634 2024-05-06 07:15:52.000000 satsure-core-test-0.2.1/satelite/sentinel2/fetch_unique_tile_date_pystac.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     3204 2024-05-14 12:04:20.000000 satsure-core-test-0.2.1/satelite/sentinel2/get_tiles.py
-drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-16 05:32:43.639666 satsure-core-test-0.2.1/satelite/sentinel2/indices/
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-13 07:33:26.000000 satsure-core-test-0.2.1/satelite/sentinel2/indices/__init__.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     3975 2024-05-15 12:01:41.000000 satsure-core-test-0.2.1/satelite/sentinel2/indices/general_indices.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      835 2024-05-15 14:22:44.000000 satsure-core-test-0.2.1/satelite/sentinel2/mosaic_custom_bands.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     2362 2024-05-15 14:15:25.000000 satsure-core-test-0.2.1/satelite/sentinel2/mosaic_same_bands.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1502 2024-05-13 07:51:34.000000 satsure-core-test-0.2.1/satelite/sentinel2/path_row_from_shp.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     3250 2024-05-13 07:33:26.000000 satsure-core-test-0.2.1/satelite/sentinel2/s2_l1c_urls.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     2912 2024-05-13 07:33:26.000000 satsure-core-test-0.2.1/satelite/sentinel2/s2_l2a_urls.py
-drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-16 05:32:43.640017 satsure-core-test-0.2.1/satelite/tests/
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-11 07:35:59.000000 satsure-core-test-0.2.1/satelite/tests/__init__.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1004 2024-05-14 12:00:39.000000 satsure-core-test-0.2.1/satelite/tests/conftest.py
-drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-16 05:32:43.642917 satsure-core-test-0.2.1/satelite/tests/sentinel2/
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-11 07:35:59.000000 satsure-core-test-0.2.1/satelite/tests/sentinel2/__init__.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      384 2024-05-13 07:58:31.000000 satsure-core-test-0.2.1/satelite/tests/sentinel2/test_fetch_unique_tile_date.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      430 2024-05-06 07:34:13.000000 satsure-core-test-0.2.1/satelite/tests/sentinel2/test_fetch_unique_tile_date_pystac.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1176 2024-05-15 12:53:42.000000 satsure-core-test-0.2.1/satelite/tests/sentinel2/test_genarate_band_stack.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1318 2024-05-16 03:04:58.000000 satsure-core-test-0.2.1/satelite/tests/sentinel2/test_general_indices.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1326 2024-05-14 12:00:39.000000 satsure-core-test-0.2.1/satelite/tests/sentinel2/test_get_tile.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      322 2024-05-13 07:33:26.000000 satsure-core-test-0.2.1/satelite/tests/sentinel2/test_mosaic_same_bands.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      871 2024-05-13 07:33:26.000000 satsure-core-test-0.2.1/satelite/tests/sentinel2/test_s2_l1c_urls.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      898 2024-05-13 07:33:26.000000 satsure-core-test-0.2.1/satelite/tests/sentinel2/test_s2_l2a_urls.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1543 2024-05-13 07:33:26.000000 satsure-core-test-0.2.1/satelite/tests/sentinel2/test_validate.py
-drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-16 05:32:43.643170 satsure-core-test-0.2.1/satelite/validators/
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-13 07:51:34.000000 satsure-core-test-0.2.1/satelite/validators/__init__.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     2381 2024-05-13 07:51:34.000000 satsure-core-test-0.2.1/satelite/validators/check_shape_of_rid.py
-drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-16 05:32:43.644292 satsure-core-test-0.2.1/satsure_core_test.egg-info/
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      515 2024-05-16 05:32:43.000000 satsure-core-test-0.2.1/satsure_core_test.egg-info/PKG-INFO
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1661 2024-05-16 05:32:43.000000 satsure-core-test-0.2.1/satsure_core_test.egg-info/SOURCES.txt
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)        1 2024-05-16 05:32:43.000000 satsure-core-test-0.2.1/satsure_core_test.egg-info/dependency_links.txt
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      141 2024-05-16 05:32:43.000000 satsure-core-test-0.2.1/satsure_core_test.egg-info/requires.txt
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)        9 2024-05-16 05:32:43.000000 satsure-core-test-0.2.1/satsure_core_test.egg-info/top_level.txt
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)       38 2024-05-16 05:32:43.644955 satsure-core-test-0.2.1/setup.cfg
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      493 2024-05-16 05:32:34.000000 satsure-core-test-0.2.1/setup.py
+drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-16 05:50:17.057100 satsure-core-test-0.2.2/
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-04-25 07:48:02.000000 satsure-core-test-0.2.2/LICENCE.txt
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      515 2024-05-16 05:50:17.056884 satsure-core-test-0.2.2/PKG-INFO
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-04-25 07:48:18.000000 satsure-core-test-0.2.2/README.md
+drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-16 05:50:17.047711 satsure-core-test-0.2.2/satelite/
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-06 07:15:52.000000 satsure-core-test-0.2.2/satelite/__init__.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      976 2024-05-14 12:00:39.000000 satsure-core-test-0.2.2/satelite/config.py
+drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-16 05:50:17.048444 satsure-core-test-0.2.2/satelite/core/
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-13 07:33:26.000000 satsure-core-test-0.2.2/satelite/core/__init__.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     4877 2024-05-16 02:50:40.000000 satsure-core-test-0.2.2/satelite/core/downloader.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      825 2024-05-16 05:29:12.000000 satsure-core-test-0.2.2/satelite/core/uploader.py
+drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-16 05:50:17.048904 satsure-core-test-0.2.2/satelite/gdal/
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-13 07:33:26.000000 satsure-core-test-0.2.2/satelite/gdal/__init__.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     2511 2024-05-14 15:24:54.000000 satsure-core-test-0.2.2/satelite/gdal/gdal_commands.py
+drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-16 05:50:17.049216 satsure-core-test-0.2.2/satelite/models/
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-13 07:33:26.000000 satsure-core-test-0.2.2/satelite/models/__init__.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      372 2024-05-13 07:33:26.000000 satsure-core-test-0.2.2/satelite/models/s2_enum.py
+drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-16 05:50:17.049531 satsure-core-test-0.2.2/satelite/raster/
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-13 07:33:26.000000 satsure-core-test-0.2.2/satelite/raster/__init__.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     8913 2024-05-13 07:51:34.000000 satsure-core-test-0.2.2/satelite/raster/raster.py
+drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-16 05:50:17.051828 satsure-core-test-0.2.2/satelite/sentinel2/
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      499 2024-05-15 14:34:51.000000 satsure-core-test-0.2.2/satelite/sentinel2/__init__.py
+drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-16 05:50:17.052178 satsure-core-test-0.2.2/satelite/sentinel2/band_stack/
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-13 07:33:26.000000 satsure-core-test-0.2.2/satelite/sentinel2/band_stack/__init__.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     2834 2024-05-15 12:28:03.000000 satsure-core-test-0.2.2/satelite/sentinel2/band_stack/generate_band_stack.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     2429 2024-05-13 07:33:26.000000 satsure-core-test-0.2.2/satelite/sentinel2/fetch_unique_tile_date.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1634 2024-05-06 07:15:52.000000 satsure-core-test-0.2.2/satelite/sentinel2/fetch_unique_tile_date_pystac.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     3204 2024-05-14 12:04:20.000000 satsure-core-test-0.2.2/satelite/sentinel2/get_tiles.py
+drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-16 05:50:17.052530 satsure-core-test-0.2.2/satelite/sentinel2/indices/
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-13 07:33:26.000000 satsure-core-test-0.2.2/satelite/sentinel2/indices/__init__.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     3975 2024-05-15 12:01:41.000000 satsure-core-test-0.2.2/satelite/sentinel2/indices/general_indices.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      835 2024-05-15 14:22:44.000000 satsure-core-test-0.2.2/satelite/sentinel2/mosaic_custom_bands.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     2362 2024-05-15 14:15:25.000000 satsure-core-test-0.2.2/satelite/sentinel2/mosaic_same_bands.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1502 2024-05-13 07:51:34.000000 satsure-core-test-0.2.2/satelite/sentinel2/path_row_from_shp.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     3251 2024-05-16 05:49:19.000000 satsure-core-test-0.2.2/satelite/sentinel2/s2_l1c_urls.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     2912 2024-05-13 07:33:26.000000 satsure-core-test-0.2.2/satelite/sentinel2/s2_l2a_urls.py
+drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-16 05:50:17.052835 satsure-core-test-0.2.2/satelite/tests/
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-11 07:35:59.000000 satsure-core-test-0.2.2/satelite/tests/__init__.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1004 2024-05-14 12:00:39.000000 satsure-core-test-0.2.2/satelite/tests/conftest.py
+drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-16 05:50:17.055760 satsure-core-test-0.2.2/satelite/tests/sentinel2/
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-11 07:35:59.000000 satsure-core-test-0.2.2/satelite/tests/sentinel2/__init__.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      384 2024-05-13 07:58:31.000000 satsure-core-test-0.2.2/satelite/tests/sentinel2/test_fetch_unique_tile_date.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      430 2024-05-06 07:34:13.000000 satsure-core-test-0.2.2/satelite/tests/sentinel2/test_fetch_unique_tile_date_pystac.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1176 2024-05-15 12:53:42.000000 satsure-core-test-0.2.2/satelite/tests/sentinel2/test_genarate_band_stack.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1318 2024-05-16 03:04:58.000000 satsure-core-test-0.2.2/satelite/tests/sentinel2/test_general_indices.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1326 2024-05-14 12:00:39.000000 satsure-core-test-0.2.2/satelite/tests/sentinel2/test_get_tile.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      322 2024-05-13 07:33:26.000000 satsure-core-test-0.2.2/satelite/tests/sentinel2/test_mosaic_same_bands.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      871 2024-05-13 07:33:26.000000 satsure-core-test-0.2.2/satelite/tests/sentinel2/test_s2_l1c_urls.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      898 2024-05-13 07:33:26.000000 satsure-core-test-0.2.2/satelite/tests/sentinel2/test_s2_l2a_urls.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1543 2024-05-13 07:33:26.000000 satsure-core-test-0.2.2/satelite/tests/sentinel2/test_validate.py
+drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-16 05:50:17.056017 satsure-core-test-0.2.2/satelite/validators/
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-13 07:51:34.000000 satsure-core-test-0.2.2/satelite/validators/__init__.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     2381 2024-05-13 07:51:34.000000 satsure-core-test-0.2.2/satelite/validators/check_shape_of_rid.py
+drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-16 05:50:17.056677 satsure-core-test-0.2.2/satsure_core_test.egg-info/
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      515 2024-05-16 05:50:16.000000 satsure-core-test-0.2.2/satsure_core_test.egg-info/PKG-INFO
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1661 2024-05-16 05:50:17.000000 satsure-core-test-0.2.2/satsure_core_test.egg-info/SOURCES.txt
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)        1 2024-05-16 05:50:16.000000 satsure-core-test-0.2.2/satsure_core_test.egg-info/dependency_links.txt
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      141 2024-05-16 05:50:16.000000 satsure-core-test-0.2.2/satsure_core_test.egg-info/requires.txt
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)        9 2024-05-16 05:50:16.000000 satsure-core-test-0.2.2/satsure_core_test.egg-info/top_level.txt
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)       38 2024-05-16 05:50:17.057148 satsure-core-test-0.2.2/setup.cfg
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      493 2024-05-16 05:50:15.000000 satsure-core-test-0.2.2/setup.py
```

### Comparing `satsure-core-test-0.2.1/PKG-INFO` & `satsure-core-test-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: satsure-core-test
-Version: 0.2.1
+Version: 0.2.2
 Summary: satsure core package
 Author: Satsure
 Author-email: kmstpm@email.com
 License-File: LICENCE.txt
 Requires-Dist: awscli
 Requires-Dist: fiona
 Requires-Dist: gdal==3.6.2
```

### Comparing `satsure-core-test-0.2.1/satelite/config.py` & `satsure-core-test-0.2.2/satelite/config.py`

 * *Files identical despite different names*

### Comparing `satsure-core-test-0.2.1/satelite/core/downloader.py` & `satsure-core-test-0.2.2/satelite/core/downloader.py`

 * *Files identical despite different names*

### Comparing `satsure-core-test-0.2.1/satelite/core/uploader.py` & `satsure-core-test-0.2.2/satelite/core/uploader.py`

 * *Files identical despite different names*

### Comparing `satsure-core-test-0.2.1/satelite/gdal/gdal_commands.py` & `satsure-core-test-0.2.2/satelite/gdal/gdal_commands.py`

 * *Files identical despite different names*

### Comparing `satsure-core-test-0.2.1/satelite/raster/raster.py` & `satsure-core-test-0.2.2/satelite/raster/raster.py`

 * *Files identical despite different names*

### Comparing `satsure-core-test-0.2.1/satelite/sentinel2/band_stack/generate_band_stack.py` & `satsure-core-test-0.2.2/satelite/sentinel2/band_stack/generate_band_stack.py`

 * *Files identical despite different names*

### Comparing `satsure-core-test-0.2.1/satelite/sentinel2/fetch_unique_tile_date.py` & `satsure-core-test-0.2.2/satelite/sentinel2/fetch_unique_tile_date.py`

 * *Files identical despite different names*

### Comparing `satsure-core-test-0.2.1/satelite/sentinel2/fetch_unique_tile_date_pystac.py` & `satsure-core-test-0.2.2/satelite/sentinel2/fetch_unique_tile_date_pystac.py`

 * *Files identical despite different names*

### Comparing `satsure-core-test-0.2.1/satelite/sentinel2/get_tiles.py` & `satsure-core-test-0.2.2/satelite/sentinel2/get_tiles.py`

 * *Files identical despite different names*

### Comparing `satsure-core-test-0.2.1/satelite/sentinel2/indices/general_indices.py` & `satsure-core-test-0.2.2/satelite/sentinel2/indices/general_indices.py`

 * *Files identical despite different names*

### Comparing `satsure-core-test-0.2.1/satelite/sentinel2/mosaic_custom_bands.py` & `satsure-core-test-0.2.2/satelite/sentinel2/mosaic_custom_bands.py`

 * *Files identical despite different names*

### Comparing `satsure-core-test-0.2.1/satelite/sentinel2/mosaic_same_bands.py` & `satsure-core-test-0.2.2/satelite/sentinel2/mosaic_same_bands.py`

 * *Files identical despite different names*

### Comparing `satsure-core-test-0.2.1/satelite/sentinel2/path_row_from_shp.py` & `satsure-core-test-0.2.2/satelite/sentinel2/path_row_from_shp.py`

 * *Files identical despite different names*

### Comparing `satsure-core-test-0.2.1/satelite/sentinel2/s2_l1c_urls.py` & `satsure-core-test-0.2.2/satelite/sentinel2/s2_l1c_urls.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,15 +36,15 @@
         gcs_bucket = gcs.get_bucket(S3_L1C_BUCKET)
         prefix = f"tiles/{tile_code[:2]}/{tile_code[2]}/{tile_code[-2:]}/"
         blobs = gcs_bucket.list_blobs(
             max_results=10000, prefix=prefix, delimiter="/")
         next(blobs, ...)
         date = str(from_date).replace("-", "")
         manifest_files = [
-            f"{GCP_BASE_URL}{S3_L1C_BUCKET}/{blob}manifest.safe"
+            f"{ GCP_BASE_URL}{S3_L1C_BUCKET}/{blob}manifest.safe"
             for blob in blobs.prefixes if date in blob
         ]
 
         return manifest_files
 
     def get_urls(self, tile_code: str, from_date: str,
                  download_path: PosixPath,
```

### Comparing `satsure-core-test-0.2.1/satelite/sentinel2/s2_l2a_urls.py` & `satsure-core-test-0.2.2/satelite/sentinel2/s2_l2a_urls.py`

 * *Files identical despite different names*

### Comparing `satsure-core-test-0.2.1/satelite/tests/conftest.py` & `satsure-core-test-0.2.2/satelite/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `satsure-core-test-0.2.1/satelite/tests/sentinel2/test_genarate_band_stack.py` & `satsure-core-test-0.2.2/satelite/tests/sentinel2/test_genarate_band_stack.py`

 * *Files identical despite different names*

### Comparing `satsure-core-test-0.2.1/satelite/tests/sentinel2/test_general_indices.py` & `satsure-core-test-0.2.2/satelite/tests/sentinel2/test_general_indices.py`

 * *Files identical despite different names*

### Comparing `satsure-core-test-0.2.1/satelite/tests/sentinel2/test_get_tile.py` & `satsure-core-test-0.2.2/satelite/tests/sentinel2/test_get_tile.py`

 * *Files identical despite different names*

### Comparing `satsure-core-test-0.2.1/satelite/tests/sentinel2/test_s2_l1c_urls.py` & `satsure-core-test-0.2.2/satelite/tests/sentinel2/test_s2_l1c_urls.py`

 * *Files identical despite different names*

### Comparing `satsure-core-test-0.2.1/satelite/tests/sentinel2/test_s2_l2a_urls.py` & `satsure-core-test-0.2.2/satelite/tests/sentinel2/test_s2_l2a_urls.py`

 * *Files identical despite different names*

### Comparing `satsure-core-test-0.2.1/satelite/tests/sentinel2/test_validate.py` & `satsure-core-test-0.2.2/satelite/tests/sentinel2/test_validate.py`

 * *Files identical despite different names*

### Comparing `satsure-core-test-0.2.1/satelite/validators/check_shape_of_rid.py` & `satsure-core-test-0.2.2/satelite/validators/check_shape_of_rid.py`

 * *Files identical despite different names*

### Comparing `satsure-core-test-0.2.1/satsure_core_test.egg-info/PKG-INFO` & `satsure-core-test-0.2.2/satsure_core_test.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: satsure-core-test
-Version: 0.2.1
+Version: 0.2.2
 Summary: satsure core package
 Author: Satsure
 Author-email: kmstpm@email.com
 License-File: LICENCE.txt
 Requires-Dist: awscli
 Requires-Dist: fiona
 Requires-Dist: gdal==3.6.2
```

### Comparing `satsure-core-test-0.2.1/satsure_core_test.egg-info/SOURCES.txt` & `satsure-core-test-0.2.2/satsure_core_test.egg-info/SOURCES.txt`

 * *Files identical despite different names*

