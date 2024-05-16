# Comparing `tmp/nostr_dvm-0.3.5.tar.gz` & `tmp/nostr_dvm-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nostr_dvm-0.3.5.tar", last modified: Mon May  6 10:19:10 2024, max compression
+gzip compressed data, was "nostr_dvm-0.3.6.tar", last modified: Thu May 16 08:31:17 2024, max compression
```

## Comparing `nostr_dvm-0.3.5.tar` & `nostr_dvm-0.3.6.tar`

### file list

```diff
@@ -1,115 +1,116 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 10:19:10.300576 nostr_dvm-0.3.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-06 10:19:03.000000 nostr_dvm-0.3.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-05-06 10:19:10.300576 nostr_dvm-0.3.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1563 2024-05-06 10:19:03.000000 nostr_dvm-0.3.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 10:19:10.284576 nostr_dvm-0.3.5/nostr_dvm/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 10:19:03.000000 nostr_dvm-0.3.5/nostr_dvm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 10:19:10.284576 nostr_dvm-0.3.5/nostr_dvm/backends/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 10:19:03.000000 nostr_dvm-0.3.5/nostr_dvm/backends/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 10:19:10.284576 nostr_dvm-0.3.5/nostr_dvm/backends/mlx/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 10:19:03.000000 nostr_dvm-0.3.5/nostr_dvm/backends/mlx/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 10:19:10.284576 nostr_dvm-0.3.5/nostr_dvm/backends/mlx/modules/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 10:19:03.000000 nostr_dvm-0.3.5/nostr_dvm/backends/mlx/modules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 10:19:10.288576 nostr_dvm-0.3.5/nostr_dvm/backends/mlx/modules/stable_diffusion/
--rw-r--r--   0 runner    (1001) docker     (127)     2945 2024-05-06 10:19:03.000000 nostr_dvm-0.3.5/nostr_dvm/backends/mlx/modules/stable_diffusion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2222 2024-05-06 10:19:03.000000 nostr_dvm-0.3.5/nostr_dvm/backends/mlx/modules/stable_diffusion/clip.py
--rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-05-06 10:19:03.000000 nostr_dvm-0.3.5/nostr_dvm/backends/mlx/modules/stable_diffusion/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     9892 2024-05-06 10:19:03.000000 nostr_dvm-0.3.5/nostr_dvm/backends/mlx/modules/stable_diffusion/model_io.py
--rw-r--r--   0 runner    (1001) docker     (127)     2300 2024-05-06 10:19:03.000000 nostr_dvm-0.3.5/nostr_dvm/backends/mlx/modules/stable_diffusion/sampler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2991 2024-05-06 10:19:03.000000 nostr_dvm-0.3.5/nostr_dvm/backends/mlx/modules/stable_diffusion/tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (127)    13685 2024-05-06 10:19:03.000000 nostr_dvm-0.3.5/nostr_dvm/backends/mlx/modules/stable_diffusion/unet.py
--rw-r--r--   0 runner    (1001) docker     (127)     7773 2024-05-06 10:19:03.000000 nostr_dvm-0.3.5/nostr_dvm/backends/mlx/modules/stable_diffusion/vae.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 10:19:10.288576 nostr_dvm-0.3.5/nostr_dvm/backends/nova_server/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 10:19:03.000000 nostr_dvm-0.3.5/nostr_dvm/backends/nova_server/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 10:19:10.288576 nostr_dvm-0.3.5/nostr_dvm/backends/nova_server/modules/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 10:19:03.000000 nostr_dvm-0.3.5/nostr_dvm/backends/nova_server/modules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 10:19:10.288576 nostr_dvm-0.3.5/nostr_dvm/backends/nova_server/modules/image_interrogator/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 10:19:03.000000 nostr_dvm-0.3.5/nostr_dvm/backends/nova_server/modules/image_interrogator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4906 2024-05-06 10:19:03.000000 nostr_dvm-0.3.5/nostr_dvm/backends/nova_server/modules/image_interrogator/image_interrogator.py
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-05-06 10:19:03.000000 nostr_dvm-0.3.5/nostr_dvm/backends/nova_server/modules/image_interrogator/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 10:19:10.288576 nostr_dvm-0.3.5/nostr_dvm/backends/nova_server/modules/image_upscale/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 10:19:03.000000 nostr_dvm-0.3.5/nostr_dvm/backends/nova_server/modules/image_upscale/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6863 2024-05-06 10:19:03.000000 nostr_dvm-0.3.5/nostr_dvm/backends/nova_server/modules/image_upscale/image_upscale_realesrgan.py
--rw-r--r--   0 runner    (1001) docker     (127)     7745 2024-05-06 10:19:03.000000 nostr_dvm-0.3.5/nostr_dvm/backends/nova_server/modules/image_upscale/inference_realesrgan.py
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-06 10:19:03.000000 nostr_dvm-0.3.5/nostr_dvm/backends/nova_server/modules/image_upscale/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 10:19:10.288576 nostr_dvm-0.3.5/nostr_dvm/backends/nova_server/modules/stablediffusionxl/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 10:19:03.000000 nostr_dvm-0.3.5/nostr_dvm/backends/nova_server/modules/stablediffusionxl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3319 2024-05-06 10:19:03.000000 nostr_dvm-0.3.5/nostr_dvm/backends/nova_server/modules/stablediffusionxl/lora.py
--rw-r--r--   0 runner    (1001) docker     (127)     6854 2024-05-06 10:19:03.000000 nostr_dvm-0.3.5/nostr_dvm/backends/nova_server/modules/stablediffusionxl/stablediffusionxl-img2img.py
--rw-r--r--   0 runner    (1001) docker     (127)     9229 2024-05-06 10:19:03.000000 nostr_dvm-0.3.5/nostr_dvm/backends/nova_server/modules/stablediffusionxl/stablediffusionxl.py
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-06 10:19:03.000000 nostr_dvm-0.3.5/nostr_dvm/backends/nova_server/modules/stablediffusionxl/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 10:19:10.288576 nostr_dvm-0.3.5/nostr_dvm/backends/nova_server/modules/whisperx/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 10:19:03.000000 nostr_dvm-0.3.5/nostr_dvm/backends/nova_server/modules/whisperx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-05-06 10:19:03.000000 nostr_dvm-0.3.5/nostr_dvm/backends/nova_server/modules/whisperx/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     5250 2024-05-06 10:19:03.000000 nostr_dvm-0.3.5/nostr_dvm/backends/nova_server/modules/whisperx/whisperx_transcript.py
--rw-r--r--   0 runner    (1001) docker     (127)     4880 2024-05-06 10:19:03.000000 nostr_dvm-0.3.5/nostr_dvm/backends/nova_server/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    39816 2024-05-06 10:19:03.000000 nostr_dvm-0.3.5/nostr_dvm/bot.py
--rw-r--r--   0 runner    (1001) docker     (127)    39377 2024-05-06 10:19:03.000000 nostr_dvm-0.3.5/nostr_dvm/dvm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 10:19:10.292576 nostr_dvm-0.3.5/nostr_dvm/interfaces/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 10:19:03.000000 nostr_dvm-0.3.5/nostr_dvm/interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6126 2024-05-06 10:19:03.000000 nostr_dvm-0.3.5/nostr_dvm/interfaces/dvmtaskinterface.py
--rw-r--r--   0 runner    (1001) docker     (127)    23351 2024-05-06 10:19:03.000000 nostr_dvm-0.3.5/nostr_dvm/subscription.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 10:19:10.296576 nostr_dvm-0.3.5/nostr_dvm/tasks/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 10:19:03.000000 nostr_dvm-0.3.5/nostr_dvm/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8321 2024-05-06 10:19:03.000000 nostr_dvm-0.3.5/nostr_dvm/tasks/advanced_search.py
--rw-r--r--   0 runner    (1001) docker     (127)     7452 2024-05-06 10:19:03.000000 nostr_dvm-0.3.5/nostr_dvm/tasks/advanced_search_wine.py
--rw-r--r--   0 runner    (1001) docker     (127)    11255 2024-05-06 10:19:03.000000 nostr_dvm-0.3.5/nostr_dvm/tasks/content_discovery_currently_popular.py
--rw-r--r--   0 runner    (1001) docker     (127)    12843 2024-05-06 10:19:03.000000 nostr_dvm-0.3.5/nostr_dvm/tasks/content_discovery_currently_popular_followers.py
--rw-r--r--   0 runner    (1001) docker     (127)     4049 2024-05-06 10:19:03.000000 nostr_dvm-0.3.5/nostr_dvm/tasks/convert_media.py
--rw-r--r--   0 runner    (1001) docker     (127)     7851 2024-05-06 10:19:03.000000 nostr_dvm-0.3.5/nostr_dvm/tasks/discovery_bot_farms.py
--rw-r--r--   0 runner    (1001) docker     (127)     8189 2024-05-06 10:19:03.000000 nostr_dvm-0.3.5/nostr_dvm/tasks/discovery_censor_wot.py
--rw-r--r--   0 runner    (1001) docker     (127)     8964 2024-05-06 10:19:03.000000 nostr_dvm-0.3.5/nostr_dvm/tasks/discovery_inactive_follows.py
--rw-r--r--   0 runner    (1001) docker     (127)     8995 2024-05-06 10:19:03.000000 nostr_dvm-0.3.5/nostr_dvm/tasks/discovery_nonfollowers.py
--rw-r--r--   0 runner    (1001) docker     (127)     4473 2024-05-06 10:19:03.000000 nostr_dvm-0.3.5/nostr_dvm/tasks/discovery_trending_notes_nostrband.py
--rw-r--r--   0 runner    (1001) docker     (127)     6218 2024-05-06 10:19:03.000000 nostr_dvm-0.3.5/nostr_dvm/tasks/imagegeneration_openai_dalle.py
--rw-r--r--   0 runner    (1001) docker     (127)     5968 2024-05-06 10:19:03.000000 nostr_dvm-0.3.5/nostr_dvm/tasks/imagegeneration_replicate_sdxl.py
--rw-r--r--   0 runner    (1001) docker     (127)     6897 2024-05-06 10:19:03.000000 nostr_dvm-0.3.5/nostr_dvm/tasks/imagegeneration_sd21_mlx.py
--rw-r--r--   0 runner    (1001) docker     (127)     8391 2024-05-06 10:19:03.000000 nostr_dvm-0.3.5/nostr_dvm/tasks/imagegeneration_sdxl.py
--rw-r--r--   0 runner    (1001) docker     (127)     9045 2024-05-06 10:19:03.000000 nostr_dvm-0.3.5/nostr_dvm/tasks/imagegeneration_sdxlimg2img.py
--rw-r--r--   0 runner    (1001) docker     (127)     5281 2024-05-06 10:19:03.000000 nostr_dvm-0.3.5/nostr_dvm/tasks/imageinterrogator.py
--rw-r--r--   0 runner    (1001) docker     (127)     5283 2024-05-06 10:19:03.000000 nostr_dvm-0.3.5/nostr_dvm/tasks/imageupscale.py
--rw-r--r--   0 runner    (1001) docker     (127)     8169 2024-05-06 10:19:03.000000 nostr_dvm-0.3.5/nostr_dvm/tasks/search_users.py
--rw-r--r--   0 runner    (1001) docker     (127)     6450 2024-05-06 10:19:03.000000 nostr_dvm-0.3.5/nostr_dvm/tasks/summarization_huggingchat.py
--rw-r--r--   0 runner    (1001) docker     (127)     6945 2024-05-06 10:19:03.000000 nostr_dvm-0.3.5/nostr_dvm/tasks/summarization_unleashed_chat.py
--rw-r--r--   0 runner    (1001) docker     (127)     6774 2024-05-06 10:19:03.000000 nostr_dvm-0.3.5/nostr_dvm/tasks/textextraction_google.py
--rw-r--r--   0 runner    (1001) docker     (127)     4514 2024-05-06 10:19:03.000000 nostr_dvm-0.3.5/nostr_dvm/tasks/textextraction_pdf.py
--rw-r--r--   0 runner    (1001) docker     (127)     7781 2024-05-06 10:19:03.000000 nostr_dvm-0.3.5/nostr_dvm/tasks/textextraction_whisperx.py
--rw-r--r--   0 runner    (1001) docker     (127)     4320 2024-05-06 10:19:03.000000 nostr_dvm-0.3.5/nostr_dvm/tasks/textgeneration_huggingchat.py
--rw-r--r--   0 runner    (1001) docker     (127)     4985 2024-05-06 10:19:03.000000 nostr_dvm-0.3.5/nostr_dvm/tasks/textgeneration_llmlite.py
--rw-r--r--   0 runner    (1001) docker     (127)     4664 2024-05-06 10:19:03.000000 nostr_dvm-0.3.5/nostr_dvm/tasks/textgeneration_unleashed_chat.py
--rw-r--r--   0 runner    (1001) docker     (127)     6897 2024-05-06 10:19:03.000000 nostr_dvm-0.3.5/nostr_dvm/tasks/texttospeech.py
--rw-r--r--   0 runner    (1001) docker     (127)     7004 2024-05-06 10:19:03.000000 nostr_dvm-0.3.5/nostr_dvm/tasks/translation_google.py
--rw-r--r--   0 runner    (1001) docker     (127)     6895 2024-05-06 10:19:03.000000 nostr_dvm-0.3.5/nostr_dvm/tasks/translation_libretranslate.py
--rw-r--r--   0 runner    (1001) docker     (127)     5571 2024-05-06 10:19:03.000000 nostr_dvm-0.3.5/nostr_dvm/tasks/videogeneration_replicate_svd.py
--rw-r--r--   0 runner    (1001) docker     (127)     4892 2024-05-06 10:19:03.000000 nostr_dvm-0.3.5/nostr_dvm/tasks/videogeneration_svd.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 10:19:10.296576 nostr_dvm-0.3.5/nostr_dvm/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 10:19:03.000000 nostr_dvm-0.3.5/nostr_dvm/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4334 2024-05-06 10:19:03.000000 nostr_dvm-0.3.5/nostr_dvm/utils/admin_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8745 2024-05-06 10:19:03.000000 nostr_dvm-0.3.5/nostr_dvm/utils/backend_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6163 2024-05-06 10:19:03.000000 nostr_dvm-0.3.5/nostr_dvm/utils/cashu_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     9473 2024-05-06 10:19:03.000000 nostr_dvm-0.3.5/nostr_dvm/utils/database_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2700 2024-05-06 10:19:03.000000 nostr_dvm-0.3.5/nostr_dvm/utils/definitions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2387 2024-05-06 10:19:03.000000 nostr_dvm-0.3.5/nostr_dvm/utils/dvmconfig.py
--rw-r--r--   0 runner    (1001) docker     (127)     2761 2024-05-06 10:19:03.000000 nostr_dvm-0.3.5/nostr_dvm/utils/external_dvm_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    13403 2024-05-06 10:19:03.000000 nostr_dvm-0.3.5/nostr_dvm/utils/mediasource_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8866 2024-05-06 10:19:03.000000 nostr_dvm-0.3.5/nostr_dvm/utils/nip88_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4170 2024-05-06 10:19:03.000000 nostr_dvm-0.3.5/nostr_dvm/utils/nip89_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8449 2024-05-06 10:19:03.000000 nostr_dvm-0.3.5/nostr_dvm/utils/nostr_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3795 2024-05-06 10:19:03.000000 nostr_dvm-0.3.5/nostr_dvm/utils/nwc_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     9011 2024-05-06 10:19:03.000000 nostr_dvm-0.3.5/nostr_dvm/utils/output_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 10:19:10.300576 nostr_dvm-0.3.5/nostr_dvm/utils/scrapper/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 10:19:03.000000 nostr_dvm-0.3.5/nostr_dvm/utils/scrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    26119 2024-05-06 10:19:03.000000 nostr_dvm-0.3.5/nostr_dvm/utils/scrapper/media_scrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     5712 2024-05-06 10:19:03.000000 nostr_dvm-0.3.5/nostr_dvm/utils/subscription_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    15021 2024-05-06 10:19:03.000000 nostr_dvm-0.3.5/nostr_dvm/utils/zap_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 10:19:10.300576 nostr_dvm-0.3.5/nostr_dvm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-05-06 10:19:10.000000 nostr_dvm-0.3.5/nostr_dvm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4118 2024-05-06 10:19:10.000000 nostr_dvm-0.3.5/nostr_dvm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 10:19:10.000000 nostr_dvm-0.3.5/nostr_dvm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-05-06 10:19:10.000000 nostr_dvm-0.3.5/nostr_dvm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-06 10:19:10.000000 nostr_dvm-0.3.5/nostr_dvm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 10:19:10.300576 nostr_dvm-0.3.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-05-06 10:19:03.000000 nostr_dvm-0.3.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 10:19:10.300576 nostr_dvm-0.3.5/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    12655 2024-05-06 10:19:03.000000 nostr_dvm-0.3.5/tests/test_dvm_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     3213 2024-05-06 10:19:03.000000 nostr_dvm-0.3.5/tests/test_events.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 08:31:17.680931 nostr_dvm-0.3.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-16 08:31:13.000000 nostr_dvm-0.3.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-05-16 08:31:17.680931 nostr_dvm-0.3.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-05-16 08:31:13.000000 nostr_dvm-0.3.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 08:31:17.660931 nostr_dvm-0.3.6/nostr_dvm/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 08:31:13.000000 nostr_dvm-0.3.6/nostr_dvm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 08:31:17.664931 nostr_dvm-0.3.6/nostr_dvm/backends/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 08:31:13.000000 nostr_dvm-0.3.6/nostr_dvm/backends/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 08:31:17.664931 nostr_dvm-0.3.6/nostr_dvm/backends/mlx/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 08:31:13.000000 nostr_dvm-0.3.6/nostr_dvm/backends/mlx/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 08:31:17.664931 nostr_dvm-0.3.6/nostr_dvm/backends/mlx/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 08:31:13.000000 nostr_dvm-0.3.6/nostr_dvm/backends/mlx/modules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 08:31:17.664931 nostr_dvm-0.3.6/nostr_dvm/backends/mlx/modules/stable_diffusion/
+-rw-r--r--   0 runner    (1001) docker     (127)     2945 2024-05-16 08:31:13.000000 nostr_dvm-0.3.6/nostr_dvm/backends/mlx/modules/stable_diffusion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2222 2024-05-16 08:31:13.000000 nostr_dvm-0.3.6/nostr_dvm/backends/mlx/modules/stable_diffusion/clip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-05-16 08:31:13.000000 nostr_dvm-0.3.6/nostr_dvm/backends/mlx/modules/stable_diffusion/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9892 2024-05-16 08:31:13.000000 nostr_dvm-0.3.6/nostr_dvm/backends/mlx/modules/stable_diffusion/model_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2300 2024-05-16 08:31:13.000000 nostr_dvm-0.3.6/nostr_dvm/backends/mlx/modules/stable_diffusion/sampler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2991 2024-05-16 08:31:13.000000 nostr_dvm-0.3.6/nostr_dvm/backends/mlx/modules/stable_diffusion/tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13685 2024-05-16 08:31:13.000000 nostr_dvm-0.3.6/nostr_dvm/backends/mlx/modules/stable_diffusion/unet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7773 2024-05-16 08:31:13.000000 nostr_dvm-0.3.6/nostr_dvm/backends/mlx/modules/stable_diffusion/vae.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 08:31:17.664931 nostr_dvm-0.3.6/nostr_dvm/backends/nova_server/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 08:31:13.000000 nostr_dvm-0.3.6/nostr_dvm/backends/nova_server/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 08:31:17.664931 nostr_dvm-0.3.6/nostr_dvm/backends/nova_server/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 08:31:13.000000 nostr_dvm-0.3.6/nostr_dvm/backends/nova_server/modules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 08:31:17.668931 nostr_dvm-0.3.6/nostr_dvm/backends/nova_server/modules/image_interrogator/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 08:31:13.000000 nostr_dvm-0.3.6/nostr_dvm/backends/nova_server/modules/image_interrogator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4906 2024-05-16 08:31:13.000000 nostr_dvm-0.3.6/nostr_dvm/backends/nova_server/modules/image_interrogator/image_interrogator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-05-16 08:31:13.000000 nostr_dvm-0.3.6/nostr_dvm/backends/nova_server/modules/image_interrogator/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 08:31:17.668931 nostr_dvm-0.3.6/nostr_dvm/backends/nova_server/modules/image_upscale/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 08:31:13.000000 nostr_dvm-0.3.6/nostr_dvm/backends/nova_server/modules/image_upscale/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6863 2024-05-16 08:31:13.000000 nostr_dvm-0.3.6/nostr_dvm/backends/nova_server/modules/image_upscale/image_upscale_realesrgan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7745 2024-05-16 08:31:13.000000 nostr_dvm-0.3.6/nostr_dvm/backends/nova_server/modules/image_upscale/inference_realesrgan.py
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-16 08:31:13.000000 nostr_dvm-0.3.6/nostr_dvm/backends/nova_server/modules/image_upscale/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 08:31:17.668931 nostr_dvm-0.3.6/nostr_dvm/backends/nova_server/modules/stablediffusionxl/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 08:31:13.000000 nostr_dvm-0.3.6/nostr_dvm/backends/nova_server/modules/stablediffusionxl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3319 2024-05-16 08:31:13.000000 nostr_dvm-0.3.6/nostr_dvm/backends/nova_server/modules/stablediffusionxl/lora.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6854 2024-05-16 08:31:13.000000 nostr_dvm-0.3.6/nostr_dvm/backends/nova_server/modules/stablediffusionxl/stablediffusionxl-img2img.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9229 2024-05-16 08:31:13.000000 nostr_dvm-0.3.6/nostr_dvm/backends/nova_server/modules/stablediffusionxl/stablediffusionxl.py
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-16 08:31:13.000000 nostr_dvm-0.3.6/nostr_dvm/backends/nova_server/modules/stablediffusionxl/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 08:31:17.668931 nostr_dvm-0.3.6/nostr_dvm/backends/nova_server/modules/whisperx/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 08:31:13.000000 nostr_dvm-0.3.6/nostr_dvm/backends/nova_server/modules/whisperx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-05-16 08:31:13.000000 nostr_dvm-0.3.6/nostr_dvm/backends/nova_server/modules/whisperx/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5250 2024-05-16 08:31:13.000000 nostr_dvm-0.3.6/nostr_dvm/backends/nova_server/modules/whisperx/whisperx_transcript.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4880 2024-05-16 08:31:13.000000 nostr_dvm-0.3.6/nostr_dvm/backends/nova_server/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39902 2024-05-16 08:31:13.000000 nostr_dvm-0.3.6/nostr_dvm/bot.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39377 2024-05-16 08:31:13.000000 nostr_dvm-0.3.6/nostr_dvm/dvm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 08:31:17.668931 nostr_dvm-0.3.6/nostr_dvm/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 08:31:13.000000 nostr_dvm-0.3.6/nostr_dvm/interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6126 2024-05-16 08:31:13.000000 nostr_dvm-0.3.6/nostr_dvm/interfaces/dvmtaskinterface.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23582 2024-05-16 08:31:13.000000 nostr_dvm-0.3.6/nostr_dvm/subscription.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 08:31:17.676931 nostr_dvm-0.3.6/nostr_dvm/tasks/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 08:31:13.000000 nostr_dvm-0.3.6/nostr_dvm/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8321 2024-05-16 08:31:13.000000 nostr_dvm-0.3.6/nostr_dvm/tasks/advanced_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7452 2024-05-16 08:31:13.000000 nostr_dvm-0.3.6/nostr_dvm/tasks/advanced_search_wine.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12451 2024-05-16 08:31:13.000000 nostr_dvm-0.3.6/nostr_dvm/tasks/content_discovery_currently_popular.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13154 2024-05-16 08:31:13.000000 nostr_dvm-0.3.6/nostr_dvm/tasks/content_discovery_currently_popular_followers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13270 2024-05-16 08:31:13.000000 nostr_dvm-0.3.6/nostr_dvm/tasks/content_discovery_currently_popular_topic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4049 2024-05-16 08:31:13.000000 nostr_dvm-0.3.6/nostr_dvm/tasks/convert_media.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7854 2024-05-16 08:31:13.000000 nostr_dvm-0.3.6/nostr_dvm/tasks/discovery_bot_farms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8189 2024-05-16 08:31:13.000000 nostr_dvm-0.3.6/nostr_dvm/tasks/discovery_censor_wot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8964 2024-05-16 08:31:13.000000 nostr_dvm-0.3.6/nostr_dvm/tasks/discovery_inactive_follows.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8995 2024-05-16 08:31:13.000000 nostr_dvm-0.3.6/nostr_dvm/tasks/discovery_nonfollowers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4474 2024-05-16 08:31:13.000000 nostr_dvm-0.3.6/nostr_dvm/tasks/discovery_trending_notes_nostrband.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6218 2024-05-16 08:31:13.000000 nostr_dvm-0.3.6/nostr_dvm/tasks/imagegeneration_openai_dalle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5968 2024-05-16 08:31:13.000000 nostr_dvm-0.3.6/nostr_dvm/tasks/imagegeneration_replicate_sdxl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6897 2024-05-16 08:31:13.000000 nostr_dvm-0.3.6/nostr_dvm/tasks/imagegeneration_sd21_mlx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8391 2024-05-16 08:31:13.000000 nostr_dvm-0.3.6/nostr_dvm/tasks/imagegeneration_sdxl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9045 2024-05-16 08:31:13.000000 nostr_dvm-0.3.6/nostr_dvm/tasks/imagegeneration_sdxlimg2img.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5281 2024-05-16 08:31:13.000000 nostr_dvm-0.3.6/nostr_dvm/tasks/imageinterrogator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5283 2024-05-16 08:31:13.000000 nostr_dvm-0.3.6/nostr_dvm/tasks/imageupscale.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8186 2024-05-16 08:31:13.000000 nostr_dvm-0.3.6/nostr_dvm/tasks/search_users.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6450 2024-05-16 08:31:13.000000 nostr_dvm-0.3.6/nostr_dvm/tasks/summarization_huggingchat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6945 2024-05-16 08:31:13.000000 nostr_dvm-0.3.6/nostr_dvm/tasks/summarization_unleashed_chat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6774 2024-05-16 08:31:13.000000 nostr_dvm-0.3.6/nostr_dvm/tasks/textextraction_google.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4514 2024-05-16 08:31:13.000000 nostr_dvm-0.3.6/nostr_dvm/tasks/textextraction_pdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7781 2024-05-16 08:31:13.000000 nostr_dvm-0.3.6/nostr_dvm/tasks/textextraction_whisperx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4320 2024-05-16 08:31:13.000000 nostr_dvm-0.3.6/nostr_dvm/tasks/textgeneration_huggingchat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4985 2024-05-16 08:31:13.000000 nostr_dvm-0.3.6/nostr_dvm/tasks/textgeneration_llmlite.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4664 2024-05-16 08:31:13.000000 nostr_dvm-0.3.6/nostr_dvm/tasks/textgeneration_unleashed_chat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6897 2024-05-16 08:31:13.000000 nostr_dvm-0.3.6/nostr_dvm/tasks/texttospeech.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7004 2024-05-16 08:31:13.000000 nostr_dvm-0.3.6/nostr_dvm/tasks/translation_google.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6895 2024-05-16 08:31:13.000000 nostr_dvm-0.3.6/nostr_dvm/tasks/translation_libretranslate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5571 2024-05-16 08:31:13.000000 nostr_dvm-0.3.6/nostr_dvm/tasks/videogeneration_replicate_svd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4892 2024-05-16 08:31:13.000000 nostr_dvm-0.3.6/nostr_dvm/tasks/videogeneration_svd.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 08:31:17.676931 nostr_dvm-0.3.6/nostr_dvm/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 08:31:13.000000 nostr_dvm-0.3.6/nostr_dvm/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4334 2024-05-16 08:31:13.000000 nostr_dvm-0.3.6/nostr_dvm/utils/admin_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8745 2024-05-16 08:31:13.000000 nostr_dvm-0.3.6/nostr_dvm/utils/backend_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6163 2024-05-16 08:31:13.000000 nostr_dvm-0.3.6/nostr_dvm/utils/cashu_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9473 2024-05-16 08:31:13.000000 nostr_dvm-0.3.6/nostr_dvm/utils/database_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2700 2024-05-16 08:31:13.000000 nostr_dvm-0.3.6/nostr_dvm/utils/definitions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2387 2024-05-16 08:31:13.000000 nostr_dvm-0.3.6/nostr_dvm/utils/dvmconfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2761 2024-05-16 08:31:13.000000 nostr_dvm-0.3.6/nostr_dvm/utils/external_dvm_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13403 2024-05-16 08:31:13.000000 nostr_dvm-0.3.6/nostr_dvm/utils/mediasource_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8866 2024-05-16 08:31:13.000000 nostr_dvm-0.3.6/nostr_dvm/utils/nip88_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4170 2024-05-16 08:31:13.000000 nostr_dvm-0.3.6/nostr_dvm/utils/nip89_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8449 2024-05-16 08:31:13.000000 nostr_dvm-0.3.6/nostr_dvm/utils/nostr_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3795 2024-05-16 08:31:13.000000 nostr_dvm-0.3.6/nostr_dvm/utils/nwc_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9011 2024-05-16 08:31:13.000000 nostr_dvm-0.3.6/nostr_dvm/utils/output_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 08:31:17.680931 nostr_dvm-0.3.6/nostr_dvm/utils/scrapper/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 08:31:13.000000 nostr_dvm-0.3.6/nostr_dvm/utils/scrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26119 2024-05-16 08:31:13.000000 nostr_dvm-0.3.6/nostr_dvm/utils/scrapper/media_scrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5712 2024-05-16 08:31:13.000000 nostr_dvm-0.3.6/nostr_dvm/utils/subscription_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15021 2024-05-16 08:31:13.000000 nostr_dvm-0.3.6/nostr_dvm/utils/zap_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 08:31:17.680931 nostr_dvm-0.3.6/nostr_dvm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-05-16 08:31:17.000000 nostr_dvm-0.3.6/nostr_dvm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4179 2024-05-16 08:31:17.000000 nostr_dvm-0.3.6/nostr_dvm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 08:31:17.000000 nostr_dvm-0.3.6/nostr_dvm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-05-16 08:31:17.000000 nostr_dvm-0.3.6/nostr_dvm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-16 08:31:17.000000 nostr_dvm-0.3.6/nostr_dvm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 08:31:17.680931 nostr_dvm-0.3.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-05-16 08:31:13.000000 nostr_dvm-0.3.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 08:31:17.680931 nostr_dvm-0.3.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    13764 2024-05-16 08:31:13.000000 nostr_dvm-0.3.6/tests/test_dvm_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3213 2024-05-16 08:31:13.000000 nostr_dvm-0.3.6/tests/test_events.py
```

### Comparing `nostr_dvm-0.3.5/LICENSE` & `nostr_dvm-0.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.5/PKG-INFO` & `nostr_dvm-0.3.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nostr-dvm
-Version: 0.3.5
+Version: 0.3.6
 Summary: A framework to build and run Nostr NIP90 Data Vending Machines
 Home-page: https://github.com/believethehype/nostrdvm
 Author: Believethehype
 Author-email: believethehypeonnostr@proton.me
 License: MIT
 Keywords: nostr,nip90,dvm,data vending machine
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `nostr_dvm-0.3.5/README.md` & `nostr_dvm-0.3.6/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 ## To get started:
 
 Create a new venv by running `"python -m venv venv"`
   - Place .env file (based on .env_example) in main folder.
   - Create a `LNbits` account on an accessible instance of your choice, enter one account's id and admin key (this account will create other accounts for the dvms)
   - the framework will then automatically create keys, nip89 tags and zapable NIP57 `lightning addresses` for your dvms in this file.
-  - Activate the venv by typing `".venv\Scripts\activate"` on Windows or `"source .venv/bin/activate"` otherwise
+  - Activate the venv by typing `".venv\Scripts\activate"` on Windows or `"source venv/bin/activate"` otherwise
   - pip install nostr-dvm
   - Run python3 main.py. (or check single examples in the example folder)
 
 In each task component DVM examples are already prepared. Feel free to play along with the existing ones.
 You can also add new tasks by using the interface, just like the existing tasks in the `tasks` folder.
 
 A `bot` is running by default that lists and communicates with the `DVMs` added to it,
```

### Comparing `nostr_dvm-0.3.5/nostr_dvm/backends/mlx/modules/stable_diffusion/__init__.py` & `nostr_dvm-0.3.6/nostr_dvm/backends/mlx/modules/stable_diffusion/__init__.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.5/nostr_dvm/backends/mlx/modules/stable_diffusion/clip.py` & `nostr_dvm-0.3.6/nostr_dvm/backends/mlx/modules/stable_diffusion/clip.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.5/nostr_dvm/backends/mlx/modules/stable_diffusion/config.py` & `nostr_dvm-0.3.6/nostr_dvm/backends/mlx/modules/stable_diffusion/config.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.5/nostr_dvm/backends/mlx/modules/stable_diffusion/model_io.py` & `nostr_dvm-0.3.6/nostr_dvm/backends/mlx/modules/stable_diffusion/model_io.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.5/nostr_dvm/backends/mlx/modules/stable_diffusion/sampler.py` & `nostr_dvm-0.3.6/nostr_dvm/backends/mlx/modules/stable_diffusion/sampler.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.5/nostr_dvm/backends/mlx/modules/stable_diffusion/tokenizer.py` & `nostr_dvm-0.3.6/nostr_dvm/backends/mlx/modules/stable_diffusion/tokenizer.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.5/nostr_dvm/backends/mlx/modules/stable_diffusion/unet.py` & `nostr_dvm-0.3.6/nostr_dvm/backends/mlx/modules/stable_diffusion/unet.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.5/nostr_dvm/backends/mlx/modules/stable_diffusion/vae.py` & `nostr_dvm-0.3.6/nostr_dvm/backends/mlx/modules/stable_diffusion/vae.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.5/nostr_dvm/backends/nova_server/modules/image_interrogator/image_interrogator.py` & `nostr_dvm-0.3.6/nostr_dvm/backends/nova_server/modules/image_interrogator/image_interrogator.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.5/nostr_dvm/backends/nova_server/modules/image_upscale/image_upscale_realesrgan.py` & `nostr_dvm-0.3.6/nostr_dvm/backends/nova_server/modules/image_upscale/image_upscale_realesrgan.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.5/nostr_dvm/backends/nova_server/modules/image_upscale/inference_realesrgan.py` & `nostr_dvm-0.3.6/nostr_dvm/backends/nova_server/modules/image_upscale/inference_realesrgan.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.5/nostr_dvm/backends/nova_server/modules/stablediffusionxl/lora.py` & `nostr_dvm-0.3.6/nostr_dvm/backends/nova_server/modules/stablediffusionxl/lora.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.5/nostr_dvm/backends/nova_server/modules/stablediffusionxl/stablediffusionxl-img2img.py` & `nostr_dvm-0.3.6/nostr_dvm/backends/nova_server/modules/stablediffusionxl/stablediffusionxl-img2img.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.5/nostr_dvm/backends/nova_server/modules/stablediffusionxl/stablediffusionxl.py` & `nostr_dvm-0.3.6/nostr_dvm/backends/nova_server/modules/stablediffusionxl/stablediffusionxl.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.5/nostr_dvm/backends/nova_server/modules/whisperx/whisperx_transcript.py` & `nostr_dvm-0.3.6/nostr_dvm/backends/nova_server/modules/whisperx/whisperx_transcript.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.5/nostr_dvm/backends/nova_server/utils.py` & `nostr_dvm-0.3.6/nostr_dvm/backends/nova_server/utils.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.5/nostr_dvm/bot.py` & `nostr_dvm-0.3.6/nostr_dvm/bot.py`

 * *Files 0% similar despite different names*

```diff
@@ -445,15 +445,17 @@
             print("[" + self.NAME + "] Zap received")
             try:
                 invoice_amount, zapped_event, sender, message, anon = parse_zap_event_tags(zap_event,
                                                                                            self.keys, self.NAME,
                                                                                            self.client, self.dvm_config)
 
                 etag = ""
-                for tag in zap_event.tags():
+                print(zap_event.tags())
+                print(zapped_event.tags())
+                for tag in zapped_event.tags():
                     if tag.as_vec()[0] == "e":
                         etag = tag.as_vec()[1]
 
                 user = get_or_add_user(self.dvm_config.DB, sender, client=self.client, config=self.dvm_config)
 
                 entry = next((x for x in self.job_list if x['event_id'] == etag), None)
                 print(entry)
```

### Comparing `nostr_dvm-0.3.5/nostr_dvm/dvm.py` & `nostr_dvm-0.3.6/nostr_dvm/dvm.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.5/nostr_dvm/interfaces/dvmtaskinterface.py` & `nostr_dvm-0.3.6/nostr_dvm/interfaces/dvmtaskinterface.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.5/nostr_dvm/subscription.py` & `nostr_dvm-0.3.6/nostr_dvm/subscription.py`

 * *Files 0% similar despite different names*

```diff
@@ -183,14 +183,16 @@
                     if nwc_event_id is None:
                         print("error zapping " + lud16)
                     else:
                         zapped_amount = zapped_amount + (splitted_amount * 1000)
                         print(str(zapped_amount) + "/" + str(overall_amount))
 
             if zapped_amount < overall_amount * 0.8:  # TODO how do we handle failed zaps for some addresses? we are ok with 80% for now
+            #if zapped_amount < int(zaps[0][3]):
+
                 success = False
             else:
                 success = True
                 # if no active subscription exists OR the subscription ended, pay
 
             return success
 
@@ -400,44 +402,47 @@
                                                                                        " ")))
             evt = EventBuilder.encrypted_direct_msg(keys, PublicKey.parse(subscription.subscriber),
                                                     message,
                                                     None).to_event(keys)
             send_event(evt, client=self.client, dvm_config=dvm_config)
 
         def check_subscriptions():
-            subscriptions = get_all_subscriptions_from_sql_table(dvm_config.DB)
+            try:
+                subscriptions = get_all_subscriptions_from_sql_table(dvm_config.DB)
 
-            for subscription in subscriptions:
-                if subscription.active:
-                    if subscription.end < Timestamp.now().as_secs():
-                        # We could directly zap, but let's make another check if our subscription expired
-                        subscription_status = nip88_has_active_subscription(
-                            PublicKey.parse(subscription.subscriber),
-                            subscription.tier_dtag, self.client, subscription.recipent)
-
-                        if subscription_status["expires"]:
-                            # if subscription expires, just note it as not active
-                            update_subscription_sql_table(dvm_config.DB, subscription_status["subscriptionId"],
-                                                          subscription.recipent,
-                                                          subscription.subscriber, subscription.nwc,
-                                                          subscription.cadence, subscription.amount,
-                                                          subscription.unit,
-                                                          subscription.begin, subscription.end,
-                                                          subscription.tier_dtag, subscription.zaps,
-                                                          subscription.recipe,
-                                                          False,
-                                                          Timestamp.now().as_secs(), subscription.tier)
-                        else:
-                            handle_subscription_renewal(subscription)
+                for subscription in subscriptions:
+                    if subscription.active:
+                        if subscription.end < Timestamp.now().as_secs():
+                            # We could directly zap, but let's make another check if our subscription expired
+                            subscription_status = nip88_has_active_subscription(
+                                PublicKey.parse(subscription.subscriber),
+                                subscription.tier_dtag, self.client, subscription.recipent)
 
-                else:
-                    handle_expired_subscription(subscription)
+                            if subscription_status["expires"]:
+                                # if subscription expires, just note it as not active
+                                update_subscription_sql_table(dvm_config.DB, subscription_status["subscriptionId"],
+                                                              subscription.recipent,
+                                                              subscription.subscriber, subscription.nwc,
+                                                              subscription.cadence, subscription.amount,
+                                                              subscription.unit,
+                                                              subscription.begin, subscription.end,
+                                                              subscription.tier_dtag, subscription.zaps,
+                                                              subscription.recipe,
+                                                              False,
+                                                              Timestamp.now().as_secs(), subscription.tier)
+                            else:
+                                handle_subscription_renewal(subscription)
+
+                    else:
+                        handle_expired_subscription(subscription)
 
-            print(str(Timestamp.now().as_secs()) + ": Checking " + str(
-                len(subscriptions)) + " Subscription entries..")
+                print(str(Timestamp.now().as_secs()) + ": Checking " + str(
+                    len(subscriptions)) + " Subscription entries..")
+            except Exception as e:
+                print(e)
 
         self.client.handle_notifications(NotificationHandler())
 
         try:
             while True:
                 time.sleep(60.0)
                 check_subscriptions()
```

### Comparing `nostr_dvm-0.3.5/nostr_dvm/tasks/advanced_search.py` & `nostr_dvm-0.3.6/nostr_dvm/tasks/advanced_search.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.5/nostr_dvm/tasks/advanced_search_wine.py` & `nostr_dvm-0.3.6/nostr_dvm/tasks/advanced_search_wine.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.5/nostr_dvm/tasks/content_discovery_currently_popular.py` & `nostr_dvm-0.3.6/nostr_dvm/tasks/content_discovery_currently_popular.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,28 +23,41 @@
 
 class DicoverContentCurrentlyPopular(DVMTaskInterface):
     KIND: Kind = EventDefinitions.KIND_NIP90_CONTENT_DISCOVERY
     TASK: str = "discover-content"
     FIX_COST: float = 0
     dvm_config: DVMConfig
     last_schedule: int
+    db_since = 3600
+    db_name = "db/nostr_recent_notes.db"
+    min_reactions = 2
+    personalized = False
+    result = ""
 
     def __init__(self, name, dvm_config: DVMConfig, nip89config: NIP89Config, nip88config: NIP88Config = None,
                  admin_config: AdminConfig = None, options=None):
         dvm_config.SCRIPT = os.path.abspath(__file__)
         super().__init__(name=name, dvm_config=dvm_config, nip89config=nip89config, nip88config=nip88config,
                          admin_config=admin_config, options=options)
 
+        self.request_form = {"jobID": "generic"}
+        opts = {
+            "max_results": 200,
+        }
+        self.request_form['options'] = json.dumps(opts)
+
         self.last_schedule = Timestamp.now().as_secs()
 
         use_logger = False
         if use_logger:
             init_logger(LogLevel.DEBUG)
 
         self.sync_db()
+        if not self.personalized:
+            self.result = self.calculate_result(self.request_form)
 
     def is_input_supported(self, tags, client=None, dvm_config=None):
         for tag in tags:
             if tag.as_vec()[0] == 'i':
                 input_value = tag.as_vec()[1]
                 input_type = tag.as_vec()[2]
                 if input_type != "text":
@@ -72,50 +85,60 @@
         options = {
             "max_results": max_results,
         }
         request_form['options'] = json.dumps(options)
         return request_form
 
     def process(self, request_form):
+        # if the dvm supports individual results, recalculate it every time for the request
+        if self.personalized:
+            return self.calculate_result(request_form)
+        # else return the result that gets updated once every scheduled update. In this case on database update.
+        else:
+            return self.result
+
+    def calculate_result(self, request_form):
         from nostr_sdk import Filter
         from types import SimpleNamespace
         ns = SimpleNamespace()
 
         options = DVMTaskInterface.set_options(request_form)
 
         opts = (Options().wait_for_send(False).send_timeout(timedelta(seconds=self.dvm_config.RELAY_TIMEOUT)))
         sk = SecretKey.from_hex(self.dvm_config.PRIVATE_KEY)
         keys = Keys.parse(sk.to_hex())
         signer = NostrSigner.keys(keys)
 
-        database = NostrDatabase.sqlite("db/nostr_recent_notes.db")
+        database = NostrDatabase.sqlite(self.db_name)
         cli = ClientBuilder().database(database).signer(signer).opts(opts).build()
 
         cli.add_relay("wss://relay.damus.io")
         cli.connect()
 
         # Negentropy reconciliation
         # Query events from database
-        timestamp_hour_ago = Timestamp.now().as_secs() - 3600
+        timestamp_hour_ago = Timestamp.now().as_secs() - self.db_since
         lasthour = Timestamp.from_secs(timestamp_hour_ago)
 
         filter1 = Filter().kind(definitions.EventDefinitions.KIND_NOTE).since(lasthour)
         events = cli.database().query([filter1])
         ns.finallist = {}
         for event in events:
             if event.created_at().as_secs() > timestamp_hour_ago:
-                ns.finallist[event.id().to_hex()] = 0
-                filt = Filter().kinds([definitions.EventDefinitions.KIND_ZAP, definitions.EventDefinitions.KIND_REPOST, definitions.EventDefinitions.KIND_REACTION, definitions.EventDefinitions.KIND_NOTE]).event(event.id()).since(lasthour)
+                filt = Filter().kinds([definitions.EventDefinitions.KIND_ZAP, definitions.EventDefinitions.KIND_REPOST,
+                                       definitions.EventDefinitions.KIND_REACTION,
+                                       definitions.EventDefinitions.KIND_NOTE]).event(event.id()).since(lasthour)
                 reactions = cli.database().query([filt])
-                ns.finallist[event.id().to_hex()] = len(reactions)
+                if len(reactions) >= self.min_reactions:
+                    ns.finallist[event.id().to_hex()] = len(reactions)
 
         result_list = []
         finallist_sorted = sorted(ns.finallist.items(), key=lambda x: x[1], reverse=True)[:int(options["max_results"])]
         for entry in finallist_sorted:
-            #print(EventId.parse(entry[0]).to_bech32() + "/" + EventId.parse(entry[0]).to_hex() + ": " + str(entry[1]))
+            # print(EventId.parse(entry[0]).to_bech32() + "/" + EventId.parse(entry[0]).to_hex() + ": " + str(entry[1]))
             e_tag = Tag.parse(["e", entry[0]])
             result_list.append(e_tag.as_vec())
 
         return json.dumps(result_list)
 
     def post_process(self, result, event):
         """Overwrite the interface function to return a social client readable format, if requested"""
@@ -131,40 +154,44 @@
     def schedule(self, dvm_config):
         if dvm_config.SCHEDULE_UPDATES_SECONDS == 0:
             return 0
         else:
             if Timestamp.now().as_secs() >= self.last_schedule + dvm_config.SCHEDULE_UPDATES_SECONDS:
                 self.sync_db()
                 self.last_schedule = Timestamp.now().as_secs()
+                self.result = self.calculate_result(self.request_form)
                 return 1
 
     def sync_db(self):
         opts = (Options().wait_for_send(False).send_timeout(timedelta(seconds=self.dvm_config.RELAY_TIMEOUT)))
         sk = SecretKey.from_hex(self.dvm_config.PRIVATE_KEY)
         keys = Keys.parse(sk.to_hex())
         signer = NostrSigner.keys(keys)
-        database = NostrDatabase.sqlite("db/nostr_recent_notes.db")
+        database = NostrDatabase.sqlite(self.db_name)
         cli = ClientBuilder().signer(signer).database(database).opts(opts).build()
 
         cli.add_relay("wss://relay.damus.io")
         cli.connect()
 
-        timestamp_hour_ago = Timestamp.now().as_secs() - 3600
+        timestamp_hour_ago = Timestamp.now().as_secs() - self.db_since
         lasthour = Timestamp.from_secs(timestamp_hour_ago)
 
-        filter1 = Filter().kinds([definitions.EventDefinitions.KIND_NOTE, definitions.EventDefinitions.KIND_REACTION, definitions.EventDefinitions.KIND_ZAP]).since(lasthour)  # Notes, reactions, zaps
+        filter1 = Filter().kinds([definitions.EventDefinitions.KIND_NOTE, definitions.EventDefinitions.KIND_REACTION,
+                                  definitions.EventDefinitions.KIND_ZAP]).since(lasthour)  # Notes, reactions, zaps
 
         # filter = Filter().author(keys.public_key())
-        print("Syncing Notes of last hour.. this might take a while..")
+        print("[" + self.dvm_config.IDENTIFIER + "] Syncing notes of the last " + str(
+            self.db_since) + " seconds.. this might take a while..")
         dbopts = NegentropyOptions().direction(NegentropyDirection.DOWN)
         cli.reconcile(filter1, dbopts)
         database.delete(Filter().until(Timestamp.from_secs(
-            Timestamp.now().as_secs() - 3600)))  # Clear old events so db doesnt get too full.
+            Timestamp.now().as_secs() - self.db_since)))  # Clear old events so db doesnt get too full.
 
-        print("Done Syncing Notes of Last hour.")
+        print(
+            "[" + self.dvm_config.IDENTIFIER + "] Done Syncing Notes of the last " + str(self.db_since) + " seconds..")
 
 
 # We build an example here that we can call by either calling this file directly from the main directory,
 # or by adding it to our playground. You can call the example and adjust it to your needs or redefine it in the
 # playground or elsewhere
 def build_example(name, identifier, admin_config):
     dvm_config = build_default_config(identifier)
@@ -180,14 +207,15 @@
     nip89info = {
         "name": name,
         "image": "https://image.nostr.build/b29b6ec4bf9b6184f69d33cb44862db0d90a2dd9a506532e7ba5698af7d36210.jpg",
         "about": "I show notes that are currently popular",
         "lud16": dvm_config.LN_ADDRESS,
         "encryptionSupported": True,
         "cashuAccepted": True,
+        "personalized": False,
         "amount": "free",
         "nip90Params": {
             "max_results": {
                 "required": False,
                 "values": [],
                 "description": "The number of maximum results to return (default currently 100)"
             }
@@ -219,14 +247,15 @@
         "name": name,
         "image": "https://image.nostr.build/b29b6ec4bf9b6184f69d33cb44862db0d90a2dd9a506532e7ba5698af7d36210.jpg",
         "about": "I show notes that are currently popular all over Nostr. I'm also used for testing subscriptions.",
         "lud16": dvm_config.LN_ADDRESS,
         "encryptionSupported": True,
         "cashuAccepted": True,
         "subscription": True,
+        "personalized": False,
         "nip90Params": {
             "max_results": {
                 "required": False,
                 "values": [],
                 "description": "The number of maximum results to return (default currently 100)"
             }
         }
@@ -249,17 +278,17 @@
     nip88config.PERK2DESC = "Support NostrDVM & NostrSDK development"
     nip88config.PAYMENT_VERIFIER_PUBKEY = "5b5c045ecdf66fb540bdf2049fe0ef7f1a566fa427a4fe50d400a011b65a3a7e"
 
     admin_config.UPDATE_PROFILE = False
     admin_config.REBROADCAST_NIP89 = False
     admin_config.REBROADCAST_NIP88 = False
 
-   # admin_config.FETCH_NIP88 = True
-   # admin_config.EVENTID = "63a791cdc7bf78c14031616963105fce5793f532bb231687665b14fb6d805fdb"
-   # admin_config.PRIVKEY = dvm_config.PRIVATE_KEY
+    # admin_config.FETCH_NIP88 = True
+    # admin_config.EVENTID = "63a791cdc7bf78c14031616963105fce5793f532bb231687665b14fb6d805fdb"
+    # admin_config.PRIVKEY = dvm_config.PRIVATE_KEY
 
     return DicoverContentCurrentlyPopular(name=name, dvm_config=dvm_config, nip89config=nip89config,
                                           nip88config=nip88config,
                                           admin_config=admin_config)
 
 
 if __name__ == '__main__':
```

### Comparing `nostr_dvm-0.3.5/nostr_dvm/tasks/content_discovery_currently_popular_followers.py` & `nostr_dvm-0.3.6/nostr_dvm/tasks/content_discovery_currently_popular_followers.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,14 +24,17 @@
 
 class DicoverContentCurrentlyPopularFollowers(DVMTaskInterface):
     KIND: Kind = EventDefinitions.KIND_NIP90_CONTENT_DISCOVERY
     TASK: str = "discover-content"
     FIX_COST: float = 0
     dvm_config: DVMConfig
     last_schedule: int
+    db_since = 2 * 3600
+    db_name = "db/nostr_recent_notes2.db"
+    min_reactions = 2
 
     def __init__(self, name, dvm_config: DVMConfig, nip89config: NIP89Config, nip88config: NIP88Config = None,
                  admin_config: AdminConfig = None, options=None):
         dvm_config.SCRIPT = os.path.abspath(__file__)
         super().__init__(name=name, dvm_config=dvm_config, nip89config=nip89config, nip88config=nip88config,
                          admin_config=admin_config, options=options)
 
@@ -90,65 +93,66 @@
         options = DVMTaskInterface.set_options(request_form)
         relaylimits = RelayLimits.disable()
         opts = (Options().wait_for_send(True).send_timeout(timedelta(seconds=self.dvm_config.RELAY_TIMEOUT)).relay_limits(relaylimits))
         sk = SecretKey.from_hex(self.dvm_config.PRIVATE_KEY)
         keys = Keys.parse(sk.to_hex())
         signer = NostrSigner.keys(keys)
 
-        database = NostrDatabase.sqlite("db/nostr_recent_notes2.db")
+        database = NostrDatabase.sqlite(self.db_name)
         cli = ClientBuilder().database(database).signer(signer).opts(opts).build()
         cli.add_relay("wss://relay.damus.io")
         cli.add_relay("wss://nos.lol")
         cli.add_relay("wss://pablof7z.nostr1.com")
 
         ropts = RelayOptions().ping(False)
         cli.add_relay_with_opts("wss://nostr.band", ropts)
 
         cli.connect()
 
         user = PublicKey.parse(options["user"])
         followers_filter = Filter().author(user).kinds([Kind(3)])
         followers = cli.get_events_of([followers_filter], timedelta(seconds=self.dvm_config.RELAY_TIMEOUT))
-        print(followers)
+        #print(followers)
 
         # Negentropy reconciliation
         # Query events from database
-        timestamp_hour_ago = Timestamp.now().as_secs() - 7200
+        timestamp_hour_ago = Timestamp.now().as_secs() - self.db_since
         lasthour = Timestamp.from_secs(timestamp_hour_ago)
 
 
         result_list = []
 
         if len(followers) > 0:
             newest = 0
             best_entry = followers[0]
             for entry in followers:
                 if entry.created_at().as_secs() > newest:
                     newest = entry.created_at().as_secs()
                     best_entry = entry
 
-            print(best_entry.as_json())
+            #print(best_entry.as_json())
             followings = []
             for tag in best_entry.tags():
                 if tag.as_vec()[0] == "p":
                     following = PublicKey.parse(tag.as_vec()[1])
                     followings.append(following)
 
             filter1 = Filter().kind(definitions.EventDefinitions.KIND_NOTE).authors(followings).since(lasthour)
             events = cli.database().query([filter1])
 
             ns.finallist = {}
             for event in events:
                 if event.created_at().as_secs() > timestamp_hour_ago:
-                    ns.finallist[event.id().to_hex()] = 0
                     filt = Filter().kinds(
                         [definitions.EventDefinitions.KIND_ZAP, definitions.EventDefinitions.KIND_REACTION, definitions.EventDefinitions.KIND_REPOST,
                          definitions.EventDefinitions.KIND_NOTE]).event(event.id()).since(lasthour)
                     reactions = cli.database().query([filt])
-                    ns.finallist[event.id().to_hex()] = len(reactions)
+                    if len(reactions) >= self.min_reactions:
+                        ns.finallist[event.id().to_hex()] = len(reactions)
+
 
 
             finallist_sorted = sorted(ns.finallist.items(), key=lambda x: x[1], reverse=True)[:int(options["max_results"])]
             for entry in finallist_sorted:
                 # print(EventId.parse(entry[0]).to_bech32() + "/" + EventId.parse(entry[0]).to_hex() + ": " + str(entry[1]))
                 e_tag = Tag.parse(["e", entry[0]])
                 result_list.append(e_tag.as_vec())
@@ -178,34 +182,34 @@
                 return 1
 
     def sync_db(self):
         opts = (Options().wait_for_send(False).send_timeout(timedelta(seconds=self.dvm_config.RELAY_TIMEOUT)))
         sk = SecretKey.from_hex(self.dvm_config.PRIVATE_KEY)
         keys = Keys.parse(sk.to_hex())
         signer = NostrSigner.keys(keys)
-        database = NostrDatabase.sqlite("db/nostr_recent_notes2.db")
+        database = NostrDatabase.sqlite(self.db_name)
         cli = ClientBuilder().signer(signer).database(database).opts(opts).build()
 
         cli.add_relay("wss://relay.damus.io")
         cli.connect()
 
-        timestamp_hour_ago = Timestamp.now().as_secs() - 7200
+        timestamp_hour_ago = Timestamp.now().as_secs() - self.db_since
         lasthour = Timestamp.from_secs(timestamp_hour_ago)
 
         filter1 = Filter().kinds([definitions.EventDefinitions.KIND_NOTE, definitions.EventDefinitions.KIND_REACTION,
                                   definitions.EventDefinitions.KIND_ZAP]).since(lasthour)  # Notes, reactions, zaps
 
         # filter = Filter().author(keys.public_key())
-        print("Syncing Notes.. this might take a while..")
+        print("[" + self.dvm_config.IDENTIFIER + "] Syncing notes of the last " + str(self.db_since) + " seconds.. this might take a while..")
         dbopts = NegentropyOptions().direction(NegentropyDirection.DOWN)
         cli.reconcile(filter1, dbopts)
         database.delete(Filter().until(Timestamp.from_secs(
-            Timestamp.now().as_secs() - 7200)))  # Clear old events so db doesnt get too full.
+            Timestamp.now().as_secs() - self.db_since)))  # Clear old events so db doesnt get too full.
 
-        print("Done Syncing Notes of Last hour.")
+        print("[" + self.dvm_config.IDENTIFIER + "] Done Syncing Notes of the last " + str(self.db_since) + " seconds..")
 
 
 # We build an example here that we can call by either calling this file directly from the main directory,
 # or by adding it to our playground. You can call the example and adjust it to your needs or redefine it in the
 # playground or elsewhere
 def build_example(name, identifier, admin_config):
     dvm_config = build_default_config(identifier)
@@ -221,14 +225,15 @@
     nip89info = {
         "name": name,
         "image": "https://image.nostr.build/d92652a6a07677e051d647dcf9f0f59e265299b3335a939d008183a911513f4a.jpg",
         "about": "I show notes that are currently popular from people you follow",
         "lud16": dvm_config.LN_ADDRESS,
         "encryptionSupported": True,
         "cashuAccepted": True,
+        "personalized": True,
         "amount": "free",
         "nip90Params": {
             "max_results": {
                 "required": False,
                 "values": [],
                 "description": "The number of maximum results to return (default currently 100)"
             }
@@ -259,14 +264,15 @@
     nip89info = {
         "name": name,
         "image": "https://image.nostr.build/b29b6ec4bf9b6184f69d33cb44862db0d90a2dd9a506532e7ba5698af7d36210.jpg",
         "about": "I show notes that are currently popular, just like the free DVM, I'm also used for testing subscriptions. (beta)",
         "lud16": dvm_config.LN_ADDRESS,
         "encryptionSupported": True,
         "cashuAccepted": True,
+        "personalized": True,
         "subscription": True,
         "nip90Params": {
             "max_results": {
                 "required": False,
                 "values": [],
                 "description": "The number of maximum results to return (default currently 100)"
             }
```

### Comparing `nostr_dvm-0.3.5/nostr_dvm/tasks/convert_media.py` & `nostr_dvm-0.3.6/nostr_dvm/tasks/convert_media.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.5/nostr_dvm/tasks/discovery_bot_farms.py` & `nostr_dvm-0.3.6/nostr_dvm/tasks/discovery_bot_farms.py`

 * *Files 4% similar despite different names*

```diff
@@ -51,15 +51,15 @@
     def create_request_from_nostr_event(self, event, client=None, dvm_config=None):
         self.dvm_config = dvm_config
         print(self.dvm_config.PRIVATE_KEY)
 
         request_form = {"jobID": event.id().to_hex()}
 
         # default values
-        search = "airdrop;@nostrich.house;just your average nostr enjoyer"
+        search = "airdrop;just your average nostr enjoyer" #;@nostrich.house;
         max_results = 500
 
         for tag in event.tags():
             if tag.as_vec()[0] == 'i':
                 input_type = tag.as_vec()[2]
                 if input_type == "text":
                     search = tag.as_vec()[1]
```

### Comparing `nostr_dvm-0.3.5/nostr_dvm/tasks/discovery_censor_wot.py` & `nostr_dvm-0.3.6/nostr_dvm/tasks/discovery_censor_wot.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.5/nostr_dvm/tasks/discovery_inactive_follows.py` & `nostr_dvm-0.3.6/nostr_dvm/tasks/discovery_inactive_follows.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.5/nostr_dvm/tasks/discovery_nonfollowers.py` & `nostr_dvm-0.3.6/nostr_dvm/tasks/discovery_nonfollowers.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.5/nostr_dvm/tasks/discovery_trending_notes_nostrband.py` & `nostr_dvm-0.3.6/nostr_dvm/tasks/discovery_trending_notes_nostrband.py`

 * *Files 0% similar despite different names*

```diff
@@ -67,15 +67,15 @@
             result_list = []
             i = 0
             if len(response_json["notes"]) > 0:
                 for note in response_json["notes"]:
                     i += 1
                     if i < 20:
                         e_tag = Tag.parse(["e", note["id"]])
-                        print(e_tag.as_vec())
+                        #print(e_tag.as_vec())
                         result_list.append(e_tag.as_vec())
                     else:
                         break
 
             return json.dumps(result_list)
 
         except Exception as e:
```

### Comparing `nostr_dvm-0.3.5/nostr_dvm/tasks/imagegeneration_openai_dalle.py` & `nostr_dvm-0.3.6/nostr_dvm/tasks/imagegeneration_openai_dalle.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.5/nostr_dvm/tasks/imagegeneration_replicate_sdxl.py` & `nostr_dvm-0.3.6/nostr_dvm/tasks/imagegeneration_replicate_sdxl.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.5/nostr_dvm/tasks/imagegeneration_sd21_mlx.py` & `nostr_dvm-0.3.6/nostr_dvm/tasks/imagegeneration_sd21_mlx.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.5/nostr_dvm/tasks/imagegeneration_sdxl.py` & `nostr_dvm-0.3.6/nostr_dvm/tasks/imagegeneration_sdxl.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.5/nostr_dvm/tasks/imagegeneration_sdxlimg2img.py` & `nostr_dvm-0.3.6/nostr_dvm/tasks/imagegeneration_sdxlimg2img.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.5/nostr_dvm/tasks/imageinterrogator.py` & `nostr_dvm-0.3.6/nostr_dvm/tasks/imageinterrogator.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.5/nostr_dvm/tasks/imageupscale.py` & `nostr_dvm-0.3.6/nostr_dvm/tasks/imageupscale.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.5/nostr_dvm/tasks/search_users.py` & `nostr_dvm-0.3.6/nostr_dvm/tasks/search_users.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 
 class SearchUser(DVMTaskInterface):
     KIND: Kind = EventDefinitions.KIND_NIP90_USER_SEARCH
     TASK: str = "search-user"
     FIX_COST: float = 0
     dvm_config: DVMConfig
     last_schedule: int = 0
+    db_name = "db/nostr_profiles.db"
 
     def __init__(self, name, dvm_config: DVMConfig, nip89config: NIP89Config, nip88config: NIP88Config = None,
                  admin_config: AdminConfig = None, options=None):
         dvm_config.SCRIPT = os.path.abspath(__file__)
         super().__init__(name=name, dvm_config=dvm_config, nip89config=nip89config, nip88config=nip88config,
                          admin_config=admin_config, options=options)
 
@@ -80,15 +81,15 @@
         options = DVMTaskInterface.set_options(request_form)
 
         opts = (Options().wait_for_send(False).send_timeout(timedelta(seconds=self.dvm_config.RELAY_TIMEOUT)))
         sk = SecretKey.from_hex(self.dvm_config.PRIVATE_KEY)
         keys = Keys.parse(sk.to_hex())
         signer = NostrSigner.keys(keys)
 
-        database = NostrDatabase.sqlite("db/nostr_profiles.db")
+        database = NostrDatabase.sqlite(self.db_name)
         cli = ClientBuilder().database(database).signer(signer).opts(opts).build()
 
         cli.add_relay("wss://relay.damus.io")
         # cli.add_relay("wss://atl.purplerelay.com")
         cli.connect()
 
         # Negentropy reconciliation
@@ -143,15 +144,15 @@
                 return 1
 
     def sync_db(self):
         opts = (Options().wait_for_send(False).send_timeout(timedelta(seconds=self.dvm_config.RELAY_TIMEOUT)))
         sk = SecretKey.from_hex(self.dvm_config.PRIVATE_KEY)
         keys = Keys.parse(sk.to_hex())
         signer = NostrSigner.keys(keys)
-        database = NostrDatabase.sqlite("db/nostr_profiles.db")
+        database = NostrDatabase.sqlite(self.db_name)
         cli = ClientBuilder().signer(signer).database(database).opts(opts).build()
 
         cli.add_relay("wss://relay.damus.io")
         cli.connect()
 
         filter1 = Filter().kind(Kind(0))
```

### Comparing `nostr_dvm-0.3.5/nostr_dvm/tasks/summarization_huggingchat.py` & `nostr_dvm-0.3.6/nostr_dvm/tasks/summarization_huggingchat.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.5/nostr_dvm/tasks/summarization_unleashed_chat.py` & `nostr_dvm-0.3.6/nostr_dvm/tasks/summarization_unleashed_chat.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.5/nostr_dvm/tasks/textextraction_google.py` & `nostr_dvm-0.3.6/nostr_dvm/tasks/textextraction_google.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.5/nostr_dvm/tasks/textextraction_pdf.py` & `nostr_dvm-0.3.6/nostr_dvm/tasks/textextraction_pdf.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.5/nostr_dvm/tasks/textextraction_whisperx.py` & `nostr_dvm-0.3.6/nostr_dvm/tasks/textextraction_whisperx.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.5/nostr_dvm/tasks/textgeneration_huggingchat.py` & `nostr_dvm-0.3.6/nostr_dvm/tasks/textgeneration_huggingchat.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.5/nostr_dvm/tasks/textgeneration_llmlite.py` & `nostr_dvm-0.3.6/nostr_dvm/tasks/textgeneration_llmlite.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.5/nostr_dvm/tasks/textgeneration_unleashed_chat.py` & `nostr_dvm-0.3.6/nostr_dvm/tasks/textgeneration_unleashed_chat.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.5/nostr_dvm/tasks/texttospeech.py` & `nostr_dvm-0.3.6/nostr_dvm/tasks/texttospeech.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.5/nostr_dvm/tasks/translation_google.py` & `nostr_dvm-0.3.6/nostr_dvm/tasks/translation_google.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.5/nostr_dvm/tasks/translation_libretranslate.py` & `nostr_dvm-0.3.6/nostr_dvm/tasks/translation_libretranslate.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.5/nostr_dvm/tasks/videogeneration_replicate_svd.py` & `nostr_dvm-0.3.6/nostr_dvm/tasks/videogeneration_replicate_svd.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.5/nostr_dvm/tasks/videogeneration_svd.py` & `nostr_dvm-0.3.6/nostr_dvm/tasks/videogeneration_svd.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.5/nostr_dvm/utils/admin_utils.py` & `nostr_dvm-0.3.6/nostr_dvm/utils/admin_utils.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.5/nostr_dvm/utils/backend_utils.py` & `nostr_dvm-0.3.6/nostr_dvm/utils/backend_utils.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.5/nostr_dvm/utils/cashu_utils.py` & `nostr_dvm-0.3.6/nostr_dvm/utils/cashu_utils.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.5/nostr_dvm/utils/database_utils.py` & `nostr_dvm-0.3.6/nostr_dvm/utils/database_utils.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.5/nostr_dvm/utils/definitions.py` & `nostr_dvm-0.3.6/nostr_dvm/utils/definitions.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.5/nostr_dvm/utils/dvmconfig.py` & `nostr_dvm-0.3.6/nostr_dvm/utils/dvmconfig.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.5/nostr_dvm/utils/external_dvm_utils.py` & `nostr_dvm-0.3.6/nostr_dvm/utils/external_dvm_utils.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.5/nostr_dvm/utils/mediasource_utils.py` & `nostr_dvm-0.3.6/nostr_dvm/utils/mediasource_utils.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.5/nostr_dvm/utils/nip88_utils.py` & `nostr_dvm-0.3.6/nostr_dvm/utils/nip88_utils.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.5/nostr_dvm/utils/nip89_utils.py` & `nostr_dvm-0.3.6/nostr_dvm/utils/nip89_utils.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.5/nostr_dvm/utils/nostr_utils.py` & `nostr_dvm-0.3.6/nostr_dvm/utils/nostr_utils.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.5/nostr_dvm/utils/nwc_tools.py` & `nostr_dvm-0.3.6/nostr_dvm/utils/nwc_tools.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.5/nostr_dvm/utils/output_utils.py` & `nostr_dvm-0.3.6/nostr_dvm/utils/output_utils.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.5/nostr_dvm/utils/scrapper/media_scrapper.py` & `nostr_dvm-0.3.6/nostr_dvm/utils/scrapper/media_scrapper.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.5/nostr_dvm/utils/subscription_utils.py` & `nostr_dvm-0.3.6/nostr_dvm/utils/subscription_utils.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.5/nostr_dvm/utils/zap_utils.py` & `nostr_dvm-0.3.6/nostr_dvm/utils/zap_utils.py`

 * *Files identical despite different names*

### Comparing `nostr_dvm-0.3.5/nostr_dvm.egg-info/PKG-INFO` & `nostr_dvm-0.3.6/nostr_dvm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nostr-dvm
-Version: 0.3.5
+Version: 0.3.6
 Summary: A framework to build and run Nostr NIP90 Data Vending Machines
 Home-page: https://github.com/believethehype/nostrdvm
 Author: Believethehype
 Author-email: believethehypeonnostr@proton.me
 License: MIT
 Keywords: nostr,nip90,dvm,data vending machine
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `nostr_dvm-0.3.5/nostr_dvm.egg-info/SOURCES.txt` & `nostr_dvm-0.3.6/nostr_dvm.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -42,14 +42,15 @@
 nostr_dvm/interfaces/__init__.py
 nostr_dvm/interfaces/dvmtaskinterface.py
 nostr_dvm/tasks/__init__.py
 nostr_dvm/tasks/advanced_search.py
 nostr_dvm/tasks/advanced_search_wine.py
 nostr_dvm/tasks/content_discovery_currently_popular.py
 nostr_dvm/tasks/content_discovery_currently_popular_followers.py
+nostr_dvm/tasks/content_discovery_currently_popular_topic.py
 nostr_dvm/tasks/convert_media.py
 nostr_dvm/tasks/discovery_bot_farms.py
 nostr_dvm/tasks/discovery_censor_wot.py
 nostr_dvm/tasks/discovery_inactive_follows.py
 nostr_dvm/tasks/discovery_nonfollowers.py
 nostr_dvm/tasks/discovery_trending_notes_nostrband.py
 nostr_dvm/tasks/imagegeneration_openai_dalle.py
```

### Comparing `nostr_dvm-0.3.5/setup.py` & `nostr_dvm-0.3.6/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.3.5'
+VERSION = '0.3.6'
 DESCRIPTION = 'A framework to build and run Nostr NIP90 Data Vending Machines'
 LONG_DESCRIPTION = ('A framework to build and run Nostr NIP90 Data Vending Machines. See the github repository for more information')
 
 # Setting up
 setup(
     name="nostr-dvm",
     version=VERSION,
```

### Comparing `nostr_dvm-0.3.5/tests/test_dvm_client.py` & `nostr_dvm-0.3.6/tests/test_dvm_client.py`

 * *Files 5% similar despite different names*

```diff
@@ -172,14 +172,43 @@
         client.add_relay(relay)
     client.connect()
     config = DVMConfig
     send_event(event, client=client, dvm_config=config)
     return event.as_json()
 
 
+def nostr_client_test_disovery(user, ptag):
+    keys = Keys.parse(check_and_set_private_key("test_client"))
+
+    relay_list = ["wss://relay.damus.io", "wss://blastr.f7z.xyz",
+                  ]
+
+    relaysTag = Tag.parse(relay_list)
+    alttag = Tag.parse(["alt", "This is a NIP90 DVM AI task to find content"])
+    paramTag = Tag.parse(["param", "user", user])
+    pTag = Tag.parse(["p", ptag])
+
+    tags = [relaysTag, alttag, paramTag, pTag]
+
+
+    event = EventBuilder(EventDefinitions.KIND_NIP90_CONTENT_DISCOVERY, str("Give me content"),
+                         tags).to_event(keys)
+
+    signer = NostrSigner.keys(keys)
+    client = Client(signer)
+    for relay in relay_list:
+        client.add_relay(relay)
+    ropts = RelayOptions().ping(False)
+    client.add_relay_with_opts("wss://nostr.band", ropts)
+    client.connect()
+    config = DVMConfig
+    send_event(event, client=client, dvm_config=config)
+    return event.as_json()
+
+
 def nostr_client_test_image_private(prompt, cashutoken):
     keys = Keys.parse(check_and_set_private_key("test_client"))
     receiver_keys = Keys.parse(check_and_set_private_key("replicate_sdxl"))
 
     relay_list = ["wss://relay.damus.io", "wss://blastr.f7z.xyz", "wss://relayable.org",
                   "wss://nostr-pub.wellorder.net"]
     i_tag = Tag.parse(["i", prompt, "text"])
@@ -240,16 +269,17 @@
 
     # nostr_client_test_translation("This is the result of the DVM in spanish", "text", "es", 20, 20)
     # nostr_client_test_translation("note1p8cx2dz5ss5gnk7c59zjydcncx6a754c0hsyakjvnw8xwlm5hymsnc23rs", "event", "es", 20,20)
     # nostr_client_test_translation("44a0a8b395ade39d46b9d20038b3f0c8a11168e67c442e3ece95e4a1703e2beb", "event", "zh", 20, 20)
     # nostr_client_test_image("a beautiful purple ostrich watching the sunset")
     # nostr_client_test_search_profile("dontbelieve")
     wot = ["99bb5591c9116600f845107d31f9b59e2f7c7e09a1ff802e84f1d43da557ca64"]
+    nostr_client_test_disovery("99bb5591c9116600f845107d31f9b59e2f7c7e09a1ff802e84f1d43da557ca64", "a21592a70ef9a00695efb3f7e816e17742d251559aff154b16d063a408bcd74d")
     #nostr_client_test_censor_filter(wot)
-    nostr_client_test_inactive_filter("99bb5591c9116600f845107d31f9b59e2f7c7e09a1ff802e84f1d43da557ca64")
+    #nostr_client_test_inactive_filter("99bb5591c9116600f845107d31f9b59e2f7c7e09a1ff802e84f1d43da557ca64")
 
     # nostr_client_test_tts("Hello, this is a test. Mic check one, two.")
 
     # cashutoken = "cashuAeyJ0b2tlbiI6W3sicHJvb2ZzIjpbeyJpZCI6InZxc1VRSVorb0sxOSIsImFtb3VudCI6MSwiQyI6IjAyNWU3ODZhOGFkMmExYTg0N2YxMzNiNGRhM2VhMGIyYWRhZGFkOTRiYzA4M2E2NWJjYjFlOTgwYTE1NGIyMDA2NCIsInNlY3JldCI6InQ1WnphMTZKMGY4UElQZ2FKTEg4V3pPck5rUjhESWhGa291LzVzZFd4S0U9In0seyJpZCI6InZxc1VRSVorb0sxOSIsImFtb3VudCI6NCwiQyI6IjAyOTQxNmZmMTY2MzU5ZWY5ZDc3MDc2MGNjZmY0YzliNTMzMzVmZTA2ZGI5YjBiZDg2Njg5Y2ZiZTIzMjVhYWUwYiIsInNlY3JldCI6IlRPNHB5WE43WlZqaFRQbnBkQ1BldWhncm44UHdUdE5WRUNYWk9MTzZtQXM9In0seyJpZCI6InZxc1VRSVorb0sxOSIsImFtb3VudCI6MTYsIkMiOiIwMmRiZTA3ZjgwYmMzNzE0N2YyMDJkNTZiMGI3ZTIzZTdiNWNkYTBhNmI3Yjg3NDExZWYyOGRiZDg2NjAzNzBlMWIiLCJzZWNyZXQiOiJHYUNIdHhzeG9HM3J2WWNCc0N3V0YxbU1NVXczK0dDN1RKRnVwOHg1cURzPSJ9XSwibWludCI6Imh0dHBzOi8vbG5iaXRzLmJpdGNvaW5maXhlc3RoaXMub3JnL2Nhc2h1L2FwaS92MS9ScDlXZGdKZjlxck51a3M1eVQ2SG5rIn1dfQ=="
     # nostr_client_test_image_private("a beautiful ostrich watching the sunset")
     class NotificationHandler(HandleNotification):
         def handle(self, relay_url, subscription_id, event: Event):
```

### Comparing `nostr_dvm-0.3.5/tests/test_events.py` & `nostr_dvm-0.3.6/tests/test_events.py`

 * *Files identical despite different names*

