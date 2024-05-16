# Comparing `tmp/toon3d-0.0.2.tar.gz` & `tmp/toon3d-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "toon3d-0.0.2.tar", last modified: Mon May 13 05:32:20 2024, max compression
+gzip compressed data, was "toon3d-0.0.3.tar", last modified: Thu May 16 20:20:55 2024, max compression
```

## Comparing `toon3d-0.0.2.tar` & `toon3d-0.0.3.tar`

### file list

```diff
@@ -1,65 +1,53 @@
-drwxr-xr-x   0 ethanweber (1000282) users    (1000001)        0 2024-05-13 05:32:20.454004 toon3d-0.0.2/
--rw-r--r--   0 ethanweber (1000282) users    (1000001)      826 2024-05-13 05:32:20.454004 toon3d-0.0.2/PKG-INFO
--rw-r--r--   0 ethanweber (1000282) users    (1000001)     5785 2024-05-12 06:19:19.000000 toon3d-0.0.2/README.md
--rw-r--r--   0 ethanweber (1000282) users    (1000001)     1240 2024-05-13 05:31:47.000000 toon3d-0.0.2/pyproject.toml
--rw-r--r--   0 ethanweber (1000282) users    (1000001)       38 2024-05-13 05:32:20.454004 toon3d-0.0.2/setup.cfg
-drwxr-xr-x   0 ethanweber (1000282) users    (1000001)        0 2024-05-13 05:32:20.450004 toon3d-0.0.2/tests/
--rw-r--r--   0 ethanweber (1000282) users    (1000001)      344 2024-03-15 01:48:57.000000 toon3d-0.0.2/tests/test_finetune.py
-drwxr-xr-x   0 ethanweber (1000282) users    (1000001)        0 2024-05-13 05:32:20.450004 toon3d-0.0.2/toon3d/
--rw-r--r--   0 ethanweber (1000282) users    (1000001)        0 2024-03-15 01:48:57.000000 toon3d-0.0.2/toon3d/__init__.py
--rw-r--r--   0 ethanweber (1000282) users    (1000001)     1728 2024-03-15 01:48:57.000000 toon3d-0.0.2/toon3d/color_palette.py
-drwxr-xr-x   0 ethanweber (1000282) users    (1000001)        0 2024-05-13 05:32:20.450004 toon3d-0.0.2/toon3d/configs/
--rw-r--r--   0 ethanweber (1000282) users    (1000001)     1475 2024-03-15 01:48:57.000000 toon3d-0.0.2/toon3d/configs/prompts.py
-drwxr-xr-x   0 ethanweber (1000282) users    (1000001)        0 2024-05-13 05:32:20.450004 toon3d-0.0.2/toon3d/generative/
--rw-r--r--   0 ethanweber (1000282) users    (1000001)    14001 2024-03-15 01:48:57.000000 toon3d-0.0.2/toon3d/generative/ldm3d.py
--rw-r--r--   0 ethanweber (1000282) users    (1000001)    10358 2024-03-15 01:48:57.000000 toon3d-0.0.2/toon3d/generative/marigold.py
-drwxr-xr-x   0 ethanweber (1000282) users    (1000001)        0 2024-05-13 05:32:20.454004 toon3d-0.0.2/toon3d/scripts/
--rw-r--r--   0 ethanweber (1000282) users    (1000001)     4646 2024-05-10 20:12:48.000000 toon3d-0.0.2/toon3d/scripts/colmap_with_corrs.py
--rw-r--r--   0 ethanweber (1000282) users    (1000001)     6596 2024-03-15 01:48:57.000000 toon3d-0.0.2/toon3d/scripts/download_data.py
--rw-r--r--   0 ethanweber (1000282) users    (1000001)    19820 2024-03-15 01:48:57.000000 toon3d-0.0.2/toon3d/scripts/finetune.py
--rw-r--r--   0 ethanweber (1000282) users    (1000001)     8611 2024-05-10 21:53:19.000000 toon3d-0.0.2/toon3d/scripts/process_data.py
--rw-r--r--   0 ethanweber (1000282) users    (1000001)    34172 2024-03-29 05:06:36.000000 toon3d-0.0.2/toon3d/scripts/render.py
--rw-r--r--   0 ethanweber (1000282) users    (1000001)    37741 2024-05-12 17:37:52.000000 toon3d-0.0.2/toon3d/scripts/run.py
--rw-r--r--   0 ethanweber (1000282) users    (1000001)     1185 2024-03-15 01:48:57.000000 toon3d-0.0.2/toon3d/scripts/server.py
--rw-r--r--   0 ethanweber (1000282) users    (1000001)     4685 2024-05-13 05:11:25.000000 toon3d-0.0.2/toon3d/scripts/viser_vis.py
--rw-r--r--   0 ethanweber (1000282) users    (1000001)     2847 2024-03-15 01:48:57.000000 toon3d-0.0.2/toon3d/toon3d_config.py
--rw-r--r--   0 ethanweber (1000282) users    (1000001)     5939 2024-03-15 01:48:57.000000 toon3d-0.0.2/toon3d/toon3d_datamanager.py
--rw-r--r--   0 ethanweber (1000282) users    (1000001)     2290 2024-03-15 01:48:57.000000 toon3d-0.0.2/toon3d/toon3d_dataparser.py
--rw-r--r--   0 ethanweber (1000282) users    (1000001)    17776 2024-03-15 01:48:57.000000 toon3d-0.0.2/toon3d/toon3d_model.py
--rw-r--r--   0 ethanweber (1000282) users    (1000001)     5605 2024-03-15 01:48:57.000000 toon3d-0.0.2/toon3d/toon3d_pipeline.py
--rw-r--r--   0 ethanweber (1000282) users    (1000001)        0 2024-03-15 01:48:57.000000 toon3d-0.0.2/toon3d/toon3d_process_data.py
-drwxr-xr-x   0 ethanweber (1000282) users    (1000001)        0 2024-05-13 05:32:20.454004 toon3d-0.0.2/toon3d/utils/
--rw-r--r--   0 ethanweber (1000282) users    (1000001)     3376 2024-03-15 01:48:57.000000 toon3d-0.0.2/toon3d/utils/camera_utils.py
--rw-r--r--   0 ethanweber (1000282) users    (1000001)    12545 2024-03-15 01:48:57.000000 toon3d-0.0.2/toon3d/utils/colmap_database.py
--rw-r--r--   0 ethanweber (1000282) users    (1000001)     1514 2024-03-15 01:48:57.000000 toon3d-0.0.2/toon3d/utils/convert_points.py
--rw-r--r--   0 ethanweber (1000282) users    (1000001)     3008 2024-03-15 01:48:57.000000 toon3d-0.0.2/toon3d/utils/depth_utils.py
--rw-r--r--   0 ethanweber (1000282) users    (1000001)     2699 2024-03-15 01:48:57.000000 toon3d-0.0.2/toon3d/utils/draw_utils.py
--rw-r--r--   0 ethanweber (1000282) users    (1000001)     4322 2024-05-10 21:50:37.000000 toon3d-0.0.2/toon3d/utils/image_processing_utils.py
--rw-r--r--   0 ethanweber (1000282) users    (1000001)     2108 2024-03-15 01:48:57.000000 toon3d-0.0.2/toon3d/utils/losses.py
--rw-r--r--   0 ethanweber (1000282) users    (1000001)     9203 2024-03-15 01:48:57.000000 toon3d-0.0.2/toon3d/utils/mesh_utils.py
--rw-r--r--   0 ethanweber (1000282) users    (1000001)     1767 2024-03-15 01:48:57.000000 toon3d-0.0.2/toon3d/utils/novel_view_samplers.py
-drwxr-xr-x   0 ethanweber (1000282) users    (1000001)        0 2024-05-13 05:32:20.454004 toon3d-0.0.2/toon3d/utils/pytorch_arap/
--rw-r--r--   0 ethanweber (1000282) users    (1000001)    23448 2024-03-15 01:48:57.000000 toon3d-0.0.2/toon3d/utils/pytorch_arap/arap.py
--rw-r--r--   0 ethanweber (1000282) users    (1000001)     8227 2024-03-15 01:48:57.000000 toon3d-0.0.2/toon3d/utils/pytorch_arap/arap_utils.py
--rw-r--r--   0 ethanweber (1000282) users    (1000001)     2675 2024-03-15 01:48:57.000000 toon3d-0.0.2/toon3d/utils/tsdf_utils.py
--rw-r--r--   0 ethanweber (1000282) users    (1000001)     3316 2024-03-26 21:11:46.000000 toon3d-0.0.2/toon3d/utils/viser_utils.py
-drwxr-xr-x   0 ethanweber (1000282) users    (1000001)        0 2024-05-13 05:32:20.454004 toon3d-0.0.2/toon3d/warp/
--rw-r--r--   0 ethanweber (1000282) users    (1000001)     3415 2024-04-12 21:13:30.000000 toon3d-0.0.2/toon3d/warp/arap_utils.py
--rw-r--r--   0 ethanweber (1000282) users    (1000001)     4744 2024-03-15 01:48:57.000000 toon3d-0.0.2/toon3d/warp/tri_rasterize.py
--rw-r--r--   0 ethanweber (1000282) users    (1000001)    10060 2024-04-12 21:13:30.000000 toon3d-0.0.2/toon3d/warp/warp_mesh.py
--rw-r--r--   0 ethanweber (1000282) users    (1000001)     7403 2024-03-15 01:48:57.000000 toon3d-0.0.2/toon3d/warp_model.py
-drwxr-xr-x   0 ethanweber (1000282) users    (1000001)        0 2024-05-13 05:32:20.450004 toon3d-0.0.2/toon3d-labeler/
-drwxr-xr-x   0 ethanweber (1000282) users    (1000001)        0 2024-05-13 05:32:20.450004 toon3d-0.0.2/toon3d-labeler/node_modules/
-drwxr-xr-x   0 ethanweber (1000282) users    (1000001)        0 2024-05-13 05:32:20.450004 toon3d-0.0.2/toon3d-labeler/node_modules/flatted/
-drwxr-xr-x   0 ethanweber (1000282) users    (1000001)        0 2024-05-13 05:32:20.450004 toon3d-0.0.2/toon3d-labeler/node_modules/flatted/python/
--rw-r--r--   0 ethanweber (1000282) users    (1000001)     3879 2024-04-30 22:25:05.000000 toon3d-0.0.2/toon3d-labeler/node_modules/flatted/python/flatted.py
--rw-r--r--   0 ethanweber (1000282) users    (1000001)     2129 2024-04-30 22:25:05.000000 toon3d-0.0.2/toon3d-labeler/node_modules/flatted/python/test.py
-drwxr-xr-x   0 ethanweber (1000282) users    (1000001)        0 2024-05-13 05:32:20.450004 toon3d-0.0.2/toon3d-spaces/
--rw-r--r--   0 ethanweber (1000282) users    (1000001)    10976 2024-05-13 05:21:40.000000 toon3d-0.0.2/toon3d-spaces/app.py
-drwxr-xr-x   0 ethanweber (1000282) users    (1000001)        0 2024-05-13 05:32:20.454004 toon3d-0.0.2/toon3d.egg-info/
--rw-r--r--   0 ethanweber (1000282) users    (1000001)      826 2024-05-13 05:32:19.000000 toon3d-0.0.2/toon3d.egg-info/PKG-INFO
--rw-r--r--   0 ethanweber (1000282) users    (1000001)     1369 2024-05-13 05:32:20.000000 toon3d-0.0.2/toon3d.egg-info/SOURCES.txt
--rw-r--r--   0 ethanweber (1000282) users    (1000001)        1 2024-05-13 05:32:19.000000 toon3d-0.0.2/toon3d.egg-info/dependency_links.txt
--rw-r--r--   0 ethanweber (1000282) users    (1000001)      393 2024-05-13 05:32:19.000000 toon3d-0.0.2/toon3d.egg-info/entry_points.txt
--rw-r--r--   0 ethanweber (1000282) users    (1000001)      280 2024-05-13 05:32:19.000000 toon3d-0.0.2/toon3d.egg-info/requires.txt
--rw-r--r--   0 ethanweber (1000282) users    (1000001)       56 2024-05-13 05:32:19.000000 toon3d-0.0.2/toon3d.egg-info/top_level.txt
+drwxr-xr-x   0 ethanweber (1000282) users    (1000001)        0 2024-05-16 20:20:55.791628 toon3d-0.0.3/
+-rw-r--r--   0 ethanweber (1000282) users    (1000001)      906 2024-05-16 20:20:55.791628 toon3d-0.0.3/PKG-INFO
+-rw-r--r--   0 ethanweber (1000282) users    (1000001)     5271 2024-05-16 20:18:19.000000 toon3d-0.0.3/README.md
+-rw-r--r--   0 ethanweber (1000282) users    (1000001)     1296 2024-05-16 20:19:43.000000 toon3d-0.0.3/pyproject.toml
+-rw-r--r--   0 ethanweber (1000282) users    (1000001)       38 2024-05-16 20:20:55.791628 toon3d-0.0.3/setup.cfg
+drwxr-xr-x   0 ethanweber (1000282) users    (1000001)        0 2024-05-16 20:20:55.787628 toon3d-0.0.3/toon3d/
+-rw-r--r--   0 ethanweber (1000282) users    (1000001)        0 2024-03-15 01:48:57.000000 toon3d-0.0.3/toon3d/__init__.py
+-rw-r--r--   0 ethanweber (1000282) users    (1000001)     1728 2024-03-15 01:48:57.000000 toon3d-0.0.3/toon3d/color_palette.py
+drwxr-xr-x   0 ethanweber (1000282) users    (1000001)        0 2024-05-16 20:20:55.787628 toon3d-0.0.3/toon3d/configs/
+-rw-r--r--   0 ethanweber (1000282) users    (1000001)     1475 2024-03-15 01:48:57.000000 toon3d-0.0.3/toon3d/configs/prompts.py
+drwxr-xr-x   0 ethanweber (1000282) users    (1000001)        0 2024-05-16 20:20:55.787628 toon3d-0.0.3/toon3d/generative/
+-rw-r--r--   0 ethanweber (1000282) users    (1000001)    10358 2024-03-15 01:48:57.000000 toon3d-0.0.3/toon3d/generative/marigold.py
+drwxr-xr-x   0 ethanweber (1000282) users    (1000001)        0 2024-05-16 20:20:55.787628 toon3d-0.0.3/toon3d/scripts/
+-rw-r--r--   0 ethanweber (1000282) users    (1000001)     4646 2024-05-10 20:12:48.000000 toon3d-0.0.3/toon3d/scripts/colmap_with_corrs.py
+-rw-r--r--   0 ethanweber (1000282) users    (1000001)     6596 2024-05-16 05:41:22.000000 toon3d-0.0.3/toon3d/scripts/download_data.py
+-rw-r--r--   0 ethanweber (1000282) users    (1000001)     8611 2024-05-10 21:53:19.000000 toon3d-0.0.3/toon3d/scripts/process_data.py
+-rw-r--r--   0 ethanweber (1000282) users    (1000001)    34579 2024-05-16 20:19:04.000000 toon3d-0.0.3/toon3d/scripts/run.py
+-rw-r--r--   0 ethanweber (1000282) users    (1000001)     1185 2024-03-15 01:48:57.000000 toon3d-0.0.3/toon3d/scripts/server.py
+-rw-r--r--   0 ethanweber (1000282) users    (1000001)     4685 2024-05-13 05:11:25.000000 toon3d-0.0.3/toon3d/scripts/viser_vis.py
+-rw-r--r--   0 ethanweber (1000282) users    (1000001)     2847 2024-03-15 01:48:57.000000 toon3d-0.0.3/toon3d/toon3d_config.py
+-rw-r--r--   0 ethanweber (1000282) users    (1000001)     5939 2024-03-15 01:48:57.000000 toon3d-0.0.3/toon3d/toon3d_datamanager.py
+-rw-r--r--   0 ethanweber (1000282) users    (1000001)     1492 2024-05-16 20:15:55.000000 toon3d-0.0.3/toon3d/toon3d_dataparser.py
+-rw-r--r--   0 ethanweber (1000282) users    (1000001)    12830 2024-05-16 20:15:55.000000 toon3d-0.0.3/toon3d/toon3d_model.py
+-rw-r--r--   0 ethanweber (1000282) users    (1000001)     3495 2024-05-16 20:15:55.000000 toon3d-0.0.3/toon3d/toon3d_pipeline.py
+drwxr-xr-x   0 ethanweber (1000282) users    (1000001)        0 2024-05-16 20:20:55.791628 toon3d-0.0.3/toon3d/utils/
+-rw-r--r--   0 ethanweber (1000282) users    (1000001)     3376 2024-03-15 01:48:57.000000 toon3d-0.0.3/toon3d/utils/camera_utils.py
+-rw-r--r--   0 ethanweber (1000282) users    (1000001)    12545 2024-03-15 01:48:57.000000 toon3d-0.0.3/toon3d/utils/colmap_database.py
+-rw-r--r--   0 ethanweber (1000282) users    (1000001)     1514 2024-03-15 01:48:57.000000 toon3d-0.0.3/toon3d/utils/convert_points.py
+-rw-r--r--   0 ethanweber (1000282) users    (1000001)     3008 2024-03-15 01:48:57.000000 toon3d-0.0.3/toon3d/utils/depth_utils.py
+-rw-r--r--   0 ethanweber (1000282) users    (1000001)     2699 2024-03-15 01:48:57.000000 toon3d-0.0.3/toon3d/utils/draw_utils.py
+-rw-r--r--   0 ethanweber (1000282) users    (1000001)     4322 2024-05-10 21:50:37.000000 toon3d-0.0.3/toon3d/utils/image_processing_utils.py
+-rw-r--r--   0 ethanweber (1000282) users    (1000001)     2108 2024-03-15 01:48:57.000000 toon3d-0.0.3/toon3d/utils/losses.py
+-rw-r--r--   0 ethanweber (1000282) users    (1000001)     1767 2024-03-15 01:48:57.000000 toon3d-0.0.3/toon3d/utils/novel_view_samplers.py
+-rw-r--r--   0 ethanweber (1000282) users    (1000001)     2675 2024-03-15 01:48:57.000000 toon3d-0.0.3/toon3d/utils/tsdf_utils.py
+-rw-r--r--   0 ethanweber (1000282) users    (1000001)     3316 2024-03-26 21:11:46.000000 toon3d-0.0.3/toon3d/utils/viser_utils.py
+drwxr-xr-x   0 ethanweber (1000282) users    (1000001)        0 2024-05-16 20:20:55.791628 toon3d-0.0.3/toon3d/warp/
+-rw-r--r--   0 ethanweber (1000282) users    (1000001)     3415 2024-04-12 21:13:30.000000 toon3d-0.0.3/toon3d/warp/arap_utils.py
+-rw-r--r--   0 ethanweber (1000282) users    (1000001)    11952 2024-05-16 20:15:55.000000 toon3d-0.0.3/toon3d/warp/warp_mesh.py
+drwxr-xr-x   0 ethanweber (1000282) users    (1000001)        0 2024-05-16 20:20:55.783628 toon3d-0.0.3/toon3d-labeler/
+drwxr-xr-x   0 ethanweber (1000282) users    (1000001)        0 2024-05-16 20:20:55.783628 toon3d-0.0.3/toon3d-labeler/node_modules/
+drwxr-xr-x   0 ethanweber (1000282) users    (1000001)        0 2024-05-16 20:20:55.783628 toon3d-0.0.3/toon3d-labeler/node_modules/flatted/
+drwxr-xr-x   0 ethanweber (1000282) users    (1000001)        0 2024-05-16 20:20:55.787628 toon3d-0.0.3/toon3d-labeler/node_modules/flatted/python/
+-rw-r--r--   0 ethanweber (1000282) users    (1000001)     3879 2024-04-30 22:25:05.000000 toon3d-0.0.3/toon3d-labeler/node_modules/flatted/python/flatted.py
+-rw-r--r--   0 ethanweber (1000282) users    (1000001)     2129 2024-04-30 22:25:05.000000 toon3d-0.0.3/toon3d-labeler/node_modules/flatted/python/test.py
+drwxr-xr-x   0 ethanweber (1000282) users    (1000001)        0 2024-05-16 20:20:55.787628 toon3d-0.0.3/toon3d-spaces/
+-rw-r--r--   0 ethanweber (1000282) users    (1000001)    11016 2024-05-13 22:54:51.000000 toon3d-0.0.3/toon3d-spaces/app.py
+drwxr-xr-x   0 ethanweber (1000282) users    (1000001)        0 2024-05-16 20:20:55.791628 toon3d-0.0.3/toon3d.egg-info/
+-rw-r--r--   0 ethanweber (1000282) users    (1000001)      906 2024-05-16 20:20:55.000000 toon3d-0.0.3/toon3d.egg-info/PKG-INFO
+-rw-r--r--   0 ethanweber (1000282) users    (1000001)     1086 2024-05-16 20:20:55.000000 toon3d-0.0.3/toon3d.egg-info/SOURCES.txt
+-rw-r--r--   0 ethanweber (1000282) users    (1000001)        1 2024-05-16 20:20:55.000000 toon3d-0.0.3/toon3d.egg-info/dependency_links.txt
+-rw-r--r--   0 ethanweber (1000282) users    (1000001)      393 2024-05-16 20:20:55.000000 toon3d-0.0.3/toon3d.egg-info/entry_points.txt
+-rw-r--r--   0 ethanweber (1000282) users    (1000001)      315 2024-05-16 20:20:55.000000 toon3d-0.0.3/toon3d.egg-info/requires.txt
+-rw-r--r--   0 ethanweber (1000282) users    (1000001)       56 2024-05-16 20:20:55.000000 toon3d-0.0.3/toon3d.egg-info/top_level.txt
```

### Comparing `toon3d-0.0.2/PKG-INFO` & `toon3d-0.0.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: toon3d
-Version: 0.0.2
+Version: 0.0.3
 Summary: toon3d package
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python
 Requires-Python: >=3.7.3
 Requires-Dist: black
 Requires-Dist: h5py
 Requires-Dist: mediapy
@@ -25,7 +25,10 @@
 Requires-Dist: matplotlib
 Requires-Dist: onnxruntime
 Requires-Dist: onnx
 Requires-Dist: gdown==5.0.0
 Requires-Dist: diffusers>=0.25.1
 Requires-Dist: wandb>=0.16.2
 Requires-Dist: peft>=0.6.0
+Requires-Dist: viser
+Requires-Dist: jaxtyping>=0.2.15
+Requires-Dist: nerfstudio
```

### Comparing `toon3d-0.0.2/README.md` & `toon3d-0.0.3/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,85 +1,45 @@
 # Toon3D
 
-This project enables 3D reconstruction of non-geometrically consistent scenes, such as cartoons. _We take a few images from a cartoon and reconstruct it in 3D._
+<i>Humans can perceive 3D world from images that aren't 3D consistent, but why can't machines?</i> This project enables 3D reconstruction of non-geometrically consistent scenes, such as cartoons. _We take a few images from a cartoon and reconstruct it in 3D. Our project page is at [https://toon3d.studio/](https://toon3d.studio/).
 
 |   Image 1   |   Image 2   |   Image 3   |
 | :------------------------: | :--------------------------: | :-------------------------: |
 | ![](toon3d/assets/randm_left.jpeg) | ![](toon3d/assets/randm_center.jpeg) | ![](toon3d/assets/randm_right.jpeg) |
 
 # Setting up the environment
 
-Create a conda environment. 
-
-1. Install the latest nerfstudio package.
-
-2. Then install this codebase as a pip package.
+Create a conda environment and install Toon3D.
 
 ```bash
 pip install -e .
 ```
 
-3. Install the `pytorch3d` package.
-
-```bash
-pip install git+https://github.com/facebookresearch/pytorch3d.git
-```
-
-4. Optionally, install `torch-batch-svd`:
+# Download Toon3D Dataset scenes
 
-```bash
-pip install git+https://github.com/KinglittleQ/torch-batch-svd.git
-```
-
-# Download pre-processed datasets
-
-To download all our [pre-processed datasets from Google Drive](TODO), run
-
-```bash
-tnd-download-data dataset --dataset all
-```
+Download the Toon3D Dataset from [here](https://huggingface.co/datasets/ethanweber/toon3d-dataset) and place the dataset folders in `data/processed`.
 
 # Running the full SfM pipeline (optional, for custom data)
 
 This section walks you through starting from a small collection of images, annotating them, and running our custom SfM to create the initial dataset. This is how we created the pre-processed datasets, available above.
 
-## Download images
-
-To download one of our [image collections from Google Drive](https://drive.google.com/drive/folders/11ogFtOOBB-UIq6seMukYncqqFacxBn5-?usp=drive_link) run
-
-```bash
-tnd-download-data images --dataset [dataset]
-```
-
-For example,
-
-```bash
-tnd-download-data images --dataset bobs-burgers-dining
-```
+## Obtain images
 
-If this fails, that means the `name <=> link` association is not set at the top of the file [toon3d/scripts/download_data.py](toon3d/scripts/download_data.py). Feel free to file and issue or make a PR. Or, make sure a Google Drive folder is set to public and copy it's link.
+You can download one of our image collections from [this Google Drive link](https://drive.google.com/drive/folders/11ogFtOOBB-UIq6seMukYncqqFacxBn5-?usp=drive_link) or simply use your own. Place the images in a folder such as `data/images/[dataset]`, where [dataset] is the dataset name. To get started, download the `bobs-burgers-dining` images and follow the instructions below.
 
-Then do
+## Process Data
 
-```bash
-tnd-download-data images --dataset [dataset] --link [link]
-```
+This step runs depth estimation and Segment Anything (SAM).
 
-For example,
+Install with 
 
 ```bash
-tnd-download-data images --dataset bobs-burgers-dining --link https://drive.google.com/drive/folders/1eicpYlQRUMuCbWfBG5SZev_4Y8FKHMKS?usp=drive_link
+pip install segment_anything @ git+https://github.com/facebookresearch/segment-anything.git
 ```
 
-and the directory will be downloaded to `data/images/[dataset]`
-
-## Process Data
-
-This step runs depth estimation and Segment Anything (SAM).
-
 Download [SAM](https://github.com/facebookresearch/segment-anything) weights with `tnd-download-data sam`.
 
 Now, you can run
 
 ```bash
 tnd-process-data initialize --dataset [dataset] --input_path [input_path]
 ```
```

### Comparing `toon3d-0.0.2/pyproject.toml` & `toon3d-0.0.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "toon3d"
-version = "0.0.2"
+version = "0.0.3"
 description = "toon3d package"
 requires-python = ">=3.7.3"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Programming Language :: Python",
 ]
 dependencies = [
@@ -31,15 +31,18 @@
     "pycocotools", 
     "matplotlib", 
     "onnxruntime", 
     "onnx",
     "gdown==5.0.0",
     "diffusers>=0.25.1",
     "wandb>=0.16.2",
-    "peft>=0.6.0"
+    "peft>=0.6.0",
+    "viser",
+    "jaxtyping>=0.2.15",
+    "nerfstudio"
 ]
 
 [tool.setuptools.packages.find]
 include = ["toon3d*"]
 
 [project.entry-points.'nerfstudio.method_configs']
 toon3d = "toon3d.toon3d_config:toon3d_config"
```

### Comparing `toon3d-0.0.2/toon3d/color_palette.py` & `toon3d-0.0.3/toon3d/color_palette.py`

 * *Files identical despite different names*

### Comparing `toon3d-0.0.2/toon3d/configs/prompts.py` & `toon3d-0.0.3/toon3d/configs/prompts.py`

 * *Files identical despite different names*

### Comparing `toon3d-0.0.2/toon3d/generative/marigold.py` & `toon3d-0.0.3/toon3d/generative/marigold.py`

 * *Files identical despite different names*

### Comparing `toon3d-0.0.2/toon3d/scripts/colmap_with_corrs.py` & `toon3d-0.0.3/toon3d/scripts/colmap_with_corrs.py`

 * *Files identical despite different names*

### Comparing `toon3d-0.0.2/toon3d/scripts/download_data.py` & `toon3d-0.0.3/toon3d/scripts/download_data.py`

 * *Files identical despite different names*

### Comparing `toon3d-0.0.2/toon3d/scripts/process_data.py` & `toon3d-0.0.3/toon3d/scripts/process_data.py`

 * *Files identical despite different names*

### Comparing `toon3d-0.0.2/toon3d/scripts/run.py` & `toon3d-0.0.3/toon3d/scripts/run.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,30 +7,29 @@
 from datetime import datetime
 import io
 
 import cv2 
 import kornia
 import mediapy
 import numpy as np
-import plotly.graph_objects as go
 import torch
 import torch.nn as nn
 from tqdm import tqdm
 import shutil
 import cv2
 
 import tyro
 import viser
 from toon3d.utils.draw_utils import get_images_with_keypoints
 from toon3d.utils.viser_utils import view_pcs_cameras
 from toon3d.utils.camera_utils import Cameras
 from toon3d.warp.warp_mesh import WarpMesh, draw_tris, draw_points, FrameMeshes, get_simplices
 from toon3d.warp.arap_utils import face_verts_arap_loss, calc_area_loss, signed_areas
 from toon3d.utils.depth_utils import create_discontinuity_mask
-from toon3d.utils.mesh_utils import get_mesh, save_mesh
+
 
 from nerfstudio.utils.colormaps import apply_depth_colormap
 from nerfstudio.utils.rich_utils import CONSOLE
 
 
 def make_transforms_json(fxs, fys, Rs, ts, widths, heights):
     fxs, fys, Rs, ts = fxs.detach().cpu(), fys.detach().cpu(), Rs.detach().cpu(), ts.detach().cpu()
@@ -86,40 +85,14 @@
         y = grid_y[::factor, ::factor].flatten()
         z = depth_map[::factor, ::factor].T.flatten()
 
         dense_points_3d.append(cameras(x, y, z)[ndx])
 
     return dense_points_3d
 
-def make_dense_points_3d_no_flatten(cameras, depths, factor=1):
-    dense_points_3d = []
-
-    for ndx, depth_map in enumerate(depths): 
-        height, width = depth_map.shape
-        xs = torch.arange(width).to(depth_map.device)
-        ys = torch.arange(height).to(depth_map.device)
-        grid_x, grid_y = torch.meshgrid(xs, ys, indexing="ij")
-
-        grid_x = (grid_x / (width - 1) * 2) - 1
-        grid_y = (grid_y / (height - 1) * 2) - 1
-
-        x = grid_x
-        y = grid_y
-        z = depth_map.T
-
-        shape = x.shape
-
-        points = cameras(x.flatten(), y.flatten(), z.flatten())[ndx]
-        points = points.reshape(shape + (3,))
-
-        dense_points_3d.append(points)
-
-    return dense_points_3d
-
-
 def make_plys(images_colors, points_3d):
     n = len(images_colors)
     plys = []
     for i in range(n):
         image_colors = images_colors[i]
         ply_points = points_3d[i]
 
@@ -141,19 +114,19 @@
             ply.write(f"{x:8f} {y:8f} {z:8f} {r} {g} {b}\n")
 
         plys.append(ply.getvalue())
         ply.close()
 
     return plys
 
-def load_dataset(data_prefix, dataset, device="cpu", dilate_mask_iters=4, dilate_lines_thresh=0.05, dilate_lines_iters=3, min_valid_points=3):
-    images_path = data_prefix / f"{dataset}/images"
-    metadata_path = data_prefix / f"{dataset}/metadata.json"
-    points_path = data_prefix / f"{dataset}/points.json"
-    depths_path = data_prefix / f"{dataset}/depths"
+def load_dataset(data_path, device="cpu", dilate_mask_iters=4, dilate_lines_thresh=0.05, dilate_lines_iters=3, min_valid_points=3):
+    images_path = data_path / "images"
+    metadata_path = data_path / "metadata.json"
+    points_path = data_path / "points.json"
+    depths_path = data_path / "depths"
 
     metadata_json = json.loads(metadata_path.read_text())
 
     points_json = json.loads(points_path.read_text())
     valid_images = points_json["validImages"]
     points_list = [[[p["x"], p["y"]] for p in points] for points in points_json["points"]]
     valid_points_list = points_json["validPoints"]
@@ -226,64 +199,63 @@
     return images, heights, widths, points, points_normed, points_mask, depths, masks
 
 
 def main(
     data_prefix: Path = Path("data/processed"),
     dataset: str = "rick-house",
     device: str = "cpu",
-    niters: int = 5000,
+    niters: int = 2000,
     lr: float = 0.01,
     affine_loss_mult: float = 1000.0,
     scale_loss_mult: float = 1e3,
     scale_loss_target: float = 1.0,
     offset_loss_mult: float = 1e3,
     focal_mag_mult: float = 1e-3,
     aspect_mult: float = 1,
     up_mult: float = 0,
-    niters_warp: int = 2000,
+    niters_warp: int = 1000,
     lr_warp: float = 0.01,
-    arap_mult: float = 1e3, 
-    zs_diff_mult: float = 0.0,
+    arap_mult: float = 1, 
+    zs_diff_mult: float = 1,
     output_prefix: Path = Path("outputs"),
     output_method: Path = Path("run"),
     nerfstudio_folder: Path = Path("data/nerfstudio"),
     ply_downscale_factor: int = 4,
     view_point_cloud: bool = True,
     make_video: bool = False,
-    coarse_camera_params: torch.Tensor = None,
-    dzs: torch.Tensor = None,
-    szs: torch.Tensor = None,
     save_geometry: bool = True,
     write_to_nerfstudio: bool = True,
     mask_random_points: int = 0,
-    port: int = 8080,
+    port: int = 7007,
+    seed: int = None,
 ):
     """Script to run our SfM on cartoons."""
 
     output_folder = output_prefix / dataset / output_method / datetime.now().strftime("%Y-%m-%d_%H%M%S")
     output_folder.mkdir(parents=True)
 
-    images, heights, widths, points, points_normed, points_mask, depths, masks = load_dataset(data_prefix, dataset, device)
+    images, heights, widths, points, points_normed, points_mask, depths, masks = load_dataset(data_prefix / dataset, device)
     n, m = points.shape[:2]
+
+    # for ablations
+    if seed is not None:
+        torch.manual_seed(seed)
     
     # for hold-out evaluation
-    original_points_mask = points_mask.clone()
     mask_random_points_indices = None
     if mask_random_points > 0:
         # set a seed
         torch.manual_seed(0)
         mask_random_points_indices = torch.randperm(m)[:mask_random_points]
         points_mask[:, mask_random_points_indices] = False
 
+    # offset relative depths
     depth_offset = 0.2
     depths = [depths[i] + depth_offset for i in range(n)]
 
-    # set all depths to depth_offset
-    depths = [torch.ones_like(depth) for depth in depths]
-
     # draw keypoints on image
     point_colors = torch.rand((m, 3)).to(device)
     colors = point_colors[None].repeat(n, 1, 1)
     colors[~points_mask] = torch.tensor([1, 1, 1]).float().to(device)
     output_images_dir = Path(output_folder / "images")
     output_images_dir.mkdir(parents=True)
     for i in range(n):
@@ -296,16 +268,16 @@
     # make borders
     border_masks = []
     for ndx in range(n):
         pts = points[ndx][points_mask[ndx]]
         spls = get_simplices(pts)
 
         mask_mesh = WarpMesh(pts, spls, heights[ndx], widths[ndx], pts, device=device)
-        border_mask = (mask_mesh.rasterize().pix_to_face[0,...,0] > -1) * 1.0
-        border_mask = border_mask.cpu().numpy()
+        border_mask = mask_mesh.apply_warp(torch.zeros(heights[ndx], widths[ndx], 1))[..., 0]
+        border_mask = 1 - border_mask.cpu().numpy()
 
         masks[ndx] = masks[ndx] * border_mask
         border_masks.append(border_mask)
 
     ########################################
     ###### coarse camera optimization ######
     ########################################
@@ -333,52 +305,49 @@
     dzs = nn.Parameter(torch.zeros([n]).float().to(device)) # delta zs
     szs = nn.Parameter(torch.ones([n]).float().to(device)) # scale zs
 
     # make cameras and optimizer
     coarse_cameras = Cameras(n).to(device)
 
     # load cameras if exist
-    if coarse_camera_params is not None:
-        coarse_cameras.load_state_dict(coarse_camera_params)
-    else:
-        optimizer = torch.optim.Adam(list(coarse_cameras.parameters()) + [szs, dzs], lr=lr)
+    optimizer = torch.optim.Adam(list(coarse_cameras.parameters()) + [szs, dzs], lr=lr)
+
+    # optimization loop
+    pbar = tqdm(range(niters))
 
-        # optimization loop
-        pbar = tqdm(range(niters))
+    for i in pbar:
 
-        for i in pbar:
+        new_zs = zs * szs[...,None] + dzs[...,None]
+        points_3d = coarse_cameras(us_normed, vs_normed, new_zs)
+        paired_points = points_3d[pairs]
+        affine_loss = affine_loss_mult * torch.mean(((paired_points[0] - paired_points[1]) ** 2) * pairs_mask)
 
-            new_zs = zs * szs[...,None] + dzs[...,None]
-            points_3d = coarse_cameras(us_normed, vs_normed, new_zs)
-            paired_points = points_3d[pairs]
-            affine_loss = affine_loss_mult * torch.mean(((paired_points[0] - paired_points[1]) ** 2) * pairs_mask)
-
-            scale_loss = scale_loss_mult * ((torch.mean(szs) - scale_loss_target) ** 2 + torch.mean(torch.relu(-szs) ** 2))
-            offset_loss = offset_loss_mult * torch.mean(torch.relu(-dzs) ** 2)
-            focal_mag = focal_mag_mult * (torch.mean(coarse_cameras.fxs) + torch.mean(coarse_cameras.fys))
-            focal_fix = aspect_mult * torch.mean((coarse_cameras.fys / coarse_cameras.fxs - widths / heights) ** 2)
-            up_loss = up_mult * torch.mean((torch.abs((coarse_cameras.Rs @ torch.tensor([0, 1, 0]).float().to(device))[:,1] - 1)))
-            loss = affine_loss + scale_loss + offset_loss + focal_mag + focal_fix + up_loss
-
-            optimizer.zero_grad()
-            loss.backward()
-            optimizer.step()
-
-            # keep first point cloud fixed
-            with torch.no_grad():
-                coarse_cameras.quats[0] = torch.tensor([1, 0, 0, 0])
-                coarse_cameras.ts[0] = torch.zeros([3])
-
-                pbar.set_description(f"Loss: {loss:.2e}, 3D: {affine_loss:.2e}", refresh=True)
-
-                # unbounded scale and offset
-                if scale_loss_mult == 0:
-                    szs[:] = 1
-                if offset_loss_mult == 0:
-                    dzs[:] = 0
+        scale_loss = scale_loss_mult * ((torch.mean(szs) - scale_loss_target) ** 2 + torch.mean(torch.relu(-szs) ** 2))
+        offset_loss = offset_loss_mult * torch.mean(torch.relu(-dzs) ** 2)
+        focal_mag = focal_mag_mult * (torch.mean(coarse_cameras.fxs) + torch.mean(coarse_cameras.fys))
+        focal_fix = aspect_mult * torch.mean((coarse_cameras.fys / coarse_cameras.fxs - widths / heights) ** 2)
+        up_loss = up_mult * torch.mean((torch.abs((coarse_cameras.Rs @ torch.tensor([0, 1, 0]).float().to(device))[:,1] - 1)))
+        loss = affine_loss + scale_loss + offset_loss + focal_mag + focal_fix + up_loss
+
+        optimizer.zero_grad()
+        loss.backward()
+        optimizer.step()
+
+        # keep first point cloud fixed
+        with torch.no_grad():
+            coarse_cameras.quats[0] = torch.tensor([1, 0, 0, 0])
+            coarse_cameras.ts[0] = torch.zeros([3])
+
+            pbar.set_description(f"Loss: {loss:.2e}, 3D: {affine_loss:.2e}", refresh=True)
+
+            # unbounded scale and offset
+            if scale_loss_mult == 0:
+                szs[:] = 1
+            if offset_loss_mult == 0:
+                dzs[:] = 0
 
     # make new cameras
     refined_cameras = Cameras(n, 
                             coarse_cameras.fxs.detach().clone(), 
                             coarse_cameras.fys.detach().clone(), 
                             coarse_cameras.quats.detach().clone(), 
                             coarse_cameras.ts.detach().clone()).to(device)
@@ -386,30 +355,29 @@
     new_zs = zs * szs[...,None] + dzs[...,None]
 
     ################################
     ###### make triangulation ######
     ################################
     CONSOLE.print("[bold green] Image triangulation")
 
-    frame_meshes = FrameMeshes(points, points_mask, depths, heights, widths)
+    frame_meshes = FrameMeshes(points, points_mask, depths)
 
     # face verts for ARAP
     face_verts_packed = frame_meshes.points_packed[frame_meshes.simplices_packed].mT
 
     ###################################
     ###### epipolar optimization ######
     ###################################
     CONSOLE.print("[bold green] Image Warping")
 
     dzs_warp = nn.Parameter(dzs.detach().clone()) # delta zs
     szs_warp = nn.Parameter(szs.detach().clone()) # scale zs
 
     # set up optimizer
     optimizer = torch.optim.Adam(list(frame_meshes.parameters()) + list(refined_cameras.parameters()) + [szs_warp, dzs_warp], lr=lr_warp)
-    # optimizer = torch.optim.Adam(frame_meshes.parameters(), lr=lr_warp)
     video_warped_mesh_points = [[] for _ in range(n)]
 
     # optimization loop
     pbar = tqdm(range(niters_warp))
 
     tri_areas = signed_areas(face_verts_packed)
 
@@ -509,28 +477,26 @@
 
     CONSOLE.print("[bold green] Rendering Images")
 
     for ndx in range(len(all_meshes)):
         mesh = all_meshes[ndx]
         image = images[ndx]
         depth_map = depths[ndx]
+        delta_zs = frame_meshes.delta_zs_list[ndx]
         mask = torch.from_numpy(masks[ndx]).float()
 
-        mesh.pzs = frame_meshes.delta_zs_list[ndx]
-
-        fragments = mesh.rasterize()
-        warped_pdepth = (fragments.zbuf[0,...,0] - mesh.z_offset)
-        warped_image = mesh.render(image, fragments).cpu().detach()
-        warped_depth = mesh.render(depth_map, fragments)
+        warped_image = mesh.apply_warp(image).cpu().detach()
+        warped_depth_uv = mesh.apply_warp(depth_map[...,None]).cpu().detach()[...,0]
+        warped_depth_z = mesh.vertex_coloring(delta_zs).cpu().detach()
+        warped_mask = mesh.apply_warp(mask[...,None]).cpu().detach()[...,0]
 
-        warped_mask = mesh.render(mask, fragments)
+        warped_depth = warped_depth_uv + warped_depth_z
+        warped_mask = warped_mask.to(torch.uint8).numpy()
         warped_mask[warped_mask < 100] = 0
-
-        warped_depth = warped_depth.cpu().detach()[...,0] + warped_pdepth.cpu().detach()
-        warped_mask = warped_mask.cpu().detach()[...,0].to(torch.uint8).numpy()
+        warped_mask[warped_mask >= 100] = 255
 
         wire_img = draw_tris(mesh, image = warped_image.numpy())
         points_img = draw_points(mesh, image=wire_img, points=frame_meshes.warped_corr_points_list[ndx], colors=point_colors[points_mask[ndx]].tolist())
 
         border_mask = border_masks[ndx]
         image[border_mask == 0] = 1
         warp_transition = ((warped_image * 0.5) + (image * 0.5)).numpy()
@@ -552,15 +518,15 @@
 
         # save warps to outputs
         mediapy.write_image(output_warped_images_dir / f"{ndx:02d}.png", warped_image.numpy())
         mediapy.write_image(output_warped_images_dir / f"wire_{ndx:02d}.png", points_img)
         mediapy.write_image(output_warped_images_dir / f"duo_{ndx:02d}.png", np.concatenate([warped_image.numpy(), points_img], axis=1))
 
         mediapy.write_image(output_warped_depths_dir / f"{ndx:02d}.png", warped_depth)
-        mediapy.write_image(output_warped_depths_dir / f"pdepth_{ndx:02d}.png", warped_pdepth.cpu().detach().numpy())
+        mediapy.write_image(output_warped_depths_dir / f"zdepth_{ndx:02d}.png", warped_depth_z.numpy())
         mediapy.write_image(output_warped_masks_dir / f"{ndx:02d}.png", warped_mask)
 
         warped_images.append(warped_image)
         warped_depths.append(warped_depth)
         warped_masks.append(warped_mask)
 
     if make_video:
@@ -576,15 +542,15 @@
 
             mesh = WarpMesh(warped_mesh_points, simplices, heights[ndx], widths[ndx], uv_points, device=device)
 
             for warped_mesh_points in warped_mesh_points_frames:
                 mesh.points = warped_mesh_points.to(mesh.device).float()
                 image = images[ndx]
 
-                warped_image = mesh.render(image).cpu().detach()
+                warped_image = mesh.apply_warp(image).cpu().detach()
                 wire_img = draw_tris(mesh, image = warped_image.numpy())
                 points_img = draw_points(mesh, image=wire_img, points=warped_mesh_points[:frame_meshes.num_corrs_per_mesh[ndx]], colors=point_colors[points_mask[ndx]].tolist())
                 video_frames.append(np.concatenate([warped_image.numpy(), points_img], axis=1))
 
             mediapy.write_video(output_warped_images_dir / f"{ndx:02d}.mp4", video_frames)
 
 
@@ -746,18 +712,18 @@
     
     torch.save(coarse_dense_points_3d, output_dense_points_dir / "dense_points.pt")
     torch.save(warped_dense_points_3d, output_dense_points_dir / "warped_dense_points.pt")
 
     torch.save(images_colors, output_img_colors_dir / "img_colors.pt")
     torch.save(warped_images_colors, output_img_colors_dir / "warped_img_colors.pt")
 
+    #############################
+    ###### compute metrics ######
+    #############################
     if mask_random_points_indices is not None:
-        # #############################
-        # ###### compute metrics ######
-        # #############################
         with torch.no_grad():
             warped_us = frame_meshes.warped_corr_points_padded[...,0]
             warped_vs = frame_meshes.warped_corr_points_padded[...,1]
 
             warped_us_normed = warped_us / (widths[..., None] - 1) * 2 - 1
             warped_vs_normed = warped_vs / (heights[..., None] - 1) * 2 - 1
             warped_zs = frame_meshes.warped_corr_zs_padded * szs_warp[...,None] + dzs_warp[...,None]
@@ -769,18 +735,15 @@
             with open(output_folder / "metrics.json", "w", encoding="utf-8") as f:
                 json.dump(metrics, f, indent=4)
         CONSOLE.print(f"[bold green] Metrics: {metrics}")
     else:
         metrics = None
 
 
-    if save_geometry:
-        # #######################
-        # ###### make plys ######
-        # #######################
+    if write_to_nerfstudio or save_geometry:
         CONSOLE.print("[bold green] Writing objs and plys")
 
         # create plys (point clouds)
         plys = make_plys(warped_images_colors, warped_dense_points_3d)
         for i, ply in enumerate(plys):
             with open(output_folder / "nerfstudio" / "plys" / f"{i:05d}.ply", "w") as f:
                 f.write(ply)
@@ -798,66 +761,40 @@
             f.write("property uint8 blue\n")
             f.write("end_header\n")
 
             for ply in plys:
                 for line in ply.splitlines()[14:]:
                     f.write(line + "\n")
 
-        # TODO: move a lot of this code to functions
-        # create objs (meshes, i.e., connected point clouds)
-        obj_colors = [image.permute(1, 0, 2).cpu() for image in images]
-        obj_points = make_dense_points_3d_no_flatten(refined_cameras, warped_depths)
-        obj_all_vertices = []
-        obj_all_vertex_colors = []
-        obj_all_faces = []
-        all_vertices_count = 0
-        for i in range(len(obj_points)):
-            temp_masks = torch.from_numpy(masks[i]).permute(1, 0)[None]
-            temp_images = obj_colors[i].permute(2, 0, 1)[None]
-            temp_vertices = obj_points[i].permute(2, 0, 1)[None].cpu()
-            temp_masks = temp_masks[..., ::ply_downscale_factor, ::ply_downscale_factor]
-            temp_images = temp_images[..., ::ply_downscale_factor, ::ply_downscale_factor]
-            temp_vertices = temp_vertices[..., ::ply_downscale_factor, ::ply_downscale_factor]
-            vertices, vertex_colors, faces, faces_mask = get_mesh(images=temp_images, vertices=temp_vertices, masks=temp_masks, distance_threshold=0.5)
-            faces = faces[faces_mask] # remove faces that are masked out
-            save_mesh(vertices, vertex_colors, faces, filename=str(output_folder / "nerfstudio" / "objs" / f"{i:05d}.obj"))
-            obj_all_vertices.append(vertices)
-            obj_all_vertex_colors.append(vertex_colors)
-            obj_all_faces.append(faces + all_vertices_count)
-            all_vertices_count += vertices.shape[0]
-        obj_all_vertices = torch.cat(obj_all_vertices)
-        obj_all_vertex_colors = torch.cat(obj_all_vertex_colors)
-        obj_all_faces = torch.cat(obj_all_faces)
-        save_mesh(obj_all_vertices, obj_all_vertex_colors, obj_all_faces, filename=str(output_folder / "nerfstudio" / "objs" / "all.obj"))
-
     if write_to_nerfstudio:
         # remove folder if exists
         if nerfstudio_folder:
             if (nerfstudio_folder / dataset).exists():
                 shutil.rmtree(nerfstudio_folder / dataset)
             shutil.copytree(output_folder / "nerfstudio", nerfstudio_folder / dataset)
 
     if view_point_cloud:
 
         sparse_point_colors = [point_colors[points_mask[ndx]] for ndx in range(n)]
         mesh_colors = [np.random.rand(3) for _ in range(n)]
         
         server = viser.ViserServer(request_share_url=True, port=port)
 
-        # view_pcs_cameras(server, 
-        #                  images, # cameras
-        #                  coarse_cameras,
-        #                  coarse_dense_points_3d, # dense pc
-        #                  images_colors, 
-        #                  coarse_corrs_3d, # sparse pc
-        #                  sparse_point_colors,
-        #                  mesh_verts_list, # mesh
-        #                  frame_meshes.simplices_list,
-        #                  mesh_colors,
-        #                  prefix="coarse")
+        view_pcs_cameras(server, 
+                         images, # cameras
+                         coarse_cameras,
+                         coarse_dense_points_3d, # dense pc
+                         images_colors, 
+                         coarse_corrs_3d, # sparse pc
+                         sparse_point_colors,
+                         mesh_verts_list, # mesh
+                         frame_meshes.simplices_list,
+                         mesh_colors,
+                         visible=False,
+                         prefix="coarse")
         
         view_pcs_cameras(server, 
                          warped_images, # cameras
                          refined_cameras,
                          warped_dense_points_3d, # dense pc
                          warped_images_colors, 
                          refined_corrs_3d, # sparse pc
```

### Comparing `toon3d-0.0.2/toon3d/scripts/server.py` & `toon3d-0.0.3/toon3d/scripts/server.py`

 * *Files identical despite different names*

### Comparing `toon3d-0.0.2/toon3d/scripts/viser_vis.py` & `toon3d-0.0.3/toon3d/scripts/viser_vis.py`

 * *Files identical despite different names*

### Comparing `toon3d-0.0.2/toon3d/toon3d_config.py` & `toon3d-0.0.3/toon3d/toon3d_config.py`

 * *Files identical despite different names*

### Comparing `toon3d-0.0.2/toon3d/toon3d_datamanager.py` & `toon3d-0.0.3/toon3d/toon3d_datamanager.py`

 * *Files identical despite different names*

### Comparing `toon3d-0.0.2/toon3d/toon3d_dataparser.py` & `toon3d-0.0.3/toon3d/toon3d_dataparser.py`

 * *Files 14% similar despite different names*

```diff
@@ -37,23 +37,8 @@
 class Toon3D(Nerfstudio):
     """Toon3D DatasetParser"""
 
     config: Toon3DDataParserConfig
 
     def _generate_dataparser_outputs(self, split="train"):
         dataparser_outputs = super()._generate_dataparser_outputs(split=split)
-
-        if self.config.data.suffix == ".json":
-            meta = load_from_json(self.config.data)
-            data_dir = self.config.data.parent
-        else:
-            meta = load_from_json(self.config.data / "transforms.json")
-            data_dir = self.config.data
-
-        # import pdb; pdb.set_trace();
-        dataparser_outputs.metadata["points"] = torch.load(data_dir / meta["points"])
-        dataparser_outputs.metadata["points_mask"] = torch.load(data_dir / meta["points_mask"])
-        dataparser_outputs.metadata["mesh_points"] = torch.load(data_dir / meta["meshes_points"])
-        dataparser_outputs.metadata["warped_mesh_points"] = torch.load(data_dir / meta["warped_meshes_points"])
-        dataparser_outputs.metadata["simplices"] = torch.load(data_dir / meta["simplices"])
-
         return dataparser_outputs
```

### Comparing `toon3d-0.0.2/toon3d/toon3d_model.py` & `toon3d-0.0.3/toon3d/toon3d_model.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,20 +4,19 @@
 
 from __future__ import annotations
 
 from dataclasses import dataclass, field
 from typing import Dict, List, Type
 import torch
 from torch.nn import Parameter
-from nerfstudio.models.splatfacto import SplatfactoModel, SplatfactoModelConfig, projection_matrix
+from nerfstudio.models.splatfacto import SplatfactoModel, SplatfactoModelConfig
 
 import torch
 from torch.nn import Parameter
 
-from toon3d.warp.warp_mesh import WarpMesh
 from toon3d.utils.losses import depth_ranking_loss
 
 import math
 from dataclasses import dataclass, field
 from typing import Dict, List, Optional, Tuple, Type, Union
 
 import numpy as np
@@ -42,34 +41,28 @@
 # need following import for background color override
 from nerfstudio.model_components import renderers
 from nerfstudio.model_components.losses import tv_loss
 from nerfstudio.models.base_model import Model, ModelConfig
 from nerfstudio.utils.rich_utils import CONSOLE
 from nerfstudio.utils.colormaps import apply_depth_colormap
 
-from toon3d.generative.ldm3d import LDM3D
 import mediapy
 from toon3d.configs.prompts import get_prompts
 from toon3d.utils.novel_view_samplers import sample_interpolated_camera
 from toon3d.utils.depth_utils import depth_to_disparity
-from pytorch3d.loss.chamfer import chamfer_distance
 from nerfstudio.viewer.viewer_elements import ViewerControl
 from nerfstudio.viewer.viewer import VISER_NERFSTUDIO_SCALE_RATIO
 
 
 @dataclass
 class Toon3DModelConfig(SplatfactoModelConfig):
     """Config for the toon3d model."""
 
     _target: Type = field(default_factory=lambda: Toon3DModel)
 
-    # warp parameters
-    warp_images: bool = False
-    """Warp input images"""
-
     # color palette parameters
     use_color_palette: bool = False
     """Whether to use the color palette for the toon3d model."""
     color_palette_project_before_render: bool = False
     """Whether to project nd dim with the color palette before rendering."""
     color_palette_use_as_colors: bool = False
     """Whether to use the color palette as the rgb output of the model."""
@@ -100,36 +93,16 @@
     depth_ranking_loss_num_patches: int = 8
     """Number of patches to sample for the depth ranking loss."""
     use_depth_loss: bool = False
     """Whether to use the depth loss."""
     depth_loss_mult: float = 1.0
     """Multiplier for the depth loss."""
 
-    # sds parameters
-    use_sds: bool = False
-    """Whether to use the sds loss."""
-    sds_mult: float = 1.0
-    """Multiplier for the sds loss."""
-    steps_per_sds: int = 10
-    """Number of steps per sds loss."""
-    sds_device: str = "cuda:1"
-    """device for sds diffusion model"""
-    sds_guidance_scale: float = 10.0
-    """Guidance scale for sds loss."""
-    sds_dataset: Optional[str] = None
-    """Dataset for sds model."""
-    sds_lora_weights_path: Optional[str] = None
-    """Path to the lora weights for sds model."""
-
-    use_chamfer_loss: bool = False
-    """Whether to use the chamfer loss."""
-    chamfer_loss_mult: float = 1.0
-    """Multiplier for the chamfer loss."""
-    chamfer_loss_num_points: int = 10000
-    """Number of points to use for the chamfer loss."""
+    steps_per_perturb: int = 10
+    """Number of steps per perturb for novel view."""
 
     use_isotropic_loss: bool = False
     """Whether to use the isotropic loss."""
     isotropic_ratio_mult: float = 1e6
     """Multiplier for the isotropic ratio loss."""
 
     use_ratio_loss: bool = True
@@ -144,23 +117,15 @@
 class Toon3DModel(SplatfactoModel):
     """Model for toon3d."""
 
     config: Toon3DModelConfig
 
     def __init__(self, *args, **kwargs):
         self.color_palette = kwargs["color_palette"]
-        self.images = kwargs["images"]
-        self.points = kwargs["points"]
-        self.points_mask = kwargs["points_mask"]
-        self.mesh_points = kwargs["mesh_points"]
-        self.warped_mesh_points = kwargs["warped_mesh_points"]
-        self.simplices_list = kwargs["simplices"]
         self.cameras = kwargs["cameras"]
-        self.points3D_xyz = kwargs["points3D_xyz"]
-        self.devic = kwargs["device"] # would be device but otherwise get a AttributeError: can't set attribute
         super().__init__(*args, **kwargs)
 
     def populate_modules(self):
         """Required for our custom models."""
 
         # modify the config for nd attributes
         if self.config.use_color_palette:
@@ -168,65 +133,27 @@
             if self.config.color_palette_use_as_colors:
                 self.config.nd_detach = False
             else:
                 self.config.nd_detach = True
 
         super().populate_modules()
 
-        # import pdb; pdb.set_trace();
-        self.iters = 0
-
-        # warping modules
-        if self.config.warp_images:
-            corr_points_list = self.mesh_points["corr_points"]
-            boundary_points_list = self.mesh_points["boundary_points"]
-            inner_points_list = self.mesh_points["inner_points"]
-
-            warped_corr_points_list = self.warped_mesh_points["corr_points"]
-            warped_boundary_points_list = self.warped_mesh_points["boundary_points"]
-            warped_inner_points_list = self.warped_mesh_points["inner_points"]
-
-            original_mesh_points_list = [torch.cat(wmp_triple) for wmp_triple in zip(corr_points_list, boundary_points_list, inner_points_list)]
-            warped_mesh_points_list = [torch.cat(wmp_triple) for wmp_triple in zip(warped_corr_points_list, warped_boundary_points_list, warped_inner_points_list)]
-
-            self.meshes = []
-
-            for ndx in range(len(self.images)):
-                image = self.images[ndx]
-                height, width = image.shape[:2]
-
-                uv_points = original_mesh_points_list[ndx]
-                warped_mesh_points = warped_mesh_points_list[ndx]
-                simplices = self.simplices_list[ndx]
-
-                mesh = WarpMesh(warped_mesh_points, simplices, height, width, uv_points, device=self.devic)
-
-                self.meshes.append(mesh)
-
         # we toggle this on and off
-        # when True, we perturb the camera and apply an SDS loss
+        # when True, we perturb the camera
         self.perturb_camera = False
-        if self.config.use_sds:
-            if not self.config.sds_dataset:
-                raise ValueError("--pipeline.model.sds_dataset must be provided when using SDS")
-            self.diffusion_model = LDM3D(
-                device=self.config.sds_device, lora_weights_path=self.config.sds_lora_weights_path
-            )
-            prompts, negative_prompts = get_prompts(self.config.sds_dataset)
-            self.text_embeddings = self.diffusion_model.get_text_embeds(prompts, negative_prompts)
 
     def get_training_callbacks(
         self, training_callback_attributes: TrainingCallbackAttributes
     ) -> List[TrainingCallback]:
         cbs = super().get_training_callbacks(training_callback_attributes)
 
-        if self.config.use_sds or self.config.use_tv_in_novel_views:
+        if self.config.use_tv_in_novel_views:
 
             def toggle_perturb(step, **kwargs):
-                if step != 0 and step % self.config.steps_per_sds == 0:
+                if step != 0 and step % self.config.steps_per_perturb == 0:
                     self.perturb_camera = not self.perturb_camera
 
             cbs.append(
                 TrainingCallback(
                     [TrainingCallbackLocation.BEFORE_TRAIN_ITERATION, TrainingCallbackLocation.AFTER_TRAIN_ITERATION],
                     toggle_perturb,
                 )
@@ -310,56 +237,28 @@
             metrics_dict: dictionary of metrics, some of which we can use for loss
         """
         loss_dict = {}
         # import pdb; pdb.set_trace();
         assert "mask" in batch, "mask must be in batch"
 
         if self.perturb_camera:
-            if self.config.use_sds:
-                disparity = depth_to_disparity(outputs["depth"][None])[0]
-                rgbd = torch.cat([outputs["rgb"], disparity], dim=-1).permute(2, 0, 1)[None]
-                rgbd = rgbd.to(self.config.sds_device)
-                sds_loss = self.diffusion_model.sds_loss(
-                    self.text_embeddings,
-                    rgbd,
-                    guidance_scale=self.config.sds_guidance_scale,
-                )
-                loss_dict["sds"] = sds_loss.to(self.device)
             if self.config.use_tv_in_novel_views:
                 pred_depth = outputs["depth"]
                 for stride in self.config.tv_in_novel_views_loss_strides:
                     l = self.config.tv_in_novel_views_loss_mult * tv_loss(pred_depth.permute(2, 0, 1)[None, :, ::stride, ::stride])
                     if l > 0:
                         loss_dict[f"depth_tv_in_novel_views_loss_stride-{stride}"] = l
             # hack to avoid having no gradients for backprop
             loss_dict["hack"] = (self.xys * 0).sum()
             return loss_dict
 
-        # dense warp for image
-        image_idx = batch["image_idx"]
         image = batch["image"] # (height, width, 3)
         mask = batch["mask"].to(image.device)[..., 0] # (height, width)
         depth = batch["depth_image"] # (height, width, 1)
 
-        # import pdb; pdb.set_trace()
-
-        if self.config.warp_images:
-            mesh = self.meshes[image_idx]
-            fragments = mesh.rasterize()
-            image = mesh.render(image, fragments)
-            mask = mesh.render(mask.float(), fragments)[...,0] > 0.5
-            depth = mesh.render(depth, fragments)
-
-        # mediapy.write_image("image.png", image.detach().cpu())
-        # mediapy.write_image("mask.png", (mask.float()).detach().cpu())
-        # mediapy.write_image("depth.png", apply_depth_colormap(depth).detach().cpu())
-
-        # import pdb; pdb.set_trace();
-        self.iters += 1
-
         assert self._get_downscale_factor() == 1, "downscale factor must be 1 for toon3d model"
 
         gt_img = image
 
         # rgb loss
         if self.config.use_color_palette and self.config.color_palette_use_as_colors:
             rgb = outputs["nd_value"] * mask[...,None].to(outputs["nd_value"].device)
@@ -405,20 +304,14 @@
             )
 
         if self.config.use_depth_loss:
             pred_depth = outputs["depth"]
             gt_depth = depth.to(pred_depth.device)
             loss_dict["depth_loss"] = self.config.depth_loss_mult * torch.abs(pred_depth[mask] - gt_depth[mask]).mean()
 
-        if self.config.use_chamfer_loss:
-            indices = torch.randperm(self.points3D_xyz.shape[0])[:self.config.chamfer_loss_num_points]
-            points3D_xyz = self.points3D_xyz[indices].to(self.means.device)
-            chamfer_loss = chamfer_distance(self.means[None], points3D_xyz[None], single_directional=True)[0]
-            loss_dict["chamfer_loss"] = self.config.chamfer_loss_mult * chamfer_loss
-
         if self.config.use_isotropic_loss:
             scale_var = torch.mean(torch.var(self.scales, dim=1))
             loss_dict["isotropic_loss"] = self.config.isotropic_ratio_mult * scale_var
 
         if self.config.use_ratio_loss:
             scale_exp = torch.exp(self.scales)
             scale_reg = (
```

### Comparing `toon3d-0.0.2/toon3d/utils/camera_utils.py` & `toon3d-0.0.3/toon3d/utils/camera_utils.py`

 * *Files identical despite different names*

### Comparing `toon3d-0.0.2/toon3d/utils/colmap_database.py` & `toon3d-0.0.3/toon3d/utils/colmap_database.py`

 * *Files identical despite different names*

### Comparing `toon3d-0.0.2/toon3d/utils/convert_points.py` & `toon3d-0.0.3/toon3d/utils/convert_points.py`

 * *Files identical despite different names*

### Comparing `toon3d-0.0.2/toon3d/utils/depth_utils.py` & `toon3d-0.0.3/toon3d/utils/depth_utils.py`

 * *Files identical despite different names*

### Comparing `toon3d-0.0.2/toon3d/utils/draw_utils.py` & `toon3d-0.0.3/toon3d/utils/draw_utils.py`

 * *Files identical despite different names*

### Comparing `toon3d-0.0.2/toon3d/utils/image_processing_utils.py` & `toon3d-0.0.3/toon3d/utils/image_processing_utils.py`

 * *Files identical despite different names*

### Comparing `toon3d-0.0.2/toon3d/utils/losses.py` & `toon3d-0.0.3/toon3d/utils/losses.py`

 * *Files identical despite different names*

### Comparing `toon3d-0.0.2/toon3d/utils/novel_view_samplers.py` & `toon3d-0.0.3/toon3d/utils/novel_view_samplers.py`

 * *Files identical despite different names*

### Comparing `toon3d-0.0.2/toon3d/utils/tsdf_utils.py` & `toon3d-0.0.3/toon3d/utils/tsdf_utils.py`

 * *Files identical despite different names*

### Comparing `toon3d-0.0.2/toon3d/utils/viser_utils.py` & `toon3d-0.0.3/toon3d/utils/viser_utils.py`

 * *Files identical despite different names*

### Comparing `toon3d-0.0.2/toon3d/warp/arap_utils.py` & `toon3d-0.0.3/toon3d/warp/arap_utils.py`

 * *Files identical despite different names*

### Comparing `toon3d-0.0.2/toon3d/warp/warp_mesh.py` & `toon3d-0.0.3/toon3d/warp/warp_mesh.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,19 +4,14 @@
 
 import cv2 
 import torch
 import torch.nn as nn
 from scipy.spatial import Delaunay
 import numpy as np
 
-from pytorch3d.renderer.mesh.rasterizer import Fragments
-
-from toon3d.warp.tri_rasterize import rasterize_face_verts, rasterize_texture
-
-
 def get_simplices(points):
     tri = Delaunay(points.detach().cpu().numpy())
     simplices = torch.tensor(tri.simplices, device=points.device)
     return simplices
 
 def get_half_edges(faces):
     half_edges = torch.stack((faces[:, [0, 1]], faces[:, [1, 2]], faces[:, [2, 0]]), dim=0).permute(1, 0, 2).flatten(0, 1)
@@ -80,15 +75,15 @@
 
     for point, color in zip(points, colors):
         x, y = point[0].int().item(), point[1].int().item()
         image = cv2.circle(image, (x, y), 2, color, thickness=5)
     return image
 
 class FrameMeshes(nn.Module):
-    def __init__(self, corr_points_padded, corr_masks_padded, depths, heights, widths):
+    def __init__(self, corr_points_padded, corr_masks_padded, depths):
         super().__init__()
 
         self.n = len(corr_points_padded)
 
         self.corr_points_padded = corr_points_padded.clone().float()
         self.corr_masks_padded = corr_masks_padded.clone()
 
@@ -213,15 +208,31 @@
     def warped_corr_zs_list(self):
         return (self.corr_zs_packed + self.delta_corr_zs_packed).split(self.num_corrs_per_mesh)
     
     @property
     def warped_zs_list(self):
         return self.warped_zs_packed.split(self.num_points_per_mesh)
     
+def barycentric_coordinates_batch(p, a, b, c):
+    v0 = b - a
+    v1 = c - a
+    v2 = p - a
+
+    d00 = (v0 * v0).sum(-1)
+    d01 = (v0 * v1).sum(-1)
+    d11 = (v1 * v1).sum(-1)
+    d20 = (v2 * v0).sum(-1)
+    d21 = (v2 * v1).sum(-1)
+
+    denom = d00 * d11 - d01 * d01
+    v = (d11 * d20 - d01 * d21) / denom
+    w = (d00 * d21 - d01 * d20) / denom
+    u = 1.0 - v - w
 
+    return u, v, w
 
 class WarpMesh(nn.Module):
     def __init__(self, points, simplices, height, width, uv_points=None, device="cpu"):
         """
         Creates a Mesh designed to fit an input image with triangulation
         """
         super().__init__()
@@ -232,87 +243,104 @@
         self.points = points.to(device).float()
         self.faces = simplices.to(device)
 
         if uv_points is None:
             uv_points = self.points.clone()
         self.uv_points = uv_points.to(device)
 
+        self.points_normed =  self.points.clone() / torch.tensor([width - 1, height - 1]).to(device) * 2 - 1
+        self.uv_points_normed =  self.uv_points.clone() / torch.tensor([width - 1, height - 1]).to(device) * 2 - 1
+
+        self.eps = 1 / (max(height - 1, width - 1))
+
         self.half_edges = get_half_edges(self.faces)
         self.edge_pairs = get_edge_pairs(self.half_edges)
         self.edge_twins = get_edge_twins(self.half_edges, self.edge_pairs)
 
         self.device = device
 
-        self.dpx = 1 / min(self.height - 1, self.width - 1)
-        self.faces_per_pixel = 1
+    def apply_warp(self, image):
+        """Applies warp to image
 
-        self.z_offset = 1
-        self.pzs = None
+        Args:
+            Image (torch.tensor): Image size (H, W, c)
 
-    @property
-    def normalized_points(self):
-        points = self.points
-        points_normed = points / torch.tensor([self.width - 1, self.height - 1], device=self.device) * 2 - 1
-        ratio = self.width / self.height
+        Returns:
+            Warped Image (torch.tensor): size (H, W, c)
+        """
+        image = image.permute(2, 0, 1)[None].to(self.device)
 
-        if ratio > 1:
-            points_normed[..., 0] *= ratio
-        elif ratio < 1:
-            points_normed[..., 1] /= ratio
+        target_image = torch.ones_like(image)
+        image_coords = torch.meshgrid(torch.linspace(-1, 1, self.height), torch.linspace(-1, 1, self.width), indexing="ij")
+        image_coords = torch.flip(torch.stack(image_coords, dim=-1), dims=[-1]).to(self.device)  # stored as (x,y) coordinates
 
-        points_normed[..., 0] *= (self.width - 1) / self.width
-        points_normed[..., 1] *= (self.height - 1) / self.height
+        for idx0, idx1, idx2 in self.faces:
 
-        return points_normed # exact barycentric
+            # skip if all simplices are zero because thats how we pad
+            if idx0 == idx1 == idx2 == 0:
+                continue
 
-    @property
-    def verts(self):
-        points_normed = self.normalized_points
-        zs = torch.full([len(points_normed),], self.z_offset).float().to(self.device)
-        if self.pzs is not None:
-            zs += self.pzs.to(self.device)
-        verts = torch.cat([points_normed, zs[...,None]], 1)
-        # zs = torch.ones(len(points_normed), 1).to(self.device)
-        # verts = torch.cat([points_normed, zs], 1)
+            # source image (from which we are copying)
+            S_a = self.uv_points_normed[idx0][None, None].repeat(self.height, self.width, 1)  # (H, W, 2,)
+            S_b = self.uv_points_normed[idx1][None, None].repeat(self.height, self.width, 1)  # (H, W, 2,)
+            S_c = self.uv_points_normed[idx2][None, None].repeat(self.height, self.width, 1)  # (H, W, 2,)
 
-        return verts
+            # destination image (to which we are copying)
+            a = self.points_normed[idx0][None, None].repeat(self.height, self.width, 1)  # (H, W, 2,)
+            b = self.points_normed[idx1][None, None].repeat(self.height, self.width, 1)  # (H, W, 2,)
+            c = self.points_normed[idx2][None, None].repeat(self.height, self.width, 1)  # (H, W, 2,)
 
-    @property
-    def face_verts(self):
-        return self.verts[self.faces]
+            # (u, v, w)
+            # https://gamedev.stackexchange.com/questions/23743/whats-the-most-efficient-way-to-find-barycentric-coordinates
+            v0 = b - a
+            v1 = c - a
+            v2 = image_coords - a
+
+            # replace dot without the function
+            d00 = (v0 * v0).sum(-1)
+            d01 = (v0 * v1).sum(-1)
+            d11 = (v1 * v1).sum(-1)
+            d20 = (v2 * v0).sum(-1)
+            d21 = (v2 * v1).sum(-1)
+
+            denom = d00 * d11 - d01 * d01
+            w_b = (d11 * d20 - d01 * d21) / denom
+            w_c = (d00 * d21 - d01 * d20) / denom
+            w_a = 1.0 - w_b - w_c
+
+            grid_sample_coordinates = S_a * w_a.unsqueeze(-1) + S_b * w_b.unsqueeze(-1) + S_c * w_c.unsqueeze(-1)
+            _grid = grid_sample_coordinates.unsqueeze(0).float()
+
+            pixels = torch.nn.functional.grid_sample(image, _grid, align_corners=True)[0]
+
+            valid_mask = (w_b >= 0 - self.eps) * (w_b <= 1 + self.eps) * (w_c >= 0 - self.eps) * (w_c <= 1 + self.eps) * (w_b + w_c <= 1 + self.eps)
+            mask = valid_mask.float().unsqueeze(0)
+
+            target_image = target_image * (1.0 - mask) + pixels * mask
+
+        return target_image[0].permute(1, 2, 0)
     
-    @property
-    def verts_uvs(self):
-        uv_points_normed = self.uv_points / torch.tensor([self.width - 1, self.height - 1], device=self.device)
-        return uv_points_normed[self.faces]
+    def vertex_coloring(self, vertex_colors):
+        img = torch.zeros((self.height, self.width), dtype=torch.float32).to(self.device)
 
-    def rasterize(self, variations=False):
-        face_verts = self.face_verts.clone()
+        for face in self.faces:
+            a, b, c = self.points[face]
+            color_a, color_b, color_c = vertex_colors[face]
 
-        # make variations
-        if variations:
-            face_verts = torch.cat([face_verts, self.face_verts_variations])
+            min_x = max(int(torch.min(torch.tensor([a[0], b[0], c[0]]))), 0)
+            max_x = min(int(torch.max(torch.tensor([a[0], b[0], c[0]]))), self.width - 1)
+            min_y = max(int(torch.min(torch.tensor([a[1], b[1], c[1]]))), 0)
+            max_y = min(int(torch.max(torch.tensor([a[1], b[1], c[1]]))), self.height - 1)
 
-        # rasterize
-        while True:
-            fragments = rasterize_face_verts(face_verts, (self.height, self.width), self.faces_per_pixel)
-            
-            # want to make sure there are enough k-dims in rasterization for all faces
-            # if torch.any(fragments.pix_to_face[...,-1] > -1):
-            #     self.faces_per_pixel += 1
-            # else:
-            return fragments
+            xx, yy = torch.meshgrid(torch.arange(min_x, max_x + 1).to(self.device), torch.arange(min_y, max_y + 1).to(self.device), indexing='xy')
+            xx, yy = xx.flatten(), yy.flatten()
+            p = torch.stack([xx, yy], dim=-1).float()
 
-    def render(self, image, fragments=None):
-        if len(image.shape) == 2:
-            image = image[None,...,None]
-        if len(image.shape) == 3:
-            image = image[None]
+            u, v, w = barycentric_coordinates_batch(p, a, b, c)
 
-        assert image.shape[1] == self.height and image.shape[2] == self.width
-        assert len(image.shape) == 4, "must be of size (1, height, width, c)"
-        if fragments is None:
-            fragments = self.rasterize()
+            mask = (u >= 0) & (v >= 0) & (w >= 0) & (u <= 1) & (v <= 1) & (w <= 1)
 
-        rendered_image = rasterize_texture(image, self.verts_uvs, fragments)[0]
+            if mask.any():
+                color = u[mask] * color_a + v[mask] * color_b + w[mask] * color_c
+                img[yy[mask].long(), xx[mask].long()] = color
 
-        return rendered_image
+        return img
```

### Comparing `toon3d-0.0.2/toon3d-labeler/node_modules/flatted/python/flatted.py` & `toon3d-0.0.3/toon3d-labeler/node_modules/flatted/python/flatted.py`

 * *Files identical despite different names*

### Comparing `toon3d-0.0.2/toon3d-labeler/node_modules/flatted/python/test.py` & `toon3d-0.0.3/toon3d-labeler/node_modules/flatted/python/test.py`

 * *Files identical despite different names*

### Comparing `toon3d-0.0.2/toon3d-spaces/app.py` & `toon3d-0.0.3/toon3d-spaces/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,15 +56,15 @@
 </div>
 '''
 
 def check_input_images(input_images):
     if input_images is None:
         raise gr.Error("No images uploaded!")
 
-@spaces.GPU
+@spaces.GPU(duration=120)
 def process_images(input_images):
 
     images_path = "/tmp/gradio/images"
     processed_path = "/tmp/gradio/processed"
 
     # remove the images_path folder
     os.system(f"rm -rf {images_path}")
@@ -96,15 +96,15 @@
     else:
         return ""
 
 def check_input_toon3d(processed_data_zip, labeled_data):
     if processed_data_zip is None:
         raise gr.Error("No images uploaded!")
     
-@spaces.GPU
+@spaces.GPU(duration=120)
 def run_toon3d(processed_data_zip, labeled_data):
 
     data_prefix = "/tmp/gradio/inputs"
     processed_path = f"{data_prefix}/toon3d-dataset"
     output_prefix = "/tmp/gradio/outputs"
     nerfstudio_folder = "/tmp/gradio/nerfstudio"
 
@@ -264,8 +264,9 @@
     open_viewer_button.click(fn=check_input_open_viewer, inputs=[processed_data_zip, labeled_data, toon3d_output_zip]).success(
         fn=start_viewer,
         inputs=[processed_data_zip, labeled_data, toon3d_output_zip],
         outputs=[viser_link],
     )
 
 if __name__ == "__main__":
-    demo.launch(server_port=7862)
+    demo.queue(max_size=10)
+    demo.launch()
```

### Comparing `toon3d-0.0.2/toon3d.egg-info/PKG-INFO` & `toon3d-0.0.3/toon3d.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: toon3d
-Version: 0.0.2
+Version: 0.0.3
 Summary: toon3d package
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python
 Requires-Python: >=3.7.3
 Requires-Dist: black
 Requires-Dist: h5py
 Requires-Dist: mediapy
@@ -25,7 +25,10 @@
 Requires-Dist: matplotlib
 Requires-Dist: onnxruntime
 Requires-Dist: onnx
 Requires-Dist: gdown==5.0.0
 Requires-Dist: diffusers>=0.25.1
 Requires-Dist: wandb>=0.16.2
 Requires-Dist: peft>=0.6.0
+Requires-Dist: viser
+Requires-Dist: jaxtyping>=0.2.15
+Requires-Dist: nerfstudio
```

### Comparing `toon3d-0.0.2/toon3d.egg-info/SOURCES.txt` & `toon3d-0.0.3/toon3d.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,48 +1,38 @@
 README.md
 pyproject.toml
-tests/test_finetune.py
 toon3d/__init__.py
 toon3d/color_palette.py
 toon3d/toon3d_config.py
 toon3d/toon3d_datamanager.py
 toon3d/toon3d_dataparser.py
 toon3d/toon3d_model.py
 toon3d/toon3d_pipeline.py
-toon3d/toon3d_process_data.py
-toon3d/warp_model.py
 toon3d-labeler/node_modules/flatted/python/flatted.py
 toon3d-labeler/node_modules/flatted/python/test.py
 toon3d-spaces/app.py
 toon3d.egg-info/PKG-INFO
 toon3d.egg-info/SOURCES.txt
 toon3d.egg-info/dependency_links.txt
 toon3d.egg-info/entry_points.txt
 toon3d.egg-info/requires.txt
 toon3d.egg-info/top_level.txt
 toon3d/configs/prompts.py
-toon3d/generative/ldm3d.py
 toon3d/generative/marigold.py
 toon3d/scripts/colmap_with_corrs.py
 toon3d/scripts/download_data.py
-toon3d/scripts/finetune.py
 toon3d/scripts/process_data.py
-toon3d/scripts/render.py
 toon3d/scripts/run.py
 toon3d/scripts/server.py
 toon3d/scripts/viser_vis.py
 toon3d/utils/camera_utils.py
 toon3d/utils/colmap_database.py
 toon3d/utils/convert_points.py
 toon3d/utils/depth_utils.py
 toon3d/utils/draw_utils.py
 toon3d/utils/image_processing_utils.py
 toon3d/utils/losses.py
-toon3d/utils/mesh_utils.py
 toon3d/utils/novel_view_samplers.py
 toon3d/utils/tsdf_utils.py
 toon3d/utils/viser_utils.py
-toon3d/utils/pytorch_arap/arap.py
-toon3d/utils/pytorch_arap/arap_utils.py
 toon3d/warp/arap_utils.py
-toon3d/warp/tri_rasterize.py
 toon3d/warp/warp_mesh.py
```

