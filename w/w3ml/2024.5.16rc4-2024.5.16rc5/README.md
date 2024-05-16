# Comparing `tmp/w3ml-2024.5.16rc4.tar.gz` & `tmp/w3ml-2024.5.16rc5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/w3ml-2024.5.16rc4.tar", last modified: Thu May 16 04:05:21 2024, max compression
+gzip compressed data, was "dist/w3ml-2024.5.16rc5.tar", last modified: Thu May 16 04:29:06 2024, max compression
```

## Comparing `w3ml-2024.5.16rc4.tar` & `w3ml-2024.5.16rc5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 04:05:21.000000 w3ml-2024.5.16rc4/
--rw-r--r--   0 runner    (1001) docker     (127)      481 2024-05-16 04:05:21.000000 w3ml-2024.5.16rc4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-05-16 04:05:13.000000 w3ml-2024.5.16rc4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 04:05:21.000000 w3ml-2024.5.16rc4/w3ml/
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-16 04:05:13.000000 w3ml-2024.5.16rc4/w3ml/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 04:05:21.000000 w3ml-2024.5.16rc4/w3ml/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-16 04:05:13.000000 w3ml-2024.5.16rc4/w3ml/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 04:05:21.000000 w3ml-2024.5.16rc4/w3ml/models/
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-16 04:05:13.000000 w3ml-2024.5.16rc4/w3ml/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 04:05:21.000000 w3ml-2024.5.16rc4/w3ml/models/contrib/
--rw-r--r--   0 runner    (1001) docker     (127)      255 2024-05-16 04:05:13.000000 w3ml-2024.5.16rc4/w3ml/models/contrib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6220 2024-05-16 04:05:13.000000 w3ml-2024.5.16rc4/w3ml/models/contrib/automl_multilabel.py
--rw-r--r--   0 runner    (1001) docker     (127)    10188 2024-05-16 04:05:13.000000 w3ml-2024.5.16rc4/w3ml/models/contrib/automl_binary.py
--rw-r--r--   0 runner    (1001) docker     (127)     9527 2024-05-16 04:05:13.000000 w3ml-2024.5.16rc4/w3ml/models/contrib/automl_multiclass.py
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-16 04:05:13.000000 w3ml-2024.5.16rc4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 04:05:21.000000 w3ml-2024.5.16rc4/w3ml.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      481 2024-05-16 04:05:21.000000 w3ml-2024.5.16rc4/w3ml.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-16 04:05:21.000000 w3ml-2024.5.16rc4/w3ml.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-16 04:05:21.000000 w3ml-2024.5.16rc4/w3ml.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)      380 2024-05-16 04:05:21.000000 w3ml-2024.5.16rc4/w3ml.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 04:05:21.000000 w3ml-2024.5.16rc4/w3ml.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 04:05:21.000000 w3ml-2024.5.16rc4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-05-16 04:05:13.000000 w3ml-2024.5.16rc4/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 04:29:06.000000 w3ml-2024.5.16rc5/
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-05-16 04:29:06.000000 w3ml-2024.5.16rc5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-05-16 04:28:57.000000 w3ml-2024.5.16rc5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 04:29:06.000000 w3ml-2024.5.16rc5/w3ml/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-16 04:28:57.000000 w3ml-2024.5.16rc5/w3ml/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 04:29:06.000000 w3ml-2024.5.16rc5/w3ml/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-16 04:28:57.000000 w3ml-2024.5.16rc5/w3ml/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 04:29:06.000000 w3ml-2024.5.16rc5/w3ml/models/
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-16 04:28:57.000000 w3ml-2024.5.16rc5/w3ml/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 04:29:06.000000 w3ml-2024.5.16rc5/w3ml/models/contrib/
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2024-05-16 04:28:57.000000 w3ml-2024.5.16rc5/w3ml/models/contrib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6220 2024-05-16 04:28:57.000000 w3ml-2024.5.16rc5/w3ml/models/contrib/automl_multilabel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10240 2024-05-16 04:28:57.000000 w3ml-2024.5.16rc5/w3ml/models/contrib/automl_binary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9527 2024-05-16 04:28:57.000000 w3ml-2024.5.16rc5/w3ml/models/contrib/automl_multiclass.py
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-16 04:28:57.000000 w3ml-2024.5.16rc5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 04:29:06.000000 w3ml-2024.5.16rc5/w3ml.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-05-16 04:29:06.000000 w3ml-2024.5.16rc5/w3ml.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-16 04:29:06.000000 w3ml-2024.5.16rc5/w3ml.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-16 04:29:06.000000 w3ml-2024.5.16rc5/w3ml.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-05-16 04:29:06.000000 w3ml-2024.5.16rc5/w3ml.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 04:29:06.000000 w3ml-2024.5.16rc5/w3ml.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 04:29:06.000000 w3ml-2024.5.16rc5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-05-16 04:28:57.000000 w3ml-2024.5.16rc5/LICENSE
```

### Comparing `w3ml-2024.5.16rc4/setup.py` & `w3ml-2024.5.16rc5/setup.py`

 * *Files identical despite different names*

### Comparing `w3ml-2024.5.16rc4/w3ml/models/contrib/automl_multilabel.py` & `w3ml-2024.5.16rc5/w3ml/models/contrib/automl_multilabel.py`

 * *Files identical despite different names*

### Comparing `w3ml-2024.5.16rc4/w3ml/models/contrib/automl_binary.py` & `w3ml-2024.5.16rc5/w3ml/models/contrib/automl_binary.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
             "TRANSF",
             "custom",
         ],
         keep_only_best =True,
     ):
         """
         2024.06.01 v1 개발
-        Contact : 이규남(kyunam@sk.com), 김태형(th0804@sk.com), 강예진(yejin.k@sk.com), 정유철(jungyc@sk.com), 진기훈(kh.jin@sk.com)
+        Contact : 이규남(kyunam@sk.com), 김태형(th0804@sk.com), 강예진(yejin.k@sk.com), 정유철(jungyc@sk.com), 진기훈(kh.jin@sk.com), 송지영(jiyoung.song@sk.com)
 
         AutoML을 통해 모델을 학습합니다.
         Class의 개수는 Multi가 아니라 2개 까지 지원합니다. 3개 이상의 Class는 타 함수를 참조바랍니다.
 
         ## 참고 사항
         - AutoML이 자동으로 학습합니다.
         - 성능 지표를 설정할 수 있으나, 분류 문제의 경우 기본값인 `roc_auc` 사용을 권장합니다.
@@ -185,10 +185,10 @@
         assert isinstance(
             test_data, pd.DataFrame
         ), "`test_data(는) pd.DataFrame 타입이어야 합니다.`"
         assert isinstance(feature_importance_time_limit, int), "`feature_importance_time_limit(는) int 타입이어야 합니다.`"
         columns = [f for f in self.models.features()] + [
             self.label
         ]
-        return self.models.feature_importance(test_data[columns], silent=True, feature_importance_time_limit)[
+        return self.models.feature_importance(time_limit = feature_importance_time_limit, data = test_data[columns], silent=True)[
             "importance"
         ]
```

### Comparing `w3ml-2024.5.16rc4/w3ml/models/contrib/automl_multiclass.py` & `w3ml-2024.5.16rc5/w3ml/models/contrib/automl_multiclass.py`

 * *Files identical despite different names*

### Comparing `w3ml-2024.5.16rc4/LICENSE` & `w3ml-2024.5.16rc5/LICENSE`

 * *Files identical despite different names*

