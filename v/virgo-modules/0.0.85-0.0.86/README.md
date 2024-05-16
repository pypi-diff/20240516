# Comparing `tmp/virgo_modules-0.0.85.tar.gz` & `tmp/virgo_modules-0.0.86.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "virgo_modules-0.0.85.tar", last modified: Mon May 13 19:18:57 2024, max compression
+gzip compressed data, was "virgo_modules-0.0.86.tar", last modified: Thu May 16 12:04:14 2024, max compression
```

## Comparing `virgo_modules-0.0.85.tar` & `virgo_modules-0.0.86.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-05-13 19:18:57.881178 virgo_modules-0.0.85/
--rw-rw-rw-   0        0        0     1097 2024-01-28 08:59:04.000000 virgo_modules-0.0.85/LICENSE
--rw-rw-rw-   0        0        0     1411 2024-05-13 19:18:57.878178 virgo_modules-0.0.85/PKG-INFO
--rw-rw-rw-   0        0        0      354 2024-01-28 09:03:10.000000 virgo_modules-0.0.85/README.md
--rw-rw-rw-   0        0        0       42 2024-05-13 19:18:57.883186 virgo_modules-0.0.85/setup.cfg
--rw-rw-rw-   0        0        0     1230 2024-05-13 19:18:08.000000 virgo_modules-0.0.85/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-13 19:18:57.795129 virgo_modules-0.0.85/virgo_app/
-drwxrwxrwx   0        0        0        0 2024-05-13 19:18:57.822816 virgo_modules-0.0.85/virgo_app/virgo_modules/
--rw-rw-rw-   0        0        0        0 2024-01-25 18:20:42.000000 virgo_modules-0.0.85/virgo_app/virgo_modules/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-13 19:18:57.871010 virgo_modules-0.0.85/virgo_app/virgo_modules/src/
--rw-rw-rw-   0        0        0        0 2024-01-25 17:59:03.000000 virgo_modules-0.0.85/virgo_app/virgo_modules/src/__init__.py
--rw-rw-rw-   0        0        0     2571 2024-04-05 07:01:35.000000 virgo_modules-0.0.85/virgo_app/virgo_modules/src/aws_utils.py
--rw-rw-rw-   0        0        0    13268 2024-04-05 06:56:27.000000 virgo_modules-0.0.85/virgo_app/virgo_modules/src/edge_utils.py
--rw-rw-rw-   0        0        0     1989 2023-12-10 12:51:06.000000 virgo_modules-0.0.85/virgo_app/virgo_modules/src/pull_artifacts.py
--rw-rw-rw-   0        0        0    71603 2024-05-13 19:18:08.000000 virgo_modules-0.0.85/virgo_app/virgo_modules/src/re_utils.py
--rw-rw-rw-   0        0        0   143298 2024-05-02 07:44:54.000000 virgo_modules-0.0.85/virgo_app/virgo_modules/src/ticketer_source.py
-drwxrwxrwx   0        0        0        0 2024-05-13 19:18:57.840006 virgo_modules-0.0.85/virgo_app/virgo_modules.egg-info/
--rw-rw-rw-   0        0        0     1411 2024-05-13 19:18:57.000000 virgo_modules-0.0.85/virgo_app/virgo_modules.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      552 2024-05-13 19:18:57.000000 virgo_modules-0.0.85/virgo_app/virgo_modules.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-13 19:18:57.000000 virgo_modules-0.0.85/virgo_app/virgo_modules.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      276 2024-05-13 19:18:57.000000 virgo_modules-0.0.85/virgo_app/virgo_modules.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-05-13 19:18:57.000000 virgo_modules-0.0.85/virgo_app/virgo_modules.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-16 12:04:14.888759 virgo_modules-0.0.86/
+-rw-rw-rw-   0        0        0     1097 2024-01-28 08:59:04.000000 virgo_modules-0.0.86/LICENSE
+-rw-rw-rw-   0        0        0     1411 2024-05-16 12:04:14.886786 virgo_modules-0.0.86/PKG-INFO
+-rw-rw-rw-   0        0        0      354 2024-01-28 09:03:10.000000 virgo_modules-0.0.86/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-16 12:04:14.889760 virgo_modules-0.0.86/setup.cfg
+-rw-rw-rw-   0        0        0     1230 2024-05-16 10:57:12.000000 virgo_modules-0.0.86/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-16 12:04:14.743499 virgo_modules-0.0.86/virgo_app/
+drwxrwxrwx   0        0        0        0 2024-05-16 12:04:14.796500 virgo_modules-0.0.86/virgo_app/virgo_modules/
+-rw-rw-rw-   0        0        0        0 2024-01-25 18:20:42.000000 virgo_modules-0.0.86/virgo_app/virgo_modules/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-16 12:04:14.878683 virgo_modules-0.0.86/virgo_app/virgo_modules/src/
+-rw-rw-rw-   0        0        0        0 2024-01-25 17:59:03.000000 virgo_modules-0.0.86/virgo_app/virgo_modules/src/__init__.py
+-rw-rw-rw-   0        0        0     2571 2024-04-05 07:01:35.000000 virgo_modules-0.0.86/virgo_app/virgo_modules/src/aws_utils.py
+-rw-rw-rw-   0        0        0    13732 2024-05-16 12:03:48.000000 virgo_modules-0.0.86/virgo_app/virgo_modules/src/edge_utils.py
+-rw-rw-rw-   0        0        0     1989 2023-12-10 12:51:06.000000 virgo_modules-0.0.86/virgo_app/virgo_modules/src/pull_artifacts.py
+-rw-rw-rw-   0        0        0    71603 2024-05-13 19:18:08.000000 virgo_modules-0.0.86/virgo_app/virgo_modules/src/re_utils.py
+-rw-rw-rw-   0        0        0   143298 2024-05-02 07:44:54.000000 virgo_modules-0.0.86/virgo_app/virgo_modules/src/ticketer_source.py
+drwxrwxrwx   0        0        0        0 2024-05-16 12:04:14.825497 virgo_modules-0.0.86/virgo_app/virgo_modules.egg-info/
+-rw-rw-rw-   0        0        0     1411 2024-05-16 12:04:13.000000 virgo_modules-0.0.86/virgo_app/virgo_modules.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      552 2024-05-16 12:04:14.000000 virgo_modules-0.0.86/virgo_app/virgo_modules.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-16 12:04:13.000000 virgo_modules-0.0.86/virgo_app/virgo_modules.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      276 2024-05-16 12:04:13.000000 virgo_modules-0.0.86/virgo_app/virgo_modules.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-05-16 12:04:13.000000 virgo_modules-0.0.86/virgo_app/virgo_modules.egg-info/top_level.txt
```

### Comparing `virgo_modules-0.0.85/LICENSE` & `virgo_modules-0.0.86/LICENSE`

 * *Files identical despite different names*

### Comparing `virgo_modules-0.0.85/PKG-INFO` & `virgo_modules-0.0.86/virgo_app/virgo_modules.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: virgo_modules
-Version: 0.0.85
+Name: virgo-modules
+Version: 0.0.86
 Summary: data processing and statistical modeling using stock market data
 Home-page: https://github.com/miguelmayhem92/virgo_module
 Author: Miguel Mayhuire
 Author-email: miguelmayhem92@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `virgo_modules-0.0.85/setup.py` & `virgo_modules-0.0.86/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open("virgo_app/README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="virgo_modules",
-    version="0.0.85",
+    version="0.0.86",
     description="data processing and statistical modeling using stock market data",
     package_dir={"": "virgo_app"},
     packages=find_packages(where="virgo_app"),
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/miguelmayhem92/virgo_module",
     author="Miguel Mayhuire",
```

### Comparing `virgo_modules-0.0.85/virgo_app/virgo_modules/src/aws_utils.py` & `virgo_modules-0.0.86/virgo_app/virgo_modules/src/aws_utils.py`

 * *Files identical despite different names*

### Comparing `virgo_modules-0.0.85/virgo_app/virgo_modules/src/edge_utils.py` & `virgo_modules-0.0.86/virgo_app/virgo_modules/src/edge_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from sklearn.metrics import roc_auc_score, precision_score, recall_score
 from sklearn.pipeline import Pipeline
 
 from feature_engine.selection import DropFeatures, DropCorrelatedFeatures
 from feature_engine.imputation import  MeanMedianImputer
 from virgo_modules.src.ticketer_source import FeatureSelector
 from feature_engine.discretisation import EqualWidthDiscretiser
+from feature_engine.datetime import DatetimeFeatures
 
 from .ticketer_source import VirgoWinsorizerFeature, InverseHyperbolicSine
 
 class produce_model_wrapper:
     """
     class that wraps a pipeline and a machine learning model. it also provides data spliting train/validation
 
@@ -211,48 +212,53 @@
     print(recall_score(y,preds, average=None))
 
 
 def data_processing_pipeline_classifier(
         features_base,features_to_drop = False, winsorizer_conf = False, discretize_columns = False,
         bins_discretize = 10, correlation = 0.85, fillna = True,
         invhypervolsin_features = False,
-        pipeline_order = 'selector//winzorizer//discretizer//median_inputer//drop//correlation'):
+        date_features_list = False,
+        pipeline_order = 'selector//winzorizer//discretizer//median_inputer//drop//correlation'
+        ):
 
     '''
     pipeline builder
 
             Parameters:
                     features_base (list): model pipeline
                     features_to_drop (list): features to drop list
                     winsorizer_conf (dict): winsorising configuration dictionary
                     discretize_columns (list): feature list to discretize
                     bins_discretize (int): number of bins to discretize
                     correlation (float): correlation threshold to discard correlated features
                     fillna (boolean): if true to fill na features
                     invhypervolsin_features (list): list of features to apply inverse hyperbolic sine
+                    date_features_list (list): list of features to compute from Date field. (list of features from feature_engine)
                     pipeline_order (str): custom pipeline order eg. selector//winzorizer//discretizer//median_inputer//drop//correlation
             Returns:
                     pipe (obj): pipeline object
     '''
     select_pipe = [('selector', FeatureSelector(features_base))] if features_base else []
     winzorizer_pipe = [('winzorized_features', VirgoWinsorizerFeature(winsorizer_conf))] if winsorizer_conf else []
     drop_pipe = [('drop_features' , DropFeatures(features_to_drop=features_to_drop))] if features_to_drop else []
     discretize = [('discretize',EqualWidthDiscretiser(discretize_columns, bins = bins_discretize ))] if discretize_columns else []
     drop_corr = [('drop_corr', DropCorrelatedFeatures(threshold=correlation, method = 'spearman'))] if correlation else []
     median_imputer_pipe = [('median_imputer', MeanMedianImputer())] if fillna else []
     invhypersin_pipe = [('invhypervolsin scaler', InverseHyperbolicSine(features = invhypervolsin_features))] if invhypervolsin_features else []
+    datetimeFeatures_pipe = [('date features', DatetimeFeatures(features_to_extract = date_features_list, variables = 'Date', drop_original = False))] if date_features_list else []
 
     pipe_dictionary = {
         'selector': select_pipe,
         'winzorizer':winzorizer_pipe,
         'drop':drop_pipe,
         'discretizer': discretize,
         'correlation': drop_corr,
         'median_inputer':median_imputer_pipe,
         'arcsinh_scaler': invhypersin_pipe,
+        'date_features': datetimeFeatures_pipe,
     }
 
     pipeline_steps = pipeline_order.split('//')
     ## validation
     for step in pipeline_steps:
         if step not in pipe_dictionary.keys():
             raise Exception(f'{step} step not in list of steps, the list is: {list(pipe_dictionary.keys())}')
```

### Comparing `virgo_modules-0.0.85/virgo_app/virgo_modules/src/pull_artifacts.py` & `virgo_modules-0.0.86/virgo_app/virgo_modules/src/pull_artifacts.py`

 * *Files identical despite different names*

### Comparing `virgo_modules-0.0.85/virgo_app/virgo_modules/src/re_utils.py` & `virgo_modules-0.0.86/virgo_app/virgo_modules/src/re_utils.py`

 * *Files identical despite different names*

### Comparing `virgo_modules-0.0.85/virgo_app/virgo_modules/src/ticketer_source.py` & `virgo_modules-0.0.86/virgo_app/virgo_modules/src/ticketer_source.py`

 * *Files identical despite different names*

### Comparing `virgo_modules-0.0.85/virgo_app/virgo_modules.egg-info/PKG-INFO` & `virgo_modules-0.0.86/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: virgo-modules
-Version: 0.0.85
+Name: virgo_modules
+Version: 0.0.86
 Summary: data processing and statistical modeling using stock market data
 Home-page: https://github.com/miguelmayhem92/virgo_module
 Author: Miguel Mayhuire
 Author-email: miguelmayhem92@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `virgo_modules-0.0.85/virgo_app/virgo_modules.egg-info/SOURCES.txt` & `virgo_modules-0.0.86/virgo_app/virgo_modules.egg-info/SOURCES.txt`

 * *Files identical despite different names*

