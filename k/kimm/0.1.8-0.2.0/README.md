# Comparing `tmp/kimm-0.1.8.tar.gz` & `tmp/kimm-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kimm-0.1.8.tar", last modified: Sat Mar 23 11:30:21 2024, max compression
+gzip compressed data, was "kimm-0.2.0.tar", last modified: Thu May 16 09:29:44 2024, max compression
```

## Comparing `kimm-0.1.8.tar` & `kimm-0.2.0.tar`

### file list

```diff
@@ -1,72 +1,125 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 11:30:21.237134 kimm-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-03-23 11:29:06.000000 kimm-0.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    10910 2024-03-23 11:30:21.237134 kimm-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9041 2024-03-23 11:29:06.000000 kimm-0.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 11:30:21.225134 kimm-0.1.8/kimm/
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-03-23 11:29:06.000000 kimm-0.1.8/kimm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 11:30:21.225134 kimm-0.1.8/kimm/blocks/
--rw-r--r--   0 runner    (1001) docker     (127)      451 2024-03-23 11:29:06.000000 kimm-0.1.8/kimm/blocks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3782 2024-03-23 11:29:06.000000 kimm-0.1.8/kimm/blocks/base_block.py
--rw-r--r--   0 runner    (1001) docker     (127)     1863 2024-03-23 11:29:06.000000 kimm-0.1.8/kimm/blocks/depthwise_separation_block.py
--rw-r--r--   0 runner    (1001) docker     (127)     2381 2024-03-23 11:29:06.000000 kimm-0.1.8/kimm/blocks/inverted_residual_block.py
--rw-r--r--   0 runner    (1001) docker     (127)     2343 2024-03-23 11:29:06.000000 kimm-0.1.8/kimm/blocks/transformer_block.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 11:30:21.225134 kimm-0.1.8/kimm/export/
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-03-23 11:29:06.000000 kimm-0.1.8/kimm/export/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2600 2024-03-23 11:29:06.000000 kimm-0.1.8/kimm/export/export_onnx.py
--rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-03-23 11:29:06.000000 kimm-0.1.8/kimm/export/export_onnx_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3532 2024-03-23 11:29:06.000000 kimm-0.1.8/kimm/export/export_tflite.py
--rw-r--r--   0 runner    (1001) docker     (127)     2261 2024-03-23 11:29:06.000000 kimm-0.1.8/kimm/export/export_tflite_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 11:30:21.229134 kimm-0.1.8/kimm/layers/
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-03-23 11:29:06.000000 kimm-0.1.8/kimm/layers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3933 2024-03-23 11:29:06.000000 kimm-0.1.8/kimm/layers/attention.py
--rw-r--r--   0 runner    (1001) docker     (127)      646 2024-03-23 11:29:06.000000 kimm-0.1.8/kimm/layers/attention_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1689 2024-03-23 11:29:06.000000 kimm-0.1.8/kimm/layers/layer_scale.py
--rw-r--r--   0 runner    (1001) docker     (127)      623 2024-03-23 11:29:06.000000 kimm-0.1.8/kimm/layers/layer_scale_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-03-23 11:29:06.000000 kimm-0.1.8/kimm/layers/learnable_affine.py
--rw-r--r--   0 runner    (1001) docker     (127)      670 2024-03-23 11:29:06.000000 kimm-0.1.8/kimm/layers/learnable_affine_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    13626 2024-03-23 11:29:06.000000 kimm-0.1.8/kimm/layers/mobile_one_conv2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     4922 2024-03-23 11:29:06.000000 kimm-0.1.8/kimm/layers/mobile_one_conv2d_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1320 2024-03-23 11:29:06.000000 kimm-0.1.8/kimm/layers/position_embedding.py
--rw-r--r--   0 runner    (1001) docker     (127)      986 2024-03-23 11:29:06.000000 kimm-0.1.8/kimm/layers/position_embedding_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    10617 2024-03-23 11:29:06.000000 kimm-0.1.8/kimm/layers/rep_conv2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     3960 2024-03-23 11:29:06.000000 kimm-0.1.8/kimm/layers/rep_conv2d_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 11:30:21.233134 kimm-0.1.8/kimm/models/
--rw-r--r--   0 runner    (1001) docker     (127)      930 2024-03-23 11:29:06.000000 kimm-0.1.8/kimm/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8469 2024-03-23 11:29:06.000000 kimm-0.1.8/kimm/models/base_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2384 2024-03-23 11:29:06.000000 kimm-0.1.8/kimm/models/base_model_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     7795 2024-03-23 11:29:06.000000 kimm-0.1.8/kimm/models/convmixer.py
--rw-r--r--   0 runner    (1001) docker     (127)    18828 2024-03-23 11:29:06.000000 kimm-0.1.8/kimm/models/convnext.py
--rw-r--r--   0 runner    (1001) docker     (127)    10204 2024-03-23 11:29:06.000000 kimm-0.1.8/kimm/models/densenet.py
--rw-r--r--   0 runner    (1001) docker     (127)    52040 2024-03-23 11:29:06.000000 kimm-0.1.8/kimm/models/efficientnet.py
--rw-r--r--   0 runner    (1001) docker     (127)    18111 2024-03-23 11:29:06.000000 kimm-0.1.8/kimm/models/ghostnet.py
--rw-r--r--   0 runner    (1001) docker     (127)    28970 2024-03-23 11:29:06.000000 kimm-0.1.8/kimm/models/hgnet.py
--rw-r--r--   0 runner    (1001) docker     (127)    11352 2024-03-23 11:29:06.000000 kimm-0.1.8/kimm/models/inception_next.py
--rw-r--r--   0 runner    (1001) docker     (127)    11498 2024-03-23 11:29:06.000000 kimm-0.1.8/kimm/models/inception_v3.py
--rw-r--r--   0 runner    (1001) docker     (127)    11301 2024-03-23 11:29:06.000000 kimm-0.1.8/kimm/models/mobilenet_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)    27587 2024-03-23 11:29:06.000000 kimm-0.1.8/kimm/models/mobilenet_v3.py
--rw-r--r--   0 runner    (1001) docker     (127)    11100 2024-03-23 11:29:06.000000 kimm-0.1.8/kimm/models/mobileone.py
--rw-r--r--   0 runner    (1001) docker     (127)    31980 2024-03-23 11:29:06.000000 kimm-0.1.8/kimm/models/mobilevit.py
--rw-r--r--   0 runner    (1001) docker     (127)    16367 2024-03-23 11:29:06.000000 kimm-0.1.8/kimm/models/models_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    37674 2024-03-23 11:29:06.000000 kimm-0.1.8/kimm/models/regnet.py
--rw-r--r--   0 runner    (1001) docker     (127)    14125 2024-03-23 11:29:06.000000 kimm-0.1.8/kimm/models/repvgg.py
--rw-r--r--   0 runner    (1001) docker     (127)    11593 2024-03-23 11:29:06.000000 kimm-0.1.8/kimm/models/resnet.py
--rw-r--r--   0 runner    (1001) docker     (127)     9355 2024-03-23 11:29:06.000000 kimm-0.1.8/kimm/models/vgg.py
--rw-r--r--   0 runner    (1001) docker     (127)    17295 2024-03-23 11:29:06.000000 kimm-0.1.8/kimm/models/vision_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)     5972 2024-03-23 11:29:06.000000 kimm-0.1.8/kimm/models/xception.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 11:30:21.233134 kimm-0.1.8/kimm/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      332 2024-03-23 11:29:06.000000 kimm-0.1.8/kimm/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-03-23 11:29:06.000000 kimm-0.1.8/kimm/utils/make_divisble.py
--rw-r--r--   0 runner    (1001) docker     (127)     3219 2024-03-23 11:29:06.000000 kimm-0.1.8/kimm/utils/model_registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     3580 2024-03-23 11:29:06.000000 kimm-0.1.8/kimm/utils/model_registry_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-03-23 11:29:06.000000 kimm-0.1.8/kimm/utils/model_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-03-23 11:29:06.000000 kimm-0.1.8/kimm/utils/model_utils_test.py
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-03-23 11:29:06.000000 kimm-0.1.8/kimm/utils/module_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4839 2024-03-23 11:29:06.000000 kimm-0.1.8/kimm/utils/timm_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 11:30:21.233134 kimm-0.1.8/kimm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10910 2024-03-23 11:30:21.000000 kimm-0.1.8/kimm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1690 2024-03-23 11:30:21.000000 kimm-0.1.8/kimm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-23 11:30:21.000000 kimm-0.1.8/kimm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-03-23 11:30:21.000000 kimm-0.1.8/kimm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-03-23 11:30:21.000000 kimm-0.1.8/kimm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2853 2024-03-23 11:29:06.000000 kimm-0.1.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-23 11:30:21.237134 kimm-0.1.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:29:44.044131 kimm-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-16 09:28:33.000000 kimm-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    10993 2024-05-16 09:29:44.044131 kimm-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9041 2024-05-16 09:28:33.000000 kimm-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:29:44.028131 kimm-0.2.0/kimm/
+-rw-r--r--   0 runner    (1001) docker     (127)      385 2024-05-16 09:28:33.000000 kimm-0.2.0/kimm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:29:44.028131 kimm-0.2.0/kimm/_src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:29:44.028131 kimm-0.2.0/kimm/_src/blocks/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 09:28:33.000000 kimm-0.2.0/kimm/_src/blocks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2115 2024-05-16 09:28:33.000000 kimm-0.2.0/kimm/_src/blocks/conv2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1969 2024-05-16 09:28:33.000000 kimm-0.2.0/kimm/_src/blocks/depthwise_separation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2506 2024-05-16 09:28:33.000000 kimm-0.2.0/kimm/_src/blocks/inverted_residual.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-05-16 09:28:33.000000 kimm-0.2.0/kimm/_src/blocks/squeeze_and_excitation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2471 2024-05-16 09:28:33.000000 kimm-0.2.0/kimm/_src/blocks/transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:29:44.032132 kimm-0.2.0/kimm/_src/export/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 09:28:33.000000 kimm-0.2.0/kimm/_src/export/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2709 2024-05-16 09:28:33.000000 kimm-0.2.0/kimm/_src/export/export_onnx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-05-16 09:28:33.000000 kimm-0.2.0/kimm/_src/export/export_onnx_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3647 2024-05-16 09:28:33.000000 kimm-0.2.0/kimm/_src/export/export_tflite.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2355 2024-05-16 09:28:33.000000 kimm-0.2.0/kimm/_src/export/export_tflite_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2867 2024-05-16 09:28:33.000000 kimm-0.2.0/kimm/_src/kimm_export.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:29:44.032132 kimm-0.2.0/kimm/_src/layers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 09:28:33.000000 kimm-0.2.0/kimm/_src/layers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4022 2024-05-16 09:28:33.000000 kimm-0.2.0/kimm/_src/layers/attention.py
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-05-16 09:28:33.000000 kimm-0.2.0/kimm/_src/layers/attention_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1692 2024-05-16 09:28:33.000000 kimm-0.2.0/kimm/_src/layers/layer_scale.py
+-rw-r--r--   0 runner    (1001) docker     (127)      628 2024-05-16 09:28:33.000000 kimm-0.2.0/kimm/_src/layers/layer_scale_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-05-16 09:28:33.000000 kimm-0.2.0/kimm/_src/layers/learnable_affine.py
+-rw-r--r--   0 runner    (1001) docker     (127)      675 2024-05-16 09:28:33.000000 kimm-0.2.0/kimm/_src/layers/learnable_affine_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13715 2024-05-16 09:28:33.000000 kimm-0.2.0/kimm/_src/layers/mobile_one_conv2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4927 2024-05-16 09:28:33.000000 kimm-0.2.0/kimm/_src/layers/mobile_one_conv2d_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1409 2024-05-16 09:28:33.000000 kimm-0.2.0/kimm/_src/layers/position_embedding.py
+-rw-r--r--   0 runner    (1001) docker     (127)      991 2024-05-16 09:28:33.000000 kimm-0.2.0/kimm/_src/layers/position_embedding_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10706 2024-05-16 09:28:33.000000 kimm-0.2.0/kimm/_src/layers/rep_conv2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3965 2024-05-16 09:28:33.000000 kimm-0.2.0/kimm/_src/layers/rep_conv2d_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:29:44.036131 kimm-0.2.0/kimm/_src/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      755 2024-05-16 09:28:33.000000 kimm-0.2.0/kimm/_src/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8660 2024-05-16 09:28:33.000000 kimm-0.2.0/kimm/_src/models/base_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6873 2024-05-16 09:28:33.000000 kimm-0.2.0/kimm/_src/models/convmixer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12992 2024-05-16 09:28:33.000000 kimm-0.2.0/kimm/_src/models/convnext.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8266 2024-05-16 09:28:33.000000 kimm-0.2.0/kimm/_src/models/densenet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29575 2024-05-16 09:28:33.000000 kimm-0.2.0/kimm/_src/models/efficientnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14324 2024-05-16 09:28:33.000000 kimm-0.2.0/kimm/_src/models/ghostnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21491 2024-05-16 09:28:33.000000 kimm-0.2.0/kimm/_src/models/hgnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10497 2024-05-16 09:28:33.000000 kimm-0.2.0/kimm/_src/models/inception_next.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11683 2024-05-16 09:28:33.000000 kimm-0.2.0/kimm/_src/models/inception_v3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8410 2024-05-16 09:28:33.000000 kimm-0.2.0/kimm/_src/models/mobilenet_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19121 2024-05-16 09:28:33.000000 kimm-0.2.0/kimm/_src/models/mobilenet_v3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9027 2024-05-16 09:28:33.000000 kimm-0.2.0/kimm/_src/models/mobileone.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26230 2024-05-16 09:28:33.000000 kimm-0.2.0/kimm/_src/models/mobilevit.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19067 2024-05-16 09:28:33.000000 kimm-0.2.0/kimm/_src/models/models_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18229 2024-05-16 09:28:33.000000 kimm-0.2.0/kimm/_src/models/regnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9112 2024-05-16 09:28:33.000000 kimm-0.2.0/kimm/_src/models/repvgg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8700 2024-05-16 09:28:33.000000 kimm-0.2.0/kimm/_src/models/resnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7235 2024-05-16 09:28:33.000000 kimm-0.2.0/kimm/_src/models/vgg.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11292 2024-05-16 09:28:33.000000 kimm-0.2.0/kimm/_src/models/vision_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6114 2024-05-16 09:28:33.000000 kimm-0.2.0/kimm/_src/models/xception.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:29:44.036131 kimm-0.2.0/kimm/_src/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 09:28:33.000000 kimm-0.2.0/kimm/_src/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-05-16 09:28:33.000000 kimm-0.2.0/kimm/_src/utils/make_divisble.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3339 2024-05-16 09:28:33.000000 kimm-0.2.0/kimm/_src/utils/model_registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3605 2024-05-16 09:28:33.000000 kimm-0.2.0/kimm/_src/utils/model_registry_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1197 2024-05-16 09:28:33.000000 kimm-0.2.0/kimm/_src/utils/model_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-05-16 09:28:33.000000 kimm-0.2.0/kimm/_src/utils/model_utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-16 09:28:33.000000 kimm-0.2.0/kimm/_src/utils/module_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5070 2024-05-16 09:28:33.000000 kimm-0.2.0/kimm/_src/utils/timm_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-05-16 09:28:33.000000 kimm-0.2.0/kimm/_src/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:29:44.036131 kimm-0.2.0/kimm/blocks/
+-rw-r--r--   0 runner    (1001) docker     (127)      535 2024-05-16 09:28:33.000000 kimm-0.2.0/kimm/blocks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:29:44.036131 kimm-0.2.0/kimm/export/
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-05-16 09:28:33.000000 kimm-0.2.0/kimm/export/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:29:44.036131 kimm-0.2.0/kimm/layers/
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-05-16 09:28:33.000000 kimm-0.2.0/kimm/layers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:29:44.036131 kimm-0.2.0/kimm/models/
+-rw-r--r--   0 runner    (1001) docker     (127)     8268 2024-05-16 09:28:33.000000 kimm-0.2.0/kimm/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:29:44.040131 kimm-0.2.0/kimm/models/base_model/
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-16 09:28:33.000000 kimm-0.2.0/kimm/models/base_model/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:29:44.040131 kimm-0.2.0/kimm/models/convmixer/
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-05-16 09:28:33.000000 kimm-0.2.0/kimm/models/convmixer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:29:44.040131 kimm-0.2.0/kimm/models/convnext/
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-05-16 09:28:33.000000 kimm-0.2.0/kimm/models/convnext/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:29:44.040131 kimm-0.2.0/kimm/models/densenet/
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-16 09:28:33.000000 kimm-0.2.0/kimm/models/densenet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:29:44.040131 kimm-0.2.0/kimm/models/efficientnet/
+-rw-r--r--   0 runner    (1001) docker     (127)     1607 2024-05-16 09:28:33.000000 kimm-0.2.0/kimm/models/efficientnet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:29:44.040131 kimm-0.2.0/kimm/models/ghostnet/
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-05-16 09:28:33.000000 kimm-0.2.0/kimm/models/ghostnet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:29:44.040131 kimm-0.2.0/kimm/models/hgnet/
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-05-16 09:28:33.000000 kimm-0.2.0/kimm/models/hgnet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:29:44.040131 kimm-0.2.0/kimm/models/inception_next/
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-05-16 09:28:33.000000 kimm-0.2.0/kimm/models/inception_next/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:29:44.040131 kimm-0.2.0/kimm/models/inception_v3/
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-16 09:28:33.000000 kimm-0.2.0/kimm/models/inception_v3/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:29:44.040131 kimm-0.2.0/kimm/models/mobilenet_v2/
+-rw-r--r--   0 runner    (1001) docker     (127)      412 2024-05-16 09:28:33.000000 kimm-0.2.0/kimm/models/mobilenet_v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:29:44.040131 kimm-0.2.0/kimm/models/mobilenet_v3/
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-05-16 09:28:33.000000 kimm-0.2.0/kimm/models/mobilenet_v3/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:29:44.040131 kimm-0.2.0/kimm/models/mobileone/
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-05-16 09:28:33.000000 kimm-0.2.0/kimm/models/mobileone/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:29:44.040131 kimm-0.2.0/kimm/models/mobilevit/
+-rw-r--r--   0 runner    (1001) docker     (127)      660 2024-05-16 09:28:33.000000 kimm-0.2.0/kimm/models/mobilevit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:29:44.040131 kimm-0.2.0/kimm/models/regnet/
+-rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-05-16 09:28:33.000000 kimm-0.2.0/kimm/models/regnet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:29:44.040131 kimm-0.2.0/kimm/models/repvgg/
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-05-16 09:28:33.000000 kimm-0.2.0/kimm/models/repvgg/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:29:44.040131 kimm-0.2.0/kimm/models/resnet/
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-05-16 09:28:33.000000 kimm-0.2.0/kimm/models/resnet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:29:44.040131 kimm-0.2.0/kimm/models/vgg/
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-05-16 09:28:33.000000 kimm-0.2.0/kimm/models/vgg/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:29:44.040131 kimm-0.2.0/kimm/models/vision_transformer/
+-rw-r--r--   0 runner    (1001) docker     (127)      702 2024-05-16 09:28:33.000000 kimm-0.2.0/kimm/models/vision_transformer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:29:44.040131 kimm-0.2.0/kimm/models/xception/
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-16 09:28:33.000000 kimm-0.2.0/kimm/models/xception/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:29:44.040131 kimm-0.2.0/kimm/timm_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2024-05-16 09:28:33.000000 kimm-0.2.0/kimm/timm_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:29:44.040131 kimm-0.2.0/kimm/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-05-16 09:28:33.000000 kimm-0.2.0/kimm/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:29:44.040131 kimm-0.2.0/kimm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10993 2024-05-16 09:29:44.000000 kimm-0.2.0/kimm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2783 2024-05-16 09:29:44.000000 kimm-0.2.0/kimm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 09:29:44.000000 kimm-0.2.0/kimm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-05-16 09:29:44.000000 kimm-0.2.0/kimm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-16 09:29:44.000000 kimm-0.2.0/kimm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2869 2024-05-16 09:28:33.000000 kimm-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 09:29:44.044131 kimm-0.2.0/setup.cfg
```

### Comparing `kimm-0.1.8/LICENSE` & `kimm-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `kimm-0.1.8/PKG-INFO` & `kimm-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kimm
-Version: 0.1.8
+Version: 0.2.0
 Summary: A Keras model zoo with pretrained weights.
 Author-email: Hong-Yu Chiu <james77777778@gmail.com>
 Maintainer-email: Hong-Yu Chiu <james77777778@gmail.com>
 License: Apache License 2.0
 Project-URL: Homepage, https://github.com/james77777778/keras-image-models
 Project-URL: Documentation, https://github.com/james77777778/keras-image-models
 Project-URL: Repository, https://github.com/james77777778/keras-image-models.git
@@ -33,25 +33,27 @@
 Requires-Dist: onnxsim; extra == "tests"
 Requires-Dist: isort; extra == "tests"
 Requires-Dist: ruff; extra == "tests"
 Requires-Dist: black; extra == "tests"
 Requires-Dist: pytest; extra == "tests"
 Requires-Dist: pytest-cov; extra == "tests"
 Requires-Dist: coverage; extra == "tests"
+Requires-Dist: pre-commit; extra == "tests"
+Requires-Dist: namex; extra == "tests"
 Provides-Extra: examples
 Requires-Dist: opencv-python; extra == "examples"
 Requires-Dist: matplotlib; extra == "examples"
 
 <!-- markdownlint-disable MD033 -->
 <!-- markdownlint-disable MD041 -->
 
 <div align="center">
 <img width="50%" src="https://github.com/james77777778/kimm/assets/20734616/b21db8f2-307b-4791-b93d-e913e45fb238" alt="KIMM">
 
-[![Keras](https://img.shields.io/badge/keras-v3.0.4+-success.svg)](https://github.com/keras-team/keras)
+[![Keras](https://img.shields.io/badge/keras-v3.3.0+-success.svg)](https://github.com/keras-team/keras)
 [![PyPI](https://img.shields.io/pypi/v/kimm)](https://pypi.org/project/kimm/)
 [![Contributions Welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat)](https://github.com/james77777778/kimm/issues)
 [![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/james77777778/keras-image-models/actions.yml?label=tests)](https://github.com/james77777778/keras-image-models/actions/workflows/actions.yml?query=branch%3Amain++)
 [![codecov](https://codecov.io/gh/james77777778/keras-image-models/graph/badge.svg?token=eEha1SR80D)](https://codecov.io/gh/james77777778/keras-image-models)
 </div>
 
 # Keras Image Models
```

### Comparing `kimm-0.1.8/README.md` & `kimm-0.2.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!-- markdownlint-disable MD033 -->
 <!-- markdownlint-disable MD041 -->
 
 <div align="center">
 <img width="50%" src="https://github.com/james77777778/kimm/assets/20734616/b21db8f2-307b-4791-b93d-e913e45fb238" alt="KIMM">
 
-[![Keras](https://img.shields.io/badge/keras-v3.0.4+-success.svg)](https://github.com/keras-team/keras)
+[![Keras](https://img.shields.io/badge/keras-v3.3.0+-success.svg)](https://github.com/keras-team/keras)
 [![PyPI](https://img.shields.io/pypi/v/kimm)](https://pypi.org/project/kimm/)
 [![Contributions Welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat)](https://github.com/james77777778/kimm/issues)
 [![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/james77777778/keras-image-models/actions.yml?label=tests)](https://github.com/james77777778/keras-image-models/actions/workflows/actions.yml?query=branch%3Amain++)
 [![codecov](https://codecov.io/gh/james77777778/keras-image-models/graph/badge.svg?token=eEha1SR80D)](https://codecov.io/gh/james77777778/keras-image-models)
 </div>
 
 # Keras Image Models
```

### Comparing `kimm-0.1.8/kimm/blocks/base_block.py` & `kimm-0.2.0/kimm/_src/blocks/depthwise_separation.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,127 +1,65 @@
 import typing
 
 from keras import backend
 from keras import layers
 
-from kimm.utils import make_divisible
+from kimm._src.blocks.conv2d import apply_conv2d_block
+from kimm._src.blocks.squeeze_and_excitation import apply_se_block
+from kimm._src.kimm_export import kimm_export
 
 
-def apply_activation(
-    inputs, activation: typing.Optional[str] = None, name: str = "activation"
-):
-    x = inputs
-    if activation is not None:
-        if isinstance(activation, str):
-            x = layers.Activation(activation, name=name)(x)
-        elif isinstance(activation, layers.Layer):
-            x = activation(x)
-        else:
-            NotImplementedError(
-                f"Unsupported activation type: {type(activation)}"
-            )
-    return x
-
-
-def apply_conv2d_block(
+@kimm_export(parent_path=["kimm.blocks"])
+def apply_depthwise_separation_block(
     inputs,
-    filters: typing.Optional[int] = None,
-    kernel_size: typing.Optional[
-        typing.Union[int, typing.Sequence[int]]
-    ] = None,
+    output_channels: int,
+    depthwise_kernel_size: int = 3,
+    pointwise_kernel_size: int = 1,
     strides: int = 1,
-    groups: int = 1,
-    activation: typing.Optional[str] = None,
-    use_depthwise: bool = False,
-    add_skip: bool = False,
-    bn_momentum: float = 0.9,
+    se_ratio: float = 0.0,
+    activation: typing.Optional[str] = "swish",
+    se_activation: typing.Optional[str] = "relu",
+    se_gate_activation: typing.Optional[str] = "sigmoid",
+    se_make_divisible_number: typing.Optional[int] = None,
+    pw_activation: typing.Optional[str] = None,
+    skip: bool = True,
     bn_epsilon: float = 1e-5,
     padding: typing.Optional[typing.Literal["same", "valid"]] = None,
-    name="conv2d_block",
+    name: str = "depthwise_separation_block",
 ):
-    if kernel_size is None:
-        raise ValueError(
-            f"kernel_size must be passed. Received: kernel_size={kernel_size}"
-        )
-    if isinstance(kernel_size, int):
-        kernel_size = [kernel_size, kernel_size]
-
     channels_axis = -1 if backend.image_data_format() == "channels_last" else -3
     input_channels = inputs.shape[channels_axis]
-    has_skip = add_skip and strides == 1 and input_channels == filters
-    x = inputs
-
-    if padding is None:
-        padding = "same"
-        if strides > 1:
-            padding = "valid"
-            x = layers.ZeroPadding2D(
-                ((kernel_size[0] - 1) // 2, (kernel_size[1] - 1) // 2),
-                name=f"{name}_pad",
-            )(x)
+    has_skip = skip and (strides == 1 and input_channels == output_channels)
 
-    if not use_depthwise:
-        x = layers.Conv2D(
-            filters,
-            kernel_size,
-            strides,
-            padding=padding,
-            groups=groups,
-            use_bias=False,
-            name=f"{name}_conv2d",
-        )(x)
-    else:
-        x = layers.DepthwiseConv2D(
-            kernel_size,
-            strides,
-            padding=padding,
-            use_bias=False,
-            name=f"{name}_dwconv2d",
-        )(x)
-    x = layers.BatchNormalization(
-        axis=channels_axis,
-        name=f"{name}_bn",
-        momentum=bn_momentum,
-        epsilon=bn_epsilon,
-    )(x)
-    x = apply_activation(x, activation, name=name)
+    x = inputs
+    x = apply_conv2d_block(
+        x,
+        kernel_size=depthwise_kernel_size,
+        strides=strides,
+        activation=activation,
+        use_depthwise=True,
+        bn_epsilon=bn_epsilon,
+        padding=padding,
+        name=f"{name}_conv_dw",
+    )
+    if se_ratio > 0:
+        x = apply_se_block(
+            x,
+            se_ratio,
+            activation=se_activation,
+            gate_activation=se_gate_activation,
+            make_divisible_number=se_make_divisible_number,
+            name=f"{name}_se",
+        )
+    x = apply_conv2d_block(
+        x,
+        output_channels,
+        pointwise_kernel_size,
+        1,
+        activation=pw_activation,
+        bn_epsilon=bn_epsilon,
+        padding=padding,
+        name=f"{name}_conv_pw",
+    )
     if has_skip:
         x = layers.Add()([x, inputs])
     return x
-
-
-def apply_se_block(
-    inputs,
-    se_ratio: float = 0.25,
-    activation: typing.Optional[str] = "relu",
-    gate_activation: typing.Optional[str] = "sigmoid",
-    make_divisible_number: typing.Optional[int] = None,
-    se_input_channels: typing.Optional[int] = None,
-    name: str = "se_block",
-):
-    channels_axis = -1 if backend.image_data_format() == "channels_last" else -3
-    input_channels = inputs.shape[channels_axis]
-    if se_input_channels is None:
-        se_input_channels = input_channels
-    if make_divisible_number is None:
-        se_channels = round(se_input_channels * se_ratio)
-    else:
-        se_channels = make_divisible(
-            se_input_channels * se_ratio, make_divisible_number
-        )
-
-    x = inputs
-    x = layers.GlobalAveragePooling2D(
-        data_format=backend.image_data_format(),
-        keepdims=True,
-        name=f"{name}_mean",
-    )(x)
-    x = layers.Conv2D(
-        se_channels, 1, use_bias=True, name=f"{name}_conv_reduce"
-    )(x)
-    x = apply_activation(x, activation, name=f"{name}_act1")
-    x = layers.Conv2D(
-        input_channels, 1, use_bias=True, name=f"{name}_conv_expand"
-    )(x)
-    x = apply_activation(x, gate_activation, name=f"{name}_gate")
-    x = layers.Multiply(name=name)([inputs, x])
-    return x
```

### Comparing `kimm-0.1.8/kimm/blocks/depthwise_separation_block.py` & `kimm-0.2.0/kimm/_src/blocks/inverted_residual.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,63 +1,83 @@
 import typing
 
 from keras import backend
 from keras import layers
 
-from kimm.blocks.base_block import apply_conv2d_block
-from kimm.blocks.base_block import apply_se_block
+from kimm._src.blocks.conv2d import apply_conv2d_block
+from kimm._src.blocks.squeeze_and_excitation import apply_se_block
+from kimm._src.kimm_export import kimm_export
+from kimm._src.utils.make_divisble import make_divisible
 
 
-def apply_depthwise_separation_block(
+@kimm_export(parent_path=["kimm.blocks"])
+def apply_inverted_residual_block(
     inputs,
     output_channels: int,
     depthwise_kernel_size: int = 3,
+    expansion_kernel_size: int = 1,
     pointwise_kernel_size: int = 1,
     strides: int = 1,
+    expansion_ratio: float = 1.0,
     se_ratio: float = 0.0,
-    activation: typing.Optional[str] = "swish",
-    se_activation: typing.Optional[str] = "relu",
+    activation: str = "swish",
+    se_channels: typing.Optional[int] = None,
+    se_activation: typing.Optional[str] = None,
     se_gate_activation: typing.Optional[str] = "sigmoid",
     se_make_divisible_number: typing.Optional[int] = None,
-    pw_activation: typing.Optional[str] = None,
-    skip: bool = True,
     bn_epsilon: float = 1e-5,
     padding: typing.Optional[typing.Literal["same", "valid"]] = None,
-    name: str = "depthwise_separation_block",
+    name: str = "inverted_residual_block",
 ):
     channels_axis = -1 if backend.image_data_format() == "channels_last" else -3
     input_channels = inputs.shape[channels_axis]
-    has_skip = skip and (strides == 1 and input_channels == output_channels)
+    hidden_channels = make_divisible(input_channels * expansion_ratio)
+    has_skip = strides == 1 and input_channels == output_channels
 
     x = inputs
+    # Point-wise expansion
+    x = apply_conv2d_block(
+        x,
+        hidden_channels,
+        expansion_kernel_size,
+        1,
+        activation=activation,
+        bn_epsilon=bn_epsilon,
+        padding=padding,
+        name=f"{name}_conv_pw",
+    )
+    # Depth-wise convolution
     x = apply_conv2d_block(
         x,
         kernel_size=depthwise_kernel_size,
         strides=strides,
         activation=activation,
         use_depthwise=True,
         bn_epsilon=bn_epsilon,
         padding=padding,
         name=f"{name}_conv_dw",
     )
+    # Squeeze-and-excitation
     if se_ratio > 0:
         x = apply_se_block(
             x,
             se_ratio,
-            activation=se_activation,
+            activation=se_activation or activation,
             gate_activation=se_gate_activation,
+            se_input_channels=se_channels,
             make_divisible_number=se_make_divisible_number,
             name=f"{name}_se",
         )
+    # Point-wise linear projection
     x = apply_conv2d_block(
         x,
         output_channels,
         pointwise_kernel_size,
         1,
-        activation=pw_activation,
+        activation=None,
         bn_epsilon=bn_epsilon,
         padding=padding,
-        name=f"{name}_conv_pw",
+        name=f"{name}_conv_pwl",
     )
     if has_skip:
         x = layers.Add()([x, inputs])
     return x
```

### Comparing `kimm-0.1.8/kimm/blocks/transformer_block.py` & `kimm-0.2.0/kimm/_src/blocks/transformer.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 import typing
 
 from keras import backend
 from keras import layers
 
-from kimm import layers as kimm_layers
+from kimm._src.kimm_export import kimm_export
+from kimm._src.layers.attention import Attention
 
 
+@kimm_export(parent_path=["kimm.blocks"])
 def apply_mlp_block(
     inputs,
     hidden_dim: int,
     output_dim: typing.Optional[int] = None,
     activation: str = "gelu",
     use_bias: bool = True,
     dropout_rate: float = 0.0,
@@ -38,14 +40,15 @@
         )(x)
     else:
         x = layers.Dense(output_dim, use_bias=use_bias, name=f"{name}_fc2")(x)
     x = layers.Dropout(dropout_rate, name=f"{name}_drop2")(x)
     return x
 
 
+@kimm_export(parent_path=["kimm.blocks"])
 def apply_transformer_block(
     inputs,
     dim: int,
     num_heads: int,
     mlp_ratio: float = 4.0,
     use_qkv_bias: bool = False,
     use_qk_norm: bool = False,
@@ -54,15 +57,15 @@
     activation: str = "gelu",
     name: str = "transformer_block",
 ):
     x = inputs
     residual_1 = x
 
     x = layers.LayerNormalization(epsilon=1e-6, name=f"{name}_norm1")(x)
-    x = kimm_layers.Attention(
+    x = Attention(
         dim,
         num_heads,
         use_qkv_bias,
         use_qk_norm,
         attention_dropout_rate,
         projection_dropout_rate,
         name=f"{name}_attn",
```

### Comparing `kimm-0.1.8/kimm/export/export_onnx.py` & `kimm-0.2.0/kimm/_src/export/export_onnx.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,18 +2,20 @@
 import typing
 
 from keras import backend
 from keras import layers
 from keras import models
 from keras import ops
 
-from kimm.models import BaseModel
-from kimm.utils.module_utils import torch
+from kimm._src.kimm_export import kimm_export
+from kimm._src.models.base_model import BaseModel
+from kimm._src.utils.module_utils import torch
 
 
+@kimm_export(parent_path=["kimm.export"])
 def export_onnx(
     model: BaseModel,
     input_shape: typing.Union[int, typing.Sequence[int]],
     export_path: typing.Union[str, pathlib.Path],
     batch_size: int = 1,
 ):
     """Export the model to onnx format (in float32).
```

### Comparing `kimm-0.1.8/kimm/export/export_onnx_test.py` & `kimm-0.2.0/kimm/_src/export/export_tflite_test.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,36 +1,76 @@
 import pytest
 from absl.testing import parameterized
 from keras import backend
+from keras import ops
+from keras import random
 from keras.src import testing
 
-from kimm import export
-from kimm import models
+from kimm._src import models
+from kimm._src.export import export_tflite
 
 
-class ExportOnnxTest(testing.TestCase, parameterized.TestCase):
-    def get_model(self):
-        input_shape = [3, 224, 224]  # channels_first
-        model = models.MobileNetV3W050Small(include_preprocessing=False)
-        return input_shape, model
+class ExportTFLiteTest(testing.TestCase, parameterized.TestCase):
+    def get_model_and_representative_dataset(self):
+        input_shape = [224, 224, 3]
+        model = models.mobilenet_v3.MobileNetV3W050Small(
+            include_preprocessing=False, weights=None
+        )
+
+        def representative_dataset():
+            for _ in range(10):
+                yield [
+                    ops.convert_to_numpy(
+                        random.uniform([1, *input_shape], maxval=255.0)
+                    )
+                ]
+
+        return input_shape, model, representative_dataset
 
     @classmethod
     def setUpClass(cls):
         cls.original_image_data_format = backend.image_data_format()
 
     @classmethod
     def tearDownClass(cls):
         backend.set_image_data_format(cls.original_image_data_format)
 
     @pytest.mark.skipif(
-        backend.backend() != "torch", reason="Requires torch backend."
+        backend.backend() != "tensorflow", reason="Requires tensorflow backend."
+    )
+    def test_export_tflite_fp32(self):
+        (input_shape, model, _) = self.get_model_and_representative_dataset()
+        temp_dir = self.get_temp_dir()
+
+        export_tflite.export_tflite(
+            model, input_shape, f"{temp_dir}/model_fp32.onnx", "float32"
+        )
+
+    @pytest.mark.skipif(
+        backend.backend() != "tensorflow", reason="Requires tensorflow backend."
     )
-    def DISABLE_test_export_onnx_use(self):
-        # TODO: turn on this test
-        # SystemError: <method '__int__' of 'torch._C._TensorBase' objects>
-        # returned a result with an exception set
-        backend.set_image_data_format("channels_first")
-        input_shape, model = self.get_model()
+    def test_export_tflite_fp16(self):
+        (input_shape, model, _) = self.get_model_and_representative_dataset()
+        temp_dir = self.get_temp_dir()
+
+        export_tflite.export_tflite(
+            model, input_shape, f"{temp_dir}/model_fp16.tflite", "float16"
+        )
 
+    @pytest.mark.skipif(
+        backend.backend() != "tensorflow", reason="Requires tensorflow backend."
+    )
+    def test_export_tflite_int8(self):
+        (
+            input_shape,
+            model,
+            representative_dataset,
+        ) = self.get_model_and_representative_dataset()
         temp_dir = self.get_temp_dir()
 
-        export.export_onnx(model, input_shape, f"{temp_dir}/model.onnx")
+        export_tflite.export_tflite(
+            model,
+            input_shape,
+            f"{temp_dir}/model_int8.tflite",
+            "int8",
+            representative_dataset,
+        )
```

### Comparing `kimm-0.1.8/kimm/export/export_tflite.py` & `kimm-0.2.0/kimm/_src/export/export_tflite.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,46 +3,49 @@
 import typing
 
 from keras import backend
 from keras import layers
 from keras import models
 from keras.src.utils.module_utils import tensorflow as tf
 
-from kimm.models import BaseModel
+from kimm._src.kimm_export import kimm_export
+from kimm._src.models.base_model import BaseModel
 
 
+@kimm_export(parent_path=["kimm.export"])
 def export_tflite(
     model: BaseModel,
     input_shape: typing.Union[int, typing.Sequence[int]],
     export_path: typing.Union[str, pathlib.Path],
     export_dtype: typing.Literal["float32", "float16", "int8"] = "float32",
     representative_dataset: typing.Optional[typing.Iterator] = None,
     batch_size: int = 1,
 ):
     """Export the model to tflite format.
 
-    Only tensorflow backend with 'channels_last' is supported. The tflite model
-    will be generated using `tf.lite.TFLiteConverter.from_saved_model` and
-    optimized through tflite built-in functions.
+    Only TensorFlow backend with 'channels_last' is supported. The
+    tflite model will be generated using
+    `tf.lite.TFLiteConverter.from_saved_model` and optimized through tflite
+    built-in functions.
 
     Note that when exporting an `int8` tflite model, `representative_dataset`
     must be passed.
 
     Args:
         model: keras.Model, the model to be exported.
         input_shape: int or sequence of int, specifying the shape of the input.
         export_path: str or pathlib.Path, specifying the path to export.
         export_dtype: str, specifying the export dtype.
         representative_dataset: None or Iterator, the calibration dataset for
             exporting int8 tflite.
         batch_size: int, specifying the batch size of the input,
             defaults to `1`.
     """
-    if backend.backend() != "tensorflow":
-        raise ValueError("`export_tflite` only supports tensorflow backend")
+    if backend.backend() not in ("tensorflow",):
+        raise ValueError("`export_tflite` only supports TensorFlow backend")
     if backend.image_data_format() != "channels_last":
         raise ValueError(
             "`export_tflite` only supports 'channels_last' data format."
         )
     if export_dtype not in ("float32", "float16", "int8"):
         raise ValueError(
             "`export_dtype` must be one of ('float32', 'float16', 'int8'). "
```

### Comparing `kimm-0.1.8/kimm/layers/attention.py` & `kimm-0.2.0/kimm/_src/layers/attention.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 import keras
 from keras import layers
 from keras import ops
 
+from kimm._src.kimm_export import kimm_export
 
+
+@kimm_export(parent_path=["kimm.layers"])
 @keras.saving.register_keras_serializable(package="kimm")
 class Attention(layers.Layer):
     def __init__(
         self,
         hidden_dim: int,
         num_heads: int = 8,
         use_qkv_bias: bool = False,
```

### Comparing `kimm-0.1.8/kimm/layers/attention_test.py` & `kimm-0.2.0/kimm/_src/layers/attention_test.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import pytest
 from absl.testing import parameterized
 from keras.src import testing
 
-from kimm.layers.attention import Attention
+from kimm._src.layers.attention import Attention
 
 
 class AttentionTest(testing.TestCase, parameterized.TestCase):
     @pytest.mark.requires_trainable_backend
     def test_attention_basic(self):
         self.run_layer_test(
             Attention,
```

### Comparing `kimm-0.1.8/kimm/layers/layer_scale.py` & `kimm-0.2.0/kimm/_src/layers/layer_scale.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 import keras
 from keras import initializers
 from keras import layers
 from keras import ops
-from keras.initializers import Initializer
 
+from kimm._src.kimm_export import kimm_export
 
+
+@kimm_export(parent_path=["kimm.layers"])
 @keras.saving.register_keras_serializable(package="kimm")
 class LayerScale(layers.Layer):
     def __init__(
         self,
         axis: int = -1,
-        initializer: Initializer = initializers.Constant(1e-5),
+        initializer: initializers.Initializer = initializers.Constant(1e-5),
         **kwargs,
     ):
         super().__init__(**kwargs)
         self.axis = axis
         self.initializer = initializer
 
     def build(self, input_shape):
@@ -25,26 +27,23 @@
             self.axis = [self.axis]
         self.gamma = self.add_weight(
             shape, initializer=self.initializer, name="gamma"
         )
         self.built = True
 
     def call(self, inputs, training=None, mask=None):
-        inputs = ops.cast(inputs, self.compute_dtype)
-
         # Broadcasting only necessary for norm when the axis is not just
         # the last dimension
         input_shape = inputs.shape
         ndims = len(inputs.shape)
         broadcast_shape = [1] * ndims
         for dim in self.axis:
             broadcast_shape[dim] = input_shape[dim]
         gamma = ops.reshape(self.gamma, broadcast_shape)
         gamma = ops.cast(gamma, self.compute_dtype)
-
         return ops.multiply(inputs, gamma)
 
     def get_config(self):
         config = super().get_config()
         config.update(
             {
                 "axis": self.axis,
```

### Comparing `kimm-0.1.8/kimm/layers/layer_scale_test.py` & `kimm-0.2.0/kimm/_src/layers/layer_scale_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import pytest
 from absl.testing import parameterized
 from keras.src import testing
 
-from kimm.layers.layer_scale import LayerScale
+from kimm._src.layers.layer_scale import LayerScale
 
 
 class LayerScaleTest(testing.TestCase, parameterized.TestCase):
     @pytest.mark.requires_trainable_backend
     def test_layer_scale_basic(self):
         self.run_layer_test(
             LayerScale,
```

### Comparing `kimm-0.1.8/kimm/layers/learnable_affine.py` & `kimm-0.2.0/kimm/_src/layers/learnable_affine.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 import keras
 from keras import layers
 from keras import ops
 
+from kimm._src.kimm_export import kimm_export
 
+
+@kimm_export(parent_path=["kimm.layers"])
 @keras.saving.register_keras_serializable(package="kimm")
 class LearnableAffine(layers.Layer):
     def __init__(self, scale_value=1.0, bias_value=0.0, **kwargs):
         super().__init__(**kwargs)
         if isinstance(scale_value, int):
             raise ValueError(
                 f"scale_value must be a integer. Received: {scale_value}"
```

### Comparing `kimm-0.1.8/kimm/layers/learnable_affine_test.py` & `kimm-0.2.0/kimm/_src/layers/learnable_affine_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import pytest
 from absl.testing import parameterized
 from keras.src import testing
 
-from kimm.layers.learnable_affine import LearnableAffine
+from kimm._src.layers.learnable_affine import LearnableAffine
 
 
 class LearnableAffineTest(testing.TestCase, parameterized.TestCase):
     @pytest.mark.requires_trainable_backend
     def test_layer_scale_basic(self):
         self.run_layer_test(
             LearnableAffine,
```

### Comparing `kimm-0.1.8/kimm/layers/mobile_one_conv2d.py` & `kimm-0.2.0/kimm/_src/layers/mobile_one_conv2d.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,18 @@
 from keras import Sequential
 from keras import layers
 from keras import ops
 from keras.src.backend import standardize_data_format
 from keras.src.layers import Layer
 from keras.src.utils.argument_validation import standardize_tuple
 
+from kimm._src.kimm_export import kimm_export
 
+
+@kimm_export(parent_path=["kimm.layers"])
 @keras.saving.register_keras_serializable(package="kimm")
 class MobileOneConv2D(Layer):
     def __init__(
         self,
         filters,
         kernel_size,
         strides=(1, 1),
```

### Comparing `kimm-0.1.8/kimm/layers/mobile_one_conv2d_test.py` & `kimm-0.2.0/kimm/_src/layers/mobile_one_conv2d_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import pytest
 from absl.testing import parameterized
 from keras import backend
 from keras import random
 from keras.src import testing
 
-from kimm.layers.mobile_one_conv2d import MobileOneConv2D
+from kimm._src.layers.mobile_one_conv2d import MobileOneConv2D
 
 TEST_CASES = [
     {
         "filters": 16,
         "kernel_size": 3,
         "has_skip": True,
         "use_depthwise": False,
```

### Comparing `kimm-0.1.8/kimm/layers/position_embedding.py` & `kimm-0.2.0/kimm/_src/layers/position_embedding.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 import keras
 from keras import layers
 from keras import ops
 
+from kimm._src.kimm_export import kimm_export
 
+
+@kimm_export(parent_path=["kimm.layers"])
 @keras.saving.register_keras_serializable(package="kimm")
 class PositionEmbedding(layers.Layer):
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
 
     def build(self, input_shape):
         if len(input_shape) != 3:
```

### Comparing `kimm-0.1.8/kimm/layers/position_embedding_test.py` & `kimm-0.2.0/kimm/_src/layers/position_embedding_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import pytest
 from absl.testing import parameterized
 from keras import layers
 from keras.src import testing
 
-from kimm.layers.position_embedding import PositionEmbedding
+from kimm._src.layers.position_embedding import PositionEmbedding
 
 
 class PositionEmbeddingTest(testing.TestCase, parameterized.TestCase):
     @pytest.mark.requires_trainable_backend
     def test_position_embedding_basic(self):
         self.run_layer_test(
             PositionEmbedding,
```

### Comparing `kimm-0.1.8/kimm/layers/rep_conv2d.py` & `kimm-0.2.0/kimm/_src/layers/rep_conv2d.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,18 @@
 from keras import Sequential
 from keras import layers
 from keras import ops
 from keras.src.backend import standardize_data_format
 from keras.src.layers import Layer
 from keras.src.utils.argument_validation import standardize_tuple
 
+from kimm._src.kimm_export import kimm_export
 
+
+@kimm_export(parent_path=["kimm.layers"])
 @keras.saving.register_keras_serializable(package="kimm")
 class RepConv2D(Layer):
     def __init__(
         self,
         filters,
         kernel_size,
         strides=(1, 1),
```

### Comparing `kimm-0.1.8/kimm/layers/rep_conv2d_test.py` & `kimm-0.2.0/kimm/_src/layers/rep_conv2d_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import pytest
 from absl.testing import parameterized
 from keras import backend
 from keras import random
 from keras.src import testing
 
-from kimm.layers.rep_conv2d import RepConv2D
+from kimm._src.layers.rep_conv2d import RepConv2D
 
 TEST_CASES = [
     {
         "filters": 16,
         "kernel_size": 3,
         "has_skip": True,
         "data_format": "channels_last",
```

### Comparing `kimm-0.1.8/kimm/models/base_model.py` & `kimm-0.2.0/kimm/_src/models/base_model.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,29 +5,33 @@
 from keras import KerasTensor
 from keras import backend
 from keras import layers
 from keras import models
 from keras import utils
 from keras.src.applications import imagenet_utils
 
+from kimm._src.kimm_export import kimm_export
 
+
+@kimm_export(parent_path=["kimm.models", "kimm.models.base_model"])
 class BaseModel(models.Model):
     default_origin = (
         "https://github.com/james77777778/kimm/releases/download/0.1.0/"
     )
     available_feature_keys = []
     available_weights = []
 
     def __init__(
         self,
         inputs,
         outputs,
         features: typing.Optional[typing.Dict[str, KerasTensor]] = None,
         **kwargs,
     ):
+        _include_top = getattr(self, "_include_top", True)
         if not hasattr(self, "_feature_extractor"):
             del features
             super().__init__(inputs=inputs, outputs=outputs, **kwargs)
         else:
             if not hasattr(self, "_feature_keys"):
                 raise AttributeError(
                     "`self._feature_keys` must be set when initializing "
@@ -46,15 +50,15 @@
                     if k not in features:
                         raise KeyError(
                             f"'{k}' is not a key of `features`. Available keys "
                             f"are: {list(features.keys())}"
                         )
                     filtered_features[k] = features[k]
                 # Add outputs
-                if backend.is_keras_tensor(outputs):
+                if _include_top and backend.is_keras_tensor(outputs):
                     filtered_features["TOP"] = outputs
                 super().__init__(
                     inputs=inputs, outputs=filtered_features, **kwargs
                 )
             else:
                 del features
                 super().__init__(inputs=inputs, outputs=outputs, **kwargs)
```

### Comparing `kimm-0.1.8/kimm/models/convmixer.py` & `kimm-0.2.0/kimm/_src/models/convmixer.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import typing
 
 import keras
 from keras import backend
 from keras import layers
 
-from kimm.models.base_model import BaseModel
-from kimm.utils import add_model_to_registry
+from kimm._src.kimm_export import kimm_export
+from kimm._src.models.base_model import BaseModel
+from kimm._src.utils.model_registry import add_model_to_registry
 
 
 def apply_convmixer_block(
     inputs, output_channels, kernel_size, activation, name="convmixer_block"
 ):
     channels_axis = -1 if backend.image_data_format() == "channels_last" else -3
 
@@ -130,150 +131,118 @@
             "activation",
         ]
         for k in unused_kwargs:
             config.pop(k, None)
         return config
 
 
-"""
-Model Definition
-"""
+# Model Definition
 
 
-class ConvMixer736D32(ConvMixer):
-    available_feature_keys = ["STEM", *[f"BLOCK{i}" for i in range(32)]]
-    available_weights = [
-        (
-            "imagenet",
-            ConvMixer.default_origin,
-            "convmixer736d32_convmixer_768_32.in1k.keras",
-        )
-    ]
+class ConvMixerVariant(ConvMixer):
+    # Parameters
+    depth = None
+    hidden_channels = None
+    patch_size = None
+    kernel_size = None
+    activation = None
 
     def __init__(
         self,
         input_tensor: keras.KerasTensor = None,
         input_shape: typing.Optional[typing.Sequence[int]] = None,
         include_preprocessing: bool = True,
         include_top: bool = True,
         pooling: typing.Optional[str] = None,
         dropout_rate: float = 0.0,
         classes: int = 1000,
         classifier_activation: str = "softmax",
         weights: typing.Optional[str] = "imagenet",
-        name: str = "ConvMixer736D32",
+        name: typing.Optional[str] = None,
         **kwargs,
     ):
+        if type(self) is ConvMixerVariant:
+            raise NotImplementedError(
+                f"Cannot instantiate base class: {self.__class__.__name__}. "
+                "You should use its subclasses."
+            )
         kwargs = self.fix_config(kwargs)
         super().__init__(
-            32,
-            768,
-            7,
-            7,
-            "relu",
+            depth=self.depth,
+            hidden_channels=self.hidden_channels,
+            patch_size=self.patch_size,
+            kernel_size=self.kernel_size,
+            activation=self.activation,
             input_tensor=input_tensor,
             input_shape=input_shape,
             include_preprocessing=include_preprocessing,
             include_top=include_top,
             pooling=pooling,
             dropout_rate=dropout_rate,
             classes=classes,
             classifier_activation=classifier_activation,
             weights=weights,
-            name=name,
+            name=name or str(self.__class__.__name__),
             **kwargs,
         )
 
 
-class ConvMixer1024D20(ConvMixer):
+@kimm_export(parent_path=["kimm.models", "kimm.models.convmixer"])
+class ConvMixer736D32(ConvMixerVariant):
+    available_feature_keys = ["STEM", *[f"BLOCK{i}" for i in range(32)]]
+    available_weights = [
+        (
+            "imagenet",
+            ConvMixer.default_origin,
+            "convmixer736d32_convmixer_768_32.in1k.keras",
+        )
+    ]
+
+    # Parameters
+    depth = 32
+    hidden_channels = 768
+    patch_size = 7
+    kernel_size = 7
+    activation = "relu"
+
+
+@kimm_export(parent_path=["kimm.models", "kimm.models.convmixer"])
+class ConvMixer1024D20(ConvMixerVariant):
     available_feature_keys = ["STEM", *[f"BLOCK{i}" for i in range(20)]]
     available_weights = [
         (
             "imagenet",
             ConvMixer.default_origin,
             "convmixer1024d20_convmixer_1024_20_ks9_p14.in1k.keras",
         )
     ]
 
-    def __init__(
-        self,
-        input_tensor: keras.KerasTensor = None,
-        input_shape: typing.Optional[typing.Sequence[int]] = None,
-        include_preprocessing: bool = True,
-        include_top: bool = True,
-        pooling: typing.Optional[str] = None,
-        dropout_rate: float = 0.0,
-        classes: int = 1000,
-        classifier_activation: str = "softmax",
-        weights: typing.Optional[str] = "imagenet",
-        name: str = "ConvMixer1024D20",
-        **kwargs,
-    ):
-        kwargs = self.fix_config(kwargs)
-        super().__init__(
-            20,
-            1024,
-            14,
-            9,
-            "gelu",
-            input_tensor=input_tensor,
-            input_shape=input_shape,
-            include_preprocessing=include_preprocessing,
-            include_top=include_top,
-            pooling=pooling,
-            dropout_rate=dropout_rate,
-            classes=classes,
-            classifier_activation=classifier_activation,
-            weights=weights,
-            name=name,
-            **kwargs,
-        )
+    # Parameters
+    depth = 20
+    hidden_channels = 1024
+    patch_size = 14
+    kernel_size = 9
+    activation = "gelu"
 
 
-class ConvMixer1536D20(ConvMixer):
+@kimm_export(parent_path=["kimm.models", "kimm.models.convmixer"])
+class ConvMixer1536D20(ConvMixerVariant):
     available_feature_keys = ["STEM", *[f"BLOCK{i}" for i in range(20)]]
     available_weights = [
         (
             "imagenet",
             ConvMixer.default_origin,
             "convmixer1536d20_convmixer_1536_20.in1k.keras",
         )
     ]
 
-    def __init__(
-        self,
-        input_tensor: keras.KerasTensor = None,
-        input_shape: typing.Optional[typing.Sequence[int]] = None,
-        include_preprocessing: bool = True,
-        include_top: bool = True,
-        pooling: typing.Optional[str] = None,
-        dropout_rate: float = 0.0,
-        classes: int = 1000,
-        classifier_activation: str = "softmax",
-        weights: typing.Optional[str] = "imagenet",
-        name: str = "ConvMixer1536D20",
-        **kwargs,
-    ):
-        kwargs = self.fix_config(kwargs)
-        super().__init__(
-            20,
-            1536,
-            7,
-            9,
-            "gelu",
-            input_tensor=input_tensor,
-            input_shape=input_shape,
-            include_preprocessing=include_preprocessing,
-            include_top=include_top,
-            pooling=pooling,
-            dropout_rate=dropout_rate,
-            classes=classes,
-            classifier_activation=classifier_activation,
-            weights=weights,
-            name=name,
-            **kwargs,
-        )
+    # Parameters
+    depth = 20
+    hidden_channels = 1536
+    patch_size = 7
+    kernel_size = 9
+    activation = "gelu"
 
 
 add_model_to_registry(ConvMixer736D32, "imagenet")
 add_model_to_registry(ConvMixer1024D20, "imagenet")
 add_model_to_registry(ConvMixer1536D20, "imagenet")
```

### Comparing `kimm-0.1.8/kimm/models/densenet.py` & `kimm-0.2.0/kimm/_src/models/inception_next.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,346 +1,362 @@
+import itertools
 import typing
 
 import keras
 from keras import backend
+from keras import initializers
 from keras import layers
+from keras import ops
 
-from kimm.blocks import apply_conv2d_block
-from kimm.models import BaseModel
-from kimm.utils import add_model_to_registry
+from kimm._src.blocks.transformer import apply_mlp_block
+from kimm._src.kimm_export import kimm_export
+from kimm._src.layers.layer_scale import LayerScale
+from kimm._src.models.base_model import BaseModel
+from kimm._src.utils.model_registry import add_model_to_registry
 
 
-def apply_dense_layer(
-    inputs, growth_rate, expansion_ratio=4.0, name="dense_layer"
+def apply_inception_depthwise_conv2d(
+    inputs,
+    square_kernel_size: int = 3,
+    band_kernel_size: int = 11,
+    branch_ratio: float = 0.125,
+    name="inception_depthwise_conv2d",
 ):
     channels_axis = -1 if backend.image_data_format() == "channels_last" else -3
+    input_channels = inputs.shape[channels_axis]
+    branch_channels = int(input_channels * branch_ratio)
+    split_sizes = (
+        input_channels - 3 * branch_channels,
+        branch_channels,
+        branch_channels,
+        branch_channels,
+    )
+    split_indices = list(itertools.accumulate(split_sizes[:-1]))
+    square_padding = (square_kernel_size - 1) // 2
+    band_padding = (band_kernel_size - 1) // 2
 
     x = inputs
+
+    x_id, x_hw, x_w, x_h = ops.split(x, split_indices, axis=channels_axis)
+    x_hw = layers.ZeroPadding2D(square_padding)(x_hw)
+    x_hw = layers.DepthwiseConv2D(
+        square_kernel_size,
+        use_bias=True,
+        name=f"{name}_dwconv_hw_dwconv2d",
+    )(x_hw)
+
+    x_w = layers.ZeroPadding2D((0, band_padding))(x_w)
+    x_w = layers.DepthwiseConv2D(
+        (1, band_kernel_size),
+        use_bias=True,
+        name=f"{name}_dwconv_w_dwconv2d",
+    )(x_w)
+
+    x_h = layers.ZeroPadding2D((band_padding, 0))(x_h)
+    x_h = layers.DepthwiseConv2D(
+        (band_kernel_size, 1),
+        use_bias=True,
+        name=f"{name}_dwconv_h_dwconv2d",
+    )(x_h)
+
+    x = layers.Concatenate(axis=channels_axis)([x_id, x_hw, x_w, x_h])
+    return x
+
+
+def apply_metanext_block(
+    inputs,
+    output_channels: int,
+    mlp_ratio: float = 4.0,
+    activation="gelu",
+    name="metanext_block",
+):
+    channels_axis = -1 if backend.image_data_format() == "channels_last" else -3
+    hidden_channels = int(mlp_ratio * output_channels)
+
+    x = inputs
+
+    x = apply_inception_depthwise_conv2d(x, name=f"{name}_token_mixer")
     x = layers.BatchNormalization(
-        axis=channels_axis, momentum=0.9, epsilon=1e-5, name=f"{name}_norm1"
+        axis=channels_axis, epsilon=1e-5, name=f"{name}_norm"
     )(x)
-    x = layers.ReLU()(x)
-    x = apply_conv2d_block(
+    x = apply_mlp_block(
         x,
-        int(growth_rate * expansion_ratio),
-        1,
-        1,
-        activation="relu",
-        name=f"{name}_conv1",
+        hidden_channels,
+        output_channels,
+        activation,
+        use_bias=True,
+        use_conv_mlp=True,
+        name=f"{name}_mlp",
     )
-    x = layers.Conv2D(
-        growth_rate, 3, 1, padding="same", use_bias=False, name=f"{name}_conv2"
+    x = LayerScale(
+        axis=channels_axis,
+        initializer=initializers.Constant(1e-6),
+        name=f"{name}_layerscale",
     )(x)
+
+    x = layers.Add()([x, inputs])
     return x
 
 
-def apply_dense_block(
-    inputs, num_layers, growth_rate, expansion_ratio=4.0, name="dense_block"
+def apply_metanext_stage(
+    inputs,
+    depth: int,
+    output_channels: int,
+    strides: int,
+    mlp_ratio: float = 4,
+    activation="gelu",
+    name="convnext_stage",
 ):
     channels_axis = -1 if backend.image_data_format() == "channels_last" else -3
 
     x = inputs
-    features = [x]
-    for i in range(num_layers):
-        new_features = layers.Concatenate(axis=channels_axis)(features)
-        new_features = apply_dense_layer(
-            new_features,
-            growth_rate,
-            expansion_ratio,
-            name=f"{name}_denselayer{i + 1}",
-        )
-        features.append(new_features)
-    x = layers.Concatenate(axis=channels_axis)(features)
-    return x
 
+    # Downsample
+    if strides > 1:
+        x = layers.BatchNormalization(
+            axis=channels_axis,
+            momentum=0.9,
+            epsilon=1e-5,
+            name=f"{name}_downsample_0",
+        )(x)
+        x = layers.Conv2D(
+            output_channels,
+            2,
+            strides,
+            use_bias=True,
+            name=f"{name}_downsample_1_conv2d",
+        )(x)
 
-def apply_dense_transition_block(
-    inputs, output_channels, name="dense_transition_block"
-):
-    channels_axis = -1 if backend.image_data_format() == "channels_last" else -3
-    x = inputs
-    x = layers.BatchNormalization(
-        axis=channels_axis, momentum=0.9, epsilon=1e-5, name=f"{name}_norm"
-    )(x)
-    x = layers.ReLU()(x)
-    x = layers.Conv2D(
-        output_channels, 1, 1, "same", use_bias=False, name=f"{name}_conv"
-    )(x)
-    x = layers.AveragePooling2D(
-        2, 2, data_format=backend.image_data_format(), name=f"{name}_pool"
-    )(x)
+    # Blocks
+    for i in range(depth):
+        x = apply_metanext_block(
+            x,
+            output_channels,
+            mlp_ratio=mlp_ratio,
+            activation=activation,
+            name=f"{name}_blocks_{i}",
+        )
     return x
 
 
 @keras.saving.register_keras_serializable(package="kimm")
-class DenseNet(BaseModel):
+class InceptionNeXt(BaseModel):
     available_feature_keys = [
         "STEM_S4",
-        *[f"BLOCK{i}_S{j}" for i, j in zip(range(4), [8, 16, 32, 32])],
+        *[f"BLOCK{i}_S{j}" for i, j in zip(range(4), [4, 8, 16, 32])],
     ]
 
     def __init__(
         self,
-        growth_rate: float = 32,
-        num_blocks: typing.Sequence[int] = [6, 12, 24, 16],
+        depths: typing.Sequence[int] = [3, 3, 9, 3],
+        hidden_channels: typing.Sequence[int] = [96, 192, 384, 768],
+        mlp_ratios: typing.Sequence[float] = [4, 4, 4, 3],
+        activation: str = "gelu",
         **kwargs,
     ):
         kwargs["weights_url"] = self.get_weights_url(kwargs["weights"])
+
         input_tensor = kwargs.pop("input_tensor", None)
-        self.set_properties(kwargs)
+        self.set_properties(kwargs, 224)
         channels_axis = (
             -1 if backend.image_data_format() == "channels_last" else -3
         )
 
         inputs = self.determine_input_tensor(
             input_tensor,
             self._input_shape,
             self._default_size,
+            require_flatten=self._include_top,
         )
         x = inputs
 
         x = self.build_preprocessing(x, "imagenet")
 
         # Prepare feature extraction
         features = {}
 
-        # Stem block
-        stem_channel = growth_rate * 2
-        x = apply_conv2d_block(
-            x, stem_channel, 7, 2, activation="relu", name="features_conv0"
-        )
-        x = layers.ZeroPadding2D(1, name="features_pad0")(x)
-        x = layers.MaxPooling2D(3, 2, name="features_pool0")(x)
+        # Stem
+        x = layers.Conv2D(
+            hidden_channels[0], 4, 4, use_bias=True, name="stem_0_conv2d"
+        )(x)
+        x = layers.BatchNormalization(
+            axis=channels_axis, momentum=0.9, epsilon=1e-5, name="stem_1"
+        )(x)
         features["STEM_S4"] = x
 
-        # Blocks
+        # Blocks (4 stages)
         current_stride = 4
-        input_channels = stem_channel
-        for current_block_idx, num_layers in enumerate(num_blocks):
-            x = apply_dense_block(
+        for i in range(4):
+            strides = 2 if i > 0 else 1
+            x = apply_metanext_stage(
                 x,
-                num_layers,
-                growth_rate,
-                expansion_ratio=4.0,
-                name=f"features_denseblock{current_block_idx + 1}",
+                depths[i],
+                hidden_channels[i],
+                strides,
+                mlp_ratios[i],
+                activation=activation,
+                name=f"stages_{i}",
             )
-            input_channels = input_channels + num_layers * growth_rate
-            if current_block_idx != len(num_blocks) - 1:
-                current_stride *= 2
-                x = apply_dense_transition_block(
-                    x,
-                    input_channels // 2,
-                    name=f"features_transition{current_block_idx + 1}",
-                )
-                input_channels = input_channels // 2
-
-            features[f"BLOCK{current_block_idx}_S{current_stride}"] = x
-
-        # Final batch norm
-        x = layers.BatchNormalization(
-            axis=channels_axis,
-            momentum=0.9,
-            epsilon=1e-5,
-            name="features_norm5",
-        )(x)
-        x = layers.ReLU()(x)
+            current_stride *= strides
+            # Add feature
+            features[f"BLOCK{i}_S{current_stride}"] = x
 
         # Head
         x = self.build_head(x)
-
         super().__init__(inputs=inputs, outputs=x, features=features, **kwargs)
 
         # All references to `self` below this line
-        self.growth_rate = growth_rate
-        self.num_blocks = num_blocks
+        self.depths = depths
+        self.hidden_channels = hidden_channels
+        self.mlp_ratios = mlp_ratios
+        self.activation = activation
+
+    def build_top(self, inputs, classes, classifier_activation, dropout_rate):
+        channels_axis = (
+            -1 if backend.image_data_format() == "channels_last" else -3
+        )
+        input_channels = inputs.shape[channels_axis]
+        hidden_channels = int(input_channels * 3.0)
+
+        x = inputs
+        x = layers.GlobalAveragePooling2D(name="avg_pool")(inputs)
+        x = layers.Dense(hidden_channels, use_bias=True, name="head_fc1")(x)
+        x = layers.Activation("gelu")(x)
+        x = layers.LayerNormalization(axis=-1, epsilon=1e-6, name="head_norm")(
+            x
+        )
+        x = layers.Dropout(rate=dropout_rate, name="head_dropout")(x)
+        x = layers.Dense(
+            classes, activation=classifier_activation, name="classifier"
+        )(x)
+        return x
 
     def get_config(self):
         config = super().get_config()
         config.update(
-            {"growth_rate": self.growth_rate, "num_blocks": self.num_blocks}
+            {
+                "depths": self.depths,
+                "hidden_channels": self.hidden_channels,
+                "mlp_ratios": self.mlp_ratios,
+                "activation": self.activation,
+            }
         )
         return config
 
     def fix_config(self, config: typing.Dict):
-        unused_kwargs = ["growth_rate", "num_blocks"]
+        unused_kwargs = [
+            "depths",
+            "hidden_channels",
+            "mlp_ratios",
+            "activation",
+        ]
         for k in unused_kwargs:
             config.pop(k, None)
         return config
 
 
-"""
-Model Definition
-"""
+# Model Definition
 
 
-class DenseNet121(DenseNet):
-    available_weights = [
-        (
-            "imagenet",
-            DenseNet.default_origin,
-            "densenet121_densenet121.ra_in1k.keras",
-        )
-    ]
+class InceptionNeXtVariant(InceptionNeXt):
+    # Parameters
+    depths = None
+    hidden_channels = None
+    mlp_ratios = None
+    activation = None
 
     def __init__(
         self,
         input_tensor: keras.KerasTensor = None,
         input_shape: typing.Optional[typing.Sequence[int]] = None,
         include_preprocessing: bool = True,
         include_top: bool = True,
         pooling: typing.Optional[str] = None,
         dropout_rate: float = 0.0,
         classes: int = 1000,
         classifier_activation: str = "softmax",
         weights: typing.Optional[str] = "imagenet",
-        name: str = "DenseNet121",
+        name: typing.Optional[str] = None,
         **kwargs,
     ):
+        if type(self) is InceptionNeXtVariant:
+            raise NotImplementedError(
+                f"Cannot instantiate base class: {self.__class__.__name__}. "
+                "You should use its subclasses."
+            )
         kwargs = self.fix_config(kwargs)
+        if hasattr(self, "default_size"):
+            kwargs["default_size"] = self.default_size
         super().__init__(
-            32,
-            [6, 12, 24, 16],
+            depths=self.depths,
+            hidden_channels=self.hidden_channels,
+            mlp_ratios=self.mlp_ratios,
+            activation=self.activation,
             input_tensor=input_tensor,
             input_shape=input_shape,
             include_preprocessing=include_preprocessing,
             include_top=include_top,
             pooling=pooling,
             dropout_rate=dropout_rate,
             classes=classes,
             classifier_activation=classifier_activation,
             weights=weights,
-            name=name,
-            default_size=288,
+            name=name or str(self.__class__.__name__),
             **kwargs,
         )
 
 
-class DenseNet161(DenseNet):
+@kimm_export(parent_path=["kimm.models", "kimm.models.inception_next"])
+class InceptionNeXtTiny(InceptionNeXtVariant):
     available_weights = [
         (
             "imagenet",
-            DenseNet.default_origin,
-            "densenet161_densenet161.tv_in1k.keras",
+            InceptionNeXt.default_origin,
+            "inceptionnexttiny_inception_next_tiny.sail_in1k.keras",
         )
     ]
 
-    def __init__(
-        self,
-        input_tensor: keras.KerasTensor = None,
-        input_shape: typing.Optional[typing.Sequence[int]] = None,
-        include_preprocessing: bool = True,
-        include_top: bool = True,
-        pooling: typing.Optional[str] = None,
-        dropout_rate: float = 0.0,
-        classes: int = 1000,
-        classifier_activation: str = "softmax",
-        weights: typing.Optional[str] = "imagenet",
-        name: str = "DenseNet161",
-        **kwargs,
-    ):
-        kwargs = self.fix_config(kwargs)
-        super().__init__(
-            48,
-            [6, 12, 36, 24],
-            input_tensor=input_tensor,
-            input_shape=input_shape,
-            include_preprocessing=include_preprocessing,
-            include_top=include_top,
-            pooling=pooling,
-            dropout_rate=dropout_rate,
-            classes=classes,
-            classifier_activation=classifier_activation,
-            weights=weights,
-            name=name,
-            default_size=224,
-            **kwargs,
-        )
+    # Parameters
+    depths = (3, 3, 9, 3)
+    hidden_channels = (96, 192, 384, 768)
+    mlp_ratios = (4, 4, 4, 3)
+    activation = "gelu"
 
 
-class DenseNet169(DenseNet):
+@kimm_export(parent_path=["kimm.models", "kimm.models.inception_next"])
+class InceptionNeXtSmall(InceptionNeXtVariant):
     available_weights = [
         (
             "imagenet",
-            DenseNet.default_origin,
-            "densenet169_densenet169.tv_in1k.keras",
+            InceptionNeXt.default_origin,
+            "inceptionnextsmall_inception_next_small.sail_in1k.keras",
         )
     ]
 
-    def __init__(
-        self,
-        input_tensor: keras.KerasTensor = None,
-        input_shape: typing.Optional[typing.Sequence[int]] = None,
-        include_preprocessing: bool = True,
-        include_top: bool = True,
-        pooling: typing.Optional[str] = None,
-        dropout_rate: float = 0.0,
-        classes: int = 1000,
-        classifier_activation: str = "softmax",
-        weights: typing.Optional[str] = "imagenet",
-        name: str = "DenseNet169",
-        **kwargs,
-    ):
-        kwargs = self.fix_config(kwargs)
-        super().__init__(
-            32,
-            [6, 12, 32, 32],
-            input_tensor=input_tensor,
-            input_shape=input_shape,
-            include_preprocessing=include_preprocessing,
-            include_top=include_top,
-            pooling=pooling,
-            dropout_rate=dropout_rate,
-            classes=classes,
-            classifier_activation=classifier_activation,
-            weights=weights,
-            name=name,
-            default_size=224,
-            **kwargs,
-        )
+    # Parameters
+    depths = (3, 3, 27, 3)
+    hidden_channels = (96, 192, 384, 768)
+    mlp_ratios = (4, 4, 4, 3)
+    activation = "gelu"
 
 
-class DenseNet201(DenseNet):
+@kimm_export(parent_path=["kimm.models", "kimm.models.inception_next"])
+class InceptionNeXtBase(InceptionNeXtVariant):
     available_weights = [
         (
             "imagenet",
-            DenseNet.default_origin,
-            "densenet201_densenet201.tv_in1k.keras",
+            InceptionNeXt.default_origin,
+            "inceptionnextbase_inception_next_base.sail_in1k_384.keras",
         )
     ]
 
-    def __init__(
-        self,
-        input_tensor: keras.KerasTensor = None,
-        input_shape: typing.Optional[typing.Sequence[int]] = None,
-        include_preprocessing: bool = True,
-        include_top: bool = True,
-        pooling: typing.Optional[str] = None,
-        dropout_rate: float = 0.0,
-        classes: int = 1000,
-        classifier_activation: str = "softmax",
-        weights: typing.Optional[str] = "imagenet",
-        name: str = "DenseNet201",
-        **kwargs,
-    ):
-        kwargs = self.fix_config(kwargs)
-        super().__init__(
-            32,
-            [6, 12, 48, 32],
-            input_tensor=input_tensor,
-            input_shape=input_shape,
-            include_preprocessing=include_preprocessing,
-            include_top=include_top,
-            pooling=pooling,
-            dropout_rate=dropout_rate,
-            classes=classes,
-            classifier_activation=classifier_activation,
-            weights=weights,
-            name=name,
-            default_size=224,
-            **kwargs,
-        )
+    # Parameters
+    depths = (3, 3, 27, 3)
+    hidden_channels = (128, 256, 512, 1024)
+    mlp_ratios = (4, 4, 4, 3)
+    activation = "gelu"
+    default_size = 384
 
 
-add_model_to_registry(DenseNet121, "imagenet")
-add_model_to_registry(DenseNet161, "imagenet")
-add_model_to_registry(DenseNet169, "imagenet")
-add_model_to_registry(DenseNet201, "imagenet")
+add_model_to_registry(InceptionNeXtTiny, "imagenet")
+add_model_to_registry(InceptionNeXtSmall, "imagenet")
+add_model_to_registry(InceptionNeXtBase, "imagenet")
```

### Comparing `kimm-0.1.8/kimm/models/hgnet.py` & `kimm-0.2.0/kimm/_src/models/hgnet.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 import typing
 
 import keras
 from keras import backend
 from keras import layers
 
-from kimm import layers as kimm_layers
-from kimm.blocks import apply_conv2d_block
-from kimm.models.base_model import BaseModel
-from kimm.utils import add_model_to_registry
+from kimm._src.blocks.conv2d import apply_conv2d_block
+from kimm._src.kimm_export import kimm_export
+from kimm._src.layers.learnable_affine import LearnableAffine
+from kimm._src.models.base_model import BaseModel
+from kimm._src.utils.model_registry import add_model_to_registry
 
 DEFAULT_V1_TINY_CONFIG = dict(
     stem_type="v1",
     stem_channels=[48, 48, 96],
     use_learnable_affine=False,
     # input_channels, hidden_channels, output_channels, blocks, downsample,
     # light_block, kernel_size, num_layers
@@ -140,15 +141,15 @@
         strides,
         activation=activation,
         use_depthwise=use_depthwise,
         padding=padding,
         name=name,
     )
     if activation is not None and use_learnable_affine:
-        x = kimm_layers.LearnableAffine(name=f"{name}_lab")(x)
+        x = LearnableAffine(name=f"{name}_lab")(x)
     return x
 
 
 def apply_stem_v1(inputs, stem_channels, name="stem_v1"):
     x = inputs
     for i, c in enumerate(stem_channels):
         x = apply_conv_bn_act_block(
@@ -510,15 +511,15 @@
             1,
             "valid",
             activation="relu",
             use_bias=False,
             name="head_last_conv_0",
         )(x)
         if use_learnable_affine:
-            x = kimm_layers.LearnableAffine(name="head_last_conv_2")(x)
+            x = LearnableAffine(name="head_last_conv_2")(x)
         x = layers.Dropout(rate=dropout_rate, name="head_dropout")(x)
         x = layers.Flatten()(x)
         x = layers.Dense(
             classes, activation=classifier_activation, name="classifier"
         )(x)
         return x
 
@@ -547,417 +548,195 @@
     def fix_config(self, config):
         unused_kwargs = ["config"]
         for k in unused_kwargs:
             config.pop(k, None)
         return config
 
 
-"""
-Model Definition
-"""
+# Model Definition
 
 
-class HGNetTiny(HGNet):
-    available_weights = [
-        (
-            "imagenet",
-            HGNet.default_origin,
-            "hgnettiny_hgnet_tiny.ssld_in1k.keras",
-        )
-    ]
+class HGNetVariant(HGNet):
+    # Parameters
+    config = None
 
     def __init__(
         self,
         input_tensor: keras.KerasTensor = None,
         input_shape: typing.Optional[typing.Sequence[int]] = None,
         include_preprocessing: bool = True,
         include_top: bool = True,
         pooling: typing.Optional[str] = None,
         dropout_rate: float = 0.0,
         classes: int = 1000,
         classifier_activation: str = "softmax",
         weights: typing.Optional[str] = "imagenet",
-        name: str = "HGNetTiny",
+        name: typing.Optional[str] = None,
         **kwargs,
     ):
+        if type(self) is HGNetVariant:
+            raise NotImplementedError(
+                f"Cannot instantiate base class: {self.__class__.__name__}. "
+                "You should use its subclasses."
+            )
         kwargs = self.fix_config(kwargs)
         super().__init__(
-            config="v1_tiny",
+            config=self.config,
             input_tensor=input_tensor,
             input_shape=input_shape,
             include_preprocessing=include_preprocessing,
             include_top=include_top,
             pooling=pooling,
             dropout_rate=dropout_rate,
             classes=classes,
             classifier_activation=classifier_activation,
             weights=weights,
-            name=name,
+            name=name or str(self.__class__.__name__),
             **kwargs,
         )
 
 
-class HGNetSmall(HGNet):
+@kimm_export(parent_path=["kimm.models", "kimm.models.hgnet"])
+class HGNetTiny(HGNetVariant):
     available_weights = [
         (
             "imagenet",
             HGNet.default_origin,
-            "hgnetsmall_hgnet_small.ssld_in1k.keras",
+            "hgnettiny_hgnet_tiny.ssld_in1k.keras",
         )
     ]
 
-    def __init__(
-        self,
-        input_tensor: keras.KerasTensor = None,
-        input_shape: typing.Optional[typing.Sequence[int]] = None,
-        include_preprocessing: bool = True,
-        include_top: bool = True,
-        pooling: typing.Optional[str] = None,
-        dropout_rate: float = 0.0,
-        classes: int = 1000,
-        classifier_activation: str = "softmax",
-        weights: typing.Optional[str] = "imagenet",
-        name: str = "HGNetSmall",
-        **kwargs,
-    ):
-        kwargs = self.fix_config(kwargs)
-        super().__init__(
-            config="v1_small",
-            input_tensor=input_tensor,
-            input_shape=input_shape,
-            include_preprocessing=include_preprocessing,
-            include_top=include_top,
-            pooling=pooling,
-            dropout_rate=dropout_rate,
-            classes=classes,
-            classifier_activation=classifier_activation,
-            weights=weights,
-            name=name,
-            **kwargs,
+    # Parameters
+    config = "v1_tiny"
+
+
+@kimm_export(parent_path=["kimm.models", "kimm.models.hgnet"])
+class HGNetSmall(HGNetVariant):
+    available_weights = [
+        (
+            "imagenet",
+            HGNet.default_origin,
+            "hgnetsmall_hgnet_small.ssld_in1k.keras",
         )
+    ]
+
+    # Parameters
+    config = "v1_small"
 
 
-class HGNetBase(HGNet):
+@kimm_export(parent_path=["kimm.models", "kimm.models.hgnet"])
+class HGNetBase(HGNetVariant):
     available_weights = [
         (
             "imagenet",
             HGNet.default_origin,
             "hgnetbase_hgnet_base.ssld_in1k.keras",
         )
     ]
 
-    def __init__(
-        self,
-        input_tensor: keras.KerasTensor = None,
-        input_shape: typing.Optional[typing.Sequence[int]] = None,
-        include_preprocessing: bool = True,
-        include_top: bool = True,
-        pooling: typing.Optional[str] = None,
-        dropout_rate: float = 0.0,
-        classes: int = 1000,
-        classifier_activation: str = "softmax",
-        weights: typing.Optional[str] = "imagenet",
-        name: str = "HGNetBase",
-        **kwargs,
-    ):
-        kwargs = self.fix_config(kwargs)
-        super().__init__(
-            config="v1_base",
-            input_tensor=input_tensor,
-            input_shape=input_shape,
-            include_preprocessing=include_preprocessing,
-            include_top=include_top,
-            pooling=pooling,
-            dropout_rate=dropout_rate,
-            classes=classes,
-            classifier_activation=classifier_activation,
-            weights=weights,
-            name=name,
-            **kwargs,
-        )
+    # Parameters
+    config = "v1_base"
 
 
-class HGNetV2B0(HGNet):
+@kimm_export(parent_path=["kimm.models", "kimm.models.hgnet"])
+class HGNetV2B0(HGNetVariant):
     available_weights = [
         (
             "imagenet",
             HGNet.default_origin,
             "hgnetv2b0_hgnetv2_b0.ssld_stage2_ft_in1k.keras",
         )
     ]
 
-    def __init__(
-        self,
-        input_tensor: keras.KerasTensor = None,
-        input_shape: typing.Optional[typing.Sequence[int]] = None,
-        include_preprocessing: bool = True,
-        include_top: bool = True,
-        pooling: typing.Optional[str] = None,
-        dropout_rate: float = 0.0,
-        classes: int = 1000,
-        classifier_activation: str = "softmax",
-        weights: typing.Optional[str] = "imagenet",
-        name: str = "HGNetV2B0",
-        **kwargs,
-    ):
-        kwargs = self.fix_config(kwargs)
-        super().__init__(
-            config="v2_b0",
-            input_tensor=input_tensor,
-            input_shape=input_shape,
-            include_preprocessing=include_preprocessing,
-            include_top=include_top,
-            pooling=pooling,
-            dropout_rate=dropout_rate,
-            classes=classes,
-            classifier_activation=classifier_activation,
-            weights=weights,
-            name=name,
-            **kwargs,
-        )
+    # Parameters
+    config = "v2_b0"
 
 
-class HGNetV2B1(HGNet):
+@kimm_export(parent_path=["kimm.models", "kimm.models.hgnet"])
+class HGNetV2B1(HGNetVariant):
     available_weights = [
         (
             "imagenet",
             HGNet.default_origin,
             "hgnetv2b1_hgnetv2_b1.ssld_stage2_ft_in1k.keras",
         )
     ]
 
-    def __init__(
-        self,
-        input_tensor: keras.KerasTensor = None,
-        input_shape: typing.Optional[typing.Sequence[int]] = None,
-        include_preprocessing: bool = True,
-        include_top: bool = True,
-        pooling: typing.Optional[str] = None,
-        dropout_rate: float = 0.0,
-        classes: int = 1000,
-        classifier_activation: str = "softmax",
-        weights: typing.Optional[str] = "imagenet",
-        name: str = "HGNetV2B1",
-        **kwargs,
-    ):
-        kwargs = self.fix_config(kwargs)
-        super().__init__(
-            config="v2_b1",
-            input_tensor=input_tensor,
-            input_shape=input_shape,
-            include_preprocessing=include_preprocessing,
-            include_top=include_top,
-            pooling=pooling,
-            dropout_rate=dropout_rate,
-            classes=classes,
-            classifier_activation=classifier_activation,
-            weights=weights,
-            name=name,
-            **kwargs,
-        )
+    # Parameters
+    config = "v2_b1"
 
 
-class HGNetV2B2(HGNet):
+@kimm_export(parent_path=["kimm.models", "kimm.models.hgnet"])
+class HGNetV2B2(HGNetVariant):
     available_weights = [
         (
             "imagenet",
             HGNet.default_origin,
             "hgnetv2b2_hgnetv2_b2.ssld_stage2_ft_in1k.keras",
         )
     ]
 
-    def __init__(
-        self,
-        input_tensor: keras.KerasTensor = None,
-        input_shape: typing.Optional[typing.Sequence[int]] = None,
-        include_preprocessing: bool = True,
-        include_top: bool = True,
-        pooling: typing.Optional[str] = None,
-        dropout_rate: float = 0.0,
-        classes: int = 1000,
-        classifier_activation: str = "softmax",
-        weights: typing.Optional[str] = "imagenet",
-        name: str = "HGNetV2B2",
-        **kwargs,
-    ):
-        kwargs = self.fix_config(kwargs)
-        super().__init__(
-            config="v2_b2",
-            input_tensor=input_tensor,
-            input_shape=input_shape,
-            include_preprocessing=include_preprocessing,
-            include_top=include_top,
-            pooling=pooling,
-            dropout_rate=dropout_rate,
-            classes=classes,
-            classifier_activation=classifier_activation,
-            weights=weights,
-            name=name,
-            **kwargs,
-        )
+    # Parameters
+    config = "v2_b2"
 
 
-class HGNetV2B3(HGNet):
+@kimm_export(parent_path=["kimm.models", "kimm.models.hgnet"])
+class HGNetV2B3(HGNetVariant):
     available_weights = [
         (
             "imagenet",
             HGNet.default_origin,
             "hgnetv2b3_hgnetv2_b3.ssld_stage2_ft_in1k.keras",
         )
     ]
 
-    def __init__(
-        self,
-        input_tensor: keras.KerasTensor = None,
-        input_shape: typing.Optional[typing.Sequence[int]] = None,
-        include_preprocessing: bool = True,
-        include_top: bool = True,
-        pooling: typing.Optional[str] = None,
-        dropout_rate: float = 0.0,
-        classes: int = 1000,
-        classifier_activation: str = "softmax",
-        weights: typing.Optional[str] = "imagenet",
-        name: str = "HGNetV2B3",
-        **kwargs,
-    ):
-        kwargs = self.fix_config(kwargs)
-        super().__init__(
-            config="v2_b3",
-            input_tensor=input_tensor,
-            input_shape=input_shape,
-            include_preprocessing=include_preprocessing,
-            include_top=include_top,
-            pooling=pooling,
-            dropout_rate=dropout_rate,
-            classes=classes,
-            classifier_activation=classifier_activation,
-            weights=weights,
-            name=name,
-            **kwargs,
-        )
+    # Parameters
+    config = "v2_b3"
 
 
-class HGNetV2B4(HGNet):
+@kimm_export(parent_path=["kimm.models", "kimm.models.hgnet"])
+class HGNetV2B4(HGNetVariant):
     available_weights = [
         (
             "imagenet",
             HGNet.default_origin,
             "hgnetv2b4_hgnetv2_b4.ssld_stage2_ft_in1k.keras",
         )
     ]
 
-    def __init__(
-        self,
-        input_tensor: keras.KerasTensor = None,
-        input_shape: typing.Optional[typing.Sequence[int]] = None,
-        include_preprocessing: bool = True,
-        include_top: bool = True,
-        pooling: typing.Optional[str] = None,
-        dropout_rate: float = 0.0,
-        classes: int = 1000,
-        classifier_activation: str = "softmax",
-        weights: typing.Optional[str] = "imagenet",
-        name: str = "HGNetV2B4",
-        **kwargs,
-    ):
-        kwargs = self.fix_config(kwargs)
-        super().__init__(
-            config="v2_b4",
-            input_tensor=input_tensor,
-            input_shape=input_shape,
-            include_preprocessing=include_preprocessing,
-            include_top=include_top,
-            pooling=pooling,
-            dropout_rate=dropout_rate,
-            classes=classes,
-            classifier_activation=classifier_activation,
-            weights=weights,
-            name=name,
-            **kwargs,
-        )
+    # Parameters
+    config = "v2_b4"
 
 
-class HGNetV2B5(HGNet):
+@kimm_export(parent_path=["kimm.models", "kimm.models.hgnet"])
+class HGNetV2B5(HGNetVariant):
     available_weights = [
         (
             "imagenet",
             HGNet.default_origin,
             "hgnetv2b5_hgnetv2_b5.ssld_stage2_ft_in1k.keras",
         )
     ]
 
-    def __init__(
-        self,
-        input_tensor: keras.KerasTensor = None,
-        input_shape: typing.Optional[typing.Sequence[int]] = None,
-        include_preprocessing: bool = True,
-        include_top: bool = True,
-        pooling: typing.Optional[str] = None,
-        dropout_rate: float = 0.0,
-        classes: int = 1000,
-        classifier_activation: str = "softmax",
-        weights: typing.Optional[str] = "imagenet",
-        name: str = "HGNetV2B5",
-        **kwargs,
-    ):
-        kwargs = self.fix_config(kwargs)
-        super().__init__(
-            config="v2_b5",
-            input_tensor=input_tensor,
-            input_shape=input_shape,
-            include_preprocessing=include_preprocessing,
-            include_top=include_top,
-            pooling=pooling,
-            dropout_rate=dropout_rate,
-            classes=classes,
-            classifier_activation=classifier_activation,
-            weights=weights,
-            name=name,
-            **kwargs,
-        )
+    # Parameters
+    config = "v2_b5"
 
 
-class HGNetV2B6(HGNet):
+@kimm_export(parent_path=["kimm.models", "kimm.models.hgnet"])
+class HGNetV2B6(HGNetVariant):
     available_weights = [
         (
             "imagenet",
             HGNet.default_origin,
             "hgnetv2b6_hgnetv2_b6.ssld_stage2_ft_in1k.keras",
         )
     ]
 
-    def __init__(
-        self,
-        input_tensor: keras.KerasTensor = None,
-        input_shape: typing.Optional[typing.Sequence[int]] = None,
-        include_preprocessing: bool = True,
-        include_top: bool = True,
-        pooling: typing.Optional[str] = None,
-        dropout_rate: float = 0.0,
-        classes: int = 1000,
-        classifier_activation: str = "softmax",
-        weights: typing.Optional[str] = "imagenet",
-        name: str = "HGNetV2B6",
-        **kwargs,
-    ):
-        kwargs = self.fix_config(kwargs)
-        super().__init__(
-            config="v2_b6",
-            input_tensor=input_tensor,
-            input_shape=input_shape,
-            include_preprocessing=include_preprocessing,
-            include_top=include_top,
-            pooling=pooling,
-            dropout_rate=dropout_rate,
-            classes=classes,
-            classifier_activation=classifier_activation,
-            weights=weights,
-            name=name,
-            **kwargs,
-        )
+    # Parameters
+    config = "v2_b6"
 
 
 add_model_to_registry(HGNetTiny, "imagenet")
 add_model_to_registry(HGNetSmall, "imagenet")
 add_model_to_registry(HGNetBase, "imagenet")
 add_model_to_registry(HGNetV2B0, "imagenet")
 add_model_to_registry(HGNetV2B1, "imagenet")
```

### Comparing `kimm-0.1.8/kimm/models/inception_next.py` & `kimm-0.2.0/kimm/_src/models/ghostnet.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,393 +1,526 @@
-import itertools
 import typing
+import warnings
 
 import keras
 from keras import backend
-from keras import initializers
 from keras import layers
 from keras import ops
 
-from kimm import layers as kimm_layers
-from kimm.blocks import apply_mlp_block
-from kimm.models import BaseModel
-from kimm.utils import add_model_to_registry
+from kimm._src.blocks.conv2d import apply_conv2d_block
+from kimm._src.blocks.squeeze_and_excitation import apply_se_block
+from kimm._src.kimm_export import kimm_export
+from kimm._src.models.base_model import BaseModel
+from kimm._src.utils.make_divisble import make_divisible
+from kimm._src.utils.model_registry import add_model_to_registry
+
+DEFAULT_CONFIG = [
+    # k, t, c, SE, s
+    # stage1
+    [
+        [3, 16, 16, 0, 1],
+    ],
+    # stage2
+    [
+        [3, 48, 24, 0, 2],
+    ],
+    [
+        [3, 72, 24, 0, 1],
+    ],
+    # stage3
+    [
+        [5, 72, 40, 0.25, 2],
+    ],
+    [
+        [5, 120, 40, 0.25, 1],
+    ],
+    # stage4
+    [
+        [3, 240, 80, 0, 2],
+    ],
+    [
+        [3, 200, 80, 0, 1],
+        [3, 184, 80, 0, 1],
+        [3, 184, 80, 0, 1],
+        [3, 480, 112, 0.25, 1],
+        [3, 672, 112, 0.25, 1],
+    ],
+    # stage5
+    [
+        [5, 672, 160, 0.25, 2],
+    ],
+    [
+        [5, 960, 160, 0, 1],
+        [5, 960, 160, 0.25, 1],
+        [5, 960, 160, 0, 1],
+        [5, 960, 160, 0.25, 1],
+    ],
+]
 
 
-def apply_inception_depthwise_conv2d(
+def apply_ghost_block(
     inputs,
-    square_kernel_size: int = 3,
-    band_kernel_size: int = 11,
-    branch_ratio: float = 0.125,
-    name="inception_depthwise_conv2d",
+    output_channels: int,
+    expand_ratio: float = 2.0,
+    kernel_size: int = 1,
+    depthwise_kernel_size: int = 3,
+    strides: int = 1,
+    activation="relu",
+    name="ghost_block",
 ):
     channels_axis = -1 if backend.image_data_format() == "channels_last" else -3
-    input_channels = inputs.shape[channels_axis]
-    branch_channels = int(input_channels * branch_ratio)
-    split_sizes = (
-        input_channels - 3 * branch_channels,
-        branch_channels,
-        branch_channels,
-        branch_channels,
-    )
-    split_indices = list(itertools.accumulate(split_sizes[:-1]))
-    square_padding = (square_kernel_size - 1) // 2
-    band_padding = (band_kernel_size - 1) // 2
+    hidden_channels_1 = int(ops.ceil(output_channels / expand_ratio))
+    hidden_channels_2 = int(hidden_channels_1 * (expand_ratio - 1.0))
 
     x = inputs
-
-    x_id, x_hw, x_w, x_h = ops.split(x, split_indices, axis=channels_axis)
-    x_hw = layers.ZeroPadding2D(square_padding)(x_hw)
-    x_hw = layers.DepthwiseConv2D(
-        square_kernel_size,
-        use_bias=True,
-        name=f"{name}_dwconv_hw_dwconv2d",
-    )(x_hw)
-
-    x_w = layers.ZeroPadding2D((0, band_padding))(x_w)
-    x_w = layers.DepthwiseConv2D(
-        (1, band_kernel_size),
-        use_bias=True,
-        name=f"{name}_dwconv_w_dwconv2d",
-    )(x_w)
-
-    x_h = layers.ZeroPadding2D((band_padding, 0))(x_h)
-    x_h = layers.DepthwiseConv2D(
-        (band_kernel_size, 1),
-        use_bias=True,
-        name=f"{name}_dwconv_h_dwconv2d",
-    )(x_h)
-
-    x = layers.Concatenate(axis=channels_axis)([x_id, x_hw, x_w, x_h])
-    return x
+    x1 = apply_conv2d_block(
+        x,
+        hidden_channels_1,
+        kernel_size,
+        strides,
+        activation=activation,
+        name=f"{name}_primary_conv",
+    )
+    x2 = apply_conv2d_block(
+        x1,
+        hidden_channels_2,
+        depthwise_kernel_size,
+        1,
+        activation=activation,
+        use_depthwise=True,
+        name=f"{name}_cheap_operation",
+    )
+    out = layers.Concatenate(axis=channels_axis, name=f"{name}")([x1, x2])
+    if channels_axis == -1:
+        return out[..., :output_channels]
+    else:
+        return out[:, :output_channels, ...]
 
 
-def apply_metanext_block(
+def apply_ghost_block_v2(
     inputs,
     output_channels: int,
-    mlp_ratio: float = 4.0,
-    activation="gelu",
-    name="metanext_block",
+    expand_ratio: float = 2.0,
+    kernel_size: int = 1,
+    depthwise_kernel_size: int = 3,
+    strides: int = 1,
+    activation="relu",
+    name="ghost_block_v2",
 ):
     channels_axis = -1 if backend.image_data_format() == "channels_last" else -3
-    hidden_channels = int(mlp_ratio * output_channels)
+    if backend.image_data_format() == "channels_last":
+        output_axis = (-3, -2)
+    else:
+        output_axis = (-2, -1)
 
-    x = inputs
+    hidden_channels_1 = int(ops.ceil(output_channels / expand_ratio))
+    hidden_channels_2 = int(hidden_channels_1 * (expand_ratio - 1.0))
 
-    x = apply_inception_depthwise_conv2d(x, name=f"{name}_token_mixer")
-    x = layers.BatchNormalization(
-        axis=channels_axis, epsilon=1e-5, name=f"{name}_norm"
-    )(x)
-    x = apply_mlp_block(
+    x = inputs
+    residual = inputs
+    x1 = apply_conv2d_block(
         x,
-        hidden_channels,
-        output_channels,
-        activation,
-        use_bias=True,
-        use_conv_mlp=True,
-        name=f"{name}_mlp",
+        hidden_channels_1,
+        kernel_size,
+        strides,
+        activation=activation,
+        name=f"{name}_primary_conv",
+    )
+    x2 = apply_conv2d_block(
+        x1,
+        hidden_channels_2,
+        depthwise_kernel_size,
+        1,
+        activation=activation,
+        use_depthwise=True,
+        name=f"{name}_cheap_operation",
+    )
+    out = layers.Concatenate(axis=channels_axis, name=f"{name}_concat")(
+        [x1, x2]
     )
-    x = kimm_layers.LayerScale(
-        axis=channels_axis,
-        initializer=initializers.Constant(1e-6),
-        name=f"{name}_layerscale",
-    )(x)
 
-    x = layers.Add()([x, inputs])
-    return x
+    residual = layers.AveragePooling2D(
+        2, 2, data_format=backend.image_data_format(), name=f"{name}_avg_pool"
+    )(residual)
+    residual = apply_conv2d_block(
+        residual,
+        output_channels,
+        kernel_size,
+        strides,
+        name=f"{name}_short_conv1",
+    )
+    residual = apply_conv2d_block(
+        residual,
+        output_channels,
+        (1, 5),
+        1,
+        use_depthwise=True,
+        name=f"{name}_short_conv2",
+    )
+    residual = apply_conv2d_block(
+        residual,
+        output_channels,
+        (5, 1),
+        1,
+        use_depthwise=True,
+        name=f"{name}_short_conv3",
+    )
+    residual = layers.Activation("sigmoid", name=f"{name}_gate")(residual)
+    # TODO: support dynamic shape
+    residual = layers.Resizing(
+        out.shape[output_axis[0]], out.shape[output_axis[1]], "nearest"
+    )(residual)
+    if channels_axis == -1:
+        out = out[..., :output_channels]
+    else:
+        out = out[:, :output_channels, ...]
+    out = layers.Multiply(name=name)([out, residual])
+    return out
 
 
-def apply_metanext_stage(
+def apply_ghost_bottleneck(
     inputs,
-    depth: int,
+    hidden_channels: int,
     output_channels: int,
-    strides: int,
-    mlp_ratio: float = 4,
-    activation="gelu",
-    name="convnext_stage",
+    depthwise_kernel_size: int = 3,
+    strides: int = 1,
+    se_ratio: float = 0.0,
+    activation="relu",
+    use_attention=False,  # GhostNetV2
+    name="ghost_bottlenect",
 ):
     channels_axis = -1 if backend.image_data_format() == "channels_last" else -3
+    input_channels = inputs.shape[channels_axis]
+    has_se = se_ratio is not None and se_ratio > 0.0
 
     x = inputs
-
-    # Downsample
+    shortcut = inputs
+    # point-wise
+    if use_attention:
+        x = apply_ghost_block_v2(
+            x, hidden_channels, activation=activation, name=f"{name}_ghost1"
+        )
+    else:
+        x = apply_ghost_block(
+            x, hidden_channels, activation=activation, name=f"{name}_ghost1"
+        )
+    # depthwise
     if strides > 1:
-        x = layers.BatchNormalization(
-            axis=channels_axis,
-            momentum=0.9,
-            epsilon=1e-5,
-            name=f"{name}_downsample_0",
-        )(x)
-        x = layers.Conv2D(
-            output_channels,
-            2,
+        x = apply_conv2d_block(
+            x,
+            hidden_channels,
+            depthwise_kernel_size,
             strides,
-            use_bias=True,
-            name=f"{name}_downsample_1_conv2d",
-        )(x)
-
-    # Blocks
-    for i in range(depth):
-        x = apply_metanext_block(
+            use_depthwise=True,
+            name=f"{name}_conv_dw",
+        )
+    # squeeze-and-excitation
+    if has_se:
+        x = apply_se_block(
             x,
+            se_ratio,
+            gate_activation="hard_sigmoid",
+            make_divisible_number=4,
+            name=f"{name}_se",
+        )
+    # point-wise
+    x = apply_ghost_block(
+        x, output_channels, activation=None, name=f"{name}_ghost2"
+    )
+    # shortcut
+    if input_channels != output_channels or strides > 1:
+        shortcut = apply_conv2d_block(
+            shortcut,
+            input_channels,
+            depthwise_kernel_size,
+            strides,
+            activation=None,
+            use_depthwise=True,
+            name=f"{name}_shortcut1",
+        )
+        shortcut = apply_conv2d_block(
+            shortcut,
             output_channels,
-            mlp_ratio=mlp_ratio,
-            activation=activation,
-            name=f"{name}_blocks_{i}",
+            1,
+            1,
+            activation=None,
+            name=f"{name}_shortcut2",
         )
-    return x
+    out = layers.Add(name=name)([x, shortcut])
+    return out
 
 
 @keras.saving.register_keras_serializable(package="kimm")
-class InceptionNeXt(BaseModel):
+class GhostNet(BaseModel):
     available_feature_keys = [
-        "STEM_S4",
-        *[f"BLOCK{i}_S{j}" for i, j in zip(range(4), [4, 8, 16, 32])],
+        "STEM_S2",
+        *[
+            f"BLOCK{i}_S{j}"
+            for i, j in zip(range(9), [2, 4, 4, 8, 8, 16, 16, 32, 32])
+        ],
     ]
 
     def __init__(
         self,
-        depths: typing.Sequence[int] = [3, 3, 9, 3],
-        hidden_channels: typing.Sequence[int] = [96, 192, 384, 768],
-        mlp_ratios: typing.Sequence[float] = [4, 4, 4, 3],
-        activation: str = "gelu",
+        width: float = 1.0,
+        config: typing.Union[str, typing.List] = "default",
+        version: typing.Literal["v1", "v2"] = "v1",
         **kwargs,
     ):
         kwargs["weights_url"] = self.get_weights_url(kwargs["weights"])
 
-        input_tensor = kwargs.pop("input_tensor", None)
-        self.set_properties(kwargs, 224)
-        channels_axis = (
-            -1 if backend.image_data_format() == "channels_last" else -3
-        )
+        _available_configs = ["default"]
+        if config == "default":
+            _config = DEFAULT_CONFIG
+        else:
+            raise ValueError(
+                f"config must be one of {_available_configs} using string. "
+                f"Received: config={config}"
+            )
+        if version not in ("v1", "v2"):
+            raise ValueError(
+                "`version` must be one of ('v1', 'v2'). "
+                f"Received version={version}"
+            )
 
+        input_tensor = kwargs.pop("input_tensor", None)
+        self.set_properties(kwargs)
         inputs = self.determine_input_tensor(
             input_tensor,
             self._input_shape,
             self._default_size,
             require_flatten=self._include_top,
+            static_shape=True if version == "v2" else False,
         )
         x = inputs
 
         x = self.build_preprocessing(x, "imagenet")
 
         # Prepare feature extraction
         features = {}
 
-        # Stem
-        x = layers.Conv2D(
-            hidden_channels[0], 4, 4, use_bias=True, name="stem_0_conv2d"
-        )(x)
-        x = layers.BatchNormalization(
-            axis=channels_axis, momentum=0.9, epsilon=1e-5, name="stem_1"
-        )(x)
-        features["STEM_S4"] = x
-
-        # Blocks (4 stages)
-        current_stride = 4
-        for i in range(4):
-            strides = 2 if i > 0 else 1
-            x = apply_metanext_stage(
-                x,
-                depths[i],
-                hidden_channels[i],
-                strides,
-                mlp_ratios[i],
-                activation=activation,
-                name=f"stages_{i}",
-            )
-            current_stride *= strides
-            # Add feature
-            features[f"BLOCK{i}_S{current_stride}"] = x
+        # stem
+        stem_channels = make_divisible(16 * width, 4)
+        x = apply_conv2d_block(
+            x, stem_channels, 3, 2, activation="relu", name="conv_stem"
+        )
+        features["STEM_S2"] = x
+
+        # blocks
+        total_layer_idx = 0
+        current_stride = 2
+        for current_block_idx, cfg in enumerate(_config):
+            for current_layer_idx, (k, e, c, se, s) in enumerate(cfg):
+                output_channels = make_divisible(c * width, 4)
+                hidden_channels = make_divisible(e * width, 4)
+                use_attention = False
+                if version == "v2" and total_layer_idx > 1:
+                    use_attention = True
+                name = f"blocks_{current_block_idx}_{current_layer_idx}"
+                x = apply_ghost_bottleneck(
+                    x,
+                    hidden_channels,
+                    output_channels,
+                    k,
+                    s,
+                    se_ratio=se,
+                    use_attention=use_attention,
+                    name=name,
+                )
+                total_layer_idx += 1
+            current_stride *= s
+            features[f"BLOCK{current_block_idx}_S{current_stride}"] = x
+        # post stages conv block
+        output_channels = make_divisible(e * width, 4)
+        x = apply_conv2d_block(
+            x,
+            output_channels,
+            1,
+            activation="relu",
+            name=f"blocks_{current_block_idx+1}",
+        )
 
         # Head
         x = self.build_head(x)
+
         super().__init__(inputs=inputs, outputs=x, features=features, **kwargs)
 
         # All references to `self` below this line
-        self.depths = depths
-        self.hidden_channels = hidden_channels
-        self.mlp_ratios = mlp_ratios
-        self.activation = activation
+        self.width = width
+        self.config = config
+        self.version = version
 
     def build_top(self, inputs, classes, classifier_activation, dropout_rate):
-        channels_axis = (
-            -1 if backend.image_data_format() == "channels_last" else -3
+        x = layers.GlobalAveragePooling2D(name="avg_pool", keepdims=True)(
+            inputs
         )
-        input_channels = inputs.shape[channels_axis]
-        hidden_channels = int(input_channels * 3.0)
-
-        x = inputs
-        x = layers.GlobalAveragePooling2D(name="avg_pool")(inputs)
-        x = layers.Dense(hidden_channels, use_bias=True, name="head_fc1")(x)
-        x = layers.Activation("gelu")(x)
-        x = layers.LayerNormalization(axis=-1, epsilon=1e-6, name="head_norm")(
-            x
-        )
-        x = layers.Dropout(rate=dropout_rate, name="head_dropout")(x)
+        x = layers.Conv2D(
+            1280, 1, 1, use_bias=True, activation="relu", name="conv_head"
+        )(x)
+        x = layers.Flatten()(x)
+        x = layers.Dropout(rate=dropout_rate, name="conv_head_dropout")(x)
         x = layers.Dense(
             classes, activation=classifier_activation, name="classifier"
         )(x)
         return x
 
     def get_config(self):
         config = super().get_config()
         config.update(
             {
-                "depths": self.depths,
-                "hidden_channels": self.hidden_channels,
-                "mlp_ratios": self.mlp_ratios,
-                "activation": self.activation,
+                "width": self.width,
+                "config": self.config,
+                "version": self.version,
             }
         )
         return config
 
-    def fix_config(self, config: typing.Dict):
-        unused_kwargs = [
-            "depths",
-            "hidden_channels",
-            "mlp_ratios",
-            "activation",
-        ]
+    def fix_config(self, config):
+        unused_kwargs = ["width", "config", "version"]
         for k in unused_kwargs:
             config.pop(k, None)
         return config
 
 
-"""
-Model Definition
-"""
+# Model Definition
 
 
-class InceptionNeXtTiny(InceptionNeXt):
-    available_weights = [
-        (
-            "imagenet",
-            InceptionNeXt.default_origin,
-            "inceptionnexttiny_inception_next_tiny.sail_in1k.keras",
-        )
-    ]
+class GhostNetVariant(GhostNet):
+    # Parameters
+    width = None
+    config = None
+    version = None
 
     def __init__(
         self,
         input_tensor: keras.KerasTensor = None,
         input_shape: typing.Optional[typing.Sequence[int]] = None,
         include_preprocessing: bool = True,
         include_top: bool = True,
         pooling: typing.Optional[str] = None,
-        dropout_rate: float = 0.0,
+        dropout_rate: float = 0.2,
         classes: int = 1000,
         classifier_activation: str = "softmax",
         weights: typing.Optional[str] = "imagenet",
-        name: str = "InceptionNeXtTiny",
+        name: typing.Optional[str] = None,
         **kwargs,
     ):
+        if type(self) is GhostNetVariant:
+            raise NotImplementedError(
+                f"Cannot instantiate base class: {self.__class__.__name__}. "
+                "You should use its subclasses."
+            )
         kwargs = self.fix_config(kwargs)
+        if len(getattr(self, "available_weights", [])) == 0:
+            warnings.warn(
+                f"{self.__class__.__name__} doesn't have pretrained weights "
+                f"for '{weights}'."
+            )
+            weights = None
         super().__init__(
-            (3, 3, 9, 3),
-            (96, 192, 384, 768),
-            (4, 4, 4, 3),
-            "gelu",
+            width=self.width,
+            config=self.config,
+            version=self.version,
             input_tensor=input_tensor,
             input_shape=input_shape,
             include_preprocessing=include_preprocessing,
             include_top=include_top,
             pooling=pooling,
             dropout_rate=dropout_rate,
             classes=classes,
             classifier_activation=classifier_activation,
             weights=weights,
-            name=name,
+            name=name or str(self.__class__.__name__),
             **kwargs,
         )
 
 
-class InceptionNeXtSmall(InceptionNeXt):
+@kimm_export(parent_path=["kimm.models", "kimm.models.ghostnet"])
+class GhostNet050(GhostNetVariant):
+    available_weights = []
+
+    # Parameters
+    width = 0.5
+    config = "default"
+    version = "v1"
+
+
+@kimm_export(parent_path=["kimm.models", "kimm.models.ghostnet"])
+class GhostNet100(GhostNetVariant):
     available_weights = [
         (
             "imagenet",
-            InceptionNeXt.default_origin,
-            "inceptionnextsmall_inception_next_small.sail_in1k.keras",
+            GhostNet.default_origin,
+            "ghostnet100_ghostnet_100.keras",
         )
     ]
 
-    def __init__(
-        self,
-        input_tensor: keras.KerasTensor = None,
-        input_shape: typing.Optional[typing.Sequence[int]] = None,
-        include_preprocessing: bool = True,
-        include_top: bool = True,
-        pooling: typing.Optional[str] = None,
-        dropout_rate: float = 0.0,
-        classes: int = 1000,
-        classifier_activation: str = "softmax",
-        weights: typing.Optional[str] = "imagenet",
-        name: str = "InceptionNeXtSmall",
-        **kwargs,
-    ):
-        kwargs = self.fix_config(kwargs)
-        super().__init__(
-            (3, 3, 27, 3),
-            (96, 192, 384, 768),
-            (4, 4, 4, 3),
-            "gelu",
-            input_tensor=input_tensor,
-            input_shape=input_shape,
-            include_preprocessing=include_preprocessing,
-            include_top=include_top,
-            pooling=pooling,
-            dropout_rate=dropout_rate,
-            classes=classes,
-            classifier_activation=classifier_activation,
-            weights=weights,
-            name=name,
-            **kwargs,
+    # Parameters
+    width = 1.0
+    config = "default"
+    version = "v1"
+
+
+@kimm_export(parent_path=["kimm.models", "kimm.models.ghostnet"])
+class GhostNet130(GhostNetVariant):
+    available_weights = []
+
+    # Parameters
+    width = 1.3
+    config = "default"
+    version = "v1"
+
+
+@kimm_export(parent_path=["kimm.models", "kimm.models.ghostnet"])
+class GhostNet100V2(GhostNetVariant):
+    available_weights = [
+        (
+            "imagenet",
+            GhostNet.default_origin,
+            "ghostnet100v2_ghostnetv2_100.keras",
         )
+    ]
+
+    # Parameters
+    width = 1.0
+    config = "default"
+    version = "v2"
 
 
-class InceptionNeXtBase(InceptionNeXt):
+@kimm_export(parent_path=["kimm.models", "kimm.models.ghostnet"])
+class GhostNet130V2(GhostNetVariant):
     available_weights = [
         (
             "imagenet",
-            InceptionNeXt.default_origin,
-            "inceptionnextbase_inception_next_base.sail_in1k_384.keras",
+            GhostNet.default_origin,
+            "ghostnet130v2_ghostnetv2_130.keras",
         )
     ]
 
-    def __init__(
-        self,
-        input_tensor: keras.KerasTensor = None,
-        input_shape: typing.Optional[typing.Sequence[int]] = None,
-        include_preprocessing: bool = True,
-        include_top: bool = True,
-        pooling: typing.Optional[str] = None,
-        dropout_rate: float = 0.0,
-        classes: int = 1000,
-        classifier_activation: str = "softmax",
-        weights: typing.Optional[str] = "imagenet",
-        name: str = "InceptionNeXtBase",
-        **kwargs,
-    ):
-        kwargs = self.fix_config(kwargs)
-        super().__init__(
-            (3, 3, 27, 3),
-            (128, 256, 512, 1024),
-            (4, 4, 4, 3),
-            "gelu",
-            input_tensor=input_tensor,
-            input_shape=input_shape,
-            include_preprocessing=include_preprocessing,
-            include_top=include_top,
-            pooling=pooling,
-            dropout_rate=dropout_rate,
-            classes=classes,
-            classifier_activation=classifier_activation,
-            weights=weights,
-            name=name,
-            default_size=384,
-            **kwargs,
+    # Parameters
+    width = 1.3
+    config = "default"
+    version = "v2"
+
+
+@kimm_export(parent_path=["kimm.models", "kimm.models.ghostnet"])
+class GhostNet160V2(GhostNetVariant):
+    available_weights = [
+        (
+            "imagenet",
+            GhostNet.default_origin,
+            "ghostnet160v2_ghostnetv2_160.keras",
         )
+    ]
+
+    # Parameters
+    width = 1.6
+    config = "default"
+    version = "v2"
 
 
-add_model_to_registry(InceptionNeXtTiny, "imagenet")
-add_model_to_registry(InceptionNeXtSmall, "imagenet")
-add_model_to_registry(InceptionNeXtBase, "imagenet")
+add_model_to_registry(GhostNet050)
+add_model_to_registry(GhostNet100, "imagenet")
+add_model_to_registry(GhostNet130)
+add_model_to_registry(GhostNet100V2, "imagenet")
+add_model_to_registry(GhostNet130V2, "imagenet")
+add_model_to_registry(GhostNet160V2, "imagenet")
```

### Comparing `kimm-0.1.8/kimm/models/inception_v3.py` & `kimm-0.2.0/kimm/_src/models/inception_v3.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 import functools
 import typing
 
 import keras
 from keras import backend
 from keras import layers
 
-from kimm.blocks import apply_conv2d_block
-from kimm.models import BaseModel
-from kimm.utils import add_model_to_registry
+from kimm._src.blocks.conv2d import apply_conv2d_block
+from kimm._src.kimm_export import kimm_export
+from kimm._src.models.base_model import BaseModel
+from kimm._src.utils.model_registry import add_model_to_registry
 
 _apply_conv2d_block = functools.partial(
     apply_conv2d_block, activation="relu", bn_epsilon=1e-3, padding="valid"
 )
 
 
 def apply_inception_a_block(inputs, pool_channels, name="inception_a_block"):
@@ -305,14 +306,18 @@
         config.update({"has_aux_logits": self.has_aux_logits})
         return config
 
     def fix_config(self, config: typing.Dict):
         return config
 
 
+# Model Definition
+
+
+@kimm_export(parent_path=["kimm.models", "kimm.models.inception_v3"])
 class InceptionV3(InceptionV3Base):
     available_weights = [
         (
             "imagenet_aux_logits",
             InceptionV3Base.default_origin,
             "inceptionv3_inception_v3.gluon_in1k_aux_logits.keras",
         ),
```

### Comparing `kimm-0.1.8/kimm/models/mobilenet_v3.py` & `kimm-0.2.0/kimm/_src/models/mobilevit.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,873 +1,899 @@
 import math
 import typing
 
 import keras
+from keras import backend
 from keras import layers
+from keras import ops
 
-from kimm.blocks import apply_conv2d_block
-from kimm.blocks import apply_depthwise_separation_block
-from kimm.blocks import apply_inverted_residual_block
-from kimm.models.base_model import BaseModel
-from kimm.utils import add_model_to_registry
-from kimm.utils import make_divisible
-
-DEFAULT_SMALL_CONFIG = [
-    # type, repeat, kernel_size, strides, expansion_ratio, channels, se_ratio,
-    # activation
-    # stage0
-    [["ds", 1, 3, 2, 1.0, 16, 0.25, "relu"]],
-    # stage1
-    [
-        ["ir", 1, 3, 2, 4.5, 24, 0.0, "relu"],
-        ["ir", 1, 3, 1, 3.67, 24, 0.0, "relu"],
-    ],
-    # stage2
-    [
-        ["ir", 1, 5, 2, 4.0, 40, 0.25, "hard_swish"],
-        ["ir", 2, 5, 1, 6.0, 40, 0.25, "hard_swish"],
-    ],
-    # stage3
-    [["ir", 2, 5, 1, 3.0, 48, 0.25, "hard_swish"]],
-    # stage4
-    [["ir", 3, 5, 2, 6.0, 96, 0.25, "hard_swish"]],
-    # stage5
-    [["cn", 1, 1, 1, 1.0, 576, 0.0, "hard_swish"]],
+from kimm._src.blocks.conv2d import apply_conv2d_block
+from kimm._src.blocks.inverted_residual import apply_inverted_residual_block
+from kimm._src.blocks.transformer import apply_mlp_block
+from kimm._src.blocks.transformer import apply_transformer_block
+from kimm._src.kimm_export import kimm_export
+from kimm._src.models.base_model import BaseModel
+from kimm._src.utils.make_divisble import make_divisible
+from kimm._src.utils.model_registry import add_model_to_registry
+
+# type, repeat, kernel_size, channels, strides, expansion_ratio,
+# transformer_dim, transformer_depth, patch_size
+DEFAULT_V1_S_CONFIG = [
+    ["ir", 1, 3, 32, 1, 4.0, None, None, None],
+    ["ir", 3, 3, 64, 2, 4.0, None, None, None],
+    ["mobilevit", 1, 3, 96, 2, 4.0, 144, 2, 2],
+    ["mobilevit", 1, 3, 128, 2, 4.0, 192, 4, 2],
+    ["mobilevit", 1, 3, 160, 2, 4.0, 240, 3, 2],
 ]
-DEFAULT_LARGE_CONFIG = [
-    # type, repeat, kernel_size, strides, expansion_ratio, channels, se_ratio,
-    # activation
-    # stage0
-    [["ds", 1, 3, 1, 1.0, 16, 0.0, "relu"]],
-    # stage1
-    [
-        ["ir", 1, 3, 2, 4.0, 24, 0.0, "relu"],
-        ["ir", 1, 3, 1, 3.0, 24, 0.0, "relu"],
-    ],
-    # stage2
-    [["ir", 3, 5, 2, 3.0, 40, 0.25, "relu"]],
-    # stage3
-    [
-        ["ir", 1, 3, 2, 6.0, 80, 0.0, "hard_swish"],
-        ["ir", 1, 3, 1, 2.5, 80, 0.0, "hard_swish"],
-        ["ir", 2, 3, 1, 2.3, 80, 0.0, "hard_swish"],
-    ],
-    # stage4
-    [["ir", 2, 3, 1, 6.0, 112, 0.25, "hard_swish"]],
-    # stage5
-    [["ir", 3, 5, 2, 6.0, 160, 0.25, "hard_swish"]],
-    # stage6
-    [["cn", 1, 1, 1, 1.0, 960, 0.0, "hard_swish"]],
+DEFAULT_V1_XS_CONFIG = [
+    ["ir", 1, 3, 32, 1, 4.0, None, None, None],
+    ["ir", 3, 3, 48, 2, 4.0, None, None, None],
+    ["mobilevit", 1, 3, 64, 2, 4.0, 96, 2, 2],
+    ["mobilevit", 1, 3, 80, 2, 4.0, 120, 4, 2],
+    ["mobilevit", 1, 3, 96, 2, 4.0, 144, 3, 2],
 ]
-DEFAULT_LCNET_CONFIG = [
-    # type, repeat, kernel_size, strides, expansion_ratio, channels, se_ratio,
-    # activation
-    # stage0
-    [["dsa", 1, 3, 1, 1.0, 32, 0.0, "hard_swish"]],
-    # stage1
-    [["dsa", 2, 3, 2, 1.0, 64, 0.0, "hard_swish"]],
-    # stage2
-    [["dsa", 2, 3, 2, 1.0, 128, 0.0, "hard_swish"]],
-    # stage3
-    [
-        ["dsa", 1, 3, 2, 1.0, 256, 0.0, "hard_swish"],
-        ["dsa", 1, 5, 1, 1.0, 256, 0.0, "hard_swish"],
-    ],
-    # stage4
-    [["dsa", 4, 5, 1, 1.0, 256, 0.0, "hard_swish"]],
-    # stage5
-    [["dsa", 2, 5, 2, 1.0, 512, 0.25, "hard_swish"]],
+DEFAULT_V1_XXS_CONFIG = [
+    ["ir", 1, 3, 16, 1, 2.0, None, None, None],
+    ["ir", 3, 3, 24, 2, 2.0, None, None, None],
+    ["mobilevit", 1, 3, 48, 2, 2.0, 64, 2, 2],
+    ["mobilevit", 1, 3, 64, 2, 2.0, 80, 4, 2],
+    ["mobilevit", 1, 3, 80, 2, 2.0, 96, 3, 2],
 ]
+DEFAULT_V2_CONFIG = [
+    ["ir", 1, 3, 64, 1, 2.0, None, None, None],
+    ["ir", 2, 3, 128, 2, 2.0, None, None, None],
+    ["mobilevitv2", 1, 3, 256, 2, 2.0, 128, 2, 2],
+    ["mobilevitv2", 1, 3, 384, 2, 2.0, 192, 4, 2],
+    ["mobilevitv2", 1, 3, 512, 2, 2.0, 256, 3, 2],
+]
+
+
+def unfold(inputs, patch_size):
+    # TODO: improve performance
+    x = inputs
+    h, w, c = x.shape[-3], x.shape[-2], x.shape[-1]
+    new_h, new_w = (
+        math.ceil(h / patch_size) * patch_size,
+        math.ceil(w / patch_size) * patch_size,
+    )
+    num_patches_h = new_h // patch_size
+    num_patches_w = new_w // patch_size
+    num_patches = num_patches_h * num_patches_w
+    # [B, H, W, C] -> [B * P, N, C]
+    x = ops.reshape(
+        x, [-1, num_patches_h, patch_size, num_patches_w, patch_size, c]
+    )
+    x = ops.transpose(x, [0, 2, 4, 1, 3, 5])
+    x = ops.reshape(x, [-1, num_patches, c])
+    return x
+
+
+def fold(inputs, h, w, c, patch_size):
+    # TODO: improve performance
+    x = inputs
+    new_h, new_w = (
+        math.ceil(h / patch_size) * patch_size,
+        math.ceil(w / patch_size) * patch_size,
+    )
+    num_patches_h = new_h // patch_size
+    num_patches_w = new_w // patch_size
+    # [B * P, N, C] -> [B, P, N, C] -> [B, H, W, C]
+    x = ops.reshape(
+        x, [-1, patch_size, patch_size, num_patches_h, num_patches_w, c]
+    )
+    x = ops.transpose(x, [0, 3, 1, 4, 2, 5])
+    x = ops.reshape(
+        x, [-1, num_patches_h * patch_size, num_patches_w * patch_size, c]
+    )
+    return x
+
+
+def apply_mobilevit_block(
+    inputs,
+    output_channels: int,
+    kernel_size: int = 3,
+    strides: int = 1,
+    expansion_ratio: float = 1.0,
+    mlp_ratio: float = 2.0,
+    transformer_dim: typing.Optional[int] = None,
+    transformer_depth: int = 2,
+    patch_size: int = 8,
+    num_heads: int = 4,
+    activation="swish",
+    transformer_activation="swish",
+    fusion: bool = True,
+    name="mobilevit_block",
+):
+    channels_axis = -1 if backend.image_data_format() == "channels_last" else -3
+    input_channels = inputs.shape[channels_axis]
+    transformer_dim = transformer_dim or make_divisible(
+        input_channels * expansion_ratio
+    )
+
+    x = inputs
+
+    # Local representation
+    x = apply_conv2d_block(
+        x,
+        input_channels,
+        kernel_size,
+        strides,
+        activation=activation,
+        name=f"{name}_conv_kxk",
+    )
+    x = layers.Conv2D(
+        transformer_dim, 1, use_bias=False, name=f"{name}_conv_1x1"
+    )(x)
+
+    # TODO: natively support channels_first
+    # Unfold (feature map -> patches)
+    if backend.image_data_format() == "channels_first":
+        x = ops.transpose(x, [0, 2, 3, 1])
+
+    h, w, c = x.shape[-3], x.shape[-2], x.shape[-1]
+    x = unfold(x, patch_size)
+
+    # Global representations
+    for i in range(transformer_depth):
+        x = apply_transformer_block(
+            x,
+            transformer_dim,
+            num_heads,
+            mlp_ratio,
+            True,
+            False,
+            activation=transformer_activation,
+            name=f"{name}_transformer_{i}",
+        )
+    x = layers.LayerNormalization(axis=-1, epsilon=1e-6, name=f"{name}_norm")(x)
+
+    # Fold (patch -> feature map)
+    x = fold(x, h, w, c, patch_size)
+
+    # TODO: natively support channels_first
+    if backend.image_data_format() == "channels_first":
+        x = ops.transpose(x, [0, 3, 1, 2])
+
+    x = apply_conv2d_block(
+        x,
+        output_channels,
+        1,
+        1,
+        activation=activation,
+        name=f"{name}_conv_proj",
+    )
+    if fusion:
+        x = layers.Concatenate(axis=channels_axis)([inputs, x])
+
+    x = apply_conv2d_block(
+        x,
+        output_channels,
+        kernel_size,
+        1,
+        activation=activation,
+        name=f"{name}_conv_fusion",
+    )
+    return x
+
+
+def unfold_v2(inputs, patch_size):
+    x = inputs
+
+    if backend.image_data_format() == "channels_last":
+        h, w, c = x.shape[-3], x.shape[-2], x.shape[-1]
+    else:
+        c, h, w = x.shape[-3], x.shape[-2], x.shape[-1]
+
+    new_h, new_w = (
+        math.ceil(h / patch_size) * patch_size,
+        math.ceil(w / patch_size) * patch_size,
+    )
+    num_patches_h = new_h // patch_size
+    num_patches_w = new_w // patch_size
+    num_patches = num_patches_h * num_patches_w
+
+    if backend.image_data_format() == "channels_last":
+        # [B, H, W, C] -> [B, P, N, C]
+        x = ops.reshape(
+            x, [-1, num_patches_h, patch_size, num_patches_w, patch_size, c]
+        )
+        x = ops.transpose(x, [0, 2, 4, 1, 3, 5])
+        x = ops.reshape(x, [-1, patch_size * patch_size, num_patches, c])
+    else:
+        # [B, C, H, W] -> [B, C, P, N]
+        x = ops.reshape(
+            x, [-1, c, num_patches_h, patch_size, num_patches_w, patch_size]
+        )
+        x = ops.transpose(x, [0, 1, 3, 5, 2, 4])
+        x = ops.reshape(x, [-1, c, patch_size * patch_size, num_patches])
+    return x
+
+
+def fold_v2(inputs, h, w, c, patch_size):
+    x = inputs
+
+    new_h, new_w = (
+        math.ceil(h / patch_size) * patch_size,
+        math.ceil(w / patch_size) * patch_size,
+    )
+    num_patches_h = new_h // patch_size
+    num_patches_w = new_w // patch_size
+    if backend.image_data_format() == "channels_last":
+        # [B, P, N, C] -> [B, H, W, C]
+        x = ops.reshape(
+            x, [-1, patch_size, patch_size, num_patches_h, num_patches_w, c]
+        )
+        x = ops.transpose(x, [0, 3, 1, 4, 2, 5])
+        x = ops.reshape(
+            x, [-1, num_patches_h * patch_size, num_patches_w * patch_size, c]
+        )
+    else:
+        # [B, C, P, N] -> [B, C, H, W]
+        x = ops.reshape(
+            x, [-1, c, patch_size, patch_size, num_patches_h, num_patches_w]
+        )
+        x = ops.transpose(x, [0, 1, 4, 2, 5, 3])
+        x = ops.reshape(
+            x, [-1, c, num_patches_h * patch_size, num_patches_w * patch_size]
+        )
+    return x
+
+
+def apply_linear_self_attention_block(
+    inputs, dim: int, use_bias=True, name="linear_self_attention_block"
+):
+    channels_axis = -1 if backend.image_data_format() == "channels_last" else -3
+    num_patch_axis = (
+        -2 if backend.image_data_format() == "channels_last" else -1
+    )
+
+    x = inputs
+
+    # [B, P, N, C] -> [B, P, N, h + 2d]
+    # Project x into query, key and value
+    # Query: [B, P, N, 1]
+    # Value & Key: [B, P, N, d]
+    x = layers.Conv2D(
+        1 + (2 * dim), 1, use_bias=use_bias, name=f"{name}_qkv_proj_conv2d"
+    )(x)
+    query, key, value = ops.split(x, [1, 1 + dim], axis=channels_axis)
+
+    # Apply softmax along N dimension
+    context_scores = ops.softmax(query, axis=num_patch_axis)
+
+    # Compute context vector
+    # [B, P, N, d] x [B, P, N, 1] -> [B, P, N, d] -> [B, P, 1, d]
+    context_vector = layers.Multiply()([key, context_scores])
+    context_vector = ops.sum(context_vector, axis=num_patch_axis, keepdims=True)
+
+    # Combine context vector with values
+    # [B, P, N, d] * [B, P, 1, d] -> [B, P, N, d]
+    out = layers.ReLU()(value)
+    out = layers.Multiply()([out, context_vector])
+    out = layers.Conv2D(
+        dim, 1, use_bias=use_bias, name=f"{name}_out_proj_conv2d"
+    )(out)
+    return out
+
+
+def apply_linear_transformer_block(
+    inputs,
+    dim: int,
+    mlp_ratio: float = 2.0,
+    activation="swish",
+    name="linear_transformer_block",
+):
+    channels_axis = -1 if backend.image_data_format() == "channels_last" else -3
+    x = inputs
+
+    # Self-attention
+    x = layers.GroupNormalization(
+        1, axis=channels_axis, epsilon=1e-5, name=f"{name}_norm1"
+    )(x)
+    x = apply_linear_self_attention_block(
+        x, dim, use_bias=True, name=f"{name}_attn"
+    )
+    x = layers.Add()([inputs, x])
+
+    # Feedforward network
+    residual = x
+    x = layers.GroupNormalization(
+        1, axis=channels_axis, epsilon=1e-5, name=f"{name}_norm2"
+    )(x)
+    x = apply_mlp_block(
+        x,
+        int(dim * mlp_ratio),
+        activation=activation,
+        use_bias=True,
+        use_conv_mlp=True,
+        name=f"{name}_mlp",
+    )
+    x = layers.Add()([residual, x])
+    return x
+
+
+def apply_mobilevitv2_block(
+    inputs,
+    output_channels: int,
+    kernel_size: int = 3,
+    strides: int = 1,
+    expansion_ratio: float = 1.0,
+    mlp_ratio: float = 2.0,
+    transformer_dim: typing.Optional[int] = None,
+    transformer_depth: int = 2,
+    patch_size: int = 8,
+    activation="swish",
+    transformer_activation="swish",
+    name="mobilevitv2_block",
+):
+    channels_axis = -1 if backend.image_data_format() == "channels_last" else -3
+    input_channels = inputs.shape[channels_axis]
+    transformer_dim = transformer_dim or make_divisible(
+        input_channels * expansion_ratio
+    )
+
+    x = inputs
+
+    # Local representation
+    x = apply_conv2d_block(
+        x,
+        input_channels,
+        kernel_size,
+        strides,
+        activation=activation,
+        use_depthwise=True,
+        name=f"{name}_conv_kxk",
+    )
+    x = layers.Conv2D(
+        transformer_dim, 1, use_bias=False, name=f"{name}_conv_1x1"
+    )(x)
+
+    # Unfold (feature map -> patches)
+    if backend.image_data_format() == "channels_last":
+        h, w, c = x.shape[-3], x.shape[-2], x.shape[-1]
+    else:
+        c, h, w = x.shape[-3], x.shape[-2], x.shape[-1]
+    x = unfold_v2(x, patch_size)
+
+    # Global representations:
+    for i in range(transformer_depth):
+        x = apply_linear_transformer_block(
+            x,
+            transformer_dim,
+            mlp_ratio,
+            activation=transformer_activation,
+            name=f"{name}_transformer_{i}",
+        )
+    x = layers.GroupNormalization(
+        1, axis=channels_axis, epsilon=1e-5, name=f"{name}_norm"
+    )(x)
+
+    # Fold (patch -> feature map)
+    x = fold_v2(x, h, w, c, patch_size)
+
+    x = apply_conv2d_block(
+        x,
+        output_channels,
+        1,
+        1,
+        activation=None,
+        name=f"{name}_conv_proj",
+    )
+    return x
 
 
 @keras.saving.register_keras_serializable(package="kimm")
-class MobileNetV3(BaseModel):
+class MobileViT(BaseModel):
+    available_feature_keys = [
+        "STEM_S2",
+        *[f"BLOCK{i}_S{j}" for i, j in zip(range(5), [2, 4, 8, 16, 32])],
+    ]
+
     def __init__(
         self,
-        width: float = 1.0,
-        depth: float = 1.0,
-        fix_stem_and_head_channels: bool = False,
-        config: typing.Literal["small", "large", "lcnet"] = "large",
-        minimal: bool = False,
+        stem_channels: int = 16,
+        head_channels: int = 640,
+        activation: str = "swish",
+        config: str = "v1_s",
         **kwargs,
     ):
         kwargs["weights_url"] = self.get_weights_url(kwargs["weights"])
 
-        _available_configs = ["small", "large", "lcnet"]
-        if config == "small":
-            _config = DEFAULT_SMALL_CONFIG
-            conv_head_channels = 1024
-        elif config == "large":
-            _config = DEFAULT_LARGE_CONFIG
-            conv_head_channels = 1280
-        elif config == "lcnet":
-            _config = DEFAULT_LCNET_CONFIG
-            conv_head_channels = 1280
+        _available_configs = ["v1_s", "v1_xs", "v1_xss"]
+        if config == "v1_s":
+            _config = DEFAULT_V1_S_CONFIG
+        elif config == "v1_xs":
+            _config = DEFAULT_V1_XS_CONFIG
+        elif config == "v1_xxs":
+            _config = DEFAULT_V1_XXS_CONFIG
         else:
             raise ValueError(
                 f"config must be one of {_available_configs} using string. "
                 f"Received: config={config}"
             )
-        if minimal:
-            force_activation = "relu"
-            force_kernel_size = 3
-            no_se = True
-        else:
-            force_activation = None
-            force_kernel_size = None
-            no_se = False
-        # TF default config
-        bn_epsilon = kwargs.pop("bn_epsilon", 1e-5)
-        padding = kwargs.pop("padding", None)
 
         input_tensor = kwargs.pop("input_tensor", None)
-        self.set_properties(kwargs)
+        self.set_properties(kwargs, 256)
+
         inputs = self.determine_input_tensor(
             input_tensor,
             self._input_shape,
             self._default_size,
+            static_shape=True,
         )
         x = inputs
 
-        x = self.build_preprocessing(x, "imagenet")
+        x = self.build_preprocessing(x, "0_1")
 
         # Prepare feature extraction
         features = {}
 
         # stem
-        stem_channel = (
-            16 if fix_stem_and_head_channels else make_divisible(16 * width)
-        )
         x = apply_conv2d_block(
-            x,
-            stem_channel,
-            3,
-            2,
-            activation=force_activation or "hard_swish",
-            bn_epsilon=bn_epsilon,
-            padding=padding,
-            name="conv_stem",
+            x, stem_channels, 3, 2, activation=activation, name="stem"
         )
         features["STEM_S2"] = x
 
         # blocks
         current_stride = 2
-        for current_stage_idx, cfg in enumerate(_config):
-            for current_block_idx, sub_cfg in enumerate(cfg):
-                block_type, r, k, s, e, c, se, act = sub_cfg
-
-                # override default config
-                if force_activation is not None:
-                    act = force_activation
-                if force_kernel_size is not None:
-                    k = force_kernel_size if k > force_kernel_size else k
-                if no_se:
-                    se = 0.0
-
-                c = make_divisible(c * width)
-                # no depth multiplier at first and last block
-                if current_block_idx not in (0, len(_config) - 1):
-                    r = int(math.ceil(r * depth))
-                for current_layer_idx in range(r):
-                    s = s if current_layer_idx == 0 else 1
-                    _kwargs = {
-                        "bn_epsilon": bn_epsilon,
-                        "padding": padding,
-                        "name": (
-                            f"blocks_{current_stage_idx}_"
-                            f"{current_block_idx + current_layer_idx}"
-                        ),
-                    }
-                    if block_type in ("ds", "dsa"):
-                        x = apply_depthwise_separation_block(
-                            x,
-                            c,
-                            k,
-                            1,
-                            s,
-                            se,
-                            act,
-                            se_activation="relu",
-                            se_gate_activation="hard_sigmoid",
-                            se_make_divisible_number=8,
-                            pw_activation=act if block_type == "dsa" else None,
-                            skip=False if block_type == "dsa" else True,
-                            **_kwargs,
-                        )
-                    elif block_type == "ir":
-                        x = apply_inverted_residual_block(
-                            x,
-                            c,
-                            k,
-                            1,
-                            1,
-                            s,
-                            e,
-                            se,
-                            act,
-                            se_activation="relu",
-                            se_gate_activation="hard_sigmoid",
-                            se_make_divisible_number=8,
-                            **_kwargs,
-                        )
-                    elif block_type == "cn":
-                        x = apply_conv2d_block(
-                            x, c, k, s, activation=act, **_kwargs
-                        )
-                    current_stride *= s
-            features[f"BLOCK{current_stage_idx}_S{current_stride}"] = x
+        for current_block_idx, cfg in enumerate(_config):
+            (
+                block_type,
+                r,
+                k,
+                c,
+                s,
+                e,
+                transformer_dim,
+                transformer_depth,
+                patch_size,
+            ) = cfg
+            # always apply inverted_residual_block
+            for current_layer_idx in range(r):
+                s = s if current_layer_idx == 0 else 1
+                name = f"stages_{current_block_idx}_{current_layer_idx}"
+                x = apply_inverted_residual_block(
+                    x, c, k, 1, 1, s, e, activation=activation, name=name
+                )
+                current_stride *= s
+            if block_type == "mobilevit":
+                name = f"stages_{current_block_idx}_{current_layer_idx + 1}"
+                x = apply_mobilevit_block(
+                    x,
+                    c,
+                    k,
+                    1,
+                    transformer_dim=transformer_dim,
+                    transformer_depth=transformer_depth,
+                    patch_size=patch_size,
+                    activation=activation,
+                    transformer_activation=activation,
+                    name=name,
+                )
+            features[f"BLOCK{current_block_idx}_S{current_stride}"] = x
+
+        # last conv block
+        x = apply_conv2d_block(
+            x, head_channels, 1, 1, activation=activation, name="final_conv"
+        )
 
         # Head
-        if self._include_top:
-            if fix_stem_and_head_channels:
-                conv_head_channels = conv_head_channels
-            else:
-                conv_head_channels = max(
-                    conv_head_channels,
-                    make_divisible(conv_head_channels * width),
-                )
-            head_activation = force_activation or "hard_swish"
-            x = self.build_top(
-                x,
-                self._classes,
-                self._classifier_activation,
-                self._dropout_rate,
-                conv_head_channels=conv_head_channels,
-                head_activation=head_activation,
-            )
-        else:
-            if self._pooling == "avg":
-                x = layers.GlobalAveragePooling2D(name="avg_pool")(x)
-            elif self._pooling == "max":
-                x = layers.GlobalMaxPooling2D(name="max_pool")(x)
+        x = self.build_head(x)
 
         super().__init__(inputs=inputs, outputs=x, features=features, **kwargs)
 
         # All references to `self` below this line
-        self.width = width
-        self.depth = depth
-        self.fix_stem_and_head_channels = fix_stem_and_head_channels
+        self.stem_channels = stem_channels
+        self.head_channels = head_channels
+        self.activation = activation
         self.config = config
-        self.minimal = minimal
-
-    def build_top(
-        self,
-        inputs,
-        classes,
-        classifier_activation,
-        dropout_rate,
-        conv_head_channels,
-        head_activation,
-    ):
-        x = layers.GlobalAveragePooling2D(name="avg_pool", keepdims=True)(
-            inputs
-        )
-        x = layers.Conv2D(
-            conv_head_channels, 1, 1, use_bias=True, name="conv_head"
-        )(x)
-        x = layers.Activation(head_activation, name="act2")(x)
-        x = layers.Flatten()(x)
-        x = layers.Dropout(rate=dropout_rate, name="conv_head_dropout")(x)
-        x = layers.Dense(
-            classes, activation=classifier_activation, name="classifier"
-        )(x)
-        return x
 
     def get_config(self):
         config = super().get_config()
         config.update(
             {
-                "width": self.width,
-                "depth": self.depth,
-                "fix_stem_and_head_channels": self.fix_stem_and_head_channels,
+                "stem_channels": self.stem_channels,
+                "head_channels": self.head_channels,
+                "activation": self.activation,
                 "config": self.config,
-                "minimal": self.minimal,
             }
         )
         return config
 
     def fix_config(self, config):
         unused_kwargs = [
-            "width",
-            "depth",
-            "fix_stem_and_head_channels",
+            "stem_channels",
+            "head_channels",
+            "activation",
             "config",
-            "minimal",
         ]
         for k in unused_kwargs:
             config.pop(k, None)
         return config
 
 
-"""
-Model Definition
-"""
-
-
-class MobileNetV3W050Small(MobileNetV3):
+@keras.saving.register_keras_serializable(package="kimm")
+class MobileViTV2(BaseModel):
     available_feature_keys = [
         "STEM_S2",
-        *[f"BLOCK{i}_S{j}" for i, j in zip(range(6), [4, 8, 16, 16, 32, 32])],
-    ]
-    available_weights = [
-        (
-            "imagenet",
-            MobileNetV3.default_origin,
-            "mobilenet050v3small_mobilenetv3_small_050.lamb_in1k.keras",
-        )
+        *[f"BLOCK{i}_S{j}" for i, j in zip(range(5), [2, 4, 8, 16, 32])],
     ]
 
     def __init__(
         self,
-        input_tensor: keras.KerasTensor = None,
-        input_shape: typing.Optional[typing.Sequence[int]] = None,
-        include_preprocessing: bool = True,
-        include_top: bool = True,
-        pooling: typing.Optional[str] = None,
-        dropout_rate: float = 0.0,
-        classes: int = 1000,
-        classifier_activation: str = "softmax",
-        weights: typing.Optional[str] = "imagenet",
-        config: typing.Union[str, typing.List] = "small",
-        name: str = "MobileNetV3W050Small",
+        multiplier: float = 1.0,
+        activation: str = "swish",
+        config: str = "v2",
         **kwargs,
     ):
-        kwargs = self.fix_config(kwargs)
-        super().__init__(
-            0.5,
-            1.0,
-            True,
-            config,
-            input_tensor=input_tensor,
-            input_shape=input_shape,
-            include_preprocessing=include_preprocessing,
-            include_top=include_top,
-            pooling=pooling,
-            dropout_rate=dropout_rate,
-            classes=classes,
-            classifier_activation=classifier_activation,
-            weights=weights,
-            name=name,
-            **kwargs,
+        kwargs["weights_url"] = self.get_weights_url(kwargs["weights"])
+
+        _available_configs = ["v2"]
+        if config == "v2":
+            _config = DEFAULT_V2_CONFIG
+        else:
+            raise ValueError(
+                f"config must be one of {_available_configs} using string. "
+                f"Received: config={config}"
+            )
+
+        input_tensor = kwargs.pop("input_tensor", None)
+        self.set_properties(kwargs, 256)
+
+        inputs = self.determine_input_tensor(
+            input_tensor,
+            self._input_shape,
+            self._default_size,
+            static_shape=True,
         )
+        x = inputs
 
+        x = self.build_preprocessing(x, "0_1")
 
-class MobileNetV3W075Small(MobileNetV3):
-    available_feature_keys = [
-        "STEM_S2",
-        *[f"BLOCK{i}_S{j}" for i, j in zip(range(6), [4, 8, 16, 16, 32, 32])],
-    ]
-    available_weights = [
-        (
-            "imagenet",
-            MobileNetV3.default_origin,
-            "mobilenet075v3small_mobilenetv3_small_075.lamb_in1k.keras",
+        # Prepare feature extraction
+        features = {}
+
+        # stem
+        x = apply_conv2d_block(
+            x,
+            int(32 * multiplier),
+            3,
+            2,
+            activation=activation,
+            name="stem",
         )
-    ]
+        features["STEM_S2"] = x
+
+        # blocks
+        current_stride = 2
+        for current_block_idx, cfg in enumerate(_config):
+            (
+                block_type,
+                r,
+                k,
+                c,
+                s,
+                e,
+                _,
+                transformer_depth,
+                patch_size,
+            ) = cfg
+            c = int(c * multiplier)
+            # always apply inverted_residual_block
+            for current_layer_idx in range(r):
+                s = s if current_layer_idx == 0 else 1
+                name = f"stages_{current_block_idx}_{current_layer_idx}"
+                x = apply_inverted_residual_block(
+                    x, c, k, 1, 1, s, e, activation=activation, name=name
+                )
+                current_stride *= s
+            if block_type == "mobilevitv2":
+                name = f"stages_{current_block_idx}_{current_layer_idx + 1}"
+                x = apply_mobilevitv2_block(
+                    x,
+                    c,
+                    k,
+                    1,
+                    0.5,
+                    mlp_ratio=2.0,
+                    transformer_depth=transformer_depth,
+                    patch_size=patch_size,
+                    activation=activation,
+                    transformer_activation=activation,
+                    name=name,
+                )
+            features[f"BLOCK{current_block_idx}_S{current_stride}"] = x
+
+        # Head
+        x = self.build_head(x)
+
+        super().__init__(inputs=inputs, outputs=x, features=features, **kwargs)
+
+        # All references to `self` below this line
+        self.multiplier = multiplier
+        self.activation = activation
+        self.config = config
+
+    def get_config(self):
+        config = super().get_config()
+        config.update(
+            {
+                "multiplier": self.multiplier,
+                "activation": self.activation,
+                "config": self.config,
+            }
+        )
+        return config
+
+    def fix_config(self, config):
+        unused_kwargs = ["multiplier", "activation", "config"]
+        for k in unused_kwargs:
+            config.pop(k, None)
+        return config
+
+
+# Model Definition
+
+
+class MobileViTVariant(MobileViT):
+    # Parameters
+    stem_channels = None
+    head_channels = None
+    activation = None
+    config = None
 
     def __init__(
         self,
         input_tensor: keras.KerasTensor = None,
         input_shape: typing.Optional[typing.Sequence[int]] = None,
         include_preprocessing: bool = True,
         include_top: bool = True,
         pooling: typing.Optional[str] = None,
-        dropout_rate: float = 0.0,
+        dropout_rate: float = 0.1,
         classes: int = 1000,
         classifier_activation: str = "softmax",
         weights: typing.Optional[str] = "imagenet",
-        config: typing.Union[str, typing.List] = "small",
-        name: str = "MobileNetV3W075Small",
+        name: typing.Optional[str] = None,
         **kwargs,
     ):
+        if type(self) is MobileViTVariant:
+            raise NotImplementedError(
+                f"Cannot instantiate base class: {self.__class__.__name__}. "
+                "You should use its subclasses."
+            )
         kwargs = self.fix_config(kwargs)
         super().__init__(
-            0.75,
-            1.0,
-            False,
-            config,
+            stem_channels=self.stem_channels,
+            head_channels=self.head_channels,
+            activation=self.activation,
+            config=self.config,
             input_tensor=input_tensor,
             input_shape=input_shape,
             include_preprocessing=include_preprocessing,
             include_top=include_top,
             pooling=pooling,
             dropout_rate=dropout_rate,
             classes=classes,
             classifier_activation=classifier_activation,
             weights=weights,
-            name=name,
+            name=name or str(self.__class__.__name__),
             **kwargs,
         )
 
 
-class MobileNetV3W100Small(MobileNetV3):
-    available_feature_keys = [
-        "STEM_S2",
-        *[f"BLOCK{i}_S{j}" for i, j in zip(range(6), [4, 8, 16, 16, 32, 32])],
-    ]
+@kimm_export(parent_path=["kimm.models", "kimm.models.mobilevit"])
+class MobileViTXXS(MobileViTVariant):
     available_weights = [
         (
             "imagenet",
-            MobileNetV3.default_origin,
-            "mobilenet100v3small_mobilenetv3_small_100.lamb_in1k.keras",
+            MobileViT.default_origin,
+            "mobilevitxxs_mobilevit_xxs.cvnets_in1k.keras",
         )
     ]
 
-    def __init__(
-        self,
-        input_tensor: keras.KerasTensor = None,
-        input_shape: typing.Optional[typing.Sequence[int]] = None,
-        include_preprocessing: bool = True,
-        include_top: bool = True,
-        pooling: typing.Optional[str] = None,
-        dropout_rate: float = 0.0,
-        classes: int = 1000,
-        classifier_activation: str = "softmax",
-        weights: typing.Optional[str] = "imagenet",
-        config: typing.Union[str, typing.List] = "small",
-        name: str = "MobileNetV3W100Small",
-        **kwargs,
-    ):
-        kwargs = self.fix_config(kwargs)
-        super().__init__(
-            1.0,
-            1.0,
-            False,
-            config,
-            input_tensor=input_tensor,
-            input_shape=input_shape,
-            include_preprocessing=include_preprocessing,
-            include_top=include_top,
-            pooling=pooling,
-            dropout_rate=dropout_rate,
-            classes=classes,
-            classifier_activation=classifier_activation,
-            weights=weights,
-            name=name,
-            **kwargs,
-        )
+    # Parameters
+    stem_channels = 16
+    head_channels = 320
+    activation = "swish"
+    config = "v1_xxs"
 
 
-class MobileNetV3W100SmallMinimal(MobileNetV3):
-    available_feature_keys = [
-        "STEM_S2",
-        *[f"BLOCK{i}_S{j}" for i, j in zip(range(6), [4, 8, 16, 16, 32, 32])],
-    ]
+@kimm_export(parent_path=["kimm.models", "kimm.models.mobilevit"])
+class MobileViTXS(MobileViTVariant):
     available_weights = [
         (
             "imagenet",
-            MobileNetV3.default_origin,
-            (
-                "mobilenet100v3smallminimal_"
-                "tf_mobilenetv3_small_minimal_100.in1k.keras"
-            ),
+            MobileViT.default_origin,
+            "mobilevitxs_mobilevit_xs.cvnets_in1k.keras",
         )
     ]
 
-    def __init__(
-        self,
-        input_tensor: keras.KerasTensor = None,
-        input_shape: typing.Optional[typing.Sequence[int]] = None,
-        include_preprocessing: bool = True,
-        include_top: bool = True,
-        pooling: typing.Optional[str] = None,
-        dropout_rate: float = 0.0,
-        classes: int = 1000,
-        classifier_activation: str = "softmax",
-        weights: typing.Optional[str] = "imagenet",
-        config: typing.Union[str, typing.List] = "small",
-        name: str = "MobileNetV3W100SmallMinimal",
-        **kwargs,
-    ):
-        kwargs = self.fix_config(kwargs)
-        # default to TF configuration (bn_epsilon=1e-3 and padding="same")
-        super().__init__(
-            1.0,
-            1.0,
-            False,
-            config,
-            True,
-            input_tensor=input_tensor,
-            input_shape=input_shape,
-            include_preprocessing=include_preprocessing,
-            include_top=include_top,
-            pooling=pooling,
-            dropout_rate=dropout_rate,
-            classes=classes,
-            classifier_activation=classifier_activation,
-            weights=weights,
-            name=name,
-            bn_epsilon=1e-3,
-            padding="same",
-            **kwargs,
-        )
+    # Parameters
+    stem_channels = 16
+    head_channels = 384
+    activation = "swish"
+    config = "v1_xs"
 
 
-class MobileNetV3W100Large(MobileNetV3):
-    available_feature_keys = [
-        "STEM_S2",
-        *[
-            f"BLOCK{i}_S{j}"
-            for i, j in zip(range(7), [2, 4, 8, 16, 16, 32, 32])
-        ],
-    ]
+@kimm_export(parent_path=["kimm.models", "kimm.models.mobilevit"])
+class MobileViTS(MobileViTVariant):
     available_weights = [
         (
             "imagenet",
-            MobileNetV3.default_origin,
-            (
-                "mobilenet100v3large_"
-                "mobilenetv3_large_100.miil_in21k_ft_in1k.keras"
-            ),
+            MobileViT.default_origin,
+            "mobilevits_mobilevit_s.cvnets_in1k.keras",
         )
     ]
 
+    # Parameters
+    stem_channels = 16
+    head_channels = 640
+    activation = "swish"
+    config = "v1_s"
+
+
+class MobileViTV2Variant(MobileViTV2):
+    # Parameters
+    multiplier = None
+    activation = None
+    config = None
+
     def __init__(
         self,
         input_tensor: keras.KerasTensor = None,
         input_shape: typing.Optional[typing.Sequence[int]] = None,
         include_preprocessing: bool = True,
         include_top: bool = True,
         pooling: typing.Optional[str] = None,
-        dropout_rate: float = 0.0,
+        dropout_rate: float = 0.1,
         classes: int = 1000,
         classifier_activation: str = "softmax",
         weights: typing.Optional[str] = "imagenet",
-        config: typing.Union[str, typing.List] = "large",
-        name: str = "MobileNetV3W100Large",
+        name: typing.Optional[str] = None,
         **kwargs,
     ):
+        if type(self) is MobileViTVariant:
+            raise NotImplementedError(
+                f"Cannot instantiate base class: {self.__class__.__name__}. "
+                "You should use its subclasses."
+            )
         kwargs = self.fix_config(kwargs)
         super().__init__(
-            1.0,
-            1.0,
-            False,
-            config,
+            multiplier=self.multiplier,
+            activation=self.activation,
+            config=self.config,
             input_tensor=input_tensor,
             input_shape=input_shape,
             include_preprocessing=include_preprocessing,
             include_top=include_top,
             pooling=pooling,
             dropout_rate=dropout_rate,
             classes=classes,
             classifier_activation=classifier_activation,
             weights=weights,
-            name=name,
+            name=name or str(self.__class__.__name__),
             **kwargs,
         )
 
-    def build_preprocessing(self, inputs, mode="imagenet"):
-        if (
-            self._weights_url is not None
-            and "miil_in21k_ft_in1k" in self._weights_url
-        ):
-            """`miil_in21k_ft_in1k` needs `0_1`"""
-            return super().build_preprocessing(inputs, "0_1")
-        else:
-            return super().build_preprocessing(inputs, mode)
-
 
-class MobileNetV3W100LargeMinimal(MobileNetV3):
-    available_feature_keys = [
-        "STEM_S2",
-        *[
-            f"BLOCK{i}_S{j}"
-            for i, j in zip(range(7), [2, 4, 8, 16, 16, 32, 32])
-        ],
-    ]
+@kimm_export(parent_path=["kimm.models", "kimm.models.mobilevit"])
+class MobileViTV2W050(MobileViTV2Variant):
     available_weights = [
         (
             "imagenet",
-            MobileNetV3.default_origin,
-            (
-                "mobilenet100v3largeminimal_"
-                "tf_mobilenetv3_large_minimal_100.in1k.keras"
-            ),
+            MobileViTV2.default_origin,
+            "mobilevitv2w050_mobilevitv2_050.cvnets_in1k.keras",
         )
     ]
 
-    def __init__(
-        self,
-        input_tensor: keras.KerasTensor = None,
-        input_shape: typing.Optional[typing.Sequence[int]] = None,
-        include_preprocessing: bool = True,
-        include_top: bool = True,
-        pooling: typing.Optional[str] = None,
-        dropout_rate: float = 0.0,
-        classes: int = 1000,
-        classifier_activation: str = "softmax",
-        weights: typing.Optional[str] = "imagenet",
-        config: typing.Union[str, typing.List] = "large",
-        name: str = "MobileNetV3W100LargeMinimal",
-        **kwargs,
-    ):
-        kwargs = self.fix_config(kwargs)
-        # default to TF configuration (bn_epsilon=1e-3 and padding="same")
-        super().__init__(
-            1.0,
-            1.0,
-            False,
-            config,
-            True,
-            input_tensor=input_tensor,
-            input_shape=input_shape,
-            include_preprocessing=include_preprocessing,
-            include_top=include_top,
-            pooling=pooling,
-            dropout_rate=dropout_rate,
-            classes=classes,
-            classifier_activation=classifier_activation,
-            weights=weights,
-            name=name,
-            bn_epsilon=1e-3,
-            padding="same",
-            **kwargs,
-        )
+    # Parameters
+    multiplier = 0.5
+    activation = "swish"
+    config = "v2"
 
 
-class LCNet035(MobileNetV3):
-    available_feature_keys = [
-        "STEM_S2",
-        *[f"BLOCK{i}_S{j}" for i, j in zip(range(6), [2, 4, 8, 16, 16, 32])],
+@kimm_export(parent_path=["kimm.models", "kimm.models.mobilevit"])
+class MobileViTV2W075(MobileViTV2Variant):
+    available_weights = [
+        (
+            "imagenet",
+            MobileViTV2.default_origin,
+            "mobilevitv2w075_mobilevitv2_075.cvnets_in1k.keras",
+        )
     ]
-    available_weights = []
 
-    def __init__(
-        self,
-        input_tensor: keras.KerasTensor = None,
-        input_shape: typing.Optional[typing.Sequence[int]] = None,
-        include_preprocessing: bool = True,
-        include_top: bool = True,
-        pooling: typing.Optional[str] = None,
-        dropout_rate: float = 0.0,
-        classes: int = 1000,
-        classifier_activation: str = "softmax",
-        weights: typing.Optional[str] = None,
-        config: typing.Union[str, typing.List] = "lcnet",
-        name: str = "LCNet035",
-        **kwargs,
-    ):
-        kwargs = self.fix_config(kwargs)
-        # default to TF configuration (bn_epsilon=1e-3 and padding="same")
-        super().__init__(
-            0.35,
-            1.0,
-            False,
-            config,
-            input_tensor=input_tensor,
-            input_shape=input_shape,
-            include_preprocessing=include_preprocessing,
-            include_top=include_top,
-            pooling=pooling,
-            dropout_rate=dropout_rate,
-            classes=classes,
-            classifier_activation=classifier_activation,
-            weights=weights,
-            name=name,
-            **kwargs,
-        )
+    # Parameters
+    multiplier = 0.75
+    activation = "swish"
+    config = "v2"
 
 
-class LCNet050(MobileNetV3):
-    available_feature_keys = [
-        "STEM_S2",
-        *[f"BLOCK{i}_S{j}" for i, j in zip(range(6), [2, 4, 8, 16, 16, 32])],
-    ]
+@kimm_export(parent_path=["kimm.models", "kimm.models.mobilevit"])
+class MobileViTV2W100(MobileViTV2Variant):
     available_weights = [
         (
             "imagenet",
-            MobileNetV3.default_origin,
-            "lcnet050_lcnet_050.ra2_in1k.keras",
+            MobileViTV2.default_origin,
+            "mobilevitv2w100_mobilevitv2_100.cvnets_in1k.keras",
         )
     ]
 
-    def __init__(
-        self,
-        input_tensor: keras.KerasTensor = None,
-        input_shape: typing.Optional[typing.Sequence[int]] = None,
-        include_preprocessing: bool = True,
-        include_top: bool = True,
-        pooling: typing.Optional[str] = None,
-        dropout_rate: float = 0.0,
-        classes: int = 1000,
-        classifier_activation: str = "softmax",
-        weights: typing.Optional[str] = "imagenet",  # TODO: imagenet
-        config: typing.Union[str, typing.List] = "lcnet",
-        name: str = "LCNet050",
-        **kwargs,
-    ):
-        kwargs = self.fix_config(kwargs)
-        # default to TF configuration (bn_epsilon=1e-3 and padding="same")
-        super().__init__(
-            0.5,
-            1.0,
-            False,
-            config,
-            input_tensor=input_tensor,
-            input_shape=input_shape,
-            include_preprocessing=include_preprocessing,
-            include_top=include_top,
-            pooling=pooling,
-            dropout_rate=dropout_rate,
-            classes=classes,
-            classifier_activation=classifier_activation,
-            weights=weights,
-            name=name,
-            **kwargs,
-        )
+    # Parameters
+    multiplier = 1.0
+    activation = "swish"
+    config = "v2"
 
 
-class LCNet075(MobileNetV3):
-    available_feature_keys = [
-        "STEM_S2",
-        *[f"BLOCK{i}_S{j}" for i, j in zip(range(6), [2, 4, 8, 16, 16, 32])],
-    ]
+@kimm_export(parent_path=["kimm.models", "kimm.models.mobilevit"])
+class MobileViTV2W125(MobileViTV2Variant):
     available_weights = [
         (
             "imagenet",
-            MobileNetV3.default_origin,
-            "lcnet075_lcnet_075.ra2_in1k.keras",
+            MobileViTV2.default_origin,
+            "mobilevitv2w125_mobilevitv2_125.cvnets_in1k.keras",
         )
     ]
 
-    def __init__(
-        self,
-        input_tensor: keras.KerasTensor = None,
-        input_shape: typing.Optional[typing.Sequence[int]] = None,
-        include_preprocessing: bool = True,
-        include_top: bool = True,
-        pooling: typing.Optional[str] = None,
-        dropout_rate: float = 0.0,
-        classes: int = 1000,
-        classifier_activation: str = "softmax",
-        weights: typing.Optional[str] = "imagenet",
-        config: typing.Union[str, typing.List] = "lcnet",
-        name: str = "LCNet075",
-        **kwargs,
-    ):
-        kwargs = self.fix_config(kwargs)
-        # default to TF configuration (bn_epsilon=1e-3 and padding="same")
-        super().__init__(
-            0.75,
-            1.0,
-            False,
-            config,
-            input_tensor=input_tensor,
-            input_shape=input_shape,
-            include_preprocessing=include_preprocessing,
-            include_top=include_top,
-            pooling=pooling,
-            dropout_rate=dropout_rate,
-            classes=classes,
-            classifier_activation=classifier_activation,
-            weights=weights,
-            name=name,
-            **kwargs,
-        )
+    # Parameters
+    multiplier = 1.25
+    activation = "swish"
+    config = "v2"
 
 
-class LCNet100(MobileNetV3):
-    available_feature_keys = [
-        "STEM_S2",
-        *[f"BLOCK{i}_S{j}" for i, j in zip(range(6), [2, 4, 8, 16, 16, 32])],
-    ]
+@kimm_export(parent_path=["kimm.models", "kimm.models.mobilevit"])
+class MobileViTV2W150(MobileViTV2Variant):
     available_weights = [
         (
             "imagenet",
-            MobileNetV3.default_origin,
-            "lcnet100_lcnet_100.ra2_in1k.keras",
+            MobileViTV2.default_origin,
+            "mobilevitv2w150_mobilevitv2_150.cvnets_in22k_ft_in1k_384.keras",
         )
     ]
 
-    def __init__(
-        self,
-        input_tensor: keras.KerasTensor = None,
-        input_shape: typing.Optional[typing.Sequence[int]] = None,
-        include_preprocessing: bool = True,
-        include_top: bool = True,
-        pooling: typing.Optional[str] = None,
-        dropout_rate: float = 0.0,
-        classes: int = 1000,
-        classifier_activation: str = "softmax",
-        weights: typing.Optional[str] = "imagenet",
-        config: typing.Union[str, typing.List] = "lcnet",
-        name: str = "LCNet100",
-        **kwargs,
-    ):
-        kwargs = self.fix_config(kwargs)
-        # default to TF configuration (bn_epsilon=1e-3 and padding="same")
-        super().__init__(
-            1.0,
-            1.0,
-            False,
-            config,
-            input_tensor=input_tensor,
-            input_shape=input_shape,
-            include_preprocessing=include_preprocessing,
-            include_top=include_top,
-            pooling=pooling,
-            dropout_rate=dropout_rate,
-            classes=classes,
-            classifier_activation=classifier_activation,
-            weights=weights,
-            name=name,
-            **kwargs,
-        )
+    # Parameters
+    multiplier = 1.5
+    activation = "swish"
+    config = "v2"
 
 
-class LCNet150(MobileNetV3):
-    available_feature_keys = [
-        "STEM_S2",
-        *[
-            f"BLOCK{i}_S{j}"
-            for i, j in zip(range(7), [2, 4, 8, 16, 16, 32, 32])
-        ],
+@kimm_export(parent_path=["kimm.models", "kimm.models.mobilevit"])
+class MobileViTV2W175(MobileViTV2Variant):
+    available_weights = [
+        (
+            "imagenet",
+            MobileViTV2.default_origin,
+            "mobilevitv2w175_mobilevitv2_175.cvnets_in22k_ft_in1k_384.keras",
+        )
     ]
-    available_weights = []
 
-    def __init__(
-        self,
-        input_tensor: keras.KerasTensor = None,
-        input_shape: typing.Optional[typing.Sequence[int]] = None,
-        include_preprocessing: bool = True,
-        include_top: bool = True,
-        pooling: typing.Optional[str] = None,
-        dropout_rate: float = 0.0,
-        classes: int = 1000,
-        classifier_activation: str = "softmax",
-        weights: typing.Optional[str] = None,
-        config: typing.Union[str, typing.List] = "lcnet",
-        name: str = "LCNet150",
-        **kwargs,
-    ):
-        kwargs = self.fix_config(kwargs)
-        # default to TF configuration (bn_epsilon=1e-3 and padding="same")
-        super().__init__(
-            1.5,
-            1.0,
-            False,
-            config,
-            input_tensor=input_tensor,
-            input_shape=input_shape,
-            include_preprocessing=include_preprocessing,
-            include_top=include_top,
-            pooling=pooling,
-            dropout_rate=dropout_rate,
-            classes=classes,
-            classifier_activation=classifier_activation,
-            weights=weights,
-            name=name,
-            **kwargs,
-        )
+    # Parameters
+    multiplier = 1.75
+    activation = "swish"
+    config = "v2"
+
 
+@kimm_export(parent_path=["kimm.models", "kimm.models.mobilevit"])
+class MobileViTV2W200(MobileViTV2Variant):
+    available_weights = [
+        (
+            "imagenet",
+            MobileViTV2.default_origin,
+            "mobilevitv2w200_mobilevitv2_200.cvnets_in22k_ft_in1k_384.keras",
+        )
+    ]
 
-add_model_to_registry(MobileNetV3W050Small, "imagenet")
-add_model_to_registry(MobileNetV3W075Small, "imagenet")
-add_model_to_registry(MobileNetV3W100Small, "imagenet")
-add_model_to_registry(MobileNetV3W100SmallMinimal, "imagenet")
-add_model_to_registry(MobileNetV3W100Large, "imagenet")
-add_model_to_registry(MobileNetV3W100LargeMinimal, "imagenet")
-add_model_to_registry(LCNet035)
-add_model_to_registry(LCNet050, "imagenet")
-add_model_to_registry(LCNet075, "imagenet")
-add_model_to_registry(LCNet100, "imagenet")
-add_model_to_registry(LCNet150)
+    # Parameters
+    multiplier = 2.0
+    activation = "swish"
+    config = "v2"
+
+
+add_model_to_registry(MobileViTXXS, "imagenet")
+add_model_to_registry(MobileViTXS, "imagenet")
+add_model_to_registry(MobileViTS, "imagenet")
+add_model_to_registry(MobileViTV2W050, "imagenet")
+add_model_to_registry(MobileViTV2W075, "imagenet")
+add_model_to_registry(MobileViTV2W100, "imagenet")
+add_model_to_registry(MobileViTV2W125, "imagenet")
+add_model_to_registry(MobileViTV2W150, "imagenet")
+add_model_to_registry(MobileViTV2W175, "imagenet")
+add_model_to_registry(MobileViTV2W200, "imagenet")
```

### Comparing `kimm-0.1.8/kimm/models/mobileone.py` & `kimm-0.2.0/kimm/_src/models/mobileone.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import typing
 
 import keras
 from keras import backend
 
-from kimm import layers as kimm_layers
-from kimm.models.base_model import BaseModel
-from kimm.utils import add_model_to_registry
+from kimm._src.kimm_export import kimm_export
+from kimm._src.layers.mobile_one_conv2d import MobileOneConv2D
+from kimm._src.models.base_model import BaseModel
+from kimm._src.utils.model_registry import add_model_to_registry
 
 
 @keras.saving.register_keras_serializable(package="kimm")
 class MobileOne(BaseModel):
     available_feature_keys = [
         "STEM_S2",
         *[f"BLOCK{i}_S{j}" for i, j in zip(range(4), [4, 8, 16, 32])],
@@ -50,15 +51,15 @@
 
         x = self.build_preprocessing(x, "imagenet")
 
         # Prepare feature extraction
         features = {}
 
         # stem
-        x = kimm_layers.MobileOneConv2D(
+        x = MobileOneConv2D(
             stem_channels,
             3,
             2,
             has_skip=False,
             reparameterized=reparameterized,
             activation="relu",
             name="stem",
@@ -78,27 +79,27 @@
                 strides = strides if current_block_idx == 0 else 1
                 input_channels = x.shape[channels_axis]
                 has_skip1 = strides == 1
                 has_skip2 = input_channels == c
                 name1 = f"stages_{current_stage_idx}_{current_block_idx}"
                 name2 = f"stages_{current_stage_idx}_{current_block_idx+1}"
                 # Depthwise
-                x = kimm_layers.MobileOneConv2D(
+                x = MobileOneConv2D(
                     input_channels,
                     3,
                     strides,
                     has_skip=has_skip1,
                     use_depthwise=True,
                     branch_size=branch_size,
                     reparameterized=reparameterized,
                     activation="relu",
                     name=name1,
                 )(x)
                 # Pointwise
-                x = kimm_layers.MobileOneConv2D(
+                x = MobileOneConv2D(
                     c,
                     1,
                     1,
                     has_skip=has_skip2,
                     use_depthwise=False,
                     branch_size=branch_size,
                     reparameterized=reparameterized,
@@ -160,197 +161,131 @@
                 for weight, target_weight in zip(
                     layer.weights, reparameterized_layer.weights
                 ):
                     target_weight.assign(weight)
         return model
 
 
-"""
-Model Definition
-"""
+# Model Definition
 
 
-class MobileOneS0(MobileOne):
-    available_weights = [
-        (
-            "imagenet",
-            MobileOne.default_origin,
-            "mobileones0_mobileone_s0.apple_in1k.keras",
-        )
-    ]
+class MobileOneVariant(MobileOne):
+    # Parameters
+    num_blocks = None
+    num_channels = None
+    stem_channels = None
+    branch_size = None
 
     def __init__(
         self,
         reparameterized: bool = False,
         input_tensor: keras.KerasTensor = None,
         input_shape: typing.Optional[typing.Sequence[int]] = None,
         include_preprocessing: bool = True,
         include_top: bool = True,
         pooling: typing.Optional[str] = None,
         dropout_rate: float = 0.0,
         classes: int = 1000,
         classifier_activation: str = "softmax",
         weights: typing.Optional[str] = "imagenet",
-        name: str = "MobileOneS0",
+        name: typing.Optional[str] = None,
         **kwargs,
     ):
+        if type(self) is MobileOneVariant:
+            raise NotImplementedError(
+                f"Cannot instantiate base class: {self.__class__.__name__}. "
+                "You should use its subclasses."
+            )
         kwargs = self.fix_config(kwargs)
         super().__init__(
-            [2, 8, 10, 1],
-            [48, 128, 256, 1024],
-            48,
-            4,
+            num_blocks=self.num_blocks,
+            num_channels=self.num_channels,
+            stem_channels=self.stem_channels,
+            branch_size=self.branch_size,
             reparameterized=reparameterized,
             input_tensor=input_tensor,
             input_shape=input_shape,
             include_preprocessing=include_preprocessing,
             include_top=include_top,
             pooling=pooling,
             dropout_rate=dropout_rate,
             classes=classes,
             classifier_activation=classifier_activation,
             weights=weights,
-            name=name,
+            name=name or str(self.__class__.__name__),
             **kwargs,
         )
 
 
-class MobileOneS1(MobileOne):
+@kimm_export(parent_path=["kimm.models", "kimm.models.mobileone"])
+class MobileOneS0(MobileOneVariant):
     available_weights = [
         (
             "imagenet",
             MobileOne.default_origin,
-            "mobileones1_mobileone_s1.apple_in1k.keras",
+            "mobileones0_mobileone_s0.apple_in1k.keras",
         )
     ]
 
-    def __init__(
-        self,
-        reparameterized: bool = False,
-        input_tensor: keras.KerasTensor = None,
-        input_shape: typing.Optional[typing.Sequence[int]] = None,
-        include_preprocessing: bool = True,
-        include_top: bool = True,
-        pooling: typing.Optional[str] = None,
-        dropout_rate: float = 0.0,
-        classes: int = 1000,
-        classifier_activation: str = "softmax",
-        weights: typing.Optional[str] = "imagenet",
-        name: str = "MobileOneS1",
-        **kwargs,
-    ):
-        kwargs = self.fix_config(kwargs)
-        super().__init__(
-            [2, 8, 10, 1],
-            [96, 192, 512, 1280],
-            64,
-            1,
-            reparameterized=reparameterized,
-            input_tensor=input_tensor,
-            input_shape=input_shape,
-            include_preprocessing=include_preprocessing,
-            include_top=include_top,
-            pooling=pooling,
-            dropout_rate=dropout_rate,
-            classes=classes,
-            classifier_activation=classifier_activation,
-            weights=weights,
-            name=name,
-            **kwargs,
+    # Parameters
+    num_blocks = [2, 8, 10, 1]
+    num_channels = [48, 128, 256, 1024]
+    stem_channels = 48
+    branch_size = 4
+
+
+@kimm_export(parent_path=["kimm.models", "kimm.models.mobileone"])
+class MobileOneS1(MobileOneVariant):
+    available_weights = [
+        (
+            "imagenet",
+            MobileOne.default_origin,
+            "mobileones1_mobileone_s1.apple_in1k.keras",
         )
+    ]
 
+    # Parameters
+    num_blocks = [2, 8, 10, 1]
+    num_channels = [96, 192, 512, 1280]
+    stem_channels = 64
+    branch_size = 1
 
-class MobileOneS2(MobileOne):
+
+@kimm_export(parent_path=["kimm.models", "kimm.models.mobileone"])
+class MobileOneS2(MobileOneVariant):
     available_weights = [
         (
             "imagenet",
             MobileOne.default_origin,
             "mobileones2_mobileone_s2.apple_in1k.keras",
         )
     ]
 
-    def __init__(
-        self,
-        reparameterized: bool = False,
-        input_tensor: keras.KerasTensor = None,
-        input_shape: typing.Optional[typing.Sequence[int]] = None,
-        include_preprocessing: bool = True,
-        include_top: bool = True,
-        pooling: typing.Optional[str] = None,
-        dropout_rate: float = 0.0,
-        classes: int = 1000,
-        classifier_activation: str = "softmax",
-        weights: typing.Optional[str] = "imagenet",
-        name: str = "MobileOneS2",
-        **kwargs,
-    ):
-        kwargs = self.fix_config(kwargs)
-        super().__init__(
-            [2, 8, 10, 1],
-            [96, 256, 640, 2048],
-            64,
-            1,
-            reparameterized=reparameterized,
-            input_tensor=input_tensor,
-            input_shape=input_shape,
-            include_preprocessing=include_preprocessing,
-            include_top=include_top,
-            pooling=pooling,
-            dropout_rate=dropout_rate,
-            classes=classes,
-            classifier_activation=classifier_activation,
-            weights=weights,
-            name=name,
-            **kwargs,
-        )
+    # Parameters
+    num_blocks = [2, 8, 10, 1]
+    num_channels = [96, 256, 640, 2048]
+    stem_channels = 64
+    branch_size = 1
 
 
-class MobileOneS3(MobileOne):
+@kimm_export(parent_path=["kimm.models", "kimm.models.mobileone"])
+class MobileOneS3(MobileOneVariant):
     available_weights = [
         (
             "imagenet",
             MobileOne.default_origin,
             "mobileones3_mobileone_s3.apple_in1k.keras",
         )
     ]
 
-    def __init__(
-        self,
-        reparameterized: bool = False,
-        input_tensor: keras.KerasTensor = None,
-        input_shape: typing.Optional[typing.Sequence[int]] = None,
-        include_preprocessing: bool = True,
-        include_top: bool = True,
-        pooling: typing.Optional[str] = None,
-        dropout_rate: float = 0.0,
-        classes: int = 1000,
-        classifier_activation: str = "softmax",
-        weights: typing.Optional[str] = "imagenet",
-        name: str = "MobileOneS3",
-        **kwargs,
-    ):
-        kwargs = self.fix_config(kwargs)
-        super().__init__(
-            [2, 8, 10, 1],
-            [128, 320, 768, 2048],
-            64,
-            1,
-            reparameterized=reparameterized,
-            input_tensor=input_tensor,
-            input_shape=input_shape,
-            include_preprocessing=include_preprocessing,
-            include_top=include_top,
-            pooling=pooling,
-            dropout_rate=dropout_rate,
-            classes=classes,
-            classifier_activation=classifier_activation,
-            weights=weights,
-            name=name,
-            **kwargs,
-        )
+    # Parameters
+    num_blocks = [2, 8, 10, 1]
+    num_channels = [128, 320, 768, 2048]
+    stem_channels = 64
+    branch_size = 1
 
 
 # TODO: Add MobileOneS4 (w/ SE blocks)
 
 
 add_model_to_registry(MobileOneS0, "imagenet")
 add_model_to_registry(MobileOneS1, "imagenet")
```

### Comparing `kimm-0.1.8/kimm/models/models_test.py` & `kimm-0.2.0/kimm/_src/models/models_test.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,505 +1,579 @@
 import keras
 import pytest
 import tensorflow as tf
 from absl.testing import parameterized
-from keras import backend
-from keras import models
-from keras import ops
-from keras import random
-from keras import utils
-from keras.applications.imagenet_utils import decode_predictions
 from keras.src import testing
 
-from kimm import models as kimm_models
-from kimm.utils import make_divisible
+from kimm._src import models as kimm_models
+from kimm._src.utils.make_divisble import make_divisible
+
+decode_predictions = keras.applications.imagenet_utils.decode_predictions
+
+# Test BaseModel
+
+
+class SampleModel(kimm_models.BaseModel):
+    available_feature_keys = [f"S{2**i}" for i in range(1, 6)]
+
+    def __init__(self, **kwargs):
+        self.set_properties(kwargs)
+        inputs = keras.layers.Input(shape=[224, 224, 3])
+
+        features = {}
+        s2 = keras.layers.Conv2D(3, 1, 2, use_bias=False)(inputs)
+        features["S2"] = s2
+        s4 = keras.layers.Conv2D(3, 1, 2, use_bias=False)(s2)
+        features["S4"] = s4
+        s8 = keras.layers.Conv2D(3, 1, 2, use_bias=False)(s4)
+        features["S8"] = s8
+        s16 = keras.layers.Conv2D(3, 1, 2, use_bias=False)(s8)
+        features["S16"] = s16
+        s32 = keras.layers.Conv2D(3, 1, 2, use_bias=False)(s16)
+        features["S32"] = s32
+        outputs = keras.layers.GlobalAveragePooling2D()(s32)
+        super().__init__(
+            inputs=inputs, outputs=outputs, features=features, **kwargs
+        )
+
+
+class BaseModelTest(testing.TestCase, parameterized.TestCase):
+    def test_feature_extractor(self):
+        x = keras.random.uniform([1, 224, 224, 3])
+
+        # Test availiable_feature_keys
+        self.assertContainsSubset(
+            ["S2", "S4", "S8", "S16", "S32"],
+            SampleModel.available_feature_keys,
+        )
+
+        # Test feature_extractor=False
+        model = SampleModel()
+        y = model(x, training=False)
+        self.assertNotIsInstance(y, dict)
+        self.assertEqual(list(y.shape), [1, 3])
+
+        # Test feature_extractor=True
+        model = SampleModel(feature_extractor=True)
+        y = model(x, training=False)
+        self.assertIsInstance(y, dict)
+        self.assertEqual(list(y["S2"].shape), [1, 112, 112, 3])
+        self.assertEqual(list(y["S32"].shape), [1, 7, 7, 3])
+
+        # Test feature_extractor=True with feature_keys
+        model = SampleModel(
+            include_top=False,
+            feature_extractor=True,
+            feature_keys=["S2", "S16", "S32"],
+        )
+        y = model(x, training=False)
+        self.assertIsInstance(y, dict)
+        self.assertNotIn("S4", y)
+        self.assertNotIn("S8", y)
+        self.assertEqual(list(y["S2"].shape), [1, 112, 112, 3])
+        self.assertEqual(list(y["S16"].shape), [1, 14, 14, 3])
+        self.assertEqual(list(y["S32"].shape), [1, 7, 7, 3])
+        self.assertNotIn("TOP", y)
+
+
+# Test some small models
 
 # name, class, default_size, features (name, shape),
 # weights (defaults to imagenet)
 MODEL_CONFIGS = [
     # convmixer
     (
-        kimm_models.ConvMixer736D32.__name__,
-        kimm_models.ConvMixer736D32,
+        kimm_models.convmixer.ConvMixer736D32.__name__,
+        kimm_models.convmixer.ConvMixer736D32,
         224,
         [
             ("STEM", [1, 32, 32, 768]),
             *((f"BLOCK{i}", [1, 32, 32, 768]) for i in range(32)),
         ],
     ),
     # convnext
     (
-        kimm_models.ConvNeXtAtto.__name__,
-        kimm_models.ConvNeXtAtto,
+        kimm_models.convnext.ConvNeXtAtto.__name__,
+        kimm_models.convnext.ConvNeXtAtto,
         288,
         [
             ("STEM_S4", [1, 72, 72, 40]),
             ("BLOCK0_S4", [1, 72, 72, 40]),
             ("BLOCK1_S8", [1, 36, 36, 80]),
             ("BLOCK2_S16", [1, 18, 18, 160]),
             ("BLOCK3_S32", [1, 9, 9, 320]),
         ],
     ),
     # densenet
     (
-        kimm_models.DenseNet121.__name__,
-        kimm_models.DenseNet121,
+        kimm_models.densenet.DenseNet121.__name__,
+        kimm_models.densenet.DenseNet121,
         224,
         [
             ("STEM_S4", [1, 56, 56, 64]),
             ("BLOCK0_S8", [1, 28, 28, 128]),
             ("BLOCK1_S16", [1, 14, 14, 256]),
             ("BLOCK2_S32", [1, 7, 7, 512]),
             ("BLOCK3_S32", [1, 7, 7, 1024]),
         ],
     ),
     # efficientnet
     (
-        kimm_models.EfficientNetB2.__name__,
-        kimm_models.EfficientNetB2,
+        kimm_models.efficientnet.EfficientNetB2.__name__,
+        kimm_models.efficientnet.EfficientNetB2,
         260,
         [
             ("STEM_S2", [1, 130, 130, make_divisible(32 * 1.1)]),
             ("BLOCK1_S4", [1, 65, 65, make_divisible(24 * 1.1)]),
             ("BLOCK2_S8", [1, 33, 33, make_divisible(40 * 1.1)]),
             ("BLOCK3_S16", [1, 17, 17, make_divisible(80 * 1.1)]),
             ("BLOCK5_S32", [1, 9, 9, make_divisible(192 * 1.1)]),
         ],
     ),
     (
-        kimm_models.EfficientNetLiteB2.__name__,
-        kimm_models.EfficientNetLiteB2,
+        kimm_models.efficientnet.EfficientNetLiteB2.__name__,
+        kimm_models.efficientnet.EfficientNetLiteB2,
         260,
         [
             ("STEM_S2", [1, 130, 130, make_divisible(32 * 1.1)]),
             ("BLOCK1_S4", [1, 65, 65, make_divisible(24 * 1.1)]),
             ("BLOCK2_S8", [1, 33, 33, make_divisible(40 * 1.1)]),
             ("BLOCK3_S16", [1, 17, 17, make_divisible(80 * 1.1)]),
             ("BLOCK5_S32", [1, 9, 9, make_divisible(192 * 1.1)]),
         ],
     ),
     (
-        kimm_models.EfficientNetV2S.__name__,
-        kimm_models.EfficientNetV2S,
+        kimm_models.efficientnet.EfficientNetV2S.__name__,
+        kimm_models.efficientnet.EfficientNetV2S,
         300,
         [
             ("STEM_S2", [1, 150, 150, make_divisible(24 * 1.0)]),
             ("BLOCK1_S4", [1, 75, 75, make_divisible(48 * 1.0)]),
             ("BLOCK2_S8", [1, 38, 38, make_divisible(64 * 1.0)]),
             ("BLOCK3_S16", [1, 19, 19, make_divisible(128 * 1.0)]),
             ("BLOCK5_S32", [1, 10, 10, make_divisible(256 * 1.0)]),
         ],
     ),
     (
-        kimm_models.EfficientNetV2B0.__name__,
-        kimm_models.EfficientNetV2B0,
+        kimm_models.efficientnet.EfficientNetV2B0.__name__,
+        kimm_models.efficientnet.EfficientNetV2B0,
         192,
         [
             ("STEM_S2", [1, 96, 96, make_divisible(32 * 1.0)]),
             ("BLOCK1_S4", [1, 48, 48, make_divisible(32 * 1.0)]),
             ("BLOCK2_S8", [1, 24, 24, make_divisible(48 * 1.0)]),
             ("BLOCK3_S16", [1, 12, 12, make_divisible(96 * 1.0)]),
             ("BLOCK5_S32", [1, 6, 6, make_divisible(192 * 1.0)]),
         ],
     ),
     (
-        kimm_models.TinyNetE.__name__,
-        kimm_models.TinyNetE,
+        kimm_models.efficientnet.TinyNetE.__name__,
+        kimm_models.efficientnet.TinyNetE,
         106,
         [
             ("STEM_S2", [1, 53, 53, 32]),
             ("BLOCK1_S4", [1, 27, 27, make_divisible(24 * 0.51)]),
             ("BLOCK2_S8", [1, 14, 14, make_divisible(40 * 0.51)]),
             ("BLOCK3_S16", [1, 7, 7, make_divisible(80 * 0.51)]),
             ("BLOCK5_S32", [1, 4, 4, make_divisible(192 * 0.51)]),
         ],
     ),
     # ghostnet
     (
-        kimm_models.GhostNet100.__name__,
-        kimm_models.GhostNet100,
+        kimm_models.ghostnet.GhostNet100.__name__,
+        kimm_models.ghostnet.GhostNet100,
         224,
         [
             ("STEM_S2", [1, 112, 112, 16]),
             ("BLOCK1_S4", [1, 56, 56, 24]),
             ("BLOCK3_S8", [1, 28, 28, 40]),
             ("BLOCK5_S16", [1, 14, 14, 80]),
             ("BLOCK7_S32", [1, 7, 7, 160]),
         ],
     ),
     (
-        kimm_models.GhostNet100V2.__name__,
-        kimm_models.GhostNet100V2,
+        kimm_models.ghostnet.GhostNet100V2.__name__,
+        kimm_models.ghostnet.GhostNet100V2,
         224,
         [
             ("STEM_S2", [1, 112, 112, 16]),
             ("BLOCK1_S4", [1, 56, 56, 24]),
             ("BLOCK3_S8", [1, 28, 28, 40]),
             ("BLOCK5_S16", [1, 14, 14, 80]),
             ("BLOCK7_S32", [1, 7, 7, 160]),
         ],
     ),
     # hgnet
     (
-        kimm_models.HGNetTiny.__name__,
-        kimm_models.HGNetTiny,
+        kimm_models.hgnet.HGNetTiny.__name__,
+        kimm_models.hgnet.HGNetTiny,
         224,
         [
             ("STEM_S4", [1, 56, 56, 96]),
             ("BLOCK0_S4", [1, 56, 56, 224]),
             ("BLOCK1_S8", [1, 28, 28, 448]),
             ("BLOCK2_S16", [1, 14, 14, 512]),
             ("BLOCK3_S32", [1, 7, 7, 768]),
         ],
     ),
     (
-        kimm_models.HGNetV2B0.__name__,
-        kimm_models.HGNetV2B0,
+        kimm_models.hgnet.HGNetV2B0.__name__,
+        kimm_models.hgnet.HGNetV2B0,
         224,
         [
             ("STEM_S4", [1, 56, 56, 16]),
             ("BLOCK0_S4", [1, 56, 56, 64]),
             ("BLOCK1_S8", [1, 28, 28, 256]),
             ("BLOCK2_S16", [1, 14, 14, 512]),
             ("BLOCK3_S32", [1, 7, 7, 1024]),
         ],
     ),
     # inception_next
     (
-        kimm_models.InceptionNeXtTiny.__name__,
-        kimm_models.InceptionNeXtTiny,
+        kimm_models.inception_next.InceptionNeXtTiny.__name__,
+        kimm_models.inception_next.InceptionNeXtTiny,
         224,
         [
             ("STEM_S4", [1, 56, 56, 96]),
             ("BLOCK0_S4", [1, 56, 56, 96]),
             ("BLOCK1_S8", [1, 28, 28, 192]),
             ("BLOCK2_S16", [1, 14, 14, 384]),
             ("BLOCK3_S32", [1, 7, 7, 768]),
         ],
     ),
     # inception_v3
     (
-        kimm_models.InceptionV3.__name__,
-        kimm_models.InceptionV3,
+        kimm_models.inception_v3.InceptionV3.__name__,
+        kimm_models.inception_v3.InceptionV3,
         299,
         [
             ("STEM_S2", [1, 147, 147, 64]),
             ("BLOCK0_S4", [1, 71, 71, 192]),
             ("BLOCK1_S8", [1, 35, 35, 288]),
             ("BLOCK2_S16", [1, 17, 17, 768]),
             ("BLOCK3_S32", [1, 8, 8, 2048]),
         ],
     ),
     # mobilenet_v2
     (
-        kimm_models.MobileNetV2W050.__name__,
-        kimm_models.MobileNetV2W050,
+        kimm_models.mobilenet_v2.MobileNetV2W050.__name__,
+        kimm_models.mobilenet_v2.MobileNetV2W050,
         224,
         [
             ("STEM_S2", [1, 112, 112, make_divisible(32 * 0.5)]),
             ("BLOCK1_S4", [1, 56, 56, make_divisible(24 * 0.5)]),
             ("BLOCK2_S8", [1, 28, 28, make_divisible(32 * 0.5)]),
             ("BLOCK3_S16", [1, 14, 14, make_divisible(64 * 0.5)]),
             ("BLOCK5_S32", [1, 7, 7, make_divisible(160 * 0.5)]),
         ],
     ),
     # mobilenet_v3
     (
-        kimm_models.LCNet100.__name__,
-        kimm_models.LCNet100,
+        kimm_models.mobilenet_v3.LCNet100.__name__,
+        kimm_models.mobilenet_v3.LCNet100,
         224,
         [
             ("STEM_S2", [1, 112, 112, make_divisible(16 * 1.0)]),
             ("BLOCK1_S4", [1, 56, 56, make_divisible(64 * 1.0)]),
             ("BLOCK2_S8", [1, 28, 28, make_divisible(128 * 1.0)]),
             ("BLOCK3_S16", [1, 14, 14, make_divisible(256 * 1.0)]),
             ("BLOCK5_S32", [1, 7, 7, make_divisible(512 * 1.0)]),
         ],
     ),
     (
-        kimm_models.MobileNetV3W050Small.__name__,
-        kimm_models.MobileNetV3W050Small,
+        kimm_models.mobilenet_v3.MobileNetV3W050Small.__name__,
+        kimm_models.mobilenet_v3.MobileNetV3W050Small,
         224,
         [
             ("STEM_S2", [1, 112, 112, 16]),
             ("BLOCK0_S4", [1, 56, 56, 8]),
             ("BLOCK1_S8", [1, 28, 28, 16]),
             ("BLOCK2_S16", [1, 14, 14, 24]),
             ("BLOCK4_S32", [1, 7, 7, 48]),
         ],
     ),
     (
-        kimm_models.MobileNetV3W100SmallMinimal.__name__,
-        kimm_models.MobileNetV3W100SmallMinimal,
+        kimm_models.mobilenet_v3.MobileNetV3W100SmallMinimal.__name__,
+        kimm_models.mobilenet_v3.MobileNetV3W100SmallMinimal,
         224,
         [
             ("STEM_S2", [1, 112, 112, make_divisible(16 * 1.0)]),
             ("BLOCK0_S4", [1, 56, 56, make_divisible(16 * 1.0)]),
             ("BLOCK1_S8", [1, 28, 28, make_divisible(24 * 1.0)]),
             ("BLOCK2_S16", [1, 14, 14, make_divisible(40 * 1.0)]),
             ("BLOCK4_S32", [1, 7, 7, make_divisible(96 * 1.0)]),
         ],
     ),
     # mobileone
     (
-        kimm_models.MobileOneS0.__name__,
-        kimm_models.MobileOneS0,
+        kimm_models.mobileone.MobileOneS0.__name__,
+        kimm_models.mobileone.MobileOneS0,
         224,
         [
             ("STEM_S2", [1, 112, 112, 48]),
             ("BLOCK0_S4", [1, 56, 56, 48]),
             ("BLOCK1_S8", [1, 28, 28, 128]),
             ("BLOCK2_S16", [1, 14, 14, 256]),
             ("BLOCK3_S32", [1, 7, 7, 1024]),
         ],
     ),
     # mobilevit
     (
-        kimm_models.MobileViTS.__name__,
-        kimm_models.MobileViTS,
+        kimm_models.mobilevit.MobileViTS.__name__,
+        kimm_models.mobilevit.MobileViTS,
         256,
         [
             ("STEM_S2", [1, 128, 128, 16]),
             ("BLOCK1_S4", [1, 64, 64, 64]),
             ("BLOCK2_S8", [1, 32, 32, 96]),
             ("BLOCK3_S16", [1, 16, 16, 128]),
             ("BLOCK4_S32", [1, 8, 8, 160]),
         ],
     ),
     # mobilevitv2
     (
-        kimm_models.MobileViTV2W050.__name__,
-        kimm_models.MobileViTV2W050,
+        kimm_models.mobilevit.MobileViTV2W050.__name__,
+        kimm_models.mobilevit.MobileViTV2W050,
         256,
         [
             ("STEM_S2", [1, 128, 128, 16]),
             ("BLOCK1_S4", [1, 64, 64, 64]),
             ("BLOCK2_S8", [1, 32, 32, 128]),
             ("BLOCK3_S16", [1, 16, 16, 192]),
             ("BLOCK4_S32", [1, 8, 8, 256]),
         ],
     ),
     # regnet
     (
-        kimm_models.RegNetX002.__name__,
-        kimm_models.RegNetX002,
+        kimm_models.regnet.RegNetX002.__name__,
+        kimm_models.regnet.RegNetX002,
         224,
         [
             ("STEM_S2", [1, 112, 112, 32]),
             ("BLOCK0_S4", [1, 56, 56, 24]),
             ("BLOCK1_S8", [1, 28, 28, 56]),
             ("BLOCK2_S16", [1, 14, 14, 152]),
             ("BLOCK3_S32", [1, 7, 7, 368]),
         ],
     ),
     (
-        kimm_models.RegNetY002.__name__,
-        kimm_models.RegNetY002,
+        kimm_models.regnet.RegNetY002.__name__,
+        kimm_models.regnet.RegNetY002,
         224,
         [
             ("STEM_S2", [1, 112, 112, 32]),
             ("BLOCK0_S4", [1, 56, 56, 24]),
             ("BLOCK1_S8", [1, 28, 28, 56]),
             ("BLOCK2_S16", [1, 14, 14, 152]),
             ("BLOCK3_S32", [1, 7, 7, 368]),
         ],
     ),
     # repvgg
     (
-        kimm_models.RepVGGA0.__name__,
-        kimm_models.RepVGGA0,
+        kimm_models.repvgg.RepVGGA0.__name__,
+        kimm_models.repvgg.RepVGGA0,
         224,
         [
             ("STEM_S2", [1, 112, 112, 48]),
             ("BLOCK0_S4", [1, 56, 56, 48]),
             ("BLOCK1_S8", [1, 28, 28, 96]),
             ("BLOCK2_S16", [1, 14, 14, 192]),
             ("BLOCK3_S32", [1, 7, 7, 1280]),
         ],
     ),
     # resnet
     (
-        kimm_models.ResNet18.__name__,
-        kimm_models.ResNet18,
+        kimm_models.resnet.ResNet18.__name__,
+        kimm_models.resnet.ResNet18,
         224,
         [
             ("STEM_S2", [1, 112, 112, 64]),
             ("BLOCK0_S4", [1, 56, 56, 64]),
             ("BLOCK1_S8", [1, 28, 28, 128]),
             ("BLOCK2_S16", [1, 14, 14, 256]),
             ("BLOCK3_S32", [1, 7, 7, 512]),
         ],
     ),
     (
-        kimm_models.ResNet50.__name__,
-        kimm_models.ResNet50,
+        kimm_models.resnet.ResNet50.__name__,
+        kimm_models.resnet.ResNet50,
         224,
         [
             ("STEM_S2", [1, 112, 112, 64]),
             ("BLOCK0_S4", [1, 56, 56, 64 * 4]),
             ("BLOCK1_S8", [1, 28, 28, 128 * 4]),
             ("BLOCK2_S16", [1, 14, 14, 256 * 4]),
             ("BLOCK3_S32", [1, 7, 7, 512 * 4]),
         ],
     ),
     # vgg
     (
-        kimm_models.VGG11.__name__,
-        kimm_models.VGG11,
+        kimm_models.vgg.VGG11.__name__,
+        kimm_models.vgg.VGG11,
         224,
         [
             ("BLOCK0_S1", [1, 224, 224, 64]),
             ("BLOCK1_S2", [1, 112, 112, 128]),
             ("BLOCK2_S4", [1, 56, 56, 256]),
             ("BLOCK3_S8", [1, 28, 28, 512]),
             ("BLOCK4_S16", [1, 14, 14, 512]),
             ("BLOCK5_S32", [1, 7, 7, 512]),
         ],
         None,  # skip weights to save time
     ),
     # vision_transformer
     (
-        kimm_models.VisionTransformerTiny16.__name__,
-        kimm_models.VisionTransformerTiny16,
+        kimm_models.vision_transformer.VisionTransformerTiny16.__name__,
+        kimm_models.vision_transformer.VisionTransformerTiny16,
         384,
         [*((f"BLOCK{i}", [1, 577, 192]) for i in range(5))],
     ),
     (
-        kimm_models.VisionTransformerTiny32.__name__,
-        kimm_models.VisionTransformerTiny32,
+        kimm_models.vision_transformer.VisionTransformerTiny32.__name__,
+        kimm_models.vision_transformer.VisionTransformerTiny32,
         384,
         [*((f"BLOCK{i}", [1, 145, 192]) for i in range(5))],
         None,  # no weights
     ),
     # xception
     (
-        kimm_models.Xception.__name__,
-        kimm_models.Xception,
+        kimm_models.xception.Xception.__name__,
+        kimm_models.xception.Xception,
         299,
         [
             ("STEM_S2", [1, 147, 147, 64]),
             ("BLOCK0_S4", [1, 74, 74, 128]),
             ("BLOCK1_S8", [1, 37, 37, 256]),
             ("BLOCK2_S16", [1, 19, 19, 728]),
             ("BLOCK3_S32", [1, 10, 10, 2048]),
         ],
     ),
 ]
 
 
 @pytest.mark.requires_trainable_backend  # numpy is too slow to test
-class ModelTest(testing.TestCase, parameterized.TestCase):
+class ModelsTest(testing.TestCase, parameterized.TestCase):
     @classmethod
     def setUpClass(cls):
-        cls.original_image_data_format = backend.image_data_format()
+        cls.original_image_data_format = keras.backend.image_data_format()
 
     @classmethod
     def tearDownClass(cls):
-        backend.set_image_data_format(cls.original_image_data_format)
+        keras.backend.set_image_data_format(cls.original_image_data_format)
 
     @parameterized.named_parameters(MODEL_CONFIGS)
-    def test_model_base_channels_last(
-        self, model_class, image_size, features, weights="imagenet"
+    def test_predict(
+        self,
+        model_class,
+        image_size,
+        features,
+        weights="imagenet",
     ):
-        backend.set_image_data_format("channels_last")
-        model = model_class(weights=weights)
+        # We also enable feature_extractor=True in model instantiation to
+        # speed up the testing
+
+        # Load the image
         image_path = keras.utils.get_file(
             "elephant.png",
             "https://github.com/james77777778/keras-image-models/releases/download/0.1.0/elephant.png",
         )
-        # preprocessing
-        image = utils.load_img(image_path, target_size=(image_size, image_size))
-        image = utils.img_to_array(image, data_format="channels_last")
-        x = ops.convert_to_tensor(image)
-        x = ops.expand_dims(x, axis=0)
+        image = keras.utils.load_img(
+            image_path, target_size=(image_size, image_size)
+        )
+
+        # Test channels_last and feature_extractor=True
+        keras.backend.set_image_data_format("channels_last")
+        model = model_class(weights=weights, feature_extractor=True)
+        x = keras.utils.img_to_array(image, data_format="channels_last")
+        x = keras.ops.expand_dims(keras.ops.convert_to_tensor(x), axis=0)
 
         y = model(x, training=False)
 
+        # Verify output correctness
+        prob = y["TOP"]
         if weights == "imagenet":
-            names = [p[1] for p in decode_predictions(y)[0]]
+            names = [p[1] for p in decode_predictions(prob)[0]]
             # Test correct label is in top 3 (weak correctness test).
             self.assertIn("African_elephant", names[:3])
         elif weights is None:
-            self.assertEqual(list(y.shape), [1, 1000])
+            self.assertEqual(list(prob.shape), [1, 1000])
 
-    @parameterized.named_parameters(MODEL_CONFIGS)
-    def test_model_base_channels_first(
-        self, model_class, image_size, features, weights="imagenet"
-    ):
+        # Verify features
+        self.assertIsInstance(y, dict)
+        self.assertContainsSubset(
+            model_class.available_feature_keys, list(y.keys())
+        )
+        for feature_info in features:
+            name, shape = feature_info
+            self.assertEqual(list(y[name].shape), shape)
+
+        # Test channels_first
         if (
             len(tf.config.list_physical_devices("GPU")) == 0
-            and backend.backend() == "tensorflow"
+            and keras.backend.backend() == "tensorflow"
         ):
-            self.skipTest(
-                "Conv2D doesn't support channels_first using CPU with "
-                "tensorflow backend"
-            )
+            # TensorFlow doesn't support channels_first using CPU
+            return
 
-        backend.set_image_data_format("channels_first")
+        keras.backend.set_image_data_format("channels_first")
         model = model_class(weights=weights)
-        image_path = keras.utils.get_file(
-            "elephant.png",
-            "https://github.com/james77777778/keras-image-models/releases/download/0.1.0/elephant.png",
-        )
-        # preprocessing
-        image = utils.load_img(image_path, target_size=(image_size, image_size))
-        image = utils.img_to_array(image, data_format="channels_first")
-        x = ops.convert_to_tensor(image)
-        x = ops.expand_dims(x, axis=0)
+        x = keras.utils.img_to_array(image, data_format="channels_first")
+        x = keras.ops.expand_dims(keras.ops.convert_to_tensor(x), axis=0)
 
         y = model(x, training=False)
 
+        # Verify output correctness
         if weights == "imagenet":
             names = [p[1] for p in decode_predictions(y)[0]]
             # Test correct label is in top 3 (weak correctness test).
             self.assertIn("African_elephant", names[:3])
         elif weights is None:
             self.assertEqual(list(y.shape), [1, 1000])
 
-    @parameterized.named_parameters(MODEL_CONFIGS)
-    def test_model_feature_extractor(
-        self, model_class, image_size, features, weights="imagenet"
-    ):
-        backend.set_image_data_format("channels_last")
-        x = random.uniform([1, image_size, image_size, 3]) * 255.0
-        model = model_class(weights=None, feature_extractor=True)
-
-        y = model(x, training=False)
-
-        self.assertIsInstance(y, dict)
-        self.assertContainsSubset(
-            model_class.available_feature_keys, list(y.keys())
-        )
-        for feature_info in features:
-            name, shape = feature_info
-            self.assertEqual(list(y[name].shape), shape)
-
     @parameterized.named_parameters(
-        (kimm_models.RepVGGA0.__name__, kimm_models.RepVGGA0, 224),
-        (kimm_models.MobileOneS0.__name__, kimm_models.MobileOneS0, 224),
+        (
+            kimm_models.repvgg.RepVGGA0.__name__,
+            kimm_models.repvgg.RepVGGA0,
+            224,
+        ),
+        (
+            kimm_models.mobileone.MobileOneS0.__name__,
+            kimm_models.mobileone.MobileOneS0,
+            224,
+        ),
     )
-    def test_model_get_reparameterized_model(self, model_class, image_size):
-        x = random.uniform([1, image_size, image_size, 3]) * 255.0
+    def test_get_reparameterized_model(
+        self,
+        model_class,
+        image_size,
+    ):
+        x = keras.random.uniform([1, image_size, image_size, 3]) * 255.0
         model = model_class()
         reparameterized_model = model.get_reparameterized_model()
 
         y1 = model(x, training=False)
         y2 = reparameterized_model(x, training=False)
 
         self.assertAllClose(y1, y2, atol=1e-5)
 
     @pytest.mark.serialization
     @parameterized.named_parameters(MODEL_CONFIGS)
-    def test_model_serialization(
-        self, model_class, image_size, features, weights="imagenet"
+    def test_serialization(
+        self,
+        model_class,
+        image_size,
+        features,
+        weights="imagenet",
     ):
-        backend.set_image_data_format("channels_last")
-        x = random.uniform([1, image_size, image_size, 3]) * 255.0
+        keras.backend.set_image_data_format("channels_last")
+        x = keras.random.uniform([1, image_size, image_size, 3]) * 255.0
         temp_dir = self.get_temp_dir()
         model1 = model_class(weights=None)
+        if hasattr(model1, "get_reparameterized_model"):
+            model1 = model1.get_reparameterized_model()
 
         y1 = model1(x, training=False)
         model1.save(temp_dir + "/model.keras")
-        model2 = models.load_model(temp_dir + "/model.keras")
+        model2 = keras.models.load_model(temp_dir + "/model.keras")
         y2 = model2(x, training=False)
 
         self.assertAllClose(y1, y2)
```

### Comparing `kimm-0.1.8/kimm/models/resnet.py` & `kimm-0.2.0/kimm/_src/models/resnet.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 import typing
 
 import keras
 from keras import backend
 from keras import layers
 
-from kimm.blocks import apply_conv2d_block
-from kimm.models.base_model import BaseModel
-from kimm.utils import add_model_to_registry
+from kimm._src.blocks.conv2d import apply_conv2d_block
+from kimm._src.kimm_export import kimm_export
+from kimm._src.models.base_model import BaseModel
+from kimm._src.utils.model_registry import add_model_to_registry
 
 
 def apply_basic_block(
     inputs,
     output_channels: int,
     strides: int = 1,
     activation="relu",
@@ -192,222 +193,132 @@
     def fix_config(self, config):
         unused_kwargs = ["block_fn", "num_blocks"]
         for k in unused_kwargs:
             config.pop(k, None)
         return config
 
 
-"""
-Model Definition
-"""
+# Model Definition
 
 
-class ResNet18(ResNet):
-    available_weights = [
-        (
-            "imagenet",
-            ResNet.default_origin,
-            "resnet18_resnet18.a1_in1k.keras",
-        )
-    ]
+class ResNetVariant(ResNet):
+    # Parameters
+    block_fn = None
+    num_blocks = None
 
     def __init__(
         self,
         input_tensor: keras.KerasTensor = None,
         input_shape: typing.Optional[typing.Sequence[int]] = None,
         include_preprocessing: bool = True,
         include_top: bool = True,
         pooling: typing.Optional[str] = None,
         dropout_rate: float = 0.0,
         classes: int = 1000,
         classifier_activation: str = "softmax",
         weights: typing.Optional[str] = "imagenet",
-        name: str = "ResNet18",
+        name: typing.Optional[str] = None,
         **kwargs,
     ):
+        if type(self) is ResNetVariant:
+            raise NotImplementedError(
+                f"Cannot instantiate base class: {self.__class__.__name__}. "
+                "You should use its subclasses."
+            )
         kwargs = self.fix_config(kwargs)
         super().__init__(
-            "basic",
-            [2, 2, 2, 2],
+            block_fn=self.block_fn,
+            num_blocks=self.num_blocks,
             input_tensor=input_tensor,
             input_shape=input_shape,
             include_preprocessing=include_preprocessing,
             include_top=include_top,
             pooling=pooling,
             dropout_rate=dropout_rate,
             classes=classes,
             classifier_activation=classifier_activation,
             weights=weights,
-            name=name,
+            name=name or str(self.__class__.__name__),
             **kwargs,
         )
 
 
-class ResNet34(ResNet):
+@kimm_export(parent_path=["kimm.models", "kimm.models.resnet"])
+class ResNet18(ResNetVariant):
     available_weights = [
         (
             "imagenet",
             ResNet.default_origin,
-            "resnet34_resnet34.a1_in1k.keras",
+            "resnet18_resnet18.a1_in1k.keras",
         )
     ]
 
-    def __init__(
-        self,
-        input_tensor: keras.KerasTensor = None,
-        input_shape: typing.Optional[typing.Sequence[int]] = None,
-        include_preprocessing: bool = True,
-        include_top: bool = True,
-        pooling: typing.Optional[str] = None,
-        dropout_rate: float = 0.0,
-        classes: int = 1000,
-        classifier_activation: str = "softmax",
-        weights: typing.Optional[str] = "imagenet",
-        name: str = "ResNet34",
-        **kwargs,
-    ):
-        kwargs = self.fix_config(kwargs)
-        super().__init__(
-            "basic",
-            [3, 4, 6, 3],
-            input_tensor=input_tensor,
-            input_shape=input_shape,
-            include_preprocessing=include_preprocessing,
-            include_top=include_top,
-            pooling=pooling,
-            dropout_rate=dropout_rate,
-            classes=classes,
-            classifier_activation=classifier_activation,
-            weights=weights,
-            name=name,
-            **kwargs,
+    # Parameters
+    block_fn = "basic"
+    num_blocks = [2, 2, 2, 2]
+
+
+@kimm_export(parent_path=["kimm.models", "kimm.models.resnet"])
+class ResNet34(ResNetVariant):
+    available_weights = [
+        (
+            "imagenet",
+            ResNet.default_origin,
+            "resnet34_resnet34.a1_in1k.keras",
         )
+    ]
 
+    # Parameters
+    block_fn = "basic"
+    num_blocks = [3, 4, 6, 3]
 
-class ResNet50(ResNet):
+
+@kimm_export(parent_path=["kimm.models", "kimm.models.resnet"])
+class ResNet50(ResNetVariant):
     available_weights = [
         (
             "imagenet",
             ResNet.default_origin,
             "resnet50_resnet50.a1_in1k.keras",
         )
     ]
 
-    def __init__(
-        self,
-        input_tensor: keras.KerasTensor = None,
-        input_shape: typing.Optional[typing.Sequence[int]] = None,
-        include_preprocessing: bool = True,
-        include_top: bool = True,
-        pooling: typing.Optional[str] = None,
-        dropout_rate: float = 0.0,
-        classes: int = 1000,
-        classifier_activation: str = "softmax",
-        weights: typing.Optional[str] = "imagenet",
-        name: str = "ResNet50",
-        **kwargs,
-    ):
-        kwargs = self.fix_config(kwargs)
-        super().__init__(
-            "bottleneck",
-            [3, 4, 6, 3],
-            input_tensor=input_tensor,
-            input_shape=input_shape,
-            include_preprocessing=include_preprocessing,
-            include_top=include_top,
-            pooling=pooling,
-            dropout_rate=dropout_rate,
-            classes=classes,
-            classifier_activation=classifier_activation,
-            weights=weights,
-            name=name,
-            **kwargs,
-        )
+    # Parameters
+    block_fn = "bottleneck"
+    num_blocks = [3, 4, 6, 3]
 
 
-class ResNet101(ResNet):
+@kimm_export(parent_path=["kimm.models", "kimm.models.resnet"])
+class ResNet101(ResNetVariant):
     available_weights = [
         (
             "imagenet",
             ResNet.default_origin,
             "resnet101_resnet101.a1_in1k.keras",
         )
     ]
 
-    def __init__(
-        self,
-        input_tensor: keras.KerasTensor = None,
-        input_shape: typing.Optional[typing.Sequence[int]] = None,
-        include_preprocessing: bool = True,
-        include_top: bool = True,
-        pooling: typing.Optional[str] = None,
-        dropout_rate: float = 0.0,
-        classes: int = 1000,
-        classifier_activation: str = "softmax",
-        weights: typing.Optional[str] = "imagenet",
-        name: str = "ResNet101",
-        **kwargs,
-    ):
-        kwargs = self.fix_config(kwargs)
-        super().__init__(
-            "bottleneck",
-            [3, 4, 23, 3],
-            input_tensor=input_tensor,
-            input_shape=input_shape,
-            include_preprocessing=include_preprocessing,
-            include_top=include_top,
-            pooling=pooling,
-            dropout_rate=dropout_rate,
-            classes=classes,
-            classifier_activation=classifier_activation,
-            weights=weights,
-            name=name,
-            **kwargs,
-        )
+    # Parameters
+    block_fn = "bottleneck"
+    num_blocks = [3, 4, 23, 3]
 
 
-class ResNet152(ResNet):
+@kimm_export(parent_path=["kimm.models", "kimm.models.resnet"])
+class ResNet152(ResNetVariant):
     available_weights = [
         (
             "imagenet",
             ResNet.default_origin,
             "resnet152_resnet152.a1_in1k.keras",
         )
     ]
 
-    def __init__(
-        self,
-        input_tensor: keras.KerasTensor = None,
-        input_shape: typing.Optional[typing.Sequence[int]] = None,
-        include_preprocessing: bool = True,
-        include_top: bool = True,
-        pooling: typing.Optional[str] = None,
-        dropout_rate: float = 0.0,
-        classes: int = 1000,
-        classifier_activation: str = "softmax",
-        weights: typing.Optional[str] = "imagenet",
-        name: str = "ResNet152",
-        **kwargs,
-    ):
-        kwargs = self.fix_config(kwargs)
-        super().__init__(
-            "bottleneck",
-            [3, 8, 36, 3],
-            input_tensor=input_tensor,
-            input_shape=input_shape,
-            include_preprocessing=include_preprocessing,
-            include_top=include_top,
-            pooling=pooling,
-            dropout_rate=dropout_rate,
-            classes=classes,
-            classifier_activation=classifier_activation,
-            weights=weights,
-            name=name,
-            **kwargs,
-        )
+    # Parameters
+    block_fn = "bottleneck"
+    num_blocks = [3, 8, 36, 3]
 
 
 add_model_to_registry(ResNet18, "imagenet")
 add_model_to_registry(ResNet34, "imagenet")
 add_model_to_registry(ResNet50, "imagenet")
 add_model_to_registry(ResNet101, "imagenet")
 add_model_to_registry(ResNet152, "imagenet")
```

### Comparing `kimm-0.1.8/kimm/models/vision_transformer.py` & `kimm-0.2.0/kimm/_src/models/regnet.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,578 +1,768 @@
 import typing
 
 import keras
+import numpy as np
 from keras import backend
 from keras import layers
-from keras import ops
 
-from kimm import layers as kimm_layers
-from kimm.blocks import apply_transformer_block
-from kimm.models.base_model import BaseModel
-from kimm.utils import add_model_to_registry
+from kimm._src.blocks.conv2d import apply_conv2d_block
+from kimm._src.blocks.squeeze_and_excitation import apply_se_block
+from kimm._src.kimm_export import kimm_export
+from kimm._src.models.base_model import BaseModel
+from kimm._src.utils.model_registry import add_model_to_registry
+
+
+def _adjust_widths_and_groups(widths, groups, expansion_ratio):
+    def _quantize_float(f, q):
+        return int(round(f / q) * q)
+
+    bottleneck_widths = [int(w * b) for w, b in zip(widths, expansion_ratio)]
+    groups = [min(g, w_bot) for g, w_bot in zip(groups, bottleneck_widths)]
+    bottleneck_widths = [
+        _quantize_float(w_bot, g) for w_bot, g in zip(bottleneck_widths, groups)
+    ]
+    widths = [
+        int(w_bot / b) for w_bot, b in zip(bottleneck_widths, expansion_ratio)
+    ]
+    return widths, groups
+
+
+def _generate_regnet(
+    width_init,
+    width_slope,
+    width_mult,
+    group_size,
+    depth,
+    quant=8,
+    expansion_ratio=1.0,
+):
+    widths_cont = np.arange(depth) * width_slope + width_init
+    width_exps = np.round(np.log(widths_cont / width_init) / np.log(width_mult))
+    widths = (
+        np.round(
+            np.divide(width_init * np.power(width_mult, width_exps), quant)
+        )
+        * quant
+    )
+    num_stages = len(np.unique(widths))
+    groups = np.array([group_size for _ in range(num_stages)])
+
+    widths = np.array(widths).astype(int).tolist()
+    stage_gs = groups.astype(int).tolist()
+
+    # Convert to per-stage format
+    stage_widths, stage_depths = np.unique(widths, return_counts=True)
+    stage_e = [expansion_ratio for _ in range(num_stages)]
+    stage_strides = []
+    for _ in range(num_stages):
+        stride = 2
+        stage_strides.append(stride)
+
+    # Adjust the compatibility of ws and gws
+    stage_widths, stage_gs = _adjust_widths_and_groups(
+        stage_widths, stage_gs, stage_e
+    )
+    per_stage_args = [
+        params
+        for params in zip(
+            stage_widths,
+            stage_strides,
+            stage_depths,
+            stage_e,
+            stage_gs,
+        )
+    ]
+    return per_stage_args
+
+
+def apply_bottleneck_block(
+    inputs,
+    output_channels: int,
+    strides: int = 1,
+    expansion_ratio: float = 1.0,
+    group_size: int = 1,
+    se_ratio: float = 0.25,
+    activation="relu",
+    linear_out: bool = False,
+    name="bottleneck_block",
+):
+    channels_axis = -1 if backend.image_data_format() == "channels_last" else -3
+    input_channels = inputs.shape[channels_axis]
+    expansion_channels = int(round(output_channels * expansion_ratio))
+    groups = expansion_channels // group_size
+
+    shortcut = inputs
+    x = inputs
+    x = apply_conv2d_block(
+        x,
+        expansion_channels,
+        1,
+        1,
+        activation=activation,
+        name=f"{name}_conv1",
+    )
+    x = apply_conv2d_block(
+        x,
+        expansion_channels,
+        3,
+        strides,
+        groups=groups,
+        activation=activation,
+        name=f"{name}_conv2",
+    )
+    if se_ratio > 0.0:
+        x = apply_se_block(
+            x,
+            se_ratio,
+            activation,
+            se_input_channels=input_channels,
+            name=f"{name}_se",
+        )
+    x = apply_conv2d_block(
+        x,
+        output_channels,
+        1,
+        1,
+        activation=None,
+        name=f"{name}_conv3",
+    )
+
+    # downsampling
+    if strides != 1 or input_channels != output_channels:
+        shortcut = apply_conv2d_block(
+            shortcut,
+            output_channels,
+            1,
+            strides,
+            activation=None,
+            name=f"{name}_downsample",
+        )
+
+    x = layers.Add(name=f"{name}_add")([x, shortcut])
+    if not linear_out:
+        x = layers.Activation(activation=activation, name=f"{name}")(x)
+    return x
 
 
 @keras.saving.register_keras_serializable(package="kimm")
-class VisionTransformer(BaseModel):
+class RegNet(BaseModel):
+    available_feature_keys = [
+        "STEM_S2",
+        *[f"BLOCK{i}_S{j}" for i, j in zip(range(4), [4, 8, 16, 32])],
+    ]
+
     def __init__(
         self,
-        patch_size: int,
-        embed_dim: int,
-        depth: int,
-        num_heads: int,
-        mlp_ratio: float = 4.0,
-        use_qkv_bias: bool = True,
-        use_qk_norm: bool = False,
-        pos_dropout_rate: float = 0.0,
+        w0: int = 80,
+        wa: float = 42.64,
+        wm: float = 2.66,
+        group_size: int = 24,
+        depth: int = 21,
+        se_ratio: float = 0.0,
         **kwargs,
     ):
         kwargs["weights_url"] = self.get_weights_url(kwargs["weights"])
 
+        per_stage_config = _generate_regnet(w0, wa, wm, group_size, depth)
+
         input_tensor = kwargs.pop("input_tensor", None)
-        self.set_properties(kwargs, 384)
-        if self._pooling is not None:
-            raise ValueError(
-                "`VisionTransformer` doesn't support `pooling`. "
-                f"Received: pooling={self._pooling}"
-            )
+        self.set_properties(kwargs)
         inputs = self.determine_input_tensor(
             input_tensor,
             self._input_shape,
             self._default_size,
-            static_shape=True,
         )
         x = inputs
 
-        x = self.build_preprocessing(x, "-1_1")
+        x = self.build_preprocessing(x, "imagenet")
 
         # Prepare feature extraction
         features = {}
 
-        # Patch embedding
-        x = layers.Conv2D(
-            embed_dim,
-            kernel_size=patch_size,
-            strides=patch_size,
-            padding="valid",
-            use_bias=True,
-            name="patch_embed_conv",
-        )(x)
-
-        # TODO: natively support channels_first
-        if backend.image_data_format() == "channels_first":
-            x = ops.transpose(x, [0, 2, 3, 1])
-
-        x = layers.Reshape((-1, embed_dim))(x)
-        x = kimm_layers.PositionEmbedding(name="postition_embedding")(x)
-        features["EMBEDDING"] = x
-        x = layers.Dropout(pos_dropout_rate, name="pos_dropout")(x)
-
-        for i in range(depth):
-            x = apply_transformer_block(
-                x,
-                embed_dim,
-                num_heads,
-                mlp_ratio,
-                use_qkv_bias,
-                use_qk_norm,
-                activation="gelu",
-                name=f"blocks_{i}",
-            )
-            features[f"BLOCK{i}"] = x
-        x = layers.LayerNormalization(epsilon=1e-6, name="norm")(x)
+        # stem
+        stem_channels = 32
+        x = apply_conv2d_block(
+            x, stem_channels, 3, 2, activation="relu", name="stem"
+        )
+        features["STEM_S2"] = x
+
+        # stages
+        current_stride = 2
+        for current_stage_idx, params in enumerate(per_stage_config):
+            c, s, d, e, g = params
+            current_stride *= s
+            # blocks
+            for current_block_idx in range(d):
+                s = s if current_block_idx == 0 else 1
+                name = f"s{current_stage_idx + 1}_b{current_block_idx + 1}"
+                x = apply_bottleneck_block(x, c, s, e, g, se_ratio, name=name)
+            # add feature
+            features[f"BLOCK{current_stage_idx}_S{current_stride}"] = x
 
         # Head
-        if self._include_top:
-            x = self.build_top(
-                x,
-                self._classes,
-                self._classifier_activation,
-                self._dropout_rate,
-            )
+        x = self.build_head(x)
 
         super().__init__(inputs=inputs, outputs=x, features=features, **kwargs)
 
         # All references to `self` below this line
-        self.patch_size = patch_size
-        self.embed_dim = embed_dim
+        self.w0 = w0
+        self.wa = wa
+        self.wm = wm
+        self.group_size = group_size
         self.depth = depth
-        self.num_heads = num_heads
-        self.mlp_ratio = mlp_ratio
-        self.use_qkv_bias = use_qkv_bias
-        self.use_qk_norm = use_qk_norm
-        self.pos_dropout_rate = pos_dropout_rate
-
-    def build_top(self, inputs, classes, classifier_activation, dropout_rate):
-        x = inputs[:, 0]  # class token
-        x = layers.Dropout(dropout_rate, name="head_drop")(x)
-        x = layers.Dense(
-            classes, activation=classifier_activation, name="head"
-        )(x)
-        return x
+        self.se_ratio = se_ratio
 
     def get_config(self):
         config = super().get_config()
         config.update(
             {
-                "patch_size": self.patch_size,
-                "embed_dim": self.embed_dim,
+                "w0": self.w0,
+                "wa": self.wa,
+                "wm": self.wm,
+                "group_size": self.group_size,
                 "depth": self.depth,
-                "num_heads": self.num_heads,
-                "mlp_ratio": self.mlp_ratio,
-                "use_qkv_bias": self.use_qkv_bias,
-                "use_qk_norm": self.use_qk_norm,
-                "pos_dropout_rate": self.pos_dropout_rate,
+                "se_ratio": self.se_ratio,
             }
         )
         return config
 
     def fix_config(self, config):
-        unused_kwargs = [
-            "patch_size",
-            "embed_dim",
-            "depth",
-            "num_heads",
-            "mlp_ratio",
-            "use_qkv_bias",
-            "use_qk_norm",
-            "pos_dropout_rate",
-        ]
+        unused_kwargs = ["w0", "wa", "wm", "group_size", "depth", "se_ratio"]
         for k in unused_kwargs:
             config.pop(k, None)
         return config
 
 
-"""
-Model Definition
-"""
+# Model Definition
 
 
-class VisionTransformerTiny16(VisionTransformer):
-    available_feature_keys = [
-        "EMBEDDING",
-        *[f"BLOCK{i}" for i in range(12)],
-    ]
-    available_weights = [
-        (
-            "imagenet",
-            VisionTransformer.default_origin,
-            "visiontransformertiny16_vit_tiny_patch16_384.keras",
-        )
-    ]
+class RegNetVariant(RegNet):
+    # Parameters
+    w0 = None
+    wa = None
+    wm = None
+    group_size = None
+    depth = None
+    se_ratio = None
 
     def __init__(
         self,
-        mlp_ratio: float = 4.0,
-        use_qkv_bias: bool = True,
-        use_qk_norm: bool = False,
         input_tensor: keras.KerasTensor = None,
         input_shape: typing.Optional[typing.Sequence[int]] = None,
         include_preprocessing: bool = True,
         include_top: bool = True,
         pooling: typing.Optional[str] = None,
-        pos_dropout_rate: float = 0.0,
-        dropout_rate: float = 0.1,
+        dropout_rate: float = 0.0,
         classes: int = 1000,
         classifier_activation: str = "softmax",
         weights: typing.Optional[str] = "imagenet",
-        name: str = "VisionTransformerTiny16",
+        name: typing.Optional[str] = None,
         **kwargs,
     ):
+        if type(self) is RegNetVariant:
+            raise NotImplementedError(
+                f"Cannot instantiate base class: {self.__class__.__name__}. "
+                "You should use its subclasses."
+            )
         kwargs = self.fix_config(kwargs)
         super().__init__(
-            16,
-            192,
-            12,
-            3,
-            mlp_ratio,
-            use_qkv_bias,
-            use_qk_norm,
-            pos_dropout_rate,
+            w0=self.w0,
+            wa=self.wa,
+            wm=self.wm,
+            group_size=self.group_size,
+            depth=self.depth,
+            se_ratio=self.se_ratio,
             input_tensor=input_tensor,
             input_shape=input_shape,
             include_preprocessing=include_preprocessing,
             include_top=include_top,
             pooling=pooling,
             dropout_rate=dropout_rate,
             classes=classes,
             classifier_activation=classifier_activation,
             weights=weights,
-            name=name,
+            name=name or str(self.__class__.__name__),
             **kwargs,
         )
 
 
-class VisionTransformerTiny32(VisionTransformer):
-    available_feature_keys = [
-        "EMBEDDING",
-        *[f"BLOCK{i}" for i in range(12)],
+@kimm_export(parent_path=["kimm.models", "kimm.models.regnet"])
+class RegNetX002(RegNetVariant):
+    available_weights = [
+        (
+            "imagenet",
+            RegNet.default_origin,
+            "regnetx002_regnetx_002.pycls_in1k.keras",
+        )
     ]
-    available_weights = []
 
-    def __init__(
-        self,
-        mlp_ratio: float = 4.0,
-        use_qkv_bias: bool = True,
-        use_qk_norm: bool = False,
-        input_tensor: keras.KerasTensor = None,
-        input_shape: typing.Optional[typing.Sequence[int]] = None,
-        include_preprocessing: bool = True,
-        include_top: bool = True,
-        pooling: typing.Optional[str] = None,
-        pos_dropout_rate: float = 0.0,
-        dropout_rate: float = 0.1,
-        classes: int = 1000,
-        classifier_activation: str = "softmax",
-        weights: typing.Optional[str] = None,
-        name: str = "VisionTransformerTiny32",
-        **kwargs,
-    ):
-        kwargs = self.fix_config(kwargs)
-        super().__init__(
-            32,
-            192,
-            12,
-            3,
-            mlp_ratio,
-            use_qkv_bias,
-            use_qk_norm,
-            pos_dropout_rate,
-            input_tensor=input_tensor,
-            input_shape=input_shape,
-            include_preprocessing=include_preprocessing,
-            include_top=include_top,
-            pooling=pooling,
-            dropout_rate=dropout_rate,
-            classes=classes,
-            classifier_activation=classifier_activation,
-            weights=weights,
-            name=name,
-            **kwargs,
+    # Parameters
+    w0 = 24
+    wa = 36.44
+    wm = 2.49
+    group_size = 8
+    depth = 13
+    se_ratio = 0.0
+
+
+@kimm_export(parent_path=["kimm.models", "kimm.models.regnet"])
+class RegNetY002(RegNetVariant):
+    available_weights = [
+        (
+            "imagenet",
+            RegNet.default_origin,
+            "regnety002_regnety_002.pycls_in1k.keras",
         )
+    ]
 
+    # Parameters
+    w0 = 24
+    wa = 36.44
+    wm = 2.49
+    group_size = 8
+    depth = 13
+    se_ratio = 0.25
 
-class VisionTransformerSmall16(VisionTransformer):
-    available_feature_keys = [
-        "EMBEDDING",
-        *[f"BLOCK{i}" for i in range(12)],
+
+@kimm_export(parent_path=["kimm.models", "kimm.models.regnet"])
+class RegNetX004(RegNetVariant):
+    available_weights = [
+        (
+            "imagenet",
+            RegNet.default_origin,
+            "regnetx004_regnetx_004.pycls_in1k.keras",
+        )
     ]
+
+    # Parameters
+    w0 = 24
+    wa = 24.48
+    wm = 2.54
+    group_size = 16
+    depth = 22
+    se_ratio = 0.0
+
+
+@kimm_export(parent_path=["kimm.models", "kimm.models.regnet"])
+class RegNetY004(RegNetVariant):
     available_weights = [
         (
             "imagenet",
-            VisionTransformer.default_origin,
-            "visiontransformersmall16_vit_small_patch16_384.keras",
+            RegNet.default_origin,
+            "regnety004_regnety_004.tv2_in1k.keras",
         )
     ]
 
-    def __init__(
-        self,
-        mlp_ratio: float = 4.0,
-        use_qkv_bias: bool = True,
-        use_qk_norm: bool = False,
-        input_tensor: keras.KerasTensor = None,
-        input_shape: typing.Optional[typing.Sequence[int]] = None,
-        include_preprocessing: bool = True,
-        include_top: bool = True,
-        pooling: typing.Optional[str] = None,
-        pos_dropout_rate: float = 0.0,
-        dropout_rate: float = 0.1,
-        classes: int = 1000,
-        classifier_activation: str = "softmax",
-        weights: typing.Optional[str] = "imagenet",
-        name: str = "VisionTransformerSmall16",
-        **kwargs,
-    ):
-        kwargs = self.fix_config(kwargs)
-        super().__init__(
-            16,
-            384,
-            12,
-            6,
-            mlp_ratio,
-            use_qkv_bias,
-            use_qk_norm,
-            pos_dropout_rate,
-            input_tensor=input_tensor,
-            input_shape=input_shape,
-            include_preprocessing=include_preprocessing,
-            include_top=include_top,
-            pooling=pooling,
-            dropout_rate=dropout_rate,
-            classes=classes,
-            classifier_activation=classifier_activation,
-            weights=weights,
-            name=name,
-            **kwargs,
+    # Parameters
+    w0 = 48
+    wa = 27.89
+    wm = 2.09
+    group_size = 8
+    depth = 16
+    se_ratio = 0.25
+
+
+@kimm_export(parent_path=["kimm.models", "kimm.models.regnet"])
+class RegNetX006(RegNetVariant):
+    available_weights = [
+        (
+            "imagenet",
+            RegNet.default_origin,
+            "regnetx006_regnetx_006.pycls_in1k.keras",
         )
+    ]
 
+    # Parameters
+    w0 = 48
+    wa = 36.97
+    wm = 2.24
+    group_size = 24
+    depth = 16
+    se_ratio = 0.0
 
-class VisionTransformerSmall32(VisionTransformer):
-    available_feature_keys = [
-        "EMBEDDING",
-        *[f"BLOCK{i}" for i in range(12)],
+
+@kimm_export(parent_path=["kimm.models", "kimm.models.regnet"])
+class RegNetY006(RegNetVariant):
+    available_weights = [
+        (
+            "imagenet",
+            RegNet.default_origin,
+            "regnety006_regnety_006.pycls_in1k.keras",
+        )
     ]
+
+    # Parameters
+    w0 = 48
+    wa = 32.54
+    wm = 2.32
+    group_size = 16
+    depth = 15
+    se_ratio = 0.25
+
+
+@kimm_export(parent_path=["kimm.models", "kimm.models.regnet"])
+class RegNetX008(RegNetVariant):
     available_weights = [
         (
             "imagenet",
-            VisionTransformer.default_origin,
-            "visiontransformersmall32_vit_small_patch32_384.keras",
+            RegNet.default_origin,
+            "regnetx008_regnetx_008.tv2_in1k.keras",
         )
     ]
 
-    def __init__(
-        self,
-        mlp_ratio: float = 4.0,
-        use_qkv_bias: bool = True,
-        use_qk_norm: bool = False,
-        input_tensor: keras.KerasTensor = None,
-        input_shape: typing.Optional[typing.Sequence[int]] = None,
-        include_preprocessing: bool = True,
-        include_top: bool = True,
-        pooling: typing.Optional[str] = None,
-        pos_dropout_rate: float = 0.0,
-        dropout_rate: float = 0.1,
-        classes: int = 1000,
-        classifier_activation: str = "softmax",
-        weights: typing.Optional[str] = "imagenet",
-        name: str = "VisionTransformerSmall32",
-        **kwargs,
-    ):
-        kwargs = self.fix_config(kwargs)
-        super().__init__(
-            32,
-            384,
-            12,
-            6,
-            mlp_ratio,
-            use_qkv_bias,
-            use_qk_norm,
-            pos_dropout_rate,
-            input_tensor=input_tensor,
-            input_shape=input_shape,
-            include_preprocessing=include_preprocessing,
-            include_top=include_top,
-            pooling=pooling,
-            dropout_rate=dropout_rate,
-            classes=classes,
-            classifier_activation=classifier_activation,
-            weights=weights,
-            name=name,
-            **kwargs,
+    # Parameters
+    w0 = 56
+    wa = 35.73
+    wm = 2.28
+    group_size = 16
+    depth = 16
+    se_ratio = 0.0
+
+
+@kimm_export(parent_path=["kimm.models", "kimm.models.regnet"])
+class RegNetY008(RegNetVariant):
+    available_weights = [
+        (
+            "imagenet",
+            RegNet.default_origin,
+            "regnety008_regnety_008.pycls_in1k.keras",
         )
+    ]
 
+    # Parameters
+    w0 = 56
+    wa = 38.84
+    wm = 2.4
+    group_size = 16
+    depth = 14
+    se_ratio = 0.25
 
-class VisionTransformerBase16(VisionTransformer):
-    available_feature_keys = [
-        "EMBEDDING",
-        *[f"BLOCK{i}" for i in range(12)],
+
+@kimm_export(parent_path=["kimm.models", "kimm.models.regnet"])
+class RegNetX016(RegNetVariant):
+    available_weights = [
+        (
+            "imagenet",
+            RegNet.default_origin,
+            "regnetx016_regnetx_016.tv2_in1k.keras",
+        )
     ]
+
+    # Parameters
+    w0 = 80
+    wa = 34.01
+    wm = 2.25
+    group_size = 24
+    depth = 18
+    se_ratio = 0.0
+
+
+@kimm_export(parent_path=["kimm.models", "kimm.models.regnet"])
+class RegNetY016(RegNetVariant):
     available_weights = [
         (
             "imagenet",
-            VisionTransformer.default_origin,
-            "visiontransformerbase16_vit_base_patch16_384.keras",
+            RegNet.default_origin,
+            "regnety016_regnety_016.tv2_in1k.keras",
         )
     ]
 
-    def __init__(
-        self,
-        mlp_ratio: float = 4.0,
-        use_qkv_bias: bool = True,
-        use_qk_norm: bool = False,
-        input_tensor: keras.KerasTensor = None,
-        input_shape: typing.Optional[typing.Sequence[int]] = None,
-        include_preprocessing: bool = True,
-        include_top: bool = True,
-        pooling: typing.Optional[str] = None,
-        pos_dropout_rate: float = 0.0,
-        dropout_rate: float = 0.1,
-        classes: int = 1000,
-        classifier_activation: str = "softmax",
-        weights: typing.Optional[str] = "imagenet",
-        name: str = "VisionTransformerBase16",
-        **kwargs,
-    ):
-        kwargs = self.fix_config(kwargs)
-        super().__init__(
-            16,
-            768,
-            12,
-            12,
-            mlp_ratio,
-            use_qkv_bias,
-            use_qk_norm,
-            pos_dropout_rate,
-            input_tensor=input_tensor,
-            input_shape=input_shape,
-            include_preprocessing=include_preprocessing,
-            include_top=include_top,
-            pooling=pooling,
-            dropout_rate=dropout_rate,
-            classes=classes,
-            classifier_activation=classifier_activation,
-            weights=weights,
-            name=name,
-            **kwargs,
+    # Parameters
+    w0 = 48
+    wa = 20.71
+    wm = 2.65
+    group_size = 24
+    depth = 27
+    se_ratio = 0.25
+
+
+@kimm_export(parent_path=["kimm.models", "kimm.models.regnet"])
+class RegNetX032(RegNetVariant):
+    available_weights = [
+        (
+            "imagenet",
+            RegNet.default_origin,
+            "regnetx032_regnetx_032.tv2_in1k.keras",
         )
+    ]
 
+    # Parameters
+    w0 = 88
+    wa = 26.31
+    wm = 2.25
+    group_size = 48
+    depth = 25
+    se_ratio = 0.0
 
-class VisionTransformerBase32(VisionTransformer):
-    available_feature_keys = [
-        "EMBEDDING",
-        *[f"BLOCK{i}" for i in range(12)],
+
+@kimm_export(parent_path=["kimm.models", "kimm.models.regnet"])
+class RegNetY032(RegNetVariant):
+    available_weights = [
+        (
+            "imagenet",
+            RegNet.default_origin,
+            "regnety032_regnety_032.ra_in1k.keras",
+        )
     ]
+
+    # Parameters
+    w0 = 80
+    wa = 42.63
+    wm = 2.66
+    group_size = 24
+    depth = 21
+    se_ratio = 0.25
+
+
+@kimm_export(parent_path=["kimm.models", "kimm.models.regnet"])
+class RegNetX040(RegNetVariant):
     available_weights = [
         (
             "imagenet",
-            VisionTransformer.default_origin,
-            "visiontransformerbase32_vit_base_patch32_384.keras",
+            RegNet.default_origin,
+            "regnetx040_regnetx_040.pycls_in1k.keras",
         )
     ]
 
-    def __init__(
-        self,
-        mlp_ratio: float = 4.0,
-        use_qkv_bias: bool = True,
-        use_qk_norm: bool = False,
-        input_tensor: keras.KerasTensor = None,
-        input_shape: typing.Optional[typing.Sequence[int]] = None,
-        include_preprocessing: bool = True,
-        include_top: bool = True,
-        pooling: typing.Optional[str] = None,
-        pos_dropout_rate: float = 0.0,
-        dropout_rate: float = 0.1,
-        classes: int = 1000,
-        classifier_activation: str = "softmax",
-        weights: typing.Optional[str] = "imagenet",
-        name: str = "VisionTransformerBase32",
-        **kwargs,
-    ):
-        kwargs = self.fix_config(kwargs)
-        super().__init__(
-            32,
-            768,
-            12,
-            12,
-            mlp_ratio,
-            use_qkv_bias,
-            use_qk_norm,
-            pos_dropout_rate,
-            input_tensor=input_tensor,
-            input_shape=input_shape,
-            include_preprocessing=include_preprocessing,
-            include_top=include_top,
-            pooling=pooling,
-            dropout_rate=dropout_rate,
-            classes=classes,
-            classifier_activation=classifier_activation,
-            weights=weights,
-            name=name,
-            **kwargs,
+    # Parameters
+    w0 = 96
+    wa = 38.65
+    wm = 2.43
+    group_size = 40
+    depth = 23
+    se_ratio = 0.0
+
+
+@kimm_export(parent_path=["kimm.models", "kimm.models.regnet"])
+class RegNetY040(RegNetVariant):
+    available_weights = [
+        (
+            "imagenet",
+            RegNet.default_origin,
+            "regnety040_regnety_040.ra3_in1k.keras",
         )
+    ]
 
+    # Parameters
+    w0 = 96
+    wa = 31.41
+    wm = 2.24
+    group_size = 64
+    depth = 22
+    se_ratio = 0.25
 
-class VisionTransformerLarge16(VisionTransformer):
-    available_feature_keys = [
-        "EMBEDDING",
-        *[f"BLOCK{i}" for i in range(24)],
+
+@kimm_export(parent_path=["kimm.models", "kimm.models.regnet"])
+class RegNetX064(RegNetVariant):
+    available_weights = [
+        (
+            "imagenet",
+            RegNet.default_origin,
+            "regnetx064_regnetx_064.pycls_in1k.keras",
+        )
     ]
-    available_weights = []
 
-    def __init__(
-        self,
-        mlp_ratio: float = 4.0,
-        use_qkv_bias: bool = True,
-        use_qk_norm: bool = False,
-        input_tensor: keras.KerasTensor = None,
-        input_shape: typing.Optional[typing.Sequence[int]] = None,
-        include_preprocessing: bool = True,
-        include_top: bool = True,
-        pooling: typing.Optional[str] = None,
-        pos_dropout_rate: float = 0.0,
-        dropout_rate: float = 0.1,
-        classes: int = 1000,
-        classifier_activation: str = "softmax",
-        weights: typing.Optional[str] = None,
-        name: str = "VisionTransformerLarge16",
-        **kwargs,
-    ):
-        kwargs = self.fix_config(kwargs)
-        super().__init__(
-            16,
-            1024,
-            24,
-            16,
-            mlp_ratio,
-            use_qkv_bias,
-            use_qk_norm,
-            pos_dropout_rate,
-            input_tensor=input_tensor,
-            input_shape=input_shape,
-            include_preprocessing=include_preprocessing,
-            include_top=include_top,
-            pooling=pooling,
-            dropout_rate=dropout_rate,
-            classes=classes,
-            classifier_activation=classifier_activation,
-            weights=weights,
-            name=name,
-            **kwargs,
+    # Parameters
+    w0 = 184
+    wa = 60.83
+    wm = 2.07
+    group_size = 56
+    depth = 17
+    se_ratio = 0.0
+
+
+@kimm_export(parent_path=["kimm.models", "kimm.models.regnet"])
+class RegNetY064(RegNetVariant):
+    available_weights = [
+        (
+            "imagenet",
+            RegNet.default_origin,
+            "regnety064_regnety_064.ra3_in1k.keras",
         )
+    ]
 
+    # Parameters
+    w0 = 112
+    wa = 33.22
+    wm = 2.27
+    group_size = 72
+    depth = 25
+    se_ratio = 0.25
 
-class VisionTransformerLarge32(VisionTransformer):
-    available_feature_keys = [
-        "EMBEDDING",
-        *[f"BLOCK{i}" for i in range(24)],
+
+@kimm_export(parent_path=["kimm.models", "kimm.models.regnet"])
+class RegNetX080(RegNetVariant):
+    available_weights = [
+        (
+            "imagenet",
+            RegNet.default_origin,
+            "regnetx080_regnetx_080.tv2_in1k.keras",
+        )
     ]
-    available_weights = []
 
-    def __init__(
-        self,
-        mlp_ratio: float = 4.0,
-        use_qkv_bias: bool = True,
-        use_qk_norm: bool = False,
-        input_tensor: keras.KerasTensor = None,
-        input_shape: typing.Optional[typing.Sequence[int]] = None,
-        include_preprocessing: bool = True,
-        include_top: bool = True,
-        pooling: typing.Optional[str] = None,
-        pos_dropout_rate: float = 0.0,
-        dropout_rate: float = 0.1,
-        classes: int = 1000,
-        classifier_activation: str = "softmax",
-        weights: typing.Optional[str] = None,
-        name: str = "VisionTransformerLarge32",
-        **kwargs,
-    ):
-        kwargs = self.fix_config(kwargs)
-        super().__init__(
-            32,
-            1024,
-            24,
-            16,
-            mlp_ratio,
-            use_qkv_bias,
-            use_qk_norm,
-            pos_dropout_rate,
-            input_tensor=input_tensor,
-            input_shape=input_shape,
-            include_preprocessing=include_preprocessing,
-            include_top=include_top,
-            pooling=pooling,
-            dropout_rate=dropout_rate,
-            classes=classes,
-            classifier_activation=classifier_activation,
-            weights=weights,
-            name=name,
-            **kwargs,
+    # Parameters
+    w0 = 80
+    wa = 49.56
+    wm = 2.88
+    group_size = 120
+    depth = 23
+    se_ratio = 0.0
+
+
+@kimm_export(parent_path=["kimm.models", "kimm.models.regnet"])
+class RegNetY080(RegNetVariant):
+    available_weights = [
+        (
+            "imagenet",
+            RegNet.default_origin,
+            "regnety080_regnety_080.ra3_in1k.keras",
+        )
+    ]
+
+    # Parameters
+    w0 = 192
+    wa = 76.82
+    wm = 2.19
+    group_size = 56
+    depth = 17
+    se_ratio = 0.25
+
+
+@kimm_export(parent_path=["kimm.models", "kimm.models.regnet"])
+class RegNetX120(RegNetVariant):
+    available_weights = [
+        (
+            "imagenet",
+            RegNet.default_origin,
+            "regnetx120_regnetx_120.pycls_in1k.keras",
         )
+    ]
+
+    # Parameters
+    w0 = 168
+    wa = 73.36
+    wm = 2.37
+    group_size = 112
+    depth = 19
+    se_ratio = 0.0
+
+
+@kimm_export(parent_path=["kimm.models", "kimm.models.regnet"])
+class RegNetY120(RegNetVariant):
+    available_weights = [
+        (
+            "imagenet",
+            RegNet.default_origin,
+            "regnety120_regnety_120.sw_in12k_ft_in1k.keras",
+        )
+    ]
+
+    # Parameters
+    w0 = 168
+    wa = 73.36
+    wm = 2.37
+    group_size = 112
+    depth = 19
+    se_ratio = 0.25
+
+
+@kimm_export(parent_path=["kimm.models", "kimm.models.regnet"])
+class RegNetX160(RegNetVariant):
+    available_weights = [
+        (
+            "imagenet",
+            RegNet.default_origin,
+            "regnetx160_regnetx_160.tv2_in1k.keras",
+        )
+    ]
+
+    # Parameters
+    w0 = 216
+    wa = 55.59
+    wm = 2.1
+    group_size = 128
+    depth = 22
+    se_ratio = 0.0
+
+
+@kimm_export(parent_path=["kimm.models", "kimm.models.regnet"])
+class RegNetY160(RegNetVariant):
+    available_weights = [
+        (
+            "imagenet",
+            RegNet.default_origin,
+            "regnety160_regnety_160.swag_ft_in1k.keras",
+        )
+    ]
+
+    # Parameters
+    w0 = 200
+    wa = 106.23
+    wm = 2.48
+    group_size = 112
+    depth = 18
+    se_ratio = 0.25
+
+
+@kimm_export(parent_path=["kimm.models", "kimm.models.regnet"])
+class RegNetX320(RegNetVariant):
+    available_weights = [
+        (
+            "imagenet",
+            RegNet.default_origin,
+            "regnetx320_regnetx_320.tv2_in1k.keras",
+        )
+    ]
+
+    # Parameters
+    w0 = 320
+    wa = 69.86
+    wm = 2.0
+    group_size = 168
+    depth = 23
+    se_ratio = 0.0
+
 
+@kimm_export(parent_path=["kimm.models", "kimm.models.regnet"])
+class RegNetY320(RegNetVariant):
+    available_weights = [
+        (
+            "imagenet",
+            RegNet.default_origin,
+            "regnety320_regnety_320.swag_ft_in1k.keras",
+        )
+    ]
 
-add_model_to_registry(VisionTransformerTiny16, "imagenet")
-add_model_to_registry(VisionTransformerTiny32)
-add_model_to_registry(VisionTransformerSmall16, "imagenet")
-add_model_to_registry(VisionTransformerSmall32, "imagenet")
-add_model_to_registry(VisionTransformerBase16, "imagenet")
-add_model_to_registry(VisionTransformerBase32, "imagenet")
-add_model_to_registry(VisionTransformerLarge16)
-add_model_to_registry(VisionTransformerLarge32)
+    # Parameters
+    w0 = 232
+    wa = 115.89
+    wm = 2.53
+    group_size = 232
+    depth = 20
+    se_ratio = 0.25
+
+
+add_model_to_registry(RegNetX002, "imagenet")
+add_model_to_registry(RegNetY002, "imagenet")
+add_model_to_registry(RegNetX004, "imagenet")
+add_model_to_registry(RegNetY004, "imagenet")
+add_model_to_registry(RegNetX006, "imagenet")
+add_model_to_registry(RegNetY006, "imagenet")
+add_model_to_registry(RegNetX008, "imagenet")
+add_model_to_registry(RegNetY008, "imagenet")
+add_model_to_registry(RegNetX016, "imagenet")
+add_model_to_registry(RegNetY016, "imagenet")
+add_model_to_registry(RegNetX032, "imagenet")
+add_model_to_registry(RegNetY032, "imagenet")
+add_model_to_registry(RegNetX040, "imagenet")
+add_model_to_registry(RegNetY040, "imagenet")
+add_model_to_registry(RegNetX064, "imagenet")
+add_model_to_registry(RegNetY064, "imagenet")
+add_model_to_registry(RegNetX080, "imagenet")
+add_model_to_registry(RegNetY080, "imagenet")
+add_model_to_registry(RegNetX120, "imagenet")
+add_model_to_registry(RegNetY120, "imagenet")
+add_model_to_registry(RegNetX160, "imagenet")
+add_model_to_registry(RegNetY160, "imagenet")
+add_model_to_registry(RegNetX320, "imagenet")
+add_model_to_registry(RegNetY320, "imagenet")
```

### Comparing `kimm-0.1.8/kimm/models/xception.py` & `kimm-0.2.0/kimm/_src/models/xception.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import typing
 
 import keras
 from keras import backend
 from keras import layers
 
-from kimm.models import BaseModel
-from kimm.utils import add_model_to_registry
+from kimm._src.kimm_export import kimm_export
+from kimm._src.models.base_model import BaseModel
+from kimm._src.utils.model_registry import add_model_to_registry
 
 
 def apply_xception_block(
     inputs,
     depth: int,
     output_channels: int,
     strides: int = 1,
@@ -150,19 +151,18 @@
     def get_config(self):
         return super().get_config()
 
     def fix_config(self, config: typing.Dict):
         return config
 
 
-"""
-Model Definition
-"""
+# Model Definition
 
 
+@kimm_export(parent_path=["kimm.models", "kimm.models.xception"])
 class Xception(XceptionBase):
     available_weights = [
         (
             "imagenet",
             XceptionBase.default_origin,
             "xception.keras",
         )
```

### Comparing `kimm-0.1.8/kimm/utils/model_registry.py` & `kimm-0.2.0/kimm/_src/utils/model_registry.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 import sys
 import typing
 import warnings
 
+from kimm._src.kimm_export import kimm_export
+
 # {
 #     "name",  # str
 #     "feature_extractor",  # bool
 #     "feature_keys",  # list of str
 #     "weights",  # None or str
 # }
 MODEL_REGISTRY: typing.List[typing.Dict[str, typing.Union[str, bool]]] = []
@@ -29,25 +31,25 @@
 
 
 def clear_registry():
     MODEL_REGISTRY.clear()
 
 
 def add_model_to_registry(model_cls, weights: typing.Optional[str] = None):
-    from kimm.models.base_model import BaseModel
+    from kimm._src.models.base_model import BaseModel
 
-    # deal with __all__
+    # Deal with __all__
     mod = sys.modules[model_cls.__module__]
     model_name = model_cls.__name__
     if hasattr(mod, "__all__"):
         mod.__all__.append(model_name)
     else:
         mod.__all__ = [model_name]
 
-    # add model information
+    # Add model information
     feature_extractor = False
     feature_keys = []
     if issubclass(model_cls, BaseModel):
         feature_extractor = True
         feature_keys = model_cls.available_feature_keys
     for info in MODEL_REGISTRY:
         if info["name"] == model_cls.__name__:
@@ -67,40 +69,40 @@
             "feature_extractor": feature_extractor,
             "feature_keys": feature_keys,
             "weights": weights,
         }
     )
 
 
+@kimm_export(parent_path=["kimm", "kimm.utils"])
 def list_models(
     name: typing.Optional[str] = None,
     feature_extractor: typing.Optional[bool] = None,
     weights: typing.Optional[typing.Union[bool, str]] = None,
-):
+) -> typing.List[str]:
     result_names: typing.Set = set()
     for info in MODEL_REGISTRY:
-        # add by default
+        # Add by default
         result_names.add(info["name"])
         need_remove = False
 
-        # match string (simple implementation)
+        # Match string (simple implementation)
         if name is not None:
             need_remove = not _match_string(name, info["name"])
 
-        # filter by feature_extractor and weights
+        # Filter by feature_extractor and weights
         if (
             feature_extractor is not None
             and info["feature_extractor"] is not feature_extractor
         ):
             need_remove = True
         if weights is not None and info["weights"] != weights:
             if weights is True and info["weights"] is None:
                 need_remove = True
             elif weights is False and info["weights"] is not None:
                 need_remove = True
             elif isinstance(weights, str):
                 if weights.lower() != info["weights"]:
                     need_remove = True
-
         if need_remove:
             result_names.remove(info["name"])
     return sorted(result_names)
```

### Comparing `kimm-0.1.8/kimm/utils/model_registry_test.py` & `kimm-0.2.0/kimm/_src/utils/model_registry_test.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from keras import models
 from keras.src import testing
 
-from kimm.models.base_model import BaseModel
-from kimm.utils.model_registry import MODEL_REGISTRY
-from kimm.utils.model_registry import add_model_to_registry
-from kimm.utils.model_registry import clear_registry
-from kimm.utils.model_registry import list_models
+from kimm._src.models.base_model import BaseModel
+from kimm._src.utils.model_registry import MODEL_REGISTRY
+from kimm._src.utils.model_registry import add_model_to_registry
+from kimm._src.utils.model_registry import clear_registry
+from kimm._src.utils.model_registry import list_models
 
 
 class DummyModel(models.Model):
     pass
 
 
 class DummyFeatureExtractor(BaseModel):
```

### Comparing `kimm-0.1.8/kimm/utils/model_utils.py` & `kimm-0.2.0/kimm/_src/utils/model_utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,12 @@
-from kimm.models.base_model import BaseModel
+from kimm._src.kimm_export import kimm_export
+from kimm._src.models.base_model import BaseModel
 
 
+@kimm_export(parent_path=["kimm.utils"])
 def get_reparameterized_model(model: BaseModel):
     if not hasattr(model, "get_reparameterized_model"):
         raise ValueError(
             "There is no 'get_reparameterized_model' method in the model. "
             f"Received: model type={type(model)}"
         )
```

### Comparing `kimm-0.1.8/kimm/utils/model_utils_test.py` & `kimm-0.2.0/kimm/_src/utils/model_utils_test.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from keras import random
 from keras.src import testing
 
-from kimm.models.regnet import RegNetX002
-from kimm.models.repvgg import RepVGG
-from kimm.utils.model_utils import get_reparameterized_model
+from kimm._src.models.regnet import RegNetX002
+from kimm._src.models.repvgg import RepVGG
+from kimm._src.utils.model_utils import get_reparameterized_model
 
 
 class ModelUtilsTest(testing.TestCase):
     def test_get_reparameterized_model(self):
         # dummy RepVGG with random initialization
         model = RepVGG(
             [1, 1, 1, 1],
```

### Comparing `kimm-0.1.8/kimm/utils/timm_utils.py` & `kimm-0.2.0/kimm/_src/utils/timm_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import typing
 
 import keras
 import numpy as np
 
+from kimm._src.kimm_export import kimm_export
+
 
 def _is_useless_weights(name: str):
     if "num_batches_tracked" in name:
         return True
     else:
         return False
 
@@ -14,14 +16,15 @@
 def _is_non_trainable_weights(name: str):
     if "running_mean" in name or "running_var" in name:
         return True
     else:
         return False
 
 
+@kimm_export(parent_path=["kimm.timm_utils"])
 def separate_torch_state_dict(state_dict: typing.OrderedDict):
     trainable_state_dict = state_dict.copy()
     non_trainable_state_dict = state_dict.copy()
     trainable_remove_keys = []
     non_trainable_remove_keys = []
     for k in state_dict.keys():
         if _is_useless_weights(k):
@@ -35,14 +38,15 @@
     for k in trainable_remove_keys:
         trainable_state_dict.pop(k)
     for k in non_trainable_remove_keys:
         non_trainable_state_dict.pop(k)
     return trainable_state_dict, non_trainable_state_dict
 
 
+@kimm_export(parent_path=["kimm.timm_utils"])
 def separate_keras_weights(keras_model: keras.Model):
     trainable_weights = []
     non_trainable_weights = []
     for layer in keras_model.layers:
         if hasattr(layer, "extra_layers"):
             for sub_layer in layer.extra_layers:
                 sub_layer: keras.Layer
@@ -63,14 +67,15 @@
             for weight in layer.non_trainable_weights:
                 non_trainable_weights.append(
                     (weight, layer.name + "_" + weight.name)
                 )
     return trainable_weights, non_trainable_weights
 
 
+@kimm_export(parent_path=["kimm.timm_utils"])
 def assign_weights(
     keras_name: str, keras_weight: keras.Variable, torch_weight: np.ndarray
 ):
     if len(keras_weight.shape) == 4:
         if (
             "conv" in keras_name
             or "pointwise" in keras_name
@@ -103,14 +108,15 @@
         raise ValueError(
             f"Failed to assign {keras_name}, "
             f"keras_weight.shape={keras_weight.shape}, "
             f"torch_weight.shape={torch_weight.shape}, "
         )
 
 
+@kimm_export(parent_path=["kimm.timm_utils"])
 def is_same_weights(
     keras_name: str,
     keras_weights: keras.Variable,
     torch_name: str,
     torch_weights: np.ndarray,
 ):
     if np.sum(keras_weights.shape) != np.sum(torch_weights.shape):
```

### Comparing `kimm-0.1.8/kimm.egg-info/PKG-INFO` & `kimm-0.2.0/kimm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kimm
-Version: 0.1.8
+Version: 0.2.0
 Summary: A Keras model zoo with pretrained weights.
 Author-email: Hong-Yu Chiu <james77777778@gmail.com>
 Maintainer-email: Hong-Yu Chiu <james77777778@gmail.com>
 License: Apache License 2.0
 Project-URL: Homepage, https://github.com/james77777778/keras-image-models
 Project-URL: Documentation, https://github.com/james77777778/keras-image-models
 Project-URL: Repository, https://github.com/james77777778/keras-image-models.git
@@ -33,25 +33,27 @@
 Requires-Dist: onnxsim; extra == "tests"
 Requires-Dist: isort; extra == "tests"
 Requires-Dist: ruff; extra == "tests"
 Requires-Dist: black; extra == "tests"
 Requires-Dist: pytest; extra == "tests"
 Requires-Dist: pytest-cov; extra == "tests"
 Requires-Dist: coverage; extra == "tests"
+Requires-Dist: pre-commit; extra == "tests"
+Requires-Dist: namex; extra == "tests"
 Provides-Extra: examples
 Requires-Dist: opencv-python; extra == "examples"
 Requires-Dist: matplotlib; extra == "examples"
 
 <!-- markdownlint-disable MD033 -->
 <!-- markdownlint-disable MD041 -->
 
 <div align="center">
 <img width="50%" src="https://github.com/james77777778/kimm/assets/20734616/b21db8f2-307b-4791-b93d-e913e45fb238" alt="KIMM">
 
-[![Keras](https://img.shields.io/badge/keras-v3.0.4+-success.svg)](https://github.com/keras-team/keras)
+[![Keras](https://img.shields.io/badge/keras-v3.3.0+-success.svg)](https://github.com/keras-team/keras)
 [![PyPI](https://img.shields.io/pypi/v/kimm)](https://pypi.org/project/kimm/)
 [![Contributions Welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat)](https://github.com/james77777778/kimm/issues)
 [![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/james77777778/keras-image-models/actions.yml?label=tests)](https://github.com/james77777778/keras-image-models/actions/workflows/actions.yml?query=branch%3Amain++)
 [![codecov](https://codecov.io/gh/james77777778/keras-image-models/graph/badge.svg?token=eEha1SR80D)](https://codecov.io/gh/james77777778/keras-image-models)
 </div>
 
 # Keras Image Models
```

### Comparing `kimm-0.1.8/pyproject.toml` & `kimm-0.2.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -54,14 +54,17 @@
     # linter and formatter
     "isort",
     "ruff",
     "black",
     "pytest",
     "pytest-cov",
     "coverage",
+    # tool
+    "pre-commit",
+    "namex",
 ]
 examples = ["opencv-python", "matplotlib"]
 
 [tool.setuptools.packages]
 find = { include = ["kimm*"] }
 
 [tool.setuptools.dynamic]
@@ -80,38 +83,38 @@
     ".github",
     ".devcontainer",
     "venv",
     "__pycache__",
 ]
 
 [tool.ruff.lint.per-file-ignores]
-"./examples/**/*" = ["E402"]
 "**/__init__.py" = ["F401"]
 
 [tool.isort]
 profile = "black"
 force_single_line = true
 known_first_party = ["kimm"]
 line_length = 80
 
 [tool.pytest.ini_options]
-addopts = "--durations 10 --cov --cov-report html --cov-report term:skip-covered --cov-report xml"
+addopts = "-vv --durations 10 --cov --cov-report html --cov-report term:skip-covered --cov-report xml"
 testpaths = ["kimm"]
 filterwarnings = [
     "error",
+    "ignore::UserWarning",
     "ignore::DeprecationWarning",
     "ignore::ImportWarning",
     "ignore::RuntimeWarning",
     "ignore::PendingDeprecationWarning",
     "ignore::FutureWarning",
 ]
 
 [tool.coverage.run]
 source = ["kimm"]
-omit = ["**/__init__.py", "*test*", "kimm/utils/timm_utils.py"]
+omit = ["**/__init__.py", "*test*"]
 
 [tool.coverage.report]
 exclude_lines = [
     "pragma: no cover",
     "@abstract",
     "raise NotImplementedError",
     "raise ValueError",
```

