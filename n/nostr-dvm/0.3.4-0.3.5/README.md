# Comparing `tmp/nostr_dvm-0.3.4.tar.gz` & `tmp/nostr_dvm-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nostr_dvm-0.3.4.tar", last modified: Mon Apr 29 13:36:26 2024, max compression
+gzip compressed data, was "nostr_dvm-0.3.5.tar", last modified: Mon May  6 10:19:10 2024, max compression
```

## Comparing `nostr_dvm-0.3.4.tar` & `nostr_dvm-0.3.5.tar`

### file list

```diff
@@ -1,115 +1,115 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:36:26.079397 nostr_dvm-0.3.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-29 13:36:22.000000 nostr_dvm-0.3.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-04-29 13:36:26.079397 nostr_dvm-0.3.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1563 2024-04-29 13:36:22.000000 nostr_dvm-0.3.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:36:26.067397 nostr_dvm-0.3.4/nostr_dvm/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 13:36:22.000000 nostr_dvm-0.3.4/nostr_dvm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:36:26.067397 nostr_dvm-0.3.4/nostr_dvm/backends/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 13:36:22.000000 nostr_dvm-0.3.4/nostr_dvm/backends/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:36:26.067397 nostr_dvm-0.3.4/nostr_dvm/backends/mlx/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 13:36:22.000000 nostr_dvm-0.3.4/nostr_dvm/backends/mlx/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:36:26.067397 nostr_dvm-0.3.4/nostr_dvm/backends/mlx/modules/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 13:36:22.000000 nostr_dvm-0.3.4/nostr_dvm/backends/mlx/modules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:36:26.067397 nostr_dvm-0.3.4/nostr_dvm/backends/mlx/modules/stable_diffusion/
--rw-r--r--   0 runner    (1001) docker     (127)     2945 2024-04-29 13:36:22.000000 nostr_dvm-0.3.4/nostr_dvm/backends/mlx/modules/stable_diffusion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2222 2024-04-29 13:36:22.000000 nostr_dvm-0.3.4/nostr_dvm/backends/mlx/modules/stable_diffusion/clip.py
--rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-04-29 13:36:22.000000 nostr_dvm-0.3.4/nostr_dvm/backends/mlx/modules/stable_diffusion/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     9892 2024-04-29 13:36:22.000000 nostr_dvm-0.3.4/nostr_dvm/backends/mlx/modules/stable_diffusion/model_io.py
--rw-r--r--   0 runner    (1001) docker     (127)     2300 2024-04-29 13:36:22.000000 nostr_dvm-0.3.4/nostr_dvm/backends/mlx/modules/stable_diffusion/sampler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2991 2024-04-29 13:36:22.000000 nostr_dvm-0.3.4/nostr_dvm/backends/mlx/modules/stable_diffusion/tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (127)    13685 2024-04-29 13:36:22.000000 nostr_dvm-0.3.4/nostr_dvm/backends/mlx/modules/stable_diffusion/unet.py
--rw-r--r--   0 runner    (1001) docker     (127)     7773 2024-04-29 13:36:22.000000 nostr_dvm-0.3.4/nostr_dvm/backends/mlx/modules/stable_diffusion/vae.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:36:26.067397 nostr_dvm-0.3.4/nostr_dvm/backends/nova_server/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 13:36:22.000000 nostr_dvm-0.3.4/nostr_dvm/backends/nova_server/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:36:26.067397 nostr_dvm-0.3.4/nostr_dvm/backends/nova_server/modules/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 13:36:22.000000 nostr_dvm-0.3.4/nostr_dvm/backends/nova_server/modules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:36:26.071397 nostr_dvm-0.3.4/nostr_dvm/backends/nova_server/modules/image_interrogator/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 13:36:22.000000 nostr_dvm-0.3.4/nostr_dvm/backends/nova_server/modules/image_interrogator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4906 2024-04-29 13:36:22.000000 nostr_dvm-0.3.4/nostr_dvm/backends/nova_server/modules/image_interrogator/image_interrogator.py
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-04-29 13:36:22.000000 nostr_dvm-0.3.4/nostr_dvm/backends/nova_server/modules/image_interrogator/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:36:26.071397 nostr_dvm-0.3.4/nostr_dvm/backends/nova_server/modules/image_upscale/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 13:36:22.000000 nostr_dvm-0.3.4/nostr_dvm/backends/nova_server/modules/image_upscale/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6863 2024-04-29 13:36:22.000000 nostr_dvm-0.3.4/nostr_dvm/backends/nova_server/modules/image_upscale/image_upscale_realesrgan.py
--rw-r--r--   0 runner    (1001) docker     (127)     7745 2024-04-29 13:36:22.000000 nostr_dvm-0.3.4/nostr_dvm/backends/nova_server/modules/image_upscale/inference_realesrgan.py
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-04-29 13:36:22.000000 nostr_dvm-0.3.4/nostr_dvm/backends/nova_server/modules/image_upscale/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:36:26.071397 nostr_dvm-0.3.4/nostr_dvm/backends/nova_server/modules/stablediffusionxl/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 13:36:22.000000 nostr_dvm-0.3.4/nostr_dvm/backends/nova_server/modules/stablediffusionxl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3319 2024-04-29 13:36:22.000000 nostr_dvm-0.3.4/nostr_dvm/backends/nova_server/modules/stablediffusionxl/lora.py
--rw-r--r--   0 runner    (1001) docker     (127)     6854 2024-04-29 13:36:22.000000 nostr_dvm-0.3.4/nostr_dvm/backends/nova_server/modules/stablediffusionxl/stablediffusionxl-img2img.py
--rw-r--r--   0 runner    (1001) docker     (127)     9229 2024-04-29 13:36:22.000000 nostr_dvm-0.3.4/nostr_dvm/backends/nova_server/modules/stablediffusionxl/stablediffusionxl.py
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-29 13:36:22.000000 nostr_dvm-0.3.4/nostr_dvm/backends/nova_server/modules/stablediffusionxl/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:36:26.071397 nostr_dvm-0.3.4/nostr_dvm/backends/nova_server/modules/whisperx/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 13:36:22.000000 nostr_dvm-0.3.4/nostr_dvm/backends/nova_server/modules/whisperx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-29 13:36:22.000000 nostr_dvm-0.3.4/nostr_dvm/backends/nova_server/modules/whisperx/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     5250 2024-04-29 13:36:22.000000 nostr_dvm-0.3.4/nostr_dvm/backends/nova_server/modules/whisperx/whisperx_transcript.py
--rw-r--r--   0 runner    (1001) docker     (127)     4880 2024-04-29 13:36:22.000000 nostr_dvm-0.3.4/nostr_dvm/backends/nova_server/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    39816 2024-04-29 13:36:22.000000 nostr_dvm-0.3.4/nostr_dvm/bot.py
--rw-r--r--   0 runner    (1001) docker     (127)    39377 2024-04-29 13:36:22.000000 nostr_dvm-0.3.4/nostr_dvm/dvm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:36:26.071397 nostr_dvm-0.3.4/nostr_dvm/interfaces/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 13:36:22.000000 nostr_dvm-0.3.4/nostr_dvm/interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6126 2024-04-29 13:36:22.000000 nostr_dvm-0.3.4/nostr_dvm/interfaces/dvmtaskinterface.py
--rw-r--r--   0 runner    (1001) docker     (127)    23351 2024-04-29 13:36:22.000000 nostr_dvm-0.3.4/nostr_dvm/subscription.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:36:26.075397 nostr_dvm-0.3.4/nostr_dvm/tasks/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 13:36:22.000000 nostr_dvm-0.3.4/nostr_dvm/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8321 2024-04-29 13:36:22.000000 nostr_dvm-0.3.4/nostr_dvm/tasks/advanced_search.py
--rw-r--r--   0 runner    (1001) docker     (127)     7452 2024-04-29 13:36:22.000000 nostr_dvm-0.3.4/nostr_dvm/tasks/advanced_search_wine.py
--rw-r--r--   0 runner    (1001) docker     (127)    11255 2024-04-29 13:36:22.000000 nostr_dvm-0.3.4/nostr_dvm/tasks/content_discovery_currently_popular.py
--rw-r--r--   0 runner    (1001) docker     (127)    12843 2024-04-29 13:36:22.000000 nostr_dvm-0.3.4/nostr_dvm/tasks/content_discovery_currently_popular_followers.py
--rw-r--r--   0 runner    (1001) docker     (127)     4049 2024-04-29 13:36:22.000000 nostr_dvm-0.3.4/nostr_dvm/tasks/convert_media.py
--rw-r--r--   0 runner    (1001) docker     (127)     7785 2024-04-29 13:36:22.000000 nostr_dvm-0.3.4/nostr_dvm/tasks/discovery_bot_farms.py
--rw-r--r--   0 runner    (1001) docker     (127)     8084 2024-04-29 13:36:22.000000 nostr_dvm-0.3.4/nostr_dvm/tasks/discovery_censor_wot.py
--rw-r--r--   0 runner    (1001) docker     (127)     8964 2024-04-29 13:36:22.000000 nostr_dvm-0.3.4/nostr_dvm/tasks/discovery_inactive_follows.py
--rw-r--r--   0 runner    (1001) docker     (127)     8995 2024-04-29 13:36:22.000000 nostr_dvm-0.3.4/nostr_dvm/tasks/discovery_nonfollowers.py
--rw-r--r--   0 runner    (1001) docker     (127)     4473 2024-04-29 13:36:22.000000 nostr_dvm-0.3.4/nostr_dvm/tasks/discovery_trending_notes_nostrband.py
--rw-r--r--   0 runner    (1001) docker     (127)     6218 2024-04-29 13:36:22.000000 nostr_dvm-0.3.4/nostr_dvm/tasks/imagegeneration_openai_dalle.py
--rw-r--r--   0 runner    (1001) docker     (127)     5968 2024-04-29 13:36:22.000000 nostr_dvm-0.3.4/nostr_dvm/tasks/imagegeneration_replicate_sdxl.py
--rw-r--r--   0 runner    (1001) docker     (127)     6897 2024-04-29 13:36:22.000000 nostr_dvm-0.3.4/nostr_dvm/tasks/imagegeneration_sd21_mlx.py
--rw-r--r--   0 runner    (1001) docker     (127)     8391 2024-04-29 13:36:22.000000 nostr_dvm-0.3.4/nostr_dvm/tasks/imagegeneration_sdxl.py
--rw-r--r--   0 runner    (1001) docker     (127)     9045 2024-04-29 13:36:22.000000 nostr_dvm-0.3.4/nostr_dvm/tasks/imagegeneration_sdxlimg2img.py
--rw-r--r--   0 runner    (1001) docker     (127)     5281 2024-04-29 13:36:22.000000 nostr_dvm-0.3.4/nostr_dvm/tasks/imageinterrogator.py
--rw-r--r--   0 runner    (1001) docker     (127)     5283 2024-04-29 13:36:22.000000 nostr_dvm-0.3.4/nostr_dvm/tasks/imageupscale.py
--rw-r--r--   0 runner    (1001) docker     (127)     8169 2024-04-29 13:36:22.000000 nostr_dvm-0.3.4/nostr_dvm/tasks/search_users.py
--rw-r--r--   0 runner    (1001) docker     (127)     6450 2024-04-29 13:36:22.000000 nostr_dvm-0.3.4/nostr_dvm/tasks/summarization_huggingchat.py
--rw-r--r--   0 runner    (1001) docker     (127)     6945 2024-04-29 13:36:22.000000 nostr_dvm-0.3.4/nostr_dvm/tasks/summarization_unleashed_chat.py
--rw-r--r--   0 runner    (1001) docker     (127)     6774 2024-04-29 13:36:22.000000 nostr_dvm-0.3.4/nostr_dvm/tasks/textextraction_google.py
--rw-r--r--   0 runner    (1001) docker     (127)     4514 2024-04-29 13:36:22.000000 nostr_dvm-0.3.4/nostr_dvm/tasks/textextraction_pdf.py
--rw-r--r--   0 runner    (1001) docker     (127)     7781 2024-04-29 13:36:22.000000 nostr_dvm-0.3.4/nostr_dvm/tasks/textextraction_whisperx.py
--rw-r--r--   0 runner    (1001) docker     (127)     4320 2024-04-29 13:36:22.000000 nostr_dvm-0.3.4/nostr_dvm/tasks/textgeneration_huggingchat.py
--rw-r--r--   0 runner    (1001) docker     (127)     4985 2024-04-29 13:36:22.000000 nostr_dvm-0.3.4/nostr_dvm/tasks/textgeneration_llmlite.py
--rw-r--r--   0 runner    (1001) docker     (127)     4664 2024-04-29 13:36:22.000000 nostr_dvm-0.3.4/nostr_dvm/tasks/textgeneration_unleashed_chat.py
--rw-r--r--   0 runner    (1001) docker     (127)     6897 2024-04-29 13:36:22.000000 nostr_dvm-0.3.4/nostr_dvm/tasks/texttospeech.py
--rw-r--r--   0 runner    (1001) docker     (127)     7004 2024-04-29 13:36:22.000000 nostr_dvm-0.3.4/nostr_dvm/tasks/translation_google.py
--rw-r--r--   0 runner    (1001) docker     (127)     6895 2024-04-29 13:36:22.000000 nostr_dvm-0.3.4/nostr_dvm/tasks/translation_libretranslate.py
--rw-r--r--   0 runner    (1001) docker     (127)     5571 2024-04-29 13:36:22.000000 nostr_dvm-0.3.4/nostr_dvm/tasks/videogeneration_replicate_svd.py
--rw-r--r--   0 runner    (1001) docker     (127)     4892 2024-04-29 13:36:22.000000 nostr_dvm-0.3.4/nostr_dvm/tasks/videogeneration_svd.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:36:26.079397 nostr_dvm-0.3.4/nostr_dvm/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 13:36:22.000000 nostr_dvm-0.3.4/nostr_dvm/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4334 2024-04-29 13:36:22.000000 nostr_dvm-0.3.4/nostr_dvm/utils/admin_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8745 2024-04-29 13:36:22.000000 nostr_dvm-0.3.4/nostr_dvm/utils/backend_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6163 2024-04-29 13:36:22.000000 nostr_dvm-0.3.4/nostr_dvm/utils/cashu_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     9473 2024-04-29 13:36:22.000000 nostr_dvm-0.3.4/nostr_dvm/utils/database_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2700 2024-04-29 13:36:22.000000 nostr_dvm-0.3.4/nostr_dvm/utils/definitions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2387 2024-04-29 13:36:22.000000 nostr_dvm-0.3.4/nostr_dvm/utils/dvmconfig.py
--rw-r--r--   0 runner    (1001) docker     (127)     2761 2024-04-29 13:36:22.000000 nostr_dvm-0.3.4/nostr_dvm/utils/external_dvm_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    13403 2024-04-29 13:36:22.000000 nostr_dvm-0.3.4/nostr_dvm/utils/mediasource_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8866 2024-04-29 13:36:22.000000 nostr_dvm-0.3.4/nostr_dvm/utils/nip88_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4170 2024-04-29 13:36:22.000000 nostr_dvm-0.3.4/nostr_dvm/utils/nip89_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8449 2024-04-29 13:36:22.000000 nostr_dvm-0.3.4/nostr_dvm/utils/nostr_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3795 2024-04-29 13:36:22.000000 nostr_dvm-0.3.4/nostr_dvm/utils/nwc_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     9014 2024-04-29 13:36:22.000000 nostr_dvm-0.3.4/nostr_dvm/utils/output_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:36:26.079397 nostr_dvm-0.3.4/nostr_dvm/utils/scrapper/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 13:36:22.000000 nostr_dvm-0.3.4/nostr_dvm/utils/scrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    26119 2024-04-29 13:36:22.000000 nostr_dvm-0.3.4/nostr_dvm/utils/scrapper/media_scrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     5712 2024-04-29 13:36:22.000000 nostr_dvm-0.3.4/nostr_dvm/utils/subscription_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    15021 2024-04-29 13:36:22.000000 nostr_dvm-0.3.4/nostr_dvm/utils/zap_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:36:26.079397 nostr_dvm-0.3.4/nostr_dvm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-04-29 13:36:26.000000 nostr_dvm-0.3.4/nostr_dvm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4118 2024-04-29 13:36:26.000000 nostr_dvm-0.3.4/nostr_dvm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 13:36:26.000000 nostr_dvm-0.3.4/nostr_dvm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-04-29 13:36:26.000000 nostr_dvm-0.3.4/nostr_dvm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-29 13:36:26.000000 nostr_dvm-0.3.4/nostr_dvm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 13:36:26.079397 nostr_dvm-0.3.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1652 2024-04-29 13:36:22.000000 nostr_dvm-0.3.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:36:26.079397 nostr_dvm-0.3.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    12655 2024-04-29 13:36:22.000000 nostr_dvm-0.3.4/tests/test_dvm_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     3213 2024-04-29 13:36:22.000000 nostr_dvm-0.3.4/tests/test_events.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 10:19:10.300576 nostr_dvm-0.3.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-06 10:19:03.000000 nostr_dvm-0.3.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-05-06 10:19:10.300576 nostr_dvm-0.3.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1563 2024-05-06 10:19:03.000000 nostr_dvm-0.3.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 10:19:10.284576 nostr_dvm-0.3.5/nostr_dvm/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 10:19:03.000000 nostr_dvm-0.3.5/nostr_dvm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 10:19:10.284576 nostr_dvm-0.3.5/nostr_dvm/backends/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 10:19:03.000000 nostr_dvm-0.3.5/nostr_dvm/backends/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 10:19:10.284576 nostr_dvm-0.3.5/nostr_dvm/backends/mlx/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 10:19:03.000000 nostr_dvm-0.3.5/nostr_dvm/backends/mlx/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 10:19:10.284576 nostr_dvm-0.3.5/nostr_dvm/backends/mlx/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 10:19:03.000000 nostr_dvm-0.3.5/nostr_dvm/backends/mlx/modules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 10:19:10.288576 nostr_dvm-0.3.5/nostr_dvm/backends/mlx/modules/stable_diffusion/
+-rw-r--r--   0 runner    (1001) docker     (127)     2945 2024-05-06 10:19:03.000000 nostr_dvm-0.3.5/nostr_dvm/backends/mlx/modules/stable_diffusion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2222 2024-05-06 10:19:03.000000 nostr_dvm-0.3.5/nostr_dvm/backends/mlx/modules/stable_diffusion/clip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-05-06 10:19:03.000000 nostr_dvm-0.3.5/nostr_dvm/backends/mlx/modules/stable_diffusion/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9892 2024-05-06 10:19:03.000000 nostr_dvm-0.3.5/nostr_dvm/backends/mlx/modules/stable_diffusion/model_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2300 2024-05-06 10:19:03.000000 nostr_dvm-0.3.5/nostr_dvm/backends/mlx/modules/stable_diffusion/sampler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2991 2024-05-06 10:19:03.000000 nostr_dvm-0.3.5/nostr_dvm/backends/mlx/modules/stable_diffusion/tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13685 2024-05-06 10:19:03.000000 nostr_dvm-0.3.5/nostr_dvm/backends/mlx/modules/stable_diffusion/unet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7773 2024-05-06 10:19:03.000000 nostr_dvm-0.3.5/nostr_dvm/backends/mlx/modules/stable_diffusion/vae.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 10:19:10.288576 nostr_dvm-0.3.5/nostr_dvm/backends/nova_server/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 10:19:03.000000 nostr_dvm-0.3.5/nostr_dvm/backends/nova_server/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 10:19:10.288576 nostr_dvm-0.3.5/nostr_dvm/backends/nova_server/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 10:19:03.000000 nostr_dvm-0.3.5/nostr_dvm/backends/nova_server/modules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 10:19:10.288576 nostr_dvm-0.3.5/nostr_dvm/backends/nova_server/modules/image_interrogator/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 10:19:03.000000 nostr_dvm-0.3.5/nostr_dvm/backends/nova_server/modules/image_interrogator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4906 2024-05-06 10:19:03.000000 nostr_dvm-0.3.5/nostr_dvm/backends/nova_server/modules/image_interrogator/image_interrogator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-05-06 10:19:03.000000 nostr_dvm-0.3.5/nostr_dvm/backends/nova_server/modules/image_interrogator/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 10:19:10.288576 nostr_dvm-0.3.5/nostr_dvm/backends/nova_server/modules/image_upscale/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 10:19:03.000000 nostr_dvm-0.3.5/nostr_dvm/backends/nova_server/modules/image_upscale/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6863 2024-05-06 10:19:03.000000 nostr_dvm-0.3.5/nostr_dvm/backends/nova_server/modules/image_upscale/image_upscale_realesrgan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7745 2024-05-06 10:19:03.000000 nostr_dvm-0.3.5/nostr_dvm/backends/nova_server/modules/image_upscale/inference_realesrgan.py
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-06 10:19:03.000000 nostr_dvm-0.3.5/nostr_dvm/backends/nova_server/modules/image_upscale/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 10:19:10.288576 nostr_dvm-0.3.5/nostr_dvm/backends/nova_server/modules/stablediffusionxl/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 10:19:03.000000 nostr_dvm-0.3.5/nostr_dvm/backends/nova_server/modules/stablediffusionxl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3319 2024-05-06 10:19:03.000000 nostr_dvm-0.3.5/nostr_dvm/backends/nova_server/modules/stablediffusionxl/lora.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6854 2024-05-06 10:19:03.000000 nostr_dvm-0.3.5/nostr_dvm/backends/nova_server/modules/stablediffusionxl/stablediffusionxl-img2img.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9229 2024-05-06 10:19:03.000000 nostr_dvm-0.3.5/nostr_dvm/backends/nova_server/modules/stablediffusionxl/stablediffusionxl.py
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-06 10:19:03.000000 nostr_dvm-0.3.5/nostr_dvm/backends/nova_server/modules/stablediffusionxl/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 10:19:10.288576 nostr_dvm-0.3.5/nostr_dvm/backends/nova_server/modules/whisperx/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 10:19:03.000000 nostr_dvm-0.3.5/nostr_dvm/backends/nova_server/modules/whisperx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-05-06 10:19:03.000000 nostr_dvm-0.3.5/nostr_dvm/backends/nova_server/modules/whisperx/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5250 2024-05-06 10:19:03.000000 nostr_dvm-0.3.5/nostr_dvm/backends/nova_server/modules/whisperx/whisperx_transcript.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4880 2024-05-06 10:19:03.000000 nostr_dvm-0.3.5/nostr_dvm/backends/nova_server/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39816 2024-05-06 10:19:03.000000 nostr_dvm-0.3.5/nostr_dvm/bot.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39377 2024-05-06 10:19:03.000000 nostr_dvm-0.3.5/nostr_dvm/dvm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 10:19:10.292576 nostr_dvm-0.3.5/nostr_dvm/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 10:19:03.000000 nostr_dvm-0.3.5/nostr_dvm/interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6126 2024-05-06 10:19:03.000000 nostr_dvm-0.3.5/nostr_dvm/interfaces/dvmtaskinterface.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23351 2024-05-06 10:19:03.000000 nostr_dvm-0.3.5/nostr_dvm/subscription.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 10:19:10.296576 nostr_dvm-0.3.5/nostr_dvm/tasks/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 10:19:03.000000 nostr_dvm-0.3.5/nostr_dvm/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8321 2024-05-06 10:19:03.000000 nostr_dvm-0.3.5/nostr_dvm/tasks/advanced_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7452 2024-05-06 10:19:03.000000 nostr_dvm-0.3.5/nostr_dvm/tasks/advanced_search_wine.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11255 2024-05-06 10:19:03.000000 nostr_dvm-0.3.5/nostr_dvm/tasks/content_discovery_currently_popular.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12843 2024-05-06 10:19:03.000000 nostr_dvm-0.3.5/nostr_dvm/tasks/content_discovery_currently_popular_followers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4049 2024-05-06 10:19:03.000000 nostr_dvm-0.3.5/nostr_dvm/tasks/convert_media.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7851 2024-05-06 10:19:03.000000 nostr_dvm-0.3.5/nostr_dvm/tasks/discovery_bot_farms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8189 2024-05-06 10:19:03.000000 nostr_dvm-0.3.5/nostr_dvm/tasks/discovery_censor_wot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8964 2024-05-06 10:19:03.000000 nostr_dvm-0.3.5/nostr_dvm/tasks/discovery_inactive_follows.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8995 2024-05-06 10:19:03.000000 nostr_dvm-0.3.5/nostr_dvm/tasks/discovery_nonfollowers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4473 2024-05-06 10:19:03.000000 nostr_dvm-0.3.5/nostr_dvm/tasks/discovery_trending_notes_nostrband.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6218 2024-05-06 10:19:03.000000 nostr_dvm-0.3.5/nostr_dvm/tasks/imagegeneration_openai_dalle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5968 2024-05-06 10:19:03.000000 nostr_dvm-0.3.5/nostr_dvm/tasks/imagegeneration_replicate_sdxl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6897 2024-05-06 10:19:03.000000 nostr_dvm-0.3.5/nostr_dvm/tasks/imagegeneration_sd21_mlx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8391 2024-05-06 10:19:03.000000 nostr_dvm-0.3.5/nostr_dvm/tasks/imagegeneration_sdxl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9045 2024-05-06 10:19:03.000000 nostr_dvm-0.3.5/nostr_dvm/tasks/imagegeneration_sdxlimg2img.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5281 2024-05-06 10:19:03.000000 nostr_dvm-0.3.5/nostr_dvm/tasks/imageinterrogator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5283 2024-05-06 10:19:03.000000 nostr_dvm-0.3.5/nostr_dvm/tasks/imageupscale.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8169 2024-05-06 10:19:03.000000 nostr_dvm-0.3.5/nostr_dvm/tasks/search_users.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6450 2024-05-06 10:19:03.000000 nostr_dvm-0.3.5/nostr_dvm/tasks/summarization_huggingchat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6945 2024-05-06 10:19:03.000000 nostr_dvm-0.3.5/nostr_dvm/tasks/summarization_unleashed_chat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6774 2024-05-06 10:19:03.000000 nostr_dvm-0.3.5/nostr_dvm/tasks/textextraction_google.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4514 2024-05-06 10:19:03.000000 nostr_dvm-0.3.5/nostr_dvm/tasks/textextraction_pdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7781 2024-05-06 10:19:03.000000 nostr_dvm-0.3.5/nostr_dvm/tasks/textextraction_whisperx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4320 2024-05-06 10:19:03.000000 nostr_dvm-0.3.5/nostr_dvm/tasks/textgeneration_huggingchat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4985 2024-05-06 10:19:03.000000 nostr_dvm-0.3.5/nostr_dvm/tasks/textgeneration_llmlite.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4664 2024-05-06 10:19:03.000000 nostr_dvm-0.3.5/nostr_dvm/tasks/textgeneration_unleashed_chat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6897 2024-05-06 10:19:03.000000 nostr_dvm-0.3.5/nostr_dvm/tasks/texttospeech.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7004 2024-05-06 10:19:03.000000 nostr_dvm-0.3.5/nostr_dvm/tasks/translation_google.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6895 2024-05-06 10:19:03.000000 nostr_dvm-0.3.5/nostr_dvm/tasks/translation_libretranslate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5571 2024-05-06 10:19:03.000000 nostr_dvm-0.3.5/nostr_dvm/tasks/videogeneration_replicate_svd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4892 2024-05-06 10:19:03.000000 nostr_dvm-0.3.5/nostr_dvm/tasks/videogeneration_svd.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 10:19:10.296576 nostr_dvm-0.3.5/nostr_dvm/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 10:19:03.000000 nostr_dvm-0.3.5/nostr_dvm/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4334 2024-05-06 10:19:03.000000 nostr_dvm-0.3.5/nostr_dvm/utils/admin_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8745 2024-05-06 10:19:03.000000 nostr_dvm-0.3.5/nostr_dvm/utils/backend_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6163 2024-05-06 10:19:03.000000 nostr_dvm-0.3.5/nostr_dvm/utils/cashu_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9473 2024-05-06 10:19:03.000000 nostr_dvm-0.3.5/nostr_dvm/utils/database_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2700 2024-05-06 10:19:03.000000 nostr_dvm-0.3.5/nostr_dvm/utils/definitions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2387 2024-05-06 10:19:03.000000 nostr_dvm-0.3.5/nostr_dvm/utils/dvmconfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2761 2024-05-06 10:19:03.000000 nostr_dvm-0.3.5/nostr_dvm/utils/external_dvm_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13403 2024-05-06 10:19:03.000000 nostr_dvm-0.3.5/nostr_dvm/utils/mediasource_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8866 2024-05-06 10:19:03.000000 nostr_dvm-0.3.5/nostr_dvm/utils/nip88_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4170 2024-05-06 10:19:03.000000 nostr_dvm-0.3.5/nostr_dvm/utils/nip89_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8449 2024-05-06 10:19:03.000000 nostr_dvm-0.3.5/nostr_dvm/utils/nostr_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3795 2024-05-06 10:19:03.000000 nostr_dvm-0.3.5/nostr_dvm/utils/nwc_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9011 2024-05-06 10:19:03.000000 nostr_dvm-0.3.5/nostr_dvm/utils/output_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 10:19:10.300576 nostr_dvm-0.3.5/nostr_dvm/utils/scrapper/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 10:19:03.000000 nostr_dvm-0.3.5/nostr_dvm/utils/scrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26119 2024-05-06 10:19:03.000000 nostr_dvm-0.3.5/nostr_dvm/utils/scrapper/media_scrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5712 2024-05-06 10:19:03.000000 nostr_dvm-0.3.5/nostr_dvm/utils/subscription_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15021 2024-05-06 10:19:03.000000 nostr_dvm-0.3.5/nostr_dvm/utils/zap_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 10:19:10.300576 nostr_dvm-0.3.5/nostr_dvm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-05-06 10:19:10.000000 nostr_dvm-0.3.5/nostr_dvm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4118 2024-05-06 10:19:10.000000 nostr_dvm-0.3.5/nostr_dvm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 10:19:10.000000 nostr_dvm-0.3.5/nostr_dvm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-05-06 10:19:10.000000 nostr_dvm-0.3.5/nostr_dvm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-06 10:19:10.000000 nostr_dvm-0.3.5/nostr_dvm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 10:19:10.300576 nostr_dvm-0.3.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-05-06 10:19:03.000000 nostr_dvm-0.3.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 10:19:10.300576 nostr_dvm-0.3.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    12655 2024-05-06 10:19:03.000000 nostr_dvm-0.3.5/tests/test_dvm_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3213 2024-05-06 10:19:03.000000 nostr_dvm-0.3.5/tests/test_events.py
```

### Comparing `nostr_dvm-0.3.4/LICENSE` & `nostr_dvm-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.4/PKG-INFO` & `nostr_dvm-0.3.5/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nostr-dvm
-Version: 0.3.4
+Version: 0.3.5
 Summary: A framework to build and run Nostr NIP90 Data Vending Machines
 Home-page: https://github.com/believethehype/nostrdvm
 Author: Believethehype
 Author-email: believethehypeonnostr@proton.me
 License: MIT
 Keywords: nostr,nip90,dvm,data vending machine
 Classifier: Development Status :: 3 - Alpha
@@ -26,8 +26,8 @@
 Requires-Dist: instaloader==4.10.1
 Requires-Dist: pytube==15.0.0
 Requires-Dist: moviepy==2.0.0.dev2
 Requires-Dist: zipp==3.17.0
 Requires-Dist: urllib3==2.1.0
 Requires-Dist: typing_extensions>=4.9.0
 
-A framework to build and run Nostr NIP90 Data Vending Machines. This is an early stage release. Interfaces might change/brick
+A framework to build and run Nostr NIP90 Data Vending Machines. See the github repository for more information
```

### Comparing `nostr_dvm-0.3.4/README.md` & `nostr_dvm-0.3.5/README.md`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.4/nostr_dvm/backends/mlx/modules/stable_diffusion/__init__.py` & `nostr_dvm-0.3.5/nostr_dvm/backends/mlx/modules/stable_diffusion/__init__.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.4/nostr_dvm/backends/mlx/modules/stable_diffusion/clip.py` & `nostr_dvm-0.3.5/nostr_dvm/backends/mlx/modules/stable_diffusion/clip.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.4/nostr_dvm/backends/mlx/modules/stable_diffusion/config.py` & `nostr_dvm-0.3.5/nostr_dvm/backends/mlx/modules/stable_diffusion/config.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.4/nostr_dvm/backends/mlx/modules/stable_diffusion/model_io.py` & `nostr_dvm-0.3.5/nostr_dvm/backends/mlx/modules/stable_diffusion/model_io.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.4/nostr_dvm/backends/mlx/modules/stable_diffusion/sampler.py` & `nostr_dvm-0.3.5/nostr_dvm/backends/mlx/modules/stable_diffusion/sampler.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.4/nostr_dvm/backends/mlx/modules/stable_diffusion/tokenizer.py` & `nostr_dvm-0.3.5/nostr_dvm/backends/mlx/modules/stable_diffusion/tokenizer.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.4/nostr_dvm/backends/mlx/modules/stable_diffusion/unet.py` & `nostr_dvm-0.3.5/nostr_dvm/backends/mlx/modules/stable_diffusion/unet.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.4/nostr_dvm/backends/mlx/modules/stable_diffusion/vae.py` & `nostr_dvm-0.3.5/nostr_dvm/backends/mlx/modules/stable_diffusion/vae.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.4/nostr_dvm/backends/nova_server/modules/image_interrogator/image_interrogator.py` & `nostr_dvm-0.3.5/nostr_dvm/backends/nova_server/modules/image_interrogator/image_interrogator.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.4/nostr_dvm/backends/nova_server/modules/image_upscale/image_upscale_realesrgan.py` & `nostr_dvm-0.3.5/nostr_dvm/backends/nova_server/modules/image_upscale/image_upscale_realesrgan.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.4/nostr_dvm/backends/nova_server/modules/image_upscale/inference_realesrgan.py` & `nostr_dvm-0.3.5/nostr_dvm/backends/nova_server/modules/image_upscale/inference_realesrgan.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.4/nostr_dvm/backends/nova_server/modules/stablediffusionxl/lora.py` & `nostr_dvm-0.3.5/nostr_dvm/backends/nova_server/modules/stablediffusionxl/lora.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.4/nostr_dvm/backends/nova_server/modules/stablediffusionxl/stablediffusionxl-img2img.py` & `nostr_dvm-0.3.5/nostr_dvm/backends/nova_server/modules/stablediffusionxl/stablediffusionxl-img2img.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.4/nostr_dvm/backends/nova_server/modules/stablediffusionxl/stablediffusionxl.py` & `nostr_dvm-0.3.5/nostr_dvm/backends/nova_server/modules/stablediffusionxl/stablediffusionxl.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.4/nostr_dvm/backends/nova_server/modules/whisperx/whisperx_transcript.py` & `nostr_dvm-0.3.5/nostr_dvm/backends/nova_server/modules/whisperx/whisperx_transcript.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.4/nostr_dvm/backends/nova_server/utils.py` & `nostr_dvm-0.3.5/nostr_dvm/backends/nova_server/utils.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.4/nostr_dvm/bot.py` & `nostr_dvm-0.3.5/nostr_dvm/bot.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.4/nostr_dvm/dvm.py` & `nostr_dvm-0.3.5/nostr_dvm/dvm.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.4/nostr_dvm/interfaces/dvmtaskinterface.py` & `nostr_dvm-0.3.5/nostr_dvm/interfaces/dvmtaskinterface.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.4/nostr_dvm/subscription.py` & `nostr_dvm-0.3.5/nostr_dvm/subscription.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.4/nostr_dvm/tasks/advanced_search.py` & `nostr_dvm-0.3.5/nostr_dvm/tasks/advanced_search.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.4/nostr_dvm/tasks/advanced_search_wine.py` & `nostr_dvm-0.3.5/nostr_dvm/tasks/advanced_search_wine.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.4/nostr_dvm/tasks/content_discovery_currently_popular.py` & `nostr_dvm-0.3.5/nostr_dvm/tasks/content_discovery_currently_popular.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.4/nostr_dvm/tasks/content_discovery_currently_popular_followers.py` & `nostr_dvm-0.3.5/nostr_dvm/tasks/content_discovery_currently_popular_followers.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.4/nostr_dvm/tasks/convert_media.py` & `nostr_dvm-0.3.5/nostr_dvm/tasks/convert_media.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.4/nostr_dvm/tasks/discovery_bot_farms.py` & `nostr_dvm-0.3.5/nostr_dvm/tasks/discovery_bot_farms.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,15 +51,15 @@
     def create_request_from_nostr_event(self, event, client=None, dvm_config=None):
         self.dvm_config = dvm_config
         print(self.dvm_config.PRIVATE_KEY)
 
         request_form = {"jobID": event.id().to_hex()}
 
         # default values
-        search = "@nostrich.house;Optimism Airdrop"
+        search = "airdrop;@nostrich.house;just your average nostr enjoyer"
         max_results = 500
 
         for tag in event.tags():
             if tag.as_vec()[0] == 'i':
                 input_type = tag.as_vec()[2]
                 if input_type == "text":
                     search = tag.as_vec()[1]
@@ -149,14 +149,15 @@
         sk = SecretKey.from_hex(self.dvm_config.PRIVATE_KEY)
         keys = Keys.parse(sk.to_hex())
         signer = NostrSigner.keys(keys)
         database = NostrDatabase.sqlite("db/nostr_profiles.db")
         cli = ClientBuilder().signer(signer).database(database).opts(opts).build()
 
         cli.add_relay("wss://relay.damus.io")
+        cli.add_relay("wss://nostr21.com")
         cli.connect()
 
         filter1 = Filter().kind(Kind(0))
 
         # filter = Filter().author(keys.public_key())
         print("Syncing Profile Database.. this might take a while..")
         dbopts = NegentropyOptions().direction(NegentropyDirection.DOWN)
```

### Comparing `nostr_dvm-0.3.4/nostr_dvm/tasks/discovery_censor_wot.py` & `nostr_dvm-0.3.5/nostr_dvm/tasks/discovery_censor_wot.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,14 +53,16 @@
         for tag in event.tags():
             if tag.as_vec()[0] == 'i':
                 users.append(tag.as_vec()[1])
             elif tag.as_vec()[0] == 'param':
                 param = tag.as_vec()[1]
                 if param == "since_days":  # check for param type
                     since_days = int(tag.as_vec()[2])
+                if param == "user":  # check for param type
+                    sender = tag.as_vec()[2]
 
         options = {
             "users": users,
             "sender": sender,
             "since_days": since_days,
         }
         request_form['options'] = json.dumps(options)
```

### Comparing `nostr_dvm-0.3.4/nostr_dvm/tasks/discovery_inactive_follows.py` & `nostr_dvm-0.3.5/nostr_dvm/tasks/discovery_inactive_follows.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.4/nostr_dvm/tasks/discovery_nonfollowers.py` & `nostr_dvm-0.3.5/nostr_dvm/tasks/discovery_nonfollowers.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.4/nostr_dvm/tasks/discovery_trending_notes_nostrband.py` & `nostr_dvm-0.3.5/nostr_dvm/tasks/discovery_trending_notes_nostrband.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.4/nostr_dvm/tasks/imagegeneration_openai_dalle.py` & `nostr_dvm-0.3.5/nostr_dvm/tasks/imagegeneration_openai_dalle.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.4/nostr_dvm/tasks/imagegeneration_replicate_sdxl.py` & `nostr_dvm-0.3.5/nostr_dvm/tasks/imagegeneration_replicate_sdxl.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.4/nostr_dvm/tasks/imagegeneration_sd21_mlx.py` & `nostr_dvm-0.3.5/nostr_dvm/tasks/imagegeneration_sd21_mlx.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.4/nostr_dvm/tasks/imagegeneration_sdxl.py` & `nostr_dvm-0.3.5/nostr_dvm/tasks/imagegeneration_sdxl.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.4/nostr_dvm/tasks/imagegeneration_sdxlimg2img.py` & `nostr_dvm-0.3.5/nostr_dvm/tasks/imagegeneration_sdxlimg2img.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.4/nostr_dvm/tasks/imageinterrogator.py` & `nostr_dvm-0.3.5/nostr_dvm/tasks/imageinterrogator.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.4/nostr_dvm/tasks/imageupscale.py` & `nostr_dvm-0.3.5/nostr_dvm/tasks/imageupscale.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.4/nostr_dvm/tasks/search_users.py` & `nostr_dvm-0.3.5/nostr_dvm/tasks/search_users.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.4/nostr_dvm/tasks/summarization_huggingchat.py` & `nostr_dvm-0.3.5/nostr_dvm/tasks/summarization_huggingchat.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.4/nostr_dvm/tasks/summarization_unleashed_chat.py` & `nostr_dvm-0.3.5/nostr_dvm/tasks/summarization_unleashed_chat.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.4/nostr_dvm/tasks/textextraction_google.py` & `nostr_dvm-0.3.5/nostr_dvm/tasks/textextraction_google.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.4/nostr_dvm/tasks/textextraction_pdf.py` & `nostr_dvm-0.3.5/nostr_dvm/tasks/textextraction_pdf.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.4/nostr_dvm/tasks/textextraction_whisperx.py` & `nostr_dvm-0.3.5/nostr_dvm/tasks/textextraction_whisperx.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.4/nostr_dvm/tasks/textgeneration_huggingchat.py` & `nostr_dvm-0.3.5/nostr_dvm/tasks/textgeneration_huggingchat.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.4/nostr_dvm/tasks/textgeneration_llmlite.py` & `nostr_dvm-0.3.5/nostr_dvm/tasks/textgeneration_llmlite.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.4/nostr_dvm/tasks/textgeneration_unleashed_chat.py` & `nostr_dvm-0.3.5/nostr_dvm/tasks/textgeneration_unleashed_chat.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.4/nostr_dvm/tasks/texttospeech.py` & `nostr_dvm-0.3.5/nostr_dvm/tasks/texttospeech.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.4/nostr_dvm/tasks/translation_google.py` & `nostr_dvm-0.3.5/nostr_dvm/tasks/translation_google.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.4/nostr_dvm/tasks/translation_libretranslate.py` & `nostr_dvm-0.3.5/nostr_dvm/tasks/translation_libretranslate.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.4/nostr_dvm/tasks/videogeneration_replicate_svd.py` & `nostr_dvm-0.3.5/nostr_dvm/tasks/videogeneration_replicate_svd.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.4/nostr_dvm/tasks/videogeneration_svd.py` & `nostr_dvm-0.3.5/nostr_dvm/tasks/videogeneration_svd.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.4/nostr_dvm/utils/admin_utils.py` & `nostr_dvm-0.3.5/nostr_dvm/utils/admin_utils.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.4/nostr_dvm/utils/backend_utils.py` & `nostr_dvm-0.3.5/nostr_dvm/utils/backend_utils.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.4/nostr_dvm/utils/cashu_utils.py` & `nostr_dvm-0.3.5/nostr_dvm/utils/cashu_utils.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.4/nostr_dvm/utils/database_utils.py` & `nostr_dvm-0.3.5/nostr_dvm/utils/database_utils.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.4/nostr_dvm/utils/definitions.py` & `nostr_dvm-0.3.5/nostr_dvm/utils/definitions.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.4/nostr_dvm/utils/dvmconfig.py` & `nostr_dvm-0.3.5/nostr_dvm/utils/dvmconfig.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.4/nostr_dvm/utils/external_dvm_utils.py` & `nostr_dvm-0.3.5/nostr_dvm/utils/external_dvm_utils.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.4/nostr_dvm/utils/mediasource_utils.py` & `nostr_dvm-0.3.5/nostr_dvm/utils/mediasource_utils.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.4/nostr_dvm/utils/nip88_utils.py` & `nostr_dvm-0.3.5/nostr_dvm/utils/nip88_utils.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.4/nostr_dvm/utils/nip89_utils.py` & `nostr_dvm-0.3.5/nostr_dvm/utils/nip89_utils.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.4/nostr_dvm/utils/nostr_utils.py` & `nostr_dvm-0.3.5/nostr_dvm/utils/nostr_utils.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.4/nostr_dvm/utils/nwc_tools.py` & `nostr_dvm-0.3.5/nostr_dvm/utils/nwc_tools.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.4/nostr_dvm/utils/output_utils.py` & `nostr_dvm-0.3.5/nostr_dvm/utils/output_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -109,15 +109,15 @@
 def post_process_list_to_users(result):
     result_list = json.loads(result)
     result_str = ""
     if len(result_list) == 0:
         return "No results found"
     for tag in result_list:
         p_tag = Tag.parse(tag)
-        result_str = result_str + "nostr:" + PublicKey.from_hex(
+        result_str = result_str + "nostr:" + PublicKey.parse(
             p_tag.as_vec()[1]).to_bech32() + "\n"
     return result_str
 
 
 def pandas_to_plaintext(anno):
     result = ""
     for each_row in anno['name']:
```

### Comparing `nostr_dvm-0.3.4/nostr_dvm/utils/scrapper/media_scrapper.py` & `nostr_dvm-0.3.5/nostr_dvm/utils/scrapper/media_scrapper.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.4/nostr_dvm/utils/subscription_utils.py` & `nostr_dvm-0.3.5/nostr_dvm/utils/subscription_utils.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.4/nostr_dvm/utils/zap_utils.py` & `nostr_dvm-0.3.5/nostr_dvm/utils/zap_utils.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.4/nostr_dvm.egg-info/PKG-INFO` & `nostr_dvm-0.3.5/nostr_dvm.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nostr-dvm
-Version: 0.3.4
+Version: 0.3.5
 Summary: A framework to build and run Nostr NIP90 Data Vending Machines
 Home-page: https://github.com/believethehype/nostrdvm
 Author: Believethehype
 Author-email: believethehypeonnostr@proton.me
 License: MIT
 Keywords: nostr,nip90,dvm,data vending machine
 Classifier: Development Status :: 3 - Alpha
@@ -26,8 +26,8 @@
 Requires-Dist: instaloader==4.10.1
 Requires-Dist: pytube==15.0.0
 Requires-Dist: moviepy==2.0.0.dev2
 Requires-Dist: zipp==3.17.0
 Requires-Dist: urllib3==2.1.0
 Requires-Dist: typing_extensions>=4.9.0
 
-A framework to build and run Nostr NIP90 Data Vending Machines. This is an early stage release. Interfaces might change/brick
+A framework to build and run Nostr NIP90 Data Vending Machines. See the github repository for more information
```

### Comparing `nostr_dvm-0.3.4/nostr_dvm.egg-info/SOURCES.txt` & `nostr_dvm-0.3.5/nostr_dvm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.4/setup.py` & `nostr_dvm-0.3.5/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.3.4'
+VERSION = '0.3.5'
 DESCRIPTION = 'A framework to build and run Nostr NIP90 Data Vending Machines'
-LONG_DESCRIPTION = ('A framework to build and run Nostr NIP90 Data Vending Machines. '
-                    'This is an early stage release. Interfaces might change/brick')
+LONG_DESCRIPTION = ('A framework to build and run Nostr NIP90 Data Vending Machines. See the github repository for more information')
 
 # Setting up
 setup(
     name="nostr-dvm",
     version=VERSION,
     author="Believethehype",
     author_email="believethehypeonnostr@proton.me",
```

### Comparing `nostr_dvm-0.3.4/tests/test_dvm_client.py` & `nostr_dvm-0.3.5/tests/test_dvm_client.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.4/tests/test_events.py` & `nostr_dvm-0.3.5/tests/test_events.py`

 * *Files identical despite different names*

