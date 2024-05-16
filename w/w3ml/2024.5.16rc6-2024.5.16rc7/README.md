# Comparing `tmp/w3ml-2024.5.16rc6.tar.gz` & `tmp/w3ml-2024.5.16rc7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/w3ml-2024.5.16rc6.tar", last modified: Thu May 16 04:44:21 2024, max compression
+gzip compressed data, was "dist/w3ml-2024.5.16rc7.tar", last modified: Thu May 16 04:55:33 2024, max compression
```

## Comparing `w3ml-2024.5.16rc6.tar` & `w3ml-2024.5.16rc7.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 04:44:21.000000 w3ml-2024.5.16rc6/
--rw-r--r--   0 runner    (1001) docker     (127)      481 2024-05-16 04:44:21.000000 w3ml-2024.5.16rc6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-05-16 04:44:12.000000 w3ml-2024.5.16rc6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 04:44:21.000000 w3ml-2024.5.16rc6/w3ml/
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-16 04:44:12.000000 w3ml-2024.5.16rc6/w3ml/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 04:44:21.000000 w3ml-2024.5.16rc6/w3ml/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-16 04:44:12.000000 w3ml-2024.5.16rc6/w3ml/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 04:44:21.000000 w3ml-2024.5.16rc6/w3ml/models/
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-16 04:44:12.000000 w3ml-2024.5.16rc6/w3ml/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 04:44:21.000000 w3ml-2024.5.16rc6/w3ml/models/contrib/
--rw-r--r--   0 runner    (1001) docker     (127)      255 2024-05-16 04:44:12.000000 w3ml-2024.5.16rc6/w3ml/models/contrib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6220 2024-05-16 04:44:12.000000 w3ml-2024.5.16rc6/w3ml/models/contrib/automl_multilabel.py
--rw-r--r--   0 runner    (1001) docker     (127)    10240 2024-05-16 04:44:12.000000 w3ml-2024.5.16rc6/w3ml/models/contrib/automl_binary.py
--rw-r--r--   0 runner    (1001) docker     (127)     9527 2024-05-16 04:44:12.000000 w3ml-2024.5.16rc6/w3ml/models/contrib/automl_multiclass.py
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-16 04:44:12.000000 w3ml-2024.5.16rc6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 04:44:21.000000 w3ml-2024.5.16rc6/w3ml.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      481 2024-05-16 04:44:21.000000 w3ml-2024.5.16rc6/w3ml.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-16 04:44:21.000000 w3ml-2024.5.16rc6/w3ml.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-16 04:44:21.000000 w3ml-2024.5.16rc6/w3ml.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)      380 2024-05-16 04:44:21.000000 w3ml-2024.5.16rc6/w3ml.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 04:44:21.000000 w3ml-2024.5.16rc6/w3ml.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 04:44:21.000000 w3ml-2024.5.16rc6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-05-16 04:44:12.000000 w3ml-2024.5.16rc6/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 04:55:33.000000 w3ml-2024.5.16rc7/
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-05-16 04:55:33.000000 w3ml-2024.5.16rc7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-05-16 04:55:24.000000 w3ml-2024.5.16rc7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 04:55:33.000000 w3ml-2024.5.16rc7/w3ml/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-16 04:55:24.000000 w3ml-2024.5.16rc7/w3ml/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 04:55:33.000000 w3ml-2024.5.16rc7/w3ml/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-16 04:55:24.000000 w3ml-2024.5.16rc7/w3ml/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 04:55:33.000000 w3ml-2024.5.16rc7/w3ml/models/
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-16 04:55:24.000000 w3ml-2024.5.16rc7/w3ml/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 04:55:33.000000 w3ml-2024.5.16rc7/w3ml/models/contrib/
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2024-05-16 04:55:24.000000 w3ml-2024.5.16rc7/w3ml/models/contrib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6220 2024-05-16 04:55:24.000000 w3ml-2024.5.16rc7/w3ml/models/contrib/automl_multilabel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10516 2024-05-16 04:55:24.000000 w3ml-2024.5.16rc7/w3ml/models/contrib/automl_binary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9527 2024-05-16 04:55:24.000000 w3ml-2024.5.16rc7/w3ml/models/contrib/automl_multiclass.py
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-16 04:55:24.000000 w3ml-2024.5.16rc7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 04:55:33.000000 w3ml-2024.5.16rc7/w3ml.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-05-16 04:55:33.000000 w3ml-2024.5.16rc7/w3ml.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-16 04:55:33.000000 w3ml-2024.5.16rc7/w3ml.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-16 04:55:33.000000 w3ml-2024.5.16rc7/w3ml.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-05-16 04:55:33.000000 w3ml-2024.5.16rc7/w3ml.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 04:55:33.000000 w3ml-2024.5.16rc7/w3ml.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 04:55:33.000000 w3ml-2024.5.16rc7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-05-16 04:55:24.000000 w3ml-2024.5.16rc7/LICENSE
```

### Comparing `w3ml-2024.5.16rc6/setup.py` & `w3ml-2024.5.16rc7/setup.py`

 * *Files identical despite different names*

### Comparing `w3ml-2024.5.16rc6/w3ml/models/contrib/automl_multilabel.py` & `w3ml-2024.5.16rc7/w3ml/models/contrib/automl_multilabel.py`

 * *Files identical despite different names*

### Comparing `w3ml-2024.5.16rc6/w3ml/models/contrib/automl_binary.py` & `w3ml-2024.5.16rc7/w3ml/models/contrib/automl_binary.py`

 * *Files 3% similar despite different names*

```diff
@@ -68,14 +68,18 @@
         my_model_v1.fit()
         # 성능 확인
         print(my_model_v1.evaluate(test_data))
         print(my_model_v1.get_feature_importance(test_data))
         # predict 테스트
         print(my_model_v1.batch_prediction(test_data, "predict"))
         """
+        assert isinstance(model_name, str), "`model_name(는) str 타입이어야 합니다.`"
+        assert isinstance(model_version, str), "`model_version(는) str 타입이어야 합니다.`"
+        self.model_name = model_name
+        self.model_version = model_version
         assert isinstance(
             train_data, pd.DataFrame
         ), "`train_data은(는) pd.DataFrame 타입이어야 합니다.`"
         assert isinstance(label, str), "`label(는) str 타입이어야 합니다.`"
         assert isinstance(
             non_training_features, list
         ), "`non_training_features은(는) list 타입이어야 합니다.`"
```

### Comparing `w3ml-2024.5.16rc6/w3ml/models/contrib/automl_multiclass.py` & `w3ml-2024.5.16rc7/w3ml/models/contrib/automl_multiclass.py`

 * *Files identical despite different names*

### Comparing `w3ml-2024.5.16rc6/LICENSE` & `w3ml-2024.5.16rc7/LICENSE`

 * *Files identical despite different names*

