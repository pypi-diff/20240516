# Comparing `tmp/torch_log_wmse_audio_quality-0.1.0.tar.gz` & `tmp/torch_log_wmse_audio_quality-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torch_log_wmse_audio_quality-0.1.0.tar", last modified: Wed May 15 22:11:42 2024, max compression
+gzip compressed data, was "torch_log_wmse_audio_quality-0.1.1.tar", last modified: Thu May 16 01:03:56 2024, max compression
```

## Comparing `torch_log_wmse_audio_quality-0.1.0.tar` & `torch_log_wmse_audio_quality-0.1.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 chris      (501) staff       (20)        0 2024-05-15 22:11:42.473780 torch_log_wmse_audio_quality-0.1.0/
--rw-r--r--   0 chris      (501) staff       (20)    11370 2024-05-15 20:08:40.000000 torch_log_wmse_audio_quality-0.1.0/LICENSE
--rw-r--r--   0 chris      (501) staff       (20)     3550 2024-05-15 22:11:42.473700 torch_log_wmse_audio_quality-0.1.0/PKG-INFO
--rw-r--r--   0 chris      (501) staff       (20)     2721 2024-05-15 22:08:01.000000 torch_log_wmse_audio_quality-0.1.0/README.md
--rw-r--r--   0 chris      (501) staff       (20)      103 2024-05-15 21:20:06.000000 torch_log_wmse_audio_quality-0.1.0/pyproject.toml
--rw-r--r--   0 chris      (501) staff       (20)     1006 2024-05-15 22:11:42.474061 torch_log_wmse_audio_quality-0.1.0/setup.cfg
-drwxr-xr-x   0 chris      (501) staff       (20)        0 2024-05-15 22:11:42.470089 torch_log_wmse_audio_quality-0.1.0/tests/
--rw-r--r--   0 chris      (501) staff       (20)     4165 2024-05-15 21:48:36.000000 torch_log_wmse_audio_quality-0.1.0/tests/test_metric.py
-drwxr-xr-x   0 chris      (501) staff       (20)        0 2024-05-15 22:11:42.472530 torch_log_wmse_audio_quality-0.1.0/torch_log_wmse_audio_quality/
--rw-r--r--   0 chris      (501) staff       (20)       51 2024-05-15 20:27:31.000000 torch_log_wmse_audio_quality-0.1.0/torch_log_wmse_audio_quality/__init__.py
--rw-r--r--   0 chris      (501) staff       (20)      599 2024-03-29 20:25:42.000000 torch_log_wmse_audio_quality-0.1.0/torch_log_wmse_audio_quality/constants.py
--rw-r--r--   0 chris      (501) staff       (20)    32151 2024-03-28 21:53:42.000000 torch_log_wmse_audio_quality-0.1.0/torch_log_wmse_audio_quality/filter_ir.pkl
--rw-r--r--   0 chris      (501) staff       (20)     5980 2024-05-15 19:18:50.000000 torch_log_wmse_audio_quality-0.1.0/torch_log_wmse_audio_quality/freq_weighting_filter.py
--rw-r--r--   0 chris      (501) staff       (20)     5348 2024-05-15 19:52:25.000000 torch_log_wmse_audio_quality-0.1.0/torch_log_wmse_audio_quality/metric.py
--rw-r--r--   0 chris      (501) staff       (20)      947 2024-05-15 18:39:32.000000 torch_log_wmse_audio_quality-0.1.0/torch_log_wmse_audio_quality/utils.py
-drwxr-xr-x   0 chris      (501) staff       (20)        0 2024-05-15 22:11:42.473469 torch_log_wmse_audio_quality-0.1.0/torch_log_wmse_audio_quality.egg-info/
--rw-r--r--   0 chris      (501) staff       (20)     3550 2024-05-15 22:11:42.000000 torch_log_wmse_audio_quality-0.1.0/torch_log_wmse_audio_quality.egg-info/PKG-INFO
--rw-r--r--   0 chris      (501) staff       (20)      579 2024-05-15 22:11:42.000000 torch_log_wmse_audio_quality-0.1.0/torch_log_wmse_audio_quality.egg-info/SOURCES.txt
--rw-r--r--   0 chris      (501) staff       (20)        1 2024-05-15 22:11:42.000000 torch_log_wmse_audio_quality-0.1.0/torch_log_wmse_audio_quality.egg-info/dependency_links.txt
--rw-r--r--   0 chris      (501) staff       (20)       45 2024-05-15 22:11:42.000000 torch_log_wmse_audio_quality-0.1.0/torch_log_wmse_audio_quality.egg-info/requires.txt
--rw-r--r--   0 chris      (501) staff       (20)       29 2024-05-15 22:11:42.000000 torch_log_wmse_audio_quality-0.1.0/torch_log_wmse_audio_quality.egg-info/top_level.txt
+drwxr-xr-x   0 chris      (501) staff       (20)        0 2024-05-16 01:03:56.811643 torch_log_wmse_audio_quality-0.1.1/
+-rw-r--r--   0 chris      (501) staff       (20)    11370 2024-05-15 20:08:40.000000 torch_log_wmse_audio_quality-0.1.1/LICENSE
+-rw-r--r--   0 chris      (501) staff       (20)     4296 2024-05-16 01:03:56.811578 torch_log_wmse_audio_quality-0.1.1/PKG-INFO
+-rw-r--r--   0 chris      (501) staff       (20)     3467 2024-05-15 22:43:18.000000 torch_log_wmse_audio_quality-0.1.1/README.md
+-rw-r--r--   0 chris      (501) staff       (20)      103 2024-05-15 21:20:06.000000 torch_log_wmse_audio_quality-0.1.1/pyproject.toml
+-rw-r--r--   0 chris      (501) staff       (20)     1006 2024-05-16 01:03:56.811931 torch_log_wmse_audio_quality-0.1.1/setup.cfg
+drwxr-xr-x   0 chris      (501) staff       (20)        0 2024-05-16 01:03:56.805201 torch_log_wmse_audio_quality-0.1.1/tests/
+-rw-r--r--   0 chris      (501) staff       (20)     4165 2024-05-15 21:48:36.000000 torch_log_wmse_audio_quality-0.1.1/tests/test_metric.py
+drwxr-xr-x   0 chris      (501) staff       (20)        0 2024-05-16 01:03:56.810216 torch_log_wmse_audio_quality-0.1.1/torch_log_wmse_audio_quality/
+-rw-r--r--   0 chris      (501) staff       (20)       51 2024-05-15 20:27:31.000000 torch_log_wmse_audio_quality-0.1.1/torch_log_wmse_audio_quality/__init__.py
+-rw-r--r--   0 chris      (501) staff       (20)      599 2024-03-29 20:25:42.000000 torch_log_wmse_audio_quality-0.1.1/torch_log_wmse_audio_quality/constants.py
+-rw-r--r--   0 chris      (501) staff       (20)    32151 2024-03-28 21:53:42.000000 torch_log_wmse_audio_quality-0.1.1/torch_log_wmse_audio_quality/filter_ir.pkl
+-rw-r--r--   0 chris      (501) staff       (20)     5747 2024-05-16 01:00:43.000000 torch_log_wmse_audio_quality-0.1.1/torch_log_wmse_audio_quality/freq_weighting_filter.py
+-rw-r--r--   0 chris      (501) staff       (20)     5348 2024-05-15 19:52:25.000000 torch_log_wmse_audio_quality-0.1.1/torch_log_wmse_audio_quality/metric.py
+-rw-r--r--   0 chris      (501) staff       (20)      947 2024-05-15 18:39:32.000000 torch_log_wmse_audio_quality-0.1.1/torch_log_wmse_audio_quality/utils.py
+drwxr-xr-x   0 chris      (501) staff       (20)        0 2024-05-16 01:03:56.811271 torch_log_wmse_audio_quality-0.1.1/torch_log_wmse_audio_quality.egg-info/
+-rw-r--r--   0 chris      (501) staff       (20)     4296 2024-05-16 01:03:56.000000 torch_log_wmse_audio_quality-0.1.1/torch_log_wmse_audio_quality.egg-info/PKG-INFO
+-rw-r--r--   0 chris      (501) staff       (20)      579 2024-05-16 01:03:56.000000 torch_log_wmse_audio_quality-0.1.1/torch_log_wmse_audio_quality.egg-info/SOURCES.txt
+-rw-r--r--   0 chris      (501) staff       (20)        1 2024-05-16 01:03:56.000000 torch_log_wmse_audio_quality-0.1.1/torch_log_wmse_audio_quality.egg-info/dependency_links.txt
+-rw-r--r--   0 chris      (501) staff       (20)       45 2024-05-16 01:03:56.000000 torch_log_wmse_audio_quality-0.1.1/torch_log_wmse_audio_quality.egg-info/requires.txt
+-rw-r--r--   0 chris      (501) staff       (20)       29 2024-05-16 01:03:56.000000 torch_log_wmse_audio_quality-0.1.1/torch_log_wmse_audio_quality.egg-info/top_level.txt
```

### Comparing `torch_log_wmse_audio_quality-0.1.0/LICENSE` & `torch_log_wmse_audio_quality-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `torch_log_wmse_audio_quality-0.1.0/PKG-INFO` & `torch_log_wmse_audio_quality-0.1.1/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,66 +1,46 @@
-Metadata-Version: 2.1
-Name: torch-log-wmse-audio-quality
-Version: 0.1.0
-Summary: logWMSE is an audio quality metric & loss function with support for digital silence target. Useful for training and evaluating audio source separation systems.
-Home-page: https://github.com/crlandsc/torch-log-wmse-audio-quality
-Author: Christopher Landschoot
-Author-email: crlandschoot@gmail.com
-License: Apache License 2.0
-Project-URL: Bug Tracker, https://github.com/crlandsc/torch-log-wmse-audio-quality/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: torch>=1.8.0
-Requires-Dist: torchaudio>=1.8.0
-Requires-Dist: numpy>=1.23.5
-
 # torch-log-wmse-audio-quality
 
-This repository contains the torch implementation of an audio quality metric, [logWMSE](https://github.com/nomonosound/log-wmse-audio-quality), originally suggested by [Iver Jordal](https://github.com/iver56) of [Nomono](https://nomono.co/). In addition to the original metric, this implementation can also be used as a loss function for training audio models.
+[![LICENSE](https://img.shields.io/github/license/crlandsc/torch-log-wmse-audio-quality)](https://github.com/crlandsc/torch-log-wmse-audio-quality/blob/main/LICENSE) [![GitHub Repo stars](https://img.shields.io/github/stars/crlandsc/torch-log-wmse-audio-quality)](https://github.com/crlandsc/torch-log-wmse-audio-quality/stargazers) [![GitHub forks](https://img.shields.io/github/forks/crlandsc/torch-log-wmse-audio-quality)](https://github.com/crlandsc/torch-log-wmse-audio-quality/forks)
+
+This repository contains the torch implementation of an audio quality metric, [logWMSE](https://github.com/nomonosound/log-wmse-audio-quality), originally proposed by [Iver Jordal](https://github.com/iver56) of [Nomono](https://nomono.co/). In addition to the original metric, this implementation can also be used as a loss function for training audio models.
 
 logWMSE is a custom metric and loss function for audio signals that calculates the logarithm (log)
 of a frequency-weighted (W) Mean Squared Error (MSE). It is designed to address several shortcomings of common audio metrics, most importantly the lack of support for digital silence targets.
 
 ## Installation
 
-To use this repository, clone it and install the required dependencies:
+[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/torch-log-wmse-audio-quality)](https://pypi.org/project/torch-log-wmse-audio-quality/) [![PyPI - Version](https://img.shields.io/pypi/v/torch-log-wmse-audio-quality)](https://pypi.org/project/torch-log-wmse-audio-quality/) [![Number of downloads from PyPI per month](https://img.shields.io/pypi/dm/torch-log-wmse-audio-quality)](https://pypi.org/project/torch-log-wmse-audio-quality/)
 
-```bash
-git clone https://github.com/your-username/torch-log-wmse-audio-quality.git
-cd torch-log-wmse-audio-quality
-pip install -r requirements.txt
-```
+
+`pip install torch-log-wmse-audio-quality`
 
 ## Usage Example
 
 ```python
 import torch
 from torch_log_wmse_audio_quality import LogWMSE
 
 # Tensor shapes
 audio_length = 1.0
 sample_rate = 44100
 audio_channels = 2 # stereo
 audio_stems = 3 # 3 audio stems
 batch = 4 # batch size
 
-# Instantiate logWMSELoss
-log_wmse_loss = LogWMSE(audio_length=audio_length, sample_rate=sample_rate, return_as_loss=True)
+# Instantiate logWMSE
+log_wmse = LogWMSE(audio_length=audio_length, sample_rate=sample_rate, return_as_loss=True)
 
 # Generate random inputs (scale between -1 and 1)
 audio_lengths_samples = int(audio_length * sample_rate)
 unprocessed_audio = 2 * torch.rand(batch, audio_channels, audio_lengths_samples) - 1
 processed_audio = unprocessed_audio.unsqueeze(2).expand(-1, -1, audio_stems, -1) * 0.1
 target_audio = torch.zeros(batch, audio_channels, audio_stems, audio_lengths_samples)
 
-log_wmse = log_wmse_loss(unprocessed_audio, processed_audio, target_audio)
+log_wmse = log_wmse(unprocessed_audio, processed_audio, target_audio)
 print(log_wmse)  # Expected output: approx. -18.42
 ```
 
 ## Motivation
 * Supports digital silence targets not supported by other audio metrics.
     i.e. (SI-)SDR, SIR, SAR, ISR, VISQOL_audio, STOI, CDPAM, and VISQOL.
 * Overcomes the small value range issue of MSE (i.e. between 1e-8 and 1e-3), making number
```

### Comparing `torch_log_wmse_audio_quality-0.1.0/setup.cfg` & `torch_log_wmse_audio_quality-0.1.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = torch-log-wmse-audio-quality
-version = 0.1.0
+version = 0.1.1
 author = Christopher Landschoot
 author_email = crlandschoot@gmail.com
 license = Apache License 2.0
 description = logWMSE is an audio quality metric & loss function with support for digital silence target. Useful for training and evaluating audio source separation systems.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/crlandsc/torch-log-wmse-audio-quality
```

### Comparing `torch_log_wmse_audio_quality-0.1.0/tests/test_metric.py` & `torch_log_wmse_audio_quality-0.1.1/tests/test_metric.py`

 * *Files identical despite different names*

### Comparing `torch_log_wmse_audio_quality-0.1.0/torch_log_wmse_audio_quality/constants.py` & `torch_log_wmse_audio_quality-0.1.1/torch_log_wmse_audio_quality/constants.py`

 * *Files identical despite different names*

### Comparing `torch_log_wmse_audio_quality-0.1.0/torch_log_wmse_audio_quality/filter_ir.pkl` & `torch_log_wmse_audio_quality-0.1.1/torch_log_wmse_audio_quality/filter_ir.pkl`

 * *Files identical despite different names*

### Comparing `torch_log_wmse_audio_quality-0.1.0/torch_log_wmse_audio_quality/freq_weighting_filter.py` & `torch_log_wmse_audio_quality-0.1.1/torch_log_wmse_audio_quality/freq_weighting_filter.py`

 * *Files 4% similar despite different names*

```diff
@@ -71,18 +71,14 @@
     """
     def __init__(self, audio_length: int = 1, sample_rate: int = 44100, impulse_response: Tensor = None, impulse_response_sample_rate: int = 44100):
         # Load the impulse response if not provided
         if impulse_response is None:
             with resources.open_binary("torch_log_wmse_audio_quality", "filter_ir.pkl") as f:
                 impulse_response = torch.tensor(pickle.load(f), dtype=torch.float32)
 
-        # Move impulse response to available cude if available - also dynamically set during fft_convolve
-        device = 'cuda' if torch.cuda.is_available() else 'cpu'
-        impulse_response = impulse_response.to(device=device)
-
         # Resample the impulse response if necessary
         if impulse_response_sample_rate != sample_rate:
             self.resampler = Resample(orig_freq=impulse_response_sample_rate, new_freq=sample_rate)
             impulse_response = self.resampler(impulse_response)
 
         # Remove any singleton dimensions
         self.impulse_response = impulse_response.squeeze()
```

### Comparing `torch_log_wmse_audio_quality-0.1.0/torch_log_wmse_audio_quality/metric.py` & `torch_log_wmse_audio_quality-0.1.1/torch_log_wmse_audio_quality/metric.py`

 * *Files identical despite different names*

### Comparing `torch_log_wmse_audio_quality-0.1.0/torch_log_wmse_audio_quality/utils.py` & `torch_log_wmse_audio_quality-0.1.1/torch_log_wmse_audio_quality/utils.py`

 * *Files identical despite different names*

### Comparing `torch_log_wmse_audio_quality-0.1.0/torch_log_wmse_audio_quality.egg-info/PKG-INFO` & `torch_log_wmse_audio_quality-0.1.1/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torch-log-wmse-audio-quality
-Version: 0.1.0
+Version: 0.1.1
 Summary: logWMSE is an audio quality metric & loss function with support for digital silence target. Useful for training and evaluating audio source separation systems.
 Home-page: https://github.com/crlandsc/torch-log-wmse-audio-quality
 Author: Christopher Landschoot
 Author-email: crlandschoot@gmail.com
 License: Apache License 2.0
 Project-URL: Bug Tracker, https://github.com/crlandsc/torch-log-wmse-audio-quality/issues
 Classifier: Programming Language :: Python :: 3
@@ -15,52 +15,51 @@
 License-File: LICENSE
 Requires-Dist: torch>=1.8.0
 Requires-Dist: torchaudio>=1.8.0
 Requires-Dist: numpy>=1.23.5
 
 # torch-log-wmse-audio-quality
 
-This repository contains the torch implementation of an audio quality metric, [logWMSE](https://github.com/nomonosound/log-wmse-audio-quality), originally suggested by [Iver Jordal](https://github.com/iver56) of [Nomono](https://nomono.co/). In addition to the original metric, this implementation can also be used as a loss function for training audio models.
+[![LICENSE](https://img.shields.io/github/license/crlandsc/torch-log-wmse-audio-quality)](https://github.com/crlandsc/torch-log-wmse-audio-quality/blob/main/LICENSE) [![GitHub Repo stars](https://img.shields.io/github/stars/crlandsc/torch-log-wmse-audio-quality)](https://github.com/crlandsc/torch-log-wmse-audio-quality/stargazers) [![GitHub forks](https://img.shields.io/github/forks/crlandsc/torch-log-wmse-audio-quality)](https://github.com/crlandsc/torch-log-wmse-audio-quality/forks)
+
+This repository contains the torch implementation of an audio quality metric, [logWMSE](https://github.com/nomonosound/log-wmse-audio-quality), originally proposed by [Iver Jordal](https://github.com/iver56) of [Nomono](https://nomono.co/). In addition to the original metric, this implementation can also be used as a loss function for training audio models.
 
 logWMSE is a custom metric and loss function for audio signals that calculates the logarithm (log)
 of a frequency-weighted (W) Mean Squared Error (MSE). It is designed to address several shortcomings of common audio metrics, most importantly the lack of support for digital silence targets.
 
 ## Installation
 
-To use this repository, clone it and install the required dependencies:
+[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/torch-log-wmse-audio-quality)](https://pypi.org/project/torch-log-wmse-audio-quality/) [![PyPI - Version](https://img.shields.io/pypi/v/torch-log-wmse-audio-quality)](https://pypi.org/project/torch-log-wmse-audio-quality/) [![Number of downloads from PyPI per month](https://img.shields.io/pypi/dm/torch-log-wmse-audio-quality)](https://pypi.org/project/torch-log-wmse-audio-quality/)
 
-```bash
-git clone https://github.com/your-username/torch-log-wmse-audio-quality.git
-cd torch-log-wmse-audio-quality
-pip install -r requirements.txt
-```
+
+`pip install torch-log-wmse-audio-quality`
 
 ## Usage Example
 
 ```python
 import torch
 from torch_log_wmse_audio_quality import LogWMSE
 
 # Tensor shapes
 audio_length = 1.0
 sample_rate = 44100
 audio_channels = 2 # stereo
 audio_stems = 3 # 3 audio stems
 batch = 4 # batch size
 
-# Instantiate logWMSELoss
-log_wmse_loss = LogWMSE(audio_length=audio_length, sample_rate=sample_rate, return_as_loss=True)
+# Instantiate logWMSE
+log_wmse = LogWMSE(audio_length=audio_length, sample_rate=sample_rate, return_as_loss=True)
 
 # Generate random inputs (scale between -1 and 1)
 audio_lengths_samples = int(audio_length * sample_rate)
 unprocessed_audio = 2 * torch.rand(batch, audio_channels, audio_lengths_samples) - 1
 processed_audio = unprocessed_audio.unsqueeze(2).expand(-1, -1, audio_stems, -1) * 0.1
 target_audio = torch.zeros(batch, audio_channels, audio_stems, audio_lengths_samples)
 
-log_wmse = log_wmse_loss(unprocessed_audio, processed_audio, target_audio)
+log_wmse = log_wmse(unprocessed_audio, processed_audio, target_audio)
 print(log_wmse)  # Expected output: approx. -18.42
 ```
 
 ## Motivation
 * Supports digital silence targets not supported by other audio metrics.
     i.e. (SI-)SDR, SIR, SAR, ISR, VISQOL_audio, STOI, CDPAM, and VISQOL.
 * Overcomes the small value range issue of MSE (i.e. between 1e-8 and 1e-3), making number
```

### Comparing `torch_log_wmse_audio_quality-0.1.0/torch_log_wmse_audio_quality.egg-info/SOURCES.txt` & `torch_log_wmse_audio_quality-0.1.1/torch_log_wmse_audio_quality.egg-info/SOURCES.txt`

 * *Files identical despite different names*

