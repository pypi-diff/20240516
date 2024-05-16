# Comparing `tmp/dataset_iterator-0.4.3.tar.gz` & `tmp/dataset_iterator-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dataset_iterator-0.4.3.tar", last modified: Fri May  3 22:15:51 2024, max compression
+gzip compressed data, was "dataset_iterator-0.4.4.tar", last modified: Thu May 16 15:35:04 2024, max compression
```

## Comparing `dataset_iterator-0.4.3.tar` & `dataset_iterator-0.4.4.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 22:15:51.448933 dataset_iterator-0.4.3/
--rw-r--r--   0 runner    (1001) docker     (127)    10141 2024-05-03 22:15:47.000000 dataset_iterator-0.4.3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3603 2024-05-03 22:15:51.448933 dataset_iterator-0.4.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2412 2024-05-03 22:15:47.000000 dataset_iterator-0.4.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 22:15:51.444933 dataset_iterator-0.4.3/dataset_iterator/
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-05-03 22:15:47.000000 dataset_iterator-0.4.3/dataset_iterator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6747 2024-05-03 22:15:47.000000 dataset_iterator-0.4.3/dataset_iterator/concat_iterator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 22:15:51.448933 dataset_iterator-0.4.3/dataset_iterator/datasetIO/
--rw-r--r--   0 runner    (1001) docker     (127)      320 2024-05-03 22:15:47.000000 dataset_iterator-0.4.3/dataset_iterator/datasetIO/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-05-03 22:15:47.000000 dataset_iterator-0.4.3/dataset_iterator/datasetIO/concatenate_datasetIO.py
--rw-r--r--   0 runner    (1001) docker     (127)     1801 2024-05-03 22:15:47.000000 dataset_iterator-0.4.3/dataset_iterator/datasetIO/datasetIO.py
--rw-r--r--   0 runner    (1001) docker     (127)     3011 2024-05-03 22:15:47.000000 dataset_iterator-0.4.3/dataset_iterator/datasetIO/group_datasetIO.py
--rw-r--r--   0 runner    (1001) docker     (127)     2951 2024-05-03 22:15:47.000000 dataset_iterator-0.4.3/dataset_iterator/datasetIO/h5pyIO.py
--rw-r--r--   0 runner    (1001) docker     (127)     4338 2024-05-03 22:15:47.000000 dataset_iterator-0.4.3/dataset_iterator/datasetIO/memoryIO.py
--rw-r--r--   0 runner    (1001) docker     (127)     3632 2024-05-03 22:15:47.000000 dataset_iterator-0.4.3/dataset_iterator/datasetIO/multiple_datasetIO.py
--rw-r--r--   0 runner    (1001) docker     (127)    15378 2024-05-03 22:15:47.000000 dataset_iterator-0.4.3/dataset_iterator/datasetIO/multiple_fileIO.py
--rw-r--r--   0 runner    (1001) docker     (127)    11884 2024-05-03 22:15:47.000000 dataset_iterator-0.4.3/dataset_iterator/hard_sample_mining.py
--rw-r--r--   0 runner    (1001) docker     (127)    11687 2024-05-03 22:15:47.000000 dataset_iterator-0.4.3/dataset_iterator/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)    20472 2024-05-03 22:15:47.000000 dataset_iterator-0.4.3/dataset_iterator/image_data_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     5433 2024-05-03 22:15:47.000000 dataset_iterator-0.4.3/dataset_iterator/index_array_iterator.py
--rw-r--r--   0 runner    (1001) docker     (127)    58005 2024-05-03 22:15:47.000000 dataset_iterator-0.4.3/dataset_iterator/multichannel_iterator.py
--rw-r--r--   0 runner    (1001) docker     (127)     7528 2024-05-03 22:15:47.000000 dataset_iterator-0.4.3/dataset_iterator/ordered_enqueuer_cf.py
--rw-r--r--   0 runner    (1001) docker     (127)    13972 2024-05-03 22:15:47.000000 dataset_iterator-0.4.3/dataset_iterator/pre_processing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3656 2024-05-03 22:15:47.000000 dataset_iterator-0.4.3/dataset_iterator/shared_memory.py
--rw-r--r--   0 runner    (1001) docker     (127)    22835 2024-05-03 22:15:47.000000 dataset_iterator-0.4.3/dataset_iterator/tile_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    12642 2024-05-03 22:15:47.000000 dataset_iterator-0.4.3/dataset_iterator/tracking_iterator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2901 2024-05-03 22:15:47.000000 dataset_iterator-0.4.3/dataset_iterator/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 22:15:51.448933 dataset_iterator-0.4.3/dataset_iterator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3603 2024-05-03 22:15:51.000000 dataset_iterator-0.4.3/dataset_iterator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1037 2024-05-03 22:15:51.000000 dataset_iterator-0.4.3/dataset_iterator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 22:15:51.000000 dataset_iterator-0.4.3/dataset_iterator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-03 22:15:51.000000 dataset_iterator-0.4.3/dataset_iterator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-03 22:15:51.000000 dataset_iterator-0.4.3/dataset_iterator.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 22:15:51.448933 dataset_iterator-0.4.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1391 2024-05-03 22:15:47.000000 dataset_iterator-0.4.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 15:35:04.775952 dataset_iterator-0.4.4/
+-rw-r--r--   0 runner    (1001) docker     (127)    10141 2024-05-16 15:35:01.000000 dataset_iterator-0.4.4/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3603 2024-05-16 15:35:04.775952 dataset_iterator-0.4.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2412 2024-05-16 15:35:01.000000 dataset_iterator-0.4.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 15:35:04.775952 dataset_iterator-0.4.4/dataset_iterator/
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-05-16 15:35:01.000000 dataset_iterator-0.4.4/dataset_iterator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6747 2024-05-16 15:35:01.000000 dataset_iterator-0.4.4/dataset_iterator/concat_iterator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 15:35:04.775952 dataset_iterator-0.4.4/dataset_iterator/datasetIO/
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-05-16 15:35:01.000000 dataset_iterator-0.4.4/dataset_iterator/datasetIO/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-05-16 15:35:01.000000 dataset_iterator-0.4.4/dataset_iterator/datasetIO/concatenate_datasetIO.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1801 2024-05-16 15:35:01.000000 dataset_iterator-0.4.4/dataset_iterator/datasetIO/datasetIO.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3011 2024-05-16 15:35:01.000000 dataset_iterator-0.4.4/dataset_iterator/datasetIO/group_datasetIO.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2951 2024-05-16 15:35:01.000000 dataset_iterator-0.4.4/dataset_iterator/datasetIO/h5pyIO.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2677 2024-05-16 15:35:01.000000 dataset_iterator-0.4.4/dataset_iterator/datasetIO/memoryIO.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3632 2024-05-16 15:35:01.000000 dataset_iterator-0.4.4/dataset_iterator/datasetIO/multiple_datasetIO.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15378 2024-05-16 15:35:01.000000 dataset_iterator-0.4.4/dataset_iterator/datasetIO/multiple_fileIO.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11374 2024-05-16 15:35:01.000000 dataset_iterator-0.4.4/dataset_iterator/hard_sample_mining.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11687 2024-05-16 15:35:01.000000 dataset_iterator-0.4.4/dataset_iterator/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22252 2024-05-16 15:35:01.000000 dataset_iterator-0.4.4/dataset_iterator/image_data_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5433 2024-05-16 15:35:01.000000 dataset_iterator-0.4.4/dataset_iterator/index_array_iterator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    57901 2024-05-16 15:35:01.000000 dataset_iterator-0.4.4/dataset_iterator/multichannel_iterator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7487 2024-05-16 15:35:01.000000 dataset_iterator-0.4.4/dataset_iterator/ordered_enqueuer_cf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13972 2024-05-16 15:35:01.000000 dataset_iterator-0.4.4/dataset_iterator/pre_processing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3972 2024-05-16 15:35:01.000000 dataset_iterator-0.4.4/dataset_iterator/shared_memory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22835 2024-05-16 15:35:01.000000 dataset_iterator-0.4.4/dataset_iterator/tile_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12642 2024-05-16 15:35:01.000000 dataset_iterator-0.4.4/dataset_iterator/tracking_iterator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2901 2024-05-16 15:35:01.000000 dataset_iterator-0.4.4/dataset_iterator/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 15:35:04.775952 dataset_iterator-0.4.4/dataset_iterator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3603 2024-05-16 15:35:04.000000 dataset_iterator-0.4.4/dataset_iterator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1037 2024-05-16 15:35:04.000000 dataset_iterator-0.4.4/dataset_iterator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 15:35:04.000000 dataset_iterator-0.4.4/dataset_iterator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-16 15:35:04.000000 dataset_iterator-0.4.4/dataset_iterator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-16 15:35:04.000000 dataset_iterator-0.4.4/dataset_iterator.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 15:35:04.775952 dataset_iterator-0.4.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1391 2024-05-16 15:35:01.000000 dataset_iterator-0.4.4/setup.py
```

### Comparing `dataset_iterator-0.4.3/LICENSE.txt` & `dataset_iterator-0.4.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dataset_iterator-0.4.3/PKG-INFO` & `dataset_iterator-0.4.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: dataset_iterator
-Version: 0.4.3
+Version: 0.4.4
 Summary: Keras-style data iterator for images contained in dataset files such as hdf5 or PIL readable files. Images can be contained in several files.
 Home-page: https://github.com/jeanollion/dataset_iterator.git
-Download-URL: https://github.com/jeanollion/dataset_iterator/releases/download/v0.4.3/dataset_iterator-0.4.3.tar.gz
+Download-URL: https://github.com/jeanollion/dataset_iterator/releases/download/v0.4.4/dataset_iterator-0.4.4.tar.gz
 Author: Jean Ollion
 Author-email: jean.ollion@polytechnique.org
 Keywords: Iterator,Dataset,Image,Numpy
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Image Processing
```

### Comparing `dataset_iterator-0.4.3/README.md` & `dataset_iterator-0.4.4/README.md`

 * *Files identical despite different names*

### Comparing `dataset_iterator-0.4.3/dataset_iterator/__init__.py` & `dataset_iterator-0.4.4/dataset_iterator/__init__.py`

 * *Files identical despite different names*

### Comparing `dataset_iterator-0.4.3/dataset_iterator/concat_iterator.py` & `dataset_iterator-0.4.4/dataset_iterator/concat_iterator.py`

 * *Files identical despite different names*

### Comparing `dataset_iterator-0.4.3/dataset_iterator/datasetIO/concatenate_datasetIO.py` & `dataset_iterator-0.4.4/dataset_iterator/datasetIO/concatenate_datasetIO.py`

 * *Files identical despite different names*

### Comparing `dataset_iterator-0.4.3/dataset_iterator/datasetIO/datasetIO.py` & `dataset_iterator-0.4.4/dataset_iterator/datasetIO/datasetIO.py`

 * *Files identical despite different names*

### Comparing `dataset_iterator-0.4.3/dataset_iterator/datasetIO/group_datasetIO.py` & `dataset_iterator-0.4.4/dataset_iterator/datasetIO/group_datasetIO.py`

 * *Files identical despite different names*

### Comparing `dataset_iterator-0.4.3/dataset_iterator/datasetIO/h5pyIO.py` & `dataset_iterator-0.4.4/dataset_iterator/datasetIO/h5pyIO.py`

 * *Files identical despite different names*

### Comparing `dataset_iterator-0.4.3/dataset_iterator/datasetIO/multiple_datasetIO.py` & `dataset_iterator-0.4.4/dataset_iterator/datasetIO/multiple_datasetIO.py`

 * *Files identical despite different names*

### Comparing `dataset_iterator-0.4.3/dataset_iterator/datasetIO/multiple_fileIO.py` & `dataset_iterator-0.4.4/dataset_iterator/datasetIO/multiple_fileIO.py`

 * *Files identical despite different names*

### Comparing `dataset_iterator-0.4.3/dataset_iterator/hard_sample_mining.py` & `dataset_iterator-0.4.4/dataset_iterator/hard_sample_mining.py`

 * *Files 3% similar despite different names*

```diff
@@ -44,21 +44,19 @@
 
     def on_epoch_begin(self, epoch, logs=None):
         if self.proba_per_metric is not None or self.need_compute(epoch):
             self.wait_for_me.clear()  # will lock
 
     def on_epoch_end(self, epoch, logs=None):
         if self.need_compute(epoch):
-            if self.target_iterator is not self.iterator:
-                self.target_iterator.close()
-                self.iterator.open()
+            self.target_iterator.close()
+            self.iterator.open()
             metrics = self.compute_metrics()
-            if self.target_iterator is not self.iterator:
-                self.iterator.close()
-                self.target_iterator.open()
+            self.iterator.close()
+            self.target_iterator.open()
             first = self.proba_per_metric is None
             self.proba_per_metric = get_index_probability(metrics, enrich_factor=self.enrich_factor, quantile_max=self.quantile_max, quantile_min=self.quantile_min, verbose=self.verbose)
             self.n_metrics = self.proba_per_metric.shape[0] if len(self.proba_per_metric.shape) == 2 else 1
             if first and self.n_metrics > self.period:
                 warnings.warn(f"Hard sample mining period = {self.period} should be greater than metric number = {self.n_metrics}")
         if self.proba_per_metric is not None:
             if len(self.proba_per_metric.shape) == 2:
@@ -73,28 +71,16 @@
         self.close()
 
     def compute_metrics(self):
         workers = os.cpu_count() if self.workers is None else self.workers
         self.enq.start(workers=workers, max_queue_size=max(2, min(self.n_batches, workers)))
         gen = self.enq.get()
         compute_metrics_fun = get_compute_metrics_fun(self.predict_fun, self.metrics_fun, self.batch_size)
-        computed = False
-        metrics = None
-        while not computed:
-            try:
-                metrics = compute_metrics_loop(compute_metrics_fun, gen, self.batch_size, self.n_batches, self.verbose)
-            except BrokenPipeError as e:
-                print("broken pipe error, will re-try metric computation")
-                self.enq.stop()
-                self.enq.start(workers=workers, max_queue_size=max(2, min(self.n_batches, workers)))
-                gen = self.enq.get()
-            else:
-                computed = True
+        metrics = compute_metrics_loop(compute_metrics_fun, gen, self.batch_size, self.n_batches, self.verbose)
         self.enq.stop()
-        #self.iterator.close()
         return metrics
 
 
 def get_index_probability_1d(metric, enrich_factor:float=10., quantile_min:float=0.01, quantile_max:float=None, max_power:int=10, power_accuracy:float=0.1, verbose:int=1):
     assert 0.5 > quantile_min >= 0, f"invalid min quantile: {quantile_min}"
     if 1. / enrich_factor < quantile_min: # incompatible enrich factor and quantile
         quantile_min = 1. / enrich_factor
@@ -105,15 +91,15 @@
 
     Nh = metric[metric <= metric_quantiles[0]].shape[0] # hard examples (low metric)
     Ne = metric[metric >= metric_quantiles[1]].shape[0] # easy examples (high metric)
     metric_sub = metric[(metric < metric_quantiles[1]) & (metric > metric_quantiles[0])]
     Nm = metric_sub.shape[0]
     S = np.sum( ((metric_sub - metric_quantiles[1]) / (metric_quantiles[0] - metric_quantiles[1])) )
     p_max = enrich_factor / metric.shape[0]
-    p_min = (1 - p_max * (Nh + S)) / (Nm + Ne - S) if (Nm + Ne - S)!=0 else -1
+    p_min = (1 - p_max * (Nh + S)) / (Nm + Ne - S) if (Nm + Ne - S) != 0 else -1
     if p_min<0:
         p_min = 0.
         target = 1./p_max - Nh
         if target <= 0: # cannot reach enrich factor: too many hard examples
             power = max_power
         else:
             fun = lambda power_: np.sum(((metric_sub - metric_quantiles[1]) / (metric_quantiles[0] - metric_quantiles[1])) ** power_)
@@ -150,37 +136,39 @@
     probas_per_metric = [get_index_probability_1d(metrics[:, i], enrich_factor=enrich_factor, quantile_max=quantile_max, quantile_min=quantile_min, verbose=verbose) for i in range(metrics.shape[1])]
     probas_per_metric = np.stack(probas_per_metric, axis=0)
     #proba = np.max(probas_per_metric, axis=0)
     #proba /= np.sum(proba)
     return probas_per_metric
 
 def compute_metrics(iterator, predict_function, metrics_function, disable_augmentation:bool=True, disable_channel_postprocessing:bool=False, workers:int=None, verbose:int=1):
+    iterator.open()
     data_aug_param = iterator.disable_random_transforms(disable_augmentation, disable_channel_postprocessing)
     simple_iterator = SimpleIterator(iterator)
     batch_size = iterator.get_batch_size()
     n_batches = len(simple_iterator)
 
     compute_metrics_fun = get_compute_metrics_fun(predict_function, metrics_function, batch_size)
-
     if workers is None:
         workers = os.cpu_count()
-    #enq = tf.keras.utils.OrderedEnqueuer(simple_iterator, use_multiprocessing=True, shuffle=False)
-    enq = OrderedEnqueuerCF(simple_iterator, single_epoch=True, shuffle=False)
+    enq = OrderedEnqueuerCF(simple_iterator, single_epoch=True, shuffle=False, use_shm=True)
     enq.start(workers=workers, max_queue_size=max(3, min(n_batches, workers)))
     gen = enq.get()
     metrics = compute_metrics_loop(compute_metrics_fun, gen, batch_size, n_batches, verbose)
     enq.stop()
     if data_aug_param is not None:
         iterator.enable_random_transforms(data_aug_param)
     iterator.close()
+    #for i in range(metrics.shape[1]):
+    #    print(f"metric: range: [{np.min(metrics[:,i])}, {np.max(metrics[:,i])}] mean: {np.mean(metrics[:,i])}")
     return metrics
 
+
 def compute_metrics_loop(compute_metrics_fun, gen, batch_size, n_batches, verbose):
     metrics = []
-    if verbose>=1:
+    if verbose >= 1:
         print(f"Hard Sample Mining: computing metrics...", flush=True)
         progbar = tf.keras.utils.Progbar(n_batches)
     n_tiles = None
     for i in range(n_batches):
         x, y_true = next(gen)
         batch_metrics = compute_metrics_fun(x, y_true)
         if x.shape[0] > batch_size or n_tiles is not None:  # tiling: keep hardest tile per sample
```

### Comparing `dataset_iterator-0.4.3/dataset_iterator/helpers.py` & `dataset_iterator-0.4.4/dataset_iterator/helpers.py`

 * *Files identical despite different names*

### Comparing `dataset_iterator-0.4.3/dataset_iterator/image_data_generator.py` & `dataset_iterator-0.4.4/dataset_iterator/image_data_generator.py`

 * *Files 9% similar despite different names*

```diff
@@ -359,16 +359,46 @@
 
 class KerasImageDataGenerator(tf.keras.preprocessing.image.ImageDataGenerator):
     def __init__(self, **kwargs):
         if "interpolation_order" in kwargs: # interpolation_order was introduced at version 2.9.0
             tf_version = get_tf_version()
             if tf_version < (2,9,0):
                 kwargs.pop("interpolation_order")
+        if "height_shift_range" in kwargs:
+            self.x_shift_range = kwargs.pop("height_shift_range")
+            if self.x_shift_range is not None:
+                if isinstance(self.x_shift_range, (tuple, list)):
+                    assert len(self.x_shift_range) == 2, "height_shift_range should either be a number either a list or tuple of len 2"
+                else:
+                    self.x_shift_range = [-self.x_shift_range, self.x_shift_range]
+        else:
+            self.x_shift_range = None
+        if "width_shift_range" in kwargs:
+            self.y_shift_range = kwargs.pop("width_shift_range")
+            if self.y_shift_range is not None:
+                if isinstance(self.y_shift_range, (tuple, list)):
+                    assert len(self.y_shift_range) == 2, "width_shift_range should either be a number either a list or tuple of len 2"
+                else:
+                    self.y_shift_range = [-self.y_shift_range, self.y_shift_range]
+        else:
+            self.y_shift_range = None
         super().__init__(**kwargs)
 
+    def get_random_transform(self, img_shape, seed=None):
+        random_transform = super().get_random_transform(img_shape, seed)
+        if self.x_shift_range is not None:
+            random_transform["tx"] = np.random.uniform(self.x_shift_range[0], self.x_shift_range[1])
+            if np.max(np.abs(self.x_shift_range)) < 1:
+                random_transform["tx"] = random_transform["tx"] * img_shape[self.row_axis - 1]
+        if self.y_shift_range is not None:
+            random_transform["ty"] = -np.random.uniform(self.y_shift_range[0], self.y_shift_range[1])
+            if np.max(np.abs(self.y_shift_range)) < 1:
+                random_transform["ty"] = random_transform["ty"] * img_shape[self.col_axis - 1]
+        return random_transform
+
     def transfer_parameters(self, source, destination):
         destination['flip_vertical'] = source.get('flip_vertical', False)
         destination['flip_horizontal'] = source.get('flip_horizontal', False)
         destination['zy'] = source.get('zy', 1)
         destination['zx'] = source.get('zx', 1)
         destination['shear'] = source.get('shear', 0)
         if 'brightness' in source:
```

### Comparing `dataset_iterator-0.4.3/dataset_iterator/index_array_iterator.py` & `dataset_iterator-0.4.4/dataset_iterator/index_array_iterator.py`

 * *Files identical despite different names*

### Comparing `dataset_iterator-0.4.3/dataset_iterator/multichannel_iterator.py` & `dataset_iterator-0.4.4/dataset_iterator/multichannel_iterator.py`

 * *Files 0% similar despite different names*

```diff
@@ -167,18 +167,19 @@
                  shuffle=True,
                  perform_data_augmentation=True,
                  elasticdeform_parameters=None,
                  return_image_index:bool = False,
                  seed=None,
                  dtype='float32',
                  convert_masks_to_dtype=True,
-                 memory_persistant=False,
+                 memory_persistent=False,
                  incomplete_last_batch_mode=INCOMPLETE_LAST_BATCH_MODE[1]):
         self.dataset = dataset
-        self.memory_persistant=memory_persistant
+        self.datasetIO = None
+        self.memory_persistent=memory_persistent
         self.n_spatial_dims=n_spatial_dims
         self.group_keyword=group_keyword
         self.group_proportion=group_proportion
         self.group_proportion_init=False
         if group_proportion is not None:
             assert group_keyword is not None and isinstance(group_keyword, (tuple, list)) and isinstance(group_proportion, (tuple, list)) and len(group_proportion)==len(group_keyword), "when group_proportion is not None, group_keyword should be a list/tuple group_proportion should be of same length as group_keyword"
         self.channel_keywords=channel_keywords
@@ -282,31 +283,33 @@
             if len(self.labels)!=len(self.ds_array[0]):
                 raise ValueError('Invalid input file: number of label array differ from dataset number')
             if any(len(self.labels[i].shape)==0 or len(self.labels[i]) != len(self.ds_array[0][i]) for i in range(len(self.labels))):
                 raise ValueError('Invalid input file: at least one dataset has element numbers that differ from corresponding label array')
         except:
             self.labels = None
 
-        if not memory_persistant:
-            self._close_datasetIO()
+        #if not memory_persistant:
+        #    self._close_datasetIO()
         self.void_mask_proportion = void_mask_proportion
         if self.void_mask_proportion is not None:
             assert self.group_proportion is None, "cannot define void mask proportion and group proportion simultaneously"
             assert len(void_mask_proportion) == 2 and void_mask_proportion[0]<=void_mask_proportion[1] and void_mask_proportion[0]>=0 and void_mask_proportion[1]<=1, "invalid void_mask_proportion must be a proportion range"
             assert len(mask_channels)>0, "mask channels must be defined if void mask proportion is defined"
         if len(mask_channels)>0:
             self.void_mask_chan = mask_channels[0]
         else:
             self.void_mask_chan=-1
         self.total_n = indexes[-1]
         super().__init__(self.total_n, batch_size, shuffle, seed, incomplete_last_batch_mode, step_number=step_number)
 
     def _open_datasetIO(self):
+        if self.datasetIO is not None:
+            self.datasetIO.close()
         self.datasetIO = get_datasetIO(self.dataset, 'r')
-        if self.memory_persistant:
+        if self.memory_persistent:
             self.datasetIO = MemoryIO(self.datasetIO)
         if self.paths is None:
             self.group_map_paths = dict()
             group_list = self.group_keyword if isinstance(self.group_keyword, (list, tuple)) else [self.group_keyword]
             for k in group_list:
                 # get all dataset paths
                 paths = self.datasetIO.get_dataset_paths(self.channel_keywords[0], k)
@@ -318,16 +321,16 @@
         self.ds_array = [ [self.datasetIO.get_dataset(self._get_dataset_path(c, ds_idx)) for ds_idx in range(len(self.paths))] if self.channel_keywords[c] is not None else None for c in range(len(self.channel_keywords))]
         self.ads_array = [ [self.datasetIO.get_dataset(self._get_dataset_path(c, ds_idx, is_array=True)) for ds_idx in range(len(self.paths))] if self.array_keywords[c] is not None else None for c in range(len(self.array_keywords))]
         getAttribute = lambda a, def_val : def_val if a is None else (a[0] if isinstance(a, list) else a)
         self.ds_scaling_center = [[getAttribute(self.datasetIO.get_attribute(self._get_dataset_path(c, ds_idx), "scaling_center"), 0) for ds_idx in range(len(self.paths))]  if self.channel_keywords[c] is not None else None for c in range(len(self.channel_keywords))]
         self.ds_scaling_factor = [[getAttribute(self.datasetIO.get_attribute(self._get_dataset_path(c, ds_idx), "scaling_factor"), 1) for ds_idx in range(len(self.paths))]  if self.channel_keywords[c] is not None else None for c in range(len(self.channel_keywords))]
 
     def open(self):
-        self._open_datasetIO()
-
+        if self.datasetIO is None:
+            self._open_datasetIO()
 
     def _close_datasetIO(self):
         if self.datasetIO is not None:
             self.datasetIO.close()
             self.datasetIO = None
             self.ds_array = None
             self.ads_array = None
@@ -446,16 +449,15 @@
                 if not isinstance(input, list):
                     input = [input]
                 input.append(batch_by_channel[-1])
             output = _apply_multiplicity(output, self.output_multiplicity) # removes None batches
             return input, output
 
     def _get_batch_by_channel(self, index_array, perform_augmentation, input_only=False, perform_elasticdeform=True, perform_tiling=True, **kwargs):
-        if self.datasetIO is None: # each worker opens file is open file
-            self._open_datasetIO()
+        self.open()
         index_array = np.copy(index_array) # so that main index array is not modified
         index_ds = self._get_ds_idx(index_array) # modifies index_array
 
         batch_by_channel = dict()
         channels = self.input_channels if input_only else [c_idx for c_idx, key in enumerate(self.channel_keywords) if key is not None]
         #if len(self.mask_channels)>0 and self.mask_channels[0] in channels: # put mask channel first so it can be used for determining some data augmentation parameters
         #    channels.insert(0, channels.pop(channels.index(self.mask_channels[0])))
@@ -769,16 +771,15 @@
             of.close()
 
         # reset iterators parameters
         self.shuffle = shuffle
         self.batch_index = batch_index
 
     def _ensure_dataset(self, output_file, output_shapes, output_keys, ds_i, **create_dataset_options):
-        if self.datasetIO is None:
-            self._open_datasetIO()
+        self.open()
         if self.labels is not None:
             label_path = replace_last(self.paths[ds_i], self.channel_keywords[0], '/labels')
             if label_path not in output_file:
                 output_file.create_dataset(label_path, data=np.asarray(self.labels[ds_i], dtype=np.string_))
         dim_path = replace_last(self.paths[ds_i], self.channel_keywords[0], '/originalDimensions')
         if dim_path not in output_file and dim_path in self.datasetIO:
             output_file.create_dataset(dim_path, data=self.datasetIO.get_dataset(dim_path))
@@ -790,16 +791,15 @@
     def _has_object_at_y_borders(self, mask_channel_idx, ds_idx, im_idx):
         ds = self.ds_array[mask_channel_idx][ds_idx]
         off = self.ds_scaling_center[mask_channel_idx][ds_idx] # supposes there are no other scaling for mask channel
         return np.any(ds[im_idx, [-1,0], :] - off, 1) # np.flip()
 
     def _get_void_masks(self):
         assert len(self.mask_channels)>0, "cannot compute void mask if no mask channel is defined"
-        if self.datasetIO is None: # for concurency issues: file is open lazyly by each worker
-            self._open_datasetIO()
+        self.open()
         mask_channel = self.void_mask_chan
         index_array = np.copy(self.allowed_indexes)
         index_ds = self._get_ds_idx(index_array)
         void_masks = np.array([not np.any(self._read_image(mask_channel, ds_idx, im_idx)) for i, (ds_idx, im_idx) in enumerate(zip(index_ds, index_array))])
         return void_masks
 
     def set_allowed_indexes(self, indexes):
```

### Comparing `dataset_iterator-0.4.3/dataset_iterator/ordered_enqueuer_cf.py` & `dataset_iterator-0.4.4/dataset_iterator/ordered_enqueuer_cf.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,22 @@
 import os
+import gc
 import traceback
-from concurrent.futures import ProcessPoolExecutor
+from concurrent.futures import ProcessPoolExecutor, CancelledError, TimeoutError
 import multiprocessing
 import random
 import threading
 import time
-from multiprocessing import managers
 from threading import BoundedSemaphore
-from .shared_memory import to_shm, from_shm
+from .shared_memory import to_shm, from_shm, unlink_tensor_ref
 
 # adapted from https://github.com/keras-team/keras/blob/v2.13.1/keras/utils/data_utils.py#L651-L776
 # uses concurrent.futures, solves a memory leak in case of hard sample mining run as callback with regular orderedEnqueur. Option to pass tensors through shared memory
-
-
 # Global variables to be shared across processes
 _SHARED_SEQUENCES = {}
-_SHARED_SHM_MANAGER = {}
 # We use a Value to provide unique id to different processes.
 _SEQUENCE_COUNTER = None
 
 class OrderedEnqueuerCF():
     def __init__(self, sequence, shuffle=False, single_epoch:bool=False, use_shm:bool=True, wait_for_me:threading.Event=None):
         self.sequence = sequence
         self.shuffle = shuffle
@@ -45,92 +42,91 @@
                 self.uid = _SEQUENCE_COUNTER.value
                 _SEQUENCE_COUNTER.value += 1
 
         self.workers = 0
         self.queue = None
         self.run_thread = None
         self.stop_signal = None
-        self.shm_manager = None
+        self.stop_signal = None
         self.semaphore = None
 
     def is_running(self):
         return self.stop_signal is not None and not self.stop_signal.is_set()
 
     def start(self, workers=1, max_queue_size=10):
         """Starts the handler's workers.
 
         Args:
             workers: Number of workers.
             max_queue_size: queue size
                 (when full, workers could block on `put()`)
         """
+        if self.use_shm:  # load in shared memory before spawning threads otherwise each thread will load in memory
+            try:
+                self.sequence.open()
+            except AttributeError:
+                pass
         self.workers = workers
         if max_queue_size <= 0:
             max_queue_size = self.workers
         self.semaphore = BoundedSemaphore(max_queue_size)
         self.queue = []
         self.stop_signal = threading.Event()
-        if self.use_shm:
-            self.shm_manager = managers.SharedMemoryManager()
-            self.shm_manager.start()
         self.run_thread = threading.Thread(target=self._run)
         self.run_thread.daemon = True
         self.run_thread.start()
 
     def _wait_queue(self, empty:bool):
-        """Wait for the queue to be empty."""
+        """Wait for the queue to be empty or not empty."""
         while True:
             if (empty and len(self.queue) == 0) or (not empty and len(self.queue) > 0) or self.stop_signal.is_set():
                 return
             time.sleep(0.1)
 
     def _task_done(self, _):
         """Called once task is done, releases the queue if blocked."""
         self.semaphore.release()
 
     def _run(self):
         """Submits request to the executor and queue the `Future` objects."""
-
+        task = get_item_shm if self.use_shm else get_item
         sequence = list(range(len(self.sequence)))
         self._send_sequence()  # Share the initial sequence
         while True:
             if self.shuffle:
                 random.shuffle(sequence)
-            task = get_item_shm if self.use_shm else get_item
-            executor = ProcessPoolExecutor(max_workers=self.workers, initializer=init_pool_generator, initargs=(self.sequence, self.uid, self.shm_manager))
-            #print(f"executor started", flush=True)
+            executor = ProcessPoolExecutor(max_workers=self.workers)
             for idx, i in enumerate(sequence):
                 if self.stop_signal.is_set():
+                    executor.shutdown(wait=False, cancel_futures=True)
                     return
                 self.semaphore.acquire()
                 future = executor.submit(task, self.uid, i)
                 self.queue.append((future, i))
-                #print(f"sumit task: {i} {idx+1}/{len(sequence)}")
             # Done with the current epoch, waiting for the final batches
             self._wait_queue(True) # safer to wait before calling shutdown than calling directly shutdown with wait=True
-            #print("exiting from ProcessPoolExecutor...", flush=True)
             time.sleep(0.1)
             executor.shutdown(wait=False, cancel_futures=True)
-            #print("exiting from ProcessPoolExecutor done", flush=True)
+            del executor
+            gc.collect()
             if self.stop_signal.is_set() or self.single_epoch:
-                # We're done
                 return
             if self.wait_for_me is not None:
                 self.wait_for_me.wait()
-            # Call the internal on epoch end.
-            self.sequence.on_epoch_end()
             self._send_sequence()  # Update the pool
 
     def _send_sequence(self):
         """Sends current Iterable to all workers."""
         # For new processes that may spawn
         global _SHARED_SEQUENCES
+        try:
+            self.sequence.on_epoch_end()
+        except AttributeError:
+            pass
         _SHARED_SEQUENCES[self.uid] = self.sequence
-        global _SHARED_SHM_MANAGER
-        _SHARED_SHM_MANAGER[self.uid] = self.shm_manager
 
     def get(self):
         """Creates a generator to extract data from the queue.
 
         Skip the data if it is `None`.
 
         Yields:
@@ -164,33 +160,32 @@
         Should be called by the same thread which called `start()`.
 
         Args:
             timeout: maximum time to wait on `thread.join()`
         """
         self.stop_signal.set()
         self.run_thread.join(timeout)
-        if self.shm_manager is not None:
-            self.shm_manager.shutdown()
-            self.shm_manager.join()
+        if self.use_shm and self.queue is not None and len(self.queue) > 0:  # clean shm
+            for (future, _) in self.queue:
+                if future.exception() is None:
+                    try:
+                        unlink_tensor_ref(*future.result(timeout=0.1))
+                    except CancelledError | TimeoutError:  # save to shm is the last step, if task was not finished it is likely not saved to shm
+                        pass
         self.queue = None
         self.semaphore = None
-        global _SHARED_SHM_MANAGER
-        _SHARED_SHM_MANAGER[self.uid] = None
         global _SHARED_SEQUENCES
         _SHARED_SEQUENCES[self.uid] = None
 
-
-def init_pool_generator(gen, uid, shm_manager):
-    global _SHARED_SEQUENCES
-    _SHARED_SEQUENCES[uid] = gen
-    global _SHARED_SHM_MANAGER
-    _SHARED_SHM_MANAGER[uid] = shm_manager
+    def __del__(self):
+        self.stop()
 
 
 def get_item_shm(uid, i):
     tensors = _SHARED_SEQUENCES[uid][i]
-    return to_shm(_SHARED_SHM_MANAGER[uid], tensors)
+    #print(f"item {i} -> {_SHARED_SEQUENCES[uid].index_array[i]} process: {os.getpid()}", flush=True)
+    return to_shm(tensors)
 
 
 def get_item(uid, i):
     return _SHARED_SEQUENCES[uid][i]
```

### Comparing `dataset_iterator-0.4.3/dataset_iterator/pre_processing.py` & `dataset_iterator-0.4.4/dataset_iterator/pre_processing.py`

 * *Files identical despite different names*

### Comparing `dataset_iterator-0.4.3/dataset_iterator/shared_memory.py` & `dataset_iterator-0.4.4/dataset_iterator/shared_memory.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import numpy as np
 from multiprocessing import shared_memory
 
 
-def to_shm(shm_manager, tensors):
+def to_shm(tensors, shm_manager=None):
     flatten_tensor_list, nested_structure = get_flatten_list(tensors)
     size = np.sum([a.nbytes for a in flatten_tensor_list])
     shm = shm_manager.SharedMemory(size=size) if shm_manager is not None else shared_memory.SharedMemory(create=True, size=size)
     shapes = []
     dtypes = []
     offset = 0
     for a in flatten_tensor_list:
@@ -84,26 +84,39 @@
             offset = _get_nested(flatten_list, sub_nested, offset, result[-1])
         return offset
     else:
         result.append(flatten_list[offset])
         return offset + 1
 
 
+def unlink_tensor_ref(shapes, dtypes, shm_name, nested_structure):
+    unlink_shm_ref(shm_name)
+
+
+def unlink_shm_ref(shm_name):
+    try:
+        existing_shm = shared_memory.SharedMemory(shm_name)
+        existing_shm.unlink()
+    except (FileExistsError, FileNotFoundError):
+        pass
+
+
 # code from: https://muditb.medium.com/speed-up-your-keras-sequence-pipeline-f5d158359f46
 class ShmArray(np.ndarray):
     def __new__(cls, shape, dtype=float, buffer=None, offset=0, strides=None, order=None, shm=None):
         obj = super(ShmArray, cls).__new__(cls, shape, dtype, buffer, offset, strides,  order)
         obj.shm = shm
         return obj
 
     def __array_finalize__(self, obj):
         if obj is None:
             return
         self.shm = getattr(obj, 'shm', None)
 
+
 class ErasingSharedMemory(shared_memory.SharedMemory):
     def __del__(self):
         super(ErasingSharedMemory, self).__del__()
         try:
             self.unlink()
-        except FileNotFoundError:  # manager can delete the file before array is finalized
+        except (FileExistsError, FileNotFoundError):  # manager can delete the file before array is finalized
             pass
```

### Comparing `dataset_iterator-0.4.3/dataset_iterator/tile_utils.py` & `dataset_iterator-0.4.4/dataset_iterator/tile_utils.py`

 * *Files identical despite different names*

### Comparing `dataset_iterator-0.4.3/dataset_iterator/tracking_iterator.py` & `dataset_iterator-0.4.4/dataset_iterator/tracking_iterator.py`

 * *Files identical despite different names*

### Comparing `dataset_iterator-0.4.3/dataset_iterator/utils.py` & `dataset_iterator-0.4.4/dataset_iterator/utils.py`

 * *Files identical despite different names*

### Comparing `dataset_iterator-0.4.3/dataset_iterator.egg-info/PKG-INFO` & `dataset_iterator-0.4.4/dataset_iterator.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: dataset_iterator
-Version: 0.4.3
+Version: 0.4.4
 Summary: Keras-style data iterator for images contained in dataset files such as hdf5 or PIL readable files. Images can be contained in several files.
 Home-page: https://github.com/jeanollion/dataset_iterator.git
-Download-URL: https://github.com/jeanollion/dataset_iterator/releases/download/v0.4.3/dataset_iterator-0.4.3.tar.gz
+Download-URL: https://github.com/jeanollion/dataset_iterator/releases/download/v0.4.4/dataset_iterator-0.4.4.tar.gz
 Author: Jean Ollion
 Author-email: jean.ollion@polytechnique.org
 Keywords: Iterator,Dataset,Image,Numpy
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Image Processing
```

### Comparing `dataset_iterator-0.4.3/dataset_iterator.egg-info/SOURCES.txt` & `dataset_iterator-0.4.4/dataset_iterator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dataset_iterator-0.4.3/setup.py` & `dataset_iterator-0.4.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="dataset_iterator",
-    version="0.4.3",
+    version="0.4.4",
     author="Jean Ollion",
     author_email="jean.ollion@polytechnique.org",
     description="Keras-style data iterator for images contained in dataset files such as hdf5 or PIL readable files. Images can be contained in several files.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/jeanollion/dataset_iterator.git",
-    download_url='https://github.com/jeanollion/dataset_iterator/releases/download/v0.4.3/dataset_iterator-0.4.3.tar.gz',
+    download_url='https://github.com/jeanollion/dataset_iterator/releases/download/v0.4.4/dataset_iterator-0.4.4.tar.gz',
     keywords=['Iterator', 'Dataset', 'Image', 'Numpy'],
     packages=setuptools.find_packages(),
     classifiers=[ #https://pypi.org/classifiers/
         'Development Status :: 4 - Beta',
         'Intended Audience :: Science/Research',
         'Topic :: Scientific/Engineering :: Artificial Intelligence',
         'Topic :: Scientific/Engineering :: Image Processing',
```

