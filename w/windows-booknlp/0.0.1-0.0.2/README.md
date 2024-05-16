# Comparing `tmp/windows_booknlp-0.0.1.tar.gz` & `tmp/windows_booknlp-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "windows_booknlp-0.0.1.tar", last modified: Wed May 15 16:21:05 2024, max compression
+gzip compressed data, was "windows_booknlp-0.0.2.tar", last modified: Wed May 15 16:43:25 2024, max compression
```

## Comparing `windows_booknlp-0.0.1.tar` & `windows_booknlp-0.0.2.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 test       (507) staff       (20)        0 2024-05-15 16:21:05.386297 windows_booknlp-0.0.1/
--rw-r--r--   0 test       (507) staff       (20)       30 2021-11-05 23:50:08.000000 windows_booknlp-0.0.1/MANIFEST.in
--rw-r--r--   0 test       (507) staff       (20)    13290 2024-05-15 16:21:05.385912 windows_booknlp-0.0.1/PKG-INFO
--rw-r--r--   0 test       (507) staff       (20)    12943 2024-05-15 16:12:08.000000 windows_booknlp-0.0.1/README.md
-drwxr-xr-x   0 test       (507) staff       (20)        0 2024-05-15 16:21:05.331672 windows_booknlp-0.0.1/booknlp/
--rw-r--r--   0 test       (507) staff       (20)        0 2024-05-15 15:40:03.000000 windows_booknlp-0.0.1/booknlp/__init__.py
--rw-r--r--   0 test       (507) staff       (20)     1407 2024-05-15 15:40:03.000000 windows_booknlp-0.0.1/booknlp/booknlp.py
-drwxr-xr-x   0 test       (507) staff       (20)        0 2024-05-15 16:21:05.338770 windows_booknlp-0.0.1/booknlp/common/
--rw-r--r--   0 test       (507) staff       (20)        0 2024-05-15 15:40:03.000000 windows_booknlp-0.0.1/booknlp/common/__init__.py
--rw-r--r--   0 test       (507) staff       (20)     1295 2024-05-15 15:40:03.000000 windows_booknlp-0.0.1/booknlp/common/b3.py
--rw-r--r--   0 test       (507) staff       (20)     1191 2024-05-15 15:40:03.000000 windows_booknlp-0.0.1/booknlp/common/calc_coref_metrics.py
--rw-r--r--   0 test       (507) staff       (20)     5585 2024-05-15 15:40:03.000000 windows_booknlp-0.0.1/booknlp/common/crf.py
--rw-r--r--   0 test       (507) staff       (20)    11082 2024-05-15 15:40:03.000000 windows_booknlp-0.0.1/booknlp/common/layered_reader.py
--rw-r--r--   0 test       (507) staff       (20)     4909 2024-05-15 15:40:03.000000 windows_booknlp-0.0.1/booknlp/common/pipelines.py
--rw-r--r--   0 test       (507) staff       (20)     4401 2024-05-15 15:40:03.000000 windows_booknlp-0.0.1/booknlp/common/sequence_eval.py
--rw-r--r--   0 test       (507) staff       (20)     3725 2024-05-15 15:40:03.000000 windows_booknlp-0.0.1/booknlp/common/sequence_layered_reader.py
-drwxr-xr-x   0 test       (507) staff       (20)        0 2024-05-15 16:21:05.351303 windows_booknlp-0.0.1/booknlp/english/
--rw-r--r--   0 test       (507) staff       (20)        0 2024-05-15 15:40:03.000000 windows_booknlp-0.0.1/booknlp/english/__init__.py
--rw-r--r--   0 test       (507) staff       (20)    31039 2024-05-15 15:40:03.000000 windows_booknlp-0.0.1/booknlp/english/bert_coref_quote_pronouns.py
--rw-r--r--   0 test       (507) staff       (20)     9366 2024-05-15 15:40:03.000000 windows_booknlp-0.0.1/booknlp/english/bert_qa.py
-drwxr-xr-x   0 test       (507) staff       (20)        0 2024-05-15 16:21:05.371943 windows_booknlp-0.0.1/booknlp/english/data/
--rw-r--r--   0 test       (507) staff       (20)        0 2024-05-15 15:40:03.000000 windows_booknlp-0.0.1/booknlp/english/data/__init__.py
--rw-r--r--   0 test       (507) staff       (20)    20043 2024-05-15 15:40:03.000000 windows_booknlp-0.0.1/booknlp/english/data/aliases.txt
--rw-r--r--   0 test       (507) staff       (20)      487 2024-05-15 15:40:03.000000 windows_booknlp-0.0.1/booknlp/english/data/entity_cat.tagset
--rw-r--r--   0 test       (507) staff       (20)  5870690 2024-05-15 15:40:03.000000 windows_booknlp-0.0.1/booknlp/english/data/gutenberg_prop_gender_terms.txt
--rw-r--r--   0 test       (507) staff       (20)     1488 2024-05-15 15:40:03.000000 windows_booknlp-0.0.1/booknlp/english/data/supersense.tagset
--rw-r--r--   0 test       (507) staff       (20)  2343705 2024-05-15 15:40:03.000000 windows_booknlp-0.0.1/booknlp/english/data/wordnet.first.sense
--rw-r--r--   0 test       (507) staff       (20)    20251 2024-05-15 15:40:03.000000 windows_booknlp-0.0.1/booknlp/english/english_booknlp.py
--rw-r--r--   0 test       (507) staff       (20)     5861 2024-05-15 15:40:03.000000 windows_booknlp-0.0.1/booknlp/english/entity_tagger.py
--rw-r--r--   0 test       (507) staff       (20)    15831 2024-05-15 15:40:03.000000 windows_booknlp-0.0.1/booknlp/english/gender_inference_model_1.py
--rw-r--r--   0 test       (507) staff       (20)     4888 2024-05-15 15:40:03.000000 windows_booknlp-0.0.1/booknlp/english/litbank_coref.py
--rw-r--r--   0 test       (507) staff       (20)     1662 2024-05-15 15:40:03.000000 windows_booknlp-0.0.1/booknlp/english/litbank_quote.py
--rw-r--r--   0 test       (507) staff       (20)    11681 2024-05-15 15:40:03.000000 windows_booknlp-0.0.1/booknlp/english/name_coref.py
--rw-r--r--   0 test       (507) staff       (20)     6550 2024-05-15 15:40:03.000000 windows_booknlp-0.0.1/booknlp/english/speaker_attribution.py
--rw-r--r--   0 test       (507) staff       (20)    33737 2024-05-15 15:40:03.000000 windows_booknlp-0.0.1/booknlp/english/tagger.py
--rw-r--r--   0 test       (507) staff       (20)       38 2024-05-15 16:21:05.387231 windows_booknlp-0.0.1/setup.cfg
--rw-r--r--   0 test       (507) staff       (20)      727 2024-05-15 16:20:58.000000 windows_booknlp-0.0.1/setup.py
-drwxr-xr-x   0 test       (507) staff       (20)        0 2024-05-15 16:21:05.384483 windows_booknlp-0.0.1/windows_booknlp.egg-info/
--rw-r--r--   0 test       (507) staff       (20)    13290 2024-05-15 16:21:05.000000 windows_booknlp-0.0.1/windows_booknlp.egg-info/PKG-INFO
--rw-r--r--   0 test       (507) staff       (20)     1126 2024-05-15 16:21:05.000000 windows_booknlp-0.0.1/windows_booknlp.egg-info/SOURCES.txt
--rw-r--r--   0 test       (507) staff       (20)        1 2024-05-15 16:21:05.000000 windows_booknlp-0.0.1/windows_booknlp.egg-info/dependency_links.txt
--rw-r--r--   0 test       (507) staff       (20)       52 2024-05-15 16:21:05.000000 windows_booknlp-0.0.1/windows_booknlp.egg-info/requires.txt
--rw-r--r--   0 test       (507) staff       (20)        8 2024-05-15 16:21:05.000000 windows_booknlp-0.0.1/windows_booknlp.egg-info/top_level.txt
+drwxr-xr-x   0 test       (507) staff       (20)        0 2024-05-15 16:43:25.610609 windows_booknlp-0.0.2/
+-rw-r--r--   0 test       (507) staff       (20)       30 2021-11-05 23:50:08.000000 windows_booknlp-0.0.2/MANIFEST.in
+-rw-r--r--   0 test       (507) staff       (20)    13291 2024-05-15 16:43:25.610146 windows_booknlp-0.0.2/PKG-INFO
+-rw-r--r--   0 test       (507) staff       (20)    12944 2024-05-15 16:40:42.000000 windows_booknlp-0.0.2/README.md
+drwxr-xr-x   0 test       (507) staff       (20)        0 2024-05-15 16:43:25.567329 windows_booknlp-0.0.2/booknlp/
+-rw-r--r--   0 test       (507) staff       (20)        0 2024-05-15 15:40:03.000000 windows_booknlp-0.0.2/booknlp/__init__.py
+-rw-r--r--   0 test       (507) staff       (20)     1407 2024-05-15 15:40:03.000000 windows_booknlp-0.0.2/booknlp/booknlp.py
+drwxr-xr-x   0 test       (507) staff       (20)        0 2024-05-15 16:43:25.571686 windows_booknlp-0.0.2/booknlp/common/
+-rw-r--r--   0 test       (507) staff       (20)        0 2024-05-15 15:40:03.000000 windows_booknlp-0.0.2/booknlp/common/__init__.py
+-rw-r--r--   0 test       (507) staff       (20)     1295 2024-05-15 15:40:03.000000 windows_booknlp-0.0.2/booknlp/common/b3.py
+-rw-r--r--   0 test       (507) staff       (20)     1191 2024-05-15 15:40:03.000000 windows_booknlp-0.0.2/booknlp/common/calc_coref_metrics.py
+-rw-r--r--   0 test       (507) staff       (20)     5585 2024-05-15 15:40:03.000000 windows_booknlp-0.0.2/booknlp/common/crf.py
+-rw-r--r--   0 test       (507) staff       (20)    11082 2024-05-15 15:40:03.000000 windows_booknlp-0.0.2/booknlp/common/layered_reader.py
+-rw-r--r--   0 test       (507) staff       (20)     4909 2024-05-15 15:40:03.000000 windows_booknlp-0.0.2/booknlp/common/pipelines.py
+-rw-r--r--   0 test       (507) staff       (20)     4401 2024-05-15 15:40:03.000000 windows_booknlp-0.0.2/booknlp/common/sequence_eval.py
+-rw-r--r--   0 test       (507) staff       (20)     3725 2024-05-15 15:40:03.000000 windows_booknlp-0.0.2/booknlp/common/sequence_layered_reader.py
+drwxr-xr-x   0 test       (507) staff       (20)        0 2024-05-15 16:43:25.580786 windows_booknlp-0.0.2/booknlp/english/
+-rw-r--r--   0 test       (507) staff       (20)        0 2024-05-15 15:40:03.000000 windows_booknlp-0.0.2/booknlp/english/__init__.py
+-rw-r--r--   0 test       (507) staff       (20)    31039 2024-05-15 15:40:03.000000 windows_booknlp-0.0.2/booknlp/english/bert_coref_quote_pronouns.py
+-rw-r--r--   0 test       (507) staff       (20)     9366 2024-05-15 15:40:03.000000 windows_booknlp-0.0.2/booknlp/english/bert_qa.py
+drwxr-xr-x   0 test       (507) staff       (20)        0 2024-05-15 16:43:25.597795 windows_booknlp-0.0.2/booknlp/english/data/
+-rw-r--r--   0 test       (507) staff       (20)        0 2024-05-15 15:40:03.000000 windows_booknlp-0.0.2/booknlp/english/data/__init__.py
+-rw-r--r--   0 test       (507) staff       (20)    20043 2024-05-15 15:40:03.000000 windows_booknlp-0.0.2/booknlp/english/data/aliases.txt
+-rw-r--r--   0 test       (507) staff       (20)      487 2024-05-15 15:40:03.000000 windows_booknlp-0.0.2/booknlp/english/data/entity_cat.tagset
+-rw-r--r--   0 test       (507) staff       (20)  5870690 2024-05-15 15:40:03.000000 windows_booknlp-0.0.2/booknlp/english/data/gutenberg_prop_gender_terms.txt
+-rw-r--r--   0 test       (507) staff       (20)     1488 2024-05-15 15:40:03.000000 windows_booknlp-0.0.2/booknlp/english/data/supersense.tagset
+-rw-r--r--   0 test       (507) staff       (20)  2343705 2024-05-15 15:40:03.000000 windows_booknlp-0.0.2/booknlp/english/data/wordnet.first.sense
+-rw-r--r--   0 test       (507) staff       (20)    20251 2024-05-15 15:40:03.000000 windows_booknlp-0.0.2/booknlp/english/english_booknlp.py
+-rw-r--r--   0 test       (507) staff       (20)     5861 2024-05-15 15:40:03.000000 windows_booknlp-0.0.2/booknlp/english/entity_tagger.py
+-rw-r--r--   0 test       (507) staff       (20)    15831 2024-05-15 15:40:03.000000 windows_booknlp-0.0.2/booknlp/english/gender_inference_model_1.py
+-rw-r--r--   0 test       (507) staff       (20)     4888 2024-05-15 15:40:03.000000 windows_booknlp-0.0.2/booknlp/english/litbank_coref.py
+-rw-r--r--   0 test       (507) staff       (20)     1662 2024-05-15 15:40:03.000000 windows_booknlp-0.0.2/booknlp/english/litbank_quote.py
+-rw-r--r--   0 test       (507) staff       (20)    11681 2024-05-15 15:40:03.000000 windows_booknlp-0.0.2/booknlp/english/name_coref.py
+-rw-r--r--   0 test       (507) staff       (20)     6550 2024-05-15 15:40:03.000000 windows_booknlp-0.0.2/booknlp/english/speaker_attribution.py
+-rw-r--r--   0 test       (507) staff       (20)    33737 2024-05-15 15:40:03.000000 windows_booknlp-0.0.2/booknlp/english/tagger.py
+-rw-r--r--   0 test       (507) staff       (20)       38 2024-05-15 16:43:25.611448 windows_booknlp-0.0.2/setup.cfg
+-rw-r--r--   0 test       (507) staff       (20)      727 2024-05-15 16:42:50.000000 windows_booknlp-0.0.2/setup.py
+drwxr-xr-x   0 test       (507) staff       (20)        0 2024-05-15 16:43:25.608862 windows_booknlp-0.0.2/windows_booknlp.egg-info/
+-rw-r--r--   0 test       (507) staff       (20)    13291 2024-05-15 16:43:25.000000 windows_booknlp-0.0.2/windows_booknlp.egg-info/PKG-INFO
+-rw-r--r--   0 test       (507) staff       (20)     1126 2024-05-15 16:43:25.000000 windows_booknlp-0.0.2/windows_booknlp.egg-info/SOURCES.txt
+-rw-r--r--   0 test       (507) staff       (20)        1 2024-05-15 16:43:25.000000 windows_booknlp-0.0.2/windows_booknlp.egg-info/dependency_links.txt
+-rw-r--r--   0 test       (507) staff       (20)       52 2024-05-15 16:43:25.000000 windows_booknlp-0.0.2/windows_booknlp.egg-info/requires.txt
+-rw-r--r--   0 test       (507) staff       (20)        8 2024-05-15 16:43:25.000000 windows_booknlp-0.0.2/windows_booknlp.egg-info/top_level.txt
```

### Comparing `windows_booknlp-0.0.1/PKG-INFO` & `windows_booknlp-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: windows_booknlp
-Version: 0.0.1
+Version: 0.0.2
 Home-page: https://github.com/DrewThomasson/booknlp
 Author: David Bamman and Andrew Phillip Thomasson
 Author-email: dbamman@berkeley.edu
 License: MIT
 Description-Content-Type: text/markdown
 Requires-Dist: torch>=1.7.1
 Requires-Dist: spacy>=3
 Requires-Dist: transformers<=4.30.0,>=4.11.3
 
-# This is a modifed Booknlp to make it work on windows nativly 
+# This is a modifed Booknlp to make it work on windows natively 
 -Modifed by Drew Thomasson
 -https://github.com/DrewThomasson/booknlp
 # BookNLP
 
 BookNLP is a natural language processing pipeline that scales to books and other long documents (in English), including:
 
 * Part-of-speech tagging
```

### Comparing `windows_booknlp-0.0.1/README.md` & `windows_booknlp-0.0.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This is a modifed Booknlp to make it work on windows nativly 
+# This is a modifed Booknlp to make it work on windows natively 
 -Modifed by Drew Thomasson
 -https://github.com/DrewThomasson/booknlp
 # BookNLP
 
 BookNLP is a natural language processing pipeline that scales to books and other long documents (in English), including:
 
 * Part-of-speech tagging
```

### Comparing `windows_booknlp-0.0.1/booknlp/booknlp.py` & `windows_booknlp-0.0.2/booknlp/booknlp.py`

 * *Files identical despite different names*

### Comparing `windows_booknlp-0.0.1/booknlp/common/b3.py` & `windows_booknlp-0.0.2/booknlp/common/b3.py`

 * *Files identical despite different names*

### Comparing `windows_booknlp-0.0.1/booknlp/common/calc_coref_metrics.py` & `windows_booknlp-0.0.2/booknlp/common/calc_coref_metrics.py`

 * *Files identical despite different names*

### Comparing `windows_booknlp-0.0.1/booknlp/common/crf.py` & `windows_booknlp-0.0.2/booknlp/common/crf.py`

 * *Files identical despite different names*

### Comparing `windows_booknlp-0.0.1/booknlp/common/layered_reader.py` & `windows_booknlp-0.0.2/booknlp/common/layered_reader.py`

 * *Files identical despite different names*

### Comparing `windows_booknlp-0.0.1/booknlp/common/pipelines.py` & `windows_booknlp-0.0.2/booknlp/common/pipelines.py`

 * *Files identical despite different names*

### Comparing `windows_booknlp-0.0.1/booknlp/common/sequence_eval.py` & `windows_booknlp-0.0.2/booknlp/common/sequence_eval.py`

 * *Files identical despite different names*

### Comparing `windows_booknlp-0.0.1/booknlp/common/sequence_layered_reader.py` & `windows_booknlp-0.0.2/booknlp/common/sequence_layered_reader.py`

 * *Files identical despite different names*

### Comparing `windows_booknlp-0.0.1/booknlp/english/bert_coref_quote_pronouns.py` & `windows_booknlp-0.0.2/booknlp/english/bert_coref_quote_pronouns.py`

 * *Files identical despite different names*

### Comparing `windows_booknlp-0.0.1/booknlp/english/bert_qa.py` & `windows_booknlp-0.0.2/booknlp/english/bert_qa.py`

 * *Files identical despite different names*

### Comparing `windows_booknlp-0.0.1/booknlp/english/data/aliases.txt` & `windows_booknlp-0.0.2/booknlp/english/data/aliases.txt`

 * *Files identical despite different names*

### Comparing `windows_booknlp-0.0.1/booknlp/english/data/gutenberg_prop_gender_terms.txt` & `windows_booknlp-0.0.2/booknlp/english/data/gutenberg_prop_gender_terms.txt`

 * *Files identical despite different names*

### Comparing `windows_booknlp-0.0.1/booknlp/english/data/supersense.tagset` & `windows_booknlp-0.0.2/booknlp/english/data/supersense.tagset`

 * *Files identical despite different names*

### Comparing `windows_booknlp-0.0.1/booknlp/english/data/wordnet.first.sense` & `windows_booknlp-0.0.2/booknlp/english/data/wordnet.first.sense`

 * *Files identical despite different names*

### Comparing `windows_booknlp-0.0.1/booknlp/english/english_booknlp.py` & `windows_booknlp-0.0.2/booknlp/english/english_booknlp.py`

 * *Files identical despite different names*

### Comparing `windows_booknlp-0.0.1/booknlp/english/entity_tagger.py` & `windows_booknlp-0.0.2/booknlp/english/entity_tagger.py`

 * *Files identical despite different names*

### Comparing `windows_booknlp-0.0.1/booknlp/english/gender_inference_model_1.py` & `windows_booknlp-0.0.2/booknlp/english/gender_inference_model_1.py`

 * *Files identical despite different names*

### Comparing `windows_booknlp-0.0.1/booknlp/english/litbank_coref.py` & `windows_booknlp-0.0.2/booknlp/english/litbank_coref.py`

 * *Files identical despite different names*

### Comparing `windows_booknlp-0.0.1/booknlp/english/litbank_quote.py` & `windows_booknlp-0.0.2/booknlp/english/litbank_quote.py`

 * *Files identical despite different names*

### Comparing `windows_booknlp-0.0.1/booknlp/english/name_coref.py` & `windows_booknlp-0.0.2/booknlp/english/name_coref.py`

 * *Files identical despite different names*

### Comparing `windows_booknlp-0.0.1/booknlp/english/speaker_attribution.py` & `windows_booknlp-0.0.2/booknlp/english/speaker_attribution.py`

 * *Files identical despite different names*

### Comparing `windows_booknlp-0.0.1/booknlp/english/tagger.py` & `windows_booknlp-0.0.2/booknlp/english/tagger.py`

 * *Files identical despite different names*

### Comparing `windows_booknlp-0.0.1/setup.py` & `windows_booknlp-0.0.2/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='windows_booknlp',
-    version='0.0.1', 
+    version='0.0.2', 
     packages=find_packages(),
     py_modules=['booknlp'],
     url="https://github.com/DrewThomasson/booknlp",
     author="David Bamman and Andrew Phillip Thomasson",
     author_email="dbamman@berkeley.edu",
     include_package_data=True, 
     license="MIT",
```

### Comparing `windows_booknlp-0.0.1/windows_booknlp.egg-info/PKG-INFO` & `windows_booknlp-0.0.2/windows_booknlp.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: windows-booknlp
-Version: 0.0.1
+Version: 0.0.2
 Home-page: https://github.com/DrewThomasson/booknlp
 Author: David Bamman and Andrew Phillip Thomasson
 Author-email: dbamman@berkeley.edu
 License: MIT
 Description-Content-Type: text/markdown
 Requires-Dist: torch>=1.7.1
 Requires-Dist: spacy>=3
 Requires-Dist: transformers<=4.30.0,>=4.11.3
 
-# This is a modifed Booknlp to make it work on windows nativly 
+# This is a modifed Booknlp to make it work on windows natively 
 -Modifed by Drew Thomasson
 -https://github.com/DrewThomasson/booknlp
 # BookNLP
 
 BookNLP is a natural language processing pipeline that scales to books and other long documents (in English), including:
 
 * Part-of-speech tagging
```

### Comparing `windows_booknlp-0.0.1/windows_booknlp.egg-info/SOURCES.txt` & `windows_booknlp-0.0.2/windows_booknlp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

