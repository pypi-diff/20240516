# Comparing `tmp/biomedisa-2024.5.20.tar.gz` & `tmp/biomedisa-2024.5.21.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "biomedisa-2024.5.20.tar", last modified: Thu May 16 01:32:53 2024, max compression
+gzip compressed data, was "biomedisa-2024.5.21.tar", last modified: Thu May 16 04:50:01 2024, max compression
```

## Comparing `biomedisa-2024.5.20.tar` & `biomedisa-2024.5.21.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxrwxr-x   0 philipp   (1000) philipp   (1000)        0 2024-05-16 01:32:53.216466 biomedisa-2024.5.20/
--rwxrwxr-x   0 philipp   (1000) philipp   (1000)    14152 2023-06-09 06:17:35.000000 biomedisa-2024.5.20/LICENSE
--rw-r--r--   0 philipp   (1000) philipp   (1000)    10677 2024-05-16 01:32:53.216466 biomedisa-2024.5.20/PKG-INFO
--rwxrwxr-x   0 philipp   (1000) philipp   (1000)    10069 2024-05-15 23:50:44.000000 biomedisa-2024.5.20/README.md
--rw-rw-r--   0 philipp   (1000) philipp   (1000)      664 2024-05-16 01:26:42.000000 biomedisa-2024.5.20/pyproject.toml
--rw-rw-r--   0 philipp   (1000) philipp   (1000)       38 2024-05-16 01:32:53.216466 biomedisa-2024.5.20/setup.cfg
-drwxrwxr-x   0 philipp   (1000) philipp   (1000)        0 2024-05-16 01:32:53.216466 biomedisa-2024.5.20/src/
-drwxrwxr-x   0 philipp   (1000) philipp   (1000)        0 2024-05-16 01:32:53.216466 biomedisa-2024.5.20/src/biomedisa/
--rwxrwxr-x   0 philipp   (1000) philipp   (1000)     1538 2024-05-16 00:26:26.000000 biomedisa-2024.5.20/src/biomedisa/__init__.py
--rwxrwxr-x   0 philipp   (1000) philipp   (1000)      536 2024-05-08 09:06:16.000000 biomedisa-2024.5.20/src/biomedisa/__main__.py
--rwxrwxr-x   0 philipp   (1000) philipp   (1000)    27064 2024-05-16 00:15:17.000000 biomedisa-2024.5.20/src/biomedisa/deeplearning.py
-drwxrwxr-x   0 philipp   (1000) philipp   (1000)        0 2024-05-16 01:32:53.216466 biomedisa-2024.5.20/src/biomedisa/features/
--rwxrwxr-x   0 philipp   (1000) philipp   (1000)    12770 2024-05-16 00:17:46.000000 biomedisa-2024.5.20/src/biomedisa/features/DataGenerator.py
--rwxrwxr-x   0 philipp   (1000) philipp   (1000)     5454 2024-05-16 00:17:55.000000 biomedisa-2024.5.20/src/biomedisa/features/DataGeneratorCrop.py
--rwxrwxr-x   0 philipp   (1000) philipp   (1000)     4074 2024-05-16 00:30:03.000000 biomedisa-2024.5.20/src/biomedisa/features/PredictDataGenerator.py
--rwxrwxr-x   0 philipp   (1000) philipp   (1000)     3431 2024-05-16 00:30:13.000000 biomedisa-2024.5.20/src/biomedisa/features/PredictDataGeneratorCrop.py
--rwxrwxr-x   0 philipp   (1000) philipp   (1000)        0 2023-06-09 06:17:35.000000 biomedisa-2024.5.20/src/biomedisa/features/__init__.py
--rwxrwxr-x   0 philipp   (1000) philipp   (1000)    18096 2024-05-16 00:12:55.000000 biomedisa-2024.5.20/src/biomedisa/features/active_contour.py
-drwxrwxr-x   0 philipp   (1000) philipp   (1000)        0 2024-05-16 01:32:53.216466 biomedisa-2024.5.20/src/biomedisa/features/amira_to_np/
--rwxrwxr-x   0 philipp   (1000) philipp   (1000)        0 2023-06-09 06:17:35.000000 biomedisa-2024.5.20/src/biomedisa/features/amira_to_np/__init__.py
--rwxrwxr-x   0 philipp   (1000) philipp   (1000)    32618 2023-06-09 06:17:35.000000 biomedisa-2024.5.20/src/biomedisa/features/amira_to_np/amira_data_stream.py
--rwxrwxr-x   0 philipp   (1000) philipp   (1000)    14324 2023-06-09 06:17:35.000000 biomedisa-2024.5.20/src/biomedisa/features/amira_to_np/amira_grammar.py
--rwxrwxr-x   0 philipp   (1000) philipp   (1000)    11553 2023-06-09 06:17:35.000000 biomedisa-2024.5.20/src/biomedisa/features/amira_to_np/amira_header.py
--rwxrwxr-x   0 philipp   (1000) philipp   (1000)     2218 2023-06-09 06:17:35.000000 biomedisa-2024.5.20/src/biomedisa/features/amira_to_np/amira_helper.py
--rwxrwxr-x   0 philipp   (1000) philipp   (1000)     6537 2024-05-16 00:13:13.000000 biomedisa-2024.5.20/src/biomedisa/features/assd.py
--rwxrwxr-x   0 philipp   (1000) philipp   (1000)    32250 2024-05-16 00:14:20.000000 biomedisa-2024.5.20/src/biomedisa/features/biomedisa_helper.py
--rwxrwxr-x   0 philipp   (1000) philipp   (1000)    13001 2024-05-16 00:16:37.000000 biomedisa-2024.5.20/src/biomedisa/features/create_slices.py
--rwxrwxr-x   0 philipp   (1000) philipp   (1000)    24533 2024-05-16 00:17:17.000000 biomedisa-2024.5.20/src/biomedisa/features/crop_helper.py
--rwxrwxr-x   0 philipp   (1000) philipp   (1000)     7049 2024-05-16 00:17:36.000000 biomedisa-2024.5.20/src/biomedisa/features/curvop_numba.py
--rw-rw-r--   0 philipp   (1000) philipp   (1000)     8942 2024-05-16 00:19:36.000000 biomedisa-2024.5.20/src/biomedisa/features/django_env.py
--rwxrwxr-x   0 philipp   (1000) philipp   (1000)    50250 2024-05-16 00:20:22.000000 biomedisa-2024.5.20/src/biomedisa/features/keras_helper.py
--rwxrwxr-x   0 philipp   (1000) philipp   (1000)     7406 2024-05-16 00:20:46.000000 biomedisa-2024.5.20/src/biomedisa/features/nc_reader.py
--rw-rw-r--   0 philipp   (1000) philipp   (1000)     2545 2024-05-16 00:29:46.000000 biomedisa-2024.5.20/src/biomedisa/features/pid.py
--rw-rw-r--   0 philipp   (1000) philipp   (1000)    11091 2024-05-16 00:31:34.000000 biomedisa-2024.5.20/src/biomedisa/features/process_image.py
--rwxrwxr-x   0 philipp   (1000) philipp   (1000)     3275 2024-05-16 00:31:56.000000 biomedisa-2024.5.20/src/biomedisa/features/pycuda_test.py
-drwxrwxr-x   0 philipp   (1000) philipp   (1000)        0 2024-05-16 01:32:53.216466 biomedisa-2024.5.20/src/biomedisa/features/random_walk/
--rwxrwxr-x   0 philipp   (1000) philipp   (1000)        0 2023-06-09 06:17:35.000000 biomedisa-2024.5.20/src/biomedisa/features/random_walk/__init__.py
--rwxrwxr-x   0 philipp   (1000) philipp   (1000)     7191 2024-05-16 00:09:35.000000 biomedisa-2024.5.20/src/biomedisa/features/random_walk/gpu_kernels.py
--rwxrwxr-x   0 philipp   (1000) philipp   (1000)    32917 2024-05-16 00:10:02.000000 biomedisa-2024.5.20/src/biomedisa/features/random_walk/pycuda_large.py
--rwxrwxr-x   0 philipp   (1000) philipp   (1000)    30677 2024-05-16 00:10:19.000000 biomedisa-2024.5.20/src/biomedisa/features/random_walk/pycuda_large_allx.py
--rwxrwxr-x   0 philipp   (1000) philipp   (1000)    15786 2024-05-16 00:09:10.000000 biomedisa-2024.5.20/src/biomedisa/features/random_walk/pycuda_small.py
--rwxrwxr-x   0 philipp   (1000) philipp   (1000)    18225 2024-05-16 00:10:42.000000 biomedisa-2024.5.20/src/biomedisa/features/random_walk/pycuda_small_allx.py
--rwxrwxr-x   0 philipp   (1000) philipp   (1000)    31015 2024-05-16 00:10:54.000000 biomedisa-2024.5.20/src/biomedisa/features/random_walk/pyopencl_large.py
--rwxrwxr-x   0 philipp   (1000) philipp   (1000)    17068 2024-05-16 00:11:11.000000 biomedisa-2024.5.20/src/biomedisa/features/random_walk/pyopencl_small.py
--rwxrwxr-x   0 philipp   (1000) philipp   (1000)    19805 2024-05-16 00:08:50.000000 biomedisa-2024.5.20/src/biomedisa/features/random_walk/rw_large.py
--rwxrwxr-x   0 philipp   (1000) philipp   (1000)    14881 2024-05-16 00:08:13.000000 biomedisa-2024.5.20/src/biomedisa/features/random_walk/rw_small.py
--rwxrwxr-x   0 philipp   (1000) philipp   (1000)    16756 2024-05-16 00:33:15.000000 biomedisa-2024.5.20/src/biomedisa/features/remove_outlier.py
--rwxrwxr-x   0 philipp   (1000) philipp   (1000)     8926 2024-05-16 00:39:38.000000 biomedisa-2024.5.20/src/biomedisa/features/split_volume.py
--rwxrwxr-x   0 philipp   (1000) philipp   (1000)    17253 2024-05-16 00:15:01.000000 biomedisa-2024.5.20/src/biomedisa/interpolation.py
--rwxrwxr-x   0 philipp   (1000) philipp   (1000)    15819 2024-05-16 00:37:59.000000 biomedisa-2024.5.20/src/biomedisa/mesh.py
-drwxrwxr-x   0 philipp   (1000) philipp   (1000)        0 2024-05-16 01:32:53.216466 biomedisa-2024.5.20/src/biomedisa.egg-info/
--rw-r--r--   0 philipp   (1000) philipp   (1000)    10677 2024-05-16 01:32:53.000000 biomedisa-2024.5.20/src/biomedisa.egg-info/PKG-INFO
--rw-rw-r--   0 philipp   (1000) philipp   (1000)     1832 2024-05-16 01:32:53.000000 biomedisa-2024.5.20/src/biomedisa.egg-info/SOURCES.txt
--rw-rw-r--   0 philipp   (1000) philipp   (1000)        1 2024-05-16 01:32:53.000000 biomedisa-2024.5.20/src/biomedisa.egg-info/dependency_links.txt
--rw-rw-r--   0 philipp   (1000) philipp   (1000)       10 2024-05-16 01:32:53.000000 biomedisa-2024.5.20/src/biomedisa.egg-info/top_level.txt
+drwxrwxr-x   0 philipp   (1000) philipp   (1000)        0 2024-05-16 04:50:01.326235 biomedisa-2024.5.21/
+-rwxrwxr-x   0 philipp   (1000) philipp   (1000)    14152 2023-06-09 06:17:35.000000 biomedisa-2024.5.21/LICENSE
+-rw-r--r--   0 philipp   (1000) philipp   (1000)    10465 2024-05-16 04:50:01.326235 biomedisa-2024.5.21/PKG-INFO
+-rwxrwxr-x   0 philipp   (1000) philipp   (1000)     9857 2024-05-16 04:44:50.000000 biomedisa-2024.5.21/README.md
+-rw-rw-r--   0 philipp   (1000) philipp   (1000)      664 2024-05-16 04:49:09.000000 biomedisa-2024.5.21/pyproject.toml
+-rw-rw-r--   0 philipp   (1000) philipp   (1000)       38 2024-05-16 04:50:01.326235 biomedisa-2024.5.21/setup.cfg
+drwxrwxr-x   0 philipp   (1000) philipp   (1000)        0 2024-05-16 04:50:01.322235 biomedisa-2024.5.21/src/
+drwxrwxr-x   0 philipp   (1000) philipp   (1000)        0 2024-05-16 04:50:01.322235 biomedisa-2024.5.21/src/biomedisa/
+-rwxrwxr-x   0 philipp   (1000) philipp   (1000)     1526 2024-05-16 02:12:35.000000 biomedisa-2024.5.21/src/biomedisa/__init__.py
+-rwxrwxr-x   0 philipp   (1000) philipp   (1000)      536 2024-05-08 09:06:16.000000 biomedisa-2024.5.21/src/biomedisa/__main__.py
+-rwxrwxr-x   0 philipp   (1000) philipp   (1000)    27064 2024-05-16 00:15:17.000000 biomedisa-2024.5.21/src/biomedisa/deeplearning.py
+drwxrwxr-x   0 philipp   (1000) philipp   (1000)        0 2024-05-16 04:50:01.326235 biomedisa-2024.5.21/src/biomedisa/features/
+-rwxrwxr-x   0 philipp   (1000) philipp   (1000)    12770 2024-05-16 00:17:46.000000 biomedisa-2024.5.21/src/biomedisa/features/DataGenerator.py
+-rwxrwxr-x   0 philipp   (1000) philipp   (1000)     5454 2024-05-16 00:17:55.000000 biomedisa-2024.5.21/src/biomedisa/features/DataGeneratorCrop.py
+-rwxrwxr-x   0 philipp   (1000) philipp   (1000)     4074 2024-05-16 00:30:03.000000 biomedisa-2024.5.21/src/biomedisa/features/PredictDataGenerator.py
+-rwxrwxr-x   0 philipp   (1000) philipp   (1000)     3431 2024-05-16 00:30:13.000000 biomedisa-2024.5.21/src/biomedisa/features/PredictDataGeneratorCrop.py
+-rwxrwxr-x   0 philipp   (1000) philipp   (1000)        0 2023-06-09 06:17:35.000000 biomedisa-2024.5.21/src/biomedisa/features/__init__.py
+-rwxrwxr-x   0 philipp   (1000) philipp   (1000)    18096 2024-05-16 00:12:55.000000 biomedisa-2024.5.21/src/biomedisa/features/active_contour.py
+drwxrwxr-x   0 philipp   (1000) philipp   (1000)        0 2024-05-16 04:50:01.326235 biomedisa-2024.5.21/src/biomedisa/features/amira_to_np/
+-rwxrwxr-x   0 philipp   (1000) philipp   (1000)        0 2023-06-09 06:17:35.000000 biomedisa-2024.5.21/src/biomedisa/features/amira_to_np/__init__.py
+-rwxrwxr-x   0 philipp   (1000) philipp   (1000)    32618 2023-06-09 06:17:35.000000 biomedisa-2024.5.21/src/biomedisa/features/amira_to_np/amira_data_stream.py
+-rwxrwxr-x   0 philipp   (1000) philipp   (1000)    14324 2023-06-09 06:17:35.000000 biomedisa-2024.5.21/src/biomedisa/features/amira_to_np/amira_grammar.py
+-rwxrwxr-x   0 philipp   (1000) philipp   (1000)    11553 2023-06-09 06:17:35.000000 biomedisa-2024.5.21/src/biomedisa/features/amira_to_np/amira_header.py
+-rwxrwxr-x   0 philipp   (1000) philipp   (1000)     2218 2023-06-09 06:17:35.000000 biomedisa-2024.5.21/src/biomedisa/features/amira_to_np/amira_helper.py
+-rwxrwxr-x   0 philipp   (1000) philipp   (1000)     6537 2024-05-16 00:13:13.000000 biomedisa-2024.5.21/src/biomedisa/features/assd.py
+-rwxrwxr-x   0 philipp   (1000) philipp   (1000)    32250 2024-05-16 00:14:20.000000 biomedisa-2024.5.21/src/biomedisa/features/biomedisa_helper.py
+-rwxrwxr-x   0 philipp   (1000) philipp   (1000)    13001 2024-05-16 00:16:37.000000 biomedisa-2024.5.21/src/biomedisa/features/create_slices.py
+-rwxrwxr-x   0 philipp   (1000) philipp   (1000)    24533 2024-05-16 00:17:17.000000 biomedisa-2024.5.21/src/biomedisa/features/crop_helper.py
+-rwxrwxr-x   0 philipp   (1000) philipp   (1000)     7049 2024-05-16 00:17:36.000000 biomedisa-2024.5.21/src/biomedisa/features/curvop_numba.py
+-rw-rw-r--   0 philipp   (1000) philipp   (1000)     8942 2024-05-16 00:19:36.000000 biomedisa-2024.5.21/src/biomedisa/features/django_env.py
+-rwxrwxr-x   0 philipp   (1000) philipp   (1000)    50250 2024-05-16 00:20:22.000000 biomedisa-2024.5.21/src/biomedisa/features/keras_helper.py
+-rwxrwxr-x   0 philipp   (1000) philipp   (1000)     7406 2024-05-16 00:20:46.000000 biomedisa-2024.5.21/src/biomedisa/features/nc_reader.py
+-rw-rw-r--   0 philipp   (1000) philipp   (1000)     2545 2024-05-16 00:29:46.000000 biomedisa-2024.5.21/src/biomedisa/features/pid.py
+-rw-rw-r--   0 philipp   (1000) philipp   (1000)    11091 2024-05-16 00:31:34.000000 biomedisa-2024.5.21/src/biomedisa/features/process_image.py
+-rwxrwxr-x   0 philipp   (1000) philipp   (1000)     3275 2024-05-16 00:31:56.000000 biomedisa-2024.5.21/src/biomedisa/features/pycuda_test.py
+drwxrwxr-x   0 philipp   (1000) philipp   (1000)        0 2024-05-16 04:50:01.326235 biomedisa-2024.5.21/src/biomedisa/features/random_walk/
+-rwxrwxr-x   0 philipp   (1000) philipp   (1000)        0 2023-06-09 06:17:35.000000 biomedisa-2024.5.21/src/biomedisa/features/random_walk/__init__.py
+-rwxrwxr-x   0 philipp   (1000) philipp   (1000)     7191 2024-05-16 00:09:35.000000 biomedisa-2024.5.21/src/biomedisa/features/random_walk/gpu_kernels.py
+-rwxrwxr-x   0 philipp   (1000) philipp   (1000)    32917 2024-05-16 00:10:02.000000 biomedisa-2024.5.21/src/biomedisa/features/random_walk/pycuda_large.py
+-rwxrwxr-x   0 philipp   (1000) philipp   (1000)    30677 2024-05-16 00:10:19.000000 biomedisa-2024.5.21/src/biomedisa/features/random_walk/pycuda_large_allx.py
+-rwxrwxr-x   0 philipp   (1000) philipp   (1000)    15786 2024-05-16 00:09:10.000000 biomedisa-2024.5.21/src/biomedisa/features/random_walk/pycuda_small.py
+-rwxrwxr-x   0 philipp   (1000) philipp   (1000)    18225 2024-05-16 00:10:42.000000 biomedisa-2024.5.21/src/biomedisa/features/random_walk/pycuda_small_allx.py
+-rwxrwxr-x   0 philipp   (1000) philipp   (1000)    31015 2024-05-16 00:10:54.000000 biomedisa-2024.5.21/src/biomedisa/features/random_walk/pyopencl_large.py
+-rwxrwxr-x   0 philipp   (1000) philipp   (1000)    17068 2024-05-16 00:11:11.000000 biomedisa-2024.5.21/src/biomedisa/features/random_walk/pyopencl_small.py
+-rwxrwxr-x   0 philipp   (1000) philipp   (1000)    19805 2024-05-16 00:08:50.000000 biomedisa-2024.5.21/src/biomedisa/features/random_walk/rw_large.py
+-rwxrwxr-x   0 philipp   (1000) philipp   (1000)    14881 2024-05-16 00:08:13.000000 biomedisa-2024.5.21/src/biomedisa/features/random_walk/rw_small.py
+-rwxrwxr-x   0 philipp   (1000) philipp   (1000)    16756 2024-05-16 00:33:15.000000 biomedisa-2024.5.21/src/biomedisa/features/remove_outlier.py
+-rwxrwxr-x   0 philipp   (1000) philipp   (1000)     8917 2024-05-16 04:15:45.000000 biomedisa-2024.5.21/src/biomedisa/features/split_volume.py
+-rwxrwxr-x   0 philipp   (1000) philipp   (1000)    17253 2024-05-16 00:15:01.000000 biomedisa-2024.5.21/src/biomedisa/interpolation.py
+-rwxrwxr-x   0 philipp   (1000) philipp   (1000)    15819 2024-05-16 00:37:59.000000 biomedisa-2024.5.21/src/biomedisa/mesh.py
+drwxrwxr-x   0 philipp   (1000) philipp   (1000)        0 2024-05-16 04:50:01.326235 biomedisa-2024.5.21/src/biomedisa.egg-info/
+-rw-r--r--   0 philipp   (1000) philipp   (1000)    10465 2024-05-16 04:50:01.000000 biomedisa-2024.5.21/src/biomedisa.egg-info/PKG-INFO
+-rw-rw-r--   0 philipp   (1000) philipp   (1000)     1832 2024-05-16 04:50:01.000000 biomedisa-2024.5.21/src/biomedisa.egg-info/SOURCES.txt
+-rw-rw-r--   0 philipp   (1000) philipp   (1000)        1 2024-05-16 04:50:01.000000 biomedisa-2024.5.21/src/biomedisa.egg-info/dependency_links.txt
+-rw-rw-r--   0 philipp   (1000) philipp   (1000)       10 2024-05-16 04:50:01.000000 biomedisa-2024.5.21/src/biomedisa.egg-info/top_level.txt
```

### Comparing `biomedisa-2024.5.20/LICENSE` & `biomedisa-2024.5.21/LICENSE`

 * *Files identical despite different names*

### Comparing `biomedisa-2024.5.20/PKG-INFO` & `biomedisa-2024.5.21/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,60 +1,49 @@
-Metadata-Version: 2.1
-Name: biomedisa
-Version: 2024.5.20
-Summary: Segmentation of 3D volumetric image data
-Author: Philipp Lösel
-Author-email: philipp.loesel@anu.edu.au
-Project-URL: Homepage, https://biomedisa.info
-Project-URL: Issues, https://github.com/biomedisa/biomedisa/issues
-Project-URL: GitHub, https://github.com/biomedisa/biomedisa
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: European Union Public Licence 1.2 (EUPL 1.2)
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 [![biomedisa](https://raw.githubusercontent.com/biomedisa/biomedisa/master/biomedisa_app/static/biomedisa_logo.svg)](https://biomedisa.info)
 -----------
 - [Overview](#overview)
 - [Hardware Requirements](#hardware-requirements)
 - [Installation (command-line based)](#installation-command-line-based)
 - [Installation (browser based)](#installation-browser-based)
 - [Download Data](#download-data)
+- [Revisions](#revisions)
 - [Smart Interpolation](#smart-interpolation)
 - [Deep Learning](#deep-learning)
 - [Biomedisa Features](#biomedisa-features)
-- [Update Biomedisa](#update-biomedisa)
-- [Releases](#releases)
 - [Authors](#authors)
 - [FAQ](#faq)
 - [Citation](#citation)
 - [License](#license)
 
-# Overview
+## Overview
 Biomedisa (https://biomedisa.info) is a free and easy-to-use open-source application for segmenting large volumetric images, e.g. CT and MRI scans, developed at [The Australian National University CTLab](https://ctlab.anu.edu.au/). Biomedisa's semi-automated segmentation is based on a smart interpolation of sparsely pre-segmented slices, taking into account the complete underlying image data. In addition, Biomedisa enables deep learning for the fully automated segmentation of series of similar samples. It can be used in combination with segmentation tools such as Amira/Avizo, ImageJ/Fiji and 3D Slicer. If you are using Biomedisa or the data for your research please cite: Lösel, P.D. et al. [Introducing Biomedisa as an open-source online platform for biomedical image segmentation.](https://www.nature.com/articles/s41467-020-19303-w) *Nat. Commun.* **11**, 5577 (2020).
 
-# Hardware Requirements
+## Hardware Requirements
 + One or more NVIDIA GPUs with compute capability 3.0 or higher or an Intel CPU.
 
-# Installation (command-line based)
+## Installation (command-line based)
 + [Ubuntu 22.04 + CUDA + GPU (recommended)](https://github.com/biomedisa/biomedisa/blob/master/README/ubuntu2204_cuda11.8_gpu_cli.md)
 + [Ubuntu 22.04 + OpenCL + CPU (smart interpolation only and very slow)](https://github.com/biomedisa/biomedisa/blob/master/README/ubuntu2204_opencl_cpu_cli.md)
 + [Windows 10 + CUDA + GPU (recommended)](https://github.com/biomedisa/biomedisa/blob/master/README/windows10_cuda_gpu_cli.md)
 + [Windows 10 + OpenCL + GPU (easy to install but lacks features like allaxis, smoothing, uncertainty, optimized GPU memory usage)](https://github.com/biomedisa/biomedisa/blob/master/README/windows10_opencl_gpu_cli.md)
 + [Windows 10 + OpenCL + CPU (very slow)](https://github.com/biomedisa/biomedisa/blob/master/README/windows10_opencl_cpu_cli.md)
 
-# Installation (browser based)
+## Installation (browser based)
 + [Ubuntu 22.04](https://github.com/biomedisa/biomedisa/blob/master/README/ubuntu2204_cuda11.8.md)
 
-# Download Data
+## Download Data
 + Download the data from our [gallery](https://biomedisa.info/gallery/)
 
-# Smart Interpolation
+## Revisions
+2024.05.21
++ Pip is the preferred installation method
++ Commands, module names and imports have been changed to conform to the Pip standard
++ For versions <=2023.09.1 please check [README](https://github.com/biomedisa/biomedisa/blob/master/README/deprecated/README_2023.09.1.md)
+
+## Smart Interpolation
 + [Parameters and Examples](https://github.com/biomedisa/biomedisa/blob/master/README/smart_interpolation.md)
 
 #### Python example
 ```python
 from biomedisa.features.biomedisa_helper import load_data, save_data
 from biomedisa.interpolation import smart_interpolation
 
@@ -73,17 +62,20 @@
 save_data('Downloads/final.trigonopterus.am', regular_result, header=header)
 save_data('Downloads/final.trigonopterus.smooth.am', smooth_result, header=header)
 ```
 
 #### Command-line based
 ```
 python -m biomedisa.interpolation C:\Users\%USERNAME%\Downloads\tumor.tif C:\Users\%USERNAME%\Downloads\labels.tumor.tif
+
+# if pre-segmentation is not exclusively in the XY plane
+python -m biomedisa.interpolation C:\Users\%USERNAME%\Downloads\tumor.tif C:\Users\%USERNAME%\Downloads\labels.tumor.tif --allaxis
 ```
 
-# Deep Learning
+## Deep Learning
 + [Parameters and Examples](https://github.com/biomedisa/biomedisa/blob/master/README/deep_learning.md)
 
 #### Python example (training)
 ```python
 from biomedisa.features.biomedisa_helper import load_data
 from biomedisa.deeplearning import deep_learning
 
@@ -111,18 +103,18 @@
         val_img_data=val_img_data, val_label_data=val_label_data,
         header=header, extension=ext, path_to_model='honeybees.h5')
 ```
 
 #### Command-line based (training)
 ```
 # start training with a batch size of 12
-python -m biomedisa.deeplearning C:\Users\%USERNAME%\Downloads\training_heart C:\Users\%USERNAME%\Downloads\training_heart_labels -t -bs 12
+python -m biomedisa.deeplearning C:\Users\%USERNAME%\Downloads\training_heart C:\Users\%USERNAME%\Downloads\training_heart_labels -t -bs=12
 
 # validation (optional)
-python -m biomedisa.deeplearning C:\Users\%USERNAME%\Downloads\training_heart C:\Users\%USERNAME%\Downloads\training_heart_labels -t -vi C:\Users\%USERNAME%\Downloads\val_img -vl C:\Users\%USERNAME%\Downloads\val_labels
+python -m biomedisa.deeplearning C:\Users\%USERNAME%\Downloads\training_heart C:\Users\%USERNAME%\Downloads\training_heart_labels -t -vi=C:\Users\%USERNAME%\Downloads\val_img -vl=C:\Users\%USERNAME%\Downloads\val_labels
 ```
 If running into ResourceExhaustedError due to out of memory (OOM), try to use smaller batch size.
 
 #### Python example (prediction)
 ```python
 from biomedisa.features.biomedisa_helper import load_data, save_data
 from biomedisa.deeplearning import deep_learning
@@ -139,15 +131,15 @@
 ```
 
 #### Command-line based (prediction)
 ```
 python -m biomedisa.deeplearning C:\Users\%USERNAME%\Downloads\testing_axial_crop_pat13.nii.gz C:\Users\%USERNAME%\Downloads\heart.h5 -p
 ```
 
-# Biomedisa Features
+## Biomedisa Features
 
 #### Load and save data (such as Amira Mesh, TIFF, NRRD, NIfTI or DICOM)
 ```python
 from biomedisa.features.biomedisa_helper import load_data, save_data
 
 # load data as numpy array
 # for DICOM, PNG files, or similar formats, 'path_to_data' must reference
@@ -218,59 +210,34 @@
 #### Accuracy assessment
 ```python
 from biomedisa.features.biomedisa_helper import Dice_score, ASSD
 dice = Dice_score(ground_truth, result)
 assd = ASSD(ground_truth, result)
 ```
 
-# Update Biomedisa
-If you installed Biomedisa via Pip
-```
-pip install --upgrade biomedisa
-```
-If you used `git clone`, change to the Biomedisa directory and make a pull request
-```
-cd git/biomedisa
-git pull
-```
-
-If you installed the browser based version of Biomedisa (including MySQL database), you also need to update the database
-```
-python manage.py migrate
-```
-
-If you installed an [Apache Server](https://github.com/biomedisa/biomedisa/blob/master/README/APACHE_SERVER.md), you need to restart the server
-```
-sudo service apache2 restart
-```
-
-# Releases
-
-For the versions available, see the [list of releases](https://github.com/biomedisa/biomedisa/releases). 
-
-# Authors
+## Authors
 
 * **Philipp D. Lösel**
 
 See also the list of [contributors](https://github.com/biomedisa/biomedisa/blob/master/credits.md) who participated in this project.
 
-# FAQ
+## FAQ
 Frequently asked questions can be found at: https://biomedisa.info/faq/.
 
-# Citation
+## Citation
 
 If you use Biomedisa or the data, please cite the following paper:
 
 `Lösel, P.D. et al. Introducing Biomedisa as an open-source online platform for biomedical image segmentation. Nat. Commun. 11, 5577 (2020).` https://doi.org/10.1038/s41467-020-19303-w
 
 If you use Biomedisa's Deep Learning, you may also cite:
 
 `Lösel, P.D. et al. Natural variability in bee brain size and symmetry revealed by micro-CT imaging and deep learning. PLoS Comput. Biol. 19, e1011529 (2023).` https://doi.org/10.1371/journal.pcbi.1011529
 
 If you use Biomedisa's Smart Interpolation, you can also cite the initial description of this method:
 
 `Lösel, P. & Heuveline, V. Enhancing a diffusion algorithm for 4D image segmentation using local information. Proc. SPIE 9784, 97842L (2016).` https://doi.org/10.1117/12.2216202
 
-# License
+## License
 
 This project is covered under the **EUROPEAN UNION PUBLIC LICENCE v. 1.2 (EUPL)**.
```

### Comparing `biomedisa-2024.5.20/README.md` & `biomedisa-2024.5.21/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,44 +1,65 @@
+Metadata-Version: 2.1
+Name: biomedisa
+Version: 2024.5.21
+Summary: Segmentation of 3D volumetric image data
+Author: Philipp Lösel
+Author-email: philipp.loesel@anu.edu.au
+Project-URL: Homepage, https://biomedisa.info
+Project-URL: Issues, https://github.com/biomedisa/biomedisa/issues
+Project-URL: GitHub, https://github.com/biomedisa/biomedisa
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: European Union Public Licence 1.2 (EUPL 1.2)
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 [![biomedisa](https://raw.githubusercontent.com/biomedisa/biomedisa/master/biomedisa_app/static/biomedisa_logo.svg)](https://biomedisa.info)
 -----------
 - [Overview](#overview)
 - [Hardware Requirements](#hardware-requirements)
 - [Installation (command-line based)](#installation-command-line-based)
 - [Installation (browser based)](#installation-browser-based)
 - [Download Data](#download-data)
+- [Revisions](#revisions)
 - [Smart Interpolation](#smart-interpolation)
 - [Deep Learning](#deep-learning)
 - [Biomedisa Features](#biomedisa-features)
-- [Update Biomedisa](#update-biomedisa)
-- [Releases](#releases)
 - [Authors](#authors)
 - [FAQ](#faq)
 - [Citation](#citation)
 - [License](#license)
 
-# Overview
+## Overview
 Biomedisa (https://biomedisa.info) is a free and easy-to-use open-source application for segmenting large volumetric images, e.g. CT and MRI scans, developed at [The Australian National University CTLab](https://ctlab.anu.edu.au/). Biomedisa's semi-automated segmentation is based on a smart interpolation of sparsely pre-segmented slices, taking into account the complete underlying image data. In addition, Biomedisa enables deep learning for the fully automated segmentation of series of similar samples. It can be used in combination with segmentation tools such as Amira/Avizo, ImageJ/Fiji and 3D Slicer. If you are using Biomedisa or the data for your research please cite: Lösel, P.D. et al. [Introducing Biomedisa as an open-source online platform for biomedical image segmentation.](https://www.nature.com/articles/s41467-020-19303-w) *Nat. Commun.* **11**, 5577 (2020).
 
-# Hardware Requirements
+## Hardware Requirements
 + One or more NVIDIA GPUs with compute capability 3.0 or higher or an Intel CPU.
 
-# Installation (command-line based)
+## Installation (command-line based)
 + [Ubuntu 22.04 + CUDA + GPU (recommended)](https://github.com/biomedisa/biomedisa/blob/master/README/ubuntu2204_cuda11.8_gpu_cli.md)
 + [Ubuntu 22.04 + OpenCL + CPU (smart interpolation only and very slow)](https://github.com/biomedisa/biomedisa/blob/master/README/ubuntu2204_opencl_cpu_cli.md)
 + [Windows 10 + CUDA + GPU (recommended)](https://github.com/biomedisa/biomedisa/blob/master/README/windows10_cuda_gpu_cli.md)
 + [Windows 10 + OpenCL + GPU (easy to install but lacks features like allaxis, smoothing, uncertainty, optimized GPU memory usage)](https://github.com/biomedisa/biomedisa/blob/master/README/windows10_opencl_gpu_cli.md)
 + [Windows 10 + OpenCL + CPU (very slow)](https://github.com/biomedisa/biomedisa/blob/master/README/windows10_opencl_cpu_cli.md)
 
-# Installation (browser based)
+## Installation (browser based)
 + [Ubuntu 22.04](https://github.com/biomedisa/biomedisa/blob/master/README/ubuntu2204_cuda11.8.md)
 
-# Download Data
+## Download Data
 + Download the data from our [gallery](https://biomedisa.info/gallery/)
 
-# Smart Interpolation
+## Revisions
+2024.05.21
++ Pip is the preferred installation method
++ Commands, module names and imports have been changed to conform to the Pip standard
++ For versions <=2023.09.1 please check [README](https://github.com/biomedisa/biomedisa/blob/master/README/deprecated/README_2023.09.1.md)
+
+## Smart Interpolation
 + [Parameters and Examples](https://github.com/biomedisa/biomedisa/blob/master/README/smart_interpolation.md)
 
 #### Python example
 ```python
 from biomedisa.features.biomedisa_helper import load_data, save_data
 from biomedisa.interpolation import smart_interpolation
 
@@ -57,17 +78,20 @@
 save_data('Downloads/final.trigonopterus.am', regular_result, header=header)
 save_data('Downloads/final.trigonopterus.smooth.am', smooth_result, header=header)
 ```
 
 #### Command-line based
 ```
 python -m biomedisa.interpolation C:\Users\%USERNAME%\Downloads\tumor.tif C:\Users\%USERNAME%\Downloads\labels.tumor.tif
+
+# if pre-segmentation is not exclusively in the XY plane
+python -m biomedisa.interpolation C:\Users\%USERNAME%\Downloads\tumor.tif C:\Users\%USERNAME%\Downloads\labels.tumor.tif --allaxis
 ```
 
-# Deep Learning
+## Deep Learning
 + [Parameters and Examples](https://github.com/biomedisa/biomedisa/blob/master/README/deep_learning.md)
 
 #### Python example (training)
 ```python
 from biomedisa.features.biomedisa_helper import load_data
 from biomedisa.deeplearning import deep_learning
 
@@ -95,18 +119,18 @@
         val_img_data=val_img_data, val_label_data=val_label_data,
         header=header, extension=ext, path_to_model='honeybees.h5')
 ```
 
 #### Command-line based (training)
 ```
 # start training with a batch size of 12
-python -m biomedisa.deeplearning C:\Users\%USERNAME%\Downloads\training_heart C:\Users\%USERNAME%\Downloads\training_heart_labels -t -bs 12
+python -m biomedisa.deeplearning C:\Users\%USERNAME%\Downloads\training_heart C:\Users\%USERNAME%\Downloads\training_heart_labels -t -bs=12
 
 # validation (optional)
-python -m biomedisa.deeplearning C:\Users\%USERNAME%\Downloads\training_heart C:\Users\%USERNAME%\Downloads\training_heart_labels -t -vi C:\Users\%USERNAME%\Downloads\val_img -vl C:\Users\%USERNAME%\Downloads\val_labels
+python -m biomedisa.deeplearning C:\Users\%USERNAME%\Downloads\training_heart C:\Users\%USERNAME%\Downloads\training_heart_labels -t -vi=C:\Users\%USERNAME%\Downloads\val_img -vl=C:\Users\%USERNAME%\Downloads\val_labels
 ```
 If running into ResourceExhaustedError due to out of memory (OOM), try to use smaller batch size.
 
 #### Python example (prediction)
 ```python
 from biomedisa.features.biomedisa_helper import load_data, save_data
 from biomedisa.deeplearning import deep_learning
@@ -123,15 +147,15 @@
 ```
 
 #### Command-line based (prediction)
 ```
 python -m biomedisa.deeplearning C:\Users\%USERNAME%\Downloads\testing_axial_crop_pat13.nii.gz C:\Users\%USERNAME%\Downloads\heart.h5 -p
 ```
 
-# Biomedisa Features
+## Biomedisa Features
 
 #### Load and save data (such as Amira Mesh, TIFF, NRRD, NIfTI or DICOM)
 ```python
 from biomedisa.features.biomedisa_helper import load_data, save_data
 
 # load data as numpy array
 # for DICOM, PNG files, or similar formats, 'path_to_data' must reference
@@ -202,59 +226,34 @@
 #### Accuracy assessment
 ```python
 from biomedisa.features.biomedisa_helper import Dice_score, ASSD
 dice = Dice_score(ground_truth, result)
 assd = ASSD(ground_truth, result)
 ```
 
-# Update Biomedisa
-If you installed Biomedisa via Pip
-```
-pip install --upgrade biomedisa
-```
-If you used `git clone`, change to the Biomedisa directory and make a pull request
-```
-cd git/biomedisa
-git pull
-```
-
-If you installed the browser based version of Biomedisa (including MySQL database), you also need to update the database
-```
-python manage.py migrate
-```
-
-If you installed an [Apache Server](https://github.com/biomedisa/biomedisa/blob/master/README/APACHE_SERVER.md), you need to restart the server
-```
-sudo service apache2 restart
-```
-
-# Releases
-
-For the versions available, see the [list of releases](https://github.com/biomedisa/biomedisa/releases). 
-
-# Authors
+## Authors
 
 * **Philipp D. Lösel**
 
 See also the list of [contributors](https://github.com/biomedisa/biomedisa/blob/master/credits.md) who participated in this project.
 
-# FAQ
+## FAQ
 Frequently asked questions can be found at: https://biomedisa.info/faq/.
 
-# Citation
+## Citation
 
 If you use Biomedisa or the data, please cite the following paper:
 
 `Lösel, P.D. et al. Introducing Biomedisa as an open-source online platform for biomedical image segmentation. Nat. Commun. 11, 5577 (2020).` https://doi.org/10.1038/s41467-020-19303-w
 
 If you use Biomedisa's Deep Learning, you may also cite:
 
 `Lösel, P.D. et al. Natural variability in bee brain size and symmetry revealed by micro-CT imaging and deep learning. PLoS Comput. Biol. 19, e1011529 (2023).` https://doi.org/10.1371/journal.pcbi.1011529
 
 If you use Biomedisa's Smart Interpolation, you can also cite the initial description of this method:
 
 `Lösel, P. & Heuveline, V. Enhancing a diffusion algorithm for 4D image segmentation using local information. Proc. SPIE 9784, 97842L (2016).` https://doi.org/10.1117/12.2216202
 
-# License
+## License
 
 This project is covered under the **EUROPEAN UNION PUBLIC LICENCE v. 1.2 (EUPL)**.
```

### Comparing `biomedisa-2024.5.20/pyproject.toml` & `biomedisa-2024.5.21/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "biomedisa"
-version = "2024.5.20"
+version = "2024.5.21"
 authors = [
   { name="Philipp Lösel"}, {email="philipp.loesel@anu.edu.au" },
 ]
 description = "Segmentation of 3D volumetric image data"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `biomedisa-2024.5.20/src/biomedisa/__init__.py` & `biomedisa-2024.5.21/src/biomedisa/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os
 import subprocess
 
-# from source base directory
+# base directory
 BASE_DIR = os.path.dirname(os.path.dirname(os.path.abspath(__file__)))
 
 # pip installation
 if not os.path.exists(os.path.join(BASE_DIR,'biomedisa/settings.py')):
 
     # metadata
     import importlib_metadata
```

### Comparing `biomedisa-2024.5.20/src/biomedisa/__main__.py` & `biomedisa-2024.5.21/src/biomedisa/__main__.py`

 * *Files identical despite different names*

### Comparing `biomedisa-2024.5.20/src/biomedisa/deeplearning.py` & `biomedisa-2024.5.21/src/biomedisa/deeplearning.py`

 * *Files identical despite different names*

### Comparing `biomedisa-2024.5.20/src/biomedisa/features/DataGenerator.py` & `biomedisa-2024.5.21/src/biomedisa/features/DataGenerator.py`

 * *Files identical despite different names*

### Comparing `biomedisa-2024.5.20/src/biomedisa/features/DataGeneratorCrop.py` & `biomedisa-2024.5.21/src/biomedisa/features/DataGeneratorCrop.py`

 * *Files identical despite different names*

### Comparing `biomedisa-2024.5.20/src/biomedisa/features/PredictDataGenerator.py` & `biomedisa-2024.5.21/src/biomedisa/features/PredictDataGenerator.py`

 * *Files identical despite different names*

### Comparing `biomedisa-2024.5.20/src/biomedisa/features/PredictDataGeneratorCrop.py` & `biomedisa-2024.5.21/src/biomedisa/features/PredictDataGeneratorCrop.py`

 * *Files identical despite different names*

### Comparing `biomedisa-2024.5.20/src/biomedisa/features/active_contour.py` & `biomedisa-2024.5.21/src/biomedisa/features/active_contour.py`

 * *Files identical despite different names*

### Comparing `biomedisa-2024.5.20/src/biomedisa/features/amira_to_np/amira_data_stream.py` & `biomedisa-2024.5.21/src/biomedisa/features/amira_to_np/amira_data_stream.py`

 * *Files identical despite different names*

### Comparing `biomedisa-2024.5.20/src/biomedisa/features/amira_to_np/amira_grammar.py` & `biomedisa-2024.5.21/src/biomedisa/features/amira_to_np/amira_grammar.py`

 * *Files identical despite different names*

### Comparing `biomedisa-2024.5.20/src/biomedisa/features/amira_to_np/amira_header.py` & `biomedisa-2024.5.21/src/biomedisa/features/amira_to_np/amira_header.py`

 * *Files identical despite different names*

### Comparing `biomedisa-2024.5.20/src/biomedisa/features/amira_to_np/amira_helper.py` & `biomedisa-2024.5.21/src/biomedisa/features/amira_to_np/amira_helper.py`

 * *Files identical despite different names*

### Comparing `biomedisa-2024.5.20/src/biomedisa/features/assd.py` & `biomedisa-2024.5.21/src/biomedisa/features/assd.py`

 * *Files identical despite different names*

### Comparing `biomedisa-2024.5.20/src/biomedisa/features/biomedisa_helper.py` & `biomedisa-2024.5.21/src/biomedisa/features/biomedisa_helper.py`

 * *Files identical despite different names*

### Comparing `biomedisa-2024.5.20/src/biomedisa/features/create_slices.py` & `biomedisa-2024.5.21/src/biomedisa/features/create_slices.py`

 * *Files identical despite different names*

### Comparing `biomedisa-2024.5.20/src/biomedisa/features/crop_helper.py` & `biomedisa-2024.5.21/src/biomedisa/features/crop_helper.py`

 * *Files identical despite different names*

### Comparing `biomedisa-2024.5.20/src/biomedisa/features/curvop_numba.py` & `biomedisa-2024.5.21/src/biomedisa/features/curvop_numba.py`

 * *Files identical despite different names*

### Comparing `biomedisa-2024.5.20/src/biomedisa/features/django_env.py` & `biomedisa-2024.5.21/src/biomedisa/features/django_env.py`

 * *Files identical despite different names*

### Comparing `biomedisa-2024.5.20/src/biomedisa/features/keras_helper.py` & `biomedisa-2024.5.21/src/biomedisa/features/keras_helper.py`

 * *Files identical despite different names*

### Comparing `biomedisa-2024.5.20/src/biomedisa/features/nc_reader.py` & `biomedisa-2024.5.21/src/biomedisa/features/nc_reader.py`

 * *Files identical despite different names*

### Comparing `biomedisa-2024.5.20/src/biomedisa/features/pid.py` & `biomedisa-2024.5.21/src/biomedisa/features/pid.py`

 * *Files identical despite different names*

### Comparing `biomedisa-2024.5.20/src/biomedisa/features/process_image.py` & `biomedisa-2024.5.21/src/biomedisa/features/process_image.py`

 * *Files identical despite different names*

### Comparing `biomedisa-2024.5.20/src/biomedisa/features/pycuda_test.py` & `biomedisa-2024.5.21/src/biomedisa/features/pycuda_test.py`

 * *Files identical despite different names*

### Comparing `biomedisa-2024.5.20/src/biomedisa/features/random_walk/gpu_kernels.py` & `biomedisa-2024.5.21/src/biomedisa/features/random_walk/gpu_kernels.py`

 * *Files identical despite different names*

### Comparing `biomedisa-2024.5.20/src/biomedisa/features/random_walk/pycuda_large.py` & `biomedisa-2024.5.21/src/biomedisa/features/random_walk/pycuda_large.py`

 * *Files identical despite different names*

### Comparing `biomedisa-2024.5.20/src/biomedisa/features/random_walk/pycuda_large_allx.py` & `biomedisa-2024.5.21/src/biomedisa/features/random_walk/pycuda_large_allx.py`

 * *Files identical despite different names*

### Comparing `biomedisa-2024.5.20/src/biomedisa/features/random_walk/pycuda_small.py` & `biomedisa-2024.5.21/src/biomedisa/features/random_walk/pycuda_small.py`

 * *Files identical despite different names*

### Comparing `biomedisa-2024.5.20/src/biomedisa/features/random_walk/pycuda_small_allx.py` & `biomedisa-2024.5.21/src/biomedisa/features/random_walk/pycuda_small_allx.py`

 * *Files identical despite different names*

### Comparing `biomedisa-2024.5.20/src/biomedisa/features/random_walk/pyopencl_large.py` & `biomedisa-2024.5.21/src/biomedisa/features/random_walk/pyopencl_large.py`

 * *Files identical despite different names*

### Comparing `biomedisa-2024.5.20/src/biomedisa/features/random_walk/pyopencl_small.py` & `biomedisa-2024.5.21/src/biomedisa/features/random_walk/pyopencl_small.py`

 * *Files identical despite different names*

### Comparing `biomedisa-2024.5.20/src/biomedisa/features/random_walk/rw_large.py` & `biomedisa-2024.5.21/src/biomedisa/features/random_walk/rw_large.py`

 * *Files identical despite different names*

### Comparing `biomedisa-2024.5.20/src/biomedisa/features/random_walk/rw_small.py` & `biomedisa-2024.5.21/src/biomedisa/features/random_walk/rw_small.py`

 * *Files identical despite different names*

### Comparing `biomedisa-2024.5.20/src/biomedisa/features/remove_outlier.py` & `biomedisa-2024.5.21/src/biomedisa/features/remove_outlier.py`

 * *Files identical despite different names*

### Comparing `biomedisa-2024.5.20/src/biomedisa/features/split_volume.py` & `biomedisa-2024.5.21/src/biomedisa/features/split_volume.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 ##  See the Licence for the specific language governing                 ##
 ##  permissions and limitations under the Licence.                      ##
 ##                                                                      ##
 ##########################################################################
 
 import os
 from biomedisa.features.biomedisa_helper import load_data, save_data
-from biomedisa.features.interpolation import smart_interpolation
+from biomedisa.interpolation import smart_interpolation
 from tifffile import imread, imwrite, TiffFile
 import numpy as np
 import argparse
 
 if __name__ == '__main__':
 
     # initialize arguments
```

### Comparing `biomedisa-2024.5.20/src/biomedisa/interpolation.py` & `biomedisa-2024.5.21/src/biomedisa/interpolation.py`

 * *Files identical despite different names*

### Comparing `biomedisa-2024.5.20/src/biomedisa/mesh.py` & `biomedisa-2024.5.21/src/biomedisa/mesh.py`

 * *Files identical despite different names*

### Comparing `biomedisa-2024.5.20/src/biomedisa.egg-info/PKG-INFO` & `biomedisa-2024.5.21/src/biomedisa.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: biomedisa
-Version: 2024.5.20
+Version: 2024.5.21
 Summary: Segmentation of 3D volumetric image data
 Author: Philipp Lösel
 Author-email: philipp.loesel@anu.edu.au
 Project-URL: Homepage, https://biomedisa.info
 Project-URL: Issues, https://github.com/biomedisa/biomedisa/issues
 Project-URL: GitHub, https://github.com/biomedisa/biomedisa
 Classifier: Programming Language :: Python :: 3
@@ -17,44 +17,49 @@
 [![biomedisa](https://raw.githubusercontent.com/biomedisa/biomedisa/master/biomedisa_app/static/biomedisa_logo.svg)](https://biomedisa.info)
 -----------
 - [Overview](#overview)
 - [Hardware Requirements](#hardware-requirements)
 - [Installation (command-line based)](#installation-command-line-based)
 - [Installation (browser based)](#installation-browser-based)
 - [Download Data](#download-data)
+- [Revisions](#revisions)
 - [Smart Interpolation](#smart-interpolation)
 - [Deep Learning](#deep-learning)
 - [Biomedisa Features](#biomedisa-features)
-- [Update Biomedisa](#update-biomedisa)
-- [Releases](#releases)
 - [Authors](#authors)
 - [FAQ](#faq)
 - [Citation](#citation)
 - [License](#license)
 
-# Overview
+## Overview
 Biomedisa (https://biomedisa.info) is a free and easy-to-use open-source application for segmenting large volumetric images, e.g. CT and MRI scans, developed at [The Australian National University CTLab](https://ctlab.anu.edu.au/). Biomedisa's semi-automated segmentation is based on a smart interpolation of sparsely pre-segmented slices, taking into account the complete underlying image data. In addition, Biomedisa enables deep learning for the fully automated segmentation of series of similar samples. It can be used in combination with segmentation tools such as Amira/Avizo, ImageJ/Fiji and 3D Slicer. If you are using Biomedisa or the data for your research please cite: Lösel, P.D. et al. [Introducing Biomedisa as an open-source online platform for biomedical image segmentation.](https://www.nature.com/articles/s41467-020-19303-w) *Nat. Commun.* **11**, 5577 (2020).
 
-# Hardware Requirements
+## Hardware Requirements
 + One or more NVIDIA GPUs with compute capability 3.0 or higher or an Intel CPU.
 
-# Installation (command-line based)
+## Installation (command-line based)
 + [Ubuntu 22.04 + CUDA + GPU (recommended)](https://github.com/biomedisa/biomedisa/blob/master/README/ubuntu2204_cuda11.8_gpu_cli.md)
 + [Ubuntu 22.04 + OpenCL + CPU (smart interpolation only and very slow)](https://github.com/biomedisa/biomedisa/blob/master/README/ubuntu2204_opencl_cpu_cli.md)
 + [Windows 10 + CUDA + GPU (recommended)](https://github.com/biomedisa/biomedisa/blob/master/README/windows10_cuda_gpu_cli.md)
 + [Windows 10 + OpenCL + GPU (easy to install but lacks features like allaxis, smoothing, uncertainty, optimized GPU memory usage)](https://github.com/biomedisa/biomedisa/blob/master/README/windows10_opencl_gpu_cli.md)
 + [Windows 10 + OpenCL + CPU (very slow)](https://github.com/biomedisa/biomedisa/blob/master/README/windows10_opencl_cpu_cli.md)
 
-# Installation (browser based)
+## Installation (browser based)
 + [Ubuntu 22.04](https://github.com/biomedisa/biomedisa/blob/master/README/ubuntu2204_cuda11.8.md)
 
-# Download Data
+## Download Data
 + Download the data from our [gallery](https://biomedisa.info/gallery/)
 
-# Smart Interpolation
+## Revisions
+2024.05.21
++ Pip is the preferred installation method
++ Commands, module names and imports have been changed to conform to the Pip standard
++ For versions <=2023.09.1 please check [README](https://github.com/biomedisa/biomedisa/blob/master/README/deprecated/README_2023.09.1.md)
+
+## Smart Interpolation
 + [Parameters and Examples](https://github.com/biomedisa/biomedisa/blob/master/README/smart_interpolation.md)
 
 #### Python example
 ```python
 from biomedisa.features.biomedisa_helper import load_data, save_data
 from biomedisa.interpolation import smart_interpolation
 
@@ -73,17 +78,20 @@
 save_data('Downloads/final.trigonopterus.am', regular_result, header=header)
 save_data('Downloads/final.trigonopterus.smooth.am', smooth_result, header=header)
 ```
 
 #### Command-line based
 ```
 python -m biomedisa.interpolation C:\Users\%USERNAME%\Downloads\tumor.tif C:\Users\%USERNAME%\Downloads\labels.tumor.tif
+
+# if pre-segmentation is not exclusively in the XY plane
+python -m biomedisa.interpolation C:\Users\%USERNAME%\Downloads\tumor.tif C:\Users\%USERNAME%\Downloads\labels.tumor.tif --allaxis
 ```
 
-# Deep Learning
+## Deep Learning
 + [Parameters and Examples](https://github.com/biomedisa/biomedisa/blob/master/README/deep_learning.md)
 
 #### Python example (training)
 ```python
 from biomedisa.features.biomedisa_helper import load_data
 from biomedisa.deeplearning import deep_learning
 
@@ -111,18 +119,18 @@
         val_img_data=val_img_data, val_label_data=val_label_data,
         header=header, extension=ext, path_to_model='honeybees.h5')
 ```
 
 #### Command-line based (training)
 ```
 # start training with a batch size of 12
-python -m biomedisa.deeplearning C:\Users\%USERNAME%\Downloads\training_heart C:\Users\%USERNAME%\Downloads\training_heart_labels -t -bs 12
+python -m biomedisa.deeplearning C:\Users\%USERNAME%\Downloads\training_heart C:\Users\%USERNAME%\Downloads\training_heart_labels -t -bs=12
 
 # validation (optional)
-python -m biomedisa.deeplearning C:\Users\%USERNAME%\Downloads\training_heart C:\Users\%USERNAME%\Downloads\training_heart_labels -t -vi C:\Users\%USERNAME%\Downloads\val_img -vl C:\Users\%USERNAME%\Downloads\val_labels
+python -m biomedisa.deeplearning C:\Users\%USERNAME%\Downloads\training_heart C:\Users\%USERNAME%\Downloads\training_heart_labels -t -vi=C:\Users\%USERNAME%\Downloads\val_img -vl=C:\Users\%USERNAME%\Downloads\val_labels
 ```
 If running into ResourceExhaustedError due to out of memory (OOM), try to use smaller batch size.
 
 #### Python example (prediction)
 ```python
 from biomedisa.features.biomedisa_helper import load_data, save_data
 from biomedisa.deeplearning import deep_learning
@@ -139,15 +147,15 @@
 ```
 
 #### Command-line based (prediction)
 ```
 python -m biomedisa.deeplearning C:\Users\%USERNAME%\Downloads\testing_axial_crop_pat13.nii.gz C:\Users\%USERNAME%\Downloads\heart.h5 -p
 ```
 
-# Biomedisa Features
+## Biomedisa Features
 
 #### Load and save data (such as Amira Mesh, TIFF, NRRD, NIfTI or DICOM)
 ```python
 from biomedisa.features.biomedisa_helper import load_data, save_data
 
 # load data as numpy array
 # for DICOM, PNG files, or similar formats, 'path_to_data' must reference
@@ -218,59 +226,34 @@
 #### Accuracy assessment
 ```python
 from biomedisa.features.biomedisa_helper import Dice_score, ASSD
 dice = Dice_score(ground_truth, result)
 assd = ASSD(ground_truth, result)
 ```
 
-# Update Biomedisa
-If you installed Biomedisa via Pip
-```
-pip install --upgrade biomedisa
-```
-If you used `git clone`, change to the Biomedisa directory and make a pull request
-```
-cd git/biomedisa
-git pull
-```
-
-If you installed the browser based version of Biomedisa (including MySQL database), you also need to update the database
-```
-python manage.py migrate
-```
-
-If you installed an [Apache Server](https://github.com/biomedisa/biomedisa/blob/master/README/APACHE_SERVER.md), you need to restart the server
-```
-sudo service apache2 restart
-```
-
-# Releases
-
-For the versions available, see the [list of releases](https://github.com/biomedisa/biomedisa/releases). 
-
-# Authors
+## Authors
 
 * **Philipp D. Lösel**
 
 See also the list of [contributors](https://github.com/biomedisa/biomedisa/blob/master/credits.md) who participated in this project.
 
-# FAQ
+## FAQ
 Frequently asked questions can be found at: https://biomedisa.info/faq/.
 
-# Citation
+## Citation
 
 If you use Biomedisa or the data, please cite the following paper:
 
 `Lösel, P.D. et al. Introducing Biomedisa as an open-source online platform for biomedical image segmentation. Nat. Commun. 11, 5577 (2020).` https://doi.org/10.1038/s41467-020-19303-w
 
 If you use Biomedisa's Deep Learning, you may also cite:
 
 `Lösel, P.D. et al. Natural variability in bee brain size and symmetry revealed by micro-CT imaging and deep learning. PLoS Comput. Biol. 19, e1011529 (2023).` https://doi.org/10.1371/journal.pcbi.1011529
 
 If you use Biomedisa's Smart Interpolation, you can also cite the initial description of this method:
 
 `Lösel, P. & Heuveline, V. Enhancing a diffusion algorithm for 4D image segmentation using local information. Proc. SPIE 9784, 97842L (2016).` https://doi.org/10.1117/12.2216202
 
-# License
+## License
 
 This project is covered under the **EUROPEAN UNION PUBLIC LICENCE v. 1.2 (EUPL)**.
```

### Comparing `biomedisa-2024.5.20/src/biomedisa.egg-info/SOURCES.txt` & `biomedisa-2024.5.21/src/biomedisa.egg-info/SOURCES.txt`

 * *Files identical despite different names*

