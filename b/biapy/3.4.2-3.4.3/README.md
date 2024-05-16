# Comparing `tmp/biapy-3.4.2.tar.gz` & `tmp/biapy-3.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "biapy-3.4.2.tar", last modified: Mon Apr 29 14:44:07 2024, max compression
+gzip compressed data, was "biapy-3.4.3.tar", last modified: Thu May 16 10:34:24 2024, max compression
```

## Comparing `biapy-3.4.2.tar` & `biapy-3.4.3.tar`

### file list

```diff
@@ -1,97 +1,98 @@
-drwxrwxr-x   0 dfranco   (1001) dfranco   (1001)        0 2024-04-29 14:44:07.171722 biapy-3.4.2/
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)     1079 2023-10-17 15:21:29.000000 biapy-3.4.2/LICENSE.md
--rw-r--r--   0 dfranco   (1001) dfranco   (1001)    23500 2024-04-29 14:44:07.171722 biapy-3.4.2/PKG-INFO
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)    20933 2024-02-13 08:45:05.000000 biapy-3.4.2/README.md
-drwxrwxr-x   0 dfranco   (1001) dfranco   (1001)        0 2024-04-29 14:44:07.163721 biapy-3.4.2/biapy/
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)     2097 2024-04-28 17:54:13.000000 biapy-3.4.2/biapy/__init__.py
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)    19820 2024-04-10 10:46:29.000000 biapy-3.4.2/biapy/_biapy.py
-drwxrwxr-x   0 dfranco   (1001) dfranco   (1001)        0 2024-04-29 14:44:07.163721 biapy-3.4.2/biapy/config/
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)       22 2024-01-08 16:04:47.000000 biapy-3.4.2/biapy/config/__init__.py
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)    75069 2024-04-17 17:01:31.000000 biapy-3.4.2/biapy/config/config.py
-drwxrwxr-x   0 dfranco   (1001) dfranco   (1001)        0 2024-04-29 14:44:07.163721 biapy-3.4.2/biapy/data/
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)        0 2024-01-08 16:04:47.000000 biapy-3.4.2/biapy/data/__init__.py
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)    41275 2024-04-17 17:47:14.000000 biapy-3.4.2/biapy/data/data_2D_manipulation.py
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)    62136 2024-04-10 10:46:29.000000 biapy-3.4.2/biapy/data/data_3D_manipulation.py
-drwxrwxr-x   0 dfranco   (1001) dfranco   (1001)        0 2024-04-29 14:44:07.167721 biapy-3.4.2/biapy/data/generators/
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)    27729 2024-04-17 17:30:50.000000 biapy-3.4.2/biapy/data/generators/__init__.py
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)    66739 2024-04-14 17:29:53.000000 biapy-3.4.2/biapy/data/generators/augmentors.py
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)    69342 2024-04-29 13:24:42.000000 biapy-3.4.2/biapy/data/generators/pair_base_data_generator.py
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)     5531 2024-04-10 07:02:56.000000 biapy-3.4.2/biapy/data/generators/pair_data_2D_generator.py
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)     7767 2024-04-11 11:49:07.000000 biapy-3.4.2/biapy/data/generators/pair_data_3D_generator.py
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)    21839 2024-04-17 17:50:54.000000 biapy-3.4.2/biapy/data/generators/single_base_data_generator.py
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)     1612 2024-01-10 14:40:34.000000 biapy-3.4.2/biapy/data/generators/single_data_2D_generator.py
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)     2864 2024-04-10 07:26:02.000000 biapy-3.4.2/biapy/data/generators/single_data_3D_generator.py
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)    18755 2024-04-29 14:34:06.000000 biapy-3.4.2/biapy/data/generators/test_pair_data_generators.py
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)    10205 2024-04-29 14:33:55.000000 biapy-3.4.2/biapy/data/generators/test_single_data_generator.py
-drwxrwxr-x   0 dfranco   (1001) dfranco   (1001)        0 2024-04-29 14:44:07.167721 biapy-3.4.2/biapy/data/post_processing/
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)     3028 2024-01-08 16:04:47.000000 biapy-3.4.2/biapy/data/post_processing/__init__.py
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)    76121 2024-02-25 18:30:55.000000 biapy-3.4.2/biapy/data/post_processing/post_processing.py
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)    10434 2024-01-08 16:04:47.000000 biapy-3.4.2/biapy/data/post_processing/smooth_tiled_predictions.py
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)    59239 2024-04-17 17:29:25.000000 biapy-3.4.2/biapy/data/pre_processing.py
-drwxrwxr-x   0 dfranco   (1001) dfranco   (1001)        0 2024-04-29 14:44:07.167721 biapy-3.4.2/biapy/engine/
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)     2606 2024-02-23 08:04:46.000000 biapy-3.4.2/biapy/engine/__init__.py
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)    92000 2024-04-29 14:24:57.000000 biapy-3.4.2/biapy/engine/base_workflow.py
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)    60824 2024-04-16 06:30:21.000000 biapy-3.4.2/biapy/engine/check_configuration.py
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)    15050 2024-04-10 10:46:29.000000 biapy-3.4.2/biapy/engine/classification.py
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)    22609 2024-04-10 11:22:44.000000 biapy-3.4.2/biapy/engine/denoising.py
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)    53161 2024-04-10 11:27:47.000000 biapy-3.4.2/biapy/engine/detection.py
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)    13410 2024-04-14 15:24:09.000000 biapy-3.4.2/biapy/engine/image_to_image.py
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)    48257 2024-04-10 10:46:29.000000 biapy-3.4.2/biapy/engine/instance_seg.py
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)    25026 2024-04-14 10:22:07.000000 biapy-3.4.2/biapy/engine/metrics.py
-drwxrwxr-x   0 dfranco   (1001) dfranco   (1001)        0 2024-04-29 14:44:07.167721 biapy-3.4.2/biapy/engine/schedulers/
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)      956 2024-01-08 16:04:47.000000 biapy-3.4.2/biapy/engine/schedulers/warmup_cosine_decay.py
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)    21105 2024-04-10 11:29:23.000000 biapy-3.4.2/biapy/engine/self_supervised.py
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)    11246 2024-04-14 15:53:50.000000 biapy-3.4.2/biapy/engine/semantic_seg.py
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)    13055 2024-04-10 10:46:29.000000 biapy-3.4.2/biapy/engine/super_resolution.py
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)     4664 2024-04-10 06:46:00.000000 biapy-3.4.2/biapy/engine/train_engine.py
-drwxrwxr-x   0 dfranco   (1001) dfranco   (1001)        0 2024-04-29 14:44:07.171722 biapy-3.4.2/biapy/models/
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)    11931 2024-04-10 06:46:00.000000 biapy-3.4.2/biapy/models/__init__.py
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)     7576 2024-02-25 11:08:42.000000 biapy-3.4.2/biapy/models/attention_unet.py
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)    17636 2024-01-08 16:04:47.000000 biapy-3.4.2/biapy/models/blocks.py
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)     3637 2024-02-25 11:08:42.000000 biapy-3.4.2/biapy/models/dfcan.py
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)     3305 2024-02-25 11:08:42.000000 biapy-3.4.2/biapy/models/edsr.py
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)     1221 2024-02-05 08:46:05.000000 biapy-3.4.2/biapy/models/efficientnet.py
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)    18737 2024-04-10 06:46:00.000000 biapy-3.4.2/biapy/models/mae.py
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)    13552 2024-02-25 11:08:42.000000 biapy-3.4.2/biapy/models/multiresunet.py
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)     2732 2024-02-25 11:08:42.000000 biapy-3.4.2/biapy/models/rcan.py
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)     9139 2024-02-25 11:08:42.000000 biapy-3.4.2/biapy/models/resunet++.py
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)     7451 2024-03-06 11:13:09.000000 biapy-3.4.2/biapy/models/resunet.py
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)     7231 2024-02-25 11:08:42.000000 biapy-3.4.2/biapy/models/seunet.py
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)     2998 2024-01-08 16:04:47.000000 biapy-3.4.2/biapy/models/simple_cnn.py
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)     1734 2024-02-26 12:21:55.000000 biapy-3.4.2/biapy/models/tr_layers.py
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)     7186 2024-02-25 11:08:42.000000 biapy-3.4.2/biapy/models/unet.py
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)    10300 2024-04-10 06:46:00.000000 biapy-3.4.2/biapy/models/unetr.py
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)     3592 2024-01-08 16:04:47.000000 biapy-3.4.2/biapy/models/vit.py
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)     2982 2024-02-25 11:08:42.000000 biapy-3.4.2/biapy/models/wdsr.py
-drwxrwxr-x   0 dfranco   (1001) dfranco   (1001)        0 2024-04-29 14:44:07.171722 biapy-3.4.2/biapy/utils/
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)     4243 2024-01-08 16:04:47.000000 biapy-3.4.2/biapy/utils/callbacks.py
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)    12958 2024-04-14 08:44:02.000000 biapy-3.4.2/biapy/utils/matching.py
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)    14861 2024-03-01 08:53:49.000000 biapy-3.4.2/biapy/utils/misc.py
-drwxrwxr-x   0 dfranco   (1001) dfranco   (1001)        0 2024-04-29 14:44:07.171722 biapy-3.4.2/biapy/utils/scripts/
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)     3617 2024-01-08 16:04:47.000000 biapy-3.4.2/biapy/utils/scripts/calculate_detection_metrics.py
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)     5803 2024-01-08 16:04:47.000000 biapy-3.4.2/biapy/utils/scripts/calculate_metrics_3D.py
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)     5021 2024-01-08 16:04:47.000000 biapy-3.4.2/biapy/utils/scripts/create_probability_csv.py
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)     1808 2024-01-08 16:04:47.000000 biapy-3.4.2/biapy/utils/scripts/crop_2D_dataset.py
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)     1171 2024-01-08 16:04:47.000000 biapy-3.4.2/biapy/utils/scripts/crop_3D_dataset.py
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)     1828 2024-01-08 16:04:47.000000 biapy-3.4.2/biapy/utils/scripts/crop_and_discard_3D_dataset.py
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)     1726 2024-01-08 16:04:47.000000 biapy-3.4.2/biapy/utils/scripts/detection_plots.py
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)     4873 2024-01-08 16:04:47.000000 biapy-3.4.2/biapy/utils/scripts/detection_probs_to_points.py
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)     2374 2024-01-08 16:04:47.000000 biapy-3.4.2/biapy/utils/scripts/fill_holes_in_seg_masks.py
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)     3864 2024-01-08 16:04:47.000000 biapy-3.4.2/biapy/utils/scripts/filter_close_points.py
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)     1895 2024-01-08 16:04:47.000000 biapy-3.4.2/biapy/utils/scripts/from_class_csv_to_folders.py
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)      674 2024-01-08 16:04:47.000000 biapy-3.4.2/biapy/utils/scripts/h5_to_tif.py
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)     1212 2024-01-08 16:04:47.000000 biapy-3.4.2/biapy/utils/scripts/h5_to_zarr.py
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)     2328 2024-04-22 08:23:08.000000 biapy-3.4.2/biapy/utils/scripts/lightmycell_data_preparation.py
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)      920 2024-01-08 16:04:47.000000 biapy-3.4.2/biapy/utils/scripts/merge_dataset_channels.py
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)     2538 2024-01-08 16:04:47.000000 biapy-3.4.2/biapy/utils/scripts/order_axes.py
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)      966 2024-01-08 16:04:47.000000 biapy-3.4.2/biapy/utils/scripts/tif_to_h5.py
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)    57739 2024-04-14 16:12:07.000000 biapy-3.4.2/biapy/utils/util.py
-drwxrwxr-x   0 dfranco   (1001) dfranco   (1001)        0 2024-04-29 14:44:07.171722 biapy-3.4.2/biapy.egg-info/
--rw-r--r--   0 dfranco   (1001) dfranco   (1001)    23500 2024-04-29 14:44:07.000000 biapy-3.4.2/biapy.egg-info/PKG-INFO
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)     2703 2024-04-29 14:44:07.000000 biapy-3.4.2/biapy.egg-info/SOURCES.txt
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)        1 2024-04-29 14:44:07.000000 biapy-3.4.2/biapy.egg-info/dependency_links.txt
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)       37 2024-04-29 14:44:07.000000 biapy-3.4.2/biapy.egg-info/entry_points.txt
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)      348 2024-04-29 14:44:07.000000 biapy-3.4.2/biapy.egg-info/requires.txt
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)        6 2024-04-29 14:44:07.000000 biapy-3.4.2/biapy.egg-info/top_level.txt
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)     1718 2024-04-29 09:21:38.000000 biapy-3.4.2/pyproject.toml
--rw-rw-r--   0 dfranco   (1001) dfranco   (1001)       38 2024-04-29 14:44:07.171722 biapy-3.4.2/setup.cfg
+drwxrwxr-x   0 dfranco   (1001) dfranco   (1001)        0 2024-05-16 10:34:24.306904 biapy-3.4.3/
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)     1079 2023-03-09 07:44:00.000000 biapy-3.4.3/LICENSE.md
+-rw-r--r--   0 dfranco   (1001) dfranco   (1001)    23500 2024-05-16 10:34:24.306904 biapy-3.4.3/PKG-INFO
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)    20933 2024-02-13 08:39:35.000000 biapy-3.4.3/README.md
+drwxrwxr-x   0 dfranco   (1001) dfranco   (1001)        0 2024-05-16 10:34:24.294904 biapy-3.4.3/biapy/
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)     2097 2024-05-16 10:33:18.000000 biapy-3.4.3/biapy/__init__.py
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)    19898 2024-05-16 10:33:18.000000 biapy-3.4.3/biapy/_biapy.py
+drwxrwxr-x   0 dfranco   (1001) dfranco   (1001)        0 2024-05-16 10:34:24.294904 biapy-3.4.3/biapy/config/
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)       22 2024-01-04 12:54:41.000000 biapy-3.4.3/biapy/config/__init__.py
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)    75082 2024-05-16 10:33:18.000000 biapy-3.4.3/biapy/config/config.py
+drwxrwxr-x   0 dfranco   (1001) dfranco   (1001)        0 2024-05-16 10:34:24.298904 biapy-3.4.3/biapy/data/
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)        0 2024-01-04 12:54:41.000000 biapy-3.4.3/biapy/data/__init__.py
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)    45284 2024-05-16 10:33:18.000000 biapy-3.4.3/biapy/data/data_2D_manipulation.py
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)    66558 2024-05-16 10:33:18.000000 biapy-3.4.3/biapy/data/data_3D_manipulation.py
+drwxrwxr-x   0 dfranco   (1001) dfranco   (1001)        0 2024-05-16 10:34:24.298904 biapy-3.4.3/biapy/data/generators/
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)    27960 2024-05-16 10:33:18.000000 biapy-3.4.3/biapy/data/generators/__init__.py
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)    66734 2024-05-16 10:33:18.000000 biapy-3.4.3/biapy/data/generators/augmentors.py
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)    69136 2024-05-16 10:33:18.000000 biapy-3.4.3/biapy/data/generators/pair_base_data_generator.py
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)     5616 2024-05-16 10:33:18.000000 biapy-3.4.3/biapy/data/generators/pair_data_2D_generator.py
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)     7835 2024-05-16 10:33:18.000000 biapy-3.4.3/biapy/data/generators/pair_data_3D_generator.py
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)    22270 2024-05-16 10:33:18.000000 biapy-3.4.3/biapy/data/generators/single_base_data_generator.py
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)     1612 2024-01-10 14:29:17.000000 biapy-3.4.3/biapy/data/generators/single_data_2D_generator.py
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)     2864 2024-04-12 16:11:48.000000 biapy-3.4.3/biapy/data/generators/single_data_3D_generator.py
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)    19467 2024-05-16 10:33:18.000000 biapy-3.4.3/biapy/data/generators/test_pair_data_generators.py
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)    10987 2024-05-16 10:33:18.000000 biapy-3.4.3/biapy/data/generators/test_single_data_generator.py
+drwxrwxr-x   0 dfranco   (1001) dfranco   (1001)        0 2024-05-16 10:34:24.298904 biapy-3.4.3/biapy/data/post_processing/
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)     3028 2024-01-04 12:54:41.000000 biapy-3.4.3/biapy/data/post_processing/__init__.py
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)    76226 2024-05-16 10:33:18.000000 biapy-3.4.3/biapy/data/post_processing/post_processing.py
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)    10434 2024-01-04 12:54:41.000000 biapy-3.4.3/biapy/data/post_processing/smooth_tiled_predictions.py
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)    59305 2024-05-16 10:33:18.000000 biapy-3.4.3/biapy/data/pre_processing.py
+drwxrwxr-x   0 dfranco   (1001) dfranco   (1001)        0 2024-05-16 10:34:24.298904 biapy-3.4.3/biapy/engine/
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)     2606 2024-02-25 18:32:47.000000 biapy-3.4.3/biapy/engine/__init__.py
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)    91979 2024-05-16 10:33:18.000000 biapy-3.4.3/biapy/engine/base_workflow.py
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)    60972 2024-05-16 10:33:18.000000 biapy-3.4.3/biapy/engine/check_configuration.py
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)    16287 2024-05-16 10:33:18.000000 biapy-3.4.3/biapy/engine/classification.py
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)    22609 2024-04-12 16:11:48.000000 biapy-3.4.3/biapy/engine/denoising.py
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)    53230 2024-05-16 10:33:18.000000 biapy-3.4.3/biapy/engine/detection.py
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)    13410 2024-04-14 17:17:46.000000 biapy-3.4.3/biapy/engine/image_to_image.py
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)    48723 2024-05-16 10:33:18.000000 biapy-3.4.3/biapy/engine/instance_seg.py
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)    25026 2024-04-14 17:17:46.000000 biapy-3.4.3/biapy/engine/metrics.py
+drwxrwxr-x   0 dfranco   (1001) dfranco   (1001)        0 2024-05-16 10:34:24.298904 biapy-3.4.3/biapy/engine/schedulers/
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)      956 2024-01-04 12:54:41.000000 biapy-3.4.3/biapy/engine/schedulers/warmup_cosine_decay.py
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)    21105 2024-04-12 16:11:48.000000 biapy-3.4.3/biapy/engine/self_supervised.py
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)    11246 2024-04-14 17:17:46.000000 biapy-3.4.3/biapy/engine/semantic_seg.py
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)    13055 2024-04-12 16:11:48.000000 biapy-3.4.3/biapy/engine/super_resolution.py
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)     4952 2024-05-16 10:33:18.000000 biapy-3.4.3/biapy/engine/train_engine.py
+drwxrwxr-x   0 dfranco   (1001) dfranco   (1001)        0 2024-05-16 10:34:24.302904 biapy-3.4.3/biapy/models/
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)    11931 2024-04-12 16:11:48.000000 biapy-3.4.3/biapy/models/__init__.py
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)     7576 2024-02-25 18:32:47.000000 biapy-3.4.3/biapy/models/attention_unet.py
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)    17636 2024-01-04 12:54:41.000000 biapy-3.4.3/biapy/models/blocks.py
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)     3637 2024-02-25 18:32:47.000000 biapy-3.4.3/biapy/models/dfcan.py
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)     3305 2024-02-25 18:32:47.000000 biapy-3.4.3/biapy/models/edsr.py
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)     1221 2024-02-08 07:25:10.000000 biapy-3.4.3/biapy/models/efficientnet.py
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)    18966 2024-05-16 10:33:18.000000 biapy-3.4.3/biapy/models/mae.py
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)    13552 2024-02-25 18:32:47.000000 biapy-3.4.3/biapy/models/multiresunet.py
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)     2732 2024-02-25 18:32:47.000000 biapy-3.4.3/biapy/models/rcan.py
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)     9139 2024-02-25 18:32:47.000000 biapy-3.4.3/biapy/models/resunet++.py
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)     7451 2024-02-26 08:40:58.000000 biapy-3.4.3/biapy/models/resunet.py
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)     7231 2024-02-25 18:32:47.000000 biapy-3.4.3/biapy/models/seunet.py
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)     2998 2024-01-04 12:54:41.000000 biapy-3.4.3/biapy/models/simple_cnn.py
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)     1734 2024-02-15 12:34:02.000000 biapy-3.4.3/biapy/models/tr_layers.py
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)     7186 2024-02-25 18:32:47.000000 biapy-3.4.3/biapy/models/unet.py
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)    10300 2024-04-12 16:11:48.000000 biapy-3.4.3/biapy/models/unetr.py
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)     3592 2024-01-04 12:54:41.000000 biapy-3.4.3/biapy/models/vit.py
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)     2982 2024-02-25 18:32:47.000000 biapy-3.4.3/biapy/models/wdsr.py
+drwxrwxr-x   0 dfranco   (1001) dfranco   (1001)        0 2024-05-16 10:34:24.302904 biapy-3.4.3/biapy/utils/
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)     4243 2024-01-04 12:54:41.000000 biapy-3.4.3/biapy/utils/callbacks.py
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)    12958 2024-04-13 10:16:32.000000 biapy-3.4.3/biapy/utils/matching.py
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)    14861 2024-02-15 12:34:02.000000 biapy-3.4.3/biapy/utils/misc.py
+drwxrwxr-x   0 dfranco   (1001) dfranco   (1001)        0 2024-05-16 10:34:24.302904 biapy-3.4.3/biapy/utils/scripts/
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)     3617 2024-01-04 12:54:41.000000 biapy-3.4.3/biapy/utils/scripts/calculate_detection_metrics.py
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)     5803 2024-01-04 12:54:41.000000 biapy-3.4.3/biapy/utils/scripts/calculate_metrics_3D.py
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)     5021 2024-01-04 12:54:41.000000 biapy-3.4.3/biapy/utils/scripts/create_probability_csv.py
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)     1808 2024-01-04 12:54:41.000000 biapy-3.4.3/biapy/utils/scripts/crop_2D_dataset.py
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)     1171 2024-01-04 12:54:41.000000 biapy-3.4.3/biapy/utils/scripts/crop_3D_dataset.py
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)     1828 2024-01-04 12:54:41.000000 biapy-3.4.3/biapy/utils/scripts/crop_and_discard_3D_dataset.py
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)     1726 2024-01-04 12:54:41.000000 biapy-3.4.3/biapy/utils/scripts/detection_plots.py
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)     4873 2024-01-04 12:54:41.000000 biapy-3.4.3/biapy/utils/scripts/detection_probs_to_points.py
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)     2374 2024-01-04 12:54:41.000000 biapy-3.4.3/biapy/utils/scripts/fill_holes_in_seg_masks.py
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)     3864 2024-01-04 12:54:41.000000 biapy-3.4.3/biapy/utils/scripts/filter_close_points.py
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)     1895 2024-01-04 12:54:41.000000 biapy-3.4.3/biapy/utils/scripts/from_class_csv_to_folders.py
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)      674 2024-01-04 12:54:41.000000 biapy-3.4.3/biapy/utils/scripts/h5_to_tif.py
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)     1212 2024-01-04 12:54:41.000000 biapy-3.4.3/biapy/utils/scripts/h5_to_zarr.py
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)     2328 2024-04-27 18:57:13.000000 biapy-3.4.3/biapy/utils/scripts/lightmycell_data_preparation.py
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)      920 2024-01-04 12:54:41.000000 biapy-3.4.3/biapy/utils/scripts/merge_dataset_channels.py
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)     2538 2024-01-04 12:54:41.000000 biapy-3.4.3/biapy/utils/scripts/order_axes.py
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)   118081 2024-05-16 10:33:18.000000 biapy-3.4.3/biapy/utils/scripts/run_checks.py
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)      966 2024-01-04 12:54:41.000000 biapy-3.4.3/biapy/utils/scripts/tif_to_h5.py
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)    57739 2024-04-12 16:11:48.000000 biapy-3.4.3/biapy/utils/util.py
+drwxrwxr-x   0 dfranco   (1001) dfranco   (1001)        0 2024-05-16 10:34:24.302904 biapy-3.4.3/biapy.egg-info/
+-rw-r--r--   0 dfranco   (1001) dfranco   (1001)    23500 2024-05-16 10:34:24.000000 biapy-3.4.3/biapy.egg-info/PKG-INFO
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)     2737 2024-05-16 10:34:24.000000 biapy-3.4.3/biapy.egg-info/SOURCES.txt
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)        1 2024-05-16 10:34:24.000000 biapy-3.4.3/biapy.egg-info/dependency_links.txt
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)       37 2024-05-16 10:34:24.000000 biapy-3.4.3/biapy.egg-info/entry_points.txt
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)      348 2024-05-16 10:34:24.000000 biapy-3.4.3/biapy.egg-info/requires.txt
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)        6 2024-05-16 10:34:24.000000 biapy-3.4.3/biapy.egg-info/top_level.txt
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)     1718 2024-05-16 10:34:12.000000 biapy-3.4.3/pyproject.toml
+-rw-rw-r--   0 dfranco   (1001) dfranco   (1001)       38 2024-05-16 10:34:24.306904 biapy-3.4.3/setup.cfg
```

### Comparing `biapy-3.4.2/LICENSE.md` & `biapy-3.4.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `biapy-3.4.2/PKG-INFO` & `biapy-3.4.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: biapy
-Version: 3.4.2
+Version: 3.4.3
 Summary: BiaPy: Bioimage analysis pipelines in Python
 Author-email: Daniel Franco-Barranco <daniel.franco@dipc.org>
 Maintainer-email: Daniel Franco-Barranco <daniel.franco@dipc.org>
 License: MIT License
         
         Copyright (c) 2022 Daniel Franco-Barranco
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: biapy Version: 3.4.2 Summary: BiaPy: Bioimage
+Metadata-Version: 2.1 Name: biapy Version: 3.4.3 Summary: BiaPy: Bioimage
 analysis pipelines in Python Author-email: Daniel Franco-Barranco
 dipc.org> Maintainer-email: Daniel Franco-Barranco
 dipc.org> License: MIT License Copyright (c) 2022 Daniel Franco-Barranco
 Permission is hereby granted, free of charge, to any person obtaining a copy of
 this software and associated documentation files (the "Software"), to deal in
 the Software without restriction, including without limitation the rights to
 use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies
```

### Comparing `biapy-3.4.2/README.md` & `biapy-3.4.3/README.md`

 * *Files identical despite different names*

### Comparing `biapy-3.4.2/biapy/__init__.py` & `biapy-3.4.3/biapy/__init__.py`

 * *Files identical despite different names*

### Comparing `biapy-3.4.2/biapy/_biapy.py` & `biapy-3.4.3/biapy/_biapy.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import torch.backends.cudnn as cudnn
 import torch.distributed as dist
 from shutil import copyfile
 import numpy as np
 import importlib
 import multiprocessing
 
-from biapy.utils.misc import init_devices, is_dist_avail_and_initialized, set_seed, get_rank
+from biapy.utils.misc import init_devices, is_dist_avail_and_initialized, set_seed, get_rank, setup_for_distributed
 from biapy.config.config import Config
 from biapy.engine.check_configuration import check_configuration
 
 class BiaPy():
     def __init__(self, config, result_dir=os.getenv('HOME'), name="unknown_job", run_id=1, gpu=None, world_size=1, 
         local_rank=-1, dist_on_itp=False, dist_url='env://', dist_backend='nccl'):
         """
@@ -416,11 +416,12 @@
             dist.barrier()
 
         if self.cfg.TEST.ENABLE:
             self.test()
 
         if is_dist_avail_and_initialized():
             print(f"[Rank {get_rank()} ({os.getpid()})] Process waiting (test finished) . . . ")
+            setup_for_distributed(self.args.rank == 0)
             dist.barrier()
             dist.destroy_process_group()
 
         print("FINISHED JOB {} !!".format(self.job_identifier))
```

### Comparing `biapy-3.4.2/biapy/config/config.py` & `biapy-3.4.3/biapy/config/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -180,32 +180,34 @@
         # of it. Useful to avoid extracting patches which no foreground class information. Use it only when
         # 'PROBLEM.TYPE' is 'SEMANTIC_SEG' 
         _C.DATA.PROBABILITY_MAP = False # Used when _C.DATA.EXTRACT_RANDOM_PATCH=True
         _C.DATA.W_FOREGROUND = 0.94 # Used when _C.DATA.PROBABILITY_MAP=True
         _C.DATA.W_BACKGROUND = 0.06 # Used when _C.DATA.PROBABILITY_MAP=True
 
         # Whether to reshape the dimensions that does not satisfy the patch shape selected by padding it with reflect. It's not
-        # implemented in super-resolution workflow.
+        # implemented in super-resolution inference phase workflow (as usually the patch size is small).
         _C.DATA.REFLECT_TO_COMPLETE_SHAPE = False
 
         _C.DATA.NORMALIZATION = CN()
+        # Whether to apply or not a percentile clipping before normalizing the data
+        _C.DATA.NORMALIZATION.PERC_CLIP = False
+        # Lower and upper bound for percentile clip. Must be set when DATA.NORMALIZATION.PERC_CLIP = 'True'
+        _C.DATA.NORMALIZATION.PERC_LOWER = -1.0
+        _C.DATA.NORMALIZATION.PERC_UPPER = -1.0
         # Normalization type to use. Possible options:
         #   'div' to divide values from 0/255 (or 0/65535 if uint16) in [0,1] range
         #   'custom' to use DATA.NORMALIZATION.CUSTOM_MEAN and DATA.NORMALIZATION.CUSTOM_STD to normalize
         _C.DATA.NORMALIZATION.TYPE = 'div'
-        # Whether to apply the normalization by sample ("image") or by all dataset statistics ("dataset"). Options: ["image", "dataset"]  
+        # Whether to apply the normalization by sample ("image") or by all dataset statistics ("dataset"). 
+        # Used with 'DATA.NORMALIZATION.PERC_CLIP' == 'True' and/or when 'DATA.NORMALIZATION.TYPE' == 'custom'. 
+        # Options: ["image", "dataset"]  
         _C.DATA.NORMALIZATION.APPLICATION_MODE = "image"
         # Custom normalization variables: mean and std (they are calculated if not provided)
         _C.DATA.NORMALIZATION.CUSTOM_MEAN = -1.0
         _C.DATA.NORMALIZATION.CUSTOM_STD = -1.0
-        # Whether to apply or not a percentile clipping before normalizing the data
-        _C.DATA.NORMALIZATION.PERC_CLIP = False
-        # Lower and upper bound for percentile clip. Must be set when DATA.NORMALIZATION.PERC_CLIP = 'True'
-        _C.DATA.NORMALIZATION.PERC_LOWER = -1.0
-        _C.DATA.NORMALIZATION.PERC_UPPER = -1.0
 
         # If 'DATA.PATCH_SIZE' selected has 3 channels, e.g. RGB images are expected, so will force grayscale images to be
         # converted into RGB (e.g. in ImageNet some of the images are grayscale)
         _C.DATA.FORCE_RGB = False
 
         # Train
         _C.DATA.TRAIN = CN()
@@ -380,17 +382,14 @@
         # The values must be floats between range [0, 1). It needs to be a 2D tuple when using _C.PROBLEM.NDIM='2D' and
         # 3D tuple when using _C.PROBLEM.NDIM='3D'. This is only used when the validation is loaded from disk, and thus, 
         # not extracted from training. 
         _C.DATA.VAL.OVERLAP = (0,0)
         # Padding to be done in (y,x)/(z,y,x) when cropping validation data. Useful to avoid patch 'border effect'. This 
         # is only used when the validation is loaded from disk, and thus, not extracted from training. 
         _C.DATA.VAL.PADDING = (0,0)
-        # Directory where validation binary masks should be located. This binary mask will be applied only when MW_TH*
-        # optimized values are find, that is, when _C.PROBLEM.INSTANCE_SEG.DATA_MW_OPTIMIZE_THS = True and _C.TEST.POST_PROCESSING.APPLY_MASK = True
-        _C.DATA.VAL.BINARY_MASKS = os.path.join("user_data", 'val', 'bin_mask')
         # Not used yet.
         _C.DATA.VAL.RESOLUTION = (-1,)
         # Order of the axes of the image when using Zarr/H5 images to train
         _C.DATA.VAL.INPUT_IMG_AXES_ORDER = 'TZCYX'
         # Order of the axes of the mask when using Zarr/H5 images to train. 
         # detection the mask
         _C.DATA.VAL.INPUT_MASK_AXES_ORDER = 'TZCYX'
@@ -431,15 +430,15 @@
         _C.AUGMENTOR.SHIFT = False
         # Shift range. Translation as a fraction of the image height/width (x-translation, y-translation), where 0 denotes 
         # “no change” and 0.5 denotes “half of the axis size”.
         _C.AUGMENTOR.SHIFT_RANGE = (0.1, 0.2)
         # How to fill up the new values created with affine transformations (rotations, shear, shift and zoom).
         # Same meaning as in scipy: 'reflect', grid-'mirror', 'constant', 'grid-constant', 'nearest', 'mirror', 
         # 'grid-wrap' and 'wrap'. 
-        _C.AUGMENTOR.AFFINE_MODE = 'constant'
+        _C.AUGMENTOR.AFFINE_MODE = 'reflect'
         # Make vertical flips
         _C.AUGMENTOR.VFLIP = False
         # Make horizontal flips
         _C.AUGMENTOR.HFLIP = False
         # Make z-axis flips
         _C.AUGMENTOR.ZFLIP = False
         # Elastic transformations
@@ -839,15 +838,15 @@
         _C.TEST.EVALUATE = True
         # Stack 2D images into a 3D image and then process it entirely instead of going image per image
         _C.TEST.ANALIZE_2D_IMGS_AS_3D_STACK = False
         # Whether to reuse the existing ones (from file) or calculate predictions using the model
         _C.TEST.REUSE_PREDICTIONS = False
 
         # If PROBLEM.NDIM = '2D' this can be activated to process each image entirely instead of patch by patch. Only can be done 
-        # if the neural network is fully convolutional
+        # if the neural network is fully convolutional. It's not implemented in super-resolution workflow. 
         _C.TEST.FULL_IMG = False 
 
         ### Instance segmentation
         # Whether to calculate matching statistics (average overlap, accuracy, recall, precision, etc.)
         _C.TEST.MATCHING_STATS = True
         # Theshold of overlap to consider a TP when calculating the metrics. If more than one value is provided 
         # the process is repeated with each of the threshold values
@@ -887,17 +886,20 @@
         #~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
         # When PROBLEM.NDIM = '2D' only applies when _C.TEST.ANALIZE_2D_IMGS_AS_3D_STACK = True
         _C.TEST.POST_PROCESSING = CN()
         _C.TEST.POST_PROCESSING.YZ_FILTERING = False
         _C.TEST.POST_PROCESSING.YZ_FILTERING_SIZE = 5
         _C.TEST.POST_PROCESSING.Z_FILTERING = False
         _C.TEST.POST_PROCESSING.Z_FILTERING_SIZE = 5
-        # Apply a binary mask to remove possible segmentation outside it
+        # Apply a binary mask to remove possible segmentation outside it (you need to provide the mask and it must 
+        # contain two values: '1' -> preserve the pixel ; '0' discard pixel ). A mask for each test sample must be 
+        # provided and it will be loaded using 'DATA.TEST.BINARY_MASKS' variable.
         _C.TEST.POST_PROCESSING.APPLY_MASK = False
 
+        ### Instance segmentation
         # Whether to measure morphological features on each instances, i.e. 'circularity' (2D), 'elongation' (2D), 'npixels', 'area', 'diameter', 
         # 'perimeter', 'sphericity' (3D)
         _C.TEST.POST_PROCESSING.MEASURE_PROPERTIES = CN() 
         _C.TEST.POST_PROCESSING.MEASURE_PROPERTIES.ENABLE = False
         # Remove instances by the conditions based in each instance properties. The three variables, TEST.POST_PROCESSING.MEASURE_PROPERTIES.REMOVE_BY_PROPERTIES.PROPS, 
         # TEST.POST_PROCESSING.MEASURE_PROPERTIES.REMOVE_BY_PROPERTIES.VALUES and TEST.POST_PROCESSING.MEASURE_PROPERTIES.REMOVE_BY_PROPERTIES.SIGN will compose a list 
         # of conditions to remove the instances. They are list of list of conditions. For instance, the conditions can be like this: [['A'], ['B','C']]. Then, if the instance satisfies 
@@ -960,15 +962,14 @@
         # List of ints/float that represent the values of the properties listed in TEST.POST_PROCESSING.MEASURE_PROPERTIES.REMOVE_BY_PROPERTIES 
         # that the instances need to satisfy to not be dropped.
         _C.TEST.POST_PROCESSING.MEASURE_PROPERTIES.REMOVE_BY_PROPERTIES.VALUES = []
         # List of list of signs to do the comparison. Options: ['gt', 'ge', 'lt', 'le'] that corresponds to "greather than", e.g. ">", 
         # "greather equal", e.g. ">=", "less than", e.g. "<", and "less equal" e.g. "<=" comparisons.
         _C.TEST.POST_PROCESSING.MEASURE_PROPERTIES.REMOVE_BY_PROPERTIES.SIGN = []
 
-        ### Instance segmentation
         # Whether to apply Voronoi using 'BC' or 'M' channels need to be present
         _C.TEST.POST_PROCESSING.VORONOI_ON_MASK = False
         # Threshold to be applied to the 'M' channel when expanding the instances with Voronoi. Need to be in [0,1] range.
         # Leave it to 0 to adjust the threhold with Otsu
         _C.TEST.POST_PROCESSING.VORONOI_TH = 0.
         # Set it to try to repare large instances by merging their neighbors with them and removing possible central holes.  
         # Its value determines which instances are going to be repared by size (number of pixels that compose the instance)
@@ -982,15 +983,16 @@
         # To remove close points to each other. This can also be set when using 'BP' channels for instance segmentation.
         _C.TEST.POST_PROCESSING.REMOVE_CLOSE_POINTS = False
         # Distance between points to be considered the same. Only applies when TEST.POST_PROCESSING.REMOVE_CLOSE_POINTS = True
         # This can also be set when using 'BP' channels for instance segmentation.
         _C.TEST.POST_PROCESSING.REMOVE_CLOSE_POINTS_RADIUS = [-1.0]
         # Whether to apply a watershed to grow the points detected 
         _C.TEST.POST_PROCESSING.DET_WATERSHED = False
-        # Structure per each class to dilate the initial seeds before watershed
+        # Structure per each class to dilate the initial seeds before watershed. For instance, with two classes in a 3D problem:
+        # [ [2,2,1], [10,10,4] ]
         _C.TEST.POST_PROCESSING.DET_WATERSHED_FIRST_DILATION = [[-1,-1],]
         # List of classes to be consider as 'donuts'. For those class points, the 'donuts' type cell means that their nucleus is 
         # to big and that the seeds need to be dilated more so the watershed can grow the instances properly.
         _C.TEST.POST_PROCESSING.DET_WATERSHED_DONUTS_CLASSES = [-1]
         # Patch shape to extract all donuts type cells. It needs to be a bit greater than bigest donuts type cell so all of them can
         # be contained in this patch. This is used to analize that area for each point of class `DET_WATERSHED_DONUTS_CLASSES`.
         _C.TEST.POST_PROCESSING.DET_WATERSHED_DONUTS_PATCH = [13,120,120]
@@ -1010,24 +1012,24 @@
         _C.PATHS.RESULT_DIR.PER_IMAGE_INSTANCES = os.path.join(_C.PATHS.RESULT_DIR.PATH, 'per_image_instances')
         _C.PATHS.RESULT_DIR.PER_IMAGE_POST_PROCESSING = os.path.join(_C.PATHS.RESULT_DIR.PATH, 'per_image_post_processing')
         _C.PATHS.RESULT_DIR.FULL_IMAGE = os.path.join(_C.PATHS.RESULT_DIR.PATH, 'full_image')
         _C.PATHS.RESULT_DIR.FULL_IMAGE_BIN = os.path.join(_C.PATHS.RESULT_DIR.PATH, 'full_image_binarized')
         _C.PATHS.RESULT_DIR.FULL_IMAGE_INSTANCES = os.path.join(_C.PATHS.RESULT_DIR.PATH, 'full_image_instances')
         _C.PATHS.RESULT_DIR.FULL_IMAGE_POST_PROCESSING = os.path.join(_C.PATHS.RESULT_DIR.PATH, 'full_image_post_processing')
         _C.PATHS.RESULT_DIR.AS_3D_STACK = os.path.join(_C.PATHS.RESULT_DIR.PATH, 'as_3d_stack')
+        _C.PATHS.RESULT_DIR.AS_3D_STACK_BIN = os.path.join(_C.PATHS.RESULT_DIR.PATH, 'as_3d_stack_binarized')
         _C.PATHS.RESULT_DIR.AS_3D_STACK_POST_PROCESSING = os.path.join(_C.PATHS.RESULT_DIR.PATH, 'as_3d_stack_post_processing')
         _C.PATHS.RESULT_DIR.DET_LOCAL_MAX_COORDS_CHECK = os.path.join(_C.PATHS.RESULT_DIR.PATH, 'per_image_local_max_check')
         _C.PATHS.RESULT_DIR.DET_ASSOC_POINTS = os.path.join(_C.PATHS.RESULT_DIR.PATH, 'point_associations')
         _C.PATHS.RESULT_DIR.INST_ASSOC_POINTS = os.path.join(_C.PATHS.RESULT_DIR.PATH, 'instance_associations')
         
         # Path to store profiler files
         _C.PATHS.PROFILER = os.path.join(_C.PATHS.RESULT_DIR.PATH, 'profiler')
 
         # Name of the folder where the charts of the loss and metrics values while training the network are stored.
-        # Additionally, MW_TH* variable charts are stored if _C.PROBLEM.INSTANCE_SEG.DATA_MW_OPTIMIZE_THS = True
         _C.PATHS.CHARTS = os.path.join(_C.PATHS.RESULT_DIR.PATH, 'charts')
         # Folder where samples of DA will be stored
         _C.PATHS.DA_SAMPLES = os.path.join(_C.PATHS.RESULT_DIR.PATH, 'aug')
         # Folder where generator samples (X) will be stored
         _C.PATHS.GEN_CHECKS = os.path.join(_C.PATHS.RESULT_DIR.PATH, 'gen_check')
         # Folder where generator samples (Y) will be stored
         _C.PATHS.GEN_MASK_CHECKS = os.path.join(_C.PATHS.RESULT_DIR.PATH, 'gen_mask_check')
@@ -1087,16 +1089,14 @@
         self._C.DATA.TRAIN.INSTANCE_CHANNELS_DIR = self._C.DATA.TRAIN.PATH+'_'+self._C.PROBLEM.INSTANCE_SEG.DATA_CHANNELS+'_'+self._C.PROBLEM.INSTANCE_SEG.DATA_CONTOUR_MODE
         self._C.DATA.TRAIN.INSTANCE_CHANNELS_MASK_DIR = self._C.DATA.TRAIN.GT_PATH+'_'+self._C.PROBLEM.INSTANCE_SEG.DATA_CHANNELS+'_'+self._C.PROBLEM.INSTANCE_SEG.DATA_CONTOUR_MODE
         self._C.DATA.TRAIN.DETECTION_MASK_DIR = self._C.DATA.TRAIN.GT_PATH+'_detection_masks'
         self._C.DATA.TRAIN.SSL_SOURCE_DIR = self._C.DATA.TRAIN.PATH+'_ssl_source'
         self._C.DATA.VAL.INSTANCE_CHANNELS_DIR = self._C.DATA.VAL.PATH+'_'+self._C.PROBLEM.INSTANCE_SEG.DATA_CHANNELS+'_'+self._C.PROBLEM.INSTANCE_SEG.DATA_CONTOUR_MODE
         self._C.DATA.VAL.INSTANCE_CHANNELS_MASK_DIR = self._C.DATA.VAL.GT_PATH+'_'+self._C.PROBLEM.INSTANCE_SEG.DATA_CHANNELS+'_'+self._C.PROBLEM.INSTANCE_SEG.DATA_CONTOUR_MODE
         # If value is not the default
-        if self._C.DATA.VAL.BINARY_MASKS == os.path.join("user_data", 'val', 'bin_mask'):
-            self._C.DATA.VAL.BINARY_MASKS = os.path.join(self._C.DATA.VAL.PATH, '..', 'bin_mask')
         self._C.DATA.VAL.DETECTION_MASK_DIR = self._C.DATA.VAL.GT_PATH+'_detection_masks'
         self._C.DATA.VAL.SSL_SOURCE_DIR = self._C.DATA.VAL.PATH+'_ssl_source'
         self._C.DATA.TEST.INSTANCE_CHANNELS_DIR = self._C.DATA.TEST.PATH+'_'+self._C.PROBLEM.INSTANCE_SEG.DATA_CHANNELS+'_'+self._C.PROBLEM.INSTANCE_SEG.DATA_CONTOUR_MODE
         self._C.DATA.TEST.INSTANCE_CHANNELS_MASK_DIR = self._C.DATA.TEST.GT_PATH+'_'+self._C.PROBLEM.INSTANCE_SEG.DATA_CHANNELS+'_'+self._C.PROBLEM.INSTANCE_SEG.DATA_CONTOUR_MODE
         # If value is not the default
         if self._C.DATA.TEST.BINARY_MASKS == os.path.join("user_data", 'test', 'bin_mask'):
             self._C.DATA.TEST.BINARY_MASKS = os.path.join(self._C.DATA.TEST.PATH, '..', 'bin_mask')
```

### Comparing `biapy-3.4.2/biapy/data/data_2D_manipulation.py` & `biapy-3.4.3/biapy/data/data_2D_manipulation.py`

 * *Files 6% similar despite different names*

```diff
@@ -98,15 +98,15 @@
 
     Y_val : 4D Numpy array, optional
         Validation images' mask (``val_split > 0``). E.g. ``(num_of_images, y, x, channels)``.
 
     filenames : List of str
         Loaded train filenames.
 
-    val_index : List of ints
+    test_index : List of ints
         Indexes of the samples beloging to the validation.
 
     Examples
     --------
     ::
 
         # EXAMPLE 1
@@ -140,25 +140,24 @@
         #    *** Loaded validation data shape is: (204, 256, 256, 1)
 
     """
 
     print("### LOAD ###")
 
     # Disable crops when random_crops_in_DA is selected
-    # Disable crops when random_crops_in_DA is selected
+    delay_crop = False
     if random_crops_in_DA:
         crop = False  
     else:
         if cross_val:
             crop = False
             # Delay the crop to be made after cross validation
             delay_crop = True  
         else:
             crop = True
-            delay_crop = False  
 
     # Check validation
     if val_split > 0 or cross_val:
         create_val = True  
     else:
         create_val = False
 
@@ -168,14 +167,27 @@
         convert_to_rgb=convert_to_rgb, preprocess_cfg=preprocess_cfg, is_mask=False, preprocess_f=preprocess_f)
     if train_mask_path is not None:                                            
         print("1) Loading train GT . . .")
         scrop = (crop_shape[0]*y_upscaling[0], crop_shape[1]*y_upscaling[1], crop_shape[2])
         Y_train, _, _, _ = load_data_from_dir(train_mask_path, crop=crop, crop_shape=scrop, overlap=ov, padding=padding, 
             return_filenames=True, check_channel=False, check_drange=False, reflect_to_complete_shape=reflect_to_complete_shape,
             preprocess_cfg=preprocess_cfg, is_mask=is_y_mask, preprocess_f=preprocess_f)
+        
+        # Check that the shape of all images match
+        if isinstance(Y_train, list):
+            for i in range(len(Y_train)):
+                xshape = X_train[i].shape
+                yshape = Y_train[i].shape
+                real_x_shape = (xshape[0]*y_upscaling[0], xshape[1]*y_upscaling[1], xshape[2]) 
+                real_y_shape = (yshape[0]*y_upscaling[0], yshape[1]*y_upscaling[1], yshape[2])
+                print(real_x_shape,real_y_shape)
+                if real_x_shape != real_y_shape:
+                    raise ValueError(f"There is a mismatch between input image and its corresponding ground truth ({real_x_shape} vs "
+                        f"{real_y_shape}). Please check the images. Specifically, the sample that doesn't match is the number {i}"
+                        f" (file: {t_filenames[i]})")
     else:
         Y_train = None
     
     # Discard images that do not surpass the foreground percentage threshold imposed 
     if minimum_foreground_perc != -1 and Y_train is not None:
         print("Data that do not have {}% of foreground is discarded".format(minimum_foreground_perc))
 
@@ -253,81 +265,108 @@
             else:
                 X_train, X_val = train_test_split(
                     X_train, test_size=val_split, shuffle=shuffle_val, random_state=seed)
         else:
             skf = StratifiedKFold(n_splits=cross_val_nsplits, shuffle=shuffle_val,
                 random_state=seed)
             fold = 1
-            train_index, val_index = None, None
+            train_index, test_index = None, None
 
             y_len = len(Y_train) if Y_train is not None else len(X_train)
             for t_index, te_index in skf.split(np.zeros(len(X_train)), np.zeros(y_len)):
                 if cross_val_fold == fold:
-                    X_train, X_val = X_train[t_index], X_train[te_index]
+                    if not isinstance(X_train, list):
+                        X_train, X_val = X_train[t_index], X_train[te_index]
+                    else:
+                        X_val = []
+                        for val_idx in te_index:
+                            X_val.append(X_train[val_idx])
+                        for val_idx in te_index:
+                            del X_val[val_idx]
                     if Y_train is not None:
-                        Y_train, Y_val = Y_train[t_index], Y_train[te_index]
+                        if not isinstance(Y_train, list):
+                            Y_train, Y_val = Y_train[t_index], Y_train[te_index]
+                        else:
+                            Y_val = []
+                            for val_idx in te_index:
+                                Y_val.append(Y_val[val_idx])
+                            for val_idx in te_index:
+                                del Y_val[val_idx]
                     train_index, test_index = t_index.copy(), te_index.copy()
                     break
                 fold+= 1
 
-            if len(val_index) > 5:
-                print("Fold number {}. Printing the first 5 ids: {}".format(fold, val_index[:5]))
+            if len(test_index) > 5:
+                print("Fold number {}. Printing the first 5 ids: {}".format(fold, test_index[:5]))
             else:
-                print("Fold number {}. Indexes used in cross validation: {}".format(fold, val_index))
+                print("Fold number {}. Indexes used in cross validation: {}".format(fold, test_index))
 
             # Then crop after cross validation
             if delay_crop:
                 # X_train
                 data = []
                 for img_num in range(len(X_train)):
                     if X_train[img_num].shape != crop_shape[:2]+(X_train[img_num].shape[-1],):
-                        img = X_train[img_num]
-                        img = crop_2D_data_with_overlap(X_train[img_num][0] if isinstance(X_train, list) else X_train[img_num], 
+                        img = crop_data_with_overlap(
+                            X_train[img_num][0] if isinstance(X_train, list) else np.expand_dims(X_train[img_num],0), 
                             crop_shape[:2]+(X_train[img_num].shape[-1],), overlap=ov, padding=padding, verbose=False)
                     data.append(img)
                 X_train = np.concatenate(data)
                 del data
 
                 # Y_train
                 if Y_train is not None:
                     data_mask = []
                     scrop = (crop_shape[0]*y_upscaling[0], crop_shape[1]*y_upscaling[1], crop_shape[2])
                     for img_num in range(len(Y_train)):
                         if Y_train[img_num].shape != scrop[:2]+(Y_train[img_num].shape[-1],):
-                            img = Y_train[img_num]
-                            img = crop_2D_data_with_overlap(Y_train[img_num][0] if isinstance(Y_train, list) else Y_train[img_num],
+                            img = crop_data_with_overlap(
+                                Y_train[img_num][0] if isinstance(Y_train, list) else np.expand_dims(Y_train[img_num],0),
                                 scrop[:2]+(Y_train[img_num].shape[-1],), overlap=ov, padding=padding, verbose=False)
                         data_mask.append(img)
                     Y_train = np.concatenate(data_mask)
                     del data_mask
                 
                 # X_val
                 data = []
                 for img_num in range(len(X_val)):
                     if X_val[img_num].shape != crop_shape[:2]+(X_val[img_num].shape[-1],):
-                        img = X_val[img_num]
-                        img = crop_2D_data_with_overlap(X_val[img_num][0] if isinstance(X_val, list) else X_val[img_num], 
+                        img = crop_data_with_overlap(
+                            X_val[img_num][0] if isinstance(X_val, list) else np.expand_dims(X_val[img_num],0), 
                             crop_shape[:2]+(X_val[img_num].shape[-1],), overlap=ov, padding=padding, verbose=False)
                     data.append(img)
                 X_val = np.concatenate(data)
                 del data
 
                 # Y_val
                 if Y_val is not None:
                     data_mask = []
                     scrop = (crop_shape[0]*y_upscaling[0], crop_shape[1]*y_upscaling[1], crop_shape[2])
                     for img_num in range(len(Y_val)):
                         if Y_val[img_num].shape != scrop[:2]+(Y_val[img_num].shape[-1],):
-                            img = Y_val[img_num]
-                            img = crop_2D_data_with_overlap(Y_val[img_num][0] if isinstance(Y_val, list) else Y_val[img_num],
+                            img = crop_data_with_overlap(
+                                Y_val[img_num][0] if isinstance(Y_val, list) else np.expand_dims(Y_val[img_num],0),
                                 scrop[:2]+(Y_val[img_num].shape[-1],), overlap=ov, padding=padding, verbose=False)
                         data_mask.append(img)
                     Y_val = np.concatenate(data_mask)
                     del data_mask
 
+    # Check that the shape of all images match
+    if Y_train is not None:
+        if not isinstance(X_train, list):
+            if Y_train.shape[0] != X_train.shape[0]:
+                raise ValueError(f"Seems that input images do not correspond to their ground truth in shape ({X_train.shape[0]} samples vs "
+                    f"{Y_train.shape[0]} samples). Please check the images. If you are in super-resolution workflow maybe you did not "
+                    "configured properly 'PROBLEM.SUPER_RESOLUTION.UPSCALING' variable")
+        else:
+            if Y_train[0].shape[0] != X_train[0].shape[0]:
+                raise ValueError(f"Seems that input images do not correspond to their ground truth in shape ({X_train[0].shape[0]} samples vs "
+                    f"{Y_train[0].shape[0]} samples). Please check the images. If you are in super-resolution workflow maybe you did not "
+                    "configured properly 'PROBLEM.SUPER_RESOLUTION.UPSCALING' variable")
+
     s = X_train.shape if not isinstance(X_train, list) else (len(X_train),)+X_train[0].shape[1:]
     if Y_train is not None:
         sm = Y_train.shape if not isinstance(Y_train, list) else (len(Y_train),)+Y_train[0].shape[1:]
     if create_val:
         sv = X_val.shape if not isinstance(X_val, list) else (len(X_val),)+X_val[0].shape[1:]
         if Y_val is not None:
             svm = Y_val.shape if not isinstance(Y_val, list) else (len(Y_val),)+Y_val[0].shape[1:]
@@ -340,15 +379,15 @@
         if Y_val is not None:
             print("*** Loaded validation GT shape is: {}".format(svm))
         print("### END LOAD ###")
 
         if not cross_val:
             return X_train, Y_train, X_val, Y_val, t_filenames
         else:
-            return X_train, Y_train, X_val, Y_val, t_filenames, val_index
+            return X_train, Y_train, X_val, Y_val, t_filenames, test_index
     else:
         print("*** Loaded train data shape is: {}".format(s))
         print("### END LOAD ###")
 
         return X_train, Y_train, t_filenames
 
 
@@ -439,15 +478,19 @@
            #     Minimum overlap selected: (0.5, 0)
            #     Real overlapping (%): (0.59765625, 0.0)
            #     Real overlapping (pixels): (153.0, 0.0)
            #     (6, 4) patches per (x,y) axis
            #     **** New data shape is: (3960, 256, 256, 1)
     """
 
+    if data.ndim != 4:
+        raise ValueError("data expected to be 4 dimensional, given {}".format(data.shape))
     if data_mask is not None:
+        if data.ndim != 4:
+            raise ValueError("data mask expected to be 4 dimensional, given {}".format(data_mask.shape))
         if data.shape[:-1] != data_mask.shape[:-1]:
             raise ValueError("data and data_mask shapes mismatch: {} vs {}".format(data.shape[:-1], data_mask.shape[:-1]))
 
     for i,p in enumerate(padding):
         if p >= crop_shape[i]//2:
             raise ValueError("'Padding' can not be greater than the half of 'crop_shape'. Max value for this {} input shape is {}"
                               .format(data.shape, [(crop_shape[0]//2)-1,(crop_shape[1]//2)-1]))
@@ -795,16 +838,16 @@
 
     if data_mask is not None:
         return merged_data, merged_data_mask
     else:
         return merged_data
 
 
-def load_data_classification(data_dir, patch_shape, convert_to_rgb=True, expected_classes=None, cross_val=False, cross_val_nsplits=5, cross_val_fold=1, 
-    val_split=0.1, seed=0, shuffle_val=True):
+def load_data_classification(data_dir, patch_shape, convert_to_rgb=True, expected_classes=None, cross_val=False, cross_val_nsplits=5, 
+    cross_val_fold=1, val_split=0.1, seed=0, shuffle_val=True, preprocess_cfg=None, preprocess_f=None):
     """
     Load data to train classification methods.
 
     Parameters
     ----------
     data_dir : str
         Path to the training data.
@@ -833,14 +876,20 @@
 
     seed : int, optional
         Seed value.
 
     shuffle_val : bool, optional
         Take random training examples to create validation data.
 
+    preprocess_cfg : dict, optional
+        Configuration parameters for preprocessing, is necessary in case you want to apply any preprocessing.
+    
+    preprocess_f : function, optional
+        The preprocessing function, is necessary in case you want to apply any preprocessing.
+
     Returns
     -------
     X_data : 4D Numpy array
         Train images. E.g. ``(num_of_images, y, x, channels)``.
 
     Y_data : 4D Numpy array
         Train images' mask. E.g. ``(num_of_images, y, x, channels)``.
@@ -850,15 +899,15 @@
 
     Y_val : 4D Numpy array, optional
         Validation images' mask (``val_split > 0``). E.g. ``(num_of_images, y, x, channels)``.
 
     all_ids : List of str
         Loaded data filenames.
 
-    val_index : List of ints
+    test_index : List of ints
         Indexes of the samples beloging to the validation.
     """
 
     print("### LOAD ###")
 
     # Check validation
     if val_split > 0 or cross_val:
@@ -885,15 +934,16 @@
         if len(ids) == 0:
             raise ValueError("There are no images in class {}".format(f))
         else:
             print("Found {} samples".format(len(ids)))
 
         # Loading images 
         images, _, _, image_ids = load_data_from_dir(f, return_filenames=True, crop_shape=patch_shape, 
-            convert_to_rgb=convert_to_rgb)
+            convert_to_rgb=convert_to_rgb, preprocess_cfg=preprocess_cfg, is_mask=False, 
+            preprocess_f=preprocess_f)
 
         X_data.append(images)
         Y_data.append((c_num,)*len(ids))
         all_ids += image_ids
 
     # Fuse all data
     try:
@@ -904,39 +954,54 @@
     Y_data = np.concatenate(Y_data, 0)
     Y_data = np.squeeze(Y_data)
 
     # Create validation data splitting the train
     if create_val:
         print("Creating validation data")
         if not cross_val:
+            if len(X_data) == 1:
+                raise ValueError("Validation data can not be extracted from training data as it only has one sample. Please check the data.")
             X_data, X_val, Y_data, Y_val = train_test_split(
                 X_data, Y_data, test_size=val_split, shuffle=shuffle_val, random_state=seed,
                 stratify=Y_data)
         else:
+            if len(X_data) < cross_val_nsplits:
+                raise ValueError(f"Validation data can not be extracted from training data as the number of splits ({cross_val_nsplits}) "
+                    f"is greater than the number of samples {len(X_data)}. Please check the data.")
             skf = StratifiedKFold(n_splits=cross_val_nsplits, shuffle=shuffle_val,
                 random_state=seed)
             fold = 1
-            train_index, val_index = None, None
+            train_index, test_index = None, None
 
             for t_index, te_index in skf.split(X_data, Y_data):
                 if cross_val_fold == fold:
-                    X_data, X_val = X_data[t_index], X_data[te_index]
-                    Y_data, Y_val = Y_data[t_index], Y_data[te_index]
-                    train_index, val_index = t_index.copy(), te_index.copy()
+                    if not isinstance(X_data, list):
+                        X_data, X_val = X_data[t_index], X_data[te_index]
+                        Y_data, Y_val = Y_data[t_index], Y_data[te_index]
+                    else:
+                        X_val = []
+                        Y_val = []
+                        for val_idx in te_index:
+                            X_val.append(X_data[val_idx])
+                            Y_val.append(Y_data[val_idx])
+                        for val_idx in te_index:
+                            del X_val[val_idx]
+                            del Y_val[val_idx]
+                    train_index, test_index = t_index.copy(), te_index.copy()
                     break
                 fold+= 1
-            if len(val_index) > 5:
-                print("Fold number {}. Printing the first 5 ids: {}".format(fold, val_index[:5]))
+            if len(test_index) > 5:
+                print("Fold number {}. Printing the first 5 ids: {}".format(fold, test_index[:5]))
             else:
-                print("Fold number {}. Indexes used in cross validation: {}".format(fold, val_index))
+                print("Fold number {}. Indexes used in cross validation: {}".format(fold, test_index))
 
     if create_val:
         print("*** Loaded train data shape is: {}".format(X_data.shape))
         print("*** Loaded validation data shape is: {}".format(X_val.shape))
         if not cross_val:
             return X_data, Y_data, X_val, Y_val, all_ids
         else:
-            return X_data, Y_data, X_val, Y_val, all_ids, val_index
+            return X_data, Y_data, X_val, Y_val, all_ids, test_index
     else:
         print("*** Loaded train data shape is: {}".format(X_data.shape))
         return X_data, Y_data, all_ids
```

### Comparing `biapy-3.4.2/biapy/data/data_3D_manipulation.py` & `biapy-3.4.3/biapy/data/data_3D_manipulation.py`

 * *Files 8% similar despite different names*

```diff
@@ -124,24 +124,24 @@
         #     *** Loaded validation mask shape is: (35, 40, 256, 256, 1)
         #
     """
 
     print("### LOAD ###")
 
     # Disable crops when random_crops_in_DA is selected
+    delay_crop = False
     if random_crops_in_DA:
         crop = False  
     else:
         if cross_val:
             crop = False
             # Delay the crop to be made after cross validation
             delay_crop = True  
         else:
             crop = True
-            delay_crop = False  
 
     # Check validation
     if val_split > 0 or cross_val:
         create_val = True  
     else:
         create_val = False
 
@@ -152,23 +152,29 @@
 
     if train_mask_path is not None:
         print("1) Loading train GT . . .")
         scrop = (crop_shape[0]*y_upscaling[0], crop_shape[1]*y_upscaling[1], crop_shape[2]*y_upscaling[2], crop_shape[3])
         Y_train, _, _ = load_3d_images_from_dir(train_mask_path, crop=crop, crop_shape=scrop, overlap=ov,
             padding=padding, reflect_to_complete_shape=reflect_to_complete_shape, check_channel=False, check_drange=False,
             preprocess_cfg=preprocess_cfg, is_mask=is_y_mask, preprocess_f=preprocess_f)
+
+        # Check that the shape of all images match
+        if isinstance(Y_train, list):
+            for i in range(len(Y_train)):
+                xshape = X_train[i].shape
+                yshape = Y_train[i].shape
+                real_x_shape = (xshape[0]*y_upscaling[0], xshape[1]*y_upscaling[1], xshape[2]*y_upscaling[2], xshape[3]) 
+                real_y_shape = (yshape[0]*y_upscaling[0], yshape[1]*y_upscaling[1], yshape[2]*y_upscaling[2], yshape[3])
+                if real_x_shape != real_y_shape:
+                    raise ValueError(f"There is a mismatch between input image and its corresponding ground truth ({real_x_shape} vs "
+                        f"{real_y_shape}). Please check the images. Specifically, the sample that doesn't match is the number {i}"
+                        f" (file: {t_filenames[i]})")
     else:
         Y_train = None
 
-    if isinstance(X_train, list):
-        raise NotImplementedError("If you arrived here means that your images are not all of the same shape, and you "
-                                  "select DATA.EXTRACT_RANDOM_PATCH = True, so no crops are made to ensure all images "
-                                  "have the same shape. Please, crop them into your DATA.PATCH_SIZE and run again (you "
-                                  "can use one of the script from here to crop: https://github.com/BiaPyX/BiaPy/tree/master/biapy/utils/scripts)")
-
     # Discard images that do not surpass the foreground percentage threshold imposed 
     if minimum_foreground_perc != -1 and Y_train is not None:
         print("Data that do not have {}% of foreground is discarded".format(minimum_foreground_perc))
 
         X_train_keep = []
         Y_train_keep = []
         are_lists = True if type(Y_train) is list else False
@@ -228,32 +234,50 @@
             "Please check the data!".format(len(X_train), len(Y_train)))
             
     # Create validation data splitting the train
     if create_val:
         print("Creating validation data")
         Y_val = None
         if not cross_val:
+            if len(X_train) == 1:
+                raise ValueError("Validation data can not be extracted from training data as it only has one sample. Please check the data.")
             if Y_train is not None:
                 X_train, X_val, Y_train, Y_val = train_test_split(
                     X_train, Y_train, test_size=val_split, shuffle=shuffle_val, random_state=seed)
             else:
                 X_train, X_val = train_test_split(
                     X_train, test_size=val_split, shuffle=shuffle_val, random_state=seed)
         else:
+            if len(X_train) < cross_val_nsplits:
+                raise ValueError(f"Validation data can not be extracted from training data as the number of splits ({cross_val_nsplits}) "
+                    f"is greater than the number of samples {len(X_train)}. Please check the data.")
             skf = StratifiedKFold(n_splits=cross_val_nsplits, shuffle=shuffle_val,
                 random_state=seed)
             fold = 1
             train_index, test_index = None, None
-
             y_len = len(Y_train) if Y_train is not None else len(X_train)
             for t_index, te_index in skf.split(np.zeros(len(X_train)), np.zeros(y_len)):
                 if cross_val_fold == fold:
-                    X_train, X_val = X_train[t_index], X_train[te_index]
+                    if not isinstance(X_train, list):
+                        X_train, X_val = X_train[t_index], X_train[te_index]
+                    else:
+                        X_val = []
+                        for val_idx in te_index:
+                            X_val.append(X_train[val_idx])
+                        for val_idx in te_index:
+                            del X_train[val_idx]
                     if Y_train is not None:
-                        Y_train, Y_val = Y_train[t_index], Y_train[te_index]
+                        if not isinstance(X_train, list):
+                            Y_train, Y_val = Y_train[t_index], Y_train[te_index]
+                        else:
+                            Y_val = []
+                            for val_idx in te_index:
+                                Y_val.append(Y_train[val_idx])
+                            for val_idx in te_index:
+                                del Y_train[val_idx]
                     train_index, test_index = t_index.copy(), te_index.copy()
                     break
                 fold+= 1
 
             if len(test_index) > 5:
                 print("Fold number {}. Printing the first 5 ids: {}".format(fold, test_index[:5]))
             else:
@@ -261,75 +285,93 @@
 
             # Then crop after cross validation
             if delay_crop:
                 # X_train
                 data = []
                 for img_num in range(len(X_train)):
                     if X_train[img_num].shape != crop_shape[:3]+(X_train[img_num].shape[-1],):
-                        img = X_train[img_num]
                         img = crop_3D_data_with_overlap(X_train[img_num][0] if isinstance(X_train, list) else X_train[img_num], 
                             crop_shape[:3]+(X_train[img_num].shape[-1],), overlap=ov, padding=padding, verbose=False)
                     data.append(img)
                 X_train = np.concatenate(data)
                 del data
 
                 # Y_train
                 if Y_train is not None:
                     data_mask = []
-                    scrop = (crop_shape[0], crop_shape[1]*y_upscaling[0], crop_shape[2]*y_upscaling[1], crop_shape[3]*y_upscaling[2])
+                    scrop = (crop_shape[0]*y_upscaling[0], crop_shape[1]*y_upscaling[1], crop_shape[2]*y_upscaling[2], crop_shape[3])
                     for img_num in range(len(Y_train)):
                         if Y_train[img_num].shape != scrop[:3]+(Y_train[img_num].shape[-1],):
-                            img = Y_train[img_num]
                             img = crop_3D_data_with_overlap(Y_train[img_num][0] if isinstance(Y_train, list) else Y_train[img_num],
                                 scrop[:3]+(Y_train[img_num].shape[-1],), overlap=ov, padding=padding, verbose=False)
                         data_mask.append(img)
                     Y_train = np.concatenate(data_mask)
                     del data_mask
                     
                 # X_val
                 data = []
                 for img_num in range(len(X_val)):
                     if X_val[img_num].shape != crop_shape[:3]+(X_val[img_num].shape[-1],):
-                        img = X_val[img_num]
                         img = crop_3D_data_with_overlap(X_val[img_num][0] if isinstance(X_val, list) else X_val[img_num], 
                             crop_shape[:3]+(X_val[img_num].shape[-1],), overlap=ov, padding=padding, verbose=False)
                     data.append(img)
                 X_val = np.concatenate(data)
                 del data
 
                 # Y_val
                 if Y_val is not None:
                     data_mask = []
-                    scrop = (crop_shape[0], crop_shape[1]*y_upscaling[0], crop_shape[2]*y_upscaling[1], crop_shape[3]*y_upscaling[2])
+                    scrop = (crop_shape[0]*y_upscaling[0], crop_shape[1]*y_upscaling[1], crop_shape[2]*y_upscaling[2], crop_shape[3])
                     for img_num in range(len(Y_val)):
                         if Y_val[img_num].shape != scrop[:3]+(Y_val[img_num].shape[-1],):
-                            img = Y_val[img_num]
                             img = crop_3D_data_with_overlap(Y_val[img_num][0] if isinstance(Y_val, list) else Y_val[img_num],
                                 scrop[:3]+(Y_val[img_num].shape[-1],), overlap=ov, padding=padding, verbose=False)
                         data_mask.append(img)
                     Y_val = np.concatenate(data_mask)
                     del data_mask
 
     # Convert the original volumes as they were a unique subvolume
-    if random_crops_in_DA and X_train.ndim == 4:
+    if random_crops_in_DA and not isinstance(X_train, list) and X_train.ndim == 4:
         X_train = np.expand_dims(X_train, axis=0)
         if Y_train is not None:
             Y_train = np.expand_dims(Y_train, axis=0)
         if create_val:
             X_val = np.expand_dims(X_val, axis=0)
             if Y_val is not None:
                 Y_val = np.expand_dims(Y_val, axis=0)
 
+    # Check that the shape of all images match
+    if Y_train is not None:
+        if not isinstance(X_train, list):
+            if Y_train.shape[0] != X_train.shape[0]:
+                raise ValueError(f"Seems that input images do not correspond to their ground truth in shape ({X_train.shape[0]} samples vs "
+                    f"{Y_train.shape[0]} samples). Please check the images. If you are in super-resolution workflow maybe you did not "
+                    "configured properly 'PROBLEM.SUPER_RESOLUTION.UPSCALING' variable")
+        else:
+            if Y_train[0].shape[0] != X_train[0].shape[0]:
+                raise ValueError(f"Seems that input images do not correspond to their ground truth in shape ({X_train[0].shape[0]} samples vs "
+                    f"{Y_train[0].shape[0]} samples). Please check the images. If you are in super-resolution workflow maybe you did not "
+                    "configured properly 'PROBLEM.SUPER_RESOLUTION.UPSCALING' variable")
+
+    s = X_train.shape if not isinstance(X_train, list) else (len(X_train),)+X_train[0].shape[1:]
+    if Y_train is not None:
+        sm = Y_train.shape if not isinstance(Y_train, list) else (len(Y_train),)+Y_train[0].shape[1:]
     if create_val:
-        print("*** Loaded train data shape is: {}".format(X_train.shape))
+        sv = X_val.shape if not isinstance(X_val, list) else (len(X_val),)+X_val[0].shape[1:]
+        if Y_val is not None:
+            svm = Y_val.shape if not isinstance(Y_val, list) else (len(Y_val),)+Y_val[0].shape[1:]
+        if not isinstance(X_train, list):
+            print("Not all samples seem to have the same shape. Number of samples: {}".format(len(X_train)))
+        print("*** Loaded train data shape is: {}".format(s))
         if Y_train is not None:
-            print("*** Loaded train GT shape is: {}".format(Y_train.shape))
-        print("*** Loaded validation data shape is: {}".format(X_val.shape))
+            print("*** Loaded train GT shape is: {}".format(sm))
+        print("*** Loaded validation data shape is: {}".format(sv))
         if Y_val is not None:
-            print("*** Loaded validation GT shape is: {}".format(Y_val.shape))
+            print("*** Loaded validation GT shape is: {}".format(svm))
+        print("### END LOAD ###")
         if not cross_val:
             return X_train, Y_train, X_val, Y_val, t_filenames
         else:
             return X_train, Y_train, X_val, Y_val, t_filenames, test_index
     else:
         print("*** Loaded train data shape is: {}".format(X_train.shape))
         if Y_train is not None:
@@ -510,17 +552,31 @@
                 random_state=seed)
             fold = 1
             train_index, test_index = None, None
 
             y_len = len(Y_train) if Y_train is not None else len(X_train)
             for t_index, te_index in skf.split(np.zeros(len(X_train)), np.zeros(y_len)):
                 if cross_val_fold == fold:
-                    X_train, X_val = X_train[t_index], X_train[te_index]
+                    if not isinstance(X_train, list):
+                        X_train, X_val = X_train[t_index], X_train[te_index]
+                    else:
+                        X_val = []
+                        for val_idx in te_index:
+                            X_val.append(X_train[val_idx])
+                        for val_idx in te_index:
+                            del X_train[val_idx]
                     if Y_train is not None:
-                        Y_train, Y_val = Y_train[t_index], Y_train[te_index]
+                        if not isinstance(X_train, list):
+                            Y_train, Y_val = Y_train[t_index], Y_train[te_index]
+                        else:
+                            Y_val = []
+                            for val_idx in te_index:
+                                Y_val.append(Y_train[val_idx])  
+                            for val_idx in te_index:
+                                del Y_train[val_idx]                              
                     train_index, test_index = t_index.copy(), te_index.copy()
                     break
                 fold+= 1
 
             if len(test_index) > 5:
                 print("Fold number {}. Printing the first 5 ids: {}".format(fold, test_index[:5]))
             else:
@@ -1107,15 +1163,15 @@
         raise ValueError("'vol_shape[2]' {} greater than {} (you can reduce 'DATA.PATCH_SIZE')"
             .format(vol_shape[2], x_dim))
     if (overlap[0] >= 1 or overlap[0] < 0) or (overlap[1] >= 1 or overlap[1] < 0) or (overlap[2] >= 1 or overlap[2] < 0):
         raise ValueError("'overlap' values must be floats between range [0, 1)")
     for i,p in enumerate(padding):
         if p >= vol_shape[i]//2:
             raise ValueError("'Padding' can not be greater than the half of 'vol_shape'. Max value for this {} input shape is {}"
-                             .format(data_shape, [(vol_shape[0]//2)-1,(vol_shape[1]//2)-1,(vol_shape[2]//2)-1]))
+                             .format(data.shape, [(vol_shape[0]//2)-1,(vol_shape[1]//2)-1,(vol_shape[2]//2)-1]))
 
     padded_data_shape = [z_dim+padding[0]*2,y_dim+padding[1]*2,x_dim+padding[2]*2,c_dim]
     padded_vol_shape = vol_shape
 
     # Calculate overlapping variables
     overlap_z = 1 if overlap[0] == 0 else 1-overlap[0]
     overlap_y = 1 if overlap[1] == 0 else 1-overlap[1]
@@ -1252,15 +1308,15 @@
                 if rank == 0:
                     yield img, real_patch_in_data, total_vol, z_vol_info, list_of_vols_in_z
                 else:
                     yield img, real_patch_in_data, total_vol
 
 
 def load_3d_data_classification(data_dir, patch_shape, convert_to_rgb=False, expected_classes=None, cross_val=False, cross_val_nsplits=5, 
-    cross_val_fold=1, val_split=0.1, seed=0, shuffle_val=True):
+    cross_val_fold=1, val_split=0.1, seed=0, shuffle_val=True, preprocess_cfg=None, preprocess_f=None):
     """
     Load 3D data to train classification methods.
 
     Parameters
     ----------
     data_dir : str
         Path to the training data.
@@ -1289,14 +1345,20 @@
 
     seed : int, optional
         Seed value.
 
     shuffle_val : bool, optional
         Take random training examples to create validation data.
 
+    preprocess_cfg : dict, optional
+        Configuration parameters for preprocessing, is necessary in case you want to apply any preprocessing.
+    
+    preprocess_f : function, optional
+        The preprocessing function, is necessary in case you want to apply any preprocessing.
+
     Returns
     -------
     X_data : 5D Numpy array
         Train/test images. E.g. ``(num_of_images, z, y, x, channels)``.
 
     Y_data : 1D Numpy array
         Train/test images' classes. E.g. ``(num_of_images)``.
@@ -1341,15 +1403,16 @@
         if len(ids) == 0:
             raise ValueError("There are no images in class {}".format(f))
         else:
             print("Found {} samples".format(len(ids)))
 
         # Loading images 
         images, _, _, image_ids = load_3d_images_from_dir(f, return_filenames=True, crop_shape=patch_shape, 
-            convert_to_rgb=convert_to_rgb)
+            convert_to_rgb=convert_to_rgb, preprocess_cfg=preprocess_cfg, is_mask=False, 
+            preprocess_f=preprocess_f)
 
         X_data.append(images)
         Y_data.append((c_num,)*len(ids))
         all_ids += image_ids
 
     # Fuse all data
     X_data = np.concatenate(X_data, 0)
@@ -1366,16 +1429,26 @@
             skf = StratifiedKFold(n_splits=cross_val_nsplits, shuffle=shuffle_val,
                 random_state=seed)
             fold = 1
             train_index, test_index = None, None
 
             for t_index, te_index in skf.split(X_data, Y_data):
                 if cross_val_fold == fold:
-                    X_data, X_val = X_data[t_index], X_data[te_index]
-                    Y_data, Y_val = Y_data[t_index], Y_data[te_index]
+                    if not isinstance(X_data, list):
+                        X_data, X_val = X_data[t_index], X_data[te_index]
+                        Y_data, Y_val = Y_data[t_index], Y_data[te_index]
+                    else:
+                        X_val = []
+                        Y_val = []
+                        for val_idx in te_index:
+                            X_val.append(X_data[val_idx])
+                            Y_val.append(Y_data[val_idx])
+                        for val_idx in te_index:
+                            del X_val[val_idx]
+                            del Y_val[val_idx]
                     train_index, test_index = t_index.copy(), te_index.copy()
                     break
                 fold+= 1
             if len(test_index) > 5:
                 print("Fold number {}. Printing the first 5 ids: {}".format(fold, test_index[:5]))
             else:
                 print("Fold number {}. Indexes used in cross validation: {}".format(fold, test_index))
```

### Comparing `biapy-3.4.2/biapy/data/generators/__init__.py` & `biapy-3.4.3/biapy/data/generators/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,14 +67,15 @@
     # Percentile clipping
     if cfg.DATA.NORMALIZATION.PERC_CLIP:
         norm_dict['lower_bound'] = cfg.DATA.NORMALIZATION.PERC_LOWER
         norm_dict['upper_bound'] = cfg.DATA.NORMALIZATION.PERC_UPPER
         if cfg.DATA.NORMALIZATION.APPLICATION_MODE == "dataset":
             X_train, norm_dict['dataset_X_lower_value'], \
             norm_dict['dataset_X_upper_value'] = percentile_clip(X_train, norm_dict['lower_bound'], norm_dict['upper_bound'])
+            os.makedirs(os.path.dirname(cfg.PATHS.LWR_X_FILE), exist_ok=True)
             np.save(cfg.PATHS.LWR_X_FILE, norm_dict['dataset_X_lower_value'])
             np.save(cfg.PATHS.UPR_X_FILE, norm_dict['dataset_X_upper_value'])
 
         print(f"X_train clipped using the following values: {norm_dict}")
 
     if cfg.DATA.NORMALIZATION.TYPE == 'custom':    
         if cfg.DATA.NORMALIZATION.APPLICATION_MODE == "dataset":
@@ -342,25 +343,29 @@
     norm_dict['mask_norm'] = 'as_mask'
     norm_dict['application_mode'] = cfg.DATA.NORMALIZATION.APPLICATION_MODE
 
     # Percentile clipping
     if cfg.DATA.NORMALIZATION.PERC_CLIP:
         norm_dict['lower_bound'] = cfg.DATA.NORMALIZATION.PERC_LOWER
         norm_dict['upper_bound'] = cfg.DATA.NORMALIZATION.PERC_UPPER
+        norm_dict['clipped'] = X_test is not None
         if cfg.DATA.NORMALIZATION.APPLICATION_MODE == "dataset":
             if not os.path.exists(cfg.PATHS.LWR_X_FILE) or not os.path.exists(cfg.PATHS.UPR_X_FILE):
                     raise FileNotFoundError("Lower/uper percentile files not found in {} and {}"
                         .format(cfg.PATHS.LWR_X_FILE, cfg.PATHS.UPR_X_FILE))
             else:
                 norm_dict['dataset_X_lower_value'] = float(np.load(cfg.PATHS.LWR_X_FILE))
                 norm_dict['dataset_X_upper_value'] = float(np.load(cfg.PATHS.UPR_X_FILE))
 
-            X_test, _, _ = percentile_clip(X_test, lwr_perc_val=norm_dict['dataset_X_lower_value'],
-                uppr_perc_val=norm_dict['dataset_X_upper_value'])
-        print(f"X_test clipped using the following values: {norm_dict}")
+            if X_test is not None:
+                X_test, _, _ = percentile_clip(X_test, lwr_perc_val=norm_dict['dataset_X_lower_value'],
+                    uppr_perc_val=norm_dict['dataset_X_upper_value'])
+                
+        if X_test is not None:        
+            print(f"X_test clipped using the following values: {norm_dict}")
 
     if cfg.DATA.NORMALIZATION.TYPE == 'custom':    
         if cfg.DATA.NORMALIZATION.APPLICATION_MODE == "dataset":
             if cfg.DATA.NORMALIZATION.CUSTOM_MEAN == -1 and cfg.DATA.NORMALIZATION.CUSTOM_STD == -1:
                 print("Test normalization: trying to load mean from {}".format(cfg.PATHS.MEAN_INFO_FILE))
                 print("Test normalization: trying to load std from {}".format(cfg.PATHS.STD_INFO_FILE))
                 if not os.path.exists(cfg.PATHS.MEAN_INFO_FILE) or not os.path.exists(cfg.PATHS.STD_INFO_FILE):
```

### Comparing `biapy-3.4.2/biapy/data/generators/augmentors.py` & `biapy-3.4.3/biapy/data/generators/augmentors.py`

 * *Files 0% similar despite different names*

```diff
@@ -1085,15 +1085,15 @@
     else:
         if img_prob is not None:
             prob = img_prob.ravel()
 
             # Generate the random coordinates based on the distribution
             choices = np.prod(img_prob.shape)
             index = np.random.choice(choices, size=1, p=prob)
-            coordinates = np.unravel_index(index, dims=img_prob.shape)
+            coordinates = np.unravel_index(index, img_prob.shape)
             x = int(coordinates[1][0])
             y = int(coordinates[0][0])
             ox = int(coordinates[1][0])
             oy = int(coordinates[0][0])
 
             # Adjust the coordinates to be the origin of the crop and control to
             # not be out of the image
```

### Comparing `biapy-3.4.2/biapy/data/generators/pair_base_data_generator.py` & `biapy-3.4.3/biapy/data/generators/pair_base_data_generator.py`

 * *Files 0% similar despite different names*

```diff
@@ -980,17 +980,17 @@
         img, mask =  self.load_sample(index)
 
         # Apply random crops if it is selected
         if self.random_crops_in_DA:
             # Capture probability map
             if self.prob_map is not None:
                 if isinstance(self.prob_map, list):
-                    img_prob = np.load(self.prob_map[j])
+                    img_prob = np.load(self.prob_map[index])
                 else:
-                    img_prob = self.prob_map[j]
+                    img_prob = self.prob_map[index]
             else:
                 img_prob = None
             
             # Pad and reflect img/mask if necessary
             img = pad_and_reflect(img, self.shape, verbose=False)
             mask = pad_and_reflect(mask, self.shape, verbose=False)
 
@@ -1335,21 +1335,17 @@
                 pos = i
 
             img, mask = self.load_sample(pos)
             if save_to_dir:
                 orig_images = {}
                 orig_images['o_x'] = np.copy(img) 
                 orig_images['o_y'] = np.copy(mask) 
-                orig_images['o_x2'] = np.copy(img) 
-                orig_images['o_y2'] = np.copy(mask) 
                 if draw_grid:
                     self.draw_grid(orig_images['o_x'])
                     self.draw_grid(orig_images['o_y'])
-                    self.draw_grid(orig_images['o_x2'])
-                    self.draw_grid(orig_images['o_y2'])
 
             # Apply random crops if it is selected
             if self.random_crops_in_DA:
                 # Capture probability map
                 if self.prob_map is not None:
                     if isinstance(self.prob_map, list):
                         img_prob = np.load(self.prob_map[pos])
@@ -1395,45 +1391,45 @@
                 img, mask = self.prepare_n2v(img)
                 sample_y[i] = mask
 
             if save_to_dir:
                 self.save_aug_samples(sample_x[i], sample_y[i], orig_images, i, pos, out_dir, point_dict)
 
 
-    def draw_grid(self, im, grid_width=50):
+    def draw_grid(self, im, grid_width=None):
         """
         Draw grid of the specified size on an image.
 
         Parameters
         ----------
         im : 3D/4D Numpy array
             Image to draw the grid into. E.g. ``(y, x, channels)`` in ``2D`` or ``(z, y, x, channels)`` in ``3D``.
 
         grid_width : int, optional
             Grid's width.
         """
         v = np.max(im)
+        if grid_width is not None:
+            grid_y = grid_width
+            grid_x = grid_width
+        else:
+            grid_y = im.shape[self.ndim-2]//5
+            grid_x = im.shape[self.ndim-2]//5
 
         if self.ndim == 2:
-            for i in range(0, im.shape[0], grid_width):
-                im[i] = v
-            for j in range(0, im.shape[1], grid_width):
-                im[:, j] = v
+            for i in range(0, im.shape[0], grid_y):
+                im[i] = [v]*im.shape[-1]
+            for j in range(0, im.shape[1], grid_x):
+                im[:, j] = [v]*im.shape[-1]
         else:
             for k in range(0, im.shape[0]):
-                for i in range(0, im.shape[2], grid_width):
-                    if im.shape[-1] == 1:
-                        im[k,:,i] = v
-                    else:
-                        im[k,:,i] = [v]*im.shape[-1]
-                for j in range(0, im.shape[1], grid_width):
-                    if im.shape[-1] == 1:
-                        im[k,j] = v
-                    else:
-                        im[k,j] = [v]*im.shape[-1]
+                for i in range(0, im.shape[2], grid_x):
+                    im[k,:,i] = [v]*im.shape[-1]
+                for j in range(0, im.shape[1], grid_y):
+                    im[k,j] = [v]*im.shape[-1]
         return im
         
     def prepare_n2v(self, _img):
         """
         Creates Noise2Void mask.
 
         Parameters
```

### Comparing `biapy-3.4.2/biapy/data/generators/pair_data_2D_generator.py` & `biapy-3.4.3/biapy/data/generators/pair_data_2D_generator.py`

 * *Files 15% similar despite different names*

```diff
@@ -57,15 +57,16 @@
         aux = np.expand_dims(mask, 0).astype(np.float32)
         save_tif(aux, out_dir, [str(i)+"_"+str(pos)+'_y'+self.trans_made+".tif"], verbose=False)
 
         # Save the original images with a point that represents the selected coordinates to be the center of
         # the crop
         if self.random_crops_in_DA and self.prob_map is not None:
             img, mask = self.load_sample(pos)
-
+            if img.max() < 1: img *= 255 
+            if mask.max() == 1: mask *= 255
             img, mask = (img).astype(np.uint8), mask.astype(np.uint8)
 
             if self.shape[-1] == 1:
                 im = Image.fromarray(np.repeat(img, 3, axis=2), 'RGB')
             else:
                 im = Image.fromarray(img, 'RGB')
             px = im.load()
@@ -82,15 +83,15 @@
             for row in range(point_dict['s_x'], point_dict['s_x']+self.shape[0]):
                 px[row, point_dict['s_y']] = (0, 0, 255)
                 px[row, point_dict['s_y']+self.shape[0]-1] = (0, 0, 255)
             for col in range(point_dict['s_y'], point_dict['s_y']+self.shape[0]):
                 px[point_dict['s_x'], col] = (0, 0, 255)
                 px[point_dict['s_x']+self.shape[0]-1, col] = (0, 0, 255)
 
-            im.save(os.path.join(out_dir, str(i)+"_"+str(pos)+'_mark_x'+self.trans_made+'.png'))
+            im.save(os.path.join(out_dir, str(i)+"_"+str(pos)+'_mark_x'+self.trans_made+'.tif'))
 
             if mask.shape[-1] == 1:
                 m = Image.fromarray(np.repeat(mask, 3, axis=2), 'RGB')
             else:
                 m = Image.fromarray(mask, 'RGB')
             px = m.load()
 
@@ -105,8 +106,8 @@
             for row in range(point_dict['s_x'], point_dict['s_x']+self.shape[0]):
                 px[row, point_dict['s_y']] = (0, 0, 255)
                 px[row, point_dict['s_y']+self.shape[0]-1] = (0, 0, 255)
             for col in range(point_dict['s_y'], point_dict['s_y']+self.shape[0]):
                 px[point_dict['s_x'], col] = (0, 0, 255)
                 px[point_dict['s_x']+self.shape[0]-1, col] = (0, 0, 255)
 
-            m.save(os.path.join(out_dir, str(i)+"_"+str(pos)+'_mark_y'+self.trans_made+'.png'))
+            m.save(os.path.join(out_dir, str(i)+"_"+str(pos)+'_mark_y'+self.trans_made+'.tif'))
```

### Comparing `biapy-3.4.2/biapy/data/generators/pair_data_3D_generator.py` & `biapy-3.4.3/biapy/data/generators/pair_data_3D_generator.py`

 * *Files 3% similar despite different names*

```diff
@@ -94,25 +94,27 @@
         save_tif(aux, out_dir, [str(i)+"_orig_y_"+str(pos)+"_"+self.trans_made+'.tif'], verbose=False)
 
         # Save transformed images/masks
         aux = np.expand_dims(img,0).astype(np.float32)
         save_tif(aux, out_dir, [str(i)+"_x_aug_"+str(pos)+"_"+self.trans_made+'.tif'], verbose=False)
         aux = np.expand_dims(mask,0).astype(np.float32)
         save_tif(aux, out_dir, [str(i)+"_y_aug_"+str(pos)+"_"+self.trans_made+'.tif'], verbose=False)
+        del img, mask
 
         # Save the original images with a red point and a blue square that represents the point selected with
         # the probability map and the random volume extracted from the original data
         if self.random_crops_in_DA and self.prob_map is not None and i == 0:
-            os.makedirs(out_dir, exist_ok=True)
-
+            aux, auxm = self.load_sample(pos)
+            if aux.max() < 1: aux *= 255 
+            if auxm.max() == 1: auxm *= 255
+            aux, auxm = (aux).astype(np.uint8), auxm.astype(np.uint8)
+             
             print("The selected point of the random crop was [{},{},{}]".format(point_dict['oz'],point_dict['oy'],point_dict['ox']))
 
-            aux = (orig_images['o_x2']).astype(np.uint8)
             if aux.shape[-1] == 1: aux = np.repeat(aux, 3, axis=3)
-            auxm = (orig_images['o_y2']).astype(np.uint8)
             if auxm.shape[-1] == 1: auxm = np.repeat(auxm, 3, axis=3)
 
             for s in range(aux.shape[0]):
                 if s >= point_dict['s_z'] and s < point_dict['s_z']+self.shape[0]:
                     im = Image.fromarray(aux[s,...,0])
                     im = im.convert('RGB')
                     px = im.load()
@@ -134,21 +136,21 @@
                         py[point_dict['s_x']+self.shape[2]-1, col] = (0, 0, 255)
 
                     # Paint the selected point in red
                     if s == point_dict['oz']:
                         p_size=6
                         for row in range(point_dict['ox']-p_size,point_dict['ox']+p_size):
                             for col in range(point_dict['oy']-p_size,point_dict['oy']+p_size):
-                                if col >= 0 and col < img.shape[1] and row >= 0 and row < img.shape[2]:
+                                if col >= 0 and col < aux.shape[1] and row >= 0 and row < aux.shape[2]:
                                     px[row, col] = (255, 0, 0)
                                     py[row, col] = (255, 0, 0)
 
                     aux[s] = im
                     auxm[s] = m
 
             aux = np.expand_dims(aux,0).astype(np.float32)
-            save_tif(aux, out_dir, ["extract_example_"+str(pos)+"_mark_x_"+self.trans_made+'.tif'], verbose=False)
-
+            save_tif(aux, out_dir, [str(i)+"_"+str(pos)+'_mark_x'+self.trans_made+'.tif'], verbose=False)
+            
             auxm = np.expand_dims(auxm,0).astype(np.float32)
-            save_tif(auxm, out_dir, ["extract_example_"+str(pos)+"_mark_y_"+self.trans_made+'.tif'], verbose=False)
+            save_tif(auxm, out_dir, [str(i)+"_"+str(pos)+'_mark_y'+self.trans_made+'.tif'], verbose=False)
```

### Comparing `biapy-3.4.2/biapy/data/generators/single_base_data_generator.py` & `biapy-3.4.3/biapy/data/generators/single_base_data_generator.py`

 * *Files 2% similar despite different names*

```diff
@@ -467,35 +467,47 @@
         image = self.seq(image=image)
 
         # Recover the original shape
         image = image.reshape(o_img_shape)
 
         return image
 
-    def draw_grid(self, im, grid_width=50):
+    def draw_grid(self, im, grid_width=None):
         """
         Draw grid of the specified size on an image.
 
         Parameters
         ----------
         im : 3D/4D Numpy array
             Image to be modified. E.g. ``(y, x, channels)`` in ``2D`` or ``(z, y, x, channels)`` in ``3D``.
 
         grid_width : int, optional
             Grid's width.
         """
-        v = 1 if int(np.max(im)) == 0 else int(np.max(im))
-
-        for i in range(0, im.shape[0], grid_width):
-            im[i] = v
-        for j in range(0, im.shape[1], grid_width):
-            im[:, j] = v
+        v = np.max(im)
+        if grid_width is not None:
+            grid_y = grid_width
+            grid_x = grid_width
+        else:
+            grid_y = im.shape[self.ndim-2]//5
+            grid_x = im.shape[self.ndim-2]//5
+
+        if self.ndim == 2:
+            for i in range(0, im.shape[0], grid_y):
+                im[i] = [v]*im.shape[-1]
+            for j in range(0, im.shape[1], grid_x):
+                im[:, j] = [v]*im.shape[-1]
+        else:
+            for k in range(0, im.shape[0]):
+                for i in range(0, im.shape[2], grid_x):
+                    im[k,:,i] = [v]*im.shape[-1]
+                for j in range(0, im.shape[1], grid_y):
+                    im[k,j] = [v]*im.shape[-1]
+        return im
         
-        return im 
-
     def get_transformed_samples(self, num_examples, random_images=True, save_to_dir=True, out_dir='aug', train=False,
                                 draw_grid=True):
         """
         Apply selected transformations to a defined number of images from the dataset.
 
         Parameters
         ----------
@@ -530,15 +542,14 @@
         if random_images == False and num_examples > self.length:
             num_examples = self.length
             print("WARNING: More samples requested than the ones available. 'num_examples' fixed to {}".format(num_examples))
 
         sample_x = []
 
         # Generate the examples
-        print("0) Creating the examples of data augmentation . . .")
         for i in tqdm(range(num_examples), disable=not is_main_process()):
             if random_images:
                 pos = random.randint(0,self.length-1) if self.length > 2 else 0
             else:
                 pos = i
 
             img, img_class = self.load_sample(pos)
```

### Comparing `biapy-3.4.2/biapy/data/generators/single_data_2D_generator.py` & `biapy-3.4.3/biapy/data/generators/single_data_2D_generator.py`

 * *Files identical despite different names*

### Comparing `biapy-3.4.2/biapy/data/generators/single_data_3D_generator.py` & `biapy-3.4.3/biapy/data/generators/single_data_3D_generator.py`

 * *Files identical despite different names*

### Comparing `biapy-3.4.2/biapy/data/generators/test_pair_data_generators.py` & `biapy-3.4.3/biapy/data/generators/test_pair_data_generators.py`

 * *Files 2% similar despite different names*

```diff
@@ -212,18 +212,21 @@
         
         xnorm : dict, optional
             Normalization info. 
         """
         xnorm = None
         if self.norm_dict['enable']:
             # Percentile clipping
-            if 'lower_bound' in self.norm_dict and self.norm_dict['application_mode'] == "image":
-                img, _, _ = percentile_clip(img, lower=self.norm_dict['lower_bound'],                                     
-                    upper=self.norm_dict['upper_bound'])
-
+            if 'lower_bound' in self.norm_dict:
+                if self.norm_dict['application_mode'] == "image":
+                    img, _, _ = percentile_clip(img, lower=self.norm_dict['lower_bound'],                                     
+                        upper=self.norm_dict['upper_bound'])
+                elif self.norm_dict['application_mode'] == "dataset" and not self.norm_dict['clipped']:
+                    img, _, _ = percentile_clip(img, lwr_perc_val=self.norm_dict['dataset_X_lower_value'],                                     
+                        uppr_perc_val=self.norm_dict['dataset_X_upper_value'])
             if self.X_norm['type'] == 'div':
                 img, xnorm = norm_range01(img, dtype=self.dtype)
             elif self.X_norm['type'] == 'custom':
                 if self.norm_dict['application_mode'] == "image":
                     xnorm = {}
                     xnorm['mean'] = img.mean()
                     xnorm['std'] = img.std()
@@ -252,18 +255,22 @@
         """
         ynorm = None
         if self.norm_dict['mask_norm'] == 'as_mask':
             if 'div' in self.Y_norm:
                 mask = mask/255
         elif self.norm_dict['mask_norm'] == 'as_image':
             # Percentile clipping
-            if 'lower_bound' in self.norm_dict and self.norm_dict['application_mode'] == "image":
-                mask, _, _ = percentile_clip(mask, lower=self.norm_dict['lower_bound'],                                     
-                    upper=self.norm_dict['upper_bound'])
-
+            if 'lower_bound' in self.norm_dict:
+                if self.norm_dict['application_mode'] == "image":
+                    mask, _, _ = percentile_clip(mask, lower=self.norm_dict['lower_bound'],                                     
+                        upper=self.norm_dict['upper_bound'])
+                elif self.norm_dict['application_mode'] == "dataset" and not self.norm_dict['clipped']:
+                    mask, _, _ = percentile_clip(mask, lower=self.norm_dict['dataset_X_lower_value'],                                     
+                        upper=self.norm_dict['dataset_X_upper_value'])
+                        
             if self.X_norm['type'] == 'div':
                 mask, ynorm = norm_range01(mask, dtype=self.dtype)
             elif self.X_norm['type'] == 'custom':
                 if self.norm_dict['application_mode'] == "image":
                     ynorm = {}
                     ynorm['mean'] = mask.mean()
                     ynorm['std'] = mask.std()
```

### Comparing `biapy-3.4.2/biapy/data/generators/test_single_data_generator.py` & `biapy-3.4.3/biapy/data/generators/test_single_data_generator.py`

 * *Files 9% similar despite different names*

```diff
@@ -55,15 +55,15 @@
 
     reduce_mem : bool, optional
         To reduce the dtype from float32 to float16. 
 
     crop_center : bool, optional
         Whether to extract a
 
-    sample_ids :  List of ints, optional
+    sample_ids : List of ints, optional
         When cross validation is used specific training samples are passed to the generator. 
         Not used in this generator. 
 
     convert_to_rgb : bool, optional
         In case RGB images are expected, e.g. if ``crop_shape`` channel is 3, those images that are grayscale are 
         converted into RGB.
     
@@ -108,14 +108,23 @@
                 for folder in self.class_names:
                     print("Analizing folder {}".format(os.path.join(d_path,folder)))
                     ids = sorted(next(os.walk(os.path.join(d_path,folder)))[2])
                     print("Found {} samples".format(len(ids)))
                     for i in range(len(ids)):
                         self.classes[ids[i]] = folder
                         self.data_path.append(ids[i])
+                
+                if sample_ids is not None:
+                    self.data_path = [x for i, x in enumerate(self.data_path) if i in sample_ids]
+                    old_classes = self.classes.copy()
+                    for i, key in enumerate(old_classes.keys()):
+                        if i not in sample_ids:
+                            del self.classes[key]
+                    del old_classes
+                    
                 self.len = len(self.data_path)
                 if self.len == 0:
                     raise ValueError("No image found in {}".format(d_path))
             else:
                 self.len = len(X)
         else:
             self.data_path = sorted(next(os.walk(d_path))[2])
@@ -188,17 +197,21 @@
             else:
                 if img.shape[0] <= 3: img = img.transpose((1,2,0))
 
         # Normalization
         xnorm = None
         if self.norm_dict['enable']:
             # Percentile clipping
-            if 'lower_bound' in self.norm_dict and self.norm_dict['application_mode'] == "image":
-                img, _, _ = percentile_clip(img, lower=self.norm_dict['lower_bound'],                                     
-                    upper=self.norm_dict['upper_bound'])
+            if 'lower_bound' in self.norm_dict:
+                if self.norm_dict['application_mode'] == "image":
+                    img, _, _ = percentile_clip(img, lower=self.norm_dict['lower_bound'],                                     
+                        upper=self.norm_dict['upper_bound'])
+                elif self.norm_dict['application_mode'] == "dataset" and not self.norm_dict['clipped']:
+                    img, _, _ = percentile_clip(img, lwr_perc_val=self.norm_dict['dataset_X_lower_value'],                                     
+                        uppr_perc_val=self.norm_dict['dataset_X_upper_value'])
 
             if self.X_norm['type'] == 'div':
                 img, xnorm = norm_range01(img, dtype=self.dtype)
             elif self.X_norm['type'] == 'custom':
                 if self.norm_dict['application_mode'] == "image":
                     xnorm = {}
                     xnorm['mean'] = img.mean()
```

### Comparing `biapy-3.4.2/biapy/data/post_processing/__init__.py` & `biapy-3.4.3/biapy/data/post_processing/__init__.py`

 * *Files identical despite different names*

### Comparing `biapy-3.4.2/biapy/data/post_processing/post_processing.py` & `biapy-3.4.3/biapy/data/post_processing/post_processing.py`

 * *Files 0% similar despite different names*

```diff
@@ -1473,16 +1473,17 @@
     unsure_str = "Removed"
 
     comment = []
     label_list = []
     label_list, npixels = np.unique(img, return_counts=True)
     
     # Delete background instance '0'
-    label_list = label_list[1:] 
-    npixels = npixels[1:]
+    if label_list[0] == 0:
+        label_list = label_list[1:] 
+        npixels = npixels[1:]
 
     total_labels = len(label_list)
     comment = ['none' for i in range(total_labels)]
 
     # Measure array definitions
     areas = np.zeros(total_labels, dtype=np.uint32)
     diameters = np.zeros(total_labels, dtype=np.uint32)
@@ -1543,15 +1544,15 @@
     for i in tqdm(range(len(circularities)), leave=False):
         conditions.append([])
         if filter_instances:
             for k, list_of_conditions in enumerate(properties):
                 # Check each list of conditions
                 comps = []
                 for j, prop in enumerate(list_of_conditions):
-                    if prop == "circularity":
+                    if prop in ["circularity", "sphericity"]:
                         value_to_compare = circularities[i]
                     elif prop == "npixels":
                         value_to_compare = npixels[i]
                     elif prop == "area":
                         value_to_compare = areas[i]
                     elif prop == "diameter":
                         value_to_compare = diameters[i]
@@ -1590,21 +1591,21 @@
         # If satisfied all conditions remove the instance 
         if any(conditions[-1]):
             comment[i] = unsure_str
             img[img==label_list[i]] = 0
             labels_removed += 1
         else:
             comment[i] = correct_str
-
+    cir_name = 'sphericities' if image3d else 'circularities'
     d_result = {
         'labels': label_list,
         'centers': centers,
         'npixels': npixels,
         'areas': areas,
-        'circularities': circularities,
+        cir_name: circularities,
         'diameters': diameters,
         'perimeters': perimeters,
         'comment': comment,
         'conditions': conditions,
     }
 
     if not image3d:
```

### Comparing `biapy-3.4.2/biapy/data/post_processing/smooth_tiled_predictions.py` & `biapy-3.4.3/biapy/data/post_processing/smooth_tiled_predictions.py`

 * *Files identical despite different names*

### Comparing `biapy-3.4.2/biapy/data/pre_processing.py` & `biapy-3.4.3/biapy/data/pre_processing.py`

 * *Files 1% similar despite different names*

```diff
@@ -354,15 +354,15 @@
                     if img.ndim == 3: 
                         img = np.expand_dims(img, -1)
                     else:
                         if img.shape[0] <= 3: img = img.transpose((1,2,3,0))
                 shape = img.shape[:-1]
             else:
                 img_zarr_file, img = read_chunked_data(os.path.join(img_dir, img_filename))
-                shape = img.shape
+                shape = img.shape if img.ndim == 3 else img.shape[:-1]
 
                 if isinstance(img_zarr_file, h5py.File):
                     img_zarr_file.close()
                 del img_zarr_file
                 
             del img 
             
@@ -466,15 +466,16 @@
 
             # Dilate the mask
             if cfg.PROBLEM.DETECTION.CENTRAL_POINT_DILATION > 0:
                 print("Dilating all points . . .")
                 if cfg.PROBLEM.NDIM == '2D': mask = np.expand_dims(mask,0)
                 for k in tqdm(range(mask.shape[0]), total=len(mask), leave=False, disable=not is_main_process()): 
                     for ch in range(mask.shape[-1]):                                                                                  
-                        mask[k,...,ch] = binary_dilation_scipy(mask[k,...,ch], iterations=1,  structure=disk(cfg.PROBLEM.DETECTION.CENTRAL_POINT_DILATION))                                                                                                                                                    
+                        mask[k,...,ch] = binary_dilation_scipy(mask[k,...,ch], iterations=1,  
+                            structure=disk(cfg.PROBLEM.DETECTION.CENTRAL_POINT_DILATION))                                                                                                                                                    
                 if cfg.PROBLEM.NDIM == '2D': mask = mask[0]
 
             if cfg.PROBLEM.DETECTION.CHECK_POINTS_CREATED:
                 print("Check points created to see if some of them are very close that create a large label") 
                 error_found = False
                 for ch in tqdm(range(mask.shape[-1]), total=len(mask), leave=False, disable=not is_main_process()):
                     _, index, counts = np.unique(label(clear_border(mask[...,ch])), return_counts=True, return_index=True)
```

### Comparing `biapy-3.4.2/biapy/engine/__init__.py` & `biapy-3.4.3/biapy/engine/__init__.py`

 * *Files identical despite different names*

### Comparing `biapy-3.4.2/biapy/engine/base_workflow.py` & `biapy-3.4.3/biapy/engine/base_workflow.py`

 * *Files 1% similar despite different names*

```diff
@@ -655,19 +655,19 @@
                 for i in range(len(self.metric_names)):
                     self.plot_values[self.metric_names[i]].append(train_stats[self.metric_names[i]])
                     if self.val_generator is not None:
                         self.plot_values['val_'+self.metric_names[i]].append(test_stats[self.metric_names[i]])
                 if (epoch+1) % self.cfg.LOG.CHART_CREATION_FREQ == 0:
                     create_plots(self.plot_values, self.metric_names, self.job_identifier, self.cfg.PATHS.CHARTS)
 
-                if self.val_generator is not None and self.early_stopping is not None:
-                    self.early_stopping(test_stats['loss'])
-                    if self.early_stopping.early_stop:
-                        print("Early stopping")
-                        break
+            if self.val_generator is not None and self.early_stopping is not None:
+                self.early_stopping(test_stats['loss'])
+                if self.early_stopping.early_stop:
+                    print("Early stopping")
+                    break
                         
             e_end = time.time()
             t_epoch = e_end - e_start
             print("[Time] {} {}/{}\n".format(time_text(t_epoch), time_text(e_end - start_time),
                                              time_text((e_end - start_time)+(t_epoch*(self.cfg.TRAIN.EPOCHS-epoch)))))
             
         total_time = time.time() - start_time
@@ -861,19 +861,19 @@
             if 'Y' in gen_obj: self._Y = gen_obj['Y']
             if 'Y_norm' in gen_obj: Y_norm = gen_obj['Y_norm']
             self.processing_filenames = self.test_filenames[gen_obj['file']] if isinstance(gen_obj['file'], int) else gen_obj['file']
             self.processing_filenames = [os.path.basename(self.processing_filenames)]
             self.f_numbers = [i]
             del gen_obj
 
-            if is_main_process():
-                if self.cfg.TEST.BY_CHUNKS.ENABLE and self.cfg.PROBLEM.NDIM == '3D':
-                    print(f"[Rank {get_rank()} ({os.getpid()})] Processing image(s): {self.processing_filenames[0]}")
-                    self.process_sample_by_chunks(self.processing_filenames[0])
-                else:
+            if self.cfg.TEST.BY_CHUNKS.ENABLE and self.cfg.PROBLEM.NDIM == '3D':
+                print(f"[Rank {get_rank()} ({os.getpid()})] Processing image(s): {self.processing_filenames[0]}")
+                self.process_sample_by_chunks(self.processing_filenames[0])
+            else:
+                if is_main_process():
                     print("Processing image: {}".format(self.processing_filenames[0]))
                     self.process_sample(norm=(X_norm, Y_norm))                        
             
             image_counter += 1
 
         self.destroy_test_data()
 
@@ -1410,15 +1410,14 @@
                     with torch.cuda.amp.autocast():
                         pred = self.model_call_func(self._X)
                 pred = self.apply_model_activations(pred)
                 # Multi-head concatenation
                 if isinstance(pred, list):
                     pred = torch.cat((pred[0], torch.argmax(pred[1], axis=1).unsqueeze(1)), dim=1)  
                 pred = to_numpy_format(pred, self.axis_order_back)  
-                if self.cfg.TEST.AUGMENTATION: pred = np.expand_dims(pred, 0)
                 del self._X 
 
                 # Recover original shape if padded with check_downsample_division
                 pred = pred[:,:o_test_shape[1],:o_test_shape[2]]
                 if self.cfg.DATA.TEST.LOAD_GT: self._Y = self._Y[:,:o_test_shape[1],:o_test_shape[2]]
 
                 # Save image
@@ -1473,17 +1472,14 @@
         self.stats['iou'] = self.stats['iou'] / image_counter
         self.stats['loss'] = self.stats['loss'] / image_counter
         self.stats['ov_iou'] = self.stats['ov_iou'] / image_counter
 
         if self.post_processing['per_image']:
             self.stats['iou_merge_patches_post'] = self.stats['iou_merge_patches_post'] / image_counter
             self.stats['ov_iou_merge_patches_post'] = self.stats['ov_iou_merge_patches_post'] / image_counter
-        if self.post_processing['as_3D_stack']:
-            self.stats['iou_as_3D_stack_post'] = self.stats['iou_as_3D_stack_post'] / image_counter
-            self.stats['ov_iou_as_3D_stack_post'] = self.stats['ov_iou_as_3D_stack_post'] / image_counter
             
     def print_stats(self, image_counter):
         """
         Print statistics.  
 
         Parameters
         ----------
@@ -1597,14 +1593,16 @@
         """
         ############################
         ### POST-PROCESSING (2D) ###
         ############################
         if self.post_processing['as_3D_stack']:
             self.all_pred = np.concatenate(self.all_pred)
             self.all_gt = np.concatenate(self.all_gt) if self.cfg.DATA.TEST.LOAD_GT else None
+            save_tif(np.expand_dims(self.all_pred,0), self.cfg.PATHS.RESULT_DIR.AS_3D_STACK, verbose=self.cfg.TEST.VERBOSE)
+            save_tif(np.expand_dims((self.all_pred>0.5).astype(np.uint8),0), self.cfg.PATHS.RESULT_DIR.AS_3D_STACK_BIN, verbose=self.cfg.TEST.VERBOSE)
             self.all_pred, self.stats['iou_as_3D_stack_post'], self.stats['ov_iou_as_3D_stack_post'] = apply_post_processing(self.cfg, self.all_pred, self.all_gt)
             save_tif(np.expand_dims(self.all_pred,0), self.cfg.PATHS.RESULT_DIR.AS_3D_STACK_POST_PROCESSING, verbose=self.cfg.TEST.VERBOSE)
 
 def extract_patch_from_dataset(data, cfg, input_queue, extract_info_queue, verbose=False):
     """
     Extract patches from data and put them into a queue read by each GPU inference process.
     This function will be run by a child process created for every test sample.  
@@ -1725,20 +1723,21 @@
     # Obtain the total patches so we can display it for the user
     total_patches = extract_info_queue.get(timeout=60)
     for i in tqdm(range(total_patches), disable=not is_main_process()):
         p, m, patch_coords = output_queue.get(timeout=60)
 
         if 'data' not in locals():
             # Channel dimension should be equal to the number of channel of the prediction
-            out_data_shape = tuple(data_shape)
+            out_data_shape = np.array(data_shape)
             if "C" not in cfg.TEST.BY_CHUNKS.INPUT_IMG_AXES_ORDER:
                 out_data_shape = tuple(out_data_shape) + (p.shape[-1],)
                 out_data_order = cfg.TEST.BY_CHUNKS.INPUT_IMG_AXES_ORDER + "C"
             else:
-                out_data_shape = tuple(out_data_shape[:-1]) + (p.shape[-1],)
+                out_data_shape[cfg.TEST.BY_CHUNKS.INPUT_IMG_AXES_ORDER.index("C")] = 1
+                out_data_shape = tuple(out_data_shape)
                 out_data_order = cfg.TEST.BY_CHUNKS.INPUT_IMG_AXES_ORDER
 
             if file_type == "h5":
                 data = fid.create_dataset("data", out_data_shape, dtype=dtype_str, compression="gzip")
                 mask = fid_mask.create_dataset("data", out_data_shape, dtype=dtype_str, compression="gzip")
             else:
                 data = fid.create_dataset("data", shape=out_data_shape, dtype=dtype_str)
```

### Comparing `biapy-3.4.2/biapy/engine/check_configuration.py` & `biapy-3.4.3/biapy/engine/check_configuration.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,14 +50,19 @@
     if len(cfg.DATA.TRAIN.RESOLUTION) == 1 and cfg.DATA.TRAIN.RESOLUTION[0] == -1:
         opts.extend(['DATA.TRAIN.RESOLUTION', (1,)*dim_count])
     if len(cfg.DATA.VAL.RESOLUTION) == 1 and cfg.DATA.VAL.RESOLUTION[0] == -1:
         opts.extend(['DATA.VAL.RESOLUTION', (1,)*dim_count])
     if len(cfg.DATA.TEST.RESOLUTION) == 1 and cfg.DATA.TEST.RESOLUTION[0] == -1:
         opts.extend(['DATA.TEST.RESOLUTION', (1,)*dim_count])
 
+    if cfg.TEST.POST_PROCESSING.REPARE_LARGE_BLOBS_SIZE != -1:
+        if cfg.PROBLEM.TYPE != 'INSTANCE_SEG':
+            raise ValueError("'TEST.POST_PROCESSING.REPARE_LARGE_BLOBS_SIZE' can only be set when 'PROBLEM.TYPE' is 'INSTANCE_SEG'")
+        if cfg.PROBLEM.INSTANCE_SEG.DATA_CHANNELS != 'BP':
+            raise ValueError("'TEST.POST_PROCESSING.REPARE_LARGE_BLOBS_SIZE' only makes sense when 'PROBLEM.INSTANCE_SEG.DATA_CHANNELS == 'BP'")
     if cfg.TEST.POST_PROCESSING.DET_WATERSHED and cfg.PROBLEM.TYPE != 'DETECTION':
         raise ValueError("'TEST.POST_PROCESSING.DET_WATERSHED' can only be set when 'PROBLEM.TYPE' is 'DETECTION'")
     if cfg.TEST.POST_PROCESSING.DET_WATERSHED:
         for x in cfg.TEST.POST_PROCESSING.DET_WATERSHED_FIRST_DILATION:
             if not isinstance(x, list):
                 raise ValueError("'TEST.POST_PROCESSING.DET_WATERSHED_FIRST_DILATION' needs to be a list of list") 
             if any(y == -1 for y in x):
@@ -77,23 +82,14 @@
 
     if not (len(cfg.TEST.POST_PROCESSING.MEASURE_PROPERTIES.REMOVE_BY_PROPERTIES.PROPS) == \
         len(cfg.TEST.POST_PROCESSING.MEASURE_PROPERTIES.REMOVE_BY_PROPERTIES.VALUES) == \
         len(cfg.TEST.POST_PROCESSING.MEASURE_PROPERTIES.REMOVE_BY_PROPERTIES.SIGN)):
         raise ValueError("'TEST.POST_PROCESSING.MEASURE_PROPERTIES.REMOVE_BY_PROPERTIES.PROPS', 'TEST.POST_PROCESSING.MEASURE_PROPERTIES.REMOVE_BY_PROPERTIES.VALUES' and "
             "'TEST.POST_PROCESSING.MEASURE_PROPERTIES.REMOVE_BY_PROPERTIES.SIGN' need to have same length")
             
-    if cfg.PROBLEM.TYPE == 'DETECTION':
-        if cfg.TEST.POST_PROCESSING.MEASURE_PROPERTIES.ENABLE and \
-            cfg.TEST.POST_PROCESSING.MEASURE_PROPERTIES.REMOVE_BY_PROPERTIES.ENABLE:
-            for i in range(len(cfg.TEST.POST_PROCESSING.MEASURE_PROPERTIES.REMOVE_BY_PROPERTIES.PROPS)):
-                if len(cfg.TEST.POST_PROCESSING.MEASURE_PROPERTIES.REMOVE_BY_PROPERTIES.PROPS[i]) > 1:
-                    raise ValueError("In DETECTION 'TEST.POST_PROCESSING.MEASURE_PROPERTIES.REMOVE_BY_PROPERTIES.PROPS' can only be used for filtering 'circularity'.")
-                if len(cfg.TEST.POST_PROCESSING.MEASURE_PROPERTIES.REMOVE_BY_PROPERTIES.PROPS[i]) == 1 and cfg.TEST.POST_PROCESSING.MEASURE_PROPERTIES.REMOVE_BY_PROPERTIES.PROPS[i][0] != 'circularity':  
-                    raise ValueError("In DETECTION 'TEST.POST_PROCESSING.MEASURE_PROPERTIES.REMOVE_BY_PROPERTIES.PROPS' can only be used for filtering 'circularity'.")
-    
     if cfg.TEST.POST_PROCESSING.MEASURE_PROPERTIES.ENABLE and \
         cfg.TEST.POST_PROCESSING.MEASURE_PROPERTIES.REMOVE_BY_PROPERTIES.ENABLE:
         if cfg.PROBLEM.TYPE not in ['INSTANCE_SEG', 'DETECTION']:
             raise ValueError("'TEST.POST_PROCESSING.MEASURE_PROPERTIES.REMOVE_BY_PROPERTIES.PROPS' can only be used in INSTANCE_SEG and DETECTION workflows")
 
         if len(cfg.TEST.POST_PROCESSING.MEASURE_PROPERTIES.REMOVE_BY_PROPERTIES.PROPS) == 0:
             raise ValueError("'TEST.POST_PROCESSING.MEASURE_PROPERTIES.REMOVE_BY_PROPERTIES.PROPS' can not be an empty list when "
@@ -116,25 +112,30 @@
             # Check for unique values 
             if len([item for item, count in collections.Counter(cfg.TEST.POST_PROCESSING.MEASURE_PROPERTIES.REMOVE_BY_PROPERTIES.PROPS[i]).items() if count > 1]) > 0:
                 raise ValueError("Non repeated values are allowed in 'TEST.POST_PROCESSING.MEASURE_PROPERTIES.REMOVE_BY_PROPERTIES'")
             for j in range(len(cfg.TEST.POST_PROCESSING.MEASURE_PROPERTIES.REMOVE_BY_PROPERTIES.PROPS[i])):
                 if cfg.TEST.POST_PROCESSING.MEASURE_PROPERTIES.REMOVE_BY_PROPERTIES.PROPS[i][j] not in ['circularity', 'npixels', 'area', 'diameter', 'elongation', 'sphericity', 'perimeter']:
                     raise ValueError("'TEST.POST_PROCESSING.MEASURE_PROPERTIES.REMOVE_BY_PROPERTIES.PROPS' can only be one among these: ['circularity', 'npixels', 'area', 'diameter', 'elongation', 'sphericity', 'perimeter']")
                 if cfg.TEST.POST_PROCESSING.MEASURE_PROPERTIES.REMOVE_BY_PROPERTIES.PROPS[i][j] in ["circularity", "elongation"] and cfg.PROBLEM.NDIM != '2D':
-                    raise ValueError("'circularity' or 'elongation' properties can only be measured in 2D images. Delete them from 'TEST.POST_PROCESSING.MEASURE_PROPERTIES.REMOVE_BY_PROPERTIES.PROPS'")
+                    raise ValueError("'circularity' or 'elongation' properties can only be measured in 2D images. Delete them from 'TEST.POST_PROCESSING.MEASURE_PROPERTIES.REMOVE_BY_PROPERTIES.PROPS'. "
+                        "'circularity'-kind property in 3D is 'sphericity'")
                 if cfg.TEST.POST_PROCESSING.MEASURE_PROPERTIES.REMOVE_BY_PROPERTIES.PROPS[i][j] == "sphericity" and cfg.PROBLEM.NDIM != '3D':
-                    raise ValueError("'sphericity' property can only be measured in 3D images. Delete it from 'TEST.POST_PROCESSING.MEASURE_PROPERTIES.REMOVE_BY_PROPERTIES.PROPS'")
+                    raise ValueError("'sphericity' property can only be measured in 3D images. Delete it from 'TEST.POST_PROCESSING.MEASURE_PROPERTIES.REMOVE_BY_PROPERTIES.PROPS'. "
+                        "'sphericity'-kind property in 2D is 'circularity'")
                 if cfg.TEST.POST_PROCESSING.MEASURE_PROPERTIES.REMOVE_BY_PROPERTIES.SIGN[i][j] not in ['gt', 'ge', 'lt', 'le']:
                     raise ValueError("'TEST.POST_PROCESSING.MEASURE_PROPERTIES.REMOVE_BY_PROPERTIES.SIGN' can only be one among these: ['gt', 'ge', 'lt', 'le']")
                 if cfg.TEST.POST_PROCESSING.MEASURE_PROPERTIES.REMOVE_BY_PROPERTIES.PROPS[i][j] == "circularity" and not check_value(cfg.TEST.POST_PROCESSING.MEASURE_PROPERTIES.REMOVE_BY_PROPERTIES.VALUES[i][j]):
                     raise ValueError("Circularity can only have values in [0, 1] range (check  'TEST.POST_PROCESSING.MEASURE_PROPERTIES.REMOVE_BY_PROPERTIES.VALUES' values)")
                     
     if cfg.PROBLEM.TYPE != 'INSTANCE_SEG':  
         if cfg.TEST.POST_PROCESSING.VORONOI_ON_MASK:
             raise ValueError("'TEST.POST_PROCESSING.VORONOI_ON_MASK' can only be enabled in a 'INSTANCE_SEG' problem")
+        if cfg.TEST.POST_PROCESSING.CLEAR_BORDER:
+            raise ValueError("'TEST.POST_PROCESSING.CLEAR_BORDER' can only be enabled in a 'INSTANCE_SEG' problem")
+
     if cfg.TEST.POST_PROCESSING.DET_WATERSHED and cfg.PROBLEM.TYPE != 'DETECTION':
         raise ValueError("'TEST.POST_PROCESSING.DET_WATERSHED' can only be set when 'PROBLEM.TYPE' is 'DETECTION'")
 
     if cfg.PROBLEM.NDIM == "2D":
         if (cfg.TEST.POST_PROCESSING.YZ_FILTERING or cfg.TEST.POST_PROCESSING.Z_FILTERING) \
             and not cfg.TEST.ANALIZE_2D_IMGS_AS_3D_STACK:
             raise ValueError("'TEST.POST_PROCESSING.YZ_FILTERING' and 'TEST.POST_PROCESSING.Z_FILTERING' is done only if"
@@ -275,20 +276,21 @@
             if any(len(x) != dim_count for x in cfg.TEST.POST_PROCESSING.DET_WATERSHED_FIRST_DILATION):
                 raise ValueError("Each structure object defined in 'TEST.POST_PROCESSING.DET_WATERSHED_FIRST_DILATION' "
                                  "needs to be of {} dimension".format(dim_count))
             if not cfg.TEST.POST_PROCESSING.MEASURE_PROPERTIES.ENABLE or \
                 not cfg.TEST.POST_PROCESSING.MEASURE_PROPERTIES.REMOVE_BY_PROPERTIES.ENABLE:
                 raise ValueError("'TEST.POST_PROCESSING.MEASURE_PROPERTIES.ENABLE' and "
                     "'TEST.POST_PROCESSING.MEASURE_PROPERTIES.REMOVE_BY_PROPERTIES.ENABLE' needs to be set when 'TEST.POST_PROCESSING.DET_WATERSHED' is enabled")
-            if len(cfg.TEST.POST_PROCESSING.MEASURE_PROPERTIES.REMOVE_BY_PROPERTIES.PROPS[0]) != 0: 
-                raise ValueError("'TEST.POST_PROCESSING.MEASURE_PROPERTIES.REMOVE_BY_PROPERTIES.PROPS' needs to be set to 'circularity' or 'sphericity' filtering "
-                    "when 'TEST.POST_PROCESSING.DET_WATERSHED' is enabled")
-            if cfg.TEST.POST_PROCESSING.MEASURE_PROPERTIES.REMOVE_BY_PROPERTIES.PROPS[0][0] not in ['circularity', 'sphericity']: 
-                raise ValueError("'TEST.POST_PROCESSING.MEASURE_PROPERTIES.REMOVE_BY_PROPERTIES.PROPS' needs to be set to 'circularity' or 'sphericity' filtering "
-                    "when 'TEST.POST_PROCESSING.DET_WATERSHED' is enabled")
+            for lprop in cfg.TEST.POST_PROCESSING.MEASURE_PROPERTIES.REMOVE_BY_PROPERTIES.PROPS:
+                if len(lprop) != 1:
+                    raise ValueError("'TEST.POST_PROCESSING.MEASURE_PROPERTIES.REMOVE_BY_PROPERTIES.PROPS' can not be set with more than one property and that property"
+                        " needs to be set to 'circularity' or 'sphericity'. This restriction is because 'TEST.POST_PROCESSING.DET_WATERSHED' is enabled")
+                if lprop[0] not in ['circularity', 'sphericity']: 
+                    raise ValueError("Only 'circularity' or 'sphericity' can be used in 'TEST.POST_PROCESSING.MEASURE_PROPERTIES.REMOVE_BY_PROPERTIES.PROPS' "
+                        "when 'TEST.POST_PROCESSING.DET_WATERSHED' is enabled")
         if cfg.TEST.DET_POINT_CREATION_FUNCTION not in ['peak_local_max', 'blob_log']:
             raise ValueError("'TEST.DET_POINT_CREATION_FUNCTION' must be one between: ['peak_local_max', 'blob_log']")
         if cfg.MODEL.SOURCE == "torchvision":
             if cfg.MODEL.TORCHVISION_MODEL_NAME not in ['fasterrcnn_mobilenet_v3_large_320_fpn', 'fasterrcnn_mobilenet_v3_large_fpn', \
                 'fasterrcnn_resnet50_fpn', 'fasterrcnn_resnet50_fpn_v2', 'fcos_resnet50_fpn', 'ssd300_vgg16', 'ssdlite320_mobilenet_v3_large', \
                 'retinanet_resnet50_fpn', 'retinanet_resnet50_fpn_v2']:
                 raise ValueError("'MODEL.SOURCE' must be one between ['fasterrcnn_mobilenet_v3_large_320_fpn', 'fasterrcnn_mobilenet_v3_large_fpn', "
@@ -317,14 +319,16 @@
     #### Self-supervision ####
     elif cfg.PROBLEM.TYPE == 'SELF_SUPERVISED':
         if cfg.PROBLEM.SELF_SUPERVISED.PRETEXT_TASK == "crappify":
             if cfg.PROBLEM.SELF_SUPERVISED.RESIZING_FACTOR not in [2,4,6]:
                 raise ValueError("'PROBLEM.SELF_SUPERVISED.RESIZING_FACTOR' not in [2,4,6]")
             if not check_value(cfg.PROBLEM.SELF_SUPERVISED.NOISE):
                 raise ValueError("'PROBLEM.SELF_SUPERVISED.NOISE' not in [0, 1] range")
+            if model_arch == 'mae':
+                raise ValueError("'MODEL.ARCHITECTURE' can not be 'mae' when 'PROBLEM.SELF_SUPERVISED.PRETEXT_TASK' is 'crappify'")
         elif cfg.PROBLEM.SELF_SUPERVISED.PRETEXT_TASK == "masking":
             if model_arch != 'mae':
                 raise ValueError("'MODEL.ARCHITECTURE' needs to be 'mae' when 'PROBLEM.SELF_SUPERVISED.PRETEXT_TASK' is 'masking'")  
             assert cfg.MODEL.MAE_MASK_TYPE in ["random", "grid"], "'MODEL.MAE_MASK_TYPE' needs to be one between ['random', 'grid']"
             if cfg.MODEL.MAE_MASK_TYPE == "random" and not check_value(cfg.MODEL.MAE_MASK_RATIO):
                 raise ValueError("'MODEL.MAE_MASK_RATIO' not in [0, 1] range")
         else:
@@ -389,15 +393,17 @@
         if cfg.PROBLEM.IMAGE_TO_IMAGE.MULTIPLE_RAW_ONE_TARGET_LOADER:
             if cfg.DATA.TRAIN.IN_MEMORY:
                 raise ValueError("'PROBLEM.IMAGE_TO_IMAGE.MULTIPLE_RAW_ONE_TARGET_LOADER' can only be used if 'DATA.TRAIN.IN_MEMORY' == 'False'")
             if cfg.DATA.VAL.IN_MEMORY:
                 raise ValueError("'PROBLEM.IMAGE_TO_IMAGE.MULTIPLE_RAW_ONE_TARGET_LOADER' can only be used if 'DATA.VAL.IN_MEMORY' == 'False'")
             if cfg.DATA.TEST.IN_MEMORY:
                 raise ValueError("'PROBLEM.IMAGE_TO_IMAGE.MULTIPLE_RAW_ONE_TARGET_LOADER' can only be used if 'DATA.TEST.IN_MEMORY' == 'False'")
-
+        if cfg.PROBLEM.NDIM == '3D':
+            raise ValueError("3D workflow not available for 'IMAGE_TO_IMAGE' yet")
+            
     if cfg.DATA.EXTRACT_RANDOM_PATCH and cfg.DATA.PROBABILITY_MAP:
         if cfg.DATA.W_FOREGROUND+cfg.DATA.W_BACKGROUND != 1:
             raise ValueError("cfg.DATA.W_FOREGROUND+cfg.DATA.W_BACKGROUND need to sum 1. E.g. 0.94 and 0.06 respectively.")
     if not cfg.DATA.TRAIN.IN_MEMORY and cfg.DATA.PREPROCESS.TRAIN:
         raise ValueError('To use preprocessing DATA.TRAIN.IN_MEMORY needs to be True.')
     if not cfg.DATA.VAL.IN_MEMORY and cfg.DATA.PREPROCESS.VAL:
         if cfg.DATA.VAL.FROM_TRAIN:
@@ -615,37 +621,34 @@
     if cfg.MODEL.SOURCE == "biapy":
         assert cfg.MODEL.LAST_ACTIVATION.lower() in ["relu", "tanh", "leaky_relu", "elu", "gelu", "silu", "sigmoid","softmax", "linear", "none"], \
             "Get unknown activation key {}".format(activation)
     
         if cfg.MODEL.UPSAMPLE_LAYER.lower() not in ["upsampling", "convtranspose"]:
             raise ValueError("cfg.MODEL.UPSAMPLE_LAYER' needs to be one between ['upsampling', 'convtranspose']. Provided {}"
                             .format(cfg.MODEL.UPSAMPLE_LAYER))
-        if cfg.PROBLEM.TYPE == "SEMANTIC_SEG" and model_arch not in ['unet', 'resunet', 'resunet++', 'attention_unet', \
-            'multiresunet', 'seunet', 'unetr']:
-            raise ValueError("Not implemented pipeline option: semantic segmentation models are ['unet', 'resunet', 'resunet++', "
-                            "'attention_unet', 'multiresunet', 'seunet', 'unetr']")
-        if cfg.PROBLEM.TYPE == "INSTANCE_SEG" and model_arch not in ['unet', 'resunet', 'resunet++', 'seunet', 'attention_unet', 'unetr', 'multiresunet']:
-            raise ValueError("Not implemented pipeline option: instance segmentation models are ['unet', 'resunet', 'resunet++', 'seunet', 'attention_unet', 'unetr', 'multiresunet']")    
-        if cfg.PROBLEM.TYPE in ['DETECTION', 'DENOISING'] and \
-            model_arch not in ['unet', 'resunet', 'resunet++', 'seunet', 'attention_unet']:
-            raise ValueError("Architectures available for {} are: ['unet', 'resunet', 'resunet++', 'seunet', 'attention_unet']"
-                            .format(cfg.PROBLEM.TYPE))
-        if cfg.PROBLEM.TYPE == 'SUPER_RESOLUTION':
+        if cfg.PROBLEM.TYPE in ["SEMANTIC_SEG", "INSTANCE_SEG", "DETECTION", "DENOISING"]:
+            if model_arch not in ['unet', 'resunet', 'resunet++', 'seunet', 'attention_unet', 'unetr', 'multiresunet']:
+                raise ValueError("Architectures available for {} are: ['unet', 'resunet', 'resunet++', 'seunet', 'attention_unet', 'unetr', 'multiresunet']"
+                                .format(cfg.PROBLEM.TYPE))
+        elif cfg.PROBLEM.TYPE == 'SUPER_RESOLUTION':
             if cfg.PROBLEM.NDIM == '2D' and model_arch not in ['edsr', 'rcan', 'dfcan', 'wdsr', 'unet', 'resunet', 'resunet++', 'seunet', 'attention_unet', 'multiresunet']:
                 raise ValueError("Architectures available for 2D 'SUPER_RESOLUTION' are: ['edsr', 'rcan', 'dfcan', 'wdsr', 'unet', 'resunet', 'resunet++', 'seunet', 'attention_unet', 'multiresunet']")
             elif cfg.PROBLEM.NDIM == '3D':
                 if model_arch not in ['unet', 'resunet', 'resunet++', 'seunet', 'attention_unet', 'multiresunet']:
                     raise ValueError("Architectures available for 3D 'SUPER_RESOLUTION' are: ['unet', 'resunet', 'resunet++', 'seunet', 'attention_unet', 'multiresunet']")
                 assert cfg.MODEL.UNET_SR_UPSAMPLE_POSITION in ["pre", "post"], "'MODEL.UNET_SR_UPSAMPLE_POSITION' not in ['pre', 'post']"
-        if cfg.PROBLEM.TYPE == 'SELF_SUPERVISED':
+        elif cfg.PROBLEM.TYPE == 'IMAGE_TO_IMAGE':
+            if model_arch not in ['edsr', 'rcan', 'dfcan', 'wdsr', 'unet', 'resunet', 'resunet++', 'seunet', 'attention_unet', 'unetr', 'multiresunet']:
+                raise ValueError("Architectures available for 2D 'SUPER_RESOLUTION' are: ['edsr', 'rcan', 'dfcan', 'wdsr', 'unet', 'resunet', 'resunet++', 'seunet', 'attention_unet', 'unetr', 'multiresunet']")
+        elif cfg.PROBLEM.TYPE == 'SELF_SUPERVISED':
             if model_arch not in ['unet', 'resunet', 'resunet++', 'attention_unet', 'multiresunet', 'seunet',  
                 'unetr', 'edsr', 'rcan', 'dfcan', 'wdsr', 'vit', 'mae']:
                 raise ValueError("'SELF_SUPERVISED' models available are these: ['unet', 'resunet', 'resunet++', 'attention_unet', 'multiresunet', 'seunet', " 
                     "'unetr', 'edsr', 'rcan', 'dfcan', 'wdsr', 'vit', 'mae']")
-        if cfg.PROBLEM.TYPE == 'CLASSIFICATION':
+        elif cfg.PROBLEM.TYPE == 'CLASSIFICATION':
             if model_arch not in ['simple_cnn', 'vit'] and 'efficientnet' not in model_arch:
                 raise ValueError("Architectures available for 'CLASSIFICATION' are: ['simple_cnn', 'efficientnet_b[0-7]', 'vit']")
             if cfg.PROBLEM.NDIM == '3D' and 'efficientnet' in model_arch:
                 raise ValueError("EfficientNet architectures are only available for 2D images")
         if model_arch in ['unetr', 'vit', 'mae']:    
             if model_arch == 'mae' and cfg.PROBLEM.TYPE != 'SELF_SUPERVISED':
                 raise ValueError("'mae' model can only be used in 'SELF_SUPERVISED' workflow")
@@ -686,15 +689,17 @@
                 raise ValueError("'TRAIN.LR_SCHEDULER.REDUCEONPLATEAU_PATIENCE' needs to be set when 'TRAIN.LR_SCHEDULER.NAME' is 'reduceonplateau'")
             if cfg.TRAIN.LR_SCHEDULER.REDUCEONPLATEAU_PATIENCE >= cfg.TRAIN.PATIENCE:
                 raise ValueError("'TRAIN.LR_SCHEDULER.REDUCEONPLATEAU_PATIENCE' needs to be less than 'TRAIN.PATIENCE' ")
       
         if cfg.TRAIN.LR_SCHEDULER.NAME == 'warmupcosine':
             if cfg.TRAIN.LR_SCHEDULER.WARMUP_COSINE_DECAY_EPOCHS == -1:
                 raise ValueError("'TRAIN.LR_SCHEDULER.WARMUP_COSINE_DECAY_EPOCHS' needs to be set when 'TRAIN.LR_SCHEDULER.NAME' is 'warmupcosine'")
-             
+            if cfg.TRAIN.LR_SCHEDULER.WARMUP_COSINE_DECAY_EPOCHS > cfg.TRAIN.EPOCHS:
+                raise ValueError("'TRAIN.LR_SCHEDULER.WARMUP_COSINE_DECAY_EPOCHS' needs to be less than 'TRAIN.EPOCHS'")
+
     #### Augmentation ####
     if cfg.AUGMENTOR.ENABLE:
         if not check_value(cfg.AUGMENTOR.DA_PROB):
             raise ValueError("AUGMENTOR.DA_PROB not in [0, 1] range")
         if cfg.AUGMENTOR.RANDOM_ROT:
             if not check_value(cfg.AUGMENTOR.RANDOM_ROT_RANGE, (-360,360)):
                 raise ValueError("AUGMENTOR.RANDOM_ROT_RANGE values needs to be between [-360,360]")
```

### Comparing `biapy-3.4.2/biapy/engine/classification.py` & `biapy-3.4.3/biapy/engine/classification.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,20 +2,22 @@
 import torch
 import math
 import numpy as np
 import pandas as pd
 from tqdm import tqdm
 from sklearn.metrics import accuracy_score, confusion_matrix, classification_report
 from torchmetrics import Accuracy
+from sklearn.model_selection import StratifiedKFold
 
 from biapy.engine.base_workflow import Base_Workflow
 from biapy.data.pre_processing import norm_range01
 from biapy.data.data_2D_manipulation import load_data_classification
 from biapy.data.data_3D_manipulation import load_3d_data_classification
 from biapy.utils.misc import is_main_process
+from biapy.data.pre_processing import preprocess_data
 
 class Classification_Workflow(Base_Workflow):
     """
     Classification workflow where the goal of this workflow is to assing a label to the input image.
     More details in `our documentation <https://biapy.readthedocs.io/en/latest/workflows/classification.html>`_. 
 
     Parameters
@@ -124,19 +126,22 @@
         if self.cfg.TRAIN.ENABLE:
             print("##########################\n"
                   "#   LOAD TRAINING DATA   #\n"
                   "##########################\n")
             if self.cfg.DATA.TRAIN.IN_MEMORY:
                 val_split = self.cfg.DATA.VAL.SPLIT_TRAIN if self.cfg.DATA.VAL.FROM_TRAIN else 0.
                 f_name = load_data_classification if self.cfg.PROBLEM.NDIM == '2D' else load_3d_data_classification
+                preprocess_cfg = self.cfg.DATA.PREPROCESS if self.cfg.DATA.PREPROCESS.TRAIN else None
+                preprocess_fn = preprocess_data if self.cfg.DATA.PREPROCESS.TRAIN else None
                 print("0) Loading train images . . .")
                 objs = f_name(self.cfg.DATA.TRAIN.PATH, self.cfg.DATA.PATCH_SIZE, convert_to_rgb=self.cfg.DATA.FORCE_RGB,
                     expected_classes=self.cfg.MODEL.N_CLASSES, cross_val=self.cfg.DATA.VAL.CROSS_VAL, 
                     cross_val_nsplits=self.cfg.DATA.VAL.CROSS_VAL_NFOLD, cross_val_fold=self.cfg.DATA.VAL.CROSS_VAL_FOLD, 
-                    val_split=val_split, seed=self.cfg.SYSTEM.SEED, shuffle_val=self.cfg.DATA.VAL.RANDOM)
+                    val_split=val_split, seed=self.cfg.SYSTEM.SEED, shuffle_val=self.cfg.DATA.VAL.RANDOM, 
+                    preprocess_cfg=preprocess_cfg, preprocess_f=preprocess_fn)
             
                 if self.cfg.DATA.VAL.FROM_TRAIN:
                     if self.cfg.DATA.VAL.CROSS_VAL:
                         self.X_train, self.Y_train, self.X_val, self.Y_val, self.train_filenames, self.cross_val_samples_ids = objs
                     else:
                         self.X_train, self.Y_train, self.X_val, self.Y_val, self.train_filenames = objs
                 else:
@@ -148,17 +153,19 @@
             ##################
             ### VALIDATION ###
             ##################
             if not self.cfg.DATA.VAL.FROM_TRAIN:
                 if self.cfg.DATA.VAL.IN_MEMORY:
                     print("1) Loading validation images . . .")
                     f_name = load_data_classification if self.cfg.PROBLEM.NDIM == '2D' else load_3d_data_classification
+                    preprocess_cfg = self.cfg.DATA.PREPROCESS if self.cfg.DATA.PREPROCESS.VAL else None
+                    preprocess_fn = preprocess_data if self.cfg.DATA.PREPROCESS.VAL else None
                     self.X_val, self.Y_val, _ = f_name(self.cfg.DATA.VAL.PATH, self.cfg.DATA.PATCH_SIZE, 
                         convert_to_rgb=self.cfg.DATA.FORCE_RGB, expected_classes=self.cfg.MODEL.N_CLASSES, 
-                        val_split=0)
+                        val_split=0, preprocess_cfg=preprocess_cfg, preprocess_f=preprocess_fn)
 
                     if self.Y_val is not None and len(self.X_val) != len(self.Y_val):
                         raise ValueError("Different number of raw and ground truth items ({} vs {}). "
                             "Please check the data!".format(len(self.X_val), len(self.Y_val)))
                 else:
                     self.X_val, self.Y_val = None, None
 
@@ -170,41 +177,43 @@
             print("######################\n"
                   "#   LOAD TEST DATA   #\n"
                   "######################\n")
             if not self.cfg.DATA.TEST.USE_VAL_AS_TEST:
                 if self.cfg.DATA.TEST.IN_MEMORY:
                     print("2) Loading test images . . .")
                     f_name = load_data_classification if self.cfg.PROBLEM.NDIM == '2D' else load_3d_data_classification
+                    preprocess_cfg = self.cfg.DATA.PREPROCESS if self.cfg.DATA.PREPROCESS.TEST else None
+                    preprocess_fn = preprocess_data if self.cfg.DATA.PREPROCESS.TEST else None
                     self.X_test, self.Y_test, self.test_filenames = f_name(self.cfg.DATA.TEST.PATH, self.cfg.DATA.PATCH_SIZE,
-                        convert_to_rgb=self.cfg.DATA.FORCE_RGB, 
+                        convert_to_rgb=self.cfg.DATA.FORCE_RGB, preprocess_cfg=preprocess_cfg, preprocess_f=preprocess_fn,
                         expected_classes=self.cfg.MODEL.N_CLASSES if self.cfg.DATA.TEST.LOAD_GT else None, val_split=0)
                     self.class_names = sorted(next(os.walk(self.cfg.DATA.TEST.PATH))[1])
                 else:
                     self.X_test, self.Y_test = None, None
 
                 self.class_names = sorted(next(os.walk(self.cfg.DATA.TEST.PATH))[1])
                 if self.test_filenames is None:
                     self.test_filenames = []
                     for c_num, folder in enumerate(self.class_names):
                         self.test_filenames += sorted(next(os.walk(os.path.join(self.cfg.DATA.TEST.PATH, folder)))[2])
             else:
                 # The test is the validation, and as it is only available when validation is obtained from train and when 
                 # cross validation is enabled, the test set files reside in the train folder
                 self.X_test, self.Y_test = None, None
+                self.class_names = sorted(next(os.walk(self.cfg.DATA.TRAIN.PATH))[1])
                 if self.cross_val_samples_ids is None:                      
                     # Split the test as it was the validation when train is not enabled 
                     skf = StratifiedKFold(n_splits=self.cfg.DATA.VAL.CROSS_VAL_NFOLD, shuffle=self.cfg.DATA.VAL.RANDOM,
                         random_state=self.cfg.SYSTEM.SEED)
                     fold = 1
                     test_index = None
-                    self.class_names = sorted(next(os.walk(self.cfg.DATA.TRAIN.PATH))[2])
                     self.test_filenames = []
                     B = []
                     for c_num, folder in enumerate(self.class_names):
-                        ids += sorted(next(os.walk(os.path.join(self.cfg.DATA.TRAIN.PATH,folder)))[2])
+                        ids = sorted(next(os.walk(os.path.join(self.cfg.DATA.TRAIN.PATH,folder)))[2])
                         B.append((c_num,)*len(ids))
                         self.test_filenames += ids
                     A = np.zeros(len(self.test_filenames)) 
                     B = np.concatenate(B, 0)  
                 
                     for _, te_index in skf.split(A, B):
                         if self.cfg.DATA.VAL.CROSS_VAL_FOLD == fold:
@@ -212,14 +221,20 @@
                             break
                         fold += 1
                     if len(self.cross_val_samples_ids) > 5:
                         print("Fold number {} used for test data. Printing the first 5 ids: {}".format(fold, self.cross_val_samples_ids[:5]))
                     else:
                         print("Fold number {}. Indexes used in cross validation: {}".format(fold, self.cross_val_samples_ids))
                 
+                if self.test_filenames is None:
+                    self.test_filenames = []
+                    for c_num, folder in enumerate(self.class_names):
+                        f = os.path.join(self.cfg.DATA.TRAIN.PATH, folder)
+                        ids = sorted(next(os.walk(f))[2])
+                        self.test_filenames += ids
                 self.test_filenames = [x for i, x in enumerate(self.test_filenames) if i in self.cross_val_samples_ids]
                 self.original_test_path = self.orig_train_path
                 self.original_test_mask_path = self.orig_train_mask_path  
 
     def process_sample(self, norm):   
         """
         Function to process a sample in the inference phase.
```

### Comparing `biapy-3.4.2/biapy/engine/denoising.py` & `biapy-3.4.3/biapy/engine/denoising.py`

 * *Files identical despite different names*

### Comparing `biapy-3.4.2/biapy/engine/detection.py` & `biapy-3.4.3/biapy/engine/detection.py`

 * *Files 0% similar despite different names*

```diff
@@ -268,24 +268,23 @@
 
             # Detection watershed
             if self.cfg.TEST.POST_PROCESSING.DET_WATERSHED:
                 data_filename = os.path.join(self.cfg.DATA.TEST.PATH, filenames[0])
                 w_dir = os.path.join(self.cfg.PATHS.WATERSHED_DIR, filenames[0])
                 check_wa = w_dir if self.cfg.PROBLEM.DETECTION.DATA_CHECK_MW else None
                 points_pred = detection_watershed(points_pred, all_points, data_filename, self.cfg.TEST.POST_PROCESSING.DET_WATERSHED_FIRST_DILATION,
-                    clases, ndim=ndim, donuts_classes=self.cfg.TEST.POST_PROCESSING.DET_WATERSHED_DONUTS_CLASSES,
+                    nclasses=classes, ndim=ndim, donuts_classes=self.cfg.TEST.POST_PROCESSING.DET_WATERSHED_DONUTS_CLASSES,
                     donuts_patch=self.cfg.TEST.POST_PROCESSING.DET_WATERSHED_DONUTS_PATCH, 
                     donuts_nucleus_diameter=self.cfg.TEST.POST_PROCESSING.DET_WATERSHED_DONUTS_NUCLEUS_DIAMETER, save_dir=check_wa)
                 
                 # Instance filtering by properties     
                 points_pred, d_result = measure_morphological_props_and_filter(points_pred, self.cfg.DATA.TEST.RESOLUTION, 
                     properties=self.cfg.TEST.POST_PROCESSING.MEASURE_PROPERTIES.REMOVE_BY_PROPERTIES.PROPS, 
                     prop_values=self.cfg.TEST.POST_PROCESSING.MEASURE_PROPERTIES.REMOVE_BY_PROPERTIES.VALUES, 
-                    comp_signs=self.cfg.TEST.POST_PROCESSING.MEASURE_PROPERTIES.REMOVE_BY_PROPERTIES.SIGN, 
-                    coords_list=np.concatenate(all_points, axis=0))
+                    comp_signs=self.cfg.TEST.POST_PROCESSING.MEASURE_PROPERTIES.REMOVE_BY_PROPERTIES.SIGN)
 
                 if file_ext in ['.hdf5', '.h5', ".zarr"]:
                     write_chunked_data(np.expand_dims(np.expand_dims(points_pred,-1),0), self.cfg.PATHS.RESULT_DIR.DET_ASSOC_POINTS, 
                         filenames[0], dtype_str="uint8", verbose=self.cfg.TEST.VERBOSE)
                 else:
                     save_tif(np.expand_dims(np.expand_dims(points_pred,0),-1), self.cfg.PATHS.RESULT_DIR.PER_IMAGE_POST_PROCESSING,
                         filenames, verbose=self.cfg.TEST.VERBOSE)
@@ -297,15 +296,15 @@
         if len(aux) != 0:
             if self.cfg.PROBLEM.NDIM == "3D":
                 prob = pred[aux[:,0], aux[:,1], aux[:,2], all_classes]
                 prob = np.concatenate(prob, axis=0)
                 all_classes = np.concatenate(all_classes, axis=0)
                 if self.cfg.TEST.POST_PROCESSING.DET_WATERSHED:
                     df = pd.DataFrame(zip(d_result['labels'], list(aux[:,0]), list(aux[:,1]), list(aux[:,2]), list(prob), list(all_classes),
-                        d_result['npixels'], d_result['areas'], d_result['circularities'], d_result['diameters'], d_result['perimeters'], 
+                        d_result['npixels'], d_result['areas'], d_result['sphericities'], d_result['diameters'], d_result['perimeters'], 
                         d_result['comment'], d_result['conditions']), columns =['pred_id', 'axis-0', 'axis-1', 'axis-2', 'probability', 
                         'class', 'npixels', 'volume', 'sphericity', 'diameter', 'perimeter (surface area)', 'comment', 'conditions'])
                     df = df.sort_values(by=['pred_id'])   
                 else:
                     labels = []
                     for i, pred_coordinates in enumerate(all_points):
                         for j in range(len(pred_coordinates)):
@@ -335,15 +334,15 @@
             # Save just the points and their probabilities 
             os.makedirs(self.cfg.PATHS.RESULT_DIR.DET_LOCAL_MAX_COORDS_CHECK, exist_ok=True)
             df.to_csv(os.path.join(self.cfg.PATHS.RESULT_DIR.DET_LOCAL_MAX_COORDS_CHECK, os.path.splitext(filenames[0])[0]+'_full_info.csv'))
             if self.cfg.TEST.POST_PROCESSING.DET_WATERSHED:
                 if ndim == 2:
                     cols = ['class', 'pred_id', 'npixels', 'area', 'circularity', 'perimeter', 'elongation', 'comment', 'conditions']
                 else:
-                    cols = ['class', 'pred_id', 'npixels', 'volume', 'sphericity', 'perimeter', 'surface area', 'comment', 'conditions']
+                    cols = ['class', 'pred_id', 'npixels', 'volume', 'sphericity', 'perimeter (surface area)', 'comment', 'conditions']
                 df = df.drop(columns=cols)
             else:
                 df = df.drop(columns=['class'])
             df.to_csv(os.path.join(self.cfg.PATHS.RESULT_DIR.DET_LOCAL_MAX_COORDS_CHECK, os.path.splitext(filenames[0])[0]+'_prob.csv'))
 
         # Calculate detection metrics
         if self.use_gt:
@@ -468,18 +467,18 @@
             if self.cfg.TEST.VERBOSE:
                 print("Creating the image with a summary of detected points and false positives with colors . . .")
             if not self.by_chunks:
                 points_pred = np.zeros(pred_shape[:-1]+(3,), dtype=np.uint8)
                 for ch, gt_coords in enumerate(gt_all_coords):
                     # if gt_assoc is None: 
                     gt_assoc, fp = None, None
-                    if len(dfs) > 0 and len(dfs[i]) > 0:
-                        if dfs[i][0] is not None:
+                    if len(dfs) > 0 and len(dfs[ch]) > 0:
+                        if dfs[ch][0] is not None:
                             gt_assoc = dfs[ch][0]
-                        if dfs[i][1] is not None:
+                        if dfs[ch][1] is not None:
                             fp = dfs[ch][1]
 
                     # TP and FN
                     gt_id_img = np.zeros(pred_shape[:-1], dtype=np.uint32)
                     for j, cor in enumerate(gt_coords):
                         z,y,x = cor
                         z,y,x = int(z),int(y),int(x)
@@ -728,27 +727,30 @@
         with ThreadPoolExecutor(max_workers=workers) as executor:
             futures = []
             for z in tqdm(range(z_vols), disable=not is_main_process()):
                 for y in range(y_vols):
                     for x in range(x_vols):
                         futures.append(executor.submit(self.process_patch, z, y, x, _filename, total_patches, c, pred, d, file_ext, z_dim, y_dim, x_dim))
                         c+=1
-
+        df = None
         for future in futures:
             df_patch, fname = future.result()
             if df_patch is not None:
                 if 'df' not in locals():
                     df = df_patch.copy()
                     df['file'] = fname
                 else:
                     df_patch['file'] = fname
                     df = pd.concat([df, df_patch], ignore_index=True)
 
         # Take point coords
         pred_coordinates = []
+        if df is None: 
+            print("No points created, skipping evaluation . . .")
+            return 
         coordz = df['axis-0'].tolist()
         coordy = df['axis-1'].tolist()
         coordx = df['axis-2'].tolist()
         for z,y,x in zip(coordz,coordy,coordx):
             pred_coordinates.append([z,y,x])
 
         # Apply post-processing of removing points
```

### Comparing `biapy-3.4.2/biapy/engine/image_to_image.py` & `biapy-3.4.3/biapy/engine/image_to_image.py`

 * *Files identical despite different names*

### Comparing `biapy-3.4.2/biapy/engine/instance_seg.py` & `biapy-3.4.3/biapy/engine/instance_seg.py`

 * *Files 2% similar despite different names*

```diff
@@ -109,14 +109,15 @@
             
         # Workflow specific training variables
         self.mask_path = cfg.DATA.TRAIN.GT_PATH
         self.load_Y_val = True
 
         # Specific instance segmentation post-processing
         if self.cfg.TEST.POST_PROCESSING.VORONOI_ON_MASK or \
+            self.cfg.TEST.POST_PROCESSING.CLEAR_BORDER or\
             self.cfg.TEST.POST_PROCESSING.MEASURE_PROPERTIES.REMOVE_BY_PROPERTIES.ENABLE or \
             self.cfg.TEST.POST_PROCESSING.REPARE_LARGE_BLOBS_SIZE != -1:
             self.post_processing['instance_post'] = True
         else:
             self.post_processing['instance_post'] = False            
         self.instances_already_created = False 
 
@@ -383,57 +384,64 @@
                             [os.path.splitext(filenames[0])[0]+'_th_{}.tif'.format(thr)], verbose=self.cfg.TEST.VERBOSE)          
                     del colored_result
 
         ###################
         # Post-processing #
         ###################
         if self.cfg.TEST.POST_PROCESSING.REPARE_LARGE_BLOBS_SIZE != -1:
-            w_pred = repare_large_blobs(w_pred, self.cfg.TEST.POST_PROCESSING.REPARE_LARGE_BLOBS_SIZE)
+            if self.cfg.PROBLEM.NDIM == "2D": w_pred = w_pred[0]
+            w_pred = repare_large_blobs(w_pred[0], self.cfg.TEST.POST_PROCESSING.REPARE_LARGE_BLOBS_SIZE)
+            if self.cfg.PROBLEM.NDIM == "2D": w_pred = np.expand_dims(w_pred,0)
+        
+        if self.cfg.TEST.POST_PROCESSING.VORONOI_ON_MASK:
+            w_pred = voronoi_on_mask(w_pred, pred, th=self.cfg.TEST.POST_PROCESSING.VORONOI_TH, verbose=self.cfg.TEST.VERBOSE)
+        del pred
+
+        if self.cfg.TEST.POST_PROCESSING.CLEAR_BORDER:
+            print("Clearing borders . . .")
+            if self.cfg.PROBLEM.NDIM == "2D": w_pred = w_pred[0]
+            w_pred = clear_border(w_pred)
+            if self.cfg.PROBLEM.NDIM == "2D": w_pred = np.expand_dims(w_pred,0)
 
         if self.cfg.TEST.POST_PROCESSING.MEASURE_PROPERTIES.ENABLE or \
             self.cfg.TEST.POST_PROCESSING.MEASURE_PROPERTIES.REMOVE_BY_PROPERTIES.ENABLE:
-            w_pred, d_result = measure_morphological_props_and_filter(w_pred.squeeze(), resolution, 
+            if self.cfg.PROBLEM.NDIM == "2D": w_pred = w_pred[0]
+            w_pred, d_result = measure_morphological_props_and_filter(w_pred, resolution, 
                 filter_instances=self.cfg.TEST.POST_PROCESSING.MEASURE_PROPERTIES.REMOVE_BY_PROPERTIES.ENABLE,
                 properties=self.cfg.TEST.POST_PROCESSING.MEASURE_PROPERTIES.REMOVE_BY_PROPERTIES.PROPS, 
                 prop_values=self.cfg.TEST.POST_PROCESSING.MEASURE_PROPERTIES.REMOVE_BY_PROPERTIES.VALUES,
                 comp_signs=self.cfg.TEST.POST_PROCESSING.MEASURE_PROPERTIES.REMOVE_BY_PROPERTIES.SIGN)
+            if self.cfg.PROBLEM.NDIM == "2D": w_pred = np.expand_dims(w_pred,0)
 
             # Save all instance stats            
             if self.cfg.PROBLEM.NDIM == "2D":
                 df = pd.DataFrame(zip(np.array(d_result['labels'], dtype=np.uint64), list(d_result['centers'][:,0]), list(d_result['centers'][:,1]), 
                     d_result['npixels'], d_result['areas'], d_result['circularities'], d_result['diameters'], d_result['perimeters'], d_result['elongations'],
                     d_result['comment'], d_result['conditions']), columns=['label', 'axis-0', 'axis-1', 'npixels', 'area', 'circularity', 'diameter', 
                     'perimeter', 'elongation', 'comment', 'conditions'])
             else:
                 df = pd.DataFrame(zip(np.array(d_result['labels'], dtype=np.uint64), list(d_result['centers'][:,0]), list(d_result['centers'][:,1]), 
-                    list(d_result['centers'][:,2]), d_result['npixels'], d_result['areas'], d_result['circularities'], d_result['diameters'], 
+                    list(d_result['centers'][:,2]), d_result['npixels'], d_result['areas'], d_result['sphericities'], d_result['diameters'], 
                     d_result['perimeters'], d_result['comment'], d_result['conditions']), columns=['label', 'axis-0', 'axis-1', 
                     'axis-2', 'npixels', 'volume', 'sphericity', 'diameter', 'perimeter (surface area)', 'comment', 'conditions'])
             df = df.sort_values(by=['label'])   
             df.to_csv(os.path.join(out_dir, os.path.splitext(filenames[0])[0]+'_full_stats.csv'), index=False)
             # Save only remain instances stats
             df = df[df["comment"].str.contains("Strange")==False] 
             os.makedirs(out_dir_post_proc, exist_ok=True)
             df.to_csv(os.path.join(out_dir_post_proc, os.path.splitext(filenames[0])[0]+'_filtered_stats.csv'), index=False)
             del df
 
-        if self.cfg.TEST.POST_PROCESSING.VORONOI_ON_MASK:
-            w_pred = voronoi_on_mask(w_pred, pred, th=self.cfg.TEST.POST_PROCESSING.VORONOI_TH, verbose=self.cfg.TEST.VERBOSE)
-        del pred
-
-        if self.cfg.TEST.POST_PROCESSING.CLEAR_BORDER:
-            print("Clearing borders . . .")
-            w_pred = clear_border(w_pred)
-
         results_post_proc = None
         results_class_post_proc = None
         if self.post_processing['instance_post']:
+            if self.cfg.PROBLEM.NDIM == "2D": w_pred = w_pred[0]
+
             # Multi-head: instances + classification
             if self.cfg.MODEL.N_CLASSES > 2:
-                w_pred = w_pred.squeeze()
                 class_channel = np.where(w_pred>0, class_channel, 0) # Adapt changes to post-processed w_pred
                 save_tif(np.expand_dims(np.concatenate([np.expand_dims(w_pred,-1), np.expand_dims(class_channel,-1)],axis=-1),0), 
                     out_dir_post_proc, filenames, verbose=self.cfg.TEST.VERBOSE)
             else:
                 save_tif(np.expand_dims(np.expand_dims(w_pred,-1),0), out_dir_post_proc, filenames, verbose=self.cfg.TEST.VERBOSE)
 
             if self.cfg.TEST.MATCHING_STATS and (self.cfg.DATA.TEST.LOAD_GT or self.cfg.DATA.TEST.USE_VAL_AS_TEST):
@@ -442,17 +450,15 @@
                     # Measure class IoU
                     class_iou = self.jaccard_index_matching(torch.as_tensor(class_channel.squeeze().astype(np.int32)),
                         torch.as_tensor(_Y_classes.squeeze().astype(np.int32)))
                     class_iou = class_iou.item() if not torch.isnan(class_iou) else 0
                     print(f"Class IoU (post-processing): {class_iou}")
                     results_class_post_proc = class_iou
                     
-                # Add extra dimension if working in 2D
-                if w_pred.ndim == 2:
-                    w_pred = np.expand_dims(w_pred,0)
+                if self.cfg.PROBLEM.NDIM == "2D": w_pred = np.expand_dims(w_pred,0)
 
                 print("Calculating matching stats after post-processing . . .")
                 results_post_proc = matching(_Y, w_pred, thresh=self.cfg.TEST.MATCHING_STATS_THS, report_matches=True)
                 
                 for i in range(len(results_post_proc)):
                     # Extract TPs, FPs and FNs from the resulting matching data structure 
                     r_stats = results_post_proc[i] 
@@ -608,15 +614,15 @@
         """
         super().after_all_images()
         if self.cfg.TEST.ANALIZE_2D_IMGS_AS_3D_STACK:
             print("Analysing all images as a 3D stack . . .")    
             if type(self.all_pred) is list:
                 self.all_pred = np.concatenate(self.all_pred)
             resolution = self.cfg.DATA.TEST.RESOLUTION if len(self.cfg.DATA.TEST.RESOLUTION) == 3 else (self.cfg.DATA.TEST.RESOLUTION[0],)+self.cfg.DATA.TEST.RESOLUTION
-            r, r_post, rcls, rcls_post = self.instance_seg_process(self.all_pred, ["3D_stack.tif"], self.cfg.PATHS.RESULT_DIR.AS_3D_STACK,
+            r, r_post, rcls, rcls_post = self.instance_seg_process(self.all_pred, ["3D_stack_instances.tif"], self.cfg.PATHS.RESULT_DIR.AS_3D_STACK,
                 self.cfg.PATHS.RESULT_DIR.AS_3D_STACK_POST_PROCESSING, resolution)
             if r is not None:
                 self.all_matching_stats_as_3D_stack.append(r)
             if r_post is not None:
                 self.all_matching_stats_as_3D_stack_post.append(r_post)
             if rcls is not None:
                 self.all_class_stats_as_3D_stack.append(rcls)
```

### Comparing `biapy-3.4.2/biapy/engine/metrics.py` & `biapy-3.4.3/biapy/engine/metrics.py`

 * *Files identical despite different names*

### Comparing `biapy-3.4.2/biapy/engine/schedulers/warmup_cosine_decay.py` & `biapy-3.4.3/biapy/engine/schedulers/warmup_cosine_decay.py`

 * *Files identical despite different names*

### Comparing `biapy-3.4.2/biapy/engine/self_supervised.py` & `biapy-3.4.3/biapy/engine/self_supervised.py`

 * *Files identical despite different names*

### Comparing `biapy-3.4.2/biapy/engine/semantic_seg.py` & `biapy-3.4.3/biapy/engine/semantic_seg.py`

 * *Files identical despite different names*

### Comparing `biapy-3.4.2/biapy/engine/super_resolution.py` & `biapy-3.4.3/biapy/engine/super_resolution.py`

 * *Files identical despite different names*

### Comparing `biapy-3.4.2/biapy/engine/train_engine.py` & `biapy-3.4.3/biapy/engine/train_engine.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,14 +29,18 @@
             lr_scheduler.adjust_learning_rate(optimizer, step / len(data_loader) + epoch)
 
         it = start_steps + step  # global training iteration
 
         # Gather inputs
         targets = prepare_targets(targets, batch)
 
+        if batch.shape[1:-1] != cfg.DATA.PATCH_SIZE[:-1]:
+            raise ValueError("Trying to input data with different shape than 'DATA.PATCH_SIZE'. Check your configuration."
+                f" Input: {batch.shape[1:-1]} vs PATCH_SIZE: {cfg.DATA.PATCH_SIZE[:-1]}")
+                
         # Pass the images through the model
         # TODO: control autocast and mixed precision
         with torch.cuda.amp.autocast(enabled=False):
             outputs = activations(model_call_func(batch, is_train=True), training=True)
             loss = loss_function(outputs, targets)
 
         loss_value = loss.item()
```

### Comparing `biapy-3.4.2/biapy/models/__init__.py` & `biapy-3.4.3/biapy/models/__init__.py`

 * *Files identical despite different names*

### Comparing `biapy-3.4.2/biapy/models/attention_unet.py` & `biapy-3.4.3/biapy/models/attention_unet.py`

 * *Files identical despite different names*

### Comparing `biapy-3.4.2/biapy/models/blocks.py` & `biapy-3.4.3/biapy/models/blocks.py`

 * *Files identical despite different names*

### Comparing `biapy-3.4.2/biapy/models/dfcan.py` & `biapy-3.4.3/biapy/models/dfcan.py`

 * *Files identical despite different names*

### Comparing `biapy-3.4.2/biapy/models/edsr.py` & `biapy-3.4.3/biapy/models/edsr.py`

 * *Files identical despite different names*

### Comparing `biapy-3.4.2/biapy/models/efficientnet.py` & `biapy-3.4.3/biapy/models/efficientnet.py`

 * *Files identical despite different names*

### Comparing `biapy-3.4.2/biapy/models/mae.py` & `biapy-3.4.3/biapy/models/mae.py`

 * *Files 2% similar despite different names*

```diff
@@ -120,17 +120,22 @@
         if masking_type == "random":
             self.masking_func = self.random_masking
         else:
             self.masking_func = self.grid_masking
             
             # Define grid mask, as it doesn't change over epochs
             D, L = embed_dim, self.patch_embed.num_patches
-            self.mask = torch.zeros([int(math.sqrt(1024)),int(math.sqrt(1024))], device=device)
-            self.mask[::2,::2] = 1
-            self.mask[1::2,1::2] = 1
+            if self.ndim == 2:
+                self.mask = torch.zeros([img_size//patch_size,img_size//patch_size], device=device)
+                self.mask[::2,::2] = 1
+                self.mask[1::2,1::2] = 1
+            else:
+                self.mask = torch.zeros([img_size//patch_size,img_size//patch_size,img_size//patch_size], device=device)
+                self.mask[::2,::2,::2] = 1
+                self.mask[1::2,1::2,1::2] = 1
             self.mask = self.mask.flatten()
             self.ids_keep = torch.argsort(self.mask)[:L//2].unsqueeze(-1).repeat(1, 1, D)
             self.mask = self.mask.unsqueeze(0)
             self.ids_restore = torch.argsort(torch.argsort(self.mask))
 
         self.norm_pix_loss = norm_pix_loss
 
@@ -411,16 +416,14 @@
             Predicted images's mask. In 2D: ``(N, H, W, C)``, in 3D: ``(N, Z, H, W, C)``. Where ``N`` is the batch size, 
             ``C`` are the channels, ``Z`` image depth, ``H`` image height and ``W`` image's width. 
         
         pred_visi : 4D/5D Numpy array
             Predicted image with visible patches. In 2D: ``(N, H, W, C)``, in 3D: ``(N, Z, H, W, C)``. Where ``N`` is the batch size, 
             ``C`` are the channels, ``Z`` image depth, ``H`` image height and ``W`` image's width. 
         """
-        print("Saving MAE images . . .")
-
         pred = np.zeros(_x.shape, dtype=dtype)
         p_mask = np.zeros(_x.shape, dtype=dtype)
         pred_visi = np.zeros(_x.shape, dtype=dtype)
         for i in range(len(_x)):
             y = self.unpatchify(_y[i].unsqueeze(dim=0))[0]
             y = y.detach().cpu()
```

### Comparing `biapy-3.4.2/biapy/models/multiresunet.py` & `biapy-3.4.3/biapy/models/multiresunet.py`

 * *Files identical despite different names*

### Comparing `biapy-3.4.2/biapy/models/rcan.py` & `biapy-3.4.3/biapy/models/rcan.py`

 * *Files identical despite different names*

### Comparing `biapy-3.4.2/biapy/models/resunet++.py` & `biapy-3.4.3/biapy/models/resunet++.py`

 * *Files identical despite different names*

### Comparing `biapy-3.4.2/biapy/models/resunet.py` & `biapy-3.4.3/biapy/models/resunet.py`

 * *Files identical despite different names*

### Comparing `biapy-3.4.2/biapy/models/seunet.py` & `biapy-3.4.3/biapy/models/seunet.py`

 * *Files identical despite different names*

### Comparing `biapy-3.4.2/biapy/models/simple_cnn.py` & `biapy-3.4.3/biapy/models/simple_cnn.py`

 * *Files identical despite different names*

### Comparing `biapy-3.4.2/biapy/models/tr_layers.py` & `biapy-3.4.3/biapy/models/tr_layers.py`

 * *Files identical despite different names*

### Comparing `biapy-3.4.2/biapy/models/unet.py` & `biapy-3.4.3/biapy/models/unet.py`

 * *Files identical despite different names*

### Comparing `biapy-3.4.2/biapy/models/unetr.py` & `biapy-3.4.3/biapy/models/unetr.py`

 * *Files identical despite different names*

### Comparing `biapy-3.4.2/biapy/models/vit.py` & `biapy-3.4.3/biapy/models/vit.py`

 * *Files identical despite different names*

### Comparing `biapy-3.4.2/biapy/models/wdsr.py` & `biapy-3.4.3/biapy/models/wdsr.py`

 * *Files identical despite different names*

### Comparing `biapy-3.4.2/biapy/utils/callbacks.py` & `biapy-3.4.3/biapy/utils/callbacks.py`

 * *Files identical despite different names*

### Comparing `biapy-3.4.2/biapy/utils/matching.py` & `biapy-3.4.3/biapy/utils/matching.py`

 * *Files identical despite different names*

### Comparing `biapy-3.4.2/biapy/utils/misc.py` & `biapy-3.4.3/biapy/utils/misc.py`

 * *Files identical despite different names*

### Comparing `biapy-3.4.2/biapy/utils/scripts/calculate_detection_metrics.py` & `biapy-3.4.3/biapy/utils/scripts/calculate_detection_metrics.py`

 * *Files identical despite different names*

### Comparing `biapy-3.4.2/biapy/utils/scripts/calculate_metrics_3D.py` & `biapy-3.4.3/biapy/utils/scripts/calculate_metrics_3D.py`

 * *Files identical despite different names*

### Comparing `biapy-3.4.2/biapy/utils/scripts/create_probability_csv.py` & `biapy-3.4.3/biapy/utils/scripts/create_probability_csv.py`

 * *Files identical despite different names*

### Comparing `biapy-3.4.2/biapy/utils/scripts/crop_2D_dataset.py` & `biapy-3.4.3/biapy/utils/scripts/crop_2D_dataset.py`

 * *Files identical despite different names*

### Comparing `biapy-3.4.2/biapy/utils/scripts/crop_3D_dataset.py` & `biapy-3.4.3/biapy/utils/scripts/crop_3D_dataset.py`

 * *Files identical despite different names*

### Comparing `biapy-3.4.2/biapy/utils/scripts/crop_and_discard_3D_dataset.py` & `biapy-3.4.3/biapy/utils/scripts/crop_and_discard_3D_dataset.py`

 * *Files identical despite different names*

### Comparing `biapy-3.4.2/biapy/utils/scripts/detection_plots.py` & `biapy-3.4.3/biapy/utils/scripts/detection_plots.py`

 * *Files identical despite different names*

### Comparing `biapy-3.4.2/biapy/utils/scripts/detection_probs_to_points.py` & `biapy-3.4.3/biapy/utils/scripts/detection_probs_to_points.py`

 * *Files identical despite different names*

### Comparing `biapy-3.4.2/biapy/utils/scripts/fill_holes_in_seg_masks.py` & `biapy-3.4.3/biapy/utils/scripts/fill_holes_in_seg_masks.py`

 * *Files identical despite different names*

### Comparing `biapy-3.4.2/biapy/utils/scripts/filter_close_points.py` & `biapy-3.4.3/biapy/utils/scripts/filter_close_points.py`

 * *Files identical despite different names*

### Comparing `biapy-3.4.2/biapy/utils/scripts/from_class_csv_to_folders.py` & `biapy-3.4.3/biapy/utils/scripts/from_class_csv_to_folders.py`

 * *Files identical despite different names*

### Comparing `biapy-3.4.2/biapy/utils/scripts/h5_to_tif.py` & `biapy-3.4.3/biapy/utils/scripts/h5_to_tif.py`

 * *Files identical despite different names*

### Comparing `biapy-3.4.2/biapy/utils/scripts/h5_to_zarr.py` & `biapy-3.4.3/biapy/utils/scripts/h5_to_zarr.py`

 * *Files identical despite different names*

### Comparing `biapy-3.4.2/biapy/utils/scripts/lightmycell_data_preparation.py` & `biapy-3.4.3/biapy/utils/scripts/lightmycell_data_preparation.py`

 * *Files identical despite different names*

### Comparing `biapy-3.4.2/biapy/utils/scripts/merge_dataset_channels.py` & `biapy-3.4.3/biapy/utils/scripts/merge_dataset_channels.py`

 * *Files identical despite different names*

### Comparing `biapy-3.4.2/biapy/utils/scripts/order_axes.py` & `biapy-3.4.3/biapy/utils/scripts/order_axes.py`

 * *Files identical despite different names*

### Comparing `biapy-3.4.2/biapy/utils/scripts/tif_to_h5.py` & `biapy-3.4.3/biapy/utils/scripts/tif_to_h5.py`

 * *Files identical despite different names*

### Comparing `biapy-3.4.2/biapy/utils/util.py` & `biapy-3.4.3/biapy/utils/util.py`

 * *Files identical despite different names*

### Comparing `biapy-3.4.2/biapy.egg-info/PKG-INFO` & `biapy-3.4.3/biapy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: biapy
-Version: 3.4.2
+Version: 3.4.3
 Summary: BiaPy: Bioimage analysis pipelines in Python
 Author-email: Daniel Franco-Barranco <daniel.franco@dipc.org>
 Maintainer-email: Daniel Franco-Barranco <daniel.franco@dipc.org>
 License: MIT License
         
         Copyright (c) 2022 Daniel Franco-Barranco
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: biapy Version: 3.4.2 Summary: BiaPy: Bioimage
+Metadata-Version: 2.1 Name: biapy Version: 3.4.3 Summary: BiaPy: Bioimage
 analysis pipelines in Python Author-email: Daniel Franco-Barranco
 dipc.org> Maintainer-email: Daniel Franco-Barranco
 dipc.org> License: MIT License Copyright (c) 2022 Daniel Franco-Barranco
 Permission is hereby granted, free of charge, to any person obtaining a copy of
 this software and associated documentation files (the "Software"), to deal in
 the Software without restriction, including without limitation the rights to
 use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies
```

### Comparing `biapy-3.4.2/biapy.egg-info/SOURCES.txt` & `biapy-3.4.3/biapy.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -76,8 +76,9 @@
 biapy/utils/scripts/filter_close_points.py
 biapy/utils/scripts/from_class_csv_to_folders.py
 biapy/utils/scripts/h5_to_tif.py
 biapy/utils/scripts/h5_to_zarr.py
 biapy/utils/scripts/lightmycell_data_preparation.py
 biapy/utils/scripts/merge_dataset_channels.py
 biapy/utils/scripts/order_axes.py
+biapy/utils/scripts/run_checks.py
 biapy/utils/scripts/tif_to_h5.py
```

### Comparing `biapy-3.4.2/pyproject.toml` & `biapy-3.4.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "biapy"
-version = "3.4.2"
+version = "3.4.3"
 description = "BiaPy: Bioimage analysis pipelines in Python"
 readme = "README.md"
 requires-python = ">=3.10"
 authors = [{ name = "Daniel Franco-Barranco", email = "daniel.franco@dipc.org" }]
 maintainers = [{ name = "Daniel Franco-Barranco", email = "daniel.franco@dipc.org" }]
 license = { file = "LICENSE.md" }
 classifiers = [
```

