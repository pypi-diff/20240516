# Comparing `tmp/saf_datasets-0.6.5.tar.gz` & `tmp/saf_datasets-0.6.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "saf_datasets-0.6.5.tar", last modified: Wed May 15 07:41:38 2024, max compression
+gzip compressed data, was "saf_datasets-0.6.6.tar", last modified: Thu May 16 16:30:03 2024, max compression
```

## Comparing `saf_datasets-0.6.5.tar` & `saf_datasets-0.6.6.tar`

### file list

```diff
@@ -1,36 +1,37 @@
-drwxr-xr-x   0 dsilvadecarvalho   (505) staff       (20)        0 2024-05-15 07:41:38.005500 saf_datasets-0.6.5/
--rw-------   0 dsilvadecarvalho   (505) staff       (20)    35149 2023-03-15 12:32:16.000000 saf_datasets-0.6.5/LICENSE
--rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)     4322 2024-05-15 07:41:38.005228 saf_datasets-0.6.5/PKG-INFO
--rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)     3491 2024-05-08 18:45:21.000000 saf_datasets-0.6.5/README.md
--rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)      671 2024-05-15 07:41:21.000000 saf_datasets-0.6.5/pyproject.toml
--rw-------   0 dsilvadecarvalho   (505) staff       (20)       77 2024-05-08 14:09:52.000000 saf_datasets-0.6.5/requirements.txt
-drwxr-xr-x   0 dsilvadecarvalho   (505) staff       (20)        0 2024-05-15 07:41:37.996215 saf_datasets-0.6.5/saf_datasets/
--rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)      366 2024-05-09 14:03:38.000000 saf_datasets-0.6.5/saf_datasets/__init__.py
-drwxr-xr-x   0 dsilvadecarvalho   (505) staff       (20)        0 2024-05-15 07:41:38.000083 saf_datasets-0.6.5/saf_datasets/annotators/
--rw-------   0 dsilvadecarvalho   (505) staff       (20)       80 2024-04-22 11:09:48.000000 saf_datasets-0.6.5/saf_datasets/annotators/__init__.py
--rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)     1325 2024-05-14 14:26:13.000000 saf_datasets-0.6.5/saf_datasets/annotators/allennlp_srl.py
--rw-------   0 dsilvadecarvalho   (505) staff       (20)      165 2023-11-29 15:12:10.000000 saf_datasets-0.6.5/saf_datasets/annotators/models.py
--rw-------   0 dsilvadecarvalho   (505) staff       (20)     1088 2024-05-08 16:03:49.000000 saf_datasets-0.6.5/saf_datasets/annotators/spacy.py
--rw-------   0 dsilvadecarvalho   (505) staff       (20)     4882 2024-05-10 08:55:47.000000 saf_datasets-0.6.5/saf_datasets/annotators/transformer.py
-drwxr-xr-x   0 dsilvadecarvalho   (505) staff       (20)        0 2024-05-15 07:41:38.003523 saf_datasets-0.6.5/saf_datasets/data_access/
--rw-------   0 dsilvadecarvalho   (505) staff       (20)        0 2023-03-13 13:13:57.000000 saf_datasets-0.6.5/saf_datasets/data_access/__init__.py
--rw-------   0 dsilvadecarvalho   (505) staff       (20)     1941 2024-05-08 15:54:57.000000 saf_datasets-0.6.5/saf_datasets/data_access/allnli.py
--rw-------   0 dsilvadecarvalho   (505) staff       (20)     5375 2024-05-08 15:28:33.000000 saf_datasets-0.6.5/saf_datasets/data_access/codwoe.py
--rw-------   0 dsilvadecarvalho   (505) staff       (20)     1907 2024-05-08 15:32:04.000000 saf_datasets-0.6.5/saf_datasets/data_access/cpae.py
--rw-------   0 dsilvadecarvalho   (505) staff       (20)    12727 2024-05-08 14:56:10.000000 saf_datasets-0.6.5/saf_datasets/data_access/dataset.py
--rw-------   0 dsilvadecarvalho   (505) staff       (20)     3962 2024-05-15 07:35:09.000000 saf_datasets-0.6.5/saf_datasets/data_access/entailmentbank.py
--rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)     2608 2024-05-08 17:18:08.000000 saf_datasets-0.6.5/saf_datasets/data_access/stsb.py
--rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)     8835 2024-05-15 07:37:13.000000 saf_datasets-0.6.5/saf_datasets/data_access/wiktionary.py
--rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)     4089 2024-05-15 07:37:13.000000 saf_datasets-0.6.5/saf_datasets/data_access/wordnet_filtered.py
-drwxr-xr-x   0 dsilvadecarvalho   (505) staff       (20)        0 2024-05-15 07:41:38.004456 saf_datasets-0.6.5/saf_datasets/wrappers/
--rw-------   0 dsilvadecarvalho   (505) staff       (20)        0 2023-11-13 14:11:53.000000 saf_datasets-0.6.5/saf_datasets/wrappers/__init__.py
--rw-------   0 dsilvadecarvalho   (505) staff       (20)      793 2024-05-08 15:45:05.000000 saf_datasets-0.6.5/saf_datasets/wrappers/hf.py
--rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)     2062 2024-05-08 15:51:39.000000 saf_datasets-0.6.5/saf_datasets/wrappers/torch.py
-drwxr-xr-x   0 dsilvadecarvalho   (505) staff       (20)        0 2024-05-15 07:41:38.004935 saf_datasets-0.6.5/saf_datasets.egg-info/
--rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)     4322 2024-05-15 07:41:37.000000 saf_datasets-0.6.5/saf_datasets.egg-info/PKG-INFO
--rw-------   0 dsilvadecarvalho   (505) staff       (20)      873 2024-05-15 07:41:37.000000 saf_datasets-0.6.5/saf_datasets.egg-info/SOURCES.txt
--rw-------   0 dsilvadecarvalho   (505) staff       (20)        1 2024-05-15 07:41:37.000000 saf_datasets-0.6.5/saf_datasets.egg-info/dependency_links.txt
--rw-------   0 dsilvadecarvalho   (505) staff       (20)       77 2024-05-15 07:41:37.000000 saf_datasets-0.6.5/saf_datasets.egg-info/requires.txt
--rw-------   0 dsilvadecarvalho   (505) staff       (20)       13 2024-05-15 07:41:37.000000 saf_datasets-0.6.5/saf_datasets.egg-info/top_level.txt
--rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)       38 2024-05-15 07:41:38.005562 saf_datasets-0.6.5/setup.cfg
--rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)      815 2024-05-15 07:41:27.000000 saf_datasets-0.6.5/setup.py
+drwxr-xr-x   0 dsilvadecarvalho   (505) staff       (20)        0 2024-05-16 16:30:03.536949 saf_datasets-0.6.6/
+-rw-------   0 dsilvadecarvalho   (505) staff       (20)    35149 2023-03-15 12:32:16.000000 saf_datasets-0.6.6/LICENSE
+-rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)     4322 2024-05-16 16:30:03.536748 saf_datasets-0.6.6/PKG-INFO
+-rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)     3491 2024-05-08 18:45:21.000000 saf_datasets-0.6.6/README.md
+-rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)      671 2024-05-16 16:28:22.000000 saf_datasets-0.6.6/pyproject.toml
+-rw-------   0 dsilvadecarvalho   (505) staff       (20)       77 2024-05-08 14:09:52.000000 saf_datasets-0.6.6/requirements.txt
+drwxr-xr-x   0 dsilvadecarvalho   (505) staff       (20)        0 2024-05-16 16:30:03.527062 saf_datasets-0.6.6/saf_datasets/
+-rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)       27 2024-05-16 16:27:52.000000 saf_datasets-0.6.6/saf_datasets/__init__.py
+drwxr-xr-x   0 dsilvadecarvalho   (505) staff       (20)        0 2024-05-16 16:30:03.530720 saf_datasets-0.6.6/saf_datasets/annotators/
+-rw-------   0 dsilvadecarvalho   (505) staff       (20)       80 2024-04-22 11:09:48.000000 saf_datasets-0.6.6/saf_datasets/annotators/__init__.py
+-rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)     1325 2024-05-16 16:27:17.000000 saf_datasets-0.6.6/saf_datasets/annotators/allennlp_srl.py
+-rw-------   0 dsilvadecarvalho   (505) staff       (20)      165 2023-11-29 15:12:10.000000 saf_datasets-0.6.6/saf_datasets/annotators/models.py
+-rw-------   0 dsilvadecarvalho   (505) staff       (20)     1088 2024-05-08 16:03:49.000000 saf_datasets-0.6.6/saf_datasets/annotators/spacy.py
+-rw-------   0 dsilvadecarvalho   (505) staff       (20)     4882 2024-05-10 08:55:47.000000 saf_datasets-0.6.6/saf_datasets/annotators/transformer.py
+drwxr-xr-x   0 dsilvadecarvalho   (505) staff       (20)        0 2024-05-16 16:30:03.534760 saf_datasets-0.6.6/saf_datasets/data_access/
+-rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)      341 2024-05-16 16:27:52.000000 saf_datasets-0.6.6/saf_datasets/data_access/__init__.py
+-rw-------   0 dsilvadecarvalho   (505) staff       (20)     1941 2024-05-08 15:54:57.000000 saf_datasets-0.6.6/saf_datasets/data_access/allnli.py
+-rw-------   0 dsilvadecarvalho   (505) staff       (20)     5375 2024-05-08 15:28:33.000000 saf_datasets-0.6.6/saf_datasets/data_access/codwoe.py
+-rw-------   0 dsilvadecarvalho   (505) staff       (20)     1907 2024-05-08 15:32:04.000000 saf_datasets-0.6.6/saf_datasets/data_access/cpae.py
+-rw-------   0 dsilvadecarvalho   (505) staff       (20)    12727 2024-05-08 14:56:10.000000 saf_datasets-0.6.6/saf_datasets/data_access/dataset.py
+-rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)     3962 2024-05-16 16:27:17.000000 saf_datasets-0.6.6/saf_datasets/data_access/entailmentbank.py
+-rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)     2608 2024-05-08 17:18:08.000000 saf_datasets-0.6.6/saf_datasets/data_access/stsb.py
+-rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)     8835 2024-05-16 16:27:17.000000 saf_datasets-0.6.6/saf_datasets/data_access/wiktionary.py
+-rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)     4089 2024-05-16 16:27:52.000000 saf_datasets-0.6.6/saf_datasets/data_access/wordnet_filtered.py
+-rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)     2891 2024-05-16 16:27:52.000000 saf_datasets-0.6.6/saf_datasets/data_access/wordnet_spanish.py
+drwxr-xr-x   0 dsilvadecarvalho   (505) staff       (20)        0 2024-05-16 16:30:03.535906 saf_datasets-0.6.6/saf_datasets/wrappers/
+-rw-------   0 dsilvadecarvalho   (505) staff       (20)        0 2023-11-13 14:11:53.000000 saf_datasets-0.6.6/saf_datasets/wrappers/__init__.py
+-rw-------   0 dsilvadecarvalho   (505) staff       (20)      793 2024-05-08 15:45:05.000000 saf_datasets-0.6.6/saf_datasets/wrappers/hf.py
+-rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)     2062 2024-05-08 15:51:39.000000 saf_datasets-0.6.6/saf_datasets/wrappers/torch.py
+drwxr-xr-x   0 dsilvadecarvalho   (505) staff       (20)        0 2024-05-16 16:30:03.536470 saf_datasets-0.6.6/saf_datasets.egg-info/
+-rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)     4322 2024-05-16 16:30:03.000000 saf_datasets-0.6.6/saf_datasets.egg-info/PKG-INFO
+-rw-------   0 dsilvadecarvalho   (505) staff       (20)      917 2024-05-16 16:30:03.000000 saf_datasets-0.6.6/saf_datasets.egg-info/SOURCES.txt
+-rw-------   0 dsilvadecarvalho   (505) staff       (20)        1 2024-05-16 16:30:03.000000 saf_datasets-0.6.6/saf_datasets.egg-info/dependency_links.txt
+-rw-------   0 dsilvadecarvalho   (505) staff       (20)       77 2024-05-16 16:30:03.000000 saf_datasets-0.6.6/saf_datasets.egg-info/requires.txt
+-rw-------   0 dsilvadecarvalho   (505) staff       (20)       13 2024-05-16 16:30:03.000000 saf_datasets-0.6.6/saf_datasets.egg-info/top_level.txt
+-rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)       38 2024-05-16 16:30:03.537243 saf_datasets-0.6.6/setup.cfg
+-rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)      815 2024-05-16 16:28:27.000000 saf_datasets-0.6.6/setup.py
```

### Comparing `saf_datasets-0.6.5/LICENSE` & `saf_datasets-0.6.6/LICENSE`

 * *Files identical despite different names*

### Comparing `saf_datasets-0.6.5/PKG-INFO` & `saf_datasets-0.6.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: saf-datasets
-Version: 0.6.5
+Version: 0.6.6
 Summary: Data set loading and annotation facilities for the Simple Annotation Framework
 Home-page: 
 Author: Danilo S. Carvalho
 Author-email: "Danilo S. Carvalho" <danilo.carvalho@manchester.ac.uk>
 Project-URL: Homepage, https://github.com/neuro-symbolic-ai/saf_datasets
 Project-URL: Issues, https://github.com/neuro-symbolic-ai/saf_datasets/issues
 Keywords: datasets,annotated,nlp
```

### Comparing `saf_datasets-0.6.5/README.md` & `saf_datasets-0.6.6/README.md`

 * *Files identical despite different names*

### Comparing `saf_datasets-0.6.5/pyproject.toml` & `saf_datasets-0.6.6/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "saf-datasets"
-version = "0.6.5"
+version = "0.6.6"
 authors = [
   { name="Danilo S. Carvalho", email="danilo.carvalho@manchester.ac.uk" }
 ]
 description = "Data set loading and annotation facilities for the Simple Annotation Framework"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `saf_datasets-0.6.5/saf_datasets/annotators/allennlp_srl.py` & `saf_datasets-0.6.6/saf_datasets/annotators/allennlp_srl.py`

 * *Files identical despite different names*

### Comparing `saf_datasets-0.6.5/saf_datasets/annotators/spacy.py` & `saf_datasets-0.6.6/saf_datasets/annotators/spacy.py`

 * *Files identical despite different names*

### Comparing `saf_datasets-0.6.5/saf_datasets/annotators/transformer.py` & `saf_datasets-0.6.6/saf_datasets/annotators/transformer.py`

 * *Files identical despite different names*

### Comparing `saf_datasets-0.6.5/saf_datasets/data_access/allnli.py` & `saf_datasets-0.6.6/saf_datasets/data_access/allnli.py`

 * *Files identical despite different names*

### Comparing `saf_datasets-0.6.5/saf_datasets/data_access/codwoe.py` & `saf_datasets-0.6.6/saf_datasets/data_access/codwoe.py`

 * *Files identical despite different names*

### Comparing `saf_datasets-0.6.5/saf_datasets/data_access/cpae.py` & `saf_datasets-0.6.6/saf_datasets/data_access/cpae.py`

 * *Files identical despite different names*

### Comparing `saf_datasets-0.6.5/saf_datasets/data_access/dataset.py` & `saf_datasets-0.6.6/saf_datasets/data_access/dataset.py`

 * *Files identical despite different names*

### Comparing `saf_datasets-0.6.5/saf_datasets/data_access/entailmentbank.py` & `saf_datasets-0.6.6/saf_datasets/data_access/entailmentbank.py`

 * *Files identical despite different names*

### Comparing `saf_datasets-0.6.5/saf_datasets/data_access/stsb.py` & `saf_datasets-0.6.6/saf_datasets/data_access/stsb.py`

 * *Files identical despite different names*

### Comparing `saf_datasets-0.6.5/saf_datasets/data_access/wiktionary.py` & `saf_datasets-0.6.6/saf_datasets/data_access/wiktionary.py`

 * *Files identical despite different names*

### Comparing `saf_datasets-0.6.5/saf_datasets/data_access/wordnet_filtered.py` & `saf_datasets-0.6.6/saf_datasets/data_access/wordnet_filtered.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
         "url": BASE_URL + "wordnet_filtered_spacy_dsr_srl.pickle.gz"
     }
 }
 
 
 class WordNetFilteredDataSet(SentenceDataSet):
     """
-    Wordnet filtered data set: A collection of filtered definition sentences from WordNet
+    WordNet filtered data set: A collection of filtered definition sentences from WordNet
 
     Each element of this dataset is a definition sentence (gloss) of a single synset, as it appears in WordNet.
     Definitions were filtered to only include those which definiendum (the term being defined) is representable by
     a single token from the LLaMa tokenizer.
     Each sentence is annotated with a "definiendum" and corresponding metadata from WordNet (WordNet id,
     brown_frequency, wordnet_frequency, category, abstraction_level, generalization_level).
```

### Comparing `saf_datasets-0.6.5/saf_datasets/wrappers/hf.py` & `saf_datasets-0.6.6/saf_datasets/wrappers/hf.py`

 * *Files identical despite different names*

### Comparing `saf_datasets-0.6.5/saf_datasets/wrappers/torch.py` & `saf_datasets-0.6.6/saf_datasets/wrappers/torch.py`

 * *Files identical despite different names*

### Comparing `saf_datasets-0.6.5/saf_datasets.egg-info/PKG-INFO` & `saf_datasets-0.6.6/saf_datasets.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: saf-datasets
-Version: 0.6.5
+Version: 0.6.6
 Summary: Data set loading and annotation facilities for the Simple Annotation Framework
 Home-page: 
 Author: Danilo S. Carvalho
 Author-email: "Danilo S. Carvalho" <danilo.carvalho@manchester.ac.uk>
 Project-URL: Homepage, https://github.com/neuro-symbolic-ai/saf_datasets
 Project-URL: Issues, https://github.com/neuro-symbolic-ai/saf_datasets/issues
 Keywords: datasets,annotated,nlp
```

### Comparing `saf_datasets-0.6.5/saf_datasets.egg-info/SOURCES.txt` & `saf_datasets-0.6.6/saf_datasets.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -19,10 +19,11 @@
 saf_datasets/data_access/codwoe.py
 saf_datasets/data_access/cpae.py
 saf_datasets/data_access/dataset.py
 saf_datasets/data_access/entailmentbank.py
 saf_datasets/data_access/stsb.py
 saf_datasets/data_access/wiktionary.py
 saf_datasets/data_access/wordnet_filtered.py
+saf_datasets/data_access/wordnet_spanish.py
 saf_datasets/wrappers/__init__.py
 saf_datasets/wrappers/hf.py
 saf_datasets/wrappers/torch.py
```

### Comparing `saf_datasets-0.6.5/setup.py` & `saf_datasets-0.6.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     install_requires = [str(x).strip() for x in all_reqs]
 
     return install_requires
 
 
 setup(
     name='saf_datasets',
-    version='0.6.5',
+    version='0.6.6',
     packages=['saf_datasets', 'saf_datasets.annotators', 'saf_datasets.data_access', 'saf_datasets.wrappers'],
     url='',
     author='Danilo S. Carvalho',
     author_email='danilo.carvalho@manchester.ac.uk',
     description='Data set loading and annotation facilities for the Simple Annotation Framework',
     install_requires=load_requirements()
 )
```

