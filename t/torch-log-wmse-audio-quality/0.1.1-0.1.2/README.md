# Comparing `tmp/torch_log_wmse_audio_quality-0.1.1.tar.gz` & `tmp/torch_log_wmse_audio_quality-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torch_log_wmse_audio_quality-0.1.1.tar", last modified: Thu May 16 01:03:56 2024, max compression
+gzip compressed data, was "torch_log_wmse_audio_quality-0.1.2.tar", last modified: Thu May 16 17:48:13 2024, max compression
```

## Comparing `torch_log_wmse_audio_quality-0.1.1.tar` & `torch_log_wmse_audio_quality-0.1.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 chris      (501) staff       (20)        0 2024-05-16 01:03:56.811643 torch_log_wmse_audio_quality-0.1.1/
--rw-r--r--   0 chris      (501) staff       (20)    11370 2024-05-15 20:08:40.000000 torch_log_wmse_audio_quality-0.1.1/LICENSE
--rw-r--r--   0 chris      (501) staff       (20)     4296 2024-05-16 01:03:56.811578 torch_log_wmse_audio_quality-0.1.1/PKG-INFO
--rw-r--r--   0 chris      (501) staff       (20)     3467 2024-05-15 22:43:18.000000 torch_log_wmse_audio_quality-0.1.1/README.md
--rw-r--r--   0 chris      (501) staff       (20)      103 2024-05-15 21:20:06.000000 torch_log_wmse_audio_quality-0.1.1/pyproject.toml
--rw-r--r--   0 chris      (501) staff       (20)     1006 2024-05-16 01:03:56.811931 torch_log_wmse_audio_quality-0.1.1/setup.cfg
-drwxr-xr-x   0 chris      (501) staff       (20)        0 2024-05-16 01:03:56.805201 torch_log_wmse_audio_quality-0.1.1/tests/
--rw-r--r--   0 chris      (501) staff       (20)     4165 2024-05-15 21:48:36.000000 torch_log_wmse_audio_quality-0.1.1/tests/test_metric.py
-drwxr-xr-x   0 chris      (501) staff       (20)        0 2024-05-16 01:03:56.810216 torch_log_wmse_audio_quality-0.1.1/torch_log_wmse_audio_quality/
--rw-r--r--   0 chris      (501) staff       (20)       51 2024-05-15 20:27:31.000000 torch_log_wmse_audio_quality-0.1.1/torch_log_wmse_audio_quality/__init__.py
--rw-r--r--   0 chris      (501) staff       (20)      599 2024-03-29 20:25:42.000000 torch_log_wmse_audio_quality-0.1.1/torch_log_wmse_audio_quality/constants.py
--rw-r--r--   0 chris      (501) staff       (20)    32151 2024-03-28 21:53:42.000000 torch_log_wmse_audio_quality-0.1.1/torch_log_wmse_audio_quality/filter_ir.pkl
--rw-r--r--   0 chris      (501) staff       (20)     5747 2024-05-16 01:00:43.000000 torch_log_wmse_audio_quality-0.1.1/torch_log_wmse_audio_quality/freq_weighting_filter.py
--rw-r--r--   0 chris      (501) staff       (20)     5348 2024-05-15 19:52:25.000000 torch_log_wmse_audio_quality-0.1.1/torch_log_wmse_audio_quality/metric.py
--rw-r--r--   0 chris      (501) staff       (20)      947 2024-05-15 18:39:32.000000 torch_log_wmse_audio_quality-0.1.1/torch_log_wmse_audio_quality/utils.py
-drwxr-xr-x   0 chris      (501) staff       (20)        0 2024-05-16 01:03:56.811271 torch_log_wmse_audio_quality-0.1.1/torch_log_wmse_audio_quality.egg-info/
--rw-r--r--   0 chris      (501) staff       (20)     4296 2024-05-16 01:03:56.000000 torch_log_wmse_audio_quality-0.1.1/torch_log_wmse_audio_quality.egg-info/PKG-INFO
--rw-r--r--   0 chris      (501) staff       (20)      579 2024-05-16 01:03:56.000000 torch_log_wmse_audio_quality-0.1.1/torch_log_wmse_audio_quality.egg-info/SOURCES.txt
--rw-r--r--   0 chris      (501) staff       (20)        1 2024-05-16 01:03:56.000000 torch_log_wmse_audio_quality-0.1.1/torch_log_wmse_audio_quality.egg-info/dependency_links.txt
--rw-r--r--   0 chris      (501) staff       (20)       45 2024-05-16 01:03:56.000000 torch_log_wmse_audio_quality-0.1.1/torch_log_wmse_audio_quality.egg-info/requires.txt
--rw-r--r--   0 chris      (501) staff       (20)       29 2024-05-16 01:03:56.000000 torch_log_wmse_audio_quality-0.1.1/torch_log_wmse_audio_quality.egg-info/top_level.txt
+drwxr-xr-x   0 chris      (501) staff       (20)        0 2024-05-16 17:48:13.217533 torch_log_wmse_audio_quality-0.1.2/
+-rw-r--r--   0 chris      (501) staff       (20)    11370 2024-05-15 20:08:40.000000 torch_log_wmse_audio_quality-0.1.2/LICENSE
+-rw-r--r--   0 chris      (501) staff       (20)     7396 2024-05-16 17:48:13.217454 torch_log_wmse_audio_quality-0.1.2/PKG-INFO
+-rw-r--r--   0 chris      (501) staff       (20)     6567 2024-05-16 17:47:05.000000 torch_log_wmse_audio_quality-0.1.2/README.md
+-rw-r--r--   0 chris      (501) staff       (20)      103 2024-05-15 21:20:06.000000 torch_log_wmse_audio_quality-0.1.2/pyproject.toml
+-rw-r--r--   0 chris      (501) staff       (20)     1006 2024-05-16 17:48:13.217825 torch_log_wmse_audio_quality-0.1.2/setup.cfg
+drwxr-xr-x   0 chris      (501) staff       (20)        0 2024-05-16 17:48:13.213631 torch_log_wmse_audio_quality-0.1.2/tests/
+-rw-r--r--   0 chris      (501) staff       (20)     4159 2024-05-16 17:08:03.000000 torch_log_wmse_audio_quality-0.1.2/tests/test_metric.py
+drwxr-xr-x   0 chris      (501) staff       (20)        0 2024-05-16 17:48:13.215646 torch_log_wmse_audio_quality-0.1.2/torch_log_wmse_audio_quality/
+-rw-r--r--   0 chris      (501) staff       (20)       51 2024-05-15 20:27:31.000000 torch_log_wmse_audio_quality-0.1.2/torch_log_wmse_audio_quality/__init__.py
+-rw-r--r--   0 chris      (501) staff       (20)      599 2024-03-29 20:25:42.000000 torch_log_wmse_audio_quality-0.1.2/torch_log_wmse_audio_quality/constants.py
+-rw-r--r--   0 chris      (501) staff       (20)    32151 2024-03-28 21:53:42.000000 torch_log_wmse_audio_quality-0.1.2/torch_log_wmse_audio_quality/filter_ir.pkl
+-rw-r--r--   0 chris      (501) staff       (20)     5747 2024-05-16 16:39:36.000000 torch_log_wmse_audio_quality-0.1.2/torch_log_wmse_audio_quality/freq_weighting_filter.py
+-rw-r--r--   0 chris      (501) staff       (20)     5473 2024-05-16 17:39:28.000000 torch_log_wmse_audio_quality-0.1.2/torch_log_wmse_audio_quality/metric.py
+-rw-r--r--   0 chris      (501) staff       (20)      947 2024-05-15 18:39:32.000000 torch_log_wmse_audio_quality-0.1.2/torch_log_wmse_audio_quality/utils.py
+drwxr-xr-x   0 chris      (501) staff       (20)        0 2024-05-16 17:48:13.217063 torch_log_wmse_audio_quality-0.1.2/torch_log_wmse_audio_quality.egg-info/
+-rw-r--r--   0 chris      (501) staff       (20)     7396 2024-05-16 17:48:13.000000 torch_log_wmse_audio_quality-0.1.2/torch_log_wmse_audio_quality.egg-info/PKG-INFO
+-rw-r--r--   0 chris      (501) staff       (20)      579 2024-05-16 17:48:13.000000 torch_log_wmse_audio_quality-0.1.2/torch_log_wmse_audio_quality.egg-info/SOURCES.txt
+-rw-r--r--   0 chris      (501) staff       (20)        1 2024-05-16 17:48:13.000000 torch_log_wmse_audio_quality-0.1.2/torch_log_wmse_audio_quality.egg-info/dependency_links.txt
+-rw-r--r--   0 chris      (501) staff       (20)       45 2024-05-16 17:48:13.000000 torch_log_wmse_audio_quality-0.1.2/torch_log_wmse_audio_quality.egg-info/requires.txt
+-rw-r--r--   0 chris      (501) staff       (20)       29 2024-05-16 17:48:13.000000 torch_log_wmse_audio_quality-0.1.2/torch_log_wmse_audio_quality.egg-info/top_level.txt
```

### Comparing `torch_log_wmse_audio_quality-0.1.1/LICENSE` & `torch_log_wmse_audio_quality-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `torch_log_wmse_audio_quality-0.1.1/setup.cfg` & `torch_log_wmse_audio_quality-0.1.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = torch-log-wmse-audio-quality
-version = 0.1.1
+version = 0.1.2
 author = Christopher Landschoot
 author_email = crlandschoot@gmail.com
 license = Apache License 2.0
 description = logWMSE is an audio quality metric & loss function with support for digital silence target. Useful for training and evaluating audio source separation systems.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/crlandsc/torch-log-wmse-audio-quality
```

### Comparing `torch_log_wmse_audio_quality-0.1.1/tests/test_metric.py` & `torch_log_wmse_audio_quality-0.1.2/tests/test_metric.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,26 +21,26 @@
                 self.assertEqual(rms.shape, (2, 2))
 
                 print(f"Test {i}, RMS Value: {rms.mean()}")
 
     def test_calculate_log_wmse(self):
         log_wmse_loss = LogWMSE(audio_length=1.0, sample_rate=44100)
         input_rms = torch.ones(2, 2)
-        processed_audio = torch.ones(2, 2, 3, 44100)
-        target_audio = torch.ones(2, 2, 3, 44100)
+        processed_audio = torch.ones(2, 3, 2, 44100)
+        target_audio = torch.ones(2, 3, 2, 44100)
 
         values = log_wmse_loss._calculate_log_wmse(
             input_rms,
             log_wmse_loss.filters,
             processed_audio,
             target_audio,
         )
 
         self.assertIsInstance(values, torch.Tensor)
-        self.assertEqual(values.shape, (2, 2, 3))
+        self.assertEqual(values.shape, (2, 3, 2))
 
         print(f"Values: {values}")
 
     def test_forward(self):
         audio_lengths = [0.1, 0.5, 1.0]  # Different audio lengths
         sample_rate = 44100
         audio_channels = 2 # stereo
@@ -52,16 +52,16 @@
             for j in range(3):
                 with self.subTest(i=i, j=j):
                     torch.manual_seed((i+1)*(j+1))  # Ensure reproducibility
 
                     # Generate random inputs (scale between -1 and 1)
                     audio_lengths_samples = int(audio_length * sample_rate)
                     unprocessed_audio = 2 * torch.rand(batch, audio_channels, audio_lengths_samples) - 1
-                    processed_audio = unprocessed_audio.unsqueeze(2).expand(-1, -1, audio_stems, -1) * 0.1
-                    target_audio = torch.zeros(batch, audio_channels, audio_stems, audio_lengths_samples)
+                    processed_audio = unprocessed_audio.unsqueeze(1).expand(-1, audio_stems, -1, -1) * 0.1
+                    target_audio = torch.zeros(batch, audio_stems, audio_channels, audio_lengths_samples)
 
                     loss = log_wmse_loss(unprocessed_audio, processed_audio, target_audio)
 
                     self.assertIsInstance(loss, torch.Tensor)
                     self.assertEqual(loss.ndim, 0)
 
                     print(f"Test {i}, Subtest {j}, Audio Length: {audio_length}, Loss: {loss}, Seed: {(i+1)*(j+1)}")
@@ -75,16 +75,16 @@
                 with self.subTest(i=i, j=j):
                     torch.manual_seed((i+1)*(j+1))  # Ensure reproducibility
                     np.random.seed((i+1)*(j+1))  # to make the test reproducible
 
                     # Generate random inputs
                     audio_lengths_samples = int(audio_length * 44100)
                     unprocessed_audio = torch.from_numpy(np.random.rand(2, audio_lengths_samples).astype(np.float32))[None, ...]
-                    processed_audio = torch.from_numpy(np.random.rand(2, audio_lengths_samples).astype(np.float32))[None, :, None, ...].repeat(1, 1, 4, 1)
-                    target_audio = torch.from_numpy(np.random.rand(2, audio_lengths_samples).astype(np.float32))[None, :, None, ...].repeat(1, 1, 4, 1)
+                    processed_audio = torch.from_numpy(np.random.rand(2, audio_lengths_samples).astype(np.float32))[None, None, ...].repeat(1, 4, 1, 1)
+                    target_audio = torch.from_numpy(np.random.rand(2, audio_lengths_samples).astype(np.float32))[None, None, ...].repeat(1, 4, 1, 1)
 
                     loss = log_wmse_loss(unprocessed_audio, processed_audio, target_audio)
 
                     self.assertIsInstance(loss, torch.Tensor)
                     self.assertEqual(loss.ndim, 0)
 
                     print(f"Test {i}, Subtest {j}, Audio Length: {audio_length}, Loss: {loss}, Seed: {(i+1)*(j+1)}")
```

### Comparing `torch_log_wmse_audio_quality-0.1.1/torch_log_wmse_audio_quality/constants.py` & `torch_log_wmse_audio_quality-0.1.2/torch_log_wmse_audio_quality/constants.py`

 * *Files identical despite different names*

### Comparing `torch_log_wmse_audio_quality-0.1.1/torch_log_wmse_audio_quality/filter_ir.pkl` & `torch_log_wmse_audio_quality-0.1.2/torch_log_wmse_audio_quality/filter_ir.pkl`

 * *Files identical despite different names*

### Comparing `torch_log_wmse_audio_quality-0.1.1/torch_log_wmse_audio_quality/freq_weighting_filter.py` & `torch_log_wmse_audio_quality-0.1.2/torch_log_wmse_audio_quality/freq_weighting_filter.py`

 * *Files 0% similar despite different names*

```diff
@@ -98,21 +98,21 @@
 
         NOTE: The original logWMSE metric implementation in numpy used time-domain convolution for
               single-channel/single-batch/single-stem audio. This torch implementation uses FFT convolution
               for efficiency. This will result in slightly different outputs due to the different convolution
               methods.
         
         Args: audio (torch.Tensor): A tensor containing the audio signal to be filtered. 
-                                    Expected shape is [batch, channels, stem, time].
+                                    Expected shape is [batch, stem, channels, time].
         
         Returns: torch.Tensor: The filtered audio signal with the same shape as the input.
         """
-        # Ensure audio has the correct dimensions: [batch, channels, stem, time]
+        # Ensure audio has the correct dimensions: [batch, stem, channels, time]
         if audio.ndim != 4:
-            raise ValueError("Audio input must have dimensions [batch, channels, stem, time].")
+            raise ValueError("Audio input must have dimensions [batch, stem, channels, time].")
 
         # Move impulse response to audio device if necessary
         if self.impulse_response_fft.device != audio.device:
             self.impulse_response_fft = self.impulse_response_fft.to(audio.device)
 
         # Pad audio to match padded FFT size (N+M-1)
         audio = torch.nn.functional.pad(audio, (0, self.fft_size - audio.shape[-1]))
```

### Comparing `torch_log_wmse_audio_quality-0.1.1/torch_log_wmse_audio_quality/metric.py` & `torch_log_wmse_audio_quality-0.1.2/torch_log_wmse_audio_quality/metric.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     Args:
         audio_length (int): The length of the audio signal in seconds.
         sample_rate (int, optional): The sample rate of the audio signal in Hz. Defaults to 44100.
         impulse_response (Tensor, optional): The finite impulse response (FIR) filter for 
             frequency weighting. If None (default), use built-in FIR. Currently only supports
             single-channel FIRs (applied to all batches & audio channels).
         impulse_response_sample_rate (int, optional): The sample rate of the FIR in Hz. Defaults to 44100.
-        return_as_loss (bool, optional): Whether to return the loss value. Defaults to True.
+        return_as_loss (bool, optional): Whether to return the loss value (i.e. negative of the metric). Defaults to True.
     """
     def __init__(
             self,
             audio_length: int,
             sample_rate: int = 44100,
             impulse_response: Optional[Tensor] = None,
             impulse_response_sample_rate: int = 44100,
@@ -56,15 +56,15 @@
     def forward(self, unprocessed_audio: Tensor, processed_audio: Tensor, target_audio: Tensor):
         assert unprocessed_audio.ndim == 3 # unprocessed_audio audio shape: [batch, channel, time]
         assert processed_audio.ndim == 4 # processed_audio audio shape: [batch, channel, stem, time]
         assert target_audio.ndim == 4 # target_audio audio shape: [batch, channel, stem, time]
         assert processed_audio.shape == target_audio.shape # processed_audio and target_audio should have the same shape
         assert processed_audio.shape[-1] == target_audio.shape[-1] == unprocessed_audio.shape[-1] # all should have the same length
 
-        input_rms = calculate_rms(self.filters(unprocessed_audio.unsqueeze(2))) # unsqueeze to add "stem" dimension
+        input_rms = calculate_rms(self.filters(unprocessed_audio.unsqueeze(1))) # unsqueeze to add "stem" dimension
 
         # Avoid log(0)
         if input_rms.sum() == 0:
             return torch.log(torch.tensor(EPS)) * SCALER
 
         # Calculate the logWMSE
         values = self._calculate_log_wmse(
@@ -98,14 +98,16 @@
         Returns:
             Tensor: The logWMSE between the processed audio and target audio.
         """
         # Calculate the scaling factor based on the input RMS
         scaling_factor = 1 / input_rms
 
         # Add extra dimensions to scaling_factor to match the shape of processed_audio and target_audio
+        if scaling_factor.dim() == 2:
+            scaling_factor = scaling_factor.unsqueeze(1)
         while scaling_factor.dim() < processed_audio.dim():
             scaling_factor = scaling_factor.unsqueeze(-1)
 
         # Expand scaling_factor to match the shape of processed_audio and target_audio
         scaling_factor = scaling_factor.expand(*processed_audio.shape)
 
         # Calculate the frequency-weighted differences, ignoring small imperceptible differences
```

### Comparing `torch_log_wmse_audio_quality-0.1.1/torch_log_wmse_audio_quality/utils.py` & `torch_log_wmse_audio_quality-0.1.2/torch_log_wmse_audio_quality/utils.py`

 * *Files identical despite different names*

### Comparing `torch_log_wmse_audio_quality-0.1.1/torch_log_wmse_audio_quality.egg-info/SOURCES.txt` & `torch_log_wmse_audio_quality-0.1.2/torch_log_wmse_audio_quality.egg-info/SOURCES.txt`

 * *Files identical despite different names*

