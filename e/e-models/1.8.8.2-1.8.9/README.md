# Comparing `tmp/e-models-1.8.8.2.tar.gz` & `tmp/e_models-1.8.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "e-models-1.8.8.2.tar", last modified: Thu May  9 17:34:48 2024, max compression
+gzip compressed data, was "e_models-1.8.9.tar", last modified: Wed May 15 20:07:53 2024, max compression
```

## Comparing `e-models-1.8.8.2.tar` & `e_models-1.8.9.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2024-05-09 17:34:48.579804 e-models-1.8.8.2/
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     1501 2023-03-30 21:13:00.000000 e-models-1.8.8.2/LICENSE
--rw-r--r--   0 molveyra  (1001) molveyra  (1001)    13332 2024-05-09 17:34:48.579804 e-models-1.8.8.2/PKG-INFO
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)    12478 2024-02-27 17:55:52.000000 e-models-1.8.8.2/README.md
-drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2024-05-09 17:34:48.571804 e-models-1.8.8.2/e_models.egg-info/
--rw-r--r--   0 molveyra  (1001) molveyra  (1001)    13332 2024-05-09 17:34:48.000000 e-models-1.8.8.2/e_models.egg-info/PKG-INFO
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)      710 2024-05-09 17:34:48.000000 e-models-1.8.8.2/e_models.egg-info/SOURCES.txt
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)        1 2024-05-09 17:34:48.000000 e-models-1.8.8.2/e_models.egg-info/dependency_links.txt
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)      104 2024-05-09 17:34:48.000000 e-models-1.8.8.2/e_models.egg-info/requires.txt
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)        8 2024-05-09 17:34:48.000000 e-models-1.8.8.2/e_models.egg-info/top_level.txt
-drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2024-05-09 17:34:48.575804 e-models-1.8.8.2/emodels/
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)       24 2024-05-09 17:30:26.000000 e-models-1.8.8.2/emodels/__init__.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)      340 2023-11-06 19:18:12.000000 e-models-1.8.8.2/emodels/config.py
-drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2024-05-09 17:34:48.575804 e-models-1.8.8.2/emodels/datasets/
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)        0 2023-06-23 18:11:59.000000 e-models-1.8.8.2/emodels/datasets/__init__.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)    16404 2023-11-03 19:09:54.000000 e-models-1.8.8.2/emodels/datasets/hugging.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)    21433 2024-04-18 23:00:27.000000 e-models-1.8.8.2/emodels/datasets/models.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)      374 2023-08-31 18:27:15.000000 e-models-1.8.8.2/emodels/datasets/stypes.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     2299 2024-03-14 19:03:35.000000 e-models-1.8.8.2/emodels/datasets/tokenizers.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)    12361 2024-03-18 21:52:08.000000 e-models-1.8.8.2/emodels/datasets/utils.py
-drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2024-05-09 17:34:48.575804 e-models-1.8.8.2/emodels/html2text/
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)    35479 2023-07-21 16:26:32.000000 e-models-1.8.8.2/emodels/html2text/__init__.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     3873 2023-05-04 18:51:26.000000 e-models-1.8.8.2/emodels/html2text/config.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)      423 2023-05-04 18:51:26.000000 e-models-1.8.8.2/emodels/html2text/elements.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)       71 2023-05-04 18:51:26.000000 e-models-1.8.8.2/emodels/html2text/typing.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     8034 2023-05-04 18:51:26.000000 e-models-1.8.8.2/emodels/html2text/utils.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)        0 2023-05-04 18:51:26.000000 e-models-1.8.8.2/emodels/py.typed
-drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2024-05-09 17:34:48.575804 e-models-1.8.8.2/emodels/scrapyutils/
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)        0 2023-08-04 13:47:09.000000 e-models-1.8.8.2/emodels/scrapyutils/__init__.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     4734 2024-02-27 12:04:53.000000 e-models-1.8.8.2/emodels/scrapyutils/loader.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     6339 2024-02-27 17:16:48.000000 e-models-1.8.8.2/emodels/scrapyutils/response.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)       31 2023-03-30 21:32:48.000000 e-models-1.8.8.2/pyproject.toml
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)       38 2024-05-09 17:34:48.579804 e-models-1.8.8.2/setup.cfg
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     1088 2024-05-09 17:30:09.000000 e-models-1.8.8.2/setup.py
-drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2024-05-09 17:34:48.575804 e-models-1.8.8.2/tests/
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     6355 2023-08-04 13:47:35.000000 e-models-1.8.8.2/tests/test_html2text.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)    12999 2024-02-27 17:16:48.000000 e-models-1.8.8.2/tests/test_scrapyutils.py
+drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2024-05-15 20:07:53.597839 e_models-1.8.9/
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     1501 2023-03-30 21:13:00.000000 e_models-1.8.9/LICENSE
+-rw-r--r--   0 molveyra  (1001) molveyra  (1001)    13540 2024-05-15 20:07:53.597839 e_models-1.8.9/PKG-INFO
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)    12688 2024-05-15 19:54:08.000000 e_models-1.8.9/README.md
+drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2024-05-15 20:07:53.593839 e_models-1.8.9/e_models.egg-info/
+-rw-r--r--   0 molveyra  (1001) molveyra  (1001)    13540 2024-05-15 20:07:53.000000 e_models-1.8.9/e_models.egg-info/PKG-INFO
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)      710 2024-05-15 20:07:53.000000 e_models-1.8.9/e_models.egg-info/SOURCES.txt
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)        1 2024-05-15 20:07:53.000000 e_models-1.8.9/e_models.egg-info/dependency_links.txt
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)      104 2024-05-15 20:07:53.000000 e_models-1.8.9/e_models.egg-info/requires.txt
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)        8 2024-05-15 20:07:53.000000 e_models-1.8.9/e_models.egg-info/top_level.txt
+drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2024-05-15 20:07:53.593839 e_models-1.8.9/emodels/
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)       22 2024-05-15 20:07:34.000000 e_models-1.8.9/emodels/__init__.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)      412 2024-05-15 19:08:03.000000 e_models-1.8.9/emodels/config.py
+drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2024-05-15 20:07:53.593839 e_models-1.8.9/emodels/datasets/
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)        0 2023-06-23 18:11:59.000000 e_models-1.8.9/emodels/datasets/__init__.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)    16404 2023-11-03 19:09:54.000000 e_models-1.8.9/emodels/datasets/hugging.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)    21433 2024-04-18 23:00:27.000000 e_models-1.8.9/emodels/datasets/models.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)      374 2023-08-31 18:27:15.000000 e_models-1.8.9/emodels/datasets/stypes.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     2299 2024-03-14 19:03:35.000000 e_models-1.8.9/emodels/datasets/tokenizers.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)    12361 2024-03-18 21:52:08.000000 e_models-1.8.9/emodels/datasets/utils.py
+drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2024-05-15 20:07:53.593839 e_models-1.8.9/emodels/html2text/
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)    35479 2023-07-21 16:26:32.000000 e_models-1.8.9/emodels/html2text/__init__.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     3873 2023-05-04 18:51:26.000000 e_models-1.8.9/emodels/html2text/config.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)      423 2023-05-04 18:51:26.000000 e_models-1.8.9/emodels/html2text/elements.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)       71 2023-05-04 18:51:26.000000 e_models-1.8.9/emodels/html2text/typing.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     8034 2023-05-04 18:51:26.000000 e_models-1.8.9/emodels/html2text/utils.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)        0 2023-05-04 18:51:26.000000 e_models-1.8.9/emodels/py.typed
+drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2024-05-15 20:07:53.593839 e_models-1.8.9/emodels/scrapyutils/
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)        0 2023-08-04 13:47:09.000000 e_models-1.8.9/emodels/scrapyutils/__init__.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     5169 2024-05-15 19:52:54.000000 e_models-1.8.9/emodels/scrapyutils/loader.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     6339 2024-02-27 17:16:48.000000 e_models-1.8.9/emodels/scrapyutils/response.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)       31 2023-03-30 21:32:48.000000 e_models-1.8.9/pyproject.toml
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)       38 2024-05-15 20:07:53.597839 e_models-1.8.9/setup.cfg
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     1086 2024-05-15 20:07:34.000000 e_models-1.8.9/setup.py
+drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2024-05-15 20:07:53.593839 e_models-1.8.9/tests/
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     6355 2023-08-04 13:47:35.000000 e_models-1.8.9/tests/test_html2text.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)    12999 2024-02-27 17:16:48.000000 e_models-1.8.9/tests/test_scrapyutils.py
```

### Comparing `e-models-1.8.8.2/LICENSE` & `e_models-1.8.9/LICENSE`

 * *Files identical despite different names*

### Comparing `e-models-1.8.8.2/PKG-INFO` & `e_models-1.8.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: e-models
-Version: 1.8.8.2
+Version: 1.8.9
 Summary: Tools for helping build of extraction models with scrapy spiders.
 Home-page: https://github.com/kalessin/emodels
 Author: Martin Olveyra
 Author-email: molveyra@gmail.com
 License: BSD
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -48,21 +48,22 @@
    any other line of the spider code. If the selector still works, it is not needed to be changed. If it doesn't work anymore, it can be replaced by common and known selectors without affecting
    anything else.
 
 #### Set up
 
 Instead of subclass your item loaders from `scrapy.loader.ItemLoader`, use `emodels.scrapyutils.loader.ExtractItemLoader`. This action will not affect the working of itemloaders and will enable the
 properties just described above. In addition, in order to save the collected extraction data, it is required to set the environment variable `EMODELS_SAVE_EXTRACT_ITEMS` to 1. The collected
-extraction data will be stored at `<user home folder>/.datasets/items/<item class name>/<sequence number>.jl.gz`. The base folder `<user home folder>/.datasets` is the default one. You can
+extraction data will be stored by default at `<user home folder>/.datasets/items/<item class name>/<sequence number>.jl.gz`. Instead of a default sequence number you may want to use a custom filename.
+For that purpose you can use the environment variable `EMODELS_ITEMS_FILENAME`. The base folder `<user home folder>/.datasets` is the default one. You can
 customize it via the environment variable `EMODELS_REPOSITORY`.
 
 So, in order to maintain a clean and organized dataset, only enable extract items saving when you are sure you have the correct extraction selectors. Then run locally:
 
 ```
-EMODELS_SAVE_EXTRACT_ITEMS=1 scrapy crawl myspider
+EMODELS_SAVE_EXTRACT_ITEMS=1 [EMODELS_ITEMS_FILENAME=<custom filename>] scrapy crawl myspider
 ```
 
 In addition, in order to have your dataset organized, you may want to choose the same item class name for same item schema, even accross multiple projects. And avoid to repeat it among items with different
 schema. However, in general you will use extraction data from all classes of items at same time in order to train a transformer model, as this is the way how transformers learn to generalize. In addition
 avoid to create multiple collections for same item class and target site, as they will not provide diversity and you may commit the mistake of having same sample distribution in train and test datasets.
 
 At the end you will have a transformer model that is suited to extract any kind of item, as they are trained not to extract "data from x item" but instead to recognize and extract based on fields.
```

### Comparing `e-models-1.8.8.2/README.md` & `e_models-1.8.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -24,21 +24,22 @@
    any other line of the spider code. If the selector still works, it is not needed to be changed. If it doesn't work anymore, it can be replaced by common and known selectors without affecting
    anything else.
 
 #### Set up
 
 Instead of subclass your item loaders from `scrapy.loader.ItemLoader`, use `emodels.scrapyutils.loader.ExtractItemLoader`. This action will not affect the working of itemloaders and will enable the
 properties just described above. In addition, in order to save the collected extraction data, it is required to set the environment variable `EMODELS_SAVE_EXTRACT_ITEMS` to 1. The collected
-extraction data will be stored at `<user home folder>/.datasets/items/<item class name>/<sequence number>.jl.gz`. The base folder `<user home folder>/.datasets` is the default one. You can
+extraction data will be stored by default at `<user home folder>/.datasets/items/<item class name>/<sequence number>.jl.gz`. Instead of a default sequence number you may want to use a custom filename.
+For that purpose you can use the environment variable `EMODELS_ITEMS_FILENAME`. The base folder `<user home folder>/.datasets` is the default one. You can
 customize it via the environment variable `EMODELS_REPOSITORY`.
 
 So, in order to maintain a clean and organized dataset, only enable extract items saving when you are sure you have the correct extraction selectors. Then run locally:
 
 ```
-EMODELS_SAVE_EXTRACT_ITEMS=1 scrapy crawl myspider
+EMODELS_SAVE_EXTRACT_ITEMS=1 [EMODELS_ITEMS_FILENAME=<custom filename>] scrapy crawl myspider
 ```
 
 In addition, in order to have your dataset organized, you may want to choose the same item class name for same item schema, even accross multiple projects. And avoid to repeat it among items with different
 schema. However, in general you will use extraction data from all classes of items at same time in order to train a transformer model, as this is the way how transformers learn to generalize. In addition
 avoid to create multiple collections for same item class and target site, as they will not provide diversity and you may commit the mistake of having same sample distribution in train and test datasets.
 
 At the end you will have a transformer model that is suited to extract any kind of item, as they are trained not to extract "data from x item" but instead to recognize and extract based on fields.
```

### Comparing `e-models-1.8.8.2/e_models.egg-info/PKG-INFO` & `e_models-1.8.9/e_models.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: e-models
-Version: 1.8.8.2
+Version: 1.8.9
 Summary: Tools for helping build of extraction models with scrapy spiders.
 Home-page: https://github.com/kalessin/emodels
 Author: Martin Olveyra
 Author-email: molveyra@gmail.com
 License: BSD
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -48,21 +48,22 @@
    any other line of the spider code. If the selector still works, it is not needed to be changed. If it doesn't work anymore, it can be replaced by common and known selectors without affecting
    anything else.
 
 #### Set up
 
 Instead of subclass your item loaders from `scrapy.loader.ItemLoader`, use `emodels.scrapyutils.loader.ExtractItemLoader`. This action will not affect the working of itemloaders and will enable the
 properties just described above. In addition, in order to save the collected extraction data, it is required to set the environment variable `EMODELS_SAVE_EXTRACT_ITEMS` to 1. The collected
-extraction data will be stored at `<user home folder>/.datasets/items/<item class name>/<sequence number>.jl.gz`. The base folder `<user home folder>/.datasets` is the default one. You can
+extraction data will be stored by default at `<user home folder>/.datasets/items/<item class name>/<sequence number>.jl.gz`. Instead of a default sequence number you may want to use a custom filename.
+For that purpose you can use the environment variable `EMODELS_ITEMS_FILENAME`. The base folder `<user home folder>/.datasets` is the default one. You can
 customize it via the environment variable `EMODELS_REPOSITORY`.
 
 So, in order to maintain a clean and organized dataset, only enable extract items saving when you are sure you have the correct extraction selectors. Then run locally:
 
 ```
-EMODELS_SAVE_EXTRACT_ITEMS=1 scrapy crawl myspider
+EMODELS_SAVE_EXTRACT_ITEMS=1 [EMODELS_ITEMS_FILENAME=<custom filename>] scrapy crawl myspider
 ```
 
 In addition, in order to have your dataset organized, you may want to choose the same item class name for same item schema, even accross multiple projects. And avoid to repeat it among items with different
 schema. However, in general you will use extraction data from all classes of items at same time in order to train a transformer model, as this is the way how transformers learn to generalize. In addition
 avoid to create multiple collections for same item class and target site, as they will not provide diversity and you may commit the mistake of having same sample distribution in train and test datasets.
 
 At the end you will have a transformer model that is suited to extract any kind of item, as they are trained not to extract "data from x item" but instead to recognize and extract based on fields.
```

### Comparing `e-models-1.8.8.2/e_models.egg-info/SOURCES.txt` & `e_models-1.8.9/e_models.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `e-models-1.8.8.2/emodels/datasets/hugging.py` & `e_models-1.8.9/emodels/datasets/hugging.py`

 * *Files identical despite different names*

### Comparing `e-models-1.8.8.2/emodels/datasets/models.py` & `e_models-1.8.9/emodels/datasets/models.py`

 * *Files identical despite different names*

### Comparing `e-models-1.8.8.2/emodels/datasets/tokenizers.py` & `e_models-1.8.9/emodels/datasets/tokenizers.py`

 * *Files identical despite different names*

### Comparing `e-models-1.8.8.2/emodels/datasets/utils.py` & `e_models-1.8.9/emodels/datasets/utils.py`

 * *Files identical despite different names*

### Comparing `e-models-1.8.8.2/emodels/html2text/__init__.py` & `e_models-1.8.9/emodels/html2text/__init__.py`

 * *Files identical despite different names*

### Comparing `e-models-1.8.8.2/emodels/html2text/config.py` & `e_models-1.8.9/emodels/html2text/config.py`

 * *Files identical despite different names*

### Comparing `e-models-1.8.8.2/emodels/html2text/utils.py` & `e_models-1.8.9/emodels/html2text/utils.py`

 * *Files identical despite different names*

### Comparing `e-models-1.8.8.2/emodels/scrapyutils/loader.py` & `e_models-1.8.9/emodels/scrapyutils/loader.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,33 +1,42 @@
 import os
 import re
 import logging
+from glob import glob
 from typing import Optional
 
 from scrapy.loader import ItemLoader
 from scrapy.http import TextResponse
 from scrapy import Item
 
-from emodels.config import EMODELS_ITEMS_DIR, EMODELS_SAVE_EXTRACT_ITEMS
+from emodels.config import EMODELS_ITEMS_DIR, EMODELS_SAVE_EXTRACT_ITEMS, EMODELS_ITEMS_FILENAME
 from emodels.datasets.utils import DatasetFilename
 from emodels.scrapyutils.response import ExtractTextResponse, DEFAULT_SKIP_PREFIX
 from emodels.datasets.stypes import ExtractDict, ItemSample
 
 
 LOG = logging.getLogger(__name__)
 
 
 class ExtractItemLoader(ItemLoader):
     def __new__(cls, *args, **kwargs):
         obj = super().__new__(cls)
         if not hasattr(cls, "savefile"):
             folder = os.path.join(EMODELS_ITEMS_DIR, obj.default_item_class.__name__)
             os.makedirs(folder, exist_ok=True)
-            findex = len(os.listdir(folder))
-            cls.savefile: DatasetFilename[ItemSample] = DatasetFilename(os.path.join(folder, f"{findex}.jl.gz"))
+            fname_prefix = EMODELS_ITEMS_FILENAME
+            complete_fname_prefix = os.path.join(folder, fname_prefix)
+            idx = len(glob(complete_fname_prefix + "*"))
+            if idx > 0:
+                if fname_prefix:
+                    complete_fname_prefix += "-"
+                complete_fname_prefix += str(idx)
+            complete_fname = complete_fname_prefix + ".jl.gz"
+            cls.savefile: DatasetFilename[ItemSample] = DatasetFilename(complete_fname)
+            LOG.info(f"Items will be saved to {cls.savefile}")
         return obj
 
     def _check_valid_response(self):
         return isinstance(self.context.get("response"), TextResponse)
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
```

### Comparing `e-models-1.8.8.2/emodels/scrapyutils/response.py` & `e_models-1.8.9/emodels/scrapyutils/response.py`

 * *Files identical despite different names*

### Comparing `e-models-1.8.8.2/setup.py` & `e_models-1.8.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Automatically created by: shub deploy
 
 from setuptools import setup, find_packages
 
 setup(
     name         = 'e-models',
-    version      = '1.8.8.2',
+    version      = '1.8.9',
     description  = 'Tools for helping build of extraction models with scrapy spiders.',
     long_description = open('README.md').read(),
     long_description_content_type = 'text/markdown',
     license      = 'BSD',
     author       = 'Martin Olveyra',
     author_email = 'molveyra@gmail.com',
     url          = 'https://github.com/kalessin/emodels',
```

### Comparing `e-models-1.8.8.2/tests/test_html2text.py` & `e_models-1.8.9/tests/test_html2text.py`

 * *Files identical despite different names*

### Comparing `e-models-1.8.8.2/tests/test_scrapyutils.py` & `e_models-1.8.9/tests/test_scrapyutils.py`

 * *Files identical despite different names*

