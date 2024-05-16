# Comparing `tmp/torch_log_wmse_audio_quality-0.1.2.tar.gz` & `tmp/torch_log_wmse_audio_quality-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torch_log_wmse_audio_quality-0.1.2.tar", last modified: Thu May 16 17:48:13 2024, max compression
+gzip compressed data, was "torch_log_wmse_audio_quality-0.1.3.tar", last modified: Thu May 16 17:58:28 2024, max compression
```

## Comparing `torch_log_wmse_audio_quality-0.1.2.tar` & `torch_log_wmse_audio_quality-0.1.3.tar`

### file list

```diff
@@ -1,21 +1,23 @@
-drwxr-xr-x   0 chris      (501) staff       (20)        0 2024-05-16 17:48:13.217533 torch_log_wmse_audio_quality-0.1.2/
--rw-r--r--   0 chris      (501) staff       (20)    11370 2024-05-15 20:08:40.000000 torch_log_wmse_audio_quality-0.1.2/LICENSE
--rw-r--r--   0 chris      (501) staff       (20)     7396 2024-05-16 17:48:13.217454 torch_log_wmse_audio_quality-0.1.2/PKG-INFO
--rw-r--r--   0 chris      (501) staff       (20)     6567 2024-05-16 17:47:05.000000 torch_log_wmse_audio_quality-0.1.2/README.md
--rw-r--r--   0 chris      (501) staff       (20)      103 2024-05-15 21:20:06.000000 torch_log_wmse_audio_quality-0.1.2/pyproject.toml
--rw-r--r--   0 chris      (501) staff       (20)     1006 2024-05-16 17:48:13.217825 torch_log_wmse_audio_quality-0.1.2/setup.cfg
-drwxr-xr-x   0 chris      (501) staff       (20)        0 2024-05-16 17:48:13.213631 torch_log_wmse_audio_quality-0.1.2/tests/
--rw-r--r--   0 chris      (501) staff       (20)     4159 2024-05-16 17:08:03.000000 torch_log_wmse_audio_quality-0.1.2/tests/test_metric.py
-drwxr-xr-x   0 chris      (501) staff       (20)        0 2024-05-16 17:48:13.215646 torch_log_wmse_audio_quality-0.1.2/torch_log_wmse_audio_quality/
--rw-r--r--   0 chris      (501) staff       (20)       51 2024-05-15 20:27:31.000000 torch_log_wmse_audio_quality-0.1.2/torch_log_wmse_audio_quality/__init__.py
--rw-r--r--   0 chris      (501) staff       (20)      599 2024-03-29 20:25:42.000000 torch_log_wmse_audio_quality-0.1.2/torch_log_wmse_audio_quality/constants.py
--rw-r--r--   0 chris      (501) staff       (20)    32151 2024-03-28 21:53:42.000000 torch_log_wmse_audio_quality-0.1.2/torch_log_wmse_audio_quality/filter_ir.pkl
--rw-r--r--   0 chris      (501) staff       (20)     5747 2024-05-16 16:39:36.000000 torch_log_wmse_audio_quality-0.1.2/torch_log_wmse_audio_quality/freq_weighting_filter.py
--rw-r--r--   0 chris      (501) staff       (20)     5473 2024-05-16 17:39:28.000000 torch_log_wmse_audio_quality-0.1.2/torch_log_wmse_audio_quality/metric.py
--rw-r--r--   0 chris      (501) staff       (20)      947 2024-05-15 18:39:32.000000 torch_log_wmse_audio_quality-0.1.2/torch_log_wmse_audio_quality/utils.py
-drwxr-xr-x   0 chris      (501) staff       (20)        0 2024-05-16 17:48:13.217063 torch_log_wmse_audio_quality-0.1.2/torch_log_wmse_audio_quality.egg-info/
--rw-r--r--   0 chris      (501) staff       (20)     7396 2024-05-16 17:48:13.000000 torch_log_wmse_audio_quality-0.1.2/torch_log_wmse_audio_quality.egg-info/PKG-INFO
--rw-r--r--   0 chris      (501) staff       (20)      579 2024-05-16 17:48:13.000000 torch_log_wmse_audio_quality-0.1.2/torch_log_wmse_audio_quality.egg-info/SOURCES.txt
--rw-r--r--   0 chris      (501) staff       (20)        1 2024-05-16 17:48:13.000000 torch_log_wmse_audio_quality-0.1.2/torch_log_wmse_audio_quality.egg-info/dependency_links.txt
--rw-r--r--   0 chris      (501) staff       (20)       45 2024-05-16 17:48:13.000000 torch_log_wmse_audio_quality-0.1.2/torch_log_wmse_audio_quality.egg-info/requires.txt
--rw-r--r--   0 chris      (501) staff       (20)       29 2024-05-16 17:48:13.000000 torch_log_wmse_audio_quality-0.1.2/torch_log_wmse_audio_quality.egg-info/top_level.txt
+drwxr-xr-x   0 chris      (501) staff       (20)        0 2024-05-16 17:58:28.439804 torch_log_wmse_audio_quality-0.1.3/
+-rw-r--r--   0 chris      (501) staff       (20)    11370 2024-05-15 20:08:40.000000 torch_log_wmse_audio_quality-0.1.3/LICENSE
+-rw-r--r--   0 chris      (501) staff       (20)     7425 2024-05-16 17:58:28.439738 torch_log_wmse_audio_quality-0.1.3/PKG-INFO
+-rw-r--r--   0 chris      (501) staff       (20)     6596 2024-05-16 17:58:07.000000 torch_log_wmse_audio_quality-0.1.3/README.md
+-rw-r--r--   0 chris      (501) staff       (20)      103 2024-05-15 21:20:06.000000 torch_log_wmse_audio_quality-0.1.3/pyproject.toml
+-rw-r--r--   0 chris      (501) staff       (20)     1038 2024-05-16 17:58:28.440080 torch_log_wmse_audio_quality-0.1.3/setup.cfg
+drwxr-xr-x   0 chris      (501) staff       (20)        0 2024-05-16 17:58:28.435758 torch_log_wmse_audio_quality-0.1.3/tests/
+-rw-r--r--   0 chris      (501) staff       (20)     4159 2024-05-16 17:08:03.000000 torch_log_wmse_audio_quality-0.1.3/tests/test_metric.py
+drwxr-xr-x   0 chris      (501) staff       (20)        0 2024-05-16 17:58:28.437939 torch_log_wmse_audio_quality-0.1.3/torch_log_wmse_audio_quality/
+-rw-r--r--   0 chris      (501) staff       (20)       51 2024-05-15 20:27:31.000000 torch_log_wmse_audio_quality-0.1.3/torch_log_wmse_audio_quality/__init__.py
+-rw-r--r--   0 chris      (501) staff       (20)      599 2024-03-29 20:25:42.000000 torch_log_wmse_audio_quality-0.1.3/torch_log_wmse_audio_quality/constants.py
+-rw-r--r--   0 chris      (501) staff       (20)    32151 2024-03-28 21:53:42.000000 torch_log_wmse_audio_quality-0.1.3/torch_log_wmse_audio_quality/filter_ir.pkl
+-rw-r--r--   0 chris      (501) staff       (20)     5747 2024-05-16 16:39:36.000000 torch_log_wmse_audio_quality-0.1.3/torch_log_wmse_audio_quality/freq_weighting_filter.py
+drwxr-xr-x   0 chris      (501) staff       (20)        0 2024-05-16 17:58:28.438976 torch_log_wmse_audio_quality-0.1.3/torch_log_wmse_audio_quality/images/
+-rw-r--r--   0 chris      (501) staff       (20)    31278 2024-03-28 21:53:42.000000 torch_log_wmse_audio_quality-0.1.3/torch_log_wmse_audio_quality/images/frequency_weighting.png
+-rw-r--r--   0 chris      (501) staff       (20)     5473 2024-05-16 17:39:28.000000 torch_log_wmse_audio_quality-0.1.3/torch_log_wmse_audio_quality/metric.py
+-rw-r--r--   0 chris      (501) staff       (20)      947 2024-05-15 18:39:32.000000 torch_log_wmse_audio_quality-0.1.3/torch_log_wmse_audio_quality/utils.py
+drwxr-xr-x   0 chris      (501) staff       (20)        0 2024-05-16 17:58:28.439415 torch_log_wmse_audio_quality-0.1.3/torch_log_wmse_audio_quality.egg-info/
+-rw-r--r--   0 chris      (501) staff       (20)     7425 2024-05-16 17:58:28.000000 torch_log_wmse_audio_quality-0.1.3/torch_log_wmse_audio_quality.egg-info/PKG-INFO
+-rw-r--r--   0 chris      (501) staff       (20)      639 2024-05-16 17:58:28.000000 torch_log_wmse_audio_quality-0.1.3/torch_log_wmse_audio_quality.egg-info/SOURCES.txt
+-rw-r--r--   0 chris      (501) staff       (20)        1 2024-05-16 17:58:28.000000 torch_log_wmse_audio_quality-0.1.3/torch_log_wmse_audio_quality.egg-info/dependency_links.txt
+-rw-r--r--   0 chris      (501) staff       (20)       45 2024-05-16 17:58:28.000000 torch_log_wmse_audio_quality-0.1.3/torch_log_wmse_audio_quality.egg-info/requires.txt
+-rw-r--r--   0 chris      (501) staff       (20)       29 2024-05-16 17:58:28.000000 torch_log_wmse_audio_quality-0.1.3/torch_log_wmse_audio_quality.egg-info/top_level.txt
```

### Comparing `torch_log_wmse_audio_quality-0.1.2/LICENSE` & `torch_log_wmse_audio_quality-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `torch_log_wmse_audio_quality-0.1.2/PKG-INFO` & `torch_log_wmse_audio_quality-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torch-log-wmse-audio-quality
-Version: 0.1.2
+Version: 0.1.3
 Summary: logWMSE is an audio quality metric & loss function with support for digital silence target. Useful for training and evaluating audio source separation systems.
 Home-page: https://github.com/crlandsc/torch-log-wmse-audio-quality
 Author: Christopher Landschoot
 Author-email: crlandschoot@gmail.com
 License: Apache License 2.0
 Project-URL: Bug Tracker, https://github.com/crlandsc/torch-log-wmse-audio-quality/issues
 Classifier: Programming Language :: Python :: 3
@@ -80,15 +80,15 @@
 - Invariant to the tiny errors of MSE that are inaudible to humans.
 - Logarithmic, reflecting the logarithmic sensitivity of human hearing.
 - Tailored specifically for audio signals.
 
 ##### Frequency Weighting
 To measure the frequencies of a signal closer to that of human hearing, the following frequency weighting is applied. This helps the model effectively pay less attention to errors at frequencies that humans are not sensitive to (e.g. 50 Hz) and give more weight to those that we are acutely tuned to (e.g. 3kHz).
 
-![Frequency Weighting](images/frequency_weighting.png)
+![Frequency Weighting](torch_log_wmse_audio_quality/images/frequency_weighting.png)
 
 This metric has been constructed with high fidelity audio in mind (sample rates &ge; 44.1kHz). It theoretically could work for lower sample rates, like 16kHz, but the metric performs an internal resampling to 44.1kHz for consistency across any input sample rates.
 
 ##### Inputs
 Unlike many audio quality metrics, logWMSE accepts 3 audio inputs rather than 2:
 
 - Unprocessed audio (e.g. raw, noisy audio)
```

### Comparing `torch_log_wmse_audio_quality-0.1.2/README.md` & `torch_log_wmse_audio_quality-0.1.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -61,15 +61,15 @@
 - Invariant to the tiny errors of MSE that are inaudible to humans.
 - Logarithmic, reflecting the logarithmic sensitivity of human hearing.
 - Tailored specifically for audio signals.
 
 ##### Frequency Weighting
 To measure the frequencies of a signal closer to that of human hearing, the following frequency weighting is applied. This helps the model effectively pay less attention to errors at frequencies that humans are not sensitive to (e.g. 50 Hz) and give more weight to those that we are acutely tuned to (e.g. 3kHz).
 
-![Frequency Weighting](images/frequency_weighting.png)
+![Frequency Weighting](torch_log_wmse_audio_quality/images/frequency_weighting.png)
 
 This metric has been constructed with high fidelity audio in mind (sample rates &ge; 44.1kHz). It theoretically could work for lower sample rates, like 16kHz, but the metric performs an internal resampling to 44.1kHz for consistency across any input sample rates.
 
 ##### Inputs
 Unlike many audio quality metrics, logWMSE accepts 3 audio inputs rather than 2:
 
 - Unprocessed audio (e.g. raw, noisy audio)
```

### Comparing `torch_log_wmse_audio_quality-0.1.2/setup.cfg` & `torch_log_wmse_audio_quality-0.1.3/setup.cfg`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = torch-log-wmse-audio-quality
-version = 0.1.2
+version = 0.1.3
 author = Christopher Landschoot
 author_email = crlandschoot@gmail.com
 license = Apache License 2.0
 description = logWMSE is an audio quality metric & loss function with support for digital silence target. Useful for training and evaluating audio source separation systems.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/crlandsc/torch-log-wmse-audio-quality
@@ -21,15 +21,15 @@
 python_requires = >=3.8
 install_requires = 
 	torch>=1.8.0
 	torchaudio>=1.8.0
 	numpy>=1.23.5
 
 [options.package_data]
-torch_log_wmse_audio_quality = filter_ir.pkl
+torch_log_wmse_audio_quality = filter_ir.pkl, images/frequency_weighting.png
 
 [options.packages.find]
 where = .
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `torch_log_wmse_audio_quality-0.1.2/tests/test_metric.py` & `torch_log_wmse_audio_quality-0.1.3/tests/test_metric.py`

 * *Files identical despite different names*

### Comparing `torch_log_wmse_audio_quality-0.1.2/torch_log_wmse_audio_quality/constants.py` & `torch_log_wmse_audio_quality-0.1.3/torch_log_wmse_audio_quality/constants.py`

 * *Files identical despite different names*

### Comparing `torch_log_wmse_audio_quality-0.1.2/torch_log_wmse_audio_quality/filter_ir.pkl` & `torch_log_wmse_audio_quality-0.1.3/torch_log_wmse_audio_quality/filter_ir.pkl`

 * *Files identical despite different names*

### Comparing `torch_log_wmse_audio_quality-0.1.2/torch_log_wmse_audio_quality/freq_weighting_filter.py` & `torch_log_wmse_audio_quality-0.1.3/torch_log_wmse_audio_quality/freq_weighting_filter.py`

 * *Files identical despite different names*

### Comparing `torch_log_wmse_audio_quality-0.1.2/torch_log_wmse_audio_quality/metric.py` & `torch_log_wmse_audio_quality-0.1.3/torch_log_wmse_audio_quality/metric.py`

 * *Files identical despite different names*

### Comparing `torch_log_wmse_audio_quality-0.1.2/torch_log_wmse_audio_quality/utils.py` & `torch_log_wmse_audio_quality-0.1.3/torch_log_wmse_audio_quality/utils.py`

 * *Files identical despite different names*

### Comparing `torch_log_wmse_audio_quality-0.1.2/torch_log_wmse_audio_quality.egg-info/PKG-INFO` & `torch_log_wmse_audio_quality-0.1.3/torch_log_wmse_audio_quality.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torch-log-wmse-audio-quality
-Version: 0.1.2
+Version: 0.1.3
 Summary: logWMSE is an audio quality metric & loss function with support for digital silence target. Useful for training and evaluating audio source separation systems.
 Home-page: https://github.com/crlandsc/torch-log-wmse-audio-quality
 Author: Christopher Landschoot
 Author-email: crlandschoot@gmail.com
 License: Apache License 2.0
 Project-URL: Bug Tracker, https://github.com/crlandsc/torch-log-wmse-audio-quality/issues
 Classifier: Programming Language :: Python :: 3
@@ -80,15 +80,15 @@
 - Invariant to the tiny errors of MSE that are inaudible to humans.
 - Logarithmic, reflecting the logarithmic sensitivity of human hearing.
 - Tailored specifically for audio signals.
 
 ##### Frequency Weighting
 To measure the frequencies of a signal closer to that of human hearing, the following frequency weighting is applied. This helps the model effectively pay less attention to errors at frequencies that humans are not sensitive to (e.g. 50 Hz) and give more weight to those that we are acutely tuned to (e.g. 3kHz).
 
-![Frequency Weighting](images/frequency_weighting.png)
+![Frequency Weighting](torch_log_wmse_audio_quality/images/frequency_weighting.png)
 
 This metric has been constructed with high fidelity audio in mind (sample rates &ge; 44.1kHz). It theoretically could work for lower sample rates, like 16kHz, but the metric performs an internal resampling to 44.1kHz for consistency across any input sample rates.
 
 ##### Inputs
 Unlike many audio quality metrics, logWMSE accepts 3 audio inputs rather than 2:
 
 - Unprocessed audio (e.g. raw, noisy audio)
```

### Comparing `torch_log_wmse_audio_quality-0.1.2/torch_log_wmse_audio_quality.egg-info/SOURCES.txt` & `torch_log_wmse_audio_quality-0.1.3/torch_log_wmse_audio_quality.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -9,8 +9,9 @@
 torch_log_wmse_audio_quality/freq_weighting_filter.py
 torch_log_wmse_audio_quality/metric.py
 torch_log_wmse_audio_quality/utils.py
 torch_log_wmse_audio_quality.egg-info/PKG-INFO
 torch_log_wmse_audio_quality.egg-info/SOURCES.txt
 torch_log_wmse_audio_quality.egg-info/dependency_links.txt
 torch_log_wmse_audio_quality.egg-info/requires.txt
-torch_log_wmse_audio_quality.egg-info/top_level.txt
+torch_log_wmse_audio_quality.egg-info/top_level.txt
+torch_log_wmse_audio_quality/images/frequency_weighting.png
```

