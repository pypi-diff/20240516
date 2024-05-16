# Comparing `tmp/lacss-0.8.0.tar.gz` & `tmp/lacss-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lacss-0.8.0.tar", max compression
+gzip compressed data, was "lacss-0.8.1.tar", max compression
```

## Comparing `lacss-0.8.0.tar` & `lacss-0.8.1.tar`

### file list

```diff
@@ -1,48 +1,48 @@
--rw-r--r--   0        0        0     1062 2024-04-09 16:25:19.232858 lacss-0.8.0/LICENSE
--rw-r--r--   0        0        0     2539 2024-04-09 16:25:19.232858 lacss-0.8.0/README.md
--rw-r--r--   0        0        0      157 2024-04-09 16:25:19.232858 lacss-0.8.0/lacss/__init__.py
--rw-r--r--   0        0        0       48 2024-04-09 16:25:19.232858 lacss-0.8.0/lacss/data/__init__.py
--rw-r--r--   0        0        0    14546 2024-04-09 16:25:19.232858 lacss-0.8.0/lacss/data/augment.py
--rw-r--r--   0        0        0    13109 2024-04-09 16:25:19.232858 lacss-0.8.0/lacss/data/generator.py
--rw-r--r--   0        0        0       43 2024-04-09 16:25:19.232858 lacss-0.8.0/lacss/deploy/__init__.py
--rw-r--r--   0        0        0     3151 2024-04-09 16:25:19.232858 lacss-0.8.0/lacss/deploy/lacss_pb2.py
--rw-r--r--   0        0        0    21615 2024-04-09 16:25:19.232858 lacss-0.8.0/lacss/deploy/predict.py
--rw-r--r--   0        0        0     4125 2024-04-09 16:25:19.232858 lacss-0.8.0/lacss/deploy/server.py
--rw-r--r--   0        0        0       74 2024-04-09 16:25:19.232858 lacss-0.8.0/lacss/losses/__init__.py
--rw-r--r--   0        0        0     6115 2024-04-09 16:25:19.232858 lacss-0.8.0/lacss/losses/auxiliary.py
--rw-r--r--   0        0        0      965 2024-04-09 16:25:19.232858 lacss-0.8.0/lacss/losses/common.py
--rw-r--r--   0        0        0     1748 2024-04-09 16:25:19.232858 lacss-0.8.0/lacss/losses/detection.py
--rw-r--r--   0        0        0     5406 2024-04-09 16:25:19.232858 lacss-0.8.0/lacss/losses/instance.py
--rw-r--r--   0        0        0       22 2024-04-09 16:25:19.232858 lacss-0.8.0/lacss/metrics/__init__.py
--rw-r--r--   0        0        0     5559 2024-04-09 16:25:19.232858 lacss-0.8.0/lacss/metrics/ranked.py
--rw-r--r--   0        0        0      330 2024-04-09 16:25:19.232858 lacss-0.8.0/lacss/modules/__init__.py
--rw-r--r--   0        0        0     2355 2024-04-09 16:25:19.232858 lacss-0.8.0/lacss/modules/common.py
--rw-r--r--   0        0        0     7968 2024-04-09 16:25:19.232858 lacss-0.8.0/lacss/modules/convnext.py
--rw-r--r--   0        0        0     7808 2024-04-09 16:25:19.232858 lacss-0.8.0/lacss/modules/detector.py
--rw-r--r--   0        0        0     3899 2024-04-09 16:25:19.232858 lacss-0.8.0/lacss/modules/lacss.py
--rw-r--r--   0        0        0     3292 2024-04-09 16:25:19.232858 lacss-0.8.0/lacss/modules/lpn.py
--rw-r--r--   0        0        0     3830 2024-04-09 16:25:19.232858 lacss-0.8.0/lacss/modules/resnet.py
--rw-r--r--   0        0        0     5557 2024-04-09 16:25:19.232858 lacss-0.8.0/lacss/modules/segmentor.py
--rw-r--r--   0        0        0     2297 2024-04-09 16:25:19.232858 lacss-0.8.0/lacss/modules/unet.py
--rw-r--r--   0        0        0      153 2024-04-09 16:25:19.232858 lacss-0.8.0/lacss/ops/__init__.py
--rw-r--r--   0        0        0     2474 2024-04-09 16:25:19.232858 lacss-0.8.0/lacss/ops/boxes.py
--rw-r--r--   0        0        0     3551 2024-04-09 16:25:19.232858 lacss-0.8.0/lacss/ops/image.py
--rw-r--r--   0        0        0     3136 2024-04-09 16:25:19.232858 lacss-0.8.0/lacss/ops/locations.py
--rw-r--r--   0        0        0     5961 2024-04-09 16:25:19.232858 lacss-0.8.0/lacss/ops/nms.py
--rw-r--r--   0        0        0    11822 2024-04-09 16:25:19.232858 lacss-0.8.0/lacss/ops/patches.py
--rw-r--r--   0        0        0      482 2024-04-09 16:25:19.232858 lacss-0.8.0/lacss/ops/uda.py
--rw-r--r--   0        0        0       63 2024-04-09 16:25:19.232858 lacss-0.8.0/lacss/tracking/__init__.py
--rw-r--r--   0        0        0     3340 2024-04-09 16:25:19.232858 lacss-0.8.0/lacss/tracking/predict.py
--rw-r--r--   0        0        0    12670 2024-04-09 16:25:19.232858 lacss-0.8.0/lacss/tracking/seqnms.py
--rw-r--r--   0        0        0     6741 2024-04-09 16:25:19.232858 lacss-0.8.0/lacss/tracking/smc.py
--rw-r--r--   0        0        0     5646 2024-04-09 16:25:19.232858 lacss-0.8.0/lacss/tracking/utils.py
--rw-r--r--   0        0        0      203 2024-04-09 16:25:19.232858 lacss-0.8.0/lacss/train/__init__.py
--rw-r--r--   0        0        0    10383 2024-04-09 16:25:19.232858 lacss-0.8.0/lacss/train/base_trainer.py
--rw-r--r--   0        0        0    10541 2024-04-09 16:25:19.232858 lacss-0.8.0/lacss/train/lacss_trainer.py
--rw-r--r--   0        0        0     1170 2024-04-09 16:25:19.232858 lacss-0.8.0/lacss/train/loss.py
--rw-r--r--   0        0        0     4564 2024-04-09 16:25:19.232858 lacss-0.8.0/lacss/train/strategy.py
--rw-r--r--   0        0        0     5541 2024-04-09 16:25:19.232858 lacss-0.8.0/lacss/train/utils.py
--rw-r--r--   0        0        0      931 2024-04-09 16:25:19.232858 lacss-0.8.0/lacss/typing.py
--rw-r--r--   0        0        0     5151 2024-04-09 16:25:19.232858 lacss-0.8.0/lacss/utils.py
--rw-r--r--   0        0        0      995 2024-04-09 16:25:35.776837 lacss-0.8.0/pyproject.toml
--rw-r--r--   0        0        0     3285 1970-01-01 00:00:00.000000 lacss-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1062 2024-04-12 13:57:54.798780 lacss-0.8.1/LICENSE
+-rw-r--r--   0        0        0     2539 2024-04-12 13:57:54.798780 lacss-0.8.1/README.md
+-rw-r--r--   0        0        0      157 2024-04-12 13:57:54.798780 lacss-0.8.1/lacss/__init__.py
+-rw-r--r--   0        0        0       48 2024-04-12 13:57:54.798780 lacss-0.8.1/lacss/data/__init__.py
+-rw-r--r--   0        0        0    14546 2024-04-12 13:57:54.798780 lacss-0.8.1/lacss/data/augment.py
+-rw-r--r--   0        0        0    13109 2024-04-12 13:57:54.798780 lacss-0.8.1/lacss/data/generator.py
+-rw-r--r--   0        0        0       43 2024-04-12 13:57:54.802780 lacss-0.8.1/lacss/deploy/__init__.py
+-rw-r--r--   0        0        0     3151 2024-04-12 13:57:54.802780 lacss-0.8.1/lacss/deploy/lacss_pb2.py
+-rw-r--r--   0        0        0    21615 2024-04-12 13:57:54.802780 lacss-0.8.1/lacss/deploy/predict.py
+-rw-r--r--   0        0        0     4125 2024-04-12 13:57:54.802780 lacss-0.8.1/lacss/deploy/server.py
+-rw-r--r--   0        0        0       74 2024-04-12 13:57:54.802780 lacss-0.8.1/lacss/losses/__init__.py
+-rw-r--r--   0        0        0     6115 2024-04-12 13:57:54.802780 lacss-0.8.1/lacss/losses/auxiliary.py
+-rw-r--r--   0        0        0      965 2024-04-12 13:57:54.802780 lacss-0.8.1/lacss/losses/common.py
+-rw-r--r--   0        0        0     1748 2024-04-12 13:57:54.802780 lacss-0.8.1/lacss/losses/detection.py
+-rw-r--r--   0        0        0     5406 2024-04-12 13:57:54.802780 lacss-0.8.1/lacss/losses/instance.py
+-rw-r--r--   0        0        0       22 2024-04-12 13:57:54.802780 lacss-0.8.1/lacss/metrics/__init__.py
+-rw-r--r--   0        0        0     5559 2024-04-12 13:57:54.802780 lacss-0.8.1/lacss/metrics/ranked.py
+-rw-r--r--   0        0        0      330 2024-04-12 13:57:54.802780 lacss-0.8.1/lacss/modules/__init__.py
+-rw-r--r--   0        0        0     2355 2024-04-12 13:57:54.802780 lacss-0.8.1/lacss/modules/common.py
+-rw-r--r--   0        0        0     7968 2024-04-12 13:57:54.802780 lacss-0.8.1/lacss/modules/convnext.py
+-rw-r--r--   0        0        0     7808 2024-04-12 13:57:54.802780 lacss-0.8.1/lacss/modules/detector.py
+-rw-r--r--   0        0        0     3899 2024-04-12 13:57:54.802780 lacss-0.8.1/lacss/modules/lacss.py
+-rw-r--r--   0        0        0     3292 2024-04-12 13:57:54.802780 lacss-0.8.1/lacss/modules/lpn.py
+-rw-r--r--   0        0        0     3830 2024-04-12 13:57:54.802780 lacss-0.8.1/lacss/modules/resnet.py
+-rw-r--r--   0        0        0     5557 2024-04-12 13:57:54.802780 lacss-0.8.1/lacss/modules/segmentor.py
+-rw-r--r--   0        0        0     2297 2024-04-12 13:57:54.802780 lacss-0.8.1/lacss/modules/unet.py
+-rw-r--r--   0        0        0      153 2024-04-12 13:57:54.802780 lacss-0.8.1/lacss/ops/__init__.py
+-rw-r--r--   0        0        0     2474 2024-04-12 13:57:54.802780 lacss-0.8.1/lacss/ops/boxes.py
+-rw-r--r--   0        0        0     3551 2024-04-12 13:57:54.802780 lacss-0.8.1/lacss/ops/image.py
+-rw-r--r--   0        0        0     3136 2024-04-12 13:57:54.802780 lacss-0.8.1/lacss/ops/locations.py
+-rw-r--r--   0        0        0     5961 2024-04-12 13:57:54.802780 lacss-0.8.1/lacss/ops/nms.py
+-rw-r--r--   0        0        0    11822 2024-04-12 13:57:54.802780 lacss-0.8.1/lacss/ops/patches.py
+-rw-r--r--   0        0        0      482 2024-04-12 13:57:54.802780 lacss-0.8.1/lacss/ops/uda.py
+-rw-r--r--   0        0        0       63 2024-04-12 13:57:54.802780 lacss-0.8.1/lacss/tracking/__init__.py
+-rw-r--r--   0        0        0     3340 2024-04-12 13:57:54.802780 lacss-0.8.1/lacss/tracking/predict.py
+-rw-r--r--   0        0        0    12670 2024-04-12 13:57:54.802780 lacss-0.8.1/lacss/tracking/seqnms.py
+-rw-r--r--   0        0        0     6741 2024-04-12 13:57:54.802780 lacss-0.8.1/lacss/tracking/smc.py
+-rw-r--r--   0        0        0     5646 2024-04-12 13:57:54.802780 lacss-0.8.1/lacss/tracking/utils.py
+-rw-r--r--   0        0        0      203 2024-04-12 13:57:54.802780 lacss-0.8.1/lacss/train/__init__.py
+-rw-r--r--   0        0        0    10358 2024-04-12 13:57:54.802780 lacss-0.8.1/lacss/train/base_trainer.py
+-rw-r--r--   0        0        0    10541 2024-04-12 13:57:54.802780 lacss-0.8.1/lacss/train/lacss_trainer.py
+-rw-r--r--   0        0        0     1170 2024-04-12 13:57:54.802780 lacss-0.8.1/lacss/train/loss.py
+-rw-r--r--   0        0        0     4564 2024-04-12 13:57:54.802780 lacss-0.8.1/lacss/train/strategy.py
+-rw-r--r--   0        0        0     5541 2024-04-12 13:57:54.802780 lacss-0.8.1/lacss/train/utils.py
+-rw-r--r--   0        0        0      931 2024-04-12 13:57:54.802780 lacss-0.8.1/lacss/typing.py
+-rw-r--r--   0        0        0     5151 2024-04-12 13:57:54.802780 lacss-0.8.1/lacss/utils.py
+-rw-r--r--   0        0        0      988 2024-04-12 13:58:13.111070 lacss-0.8.1/pyproject.toml
+-rw-r--r--   0        0        0     3337 1970-01-01 00:00:00.000000 lacss-0.8.1/PKG-INFO
```

### Comparing `lacss-0.8.0/LICENSE` & `lacss-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `lacss-0.8.0/README.md` & `lacss-0.8.1/README.md`

 * *Files identical despite different names*

### Comparing `lacss-0.8.0/lacss/data/augment.py` & `lacss-0.8.1/lacss/data/augment.py`

 * *Files identical despite different names*

### Comparing `lacss-0.8.0/lacss/data/generator.py` & `lacss-0.8.1/lacss/data/generator.py`

 * *Files identical despite different names*

### Comparing `lacss-0.8.0/lacss/deploy/lacss_pb2.py` & `lacss-0.8.1/lacss/deploy/lacss_pb2.py`

 * *Files identical despite different names*

### Comparing `lacss-0.8.0/lacss/deploy/predict.py` & `lacss-0.8.1/lacss/deploy/predict.py`

 * *Files identical despite different names*

### Comparing `lacss-0.8.0/lacss/deploy/server.py` & `lacss-0.8.1/lacss/deploy/server.py`

 * *Files identical despite different names*

### Comparing `lacss-0.8.0/lacss/losses/auxiliary.py` & `lacss-0.8.1/lacss/losses/auxiliary.py`

 * *Files identical despite different names*

### Comparing `lacss-0.8.0/lacss/losses/common.py` & `lacss-0.8.1/lacss/losses/common.py`

 * *Files identical despite different names*

### Comparing `lacss-0.8.0/lacss/losses/detection.py` & `lacss-0.8.1/lacss/losses/detection.py`

 * *Files identical despite different names*

### Comparing `lacss-0.8.0/lacss/losses/instance.py` & `lacss-0.8.1/lacss/losses/instance.py`

 * *Files identical despite different names*

### Comparing `lacss-0.8.0/lacss/metrics/ranked.py` & `lacss-0.8.1/lacss/metrics/ranked.py`

 * *Files identical despite different names*

### Comparing `lacss-0.8.0/lacss/modules/common.py` & `lacss-0.8.1/lacss/modules/common.py`

 * *Files identical despite different names*

### Comparing `lacss-0.8.0/lacss/modules/convnext.py` & `lacss-0.8.1/lacss/modules/convnext.py`

 * *Files identical despite different names*

### Comparing `lacss-0.8.0/lacss/modules/detector.py` & `lacss-0.8.1/lacss/modules/detector.py`

 * *Files identical despite different names*

### Comparing `lacss-0.8.0/lacss/modules/lacss.py` & `lacss-0.8.1/lacss/modules/lacss.py`

 * *Files identical despite different names*

### Comparing `lacss-0.8.0/lacss/modules/lpn.py` & `lacss-0.8.1/lacss/modules/lpn.py`

 * *Files identical despite different names*

### Comparing `lacss-0.8.0/lacss/modules/resnet.py` & `lacss-0.8.1/lacss/modules/resnet.py`

 * *Files identical despite different names*

### Comparing `lacss-0.8.0/lacss/modules/segmentor.py` & `lacss-0.8.1/lacss/modules/segmentor.py`

 * *Files identical despite different names*

### Comparing `lacss-0.8.0/lacss/modules/unet.py` & `lacss-0.8.1/lacss/modules/unet.py`

 * *Files identical despite different names*

### Comparing `lacss-0.8.0/lacss/ops/boxes.py` & `lacss-0.8.1/lacss/ops/boxes.py`

 * *Files identical despite different names*

### Comparing `lacss-0.8.0/lacss/ops/image.py` & `lacss-0.8.1/lacss/ops/image.py`

 * *Files identical despite different names*

### Comparing `lacss-0.8.0/lacss/ops/locations.py` & `lacss-0.8.1/lacss/ops/locations.py`

 * *Files identical despite different names*

### Comparing `lacss-0.8.0/lacss/ops/nms.py` & `lacss-0.8.1/lacss/ops/nms.py`

 * *Files identical despite different names*

### Comparing `lacss-0.8.0/lacss/ops/patches.py` & `lacss-0.8.1/lacss/ops/patches.py`

 * *Files identical despite different names*

### Comparing `lacss-0.8.0/lacss/tracking/predict.py` & `lacss-0.8.1/lacss/tracking/predict.py`

 * *Files identical despite different names*

### Comparing `lacss-0.8.0/lacss/tracking/seqnms.py` & `lacss-0.8.1/lacss/tracking/seqnms.py`

 * *Files identical despite different names*

### Comparing `lacss-0.8.0/lacss/tracking/smc.py` & `lacss-0.8.1/lacss/tracking/smc.py`

 * *Files identical despite different names*

### Comparing `lacss-0.8.0/lacss/tracking/utils.py` & `lacss-0.8.1/lacss/tracking/utils.py`

 * *Files identical despite different names*

### Comparing `lacss-0.8.0/lacss/train/base_trainer.py` & `lacss-0.8.1/lacss/train/base_trainer.py`

 * *Files 1% similar despite different names*

```diff
@@ -288,17 +288,16 @@
     ) -> Iterator:
         """Create test/validation iterator.
 
         Args:
             dataset: An iterator or iterable to supply the testing data.
                 The iterator should yield a tupple of (inputs, labels).
             metrics: A list of Metric objects. They should have two functions:
-                m.update(preds, **kwargs):
-                    preds is the model output. the remaining kwargs are content of
-                    labels.
+                m.update(batch, prediction):
+                    prediction is the model output, batch is a tuple of (x, y_true)
                 m.compute():
                     which should return the accumulated metric value.
             variables: Model weights etc. typically get from TrainIterator
             strategy: Optionally override the default strategy.
 
         Returns:
             An iterator. Stepping through it will drive the updating of each metric
```

### Comparing `lacss-0.8.0/lacss/train/lacss_trainer.py` & `lacss-0.8.1/lacss/train/lacss_trainer.py`

 * *Files identical despite different names*

### Comparing `lacss-0.8.0/lacss/train/loss.py` & `lacss-0.8.1/lacss/train/loss.py`

 * *Files identical despite different names*

### Comparing `lacss-0.8.0/lacss/train/strategy.py` & `lacss-0.8.1/lacss/train/strategy.py`

 * *Files identical despite different names*

### Comparing `lacss-0.8.0/lacss/train/utils.py` & `lacss-0.8.1/lacss/train/utils.py`

 * *Files identical despite different names*

### Comparing `lacss-0.8.0/lacss/typing.py` & `lacss-0.8.1/lacss/typing.py`

 * *Files identical despite different names*

### Comparing `lacss-0.8.0/lacss/utils.py` & `lacss-0.8.1/lacss/utils.py`

 * *Files identical despite different names*

### Comparing `lacss-0.8.0/pyproject.toml` & `lacss-0.8.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [tool.poetry]
 name = "lacss"
-version = "0.8.0"
+version = "0.8.1"
 description = "Cell segmentation and tracking"
 authors = ["Ji Yu <jyu@uchc.edu>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
-python = ">=3.9, <3.11"
+python = "^3.10"
 flax = "^0.7.2"
 tqdm = "^4.65.0"
 imageio = "^2.9.0"
 scikit-image = ">=0.19.0"
 typer = ">=0.4.0"
 imagecodecs = "^2023.3.16"
 opencv-python = "^4.8.1.78"
```

### Comparing `lacss-0.8.0/PKG-INFO` & `lacss-0.8.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: lacss
-Version: 0.8.0
+Version: 0.8.1
 Summary: Cell segmentation and tracking
 License: MIT
 Author: Ji Yu
 Author-email: jyu@uchc.edu
-Requires-Python: >=3.9,<3.11
+Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: flax (>=0.7.2,<0.8.0)
 Requires-Dist: imagecodecs (>=2023.3.16,<2024.0.0)
 Requires-Dist: imageio (>=2.9.0,<3.0.0)
 Requires-Dist: opencv-python (>=4.8.1.78,<5.0.0.0)
 Requires-Dist: orbax-checkpoint (>=0.5,<0.6)
 Requires-Dist: scikit-image (>=0.19.0)
 Requires-Dist: tqdm (>=4.65.0,<5.0.0)
```

