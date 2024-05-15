# Comparing `tmp/senepy-0.1.1.tar.gz` & `tmp/senepy-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "senepy-0.1.1.tar", last modified: Mon Jan  9 21:17:48 2023, max compression
+gzip compressed data, was "senepy-0.2.0.tar", last modified: Wed May 15 21:57:02 2024, max compression
```

## Comparing `senepy-0.1.1.tar` & `senepy-0.2.0.tar`

### file list

```diff
@@ -1,27 +1,30 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-01-09 21:17:31.000000 senepy-0.1.1/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1073 2023-01-03 20:08:51.000000 senepy-0.1.1/LICENSE
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      619 2023-01-09 21:17:48.000000 senepy-0.1.1/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       85 2023-01-05 17:24:07.000000 senepy-0.1.1/README.md
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      734 2023-01-09 21:15:25.000000 senepy-0.1.1/pyproject.toml
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-01-09 21:17:31.000000 senepy-0.1.1/senepy/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       75 2023-01-03 23:45:29.000000 senepy-0.1.1/senepy/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-01-09 21:17:31.000000 senepy-0.1.1/senepy/data/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)   247439 2023-01-03 19:55:02.000000 senepy-0.1.1/senepy/data/5_TMS_HUBS_DICTIONARY_FILTERED.pickle
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4377 2023-01-03 19:55:02.000000 senepy-0.1.1/senepy/data/5_TMS_HUBS_METADATA_FILTERED.pickle
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)   251065 2023-01-03 19:55:03.000000 senepy-0.1.1/senepy/data/5_TMS_SIGS_DICTIONARY_FILTERED.pickle
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3005 2023-01-03 19:55:03.000000 senepy-0.1.1/senepy/data/5_TMS_SIGS_METADATA_FILTERED.pickle
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)   451173 2023-01-03 19:55:04.000000 senepy-0.1.1/senepy/data/6_HUMAN_HUBS_DICTIONARY_FILTERED.pickle
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3735 2023-01-03 19:55:04.000000 senepy-0.1.1/senepy/data/6_HUMAN_HUBS_METADATA_FILTERED.pickle
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)   454899 2023-01-03 19:55:05.000000 senepy-0.1.1/senepy/data/6_HUMAN_SIGS_DICTIONARY_FILTERED.pickle
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2815 2023-01-03 19:55:05.000000 senepy-0.1.1/senepy/data/6_HUMAN_SIGS_METADATA_FILTERED.pickle
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000) 61855198 2023-01-03 18:44:12.000000 senepy-0.1.1/senepy/data/mart_export.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3627 2023-01-04 16:59:37.000000 senepy-0.1.1/senepy/load_hubs.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8318 2023-01-09 21:15:02.000000 senepy-0.1.1/senepy/score_hub.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4049 2023-01-04 20:20:55.000000 senepy-0.1.1/senepy/translator.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-01-09 21:17:31.000000 senepy-0.1.1/senepy.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      619 2023-01-09 21:17:29.000000 senepy-0.1.1/senepy.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      689 2023-01-09 21:17:30.000000 senepy-0.1.1/senepy.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-01-09 21:17:29.000000 senepy-0.1.1/senepy.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       26 2023-01-09 21:17:29.000000 senepy-0.1.1/senepy.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        7 2023-01-09 21:17:29.000000 senepy-0.1.1/senepy.egg-info/top_level.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-01-09 21:17:48.000000 senepy-0.1.1/setup.cfg
+drwxrwxr-x   0 jrlab     (1000) jrlab     (1000)        0 2024-05-15 21:57:02.873359 senepy-0.2.0/
+-rw-rw-r--   0 jrlab     (1000) jrlab     (1000)     1073 2023-01-03 20:08:52.000000 senepy-0.2.0/LICENSE
+-rw-r--r--   0 jrlab     (1000) jrlab     (1000)      695 2024-05-15 21:57:02.873359 senepy-0.2.0/PKG-INFO
+-rw-rw-r--   0 jrlab     (1000) jrlab     (1000)       85 2023-01-05 17:24:08.000000 senepy-0.2.0/README.md
+-rw-rw-r--   0 jrlab     (1000) jrlab     (1000)      742 2024-05-15 21:54:47.000000 senepy-0.2.0/pyproject.toml
+drwxrwxr-x   0 jrlab     (1000) jrlab     (1000)        0 2024-05-15 21:57:02.797357 senepy-0.2.0/senepy/
+-rw-rw-r--   0 jrlab     (1000) jrlab     (1000)       75 2023-01-03 23:45:30.000000 senepy-0.2.0/senepy/__init__.py
+drwxrwxr-x   0 jrlab     (1000) jrlab     (1000)        0 2024-05-15 21:57:02.873359 senepy-0.2.0/senepy/data/
+-rw-rw-r--   0 jrlab     (1000) jrlab     (1000)   247439 2023-01-03 19:55:03.000000 senepy-0.2.0/senepy/data/5_TMS_HUBS_DICTIONARY_FILTERED.pickle
+-rw-rw-r--   0 jrlab     (1000) jrlab     (1000)     4377 2023-01-03 19:55:03.000000 senepy-0.2.0/senepy/data/5_TMS_HUBS_METADATA_FILTERED.pickle
+-rw-rw-r--   0 jrlab     (1000) jrlab     (1000)   251065 2023-01-03 19:55:04.000000 senepy-0.2.0/senepy/data/5_TMS_SIGS_DICTIONARY_FILTERED.pickle
+-rw-rw-r--   0 jrlab     (1000) jrlab     (1000)     3005 2023-01-03 19:55:04.000000 senepy-0.2.0/senepy/data/5_TMS_SIGS_METADATA_FILTERED.pickle
+-rw-rw-r--   0 jrlab     (1000) jrlab     (1000)   451173 2023-01-03 19:55:05.000000 senepy-0.2.0/senepy/data/6_HUMAN_HUBS_DICTIONARY_FILTERED.pickle
+-rw-rw-r--   0 jrlab     (1000) jrlab     (1000)     3735 2023-01-03 19:55:05.000000 senepy-0.2.0/senepy/data/6_HUMAN_HUBS_METADATA_FILTERED.pickle
+-rw-rw-r--   0 jrlab     (1000) jrlab     (1000)   454899 2023-01-03 19:55:06.000000 senepy-0.2.0/senepy/data/6_HUMAN_SIGS_DICTIONARY_FILTERED.pickle
+-rw-rw-r--   0 jrlab     (1000) jrlab     (1000)     2815 2023-01-03 19:55:06.000000 senepy-0.2.0/senepy/data/6_HUMAN_SIGS_METADATA_FILTERED.pickle
+-rw-rw-r--   0 jrlab     (1000) jrlab     (1000)     3936 2024-05-14 20:15:32.000000 senepy-0.2.0/senepy/data/Human_literature_markers.pickle
+-rw-rw-r--   0 jrlab     (1000) jrlab     (1000)     3982 2024-05-14 20:02:40.000000 senepy-0.2.0/senepy/data/Mouse_literature_markers.pickle
+-rw-rw-r--   0 jrlab     (1000) jrlab     (1000) 61855198 2023-01-03 18:44:13.000000 senepy-0.2.0/senepy/data/mart_export.txt
+-rw-rw-r--   0 jrlab     (1000) jrlab     (1000)      566 2023-04-10 02:01:32.000000 senepy-0.2.0/senepy/data/senGPT.txt
+-rw-rw-r--   0 jrlab     (1000) jrlab     (1000)    10546 2024-05-15 21:38:21.000000 senepy-0.2.0/senepy/load_hubs.py
+-rw-rw-r--   0 jrlab     (1000) jrlab     (1000)     8318 2023-01-09 21:15:03.000000 senepy-0.2.0/senepy/score_hub.py
+-rw-rw-r--   0 jrlab     (1000) jrlab     (1000)     4049 2023-01-04 20:20:56.000000 senepy-0.2.0/senepy/translator.py
+drwxrwxr-x   0 jrlab     (1000) jrlab     (1000)        0 2024-05-15 21:57:02.873359 senepy-0.2.0/senepy.egg-info/
+-rw-r--r--   0 jrlab     (1000) jrlab     (1000)      695 2024-05-15 21:57:02.000000 senepy-0.2.0/senepy.egg-info/PKG-INFO
+-rw-rw-r--   0 jrlab     (1000) jrlab     (1000)      800 2024-05-15 21:57:02.000000 senepy-0.2.0/senepy.egg-info/SOURCES.txt
+-rw-rw-r--   0 jrlab     (1000) jrlab     (1000)        1 2024-05-15 21:57:02.000000 senepy-0.2.0/senepy.egg-info/dependency_links.txt
+-rw-rw-r--   0 jrlab     (1000) jrlab     (1000)       31 2024-05-15 21:57:02.000000 senepy-0.2.0/senepy.egg-info/requires.txt
+-rw-rw-r--   0 jrlab     (1000) jrlab     (1000)        7 2024-05-15 21:57:02.000000 senepy-0.2.0/senepy.egg-info/top_level.txt
+-rw-rw-r--   0 jrlab     (1000) jrlab     (1000)       38 2024-05-15 21:57:02.873359 senepy-0.2.0/setup.cfg
```

### Comparing `senepy-0.1.1/LICENSE` & `senepy-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `senepy-0.1.1/PKG-INFO` & `senepy-0.2.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 Metadata-Version: 2.1
 Name: senepy
-Version: 0.1.1
+Version: 0.2.0
 Summary: tools to score single-cells based on senescence marker expression
 Author-email: Mark Sanborn <mark.email24@gmail.com>
 Project-URL: Homepage, https://github.com/mousepixels/senepy
 Project-URL: Bug Tracker, https://github.com/mousepixels/senepy
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: pandas>=1.0
+Requires-Dist: numpy>=1.17.0
+Requires-Dist: tqdm
 
 Tools to score single cells based on their expression of senescnece markers.# senepy
```

### Comparing `senepy-0.1.1/pyproject.toml` & `senepy-0.2.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "senepy"
-version = "0.1.1"
+version = "0.2.0"
 authors = [
   { name="Mark Sanborn", email="mark.email24@gmail.com" },
 ]
 description = "tools to score single-cells based on senescence marker expression"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 dependencies = [
-"pandas>=1.0", "numpy>=1.17.0"
+"pandas>=1.0", "numpy>=1.17.0", "tqdm"
 ]
 
 
 [project.urls]
 "Homepage" = "https://github.com/mousepixels/senepy"
 "Bug Tracker" = "https://github.com/mousepixels/senepy"
```

### Comparing `senepy-0.1.1/senepy/data/5_TMS_HUBS_DICTIONARY_FILTERED.pickle` & `senepy-0.2.0/senepy/data/5_TMS_HUBS_DICTIONARY_FILTERED.pickle`

 * *Files identical despite different names*

### Comparing `senepy-0.1.1/senepy/data/5_TMS_HUBS_METADATA_FILTERED.pickle` & `senepy-0.2.0/senepy/data/5_TMS_HUBS_METADATA_FILTERED.pickle`

 * *Files identical despite different names*

### Comparing `senepy-0.1.1/senepy/data/5_TMS_SIGS_DICTIONARY_FILTERED.pickle` & `senepy-0.2.0/senepy/data/5_TMS_SIGS_DICTIONARY_FILTERED.pickle`

 * *Files identical despite different names*

### Comparing `senepy-0.1.1/senepy/data/5_TMS_SIGS_METADATA_FILTERED.pickle` & `senepy-0.2.0/senepy/data/5_TMS_SIGS_METADATA_FILTERED.pickle`

 * *Files identical despite different names*

### Comparing `senepy-0.1.1/senepy/data/6_HUMAN_HUBS_DICTIONARY_FILTERED.pickle` & `senepy-0.2.0/senepy/data/6_HUMAN_HUBS_DICTIONARY_FILTERED.pickle`

 * *Files identical despite different names*

### Comparing `senepy-0.1.1/senepy/data/6_HUMAN_HUBS_METADATA_FILTERED.pickle` & `senepy-0.2.0/senepy/data/6_HUMAN_HUBS_METADATA_FILTERED.pickle`

 * *Files identical despite different names*

### Comparing `senepy-0.1.1/senepy/data/6_HUMAN_SIGS_DICTIONARY_FILTERED.pickle` & `senepy-0.2.0/senepy/data/6_HUMAN_SIGS_DICTIONARY_FILTERED.pickle`

 * *Files identical despite different names*

### Comparing `senepy-0.1.1/senepy/data/6_HUMAN_SIGS_METADATA_FILTERED.pickle` & `senepy-0.2.0/senepy/data/6_HUMAN_SIGS_METADATA_FILTERED.pickle`

 * *Files identical despite different names*

### Comparing `senepy-0.1.1/senepy/data/mart_export.txt` & `senepy-0.2.0/senepy/data/mart_export.txt`

 * *Files identical despite different names*

### Comparing `senepy-0.1.1/senepy/score_hub.py` & `senepy-0.2.0/senepy/score_hub.py`

 * *Files identical despite different names*

### Comparing `senepy-0.1.1/senepy/translator.py` & `senepy-0.2.0/senepy/translator.py`

 * *Files identical despite different names*

### Comparing `senepy-0.1.1/senepy.egg-info/PKG-INFO` & `senepy-0.2.0/senepy.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 Metadata-Version: 2.1
 Name: senepy
-Version: 0.1.1
+Version: 0.2.0
 Summary: tools to score single-cells based on senescence marker expression
 Author-email: Mark Sanborn <mark.email24@gmail.com>
 Project-URL: Homepage, https://github.com/mousepixels/senepy
 Project-URL: Bug Tracker, https://github.com/mousepixels/senepy
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: pandas>=1.0
+Requires-Dist: numpy>=1.17.0
+Requires-Dist: tqdm
 
 Tools to score single cells based on their expression of senescnece markers.# senepy
```

### Comparing `senepy-0.1.1/senepy.egg-info/SOURCES.txt` & `senepy-0.2.0/senepy.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -14,8 +14,11 @@
 senepy/data/5_TMS_HUBS_METADATA_FILTERED.pickle
 senepy/data/5_TMS_SIGS_DICTIONARY_FILTERED.pickle
 senepy/data/5_TMS_SIGS_METADATA_FILTERED.pickle
 senepy/data/6_HUMAN_HUBS_DICTIONARY_FILTERED.pickle
 senepy/data/6_HUMAN_HUBS_METADATA_FILTERED.pickle
 senepy/data/6_HUMAN_SIGS_DICTIONARY_FILTERED.pickle
 senepy/data/6_HUMAN_SIGS_METADATA_FILTERED.pickle
-senepy/data/mart_export.txt
+senepy/data/Human_literature_markers.pickle
+senepy/data/Mouse_literature_markers.pickle
+senepy/data/mart_export.txt
+senepy/data/senGPT.txt
```

