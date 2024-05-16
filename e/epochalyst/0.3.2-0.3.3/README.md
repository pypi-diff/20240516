# Comparing `tmp/epochalyst-0.3.2.tar.gz` & `tmp/epochalyst-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "epochalyst-0.3.2.tar", last modified: Wed Apr 17 10:05:33 2024, max compression
+gzip compressed data, was "epochalyst-0.3.3.tar", last modified: Thu May 16 09:09:58 2024, max compression
```

## Comparing `epochalyst-0.3.2.tar` & `epochalyst-0.3.3.tar`

### file list

```diff
@@ -1,52 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:05:33.570246 epochalyst-0.3.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-17 10:05:27.000000 epochalyst-0.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2892 2024-04-17 10:05:33.570246 epochalyst-0.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2234 2024-04-17 10:05:27.000000 epochalyst-0.3.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:05:33.566246 epochalyst-0.3.2/epochalyst/
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-17 10:05:28.000000 epochalyst-0.3.2/epochalyst/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:05:33.566246 epochalyst-0.3.2/epochalyst/_core/
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-17 10:05:28.000000 epochalyst-0.3.2/epochalyst/_core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:05:33.566246 epochalyst-0.3.2/epochalyst/_core/_caching/
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-17 10:05:28.000000 epochalyst-0.3.2/epochalyst/_core/_caching/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15786 2024-04-17 10:05:28.000000 epochalyst-0.3.2/epochalyst/_core/_caching/_cacher.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:05:33.566246 epochalyst-0.3.2/epochalyst/_core/_logging/
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-17 10:05:28.000000 epochalyst-0.3.2/epochalyst/_core/_logging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3032 2024-04-17 10:05:28.000000 epochalyst-0.3.2/epochalyst/_core/_logging/_logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:05:33.566246 epochalyst-0.3.2/epochalyst/_core/_pipeline/
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-17 10:05:28.000000 epochalyst-0.3.2/epochalyst/_core/_pipeline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      363 2024-04-17 10:05:28.000000 epochalyst-0.3.2/epochalyst/_core/_pipeline/_custom_data_parallel.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:05:33.566246 epochalyst-0.3.2/epochalyst/logging/
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-17 10:05:28.000000 epochalyst-0.3.2/epochalyst/logging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      870 2024-04-17 10:05:28.000000 epochalyst-0.3.2/epochalyst/logging/section_separator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:05:33.566246 epochalyst-0.3.2/epochalyst/pipeline/
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-17 10:05:28.000000 epochalyst-0.3.2/epochalyst/pipeline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1623 2024-04-17 10:05:28.000000 epochalyst-0.3.2/epochalyst/pipeline/ensemble.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:05:33.566246 epochalyst-0.3.2/epochalyst/pipeline/model/
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-17 10:05:28.000000 epochalyst-0.3.2/epochalyst/pipeline/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2124 2024-04-17 10:05:28.000000 epochalyst-0.3.2/epochalyst/pipeline/model/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:05:33.570246 epochalyst-0.3.2/epochalyst/pipeline/model/training/
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-17 10:05:28.000000 epochalyst-0.3.2/epochalyst/pipeline/model/training/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:05:33.570246 epochalyst-0.3.2/epochalyst/pipeline/model/training/augmentation/
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-17 10:05:28.000000 epochalyst-0.3.2/epochalyst/pipeline/model/training/augmentation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3152 2024-04-17 10:05:28.000000 epochalyst-0.3.2/epochalyst/pipeline/model/training/augmentation/image_augmentations.py
--rw-r--r--   0 runner    (1001) docker     (127)     6889 2024-04-17 10:05:28.000000 epochalyst-0.3.2/epochalyst/pipeline/model/training/augmentation/time_series_augmentations.py
--rw-r--r--   0 runner    (1001) docker     (127)     3467 2024-04-17 10:05:28.000000 epochalyst-0.3.2/epochalyst/pipeline/model/training/augmentation/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:05:33.570246 epochalyst-0.3.2/epochalyst/pipeline/model/training/models/
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-17 10:05:28.000000 epochalyst-0.3.2/epochalyst/pipeline/model/training/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-04-17 10:05:28.000000 epochalyst-0.3.2/epochalyst/pipeline/model/training/models/timm.py
--rw-r--r--   0 runner    (1001) docker     (127)     3448 2024-04-17 10:05:28.000000 epochalyst-0.3.2/epochalyst/pipeline/model/training/pretrain_block.py
--rw-r--r--   0 runner    (1001) docker     (127)    30679 2024-04-17 10:05:28.000000 epochalyst-0.3.2/epochalyst/pipeline/model/training/torch_trainer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4966 2024-04-17 10:05:28.000000 epochalyst-0.3.2/epochalyst/pipeline/model/training/training.py
--rw-r--r--   0 runner    (1001) docker     (127)     4891 2024-04-17 10:05:28.000000 epochalyst-0.3.2/epochalyst/pipeline/model/training/training_block.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:05:33.570246 epochalyst-0.3.2/epochalyst/pipeline/model/transformation/
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-17 10:05:28.000000 epochalyst-0.3.2/epochalyst/pipeline/model/transformation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4441 2024-04-17 10:05:28.000000 epochalyst-0.3.2/epochalyst/pipeline/model/transformation/transformation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3285 2024-04-17 10:05:28.000000 epochalyst-0.3.2/epochalyst/pipeline/model/transformation/transformation_block.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:05:33.570246 epochalyst-0.3.2/epochalyst.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2892 2024-04-17 10:05:33.000000 epochalyst-0.3.2/epochalyst.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1500 2024-04-17 10:05:33.000000 epochalyst-0.3.2/epochalyst.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 10:05:33.000000 epochalyst-0.3.2/epochalyst.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-17 10:05:33.000000 epochalyst-0.3.2/epochalyst.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-17 10:05:33.000000 epochalyst-0.3.2/epochalyst.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3663 2024-04-17 10:05:28.000000 epochalyst-0.3.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 10:05:33.570246 epochalyst-0.3.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:09:58.291777 epochalyst-0.3.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-16 09:09:52.000000 epochalyst-0.3.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2892 2024-05-16 09:09:58.291777 epochalyst-0.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2234 2024-05-16 09:09:52.000000 epochalyst-0.3.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:09:58.283777 epochalyst-0.3.3/epochalyst/
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-05-16 09:09:52.000000 epochalyst-0.3.3/epochalyst/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:09:58.287777 epochalyst-0.3.3/epochalyst/_core/
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-16 09:09:52.000000 epochalyst-0.3.3/epochalyst/_core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:09:58.287777 epochalyst-0.3.3/epochalyst/_core/_caching/
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-16 09:09:52.000000 epochalyst-0.3.3/epochalyst/_core/_caching/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15786 2024-05-16 09:09:52.000000 epochalyst-0.3.3/epochalyst/_core/_caching/_cacher.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:09:58.287777 epochalyst-0.3.3/epochalyst/_core/_logging/
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-16 09:09:52.000000 epochalyst-0.3.3/epochalyst/_core/_logging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3032 2024-05-16 09:09:52.000000 epochalyst-0.3.3/epochalyst/_core/_logging/_logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:09:58.287777 epochalyst-0.3.3/epochalyst/_core/_pipeline/
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-16 09:09:52.000000 epochalyst-0.3.3/epochalyst/_core/_pipeline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-05-16 09:09:52.000000 epochalyst-0.3.3/epochalyst/_core/_pipeline/_custom_data_parallel.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:09:58.287777 epochalyst-0.3.3/epochalyst/logging/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-16 09:09:52.000000 epochalyst-0.3.3/epochalyst/logging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      870 2024-05-16 09:09:52.000000 epochalyst-0.3.3/epochalyst/logging/section_separator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:09:58.287777 epochalyst-0.3.3/epochalyst/pipeline/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-16 09:09:52.000000 epochalyst-0.3.3/epochalyst/pipeline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1623 2024-05-16 09:09:52.000000 epochalyst-0.3.3/epochalyst/pipeline/ensemble.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:09:58.287777 epochalyst-0.3.3/epochalyst/pipeline/model/
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-16 09:09:52.000000 epochalyst-0.3.3/epochalyst/pipeline/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2124 2024-05-16 09:09:52.000000 epochalyst-0.3.3/epochalyst/pipeline/model/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:09:58.287777 epochalyst-0.3.3/epochalyst/pipeline/model/training/
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-16 09:09:52.000000 epochalyst-0.3.3/epochalyst/pipeline/model/training/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:09:58.291777 epochalyst-0.3.3/epochalyst/pipeline/model/training/augmentation/
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-16 09:09:52.000000 epochalyst-0.3.3/epochalyst/pipeline/model/training/augmentation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3152 2024-05-16 09:09:52.000000 epochalyst-0.3.3/epochalyst/pipeline/model/training/augmentation/image_augmentations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6889 2024-05-16 09:09:52.000000 epochalyst-0.3.3/epochalyst/pipeline/model/training/augmentation/time_series_augmentations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3467 2024-05-16 09:09:52.000000 epochalyst-0.3.3/epochalyst/pipeline/model/training/augmentation/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:09:58.291777 epochalyst-0.3.3/epochalyst/pipeline/model/training/models/
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-16 09:09:52.000000 epochalyst-0.3.3/epochalyst/pipeline/model/training/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-05-16 09:09:52.000000 epochalyst-0.3.3/epochalyst/pipeline/model/training/models/timm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3448 2024-05-16 09:09:52.000000 epochalyst-0.3.3/epochalyst/pipeline/model/training/pretrain_block.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31352 2024-05-16 09:09:52.000000 epochalyst-0.3.3/epochalyst/pipeline/model/training/torch_trainer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5153 2024-05-16 09:09:52.000000 epochalyst-0.3.3/epochalyst/pipeline/model/training/training.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5117 2024-05-16 09:09:52.000000 epochalyst-0.3.3/epochalyst/pipeline/model/training/training_block.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:09:58.291777 epochalyst-0.3.3/epochalyst/pipeline/model/training/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-16 09:09:52.000000 epochalyst-0.3.3/epochalyst/pipeline/model/training/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-05-16 09:09:52.000000 epochalyst-0.3.3/epochalyst/pipeline/model/training/utils/tensor_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:09:58.291777 epochalyst-0.3.3/epochalyst/pipeline/model/transformation/
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-16 09:09:52.000000 epochalyst-0.3.3/epochalyst/pipeline/model/transformation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4537 2024-05-16 09:09:52.000000 epochalyst-0.3.3/epochalyst/pipeline/model/transformation/transformation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3368 2024-05-16 09:09:52.000000 epochalyst-0.3.3/epochalyst/pipeline/model/transformation/transformation_block.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:09:58.291777 epochalyst-0.3.3/epochalyst.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2892 2024-05-16 09:09:58.000000 epochalyst-0.3.3/epochalyst.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-05-16 09:09:58.000000 epochalyst-0.3.3/epochalyst.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 09:09:58.000000 epochalyst-0.3.3/epochalyst.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-16 09:09:58.000000 epochalyst-0.3.3/epochalyst.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-16 09:09:58.000000 epochalyst-0.3.3/epochalyst.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3663 2024-05-16 09:09:52.000000 epochalyst-0.3.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 09:09:58.291777 epochalyst-0.3.3/setup.cfg
```

### Comparing `epochalyst-0.3.2/LICENSE` & `epochalyst-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `epochalyst-0.3.2/PKG-INFO` & `epochalyst-0.3.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: epochalyst
-Version: 0.3.2
+Version: 0.3.3
 Summary: This package contains the code for team Epoch's pipeline
 Author-email: Jasper van Selm <jmvanselm@gmail.com>, Ariel Ebersberger <arielebersberger@gmail.com>, Tolga Kopar <cahittolgakopar@gmail.com>, Jeffrey Lim <jeffrey-lim@outlook.com>, Hugo de Heer <hugodeheer1234@gmail.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `epochalyst-0.3.2/README.md` & `epochalyst-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `epochalyst-0.3.2/epochalyst/_core/_caching/_cacher.py` & `epochalyst-0.3.3/epochalyst/_core/_caching/_cacher.py`

 * *Files identical despite different names*

### Comparing `epochalyst-0.3.2/epochalyst/_core/_logging/_logger.py` & `epochalyst-0.3.3/epochalyst/_core/_logging/_logger.py`

 * *Files identical despite different names*

### Comparing `epochalyst-0.3.2/epochalyst/logging/section_separator.py` & `epochalyst-0.3.3/epochalyst/logging/section_separator.py`

 * *Files identical despite different names*

### Comparing `epochalyst-0.3.2/epochalyst/pipeline/ensemble.py` & `epochalyst-0.3.3/epochalyst/pipeline/ensemble.py`

 * *Files identical despite different names*

### Comparing `epochalyst-0.3.2/epochalyst/pipeline/model/model.py` & `epochalyst-0.3.3/epochalyst/pipeline/model/model.py`

 * *Files identical despite different names*

### Comparing `epochalyst-0.3.2/epochalyst/pipeline/model/training/augmentation/image_augmentations.py` & `epochalyst-0.3.3/epochalyst/pipeline/model/training/augmentation/image_augmentations.py`

 * *Files identical despite different names*

### Comparing `epochalyst-0.3.2/epochalyst/pipeline/model/training/augmentation/time_series_augmentations.py` & `epochalyst-0.3.3/epochalyst/pipeline/model/training/augmentation/time_series_augmentations.py`

 * *Files identical despite different names*

### Comparing `epochalyst-0.3.2/epochalyst/pipeline/model/training/augmentation/utils.py` & `epochalyst-0.3.3/epochalyst/pipeline/model/training/augmentation/utils.py`

 * *Files identical despite different names*

### Comparing `epochalyst-0.3.2/epochalyst/pipeline/model/training/models/timm.py` & `epochalyst-0.3.3/epochalyst/pipeline/model/training/models/timm.py`

 * *Files identical despite different names*

### Comparing `epochalyst-0.3.2/epochalyst/pipeline/model/training/pretrain_block.py` & `epochalyst-0.3.3/epochalyst/pipeline/model/training/pretrain_block.py`

 * *Files identical despite different names*

### Comparing `epochalyst-0.3.2/epochalyst/pipeline/model/training/torch_trainer.py` & `epochalyst-0.3.3/epochalyst/pipeline/model/training/torch_trainer.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 from torch.optim.lr_scheduler import LRScheduler
 from torch.utils.data import DataLoader, Dataset, TensorDataset
 from tqdm import tqdm
 
 from epochalyst._core._pipeline._custom_data_parallel import _CustomDataParallel
 from epochalyst.logging.section_separator import print_section_separator
 from epochalyst.pipeline.model.training.training_block import TrainingBlock
+from epochalyst.pipeline.model.training.utils.tensor_functions import batch_to_device
 
 T = TypeVar("T", bound=Dataset)  # type: ignore[type-arg]
 T_co = TypeVar("T_co", covariant=True)
 
 
 @dataclass
 class TorchTrainer(TrainingBlock):
@@ -39,14 +40,17 @@
     - `batch_size` (int): Batch size
     - `patience` (int): Patience for early stopping
     - `test_size` (float): Relative size of the test set
     - `to_predict` (str): Whether to predict on the 'test' set, 'all' data or 'none'
     - `model_name` (str): Name of the model
     - `n_folds` (float): Number of folds for cross validation (0 for train full,
     - `fold` (int): Fold number
+    - `dataloader_args (dict): Arguments for the dataloader`
+    - `x_tensor_type` (str): Type of x tensor for data
+    - `y_tensor_type` (str): Type of y tensor for labels
 
     Methods
     -------
     .. code-block:: python
         @abstractmethod
         def log_to_terminal(self, message: str) -> None:
             # Logs to terminal if implemented
@@ -138,14 +142,20 @@
     test_size: Annotated[float, Interval(ge=0, le=1)] = 0.2  # Hashing purposes
     to_predict: str = "test"
     model_name: str = "MODEL_NAME_NOT_SPECIFIED"  # No spaces allowed
 
     _fold: int = field(default=-1, init=False, repr=False, compare=False)
     n_folds: float = field(default=-1, init=True, repr=False, compare=False)
 
+    dataloader_args: dict[str, Any] = field(default_factory=dict, repr=False)
+
+    # Types for tensors
+    x_tensor_type: str = "float"
+    y_tensor_type: str = "float"
+
     def __post_init__(self) -> None:
         """Post init method for the TorchTrainer class."""
         # Make sure to_predict is either "test" or "all" or "none"
         if self.to_predict not in ["test", "all", "none"]:
             raise ValueError("to_predict should be either 'test', 'all' or 'none'")
 
         if self.n_folds == -1:
@@ -393,18 +403,19 @@
         loader = DataLoader(
             loader.dataset,
             batch_size=loader.batch_size,
             shuffle=False,
             collate_fn=(
                 collate_fn if hasattr(loader.dataset, "__getitems__") else None  # type: ignore[arg-type]
             ),
+            **self.dataloader_args,
         )
         with torch.no_grad(), tqdm(loader, unit="batch", disable=False) as tepoch:
             for data in tepoch:
-                X_batch = data[0].to(self.device).float()
+                X_batch = batch_to_device(data[0], self.x_tensor_type, self.device)
 
                 y_pred = self.model(X_batch).squeeze(1).cpu().numpy()
                 predictions.extend(y_pred)
 
         self.log_to_terminal("Done predicting")
         return np.array(predictions)
 
@@ -469,20 +480,22 @@
         :return: The training and validation dataloaders.
         """
         train_loader = DataLoader(
             train_dataset,
             batch_size=self.batch_size,
             shuffle=True,
             collate_fn=(collate_fn if hasattr(train_dataset, "__getitems__") else None),  # type: ignore[arg-type]
+            **self.dataloader_args,
         )
         test_loader = DataLoader(
             test_dataset,
             batch_size=self.batch_size,
             shuffle=False,
             collate_fn=(collate_fn if hasattr(test_dataset, "__getitems__") else None),  # type: ignore[arg-type]
+            **self.dataloader_args,
         )
         return train_loader, test_loader
 
     def update_model_directory(self, model_directory: Path) -> None:
         """Update the model directory.
 
         :param model_directory: The model directory.
@@ -597,16 +610,17 @@
         pbar = tqdm(
             dataloader,
             unit="batch",
             desc=f"Epoch {epoch} Train ({self.initialized_optimizer.param_groups[0]['lr']})",
         )
         for batch in pbar:
             X_batch, y_batch = batch
-            X_batch = X_batch.to(self.device).float()
-            y_batch = y_batch.to(self.device).float()
+
+            X_batch = batch_to_device(X_batch, self.x_tensor_type, self.device)
+            y_batch = batch_to_device(y_batch, self.x_tensor_type, self.device)
 
             # Forward pass
             y_pred = self.model(X_batch).squeeze(1)
             loss = self.criterion(y_pred, y_batch)
 
             # Backward pass
             self.initialized_optimizer.zero_grad()
@@ -615,15 +629,15 @@
 
             # Print tqdm
             losses.append(loss.item())
             pbar.set_postfix(loss=sum(losses) / len(losses))
 
         # Step the scheduler
         if self.initialized_scheduler is not None:
-            self.initialized_scheduler.step(epoch=epoch)
+            self.initialized_scheduler.step(epoch=epoch + 1)
 
         # Remove the cuda cache
         torch.cuda.empty_cache()
         gc.collect()
 
         return sum(losses) / len(losses)
 
@@ -640,16 +654,17 @@
         """
         losses = []
         self.model.eval()
         pbar = tqdm(dataloader, unit="batch")
         with torch.no_grad():
             for batch in pbar:
                 X_batch, y_batch = batch
-                X_batch = X_batch.to(self.device).float()
-                y_batch = y_batch.to(self.device).float()
+
+                X_batch = batch_to_device(X_batch, self.x_tensor_type, self.device)
+                y_batch = batch_to_device(y_batch, self.y_tensor_type, self.device)
 
                 # Forward pass
                 y_pred = self.model(X_batch).squeeze(1)
                 loss = self.criterion(y_pred, y_batch)
 
                 # Print losses
                 losses.append(loss.item())
```

### Comparing `epochalyst-0.3.2/epochalyst/pipeline/model/training/training.py` & `epochalyst-0.3.3/epochalyst/pipeline/model/training/training.py`

 * *Files 11% similar despite different names*

```diff
@@ -59,14 +59,15 @@
                     f"Cache exists for {step}, moving index of steps to {i}",
                 )
                 self.steps = self.all_steps[i:]
 
         x, y = super().train(x, y, **train_args)
 
         if cache_args:
+            self.log_to_terminal(f"Storing cache for x and y to {cache_args['storage_path']}")
             self._store_cache(name=self.get_hash() + "x", data=x, cache_args=cache_args)
             self._store_cache(name=self.get_hash() + "y", data=y, cache_args=cache_args)
 
         # Set steps to original in case class is called again (case: train -> predict)
         self.steps = self.all_steps
 
         return x, y
@@ -111,13 +112,15 @@
                 self.log_to_debug(
                     f"Cache exists for {step}, moving index of steps to {i}",
                 )
                 self.steps = self.all_steps[i:]
 
         x = super().predict(x, **pred_args)
 
-        self._store_cache(self.get_hash() + "p", x, cache_args) if cache_args else None
+        if cache_args:
+            self.log_to_terminal(f"Storing cache for x to {cache_args['storage_path']}")
+            self._store_cache(self.get_hash() + "p", x, cache_args)
 
         # Set steps to original in case class is called again
         self.steps = self.all_steps
 
         return x
```

### Comparing `epochalyst-0.3.2/epochalyst/pipeline/model/training/training_block.py` & `epochalyst-0.3.3/epochalyst/pipeline/model/training/training_block.py`

 * *Files 5% similar despite different names*

```diff
@@ -72,24 +72,26 @@
             )
             x = self._get_cache(name=self.get_hash() + "x", cache_args=cache_args)
             y = self._get_cache(name=self.get_hash() + "y", cache_args=cache_args)
             return x, y
 
         x, y = self.custom_train(x, y, **train_args)
 
-        self._store_cache(
-            name=self.get_hash() + "x",
-            data=x,
-            cache_args=cache_args,
-        ) if cache_args else None
-        self._store_cache(
-            name=self.get_hash() + "y",
-            data=y,
-            cache_args=cache_args,
-        ) if cache_args else None
+        if cache_args:
+            self.log_to_terminal(f"Storing cache for x and y to {cache_args['storage_path']}")
+            self._store_cache(
+                name=self.get_hash() + "x",
+                data=x,
+                cache_args=cache_args,
+            )
+            self._store_cache(
+                name=self.get_hash() + "y",
+                data=y,
+                cache_args=cache_args,
+            )
 
         return x, y
 
     @abstractmethod
     def custom_train(self, x: Any, y: Any, **train_args: Any) -> tuple[Any, Any]:  # noqa: ANN401
         """Train the model.
 
@@ -112,19 +114,21 @@
             name=self.get_hash() + "p",
             cache_args=cache_args,
         ):
             return self._get_cache(name=self.get_hash() + "p", cache_args=cache_args)
 
         x = self.custom_predict(x, **pred_args)
 
-        self._store_cache(
-            name=self.get_hash() + "p",
-            data=x,
-            cache_args=cache_args,
-        ) if cache_args else None
+        if cache_args:
+            self.log_to_terminal(f"Store cache for predictions to {cache_args['storage_path']}")
+            self._store_cache(
+                name=self.get_hash() + "p",
+                data=x,
+                cache_args=cache_args,
+            )
 
         return x
 
     @abstractmethod
     def custom_predict(self, x: Any, **pred_args: Any) -> Any:  # noqa: ANN401
         """Predict using the model.
```

### Comparing `epochalyst-0.3.2/epochalyst/pipeline/model/transformation/transformation.py` & `epochalyst-0.3.3/epochalyst/pipeline/model/transformation/transformation.py`

 * *Files 2% similar despite different names*

```diff
@@ -101,13 +101,14 @@
                     f"Cache exists for {step}, moving index of steps to {i}",
                 )
                 self.steps = self.all_steps[i:]
 
         data = super().transform(data, **transform_args)
 
         if cache_args:
+            self.log_to_terminal(f"Storing cache for pipeline to {cache_args['storage_path']}")
             self._store_cache(self.get_hash(), data, cache_args)
 
         # Set steps to original in case class is called again
         self.steps = self.all_steps
 
         return data
```

### Comparing `epochalyst-0.3.2/epochalyst/pipeline/model/transformation/transformation_block.py` & `epochalyst-0.3.3/epochalyst/pipeline/model/transformation/transformation_block.py`

 * *Files 4% similar despite different names*

```diff
@@ -69,14 +69,15 @@
             self.log_to_terminal(
                 f"Cache exists for {self.__class__} with hash: {self.get_hash()}. Using the cache.",
             )
             return self._get_cache(name=self.get_hash(), cache_args=cache_args)
 
         data = self.custom_transform(data, **transform_args)
         if cache_args:
+            self.log_to_terminal(f"Storing cache to {cache_args['storage_path']}")
             self._store_cache(name=self.get_hash(), data=data, cache_args=cache_args)
         return data
 
     @abstractmethod
     def custom_transform(self, data: Any, **transform_args: Any) -> Any:  # noqa: ANN401
         """Transform the input data using a custom method.
```

### Comparing `epochalyst-0.3.2/epochalyst.egg-info/PKG-INFO` & `epochalyst-0.3.3/epochalyst.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: epochalyst
-Version: 0.3.2
+Version: 0.3.3
 Summary: This package contains the code for team Epoch's pipeline
 Author-email: Jasper van Selm <jmvanselm@gmail.com>, Ariel Ebersberger <arielebersberger@gmail.com>, Tolga Kopar <cahittolgakopar@gmail.com>, Jeffrey Lim <jeffrey-lim@outlook.com>, Hugo de Heer <hugodeheer1234@gmail.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `epochalyst-0.3.2/epochalyst.egg-info/SOURCES.txt` & `epochalyst-0.3.3/epochalyst.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -27,10 +27,12 @@
 epochalyst/pipeline/model/training/training_block.py
 epochalyst/pipeline/model/training/augmentation/__init__.py
 epochalyst/pipeline/model/training/augmentation/image_augmentations.py
 epochalyst/pipeline/model/training/augmentation/time_series_augmentations.py
 epochalyst/pipeline/model/training/augmentation/utils.py
 epochalyst/pipeline/model/training/models/__init__.py
 epochalyst/pipeline/model/training/models/timm.py
+epochalyst/pipeline/model/training/utils/__init__.py
+epochalyst/pipeline/model/training/utils/tensor_functions.py
 epochalyst/pipeline/model/transformation/__init__.py
 epochalyst/pipeline/model/transformation/transformation.py
 epochalyst/pipeline/model/transformation/transformation_block.py
```

### Comparing `epochalyst-0.3.2/pyproject.toml` & `epochalyst-0.3.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "epochalyst"
-version = "0.3.2"
+version = "0.3.3"
 authors = [
     { name = "Jasper van Selm", email = "jmvanselm@gmail.com" },
     { name = "Ariel Ebersberger", email = "arielebersberger@gmail.com" },
     { name = "Tolga Kopar", email = "cahittolgakopar@gmail.com" },
     { name = "Jeffrey Lim", email = "jeffrey-lim@outlook.com" },
     { name = "Hugo de Heer", email = "hugodeheer1234@gmail.com"},
 ]
```

