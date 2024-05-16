# Comparing `tmp/w3ml-2024.5.16rc7.tar.gz` & `tmp/w3ml-2024.5.16rc8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/w3ml-2024.5.16rc7.tar", last modified: Thu May 16 04:55:33 2024, max compression
+gzip compressed data, was "dist/w3ml-2024.5.16rc8.tar", last modified: Thu May 16 05:11:36 2024, max compression
```

## Comparing `w3ml-2024.5.16rc7.tar` & `w3ml-2024.5.16rc8.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 04:55:33.000000 w3ml-2024.5.16rc7/
--rw-r--r--   0 runner    (1001) docker     (127)      481 2024-05-16 04:55:33.000000 w3ml-2024.5.16rc7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-05-16 04:55:24.000000 w3ml-2024.5.16rc7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 04:55:33.000000 w3ml-2024.5.16rc7/w3ml/
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-16 04:55:24.000000 w3ml-2024.5.16rc7/w3ml/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 04:55:33.000000 w3ml-2024.5.16rc7/w3ml/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-16 04:55:24.000000 w3ml-2024.5.16rc7/w3ml/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 04:55:33.000000 w3ml-2024.5.16rc7/w3ml/models/
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-16 04:55:24.000000 w3ml-2024.5.16rc7/w3ml/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 04:55:33.000000 w3ml-2024.5.16rc7/w3ml/models/contrib/
--rw-r--r--   0 runner    (1001) docker     (127)      255 2024-05-16 04:55:24.000000 w3ml-2024.5.16rc7/w3ml/models/contrib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6220 2024-05-16 04:55:24.000000 w3ml-2024.5.16rc7/w3ml/models/contrib/automl_multilabel.py
--rw-r--r--   0 runner    (1001) docker     (127)    10516 2024-05-16 04:55:24.000000 w3ml-2024.5.16rc7/w3ml/models/contrib/automl_binary.py
--rw-r--r--   0 runner    (1001) docker     (127)     9527 2024-05-16 04:55:24.000000 w3ml-2024.5.16rc7/w3ml/models/contrib/automl_multiclass.py
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-16 04:55:24.000000 w3ml-2024.5.16rc7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 04:55:33.000000 w3ml-2024.5.16rc7/w3ml.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      481 2024-05-16 04:55:33.000000 w3ml-2024.5.16rc7/w3ml.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-16 04:55:33.000000 w3ml-2024.5.16rc7/w3ml.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-16 04:55:33.000000 w3ml-2024.5.16rc7/w3ml.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)      380 2024-05-16 04:55:33.000000 w3ml-2024.5.16rc7/w3ml.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 04:55:33.000000 w3ml-2024.5.16rc7/w3ml.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 04:55:33.000000 w3ml-2024.5.16rc7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-05-16 04:55:24.000000 w3ml-2024.5.16rc7/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 05:11:36.000000 w3ml-2024.5.16rc8/
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-05-16 05:11:36.000000 w3ml-2024.5.16rc8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-05-16 05:11:28.000000 w3ml-2024.5.16rc8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 05:11:36.000000 w3ml-2024.5.16rc8/w3ml/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-16 05:11:28.000000 w3ml-2024.5.16rc8/w3ml/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 05:11:36.000000 w3ml-2024.5.16rc8/w3ml/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-16 05:11:28.000000 w3ml-2024.5.16rc8/w3ml/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 05:11:36.000000 w3ml-2024.5.16rc8/w3ml/models/
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-16 05:11:28.000000 w3ml-2024.5.16rc8/w3ml/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 05:11:36.000000 w3ml-2024.5.16rc8/w3ml/models/contrib/
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2024-05-16 05:11:28.000000 w3ml-2024.5.16rc8/w3ml/models/contrib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6220 2024-05-16 05:11:28.000000 w3ml-2024.5.16rc8/w3ml/models/contrib/automl_multilabel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10696 2024-05-16 05:11:28.000000 w3ml-2024.5.16rc8/w3ml/models/contrib/automl_binary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9527 2024-05-16 05:11:28.000000 w3ml-2024.5.16rc8/w3ml/models/contrib/automl_multiclass.py
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-16 05:11:28.000000 w3ml-2024.5.16rc8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 05:11:36.000000 w3ml-2024.5.16rc8/w3ml.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-05-16 05:11:36.000000 w3ml-2024.5.16rc8/w3ml.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-16 05:11:36.000000 w3ml-2024.5.16rc8/w3ml.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-16 05:11:36.000000 w3ml-2024.5.16rc8/w3ml.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-05-16 05:11:36.000000 w3ml-2024.5.16rc8/w3ml.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 05:11:36.000000 w3ml-2024.5.16rc8/w3ml.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 05:11:36.000000 w3ml-2024.5.16rc8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-05-16 05:11:28.000000 w3ml-2024.5.16rc8/LICENSE
```

### Comparing `w3ml-2024.5.16rc7/setup.py` & `w3ml-2024.5.16rc8/setup.py`

 * *Files identical despite different names*

### Comparing `w3ml-2024.5.16rc7/w3ml/models/contrib/automl_multilabel.py` & `w3ml-2024.5.16rc8/w3ml/models/contrib/automl_multilabel.py`

 * *Files identical despite different names*

### Comparing `w3ml-2024.5.16rc7/w3ml/models/contrib/automl_binary.py` & `w3ml-2024.5.16rc8/w3ml/models/contrib/automl_binary.py`

 * *Files 2% similar despite different names*

```diff
@@ -91,21 +91,25 @@
             self.path = MODEL_DIR.joinpath(self.model_name, self.model_version)
         else:
             assert isinstance(path, str), "`path(는) str 타입이어야 합니다.`"
             self.path = path
 
         assert isinstance(presets, str), "`presets(는) str 타입이어야 합니다.`"
         assert presets in ['best_quality', 'high_quality', 'good_quality', 'medium_quality', 'optimize_for_deployment']
+        
+        assert isinstance(keep_only_best, bool), "`presets(는) str 타입이어야 합니다.`"
+        
         self.presets = presets
         self.train_data = train_data
         self.label = label
         self.non_training_features = non_training_features
         self.eval_metric = eval_metric
         self.time_limit = time_limit
         self.excluded_model_types = excluded_model_types
+        self.keep_only_best = keep_only_best
 
     def fit(self):
         try:
             self.models = self._fit()
             os.rmdir(self.path)
         except Exception as e:
             os.rmdir(self.path)
@@ -119,19 +123,19 @@
             label=self.label,
             eval_metric=self.eval_metric,
             path=self.path,
             sample_weight="balance_weight",
             verbosity=0,
         )
         return predictor.fit(
-            train_data=train_data[columns],
+            train_data=self.train_data[columns],
             presets=self.presets,
             time_limit=self.time_limit,
             excluded_model_types=self.excluded_model_types,
-            keep_only_best=True,
+            keep_only_best=self.keep_only_best,
         )
 
     def batch_prediction(self, batch_data: pd.DataFrame, predict_fn) -> pd.DataFrame:
         """
         학습한 모델의 배치 예측을 지원합니다.
         ## 참고 사항
         - `fit` 함수를 통해 학습이 된 경우에만 정상적으로 동작합니다.
```

### Comparing `w3ml-2024.5.16rc7/w3ml/models/contrib/automl_multiclass.py` & `w3ml-2024.5.16rc8/w3ml/models/contrib/automl_multiclass.py`

 * *Files identical despite different names*

### Comparing `w3ml-2024.5.16rc7/LICENSE` & `w3ml-2024.5.16rc8/LICENSE`

 * *Files identical despite different names*

