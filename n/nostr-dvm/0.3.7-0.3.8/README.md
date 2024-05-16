# Comparing `tmp/nostr_dvm-0.3.7.tar.gz` & `tmp/nostr_dvm-0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nostr_dvm-0.3.7.tar", last modified: Thu May 16 08:51:59 2024, max compression
+gzip compressed data, was "nostr_dvm-0.3.8.tar", last modified: Thu May 16 09:58:38 2024, max compression
```

## Comparing `nostr_dvm-0.3.7.tar` & `nostr_dvm-0.3.8.tar`

### file list

```diff
@@ -1,116 +1,116 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 08:51:59.012030 nostr_dvm-0.3.7/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-16 08:51:54.000000 nostr_dvm-0.3.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-05-16 08:51:59.012030 nostr_dvm-0.3.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-05-16 08:51:54.000000 nostr_dvm-0.3.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 08:51:58.996030 nostr_dvm-0.3.7/nostr_dvm/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 08:51:54.000000 nostr_dvm-0.3.7/nostr_dvm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 08:51:59.000030 nostr_dvm-0.3.7/nostr_dvm/backends/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 08:51:54.000000 nostr_dvm-0.3.7/nostr_dvm/backends/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 08:51:59.000030 nostr_dvm-0.3.7/nostr_dvm/backends/mlx/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 08:51:54.000000 nostr_dvm-0.3.7/nostr_dvm/backends/mlx/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 08:51:59.000030 nostr_dvm-0.3.7/nostr_dvm/backends/mlx/modules/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 08:51:54.000000 nostr_dvm-0.3.7/nostr_dvm/backends/mlx/modules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 08:51:59.000030 nostr_dvm-0.3.7/nostr_dvm/backends/mlx/modules/stable_diffusion/
--rw-r--r--   0 runner    (1001) docker     (127)     2945 2024-05-16 08:51:54.000000 nostr_dvm-0.3.7/nostr_dvm/backends/mlx/modules/stable_diffusion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2222 2024-05-16 08:51:54.000000 nostr_dvm-0.3.7/nostr_dvm/backends/mlx/modules/stable_diffusion/clip.py
--rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-05-16 08:51:54.000000 nostr_dvm-0.3.7/nostr_dvm/backends/mlx/modules/stable_diffusion/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     9892 2024-05-16 08:51:54.000000 nostr_dvm-0.3.7/nostr_dvm/backends/mlx/modules/stable_diffusion/model_io.py
--rw-r--r--   0 runner    (1001) docker     (127)     2300 2024-05-16 08:51:54.000000 nostr_dvm-0.3.7/nostr_dvm/backends/mlx/modules/stable_diffusion/sampler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2991 2024-05-16 08:51:54.000000 nostr_dvm-0.3.7/nostr_dvm/backends/mlx/modules/stable_diffusion/tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (127)    13685 2024-05-16 08:51:54.000000 nostr_dvm-0.3.7/nostr_dvm/backends/mlx/modules/stable_diffusion/unet.py
--rw-r--r--   0 runner    (1001) docker     (127)     7773 2024-05-16 08:51:54.000000 nostr_dvm-0.3.7/nostr_dvm/backends/mlx/modules/stable_diffusion/vae.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 08:51:59.000030 nostr_dvm-0.3.7/nostr_dvm/backends/nova_server/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 08:51:54.000000 nostr_dvm-0.3.7/nostr_dvm/backends/nova_server/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 08:51:59.000030 nostr_dvm-0.3.7/nostr_dvm/backends/nova_server/modules/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 08:51:54.000000 nostr_dvm-0.3.7/nostr_dvm/backends/nova_server/modules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 08:51:59.000030 nostr_dvm-0.3.7/nostr_dvm/backends/nova_server/modules/image_interrogator/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 08:51:54.000000 nostr_dvm-0.3.7/nostr_dvm/backends/nova_server/modules/image_interrogator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4906 2024-05-16 08:51:54.000000 nostr_dvm-0.3.7/nostr_dvm/backends/nova_server/modules/image_interrogator/image_interrogator.py
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-05-16 08:51:54.000000 nostr_dvm-0.3.7/nostr_dvm/backends/nova_server/modules/image_interrogator/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 08:51:59.000030 nostr_dvm-0.3.7/nostr_dvm/backends/nova_server/modules/image_upscale/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 08:51:54.000000 nostr_dvm-0.3.7/nostr_dvm/backends/nova_server/modules/image_upscale/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6863 2024-05-16 08:51:54.000000 nostr_dvm-0.3.7/nostr_dvm/backends/nova_server/modules/image_upscale/image_upscale_realesrgan.py
--rw-r--r--   0 runner    (1001) docker     (127)     7745 2024-05-16 08:51:54.000000 nostr_dvm-0.3.7/nostr_dvm/backends/nova_server/modules/image_upscale/inference_realesrgan.py
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-16 08:51:54.000000 nostr_dvm-0.3.7/nostr_dvm/backends/nova_server/modules/image_upscale/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 08:51:59.004030 nostr_dvm-0.3.7/nostr_dvm/backends/nova_server/modules/stablediffusionxl/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 08:51:54.000000 nostr_dvm-0.3.7/nostr_dvm/backends/nova_server/modules/stablediffusionxl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3319 2024-05-16 08:51:54.000000 nostr_dvm-0.3.7/nostr_dvm/backends/nova_server/modules/stablediffusionxl/lora.py
--rw-r--r--   0 runner    (1001) docker     (127)     6854 2024-05-16 08:51:54.000000 nostr_dvm-0.3.7/nostr_dvm/backends/nova_server/modules/stablediffusionxl/stablediffusionxl-img2img.py
--rw-r--r--   0 runner    (1001) docker     (127)     9229 2024-05-16 08:51:54.000000 nostr_dvm-0.3.7/nostr_dvm/backends/nova_server/modules/stablediffusionxl/stablediffusionxl.py
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-16 08:51:54.000000 nostr_dvm-0.3.7/nostr_dvm/backends/nova_server/modules/stablediffusionxl/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 08:51:59.004030 nostr_dvm-0.3.7/nostr_dvm/backends/nova_server/modules/whisperx/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 08:51:54.000000 nostr_dvm-0.3.7/nostr_dvm/backends/nova_server/modules/whisperx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-05-16 08:51:54.000000 nostr_dvm-0.3.7/nostr_dvm/backends/nova_server/modules/whisperx/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     5250 2024-05-16 08:51:54.000000 nostr_dvm-0.3.7/nostr_dvm/backends/nova_server/modules/whisperx/whisperx_transcript.py
--rw-r--r--   0 runner    (1001) docker     (127)     4880 2024-05-16 08:51:54.000000 nostr_dvm-0.3.7/nostr_dvm/backends/nova_server/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    39902 2024-05-16 08:51:54.000000 nostr_dvm-0.3.7/nostr_dvm/bot.py
--rw-r--r--   0 runner    (1001) docker     (127)    39377 2024-05-16 08:51:54.000000 nostr_dvm-0.3.7/nostr_dvm/dvm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 08:51:59.004030 nostr_dvm-0.3.7/nostr_dvm/interfaces/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 08:51:54.000000 nostr_dvm-0.3.7/nostr_dvm/interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6126 2024-05-16 08:51:54.000000 nostr_dvm-0.3.7/nostr_dvm/interfaces/dvmtaskinterface.py
--rw-r--r--   0 runner    (1001) docker     (127)    23582 2024-05-16 08:51:54.000000 nostr_dvm-0.3.7/nostr_dvm/subscription.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 08:51:59.008030 nostr_dvm-0.3.7/nostr_dvm/tasks/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 08:51:54.000000 nostr_dvm-0.3.7/nostr_dvm/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8321 2024-05-16 08:51:54.000000 nostr_dvm-0.3.7/nostr_dvm/tasks/advanced_search.py
--rw-r--r--   0 runner    (1001) docker     (127)     7452 2024-05-16 08:51:54.000000 nostr_dvm-0.3.7/nostr_dvm/tasks/advanced_search_wine.py
--rw-r--r--   0 runner    (1001) docker     (127)    12456 2024-05-16 08:51:54.000000 nostr_dvm-0.3.7/nostr_dvm/tasks/content_discovery_currently_popular.py
--rw-r--r--   0 runner    (1001) docker     (127)    13027 2024-05-16 08:51:54.000000 nostr_dvm-0.3.7/nostr_dvm/tasks/content_discovery_currently_popular_followers.py
--rw-r--r--   0 runner    (1001) docker     (127)    13058 2024-05-16 08:51:54.000000 nostr_dvm-0.3.7/nostr_dvm/tasks/content_discovery_currently_popular_topic.py
--rw-r--r--   0 runner    (1001) docker     (127)     4049 2024-05-16 08:51:54.000000 nostr_dvm-0.3.7/nostr_dvm/tasks/convert_media.py
--rw-r--r--   0 runner    (1001) docker     (127)     7854 2024-05-16 08:51:54.000000 nostr_dvm-0.3.7/nostr_dvm/tasks/discovery_bot_farms.py
--rw-r--r--   0 runner    (1001) docker     (127)     8189 2024-05-16 08:51:54.000000 nostr_dvm-0.3.7/nostr_dvm/tasks/discovery_censor_wot.py
--rw-r--r--   0 runner    (1001) docker     (127)     8964 2024-05-16 08:51:54.000000 nostr_dvm-0.3.7/nostr_dvm/tasks/discovery_inactive_follows.py
--rw-r--r--   0 runner    (1001) docker     (127)     8995 2024-05-16 08:51:54.000000 nostr_dvm-0.3.7/nostr_dvm/tasks/discovery_nonfollowers.py
--rw-r--r--   0 runner    (1001) docker     (127)     4474 2024-05-16 08:51:54.000000 nostr_dvm-0.3.7/nostr_dvm/tasks/discovery_trending_notes_nostrband.py
--rw-r--r--   0 runner    (1001) docker     (127)     6218 2024-05-16 08:51:54.000000 nostr_dvm-0.3.7/nostr_dvm/tasks/imagegeneration_openai_dalle.py
--rw-r--r--   0 runner    (1001) docker     (127)     5968 2024-05-16 08:51:54.000000 nostr_dvm-0.3.7/nostr_dvm/tasks/imagegeneration_replicate_sdxl.py
--rw-r--r--   0 runner    (1001) docker     (127)     6897 2024-05-16 08:51:54.000000 nostr_dvm-0.3.7/nostr_dvm/tasks/imagegeneration_sd21_mlx.py
--rw-r--r--   0 runner    (1001) docker     (127)     8391 2024-05-16 08:51:54.000000 nostr_dvm-0.3.7/nostr_dvm/tasks/imagegeneration_sdxl.py
--rw-r--r--   0 runner    (1001) docker     (127)     9045 2024-05-16 08:51:54.000000 nostr_dvm-0.3.7/nostr_dvm/tasks/imagegeneration_sdxlimg2img.py
--rw-r--r--   0 runner    (1001) docker     (127)     5281 2024-05-16 08:51:54.000000 nostr_dvm-0.3.7/nostr_dvm/tasks/imageinterrogator.py
--rw-r--r--   0 runner    (1001) docker     (127)     5283 2024-05-16 08:51:54.000000 nostr_dvm-0.3.7/nostr_dvm/tasks/imageupscale.py
--rw-r--r--   0 runner    (1001) docker     (127)     8186 2024-05-16 08:51:54.000000 nostr_dvm-0.3.7/nostr_dvm/tasks/search_users.py
--rw-r--r--   0 runner    (1001) docker     (127)     6450 2024-05-16 08:51:54.000000 nostr_dvm-0.3.7/nostr_dvm/tasks/summarization_huggingchat.py
--rw-r--r--   0 runner    (1001) docker     (127)     6945 2024-05-16 08:51:54.000000 nostr_dvm-0.3.7/nostr_dvm/tasks/summarization_unleashed_chat.py
--rw-r--r--   0 runner    (1001) docker     (127)     6774 2024-05-16 08:51:54.000000 nostr_dvm-0.3.7/nostr_dvm/tasks/textextraction_google.py
--rw-r--r--   0 runner    (1001) docker     (127)     4514 2024-05-16 08:51:54.000000 nostr_dvm-0.3.7/nostr_dvm/tasks/textextraction_pdf.py
--rw-r--r--   0 runner    (1001) docker     (127)     7781 2024-05-16 08:51:54.000000 nostr_dvm-0.3.7/nostr_dvm/tasks/textextraction_whisperx.py
--rw-r--r--   0 runner    (1001) docker     (127)     4320 2024-05-16 08:51:54.000000 nostr_dvm-0.3.7/nostr_dvm/tasks/textgeneration_huggingchat.py
--rw-r--r--   0 runner    (1001) docker     (127)     4985 2024-05-16 08:51:54.000000 nostr_dvm-0.3.7/nostr_dvm/tasks/textgeneration_llmlite.py
--rw-r--r--   0 runner    (1001) docker     (127)     4664 2024-05-16 08:51:54.000000 nostr_dvm-0.3.7/nostr_dvm/tasks/textgeneration_unleashed_chat.py
--rw-r--r--   0 runner    (1001) docker     (127)     6897 2024-05-16 08:51:54.000000 nostr_dvm-0.3.7/nostr_dvm/tasks/texttospeech.py
--rw-r--r--   0 runner    (1001) docker     (127)     7004 2024-05-16 08:51:54.000000 nostr_dvm-0.3.7/nostr_dvm/tasks/translation_google.py
--rw-r--r--   0 runner    (1001) docker     (127)     6895 2024-05-16 08:51:54.000000 nostr_dvm-0.3.7/nostr_dvm/tasks/translation_libretranslate.py
--rw-r--r--   0 runner    (1001) docker     (127)     5571 2024-05-16 08:51:54.000000 nostr_dvm-0.3.7/nostr_dvm/tasks/videogeneration_replicate_svd.py
--rw-r--r--   0 runner    (1001) docker     (127)     4892 2024-05-16 08:51:54.000000 nostr_dvm-0.3.7/nostr_dvm/tasks/videogeneration_svd.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 08:51:59.012030 nostr_dvm-0.3.7/nostr_dvm/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 08:51:54.000000 nostr_dvm-0.3.7/nostr_dvm/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4334 2024-05-16 08:51:54.000000 nostr_dvm-0.3.7/nostr_dvm/utils/admin_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8745 2024-05-16 08:51:54.000000 nostr_dvm-0.3.7/nostr_dvm/utils/backend_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6163 2024-05-16 08:51:54.000000 nostr_dvm-0.3.7/nostr_dvm/utils/cashu_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     9473 2024-05-16 08:51:54.000000 nostr_dvm-0.3.7/nostr_dvm/utils/database_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2700 2024-05-16 08:51:54.000000 nostr_dvm-0.3.7/nostr_dvm/utils/definitions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2387 2024-05-16 08:51:54.000000 nostr_dvm-0.3.7/nostr_dvm/utils/dvmconfig.py
--rw-r--r--   0 runner    (1001) docker     (127)     2761 2024-05-16 08:51:54.000000 nostr_dvm-0.3.7/nostr_dvm/utils/external_dvm_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    13403 2024-05-16 08:51:54.000000 nostr_dvm-0.3.7/nostr_dvm/utils/mediasource_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8866 2024-05-16 08:51:54.000000 nostr_dvm-0.3.7/nostr_dvm/utils/nip88_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4170 2024-05-16 08:51:54.000000 nostr_dvm-0.3.7/nostr_dvm/utils/nip89_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8449 2024-05-16 08:51:54.000000 nostr_dvm-0.3.7/nostr_dvm/utils/nostr_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3795 2024-05-16 08:51:54.000000 nostr_dvm-0.3.7/nostr_dvm/utils/nwc_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     9011 2024-05-16 08:51:54.000000 nostr_dvm-0.3.7/nostr_dvm/utils/output_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 08:51:59.012030 nostr_dvm-0.3.7/nostr_dvm/utils/scrapper/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 08:51:54.000000 nostr_dvm-0.3.7/nostr_dvm/utils/scrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    26119 2024-05-16 08:51:54.000000 nostr_dvm-0.3.7/nostr_dvm/utils/scrapper/media_scrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     5712 2024-05-16 08:51:54.000000 nostr_dvm-0.3.7/nostr_dvm/utils/subscription_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    15021 2024-05-16 08:51:54.000000 nostr_dvm-0.3.7/nostr_dvm/utils/zap_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 08:51:59.012030 nostr_dvm-0.3.7/nostr_dvm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-05-16 08:51:58.000000 nostr_dvm-0.3.7/nostr_dvm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4179 2024-05-16 08:51:58.000000 nostr_dvm-0.3.7/nostr_dvm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 08:51:58.000000 nostr_dvm-0.3.7/nostr_dvm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-05-16 08:51:58.000000 nostr_dvm-0.3.7/nostr_dvm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-16 08:51:58.000000 nostr_dvm-0.3.7/nostr_dvm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 08:51:59.012030 nostr_dvm-0.3.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-05-16 08:51:54.000000 nostr_dvm-0.3.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 08:51:59.012030 nostr_dvm-0.3.7/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    13764 2024-05-16 08:51:54.000000 nostr_dvm-0.3.7/tests/test_dvm_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     3213 2024-05-16 08:51:54.000000 nostr_dvm-0.3.7/tests/test_events.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:58:38.766839 nostr_dvm-0.3.8/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-16 09:58:34.000000 nostr_dvm-0.3.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-05-16 09:58:38.766839 nostr_dvm-0.3.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-05-16 09:58:34.000000 nostr_dvm-0.3.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:58:38.750839 nostr_dvm-0.3.8/nostr_dvm/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 09:58:34.000000 nostr_dvm-0.3.8/nostr_dvm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:58:38.750839 nostr_dvm-0.3.8/nostr_dvm/backends/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 09:58:34.000000 nostr_dvm-0.3.8/nostr_dvm/backends/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:58:38.750839 nostr_dvm-0.3.8/nostr_dvm/backends/mlx/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 09:58:34.000000 nostr_dvm-0.3.8/nostr_dvm/backends/mlx/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:58:38.750839 nostr_dvm-0.3.8/nostr_dvm/backends/mlx/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 09:58:34.000000 nostr_dvm-0.3.8/nostr_dvm/backends/mlx/modules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:58:38.750839 nostr_dvm-0.3.8/nostr_dvm/backends/mlx/modules/stable_diffusion/
+-rw-r--r--   0 runner    (1001) docker     (127)     2945 2024-05-16 09:58:34.000000 nostr_dvm-0.3.8/nostr_dvm/backends/mlx/modules/stable_diffusion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2222 2024-05-16 09:58:34.000000 nostr_dvm-0.3.8/nostr_dvm/backends/mlx/modules/stable_diffusion/clip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-05-16 09:58:34.000000 nostr_dvm-0.3.8/nostr_dvm/backends/mlx/modules/stable_diffusion/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9892 2024-05-16 09:58:34.000000 nostr_dvm-0.3.8/nostr_dvm/backends/mlx/modules/stable_diffusion/model_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2300 2024-05-16 09:58:34.000000 nostr_dvm-0.3.8/nostr_dvm/backends/mlx/modules/stable_diffusion/sampler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2991 2024-05-16 09:58:34.000000 nostr_dvm-0.3.8/nostr_dvm/backends/mlx/modules/stable_diffusion/tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13685 2024-05-16 09:58:34.000000 nostr_dvm-0.3.8/nostr_dvm/backends/mlx/modules/stable_diffusion/unet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7773 2024-05-16 09:58:34.000000 nostr_dvm-0.3.8/nostr_dvm/backends/mlx/modules/stable_diffusion/vae.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:58:38.750839 nostr_dvm-0.3.8/nostr_dvm/backends/nova_server/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 09:58:34.000000 nostr_dvm-0.3.8/nostr_dvm/backends/nova_server/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:58:38.754839 nostr_dvm-0.3.8/nostr_dvm/backends/nova_server/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 09:58:34.000000 nostr_dvm-0.3.8/nostr_dvm/backends/nova_server/modules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:58:38.754839 nostr_dvm-0.3.8/nostr_dvm/backends/nova_server/modules/image_interrogator/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 09:58:34.000000 nostr_dvm-0.3.8/nostr_dvm/backends/nova_server/modules/image_interrogator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4906 2024-05-16 09:58:34.000000 nostr_dvm-0.3.8/nostr_dvm/backends/nova_server/modules/image_interrogator/image_interrogator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-05-16 09:58:34.000000 nostr_dvm-0.3.8/nostr_dvm/backends/nova_server/modules/image_interrogator/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:58:38.754839 nostr_dvm-0.3.8/nostr_dvm/backends/nova_server/modules/image_upscale/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 09:58:34.000000 nostr_dvm-0.3.8/nostr_dvm/backends/nova_server/modules/image_upscale/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6863 2024-05-16 09:58:34.000000 nostr_dvm-0.3.8/nostr_dvm/backends/nova_server/modules/image_upscale/image_upscale_realesrgan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7745 2024-05-16 09:58:34.000000 nostr_dvm-0.3.8/nostr_dvm/backends/nova_server/modules/image_upscale/inference_realesrgan.py
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-16 09:58:34.000000 nostr_dvm-0.3.8/nostr_dvm/backends/nova_server/modules/image_upscale/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:58:38.754839 nostr_dvm-0.3.8/nostr_dvm/backends/nova_server/modules/stablediffusionxl/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 09:58:34.000000 nostr_dvm-0.3.8/nostr_dvm/backends/nova_server/modules/stablediffusionxl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3319 2024-05-16 09:58:34.000000 nostr_dvm-0.3.8/nostr_dvm/backends/nova_server/modules/stablediffusionxl/lora.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6854 2024-05-16 09:58:34.000000 nostr_dvm-0.3.8/nostr_dvm/backends/nova_server/modules/stablediffusionxl/stablediffusionxl-img2img.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9229 2024-05-16 09:58:34.000000 nostr_dvm-0.3.8/nostr_dvm/backends/nova_server/modules/stablediffusionxl/stablediffusionxl.py
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-16 09:58:34.000000 nostr_dvm-0.3.8/nostr_dvm/backends/nova_server/modules/stablediffusionxl/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:58:38.754839 nostr_dvm-0.3.8/nostr_dvm/backends/nova_server/modules/whisperx/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 09:58:34.000000 nostr_dvm-0.3.8/nostr_dvm/backends/nova_server/modules/whisperx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-05-16 09:58:34.000000 nostr_dvm-0.3.8/nostr_dvm/backends/nova_server/modules/whisperx/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5250 2024-05-16 09:58:34.000000 nostr_dvm-0.3.8/nostr_dvm/backends/nova_server/modules/whisperx/whisperx_transcript.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4880 2024-05-16 09:58:34.000000 nostr_dvm-0.3.8/nostr_dvm/backends/nova_server/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39902 2024-05-16 09:58:34.000000 nostr_dvm-0.3.8/nostr_dvm/bot.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39670 2024-05-16 09:58:34.000000 nostr_dvm-0.3.8/nostr_dvm/dvm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:58:38.754839 nostr_dvm-0.3.8/nostr_dvm/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 09:58:34.000000 nostr_dvm-0.3.8/nostr_dvm/interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6126 2024-05-16 09:58:34.000000 nostr_dvm-0.3.8/nostr_dvm/interfaces/dvmtaskinterface.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23582 2024-05-16 09:58:34.000000 nostr_dvm-0.3.8/nostr_dvm/subscription.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:58:38.762839 nostr_dvm-0.3.8/nostr_dvm/tasks/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 09:58:34.000000 nostr_dvm-0.3.8/nostr_dvm/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8321 2024-05-16 09:58:34.000000 nostr_dvm-0.3.8/nostr_dvm/tasks/advanced_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7452 2024-05-16 09:58:34.000000 nostr_dvm-0.3.8/nostr_dvm/tasks/advanced_search_wine.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12712 2024-05-16 09:58:34.000000 nostr_dvm-0.3.8/nostr_dvm/tasks/content_discovery_currently_popular.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13233 2024-05-16 09:58:34.000000 nostr_dvm-0.3.8/nostr_dvm/tasks/content_discovery_currently_popular_followers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13312 2024-05-16 09:58:34.000000 nostr_dvm-0.3.8/nostr_dvm/tasks/content_discovery_currently_popular_topic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4049 2024-05-16 09:58:34.000000 nostr_dvm-0.3.8/nostr_dvm/tasks/convert_media.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7854 2024-05-16 09:58:34.000000 nostr_dvm-0.3.8/nostr_dvm/tasks/discovery_bot_farms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8189 2024-05-16 09:58:34.000000 nostr_dvm-0.3.8/nostr_dvm/tasks/discovery_censor_wot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8964 2024-05-16 09:58:34.000000 nostr_dvm-0.3.8/nostr_dvm/tasks/discovery_inactive_follows.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8995 2024-05-16 09:58:34.000000 nostr_dvm-0.3.8/nostr_dvm/tasks/discovery_nonfollowers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4562 2024-05-16 09:58:34.000000 nostr_dvm-0.3.8/nostr_dvm/tasks/discovery_trending_notes_nostrband.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6218 2024-05-16 09:58:34.000000 nostr_dvm-0.3.8/nostr_dvm/tasks/imagegeneration_openai_dalle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5968 2024-05-16 09:58:34.000000 nostr_dvm-0.3.8/nostr_dvm/tasks/imagegeneration_replicate_sdxl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6897 2024-05-16 09:58:34.000000 nostr_dvm-0.3.8/nostr_dvm/tasks/imagegeneration_sd21_mlx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8391 2024-05-16 09:58:34.000000 nostr_dvm-0.3.8/nostr_dvm/tasks/imagegeneration_sdxl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9045 2024-05-16 09:58:34.000000 nostr_dvm-0.3.8/nostr_dvm/tasks/imagegeneration_sdxlimg2img.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5281 2024-05-16 09:58:34.000000 nostr_dvm-0.3.8/nostr_dvm/tasks/imageinterrogator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5283 2024-05-16 09:58:34.000000 nostr_dvm-0.3.8/nostr_dvm/tasks/imageupscale.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8186 2024-05-16 09:58:34.000000 nostr_dvm-0.3.8/nostr_dvm/tasks/search_users.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6450 2024-05-16 09:58:34.000000 nostr_dvm-0.3.8/nostr_dvm/tasks/summarization_huggingchat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6945 2024-05-16 09:58:34.000000 nostr_dvm-0.3.8/nostr_dvm/tasks/summarization_unleashed_chat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6774 2024-05-16 09:58:34.000000 nostr_dvm-0.3.8/nostr_dvm/tasks/textextraction_google.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4514 2024-05-16 09:58:34.000000 nostr_dvm-0.3.8/nostr_dvm/tasks/textextraction_pdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7781 2024-05-16 09:58:34.000000 nostr_dvm-0.3.8/nostr_dvm/tasks/textextraction_whisperx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4320 2024-05-16 09:58:34.000000 nostr_dvm-0.3.8/nostr_dvm/tasks/textgeneration_huggingchat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4985 2024-05-16 09:58:34.000000 nostr_dvm-0.3.8/nostr_dvm/tasks/textgeneration_llmlite.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4664 2024-05-16 09:58:34.000000 nostr_dvm-0.3.8/nostr_dvm/tasks/textgeneration_unleashed_chat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6897 2024-05-16 09:58:34.000000 nostr_dvm-0.3.8/nostr_dvm/tasks/texttospeech.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7004 2024-05-16 09:58:34.000000 nostr_dvm-0.3.8/nostr_dvm/tasks/translation_google.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6895 2024-05-16 09:58:34.000000 nostr_dvm-0.3.8/nostr_dvm/tasks/translation_libretranslate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5571 2024-05-16 09:58:34.000000 nostr_dvm-0.3.8/nostr_dvm/tasks/videogeneration_replicate_svd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4892 2024-05-16 09:58:34.000000 nostr_dvm-0.3.8/nostr_dvm/tasks/videogeneration_svd.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:58:38.766839 nostr_dvm-0.3.8/nostr_dvm/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 09:58:34.000000 nostr_dvm-0.3.8/nostr_dvm/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4334 2024-05-16 09:58:34.000000 nostr_dvm-0.3.8/nostr_dvm/utils/admin_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8745 2024-05-16 09:58:34.000000 nostr_dvm-0.3.8/nostr_dvm/utils/backend_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6163 2024-05-16 09:58:34.000000 nostr_dvm-0.3.8/nostr_dvm/utils/cashu_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9473 2024-05-16 09:58:34.000000 nostr_dvm-0.3.8/nostr_dvm/utils/database_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2700 2024-05-16 09:58:34.000000 nostr_dvm-0.3.8/nostr_dvm/utils/definitions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2424 2024-05-16 09:58:34.000000 nostr_dvm-0.3.8/nostr_dvm/utils/dvmconfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2761 2024-05-16 09:58:34.000000 nostr_dvm-0.3.8/nostr_dvm/utils/external_dvm_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13403 2024-05-16 09:58:34.000000 nostr_dvm-0.3.8/nostr_dvm/utils/mediasource_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8866 2024-05-16 09:58:34.000000 nostr_dvm-0.3.8/nostr_dvm/utils/nip88_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4170 2024-05-16 09:58:34.000000 nostr_dvm-0.3.8/nostr_dvm/utils/nip89_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8449 2024-05-16 09:58:34.000000 nostr_dvm-0.3.8/nostr_dvm/utils/nostr_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3795 2024-05-16 09:58:34.000000 nostr_dvm-0.3.8/nostr_dvm/utils/nwc_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9011 2024-05-16 09:58:34.000000 nostr_dvm-0.3.8/nostr_dvm/utils/output_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:58:38.766839 nostr_dvm-0.3.8/nostr_dvm/utils/scrapper/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 09:58:34.000000 nostr_dvm-0.3.8/nostr_dvm/utils/scrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26119 2024-05-16 09:58:34.000000 nostr_dvm-0.3.8/nostr_dvm/utils/scrapper/media_scrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5712 2024-05-16 09:58:34.000000 nostr_dvm-0.3.8/nostr_dvm/utils/subscription_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15021 2024-05-16 09:58:34.000000 nostr_dvm-0.3.8/nostr_dvm/utils/zap_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:58:38.766839 nostr_dvm-0.3.8/nostr_dvm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-05-16 09:58:38.000000 nostr_dvm-0.3.8/nostr_dvm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4179 2024-05-16 09:58:38.000000 nostr_dvm-0.3.8/nostr_dvm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 09:58:38.000000 nostr_dvm-0.3.8/nostr_dvm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-05-16 09:58:38.000000 nostr_dvm-0.3.8/nostr_dvm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-16 09:58:38.000000 nostr_dvm-0.3.8/nostr_dvm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 09:58:38.766839 nostr_dvm-0.3.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-05-16 09:58:34.000000 nostr_dvm-0.3.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:58:38.766839 nostr_dvm-0.3.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    13764 2024-05-16 09:58:34.000000 nostr_dvm-0.3.8/tests/test_dvm_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3213 2024-05-16 09:58:34.000000 nostr_dvm-0.3.8/tests/test_events.py
```

### Comparing `nostr_dvm-0.3.7/LICENSE` & `nostr_dvm-0.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.7/PKG-INFO` & `nostr_dvm-0.3.8/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nostr-dvm
-Version: 0.3.7
+Version: 0.3.8
 Summary: A framework to build and run Nostr NIP90 Data Vending Machines
 Home-page: https://github.com/believethehype/nostrdvm
 Author: Believethehype
 Author-email: believethehypeonnostr@proton.me
 License: MIT
 Keywords: nostr,nip90,dvm,data vending machine
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `nostr_dvm-0.3.7/README.md` & `nostr_dvm-0.3.8/README.md`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.7/nostr_dvm/backends/mlx/modules/stable_diffusion/__init__.py` & `nostr_dvm-0.3.8/nostr_dvm/backends/mlx/modules/stable_diffusion/__init__.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.7/nostr_dvm/backends/mlx/modules/stable_diffusion/clip.py` & `nostr_dvm-0.3.8/nostr_dvm/backends/mlx/modules/stable_diffusion/clip.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.7/nostr_dvm/backends/mlx/modules/stable_diffusion/config.py` & `nostr_dvm-0.3.8/nostr_dvm/backends/mlx/modules/stable_diffusion/config.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.7/nostr_dvm/backends/mlx/modules/stable_diffusion/model_io.py` & `nostr_dvm-0.3.8/nostr_dvm/backends/mlx/modules/stable_diffusion/model_io.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.7/nostr_dvm/backends/mlx/modules/stable_diffusion/sampler.py` & `nostr_dvm-0.3.8/nostr_dvm/backends/mlx/modules/stable_diffusion/sampler.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.7/nostr_dvm/backends/mlx/modules/stable_diffusion/tokenizer.py` & `nostr_dvm-0.3.8/nostr_dvm/backends/mlx/modules/stable_diffusion/tokenizer.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.7/nostr_dvm/backends/mlx/modules/stable_diffusion/unet.py` & `nostr_dvm-0.3.8/nostr_dvm/backends/mlx/modules/stable_diffusion/unet.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.7/nostr_dvm/backends/mlx/modules/stable_diffusion/vae.py` & `nostr_dvm-0.3.8/nostr_dvm/backends/mlx/modules/stable_diffusion/vae.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.7/nostr_dvm/backends/nova_server/modules/image_interrogator/image_interrogator.py` & `nostr_dvm-0.3.8/nostr_dvm/backends/nova_server/modules/image_interrogator/image_interrogator.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.7/nostr_dvm/backends/nova_server/modules/image_upscale/image_upscale_realesrgan.py` & `nostr_dvm-0.3.8/nostr_dvm/backends/nova_server/modules/image_upscale/image_upscale_realesrgan.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.7/nostr_dvm/backends/nova_server/modules/image_upscale/inference_realesrgan.py` & `nostr_dvm-0.3.8/nostr_dvm/backends/nova_server/modules/image_upscale/inference_realesrgan.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.7/nostr_dvm/backends/nova_server/modules/stablediffusionxl/lora.py` & `nostr_dvm-0.3.8/nostr_dvm/backends/nova_server/modules/stablediffusionxl/lora.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.7/nostr_dvm/backends/nova_server/modules/stablediffusionxl/stablediffusionxl-img2img.py` & `nostr_dvm-0.3.8/nostr_dvm/backends/nova_server/modules/stablediffusionxl/stablediffusionxl-img2img.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.7/nostr_dvm/backends/nova_server/modules/stablediffusionxl/stablediffusionxl.py` & `nostr_dvm-0.3.8/nostr_dvm/backends/nova_server/modules/stablediffusionxl/stablediffusionxl.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.7/nostr_dvm/backends/nova_server/modules/whisperx/whisperx_transcript.py` & `nostr_dvm-0.3.8/nostr_dvm/backends/nova_server/modules/whisperx/whisperx_transcript.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.7/nostr_dvm/backends/nova_server/utils.py` & `nostr_dvm-0.3.8/nostr_dvm/backends/nova_server/utils.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.7/nostr_dvm/bot.py` & `nostr_dvm-0.3.8/nostr_dvm/bot.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.7/nostr_dvm/dvm.py` & `nostr_dvm-0.3.8/nostr_dvm/dvm.py`

 * *Files 2% similar despite different names*

```diff
@@ -187,14 +187,15 @@
                         self.dvm_config.PUBLIC_KEY):
                     print(
                         "[" + self.dvm_config.NIP89.NAME + "] Free task or Whitelisted for task " + task +
                         ". Starting processing..")
 
                     if dvm_config.SEND_FEEDBACK_EVENTS:
                         send_job_status_reaction(nip90_event, "processing", True, 0,
+                                                 content=dvm_config.CUSTOM_PROCESSING_MESSAGE,
                                                  client=self.client, dvm_config=self.dvm_config, user=user)
 
                     #  when we reimburse users on error make sure to not send anything if it was free
                     if user.iswhitelisted or task_is_free:
                         amount = 0
                     do_work(nip90_event, amount)
                 # if task is directed to us via p tag and user has balance or is subscribed, do the job and update balance
@@ -214,14 +215,15 @@
                             "[" + self.dvm_config.NIP89.NAME + "] Using user's balance for task: " + task +
                             ". Starting processing.. New balance is: " + str(balance))
                     else:
                         print("[" + self.dvm_config.NIP89.NAME + "] User has active subscription for task: " + task +
                               ". Starting processing.. Balance remains at: " + str(user.balance))
 
                     send_job_status_reaction(nip90_event, "processing", True, 0,
+                                             content=dvm_config.CUSTOM_PROCESSING_MESSAGE,
                                              client=self.client, dvm_config=self.dvm_config)
 
                     do_work(nip90_event, amount)
 
                 # else send a payment required event to user
                 elif p_tag_str == "" or p_tag_str == self.dvm_config.PUBLIC_KEY:
 
@@ -306,14 +308,15 @@
                                                                            config=self.dvm_config)
                             if job_event is not None and task_supported:
                                 print("Zap received for NIP90 task: " + str(invoice_amount) + " Sats from " + str(
                                     user.name))
                                 if amount <= invoice_amount:
                                     print("[" + self.dvm_config.NIP89.NAME + "]  Payment-request fulfilled...")
                                     send_job_status_reaction(job_event, "processing", client=self.client,
+                                                             content=dvm_config.CUSTOM_PROCESSING_MESSAGE,
                                                              dvm_config=self.dvm_config, user=user)
                                     indices = [i for i, x in enumerate(self.job_list) if
                                                x.event == job_event]
                                     index = -1
                                     if len(indices) > 0:
                                         index = indices[0]
                                     if index > -1:
```

### Comparing `nostr_dvm-0.3.7/nostr_dvm/interfaces/dvmtaskinterface.py` & `nostr_dvm-0.3.8/nostr_dvm/interfaces/dvmtaskinterface.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.7/nostr_dvm/subscription.py` & `nostr_dvm-0.3.8/nostr_dvm/subscription.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.7/nostr_dvm/tasks/advanced_search.py` & `nostr_dvm-0.3.8/nostr_dvm/tasks/advanced_search.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.7/nostr_dvm/tasks/advanced_search_wine.py` & `nostr_dvm-0.3.8/nostr_dvm/tasks/advanced_search_wine.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.7/nostr_dvm/tasks/content_discovery_currently_popular.py` & `nostr_dvm-0.3.8/nostr_dvm/tasks/content_discovery_currently_popular.py`

 * *Files 3% similar despite different names*

```diff
@@ -189,23 +189,27 @@
         print(
             "[" + self.dvm_config.IDENTIFIER + "] Done Syncing Notes of the last " + str(self.db_since) + " seconds..")
 
 
 # We build an example here that we can call by either calling this file directly from the main directory,
 # or by adding it to our playground. You can call the example and adjust it to your needs or redefine it in the
 # playground or elsewhere
-def build_example(name, identifier, admin_config):
+def build_example(name, identifier, admin_config, processing_msg=None):
     dvm_config = build_default_config(identifier)
     dvm_config.USE_OWN_VENV = False
     dvm_config.SHOWLOG = True
     dvm_config.SCHEDULE_UPDATES_SECONDS = 600  # Every 10 minutes
     # Activate these to use a subscription based model instead
     # dvm_config.SUBSCRIPTION_REQUIRED = True
     # dvm_config.SUBSCRIPTION_DAILY_COST = 1
     dvm_config.FIX_COST = 0
+    dvm_config.CUSTOM_PROCESSING_MESSAGE = processing_msg
+    admin_config.LUD16 = dvm_config.LN_ADDRESS
+
+
 
     # Add NIP89
     nip89info = {
         "name": name,
         "image": "https://image.nostr.build/b29b6ec4bf9b6184f69d33cb44862db0d90a2dd9a506532e7ba5698af7d36210.jpg",
         "about": "I show notes that are currently popular",
         "lud16": dvm_config.LN_ADDRESS,
@@ -229,22 +233,26 @@
     #admin_config.UPDATE_PROFILE = False
     #admin_config.REBROADCAST_NIP89 = False
 
     return DicoverContentCurrentlyPopular(name=name, dvm_config=dvm_config, nip89config=nip89config,
                                           admin_config=admin_config)
 
 
-def build_example_subscription(name, identifier, admin_config):
+def build_example_subscription(name, identifier, admin_config, processing_msg=None):
     dvm_config = build_default_config(identifier)
     dvm_config.USE_OWN_VENV = False
     dvm_config.SHOWLOG = True
     dvm_config.SCHEDULE_UPDATES_SECONDS = 600  # Every 10 minutes
     # Activate these to use a subscription based model instead
     # dvm_config.SUBSCRIPTION_DAILY_COST = 1
     dvm_config.FIX_COST = 0
+    dvm_config.CUSTOM_PROCESSING_MESSAGE = processing_msg
+    admin_config.LUD16 = dvm_config.LN_ADDRESS
+
+
 
     # Add NIP89
     nip89info = {
         "name": name,
         "image": "https://image.nostr.build/b29b6ec4bf9b6184f69d33cb44862db0d90a2dd9a506532e7ba5698af7d36210.jpg",
         "about": "I show notes that are currently popular all over Nostr. I'm also used for testing subscriptions.",
         "lud16": dvm_config.LN_ADDRESS,
```

### Comparing `nostr_dvm-0.3.7/nostr_dvm/tasks/content_discovery_currently_popular_followers.py` & `nostr_dvm-0.3.8/nostr_dvm/tasks/content_discovery_currently_popular_followers.py`

 * *Files 2% similar despite different names*

```diff
@@ -207,23 +207,26 @@
 
         print("[" + self.dvm_config.IDENTIFIER + "] Done Syncing Notes of the last " + str(self.db_since) + " seconds..")
 
 
 # We build an example here that we can call by either calling this file directly from the main directory,
 # or by adding it to our playground. You can call the example and adjust it to your needs or redefine it in the
 # playground or elsewhere
-def build_example(name, identifier, admin_config):
+def build_example(name, identifier, admin_config, processing_msg=None):
     dvm_config = build_default_config(identifier)
     dvm_config.USE_OWN_VENV = False
     dvm_config.SHOWLOG = True
     dvm_config.SCHEDULE_UPDATES_SECONDS = 600  # Every 10 minutes
     # Activate these to use a subscription based model instead
     # dvm_config.SUBSCRIPTION_REQUIRED = True
     # dvm_config.SUBSCRIPTION_DAILY_COST = 1
     dvm_config.FIX_COST = 0
+    dvm_config.CUSTOM_PROCESSING_MESSAGE = processing_msg
+    admin_config.LUD16 = dvm_config.LN_ADDRESS
+
 
     # Add NIP89
     nip89info = {
         "name": name,
         "image": "https://image.nostr.build/d92652a6a07677e051d647dcf9f0f59e265299b3335a939d008183a911513f4a.jpg",
         "about": "I show notes that are currently popular from people you follow",
         "lud16": dvm_config.LN_ADDRESS,
@@ -247,22 +250,23 @@
     admin_config.UPDATE_PROFILE = False
     admin_config.REBROADCAST_NIP89 = False
 
     return DicoverContentCurrentlyPopularFollowers(name=name, dvm_config=dvm_config, nip89config=nip89config,
                                                    admin_config=admin_config)
 
 
-def build_example_subscription(name, identifier, admin_config):
+def build_example_subscription(name, identifier, admin_config, processing_msg=None):
     dvm_config = build_default_config(identifier)
     dvm_config.USE_OWN_VENV = False
     dvm_config.SHOWLOG = True
     dvm_config.SCHEDULE_UPDATES_SECONDS = 600  # Every 10 minutes
     # Activate these to use a subscription based model instead
     # dvm_config.SUBSCRIPTION_DAILY_COST = 1
     dvm_config.FIX_COST = 0
+    dvm_config.CUSTOM_PROCESSING_MESSAGE = processing_msg
 
     # Add NIP89
     nip89info = {
         "name": name,
         "image": "https://image.nostr.build/b29b6ec4bf9b6184f69d33cb44862db0d90a2dd9a506532e7ba5698af7d36210.jpg",
         "about": "I show notes that are currently popular, just like the free DVM, I'm also used for testing subscriptions. (beta)",
         "lud16": dvm_config.LN_ADDRESS,
```

### Comparing `nostr_dvm-0.3.7/nostr_dvm/tasks/content_discovery_currently_popular_topic.py` & `nostr_dvm-0.3.8/nostr_dvm/tasks/content_discovery_currently_popular_topic.py`

 * *Files 2% similar despite different names*

```diff
@@ -214,23 +214,26 @@
 
         print("[" + self.dvm_config.IDENTIFIER + "] Done Syncing Notes of the last " + str(self.db_since) + " seconds..")
 
 
 # We build an example here that we can call by either calling this file directly from the main directory,
 # or by adding it to our playground. You can call the example and adjust it to your needs or redefine it in the
 # playground or elsewhere
-def build_example(name, identifier, admin_config, options, image, description):
+def build_example(name, identifier, admin_config, options, image, description, processing_msg=None):
     dvm_config = build_default_config(identifier)
     dvm_config.USE_OWN_VENV = False
     dvm_config.SHOWLOG = True
     dvm_config.SCHEDULE_UPDATES_SECONDS = 600  # Every 10 minutes
     # Activate these to use a subscription based model instead
     # dvm_config.SUBSCRIPTION_REQUIRED = True
     # dvm_config.SUBSCRIPTION_DAILY_COST = 1
     dvm_config.FIX_COST = 0
+    dvm_config.CUSTOM_PROCESSING_MESSAGE = processing_msg
+    admin_config.LUD16 = dvm_config.LN_ADDRESS
+
 
     # Add NIP89
     nip89info = {
         "name": name,
         "image": image,
         "about": description,
         "lud16": dvm_config.LN_ADDRESS,
@@ -251,21 +254,24 @@
     nip89config.DTAG = check_and_set_d_tag(identifier, name, dvm_config.PRIVATE_KEY, nip89info["image"])
     nip89config.CONTENT = json.dumps(nip89info)
 
     return DicoverContentCurrentlyPopularbyTopic(name=name, dvm_config=dvm_config, nip89config=nip89config,
                                           admin_config=admin_config, options=options)
 
 
-def build_example_subscription(name, identifier, admin_config, options, image, description):
+def build_example_subscription(name, identifier, admin_config, options, image, description, processing_msg=None):
     dvm_config = build_default_config(identifier)
     dvm_config.USE_OWN_VENV = False
     dvm_config.SHOWLOG = True
     dvm_config.SCHEDULE_UPDATES_SECONDS = 600  # Every 10 minutes
     # Activate these to use a subscription based model instead
     dvm_config.FIX_COST = 0
+    dvm_config.CUSTOM_PROCESSING_MESSAGE = processing_msg
+    admin_config.LUD16 = dvm_config.LN_ADDRESS
+
 
     # Add NIP89
     nip89info = {
         "name": name,
         "image": image,
         "about": description,
         "lud16": dvm_config.LN_ADDRESS,
```

### Comparing `nostr_dvm-0.3.7/nostr_dvm/tasks/convert_media.py` & `nostr_dvm-0.3.8/nostr_dvm/tasks/convert_media.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.7/nostr_dvm/tasks/discovery_bot_farms.py` & `nostr_dvm-0.3.8/nostr_dvm/tasks/discovery_bot_farms.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.7/nostr_dvm/tasks/discovery_censor_wot.py` & `nostr_dvm-0.3.8/nostr_dvm/tasks/discovery_censor_wot.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.7/nostr_dvm/tasks/discovery_inactive_follows.py` & `nostr_dvm-0.3.8/nostr_dvm/tasks/discovery_inactive_follows.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.7/nostr_dvm/tasks/discovery_nonfollowers.py` & `nostr_dvm-0.3.8/nostr_dvm/tasks/discovery_nonfollowers.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.7/nostr_dvm/tasks/discovery_trending_notes_nostrband.py` & `nostr_dvm-0.3.8/nostr_dvm/tasks/discovery_trending_notes_nostrband.py`

 * *Files 2% similar despite different names*

```diff
@@ -93,17 +93,18 @@
         # if not text/plain, don't post-process
         return result
 
 
 # We build an example here that we can call by either calling this file directly from the main directory,
 # or by adding it to our playground. You can call the example and adjust it to your needs or redefine it in the
 # playground or elsewhere
-def build_example(name, identifier, admin_config):
+def build_example(name, identifier, admin_config, custom_processing_msg):
     dvm_config = build_default_config(identifier)
     dvm_config.USE_OWN_VENV = False
+    dvm_config.CUSTOM_PROCESSING_MESSAGE = custom_processing_msg
     admin_config.LUD16 = dvm_config.LN_ADDRESS
     # Add NIP89
 
     nip89info = {
         "name": name,
         "image": "https://nostr.band/android-chrome-192x192.png",
         "about": "I show trending notes from nostr.band",
```

### Comparing `nostr_dvm-0.3.7/nostr_dvm/tasks/imagegeneration_openai_dalle.py` & `nostr_dvm-0.3.8/nostr_dvm/tasks/imagegeneration_openai_dalle.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.7/nostr_dvm/tasks/imagegeneration_replicate_sdxl.py` & `nostr_dvm-0.3.8/nostr_dvm/tasks/imagegeneration_replicate_sdxl.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.7/nostr_dvm/tasks/imagegeneration_sd21_mlx.py` & `nostr_dvm-0.3.8/nostr_dvm/tasks/imagegeneration_sd21_mlx.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.7/nostr_dvm/tasks/imagegeneration_sdxl.py` & `nostr_dvm-0.3.8/nostr_dvm/tasks/imagegeneration_sdxl.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.7/nostr_dvm/tasks/imagegeneration_sdxlimg2img.py` & `nostr_dvm-0.3.8/nostr_dvm/tasks/imagegeneration_sdxlimg2img.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.7/nostr_dvm/tasks/imageinterrogator.py` & `nostr_dvm-0.3.8/nostr_dvm/tasks/imageinterrogator.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.7/nostr_dvm/tasks/imageupscale.py` & `nostr_dvm-0.3.8/nostr_dvm/tasks/imageupscale.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.7/nostr_dvm/tasks/search_users.py` & `nostr_dvm-0.3.8/nostr_dvm/tasks/search_users.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.7/nostr_dvm/tasks/summarization_huggingchat.py` & `nostr_dvm-0.3.8/nostr_dvm/tasks/summarization_huggingchat.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.7/nostr_dvm/tasks/summarization_unleashed_chat.py` & `nostr_dvm-0.3.8/nostr_dvm/tasks/summarization_unleashed_chat.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.7/nostr_dvm/tasks/textextraction_google.py` & `nostr_dvm-0.3.8/nostr_dvm/tasks/textextraction_google.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.7/nostr_dvm/tasks/textextraction_pdf.py` & `nostr_dvm-0.3.8/nostr_dvm/tasks/textextraction_pdf.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.7/nostr_dvm/tasks/textextraction_whisperx.py` & `nostr_dvm-0.3.8/nostr_dvm/tasks/textextraction_whisperx.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.7/nostr_dvm/tasks/textgeneration_huggingchat.py` & `nostr_dvm-0.3.8/nostr_dvm/tasks/textgeneration_huggingchat.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.7/nostr_dvm/tasks/textgeneration_llmlite.py` & `nostr_dvm-0.3.8/nostr_dvm/tasks/textgeneration_llmlite.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.7/nostr_dvm/tasks/textgeneration_unleashed_chat.py` & `nostr_dvm-0.3.8/nostr_dvm/tasks/textgeneration_unleashed_chat.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.7/nostr_dvm/tasks/texttospeech.py` & `nostr_dvm-0.3.8/nostr_dvm/tasks/texttospeech.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.7/nostr_dvm/tasks/translation_google.py` & `nostr_dvm-0.3.8/nostr_dvm/tasks/translation_google.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.7/nostr_dvm/tasks/translation_libretranslate.py` & `nostr_dvm-0.3.8/nostr_dvm/tasks/translation_libretranslate.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.7/nostr_dvm/tasks/videogeneration_replicate_svd.py` & `nostr_dvm-0.3.8/nostr_dvm/tasks/videogeneration_replicate_svd.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.7/nostr_dvm/tasks/videogeneration_svd.py` & `nostr_dvm-0.3.8/nostr_dvm/tasks/videogeneration_svd.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.7/nostr_dvm/utils/admin_utils.py` & `nostr_dvm-0.3.8/nostr_dvm/utils/admin_utils.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.7/nostr_dvm/utils/backend_utils.py` & `nostr_dvm-0.3.8/nostr_dvm/utils/backend_utils.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.7/nostr_dvm/utils/cashu_utils.py` & `nostr_dvm-0.3.8/nostr_dvm/utils/cashu_utils.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.7/nostr_dvm/utils/database_utils.py` & `nostr_dvm-0.3.8/nostr_dvm/utils/database_utils.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.7/nostr_dvm/utils/definitions.py` & `nostr_dvm-0.3.8/nostr_dvm/utils/definitions.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.7/nostr_dvm/utils/dvmconfig.py` & `nostr_dvm-0.3.8/nostr_dvm/utils/dvmconfig.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,14 +34,15 @@
     NEW_USER_BALANCE: int = 0  # Free credits for new users
     SUBSCRIPTION_MANAGEMENT = 'https://noogle.lol/discovery'
     NIP88: NIP88Config
     NIP89: NIP89Config
     SEND_FEEDBACK_EVENTS = True
     SHOW_RESULT_BEFORE_PAYMENT: bool = False  # if this is true show results even when not paid right after autoprocess
     SCHEDULE_UPDATES_SECONDS = 0
+    CUSTOM_PROCESSING_MESSAGE = None
 
 
 def build_default_config(identifier):
     dvm_config = DVMConfig()
     dvm_config.PRIVATE_KEY = check_and_set_private_key(identifier)
     dvm_config.IDENTIFIER = identifier
     npub = Keys.parse(dvm_config.PRIVATE_KEY).public_key().to_bech32()
```

### Comparing `nostr_dvm-0.3.7/nostr_dvm/utils/external_dvm_utils.py` & `nostr_dvm-0.3.8/nostr_dvm/utils/external_dvm_utils.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.7/nostr_dvm/utils/mediasource_utils.py` & `nostr_dvm-0.3.8/nostr_dvm/utils/mediasource_utils.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.7/nostr_dvm/utils/nip88_utils.py` & `nostr_dvm-0.3.8/nostr_dvm/utils/nip88_utils.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.7/nostr_dvm/utils/nip89_utils.py` & `nostr_dvm-0.3.8/nostr_dvm/utils/nip89_utils.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.7/nostr_dvm/utils/nostr_utils.py` & `nostr_dvm-0.3.8/nostr_dvm/utils/nostr_utils.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.7/nostr_dvm/utils/nwc_tools.py` & `nostr_dvm-0.3.8/nostr_dvm/utils/nwc_tools.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.7/nostr_dvm/utils/output_utils.py` & `nostr_dvm-0.3.8/nostr_dvm/utils/output_utils.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.7/nostr_dvm/utils/scrapper/media_scrapper.py` & `nostr_dvm-0.3.8/nostr_dvm/utils/scrapper/media_scrapper.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.7/nostr_dvm/utils/subscription_utils.py` & `nostr_dvm-0.3.8/nostr_dvm/utils/subscription_utils.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.7/nostr_dvm/utils/zap_utils.py` & `nostr_dvm-0.3.8/nostr_dvm/utils/zap_utils.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.7/nostr_dvm.egg-info/PKG-INFO` & `nostr_dvm-0.3.8/nostr_dvm.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nostr-dvm
-Version: 0.3.7
+Version: 0.3.8
 Summary: A framework to build and run Nostr NIP90 Data Vending Machines
 Home-page: https://github.com/believethehype/nostrdvm
 Author: Believethehype
 Author-email: believethehypeonnostr@proton.me
 License: MIT
 Keywords: nostr,nip90,dvm,data vending machine
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `nostr_dvm-0.3.7/nostr_dvm.egg-info/SOURCES.txt` & `nostr_dvm-0.3.8/nostr_dvm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.7/setup.py` & `nostr_dvm-0.3.8/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.3.7'
+VERSION = '0.3.8'
 DESCRIPTION = 'A framework to build and run Nostr NIP90 Data Vending Machines'
 LONG_DESCRIPTION = ('A framework to build and run Nostr NIP90 Data Vending Machines. See the github repository for more information')
 
 # Setting up
 setup(
     name="nostr-dvm",
     version=VERSION,
```

### Comparing `nostr_dvm-0.3.7/tests/test_dvm_client.py` & `nostr_dvm-0.3.8/tests/test_dvm_client.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.7/tests/test_events.py` & `nostr_dvm-0.3.8/tests/test_events.py`

 * *Files identical despite different names*
