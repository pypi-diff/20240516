# Comparing `tmp/icad_tone_detection-1.2.tar.gz` & `tmp/icad_tone_detection-1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "icad_tone_detection-1.2.tar", last modified: Tue May 14 20:24:07 2024, max compression
+gzip compressed data, was "icad_tone_detection-1.3.tar", last modified: Wed May 15 23:39:45 2024, max compression
```

## Comparing `icad_tone_detection-1.2.tar` & `icad_tone_detection-1.3.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 20:24:07.488980 icad_tone_detection-1.2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 20:24:07.484980 icad_tone_detection-1.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 20:24:07.484980 icad_tone_detection-1.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1823 2024-05-14 20:23:57.000000 icad_tone_detection-1.2/.github/workflows/python-package.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3084 2024-05-14 20:23:57.000000 icad_tone_detection-1.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      555 2024-05-14 20:23:57.000000 icad_tone_detection-1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-14 20:23:57.000000 icad_tone_detection-1.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-05-14 20:24:07.488980 icad_tone_detection-1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      457 2024-05-14 20:23:57.000000 icad_tone_detection-1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 20:24:07.484980 icad_tone_detection-1.2/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      498 2024-05-14 20:23:57.000000 icad_tone_detection-1.2/examples/detect_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 20:24:07.488980 icad_tone_detection-1.2/examples/example_audio/
--rw-r--r--   0 runner    (1001) docker     (127)   282092 2024-05-14 20:23:57.000000 icad_tone_detection-1.2/examples/example_audio/hi_low_tone_example.wav
--rw-r--r--   0 runner    (1001) docker     (127)   799686 2024-05-14 20:23:57.000000 icad_tone_detection-1.2/examples/example_audio/long_tone_example.wav
--rw-r--r--   0 runner    (1001) docker     (127)   805000 2024-05-14 20:23:57.000000 icad_tone_detection-1.2/examples/example_audio/two_tone_example.wav
--rw-r--r--   0 runner    (1001) docker     (127)      962 2024-05-14 20:23:57.000000 icad_tone_detection-1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 20:24:07.488980 icad_tone_detection-1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 20:23:57.000000 icad_tone_detection-1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 20:24:07.484980 icad_tone_detection-1.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 20:24:07.488980 icad_tone_detection-1.2/src/icad_tone_detection/
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-14 20:23:57.000000 icad_tone_detection-1.2/src/icad_tone_detection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2599 2024-05-14 20:23:57.000000 icad_tone_detection-1.2/src/icad_tone_detection/audio_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)     6330 2024-05-14 20:23:57.000000 icad_tone_detection-1.2/src/icad_tone_detection/frequency_extraction.py
--rw-r--r--   0 runner    (1001) docker     (127)     2977 2024-05-14 20:23:57.000000 icad_tone_detection-1.2/src/icad_tone_detection/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     6282 2024-05-14 20:23:57.000000 icad_tone_detection-1.2/src/icad_tone_detection/tone_detection.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 20:24:07.488980 icad_tone_detection-1.2/src/icad_tone_detection.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-05-14 20:24:07.000000 icad_tone_detection-1.2/src/icad_tone_detection.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      693 2024-05-14 20:24:07.000000 icad_tone_detection-1.2/src/icad_tone_detection.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 20:24:07.000000 icad_tone_detection-1.2/src/icad_tone_detection.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-14 20:24:07.000000 icad_tone_detection-1.2/src/icad_tone_detection.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-14 20:24:07.000000 icad_tone_detection-1.2/src/icad_tone_detection.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:39:45.563603 icad_tone_detection-1.3/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:39:45.555603 icad_tone_detection-1.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:39:45.559603 icad_tone_detection-1.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1823 2024-05-15 23:39:31.000000 icad_tone_detection-1.3/.github/workflows/python-package.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3084 2024-05-15 23:39:31.000000 icad_tone_detection-1.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      555 2024-05-15 23:39:31.000000 icad_tone_detection-1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-15 23:39:31.000000 icad_tone_detection-1.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-05-15 23:39:45.563603 icad_tone_detection-1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      457 2024-05-15 23:39:31.000000 icad_tone_detection-1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:39:45.559603 icad_tone_detection-1.3/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2024-05-15 23:39:31.000000 icad_tone_detection-1.3/examples/detect_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:39:45.559603 icad_tone_detection-1.3/examples/example_audio/
+-rw-r--r--   0 runner    (1001) docker     (127)   282092 2024-05-15 23:39:31.000000 icad_tone_detection-1.3/examples/example_audio/hi_low_tone_example.wav
+-rw-r--r--   0 runner    (1001) docker     (127)   799686 2024-05-15 23:39:31.000000 icad_tone_detection-1.3/examples/example_audio/long_tone_example.wav
+-rw-r--r--   0 runner    (1001) docker     (127)   805000 2024-05-15 23:39:31.000000 icad_tone_detection-1.3/examples/example_audio/two_tone_example.wav
+-rw-r--r--   0 runner    (1001) docker     (127)      962 2024-05-15 23:39:31.000000 icad_tone_detection-1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 23:39:45.563603 icad_tone_detection-1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 23:39:31.000000 icad_tone_detection-1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:39:45.555603 icad_tone_detection-1.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:39:45.563603 icad_tone_detection-1.3/src/icad_tone_detection/
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-15 23:39:31.000000 icad_tone_detection-1.3/src/icad_tone_detection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2591 2024-05-15 23:39:31.000000 icad_tone_detection-1.3/src/icad_tone_detection/audio_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6318 2024-05-15 23:39:31.000000 icad_tone_detection-1.3/src/icad_tone_detection/frequency_extraction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2990 2024-05-15 23:39:31.000000 icad_tone_detection-1.3/src/icad_tone_detection/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6282 2024-05-15 23:39:31.000000 icad_tone_detection-1.3/src/icad_tone_detection/tone_detection.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:39:45.563603 icad_tone_detection-1.3/src/icad_tone_detection.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-05-15 23:39:45.000000 icad_tone_detection-1.3/src/icad_tone_detection.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      693 2024-05-15 23:39:45.000000 icad_tone_detection-1.3/src/icad_tone_detection.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 23:39:45.000000 icad_tone_detection-1.3/src/icad_tone_detection.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-15 23:39:45.000000 icad_tone_detection-1.3/src/icad_tone_detection.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-15 23:39:45.000000 icad_tone_detection-1.3/src/icad_tone_detection.egg-info/top_level.txt
```

### Comparing `icad_tone_detection-1.2/.github/workflows/python-package.yml` & `icad_tone_detection-1.3/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `icad_tone_detection-1.2/.gitignore` & `icad_tone_detection-1.3/.gitignore`

 * *Files identical despite different names*

### Comparing `icad_tone_detection-1.2/LICENSE` & `icad_tone_detection-1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `icad_tone_detection-1.2/PKG-INFO` & `icad_tone_detection-1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: icad_tone_detection
-Version: 1.2
+Version: 1.3
 Summary: A Python library for extracting scanner radio tones from scanner audio.
 Author-email: TheGreatCodeholio <ian@icarey.net>
 Project-URL: Homepage, https://github.com/thegreatcodeholio/icad_tone_detection
 Project-URL: Issues, https://github.com/thegreatcodeholio/icad_tone_detection/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `icad_tone_detection-1.2/examples/example_audio/hi_low_tone_example.wav` & `icad_tone_detection-1.3/examples/example_audio/hi_low_tone_example.wav`

 * *Files identical despite different names*

### Comparing `icad_tone_detection-1.2/examples/example_audio/long_tone_example.wav` & `icad_tone_detection-1.3/examples/example_audio/long_tone_example.wav`

 * *Files identical despite different names*

### Comparing `icad_tone_detection-1.2/examples/example_audio/two_tone_example.wav` & `icad_tone_detection-1.3/examples/example_audio/two_tone_example.wav`

 * *Files identical despite different names*

### Comparing `icad_tone_detection-1.2/pyproject.toml` & `icad_tone_detection-1.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "icad_tone_detection"
-version = "1.2"
+version = "1.3"
 authors = [
   {name = "TheGreatCodeholio", email = "ian@icarey.net"},
 ]
 description = "A Python library for extracting scanner radio tones from scanner audio."
 readme = "README.md"
 requires-python = ">=3.10"
 dependencies = [
```

### Comparing `icad_tone_detection-1.2/src/icad_tone_detection/audio_loader.py` & `icad_tone_detection-1.3/src/icad_tone_detection/audio_loader.py`

 * *Files 7% similar despite different names*

```diff
@@ -34,15 +34,16 @@
         raise ValueError("Unsupported audio input type. Must be a file path, URL, Bytes object, or Pydub AudioSegment.")
 
     # Processing
     try:
         audio = audio.set_channels(1)  # Ensure the audio is mono
         audio = audio.set_frame_rate(22050)  # Set the frame rate to 22050 Hz
         samples = np.array(audio.get_array_of_samples()).astype(np.float32)
-        samples /= np.iinfo(audio.sample_width * 8).max  # Adjusted for correct normalization
+        max_val = float(2 ** (audio.sample_width * 8 - 1))
+        samples /= max_val
     except Exception as e:
         raise RuntimeError(f"Error processing audio: {e}")
 
     return samples, audio.frame_rate, audio.duration_seconds
 
 
 def get_audio_from_url(url):
```

### Comparing `icad_tone_detection-1.2/src/icad_tone_detection/frequency_extraction.py` & `icad_tone_detection-1.3/src/icad_tone_detection/frequency_extraction.py`

 * *Files 3% similar despite different names*

```diff
@@ -74,15 +74,15 @@
         return base_frequency * self.matching_threshold / 100
 
     def calculate_times(self, start_index, end_index, time_samples):
         """
         Calculates accurate start and end times for frequency matches.
         """
         start_time = round(time_samples[start_index], 3)
-        end_time = round(time_samples[end_index - 1], 3)
+        end_time = round(time_samples[end_index], 3)  # Use end_index directly
         return start_time, end_time
 
     @staticmethod
     def amplitude_to_decibels(amplitude, reference_value):
         """
         Converts amplitude to decibels relative to a reference value.
 
@@ -95,23 +95,23 @@
         """
         # Ensure the reference is not zero to avoid division by zero
         reference_value = np.maximum(reference_value, 1e-20)
         return 20 * np.log10(np.maximum(amplitude, 1e-20) / reference_value)
 
     def match_frequencies(self, detected_frequencies, time_samples):
         """
-            Identifies and groups matching frequencies from a list of detected frequencies based on the matching threshold.
-            Each group's start time, end time, and the matching frequencies are returned.
+        Identifies and groups matching frequencies from a list of detected frequencies based on the matching threshold.
+        Each group's start time, end time, and the matching frequencies are returned.
 
-            Parameters:
-                detected_frequencies (list of float): The detected frequencies from the audio sample.
-                time_samples (np.array): Array of times corresponding to each frequency sample.
+        Parameters:
+            detected_frequencies (list of float): The detected frequencies from the audio sample.
+            time_samples (np.array): Array of times corresponding to each frequency sample.
 
-            Returns:
-                list of tuples: Each tuple contains the start time, end time, and a list of matching frequencies.
+        Returns:
+            list of tuples: Each tuple contains the start time, end time, and a list of matching frequencies.
         """
 
         if not detected_frequencies:
             return []
 
         try:
             frequencies = [round(f, 1) for f in detected_frequencies]
@@ -121,22 +121,22 @@
 
             for i in range(1, len(frequencies)):
                 threshold = self.dynamic_threshold(frequencies, i)
                 if abs(frequencies[i] - frequencies[i - 1]) <= threshold:
                     current_match.append(frequencies[i])
                 else:
                     if len(current_match) >= 2:
-                        start_time, end_time = self.calculate_times(start_index, i, time_samples)
-                        freq_length = round((end_time - start_time) + .1, 2)
+                        start_time, end_time = self.calculate_times(start_index, i - 1, time_samples)
+                        freq_length = round(end_time - start_time, 3)
                         matching_frequencies.append((start_time, end_time, freq_length, current_match))
                     current_match = [frequencies[i]]
                     start_index = i
 
             if len(current_match) >= 2:
-                start_time, end_time = self.calculate_times(start_index, len(frequencies), time_samples)
-                freq_length = round((end_time - start_time) + .1, 2)
+                start_time, end_time = self.calculate_times(start_index, len(frequencies) - 1, time_samples)
+                freq_length = round(end_time - start_time, 3)
                 matching_frequencies.append((start_time, end_time, freq_length, current_match))
 
             return matching_frequencies
         except Exception as e:
             print(f"Error matching frequencies: {e}")
             return []
```

### Comparing `icad_tone_detection-1.2/src/icad_tone_detection/main.py` & `icad_tone_detection-1.3/src/icad_tone_detection/main.py`

 * *Files 17% similar despite different names*

```diff
@@ -6,30 +6,30 @@
 class ToneDetectionResult:
     def __init__(self, two_tone_result, long_result, hi_low_result):
         self.two_tone_result = two_tone_result
         self.long_result = long_result
         self.hi_low_result = hi_low_result
 
 
-def tone_detect(audio_path, matching_threshold=2, time_resolution_ms=100, tone_a_min_length=0.8, tone_b_min_length=2.8, hi_low_interval=0.2,
-                hi_low_min_alternations=4, long_tone_min_length=3.8, debug=False):
+def tone_detect(audio_path, matching_threshold=2.5, time_resolution_ms=25, tone_a_min_length=0.7, tone_b_min_length=2.7, hi_low_interval=0.2,
+                hi_low_min_alternations=6, long_tone_min_length=3.8, debug=False):
     """
         Loads audio from various sources including local path, URL, BytesIO object, or a PyDub AudioSegment.
 
         Parameters:
            - audio_input: Can be a string (path or URL), bytes like object, or AudioSegment.
            - matching_threshold (float): The percentage threshold used to determine if two frequencies
                 are considered a match. For example, a threshold of 2 means that two frequencies are considered matching
-                if they are within 2% of each other.
-           - time_resolution_ms (int): The time resolution in milliseconds for the STFT. Default is 100ms.
+                if they are within x% of each other. Default 2.5%
+           - time_resolution_ms (int): The time resolution in milliseconds for the STFT. Default is 25ms.
            - tone_a_min_length (float): The minimum length in seconds of an A tone for two tone detections. Default 0.8 Seconds
            - tone_b_min_length (float): The minimum length in seconds of a B tone for two tone detections. Default 2.8 Seconds
            - long_tone_min_length (float): The minimum length a long tone needs to be to consider it a match. Default 3.8 Seconds
            - hi_low_interval (float): The maximum allowed interval in seconds between two consecutive alternating tones. Default is 0.2 Seconds
-           - hi_low_min_alternations (int): The minimum number of alternations for a hi-low warble tone sequence to be considered valid. Default 4
+           - hi_low_min_alternations (int): The minimum number of alternations for a hi-low warble tone sequence to be considered valid. Default 6
            - debug (bool): If debug is enabled, print all tones found in audio file. Default is False
 
         Returns:
            - An instance of ToneDetectionResult containing information about the found tones in the audio.
 
         Raises:
             -ValueError for unsupported audio input types or errors in processing.
```

### Comparing `icad_tone_detection-1.2/src/icad_tone_detection/tone_detection.py` & `icad_tone_detection-1.3/src/icad_tone_detection/tone_detection.py`

 * *Files identical despite different names*

### Comparing `icad_tone_detection-1.2/src/icad_tone_detection.egg-info/PKG-INFO` & `icad_tone_detection-1.3/src/icad_tone_detection.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: icad_tone_detection
-Version: 1.2
+Version: 1.3
 Summary: A Python library for extracting scanner radio tones from scanner audio.
 Author-email: TheGreatCodeholio <ian@icarey.net>
 Project-URL: Homepage, https://github.com/thegreatcodeholio/icad_tone_detection
 Project-URL: Issues, https://github.com/thegreatcodeholio/icad_tone_detection/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `icad_tone_detection-1.2/src/icad_tone_detection.egg-info/SOURCES.txt` & `icad_tone_detection-1.3/src/icad_tone_detection.egg-info/SOURCES.txt`

 * *Files identical despite different names*

