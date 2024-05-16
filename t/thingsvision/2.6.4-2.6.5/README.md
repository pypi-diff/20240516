# Comparing `tmp/thingsvision-2.6.4.tar.gz` & `tmp/thingsvision-2.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thingsvision-2.6.4.tar", last modified: Thu May  2 10:08:06 2024, max compression
+gzip compressed data, was "thingsvision-2.6.5.tar", last modified: Thu May 16 09:23:15 2024, max compression
```

## Comparing `thingsvision-2.6.4.tar` & `thingsvision-2.6.5.tar`

### file list

```diff
@@ -1,101 +1,103 @@
-drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-05-02 10:08:06.062951 thingsvision-2.6.4/
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     1097 2021-01-22 09:49:59.000000 thingsvision-2.6.4/LICENSE
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)    16819 2024-05-02 10:08:06.061794 thingsvision-2.6.4/PKG-INFO
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)    16216 2024-04-24 14:58:04.000000 thingsvision-2.6.4/README.md
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)       38 2024-05-02 10:08:06.063238 thingsvision-2.6.4/setup.cfg
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     1698 2024-04-22 08:56:16.000000 thingsvision-2.6.4/setup.py
-drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-05-02 10:08:06.015391 thingsvision-2.6.4/tests/
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)        0 2022-02-02 09:19:53.000000 thingsvision-2.6.4/tests/__init__.py
-drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-05-02 10:08:06.017644 thingsvision-2.6.4/tests/extractor/
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)        0 2022-08-22 09:49:44.000000 thingsvision-2.6.4/tests/extractor/__init__.py
-drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-05-02 10:08:06.021141 thingsvision-2.6.4/tests/extractor/extraction/
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)        0 2022-08-22 09:49:44.000000 thingsvision-2.6.4/tests/extractor/extraction/__init__.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     2452 2024-04-06 10:03:37.000000 thingsvision-2.6.4/tests/extractor/extraction/test_custom_model.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     3196 2024-04-01 11:22:39.000000 thingsvision-2.6.4/tests/extractor/extraction/test_model_extractor.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     1954 2024-04-22 12:22:02.000000 thingsvision-2.6.4/tests/extractor/extraction/test_pretrained_model.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     2977 2024-04-06 10:04:01.000000 thingsvision-2.6.4/tests/extractor/extraction/test_torch_vs_tensorflow.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     4459 2024-04-22 12:21:01.000000 thingsvision-2.6.4/tests/extractor/test_load_extractor.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     1487 2023-02-22 09:56:38.000000 thingsvision-2.6.4/tests/extractor/test_transformations.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)    11260 2024-04-24 14:58:04.000000 thingsvision-2.6.4/tests/helper.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     4447 2024-04-22 11:26:42.000000 thingsvision-2.6.4/tests/test_features.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     4304 2024-04-22 11:26:42.000000 thingsvision-2.6.4/tests/test_rest.py
-drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-05-02 10:08:06.023662 thingsvision-2.6.4/thingsvision/
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)      103 2022-11-09 16:59:35.000000 thingsvision-2.6.4/thingsvision/__init__.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)       22 2024-05-02 10:07:21.000000 thingsvision-2.6.4/thingsvision/_version.py
-drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-05-02 10:08:06.028694 thingsvision-2.6.4/thingsvision/core/
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)        0 2022-09-23 10:25:59.000000 thingsvision-2.6.4/thingsvision/core/__init__.py
-drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-05-02 10:08:06.031649 thingsvision-2.6.4/thingsvision/core/cka/
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)       29 2024-04-22 08:56:16.000000 thingsvision-2.6.4/thingsvision/core/cka/__init__.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     2269 2024-04-22 08:56:16.000000 thingsvision-2.6.4/thingsvision/core/cka/cka_base.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     3567 2024-04-22 08:56:16.000000 thingsvision-2.6.4/thingsvision/core/cka/cka_numpy.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     5957 2024-04-22 11:26:42.000000 thingsvision-2.6.4/thingsvision/core/cka/cka_torch.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)      818 2024-04-22 08:56:16.000000 thingsvision-2.6.4/thingsvision/core/cka/helpers.py
-drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-05-02 10:08:06.035563 thingsvision-2.6.4/thingsvision/core/extraction/
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)      176 2024-04-24 08:51:44.000000 thingsvision-2.6.4/thingsvision/core/extraction/__init__.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)    10927 2024-04-24 14:58:04.000000 thingsvision-2.6.4/thingsvision/core/extraction/base.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)    17360 2024-05-02 10:07:13.000000 thingsvision-2.6.4/thingsvision/core/extraction/extractors.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     8453 2024-04-24 14:58:04.000000 thingsvision-2.6.4/thingsvision/core/extraction/helpers.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     3134 2024-04-04 09:43:21.000000 thingsvision-2.6.4/thingsvision/core/extraction/tensorflow.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)    10948 2024-04-29 13:15:16.000000 thingsvision-2.6.4/thingsvision/core/extraction/torch.py
-drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-05-02 10:08:06.037193 thingsvision-2.6.4/thingsvision/core/rsa/
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)       59 2022-08-22 09:49:44.000000 thingsvision-2.6.4/thingsvision/core/rsa/__init__.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)        0 2022-08-29 15:24:25.000000 thingsvision-2.6.4/thingsvision/core/rsa/base.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     4651 2022-08-31 09:02:04.000000 thingsvision-2.6.4/thingsvision/core/rsa/helpers.py
-drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-05-02 10:08:06.043128 thingsvision-2.6.4/thingsvision/custom_models/
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)      286 2023-08-04 09:46:20.000000 thingsvision-2.6.4/thingsvision/custom_models/__init__.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)      620 2023-07-11 09:50:14.000000 thingsvision-2.6.4/thingsvision/custom_models/alexnet_ecoset.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)      627 2023-07-11 09:50:14.000000 thingsvision-2.6.4/thingsvision/custom_models/alexnet_salobjsub.py
-drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-05-02 10:08:06.046155 thingsvision-2.6.4/thingsvision/custom_models/cornet/
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     1474 2022-08-22 09:49:44.000000 thingsvision-2.6.4/thingsvision/custom_models/cornet/__init__.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     3588 2022-08-22 09:49:44.000000 thingsvision-2.6.4/thingsvision/custom_models/cornet/cornet_r.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     3682 2022-08-22 09:49:44.000000 thingsvision-2.6.4/thingsvision/custom_models/cornet/cornet_rt.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     4203 2022-08-22 09:49:44.000000 thingsvision-2.6.4/thingsvision/custom_models/cornet/cornet_s.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     2013 2022-08-22 09:49:44.000000 thingsvision-2.6.4/thingsvision/custom_models/cornet/cornet_z.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)      287 2023-01-18 14:03:54.000000 thingsvision-2.6.4/thingsvision/custom_models/custom.py
-drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-05-02 10:08:06.047342 thingsvision-2.6.4/thingsvision/custom_models/dreamsim/
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)       31 2023-08-04 09:46:20.000000 thingsvision-2.6.4/thingsvision/custom_models/dreamsim/__init__.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     1999 2024-03-19 09:46:42.000000 thingsvision-2.6.4/thingsvision/custom_models/dreamsim/dreamsim.py
-drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-05-02 10:08:06.048555 thingsvision-2.6.4/thingsvision/custom_models/harmonization/
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)       41 2023-03-06 11:11:47.000000 thingsvision-2.6.4/thingsvision/custom_models/harmonization/__init__.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     1366 2023-03-06 11:11:52.000000 thingsvision-2.6.4/thingsvision/custom_models/harmonization/harmonization.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)      629 2023-08-04 09:17:34.000000 thingsvision-2.6.4/thingsvision/custom_models/inception_ecoset.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)      453 2023-07-26 10:09:51.000000 thingsvision-2.6.4/thingsvision/custom_models/official_clip.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     1033 2023-07-11 09:50:14.000000 thingsvision-2.6.4/thingsvision/custom_models/openclip.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)      623 2023-08-04 09:16:38.000000 thingsvision-2.6.4/thingsvision/custom_models/resnet50_ecoset.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)      614 2023-08-04 09:31:47.000000 thingsvision-2.6.4/thingsvision/custom_models/vgg16_ecoset.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)      621 2023-08-04 09:46:20.000000 thingsvision-2.6.4/thingsvision/custom_models/vgg16bn_ecoset.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     5992 2024-04-16 08:05:49.000000 thingsvision-2.6.4/thingsvision/thingsvision.py
-drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-05-02 10:08:06.049164 thingsvision-2.6.4/thingsvision/utils/
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)        0 2022-09-26 11:38:32.000000 thingsvision-2.6.4/thingsvision/utils/__init__.py
-drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-05-02 10:08:06.050293 thingsvision-2.6.4/thingsvision/utils/alignment/
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)       31 2024-03-28 13:19:33.000000 thingsvision-2.6.4/thingsvision/utils/alignment/__init__.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     2633 2024-03-28 13:33:43.000000 thingsvision-2.6.4/thingsvision/utils/alignment/transforms.py
-drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-05-02 10:08:06.050923 thingsvision-2.6.4/thingsvision/utils/checkpointing/
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)      522 2023-07-26 10:09:51.000000 thingsvision-2.6.4/thingsvision/utils/checkpointing/__init__.py
-drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-05-02 10:08:06.053412 thingsvision-2.6.4/thingsvision/utils/data/
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     2013 2022-11-15 12:25:36.000000 thingsvision-2.6.4/thingsvision/utils/data/__init__.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     1778 2022-11-15 12:25:36.000000 thingsvision-2.6.4/thingsvision/utils/data/data_loader.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     7808 2022-11-15 12:25:36.000000 thingsvision-2.6.4/thingsvision/utils/data/dataset.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     2969 2022-08-25 08:25:51.000000 thingsvision-2.6.4/thingsvision/utils/data/helpers.py
-drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-05-02 10:08:06.054031 thingsvision-2.6.4/thingsvision/utils/imagenet/
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     2355 2022-08-22 09:49:44.000000 thingsvision-2.6.4/thingsvision/utils/imagenet/__init__.py
-drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-05-02 10:08:06.054636 thingsvision-2.6.4/thingsvision/utils/models/
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)        0 2023-08-09 09:09:13.000000 thingsvision-2.6.4/thingsvision/utils/models/__init__.py
-drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-05-02 10:08:06.056336 thingsvision-2.6.4/thingsvision/utils/models/dino/
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)       62 2024-04-05 17:27:52.000000 thingsvision-2.6.4/thingsvision/utils/models/dino/__init__.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     2396 2023-08-08 13:01:35.000000 thingsvision-2.6.4/thingsvision/utils/models/dino/utils.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)    11168 2023-08-08 13:01:35.000000 thingsvision-2.6.4/thingsvision/utils/models/dino/vision_transformer.py
-drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-05-02 10:08:06.058143 thingsvision-2.6.4/thingsvision/utils/models/mae/
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)      116 2024-04-08 11:02:58.000000 thingsvision-2.6.4/thingsvision/utils/models/mae/__init__.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     2157 2024-04-08 11:02:58.000000 thingsvision-2.6.4/thingsvision/utils/models/mae/utils.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     2108 2024-04-08 11:02:58.000000 thingsvision-2.6.4/thingsvision/utils/models/mae/vit_mae.py
-drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-05-02 10:08:06.060596 thingsvision-2.6.4/thingsvision/utils/storing/
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)       67 2022-08-22 09:49:44.000000 thingsvision-2.6.4/thingsvision/utils/storing/__init__.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     7325 2024-04-20 11:40:10.000000 thingsvision-2.6.4/thingsvision/utils/storing/helpers.py
-drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-05-02 10:08:06.028013 thingsvision-2.6.4/thingsvision.egg-info/
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)    16819 2024-05-02 10:08:05.000000 thingsvision-2.6.4/thingsvision.egg-info/PKG-INFO
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     2880 2024-05-02 10:08:05.000000 thingsvision-2.6.4/thingsvision.egg-info/SOURCES.txt
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)       39 2024-05-02 10:08:05.000000 thingsvision-2.6.4/thingsvision.egg-info/dependency_links.txt
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)       64 2024-05-02 10:08:05.000000 thingsvision-2.6.4/thingsvision.egg-info/entry_points.txt
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)      325 2024-05-02 10:08:05.000000 thingsvision-2.6.4/thingsvision.egg-info/requires.txt
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)       19 2024-05-02 10:08:05.000000 thingsvision-2.6.4/thingsvision.egg-info/top_level.txt
+drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-05-16 09:23:15.905620 thingsvision-2.6.5/
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     1097 2021-01-22 09:49:59.000000 thingsvision-2.6.5/LICENSE
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)    16819 2024-05-16 09:23:15.905293 thingsvision-2.6.5/PKG-INFO
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)    16216 2024-04-24 14:58:04.000000 thingsvision-2.6.5/README.md
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)       38 2024-05-16 09:23:15.905700 thingsvision-2.6.5/setup.cfg
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     1725 2024-05-16 09:23:05.000000 thingsvision-2.6.5/setup.py
+drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-05-16 09:23:15.867497 thingsvision-2.6.5/tests/
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)        0 2022-02-02 09:19:53.000000 thingsvision-2.6.5/tests/__init__.py
+drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-05-16 09:23:15.869043 thingsvision-2.6.5/tests/extractor/
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)        0 2022-08-22 09:49:44.000000 thingsvision-2.6.5/tests/extractor/__init__.py
+drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-05-16 09:23:15.871299 thingsvision-2.6.5/tests/extractor/extraction/
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)        0 2022-08-22 09:49:44.000000 thingsvision-2.6.5/tests/extractor/extraction/__init__.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     2452 2024-04-06 10:03:37.000000 thingsvision-2.6.5/tests/extractor/extraction/test_custom_model.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     3196 2024-04-01 11:22:39.000000 thingsvision-2.6.5/tests/extractor/extraction/test_model_extractor.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     2180 2024-05-16 09:23:05.000000 thingsvision-2.6.5/tests/extractor/extraction/test_pretrained_model.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     2977 2024-04-06 10:04:01.000000 thingsvision-2.6.5/tests/extractor/extraction/test_torch_vs_tensorflow.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     4459 2024-04-22 12:21:01.000000 thingsvision-2.6.5/tests/extractor/test_load_extractor.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     1487 2023-02-22 09:56:38.000000 thingsvision-2.6.5/tests/extractor/test_transformations.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)    12379 2024-05-16 09:23:05.000000 thingsvision-2.6.5/tests/helper.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     4447 2024-04-22 11:26:42.000000 thingsvision-2.6.5/tests/test_features.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     4304 2024-04-22 11:26:42.000000 thingsvision-2.6.5/tests/test_rest.py
+drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-05-16 09:23:15.873108 thingsvision-2.6.5/thingsvision/
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)      103 2022-11-09 16:59:35.000000 thingsvision-2.6.5/thingsvision/__init__.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)       22 2024-05-16 09:23:05.000000 thingsvision-2.6.5/thingsvision/_version.py
+drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-05-16 09:23:15.875781 thingsvision-2.6.5/thingsvision/core/
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)        0 2022-09-23 10:25:59.000000 thingsvision-2.6.5/thingsvision/core/__init__.py
+drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-05-16 09:23:15.878159 thingsvision-2.6.5/thingsvision/core/cka/
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)       29 2024-04-22 08:56:16.000000 thingsvision-2.6.5/thingsvision/core/cka/__init__.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     2269 2024-04-22 08:56:16.000000 thingsvision-2.6.5/thingsvision/core/cka/cka_base.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     3567 2024-04-22 08:56:16.000000 thingsvision-2.6.5/thingsvision/core/cka/cka_numpy.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     5957 2024-04-22 11:26:42.000000 thingsvision-2.6.5/thingsvision/core/cka/cka_torch.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)      818 2024-04-22 08:56:16.000000 thingsvision-2.6.5/thingsvision/core/cka/helpers.py
+drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-05-16 09:23:15.881982 thingsvision-2.6.5/thingsvision/core/extraction/
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)      176 2024-04-24 08:51:44.000000 thingsvision-2.6.5/thingsvision/core/extraction/__init__.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)    10927 2024-04-24 14:58:04.000000 thingsvision-2.6.5/thingsvision/core/extraction/base.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)    17360 2024-05-02 10:07:13.000000 thingsvision-2.6.5/thingsvision/core/extraction/extractors.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     8453 2024-04-24 14:58:04.000000 thingsvision-2.6.5/thingsvision/core/extraction/helpers.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     3134 2024-04-04 09:43:21.000000 thingsvision-2.6.5/thingsvision/core/extraction/tensorflow.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)    10948 2024-04-29 13:15:16.000000 thingsvision-2.6.5/thingsvision/core/extraction/torch.py
+drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-05-16 09:23:15.883467 thingsvision-2.6.5/thingsvision/core/rsa/
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)       59 2022-08-22 09:49:44.000000 thingsvision-2.6.5/thingsvision/core/rsa/__init__.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)        0 2022-08-29 15:24:25.000000 thingsvision-2.6.5/thingsvision/core/rsa/base.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     4651 2022-08-31 09:02:04.000000 thingsvision-2.6.5/thingsvision/core/rsa/helpers.py
+drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-05-16 09:23:15.890787 thingsvision-2.6.5/thingsvision/custom_models/
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)      355 2024-05-16 09:23:05.000000 thingsvision-2.6.5/thingsvision/custom_models/__init__.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)      620 2023-07-11 09:50:14.000000 thingsvision-2.6.5/thingsvision/custom_models/alexnet_ecoset.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)      627 2023-07-11 09:50:14.000000 thingsvision-2.6.5/thingsvision/custom_models/alexnet_salobjsub.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)      627 2024-05-16 09:23:05.000000 thingsvision-2.6.5/thingsvision/custom_models/align.py
+drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-05-16 09:23:15.893247 thingsvision-2.6.5/thingsvision/custom_models/cornet/
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     1474 2022-08-22 09:49:44.000000 thingsvision-2.6.5/thingsvision/custom_models/cornet/__init__.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     3588 2022-08-22 09:49:44.000000 thingsvision-2.6.5/thingsvision/custom_models/cornet/cornet_r.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     3682 2022-08-22 09:49:44.000000 thingsvision-2.6.5/thingsvision/custom_models/cornet/cornet_rt.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     4203 2022-08-22 09:49:44.000000 thingsvision-2.6.5/thingsvision/custom_models/cornet/cornet_s.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     2013 2022-08-22 09:49:44.000000 thingsvision-2.6.5/thingsvision/custom_models/cornet/cornet_z.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)      287 2023-01-18 14:03:54.000000 thingsvision-2.6.5/thingsvision/custom_models/custom.py
+drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-05-16 09:23:15.894253 thingsvision-2.6.5/thingsvision/custom_models/dreamsim/
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)       31 2023-08-04 09:46:20.000000 thingsvision-2.6.5/thingsvision/custom_models/dreamsim/__init__.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     1999 2024-03-19 09:46:42.000000 thingsvision-2.6.5/thingsvision/custom_models/dreamsim/dreamsim.py
+drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-05-16 09:23:15.895470 thingsvision-2.6.5/thingsvision/custom_models/harmonization/
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)       41 2023-03-06 11:11:47.000000 thingsvision-2.6.5/thingsvision/custom_models/harmonization/__init__.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     1366 2023-03-06 11:11:52.000000 thingsvision-2.6.5/thingsvision/custom_models/harmonization/harmonization.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)      629 2023-08-04 09:17:34.000000 thingsvision-2.6.5/thingsvision/custom_models/inception_ecoset.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)      453 2023-07-26 10:09:51.000000 thingsvision-2.6.5/thingsvision/custom_models/official_clip.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     1033 2023-07-11 09:50:14.000000 thingsvision-2.6.5/thingsvision/custom_models/openclip.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)      623 2023-08-04 09:16:38.000000 thingsvision-2.6.5/thingsvision/custom_models/resnet50_ecoset.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     3360 2024-05-16 09:23:05.000000 thingsvision-2.6.5/thingsvision/custom_models/sam.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)      614 2023-08-04 09:31:47.000000 thingsvision-2.6.5/thingsvision/custom_models/vgg16_ecoset.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)      621 2023-08-04 09:46:20.000000 thingsvision-2.6.5/thingsvision/custom_models/vgg16bn_ecoset.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     5992 2024-04-16 08:05:49.000000 thingsvision-2.6.5/thingsvision/thingsvision.py
+drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-05-16 09:23:15.896118 thingsvision-2.6.5/thingsvision/utils/
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)        0 2022-09-26 11:38:32.000000 thingsvision-2.6.5/thingsvision/utils/__init__.py
+drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-05-16 09:23:15.897004 thingsvision-2.6.5/thingsvision/utils/alignment/
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)       31 2024-03-28 13:19:33.000000 thingsvision-2.6.5/thingsvision/utils/alignment/__init__.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     2633 2024-03-28 13:33:43.000000 thingsvision-2.6.5/thingsvision/utils/alignment/transforms.py
+drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-05-16 09:23:15.897616 thingsvision-2.6.5/thingsvision/utils/checkpointing/
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)      522 2023-07-26 10:09:51.000000 thingsvision-2.6.5/thingsvision/utils/checkpointing/__init__.py
+drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-05-16 09:23:15.899665 thingsvision-2.6.5/thingsvision/utils/data/
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     2013 2022-11-15 12:25:36.000000 thingsvision-2.6.5/thingsvision/utils/data/__init__.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     1778 2022-11-15 12:25:36.000000 thingsvision-2.6.5/thingsvision/utils/data/data_loader.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     7808 2022-11-15 12:25:36.000000 thingsvision-2.6.5/thingsvision/utils/data/dataset.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     2969 2022-08-25 08:25:51.000000 thingsvision-2.6.5/thingsvision/utils/data/helpers.py
+drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-05-16 09:23:15.900238 thingsvision-2.6.5/thingsvision/utils/imagenet/
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     2355 2022-08-22 09:49:44.000000 thingsvision-2.6.5/thingsvision/utils/imagenet/__init__.py
+drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-05-16 09:23:15.900627 thingsvision-2.6.5/thingsvision/utils/models/
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)        0 2023-08-09 09:09:13.000000 thingsvision-2.6.5/thingsvision/utils/models/__init__.py
+drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-05-16 09:23:15.902095 thingsvision-2.6.5/thingsvision/utils/models/dino/
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)       62 2024-04-05 17:27:52.000000 thingsvision-2.6.5/thingsvision/utils/models/dino/__init__.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     2396 2023-08-08 13:01:35.000000 thingsvision-2.6.5/thingsvision/utils/models/dino/utils.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)    11168 2023-08-08 13:01:35.000000 thingsvision-2.6.5/thingsvision/utils/models/dino/vision_transformer.py
+drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-05-16 09:23:15.903825 thingsvision-2.6.5/thingsvision/utils/models/mae/
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)      116 2024-04-08 11:02:58.000000 thingsvision-2.6.5/thingsvision/utils/models/mae/__init__.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     2157 2024-04-08 11:02:58.000000 thingsvision-2.6.5/thingsvision/utils/models/mae/utils.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     2108 2024-04-08 11:02:58.000000 thingsvision-2.6.5/thingsvision/utils/models/mae/vit_mae.py
+drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-05-16 09:23:15.904584 thingsvision-2.6.5/thingsvision/utils/storing/
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)       67 2022-08-22 09:49:44.000000 thingsvision-2.6.5/thingsvision/utils/storing/__init__.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     7325 2024-04-20 11:40:10.000000 thingsvision-2.6.5/thingsvision/utils/storing/helpers.py
+drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-05-16 09:23:15.875443 thingsvision-2.6.5/thingsvision.egg-info/
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)    16819 2024-05-16 09:23:15.000000 thingsvision-2.6.5/thingsvision.egg-info/PKG-INFO
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     2950 2024-05-16 09:23:15.000000 thingsvision-2.6.5/thingsvision.egg-info/SOURCES.txt
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)       39 2024-05-16 09:23:15.000000 thingsvision-2.6.5/thingsvision.egg-info/dependency_links.txt
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)       64 2024-05-16 09:23:15.000000 thingsvision-2.6.5/thingsvision.egg-info/entry_points.txt
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)      346 2024-05-16 09:23:15.000000 thingsvision-2.6.5/thingsvision.egg-info/requires.txt
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)       19 2024-05-16 09:23:15.000000 thingsvision-2.6.5/thingsvision.egg-info/top_level.txt
```

### Comparing `thingsvision-2.6.4/LICENSE` & `thingsvision-2.6.5/LICENSE`

 * *Files identical despite different names*

### Comparing `thingsvision-2.6.4/PKG-INFO` & `thingsvision-2.6.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thingsvision
-Version: 2.6.4
+Version: 2.6.5
 Summary: Extracting image features from state-of-the-art neural networks for Computer Vision made easy
 Home-page: https://github.com/ViCCo-Group/thingsvision
 Author: Lukas Muttenthaler
 Author-email: muttenthaler@cbs.mpg.de
 License: MIT License
 Keywords: feature extraction
 Classifier: Programming Language :: Python :: 3.8
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: thingsvision Version: 2.6.4 Summary: Extracting
+Metadata-Version: 2.1 Name: thingsvision Version: 2.6.5 Summary: Extracting
 image features from state-of-the-art neural networks for Computer Vision made
 easy Home-page: https://github.com/ViCCo-Group/thingsvision Author: Lukas
 Muttenthaler Author-email: muttenthaler@cbs.mpg.de License: MIT License
 Keywords: feature extraction Classifier: Programming Language :: Python :: 3.8
 Classifier: Natural Language :: English Classifier: License :: OSI Approved ::
 MIT License Classifier: Operating System :: OS Independent Requires-Python:
 >=3.8 Description-Content-Type: text/markdown License-File: LICENSE
```

### Comparing `thingsvision-2.6.4/README.md` & `thingsvision-2.6.5/README.md`

 * *Files identical despite different names*

### Comparing `thingsvision-2.6.4/setup.py` & `thingsvision-2.6.5/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,14 +22,15 @@
     "tensorflow-macos==2.9.* ; sys_platform == 'darwin' and platform_machine == 'arm64'",
     "timm",
     "torch>=2.0.0",
     "torchvision==0.15.2",
     "torchtyping",
     "tqdm",
     "CLIP",
+    "transformers==4.40.1"
     # 'CLIP @ git+ssh://git@github.com/openai/CLIP@v1.0#egg=CLIP' # TODO: see issue #111
 ]
 
 setuptools.setup(
     name="thingsvision",
     version=__version__,
     author="Lukas Muttenthaler",
```

### Comparing `thingsvision-2.6.4/tests/extractor/extraction/test_custom_model.py` & `thingsvision-2.6.5/tests/extractor/extraction/test_custom_model.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.6.4/tests/extractor/extraction/test_model_extractor.py` & `thingsvision-2.6.5/tests/extractor/extraction/test_model_extractor.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.6.4/tests/extractor/extraction/test_pretrained_model.py` & `thingsvision-2.6.5/tests/extractor/extraction/test_pretrained_model.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,14 @@
-import re
+import shutil
 import unittest
+import os
 
 import numpy as np
 import tests.helper as helper
+from thingsvision.utils.checkpointing import get_torch_home
 
 Array = np.ndarray
 
 
 class ExtractionPretrainedTestCase(unittest.TestCase):
     @classmethod
     def setUpClass(cls):
@@ -17,15 +19,14 @@
         for (
             extractor,
             dataset,
             batches,
             module_names,
             model_name
         ) in helper.iterate_through_all_model_combinations():
-            self.assertEqual(len(dataset), len(batches) * helper.BATCH_SIZE)
             num_objects = len(dataset)
 
             for module_name in module_names:
                 features = extractor.extract_features(
                     batches=batches,
                     module_name=module_name,
                     flatten_acts=False,
@@ -44,7 +45,13 @@
                     if model_name in helper.ALIGNED_MODELS:
                         if module_name == helper.ALIGNED_MODELS[model_name]:
                             print(f"\nAligning representations extracted from layer: {module_name} of model: {model_name}")
                             aligned_features = extractor.align(features=features, module_name=module_name)
                             print(f"Successfully aligned the representation space of model: {model_name}\n")
                             self.assertTrue(isinstance(aligned_features, Array))
                             self.assertEqual(aligned_features.shape, features.shape)
+
+            # cleanup downloaded torch models
+            torch_home = get_torch_home()
+            if os.path.exists(torch_home):
+                shutil.rmtree(torch_home)
+                os.makedirs(torch_home, exist_ok=True)
```

### Comparing `thingsvision-2.6.4/tests/extractor/extraction/test_torch_vs_tensorflow.py` & `thingsvision-2.6.5/tests/extractor/extraction/test_torch_vs_tensorflow.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.6.4/tests/extractor/test_load_extractor.py` & `thingsvision-2.6.5/tests/extractor/test_load_extractor.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.6.4/tests/extractor/test_transformations.py` & `thingsvision-2.6.5/tests/extractor/test_transformations.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.6.4/tests/helper.py` & `thingsvision-2.6.5/tests/helper.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 import torch
 import torch.nn as nn
 from tensorflow.keras.layers import Dense
 from tensorflow.keras.models import Sequential
 
 from thingsvision import get_extractor
 from thingsvision.utils.data import DataLoader, ImageDataset
+from torch.utils.data import Subset
 
 DATA_PATH = "./data"
 TEST_PATH = "./test_images"
 OUT_PATH = "./test"
 
 MODEL_AND_MODULE_NAMES = {
     # Torchvision models
@@ -205,14 +206,30 @@
     "DreamSim_mlp_dino_vitb16": {
         "model_name": "DreamSim",
         "modules": ["model.mlp"],
         "pretrained": True,
         "source": "custom",
         "kwargs": {"variant": "dino_vitb16"},
     },
+    "SegmentAnything_vit_b": {
+        "model_name": "SegmentAnything",
+        "modules": ["flatten"],
+        "pretrained": True,
+        "source": "custom",
+        "kwargs": {"variant": "vit_b"},
+        # model input size is large, therefore reduce test case on cpu
+        "batch_size": 1,
+        "num_samples": 1
+    },
+    "kakobrain_align_model": {
+        "model_name": "Kakaobrain_Align",
+        "modules": ["pooler"],
+        "pretrained": True,
+        "source": "custom",
+    },
 }
 
 ALIGNED_MODELS = {
     "alexnet": "classifier.4",
     "vgg16": "classifier.3",
     "resnet18": "avgpool",
     "resnet50": "avgpool",
@@ -308,24 +325,30 @@
 
 def iterate_through_all_model_combinations():
     for model_config in MODEL_AND_MODULE_NAMES.values():
         model_name = model_config["model_name"]
         pretrained = model_config["pretrained"]
         source = model_config["source"]
         kwargs = model_config.get("kwargs", {})
+
+        # we can set batch size and num_samples to reduce load for large models requiring a large image size
+        batch_size = model_config.get("batch_size", BATCH_SIZE)
+        num_samples = model_config.get("num_samples", NUM_SAMPLES)
+
         extractor, dataset, batches = create_extractor_and_dataloader(
-            model_name, pretrained, source, kwargs
+            model_name, pretrained, source, kwargs, batch_size, num_samples
         )
 
         modules = model_config["modules"]
         yield extractor, dataset, batches, modules, model_name
 
 
 def create_extractor_and_dataloader(
-    model_name: str, pretrained: bool, source: str, kwargs: dict = {}
+        model_name: str, pretrained: bool, source: str, kwargs: dict = {},
+        batch_size: int = BATCH_SIZE, num_samples: int = NUM_SAMPLES
 ):
     """Iterate through models and create model, dataset and data loader."""
     extractor = get_extractor(
         model_name=model_name,
         pretrained=pretrained,
         device=DEVICE,
         source=source,
@@ -333,17 +356,22 @@
     )
     dataset = ImageDataset(
         root=TEST_PATH,
         out_path=OUT_PATH,
         backend=extractor.get_backend(),
         transforms=extractor.get_transformations(),
     )
+    if num_samples > NUM_SAMPLES:
+        raise ValueError("\nNumber of samples in test case cannot be larger than the default value, only smaller.\n")
+    elif num_samples < NUM_SAMPLES:
+        dataset = Subset(dataset, np.arange(num_samples))
+
     batches = DataLoader(
         dataset,
-        batch_size=BATCH_SIZE,
+        batch_size=batch_size,
         backend=extractor.get_backend(),
     )
     return extractor, dataset, batches
 
 
 def create_test_images(n_samples: int = NUM_SAMPLES) -> None:
     """Create an artificial image dataset to be used for performing tests."""
```

### Comparing `thingsvision-2.6.4/tests/test_features.py` & `thingsvision-2.6.5/tests/test_features.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.6.4/tests/test_rest.py` & `thingsvision-2.6.5/tests/test_rest.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.6.4/thingsvision/core/cka/cka_base.py` & `thingsvision-2.6.5/thingsvision/core/cka/cka_base.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.6.4/thingsvision/core/cka/cka_numpy.py` & `thingsvision-2.6.5/thingsvision/core/cka/cka_numpy.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.6.4/thingsvision/core/cka/cka_torch.py` & `thingsvision-2.6.5/thingsvision/core/cka/cka_torch.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.6.4/thingsvision/core/cka/helpers.py` & `thingsvision-2.6.5/thingsvision/core/cka/helpers.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.6.4/thingsvision/core/extraction/base.py` & `thingsvision-2.6.5/thingsvision/core/extraction/base.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.6.4/thingsvision/core/extraction/extractors.py` & `thingsvision-2.6.5/thingsvision/core/extraction/extractors.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.6.4/thingsvision/core/extraction/helpers.py` & `thingsvision-2.6.5/thingsvision/core/extraction/helpers.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.6.4/thingsvision/core/extraction/tensorflow.py` & `thingsvision-2.6.5/thingsvision/core/extraction/tensorflow.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.6.4/thingsvision/core/extraction/torch.py` & `thingsvision-2.6.5/thingsvision/core/extraction/torch.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.6.4/thingsvision/core/rsa/helpers.py` & `thingsvision-2.6.5/thingsvision/core/rsa/helpers.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.6.4/thingsvision/custom_models/alexnet_ecoset.py` & `thingsvision-2.6.5/thingsvision/custom_models/alexnet_ecoset.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.6.4/thingsvision/custom_models/alexnet_salobjsub.py` & `thingsvision-2.6.5/thingsvision/custom_models/alexnet_salobjsub.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.6.4/thingsvision/custom_models/cornet/__init__.py` & `thingsvision-2.6.5/thingsvision/custom_models/cornet/__init__.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.6.4/thingsvision/custom_models/cornet/cornet_r.py` & `thingsvision-2.6.5/thingsvision/custom_models/cornet/cornet_r.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.6.4/thingsvision/custom_models/cornet/cornet_rt.py` & `thingsvision-2.6.5/thingsvision/custom_models/cornet/cornet_rt.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.6.4/thingsvision/custom_models/cornet/cornet_s.py` & `thingsvision-2.6.5/thingsvision/custom_models/cornet/cornet_s.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.6.4/thingsvision/custom_models/cornet/cornet_z.py` & `thingsvision-2.6.5/thingsvision/custom_models/cornet/cornet_z.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.6.4/thingsvision/custom_models/dreamsim/dreamsim.py` & `thingsvision-2.6.5/thingsvision/custom_models/dreamsim/dreamsim.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.6.4/thingsvision/custom_models/harmonization/harmonization.py` & `thingsvision-2.6.5/thingsvision/custom_models/harmonization/harmonization.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.6.4/thingsvision/custom_models/inception_ecoset.py` & `thingsvision-2.6.5/thingsvision/custom_models/inception_ecoset.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.6.4/thingsvision/custom_models/openclip.py` & `thingsvision-2.6.5/thingsvision/custom_models/openclip.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.6.4/thingsvision/custom_models/resnet50_ecoset.py` & `thingsvision-2.6.5/thingsvision/custom_models/resnet50_ecoset.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.6.4/thingsvision/custom_models/vgg16_ecoset.py` & `thingsvision-2.6.5/thingsvision/custom_models/vgg16_ecoset.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.6.4/thingsvision/custom_models/vgg16bn_ecoset.py` & `thingsvision-2.6.5/thingsvision/custom_models/vgg16bn_ecoset.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.6.4/thingsvision/thingsvision.py` & `thingsvision-2.6.5/thingsvision/thingsvision.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.6.4/thingsvision/utils/alignment/transforms.py` & `thingsvision-2.6.5/thingsvision/utils/alignment/transforms.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.6.4/thingsvision/utils/checkpointing/__init__.py` & `thingsvision-2.6.5/thingsvision/utils/checkpointing/__init__.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.6.4/thingsvision/utils/data/__init__.py` & `thingsvision-2.6.5/thingsvision/utils/data/__init__.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.6.4/thingsvision/utils/data/data_loader.py` & `thingsvision-2.6.5/thingsvision/utils/data/data_loader.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.6.4/thingsvision/utils/data/dataset.py` & `thingsvision-2.6.5/thingsvision/utils/data/dataset.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.6.4/thingsvision/utils/data/helpers.py` & `thingsvision-2.6.5/thingsvision/utils/data/helpers.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.6.4/thingsvision/utils/imagenet/__init__.py` & `thingsvision-2.6.5/thingsvision/utils/imagenet/__init__.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.6.4/thingsvision/utils/models/dino/utils.py` & `thingsvision-2.6.5/thingsvision/utils/models/dino/utils.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.6.4/thingsvision/utils/models/dino/vision_transformer.py` & `thingsvision-2.6.5/thingsvision/utils/models/dino/vision_transformer.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.6.4/thingsvision/utils/models/mae/utils.py` & `thingsvision-2.6.5/thingsvision/utils/models/mae/utils.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.6.4/thingsvision/utils/models/mae/vit_mae.py` & `thingsvision-2.6.5/thingsvision/utils/models/mae/vit_mae.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.6.4/thingsvision/utils/storing/helpers.py` & `thingsvision-2.6.5/thingsvision/utils/storing/helpers.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.6.4/thingsvision.egg-info/PKG-INFO` & `thingsvision-2.6.5/thingsvision.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thingsvision
-Version: 2.6.4
+Version: 2.6.5
 Summary: Extracting image features from state-of-the-art neural networks for Computer Vision made easy
 Home-page: https://github.com/ViCCo-Group/thingsvision
 Author: Lukas Muttenthaler
 Author-email: muttenthaler@cbs.mpg.de
 License: MIT License
 Keywords: feature extraction
 Classifier: Programming Language :: Python :: 3.8
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: thingsvision Version: 2.6.4 Summary: Extracting
+Metadata-Version: 2.1 Name: thingsvision Version: 2.6.5 Summary: Extracting
 image features from state-of-the-art neural networks for Computer Vision made
 easy Home-page: https://github.com/ViCCo-Group/thingsvision Author: Lukas
 Muttenthaler Author-email: muttenthaler@cbs.mpg.de License: MIT License
 Keywords: feature extraction Classifier: Programming Language :: Python :: 3.8
 Classifier: Natural Language :: English Classifier: License :: OSI Approved ::
 MIT License Classifier: Operating System :: OS Independent Requires-Python:
 >=3.8 Description-Content-Type: text/markdown License-File: LICENSE
```

### Comparing `thingsvision-2.6.4/thingsvision.egg-info/SOURCES.txt` & `thingsvision-2.6.5/thingsvision.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -36,19 +36,21 @@
 thingsvision/core/extraction/torch.py
 thingsvision/core/rsa/__init__.py
 thingsvision/core/rsa/base.py
 thingsvision/core/rsa/helpers.py
 thingsvision/custom_models/__init__.py
 thingsvision/custom_models/alexnet_ecoset.py
 thingsvision/custom_models/alexnet_salobjsub.py
+thingsvision/custom_models/align.py
 thingsvision/custom_models/custom.py
 thingsvision/custom_models/inception_ecoset.py
 thingsvision/custom_models/official_clip.py
 thingsvision/custom_models/openclip.py
 thingsvision/custom_models/resnet50_ecoset.py
+thingsvision/custom_models/sam.py
 thingsvision/custom_models/vgg16_ecoset.py
 thingsvision/custom_models/vgg16bn_ecoset.py
 thingsvision/custom_models/cornet/__init__.py
 thingsvision/custom_models/cornet/cornet_r.py
 thingsvision/custom_models/cornet/cornet_rt.py
 thingsvision/custom_models/cornet/cornet_s.py
 thingsvision/custom_models/cornet/cornet_z.py
```

