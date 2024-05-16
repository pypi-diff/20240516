# Comparing `tmp/PixMClass-0.1.0.tar.gz` & `tmp/pixmclass-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PixMClass-0.1.0.tar", last modified: Fri Apr 12 15:49:38 2024, max compression
+gzip compressed data, was "pixmclass-0.1.1.tar", last modified: Thu May 16 15:32:30 2024, max compression
```

## Comparing `PixMClass-0.1.0.tar` & `pixmclass-0.1.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:49:38.435890 PixMClass-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     9227 2024-04-12 15:49:35.000000 PixMClass-0.1.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1559 2024-04-12 15:49:38.435890 PixMClass-0.1.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:49:38.435890 PixMClass-0.1.0/PixMClass.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1559 2024-04-12 15:49:38.000000 PixMClass-0.1.0/PixMClass.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      324 2024-04-12 15:49:38.000000 PixMClass-0.1.0/PixMClass.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 15:49:38.000000 PixMClass-0.1.0/PixMClass.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-12 15:49:38.000000 PixMClass-0.1.0/PixMClass.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-12 15:49:38.000000 PixMClass-0.1.0/PixMClass.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      597 2024-04-12 15:49:35.000000 PixMClass-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:49:38.435890 PixMClass-0.1.0/pix_mclass/
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-12 15:49:35.000000 PixMClass-0.1.0/pix_mclass/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2626 2024-04-12 15:49:35.000000 PixMClass-0.1.0/pix_mclass/callbacks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2513 2024-04-12 15:49:35.000000 PixMClass-0.1.0/pix_mclass/losses.py
--rw-r--r--   0 runner    (1001) docker     (127)     3898 2024-04-12 15:49:35.000000 PixMClass-0.1.0/pix_mclass/training.py
--rw-r--r--   0 runner    (1001) docker     (127)     4483 2024-04-12 15:49:35.000000 PixMClass-0.1.0/pix_mclass/unet.py
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-04-12 15:49:35.000000 PixMClass-0.1.0/pix_mclass/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 15:49:38.435890 PixMClass-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-04-12 15:49:35.000000 PixMClass-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 15:32:30.429533 pixmclass-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     9227 2024-05-16 15:32:25.000000 pixmclass-0.1.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1559 2024-05-16 15:32:30.425533 pixmclass-0.1.1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 15:32:30.425533 pixmclass-0.1.1/PixMClass.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1559 2024-05-16 15:32:30.000000 pixmclass-0.1.1/PixMClass.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-05-16 15:32:30.000000 pixmclass-0.1.1/PixMClass.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 15:32:30.000000 pixmclass-0.1.1/PixMClass.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-16 15:32:30.000000 pixmclass-0.1.1/PixMClass.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-16 15:32:30.000000 pixmclass-0.1.1/PixMClass.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-05-16 15:32:25.000000 pixmclass-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 15:32:30.425533 pixmclass-0.1.1/pix_mclass/
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-16 15:32:25.000000 pixmclass-0.1.1/pix_mclass/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2626 2024-05-16 15:32:25.000000 pixmclass-0.1.1/pix_mclass/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2513 2024-05-16 15:32:25.000000 pixmclass-0.1.1/pix_mclass/losses.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3964 2024-05-16 15:32:25.000000 pixmclass-0.1.1/pix_mclass/training.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4483 2024-05-16 15:32:25.000000 pixmclass-0.1.1/pix_mclass/unet.py
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-05-16 15:32:25.000000 pixmclass-0.1.1/pix_mclass/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 15:32:30.429533 pixmclass-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-05-16 15:32:25.000000 pixmclass-0.1.1/setup.py
```

### Comparing `PixMClass-0.1.0/LICENSE.txt` & `pixmclass-0.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `PixMClass-0.1.0/PKG-INFO` & `pixmclass-0.1.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: PixMClass
-Version: 0.1.0
+Version: 0.1.1
 Summary: Multiclass pixel classification
 Home-page: https://github.com/jeanollion/pix_mclass
-Download-URL: https://github.com/jeanollion/pix_mclass/releases/download/v0.1.0/pix_mclass-0.1.0.tar.gz
+Download-URL: https://github.com/jeanollion/pix_mclass/releases/download/v0.1.1/pix_mclass-0.1.1.tar.gz
 Author: Jean Ollion
 Author-email: jean.ollion@polytechnique.org
 Keywords: Segmentation,Classification,Microscopy,Cell
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Image Processing
```

### Comparing `PixMClass-0.1.0/PixMClass.egg-info/PKG-INFO` & `pixmclass-0.1.1/PixMClass.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: PixMClass
-Version: 0.1.0
+Version: 0.1.1
 Summary: Multiclass pixel classification
 Home-page: https://github.com/jeanollion/pix_mclass
-Download-URL: https://github.com/jeanollion/pix_mclass/releases/download/v0.1.0/pix_mclass-0.1.0.tar.gz
+Download-URL: https://github.com/jeanollion/pix_mclass/releases/download/v0.1.1/pix_mclass-0.1.1.tar.gz
 Author: Jean Ollion
 Author-email: jean.ollion@polytechnique.org
 Keywords: Segmentation,Classification,Microscopy,Cell
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Image Processing
```

### Comparing `PixMClass-0.1.0/README.md` & `pixmclass-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `PixMClass-0.1.0/pix_mclass/callbacks.py` & `pixmclass-0.1.1/pix_mclass/callbacks.py`

 * *Files identical despite different names*

### Comparing `PixMClass-0.1.0/pix_mclass/losses.py` & `pixmclass-0.1.1/pix_mclass/losses.py`

 * *Files identical despite different names*

### Comparing `PixMClass-0.1.0/pix_mclass/training.py` & `pixmclass-0.1.1/pix_mclass/training.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from .utils import ensure_multiplicity
 def get_iterator(
     dataset, scaling_data_generator, illumination_data_generator=None,
     input_channel_keywords="raw", class_keyword:str="classes", train_group_keyword:str=None,
     batch_size:int=16, step_number:int=0,
     tiling_parameters:dict = None,
     elasticdeform_parameters=None,
-    dtype="float32", shuffle:bool=True ):
+    dtype="float32", shuffle:bool=True, memory_persistent:bool=False):
 
     """Training Iterator.
 
     Parameters
     ----------
     dataset : either string or DatasetIO object
         if a string: path to .h5 file containing
@@ -65,11 +65,11 @@
                            image_data_generators = scaling_data_generator,
                            perform_data_augmentation=True,
                            elasticdeform_parameters=elasticdeform_parameters,
                            channels_postprocessing_function=pp_fun,
                            batch_size=batch_size,
                            incomplete_last_batch_mode="CONSTANT_SIZE",
                            shuffle=shuffle, step_number=step_number,
-                           dtype=dtype)
+                           dtype=dtype, memory_persistent=memory_persistent)
 
     train_it = MultiChannelIterator(**iterator_params)
     return train_it
```

### Comparing `PixMClass-0.1.0/pix_mclass/unet.py` & `pixmclass-0.1.1/pix_mclass/unet.py`

 * *Files identical despite different names*

### Comparing `PixMClass-0.1.0/setup.py` & `pixmclass-0.1.1/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="PixMClass",
-    version="0.1.0",
+    version="0.1.1",
     author="Jean Ollion",
     author_email="jean.ollion@polytechnique.org",
     description="Multiclass pixel classification",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/jeanollion/pix_mclass",
-    download_url='https://github.com/jeanollion/pix_mclass/releases/download/v0.1.0/pix_mclass-0.1.0.tar.gz',
+    download_url='https://github.com/jeanollion/pix_mclass/releases/download/v0.1.1/pix_mclass-0.1.1.tar.gz',
     packages=setuptools.find_packages(),
     keywords = ['Segmentation', 'Classification', 'Microscopy', 'Cell'],
     classifiers=[
         'Development Status :: 4 - Beta',
         'Intended Audience :: Science/Research',
         'Topic :: Scientific/Engineering :: Artificial Intelligence',
         'Topic :: Scientific/Engineering :: Image Processing',
```

