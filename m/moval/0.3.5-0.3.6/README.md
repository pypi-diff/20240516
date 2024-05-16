# Comparing `tmp/moval-0.3.5.tar.gz` & `tmp/moval-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/zejuli/Local/Imperial/MOVAL/dist/.tmp-c7am99ez/moval-0.3.5.tar", last modified: Sun Apr 21 15:22:55 2024, max compression
+gzip compressed data, was "/Users/zejuli/Local/Imperial/MOVAL/dist/.tmp-r02e0gw1/moval-0.3.6.tar", last modified: Thu May 16 14:35:32 2024, max compression
```

## Comparing `moval-0.3.5.tar` & `moval-0.3.6.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 zejuli     (501) staff       (20)        0 2024-04-21 15:22:55.551315 moval-0.3.5/
--rw-r--r--   0 zejuli     (501) staff       (20)     3097 2024-04-21 15:22:55.551256 moval-0.3.5/PKG-INFO
--rw-r--r--   0 zejuli     (501) staff       (20)     2259 2024-01-19 15:02:41.000000 moval-0.3.5/README.md
-drwxr-xr-x   0 zejuli     (501) staff       (20)        0 2024-04-21 15:22:55.548111 moval-0.3.5/moval/
--rw-r--r--   0 zejuli     (501) staff       (20)      706 2024-04-21 15:17:03.000000 moval-0.3.5/moval/__init__.py
-drwxr-xr-x   0 zejuli     (501) staff       (20)        0 2024-04-21 15:22:55.548984 moval-0.3.5/moval/integrations/
--rw-r--r--   0 zejuli     (501) staff       (20)       68 2023-07-28 01:11:44.000000 moval-0.3.5/moval/integrations/__init__.py
-drwxr-xr-x   0 zejuli     (501) staff       (20)        0 2024-04-21 15:22:55.549263 moval-0.3.5/moval/integrations/sklearn/
--rw-r--r--   0 zejuli     (501) staff       (20)      462 2023-10-26 14:28:12.000000 moval-0.3.5/moval/integrations/sklearn/__init__.py
--rw-r--r--   0 zejuli     (501) staff       (20)    41094 2024-04-15 02:33:08.000000 moval-0.3.5/moval/integrations/sklearn/moval.py
-drwxr-xr-x   0 zejuli     (501) staff       (20)        0 2024-04-21 15:22:55.550148 moval-0.3.5/moval/models/
--rw-r--r--   0 zejuli     (501) staff       (20)      447 2023-11-09 00:55:21.000000 moval-0.3.5/moval/models/__init__.py
--rw-r--r--   0 zejuli     (501) staff       (20)     6840 2023-11-26 14:30:38.000000 moval-0.3.5/moval/models/confidences.py
--rw-r--r--   0 zejuli     (501) staff       (20)    44866 2024-04-21 15:22:16.000000 moval-0.3.5/moval/models/model.py
--rw-r--r--   0 zejuli     (501) staff       (20)     1631 2024-01-08 19:28:25.000000 moval-0.3.5/moval/models/solver_temperature.py
--rw-r--r--   0 zejuli     (501) staff       (20)    10804 2024-04-20 02:13:02.000000 moval-0.3.5/moval/models/utils.py
--rw-r--r--   0 zejuli     (501) staff       (20)    15406 2023-11-08 14:02:19.000000 moval-0.3.5/moval/registry.py
-drwxr-xr-x   0 zejuli     (501) staff       (20)        0 2024-04-21 15:22:55.550846 moval-0.3.5/moval/solvers/
--rw-r--r--   0 zejuli     (501) staff       (20)      429 2023-11-09 00:58:57.000000 moval-0.3.5/moval/solvers/__init__.py
--rw-r--r--   0 zejuli     (501) staff       (20)    11235 2024-04-15 02:36:06.000000 moval-0.3.5/moval/solvers/criterions.py
--rw-r--r--   0 zejuli     (501) staff       (20)    28951 2024-04-21 15:17:30.000000 moval-0.3.5/moval/solvers/solver.py
--rw-r--r--   0 zejuli     (501) staff       (20)     3054 2024-04-08 23:54:48.000000 moval-0.3.5/moval/solvers/utils.py
-drwxr-xr-x   0 zejuli     (501) staff       (20)        0 2024-04-21 15:22:55.551026 moval-0.3.5/moval.egg-info/
--rw-r--r--   0 zejuli     (501) staff       (20)     3097 2024-04-21 15:22:55.000000 moval-0.3.5/moval.egg-info/PKG-INFO
--rw-r--r--   0 zejuli     (501) staff       (20)      553 2024-04-21 15:22:55.000000 moval-0.3.5/moval.egg-info/SOURCES.txt
--rw-r--r--   0 zejuli     (501) staff       (20)        1 2024-04-21 15:22:55.000000 moval-0.3.5/moval.egg-info/dependency_links.txt
--rw-r--r--   0 zejuli     (501) staff       (20)       61 2024-04-21 15:22:55.000000 moval-0.3.5/moval.egg-info/requires.txt
--rw-r--r--   0 zejuli     (501) staff       (20)        6 2024-04-21 15:22:55.000000 moval-0.3.5/moval.egg-info/top_level.txt
--rw-r--r--   0 zejuli     (501) staff       (20)    15479 2023-12-08 04:03:18.000000 moval-0.3.5/pyproject.toml
--rw-r--r--   0 zejuli     (501) staff       (20)      896 2024-04-21 15:22:55.551657 moval-0.3.5/setup.cfg
+drwxr-xr-x   0 zejuli     (501) staff       (20)        0 2024-05-16 14:35:32.533845 moval-0.3.6/
+-rw-r--r--   0 zejuli     (501) staff       (20)     3097 2024-05-16 14:35:32.533788 moval-0.3.6/PKG-INFO
+-rw-r--r--   0 zejuli     (501) staff       (20)     2259 2024-01-19 15:02:41.000000 moval-0.3.6/README.md
+drwxr-xr-x   0 zejuli     (501) staff       (20)        0 2024-05-16 14:35:32.527877 moval-0.3.6/moval/
+-rw-r--r--   0 zejuli     (501) staff       (20)      706 2024-05-16 14:34:58.000000 moval-0.3.6/moval/__init__.py
+drwxr-xr-x   0 zejuli     (501) staff       (20)        0 2024-05-16 14:35:32.529120 moval-0.3.6/moval/integrations/
+-rw-r--r--   0 zejuli     (501) staff       (20)       68 2023-07-28 01:11:44.000000 moval-0.3.6/moval/integrations/__init__.py
+drwxr-xr-x   0 zejuli     (501) staff       (20)        0 2024-05-16 14:35:32.529737 moval-0.3.6/moval/integrations/sklearn/
+-rw-r--r--   0 zejuli     (501) staff       (20)      462 2023-10-26 14:28:12.000000 moval-0.3.6/moval/integrations/sklearn/__init__.py
+-rw-r--r--   0 zejuli     (501) staff       (20)    41330 2024-05-16 14:33:33.000000 moval-0.3.6/moval/integrations/sklearn/moval.py
+drwxr-xr-x   0 zejuli     (501) staff       (20)        0 2024-05-16 14:35:32.531831 moval-0.3.6/moval/models/
+-rw-r--r--   0 zejuli     (501) staff       (20)      447 2023-11-09 00:55:21.000000 moval-0.3.6/moval/models/__init__.py
+-rw-r--r--   0 zejuli     (501) staff       (20)     6840 2023-11-26 14:30:38.000000 moval-0.3.6/moval/models/confidences.py
+-rw-r--r--   0 zejuli     (501) staff       (20)    44866 2024-04-21 15:22:16.000000 moval-0.3.6/moval/models/model.py
+-rw-r--r--   0 zejuli     (501) staff       (20)     1631 2024-01-08 19:28:25.000000 moval-0.3.6/moval/models/solver_temperature.py
+-rw-r--r--   0 zejuli     (501) staff       (20)    10804 2024-04-20 02:13:02.000000 moval-0.3.6/moval/models/utils.py
+-rw-r--r--   0 zejuli     (501) staff       (20)    15406 2023-11-08 14:02:19.000000 moval-0.3.6/moval/registry.py
+drwxr-xr-x   0 zejuli     (501) staff       (20)        0 2024-05-16 14:35:32.533244 moval-0.3.6/moval/solvers/
+-rw-r--r--   0 zejuli     (501) staff       (20)      429 2023-11-09 00:58:57.000000 moval-0.3.6/moval/solvers/__init__.py
+-rw-r--r--   0 zejuli     (501) staff       (20)    11235 2024-04-15 02:36:06.000000 moval-0.3.6/moval/solvers/criterions.py
+-rw-r--r--   0 zejuli     (501) staff       (20)    28881 2024-05-16 14:34:21.000000 moval-0.3.6/moval/solvers/solver.py
+-rw-r--r--   0 zejuli     (501) staff       (20)     3054 2024-04-08 23:54:48.000000 moval-0.3.6/moval/solvers/utils.py
+drwxr-xr-x   0 zejuli     (501) staff       (20)        0 2024-05-16 14:35:32.533545 moval-0.3.6/moval.egg-info/
+-rw-r--r--   0 zejuli     (501) staff       (20)     3097 2024-05-16 14:35:32.000000 moval-0.3.6/moval.egg-info/PKG-INFO
+-rw-r--r--   0 zejuli     (501) staff       (20)      553 2024-05-16 14:35:32.000000 moval-0.3.6/moval.egg-info/SOURCES.txt
+-rw-r--r--   0 zejuli     (501) staff       (20)        1 2024-05-16 14:35:32.000000 moval-0.3.6/moval.egg-info/dependency_links.txt
+-rw-r--r--   0 zejuli     (501) staff       (20)       61 2024-05-16 14:35:32.000000 moval-0.3.6/moval.egg-info/requires.txt
+-rw-r--r--   0 zejuli     (501) staff       (20)        6 2024-05-16 14:35:32.000000 moval-0.3.6/moval.egg-info/top_level.txt
+-rw-r--r--   0 zejuli     (501) staff       (20)    15479 2023-12-08 04:03:18.000000 moval-0.3.6/pyproject.toml
+-rw-r--r--   0 zejuli     (501) staff       (20)      896 2024-05-16 14:35:32.534187 moval-0.3.6/setup.cfg
```

### Comparing `moval-0.3.5/PKG-INFO` & `moval-0.3.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moval
-Version: 0.3.5
+Version: 0.3.6
 Summary: Model evaluation without manual labels
 Home-page: https://github.com/ZerojumpLine/MOVAL
 Author: Zeju Li
 Author-email: lizeju8@gmail.com
 Project-URL: Bug Tracker, https://github.com/ZerojumpLine/MOVAL/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: GPU :: NVIDIA CUDA
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: moval Version: 0.3.5 Summary: Model evaluation
+Metadata-Version: 2.1 Name: moval Version: 0.3.6 Summary: Model evaluation
 without manual labels Home-page: https://github.com/ZerojumpLine/MOVAL Author:
 Zeju Li Author-email: lizeju8@gmail.com Project-URL: Bug Tracker, https://
 github.com/ZerojumpLine/MOVAL/issues Classifier: Development Status :: 3 -
 Alpha Classifier: Environment :: GPU :: NVIDIA CUDA Classifier: Intended
 Audience :: Science/Research Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 Classifier: Topic ::
 Scientific/Engineering :: Artificial Intelligence Classifier: License :: Free
```

### Comparing `moval-0.3.5/README.md` & `moval-0.3.6/README.md`

 * *Files identical despite different names*

### Comparing `moval-0.3.5/moval/__init__.py` & `moval-0.3.6/moval/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 try:
     from moval.integrations.sklearn.moval import MOVAL
 except ImportError as e:
     # silently fail for now
     pass
 
-__version__ = "0.3.5"
+__version__ = "0.3.6"
 __all__ = ["MOVAL"]
 
 def __getattr__(key):
     """Lazy import of moval submodules and -packages.
 
     Once :py:mod:`moval` is imported, it is possible to lazy import
```

### Comparing `moval-0.3.5/moval/integrations/sklearn/moval.py` & `moval-0.3.6/moval/integrations/sklearn/moval.py`

 * *Files 1% similar despite different names*

```diff
@@ -172,27 +172,28 @@
                     estim_algorithm,
                     mode = mode,
                     num_class = self.numclass,
                     confidence_scores = confidence_scores,
                     class_specific = class_specific
                 )
 
-                if class_specific == True:
-                    # find a good initatlization, as other metrics would also depend on non-maximum logits
-                    # also find a good init for accuary of sensitivty, to handle the corner cases, where making no prediction for specific classes.
-                    model_pre = moval.models.init(
-                        estim_algorithm,
-                        mode = self.mode,
-                        num_class = self.numclass,
-                        confidence_scores = self.confidence_scores,
-                        class_specific = False
-                        )
-                    solver_pre = moval.solvers.init("base-solver", model = model_pre, metric = "accuracy")
-                    solver_pre.fit(logits, gt)
-                    model.param = np.ones(self.numclass) * model_pre.param
+                # Zeju Li, 16 May 2024: The leads to weird behaviour of precision estimation, skip it now.
+                # if class_specific == True:
+                #     # find a good initatlization, as other metrics would also depend on non-maximum logits
+                #     # also find a good init for accuary of sensitivty, to handle the corner cases, where making no prediction for specific classes.
+                #     model_pre = moval.models.init(
+                #         estim_algorithm,
+                #         mode = self.mode,
+                #         num_class = self.numclass,
+                #         confidence_scores = self.confidence_scores,
+                #         class_specific = False
+                #         )
+                #     solver_pre = moval.solvers.init("base-solver", model = model_pre, metric = "accuracy")
+                #     solver_pre.fit(logits, gt)
+                #     model.param = np.ones(self.numclass) * model_pre.param
 
                 solver = moval.solvers.init("base-solver", model = model, metric = self.metric)
                 solver.fit(logits, gt, batch) # model fitting
                 if self.metric == "precision" or self.metric == "auc":
                     probability_cond = model.calculate_probability(logits, appr = True, full = True) # ``(n, d)`` or a list of n ``(d, H, W, (D))``
                 else:
                     probability_cond = model.calculate_probability(logits, appr = True) # ``(n, d)`` or a list of n ``(d, H, W, (D))``
@@ -216,27 +217,28 @@
                 self.estim_algorithm,
                 mode = self.mode,
                 num_class = self.numclass,
                 confidence_scores = self.confidence_scores,
                 class_specific = self.class_specific
                 )
             
-            if self.class_specific == True:
-                # find a good initatlization, as other metrics would also depend on non-maximum logits
-                # also find a good init for accuary of sensitivty, to handle the corner cases, where making no prediction for specific classes.
-                model_pre = moval.models.init(
-                    self.estim_algorithm,
-                    mode = self.mode,
-                    num_class = self.numclass,
-                    confidence_scores = self.confidence_scores,
-                    class_specific = False
-                    )
-                solver_pre = moval.solvers.init("base-solver", model = model_pre, metric = "accuracy")
-                solver_pre.fit(logits, gt)
-                model.param = np.ones(self.numclass) * model_pre.param
+            # Zeju Li, 16 May 2024: The leads to weird behaviour of precision estimation, skip it now.
+            # if self.class_specific == True:
+            #     # find a good initatlization, as other metrics would also depend on non-maximum logits
+            #     # also find a good init, to handle the corner cases, where making no prediction for specific classes.
+            #     model_pre = moval.models.init(
+            #         self.estim_algorithm,
+            #         mode = self.mode,
+            #         num_class = self.numclass,
+            #         confidence_scores = self.confidence_scores,
+            #         class_specific = False
+            #         )
+            #     solver_pre = moval.solvers.init("base-solver", model = model_pre, metric = "accuracy")
+            #     solver_pre.fit(logits, gt)
+            #     model.param = np.ones(self.numclass) * model_pre.param
 
             solver = moval.solvers.init("base-solver", model = model, metric = self.metric)
             solver.fit(logits, gt, batch) # model fitting
 
             # save the results to self attributes.
             self.model_ = model
             self.solver_ = solver
```

### Comparing `moval-0.3.5/moval/models/confidences.py` & `moval-0.3.6/moval/models/confidences.py`

 * *Files identical despite different names*

### Comparing `moval-0.3.5/moval/models/model.py` & `moval-0.3.6/moval/models/model.py`

 * *Files identical despite different names*

### Comparing `moval-0.3.5/moval/models/solver_temperature.py` & `moval-0.3.6/moval/models/solver_temperature.py`

 * *Files identical despite different names*

### Comparing `moval-0.3.5/moval/models/utils.py` & `moval-0.3.6/moval/models/utils.py`

 * *Files identical despite different names*

### Comparing `moval-0.3.5/moval/registry.py` & `moval-0.3.6/moval/registry.py`

 * *Files identical despite different names*

### Comparing `moval-0.3.5/moval/solvers/criterions.py` & `moval-0.3.6/moval/solvers/criterions.py`

 * *Files identical despite different names*

### Comparing `moval-0.3.5/moval/solvers/solver.py` & `moval-0.3.6/moval/solvers/solver.py`

 * *Files 0% similar despite different names*

```diff
@@ -141,15 +141,15 @@
                 kcls_all.append(kcls)
 
             err = self.criterions(self.inp, self.gt, estim_perf_all, kcls_all)
 
         return err
 
     def kcls_order_list(self, inp: np.ndarray, exclusive_background: bool = False) -> List[Iterable]:
-        """Generate a list of kcls, such that the predicted samples are in ascending order.
+        """Generate a list of kcls, such that the predicted samples are in descending order.
 
         Args:
             inp: The network output (logits) of shape ``(n, d)`` for classification and a list of n ``(d, H, W, (D))`` for segmentation. 
             exclusive_background: If ``False``, we exclude the background class (the most majority class).
         
         Return:
             kcls_list: a list of class index. The first element should correspond to the most minority class.
@@ -167,15 +167,15 @@
                     pred_case = np.argmax(inp[n_case], axis = 0)
                     kcls_sample[kcls] = kcls_sample[kcls] + np.sum(pred_case == kcls)
         
         kcls_list = np.argsort(kcls_sample)
         if exclusive_background:
             kcls_list = kcls_list[:-1]
 
-        return kcls_list
+        return kcls_list[::-1]
 
     def fit(
         self,
         inp: Union[List[Iterable], np.ndarray],
         gt: Union[List[Iterable], np.ndarray],
         batch: int = 1
     ) -> Union[Tuple[np.ndarray, np.ndarray], np.ndarray]:
@@ -256,16 +256,14 @@
             print(f"Opitimizing with {len(inp)} samples...")
             print("Be patient, it should take a while...")
             if self.metric != "accuracy":
                 exclusive_background = True # leave the background class uncalibrated.
 
         # generate a list of length kcls, from high to low
         kcls_list = self.kcls_order_list(self.inp, exclusive_background)
-        if self.metric == "f1score":
-            kcls_list = kcls_list[::-1]
 
         if self.class_specific:
             
             if self.model.mode == "classification":
                 pred = np.argmax(inp, axis = 1)
             else:
                 preds = []
```

### Comparing `moval-0.3.5/moval/solvers/utils.py` & `moval-0.3.6/moval/solvers/utils.py`

 * *Files identical despite different names*

### Comparing `moval-0.3.5/moval.egg-info/PKG-INFO` & `moval-0.3.6/moval.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moval
-Version: 0.3.5
+Version: 0.3.6
 Summary: Model evaluation without manual labels
 Home-page: https://github.com/ZerojumpLine/MOVAL
 Author: Zeju Li
 Author-email: lizeju8@gmail.com
 Project-URL: Bug Tracker, https://github.com/ZerojumpLine/MOVAL/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: GPU :: NVIDIA CUDA
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: moval Version: 0.3.5 Summary: Model evaluation
+Metadata-Version: 2.1 Name: moval Version: 0.3.6 Summary: Model evaluation
 without manual labels Home-page: https://github.com/ZerojumpLine/MOVAL Author:
 Zeju Li Author-email: lizeju8@gmail.com Project-URL: Bug Tracker, https://
 github.com/ZerojumpLine/MOVAL/issues Classifier: Development Status :: 3 -
 Alpha Classifier: Environment :: GPU :: NVIDIA CUDA Classifier: Intended
 Audience :: Science/Research Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 Classifier: Topic ::
 Scientific/Engineering :: Artificial Intelligence Classifier: License :: Free
```

### Comparing `moval-0.3.5/moval.egg-info/SOURCES.txt` & `moval-0.3.6/moval.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `moval-0.3.5/pyproject.toml` & `moval-0.3.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `moval-0.3.5/setup.cfg` & `moval-0.3.6/setup.cfg`

 * *Files identical despite different names*

