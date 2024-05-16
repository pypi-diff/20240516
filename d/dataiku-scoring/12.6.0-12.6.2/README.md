# Comparing `tmp/dataiku-scoring-12.6.0.tar.gz` & `tmp/dataiku-scoring-12.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dataiku-scoring-12.6.0.tar", last modified: Tue Apr  9 08:28:48 2024, max compression
+gzip compressed data, was "dataiku-scoring-12.6.2.tar", last modified: Thu May 16 13:21:47 2024, max compression
```

## Comparing `dataiku-scoring-12.6.0.tar` & `dataiku-scoring-12.6.2.tar`

### file list

```diff
@@ -1,78 +1,78 @@
-drwxr-xr-x   0 kevin.remy@dataiku.com   (502) staff       (20)        0 2024-04-09 08:28:48.012688 dataiku-scoring-12.6.0/
--rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)      995 2024-04-09 08:28:29.000000 dataiku-scoring-12.6.0/HISTORY.txt
--rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)      524 2024-01-15 09:52:42.000000 dataiku-scoring-12.6.0/LICENSE.txt
--rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)       65 2024-01-15 09:52:42.000000 dataiku-scoring-12.6.0/MANIFEST.in
--rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)       27 2024-01-15 09:52:42.000000 dataiku-scoring-12.6.0/NOTICE.txt
--rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)     1813 2024-04-09 08:28:48.011979 dataiku-scoring-12.6.0/PKG-INFO
--rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)      214 2024-01-15 09:52:42.000000 dataiku-scoring-12.6.0/README.md
-drwxr-xr-x   0 kevin.remy@dataiku.com   (502) staff       (20)        0 2024-04-09 08:28:48.011253 dataiku-scoring-12.6.0/dataiku_scoring.egg-info/
--rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)     1813 2024-04-09 08:28:47.000000 dataiku-scoring-12.6.0/dataiku_scoring.egg-info/PKG-INFO
--rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)     2506 2024-04-09 08:28:47.000000 dataiku-scoring-12.6.0/dataiku_scoring.egg-info/SOURCES.txt
--rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)        1 2024-04-09 08:28:47.000000 dataiku-scoring-12.6.0/dataiku_scoring.egg-info/dependency_links.txt
--rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)        6 2024-04-09 08:28:47.000000 dataiku-scoring-12.6.0/dataiku_scoring.egg-info/requires.txt
--rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)       15 2024-04-09 08:28:47.000000 dataiku-scoring-12.6.0/dataiku_scoring.egg-info/top_level.txt
-drwxr-xr-x   0 kevin.remy@dataiku.com   (502) staff       (20)        0 2024-04-09 08:28:47.675845 dataiku-scoring-12.6.0/dataikuscoring/
--rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)     1069 2023-12-14 11:08:55.000000 dataiku-scoring-12.6.0/dataikuscoring/__init__.py
-drwxr-xr-x   0 kevin.remy@dataiku.com   (502) staff       (20)        0 2024-04-09 08:28:47.772009 dataiku-scoring-12.6.0/dataikuscoring/algorithms/
--rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)      903 2023-12-14 11:08:55.000000 dataiku-scoring-12.6.0/dataikuscoring/algorithms/__init__.py
--rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)      576 2023-12-14 11:08:55.000000 dataiku-scoring-12.6.0/dataikuscoring/algorithms/common.py
--rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)     5451 2024-04-09 08:28:29.000000 dataiku-scoring-12.6.0/dataikuscoring/algorithms/decision_tree_model.py
--rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)      708 2023-12-14 11:08:55.000000 dataiku-scoring-12.6.0/dataikuscoring/algorithms/forest_classifier.py
--rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)      672 2023-12-14 11:08:55.000000 dataiku-scoring-12.6.0/dataikuscoring/algorithms/forest_regressor.py
--rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)     1157 2023-12-14 11:08:55.000000 dataiku-scoring-12.6.0/dataikuscoring/algorithms/generic_mlp.py
--rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)     1558 2024-04-09 08:28:29.000000 dataiku-scoring-12.6.0/dataikuscoring/algorithms/gradient_boosting_classifier.py
--rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)     1103 2023-12-14 11:08:55.000000 dataiku-scoring-12.6.0/dataikuscoring/algorithms/gradient_boosting_regressor.py
--rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)      429 2023-12-14 11:08:55.000000 dataiku-scoring-12.6.0/dataikuscoring/algorithms/linear_regression.py
--rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)     1597 2023-12-14 11:08:55.000000 dataiku-scoring-12.6.0/dataikuscoring/algorithms/logistic.py
--rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)      848 2023-12-14 11:08:55.000000 dataiku-scoring-12.6.0/dataikuscoring/algorithms/mlp_classifier.py
--rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)      258 2023-12-14 11:08:55.000000 dataiku-scoring-12.6.0/dataikuscoring/algorithms/mlp_regressor.py
--rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)    10063 2024-04-09 08:28:29.000000 dataiku-scoring-12.6.0/dataikuscoring/load.py
-drwxr-xr-x   0 kevin.remy@dataiku.com   (502) staff       (20)        0 2024-04-09 08:28:47.796887 dataiku-scoring-12.6.0/dataikuscoring/mlflow/
--rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)      681 2023-12-14 11:08:55.000000 dataiku-scoring-12.6.0/dataikuscoring/mlflow/__init__.py
--rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)    12865 2024-04-03 18:04:59.000000 dataiku-scoring-12.6.0/dataikuscoring/mlflow/classification.py
--rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)     7936 2023-12-14 11:08:55.000000 dataiku-scoring-12.6.0/dataikuscoring/mlflow/common.py
--rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)    11001 2023-12-14 11:08:55.000000 dataiku-scoring-12.6.0/dataikuscoring/mlflow/dss_flavor.py
--rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)     2656 2023-12-14 11:08:55.000000 dataiku-scoring-12.6.0/dataikuscoring/mlflow/regression.py
-drwxr-xr-x   0 kevin.remy@dataiku.com   (502) staff       (20)        0 2024-04-09 08:28:47.830277 dataiku-scoring-12.6.0/dataikuscoring/models/
--rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)      635 2023-12-14 11:08:55.000000 dataiku-scoring-12.6.0/dataikuscoring/models/__init__.py
--rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)      880 2023-12-14 11:08:55.000000 dataiku-scoring-12.6.0/dataikuscoring/models/binary.py
--rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)     2409 2023-12-14 11:08:55.000000 dataiku-scoring-12.6.0/dataikuscoring/models/common.py
--rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)     2609 2023-12-14 11:08:55.000000 dataiku-scoring-12.6.0/dataikuscoring/models/mlflow.py
--rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)     3964 2023-12-14 11:08:55.000000 dataiku-scoring-12.6.0/dataikuscoring/models/model.py
--rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)      334 2023-12-14 11:08:55.000000 dataiku-scoring-12.6.0/dataikuscoring/models/multiclass.py
--rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)     7552 2023-12-14 11:08:55.000000 dataiku-scoring-12.6.0/dataikuscoring/models/partitioned.py
--rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)      205 2023-12-14 11:08:55.000000 dataiku-scoring-12.6.0/dataikuscoring/models/regression.py
-drwxr-xr-x   0 kevin.remy@dataiku.com   (502) staff       (20)        0 2024-04-09 08:28:47.936041 dataiku-scoring-12.6.0/dataikuscoring/processors/
--rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)     1241 2023-12-14 11:08:55.000000 dataiku-scoring-12.6.0/dataikuscoring/processors/__init__.py
--rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)      711 2023-12-14 11:08:55.000000 dataiku-scoring-12.6.0/dataikuscoring/processors/binarize.py
--rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)     2863 2023-12-14 11:08:55.000000 dataiku-scoring-12.6.0/dataikuscoring/processors/calibration.py
--rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)     1047 2023-12-14 11:08:55.000000 dataiku-scoring-12.6.0/dataikuscoring/processors/cat_cat_interaction.py
--rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)     1399 2023-12-14 11:08:55.000000 dataiku-scoring-12.6.0/dataikuscoring/processors/categorical_encode.py
--rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)     2098 2023-12-14 11:08:55.000000 dataiku-scoring-12.6.0/dataikuscoring/processors/datetime_cyclical.py
--rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)     1290 2023-12-14 11:08:55.000000 dataiku-scoring-12.6.0/dataikuscoring/processors/derive.py
--rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)     2080 2023-12-14 11:08:55.000000 dataiku-scoring-12.6.0/dataikuscoring/processors/derive_rescale.py
--rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)      995 2023-12-14 11:08:55.000000 dataiku-scoring-12.6.0/dataikuscoring/processors/drop_rows.py
--rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)     1222 2024-04-09 08:28:29.000000 dataiku-scoring-12.6.0/dataikuscoring/processors/dummify.py
--rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)      850 2024-04-09 08:28:29.000000 dataiku-scoring-12.6.0/dataikuscoring/processors/flag.py
--rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)     1205 2023-12-14 11:08:55.000000 dataiku-scoring-12.6.0/dataikuscoring/processors/impute.py
--rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)     1423 2023-12-14 11:08:55.000000 dataiku-scoring-12.6.0/dataikuscoring/processors/normalize.py
--rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)      864 2023-12-14 11:08:55.000000 dataiku-scoring-12.6.0/dataikuscoring/processors/num_cat_interaction.py
--rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)     1023 2023-12-14 11:08:55.000000 dataiku-scoring-12.6.0/dataikuscoring/processors/num_num_interaction.py
--rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)     5038 2023-12-14 11:08:55.000000 dataiku-scoring-12.6.0/dataikuscoring/processors/prepare_input.py
--rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)     1493 2024-04-09 08:28:29.000000 dataiku-scoring-12.6.0/dataikuscoring/processors/preprocessings.py
--rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)      996 2023-12-14 11:08:55.000000 dataiku-scoring-12.6.0/dataikuscoring/processors/preprocessor.py
--rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)      928 2023-12-14 11:08:55.000000 dataiku-scoring-12.6.0/dataikuscoring/processors/rescale.py
--rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)     1682 2024-04-09 08:28:29.000000 dataiku-scoring-12.6.0/dataikuscoring/processors/selection.py
--rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)     2471 2023-12-14 11:08:55.000000 dataiku-scoring-12.6.0/dataikuscoring/processors/vectorize_tfidf.py
--rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)     1246 2023-12-14 11:08:55.000000 dataiku-scoring-12.6.0/dataikuscoring/processors/vectorize_word_count.py
--rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)      783 2023-12-14 11:08:55.000000 dataiku-scoring-12.6.0/dataikuscoring/processors/vectors_unfold.py
-drwxr-xr-x   0 kevin.remy@dataiku.com   (502) staff       (20)        0 2024-04-09 08:28:48.010453 dataiku-scoring-12.6.0/dataikuscoring/utils/
--rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)      242 2023-12-14 11:08:55.000000 dataiku-scoring-12.6.0/dataikuscoring/utils/__init__.py
--rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)     2323 2023-12-14 11:08:55.000000 dataiku-scoring-12.6.0/dataikuscoring/utils/indexed_matrix.py
--rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)      239 2023-12-14 11:08:55.000000 dataiku-scoring-12.6.0/dataikuscoring/utils/math_utils.py
--rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)     8696 2024-04-09 08:28:29.000000 dataiku-scoring-12.6.0/dataikuscoring/utils/prediction_result.py
--rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)     1379 2023-12-14 11:08:55.000000 dataiku-scoring-12.6.0/dataikuscoring/utils/scoring_data.py
--rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)     1413 2023-12-14 11:08:55.000000 dataiku-scoring-12.6.0/dataikuscoring/utils/tokenizer.py
--rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)        6 2024-01-15 09:52:42.000000 dataiku-scoring-12.6.0/requirements.txt
--rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)       38 2024-04-09 08:28:48.012803 dataiku-scoring-12.6.0/setup.cfg
--rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)      876 2024-04-09 08:28:29.000000 dataiku-scoring-12.6.0/setup.py
+drwxr-xr-x   0 kevin.remy@dataiku.com   (502) staff       (20)        0 2024-05-16 13:21:47.456348 dataiku-scoring-12.6.2/
+-rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)     1070 2024-05-16 13:21:19.000000 dataiku-scoring-12.6.2/HISTORY.txt
+-rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)      524 2024-01-15 09:52:42.000000 dataiku-scoring-12.6.2/LICENSE.txt
+-rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)       65 2024-01-15 09:52:42.000000 dataiku-scoring-12.6.2/MANIFEST.in
+-rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)       27 2024-01-15 09:52:42.000000 dataiku-scoring-12.6.2/NOTICE.txt
+-rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)     1888 2024-05-16 13:21:47.453910 dataiku-scoring-12.6.2/PKG-INFO
+-rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)      214 2024-01-15 09:52:42.000000 dataiku-scoring-12.6.2/README.md
+drwxr-xr-x   0 kevin.remy@dataiku.com   (502) staff       (20)        0 2024-05-16 13:21:47.446585 dataiku-scoring-12.6.2/dataiku_scoring.egg-info/
+-rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)     1888 2024-05-16 13:21:46.000000 dataiku-scoring-12.6.2/dataiku_scoring.egg-info/PKG-INFO
+-rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)     2506 2024-05-16 13:21:46.000000 dataiku-scoring-12.6.2/dataiku_scoring.egg-info/SOURCES.txt
+-rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)        1 2024-05-16 13:21:46.000000 dataiku-scoring-12.6.2/dataiku_scoring.egg-info/dependency_links.txt
+-rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)        6 2024-05-16 13:21:46.000000 dataiku-scoring-12.6.2/dataiku_scoring.egg-info/requires.txt
+-rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)       15 2024-05-16 13:21:46.000000 dataiku-scoring-12.6.2/dataiku_scoring.egg-info/top_level.txt
+drwxr-xr-x   0 kevin.remy@dataiku.com   (502) staff       (20)        0 2024-05-16 13:21:46.540478 dataiku-scoring-12.6.2/dataikuscoring/
+-rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)     1069 2023-12-14 11:08:55.000000 dataiku-scoring-12.6.2/dataikuscoring/__init__.py
+drwxr-xr-x   0 kevin.remy@dataiku.com   (502) staff       (20)        0 2024-05-16 13:21:46.793959 dataiku-scoring-12.6.2/dataikuscoring/algorithms/
+-rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)      903 2023-12-14 11:08:55.000000 dataiku-scoring-12.6.2/dataikuscoring/algorithms/__init__.py
+-rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)      576 2023-12-14 11:08:55.000000 dataiku-scoring-12.6.2/dataikuscoring/algorithms/common.py
+-rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)     5595 2024-05-16 13:21:19.000000 dataiku-scoring-12.6.2/dataikuscoring/algorithms/decision_tree_model.py
+-rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)      708 2023-12-14 11:08:55.000000 dataiku-scoring-12.6.2/dataikuscoring/algorithms/forest_classifier.py
+-rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)      672 2023-12-14 11:08:55.000000 dataiku-scoring-12.6.2/dataikuscoring/algorithms/forest_regressor.py
+-rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)     1157 2023-12-14 11:08:55.000000 dataiku-scoring-12.6.2/dataikuscoring/algorithms/generic_mlp.py
+-rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)     2602 2024-05-16 13:21:19.000000 dataiku-scoring-12.6.2/dataikuscoring/algorithms/gradient_boosting_classifier.py
+-rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)     1550 2024-05-16 13:21:19.000000 dataiku-scoring-12.6.2/dataikuscoring/algorithms/gradient_boosting_regressor.py
+-rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)      429 2023-12-14 11:08:55.000000 dataiku-scoring-12.6.2/dataikuscoring/algorithms/linear_regression.py
+-rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)     1597 2023-12-14 11:08:55.000000 dataiku-scoring-12.6.2/dataikuscoring/algorithms/logistic.py
+-rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)      848 2023-12-14 11:08:55.000000 dataiku-scoring-12.6.2/dataikuscoring/algorithms/mlp_classifier.py
+-rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)      258 2023-12-14 11:08:55.000000 dataiku-scoring-12.6.2/dataikuscoring/algorithms/mlp_regressor.py
+-rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)    10063 2024-04-05 11:14:40.000000 dataiku-scoring-12.6.2/dataikuscoring/load.py
+drwxr-xr-x   0 kevin.remy@dataiku.com   (502) staff       (20)        0 2024-05-16 13:21:46.870359 dataiku-scoring-12.6.2/dataikuscoring/mlflow/
+-rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)      681 2023-12-14 11:08:55.000000 dataiku-scoring-12.6.2/dataikuscoring/mlflow/__init__.py
+-rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)    12865 2024-04-03 18:04:59.000000 dataiku-scoring-12.6.2/dataikuscoring/mlflow/classification.py
+-rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)     7936 2023-12-14 11:08:55.000000 dataiku-scoring-12.6.2/dataikuscoring/mlflow/common.py
+-rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)    11001 2024-05-14 07:35:38.000000 dataiku-scoring-12.6.2/dataikuscoring/mlflow/dss_flavor.py
+-rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)     2656 2023-12-14 11:08:55.000000 dataiku-scoring-12.6.2/dataikuscoring/mlflow/regression.py
+drwxr-xr-x   0 kevin.remy@dataiku.com   (502) staff       (20)        0 2024-05-16 13:21:47.002169 dataiku-scoring-12.6.2/dataikuscoring/models/
+-rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)      635 2023-12-14 11:08:55.000000 dataiku-scoring-12.6.2/dataikuscoring/models/__init__.py
+-rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)      880 2023-12-14 11:08:55.000000 dataiku-scoring-12.6.2/dataikuscoring/models/binary.py
+-rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)     2409 2023-12-14 11:08:55.000000 dataiku-scoring-12.6.2/dataikuscoring/models/common.py
+-rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)     2609 2023-12-14 11:08:55.000000 dataiku-scoring-12.6.2/dataikuscoring/models/mlflow.py
+-rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)     3964 2023-12-14 11:08:55.000000 dataiku-scoring-12.6.2/dataikuscoring/models/model.py
+-rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)      334 2023-12-14 11:08:55.000000 dataiku-scoring-12.6.2/dataikuscoring/models/multiclass.py
+-rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)     7552 2023-12-14 11:08:55.000000 dataiku-scoring-12.6.2/dataikuscoring/models/partitioned.py
+-rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)      205 2023-12-14 11:08:55.000000 dataiku-scoring-12.6.2/dataikuscoring/models/regression.py
+drwxr-xr-x   0 kevin.remy@dataiku.com   (502) staff       (20)        0 2024-05-16 13:21:47.386255 dataiku-scoring-12.6.2/dataikuscoring/processors/
+-rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)     1241 2023-12-14 11:08:55.000000 dataiku-scoring-12.6.2/dataikuscoring/processors/__init__.py
+-rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)      711 2023-12-14 11:08:55.000000 dataiku-scoring-12.6.2/dataikuscoring/processors/binarize.py
+-rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)     2863 2023-12-14 11:08:55.000000 dataiku-scoring-12.6.2/dataikuscoring/processors/calibration.py
+-rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)     1047 2023-12-14 11:08:55.000000 dataiku-scoring-12.6.2/dataikuscoring/processors/cat_cat_interaction.py
+-rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)     1399 2023-12-14 11:08:55.000000 dataiku-scoring-12.6.2/dataikuscoring/processors/categorical_encode.py
+-rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)     2098 2023-12-14 11:08:55.000000 dataiku-scoring-12.6.2/dataikuscoring/processors/datetime_cyclical.py
+-rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)     1290 2023-12-14 11:08:55.000000 dataiku-scoring-12.6.2/dataikuscoring/processors/derive.py
+-rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)     2080 2023-12-14 11:08:55.000000 dataiku-scoring-12.6.2/dataikuscoring/processors/derive_rescale.py
+-rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)      995 2023-12-14 11:08:55.000000 dataiku-scoring-12.6.2/dataikuscoring/processors/drop_rows.py
+-rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)     1222 2024-04-05 11:14:40.000000 dataiku-scoring-12.6.2/dataikuscoring/processors/dummify.py
+-rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)      850 2024-04-05 11:14:40.000000 dataiku-scoring-12.6.2/dataikuscoring/processors/flag.py
+-rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)     1205 2023-12-14 11:08:55.000000 dataiku-scoring-12.6.2/dataikuscoring/processors/impute.py
+-rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)     1423 2023-12-14 11:08:55.000000 dataiku-scoring-12.6.2/dataikuscoring/processors/normalize.py
+-rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)      864 2023-12-14 11:08:55.000000 dataiku-scoring-12.6.2/dataikuscoring/processors/num_cat_interaction.py
+-rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)     1023 2023-12-14 11:08:55.000000 dataiku-scoring-12.6.2/dataikuscoring/processors/num_num_interaction.py
+-rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)     5038 2023-12-14 11:08:55.000000 dataiku-scoring-12.6.2/dataikuscoring/processors/prepare_input.py
+-rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)     1493 2024-04-05 11:14:40.000000 dataiku-scoring-12.6.2/dataikuscoring/processors/preprocessings.py
+-rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)      996 2023-12-14 11:08:55.000000 dataiku-scoring-12.6.2/dataikuscoring/processors/preprocessor.py
+-rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)      928 2023-12-14 11:08:55.000000 dataiku-scoring-12.6.2/dataikuscoring/processors/rescale.py
+-rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)     1682 2024-04-05 11:14:40.000000 dataiku-scoring-12.6.2/dataikuscoring/processors/selection.py
+-rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)     2471 2023-12-14 11:08:55.000000 dataiku-scoring-12.6.2/dataikuscoring/processors/vectorize_tfidf.py
+-rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)     1246 2023-12-14 11:08:55.000000 dataiku-scoring-12.6.2/dataikuscoring/processors/vectorize_word_count.py
+-rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)      783 2023-12-14 11:08:55.000000 dataiku-scoring-12.6.2/dataikuscoring/processors/vectors_unfold.py
+drwxr-xr-x   0 kevin.remy@dataiku.com   (502) staff       (20)        0 2024-05-16 13:21:47.442901 dataiku-scoring-12.6.2/dataikuscoring/utils/
+-rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)      298 2024-05-16 13:21:19.000000 dataiku-scoring-12.6.2/dataikuscoring/utils/__init__.py
+-rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)     2323 2023-12-14 11:08:55.000000 dataiku-scoring-12.6.2/dataikuscoring/utils/indexed_matrix.py
+-rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)     2810 2024-05-16 13:21:19.000000 dataiku-scoring-12.6.2/dataikuscoring/utils/math_utils.py
+-rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)     8696 2024-04-05 11:14:40.000000 dataiku-scoring-12.6.2/dataikuscoring/utils/prediction_result.py
+-rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)     1379 2023-12-14 11:08:55.000000 dataiku-scoring-12.6.2/dataikuscoring/utils/scoring_data.py
+-rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)     1413 2023-12-14 11:08:55.000000 dataiku-scoring-12.6.2/dataikuscoring/utils/tokenizer.py
+-rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)        6 2024-01-15 09:52:42.000000 dataiku-scoring-12.6.2/requirements.txt
+-rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)       38 2024-05-16 13:21:47.456680 dataiku-scoring-12.6.2/setup.cfg
+-rw-r--r--   0 kevin.remy@dataiku.com   (502) staff       (20)      876 2024-05-16 13:21:19.000000 dataiku-scoring-12.6.2/setup.py
```

### Comparing `dataiku-scoring-12.6.0/HISTORY.txt` & `dataiku-scoring-12.6.2/HISTORY.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,17 @@
 Changelog
 ==========
 
 
 
+12.6.2 (2024-05-16)
+-------------------
+
+* Initial release for DSS 12.6.2
+
 12.6.0 (2024-04-09)
 -------------------
 
 * Initial release for DSS 12.6.0
 
 12.5.2 (2024-02-26)
 -------------------
```

### Comparing `dataiku-scoring-12.6.0/LICENSE.txt` & `dataiku-scoring-12.6.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dataiku-scoring-12.6.0/PKG-INFO` & `dataiku-scoring-12.6.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dataiku-scoring
-Version: 12.6.0
+Version: 12.6.2
 Summary: Dataiku ML Scoring Python library
 Home-page: https://www.dataiku.com
 Author: Dataiku
 Author-email: support@dataiku.com
 License: Apache Software License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -24,14 +24,19 @@
 
 
 Changelog
 ==========
 
 
 
+12.6.2 (2024-05-16)
+-------------------
+
+* Initial release for DSS 12.6.2
+
 12.6.0 (2024-04-09)
 -------------------
 
 * Initial release for DSS 12.6.0
 
 12.5.2 (2024-02-26)
 -------------------
```

### Comparing `dataiku-scoring-12.6.0/dataiku_scoring.egg-info/PKG-INFO` & `dataiku-scoring-12.6.2/dataiku_scoring.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dataiku-scoring
-Version: 12.6.0
+Version: 12.6.2
 Summary: Dataiku ML Scoring Python library
 Home-page: https://www.dataiku.com
 Author: Dataiku
 Author-email: support@dataiku.com
 License: Apache Software License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -24,14 +24,19 @@
 
 
 Changelog
 ==========
 
 
 
+12.6.2 (2024-05-16)
+-------------------
+
+* Initial release for DSS 12.6.2
+
 12.6.0 (2024-04-09)
 -------------------
 
 * Initial release for DSS 12.6.0
 
 12.5.2 (2024-02-26)
 -------------------
```

### Comparing `dataiku-scoring-12.6.0/dataiku_scoring.egg-info/SOURCES.txt` & `dataiku-scoring-12.6.2/dataiku_scoring.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dataiku-scoring-12.6.0/dataikuscoring/__init__.py` & `dataiku-scoring-12.6.2/dataikuscoring/__init__.py`

 * *Files identical despite different names*

### Comparing `dataiku-scoring-12.6.0/dataikuscoring/algorithms/__init__.py` & `dataiku-scoring-12.6.2/dataikuscoring/algorithms/__init__.py`

 * *Files identical despite different names*

### Comparing `dataiku-scoring-12.6.0/dataikuscoring/algorithms/common.py` & `dataiku-scoring-12.6.2/dataikuscoring/algorithms/common.py`

 * *Files identical despite different names*

### Comparing `dataiku-scoring-12.6.0/dataikuscoring/algorithms/decision_tree_model.py` & `dataiku-scoring-12.6.2/dataikuscoring/algorithms/decision_tree_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,20 +68,23 @@
     """
 
     def __init__(self, model_parameters):
         self.init_tree(model_parameters)
         if self.variant == "XGBOOST":
             self.feature_converter = np.float32
             self.get_terminal_node = get_terminal_node_lt
+            self.label_dtype = np.float32
         elif self.variant == "LIGHTGBM":
             self.feature_converter = np.float64
             self.get_terminal_node = get_terminal_node_lte
+            self.label_dtype = np.float64
         elif self.variant == "SKLEARN":
             self.feature_converter = lambda x: np.float64(np.float32(x))
             self.get_terminal_node = get_terminal_node_lte
+            self.label_dtype = np.float64
 
     def init_tree(self, model_parameters):
         """ Loading serialized trees
 
         We initialize one dictionary for the leaves and one for the nodes. The nodes are initialized
         without children. Then we iterate on each node and try to find a left and right child looking up at
         the child's index in the nodes map and then if not found in the leaves map (hence it stays None if
@@ -124,15 +127,15 @@
         all_nodes.update(leaves)
         self.root = all_nodes[0]
 
     def predict(self, X):
         return [self._predict(data) for data in self.feature_converter(X)]
 
     def _predict(self, data):
-        return self.get_terminal_node(self.root, data).label
+        return self.label_dtype(self.get_terminal_node(self.root, data).label)
 
     def predict_proba(self, X):
         return [self._predict_proba(data) for data in X]
 
     def _predict_proba(self, data):
         return self._predict(data)
```

### Comparing `dataiku-scoring-12.6.0/dataikuscoring/algorithms/forest_classifier.py` & `dataiku-scoring-12.6.2/dataikuscoring/algorithms/forest_classifier.py`

 * *Files identical despite different names*

### Comparing `dataiku-scoring-12.6.0/dataikuscoring/algorithms/forest_regressor.py` & `dataiku-scoring-12.6.2/dataikuscoring/algorithms/forest_regressor.py`

 * *Files identical despite different names*

### Comparing `dataiku-scoring-12.6.0/dataikuscoring/algorithms/generic_mlp.py` & `dataiku-scoring-12.6.2/dataikuscoring/algorithms/generic_mlp.py`

 * *Files identical despite different names*

### Comparing `dataiku-scoring-12.6.0/dataikuscoring/algorithms/gradient_boosting_classifier.py` & `dataiku-scoring-12.6.2/dataikuscoring/algorithms/logistic.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,38 +1,57 @@
 import numpy as np
 
 from ..utils import sigmoid, softmax
-from .decision_tree_model import DecisionTreeModel
 from .common import Classifier
 
 
-class GradientBoostingClassifier(Classifier):
-    def __init__(self, model_parameters):
-        self.trees = [[DecisionTreeModel(model_parameters) for model_parameters in trees] for trees in model_parameters["trees"]]
-        self.shrinkage = model_parameters["shrinkage"]
-        self.baseline = np.array(model_parameters["baseline"])
-        self.num_classes = 2 if len(self.trees[0]) == 1 else len(self.trees[0])
-        self.feature_converter = self.trees[0][0].feature_converter
+class LogisticRegressionClassifier(Classifier):
 
-    def decision_function(self, X):
-        return [self._decision_function(data) for data in self.feature_converter(X)]
+    def __init__(self, model_parameters):
+        self.policy = model_parameters["policy"]
+        self.intercept = np.array(model_parameters["intercept"])
+        self.coefficients = np.array(model_parameters["coefficients"])
+        self.vector_size = len(self.coefficients[0])
 
-    def _decision_function(self, data):
-        if self.num_classes == 2:
-            return [0, np.sum([tree[0]._predict(data) for tree in self.trees]) * self.shrinkage + self.baseline[0]]
-        else:
-            return np.sum([[tree._predict(data) for tree in trees] for trees in self.trees], 0) * self.shrinkage + self.baseline
+    def predict(self, X):
+        return self.predict_proba(X).argmax(axis=1)
 
     def predict_proba(self, X):
-        return [self._predict_proba(data) for data in self.feature_converter(X)]
+        dec = self.decision_function(X)
+        return POLICIES[self.policy](dec)
 
-    def _predict_proba(self, data):
-        scores = self._decision_function(data)
-        if self.num_classes == 2:
-            p = sigmoid(scores[1])
-            probas = [1 - p, p]
-        else:
-            probas = softmax(scores)
-        return probas
+    def decision_function(self, X):
+        return np.dot(X, self.coefficients.transpose()) + [self.intercept] * len(X)
 
     def __repr__(self):
-        return "GradientBoostingClassifier(n_trees={})".format(len(self.trees))
+        return """LogisticRegressionClassifier(policy={}, vector_size={})""".format(self.policy, self.vector_size)
+
+
+def one_versus_all_probabilities(dec):
+    unormalized_res = sigmoid(dec)
+    return (unormalized_res.T / unormalized_res.sum(axis=1)).T
+
+
+def multinomial_probabilities(dec):
+    return softmax(dec)
+
+
+def modified_huber_probabilities(dec):
+    p = 0.5 * (1 + np.minimum(1, np.maximum(-1, dec)))
+
+    if len(dec[0]) == 2:
+        p[:, 0] = 1 - p[:, 1]
+
+    norms = np.linalg.norm(dec, axis=1)
+
+    # scikit-learn puts equal probas in this case
+    indexes = np.where(norms < 1e-15)
+    p[indexes] = np.ones(len(dec)) * (1 / len(dec))
+
+    return p / norms
+
+
+POLICIES = {
+    "ONE_VERSUS_ALL": one_versus_all_probabilities,
+    "MULTINOMIAL": multinomial_probabilities,
+    "MODIFIED_HUBER": modified_huber_probabilities
+}
```

### Comparing `dataiku-scoring-12.6.0/dataikuscoring/algorithms/gradient_boosting_regressor.py` & `dataiku-scoring-12.6.2/dataikuscoring/algorithms/gradient_boosting_regressor.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,24 +5,31 @@
 
 
 class GradientBoostingRegressor(Regressor):
 
     def __init__(self, model_parameters):
         self.trees = [DecisionTreeModel(model_parameters)
                       for model_parameters in model_parameters["trees"]]
-        self.shrinkage = model_parameters["shrinkage"]
-        self.baseline = model_parameters["baseline"]
+        self.prediction_dtype = self.trees[0].label_dtype  # np.float32 iff model from XGBoost
+        self.shrinkage = self.prediction_dtype(model_parameters["shrinkage"])
+        self.baseline = self.prediction_dtype(model_parameters["baseline"])
         self.gamma_regression = model_parameters.get("gamma_regression", False)
         self.feature_converter = self.trees[0].feature_converter
 
     def predict(self, X):
         return [self._predict(data) for data in self.feature_converter(X)]
 
     def _predict(self, data):
         if self.gamma_regression:
-            result = np.exp(np.sum([tree._predict(data) for tree in self.trees]) * self.shrinkage) * self.baseline
+            result = np.exp(np.sum([tree._predict(data) for tree in self.trees], dtype=self.prediction_dtype) * self.shrinkage) * self.baseline
+        elif self.prediction_dtype == np.float32:
+            # Avoid np.sum to replicate XGBoost results
+            p = np.float32(0.)
+            for tree in self.trees:
+                p += tree._predict(data)
+            result = self.baseline + self.shrinkage * p
         else:
-            result = np.sum([tree._predict(data) for tree in self.trees]) * self.shrinkage + self.baseline
-        return result
+            result = self.baseline + self.shrinkage * np.sum([tree._predict(data) for tree in self.trees])
+        return float(result)
 
     def __repr__(self):
         return "GradientBoostingRegressor(n_trees={})".format(len(self.trees))
```

### Comparing `dataiku-scoring-12.6.0/dataikuscoring/algorithms/mlp_classifier.py` & `dataiku-scoring-12.6.2/dataikuscoring/algorithms/mlp_classifier.py`

 * *Files identical despite different names*

### Comparing `dataiku-scoring-12.6.0/dataikuscoring/load.py` & `dataiku-scoring-12.6.2/dataikuscoring/load.py`

 * *Files identical despite different names*

### Comparing `dataiku-scoring-12.6.0/dataikuscoring/mlflow/__init__.py` & `dataiku-scoring-12.6.2/dataikuscoring/mlflow/__init__.py`

 * *Files identical despite different names*

### Comparing `dataiku-scoring-12.6.0/dataikuscoring/mlflow/classification.py` & `dataiku-scoring-12.6.2/dataikuscoring/mlflow/classification.py`

 * *Files identical despite different names*

### Comparing `dataiku-scoring-12.6.0/dataikuscoring/mlflow/common.py` & `dataiku-scoring-12.6.2/dataikuscoring/mlflow/common.py`

 * *Files identical despite different names*

### Comparing `dataiku-scoring-12.6.0/dataikuscoring/mlflow/dss_flavor.py` & `dataiku-scoring-12.6.2/dataikuscoring/mlflow/dss_flavor.py`

 * *Files identical despite different names*

### Comparing `dataiku-scoring-12.6.0/dataikuscoring/mlflow/regression.py` & `dataiku-scoring-12.6.2/dataikuscoring/mlflow/regression.py`

 * *Files identical despite different names*

### Comparing `dataiku-scoring-12.6.0/dataikuscoring/models/__init__.py` & `dataiku-scoring-12.6.2/dataikuscoring/models/__init__.py`

 * *Files identical despite different names*

### Comparing `dataiku-scoring-12.6.0/dataikuscoring/models/binary.py` & `dataiku-scoring-12.6.2/dataikuscoring/models/binary.py`

 * *Files identical despite different names*

### Comparing `dataiku-scoring-12.6.0/dataikuscoring/models/common.py` & `dataiku-scoring-12.6.2/dataikuscoring/models/common.py`

 * *Files identical despite different names*

### Comparing `dataiku-scoring-12.6.0/dataikuscoring/models/mlflow.py` & `dataiku-scoring-12.6.2/dataikuscoring/models/mlflow.py`

 * *Files identical despite different names*

### Comparing `dataiku-scoring-12.6.0/dataikuscoring/models/model.py` & `dataiku-scoring-12.6.2/dataikuscoring/models/model.py`

 * *Files identical despite different names*

### Comparing `dataiku-scoring-12.6.0/dataikuscoring/models/partitioned.py` & `dataiku-scoring-12.6.2/dataikuscoring/models/partitioned.py`

 * *Files identical despite different names*

### Comparing `dataiku-scoring-12.6.0/dataikuscoring/processors/__init__.py` & `dataiku-scoring-12.6.2/dataikuscoring/processors/__init__.py`

 * *Files identical despite different names*

### Comparing `dataiku-scoring-12.6.0/dataikuscoring/processors/binarize.py` & `dataiku-scoring-12.6.2/dataikuscoring/processors/binarize.py`

 * *Files identical despite different names*

### Comparing `dataiku-scoring-12.6.0/dataikuscoring/processors/calibration.py` & `dataiku-scoring-12.6.2/dataikuscoring/processors/calibration.py`

 * *Files identical despite different names*

### Comparing `dataiku-scoring-12.6.0/dataikuscoring/processors/cat_cat_interaction.py` & `dataiku-scoring-12.6.2/dataikuscoring/processors/cat_cat_interaction.py`

 * *Files identical despite different names*

### Comparing `dataiku-scoring-12.6.0/dataikuscoring/processors/categorical_encode.py` & `dataiku-scoring-12.6.2/dataikuscoring/processors/categorical_encode.py`

 * *Files identical despite different names*

### Comparing `dataiku-scoring-12.6.0/dataikuscoring/processors/datetime_cyclical.py` & `dataiku-scoring-12.6.2/dataikuscoring/processors/datetime_cyclical.py`

 * *Files identical despite different names*

### Comparing `dataiku-scoring-12.6.0/dataikuscoring/processors/derive.py` & `dataiku-scoring-12.6.2/dataikuscoring/processors/derive.py`

 * *Files identical despite different names*

### Comparing `dataiku-scoring-12.6.0/dataikuscoring/processors/derive_rescale.py` & `dataiku-scoring-12.6.2/dataikuscoring/processors/derive_rescale.py`

 * *Files identical despite different names*

### Comparing `dataiku-scoring-12.6.0/dataikuscoring/processors/drop_rows.py` & `dataiku-scoring-12.6.2/dataikuscoring/processors/drop_rows.py`

 * *Files identical despite different names*

### Comparing `dataiku-scoring-12.6.0/dataikuscoring/processors/dummify.py` & `dataiku-scoring-12.6.2/dataikuscoring/processors/dummify.py`

 * *Files identical despite different names*

### Comparing `dataiku-scoring-12.6.0/dataikuscoring/processors/flag.py` & `dataiku-scoring-12.6.2/dataikuscoring/processors/flag.py`

 * *Files identical despite different names*

### Comparing `dataiku-scoring-12.6.0/dataikuscoring/processors/impute.py` & `dataiku-scoring-12.6.2/dataikuscoring/processors/impute.py`

 * *Files identical despite different names*

### Comparing `dataiku-scoring-12.6.0/dataikuscoring/processors/normalize.py` & `dataiku-scoring-12.6.2/dataikuscoring/processors/normalize.py`

 * *Files identical despite different names*

### Comparing `dataiku-scoring-12.6.0/dataikuscoring/processors/num_cat_interaction.py` & `dataiku-scoring-12.6.2/dataikuscoring/processors/num_cat_interaction.py`

 * *Files identical despite different names*

### Comparing `dataiku-scoring-12.6.0/dataikuscoring/processors/num_num_interaction.py` & `dataiku-scoring-12.6.2/dataikuscoring/processors/num_num_interaction.py`

 * *Files identical despite different names*

### Comparing `dataiku-scoring-12.6.0/dataikuscoring/processors/prepare_input.py` & `dataiku-scoring-12.6.2/dataikuscoring/processors/prepare_input.py`

 * *Files identical despite different names*

### Comparing `dataiku-scoring-12.6.0/dataikuscoring/processors/preprocessings.py` & `dataiku-scoring-12.6.2/dataikuscoring/processors/preprocessings.py`

 * *Files identical despite different names*

### Comparing `dataiku-scoring-12.6.0/dataikuscoring/processors/preprocessor.py` & `dataiku-scoring-12.6.2/dataikuscoring/processors/preprocessor.py`

 * *Files identical despite different names*

### Comparing `dataiku-scoring-12.6.0/dataikuscoring/processors/rescale.py` & `dataiku-scoring-12.6.2/dataikuscoring/processors/rescale.py`

 * *Files identical despite different names*

### Comparing `dataiku-scoring-12.6.0/dataikuscoring/processors/selection.py` & `dataiku-scoring-12.6.2/dataikuscoring/processors/selection.py`

 * *Files identical despite different names*

### Comparing `dataiku-scoring-12.6.0/dataikuscoring/processors/vectorize_tfidf.py` & `dataiku-scoring-12.6.2/dataikuscoring/processors/vectorize_tfidf.py`

 * *Files identical despite different names*

### Comparing `dataiku-scoring-12.6.0/dataikuscoring/processors/vectorize_word_count.py` & `dataiku-scoring-12.6.2/dataikuscoring/processors/vectorize_word_count.py`

 * *Files identical despite different names*

### Comparing `dataiku-scoring-12.6.0/dataikuscoring/processors/vectors_unfold.py` & `dataiku-scoring-12.6.2/dataikuscoring/processors/vectors_unfold.py`

 * *Files identical despite different names*

### Comparing `dataiku-scoring-12.6.0/dataikuscoring/utils/indexed_matrix.py` & `dataiku-scoring-12.6.2/dataikuscoring/utils/indexed_matrix.py`

 * *Files identical despite different names*

### Comparing `dataiku-scoring-12.6.0/dataikuscoring/utils/prediction_result.py` & `dataiku-scoring-12.6.2/dataikuscoring/utils/prediction_result.py`

 * *Files identical despite different names*

### Comparing `dataiku-scoring-12.6.0/dataikuscoring/utils/scoring_data.py` & `dataiku-scoring-12.6.2/dataikuscoring/utils/scoring_data.py`

 * *Files identical despite different names*

### Comparing `dataiku-scoring-12.6.0/dataikuscoring/utils/tokenizer.py` & `dataiku-scoring-12.6.2/dataikuscoring/utils/tokenizer.py`

 * *Files identical despite different names*

### Comparing `dataiku-scoring-12.6.0/setup.py` & `dataiku-scoring-12.6.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 
 import setuptools
 
 long_description = (open('README.md').read() + '\n\n' +
                     open('HISTORY.txt').read())
 
-VERSION = "12.6.0"
+VERSION = "12.6.2"
 
 setuptools.setup(
     name='dataiku-scoring',
     version=VERSION,
     license="Apache Software License",
     packages=setuptools.find_packages(),
     description="Dataiku ML Scoring Python library",
```

