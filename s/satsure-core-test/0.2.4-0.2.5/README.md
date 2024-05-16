# Comparing `tmp/satsure-core-test-0.2.4.tar.gz` & `tmp/satsure-core-test-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "satsure-core-test-0.2.4.tar", last modified: Thu May 16 06:12:17 2024, max compression
+gzip compressed data, was "satsure-core-test-0.2.5.tar", last modified: Thu May 16 08:31:52 2024, max compression
```

## Comparing `satsure-core-test-0.2.4.tar` & `satsure-core-test-0.2.5.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-16 06:12:17.389426 satsure-core-test-0.2.4/
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-04-25 07:48:02.000000 satsure-core-test-0.2.4/LICENCE.txt
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)       24 2024-05-16 06:11:06.000000 satsure-core-test-0.2.4/MANIFEST.in
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      515 2024-05-16 06:12:17.389219 satsure-core-test-0.2.4/PKG-INFO
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-04-25 07:48:18.000000 satsure-core-test-0.2.4/README.md
-drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-16 06:12:17.378710 satsure-core-test-0.2.4/satelite/
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-06 07:15:52.000000 satsure-core-test-0.2.4/satelite/__init__.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      976 2024-05-16 05:55:40.000000 satsure-core-test-0.2.4/satelite/config.py
-drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-16 06:12:17.379314 satsure-core-test-0.2.4/satelite/core/
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-13 07:33:26.000000 satsure-core-test-0.2.4/satelite/core/__init__.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     4877 2024-05-16 02:50:40.000000 satsure-core-test-0.2.4/satelite/core/downloader.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      825 2024-05-16 05:29:12.000000 satsure-core-test-0.2.4/satelite/core/uploader.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     2361 2024-04-25 12:00:27.000000 satsure-core-test-0.2.4/satelite/gcp.json
-drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-16 06:12:17.379719 satsure-core-test-0.2.4/satelite/gdal/
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-13 07:33:26.000000 satsure-core-test-0.2.4/satelite/gdal/__init__.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     2511 2024-05-14 15:24:54.000000 satsure-core-test-0.2.4/satelite/gdal/gdal_commands.py
-drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-16 06:12:17.380286 satsure-core-test-0.2.4/satelite/models/
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-13 07:33:26.000000 satsure-core-test-0.2.4/satelite/models/__init__.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      372 2024-05-13 07:33:26.000000 satsure-core-test-0.2.4/satelite/models/s2_enum.py
-drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-16 06:12:17.380598 satsure-core-test-0.2.4/satelite/raster/
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-13 07:33:26.000000 satsure-core-test-0.2.4/satelite/raster/__init__.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     8913 2024-05-13 07:51:34.000000 satsure-core-test-0.2.4/satelite/raster/raster.py
-drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-16 06:12:17.383441 satsure-core-test-0.2.4/satelite/sentinel2/
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      499 2024-05-15 14:34:51.000000 satsure-core-test-0.2.4/satelite/sentinel2/__init__.py
-drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-16 06:12:17.383828 satsure-core-test-0.2.4/satelite/sentinel2/band_stack/
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-13 07:33:26.000000 satsure-core-test-0.2.4/satelite/sentinel2/band_stack/__init__.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     2834 2024-05-15 12:28:03.000000 satsure-core-test-0.2.4/satelite/sentinel2/band_stack/generate_band_stack.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     2429 2024-05-13 07:33:26.000000 satsure-core-test-0.2.4/satelite/sentinel2/fetch_unique_tile_date.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1634 2024-05-06 07:15:52.000000 satsure-core-test-0.2.4/satelite/sentinel2/fetch_unique_tile_date_pystac.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     3204 2024-05-14 12:04:20.000000 satsure-core-test-0.2.4/satelite/sentinel2/get_tiles.py
-drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-16 06:12:17.384197 satsure-core-test-0.2.4/satelite/sentinel2/indices/
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-13 07:33:26.000000 satsure-core-test-0.2.4/satelite/sentinel2/indices/__init__.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     3975 2024-05-15 12:01:41.000000 satsure-core-test-0.2.4/satelite/sentinel2/indices/general_indices.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      835 2024-05-15 14:22:44.000000 satsure-core-test-0.2.4/satelite/sentinel2/mosaic_custom_bands.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     2362 2024-05-15 14:15:25.000000 satsure-core-test-0.2.4/satelite/sentinel2/mosaic_same_bands.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1502 2024-05-13 07:51:34.000000 satsure-core-test-0.2.4/satelite/sentinel2/path_row_from_shp.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     3251 2024-05-16 05:49:19.000000 satsure-core-test-0.2.4/satelite/sentinel2/s2_l1c_urls.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     2912 2024-05-13 07:33:26.000000 satsure-core-test-0.2.4/satelite/sentinel2/s2_l2a_urls.py
-drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-16 06:12:17.384539 satsure-core-test-0.2.4/satelite/tests/
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-11 07:35:59.000000 satsure-core-test-0.2.4/satelite/tests/__init__.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1004 2024-05-14 12:00:39.000000 satsure-core-test-0.2.4/satelite/tests/conftest.py
-drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-16 06:12:17.387656 satsure-core-test-0.2.4/satelite/tests/sentinel2/
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-11 07:35:59.000000 satsure-core-test-0.2.4/satelite/tests/sentinel2/__init__.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      384 2024-05-13 07:58:31.000000 satsure-core-test-0.2.4/satelite/tests/sentinel2/test_fetch_unique_tile_date.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      430 2024-05-06 07:34:13.000000 satsure-core-test-0.2.4/satelite/tests/sentinel2/test_fetch_unique_tile_date_pystac.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1176 2024-05-15 12:53:42.000000 satsure-core-test-0.2.4/satelite/tests/sentinel2/test_genarate_band_stack.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1318 2024-05-16 03:04:58.000000 satsure-core-test-0.2.4/satelite/tests/sentinel2/test_general_indices.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1326 2024-05-14 12:00:39.000000 satsure-core-test-0.2.4/satelite/tests/sentinel2/test_get_tile.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      322 2024-05-13 07:33:26.000000 satsure-core-test-0.2.4/satelite/tests/sentinel2/test_mosaic_same_bands.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      871 2024-05-13 07:33:26.000000 satsure-core-test-0.2.4/satelite/tests/sentinel2/test_s2_l1c_urls.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      898 2024-05-13 07:33:26.000000 satsure-core-test-0.2.4/satelite/tests/sentinel2/test_s2_l2a_urls.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1543 2024-05-13 07:33:26.000000 satsure-core-test-0.2.4/satelite/tests/sentinel2/test_validate.py
-drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-16 06:12:17.387885 satsure-core-test-0.2.4/satelite/validators/
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-13 07:51:34.000000 satsure-core-test-0.2.4/satelite/validators/__init__.py
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     2381 2024-05-13 07:51:34.000000 satsure-core-test-0.2.4/satelite/validators/check_shape_of_rid.py
-drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-16 06:12:17.388866 satsure-core-test-0.2.4/satsure_core_test.egg-info/
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      515 2024-05-16 06:12:17.000000 satsure-core-test-0.2.4/satsure_core_test.egg-info/PKG-INFO
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1691 2024-05-16 06:12:17.000000 satsure-core-test-0.2.4/satsure_core_test.egg-info/SOURCES.txt
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)        1 2024-05-16 06:12:17.000000 satsure-core-test-0.2.4/satsure_core_test.egg-info/dependency_links.txt
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      141 2024-05-16 06:12:17.000000 satsure-core-test-0.2.4/satsure_core_test.egg-info/requires.txt
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)        9 2024-05-16 06:12:17.000000 satsure-core-test-0.2.4/satsure_core_test.egg-info/top_level.txt
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)       38 2024-05-16 06:12:17.389468 satsure-core-test-0.2.4/setup.cfg
--rw-r--r--   0 meenakshisundaram   (501) staff       (20)      601 2024-05-16 06:12:13.000000 satsure-core-test-0.2.4/setup.py
+drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-16 08:31:52.165440 satsure-core-test-0.2.5/
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-04-25 07:48:02.000000 satsure-core-test-0.2.5/LICENCE.txt
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)       24 2024-05-16 06:11:06.000000 satsure-core-test-0.2.5/MANIFEST.in
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      515 2024-05-16 08:31:52.165253 satsure-core-test-0.2.5/PKG-INFO
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-04-25 07:48:18.000000 satsure-core-test-0.2.5/README.md
+drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-16 08:31:52.156683 satsure-core-test-0.2.5/satelite/
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-06 07:15:52.000000 satsure-core-test-0.2.5/satelite/__init__.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      976 2024-05-16 05:55:40.000000 satsure-core-test-0.2.5/satelite/config.py
+drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-16 08:31:52.157372 satsure-core-test-0.2.5/satelite/core/
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-13 07:33:26.000000 satsure-core-test-0.2.5/satelite/core/__init__.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     4877 2024-05-16 02:50:40.000000 satsure-core-test-0.2.5/satelite/core/downloader.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      825 2024-05-16 05:29:12.000000 satsure-core-test-0.2.5/satelite/core/uploader.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     2361 2024-04-25 12:00:27.000000 satsure-core-test-0.2.5/satelite/gcp.json
+drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-16 08:31:52.157767 satsure-core-test-0.2.5/satelite/gdal/
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-13 07:33:26.000000 satsure-core-test-0.2.5/satelite/gdal/__init__.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     2511 2024-05-14 15:24:54.000000 satsure-core-test-0.2.5/satelite/gdal/gdal_commands.py
+drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-16 08:31:52.158074 satsure-core-test-0.2.5/satelite/models/
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-13 07:33:26.000000 satsure-core-test-0.2.5/satelite/models/__init__.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      372 2024-05-13 07:33:26.000000 satsure-core-test-0.2.5/satelite/models/s2_enum.py
+drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-16 08:31:52.158359 satsure-core-test-0.2.5/satelite/raster/
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-13 07:33:26.000000 satsure-core-test-0.2.5/satelite/raster/__init__.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     8913 2024-05-13 07:51:34.000000 satsure-core-test-0.2.5/satelite/raster/raster.py
+drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-16 08:31:52.160742 satsure-core-test-0.2.5/satelite/sentinel2/
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      499 2024-05-15 14:34:51.000000 satsure-core-test-0.2.5/satelite/sentinel2/__init__.py
+drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-16 08:31:52.161077 satsure-core-test-0.2.5/satelite/sentinel2/band_stack/
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-13 07:33:26.000000 satsure-core-test-0.2.5/satelite/sentinel2/band_stack/__init__.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     2834 2024-05-15 12:28:03.000000 satsure-core-test-0.2.5/satelite/sentinel2/band_stack/generate_band_stack.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     2429 2024-05-13 07:33:26.000000 satsure-core-test-0.2.5/satelite/sentinel2/fetch_unique_tile_date.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1634 2024-05-06 07:15:52.000000 satsure-core-test-0.2.5/satelite/sentinel2/fetch_unique_tile_date_pystac.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     3204 2024-05-14 12:04:20.000000 satsure-core-test-0.2.5/satelite/sentinel2/get_tiles.py
+drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-16 08:31:52.161398 satsure-core-test-0.2.5/satelite/sentinel2/indices/
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-13 07:33:26.000000 satsure-core-test-0.2.5/satelite/sentinel2/indices/__init__.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     3975 2024-05-15 12:01:41.000000 satsure-core-test-0.2.5/satelite/sentinel2/indices/general_indices.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      835 2024-05-15 14:22:44.000000 satsure-core-test-0.2.5/satelite/sentinel2/mosaic_custom_bands.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     2553 2024-05-16 08:31:36.000000 satsure-core-test-0.2.5/satelite/sentinel2/mosaic_same_bands.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1502 2024-05-13 07:51:34.000000 satsure-core-test-0.2.5/satelite/sentinel2/path_row_from_shp.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     3251 2024-05-16 05:49:19.000000 satsure-core-test-0.2.5/satelite/sentinel2/s2_l1c_urls.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     2912 2024-05-13 07:33:26.000000 satsure-core-test-0.2.5/satelite/sentinel2/s2_l2a_urls.py
+drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-16 08:31:52.161710 satsure-core-test-0.2.5/satelite/tests/
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-11 07:35:59.000000 satsure-core-test-0.2.5/satelite/tests/__init__.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1004 2024-05-14 12:00:39.000000 satsure-core-test-0.2.5/satelite/tests/conftest.py
+drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-16 08:31:52.164208 satsure-core-test-0.2.5/satelite/tests/sentinel2/
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-11 07:35:59.000000 satsure-core-test-0.2.5/satelite/tests/sentinel2/__init__.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      384 2024-05-13 07:58:31.000000 satsure-core-test-0.2.5/satelite/tests/sentinel2/test_fetch_unique_tile_date.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      430 2024-05-06 07:34:13.000000 satsure-core-test-0.2.5/satelite/tests/sentinel2/test_fetch_unique_tile_date_pystac.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1176 2024-05-15 12:53:42.000000 satsure-core-test-0.2.5/satelite/tests/sentinel2/test_genarate_band_stack.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1318 2024-05-16 03:04:58.000000 satsure-core-test-0.2.5/satelite/tests/sentinel2/test_general_indices.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1326 2024-05-14 12:00:39.000000 satsure-core-test-0.2.5/satelite/tests/sentinel2/test_get_tile.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      322 2024-05-13 07:33:26.000000 satsure-core-test-0.2.5/satelite/tests/sentinel2/test_mosaic_same_bands.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      871 2024-05-13 07:33:26.000000 satsure-core-test-0.2.5/satelite/tests/sentinel2/test_s2_l1c_urls.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      898 2024-05-13 07:33:26.000000 satsure-core-test-0.2.5/satelite/tests/sentinel2/test_s2_l2a_urls.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1543 2024-05-13 07:33:26.000000 satsure-core-test-0.2.5/satelite/tests/sentinel2/test_validate.py
+drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-16 08:31:52.164436 satsure-core-test-0.2.5/satelite/validators/
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)        0 2024-05-13 07:51:34.000000 satsure-core-test-0.2.5/satelite/validators/__init__.py
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     2381 2024-05-13 07:51:34.000000 satsure-core-test-0.2.5/satelite/validators/check_shape_of_rid.py
+drwxr-xr-x   0 meenakshisundaram   (501) staff       (20)        0 2024-05-16 08:31:52.165057 satsure-core-test-0.2.5/satsure_core_test.egg-info/
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      515 2024-05-16 08:31:52.000000 satsure-core-test-0.2.5/satsure_core_test.egg-info/PKG-INFO
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)     1691 2024-05-16 08:31:52.000000 satsure-core-test-0.2.5/satsure_core_test.egg-info/SOURCES.txt
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)        1 2024-05-16 08:31:52.000000 satsure-core-test-0.2.5/satsure_core_test.egg-info/dependency_links.txt
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      141 2024-05-16 08:31:52.000000 satsure-core-test-0.2.5/satsure_core_test.egg-info/requires.txt
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)        9 2024-05-16 08:31:52.000000 satsure-core-test-0.2.5/satsure_core_test.egg-info/top_level.txt
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)       38 2024-05-16 08:31:52.165481 satsure-core-test-0.2.5/setup.cfg
+-rw-r--r--   0 meenakshisundaram   (501) staff       (20)      601 2024-05-16 08:31:51.000000 satsure-core-test-0.2.5/setup.py
```

### Comparing `satsure-core-test-0.2.4/PKG-INFO` & `satsure-core-test-0.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: satsure-core-test
-Version: 0.2.4
+Version: 0.2.5
 Summary: satsure core package
 Author: Satsure
 Author-email: kmstpm@email.com
 License-File: LICENCE.txt
 Requires-Dist: awscli
 Requires-Dist: fiona
 Requires-Dist: gdal==3.6.2
```

### Comparing `satsure-core-test-0.2.4/satelite/config.py` & `satsure-core-test-0.2.5/satelite/config.py`

 * *Files identical despite different names*

### Comparing `satsure-core-test-0.2.4/satelite/core/downloader.py` & `satsure-core-test-0.2.5/satelite/core/downloader.py`

 * *Files identical despite different names*

### Comparing `satsure-core-test-0.2.4/satelite/core/uploader.py` & `satsure-core-test-0.2.5/satelite/core/uploader.py`

 * *Files identical despite different names*

### Comparing `satsure-core-test-0.2.4/satelite/gcp.json` & `satsure-core-test-0.2.5/satelite/gcp.json`

 * *Files identical despite different names*

### Comparing `satsure-core-test-0.2.4/satelite/gdal/gdal_commands.py` & `satsure-core-test-0.2.5/satelite/gdal/gdal_commands.py`

 * *Files identical despite different names*

### Comparing `satsure-core-test-0.2.4/satelite/raster/raster.py` & `satsure-core-test-0.2.5/satelite/raster/raster.py`

 * *Files identical despite different names*

### Comparing `satsure-core-test-0.2.4/satelite/sentinel2/band_stack/generate_band_stack.py` & `satsure-core-test-0.2.5/satelite/sentinel2/band_stack/generate_band_stack.py`

 * *Files identical despite different names*

### Comparing `satsure-core-test-0.2.4/satelite/sentinel2/fetch_unique_tile_date.py` & `satsure-core-test-0.2.5/satelite/sentinel2/fetch_unique_tile_date.py`

 * *Files identical despite different names*

### Comparing `satsure-core-test-0.2.4/satelite/sentinel2/fetch_unique_tile_date_pystac.py` & `satsure-core-test-0.2.5/satelite/sentinel2/fetch_unique_tile_date_pystac.py`

 * *Files identical despite different names*

### Comparing `satsure-core-test-0.2.4/satelite/sentinel2/get_tiles.py` & `satsure-core-test-0.2.5/satelite/sentinel2/get_tiles.py`

 * *Files identical despite different names*

### Comparing `satsure-core-test-0.2.4/satelite/sentinel2/indices/general_indices.py` & `satsure-core-test-0.2.5/satelite/sentinel2/indices/general_indices.py`

 * *Files identical despite different names*

### Comparing `satsure-core-test-0.2.4/satelite/sentinel2/mosaic_custom_bands.py` & `satsure-core-test-0.2.5/satelite/sentinel2/mosaic_custom_bands.py`

 * *Files identical despite different names*

### Comparing `satsure-core-test-0.2.4/satelite/sentinel2/mosaic_same_bands.py` & `satsure-core-test-0.2.5/satelite/sentinel2/mosaic_same_bands.py`

 * *Files 4% similar despite different names*

```diff
@@ -58,7 +58,12 @@
                     keep_separate=False,
                     output_format=None,
                     output_datatype=None,
                     output_crs=None,
                     output_pixel_size=(10, 10),
                     creation_option=creation_option
                 )
+
+                for file in files:
+                    if file.name == f"{date}_{unique_tile}_{band}.{input_file_format}":
+                        continue
+                    file.unlink()
```

### Comparing `satsure-core-test-0.2.4/satelite/sentinel2/path_row_from_shp.py` & `satsure-core-test-0.2.5/satelite/sentinel2/path_row_from_shp.py`

 * *Files identical despite different names*

### Comparing `satsure-core-test-0.2.4/satelite/sentinel2/s2_l1c_urls.py` & `satsure-core-test-0.2.5/satelite/sentinel2/s2_l1c_urls.py`

 * *Files identical despite different names*

### Comparing `satsure-core-test-0.2.4/satelite/sentinel2/s2_l2a_urls.py` & `satsure-core-test-0.2.5/satelite/sentinel2/s2_l2a_urls.py`

 * *Files identical despite different names*

### Comparing `satsure-core-test-0.2.4/satelite/tests/conftest.py` & `satsure-core-test-0.2.5/satelite/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `satsure-core-test-0.2.4/satelite/tests/sentinel2/test_genarate_band_stack.py` & `satsure-core-test-0.2.5/satelite/tests/sentinel2/test_genarate_band_stack.py`

 * *Files identical despite different names*

### Comparing `satsure-core-test-0.2.4/satelite/tests/sentinel2/test_general_indices.py` & `satsure-core-test-0.2.5/satelite/tests/sentinel2/test_general_indices.py`

 * *Files identical despite different names*

### Comparing `satsure-core-test-0.2.4/satelite/tests/sentinel2/test_get_tile.py` & `satsure-core-test-0.2.5/satelite/tests/sentinel2/test_get_tile.py`

 * *Files identical despite different names*

### Comparing `satsure-core-test-0.2.4/satelite/tests/sentinel2/test_s2_l1c_urls.py` & `satsure-core-test-0.2.5/satelite/tests/sentinel2/test_s2_l1c_urls.py`

 * *Files identical despite different names*

### Comparing `satsure-core-test-0.2.4/satelite/tests/sentinel2/test_s2_l2a_urls.py` & `satsure-core-test-0.2.5/satelite/tests/sentinel2/test_s2_l2a_urls.py`

 * *Files identical despite different names*

### Comparing `satsure-core-test-0.2.4/satelite/tests/sentinel2/test_validate.py` & `satsure-core-test-0.2.5/satelite/tests/sentinel2/test_validate.py`

 * *Files identical despite different names*

### Comparing `satsure-core-test-0.2.4/satelite/validators/check_shape_of_rid.py` & `satsure-core-test-0.2.5/satelite/validators/check_shape_of_rid.py`

 * *Files identical despite different names*

### Comparing `satsure-core-test-0.2.4/satsure_core_test.egg-info/PKG-INFO` & `satsure-core-test-0.2.5/satsure_core_test.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: satsure-core-test
-Version: 0.2.4
+Version: 0.2.5
 Summary: satsure core package
 Author: Satsure
 Author-email: kmstpm@email.com
 License-File: LICENCE.txt
 Requires-Dist: awscli
 Requires-Dist: fiona
 Requires-Dist: gdal==3.6.2
```

### Comparing `satsure-core-test-0.2.4/satsure_core_test.egg-info/SOURCES.txt` & `satsure-core-test-0.2.5/satsure_core_test.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `satsure-core-test-0.2.4/setup.py` & `satsure-core-test-0.2.5/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 
 setup(
     name='satsure-core-test',
-    version='0.2.4',
+    version='0.2.5',
     description='satsure core package',
     author='Satsure',
     author_email='kmstpm@email.com',
     packages=find_packages(),
     install_requires=['awscli', 'fiona','gdal==3.6.2', 'google-cloud-storage', 'pandas',
                       'pyproj', 'pystac','pystac-client', 'python-dotenv', 'rasterstats',
                       'rasterio', 'requests', 'requests', 'sqlalchemy', 'wget'],
```

