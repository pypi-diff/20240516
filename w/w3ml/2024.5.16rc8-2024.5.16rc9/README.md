# Comparing `tmp/w3ml-2024.5.16rc8.tar.gz` & `tmp/w3ml-2024.5.16rc9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/w3ml-2024.5.16rc8.tar", last modified: Thu May 16 05:11:36 2024, max compression
+gzip compressed data, was "dist/w3ml-2024.5.16rc9.tar", last modified: Thu May 16 05:27:01 2024, max compression
```

## Comparing `w3ml-2024.5.16rc8.tar` & `w3ml-2024.5.16rc9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 05:11:36.000000 w3ml-2024.5.16rc8/
--rw-r--r--   0 runner    (1001) docker     (127)      481 2024-05-16 05:11:36.000000 w3ml-2024.5.16rc8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-05-16 05:11:28.000000 w3ml-2024.5.16rc8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 05:11:36.000000 w3ml-2024.5.16rc8/w3ml/
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-16 05:11:28.000000 w3ml-2024.5.16rc8/w3ml/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 05:11:36.000000 w3ml-2024.5.16rc8/w3ml/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-16 05:11:28.000000 w3ml-2024.5.16rc8/w3ml/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 05:11:36.000000 w3ml-2024.5.16rc8/w3ml/models/
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-16 05:11:28.000000 w3ml-2024.5.16rc8/w3ml/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 05:11:36.000000 w3ml-2024.5.16rc8/w3ml/models/contrib/
--rw-r--r--   0 runner    (1001) docker     (127)      255 2024-05-16 05:11:28.000000 w3ml-2024.5.16rc8/w3ml/models/contrib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6220 2024-05-16 05:11:28.000000 w3ml-2024.5.16rc8/w3ml/models/contrib/automl_multilabel.py
--rw-r--r--   0 runner    (1001) docker     (127)    10696 2024-05-16 05:11:28.000000 w3ml-2024.5.16rc8/w3ml/models/contrib/automl_binary.py
--rw-r--r--   0 runner    (1001) docker     (127)     9527 2024-05-16 05:11:28.000000 w3ml-2024.5.16rc8/w3ml/models/contrib/automl_multiclass.py
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-16 05:11:28.000000 w3ml-2024.5.16rc8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 05:11:36.000000 w3ml-2024.5.16rc8/w3ml.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      481 2024-05-16 05:11:36.000000 w3ml-2024.5.16rc8/w3ml.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-16 05:11:36.000000 w3ml-2024.5.16rc8/w3ml.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-16 05:11:36.000000 w3ml-2024.5.16rc8/w3ml.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)      380 2024-05-16 05:11:36.000000 w3ml-2024.5.16rc8/w3ml.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 05:11:36.000000 w3ml-2024.5.16rc8/w3ml.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 05:11:36.000000 w3ml-2024.5.16rc8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-05-16 05:11:28.000000 w3ml-2024.5.16rc8/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 05:27:01.000000 w3ml-2024.5.16rc9/
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-05-16 05:27:01.000000 w3ml-2024.5.16rc9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-05-16 05:26:52.000000 w3ml-2024.5.16rc9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 05:27:01.000000 w3ml-2024.5.16rc9/w3ml/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-16 05:26:52.000000 w3ml-2024.5.16rc9/w3ml/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 05:27:01.000000 w3ml-2024.5.16rc9/w3ml/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-16 05:26:52.000000 w3ml-2024.5.16rc9/w3ml/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 05:27:01.000000 w3ml-2024.5.16rc9/w3ml/models/
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-16 05:26:52.000000 w3ml-2024.5.16rc9/w3ml/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 05:27:01.000000 w3ml-2024.5.16rc9/w3ml/models/contrib/
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2024-05-16 05:26:52.000000 w3ml-2024.5.16rc9/w3ml/models/contrib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6220 2024-05-16 05:26:52.000000 w3ml-2024.5.16rc9/w3ml/models/contrib/automl_multilabel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10681 2024-05-16 05:26:52.000000 w3ml-2024.5.16rc9/w3ml/models/contrib/automl_binary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9527 2024-05-16 05:26:52.000000 w3ml-2024.5.16rc9/w3ml/models/contrib/automl_multiclass.py
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-16 05:26:52.000000 w3ml-2024.5.16rc9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 05:27:01.000000 w3ml-2024.5.16rc9/w3ml.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-05-16 05:27:01.000000 w3ml-2024.5.16rc9/w3ml.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-16 05:27:01.000000 w3ml-2024.5.16rc9/w3ml.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-16 05:27:01.000000 w3ml-2024.5.16rc9/w3ml.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-05-16 05:27:01.000000 w3ml-2024.5.16rc9/w3ml.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 05:27:01.000000 w3ml-2024.5.16rc9/w3ml.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 05:27:01.000000 w3ml-2024.5.16rc9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-05-16 05:26:52.000000 w3ml-2024.5.16rc9/LICENSE
```

### Comparing `w3ml-2024.5.16rc8/setup.py` & `w3ml-2024.5.16rc9/setup.py`

 * *Files identical despite different names*

### Comparing `w3ml-2024.5.16rc8/w3ml/models/contrib/automl_multilabel.py` & `w3ml-2024.5.16rc9/w3ml/models/contrib/automl_multilabel.py`

 * *Files identical despite different names*

### Comparing `w3ml-2024.5.16rc8/w3ml/models/contrib/automl_binary.py` & `w3ml-2024.5.16rc9/w3ml/models/contrib/automl_binary.py`

 * *Files 1% similar despite different names*

```diff
@@ -114,15 +114,15 @@
         except Exception as e:
             os.rmdir(self.path)
             raise Exception(f"Error occured : {e}")
             
     def _fit(self):
         columns = [
             f for f in self.train_data.columns if f not in self.non_training_features
-        ] + [self.label]
+        ]
         predictor = TabularPredictor(
             label=self.label,
             eval_metric=self.eval_metric,
             path=self.path,
             sample_weight="balance_weight",
             verbosity=0,
         )
```

### Comparing `w3ml-2024.5.16rc8/w3ml/models/contrib/automl_multiclass.py` & `w3ml-2024.5.16rc9/w3ml/models/contrib/automl_multiclass.py`

 * *Files identical despite different names*

### Comparing `w3ml-2024.5.16rc8/LICENSE` & `w3ml-2024.5.16rc9/LICENSE`

 * *Files identical despite different names*

