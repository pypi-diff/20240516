# Comparing `tmp/xradio-0.0.8.tar.gz` & `tmp/xradio-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xradio-0.0.8.tar", last modified: Thu Oct 19 16:11:29 2023, max compression
+gzip compressed data, was "xradio-0.0.9.tar", last modified: Wed Oct 25 01:51:18 2023, max compression
```

## Comparing `xradio-0.0.8.tar` & `xradio-0.0.9.tar`

### file list

```diff
@@ -1,80 +1,80 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-19 16:11:29.175403 xradio-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1516 2023-10-19 16:11:13.000000 xradio-0.0.8/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)       94 2023-10-19 16:11:13.000000 xradio-0.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3985 2023-10-19 16:11:29.175403 xradio-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      959 2023-10-19 16:11:13.000000 xradio-0.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      808 2023-10-19 16:11:13.000000 xradio-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-19 16:11:29.175403 xradio-0.0.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-19 16:11:29.159403 xradio-0.0.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-19 16:11:29.163403 xradio-0.0.8/src/xradio/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-19 16:11:13.000000 xradio-0.0.8/src/xradio/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-19 16:11:29.163403 xradio-0.0.8/src/xradio/_utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-19 16:11:13.000000 xradio-0.0.8/src/xradio/_utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-19 16:11:29.163403 xradio-0.0.8/src/xradio/data/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-19 16:11:13.000000 xradio-0.0.8/src/xradio/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2288 2023-10-19 16:11:13.000000 xradio-0.0.8/src/xradio/data/_dropbox.py
--rw-r--r--   0 runner    (1001) docker     (127)     4340 2023-10-19 16:11:13.000000 xradio-0.0.8/src/xradio/data/_google_drive.py
--rw-r--r--   0 runner    (1001) docker     (127)      457 2023-10-19 16:11:13.000000 xradio-0.0.8/src/xradio/data/datasets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-19 16:11:29.163403 xradio-0.0.8/src/xradio/image/
--rw-r--r--   0 runner    (1001) docker     (127)      291 2023-10-19 16:11:13.000000 xradio-0.0.8/src/xradio/image/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-19 16:11:29.167403 xradio-0.0.8/src/xradio/image/_util/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-19 16:11:29.167403 xradio-0.0.8/src/xradio/image/_util/_casacore/
--rw-r--r--   0 runner    (1001) docker     (127)       42 2023-10-19 16:11:13.000000 xradio-0.0.8/src/xradio/image/_util/_casacore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      165 2023-10-19 16:11:13.000000 xradio-0.0.8/src/xradio/image/_util/_casacore/common.py
--rw-r--r--   0 runner    (1001) docker     (127)    39144 2023-10-19 16:11:13.000000 xradio-0.0.8/src/xradio/image/_util/_casacore/xds_from_casacore.py
--rw-r--r--   0 runner    (1001) docker     (127)    13918 2023-10-19 16:11:13.000000 xradio-0.0.8/src/xradio/image/_util/_casacore/xds_to_casacore.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-19 16:11:29.167403 xradio-0.0.8/src/xradio/image/_util/_fits/
--rw-r--r--   0 runner    (1001) docker     (127)    26637 2023-10-19 16:11:13.000000 xradio-0.0.8/src/xradio/image/_util/_fits/xds_from_fits.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-19 16:11:29.167403 xradio-0.0.8/src/xradio/image/_util/_zarr/
--rw-r--r--   0 runner    (1001) docker     (127)      349 2023-10-19 16:11:13.000000 xradio-0.0.8/src/xradio/image/_util/_zarr/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     1697 2023-10-19 16:11:13.000000 xradio-0.0.8/src/xradio/image/_util/_zarr/xds_from_zarr.py
--rw-r--r--   0 runner    (1001) docker     (127)     1642 2023-10-19 16:11:13.000000 xradio-0.0.8/src/xradio/image/_util/_zarr/xds_to_zarr.py
--rw-r--r--   0 runner    (1001) docker     (127)     5452 2023-10-19 16:11:13.000000 xradio-0.0.8/src/xradio/image/_util/_zarr/zarr_low_level.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5805 2023-10-19 16:11:13.000000 xradio-0.0.8/src/xradio/image/_util/casacore.py
--rw-r--r--   0 runner    (1001) docker     (127)     3961 2023-10-19 16:11:13.000000 xradio-0.0.8/src/xradio/image/_util/common.py
--rw-r--r--   0 runner    (1001) docker     (127)      336 2023-10-19 16:11:13.000000 xradio-0.0.8/src/xradio/image/_util/fits.py
--rw-r--r--   0 runner    (1001) docker     (127)     5151 2023-10-19 16:11:13.000000 xradio-0.0.8/src/xradio/image/_util/image_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)      454 2023-10-19 16:11:13.000000 xradio-0.0.8/src/xradio/image/_util/zarr.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     8190 2023-10-19 16:11:13.000000 xradio-0.0.8/src/xradio/image/image.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-19 16:11:29.171403 xradio-0.0.8/src/xradio/vis/
--rw-r--r--   0 runner    (1001) docker     (127)      111 2023-10-19 16:11:13.000000 xradio-0.0.8/src/xradio/vis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      979 2023-10-19 16:11:13.000000 xradio-0.0.8/src/xradio/vis/_processing_set.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-19 16:11:29.171403 xradio-0.0.8/src/xradio/vis/_vis_utils/
--rw-r--r--   0 runner    (1001) docker     (127)       93 2023-10-19 16:11:13.000000 xradio-0.0.8/src/xradio/vis/_vis_utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-19 16:11:29.171403 xradio-0.0.8/src/xradio/vis/_vis_utils/_ms/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-19 16:11:29.175403 xradio-0.0.8/src/xradio/vis/_vis_utils/_ms/_tables/
--rw-r--r--   0 runner    (1001) docker     (127)     2403 2023-10-19 16:11:13.000000 xradio-0.0.8/src/xradio/vis/_vis_utils/_ms/_tables/load.py
--rw-r--r--   0 runner    (1001) docker     (127)    14397 2023-10-19 16:11:13.000000 xradio-0.0.8/src/xradio/vis/_vis_utils/_ms/_tables/load_main_table.py
--rw-r--r--   0 runner    (1001) docker     (127)    21230 2023-10-19 16:11:13.000000 xradio-0.0.8/src/xradio/vis/_vis_utils/_ms/_tables/read.py
--rw-r--r--   0 runner    (1001) docker     (127)    22526 2023-10-19 16:11:13.000000 xradio-0.0.8/src/xradio/vis/_vis_utils/_ms/_tables/read_main_table.py
--rw-r--r--   0 runner    (1001) docker     (127)    12394 2023-10-19 16:11:13.000000 xradio-0.0.8/src/xradio/vis/_vis_utils/_ms/_tables/read_subtables.py
--rw-r--r--   0 runner    (1001) docker     (127)     1293 2023-10-19 16:11:13.000000 xradio-0.0.8/src/xradio/vis/_vis_utils/_ms/_tables/table_query.py
--rw-r--r--   0 runner    (1001) docker     (127)     9192 2023-10-19 16:11:13.000000 xradio-0.0.8/src/xradio/vis/_vis_utils/_ms/_tables/write.py
--rw-r--r--   0 runner    (1001) docker     (127)    13932 2023-10-19 16:11:13.000000 xradio-0.0.8/src/xradio/vis/_vis_utils/_ms/_tables/write_exp_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     5592 2023-10-19 16:11:13.000000 xradio-0.0.8/src/xradio/vis/_vis_utils/_ms/chunks.py
--rw-r--r--   0 runner    (1001) docker     (127)     5222 2023-10-19 16:11:13.000000 xradio-0.0.8/src/xradio/vis/_vis_utils/_ms/descr.py
--rw-r--r--   0 runner    (1001) docker     (127)      855 2023-10-19 16:11:13.000000 xradio-0.0.8/src/xradio/vis/_vis_utils/_ms/msv2_msv3.py
--rw-r--r--   0 runner    (1001) docker     (127)    11161 2023-10-19 16:11:13.000000 xradio-0.0.8/src/xradio/vis/_vis_utils/_ms/partition_queries.py
--rw-r--r--   0 runner    (1001) docker     (127)    12717 2023-10-19 16:11:13.000000 xradio-0.0.8/src/xradio/vis/_vis_utils/_ms/partitions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4415 2023-10-19 16:11:13.000000 xradio-0.0.8/src/xradio/vis/_vis_utils/_ms/subtables.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-19 16:11:29.175403 xradio-0.0.8/src/xradio/vis/_vis_utils/_utils/
--rw-r--r--   0 runner    (1001) docker     (127)     1923 2023-10-19 16:11:13.000000 xradio-0.0.8/src/xradio/vis/_vis_utils/_utils/cds.py
--rw-r--r--   0 runner    (1001) docker     (127)     3945 2023-10-19 16:11:13.000000 xradio-0.0.8/src/xradio/vis/_vis_utils/_utils/partition_attrs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1305 2023-10-19 16:11:13.000000 xradio-0.0.8/src/xradio/vis/_vis_utils/_utils/stokes_types.py
--rw-r--r--   0 runner    (1001) docker     (127)    11853 2023-10-19 16:11:13.000000 xradio-0.0.8/src/xradio/vis/_vis_utils/_utils/xds_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-19 16:11:29.175403 xradio-0.0.8/src/xradio/vis/_vis_utils/_zarr/
--rw-r--r--   0 runner    (1001) docker     (127)     7834 2023-10-19 16:11:13.000000 xradio-0.0.8/src/xradio/vis/_vis_utils/_zarr/read.py
--rw-r--r--   0 runner    (1001) docker     (127)     9585 2023-10-19 16:11:13.000000 xradio-0.0.8/src/xradio/vis/_vis_utils/_zarr/write.py
--rw-r--r--   0 runner    (1001) docker     (127)     6108 2023-10-19 16:11:13.000000 xradio-0.0.8/src/xradio/vis/_vis_utils/ms.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    40644 2023-10-19 16:11:13.000000 xradio-0.0.8/src/xradio/vis/_vis_utils/ms_column_descriptions_dicts.py
--rw-r--r--   0 runner    (1001) docker     (127)     4264 2023-10-19 16:11:13.000000 xradio-0.0.8/src/xradio/vis/_vis_utils/zarr.py
--rw-r--r--   0 runner    (1001) docker     (127)    25526 2023-10-19 16:11:13.000000 xradio-0.0.8/src/xradio/vis/convert_msv2_to_processing_set.py
--rw-r--r--   0 runner    (1001) docker     (127)     4505 2023-10-19 16:11:13.000000 xradio-0.0.8/src/xradio/vis/load_processing_set.py
--rw-r--r--   0 runner    (1001) docker     (127)      688 2023-10-19 16:11:13.000000 xradio-0.0.8/src/xradio/vis/read_processing_set.py
--rw-r--r--   0 runner    (1001) docker     (127)     6022 2023-10-19 16:11:13.000000 xradio-0.0.8/src/xradio/vis/vis_io.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-19 16:11:29.163403 xradio-0.0.8/src/xradio.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3985 2023-10-19 16:11:29.000000 xradio-0.0.8/src/xradio.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2347 2023-10-19 16:11:29.000000 xradio-0.0.8/src/xradio.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-19 16:11:29.000000 xradio-0.0.8/src/xradio.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      362 2023-10-19 16:11:29.000000 xradio-0.0.8/src/xradio.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2023-10-19 16:11:29.000000 xradio-0.0.8/src/xradio.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-25 01:51:18.973810 xradio-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1516 2023-10-25 01:51:01.000000 xradio-0.0.9/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2023-10-25 01:51:01.000000 xradio-0.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3985 2023-10-25 01:51:18.973810 xradio-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      959 2023-10-25 01:51:01.000000 xradio-0.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      808 2023-10-25 01:51:01.000000 xradio-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-25 01:51:18.973810 xradio-0.0.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-25 01:51:18.961810 xradio-0.0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-25 01:51:18.965810 xradio-0.0.9/src/xradio/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-25 01:51:01.000000 xradio-0.0.9/src/xradio/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-25 01:51:18.965810 xradio-0.0.9/src/xradio/_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-25 01:51:01.000000 xradio-0.0.9/src/xradio/_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-25 01:51:18.965810 xradio-0.0.9/src/xradio/data/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-25 01:51:01.000000 xradio-0.0.9/src/xradio/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2288 2023-10-25 01:51:01.000000 xradio-0.0.9/src/xradio/data/_dropbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4340 2023-10-25 01:51:01.000000 xradio-0.0.9/src/xradio/data/_google_drive.py
+-rw-r--r--   0 runner    (1001) docker     (127)      457 2023-10-25 01:51:01.000000 xradio-0.0.9/src/xradio/data/datasets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-25 01:51:18.965810 xradio-0.0.9/src/xradio/image/
+-rw-r--r--   0 runner    (1001) docker     (127)      291 2023-10-25 01:51:01.000000 xradio-0.0.9/src/xradio/image/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-25 01:51:18.969810 xradio-0.0.9/src/xradio/image/_util/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-25 01:51:18.969810 xradio-0.0.9/src/xradio/image/_util/_casacore/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2023-10-25 01:51:01.000000 xradio-0.0.9/src/xradio/image/_util/_casacore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2023-10-25 01:51:01.000000 xradio-0.0.9/src/xradio/image/_util/_casacore/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39144 2023-10-25 01:51:01.000000 xradio-0.0.9/src/xradio/image/_util/_casacore/xds_from_casacore.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13918 2023-10-25 01:51:01.000000 xradio-0.0.9/src/xradio/image/_util/_casacore/xds_to_casacore.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-25 01:51:18.969810 xradio-0.0.9/src/xradio/image/_util/_fits/
+-rw-r--r--   0 runner    (1001) docker     (127)    26637 2023-10-25 01:51:01.000000 xradio-0.0.9/src/xradio/image/_util/_fits/xds_from_fits.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-25 01:51:18.969810 xradio-0.0.9/src/xradio/image/_util/_zarr/
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2023-10-25 01:51:01.000000 xradio-0.0.9/src/xradio/image/_util/_zarr/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1697 2023-10-25 01:51:01.000000 xradio-0.0.9/src/xradio/image/_util/_zarr/xds_from_zarr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1642 2023-10-25 01:51:01.000000 xradio-0.0.9/src/xradio/image/_util/_zarr/xds_to_zarr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6250 2023-10-25 01:51:01.000000 xradio-0.0.9/src/xradio/image/_util/_zarr/zarr_low_level.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5805 2023-10-25 01:51:01.000000 xradio-0.0.9/src/xradio/image/_util/casacore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3961 2023-10-25 01:51:01.000000 xradio-0.0.9/src/xradio/image/_util/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2023-10-25 01:51:01.000000 xradio-0.0.9/src/xradio/image/_util/fits.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5150 2023-10-25 01:51:01.000000 xradio-0.0.9/src/xradio/image/_util/image_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2023-10-25 01:51:01.000000 xradio-0.0.9/src/xradio/image/_util/zarr.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8190 2023-10-25 01:51:01.000000 xradio-0.0.9/src/xradio/image/image.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-25 01:51:18.969810 xradio-0.0.9/src/xradio/vis/
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2023-10-25 01:51:01.000000 xradio-0.0.9/src/xradio/vis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      979 2023-10-25 01:51:01.000000 xradio-0.0.9/src/xradio/vis/_processing_set.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-25 01:51:18.969810 xradio-0.0.9/src/xradio/vis/_vis_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2023-10-25 01:51:01.000000 xradio-0.0.9/src/xradio/vis/_vis_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-25 01:51:18.969810 xradio-0.0.9/src/xradio/vis/_vis_utils/_ms/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-25 01:51:18.973810 xradio-0.0.9/src/xradio/vis/_vis_utils/_ms/_tables/
+-rw-r--r--   0 runner    (1001) docker     (127)     2403 2023-10-25 01:51:01.000000 xradio-0.0.9/src/xradio/vis/_vis_utils/_ms/_tables/load.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14397 2023-10-25 01:51:01.000000 xradio-0.0.9/src/xradio/vis/_vis_utils/_ms/_tables/load_main_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20486 2023-10-25 01:51:01.000000 xradio-0.0.9/src/xradio/vis/_vis_utils/_ms/_tables/read.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22526 2023-10-25 01:51:01.000000 xradio-0.0.9/src/xradio/vis/_vis_utils/_ms/_tables/read_main_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12394 2023-10-25 01:51:01.000000 xradio-0.0.9/src/xradio/vis/_vis_utils/_ms/_tables/read_subtables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1293 2023-10-25 01:51:01.000000 xradio-0.0.9/src/xradio/vis/_vis_utils/_ms/_tables/table_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9192 2023-10-25 01:51:01.000000 xradio-0.0.9/src/xradio/vis/_vis_utils/_ms/_tables/write.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13932 2023-10-25 01:51:01.000000 xradio-0.0.9/src/xradio/vis/_vis_utils/_ms/_tables/write_exp_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5592 2023-10-25 01:51:01.000000 xradio-0.0.9/src/xradio/vis/_vis_utils/_ms/chunks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5222 2023-10-25 01:51:01.000000 xradio-0.0.9/src/xradio/vis/_vis_utils/_ms/descr.py
+-rw-r--r--   0 runner    (1001) docker     (127)      855 2023-10-25 01:51:01.000000 xradio-0.0.9/src/xradio/vis/_vis_utils/_ms/msv2_msv3.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11161 2023-10-25 01:51:01.000000 xradio-0.0.9/src/xradio/vis/_vis_utils/_ms/partition_queries.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12717 2023-10-25 01:51:01.000000 xradio-0.0.9/src/xradio/vis/_vis_utils/_ms/partitions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4415 2023-10-25 01:51:01.000000 xradio-0.0.9/src/xradio/vis/_vis_utils/_ms/subtables.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-25 01:51:18.973810 xradio-0.0.9/src/xradio/vis/_vis_utils/_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     1923 2023-10-25 01:51:01.000000 xradio-0.0.9/src/xradio/vis/_vis_utils/_utils/cds.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3945 2023-10-25 01:51:01.000000 xradio-0.0.9/src/xradio/vis/_vis_utils/_utils/partition_attrs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1305 2023-10-25 01:51:01.000000 xradio-0.0.9/src/xradio/vis/_vis_utils/_utils/stokes_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11853 2023-10-25 01:51:01.000000 xradio-0.0.9/src/xradio/vis/_vis_utils/_utils/xds_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-25 01:51:18.973810 xradio-0.0.9/src/xradio/vis/_vis_utils/_zarr/
+-rw-r--r--   0 runner    (1001) docker     (127)     7834 2023-10-25 01:51:01.000000 xradio-0.0.9/src/xradio/vis/_vis_utils/_zarr/read.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9585 2023-10-25 01:51:01.000000 xradio-0.0.9/src/xradio/vis/_vis_utils/_zarr/write.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6108 2023-10-25 01:51:01.000000 xradio-0.0.9/src/xradio/vis/_vis_utils/ms.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    40644 2023-10-25 01:51:01.000000 xradio-0.0.9/src/xradio/vis/_vis_utils/ms_column_descriptions_dicts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3520 2023-10-25 01:51:01.000000 xradio-0.0.9/src/xradio/vis/_vis_utils/zarr.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25775 2023-10-25 01:51:01.000000 xradio-0.0.9/src/xradio/vis/convert_msv2_to_processing_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4500 2023-10-25 01:51:01.000000 xradio-0.0.9/src/xradio/vis/load_processing_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)      688 2023-10-25 01:51:01.000000 xradio-0.0.9/src/xradio/vis/read_processing_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6022 2023-10-25 01:51:01.000000 xradio-0.0.9/src/xradio/vis/vis_io.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-25 01:51:18.965810 xradio-0.0.9/src/xradio.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3985 2023-10-25 01:51:18.000000 xradio-0.0.9/src/xradio.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2347 2023-10-25 01:51:18.000000 xradio-0.0.9/src/xradio.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-25 01:51:18.000000 xradio-0.0.9/src/xradio.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2023-10-25 01:51:18.000000 xradio-0.0.9/src/xradio.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2023-10-25 01:51:18.000000 xradio-0.0.9/src/xradio.egg-info/top_level.txt
```

### Comparing `xradio-0.0.8/LICENSE.txt` & `xradio-0.0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `xradio-0.0.8/PKG-INFO` & `xradio-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xradio
-Version: 0.0.8
+Version: 0.0.9
 Summary: Xarray Radio Astronomy Data IO
 Author-email: Jan-Willem Steeb <jsteeb@nrao.edu>
 License: BSD 3-Clause License
         
         Copyright (c) 2023, Associated Universities, Inc.
         
         Redistribution and use in source and binary forms, with or without
```

### Comparing `xradio-0.0.8/README.md` & `xradio-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `xradio-0.0.8/pyproject.toml` & `xradio-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "xradio"
-version = "0.0.8"
+version = "0.0.9"
 description = "Xarray Radio Astronomy Data IO"
 authors = [
     {name = "Jan-Willem Steeb", email="jsteeb@nrao.edu"},
 ]
 license = {file = "LICENSE.txt"}
 readme = "README.md"
 requires-python = ">= 3.8, < 3.12"
```

### Comparing `xradio-0.0.8/src/xradio/data/_dropbox.py` & `xradio-0.0.9/src/xradio/data/_dropbox.py`

 * *Files identical despite different names*

### Comparing `xradio-0.0.8/src/xradio/data/_google_drive.py` & `xradio-0.0.9/src/xradio/data/_google_drive.py`

 * *Files identical despite different names*

### Comparing `xradio-0.0.8/src/xradio/image/_util/_casacore/xds_from_casacore.py` & `xradio-0.0.9/src/xradio/image/_util/_casacore/xds_from_casacore.py`

 * *Files identical despite different names*

### Comparing `xradio-0.0.8/src/xradio/image/_util/_casacore/xds_to_casacore.py` & `xradio-0.0.9/src/xradio/image/_util/_casacore/xds_to_casacore.py`

 * *Files identical despite different names*

### Comparing `xradio-0.0.8/src/xradio/image/_util/_fits/xds_from_fits.py` & `xradio-0.0.9/src/xradio/image/_util/_fits/xds_from_fits.py`

 * *Files identical despite different names*

### Comparing `xradio-0.0.8/src/xradio/image/_util/_zarr/xds_from_zarr.py` & `xradio-0.0.9/src/xradio/image/_util/_zarr/xds_from_zarr.py`

 * *Files identical despite different names*

### Comparing `xradio-0.0.8/src/xradio/image/_util/_zarr/xds_to_zarr.py` & `xradio-0.0.9/src/xradio/image/_util/_zarr/xds_to_zarr.py`

 * *Files identical despite different names*

### Comparing `xradio-0.0.8/src/xradio/image/_util/_zarr/zarr_low_level.py` & `xradio-0.0.9/src/xradio/image/_util/_zarr/zarr_low_level.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from numcodecs.compat import (
     ensure_text,
     ensure_ndarray_like,
     ensure_bytes,
     ensure_contiguous_ndarray_like
 )
 
-def pad_array_with_nans(input_array, output_shape):
+def pad_array_with_nans(input_array, output_shape, dtype):
     """
     Pad an integer array with NaN values to match the specified output shape.
 
     Parameters:
     - input_array: The input NumPy array to be padded.
     - output_shape: A tuple specifying the desired output shape (e.g., (rows, columns)).
 
@@ -23,15 +23,15 @@
     # Get the input shape
     input_shape = input_array.shape
 
     # Calculate the padding dimensions
     padding_shape = tuple(max(0, o - i) for i, o in zip(input_shape, output_shape))
 
     # Create a new array filled with NaN values
-    padded_array = np.empty(output_shape)
+    padded_array = np.empty(output_shape,dtype=dtype)
     padded_array[:] = np.nan
 
     # Copy the input array to the appropriate position within the padded array
     padded_array[:input_shape[0], :input_shape[1]] = input_array
 
     return padded_array
 
@@ -44,24 +44,24 @@
     - file_path: The path to the output file where the compressed array will be saved.
     - compressor:
 
     Returns:
     - None
     """
     # Encode the NumPy array using the codec
-    compressed_arr = compressor.encode(arr)
+    compressed_arr = compressor.encode(np.ascontiguousarray(arr))
 
     # Ensure the directory exists before saving the file
     os.makedirs(os.path.dirname(file_path), exist_ok=True)
 
     # Save the compressed array to disk
     with open(file_path, 'wb') as file:
         file.write(compressed_arr)
 
-    print(f"Compressed array saved to {file_path}")
+    #print(f"Compressed array saved to {file_path}")
     
 def read_binary_blob_from_disk(file_path, compressor, dtype=np.float64):
     """
     Read a compressed binary blob from disk and decode it using Blosc.
 
     Parameters:
     - file_path: The path to the compressed binary blob file.
@@ -131,55 +131,69 @@
     Returns:
     - None
     """
     with open(file_path, 'w') as file:
         json.dump(data, file, indent=4,sort_keys=True, ensure_ascii=True, separators=(",", ": "), cls=NumberEncoder)
 
 
-def create_data_variable_meta_data_on_disk(zarr_group_name,data_varaibles_and_dims,compressor):
-
-    for data_varaible, dims in data_varaibles_and_dims.items():
-        print(data_varaible,dims)
-        data_variable_path = os.path.join(zarr_group_name,data_varaible)
+def create_data_variable_meta_data_on_disk(zarr_group_name,data_variables_and_dims,xds_dims,parallel_coords,compressor):
+    zarr_meta = data_variables_and_dims
+    
+    for data_variable_key, dims_dtype_name in data_variables_and_dims.items():
+        #print(data_variable_key, dims_dtype_name)
+    
+        dims=dims_dtype_name['dims']
+        dtype=dims_dtype_name['dtype']
+        data_variable_name = dims_dtype_name['name']
+        data_variable_path = os.path.join(zarr_group_name,data_variable_name)
         os.system('mkdir ' + data_variable_path)
         #Create .zattrs
         zattrs = {
             "_ARRAY_DIMENSIONS": dims,
             #"coordinates": "time declination right_ascension"
         }
-    
+        
+        shape=[]
+        chunks=[]
+        for d in dims:
+            shape.append(xds_dims[d])
+            if d in parallel_coords:
+                chunks.append(len(parallel_coords[d]['data_chunks'][0]))
+            else:
+                chunks.append(xds_dims[d])
+        
+        #print(chunks,shape)
         write_json_file(zattrs,os.path.join(data_variable_path,'.zattrs'))
         
         #Create .zarray
         from zarr import n5
         compressor_config = n5.compressor_config_to_zarr(n5.compressor_config_to_n5(compressor.get_config()))
-        zarray = {
-            "chunks": [
-                1,
-                1,
-                2,
-                500,
-                500
-            ],
-            "compressor":compressor_config,
-            "dtype": "<f8",
-            "fill_value": "NaN",
-            "filters": None,
-            "order": "C",
-            "shape": [
-                1,
-                1,
-                3,
-                500,
-                500
-            ],
-            "zarr_format": 2
-        }
-
-        write_json_file(zarray,os.path.join(data_variable_path,'.zarray'))
         
+        if "f" in dtype:
+            zarray = {
+                "chunks": chunks,
+                "compressor":compressor_config,
+                "dtype": dtype,
+                "fill_value": "NaN",
+                "filters": None,
+                "order": "C",
+                "shape": shape,
+                "zarr_format": 2
+            }
+        
+        else:
+            zarray = {
+                "chunks": chunks,
+                "compressor":compressor_config,
+                "dtype": dtype,
+                "fill_value": None,
+                "filters": None,
+                "order": "C",
+                "shape": shape,
+                "zarr_format": 2
+            }
         
-        
-##Image definitions
-# parallel_coords
-# img_xds (get image size and chunk size)
-# SKY, dims, dtype
+        zarr_meta[data_variable_key]['chunks']=chunks
+        zarr_meta[data_variable_key]['shape']=shape
+
+        write_json_file(zarray,os.path.join(data_variable_path,'.zarray'))
+    return zarr_meta
```

### Comparing `xradio-0.0.8/src/xradio/image/_util/casacore.py` & `xradio-0.0.9/src/xradio/image/_util/casacore.py`

 * *Files identical despite different names*

### Comparing `xradio-0.0.8/src/xradio/image/_util/common.py` & `xradio-0.0.9/src/xradio/image/_util/common.py`

 * *Files identical despite different names*

### Comparing `xradio-0.0.8/src/xradio/image/_util/image_factory.py` & `xradio-0.0.9/src/xradio/image/_util/image_factory.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,15 @@
     x, y = np.indices(w.pixel_shape)
     long, lat = w.pixel_to_world_values(x, y)
     # long, lat from above eqn will always be in degrees, so convert to rad
     f = np.pi/180
     long *= f
     lat *= f
     if not isinstance(chan_coords, list) and not isinstance(chan_coords, np.ndarray):
-        chan_coords = [ chane_coords ]
+        chan_coords = [ chan_coords ]
     chan_coords = np.array(chan_coords, dtype=np.float64)
     restfreq = chan_coords[len(chan_coords)//2]
     vel = (1 - chan_coords/restfreq) * __c
     if not isinstance(time_coords, list) and not isinstance(time_coords, np.ndarray):
         time_coords = [ time_coords ]
     time_coords = np.array(time_coords, dtype=np.float64)
     coords = {
```

### Comparing `xradio-0.0.8/src/xradio/image/image.py` & `xradio-0.0.9/src/xradio/image/image.py`

 * *Files identical despite different names*

### Comparing `xradio-0.0.8/src/xradio/vis/_processing_set.py` & `xradio-0.0.9/src/xradio/vis/_processing_set.py`

 * *Files identical despite different names*

### Comparing `xradio-0.0.8/src/xradio/vis/_vis_utils/_ms/_tables/load.py` & `xradio-0.0.9/src/xradio/vis/_vis_utils/_ms/_tables/load.py`

 * *Files identical despite different names*

### Comparing `xradio-0.0.8/src/xradio/vis/_vis_utils/_ms/_tables/load_main_table.py` & `xradio-0.0.9/src/xradio/vis/_vis_utils/_ms/_tables/load_main_table.py`

 * *Files identical despite different names*

### Comparing `xradio-0.0.8/src/xradio/vis/_vis_utils/_ms/_tables/read.py` & `xradio-0.0.9/src/xradio/vis/_vis_utils/_ms/_tables/read.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,7 @@
-#  CASA Next Generation Infrastructure
-#  Copyright (C) 2021, 2023 AUI, Inc. Washington DC, USA
-#
-#  This program is free software: you can redistribute it and/or modify
-#  it under the terms of the GNU General Public License as published by
-#  the Free Software Foundation, either version 3 of the License, or
-#  (at your option) any later version.
-#
-#  This program is distributed in the hope that it will be useful,
-#  but WITHOUT ANY WARRANTY; without even the implied warranty of
-#  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-#  GNU General Public License for more details.
-#
-#  You should have received a copy of the GNU General Public License
-#  along with this program.  If not, see <https://www.gnu.org/licenses/>.
-
 import logging, os
 from pathlib import Path
 import re
 from typing import Any, List, Dict, Tuple, Union
 
 import numpy as np
 import pandas as pd
```

### Comparing `xradio-0.0.8/src/xradio/vis/_vis_utils/_ms/_tables/read_main_table.py` & `xradio-0.0.9/src/xradio/vis/_vis_utils/_ms/_tables/read_main_table.py`

 * *Files identical despite different names*

### Comparing `xradio-0.0.8/src/xradio/vis/_vis_utils/_ms/_tables/read_subtables.py` & `xradio-0.0.9/src/xradio/vis/_vis_utils/_ms/_tables/read_subtables.py`

 * *Files identical despite different names*

### Comparing `xradio-0.0.8/src/xradio/vis/_vis_utils/_ms/_tables/table_query.py` & `xradio-0.0.9/src/xradio/vis/_vis_utils/_ms/_tables/table_query.py`

 * *Files identical despite different names*

### Comparing `xradio-0.0.8/src/xradio/vis/_vis_utils/_ms/_tables/write.py` & `xradio-0.0.9/src/xradio/vis/_vis_utils/_ms/_tables/write.py`

 * *Files identical despite different names*

### Comparing `xradio-0.0.8/src/xradio/vis/_vis_utils/_ms/_tables/write_exp_api.py` & `xradio-0.0.9/src/xradio/vis/_vis_utils/_ms/_tables/write_exp_api.py`

 * *Files identical despite different names*

### Comparing `xradio-0.0.8/src/xradio/vis/_vis_utils/_ms/chunks.py` & `xradio-0.0.9/src/xradio/vis/_vis_utils/_ms/chunks.py`

 * *Files identical despite different names*

### Comparing `xradio-0.0.8/src/xradio/vis/_vis_utils/_ms/descr.py` & `xradio-0.0.9/src/xradio/vis/_vis_utils/_ms/descr.py`

 * *Files identical despite different names*

### Comparing `xradio-0.0.8/src/xradio/vis/_vis_utils/_ms/msv2_msv3.py` & `xradio-0.0.9/src/xradio/vis/_vis_utils/_ms/msv2_msv3.py`

 * *Files identical despite different names*

### Comparing `xradio-0.0.8/src/xradio/vis/_vis_utils/_ms/partition_queries.py` & `xradio-0.0.9/src/xradio/vis/_vis_utils/_ms/partition_queries.py`

 * *Files identical despite different names*

### Comparing `xradio-0.0.8/src/xradio/vis/_vis_utils/_ms/partitions.py` & `xradio-0.0.9/src/xradio/vis/_vis_utils/_ms/partitions.py`

 * *Files identical despite different names*

### Comparing `xradio-0.0.8/src/xradio/vis/_vis_utils/_ms/subtables.py` & `xradio-0.0.9/src/xradio/vis/_vis_utils/_ms/subtables.py`

 * *Files identical despite different names*

### Comparing `xradio-0.0.8/src/xradio/vis/_vis_utils/_utils/cds.py` & `xradio-0.0.9/src/xradio/vis/_vis_utils/_utils/cds.py`

 * *Files identical despite different names*

### Comparing `xradio-0.0.8/src/xradio/vis/_vis_utils/_utils/partition_attrs.py` & `xradio-0.0.9/src/xradio/vis/_vis_utils/_utils/partition_attrs.py`

 * *Files identical despite different names*

### Comparing `xradio-0.0.8/src/xradio/vis/_vis_utils/_utils/stokes_types.py` & `xradio-0.0.9/src/xradio/vis/_vis_utils/_utils/stokes_types.py`

 * *Files identical despite different names*

### Comparing `xradio-0.0.8/src/xradio/vis/_vis_utils/_utils/xds_helper.py` & `xradio-0.0.9/src/xradio/vis/_vis_utils/_utils/xds_helper.py`

 * *Files identical despite different names*

### Comparing `xradio-0.0.8/src/xradio/vis/_vis_utils/_zarr/read.py` & `xradio-0.0.9/src/xradio/vis/_vis_utils/_zarr/read.py`

 * *Files identical despite different names*

### Comparing `xradio-0.0.8/src/xradio/vis/_vis_utils/_zarr/write.py` & `xradio-0.0.9/src/xradio/vis/_vis_utils/_zarr/write.py`

 * *Files identical despite different names*

### Comparing `xradio-0.0.8/src/xradio/vis/_vis_utils/ms.py` & `xradio-0.0.9/src/xradio/vis/_vis_utils/ms.py`

 * *Files identical despite different names*

### Comparing `xradio-0.0.8/src/xradio/vis/_vis_utils/ms_column_descriptions_dicts.py` & `xradio-0.0.9/src/xradio/vis/_vis_utils/ms_column_descriptions_dicts.py`

 * *Files identical despite different names*

### Comparing `xradio-0.0.8/src/xradio/vis/_vis_utils/zarr.py` & `xradio-0.0.9/src/xradio/vis/_vis_utils/zarr.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,23 +1,7 @@
-#  CASA Next Generation Infrastructure
-#  Copyright (C) 2021, 2023 AUI, Inc. Washington DC, USA
-#
-#  This program is free software: you can redistribute it and/or modify
-#  it under the terms of the GNU General Public License as published by
-#  the Free Software Foundation, either version 3 of the License, or
-#  (at your option) any later version.
-#
-#  This program is distributed in the hope that it will be useful,
-#  but WITHOUT ANY WARRANTY; without even the implied warranty of
-#  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-#  GNU General Public License for more details.
-#
-#  You should have received a copy of the GNU General Public License
-#  along with this program.  If not, see <https://www.gnu.org/licenses/>.
-
 import logging, numcodecs, os, time
 from pathlib import Path
 from typing import Dict, Union
 
 import zarr
 import xradio
```

### Comparing `xradio-0.0.8/src/xradio/vis/convert_msv2_to_processing_set.py` & `xradio-0.0.9/src/xradio/vis/convert_msv2_to_processing_set.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,15 +75,15 @@
     casacore_column_description, ref_code=None, time_format="unix"
 ):
     msv4_measure = {}
     if "MEASINFO" in casacore_column_description["keywords"]:
         msv4_measure["type"] = casacore_to_msv4_measure_type[
             casacore_column_description["keywords"]["MEASINFO"]["type"]
         ]["type"]
-        msv4_measure["units"] = casacore_column_description["keywords"]["QuantumUnits"]
+        msv4_measure["units"] = list(casacore_column_description["keywords"]["QuantumUnits"])
 
         if "TabRefCodes" in casacore_column_description["keywords"]["MEASINFO"]:
             ref_index = np.where(
                 casacore_column_description["keywords"]["MEASINFO"]["TabRefCodes"]
                 == ref_code
             )[0][0]
             casa_ref = casacore_column_description["keywords"]["MEASINFO"][
@@ -497,18 +497,18 @@
 
             ant_xds = create_ant_xds(infile)
 
             xds.attrs["intent"] = intent
             xds.attrs["ddi"] = ddi
 
             # Time and frequency should always be increasing
-            if xds.frequency[1] - xds.frequency[0] < 0:
+            if len(xds.frequency) > 1 and xds.frequency[1] - xds.frequency[0] < 0:
                 xds = xds.sel(frequency=slice(None, None, -1))
 
-            if xds.time[1] - xds.time[0] < 0:
+            if len(xds.time) > 1 and xds.time[1] - xds.time[0] < 0:
                 xds = xds.sel(time=slice(None, None, -1))
 
             if storage_backend == "zarr":
                 xds.to_zarr(store=file_name + "/MAIN", mode=mode)
                 ant_xds.to_zarr(store=file_name + "/ANTENNA", mode=mode)
             elif storage_backend == "netcdf":
                 # xds.to_netcdf(path=file_name+"/MAIN", mode=mode) #Does not work
@@ -574,52 +574,55 @@
 
 
 def create_field_info(xds, infile, field_id):
     field_xds = read_generic_table(
         infile,
         "FIELD",
         rename_ids=subt_rename_ids["FIELD"],
-    )
+    ).sel(field_id=field_id)
     # https://stackoverflow.com/questions/53195684/how-to-navigate-a-dict-by-list-of-keys
 
     field_column_description = field_xds.attrs["other"]["msv2"]["ctds_attrs"][
         "column_descriptions"
     ]
     # ['DELAY_DIR', 'PHASE_DIR', 'REFERENCE_DIR', 'CODE', 'FLAG_ROW', 'NAME', 'NUM_POLY', 'SOURCE_ID', 'TIME']
 
     msv4_measure = column_description_casacore_to_msv4_measure(
-        field_column_description["REFERENCE_DIR"]
+        field_column_description["REFERENCE_DIR"],
+        ref_code=getattr(field_xds.get("refdir_ref"), "data", None)
     )
     delay_dir = {
         "dims": "",
-        "data": list(field_xds["delay_dir"].data[field_id, 0, :]),
+        "data": list(field_xds["delay_dir"].data[0, :]),
         "attrs": msv4_measure,
     }
 
     msv4_measure = column_description_casacore_to_msv4_measure(
-        field_column_description["PHASE_DIR"]
+        field_column_description["PHASE_DIR"],
+        ref_code=getattr(field_xds.get("phasedir_ref"), "data", None)
     )
     phase_dir = {
         "dims": "",
-        "data": list(field_xds["phase_dir"].data[field_id, 0, :]),
+        "data": list(field_xds["phase_dir"].data[0, :]),
         "attrs": msv4_measure,
     }
 
     msv4_measure = column_description_casacore_to_msv4_measure(
-        field_column_description["DELAY_DIR"]
+        field_column_description["DELAY_DIR"],
+        ref_code=getattr(field_xds.get("delaydir_ref"), "data", None)
     )
     reference_dir = {
         "dims": "",
-        "data": list(field_xds["delay_dir"].data[field_id, 0, :]),
+        "data": list(field_xds["delay_dir"].data[0, :]),
         "attrs": msv4_measure,
     }
 
     field_info = {
-        "name": field_xds["name"].data[field_id],
-        "code": field_xds["code"].data[field_id],
+        "name": str(field_xds["name"].data),
+        "code": str(field_xds["code"].data),
         "delay_direction": delay_dir,
         "phase_direction": phase_dir,
         "reference_direction": reference_dir,
         "field_id": field_id,
     }
     xds.attrs["field_info"] = field_info
```

### Comparing `xradio-0.0.8/src/xradio/vis/load_processing_set.py` & `xradio-0.0.9/src/xradio/vis/load_processing_set.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,44 +1,44 @@
 import xarray as xr
 import zarr
 import copy
 import os
 from ._processing_set import _processing_set
 
 DIMENSION_KEY = "_ARRAY_DIMENSIONS"  # Used by xarray to store array labeling info in zarr meta data.
-# from xradio._utils._logger import _get_logger
+#from xradio._utils._logger import _get_logger
 
 
 def _get_attrs(zarr_obj):
     """
     get attributes of zarr obj (groups or arrays)
     """
     return {k: v for k, v in zarr_obj.attrs.asdict().items() if not k.startswith("_NC")}
 
 
 def _load_ms_xds(
     ps_name, ms_xds_name, slice_dict={}, cache_dir=None, chunk_id=None, date_time=""
 ):
-    # logger = _get_logger()
+    #logger = _get_logger()
     if cache_dir:
         xds_cached_name = (
             os.path.join(cache_dir, ms_xds_name) + "_" + str(chunk_id) + "_" + date_time
         )
 
         # Check if already chached:
         try:
             ms_xds = _load_ms_xds_core(
                 ms_xds_name=xds_cached_name, slice_dict=slice_dict
             )
 
-            # logger.debug(ms_xds_name + ' chunk ' + str(slice_dict) + ' was found in cache: ' + xds_cached)
+            #logger.debug(ms_xds_name + ' chunk ' + str(slice_dict) + ' was found in cache: ' + xds_cached)
             found_in_cache = True
             return xds, found_in_cache
         except:
-            # logger.debug(xds_cached + ' chunk ' + str(slice_dict) + ' was not found in cache or failed to load. Retrieving chunk from ' + ms_xds_name + ' .')
+            #logger.debug(xds_cached + ' chunk ' + str(slice_dict) + ' was not found in cache or failed to load. Retrieving chunk from ' + ms_xds_name + ' .')
             ms_xds = _load_ms_xds_core(
                 ms_xds_name=os.path.join(ps_name, ms_xds_name), slice_dict=slice_dict
             )
             write_ms_xds(ms_xds, xds_cached_name)
 
             found_in_cache = False
             return xds, found_in_cache
@@ -83,15 +83,15 @@
                 If a dim is not specified all values are retruned.
     return:
         xarray.Dataset()
 
     #Should go into general utils.
     """
 
-    # logger = _get_logger()
+    #logger = _get_logger()
     zarr_group = zarr.open_group(store=zarr_name, mode="r")
     group_attrs = _get_attrs(zarr_group)
 
     slice_dict_complete = copy.deepcopy(slice_dict)
     coords = {}
     xds = xr.Dataset()
     for var_name, var in zarr_group.arrays():
```

### Comparing `xradio-0.0.8/src/xradio/vis/read_processing_set.py` & `xradio-0.0.9/src/xradio/vis/read_processing_set.py`

 * *Files identical despite different names*

### Comparing `xradio-0.0.8/src/xradio/vis/vis_io.py` & `xradio-0.0.9/src/xradio/vis/vis_io.py`

 * *Files identical despite different names*

### Comparing `xradio-0.0.8/src/xradio.egg-info/PKG-INFO` & `xradio-0.0.9/src/xradio.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xradio
-Version: 0.0.8
+Version: 0.0.9
 Summary: Xarray Radio Astronomy Data IO
 Author-email: Jan-Willem Steeb <jsteeb@nrao.edu>
 License: BSD 3-Clause License
         
         Copyright (c) 2023, Associated Universities, Inc.
         
         Redistribution and use in source and binary forms, with or without
```

### Comparing `xradio-0.0.8/src/xradio.egg-info/SOURCES.txt` & `xradio-0.0.9/src/xradio.egg-info/SOURCES.txt`

 * *Files identical despite different names*

