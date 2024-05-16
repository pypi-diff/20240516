# Comparing `tmp/peft-0.8.2.tar.gz` & `tmp/peft-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "peft-0.8.2.tar", last modified: Thu Feb  1 14:16:39 2024, max compression
+gzip compressed data, was "peft-0.9.0.tar", last modified: Wed Feb 28 10:25:12 2024, max compression
```

## Comparing `peft-0.8.2.tar` & `peft-0.9.0.tar`

### file list

```diff
@@ -1,119 +1,128 @@
-drwxr-xr-x   0 sourabmangrulkar   (501) staff       (20)        0 2024-02-01 14:16:39.119022 peft-0.8.2/
--rw-r--r--   0 sourabmangrulkar   (501) staff       (20)    11357 2023-11-17 11:44:45.000000 peft-0.8.2/LICENSE
--rw-r--r--   0 sourabmangrulkar   (501) staff       (20)    24172 2024-02-01 14:16:39.118586 peft-0.8.2/PKG-INFO
--rw-r--r--   0 sourabmangrulkar   (501) staff       (20)    23249 2023-12-06 12:36:52.000000 peft-0.8.2/README.md
--rw-r--r--   0 sourabmangrulkar   (501) staff       (20)      986 2023-12-14 12:07:04.000000 peft-0.8.2/pyproject.toml
--rw-r--r--   0 sourabmangrulkar   (501) staff       (20)       38 2024-02-01 14:16:39.119110 peft-0.8.2/setup.cfg
--rw-r--r--   0 sourabmangrulkar   (501) staff       (20)     3961 2024-02-01 14:13:54.000000 peft-0.8.2/setup.py
-drwxr-xr-x   0 sourabmangrulkar   (501) staff       (20)        0 2024-02-01 14:16:39.056661 peft-0.8.2/src/
-drwxr-xr-x   0 sourabmangrulkar   (501) staff       (20)        0 2024-02-01 14:16:39.062154 peft-0.8.2/src/peft/
--rw-r--r--   0 sourabmangrulkar   (501) staff       (20)     2518 2024-02-01 14:13:54.000000 peft-0.8.2/src/peft/__init__.py
--rw-r--r--   0 sourabmangrulkar   (501) staff       (20)     6451 2024-02-01 11:56:41.000000 peft-0.8.2/src/peft/auto.py
--rw-r--r--   0 sourabmangrulkar   (501) staff       (20)    10928 2024-02-01 11:56:41.000000 peft-0.8.2/src/peft/config.py
--rw-r--r--   0 sourabmangrulkar   (501) staff       (20)     4423 2023-11-17 11:44:45.000000 peft-0.8.2/src/peft/helpers.py
--rw-r--r--   0 sourabmangrulkar   (501) staff       (20)     2230 2023-11-17 11:44:45.000000 peft-0.8.2/src/peft/import_utils.py
--rw-r--r--   0 sourabmangrulkar   (501) staff       (20)     5937 2024-01-17 14:01:31.000000 peft-0.8.2/src/peft/mapping.py
--rw-r--r--   0 sourabmangrulkar   (501) staff       (20)    16485 2024-02-01 11:56:41.000000 peft-0.8.2/src/peft/mixed_model.py
--rw-r--r--   0 sourabmangrulkar   (501) staff       (20)    84805 2024-02-01 13:06:41.000000 peft-0.8.2/src/peft/peft_model.py
--rw-r--r--   0 sourabmangrulkar   (501) staff       (20)        0 2023-11-17 11:44:45.000000 peft-0.8.2/src/peft/py.typed
-drwxr-xr-x   0 sourabmangrulkar   (501) staff       (20)        0 2024-02-01 14:16:39.063432 peft-0.8.2/src/peft/tuners/
--rw-r--r--   0 sourabmangrulkar   (501) staff       (20)     1535 2024-01-17 14:01:31.000000 peft-0.8.2/src/peft/tuners/__init__.py
-drwxr-xr-x   0 sourabmangrulkar   (501) staff       (20)        0 2024-02-01 14:16:39.073514 peft-0.8.2/src/peft/tuners/adalora/
--rw-r--r--   0 sourabmangrulkar   (501) staff       (20)     1313 2023-12-14 12:07:04.000000 peft-0.8.2/src/peft/tuners/adalora/__init__.py
--rw-r--r--   0 sourabmangrulkar   (501) staff       (20)     5621 2024-01-17 14:01:31.000000 peft-0.8.2/src/peft/tuners/adalora/bnb.py
--rw-r--r--   0 sourabmangrulkar   (501) staff       (20)     2673 2023-11-17 11:44:45.000000 peft-0.8.2/src/peft/tuners/adalora/config.py
--rw-r--r--   0 sourabmangrulkar   (501) staff       (20)     2734 2024-01-17 14:01:31.000000 peft-0.8.2/src/peft/tuners/adalora/gptq.py
--rw-r--r--   0 sourabmangrulkar   (501) staff       (20)    14355 2024-02-01 13:06:41.000000 peft-0.8.2/src/peft/tuners/adalora/layer.py
--rw-r--r--   0 sourabmangrulkar   (501) staff       (20)    15303 2024-01-17 14:01:31.000000 peft-0.8.2/src/peft/tuners/adalora/model.py
-drwxr-xr-x   0 sourabmangrulkar   (501) staff       (20)        0 2024-02-01 14:16:39.076281 peft-0.8.2/src/peft/tuners/adaption_prompt/
--rw-r--r--   0 sourabmangrulkar   (501) staff       (20)      809 2023-11-17 11:44:45.000000 peft-0.8.2/src/peft/tuners/adaption_prompt/__init__.py
--rw-r--r--   0 sourabmangrulkar   (501) staff       (20)     2575 2023-11-17 11:44:45.000000 peft-0.8.2/src/peft/tuners/adaption_prompt/config.py
--rw-r--r--   0 sourabmangrulkar   (501) staff       (20)     5293 2023-11-17 11:44:45.000000 peft-0.8.2/src/peft/tuners/adaption_prompt/layer.py
--rw-r--r--   0 sourabmangrulkar   (501) staff       (20)     7479 2023-12-14 12:07:04.000000 peft-0.8.2/src/peft/tuners/adaption_prompt/model.py
--rw-r--r--   0 sourabmangrulkar   (501) staff       (20)     4100 2023-12-14 12:07:04.000000 peft-0.8.2/src/peft/tuners/adaption_prompt/utils.py
-drwxr-xr-x   0 sourabmangrulkar   (501) staff       (20)        0 2024-02-01 14:16:39.077947 peft-0.8.2/src/peft/tuners/ia3/
--rw-r--r--   0 sourabmangrulkar   (501) staff       (20)     1200 2023-12-14 12:07:04.000000 peft-0.8.2/src/peft/tuners/ia3/__init__.py
--rw-r--r--   0 sourabmangrulkar   (501) staff       (20)     4683 2024-01-17 14:01:31.000000 peft-0.8.2/src/peft/tuners/ia3/bnb.py
--rw-r--r--   0 sourabmangrulkar   (501) staff       (20)     5166 2024-01-17 14:01:31.000000 peft-0.8.2/src/peft/tuners/ia3/config.py
--rw-r--r--   0 sourabmangrulkar   (501) staff       (20)    13676 2024-02-01 13:06:41.000000 peft-0.8.2/src/peft/tuners/ia3/layer.py
--rw-r--r--   0 sourabmangrulkar   (501) staff       (20)    15901 2024-01-10 07:55:52.000000 peft-0.8.2/src/peft/tuners/ia3/model.py
-drwxr-xr-x   0 sourabmangrulkar   (501) staff       (20)        0 2024-02-01 14:16:39.079171 peft-0.8.2/src/peft/tuners/loha/
--rw-r--r--   0 sourabmangrulkar   (501) staff       (20)      792 2023-11-17 11:44:45.000000 peft-0.8.2/src/peft/tuners/loha/__init__.py
--rw-r--r--   0 sourabmangrulkar   (501) staff       (20)     6052 2024-01-17 14:01:31.000000 peft-0.8.2/src/peft/tuners/loha/config.py
--rw-r--r--   0 sourabmangrulkar   (501) staff       (20)    15621 2023-12-26 13:10:17.000000 peft-0.8.2/src/peft/tuners/loha/layer.py
--rw-r--r--   0 sourabmangrulkar   (501) staff       (20)     4219 2024-01-10 07:55:52.000000 peft-0.8.2/src/peft/tuners/loha/model.py
-drwxr-xr-x   0 sourabmangrulkar   (501) staff       (20)        0 2024-02-01 14:16:39.081968 peft-0.8.2/src/peft/tuners/lokr/
--rw-r--r--   0 sourabmangrulkar   (501) staff       (20)      792 2023-11-17 11:44:45.000000 peft-0.8.2/src/peft/tuners/lokr/__init__.py
--rw-r--r--   0 sourabmangrulkar   (501) staff       (20)     6320 2024-01-17 14:01:31.000000 peft-0.8.2/src/peft/tuners/lokr/config.py
--rw-r--r--   0 sourabmangrulkar   (501) staff       (20)    15484 2023-12-26 13:10:17.000000 peft-0.8.2/src/peft/tuners/lokr/layer.py
--rw-r--r--   0 sourabmangrulkar   (501) staff       (20)     4273 2024-01-10 07:55:52.000000 peft-0.8.2/src/peft/tuners/lokr/model.py
-drwxr-xr-x   0 sourabmangrulkar   (501) staff       (20)        0 2024-02-01 14:16:39.084471 peft-0.8.2/src/peft/tuners/lora/
--rw-r--r--   0 sourabmangrulkar   (501) staff       (20)     1303 2023-12-14 12:07:04.000000 peft-0.8.2/src/peft/tuners/lora/__init__.py
--rw-r--r--   0 sourabmangrulkar   (501) staff       (20)    15922 2024-02-01 13:06:41.000000 peft-0.8.2/src/peft/tuners/lora/bnb.py
--rw-r--r--   0 sourabmangrulkar   (501) staff       (20)    13898 2024-01-17 14:01:31.000000 peft-0.8.2/src/peft/tuners/lora/config.py
--rw-r--r--   0 sourabmangrulkar   (501) staff       (20)     3654 2024-01-17 14:01:31.000000 peft-0.8.2/src/peft/tuners/lora/gptq.py
--rw-r--r--   0 sourabmangrulkar   (501) staff       (20)    30087 2024-02-01 13:06:41.000000 peft-0.8.2/src/peft/tuners/lora/layer.py
--rw-r--r--   0 sourabmangrulkar   (501) staff       (20)    27043 2024-02-01 13:05:49.000000 peft-0.8.2/src/peft/tuners/lora/model.py
--rw-r--r--   0 sourabmangrulkar   (501) staff       (20)     8527 2024-01-10 07:55:52.000000 peft-0.8.2/src/peft/tuners/lora/tp_layer.py
--rw-r--r--   0 sourabmangrulkar   (501) staff       (20)    15943 2024-02-01 13:06:41.000000 peft-0.8.2/src/peft/tuners/lycoris_utils.py
-drwxr-xr-x   0 sourabmangrulkar   (501) staff       (20)        0 2024-02-01 14:16:39.085145 peft-0.8.2/src/peft/tuners/mixed/
--rw-r--r--   0 sourabmangrulkar   (501) staff       (20)      721 2023-12-06 12:36:52.000000 peft-0.8.2/src/peft/tuners/mixed/__init__.py
--rw-r--r--   0 sourabmangrulkar   (501) staff       (20)    14677 2024-02-01 11:56:41.000000 peft-0.8.2/src/peft/tuners/mixed/model.py
-drwxr-xr-x   0 sourabmangrulkar   (501) staff       (20)        0 2024-02-01 14:16:39.085989 peft-0.8.2/src/peft/tuners/multitask_prompt_tuning/
--rw-r--r--   0 sourabmangrulkar   (501) staff       (20)      834 2023-11-17 11:44:45.000000 peft-0.8.2/src/peft/tuners/multitask_prompt_tuning/__init__.py
--rw-r--r--   0 sourabmangrulkar   (501) staff       (20)     2461 2023-11-17 11:44:45.000000 peft-0.8.2/src/peft/tuners/multitask_prompt_tuning/config.py
--rw-r--r--   0 sourabmangrulkar   (501) staff       (20)     4605 2023-11-17 11:44:45.000000 peft-0.8.2/src/peft/tuners/multitask_prompt_tuning/model.py
-drwxr-xr-x   0 sourabmangrulkar   (501) staff       (20)        0 2024-02-01 14:16:39.087616 peft-0.8.2/src/peft/tuners/oft/
--rw-r--r--   0 sourabmangrulkar   (501) staff       (20)      786 2023-12-06 12:36:52.000000 peft-0.8.2/src/peft/tuners/oft/__init__.py
--rw-r--r--   0 sourabmangrulkar   (501) staff       (20)     5843 2024-01-17 14:01:31.000000 peft-0.8.2/src/peft/tuners/oft/config.py
--rw-r--r--   0 sourabmangrulkar   (501) staff       (20)    15579 2024-02-01 13:06:41.000000 peft-0.8.2/src/peft/tuners/oft/layer.py
--rw-r--r--   0 sourabmangrulkar   (501) staff       (20)     3709 2024-01-10 07:55:52.000000 peft-0.8.2/src/peft/tuners/oft/model.py
-drwxr-xr-x   0 sourabmangrulkar   (501) staff       (20)        0 2024-02-01 14:16:39.088050 peft-0.8.2/src/peft/tuners/p_tuning/
--rw-r--r--   0 sourabmangrulkar   (501) staff       (20)      816 2023-11-17 11:44:45.000000 peft-0.8.2/src/peft/tuners/p_tuning/__init__.py
--rw-r--r--   0 sourabmangrulkar   (501) staff       (20)     2125 2023-11-17 11:44:45.000000 peft-0.8.2/src/peft/tuners/p_tuning/config.py
--rw-r--r--   0 sourabmangrulkar   (501) staff       (20)     5590 2023-12-06 12:36:52.000000 peft-0.8.2/src/peft/tuners/p_tuning/model.py
-drwxr-xr-x   0 sourabmangrulkar   (501) staff       (20)        0 2024-02-01 14:16:39.089212 peft-0.8.2/src/peft/tuners/poly/
--rw-r--r--   0 sourabmangrulkar   (501) staff       (20)      774 2024-01-17 14:01:31.000000 peft-0.8.2/src/peft/tuners/poly/__init__.py
--rw-r--r--   0 sourabmangrulkar   (501) staff       (20)     3798 2024-01-17 14:01:31.000000 peft-0.8.2/src/peft/tuners/poly/config.py
--rw-r--r--   0 sourabmangrulkar   (501) staff       (20)     6905 2024-01-17 14:01:31.000000 peft-0.8.2/src/peft/tuners/poly/layer.py
--rw-r--r--   0 sourabmangrulkar   (501) staff       (20)     6797 2024-01-17 14:01:31.000000 peft-0.8.2/src/peft/tuners/poly/model.py
--rw-r--r--   0 sourabmangrulkar   (501) staff       (20)     2815 2024-01-17 14:01:31.000000 peft-0.8.2/src/peft/tuners/poly/router.py
-drwxr-xr-x   0 sourabmangrulkar   (501) staff       (20)        0 2024-02-01 14:16:39.090515 peft-0.8.2/src/peft/tuners/prefix_tuning/
--rw-r--r--   0 sourabmangrulkar   (501) staff       (20)      738 2023-11-17 11:44:45.000000 peft-0.8.2/src/peft/tuners/prefix_tuning/__init__.py
--rw-r--r--   0 sourabmangrulkar   (501) staff       (20)     1401 2023-11-17 11:44:45.000000 peft-0.8.2/src/peft/tuners/prefix_tuning/config.py
--rw-r--r--   0 sourabmangrulkar   (501) staff       (20)     3022 2023-11-17 11:44:45.000000 peft-0.8.2/src/peft/tuners/prefix_tuning/model.py
-drwxr-xr-x   0 sourabmangrulkar   (501) staff       (20)        0 2024-02-01 14:16:39.090948 peft-0.8.2/src/peft/tuners/prompt_tuning/
--rw-r--r--   0 sourabmangrulkar   (501) staff       (20)      780 2023-11-17 11:44:45.000000 peft-0.8.2/src/peft/tuners/prompt_tuning/__init__.py
--rw-r--r--   0 sourabmangrulkar   (501) staff       (20)     2877 2023-12-06 12:36:52.000000 peft-0.8.2/src/peft/tuners/prompt_tuning/config.py
--rw-r--r--   0 sourabmangrulkar   (501) staff       (20)     3638 2024-01-10 07:55:52.000000 peft-0.8.2/src/peft/tuners/prompt_tuning/model.py
--rw-r--r--   0 sourabmangrulkar   (501) staff       (20)    27157 2024-02-01 13:06:41.000000 peft-0.8.2/src/peft/tuners/tuners_utils.py
-drwxr-xr-x   0 sourabmangrulkar   (501) staff       (20)        0 2024-02-01 14:16:39.093871 peft-0.8.2/src/peft/utils/
--rw-r--r--   0 sourabmangrulkar   (501) staff       (20)     1895 2024-01-17 14:01:31.000000 peft-0.8.2/src/peft/utils/__init__.py
--rw-r--r--   0 sourabmangrulkar   (501) staff       (20)     5589 2024-02-01 13:06:41.000000 peft-0.8.2/src/peft/utils/constants.py
--rw-r--r--   0 sourabmangrulkar   (501) staff       (20)     9327 2024-01-10 07:55:52.000000 peft-0.8.2/src/peft/utils/loftq_utils.py
--rw-r--r--   0 sourabmangrulkar   (501) staff       (20)    21339 2024-01-22 13:28:02.000000 peft-0.8.2/src/peft/utils/other.py
--rw-r--r--   0 sourabmangrulkar   (501) staff       (20)     2147 2024-01-17 14:01:31.000000 peft-0.8.2/src/peft/utils/peft_types.py
--rw-r--r--   0 sourabmangrulkar   (501) staff       (20)    14632 2024-02-01 13:06:41.000000 peft-0.8.2/src/peft/utils/save_and_load.py
-drwxr-xr-x   0 sourabmangrulkar   (501) staff       (20)        0 2024-02-01 14:16:39.062912 peft-0.8.2/src/peft.egg-info/
--rw-r--r--   0 sourabmangrulkar   (501) staff       (20)    24172 2024-02-01 14:16:38.000000 peft-0.8.2/src/peft.egg-info/PKG-INFO
--rw-r--r--   0 sourabmangrulkar   (501) staff       (20)     2959 2024-02-01 14:16:39.000000 peft-0.8.2/src/peft.egg-info/SOURCES.txt
--rw-r--r--   0 sourabmangrulkar   (501) staff       (20)        1 2024-02-01 14:16:38.000000 peft-0.8.2/src/peft.egg-info/dependency_links.txt
--rw-r--r--   0 sourabmangrulkar   (501) staff       (20)      417 2024-02-01 14:16:38.000000 peft-0.8.2/src/peft.egg-info/requires.txt
--rw-r--r--   0 sourabmangrulkar   (501) staff       (20)        5 2024-02-01 14:16:38.000000 peft-0.8.2/src/peft.egg-info/top_level.txt
-drwxr-xr-x   0 sourabmangrulkar   (501) staff       (20)        0 2024-02-01 14:16:39.112018 peft-0.8.2/tests/
--rw-r--r--   0 sourabmangrulkar   (501) staff       (20)    20274 2024-02-01 13:06:41.000000 peft-0.8.2/tests/test_adaption_prompt.py
--rw-r--r--   0 sourabmangrulkar   (501) staff       (20)     9325 2024-02-01 11:56:41.000000 peft-0.8.2/tests/test_auto.py
--rw-r--r--   0 sourabmangrulkar   (501) staff       (20)    29290 2023-12-26 13:10:17.000000 peft-0.8.2/tests/test_common_gpu.py
--rw-r--r--   0 sourabmangrulkar   (501) staff       (20)    10439 2024-02-01 11:56:41.000000 peft-0.8.2/tests/test_config.py
--rw-r--r--   0 sourabmangrulkar   (501) staff       (20)    77443 2024-02-01 13:06:41.000000 peft-0.8.2/tests/test_custom_models.py
--rw-r--r--   0 sourabmangrulkar   (501) staff       (20)    14653 2024-02-01 13:06:41.000000 peft-0.8.2/tests/test_decoder_models.py
--rw-r--r--   0 sourabmangrulkar   (501) staff       (20)    10550 2024-02-01 13:06:41.000000 peft-0.8.2/tests/test_encoder_decoder_models.py
--rw-r--r--   0 sourabmangrulkar   (501) staff       (20)     8242 2023-11-17 11:44:45.000000 peft-0.8.2/tests/test_feature_extraction_models.py
--rw-r--r--   0 sourabmangrulkar   (501) staff       (20)    53534 2024-01-17 14:01:31.000000 peft-0.8.2/tests/test_gpu_examples.py
--rw-r--r--   0 sourabmangrulkar   (501) staff       (20)     1353 2023-11-17 11:44:45.000000 peft-0.8.2/tests/test_hub_features.py
--rw-r--r--   0 sourabmangrulkar   (501) staff       (20)     2954 2023-12-14 12:07:04.000000 peft-0.8.2/tests/test_low_level_api.py
--rw-r--r--   0 sourabmangrulkar   (501) staff       (20)    10584 2024-02-01 13:06:41.000000 peft-0.8.2/tests/test_multitask_prompt_tuning.py
--rw-r--r--   0 sourabmangrulkar   (501) staff       (20)     9190 2024-02-01 13:06:41.000000 peft-0.8.2/tests/test_stablediffusion.py
--rw-r--r--   0 sourabmangrulkar   (501) staff       (20)    17596 2024-02-01 13:06:41.000000 peft-0.8.2/tests/test_tuners_utils.py
--rw-r--r--   0 sourabmangrulkar   (501) staff       (20)    49891 2024-02-01 13:06:41.000000 peft-0.8.2/tests/testing_common.py
--rw-r--r--   0 sourabmangrulkar   (501) staff       (20)     3209 2023-12-14 12:07:04.000000 peft-0.8.2/tests/testing_utils.py
+drwxrwxr-x   0 vinh      (1000) vinh      (1000)        0 2024-02-28 10:25:12.979027 peft-0.9.0/
+-rw-rw-r--   0 vinh      (1000) vinh      (1000)    11357 2023-12-13 09:11:27.000000 peft-0.9.0/LICENSE
+-rw-rw-r--   0 vinh      (1000) vinh      (1000)    12093 2024-02-28 10:25:12.979027 peft-0.9.0/PKG-INFO
+-rw-rw-r--   0 vinh      (1000) vinh      (1000)    11190 2024-02-28 10:20:13.000000 peft-0.9.0/README.md
+-rw-rw-r--   0 vinh      (1000) vinh      (1000)     1000 2024-02-28 10:20:13.000000 peft-0.9.0/pyproject.toml
+-rw-rw-r--   0 vinh      (1000) vinh      (1000)       38 2024-02-28 10:25:12.979027 peft-0.9.0/setup.cfg
+-rw-rw-r--   0 vinh      (1000) vinh      (1000)     4150 2024-02-28 10:20:13.000000 peft-0.9.0/setup.py
+drwxrwxr-x   0 vinh      (1000) vinh      (1000)        0 2024-02-28 10:25:12.963027 peft-0.9.0/src/
+drwxrwxr-x   0 vinh      (1000) vinh      (1000)        0 2024-02-28 10:25:12.967027 peft-0.9.0/src/peft/
+-rw-rw-r--   0 vinh      (1000) vinh      (1000)     2518 2024-02-28 10:20:13.000000 peft-0.9.0/src/peft/__init__.py
+-rw-rw-r--   0 vinh      (1000) vinh      (1000)     6568 2024-02-28 10:20:13.000000 peft-0.9.0/src/peft/auto.py
+-rw-rw-r--   0 vinh      (1000) vinh      (1000)    10908 2024-02-28 10:20:13.000000 peft-0.9.0/src/peft/config.py
+-rw-rw-r--   0 vinh      (1000) vinh      (1000)     4423 2023-12-13 09:11:27.000000 peft-0.9.0/src/peft/helpers.py
+-rw-rw-r--   0 vinh      (1000) vinh      (1000)     2382 2024-02-28 10:20:13.000000 peft-0.9.0/src/peft/import_utils.py
+-rw-rw-r--   0 vinh      (1000) vinh      (1000)     5916 2024-02-28 10:20:13.000000 peft-0.9.0/src/peft/mapping.py
+-rw-rw-r--   0 vinh      (1000) vinh      (1000)    15911 2024-02-28 10:20:13.000000 peft-0.9.0/src/peft/mixed_model.py
+-rw-rw-r--   0 vinh      (1000) vinh      (1000)    85718 2024-02-28 10:20:13.000000 peft-0.9.0/src/peft/peft_model.py
+-rw-rw-r--   0 vinh      (1000) vinh      (1000)        0 2023-12-13 09:11:27.000000 peft-0.9.0/src/peft/py.typed
+drwxrwxr-x   0 vinh      (1000) vinh      (1000)        0 2024-02-28 10:25:12.967027 peft-0.9.0/src/peft/tuners/
+-rw-rw-r--   0 vinh      (1000) vinh      (1000)     1535 2024-02-28 10:20:13.000000 peft-0.9.0/src/peft/tuners/__init__.py
+drwxrwxr-x   0 vinh      (1000) vinh      (1000)        0 2024-02-28 10:25:12.967027 peft-0.9.0/src/peft/tuners/adalora/
+-rw-rw-r--   0 vinh      (1000) vinh      (1000)     1298 2024-02-28 10:20:13.000000 peft-0.9.0/src/peft/tuners/adalora/__init__.py
+-rw-rw-r--   0 vinh      (1000) vinh      (1000)     5606 2024-02-28 10:20:13.000000 peft-0.9.0/src/peft/tuners/adalora/bnb.py
+-rw-rw-r--   0 vinh      (1000) vinh      (1000)     2659 2024-02-28 10:20:13.000000 peft-0.9.0/src/peft/tuners/adalora/config.py
+-rw-rw-r--   0 vinh      (1000) vinh      (1000)     2719 2024-02-28 10:20:13.000000 peft-0.9.0/src/peft/tuners/adalora/gptq.py
+-rw-rw-r--   0 vinh      (1000) vinh      (1000)    14292 2024-02-28 10:20:13.000000 peft-0.9.0/src/peft/tuners/adalora/layer.py
+-rw-rw-r--   0 vinh      (1000) vinh      (1000)    15302 2024-02-28 10:20:13.000000 peft-0.9.0/src/peft/tuners/adalora/model.py
+drwxrwxr-x   0 vinh      (1000) vinh      (1000)        0 2024-02-28 10:25:12.971027 peft-0.9.0/src/peft/tuners/adaption_prompt/
+-rw-rw-r--   0 vinh      (1000) vinh      (1000)      794 2024-02-28 10:20:13.000000 peft-0.9.0/src/peft/tuners/adaption_prompt/__init__.py
+-rw-rw-r--   0 vinh      (1000) vinh      (1000)     2560 2024-02-28 10:20:13.000000 peft-0.9.0/src/peft/tuners/adaption_prompt/config.py
+-rw-rw-r--   0 vinh      (1000) vinh      (1000)     5278 2024-02-28 10:20:13.000000 peft-0.9.0/src/peft/tuners/adaption_prompt/layer.py
+-rw-rw-r--   0 vinh      (1000) vinh      (1000)     7464 2024-02-28 10:20:13.000000 peft-0.9.0/src/peft/tuners/adaption_prompt/model.py
+-rw-rw-r--   0 vinh      (1000) vinh      (1000)     5372 2024-02-28 10:20:13.000000 peft-0.9.0/src/peft/tuners/adaption_prompt/utils.py
+drwxrwxr-x   0 vinh      (1000) vinh      (1000)        0 2024-02-28 10:25:12.971027 peft-0.9.0/src/peft/tuners/ia3/
+-rw-rw-r--   0 vinh      (1000) vinh      (1000)     1185 2024-02-28 10:20:13.000000 peft-0.9.0/src/peft/tuners/ia3/__init__.py
+-rw-rw-r--   0 vinh      (1000) vinh      (1000)     4668 2024-02-28 10:20:13.000000 peft-0.9.0/src/peft/tuners/ia3/bnb.py
+-rw-rw-r--   0 vinh      (1000) vinh      (1000)     5152 2024-02-28 10:20:13.000000 peft-0.9.0/src/peft/tuners/ia3/config.py
+-rw-rw-r--   0 vinh      (1000) vinh      (1000)    13661 2024-02-28 10:20:13.000000 peft-0.9.0/src/peft/tuners/ia3/layer.py
+-rw-rw-r--   0 vinh      (1000) vinh      (1000)    16597 2024-02-28 10:20:13.000000 peft-0.9.0/src/peft/tuners/ia3/model.py
+drwxrwxr-x   0 vinh      (1000) vinh      (1000)        0 2024-02-28 10:25:12.971027 peft-0.9.0/src/peft/tuners/loha/
+-rw-rw-r--   0 vinh      (1000) vinh      (1000)      777 2024-02-28 10:20:13.000000 peft-0.9.0/src/peft/tuners/loha/__init__.py
+-rw-rw-r--   0 vinh      (1000) vinh      (1000)     6037 2024-02-28 10:20:13.000000 peft-0.9.0/src/peft/tuners/loha/config.py
+-rw-rw-r--   0 vinh      (1000) vinh      (1000)    15606 2024-02-28 10:20:13.000000 peft-0.9.0/src/peft/tuners/loha/layer.py
+-rw-rw-r--   0 vinh      (1000) vinh      (1000)     4205 2024-02-28 10:20:13.000000 peft-0.9.0/src/peft/tuners/loha/model.py
+drwxrwxr-x   0 vinh      (1000) vinh      (1000)        0 2024-02-28 10:25:12.971027 peft-0.9.0/src/peft/tuners/lokr/
+-rw-rw-r--   0 vinh      (1000) vinh      (1000)      777 2024-02-28 10:20:13.000000 peft-0.9.0/src/peft/tuners/lokr/__init__.py
+-rw-rw-r--   0 vinh      (1000) vinh      (1000)     6305 2024-02-28 10:20:13.000000 peft-0.9.0/src/peft/tuners/lokr/config.py
+-rw-rw-r--   0 vinh      (1000) vinh      (1000)    15469 2024-02-28 10:20:13.000000 peft-0.9.0/src/peft/tuners/lokr/layer.py
+-rw-rw-r--   0 vinh      (1000) vinh      (1000)     4259 2024-02-28 10:20:13.000000 peft-0.9.0/src/peft/tuners/lokr/model.py
+drwxrwxr-x   0 vinh      (1000) vinh      (1000)        0 2024-02-28 10:25:12.971027 peft-0.9.0/src/peft/tuners/lora/
+-rw-rw-r--   0 vinh      (1000) vinh      (1000)     1288 2024-02-28 10:20:13.000000 peft-0.9.0/src/peft/tuners/lora/__init__.py
+-rw-rw-r--   0 vinh      (1000) vinh      (1000)     3320 2024-02-28 10:20:13.000000 peft-0.9.0/src/peft/tuners/lora/aqlm.py
+-rw-rw-r--   0 vinh      (1000) vinh      (1000)     3693 2024-02-28 10:20:13.000000 peft-0.9.0/src/peft/tuners/lora/awq.py
+-rw-rw-r--   0 vinh      (1000) vinh      (1000)    16671 2024-02-28 10:20:13.000000 peft-0.9.0/src/peft/tuners/lora/bnb.py
+-rw-rw-r--   0 vinh      (1000) vinh      (1000)    15498 2024-02-28 10:20:13.000000 peft-0.9.0/src/peft/tuners/lora/config.py
+-rw-rw-r--   0 vinh      (1000) vinh      (1000)     3969 2024-02-28 10:20:13.000000 peft-0.9.0/src/peft/tuners/lora/gptq.py
+-rw-rw-r--   0 vinh      (1000) vinh      (1000)    37434 2024-02-28 10:20:13.000000 peft-0.9.0/src/peft/tuners/lora/layer.py
+-rw-rw-r--   0 vinh      (1000) vinh      (1000)    31995 2024-02-28 10:20:13.000000 peft-0.9.0/src/peft/tuners/lora/model.py
+-rw-rw-r--   0 vinh      (1000) vinh      (1000)     9175 2024-02-28 10:20:13.000000 peft-0.9.0/src/peft/tuners/lora/tp_layer.py
+-rw-rw-r--   0 vinh      (1000) vinh      (1000)    16629 2024-02-28 10:20:13.000000 peft-0.9.0/src/peft/tuners/lycoris_utils.py
+drwxrwxr-x   0 vinh      (1000) vinh      (1000)        0 2024-02-28 10:25:12.971027 peft-0.9.0/src/peft/tuners/mixed/
+-rw-rw-r--   0 vinh      (1000) vinh      (1000)      706 2024-02-28 10:20:13.000000 peft-0.9.0/src/peft/tuners/mixed/__init__.py
+-rw-rw-r--   0 vinh      (1000) vinh      (1000)    15006 2024-02-28 10:20:13.000000 peft-0.9.0/src/peft/tuners/mixed/model.py
+drwxrwxr-x   0 vinh      (1000) vinh      (1000)        0 2024-02-28 10:25:12.971027 peft-0.9.0/src/peft/tuners/multitask_prompt_tuning/
+-rw-rw-r--   0 vinh      (1000) vinh      (1000)      819 2024-02-28 10:20:13.000000 peft-0.9.0/src/peft/tuners/multitask_prompt_tuning/__init__.py
+-rw-rw-r--   0 vinh      (1000) vinh      (1000)     2446 2024-02-28 10:20:13.000000 peft-0.9.0/src/peft/tuners/multitask_prompt_tuning/config.py
+-rw-rw-r--   0 vinh      (1000) vinh      (1000)     4659 2024-02-28 10:20:13.000000 peft-0.9.0/src/peft/tuners/multitask_prompt_tuning/model.py
+drwxrwxr-x   0 vinh      (1000) vinh      (1000)        0 2024-02-28 10:25:12.971027 peft-0.9.0/src/peft/tuners/oft/
+-rw-rw-r--   0 vinh      (1000) vinh      (1000)      771 2024-02-28 10:20:13.000000 peft-0.9.0/src/peft/tuners/oft/__init__.py
+-rw-rw-r--   0 vinh      (1000) vinh      (1000)     5826 2024-02-28 10:20:13.000000 peft-0.9.0/src/peft/tuners/oft/config.py
+-rw-rw-r--   0 vinh      (1000) vinh      (1000)    15591 2024-02-28 10:20:13.000000 peft-0.9.0/src/peft/tuners/oft/layer.py
+-rw-rw-r--   0 vinh      (1000) vinh      (1000)     3695 2024-02-28 10:20:13.000000 peft-0.9.0/src/peft/tuners/oft/model.py
+drwxrwxr-x   0 vinh      (1000) vinh      (1000)        0 2024-02-28 10:25:12.975027 peft-0.9.0/src/peft/tuners/p_tuning/
+-rw-rw-r--   0 vinh      (1000) vinh      (1000)      801 2024-02-28 10:20:13.000000 peft-0.9.0/src/peft/tuners/p_tuning/__init__.py
+-rw-rw-r--   0 vinh      (1000) vinh      (1000)     2110 2024-02-28 10:20:13.000000 peft-0.9.0/src/peft/tuners/p_tuning/config.py
+-rw-rw-r--   0 vinh      (1000) vinh      (1000)     5575 2024-02-28 10:20:13.000000 peft-0.9.0/src/peft/tuners/p_tuning/model.py
+drwxrwxr-x   0 vinh      (1000) vinh      (1000)        0 2024-02-28 10:25:12.975027 peft-0.9.0/src/peft/tuners/poly/
+-rw-rw-r--   0 vinh      (1000) vinh      (1000)      759 2024-02-28 10:20:13.000000 peft-0.9.0/src/peft/tuners/poly/__init__.py
+-rw-rw-r--   0 vinh      (1000) vinh      (1000)     3783 2024-02-28 10:20:13.000000 peft-0.9.0/src/peft/tuners/poly/config.py
+-rw-rw-r--   0 vinh      (1000) vinh      (1000)     6890 2024-02-28 10:20:13.000000 peft-0.9.0/src/peft/tuners/poly/layer.py
+-rw-rw-r--   0 vinh      (1000) vinh      (1000)     6782 2024-02-28 10:20:13.000000 peft-0.9.0/src/peft/tuners/poly/model.py
+-rw-rw-r--   0 vinh      (1000) vinh      (1000)     2800 2024-02-28 10:20:13.000000 peft-0.9.0/src/peft/tuners/poly/router.py
+drwxrwxr-x   0 vinh      (1000) vinh      (1000)        0 2024-02-28 10:25:12.975027 peft-0.9.0/src/peft/tuners/prefix_tuning/
+-rw-rw-r--   0 vinh      (1000) vinh      (1000)      723 2024-02-28 10:20:13.000000 peft-0.9.0/src/peft/tuners/prefix_tuning/__init__.py
+-rw-rw-r--   0 vinh      (1000) vinh      (1000)     1386 2024-02-28 10:20:13.000000 peft-0.9.0/src/peft/tuners/prefix_tuning/config.py
+-rw-rw-r--   0 vinh      (1000) vinh      (1000)     3007 2024-02-28 10:20:13.000000 peft-0.9.0/src/peft/tuners/prefix_tuning/model.py
+drwxrwxr-x   0 vinh      (1000) vinh      (1000)        0 2024-02-28 10:25:12.975027 peft-0.9.0/src/peft/tuners/prompt_tuning/
+-rw-rw-r--   0 vinh      (1000) vinh      (1000)      765 2024-02-28 10:20:13.000000 peft-0.9.0/src/peft/tuners/prompt_tuning/__init__.py
+-rw-rw-r--   0 vinh      (1000) vinh      (1000)     2862 2024-02-28 10:20:13.000000 peft-0.9.0/src/peft/tuners/prompt_tuning/config.py
+-rw-rw-r--   0 vinh      (1000) vinh      (1000)     3623 2024-02-28 10:20:13.000000 peft-0.9.0/src/peft/tuners/prompt_tuning/model.py
+-rw-rw-r--   0 vinh      (1000) vinh      (1000)    27492 2024-02-28 10:20:13.000000 peft-0.9.0/src/peft/tuners/tuners_utils.py
+drwxrwxr-x   0 vinh      (1000) vinh      (1000)        0 2024-02-28 10:25:12.975027 peft-0.9.0/src/peft/utils/
+-rw-rw-r--   0 vinh      (1000) vinh      (1000)     1895 2024-02-28 10:20:13.000000 peft-0.9.0/src/peft/utils/__init__.py
+-rw-rw-r--   0 vinh      (1000) vinh      (1000)     5751 2024-02-28 10:20:13.000000 peft-0.9.0/src/peft/utils/constants.py
+-rw-rw-r--   0 vinh      (1000) vinh      (1000)     1394 2024-02-28 10:20:13.000000 peft-0.9.0/src/peft/utils/integrations.py
+-rw-rw-r--   0 vinh      (1000) vinh      (1000)     9312 2024-02-28 10:20:13.000000 peft-0.9.0/src/peft/utils/loftq_utils.py
+-rw-rw-r--   0 vinh      (1000) vinh      (1000)     9905 2024-02-28 10:20:13.000000 peft-0.9.0/src/peft/utils/merge_utils.py
+-rw-rw-r--   0 vinh      (1000) vinh      (1000)    24532 2024-02-28 10:20:13.000000 peft-0.9.0/src/peft/utils/other.py
+-rw-rw-r--   0 vinh      (1000) vinh      (1000)     2147 2024-02-28 10:20:13.000000 peft-0.9.0/src/peft/utils/peft_types.py
+-rw-rw-r--   0 vinh      (1000) vinh      (1000)    14820 2024-02-28 10:20:13.000000 peft-0.9.0/src/peft/utils/save_and_load.py
+drwxrwxr-x   0 vinh      (1000) vinh      (1000)        0 2024-02-28 10:25:12.967027 peft-0.9.0/src/peft.egg-info/
+-rw-rw-r--   0 vinh      (1000) vinh      (1000)    12093 2024-02-28 10:25:12.000000 peft-0.9.0/src/peft.egg-info/PKG-INFO
+-rw-rw-r--   0 vinh      (1000) vinh      (1000)     3193 2024-02-28 10:25:12.000000 peft-0.9.0/src/peft.egg-info/SOURCES.txt
+-rw-rw-r--   0 vinh      (1000) vinh      (1000)        1 2024-02-28 10:25:12.000000 peft-0.9.0/src/peft.egg-info/dependency_links.txt
+-rw-rw-r--   0 vinh      (1000) vinh      (1000)      369 2024-02-28 10:25:12.000000 peft-0.9.0/src/peft.egg-info/requires.txt
+-rw-rw-r--   0 vinh      (1000) vinh      (1000)        5 2024-02-28 10:25:12.000000 peft-0.9.0/src/peft.egg-info/top_level.txt
+drwxrwxr-x   0 vinh      (1000) vinh      (1000)        0 2024-02-28 10:25:12.979027 peft-0.9.0/tests/
+-rw-rw-r--   0 vinh      (1000) vinh      (1000)    19885 2024-02-28 10:20:13.000000 peft-0.9.0/tests/test_adaption_prompt.py
+-rw-rw-r--   0 vinh      (1000) vinh      (1000)     9035 2024-02-28 10:20:13.000000 peft-0.9.0/tests/test_auto.py
+-rw-rw-r--   0 vinh      (1000) vinh      (1000)    28539 2024-02-28 10:20:13.000000 peft-0.9.0/tests/test_common_gpu.py
+-rw-rw-r--   0 vinh      (1000) vinh      (1000)    10158 2024-02-28 10:20:13.000000 peft-0.9.0/tests/test_config.py
+-rw-rw-r--   0 vinh      (1000) vinh      (1000)    79291 2024-02-28 10:20:13.000000 peft-0.9.0/tests/test_custom_models.py
+-rw-rw-r--   0 vinh      (1000) vinh      (1000)    14665 2024-02-28 10:20:13.000000 peft-0.9.0/tests/test_decoder_models.py
+-rw-rw-r--   0 vinh      (1000) vinh      (1000)    10536 2024-02-28 10:20:13.000000 peft-0.9.0/tests/test_encoder_decoder_models.py
+-rw-rw-r--   0 vinh      (1000) vinh      (1000)     8228 2024-02-28 10:20:13.000000 peft-0.9.0/tests/test_feature_extraction_models.py
+-rw-rw-r--   0 vinh      (1000) vinh      (1000)    64302 2024-02-28 10:20:13.000000 peft-0.9.0/tests/test_gpu_examples.py
+-rw-rw-r--   0 vinh      (1000) vinh      (1000)     1328 2024-02-28 10:20:13.000000 peft-0.9.0/tests/test_hub_features.py
+-rw-rw-r--   0 vinh      (1000) vinh      (1000)    14993 2024-02-28 10:20:13.000000 peft-0.9.0/tests/test_initialization.py
+-rw-rw-r--   0 vinh      (1000) vinh      (1000)     6347 2024-02-28 10:20:13.000000 peft-0.9.0/tests/test_lora_megatron.py
+-rw-rw-r--   0 vinh      (1000) vinh      (1000)     2874 2024-02-28 10:20:13.000000 peft-0.9.0/tests/test_low_level_api.py
+-rw-rw-r--   0 vinh      (1000) vinh      (1000)    38774 2024-02-28 10:20:13.000000 peft-0.9.0/tests/test_mixed.py
+-rw-rw-r--   0 vinh      (1000) vinh      (1000)    13223 2024-02-28 10:20:13.000000 peft-0.9.0/tests/test_multitask_prompt_tuning.py
+-rw-rw-r--   0 vinh      (1000) vinh      (1000)     2338 2024-02-28 10:20:13.000000 peft-0.9.0/tests/test_other.py
+-rw-rw-r--   0 vinh      (1000) vinh      (1000)     3526 2024-02-28 10:20:13.000000 peft-0.9.0/tests/test_poly.py
+-rw-rw-r--   0 vinh      (1000) vinh      (1000)     9114 2024-02-28 10:20:13.000000 peft-0.9.0/tests/test_stablediffusion.py
+-rw-rw-r--   0 vinh      (1000) vinh      (1000)    17472 2024-02-28 10:20:13.000000 peft-0.9.0/tests/test_tuners_utils.py
+-rw-rw-r--   0 vinh      (1000) vinh      (1000)    55585 2024-02-28 10:20:13.000000 peft-0.9.0/tests/testing_common.py
+-rw-rw-r--   0 vinh      (1000) vinh      (1000)     3720 2024-02-28 10:20:13.000000 peft-0.9.0/tests/testing_utils.py
```

### Comparing `peft-0.8.2/LICENSE` & `peft-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `peft-0.8.2/setup.py` & `peft-0.9.0/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -11,19 +11,26 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from setuptools import find_packages, setup
 
 
-VERSION = "0.8.2"
+VERSION = "0.9.0"
 
 extras = {}
-extras["quality"] = ["black ~= 22.0", "ruff>=0.0.241", "urllib3<=2.0.0"]
-extras["docs_specific"] = ["hf-doc-builder"]
+extras["quality"] = [
+    "black",  # doc-builder has an implicit dependency on Black, see huggingface/doc-builder#434
+    "hf-doc-builder",
+    "ruff~=0.2.1",
+]
+extras["docs_specific"] = [
+    "black",  # doc-builder has an implicit dependency on Black, see huggingface/doc-builder#434
+    "hf-doc-builder",
+]
 extras["dev"] = extras["quality"] + extras["docs_specific"]
 extras["test"] = extras["dev"] + [
     "pytest",
     "pytest-cov",
     "pytest-xdist",
     "parameterized",
     "datasets",
@@ -32,15 +39,15 @@
 ]
 
 setup(
     name="peft",
     version=VERSION,
     description="Parameter-Efficient Fine-Tuning (PEFT)",
     license_files=["LICENSE"],
-    long_description=open("README.md", "r", encoding="utf-8").read(),
+    long_description=open("README.md", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     keywords="deep learning",
     license="Apache",
     author="The HuggingFace team",
     author_email="sourab@huggingface.co",
     url="https://github.com/huggingface/peft",
     package_dir={"": "src"},
@@ -72,15 +79,15 @@
         "Programming Language :: Python :: 3.8",
         "Topic :: Scientific/Engineering :: Artificial Intelligence",
     ],
 )
 
 # Release checklist
 # 1. Change the version in __init__.py and setup.py to the release version, e.g. from "0.6.0.dev0" to "0.6.0"
-# 2. Check if there are any deprecations that need to be addressed for this release by seaching for "# TODO" in the code
+# 2. Check if there are any deprecations that need to be addressed for this release by searching for "# TODO" in the code
 # 3. Commit these changes with the message: "Release: VERSION", create a PR and merge it.
 # 4. Add a tag in git to mark the release: "git tag -a VERSION -m 'Adds tag VERSION for pypi' "
 #    Push the tag to git:
 #      git push --tags origin main
 #    It is necessary to work on the original repository, not on a fork.
 # 5. Run the following commands in the top-level directory:
 #      python setup.py bdist_wheel
```

### Comparing `peft-0.8.2/src/peft/__init__.py` & `peft-0.9.0/src/peft/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-__version__ = "0.8.2"
+__version__ = "0.9.0"
 
 from .auto import (
     AutoPeftModel,
     AutoPeftModelForCausalLM,
     AutoPeftModelForSequenceClassification,
     AutoPeftModelForSeq2SeqLM,
     AutoPeftModelForTokenClassification,
```

### Comparing `peft-0.8.2/src/peft/auto.py` & `peft-0.9.0/src/peft/auto.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# coding=utf-8
 # Copyright 2023-present the HuggingFace Inc. team.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
@@ -15,15 +14,14 @@
 
 from __future__ import annotations
 
 import importlib
 import os
 from typing import Optional
 
-from huggingface_hub import file_exists
 from transformers import (
     AutoModel,
     AutoModelForCausalLM,
     AutoModelForQuestionAnswering,
     AutoModelForSeq2SeqLM,
     AutoModelForSequenceClassification,
     AutoModelForTokenClassification,
@@ -38,23 +36,24 @@
     PeftModelForFeatureExtraction,
     PeftModelForQuestionAnswering,
     PeftModelForSeq2SeqLM,
     PeftModelForSequenceClassification,
     PeftModelForTokenClassification,
 )
 from .utils.constants import TOKENIZER_CONFIG_NAME
+from .utils.other import check_file_exists_on_hf_hub
 
 
 class _BaseAutoPeftModel:
     _target_class = None
     _target_peft_class = None
 
     def __init__(self, *args, **kwargs):
         # For consistency with transformers: https://github.com/huggingface/transformers/blob/91d7df58b6537d385e90578dac40204cb550f706/src/transformers/models/auto/auto_factory.py#L400
-        raise EnvironmentError(
+        raise EnvironmentError(  # noqa: UP024
             f"{self.__class__.__name__} is designed to be instantiated "
             f"using the `{self.__class__.__name__}.from_pretrained(pretrained_model_name_or_path)` or "
             f"`{self.__class__.__name__}.from_config(config)` methods."
         )
 
     @classmethod
     def from_pretrained(
@@ -108,24 +107,26 @@
         if os.path.exists(os.path.join(pretrained_model_name_or_path, TOKENIZER_CONFIG_NAME)):
             tokenizer_exists = True
         else:
             token = kwargs.get("token", None)
             if token is None:
                 token = kwargs.get("use_auth_token", None)
 
-            tokenizer_exists = file_exists(
+            tokenizer_exists = check_file_exists_on_hf_hub(
                 repo_id=pretrained_model_name_or_path,
                 filename=TOKENIZER_CONFIG_NAME,
                 revision=kwargs.get("revision", None),
                 repo_type=kwargs.get("repo_type", None),
                 token=token,
             )
 
         if tokenizer_exists:
-            tokenizer = AutoTokenizer.from_pretrained(pretrained_model_name_or_path)
+            tokenizer = AutoTokenizer.from_pretrained(
+                pretrained_model_name_or_path, trust_remote_code=kwargs.get("trust_remote_code", False)
+            )
             base_model.resize_token_embeddings(len(tokenizer))
 
         return cls._target_peft_class.from_pretrained(
             base_model,
             pretrained_model_name_or_path,
             adapter_name=adapter_name,
             is_trainable=is_trainable,
```

### Comparing `peft-0.8.2/src/peft/config.py` & `peft-0.9.0/src/peft/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# coding=utf-8
 # Copyright 2023-present the HuggingFace Inc. team.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
@@ -156,15 +155,15 @@
         r"""
         Loads a configuration file from a json file.
 
         Args:
             path_json_file (`str`):
                 The path to the json file.
         """
-        with open(path_json_file, "r") as file:
+        with open(path_json_file) as file:
             json_object = json.load(file)
 
         return json_object
 
     @classmethod
     def _split_kwargs(cls, kwargs):
         hf_hub_download_kwargs = {}
```

### Comparing `peft-0.8.2/src/peft/helpers.py` & `peft-0.9.0/src/peft/helpers.py`

 * *Files identical despite different names*

### Comparing `peft-0.8.2/src/peft/import_utils.py` & `peft-0.9.0/src/peft/import_utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# coding=utf-8
 # Copyright 2023-present the HuggingFace Inc. team.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
@@ -45,22 +44,30 @@
             )
 
 
 def is_optimum_available() -> bool:
     return importlib.util.find_spec("optimum") is not None
 
 
-@lru_cache()
+@lru_cache
 def is_torch_tpu_available(check_device=True):
     "Checks if `torch_xla` is installed and potentially if a TPU is in the environment"
     if importlib.util.find_spec("torch_xla") is not None:
         if check_device:
             # We need to check if `xla_device` can be found, will raise a RuntimeError if not
             try:
                 import torch_xla.core.xla_model as xm
 
                 _ = xm.xla_device()
                 return True
             except RuntimeError:
                 return False
         return True
     return False
+
+
+def is_aqlm_available():
+    return importlib.util.find_spec("aqlm") is not None
+
+
+def is_auto_awq_available():
+    return importlib.util.find_spec("awq") is not None
```

### Comparing `peft-0.8.2/src/peft/mapping.py` & `peft-0.9.0/src/peft/mapping.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# coding=utf-8
 # Copyright 2023-present the HuggingFace Inc. team.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
@@ -11,15 +10,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, Any, Dict
+from typing import TYPE_CHECKING, Any
 
 import torch
 
 from .config import PeftConfig
 from .mixed_model import PeftMixedModel
 from .peft_model import (
     PeftModel,
@@ -54,24 +53,24 @@
 from .utils import _prepare_prompt_learning_config
 
 
 if TYPE_CHECKING:
     from transformers import PreTrainedModel
 
 
-MODEL_TYPE_TO_PEFT_MODEL_MAPPING: Dict[str, PeftModel] = {
+MODEL_TYPE_TO_PEFT_MODEL_MAPPING: dict[str, PeftModel] = {
     "SEQ_CLS": PeftModelForSequenceClassification,
     "SEQ_2_SEQ_LM": PeftModelForSeq2SeqLM,
     "CAUSAL_LM": PeftModelForCausalLM,
     "TOKEN_CLS": PeftModelForTokenClassification,
     "QUESTION_ANS": PeftModelForQuestionAnswering,
     "FEATURE_EXTRACTION": PeftModelForFeatureExtraction,
 }
 
-PEFT_TYPE_TO_CONFIG_MAPPING: Dict[str, PeftConfig] = {
+PEFT_TYPE_TO_CONFIG_MAPPING: dict[str, PeftConfig] = {
     "ADAPTION_PROMPT": AdaptionPromptConfig,
     "PROMPT_TUNING": PromptTuningConfig,
     "PREFIX_TUNING": PrefixTuningConfig,
     "P_TUNING": PromptEncoderConfig,
     "LORA": LoraConfig,
     "LOHA": LoHaConfig,
     "LOKR": LoKrConfig,
@@ -89,15 +88,15 @@
     "ADALORA": AdaLoraModel,
     "IA3": IA3Model,
     "OFT": OFTModel,
     "POLY": PolyModel,
 }
 
 
-def get_peft_config(config_dict: Dict[str, Any]) -> PeftConfig:
+def get_peft_config(config_dict: dict[str, Any]) -> PeftConfig:
     """
     Returns a Peft config object from a dictionary.
 
     Args:
         config_dict (`Dict[str, Any]`): Dictionary containing the configuration parameters.
     """
```

### Comparing `peft-0.8.2/src/peft/mixed_model.py` & `peft-0.9.0/src/peft/mixed_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# coding=utf-8
 # Copyright 2023-present the HuggingFace Inc. team.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
@@ -79,47 +78,38 @@
             f"The provided `peft_type` '{peft_config.peft_type.value}' is not compatible with the `PeftMixedModel`. "
             f"Compatible types are: {COMPATIBLE_TUNER_TYPES}"
         )
 
 
 class PeftMixedModel(PushToHubMixin, torch.nn.Module):
     """
-    Peft model for mixing different types of adapters.
+    PeftMixedModel for loading mixing different types of adapters for inference.
 
-    This class currently does not support saving and loading. Instead, it is assumed that the adapters are already
-    trained and loading the model requires a script to be run each time.
+    This class does not support loading/saving, and it shouldn't usually be initialized directly. Instead, use
+    `get_peft_model` with the argument `mixed=True`.
 
-    Currently, the main purpose of mixed adapter types is to combine trained adapters for inference. Although it is
-    technically possible to train a mixed adapter model, this has not been tested and is not recommended.
+    <Tip>
 
-    Note: This class should usually not be initialized directly. Instead, use `get_peft_model` with the argument
-    `mixed=True`.
+    Read the [Mixed adapter types](https://huggingface.co/docs/peft/en/developer_guides/mixed_models) guide to learn
+    more about using different adapter types.
 
-    Below is an example that shows how to load a mixed model with two different types of adapters.
+    </Tip>
+
+    Example:
 
     ```py
     >>> from peft import get_peft_model
 
     >>> base_model = ...  # load the base model, e.g. from transformers
     >>> peft_model = PeftMixedModel.from_pretrained(base_model, path_to_adapter1, "adapter1").eval()
     >>> peft_model.load_adapter(path_to_adapter2, "adapter2")
     >>> peft_model.set_adapter(["adapter1", "adapter2"])  # activate both adapters
     >>> peft_model(data)  # forward pass using both adapters
     ```
 
-    Tips:
-
-    - Not all adapter types can be combined. See `peft.tuners.mixed.COMPATIBLE_TUNER_TYPES` for a list of compatible
-      types. An error will be raised if you are trying to combine incompatible adapter types.
-    - It is possible to mix multiple adapters of the same type. This can be useful to combine adapters with very
-      different configs.
-    - If you want to combine a lot of different adapters, it is most performant to add the same types of adapters
-      consecutively. E.g., add LoRA1, LoRA2, LoHa1, LoHa2 in this order, instead of LoRA1, LoHa1, LoRA2, LoHa2. As long
-      as the adapters are commutative, the order does not matter for the final result.
-
     Args:
         model (`torch.nn.Module`):
             The model to be tuned.
         config (`PeftConfig`):
             The config of the model to be tuned. The adapter type must be compatible.
         adapter_name (`str`, `optional`, defaults to `"default"`):
             The name of the first adapter.
@@ -223,15 +213,15 @@
 
     def add_adapter(self, adapter_name: str, peft_config: PeftConfig):
         _check_config_compatible(peft_config)
 
         try:
             self.peft_config[adapter_name] = peft_config
             self.base_model.inject_adapter(self, adapter_name)
-        except Exception:  # somthing went wrong, roll back
+        except Exception:  # something went wrong, roll back
             if adapter_name in self.peft_config:
                 del self.peft_config[adapter_name]
             raise
 
         self.set_modules_to_save(peft_config, adapter_name)
 
     def set_modules_to_save(self, peft_config: PeftConfig, adapter_name: str) -> None:
@@ -249,14 +239,23 @@
         Sets the active adapter(s) for the model.
 
         Note that the order in which the adapters are applied during the forward pass may not be the same as the order
         in which they are passed to this function. Instead, the order during the forward pass is determined by the
         order in which the adapters were loaded into the model. The active adapters only determine which adapters are
         active during the forward pass, but not the order in which they are applied.
 
+        Additionally, this function will set the specified adapters to trainable (i.e., requires_grad=True). If this is
+        not desired, use the following code.
+
+        ```py
+        >>> for name, param in model_peft.named_parameters():
+        ...     if ...:  # some check on name (ex. if 'lora' in name)
+        ...         param.requires_grad = False
+        ```
+
         Args:
             adapter_name (`str` or `List[str]`):
                 The name of the adapter(s) to be activated.
         """
         if isinstance(adapter_name, str):
             adapter_name = [adapter_name]
 
@@ -353,15 +352,15 @@
                       method (`./my_peft_config_directory/`).
             adapter_name (`str`, *optional*, defaults to `"default"`):
                 The name of the adapter to be loaded. This is useful for loading multiple adapters.
             is_trainable (`bool`, *optional*, defaults to `False`):
                 Whether the adapter should be trainable or not. If `False`, the adapter will be frozen and use for
                 inference
             config ([`~peft.PeftConfig`], *optional*):
-                The configuration object to use instead of an automatically loaded configuation. This configuration
+                The configuration object to use instead of an automatically loaded configuration. This configuration
                 object is mutually exclusive with `model_id` and `kwargs`. This is useful when configuration is already
                 loaded before calling `from_pretrained`.
             kwargs: (`optional`):
                 Additional keyword arguments passed along to the specific PEFT configuration class.
         """
         # note: adapted from PeftModel.from_pretrained
         from .mapping import PEFT_TYPE_TO_CONFIG_MAPPING
```

### Comparing `peft-0.8.2/src/peft/peft_model.py` & `peft-0.9.0/src/peft/peft_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# coding=utf-8
 # Copyright 2023-present the HuggingFace Inc. team.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
@@ -17,15 +16,15 @@
 
 import collections
 import inspect
 import os
 import warnings
 from contextlib import contextmanager
 from copy import deepcopy
-from typing import Any, Dict, List, Optional, Union
+from typing import Any, Optional, Union
 
 import packaging.version
 import torch
 import transformers
 from accelerate import dispatch_model, infer_auto_device_map
 from accelerate.hooks import AlignDevicesHook, add_hook_to_module, remove_hook_from_submodules
 from accelerate.utils import get_balanced_memory
@@ -133,15 +132,15 @@
         # the `pretraining_tp` is set for some models to simulate Tensor Parallelism during inference to avoid
         # numerical differences, https://github.com/pytorch/pytorch/issues/76232 - to avoid any unexpected
         # behavior we disable that in this line.
         if hasattr(self.base_model, "config") and hasattr(self.base_model.config, "pretraining_tp"):
             self.base_model.config.pretraining_tp = 1
 
     @property
-    def peft_config(self) -> Dict[str, PeftConfig]:
+    def peft_config(self) -> dict[str, PeftConfig]:
         if self._is_prompt_learning:
             return self._peft_config
         return self.base_model.peft_config
 
     @property
     def active_adapters(self) -> list[str]:
         try:
@@ -149,25 +148,25 @@
         except AttributeError:
             adapters = self.active_adapter
             if isinstance(adapters, str):
                 adapters = [adapters]
         return adapters
 
     @peft_config.setter
-    def peft_config(self, value: Dict[str, PeftConfig]):
+    def peft_config(self, value: dict[str, PeftConfig]):
         if self._is_prompt_learning:
             self._peft_config = value
         else:
             self.base_model.peft_config = value
 
     def save_pretrained(
         self,
         save_directory: str,
         safe_serialization: bool = True,
-        selected_adapters: Optional[List[str]] = None,
+        selected_adapters: Optional[list[str]] = None,
         save_embedding_layers: Union[str, bool] = "auto",
         is_main_process: bool = True,
         **kwargs: Any,
     ) -> None:
         r"""
         This function saves the adapter model and the adapter configuration files to a directory, so that it can be
         reloaded using the [`PeftModel.from_pretrained`] class method, and also used by the [`PeftModel.push_to_hub`]
@@ -286,15 +285,15 @@
         cls,
         model: torch.nn.Module,
         model_id: Union[str, os.PathLike],
         adapter_name: str = "default",
         is_trainable: bool = False,
         config: Optional[PeftConfig] = None,
         **kwargs: Any,
-    ) -> "PeftModel":
+    ) -> PeftModel:
         r"""
         Instantiate a PEFT model from a pretrained model and loaded PEFT weights.
 
         Note that the passed `model` may be modified inplace.
 
         Args:
             model ([`torch.nn.Module`]):
@@ -308,15 +307,15 @@
                       method (`./my_peft_config_directory/`).
             adapter_name (`str`, *optional*, defaults to `"default"`):
                 The name of the adapter to be loaded. This is useful for loading multiple adapters.
             is_trainable (`bool`, *optional*, defaults to `False`):
                 Whether the adapter should be trainable or not. If `False`, the adapter will be frozen and can only be
                 used for inference.
             config ([`~peft.PeftConfig`], *optional*):
-                The configuration object to use instead of an automatically loaded configuation. This configuration
+                The configuration object to use instead of an automatically loaded configuration. This configuration
                 object is mutually exclusive with `model_id` and `kwargs`. This is useful when configuration is already
                 loaded before calling `from_pretrained`.
             kwargs: (`optional`):
                 Additional keyword arguments passed along to the specific PEFT configuration class.
         """
         from .mapping import MODEL_TYPE_TO_PEFT_MODEL_MAPPING, PEFT_TYPE_TO_CONFIG_MAPPING
 
@@ -556,26 +555,26 @@
         >>> with model.disable_adapter():
         ...     model(inputs)
         ```
         """
         try:
             if self.peft_config[self.active_adapter].is_prompt_learning:
                 # TODO: consider replacing this patching of methods with a more robust mechanism: setting a flag and
-                # letting the underyling methods deal with it, same as how LoRA does it.
+                # letting the underlying methods deal with it, same as how LoRA does it.
                 old_forward = self.forward
                 self.forward = self.base_model.forward
                 old_prepare_inputs_for_generation = self.prepare_inputs_for_generation
                 self.prepare_inputs_for_generation = self.base_model.prepare_inputs_for_generation
             else:
                 self.base_model.disable_adapter_layers()
             yield
         finally:
             if self.peft_config[self.active_adapter].is_prompt_learning:
                 self.forward = old_forward
-                self.old_prepare_inputs_for_generation = old_prepare_inputs_for_generation
+                self.prepare_inputs_for_generation = old_prepare_inputs_for_generation
             else:
                 self.base_model.enable_adapter_layers()
 
     def get_base_model(self) -> torch.nn.Module:
         """
         Returns the base model.
         """
@@ -617,15 +616,15 @@
                 peft_config = _prepare_prompt_learning_config(peft_config, dict_config)
                 self._setup_prompt_encoder(adapter_name)
             elif peft_config.is_adaption_prompt:
                 self.base_model.add_adapter(adapter_name, peft_config)
             else:
                 self.peft_config[adapter_name] = peft_config
                 self.base_model.inject_adapter(self.base_model.model, adapter_name)
-        except Exception:  # somthing went wrong, roll back
+        except Exception:  # something went wrong, roll back
             if adapter_name in self.peft_config:
                 del self.peft_config[adapter_name]
             raise
 
         self.set_additional_trainable_modules(peft_config, adapter_name)
 
     def set_additional_trainable_modules(self, peft_config, adapter_name):
@@ -633,15 +632,15 @@
             if self.modules_to_save is None:
                 self.modules_to_save = set(peft_config.modules_to_save)
             else:
                 self.modules_to_save.update(peft_config.modules_to_save)
             _set_trainable(self, adapter_name)
 
     @classmethod
-    def _split_kwargs(cls, kwargs: Dict[str, Any]):
+    def _split_kwargs(cls, kwargs: dict[str, Any]):
         _kwargs_not_in_hf_hub_download_signature = ("use_auth_token",)
         hf_hub_download_kwargs = {}
         other_kwargs = {}
 
         for key, value in kwargs.items():
             if key in inspect.signature(hf_hub_download).parameters or key in _kwargs_not_in_hf_hub_download_signature:
                 hf_hub_download_kwargs[key] = value
@@ -743,14 +742,23 @@
 
     def set_adapter(self, adapter_name: str) -> None:
         """
         Sets the active adapter.
 
         Only one adapter can be active at a time.
 
+        Additionally, this function will set the specified adapter to trainable (i.e., requires_grad=True). If this is
+        not desired, use the following code.
+
+        ```py
+        >>> for name, param in model_peft.named_parameters():
+        ...     if ...:  # some check on name (ex. if 'lora' in name)
+        ...         param.requires_grad = False
+        ```
+
         Args:
             adapter_name (`str`):
                 The name of the adapter to be set as active. The adapter must be loaded first.
         """
         if adapter_name not in self.peft_config:
             raise ValueError(f"Adapter {adapter_name} not found.")
         self.active_adapter = adapter_name
@@ -780,15 +788,15 @@
         card = ModelCard.load(filename) if os.path.exists(filename) else ModelCard.from_template(ModelCardData())
 
         card.data["library_name"] = "peft"
 
         model_config = getattr(self, "config", None)
         if hasattr(model_config, "to_dict"):
             model_config = model_config.to_dict()
-        if model_config is not None:
+        if model_config is not None and "_name_or_path" in model_config:
             card.data["base_model"] = model_config["_name_or_path"]
 
         lines = card.text.splitlines()
 
         quantization_config = None
         if hasattr(model_config, "quantization_config"):
             quantization_config = self.config.quantization_config.to_dict()
@@ -1141,15 +1149,15 @@
         except:
             self.base_model.prepare_inputs_for_generation = self.base_model_prepare_inputs_for_generation
             raise
         else:
             self.base_model.prepare_inputs_for_generation = self.base_model_prepare_inputs_for_generation
             return outputs
 
-    def prepare_inputs_for_generation(self, *args, task_ids: torch.Tensor = None, **kwargs):
+    def prepare_inputs_for_generation(self, *args, task_ids: Optional[torch.Tensor] = None, **kwargs):
         peft_config = self.active_peft_config
         model_kwargs = self.base_model_prepare_inputs_for_generation(*args, **kwargs)
 
         # https://github.com/huggingface/transformers/pull/26681/ introduced new cache format
         # for some architectures which requires a special fix for prompt tuning etc.
         # TODO: starting with transformers 4.38, all architectures should support caching.
         uses_transformers_4_38 = packaging.version.parse(transformers.__version__) >= packaging.version.parse("4.38.0")
@@ -1193,14 +1201,20 @@
                 if model_kwargs["past_key_values"] is None:
                     inputs_embeds = self.word_embeddings(model_kwargs["input_ids"])
                     prompts = self.get_prompt(batch_size=model_kwargs["input_ids"].shape[0], task_ids=task_ids)
                     prompts = prompts.to(inputs_embeds.dtype)
                     model_kwargs["inputs_embeds"] = torch.cat((prompts, inputs_embeds), dim=1)
                     model_kwargs["input_ids"] = None
 
+        # For transformers>=4.38.0 - for some architectures such as Llama, `cache_position` is
+        # passed in the forward pass to keep track of the position ids of the cache. We have to
+        # pop that from `model_kwargs` as `cache_position` is properly created by the model, using the passed
+        # `inputs_embeds`: https://github.com/huggingface/transformers/blob/593230f0a1150ea9c0477b9d859f25daf73c8c33/src/transformers/models/llama/modeling_llama.py#L956
+        _ = model_kwargs.pop("cache_position", None)
+
         return model_kwargs
 
 
 class PeftModelForSeq2SeqLM(PeftModel):
     """
     Peft model for sequence-to-sequence language modeling.
 
@@ -1396,15 +1410,15 @@
                     PeftType.PROMPT_TUNING,
                     PeftType.P_TUNING,
                     PeftType.MULTITASK_PROMPT_TUNING,
                 ]:
                     kwargs = deepcopy(kwargs)
 
                     if "encoder_outputs" in kwargs:
-                        del kwargs["encoder_ouputs"]
+                        del kwargs["encoder_outputs"]
                         warnings.warn(
                             "`encoder_outputs` should not be passed to `generate` when using prompt tuning. Ignoring it."
                         )
 
                     input_ids = kwargs.pop("input_ids")
                     inputs_embeds = self.word_embeddings(input_ids)
                     batch_size = inputs_embeds.shape[0]
```

### Comparing `peft-0.8.2/src/peft/tuners/__init__.py` & `peft-0.9.0/src/peft/tuners/__init__.py`

 * *Files identical despite different names*

### Comparing `peft-0.8.2/src/peft/tuners/adalora/__init__.py` & `peft-0.9.0/src/peft/tuners/adalora/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# coding=utf-8
 # Copyright 2023-present the HuggingFace Inc. team.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `peft-0.8.2/src/peft/tuners/adalora/bnb.py` & `peft-0.9.0/src/peft/tuners/adalora/bnb.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# coding=utf-8
 # Copyright 2023-present the HuggingFace Inc. team.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `peft-0.8.2/src/peft/tuners/adalora/config.py` & `peft-0.9.0/src/peft/tuners/adalora/config.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# coding=utf-8
 # Copyright 2023-present the HuggingFace Inc. team.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
@@ -35,15 +34,15 @@
         beta2 (`float`): The hyperparameter of EMA for undertainty quantification.
         orth_reg_weight (`float`): The coefficient of orthogonal regularization.
         total_step (`int`): The total training steps that should be specified before training.
         rank_pattern (`list`): The allocated rank for each weight matrix by RankAllocator.
     """
 
     target_r: int = field(default=8, metadata={"help": "Target Lora matrix dimension."})
-    init_r: int = field(default=12, metadata={"help": "Intial Lora matrix dimension."})
+    init_r: int = field(default=12, metadata={"help": "Initial Lora matrix dimension."})
     tinit: int = field(default=0, metadata={"help": "The steps of initial warmup."})
     tfinal: int = field(default=0, metadata={"help": "The steps of final warmup."})
     deltaT: int = field(default=1, metadata={"help": "Step interval of rank allocation."})
     beta1: float = field(default=0.85, metadata={"help": "Hyperparameter of EMA."})
     beta2: float = field(default=0.85, metadata={"help": "Hyperparameter of EMA."})
     orth_reg_weight: float = field(default=0.5, metadata={"help": "The orthogonal regularization coefficient."})
     total_step: Optional[int] = field(default=None, metadata={"help": "The total training steps."})
```

### Comparing `peft-0.8.2/src/peft/tuners/adalora/gptq.py` & `peft-0.9.0/src/peft/tuners/adalora/gptq.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# coding=utf-8
 # Copyright 2023-present the HuggingFace Inc. team.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `peft-0.8.2/src/peft/tuners/adalora/layer.py` & `peft-0.9.0/src/peft/tuners/adalora/layer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# coding=utf-8
 # Copyright 2023-present the HuggingFace Inc. team.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
@@ -153,15 +152,14 @@
         return (
             transpose(self.lora_B[adapter] @ (self.lora_A[adapter] * self.lora_E[adapter]), self.fan_in_fan_out)
             * self.scaling[adapter]
             / (self.ranknum[adapter] + 1e-5)
         )
 
     def forward(self, x: torch.Tensor, *args: Any, **kwargs: Any) -> torch.Tensor:
-        # TODO: SVDLinear does not convert dtype, unlike lora linear, is that correct?
         if self.disable_adapters:
             if self.merged:
                 self.unmerge()
             result = self.base_layer(x, *args, **kwargs)
         elif self.merged:
             result = self.base_layer(x, *args, **kwargs)
         else:
@@ -172,14 +170,15 @@
                 lora_A = self.lora_A[active_adapter]
                 lora_B = self.lora_B[active_adapter]
                 lora_E = self.lora_E[active_adapter]
                 dropout = self.lora_dropout[active_adapter]
                 scaling = self.scaling[active_adapter]
                 ranknum = self.ranknum[active_adapter] + 1e-5
 
+                x = x.to(lora_A.dtype)
                 result += (dropout(x) @ (lora_A * lora_E).T @ lora_B.T) * scaling / ranknum
 
         return result
 
     def __repr__(self) -> str:
         rep = super().__repr__()
         return "adalora." + rep
```

### Comparing `peft-0.8.2/src/peft/tuners/adalora/model.py` & `peft-0.9.0/src/peft/tuners/adalora/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# coding=utf-8
 # Copyright 2023-present the HuggingFace Inc. team.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
@@ -242,15 +241,15 @@
                 raise ValueError("orth_reg_weight should be greater than 0. ")
 
             regu_loss = 0
             num_param = 0
             for n, p in self.model.named_parameters():
                 if ("lora_A" in n or "lora_B" in n) and self.trainable_adapter_name in n:
                     para_cov = p @ p.T if "lora_A" in n else p.T @ p
-                    I = torch.eye(*para_cov.size(), out=torch.empty_like(para_cov))
+                    I = torch.eye(*para_cov.size(), out=torch.empty_like(para_cov))  # noqa: E741
                     I.requires_grad = False
                     num_param += 1
                     regu_loss += torch.norm(para_cov - I, p="fro")
             if num_param > 0:
                 regu_loss = regu_loss / num_param
             else:
                 regu_loss = 0
@@ -262,15 +261,15 @@
         for name, rank_idx in rank_pattern.items():
             if isinstance(rank_idx, list):
                 rank = sum(rank_idx)
             elif isinstance(rank_idx, torch.Tensor):
                 rank_idx = rank_idx.view(-1)
                 rank = rank_idx.sum().item()
             else:
-                raise ValueError("Unexcepted type of rank_idx")
+                raise ValueError("Unexpected type of rank_idx")
             key = ".".join(name.split(".")[0:-2]) if adapter_name in name else ".".join(name.split(".")[0:-1])
             _, target, _ = _get_submodules(self.model, key)
             lora_E_weights = target.lora_E[adapter_name][rank_idx]
             lora_A_weights = target.lora_A[adapter_name][rank_idx]
             lora_B_weights = target.lora_B[adapter_name][:, rank_idx]
             ranknum = target.ranknum[adapter_name]
             target.update_layer(
```

### Comparing `peft-0.8.2/src/peft/tuners/adaption_prompt/__init__.py` & `peft-0.9.0/src/peft/tuners/adaption_prompt/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# coding=utf-8
 # Copyright 2023-present the HuggingFace Inc. team.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `peft-0.8.2/src/peft/tuners/adaption_prompt/config.py` & `peft-0.9.0/src/peft/tuners/adaption_prompt/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# coding=utf-8
 # Copyright 2023-present the HuggingFace Inc. team.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `peft-0.8.2/src/peft/tuners/adaption_prompt/layer.py` & `peft-0.9.0/src/peft/tuners/adaption_prompt/layer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# coding=utf-8
 # Copyright 2023-present the HuggingFace Inc. team.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `peft-0.8.2/src/peft/tuners/adaption_prompt/model.py` & `peft-0.9.0/src/peft/tuners/adaption_prompt/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# coding=utf-8
 # Copyright 2023-present the HuggingFace Inc. team.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `peft-0.8.2/src/peft/tuners/adaption_prompt/utils.py` & `peft-0.9.0/src/peft/tuners/adaption_prompt/utils.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-# coding=utf-8
 # Copyright 2023-present the HuggingFace Inc. team.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+import inspect
 
 import torch
 import torch.nn as nn
 
 
 def llama_rotate_half(x: torch.Tensor) -> torch.Tensor:
     """
@@ -55,35 +55,57 @@
         sin = sin[position_ids].unsqueeze(1)
     q_embed = (q * cos) + (llama_rotate_half(q) * sin)
     return q_embed
 
 
 def llama_compute_query_states(model: nn.Module, **kwargs) -> torch.Tensor:
     """
-    Compute query states for Llama models specifically.
-
-    They need to be recomputed as the forward() method of the original LlamaModel in the transformers library does not
-    return them. See the related discussion in the PR: https://github.com/huggingface/peft/pull/268
+    Compute query states for Llama models specifically. They need to be recomputed as the forward() method of the
+    original LlamaModel in the transformers library does not return them. See the related discussion in the PR:
+    https://github.com/huggingface/peft/pull/268
     """
     hidden_states = kwargs.get("hidden_states")
     position_ids = kwargs.get("position_ids")
     past_key_value = kwargs.get("past_key_value")
     bsz, q_len, _ = hidden_states.size()
     query_states = model.q_proj(hidden_states).view(bsz, q_len, model.num_heads, model.head_dim).transpose(1, 2)
     value_states = model.v_proj(hidden_states).view(bsz, q_len, model.num_heads, model.head_dim).transpose(1, 2)
-
     seq_len = q_len
+
     if past_key_value is not None:
         if isinstance(past_key_value, tuple):
             # for transformers <= 4.35
             seq_len += past_key_value[0].shape[-2]
         else:
             # since transformers 4.36, this is a DynamicCache instance
             seq_len += past_key_value.get_seq_length(model.layer_idx)
-    cos, sin = model.rotary_emb(value_states, seq_len=seq_len)
 
-    return llama_apply_rotary_pos_emb(query_states, cos, sin, position_ids)
+    # For transformers > 4.37.2 `position_ids` became a required arguments in the rotary embedding's forward pass.
+    if "position_ids" not in inspect.signature(model.rotary_emb.forward).parameters:
+        # TODO we assume that position_ids is not None here, not sure if that is safe but the old code also did that
+        cos, sin = model.rotary_emb(value_states, seq_len=seq_len)
+        return llama_apply_rotary_pos_emb(query_states, cos, sin, position_ids)
+
+    past_seen_tokens = 0
+    if position_ids is None:
+        # Compute position_ids, since they are required for transformers > 4.37.2
+        if past_key_value is None:
+            new_cache_positions = torch.arange(q_len, q_len + q_len, device=value_states.device)
+        else:
+            past_seen_tokens = past_key_value.get_usable_length(q_len, model.layer_idx)
+            new_cache_positions = torch.arange(past_seen_tokens, past_seen_tokens + q_len, device=value_states.device)
+        position_ids = new_cache_positions.unsqueeze(0)
+
+    cos, sin = model.rotary_emb(value_states, seq_len=q_len + past_seen_tokens, position_ids=position_ids)
+
+    # For batched inference unsqueeze it on the correct dim
+    # since: https://github.com/huggingface/transformers/pull/29109
+    if len(cos.shape) == 3:
+        cos = cos.unsqueeze(1)
+        sin = sin.unsqueeze(1)
+
+    return (query_states * cos) + (llama_rotate_half(query_states) * sin)
 
 
 def is_adaption_prompt_trainable(params: str) -> bool:
     """Return True if module is trainable under adaption prompt fine-tuning."""
     return params.split(".")[-1].startswith("adaption_")
```

### Comparing `peft-0.8.2/src/peft/tuners/ia3/__init__.py` & `peft-0.9.0/src/peft/tuners/ia3/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# coding=utf-8
 # Copyright 2023-present the HuggingFace Inc. team.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `peft-0.8.2/src/peft/tuners/ia3/bnb.py` & `peft-0.9.0/src/peft/tuners/ia3/bnb.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# coding=utf-8
 # Copyright 2023-present the HuggingFace Inc. team.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `peft-0.8.2/src/peft/tuners/ia3/config.py` & `peft-0.9.0/src/peft/tuners/ia3/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# coding=utf-8
 # Copyright 2023-present the HuggingFace Inc. team.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
@@ -52,15 +51,15 @@
         default=None,
         metadata={
             "help": (
                 "List of module names or regex expression of the module names to replace with (IA)³."
                 "For example, ['q', 'v'] or '.*decoder.*(SelfAttention|EncDecAttention).*(q|v)$'."
                 "This can also be a wildcard 'all-linear' which matches all linear/Conv1D layers except the output layer."
                 "If not specified, modules will be chosen according to the model architecture, If the architecture is "
-                "not known, an error will be raised -- in this case, you shoud specify the target modules manually."
+                "not known, an error will be raised -- in this case, you should specify the target modules manually."
             ),
         },
     )
     feedforward_modules: Optional[Union[List[str], str]] = field(
         default=None,
         metadata={
             "help": "List of module names or a regex expression of module names which are feedforward"
```

### Comparing `peft-0.8.2/src/peft/tuners/ia3/layer.py` & `peft-0.9.0/src/peft/tuners/ia3/layer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# coding=utf-8
 # Copyright 2023-present the HuggingFace Inc. team.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `peft-0.8.2/src/peft/tuners/ia3/model.py` & `peft-0.9.0/src/peft/tuners/ia3/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# coding=utf-8
 # Copyright 2023-present the HuggingFace Inc. team.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
@@ -14,15 +13,15 @@
 # limitations under the License.
 from __future__ import annotations
 
 import re
 import warnings
 from dataclasses import asdict
 from enum import Enum
-from typing import List, Optional
+from typing import Optional
 
 import torch
 from torch import nn
 from transformers.pytorch_utils import Conv1D
 
 from peft.import_utils import is_bnb_4bit_available, is_bnb_available
 from peft.tuners.tuners_utils import BaseTuner, BaseTunerLayer, check_target_module_exists
@@ -256,14 +255,23 @@
         When disabling all adapters, the model output corresponds to the output of the base model.
         """
         self._set_adapter_layers(enabled=False)
 
     def set_adapter(self, adapter_name: str | list[str]) -> None:
         """Set the active adapter(s).
 
+        Additionally, this function will set the specified adapters to trainable (i.e., requires_grad=True). If this is
+        not desired, use the following code.
+
+        ```py
+        >>> for name, param in model_peft.named_parameters():
+        ...     if ...:  # some check on name (ex. if 'lora' in name)
+        ...         param.requires_grad = False
+        ```
+
         Args:
             adapter_name (`str` or `list[str]`): Name of the adapter(s) to be activated.
         """
         for module in self.model.modules():
             if isinstance(module, IA3Layer):
                 if module.merged:
                     warnings.warn("Adapter cannot be set when the model is merged. Unmerging the model first.")
@@ -280,15 +288,15 @@
                 raise ValueError("Please specify `feedforward_modules` in `peft_config`")
             peft_config.feedforward_modules = TRANSFORMERS_MODELS_TO_IA3_FEEDFORWARD_MODULES_MAPPING[
                 model_config["model_type"]
             ]
         return peft_config
 
     def _unload_and_optionally_merge(
-        self, merge: bool = True, safe_merge: bool = False, adapter_names: Optional[List[str]] = None
+        self, merge: bool = True, safe_merge: bool = False, adapter_names: Optional[list[str]] = None
     ):
         r"""
         This method merges the (IA)^3 layers into the base model. This is needed if someone wants to use the base model
         as a standalone model.
 
         Args:
             safe_merge (`bool`, `optional`, defaults to `False`):
@@ -315,19 +323,25 @@
 
             if hasattr(target, "base_layer"):
                 if merge:
                     target.merge(safe_merge=safe_merge, adapter_names=adapter_names)
                 self._replace_module(parent, target_name, target.get_base_layer(), target)
             elif isinstance(target, ModulesToSaveWrapper):
                 # save any additional trainable modules part of `modules_to_save`
-                setattr(parent, target_name, target.modules_to_save[target.active_adapter])
+                new_module = target.modules_to_save[target.active_adapter]
+                if hasattr(new_module, "base_layer"):
+                    # check if the module is itself a tuner layer
+                    if merge:
+                        new_module.merge(safe_merge=safe_merge, adapter_names=adapter_names)
+                    new_module = new_module.get_base_layer()
+                setattr(parent, target_name, new_module)
 
         return self.model
 
-    def merge_and_unload(self, safe_merge: bool = False, adapter_names: Optional[List[str]] = None) -> torch.nn.Module:
+    def merge_and_unload(self, safe_merge: bool = False, adapter_names: Optional[list[str]] = None) -> torch.nn.Module:
         r"""
         This method merges the IA³ layers into the base model. This is needed if someone wants to use the base model as
         a standalone model.
 
         Args:
             safe_merge (`bool`):
                 whether to activate the safe merging check to check if there is any potential Nan in the adapter
```

### Comparing `peft-0.8.2/src/peft/tuners/loha/__init__.py` & `peft-0.9.0/src/peft/tuners/lokr/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,21 +1,20 @@
-# coding=utf-8
 # Copyright 2023-present the HuggingFace Inc. team.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from .config import LoHaConfig
-from .layer import Conv2d, Linear, LoHaLayer
-from .model import LoHaModel
+from .config import LoKrConfig
+from .layer import Conv2d, Linear, LoKrLayer
+from .model import LoKrModel
 
 
-__all__ = ["LoHaConfig", "LoHaModel", "Conv2d", "Linear", "LoHaLayer"]
+__all__ = ["LoKrConfig", "LoKrModel", "Conv2d", "Linear", "LoKrLayer"]
```

### Comparing `peft-0.8.2/src/peft/tuners/loha/config.py` & `peft-0.9.0/src/peft/tuners/loha/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# coding=utf-8
 # Copyright 2023-present the HuggingFace Inc. team.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `peft-0.8.2/src/peft/tuners/loha/layer.py` & `peft-0.9.0/src/peft/tuners/loha/layer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# coding=utf-8
 # Copyright 2023-present the HuggingFace Inc. team.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `peft-0.8.2/src/peft/tuners/loha/model.py` & `peft-0.9.0/src/peft/tuners/loha/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# coding=utf-8
 # Copyright 2023-present the HuggingFace Inc. team.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
@@ -98,15 +97,15 @@
     ) -> None:
         """
         A private method to create and replace the target module with the adapter module.
         """
 
         # Regexp matching - Find key which matches current target_name in patterns provided
         pattern_keys = list(chain(config.rank_pattern.keys(), config.alpha_pattern.keys()))
-        target_name_key = next(filter(lambda key: re.match(f"(.*\.)?{key}$", current_key), pattern_keys), target_name)
+        target_name_key = next(filter(lambda key: re.match(rf"(.*\.)?{key}$", current_key), pattern_keys), target_name)
 
         kwargs = config.to_dict()
         kwargs["r"] = config.rank_pattern.get(target_name_key, config.r)
         kwargs["alpha"] = config.alpha_pattern.get(target_name_key, config.alpha)
 
         if isinstance(target, LoHaLayer):
             target.update_layer(adapter_name, **kwargs)
```

### Comparing `peft-0.8.2/src/peft/tuners/lokr/__init__.py` & `peft-0.9.0/src/peft/tuners/poly/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,21 +1,20 @@
-# coding=utf-8
 # Copyright 2023-present the HuggingFace Inc. team.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from .config import LoKrConfig
-from .layer import Conv2d, Linear, LoKrLayer
-from .model import LoKrModel
+from .config import PolyConfig
+from .layer import Linear, PolyLayer
+from .model import PolyModel
 
 
-__all__ = ["LoKrConfig", "LoKrModel", "Conv2d", "Linear", "LoKrLayer"]
+__all__ = ["Linear", "PolyConfig", "PolyLayer", "PolyModel"]
```

### Comparing `peft-0.8.2/src/peft/tuners/lokr/config.py` & `peft-0.9.0/src/peft/tuners/lokr/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# coding=utf-8
 # Copyright 2023-present the HuggingFace Inc. team.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `peft-0.8.2/src/peft/tuners/lokr/layer.py` & `peft-0.9.0/src/peft/tuners/lokr/layer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# coding=utf-8
 # Copyright 2023-present the HuggingFace Inc. team.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `peft-0.8.2/src/peft/tuners/lokr/model.py` & `peft-0.9.0/src/peft/tuners/lokr/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# coding=utf-8
 # Copyright 2023-present the HuggingFace Inc. team.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
@@ -99,15 +98,15 @@
     ) -> None:
         """
         A private method to create and replace the target module with the adapter module.
         """
 
         # Regexp matching - Find key which matches current target_name in patterns provided
         pattern_keys = list(chain(config.rank_pattern.keys(), config.alpha_pattern.keys()))
-        target_name_key = next(filter(lambda key: re.match(f"(.*\.)?{key}$", current_key), pattern_keys), target_name)
+        target_name_key = next(filter(lambda key: re.match(rf"(.*\.)?{key}$", current_key), pattern_keys), target_name)
 
         kwargs = config.to_dict()
         kwargs["r"] = config.rank_pattern.get(target_name_key, config.r)
         kwargs["alpha"] = config.alpha_pattern.get(target_name_key, config.alpha)
 
         if isinstance(target, LoKrLayer):
             target.update_layer(adapter_name, **kwargs)
```

### Comparing `peft-0.8.2/src/peft/tuners/lora/__init__.py` & `peft-0.9.0/src/peft/tuners/lora/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# coding=utf-8
 # Copyright 2023-present the HuggingFace Inc. team.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `peft-0.8.2/src/peft/tuners/lora/bnb.py` & `peft-0.9.0/src/peft/tuners/lora/bnb.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# coding=utf-8
 # Copyright 2023-present the HuggingFace Inc. team.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
@@ -35,21 +34,33 @@
             base_layer: torch.nn.Module,
             adapter_name: str,
             r: int = 0,
             lora_alpha: int = 1,
             lora_dropout: float = 0.0,
             init_lora_weights: bool = True,
             use_rslora: bool = False,
+            use_dora: bool = False,
             **kwargs,
         ) -> None:
             super().__init__()
             LoraLayer.__init__(self, base_layer)
 
+            if use_dora:
+                raise ValueError(f"{self.__class__.__name__} does not support DoRA yet, please set it to False")
+
             self._active_adapter = adapter_name
-            self.update_layer(adapter_name, r, lora_alpha, lora_dropout, init_lora_weights, use_rslora)
+            self.update_layer(
+                adapter_name,
+                r,
+                lora_alpha=lora_alpha,
+                lora_dropout=lora_dropout,
+                init_lora_weights=init_lora_weights,
+                use_rslora=use_rslora,
+                use_dora=use_dora,
+            )
 
         def merge(self, safe_merge: bool = False, adapter_names: Optional[List[str]] = None) -> None:
             """
             Merge the active adapter weights into the base weights
 
             Args:
                 safe_merge (`bool`, *optional*):
@@ -168,15 +179,15 @@
                         compute_dtype = lora_A.weight.dtype
                         if x.dtype != compute_dtype:
                             x = x.to(compute_dtype)
                     output = lora_B(lora_A(dropout(x)))
                     if requires_conversion:
                         output = output.to(expected_dtype)
                     output = output * scaling
-                    result += output
+                    result = result + output
 
             return result
 
         def __repr__(self) -> str:
             rep = super().__repr__()
             return "lora." + rep
 
@@ -213,21 +224,33 @@
             base_layer: torch.nn.Module,
             adapter_name: str,
             r: int = 0,
             lora_alpha: int = 1,
             lora_dropout: float = 0.0,
             init_lora_weights: bool = True,
             use_rslora: bool = False,
+            use_dora: bool = False,
             **kwargs,
         ) -> None:
             super().__init__()
             LoraLayer.__init__(self, base_layer)
 
+            if use_dora:
+                raise ValueError(f"{self.__class__.__name__} does not support DoRA yet, please set it to False")
+
             self._active_adapter = adapter_name
-            self.update_layer(adapter_name, r, lora_alpha, lora_dropout, init_lora_weights, use_rslora)
+            self.update_layer(
+                adapter_name,
+                r,
+                lora_alpha=lora_alpha,
+                lora_dropout=lora_dropout,
+                init_lora_weights=init_lora_weights,
+                use_rslora=use_rslora,
+                use_dora=use_dora,
+            )
 
         def merge(self, safe_merge: bool = False, adapter_names: Optional[List[str]] = None) -> None:
             """
             Merge the active adapter weights into the base weights
 
             Args:
                 safe_merge (`bool`, *optional*):
@@ -329,15 +352,15 @@
                         expected_dtype = result.dtype
                         x = x.to(lora_A.weight.dtype)
 
                     output = lora_B(lora_A(dropout(x)))
                     if requires_conversion:
                         output = output.to(expected_dtype)
                     output = output * scaling
-                    result += output
+                    result = result + output
 
             return result
 
         def __repr__(self) -> str:
             rep = super().__repr__()
             return "lora." + rep
```

### Comparing `peft-0.8.2/src/peft/tuners/lora/config.py` & `peft-0.9.0/src/peft/tuners/lora/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# coding=utf-8
 # Copyright 2023-present the HuggingFace Inc. team.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
@@ -12,15 +11,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from __future__ import annotations
 
 from dataclasses import dataclass, field
-from typing import List, Literal, Optional, Union
+from typing import Literal, Optional, Union
 
 from peft.config import PeftConfig
 from peft.utils import PeftType
 
 
 @dataclass
 class LoftQConfig:
@@ -98,26 +97,33 @@
             parameter when you want to apply LoRA to the ColumnParallelLinear and RowParallelLinear layers of megatron.
         megatron_core (`Optional[str]`):
             The core module from Megatron to use, defaults to `"megatron.core"`.
         loftq_config (`Optional[LoftQConfig]`):
             The configuration of LoftQ. If this is not None, then LoftQ will be used to quantize the backbone weights
             and initialize Lora layers. Also pass `init_lora_weights='loftq'`. Note that you should not pass a
             quantized model in this case, as LoftQ will quantize the model itself.
+        use_dora (`bool`):
+            Enable 'Weight-Decomposed Low-Rank Adaptation' (DoRA). This technique decomposes the updates of the weights
+            into two parts, magnitude and direction. Direction is handled by normal LoRA, whereas the magnitude is
+            handled by a separate learnable parameter. This can improve the performance of LoRA, especially at low
+            ranks. Right now, DoRA only supports non-quantized linear layers. DoRA introduces a bigger overhead than
+            pure LoRA, so it is recommended to merge weights for inference. For more information, see
+            https://arxiv.org/abs/2402.09353.
     """
 
     r: int = field(default=8, metadata={"help": "Lora attention dimension"})
-    target_modules: Optional[Union[List[str], str]] = field(
+    target_modules: Optional[Union[list[str], str]] = field(
         default=None,
         metadata={
             "help": (
                 "List of module names or regex expression of the module names to replace with LoRA."
                 "For example, ['q', 'v'] or '.*decoder.*(SelfAttention|EncDecAttention).*(q|v)$'."
                 "This can also be a wildcard 'all-linear' which matches all linear/Conv1D layers except the output layer."
                 "If not specified, modules will be chosen according to the model architecture, If the architecture is "
-                "not known, an error will be raised -- in this case, you shoud specify the target modules manually."
+                "not known, an error will be raised -- in this case, you should specify the target modules manually."
             ),
         },
     )
     lora_alpha: int = field(default=8, metadata={"help": "Lora alpha"})
     lora_dropout: float = field(default=0.0, metadata={"help": "Lora dropout"})
     fan_in_fan_out: bool = field(
         default=False,
@@ -133,15 +139,15 @@
                 "When set to True, uses Rank-Stabilized LoRA doi.org/10.48550/arXiv.2312.03732"
                 " which sets the adapter scaling factor to `lora_alpha/math.sqrt(r)`, since it"
                 " was proven to work better. Otherwise, it will use the original default"
                 " value of `lora_alpha/r`."
             )
         },
     )
-    modules_to_save: Optional[List[str]] = field(
+    modules_to_save: Optional[list[str]] = field(
         default=None,
         metadata={
             "help": "List of modules apart from LoRA layers to be set as trainable and saved in the final checkpoint. "
             "For example, in Sequence Classification or Token Classification tasks, "
             "the final layer `classifier/score` are randomly initialized and as such need to be trainable and saved."
         },
     )
@@ -153,22 +159,22 @@
                 "initialization from the reference implementation from Microsoft. Passing 'gaussian' results "
                 "in Gaussian initialization scaled by the LoRA rank for linear and layers. Setting the initialization "
                 "to False leads to completely random initialization and is discouraged."
                 "Pass `'loftq'` to use LoftQ initialization"
             ),
         },
     )
-    layers_to_transform: Optional[Union[List[int], int]] = field(
+    layers_to_transform: Optional[Union[list[int], int]] = field(
         default=None,
         metadata={
             "help": "The layer indexes to transform, is this argument is specified, PEFT will transform only the layers indexes that are specified inside this list. If a single integer is passed, PEFT will transform only the layer at this index. "
             "This only works when target_modules is a list of str."
         },
     )
-    layers_pattern: Optional[Union[List[str], str]] = field(
+    layers_pattern: Optional[Union[list[str], str]] = field(
         default=None,
         metadata={
             "help": "The layer pattern name, used only if `layers_to_transform` is different to None and if the layer pattern is not in the common layers pattern."
             "This only works when target_modules is a list of str."
         },
     )
     rank_pattern: Optional[dict] = field(
@@ -221,28 +227,44 @@
         metadata={
             "help": (
                 "The configuration of LoftQ. If this is passed, then LoftQ will be used to quantize the backbone "
                 "weights and initialize Lora layers. Also set `init_lora_weights='loftq'` in this case."
             )
         },
     )
+    use_dora: bool = field(
+        default=False,
+        metadata={
+            "help": (
+                "Enable 'Weight-Decomposed Low-Rank Adaptation' (DoRA). This technique decomposes the updates of the "
+                "weights into two parts, magnitude and direction. Direction is handled by normal LoRA, whereas the "
+                "magnitude is handled by a separate learnable parameter. This can improve the performance of LoRA, "
+                "especially at low ranks. Right now, DoRA only supports non-quantized linear layers. DoRA introduces "
+                "a bigger overhead than pure LoRA, so it is recommended to merge weights for inference. For more "
+                "information, see  https://arxiv.org/abs/2402.09353."
+            )
+        },
+    )
 
     def __post_init__(self):
         self.peft_type = PeftType.LORA
         self.target_modules = (
             set(self.target_modules) if isinstance(self.target_modules, list) else self.target_modules
         )
         # if target_modules is a regex expression, then layers_to_transform should be None
         if isinstance(self.target_modules, str) and self.layers_to_transform is not None:
             raise ValueError("`layers_to_transform` cannot be used when `target_modules` is a str.")
 
         # if target_modules is a regex expression, then layers_pattern should be None
         if isinstance(self.target_modules, str) and self.layers_pattern is not None:
             raise ValueError("`layers_pattern` cannot be used when `target_modules` is a str.")
 
+        if self.use_dora and (self.megatron_config or self.init_lora_weights == "loftq"):
+            raise ValueError("DoRA does not support megatron_core or LoftQ. Please set `use_dora=False`.")
+
         # handle init_lora_weights and loftq_config
         if self.init_lora_weights == "loftq":
             import importlib
 
             if not importlib.util.find_spec("scipy"):
                 raise ImportError("The required package 'scipy' is not installed. Please install it to continue.")
             if self.loftq_config is None:
```

### Comparing `peft-0.8.2/src/peft/tuners/lora/gptq.py` & `peft-0.9.0/src/peft/tuners/lora/gptq.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# coding=utf-8
 # Copyright 2023-present the HuggingFace Inc. team.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
@@ -28,24 +27,36 @@
         base_layer,
         adapter_name: str,
         r: int = 0,
         lora_alpha: int = 1,
         lora_dropout: float = 0.0,
         init_lora_weights: bool = True,
         use_rslora: bool = False,
+        use_dora: bool = False,
         **kwargs,
     ):
         super().__init__()
         LoraLayer.__init__(self, base_layer)
 
+        if use_dora:
+            raise ValueError(f"{self.__class__.__name__} does not support DoRA yet, please set it to False")
+
         # self.base_layer and self.quant_linear_module are the same; we need the former for consistency and the latter
         # for backwards compatibility
         self.quant_linear_module = base_layer
         self._active_adapter = adapter_name
-        self.update_layer(adapter_name, r, lora_alpha, lora_dropout, init_lora_weights, use_rslora)
+        self.update_layer(
+            adapter_name,
+            r,
+            lora_alpha=lora_alpha,
+            lora_dropout=lora_dropout,
+            init_lora_weights=init_lora_weights,
+            use_rslora=use_rslora,
+            use_dora=use_dora,
+        )
 
     def forward(self, x: torch.Tensor):
         # note: logic differs from default Linear because merging is not supported
         result = self.quant_linear_module(x)
 
         if self.disable_adapters:
             return result
```

### Comparing `peft-0.8.2/src/peft/tuners/lora/layer.py` & `peft-0.9.0/src/peft/tuners/lora/layer.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# coding=utf-8
 # Copyright 2023-present the HuggingFace Inc. team.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
@@ -19,14 +18,15 @@
 
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 from transformers.pytorch_utils import Conv1D
 
 from peft.tuners.tuners_utils import BaseTunerLayer, check_adapters_to_merge
+from peft.utils.integrations import gather_params_ctx
 from peft.utils.other import transpose
 
 from .config import LoraConfig
 
 
 class LoraLayer(BaseTunerLayer):
     # All names of layers that may contain (trainable) adapter weights
@@ -44,14 +44,17 @@
         self.lora_B = nn.ModuleDict({})
         # For Embedding layer
         self.lora_embedding_A = nn.ParameterDict({})
         self.lora_embedding_B = nn.ParameterDict({})
         # Mark the weight as unmerged
         self._disable_adapters = False
         self.merged_adapters = []
+        self.use_dora: dict[str, bool] = {}
+        self.lora_magnitude_vector: Optional[torch.nn.ParameterDict] = None  # for DoRA
+        self._caches: dict[str, Any] = {}
         self.kwargs = kwargs
 
         base_layer = self.get_base_layer()
         if isinstance(base_layer, nn.Linear):
             in_features, out_features = base_layer.in_features, base_layer.out_features
         elif isinstance(base_layer, nn.Conv2d):
             in_features, out_features = base_layer.in_channels, base_layer.out_channels
@@ -63,21 +66,29 @@
             )
         elif hasattr(base_layer, "infeatures") and hasattr(base_layer, "outfeatures"):
             # QuantLinear
             in_features, out_features = base_layer.infeatures, base_layer.outfeatures
         elif hasattr(base_layer, "input_size") and hasattr(base_layer, "output_size"):
             # Megatron ColumnParallelLinear,RowParallelLinear
             in_features, out_features = base_layer.input_size, base_layer.output_size
+        elif hasattr(base_layer, "codebooks") and base_layer.__class__.__name__ == "QuantizedLinear":
+            # AQLM QuantLinear
+            in_features, out_features = base_layer.in_features, base_layer.out_features
+        elif hasattr(base_layer, "w_bit") and base_layer.__class__.__name__ == "WQLinear_GEMM":
+            # Awq layers
+            in_features, out_features = base_layer.in_features, base_layer.out_features
         else:
             raise ValueError(f"Unsupported layer type {type(base_layer)}")
 
         self.in_features = in_features
         self.out_features = out_features
 
-    def update_layer(self, adapter_name, r, lora_alpha, lora_dropout, init_lora_weights, use_rslora):
+    def update_layer(
+        self, adapter_name, r, lora_alpha, lora_dropout, init_lora_weights, use_rslora, use_dora: bool = False
+    ):
         # This code works for linear layers, override for other layer types
         if r <= 0:
             raise ValueError(f"`r` should be a positive integer value but the value passed is {r}")
 
         self.r[adapter_name] = r
         self.lora_alpha[adapter_name] = lora_alpha
         if lora_dropout > 0.0:
@@ -105,14 +116,21 @@
             if weight is not None:
                 # the layer is already completely initialized, this is an update
                 if weight.dtype.is_floating_point or weight.dtype.is_complex:
                     self.to(weight.device, dtype=weight.dtype)
                 else:
                     self.to(weight.device)
                 break
+
+        if use_dora:
+            self.dora_init(adapter_name)
+            self.use_dora[adapter_name] = True
+        else:
+            self.use_dora[adapter_name] = False
+
         self.set_adapter(self.active_adapters)
 
     def reset_lora_parameters(self, adapter_name, init_lora_weights):
         if init_lora_weights is False:
             return
 
         if adapter_name in self.lora_A.keys():
@@ -147,14 +165,73 @@
             self.lora_B[adapter_name].weight.data = lora_B
         if adapter_name in self.lora_embedding_A.keys():
             # initialize a the same way as the default for nn.linear and b to zero
             self.lora_embedding_A[adapter_name].weight.data = lora_A
             self.lora_embedding_B[adapter_name].weight.data = lora_B
         self.get_base_layer().weight.data = qweight
 
+    def _get_weight_norm(self, weight, lora_weight, scaling) -> torch.Tensor:
+        # calculate L2 norm of weight matrix, column-wise
+        weight = weight + scaling * lora_weight
+        weight_norm = torch.linalg.norm(weight, dim=1)
+        return weight_norm
+
+    def dora_init(self, adapter_name: str) -> None:
+        lora_A = self.lora_A[adapter_name]
+        lora_B = self.lora_B[adapter_name]
+        scaling = self.scaling[adapter_name]
+        with gather_params_ctx(self.get_base_layer()):
+            weight = self.get_base_layer().weight
+            lora_weight = lora_B.weight @ lora_A.weight
+            weight_norm = self._get_weight_norm(weight, lora_weight, scaling)
+        self.lora_magnitude_vector = nn.ParameterDict()
+        self.lora_magnitude_vector[adapter_name] = nn.Parameter(weight_norm, requires_grad=True)
+        # add lora_magnitude_vector to the list of learnable parameters
+        self.adapter_layer_names = self.adapter_layer_names[:] + ("lora_magnitude_vector",)
+
+    def _cache_store(self, key: str, value: Any) -> None:
+        self._caches[key] = value
+
+    def _cache_pop(self, key: str) -> Any:
+        value = self._caches.pop(key)
+        return value
+
+    def _apply_dora(self, x, lora_A, lora_B, scaling, active_adapter):
+        """
+        For DoRA, calculate the extra output from LoRA with DoRA applied. This should be added on top of the base layer
+        output.
+        """
+        lora_weight = lora_B.weight @ lora_A.weight
+        magnitude = self.lora_magnitude_vector[active_adapter]
+        weight = self.get_base_layer().weight
+        weight_norm = self._get_weight_norm(weight, lora_weight, scaling)
+        # see section 4.3 of DoRA (https://arxiv.org/abs/2402.09353)
+        # "[...] we suggest treating ||V +∆V ||_c in
+        # Eq. (5) as a constant, thereby detaching it from the gradient
+        # graph. This means that while ||V + ∆V ||_c dynamically
+        # reflects the updates of ∆V , it won’t receive any gradient
+        # during backpropagation"
+        weight_norm = weight_norm.detach()
+        mag_norm_scale = (magnitude / weight_norm).view(1, -1)
+        result_dora = (mag_norm_scale - 1) * (
+            F.linear(x, transpose(weight, self.fan_in_fan_out))
+        ) + mag_norm_scale * lora_B(lora_A(x)) * scaling
+
+        # Note: Computation could potentially be accelerated by using the code below instead of calculating X@W again.
+        # This is only correct if dropout=0, otherwise results will differ:
+        # https://github.com/huggingface/peft/pull/1474#issuecomment-1964682771
+        # bias = self.get_base_layer().bias
+        # if bias is not None:
+        #     result = result - bias
+        # result = mag_norm_scale * result + mag_norm_scale * lora_B(lora_A(x)) * scaling
+        # if bias is not None:
+        #     result = result + bias
+
+        return result_dora
+
     def set_scale(self, adapter, scale):
         if adapter not in self.scaling:
             # Ignore the case where the adapter is not in the layer
             return
         self.scaling[adapter] = scale * self.lora_alpha[adapter] / self.r[adapter]
 
     def scale_layer(self, scale: float) -> None:
@@ -197,22 +274,31 @@
         r: int = 0,
         lora_alpha: int = 1,
         lora_dropout: float = 0.0,
         fan_in_fan_out: bool = False,  # Set this to True if the layer to replace stores weight like (fan_in, fan_out)
         is_target_conv_1d_layer: bool = False,
         init_lora_weights: Union[bool, str] = True,
         use_rslora: bool = False,
+        use_dora: bool = False,
         **kwargs,
     ) -> None:
         super().__init__()
         LoraLayer.__init__(self, base_layer, **kwargs)
         self.fan_in_fan_out = fan_in_fan_out
 
         self._active_adapter = adapter_name
-        self.update_layer(adapter_name, r, lora_alpha, lora_dropout, init_lora_weights, use_rslora)
+        self.update_layer(
+            adapter_name,
+            r,
+            lora_alpha=lora_alpha,
+            lora_dropout=lora_dropout,
+            init_lora_weights=init_lora_weights,
+            use_rslora=use_rslora,
+            use_dora=use_dora,
+        )
         self.is_target_conv_1d_layer = is_target_conv_1d_layer
 
     def merge(self, safe_merge: bool = False, adapter_names: Optional[List[str]] = None) -> None:
         """
         Merge the active adapter weights into the base weights
 
         Args:
@@ -232,37 +318,71 @@
         for active_adapter in adapter_names:
             if active_adapter in self.lora_A.keys():
                 base_layer = self.get_base_layer()
                 if safe_merge:
                     # Note that safe_merge will be slower than the normal merge
                     # because of the copy operation.
                     orig_weights = base_layer.weight.data.clone()
-                    orig_weights += self.get_delta_weight(active_adapter)
+                    delta_weight = self.get_delta_weight(active_adapter)
+                    if not self.use_dora[active_adapter]:
+                        orig_weights += delta_weight
+                    else:
+                        # handle dora
+                        # since delta_weight already includes scaling, set it to 1 here
+                        weight_norm = self._get_weight_norm(orig_weights, delta_weight, scaling=1).detach()
+                        # We need to cache weight_norm because it has to be based on the original weights. We
+                        # cannot calculate it on the fly based on the merged weights when unmerging because its a
+                        # different value
+                        self._cache_store(f"{active_adapter}-weight_norm", weight_norm)
+                        dora_factor = self.lora_magnitude_vector[active_adapter] / weight_norm
+                        orig_weights = dora_factor.view(-1, 1) * (orig_weights + delta_weight)
 
                     if not torch.isfinite(orig_weights).all():
                         raise ValueError(
                             f"NaNs detected in the merged weights. The adapter {active_adapter} seems to be broken"
                         )
 
                     base_layer.weight.data = orig_weights
                 else:
-                    base_layer.weight.data += self.get_delta_weight(active_adapter)
+                    delta_weight = self.get_delta_weight(active_adapter)
+                    if not self.use_dora[active_adapter]:
+                        base_layer.weight.data += delta_weight
+                    else:
+                        # handle dora
+                        # since delta_weight already includes scaling, set it to 1 here
+                        weight_norm = self._get_weight_norm(base_layer.weight, delta_weight, scaling=1).detach()
+                        # We need to cache weight_norm because it has to be based on the original weights. We
+                        # cannot calculate it on the fly based on the merged weights when unmerging because its a
+                        # different value
+                        self._cache_store(f"{active_adapter}-weight_norm", weight_norm)
+                        dora_factor = self.lora_magnitude_vector[active_adapter] / weight_norm
+                        new_weight = dora_factor.view(-1, 1) * (base_layer.weight.data + delta_weight)
+                        base_layer.weight.data = new_weight
+
                 self.merged_adapters.append(active_adapter)
 
     def unmerge(self) -> None:
         """
         This method unmerges all merged adapter layers from the base weights.
         """
         if not self.merged:
             warnings.warn("Already unmerged. Nothing to do.")
             return
         while len(self.merged_adapters) > 0:
             active_adapter = self.merged_adapters.pop()
             if active_adapter in self.lora_A.keys():
-                self.get_base_layer().weight.data -= self.get_delta_weight(active_adapter)
+                weight = self.get_base_layer().weight
+                delta_weight = self.get_delta_weight(active_adapter)
+                if not self.use_dora[active_adapter]:
+                    weight.data -= delta_weight
+                else:
+                    weight_norm = self._cache_pop(f"{active_adapter}-weight_norm")
+                    dora_factor = self.lora_magnitude_vector[active_adapter] / weight_norm
+                    weight_orig = weight.data / dora_factor.view(-1, 1) - delta_weight
+                    weight.data = weight_orig
 
     def get_delta_weight(self, adapter) -> torch.Tensor:
         """
         Compute the delta weight for the given adapter.
 
         Args:
             adapter (str):
@@ -291,35 +411,39 @@
             # cast back the weights
             self.lora_A[adapter].weight.data = weight_A.to(dtype)
             self.lora_B[adapter].weight.data = weight_B.to(dtype)
 
         return output_tensor
 
     def forward(self, x: torch.Tensor, *args: Any, **kwargs: Any) -> torch.Tensor:
-        previous_dtype = x.dtype
-
         if self.disable_adapters:
             if self.merged:
                 self.unmerge()
             result = self.base_layer(x, *args, **kwargs)
         elif self.merged:
             result = self.base_layer(x, *args, **kwargs)
         else:
             result = self.base_layer(x, *args, **kwargs)
+            torch_result_dtype = result.dtype
             for active_adapter in self.active_adapters:
                 if active_adapter not in self.lora_A.keys():
                     continue
                 lora_A = self.lora_A[active_adapter]
                 lora_B = self.lora_B[active_adapter]
                 dropout = self.lora_dropout[active_adapter]
                 scaling = self.scaling[active_adapter]
                 x = x.to(lora_A.weight.dtype)
-                result += lora_B(lora_A(dropout(x))) * scaling
 
-        result = result.to(previous_dtype)
+                if not self.use_dora[active_adapter]:
+                    result = result + lora_B(lora_A(dropout(x))) * scaling
+                else:
+                    x = dropout(x)
+                    result = result + self._apply_dora(x, lora_A, lora_B, scaling, active_adapter)
+
+            result = result.to(torch_result_dtype)
         return result
 
     def __repr__(self) -> str:
         rep = super().__repr__()
         return "lora." + rep
 
 
@@ -330,23 +454,35 @@
         base_layer: nn.Module,
         adapter_name: str,
         r: int = 0,
         lora_alpha: int = 1,
         lora_dropout: float = 0.0,
         init_lora_weights: Union[bool, str] = True,
         use_rslora: bool = False,
+        use_dora: bool = False,
         **kwargs,
     ) -> None:
         super().__init__()
         LoraLayer.__init__(self, base_layer)
 
+        if use_dora:
+            raise ValueError(f"{self.__class__.__name__} does not support DoRA yet, please set it to False")
+
         self._active_adapter = adapter_name
-        self.update_layer(adapter_name, r, lora_alpha, lora_dropout, init_lora_weights, use_rslora)
+        self.update_layer(
+            adapter_name,
+            r,
+            lora_alpha=lora_alpha,
+            lora_dropout=lora_dropout,
+            init_lora_weights=init_lora_weights,
+            use_rslora=use_rslora,
+            use_dora=use_dora,
+        )
 
-    def update_layer(self, adapter_name, r, lora_alpha, lora_dropout, init_lora_weights, use_rslora):
+    def update_layer(self, adapter_name, r, lora_alpha, lora_dropout, init_lora_weights, use_rslora, use_dora):
         if r <= 0:
             raise ValueError(f"`r` should be a positive integer value but the value passed is {r}")
 
         self.r[adapter_name] = r
         self.lora_alpha[adapter_name] = lora_alpha
         if lora_dropout > 0.0:
             lora_dropout_layer = nn.Dropout(p=lora_dropout)
@@ -477,22 +613,24 @@
             if self.merged:
                 self.unmerge()
             result = self.base_layer(x, *args, **kwargs)
         elif self.merged:
             result = self.base_layer(x, *args, **kwargs)
         else:
             result = self.base_layer(x, *args, **kwargs)
+            torch_result_dtype = result.dtype
             for active_adapter in self.active_adapters:
                 if active_adapter not in self.lora_embedding_A:
                     continue
                 embedding_A = self.lora_embedding_A[active_adapter].T
                 embedding_B = self.lora_embedding_B[active_adapter].T
                 scaling = self.scaling[active_adapter]
                 after_A = self._embed(x, embedding_A)
                 result += (after_A @ embedding_B) * scaling
+            result = result.to(torch_result_dtype)
 
         return result
 
     def __repr__(self) -> str:
         rep = super().__repr__()
         return "lora." + rep
 
@@ -504,23 +642,35 @@
         base_layer: nn.Module,
         adapter_name: str,
         r: int = 0,
         lora_alpha: int = 1,
         lora_dropout: float = 0.0,
         init_lora_weights: Union[bool, str] = True,
         use_rslora: bool = False,
+        use_dora: bool = False,
         **kwargs,
     ) -> None:
         super().__init__()
         LoraLayer.__init__(self, base_layer)
 
+        if use_dora:
+            raise ValueError(f"{self.__class__.__name__} does not support DoRA yet, please set it to False")
+
         self._active_adapter = adapter_name
-        self.update_layer(adapter_name, r, lora_alpha, lora_dropout, init_lora_weights, use_rslora)
+        self.update_layer(
+            adapter_name,
+            r,
+            lora_alpha=lora_alpha,
+            lora_dropout=lora_dropout,
+            init_lora_weights=init_lora_weights,
+            use_rslora=use_rslora,
+            use_dora=use_dora,
+        )
 
-    def update_layer(self, adapter_name, r, lora_alpha, lora_dropout, init_lora_weights, use_rslora):
+    def update_layer(self, adapter_name, r, lora_alpha, lora_dropout, init_lora_weights, use_rslora, use_dora):
         if r <= 0:
             raise ValueError(f"`r` should be a positive integer value but the value passed is {r}")
 
         self.r[adapter_name] = r
         self.lora_alpha[adapter_name] = lora_alpha
         if lora_dropout > 0.0:
             lora_dropout_layer = nn.Dropout(p=lora_dropout)
@@ -644,35 +794,35 @@
             # cast back the weights
             self.lora_A[adapter].weight.data = weight_A.to(dtype)
             self.lora_B[adapter].weight.data = weight_B.to(dtype)
 
         return output_tensor
 
     def forward(self, x: torch.Tensor, *args, **kwargs) -> torch.Tensor:
-        previous_dtype = x.dtype
-
         if self.disable_adapters:
             if self.merged:
                 self.unmerge()
             result = self.base_layer(x, *args, **kwargs)
         elif self.merged:
             result = self.base_layer(x, *args, **kwargs)
         else:
             result = self.base_layer(x, *args, **kwargs)
+            torch_result_dtype = result.dtype
+
             for active_adapter in self.active_adapters:
                 if active_adapter not in self.lora_A.keys():
                     continue
                 lora_A = self.lora_A[active_adapter]
                 lora_B = self.lora_B[active_adapter]
                 dropout = self.lora_dropout[active_adapter]
                 scaling = self.scaling[active_adapter]
                 x = x.to(lora_A.weight.dtype)
                 result += lora_B(lora_A(dropout(x))) * scaling
 
-        result = result.to(previous_dtype)
+            result = result.to(torch_result_dtype)
         return result
 
     def __repr__(self) -> str:
         rep = super().__repr__()
         return "lora." + rep
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `peft-0.8.2/src/peft/tuners/lora/model.py` & `peft-0.9.0/src/peft/tuners/lora/model.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# coding=utf-8
 # Copyright 2023-present the HuggingFace Inc. team.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
@@ -18,30 +17,33 @@
 import operator
 import re
 import warnings
 from dataclasses import asdict, replace
 from enum import Enum
 from functools import reduce
 from itertools import chain
-from typing import List, Optional
+from typing import Literal, Optional
 
 import torch
 from torch import nn
 from tqdm import tqdm
 
 from peft.import_utils import is_bnb_4bit_available, is_bnb_available
 from peft.tuners.tuners_utils import BaseTuner, BaseTunerLayer, check_target_module_exists, onload_layer
 from peft.utils import (
     TRANSFORMERS_MODELS_TO_LORA_TARGET_MODULES_MAPPING,
     ModulesToSaveWrapper,
     _freeze_adapter,
     _get_submodules,
     get_quantization_config,
 )
+from peft.utils.merge_utils import dare_linear, dare_ties, magnitude_prune, task_arithmetic, ties
 
+from .aqlm import dispatch_aqlm
+from .awq import dispatch_awq
 from .config import LoraConfig
 from .gptq import dispatch_gptq
 from .layer import Conv2d, LoraLayer, dispatch_default
 from .tp_layer import dispatch_megatron
 
 
 class LoraModel(BaseTuner):
@@ -137,44 +139,48 @@
         current_key,
     ):
         if current_key is None:
             raise ValueError("Current Key shouldn't be `None`")
 
         # Regexp matching - Find key which matches current target_name in patterns provided
         pattern_keys = list(chain(lora_config.rank_pattern.keys(), lora_config.alpha_pattern.keys()))
-        target_name_key = next(filter(lambda key: re.match(f".*\.{key}$", current_key), pattern_keys), current_key)
+        target_name_key = next(filter(lambda key: re.match(rf".*\.{key}$", current_key), pattern_keys), current_key)
         r = lora_config.rank_pattern.get(target_name_key, lora_config.r)
         alpha = lora_config.alpha_pattern.get(target_name_key, lora_config.lora_alpha)
 
         kwargs = {
             "r": r,
             "lora_alpha": alpha,
             "lora_dropout": lora_config.lora_dropout,
             "fan_in_fan_out": lora_config.fan_in_fan_out,
             "init_lora_weights": lora_config.init_lora_weights,
             "use_rslora": lora_config.use_rslora,
+            "use_dora": lora_config.use_dora,
             "loaded_in_8bit": getattr(self.model, "is_loaded_in_8bit", False),
             "loaded_in_4bit": getattr(self.model, "is_loaded_in_4bit", False),
         }
 
-        quantization_config = get_quantization_config(self.model, method="gptq")
-        if quantization_config is not None:
-            kwargs["gptq_quantization_config"] = quantization_config
+        quant_methods = ["gptq", "aqlm", "awq"]
+        for quant_method in quant_methods:
+            quantization_config = get_quantization_config(self.model, method=quant_method)
+            if quantization_config is not None:
+                kwargs[f"{quant_method}_quantization_config"] = quantization_config
 
         # note: AdaLoraLayer is a subclass of LoraLayer, we need to exclude it
         from peft.tuners.adalora import AdaLoraLayer
 
         if isinstance(target, LoraLayer) and not isinstance(target, AdaLoraLayer):
             target.update_layer(
                 adapter_name,
                 r,
-                alpha,
-                lora_config.lora_dropout,
-                lora_config.init_lora_weights,
-                lora_config.use_rslora,
+                lora_alpha=alpha,
+                lora_dropout=lora_config.lora_dropout,
+                init_lora_weights=lora_config.init_lora_weights,
+                use_rslora=lora_config.use_rslora,
+                use_dora=lora_config.use_dora,
             )
         else:
             new_module = self._create_new_module(lora_config, adapter_name, target, **kwargs)
             if adapter_name != self.active_adapter:
                 # adding an additional adapter: it is not automatically trainable
                 new_module.requires_grad_(False)
             self._replace_module(parent, target_name, new_module, target)
@@ -240,15 +246,15 @@
             dispatchers.append(dispatch_bnb_8bit)
 
         if is_bnb_4bit_available():
             from .bnb import dispatch_bnb_4bit
 
             dispatchers.append(dispatch_bnb_4bit)
 
-        dispatchers.extend([dispatch_gptq, dispatch_megatron, dispatch_default])
+        dispatchers.extend([dispatch_aqlm, dispatch_awq, dispatch_gptq, dispatch_megatron, dispatch_default])
 
         new_module = None
         for dispatcher in dispatchers:
             new_module = dispatcher(target, adapter_name, lora_config=lora_config, **kwargs)
             if new_module is not None:  # first match wins
                 break
 
@@ -303,14 +309,23 @@
                 )
                 warnings.warn(msg)
         self._set_adapter_layers(enabled=False)
 
     def set_adapter(self, adapter_name: str | list[str]) -> None:
         """Set the active adapter(s).
 
+        Additionally, this function will set the specified adapters to trainable (i.e., requires_grad=True). If this is
+        not desired, use the following code.
+
+        ```py
+        >>> for name, param in model_peft.named_parameters():
+        ...     if ...:  # some check on name (ex. if 'lora' in name)
+        ...         param.requires_grad = False
+        ```
+
         Args:
             adapter_name (`str` or `list[str]`): Name of the adapter(s) to be activated.
         """
         for module in self.model.modules():
             if isinstance(module, LoraLayer):
                 if module.merged:
                     warnings.warn("Adapter cannot be set when the model is merged. Unmerging the model first.")
@@ -329,15 +344,15 @@
         return peft_config
 
     def _unload_and_optionally_merge(
         self,
         merge=True,
         progressbar: bool = False,
         safe_merge: bool = False,
-        adapter_names: Optional[List[str]] = None,
+        adapter_names: Optional[list[str]] = None,
     ):
         if merge:
             if getattr(self.model, "quantization_method", None) == "gptq":
                 raise ValueError("Cannot merge LORA layers when the model is gptq quantized")
 
         key_list = [key for key, _ in self.model.named_modules() if self.prefix not in key]
         desc = "Unloading " + ("and merging " if merge else "") + "model"
@@ -349,28 +364,36 @@
             with onload_layer(target):
                 if hasattr(target, "base_layer"):
                     if merge:
                         target.merge(safe_merge=safe_merge, adapter_names=adapter_names)
                     self._replace_module(parent, target_name, target.get_base_layer(), target)
                 elif isinstance(target, ModulesToSaveWrapper):
                     # save any additional trainable modules part of `modules_to_save`
-                    setattr(parent, target_name, target.modules_to_save[target.active_adapter])
+                    new_module = target.modules_to_save[target.active_adapter]
+                    if hasattr(new_module, "base_layer"):
+                        # check if the module is itself a tuner layer
+                        if merge:
+                            new_module.merge(safe_merge=safe_merge, adapter_names=adapter_names)
+                        new_module = new_module.get_base_layer()
+                    setattr(parent, target_name, new_module)
 
         return self.model
 
     def add_weighted_adapter(
         self,
         adapters,
         weights,
         adapter_name,
         combination_type="svd",
         svd_rank=None,
         svd_clamp=None,
         svd_full_matrices=True,
         svd_driver=None,
+        density=None,
+        majority_sign_method: Literal["total", "frequency"] = "total",
     ) -> None:
         """
         This method adds a new adapter by merging the given adapters with the given weights.
 
         When using the `cat` combination_type you should be aware that rank of the resulting adapter will be equal to
         the sum of all adapters ranks. So it's possible that the mixed adapter may become too big and result in OOM
         errors.
@@ -379,51 +402,61 @@
             adapters (`list`):
                 List of adapter names to be merged.
             weights (`list`):
                 List of weights for each adapter.
             adapter_name (`str`):
                 Name of the new adapter.
             combination_type (`str`):
-                Type of merging. Can be one of [`svd`, `linear`, `cat`]. When using the `cat` combination_type you
-                should be aware that rank of the resulting adapter will be equal to the sum of all adapters ranks. So
-                it's possible that the mixed adapter may become too big and result in OOM errors.
+                The merging type can be one of [`svd`, `linear`, `cat`, `ties`, `ties_svd`, `dare_ties`, `dare_linear`,
+                `dare_ties_svd`, `dare_linear_svd`, `magnitude_prune`, `magnitude_prune_svd`]. When using the `cat`
+                combination_type, the rank of the resulting adapter is equal to the sum of all adapters ranks (the
+                mixed adapter may be too big and result in OOM errors).
             svd_rank (`int`, *optional*):
                 Rank of output adapter for svd. If None provided, will use max rank of merging adapters.
             svd_clamp (`float`, *optional*):
                 A quantile threshold for clamping SVD decomposition output. If None is provided, do not perform
                 clamping. Defaults to None.
             svd_full_matrices (`bool`, *optional*):
                 Controls whether to compute the full or reduced SVD, and consequently, the shape of the returned
                 tensors U and Vh. Defaults to True.
             svd_driver (`str`, *optional*):
                 Name of the cuSOLVER method to be used. This keyword argument only works when merging on CUDA. Can be
                 one of [None, `gesvd`, `gesvdj`, `gesvda`]. For more info please refer to `torch.linalg.svd`
                 documentation. Defaults to None.
+            density (`float`, *optional*):
+                Value between 0 and 1. 0 means all values are pruned and 1 means no values are pruned. Should be used
+                with [`ties`, `ties_svd`, `dare_ties`, `dare_linear`, `dare_ties_svd`, `dare_linear_svd`,
+                `magnintude_prune`, `magnitude_prune_svd`]
+            majority_sign_method (`str`):
+                The method, should be one of ["total", "frequency"], to use to get the magnitude of the sign values.
+                Should be used with [`ties`, `ties_svd`, `dare_ties`, `dare_ties_svd`]
         """
 
         if adapter_name in list(self.peft_config.keys()):
             return
         for adapter in adapters:
             if adapter not in list(self.peft_config.keys()):
                 raise ValueError(f"Adapter {adapter} does not exist")
 
         # if there is only one adapter, we can only use linear merging
         combination_type = "linear" if len(adapters) == 1 else combination_type
 
         adapters_ranks = [self.peft_config[adapter].r for adapter in adapters]
-        if combination_type == "linear":
+        if combination_type in ("linear", "ties", "dare_ties", "dare_linear", "magnitude_prune"):
             # all adapters ranks should be same, new rank is just this value
             if len(set(adapters_ranks)) != 1:
-                raise ValueError("All adapters must have the same r value when using `linear` combination_type")
+                raise ValueError(
+                    "All adapters must have the same r value when using combination_type linear, ties, dare_ties or dare_linear."
+                )
             new_rank = adapters_ranks[0]
         elif combination_type == "cat":
             # adapters ranks may be different, new rank is sum of all ranks
             # be careful, because output adapter rank may be really big if mixing a lot of adapters
             new_rank = sum(adapters_ranks)
-        elif combination_type == "svd":
+        elif combination_type.endswith("svd"):
             # new rank is the max of all ranks of the adapters if not provided
             new_rank = svd_rank or max(adapters_ranks)
         else:
             raise ValueError(f"Invalid combination_type: {combination_type}")
 
         target_module_types = [type(self.peft_config[adapter].target_modules) for adapter in adapters]
         if not target_module_types:
@@ -465,93 +498,109 @@
                     target_lora_A = target.lora_embedding_A[adapter_name]
                     target_lora_B = target.lora_embedding_B[adapter_name]
                 else:
                     continue
 
                 target_lora_A.data = target_lora_A.data * 0.0
                 target_lora_B.data = target_lora_B.data * 0.0
-                if combination_type == "linear":
-                    for adapter, weight in zip(adapters, weights):
-                        if adapter in target.lora_A:
-                            current_adapter_lora_A = target.lora_A[adapter].weight
-                            current_adapter_lora_B = target.lora_B[adapter].weight
-                        elif adapter in target.lora_embedding_A:
-                            current_adapter_lora_A = target.lora_embedding_A[adapter]
-                            current_adapter_lora_B = target.lora_embedding_B[adapter]
-                        else:
-                            continue
-                        target_lora_A.data += current_adapter_lora_A.data * math.sqrt(weight) * target.scaling[adapter]
-                        target_lora_B.data += current_adapter_lora_B.data * math.sqrt(weight)
-                elif combination_type == "cat":
+                if combination_type == "cat":
                     loras_A, loras_B = [], []
                     for adapter, weight in zip(adapters, weights):
                         if adapter in target.lora_A:
                             current_adapter_lora_A = target.lora_A[adapter].weight
                             current_adapter_lora_B = target.lora_B[adapter].weight
                         elif adapter in target.lora_embedding_A:
                             current_adapter_lora_A = target.lora_embedding_A[adapter]
                             current_adapter_lora_B = target.lora_embedding_B[adapter]
                         else:
                             continue
                         loras_A.append(current_adapter_lora_A.data * weight * target.scaling[adapter])
                         loras_B.append(current_adapter_lora_B.data)
 
                     if len(loras_A) == 0:
-                        raise ValueError("No matching LoRAs found. Please raise an issue on Github.")
+                        raise ValueError("No matching LoRAs found. Please raise an issue on GitHub.")
                     loras_A = torch.cat(loras_A, dim=0)
                     loras_B = torch.cat(loras_B, dim=1)
                     target_lora_A.data[: loras_A.shape[0], :] = loras_A
                     target_lora_B.data[:, : loras_B.shape[1]] = loras_B
-                elif combination_type == "svd":
-                    target_lora_A.data, target_lora_B.data = self._svd_weighted_adapter(
+                elif combination_type in [
+                    "svd",
+                    "ties_svd",
+                    "dare_linear_svd",
+                    "dare_ties_svd",
+                    "magnitude_prune_svd",
+                ]:
+                    target_lora_A.data, target_lora_B.data = self._svd_generalized_task_arithmetic_weighted_adapter(
+                        combination_type,
                         adapters,
                         weights,
                         new_rank,
                         target,
                         target_lora_A,
                         target_lora_B,
+                        density,
+                        majority_sign_method,
                         svd_clamp,
                         full_matrices=svd_full_matrices,
                         driver=svd_driver,
                     )
+                elif combination_type in ["linear", "ties", "dare_linear", "dare_ties", "magnitude_prune"]:
+                    target_lora_A.data, target_lora_B.data = self._generalized_task_arithmetic_weighted_adapter(
+                        combination_type, adapters, weights, target, density, majority_sign_method
+                    )
 
-    def _svd_weighted_adapter(
+    def _svd_generalized_task_arithmetic_weighted_adapter(
         self,
+        combination_type,
         adapters,
         weights,
         new_rank,
         target,
         target_lora_A,
         target_lora_B,
+        density,
+        majority_sign_method,
         clamp=None,
         full_matrices=True,
         driver=None,
     ):
         valid_adapters = []
         valid_weights = []
+        is_embedding = any(adapter in target.lora_embedding_A for adapter in adapters)
         for adapter, weight in zip(adapters, weights):
             if adapter in target.lora_A or adapter in target.lora_embedding_A:
                 valid_adapters.append(adapter)
-                valid_weights.append(weight)
+                valid_weights.append(weight * target.scaling[adapter])
 
         # if no valid adapter, nothing to do
         if len(valid_adapters) == 0:
             raise ValueError("No matching LoRAs found. Please raise an issue on Github.")
+        delta_weight = [target.get_delta_weight(adapter) for adapter in valid_adapters]
+        valid_weights = torch.tensor(valid_weights).to(delta_weight[0].device)
+        if combination_type == "svd":
+            delta_weight = task_arithmetic(delta_weight, valid_weights)
+        elif combination_type == "ties_svd":
+            delta_weight = ties(delta_weight, valid_weights, density, majority_sign_method)
+        elif combination_type == "dare_linear_svd":
+            delta_weight = dare_linear(delta_weight, valid_weights, density)
+        elif combination_type == "dare_ties_svd":
+            delta_weight = dare_ties(delta_weight, valid_weights, density, majority_sign_method)
+        elif combination_type == "magnitude_prune_svd":
+            delta_weight = magnitude_prune(delta_weight, valid_weights, density)
+        else:
+            raise ValueError(f"Invalid value passed to combination type: {combination_type}")
 
-        delta_weight = valid_weights[0] * target.get_delta_weight(valid_adapters[0])
-        for adapter, weight in zip(valid_adapters[1:], valid_weights[1:]):
-            delta_weight += weight * target.get_delta_weight(adapter)
         conv2d = isinstance(target, Conv2d)
         if conv2d:
             conv2d_1x1 = target.weight.size()[2:4] == (1, 1)
             if not conv2d_1x1:
                 delta_weight = delta_weight.flatten(start_dim=1)
             else:
                 delta_weight = delta_weight.squeeze()
-        if hasattr(target, "fan_in_fan_out") and target.fan_in_fan_out:
+        if (hasattr(target, "fan_in_fan_out") and target.fan_in_fan_out) or is_embedding:
             delta_weight = delta_weight.T
 
         # based on https://github.com/kohya-ss/sd-scripts/blob/main/networks/svd_merge_lora.py#L114-L131
         U, S, Vh = torch.linalg.svd(delta_weight, full_matrices=full_matrices, driver=driver)
         U = U[:, :new_rank]
         S = S[:new_rank]
         U = U @ torch.diag(S)
@@ -563,14 +612,58 @@
             U = U.clamp(low_val, hi_val)
             Vh = Vh.clamp(low_val, hi_val)
         if conv2d:
             U = U.reshape(target_lora_B.data.shape)
             Vh = Vh.reshape(target_lora_A.data.shape)
         return Vh, U
 
+    def _generalized_task_arithmetic_weighted_adapter(
+        self,
+        combination_type,
+        adapters,
+        weights,
+        target,
+        density,
+        majority_sign_method,
+    ):
+        # account weights for LoRA A and B layers.
+        valid_weights = []
+        lora_A_deltas = []
+        lora_B_deltas = []
+        for adapter, weight in zip(adapters, weights):
+            if adapter in target.lora_A:
+                current_adapter_lora_A = target.lora_A[adapter].weight
+                current_adapter_lora_B = target.lora_B[adapter].weight
+            elif adapter in target.lora_embedding_A:
+                current_adapter_lora_A = target.lora_embedding_A[adapter]
+                current_adapter_lora_B = target.lora_embedding_B[adapter]
+            else:
+                continue
+            valid_weights.append(math.sqrt(weight * target.scaling[adapter]))
+            lora_A_deltas.append(current_adapter_lora_A.data)
+            lora_B_deltas.append(current_adapter_lora_B.data)
+        valid_weights = torch.tensor(valid_weights).to(lora_A_deltas[0].device)
+        lora_deltas = [lora_A_deltas, lora_B_deltas]
+        dtype = lora_A_deltas[0].dtype
+        for i, task_tensors in enumerate(lora_deltas):
+            if combination_type == "linear":
+                lora_deltas[i] = task_arithmetic(task_tensors, valid_weights)
+            elif combination_type == "ties":
+                lora_deltas[i] = ties(task_tensors, valid_weights, density, majority_sign_method)
+            elif combination_type == "dare_linear":
+                lora_deltas[i] = dare_linear(task_tensors, valid_weights, density)
+            elif combination_type == "dare_ties":
+                lora_deltas[i] = dare_ties(task_tensors, valid_weights, density, majority_sign_method)
+            elif combination_type == "magnitude_prune":
+                lora_deltas[i] = magnitude_prune(task_tensors, valid_weights, density)
+            else:
+                raise ValueError("Invalid combination type")
+        lora_deltas = [delta.to(dtype) for delta in lora_deltas]
+        return lora_deltas
+
     def delete_adapter(self, adapter_name: str) -> None:
         """
         Deletes an existing adapter.
 
         Args:
             adapter_name (str): Name of the adapter to be deleted.
         """
@@ -586,15 +679,15 @@
                 target.delete_adapter(adapter_name)
                 if new_adapter is None:
                     new_adapter = target.active_adapters[:]
 
         self.active_adapter = new_adapter or []
 
     def merge_and_unload(
-        self, progressbar: bool = False, safe_merge: bool = False, adapter_names: Optional[List[str]] = None
+        self, progressbar: bool = False, safe_merge: bool = False, adapter_names: Optional[list[str]] = None
     ) -> torch.nn.Module:
         r"""
         This method merges the LoRa layers into the base model. This is needed if someone wants to use the base model
         as a standalone model.
 
         Args:
             progressbar (`bool`):
```

### Comparing `peft-0.8.2/src/peft/tuners/lora/tp_layer.py` & `peft-0.9.0/src/peft/tuners/lora/tp_layer.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# coding=utf-8
 # Copyright 2023-present the HuggingFace Inc. team.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
@@ -41,21 +40,25 @@
         backend,
         r: int = 0,
         lora_alpha: int = 1,
         lora_dropout: float = 0.0,
         fan_in_fan_out: bool = False,
         init_lora_weights: bool = True,
         use_rslora: bool = False,
+        use_dora: bool = False,
         **kwargs,
     ):
         super().__init__()
         LoraLayer.__init__(self, base_layer=base_layer)
 
+        if use_dora:
+            raise ValueError(f"{self.__class__.__name__} does not support DoRA yet, please set it to False")
+
         self.backend = backend
-        self.is_paralle_a = isinstance(base_layer, backend.RowParallelLinear)
+        self.is_parallel_a = isinstance(base_layer, backend.RowParallelLinear)
         self.fan_in_fan_out = fan_in_fan_out
         self._active_adapter = adapter_name
 
         megatron_config = kwargs["megatron_config"]
         parallel_linear_kwargs = {"megatron_config": megatron_config}
         init_method = init.xavier_normal_
         if hasattr(megatron_config, "init_method"):
@@ -65,34 +68,45 @@
         if isinstance(base_layer, self.backend.RowParallelLinear):
             input_is_parallel = base_layer.input_is_parallel
         else:
             gather_output = base_layer.gather_output
         self.update_layer(
             adapter_name,
             r,
-            lora_alpha,
-            lora_dropout,
-            init_lora_weights,
-            use_rslora,
-            init_method,
-            input_is_parallel,
-            gather_output,
+            lora_alpha=lora_alpha,
+            lora_dropout=lora_dropout,
+            init_lora_weights=init_lora_weights,
+            use_rslora=use_rslora,
+            use_dora=use_dora,
+            init_method=init_method,
+            input_is_parallel=input_is_parallel,
+            gather_output=gather_output,
             **parallel_linear_kwargs,
         )
 
         self.is_target_conv_1d_layer = False
 
+    @property
+    def is_paralle_a(self):
+        # TODO: remove it in PEFT 0.10.0
+        # See https://github.com/huggingface/peft/pull/1439 for more details
+        warnings.warn(
+            "`is_paralle_a` is going to be deprecated in a future release. Please use `is_parallel_a`", FutureWarning
+        )
+        return self.is_parallel_a
+
     def update_layer(
         self,
         adapter_name,
         r,
         lora_alpha,
         lora_dropout,
         init_lora_weights,
         use_rslora,
+        use_dora=False,
         init_method=init.xavier_normal_,
         input_is_parallel=True,
         gather_output=False,
         **parallel_linear_kwargs,
     ):
         if r <= 0:
             raise ValueError(f"`r` should be a positive integer value but the value passed is {r}")
@@ -104,15 +118,15 @@
             lora_dropout_layer = nn.Identity()
 
         self.lora_dropout[adapter_name] = lora_dropout_layer
 
         megatron_config = parallel_linear_kwargs["megatron_config"]
         # lora needs to be forced to upgrade to 32-bit precision, otherwise it will overflow
         megatron_config.params_dtype = torch.float32
-        if self.is_paralle_a:
+        if self.is_parallel_a:
             lora_a = self.backend.RowParallelLinear(
                 input_size=self.in_features,
                 output_size=r,
                 bias=False,
                 input_is_parallel=input_is_parallel,
                 skip_bias_add=True,
                 init_method=init_method,
```

### Comparing `peft-0.8.2/src/peft/tuners/lycoris_utils.py` & `peft-0.9.0/src/peft/tuners/lycoris_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# coding=utf-8
 # Copyright 2023-present the HuggingFace Inc. team.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
@@ -13,15 +12,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from __future__ import annotations
 
 import warnings
 from abc import abstractmethod
 from dataclasses import dataclass, field
-from typing import Any, Dict, List, Optional, Set, Type, Union
+from typing import Any, Optional, Union
 
 import torch
 import torch.nn as nn
 from tqdm import tqdm
 
 from peft.config import PeftConfig
 from peft.utils import (
@@ -76,15 +75,15 @@
 
         # Tuner info
         self._disable_adapters = False
         self.merged_adapters = []
 
     @property
     @abstractmethod
-    def _available_adapters(self) -> Set[str]:
+    def _available_adapters(self) -> set[str]:
         ...
 
     def _init_empty_weights(self, cls, *args, **kwargs) -> None:
         # A helper method that allows to initialize the layer of the given class without spending time to initialize the
         # model weights. The implementation is inspired by
         # https://pytorch.org/docs/stable/generated/torch.nn.utils.skip_init.html but this function cannot be used
         # directly.
@@ -104,15 +103,15 @@
     def _get_delta_activations(self, adapter_name: str, x: torch.Tensor, *args: Any, **kwargs: Any) -> torch.Tensor:
         """Activations added on top of the base layer output (i.e. after the base layer forward pass)"""
 
     @abstractmethod
     def get_delta_weight(self, adapter_name: str) -> torch.Tensor:
         ...
 
-    def merge(self, safe_merge: bool = False, adapter_names: Optional[List[str]] = None) -> None:
+    def merge(self, safe_merge: bool = False, adapter_names: Optional[list[str]] = None) -> None:
         """
         Merge the active adapter weights into the base weights
 
         Args:
             safe_merge (`bool`, *optional*):
                 If `True`, the merge operation will be performed in a copy of the original weights and check for NaNs
                 before merging the weights. This is useful if you want to check if the merge operation will produce
@@ -125,17 +124,16 @@
         if not adapter_names:
             # no adapter to merge
             return
 
         for active_adapter in adapter_names:
             if active_adapter in self._available_adapters:
                 base_layer = self.get_base_layer()
-
                 if safe_merge:
-                    orig_weights = base_layer.weight.data
+                    orig_weights = base_layer.weight.data.clone()
                     orig_weights += self.get_delta_weight(active_adapter)
 
                     if not torch.isfinite(orig_weights).all():
                         raise ValueError(
                             f"NaNs detected in the merged weights. The adapter {active_adapter} seems to be broken"
                         )
 
@@ -193,15 +191,15 @@
 
 class LycorisTuner(BaseTuner):
     r"""
     A base tuner for LyCORIS like adapters
     """
 
     prefix: str
-    layers_mapping: Dict[Type[torch.nn.Module], Type[LycorisLayer]]
+    layers_mapping: dict[type[torch.nn.Module], type[LycorisLayer]]
 
     def __init__(self, model, config, adapter_name):
         super().__init__(model, config, adapter_name)
 
     def __getattr__(self, name: str):
         """Forward missing attributes to the wrapped module."""
         try:
@@ -307,15 +305,15 @@
                 module.enable_adapters(enabled)
 
     def _unload_and_optionally_merge(
         self,
         merge: bool = True,
         progressbar: bool = False,
         safe_merge: bool = False,
-        adapter_names: Optional[List[str]] = None,
+        adapter_names: Optional[list[str]] = None,
     ):
         if merge:
             if getattr(self.model, "quantization_method", None) == "gptq":
                 raise ValueError("Cannot merge LOHA layers when the model is gptq quantized")
 
         self._unloading_checks(adapter_names)
         key_list = [key for key, _ in self.model.named_modules() if self.prefix not in key]
@@ -328,15 +326,21 @@
 
             if hasattr(target, "base_layer"):
                 if merge:
                     target.merge(safe_merge=safe_merge, adapter_names=adapter_names)
                 self._replace_module(parent, target_name, target.get_base_layer(), target)
             elif isinstance(target, ModulesToSaveWrapper):
                 # save any additional trainable modules part of `modules_to_save`
-                setattr(parent, target_name, target.modules_to_save[target.active_adapter])
+                new_module = target.modules_to_save[target.active_adapter]
+                if hasattr(new_module, "base_layer"):
+                    # check if the module is itself a tuner layer
+                    if merge:
+                        new_module.merge(safe_merge=safe_merge, adapter_names=adapter_names)
+                    new_module = new_module.get_base_layer()
+                setattr(parent, target_name, new_module)
 
         return self.model
 
     def enable_adapter_layers(self) -> None:
         """Enable all adapters.
 
         Call this if you have previously disabled all adapters and want to re-enable them.
@@ -347,15 +351,15 @@
         """Disable all adapters.
 
         When disabling all adapters, the model output corresponds to the output of the base model.
         """
         self._set_adapter_layers(enabled=False)
 
     def merge_and_unload(
-        self, progressbar: bool = False, safe_merge: bool = False, adapter_names: Optional[List[str]] = None
+        self, progressbar: bool = False, safe_merge: bool = False, adapter_names: Optional[list[str]] = None
     ) -> torch.nn.Module:
         r"""
         This method merges the adapter layers into the base model. This is needed if someone wants to use the base
         model as a standalone model.
 
         Args:
             progressbar (`bool`):
@@ -378,14 +382,23 @@
         model.
         """
         return self._unload_and_optionally_merge(merge=False)
 
     def set_adapter(self, adapter_name: str | list[str]) -> None:
         """Set the active adapter(s).
 
+        Additionally, this function will set the specified adapters to trainable (i.e., requires_grad=True). If this is
+        not desired, use the following code.
+
+        ```py
+        >>> for name, param in model_peft.named_parameters():
+        ...     if ...:  # some check on name (ex. if 'lora' in name)
+        ...         param.requires_grad = False
+        ```
+
         Args:
             adapter_name (`str` or `list[str]`): Name of the adapter(s) to be activated.
         """
         for module in self.model.modules():
             if isinstance(module, LycorisLayer):
                 if module.merged:
                     warnings.warn("Adapter cannot be set when the model is merged. Unmerging the model first.")
```

### Comparing `peft-0.8.2/src/peft/tuners/mixed/__init__.py` & `peft-0.9.0/src/peft/tuners/mixed/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# coding=utf-8
 # Copyright 2023-present the HuggingFace Inc. team.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `peft-0.8.2/src/peft/tuners/mixed/model.py` & `peft-0.9.0/src/peft/tuners/mixed/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# coding=utf-8
 # Copyright 2023-present the HuggingFace Inc. team.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
@@ -259,15 +258,21 @@
 
             if hasattr(target, "base_layer"):
                 if merge:
                     merge_recursively(target)
                 self._replace_module(parent, target_name, target.get_base_layer(), target)
             elif isinstance(target, ModulesToSaveWrapper):
                 # save any additional trainable modules part of `modules_to_save`
-                setattr(parent, target_name, target.modules_to_save[target.active_adapter])
+                new_module = target.modules_to_save[target.active_adapter]
+                if hasattr(new_module, "base_layer"):
+                    # check if the module is itself a tuner layer
+                    if merge:
+                        new_module.merge(safe_merge=safe_merge, adapter_names=adapter_names)
+                    new_module = new_module.get_base_layer()
+                setattr(parent, target_name, new_module)
 
         return self.model
 
     def add_weighted_adapter(self, *args: Any, **kwargs: Any) -> None:
         raise NotImplementedError(f"Weighted adapters are not supported for {self.__class__.__name__} (yet).")
 
     def delete_adapter(self, adapter_name: Union[str, list[str]]) -> None:
```

### Comparing `peft-0.8.2/src/peft/tuners/multitask_prompt_tuning/__init__.py` & `peft-0.9.0/src/peft/tuners/multitask_prompt_tuning/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# coding=utf-8
 # Copyright 2023-present the HuggingFace Inc. team.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `peft-0.8.2/src/peft/tuners/multitask_prompt_tuning/config.py` & `peft-0.9.0/src/peft/tuners/multitask_prompt_tuning/config.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# coding=utf-8
 # Copyright 2023-present the HuggingFace Inc. team.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `peft-0.8.2/src/peft/tuners/multitask_prompt_tuning/model.py` & `peft-0.9.0/src/peft/tuners/multitask_prompt_tuning/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# coding=utf-8
 # Copyright 2023-present the HuggingFace Inc. team.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
@@ -63,17 +62,18 @@
         ]:
             if config.prompt_tuning_init_state_dict_path is None:
                 raise ValueError(
                     f"prompt_tuning_init_state_dict_path needs to be specified with {config.prompt_tuning_init} "
                     "init method"
                 )
 
+            # TODO: There should be an option for safetensors
             state_dict: dict = torch.load(
                 config.prompt_tuning_init_state_dict_path,
-                map_location=word_embeddings.device,
+                map_location=word_embeddings.weight.device,
             )
 
         if config.prompt_tuning_init in [
             MultitaskPromptTuningInit.AVERAGE_SOURCE_TASKS,
             MultitaskPromptTuningInit.EXACT_SOURCE_TASK,
         ]:
             prefix_task_cols_: torch.Tensor = state_dict["prefix_task_cols"]
```

### Comparing `peft-0.8.2/src/peft/tuners/oft/__init__.py` & `peft-0.9.0/src/peft/tuners/p_tuning/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,19 @@
-# coding=utf-8
 # Copyright 2023-present the HuggingFace Inc. team.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from .config import OFTConfig
-from .layer import Conv2d, Linear, OFTLayer
-from .model import OFTModel
+from .config import PromptEncoderConfig, PromptEncoderReparameterizationType
+from .model import PromptEncoder
 
 
-__all__ = ["OFTConfig", "OFTModel", "Conv2d", "Linear", "OFTLayer"]
+__all__ = ["PromptEncoder", "PromptEncoderConfig", "PromptEncoderReparameterizationType"]
```

### Comparing `peft-0.8.2/src/peft/tuners/oft/config.py` & `peft-0.9.0/src/peft/tuners/oft/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# coding=utf-8
 # Copyright 2023-present the HuggingFace Inc. team.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
@@ -46,15 +45,15 @@
             The layer pattern name, used only if `layers_to_transform` is different from `None`.
         rank_pattern (`dict`):
             The mapping from layer names or regexp expression to ranks which are different from the default rank
             specified by `r`.
         modules_to_save (`List[str]`):
             List of modules apart from adapter layers to be set as trainable and saved in the final checkpoint.
         coft (`bool`):
-            Whether to use the constrainted variant of OFT or not, off by default.
+            Whether to use the constrained variant of OFT or not, off by default.
         eps (`float`):
             The control strength of COFT. The freedom of rotation. Only has an effect if `coft` is set to True.
         block_share (`bool`):
             Whether to share the OFT parameters between blocks or not. This is `False` by default.
     """
 
     r: int = field(default=8, metadata={"help": "OFT rank"})
@@ -96,15 +95,15 @@
             "help": "List of modules apart from OFT layers to be set as trainable and saved in the final checkpoint. "
             "For example, in Sequence Classification or Token Classification tasks, "
             "the final layer `classifier/score` are randomly initialized and as such need to be trainable and saved."
         },
     )
     coft: bool = field(
         default=False,
-        metadata={"help": "Whether to use the constrainted variant of OFT or not."},
+        metadata={"help": "Whether to use the constrained variant of OFT or not."},
     )
     eps: float = field(
         default=6e-5,
         metadata={
             "help": "The control strength of COFT. The freedom of rotation. Only has an effect if `coft` is set to True."
         },
     )
```

### Comparing `peft-0.8.2/src/peft/tuners/oft/layer.py` & `peft-0.9.0/src/peft/tuners/oft/layer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# coding=utf-8
 # Copyright 2023-present the HuggingFace Inc. team.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
@@ -68,15 +67,15 @@
         """Internal function to create oft adapter
 
         Args:
             adapter_name (`str`): Name for the adapter to add.
             r (`int`): Rank for the added adapter.
             module_dropout (`float`): The dropout probability for disabling adapter during training.
             init_weights (`bool`): Whether to initialize weights.
-            coft (`bool`): Whether to use the constrainted variant of OFT or not.
+            coft (`bool`): Whether to use the constrained variant of OFT or not.
             eps (`float`):
                 The control strength of COFT. The freedom of rotation. Only has an effect if `coft` is set to True.
             block_share (`bool`): Whether to share the OFT parameters between blocks or not.
         """
         if r <= 0:
             raise ValueError(f"`r` should be a positive integer value but the value passed is {r}")
 
@@ -240,15 +239,15 @@
         return weight
 
     # Copied from https://github.com/Zeju1997/oft/blob/84cebb965df69781e3d9c3c875f5980b421eaf24/oft-control/oft.py#L144
     def _cayley_batch(self, data: torch.Tensor) -> torch.Tensor:
         b, r, c = data.shape
         # Ensure the input matrix is skew-symmetric
         skew = 0.5 * (data - data.transpose(1, 2))
-        I = torch.eye(r, device=data.device).unsqueeze(0).expand(b, r, c)
+        I = torch.eye(r, device=data.device).unsqueeze(0).expand(b, r, c)  # noqa: E741
 
         # Perform the Cayley parametrization
         Q = torch.bmm(I - skew, torch.inverse(I + skew))
 
         return Q
 
     # Copied from https://github.com/Zeju1997/oft/blob/84cebb965df69781e3d9c3c875f5980b421eaf24/oft-control/oft.py#L155
@@ -264,15 +263,15 @@
 
         return A
 
     # Copied from https://github.com/Zeju1997/oft/blob/84cebb965df69781e3d9c3c875f5980b421eaf24/oft-control/oft.py#L52
     def _project_batch(self, oft_r, eps=1e-5):
         # scaling factor for each of the smaller block matrix
         eps = eps * 1 / torch.sqrt(torch.tensor(oft_r.shape[0]))
-        I = (
+        I = (  # noqa: E741
             torch.zeros((oft_r.size(1), oft_r.size(1)), device=oft_r.device, dtype=oft_r.dtype)
             .unsqueeze(0)
             .expand_as(oft_r)
         )
         diff = oft_r - I
         norm_diff = torch.norm(oft_r - I, dim=(1, 2), keepdim=True)
         mask = (norm_diff <= eps).bool()
```

### Comparing `peft-0.8.2/src/peft/tuners/oft/model.py` & `peft-0.9.0/src/peft/tuners/oft/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# coding=utf-8
 # Copyright 2023-present the HuggingFace Inc. team.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
@@ -91,15 +90,15 @@
     ) -> None:
         """
         A private method to create and replace the target module with the adapter module.
         """
 
         # Regexp matching - Find key which matches current target_name in patterns provided
         pattern_keys = list(config.rank_pattern.keys())
-        target_name_key = next(filter(lambda key: re.match(f"(.*\.)?{key}$", current_key), pattern_keys), target_name)
+        target_name_key = next(filter(lambda key: re.match(rf"(.*\.)?{key}$", current_key), pattern_keys), target_name)
 
         kwargs = config.to_dict()
         kwargs["r"] = config.rank_pattern.get(target_name_key, config.r)
 
         if isinstance(target, OFTLayer):
             target.update_layer(adapter_name, **kwargs)
         else:
```

### Comparing `peft-0.8.2/src/peft/tuners/p_tuning/__init__.py` & `peft-0.9.0/src/peft/tuners/prompt_tuning/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,19 @@
-# coding=utf-8
 # Copyright 2023-present the HuggingFace Inc. team.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from .config import PromptEncoderConfig, PromptEncoderReparameterizationType
-from .model import PromptEncoder
+from .config import PromptTuningConfig, PromptTuningInit
+from .model import PromptEmbedding
 
 
-__all__ = ["PromptEncoder", "PromptEncoderConfig", "PromptEncoderReparameterizationType"]
+__all__ = ["PromptTuningConfig", "PromptEmbedding", "PromptTuningInit"]
```

### Comparing `peft-0.8.2/src/peft/tuners/p_tuning/config.py` & `peft-0.9.0/src/peft/tuners/p_tuning/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# coding=utf-8
 # Copyright 2023-present the HuggingFace Inc. team.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `peft-0.8.2/src/peft/tuners/p_tuning/model.py` & `peft-0.9.0/src/peft/tuners/p_tuning/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# coding=utf-8
 # Copyright 2023-present the HuggingFace Inc. team.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `peft-0.8.2/src/peft/tuners/poly/config.py` & `peft-0.9.0/src/peft/tuners/poly/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# coding=utf-8
 # Copyright 2023-present the HuggingFace Inc. team.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `peft-0.8.2/src/peft/tuners/poly/layer.py` & `peft-0.9.0/src/peft/tuners/poly/layer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# coding=utf-8
 # Copyright 2023-present the HuggingFace Inc. team.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `peft-0.8.2/src/peft/tuners/poly/model.py` & `peft-0.9.0/src/peft/tuners/poly/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# coding=utf-8
 # Copyright 2023-present the HuggingFace Inc. team.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `peft-0.8.2/src/peft/tuners/poly/router.py` & `peft-0.9.0/src/peft/tuners/poly/router.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# coding=utf-8
 # Copyright 2023-present the HuggingFace Inc. team.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `peft-0.8.2/src/peft/tuners/prefix_tuning/__init__.py` & `peft-0.9.0/src/peft/tuners/prefix_tuning/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# coding=utf-8
 # Copyright 2023-present the HuggingFace Inc. team.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `peft-0.8.2/src/peft/tuners/prefix_tuning/config.py` & `peft-0.9.0/src/peft/tuners/prefix_tuning/config.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# coding=utf-8
 # Copyright 2023-present the HuggingFace Inc. team.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `peft-0.8.2/src/peft/tuners/prefix_tuning/model.py` & `peft-0.9.0/src/peft/tuners/prefix_tuning/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# coding=utf-8
 # Copyright 2023-present the HuggingFace Inc. team.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `peft-0.8.2/src/peft/tuners/prompt_tuning/__init__.py` & `peft-0.9.0/src/peft/tuners/oft/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-# coding=utf-8
 # Copyright 2023-present the HuggingFace Inc. team.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from .config import PromptTuningConfig, PromptTuningInit
-from .model import PromptEmbedding
+from .config import OFTConfig
+from .layer import Conv2d, Linear, OFTLayer
+from .model import OFTModel
 
 
-__all__ = ["PromptTuningConfig", "PromptEmbedding", "PromptTuningInit"]
+__all__ = ["OFTConfig", "OFTModel", "Conv2d", "Linear", "OFTLayer"]
```

### Comparing `peft-0.8.2/src/peft/tuners/prompt_tuning/config.py` & `peft-0.9.0/src/peft/tuners/prompt_tuning/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# coding=utf-8
 # Copyright 2023-present the HuggingFace Inc. team.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `peft-0.8.2/src/peft/tuners/prompt_tuning/model.py` & `peft-0.9.0/src/peft/tuners/prompt_tuning/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# coding=utf-8
 # Copyright 2023-present the HuggingFace Inc. team.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `peft-0.8.2/src/peft/tuners/tuners_utils.py` & `peft-0.9.0/src/peft/tuners/tuners_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# coding=utf-8
 # Copyright 2023-present the HuggingFace Inc. team.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
@@ -15,15 +14,15 @@
 from __future__ import annotations
 
 import logging
 import re
 import warnings
 from abc import ABC, abstractmethod
 from contextlib import contextmanager
-from typing import Any, List, Optional, Union
+from typing import Any, Optional, Union
 
 import torch
 from accelerate.hooks import AlignDevicesHook
 from accelerate.utils import named_module_tensors, offload_state_dict
 from torch import nn
 from transformers import PreTrainedModel
 from transformers.pytorch_utils import Conv1D
@@ -99,15 +98,15 @@
     - **_prepare_adapter_config**:
         A private method to eventually prepare the adapter config, for example in case the field `target_modules` is
         missing.
     - **_create_and_replace**:
         A private method to create and replace the target module with the adapter module.
     - **_check_target_module_exists**:
         A private helper method to check if the passed module's key name matches any of the target modules in the
-        adatper_config.
+        adapter_config.
 
     The easiest is to check what is done in the `peft.tuners.lora.LoraModel` class.
 
     Attributes:
         model (`torch.nn.Module`):
             The model to which the adapter tuner layers will be attached.
         forward (`Callable`):
@@ -125,15 +124,15 @@
 
     def __init__(self, model, peft_config: Union[PeftConfig, dict[str, PeftConfig]], adapter_name: str) -> None:
         super().__init__()
 
         self.model = model
         self.targeted_module_names: list[str] = []
 
-        # For advanced developpers, if you want to attach multiple adapters to your
+        # For advanced developers, if you want to attach multiple adapters to your
         # model, just add a `peft_config` dict attribute to your model.
         if not hasattr(self, "peft_config"):
             self.peft_config = {adapter_name: peft_config} if isinstance(peft_config, PeftConfig) else peft_config
         else:
             logger.info(
                 "Already found a `peft_config` attribute in the model. This will lead to having multiple adapters"
                 " in the model. Make sure to know what you are doing!"
@@ -199,15 +198,15 @@
         adapter_name: str,
         target: nn.Module,
         target_name: str,
         parent: nn.Module,
         current_key: str,
     ) -> None:
         r"""
-        Inplace replacement of the target module with the adapter layer. This method needs to be overriden by all the
+        Inplace replacement of the target module with the adapter layer. This method needs to be overridden by all the
         tuner classes.
 
         Check `peft.tuners.lora.LoraModel._create_and_replace` for an example.
 
         Args:
             peft_config (`PeftConfig`):
                 The adapter config.
@@ -224,15 +223,15 @@
         """
         ...
 
     @abstractmethod
     def _mark_only_adapters_as_trainable(self, model: nn.Module):
         r"""
         A helper method to mark only the adapter layers as trainable (i.e. module.requires_grad = False) This needs to
-        be overriden for all tuner classes to match the correct key names.
+        be overridden for all tuner classes to match the correct key names.
 
         Check `peft.tuners.lora.LoraModel._mark_only_adapters_as_trainable` for an example.
         """
         ...
 
     def _check_new_adapter_config(self, config: PeftConfig) -> None:
         """
@@ -348,29 +347,29 @@
         This method unmerges all merged adapter layers from the base model.
         """
         for module in self.model.modules():
             if isinstance(module, BaseTunerLayer):
                 with onload_layer(module):
                     module.unmerge()
 
-    def _unloading_checks(self, adapter_names: Optional[List[str]]):
+    def _unloading_checks(self, adapter_names: Optional[list[str]]):
         adapters_to_consider = adapter_names or self.active_adapters
         is_modules_to_save_available = any(
             self.peft_config[adapter].modules_to_save for adapter in adapters_to_consider
         )
         if is_modules_to_save_available and len(adapters_to_consider) > 1:
             raise ValueError("Cannot unload multiple adapters that specify `modules_to_save`.")
 
 
 class BaseTunerLayer(ABC):
     r"""
     A tuner layer mixin that provides the common methods and attributes for all tuners.
 
     Args:
-        is_plugable (`bool`, *optional*):
+        is_pluggable (`bool`, *optional*):
             Whether the adapter layer can be plugged to any pytorch module
         active_adapters (Union[List[`str`], `str`], *optional*):
             The name of the active adapter.
     """
 
     active_adapter = None
 
@@ -460,14 +459,23 @@
                 layer = getattr(self, layer_name)
                 layer.requires_grad_(False)
             self._disable_adapters = True
 
     def set_adapter(self, adapter_names: str | list[str]) -> None:
         """Set the active adapter(s).
 
+        Additionally, this function will set the specified adapters to trainable (i.e., requires_grad=True). If this is
+        not desired, use the following code.
+
+        ```py
+        >>> for name, param in model_peft.named_parameters():
+        ...     if ...:  # some check on name (ex. if 'lora' in name)
+        ...         param.requires_grad = False
+        ```
+
         Args:
             adapter_name (`str` or `List[str]`): Name of the adapter(s) to be activated.
         """
         if isinstance(adapter_names, str):
             adapter_names = [adapter_names]
 
         # Deactivate grads on the inactive adapter and activate grads on the active adapter
@@ -562,15 +570,15 @@
             # TODO: It's still unclear how empty layers_pattern (None, [], or "") should behave
             # For now, empty layers_pattern means any layer pattern is ok
             if layers_pattern is None or len(layers_pattern) == 0:
                 layer_index = re.match(r".*\.[^.]*\.(\d+)\.", key)
             else:
                 layers_pattern = [layers_pattern] if isinstance(layers_pattern, str) else layers_pattern
                 for pattern in layers_pattern:
-                    layer_index = re.match(r".*\.{layer}\.(\d+)\.".format(layer=pattern), key)
+                    layer_index = re.match(rf".*\.{pattern}\.(\d+)\.", key)
                     if layer_index is not None:
                         break
 
             if layer_index is None:
                 target_module_found = False
             else:
                 layer_index = int(layer_index.group(1))
@@ -629,15 +637,15 @@
     if output_emb is not None:
         last_module_name = [name for name, module in model.named_modules() if module is output_emb][0]
         linear_module_names -= {last_module_name}
     peft_config.target_modules = linear_module_names
     return peft_config
 
 
-def check_adapters_to_merge(module: BaseTunerLayer, adapter_names: Optional[List[str]] = None) -> list[str]:
+def check_adapters_to_merge(module: BaseTunerLayer, adapter_names: Optional[list[str]] = None) -> list[str]:
     """
     Helper function to check which adapters should be merged.
 
     Only return those adapters that are not already merged. Give a warning if some or all of the adapters are already
     merged.
 
     """
```

### Comparing `peft-0.8.2/src/peft/utils/__init__.py` & `peft-0.9.0/src/peft/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `peft-0.8.2/src/peft/utils/constants.py` & `peft-0.9.0/src/peft/utils/constants.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# coding=utf-8
 # Copyright 2023-present the HuggingFace Inc. team.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
@@ -73,14 +72,15 @@
     "falcon": ["query_key_value"],
     "btlm": ["c_proj", "c_attn"],
     "codegen": ["qkv_proj"],
     "mistral": ["q_proj", "v_proj"],
     "mixtral": ["q_proj", "v_proj"],
     "stablelm": ["q_proj", "v_proj"],
     "phi": ["q_proj", "v_proj", "fc1", "fc2"],
+    "gemma": ["q_proj", "v_proj"],
 }
 
 TRANSFORMERS_MODELS_TO_IA3_TARGET_MODULES_MAPPING = {
     "t5": ["k", "v", "wo"],
     "mt5": ["k", "v", "wi_1"],
     "gpt2": ["c_attn", "mlp.c_proj"],
     "bloom": ["query_key_value", "mlp.dense_4h_to_h"],
@@ -89,21 +89,23 @@
     "gptj": ["q_proj", "v_proj", "fc_out"],
     "gpt_neox": ["query_key_value", "dense_4h_to_h"],
     "gpt_neo": ["q_proj", "v_proj", "c_proj"],
     "bart": ["q_proj", "v_proj", "fc2"],
     "gpt_bigcode": ["c_attn", "mlp.c_proj"],
     "llama": ["k_proj", "v_proj", "down_proj"],
     "mistral": ["k_proj", "v_proj", "down_proj"],
+    "mixtral": ["k_proj", "v_proj", "w2"],
     "bert": ["key", "value", "output.dense"],
     "deberta-v2": ["key_proj", "value_proj", "output.dense"],
     "deberta": ["in_proj", "output.dense"],
     "RefinedWebModel": ["query_key_value", "dense_4h_to_h"],
     "RefinedWeb": ["query_key_value", "dense_4h_to_h"],
     "falcon": ["query_key_value", "dense_4h_to_h"],
     "phi": ["q_proj", "v_proj", "fc2"],
+    "gemma": ["q_proj", "v_proj", "down_proj"],
 }
 
 TRANSFORMERS_MODELS_TO_IA3_FEEDFORWARD_MODULES_MAPPING = {
     "t5": ["wo"],
     "mt5": [],
     "gpt2": ["mlp.c_proj"],
     "bloom": ["mlp.dense_4h_to_h"],
@@ -112,21 +114,23 @@
     "gptj": ["fc_out"],
     "gpt_neox": ["dense_4h_to_h"],
     "gpt_neo": ["c_proj"],
     "bart": ["fc2"],
     "gpt_bigcode": ["mlp.c_proj"],
     "llama": ["down_proj"],
     "mistral": ["down_proj"],
+    "mixtral": ["w2"],
     "bert": ["output.dense"],
     "deberta-v2": ["output.dense"],
     "deberta": ["output.dense"],
     "RefinedWeb": ["dense_4h_to_h"],
     "RefinedWebModel": ["dense_4h_to_h"],
     "falcon": ["dense_4h_to_h"],
     "phi": ["fc2"],
+    "gemma": ["down_proj"],
 }
 
 TRANSFORMERS_MODELS_TO_ADALORA_TARGET_MODULES_MAPPING = {
     "t5": ["q", "k", "v", "o", "wi", "wo"],
     "mt5": ["q", "k", "v", "o", "wi_0", "wi_1", "wo"],
     "bart": ["q_proj", "k_proj", "v_proj", "out_proj", "fc1", "fc2"],
     "gpt2": ["c_attn"],
```

### Comparing `peft-0.8.2/src/peft/utils/loftq_utils.py` & `peft-0.9.0/src/peft/utils/loftq_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# coding=utf-8
 # Copyright 2023-present the HuggingFace Inc. team.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `peft-0.8.2/src/peft/utils/other.py` & `peft-0.9.0/src/peft/utils/other.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# coding=utf-8
 # Copyright 2023-present the HuggingFace Inc. team.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
@@ -10,21 +9,25 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import copy
 import inspect
+import os
 import warnings
+from contextlib import nullcontext
 from typing import Optional, Tuple
 
 import accelerate
 import torch
 from accelerate.hooks import add_hook_to_module, remove_hook_from_module
 from accelerate.utils import is_npu_available, is_xpu_available
+from huggingface_hub import file_exists
+from huggingface_hub.utils import EntryNotFoundError, HFValidationError
 from safetensors.torch import storage_ptr, storage_size
 
 from ..import_utils import is_auto_gptq_available, is_torch_tpu_available
 from .constants import (
     CONFIG_NAME,
     EMBEDDING_LAYER_NAMES,
     INCLUDE_LINEAR_LAYERS_SHORTHAND,
@@ -53,26 +56,24 @@
     "INCLUDE_LINEAR_LAYERS_SHORTHAND",
     "bloom_model_postprocess_past_key_value",
     "starcoder_model_postprocess_past_key_value",
 ]
 
 
 # Get current device name based on available devices
-def infer_device():
+def infer_device() -> str:
     if torch.cuda.is_available():
-        torch_device = "cuda"
+        return "cuda"
     elif hasattr(torch.backends, "mps") and torch.backends.mps.is_available():
-        torch_device = torch.device("mps")
+        return "mps"
     elif is_xpu_available():
-        torch_device = "xpu"
+        return "xpu"
     elif is_npu_available():
-        torch_device = "npu"
-    else:
-        torch_device = "cpu"
-    return torch_device
+        return "npu"
+    return "cpu"
 
 
 def prepare_model_for_kbit_training(model, use_gradient_checkpointing=True, gradient_checkpointing_kwargs=None):
     r"""
     Note this method only works for `transformers` models.
 
     This method wraps the entire protocol for preparing a model before running a training. This includes:
@@ -87,28 +88,29 @@
         gradient_checkpointing_kwargs (`dict`, *optional*, defaults to `None`):
             Keyword arguments to pass to the gradient checkpointing function, please refer to the documentation of
             `torch.utils.checkpoint.checkpoint` for more details about the arguments that you can pass to that method.
             Note this is only available in the latest transformers versions (> 4.34.1).
     """
     loaded_in_kbit = getattr(model, "is_loaded_in_8bit", False) or getattr(model, "is_loaded_in_4bit", False)
     is_gptq_quantized = getattr(model, "quantization_method", None) == "gptq"
+    is_aqlm_quantized = getattr(model, "quantization_method", None) == "aqlm"
     if gradient_checkpointing_kwargs is None:
         gradient_checkpointing_kwargs = {}
 
     for name, param in model.named_parameters():
         # freeze base model's layers
         param.requires_grad = False
 
-    if not is_gptq_quantized:
+    if not is_gptq_quantized and not is_aqlm_quantized:
         # cast all non INT8 parameters to fp32
         for param in model.parameters():
             if (param.dtype == torch.float16) or (param.dtype == torch.bfloat16):
                 param.data = param.data.to(torch.float32)
 
-    if (loaded_in_kbit or is_gptq_quantized) and use_gradient_checkpointing:
+    if (loaded_in_kbit or is_gptq_quantized or is_aqlm_quantized) and use_gradient_checkpointing:
         # When having `use_reentrant=False` + gradient_checkpointing, there is no need for this hack
         if "use_reentrant" not in gradient_checkpointing_kwargs or gradient_checkpointing_kwargs["use_reentrant"]:
             # For backward compatibility
             if hasattr(model, "enable_input_require_grads"):
                 model.enable_input_require_grads()
             else:
 
@@ -173,14 +175,25 @@
     def __init__(self, module_to_save, adapter_name):
         super().__init__()
         self.original_module = module_to_save
         self.modules_to_save = torch.nn.ModuleDict({})
         self._active_adapter = adapter_name
         self._disable_adapters = False
         self.update(adapter_name)
+        self.check_module()
+
+    def check_module(self):
+        """Perform some sanity checks on the module to ensure that it works"""
+        # Try to anticipate some modules that users could try to target that would not work.
+        # Note: It's not possible to check hasattr(module, "forward"), since that returns True for ModuleDict and
+        # ModuleList, even though their forward methods cannot be called
+        forbidden_classes = (torch.nn.ModuleDict, torch.nn.ModuleList, torch.nn.ParameterDict, torch.nn.ParameterList)
+        if isinstance(self.original_module, forbidden_classes):
+            cls_name = self.original_module.__class__.__name__
+            raise TypeError(f"modules_to_save cannot be applied to modules of type {cls_name}")
 
     @property
     def disable_adapters(self) -> bool:
         # use a property to ensure that disable_adapters is not set directly, instead use the enable_adapters method
         return self._disable_adapters
 
     @property
@@ -191,15 +204,25 @@
     @property
     def weight(self):
         if self.active_adapter not in self.modules_to_save:
             return self.original_module.weight
         return self.modules_to_save[self.active_adapter].weight
 
     def update(self, adapter_name):
-        self.modules_to_save.update(torch.nn.ModuleDict({adapter_name: copy.deepcopy(self.original_module)}))
+        context_manager = nullcontext()
+        for _, param in self.original_module.named_parameters():
+            num_params = param.numel()
+            # if using DS Zero 3 and the weights are initialized empty
+            if num_params == 0 and hasattr(param, "ds_numel"):
+                import deepspeed
+
+                context_manager = deepspeed.zero.GatheredParameters(self.original_module.parameters(), modifier_rank=0)
+                break
+        with context_manager:
+            self.modules_to_save.update(torch.nn.ModuleDict({adapter_name: copy.deepcopy(self.original_module)}))
 
         if hasattr(self.modules_to_save[adapter_name], "_hf_hook"):
             old_hook = self.modules_to_save[adapter_name]._hf_hook
             new_hook = self._create_new_hook(old_hook)
             remove_hook_from_module(self.modules_to_save[adapter_name])
             add_hook_to_module(self.modules_to_save[adapter_name], new_hook)
 
@@ -246,14 +269,23 @@
             self.original_module.requires_grad_(True)
             self.modules_to_save.requires_grad_(False)
             self._disable_adapters = True
 
     def set_adapter(self, adapter_name: str):
         """Set the active adapter
 
+        Additionally, this function will set the specified adapter to trainable (i.e., requires_grad=True). If this is
+        not desired, use the following code.
+
+        ```py
+        >>> for name, param in model_peft.named_parameters():
+        ...     if ...:  # some check on name (ex. if 'lora' in name)
+        ...         param.requires_grad = False
+        ```
+
         Args:
             adapter_name (str): The name of the adapter to set as active
         """
         if adapter_name not in self.modules_to_save:
             raise ValueError(f"Adapter {adapter_name} not found in {self.modules_to_save.keys()}")
 
         self.modules_to_save[self.active_adapter].requires_grad_(False)
@@ -514,7 +546,48 @@
     `torch.bfloat16` as per the mixed-precision training you are performing.
     """
     for p in model.parameters():
         if not p.requires_grad:
             p.data = p.to(dtype)
         else:
             p.data = p.to(torch.float32)
+
+
+def str_to_bool(value: str) -> int:
+    """
+    Converts a string representation of truth to `True` (1) or `False` (0).
+
+    True values are `y`, `yes`, `t`, `true`, `on`, and `1`; False value are `n`, `no`, `f`, `false`, `off`, and `0`;
+    """
+    # same as function as in accelerate.utils, which replaces the deprecated distutils.util.strtobool
+    value = value.lower()
+    if value in ("y", "yes", "t", "true", "on", "1"):
+        return 1
+    elif value in ("n", "no", "f", "false", "off", "0"):
+        return 0
+    else:
+        raise ValueError(f"invalid truth value {value}")
+
+
+def check_file_exists_on_hf_hub(repo_id: str, filename: str, **kwargs) -> Optional[bool]:
+    """Check if a file exists on HF Hub, if check was not successful returns None instead of erroring.
+
+    Respect offline mode if set.
+
+    """
+    exists: Optional[bool] = None
+    if str_to_bool(os.environ.get("HF_HUB_OFFLINE", "0")):
+        # user set offline mode, cannot check
+        return exists
+
+    try:
+        exists = file_exists(repo_id, filename, **kwargs)
+    except (HFValidationError, EntryNotFoundError):
+        # error, exists stays None
+        pass
+    except Exception as e:
+        warnings.warn(
+            f"Unable to fetch remote file due to the following error {e} - silently ignoring the lookup"
+            f" for the file {filename} in {repo_id}."
+        )
+
+    return exists
```

### Comparing `peft-0.8.2/src/peft/utils/peft_types.py` & `peft-0.9.0/src/peft/utils/peft_types.py`

 * *Files 4% similar despite different names*

```diff
@@ -54,15 +54,15 @@
 class TaskType(str, enum.Enum):
     """
     Enum class for the different types of tasks supported by PEFT.
 
     Overview of the supported task types:
     - SEQ_CLS: Text classification.
     - SEQ_2_SEQ_LM: Sequence-to-sequence language modeling.
-    - Causal LM: Causal language modeling.
+    - CAUSAL_LM: Causal language modeling.
     - TOKEN_CLS: Token classification.
     - QUESTION_ANS: Question answering.
     - FEATURE_EXTRACTION: Feature extraction. Provides the hidden states which can be used as embeddings or features
       for downstream tasks.
     """
 
     SEQ_CLS = "SEQ_CLS"
```

### Comparing `peft-0.8.2/src/peft/utils/save_and_load.py` & `peft-0.9.0/src/peft/utils/save_and_load.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# coding=utf-8
 # Copyright 2023-present the HuggingFace Inc. team.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
@@ -14,18 +13,24 @@
 # limitations under the License.
 import os
 import warnings
 from typing import Optional
 
 import torch
 from huggingface_hub import file_exists, hf_hub_download
-from huggingface_hub.utils import EntryNotFoundError, HFValidationError
+from huggingface_hub.utils import EntryNotFoundError
 from safetensors.torch import load_file as safe_load_file
 
-from .other import EMBEDDING_LAYER_NAMES, SAFETENSORS_WEIGHTS_NAME, WEIGHTS_NAME, infer_device
+from .other import (
+    EMBEDDING_LAYER_NAMES,
+    SAFETENSORS_WEIGHTS_NAME,
+    WEIGHTS_NAME,
+    check_file_exists_on_hf_hub,
+    infer_device,
+)
 from .peft_types import PeftType
 
 
 def has_valid_embedding_base_layer(layer):
     """Check if the layer has an embedding base layer"""
     return hasattr(layer, "base_layer") and isinstance(layer.base_layer, (torch.nn.Linear, torch.nn.Embedding))
 
@@ -137,22 +142,25 @@
         vocab_size = getattr(getattr(model, "config", None), "vocab_size", None)
         model_id = getattr(config, "base_model_name_or_path", None)
 
         # For some models e.g. diffusers the text config file is stored in a subfolder
         # we need to make sure we can download that config.
         has_remote_config = False
 
+        # ensure that this check is not performed in HF offline mode, see #1452
         if model_id is not None:
-            try:
-                has_remote_config = file_exists(model_id, "config.json")
-            except (HFValidationError, EntryNotFoundError):
+            exists = check_file_exists_on_hf_hub(model_id, "config.json")
+            if exists is None:
+                # check failed, could not determine if it exists or not
                 warnings.warn(
                     f"Could not find a config file in {model_id} - will assume that the vocabulary was not modified."
                 )
                 has_remote_config = False
+            else:
+                has_remote_config = exists
 
         # check if the vocab size of the base model is different from the vocab size of the finetuned model
         if (
             vocab_size
             and model_id
             and has_remote_config
             and (vocab_size != model.config.__class__.from_pretrained(model_id).vocab_size)
```

### Comparing `peft-0.8.2/src/peft.egg-info/SOURCES.txt` & `peft-0.9.0/src/peft.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -40,14 +40,16 @@
 src/peft/tuners/loha/layer.py
 src/peft/tuners/loha/model.py
 src/peft/tuners/lokr/__init__.py
 src/peft/tuners/lokr/config.py
 src/peft/tuners/lokr/layer.py
 src/peft/tuners/lokr/model.py
 src/peft/tuners/lora/__init__.py
+src/peft/tuners/lora/aqlm.py
+src/peft/tuners/lora/awq.py
 src/peft/tuners/lora/bnb.py
 src/peft/tuners/lora/config.py
 src/peft/tuners/lora/gptq.py
 src/peft/tuners/lora/layer.py
 src/peft/tuners/lora/model.py
 src/peft/tuners/lora/tp_layer.py
 src/peft/tuners/mixed/__init__.py
@@ -71,27 +73,34 @@
 src/peft/tuners/prefix_tuning/config.py
 src/peft/tuners/prefix_tuning/model.py
 src/peft/tuners/prompt_tuning/__init__.py
 src/peft/tuners/prompt_tuning/config.py
 src/peft/tuners/prompt_tuning/model.py
 src/peft/utils/__init__.py
 src/peft/utils/constants.py
+src/peft/utils/integrations.py
 src/peft/utils/loftq_utils.py
+src/peft/utils/merge_utils.py
 src/peft/utils/other.py
 src/peft/utils/peft_types.py
 src/peft/utils/save_and_load.py
 tests/test_adaption_prompt.py
 tests/test_auto.py
 tests/test_common_gpu.py
 tests/test_config.py
 tests/test_custom_models.py
 tests/test_decoder_models.py
 tests/test_encoder_decoder_models.py
 tests/test_feature_extraction_models.py
 tests/test_gpu_examples.py
 tests/test_hub_features.py
+tests/test_initialization.py
+tests/test_lora_megatron.py
 tests/test_low_level_api.py
+tests/test_mixed.py
 tests/test_multitask_prompt_tuning.py
+tests/test_other.py
+tests/test_poly.py
 tests/test_stablediffusion.py
 tests/test_tuners_utils.py
 tests/testing_common.py
 tests/testing_utils.py
```

### Comparing `peft-0.8.2/tests/test_adaption_prompt.py` & `peft-0.9.0/tests/test_adaption_prompt.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# coding=utf-8
 # Copyright 2023-present the HuggingFace Inc. team.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
@@ -15,14 +14,15 @@
 
 import importlib
 import os
 import tempfile
 import unittest
 from unittest import TestCase
 
+import pytest
 import torch
 from torch.testing import assert_close
 
 from peft.mapping import get_peft_model
 from peft.peft_model import PeftModel
 from peft.tuners.adaption_prompt import AdaptionPromptConfig
 from peft.utils.other import prepare_model_for_int8_training
@@ -70,36 +70,36 @@
         )
 
     def test_attributes(self) -> None:
         model = LlamaModel(self._create_test_llama_config())
         config = AdaptionPromptConfig(adapter_layers=1, adapter_len=4)
         model = get_peft_model(model, config)
 
-        self.assertTrue(hasattr(model, "save_pretrained"))
-        self.assertTrue(hasattr(model, "from_pretrained"))
-        self.assertTrue(hasattr(model, "push_to_hub"))
+        assert hasattr(model, "save_pretrained")
+        assert hasattr(model, "from_pretrained")
+        assert hasattr(model, "push_to_hub")
 
     def test_prepare_for_training(self) -> None:
         model = LlamaForCausalLM(self._create_test_llama_config())
         config = AdaptionPromptConfig(adapter_layers=1, adapter_len=4, task_type="CAUSAL_LM")
         model = get_peft_model(model, config)
         model = model.to(self.torch_device)
 
         dummy_input = torch.LongTensor([[1, 1, 1]]).to(self.torch_device)
         dummy_output = model.get_input_embeddings()(dummy_input)
 
-        self.assertTrue(not dummy_output.requires_grad)
+        assert not dummy_output.requires_grad
 
     def test_prepare_for_int8_training(self) -> None:
         model = LlamaForCausalLM(self._create_test_llama_config())
         model = prepare_model_for_int8_training(model)
         model = model.to(self.torch_device)
 
         for param in model.parameters():
-            self.assertTrue(not param.requires_grad)
+            assert not param.requires_grad
 
         config = AdaptionPromptConfig(adapter_layers=1, adapter_len=4, task_type="CAUSAL_LM")
         model = get_peft_model(model, config)
 
         # For backward compatibility
         if hasattr(model, "enable_input_require_grads"):
             model.enable_input_require_grads()
@@ -109,15 +109,15 @@
                 output.requires_grad_(True)
 
             model.get_input_embeddings().register_forward_hook(make_inputs_require_grad)
 
         dummy_input = torch.LongTensor([[1, 1, 1]]).to(self.torch_device)
         dummy_output = model.get_input_embeddings()(dummy_input)
 
-        self.assertTrue(dummy_output.requires_grad)
+        assert dummy_output.requires_grad
 
     def test_save_pretrained_regression(self) -> None:
         seed = 420
         torch.manual_seed(seed)
         model = LlamaForCausalLM(self._create_test_llama_config())
         config = AdaptionPromptConfig(adapter_layers=2, adapter_len=4, task_type="CAUSAL_LM")
         model = get_peft_model(model, config)
@@ -131,38 +131,36 @@
             model_from_pretrained = PeftModel.from_pretrained(model_from_pretrained, tmp_dirname)
 
             # check if the state dicts are equal
             state_dict = get_peft_model_state_dict(model)
             state_dict_from_pretrained = get_peft_model_state_dict(model_from_pretrained)
 
             # check if same keys
-            self.assertEqual(state_dict.keys(), state_dict_from_pretrained.keys())
+            assert state_dict.keys() == state_dict_from_pretrained.keys()
 
             # Check that the number of saved parameters is 4 -- 2 layers of (tokens and gate).
-            self.assertEqual(len(list(state_dict.keys())), 4)
+            assert len(state_dict) == 4
 
             # check if tensors equal
             for key in state_dict.keys():
-                self.assertTrue(
-                    torch.allclose(
-                        state_dict[key].to(self.torch_device), state_dict_from_pretrained[key].to(self.torch_device)
-                    )
+                assert torch.allclose(
+                    state_dict[key].to(self.torch_device), state_dict_from_pretrained[key].to(self.torch_device)
                 )
 
             # check if `adapter_model.bin` is present
-            self.assertTrue(os.path.exists(os.path.join(tmp_dirname, "adapter_model.bin")))
+            assert os.path.exists(os.path.join(tmp_dirname, "adapter_model.bin"))
 
             # check if `adapter_config.json` is present
-            self.assertTrue(os.path.exists(os.path.join(tmp_dirname, "adapter_config.json")))
+            assert os.path.exists(os.path.join(tmp_dirname, "adapter_config.json"))
 
             # check if `model.safetensors` is not present
-            self.assertFalse(os.path.exists(os.path.join(tmp_dirname, "model.safetensors")))
+            assert not os.path.exists(os.path.join(tmp_dirname, "model.safetensors"))
 
             # check if `config.json` is not present
-            self.assertFalse(os.path.exists(os.path.join(tmp_dirname, "config.json")))
+            assert not os.path.exists(os.path.join(tmp_dirname, "config.json"))
 
     def test_save_pretrained(self) -> None:
         seed = 420
         torch.manual_seed(seed)
         model = LlamaForCausalLM(self._create_test_llama_config())
         config = AdaptionPromptConfig(adapter_layers=2, adapter_len=4, task_type="CAUSAL_LM")
         model = get_peft_model(model, config)
@@ -176,38 +174,36 @@
             model_from_pretrained = PeftModel.from_pretrained(model_from_pretrained, tmp_dirname)
 
             # check if the state dicts are equal
             state_dict = get_peft_model_state_dict(model)
             state_dict_from_pretrained = get_peft_model_state_dict(model_from_pretrained)
 
             # check if same keys
-            self.assertEqual(state_dict.keys(), state_dict_from_pretrained.keys())
+            assert state_dict.keys() == state_dict_from_pretrained.keys()
 
             # Check that the number of saved parameters is 4 -- 2 layers of (tokens and gate).
-            self.assertEqual(len(list(state_dict.keys())), 4)
+            assert len(state_dict) == 4
 
             # check if tensors equal
             for key in state_dict.keys():
-                self.assertTrue(
-                    torch.allclose(
-                        state_dict[key].to(self.torch_device), state_dict_from_pretrained[key].to(self.torch_device)
-                    )
+                assert torch.allclose(
+                    state_dict[key].to(self.torch_device), state_dict_from_pretrained[key].to(self.torch_device)
                 )
 
             # check if `adapter_model.bin` is present
-            self.assertTrue(os.path.exists(os.path.join(tmp_dirname, "adapter_model.safetensors")))
+            assert os.path.exists(os.path.join(tmp_dirname, "adapter_model.safetensors"))
 
             # check if `adapter_config.json` is present
-            self.assertTrue(os.path.exists(os.path.join(tmp_dirname, "adapter_config.json")))
+            assert os.path.exists(os.path.join(tmp_dirname, "adapter_config.json"))
 
             # check if `model.safetensors` is not present
-            self.assertFalse(os.path.exists(os.path.join(tmp_dirname, "model.safetensors")))
+            assert not os.path.exists(os.path.join(tmp_dirname, "model.safetensors"))
 
             # check if `config.json` is not present
-            self.assertFalse(os.path.exists(os.path.join(tmp_dirname, "config.json")))
+            assert not os.path.exists(os.path.join(tmp_dirname, "config.json"))
 
     def test_save_pretrained_selected_adapters(self) -> None:
         seed = 420
         torch.manual_seed(seed)
         model = LlamaForCausalLM(self._create_test_llama_config())
         config = AdaptionPromptConfig(adapter_layers=2, adapter_len=4, task_type="CAUSAL_LM")
         model = get_peft_model(model, config)
@@ -226,38 +222,36 @@
             model_from_pretrained.load_adapter(tmp_dirname, "new_adapter")
 
             # check if the state dicts are equal
             state_dict = get_peft_model_state_dict(model)
             state_dict_from_pretrained = get_peft_model_state_dict(model_from_pretrained)
 
             # check if same keys
-            self.assertEqual(state_dict.keys(), state_dict_from_pretrained.keys())
+            assert state_dict.keys() == state_dict_from_pretrained.keys()
 
             # Check that the number of saved parameters is 4 -- 2 layers of (tokens and gate).
-            self.assertEqual(len(list(state_dict.keys())), 4)
+            assert len(state_dict) == 4
 
             # check if tensors equal
             for key in state_dict.keys():
-                self.assertTrue(
-                    torch.allclose(
-                        state_dict[key].to(self.torch_device), state_dict_from_pretrained[key].to(self.torch_device)
-                    )
+                assert torch.allclose(
+                    state_dict[key].to(self.torch_device), state_dict_from_pretrained[key].to(self.torch_device)
                 )
 
             # check if `adapter_model.bin` is present
-            self.assertTrue(os.path.exists(os.path.join(tmp_dirname, "adapter_model.safetensors")))
+            assert os.path.exists(os.path.join(tmp_dirname, "adapter_model.safetensors"))
 
             # check if `adapter_config.json` is present
-            self.assertTrue(os.path.exists(os.path.join(tmp_dirname, "adapter_config.json")))
+            assert os.path.exists(os.path.join(tmp_dirname, "adapter_config.json"))
 
             # check if `model.safetensors` is not present
-            self.assertFalse(os.path.exists(os.path.join(tmp_dirname, "model.safetensors")))
+            assert not os.path.exists(os.path.join(tmp_dirname, "model.safetensors"))
 
             # check if `config.json` is not present
-            self.assertFalse(os.path.exists(os.path.join(tmp_dirname, "config.json")))
+            assert not os.path.exists(os.path.join(tmp_dirname, "config.json"))
 
     def test_generate(self) -> None:
         model = LlamaForCausalLM(self._create_test_llama_config())
         config = AdaptionPromptConfig(adapter_layers=2, adapter_len=4, task_type="CAUSAL_LM")
         model = get_peft_model(model, config)
         model = model.to(self.torch_device)
 
@@ -296,18 +290,18 @@
         optimizer = torch.optim.SGD(adapted.parameters(), lr=1)
         optimizer.zero_grad()
         default_before.loss.backward()
         optimizer.step()
 
         # Test that the output changed.
         default_after = adapted(input_ids=input_ids, attention_mask=attention_mask, labels=target_ids)
-        self.assertFalse(torch.allclose(default_before.logits, default_after.logits))
+        assert not torch.allclose(default_before.logits, default_after.logits)
 
         with adapted.disable_adapter():
-            # Test that the output is the same as the original ouput.
+            # Test that the output is the same as the original output.
             default_disabled = adapted(input_ids=input_ids, attention_mask=attention_mask, labels=target_ids)
             assert_close(original_before.logits, default_disabled.logits, rtol=0, atol=0)
 
         # Add new adapter 1.
         adapted.add_adapter("adapter 1", AdaptionPromptConfig(adapter_layers=3, adapter_len=8, task_type="CAUSAL_LM"))
         # Test zero-init
         adapter_1_before = adapted(input_ids=input_ids, attention_mask=attention_mask, labels=target_ids)
@@ -317,31 +311,31 @@
         optimizer = torch.optim.SGD(adapted.parameters(), lr=1)
         optimizer.zero_grad()
         adapter_1_before.loss.backward()
         optimizer.step()
 
         # Test that adapter 1 output changed.
         adapter_1_after = adapted(input_ids=input_ids, attention_mask=attention_mask, labels=target_ids)
-        self.assertFalse(torch.allclose(adapter_1_before.logits, adapter_1_after.logits))
-        self.assertFalse(torch.allclose(original_before.logits, adapter_1_after.logits))
-        self.assertFalse(torch.allclose(default_after.logits, adapter_1_after.logits))
+        assert not torch.allclose(adapter_1_before.logits, adapter_1_after.logits)
+        assert not torch.allclose(original_before.logits, adapter_1_after.logits)
+        assert not torch.allclose(default_after.logits, adapter_1_after.logits)
 
         with adapted.disable_adapter():
             # Test that the output is the same as the original output.
             adapter_1_disabled = adapted(input_ids=input_ids, attention_mask=attention_mask, labels=target_ids)
             assert_close(original_before.logits, adapter_1_disabled.logits, rtol=0, atol=0)
 
         # Set adapter back to default.
         adapted.set_adapter("default")
 
         # Test that the output is the same as the default output after training.
         default_after_set = adapted(input_ids=input_ids, attention_mask=attention_mask, labels=target_ids)
         assert_close(default_after.logits, default_after_set.logits, rtol=0, atol=0)
-        self.assertFalse(torch.allclose(original_before.logits, default_after_set.logits))
-        self.assertFalse(torch.allclose(adapter_1_after.logits, default_after_set.logits))
+        assert not torch.allclose(original_before.logits, default_after_set.logits)
+        assert not torch.allclose(adapter_1_after.logits, default_after_set.logits)
 
     def test_add_and_set_while_disabled(self):
         """Test that adding and setting adapters while disabled works as intended."""
         # Test input data.
         input_ids = torch.LongTensor([[1, 1, 1], [2, 1, 2]]).to(self.torch_device)
         target_ids = torch.LongTensor([[0, 0, 0], [0, 0, 0]]).to(self.torch_device)
         attention_mask = torch.LongTensor([[1, 1, 1], [1, 0, 1]]).to(self.torch_device)
@@ -370,15 +364,15 @@
         optimizer = torch.optim.SGD(adapted.parameters(), lr=1)
         optimizer.zero_grad()
         adapter_1_before.loss.backward()
         optimizer.step()
 
         # Test that adapter 1 output changed.
         adapter_1_after = adapted(input_ids=input_ids, attention_mask=attention_mask, labels=target_ids)
-        self.assertFalse(torch.allclose(original_before.logits, adapter_1_after.logits))
+        assert not torch.allclose(original_before.logits, adapter_1_after.logits)
 
         adapted.set_adapter("default")
         with adapted.disable_adapter():
             adapted.set_adapter("adapter 1")
 
         # Test that adapter 1 is active again.
         adapter_1_after_set = adapted(input_ids=input_ids, attention_mask=attention_mask, labels=target_ids)
@@ -406,14 +400,17 @@
 
         # Set use_cache = True and generate output again.
         adapted.base_model.config.use_cache = True
         actual = adapted.generate(input_ids=input_ids, max_length=8)
         assert_close(expected, actual, rtol=0, atol=0)
 
     def test_bf16_inference(self) -> None:
+        if self.torch_device == "mps":
+            return pytest.skip("Skipping bf16 test on MPS")
+
         """Test that AdaptionPrompt works when Llama using a half-precision model."""
         input_ids = torch.LongTensor([[1, 1, 1], [2, 1, 2]]).to(self.torch_device)
         original = LlamaForCausalLM.from_pretrained(
             "trl-internal-testing/tiny-random-LlamaForCausalLM", torch_dtype=torch.bfloat16
         )
         adapted = get_peft_model(
             original, AdaptionPromptConfig(adapter_layers=2, adapter_len=4, task_type="CAUSAL_LM")
@@ -431,12 +428,12 @@
         config = AdaptionPromptConfig(adapter_layers=1, adapter_len=4, task_type="CAUSAL_LM")
         model = get_peft_model(model, config).to(self.torch_device)
         output_peft = model(dummy_input).logits
         # TODO currently this fails because scores are zeroed out:
         # https://github.com/huggingface/peft/blob/062d95a09eb5d1de35c0e5e23d4387daba99e2db/src/peft/tuners/adaption_prompt.py#L303
         # This is fine for users but makes it difficult to test if anything happens. In the future, we will have a clean
         # way to control initialization. Until then, this test is expected to fail.
-        self.assertFalse(torch.allclose(output_before, output_peft))
+        assert not torch.allclose(output_before, output_peft)
 
         with model.disable_adapter():
             output_peft_disabled = model(dummy_input).logits
-        self.assertTrue(torch.allclose(output_before, output_peft_disabled))
+        assert torch.allclose(output_before, output_peft_disabled)
```

### Comparing `peft-0.8.2/tests/test_common_gpu.py` & `peft-0.9.0/tests/test_common_gpu.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# coding=utf-8
 # Copyright 2023-present the HuggingFace Inc. team.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
@@ -117,27 +116,21 @@
             bias="none",
             task_type="CAUSAL_LM",
         )
 
         config = LoraConfig(r=32, lora_alpha=64, target_modules=["q_proj", "v_proj"], lora_dropout=0.05, bias="none")
 
         flan_8bit = get_peft_model(flan_8bit, flan_lora_config)
-        self.assertTrue(
-            isinstance(flan_8bit.base_model.model.encoder.block[0].layer[0].SelfAttention.q, LoraLinear8bitLt)
-        )
+        assert isinstance(flan_8bit.base_model.model.encoder.block[0].layer[0].SelfAttention.q, LoraLinear8bitLt)
 
         opt_8bit = get_peft_model(opt_8bit, opt_lora_config)
-        self.assertTrue(
-            isinstance(opt_8bit.base_model.model.model.decoder.layers[0].self_attn.v_proj, LoraLinear8bitLt)
-        )
+        assert isinstance(opt_8bit.base_model.model.model.decoder.layers[0].self_attn.v_proj, LoraLinear8bitLt)
 
         whisper_8bit = get_peft_model(whisper_8bit, config)
-        self.assertTrue(
-            isinstance(whisper_8bit.base_model.model.model.decoder.layers[0].self_attn.v_proj, LoraLinear8bitLt)
-        )
+        assert isinstance(whisper_8bit.base_model.model.model.decoder.layers[0].self_attn.v_proj, LoraLinear8bitLt)
 
     @require_bitsandbytes
     @pytest.mark.multi_gpu_tests
     @pytest.mark.single_gpu_tests
     def test_ia3_bnb_8bit_quantization(self):
         r"""
         Test that tests if the 8bit quantization using IA3 works as expected
@@ -167,27 +160,21 @@
             feedforward_modules=["fc2"],
             task_type="CAUSAL_LM",
         )
 
         config = IA3Config(target_modules=["q_proj", "v_proj", "fc2"], feedforward_modules=["fc2"])
 
         flan_8bit = get_peft_model(flan_8bit, flan_ia3_config)
-        self.assertTrue(
-            isinstance(flan_8bit.base_model.model.encoder.block[0].layer[0].SelfAttention.q, IA3Linear8bitLt)
-        )
+        assert isinstance(flan_8bit.base_model.model.encoder.block[0].layer[0].SelfAttention.q, IA3Linear8bitLt)
 
         opt_8bit = get_peft_model(opt_8bit, opt_ia3_config)
-        self.assertTrue(
-            isinstance(opt_8bit.base_model.model.model.decoder.layers[0].self_attn.v_proj, IA3Linear8bitLt)
-        )
+        assert isinstance(opt_8bit.base_model.model.model.decoder.layers[0].self_attn.v_proj, IA3Linear8bitLt)
 
         whisper_8bit = get_peft_model(whisper_8bit, config)
-        self.assertTrue(
-            isinstance(whisper_8bit.base_model.model.model.decoder.layers[0].self_attn.v_proj, IA3Linear8bitLt)
-        )
+        assert isinstance(whisper_8bit.base_model.model.model.decoder.layers[0].self_attn.v_proj, IA3Linear8bitLt)
 
     @require_bitsandbytes
     @pytest.mark.multi_gpu_tests
     @pytest.mark.single_gpu_tests
     @parameterized.expand(["4bit", "8bit"])
     def test_lora_bnb_quantization_from_pretrained_safetensors(self, quantization):
         r"""
@@ -208,16 +195,16 @@
 
         # loading a 2nd adapter works, #1239
         model.load_adapter(peft_model_id, "adapter2")
         model.set_adapter("adapter2")
         model.generate(input_ids=torch.LongTensor([[0, 2, 3, 1]]).to(0))
 
         # check that both adapters are in the same layer
-        self.assertIn("default", model.base_model.model.model.decoder.layers[0].self_attn.q_proj.lora_A)
-        self.assertIn("adapter2", model.base_model.model.model.decoder.layers[0].self_attn.q_proj.lora_A)
+        assert "default" in model.base_model.model.model.decoder.layers[0].self_attn.q_proj.lora_A
+        assert "adapter2" in model.base_model.model.model.decoder.layers[0].self_attn.q_proj.lora_A
 
     @require_bitsandbytes
     @pytest.mark.multi_gpu_tests
     @pytest.mark.single_gpu_tests
     @parameterized.expand(["4bit", "8bit"])
     def test_adalora_bnb_quantization_from_pretrained_safetensors(self, quantization):
         r"""
@@ -245,16 +232,16 @@
 
             # loading a 2nd adapter works, #1239
             model.load_adapter(tmp_dir, "adapter2")
             model.set_adapter("adapter2")
             model.generate(input_ids=torch.LongTensor([[0, 2, 3, 1]]).to(0))
 
             # check that both adapters are in the same layer
-            self.assertIn("default", model.base_model.model.model.decoder.layers[0].self_attn.q_proj.lora_A)
-            self.assertIn("adapter2", model.base_model.model.model.decoder.layers[0].self_attn.q_proj.lora_A)
+            assert "default" in model.base_model.model.model.decoder.layers[0].self_attn.q_proj.lora_A
+            assert "adapter2" in model.base_model.model.model.decoder.layers[0].self_attn.q_proj.lora_A
 
     @require_bitsandbytes
     @pytest.mark.multi_gpu_tests
     @pytest.mark.single_gpu_tests
     @parameterized.expand(["4bit", "8bit"])
     def test_ia3_bnb_quantization_from_pretrained_safetensors(self, quantization):
         r"""
@@ -282,16 +269,16 @@
 
             # loading a 2nd adapter works, #1239
             model.load_adapter(tmp_dir, "adapter2")
             model.set_adapter("adapter2")
             model.generate(input_ids=torch.LongTensor([[0, 2, 3, 1]]).to(0))
 
             # check that both adapters are in the same layer
-            self.assertIn("default", model.base_model.model.model.decoder.layers[0].self_attn.q_proj.ia3_l)
-            self.assertIn("adapter2", model.base_model.model.model.decoder.layers[0].self_attn.q_proj.ia3_l)
+            assert "default" in model.base_model.model.model.decoder.layers[0].self_attn.q_proj.ia3_l
+            assert "adapter2" in model.base_model.model.model.decoder.layers[0].self_attn.q_proj.ia3_l
 
     @pytest.mark.single_gpu_tests
     def test_lora_gptq_quantization_from_pretrained_safetensors(self):
         r"""
         Tests that the autogptq quantization using LoRA works as expected with safetensors weights.
         """
         from transformers import GPTQConfig
@@ -320,16 +307,16 @@
 
             # loading a 2nd adapter works, #1239
             model.load_adapter(tmp_dir, "adapter2")
             model.set_adapter("adapter2")
             model.generate(input_ids=torch.LongTensor([[0, 2, 3, 1]]).to(0))
 
             # check that both adapters are in the same layer
-            self.assertIn("default", model.base_model.model.model.decoder.layers[0].self_attn.q_proj.lora_A)
-            self.assertIn("adapter2", model.base_model.model.model.decoder.layers[0].self_attn.q_proj.lora_A)
+            assert "default" in model.base_model.model.model.decoder.layers[0].self_attn.q_proj.lora_A
+            assert "adapter2" in model.base_model.model.model.decoder.layers[0].self_attn.q_proj.lora_A
 
     @require_bitsandbytes
     @pytest.mark.multi_gpu_tests
     @pytest.mark.single_gpu_tests
     def test_lora_bnb_4bit_quantization(self):
         r"""
         Test that tests if the 4bit quantization using LoRA works as expected
@@ -364,25 +351,21 @@
             bias="none",
             task_type="CAUSAL_LM",
         )
 
         config = LoraConfig(r=32, lora_alpha=64, target_modules=["q_proj", "v_proj"], lora_dropout=0.05, bias="none")
 
         flan_4bit = get_peft_model(flan_4bit, flan_lora_config)
-        self.assertTrue(
-            isinstance(flan_4bit.base_model.model.encoder.block[0].layer[0].SelfAttention.q, LoraLinear4bit)
-        )
+        assert isinstance(flan_4bit.base_model.model.encoder.block[0].layer[0].SelfAttention.q, LoraLinear4bit)
 
         opt_4bit = get_peft_model(opt_4bit, opt_lora_config)
-        self.assertTrue(isinstance(opt_4bit.base_model.model.model.decoder.layers[0].self_attn.v_proj, LoraLinear4bit))
+        assert isinstance(opt_4bit.base_model.model.model.decoder.layers[0].self_attn.v_proj, LoraLinear4bit)
 
         whisper_4bit = get_peft_model(whisper_4bit, config)
-        self.assertTrue(
-            isinstance(whisper_4bit.base_model.model.model.decoder.layers[0].self_attn.v_proj, LoraLinear4bit)
-        )
+        assert isinstance(whisper_4bit.base_model.model.model.decoder.layers[0].self_attn.v_proj, LoraLinear4bit)
 
     @require_bitsandbytes
     @pytest.mark.multi_gpu_tests
     @pytest.mark.single_gpu_tests
     def test_ia3_bnb_4bit_quantization(self):
         r"""
         Test that tests if the 4bit quantization using IA3 works as expected
@@ -412,25 +395,21 @@
             feedforward_modules=["fc2"],
             task_type="CAUSAL_LM",
         )
 
         config = IA3Config(target_modules=["q_proj", "v_proj", "fc2"], feedforward_modules=["fc2"])
 
         flan_4bit = get_peft_model(flan_4bit, flan_ia3_config)
-        self.assertTrue(
-            isinstance(flan_4bit.base_model.model.encoder.block[0].layer[0].SelfAttention.q, IA3Linear4bit)
-        )
+        assert isinstance(flan_4bit.base_model.model.encoder.block[0].layer[0].SelfAttention.q, IA3Linear4bit)
 
         opt_4bit = get_peft_model(opt_4bit, opt_ia3_config)
-        self.assertTrue(isinstance(opt_4bit.base_model.model.model.decoder.layers[0].self_attn.v_proj, IA3Linear4bit))
+        assert isinstance(opt_4bit.base_model.model.model.decoder.layers[0].self_attn.v_proj, IA3Linear4bit)
 
         whisper_4bit = get_peft_model(whisper_4bit, config)
-        self.assertTrue(
-            isinstance(whisper_4bit.base_model.model.model.decoder.layers[0].self_attn.v_proj, IA3Linear4bit)
-        )
+        assert isinstance(whisper_4bit.base_model.model.model.decoder.layers[0].self_attn.v_proj, IA3Linear4bit)
 
     @pytest.mark.multi_gpu_tests
     @require_torch_multi_gpu
     def test_lora_causal_lm_multi_gpu_inference(self):
         r"""
         Test if LORA can be used for inference on multiple GPUs.
         """
@@ -442,18 +421,18 @@
             bias="none",
             task_type="CAUSAL_LM",
         )
 
         model = AutoModelForCausalLM.from_pretrained(self.causal_lm_model_id, device_map="balanced")
         tokenizer = AutoTokenizer.from_pretrained(self.seq2seq_model_id)
 
-        self.assertEqual(set(model.hf_device_map.values()), set(range(torch.cuda.device_count())))
+        assert set(model.hf_device_map.values()) == set(range(torch.cuda.device_count()))
 
         model = get_peft_model(model, lora_config)
-        self.assertTrue(isinstance(model, PeftModel))
+        assert isinstance(model, PeftModel)
 
         dummy_input = "This is a dummy input:"
         input_ids = tokenizer(dummy_input, return_tensors="pt").input_ids.to(self.device)
 
         # this should work without any problem
         _ = model.generate(input_ids=input_ids)
 
@@ -467,19 +446,19 @@
         lora_config = LoraConfig(
             r=16, lora_alpha=32, target_modules=["q", "v"], lora_dropout=0.05, bias="none", task_type="SEQ_2_SEQ_LM"
         )
 
         model = AutoModelForSeq2SeqLM.from_pretrained(self.seq2seq_model_id, device_map="balanced", load_in_8bit=True)
         tokenizer = AutoTokenizer.from_pretrained(self.seq2seq_model_id)
 
-        self.assertEqual(set(model.hf_device_map.values()), set(range(torch.cuda.device_count())))
+        assert set(model.hf_device_map.values()) == set(range(torch.cuda.device_count()))
 
         model = get_peft_model(model, lora_config)
-        self.assertTrue(isinstance(model, PeftModel))
-        self.assertTrue(isinstance(model.base_model.model.encoder.block[0].layer[0].SelfAttention.q, LoraLinear8bitLt))
+        assert isinstance(model, PeftModel)
+        assert isinstance(model.base_model.model.encoder.block[0].layer[0].SelfAttention.q, LoraLinear8bitLt)
 
         dummy_input = "This is a dummy input:"
         input_ids = tokenizer(dummy_input, return_tensors="pt").input_ids.to(self.device)
 
         # this should work without any problem
         _ = model.generate(input_ids=input_ids)
 
@@ -543,16 +522,16 @@
 
         config = LoraConfig(
             r=8,
         )
         model = get_peft_model(model, config)
         trainable_params, all_params = model.get_nb_trainable_parameters()
 
-        self.assertEqual(trainable_params, EXPECTED_TRAINABLE_PARAMS)
-        self.assertEqual(all_params, EXPECTED_ALL_PARAMS)
+        assert trainable_params == EXPECTED_TRAINABLE_PARAMS
+        assert all_params == EXPECTED_ALL_PARAMS
 
         # test with double quant
         bnb_config = BitsAndBytesConfig(
             load_in_4bit=True,
             bnb_4bit_use_double_quant=True,
         )
 
@@ -563,16 +542,16 @@
 
         config = LoraConfig(
             r=8,
         )
         model = get_peft_model(model, config)
         trainable_params, all_params = model.get_nb_trainable_parameters()
 
-        self.assertEqual(trainable_params, EXPECTED_TRAINABLE_PARAMS)
-        self.assertEqual(all_params, EXPECTED_ALL_PARAMS)
+        assert trainable_params == EXPECTED_TRAINABLE_PARAMS
+        assert all_params == EXPECTED_ALL_PARAMS
 
     @require_torch_gpu
     @pytest.mark.single_gpu_tests
     @require_bitsandbytes
     def test_modules_to_save_grad(self):
         model_id = "bigscience/bloomz-560m"
         load_in_4bit = True
@@ -595,21 +574,21 @@
 
         peft_model = get_peft_model(model, config)
 
         lm_head = peft_model.base_model.model.score
         original_module = lm_head.original_module
         modules_to_save = lm_head.modules_to_save.default
 
-        inputs = torch.randn((1024))
+        inputs = torch.randn(1024)
         o1 = lm_head(inputs)
         o1.mean().backward()
 
-        self.assertTrue(modules_to_save.weight.requires_grad is True)
-        self.assertTrue(original_module.weight.grad is None)
-        self.assertTrue(modules_to_save.weight.grad is not None)
+        assert modules_to_save.weight.requires_grad is True
+        assert original_module.weight.grad is None
+        assert modules_to_save.weight.grad is not None
 
     @require_torch_gpu
     @pytest.mark.single_gpu_tests
     @require_bitsandbytes
     def test_8bit_merge_lora(self):
         torch.manual_seed(1000)
         model = AutoModelForCausalLM.from_pretrained(
@@ -630,23 +609,19 @@
 
         model.merge_and_unload()
         with torch.inference_mode():
             out_after_merge = F.softmax(model(random_input).logits, dim=-1)
 
         atol = 0.01
         rtol = 10
-        self.assertFalse(torch.allclose(out_base, out_before_merge, atol=atol, rtol=rtol))
-        self.assertTrue(torch.allclose(out_before_merge, out_after_merge, atol=atol, rtol=rtol))
-        self.assertTrue(isinstance(model, PeftModel))
-        self.assertTrue(
-            isinstance(model.base_model.model.model.decoder.layers[0].self_attn.q_proj, bnb.nn.Linear8bitLt)
-        )
-        self.assertTrue(
-            isinstance(model.base_model.model.model.decoder.layers[0].self_attn.v_proj, bnb.nn.Linear8bitLt)
-        )
+        assert not torch.allclose(out_base, out_before_merge, atol=atol, rtol=rtol)
+        assert torch.allclose(out_before_merge, out_after_merge, atol=atol, rtol=rtol)
+        assert isinstance(model, PeftModel)
+        assert isinstance(model.base_model.model.model.decoder.layers[0].self_attn.q_proj, bnb.nn.Linear8bitLt)
+        assert isinstance(model.base_model.model.model.decoder.layers[0].self_attn.v_proj, bnb.nn.Linear8bitLt)
 
     @require_torch_gpu
     @pytest.mark.single_gpu_tests
     @require_bitsandbytes
     def test_8bit_merge_and_disable_lora(self):
         torch.manual_seed(1000)
         model = AutoModelForCausalLM.from_pretrained(
@@ -670,19 +645,19 @@
         model.merge_adapter()
         with model.disable_adapter():
             with torch.inference_mode():
                 out_after = F.softmax(model(random_input).logits, dim=-1)
 
         atol = 0.01
         rtol = 10
-        self.assertFalse(torch.allclose(out_base, out_before, atol=atol, rtol=rtol))
-        self.assertTrue(torch.allclose(out_base, out_after, atol=atol, rtol=rtol))
-        self.assertTrue(isinstance(model, PeftModel))
-        self.assertTrue(isinstance(model.base_model.model.model.decoder.layers[0].self_attn.q_proj, LoraLinear8bitLt))
-        self.assertTrue(isinstance(model.base_model.model.model.decoder.layers[0].self_attn.v_proj, LoraLinear8bitLt))
+        assert not torch.allclose(out_base, out_before, atol=atol, rtol=rtol)
+        assert torch.allclose(out_base, out_after, atol=atol, rtol=rtol)
+        assert isinstance(model, PeftModel)
+        assert isinstance(model.base_model.model.model.decoder.layers[0].self_attn.q_proj, LoraLinear8bitLt)
+        assert isinstance(model.base_model.model.model.decoder.layers[0].self_attn.v_proj, LoraLinear8bitLt)
 
     @require_torch_gpu
     @pytest.mark.single_gpu_tests
     @require_bitsandbytes
     def test_4bit_merge_lora(self):
         torch.manual_seed(3000)
         bnb_config = BitsAndBytesConfig(
@@ -712,19 +687,19 @@
         model.merge_and_unload()
         with torch.inference_mode():
             out_after_merge = F.softmax(model(random_input).logits, dim=-1)
 
         # tolerances are pretty high because some deviations are expected with quantization
         atol = 0.01
         rtol = 10
-        self.assertFalse(torch.allclose(out_base, out_before_merge, atol=atol, rtol=rtol))
-        self.assertTrue(torch.allclose(out_before_merge, out_after_merge, atol=atol, rtol=rtol))
-        self.assertTrue(isinstance(model, PeftModel))
-        self.assertTrue(isinstance(model.base_model.model.model.decoder.layers[0].self_attn.q_proj, bnb.nn.Linear4bit))
-        self.assertTrue(isinstance(model.base_model.model.model.decoder.layers[0].self_attn.v_proj, bnb.nn.Linear4bit))
+        assert not torch.allclose(out_base, out_before_merge, atol=atol, rtol=rtol)
+        assert torch.allclose(out_before_merge, out_after_merge, atol=atol, rtol=rtol)
+        assert isinstance(model, PeftModel)
+        assert isinstance(model.base_model.model.model.decoder.layers[0].self_attn.q_proj, bnb.nn.Linear4bit)
+        assert isinstance(model.base_model.model.model.decoder.layers[0].self_attn.v_proj, bnb.nn.Linear4bit)
 
     @require_torch_gpu
     @pytest.mark.single_gpu_tests
     @require_bitsandbytes
     def test_4bit_merge_and_disable_lora(self):
         torch.manual_seed(3000)
         bnb_config = BitsAndBytesConfig(
@@ -754,19 +729,19 @@
         model.merge_adapter()
         with model.disable_adapter():
             with torch.inference_mode():
                 out_after = F.softmax(model(random_input).logits, dim=-1)
 
         atol = 0.01
         rtol = 10
-        self.assertFalse(torch.allclose(out_base, out_before, atol=atol, rtol=rtol))
-        self.assertTrue(torch.allclose(out_base, out_after, atol=atol, rtol=rtol))
-        self.assertTrue(isinstance(model, PeftModel))
-        self.assertTrue(isinstance(model.base_model.model.model.decoder.layers[0].self_attn.q_proj, LoraLinear4bit))
-        self.assertTrue(isinstance(model.base_model.model.model.decoder.layers[0].self_attn.v_proj, LoraLinear4bit))
+        assert not torch.allclose(out_base, out_before, atol=atol, rtol=rtol)
+        assert torch.allclose(out_base, out_after, atol=atol, rtol=rtol)
+        assert isinstance(model, PeftModel)
+        assert isinstance(model.base_model.model.model.decoder.layers[0].self_attn.q_proj, LoraLinear4bit)
+        assert isinstance(model.base_model.model.model.decoder.layers[0].self_attn.v_proj, LoraLinear4bit)
 
     @require_torch_gpu
     @pytest.mark.single_gpu_tests
     def test_serialization_shared_tensors(self):
         model_checkpoint = "roberta-base"
         peft_config = LoraConfig(
             task_type=TaskType.TOKEN_CLS, inference_mode=False, r=16, lora_alpha=16, lora_dropout=0.1, bias="all"
```

### Comparing `peft-0.8.2/tests/test_config.py` & `peft-0.9.0/tests/test_config.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# coding=utf-8
 # Copyright 2023-present the HuggingFace Inc. team.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
@@ -65,18 +64,18 @@
         - to_dict
         - save_pretrained
         - from_pretrained
         - from_json_file
         """
         # test if all configs have the expected methods
         config = config_class()
-        self.assertTrue(hasattr(config, "to_dict"))
-        self.assertTrue(hasattr(config, "save_pretrained"))
-        self.assertTrue(hasattr(config, "from_pretrained"))
-        self.assertTrue(hasattr(config, "from_json_file"))
+        assert hasattr(config, "to_dict")
+        assert hasattr(config, "save_pretrained")
+        assert hasattr(config, "from_pretrained")
+        assert hasattr(config, "from_json_file")
 
     @parameterized.expand(ALL_CONFIG_CLASSES)
     def test_task_type(self, config_class):
         config_class(task_type="test")
 
     def test_from_peft_type(self):
         r"""
@@ -107,33 +106,33 @@
         - save_pretrained
         """
         config = config_class()
         with tempfile.TemporaryDirectory() as tmp_dirname:
             config.save_pretrained(tmp_dirname)
 
             config_from_pretrained = config_class.from_pretrained(tmp_dirname)
-            self.assertEqual(config.to_dict(), config_from_pretrained.to_dict())
+            assert config.to_dict() == config_from_pretrained.to_dict()
 
     @parameterized.expand(ALL_CONFIG_CLASSES)
     def test_from_json_file(self, config_class):
         config = config_class()
         with tempfile.TemporaryDirectory() as tmp_dirname:
             config.save_pretrained(tmp_dirname)
 
             config_from_json = config_class.from_json_file(os.path.join(tmp_dirname, "adapter_config.json"))
-            self.assertEqual(config.to_dict(), config_from_json)
+            assert config.to_dict() == config_from_json
 
     @parameterized.expand(ALL_CONFIG_CLASSES)
     def test_to_dict(self, config_class):
         r"""
         Test if the config can be correctly converted to a dict using:
         - to_dict
         """
         config = config_class()
-        self.assertTrue(isinstance(config.to_dict(), dict))
+        assert isinstance(config.to_dict(), dict)
 
     @parameterized.expand(ALL_CONFIG_CLASSES)
     def test_from_pretrained_cache_dir(self, config_class):
         r"""
         Test if the config is correctly loaded with extra kwargs
         """
         with tempfile.TemporaryDirectory() as tmp_dirname:
@@ -143,48 +142,48 @@
 
     def test_from_pretrained_cache_dir_remote(self):
         r"""
         Test if the config is correctly loaded with a checkpoint from the hub
         """
         with tempfile.TemporaryDirectory() as tmp_dirname:
             PeftConfig.from_pretrained("ybelkada/test-st-lora", cache_dir=tmp_dirname)
-            self.assertTrue("models--ybelkada--test-st-lora" in os.listdir(tmp_dirname))
+            assert "models--ybelkada--test-st-lora" in os.listdir(tmp_dirname)
 
     @parameterized.expand(ALL_CONFIG_CLASSES)
     def test_set_attributes(self, config_class):
         # manually set attributes and check if they are correctly written
         config = config_class(peft_type="test")
 
         # save pretrained
         with tempfile.TemporaryDirectory() as tmp_dirname:
             config.save_pretrained(tmp_dirname)
 
             config_from_pretrained = config_class.from_pretrained(tmp_dirname)
-            self.assertEqual(config.to_dict(), config_from_pretrained.to_dict())
+            assert config.to_dict() == config_from_pretrained.to_dict()
 
     @parameterized.expand(ALL_CONFIG_CLASSES)
     def test_config_copy(self, config_class):
         # see https://github.com/huggingface/peft/issues/424
         config = config_class()
         copied = copy.copy(config)
-        self.assertEqual(config.to_dict(), copied.to_dict())
+        assert config.to_dict() == copied.to_dict()
 
     @parameterized.expand(ALL_CONFIG_CLASSES)
     def test_config_deepcopy(self, config_class):
         # see https://github.com/huggingface/peft/issues/424
         config = config_class()
         copied = copy.deepcopy(config)
-        self.assertEqual(config.to_dict(), copied.to_dict())
+        assert config.to_dict() == copied.to_dict()
 
     @parameterized.expand(ALL_CONFIG_CLASSES)
     def test_config_pickle_roundtrip(self, config_class):
         # see https://github.com/huggingface/peft/issues/424
         config = config_class()
         copied = pickle.loads(pickle.dumps(config))
-        self.assertEqual(config.to_dict(), copied.to_dict())
+        assert config.to_dict() == copied.to_dict()
 
     def test_prompt_encoder_warning_num_layers(self):
         # This test checks that if a prompt encoder config is created with an argument that is ignored, there should be
         # warning. However, there should be no warning if the default value is used.
         kwargs = {
             "num_virtual_tokens": 20,
             "num_transformer_submodules": 1,
@@ -208,51 +207,44 @@
     def test_save_pretrained_with_target_modules(self, config_class):
         # See #1041, #1045
         config = config_class(target_modules=["a", "list"])
         with tempfile.TemporaryDirectory() as tmp_dirname:
             config.save_pretrained(tmp_dirname)
 
             config_from_pretrained = config_class.from_pretrained(tmp_dirname)
-            self.assertEqual(config.to_dict(), config_from_pretrained.to_dict())
+            assert config.to_dict() == config_from_pretrained.to_dict()
             # explicit test that target_modules should be converted to set
-            self.assertTrue(isinstance(config_from_pretrained.target_modules, set))
+            assert isinstance(config_from_pretrained.target_modules, set)
 
     def test_regex_with_layer_indexing_lora(self):
         # This test checks that an error is raised if `target_modules` is a regex expression and `layers_to_transform` or
         # `layers_pattern` are not None
 
         invalid_config1 = {"target_modules": ".*foo", "layers_to_transform": [0]}
         invalid_config2 = {"target_modules": ".*foo", "layers_pattern": ["bar"]}
 
         valid_config = {"target_modules": ["foo"], "layers_pattern": ["bar"], "layers_to_transform": [0]}
 
-        with self.assertRaisesRegex(
-            ValueError,
-            expected_regex="`layers_to_transform` cannot be used when `target_modules` is a str.",
-        ):
+        with pytest.raises(ValueError, match="`layers_to_transform` cannot be used when `target_modules` is a str."):
             LoraConfig(**invalid_config1)
 
-        with self.assertRaisesRegex(
-            ValueError, expected_regex="`layers_pattern` cannot be used when `target_modules` is a str."
-        ):
+        with pytest.raises(ValueError, match="`layers_pattern` cannot be used when `target_modules` is a str."):
             LoraConfig(**invalid_config2)
 
         # should run without errors
         LoraConfig(**valid_config)
 
     def test_ia3_is_feedforward_subset_invalid_config(self):
         # This test checks that the IA3 config raises a value error if the feedforward_modules argument
         # is not a subset of the target_modules argument
 
         # an example invalid config
         invalid_config = {"target_modules": ["k", "v"], "feedforward_modules": ["q"]}
 
-        with self.assertRaisesRegex(
-            ValueError, expected_regex="^`feedforward_modules` should be a subset of `target_modules`$"
-        ):
+        with pytest.raises(ValueError, match="^`feedforward_modules` should be a subset of `target_modules`$"):
             IA3Config(**invalid_config)
 
     def test_ia3_is_feedforward_subset_valid_config(self):
         # This test checks that the IA3 config is created without errors with valid arguments.
         # feedforward_modules should be a subset of target_modules if both are lists
 
         # an example valid config with regex expressions.
```

### Comparing `peft-0.8.2/tests/test_custom_models.py` & `peft-0.9.0/tests/test_custom_models.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,21 +15,23 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import copy
 import os
 import tempfile
 import unittest
 
+import pytest
 import torch
 from parameterized import parameterized
 from torch import nn
 from transformers.pytorch_utils import Conv1D
 
 from peft import AdaLoraConfig, IA3Config, LoHaConfig, LoKrConfig, LoraConfig, OFTConfig, PeftModel, get_peft_model
 from peft.tuners.tuners_utils import BaseTunerLayer
+from peft.utils import ModulesToSaveWrapper
 
 from .testing_common import PeftCommonTester
 from .testing_utils import get_state_dict
 
 
 # MLP is a vanilla FF network with only linear layers
 # EmbConv1D has an embedding and a Conv1D layer
@@ -49,14 +51,22 @@
         LoraConfig,
         {
             "target_modules": ["lin0"],
             "lora_alpha": 4,
             "lora_dropout": 0.1,
         },
     ),
+    ("Vanilla MLP 7 LoRA with DoRA", "MLP", LoraConfig, {"target_modules": ["lin0"], "use_dora": True}),
+    ("Vanilla MLP 8 LoRA with DoRA", "MLP", LoraConfig, {"target_modules": ["lin0", "lin1"], "use_dora": True}),
+    (
+        "Vanilla MLP 9 LoRA with DoRA",
+        "MLP",
+        LoraConfig,
+        {"target_modules": "lin1", "use_dora": True, "lora_alpha": 32},
+    ),
     ("Embedding + transformers Conv1D 1 LoRA", "EmbConv1D", LoraConfig, {"target_modules": ["conv1d"]}),
     ("Embedding + transformers Conv1D 2 LoRA", "EmbConv1D", LoraConfig, {"target_modules": ["emb"]}),
     ("Embedding + transformers Conv1D 3 LoRA", "EmbConv1D", LoraConfig, {"target_modules": ["emb", "conv1d"]}),
     ("Conv2d 1 LoRA", "Conv2d", LoraConfig, {"target_modules": ["conv2d"]}),
     ("Conv2d 2 LoRA", "Conv2d", LoraConfig, {"target_modules": ["conv2d", "lin0"]}),
     #######
     # IA³ #
@@ -469,14 +479,16 @@
     @parameterized.expand(TEST_CASES)
     def test_merge_layers(self, test_name, model_id, config_cls, config_kwargs):
         config_kwargs = config_kwargs.copy()
         if issubclass(config_cls, LoraConfig):
             config_kwargs["init_lora_weights"] = False
         elif issubclass(config_cls, IA3Config):
             config_kwargs["init_ia3_weights"] = False
+        else:
+            config_kwargs["init_weights"] = False
         self._test_merge_layers(model_id, config_cls, config_kwargs)
 
     @parameterized.expand(TEST_CASES)
     def test_merge_layers_fp16(self, test_name, model_id, config_cls, config_kwargs):
         config_kwargs = config_kwargs.copy()
         if issubclass(config_cls, LoraConfig):
             config_kwargs["init_lora_weights"] = False
@@ -491,14 +503,26 @@
         if issubclass(config_cls, LoraConfig):
             config_kwargs["init_lora_weights"] = False
         elif issubclass(config_cls, IA3Config):
             config_kwargs["init_ia3_weights"] = False
         self._test_merge_layers_is_idempotent(model_id, config_cls, config_kwargs)
 
     @parameterized.expand(TEST_CASES)
+    def test_safe_merge(self, test_name, model_id, config_cls, config_kwargs):
+        # calling merge twice with the same arguments should not change the output
+        config_kwargs = config_kwargs.copy()
+        if issubclass(config_cls, LoraConfig):
+            config_kwargs["init_lora_weights"] = False
+        elif issubclass(config_cls, IA3Config):
+            config_kwargs["init_ia3_weights"] = False
+        else:
+            config_kwargs["init_weights"] = False
+        self._test_safe_merge(model_id, config_cls, config_kwargs)
+
+    @parameterized.expand(TEST_CASES)
     def test_generate(self, test_name, model_id, config_cls, config_kwargs):
         # Custom models do not (necessarily) have a generate method, so this test is not performed
         pass
 
     @parameterized.expand(TEST_CASES)
     def test_generate_half_prec(self, test_name, model_id, config_cls, config_kwargs):
         # Custom models do not (necessarily) have a generate method, so this test is not performed
@@ -534,19 +558,20 @@
             base_model_name_or_path=model_id,
             **config_kwargs,
         )
         model = get_peft_model(model, config)
         model.eval()
         with torch.no_grad():
             output = model(**X)
-        self.assertTrue(torch.isfinite(output).all())
+        assert torch.isfinite(output).all()
 
     @parameterized.expand(TEST_CASES)
     def test_only_params_are_updated(self, test_name, model_id, config_cls, config_kwargs):
-        # An explicit test that when using LoRA on a custom model, only the LoRA parameters are updated during training
+        # An explicit test that when using an adapter on a custom model, only the adapter parameters are updated during
+        # training
         X = self.prepare_inputs_for_testing()
         model = self.transformers_class.from_pretrained(model_id).to(self.torch_device)
         config = config_cls(
             base_model_name_or_path=model_id,
             **config_kwargs,
         )
         model = get_peft_model(model, config)
@@ -563,38 +588,39 @@
             loss = y_pred.sum()
             loss.backward()
             optimizer.step()
 
         tol = 1e-4
         params_before = dict(model_before.named_parameters())
         params_after = dict(model.named_parameters())
-        self.assertEqual(params_before.keys(), params_after.keys())
+        assert params_before.keys() == params_after.keys()
 
         prefix = PREFIXES[config_cls]
         for name, param_before in params_before.items():
             param_after = params_after[name]
             if (prefix in name) or ("modules_to_save" in name):
                 # target_modules and modules_to_save _are_ updated
-                self.assertFalse(torch.allclose(param_before, param_after, atol=tol, rtol=tol))
+                assert not torch.allclose(param_before, param_after, atol=tol, rtol=tol)
             else:
-                self.assertTrue(torch.allclose(param_before, param_after, atol=tol, rtol=tol))
+                assert torch.allclose(param_before, param_after, atol=tol, rtol=tol)
 
     @parameterized.expand(TEST_CASES)
     def test_parameters_after_loading_model(self, test_name, model_id, config_cls, config_kwargs):
         # An explicit test that when loading a trained model, the parameters are loaded correctly
         # see issue #808
         X = self.prepare_inputs_for_testing()
         model = self.transformers_class.from_pretrained(model_id).to(self.torch_device)
         config = config_cls(
             base_model_name_or_path=model_id,
             **config_kwargs,
         )
         model = get_peft_model(model, config)
         model.train()
-        optimizer = torch.optim.SGD(model.parameters(), lr=0.5)
+        lr = 0.5 if not config_kwargs.get("use_dora") else 0.1  # otherwise we get nan
+        optimizer = torch.optim.SGD(model.parameters(), lr=lr)
 
         # train at least 3 steps for all parameters to be updated (probably this is required because of symmetry
         # breaking of some LoRA layers that are initialized with constants)
         for _ in range(3):
             optimizer.zero_grad()
             y_pred = model(**X)
             loss = y_pred.sum()
@@ -608,18 +634,18 @@
 
         with tempfile.TemporaryDirectory() as tmp_dirname:
             model.save_pretrained(tmp_dirname)
             model_from_pretrained = self.transformers_class.from_pretrained(model_id).to(self.torch_device)
             model_from_pretrained = PeftModel.from_pretrained(model_from_pretrained, tmp_dirname)
             params_after = get_state_dict(model_from_pretrained)
 
-            self.assertEqual(params_before.keys(), params_after.keys())
+            assert params_before.keys() == params_after.keys()
             for name, param_before in params_before.items():
                 param_after = params_after[name]
-                self.assertTrue(torch.allclose(param_before, param_after, atol=tol, rtol=tol))
+                assert torch.allclose(param_before, param_after, atol=tol, rtol=tol)
 
     @parameterized.expand(TEST_CASES)
     def test_disable_adapters(self, test_name, model_id, config_cls, config_kwargs):
         X = self.prepare_inputs_for_testing()
         model = self.transformers_class.from_pretrained(model_id).to(self.torch_device).eval()
         outputs_base = model(**X)
 
@@ -627,15 +653,15 @@
             base_model_name_or_path=model_id,
             **config_kwargs,
         )
         model = get_peft_model(model, config)
         model.eval()
         outputs_before = model(**X)
 
-        self.assertTrue(torch.allclose(outputs_base, outputs_before))
+        assert torch.allclose(outputs_base, outputs_before)
 
         model.train()
         # EmbConv1D is slow to learn for some reason
         lr = 0.01 if model_id != "EmbConv1D" else 1.0
         optimizer = torch.optim.SGD(model.parameters(), lr=lr)
 
         # train at least 3 steps for all parameters to be updated (probably this is required because of symmetry
@@ -653,17 +679,17 @@
 
         with model.disable_adapter():
             outputs_disabled = model(**X)
 
         # check that after leaving the disable_adapter context, everything is enabled again
         outputs_enabled_after_disable = model(**X)
 
-        self.assertFalse(torch.allclose(outputs_before, outputs_after))
-        self.assertTrue(torch.allclose(outputs_before, outputs_disabled))
-        self.assertTrue(torch.allclose(outputs_after, outputs_enabled_after_disable))
+        assert not torch.allclose(outputs_before, outputs_after)
+        assert torch.allclose(outputs_before, outputs_disabled)
+        assert torch.allclose(outputs_after, outputs_enabled_after_disable)
 
     @parameterized.expand(TEST_CASES)
     def test_disable_adapters_with_merging(self, test_name, model_id, config_cls, config_kwargs):
         # same as test_disable_adapters, but with merging
         X = self.prepare_inputs_for_testing()
         model = self.transformers_class.from_pretrained(model_id).to(self.torch_device)
         config = config_cls(
@@ -686,14 +712,15 @@
             y_pred = model(**X)
             y = torch.arange(len(y_pred)).to(self.torch_device) % 2
             loss = nn.functional.nll_loss(y_pred, y)
             loss.backward()
             optimizer.step()
 
         model.eval()
+        outputs_unmerged = model(**X)
         model.merge_adapter()
         outputs_after = model(**X)
 
         with model.disable_adapter():
             outputs_disabled = model(**X)
 
         # check that after leaving the disable_adapter context, everything is enabled again
@@ -701,21 +728,24 @@
 
         atol, rtol = 1e-5, 1e-5  # tolerances higher than defaults since merging introduces some numerical instability
 
         if issubclass(config_cls, IA3Config) and model_id == "Conv2d":  # more instability with Conv2d + IA3
             atol, rtol = 1e-3, 1e-3
 
         # check that there is a difference in results after training
-        self.assertFalse(torch.allclose(outputs_before, outputs_after, atol=atol, rtol=rtol))
+        assert not torch.allclose(outputs_before, outputs_after, atol=atol, rtol=rtol)
+
+        # unmerged or merged should make no difference
+        assert torch.allclose(outputs_after, outputs_unmerged, atol=atol, rtol=rtol)
 
         # check that disabling adapters gives the same results as before training
-        self.assertTrue(torch.allclose(outputs_before, outputs_disabled, atol=atol, rtol=rtol))
+        assert torch.allclose(outputs_before, outputs_disabled, atol=atol, rtol=rtol)
 
         # check that enabling + disabling adapters does not change the results
-        self.assertTrue(torch.allclose(outputs_after, outputs_enabled_after_disable, atol=atol, rtol=rtol))
+        assert torch.allclose(outputs_after, outputs_enabled_after_disable, atol=atol, rtol=rtol)
 
     @parameterized.expand(TEST_CASES)
     def test_disable_adapter_with_bias_warns(self, test_name, model_id, config_cls, config_kwargs):
         # When training biases in lora, disabling adapters does not reset the biases, so the output is not what users
         # might expect. Therefore, a warning should be given.
 
         # Note: We test only with custom models since they run really fast. There is really no point in testing the same
@@ -737,17 +767,17 @@
             )
             peft_model = get_peft_model(model, config)
             with peft_model.disable_adapter():
                 pass  # there is nothing to be done
 
         # check that bias=all and bias=lora_only give a warning with the correct message
         msg_start = "Careful, disabling adapter layers with bias configured to be"
-        with self.assertWarns(UserWarning, msg=msg_start):
+        with pytest.warns(UserWarning, match=msg_start):
             run_with_disable(config_kwargs, bias="lora_only")
-        with self.assertWarns(UserWarning, msg=msg_start):
+        with pytest.warns(UserWarning, match=msg_start):
             run_with_disable(config_kwargs, bias="all")
 
         # For bias=none, there is no warning. Unfortunately, AFAIK unittest has no option to assert that no warning is
         # given, therefore, we check that the unittest gives us an AssertionError if we check for a warning
         bias_warning_was_given = False
         try:
             with self.assertWarns(UserWarning) as cm:
@@ -784,83 +814,82 @@
         with tempfile.TemporaryDirectory() as tmp_dirname:
             # create a model card
             text = "---\nmeta: hello\n---\nThis is a model card\n"
             with open(os.path.join(tmp_dirname, "README.md"), "w") as f:
                 f.write(text)
 
             model.save_pretrained(tmp_dirname)
-            with open(os.path.join(tmp_dirname, "README.md"), "r") as f:
+            with open(os.path.join(tmp_dirname, "README.md")) as f:
                 model_card = f.read()
 
-        self.assertIn("library_name: peft", model_card)
-        self.assertIn("meta: hello", model_card)
-        self.assertIn("This is a model card", model_card)
+        assert "library_name: peft" in model_card
+        assert "meta: hello" in model_card
+        assert "This is a model card" in model_card
 
     def test_non_existing_model_card(self):
         # ensure that if there is already a model card, it is not overwritten
         model = MLP()
         config = LoraConfig(target_modules=["lin0"])
         model = get_peft_model(model, config)
 
         with tempfile.TemporaryDirectory() as tmp_dirname:
             model.save_pretrained(tmp_dirname)
-            with open(os.path.join(tmp_dirname, "README.md"), "r") as f:
+            with open(os.path.join(tmp_dirname, "README.md")) as f:
                 model_card = f.read()
 
-        self.assertIn("library_name: peft", model_card)
+        assert "library_name: peft" in model_card
         # rough check that the model card is pre-filled
-        self.assertGreater(len(model_card), 1000)
+        assert len(model_card) > 1000
 
     @parameterized.expand(["auto", True, False])
     def test_targeting_lora_to_embedding_layer(self, save_embedding_layers):
         model = ModelEmbWithEmbeddingUtils()
         config = LoraConfig(target_modules=["embed_tokens", "lin0"], init_lora_weights=False)
         model = get_peft_model(model, config)
 
         with tempfile.TemporaryDirectory() as tmp_dirname:
             if save_embedding_layers == "auto":
                 # assert warning
                 msg_start = "Setting `save_embedding_layers` to `True` as embedding layers found in `target_modules`."
-                with self.assertWarns(UserWarning, msg=msg_start):
+                with pytest.warns(UserWarning, match=msg_start):
                     model.save_pretrained(tmp_dirname, save_embedding_layers=save_embedding_layers)
             else:
                 model.save_pretrained(tmp_dirname, save_embedding_layers=save_embedding_layers)
             from safetensors.torch import load_file as safe_load_file
 
             state_dict = safe_load_file(os.path.join(tmp_dirname, "adapter_model.safetensors"))
             if save_embedding_layers in ["auto", True]:
-                self.assertTrue("base_model.model.embed_tokens.base_layer.weight" in state_dict)
-                self.assertTrue(
-                    torch.allclose(
-                        model.base_model.model.embed_tokens.base_layer.weight,
-                        state_dict["base_model.model.embed_tokens.base_layer.weight"],
-                    )
+                assert "base_model.model.embed_tokens.base_layer.weight" in state_dict
+                assert torch.allclose(
+                    model.base_model.model.embed_tokens.base_layer.weight,
+                    state_dict["base_model.model.embed_tokens.base_layer.weight"],
                 )
             else:
-                self.assertFalse("base_model.model.embed_tokens.base_layer.weight" in state_dict)
+                assert "base_model.model.embed_tokens.base_layer.weight" not in state_dict
             del state_dict
 
     @parameterized.expand(["auto", True, False])
     def test_targeting_lora_to_embedding_layer_non_transformers(self, save_embedding_layers):
         model = ModelEmbConv1D()
         config = LoraConfig(target_modules=["emb", "lin0"], init_lora_weights=False)
         model = get_peft_model(model, config)
 
         with tempfile.TemporaryDirectory() as tmp_dirname:
             if save_embedding_layers is True:
-                # assert warning
-                msg_start = "Could not identify embedding layer(s) because the model is not a 🤗 transformers model."
-                with self.assertWarns(UserWarning, msg=msg_start):
+                with pytest.warns(
+                    UserWarning,
+                    match=r"Could not identify embedding layer\(s\) because the model is not a 🤗 transformers model\.",
+                ):
                     model.save_pretrained(tmp_dirname, save_embedding_layers=save_embedding_layers)
             else:
                 model.save_pretrained(tmp_dirname, save_embedding_layers=save_embedding_layers)
             from safetensors.torch import load_file as safe_load_file
 
             state_dict = safe_load_file(os.path.join(tmp_dirname, "adapter_model.safetensors"))
-            self.assertFalse("base_model.model.emb.base_layer.weight" in state_dict)
+            assert "base_model.model.emb.base_layer.weight" not in state_dict
             del state_dict
 
     @parameterized.expand(
         [
             LoraConfig(target_modules=["lin0"], init_lora_weights=False),
             LoKrConfig(target_modules=["lin0"], init_weights=False),
             LoHaConfig(target_modules=["lin0"], init_weights=False),
@@ -911,19 +940,42 @@
             key2 = key.replace("default", "other-name")
             assert key1 in sd_custom1
             assert key2 in sd_custom2
         for k0, k1, k2 in zip(sd_default, sd_custom1, sd_custom2):
             assert torch.allclose(sd_default[k0], sd_custom1[k1])
             assert torch.allclose(sd_default[k0], sd_custom2[k2])
 
-        self.assertFalse(torch.allclose(output_base, output_default))
-        self.assertFalse(torch.allclose(output_base, output_custom1))
-        self.assertFalse(torch.allclose(output_base, output_custom2))
-        self.assertTrue(torch.allclose(output_custom1, output_custom2))
-        self.assertTrue(torch.allclose(output_default, output_custom1))
+        assert not torch.allclose(output_base, output_default)
+        assert not torch.allclose(output_base, output_custom1)
+        assert not torch.allclose(output_base, output_custom2)
+        assert torch.allclose(output_custom1, output_custom2)
+        assert torch.allclose(output_default, output_custom1)
+
+    @parameterized.expand(["merge_and_unload", "unload"])
+    def test_double_wrapping_merge_and_unload(self, method):
+        # see issue #1485
+        from transformers import AutoModelForTokenClassification
+
+        model = AutoModelForTokenClassification.from_pretrained("hf-internal-testing/tiny-random-RobertaModel")
+        config = LoraConfig(task_type="TOKEN_CLS", target_modules="all-linear")
+        model = get_peft_model(model, config)
+
+        # first check that double-wrapping happened
+        # Note: this may get fixed in a future PR, in which case this test can be removed
+        assert isinstance(model.base_model.model.classifier, ModulesToSaveWrapper)
+        assert hasattr(model.base_model.model.classifier.original_module, "lora_A")
+        assert hasattr(model.base_model.model.classifier.modules_to_save.default, "lora_A")
+
+        # after unloading, despite double wrapping, the classifier module should be a normal nn.Linear layer
+        if method == "merge_and_unload":
+            unloaded = model.merge_and_unload()
+        else:
+            unloaded = model.unload()
+
+        assert isinstance(unloaded.classifier, nn.Linear)
 
 
 class TestMultiRankAdapter(unittest.TestCase):
     """Tests related to multirank LoRA adapters"""
 
     def test_multirank(self):
         config_1 = LoraConfig(
@@ -947,15 +999,15 @@
         # Add second adapter
         model.add_adapter("second", config_2)
 
         # Extract current and expected ranks
         rank_current = model.lin0.lora_A["second"].weight.shape[0]
         rank_expected = config_2.rank_pattern["lin0"]
 
-        self.assertTrue(rank_current == rank_expected, f"Rank {rank_current} is not equal to expected {rank_expected}")
+        assert rank_current == rank_expected, f"Rank {rank_current} is not equal to expected {rank_expected}"
 
     def test_multirank_2(self):
         rank_pattern = {}
         alpha_pattern = {}
         r = 4
         lora_alpha = 8
 
@@ -981,65 +1033,65 @@
         model.add_adapter("second", config)
 
         for adapter in ["first", "second"]:
             for key, module in model.base_model.model.named_modules():
                 if isinstance(module, BaseTunerLayer):
                     rank_expected = rank_pattern.get(key, r)
                     rank_current = module.lora_A[adapter].weight.shape[0]
-                    self.assertTrue(
-                        rank_current == rank_expected, f"Rank {rank_current} is not equal to expected {rank_expected}"
-                    )
+                    assert (
+                        rank_current == rank_expected
+                    ), f"Rank {rank_current} is not equal to expected {rank_expected}"
 
 
 class TestRepr(unittest.TestCase):
     """Tests related to the repr of adapted models"""
 
     def test_repr_lora_linear(self):
         config = LoraConfig(target_modules=["lin0"])
         model = get_peft_model(MLP(), config)
         print_output = repr(model.model.lin0)
-        self.assertTrue(print_output.startswith("lora.Linear"))
-        self.assertTrue("in_features=10" in print_output)
-        self.assertTrue("out_features=20" in print_output)
-        self.assertTrue("lora_A" in print_output)
-        self.assertTrue("lora_B" in print_output)
-        self.assertTrue("default" in print_output)
+        assert print_output.startswith("lora.Linear")
+        assert "in_features=10" in print_output
+        assert "out_features=20" in print_output
+        assert "lora_A" in print_output
+        assert "lora_B" in print_output
+        assert "default" in print_output
 
     def test_repr_lora_embedding(self):
         config = LoraConfig(target_modules=["emb"])
         model = get_peft_model(ModelEmbConv1D(), config)
         print_output = repr(model.model.emb)
-        self.assertTrue(print_output.startswith("lora.Embedding"))
-        self.assertTrue("100, 5" in print_output)
-        self.assertTrue("lora_embedding_A" in print_output)
-        self.assertTrue("lora_embedding_B" in print_output)
-        self.assertTrue("default" in print_output)
+        assert print_output.startswith("lora.Embedding")
+        assert "100, 5" in print_output
+        assert "lora_embedding_A" in print_output
+        assert "lora_embedding_B" in print_output
+        assert "default" in print_output
 
     def test_repr_lora_conv1d(self):
         config = LoraConfig(target_modules=["conv1d"])
         model = get_peft_model(ModelEmbConv1D(), config)
         print_output = repr(model.model.conv1d)
-        self.assertTrue(print_output.startswith("lora.Linear"))
-        self.assertTrue("in_features=5" in print_output)
-        self.assertTrue("out_features=1" in print_output)
-        self.assertTrue("lora_A" in print_output)
-        self.assertTrue("lora_B" in print_output)
-        self.assertTrue("default" in print_output)
+        assert print_output.startswith("lora.Linear")
+        assert "in_features=5" in print_output
+        assert "out_features=1" in print_output
+        assert "lora_A" in print_output
+        assert "lora_B" in print_output
+        assert "default" in print_output
 
     def test_repr_lora_conv2d(self):
         config = LoraConfig(target_modules=["conv2d"])
         model = get_peft_model(ModelConv2D(), config)
         print_output = repr(model.model.conv2d)
-        self.assertTrue(print_output.startswith("lora.Conv2d"))
-        self.assertTrue("5, 10" in print_output)
-        self.assertTrue("kernel_size=(3, 3)" in print_output)
-        self.assertTrue("stride=(1, 1)" in print_output)
-        self.assertTrue("lora_A" in print_output)
-        self.assertTrue("lora_B" in print_output)
-        self.assertTrue("default" in print_output)
+        assert print_output.startswith("lora.Conv2d")
+        assert "5, 10" in print_output
+        assert "kernel_size=(3, 3)" in print_output
+        assert "stride=(1, 1)" in print_output
+        assert "lora_A" in print_output
+        assert "lora_B" in print_output
+        assert "default" in print_output
 
 
 class MultipleActiveAdaptersTester(unittest.TestCase):
     """
     A test class to test the functionality of multiple active adapters.
 
     This is not specifically tied to custom models, it's just easy to test here and testing it on all types of models
@@ -1078,27 +1130,27 @@
         peft_model.set_adapter("adapter_2")
         adapter_2_output = peft_model(**X)
 
         # set ["adapter_1", "adapter_2"]
         self.set_multiple_active_adapters(peft_model, ["adapter_1", "adapter_2"])
         combined_output = peft_model(**X)
 
-        self.assertFalse(torch.allclose(adapter_1_output, adapter_2_output, atol=1e-5))
-        self.assertFalse(torch.allclose(adapter_1_output, combined_output, atol=1e-5))
-        self.assertFalse(torch.allclose(adapter_2_output, combined_output, atol=1e-5))
+        assert not torch.allclose(adapter_1_output, adapter_2_output, atol=1e-5)
+        assert not torch.allclose(adapter_1_output, combined_output, atol=1e-5)
+        assert not torch.allclose(adapter_2_output, combined_output, atol=1e-5)
 
         if tuner_method == "lora":
             # create a weighted adapter combining both adapters and check that
             # its output is same as setting multiple active adapters
             peft_model.add_weighted_adapter(
                 ["adapter_1", "adapter_2"], [1.0, 1.0], "new_combined_adapter", combination_type="cat"
             )
             peft_model.set_adapter("new_combined_adapter")
             new_combined_output = peft_model(**X)
-            self.assertTrue(torch.allclose(new_combined_output, combined_output, atol=1e-5))
+            assert torch.allclose(new_combined_output, combined_output, atol=1e-5)
 
     @parameterized.expand(MULTIPLE_ACTIVE_ADAPTERS_TEST_CASES)
     def test_multiple_active_adapters_merge_and_unmerge(
         self, test_name, tuner_method, config_cls, config_kwargs_1, config_kwargs_2
     ):
         torch.manual_seed(0)
         model = MLP(bias=tuner_method != "ia3")
@@ -1114,22 +1166,22 @@
 
         # set ["adapter_1", "adapter_2"]
         self.set_multiple_active_adapters(peft_model, ["adapter_1", "adapter_2"])
         combined_output = peft_model(**X)
 
         peft_model.merge_adapter()
         merged_combined_output = peft_model(**X)
-        self.assertTrue(torch.allclose(merged_combined_output, combined_output, atol=1e-5))
+        assert torch.allclose(merged_combined_output, combined_output, atol=1e-5)
 
         peft_model.unmerge_adapter()
 
         with peft_model.disable_adapter():
             disabled_adapter_output = peft_model(**X)
 
-        self.assertTrue(torch.allclose(disabled_adapter_output, base_output, atol=1e-4))
+        assert torch.allclose(disabled_adapter_output, base_output, atol=1e-4)
 
     @parameterized.expand(MULTIPLE_ACTIVE_ADAPTERS_TEST_CASES)
     def test_merge_layers_multi(self, test_name, tuner_method, config_cls, config_kwargs_1, config_kwargs_2):
         torch.manual_seed(0)
         model = MLP(bias=tuner_method != "ia3")
         model.eval()
 
@@ -1147,46 +1199,46 @@
         model.add_adapter("adapter-2", config_2)
         model.set_adapter("adapter-2")
         model.eval()
 
         with torch.inference_mode():
             logits_adapter_2 = model(**dummy_input)[0]
 
-        self.assertFalse(torch.allclose(logits_adapter_1, logits_adapter_2, atol=1e-3, rtol=1e-3))
+        assert not torch.allclose(logits_adapter_1, logits_adapter_2, atol=1e-3, rtol=1e-3)
 
         model.set_adapter("default")
 
         with torch.inference_mode():
             logits_adapter_1_after_set = model(**dummy_input)[0]
 
-        self.assertTrue(torch.allclose(logits_adapter_1_after_set, logits_adapter_1, atol=1e-3, rtol=1e-3))
+        assert torch.allclose(logits_adapter_1_after_set, logits_adapter_1, atol=1e-3, rtol=1e-3)
 
         model_copy = copy.deepcopy(model)
         model_copy_2 = copy.deepcopy(model)
         model_merged_all = model.merge_and_unload(adapter_names=["adapter-2", "default"])
 
         with torch.inference_mode():
             logits_merged_all = model_merged_all(**dummy_input)[0]
 
-        self.assertFalse(torch.allclose(logits_merged_all, logits_adapter_2, atol=1e-3, rtol=1e-3))
-        self.assertFalse(torch.allclose(logits_merged_all, logits_adapter_1, atol=1e-3, rtol=1e-3))
+        assert not torch.allclose(logits_merged_all, logits_adapter_2, atol=1e-3, rtol=1e-3)
+        assert not torch.allclose(logits_merged_all, logits_adapter_1, atol=1e-3, rtol=1e-3)
 
         model_merged_adapter_2 = model_copy.merge_and_unload(adapter_names=["adapter-2"])
 
         with torch.inference_mode():
             logits_merged_adapter_2 = model_merged_adapter_2(**dummy_input)[0]
 
-        self.assertTrue(torch.allclose(logits_merged_adapter_2, logits_adapter_2, atol=1e-3, rtol=1e-3))
+        assert torch.allclose(logits_merged_adapter_2, logits_adapter_2, atol=1e-3, rtol=1e-3)
 
         model_merged_adapter_default = model_copy_2.merge_and_unload(adapter_names=["default"])
 
         with torch.inference_mode():
             logits_merged_adapter_default = model_merged_adapter_default(**dummy_input)[0]
 
-        self.assertTrue(torch.allclose(logits_merged_adapter_default, logits_adapter_1, atol=1e-3, rtol=1e-3))
+        assert torch.allclose(logits_merged_adapter_default, logits_adapter_1, atol=1e-3, rtol=1e-3)
 
 
 class RequiresGradTester(unittest.TestCase):
     """Test that requires_grad is set correctly in specific circumstances
 
     # See issue #899.
 
@@ -1197,15 +1249,15 @@
 
     def check_requires_grad(self, model, *params_expected: str):
         # Check that only the given parameters have requires_grad=True, and all others have requires_grad=False.
         # Calling without arguments besides the model means that all parameters should have requires_grad=False.
         params_with_requires_grad = [name for name, param in model.named_parameters() if param.requires_grad]
         diff = set(params_expected).symmetric_difference(set(params_with_requires_grad))
         msg = f"Expected {params_expected} to require gradients, got {params_with_requires_grad}"
-        self.assertEqual(len(diff), 0, msg=msg)
+        assert len(diff) == 0, msg
 
     def test_requires_grad_modules_to_save_default(self):
         config = LoraConfig(target_modules=["lin0"], modules_to_save=["lin1"])
         peft_model = get_peft_model(MLP(), config)
 
         self.check_requires_grad(
             peft_model,
```

### Comparing `peft-0.8.2/tests/test_decoder_models.py` & `peft-0.9.0/tests/test_decoder_models.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# coding=utf-8
 # Copyright 2023-present the HuggingFace Inc. team.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
@@ -11,14 +10,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import unittest
 from unittest.mock import Mock, call, patch
 
+import pytest
 import torch
 from parameterized import parameterized
 from transformers import AutoModelForCausalLM, AutoTokenizer
 
 from peft import AdaLoraConfig, PromptTuningConfig, PromptTuningInit, get_peft_model
 
 from .testing_common import PeftCommonTester, PeftTestConfigManager
@@ -48,14 +48,15 @@
 class PeftDecoderModelTester(unittest.TestCase, PeftCommonTester):
     r"""
     Test if the PeftModel behaves as expected. This includes:
     - test if the model has the expected methods
 
     We use parametrized.expand for debugging purposes to test each model individually.
     """
+
     transformers_class = AutoModelForCausalLM
 
     def prepare_inputs_for_testing(self):
         input_ids = torch.tensor([[1, 1, 1], [1, 2, 1]]).to(self.torch_device)
         attention_mask = torch.tensor([[1, 1, 1], [1, 0, 1]]).to(self.torch_device)
 
         input_dict = {
@@ -77,15 +78,15 @@
     def test_prepare_for_training_parametrized(self, test_name, model_id, config_cls, config_kwargs):
         self._test_prepare_for_training(model_id, config_cls, config_kwargs)
 
     @parameterized.expand(PeftTestConfigManager.get_grid_parameters(FULL_GRID))
     def test_prompt_tuning_text_prepare_for_training(self, test_name, model_id, config_cls, config_kwargs):
         # Test that prompt tuning works with text init
         if config_cls != PromptTuningConfig:
-            return
+            return pytest.skip(f"This test does not apply to {config_cls}")
 
         config_kwargs = config_kwargs.copy()
         config_kwargs["prompt_tuning_init"] = PromptTuningInit.TEXT
         config_kwargs["prompt_tuning_init_text"] = "This is a test prompt."
         config_kwargs["tokenizer_name_or_path"] = model_id
         self._test_prepare_for_training(model_id, config_cls, config_kwargs)
 
@@ -110,22 +111,21 @@
             tokenizer_kwargs={"trust_remote_code": True, "foo": "bar"},
         )
         model = self.transformers_class.from_pretrained(model_id).to(self.torch_device)
         with patch("transformers.AutoTokenizer.from_pretrained", mock_autotokenizer_from_pretrained):
             model = get_peft_model(model, config)
 
         expected_call = call(model_id, trust_remote_code=True, foo="bar")
-        self.assertEqual(mock.call_args, expected_call)
+        assert mock.call_args == expected_call
 
     def test_prompt_tuning_config_invalid_args(self):
         # Raise an error when tokenizer_kwargs is used with prompt_tuning_init!='TEXT', because this argument has no
         # function in that case
         model_id = "hf-internal-testing/tiny-random-OPTForCausalLM"
-        msg = "tokenizer_kwargs only valid when using prompt_tuning_init='TEXT'."
-        with self.assertRaisesRegex(ValueError, expected_regex=msg):
+        with pytest.raises(ValueError, match="tokenizer_kwargs only valid when using prompt_tuning_init='TEXT'."):
             PromptTuningConfig(
                 base_model_name_or_path=model_id,
                 tokenizer_name_or_path=model_id,
                 num_virtual_tokens=10,
                 task_type="CAUSAL_LM",
                 prompt_tuning_init_text="This is a test prompt.",
                 prompt_tuning_init=PromptTuningInit.RANDOM,  # <= should not be used together with tokenizer_kwargs
```

### Comparing `peft-0.8.2/tests/test_encoder_decoder_models.py` & `peft-0.9.0/tests/test_encoder_decoder_models.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# coding=utf-8
 # Copyright 2023-present the HuggingFace Inc. team.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
@@ -35,14 +34,15 @@
 class PeftEncoderDecoderModelTester(unittest.TestCase, PeftCommonTester):
     r"""
     Test if the PeftModel behaves as expected. This includes:
     - test if the model has the expected methods
 
     We use parametrized.expand for debugging purposes to test each model individually.
     """
+
     transformers_class = AutoModelForSeq2SeqLM
 
     def prepare_inputs_for_testing(self):
         input_ids = torch.tensor([[1, 1, 1], [1, 2, 1]]).to(self.torch_device)
         decoder_input_ids = torch.tensor([[1, 1, 1], [1, 2, 1]]).to(self.torch_device)
         attention_mask = torch.tensor([[1, 1, 1], [1, 0, 1]]).to(self.torch_device)
```

### Comparing `peft-0.8.2/tests/test_feature_extraction_models.py` & `peft-0.9.0/tests/test_feature_extraction_models.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# coding=utf-8
 # Copyright 2023-present the HuggingFace Inc. team.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
@@ -60,14 +59,15 @@
 class PeftFeatureExtractionModelTester(unittest.TestCase, PeftCommonTester):
     r"""
     Test if the PeftModel behaves as expected. This includes:
     - test if the model has the expected methods
 
     We use parametrized.expand for debugging purposes to test each model individually.
     """
+
     transformers_class = AutoModel
 
     def prepare_inputs_for_testing(self):
         input_ids = torch.tensor([[1, 1, 1], [1, 2, 1]]).to(self.torch_device)
         attention_mask = torch.tensor([[1, 1, 1], [1, 0, 1]]).to(self.torch_device)
 
         input_dict = {
```

### Comparing `peft-0.8.2/tests/test_gpu_examples.py` & `peft-0.9.0/tests/test_gpu_examples.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,34 +1,35 @@
-# coding=utf-8
 # Copyright 2023-present the HuggingFace Inc. team.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import gc
+import importlib
 import os
 import tempfile
 import unittest
 from dataclasses import dataclass
 from typing import Any, Dict, List, Union
 
 import pytest
 import torch
 from accelerate import infer_auto_device_map
 from accelerate.test_utils.testing import run_command
 from accelerate.utils import patch_environment
 from datasets import Audio, DatasetDict, load_dataset
+from packaging import version
 from parameterized import parameterized
 from transformers import (
     AutoModelForCausalLM,
     AutoModelForSeq2SeqLM,
     AutoTokenizer,
     DataCollatorForLanguageModeling,
     Seq2SeqTrainer,
@@ -50,14 +51,16 @@
     get_peft_model,
     prepare_model_for_int8_training,
     prepare_model_for_kbit_training,
 )
 from peft.utils import SAFETENSORS_WEIGHTS_NAME
 
 from .testing_utils import (
+    require_aqlm,
+    require_auto_awq,
     require_auto_gptq,
     require_bitsandbytes,
     require_optimum,
     require_torch_gpu,
     require_torch_multi_gpu,
 )
 
@@ -68,14 +71,15 @@
 
 @dataclass
 class DataCollatorSpeechSeq2SeqWithPadding:
     r"""
     Directly copied from:
     https://github.com/huggingface/peft/blob/main/examples/int8_training/peft_bnb_whisper_large_v2_training.ipynb
     """
+
     processor: Any
 
     def __call__(self, features: List[Dict[str, Union[List[int], torch.Tensor]]]) -> Dict[str, torch.Tensor]:
         # split inputs and labels since they have to be of different lengths and need different padding methods
         # first treat the audio inputs by simply returning torch tensors
         input_features = [{"input_features": feature["input_features"]} for feature in features]
         batch = self.processor.feature_extractor.pad(input_features, return_tensors="pt")
@@ -133,15 +137,15 @@
         gc.collect()
 
     def _check_inference_finite(self, model, batch):
         # try inference without Trainer class
         training = model.training
         model.eval()
         output = model(**batch.to(model.device))
-        self.assertTrue(torch.isfinite(output.logits).all())
+        assert torch.isfinite(output.logits).all()
         model.train(training)
 
     @pytest.mark.single_gpu_tests
     def test_causal_lm_training(self):
         r"""
         Test the CausalLM training on a single GPU device. This test is a converted version of
         https://github.com/huggingface/peft/blob/main/examples/int8_training/Finetune_opt_bnb_peft.ipynb where we train
@@ -188,19 +192,19 @@
                 data_collator=DataCollatorForLanguageModeling(tokenizer, mlm=False),
             )
             model.config.use_cache = False
             trainer.train()
 
             model.cpu().save_pretrained(tmp_dir)
 
-            self.assertTrue("adapter_config.json" in os.listdir(tmp_dir))
-            self.assertTrue(SAFETENSORS_WEIGHTS_NAME in os.listdir(tmp_dir))
+            assert "adapter_config.json" in os.listdir(tmp_dir)
+            assert SAFETENSORS_WEIGHTS_NAME in os.listdir(tmp_dir)
 
             # assert loss is not None
-            self.assertIsNotNone(trainer.state.log_history[-1]["train_loss"])
+            assert trainer.state.log_history[-1]["train_loss"] is not None
 
     @pytest.mark.single_gpu_tests
     def test_causal_lm_training_4bit(self):
         r"""
         Test the CausalLM training on a single GPU device. This test is a converted version of
         https://github.com/huggingface/peft/blob/main/examples/int8_training/Finetune_opt_bnb_peft.ipynb where we train
         `opt-6.7b` on `english_quotes` dataset in few steps using 4bit base model. The test would simply fail if the
@@ -246,19 +250,19 @@
                 data_collator=DataCollatorForLanguageModeling(tokenizer, mlm=False),
             )
             model.config.use_cache = False
             trainer.train()
 
             model.cpu().save_pretrained(tmp_dir)
 
-            self.assertTrue("adapter_config.json" in os.listdir(tmp_dir))
-            self.assertTrue(SAFETENSORS_WEIGHTS_NAME in os.listdir(tmp_dir))
+            assert "adapter_config.json" in os.listdir(tmp_dir)
+            assert SAFETENSORS_WEIGHTS_NAME in os.listdir(tmp_dir)
 
             # assert loss is not None
-            self.assertIsNotNone(trainer.state.log_history[-1]["train_loss"])
+            assert trainer.state.log_history[-1]["train_loss"] is not None
 
     @pytest.mark.multi_gpu_tests
     def test_causal_lm_training_multi_gpu_4bit(self):
         r"""
         Test the CausalLM training on a multi-GPU device with 4bit base model. The test would simply fail if the
         adapters are not set correctly.
         """
@@ -266,15 +270,15 @@
         with tempfile.TemporaryDirectory() as tmp_dir:
             model = AutoModelForCausalLM.from_pretrained(
                 self.causal_lm_model_id,
                 device_map="auto",
                 load_in_4bit=True,
             )
 
-            self.assertEqual(set(model.hf_device_map.values()), set(range(torch.cuda.device_count())))
+            assert set(model.hf_device_map.values()) == set(range(torch.cuda.device_count()))
 
             model = prepare_model_for_kbit_training(model)
 
             setattr(model, "model_parallel", True)
             setattr(model, "is_parallelizable", True)
 
             config = LoraConfig(
@@ -307,19 +311,19 @@
                 data_collator=DataCollatorForLanguageModeling(self.tokenizer, mlm=False),
             )
             model.config.use_cache = False
             trainer.train()
 
             model.cpu().save_pretrained(tmp_dir)
 
-            self.assertTrue("adapter_config.json" in os.listdir(tmp_dir))
-            self.assertTrue(SAFETENSORS_WEIGHTS_NAME in os.listdir(tmp_dir))
+            assert "adapter_config.json" in os.listdir(tmp_dir)
+            assert SAFETENSORS_WEIGHTS_NAME in os.listdir(tmp_dir)
 
             # assert loss is not None
-            self.assertIsNotNone(trainer.state.log_history[-1]["train_loss"])
+            assert trainer.state.log_history[-1]["train_loss"] is not None
 
     @pytest.mark.single_gpu_tests
     @require_torch_gpu
     def test_4bit_adalora_causalLM(self):
         r"""
         Tests the 4bit training with adalora
         """
@@ -371,19 +375,19 @@
                 data_collator=DataCollatorForLanguageModeling(tokenizer, mlm=False),
             )
             model.config.use_cache = False
             trainer.train()
 
             model.cpu().save_pretrained(tmp_dir)
 
-            self.assertTrue("adapter_config.json" in os.listdir(tmp_dir))
-            self.assertTrue(SAFETENSORS_WEIGHTS_NAME in os.listdir(tmp_dir))
+            assert "adapter_config.json" in os.listdir(tmp_dir)
+            assert SAFETENSORS_WEIGHTS_NAME in os.listdir(tmp_dir)
 
             # assert loss is not None
-            self.assertIsNotNone(trainer.state.log_history[-1]["train_loss"])
+            assert trainer.state.log_history[-1]["train_loss"] is not None
 
     @pytest.mark.single_gpu_tests
     @require_torch_gpu
     def test_8bit_adalora_causalLM(self):
         r"""
         Tests the 8bit training with adalora
         """
@@ -434,19 +438,19 @@
                 data_collator=DataCollatorForLanguageModeling(tokenizer, mlm=False),
             )
             model.config.use_cache = False
             trainer.train()
 
             model.cpu().save_pretrained(tmp_dir)
 
-            self.assertTrue("adapter_config.json" in os.listdir(tmp_dir))
-            self.assertTrue(SAFETENSORS_WEIGHTS_NAME in os.listdir(tmp_dir))
+            assert "adapter_config.json" in os.listdir(tmp_dir)
+            assert SAFETENSORS_WEIGHTS_NAME in os.listdir(tmp_dir)
 
             # assert loss is not None
-            self.assertIsNotNone(trainer.state.log_history[-1]["train_loss"])
+            assert trainer.state.log_history[-1]["train_loss"] is not None
 
     @pytest.mark.multi_gpu_tests
     @require_torch_multi_gpu
     def test_causal_lm_training_multi_gpu(self):
         r"""
         Test the CausalLM training on a multi-GPU device. This test is a converted version of
         https://github.com/huggingface/peft/blob/main/examples/int8_training/Finetune_opt_bnb_peft.ipynb where we train
@@ -456,15 +460,15 @@
         with tempfile.TemporaryDirectory() as tmp_dir:
             model = AutoModelForCausalLM.from_pretrained(
                 self.causal_lm_model_id,
                 load_in_8bit=True,
                 device_map="auto",
             )
 
-            self.assertEqual(set(model.hf_device_map.values()), set(range(torch.cuda.device_count())))
+            assert set(model.hf_device_map.values()) == set(range(torch.cuda.device_count()))
 
             tokenizer = AutoTokenizer.from_pretrained(self.causal_lm_model_id)
             model = prepare_model_for_int8_training(model)
 
             setattr(model, "model_parallel", True)
             setattr(model, "is_parallelizable", True)
 
@@ -498,19 +502,19 @@
                 data_collator=DataCollatorForLanguageModeling(tokenizer, mlm=False),
             )
             model.config.use_cache = False
             trainer.train()
 
             model.cpu().save_pretrained(tmp_dir)
 
-            self.assertTrue("adapter_config.json" in os.listdir(tmp_dir))
-            self.assertTrue(SAFETENSORS_WEIGHTS_NAME in os.listdir(tmp_dir))
+            assert "adapter_config.json" in os.listdir(tmp_dir)
+            assert SAFETENSORS_WEIGHTS_NAME in os.listdir(tmp_dir)
 
             # assert loss is not None
-            self.assertIsNotNone(trainer.state.log_history[-1]["train_loss"])
+            assert trainer.state.log_history[-1]["train_loss"] is not None
 
     @pytest.mark.single_gpu_tests
     def test_seq2seq_lm_training_single_gpu(self):
         r"""
         Test the Seq2SeqLM training on a single GPU device. This test is a converted version of
         https://github.com/huggingface/peft/blob/main/examples/int8_training/Finetune_opt_bnb_peft.ipynb where we train
         `flan-large` on `english_quotes` dataset in few steps. The test would simply fail if the adapters are not set
@@ -519,15 +523,15 @@
         with tempfile.TemporaryDirectory() as tmp_dir:
             model = AutoModelForSeq2SeqLM.from_pretrained(
                 self.seq2seq_model_id,
                 load_in_8bit=True,
                 device_map={"": 0},
             )
 
-            self.assertEqual(set(model.hf_device_map.values()), {0})
+            assert set(model.hf_device_map.values()) == {0}
 
             tokenizer = AutoTokenizer.from_pretrained(self.seq2seq_model_id)
             model = prepare_model_for_int8_training(model)
 
             config = LoraConfig(
                 r=16,
                 lora_alpha=32,
@@ -558,19 +562,19 @@
                 data_collator=DataCollatorForLanguageModeling(tokenizer, mlm=False),
             )
             model.config.use_cache = False
             trainer.train()
 
             model.cpu().save_pretrained(tmp_dir)
 
-            self.assertTrue("adapter_config.json" in os.listdir(tmp_dir))
-            self.assertTrue(SAFETENSORS_WEIGHTS_NAME in os.listdir(tmp_dir))
+            assert "adapter_config.json" in os.listdir(tmp_dir)
+            assert SAFETENSORS_WEIGHTS_NAME in os.listdir(tmp_dir)
 
             # assert loss is not None
-            self.assertIsNotNone(trainer.state.log_history[-1]["train_loss"])
+            assert trainer.state.log_history[-1]["train_loss"] is not None
 
     @pytest.mark.multi_gpu_tests
     @require_torch_multi_gpu
     def test_seq2seq_lm_training_multi_gpu(self):
         r"""
         Test the Seq2SeqLM training on a multi-GPU device. This test is a converted version of
         https://github.com/huggingface/peft/blob/main/examples/int8_training/Finetune_opt_bnb_peft.ipynb where we train
@@ -580,15 +584,15 @@
         with tempfile.TemporaryDirectory() as tmp_dir:
             model = AutoModelForSeq2SeqLM.from_pretrained(
                 self.seq2seq_model_id,
                 load_in_8bit=True,
                 device_map="balanced",
             )
 
-            self.assertEqual(set(model.hf_device_map.values()), set(range(torch.cuda.device_count())))
+            assert set(model.hf_device_map.values()) == set(range(torch.cuda.device_count()))
 
             tokenizer = AutoTokenizer.from_pretrained(self.seq2seq_model_id)
             model = prepare_model_for_int8_training(model)
 
             config = LoraConfig(
                 r=16,
                 lora_alpha=32,
@@ -619,19 +623,19 @@
                 data_collator=DataCollatorForLanguageModeling(tokenizer, mlm=False),
             )
             model.config.use_cache = False
             trainer.train()
 
             model.cpu().save_pretrained(tmp_dir)
 
-            self.assertTrue("adapter_config.json" in os.listdir(tmp_dir))
-            self.assertTrue(SAFETENSORS_WEIGHTS_NAME in os.listdir(tmp_dir))
+            assert "adapter_config.json" in os.listdir(tmp_dir)
+            assert SAFETENSORS_WEIGHTS_NAME in os.listdir(tmp_dir)
 
             # assert loss is not None
-            self.assertIsNotNone(trainer.state.log_history[-1]["train_loss"])
+            assert trainer.state.log_history[-1]["train_loss"] is not None
 
     @pytest.mark.single_gpu_tests
     def test_audio_model_training(self):
         r"""
         Test the audio model training on a single GPU device. This test is a converted version of
         https://github.com/huggingface/peft/blob/main/examples/int8_training/peft_bnb_whisper_large_v2_training.ipynb
         """
@@ -717,19 +721,19 @@
                 tokenizer=processor.feature_extractor,
             )
 
             trainer.train()
 
             model.cpu().save_pretrained(tmp_dir)
 
-            self.assertTrue("adapter_config.json" in os.listdir(tmp_dir))
-            self.assertTrue(SAFETENSORS_WEIGHTS_NAME in os.listdir(tmp_dir))
+            assert "adapter_config.json" in os.listdir(tmp_dir)
+            assert SAFETENSORS_WEIGHTS_NAME in os.listdir(tmp_dir)
 
             # assert loss is not None
-            self.assertIsNotNone(trainer.state.log_history[-1]["train_loss"])
+            assert trainer.state.log_history[-1]["train_loss"] is not None
 
     @pytest.mark.single_gpu_tests
     def test_4bit_non_default_adapter_name(self):
         # See PR 1294
         config = LoraConfig(
             r=16,
             target_modules=["q_proj", "v_proj"],
@@ -753,17 +757,18 @@
             device_map="auto",
             load_in_4bit=True,
         )
         model = prepare_model_for_kbit_training(model)
         model = get_peft_model(model, config, adapter_name="other")
         n_trainable_other, n_total_other = model.get_nb_trainable_parameters()
 
-        self.assertGreater(n_trainable_other, 0)  # sanity check
-        self.assertEqual(n_trainable_default, n_trainable_other)
-        self.assertEqual(n_total_default, n_total_other)
+        assert n_trainable_other > 0
+        # sanity check
+        assert n_trainable_default == n_trainable_other
+        assert n_total_default == n_total_other
 
     @pytest.mark.single_gpu_tests
     def test_8bit_non_default_adapter_name(self):
         # See PR 1294
         config = LoraConfig(
             r=16,
             target_modules=["q_proj", "v_proj"],
@@ -787,17 +792,18 @@
             device_map="auto",
             load_in_8bit=True,
         )
         model = prepare_model_for_kbit_training(model)
         model = get_peft_model(model, config, adapter_name="other")
         n_trainable_other, n_total_other = model.get_nb_trainable_parameters()
 
-        self.assertGreater(n_trainable_other, 0)  # sanity check
-        self.assertEqual(n_trainable_default, n_trainable_other)
-        self.assertEqual(n_total_default, n_total_other)
+        assert n_trainable_other > 0
+        # sanity check
+        assert n_trainable_default == n_trainable_other
+        assert n_total_default == n_total_other
 
 
 @require_torch_gpu
 @require_auto_gptq
 @require_optimum
 class PeftGPTQGPUTests(unittest.TestCase):
     r"""
@@ -821,15 +827,15 @@
         torch.cuda.empty_cache()
 
     def _check_inference_finite(self, model, batch):
         # try inference without Trainer class
         training = model.training
         model.eval()
         output = model(**batch.to(model.device))
-        self.assertTrue(torch.isfinite(output.logits).all())
+        assert torch.isfinite(output.logits).all()
         model.train(training)
 
     @pytest.mark.single_gpu_tests
     def test_causal_lm_training(self):
         r"""
         Test the CausalLM training on a single GPU device. The test would simply fail if the adapters are not set
         correctly.
@@ -872,19 +878,19 @@
                 data_collator=DataCollatorForLanguageModeling(self.tokenizer, mlm=False),
             )
             model.config.use_cache = False
             trainer.train()
 
             model.cpu().save_pretrained(tmp_dir)
 
-            self.assertTrue("adapter_config.json" in os.listdir(tmp_dir))
-            self.assertTrue(SAFETENSORS_WEIGHTS_NAME in os.listdir(tmp_dir))
+            assert "adapter_config.json" in os.listdir(tmp_dir)
+            assert SAFETENSORS_WEIGHTS_NAME in os.listdir(tmp_dir)
 
             # assert loss is not None
-            self.assertIsNotNone(trainer.state.log_history[-1]["train_loss"])
+            assert trainer.state.log_history[-1]["train_loss"] is not None
 
     @pytest.mark.single_gpu_tests
     def test_adalora_causalLM(self):
         r"""
         Tests the gptq training with adalora
         """
 
@@ -937,19 +943,19 @@
                 data_collator=DataCollatorForLanguageModeling(self.tokenizer, mlm=False),
             )
             model.config.use_cache = False
             trainer.train()
 
             model.cpu().save_pretrained(tmp_dir)
 
-            self.assertTrue("adapter_config.json" in os.listdir(tmp_dir))
-            self.assertTrue(SAFETENSORS_WEIGHTS_NAME in os.listdir(tmp_dir))
+            assert "adapter_config.json" in os.listdir(tmp_dir)
+            assert SAFETENSORS_WEIGHTS_NAME in os.listdir(tmp_dir)
 
             # assert loss is not None
-            self.assertIsNotNone(trainer.state.log_history[-1]["train_loss"])
+            assert trainer.state.log_history[-1]["train_loss"] is not None
 
     @pytest.mark.multi_gpu_tests
     @require_torch_multi_gpu
     def test_causal_lm_training_multi_gpu(self):
         r"""
         Test the CausalLM training on a multi-GPU device. The test would simply fail if the adapters are not set
         correctly.
@@ -959,15 +965,15 @@
             model = AutoModelForCausalLM.from_pretrained(
                 self.causal_lm_model_id,
                 torch_dtype=torch.float16,
                 device_map="auto",
                 quantization_config=self.quantization_config,
             )
 
-            self.assertEqual(set(model.hf_device_map.values()), set(range(torch.cuda.device_count())))
+            assert set(model.hf_device_map.values()) == set(range(torch.cuda.device_count()))
 
             model = prepare_model_for_kbit_training(model)
 
             setattr(model, "model_parallel", True)
             setattr(model, "is_parallelizable", True)
 
             config = LoraConfig(
@@ -1000,19 +1006,19 @@
                 data_collator=DataCollatorForLanguageModeling(self.tokenizer, mlm=False),
             )
             model.config.use_cache = False
             trainer.train()
 
             model.cpu().save_pretrained(tmp_dir)
 
-            self.assertTrue("adapter_config.json" in os.listdir(tmp_dir))
-            self.assertTrue(SAFETENSORS_WEIGHTS_NAME in os.listdir(tmp_dir))
+            assert "adapter_config.json" in os.listdir(tmp_dir)
+            assert SAFETENSORS_WEIGHTS_NAME in os.listdir(tmp_dir)
 
             # assert loss is not None
-            self.assertIsNotNone(trainer.state.log_history[-1]["train_loss"])
+            assert trainer.state.log_history[-1]["train_loss"] is not None
 
     @pytest.mark.single_gpu_tests
     def test_non_default_adapter_name(self):
         # See issue 1346
         config = LoraConfig(
             r=16,
             target_modules=["q_proj", "v_proj"],
@@ -1037,17 +1043,18 @@
             device_map="auto",
             quantization_config=self.quantization_config,
         )
         model = prepare_model_for_kbit_training(model)
         model = get_peft_model(model, config, adapter_name="other")
         n_trainable_other, n_total_other = model.get_nb_trainable_parameters()
 
-        self.assertGreater(n_trainable_other, 0)  # sanity check
-        self.assertEqual(n_trainable_default, n_trainable_other)
-        self.assertEqual(n_total_default, n_total_other)
+        assert n_trainable_other > 0
+        # sanity check
+        assert n_trainable_default == n_trainable_other
+        assert n_total_default == n_total_other
 
 
 @require_torch_gpu
 class OffloadSaveTests(unittest.TestCase):
     def setUp(self):
         self.causal_lm_model_id = "gpt2"
 
@@ -1068,45 +1075,45 @@
         torch.manual_seed(0)
         model = AutoModelForCausalLM.from_pretrained(self.causal_lm_model_id)
         tokenizer = AutoTokenizer.from_pretrained(self.causal_lm_model_id)
         # TODO: add disk offload once PeftModel.from_pretrained supports
         memory_limits = {0: "0.4GIB", "cpu": "5GIB"}
         # offloads around half of all transformer modules
         device_map = infer_auto_device_map(model, max_memory=memory_limits)
-        self.assertTrue(0 in device_map.values())
-        self.assertTrue("cpu" in device_map.values())
+        assert 0 in device_map.values()
+        assert "cpu" in device_map.values()
 
         config = LoraConfig(task_type="CAUSAL_LM", init_lora_weights=False, target_modules=["c_attn"])
 
         model = get_peft_model(model, config)
         with tempfile.TemporaryDirectory() as tmp_dir:
             model.save_pretrained(tmp_dir)
             # load the model with device_map
             model = AutoModelForCausalLM.from_pretrained(self.causal_lm_model_id, device_map=device_map).eval()
-            self.assertTrue(len({p.device for p in model.parameters()}) == 2)
+            assert len({p.device for p in model.parameters()}) == 2
             model = PeftModel.from_pretrained(model, tmp_dir, max_memory=memory_limits)
 
         input_tokens = tokenizer.encode("Four score and seven years ago", return_tensors="pt")
         model.eval()
 
         # test peft model adapter merge
         pre_merge_olayer = model(input_tokens)[0]
         model.merge_adapter()
         post_merge_olayer = model(input_tokens)[0]
-        self.assertTrue(torch.allclose(post_merge_olayer, pre_merge_olayer))
+        assert torch.allclose(post_merge_olayer, pre_merge_olayer)
 
         # test peft model adapter unmerge
         model.unmerge_adapter()
         post_unmerge_olayer = model(input_tokens)[0]
-        self.assertTrue(torch.allclose(post_unmerge_olayer, pre_merge_olayer))
+        assert torch.allclose(post_unmerge_olayer, pre_merge_olayer)
 
         # test LoRA merge and unload
         model = model.merge_and_unload()
         post_unload_merge_olayer = model(input_tokens)[0]
-        self.assertTrue(torch.allclose(post_unload_merge_olayer, pre_merge_olayer))
+        assert torch.allclose(post_unload_merge_olayer, pre_merge_olayer)
 
 
 @require_torch_gpu
 class LoftQTests(unittest.TestCase):
     r"""
     Tests for LoftQ to ensure that it reduces the quantization error compared to normal LoRA quantization.
     """
@@ -1199,100 +1206,100 @@
         # using LoftQ. When quantizing, we expect a certain level of error. However, we expect the LoftQ quantized
         # model to have less error than the normal LoRA quantized model. Note that when using normal LoRA, the
         # quantization error is simply the error from quantization without LoRA, as LoRA is a no-op before training.
         # We still apply LoRA for the test for consistency.
 
         mae_quantized, mse_quantized, mae_loftq, mse_loftq = self.get_errors(bits=4, device=device)
         # first, sanity check that all errors are > 0.0
-        self.assertTrue(mae_quantized > 0.0)
-        self.assertTrue(mse_quantized > 0.0)
-        self.assertTrue(mae_loftq > 0.0)
-        self.assertTrue(mse_loftq > 0.0)
+        assert mae_quantized > 0.0
+        assert mse_quantized > 0.0
+        assert mae_loftq > 0.0
+        assert mse_loftq > 0.0
 
         # next, check that LoftQ quantization errors are smaller than LoRA errors by a certain margin
         factor = 3
-        self.assertTrue(mae_loftq < mae_quantized / factor)
-        self.assertTrue(mse_loftq < mse_quantized / factor)
+        assert mae_loftq < (mae_quantized / factor)
+        assert mse_loftq < (mse_quantized / factor)
 
     @parameterized.expand(["cuda", "cpu"])
     def test_bloomz_loftq_4bit_iter_5(self, device):
         # Same test as the previous one but with 5 iterations. We should expect the error to be even smaller with more
         # iterations, but in practice the difference is not that large, at least not for this small base model.
         mae_quantized, mse_quantized, mae_loftq, mse_loftq = self.get_errors(bits=4, loftq_iter=5, device=device)
         # first, sanity check that all errors are > 0.0
-        self.assertTrue(mae_quantized > 0.0)
-        self.assertTrue(mse_quantized > 0.0)
-        self.assertTrue(mae_loftq > 0.0)
-        self.assertTrue(mse_loftq > 0.0)
+        assert mae_quantized > 0.0
+        assert mse_quantized > 0.0
+        assert mae_loftq > 0.0
+        assert mse_loftq > 0.0
 
         # next, check that LoftQ quantization errors are smaller than LoRA errors by a certain margin
-        self.assertTrue(mae_loftq < mae_quantized / self.error_factor)
-        self.assertTrue(mse_loftq < mse_quantized / self.error_factor)
+        assert mae_loftq < (mae_quantized / self.error_factor)
+        assert mse_loftq < (mse_quantized / self.error_factor)
 
     @parameterized.expand(["cuda", "cpu"])
     def test_bloomz_loftq_8bit(self, device):
         # Same test as test_bloomz_loftq_4bit but with 8 bits.
         mae_quantized, mse_quantized, mae_loftq, mse_loftq = self.get_errors(bits=8, device=device)
 
         # first, sanity check that all errors are > 0.0
-        self.assertTrue(mae_quantized > 0.0)
-        self.assertTrue(mse_quantized > 0.0)
-        self.assertTrue(mae_loftq > 0.0)
-        self.assertTrue(mse_loftq > 0.0)
+        assert mae_quantized > 0.0
+        assert mse_quantized > 0.0
+        assert mae_loftq > 0.0
+        assert mse_loftq > 0.0
 
         # next, check that LoftQ quantization errors are smaller than LoRA errors by a certain margin
-        self.assertTrue(mae_loftq < mae_quantized / self.error_factor)
-        self.assertTrue(mse_loftq < mse_quantized / self.error_factor)
+        assert mae_loftq < (mae_quantized / self.error_factor)
+        assert mse_loftq < (mse_quantized / self.error_factor)
 
     @parameterized.expand(["cuda", "cpu"])
     def test_bloomz_loftq_8bit_iter_5(self, device):
         # Same test as test_bloomz_loftq_4bit_iter_5 but with 8 bits.
         mae_quantized, mse_quantized, mae_loftq, mse_loftq = self.get_errors(bits=8, loftq_iter=5, device=device)
 
         # first, sanity check that all errors are > 0.0
-        self.assertTrue(mae_quantized > 0.0)
-        self.assertTrue(mse_quantized > 0.0)
-        self.assertTrue(mae_loftq > 0.0)
-        self.assertTrue(mse_loftq > 0.0)
+        assert mae_quantized > 0.0
+        assert mse_quantized > 0.0
+        assert mae_loftq > 0.0
+        assert mse_loftq > 0.0
 
         # next, check that LoftQ quantization errors are smaller than LoRA errors by a certain margin
-        self.assertTrue(mae_loftq < mae_quantized / self.error_factor)
-        self.assertTrue(mse_loftq < mse_quantized / self.error_factor)
+        assert mae_loftq < (mae_quantized / self.error_factor)
+        assert mse_loftq < (mse_quantized / self.error_factor)
 
     @parameterized.expand(["cuda", "cpu"])
     def test_t5_loftq_4bit(self, device):
         mae_quantized, mse_quantized, mae_loftq, mse_loftq = self.get_errors(
             bits=4, device=device, model_id="t5-small"
         )
         # first, sanity check that all errors are > 0.0
-        self.assertTrue(mae_quantized > 0.0)
-        self.assertTrue(mse_quantized > 0.0)
-        self.assertTrue(mae_loftq > 0.0)
-        self.assertTrue(mse_loftq > 0.0)
+        assert mae_quantized > 0.0
+        assert mse_quantized > 0.0
+        assert mae_loftq > 0.0
+        assert mse_loftq > 0.0
 
         # next, check that LoftQ quantization errors are smaller than LoRA errors by a certain margin
         factor = 3
-        self.assertTrue(mae_loftq < mae_quantized / factor)
-        self.assertTrue(mse_loftq < mse_quantized / factor)
+        assert mae_loftq < (mae_quantized / factor)
+        assert mse_loftq < (mse_quantized / factor)
 
     @parameterized.expand(["cuda", "cpu"])
     def test_t5_loftq_8bit(self, device):
         mae_quantized, mse_quantized, mae_loftq, mse_loftq = self.get_errors(
             bits=8, device=device, model_id="t5-small"
         )
         # first, sanity check that all errors are > 0.0
-        self.assertTrue(mae_quantized > 0.0)
-        self.assertTrue(mse_quantized > 0.0)
-        self.assertTrue(mae_loftq > 0.0)
-        self.assertTrue(mse_loftq > 0.0)
+        assert mae_quantized > 0.0
+        assert mse_quantized > 0.0
+        assert mae_loftq > 0.0
+        assert mse_loftq > 0.0
 
         # next, check that LoftQ quantization errors are smaller than LoRA errors by a certain margin
         factor = 3
-        self.assertTrue(mae_loftq < mae_quantized / factor)
-        self.assertTrue(mse_loftq < mse_quantized / factor)
+        assert mae_loftq < (mae_quantized / factor)
+        assert mse_loftq < (mse_quantized / factor)
 
 
 @require_bitsandbytes
 @require_torch_gpu
 class MultiprocessTester(unittest.TestCase):
     def test_notebook_launcher(self):
         script_path = os.path.join("scripts", "launch_notebook_mp.py")
@@ -1343,16 +1350,15 @@
                 args=TrainingArguments(
                     fp16=True,  # <= this is required for the error to be raised
                     logging_steps=1,
                     output_dir=tmp_dir,
                 ),
                 data_collator=DataCollatorForLanguageModeling(self.tokenizer, mlm=False),
             )
-            msg = "Attempting to unscale FP16 gradients."
-            with self.assertRaisesRegex(ValueError, msg):
+            with pytest.raises(ValueError, match="Attempting to unscale FP16 gradients."):
                 trainer.train()
 
     @pytest.mark.single_gpu_tests
     def test_model_loaded_in_float16_working(self):
         # Same test as before but containing the fix to make it work
         model = AutoModelForCausalLM.from_pretrained(
             self.causal_lm_model_id,
@@ -1374,7 +1380,344 @@
                     fp16=True,
                     max_steps=3,
                     output_dir=tmp_dir,
                 ),
                 data_collator=DataCollatorForLanguageModeling(self.tokenizer, mlm=False),
             )
             trainer.train()
+
+
+@require_torch_gpu
+@require_aqlm
+@unittest.skipUnless(
+    version.parse(importlib.metadata.version("transformers")) >= version.parse("4.38.0"),
+    "test requires `transformers>=4.38.0`",
+)
+class PeftAqlmGPUTests(unittest.TestCase):
+    r"""
+    AQLM + peft tests
+    """
+
+    def setUp(self):
+        self.causal_lm_model_id = "BlackSamorez/TinyLlama-1_1B-Chat-v1_0-AQLM-2Bit-1x16-hf"
+        self.tokenizer = AutoTokenizer.from_pretrained(self.causal_lm_model_id)
+
+    def tearDown(self):
+        r"""
+        Efficient mechanism to free GPU memory after each test. Based on
+        https://github.com/huggingface/transformers/issues/21094
+        """
+        gc.collect()
+        torch.cuda.empty_cache()
+
+    def _check_inference_finite(self, model, batch):
+        # try inference without Trainer class
+        training = model.training
+        model.eval()
+        output = model(**batch.to(model.device))
+        assert torch.isfinite(output.logits).all()
+        model.train(training)
+
+    @pytest.mark.single_gpu_tests
+    def test_causal_lm_training_aqlm(self):
+        r"""
+        Test the CausalLM training on a single GPU device. The test would simply fail if the adapters are not set
+        correctly.
+        """
+        with tempfile.TemporaryDirectory() as tmp_dir:
+            model = AutoModelForCausalLM.from_pretrained(
+                self.causal_lm_model_id,
+                device_map="cuda",
+                torch_dtype="auto",
+            )
+
+            model = prepare_model_for_kbit_training(model)
+            config = LoraConfig(
+                r=16,
+                lora_alpha=32,
+                target_modules=["q_proj", "v_proj"],
+                lora_dropout=0.05,
+                bias="none",
+                task_type="CAUSAL_LM",
+            )
+            model = get_peft_model(model, config)
+
+            data = load_dataset("ybelkada/english_quotes_copy")
+            data = data.map(lambda samples: self.tokenizer(samples["quote"]), batched=True)
+
+            trainer = Trainer(
+                model=model,
+                train_dataset=data["train"],
+                args=TrainingArguments(
+                    per_device_train_batch_size=4,
+                    gradient_accumulation_steps=4,
+                    warmup_steps=2,
+                    max_steps=3,
+                    learning_rate=2e-4,
+                    logging_steps=1,
+                    output_dir=tmp_dir,
+                    fp16=True,
+                ),
+                data_collator=DataCollatorForLanguageModeling(self.tokenizer, mlm=False),
+            )
+            model.config.use_cache = False
+            trainer.train()
+
+            model.cpu().save_pretrained(tmp_dir)
+
+            assert "adapter_config.json" in os.listdir(tmp_dir)
+            assert SAFETENSORS_WEIGHTS_NAME in os.listdir(tmp_dir)
+
+            # assert loss is not None
+            assert trainer.state.log_history[-1]["train_loss"] is not None
+
+
+@require_torch_gpu
+@require_auto_awq
+class PeftAwqGPUTests(unittest.TestCase):
+    r"""
+    Awq + peft tests
+    """
+
+    def setUp(self):
+        self.causal_lm_model_id = "peft-internal-testing/opt-125m-awq"
+        self.tokenizer = AutoTokenizer.from_pretrained(self.causal_lm_model_id)
+
+    def tearDown(self):
+        r"""
+        Efficient mechanism to free GPU memory after each test. Based on
+        https://github.com/huggingface/transformers/issues/21094
+        """
+        gc.collect()
+        torch.cuda.empty_cache()
+
+    def _check_inference_finite(self, model, batch):
+        # try inference without Trainer class
+        training = model.training
+        model.eval()
+        output = model(**batch.to(model.device))
+        assert torch.isfinite(output.logits).all()
+        model.train(training)
+
+    @pytest.mark.single_gpu_tests
+    def test_causal_lm_training_awq(self):
+        r"""
+        Test the CausalLM training on a single GPU device. The test would simply fail if the adapters are not set
+        correctly.
+        """
+        with tempfile.TemporaryDirectory() as tmp_dir:
+            model = AutoModelForCausalLM.from_pretrained(
+                self.causal_lm_model_id,
+                device_map="auto",
+            )
+
+            model = prepare_model_for_kbit_training(model)
+            config = LoraConfig(
+                r=16,
+                lora_alpha=32,
+                target_modules=["q_proj", "v_proj"],
+                lora_dropout=0.05,
+                bias="none",
+                task_type="CAUSAL_LM",
+            )
+            model = get_peft_model(model, config)
+
+            data = load_dataset("ybelkada/english_quotes_copy")
+            data = data.map(lambda samples: self.tokenizer(samples["quote"]), batched=True)
+
+            # TODO: deal correctly with this case in transformers
+            model._is_quantized_training_enabled = True
+
+            trainer = Trainer(
+                model=model,
+                train_dataset=data["train"],
+                args=TrainingArguments(
+                    per_device_train_batch_size=4,
+                    gradient_accumulation_steps=4,
+                    warmup_steps=2,
+                    max_steps=3,
+                    learning_rate=2e-4,
+                    logging_steps=1,
+                    output_dir=tmp_dir,
+                    fp16=True,
+                ),
+                data_collator=DataCollatorForLanguageModeling(self.tokenizer, mlm=False),
+            )
+            model.config.use_cache = False
+            trainer.train()
+
+            model.cpu().save_pretrained(tmp_dir)
+
+            assert "adapter_config.json" in os.listdir(tmp_dir)
+            assert SAFETENSORS_WEIGHTS_NAME in os.listdir(tmp_dir)
+
+            # assert loss is not None
+            assert trainer.state.log_history[-1]["train_loss"] is not None
+
+    @pytest.mark.multi_gpu_tests
+    @require_torch_multi_gpu
+    def test_causal_lm_training_multi_gpu(self):
+        r"""
+        Test the CausalLM training on a multi-GPU device. The test would simply fail if the adapters are not set
+        correctly.
+        """
+
+        with tempfile.TemporaryDirectory() as tmp_dir:
+            model = AutoModelForCausalLM.from_pretrained(
+                self.causal_lm_model_id,
+                device_map="auto",
+            )
+
+            assert set(model.hf_device_map.values()) == set(range(torch.cuda.device_count()))
+
+            model = prepare_model_for_kbit_training(model)
+
+            setattr(model, "model_parallel", True)
+            setattr(model, "is_parallelizable", True)
+
+            config = LoraConfig(
+                r=16,
+                lora_alpha=32,
+                target_modules=["q_proj", "v_proj"],
+                lora_dropout=0.05,
+                bias="none",
+                task_type="CAUSAL_LM",
+            )
+
+            model = get_peft_model(model, config)
+
+            data = load_dataset("Abirate/english_quotes")
+            data = data.map(lambda samples: self.tokenizer(samples["quote"]), batched=True)
+
+            trainer = Trainer(
+                model=model,
+                train_dataset=data["train"],
+                args=TrainingArguments(
+                    per_device_train_batch_size=4,
+                    gradient_accumulation_steps=4,
+                    warmup_steps=2,
+                    max_steps=3,
+                    learning_rate=2e-4,
+                    logging_steps=1,
+                    output_dir=tmp_dir,
+                ),
+                data_collator=DataCollatorForLanguageModeling(self.tokenizer, mlm=False),
+            )
+            model.config.use_cache = False
+            trainer.train()
+
+            model.cpu().save_pretrained(tmp_dir)
+
+            assert "adapter_config.json" in os.listdir(tmp_dir)
+            assert SAFETENSORS_WEIGHTS_NAME in os.listdir(tmp_dir)
+
+            # assert loss is not None
+            assert trainer.state.log_history[-1]["train_loss"] is not None
+
+
+PRECISIONS = [(torch.float32), (torch.float16), (torch.bfloat16)]
+
+LORA_PARAMS = {
+    "r": 8,
+    "lora_alpha": 16,
+    "lora_dropout": 0.05,
+}
+
+
+class SimpleModel(torch.nn.Module):
+    def __init__(self):
+        super().__init__()
+
+        self.embedding_layer = torch.nn.Embedding(1000, 768)
+        self.layer_norm = torch.nn.LayerNorm(768)
+        self.linear_transform = torch.nn.Linear(768, 256)
+
+    def forward(self, input_ids):
+        embedded_output = self.embedding_layer(input_ids)
+        norm_output = self.layer_norm(embedded_output)
+        linear_output = self.linear_transform(norm_output)
+
+        return linear_output
+
+
+class SimpleConv2DModel(torch.nn.Module):
+    def __init__(self):
+        super().__init__()
+
+        self.embedding_layer = torch.nn.Embedding(1000, 768)
+        self.layer_norm = torch.nn.LayerNorm(768)
+        self.conv2d_transform = torch.nn.Conv2d(1, 256, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1))
+
+    def forward(self, input_ids):
+        # Additional layers for your custom model
+        embedded_output = self.embedding_layer(input_ids)
+        norm_output = self.layer_norm(embedded_output)
+
+        # Reshape for Conv2d input (add batch size dimension)
+        norm_output = norm_output.unsqueeze(1)
+        conv_output = self.conv2d_transform(norm_output)
+
+        # Remove batch size dimension
+        conv_output = conv_output.squeeze(1)
+
+        return conv_output
+
+
+@require_torch_gpu
+class TestAutoCast(unittest.TestCase):
+    # This test makes sure, that Lora dtypes are consistent with the types
+    # infered by torch.autocast under tested PRECISIONS
+    @parameterized.expand(PRECISIONS)
+    def test_simple_model(self, *args, **kwargs):
+        self._test_model(SimpleModel(), *args, **kwargs)
+
+    @parameterized.expand(PRECISIONS)
+    def test_simple_lora_linear_model(self, *args, **kwargs):
+        simple_model = SimpleModel()
+        config = LoraConfig(
+            **LORA_PARAMS,
+            target_modules=["linear_transform"],
+        )
+
+        lora_model = get_peft_model(simple_model, config)
+
+        self._test_model(lora_model, *args, **kwargs)
+
+    @parameterized.expand(PRECISIONS)
+    def test_simple_lora_embedding_model(self, *args, **kwargs):
+        simple_model = SimpleModel()
+        config = LoraConfig(
+            **LORA_PARAMS,
+            target_modules=["embedding_layer"],
+        )
+        lora_model = get_peft_model(simple_model, config)
+
+        self._test_model(lora_model, *args, **kwargs)
+
+    @parameterized.expand(PRECISIONS)
+    def test_simple_conv2d_model(self, *args, **kwargs):
+        self._test_model(SimpleConv2DModel(), *args, **kwargs)
+
+    @parameterized.expand(PRECISIONS)
+    def test_simple_lora_conv2d_model(self, *args, **kwargs):
+        simple_model = SimpleConv2DModel()
+        config = LoraConfig(
+            **LORA_PARAMS,
+            target_modules=["conv2d_transform"],
+        )
+        lora_model = get_peft_model(simple_model, config)
+        self._test_model(lora_model, *args, **kwargs)
+
+    def _test_model(self, model, precision):
+        # Move model to GPU
+        model = model.cuda()
+
+        # Prepare dummy inputs
+        input_ids = torch.randint(0, 1000, (2, 10)).cuda()
+        if precision == torch.bfloat16:
+            if not torch.cuda.is_bf16_supported():
+                self.skipTest("Bfloat16 not supported on this device")
+
+        # Forward pass with test precision
+        with torch.autocast(enabled=True, dtype=precision, device_type="cuda"):
+            outputs = model(input_ids)
+            assert outputs.dtype == precision
```

### Comparing `peft-0.8.2/tests/test_hub_features.py` & `peft-0.9.0/tests/test_hub_features.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# coding=utf-8
 # Copyright 2023-present the HuggingFace Inc. team.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
@@ -31,8 +30,8 @@
             config = PeftConfig.from_pretrained(model_id, subfolder=subfolder)
 
             model = AutoModelForCausalLM.from_pretrained(
                 config.base_model_name_or_path,
             )
             model = PeftModel.from_pretrained(model, model_id, subfolder=subfolder)
 
-            self.assertTrue(isinstance(model, PeftModel))
+            assert isinstance(model, PeftModel)
```

### Comparing `peft-0.8.2/tests/test_low_level_api.py` & `peft-0.9.0/tests/test_low_level_api.py`

 * *Files 17% similar despite different names*

```diff
@@ -52,22 +52,22 @@
 
     def test_inject_adapter_in_model(self):
         dummy_inputs = torch.LongTensor([[0, 1, 2, 3, 4, 5, 6, 7]])
         _ = self.model(dummy_inputs)
 
         for name, module in self.model.named_modules():
             if name == "linear":
-                self.assertTrue(hasattr(module, "lora_A"))
-                self.assertTrue(hasattr(module, "lora_B"))
+                assert hasattr(module, "lora_A")
+                assert hasattr(module, "lora_B")
 
     def test_get_peft_model_state_dict(self):
         peft_state_dict = get_peft_model_state_dict(self.model)
 
         for key in peft_state_dict.keys():
-            self.assertTrue("lora" in key)
+            assert "lora" in key
 
     def test_modules_to_save(self):
         self.model = DummyModel()
 
         lora_config = LoraConfig(
             lora_alpha=16,
             lora_dropout=0.1,
@@ -77,17 +77,17 @@
             modules_to_save=["embedding"],
         )
 
         self.model = inject_adapter_in_model(lora_config, self.model)
 
         for name, module in self.model.named_modules():
             if name == "linear":
-                self.assertTrue(hasattr(module, "lora_A"))
-                self.assertTrue(hasattr(module, "lora_B"))
+                assert hasattr(module, "lora_A")
+                assert hasattr(module, "lora_B")
             elif name == "embedding":
-                self.assertTrue(isinstance(module, ModulesToSaveWrapper))
+                assert isinstance(module, ModulesToSaveWrapper)
 
         state_dict = get_peft_model_state_dict(self.model)
 
-        self.assertTrue("embedding.weight" in state_dict.keys())
+        assert "embedding.weight" in state_dict.keys()
 
-        self.assertTrue(hasattr(self.model.embedding, "weight"))
+        assert hasattr(self.model.embedding, "weight")
```

### Comparing `peft-0.8.2/tests/test_multitask_prompt_tuning.py` & `peft-0.9.0/tests/test_multitask_prompt_tuning.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# coding=utf-8
 # Copyright 2023-present the HuggingFace Inc. team.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
@@ -14,21 +13,23 @@
 # limitations under the License.
 
 import importlib
 import os
 import tempfile
 from unittest import TestCase
 
+import pytest
 import torch
+from parameterized import parameterized
 from torch.testing import assert_close
 
 from peft.mapping import get_peft_model
 from peft.peft_model import PeftModel
-from peft.tuners.multitask_prompt_tuning import MultitaskPromptTuningConfig
-from peft.utils.other import prepare_model_for_int8_training
+from peft.tuners.multitask_prompt_tuning import MultitaskPromptTuningConfig, MultitaskPromptTuningInit
+from peft.utils.other import WEIGHTS_NAME, prepare_model_for_int8_training
 from peft.utils.save_and_load import get_peft_model_state_dict
 from tests.testing_common import PeftCommonTester
 
 
 def is_llama_available() -> bool:
     """Check if Llama is available in the transformers library (it's not in earlier versions)."""
     try:
@@ -70,34 +71,36 @@
 
     @classmethod
     def _create_multitask_prompt_tuning_config(cls) -> MultitaskPromptTuningConfig:
         return MultitaskPromptTuningConfig(
             task_type="CAUSAL_LM",
             num_virtual_tokens=50,
             num_tasks=3,
-            prompt_tuning_init_text="classify the following into either positive or negative, or entailment, neutral or contradiction:",
+            prompt_tuning_init_text=(
+                "classify the following into either positive or negative, or entailment, neutral or contradiction:"
+            ),
         )
 
     def test_prepare_for_training(self) -> None:
         model = LlamaForCausalLM(self._create_test_llama_config())
         model = get_peft_model(model, self._create_multitask_prompt_tuning_config())
         model = model.to(self.torch_device)
 
         dummy_input = torch.LongTensor([[1, 1, 1]]).to(self.torch_device)
         dummy_output = model.get_input_embeddings()(dummy_input)
 
-        self.assertTrue(not dummy_output.requires_grad)
+        assert not dummy_output.requires_grad
 
     def test_prepare_for_int8_training(self) -> None:
         model = LlamaForCausalLM(self._create_test_llama_config())
         model = prepare_model_for_int8_training(model)
         model = model.to(self.torch_device)
 
         for param in model.parameters():
-            self.assertTrue(not param.requires_grad)
+            assert not param.requires_grad
 
         model = get_peft_model(model, self._create_multitask_prompt_tuning_config())
 
         # For backward compatibility
         if hasattr(model, "enable_input_require_grads"):
             model.enable_input_require_grads()
         else:
@@ -106,15 +109,15 @@
                 output.requires_grad_(True)
 
             model.get_input_embeddings().register_forward_hook(make_inputs_require_grad)
 
         dummy_input = torch.LongTensor([[1, 1, 1]]).to(self.torch_device)
         dummy_output = model.get_input_embeddings()(dummy_input)
 
-        self.assertTrue(dummy_output.requires_grad)
+        assert dummy_output.requires_grad
 
     def test_save_pretrained(self) -> None:
         seed = 420
         torch.manual_seed(seed)
         model = LlamaForCausalLM(self._create_test_llama_config())
         model = get_peft_model(model, self._create_multitask_prompt_tuning_config())
         model = model.to(self.torch_device)
@@ -128,38 +131,36 @@
 
             # check if the state dicts are equal
             state_dict = get_peft_model_state_dict(model)
 
             state_dict_from_pretrained = get_peft_model_state_dict(model_from_pretrained)
 
             # check if same keys
-            self.assertEqual(state_dict.keys(), state_dict_from_pretrained.keys())
+            assert state_dict.keys() == state_dict_from_pretrained.keys()
 
             # Check that the number of saved parameters is 4 -- 2 layers of (tokens and gate).
-            self.assertEqual(len(list(state_dict.keys())), 3)
+            assert len(state_dict) == 3
 
             # check if tensors equal
             for key in state_dict.keys():
-                self.assertTrue(
-                    torch.allclose(
-                        state_dict[key].to(self.torch_device), state_dict_from_pretrained[key].to(self.torch_device)
-                    )
+                assert torch.allclose(
+                    state_dict[key].to(self.torch_device), state_dict_from_pretrained[key].to(self.torch_device)
                 )
 
             # check if `adapter_model.safetensors` is present
-            self.assertTrue(os.path.exists(os.path.join(tmp_dirname, "adapter_model.safetensors")))
+            assert os.path.exists(os.path.join(tmp_dirname, "adapter_model.safetensors"))
 
             # check if `adapter_config.json` is present
-            self.assertTrue(os.path.exists(os.path.join(tmp_dirname, "adapter_config.json")))
+            assert os.path.exists(os.path.join(tmp_dirname, "adapter_config.json"))
 
             # check if `pytorch_model.bin` is not present
-            self.assertFalse(os.path.exists(os.path.join(tmp_dirname, "pytorch_model.bin")))
+            assert not os.path.exists(os.path.join(tmp_dirname, "pytorch_model.bin"))
 
             # check if `config.json` is not present
-            self.assertFalse(os.path.exists(os.path.join(tmp_dirname, "config.json")))
+            assert not os.path.exists(os.path.join(tmp_dirname, "config.json"))
 
     def test_save_pretrained_regression(self) -> None:
         seed = 420
         torch.manual_seed(seed)
         model = LlamaForCausalLM(self._create_test_llama_config())
         model = get_peft_model(model, self._create_multitask_prompt_tuning_config())
         model = model.to(self.torch_device)
@@ -173,38 +174,36 @@
 
             # check if the state dicts are equal
             state_dict = get_peft_model_state_dict(model)
 
             state_dict_from_pretrained = get_peft_model_state_dict(model_from_pretrained)
 
             # check if same keys
-            self.assertEqual(state_dict.keys(), state_dict_from_pretrained.keys())
+            assert state_dict.keys() == state_dict_from_pretrained.keys()
 
             # Check that the number of saved parameters is 4 -- 2 layers of (tokens and gate).
-            self.assertEqual(len(list(state_dict.keys())), 3)
+            assert len(state_dict) == 3
 
             # check if tensors equal
             for key in state_dict.keys():
-                self.assertTrue(
-                    torch.allclose(
-                        state_dict[key].to(self.torch_device), state_dict_from_pretrained[key].to(self.torch_device)
-                    )
+                assert torch.allclose(
+                    state_dict[key].to(self.torch_device), state_dict_from_pretrained[key].to(self.torch_device)
                 )
 
             # check if `adapter_model.bin` is present for regression
-            self.assertTrue(os.path.exists(os.path.join(tmp_dirname, "adapter_model.bin")))
+            assert os.path.exists(os.path.join(tmp_dirname, "adapter_model.bin"))
 
             # check if `adapter_config.json` is present
-            self.assertTrue(os.path.exists(os.path.join(tmp_dirname, "adapter_config.json")))
+            assert os.path.exists(os.path.join(tmp_dirname, "adapter_config.json"))
 
             # check if `pytorch_model.bin` is not present
-            self.assertFalse(os.path.exists(os.path.join(tmp_dirname, "pytorch_model.bin")))
+            assert not os.path.exists(os.path.join(tmp_dirname, "pytorch_model.bin"))
 
             # check if `config.json` is not present
-            self.assertFalse(os.path.exists(os.path.join(tmp_dirname, "config.json")))
+            assert not os.path.exists(os.path.join(tmp_dirname, "config.json"))
 
     def test_generate(self) -> None:
         model = LlamaForCausalLM(self._create_test_llama_config())
         model = get_peft_model(model, self._create_multitask_prompt_tuning_config())
         model = model.to(self.torch_device)
 
         input_ids = torch.LongTensor([[1, 1, 1], [2, 1, 2]]).to(self.torch_device)
@@ -241,7 +240,65 @@
 
         original = LlamaForCausalLM.from_pretrained(
             "trl-internal-testing/tiny-random-LlamaForCausalLM", torch_dtype=torch.bfloat16
         )
         mpt = get_peft_model(original, self._create_multitask_prompt_tuning_config())
         mpt = mpt.to(self.torch_device)
         _ = mpt.generate(input_ids=input_ids, task_ids=task_ids)
+
+    def test_generate_text_with_random_init(self) -> None:
+        model = LlamaForCausalLM(self._create_test_llama_config())
+
+        config = self._create_multitask_prompt_tuning_config()
+        config.prompt_tuning_init = MultitaskPromptTuningInit.RANDOM
+
+        model = get_peft_model(model, config)
+        model = model.to(self.torch_device)
+
+        input_ids = torch.LongTensor([[1, 1, 1], [2, 1, 2]]).to(self.torch_device)
+        attention_mask = torch.LongTensor([[1, 1, 1], [1, 0, 1]]).to(self.torch_device)
+        task_ids = torch.LongTensor([0]).to(self.torch_device)
+
+        # check if `generate` works
+        _ = model.generate(input_ids=input_ids, attention_mask=attention_mask, task_ids=task_ids)
+
+        with pytest.raises(ValueError):
+            # check if `generate` raises an error if task_ids are not passed
+            _ = model.generate(input_ids, attention_mask=attention_mask)
+
+    @parameterized.expand(
+        [
+            MultitaskPromptTuningInit.AVERAGE_SOURCE_TASKS,
+            MultitaskPromptTuningInit.EXACT_SOURCE_TASK,
+            MultitaskPromptTuningInit.ONLY_SOURCE_SHARED,
+        ],
+    )
+    def test_generate_text_with_other_init(self, prompt_tuning_init) -> None:
+        with tempfile.TemporaryDirectory() as tmp_dirname:
+            model = LlamaForCausalLM(self._create_test_llama_config())
+            model = get_peft_model(model, self._create_multitask_prompt_tuning_config())
+            model.save_pretrained(tmp_dirname, safe_serialization=False)  # bc torch.load is used
+
+            config = MultitaskPromptTuningConfig(
+                task_type="CAUSAL_LM",
+                num_virtual_tokens=50,
+                num_tasks=1,
+                prompt_tuning_init_text=(
+                    "classify the following into either positive or negative, or entailment, neutral or contradiction:"
+                ),
+                prompt_tuning_init=prompt_tuning_init,
+                prompt_tuning_init_state_dict_path=os.path.join(tmp_dirname, WEIGHTS_NAME),
+            )
+            model = LlamaForCausalLM(self._create_test_llama_config())
+            model = get_peft_model(model, config)
+            model = model.to(self.torch_device)
+
+            input_ids = torch.LongTensor([[1, 1, 1], [2, 1, 2]]).to(self.torch_device)
+            attention_mask = torch.LongTensor([[1, 1, 1], [1, 0, 1]]).to(self.torch_device)
+            task_ids = torch.LongTensor([0]).to(self.torch_device)
+
+            # check if `generate` works
+            _ = model.generate(input_ids=input_ids, attention_mask=attention_mask, task_ids=task_ids)
+
+            with pytest.raises(ValueError):
+                # check if `generate` raises an error if task_ids are not passed
+                _ = model.generate(input_ids, attention_mask=attention_mask)
```

### Comparing `peft-0.8.2/tests/test_stablediffusion.py` & `peft-0.9.0/tests/test_stablediffusion.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# coding=utf-8
 # Copyright 2023-present the HuggingFace Inc. team.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
@@ -85,14 +84,15 @@
 
 
 class StableDiffusionModelTester(TestCase, PeftCommonTester):
     r"""
     Tests that diffusers StableDiffusion model works with PEFT as expected.
 
     """
+
     transformers_class = StableDiffusionPipeline
 
     def instantiate_sd_peft(self, model_id, config_cls, config_kwargs):
         # Instantiate StableDiffusionPipeline
         model = self.transformers_class.from_pretrained(model_id)
 
         config_kwargs = config_kwargs.copy()
@@ -148,15 +148,15 @@
         model.unet = model.unet.merge_and_unload()
 
         # Generate output for peft merged StableDiffusion
         with temp_seed(seed=42):
             merged_output = np.array(model(**dummy_input).images[0]).astype(np.float32)
 
         # Images are in uint8 drange, so use large atol
-        self.assertTrue(np.allclose(peft_output, merged_output, atol=1.0))
+        assert np.allclose(peft_output, merged_output, atol=1.0)
 
     @parameterized.expand(
         PeftStableDiffusionTestConfigManager.get_grid_parameters(
             {
                 "model_ids": PEFT_DIFFUSERS_SD_MODELS_TO_TEST,
                 "lora_kwargs": {"init_lora_weights": [False]},
                 "loha_kwargs": {"init_weights": [False]},
@@ -180,15 +180,15 @@
         model.unet = model.unet.merge_and_unload(safe_merge=True)
 
         # Generate output for peft merged StableDiffusion
         with temp_seed(seed=42):
             merged_output = np.array(model(**dummy_input).images[0]).astype(np.float32)
 
         # Images are in uint8 drange, so use large atol
-        self.assertTrue(np.allclose(peft_output, merged_output, atol=1.0))
+        assert np.allclose(peft_output, merged_output, atol=1.0)
 
     @parameterized.expand(
         PeftStableDiffusionTestConfigManager.get_grid_parameters(
             {
                 "model_ids": PEFT_DIFFUSERS_SD_MODELS_TO_TEST,
                 "lora_kwargs": {"init_lora_weights": [False]},
             },
@@ -206,18 +206,16 @@
         unet_adapter_config = replace(model.unet.peft_config[unet_adapter_name])
 
         # Create weighted adapters
         model.text_encoder.add_weighted_adapter([unet_adapter_name], [0.5], "weighted_adapter_test")
         model.unet.add_weighted_adapter([unet_adapter_name], [0.5], "weighted_adapter_test")
 
         # Assert that base adapters config did not change
-        self.assertTrue(
-            asdict(text_encoder_adapter_config) == asdict(model.text_encoder.peft_config[text_encoder_adapter_name])
-        )
-        self.assertTrue(asdict(unet_adapter_config) == asdict(model.unet.peft_config[unet_adapter_name]))
+        assert asdict(text_encoder_adapter_config) == asdict(model.text_encoder.peft_config[text_encoder_adapter_name])
+        assert asdict(unet_adapter_config) == asdict(model.unet.peft_config[unet_adapter_name])
 
     @parameterized.expand(
         PeftStableDiffusionTestConfigManager.get_grid_parameters(
             {
                 "model_ids": PEFT_DIFFUSERS_SD_MODELS_TO_TEST,
                 "lora_kwargs": {"init_lora_weights": [False]},
                 "loha_kwargs": {"init_weights": [False]},
```

### Comparing `peft-0.8.2/tests/test_tuners_utils.py` & `peft-0.9.0/tests/test_tuners_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import unittest
 from copy import deepcopy
 
+import pytest
 from diffusers import StableDiffusionPipeline
 from parameterized import parameterized
 from torch import nn
 from transformers import AutoModel, AutoModelForCausalLM, AutoModelForSeq2SeqLM
 
 from peft import IA3Config, LoHaConfig, LoraConfig, get_peft_model
 from peft.tuners.tuners_utils import (
@@ -31,15 +32,15 @@
 from peft.utils import INCLUDE_LINEAR_LAYERS_SHORTHAND
 
 from .testing_utils import require_bitsandbytes, require_torch_gpu
 
 
 # Implements tests for regex matching logic common for all BaseTuner subclasses, and
 # tests for correct behaviour with different config kwargs for BaseTuners (Ex: feedforward for IA3, etc) and
-# tests for utlity function to include all linear layers
+# tests for utility function to include all linear layers
 
 REGEX_TEST_CASES = [
     # tuple of
     # 1. key
     # 2. target_modules
     # 3. layers_to_transform
     # 4. layers_pattern
@@ -171,15 +172,15 @@
         config = LoraConfig(
             base_model_name_or_path=model_id,
             target_modules=target_modules,
             layers_pattern=layers_pattern,
             layers_to_transform=layers_to_transform,
         )
         actual_result = bool(check_target_module_exists(config, key))
-        self.assertEqual(actual_result, expected_result)
+        assert actual_result == expected_result
 
     def test_module_matching_lora(self):
         # peft models that have a module matching method to inspect the matching modules to allow
         # users to easily debug their configuration. Here we only test a single case, not all possible combinations of
         # configs that could exist. This is okay as the method calls `check_target_module_exists` internally, which
         # has been extensively tested above.
         model_id = "hf-internal-testing/tiny-random-BloomForCausalLM"
@@ -193,20 +194,20 @@
         expected = [
             "h.0.self_attention.query_key_value",
             "h.1.self_attention.query_key_value",
             "h.2.self_attention.query_key_value",
             "h.3.self_attention.query_key_value",
             "h.4.self_attention.query_key_value",
         ]
-        self.assertEqual(matched, expected)  # module lists should match exactly
+        assert matched == expected  # module lists should match exactly
 
         # no overlap with matched modules
         unmatched = output["unmatched"]
         for key in expected:
-            self.assertFalse(key in unmatched)
+            assert key not in unmatched
 
     def test_feedforward_matching_ia3(self):
         model_id = "hf-internal-testing/tiny-random-T5ForConditionalGeneration"
         model = AutoModelForSeq2SeqLM.from_pretrained(model_id)
         # simple example for just one t5 block for testing
         config_kwargs = {
             "target_modules": ".*encoder.*block.0.*(SelfAttention|EncDecAttention|DenseReluDense).(k|q|v|wo|wi)$",
@@ -223,22 +224,22 @@
             "encoder.block.0.layer.1.DenseReluDense.wi",
             "encoder.block.0.layer.1.DenseReluDense.wo",
         ]
         expected_feedforward = [
             "encoder.block.0.layer.1.DenseReluDense.wi",
             "encoder.block.0.layer.1.DenseReluDense.wo",
         ]
-        self.assertEqual(matched, expected)  # not required since we do similar checks above, but just to be sure
+        assert matched == expected  # not required since we do similar checks above, but just to be sure
         module_dict = dict(model.named_modules())
         for key in matched:
             module = module_dict[key]
             if key in expected_feedforward:
-                self.assertTrue(module.is_feedforward)
+                assert module.is_feedforward
             else:  # other IA3 modules should not be marked as feedforward
-                self.assertFalse(module.is_feedforward)
+                assert not module.is_feedforward
 
     @parameterized.expand(MAYBE_INCLUDE_ALL_LINEAR_LAYERS_TEST_CASES)
     def test_maybe_include_all_linear_layers_lora(
         self, model_id, model_type, initial_target_modules, expected_target_modules
     ):
         model = self.transformers_class_map[model_type].from_pretrained(model_id)
         config_cls = LoraConfig
@@ -273,15 +274,15 @@
         model_copy = deepcopy(model)
         actual_model = get_peft_model(model, peft_config=actual_config)
         expected_model = get_peft_model(model_copy, peft_config=expected_config)
         expected_model_module_dict = dict(expected_model.named_modules())
         # compare the two models and assert that all layers are of the same type
         for name, actual_module in actual_model.named_modules():
             expected_module = expected_model_module_dict[name]
-            self.assertEqual(type(actual_module), type(expected_module))
+            assert type(actual_module) == type(expected_module)
 
     def test_maybe_include_all_linear_layers_ia3_loha(self):
         model_id, initial_target_modules, expected_target_modules = (
             "HuggingFaceH4/tiny-random-LlamaForCausalLM",
             INCLUDE_LINEAR_LAYERS_SHORTHAND,
             ["k_proj", "v_proj", "q_proj", "o_proj", "down_proj", "up_proj", "gate_proj"],
         )
@@ -298,25 +299,25 @@
     def test_maybe_include_all_linear_layers_internals(self, initial_target_modules, expected_target_modules):
         model_id = "HuggingFaceH4/tiny-random-LlamaForCausalLM"
         model = AutoModelForCausalLM.from_pretrained(model_id)
         config = LoraConfig(base_model_name_or_path=model_id, target_modules=initial_target_modules)
         new_config = _maybe_include_all_linear_layers(config, model)
         if isinstance(expected_target_modules, list):
             # assert that expected and actual target_modules have the same items
-            self.assertCountEqual(new_config.target_modules, expected_target_modules)
+            assert set(new_config.target_modules) == set(expected_target_modules)
         else:
-            self.assertEqual(new_config.target_modules, expected_target_modules)
+            assert new_config.target_modules == expected_target_modules
 
     def test_maybe_include_all_linear_layers_diffusion(self):
         model_id = "hf-internal-testing/tiny-stable-diffusion-torch"
         model = StableDiffusionPipeline.from_pretrained(model_id)
         config = LoraConfig(base_model_name_or_path=model_id, target_modules="all-linear")
-        with self.assertRaisesRegex(
+        with pytest.raises(
             ValueError,
-            "Only instances of PreTrainedModel support `target_modules='all-linear'`",
+            match="Only instances of PreTrainedModel support `target_modules='all-linear'`",
         ):
             model.unet = get_peft_model(model.unet, config)
 
 
 class MLP(nn.Module):
     def __init__(self, bias=True):
         super().__init__()
@@ -332,42 +333,42 @@
 
     This checks LoRA and IA³, but this should be sufficient, testing all other tuners is not necessary.
     """
 
     def test_one_targeted_module_regex(self):
         model = MLP()
         model = get_peft_model(model, LoraConfig(target_modules="lin0"))
-        self.assertEqual(model.targeted_module_names, ["lin0"])
+        assert model.targeted_module_names == ["lin0"]
 
     def test_two_targeted_module_regex(self):
         model = MLP()
         model = get_peft_model(model, LoraConfig(target_modules="lin.*"))
-        self.assertEqual(model.targeted_module_names, ["lin0", "lin1"])
+        assert model.targeted_module_names == ["lin0", "lin1"]
 
     def test_one_targeted_module_list(self):
         model = MLP()
         model = get_peft_model(model, LoraConfig(target_modules=["lin0"]))
-        self.assertEqual(model.targeted_module_names, ["lin0"])
+        assert model.targeted_module_names == ["lin0"]
 
     def test_two_targeted_module_list(self):
         model = MLP()
         model = get_peft_model(model, LoraConfig(target_modules=["lin0", "lin1"]))
-        self.assertEqual(model.targeted_module_names, ["lin0", "lin1"])
+        assert model.targeted_module_names == ["lin0", "lin1"]
 
     def test_ia3_targeted_module_regex(self):
         model = MLP()
         model = get_peft_model(model, IA3Config(target_modules=".*lin.*", feedforward_modules=".*lin.*"))
-        self.assertEqual(model.targeted_module_names, ["lin0", "lin1"])
+        assert model.targeted_module_names == ["lin0", "lin1"]
 
     def test_ia3_targeted_module_list(self):
         model = MLP()
         model = get_peft_model(model, IA3Config(target_modules=["lin0", "lin1"], feedforward_modules=["lin0", "lin1"]))
-        self.assertEqual(model.targeted_module_names, ["lin0", "lin1"])
+        assert model.targeted_module_names == ["lin0", "lin1"]
 
     def test_realistic_example(self):
         model = AutoModelForCausalLM.from_pretrained("hf-internal-testing/tiny-random-BloomForCausalLM")
         config = LoraConfig(task_type="CAUSAL_LM")
         model = get_peft_model(model, config)
         expected = [
             f"transformer.h.{i}.self_attention.query_key_value" for i in range(len(model.base_model.transformer.h))
         ]
-        self.assertEqual(model.targeted_module_names, expected)
+        assert model.targeted_module_names == expected
```

### Comparing `peft-0.8.2/tests/testing_common.py` & `peft-0.9.0/tests/testing_common.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# coding=utf-8
 # Copyright 2023-present the HuggingFace Inc. team.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
@@ -17,21 +16,24 @@
 import os
 import pickle
 import re
 import tempfile
 from collections import OrderedDict
 from dataclasses import replace
 
+import pytest
 import torch
 import yaml
 from diffusers import StableDiffusionPipeline
 
 from peft import (
     AdaLoraConfig,
     IA3Config,
+    LoHaConfig,
+    LoKrConfig,
     LoraConfig,
     PeftModel,
     PeftType,
     PrefixTuningConfig,
     PromptEncoderConfig,
     PromptLearningConfig,
     PromptTuningConfig,
@@ -120,15 +122,15 @@
         """
         generated_tests = []
         model_list = grid_parameters["model_ids"]
         task_type = grid_parameters["task_type"] if "task_type" in grid_parameters else None
 
         for model_id in model_list:
             for key, value in self.items():
-                if "{}_kwargs".format(key) in grid_parameters:
+                if f"{key}_kwargs" in grid_parameters:
                     peft_configs = []
                     current_peft_config = value[1].copy()
                     for current_key, current_value in grid_parameters[f"{key}_kwargs"].items():
                         for kwarg in current_value:
                             current_peft_config.update({current_key: kwarg})
 
                             if task_type is not None:
@@ -169,82 +171,82 @@
 
     def prepare_inputs_for_common(self):
         raise NotImplementedError
 
     def check_modelcard(self, tmp_dirname, model):
         # check the generated README.md
         filename = os.path.join(tmp_dirname, "README.md")
-        self.assertTrue(os.path.exists(filename))
-        with open(filename, "r", encoding="utf-8") as f:
+        assert os.path.exists(filename)
+        with open(filename, encoding="utf-8") as f:
             readme = f.read()
         metainfo = re.search(r"---\n(.*?)\n---", readme, re.DOTALL).group(1)
         dct = yaml.safe_load(metainfo)
-        self.assertEqual(dct["library_name"], "peft")
+        assert dct["library_name"] == "peft"
 
         if hasattr(model, "config"):
-            self.assertEqual(dct["base_model"], model.config.to_dict()["_name_or_path"])
+            assert dct["base_model"] == model.config.to_dict()["_name_or_path"]
         else:  # a custom model
-            self.assertTrue("base_model" not in dct)
+            assert "base_model" not in dct
 
     def check_config_json(self, tmp_dirname, model):
         # check the generated config.json
         filename = os.path.join(tmp_dirname, "adapter_config.json")
-        self.assertTrue(os.path.exists(filename))
-        with open(filename, "r", encoding="utf-8") as f:
+        assert os.path.exists(filename)
+        with open(filename, encoding="utf-8") as f:
             config = json.load(f)
 
         if hasattr(model, "config"):  # custom models don't have a config attribute
-            self.assertEqual(config["base_model_name_or_path"], model.config.to_dict()["_name_or_path"])
+            assert config["base_model_name_or_path"] == model.config.to_dict()["_name_or_path"]
 
     def _test_model_attr(self, model_id, config_cls, config_kwargs):
         model = self.transformers_class.from_pretrained(model_id)
         config = config_cls(
             base_model_name_or_path=model_id,
             **config_kwargs,
         )
         model = get_peft_model(model, config)
 
-        self.assertTrue(hasattr(model, "save_pretrained"))
-        self.assertTrue(hasattr(model, "from_pretrained"))
-        self.assertTrue(hasattr(model, "push_to_hub"))
+        assert hasattr(model, "save_pretrained")
+        assert hasattr(model, "from_pretrained")
+        assert hasattr(model, "push_to_hub")
 
     def _test_adapter_name(self, model_id, config_cls, config_kwargs):
         model = self.transformers_class.from_pretrained(model_id)
         config = config_cls(
             base_model_name_or_path=model_id,
             **config_kwargs,
         )
         model = get_peft_model(model, config, adapter_name="test-adapter")
         correctly_converted = False
         for n, _ in model.named_parameters():
             if "test-adapter" in n:
                 correctly_converted = True
                 break
 
-        self.assertTrue(correctly_converted)
+        assert correctly_converted
 
     def _test_prepare_for_training(self, model_id, config_cls, config_kwargs):
         model = self.transformers_class.from_pretrained(model_id).to(self.torch_device)
         config = config_cls(
             base_model_name_or_path=model_id,
             **config_kwargs,
         )
         model = get_peft_model(model, config)
 
         dummy_input = self.prepare_inputs_for_testing()
         dummy_output = model.get_input_embeddings()(dummy_input["input_ids"])
 
-        self.assertFalse(dummy_output.requires_grad)
+        assert not dummy_output.requires_grad
 
         # load with `prepare_model_for_int8_training`
         model = self.transformers_class.from_pretrained(model_id).to(self.torch_device)
         model = prepare_model_for_int8_training(model)
 
         for param in model.parameters():
-            self.assertFalse(param.requires_grad)
+            assert not param.requires_grad
 
         config = config_cls(
             base_model_name_or_path=model_id,
             **config_kwargs,
         )
         model = get_peft_model(model, config)
 
@@ -257,15 +259,15 @@
                 output.requires_grad_(True)
 
             model.get_input_embeddings().register_forward_hook(make_inputs_require_grad)
 
         dummy_input = self.prepare_inputs_for_testing()
         dummy_output = model.get_input_embeddings()(dummy_input["input_ids"])
 
-        self.assertTrue(dummy_output.requires_grad)
+        assert dummy_output.requires_grad
 
     def _test_save_pretrained(self, model_id, config_cls, config_kwargs, safe_serialization=True):
         # ensure that the weights are randomly initialized
         if issubclass(config_cls, LoraConfig):
             config_kwargs = config_kwargs.copy()
             config_kwargs["init_lora_weights"] = False
         if issubclass(config_cls, IA3Config):
@@ -298,41 +300,39 @@
                 state_dict_from_pretrained = get_peft_model_state_dict(model_from_pretrained, unwrap_compiled=True)
             else:
                 state_dict = get_state_dict(model, unwrap_compiled=True)
                 state_dict_from_pretrained = get_state_dict(model_from_pretrained, unwrap_compiled=True)
 
             # check if tensors equal
             for key in state_dict.keys():
-                self.assertTrue(
-                    torch.allclose(
-                        state_dict[key].to(self.torch_device), state_dict_from_pretrained[key].to(self.torch_device)
-                    )
+                assert torch.allclose(
+                    state_dict[key].to(self.torch_device), state_dict_from_pretrained[key].to(self.torch_device)
                 )
 
             target_adapter_filename = "adapter_model.safetensors" if safe_serialization else "adapter_model.bin"
 
             # check if `adapter_model.safetensors` is present
-            self.assertTrue(os.path.exists(os.path.join(tmp_dirname, target_adapter_filename)))
+            assert os.path.exists(os.path.join(tmp_dirname, target_adapter_filename))
 
             # check if `adapter_config.json` is present
-            self.assertTrue(os.path.exists(os.path.join(tmp_dirname, "adapter_config.json")))
+            assert os.path.exists(os.path.join(tmp_dirname, "adapter_config.json"))
 
             # check if `model.safetensors` is not present
-            self.assertFalse(os.path.exists(os.path.join(tmp_dirname, "model.safetensors")))
+            assert not os.path.exists(os.path.join(tmp_dirname, "model.safetensors"))
 
             # check if `config.json` is not present
-            self.assertFalse(os.path.exists(os.path.join(tmp_dirname, "config.json")))
+            assert not os.path.exists(os.path.join(tmp_dirname, "config.json"))
 
             self.check_modelcard(tmp_dirname, model)
             self.check_config_json(tmp_dirname, model)
 
     def _test_save_pretrained_selected_adapters(self, model_id, config_cls, config_kwargs, safe_serialization=True):
         if issubclass(config_cls, AdaLoraConfig):
             # AdaLora does not support adding more than 1 adapter
-            return
+            return pytest.skip(f"Test not applicable for {config_cls}")
 
         # ensure that the weights are randomly initialized
         if issubclass(config_cls, LoraConfig):
             config_kwargs = config_kwargs.copy()
             config_kwargs["init_lora_weights"] = False
         if issubclass(config_cls, IA3Config):
             config_kwargs = config_kwargs.copy()
@@ -373,53 +373,51 @@
                 state_dict = get_peft_model_state_dict(model, unwrap_compiled=True)
                 state_dict_from_pretrained = get_peft_model_state_dict(model_from_pretrained, unwrap_compiled=True)
             else:
                 state_dict = get_state_dict(model, unwrap_compiled=True)
                 state_dict_from_pretrained = get_state_dict(model_from_pretrained, unwrap_compiled=True)
 
             # check if same keys
-            self.assertEqual(state_dict.keys(), state_dict_from_pretrained.keys())
+            assert state_dict.keys() == state_dict_from_pretrained.keys()
 
             # check if tensors equal
             for key in state_dict.keys():
-                self.assertTrue(
-                    torch.allclose(
-                        state_dict[key].to(self.torch_device), state_dict_from_pretrained[key].to(self.torch_device)
-                    )
+                assert torch.allclose(
+                    state_dict[key].to(self.torch_device), state_dict_from_pretrained[key].to(self.torch_device)
                 )
 
             target_adapter_filename = "adapter_model.safetensors" if safe_serialization else "adapter_model.bin"
 
             # check if `adapter_model.safetensors` is present
-            self.assertTrue(os.path.exists(os.path.join(tmp_dirname, target_adapter_filename)))
-            self.assertTrue(os.path.exists(os.path.join(new_adapter_dir, target_adapter_filename)))
+            assert os.path.exists(os.path.join(tmp_dirname, target_adapter_filename))
+            assert os.path.exists(os.path.join(new_adapter_dir, target_adapter_filename))
 
             # check if `adapter_config.json` is present
-            self.assertTrue(os.path.exists(os.path.join(tmp_dirname, "adapter_config.json")))
-            self.assertTrue(os.path.exists(os.path.join(new_adapter_dir, "adapter_config.json")))
+            assert os.path.exists(os.path.join(tmp_dirname, "adapter_config.json"))
+            assert os.path.exists(os.path.join(new_adapter_dir, "adapter_config.json"))
 
             # check if `model.safetensors` is not present
-            self.assertFalse(os.path.exists(os.path.join(tmp_dirname, "model.safetensors")))
-            self.assertFalse(os.path.exists(os.path.join(new_adapter_dir, "model.safetensors")))
+            assert not os.path.exists(os.path.join(tmp_dirname, "model.safetensors"))
+            assert not os.path.exists(os.path.join(new_adapter_dir, "model.safetensors"))
 
             # check if `config.json` is not present
-            self.assertFalse(os.path.exists(os.path.join(tmp_dirname, "config.json")))
-            self.assertFalse(os.path.exists(os.path.join(new_adapter_dir, "config.json")))
+            assert not os.path.exists(os.path.join(tmp_dirname, "config.json"))
+            assert not os.path.exists(os.path.join(new_adapter_dir, "config.json"))
 
             self.check_modelcard(tmp_dirname, model)
             self.check_config_json(tmp_dirname, model)
 
         with tempfile.TemporaryDirectory() as tmp_dirname:
             model.save_pretrained(tmp_dirname, selected_adapters=["default"])
 
             model_from_pretrained = self.transformers_class.from_pretrained(model_id)
             model_from_pretrained = PeftModel.from_pretrained(model_from_pretrained, tmp_dirname)
 
-            self.assertTrue("default" in model_from_pretrained.peft_config.keys())
-            self.assertTrue("new_adapter" not in model_from_pretrained.peft_config.keys())
+            assert "default" in model_from_pretrained.peft_config.keys()
+            assert "new_adapter" not in model_from_pretrained.peft_config.keys()
 
     def _test_from_pretrained_config_construction(self, model_id, config_cls, config_kwargs):
         model = self.transformers_class.from_pretrained(model_id)
         config = config_cls(base_model_name_or_path=model_id, **config_kwargs)
         model = get_peft_model(model, config)
         model = model.to(self.torch_device)
 
@@ -427,21 +425,21 @@
             model.save_pretrained(tmp_dirname)
 
             model_from_pretrained = self.transformers_class.from_pretrained(model_id)
             model_from_pretrained = PeftModel.from_pretrained(
                 model_from_pretrained, tmp_dirname, is_trainable=False, config=config
             )
 
-            self.assertTrue(model_from_pretrained.peft_config["default"].inference_mode)
-            self.assertIs(model_from_pretrained.peft_config["default"], config)
+            assert model_from_pretrained.peft_config["default"].inference_mode
+            assert model_from_pretrained.peft_config["default"] is config
 
     def _test_merge_layers_fp16(self, model_id, config_cls, config_kwargs):
-        if config_cls not in (LoraConfig, IA3Config):
+        if config_cls not in (LoraConfig, IA3Config, AdaLoraConfig, LoHaConfig, LoKrConfig):
             # Merge layers only supported for LoRA and IA³
-            return
+            return pytest.skip(f"Test not applicable for {config_cls}")
 
         if ("gpt2" in model_id.lower()) and (config_cls != LoraConfig):
             self.skipTest("Merging GPT2 adapters not supported for IA³ (yet)")
 
         model = self.transformers_class.from_pretrained(model_id, torch_dtype=torch.float16)
         config = config_cls(
             base_model_name_or_path=model_id,
@@ -452,15 +450,15 @@
 
         model.eval()
 
         # This should simply work
         _ = model.merge_and_unload()
 
     def _test_merge_layers_nan(self, model_id, config_cls, config_kwargs):
-        if config_cls not in (LoraConfig, IA3Config, AdaLoraConfig):
+        if config_cls not in (LoraConfig, IA3Config, AdaLoraConfig, LoHaConfig, LoKrConfig):
             # Merge layers only supported for LoRA and IA³
             return
         if ("gpt2" in model_id.lower()) and (config_cls != LoraConfig):
             self.skipTest("Merging GPT2 adapters not supported for IA³ (yet)")
 
         model = self.transformers_class.from_pretrained(model_id)
         config = config_cls(
@@ -476,67 +474,57 @@
 
         # This should work
         logits_unmerged = model(**dummy_input)[0]
 
         model = model.merge_and_unload()
         logits_merged = model(**dummy_input)[0]
 
-        self.assertTrue(torch.allclose(logits_unmerged, logits_merged, atol=1e-3, rtol=1e-3))
+        assert torch.allclose(logits_unmerged, logits_merged, atol=1e-3, rtol=1e-3)
 
         model = self.transformers_class.from_pretrained(model_id)
         config = config_cls(
             base_model_name_or_path=model_id,
             **config_kwargs,
         )
         model = get_peft_model(model, config)
         model = model.to(self.torch_device)
 
         for name, module in model.named_parameters():
             if "lora_A" in name or "ia3" in name or "lora_E" in name or "lora_B" in name:
                 module.data[0] = torch.nan
 
-        with self.assertRaises(ValueError) as error_context:
+        with pytest.raises(
+            ValueError, match="NaNs detected in the merged weights. The adapter default seems to be broken"
+        ):
             model = model.merge_and_unload(safe_merge=True)
 
-        self.assertEqual(
-            str(error_context.exception),
-            "NaNs detected in the merged weights. The adapter default seems to be broken",
-        )
-
         for name, module in model.named_parameters():
             if "lora_A" in name or "ia3" in name or "lora_E" in name or "lora_B" in name:
                 module.data[0] = torch.inf
 
-        with self.assertRaises(ValueError) as error_context:
+        with pytest.raises(
+            ValueError, match="NaNs detected in the merged weights. The adapter default seems to be broken"
+        ):
             model = model.merge_and_unload(safe_merge=True)
 
-        self.assertEqual(
-            str(error_context.exception),
-            "NaNs detected in the merged weights. The adapter default seems to be broken",
-        )
-
     def _test_merge_layers(self, model_id, config_cls, config_kwargs):
-        if config_cls not in (LoraConfig, IA3Config):
-            # Merge layers only supported for LoRA and IA³
-            return
+        if issubclass(config_cls, PromptLearningConfig):
+            return pytest.skip(f"Test not applicable for {config_cls}")
+
         if ("gpt2" in model_id.lower()) and (config_cls != LoraConfig):
             self.skipTest("Merging GPT2 adapters not supported for IA³ (yet)")
 
         model = self.transformers_class.from_pretrained(model_id)
         config = config_cls(
             base_model_name_or_path=model_id,
             **config_kwargs,
         )
         model = get_peft_model(model, config)
         model = model.to(self.torch_device)
 
-        if config.peft_type not in ("IA3", "LORA"):
-            with self.assertRaises(AttributeError):
-                model = model.merge_and_unload()
-
         dummy_input = self.prepare_inputs_for_testing()
         model.eval()
         logits = model(**dummy_input)[0]
 
         model.merge_adapter()
         logits_merged = model(**dummy_input)[0]
         model.unmerge_adapter()
@@ -545,36 +533,36 @@
         model = model.merge_and_unload()
         logits_merged_unloaded = model(**dummy_input)[0]
 
         atol, rtol = 1e-4, 1e-4
         if (config.peft_type == "IA3") and (model_id == "Conv2d"):
             # for some reason, the IA³ Conv2d introduces a larger error
             atol, rtol = 0.3, 0.01
-        self.assertTrue(torch.allclose(logits, logits_merged, atol=atol, rtol=rtol))
-        self.assertTrue(torch.allclose(logits, logits_unmerged, atol=atol, rtol=rtol))
-        self.assertTrue(torch.allclose(logits, logits_merged_unloaded, atol=atol, rtol=rtol))
+        assert torch.allclose(logits, logits_merged, atol=atol, rtol=rtol)
+        assert torch.allclose(logits, logits_unmerged, atol=atol, rtol=rtol)
+        assert torch.allclose(logits, logits_merged_unloaded, atol=atol, rtol=rtol)
 
         # For this test to work, weights should not be initialized to identity transform (e.g.
         # init_lora_weights should be False).
         transformers_model = self.transformers_class.from_pretrained(model_id).to(self.torch_device)
         logits_transformers = transformers_model(**dummy_input)[0]
-        self.assertFalse(torch.allclose(logits_merged, logits_transformers, atol=1e-10, rtol=1e-10))
+        assert not torch.allclose(logits_merged, logits_transformers, atol=1e-10, rtol=1e-10)
 
         # test that the logits are identical after a save-load-roundtrip
         if hasattr(model, "save_pretrained"):
             # model is a transformers model
             with tempfile.TemporaryDirectory() as tmp_dirname:
                 model.save_pretrained(tmp_dirname)
                 model_from_pretrained = self.transformers_class.from_pretrained(tmp_dirname).to(self.torch_device)
         else:
             # model is not a transformers model
             model_from_pretrained = pickle.loads(pickle.dumps(model))
 
         logits_merged_from_pretrained = model_from_pretrained(**dummy_input)[0]
-        self.assertTrue(torch.allclose(logits_merged, logits_merged_from_pretrained, atol=atol, rtol=rtol))
+        assert torch.allclose(logits_merged, logits_merged_from_pretrained, atol=atol, rtol=rtol)
 
     def _test_merge_layers_multi(self, model_id, config_cls, config_kwargs):
         supported_peft_types = [PeftType.LORA, PeftType.LOHA, PeftType.LOKR, PeftType.IA3, PeftType.OFT]
 
         if ("gpt2" in model_id.lower()) and (config_cls == IA3Config):
             self.skipTest("Merging GPT2 adapters not supported for IA³ (yet)")
 
@@ -600,46 +588,46 @@
         model.add_adapter("adapter-2", config)
         model.set_adapter("adapter-2")
         model.eval()
 
         with torch.inference_mode():
             logits_adapter_2 = model(**dummy_input)[0]
 
-        self.assertFalse(torch.allclose(logits_adapter_1, logits_adapter_2, atol=1e-3, rtol=1e-3))
+        assert not torch.allclose(logits_adapter_1, logits_adapter_2, atol=1e-3, rtol=1e-3)
 
         model.set_adapter("default")
 
         with torch.inference_mode():
             logits_adapter_1_after_set = model(**dummy_input)[0]
 
-        self.assertTrue(torch.allclose(logits_adapter_1_after_set, logits_adapter_1, atol=1e-3, rtol=1e-3))
+        assert torch.allclose(logits_adapter_1_after_set, logits_adapter_1, atol=1e-3, rtol=1e-3)
 
         model_copy = copy.deepcopy(model)
         model_copy_2 = copy.deepcopy(model)
         model_merged_all = model.merge_and_unload(adapter_names=["adapter-2", "default"])
 
         with torch.inference_mode():
             logits_merged_all = model_merged_all(**dummy_input)[0]
 
-        self.assertFalse(torch.allclose(logits_merged_all, logits_adapter_2, atol=1e-3, rtol=1e-3))
-        self.assertFalse(torch.allclose(logits_merged_all, logits_adapter_1, atol=1e-3, rtol=1e-3))
+        assert not torch.allclose(logits_merged_all, logits_adapter_2, atol=1e-3, rtol=1e-3)
+        assert not torch.allclose(logits_merged_all, logits_adapter_1, atol=1e-3, rtol=1e-3)
 
         model_merged_adapter_2 = model_copy.merge_and_unload(adapter_names=["adapter-2"])
 
         with torch.inference_mode():
             logits_merged_adapter_2 = model_merged_adapter_2(**dummy_input)[0]
 
-        self.assertTrue(torch.allclose(logits_merged_adapter_2, logits_adapter_2, atol=1e-3, rtol=1e-3))
+        assert torch.allclose(logits_merged_adapter_2, logits_adapter_2, atol=1e-3, rtol=1e-3)
 
         model_merged_adapter_default = model_copy_2.merge_and_unload(adapter_names=["default"])
 
         with torch.inference_mode():
             logits_merged_adapter_default = model_merged_adapter_default(**dummy_input)[0]
 
-        self.assertTrue(torch.allclose(logits_merged_adapter_default, logits_adapter_1, atol=1e-3, rtol=1e-3))
+        assert torch.allclose(logits_merged_adapter_default, logits_adapter_1, atol=1e-3, rtol=1e-3)
 
     def _test_merge_layers_is_idempotent(self, model_id, config_cls, config_kwargs):
         if ("gpt2" in model_id.lower()) and (config_cls != LoraConfig):
             self.skipTest("Merging GPT2 adapters not supported for IA³ (yet)")
 
         model = self.transformers_class.from_pretrained(model_id)
         config = config_cls(
@@ -652,19 +640,43 @@
         model.eval()
         torch.manual_seed(0)
         model.merge_adapter()
         logits_0 = model(**self.prepare_inputs_for_testing())[0]
 
         # merging again should not change anything
         # also check warning:
-        with self.assertWarnsRegex(UserWarning, "All adapters are already merged, nothing to do"):
+        with pytest.warns(UserWarning, match="All adapters are already merged, nothing to do"):
             model.merge_adapter()
         logits_1 = model(**self.prepare_inputs_for_testing())[0]
 
-        self.assertTrue(torch.allclose(logits_0, logits_1, atol=1e-6, rtol=1e-6))
+        assert torch.allclose(logits_0, logits_1, atol=1e-6, rtol=1e-6)
+
+    def _test_safe_merge(self, model_id, config_cls, config_kwargs):
+        torch.manual_seed(0)
+        model = self.transformers_class.from_pretrained(model_id)
+        config = config_cls(
+            base_model_name_or_path=model_id,
+            **config_kwargs,
+        )
+        model = model.to(self.torch_device).eval()
+
+        inputs = self.prepare_inputs_for_testing()
+        logits_base = model(**inputs)[0]
+
+        model = get_peft_model(model, config).eval()
+        logits_peft = model(**inputs)[0]
+
+        # sanity check that the logits are different
+        assert not torch.allclose(logits_base, logits_peft, atol=1e-6, rtol=1e-6)
+
+        model_unloaded = model.merge_and_unload(safe_merge=True)
+        logits_unloaded = model_unloaded(**inputs)[0]
+
+        # check that the logits are the same after unloading
+        assert torch.allclose(logits_peft, logits_unloaded, atol=1e-6, rtol=1e-6)
 
     def _test_generate(self, model_id, config_cls, config_kwargs):
         model = self.transformers_class.from_pretrained(model_id)
         config = config_cls(
             base_model_name_or_path=model_id,
             **config_kwargs,
         )
@@ -683,24 +695,27 @@
             **config_kwargs,
         )
         model = get_peft_model(model, config)
         model = model.to(self.torch_device)
 
         inputs = self.prepare_inputs_for_testing()
         if raises_err:
-            with self.assertRaises(TypeError):
+            with pytest.raises(TypeError):
                 # check if `generate` raises an error if positional arguments are passed
                 _ = model.generate(inputs["input_ids"])
         else:
             # check if `generate` works if positional arguments are passed
             _ = model.generate(inputs["input_ids"])
 
     def _test_generate_half_prec(self, model_id, config_cls, config_kwargs):
         if config_cls not in (IA3Config, LoraConfig, PrefixTuningConfig):
-            return
+            return pytest.skip(f"Test not applicable for {config_cls}")
+
+        if self.torch_device == "mps":  # BFloat16 is not supported on MPS
+            return pytest.skip("BFloat16 is not supported on MPS")
 
         model = self.transformers_class.from_pretrained(model_id, torch_dtype=torch.bfloat16)
         config = config_cls(
             base_model_name_or_path=model_id,
             **config_kwargs,
         )
         model = get_peft_model(model, config)
@@ -710,30 +725,33 @@
         attention_mask = torch.LongTensor([[1, 1, 1], [1, 0, 1]]).to(self.torch_device)
 
         # check if `generate` works
         _ = model.generate(input_ids=input_ids, attention_mask=attention_mask)
 
     def _test_prefix_tuning_half_prec_conversion(self, model_id, config_cls, config_kwargs):
         if config_cls not in (PrefixTuningConfig,):
-            return
+            return pytest.skip(f"Test not applicable for {config_cls}")
 
         config = config_cls(
             base_model_name_or_path=model_id,
             **config_kwargs,
         )
 
         model = self.transformers_class.from_pretrained(model_id)
         model = get_peft_model(model, config)
         model = model.half()
 
-        self.assertEqual(model.base_model_torch_dtype, torch.float16)
+        assert model.base_model_torch_dtype == torch.float16
 
     def _test_training(self, model_id, config_cls, config_kwargs):
-        if config_cls not in (IA3Config, LoraConfig):
-            return
+        if issubclass(config_cls, PromptLearningConfig):
+            return pytest.skip(f"Test not applicable for {config_cls}")
+        if (config_cls == AdaLoraConfig) and ("roberta" in model_id.lower()):
+            # TODO: no gradients on the "dense" layer, other layers work, not sure why
+            self.skipTest("AdaLora with RoBERTa does not work correctly")
 
         model = self.transformers_class.from_pretrained(model_id)
         config = config_cls(
             base_model_name_or_path=model_id,
             **config_kwargs,
         )
         model = get_peft_model(model, config)
@@ -741,24 +759,26 @@
 
         inputs = self.prepare_inputs_for_testing()
 
         # check if `training` works
         output = model(**inputs)[0]
         loss = output.sum()
         loss.backward()
-        parameter_prefix = "ia3" if config_cls == IA3Config else "lora"
+        parameter_prefix = model.prefix
         for n, param in model.named_parameters():
             if (parameter_prefix in n) or ("modules_to_save" in n):
-                self.assertIsNotNone(param.grad)
+                assert param.grad is not None
             else:
-                self.assertIsNone(param.grad)
+                assert param.grad is None
 
     def _test_inference_safetensors(self, model_id, config_cls, config_kwargs):
-        if config_cls not in (LoraConfig,):
-            return
+        if (config_cls == PrefixTuningConfig) and ("deberta" in model_id.lower()):
+            # TODO: raises an error:
+            # TypeError: DebertaModel.forward() got an unexpected keyword argument 'past_key_values'
+            self.skipTest("DeBERTa with PrefixTuning does not work correctly")
 
         config = config_cls(
             base_model_name_or_path=model_id,
             **config_kwargs,
         )
         model = self.transformers_class.from_pretrained(model_id)
         model = get_peft_model(model, config)
@@ -775,26 +795,26 @@
 
         # set to eval mode, since things like dropout can affect the output otherwise
         model.eval()
         logits = model(**inputs)[0][0]
 
         with tempfile.TemporaryDirectory() as tmp_dirname:
             model.save_pretrained(tmp_dirname, safe_serialization=True)
-            self.assertTrue("adapter_model.safetensors" in os.listdir(tmp_dirname))
-            self.assertTrue("adapter_model.bin" not in os.listdir(tmp_dirname))
+            assert "adapter_model.safetensors" in os.listdir(tmp_dirname)
+            assert "adapter_model.bin" not in os.listdir(tmp_dirname)
 
             model_from_pretrained = self.transformers_class.from_pretrained(model_id)
             model_from_pretrained = PeftModel.from_pretrained(model_from_pretrained, tmp_dirname).to(self.torch_device)
 
             logits_from_pretrained = model_from_pretrained(**inputs)[0][0]
-            self.assertTrue(torch.allclose(logits, logits_from_pretrained, atol=1e-4, rtol=1e-4))
+            assert torch.allclose(logits, logits_from_pretrained, atol=1e-4, rtol=1e-4)
 
     def _test_training_layer_indexing(self, model_id, config_cls, config_kwargs):
         if config_cls not in (LoraConfig,):
-            return
+            return pytest.skip(f"Test not applicable for {config_cls}")
 
         config = config_cls(
             base_model_name_or_path=model_id,
             layers_to_transform=[0],
             **config_kwargs,
         )
         model = self.transformers_class.from_pretrained(model_id)
@@ -810,50 +830,54 @@
         loss = output.sum()
         loss.backward()
 
         nb_trainable = 0
 
         for n, param in model.named_parameters():
             if "lora" in n:
-                self.assertIsNotNone(param.grad)
+                assert param.grad is not None
                 nb_trainable += 1
             else:
-                self.assertIsNone(param.grad)
+                assert param.grad is None
 
         with tempfile.TemporaryDirectory() as tmp_dirname:
             model.save_pretrained(tmp_dirname)
 
             model_from_pretrained = self.transformers_class.from_pretrained(model_id)
             model_from_pretrained = PeftModel.from_pretrained(model_from_pretrained, tmp_dirname).to(self.torch_device)
 
             logits_from_pretrained = model_from_pretrained(**inputs)[0][0]
-            self.assertTrue(torch.allclose(logits, logits_from_pretrained, atol=1e-4, rtol=1e-4))
+            assert torch.allclose(logits, logits_from_pretrained, atol=1e-4, rtol=1e-4)
 
         model = self.transformers_class.from_pretrained(model_id)
         config = config_cls(
             base_model_name_or_path=model_id,
             **config_kwargs,
         )
         model = get_peft_model(model, config)
         nb_trainable_all = 0
 
         for n, param in model.named_parameters():
             if "lora" in n:
                 nb_trainable_all += 1
 
-        self.assertLess(nb_trainable, nb_trainable_all)
+        assert nb_trainable < nb_trainable_all
 
     def _test_training_gradient_checkpointing(self, model_id, config_cls, config_kwargs):
-        if config_cls not in (LoraConfig, IA3Config):
-            return
+        if issubclass(config_cls, PromptLearningConfig):
+            return pytest.skip(f"Test not applicable for {config_cls}")
+
+        if (config_cls == AdaLoraConfig) and ("roberta" in model_id.lower()):
+            # TODO: no gradients on the "dense" layer, other layers work, not sure why
+            self.skipTest("AdaLora with RoBERTa does not work correctly")
 
         model = self.transformers_class.from_pretrained(model_id)
 
         if not getattr(model, "supports_gradient_checkpointing", False):
-            return
+            return pytest.skip(f"Model {model_id} does not support gradient checkpointing")
 
         model.gradient_checkpointing_enable()
 
         config = config_cls(
             base_model_name_or_path=model_id,
             **config_kwargs,
         )
@@ -866,21 +890,21 @@
         output = model(**inputs)[0]
 
         loss = output.sum()
         loss.backward()
         parameter_prefix = "ia3" if config_cls == IA3Config else "lora"
         for n, param in model.named_parameters():
             if parameter_prefix in n:
-                self.assertIsNotNone(param.grad)
+                assert param.grad is not None
             else:
-                self.assertIsNone(param.grad)
+                assert param.grad is None
 
     def _test_peft_model_device_map(self, model_id, config_cls, config_kwargs):
         if config_cls not in (LoraConfig,):
-            return
+            return pytest.skip(f"Test not applicable for {config_cls}")
 
         config = config_cls(
             base_model_name_or_path=model_id,
             **config_kwargs,
         )
 
         model = self.transformers_class.from_pretrained(model_id)
@@ -894,15 +918,15 @@
             model_from_pretrained = self.transformers_class.from_pretrained(model_id)
             _ = PeftModel.from_pretrained(model_from_pretrained, tmp_dirname, device_map={"": "cpu"}).to(
                 self.torch_device
             )
 
     def _test_training_prompt_learning_tasks(self, model_id, config_cls, config_kwargs):
         if not issubclass(config_cls, PromptLearningConfig):
-            return
+            return pytest.skip(f"Test not applicable for {config_cls}")
 
         model = self.transformers_class.from_pretrained(model_id)
         config = config_cls(
             base_model_name_or_path=model_id,
             **config_kwargs,
         )
         model = get_peft_model(model, config)
@@ -913,48 +937,48 @@
         # check if `training` works
         output = model(**inputs)[0]
         loss = output.sum()
         loss.backward()
 
         # check that prompt encoder has grads
         for param in model.prompt_encoder.parameters():
-            self.assertIsNotNone(param.grad)
+            assert param.grad is not None
 
     def _test_delete_adapter(self, model_id, config_cls, config_kwargs):
         supported_peft_types = [PeftType.LORA, PeftType.LOHA, PeftType.LOKR, PeftType.IA3, PeftType.OFT]
         # IA3 does not support deleting adapters yet, but it just needs to be added
         # AdaLora does not support multiple adapters
         config = config_cls(
             base_model_name_or_path=model_id,
             **config_kwargs,
         )
         if config.peft_type not in supported_peft_types:
-            return
+            return pytest.skip(f"Test not applicable for {config.peft_type}")
 
         model = self.transformers_class.from_pretrained(model_id)
         adapter_to_delete = "delete_me"
         model = get_peft_model(model, config)
         model.add_adapter(adapter_to_delete, config)
         model.set_adapter(adapter_to_delete)
         model = model.to(self.torch_device)
         model.delete_adapter(adapter_to_delete)
-        self.assertFalse(adapter_to_delete in model.peft_config)
-        self.assertEqual(model.active_adapters, ["default"])
+        assert adapter_to_delete not in model.peft_config
+        assert model.active_adapters == ["default"]
 
         key_list = [key for key, _ in model.named_modules()]
         for key in key_list:
             _, target, _ = _get_submodules(model, key)
             attributes_to_check = getattr(target, "adapter_layer_names", []) + getattr(target, "other_param_names", [])
             for attr in attributes_to_check:
-                self.assertFalse(adapter_to_delete in getattr(target, attr))
+                assert adapter_to_delete not in getattr(target, attr)
 
         # check that we can also delete the last remaining adapter
         model.delete_adapter("default")
-        self.assertFalse("default" in model.peft_config)
-        self.assertEqual(model.active_adapters, [])
+        assert "default" not in model.peft_config
+        assert model.active_adapters == []
 
         input = self.prepare_inputs_for_testing()
         # note: we cannot call model(**input) because PeftModel always expects there to be at least one adapter
         model.base_model(**input)  # should not raise an error
 
     def _test_delete_inactive_adapter(self, model_id, config_cls, config_kwargs):
         # same as test_delete_adapter, but this time an inactive adapter is deleted
@@ -962,37 +986,37 @@
         # IA3 does not support deleting adapters yet, but it just needs to be added
         # AdaLora does not support multiple adapters
         config = config_cls(
             base_model_name_or_path=model_id,
             **config_kwargs,
         )
         if config.peft_type not in supported_peft_types:
-            return
+            return pytest.skip(f"Test not applicable for {config.peft_type}")
 
         model = self.transformers_class.from_pretrained(model_id)
         adapter_to_delete = "delete_me"
         model = get_peft_model(model, config)
         model.add_adapter(adapter_to_delete, config)
         # "delete_me" is added but not activated
         model = model.to(self.torch_device)
         model.delete_adapter(adapter_to_delete)
-        self.assertFalse(adapter_to_delete in model.peft_config)
-        self.assertEqual(model.active_adapters, ["default"])
+        assert adapter_to_delete not in model.peft_config
+        assert model.active_adapters == ["default"]
 
         key_list = [key for key, _ in model.named_modules()]
         for key in key_list:
             _, target, _ = _get_submodules(model, key)
             attributes_to_check = getattr(target, "adapter_layer_names", []) + getattr(target, "other_param_names", [])
             for attr in attributes_to_check:
-                self.assertFalse(adapter_to_delete in getattr(target, attr))
+                assert adapter_to_delete not in getattr(target, attr)
 
         # check that we can also delete the last remaining adapter
         model.delete_adapter("default")
-        self.assertFalse("default" in model.peft_config)
-        self.assertEqual(model.active_adapters, [])
+        assert "default" not in model.peft_config
+        assert model.active_adapters == []
 
         input = self.prepare_inputs_for_testing()
         # note: we cannot call model(**input) because PeftModel always expects there to be at least one adapter
         model.base_model(**input)  # should not raise an error
 
     def _test_unload_adapter(self, model_id, config_cls, config_kwargs):
         model = self.transformers_class.from_pretrained(model_id)
@@ -1000,117 +1024,227 @@
             base_model_name_or_path=model_id,
             **config_kwargs,
         )
         model = get_peft_model(model, config)
         model = model.to(self.torch_device)
 
         if config.peft_type not in ("LORA", "ADALORA", "IA3"):
-            with self.assertRaises(AttributeError):
+            with pytest.raises(AttributeError):
                 model = model.unload()
         else:
             dummy_input = self.prepare_inputs_for_testing()
             logits_with_adapter = model(**dummy_input)[0]
 
             transformers_model = self.transformers_class.from_pretrained(model_id).to(self.torch_device)
             logits_transformers = transformers_model(**dummy_input)[0]
 
             model.eval()
             model = model.unload()
             logits_unload = model(**dummy_input)[0]
 
-            self.assertFalse(torch.allclose(logits_with_adapter, logits_unload, atol=1e-10, rtol=1e-10))
-            self.assertTrue(torch.allclose(logits_transformers, logits_unload, atol=1e-4, rtol=1e-4))
+            assert not torch.allclose(logits_with_adapter, logits_unload, atol=1e-10, rtol=1e-10)
+            assert torch.allclose(logits_transformers, logits_unload, atol=1e-4, rtol=1e-4)
 
     def _test_weighted_combination_of_adapters(self, model_id, config_cls, config_kwargs):
         if issubclass(config_cls, AdaLoraConfig):
             # AdaLora does not support adding more than 1 adapter
-            return
+            return pytest.skip(f"Test not applicable for {config_cls}")
 
         adapter_list = ["adapter1", "adapter_2", "adapter_3"]
         weight_list = [0.5, 1.5, 1.5]
         config = config_cls(
             base_model_name_or_path=model_id,
             **config_kwargs,
         )
-        if not isinstance(config, (LoraConfig)):
-            return
+        if not isinstance(config, LoraConfig):
+            return pytest.skip(f"Test not applicable for {config}")
 
         model = self.transformers_class.from_pretrained(model_id)
         model = get_peft_model(model, config, adapter_list[0])
         model.add_adapter(adapter_list[1], config)
         model.add_adapter(adapter_list[2], replace(config, r=20))
         model = model.to(self.torch_device)
 
         # test re-weighting single adapter
         model.add_weighted_adapter([adapter_list[0]], [weight_list[0]], "single_adapter_reweighting")
 
         # test svd re-weighting with multiple adapters
         model.add_weighted_adapter(adapter_list[1:], weight_list[1:], "multi_adapter_svd_reweighting")
 
+        # test ties_svd re-weighting with multiple adapters
+        model.add_weighted_adapter(
+            adapter_list[1:],
+            weight_list[1:],
+            "multi_adapter_ties_svd_reweighting",
+            combination_type="ties_svd",
+            density=0.5,
+        )
+
+        # test dare_linear_svd re-weighting with multiple adapters
+        model.add_weighted_adapter(
+            adapter_list[1:],
+            weight_list[1:],
+            "multi_adapter_dare_linear_svd_reweighting",
+            combination_type="dare_linear_svd",
+            density=0.5,
+        )
+
+        # test dare_ties_svd re-weighting with multiple adapters
+        model.add_weighted_adapter(
+            adapter_list[1:],
+            weight_list[1:],
+            "multi_adapter_dare_ties_svd_reweighting",
+            combination_type="dare_ties_svd",
+            density=0.5,
+        )
+
+        # test magnitude_prune_svd re-weighting with multiple adapters
+        model.add_weighted_adapter(
+            adapter_list[1:],
+            weight_list[1:],
+            "multi_adapter_magnitude_prune_svd_reweighting",
+            combination_type="magnitude_prune_svd",
+            density=0.5,
+        )
+
         # test cat re-weighting with multiple adapters
         model.add_weighted_adapter(
             adapter_list[1:], weight_list[1:], "multi_adapter_cat_reweighting", combination_type="cat"
         )
 
         # test linear re-weighting with multiple adapters
         model.add_weighted_adapter(
             adapter_list[:2], weight_list[:2], "multi_adapter_linear_reweighting", combination_type="linear"
         )
 
+        # test ties re-weighting with multiple adapters
+        model.add_weighted_adapter(
+            adapter_list[:2], weight_list[:2], "multi_adapter_ties_reweighting", combination_type="ties", density=0.5
+        )
+
+        # test dare_linear re-weighting with multiple adapters
+        model.add_weighted_adapter(
+            adapter_list[:2],
+            weight_list[:2],
+            "multi_adapter_dare_linear_reweighting",
+            combination_type="dare_linear",
+            density=0.5,
+        )
+
+        # test dare_ties re-weighting with multiple adapters
+        model.add_weighted_adapter(
+            adapter_list[:2],
+            weight_list[:2],
+            "multi_adapter_dare_ties_reweighting",
+            combination_type="dare_ties",
+            density=0.5,
+        )
+
+        # test magnitude_prune re-weighting with multiple adapters
+        model.add_weighted_adapter(
+            adapter_list[:2],
+            weight_list[:2],
+            "multi_adapter_magnitude_prune_reweighting",
+            combination_type="magnitude_prune",
+            density=0.5,
+        )
+
         # test linear re-weighting with multiple adapters with only first adapter having non zero weight
         model.add_weighted_adapter(
             adapter_list[:2],
             [weight_list[0], 0],
             "multi_adapter_linear_reweighting_single_enabled",
             combination_type="linear",
         )
 
-        with self.assertRaises(ValueError):
+        with pytest.raises(ValueError):
             model.add_weighted_adapter(
                 adapter_list[1:],
                 weight_list[1:],
                 "multi_adapter_linear_reweighting_uneven_r",
                 combination_type="linear",
             )
 
+        with pytest.raises(ValueError):
+            model.add_weighted_adapter(
+                adapter_list[1:],
+                weight_list[1:],
+                "multi_adapter_ties_reweighting_uneven_r",
+                combination_type="ties",
+                density=0.5,
+            )
+
+        with pytest.raises(ValueError):
+            model.add_weighted_adapter(
+                adapter_list[1:],
+                weight_list[1:],
+                "multi_adapter_dare_linear_reweighting_uneven_r",
+                combination_type="dare_linear",
+                density=0.5,
+            )
+
+        with pytest.raises(ValueError):
+            model.add_weighted_adapter(
+                adapter_list[1:],
+                weight_list[1:],
+                "multi_adapter_dare_ties_reweighting_uneven_r",
+                combination_type="dare_ties",
+                density=0.5,
+            )
+
+        with pytest.raises(ValueError):
+            model.add_weighted_adapter(
+                adapter_list[1:],
+                weight_list[1:],
+                "multi_adapter_magnitude_prune_reweighting_uneven_r",
+                combination_type="magnitude_prune",
+                density=0.5,
+            )
+
         new_adapters = [
             "single_adapter_reweighting",
             "multi_adapter_svd_reweighting",
+            "multi_adapter_ties_svd_reweighting",
+            "multi_adapter_dare_linear_svd_reweighting",
+            "multi_adapter_dare_ties_svd_reweighting",
+            "multi_adapter_magnitude_prune_svd_reweighting",
             "multi_adapter_cat_reweighting",
             "multi_adapter_linear_reweighting",
             "multi_adapter_linear_reweighting_single_enabled",
+            "multi_adapter_ties_reweighting",
+            "multi_adapter_dare_linear_reweighting",
+            "multi_adapter_dare_ties_reweighting",
+            "multi_adapter_magnitude_prune_reweighting",
         ]
         for new_adapter in new_adapters:
-            self.assertTrue(new_adapter in model.peft_config)
+            assert new_adapter in model.peft_config
 
         key_list = [key for key, _ in model.named_modules()]
         for key in key_list:
             _, target, _ = _get_submodules(model, key)
             if isinstance(target, LoraLayer):
                 for adapter_name in new_adapters:
                     if "single" in adapter_name:
                         new_delta_weight = target.get_delta_weight(adapter_name)
                         weighted_original_delta_weights = target.get_delta_weight(adapter_list[0]) * weight_list[0]
-                        self.assertTrue(
-                            torch.allclose(new_delta_weight, weighted_original_delta_weights, atol=1e-4, rtol=1e-4)
-                        )
+                        assert torch.allclose(new_delta_weight, weighted_original_delta_weights, atol=1e-4, rtol=1e-4)
                     elif "svd" in adapter_name:
-                        self.assertTrue(target.r[adapter_name] == 20)
+                        assert target.r[adapter_name] == 20
                     elif "linear" in adapter_name:
-                        self.assertTrue(target.r[adapter_name] == 8)
+                        assert target.r[adapter_name] == 8
                     elif "cat" in adapter_name:
-                        self.assertTrue(target.r[adapter_name] == 28)
+                        assert target.r[adapter_name] == 28
 
         dummy_input = self.prepare_inputs_for_testing()
         model.eval()
         for adapter_name in new_adapters:
             # ensuring new adapters pass the forward loop
             model.set_adapter(adapter_name)
-            self.assertTrue(model.active_adapter == adapter_name)
-            self.assertTrue(model.active_adapters == [adapter_name])
+            assert model.active_adapter == adapter_name
+            assert model.active_adapters == [adapter_name]
             model(**dummy_input)[0]
 
     def _test_disable_adapter(self, model_id, config_cls, config_kwargs):
         task_type = config_kwargs.get("task_type")
         if (task_type == "SEQ_2_SEQ_LM") and (config_cls in (PromptTuningConfig, PromptEncoderConfig)):
             self.skipTest("Seq2Seq + prompt tuning/prompt encoder does not work with disabling adapters")
 
@@ -1154,53 +1288,58 @@
 
         output_peft = get_output(peft_model)
 
         # first check trivial case is not true that peft does not affect the output; for this to work, init_lora_weight
         # must be False
         if isinstance(peft_model, StableDiffusionPipeline):
             # for SD, check that most pixels have different values
-            self.assertTrue((output_before != output_peft).float().mean() > 0.8)
+            assert (output_before != output_peft).float().mean() > 0.8
         else:
-            self.assertFalse(torch.allclose(output_before, output_peft))
+            assert not torch.allclose(output_before, output_peft)
 
         # output with DISABLED ADAPTER
         if isinstance(peft_model, StableDiffusionPipeline):
             with peft_model.unet.disable_adapter():
                 with peft_model.text_encoder.disable_adapter():
                     output_peft_disabled = get_output(peft_model)
             # for SD, very rarely, a pixel can differ
-            self.assertTrue((output_before != output_peft_disabled).float().mean() < 1e-4)
+            assert (output_before != output_peft_disabled).float().mean() < 1e-4
         else:
             with peft_model.disable_adapter():
                 output_peft_disabled = get_output(peft_model)
-            self.assertTrue(torch.allclose(output_before, output_peft_disabled, atol=1e-6, rtol=1e-6))
+            assert torch.allclose(output_before, output_peft_disabled, atol=1e-6, rtol=1e-6)
+
+            # after leaving the disable_adapter context, the output should be the same as with enabled adapter again
+            # see #1501
+            output_peft_after_disabled = get_output(peft_model)
+            assert torch.allclose(output_peft, output_peft_after_disabled, atol=1e-6, rtol=1e-6)
 
         # TODO: add tests to check if disabling adapters works after calling merge_adapter
 
     def _test_adding_multiple_adapters_with_bias_raises(self, model_id, config_cls, config_kwargs):
         # When trying to add multiple adapters with bias in Lora or AdaLora, an error should be
         # raised. Also, the peft model should not be left in a half-initialized state.
         if not issubclass(config_cls, (LoraConfig, AdaLoraConfig)):
-            return
+            return pytest.skip(f"Test not applicable for {config_cls}")
 
         config_kwargs = config_kwargs.copy()
         config_kwargs["bias"] = "all"
         config = config_cls(
             base_model_name_or_path=model_id,
             **config_kwargs,
         )
 
         model = self.transformers_class.from_pretrained(model_id)
         model = get_peft_model(model, config, "adapter0")
-        with self.assertRaises(ValueError):
+        with pytest.raises(ValueError):
             model.add_adapter("adapter1", replace(config, r=20))
 
         # (superficial) test that the model is not left in a half-initialized state when adding an adapter fails
-        self.assertFalse("adapter1" in model.peft_config)
-        self.assertFalse("adapter1" in model.base_model.peft_config)
+        assert "adapter1" not in model.peft_config
+        assert "adapter1" not in model.base_model.peft_config
 
     def _test_passing_input_embeds_works(self, test_name, model_id, config_cls, config_kwargs):
         # https://github.com/huggingface/peft/issues/727
         model = self.transformers_class.from_pretrained(model_id)
         config = config_cls(
             base_model_name_or_path=model_id,
             **config_kwargs,
```

### Comparing `peft-0.8.2/tests/testing_utils.py` & `peft-0.9.0/tests/testing_utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# coding=utf-8
 # Copyright 2023-present the HuggingFace Inc. team.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
@@ -15,15 +14,15 @@
 import unittest
 from contextlib import contextmanager
 
 import numpy as np
 import pytest
 import torch
 
-from peft.import_utils import is_auto_gptq_available, is_optimum_available
+from peft.import_utils import is_aqlm_available, is_auto_awq_available, is_auto_gptq_available, is_optimum_available
 
 
 def require_torch_gpu(test_case):
     """
     Decorator marking a test that requires a GPU. Will be skipped when no GPU is available.
     """
     if not torch.cuda.is_available():
@@ -58,14 +57,28 @@
 def require_auto_gptq(test_case):
     """
     Decorator marking a test that requires auto-gptq. These tests are skipped when auto-gptq isn't installed.
     """
     return unittest.skipUnless(is_auto_gptq_available(), "test requires auto-gptq")(test_case)
 
 
+def require_aqlm(test_case):
+    """
+    Decorator marking a test that requires aqlm. These tests are skipped when aqlm isn't installed.
+    """
+    return unittest.skipUnless(is_aqlm_available(), "test requires aqlm")(test_case)
+
+
+def require_auto_awq(test_case):
+    """
+    Decorator marking a test that requires auto-awq. These tests are skipped when auto-awq isn't installed.
+    """
+    return unittest.skipUnless(is_auto_awq_available(), "test requires auto-awq")(test_case)
+
+
 def require_optimum(test_case):
     """
     Decorator marking a test that requires optimum. These tests are skipped when optimum isn't installed.
     """
     return unittest.skipUnless(is_optimum_available(), "test requires optimum")(test_case)
```

