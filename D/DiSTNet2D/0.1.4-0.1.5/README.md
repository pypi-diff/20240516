# Comparing `tmp/distnet2d-0.1.4.tar.gz` & `tmp/distnet2d-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "distnet2d-0.1.4.tar", last modified: Mon Apr 29 15:52:10 2024, max compression
+gzip compressed data, was "distnet2d-0.1.5.tar", last modified: Wed May 15 21:36:41 2024, max compression
```

## Comparing `distnet2d-0.1.4.tar` & `distnet2d-0.1.5.tar`

### file list

```diff
@@ -1,35 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:52:10.694016 distnet2d-0.1.4/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:52:10.694016 distnet2d-0.1.4/DiSTNet2D.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2452 2024-04-29 15:52:10.000000 distnet2d-0.1.4/DiSTNet2D.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      781 2024-04-29 15:52:10.000000 distnet2d-0.1.4/DiSTNet2D.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 15:52:10.000000 distnet2d-0.1.4/DiSTNet2D.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-29 15:52:10.000000 distnet2d-0.1.4/DiSTNet2D.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-29 15:52:10.000000 distnet2d-0.1.4/DiSTNet2D.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-29 15:52:06.000000 distnet2d-0.1.4/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2452 2024-04-29 15:52:10.694016 distnet2d-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1410 2024-04-29 15:52:06.000000 distnet2d-0.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:52:10.690016 distnet2d-0.1.4/distnet_2d/
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-29 15:52:06.000000 distnet2d-0.1.4/distnet_2d/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:52:10.690016 distnet2d-0.1.4/distnet_2d/data/
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-29 15:52:06.000000 distnet2d-0.1.4/distnet_2d/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    34930 2024-04-29 15:52:06.000000 distnet2d-0.1.4/distnet_2d/data/dydx_iterator.py
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-04-29 15:52:06.000000 distnet2d-0.1.4/distnet_2d/data/medoid.py
--rw-r--r--   0 runner    (1001) docker     (127)     2353 2024-04-29 15:52:06.000000 distnet2d-0.1.4/distnet_2d/data/swim1d.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:52:10.690016 distnet2d-0.1.4/distnet_2d/model/
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-29 15:52:06.000000 distnet2d-0.1.4/distnet_2d/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10286 2024-04-29 15:52:06.000000 distnet2d-0.1.4/distnet_2d/model/architectures.py
--rw-r--r--   0 runner    (1001) docker     (127)    37691 2024-04-29 15:52:06.000000 distnet2d-0.1.4/distnet_2d/model/distnet_2d.py
--rw-r--r--   0 runner    (1001) docker     (127)    11193 2024-04-29 15:52:06.000000 distnet2d-0.1.4/distnet_2d/model/distnet_2d_seg.py
--rw-r--r--   0 runner    (1001) docker     (127)     2589 2024-04-29 15:52:06.000000 distnet2d-0.1.4/distnet_2d/model/gradient_accumulator.py
--rw-r--r--   0 runner    (1001) docker     (127)    25438 2024-04-29 15:52:06.000000 distnet2d-0.1.4/distnet_2d/model/layers.py
--rw-r--r--   0 runner    (1001) docker     (127)     5026 2024-04-29 15:52:06.000000 distnet2d-0.1.4/distnet_2d/model/spatial_attention.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:52:10.694016 distnet2d-0.1.4/distnet_2d/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      240 2024-04-29 15:52:06.000000 distnet2d-0.1.4/distnet_2d/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2891 2024-04-29 15:52:06.000000 distnet2d-0.1.4/distnet_2d/utils/agc.py
--rw-r--r--   0 runner    (1001) docker     (127)     5222 2024-04-29 15:52:06.000000 distnet2d-0.1.4/distnet_2d/utils/callbacks.py
--rw-r--r--   0 runner    (1001) docker     (127)     3019 2024-04-29 15:52:06.000000 distnet2d-0.1.4/distnet_2d/utils/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     4097 2024-04-29 15:52:06.000000 distnet2d-0.1.4/distnet_2d/utils/losses.py
--rw-r--r--   0 runner    (1001) docker     (127)     4691 2024-04-29 15:52:06.000000 distnet2d-0.1.4/distnet_2d/utils/lovasz_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)    12536 2024-04-29 15:52:06.000000 distnet2d-0.1.4/distnet_2d/utils/objectwise_computation_tf.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 15:52:10.694016 distnet2d-0.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-04-29 15:52:06.000000 distnet2d-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:36:41.162781 distnet2d-0.1.5/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:36:41.162781 distnet2d-0.1.5/DiSTNet2D.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2452 2024-05-15 21:36:41.000000 distnet2d-0.1.5/DiSTNet2D.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      812 2024-05-15 21:36:41.000000 distnet2d-0.1.5/DiSTNet2D.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 21:36:41.000000 distnet2d-0.1.5/DiSTNet2D.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-15 21:36:41.000000 distnet2d-0.1.5/DiSTNet2D.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-15 21:36:41.000000 distnet2d-0.1.5/DiSTNet2D.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-15 21:36:33.000000 distnet2d-0.1.5/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2452 2024-05-15 21:36:41.162781 distnet2d-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1410 2024-05-15 21:36:33.000000 distnet2d-0.1.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:36:41.158781 distnet2d-0.1.5/distnet_2d/
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-15 21:36:33.000000 distnet2d-0.1.5/distnet_2d/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:36:41.158781 distnet2d-0.1.5/distnet_2d/data/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-15 21:36:33.000000 distnet2d-0.1.5/distnet_2d/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34930 2024-05-15 21:36:33.000000 distnet2d-0.1.5/distnet_2d/data/dydx_iterator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-15 21:36:33.000000 distnet2d-0.1.5/distnet_2d/data/medoid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2353 2024-05-15 21:36:33.000000 distnet2d-0.1.5/distnet_2d/data/swim1d.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:36:41.162781 distnet2d-0.1.5/distnet_2d/model/
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-15 21:36:33.000000 distnet2d-0.1.5/distnet_2d/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10286 2024-05-15 21:36:33.000000 distnet2d-0.1.5/distnet_2d/model/architectures.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37691 2024-05-15 21:36:33.000000 distnet2d-0.1.5/distnet_2d/model/distnet_2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11193 2024-05-15 21:36:33.000000 distnet2d-0.1.5/distnet_2d/model/distnet_2d_seg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2589 2024-05-15 21:36:33.000000 distnet2d-0.1.5/distnet_2d/model/gradient_accumulator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25438 2024-05-15 21:36:33.000000 distnet2d-0.1.5/distnet_2d/model/layers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5026 2024-05-15 21:36:33.000000 distnet2d-0.1.5/distnet_2d/model/spatial_attention.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:36:41.162781 distnet2d-0.1.5/distnet_2d/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-05-15 21:36:33.000000 distnet2d-0.1.5/distnet_2d/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2891 2024-05-15 21:36:33.000000 distnet2d-0.1.5/distnet_2d/utils/agc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5322 2024-05-15 21:36:33.000000 distnet2d-0.1.5/distnet_2d/utils/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3019 2024-05-15 21:36:33.000000 distnet2d-0.1.5/distnet_2d/utils/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4097 2024-05-15 21:36:33.000000 distnet2d-0.1.5/distnet_2d/utils/losses.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4691 2024-05-15 21:36:33.000000 distnet2d-0.1.5/distnet_2d/utils/lovasz_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5711 2024-05-15 21:36:33.000000 distnet2d-0.1.5/distnet_2d/utils/metrics_tf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9907 2024-05-15 21:36:33.000000 distnet2d-0.1.5/distnet_2d/utils/objectwise_computation_tf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 21:36:41.162781 distnet2d-0.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-05-15 21:36:33.000000 distnet2d-0.1.5/setup.py
```

### Comparing `distnet2d-0.1.4/DiSTNet2D.egg-info/PKG-INFO` & `distnet2d-0.1.5/DiSTNet2D.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: DiSTNet2D
-Version: 0.1.4
+Version: 0.1.5
 Summary: tensorflow/keras implementation of DiSTNet 2D
 Home-page: https://github.com/jeanollion/distnet2d
-Download-URL: https://github.com/jeanollion/distnet2d/releases/download/v0.1.4/distnet2d-0.1.4.tar.gz
+Download-URL: https://github.com/jeanollion/distnet2d/releases/download/v0.1.5/distnet2d-0.1.5.tar.gz
 Author: Jean Ollion
 Author-email: jean.ollion@polytechnique.org
 Keywords: Segmentation,Tracking,Cell,Tensorflow,Keras
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Image Processing
```

### Comparing `distnet2d-0.1.4/DiSTNet2D.egg-info/SOURCES.txt` & `distnet2d-0.1.5/DiSTNet2D.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -20,8 +20,9 @@
 distnet_2d/model/spatial_attention.py
 distnet_2d/utils/__init__.py
 distnet_2d/utils/agc.py
 distnet_2d/utils/callbacks.py
 distnet_2d/utils/helpers.py
 distnet_2d/utils/losses.py
 distnet_2d/utils/lovasz_loss.py
+distnet_2d/utils/metrics_tf.py
 distnet_2d/utils/objectwise_computation_tf.py
```

### Comparing `distnet2d-0.1.4/LICENSE.txt` & `distnet2d-0.1.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `distnet2d-0.1.4/PKG-INFO` & `distnet2d-0.1.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: DiSTNet2D
-Version: 0.1.4
+Version: 0.1.5
 Summary: tensorflow/keras implementation of DiSTNet 2D
 Home-page: https://github.com/jeanollion/distnet2d
-Download-URL: https://github.com/jeanollion/distnet2d/releases/download/v0.1.4/distnet2d-0.1.4.tar.gz
+Download-URL: https://github.com/jeanollion/distnet2d/releases/download/v0.1.5/distnet2d-0.1.5.tar.gz
 Author: Jean Ollion
 Author-email: jean.ollion@polytechnique.org
 Keywords: Segmentation,Tracking,Cell,Tensorflow,Keras
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Image Processing
```

### Comparing `distnet2d-0.1.4/README.md` & `distnet2d-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `distnet2d-0.1.4/distnet_2d/data/dydx_iterator.py` & `distnet2d-0.1.5/distnet_2d/data/dydx_iterator.py`

 * *Files identical despite different names*

### Comparing `distnet2d-0.1.4/distnet_2d/data/swim1d.py` & `distnet2d-0.1.5/distnet_2d/data/swim1d.py`

 * *Files identical despite different names*

### Comparing `distnet2d-0.1.4/distnet_2d/model/architectures.py` & `distnet2d-0.1.5/distnet_2d/model/architectures.py`

 * *Files identical despite different names*

### Comparing `distnet2d-0.1.4/distnet_2d/model/distnet_2d.py` & `distnet2d-0.1.5/distnet_2d/model/distnet_2d.py`

 * *Files identical despite different names*

### Comparing `distnet2d-0.1.4/distnet_2d/model/distnet_2d_seg.py` & `distnet2d-0.1.5/distnet_2d/model/distnet_2d_seg.py`

 * *Files identical despite different names*

### Comparing `distnet2d-0.1.4/distnet_2d/model/gradient_accumulator.py` & `distnet2d-0.1.5/distnet_2d/model/gradient_accumulator.py`

 * *Files identical despite different names*

### Comparing `distnet2d-0.1.4/distnet_2d/model/layers.py` & `distnet2d-0.1.5/distnet_2d/model/layers.py`

 * *Files identical despite different names*

### Comparing `distnet2d-0.1.4/distnet_2d/model/spatial_attention.py` & `distnet2d-0.1.5/distnet_2d/model/spatial_attention.py`

 * *Files identical despite different names*

### Comparing `distnet2d-0.1.4/distnet_2d/utils/agc.py` & `distnet2d-0.1.5/distnet_2d/utils/agc.py`

 * *Files identical despite different names*

### Comparing `distnet2d-0.1.4/distnet_2d/utils/callbacks.py` & `distnet2d-0.1.5/distnet_2d/utils/callbacks.py`

 * *Files 4% similar despite different names*

```diff
@@ -57,24 +57,27 @@
             path = self._tmp_path(path)
         return path
 
     def _tmp_path(self, path):
         split = os.path.splitext(path)
         return split[0] + "_tmp" + split[1]
 
+
 class StopOnLR(Callback):
     def __init__( self, min_lr, **kwargs, ):
         super().__init__()
         self.min_lr = min_lr
 
-    def on_epoch_end(self, epoch, logs={}):
+    def on_epoch_end(self, epoch, logs=None):
         lr = backend.get_value(self.model.optimizer.lr)
-        if(lr <= self.min_lr):
+        if lr <= self.min_lr:
+            print(f"Learning rate {lr} <= {self.min_lr} : training will be stopped", flush=True)
             self.model.stop_training = True
 
+
 class EpsilonCosineDecayCallback(Callback):
     """Reduce optimizer epsilon parameter.
     Args:
       factor: factor by which epsilon will be reduced.
         `new_epsilon = epsilon * factor`.
       period: number of epochs after which epsilon will be reduced.
       verbose: int. 0: quiet, 1: update messages.
```

### Comparing `distnet2d-0.1.4/distnet_2d/utils/helpers.py` & `distnet2d-0.1.5/distnet_2d/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `distnet2d-0.1.4/distnet_2d/utils/losses.py` & `distnet2d-0.1.5/distnet_2d/utils/losses.py`

 * *Files identical despite different names*

### Comparing `distnet2d-0.1.4/distnet_2d/utils/lovasz_loss.py` & `distnet2d-0.1.5/distnet_2d/utils/lovasz_loss.py`

 * *Files identical despite different names*

### Comparing `distnet2d-0.1.4/setup.py` & `distnet2d-0.1.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="DiSTNet2D",
-    version="0.1.4",
+    version="0.1.5",
     author="Jean Ollion",
     author_email="jean.ollion@polytechnique.org",
     description="tensorflow/keras implementation of DiSTNet 2D",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/jeanollion/distnet2d",
-    download_url='https://github.com/jeanollion/distnet2d/releases/download/v0.1.4/distnet2d-0.1.4.tar.gz',
+    download_url='https://github.com/jeanollion/distnet2d/releases/download/v0.1.5/distnet2d-0.1.5.tar.gz',
     packages=setuptools.find_packages(),
     keywords=['Segmentation', 'Tracking', 'Cell', 'Tensorflow', 'Keras'],
     classifiers=[
         'Development Status :: 4 - Beta',
         'Intended Audience :: Science/Research',
         'Topic :: Scientific/Engineering :: Artificial Intelligence',
         'Topic :: Scientific/Engineering :: Image Processing',
```

