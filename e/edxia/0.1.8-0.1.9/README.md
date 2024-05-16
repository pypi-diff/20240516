# Comparing `tmp/edxia-0.1.8.tar.gz` & `tmp/edxia-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/edxia-0.1.8.tar", last modified: Wed Dec 16 08:59:52 2020, max compression
+gzip compressed data, was "edxia-0.1.9.tar", last modified: Thu May 27 15:57:10 2021, max compression
```

## Comparing `edxia-0.1.8.tar` & `edxia-0.1.9.tar`

### file list

```diff
@@ -1,80 +1,80 @@
-drwxrwxr-x   0 manawy    (1000) manawy    (1000)        0 2020-12-16 08:59:52.000000 edxia-0.1.8/
--rw-rw-r--   0 manawy    (1000) manawy    (1000)     2662 2020-12-16 08:59:52.000000 edxia-0.1.8/PKG-INFO
--rw-rw-r--   0 manawy    (1000) manawy    (1000)     1563 2020-01-19 15:48:08.000000 edxia-0.1.8/README.md
-drwxrwxr-x   0 manawy    (1000) manawy    (1000)        0 2020-12-16 08:59:52.000000 edxia-0.1.8/edxia/
--rw-rw-r--   0 manawy    (1000) manawy    (1000)     2253 2020-08-12 12:58:23.000000 edxia-0.1.8/edxia/__init__.py
-drwxrwxr-x   0 manawy    (1000) manawy    (1000)        0 2020-12-16 08:59:52.000000 edxia-0.1.8/edxia/analysis/
--rw-rw-r--   0 manawy    (1000) manawy    (1000)     1629 2019-12-26 04:10:16.000000 edxia-0.1.8/edxia/analysis/__init__.py
--rw-rw-r--   0 manawy    (1000) manawy    (1000)     4139 2020-01-09 08:10:41.000000 edxia-0.1.8/edxia/analysis/correlation.py
--rw-rw-r--   0 manawy    (1000) manawy    (1000)     2316 2020-02-24 20:52:57.000000 edxia-0.1.8/edxia/analysis/helpers.py
--rw-rw-r--   0 manawy    (1000) manawy    (1000)     5268 2020-01-04 04:47:55.000000 edxia-0.1.8/edxia/analysis/point_counting.py
-drwxrwxr-x   0 manawy    (1000) manawy    (1000)        0 2020-12-16 08:59:52.000000 edxia-0.1.8/edxia/composite/
--rw-rw-r--   0 manawy    (1000) manawy    (1000)     1750 2019-10-19 14:16:09.000000 edxia-0.1.8/edxia/composite/__init__.py
--rw-rw-r--   0 manawy    (1000) manawy    (1000)     3477 2019-10-13 14:49:34.000000 edxia-0.1.8/edxia/composite/channels.py
--rwxrwxr-x   0 manawy    (1000) manawy    (1000)     2311 2020-05-19 08:35:46.000000 edxia-0.1.8/edxia/composite/color_analysis.py
--rw-rw-r--   0 manawy    (1000) manawy    (1000)     2668 2020-05-18 18:26:21.000000 edxia-0.1.8/edxia/composite/composite.py
--rw-rw-r--   0 manawy    (1000) manawy    (1000)     4588 2020-05-18 09:53:31.000000 edxia-0.1.8/edxia/composite/segmentation.py
-drwxrwxr-x   0 manawy    (1000) manawy    (1000)        0 2020-12-16 08:59:52.000000 edxia-0.1.8/edxia/core/
--rw-rw-r--   0 manawy    (1000) manawy    (1000)     1770 2019-12-23 09:28:42.000000 edxia-0.1.8/edxia/core/__init__.py
--rw-rw-r--   0 manawy    (1000) manawy    (1000)     7486 2020-01-29 12:35:06.000000 edxia-0.1.8/edxia/core/experiment.py
--rw-rw-r--   0 manawy    (1000) manawy    (1000)     6859 2019-10-13 14:49:34.000000 edxia-0.1.8/edxia/core/map.py
-drwxrwxr-x   0 manawy    (1000) manawy    (1000)        0 2020-12-16 08:59:52.000000 edxia-0.1.8/edxia/filters/
--rw-rw-r--   0 manawy    (1000) manawy    (1000)     1566 2019-04-22 12:50:11.000000 edxia-0.1.8/edxia/filters/__init__.py
--rw-rw-r--   0 manawy    (1000) manawy    (1000)     2270 2019-10-13 14:49:34.000000 edxia-0.1.8/edxia/filters/base_filter.py
--rw-rw-r--   0 manawy    (1000) manawy    (1000)     3117 2020-01-07 01:10:10.000000 edxia-0.1.8/edxia/filters/denoise.py
--rw-rw-r--   0 manawy    (1000) manawy    (1000)     2316 2019-10-13 14:49:34.000000 edxia-0.1.8/edxia/filters/scalers.py
-drwxrwxr-x   0 manawy    (1000) manawy    (1000)        0 2020-12-16 08:59:52.000000 edxia-0.1.8/edxia/glue/
--rw-rw-r--   0 manawy    (1000) manawy    (1000)     1699 2019-05-18 13:45:15.000000 edxia-0.1.8/edxia/glue/__init__.py
--rw-rw-r--   0 manawy    (1000) manawy    (1000)     1964 2019-05-05 08:27:58.000000 edxia-0.1.8/edxia/glue/arithmetic_data.py
--rw-rw-r--   0 manawy    (1000) manawy    (1000)     4047 2019-10-13 14:49:34.000000 edxia-0.1.8/edxia/glue/create_data.py
--rw-rw-r--   0 manawy    (1000) manawy    (1000)     1932 2019-05-18 13:45:15.000000 edxia-0.1.8/edxia/glue/link_data.py
--rw-rw-r--   0 manawy    (1000) manawy    (1000)     4343 2019-05-18 13:52:18.000000 edxia-0.1.8/edxia/glue/map_coordinates.py
--rwxrwxr-x   0 manawy    (1000) manawy    (1000)      608 2020-12-16 08:46:54.000000 edxia-0.1.8/edxia/glue/phase_data.py
-drwxrwxr-x   0 manawy    (1000) manawy    (1000)        0 2020-12-16 08:59:52.000000 edxia-0.1.8/edxia/glue/qt/
--rw-rw-r--   0 manawy    (1000) manawy    (1000)     1565 2019-05-18 13:45:15.000000 edxia-0.1.8/edxia/glue/qt/__init__.py
--rw-rw-r--   0 manawy    (1000) manawy    (1000)    11308 2020-02-22 21:36:02.000000 edxia-0.1.8/edxia/glue/qt/bse_editor.py
--rw-rw-r--   0 manawy    (1000) manawy    (1000)    11405 2020-02-24 20:52:57.000000 edxia-0.1.8/edxia/glue/qt/bse_editor.ui
--rw-rw-r--   0 manawy    (1000) manawy    (1000)     3304 2020-02-03 12:27:02.000000 edxia-0.1.8/edxia/glue/qt/exporter.py
--rw-rw-r--   0 manawy    (1000) manawy    (1000)     3945 2020-08-12 17:19:00.000000 edxia-0.1.8/edxia/glue/qt/linker.py
--rw-rw-r--   0 manawy    (1000) manawy    (1000)    21756 2020-07-24 07:25:07.000000 edxia-0.1.8/edxia/glue/qt/loader.py
--rw-rw-r--   0 manawy    (1000) manawy    (1000)    36023 2020-01-29 11:18:50.000000 edxia-0.1.8/edxia/glue/qt/loader.ui
--rw-rw-r--   0 manawy    (1000) manawy    (1000)     1868 2020-08-11 13:27:23.000000 edxia-0.1.8/edxia/glue/qt/phase_add.ui
--rwxrwxr-x   0 manawy    (1000) manawy    (1000)     4192 2020-12-16 08:49:02.000000 edxia-0.1.8/edxia/glue/qt/phases.py
--rw-rw-r--   0 manawy    (1000) manawy    (1000)     1714 2020-08-11 12:55:27.000000 edxia-0.1.8/edxia/glue/qt/phases.ui
--rw-rw-r--   0 manawy    (1000) manawy    (1000)     4619 2020-02-24 20:52:57.000000 edxia-0.1.8/edxia/glue/qt/points_loader.py
--rw-rw-r--   0 manawy    (1000) manawy    (1000)     7092 2020-02-02 09:32:03.000000 edxia-0.1.8/edxia/glue/qt/points_loader.ui
-drwxrwxr-x   0 manawy    (1000) manawy    (1000)        0 2020-12-16 08:59:52.000000 edxia-0.1.8/edxia/glue/qt/quantifier/
--rw-rw-r--   0 manawy    (1000) manawy    (1000)     2445 2020-02-24 20:52:57.000000 edxia-0.1.8/edxia/glue/qt/quantifier/composition.ui
--rw-rw-r--   0 manawy    (1000) manawy    (1000)     3479 2020-02-24 20:52:57.000000 edxia-0.1.8/edxia/glue/qt/quantifier/main_quantifier.ui
--rw-rw-r--   0 manawy    (1000) manawy    (1000)     5278 2020-01-04 06:18:53.000000 edxia-0.1.8/edxia/glue/qt/quantifier/point_fractions.ui
--rw-rw-r--   0 manawy    (1000) manawy    (1000)     4811 2020-01-07 04:26:34.000000 edxia-0.1.8/edxia/glue/qt/quantifier/s2_correlation.ui
--rw-rw-r--   0 manawy    (1000) manawy    (1000)     2175 2020-02-24 20:52:57.000000 edxia-0.1.8/edxia/glue/qt/quantifier/surface_fractions.ui
--rw-rw-r--   0 manawy    (1000) manawy    (1000)    26203 2020-02-24 20:52:57.000000 edxia-0.1.8/edxia/glue/qt/subset_quantifier.py
-drwxrwxr-x   0 manawy    (1000) manawy    (1000)        0 2020-12-16 08:59:52.000000 edxia-0.1.8/edxia/io/
--rw-rw-r--   0 manawy    (1000) manawy    (1000)     1846 2019-10-19 13:18:15.000000 edxia-0.1.8/edxia/io/__init__.py
--rw-rw-r--   0 manawy    (1000) manawy    (1000)     4382 2019-10-13 14:49:34.000000 edxia-0.1.8/edxia/io/hdf5.py
-drwxrwxr-x   0 manawy    (1000) manawy    (1000)        0 2020-12-16 08:59:52.000000 edxia-0.1.8/edxia/io/loader/
--rw-rw-r--   0 manawy    (1000) manawy    (1000)     2641 2019-11-03 15:03:03.000000 edxia-0.1.8/edxia/io/loader/__init__.py
--rw-rw-r--   0 manawy    (1000) manawy    (1000)     6314 2019-11-03 14:53:01.000000 edxia-0.1.8/edxia/io/loader/base_loader.py
--rw-rw-r--   0 manawy    (1000) manawy    (1000)     2192 2020-01-27 15:39:56.000000 edxia-0.1.8/edxia/io/loader/default_loader.py
--rw-rw-r--   0 manawy    (1000) manawy    (1000)     5230 2019-10-19 13:18:15.000000 edxia-0.1.8/edxia/io/loader/pickle_loader.py
--rw-rw-r--   0 manawy    (1000) manawy    (1000)     2450 2020-01-27 15:42:43.000000 edxia-0.1.8/edxia/io/loader/stack_loader.py
--rw-rw-r--   0 manawy    (1000) manawy    (1000)     7452 2020-02-22 18:03:41.000000 edxia-0.1.8/edxia/io/raw_io.py
-drwxrwxr-x   0 manawy    (1000) manawy    (1000)        0 2020-12-16 08:59:52.000000 edxia-0.1.8/edxia/point_analysis/
--rw-rw-r--   0 manawy    (1000) manawy    (1000)     1611 2019-10-19 16:19:32.000000 edxia-0.1.8/edxia/point_analysis/__init__.py
--rw-rw-r--   0 manawy    (1000) manawy    (1000)     6138 2020-02-01 22:42:28.000000 edxia-0.1.8/edxia/point_analysis/points.py
-drwxrwxr-x   0 manawy    (1000) manawy    (1000)        0 2020-12-16 08:59:52.000000 edxia-0.1.8/edxia/utils/
--rw-rw-r--   0 manawy    (1000) manawy    (1000)     1565 2019-04-25 19:38:24.000000 edxia-0.1.8/edxia/utils/__init__.py
--rw-rw-r--   0 manawy    (1000) manawy    (1000)     8105 2020-08-07 10:28:06.000000 edxia-0.1.8/edxia/utils/chemistry.py
--rw-rw-r--   0 manawy    (1000) manawy    (1000)     2522 2019-04-26 15:36:48.000000 edxia-0.1.8/edxia/utils/coordinates.py
--rw-rw-r--   0 manawy    (1000) manawy    (1000)     3862 2019-05-25 13:40:49.000000 edxia-0.1.8/edxia/utils/path.py
--rw-rw-r--   0 manawy    (1000) manawy    (1000)     7852 2020-08-11 11:05:59.000000 edxia-0.1.8/edxia/utils/qt.py
-drwxrwxr-x   0 manawy    (1000) manawy    (1000)        0 2020-12-16 08:59:52.000000 edxia-0.1.8/edxia.egg-info/
--rw-rw-r--   0 manawy    (1000) manawy    (1000)     2662 2020-12-16 08:59:52.000000 edxia-0.1.8/edxia.egg-info/PKG-INFO
--rw-rw-r--   0 manawy    (1000) manawy    (1000)     1770 2020-12-16 08:59:52.000000 edxia-0.1.8/edxia.egg-info/SOURCES.txt
--rw-rw-r--   0 manawy    (1000) manawy    (1000)        1 2020-12-16 08:59:52.000000 edxia-0.1.8/edxia.egg-info/dependency_links.txt
--rw-rw-r--   0 manawy    (1000) manawy    (1000)       58 2020-12-16 08:59:52.000000 edxia-0.1.8/edxia.egg-info/entry_points.txt
--rw-rw-r--   0 manawy    (1000) manawy    (1000)       98 2020-12-16 08:59:52.000000 edxia-0.1.8/edxia.egg-info/requires.txt
--rw-rw-r--   0 manawy    (1000) manawy    (1000)        6 2020-12-16 08:59:52.000000 edxia-0.1.8/edxia.egg-info/top_level.txt
--rw-rw-r--   0 manawy    (1000) manawy    (1000)       38 2020-12-16 08:59:52.000000 edxia-0.1.8/setup.cfg
--rw-rw-r--   0 manawy    (1000) manawy    (1000)     1674 2020-12-16 08:58:36.000000 edxia-0.1.8/setup.py
+drwxrwxr-x   0 manawy    (1000) manawy    (1000)        0 2021-05-27 15:57:10.870000 edxia-0.1.9/
+-rw-rw-r--   0 manawy    (1000) manawy    (1000)     2767 2021-05-27 15:57:10.870000 edxia-0.1.9/PKG-INFO
+-rw-rw-r--   0 manawy    (1000) manawy    (1000)     1563 2020-01-19 15:48:08.000000 edxia-0.1.9/README.md
+drwxrwxr-x   0 manawy    (1000) manawy    (1000)        0 2021-05-27 15:57:10.838000 edxia-0.1.9/edxia/
+-rw-rw-r--   0 manawy    (1000) manawy    (1000)     2253 2020-08-12 12:58:23.000000 edxia-0.1.9/edxia/__init__.py
+drwxrwxr-x   0 manawy    (1000) manawy    (1000)        0 2021-05-27 15:57:10.840000 edxia-0.1.9/edxia/analysis/
+-rw-rw-r--   0 manawy    (1000) manawy    (1000)     1629 2019-12-26 04:10:16.000000 edxia-0.1.9/edxia/analysis/__init__.py
+-rw-rw-r--   0 manawy    (1000) manawy    (1000)     4139 2020-01-09 08:10:41.000000 edxia-0.1.9/edxia/analysis/correlation.py
+-rw-rw-r--   0 manawy    (1000) manawy    (1000)     2316 2020-02-24 20:52:57.000000 edxia-0.1.9/edxia/analysis/helpers.py
+-rw-rw-r--   0 manawy    (1000) manawy    (1000)     5268 2020-01-04 04:47:55.000000 edxia-0.1.9/edxia/analysis/point_counting.py
+drwxrwxr-x   0 manawy    (1000) manawy    (1000)        0 2021-05-27 15:57:10.843000 edxia-0.1.9/edxia/composite/
+-rw-rw-r--   0 manawy    (1000) manawy    (1000)     1750 2019-10-19 14:16:09.000000 edxia-0.1.9/edxia/composite/__init__.py
+-rw-rw-r--   0 manawy    (1000) manawy    (1000)     3477 2019-10-13 14:49:34.000000 edxia-0.1.9/edxia/composite/channels.py
+-rwxrwxr-x   0 manawy    (1000) manawy    (1000)     2311 2020-05-19 08:35:46.000000 edxia-0.1.9/edxia/composite/color_analysis.py
+-rw-rw-r--   0 manawy    (1000) manawy    (1000)     2668 2020-05-18 18:26:21.000000 edxia-0.1.9/edxia/composite/composite.py
+-rw-rw-r--   0 manawy    (1000) manawy    (1000)     4588 2020-05-18 09:53:31.000000 edxia-0.1.9/edxia/composite/segmentation.py
+drwxrwxr-x   0 manawy    (1000) manawy    (1000)        0 2021-05-27 15:57:10.845000 edxia-0.1.9/edxia/core/
+-rw-rw-r--   0 manawy    (1000) manawy    (1000)     1770 2019-12-23 09:28:42.000000 edxia-0.1.9/edxia/core/__init__.py
+-rw-rw-r--   0 manawy    (1000) manawy    (1000)     7486 2020-01-29 12:35:06.000000 edxia-0.1.9/edxia/core/experiment.py
+-rw-rw-r--   0 manawy    (1000) manawy    (1000)     7301 2021-05-15 13:05:07.000000 edxia-0.1.9/edxia/core/map.py
+drwxrwxr-x   0 manawy    (1000) manawy    (1000)        0 2021-05-27 15:57:10.846000 edxia-0.1.9/edxia/filters/
+-rw-rw-r--   0 manawy    (1000) manawy    (1000)     1566 2019-04-22 12:50:11.000000 edxia-0.1.9/edxia/filters/__init__.py
+-rw-rw-r--   0 manawy    (1000) manawy    (1000)     2270 2019-10-13 14:49:34.000000 edxia-0.1.9/edxia/filters/base_filter.py
+-rw-rw-r--   0 manawy    (1000) manawy    (1000)     3383 2021-05-12 06:29:56.000000 edxia-0.1.9/edxia/filters/denoise.py
+-rw-rw-r--   0 manawy    (1000) manawy    (1000)     2316 2019-10-13 14:49:34.000000 edxia-0.1.9/edxia/filters/scalers.py
+drwxrwxr-x   0 manawy    (1000) manawy    (1000)        0 2021-05-27 15:57:10.851000 edxia-0.1.9/edxia/glue/
+-rw-rw-r--   0 manawy    (1000) manawy    (1000)     1699 2019-05-18 13:45:15.000000 edxia-0.1.9/edxia/glue/__init__.py
+-rw-rw-r--   0 manawy    (1000) manawy    (1000)     1964 2019-05-05 08:27:58.000000 edxia-0.1.9/edxia/glue/arithmetic_data.py
+-rw-rw-r--   0 manawy    (1000) manawy    (1000)     4047 2019-10-13 14:49:34.000000 edxia-0.1.9/edxia/glue/create_data.py
+-rw-rw-r--   0 manawy    (1000) manawy    (1000)     1932 2019-05-18 13:45:15.000000 edxia-0.1.9/edxia/glue/link_data.py
+-rw-rw-r--   0 manawy    (1000) manawy    (1000)     4343 2019-05-18 13:52:18.000000 edxia-0.1.9/edxia/glue/map_coordinates.py
+-rwxrwxr-x   0 manawy    (1000) manawy    (1000)      545 2021-05-23 13:48:21.000000 edxia-0.1.9/edxia/glue/phase_data.py
+drwxrwxr-x   0 manawy    (1000) manawy    (1000)        0 2021-05-27 15:57:10.859000 edxia-0.1.9/edxia/glue/qt/
+-rw-rw-r--   0 manawy    (1000) manawy    (1000)     1565 2019-05-18 13:45:15.000000 edxia-0.1.9/edxia/glue/qt/__init__.py
+-rw-rw-r--   0 manawy    (1000) manawy    (1000)    11308 2020-02-22 21:36:02.000000 edxia-0.1.9/edxia/glue/qt/bse_editor.py
+-rw-rw-r--   0 manawy    (1000) manawy    (1000)    11405 2020-02-24 20:52:57.000000 edxia-0.1.9/edxia/glue/qt/bse_editor.ui
+-rw-rw-r--   0 manawy    (1000) manawy    (1000)     3304 2020-02-03 12:27:02.000000 edxia-0.1.9/edxia/glue/qt/exporter.py
+-rw-rw-r--   0 manawy    (1000) manawy    (1000)     3793 2020-12-27 15:05:35.000000 edxia-0.1.9/edxia/glue/qt/linker.py
+-rw-rw-r--   0 manawy    (1000) manawy    (1000)    22673 2021-05-23 09:50:15.000000 edxia-0.1.9/edxia/glue/qt/loader.py
+-rw-rw-r--   0 manawy    (1000) manawy    (1000)    40279 2021-05-23 11:18:02.000000 edxia-0.1.9/edxia/glue/qt/loader.ui
+-rw-rw-r--   0 manawy    (1000) manawy    (1000)     1868 2021-05-23 11:18:20.000000 edxia-0.1.9/edxia/glue/qt/phase_add.ui
+-rwxrwxr-x   0 manawy    (1000) manawy    (1000)     4235 2020-12-27 14:54:17.000000 edxia-0.1.9/edxia/glue/qt/phases.py
+-rw-rw-r--   0 manawy    (1000) manawy    (1000)     1714 2020-08-11 12:55:27.000000 edxia-0.1.9/edxia/glue/qt/phases.ui
+-rw-rw-r--   0 manawy    (1000) manawy    (1000)     4619 2020-02-24 20:52:57.000000 edxia-0.1.9/edxia/glue/qt/points_loader.py
+-rw-rw-r--   0 manawy    (1000) manawy    (1000)     7092 2020-02-02 09:32:03.000000 edxia-0.1.9/edxia/glue/qt/points_loader.ui
+drwxrwxr-x   0 manawy    (1000) manawy    (1000)        0 2021-05-27 15:57:10.861000 edxia-0.1.9/edxia/glue/qt/quantifier/
+-rw-rw-r--   0 manawy    (1000) manawy    (1000)     2445 2020-02-24 20:52:57.000000 edxia-0.1.9/edxia/glue/qt/quantifier/composition.ui
+-rw-rw-r--   0 manawy    (1000) manawy    (1000)     3479 2020-02-24 20:52:57.000000 edxia-0.1.9/edxia/glue/qt/quantifier/main_quantifier.ui
+-rw-rw-r--   0 manawy    (1000) manawy    (1000)     5278 2020-01-04 06:18:53.000000 edxia-0.1.9/edxia/glue/qt/quantifier/point_fractions.ui
+-rw-rw-r--   0 manawy    (1000) manawy    (1000)     4811 2020-01-07 04:26:34.000000 edxia-0.1.9/edxia/glue/qt/quantifier/s2_correlation.ui
+-rw-rw-r--   0 manawy    (1000) manawy    (1000)     2175 2020-02-24 20:52:57.000000 edxia-0.1.9/edxia/glue/qt/quantifier/surface_fractions.ui
+-rw-rw-r--   0 manawy    (1000) manawy    (1000)    26203 2020-02-24 20:52:57.000000 edxia-0.1.9/edxia/glue/qt/subset_quantifier.py
+drwxrwxr-x   0 manawy    (1000) manawy    (1000)        0 2021-05-27 15:57:10.862000 edxia-0.1.9/edxia/io/
+-rw-rw-r--   0 manawy    (1000) manawy    (1000)     1846 2019-10-19 13:18:15.000000 edxia-0.1.9/edxia/io/__init__.py
+-rw-rw-r--   0 manawy    (1000) manawy    (1000)     4382 2019-10-13 14:49:34.000000 edxia-0.1.9/edxia/io/hdf5.py
+drwxrwxr-x   0 manawy    (1000) manawy    (1000)        0 2021-05-27 15:57:10.866000 edxia-0.1.9/edxia/io/loader/
+-rw-rw-r--   0 manawy    (1000) manawy    (1000)     2641 2019-11-03 15:03:03.000000 edxia-0.1.9/edxia/io/loader/__init__.py
+-rw-rw-r--   0 manawy    (1000) manawy    (1000)     6314 2019-11-03 14:53:01.000000 edxia-0.1.9/edxia/io/loader/base_loader.py
+-rw-rw-r--   0 manawy    (1000) manawy    (1000)     2192 2020-01-27 15:39:56.000000 edxia-0.1.9/edxia/io/loader/default_loader.py
+-rw-rw-r--   0 manawy    (1000) manawy    (1000)     5230 2019-10-19 13:18:15.000000 edxia-0.1.9/edxia/io/loader/pickle_loader.py
+-rw-rw-r--   0 manawy    (1000) manawy    (1000)     2450 2020-01-27 15:42:43.000000 edxia-0.1.9/edxia/io/loader/stack_loader.py
+-rw-rw-r--   0 manawy    (1000) manawy    (1000)     7452 2020-02-22 18:03:41.000000 edxia-0.1.9/edxia/io/raw_io.py
+drwxrwxr-x   0 manawy    (1000) manawy    (1000)        0 2021-05-27 15:57:10.866000 edxia-0.1.9/edxia/point_analysis/
+-rw-rw-r--   0 manawy    (1000) manawy    (1000)     1611 2019-10-19 16:19:32.000000 edxia-0.1.9/edxia/point_analysis/__init__.py
+-rw-rw-r--   0 manawy    (1000) manawy    (1000)     6138 2020-02-01 22:42:28.000000 edxia-0.1.9/edxia/point_analysis/points.py
+drwxrwxr-x   0 manawy    (1000) manawy    (1000)        0 2021-05-27 15:57:10.869000 edxia-0.1.9/edxia/utils/
+-rw-rw-r--   0 manawy    (1000) manawy    (1000)     1565 2019-04-25 19:38:24.000000 edxia-0.1.9/edxia/utils/__init__.py
+-rw-rw-r--   0 manawy    (1000) manawy    (1000)     8105 2020-08-07 10:28:06.000000 edxia-0.1.9/edxia/utils/chemistry.py
+-rw-rw-r--   0 manawy    (1000) manawy    (1000)     2522 2019-04-26 15:36:48.000000 edxia-0.1.9/edxia/utils/coordinates.py
+-rw-rw-r--   0 manawy    (1000) manawy    (1000)     3862 2019-05-25 13:40:49.000000 edxia-0.1.9/edxia/utils/path.py
+-rw-rw-r--   0 manawy    (1000) manawy    (1000)     7852 2020-08-11 11:05:59.000000 edxia-0.1.9/edxia/utils/qt.py
+drwxrwxr-x   0 manawy    (1000) manawy    (1000)        0 2021-05-27 15:57:10.839000 edxia-0.1.9/edxia.egg-info/
+-rw-rw-r--   0 manawy    (1000) manawy    (1000)     2767 2021-05-27 15:57:10.000000 edxia-0.1.9/edxia.egg-info/PKG-INFO
+-rw-rw-r--   0 manawy    (1000) manawy    (1000)     1770 2021-05-27 15:57:10.000000 edxia-0.1.9/edxia.egg-info/SOURCES.txt
+-rw-rw-r--   0 manawy    (1000) manawy    (1000)        1 2021-05-27 15:57:10.000000 edxia-0.1.9/edxia.egg-info/dependency_links.txt
+-rw-rw-r--   0 manawy    (1000) manawy    (1000)       58 2021-05-27 15:57:10.000000 edxia-0.1.9/edxia.egg-info/entry_points.txt
+-rw-rw-r--   0 manawy    (1000) manawy    (1000)      104 2021-05-27 15:57:10.000000 edxia-0.1.9/edxia.egg-info/requires.txt
+-rw-rw-r--   0 manawy    (1000) manawy    (1000)        6 2021-05-27 15:57:10.000000 edxia-0.1.9/edxia.egg-info/top_level.txt
+-rw-rw-r--   0 manawy    (1000) manawy    (1000)       38 2021-05-27 15:57:10.870000 edxia-0.1.9/setup.cfg
+-rw-rw-r--   0 manawy    (1000) manawy    (1000)     1798 2021-05-27 15:55:42.000000 edxia-0.1.9/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `edxia-0.1.8/PKG-INFO` & `edxia-0.1.9/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: edxia
-Version: 0.1.8
+Version: 0.1.9
 Summary: SEM-BSE-EDS image analysis
 Home-page: https://bitbucket.org/specmicp/edxia/
 Author: Fabien Georget
-Author-email: Fabien.georget@epfl.ch
+Author-email: georget@ibac.rwth-aachen.de
 License: BSD
 Project-URL: Funding, https://lmc.epfl.ch/
 Description: # edxia
         
         Analyse SEM-BSE and SEM-EDS maps.
         
         [Scanning Electron Microscopy (SEM)](https://en.wikipedia.org/wiki/Scanning_electron_microscope "Wikipedia link") coupled with [Energy-Dispersive Spectroscopy (EDX)](https://en.wikipedia.org/wiki/Energy-dispersive_X-ray_spectroscopy "wikipedia link") is an imaging technique used in the cement community to learn more about the microstructure of the material.
@@ -48,10 +48,12 @@
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Chemistry
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.4, <4
 Description-Content-Type: text/markdown
 Provides-Extra: jointBilateral
```

### Comparing `edxia-0.1.8/README.md` & `edxia-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `edxia-0.1.8/edxia/__init__.py` & `edxia-0.1.9/edxia/__init__.py`

 * *Files identical despite different names*

### Comparing `edxia-0.1.8/edxia/analysis/__init__.py` & `edxia-0.1.9/edxia/analysis/__init__.py`

 * *Files identical despite different names*

### Comparing `edxia-0.1.8/edxia/analysis/correlation.py` & `edxia-0.1.9/edxia/analysis/correlation.py`

 * *Files identical despite different names*

### Comparing `edxia-0.1.8/edxia/analysis/helpers.py` & `edxia-0.1.9/edxia/analysis/helpers.py`

 * *Files identical despite different names*

### Comparing `edxia-0.1.8/edxia/analysis/point_counting.py` & `edxia-0.1.9/edxia/analysis/point_counting.py`

 * *Files identical despite different names*

### Comparing `edxia-0.1.8/edxia/composite/__init__.py` & `edxia-0.1.9/edxia/composite/__init__.py`

 * *Files identical despite different names*

### Comparing `edxia-0.1.8/edxia/composite/channels.py` & `edxia-0.1.9/edxia/composite/channels.py`

 * *Files identical despite different names*

### Comparing `edxia-0.1.8/edxia/composite/color_analysis.py` & `edxia-0.1.9/edxia/composite/color_analysis.py`

 * *Files identical despite different names*

### Comparing `edxia-0.1.8/edxia/composite/composite.py` & `edxia-0.1.9/edxia/composite/composite.py`

 * *Files identical despite different names*

### Comparing `edxia-0.1.8/edxia/composite/segmentation.py` & `edxia-0.1.9/edxia/composite/segmentation.py`

 * *Files identical despite different names*

### Comparing `edxia-0.1.8/edxia/core/__init__.py` & `edxia-0.1.9/edxia/core/__init__.py`

 * *Files identical despite different names*

### Comparing `edxia-0.1.8/edxia/core/experiment.py` & `edxia-0.1.9/edxia/core/experiment.py`

 * *Files identical despite different names*

### Comparing `edxia-0.1.8/edxia/core/map.py` & `edxia-0.1.9/edxia/core/map.py`

 * *Files 3% similar despite different names*

```diff
@@ -193,8 +193,20 @@
 
     def sum_of_oxides_from_mass(self):
         """Compute the sum of oxides from a mass map."""
         s_oxide = np.zeros((self.shape[0], self.shape[1]))
         for ind, elem in enumerate(self.components):
             if elem in oxides.keys():
                 s_oxide += self._maps[:,:,ind]*molar_masses[oxides[elem][0]]/(oxides[elem][1]*molar_masses[elem])
-        return s_oxide
+        return s_oxide
+
+    def flatten(self, components=None):
+        flat_size = self.shape[0]*self.shape[1]
+        if components is None:
+            components = self.components
+        flat = np.zeros((flat_size, len(components)))
+        for ind, component in enumerate(components):
+            flat[:, ind] = self.map(component).flat_map
+        return flat
+
+    def reshape(self, flat_map):
+        return flat_map.reshape((self.shape[0], self.shape[1]))
```

### Comparing `edxia-0.1.8/edxia/filters/__init__.py` & `edxia-0.1.9/edxia/filters/__init__.py`

 * *Files identical despite different names*

### Comparing `edxia-0.1.8/edxia/filters/base_filter.py` & `edxia-0.1.9/edxia/filters/base_filter.py`

 * *Files identical despite different names*

### Comparing `edxia-0.1.8/edxia/filters/denoise.py` & `edxia-0.1.9/edxia/filters/denoise.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,15 +27,16 @@
 # ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
 # POSSIBILITY OF SUCH DAMAGE.
 
 
 
 import numpy as np
 from skimage.restoration import denoise_tv_chambolle
-from scipy.ndimage import gaussian_filter, uniform_filter
+from scipy.ndimage import gaussian_filter, uniform_filter, median_filter
+#default skimage.filters.rank are on int images
 
 try:
     from cv2.ximgproc import jointBilateralFilter
 except ImportError:
     jointBilateralFilter = None
 
 from .base_filter import AbstractFilter
@@ -55,14 +56,22 @@
     def __init__(self, size, **kwargs):
         self.radius = size
         self.params = kwargs
 
     def apply_impl(self, np_map):
         return uniform_filter(np_map, size=self.radius, **(self.params))
 
+class MedianFilter(AbstractFilter):
+    """Median filter"""
+    def __init__(self, size):
+        self.radius = size
+
+    def apply_impl(self, np_map):
+        return median_filter(np_map, self.radius)
+
 class GaussianFilter(AbstractFilter):
     """GaussianFilter"""
     def __init__(self, sigma, **kwargs):
         self.sigma = sigma
         self.params = kwargs
 
     def apply_impl(self, np_map):
```

### Comparing `edxia-0.1.8/edxia/filters/scalers.py` & `edxia-0.1.9/edxia/filters/scalers.py`

 * *Files identical despite different names*

### Comparing `edxia-0.1.8/edxia/glue/__init__.py` & `edxia-0.1.9/edxia/glue/__init__.py`

 * *Files identical despite different names*

### Comparing `edxia-0.1.8/edxia/glue/arithmetic_data.py` & `edxia-0.1.9/edxia/glue/arithmetic_data.py`

 * *Files identical despite different names*

### Comparing `edxia-0.1.8/edxia/glue/create_data.py` & `edxia-0.1.9/edxia/glue/create_data.py`

 * *Files identical despite different names*

### Comparing `edxia-0.1.8/edxia/glue/link_data.py` & `edxia-0.1.9/edxia/glue/link_data.py`

 * *Files identical despite different names*

### Comparing `edxia-0.1.8/edxia/glue/map_coordinates.py` & `edxia-0.1.9/edxia/glue/map_coordinates.py`

 * *Files identical despite different names*

### Comparing `edxia-0.1.8/edxia/glue/qt/__init__.py` & `edxia-0.1.9/edxia/glue/qt/__init__.py`

 * *Files identical despite different names*

### Comparing `edxia-0.1.8/edxia/glue/qt/bse_editor.py` & `edxia-0.1.9/edxia/glue/qt/bse_editor.py`

 * *Files identical despite different names*

### Comparing `edxia-0.1.8/edxia/glue/qt/bse_editor.ui` & `edxia-0.1.9/edxia/glue/qt/bse_editor.ui`

 * *Files identical despite different names*

### Comparing `edxia-0.1.8/edxia/glue/qt/exporter.py` & `edxia-0.1.9/edxia/glue/qt/exporter.py`

 * *Files identical despite different names*

### Comparing `edxia-0.1.8/edxia/glue/qt/linker.py` & `edxia-0.1.9/edxia/glue/qt/linker.py`

 * *Files 6% similar despite different names*

```diff
@@ -35,16 +35,14 @@
 import qtpy.QtWidgets as qtw
 import qtpy.QtGui as qtg
 import qtpy.QtCore as qtc
 
 from edxia.utils.chemistry import molar_masses
 from edxia.utils.qt import set_busy_app
 
-from edxia.glue.phase_data import PhaseData
-
 components = list(molar_masses.keys())
 components.append("BSE")
 components.append("SOX")
 
 def pts_ratios(numer, denom):
     return numer/denom
 
@@ -61,17 +59,14 @@
                 # Link to other components
                 for ind2, data2 in enumerate(datas):
                     if ind2 <= ind:
                         continue
                     cid2 = data2.find_component_id(component)
                     if cid2 is not None:
                         links.append(ComponentLink([cid,], cid2))
-                # Ratio links
-                if isinstance(data, PhaseData):
-                    continue
                 if component in ["Al", "S", "Cl", "Mg", "Si", "Fe"]:
                     cid_ca = data.find_component_id("Ca")
                     if cid_ca is not None:
                         # Define the ratios as ParsedCommand so they appear in the editor
                         equation = "{"+component+"}/{Ca}"
                         references = {"Ca": cid_ca, component: cid}
                         cmd = ParsedCommand(equation, references)
```

### Comparing `edxia-0.1.8/edxia/glue/qt/loader.py` & `edxia-0.1.9/edxia/glue/qt/loader.py`

 * *Files 3% similar despite different names*

```diff
@@ -53,31 +53,33 @@
 
 ## edxia import
 
 from ...core.experiment import MappingExperiment
 
 from edxia.filters import denoise
 
-from edxia.filters.denoise import DenoiseFilter, UniformFilter, GaussianFilter
+from edxia.filters.denoise import DenoiseFilter, UniformFilter, GaussianFilter, MedianFilter
 from edxia.io.loader import DefaultLoader, StackLoader
 from edxia.composite import CompositeChannels
 from edxia.composite.segmentation import SlicSegmenter
 from edxia.composite.color_analysis import ColorPCA
 from edxia.point_analysis.points import points_from_segmentation
+from edxia.core import Map
 
 from edxia.io.raw_io import TextMapFormat
 from edxia.io import raw_io
 from edxia.io.hdf5 import save_dataset, read_dataset
 
 from edxia.utils.qt import SetBusyApp
 
 from .. import gluedata_from_points, gluedata_from_stack_and_composite, gluedata_from_stack
 
 
-
+from skimage.filters.rank import median, maximum, minimum
+from skimage.morphology import disk
 
 
 
 class PreviewBSE(FigureCanvas):
     """Preview the BSE map."""
     def __init__(self, parent=None):
         fig = Figure()
@@ -318,18 +320,20 @@
     def _change_all_params(self, enabled):
         ui = self._ui
 
         widgets = [
                 ui.no_filter_check,
                 ui.tv_filter_check,
                 ui.mean_filter_check,
+                ui.median_filter_check,
                 ui.gaussian_filter_check,
 
                 ui.weight_filter_box,
                 ui.radius_filter_box,
+                ui.radius_filter_box_2,
                 ui.sigma_filter_box,
 
                 ui.test_filter_button,
                 ui.test_filter_combo,
 
                 ui.segmentation_check,
                 ui.test_segmentation_button,
@@ -375,14 +379,18 @@
             weight = float(self._ui.weight_filter_box.text())
             name = "TotalVariation({0})".format(weight)
             filters = [DenoiseFilter(weight),]
         elif self._ui.mean_filter_check.isChecked():
             radius = self._ui.radius_filter_box.value()
             name = "UniformFilter({0})".format(radius)
             filters = [UniformFilter(radius),]
+        elif self._ui.median_filter_check.isChecked():
+            radius = self._ui.radius_filter_box_2.value()
+            name = "MedianFilter({0})".format(radius)
+            filters = [MedianFilter(radius),]
         elif self._ui.gaussian_filter_check.isChecked():
             sigma = self._ui.sigma_filter_box.value()
             name = "GaussianFilter({0})".format(sigma)
             filters = [GaussianFilter(sigma),]
         elif self._ui.joint_filter_check.isChecked():
             sigmaR = self._ui.sigmaR_filter_box.value()
             sigmaS = self._ui.sigmaS_filter_box.value()
@@ -533,38 +541,48 @@
             stack_has_changed = True
 
         if stack_has_changed:
             loader = StackLoader(stack)
 
 
         if ui.segmentation_check.isChecked():
-            channels = self.get_channels()
-            composite = loader.load_composite(channels)
-
 
             bse_map =  loader.load_edsmap("BSE")
+            compactness = float(ui.compactness_box.text())
+            numberpts = float(ui.numberpts_box.text())
+            segmenter = SlicSegmenter(compactness, numberpts)
+
+            channels = self.get_channels()
+            composite = loader.load_composite(channels)
 
             if ui.bsemix_check.isChecked():
                 composite.mix_with_bse(bse_map, ui.alpha_box.value())
             if ui.filterbse_check.isChecked():
                 composite.map[bse_map.map<0.2,:] = 0
 
 
-            # segmentation
-            compactness = float(ui.compactness_box.text())
-            numberpts = float(ui.numberpts_box.text())
-            labels = SlicSegmenter(compactness, numberpts).apply(composite)
+            if ui.compositesegm_button.isChecked():
 
-            pca = ColorPCA(labels)
-            pca_transformed = pca.transform_rgb(composite.map)
-            extras["PCA1"] = pca_transformed[:,:,0]
-            extras["PCA2"] = pca_transformed[:,:,1]
-            extras["PCA3"] = pca_transformed[:,:,2]
+                # segmentation
+                labels = segmenter.apply(composite)
 
+                pca = ColorPCA(labels)
+                pca_transformed = pca.transform_rgb(composite.map)
+                extras["PCA1"] = pca_transformed[:,:,0]
+                extras["PCA2"] = pca_transformed[:,:,1]
+                extras["PCA3"] = pca_transformed[:,:,2]
+
+            elif ui.bsesegm_button.isChecked():
+                radius = ui.bsesegm_radius_box.value()
+                image = median(bse_map.map, disk(radius))
+                image = minimum(maximum(image, disk(radius)), disk(radius))
+                bse_filter = Map("BSE", image, exp)
+                labels = segmenter.apply(bse_filter)
 
+            # stack and pts data
             stack_data = gluedata_from_stack_and_composite(exp.label+"maps", stack, composite, coords=coords, extras=extras)
             pts = points_from_segmentation(stack, labels, mask_img=composite.map, include_yx=True, extras=extras)
             pts_data = gluedata_from_points(exp.label+"points", pts)
 
         else:
             composite = None
             pts = None
```

### Comparing `edxia-0.1.8/edxia/glue/qt/loader.ui` & `edxia-0.1.9/edxia/glue/qt/loader.ui`

 * *Files 2% similar despite different names*

#### Comparing `edxia-0.1.8/edxia/glue/qt/loader.ui` & `edxia-0.1.9/edxia/glue/qt/loader.ui`

```diff
@@ -152,20 +152,20 @@
               </property>
               <property name="html">
                 <string>&lt;!DOCTYPE HTML PUBLIC &quot;-//W3C//DTD HTML 4.0//EN&quot; &quot;http://www.w3.org/TR/REC-html40/strict.dtd&quot;&gt;
 &lt;html&gt;&lt;head&gt;&lt;meta name=&quot;qrichtext&quot; content=&quot;1&quot; /&gt;&lt;title&gt;Help:&lt;/title&gt;&lt;style type=&quot;text/css&quot;&gt;
 p, li { white-space: pre-wrap; }
 &lt;/style&gt;&lt;/head&gt;&lt;body style=&quot; font-family:'Sans Serif'; font-size:10pt; font-weight:400; font-style:normal;&quot;&gt;
 &lt;h2 style=&quot; margin-top:16px; margin-bottom:12px; margin-left:0px; margin-right:0px; -qt-block-indent:0; text-indent:0px;&quot;&gt;&lt;span style=&quot; font-size:x-large; font-weight:600;&quot;&gt;How to:&lt;/span&gt;&lt;/h2&gt;
-&lt;ol style=&quot;margin-top: 0px; margin-bottom: 0px; margin-left: 0px; margin-right: 0px; -qt-list-indent: 1;&quot;&gt;&lt;li style=&quot; margin-top:12px; margin-bottom:0px; margin-left:0px; margin-right:0px; -qt-block-indent:0; text-indent:0px;&quot;&gt;Select format &lt;/li&gt;
-&lt;li style=&quot; margin-top:0px; margin-bottom:0px; margin-left:0px; margin-right:0px; -qt-block-indent:0; text-indent:0px;&quot;&gt;Open preview by selecting the BSE file&lt;/li&gt;
-&lt;li style=&quot; margin-top:0px; margin-bottom:0px; margin-left:0px; margin-right:0px; -qt-block-indent:0; text-indent:0px;&quot;&gt;Check on the preview&lt;/li&gt;
-&lt;li style=&quot; margin-top:0px; margin-bottom:0px; margin-left:0px; margin-right:0px; -qt-block-indent:0; text-indent:0px;&quot;&gt;Set the scale and the units of the map&lt;/li&gt;
-&lt;li style=&quot; margin-top:0px; margin-bottom:0px; margin-left:0px; margin-right:0px; -qt-block-indent:0; text-indent:0px;&quot;&gt;Select the denoising algorithm&lt;/li&gt;
-&lt;li style=&quot; margin-top:0px; margin-bottom:12px; margin-left:0px; margin-right:0px; -qt-block-indent:0; text-indent:0px;&quot;&gt;Select the options of point analysis&lt;/li&gt;&lt;/ol&gt;
+&lt;ol style=&quot;margin-top: 0px; margin-bottom: 0px; margin-left: 0px; margin-right: 0px; -qt-list-indent: 1;&quot;&gt;&lt;li style=&quot;&quot; style=&quot; margin-top:12px; margin-bottom:0px; margin-left:0px; margin-right:0px; -qt-block-indent:0; text-indent:0px;&quot;&gt;Select format &lt;/li&gt;
+&lt;li style=&quot;&quot; style=&quot; margin-top:0px; margin-bottom:0px; margin-left:0px; margin-right:0px; -qt-block-indent:0; text-indent:0px;&quot;&gt;Open preview by selecting the BSE file&lt;/li&gt;
+&lt;li style=&quot;&quot; style=&quot; margin-top:0px; margin-bottom:0px; margin-left:0px; margin-right:0px; -qt-block-indent:0; text-indent:0px;&quot;&gt;Check on the preview&lt;/li&gt;
+&lt;li style=&quot;&quot; style=&quot; margin-top:0px; margin-bottom:0px; margin-left:0px; margin-right:0px; -qt-block-indent:0; text-indent:0px;&quot;&gt;Set the scale and the units of the map&lt;/li&gt;
+&lt;li style=&quot;&quot; style=&quot; margin-top:0px; margin-bottom:0px; margin-left:0px; margin-right:0px; -qt-block-indent:0; text-indent:0px;&quot;&gt;Select the denoising algorithm&lt;/li&gt;
+&lt;li style=&quot;&quot; style=&quot; margin-top:0px; margin-bottom:12px; margin-left:0px; margin-right:0px; -qt-block-indent:0; text-indent:0px;&quot;&gt;Select the options of point analysis&lt;/li&gt;&lt;/ol&gt;
 &lt;h2 style=&quot; margin-top:16px; margin-bottom:12px; margin-left:0px; margin-right:0px; -qt-block-indent:0; text-indent:0px;&quot;&gt;&lt;span style=&quot; font-size:x-large; font-weight:600;&quot;&gt;About:&lt;/span&gt;&lt;/h2&gt;
 &lt;p style=&quot; margin-top:12px; margin-bottom:12px; margin-left:0px; margin-right:0px; -qt-block-indent:0; text-indent:0px;&quot;&gt;edxia is a plugin to analyse EDX/BSE hypermaps, especially designed for cementitious materials.&lt;/p&gt;
 &lt;h3 style=&quot; margin-top:14px; margin-bottom:12px; margin-left:0px; margin-right:0px; -qt-block-indent:0; text-indent:0px;&quot;&gt;&lt;span style=&quot; font-size:large; font-weight:600;&quot;&gt;Author: &lt;/span&gt;&lt;/h3&gt;
 &lt;p style=&quot; margin-top:12px; margin-bottom:12px; margin-left:0px; margin-right:0px; -qt-block-indent:0; text-indent:0px;&quot;&gt;Fabien Georget,&lt;br /&gt;EPFL, laboratory of construction materials&lt;br /&gt;Lausanne, Switzerland&lt;br /&gt;&lt;a href=&quot;mailto:fabien.georget@epfl.ch&quot;&gt;&lt;span style=&quot; text-decoration: underline; color:#2980b9;&quot;&gt;fabien.georget@epfl.ch&lt;/span&gt;&lt;/a&gt;&lt;/p&gt;&lt;/body&gt;&lt;/html&gt;</string>
               </property>
             </widget>
           </widget>
@@ -539,338 +539,444 @@
             <attribute name="title">
               <string>Denoising</string>
             </attribute>
             <widget class="QWidget" name="layoutWidget">
               <property name="geometry">
                 <rect>
                   <x>70</x>
-                  <y>60</y>
-                  <width>310</width>
-                  <height>208</height>
+                  <y>40</y>
+                  <width>378</width>
+                  <height>294</height>
                 </rect>
               </property>
-              <layout class="QGridLayout" name="gridLayout">
-                <item row="2" column="1">
-                  <widget class="QLabel" name="label_10">
-                    <property name="text">
-                      <string>Radius</string>
-                    </property>
-                  </widget>
-                </item>
-                <item row="1" column="0">
-                  <widget class="QRadioButton" name="tv_filter_check">
-                    <property name="text">
-                      <string>Total variation</string>
-                    </property>
-                    <property name="checked">
-                      <bool>true</bool>
-                    </property>
-                  </widget>
-                </item>
-                <item row="0" column="0">
-                  <widget class="QRadioButton" name="no_filter_check">
-                    <property name="text">
-                      <string>No Filter</string>
-                    </property>
-                  </widget>
-                </item>
-                <item row="0" column="1">
-                  <spacer name="horizontalSpacer">
-                    <property name="orientation">
-                      <enum>Qt::Horizontal</enum>
-                    </property>
-                    <property name="sizeHint" stdset="0">
-                      <size>
-                        <width>40</width>
-                        <height>20</height>
-                      </size>
-                    </property>
-                  </spacer>
-                </item>
-                <item row="2" column="0">
-                  <widget class="QRadioButton" name="mean_filter_check">
-                    <property name="text">
-                      <string>Mean filter</string>
-                    </property>
-                  </widget>
-                </item>
-                <item row="3" column="0">
-                  <widget class="QRadioButton" name="gaussian_filter_check">
-                    <property name="text">
-                      <string>Gaussian filter</string>
-                    </property>
-                  </widget>
-                </item>
-                <item row="3" column="2">
-                  <widget class="QDoubleSpinBox" name="sigma_filter_box">
-                    <property name="decimals">
-                      <number>3</number>
-                    </property>
-                    <property name="value">
-                      <double>0.500000000000000</double>
-                    </property>
-                  </widget>
-                </item>
-                <item row="4" column="0">
-                  <widget class="QRadioButton" name="joint_filter_check">
-                    <property name="enabled">
-                      <bool>false</bool>
-                    </property>
-                    <property name="text">
-                      <string>Joint bilateral Filter</string>
-                    </property>
-                  </widget>
-                </item>
-                <item row="3" column="1">
-                  <widget class="QLabel" name="label_11">
-                    <property name="text">
-                      <string>Sigma</string>
-                    </property>
-                  </widget>
-                </item>
-                <item row="2" column="2">
-                  <widget class="QSpinBox" name="radius_filter_box">
-                    <property name="maximum">
-                      <number>999</number>
-                    </property>
-                    <property name="value">
-                      <number>3</number>
-                    </property>
-                  </widget>
-                </item>
-                <item row="1" column="1">
-                  <widget class="QLabel" name="label_9">
-                    <property name="text">
-                      <string>Weight</string>
-                    </property>
-                  </widget>
-                </item>
-                <item row="4" column="1">
-                  <widget class="QLabel" name="label_26">
-                    <property name="text">
-                      <string>Sigma S</string>
-                    </property>
-                  </widget>
-                </item>
-                <item row="1" column="2">
-                  <widget class="QLineEdit" name="weight_filter_box">
-                    <property name="inputMethodHints">
-                      <set>Qt::ImhDigitsOnly</set>
-                    </property>
-                    <property name="inputMask">
-                      <string>0000.0000</string>
-                    </property>
-                    <property name="text">
-                      <string>0.1</string>
-                    </property>
-                  </widget>
+              <layout class="QVBoxLayout" name="verticalLayout_12">
+                <item>
+                  <layout class="QGridLayout" name="gridLayout">
+                    <item row="3" column="0">
+                      <widget class="QRadioButton" name="median_filter_check">
+                        <property name="text">
+                          <string>Median filter</string>
+                        </property>
+                      </widget>
+                    </item>
+                    <item row="0" column="2">
+                      <spacer name="horizontalSpacer_2">
+                        <property name="orientation">
+                          <enum>Qt::Horizontal</enum>
+                        </property>
+                        <property name="sizeHint" stdset="0">
+                          <size>
+                            <width>40</width>
+                            <height>20</height>
+                          </size>
+                        </property>
+                      </spacer>
+                    </item>
+                    <item row="4" column="0">
+                      <widget class="QRadioButton" name="gaussian_filter_check">
+                        <property name="text">
+                          <string>Gaussian filter</string>
+                        </property>
+                      </widget>
+                    </item>
+                    <item row="5" column="2">
+                      <widget class="QDoubleSpinBox" name="sigmaS_filter_box">
+                        <property name="enabled">
+                          <bool>false</bool>
+                        </property>
+                        <property name="decimals">
+                          <number>3</number>
+                        </property>
+                        <property name="value">
+                          <double>10.000000000000000</double>
+                        </property>
+                      </widget>
+                    </item>
+                    <item row="2" column="1">
+                      <widget class="QLabel" name="label_10">
+                        <property name="text">
+                          <string>Radius</string>
+                        </property>
+                      </widget>
+                    </item>
+                    <item row="2" column="2">
+                      <widget class="QSpinBox" name="radius_filter_box">
+                        <property name="maximum">
+                          <number>999</number>
+                        </property>
+                        <property name="value">
+                          <number>3</number>
+                        </property>
+                      </widget>
+                    </item>
+                    <item row="3" column="1">
+                      <widget class="QLabel" name="label_28">
+                        <property name="text">
+                          <string>Radius</string>
+                        </property>
+                      </widget>
+                    </item>
+                    <item row="6" column="2">
+                      <widget class="QDoubleSpinBox" name="sigmaR_filter_box">
+                        <property name="enabled">
+                          <bool>false</bool>
+                        </property>
+                        <property name="decimals">
+                          <number>3</number>
+                        </property>
+                        <property name="value">
+                          <double>2.500000000000000</double>
+                        </property>
+                      </widget>
+                    </item>
+                    <item row="2" column="0">
+                      <widget class="QRadioButton" name="mean_filter_check">
+                        <property name="text">
+                          <string>Mean filter</string>
+                        </property>
+                      </widget>
+                    </item>
+                    <item row="4" column="2">
+                      <widget class="QDoubleSpinBox" name="sigma_filter_box">
+                        <property name="decimals">
+                          <number>3</number>
+                        </property>
+                        <property name="value">
+                          <double>0.500000000000000</double>
+                        </property>
+                      </widget>
+                    </item>
+                    <item row="5" column="0">
+                      <widget class="QRadioButton" name="joint_filter_check">
+                        <property name="enabled">
+                          <bool>false</bool>
+                        </property>
+                        <property name="text">
+                          <string>Joint bilateral Filter</string>
+                        </property>
+                      </widget>
+                    </item>
+                    <item row="6" column="1">
+                      <widget class="QLabel" name="label_27">
+                        <property name="text">
+                          <string>Sigma R</string>
+                        </property>
+                      </widget>
+                    </item>
+                    <item row="1" column="2">
+                      <widget class="QLineEdit" name="weight_filter_box">
+                        <property name="inputMethodHints">
+                          <set>Qt::ImhDigitsOnly</set>
+                        </property>
+                        <property name="inputMask">
+                          <string>0000.0000</string>
+                        </property>
+                        <property name="text">
+                          <string>0.1</string>
+                        </property>
+                      </widget>
+                    </item>
+                    <item row="5" column="1">
+                      <widget class="QLabel" name="label_26">
+                        <property name="text">
+                          <string>Sigma S</string>
+                        </property>
+                      </widget>
+                    </item>
+                    <item row="3" column="2">
+                      <widget class="QSpinBox" name="radius_filter_box_2">
+                        <property name="maximum">
+                          <number>999</number>
+                        </property>
+                        <property name="value">
+                          <number>3</number>
+                        </property>
+                      </widget>
+                    </item>
+                    <item row="1" column="0">
+                      <widget class="QRadioButton" name="tv_filter_check">
+                        <property name="text">
+                          <string>Total variation</string>
+                        </property>
+                        <property name="checked">
+                          <bool>true</bool>
+                        </property>
+                      </widget>
+                    </item>
+                    <item row="4" column="1">
+                      <widget class="QLabel" name="label_11">
+                        <property name="text">
+                          <string>Sigma</string>
+                        </property>
+                      </widget>
+                    </item>
+                    <item row="1" column="1">
+                      <widget class="QLabel" name="label_9">
+                        <property name="text">
+                          <string>Weight</string>
+                        </property>
+                      </widget>
+                    </item>
+                    <item row="0" column="1">
+                      <spacer name="horizontalSpacer">
+                        <property name="orientation">
+                          <enum>Qt::Horizontal</enum>
+                        </property>
+                        <property name="sizeHint" stdset="0">
+                          <size>
+                            <width>40</width>
+                            <height>20</height>
+                          </size>
+                        </property>
+                      </spacer>
+                    </item>
+                    <item row="0" column="0">
+                      <widget class="QRadioButton" name="no_filter_check">
+                        <property name="text">
+                          <string>No Filter</string>
+                        </property>
+                      </widget>
+                    </item>
+                  </layout>
                 </item>
-                <item row="0" column="2">
-                  <spacer name="horizontalSpacer_2">
+                <item>
+                  <spacer name="verticalSpacer_2">
                     <property name="orientation">
-                      <enum>Qt::Horizontal</enum>
+                      <enum>Qt::Vertical</enum>
                     </property>
                     <property name="sizeHint" stdset="0">
                       <size>
-                        <width>40</width>
-                        <height>20</height>
+                        <width>20</width>
+                        <height>40</height>
                       </size>
                     </property>
                   </spacer>
                 </item>
-                <item row="5" column="1">
-                  <widget class="QLabel" name="label_27">
-                    <property name="text">
-                      <string>Sigma R</string>
-                    </property>
-                  </widget>
-                </item>
-                <item row="4" column="2">
-                  <widget class="QDoubleSpinBox" name="sigmaS_filter_box">
-                    <property name="enabled">
-                      <bool>false</bool>
-                    </property>
-                    <property name="decimals">
-                      <number>3</number>
-                    </property>
-                    <property name="value">
-                      <double>10.000000000000000</double>
-                    </property>
-                  </widget>
-                </item>
-                <item row="5" column="2">
-                  <widget class="QDoubleSpinBox" name="sigmaR_filter_box">
-                    <property name="enabled">
-                      <bool>false</bool>
-                    </property>
-                    <property name="decimals">
-                      <number>3</number>
-                    </property>
-                    <property name="value">
-                      <double>2.500000000000000</double>
-                    </property>
-                  </widget>
-                </item>
-              </layout>
-            </widget>
-            <widget class="QWidget" name="layoutWidget">
-              <property name="geometry">
-                <rect>
-                  <x>70</x>
-                  <y>280</y>
-                  <width>197</width>
-                  <height>35</height>
-                </rect>
-              </property>
-              <layout class="QHBoxLayout" name="horizontalLayout_12">
-                <item>
-                  <widget class="QPushButton" name="test_filter_button">
-                    <property name="text">
-                      <string>Test filter on</string>
-                    </property>
-                  </widget>
-                </item>
                 <item>
-                  <widget class="QComboBox" name="test_filter_combo"/>
+                  <layout class="QHBoxLayout" name="horizontalLayout_12">
+                    <item>
+                      <spacer name="horizontalSpacer_4">
+                        <property name="orientation">
+                          <enum>Qt::Horizontal</enum>
+                        </property>
+                        <property name="sizeHint" stdset="0">
+                          <size>
+                            <width>40</width>
+                            <height>20</height>
+                          </size>
+                        </property>
+                      </spacer>
+                    </item>
+                    <item>
+                      <widget class="QPushButton" name="test_filter_button">
+                        <property name="text">
+                          <string>Test filter on</string>
+                        </property>
+                      </widget>
+                    </item>
+                    <item>
+                      <widget class="QComboBox" name="test_filter_combo"/>
+                    </item>
+                  </layout>
                 </item>
               </layout>
             </widget>
           </widget>
           <widget class="QWidget" name="param_tab">
             <attribute name="title">
               <string>Point analysis</string>
             </attribute>
             <widget class="QWidget" name="layoutWidget">
               <property name="geometry">
                 <rect>
-                  <x>20</x>
+                  <x>30</x>
                   <y>20</y>
                   <width>511</width>
-                  <height>341</height>
+                  <height>401</height>
                 </rect>
               </property>
               <layout class="QVBoxLayout" name="verticalLayout_2">
                 <item>
                   <widget class="QCheckBox" name="segmentation_check">
                     <property name="text">
                       <string>Use segmentation</string>
                     </property>
                     <property name="checked">
                       <bool>true</bool>
                     </property>
                   </widget>
                 </item>
                 <item>
-                  <layout class="QVBoxLayout" name="verticalLayout">
+                  <layout class="QVBoxLayout" name="verticalLayout_14">
                     <item>
-                      <layout class="QHBoxLayout" name="horizontalLayout_3">
-                        <item>
-                          <widget class="QLabel" name="label_3">
-                            <property name="text">
-                              <string>Green</string>
-                            </property>
-                          </widget>
-                        </item>
-                        <item>
-                          <widget class="QComboBox" name="green_combo"/>
-                        </item>
+                      <widget class="QRadioButton" name="bsesegm_button">
+                        <property name="text">
+                          <string>BSE-based segmentation</string>
+                        </property>
+                      </widget>
+                    </item>
+                    <item>
+                      <layout class="QHBoxLayout" name="horizontalLayout_14">
                         <item>
-                          <widget class="QDoubleSpinBox" name="green_factor_box">
-                            <property name="decimals">
-                              <number>2</number>
+                          <spacer name="horizontalSpacer_5">
+                            <property name="orientation">
+                              <enum>Qt::Horizontal</enum>
                             </property>
-                            <property name="value">
-                              <double>4.000000000000000</double>
+                            <property name="sizeHint" stdset="0">
+                              <size>
+                                <width>40</width>
+                                <height>20</height>
+                              </size>
                             </property>
-                          </widget>
+                          </spacer>
                         </item>
-                      </layout>
-                    </item>
-                    <item>
-                      <layout class="QHBoxLayout" name="horizontalLayout_4">
                         <item>
-                          <widget class="QLabel" name="label_4">
+                          <widget class="QLabel" name="radius_label">
                             <property name="text">
-                              <string>Red</string>
+                              <string>Filter radius</string>
                             </property>
                           </widget>
                         </item>
                         <item>
-                          <widget class="QComboBox" name="red_combo"/>
-                        </item>
-                        <item>
-                          <widget class="QDoubleSpinBox" name="red_factor_box">
+                          <widget class="QSpinBox" name="bsesegm_radius_box">
                             <property name="value">
-                              <double>4.000000000000000</double>
+                              <number>5</number>
                             </property>
                           </widget>
                         </item>
                       </layout>
                     </item>
+                  </layout>
+                </item>
+                <item>
+                  <layout class="QVBoxLayout" name="verticalLayout_11">
                     <item>
-                      <layout class="QHBoxLayout" name="horizontalLayout_5">
+                      <layout class="QVBoxLayout" name="verticalLayout_13">
                         <item>
-                          <widget class="QLabel" name="label_5">
+                          <widget class="QRadioButton" name="compositesegm_button">
                             <property name="text">
-                              <string>Blue</string>
+                              <string>Composite-based segmentation</string>
+                            </property>
+                            <property name="checked">
+                              <bool>true</bool>
                             </property>
                           </widget>
                         </item>
                         <item>
-                          <widget class="QComboBox" name="blue_combo"/>
+                          <layout class="QVBoxLayout" name="verticalLayout">
+                            <item>
+                              <layout class="QHBoxLayout" name="horizontalLayout_3">
+                                <item>
+                                  <widget class="QLabel" name="label_3">
+                                    <property name="text">
+                                      <string>Green</string>
+                                    </property>
+                                  </widget>
+                                </item>
+                                <item>
+                                  <widget class="QComboBox" name="green_combo"/>
+                                </item>
+                                <item>
+                                  <widget class="QDoubleSpinBox" name="green_factor_box">
+                                    <property name="decimals">
+                                      <number>2</number>
+                                    </property>
+                                    <property name="value">
+                                      <double>4.000000000000000</double>
+                                    </property>
+                                  </widget>
+                                </item>
+                              </layout>
+                            </item>
+                            <item>
+                              <layout class="QHBoxLayout" name="horizontalLayout_4">
+                                <item>
+                                  <widget class="QLabel" name="label_4">
+                                    <property name="text">
+                                      <string>Red</string>
+                                    </property>
+                                  </widget>
+                                </item>
+                                <item>
+                                  <widget class="QComboBox" name="red_combo"/>
+                                </item>
+                                <item>
+                                  <widget class="QDoubleSpinBox" name="red_factor_box">
+                                    <property name="value">
+                                      <double>4.000000000000000</double>
+                                    </property>
+                                  </widget>
+                                </item>
+                              </layout>
+                            </item>
+                            <item>
+                              <layout class="QHBoxLayout" name="horizontalLayout_5">
+                                <item>
+                                  <widget class="QLabel" name="label_5">
+                                    <property name="text">
+                                      <string>Blue</string>
+                                    </property>
+                                  </widget>
+                                </item>
+                                <item>
+                                  <widget class="QComboBox" name="blue_combo"/>
+                                </item>
+                                <item>
+                                  <widget class="QDoubleSpinBox" name="blue_factor_box">
+                                    <property name="value">
+                                      <double>2.000000000000000</double>
+                                    </property>
+                                  </widget>
+                                </item>
+                              </layout>
+                            </item>
+                          </layout>
                         </item>
                         <item>
-                          <widget class="QDoubleSpinBox" name="blue_factor_box">
-                            <property name="value">
-                              <double>2.000000000000000</double>
-                            </property>
-                          </widget>
+                          <layout class="QHBoxLayout" name="horizontalLayout_7">
+                            <item>
+                              <widget class="QCheckBox" name="bsemix_check">
+                                <property name="text">
+                                  <string>Mix with BSE</string>
+                                </property>
+                                <property name="checked">
+                                  <bool>true</bool>
+                                </property>
+                              </widget>
+                            </item>
+                            <item>
+                              <widget class="QLabel" name="label_7">
+                                <property name="text">
+                                  <string>Alpha</string>
+                                </property>
+                                <property name="alignment">
+                                  <set>Qt::AlignRight|Qt::AlignTrailing|Qt::AlignVCenter</set>
+                                </property>
+                              </widget>
+                            </item>
+                            <item>
+                              <widget class="QDoubleSpinBox" name="alpha_box">
+                                <property name="maximum">
+                                  <double>1.000000000000000</double>
+                                </property>
+                                <property name="singleStep">
+                                  <double>0.050000000000000</double>
+                                </property>
+                                <property name="value">
+                                  <double>0.800000000000000</double>
+                                </property>
+                              </widget>
+                            </item>
+                          </layout>
                         </item>
                       </layout>
                     </item>
                   </layout>
                 </item>
                 <item>
-                  <layout class="QHBoxLayout" name="horizontalLayout_7">
-                    <item>
-                      <widget class="QCheckBox" name="bsemix_check">
-                        <property name="text">
-                          <string>Mix with BSE</string>
-                        </property>
-                        <property name="checked">
-                          <bool>true</bool>
-                        </property>
-                      </widget>
-                    </item>
-                    <item>
-                      <widget class="QLabel" name="label_7">
-                        <property name="text">
-                          <string>Alpha</string>
-                        </property>
-                        <property name="alignment">
-                          <set>Qt::AlignRight|Qt::AlignTrailing|Qt::AlignVCenter</set>
-                        </property>
-                      </widget>
-                    </item>
-                    <item>
-                      <widget class="QDoubleSpinBox" name="alpha_box">
-                        <property name="maximum">
-                          <double>1.000000000000000</double>
-                        </property>
-                        <property name="singleStep">
-                          <double>0.050000000000000</double>
-                        </property>
-                        <property name="value">
-                          <double>0.800000000000000</double>
-                        </property>
-                      </widget>
-                    </item>
-                  </layout>
-                </item>
-                <item>
                   <layout class="QHBoxLayout" name="horizontalLayout_6">
                     <item>
                       <widget class="QLabel" name="label_6">
                         <property name="text">
                           <string>Number of points</string>
                         </property>
                       </widget>
```

### Comparing `edxia-0.1.8/edxia/glue/qt/phase_add.ui` & `edxia-0.1.9/edxia/glue/qt/phase_add.ui`

 * *Files identical despite different names*

### Comparing `edxia-0.1.8/edxia/glue/qt/phases.py` & `edxia-0.1.9/edxia/glue/qt/phases.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,47 +6,49 @@
 import qtpy.compat as qcompat
 import qtpy.QtWidgets as qtw
 
 
 from glue.utils.qt.helpers import load_ui
 
 from edxia.utils.chemistry import phases_df_from_file, formula_to_composition, normalize_composition
-from edxia.glue.phase_data import PhaseData
+from edxia.glue.phase_data import create_phase_data
 
 from edxia.utils.qt import EditablePandasTableModel
 
 __all__ = ["phases_loader"]
 
 PHASES_LABEL = "Phases"
 
 def get_phases_data(data_collection):
     if "Phases" in data_collection:
         return data_collection[PHASES_LABEL]
     else:
         return None
 
+
 @menubar_plugin("edxia: load Phases (Experimental !)")
 def phases_loader(session, data_collection):
-    """The menubar action to load the phases dataset"""
+    """The menubar action to load the phases dataset."""
     filename, _ = qcompat.getopenfilename(None, caption="Phase database")
 
     if filename == "":
         return
     else:
         df = phases_df_from_file(filename)
 
     phases = get_phases_data(data_collection)
     if phases is None:
-        data_collection[PHASES_LABEL] = PhaseData(df)
+        data_collection[PHASES_LABEL] = create_phase_data(df)
     else:
-        new_data = PhaseData(df)
+        new_data = create_phase_data(df)
         new_data.label = PHASES_LABEL
         phases.update_values_from_data(new_data)
     return
 
+
 @menubar_plugin("edxia: edit Phases (Experimental !)")
 def phases_editor(session, data_collection):
     phases = get_phases_data(data_collection)
     if phases is None:
         phases_loader(session, data_collection)
         phases = get_phases_data(data_collection)
     if phases is not None:
@@ -55,16 +57,18 @@
 
         if dialog_result != qtw.QDialog.Accepted:
             return
         else:
             phases.update_values_from_data(dialog.results)
     return
 
+
 class PhasesEditor(qtw.QDialog):
-    """Dialog to edit phases in the Glue extension"""
+    """Dialog to edit phases in the Glue extension."""
+
     def __init__(self, phases, parent=None):
         super().__init__(parent)
 
 
         self._ui = load_ui('phases.ui', self,
             directory=os.path.dirname(__file__))
 
@@ -82,15 +86,15 @@
             if cid not in coords and cid not in derived:
                 df[cid.label] = phases[cid]
 
         self.model = EditablePandasTableModel(df, fixed_columns=None)
         self.table.setModel(self.model)
 
     def add_phase_by_formula(self):
-        """Add a phase by formula, rather than adding them by coefficients"""
+        """Add a phase by formula, rather than adding them by coefficients."""
         dialog = PhaseAddition()
         dialog_result = dialog.exec_()
 
         if dialog_result != qtw.QDialog.Accepted:
             return
 
         label, compo = dialog.results
@@ -100,28 +104,29 @@
             df.loc[empty, key] = float(value)
         df.loc[empty, "phase"] = label
 
 
     def _set_data(self):
         df = self.model.get_dataframe()
         df = df.set_index("phase")
-        self.results = PhaseData(df)
+        self.results = create_phase_data(df)
         self.results.label = PHASES_LABEL
 
     def accept(self):
-        """Return the data"""
+        """Return the data."""
         try:
             self._set_data()
         except Exception as e:
             print(repr(e))
             return self.reject()
         return super().accept()
 
+
 class PhaseAddition(qtw.QDialog):
-    """Dialog to add a phase in the Glue extension"""
+    """Dialog to add a phase in the Glue extension."""
     def __init__(self, parent=None):
         super().__init__(parent)
 
 
         self._ui = load_ui('phase_add.ui', self,
             directory=os.path.dirname(__file__))
 
@@ -130,14 +135,14 @@
     def _set_data(self):
         compo = formula_to_composition(self.phase_formula.text())
         compo = normalize_composition(compo)
         label = self.phase_label.text()
         self.results = (label, compo)
 
     def accept(self):
-        """Return the data"""
+        """Return the data."""
         try:
             self._set_data()
         except Exception as e:
             print(repr(e))
             return self.reject()
         return super().accept()
```

### Comparing `edxia-0.1.8/edxia/glue/qt/phases.ui` & `edxia-0.1.9/edxia/glue/qt/phases.ui`

 * *Files identical despite different names*

### Comparing `edxia-0.1.8/edxia/glue/qt/points_loader.py` & `edxia-0.1.9/edxia/glue/qt/points_loader.py`

 * *Files identical despite different names*

### Comparing `edxia-0.1.8/edxia/glue/qt/points_loader.ui` & `edxia-0.1.9/edxia/glue/qt/points_loader.ui`

 * *Files identical despite different names*

### Comparing `edxia-0.1.8/edxia/glue/qt/quantifier/composition.ui` & `edxia-0.1.9/edxia/glue/qt/quantifier/composition.ui`

 * *Files identical despite different names*

### Comparing `edxia-0.1.8/edxia/glue/qt/quantifier/main_quantifier.ui` & `edxia-0.1.9/edxia/glue/qt/quantifier/main_quantifier.ui`

 * *Files identical despite different names*

### Comparing `edxia-0.1.8/edxia/glue/qt/quantifier/point_fractions.ui` & `edxia-0.1.9/edxia/glue/qt/quantifier/point_fractions.ui`

 * *Files identical despite different names*

### Comparing `edxia-0.1.8/edxia/glue/qt/quantifier/s2_correlation.ui` & `edxia-0.1.9/edxia/glue/qt/quantifier/s2_correlation.ui`

 * *Files identical despite different names*

### Comparing `edxia-0.1.8/edxia/glue/qt/quantifier/surface_fractions.ui` & `edxia-0.1.9/edxia/glue/qt/quantifier/surface_fractions.ui`

 * *Files identical despite different names*

### Comparing `edxia-0.1.8/edxia/glue/qt/subset_quantifier.py` & `edxia-0.1.9/edxia/glue/qt/subset_quantifier.py`

 * *Files identical despite different names*

### Comparing `edxia-0.1.8/edxia/io/__init__.py` & `edxia-0.1.9/edxia/io/__init__.py`

 * *Files identical despite different names*

### Comparing `edxia-0.1.8/edxia/io/hdf5.py` & `edxia-0.1.9/edxia/io/hdf5.py`

 * *Files identical despite different names*

### Comparing `edxia-0.1.8/edxia/io/loader/__init__.py` & `edxia-0.1.9/edxia/io/loader/__init__.py`

 * *Files identical despite different names*

### Comparing `edxia-0.1.8/edxia/io/loader/base_loader.py` & `edxia-0.1.9/edxia/io/loader/base_loader.py`

 * *Files identical despite different names*

### Comparing `edxia-0.1.8/edxia/io/loader/default_loader.py` & `edxia-0.1.9/edxia/io/loader/default_loader.py`

 * *Files identical despite different names*

### Comparing `edxia-0.1.8/edxia/io/loader/pickle_loader.py` & `edxia-0.1.9/edxia/io/loader/pickle_loader.py`

 * *Files identical despite different names*

### Comparing `edxia-0.1.8/edxia/io/loader/stack_loader.py` & `edxia-0.1.9/edxia/io/loader/stack_loader.py`

 * *Files identical despite different names*

### Comparing `edxia-0.1.8/edxia/io/raw_io.py` & `edxia-0.1.9/edxia/io/raw_io.py`

 * *Files identical despite different names*

### Comparing `edxia-0.1.8/edxia/point_analysis/__init__.py` & `edxia-0.1.9/edxia/point_analysis/__init__.py`

 * *Files identical despite different names*

### Comparing `edxia-0.1.8/edxia/point_analysis/points.py` & `edxia-0.1.9/edxia/point_analysis/points.py`

 * *Files identical despite different names*

### Comparing `edxia-0.1.8/edxia/utils/__init__.py` & `edxia-0.1.9/edxia/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `edxia-0.1.8/edxia/utils/chemistry.py` & `edxia-0.1.9/edxia/utils/chemistry.py`

 * *Files identical despite different names*

### Comparing `edxia-0.1.8/edxia/utils/coordinates.py` & `edxia-0.1.9/edxia/utils/coordinates.py`

 * *Files identical despite different names*

### Comparing `edxia-0.1.8/edxia/utils/path.py` & `edxia-0.1.9/edxia/utils/path.py`

 * *Files identical despite different names*

### Comparing `edxia-0.1.8/edxia/utils/qt.py` & `edxia-0.1.9/edxia/utils/qt.py`

 * *Files identical despite different names*

### Comparing `edxia-0.1.8/edxia.egg-info/PKG-INFO` & `edxia-0.1.9/edxia.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: edxia
-Version: 0.1.8
+Version: 0.1.9
 Summary: SEM-BSE-EDS image analysis
 Home-page: https://bitbucket.org/specmicp/edxia/
 Author: Fabien Georget
-Author-email: Fabien.georget@epfl.ch
+Author-email: georget@ibac.rwth-aachen.de
 License: BSD
 Project-URL: Funding, https://lmc.epfl.ch/
 Description: # edxia
         
         Analyse SEM-BSE and SEM-EDS maps.
         
         [Scanning Electron Microscopy (SEM)](https://en.wikipedia.org/wiki/Scanning_electron_microscope "Wikipedia link") coupled with [Energy-Dispersive Spectroscopy (EDX)](https://en.wikipedia.org/wiki/Energy-dispersive_X-ray_spectroscopy "wikipedia link") is an imaging technique used in the cement community to learn more about the microstructure of the material.
@@ -48,10 +48,12 @@
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Chemistry
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.4, <4
 Description-Content-Type: text/markdown
 Provides-Extra: jointBilateral
```

### Comparing `edxia-0.1.8/edxia.egg-info/SOURCES.txt` & `edxia-0.1.9/edxia.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `edxia-0.1.8/setup.py` & `edxia-0.1.9/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,43 +6,46 @@
 
 # Get the long description from the README file
 with open(path.join(here, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='edxia',
-    version='0.1.8',
+    version='0.1.9',
     description='SEM-BSE-EDS image analysis',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://bitbucket.org/specmicp/edxia/',
     author='Fabien Georget',
-    author_email='Fabien.georget@epfl.ch',
+    author_email='georget@ibac.rwth-aachen.de',
     license='BSD',
     classifiers=[
         'Development Status :: 3 - Alpha',
 
         'Intended Audience :: Science/Research',
         'Topic :: Scientific/Engineering :: Chemistry',
         'Topic :: Scientific/Engineering :: Visualization',
         'License :: OSI Approved :: BSD License',
 
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
+        'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
     ],
     keywords='SEM EDS BSE visualization',  # Optional
     packages=find_packages(exclude=['contrib', 'docs', 'tests']),
     python_requires='>=3.4, <4',
     install_requires=[
             'glueviz>=0.15',
             'pandas',
             'py_expression_eval',
             'scikit-image',
-            'scikit-learn'
+            'scikit-learn',
+            'numba'
             ],
 
     extras_require={
         "jointBilateral": ["opencv-python"]
     },
 
     package_data={'': ['*.ui'],
```

