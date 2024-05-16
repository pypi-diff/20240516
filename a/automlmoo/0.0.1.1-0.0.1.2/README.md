# Comparing `tmp/automlmoo-0.0.1.1.tar.gz` & `tmp/automlmoo-0.0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "automlmoo-0.0.1.1.tar", last modified: Wed May 15 22:31:39 2024, max compression
+gzip compressed data, was "automlmoo-0.0.1.2.tar", last modified: Thu May 16 21:41:59 2024, max compression
```

## Comparing `automlmoo-0.0.1.1.tar` & `automlmoo-0.0.1.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 gamhe     (1000) gamhe     (1000)        0 2024-05-15 22:31:39.933943 automlmoo-0.0.1.1/
--rw-r--r--   0 gamhe     (1000) gamhe     (1000)     1070 2024-05-12 18:00:18.000000 automlmoo-0.0.1.1/LICENSE.txt
--rw-r--r--   0 gamhe     (1000) gamhe     (1000)      616 2024-05-15 22:31:39.933943 automlmoo-0.0.1.1/PKG-INFO
--rw-r--r--   0 gamhe     (1000) gamhe     (1000)      312 2024-05-15 22:12:22.000000 automlmoo-0.0.1.1/README.md
-drwxr-xr-x   0 gamhe     (1000) gamhe     (1000)        0 2024-05-15 22:31:39.933943 automlmoo-0.0.1.1/automlmoo/
--rw-r--r--   0 gamhe     (1000) gamhe     (1000)       41 2024-05-12 18:01:34.000000 automlmoo-0.0.1.1/automlmoo/__init__.py
--rw-r--r--   0 gamhe     (1000) gamhe     (1000)     1256 2024-05-12 21:16:23.000000 automlmoo-0.0.1.1/automlmoo/autosklearn_modeling.py
--rw-r--r--   0 gamhe     (1000) gamhe     (1000)     2671 2024-05-13 10:50:54.000000 automlmoo-0.0.1.1/automlmoo/pymoo_optimization.py
--rw-r--r--   0 gamhe     (1000) gamhe     (1000)     4538 2024-05-13 13:15:20.000000 automlmoo-0.0.1.1/automlmoo/solver.py
--rw-r--r--   0 gamhe     (1000) gamhe     (1000)       21 2024-05-12 18:02:07.000000 automlmoo-0.0.1.1/automlmoo/version.py
-drwxr-xr-x   0 gamhe     (1000) gamhe     (1000)        0 2024-05-15 22:31:39.933943 automlmoo-0.0.1.1/automlmoo.egg-info/
--rw-r--r--   0 gamhe     (1000) gamhe     (1000)      616 2024-05-15 22:31:39.000000 automlmoo-0.0.1.1/automlmoo.egg-info/PKG-INFO
--rw-r--r--   0 gamhe     (1000) gamhe     (1000)      323 2024-05-15 22:31:39.000000 automlmoo-0.0.1.1/automlmoo.egg-info/SOURCES.txt
--rw-r--r--   0 gamhe     (1000) gamhe     (1000)        1 2024-05-15 22:31:39.000000 automlmoo-0.0.1.1/automlmoo.egg-info/dependency_links.txt
--rw-r--r--   0 gamhe     (1000) gamhe     (1000)       53 2024-05-15 22:31:39.000000 automlmoo-0.0.1.1/automlmoo.egg-info/requires.txt
--rw-r--r--   0 gamhe     (1000) gamhe     (1000)       10 2024-05-15 22:31:39.000000 automlmoo-0.0.1.1/automlmoo.egg-info/top_level.txt
--rw-r--r--   0 gamhe     (1000) gamhe     (1000)       38 2024-05-15 22:31:39.933943 automlmoo-0.0.1.1/setup.cfg
--rw-r--r--   0 gamhe     (1000) gamhe     (1000)      654 2024-05-15 22:30:15.000000 automlmoo-0.0.1.1/setup.py
+drwxr-xr-x   0 gamhe     (1000) gamhe     (1000)        0 2024-05-16 21:41:59.238301 automlmoo-0.0.1.2/
+-rw-r--r--   0 gamhe     (1000) gamhe     (1000)     1070 2024-05-12 18:00:18.000000 automlmoo-0.0.1.2/LICENSE.txt
+-rw-r--r--   0 gamhe     (1000) gamhe     (1000)      616 2024-05-16 21:41:59.238301 automlmoo-0.0.1.2/PKG-INFO
+-rw-r--r--   0 gamhe     (1000) gamhe     (1000)      312 2024-05-15 22:12:22.000000 automlmoo-0.0.1.2/README.md
+drwxr-xr-x   0 gamhe     (1000) gamhe     (1000)        0 2024-05-16 21:41:59.238301 automlmoo-0.0.1.2/automlmoo/
+-rw-r--r--   0 gamhe     (1000) gamhe     (1000)       41 2024-05-12 18:01:34.000000 automlmoo-0.0.1.2/automlmoo/__init__.py
+-rw-r--r--   0 gamhe     (1000) gamhe     (1000)     1308 2024-05-16 21:10:36.000000 automlmoo-0.0.1.2/automlmoo/autosklearn_modeling.py
+-rw-r--r--   0 gamhe     (1000) gamhe     (1000)     2671 2024-05-13 10:50:54.000000 automlmoo-0.0.1.2/automlmoo/pymoo_optimization.py
+-rw-r--r--   0 gamhe     (1000) gamhe     (1000)     4642 2024-05-16 21:12:14.000000 automlmoo-0.0.1.2/automlmoo/solver.py
+-rw-r--r--   0 gamhe     (1000) gamhe     (1000)       23 2024-05-16 20:40:04.000000 automlmoo-0.0.1.2/automlmoo/version.py
+drwxr-xr-x   0 gamhe     (1000) gamhe     (1000)        0 2024-05-16 21:41:59.238301 automlmoo-0.0.1.2/automlmoo.egg-info/
+-rw-r--r--   0 gamhe     (1000) gamhe     (1000)      616 2024-05-16 21:41:59.000000 automlmoo-0.0.1.2/automlmoo.egg-info/PKG-INFO
+-rw-r--r--   0 gamhe     (1000) gamhe     (1000)      323 2024-05-16 21:41:59.000000 automlmoo-0.0.1.2/automlmoo.egg-info/SOURCES.txt
+-rw-r--r--   0 gamhe     (1000) gamhe     (1000)        1 2024-05-16 21:41:59.000000 automlmoo-0.0.1.2/automlmoo.egg-info/dependency_links.txt
+-rw-r--r--   0 gamhe     (1000) gamhe     (1000)       53 2024-05-16 21:41:59.000000 automlmoo-0.0.1.2/automlmoo.egg-info/requires.txt
+-rw-r--r--   0 gamhe     (1000) gamhe     (1000)       10 2024-05-16 21:41:59.000000 automlmoo-0.0.1.2/automlmoo.egg-info/top_level.txt
+-rw-r--r--   0 gamhe     (1000) gamhe     (1000)       38 2024-05-16 21:41:59.238301 automlmoo-0.0.1.2/setup.cfg
+-rw-r--r--   0 gamhe     (1000) gamhe     (1000)      654 2024-05-16 20:40:22.000000 automlmoo-0.0.1.2/setup.py
```

### Comparing `automlmoo-0.0.1.1/LICENSE.txt` & `automlmoo-0.0.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `automlmoo-0.0.1.1/PKG-INFO` & `automlmoo-0.0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: automlmoo
-Version: 0.0.1.1
+Version: 0.0.1.2
 Summary: A package for automatic modeling and optimize systems based on data
 Home-page: UNKNOWN
 Author: Yarens J. Cruz
 License: MIT
 Platform: UNKNOWN
 Requires-Python: >=3.7, <3.10
 Description-Content-Type: text/markdown
```

### Comparing `automlmoo-0.0.1.1/automlmoo/autosklearn_modeling.py` & `automlmoo-0.0.1.2/automlmoo/autosklearn_modeling.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,25 +2,25 @@
 import time
 import six.moves.cPickle as pickle
 import numpy as np
 from sklearn.metrics import mean_squared_error, r2_score
 from sklearn.model_selection import train_test_split
 import autosklearn.regression
 
-def train_autosklearn_models(X, y, max_train_secs_per_output=120):
+def train_autosklearn_models(X, y, max_train_secs_per_output=120, memory_limit=1024 * 100):
     X = np.array(X)
     y = np.array(y)
     
     # Split data into train and test sets
     X_train, X_test, y_train, y_test = train_test_split(X, y, test_size=0.15)
 
     # Train autosklearn model for each output variable
     model_paths = []
     for i in range(np.shape(y_train)[1]):
-        model = autosklearn.regression.AutoSklearnRegressor(time_left_for_this_task=max_train_secs_per_output)
+        model = autosklearn.regression.AutoSklearnRegressor(time_left_for_this_task=max_train_secs_per_output, memory_limit=memory_limit)
         model.fit(X_train, y_train[:, i])
         model_path = f'/tmp/automlmoo_models/out{i}_{time.strftime("%Y%m%d-%H%M%S")}.dump'
         os.makedirs(os.path.dirname(model_path), exist_ok=True)
         
         with open(model_path, 'wb') as f:
             pickle.dump(model, f)
```

### Comparing `automlmoo-0.0.1.1/automlmoo/pymoo_optimization.py` & `automlmoo-0.0.1.2/automlmoo/pymoo_optimization.py`

 * *Files identical despite different names*

### Comparing `automlmoo-0.0.1.1/automlmoo/solver.py` & `automlmoo-0.0.1.2/automlmoo/solver.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,18 +11,18 @@
 class Solver():
     def __init__(self):
         self.solutions=None
         self.models_paths=None
         self.num_features=None
         self.num_objectives=None
 
-    def train_models(self, X, y, max_train_secs_per_output=120):
+    def train_models(self, X, y, max_train_secs_per_output=120, memory_limit=1024 * 100):
         self.num_features=np.array(X).shape[1]
         self.num_objectives=np.array(y).shape[1]
-        self.models_paths = autosklearn_modeling.train_autosklearn_models(X, y, max_train_secs_per_output=max_train_secs_per_output)
+        self.models_paths = autosklearn_modeling.train_autosklearn_models(X, y, max_train_secs_per_output=max_train_secs_per_output, memory_limit=memory_limit)
 
     def find_optimal_solution(self, pop_size=500, n_offprings=500, n_gen=None, max_opt_secs=None, objectives_sense=None, inequality_constraints=None, equality_constraints=None, features_lower_bounds=None, features_upper_bounds=None):
         if self.models_paths == None:
             print(f'Sorry. You must create the models before')
         else:
             vectorized_problem = pymoo_optimization.OptimizationProblem(model_paths=self.models_paths, num_features=self.num_features, num_objectives=self.num_objectives, objectives_sense=objectives_sense, inequality_constraints=inequality_constraints, equality_constraints=equality_constraints, features_lower_bounds=features_lower_bounds, features_upper_bounds=features_upper_bounds)
             
@@ -47,18 +47,18 @@
 
             for i, goal in enumerate(vectorized_problem.objectives_sense):
                 if goal == 'maximize':
                     results.F[:, i] = -1 * results.F[:, i]
 
             self.solutions = results
 
-    def train_and_optimize(self, X, y, max_train_secs_per_output=120, pop_size=500, n_offprings=500, n_gen=None, max_opt_secs=None, objectives_sense=None, inequality_constraints=None, equality_constraints=None, features_lower_bounds=None, features_upper_bounds=None):
+    def train_and_optimize(self, X, y, max_train_secs_per_output=120, memory_limit=1024 * 100, pop_size=500, n_offprings=500, n_gen=None, max_opt_secs=None, objectives_sense=None, inequality_constraints=None, equality_constraints=None, features_lower_bounds=None, features_upper_bounds=None):
         self.num_features=np.array(X).shape[1]
         self.num_objectives=np.array(y).shape[1]
-        self.models_paths = autosklearn_modeling.train_autosklearn_models(X, y, max_train_secs_per_output=max_train_secs_per_output)
+        self.models_paths = autosklearn_modeling.train_autosklearn_models(X, y, max_train_secs_per_output=max_train_secs_per_output, memory_limit=memory_limit)
         vectorized_problem = pymoo_optimization.OptimizationProblem(model_paths=self.models_paths, num_features=self.num_features, num_objectives=self.num_objectives, objectives_sense=objectives_sense, inequality_constraints=inequality_constraints, equality_constraints=equality_constraints, features_lower_bounds=features_lower_bounds, features_upper_bounds=features_upper_bounds)
             
         algorithm = NSGA2(
             pop_size=pop_size,
             n_offsprings=n_offprings,
             sampling=FloatRandomSampling(),
             crossover=SBX(prob=0.9, eta=15),
```

### Comparing `automlmoo-0.0.1.1/automlmoo.egg-info/PKG-INFO` & `automlmoo-0.0.1.2/automlmoo.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: automlmoo
-Version: 0.0.1.1
+Version: 0.0.1.2
 Summary: A package for automatic modeling and optimize systems based on data
 Home-page: UNKNOWN
 Author: Yarens J. Cruz
 License: MIT
 Platform: UNKNOWN
 Requires-Python: >=3.7, <3.10
 Description-Content-Type: text/markdown
```

### Comparing `automlmoo-0.0.1.1/setup.py` & `automlmoo-0.0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name='automlmoo',
     packages=find_packages(include=['automlmoo']),
-    version='0.0.1.1',
+    version='0.0.1.2',
     description='A package for automatic modeling and optimize systems based on data',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Yarens J. Cruz',
     install_requires=['auto-sklearn==0.15.0', 'pymoo==0.6.1.1', 'typeguard==4.2.1'],
     python_requires='>=3.7, <3.10',
     setup_requires=['pytest-runner'],
```

