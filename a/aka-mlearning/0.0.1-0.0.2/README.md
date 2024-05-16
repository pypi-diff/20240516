# Comparing `tmp/aka_mlearning-0.0.1.tar.gz` & `tmp/aka_mlearning-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aka_mlearning-0.0.1.tar", last modified: Sun May 12 12:08:30 2024, max compression
+gzip compressed data, was "aka_mlearning-0.0.2.tar", last modified: Thu May 16 15:50:56 2024, max compression
```

## Comparing `aka_mlearning-0.0.1.tar` & `aka_mlearning-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-12 12:08:32.000000 aka_mlearning-0.0.1/
--rw-rw-rw-   0        0        0      179 2024-05-12 12:08:32.000000 aka_mlearning-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-05-12 11:48:58.000000 aka_mlearning-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-12 12:08:32.000000 aka_mlearning-0.0.1/aka_MLearning/
--rw-rw-rw-   0        0        0       78 2024-05-12 11:27:34.000000 aka_mlearning-0.0.1/aka_MLearning/__init__.py
--rw-rw-rw-   0        0        0    16384 2024-05-12 10:37:30.000000 aka_mlearning-0.0.1/aka_MLearning/aka_ML_finder.py
-drwxrwxrwx   0        0        0        0 2024-05-12 12:08:32.000000 aka_mlearning-0.0.1/aka_mlearning.egg-info/
--rw-rw-rw-   0        0        0      179 2024-05-12 12:08:32.000000 aka_mlearning-0.0.1/aka_mlearning.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      259 2024-05-12 12:08:32.000000 aka_mlearning-0.0.1/aka_mlearning.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-12 12:08:32.000000 aka_mlearning-0.0.1/aka_mlearning.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       42 2024-05-12 12:08:32.000000 aka_mlearning-0.0.1/aka_mlearning.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-05-12 12:08:32.000000 aka_mlearning-0.0.1/aka_mlearning.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-12 12:08:32.000000 aka_mlearning-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      452 2024-05-12 12:03:38.000000 aka_mlearning-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-16 15:50:56.000000 aka_mlearning-0.0.2/
+-rw-rw-rw-   0        0        0      179 2024-05-16 15:50:58.000000 aka_mlearning-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-05-12 11:48:58.000000 aka_mlearning-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-16 15:50:58.000000 aka_mlearning-0.0.2/aka_MLearning/
+-rw-rw-rw-   0        0        0       78 2024-05-12 11:27:34.000000 aka_mlearning-0.0.2/aka_MLearning/__init__.py
+-rw-rw-rw-   0        0        0    17021 2024-05-16 15:48:08.000000 aka_mlearning-0.0.2/aka_MLearning/aka_ML_finder.py
+drwxrwxrwx   0        0        0        0 2024-05-16 15:50:58.000000 aka_mlearning-0.0.2/aka_mlearning.egg-info/
+-rw-rw-rw-   0        0        0      179 2024-05-16 15:50:56.000000 aka_mlearning-0.0.2/aka_mlearning.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      259 2024-05-16 15:50:56.000000 aka_mlearning-0.0.2/aka_mlearning.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-16 15:50:56.000000 aka_mlearning-0.0.2/aka_mlearning.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       42 2024-05-16 15:50:56.000000 aka_mlearning-0.0.2/aka_mlearning.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-05-16 15:50:56.000000 aka_mlearning-0.0.2/aka_mlearning.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-16 15:50:58.000000 aka_mlearning-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      452 2024-05-16 15:50:32.000000 aka_mlearning-0.0.2/setup.py
```

### Comparing `aka_mlearning-0.0.1/aka_MLearning/aka_ML_finder.py` & `aka_mlearning-0.0.2/aka_MLearning/aka_ML_finder.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import pandas as pd
 import numpy as np
 import plotly.graph_objects as go
 import plotly.figure_factory as ff
+import plotly.express as px
 
 from scipy import stats
 
 
 
 
 class aka_ML_analysis:
@@ -183,28 +184,23 @@
     # Remove empty lines
     report_lines = [line for line in report_lines if line.strip()]
     data = [line.split() for line in report_lines[1:]]
     colss = ['feature', 'precision',   'recall',  'f1-score',   'support', 'n1one']
 
     # Convert to a DataFrame
     report_df = pd.DataFrame(data, columns = colss )
-    report_df = report_df[report_df.columns[:-1]]
-    # cm = report_df.iloc[:-3,1:].apply(pd.to_numeric).values
+    report_df = report_df[report_df.columns[:-1]] 
     cm = report_df.iloc[:,1:].apply(pd.to_numeric, errors='coerce').fillna(0).values
     colss1 = [  'precision',   'recall',  'f1-score',   'support']
 
     if lab == 1:
         fig = ff.create_annotated_heatmap(cm,
                                             x = colss1,
                                             y = cmLabel[:cm.shape[0]],
-                                            colorscale='Viridis' )
-        # fig.update_yaxes(
-        #         title_text = 'y', 
-        #         showticklabels=False   
-        #         )
+                                            colorscale='Viridis' ) 
     else:
         cmm =  cm[:,:-1]
         annotation_text = [['' for _ in range(cmm.shape[1])] for _ in range(cmm.shape[0])]
         fig = ff.create_annotated_heatmap(cmm,
                                             x = colss1[:-1],
                                             colorscale='Viridis',
                                             showscale=True,
@@ -248,14 +244,36 @@
     fig.update_layout(**self.update_layout_parameter) 
     fig.update_xaxes(**self.update_axes)
     fig.update_yaxes(**self.update_axes) 
 
     return fig
 
 
+  def plot_important_features(self, model,df,max_num_feat=10):
+    import_features = model.feature_importances_
+    cols = df.columns[:-1]
+    max_num_feat = min(len(cols),max_num_feat)
+
+    importance_cols = zip(import_features, cols)
+    
+    sorted_importance_cols = sorted(importance_cols, key=lambda x: abs(x[0]), reverse=True)
+
+    sorted_import_features, sorted_cols = zip(*sorted_importance_cols)
+
+    data = pd.DataFrame({'Weight': sorted_import_features[:max_num_feat], 'Feature Name': sorted_cols[:max_num_feat]})
+
+    fig = px.bar(data, x='Weight', y='Feature Name', orientation='h', title=f'Top {max_num_feat} Importance Features by Weight')
+
+
+    fig.update_layout(**self.update_layout_parameter) 
+    fig.update_xaxes(**self.update_axes)
+    return fig
+
+
+
 
 from sklearn.metrics import mean_absolute_error, mean_squared_error, mean_squared_log_error, median_absolute_error, mean_absolute_percentage_error, max_error, r2_score
 from sklearn.linear_model import LinearRegression, SGDRegressor, Ridge
 from sklearn.ensemble import RandomForestRegressor, AdaBoostRegressor, GradientBoostingRegressor, BaggingRegressor, ExtraTreesRegressor, HistGradientBoostingRegressor
 from sklearn.tree import DecisionTreeRegressor
 from xgboost import XGBRegressor
 from catboost import CatBoostRegressor
@@ -375,26 +393,26 @@
         self.metrics = {
             'Accuracy': accuracy_score,
             'Precision': precision_score,
             'Recall': recall_score,
             'F1 Score': f1_score
         }
 
-    def train_and_find_best_classifier(self, X_train, y_train, X_test, y_test):
+    def train_and_find_best_classifier(self, X_train, y_train, X_test, y_test, cv=3):
         parameters = {
             # 'learning_rate': [0.1, 0.01, 0.05],
             # 'max_depth': [3, 5, 7],
             # 'n_estimators': [70, 100, 200,500]
         }  
         best_algorithms = {}
         metric_algorithms = {}
         clf_algorithms = {}
 
         for classifier_name, clf in self.classifiers.items():
-            clf = GridSearchCV(estimator=clf, param_grid=parameters, refit="recall", cv=3) 
+            clf = GridSearchCV(estimator=clf, param_grid=parameters, refit="recall", cv=cv) 
             clf.fit(X_train, y_train)
             clf_algorithms[classifier_name] = clf
 
         for metric_name, metric_func in self.metrics.items():
             best_error = 0
             best_classifier = None
```

