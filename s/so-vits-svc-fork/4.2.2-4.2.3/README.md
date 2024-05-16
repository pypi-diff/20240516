# Comparing `tmp/so_vits_svc_fork-4.2.2.tar.gz` & `tmp/so_vits_svc_fork-4.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "so_vits_svc_fork-4.2.2.tar", max compression
+gzip compressed data, was "so_vits_svc_fork-4.2.3.tar", max compression
```

## Comparing `so_vits_svc_fork-4.2.2.tar` & `so_vits_svc_fork-4.2.3.tar`

### file list

```diff
@@ -1,52 +1,52 @@
--rw-r--r--   0        0        0    12463 2024-05-10 11:37:21.278830 so_vits_svc_fork-4.2.2/LICENSE
--rw-r--r--   0        0        0    33321 2024-05-10 11:37:21.278830 so_vits_svc_fork-4.2.2/README.md
--rw-r--r--   0        0        0     3171 2024-05-10 11:37:22.066843 so_vits_svc_fork-4.2.2/pyproject.toml
--rw-r--r--   0        0        0       70 2024-05-10 11:37:22.026842 so_vits_svc_fork-4.2.2/src/so_vits_svc_fork/__init__.py
--rw-r--r--   0        0        0    24947 2024-05-10 11:37:21.282830 so_vits_svc_fork-4.2.2/src/so_vits_svc_fork/__main__.py
--rw-r--r--   0        0        0     1393 2024-05-10 11:37:21.282830 so_vits_svc_fork-4.2.2/src/so_vits_svc_fork/cluster/__init__.py
--rw-r--r--   0        0        0     4914 2024-05-10 11:37:21.282830 so_vits_svc_fork-4.2.2/src/so_vits_svc_fork/cluster/train_cluster.py
--rw-r--r--   0        0        0     2875 2024-05-10 11:37:21.282830 so_vits_svc_fork-4.2.2/src/so_vits_svc_fork/dataset.py
--rw-r--r--   0        0        0     2599 2024-05-10 11:37:21.282830 so_vits_svc_fork-4.2.2/src/so_vits_svc_fork/default_gui_presets.json
--rw-r--r--   0        0        0     7267 2024-05-10 11:37:21.286830 so_vits_svc_fork-4.2.2/src/so_vits_svc_fork/f0.py
--rw-r--r--   0        0        0    30708 2024-05-10 11:37:21.286830 so_vits_svc_fork-4.2.2/src/so_vits_svc_fork/gui.py
--rw-r--r--   0        0        0      872 2024-05-10 11:37:21.286830 so_vits_svc_fork-4.2.2/src/so_vits_svc_fork/hparams.py
--rw-r--r--   0        0        0        0 2024-05-10 11:37:21.286830 so_vits_svc_fork-4.2.2/src/so_vits_svc_fork/inference/__init__.py
--rw-r--r--   0        0        0    24749 2024-05-10 11:37:21.286830 so_vits_svc_fork-4.2.2/src/so_vits_svc_fork/inference/core.py
--rw-r--r--   0        0        0     9418 2024-05-10 11:37:21.286830 so_vits_svc_fork-4.2.2/src/so_vits_svc_fork/inference/main.py
--rw-r--r--   0        0        0     1169 2024-05-10 11:37:21.286830 so_vits_svc_fork-4.2.2/src/so_vits_svc_fork/logger.py
--rw-r--r--   0        0        0        0 2024-05-10 11:37:21.286830 so_vits_svc_fork-4.2.2/src/so_vits_svc_fork/modules/__init__.py
--rw-r--r--   0        0        0    16683 2024-05-10 11:37:21.286830 so_vits_svc_fork-4.2.2/src/so_vits_svc_fork/modules/attentions.py
--rw-r--r--   0        0        0     4620 2024-05-10 11:37:21.286830 so_vits_svc_fork-4.2.2/src/so_vits_svc_fork/modules/commons.py
--rw-r--r--   0        0        0        0 2024-05-10 11:37:21.286830 so_vits_svc_fork-4.2.2/src/so_vits_svc_fork/modules/decoders/__init__.py
--rw-r--r--   0        0        0     1463 2024-05-10 11:37:21.286830 so_vits_svc_fork-4.2.2/src/so_vits_svc_fork/modules/decoders/f0.py
--rw-r--r--   0        0        0       76 2024-05-10 11:37:21.286830 so_vits_svc_fork-4.2.2/src/so_vits_svc_fork/modules/decoders/hifigan/__init__.py
--rw-r--r--   0        0        0    11618 2024-05-10 11:37:21.286830 so_vits_svc_fork-4.2.2/src/so_vits_svc_fork/modules/decoders/hifigan/_models.py
--rw-r--r--   0        0        0      340 2024-05-10 11:37:21.286830 so_vits_svc_fork-4.2.2/src/so_vits_svc_fork/modules/decoders/hifigan/_utils.py
--rw-r--r--   0        0        0      318 2024-05-10 11:37:21.286830 so_vits_svc_fork-4.2.2/src/so_vits_svc_fork/modules/decoders/mb_istft/__init__.py
--rw-r--r--   0        0        0    12477 2024-05-10 11:37:21.286830 so_vits_svc_fork-4.2.2/src/so_vits_svc_fork/modules/decoders/mb_istft/_generators.py
--rw-r--r--   0        0        0      419 2024-05-10 11:37:21.286830 so_vits_svc_fork-4.2.2/src/so_vits_svc_fork/modules/decoders/mb_istft/_loss.py
--rw-r--r--   0        0        0     4733 2024-05-10 11:37:21.286830 so_vits_svc_fork-4.2.2/src/so_vits_svc_fork/modules/decoders/mb_istft/_pqmf.py
--rw-r--r--   0        0        0     8954 2024-05-10 11:37:21.286830 so_vits_svc_fork-4.2.2/src/so_vits_svc_fork/modules/decoders/mb_istft/_stft.py
--rw-r--r--   0        0        0     4879 2024-05-10 11:37:21.286830 so_vits_svc_fork-4.2.2/src/so_vits_svc_fork/modules/decoders/mb_istft/_stft_loss.py
--rw-r--r--   0        0        0     5604 2024-05-10 11:37:21.286830 so_vits_svc_fork-4.2.2/src/so_vits_svc_fork/modules/descriminators.py
--rw-r--r--   0        0        0     4400 2024-05-10 11:37:21.286830 so_vits_svc_fork-4.2.2/src/so_vits_svc_fork/modules/encoders.py
--rw-r--r--   0        0        0     1390 2024-05-10 11:37:21.286830 so_vits_svc_fork-4.2.2/src/so_vits_svc_fork/modules/flows.py
--rw-r--r--   0        0        0     1405 2024-05-10 11:37:21.286830 so_vits_svc_fork-4.2.2/src/so_vits_svc_fork/modules/losses.py
--rw-r--r--   0        0        0     5753 2024-05-10 11:37:21.286830 so_vits_svc_fork-4.2.2/src/so_vits_svc_fork/modules/mel_processing.py
--rw-r--r--   0        0        0    14435 2024-05-10 11:37:21.286830 so_vits_svc_fork-4.2.2/src/so_vits_svc_fork/modules/modules.py
--rw-r--r--   0        0        0     8178 2024-05-10 11:37:21.286830 so_vits_svc_fork-4.2.2/src/so_vits_svc_fork/modules/synthesizers.py
--rw-r--r--   0        0        0        0 2024-05-10 11:37:21.286830 so_vits_svc_fork-4.2.2/src/so_vits_svc_fork/preprocessing/__init__.py
--rw-r--r--   0        0        0     2051 2024-05-10 11:37:21.286830 so_vits_svc_fork-4.2.2/src/so_vits_svc_fork/preprocessing/config_templates/quickvc.json
--rw-r--r--   0        0        0     1705 2024-05-10 11:37:21.286830 so_vits_svc_fork-4.2.2/src/so_vits_svc_fork/preprocessing/config_templates/so-vits-svc-4.0v1-legacy.json
--rw-r--r--   0        0        0     1862 2024-05-10 11:37:21.286830 so_vits_svc_fork-4.2.2/src/so_vits_svc_fork/preprocessing/config_templates/so-vits-svc-4.0v1.json
--rw-r--r--   0        0        0     2975 2024-05-10 11:37:21.286830 so_vits_svc_fork-4.2.2/src/so_vits_svc_fork/preprocessing/preprocess_classify.py
--rw-r--r--   0        0        0     2710 2024-05-10 11:37:21.286830 so_vits_svc_fork-4.2.2/src/so_vits_svc_fork/preprocessing/preprocess_flist_config.py
--rw-r--r--   0        0        0     4667 2024-05-10 11:37:21.286830 so_vits_svc_fork-4.2.2/src/so_vits_svc_fork/preprocessing/preprocess_hubert_f0.py
--rw-r--r--   0        0        0     4447 2024-05-10 11:37:21.286830 so_vits_svc_fork-4.2.2/src/so_vits_svc_fork/preprocessing/preprocess_resample.py
--rw-r--r--   0        0        0     3004 2024-05-10 11:37:21.286830 so_vits_svc_fork-4.2.2/src/so_vits_svc_fork/preprocessing/preprocess_speaker_diarization.py
--rw-r--r--   0        0        0     2206 2024-05-10 11:37:21.286830 so_vits_svc_fork-4.2.2/src/so_vits_svc_fork/preprocessing/preprocess_split.py
--rw-r--r--   0        0        0      126 2024-05-10 11:37:21.286830 so_vits_svc_fork-4.2.2/src/so_vits_svc_fork/preprocessing/preprocess_utils.py
--rw-r--r--   0        0        0        0 2024-05-10 11:37:21.286830 so_vits_svc_fork-4.2.2/src/so_vits_svc_fork/py.typed
--rw-r--r--   0        0        0    21359 2024-05-10 11:37:21.286830 so_vits_svc_fork-4.2.2/src/so_vits_svc_fork/train.py
--rw-r--r--   0        0        0    15617 2024-05-10 11:37:21.286830 so_vits_svc_fork-4.2.2/src/so_vits_svc_fork/utils.py
--rw-r--r--   0        0        0    35298 1970-01-01 00:00:00.000000 so_vits_svc_fork-4.2.2/PKG-INFO
+-rw-r--r--   0        0        0    12463 2024-05-10 16:11:33.590942 so_vits_svc_fork-4.2.3/LICENSE
+-rw-r--r--   0        0        0    33321 2024-05-10 16:11:33.590942 so_vits_svc_fork-4.2.3/README.md
+-rw-r--r--   0        0        0     3171 2024-05-10 16:11:34.478947 so_vits_svc_fork-4.2.3/pyproject.toml
+-rw-r--r--   0        0        0       70 2024-05-10 16:11:34.438947 so_vits_svc_fork-4.2.3/src/so_vits_svc_fork/__init__.py
+-rw-r--r--   0        0        0    24947 2024-05-10 16:11:33.598942 so_vits_svc_fork-4.2.3/src/so_vits_svc_fork/__main__.py
+-rw-r--r--   0        0        0     1393 2024-05-10 16:11:33.598942 so_vits_svc_fork-4.2.3/src/so_vits_svc_fork/cluster/__init__.py
+-rw-r--r--   0        0        0     4914 2024-05-10 16:11:33.598942 so_vits_svc_fork-4.2.3/src/so_vits_svc_fork/cluster/train_cluster.py
+-rw-r--r--   0        0        0     2875 2024-05-10 16:11:33.598942 so_vits_svc_fork-4.2.3/src/so_vits_svc_fork/dataset.py
+-rw-r--r--   0        0        0     2599 2024-05-10 16:11:33.598942 so_vits_svc_fork-4.2.3/src/so_vits_svc_fork/default_gui_presets.json
+-rw-r--r--   0        0        0     7267 2024-05-10 16:11:33.598942 so_vits_svc_fork-4.2.3/src/so_vits_svc_fork/f0.py
+-rw-r--r--   0        0        0    30708 2024-05-10 16:11:33.598942 so_vits_svc_fork-4.2.3/src/so_vits_svc_fork/gui.py
+-rw-r--r--   0        0        0      872 2024-05-10 16:11:33.598942 so_vits_svc_fork-4.2.3/src/so_vits_svc_fork/hparams.py
+-rw-r--r--   0        0        0        0 2024-05-10 16:11:33.598942 so_vits_svc_fork-4.2.3/src/so_vits_svc_fork/inference/__init__.py
+-rw-r--r--   0        0        0    24749 2024-05-10 16:11:33.598942 so_vits_svc_fork-4.2.3/src/so_vits_svc_fork/inference/core.py
+-rw-r--r--   0        0        0     9418 2024-05-10 16:11:33.598942 so_vits_svc_fork-4.2.3/src/so_vits_svc_fork/inference/main.py
+-rw-r--r--   0        0        0     1169 2024-05-10 16:11:33.598942 so_vits_svc_fork-4.2.3/src/so_vits_svc_fork/logger.py
+-rw-r--r--   0        0        0        0 2024-05-10 16:11:33.598942 so_vits_svc_fork-4.2.3/src/so_vits_svc_fork/modules/__init__.py
+-rw-r--r--   0        0        0    16683 2024-05-10 16:11:33.598942 so_vits_svc_fork-4.2.3/src/so_vits_svc_fork/modules/attentions.py
+-rw-r--r--   0        0        0     4620 2024-05-10 16:11:33.598942 so_vits_svc_fork-4.2.3/src/so_vits_svc_fork/modules/commons.py
+-rw-r--r--   0        0        0        0 2024-05-10 16:11:33.598942 so_vits_svc_fork-4.2.3/src/so_vits_svc_fork/modules/decoders/__init__.py
+-rw-r--r--   0        0        0     1463 2024-05-10 16:11:33.598942 so_vits_svc_fork-4.2.3/src/so_vits_svc_fork/modules/decoders/f0.py
+-rw-r--r--   0        0        0       76 2024-05-10 16:11:33.598942 so_vits_svc_fork-4.2.3/src/so_vits_svc_fork/modules/decoders/hifigan/__init__.py
+-rw-r--r--   0        0        0    11618 2024-05-10 16:11:33.598942 so_vits_svc_fork-4.2.3/src/so_vits_svc_fork/modules/decoders/hifigan/_models.py
+-rw-r--r--   0        0        0      340 2024-05-10 16:11:33.598942 so_vits_svc_fork-4.2.3/src/so_vits_svc_fork/modules/decoders/hifigan/_utils.py
+-rw-r--r--   0        0        0      318 2024-05-10 16:11:33.598942 so_vits_svc_fork-4.2.3/src/so_vits_svc_fork/modules/decoders/mb_istft/__init__.py
+-rw-r--r--   0        0        0    12477 2024-05-10 16:11:33.598942 so_vits_svc_fork-4.2.3/src/so_vits_svc_fork/modules/decoders/mb_istft/_generators.py
+-rw-r--r--   0        0        0      419 2024-05-10 16:11:33.598942 so_vits_svc_fork-4.2.3/src/so_vits_svc_fork/modules/decoders/mb_istft/_loss.py
+-rw-r--r--   0        0        0     4733 2024-05-10 16:11:33.598942 so_vits_svc_fork-4.2.3/src/so_vits_svc_fork/modules/decoders/mb_istft/_pqmf.py
+-rw-r--r--   0        0        0     8954 2024-05-10 16:11:33.598942 so_vits_svc_fork-4.2.3/src/so_vits_svc_fork/modules/decoders/mb_istft/_stft.py
+-rw-r--r--   0        0        0     4879 2024-05-10 16:11:33.598942 so_vits_svc_fork-4.2.3/src/so_vits_svc_fork/modules/decoders/mb_istft/_stft_loss.py
+-rw-r--r--   0        0        0     5604 2024-05-10 16:11:33.598942 so_vits_svc_fork-4.2.3/src/so_vits_svc_fork/modules/descriminators.py
+-rw-r--r--   0        0        0     4400 2024-05-10 16:11:33.598942 so_vits_svc_fork-4.2.3/src/so_vits_svc_fork/modules/encoders.py
+-rw-r--r--   0        0        0     1390 2024-05-10 16:11:33.598942 so_vits_svc_fork-4.2.3/src/so_vits_svc_fork/modules/flows.py
+-rw-r--r--   0        0        0     1405 2024-05-10 16:11:33.598942 so_vits_svc_fork-4.2.3/src/so_vits_svc_fork/modules/losses.py
+-rw-r--r--   0        0        0     5753 2024-05-10 16:11:33.598942 so_vits_svc_fork-4.2.3/src/so_vits_svc_fork/modules/mel_processing.py
+-rw-r--r--   0        0        0    14435 2024-05-10 16:11:33.598942 so_vits_svc_fork-4.2.3/src/so_vits_svc_fork/modules/modules.py
+-rw-r--r--   0        0        0     8178 2024-05-10 16:11:33.598942 so_vits_svc_fork-4.2.3/src/so_vits_svc_fork/modules/synthesizers.py
+-rw-r--r--   0        0        0        0 2024-05-10 16:11:33.598942 so_vits_svc_fork-4.2.3/src/so_vits_svc_fork/preprocessing/__init__.py
+-rw-r--r--   0        0        0     2051 2024-05-10 16:11:33.598942 so_vits_svc_fork-4.2.3/src/so_vits_svc_fork/preprocessing/config_templates/quickvc.json
+-rw-r--r--   0        0        0     1705 2024-05-10 16:11:33.598942 so_vits_svc_fork-4.2.3/src/so_vits_svc_fork/preprocessing/config_templates/so-vits-svc-4.0v1-legacy.json
+-rw-r--r--   0        0        0     1862 2024-05-10 16:11:33.598942 so_vits_svc_fork-4.2.3/src/so_vits_svc_fork/preprocessing/config_templates/so-vits-svc-4.0v1.json
+-rw-r--r--   0        0        0     2975 2024-05-10 16:11:33.598942 so_vits_svc_fork-4.2.3/src/so_vits_svc_fork/preprocessing/preprocess_classify.py
+-rw-r--r--   0        0        0     2710 2024-05-10 16:11:33.598942 so_vits_svc_fork-4.2.3/src/so_vits_svc_fork/preprocessing/preprocess_flist_config.py
+-rw-r--r--   0        0        0     4667 2024-05-10 16:11:33.598942 so_vits_svc_fork-4.2.3/src/so_vits_svc_fork/preprocessing/preprocess_hubert_f0.py
+-rw-r--r--   0        0        0     4447 2024-05-10 16:11:33.598942 so_vits_svc_fork-4.2.3/src/so_vits_svc_fork/preprocessing/preprocess_resample.py
+-rw-r--r--   0        0        0     3004 2024-05-10 16:11:33.598942 so_vits_svc_fork-4.2.3/src/so_vits_svc_fork/preprocessing/preprocess_speaker_diarization.py
+-rw-r--r--   0        0        0     2206 2024-05-10 16:11:33.598942 so_vits_svc_fork-4.2.3/src/so_vits_svc_fork/preprocessing/preprocess_split.py
+-rw-r--r--   0        0        0      126 2024-05-10 16:11:33.598942 so_vits_svc_fork-4.2.3/src/so_vits_svc_fork/preprocessing/preprocess_utils.py
+-rw-r--r--   0        0        0        0 2024-05-10 16:11:33.598942 so_vits_svc_fork-4.2.3/src/so_vits_svc_fork/py.typed
+-rw-r--r--   0        0        0    21359 2024-05-10 16:11:33.598942 so_vits_svc_fork-4.2.3/src/so_vits_svc_fork/train.py
+-rw-r--r--   0        0        0    15617 2024-05-10 16:11:33.598942 so_vits_svc_fork-4.2.3/src/so_vits_svc_fork/utils.py
+-rw-r--r--   0        0        0    35298 1970-01-01 00:00:00.000000 so_vits_svc_fork-4.2.3/PKG-INFO
```

### Comparing `so_vits_svc_fork-4.2.2/LICENSE` & `so_vits_svc_fork-4.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.2.2/README.md` & `so_vits_svc_fork-4.2.3/README.md`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.2.2/pyproject.toml` & `so_vits_svc_fork-4.2.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "so-vits-svc-fork"
-version = "4.2.2"
+version = "4.2.3"
 description = "A fork of so-vits-svc."
 authors = ["34j <34j.95a2p@simplelogin.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/34j/so-vits-svc-fork"
 documentation = "https://so-vits-svc-fork.readthedocs.io"
 classifiers = [
@@ -51,15 +51,15 @@
 tqdm-joblib = "^0.0.3"
 tensorboardx = "*"
 cm-time = ">=0.1.2"
 pysimplegui = ">=4.6,<5" # never update this, advertising popup window will be shown
 pebble = ">=5.0"
 torchcrepe = ">=0.0.17"
 lightning = "^2.0.1"
-fastapi = "==0.110.1"
+fastapi = "==0.111.0"
 transformers = "^4.28.1"
 matplotlib = "^3.7.1"
 click = "^8.1.7"
 setuptools = "^69.5.1"
 
 [tool.poetry.group.dev.dependencies]
 pre-commit = ">=3"
```

### Comparing `so_vits_svc_fork-4.2.2/src/so_vits_svc_fork/__main__.py` & `so_vits_svc_fork-4.2.3/src/so_vits_svc_fork/__main__.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.2.2/src/so_vits_svc_fork/cluster/__init__.py` & `so_vits_svc_fork-4.2.3/src/so_vits_svc_fork/cluster/__init__.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.2.2/src/so_vits_svc_fork/cluster/train_cluster.py` & `so_vits_svc_fork-4.2.3/src/so_vits_svc_fork/cluster/train_cluster.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.2.2/src/so_vits_svc_fork/dataset.py` & `so_vits_svc_fork-4.2.3/src/so_vits_svc_fork/dataset.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.2.2/src/so_vits_svc_fork/default_gui_presets.json` & `so_vits_svc_fork-4.2.3/src/so_vits_svc_fork/default_gui_presets.json`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.2.2/src/so_vits_svc_fork/f0.py` & `so_vits_svc_fork-4.2.3/src/so_vits_svc_fork/f0.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.2.2/src/so_vits_svc_fork/gui.py` & `so_vits_svc_fork-4.2.3/src/so_vits_svc_fork/gui.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.2.2/src/so_vits_svc_fork/hparams.py` & `so_vits_svc_fork-4.2.3/src/so_vits_svc_fork/hparams.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.2.2/src/so_vits_svc_fork/inference/core.py` & `so_vits_svc_fork-4.2.3/src/so_vits_svc_fork/inference/core.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.2.2/src/so_vits_svc_fork/inference/main.py` & `so_vits_svc_fork-4.2.3/src/so_vits_svc_fork/inference/main.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.2.2/src/so_vits_svc_fork/logger.py` & `so_vits_svc_fork-4.2.3/src/so_vits_svc_fork/logger.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.2.2/src/so_vits_svc_fork/modules/attentions.py` & `so_vits_svc_fork-4.2.3/src/so_vits_svc_fork/modules/attentions.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.2.2/src/so_vits_svc_fork/modules/commons.py` & `so_vits_svc_fork-4.2.3/src/so_vits_svc_fork/modules/commons.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.2.2/src/so_vits_svc_fork/modules/decoders/f0.py` & `so_vits_svc_fork-4.2.3/src/so_vits_svc_fork/modules/decoders/f0.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.2.2/src/so_vits_svc_fork/modules/decoders/hifigan/_models.py` & `so_vits_svc_fork-4.2.3/src/so_vits_svc_fork/modules/decoders/hifigan/_models.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.2.2/src/so_vits_svc_fork/modules/decoders/mb_istft/_generators.py` & `so_vits_svc_fork-4.2.3/src/so_vits_svc_fork/modules/decoders/mb_istft/_generators.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.2.2/src/so_vits_svc_fork/modules/decoders/mb_istft/_pqmf.py` & `so_vits_svc_fork-4.2.3/src/so_vits_svc_fork/modules/decoders/mb_istft/_pqmf.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.2.2/src/so_vits_svc_fork/modules/decoders/mb_istft/_stft.py` & `so_vits_svc_fork-4.2.3/src/so_vits_svc_fork/modules/decoders/mb_istft/_stft.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.2.2/src/so_vits_svc_fork/modules/decoders/mb_istft/_stft_loss.py` & `so_vits_svc_fork-4.2.3/src/so_vits_svc_fork/modules/decoders/mb_istft/_stft_loss.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.2.2/src/so_vits_svc_fork/modules/descriminators.py` & `so_vits_svc_fork-4.2.3/src/so_vits_svc_fork/modules/descriminators.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.2.2/src/so_vits_svc_fork/modules/encoders.py` & `so_vits_svc_fork-4.2.3/src/so_vits_svc_fork/modules/encoders.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.2.2/src/so_vits_svc_fork/modules/flows.py` & `so_vits_svc_fork-4.2.3/src/so_vits_svc_fork/modules/flows.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.2.2/src/so_vits_svc_fork/modules/losses.py` & `so_vits_svc_fork-4.2.3/src/so_vits_svc_fork/modules/losses.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.2.2/src/so_vits_svc_fork/modules/mel_processing.py` & `so_vits_svc_fork-4.2.3/src/so_vits_svc_fork/modules/mel_processing.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.2.2/src/so_vits_svc_fork/modules/modules.py` & `so_vits_svc_fork-4.2.3/src/so_vits_svc_fork/modules/modules.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.2.2/src/so_vits_svc_fork/modules/synthesizers.py` & `so_vits_svc_fork-4.2.3/src/so_vits_svc_fork/modules/synthesizers.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.2.2/src/so_vits_svc_fork/preprocessing/config_templates/quickvc.json` & `so_vits_svc_fork-4.2.3/src/so_vits_svc_fork/preprocessing/config_templates/quickvc.json`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.2.2/src/so_vits_svc_fork/preprocessing/config_templates/so-vits-svc-4.0v1-legacy.json` & `so_vits_svc_fork-4.2.3/src/so_vits_svc_fork/preprocessing/config_templates/so-vits-svc-4.0v1-legacy.json`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.2.2/src/so_vits_svc_fork/preprocessing/config_templates/so-vits-svc-4.0v1.json` & `so_vits_svc_fork-4.2.3/src/so_vits_svc_fork/preprocessing/config_templates/so-vits-svc-4.0v1.json`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.2.2/src/so_vits_svc_fork/preprocessing/preprocess_classify.py` & `so_vits_svc_fork-4.2.3/src/so_vits_svc_fork/preprocessing/preprocess_classify.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.2.2/src/so_vits_svc_fork/preprocessing/preprocess_flist_config.py` & `so_vits_svc_fork-4.2.3/src/so_vits_svc_fork/preprocessing/preprocess_flist_config.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.2.2/src/so_vits_svc_fork/preprocessing/preprocess_hubert_f0.py` & `so_vits_svc_fork-4.2.3/src/so_vits_svc_fork/preprocessing/preprocess_hubert_f0.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.2.2/src/so_vits_svc_fork/preprocessing/preprocess_resample.py` & `so_vits_svc_fork-4.2.3/src/so_vits_svc_fork/preprocessing/preprocess_resample.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.2.2/src/so_vits_svc_fork/preprocessing/preprocess_speaker_diarization.py` & `so_vits_svc_fork-4.2.3/src/so_vits_svc_fork/preprocessing/preprocess_speaker_diarization.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.2.2/src/so_vits_svc_fork/preprocessing/preprocess_split.py` & `so_vits_svc_fork-4.2.3/src/so_vits_svc_fork/preprocessing/preprocess_split.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.2.2/src/so_vits_svc_fork/train.py` & `so_vits_svc_fork-4.2.3/src/so_vits_svc_fork/train.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.2.2/src/so_vits_svc_fork/utils.py` & `so_vits_svc_fork-4.2.3/src/so_vits_svc_fork/utils.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.2.2/PKG-INFO` & `so_vits_svc_fork-4.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: so-vits-svc-fork
-Version: 4.2.2
+Version: 4.2.3
 Summary: A fork of so-vits-svc.
 Home-page: https://github.com/34j/so-vits-svc-fork
 License: MIT
 Author: 34j
 Author-email: 34j.95a2p@simplelogin.com
 Requires-Python: >=3.9,<3.13
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -17,15 +17,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries
 Requires-Dist: SoundFile
 Requires-Dist: click (>=8.1.7,<9.0.0)
 Requires-Dist: cm-time (>=0.1.2)
-Requires-Dist: fastapi (==0.110.1)
+Requires-Dist: fastapi (==0.111.0)
 Requires-Dist: librosa
 Requires-Dist: lightning (>=2.0.1,<3.0.0)
 Requires-Dist: matplotlib (>=3.7.1,<4.0.0)
 Requires-Dist: numpy (>=1.26.4,<2.0.0)
 Requires-Dist: onnx
 Requires-Dist: onnxoptimizer
 Requires-Dist: onnxsim
```

#### html2text {}

```diff
@@ -1,20 +1,20 @@
-Metadata-Version: 2.1 Name: so-vits-svc-fork Version: 4.2.2 Summary: A fork of
+Metadata-Version: 2.1 Name: so-vits-svc-fork Version: 4.2.3 Summary: A fork of
 so-vits-svc. Home-page: https://github.com/34j/so-vits-svc-fork License: MIT
 Author: 34j Author-email: 34j.95a2p@simplelogin.com Requires-Python:
 >=3.9,<3.13 Classifier: Development Status :: 2 - Pre-Alpha Classifier:
 Intended Audience :: Developers Classifier: License :: OSI Approved :: MIT
 License Classifier: Natural Language :: English Classifier: Operating System ::
 OS Independent Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
 Programming Language :: Python :: 3.12 Classifier: Topic :: Software
 Development :: Libraries Requires-Dist: SoundFile Requires-Dist: click
 (>=8.1.7,<9.0.0) Requires-Dist: cm-time (>=0.1.2) Requires-Dist: fastapi
-(==0.110.1) Requires-Dist: librosa Requires-Dist: lightning (>=2.0.1,<3.0.0)
+(==0.111.0) Requires-Dist: librosa Requires-Dist: lightning (>=2.0.1,<3.0.0)
 Requires-Dist: matplotlib (>=3.7.1,<4.0.0) Requires-Dist: numpy
 (>=1.26.4,<2.0.0) Requires-Dist: onnx Requires-Dist: onnxoptimizer Requires-
 Dist: onnxsim Requires-Dist: pebble (>=5.0) Requires-Dist: praat-parselmouth
 Requires-Dist: pysimplegui (>=4.6,<5) Requires-Dist: pyworld Requires-Dist:
 requests Requires-Dist: rich Requires-Dist: scipy Requires-Dist: setuptools
 (>=69.5.1,<70.0.0) Requires-Dist: sounddevice Requires-Dist: tensorboard
 Requires-Dist: tensorboardx Requires-Dist: torch (>=2,<3) Requires-Dist:
```

