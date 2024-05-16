# Comparing `tmp/osc_llm-0.1.4.tar.gz` & `tmp/osc_llm-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "osc_llm-0.1.4.tar", max compression
+gzip compressed data, was "osc_llm-0.1.5.tar", last modified: Thu May 16 10:39:00 2024, max compression
```

## Comparing `osc_llm-0.1.4.tar` & `osc_llm-0.1.5.tar`

### file list

```diff
@@ -1,45 +1,64 @@
--rw-r--r--   0        0        0     1809 2024-05-14 08:53:38.515299 osc_llm-0.1.4/README.md
--rw-r--r--   0        0        0      253 2024-04-30 00:21:10.635963 osc_llm-0.1.4/osc_llm/__init__.py
--rw-r--r--   0        0        0     6755 2024-05-14 06:47:02.440862 osc_llm-0.1.4/osc_llm/__main__.py
--rw-r--r--   0        0        0       51 2024-04-27 15:22:11.337904 osc_llm-0.1.4/osc_llm/architectures/__init__.py
--rw-r--r--   0        0        0     8714 2024-05-14 21:34:40.711264 osc_llm-0.1.4/osc_llm/architectures/transformer_decoder.py
--rw-r--r--   0        0        0     4618 2024-05-14 21:34:23.938634 osc_llm-0.1.4/osc_llm/chat.py
--rw-r--r--   0        0        0      178 2024-05-10 19:18:14.078967 osc_llm-0.1.4/osc_llm/chat_templates/__init__.py
--rw-r--r--   0        0        0     2381 2024-05-14 08:11:14.162668 osc_llm-0.1.4/osc_llm/chat_templates/base.py
--rw-r--r--   0        0        0     1243 2024-05-10 19:18:05.762999 osc_llm-0.1.4/osc_llm/chat_templates/chatglm.py
--rw-r--r--   0        0        0     1052 2024-05-10 15:02:28.353483 osc_llm-0.1.4/osc_llm/chat_templates/chatml.py
--rw-r--r--   0        0        0     2998 2024-05-12 01:07:05.171122 osc_llm-0.1.4/osc_llm/chat_templates/llama.py
--rw-r--r--   0        0        0     1314 2024-04-29 23:11:24.182541 osc_llm-0.1.4/osc_llm/config.py
--rw-r--r--   0        0        0       83 2024-04-29 23:43:54.288202 osc_llm-0.1.4/osc_llm/engines/__init__.py
--rw-r--r--   0        0        0     1951 2024-05-09 00:43:57.688337 osc_llm-0.1.4/osc_llm/engines/base.py
--rw-r--r--   0        0        0     4415 2024-05-12 02:14:14.779802 osc_llm-0.1.4/osc_llm/engines/v1.py
--rw-r--r--   0        0        0     4916 2024-04-30 14:10:25.104449 osc_llm-0.1.4/osc_llm/engines/v2.py
--rw-r--r--   0        0        0      742 2024-05-12 01:04:34.995436 osc_llm-0.1.4/osc_llm/layers/__init__.py
--rw-r--r--   0        0        0      650 2024-04-27 15:10:30.656849 osc_llm-0.1.4/osc_llm/layers/activation.py
--rw-r--r--   0        0        0     7100 2024-05-11 02:07:54.277363 osc_llm-0.1.4/osc_llm/layers/attention.py
--rw-r--r--   0        0        0      186 2024-04-27 15:17:53.918752 osc_llm-0.1.4/osc_llm/layers/dropout.py
--rw-r--r--   0        0        0     2238 2024-04-27 15:10:30.684848 osc_llm-0.1.4/osc_llm/layers/embedding.py
--rw-r--r--   0        0        0     7718 2024-05-13 03:52:36.763618 osc_llm-0.1.4/osc_llm/layers/feedforward.py
--rw-r--r--   0        0        0      336 2024-04-27 15:10:30.684848 osc_llm-0.1.4/osc_llm/layers/head.py
--rw-r--r--   0        0        0     2745 2024-04-27 15:10:30.684848 osc_llm-0.1.4/osc_llm/layers/kv_cache.py
--rw-r--r--   0        0        0     6023 2024-05-09 10:13:37.142379 osc_llm-0.1.4/osc_llm/layers/linear.py
--rw-r--r--   0        0        0      823 2024-04-27 15:10:30.688848 osc_llm-0.1.4/osc_llm/layers/normalization.py
--rw-r--r--   0        0        0      476 2024-05-11 02:36:34.029609 osc_llm-0.1.4/osc_llm/model_helpers/__init__.py
--rw-r--r--   0        0        0     5307 2024-05-14 06:30:15.939422 osc_llm-0.1.4/osc_llm/model_helpers/base.py
--rw-r--r--   0        0        0     2690 2024-05-12 00:37:30.862834 osc_llm-0.1.4/osc_llm/model_helpers/chatglm.py
--rw-r--r--   0        0        0     3054 2024-04-27 15:16:30.027073 osc_llm-0.1.4/osc_llm/model_helpers/llama.py
--rw-r--r--   0        0        0     8206 2024-05-10 14:25:45.437854 osc_llm-0.1.4/osc_llm/model_helpers/qwen.py
--rw-r--r--   0        0        0      139 2024-05-09 10:14:52.802794 osc_llm-0.1.4/osc_llm/quantizers/__init__.py
--rw-r--r--   0        0        0      717 2024-04-27 15:10:37.244808 osc_llm-0.1.4/osc_llm/quantizers/base.py
--rw-r--r--   0        0        0     8861 2024-04-27 15:33:29.096094 osc_llm-0.1.4/osc_llm/quantizers/int4.py
--rw-r--r--   0        0        0     3912 2024-05-09 10:18:30.539547 osc_llm-0.1.4/osc_llm/quantizers/int8.py
--rw-r--r--   0        0        0       74 2024-04-27 15:04:12.071947 osc_llm-0.1.4/osc_llm/samplers/__init__.py
--rw-r--r--   0        0        0      903 2024-04-27 15:04:12.079947 osc_llm-0.1.4/osc_llm/samplers/base.py
--rw-r--r--   0        0        0     1122 2024-05-09 11:29:40.084349 osc_llm-0.1.4/osc_llm/samplers/top_k.py
--rw-r--r--   0        0        0     1121 2024-04-27 15:04:12.083947 osc_llm-0.1.4/osc_llm/samplers/top_p.py
--rw-r--r--   0        0        0        0 2024-05-06 11:34:05.202914 osc_llm-0.1.4/osc_llm/servers/__init__.py
--rw-r--r--   0        0        0     7566 2024-05-14 21:01:20.596843 osc_llm-0.1.4/osc_llm/servers/openai.py
--rw-r--r--   0        0        0     8999 2024-05-12 02:11:06.295796 osc_llm-0.1.4/osc_llm/tokenizer.py
--rw-r--r--   0        0        0     7136 2024-05-14 21:02:58.383637 osc_llm-0.1.4/osc_llm/utils.py
--rw-r--r--   0        0        0      717 2024-05-14 20:58:22.477897 osc_llm-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     2791 1970-01-01 00:00:00.000000 osc_llm-0.1.4/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 10:39:00.087230 osc_llm-0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     2713 2024-05-16 10:39:00.087230 osc_llm-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1994 2024-05-16 10:38:50.000000 osc_llm-0.1.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 10:39:00.079230 osc_llm-0.1.5/osc_llm/
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2024-05-16 10:38:50.000000 osc_llm-0.1.5/osc_llm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6554 2024-05-16 10:38:50.000000 osc_llm-0.1.5/osc_llm/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 10:39:00.079230 osc_llm-0.1.5/osc_llm/architectures/
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-16 10:38:50.000000 osc_llm-0.1.5/osc_llm/architectures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8920 2024-05-16 10:38:50.000000 osc_llm-0.1.5/osc_llm/architectures/transformer_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4442 2024-05-16 10:38:50.000000 osc_llm-0.1.5/osc_llm/chat.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 10:39:00.079230 osc_llm-0.1.5/osc_llm/chat_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-05-16 10:38:50.000000 osc_llm-0.1.5/osc_llm/chat_templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2352 2024-05-16 10:38:50.000000 osc_llm-0.1.5/osc_llm/chat_templates/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-05-16 10:38:50.000000 osc_llm-0.1.5/osc_llm/chat_templates/chatglm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-05-16 10:38:50.000000 osc_llm-0.1.5/osc_llm/chat_templates/chatml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2961 2024-05-16 10:38:50.000000 osc_llm-0.1.5/osc_llm/chat_templates/llama.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-05-16 10:38:50.000000 osc_llm-0.1.5/osc_llm/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 10:39:00.079230 osc_llm-0.1.5/osc_llm/engines/
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-16 10:38:50.000000 osc_llm-0.1.5/osc_llm/engines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1996 2024-05-16 10:38:50.000000 osc_llm-0.1.5/osc_llm/engines/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4378 2024-05-16 10:38:50.000000 osc_llm-0.1.5/osc_llm/engines/v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4907 2024-05-16 10:38:50.000000 osc_llm-0.1.5/osc_llm/engines/v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5866 2024-05-16 10:38:50.000000 osc_llm-0.1.5/osc_llm/engines/v3.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 10:39:00.083230 osc_llm-0.1.5/osc_llm/layers/
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-05-16 10:38:50.000000 osc_llm-0.1.5/osc_llm/layers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2024-05-16 10:38:50.000000 osc_llm-0.1.5/osc_llm/layers/activation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7321 2024-05-16 10:38:50.000000 osc_llm-0.1.5/osc_llm/layers/attention.py
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-16 10:38:50.000000 osc_llm-0.1.5/osc_llm/layers/dropout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2213 2024-05-16 10:38:50.000000 osc_llm-0.1.5/osc_llm/layers/embedding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7529 2024-05-16 10:38:50.000000 osc_llm-0.1.5/osc_llm/layers/feedforward.py
+-rw-r--r--   0 runner    (1001) docker     (127)      328 2024-05-16 10:38:50.000000 osc_llm-0.1.5/osc_llm/layers/head.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2919 2024-05-16 10:38:50.000000 osc_llm-0.1.5/osc_llm/layers/kv_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5855 2024-05-16 10:38:50.000000 osc_llm-0.1.5/osc_llm/layers/linear.py
+-rw-r--r--   0 runner    (1001) docker     (127)      762 2024-05-16 10:38:50.000000 osc_llm-0.1.5/osc_llm/layers/normalization.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 10:39:00.083230 osc_llm-0.1.5/osc_llm/model_helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-05-16 10:38:50.000000 osc_llm-0.1.5/osc_llm/model_helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5375 2024-05-16 10:38:50.000000 osc_llm-0.1.5/osc_llm/model_helpers/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2840 2024-05-16 10:38:50.000000 osc_llm-0.1.5/osc_llm/model_helpers/chatglm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3020 2024-05-16 10:38:50.000000 osc_llm-0.1.5/osc_llm/model_helpers/llama.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8293 2024-05-16 10:38:50.000000 osc_llm-0.1.5/osc_llm/model_helpers/qwen.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 10:39:00.083230 osc_llm-0.1.5/osc_llm/quantizers/
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-05-16 10:38:50.000000 osc_llm-0.1.5/osc_llm/quantizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      690 2024-05-16 10:38:50.000000 osc_llm-0.1.5/osc_llm/quantizers/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8791 2024-05-16 10:38:50.000000 osc_llm-0.1.5/osc_llm/quantizers/int4.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4185 2024-05-16 10:38:50.000000 osc_llm-0.1.5/osc_llm/quantizers/int8.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 10:39:00.083230 osc_llm-0.1.5/osc_llm/samplers/
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-16 10:38:50.000000 osc_llm-0.1.5/osc_llm/samplers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      884 2024-05-16 10:38:50.000000 osc_llm-0.1.5/osc_llm/samplers/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-05-16 10:38:50.000000 osc_llm-0.1.5/osc_llm/samplers/top_k.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-05-16 10:38:50.000000 osc_llm-0.1.5/osc_llm/samplers/top_p.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 10:39:00.083230 osc_llm-0.1.5/osc_llm/servers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 10:38:50.000000 osc_llm-0.1.5/osc_llm/servers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7751 2024-05-16 10:38:50.000000 osc_llm-0.1.5/osc_llm/servers/openai.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8816 2024-05-16 10:38:50.000000 osc_llm-0.1.5/osc_llm/tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6842 2024-05-16 10:38:50.000000 osc_llm-0.1.5/osc_llm/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 10:39:00.083230 osc_llm-0.1.5/osc_llm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2713 2024-05-16 10:39:00.000000 osc_llm-0.1.5/osc_llm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1391 2024-05-16 10:39:00.000000 osc_llm-0.1.5/osc_llm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 10:39:00.000000 osc_llm-0.1.5/osc_llm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-16 10:39:00.000000 osc_llm-0.1.5/osc_llm.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-05-16 10:39:00.000000 osc_llm-0.1.5/osc_llm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-16 10:39:00.000000 osc_llm-0.1.5/osc_llm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      992 2024-05-16 10:38:50.000000 osc_llm-0.1.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 10:39:00.087230 osc_llm-0.1.5/setup.cfg
```

### Comparing `osc_llm-0.1.4/osc_llm/__main__.py` & `osc_llm-0.1.5/osc_llm/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from jsonargparse import CLI 
+from jsonargparse import CLI
 from .chat import main as chat_main
 from .servers.openai import main as openai_main
 from .model_helpers import get_supported_architectures
 from .model_helpers.base import HFModelHelper
 from .quantizers import Int8Quantizer, WeightOnlyInt4Quantizer
 from .tokenizer import Tokenizer
 from .config import registry
@@ -12,34 +12,40 @@
 from typing import Literal, Optional
 import json
 import torch
 from lightning_utilities.core.imports import RequirementCache
 import os
 
 
-
 _SAFETENSORS_AVAILABLE = RequirementCache("safetensors")
 
-def download_huggingface_model(repo_id: str, 
-                               save_dir: str = "./checkpoints",
-                               force_download: bool = True,
-                               access_token: Optional[str] = os.getenv("HF_TOKEN"),
-                               from_safetensors: bool = False):
-    
+
+def download_huggingface_model(
+    repo_id: str,
+    save_dir: str = "./checkpoints",
+    force_download: bool = True,
+    access_token: Optional[str] = os.getenv("HF_TOKEN"),
+    from_safetensors: bool = False,
+):
     directory = Path(save_dir, repo_id)
     if directory.exists():
         if not force_download:
-            msg.fail(f"Directory {directory} already exists. Use --force_download to re-download.", exits=1)
+            msg.fail(
+                f"Directory {directory} already exists. Use --force_download to re-download.",
+                exits=1,
+            )
         else:
             msg.info(f"Directory {directory} already exists. Re-downloading.")
             import shutil
+
             shutil.rmtree(directory)
     if not directory.exists():
-        directory.mkdir(parents=True)      
+        directory.mkdir(parents=True)
     from huggingface_hub import snapshot_download
+
     download_files = ["tokenizer*", "generation_config.json", "config.json"]
     if from_safetensors:
         if not _SAFETENSORS_AVAILABLE:
             raise ModuleNotFoundError(str(_SAFETENSORS_AVAILABLE))
         download_files.append("*.safetensors")
     else:
         download_files.append("*.bin*")
@@ -48,15 +54,15 @@
         repo_id,
         local_dir=directory,
         local_dir_use_symlinks=False,
         resume_download=True,
         allow_patterns=download_files,
         token=access_token,
     )
-    
+
     # convert safetensors to PyTorch binaries
     if from_safetensors:
         from safetensors import SafetensorError
         from safetensors.torch import load_file as safetensors_load
         import torch
 
         msg.info("Converting .safetensor files to PyTorch binaries (.bin)")
@@ -67,25 +73,26 @@
             except SafetensorError as e:
                 raise RuntimeError(f"{safetensor_path} is likely corrupted. Please try to re-download it.") from e
             msg.info(f"{safetensor_path} --> {bin_path}")
             torch.save(result, bin_path)
             os.remove(safetensor_path)
 
 
-
 def get_hf_model_helper(checkpoint_dir: str) -> HFModelHelper:
     config_path = Path(checkpoint_dir) / "config.json"
     with open(config_path, "r") as f:
         config = json.load(f)
     architecture = config["architectures"][0]
     allowed_architectures = get_supported_architectures()
     if architecture not in allowed_architectures:
-        msg.fail(title="Architecture {architecture} is not supported.",
-                 text=f"Supported architectures are: {allowed_architectures}", 
-                 exits=1)
+        msg.fail(
+            title="Architecture {architecture} is not supported.",
+            text=f"Supported architectures are: {allowed_architectures}",
+            exits=1,
+        )
     model_helper: HFModelHelper = registry.model_helpers.get(architecture)(checkpoint_dir)
     return model_helper
 
 
 def convert(checkpoint_dir: str, save_dir: Optional[str] = None):
     """Convert a huggingface checkpoint to osc_transformers checkpoint.
 
@@ -93,48 +100,50 @@
         checkpoint_dir: Path to the directory containing the checkpoint.
         save_dir: Path to the directory to save the converted checkpoint. if None, the converted checkpoint will be saved in the same directory as the original checkpoint.
     """
     model_helper = get_hf_model_helper(checkpoint_dir)
     if not save_dir:
         save_dir = checkpoint_dir
     model_helper.convert_checkpoint(save_dir=save_dir)
-    
-    
+
+
 def quantize_int8(checkpoint_dir: str, save_dir: str):
     """
     Quantize the osc model to int8.
-    
+
     Args:
         checkpoint_dir: Path to the osc model directory containing the checkpoint.
         save_dir: Path to the directory to save the quantized model.
     """
-    save_dir= Path(save_dir)
+    save_dir = Path(save_dir)
     if save_dir == checkpoint_dir:
         msg.warn("The quantized model will replace the original model.")
     if not save_dir.exists():
         save_dir.mkdir(parents=True)
     tokenizer = Tokenizer(checkpoint_dir=checkpoint_dir)
     model, config = build_from_checkpoint(checkpoint_dir=checkpoint_dir, return_config=True)
     quantizer = Int8Quantizer()
     model = quantizer.quantize(model)
     config = config.merge(quantizer.quantizer_config)
     torch.save(model.state_dict(), Path(save_dir) / "osc_model.pth")
     config.to_disk(Path(save_dir) / "config.cfg")
     tokenizer.save(save_dir)
-    
-    
-def quantize_int4(checkpoint_dir: str, 
-                  save_dir: str, 
-                  groupsize: Literal[32, 64, 128, 256] = 32, 
-                  k: Literal[2, 4, 8] = 8, 
-                  padding: bool = True, 
-                  device: str = 'cuda:0'):
+
+
+def quantize_int4(
+    checkpoint_dir: str,
+    save_dir: str,
+    groupsize: Literal[32, 64, 128, 256] = 32,
+    k: Literal[2, 4, 8] = 8,
+    padding: bool = True,
+    device: str = "cuda:0",
+):
     """
     Quantize the osc model to int4.
-    
+
     Args:
         checkpoint_dir: Path to the osc model directory containing the checkpoint.
         save_dir: Path to the directory to save the quantized model.
         groupsize: The groupsize to use for the quantization.
         k: The k parameter to use for the quantization.
         padding: Whether to pad the model.
         device: The device to use for the quantization.
@@ -151,31 +160,23 @@
     model = quantizer.quantize(model)
     config = config.merge(quantizer.quantizer_config)
     torch.save(model.state_dict(), Path(save_dir) / "osc_model.pth")
     config.to_disk(Path(save_dir) / "config.cfg")
     tokenizer.save(save_dir)
 
 
-
 commands = {
     "download": download_huggingface_model,
     "chat": chat_main,
-    "sft": {
-        "lora": lambda: print("lora"),
-        "full": lambda: print("full")
-    },
+    "sft": {"lora": lambda: print("lora"), "full": lambda: print("full")},
     "convert": convert,
-    "quantize": {
-        "int8": quantize_int8,
-        "int4": quantize_int4
-    },
-    "serve": openai_main
+    "quantize": {"int8": quantize_int8, "int4": quantize_int4},
+    "serve": openai_main,
 }
 
 
-
 def run():
     CLI(components=commands, as_positional=False)
-    
-    
+
+
 if __name__ == "__main__":
-    run()
+    run()
```

### Comparing `osc_llm-0.1.4/osc_llm/architectures/transformer_decoder.py` & `osc_llm-0.1.5/osc_llm/architectures/transformer_decoder.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,204 +2,250 @@
 from ..layers.kv_cache import KVCache, StaticKVCache
 import torch.nn as nn
 from typing import Mapping, Optional, Tuple, List, Any
 import torch
 from copy import deepcopy
 
 
-RoPECache = Tuple[torch.Tensor, torch.Tensor]
-
-
 class TransformerDecoderBlock(nn.Module):
     def __init__(
         self,
         attention: nn.Module,
         attention_norm: nn.Module,
         feedforward: nn.Module,
         feedforward_norm: nn.Module,
-        prenorm: bool = True
+        prenorm: bool = True,
     ):
         super().__init__()
         self.attention = attention
         self.attention_norm = attention_norm
         self.feedforward = feedforward
         self.feedforward_norm = feedforward_norm
         self.prenorm = prenorm
-        
+
     def forward(
         self,
         x,
         input_pos: Optional[torch.Tensor] = None,
         attention_mask: Optional[torch.Tensor] = None,
         cos: Optional[torch.Tensor] = None,
         sin: Optional[torch.Tensor] = None,
     ):
         if self.prenorm:
-            x = self.attention(self.attention_norm(x), input_pos=input_pos, attention_mask=attention_mask, cos=cos, sin=sin) + x
+            x = (
+                self.attention(
+                    self.attention_norm(x),
+                    input_pos=input_pos,
+                    attention_mask=attention_mask,
+                    cos=cos,
+                    sin=sin,
+                )
+                + x
+            )
             x = x + self.feedforward(self.feedforward_norm(x))
         else:
-            x = self.attention_norm(self.attention(x, input_pos=input_pos, attention_mask=attention_mask, sin=sin, cos=cos) + x)
+            x = self.attention_norm(
+                self.attention(
+                    x,
+                    input_pos=input_pos,
+                    attention_mask=attention_mask,
+                    sin=sin,
+                    cos=cos,
+                )
+                + x
+            )
             x = self.feedforward_norm(self.feedforward(x) + x)
-        return x 
-    
-    
+        return x
+
+
 @registry.architectures.register("TransformerDecoder")
 class TransformerDecoder(nn.Module):
-    def __init__(self, 
-                 n_blocks: int,
-                 block_size: int,
-                 embedding: nn.Module,
-                 attention: nn.Module,
-                 feedforward: nn.Module,
-                 head: nn.Module,
-                 norm: nn.Module,
-                 prenorm: bool,
-                 rope_base: int = 10000,
-                 kv_cache: Optional[KVCache] = None):
+    def __init__(
+        self,
+        n_blocks: int,
+        block_size: int,
+        embedding: nn.Module,
+        attention: nn.Module,
+        feedforward: nn.Module,
+        head: nn.Module,
+        norm: nn.Module,
+        prenorm: bool,
+        rope_base: int = 10000,
+        kv_cache: Optional[KVCache] = None,
+    ):
         super().__init__()
-        
+
         self.prenorm = prenorm
         self.n_blocks = n_blocks
         self.embedding = embedding
         self.blocks = nn.ModuleList(
-            [TransformerDecoderBlock(attention=deepcopy(attention), attention_norm=deepcopy(norm), feedforward=deepcopy(feedforward), feedforward_norm=deepcopy(norm), prenorm=prenorm) for _ in range(n_blocks)]
+            [
+                TransformerDecoderBlock(
+                    attention=deepcopy(attention),
+                    attention_norm=deepcopy(norm),
+                    feedforward=deepcopy(feedforward),
+                    feedforward_norm=deepcopy(norm),
+                    prenorm=prenorm,
+                )
+                for _ in range(n_blocks)
+            ]
         )
         self.head_norm = norm if self.prenorm else None
         self.head = head
         self.rope_base = rope_base
-        
+
         self.block_size = block_size
         self.max_length = block_size
-        
+
         self.mask_cache: Optional[torch.Tensor] = None
-        
+
         if kv_cache:
             self.kv_caches = [deepcopy(kv_cache) for _ in range(n_blocks)]
-        
+
     @property
     def kv_caches(self) -> List[KVCache]:
         return [block.attention.kv_cache for block in self.blocks]
-    
+
     @kv_caches.setter
     def kv_caches(self, value: List[KVCache]):
         assert len(value) == len(self.blocks), "Number of kv_caches must match number of blocks"
         for block, kv_cache in zip(self.blocks, value):
             block.attention.kv_cache = kv_cache
-            
+
     @property
     def max_length(self) -> int:
         return self._max_length
-    
+
     @max_length.setter
     def max_length(self, value: int):
         self._max_length = value
         if self.rope_base:
             if not hasattr(self, "cos") or not hasattr(self, "sin"):
                 self.setup_rope_cache(max_length=value)
             elif self.cos.size(0) != value:
                 self.setup_rope_cache(max_length=value, device=self.cos.device)
-      
+
     def reset_parameters(self) -> None:
         # Trigger resetting the rope-cache
         self.max_seq_length = self.block_size
-        
-    def setup_kv_cache(self, 
-                     batch_size: int, 
-                     max_length: Optional[int] = None, 
-                     kv_cache: Optional[KVCache] = None,
-                     device: Optional[torch.device] = None, 
-                     dtype: Optional[torch.dtype] = None):
+
+    def setup_kv_cache(
+        self,
+        batch_size: int,
+        max_length: Optional[int] = None,
+        kv_cache: Optional[KVCache] = None,
+        device: Optional[torch.device] = None,
+        dtype: Optional[torch.dtype] = None,
+    ):
         if kv_cache:
             assert isinstance(kv_cache, KVCache), "kv_cache must be an instance of KVCache"
         else:
             kv_cache = StaticKVCache()
         self.kv_caches = [deepcopy(kv_cache) for _ in range(self.n_blocks)]
         if not max_length:
             max_length = self.block_size
         else:
             assert max_length <= self.block_size, "max_length must be less than or equal to block_size"
-            
+
         for block in self.blocks:
-            block.attention.setup_kv_cache(batch_size=batch_size, max_seq_length=max_length, device=device, dtype=dtype)
-        
-        self.mask_cache = torch.tril(torch.ones((max_length, max_length), device=device, dtype=torch.bool)).unsqueeze(0).unsqueeze(0)
+            block.attention.setup_kv_cache(
+                batch_size=batch_size,
+                max_seq_length=max_length,
+                device=device,
+                dtype=dtype,
+            )
+
+        self.mask_cache = (
+            torch.tril(torch.ones((max_length, max_length), device=device, dtype=torch.bool)).unsqueeze(0).unsqueeze(0)
+        )
 
     def setup_rope_cache(self, max_length: int, device: Optional[torch.device] = None) -> None:
         head_size = self.blocks[0].attention.head_size
-        cos, sin = build_rope_cache(seq_len=max_length, 
-                                    n_elem=head_size, 
-                                    dtype=torch.get_default_dtype(), 
-                                    base=self.rope_base,
-                                    device=device)
+        cos, sin = build_rope_cache(
+            seq_len=max_length,
+            n_elem=head_size,
+            dtype=torch.get_default_dtype(),
+            base=self.rope_base,
+            device=device,
+        )
         self.register_buffer("cos", cos, persistent=False)
         self.register_buffer("sin", sin, persistent=False)
 
-        
     def forward(self, input_ids: torch.Tensor, input_pos: Optional[torch.Tensor] = None):
         """Forward pass of the TransformerDecoder.
 
         Args:
             input_ids (torch.Tensor): Input token ids. shape = (batch_size, seq_length)
             input_pos (Optional[torch.Tensor], optional): Input position ids. prefill stage shape = (batch_size, seq_length) decode stage shape = (batch_size, 1). Defaults to None.
         """
-        
+
         B, L = input_ids.size()
-        
+
         if self.max_length < L:
             raise ValueError(f"Cannot forward sequence of length {L}, max seq length is only {self.max_seq_length}.")
 
         if input_pos is not None:
             # use rope cache
             cos = self.cos.index_select(0, input_pos)
             sin = self.sin.index_select(0, input_pos)
-            
+
             if self.mask_cache is None:
                 raise TypeError("You need to call `model.setup_kv_cache()`")
             mask = self.mask_cache.index_select(2, input_pos)
         else:
             cos = self.cos[:L]
             sin = self.sin[:L]
             mask = None
-            
+
         x = self.embedding(input_ids)
-        
+
         for block in self.blocks:
             x = block(x, input_pos=input_pos, cos=cos, sin=sin, attention_mask=mask)
-            
+
         if self.prenorm:
             x = self.head_norm(x)
-            
+
         x = self.head(x)
-        
+
         return x
-    
+
     def load_state_dict(self, state_dict: Mapping[str, Any], strict: bool = True, assign: bool = True):
         # 保证在用torch.device('meta')构建模型后, 可以运行model.to('cuda:xxx'),不然会由于cos和sin是meta data而报错
         self.setup_rope_cache(max_length=self.max_length)
         return super().load_state_dict(state_dict, strict, assign)
-    
+
     def model_size(self, include_embeddings: bool = True) -> int:
         """Calculate the model size.
 
         Args:
             include_embeddings (bool, optional): Include embeddings in the model size. Defaults to True.
 
         Returns:
             int: Model size
         """
         import itertools
+
         model_size = 0
         for n, children in self.named_children():
             if n == "embedding" and not include_embeddings:
                 continue
-            model_size += sum([p.numel() * p.dtype.itemsize for p in itertools.chain(children.parameters(), children.buffers())])
+            model_size += sum(
+                [p.numel() * p.dtype.itemsize for p in itertools.chain(children.parameters(), children.buffers())]
+            )
         return model_size
-            
-    
-def build_rope_cache(seq_len: int, n_elem: int, dtype: torch.dtype, device: torch.device, base: int = 10000, condense_ratio: int = 1) -> RoPECache:
+
+
+def build_rope_cache(
+    seq_len: int,
+    n_elem: int,
+    dtype: torch.dtype,
+    device: torch.device,
+    base: int = 10000,
+    condense_ratio: int = 1,
+) -> Tuple[torch.Tensor, torch.Tensor]:
     """Enhanced Transformer with Rotary Position Embedding.
 
     Derived from: https://github.com/labmlai/annotated_deep_learning_paper_implementations/blob/master/labml_nn/
     transformers/rope/__init__.py. MIT License:
     https://github.com/labmlai/annotated_deep_learning_paper_implementations/blob/master/license.
     """
     # $\Theta = {\theta_i = 10000^{\frac{2(i-1)}{d}}, i \in [1, 2, ..., \frac{d}{2}]}$
@@ -209,8 +255,8 @@
     seq_idx = torch.arange(seq_len, device=device) / condense_ratio
 
     # Calculate the product of position index and $\theta_i$
     idx_theta = torch.outer(seq_idx, theta).repeat(1, 2)
 
     cos, sin = torch.cos(idx_theta), torch.sin(idx_theta)
 
-    return cos, sin
+    return cos, sin
```

### Comparing `osc_llm-0.1.4/osc_llm/chat.py` & `osc_llm-0.1.5/osc_llm/chat.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,28 +4,27 @@
 from .engines import LLMEngineV1, LLMEngine, LLMEngineV2
 import torch
 import time
 from pathlib import Path
 from typing import Optional, Literal
 
 
+torch.set_float32_matmul_precision("high")
 
-torch.set_float32_matmul_precision('high')
-    
 
 @torch.inference_mode()
 def main(
     checkpoint_dir: str,
     device: int = 0,
     temperature: float = 1.0,
     top_k: int = 200,
     max_length: Optional[int] = None,
     compile: bool = False,
     multi_turn: bool = False,
-    engine: Literal["v1", "v2"] = "v1"
+    engine: Literal["v1", "v2"] = "v1",
 ):
     """chat with llm
 
     Args:
         checkpoint_dir (str): the directory of the model checkpoint
         device (int, optional): which gpu to use. Defaults to 0.
         temperature (float, optional): the temperature of the sampling. Defaults to 1.0.
@@ -36,73 +35,81 @@
         multi_turn (bool, optional): whether to use multi-turn chat. Defaults to False.
         engine (Literal["v1", "v2"], optional): which engine to use. Defaults to "v1".
     """
     checkpoint_dir: Path = Path(checkpoint_dir)
     tokenizer = Tokenizer(checkpoint_dir=checkpoint_dir)
     sampler = TopK(k=top_k, temperature=temperature)
     if engine == "v1":
-        engine: LLMEngine = LLMEngineV1(checkpoint_dir=checkpoint_dir,
-                                        sampler=sampler,
-                                        max_length=max_length,
-                                        devices=[device],
-                                        compile=compile)
+        engine: LLMEngine = LLMEngineV1(
+            checkpoint_dir=checkpoint_dir,
+            sampler=sampler,
+            max_length=max_length,
+            devices=[device],
+            compile=compile,
+        )
     elif engine == "v2":
-        engine: LLMEngine = LLMEngineV2(checkpoint_dir=checkpoint_dir,
-                                        sampler=sampler,
-                                        max_length=max_length,
-                                        devices=[device],
-                                        compile=compile)
+        engine: LLMEngine = LLMEngineV2(
+            checkpoint_dir=checkpoint_dir,
+            sampler=sampler,
+            max_length=max_length,
+            devices=[device],
+            compile=compile,
+        )
     engine.setup()
-    
+
     if not hasattr(engine, "decode_model"):
         model_size = engine.model.model_size(include_embeddings=False)
     else:
-        model_size = engine.decode_model.model_size(include_embeddings=False) + engine.prefill_model.model_size(include_embeddings=False)
-    
+        model_size = engine.decode_model.model_size(include_embeddings=False) + engine.prefill_model.model_size(
+            include_embeddings=False
+        )
+
     if compile:
         t = time.perf_counter()
-        input_ids = tokenizer.encode_messages([Message(role='user', content="你好")])
+        input_ids = tokenizer.encode_messages([Message(role="user", content="你好")])
         stream = engine.run(input_ids=input_ids, stop_ids=tokenizer.stop_ids)
         token_stream = tokenizer.decode_stream(stream=stream)
         for token in token_stream:
             pass
         engine.fabric.print(f"Time for warmup: {time.perf_counter() - t:.2f} seconds")
         engine.fabric.print("\n")
 
     messages = []
-    pre_ids_len = 0 # 多轮对话过程中,对之前的对话历史做一个缓存,这样避免在prefill阶段重新kv cache
+    pre_ids_len = 0  # 多轮对话过程中,对之前的对话历史做一个缓存,这样避免在prefill阶段重新kv cache
     while True:
         content = input("User (empty to exit): ")
         if content == "":
             break
-        
-        messages.append(Message(role='user', content=content))
+
+        messages.append(Message(role="user", content=content))
         input_ids = tokenizer.encode_messages(messages)
         with engine.fabric.init_tensor():
             input_pos = torch.arange(pre_ids_len, len(input_ids))
         input_ids = input_ids[pre_ids_len:]
-        
+
         stream = engine.run(input_ids=input_ids, stop_ids=tokenizer.stop_ids, input_pos=input_pos)
         generated_text = ""
         engine.fabric.print("Assistant: ")
         time0 = time.perf_counter()
         token_stream = tokenizer.decode_stream(stream=stream)
         for token in token_stream:
-            print(token, end='', flush=True)
+            print(token, end="", flush=True)
             generated_text += token
         time1 = time.perf_counter()
         t = time1 - time0
         num_new_tokens = len(tokenizer.encode(generated_text).tolist())
         tokens_sec = num_new_tokens / t
-        
+
         if multi_turn:
-            messages.append(Message(role='assistant', content=generated_text))
+            messages.append(Message(role="assistant", content=generated_text))
             pre_ids_len += len(input_ids)
         else:
             messages = []
             pre_ids_len = 0
-        
+
         engine.fabric.print("\n")
-        engine.fabric.print(f"Generated {num_new_tokens} tokens in {t:.02f} seconds, {(num_new_tokens / t):.2f} tokens/second")
+        engine.fabric.print(
+            f"Generated {num_new_tokens} tokens in {t:.02f} seconds, {(num_new_tokens / t):.2f} tokens/second"
+        )
         engine.fabric.print(f"Memory used: {torch.cuda.max_memory_allocated() / 1e9:.02f} GB")
         engine.fabric.print(f"Bandwidth Achieved: {model_size * tokens_sec / 1e9:.02f} GB/s")
-        engine.fabric.print("\n")
+        engine.fabric.print("\n")
```

### Comparing `osc_llm-0.1.4/osc_llm/chat_templates/base.py` & `osc_llm-0.1.5/osc_llm/chat_templates/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,45 +1,46 @@
 from typing import List, Literal, Optional, Dict
 from pydantic import BaseModel
 from pathlib import Path
 from ..config import registry, Config
 
 
-
 class Property(BaseModel):
     type: str
     description: Optional[str] = None
-    
+
+
 class Parameters(BaseModel):
-    type: str 
+    type: str
     properties: Dict[str, Property]
     required: List[str]
 
+
 class Tool(BaseModel):
     name: str
     description: str
     parameters: Parameters
 
+
 class Message(BaseModel):
     role: Literal["system", "user", "assistant", "observation"]
     content: str
     metadata: str = ""
     tools: List[Tool] = []
-    
 
-class ChatTemplate():
-    
-    default_system: Optional[str] = ''
+
+class ChatTemplate:
+    default_system: Optional[str] = ""
     stop_texts: List[str] = []
-    generate_prompt: str = ''
-    
+    generate_prompt: str = ""
+
     @classmethod
     def apply_messages(cls, messages: List[Message], add_generate_prompt: bool = True) -> str:
         raise NotImplementedError
-    
+
     @classmethod
     def apply_user(cls, user: str, add_generate_prompt: bool = True) -> str:
         messages = []
         if cls.default_system:
             messages.append(Message(role="system", content=cls.default_system))
         messages.append(Message(role="user", content=user))
         return cls.apply_messages(messages, add_generate_prompt=add_generate_prompt)
@@ -50,27 +51,27 @@
             if cls == v:
                 name = k
         config_str = f"""
         [chat_template]
         @chat_templates = {name}"""
         config = Config().from_str(config_str)
         return config
-    
+
     @classmethod
     def from_name(cls, name: str) -> "ChatTemplate":
         template_cls = None
         for k, v in registry.chat_templates.get_all().items():
             if k in name:
                 template_cls = v
         if template_cls is None:
             raise ValueError(f"Chat template for {name} not found")
         return template_cls
-    
+
     @classmethod
     def from_checkpoint(cls, checkpoint_dir: str) -> "ChatTemplate":
         checkpoint_dir = Path(checkpoint_dir)
         config_path: Path = checkpoint_dir / "config.cfg"
         if config_path.exists():
             config = Config().from_disk(config_path)
-            if 'chat_template' in config:
-                return registry.chat_templates.get(config['chat_template']['@chat_templates'])
-        return cls.from_name(checkpoint_dir.stem)
+            if "chat_template" in config:
+                return registry.chat_templates.get(config["chat_template"]["@chat_templates"])
+        return cls.from_name(checkpoint_dir.stem)
```

### Comparing `osc_llm-0.1.4/osc_llm/chat_templates/chatglm.py` & `osc_llm-0.1.5/osc_llm/chat_templates/chatglm.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,31 +1,28 @@
 from .base import ChatTemplate, Message
 from typing import List
 import json
 from ..config import registry
 
 
-
 @registry.chat_templates.register("chatglm3")
 class ChatGLM3ChatTemplate(ChatTemplate):
-    
     default_system: str = "You are ChatGLM3, a large language model trained by Zhipu.AI. Follow the user's instructions carefully. Respond using markdown."
     stop_texts: List[str] = ["<|observation|>", "<|user|>"]
-    
+
     @classmethod
     def apply_messages(cls, messages: List[Message], add_generate_prompt: bool = True) -> str:
         prompt: str = ""
         for message in messages:
             if message.role == "user":
                 prompt += f"<|user|>{message.metadata}\n{message.content}"
             elif message.role == "assistant":
                 prompt += f"<|assistant|>{message.metadata}\n{message.content}"
             elif message.role == "system":
                 content = message.content
                 if len(message.tools) > 0:
                     content += "\n"
-                    content += json.dumps(message.model_dump()['tools'])
+                    content += json.dumps(message.model_dump()["tools"])
                 prompt += f"<|system|>{message.metadata}\n{content}"
         if add_generate_prompt:
             prompt += "<|assistant|>"
         return prompt
-
```

### Comparing `osc_llm-0.1.4/osc_llm/chat_templates/chatml.py` & `osc_llm-0.1.5/osc_llm/chat_templates/chatml.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,26 @@
 from .base import ChatTemplate, Message
 from ..config import registry
 from typing import List
 
 
-
 @registry.chat_templates.register("Yi")
 @registry.chat_templates.register("Qwen")
 @registry.chat_templates.register("ChatML")
 class ChatMLChatTemplate(ChatTemplate):
-    
     default_system: str = "You are a helpful assistant."
     stop_texts: List[str] = ["<|im_end|>"]
     generate_prompt: str = "<|im_start|>assistant\n"
-    
+
     @classmethod
     def apply_messages(cls, messages: List[Message], add_generate_prompt: bool = True) -> str:
         prompt = ""
         for message in messages:
             if message.role == "user":
                 prompt += f"<|im_start|>user\n{message.content}<|im_end|>\n"
             elif message.role == "assistant":
                 prompt += f"<|im_start|>assistant\n{message.content}<|im_end|>\n"
             elif message.role == "system":
                 prompt += f"<|im_start|>system\n{message.content}<|im_end|>\n"
         if add_generate_prompt:
             prompt += cls.generate_prompt
-        return prompt
+        return prompt
```

### Comparing `osc_llm-0.1.4/osc_llm/chat_templates/llama.py` & `osc_llm-0.1.5/osc_llm/chat_templates/llama.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,62 +3,64 @@
 from ..config import registry
 
 
 @registry.chat_templates.register("Llama3-8B-Chinese-Chat")
 @registry.chat_templates.register("llama-3-chinese-8b-instruct")
 @registry.chat_templates.register("Llama-3")
 class Llama3ChatTemplate(ChatTemplate):
-    
     stop_texts: List[str] = ["<|end_of_text|>", "<|eot_id|>"]
     generate_prompt: str = "<|start_header_id|>assistant<|end_header_id|>\n\n"
-    
+
     @classmethod
     def apply_messages(cls, messages: List[Message], add_generate_prompt: bool = False) -> str:
         assert messages[-1].role == "user", "Last message must be user"
         prompt = "<|begin_of_text|>"
         for message in messages:
             prompt += _apply_message_llama3(message)
         if add_generate_prompt:
             prompt += cls.generate_prompt
         return prompt
-    
+
+
 def _apply_message_llama3(message: Message) -> str:
     template = "<|start_header_id|>{role}<|end_header_id|>\n\n{content}<|eot_id|>"
     return template.format(role=message.role, content=message.content)
 
 
 @registry.chat_templates.register("Llama-2")
 class Llama2ChatTemplate(ChatTemplate):
-    
-    default_system: str = ("You are a helpful, respectful and honest assistant. Always answer as helpfully as"
-            " possible, while being safe.  Your answers should not include any harmful, unethical, racist, sexist,"
-            " toxic, dangerous, or illegal content. Please ensure that your responses are socially unbiased and"
-            " positive in nature.\n\nIf a question does not make any sense, or is not factually coherent, explain why"
-            " instead of answering something not correct. If you don't know the answer to a question, please don't"
-            " share false information.")
+    default_system: str = (
+        "You are a helpful, respectful and honest assistant. Always answer as helpfully as"
+        " possible, while being safe.  Your answers should not include any harmful, unethical, racist, sexist,"
+        " toxic, dangerous, or illegal content. Please ensure that your responses are socially unbiased and"
+        " positive in nature.\n\nIf a question does not make any sense, or is not factually coherent, explain why"
+        " instead of answering something not correct. If you don't know the answer to a question, please don't"
+        " share false information."
+    )
     stop_texts: List[str] = []
-    generate_prompt: str = ''
-    
+    generate_prompt: str = ""
+
     @classmethod
     def apply_messages(cls, messages: List[Message], add_generate_prompt: bool = True) -> str:
-        if messages[0].role == 'system':
+        if messages[0].role == "system":
             assert len(messages) >= 2, "must have a user input"
             assert messages[1].role == "user", "must have a user input"
             prompt = f"[INST] <<SYS>>\n{messages[0].content}\n<</SYS>>\n\n{messages[1].content} [/INST]"
             for message in messages[2:]:
                 prompt += _apply_message_llama2(message)
         else:
             prompt = f"[INST] <<SYS>>\n{cls.default_system}\n<</SYS>>\n\n{messages[0].content} [/INST]"
             for message in messages[1:]:
                 prompt += _apply_message_llama2(message)
         return prompt
-    
+
+
 def _apply_message_llama2(message: Message) -> str:
     if message.role == "user":
         return f"[INST] {message.content} [/INST]"
     if message.role == "assistant":
         return f" {message.content} "
-    
+
+
 @registry.chat_templates.register("chinese-alpaca-2")
 class ChineseAlpaca2ChatTemplate(Llama2ChatTemplate):
-    
-    default_system: str = "You are a helpful assistant, 你是一个乐于助人的助手."
+    default_system: str = "You are a helpful assistant, 你是一个乐于助人的助手."
```

### Comparing `osc_llm-0.1.4/osc_llm/config.py` & `osc_llm-0.1.5/osc_llm/config.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,61 +1,30 @@
 import catalogue
 import confection
 from confection import Config
 
 
 class registry(confection.registry):
-    
-    layers = catalogue.create(
-        "osc", 
-        "layers", 
-        entry_points=True
-    )
-    
-    architectures = catalogue.create(
-        "osc", 
-        "architectures", 
-        entry_points=True
-    )
-    
-    model_helpers = catalogue.create(
-        "osc", 
-        "model_helpers", 
-        entry_points=True
-    )
-    
-    quantizers = catalogue.create(
-        "osc", 
-        "quantizers", 
-        entry_points=True
-    )
-    
-    chat_templates = catalogue.create(
-        "osc", 
-        "chat_templates", 
-        entry_points=True
-    )
-    
-    samplers = catalogue.create(
-        "osc", 
-        "samplers", 
-        entry_points=True
-    )
-    
-    engines = catalogue.create(
-        "osc", 
-        "engines", 
-        entry_points=True
-    )
+    layers = catalogue.create("osc", "layers", entry_points=True)
+
+    architectures = catalogue.create("osc", "architectures", entry_points=True)
+
+    model_helpers = catalogue.create("osc", "model_helpers", entry_points=True)
+
+    quantizers = catalogue.create("osc", "quantizers", entry_points=True)
+
+    chat_templates = catalogue.create("osc", "chat_templates", entry_points=True)
+
+    samplers = catalogue.create("osc", "samplers", entry_points=True)
+
+    engines = catalogue.create("osc", "engines", entry_points=True)
 
     @classmethod
     def create(cls, registry_name: str, entry_points: bool = False) -> None:
         """Create a new custom registry."""
         if hasattr(cls, registry_name):
             raise ValueError(f"Registry '{registry_name}' already exists")
-        reg = catalogue.create(
-            "osc", registry_name, entry_points=entry_points
-        )
+        reg = catalogue.create("osc", registry_name, entry_points=entry_points)
         setattr(cls, registry_name, reg)
 
 
-__all__ = ["Config", "registry"]
+__all__ = ["Config", "registry"]
```

### Comparing `osc_llm-0.1.4/osc_llm/engines/base.py` & `osc_llm-0.1.5/osc_llm/engines/base.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,58 +5,58 @@
 from ..samplers import Sampler, TopK
 from abc import ABC, abstractmethod
 import torch
 from ..utils import get_default_supported_precision
 
 
 class LLMEngine(ABC):
-    """语言模型引擎: 控制着大模型加载,编译,运转以及停止。
-    """
-    
+    """语言模型引擎: 控制着大模型加载,编译,运转以及停止。"""
+
     def __init__(
         self,
         checkpoint_dir: str,
+        draft_checkpoint_dir: Optional[str] = None,
         sampler: Optional[Sampler] = None,
         max_length: Optional[int] = None,
         devices: Union[int, List[int]] = 1,
         accelerator: str = "auto",
         compile: bool = True,
-        precision: Optional[str] = None
+        precision: Optional[str] = None,
     ):
-
         if not precision:
             precision = get_default_supported_precision(training=False)
         self.fabric = Fabric(devices=devices, accelerator=accelerator, precision=precision)
-        
+
         self.sampler = sampler if sampler else TopK(temperature=0.8, k=200)
         self.max_length = max_length
-        
+
         self.compile = compile
-        
+
         self.checkpoint_dir = checkpoint_dir
-    
+        self.draft_checkpoint_dir = draft_checkpoint_dir
+
     @abstractmethod
     def load_model(self) -> None:
         raise NotImplementedError
-    
+
     def compile_model(self) -> None:
         raise NotImplementedError
-    
+
     def setup_model(self) -> None:
         raise NotImplementedError
-    
+
     @abstractmethod
     def run(self, **model_inputs) -> Generator[torch.Tensor, None, None]:
         raise NotImplementedError
-    
+
     def setup(self) -> None:
         t = perf_counter()
         self.load_model()
         self.fabric.print(f"load model in {perf_counter() - t:.02f} seconds", file=sys.stderr)
         if self.compile:
             self.compile_model()
         t = perf_counter()
         self.setup_model()
         self.fabric.print(f"setup model in {perf_counter() - t:.02f} seconds", file=sys.stderr)
-            
+
     def reset_sampler(self, sampler: Sampler) -> None:
-        self.sampler = sampler
+        self.sampler = sampler
```

### Comparing `osc_llm-0.1.4/osc_llm/engines/v1.py` & `osc_llm-0.1.5/osc_llm/engines/v1.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,96 +4,101 @@
 from ..config import Config, registry
 import torch
 from torch.nn.attention import sdpa_kernel, SDPBackend
 from typing import List, Generator, Optional
 from pathlib import Path
 
 
-
 @registry.engines.register("v1.TransformerDecoder")
 @registry.engines.register("v1")
 class LLMEngineV1(LLMEngine):
     """v1版本语言模型引擎
     特点:
     1. 基于torch.compile进行``动态形状``模型编译,大大的提升了模型推理速度。
-    
+
     注意:
     1. torch.compile机制会在首次运行时候进行真正的编译,因此首次运行会比较慢。
     2. 建议先运行至少2次run方法,以便编译完成。
     """
+
     def load_model(self) -> None:
-        config_path = Path(self.checkpoint_dir) / 'config.cfg'
-        states_path = Path(self.checkpoint_dir) / 'osc_model.pth'
-        
+        config_path = Path(self.checkpoint_dir) / "config.cfg"
+        states_path = Path(self.checkpoint_dir) / "osc_model.pth"
+
         config = Config().from_disk(config_path)
-        assert config['model']['@architectures'] == "TransformerDecoder", "Only TransformerDecoder Architecture is supported"
-            
+        assert (
+            config["model"]["@architectures"] == "TransformerDecoder"
+        ), "Only TransformerDecoder Architecture is supported"
+
         self.model = build_model(config=config_path, empty_init=True).eval()
         self.fabric.load_raw(states_path, self.model)
         self.model = self.fabric.to_device(self.model)
-        
+
         with self.fabric.init_tensor():
             self.model.setup_kv_cache(batch_size=1, max_length=self.max_length, dtype=torch.bfloat16)
-            
-        
+
     def compile_model(self) -> None:
         torch._inductor.config.coordinate_descent_tuning = True
         torch._inductor.config.triton.unique_kernel_names = True
-        torch._inductor.config.fx_graph_cache = True # Experimental feature to reduce compilation times, will be on by default in future
-        torch._inductor.config.triton.cudagraph_trees = False # 目前用作server的时候有bug
-        
+        torch._inductor.config.fx_graph_cache = (
+            True  # Experimental feature to reduce compilation times, will be on by default in future
+        )
+        torch._inductor.config.triton.cudagraph_trees = False  # 目前用作server的时候有bug
+
         torch._dynamo.config.automatic_dynamic_shapes = True
         torch._dynamo.config.suppress_errors = True
         torch._dynamo.config.capture_dynamic_output_shape_ops = True
-        
-        
+
         self.model: TransformerDecoder = torch.compile(self.model, dynamic=True, fullgraph=True, mode="reduce-overhead")
 
-        
     def setup_model(self) -> None:
         self.model = self.fabric.setup_module(self.model)
-    
+
     @torch.inference_mode()
-    def run(self, input_ids: torch.Tensor, stop_ids: List[torch.Tensor], input_pos: Optional[torch.Tensor] = None) -> Generator[str, None, None]:
-        
+    def run(
+        self,
+        input_ids: torch.Tensor,
+        stop_ids: List[torch.Tensor],
+        input_pos: Optional[torch.Tensor] = None,
+    ) -> Generator[torch.Tensor, None, None]:
         # 确保输入在设备上
         input_ids = self.fabric.to_device(input_ids)
         if input_pos is None:
             input_pos = self.fabric.to_device(torch.arange(len(input_ids)))
         stop_ids = [self.fabric.to_device(stop_id) for stop_id in stop_ids]
-        
+
         max_length = self.max_length if self.max_length else self.model.block_size
-        
+
         # prefill
         input_ids = self.prefill(input_ids=input_ids.view(1, -1), input_pos=input_pos)
         yield input_ids
-        
+
         # decode
         with self.fabric.init_tensor():
             input_pos = torch.tensor([input_pos[-1].item() + 1])
         max_stop_len = max([len(stop_id) for stop_id in stop_ids])
-        yield_ids = [] # 用来存储的生成token ids, 直到长度达到stop ids中的最大长度, 然后生成
+        yield_ids = []  # 用来存储的生成token ids, 直到长度达到stop ids中的最大长度, 然后生成
         with sdpa_kernel(backends=[SDPBackend.MATH]):
             for i in range(1, max_length - input_pos.item() + 1):
                 input_ids = input_ids.view(1, -1)
                 next_token_id = self.decode(input_ids=input_ids, input_pos=input_pos)
                 yield_ids.append(next_token_id)
                 # 遍历每一个stop ids
                 for ids in stop_ids:
                     if len(yield_ids) == len(ids):
                         if all(a == b for a, b in zip(yield_ids, ids)):
-                            return 
+                            return
                 if len(yield_ids) >= max_stop_len:
                     yield from yield_ids
                     yield_ids = []
                 input_pos = input_pos.add_(1)
                 input_ids = next_token_id
-        
+
     def prefill(self, **model_inputs) -> torch.Tensor:
         logits = self.model(**model_inputs)[0, -1]
         idx = self.sampler.sample(logits=logits)
         return idx
-    
+
     def decode(self, **model_inputs) -> torch.Tensor:
         logits = self.model(**model_inputs)[0, -1]
         idx = self.sampler.sample(logits=logits)
-        return idx
+        return idx
```

### Comparing `osc_llm-0.1.4/osc_llm/engines/v2.py` & `osc_llm-0.1.5/osc_llm/engines/v2.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,100 +4,108 @@
 from ..config import Config, registry
 import torch
 from torch.nn.attention import sdpa_kernel, SDPBackend
 from typing import List, Generator, Optional
 from pathlib import Path
 
 
-
 @registry.engines.register("v2.TransformerDecoder")
 @registry.engines.register("v2")
 class LLMEngineV2(LLMEngine):
     """v2版本语言模型引擎
     特点:
     1. 基于torch.compile进行模型编译,大大的提升了模型推理速度。
     2. 为了解决每次推理都需要重新编译的问题,在prefill和decode两个阶段分别使用两份相同的模型,并且共享kv_cache和mask_cache。
     3. prefill模型用动态形状编译,decode模型用静态编译。
-    
+
     注意:
     1. torch.compile机制会在首次运行时候进行真正的编译,因此首次运行会比较慢。
     2. 建议先运行至少2次run方法,以便编译完成。
     """
+
     def load_model(self) -> None:
-        config_path = Path(self.checkpoint_dir) / 'config.cfg'
-        states_path = Path(self.checkpoint_dir) / 'osc_model.pth'
-        
+        config_path = Path(self.checkpoint_dir) / "config.cfg"
+        states_path = Path(self.checkpoint_dir) / "osc_model.pth"
+
         config = Config().from_disk(config_path)
-        assert config['model']['@architectures'] == "TransformerDecoder", "Only TransformerDecoder Architecture is supported"
-            
+        assert (
+            config["model"]["@architectures"] == "TransformerDecoder"
+        ), "Only TransformerDecoder Architecture is supported"
+
         with self.fabric.init_module(empty_init=True):
             self.prefill_model = build_model(config=config_path, empty_init=False).eval()
             self.decode_model = build_model(config=config_path, empty_init=False).eval()
-        
+
         self.fabric.load_raw(states_path, self.prefill_model)
         self.fabric.load_raw(states_path, self.decode_model)
-        
+
         with self.fabric.init_tensor():
             self.prefill_model.setup_kv_cache(batch_size=1, max_length=self.max_length, dtype=torch.bfloat16)
-            
+
         self.decode_model.kv_caches = self.prefill_model.kv_caches
         self.decode_model.mask_cache = self.prefill_model.mask_cache
-        
+
     def compile_model(self) -> None:
         torch._inductor.config.coordinate_descent_tuning = True
         torch._inductor.config.triton.unique_kernel_names = True
-        torch._inductor.config.fx_graph_cache = True # Experimental feature to reduce compilation times, will be on by default in future
+        torch._inductor.config.fx_graph_cache = (
+            True  # Experimental feature to reduce compilation times, will be on by default in future
+        )
         torch._dynamo.config.automatic_dynamic_shapes = True
         torch._dynamo.config.suppress_errors = True
         self.decode_model: TransformerDecoder = torch.compile(self.decode_model, mode="reduce-overhead", fullgraph=True)
         self.prefill_model: TransformerDecoder = torch.compile(self.prefill_model, dynamic=True)
-    
+
     def setup_model(self) -> None:
         self.prefill_model = self.fabric.setup_module(self.prefill_model)
         self.decode_model = self.fabric.setup_module(self.decode_model)
-    
+
     @torch.inference_mode()
-    def run(self, input_ids: torch.Tensor, stop_ids: List[torch.Tensor], input_pos: Optional[torch.Tensor] = None) -> Generator[str, None, None]:
-        
+    def run(
+        self,
+        input_ids: torch.Tensor,
+        stop_ids: List[torch.Tensor],
+        input_pos: Optional[torch.Tensor] = None,
+    ) -> Generator[torch.Tensor, None, None]:
         # 确保输入在设备上
         input_ids = self.fabric.to_device(input_ids)
         if input_pos is None:
             input_pos = self.fabric.to_device(torch.arange(len(input_ids)))
         stop_ids = [self.fabric.to_device(stop_id) for stop_id in stop_ids]
-        
-        # prefill 
+
+        # prefill
         max_length = self.max_length if self.max_length else self.prefill_model.block_size
         input_ids = self.prefill(input_ids=input_ids.view(1, -1), input_pos=input_pos)
         yield input_ids
-        
+
         # decode
         with self.fabric.init_tensor():
             input_pos = torch.tensor([input_pos[-1].item() + 1])
         max_stop_len = max([len(stop_id) for stop_id in stop_ids])
         yield_ids = []
         for i in range(1, max_length - input_pos.item() + 1):
             with sdpa_kernel(backends=[SDPBackend.MATH]):
                 input_ids = input_ids.view(1, -1)
                 next_token_id = self.decode(input_ids=input_ids, input_pos=input_pos)
                 yield_ids.append(next_token_id)
                 # 遍历每一个stop ids
                 for ids in stop_ids:
                     if len(yield_ids) >= len(ids):
                         if all(a == b for a, b in zip(yield_ids, ids)):
-                            return 
+                            return
                 if len(yield_ids) >= max_stop_len:
                     yield from yield_ids
                     yield_ids = []
             input_pos = input_pos.add_(1)
             input_ids = next_token_id
-        
+
     @torch.inference_mode()
     def prefill(self, **model_inputs) -> torch.Tensor:
         logits = self.prefill_model(**model_inputs)[0, -1]
         idx = self.sampler.sample(logits=logits)
         return idx
-    
+
     @torch.inference_mode()
     def decode(self, **model_inputs) -> torch.Tensor:
         logits = self.decode_model(**model_inputs)[0, -1]
         idx = self.sampler.sample(logits=logits)
-        return idx
+        return idx
```

### Comparing `osc_llm-0.1.4/osc_llm/layers/__init__.py` & `osc_llm-0.1.5/osc_llm/layers/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,9 +24,9 @@
     "SiLU",
     "GELU",
     "StaticKVCache",
     "Linear",
     "WeightOnlyInt4Linear",
     "Int8Linear",
     "Dropout",
-    "SparseMoe"
-]
+    "SparseMoe",
+]
```

### Comparing `osc_llm-0.1.4/osc_llm/layers/activation.py` & `osc_llm-0.1.5/osc_llm/layers/activation.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from ..config import registry
-import torch.nn as nn 
-
+import torch.nn as nn
 
 
 @registry.layers.register("SiLU")
 def SiLU(inplace: bool = False) -> nn.Module:
     return nn.SiLU(inplace=inplace)
 
 
@@ -26,8 +25,8 @@
 @registry.layers.register("Tanh")
 def Tanh() -> nn.Module:
     return nn.Tanh()
 
 
 @registry.layers.register("Softmax")
 def Softmax(dim: int) -> nn.Module:
-    return nn.Softmax(dim=dim)
+    return nn.Softmax(dim=dim)
```

### Comparing `osc_llm-0.1.4/osc_llm/layers/attention.py` & `osc_llm-0.1.5/osc_llm/layers/attention.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import torch.nn as nn
 import torch
 from typing import Optional
 from ..config import registry
 from .kv_cache import KVCache
 import math
-    
-    
-@registry.layers.register("CausalSelfAttention")  
+
+
+@registry.layers.register("CausalSelfAttention")
 class CausalSelfAttention(nn.Module):
     """融合了RoPE,MQA,GQA,MHA的因果自注意力机制层"""
-    
+
     # 当`n_heads=4`时MHA,GQA,MQA的区别:
     # ┌───┐┌───┐┌───┐┌───┐     ┌───┐    ┌───┐             ┌───┐
     # │ v ││ v ││ v ││ v │     │ v │    │ v │             │ v │
     # └───┘└───┘└───┘└───┘     └───┘    └───┘             └───┘
     #   │    │    │    │         │        │                 │
     # ┌───┐┌───┐┌───┐┌───┐     ┌───┐    ┌───┐             ┌───┐
     # │ k ││ k ││ k ││ k │     │ k │    │ k │             │ k │
@@ -21,117 +21,141 @@
     #   │    │    │    │      ┌──┴──┐  ┌──┴──┐      ┌────┬──┴─┬────┐
     # ┌───┐┌───┐┌───┐┌───┐  ┌───┐┌───┐┌───┐┌───┐  ┌───┐┌───┐┌───┐┌───┐
     # │ q ││ q ││ q ││ q │  │ q ││ q ││ q ││ q │  │ q ││ q ││ q ││ q │
     # └───┘└───┘└───┘└───┘  └───┘└───┘└───┘└───┘  └───┘└───┘└───┘└───┘
     # ◀──────────────────▶  ◀──────────────────▶  ◀──────────────────▶
     #         MHA                    GQA                   MQA
     #   n_query_groups=4       n_query_groups=2      n_query_groups=1
-    
+
     def __init__(
-        self, 
-        n_in: int, 
+        self,
+        n_in: int,
         n_heads: int,
         q_bias: bool = False,
         k_bias: bool = False,
         v_bias: bool = False,
         o_bias: bool = False,
         n_query_groups: Optional[int] = None,
         kv_cache: Optional[KVCache] = None,
         use_qkv_proj: bool = False,
-        qkv_bias: bool = False
+        qkv_bias: bool = False,
     ):
         super().__init__()
-        
+
         assert n_in % n_heads == 0, f"dim {n_in} must be divisible by n_heads {n_heads}"
-        
+
         self.n_heads = n_heads
         self.head_size = n_in // n_heads
         self.n_query_groups = n_query_groups if n_query_groups else n_heads
-        
+
         self.use_qkv_proj = use_qkv_proj
         if not use_qkv_proj:
             self.q_proj = nn.Linear(n_in, self.n_heads * self.head_size, bias=q_bias)
             self.k_proj = nn.Linear(n_in, self.n_query_groups * self.head_size, bias=k_bias)
             self.v_proj = nn.Linear(n_in, self.n_query_groups * self.head_size, bias=v_bias)
         else:
-            self.qkv_proj = nn.Linear(n_in, self.n_heads * self.head_size + self.n_query_groups * self.head_size * 2, bias=qkv_bias)
-            
+            self.qkv_proj = nn.Linear(
+                n_in,
+                self.n_heads * self.head_size + self.n_query_groups * self.head_size * 2,
+                bias=qkv_bias,
+            )
+
         self.o_proj = nn.Linear(n_in, n_in, bias=o_bias)
-        
-        self.kv_cache: KVCache = kv_cache
 
+        self.kv_cache: KVCache = kv_cache
 
     def forward(
         self,
         x: torch.Tensor,
         cos: Optional[torch.Tensor] = None,
         sin: Optional[torch.Tensor] = None,
         attention_mask: Optional[torch.Tensor] = None,
-        input_pos: Optional[torch.Tensor] = None
+        input_pos: Optional[torch.Tensor] = None,
     ):
-        
         B, L, D = x.size()  # batch size, sequence length, embedding dimensionality (n_embd)
         if self.use_qkv_proj:
             qkv: torch.Tensor = self.qkv_proj(x)
             q, k, v = qkv.split(
-                [self.n_heads * self.head_size, self.n_query_groups * self.head_size, self.n_query_groups * self.head_size],
-                dim=-1
+                [
+                    self.n_heads * self.head_size,
+                    self.n_query_groups * self.head_size,
+                    self.n_query_groups * self.head_size,
+                ],
+                dim=-1,
             )
             q = q.reshape(B, L, self.n_heads, self.head_size).permute(0, 2, 1, 3)
             k = k.reshape(B, L, self.n_query_groups, self.head_size).permute(0, 2, 1, 3)
             v = v.reshape(B, L, self.n_query_groups, self.head_size).permute(0, 2, 1, 3)
         else:
             q: torch.Tensor = self.q_proj(x).reshape(B, L, self.n_heads, self.head_size).permute(0, 2, 1, 3)
             k: torch.Tensor = self.k_proj(x).reshape(B, L, self.n_query_groups, self.head_size).permute(0, 2, 1, 3)
             v: torch.Tensor = self.v_proj(x).reshape(B, L, self.n_query_groups, self.head_size).permute(0, 2, 1, 3)
-        
+
         if (cos is not None) and (sin is not None):
             q = apply_rope(q, cos, sin)
             k = apply_rope(k, cos, sin)
-            
+
         if input_pos is not None:
             if not self.kv_cache:
-                raise TypeError("current attention layer does not support kv_cache, please set `kv_cache` in the layer init")
+                raise TypeError(
+                    "current attention layer does not support kv_cache, please set `kv_cache` in the layer init"
+                )
             if not hasattr(self.kv_cache, "k_cache") or not hasattr(self.kv_cache, "v_cache"):
                 raise TypeError("You need to call `model.setup_kv_cache()`")
             k, v = self.kv_cache.update(input_pos=input_pos, k=k, v=v, copy_dim=2)
-            
-        if self.n_query_groups != 1 and self.n_query_groups != self.n_heads:  # doing this would require a full kv cache with MQA (inefficient!)
+
+        if (
+            self.n_query_groups != 1 and self.n_query_groups != self.n_heads
+        ):  # doing this would require a full kv cache with MQA (inefficient!)
             # for MHA this is a no-op
-            k = k[:,:,None,:,:].expand(-1, -1, self.n_heads // self.n_query_groups, -1, -1).reshape(B, self.n_heads, -1, self.head_size)
-            v = v[:,:,None,:,:].expand(-1, -1, self.n_heads // self.n_query_groups, -1, -1).reshape(B, self.n_heads, -1, self.head_size)
+            k = (
+                k[:, :, None, :, :]
+                .expand(-1, -1, self.n_heads // self.n_query_groups, -1, -1)
+                .reshape(B, self.n_heads, -1, self.head_size)
+            )
+            v = (
+                v[:, :, None, :, :]
+                .expand(-1, -1, self.n_heads // self.n_query_groups, -1, -1)
+                .reshape(B, self.n_heads, -1, self.head_size)
+            )
 
         o = self.scaled_dot_product_attention(q, k, v, mask=attention_mask)
 
         o = o.reshape(B, L, D)
 
         o = self.o_proj(o)
 
         return o
 
     def scaled_dot_product_attention(
-        self, q: torch.Tensor, k: torch.Tensor, v: torch.Tensor, mask: Optional[torch.Tensor] = None
+        self,
+        q: torch.Tensor,
+        k: torch.Tensor,
+        v: torch.Tensor,
+        mask: Optional[torch.Tensor] = None,
     ):
         scale = 1.0 / math.sqrt(self.head_size)
         y = torch.nn.functional.scaled_dot_product_attention(
             q, k, v, attn_mask=mask, dropout_p=0.0, scale=scale, is_causal=mask is None
         )
         return y.transpose(1, 2)
-    
-    def setup_kv_cache(self, 
-                       batch_size: int, 
-                       max_seq_length: int, 
-                       device: Optional[torch.device] = None, 
-                       dtype: Optional[torch.dtype] = None) -> None:
+
+    def setup_kv_cache(
+        self,
+        batch_size: int,
+        max_seq_length: int,
+        device: Optional[torch.device] = None,
+        dtype: Optional[torch.dtype] = None,
+    ) -> None:
         n_heads = self.n_query_groups
         k_shape = (batch_size, n_heads, max_seq_length, self.head_size)
         v_shape = (batch_size, n_heads, max_seq_length, self.head_size)
         self.kv_cache.setup(k_shape, v_shape, dtype=dtype, device=device)
 
 
 def apply_rope(x: torch.Tensor, cos: torch.Tensor, sin: torch.Tensor) -> torch.Tensor:
     head_size = x.size(-1)
     x1 = x[..., : head_size // 2]  # (B, nh, T, hs/2)
     x2 = x[..., head_size // 2 :]  # (B, nh, T, hs/2)
     rotated = torch.cat((-x2, x1), dim=-1)  # (B, nh, T, hs)
     roped = (x * cos) + (rotated * sin)
-    return roped.to(x.dtype) 
+    return roped.to(x.dtype)
```

### Comparing `osc_llm-0.1.4/osc_llm/layers/embedding.py` & `osc_llm-0.1.5/osc_llm/layers/embedding.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,57 +1,60 @@
 import torch.nn as nn
 from ..config import registry
 from typing import Optional
 import torch
 
 
-
 @registry.layers.register("TokenEmbedding")
 class TokenEmbedding(nn.Module):
-    def __init__(self, 
-                 n_embeddings: int,
-                 embedding_size: int):
+    def __init__(self, n_embeddings: int, embedding_size: int):
         super().__init__()
         self.embed = nn.Embedding(num_embeddings=n_embeddings, embedding_dim=embedding_size)
-        
+
     def forward(self, x, **kwargs):
         return self.embed(x)
 
 
 @registry.layers.register("TokenEmbeddingPlus")
 class TokenEmbeddingPlus(nn.Module):
-    def __init__(self, 
-                 n_embeddings: int,
-                 embedding_size: int,
-                 n_types: Optional[int] = None,
-                 n_positions: Optional[int] = None,
-                 norm: Optional[nn.Module] = None,
-                 dropout: Optional[nn.Module] = None,
-                 ):
+    def __init__(
+        self,
+        n_embeddings: int,
+        embedding_size: int,
+        n_types: Optional[int] = None,
+        n_positions: Optional[int] = None,
+        norm: Optional[nn.Module] = None,
+        dropout: Optional[nn.Module] = None,
+    ):
         super().__init__()
         self.embed = nn.Embedding(num_embeddings=n_embeddings, embedding_dim=embedding_size)
         if n_types:
             self.type_embed = nn.Embedding(num_embeddings=n_types, embedding_dim=embedding_size)
         if n_positions:
             self.pos_embed = nn.Embedding(num_embeddings=n_positions, embedding_dim=embedding_size)
             self.max_positions = n_positions
         if norm:
             self.norm = norm
         if dropout:
             self.dropout = dropout
-        
+
     def forward(self, input_ids: torch.LongTensor, **kwargs):
         x = self.embed(input_ids)
         if hasattr(self, "type_embed"):
-            token_type_ids = kwargs.get("token_type_ids", torch.zeros_like(input_ids, device=x.device, dtype=torch.long))
+            token_type_ids = kwargs.get(
+                "token_type_ids",
+                torch.zeros_like(input_ids, device=x.device, dtype=torch.long),
+            )
             x = x + self.type_embed(token_type_ids)
         if hasattr(self, "pos_embed"):
             B, L, D = x.size()
             if L > self.max_positions:
-                raise ValueError(f"Input length {L} is greater than the maximum number of positions {self.max_positions}.")
+                raise ValueError(
+                    f"Input length {L} is greater than the maximum number of positions {self.max_positions}."
+                )
             input_pos = kwargs.get("input_pos", torch.arange(L, device=x.device).unsqueeze(0).expand(B, -1))
             x = x + self.pos_embed(input_pos)
         if hasattr(self, "norm"):
             x = self.norm(x)
         if hasattr(self, "dropout"):
             x = self.dropout(x)
-        return x
+        return x
```

### Comparing `osc_llm-0.1.4/osc_llm/layers/feedforward.py` & `osc_llm-0.1.5/osc_llm/layers/feedforward.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,114 +2,122 @@
 import torch.nn as nn
 from copy import deepcopy
 import torch
 from typing import Optional
 import torch.nn.functional as F
 
 
-
 @registry.layers.register("GLU")
 class GLU(nn.Module):
-    """门控线性单元
-    """
-    def __init__(self, 
-                 n_in: int, 
-                 n_hidden: int,
-                 activation: nn.Module,
-                 up_bias: bool = False,
-                 gate_bias: bool = False,
-                 down_bias: bool = False) -> None:
+    """门控线性单元"""
+
+    def __init__(
+        self,
+        n_in: int,
+        n_hidden: int,
+        activation: nn.Module,
+        up_bias: bool = False,
+        gate_bias: bool = False,
+        down_bias: bool = False,
+    ) -> None:
         super().__init__()
         self.up_proj = nn.Linear(n_in, n_hidden, bias=up_bias)
         self.gate_proj = nn.Linear(n_in, n_hidden, bias=gate_bias)
         self.down_proj = nn.Linear(n_hidden, n_in, bias=down_bias)
         self.activation = activation
-        
+
     def forward(self, x):
         x1 = self.up_proj(x)
         x2 = self.gate_proj(x)
         x = x1 * self.activation(x2)
         x = self.down_proj(x)
         return x
-    
+
 
 @registry.layers.register("SwiGLU.v1")
 @registry.layers.register("SwiGLU")
-def SwiGLU(n_in: int, 
-           n_hidden: int,
-           up_bias: bool = False,
-           gate_bias: bool = False,
-           down_bias: bool = False) -> nn.Module:
-    """Swish激活函数的门控线性单元
-    """
-    return GLU(n_in=n_in,
-               n_hidden=n_hidden,
-               activation=nn.SiLU(),
-               up_bias=up_bias,
-               gate_bias=gate_bias,
-               down_bias=down_bias)
-           
-           
+def SwiGLU(
+    n_in: int,
+    n_hidden: int,
+    up_bias: bool = False,
+    gate_bias: bool = False,
+    down_bias: bool = False,
+) -> nn.Module:
+    """Swish激活函数的门控线性单元"""
+    return GLU(
+        n_in=n_in,
+        n_hidden=n_hidden,
+        activation=nn.SiLU(),
+        up_bias=up_bias,
+        gate_bias=gate_bias,
+        down_bias=down_bias,
+    )
+
+
 @registry.layers.register("SwiGLU.v2")
 class SwiGLUV2(nn.Module):
     """Swish激活函数的门控线性单元另外一种实现方式,
-    
-    与v1版本的区别: 
+
+    与v1版本的区别:
     - 原本的up_proj和gate_proj合并为up_gate_proj
     - 前向传播时, up_gate_proj的输出先前后切分为up和gate两部分
     """
+
     def __init__(
         self,
         n_in: int,
         n_hidden: int,
         up_gate_bias: bool = False,
-        down_bias: bool = False
+        down_bias: bool = False,
     ):
         super().__init__()
-        
+
         self.up_gate_proj = nn.Linear(n_in, n_hidden * 2, bias=up_gate_bias)
         self.down_proj = nn.Linear(n_hidden, n_in, bias=down_bias)
 
     def forward(self, x):
         x_gate, x_up = torch.chunk(self.up_gate_proj(x), 2, dim=-1)
         x = F.silu(x_gate) * x_up
         x = self.down_proj(x)
         return x
-    
-    
+
+
 @registry.layers.register("GeGLU")
-def GeGLU(n_in: int, 
-          n_hidden: int,
-          up_bias: bool = False,
-          gate_bias: bool = False,
-          down_bias: bool = False) -> nn.Module:
-    """GELU激活函数的门控线性单元
-    """
-    return GLU(n_in=n_in,
-               n_hidden=n_hidden,
-               activation=nn.GELU(),
-               up_bias=up_bias,
-               gate_bias=gate_bias,
-               down_bias=down_bias)
-    
-    
+def GeGLU(
+    n_in: int,
+    n_hidden: int,
+    up_bias: bool = False,
+    gate_bias: bool = False,
+    down_bias: bool = False,
+) -> nn.Module:
+    """GELU激活函数的门控线性单元"""
+    return GLU(
+        n_in=n_in,
+        n_hidden=n_hidden,
+        activation=nn.GELU(),
+        up_bias=up_bias,
+        gate_bias=gate_bias,
+        down_bias=down_bias,
+    )
+
+
 @registry.layers.register("SparseMoe")
 class SparseMoe(nn.Module):
-    """稀疏的专家混合网络
-    """
+    """稀疏的专家混合网络"""
+
     def __init__(
         self,
-        n_experts: int, 
+        n_experts: int,
         n_activated_experts: int,
         expert: nn.Module,
         gate: nn.Module,
         norm_probs: bool = True,
         shared_expert: Optional[nn.Module] = None,
-        shared_gate: Optional[nn.Module] = None
-        ) -> None:
+        shared_gate: Optional[nn.Module] = None,
+    ) -> None:
         super().__init__()
         self.gate = gate
         self.experts = nn.ModuleList(deepcopy(expert) for _ in range(n_experts))
         self.n_activated_experts = n_activated_experts
         self.n_experts = n_experts
         self.norm_probs = norm_probs
         self.shared_expert = shared_expert
@@ -118,104 +126,116 @@
     def forward(self, x: torch.Tensor) -> torch.Tensor:
         """
         Derived from: https://github.com/mistralai/mistral-src/blob/b46d6/moe_one_file_ref.py#L203-L219
         See also figure 1 in https://arxiv.org/abs/2211.15841
         """
         B, T, C = x.size()  # batch size, sequence length, embedding dimensionality (n_embd)
         x = x.view(-1, C)  # (B*T, C)
-        
+
         logits = self.gate(x)  # (B*T, n_expert)
         probs = F.softmax(logits, dim=-1, dtype=torch.float)
-        probs, indices = torch.topk(probs, self.n_activated_experts, dim=-1)  # probs: (B*T, n_expert_per_token), indices: (B*T, n_expert_per_token)
+        probs, indices = torch.topk(
+            probs, self.n_activated_experts, dim=-1
+        )  # probs: (B*T, n_expert_per_token), indices: (B*T, n_expert_per_token)
         if self.norm_probs:
             probs /= probs.sum(dim=-1, keepdim=True)
         probs = probs.to(dtype=x.dtype)
-        
-        masks = indices.unsqueeze(-1) == torch.arange(self.n_experts, device=x.device) # (B*T, n_expert_per_token, n_expert)
-        masks = masks.permute(2, 0, 1) # (n_expert, B*T, n_expert_per_token)
-        
+
+        masks = indices.unsqueeze(-1) == torch.arange(
+            self.n_experts, device=x.device
+        )  # (B*T, n_expert_per_token, n_expert)
+        masks = masks.permute(2, 0, 1)  # (n_expert, B*T, n_expert_per_token)
+
         y = torch.zeros_like(x)  # (B*T, C)
         for expert, mask in zip(self.experts, masks):
             # 找出该专家对应的token
             token_idx, expert_idx = torch.where(mask)
             y[token_idx] += probs[token_idx, expert_idx, None] * expert(x[token_idx])
-        
+
         if self.shared_expert is not None:
             y += self.shared_expert(x) * self.shared_gate(x).sigmoid()
-            
+
         return y.reshape(B, T, C)
-    
-    
+
+
 @registry.layers.register("Experts.SwiGLU")
 class SwiGLUExperts(nn.Module):
-    """专家类型为SwiGLU的稀疏专家混合网络
-    """
+    """专家类型为SwiGLU的稀疏专家混合网络"""
+
     def __init__(
         self,
         n_experts: int,
         n_in: int,
         n_hidden: int,
     ):
         self.up_proj = torch.nn.Parameter(torch.empty(n_experts, n_hidden, n_in))
         self.gate_proj = torch.nn.Parameter(torch.empty(n_experts, n_hidden, n_in))
         self.down_proj = torch.nn.Parameter(torch.empty(n_experts, n_in, n_hidden))
-        
+
     def forward(self, x: torch.Tensor, expert_indices: torch.Tensor) -> torch.Tensor:
         """
         x: (tokens, n_in) == (T, D)
         expert_indices: (tokens, n_active_experts) == (T, A)
-        
+
         """
-        w_up = self.up_proj[expert_indices] # (T, A, H, D)
-        w_gate = self.gate_proj[expert_indices] # (T, A, H, D)
-        w_down = self.down_proj[expert_indices] # (T, A, D, H)
-        
+        w_up = self.up_proj[expert_indices]  # (T, A, H, D)
+        w_gate = self.gate_proj[expert_indices]  # (T, A, H, D)
+        w_down = self.down_proj[expert_indices]  # (T, A, D, H)
+
         x_gate = F.silu(torch.einsum("td, tahd -> tah", x, w_gate))
         x_up = torch.einsum("td, tahd -> tah", x, w_up)
         x_down = torch.einsum("tah, tadh -> tad", x_gate * x_up, w_down)
-        
+
         return x_down
-    
+
 
 @registry.layers.register("SparseMoe.SwiGLU")
 class SwiGLUSparseMoe(nn.Module):
-    """稀疏专家混合网络的另一种实现方式
-    """
+    """稀疏专家混合网络的另一种实现方式"""
+
     def __init__(
         self,
         n_experts: int,
         n_activated_experts: int,
         n_in: int,
         n_hidden: int,
         add_shared_expert: bool = False,
         bias: bool = False,
-        norm_probs: bool = True
+        norm_probs: bool = True,
     ):
         super().__init__()
-        
+
         self.experts = SwiGLUExperts(n_experts=n_experts, n_in=n_in, n_hidden=n_hidden)
         self.n_activated_experts = n_activated_experts
         self.gate = nn.Linear(n_in, n_experts)
         self.add_shared_expert = add_shared_expert
         self.norm_probs = norm_probs
-        
+
         if add_shared_expert:
-            self.shared_expert = SwiGLU(n_in=n_in, n_hidden=n_hidden, up_bias=bias, down_bias=bias, gate_bias=bias)
+            self.shared_expert = SwiGLU(
+                n_in=n_in,
+                n_hidden=n_hidden,
+                up_bias=bias,
+                down_bias=bias,
+                gate_bias=bias,
+            )
             self.shared_gate = nn.Linear(n_in, 1)
-        
+
     def forward(self, x: torch.Tensor) -> torch.Tensor:
         B, S, D = x.size()
         x = x.view(-1, D)
-        
+
         logits = self.gate(x)  # (B*T, n_expert)
         probs = F.softmax(logits, dim=-1, dtype=torch.float)
-        probs, indices = torch.topk(probs, self.n_activated_experts, dim=-1)  # probs: (B*T, n_expert_per_token), indices: (B*T, n_expert_per_token)
+        probs, indices = torch.topk(
+            probs, self.n_activated_experts, dim=-1
+        )  # probs: (B*T, n_expert_per_token), indices: (B*T, n_expert_per_token)
         if self.norm_probs:
             probs /= probs.sum(dim=-1, keepdim=True)
         probs = probs.to(dtype=x.dtype)
-        
+
         y = self.experts(x, indices)
-        
+
         if self.add_shared_expert:
             y += self.shared_expert(x) * self.shared_gate(x).sigmoid()
-        
-        return y.reshape(B, S, D)
+
+        return y.reshape(B, S, D)
```

### Comparing `osc_llm-0.1.4/osc_llm/layers/kv_cache.py` & `osc_llm-0.1.5/osc_llm/layers/kv_cache.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,72 +1,97 @@
-import torch.nn as nn 
+import torch.nn as nn
 import torch
 from ..config import registry
 from typing import Tuple, Optional
 
 
-
 class KVCache(nn.Module):
-    
     def __init__(self) -> None:
         super().__init__()
-    
-    def setup(self, k_shape: Tuple[int], v_shape: Tuple[int], dtype: Optional[torch.dtype] = None, device: Optional[torch.device] = None):
+
+    def setup(
+        self,
+        k_shape: Tuple[int],
+        v_shape: Tuple[int],
+        dtype: Optional[torch.dtype] = None,
+        device: Optional[torch.device] = None,
+    ):
         """构建KVCache的缓存
 
         Args:
             k_shape (Tuple[int]): k缓存的形状, 通常为(batch_size, n_heads, seq_length, head_size)
             v_shape (Tuple[int]): v缓存的形状, 通常为(batch_size, n_heads, seq_length, head_size)
             dtype (Optional[torch.dtype], optional): 数据类型.
             device (Optional[torch.device], optional): 缓存存储设备.
         """
-        self.register_buffer("k_cache", torch.zeros(k_shape, dtype=dtype, device=device), persistent=False)
-        self.register_buffer("v_cache", torch.zeros(v_shape, dtype=dtype, device=device), persistent=False)
-    
-    def update(self, k: torch.Tensor, v: torch.Tensor, input_pos: torch.Tensor, copy_dim: torch.Tensor):
+        self.register_buffer(
+            "k_cache",
+            torch.zeros(k_shape, dtype=dtype, device=device),
+            persistent=False,
+        )
+        self.register_buffer(
+            "v_cache",
+            torch.zeros(v_shape, dtype=dtype, device=device),
+            persistent=False,
+        )
+
+    def update(
+        self,
+        k: torch.Tensor,
+        v: torch.Tensor,
+        input_pos: torch.Tensor,
+        copy_dim: torch.Tensor,
+    ):
         raise NotImplementedError
-    
+
     def reset_parameter(self):
         torch.nn.init.zeros_(self.k_cache)
         torch.nn.init.zeros_(self.v_cache)
-        
+
     def reset_cache(self):
         self.k_cache.zero_()
         self.v_cache.zero_()
-        
+
     def get_max_length(self):
         raise NotImplementedError
-    
+
     def get_seq_length(self):
         raise NotImplementedError
-    
-    
+
 
 @registry.layers.register("StaticKVCache")
 class StaticKVCache(KVCache):
     """提前分配好形状的KVCache,在模型推理过程中形状不会变化,如果超出最大长度,则会报错。
     缓存的形状一般为: (batch_size, n_heads, seq_length, head_size)
     """
+
     def __init__(self) -> None:
         super().__init__()
-        
-    def update(self, k: torch.Tensor, v: torch.Tensor, input_pos: torch.Tensor, copy_dim: int = 2):
+
+    def update(
+        self,
+        k: torch.Tensor,
+        v: torch.Tensor,
+        input_pos: torch.Tensor,
+        copy_dim: int = 2,
+    ):
         """更新KVCache的缓存
 
         Args:
             k (torch.Tensor): 当前的k
             v (torch.Tensor): 当前的v
             input_pos (torch.Tensor): 输入的位置
             copy_dim (int, optional): 复制的维度. Defaults to 2.
 
         Returns:
             Tuple[Tensor, Tensor]: 更新后的k和v.
         """
-        assert hasattr(self, "k_cache") and hasattr(self, "v_cache"), "KVCache must be setup before updating. Use `setup` method to setup KVCache"
-            
-        
+        assert hasattr(self, "k_cache") and hasattr(
+            self, "v_cache"
+        ), "KVCache must be setup before updating. Use `setup` method to setup KVCache"
+
         self.k_cache: torch.Tensor = self.k_cache.to(k.dtype)
         self.v_cache: torch.Tensor = self.v_cache.to(v.dtype)
-        
+
         k = self.k_cache.index_copy_(dim=copy_dim, index=input_pos, source=k)
         v = self.v_cache.index_copy_(dim=copy_dim, index=input_pos, source=v)
-        return k, v
+        return k, v
```

### Comparing `osc_llm-0.1.4/osc_llm/layers/linear.py` & `osc_llm-0.1.5/osc_llm/layers/linear.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,68 +2,62 @@
 import torch
 import torch.nn.functional as F
 from ..config import registry
 from ..utils import find_multiple
 import math
 
 
-
 @registry.layers.register("Linear")
 def Linear(n_in: int, n_out: int, bias: bool = True):
     return nn.Linear(in_features=n_in, out_features=n_out, bias=bias)
 
 
 @registry.layers.register("Int8Linear")
 class Int8Linear(nn.Module):
     """用于量化的Linear层，只包含weight和scales两个参数"""
+
     __contains__ = ["in_features", "out_features"]
     in_features: int
     out_features: int
     weight: torch.Tensor
-    
-    def __init__(
-        self,
-        in_features: int,
-        out_features: int,
-        bias: bool = False
-    ):
+
+    def __init__(self, in_features: int, out_features: int, bias: bool = False):
         super().__init__()
-        
+
         self.in_features = in_features
         self.out_features = out_features
         self.register_buffer("weight", torch.empty((out_features, in_features), dtype=torch.int8))
         self.register_buffer("scales", torch.ones(out_features, dtype=torch.bfloat16))
         if bias:
             self.register_buffer("bias", torch.zeros(out_features, dtype=torch.bfloat16))
         else:
             self.bias = None
-        
+
     def forward(self, input: torch.Tensor) -> torch.Tensor:
-        
         if self.bias is not None:
             logits = F.linear(input, self.weight.to(dtype=input.dtype)) * self.scales + self.bias.to(dtype=input.dtype)
         else:
             logits = F.linear(input, self.weight.to(dtype=input.dtype)) * self.scales
         return logits
-    
-    
+
+
 @registry.layers.register("WeightOnlyInt4Linear")
 class WeightOnlyInt4Linear(torch.nn.Module):
-    __constants__ = ['in_features', 'out_features']
+    __constants__ = ["in_features", "out_features"]
     in_features: int
     out_features: int
     weight: torch.Tensor
 
     def __init__(
-            self, 
-            in_features: int, 
-            out_features: int,
-            bias=False,  
-            groupsize: int = 128, 
-            inner_k_tiles: int = 8,
+        self,
+        in_features: int,
+        out_features: int,
+        bias=False,
+        groupsize: int = 128,
+        inner_k_tiles: int = 8,
     ) -> None:
         super().__init__()
         self.padding = not self._check_linear_int4_k(in_features, groupsize, inner_k_tiles)
         if self.padding:
             self.origin_in_features = in_features
             in_features = find_multiple(in_features, 1024)
 
@@ -73,90 +67,95 @@
         self.groupsize = groupsize
         self.inner_k_tiles = inner_k_tiles
 
         assert out_features % 8 == 0, "require out_features % 8 == 0"
         assert in_features % (inner_k_tiles * 16) == 0, "require in_features % (innerKTiles * 16) == 0"
         self.register_buffer(
             "weight",
-            torch.empty((out_features // 8, in_features // (inner_k_tiles * 16), 32, inner_k_tiles // 2), dtype=torch.int32)
+            torch.empty(
+                (
+                    out_features // 8,
+                    in_features // (inner_k_tiles * 16),
+                    32,
+                    inner_k_tiles // 2,
+                ),
+                dtype=torch.int32,
+            ),
         )
         self.register_buffer(
             "scales_and_zeros",
-            torch.empty((in_features // groupsize, out_features, 2), dtype=torch.bfloat16)
+            torch.empty((in_features // groupsize, out_features, 2), dtype=torch.bfloat16),
         )
 
     def forward(self, input: torch.Tensor) -> torch.Tensor:
         input = input.to(torch.bfloat16)
         if self.padding:
             import torch.nn.functional as F
+
             input = F.pad(input, pad=(0, self.in_features - self.origin_in_features))
-        return self._linear_forward_int4(input,
-                                        self.weight, 
-                                        self.scales_and_zeros, 
-                                        self.out_features, 
-                                        self.groupsize)
-        
+        return self._linear_forward_int4(input, self.weight, self.scales_and_zeros, self.out_features, self.groupsize)
+
     def _check_linear_int4_k(self, in_features: int, groupsize: int, inner_k_tiles: int) -> bool:
         """check if the input features are compatible with the linear int4 kernel
 
         Args:
             in_features (int): the number of input features
             groupsize (int): the group size
             inner_k_tiles (int): the number of inner k tiles
         """
         return in_features % (inner_k_tiles * 16) == 0 and in_features % groupsize == 0
-    
+
     def _linear_forward_int4(self, x, weight_int4pack, scales_and_zeros, out_features, groupsize):
         origin_x_size = x.size()
         x = x.reshape(-1, origin_x_size[-1])
         c = torch.ops.aten._weight_int4pack_mm(x, weight_int4pack, groupsize, scales_and_zeros)
         new_shape = origin_x_size[:-1] + (out_features,)
         c = c.reshape(new_shape)
         return c
-    
-    
+
+
 class LoRALinear(nn.Module):
     def __init__(
         self,
         in_features: int,
         out_features: int,
         r: int = 0,
         alpha: int = 1,
         dropout: float = 0.0,
-        **kwargs
+        **kwargs,
     ):
         super().__init__()
         assert r >= 0, "r must be greater than or equal to 0"
         self.r = r
         self.alpha = alpha
         self.linear = nn.Linear(in_features=in_features, out_features=out_features, **kwargs)
         if r > 0:
             self.dropout = nn.Dropout(dropout)
             self.lora_A = nn.Parameter(torch.empty(r, in_features))
             self.lora_B = nn.Parameter(torch.empty(out_features, r))
             self.scale = self.alpha / self.r
             self.reset_parameters()
         self.merged = False
-        
+
     def forward(self, x: torch.Tensor) -> torch.Tensor:
         x1 = self.linear(x)
         if self.merged or self.r == 0:
             return x1
         x2 = (self.dropout(x) @ self.lora_A.T @ self.lora_B.T) * self.scale
         return x1 + x2
-        
+
     def reset_parameters(self) -> None:
         """Reset all the weights, even including pretrained ones."""
         if hasattr(self, "lora_A"):
             # initialize A the same way as the default for nn.Linear and B to zero
             # Wondering why 'a' is equal to math.sqrt(5)?: https://github.com/pytorch/pytorch/issues/15314
             nn.init.kaiming_uniform_(self.lora_A, a=math.sqrt(5))
             nn.init.zeros_(self.lora_B)
-            
+
     def get_delta_w(self):
-        return (self.lora_B @ self.lora_A )* self.scale
-    
+        return (self.lora_B @ self.lora_A) * self.scale
+
     def merge(self):
         if self.r == 0:
             return
         self.linear.weight.data += self.get_delta_w()
-        self.merged = True
+        self.merged = True
```

### Comparing `osc_llm-0.1.4/osc_llm/layers/normalization.py` & `osc_llm-0.1.5/osc_llm/layers/normalization.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,26 +1,24 @@
 import torch
 from ..config import registry
 
 
 @registry.layers.register("RMSNorm")
 class RMSNorm(torch.nn.Module):
-    def __init__(self,
-                 n_in: int,
-                 eps: float = 1e-5) -> None:
+    def __init__(self, n_in: int, eps: float = 1e-5) -> None:
         super().__init__()
         self.weight = torch.nn.Parameter(torch.ones(n_in))
         self.eps = eps
-        
+
     def forward(self, x):
         norm = torch.mean(x.pow(2), dim=-1, keepdim=True) + self.eps
         x = x * torch.rsqrt(norm)
         x = x * self.weight
         return x
-    
+
     def reset_parameters(self):
         self.weight.data.fill_(1.0)
-        
-        
+
+
 @registry.layers.register("LayerNorm")
 def LayerNorm(n_in: int, eps: float = 1e-5, elementwise_affine: bool = True, bias: bool = True):
-    return torch.nn.LayerNorm(n_in, eps=eps, elementwise_affine=elementwise_affine, bias=bias)
+    return torch.nn.LayerNorm(n_in, eps=eps, elementwise_affine=elementwise_affine, bias=bias)
```

### Comparing `osc_llm-0.1.4/osc_llm/model_helpers/base.py` & `osc_llm-0.1.5/osc_llm/model_helpers/base.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,124 +1,132 @@
-import json 
+import json
 from pathlib import Path
 from typing import Dict
 import torch
 from ..config import Config, registry
 from ..utils import build_model
 from ..tokenizer import Tokenizer
 from ..chat_templates import ChatTemplate
 from wasabi import msg
 
 
-
 class HFModelHelper:
-    """huggingface模型转换工具基类,一般情况下只需要完成`weight_map`属性和`osc_config`属性即可。
-    """
-    
+    """huggingface模型转换工具基类,一般情况下只需要完成`weight_map`属性和`osc_config`属性即可。"""
+
     hf_architecture: str
-    
+
     def __init__(self, checkpoint_dir: str):
         self.checkpoint_dir = Path(checkpoint_dir)
         with open(self.checkpoint_dir / "config.json", "r") as f:
             self.hf_config = json.load(f)
-        assert self.hf_architecture in self.hf_config['architectures'], f'Only support {self.hf_architecture} model, current model is {self.hf_config["architectures"]}'
+        assert (
+            self.hf_architecture in self.hf_config["architectures"]
+        ), f'Only support {self.hf_architecture} model, current model is {self.hf_config["architectures"]}'
         try:
             self.tokenizer = Tokenizer(self.checkpoint_dir)
         except Exception:
             msg.warn("No tokenizer found")
             self.tokenizer = None
-    
+
     @property
     def weight_map(self) -> Dict:
         """用来进行参数名称转换"""
         raise NotImplementedError("Method not implemented")
-    
+
     @property
     def osc_config(self) -> Config:
         """用来构建osc格式模型的配置文件"""
         raise NotImplementedError("Method not implemented")
-    
+
     def convert_checkpoint(self, save_dir: str, add_chat_template: bool = True):
         """将huggingface模型转换为osc格式模型
 
         Args:
             save_dir (str): 保存目录
         """
-        pytorch_model = Path(self.checkpoint_dir) / 'pytorch_model.bin'
-        pytorch_idx_file = Path(self.checkpoint_dir) / 'pytorch_model.bin.index.json'
+        pytorch_model = Path(self.checkpoint_dir) / "pytorch_model.bin"
+        pytorch_idx_file = Path(self.checkpoint_dir) / "pytorch_model.bin.index.json"
         if pytorch_model.exists() or pytorch_idx_file.exists():
             sd = self.convert_pytorch_format()
-        safetensors_model = Path(self.checkpoint_dir) / 'model.safetensors'
-        safetensors_idx_file = Path(self.checkpoint_dir) / 'model.safetensors.index.json'
+        safetensors_model = Path(self.checkpoint_dir) / "model.safetensors"
+        safetensors_idx_file = Path(self.checkpoint_dir) / "model.safetensors.index.json"
         if safetensors_model.exists() or safetensors_idx_file.exists():
             sd = self.convert_safetensor_format()
-        if not pytorch_model.exists() and not safetensors_model.exists() and not pytorch_idx_file.exists() and not safetensors_idx_file.exists():
+        if (
+            not pytorch_model.exists()
+            and not safetensors_model.exists()
+            and not pytorch_idx_file.exists()
+            and not safetensors_idx_file.exists()
+        ):
             raise FileNotFoundError("No pytorch model file found")
         out_dir = Path(save_dir)
         if not out_dir.exists():
             out_dir.mkdir(parents=True)
-        torch.save(sd, out_dir / 'osc_model.pth')
+        torch.save(sd, out_dir / "osc_model.pth")
         if add_chat_template:
             chat_template = self.get_chat_template()
             if chat_template:
                 template_config = chat_template.get_config()
         config = self.osc_config.merge(template_config)
-        config = Config(data=config, section_order=['model', 'chat_template'])
-        config.to_disk(out_dir / 'config.cfg')
+        config = Config(data=config, section_order=["model", "chat_template"])
+        config.to_disk(out_dir / "config.cfg")
         if self.tokenizer:
             self.tokenizer.save(out_dir)
-    
+
     def convert_pytorch_format(self):
         sd = {}
         wmap = self.weight_map
-        index_file = self.checkpoint_dir / 'pytorch_model.bin.index.json'
+        index_file = self.checkpoint_dir / "pytorch_model.bin.index.json"
         if index_file.exists():
-            with open(index_file, 'r') as f:
+            with open(index_file, "r") as f:
                 index = json.load(f)
-            files = [self.checkpoint_dir / file  for file in set(index['weight_map'].values())]
+            files = [self.checkpoint_dir / file for file in set(index["weight_map"].values())]
         else:
-            files = [self.checkpoint_dir / 'pytorch_model.bin']
-        assert len(files) > 0, 'No pytorch model file found'
+            files = [self.checkpoint_dir / "pytorch_model.bin"]
+        assert len(files) > 0, "No pytorch model file found"
         for file in files:
-            weights = torch.load(str(file), map_location='cpu', weights_only=True, mmap=True)
+            weights = torch.load(str(file), map_location="cpu", weights_only=True, mmap=True)
             for key in weights:
                 if key not in wmap:
                     msg.warn(f"{key} not in wmap")
                     continue
                 sd[wmap[key]] = weights[key]
         return sd
-        
+
     def convert_safetensor_format(self):
         sd = {}
         wmap = self.weight_map
-        index_file = self.checkpoint_dir / 'model.safetensors.index.json'
+        index_file = self.checkpoint_dir / "model.safetensors.index.json"
         if index_file.exists():
-            with open(index_file, 'r') as f:
+            with open(index_file, "r") as f:
                 index = json.load(f)
-            files = [self.checkpoint_dir / file  for file in set(index['weight_map'].values())]
+            files = [self.checkpoint_dir / file for file in set(index["weight_map"].values())]
         else:
-            files = [self.checkpoint_dir / 'model.safetensors']
-        assert len(files) > 0, 'No pytorch model file found'
+            files = [self.checkpoint_dir / "model.safetensors"]
+        assert len(files) > 0, "No pytorch model file found"
         try:
             from safetensors import safe_open
         except Exception:
             raise ImportError("Please install safetensors first, run `pip install safetensors`")
         for file in files:
-            with safe_open(file, framework='pt') as f:
+            with safe_open(file, framework="pt") as f:
                 for key in f.keys():
                     if key not in wmap:
                         msg.warn(f"{key} not in wmap")
                         continue
                     sd[wmap[key]] = f.get_tensor(key)
         return sd
-        
-    def load_checkpoint(self, checkpoint_name: str = 'osc_model.pth', device: str = 'cpu'):
+
+    def load_checkpoint(self, checkpoint_name: str = "osc_model.pth", device: str = "cpu"):
         model = build_model(config=self.osc_config)
-        model.load_state_dict(torch.load(str(self.checkpoint_dir / checkpoint_name), mmap=True, weights_only=True), assign=True)
+        model.load_state_dict(
+            torch.load(str(self.checkpoint_dir / checkpoint_name), mmap=True, weights_only=True),
+            assign=True,
+        )
         model.to(device)
         return model.eval()
-    
+
     def get_chat_template(self) -> ChatTemplate:
         for k, v in registry.chat_templates.get_all().items():
-            if k in self.checkpoint_dir.name: # 简单通过名称匹配
+            if k in self.checkpoint_dir.name:  # 简单通过名称匹配
                 return v
-        return None
+        return None
```

### Comparing `osc_llm-0.1.4/osc_llm/model_helpers/chatglm.py` & `osc_llm-0.1.5/osc_llm/model_helpers/chatglm.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,37 +1,45 @@
 from .base import HFModelHelper
 from ..config import Config
 
 
-
 class ChatGLM3Helper(HFModelHelper):
-    
     hf_architecture: str = "ChatGLMModel"
 
     @property
     def weight_map(self):
-        
         weight_map = {
             "transformer.embedding.word_embeddings.weight": "embedding.embed.weight",
             "transformer.encoder.final_layernorm.weight": "head_norm.weight",
-            "transformer.output_layer.weight": "head.weight"
+            "transformer.output_layer.weight": "head.weight",
         }
-        
-        for i in range(self.hf_config['num_layers']):
+
+        for i in range(self.hf_config["num_layers"]):
             weight_map[f"transformer.encoder.layers.{i}.input_layernorm.weight"] = f"blocks.{i}.attention_norm.weight"
-            weight_map[f"transformer.encoder.layers.{i}.post_attention_layernorm.weight"] = f"blocks.{i}.feedforward_norm.weight"
-            weight_map[f"transformer.encoder.layers.{i}.self_attention.query_key_value.weight"] = f"blocks.{i}.attention.qkv_proj.weight"
-            weight_map[f"transformer.encoder.layers.{i}.self_attention.query_key_value.bias"] = f"blocks.{i}.attention.qkv_proj.bias"
-            weight_map[f"transformer.encoder.layers.{i}.self_attention.dense.weight"] = f"blocks.{i}.attention.o_proj.weight"
-            weight_map[f"transformer.encoder.layers.{i}.mlp.dense_h_to_4h.weight"] = f"blocks.{i}.feedforward.up_gate_proj.weight"
-            weight_map[f"transformer.encoder.layers.{i}.mlp.dense_4h_to_h.weight"] = f"blocks.{i}.feedforward.down_proj.weight"
-            
+            weight_map[f"transformer.encoder.layers.{i}.post_attention_layernorm.weight"] = (
+                f"blocks.{i}.feedforward_norm.weight"
+            )
+            weight_map[f"transformer.encoder.layers.{i}.self_attention.query_key_value.weight"] = (
+                f"blocks.{i}.attention.qkv_proj.weight"
+            )
+            weight_map[f"transformer.encoder.layers.{i}.self_attention.query_key_value.bias"] = (
+                f"blocks.{i}.attention.qkv_proj.bias"
+            )
+            weight_map[f"transformer.encoder.layers.{i}.self_attention.dense.weight"] = (
+                f"blocks.{i}.attention.o_proj.weight"
+            )
+            weight_map[f"transformer.encoder.layers.{i}.mlp.dense_h_to_4h.weight"] = (
+                f"blocks.{i}.feedforward.up_gate_proj.weight"
+            )
+            weight_map[f"transformer.encoder.layers.{i}.mlp.dense_4h_to_h.weight"] = (
+                f"blocks.{i}.feedforward.down_proj.weight"
+            )
+
         return weight_map
-    
-    
+
     @property
     def osc_config(self) -> Config:
         tempelate = """
         [model]
         @architectures = "TransformerDecoder"
         n_blocks = {num_layers}
         block_size = {seq_length}
@@ -67,8 +75,8 @@
 
         [model.norm]
         @layers = "RMSNorm"
         n_in = {hidden_size}
         eps = {layernorm_epsilon}
         """
         config_str = tempelate.format(**self.hf_config)
-        return Config().from_str(config_str)
+        return Config().from_str(config_str)
```

### Comparing `osc_llm-0.1.4/osc_llm/model_helpers/llama.py` & `osc_llm-0.1.5/osc_llm/model_helpers/llama.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,41 +1,38 @@
 from typing import Dict
 from ..config import Config, registry
 from .base import HFModelHelper
 
 
-
 @registry.model_helpers.register("LlamaForCausalLM")
 class LlamaHelper(HFModelHelper):
-        
     hf_architecture = "LlamaForCausalLM"
-    
+
     @property
     def weight_map(self) -> Dict:
-        """获取llama2权重映射表
-        """
+        """获取llama2权重映射表"""
         weight_map = {
-        "model.embed_tokens.weight": "embedding.embed.weight",
-        "model.norm.weight": "head_norm.weight",
-        "lm_head.weight": "head.weight",
+            "model.embed_tokens.weight": "embedding.embed.weight",
+            "model.norm.weight": "head_norm.weight",
+            "lm_head.weight": "head.weight",
         }
-        
-        for i in range(self.hf_config['num_hidden_layers']):
+
+        for i in range(self.hf_config["num_hidden_layers"]):
             weight_map[f"model.layers.{i}.input_layernorm.weight"] = f"blocks.{i}.attention_norm.weight"
             weight_map[f"model.layers.{i}.post_attention_layernorm.weight"] = f"blocks.{i}.feedforward_norm.weight"
             weight_map[f"model.layers.{i}.self_attn.q_proj.weight"] = f"blocks.{i}.attention.q_proj.weight"
             weight_map[f"model.layers.{i}.self_attn.k_proj.weight"] = f"blocks.{i}.attention.k_proj.weight"
             weight_map[f"model.layers.{i}.self_attn.v_proj.weight"] = f"blocks.{i}.attention.v_proj.weight"
             weight_map[f"model.layers.{i}.self_attn.o_proj.weight"] = f"blocks.{i}.attention.o_proj.weight"
             weight_map[f"model.layers.{i}.mlp.gate_proj.weight"] = f"blocks.{i}.feedforward.gate_proj.weight"
             weight_map[f"model.layers.{i}.mlp.up_proj.weight"] = f"blocks.{i}.feedforward.up_proj.weight"
             weight_map[f"model.layers.{i}.mlp.down_proj.weight"] = f"blocks.{i}.feedforward.down_proj.weight"
-            
+
         return weight_map
-    
+
     @property
     def osc_config(self) -> Config:
         tempelate = """
         [model]
         @architectures = "TransformerDecoder"
         n_blocks = {num_hidden_layers}
         block_size = {max_length}
@@ -69,12 +66,12 @@
         bias = "False"
 
         [model.norm]
         @layers = "RMSNorm"
         n_in = {hidden_size}
         eps = {rms_norm_eps}
         """
-        self.hf_config['max_length'] = self.hf_config.get('max_length', self.hf_config['max_position_embeddings'])
-        self.hf_config['rope_theta'] = self.hf_config.get('rope_theta', 10000)
-        self.hf_config['rms_norm_eps'] = self.hf_config.get('rms_norm_eps', 1e-5)
+        self.hf_config["max_length"] = self.hf_config.get("max_length", self.hf_config["max_position_embeddings"])
+        self.hf_config["rope_theta"] = self.hf_config.get("rope_theta", 10000)
+        self.hf_config["rms_norm_eps"] = self.hf_config.get("rms_norm_eps", 1e-5)
         config_str = tempelate.format(**self.hf_config)
-        return Config().from_str(config_str)
+        return Config().from_str(config_str)
```

### Comparing `osc_llm-0.1.4/osc_llm/model_helpers/qwen.py` & `osc_llm-0.1.5/osc_llm/model_helpers/qwen.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,44 +1,41 @@
 from typing import Dict
 from ..config import Config, registry
 from .base import HFModelHelper
 
 
-
 @registry.model_helpers.register("Qwen2ForCausalLM")
 class Qwen2Helper(HFModelHelper):
-    
     hf_architecture = "Qwen2ForCausalLM"
-    
+
     @property
     def weight_map(self) -> Dict:
-        """获取qwen2权重映射表
-        """
+        """获取qwen2权重映射表"""
         weight_map = {
             "model.embed_tokens.weight": "embedding.embed.weight",
             "model.norm.weight": "head_norm.weight",
             "lm_head.weight": "head.weight",
         }
-        
-        for i in range(self.hf_config['num_hidden_layers']):
+
+        for i in range(self.hf_config["num_hidden_layers"]):
             weight_map[f"model.layers.{i}.input_layernorm.weight"] = f"blocks.{i}.attention_norm.weight"
             weight_map[f"model.layers.{i}.post_attention_layernorm.weight"] = f"blocks.{i}.feedforward_norm.weight"
             weight_map[f"model.layers.{i}.self_attn.q_proj.weight"] = f"blocks.{i}.attention.q_proj.weight"
             weight_map[f"model.layers.{i}.self_attn.q_proj.bias"] = f"blocks.{i}.attention.q_proj.bias"
             weight_map[f"model.layers.{i}.self_attn.k_proj.weight"] = f"blocks.{i}.attention.k_proj.weight"
             weight_map[f"model.layers.{i}.self_attn.k_proj.bias"] = f"blocks.{i}.attention.k_proj.bias"
             weight_map[f"model.layers.{i}.self_attn.v_proj.weight"] = f"blocks.{i}.attention.v_proj.weight"
             weight_map[f"model.layers.{i}.self_attn.v_proj.bias"] = f"blocks.{i}.attention.v_proj.bias"
             weight_map[f"model.layers.{i}.self_attn.o_proj.weight"] = f"blocks.{i}.attention.o_proj.weight"
             weight_map[f"model.layers.{i}.mlp.gate_proj.weight"] = f"blocks.{i}.feedforward.gate_proj.weight"
             weight_map[f"model.layers.{i}.mlp.up_proj.weight"] = f"blocks.{i}.feedforward.up_proj.weight"
             weight_map[f"model.layers.{i}.mlp.down_proj.weight"] = f"blocks.{i}.feedforward.down_proj.weight"
-            
+
         return weight_map
-    
+
     @property
     def osc_config(self) -> Config:
         tempelate = """
         [model]
         @architectures = "TransformerDecoder"
         n_blocks = {num_hidden_layers}
         block_size = {max_length}
@@ -75,64 +72,73 @@
         bias = "False"
 
         [model.norm]
         @layers = "RMSNorm"
         n_in = {hidden_size}
         eps = 0.000001
         """
-        self.hf_config['max_length'] = self.hf_config.get('max_length', self.hf_config['max_position_embeddings'])
+        self.hf_config["max_length"] = self.hf_config.get("max_length", self.hf_config["max_position_embeddings"])
         config_str = tempelate.format(**self.hf_config)
         return Config().from_str(config_str)
-    
+
 
 @registry.model_helpers.register("Qwen2MoeForCausalLM")
 class Qwen2MoeHelper(HFModelHelper):
-    
     hf_architecture = "Qwen2MoeForCausalLM"
-    
+
     @property
     def weight_map(self) -> Dict:
-        """qwen2moe权重映射表
-        """
+        """qwen2moe权重映射表"""
         weight_map = {
             "model.embed_tokens.weight": "embedding.embed.weight",
             "model.norm.weight": "head_norm.weight",
             "lm_head.weight": "head.weight",
         }
-        
-        for i in range(self.hf_config['num_hidden_layers']):
+
+        for i in range(self.hf_config["num_hidden_layers"]):
             weight_map[f"model.layers.{i}.input_layernorm.weight"] = f"blocks.{i}.attention_norm.weight"
             weight_map[f"model.layers.{i}.post_attention_layernorm.weight"] = f"blocks.{i}.feedforward_norm.weight"
             weight_map[f"model.layers.{i}.self_attn.q_proj.weight"] = f"blocks.{i}.attention.q_proj.weight"
             weight_map[f"model.layers.{i}.self_attn.q_proj.bias"] = f"blocks.{i}.attention.q_proj.bias"
             weight_map[f"model.layers.{i}.self_attn.k_proj.weight"] = f"blocks.{i}.attention.k_proj.weight"
             weight_map[f"model.layers.{i}.self_attn.k_proj.bias"] = f"blocks.{i}.attention.k_proj.bias"
             weight_map[f"model.layers.{i}.self_attn.v_proj.weight"] = f"blocks.{i}.attention.v_proj.weight"
             weight_map[f"model.layers.{i}.self_attn.v_proj.bias"] = f"blocks.{i}.attention.v_proj.bias"
             weight_map[f"model.layers.{i}.self_attn.o_proj.weight"] = f"blocks.{i}.attention.o_proj.weight"
             weight_map[f"model.layers.{i}.mlp.gate.weight"] = f"blocks.{i}.feedforward.gate.weight"
-            
+
             # gate
             weight_map[f"model.layers.{i}.mlp.gate.weight"] = f"blocks.{i}.feedforward.gate.weight"
-            
+
             # shared expert
-            weight_map[f"model.layers.{i}.mlp.shared_expert.up_proj.weight"] = f"blocks.{i}.feedforward.shared_expert.up_proj.weight"
-            weight_map[f"model.layers.{i}.mlp.shared_expert.down_proj.weight"] = f"blocks.{i}.feedforward.shared_expert.down_proj.weight"
-            weight_map[f"model.layers.{i}.mlp.shared_expert.gate_proj.weight"] = f"blocks.{i}.feedforward.shared_expert.gate_proj.weight"
+            weight_map[f"model.layers.{i}.mlp.shared_expert.up_proj.weight"] = (
+                f"blocks.{i}.feedforward.shared_expert.up_proj.weight"
+            )
+            weight_map[f"model.layers.{i}.mlp.shared_expert.down_proj.weight"] = (
+                f"blocks.{i}.feedforward.shared_expert.down_proj.weight"
+            )
+            weight_map[f"model.layers.{i}.mlp.shared_expert.gate_proj.weight"] = (
+                f"blocks.{i}.feedforward.shared_expert.gate_proj.weight"
+            )
             weight_map[f"model.layers.{i}.mlp.shared_expert_gate.weight"] = f"blocks.{i}.feedforward.shared_gate.weight"
-            
+
             # experts
-            for j in range(self.hf_config['num_experts']):
-                weight_map[f"model.layers.{i}.mlp.experts.{j}.up_proj.weight"] = f"blocks.{i}.feedforward.experts.{j}.up_proj.weight"
-                weight_map[f"model.layers.{i}.mlp.experts.{j}.down_proj.weight"] = f"blocks.{i}.feedforward.experts.{j}.down_proj.weight"
-                weight_map[f"model.layers.{i}.mlp.experts.{j}.gate_proj.weight"] = f"blocks.{i}.feedforward.experts.{j}.gate_proj.weight"
-            
+            for j in range(self.hf_config["num_experts"]):
+                weight_map[f"model.layers.{i}.mlp.experts.{j}.up_proj.weight"] = (
+                    f"blocks.{i}.feedforward.experts.{j}.up_proj.weight"
+                )
+                weight_map[f"model.layers.{i}.mlp.experts.{j}.down_proj.weight"] = (
+                    f"blocks.{i}.feedforward.experts.{j}.down_proj.weight"
+                )
+                weight_map[f"model.layers.{i}.mlp.experts.{j}.gate_proj.weight"] = (
+                    f"blocks.{i}.feedforward.experts.{j}.gate_proj.weight"
+                )
+
         return weight_map
-    
-    
+
     @property
     def osc_config(self) -> Config:
         tempelate = """
         [model]
         @architectures = "TransformerDecoder"
         n_blocks = {num_hidden_layers}
         block_size = {max_length}
@@ -195,10 +201,10 @@
         bias = "False"
 
         [model.norm]
         @layers = "RMSNorm"
         n_in = {hidden_size}
         eps = {rms_norm_eps}
         """
-        self.hf_config['max_length'] = self.hf_config.get('max_length', self.hf_config['max_position_embeddings'])
+        self.hf_config["max_length"] = self.hf_config.get("max_length", self.hf_config["max_position_embeddings"])
         config_str = tempelate.format(**self.hf_config)
-        return Config().from_str(config_str)
+        return Config().from_str(config_str)
```

### Comparing `osc_llm-0.1.4/osc_llm/quantizers/base.py` & `osc_llm-0.1.5/osc_llm/quantizers/base.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,27 +1,23 @@
 from abc import ABC, abstractmethod
 import torch.nn as nn
 from confection import Config
 
 
-
 class Quantizer(ABC):
-    
-    
     @abstractmethod
     def quantize(self, model: nn.Module) -> nn.Module:
-        """在线量化模型,返回量化后的模型
-        """
+        """在线量化模型,返回量化后的模型"""
         raise NotImplementedError
-    
+
     @abstractmethod
     def convert_for_runtime(self, model: nn.Module) -> nn.Module:
         """仅将模型的结构转化为量化后的结构,并不对数据进行量化。
 
         Args:
             model (nn.Module): 待转换模型,不需要加载模型状态字典
         """
         raise NotImplementedError
-    
+
     @property
     def quantizer_config(self) -> Config:
-        raise NotImplementedError
+        raise NotImplementedError
```

### Comparing `osc_llm-0.1.4/osc_llm/quantizers/int4.py` & `osc_llm-0.1.5/osc_llm/quantizers/int4.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,142 +1,146 @@
-import torch 
+import torch
 import torch.nn as nn
 from typing import Union, Literal
 from pathlib import Path
 from ..layers.linear import WeightOnlyInt4Linear
 from ..utils import find_multiple
 from .base import Quantizer
 from ..config import registry
 from confection import Config
 
-    
+
 @registry.quantizers.register("WeightOnlyInt4Quantizer")
 class WeightOnlyInt4Quantizer(Quantizer):
-    
-    def __init__(self, 
-                 groupsize: Literal[32, 64, 128, 256] = 32, 
-                 inner_k_tiles: Literal[2, 4, 8] = 8, 
-                 padding_allowed: bool = True):
+    def __init__(
+        self,
+        groupsize: Literal[32, 64, 128, 256] = 32,
+        inner_k_tiles: Literal[2, 4, 8] = 8,
+        padding_allowed: bool = True,
+    ):
         self.groupsize = groupsize
         self.inner_k_tiles = inner_k_tiles
         self.padding_allowed = padding_allowed
         assert groupsize in [32, 64, 128, 256]
         assert inner_k_tiles in [2, 4, 8]
-        
+
     def quantize(self, model: nn.Module) -> nn.Module:
         for name, children in model.named_children():
             if isinstance(children, torch.nn.Linear):
                 out_features = children.out_features
                 in_features = children.in_features
                 assert not children.bias
                 assert out_features % 8 == 0, "require out_features % 8 == 0"
                 weight = children.weight.data
                 if not _check_linear_int4_k(in_features, self.groupsize, self.inner_k_tiles):
                     if self.padding_allowed:
                         import torch.nn.functional as F
+
                         print(f"warning: {name} is padded to satisfy in_features % 1024 == 0")
                         padded_in_features = find_multiple(in_features, 1024)
                         weight = F.pad(weight, pad=(0, padded_in_features - in_features))
                         in_features = padded_in_features
                     else:
-                        print(f"warning: {name} is skipped, int4 requires that in_features is 32, 64, or is divisible by 1024, " +
-                            "and that groupsize and inner_k_tiles*16 evenly divide into it")
+                        print(
+                            f"warning: {name} is skipped, int4 requires that in_features is 32, 64, or is divisible by 1024, "
+                            + "and that groupsize and inner_k_tiles*16 evenly divide into it"
+                        )
                         continue
                 weight_int4pack, scales_and_zeros = prepare_int4_weight_and_scales_and_zeros(
                     weight.to(torch.bfloat16), self.groupsize, self.inner_k_tiles
                 )
                 int4_linear = WeightOnlyInt4Linear(
                     in_features=in_features,
                     out_features=out_features,
                     groupsize=self.groupsize,
-                    inner_k_tiles=self.inner_k_tiles
+                    inner_k_tiles=self.inner_k_tiles,
                 )
                 int4_linear.weight = weight_int4pack
                 int4_linear.scales_and_zeros = scales_and_zeros
                 setattr(model, name, int4_linear)
             else:
                 self.quantize(children)
         return model
-                
 
     @torch.no_grad()
     def save_quantized_state_dict(self, model: nn.Module, save_path: Union[str, Path]):
         cur_state_dict = model.state_dict()
         for fqn, mod in model.named_modules():
             if isinstance(mod, torch.nn.Linear):
                 assert not mod.bias
                 out_features = mod.out_features
                 in_features = mod.in_features
                 assert out_features % 8 == 0, "require out_features % 8 == 0"
                 weight = mod.weight.data
                 if not _check_linear_int4_k(in_features, self.groupsize, self.inner_k_tiles):
                     if self.padding_allowed:
                         import torch.nn.functional as F
+
                         print(f"warning: {fqn} is padded to satisfy in_features % 1024 == 0")
                         padded_in_features = find_multiple(in_features, 1024)
                         weight = F.pad(weight, pad=(0, padded_in_features - in_features))
                     else:
-                        print(f"warning: {fqn} is skipped, int4 requires that in_features is 32, 64, or is divisible by 1024, " +
-                            "and that groupsize and inner_k_tiles*16 evenly divide into it")
+                        print(
+                            f"warning: {fqn} is skipped, int4 requires that in_features is 32, 64, or is divisible by 1024, "
+                            + "and that groupsize and inner_k_tiles*16 evenly divide into it"
+                        )
                         continue
                 weight_int4pack, scales_and_zeros = prepare_int4_weight_and_scales_and_zeros(
                     weight.to(torch.bfloat16), self.groupsize, self.inner_k_tiles
                 )
-                cur_state_dict[f"{fqn}.weight"] = weight_int4pack.to('cpu')
-                cur_state_dict[f"{fqn}.scales_and_zeros"] = scales_and_zeros.to('cpu')
+                cur_state_dict[f"{fqn}.weight"] = weight_int4pack.to("cpu")
+                cur_state_dict[f"{fqn}.scales_and_zeros"] = scales_and_zeros.to("cpu")
                 if cur_state_dict.get(f"{fqn}.bias") is not None:
                     # remove bias
-                    del cur_state_dict[f"{fqn}.bias"]                
+                    del cur_state_dict[f"{fqn}.bias"]
 
         save_path = Path(save_path)
         if save_path.exists():
             save_path.unlink()
         torch.save(cur_state_dict, save_path)
 
-    def convert_for_runtime(self, model:nn.Module, use_cuda: bool = True):
+    def convert_for_runtime(self, model: nn.Module, use_cuda: bool = True):
         replace_linear_int4(model, self.groupsize, self.inner_k_tiles, self.padding_allowed, use_cuda)
         return model
-    
+
     @property
     def quantizer_config(self) -> Config:
         config_str = f"""
         [quantizer]
         @quantizers = "WeightOnlyInt4Quantizer"
         groupsize = {self.groupsize}
         inner_k_tiles = {self.inner_k_tiles}
         padding_allowed = {self.padding_allowed}
         """
         config = Config().from_str(config_str)
         return config
-    
-    
-def _check_linear_int4_k(k, groupsize = 1, inner_k_tiles = 1):
+
+
+def _check_linear_int4_k(k, groupsize=1, inner_k_tiles=1):
     return k % groupsize == 0 and k % (inner_k_tiles * 16) == 0
 
 
 def replace_linear_int4(module, groupsize, inner_k_tiles, padding_allowed, use_cuda):
     for name, child in module.named_children():
         if isinstance(child, nn.Linear):
             if _check_linear_int4_k(child.in_features, groupsize, inner_k_tiles) or padding_allowed:
                 new_module = WeightOnlyInt4Linear(
-                    in_features=child.in_features, 
-                    out_features=child.out_features, 
+                    in_features=child.in_features,
+                    out_features=child.out_features,
                     bias=False,
-                    groupsize=groupsize, 
-                    inner_k_tiles=inner_k_tiles, 
+                    groupsize=groupsize,
+                    inner_k_tiles=inner_k_tiles,
                 )
                 setattr(module, name, new_module)
         else:
             replace_linear_int4(child, groupsize, inner_k_tiles, padding_allowed, use_cuda)
 
 
 def prepare_int4_weight_and_scales_and_zeros(weight_bf16, groupsize, inner_k_tiles):
-    weight_int32, scales_and_zeros = group_quantize_tensor(
-        weight_bf16, n_bit=4, groupsize=groupsize
-    )
+    weight_int32, scales_and_zeros = group_quantize_tensor(weight_bf16, n_bit=4, groupsize=groupsize)
     weight_int4pack = torch.ops.aten._convert_weight_to_int4pack(weight_int32, inner_k_tiles)
     return weight_int4pack, scales_and_zeros
 
 
 def group_quantize_tensor(w: nn.Module, n_bit: int = 4, groupsize: int = 128):
     scales, zeros = get_group_qparams(w, n_bit, groupsize)
     w_int32 = group_quantize_tensor_from_qparams(w, scales, zeros, n_bit, groupsize)
@@ -156,18 +160,16 @@
     assert torch.isnan(to_quant).sum() == 0
 
     max_val = to_quant.amax(dim=1, keepdim=True)
     min_val = to_quant.amin(dim=1, keepdim=True)
     max_int = 2**n_bit - 1
     scales = (max_val - min_val).clamp(min=1e-6) / max_int
     zeros = min_val + scales * (2 ** (n_bit - 1))
-    return scales.to(torch.bfloat16).reshape(w.shape[0], -1), zeros.to(
-        torch.bfloat16
-    ).reshape(w.shape[0], -1)
-    
+    return scales.to(torch.bfloat16).reshape(w.shape[0], -1), zeros.to(torch.bfloat16).reshape(w.shape[0], -1)
+
 
 def pack_scales_and_zeros(scales, zeros):
     assert scales.shape == zeros.shape
     assert scales.dtype == torch.bfloat16
     assert zeros.dtype == torch.bfloat16
     return (
         torch.cat(
@@ -182,15 +184,15 @@
     )
 
 
 def unpack_scales_and_zeros(scales_and_zeros):
     assert len(scales_and_zeros.shape) == 3 and scales_and_zeros.shape[2] == 2
     assert scales_and_zeros.dtype == torch.float
     return torch.split(scales_and_zeros.transpose(0, 1), 1, 2)
-    
+
 
 def group_quantize_tensor_from_qparams(w, scales, zeros, n_bit=4, groupsize=128):
     assert groupsize > 1
     # needed for GPTQ single column quantize
     if groupsize > w.shape[-1] and scales.shape[-1] == 1:
         groupsize = w.shape[-1]
 
@@ -201,16 +203,9 @@
     assert torch.isnan(to_quant).sum() == 0
 
     scales = scales.reshape(-1, 1)
     zeros = zeros.reshape(-1, 1)
     min_val = zeros - scales * (2 ** (n_bit - 1))
     max_int = 2**n_bit - 1
     min_int = 0
-    w_int32 = (
-        to_quant.sub(min_val)
-        .div(scales)
-        .round()
-        .clamp_(min_int, max_int)
-        .to(torch.int32)
-        .reshape_as(w)
-    )
-    return w_int32
+    w_int32 = to_quant.sub(min_val).div(scales).round().clamp_(min_int, max_int).to(torch.int32).reshape_as(w)
+    return w_int32
```

### Comparing `osc_llm-0.1.4/osc_llm/quantizers/int8.py` & `osc_llm-0.1.5/osc_llm/quantizers/int8.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,61 +2,75 @@
 from ..layers import Int8Linear
 from ..config import registry
 from confection import Config
 import torch.nn as nn
 import torch
 
 
-
 @registry.quantizers.register("Int8Quantizer")
 class Int8Quantizer(Quantizer):
     def quantize(self, model: nn.Module) -> nn.Module:
         for name, children in model.named_children():
             if isinstance(children, torch.nn.Linear):
-                int8_weight, scales, _ = self._dynamically_quantize_per_channel(children.weight.float(), -128, 127, torch.int8)
+                int8_weight, scales, _ = self._dynamically_quantize_per_channel(
+                    children.weight.float(), -128, 127, torch.int8
+                )
                 if hasattr(children, "bias") and children.bias is not None:
-                    int8_linear = Int8Linear(in_features=children.in_features, out_features=children.out_features, bias=True)
+                    int8_linear = Int8Linear(
+                        in_features=children.in_features,
+                        out_features=children.out_features,
+                        bias=True,
+                    )
                     int8_linear.bias = children.bias
                     int8_linear.weight = int8_weight
                     int8_linear.scales = scales
                 else:
-                    int8_linear = Int8Linear(in_features=children.in_features, out_features=children.out_features)
+                    int8_linear = Int8Linear(
+                        in_features=children.in_features,
+                        out_features=children.out_features,
+                    )
                     int8_linear.weight = int8_weight
                     int8_linear.scales = scales
                 setattr(model, name, int8_linear)
             else:
                 self.quantize(model=children)
         return model
-        
+
     def convert_for_runtime(self, model: nn.Module) -> nn.Module:
         model = self._replace_linear_weight_only_int8_per_channel(model)
         return model
-    
+
     @property
     def quantizer_config(self):
         config_str = """
         [quantizer]
         @quantizers = "Int8Quantizer"
         """
         config = Config().from_str(config_str)
         return config
-        
+
     def _replace_linear_weight_only_int8_per_channel(self, module: nn.Module) -> nn.Module:
         """递归替换module中的所有nn.Linear为WeightOnlyInt8Linear"""
         for name, child in module.named_children():
             if isinstance(child, nn.Linear):
                 if hasattr(child, "bias") and child.bias is not None:
-                    setattr(module, name, Int8Linear(child.in_features, child.out_features, bias=True))
+                    setattr(
+                        module,
+                        name,
+                        Int8Linear(child.in_features, child.out_features, bias=True),
+                    )
                 else:
                     setattr(module, name, Int8Linear(child.in_features, child.out_features))
             else:
                 self._replace_linear_weight_only_int8_per_channel(child)
         return module
-                
-    def _dynamically_quantize_per_channel(self, x, quant_min = -128, quant_max = 127, target_dtype: torch.dtype = torch.int8):
+
+    def _dynamically_quantize_per_channel(
+        self, x, quant_min=-128, quant_max=127, target_dtype: torch.dtype = torch.int8
+    ):
         # assumes symmetric quantization
         # assumes axis == 0
         # assumes dense memory format
         # TODO(future): relax ^ as needed
 
         # default setup for affine quantization of activations
         eps = torch.finfo(torch.float32).eps
@@ -80,8 +94,8 @@
         # quantize based on qmin/qmax/scales/zp
         # reference: https://www.internalfb.com/code/fbsource/[8edc275012b1]/fbcode/caffe2/torch/ao/quantization/fx/_decomposed.py?lines=63
         x_div = x / scales.unsqueeze(-1)
         x_round = torch.round(x_div)
         x_zp = x_round + zero_points.unsqueeze(-1)
         quant = torch.clamp(x_zp, quant_min, quant_max).to(target_dtype)
 
-        return quant, scales, zero_points
+        return quant, scales, zero_points
```

### Comparing `osc_llm-0.1.4/osc_llm/samplers/base.py` & `osc_llm-0.1.5/osc_llm/samplers/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 import torch
 from abc import ABC, abstractmethod
 
 
 class Sampler(ABC):
     """Sampler can be used to sample from a distribution given logits to get ids."""
-    
+
     @abstractmethod
     def logits_to_probs(self, logits: torch.Tensor) -> torch.Tensor:
         raise NotImplementedError
-    
+
     @abstractmethod
     def probs_to_ids(self, probs: torch.Tensor) -> torch.Tensor:
         raise NotImplementedError
-    
+
     @abstractmethod
     def get_config(self, section: str = "sampler"):
         raise NotImplementedError
-    
+
     def sample(self, logits: torch.Tensor) -> torch.Tensor:
         probs = self.logits_to_probs(logits)
         return self.probs_to_ids(probs)
-    
+
     def multinomial_sample_one(self, probs: torch.Tensor) -> torch.Tensor:
         distribution = torch.empty_like(probs).exponential_(1)
-        return torch.argmax(probs / distribution, dim=-1, keepdim=True).to(dtype=torch.int)
+        return torch.argmax(probs / distribution, dim=-1, keepdim=True).to(dtype=torch.int)
```

### Comparing `osc_llm-0.1.4/osc_llm/samplers/top_k.py` & `osc_llm-0.1.5/osc_llm/samplers/top_k.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,34 +2,34 @@
 from .base import Sampler
 import torch
 
 
 @registry.samplers.register("TopK")
 class TopK(Sampler):
     def __init__(
-        self, 
+        self,
         k: int = 10,
         temperature: float = 1.0,
-        ) -> None:
+    ) -> None:
         super().__init__()
-        self.temperature = 0.001 if temperature <=0 else temperature
-        self.k = k 
-        
+        self.temperature = 0.001 if temperature <= 0 else temperature
+        self.k = k
+
     def logits_to_probs(self, logits: torch.Tensor) -> torch.Tensor:
         logits = logits / self.temperature
         values, indices = torch.topk(logits, min(self.k, logits.shape[-1]), dim=-1)
         logits = torch.full_like(logits, float("-inf")).scatter_(-1, indices, values)
         probs = torch.softmax(logits, dim=-1)
         return probs
-    
+
     def probs_to_ids(self, probs: torch.Tensor) -> torch.Tensor:
         ids = self.multinomial_sample_one(probs=probs)
         return ids
-    
+
     def get_config(self, section: str = "sampler"):
         config_str = f"""
         [{section}]
         @samplers = TopK
         k = {self.k}
         temperature = {self.temperature}"""
         config = Config().from_str(config_str)
-        return config
+        return config
```

### Comparing `osc_llm-0.1.4/osc_llm/samplers/top_p.py` & `osc_llm-0.1.5/osc_llm/samplers/top_p.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,31 +4,37 @@
 
 
 @registry.samplers.register("TopP")
 class TopP(Sampler):
     def __init__(
         self,
         p: float = 0.5,
-        ):
+    ):
         super().__init__()
         self.p = p
-        
+
     def logits_to_probs(self, logits: torch.Tensor) -> torch.Tensor:
         probs, self.indices = logits.softmax(dim=-1).sort(descending=True)
         nucleus_mask = probs.cumsum(dim=-1) < self.p
-        nucleus_mask = torch.cat([nucleus_mask.new_ones(nucleus_mask.shape[:-1] + (1,)), nucleus_mask[..., :-1]], dim=-1)
+        nucleus_mask = torch.cat(
+            [
+                nucleus_mask.new_ones(nucleus_mask.shape[:-1] + (1,)),
+                nucleus_mask[..., :-1],
+            ],
+            dim=-1,
+        )
         probs = probs * nucleus_mask
         probs /= probs.sum(dim=-1, keepdim=True)
         return probs
-    
+
     def probs_to_ids(self, probs: torch.Tensor) -> torch.Tensor:
         descending_idx = self.multinomial_sample_one(probs)
         # 得到真实的下标
         return self.indices.gather(-1, descending_idx)
-    
+
     def get_config(self, section: str = "sampler"):
         config_str = f"""
         [{section}]
         @samplers = TopP
         p = {self.p}"""
         config = Config().from_str(config_str)
-        return config
+        return config
```

### Comparing `osc_llm-0.1.4/osc_llm/servers/openai.py` & `osc_llm-0.1.5/osc_llm/servers/openai.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,36 +4,38 @@
 from ..utils import random_uuid
 from ..samplers import TopK
 from typing import List, Optional, Dict, Union, Literal
 from pydantic import BaseModel, Field
 import torch
 import time
 
-    
+
 class ErrorResponse(BaseModel):
     object: str = "error"
     message: str
     type: str
     param: Optional[str] = None
     code: int
 
+
 class ModelPermission(BaseModel):
     id: str = Field(default_factory=lambda: f"modelperm-{random_uuid()}")
     object: str = "model_permission"
     created: int = Field(default_factory=lambda: int(time.time()))
     allow_create_engine: bool = False
     allow_sampling: bool = True
     allow_logprobs: bool = True
     allow_search_indices: bool = False
     allow_view: bool = True
     allow_fine_tuning: bool = False
     organization: str = "*"
     group: Optional[str] = None
     is_blocking: str = False
-    
+
+
 class ModelCard(BaseModel):
     id: str
     object: str = "model"
     created: int = Field(default_factory=lambda: int(time.time()))
     owned_by: str = "osc"
     root: Optional[str] = None
     parent: Optional[str] = None
@@ -50,15 +52,16 @@
     total_tokens: int = 0
     completion_tokens: Optional[int] = 0
 
 
 class ChatMessage(BaseModel):
     role: str
     content: str
-    
+
+
 class LogProbs(BaseModel):
     text_offset: List[int] = Field(default_factory=list)
     token_logprobs: List[Optional[float]] = Field(default_factory=list)
     tokens: List[str] = Field(default_factory=list)
     top_logprobs: Optional[List[Optional[Dict[int, float]]]] = None
 
 
@@ -72,34 +75,37 @@
 class ChatCompletionResponse(BaseModel):
     id: str = Field(default_factory=lambda: f"chatcmpl-{random_uuid()}")
     object: str = "chat.completion"
     created: int = Field(default_factory=lambda: int(time.time()))
     model: str
     choices: List[ChatCompletionResponseChoice]
     usage: UsageInfo
-    
+
+
 class DeltaMessage(BaseModel):
     role: Optional[str] = None
     content: Optional[str] = None
-    
+
+
 class ChatCompletionResponseStreamChoice(BaseModel):
     index: int
     delta: DeltaMessage
     logprobs: Optional[LogProbs] = None
     finish_reason: Optional[Literal["stop", "length"]] = None
 
 
 class ChatCompletionStreamResponse(BaseModel):
     id: str = Field(default_factory=lambda: f"chatcmpl-{random_uuid()}")
     object: str = "chat.completion.chunk"
     created: int = Field(default_factory=lambda: int(time.time()))
     model: str
     choices: List[ChatCompletionResponseStreamChoice]
     usage: Optional[UsageInfo] = Field(default=None)
-    
+
+
 class ChatCompletionRequest(BaseModel):
     model: str
     messages: List[Message]
     temperature: Optional[float] = 0.7
     top_p: Optional[float] = 1.0
     n: Optional[int] = 1
     max_tokens: Optional[int] = None
@@ -108,79 +114,109 @@
     stream: Optional[bool] = False
     logprobs: Optional[bool] = False
     top_logprobs: Optional[int] = None
     presence_penalty: Optional[float] = 0.0
     frequency_penalty: Optional[float] = 0.0
     logit_bias: Optional[Dict[str, float]] = None
     user: Optional[str] = None
-    
-    
-def main(checkpoint_dir: str,
-         engine: Literal['v1', 'v2'] = 'v1',
-         accelerator: Literal['cuda', 'cpu', 'gpu', 'auto'] = 'cuda',
-         devices: Union[int, List[int]] = 1,
-         max_length: Optional[int] = None,
-         host: str = '0.0.0.0',
-         port: int = 8000,
-         compile: bool = True):
+
+
+def main(
+    checkpoint_dir: str,
+    engine: Literal["v1", "v2"] = "v1",
+    accelerator: Literal["cuda", "cpu", "gpu", "auto"] = "cuda",
+    devices: Union[int, List[int]] = 1,
+    max_length: Optional[int] = None,
+    host: str = "0.0.0.0",
+    port: int = 8000,
+    compile: bool = True,
+):
     """openai接口服务
 
     Args:
         checkpoint_dir (str): checkpoint目录
         engine (Literal[&#39;v1&#39;, &#39;v2&#39;], optional): LLMEngine版本. Defaults to 'v1'.
         accelerator (Literal[&#39;cuda&#39;, &#39;cpu&#39;, &#39;gpu&#39;, &#39;auto&#39;], optional): 推理硬件. Defaults to 'cuda'.
         devices (Union[int, List[int]], optional): 设备数量或者设备的ID. Defaults to 1.
         host (str, optional): 主机地址. Defaults to '0.0.0.0'.
         port (int, optional): 端口号. Defaults to 8000.
         compile (bool, optional): 是否编译模型. Defaults to True.
     """
     from fastapi import FastAPI
     from fastapi.responses import StreamingResponse, JSONResponse
     import uvicorn
-    
+
     app = FastAPI(description="OpenAI API")
-    
+
     @app.post("/v1/chat/completions")
     def create_chat_completion(request: ChatCompletionRequest):
         with engine.fabric.init_tensor():
             input_ids = tokenizer.encode_messages(request.messages)
             input_pos = torch.arange(len(input_ids))
         engine.reset_sampler(sampler=TopK(k=100, temperature=request.temperature))
         stream = engine.run(input_ids=input_ids, stop_ids=tokenizer.stop_ids, input_pos=input_pos)
         stream_tokens = tokenizer.decode_stream(stream=stream)
-        
+
         if request.stream:
+
             def stream_content(stream_tokens):
                 for token in stream_tokens:
-                    data =  ChatCompletionStreamResponse(id=f"chatcmpl-{random_uuid()}", 
-                                                        model=request.model, 
-                                                        choices=[ChatCompletionResponseStreamChoice(index=0, delta=DeltaMessage(role='assistant', content=token))],
-                                                        usage=UsageInfo(prompt_tokens=0, total_tokens=0, completion_tokens=0)).model_dump_json(exclude_unset=True)
+                    data = ChatCompletionStreamResponse(
+                        id=f"chatcmpl-{random_uuid()}",
+                        model=request.model,
+                        choices=[
+                            ChatCompletionResponseStreamChoice(
+                                index=0,
+                                delta=DeltaMessage(role="assistant", content=token),
+                            )
+                        ],
+                        usage=UsageInfo(prompt_tokens=0, total_tokens=0, completion_tokens=0),
+                    ).model_dump_json(exclude_unset=True)
                     yield f"data: {data}\n\n"
                 yield "data: [DONE]\n\n"
+
             return StreamingResponse(content=stream_content(stream_tokens), media_type="text/event-stream")
         else:
             content = ""
             completion_tokens = 0
             for token in stream_tokens:
                 content += token
                 completion_tokens += 1
             prompt_tokens = len(input_ids)
             total_tokens = prompt_tokens + completion_tokens
-            response = ChatCompletionResponse(id=f"chatcmpl-{random_uuid()}",
-                                              model=request.model,
-                                              choices=[ChatCompletionResponseChoice(index=0, message=ChatMessage(role='assistant', content=content))],
-                                              usage=UsageInfo(prompt_tokens=prompt_tokens, total_tokens=total_tokens, completion_tokens=completion_tokens))
+            response = ChatCompletionResponse(
+                id=f"chatcmpl-{random_uuid()}",
+                model=request.model,
+                choices=[ChatCompletionResponseChoice(index=0, message=ChatMessage(role="assistant", content=content))],
+                usage=UsageInfo(
+                    prompt_tokens=prompt_tokens,
+                    total_tokens=total_tokens,
+                    completion_tokens=completion_tokens,
+                ),
+            )
             return JSONResponse(content=response.model_dump(exclude_unset=True))
-    
-    if engine == 'v1':
-        engine: LLMEngine = LLMEngineV1(checkpoint_dir, devices=devices, accelerator=accelerator, compile=compile, max_length=max_length)
+
+    if engine == "v1":
+        engine: LLMEngine = LLMEngineV1(
+            checkpoint_dir,
+            devices=devices,
+            accelerator=accelerator,
+            compile=compile,
+            max_length=max_length,
+        )
     else:
-        engine: LLMEngine = LLMEngineV2(checkpoint_dir, devices=devices, accelerator=accelerator, compile=compile, max_length=max_length)
+        engine: LLMEngine = LLMEngineV2(
+            checkpoint_dir,
+            devices=devices,
+            accelerator=accelerator,
+            compile=compile,
+            max_length=max_length,
+        )
     engine.setup()
     tokenizer = Tokenizer(checkpoint_dir=checkpoint_dir)
-    
+
     # Todo: 在启动模型编译的情况下第一次运行需要耗费很多时间(几分钟),如何在启动的时候预热模型?
     if compile:
         from wasabi import msg
+
         msg.warn("you are using compile mode, the first run may take a long time")
-    uvicorn.run(app=app, host=host, port=port)
+    uvicorn.run(app=app, host=host, port=port)
```

### Comparing `osc_llm-0.1.4/osc_llm/tokenizer.py` & `osc_llm-0.1.5/osc_llm/tokenizer.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,27 +4,28 @@
 import torch
 from .chat_templates import ChatTemplate, Message
 from sentencepiece import SentencePieceProcessor
 from tokenizers import Tokenizer as HFTokenizer
 
 
 class Tokenizer:
-    def __init__(self, 
-                 checkpoint_dir: Union[Path, str],
-                 chat_template: Optional[ChatTemplate] = None,
-                 ) -> None:
+    def __init__(
+        self,
+        checkpoint_dir: Union[Path, str],
+        chat_template: Optional[ChatTemplate] = None,
+    ) -> None:
         checkpoint_dir = Path(checkpoint_dir)
         self.checkpoint_dir = checkpoint_dir
         if not checkpoint_dir.exists():
             raise NotADirectoryError(f"The checkpoint directory does not exist: {str(checkpoint_dir)}")
 
         self.use_bos = self.check_if_bos_token_used(checkpoint_dir)
         self.bos_id = None
         self.eos_id = None
-        
+
         self.chat_template = chat_template if chat_template else ChatTemplate.from_checkpoint(checkpoint_dir)
 
         # some checkpoints have both files, `.model` takes precedence
         if (vocabulary_path := checkpoint_dir / "tokenizer.model").is_file():
             self.tokenizer_path = checkpoint_dir / "tokenizer.model"
             self.processor: SentencePieceProcessor = SentencePieceProcessor(model_file=str(vocabulary_path))
             self.backend = "sentencepiece"
@@ -107,38 +108,39 @@
                 raise NotImplementedError("This tokenizer does not have a defined a bos token")
             tokens = [bos_id] + tokens
         if eos:
             tokens = tokens + [self.eos_id]
         if max_length > 0:
             tokens = tokens[:max_length]
         return torch.tensor(tokens, dtype=torch.int, device=device)
-    
-    def encode_messages(self, 
-                        messages: List[Message], 
-                        add_generate_prompt: bool = True,
-                        device: Optional[torch.device] = None,
-                        bos: Optional[bool] = None,
-                        eos: bool = False,
-                        max_length: int = -1,
-                        ) -> torch.Tensor:
+
+    def encode_messages(
+        self,
+        messages: List[Message],
+        add_generate_prompt: bool = True,
+        device: Optional[torch.device] = None,
+        bos: Optional[bool] = None,
+        eos: bool = False,
+        max_length: int = -1,
+    ) -> torch.Tensor:
         assert self.chat_template, "Chat template is required for encoding messages"
         string = self.chat_template.apply_messages(messages, add_generate_prompt=add_generate_prompt)
         return self.encode(string, device, bos, eos, max_length)
 
     def decode(self, tensor: torch.Tensor) -> str:
         tokens = [tensor.item()] if tensor.ndim == 0 else tensor.tolist()
         return self.processor.decode(tokens)
-    
+
     def decode_stream(
         self,
         stream: Generator[torch.Tensor, None, None],
     ) -> Generator[str, None, None]:
         if self.backend == "huggingface":
             buffer = torch.tensor([], dtype=torch.long)
-            text = ''
+            text = ""
             try:
                 for token in stream:
                     buffer = buffer.to(device=token.device)
                     buffer = torch.cat((buffer, token.view(-1)))
                     t = self.decode(buffer)
                     if not self.has_special_chars(t):
                         yield t
@@ -156,39 +158,38 @@
                 for token in stream:
                     so_far = so_far.to(device=token.device)
                     so_far = torch.cat((so_far, token.view(-1)))
                     decoded_new = self.decode(so_far)
                     if self.has_special_chars(decoded_new):
                         # if the text contains special characters, it means that the tokenization is not complete
                         continue
-                    yield decoded_new[len(decoded_so_far):]
+                    yield decoded_new[len(decoded_so_far) :]
                     decoded_so_far = decoded_new
             except KeyboardInterrupt:
                 # support stopping generation
                 return decoded_so_far
         else:
             raise NotImplementedError(self.backend)
-    
+
     def save(self, save_dir: str):
         save_dir = Path(save_dir)
         if save_dir == self.checkpoint_dir:
             return
         import shutil
+
         if self.backend == "huggingface":
             shutil.copyfile(self.tokenizer_path, save_dir / self.tokenizer_path.name)
             shutil.copyfile(self.tokenizer_config_path, save_dir / self.tokenizer_config_path.name)
             shutil.copyfile(self.generation_config_path, save_dir / self.generation_config_path.name)
         if self.backend == "sentencepiece":
             shutil.copyfile(self.tokenizer_path, save_dir / self.tokenizer_path.name)
-            
+
     @property
     def stop_ids(self) -> List[List[int]]:
         stop_ids = [torch.tensor([self.eos_id], dtype=torch.int)]
         if self.chat_template:
             stop_ids.extend([self.encode(text) for text in self.chat_template.stop_texts])
         return stop_ids
-    
+
     def has_special_chars(self, text: str) -> bool:
-        """使用sentencepiece时，检查文本中是否包含特殊字符�.这种情况通常是由于一个中文字符被分割为几个token,而解码时没有合并回去导致的.
-        """
-        return '�' in text
-        
+        """使用sentencepiece时，检查文本中是否包含特殊字符�.这种情况通常是由于一个中文字符被分割为几个token,而解码时没有合并回去导致的."""
+        return "�" in text
```

### Comparing `osc_llm-0.1.4/osc_llm/utils.py` & `osc_llm-0.1.5/osc_llm/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,36 +3,37 @@
 from typing import Optional, Union, Dict, Tuple
 from wasabi import msg
 import statistics
 import torch
 import uuid
 
 
-
 def find_multiple(n: int, k: int) -> int:
     assert k > 0
     if n % k == 0:
         return n
     return n + k - (n % k)
-        
-        
+
+
 def get_chat_template(name) -> Optional[Config]:
     """在一个checkpoint的名称中获取chat模板"""
     for k, v in registry.chat_templates.get_all().items():
         if k in name:
             return v
     return None
 
 
-def build_model(config: Union[Dict, str, Path, Config], 
-                model_section: str = 'model',
-                quantizer_section: str = 'quantizer',
-                empty_init: bool = True,
-                quantize: bool = True,
-                return_config: bool = False) -> Union[torch.nn.Module, Tuple[torch.nn.Module, Config]]:
+def build_model(
+    config: Union[Dict, str, Path, Config],
+    model_section: str = "model",
+    quantizer_section: str = "quantizer",
+    empty_init: bool = True,
+    quantize: bool = True,
+    return_config: bool = False,
+) -> Union[torch.nn.Module, Tuple[torch.nn.Module, Config]]:
     """Build a model from a configuration.
 
     Args:
         config (Union[Dict, str, Path, Config]): the configuration to build the model from, can be a dictionary, a path to a file or a Config object.
         model_section (str, optional): the section to look for the model in the configuration. Defaults to 'model'.
         quantizer_section (str, optional): the section to look for the quantizer in the configuration. Defaults to 'quantizer'.
         empty_init (bool, optional): whether to initialize the model with empty weights. Defaults to True.
@@ -43,15 +44,15 @@
         torch.nn.Module: the model built from the configuration.
     """
     if isinstance(config, (str, Path)):
         config = Config().from_disk(config)
     if isinstance(config, dict):
         config = Config(data=config)
     if empty_init:
-        with torch.device('meta'):
+        with torch.device("meta"):
             resolved = registry.resolve(config=config)
     else:
         resolved = registry.resolve(config=config)
     if model_section not in resolved:
         msg.fail(f"cannot find model section {model_section}")
     else:
         model = resolved[model_section]
@@ -59,23 +60,25 @@
         quantizer = resolved[quantizer_section]
         model = quantizer.convert_for_runtime(model=model)
     if return_config:
         return model, config
     return model
 
 
-def build_from_checkpoint(checkpoint_dir: Union[str, Path], 
-                         model_section: str = 'model', 
-                         config_name: str = 'config.cfg', 
-                         model_name: str = 'osc_model.pth',
-                         empty_init: bool = True,
-                         quantize: bool = True,
-                         weights_only: bool = True,
-                         load_weights: bool = True,
-                         return_config: bool = False):
+def build_from_checkpoint(
+    checkpoint_dir: Union[str, Path],
+    model_section: str = "model",
+    config_name: str = "config.cfg",
+    model_name: str = "osc_model.pth",
+    empty_init: bool = True,
+    quantize: bool = True,
+    weights_only: bool = True,
+    load_weights: bool = True,
+    return_config: bool = False,
+):
     """build a model from a checkpoint directory.
 
     Args:
         checkpoint_dir (Union[str, Path]): the directory containing the model checkpoint.
         model_section (str, optional): the section to look for the model in the configuration. Defaults to 'model'.
         config_name (str, optional): the name of the configuration file. Defaults to 'config.cfg'.
         model_name (str, optional): the name of the model file. Defaults to 'osc_model.pth'.
@@ -87,27 +90,36 @@
 
     Returns:
         torch.nn.Module: the model loaded from the checkpoint.
     """
     checkpoint_dir = Path(checkpoint_dir)
     config_path = Path(checkpoint_dir) / config_name
     if return_config:
-        model, config = build_model(config_path, 
-                                    model_section=model_section,
-                                    quantize=quantize,
-                                    empty_init=empty_init,
-                                    return_config=return_config)
+        model, config = build_model(
+            config_path,
+            model_section=model_section,
+            quantize=quantize,
+            empty_init=empty_init,
+            return_config=return_config,
+        )
     else:
-        model = build_model(config_path, 
-                            model_section=model_section,
-                            quantize=quantize,
-                            empty_init=empty_init,
-                            return_config=return_config)
+        model = build_model(
+            config_path,
+            model_section=model_section,
+            quantize=quantize,
+            empty_init=empty_init,
+            return_config=return_config,
+        )
     if load_weights:
-        states = torch.load(str(checkpoint_dir / model_name), map_location='cpu', mmap=True, weights_only=weights_only)
+        states = torch.load(
+            str(checkpoint_dir / model_name),
+            map_location="cpu",
+            mmap=True,
+            weights_only=weights_only,
+        )
         model.load_state_dict(states)
     if return_config:
         return model, config
     return model
 
 
 @torch.no_grad()
@@ -125,15 +137,15 @@
     msg.info(f"Number of iterations: {num_iters}.")
     all_time = sum(times)
     msg.info(f"Total time: {all_time:.4f} s")
     mean_time = statistics.mean(times)
     msg.info(f"Mean time: {mean_time:.4f} s")
     median_time = statistics.median(times)
     msg.info(f"Median time: {median_time:.4f} s")
-    
+
 
 def get_default_supported_precision(training: bool) -> str:
     """Return default precision that is supported by the hardware: either `bf16` or `16`.
 
     Args:
         training: `-mixed` or `-true` version of the precision to use
 
@@ -146,14 +158,15 @@
         return "16-mixed" if training else "16-true"
     return "bf16-mixed" if training else "bf16-true"
 
 
 def random_uuid() -> str:
     return str(uuid.uuid4().hex)
 
+
 def get_model_size(model: torch.nn.Module, contains_embedding: bool = False) -> int:
     """Get the size of a model in bytes.
 
     Args:
         model (torch.nn.Module): the model to get the size of.
         contains_embedding (bool, optional): whether the model contains an embedding layer. Defaults to False.
 
@@ -163,8 +176,8 @@
     size = 0
     for param in model.parameters():
         size += param.numel() * param.element_size()
     if contains_embedding:
         for name, module in model.named_modules():
             if isinstance(module, torch.nn.Embedding):
                 size += module.num_embeddings * module.embedding_dim * module.weight.element_size()
-    return size
+    return size
```

### Comparing `osc_llm-0.1.4/PKG-INFO` & `osc_llm-0.1.5/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,61 +1,58 @@
 Metadata-Version: 2.1
 Name: osc-llm
-Version: 0.1.4
+Version: 0.1.5
 Summary: 大模型训练,评估,推理,部署工具
-License: MIT
-Author: wangmengdi
-Author-email: 790990241@qq.com
-Requires-Python: >=3.8
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: catalogue (>=2.0.10)
-Requires-Dist: confection (>=0.1.4)
-Requires-Dist: fastapi (>=0.110.2)
-Requires-Dist: jsonargparse (>=4.28.0)
-Requires-Dist: lightning (>=2.2.0)
-Requires-Dist: pydantic (>=1.10.8)
-Requires-Dist: sentencepiece (>=0.2.0)
-Requires-Dist: tokenizers (>=0.19.1)
-Requires-Dist: torch (>=2.3.0)
-Requires-Dist: uvicorn[standard] (>=0.29.0)
-Requires-Dist: wasabi (>=1.1.2)
+Author-email: wangmengdi <790990241@qq.com>
+Project-URL: homepage, https://github.com/di-osc/osc-llm
+Project-URL: documentation, https://wangmengdi.notion.site/OSC-LLM-5a04563d88464530b3d32b31e27c557a?pvs=74
 Description-Content-Type: text/markdown
+Requires-Dist: torch>=2.2.0
+Requires-Dist: lightning>=2.2.0
+Requires-Dist: jsonargparse>=4.28.0
+Requires-Dist: wasabi>=1.1.2
+Requires-Dist: confection>=0.1.4
+Requires-Dist: catalogue>=2.0.10
+Requires-Dist: sentencepiece>=0.2.0
+Requires-Dist: tokenizers>=0.19.1
+Requires-Dist: pydantic>=1.10.8
+Requires-Dist: fastapi>=0.110.2
+Requires-Dist: uvicorn[standard]>=0.29.0
 
 <div align='center'>
 
 # OSC-LLM
 <a href="https://pytorch.org/get-started/locally/"><img alt="PyTorch" src="https://img.shields.io/badge/PyTorch-ee4c2c?logo=pytorch&logoColor=white"></a>
 <a href="https://lightning.ai/docs/overview/getting-started"><img alt="Lightning" src="https://img.shields.io/badge/-Lightning-792ee5?logo=pytorchlightning&logoColor=white"></a>
 
 </div>
 
 ## 📌&nbsp;&nbsp; 简介
 
+osc-llm旨在成为一个简单易用的大模型训练、评估、推理、部署工具，支持主流的大模型。
+
+> 文档地址:
+- [notion](https://wangmengdi.notion.site/OSC-LLM-5a04563d88464530b3d32b31e27c557a)
+
 ## 📌&nbsp;&nbsp; 安装
 
 - 安装[最新版本pytorch](https://pytorch.org/get-started/locally/)
 - 安装osc-llm: `pip install osc-llm`
 
 ## 📌&nbsp;&nbsp; 快速开始
 ```bash
 # 下面以llama3为例演示如何转换为osc-llm格式,并进行聊天。
 # 假设你已经下载好huggingface的llama3模型在checkpoints/meta-llama目录下
-# 1. 转换模型
+# 1. 转换
 llm convert --checkpoint_dir checkpoints/meta-llama/Meta-Llama-3-8B-Instruct
-# 2. 量化模型
+# 2. 量化
 llm quantize int8 --checkpoint_dir checkpoints/meta-llama/Meta-Llama-3-8B-Instruct --save_dir checkpoints/meta-llama/Meta-Llama-3-8B-Instruct-int8
 # 3. 聊天(使用编译功能加速推理速度,需要等待几分钟编译时间)
 llm chat --checkpoint_dir checkpoints/meta-llama/Meta-Llama-3-8B-Instruct-int8 --compile true
-# 4. 部署简易版本openai服务
+# 4. 部署
 llm serve --checkpoint_dir checkpoints/meta-llama/Meta-Llama-3-8B-Instruct-int8
 ```
 
 ## 📌&nbsp;&nbsp; 模型支持
 
 以下huggingface中的模型结构(查看config.json)已经支持转换为osc-llm格式:
 - **LlamaForCausalLM**: llama2, llama3, chinese-alpaca2等。
```

#### html2text {}

```diff
@@ -1,35 +1,35 @@
-Metadata-Version: 2.1 Name: osc-llm Version: 0.1.4 Summary:
-å¤§æ¨¡åè®­ç»,è¯ä¼°,æ¨ç,é¨ç½²å·¥å· License: MIT Author: wangmengdi
-Author-email: 790990241@qq.com Requires-Python: >=3.8 Classifier: License ::
-OSI Approved :: MIT License Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
-Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
-Language :: Python :: 3.12 Requires-Dist: catalogue (>=2.0.10) Requires-Dist:
-confection (>=0.1.4) Requires-Dist: fastapi (>=0.110.2) Requires-Dist:
-jsonargparse (>=4.28.0) Requires-Dist: lightning (>=2.2.0) Requires-Dist:
-pydantic (>=1.10.8) Requires-Dist: sentencepiece (>=0.2.0) Requires-Dist:
-tokenizers (>=0.19.1) Requires-Dist: torch (>=2.3.0) Requires-Dist: uvicorn
-[standard] (>=0.29.0) Requires-Dist: wasabi (>=1.1.2) Description-Content-Type:
-text/markdown
+Metadata-Version: 2.1 Name: osc-llm Version: 0.1.5 Summary:
+å¤§æ¨¡åè®­ç»,è¯ä¼°,æ¨ç,é¨ç½²å·¥å· Author-email: wangmengdi
+<790990241@qq.com> Project-URL: homepage, https://github.com/di-osc/osc-llm
+Project-URL: documentation, https://wangmengdi.notion.site/OSC-LLM-
+5a04563d88464530b3d32b31e27c557a?pvs=74 Description-Content-Type: text/markdown
+Requires-Dist: torch>=2.2.0 Requires-Dist: lightning>=2.2.0 Requires-Dist:
+jsonargparse>=4.28.0 Requires-Dist: wasabi>=1.1.2 Requires-Dist:
+confection>=0.1.4 Requires-Dist: catalogue>=2.0.10 Requires-Dist:
+sentencepiece>=0.2.0 Requires-Dist: tokenizers>=0.19.1 Requires-Dist:
+pydantic>=1.10.8 Requires-Dist: fastapi>=0.110.2 Requires-Dist: uvicorn
+[standard]>=0.29.0
                          # OSC-LLM_[_P_y_T_o_r_c_h_]_[_L_i_g_h_t_n_i_n_g_]
-## ð   ç®ä» ## ð   å®è£ - å®è£[ææ°çæ¬pytorch](https://
-pytorch.org/get-started/locally/) - å®è£osc-llm: `pip install osc-llm` ##
-ð   å¿«éå¼å§ ```bash # ä¸é¢ä»¥llama3ä¸ºä¾æ¼ç¤ºå¦ä½è½¬æ¢ä¸ºosc-
-llmæ ¼å¼,å¹¶è¿è¡èå¤©ã #
+## ð   ç®ä» osc-
+llmæ¨å¨æä¸ºä¸ä¸ªç®åæç¨çå¤§æ¨¡åè®­ç»ãè¯ä¼°ãæ¨çãé¨ç½²å·¥å·ï¼æ¯æä¸»æµçå¤§æ¨¡åã
+> ææ¡£å°å: - [notion](https://wangmengdi.notion.site/OSC-LLM-
+5a04563d88464530b3d32b31e27c557a) ## ð   å®è£ - å®è£
+[ææ°çæ¬pytorch](https://pytorch.org/get-started/locally/) - å®è£osc-
+llm: `pip install osc-llm` ## ð   å¿«éå¼å§ ```bash #
+ä¸é¢ä»¥llama3ä¸ºä¾æ¼ç¤ºå¦ä½è½¬æ¢ä¸ºosc-llmæ ¼å¼,å¹¶è¿è¡èå¤©ã #
 åè®¾ä½ å·²ç»ä¸è½½å¥½huggingfaceçllama3æ¨¡åå¨checkpoints/meta-
-llamaç®å½ä¸ # 1. è½¬æ¢æ¨¡å llm convert --checkpoint_dir checkpoints/meta-
-llama/Meta-Llama-3-8B-Instruct # 2. éåæ¨¡å llm quantize int8 --
-checkpoint_dir checkpoints/meta-llama/Meta-Llama-3-8B-Instruct --save_dir
-checkpoints/meta-llama/Meta-Llama-3-8B-Instruct-int8 # 3. èå¤©
+llamaç®å½ä¸ # 1. è½¬æ¢ llm convert --checkpoint_dir checkpoints/meta-llama/
+Meta-Llama-3-8B-Instruct # 2. éå llm quantize int8 --checkpoint_dir
+checkpoints/meta-llama/Meta-Llama-3-8B-Instruct --save_dir checkpoints/meta-
+llama/Meta-Llama-3-8B-Instruct-int8 # 3. èå¤©
 (ä½¿ç¨ç¼è¯åè½å éæ¨çéåº¦,éè¦ç­å¾å åéç¼è¯æ¶é´) llm
 chat --checkpoint_dir checkpoints/meta-llama/Meta-Llama-3-8B-Instruct-int8 --
-compile true # 4. é¨ç½²ç®æçæ¬openaiæå¡ llm serve --checkpoint_dir
-checkpoints/meta-llama/Meta-Llama-3-8B-Instruct-int8 ``` ## ð   æ¨¡åæ¯æ
+compile true # 4. é¨ç½² llm serve --checkpoint_dir checkpoints/meta-llama/
+Meta-Llama-3-8B-Instruct-int8 ``` ## ð   æ¨¡åæ¯æ
 ä»¥ä¸huggingfaceä¸­çæ¨¡åç»æ(æ¥çconfig.json)å·²ç»æ¯æè½¬æ¢ä¸ºosc-
 llmæ ¼å¼: - **LlamaForCausalLM**: llama2, llama3, chinese-alpaca2ç­ã -
 **Qwen2ForCausalLM**: qwen1.5ç³»åã - **Qwen2MoeForCausalLM**: qwen2-
 moeç³»å(ç®åæ æ³å®æç¼è¯,æ¨çéåº¦å¾æ¢)ã ### è´æ¬
 æ¬é¡¹ç®åèäºå¤§éçå¼æºé¡¹ç®ï¼ç¹å«æ¯ä»¥ä¸é¡¹ç®ï¼ - [litgpt]
 (https://github.com/Lightning-AI/litgpt) - [gpt-fast](https://github.com/
 pytorch-labs/gpt-fast)
```

