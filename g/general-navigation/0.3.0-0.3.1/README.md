# Comparing `tmp/general_navigation-0.3.0.tar.gz` & `tmp/general_navigation-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "general_navigation-0.3.0.tar", last modified: Wed May 15 15:57:32 2024, max compression
+gzip compressed data, was "general_navigation-0.3.1.tar", last modified: Wed May 15 22:26:55 2024, max compression
```

## Comparing `general_navigation-0.3.0.tar` & `general_navigation-0.3.1.tar`

### file list

```diff
@@ -1,287 +1,287 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:57:32.934353 general_navigation-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-15 15:57:24.000000 general_navigation-0.3.0/Containerfile
--rw-r--r--   0 runner    (1001) docker     (127)     4927 2024-05-15 15:57:24.000000 general_navigation-0.3.0/HISTORY.md
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-15 15:57:24.000000 general_navigation-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-15 15:57:24.000000 general_navigation-0.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4086 2024-05-15 15:57:32.934353 general_navigation-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2831 2024-05-15 15:57:24.000000 general_navigation-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:57:32.886353 general_navigation-0.3.0/general_navigation/
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-15 15:57:24.000000 general_navigation-0.3.0/general_navigation/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 15:57:24.000000 general_navigation-0.3.0/general_navigation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      555 2024-05-15 15:57:24.000000 general_navigation-0.3.0/general_navigation/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      356 2024-05-15 15:57:24.000000 general_navigation-0.3.0/general_navigation/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:57:32.890353 general_navigation-0.3.0/general_navigation/carla/
--rw-r--r--   0 runner    (1001) docker     (127)     4327 2024-05-15 15:57:24.000000 general_navigation-0.3.0/general_navigation/carla/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    90254 2024-05-15 15:57:24.000000 general_navigation-0.3.0/general_navigation/carla/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     7283 2024-05-15 15:57:24.000000 general_navigation-0.3.0/general_navigation/carla_run.py
--rw-r--r--   0 runner    (1001) docker     (127)     2773 2024-05-15 15:57:24.000000 general_navigation-0.3.0/general_navigation/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      579 2024-05-15 15:57:24.000000 general_navigation-0.3.0/general_navigation/common.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:57:32.890353 general_navigation-0.3.0/general_navigation/diffusion_policy/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 15:57:24.000000 general_navigation-0.3.0/general_navigation/diffusion_policy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:57:32.890353 general_navigation-0.3.0/general_navigation/diffusion_policy/codecs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 15:57:24.000000 general_navigation-0.3.0/general_navigation/diffusion_policy/codecs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    40655 2024-05-15 15:57:24.000000 general_navigation-0.3.0/general_navigation/diffusion_policy/codecs/imagecodecs_numcodecs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:57:32.894353 general_navigation-0.3.0/general_navigation/diffusion_policy/common/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 15:57:24.000000 general_navigation-0.3.0/general_navigation/diffusion_policy/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1693 2024-05-15 15:57:24.000000 general_navigation-0.3.0/general_navigation/diffusion_policy/common/checkpoint_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     4122 2024-05-15 15:57:24.000000 general_navigation-0.3.0/general_navigation/diffusion_policy/common/cv2_util.py
--rw-r--r--   0 runner    (1001) docker     (127)      739 2024-05-15 15:57:24.000000 general_navigation-0.3.0/general_navigation/diffusion_policy/common/env_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     3701 2024-05-15 15:57:24.000000 general_navigation-0.3.0/general_navigation/diffusion_policy/common/json_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)      757 2024-05-15 15:57:24.000000 general_navigation-0.3.0/general_navigation/diffusion_policy/common/nested_dict_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     7738 2024-05-15 15:57:24.000000 general_navigation-0.3.0/general_navigation/diffusion_policy/common/normalize_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     7321 2024-05-15 15:57:24.000000 general_navigation-0.3.0/general_navigation/diffusion_policy/common/pose_trajectory_interpolator.py
--rw-r--r--   0 runner    (1001) docker     (127)      736 2024-05-15 15:57:24.000000 general_navigation-0.3.0/general_navigation/diffusion_policy/common/precise_sleep.py
--rw-r--r--   0 runner    (1001) docker     (127)     8597 2024-05-15 15:57:24.000000 general_navigation-0.3.0/general_navigation/diffusion_policy/common/pymunk_override.py
--rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-05-15 15:57:24.000000 general_navigation-0.3.0/general_navigation/diffusion_policy/common/pymunk_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     2682 2024-05-15 15:57:24.000000 general_navigation-0.3.0/general_navigation/diffusion_policy/common/pytorch_util.py
--rw-r--r--   0 runner    (1001) docker     (127)    21166 2024-05-15 15:57:24.000000 general_navigation-0.3.0/general_navigation/diffusion_policy/common/replay_buffer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1577 2024-05-15 15:57:24.000000 general_navigation-0.3.0/general_navigation/diffusion_policy/common/robomimic_config_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     6543 2024-05-15 15:57:24.000000 general_navigation-0.3.0/general_navigation/diffusion_policy/common/robomimic_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     6308 2024-05-15 15:57:24.000000 general_navigation-0.3.0/general_navigation/diffusion_policy/common/sampler.py
--rw-r--r--   0 runner    (1001) docker     (127)     7856 2024-05-15 15:57:24.000000 general_navigation-0.3.0/general_navigation/diffusion_policy/common/timestamp_accumulator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:57:32.898353 general_navigation-0.3.0/general_navigation/diffusion_policy/config/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 15:57:24.000000 general_navigation-0.3.0/general_navigation/diffusion_policy/config/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:57:32.902353 general_navigation-0.3.0/general_navigation/diffusion_policy/config/task/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 15:57:24.000000 general_navigation-0.3.0/general_navigation/diffusion_policy/config/task/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      902 2024-05-15 15:57:24.000000 general_navigation-0.3.0/general_navigation/diffusion_policy/config/task/blockpush_lowdim_seed.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      909 2024-05-15 15:57:24.000000 general_navigation-0.3.0/general_navigation/diffusion_policy/config/task/blockpush_lowdim_seed_abs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1788 2024-05-15 15:57:24.000000 general_navigation-0.3.0/general_navigation/diffusion_policy/config/task/can_image.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1792 2024-05-15 15:57:24.000000 general_navigation-0.3.0/general_navigation/diffusion_policy/config/task/can_image_abs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1380 2024-05-15 15:57:24.000000 general_navigation-0.3.0/general_navigation/diffusion_policy/config/task/can_lowdim.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1412 2024-05-15 15:57:24.000000 general_navigation-0.3.0/general_navigation/diffusion_policy/config/task/can_lowdim_abs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      798 2024-05-15 15:57:24.000000 general_navigation-0.3.0/general_navigation/diffusion_policy/config/task/kitchen_lowdim.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      990 2024-05-15 15:57:24.000000 general_navigation-0.3.0/general_navigation/diffusion_policy/config/task/kitchen_lowdim_abs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1790 2024-05-15 15:57:24.000000 general_navigation-0.3.0/general_navigation/diffusion_policy/config/task/lift_image.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1772 2024-05-15 15:57:24.000000 general_navigation-0.3.0/general_navigation/diffusion_policy/config/task/lift_image_abs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1407 2024-05-15 15:57:24.000000 general_navigation-0.3.0/general_navigation/diffusion_policy/config/task/lift_lowdim.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1439 2024-05-15 15:57:24.000000 general_navigation-0.3.0/general_navigation/diffusion_policy/config/task/lift_lowdim_abs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      948 2024-05-15 15:57:24.000000 general_navigation-0.3.0/general_navigation/diffusion_policy/config/task/pusht_image.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      918 2024-05-15 15:57:24.000000 general_navigation-0.3.0/general_navigation/diffusion_policy/config/task/pusht_lowdim.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-05-15 15:57:24.000000 general_navigation-0.3.0/general_navigation/diffusion_policy/config/task/real_pusht_image.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1794 2024-05-15 15:57:24.000000 general_navigation-0.3.0/general_navigation/diffusion_policy/config/task/square_image.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1798 2024-05-15 15:57:24.000000 general_navigation-0.3.0/general_navigation/diffusion_policy/config/task/square_image_abs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1413 2024-05-15 15:57:24.000000 general_navigation-0.3.0/general_navigation/diffusion_policy/config/task/square_lowdim.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-05-15 15:57:24.000000 general_navigation-0.3.0/general_navigation/diffusion_policy/config/task/square_lowdim_abs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-05-15 15:57:24.000000 general_navigation-0.3.0/general_navigation/diffusion_policy/config/task/tool_hang_image.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1680 2024-05-15 15:57:24.000000 general_navigation-0.3.0/general_navigation/diffusion_policy/config/task/tool_hang_image_abs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1307 2024-05-15 15:57:24.000000 general_navigation-0.3.0/general_navigation/diffusion_policy/config/task/tool_hang_lowdim.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-05-15 15:57:24.000000 general_navigation-0.3.0/general_navigation/diffusion_policy/config/task/tool_hang_lowdim_abs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1947 2024-05-15 15:57:24.000000 general_navigation-0.3.0/general_navigation/diffusion_policy/config/task/transport_image.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1950 2024-05-15 15:57:24.000000 general_navigation-0.3.0/general_navigation/diffusion_policy/config/task/transport_image_abs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1416 2024-05-15 15:57:24.000000 general_navigation-0.3.0/general_navigation/diffusion_policy/config/task/transport_lowdim.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-05-15 15:57:24.000000 general_navigation-0.3.0/general_navigation/diffusion_policy/config/task/transport_lowdim_abs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3043 2024-05-15 15:57:24.000000 general_navigation-0.3.0/general_navigation/diffusion_policy/config/train_bet_lowdim_workspace.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3503 2024-05-15 15:57:24.000000 general_navigation-0.3.0/general_navigation/diffusion_policy/config/train_diffusion_transformer_hybrid_workspace.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3766 2024-05-15 15:57:24.000000 general_navigation-0.3.0/general_navigation/diffusion_policy/config/train_diffusion_transformer_lowdim_kitchen_workspace.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3761 2024-05-15 15:57:24.000000 general_navigation-0.3.0/general_navigation/diffusion_policy/config/train_diffusion_transformer_lowdim_pusht_workspace.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3768 2024-05-15 15:57:24.000000 general_navigation-0.3.0/general_navigation/diffusion_policy/config/train_diffusion_transformer_lowdim_workspace.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3482 2024-05-15 15:57:24.000000 general_navigation-0.3.0/general_navigation/diffusion_policy/config/train_diffusion_transformer_real_hybrid_workspace.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3301 2024-05-15 15:57:24.000000 general_navigation-0.3.0/general_navigation/diffusion_policy/config/train_diffusion_unet_ddim_hybrid_workspace.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3763 2024-05-15 15:57:24.000000 general_navigation-0.3.0/general_navigation/diffusion_policy/config/train_diffusion_unet_ddim_lowdim_workspace.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3331 2024-05-15 15:57:24.000000 general_navigation-0.3.0/general_navigation/diffusion_policy/config/train_diffusion_unet_hybrid_workspace.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3732 2024-05-15 15:57:24.000000 general_navigation-0.3.0/general_navigation/diffusion_policy/config/train_diffusion_unet_image_pretrained_workspace.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3733 2024-05-15 15:57:24.000000 general_navigation-0.3.0/general_navigation/diffusion_policy/config/train_diffusion_unet_image_workspace.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3789 2024-05-15 15:57:24.000000 general_navigation-0.3.0/general_navigation/diffusion_policy/config/train_diffusion_unet_lowdim_workspace.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3345 2024-05-15 15:57:24.000000 general_navigation-0.3.0/general_navigation/diffusion_policy/config/train_diffusion_unet_real_hybrid_workspace.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3694 2024-05-15 15:57:24.000000 general_navigation-0.3.0/general_navigation/diffusion_policy/config/train_diffusion_unet_real_image_workspace.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3684 2024-05-15 15:57:24.000000 general_navigation-0.3.0/general_navigation/diffusion_policy/config/train_diffusion_unet_real_pretrained_workspace.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3145 2024-05-15 15:57:24.000000 general_navigation-0.3.0/general_navigation/diffusion_policy/config/train_diffusion_unet_video_workspace.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2464 2024-05-15 15:57:24.000000 general_navigation-0.3.0/general_navigation/diffusion_policy/config/train_ibc_dfo_hybrid_workspace.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2423 2024-05-15 15:57:24.000000 general_navigation-0.3.0/general_navigation/diffusion_policy/config/train_ibc_dfo_lowdim_workspace.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2482 2024-05-15 15:57:24.000000 general_navigation-0.3.0/general_navigation/diffusion_policy/config/train_ibc_dfo_real_hybrid_workspace.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-05-15 15:57:24.000000 general_navigation-0.3.0/general_navigation/diffusion_policy/config/train_robomimic_image_workspace.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2166 2024-05-15 15:57:24.000000 general_navigation-0.3.0/general_navigation/diffusion_policy/config/train_robomimic_lowdim_workspace.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2140 2024-05-15 15:57:24.000000 general_navigation-0.3.0/general_navigation/diffusion_policy/config/train_robomimic_real_image_workspace.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:57:32.902353 general_navigation-0.3.0/general_navigation/diffusion_policy/dataset/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 15:57:24.000000 general_navigation-0.3.0/general_navigation/diffusion_policy/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1397 2024-05-15 15:57:24.000000 general_navigation-0.3.0/general_navigation/diffusion_policy/dataset/base_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     4796 2024-05-15 15:57:24.000000 general_navigation-0.3.0/general_navigation/diffusion_policy/dataset/blockpush_lowdim_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     3257 2024-05-15 15:57:24.000000 general_navigation-0.3.0/general_navigation/diffusion_policy/dataset/kitchen_lowdim_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     5041 2024-05-15 15:57:24.000000 general_navigation-0.3.0/general_navigation/diffusion_policy/dataset/kitchen_mjl_lowdim_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     3302 2024-05-15 15:57:24.000000 general_navigation-0.3.0/general_navigation/diffusion_policy/dataset/pusht_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     3761 2024-05-15 15:57:24.000000 general_navigation-0.3.0/general_navigation/diffusion_policy/dataset/pusht_image_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)    10891 2024-05-15 15:57:24.000000 general_navigation-0.3.0/general_navigation/diffusion_policy/dataset/real_pusht_image_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)    15410 2024-05-15 15:57:24.000000 general_navigation-0.3.0/general_navigation/diffusion_policy/dataset/robomimic_replay_image_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     6096 2024-05-15 15:57:24.000000 general_navigation-0.3.0/general_navigation/diffusion_policy/dataset/robomimic_replay_lowdim_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:57:32.906353 general_navigation-0.3.0/general_navigation/diffusion_policy/env_runner/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 15:57:24.000000 general_navigation-0.3.0/general_navigation/diffusion_policy/env_runner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      310 2024-05-15 15:57:24.000000 general_navigation-0.3.0/general_navigation/diffusion_policy/env_runner/base_image_runner.py
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-05-15 15:57:24.000000 general_navigation-0.3.0/general_navigation/diffusion_policy/env_runner/base_lowdim_runner.py
--rw-r--r--   0 runner    (1001) docker     (127)    11343 2024-05-15 15:57:24.000000 general_navigation-0.3.0/general_navigation/diffusion_policy/env_runner/blockpush_lowdim_runner.py
--rw-r--r--   0 runner    (1001) docker     (127)    13030 2024-05-15 15:57:24.000000 general_navigation-0.3.0/general_navigation/diffusion_policy/env_runner/kitchen_lowdim_runner.py
--rw-r--r--   0 runner    (1001) docker     (127)     9438 2024-05-15 15:57:24.000000 general_navigation-0.3.0/general_navigation/diffusion_policy/env_runner/pusht_image_runner.py
--rw-r--r--   0 runner    (1001) docker     (127)    10627 2024-05-15 15:57:24.000000 general_navigation-0.3.0/general_navigation/diffusion_policy/env_runner/pusht_keypoints_runner.py
--rw-r--r--   0 runner    (1001) docker     (127)      387 2024-05-15 15:57:24.000000 general_navigation-0.3.0/general_navigation/diffusion_policy/env_runner/real_pusht_image_runner.py
--rw-r--r--   0 runner    (1001) docker     (127)    14287 2024-05-15 15:57:24.000000 general_navigation-0.3.0/general_navigation/diffusion_policy/env_runner/robomimic_image_runner.py
--rw-r--r--   0 runner    (1001) docker     (127)    13686 2024-05-15 15:57:24.000000 general_navigation-0.3.0/general_navigation/diffusion_policy/env_runner/robomimic_lowdim_runner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:57:32.906353 general_navigation-0.3.0/general_navigation/diffusion_policy/gym_util/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 15:57:24.000000 general_navigation-0.3.0/general_navigation/diffusion_policy/gym_util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25848 2024-05-15 15:57:24.000000 general_navigation-0.3.0/general_navigation/diffusion_policy/gym_util/async_vector_env.py
--rw-r--r--   0 runner    (1001) docker     (127)     4967 2024-05-15 15:57:24.000000 general_navigation-0.3.0/general_navigation/diffusion_policy/gym_util/multistep_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     6519 2024-05-15 15:57:24.000000 general_navigation-0.3.0/general_navigation/diffusion_policy/gym_util/sync_vector_env.py
--rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-05-15 15:57:24.000000 general_navigation-0.3.0/general_navigation/diffusion_policy/gym_util/video_recording_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-05-15 15:57:24.000000 general_navigation-0.3.0/general_navigation/diffusion_policy/gym_util/video_wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:57:32.906353 general_navigation-0.3.0/general_navigation/diffusion_policy/model/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 15:57:24.000000 general_navigation-0.3.0/general_navigation/diffusion_policy/model/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:57:32.906353 general_navigation-0.3.0/general_navigation/diffusion_policy/model/bet/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 15:57:24.000000 general_navigation-0.3.0/general_navigation/diffusion_policy/model/bet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:57:32.906353 general_navigation-0.3.0/general_navigation/diffusion_policy/model/bet/action_ae/
--rw-r--r--   0 runner    (1001) docker     (127)     1818 2024-05-15 15:57:24.000000 general_navigation-0.3.0/general_navigation/diffusion_policy/model/bet/action_ae/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:57:32.910353 general_navigation-0.3.0/general_navigation/diffusion_policy/model/bet/action_ae/discretizers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 15:57:24.000000 general_navigation-0.3.0/general_navigation/diffusion_policy/model/bet/action_ae/discretizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5611 2024-05-15 15:57:24.000000 general_navigation-0.3.0/general_navigation/diffusion_policy/model/bet/action_ae/discretizers/k_means.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:57:32.910353 general_navigation-0.3.0/general_navigation/diffusion_policy/model/bet/latent_generators/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 15:57:24.000000 general_navigation-0.3.0/general_navigation/diffusion_policy/model/bet/latent_generators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2707 2024-05-15 15:57:24.000000 general_navigation-0.3.0/general_navigation/diffusion_policy/model/bet/latent_generators/latent_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     7904 2024-05-15 15:57:24.000000 general_navigation-0.3.0/general_navigation/diffusion_policy/model/bet/latent_generators/mingpt.py
--rw-r--r--   0 runner    (1001) docker     (127)     4183 2024-05-15 15:57:24.000000 general_navigation-0.3.0/general_navigation/diffusion_policy/model/bet/latent_generators/transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:57:32.910353 general_navigation-0.3.0/general_navigation/diffusion_policy/model/bet/libraries/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 15:57:24.000000 general_navigation-0.3.0/general_navigation/diffusion_policy/model/bet/libraries/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6109 2024-05-15 15:57:24.000000 general_navigation-0.3.0/general_navigation/diffusion_policy/model/bet/libraries/loss_fn.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:57:32.910353 general_navigation-0.3.0/general_navigation/diffusion_policy/model/bet/libraries/mingpt/
--rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-05-15 15:57:24.000000 general_navigation-0.3.0/general_navigation/diffusion_policy/model/bet/libraries/mingpt/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 15:57:24.000000 general_navigation-0.3.0/general_navigation/diffusion_policy/model/bet/libraries/mingpt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9700 2024-05-15 15:57:24.000000 general_navigation-0.3.0/general_navigation/diffusion_policy/model/bet/libraries/mingpt/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     6178 2024-05-15 15:57:24.000000 general_navigation-0.3.0/general_navigation/diffusion_policy/model/bet/libraries/mingpt/trainer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1747 2024-05-15 15:57:24.000000 general_navigation-0.3.0/general_navigation/diffusion_policy/model/bet/libraries/mingpt/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4108 2024-05-15 15:57:24.000000 general_navigation-0.3.0/general_navigation/diffusion_policy/model/bet/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:57:32.910353 general_navigation-0.3.0/general_navigation/diffusion_policy/model/common/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 15:57:24.000000 general_navigation-0.3.0/general_navigation/diffusion_policy/model/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1441 2024-05-15 15:57:24.000000 general_navigation-0.3.0/general_navigation/diffusion_policy/model/common/dict_of_tensor_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     2088 2024-05-15 15:57:24.000000 general_navigation-0.3.0/general_navigation/diffusion_policy/model/common/lr_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (127)      331 2024-05-15 15:57:24.000000 general_navigation-0.3.0/general_navigation/diffusion_policy/model/common/module_attr_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)    12232 2024-05-15 15:57:24.000000 general_navigation-0.3.0/general_navigation/diffusion_policy/model/common/normalizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3345 2024-05-15 15:57:24.000000 general_navigation-0.3.0/general_navigation/diffusion_policy/model/common/rotation_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)      624 2024-05-15 15:57:24.000000 general_navigation-0.3.0/general_navigation/diffusion_policy/model/common/shape_util.py
--rw-r--r--   0 runner    (1001) docker     (127)    30748 2024-05-15 15:57:24.000000 general_navigation-0.3.0/general_navigation/diffusion_policy/model/common/tensor_util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:57:32.914353 general_navigation-0.3.0/general_navigation/diffusion_policy/model/diffusion/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 15:57:24.000000 general_navigation-0.3.0/general_navigation/diffusion_policy/model/diffusion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10423 2024-05-15 15:57:24.000000 general_navigation-0.3.0/general_navigation/diffusion_policy/model/diffusion/conditional_unet1d.py
--rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-05-15 15:57:24.000000 general_navigation-0.3.0/general_navigation/diffusion_policy/model/diffusion/conv1d_components.py
--rw-r--r--   0 runner    (1001) docker     (127)     3419 2024-05-15 15:57:24.000000 general_navigation-0.3.0/general_navigation/diffusion_policy/model/diffusion/ema_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     8615 2024-05-15 15:57:24.000000 general_navigation-0.3.0/general_navigation/diffusion_policy/model/diffusion/mask_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)      482 2024-05-15 15:57:24.000000 general_navigation-0.3.0/general_navigation/diffusion_policy/model/diffusion/positional_embedding.py
--rw-r--r--   0 runner    (1001) docker     (127)    15364 2024-05-15 15:57:24.000000 general_navigation-0.3.0/general_navigation/diffusion_policy/model/diffusion/transformer_for_diffusion.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:57:32.914353 general_navigation-0.3.0/general_navigation/diffusion_policy/model/vision/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 15:57:24.000000 general_navigation-0.3.0/general_navigation/diffusion_policy/model/vision/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13222 2024-05-15 15:57:24.000000 general_navigation-0.3.0/general_navigation/diffusion_policy/model/vision/crop_randomizer.py
--rw-r--r--   0 runner    (1001) docker     (127)      720 2024-05-15 15:57:24.000000 general_navigation-0.3.0/general_navigation/diffusion_policy/model/vision/model_getter.py
--rw-r--r--   0 runner    (1001) docker     (127)     7723 2024-05-15 15:57:24.000000 general_navigation-0.3.0/general_navigation/diffusion_policy/model/vision/multi_image_obs_encoder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:57:32.918353 general_navigation-0.3.0/general_navigation/diffusion_policy/policy/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 15:57:24.000000 general_navigation-0.3.0/general_navigation/diffusion_policy/policy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      888 2024-05-15 15:57:24.000000 general_navigation-0.3.0/general_navigation/diffusion_policy/policy/base_image_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-05-15 15:57:24.000000 general_navigation-0.3.0/general_navigation/diffusion_policy/policy/base_lowdim_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)     5093 2024-05-15 15:57:24.000000 general_navigation-0.3.0/general_navigation/diffusion_policy/policy/bet_lowdim_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)    14218 2024-05-15 15:57:24.000000 general_navigation-0.3.0/general_navigation/diffusion_policy/policy/diffusion_transformer_hybrid_image_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)     8310 2024-05-15 15:57:24.000000 general_navigation-0.3.0/general_navigation/diffusion_policy/policy/diffusion_transformer_lowdim_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)    13506 2024-05-15 15:57:24.000000 general_navigation-0.3.0/general_navigation/diffusion_policy/policy/diffusion_unet_hybrid_image_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)     9968 2024-05-15 15:57:24.000000 general_navigation-0.3.0/general_navigation/diffusion_policy/policy/diffusion_unet_image_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)     9545 2024-05-15 15:57:24.000000 general_navigation-0.3.0/general_navigation/diffusion_policy/policy/diffusion_unet_lowdim_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)    11716 2024-05-15 15:57:24.000000 general_navigation-0.3.0/general_navigation/diffusion_policy/policy/diffusion_unet_video_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)    13029 2024-05-15 15:57:24.000000 general_navigation-0.3.0/general_navigation/diffusion_policy/policy/ibc_dfo_hybrid_image_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)     8532 2024-05-15 15:57:24.000000 general_navigation-0.3.0/general_navigation/diffusion_policy/policy/ibc_dfo_lowdim_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)     4940 2024-05-15 15:57:24.000000 general_navigation-0.3.0/general_navigation/diffusion_policy/policy/robomimic_image_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)     3163 2024-05-15 15:57:24.000000 general_navigation-0.3.0/general_navigation/diffusion_policy/policy/robomimic_lowdim_policy.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:57:32.918353 general_navigation-0.3.0/general_navigation/diffusion_policy/real_world/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 15:57:24.000000 general_navigation-0.3.0/general_navigation/diffusion_policy/real_world/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-05-15 15:57:24.000000 general_navigation-0.3.0/general_navigation/diffusion_policy/real_world/keystroke_counter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2326 2024-05-15 15:57:24.000000 general_navigation-0.3.0/general_navigation/diffusion_policy/real_world/multi_camera_visualizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     7900 2024-05-15 15:57:24.000000 general_navigation-0.3.0/general_navigation/diffusion_policy/real_world/multi_realsense.py
--rw-r--r--   0 runner    (1001) docker     (127)     8789 2024-05-15 15:57:24.000000 general_navigation-0.3.0/general_navigation/diffusion_policy/real_world/real_data_conversion.py
--rw-r--r--   0 runner    (1001) docker     (127)    15113 2024-05-15 15:57:24.000000 general_navigation-0.3.0/general_navigation/diffusion_policy/real_world/real_env.py
--rw-r--r--   0 runner    (1001) docker     (127)     1858 2024-05-15 15:57:24.000000 general_navigation-0.3.0/general_navigation/diffusion_policy/real_world/real_inference_util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:57:32.918353 general_navigation-0.3.0/general_navigation/diffusion_policy/real_world/realsense_config/
--rw-r--r--   0 runner    (1001) docker     (127)     3537 2024-05-15 15:57:24.000000 general_navigation-0.3.0/general_navigation/diffusion_policy/real_world/realsense_config/415_high_accuracy_mode.json
--rw-r--r--   0 runner    (1001) docker     (127)     3434 2024-05-15 15:57:24.000000 general_navigation-0.3.0/general_navigation/diffusion_policy/real_world/realsense_config/435_high_accuracy_mode.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 15:57:24.000000 general_navigation-0.3.0/general_navigation/diffusion_policy/real_world/realsense_config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13197 2024-05-15 15:57:24.000000 general_navigation-0.3.0/general_navigation/diffusion_policy/real_world/rtde_interpolation_controller.py
--rw-r--r--   0 runner    (1001) docker     (127)    19065 2024-05-15 15:57:24.000000 general_navigation-0.3.0/general_navigation/diffusion_policy/real_world/single_realsense.py
--rw-r--r--   0 runner    (1001) docker     (127)     3183 2024-05-15 15:57:24.000000 general_navigation-0.3.0/general_navigation/diffusion_policy/real_world/spacemouse.py
--rw-r--r--   0 runner    (1001) docker     (127)     5258 2024-05-15 15:57:24.000000 general_navigation-0.3.0/general_navigation/diffusion_policy/real_world/spacemouse_shared_memory.py
--rw-r--r--   0 runner    (1001) docker     (127)     5029 2024-05-15 15:57:24.000000 general_navigation-0.3.0/general_navigation/diffusion_policy/real_world/video_recorder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:57:32.922353 general_navigation-0.3.0/general_navigation/diffusion_policy/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 15:57:24.000000 general_navigation-0.3.0/general_navigation/diffusion_policy/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1426 2024-05-15 15:57:24.000000 general_navigation-0.3.0/general_navigation/diffusion_policy/scripts/bet_blockpush_conversion.py
--rw-r--r--   0 runner    (1001) docker     (127)      876 2024-05-15 15:57:24.000000 general_navigation-0.3.0/general_navigation/diffusion_policy/scripts/blockpush_abs_conversion.py
--rw-r--r--   0 runner    (1001) docker     (127)      705 2024-05-15 15:57:24.000000 general_navigation-0.3.0/general_navigation/diffusion_policy/scripts/episode_lengths.py
--rw-r--r--   0 runner    (1001) docker     (127)     2212 2024-05-15 15:57:24.000000 general_navigation-0.3.0/general_navigation/diffusion_policy/scripts/generate_bet_blockpush.py
--rw-r--r--   0 runner    (1001) docker     (127)     1918 2024-05-15 15:57:24.000000 general_navigation-0.3.0/general_navigation/diffusion_policy/scripts/real_dataset_conversion.py
--rw-r--r--   0 runner    (1001) docker     (127)     4679 2024-05-15 15:57:24.000000 general_navigation-0.3.0/general_navigation/diffusion_policy/scripts/real_pusht_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     2391 2024-05-15 15:57:24.000000 general_navigation-0.3.0/general_navigation/diffusion_policy/scripts/real_pusht_successrate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1647 2024-05-15 15:57:24.000000 general_navigation-0.3.0/general_navigation/diffusion_policy/scripts/robomimic_dataset_action_comparison.py
--rw-r--r--   0 runner    (1001) docker     (127)     3337 2024-05-15 15:57:24.000000 general_navigation-0.3.0/general_navigation/diffusion_policy/scripts/robomimic_dataset_conversion.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:57:32.922353 general_navigation-0.3.0/general_navigation/diffusion_policy/shared_memory/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 15:57:24.000000 general_navigation-0.3.0/general_navigation/diffusion_policy/shared_memory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5830 2024-05-15 15:57:24.000000 general_navigation-0.3.0/general_navigation/diffusion_policy/shared_memory/shared_memory_queue.py
--rw-r--r--   0 runner    (1001) docker     (127)     8233 2024-05-15 15:57:24.000000 general_navigation-0.3.0/general_navigation/diffusion_policy/shared_memory/shared_memory_ring_buffer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-05-15 15:57:24.000000 general_navigation-0.3.0/general_navigation/diffusion_policy/shared_memory/shared_memory_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     7392 2024-05-15 15:57:24.000000 general_navigation-0.3.0/general_navigation/diffusion_policy/shared_memory/shared_ndarray.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:57:32.926353 general_navigation-0.3.0/general_navigation/diffusion_policy/workspace/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 15:57:24.000000 general_navigation-0.3.0/general_navigation/diffusion_policy/workspace/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5135 2024-05-15 15:57:24.000000 general_navigation-0.3.0/general_navigation/diffusion_policy/workspace/base_workspace.py
--rw-r--r--   0 runner    (1001) docker     (127)    13075 2024-05-15 15:57:24.000000 general_navigation-0.3.0/general_navigation/diffusion_policy/workspace/train_bet_lowdim_workspace.py
--rw-r--r--   0 runner    (1001) docker     (127)    13128 2024-05-15 15:57:24.000000 general_navigation-0.3.0/general_navigation/diffusion_policy/workspace/train_diffusion_transformer_hybrid_workspace.py
--rw-r--r--   0 runner    (1001) docker     (127)    13338 2024-05-15 15:57:24.000000 general_navigation-0.3.0/general_navigation/diffusion_policy/workspace/train_diffusion_transformer_lowdim_workspace.py
--rw-r--r--   0 runner    (1001) docker     (127)    13135 2024-05-15 15:57:24.000000 general_navigation-0.3.0/general_navigation/diffusion_policy/workspace/train_diffusion_unet_hybrid_workspace.py
--rw-r--r--   0 runner    (1001) docker     (127)    13272 2024-05-15 15:57:24.000000 general_navigation-0.3.0/general_navigation/diffusion_policy/workspace/train_diffusion_unet_image_workspace.py
--rw-r--r--   0 runner    (1001) docker     (127)    13317 2024-05-15 15:57:24.000000 general_navigation-0.3.0/general_navigation/diffusion_policy/workspace/train_diffusion_unet_lowdim_workspace.py
--rw-r--r--   0 runner    (1001) docker     (127)     9530 2024-05-15 15:57:24.000000 general_navigation-0.3.0/general_navigation/diffusion_policy/workspace/train_diffusion_unet_video_workspace.py
--rw-r--r--   0 runner    (1001) docker     (127)    12846 2024-05-15 15:57:24.000000 general_navigation-0.3.0/general_navigation/diffusion_policy/workspace/train_ibc_dfo_hybrid_workspace.py
--rw-r--r--   0 runner    (1001) docker     (127)    12470 2024-05-15 15:57:24.000000 general_navigation-0.3.0/general_navigation/diffusion_policy/workspace/train_ibc_dfo_lowdim_workspace.py
--rw-r--r--   0 runner    (1001) docker     (127)    11336 2024-05-15 15:57:24.000000 general_navigation-0.3.0/general_navigation/diffusion_policy/workspace/train_robomimic_image_workspace.py
--rw-r--r--   0 runner    (1001) docker     (127)     9621 2024-05-15 15:57:24.000000 general_navigation-0.3.0/general_navigation/diffusion_policy/workspace/train_robomimic_lowdim_workspace.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:57:32.926353 general_navigation-0.3.0/general_navigation/gpt/
--rw-r--r--   0 runner    (1001) docker     (127)     2491 2024-05-15 15:57:24.000000 general_navigation-0.3.0/general_navigation/gpt/gpt_vision.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:57:32.926353 general_navigation-0.3.0/general_navigation/models/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 15:57:24.000000 general_navigation-0.3.0/general_navigation/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1597 2024-05-15 15:57:24.000000 general_navigation-0.3.0/general_navigation/models/base_model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:57:32.926353 general_navigation-0.3.0/general_navigation/models/config/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 15:57:24.000000 general_navigation-0.3.0/general_navigation/models/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1292 2024-05-15 15:57:24.000000 general_navigation-0.3.0/general_navigation/models/config/data_config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-05-15 15:57:24.000000 general_navigation-0.3.0/general_navigation/models/config/defaults.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3479 2024-05-15 15:57:24.000000 general_navigation-0.3.0/general_navigation/models/config/gnm.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3662 2024-05-15 15:57:24.000000 general_navigation-0.3.0/general_navigation/models/config/late_fusion.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3563 2024-05-15 15:57:24.000000 general_navigation-0.3.0/general_navigation/models/config/nomad.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3651 2024-05-15 15:57:24.000000 general_navigation-0.3.0/general_navigation/models/config/vint.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     5410 2024-05-15 15:57:24.000000 general_navigation-0.3.0/general_navigation/models/factory.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:57:32.926353 general_navigation-0.3.0/general_navigation/models/gnm/
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-15 15:57:24.000000 general_navigation-0.3.0/general_navigation/models/gnm/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 15:57:24.000000 general_navigation-0.3.0/general_navigation/models/gnm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3616 2024-05-15 15:57:24.000000 general_navigation-0.3.0/general_navigation/models/gnm/gnm.py
--rw-r--r--   0 runner    (1001) docker     (127)     5171 2024-05-15 15:57:24.000000 general_navigation-0.3.0/general_navigation/models/gnm/modified_mobilenetv2.py
--rw-r--r--   0 runner    (1001) docker     (127)    20868 2024-05-15 15:57:24.000000 general_navigation-0.3.0/general_navigation/models/model_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:57:32.930353 general_navigation-0.3.0/general_navigation/models/nomad/
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-15 15:57:24.000000 general_navigation-0.3.0/general_navigation/models/nomad/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 15:57:24.000000 general_navigation-0.3.0/general_navigation/models/nomad/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-05-15 15:57:24.000000 general_navigation-0.3.0/general_navigation/models/nomad/nomad.py
--rw-r--r--   0 runner    (1001) docker     (127)     8480 2024-05-15 15:57:24.000000 general_navigation-0.3.0/general_navigation/models/nomad/nomad_vint.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 15:57:24.000000 general_navigation-0.3.0/general_navigation/models/nomad/vib_placeholder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:57:32.930353 general_navigation-0.3.0/general_navigation/models/vint/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 15:57:24.000000 general_navigation-0.3.0/general_navigation/models/vint/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2438 2024-05-15 15:57:24.000000 general_navigation-0.3.0/general_navigation/models/vint/self_attention.py
--rw-r--r--   0 runner    (1001) docker     (127)     7113 2024-05-15 15:57:24.000000 general_navigation-0.3.0/general_navigation/models/vint/vint.py
--rw-r--r--   0 runner    (1001) docker     (127)     8146 2024-05-15 15:57:24.000000 general_navigation-0.3.0/general_navigation/models/vint/vit.py
--rw-r--r--   0 runner    (1001) docker     (127)     4719 2024-05-15 15:57:24.000000 general_navigation-0.3.0/general_navigation/mpc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:57:32.930353 general_navigation-0.3.0/general_navigation/schema/
--rw-r--r--   0 runner    (1001) docker     (127)     1745 2024-05-15 15:57:24.000000 general_navigation-0.3.0/general_navigation/schema/carla.py
--rw-r--r--   0 runner    (1001) docker     (127)      843 2024-05-15 15:57:24.000000 general_navigation-0.3.0/general_navigation/schema/image.py
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-05-15 15:57:24.000000 general_navigation-0.3.0/general_navigation/schema/packet.py
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-15 15:57:24.000000 general_navigation-0.3.0/general_navigation/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:57:32.930353 general_navigation-0.3.0/general_navigation/visualizing/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 15:57:24.000000 general_navigation-0.3.0/general_navigation/visualizing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17421 2024-05-15 15:57:24.000000 general_navigation-0.3.0/general_navigation/visualizing/action_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     7435 2024-05-15 15:57:24.000000 general_navigation-0.3.0/general_navigation/visualizing/distance_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      625 2024-05-15 15:57:24.000000 general_navigation-0.3.0/general_navigation/visualizing/visualize_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:57:32.930353 general_navigation-0.3.0/general_navigation.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4086 2024-05-15 15:57:32.000000 general_navigation-0.3.0/general_navigation.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    15689 2024-05-15 15:57:32.000000 general_navigation-0.3.0/general_navigation.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 15:57:32.000000 general_navigation-0.3.0/general_navigation.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-15 15:57:32.000000 general_navigation-0.3.0/general_navigation.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      363 2024-05-15 15:57:32.000000 general_navigation-0.3.0/general_navigation.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-15 15:57:32.000000 general_navigation-0.3.0/general_navigation.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 15:57:32.934353 general_navigation-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-05-15 15:57:24.000000 general_navigation-0.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:57:32.930353 general_navigation-0.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 15:57:24.000000 general_navigation-0.3.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      398 2024-05-15 15:57:24.000000 general_navigation-0.3.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-15 15:57:24.000000 general_navigation-0.3.0/tests/test_base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 22:26:55.441274 general_navigation-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-15 22:26:44.000000 general_navigation-0.3.1/Containerfile
+-rw-r--r--   0 runner    (1001) docker     (127)     5073 2024-05-15 22:26:44.000000 general_navigation-0.3.1/HISTORY.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-15 22:26:44.000000 general_navigation-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-15 22:26:44.000000 general_navigation-0.3.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4283 2024-05-15 22:26:55.441274 general_navigation-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3057 2024-05-15 22:26:44.000000 general_navigation-0.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 22:26:55.393274 general_navigation-0.3.1/general_navigation/
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-15 22:26:44.000000 general_navigation-0.3.1/general_navigation/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 22:26:44.000000 general_navigation-0.3.1/general_navigation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      555 2024-05-15 22:26:44.000000 general_navigation-0.3.1/general_navigation/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      356 2024-05-15 22:26:44.000000 general_navigation-0.3.1/general_navigation/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 22:26:55.397274 general_navigation-0.3.1/general_navigation/carla/
+-rw-r--r--   0 runner    (1001) docker     (127)     4327 2024-05-15 22:26:44.000000 general_navigation-0.3.1/general_navigation/carla/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    90254 2024-05-15 22:26:44.000000 general_navigation-0.3.1/general_navigation/carla/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7283 2024-05-15 22:26:44.000000 general_navigation-0.3.1/general_navigation/carla_run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2773 2024-05-15 22:26:44.000000 general_navigation-0.3.1/general_navigation/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      579 2024-05-15 22:26:44.000000 general_navigation-0.3.1/general_navigation/common.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 22:26:55.397274 general_navigation-0.3.1/general_navigation/diffusion_policy/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 22:26:44.000000 general_navigation-0.3.1/general_navigation/diffusion_policy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 22:26:55.397274 general_navigation-0.3.1/general_navigation/diffusion_policy/codecs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 22:26:44.000000 general_navigation-0.3.1/general_navigation/diffusion_policy/codecs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40655 2024-05-15 22:26:44.000000 general_navigation-0.3.1/general_navigation/diffusion_policy/codecs/imagecodecs_numcodecs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 22:26:55.401274 general_navigation-0.3.1/general_navigation/diffusion_policy/common/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 22:26:44.000000 general_navigation-0.3.1/general_navigation/diffusion_policy/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1693 2024-05-15 22:26:44.000000 general_navigation-0.3.1/general_navigation/diffusion_policy/common/checkpoint_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4122 2024-05-15 22:26:44.000000 general_navigation-0.3.1/general_navigation/diffusion_policy/common/cv2_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      739 2024-05-15 22:26:44.000000 general_navigation-0.3.1/general_navigation/diffusion_policy/common/env_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3701 2024-05-15 22:26:44.000000 general_navigation-0.3.1/general_navigation/diffusion_policy/common/json_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)      757 2024-05-15 22:26:44.000000 general_navigation-0.3.1/general_navigation/diffusion_policy/common/nested_dict_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7738 2024-05-15 22:26:44.000000 general_navigation-0.3.1/general_navigation/diffusion_policy/common/normalize_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7321 2024-05-15 22:26:44.000000 general_navigation-0.3.1/general_navigation/diffusion_policy/common/pose_trajectory_interpolator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-05-15 22:26:44.000000 general_navigation-0.3.1/general_navigation/diffusion_policy/common/precise_sleep.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8597 2024-05-15 22:26:44.000000 general_navigation-0.3.1/general_navigation/diffusion_policy/common/pymunk_override.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-05-15 22:26:44.000000 general_navigation-0.3.1/general_navigation/diffusion_policy/common/pymunk_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2682 2024-05-15 22:26:44.000000 general_navigation-0.3.1/general_navigation/diffusion_policy/common/pytorch_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21166 2024-05-15 22:26:44.000000 general_navigation-0.3.1/general_navigation/diffusion_policy/common/replay_buffer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1577 2024-05-15 22:26:44.000000 general_navigation-0.3.1/general_navigation/diffusion_policy/common/robomimic_config_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6543 2024-05-15 22:26:44.000000 general_navigation-0.3.1/general_navigation/diffusion_policy/common/robomimic_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6308 2024-05-15 22:26:44.000000 general_navigation-0.3.1/general_navigation/diffusion_policy/common/sampler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7856 2024-05-15 22:26:44.000000 general_navigation-0.3.1/general_navigation/diffusion_policy/common/timestamp_accumulator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 22:26:55.405274 general_navigation-0.3.1/general_navigation/diffusion_policy/config/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 22:26:44.000000 general_navigation-0.3.1/general_navigation/diffusion_policy/config/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 22:26:55.409274 general_navigation-0.3.1/general_navigation/diffusion_policy/config/task/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 22:26:44.000000 general_navigation-0.3.1/general_navigation/diffusion_policy/config/task/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      902 2024-05-15 22:26:44.000000 general_navigation-0.3.1/general_navigation/diffusion_policy/config/task/blockpush_lowdim_seed.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      909 2024-05-15 22:26:44.000000 general_navigation-0.3.1/general_navigation/diffusion_policy/config/task/blockpush_lowdim_seed_abs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1788 2024-05-15 22:26:44.000000 general_navigation-0.3.1/general_navigation/diffusion_policy/config/task/can_image.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1792 2024-05-15 22:26:44.000000 general_navigation-0.3.1/general_navigation/diffusion_policy/config/task/can_image_abs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1380 2024-05-15 22:26:44.000000 general_navigation-0.3.1/general_navigation/diffusion_policy/config/task/can_lowdim.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1412 2024-05-15 22:26:44.000000 general_navigation-0.3.1/general_navigation/diffusion_policy/config/task/can_lowdim_abs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      798 2024-05-15 22:26:44.000000 general_navigation-0.3.1/general_navigation/diffusion_policy/config/task/kitchen_lowdim.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      990 2024-05-15 22:26:44.000000 general_navigation-0.3.1/general_navigation/diffusion_policy/config/task/kitchen_lowdim_abs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1790 2024-05-15 22:26:44.000000 general_navigation-0.3.1/general_navigation/diffusion_policy/config/task/lift_image.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1772 2024-05-15 22:26:44.000000 general_navigation-0.3.1/general_navigation/diffusion_policy/config/task/lift_image_abs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1407 2024-05-15 22:26:44.000000 general_navigation-0.3.1/general_navigation/diffusion_policy/config/task/lift_lowdim.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1439 2024-05-15 22:26:44.000000 general_navigation-0.3.1/general_navigation/diffusion_policy/config/task/lift_lowdim_abs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      948 2024-05-15 22:26:44.000000 general_navigation-0.3.1/general_navigation/diffusion_policy/config/task/pusht_image.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      918 2024-05-15 22:26:44.000000 general_navigation-0.3.1/general_navigation/diffusion_policy/config/task/pusht_lowdim.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-05-15 22:26:44.000000 general_navigation-0.3.1/general_navigation/diffusion_policy/config/task/real_pusht_image.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1794 2024-05-15 22:26:44.000000 general_navigation-0.3.1/general_navigation/diffusion_policy/config/task/square_image.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1798 2024-05-15 22:26:44.000000 general_navigation-0.3.1/general_navigation/diffusion_policy/config/task/square_image_abs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1413 2024-05-15 22:26:44.000000 general_navigation-0.3.1/general_navigation/diffusion_policy/config/task/square_lowdim.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-05-15 22:26:44.000000 general_navigation-0.3.1/general_navigation/diffusion_policy/config/task/square_lowdim_abs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-05-15 22:26:44.000000 general_navigation-0.3.1/general_navigation/diffusion_policy/config/task/tool_hang_image.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1680 2024-05-15 22:26:44.000000 general_navigation-0.3.1/general_navigation/diffusion_policy/config/task/tool_hang_image_abs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1307 2024-05-15 22:26:44.000000 general_navigation-0.3.1/general_navigation/diffusion_policy/config/task/tool_hang_lowdim.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-05-15 22:26:44.000000 general_navigation-0.3.1/general_navigation/diffusion_policy/config/task/tool_hang_lowdim_abs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1947 2024-05-15 22:26:44.000000 general_navigation-0.3.1/general_navigation/diffusion_policy/config/task/transport_image.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1950 2024-05-15 22:26:44.000000 general_navigation-0.3.1/general_navigation/diffusion_policy/config/task/transport_image_abs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1416 2024-05-15 22:26:44.000000 general_navigation-0.3.1/general_navigation/diffusion_policy/config/task/transport_lowdim.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-05-15 22:26:44.000000 general_navigation-0.3.1/general_navigation/diffusion_policy/config/task/transport_lowdim_abs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3043 2024-05-15 22:26:44.000000 general_navigation-0.3.1/general_navigation/diffusion_policy/config/train_bet_lowdim_workspace.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3503 2024-05-15 22:26:44.000000 general_navigation-0.3.1/general_navigation/diffusion_policy/config/train_diffusion_transformer_hybrid_workspace.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3766 2024-05-15 22:26:44.000000 general_navigation-0.3.1/general_navigation/diffusion_policy/config/train_diffusion_transformer_lowdim_kitchen_workspace.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3761 2024-05-15 22:26:44.000000 general_navigation-0.3.1/general_navigation/diffusion_policy/config/train_diffusion_transformer_lowdim_pusht_workspace.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3768 2024-05-15 22:26:44.000000 general_navigation-0.3.1/general_navigation/diffusion_policy/config/train_diffusion_transformer_lowdim_workspace.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3482 2024-05-15 22:26:44.000000 general_navigation-0.3.1/general_navigation/diffusion_policy/config/train_diffusion_transformer_real_hybrid_workspace.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3301 2024-05-15 22:26:44.000000 general_navigation-0.3.1/general_navigation/diffusion_policy/config/train_diffusion_unet_ddim_hybrid_workspace.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3763 2024-05-15 22:26:44.000000 general_navigation-0.3.1/general_navigation/diffusion_policy/config/train_diffusion_unet_ddim_lowdim_workspace.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3331 2024-05-15 22:26:44.000000 general_navigation-0.3.1/general_navigation/diffusion_policy/config/train_diffusion_unet_hybrid_workspace.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3732 2024-05-15 22:26:44.000000 general_navigation-0.3.1/general_navigation/diffusion_policy/config/train_diffusion_unet_image_pretrained_workspace.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3733 2024-05-15 22:26:44.000000 general_navigation-0.3.1/general_navigation/diffusion_policy/config/train_diffusion_unet_image_workspace.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3789 2024-05-15 22:26:44.000000 general_navigation-0.3.1/general_navigation/diffusion_policy/config/train_diffusion_unet_lowdim_workspace.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3345 2024-05-15 22:26:44.000000 general_navigation-0.3.1/general_navigation/diffusion_policy/config/train_diffusion_unet_real_hybrid_workspace.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3694 2024-05-15 22:26:44.000000 general_navigation-0.3.1/general_navigation/diffusion_policy/config/train_diffusion_unet_real_image_workspace.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3684 2024-05-15 22:26:44.000000 general_navigation-0.3.1/general_navigation/diffusion_policy/config/train_diffusion_unet_real_pretrained_workspace.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3145 2024-05-15 22:26:44.000000 general_navigation-0.3.1/general_navigation/diffusion_policy/config/train_diffusion_unet_video_workspace.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2464 2024-05-15 22:26:44.000000 general_navigation-0.3.1/general_navigation/diffusion_policy/config/train_ibc_dfo_hybrid_workspace.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2423 2024-05-15 22:26:44.000000 general_navigation-0.3.1/general_navigation/diffusion_policy/config/train_ibc_dfo_lowdim_workspace.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2482 2024-05-15 22:26:44.000000 general_navigation-0.3.1/general_navigation/diffusion_policy/config/train_ibc_dfo_real_hybrid_workspace.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-05-15 22:26:44.000000 general_navigation-0.3.1/general_navigation/diffusion_policy/config/train_robomimic_image_workspace.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2166 2024-05-15 22:26:44.000000 general_navigation-0.3.1/general_navigation/diffusion_policy/config/train_robomimic_lowdim_workspace.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2140 2024-05-15 22:26:44.000000 general_navigation-0.3.1/general_navigation/diffusion_policy/config/train_robomimic_real_image_workspace.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 22:26:55.413274 general_navigation-0.3.1/general_navigation/diffusion_policy/dataset/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 22:26:44.000000 general_navigation-0.3.1/general_navigation/diffusion_policy/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1397 2024-05-15 22:26:44.000000 general_navigation-0.3.1/general_navigation/diffusion_policy/dataset/base_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4796 2024-05-15 22:26:44.000000 general_navigation-0.3.1/general_navigation/diffusion_policy/dataset/blockpush_lowdim_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3257 2024-05-15 22:26:44.000000 general_navigation-0.3.1/general_navigation/diffusion_policy/dataset/kitchen_lowdim_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5041 2024-05-15 22:26:44.000000 general_navigation-0.3.1/general_navigation/diffusion_policy/dataset/kitchen_mjl_lowdim_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3302 2024-05-15 22:26:44.000000 general_navigation-0.3.1/general_navigation/diffusion_policy/dataset/pusht_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3761 2024-05-15 22:26:44.000000 general_navigation-0.3.1/general_navigation/diffusion_policy/dataset/pusht_image_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10891 2024-05-15 22:26:44.000000 general_navigation-0.3.1/general_navigation/diffusion_policy/dataset/real_pusht_image_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15410 2024-05-15 22:26:44.000000 general_navigation-0.3.1/general_navigation/diffusion_policy/dataset/robomimic_replay_image_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6096 2024-05-15 22:26:44.000000 general_navigation-0.3.1/general_navigation/diffusion_policy/dataset/robomimic_replay_lowdim_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 22:26:55.413274 general_navigation-0.3.1/general_navigation/diffusion_policy/env_runner/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 22:26:44.000000 general_navigation-0.3.1/general_navigation/diffusion_policy/env_runner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      310 2024-05-15 22:26:44.000000 general_navigation-0.3.1/general_navigation/diffusion_policy/env_runner/base_image_runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-05-15 22:26:44.000000 general_navigation-0.3.1/general_navigation/diffusion_policy/env_runner/base_lowdim_runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11343 2024-05-15 22:26:44.000000 general_navigation-0.3.1/general_navigation/diffusion_policy/env_runner/blockpush_lowdim_runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13030 2024-05-15 22:26:44.000000 general_navigation-0.3.1/general_navigation/diffusion_policy/env_runner/kitchen_lowdim_runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9438 2024-05-15 22:26:44.000000 general_navigation-0.3.1/general_navigation/diffusion_policy/env_runner/pusht_image_runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10627 2024-05-15 22:26:44.000000 general_navigation-0.3.1/general_navigation/diffusion_policy/env_runner/pusht_keypoints_runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-05-15 22:26:44.000000 general_navigation-0.3.1/general_navigation/diffusion_policy/env_runner/real_pusht_image_runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14287 2024-05-15 22:26:44.000000 general_navigation-0.3.1/general_navigation/diffusion_policy/env_runner/robomimic_image_runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13686 2024-05-15 22:26:44.000000 general_navigation-0.3.1/general_navigation/diffusion_policy/env_runner/robomimic_lowdim_runner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 22:26:55.413274 general_navigation-0.3.1/general_navigation/diffusion_policy/gym_util/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 22:26:44.000000 general_navigation-0.3.1/general_navigation/diffusion_policy/gym_util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25848 2024-05-15 22:26:44.000000 general_navigation-0.3.1/general_navigation/diffusion_policy/gym_util/async_vector_env.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4967 2024-05-15 22:26:44.000000 general_navigation-0.3.1/general_navigation/diffusion_policy/gym_util/multistep_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6519 2024-05-15 22:26:44.000000 general_navigation-0.3.1/general_navigation/diffusion_policy/gym_util/sync_vector_env.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-05-15 22:26:44.000000 general_navigation-0.3.1/general_navigation/diffusion_policy/gym_util/video_recording_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-05-15 22:26:44.000000 general_navigation-0.3.1/general_navigation/diffusion_policy/gym_util/video_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 22:26:55.413274 general_navigation-0.3.1/general_navigation/diffusion_policy/model/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 22:26:44.000000 general_navigation-0.3.1/general_navigation/diffusion_policy/model/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 22:26:55.413274 general_navigation-0.3.1/general_navigation/diffusion_policy/model/bet/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 22:26:44.000000 general_navigation-0.3.1/general_navigation/diffusion_policy/model/bet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 22:26:55.413274 general_navigation-0.3.1/general_navigation/diffusion_policy/model/bet/action_ae/
+-rw-r--r--   0 runner    (1001) docker     (127)     1818 2024-05-15 22:26:44.000000 general_navigation-0.3.1/general_navigation/diffusion_policy/model/bet/action_ae/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 22:26:55.417274 general_navigation-0.3.1/general_navigation/diffusion_policy/model/bet/action_ae/discretizers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 22:26:44.000000 general_navigation-0.3.1/general_navigation/diffusion_policy/model/bet/action_ae/discretizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5611 2024-05-15 22:26:44.000000 general_navigation-0.3.1/general_navigation/diffusion_policy/model/bet/action_ae/discretizers/k_means.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 22:26:55.417274 general_navigation-0.3.1/general_navigation/diffusion_policy/model/bet/latent_generators/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 22:26:44.000000 general_navigation-0.3.1/general_navigation/diffusion_policy/model/bet/latent_generators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2707 2024-05-15 22:26:44.000000 general_navigation-0.3.1/general_navigation/diffusion_policy/model/bet/latent_generators/latent_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7904 2024-05-15 22:26:44.000000 general_navigation-0.3.1/general_navigation/diffusion_policy/model/bet/latent_generators/mingpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4183 2024-05-15 22:26:44.000000 general_navigation-0.3.1/general_navigation/diffusion_policy/model/bet/latent_generators/transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 22:26:55.417274 general_navigation-0.3.1/general_navigation/diffusion_policy/model/bet/libraries/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 22:26:44.000000 general_navigation-0.3.1/general_navigation/diffusion_policy/model/bet/libraries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6109 2024-05-15 22:26:44.000000 general_navigation-0.3.1/general_navigation/diffusion_policy/model/bet/libraries/loss_fn.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 22:26:55.417274 general_navigation-0.3.1/general_navigation/diffusion_policy/model/bet/libraries/mingpt/
+-rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-05-15 22:26:44.000000 general_navigation-0.3.1/general_navigation/diffusion_policy/model/bet/libraries/mingpt/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 22:26:44.000000 general_navigation-0.3.1/general_navigation/diffusion_policy/model/bet/libraries/mingpt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9700 2024-05-15 22:26:44.000000 general_navigation-0.3.1/general_navigation/diffusion_policy/model/bet/libraries/mingpt/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6178 2024-05-15 22:26:44.000000 general_navigation-0.3.1/general_navigation/diffusion_policy/model/bet/libraries/mingpt/trainer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1747 2024-05-15 22:26:44.000000 general_navigation-0.3.1/general_navigation/diffusion_policy/model/bet/libraries/mingpt/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4108 2024-05-15 22:26:44.000000 general_navigation-0.3.1/general_navigation/diffusion_policy/model/bet/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 22:26:55.417274 general_navigation-0.3.1/general_navigation/diffusion_policy/model/common/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 22:26:44.000000 general_navigation-0.3.1/general_navigation/diffusion_policy/model/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1441 2024-05-15 22:26:44.000000 general_navigation-0.3.1/general_navigation/diffusion_policy/model/common/dict_of_tensor_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2088 2024-05-15 22:26:44.000000 general_navigation-0.3.1/general_navigation/diffusion_policy/model/common/lr_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-05-15 22:26:44.000000 general_navigation-0.3.1/general_navigation/diffusion_policy/model/common/module_attr_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12232 2024-05-15 22:26:44.000000 general_navigation-0.3.1/general_navigation/diffusion_policy/model/common/normalizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3345 2024-05-15 22:26:44.000000 general_navigation-0.3.1/general_navigation/diffusion_policy/model/common/rotation_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      624 2024-05-15 22:26:44.000000 general_navigation-0.3.1/general_navigation/diffusion_policy/model/common/shape_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30748 2024-05-15 22:26:44.000000 general_navigation-0.3.1/general_navigation/diffusion_policy/model/common/tensor_util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 22:26:55.421274 general_navigation-0.3.1/general_navigation/diffusion_policy/model/diffusion/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 22:26:44.000000 general_navigation-0.3.1/general_navigation/diffusion_policy/model/diffusion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10423 2024-05-15 22:26:44.000000 general_navigation-0.3.1/general_navigation/diffusion_policy/model/diffusion/conditional_unet1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-05-15 22:26:44.000000 general_navigation-0.3.1/general_navigation/diffusion_policy/model/diffusion/conv1d_components.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3419 2024-05-15 22:26:44.000000 general_navigation-0.3.1/general_navigation/diffusion_policy/model/diffusion/ema_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8615 2024-05-15 22:26:44.000000 general_navigation-0.3.1/general_navigation/diffusion_policy/model/diffusion/mask_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2024-05-15 22:26:44.000000 general_navigation-0.3.1/general_navigation/diffusion_policy/model/diffusion/positional_embedding.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15364 2024-05-15 22:26:44.000000 general_navigation-0.3.1/general_navigation/diffusion_policy/model/diffusion/transformer_for_diffusion.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 22:26:55.421274 general_navigation-0.3.1/general_navigation/diffusion_policy/model/vision/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 22:26:44.000000 general_navigation-0.3.1/general_navigation/diffusion_policy/model/vision/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13222 2024-05-15 22:26:44.000000 general_navigation-0.3.1/general_navigation/diffusion_policy/model/vision/crop_randomizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      720 2024-05-15 22:26:44.000000 general_navigation-0.3.1/general_navigation/diffusion_policy/model/vision/model_getter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7723 2024-05-15 22:26:44.000000 general_navigation-0.3.1/general_navigation/diffusion_policy/model/vision/multi_image_obs_encoder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 22:26:55.425274 general_navigation-0.3.1/general_navigation/diffusion_policy/policy/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 22:26:44.000000 general_navigation-0.3.1/general_navigation/diffusion_policy/policy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      888 2024-05-15 22:26:44.000000 general_navigation-0.3.1/general_navigation/diffusion_policy/policy/base_image_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-05-15 22:26:44.000000 general_navigation-0.3.1/general_navigation/diffusion_policy/policy/base_lowdim_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5093 2024-05-15 22:26:44.000000 general_navigation-0.3.1/general_navigation/diffusion_policy/policy/bet_lowdim_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14218 2024-05-15 22:26:44.000000 general_navigation-0.3.1/general_navigation/diffusion_policy/policy/diffusion_transformer_hybrid_image_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8310 2024-05-15 22:26:44.000000 general_navigation-0.3.1/general_navigation/diffusion_policy/policy/diffusion_transformer_lowdim_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13506 2024-05-15 22:26:44.000000 general_navigation-0.3.1/general_navigation/diffusion_policy/policy/diffusion_unet_hybrid_image_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9968 2024-05-15 22:26:44.000000 general_navigation-0.3.1/general_navigation/diffusion_policy/policy/diffusion_unet_image_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9545 2024-05-15 22:26:44.000000 general_navigation-0.3.1/general_navigation/diffusion_policy/policy/diffusion_unet_lowdim_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11716 2024-05-15 22:26:44.000000 general_navigation-0.3.1/general_navigation/diffusion_policy/policy/diffusion_unet_video_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13029 2024-05-15 22:26:44.000000 general_navigation-0.3.1/general_navigation/diffusion_policy/policy/ibc_dfo_hybrid_image_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8532 2024-05-15 22:26:44.000000 general_navigation-0.3.1/general_navigation/diffusion_policy/policy/ibc_dfo_lowdim_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4940 2024-05-15 22:26:44.000000 general_navigation-0.3.1/general_navigation/diffusion_policy/policy/robomimic_image_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3163 2024-05-15 22:26:44.000000 general_navigation-0.3.1/general_navigation/diffusion_policy/policy/robomimic_lowdim_policy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 22:26:55.425274 general_navigation-0.3.1/general_navigation/diffusion_policy/real_world/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 22:26:44.000000 general_navigation-0.3.1/general_navigation/diffusion_policy/real_world/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-05-15 22:26:44.000000 general_navigation-0.3.1/general_navigation/diffusion_policy/real_world/keystroke_counter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2326 2024-05-15 22:26:44.000000 general_navigation-0.3.1/general_navigation/diffusion_policy/real_world/multi_camera_visualizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7900 2024-05-15 22:26:44.000000 general_navigation-0.3.1/general_navigation/diffusion_policy/real_world/multi_realsense.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8789 2024-05-15 22:26:44.000000 general_navigation-0.3.1/general_navigation/diffusion_policy/real_world/real_data_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15113 2024-05-15 22:26:44.000000 general_navigation-0.3.1/general_navigation/diffusion_policy/real_world/real_env.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1858 2024-05-15 22:26:44.000000 general_navigation-0.3.1/general_navigation/diffusion_policy/real_world/real_inference_util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 22:26:55.425274 general_navigation-0.3.1/general_navigation/diffusion_policy/real_world/realsense_config/
+-rw-r--r--   0 runner    (1001) docker     (127)     3537 2024-05-15 22:26:44.000000 general_navigation-0.3.1/general_navigation/diffusion_policy/real_world/realsense_config/415_high_accuracy_mode.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3434 2024-05-15 22:26:44.000000 general_navigation-0.3.1/general_navigation/diffusion_policy/real_world/realsense_config/435_high_accuracy_mode.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 22:26:44.000000 general_navigation-0.3.1/general_navigation/diffusion_policy/real_world/realsense_config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13197 2024-05-15 22:26:44.000000 general_navigation-0.3.1/general_navigation/diffusion_policy/real_world/rtde_interpolation_controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19065 2024-05-15 22:26:44.000000 general_navigation-0.3.1/general_navigation/diffusion_policy/real_world/single_realsense.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3183 2024-05-15 22:26:44.000000 general_navigation-0.3.1/general_navigation/diffusion_policy/real_world/spacemouse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5258 2024-05-15 22:26:44.000000 general_navigation-0.3.1/general_navigation/diffusion_policy/real_world/spacemouse_shared_memory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5029 2024-05-15 22:26:44.000000 general_navigation-0.3.1/general_navigation/diffusion_policy/real_world/video_recorder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 22:26:55.429274 general_navigation-0.3.1/general_navigation/diffusion_policy/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 22:26:44.000000 general_navigation-0.3.1/general_navigation/diffusion_policy/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1426 2024-05-15 22:26:44.000000 general_navigation-0.3.1/general_navigation/diffusion_policy/scripts/bet_blockpush_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (127)      876 2024-05-15 22:26:44.000000 general_navigation-0.3.1/general_navigation/diffusion_policy/scripts/blockpush_abs_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (127)      705 2024-05-15 22:26:44.000000 general_navigation-0.3.1/general_navigation/diffusion_policy/scripts/episode_lengths.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2212 2024-05-15 22:26:44.000000 general_navigation-0.3.1/general_navigation/diffusion_policy/scripts/generate_bet_blockpush.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1918 2024-05-15 22:26:44.000000 general_navigation-0.3.1/general_navigation/diffusion_policy/scripts/real_dataset_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4679 2024-05-15 22:26:44.000000 general_navigation-0.3.1/general_navigation/diffusion_policy/scripts/real_pusht_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2391 2024-05-15 22:26:44.000000 general_navigation-0.3.1/general_navigation/diffusion_policy/scripts/real_pusht_successrate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1647 2024-05-15 22:26:44.000000 general_navigation-0.3.1/general_navigation/diffusion_policy/scripts/robomimic_dataset_action_comparison.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3337 2024-05-15 22:26:44.000000 general_navigation-0.3.1/general_navigation/diffusion_policy/scripts/robomimic_dataset_conversion.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 22:26:55.429274 general_navigation-0.3.1/general_navigation/diffusion_policy/shared_memory/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 22:26:44.000000 general_navigation-0.3.1/general_navigation/diffusion_policy/shared_memory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5830 2024-05-15 22:26:44.000000 general_navigation-0.3.1/general_navigation/diffusion_policy/shared_memory/shared_memory_queue.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8233 2024-05-15 22:26:44.000000 general_navigation-0.3.1/general_navigation/diffusion_policy/shared_memory/shared_memory_ring_buffer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-05-15 22:26:44.000000 general_navigation-0.3.1/general_navigation/diffusion_policy/shared_memory/shared_memory_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7392 2024-05-15 22:26:44.000000 general_navigation-0.3.1/general_navigation/diffusion_policy/shared_memory/shared_ndarray.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 22:26:55.433274 general_navigation-0.3.1/general_navigation/diffusion_policy/workspace/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 22:26:44.000000 general_navigation-0.3.1/general_navigation/diffusion_policy/workspace/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5135 2024-05-15 22:26:44.000000 general_navigation-0.3.1/general_navigation/diffusion_policy/workspace/base_workspace.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13075 2024-05-15 22:26:44.000000 general_navigation-0.3.1/general_navigation/diffusion_policy/workspace/train_bet_lowdim_workspace.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13128 2024-05-15 22:26:44.000000 general_navigation-0.3.1/general_navigation/diffusion_policy/workspace/train_diffusion_transformer_hybrid_workspace.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13338 2024-05-15 22:26:44.000000 general_navigation-0.3.1/general_navigation/diffusion_policy/workspace/train_diffusion_transformer_lowdim_workspace.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13135 2024-05-15 22:26:44.000000 general_navigation-0.3.1/general_navigation/diffusion_policy/workspace/train_diffusion_unet_hybrid_workspace.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13272 2024-05-15 22:26:44.000000 general_navigation-0.3.1/general_navigation/diffusion_policy/workspace/train_diffusion_unet_image_workspace.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13317 2024-05-15 22:26:44.000000 general_navigation-0.3.1/general_navigation/diffusion_policy/workspace/train_diffusion_unet_lowdim_workspace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9530 2024-05-15 22:26:44.000000 general_navigation-0.3.1/general_navigation/diffusion_policy/workspace/train_diffusion_unet_video_workspace.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12846 2024-05-15 22:26:44.000000 general_navigation-0.3.1/general_navigation/diffusion_policy/workspace/train_ibc_dfo_hybrid_workspace.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12470 2024-05-15 22:26:44.000000 general_navigation-0.3.1/general_navigation/diffusion_policy/workspace/train_ibc_dfo_lowdim_workspace.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11336 2024-05-15 22:26:44.000000 general_navigation-0.3.1/general_navigation/diffusion_policy/workspace/train_robomimic_image_workspace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9621 2024-05-15 22:26:44.000000 general_navigation-0.3.1/general_navigation/diffusion_policy/workspace/train_robomimic_lowdim_workspace.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 22:26:55.433274 general_navigation-0.3.1/general_navigation/gpt/
+-rw-r--r--   0 runner    (1001) docker     (127)     2491 2024-05-15 22:26:44.000000 general_navigation-0.3.1/general_navigation/gpt/gpt_vision.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 22:26:55.433274 general_navigation-0.3.1/general_navigation/models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 22:26:44.000000 general_navigation-0.3.1/general_navigation/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1597 2024-05-15 22:26:44.000000 general_navigation-0.3.1/general_navigation/models/base_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 22:26:55.433274 general_navigation-0.3.1/general_navigation/models/config/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 22:26:44.000000 general_navigation-0.3.1/general_navigation/models/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1292 2024-05-15 22:26:44.000000 general_navigation-0.3.1/general_navigation/models/config/data_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-05-15 22:26:44.000000 general_navigation-0.3.1/general_navigation/models/config/defaults.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3479 2024-05-15 22:26:44.000000 general_navigation-0.3.1/general_navigation/models/config/gnm.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3662 2024-05-15 22:26:44.000000 general_navigation-0.3.1/general_navigation/models/config/late_fusion.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3563 2024-05-15 22:26:44.000000 general_navigation-0.3.1/general_navigation/models/config/nomad.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3651 2024-05-15 22:26:44.000000 general_navigation-0.3.1/general_navigation/models/config/vint.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     5410 2024-05-15 22:26:44.000000 general_navigation-0.3.1/general_navigation/models/factory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 22:26:55.433274 general_navigation-0.3.1/general_navigation/models/gnm/
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-15 22:26:44.000000 general_navigation-0.3.1/general_navigation/models/gnm/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 22:26:44.000000 general_navigation-0.3.1/general_navigation/models/gnm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3616 2024-05-15 22:26:44.000000 general_navigation-0.3.1/general_navigation/models/gnm/gnm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5171 2024-05-15 22:26:44.000000 general_navigation-0.3.1/general_navigation/models/gnm/modified_mobilenetv2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20868 2024-05-15 22:26:44.000000 general_navigation-0.3.1/general_navigation/models/model_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 22:26:55.437274 general_navigation-0.3.1/general_navigation/models/nomad/
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-15 22:26:44.000000 general_navigation-0.3.1/general_navigation/models/nomad/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 22:26:44.000000 general_navigation-0.3.1/general_navigation/models/nomad/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-05-15 22:26:44.000000 general_navigation-0.3.1/general_navigation/models/nomad/nomad.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8480 2024-05-15 22:26:44.000000 general_navigation-0.3.1/general_navigation/models/nomad/nomad_vint.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 22:26:44.000000 general_navigation-0.3.1/general_navigation/models/nomad/vib_placeholder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 22:26:55.437274 general_navigation-0.3.1/general_navigation/models/vint/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 22:26:44.000000 general_navigation-0.3.1/general_navigation/models/vint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2438 2024-05-15 22:26:44.000000 general_navigation-0.3.1/general_navigation/models/vint/self_attention.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7113 2024-05-15 22:26:44.000000 general_navigation-0.3.1/general_navigation/models/vint/vint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8146 2024-05-15 22:26:44.000000 general_navigation-0.3.1/general_navigation/models/vint/vit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4719 2024-05-15 22:26:44.000000 general_navigation-0.3.1/general_navigation/mpc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 22:26:55.437274 general_navigation-0.3.1/general_navigation/schema/
+-rw-r--r--   0 runner    (1001) docker     (127)     1745 2024-05-15 22:26:44.000000 general_navigation-0.3.1/general_navigation/schema/carla.py
+-rw-r--r--   0 runner    (1001) docker     (127)      843 2024-05-15 22:26:44.000000 general_navigation-0.3.1/general_navigation/schema/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-05-15 22:26:44.000000 general_navigation-0.3.1/general_navigation/schema/packet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-15 22:26:44.000000 general_navigation-0.3.1/general_navigation/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 22:26:55.437274 general_navigation-0.3.1/general_navigation/visualizing/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 22:26:44.000000 general_navigation-0.3.1/general_navigation/visualizing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17421 2024-05-15 22:26:44.000000 general_navigation-0.3.1/general_navigation/visualizing/action_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7435 2024-05-15 22:26:44.000000 general_navigation-0.3.1/general_navigation/visualizing/distance_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      625 2024-05-15 22:26:44.000000 general_navigation-0.3.1/general_navigation/visualizing/visualize_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 22:26:55.437274 general_navigation-0.3.1/general_navigation.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4283 2024-05-15 22:26:55.000000 general_navigation-0.3.1/general_navigation.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    15689 2024-05-15 22:26:55.000000 general_navigation-0.3.1/general_navigation.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 22:26:55.000000 general_navigation-0.3.1/general_navigation.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-15 22:26:55.000000 general_navigation-0.3.1/general_navigation.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-05-15 22:26:55.000000 general_navigation-0.3.1/general_navigation.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-15 22:26:55.000000 general_navigation-0.3.1/general_navigation.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 22:26:55.441274 general_navigation-0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-05-15 22:26:44.000000 general_navigation-0.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 22:26:55.437274 general_navigation-0.3.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 22:26:44.000000 general_navigation-0.3.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-05-15 22:26:44.000000 general_navigation-0.3.1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-15 22:26:44.000000 general_navigation-0.3.1/tests/test_base.py
```

### Comparing `general_navigation-0.3.0/HISTORY.md` & `general_navigation-0.3.1/HISTORY.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,19 @@
 Changelog
 =========
 
 
 (unreleased)
 ------------
+- Fix(requirements.txt): relaxed carla requirement. [Aditya NG]
+
+
+0.3.0 (2024-05-15)
+------------------
+- Release: version 0.3.0 🚀 [Aditya NG]
 - Feat(general_navigation/mpc.py): mpc functionality and connect to
   carla. [Aditya NG]
 - Feat(carla): connecting to carla. [Aditya NG]
 
 
 0.2.2 (2024-05-15)
 ------------------
```

### Comparing `general_navigation-0.3.0/LICENSE` & `general_navigation-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `general_navigation-0.3.0/PKG-INFO` & `general_navigation-0.3.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 Metadata-Version: 2.1
 Name: general_navigation
-Version: 0.3.0
+Version: 0.3.1
 Summary: Awesome general_navigation created by AdityaNG
 Home-page: https://github.com/AdityaNG/general-navigation/
 Author: AdityaNG
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: torch>=2.2.2
 Requires-Dist: torchvision>=0.17.2
 Requires-Dist: numpy>=1.24.4
 Requires-Dist: setuptools>=65.5.0
 Requires-Dist: einops>=0.8.0
 Requires-Dist: opencv-python>=4.9.0.80
 Requires-Dist: efficientnet_pytorch==0.7.1
 Requires-Dist: vit-pytorch==1.6.9
 Requires-Dist: pygame==2.5.2
-Requires-Dist: carla==0.9.15
 Requires-Dist: platformdirs
 Requires-Dist: gdown
 Requires-Dist: diffusers
 Requires-Dist: matplotlib
 Requires-Dist: wandb
 Requires-Dist: pydantic
 Requires-Dist: simple-pid==1.0.1
@@ -53,21 +52,29 @@
 
 [PyPi Link](https://pypi.org/project/general-navigation/)
 
 ```bash
 pip install general_navigation
 ```
 
+If you want to connect with the Carla simulator, you will also need to seperately install carla
+```bash
+pip install carla==0.9.15  # Linux and Windows
+pip install carla==0.9.5  # Linux and Windows
+```
+
 ## Usage
 
 [Documentation Link](https://adityang.github.io/general-navigation/)
 
 Creating a pytorch instance of the model
 ```py
-from .models.factory import get_default_config, get_model, get_weights
+from general_navigation.models.factory import (
+  get_default_config, get_model, get_weights
+)
 
 config = get_default_config()
 model = get_model(config)
 model = get_weights(config, model, device)
 ```
 
 Using the command line tool for inference
```

### Comparing `general_navigation-0.3.0/README.md` & `general_navigation-0.3.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -14,21 +14,29 @@
 
 [PyPi Link](https://pypi.org/project/general-navigation/)
 
 ```bash
 pip install general_navigation
 ```
 
+If you want to connect with the Carla simulator, you will also need to seperately install carla
+```bash
+pip install carla==0.9.15  # Linux and Windows
+pip install carla==0.9.5  # Linux and Windows
+```
+
 ## Usage
 
 [Documentation Link](https://adityang.github.io/general-navigation/)
 
 Creating a pytorch instance of the model
 ```py
-from .models.factory import get_default_config, get_model, get_weights
+from general_navigation.models.factory import (
+  get_default_config, get_model, get_weights
+)
 
 config = get_default_config()
 model = get_model(config)
 model = get_weights(config, model, device)
 ```
 
 Using the command line tool for inference
```

### Comparing `general_navigation-0.3.0/general_navigation/__main__.py` & `general_navigation-0.3.1/general_navigation/__main__.py`

 * *Files identical despite different names*

### Comparing `general_navigation-0.3.0/general_navigation/carla/client.py` & `general_navigation-0.3.1/general_navigation/carla/client.py`

 * *Files identical despite different names*

### Comparing `general_navigation-0.3.0/general_navigation/carla/helpers.py` & `general_navigation-0.3.1/general_navigation/carla/helpers.py`

 * *Files identical despite different names*

### Comparing `general_navigation-0.3.0/general_navigation/carla_run.py` & `general_navigation-0.3.1/general_navigation/carla_run.py`

 * *Files identical despite different names*

### Comparing `general_navigation-0.3.0/general_navigation/cli.py` & `general_navigation-0.3.1/general_navigation/cli.py`

 * *Files identical despite different names*

### Comparing `general_navigation-0.3.0/general_navigation/common.py` & `general_navigation-0.3.1/general_navigation/common.py`

 * *Files identical despite different names*

### Comparing `general_navigation-0.3.0/general_navigation/diffusion_policy/codecs/imagecodecs_numcodecs.py` & `general_navigation-0.3.1/general_navigation/diffusion_policy/codecs/imagecodecs_numcodecs.py`

 * *Files identical despite different names*

### Comparing `general_navigation-0.3.0/general_navigation/diffusion_policy/common/checkpoint_util.py` & `general_navigation-0.3.1/general_navigation/diffusion_policy/common/checkpoint_util.py`

 * *Files identical despite different names*

### Comparing `general_navigation-0.3.0/general_navigation/diffusion_policy/common/cv2_util.py` & `general_navigation-0.3.1/general_navigation/diffusion_policy/common/cv2_util.py`

 * *Files identical despite different names*

### Comparing `general_navigation-0.3.0/general_navigation/diffusion_policy/common/env_util.py` & `general_navigation-0.3.1/general_navigation/diffusion_policy/common/env_util.py`

 * *Files identical despite different names*

### Comparing `general_navigation-0.3.0/general_navigation/diffusion_policy/common/json_logger.py` & `general_navigation-0.3.1/general_navigation/diffusion_policy/common/json_logger.py`

 * *Files identical despite different names*

### Comparing `general_navigation-0.3.0/general_navigation/diffusion_policy/common/nested_dict_util.py` & `general_navigation-0.3.1/general_navigation/diffusion_policy/common/nested_dict_util.py`

 * *Files identical despite different names*

### Comparing `general_navigation-0.3.0/general_navigation/diffusion_policy/common/normalize_util.py` & `general_navigation-0.3.1/general_navigation/diffusion_policy/common/normalize_util.py`

 * *Files identical despite different names*

### Comparing `general_navigation-0.3.0/general_navigation/diffusion_policy/common/pose_trajectory_interpolator.py` & `general_navigation-0.3.1/general_navigation/diffusion_policy/common/pose_trajectory_interpolator.py`

 * *Files identical despite different names*

### Comparing `general_navigation-0.3.0/general_navigation/diffusion_policy/common/precise_sleep.py` & `general_navigation-0.3.1/general_navigation/diffusion_policy/common/precise_sleep.py`

 * *Files identical despite different names*

### Comparing `general_navigation-0.3.0/general_navigation/diffusion_policy/common/pymunk_override.py` & `general_navigation-0.3.1/general_navigation/diffusion_policy/common/pymunk_override.py`

 * *Files identical despite different names*

### Comparing `general_navigation-0.3.0/general_navigation/diffusion_policy/common/pymunk_util.py` & `general_navigation-0.3.1/general_navigation/diffusion_policy/common/pymunk_util.py`

 * *Files identical despite different names*

### Comparing `general_navigation-0.3.0/general_navigation/diffusion_policy/common/pytorch_util.py` & `general_navigation-0.3.1/general_navigation/diffusion_policy/common/pytorch_util.py`

 * *Files identical despite different names*

### Comparing `general_navigation-0.3.0/general_navigation/diffusion_policy/common/replay_buffer.py` & `general_navigation-0.3.1/general_navigation/diffusion_policy/common/replay_buffer.py`

 * *Files identical despite different names*

### Comparing `general_navigation-0.3.0/general_navigation/diffusion_policy/common/robomimic_config_util.py` & `general_navigation-0.3.1/general_navigation/diffusion_policy/common/robomimic_config_util.py`

 * *Files identical despite different names*

### Comparing `general_navigation-0.3.0/general_navigation/diffusion_policy/common/robomimic_util.py` & `general_navigation-0.3.1/general_navigation/diffusion_policy/common/robomimic_util.py`

 * *Files identical despite different names*

### Comparing `general_navigation-0.3.0/general_navigation/diffusion_policy/common/sampler.py` & `general_navigation-0.3.1/general_navigation/diffusion_policy/common/sampler.py`

 * *Files identical despite different names*

### Comparing `general_navigation-0.3.0/general_navigation/diffusion_policy/common/timestamp_accumulator.py` & `general_navigation-0.3.1/general_navigation/diffusion_policy/common/timestamp_accumulator.py`

 * *Files identical despite different names*

### Comparing `general_navigation-0.3.0/general_navigation/diffusion_policy/config/task/blockpush_lowdim_seed.yaml` & `general_navigation-0.3.1/general_navigation/diffusion_policy/config/task/blockpush_lowdim_seed.yaml`

 * *Files identical despite different names*

### Comparing `general_navigation-0.3.0/general_navigation/diffusion_policy/config/task/blockpush_lowdim_seed_abs.yaml` & `general_navigation-0.3.1/general_navigation/diffusion_policy/config/task/blockpush_lowdim_seed_abs.yaml`

 * *Files identical despite different names*

### Comparing `general_navigation-0.3.0/general_navigation/diffusion_policy/config/task/can_image.yaml` & `general_navigation-0.3.1/general_navigation/diffusion_policy/config/task/can_image.yaml`

 * *Files identical despite different names*

### Comparing `general_navigation-0.3.0/general_navigation/diffusion_policy/config/task/can_image_abs.yaml` & `general_navigation-0.3.1/general_navigation/diffusion_policy/config/task/can_image_abs.yaml`

 * *Files identical despite different names*

### Comparing `general_navigation-0.3.0/general_navigation/diffusion_policy/config/task/can_lowdim.yaml` & `general_navigation-0.3.1/general_navigation/diffusion_policy/config/task/can_lowdim.yaml`

 * *Files identical despite different names*

### Comparing `general_navigation-0.3.0/general_navigation/diffusion_policy/config/task/can_lowdim_abs.yaml` & `general_navigation-0.3.1/general_navigation/diffusion_policy/config/task/can_lowdim_abs.yaml`

 * *Files identical despite different names*

### Comparing `general_navigation-0.3.0/general_navigation/diffusion_policy/config/task/kitchen_lowdim.yaml` & `general_navigation-0.3.1/general_navigation/diffusion_policy/config/task/kitchen_lowdim.yaml`

 * *Files identical despite different names*

### Comparing `general_navigation-0.3.0/general_navigation/diffusion_policy/config/task/kitchen_lowdim_abs.yaml` & `general_navigation-0.3.1/general_navigation/diffusion_policy/config/task/kitchen_lowdim_abs.yaml`

 * *Files identical despite different names*

### Comparing `general_navigation-0.3.0/general_navigation/diffusion_policy/config/task/lift_image.yaml` & `general_navigation-0.3.1/general_navigation/diffusion_policy/config/task/lift_image.yaml`

 * *Files identical despite different names*

### Comparing `general_navigation-0.3.0/general_navigation/diffusion_policy/config/task/lift_image_abs.yaml` & `general_navigation-0.3.1/general_navigation/diffusion_policy/config/task/lift_image_abs.yaml`

 * *Files identical despite different names*

### Comparing `general_navigation-0.3.0/general_navigation/diffusion_policy/config/task/lift_lowdim.yaml` & `general_navigation-0.3.1/general_navigation/diffusion_policy/config/task/lift_lowdim.yaml`

 * *Files identical despite different names*

### Comparing `general_navigation-0.3.0/general_navigation/diffusion_policy/config/task/lift_lowdim_abs.yaml` & `general_navigation-0.3.1/general_navigation/diffusion_policy/config/task/lift_lowdim_abs.yaml`

 * *Files identical despite different names*

### Comparing `general_navigation-0.3.0/general_navigation/diffusion_policy/config/task/pusht_image.yaml` & `general_navigation-0.3.1/general_navigation/diffusion_policy/config/task/pusht_image.yaml`

 * *Files identical despite different names*

### Comparing `general_navigation-0.3.0/general_navigation/diffusion_policy/config/task/pusht_lowdim.yaml` & `general_navigation-0.3.1/general_navigation/diffusion_policy/config/task/pusht_lowdim.yaml`

 * *Files identical despite different names*

### Comparing `general_navigation-0.3.0/general_navigation/diffusion_policy/config/task/real_pusht_image.yaml` & `general_navigation-0.3.1/general_navigation/diffusion_policy/config/task/real_pusht_image.yaml`

 * *Files identical despite different names*

### Comparing `general_navigation-0.3.0/general_navigation/diffusion_policy/config/task/square_image.yaml` & `general_navigation-0.3.1/general_navigation/diffusion_policy/config/task/square_image.yaml`

 * *Files identical despite different names*

### Comparing `general_navigation-0.3.0/general_navigation/diffusion_policy/config/task/square_image_abs.yaml` & `general_navigation-0.3.1/general_navigation/diffusion_policy/config/task/square_image_abs.yaml`

 * *Files identical despite different names*

### Comparing `general_navigation-0.3.0/general_navigation/diffusion_policy/config/task/square_lowdim.yaml` & `general_navigation-0.3.1/general_navigation/diffusion_policy/config/task/square_lowdim.yaml`

 * *Files identical despite different names*

### Comparing `general_navigation-0.3.0/general_navigation/diffusion_policy/config/task/square_lowdim_abs.yaml` & `general_navigation-0.3.1/general_navigation/diffusion_policy/config/task/square_lowdim_abs.yaml`

 * *Files identical despite different names*

### Comparing `general_navigation-0.3.0/general_navigation/diffusion_policy/config/task/tool_hang_image.yaml` & `general_navigation-0.3.1/general_navigation/diffusion_policy/config/task/tool_hang_image.yaml`

 * *Files identical despite different names*

### Comparing `general_navigation-0.3.0/general_navigation/diffusion_policy/config/task/tool_hang_image_abs.yaml` & `general_navigation-0.3.1/general_navigation/diffusion_policy/config/task/tool_hang_image_abs.yaml`

 * *Files identical despite different names*

### Comparing `general_navigation-0.3.0/general_navigation/diffusion_policy/config/task/tool_hang_lowdim.yaml` & `general_navigation-0.3.1/general_navigation/diffusion_policy/config/task/tool_hang_lowdim.yaml`

 * *Files identical despite different names*

### Comparing `general_navigation-0.3.0/general_navigation/diffusion_policy/config/task/tool_hang_lowdim_abs.yaml` & `general_navigation-0.3.1/general_navigation/diffusion_policy/config/task/tool_hang_lowdim_abs.yaml`

 * *Files identical despite different names*

### Comparing `general_navigation-0.3.0/general_navigation/diffusion_policy/config/task/transport_image.yaml` & `general_navigation-0.3.1/general_navigation/diffusion_policy/config/task/transport_image.yaml`

 * *Files identical despite different names*

### Comparing `general_navigation-0.3.0/general_navigation/diffusion_policy/config/task/transport_image_abs.yaml` & `general_navigation-0.3.1/general_navigation/diffusion_policy/config/task/transport_image_abs.yaml`

 * *Files identical despite different names*

### Comparing `general_navigation-0.3.0/general_navigation/diffusion_policy/config/task/transport_lowdim.yaml` & `general_navigation-0.3.1/general_navigation/diffusion_policy/config/task/transport_lowdim.yaml`

 * *Files identical despite different names*

### Comparing `general_navigation-0.3.0/general_navigation/diffusion_policy/config/task/transport_lowdim_abs.yaml` & `general_navigation-0.3.1/general_navigation/diffusion_policy/config/task/transport_lowdim_abs.yaml`

 * *Files identical despite different names*

### Comparing `general_navigation-0.3.0/general_navigation/diffusion_policy/config/train_bet_lowdim_workspace.yaml` & `general_navigation-0.3.1/general_navigation/diffusion_policy/config/train_bet_lowdim_workspace.yaml`

 * *Files identical despite different names*

### Comparing `general_navigation-0.3.0/general_navigation/diffusion_policy/config/train_diffusion_transformer_hybrid_workspace.yaml` & `general_navigation-0.3.1/general_navigation/diffusion_policy/config/train_diffusion_transformer_hybrid_workspace.yaml`

 * *Files identical despite different names*

### Comparing `general_navigation-0.3.0/general_navigation/diffusion_policy/config/train_diffusion_transformer_lowdim_kitchen_workspace.yaml` & `general_navigation-0.3.1/general_navigation/diffusion_policy/config/train_diffusion_transformer_lowdim_kitchen_workspace.yaml`

 * *Files identical despite different names*

### Comparing `general_navigation-0.3.0/general_navigation/diffusion_policy/config/train_diffusion_transformer_lowdim_pusht_workspace.yaml` & `general_navigation-0.3.1/general_navigation/diffusion_policy/config/train_diffusion_transformer_lowdim_pusht_workspace.yaml`

 * *Files identical despite different names*

### Comparing `general_navigation-0.3.0/general_navigation/diffusion_policy/config/train_diffusion_transformer_lowdim_workspace.yaml` & `general_navigation-0.3.1/general_navigation/diffusion_policy/config/train_diffusion_transformer_lowdim_workspace.yaml`

 * *Files identical despite different names*

### Comparing `general_navigation-0.3.0/general_navigation/diffusion_policy/config/train_diffusion_transformer_real_hybrid_workspace.yaml` & `general_navigation-0.3.1/general_navigation/diffusion_policy/config/train_diffusion_transformer_real_hybrid_workspace.yaml`

 * *Files identical despite different names*

### Comparing `general_navigation-0.3.0/general_navigation/diffusion_policy/config/train_diffusion_unet_ddim_hybrid_workspace.yaml` & `general_navigation-0.3.1/general_navigation/diffusion_policy/config/train_diffusion_unet_ddim_hybrid_workspace.yaml`

 * *Files identical despite different names*

### Comparing `general_navigation-0.3.0/general_navigation/diffusion_policy/config/train_diffusion_unet_ddim_lowdim_workspace.yaml` & `general_navigation-0.3.1/general_navigation/diffusion_policy/config/train_diffusion_unet_ddim_lowdim_workspace.yaml`

 * *Files identical despite different names*

### Comparing `general_navigation-0.3.0/general_navigation/diffusion_policy/config/train_diffusion_unet_hybrid_workspace.yaml` & `general_navigation-0.3.1/general_navigation/diffusion_policy/config/train_diffusion_unet_hybrid_workspace.yaml`

 * *Files identical despite different names*

### Comparing `general_navigation-0.3.0/general_navigation/diffusion_policy/config/train_diffusion_unet_image_pretrained_workspace.yaml` & `general_navigation-0.3.1/general_navigation/diffusion_policy/config/train_diffusion_unet_image_pretrained_workspace.yaml`

 * *Files identical despite different names*

### Comparing `general_navigation-0.3.0/general_navigation/diffusion_policy/config/train_diffusion_unet_image_workspace.yaml` & `general_navigation-0.3.1/general_navigation/diffusion_policy/config/train_diffusion_unet_image_workspace.yaml`

 * *Files identical despite different names*

### Comparing `general_navigation-0.3.0/general_navigation/diffusion_policy/config/train_diffusion_unet_lowdim_workspace.yaml` & `general_navigation-0.3.1/general_navigation/diffusion_policy/config/train_diffusion_unet_lowdim_workspace.yaml`

 * *Files identical despite different names*

### Comparing `general_navigation-0.3.0/general_navigation/diffusion_policy/config/train_diffusion_unet_real_hybrid_workspace.yaml` & `general_navigation-0.3.1/general_navigation/diffusion_policy/config/train_diffusion_unet_real_hybrid_workspace.yaml`

 * *Files identical despite different names*

### Comparing `general_navigation-0.3.0/general_navigation/diffusion_policy/config/train_diffusion_unet_real_image_workspace.yaml` & `general_navigation-0.3.1/general_navigation/diffusion_policy/config/train_diffusion_unet_real_image_workspace.yaml`

 * *Files identical despite different names*

### Comparing `general_navigation-0.3.0/general_navigation/diffusion_policy/config/train_diffusion_unet_real_pretrained_workspace.yaml` & `general_navigation-0.3.1/general_navigation/diffusion_policy/config/train_diffusion_unet_real_pretrained_workspace.yaml`

 * *Files identical despite different names*

### Comparing `general_navigation-0.3.0/general_navigation/diffusion_policy/config/train_diffusion_unet_video_workspace.yaml` & `general_navigation-0.3.1/general_navigation/diffusion_policy/config/train_diffusion_unet_video_workspace.yaml`

 * *Files identical despite different names*

### Comparing `general_navigation-0.3.0/general_navigation/diffusion_policy/config/train_ibc_dfo_hybrid_workspace.yaml` & `general_navigation-0.3.1/general_navigation/diffusion_policy/config/train_ibc_dfo_hybrid_workspace.yaml`

 * *Files identical despite different names*

### Comparing `general_navigation-0.3.0/general_navigation/diffusion_policy/config/train_ibc_dfo_lowdim_workspace.yaml` & `general_navigation-0.3.1/general_navigation/diffusion_policy/config/train_ibc_dfo_lowdim_workspace.yaml`

 * *Files identical despite different names*

### Comparing `general_navigation-0.3.0/general_navigation/diffusion_policy/config/train_ibc_dfo_real_hybrid_workspace.yaml` & `general_navigation-0.3.1/general_navigation/diffusion_policy/config/train_ibc_dfo_real_hybrid_workspace.yaml`

 * *Files identical despite different names*

### Comparing `general_navigation-0.3.0/general_navigation/diffusion_policy/config/train_robomimic_image_workspace.yaml` & `general_navigation-0.3.1/general_navigation/diffusion_policy/config/train_robomimic_image_workspace.yaml`

 * *Files identical despite different names*

### Comparing `general_navigation-0.3.0/general_navigation/diffusion_policy/config/train_robomimic_lowdim_workspace.yaml` & `general_navigation-0.3.1/general_navigation/diffusion_policy/config/train_robomimic_lowdim_workspace.yaml`

 * *Files identical despite different names*

### Comparing `general_navigation-0.3.0/general_navigation/diffusion_policy/config/train_robomimic_real_image_workspace.yaml` & `general_navigation-0.3.1/general_navigation/diffusion_policy/config/train_robomimic_real_image_workspace.yaml`

 * *Files identical despite different names*

### Comparing `general_navigation-0.3.0/general_navigation/diffusion_policy/dataset/base_dataset.py` & `general_navigation-0.3.1/general_navigation/diffusion_policy/dataset/base_dataset.py`

 * *Files identical despite different names*

### Comparing `general_navigation-0.3.0/general_navigation/diffusion_policy/dataset/blockpush_lowdim_dataset.py` & `general_navigation-0.3.1/general_navigation/diffusion_policy/dataset/blockpush_lowdim_dataset.py`

 * *Files identical despite different names*

### Comparing `general_navigation-0.3.0/general_navigation/diffusion_policy/dataset/kitchen_lowdim_dataset.py` & `general_navigation-0.3.1/general_navigation/diffusion_policy/dataset/kitchen_lowdim_dataset.py`

 * *Files identical despite different names*

### Comparing `general_navigation-0.3.0/general_navigation/diffusion_policy/dataset/kitchen_mjl_lowdim_dataset.py` & `general_navigation-0.3.1/general_navigation/diffusion_policy/dataset/kitchen_mjl_lowdim_dataset.py`

 * *Files identical despite different names*

### Comparing `general_navigation-0.3.0/general_navigation/diffusion_policy/dataset/pusht_dataset.py` & `general_navigation-0.3.1/general_navigation/diffusion_policy/dataset/pusht_dataset.py`

 * *Files identical despite different names*

### Comparing `general_navigation-0.3.0/general_navigation/diffusion_policy/dataset/pusht_image_dataset.py` & `general_navigation-0.3.1/general_navigation/diffusion_policy/dataset/pusht_image_dataset.py`

 * *Files identical despite different names*

### Comparing `general_navigation-0.3.0/general_navigation/diffusion_policy/dataset/real_pusht_image_dataset.py` & `general_navigation-0.3.1/general_navigation/diffusion_policy/dataset/real_pusht_image_dataset.py`

 * *Files identical despite different names*

### Comparing `general_navigation-0.3.0/general_navigation/diffusion_policy/dataset/robomimic_replay_image_dataset.py` & `general_navigation-0.3.1/general_navigation/diffusion_policy/dataset/robomimic_replay_image_dataset.py`

 * *Files identical despite different names*

### Comparing `general_navigation-0.3.0/general_navigation/diffusion_policy/dataset/robomimic_replay_lowdim_dataset.py` & `general_navigation-0.3.1/general_navigation/diffusion_policy/dataset/robomimic_replay_lowdim_dataset.py`

 * *Files identical despite different names*

### Comparing `general_navigation-0.3.0/general_navigation/diffusion_policy/env_runner/blockpush_lowdim_runner.py` & `general_navigation-0.3.1/general_navigation/diffusion_policy/env_runner/blockpush_lowdim_runner.py`

 * *Files identical despite different names*

### Comparing `general_navigation-0.3.0/general_navigation/diffusion_policy/env_runner/kitchen_lowdim_runner.py` & `general_navigation-0.3.1/general_navigation/diffusion_policy/env_runner/kitchen_lowdim_runner.py`

 * *Files identical despite different names*

### Comparing `general_navigation-0.3.0/general_navigation/diffusion_policy/env_runner/pusht_image_runner.py` & `general_navigation-0.3.1/general_navigation/diffusion_policy/env_runner/pusht_image_runner.py`

 * *Files identical despite different names*

### Comparing `general_navigation-0.3.0/general_navigation/diffusion_policy/env_runner/pusht_keypoints_runner.py` & `general_navigation-0.3.1/general_navigation/diffusion_policy/env_runner/pusht_keypoints_runner.py`

 * *Files identical despite different names*

### Comparing `general_navigation-0.3.0/general_navigation/diffusion_policy/env_runner/robomimic_image_runner.py` & `general_navigation-0.3.1/general_navigation/diffusion_policy/env_runner/robomimic_image_runner.py`

 * *Files identical despite different names*

### Comparing `general_navigation-0.3.0/general_navigation/diffusion_policy/env_runner/robomimic_lowdim_runner.py` & `general_navigation-0.3.1/general_navigation/diffusion_policy/env_runner/robomimic_lowdim_runner.py`

 * *Files identical despite different names*

### Comparing `general_navigation-0.3.0/general_navigation/diffusion_policy/gym_util/async_vector_env.py` & `general_navigation-0.3.1/general_navigation/diffusion_policy/gym_util/async_vector_env.py`

 * *Files identical despite different names*

### Comparing `general_navigation-0.3.0/general_navigation/diffusion_policy/gym_util/multistep_wrapper.py` & `general_navigation-0.3.1/general_navigation/diffusion_policy/gym_util/multistep_wrapper.py`

 * *Files identical despite different names*

### Comparing `general_navigation-0.3.0/general_navigation/diffusion_policy/gym_util/sync_vector_env.py` & `general_navigation-0.3.1/general_navigation/diffusion_policy/gym_util/sync_vector_env.py`

 * *Files identical despite different names*

### Comparing `general_navigation-0.3.0/general_navigation/diffusion_policy/gym_util/video_recording_wrapper.py` & `general_navigation-0.3.1/general_navigation/diffusion_policy/gym_util/video_recording_wrapper.py`

 * *Files identical despite different names*

### Comparing `general_navigation-0.3.0/general_navigation/diffusion_policy/gym_util/video_wrapper.py` & `general_navigation-0.3.1/general_navigation/diffusion_policy/gym_util/video_wrapper.py`

 * *Files identical despite different names*

### Comparing `general_navigation-0.3.0/general_navigation/diffusion_policy/model/bet/action_ae/__init__.py` & `general_navigation-0.3.1/general_navigation/diffusion_policy/model/bet/action_ae/__init__.py`

 * *Files identical despite different names*

### Comparing `general_navigation-0.3.0/general_navigation/diffusion_policy/model/bet/action_ae/discretizers/k_means.py` & `general_navigation-0.3.1/general_navigation/diffusion_policy/model/bet/action_ae/discretizers/k_means.py`

 * *Files identical despite different names*

### Comparing `general_navigation-0.3.0/general_navigation/diffusion_policy/model/bet/latent_generators/latent_generator.py` & `general_navigation-0.3.1/general_navigation/diffusion_policy/model/bet/latent_generators/latent_generator.py`

 * *Files identical despite different names*

### Comparing `general_navigation-0.3.0/general_navigation/diffusion_policy/model/bet/latent_generators/mingpt.py` & `general_navigation-0.3.1/general_navigation/diffusion_policy/model/bet/latent_generators/mingpt.py`

 * *Files identical despite different names*

### Comparing `general_navigation-0.3.0/general_navigation/diffusion_policy/model/bet/latent_generators/transformer.py` & `general_navigation-0.3.1/general_navigation/diffusion_policy/model/bet/latent_generators/transformer.py`

 * *Files identical despite different names*

### Comparing `general_navigation-0.3.0/general_navigation/diffusion_policy/model/bet/libraries/loss_fn.py` & `general_navigation-0.3.1/general_navigation/diffusion_policy/model/bet/libraries/loss_fn.py`

 * *Files identical despite different names*

### Comparing `general_navigation-0.3.0/general_navigation/diffusion_policy/model/bet/libraries/mingpt/LICENSE` & `general_navigation-0.3.1/general_navigation/diffusion_policy/model/bet/libraries/mingpt/LICENSE`

 * *Files identical despite different names*

### Comparing `general_navigation-0.3.0/general_navigation/diffusion_policy/model/bet/libraries/mingpt/model.py` & `general_navigation-0.3.1/general_navigation/diffusion_policy/model/bet/libraries/mingpt/model.py`

 * *Files identical despite different names*

### Comparing `general_navigation-0.3.0/general_navigation/diffusion_policy/model/bet/libraries/mingpt/trainer.py` & `general_navigation-0.3.1/general_navigation/diffusion_policy/model/bet/libraries/mingpt/trainer.py`

 * *Files identical despite different names*

### Comparing `general_navigation-0.3.0/general_navigation/diffusion_policy/model/bet/libraries/mingpt/utils.py` & `general_navigation-0.3.1/general_navigation/diffusion_policy/model/bet/libraries/mingpt/utils.py`

 * *Files identical despite different names*

### Comparing `general_navigation-0.3.0/general_navigation/diffusion_policy/model/bet/utils.py` & `general_navigation-0.3.1/general_navigation/diffusion_policy/model/bet/utils.py`

 * *Files identical despite different names*

### Comparing `general_navigation-0.3.0/general_navigation/diffusion_policy/model/common/dict_of_tensor_mixin.py` & `general_navigation-0.3.1/general_navigation/diffusion_policy/model/common/dict_of_tensor_mixin.py`

 * *Files identical despite different names*

### Comparing `general_navigation-0.3.0/general_navigation/diffusion_policy/model/common/lr_scheduler.py` & `general_navigation-0.3.1/general_navigation/diffusion_policy/model/common/lr_scheduler.py`

 * *Files identical despite different names*

### Comparing `general_navigation-0.3.0/general_navigation/diffusion_policy/model/common/normalizer.py` & `general_navigation-0.3.1/general_navigation/diffusion_policy/model/common/normalizer.py`

 * *Files identical despite different names*

### Comparing `general_navigation-0.3.0/general_navigation/diffusion_policy/model/common/rotation_transformer.py` & `general_navigation-0.3.1/general_navigation/diffusion_policy/model/common/rotation_transformer.py`

 * *Files identical despite different names*

### Comparing `general_navigation-0.3.0/general_navigation/diffusion_policy/model/common/shape_util.py` & `general_navigation-0.3.1/general_navigation/diffusion_policy/model/common/shape_util.py`

 * *Files identical despite different names*

### Comparing `general_navigation-0.3.0/general_navigation/diffusion_policy/model/common/tensor_util.py` & `general_navigation-0.3.1/general_navigation/diffusion_policy/model/common/tensor_util.py`

 * *Files identical despite different names*

### Comparing `general_navigation-0.3.0/general_navigation/diffusion_policy/model/diffusion/conditional_unet1d.py` & `general_navigation-0.3.1/general_navigation/diffusion_policy/model/diffusion/conditional_unet1d.py`

 * *Files identical despite different names*

### Comparing `general_navigation-0.3.0/general_navigation/diffusion_policy/model/diffusion/conv1d_components.py` & `general_navigation-0.3.1/general_navigation/diffusion_policy/model/diffusion/conv1d_components.py`

 * *Files identical despite different names*

### Comparing `general_navigation-0.3.0/general_navigation/diffusion_policy/model/diffusion/ema_model.py` & `general_navigation-0.3.1/general_navigation/diffusion_policy/model/diffusion/ema_model.py`

 * *Files identical despite different names*

### Comparing `general_navigation-0.3.0/general_navigation/diffusion_policy/model/diffusion/mask_generator.py` & `general_navigation-0.3.1/general_navigation/diffusion_policy/model/diffusion/mask_generator.py`

 * *Files identical despite different names*

### Comparing `general_navigation-0.3.0/general_navigation/diffusion_policy/model/diffusion/transformer_for_diffusion.py` & `general_navigation-0.3.1/general_navigation/diffusion_policy/model/diffusion/transformer_for_diffusion.py`

 * *Files identical despite different names*

### Comparing `general_navigation-0.3.0/general_navigation/diffusion_policy/model/vision/crop_randomizer.py` & `general_navigation-0.3.1/general_navigation/diffusion_policy/model/vision/crop_randomizer.py`

 * *Files identical despite different names*

### Comparing `general_navigation-0.3.0/general_navigation/diffusion_policy/model/vision/model_getter.py` & `general_navigation-0.3.1/general_navigation/diffusion_policy/model/vision/model_getter.py`

 * *Files identical despite different names*

### Comparing `general_navigation-0.3.0/general_navigation/diffusion_policy/model/vision/multi_image_obs_encoder.py` & `general_navigation-0.3.1/general_navigation/diffusion_policy/model/vision/multi_image_obs_encoder.py`

 * *Files identical despite different names*

### Comparing `general_navigation-0.3.0/general_navigation/diffusion_policy/policy/base_image_policy.py` & `general_navigation-0.3.1/general_navigation/diffusion_policy/policy/base_image_policy.py`

 * *Files identical despite different names*

### Comparing `general_navigation-0.3.0/general_navigation/diffusion_policy/policy/base_lowdim_policy.py` & `general_navigation-0.3.1/general_navigation/diffusion_policy/policy/base_lowdim_policy.py`

 * *Files identical despite different names*

### Comparing `general_navigation-0.3.0/general_navigation/diffusion_policy/policy/bet_lowdim_policy.py` & `general_navigation-0.3.1/general_navigation/diffusion_policy/policy/bet_lowdim_policy.py`

 * *Files identical despite different names*

### Comparing `general_navigation-0.3.0/general_navigation/diffusion_policy/policy/diffusion_transformer_hybrid_image_policy.py` & `general_navigation-0.3.1/general_navigation/diffusion_policy/policy/diffusion_transformer_hybrid_image_policy.py`

 * *Files identical despite different names*

### Comparing `general_navigation-0.3.0/general_navigation/diffusion_policy/policy/diffusion_transformer_lowdim_policy.py` & `general_navigation-0.3.1/general_navigation/diffusion_policy/policy/diffusion_transformer_lowdim_policy.py`

 * *Files identical despite different names*

### Comparing `general_navigation-0.3.0/general_navigation/diffusion_policy/policy/diffusion_unet_hybrid_image_policy.py` & `general_navigation-0.3.1/general_navigation/diffusion_policy/policy/diffusion_unet_hybrid_image_policy.py`

 * *Files identical despite different names*

### Comparing `general_navigation-0.3.0/general_navigation/diffusion_policy/policy/diffusion_unet_image_policy.py` & `general_navigation-0.3.1/general_navigation/diffusion_policy/policy/diffusion_unet_image_policy.py`

 * *Files identical despite different names*

### Comparing `general_navigation-0.3.0/general_navigation/diffusion_policy/policy/diffusion_unet_lowdim_policy.py` & `general_navigation-0.3.1/general_navigation/diffusion_policy/policy/diffusion_unet_lowdim_policy.py`

 * *Files identical despite different names*

### Comparing `general_navigation-0.3.0/general_navigation/diffusion_policy/policy/diffusion_unet_video_policy.py` & `general_navigation-0.3.1/general_navigation/diffusion_policy/policy/diffusion_unet_video_policy.py`

 * *Files identical despite different names*

### Comparing `general_navigation-0.3.0/general_navigation/diffusion_policy/policy/ibc_dfo_hybrid_image_policy.py` & `general_navigation-0.3.1/general_navigation/diffusion_policy/policy/ibc_dfo_hybrid_image_policy.py`

 * *Files identical despite different names*

### Comparing `general_navigation-0.3.0/general_navigation/diffusion_policy/policy/ibc_dfo_lowdim_policy.py` & `general_navigation-0.3.1/general_navigation/diffusion_policy/policy/ibc_dfo_lowdim_policy.py`

 * *Files identical despite different names*

### Comparing `general_navigation-0.3.0/general_navigation/diffusion_policy/policy/robomimic_image_policy.py` & `general_navigation-0.3.1/general_navigation/diffusion_policy/policy/robomimic_image_policy.py`

 * *Files identical despite different names*

### Comparing `general_navigation-0.3.0/general_navigation/diffusion_policy/policy/robomimic_lowdim_policy.py` & `general_navigation-0.3.1/general_navigation/diffusion_policy/policy/robomimic_lowdim_policy.py`

 * *Files identical despite different names*

### Comparing `general_navigation-0.3.0/general_navigation/diffusion_policy/real_world/keystroke_counter.py` & `general_navigation-0.3.1/general_navigation/diffusion_policy/real_world/keystroke_counter.py`

 * *Files identical despite different names*

### Comparing `general_navigation-0.3.0/general_navigation/diffusion_policy/real_world/multi_camera_visualizer.py` & `general_navigation-0.3.1/general_navigation/diffusion_policy/real_world/multi_camera_visualizer.py`

 * *Files identical despite different names*

### Comparing `general_navigation-0.3.0/general_navigation/diffusion_policy/real_world/multi_realsense.py` & `general_navigation-0.3.1/general_navigation/diffusion_policy/real_world/multi_realsense.py`

 * *Files identical despite different names*

### Comparing `general_navigation-0.3.0/general_navigation/diffusion_policy/real_world/real_data_conversion.py` & `general_navigation-0.3.1/general_navigation/diffusion_policy/real_world/real_data_conversion.py`

 * *Files identical despite different names*

### Comparing `general_navigation-0.3.0/general_navigation/diffusion_policy/real_world/real_env.py` & `general_navigation-0.3.1/general_navigation/diffusion_policy/real_world/real_env.py`

 * *Files identical despite different names*

### Comparing `general_navigation-0.3.0/general_navigation/diffusion_policy/real_world/real_inference_util.py` & `general_navigation-0.3.1/general_navigation/diffusion_policy/real_world/real_inference_util.py`

 * *Files identical despite different names*

### Comparing `general_navigation-0.3.0/general_navigation/diffusion_policy/real_world/realsense_config/415_high_accuracy_mode.json` & `general_navigation-0.3.1/general_navigation/diffusion_policy/real_world/realsense_config/415_high_accuracy_mode.json`

 * *Files identical despite different names*

### Comparing `general_navigation-0.3.0/general_navigation/diffusion_policy/real_world/realsense_config/435_high_accuracy_mode.json` & `general_navigation-0.3.1/general_navigation/diffusion_policy/real_world/realsense_config/435_high_accuracy_mode.json`

 * *Files identical despite different names*

### Comparing `general_navigation-0.3.0/general_navigation/diffusion_policy/real_world/rtde_interpolation_controller.py` & `general_navigation-0.3.1/general_navigation/diffusion_policy/real_world/rtde_interpolation_controller.py`

 * *Files identical despite different names*

### Comparing `general_navigation-0.3.0/general_navigation/diffusion_policy/real_world/single_realsense.py` & `general_navigation-0.3.1/general_navigation/diffusion_policy/real_world/single_realsense.py`

 * *Files identical despite different names*

### Comparing `general_navigation-0.3.0/general_navigation/diffusion_policy/real_world/spacemouse.py` & `general_navigation-0.3.1/general_navigation/diffusion_policy/real_world/spacemouse.py`

 * *Files identical despite different names*

### Comparing `general_navigation-0.3.0/general_navigation/diffusion_policy/real_world/spacemouse_shared_memory.py` & `general_navigation-0.3.1/general_navigation/diffusion_policy/real_world/spacemouse_shared_memory.py`

 * *Files identical despite different names*

### Comparing `general_navigation-0.3.0/general_navigation/diffusion_policy/real_world/video_recorder.py` & `general_navigation-0.3.1/general_navigation/diffusion_policy/real_world/video_recorder.py`

 * *Files identical despite different names*

### Comparing `general_navigation-0.3.0/general_navigation/diffusion_policy/scripts/bet_blockpush_conversion.py` & `general_navigation-0.3.1/general_navigation/diffusion_policy/scripts/bet_blockpush_conversion.py`

 * *Files identical despite different names*

### Comparing `general_navigation-0.3.0/general_navigation/diffusion_policy/scripts/blockpush_abs_conversion.py` & `general_navigation-0.3.1/general_navigation/diffusion_policy/scripts/blockpush_abs_conversion.py`

 * *Files identical despite different names*

### Comparing `general_navigation-0.3.0/general_navigation/diffusion_policy/scripts/episode_lengths.py` & `general_navigation-0.3.1/general_navigation/diffusion_policy/scripts/episode_lengths.py`

 * *Files identical despite different names*

### Comparing `general_navigation-0.3.0/general_navigation/diffusion_policy/scripts/generate_bet_blockpush.py` & `general_navigation-0.3.1/general_navigation/diffusion_policy/scripts/generate_bet_blockpush.py`

 * *Files identical despite different names*

### Comparing `general_navigation-0.3.0/general_navigation/diffusion_policy/scripts/real_dataset_conversion.py` & `general_navigation-0.3.1/general_navigation/diffusion_policy/scripts/real_dataset_conversion.py`

 * *Files identical despite different names*

### Comparing `general_navigation-0.3.0/general_navigation/diffusion_policy/scripts/real_pusht_metrics.py` & `general_navigation-0.3.1/general_navigation/diffusion_policy/scripts/real_pusht_metrics.py`

 * *Files identical despite different names*

### Comparing `general_navigation-0.3.0/general_navigation/diffusion_policy/scripts/real_pusht_successrate.py` & `general_navigation-0.3.1/general_navigation/diffusion_policy/scripts/real_pusht_successrate.py`

 * *Files identical despite different names*

### Comparing `general_navigation-0.3.0/general_navigation/diffusion_policy/scripts/robomimic_dataset_action_comparison.py` & `general_navigation-0.3.1/general_navigation/diffusion_policy/scripts/robomimic_dataset_action_comparison.py`

 * *Files identical despite different names*

### Comparing `general_navigation-0.3.0/general_navigation/diffusion_policy/scripts/robomimic_dataset_conversion.py` & `general_navigation-0.3.1/general_navigation/diffusion_policy/scripts/robomimic_dataset_conversion.py`

 * *Files identical despite different names*

### Comparing `general_navigation-0.3.0/general_navigation/diffusion_policy/shared_memory/shared_memory_queue.py` & `general_navigation-0.3.1/general_navigation/diffusion_policy/shared_memory/shared_memory_queue.py`

 * *Files identical despite different names*

### Comparing `general_navigation-0.3.0/general_navigation/diffusion_policy/shared_memory/shared_memory_ring_buffer.py` & `general_navigation-0.3.1/general_navigation/diffusion_policy/shared_memory/shared_memory_ring_buffer.py`

 * *Files identical despite different names*

### Comparing `general_navigation-0.3.0/general_navigation/diffusion_policy/shared_memory/shared_memory_util.py` & `general_navigation-0.3.1/general_navigation/diffusion_policy/shared_memory/shared_memory_util.py`

 * *Files identical despite different names*

### Comparing `general_navigation-0.3.0/general_navigation/diffusion_policy/shared_memory/shared_ndarray.py` & `general_navigation-0.3.1/general_navigation/diffusion_policy/shared_memory/shared_ndarray.py`

 * *Files identical despite different names*

### Comparing `general_navigation-0.3.0/general_navigation/diffusion_policy/workspace/base_workspace.py` & `general_navigation-0.3.1/general_navigation/diffusion_policy/workspace/base_workspace.py`

 * *Files identical despite different names*

### Comparing `general_navigation-0.3.0/general_navigation/diffusion_policy/workspace/train_bet_lowdim_workspace.py` & `general_navigation-0.3.1/general_navigation/diffusion_policy/workspace/train_bet_lowdim_workspace.py`

 * *Files identical despite different names*

### Comparing `general_navigation-0.3.0/general_navigation/diffusion_policy/workspace/train_diffusion_transformer_hybrid_workspace.py` & `general_navigation-0.3.1/general_navigation/diffusion_policy/workspace/train_diffusion_transformer_hybrid_workspace.py`

 * *Files identical despite different names*

### Comparing `general_navigation-0.3.0/general_navigation/diffusion_policy/workspace/train_diffusion_transformer_lowdim_workspace.py` & `general_navigation-0.3.1/general_navigation/diffusion_policy/workspace/train_diffusion_transformer_lowdim_workspace.py`

 * *Files identical despite different names*

### Comparing `general_navigation-0.3.0/general_navigation/diffusion_policy/workspace/train_diffusion_unet_hybrid_workspace.py` & `general_navigation-0.3.1/general_navigation/diffusion_policy/workspace/train_diffusion_unet_hybrid_workspace.py`

 * *Files identical despite different names*

### Comparing `general_navigation-0.3.0/general_navigation/diffusion_policy/workspace/train_diffusion_unet_image_workspace.py` & `general_navigation-0.3.1/general_navigation/diffusion_policy/workspace/train_diffusion_unet_image_workspace.py`

 * *Files identical despite different names*

### Comparing `general_navigation-0.3.0/general_navigation/diffusion_policy/workspace/train_diffusion_unet_lowdim_workspace.py` & `general_navigation-0.3.1/general_navigation/diffusion_policy/workspace/train_diffusion_unet_lowdim_workspace.py`

 * *Files identical despite different names*

### Comparing `general_navigation-0.3.0/general_navigation/diffusion_policy/workspace/train_diffusion_unet_video_workspace.py` & `general_navigation-0.3.1/general_navigation/diffusion_policy/workspace/train_diffusion_unet_video_workspace.py`

 * *Files identical despite different names*

### Comparing `general_navigation-0.3.0/general_navigation/diffusion_policy/workspace/train_ibc_dfo_hybrid_workspace.py` & `general_navigation-0.3.1/general_navigation/diffusion_policy/workspace/train_ibc_dfo_hybrid_workspace.py`

 * *Files identical despite different names*

### Comparing `general_navigation-0.3.0/general_navigation/diffusion_policy/workspace/train_ibc_dfo_lowdim_workspace.py` & `general_navigation-0.3.1/general_navigation/diffusion_policy/workspace/train_ibc_dfo_lowdim_workspace.py`

 * *Files identical despite different names*

### Comparing `general_navigation-0.3.0/general_navigation/diffusion_policy/workspace/train_robomimic_image_workspace.py` & `general_navigation-0.3.1/general_navigation/diffusion_policy/workspace/train_robomimic_image_workspace.py`

 * *Files identical despite different names*

### Comparing `general_navigation-0.3.0/general_navigation/diffusion_policy/workspace/train_robomimic_lowdim_workspace.py` & `general_navigation-0.3.1/general_navigation/diffusion_policy/workspace/train_robomimic_lowdim_workspace.py`

 * *Files identical despite different names*

### Comparing `general_navigation-0.3.0/general_navigation/gpt/gpt_vision.py` & `general_navigation-0.3.1/general_navigation/gpt/gpt_vision.py`

 * *Files identical despite different names*

### Comparing `general_navigation-0.3.0/general_navigation/models/base_model.py` & `general_navigation-0.3.1/general_navigation/models/base_model.py`

 * *Files identical despite different names*

### Comparing `general_navigation-0.3.0/general_navigation/models/config/data_config.yaml` & `general_navigation-0.3.1/general_navigation/models/config/data_config.yaml`

 * *Files identical despite different names*

### Comparing `general_navigation-0.3.0/general_navigation/models/config/defaults.yaml` & `general_navigation-0.3.1/general_navigation/models/config/defaults.yaml`

 * *Files identical despite different names*

### Comparing `general_navigation-0.3.0/general_navigation/models/config/gnm.yaml` & `general_navigation-0.3.1/general_navigation/models/config/gnm.yaml`

 * *Files identical despite different names*

### Comparing `general_navigation-0.3.0/general_navigation/models/config/late_fusion.yaml` & `general_navigation-0.3.1/general_navigation/models/config/late_fusion.yaml`

 * *Files identical despite different names*

### Comparing `general_navigation-0.3.0/general_navigation/models/config/nomad.yaml` & `general_navigation-0.3.1/general_navigation/models/config/nomad.yaml`

 * *Files identical despite different names*

### Comparing `general_navigation-0.3.0/general_navigation/models/config/vint.yaml` & `general_navigation-0.3.1/general_navigation/models/config/vint.yaml`

 * *Files identical despite different names*

### Comparing `general_navigation-0.3.0/general_navigation/models/factory.py` & `general_navigation-0.3.1/general_navigation/models/factory.py`

 * *Files identical despite different names*

### Comparing `general_navigation-0.3.0/general_navigation/models/gnm/gnm.py` & `general_navigation-0.3.1/general_navigation/models/gnm/gnm.py`

 * *Files identical despite different names*

### Comparing `general_navigation-0.3.0/general_navigation/models/gnm/modified_mobilenetv2.py` & `general_navigation-0.3.1/general_navigation/models/gnm/modified_mobilenetv2.py`

 * *Files identical despite different names*

### Comparing `general_navigation-0.3.0/general_navigation/models/model_utils.py` & `general_navigation-0.3.1/general_navigation/models/model_utils.py`

 * *Files identical despite different names*

### Comparing `general_navigation-0.3.0/general_navigation/models/nomad/nomad.py` & `general_navigation-0.3.1/general_navigation/models/nomad/nomad.py`

 * *Files identical despite different names*

### Comparing `general_navigation-0.3.0/general_navigation/models/nomad/nomad_vint.py` & `general_navigation-0.3.1/general_navigation/models/nomad/nomad_vint.py`

 * *Files identical despite different names*

### Comparing `general_navigation-0.3.0/general_navigation/models/vint/self_attention.py` & `general_navigation-0.3.1/general_navigation/models/vint/self_attention.py`

 * *Files identical despite different names*

### Comparing `general_navigation-0.3.0/general_navigation/models/vint/vint.py` & `general_navigation-0.3.1/general_navigation/models/vint/vint.py`

 * *Files identical despite different names*

### Comparing `general_navigation-0.3.0/general_navigation/models/vint/vit.py` & `general_navigation-0.3.1/general_navigation/models/vint/vit.py`

 * *Files identical despite different names*

### Comparing `general_navigation-0.3.0/general_navigation/mpc.py` & `general_navigation-0.3.1/general_navigation/mpc.py`

 * *Files identical despite different names*

### Comparing `general_navigation-0.3.0/general_navigation/schema/carla.py` & `general_navigation-0.3.1/general_navigation/schema/carla.py`

 * *Files identical despite different names*

### Comparing `general_navigation-0.3.0/general_navigation/schema/image.py` & `general_navigation-0.3.1/general_navigation/schema/image.py`

 * *Files identical despite different names*

### Comparing `general_navigation-0.3.0/general_navigation/settings.py` & `general_navigation-0.3.1/general_navigation/settings.py`

 * *Files identical despite different names*

### Comparing `general_navigation-0.3.0/general_navigation/visualizing/action_utils.py` & `general_navigation-0.3.1/general_navigation/visualizing/action_utils.py`

 * *Files identical despite different names*

### Comparing `general_navigation-0.3.0/general_navigation/visualizing/distance_utils.py` & `general_navigation-0.3.1/general_navigation/visualizing/distance_utils.py`

 * *Files identical despite different names*

### Comparing `general_navigation-0.3.0/general_navigation/visualizing/visualize_utils.py` & `general_navigation-0.3.1/general_navigation/visualizing/visualize_utils.py`

 * *Files identical despite different names*

### Comparing `general_navigation-0.3.0/general_navigation.egg-info/PKG-INFO` & `general_navigation-0.3.1/general_navigation.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 Metadata-Version: 2.1
 Name: general_navigation
-Version: 0.3.0
+Version: 0.3.1
 Summary: Awesome general_navigation created by AdityaNG
 Home-page: https://github.com/AdityaNG/general-navigation/
 Author: AdityaNG
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: torch>=2.2.2
 Requires-Dist: torchvision>=0.17.2
 Requires-Dist: numpy>=1.24.4
 Requires-Dist: setuptools>=65.5.0
 Requires-Dist: einops>=0.8.0
 Requires-Dist: opencv-python>=4.9.0.80
 Requires-Dist: efficientnet_pytorch==0.7.1
 Requires-Dist: vit-pytorch==1.6.9
 Requires-Dist: pygame==2.5.2
-Requires-Dist: carla==0.9.15
 Requires-Dist: platformdirs
 Requires-Dist: gdown
 Requires-Dist: diffusers
 Requires-Dist: matplotlib
 Requires-Dist: wandb
 Requires-Dist: pydantic
 Requires-Dist: simple-pid==1.0.1
@@ -53,21 +52,29 @@
 
 [PyPi Link](https://pypi.org/project/general-navigation/)
 
 ```bash
 pip install general_navigation
 ```
 
+If you want to connect with the Carla simulator, you will also need to seperately install carla
+```bash
+pip install carla==0.9.15  # Linux and Windows
+pip install carla==0.9.5  # Linux and Windows
+```
+
 ## Usage
 
 [Documentation Link](https://adityang.github.io/general-navigation/)
 
 Creating a pytorch instance of the model
 ```py
-from .models.factory import get_default_config, get_model, get_weights
+from general_navigation.models.factory import (
+  get_default_config, get_model, get_weights
+)
 
 config = get_default_config()
 model = get_model(config)
 model = get_weights(config, model, device)
 ```
 
 Using the command line tool for inference
```

### Comparing `general_navigation-0.3.0/general_navigation.egg-info/SOURCES.txt` & `general_navigation-0.3.1/general_navigation.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `general_navigation-0.3.0/setup.py` & `general_navigation-0.3.1/setup.py`

 * *Files identical despite different names*

