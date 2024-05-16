# Comparing `tmp/panelsplit-0.3.0.tar.gz` & `tmp/panelsplit-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "panelsplit-0.3.0.tar", last modified: Wed May  8 20:48:20 2024, max compression
+gzip compressed data, was "panelsplit-0.4.0.tar", last modified: Tue May 14 18:38:08 2024, max compression
```

## Comparing `panelsplit-0.3.0.tar` & `panelsplit-0.4.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 ericfrey   (501) staff       (20)        0 2024-05-08 20:48:20.273117 panelsplit-0.3.0/
--rw-r--r--   0 ericfrey   (501) staff       (20)      411 2024-05-08 20:39:25.000000 panelsplit-0.3.0/CITATION.cff
--rw-r--r--   0 ericfrey   (501) staff       (20)     1081 2024-03-26 16:58:07.000000 panelsplit-0.3.0/LICENSE
--rw-r--r--   0 ericfrey   (501) staff       (20)     8094 2024-05-08 20:48:20.272018 panelsplit-0.3.0/PKG-INFO
--rw-r--r--   0 ericfrey   (501) staff       (20)     7644 2024-03-26 16:58:07.000000 panelsplit-0.3.0/README.md
-drwxr-xr-x   0 ericfrey   (501) staff       (20)        0 2024-05-08 20:48:20.261206 panelsplit-0.3.0/examples/
--rw-r--r--   0 ericfrey   (501) staff       (20)   108532 2024-03-26 16:58:07.000000 panelsplit-0.3.0/examples/An introduction to PanelSplit.ipynb
-drwxr-xr-x   0 ericfrey   (501) staff       (20)        0 2024-05-08 20:48:20.264761 panelsplit-0.3.0/panelsplit/
--rw-r--r--   0 ericfrey   (501) staff       (20)       35 2024-02-19 10:30:46.000000 panelsplit-0.3.0/panelsplit/__init__.py
--rw-r--r--   0 ericfrey   (501) staff       (20)    18101 2024-05-08 20:00:30.000000 panelsplit-0.3.0/panelsplit/panelsplit.py
-drwxr-xr-x   0 ericfrey   (501) staff       (20)        0 2024-05-08 20:48:20.268916 panelsplit-0.3.0/panelsplit.egg-info/
--rw-r--r--   0 ericfrey   (501) staff       (20)     8094 2024-05-08 20:48:19.000000 panelsplit-0.3.0/panelsplit.egg-info/PKG-INFO
--rw-r--r--   0 ericfrey   (501) staff       (20)      344 2024-05-08 20:48:20.000000 panelsplit-0.3.0/panelsplit.egg-info/SOURCES.txt
--rw-r--r--   0 ericfrey   (501) staff       (20)        1 2024-05-08 20:48:19.000000 panelsplit-0.3.0/panelsplit.egg-info/dependency_links.txt
--rw-r--r--   0 ericfrey   (501) staff       (20)       49 2024-05-08 20:48:19.000000 panelsplit-0.3.0/panelsplit.egg-info/requires.txt
--rw-r--r--   0 ericfrey   (501) staff       (20)       11 2024-05-08 20:48:19.000000 panelsplit-0.3.0/panelsplit.egg-info/top_level.txt
--rw-r--r--   0 ericfrey   (501) staff       (20)       38 2024-05-08 20:48:20.273360 panelsplit-0.3.0/setup.cfg
--rw-r--r--   0 ericfrey   (501) staff       (20)     1219 2024-05-08 20:35:39.000000 panelsplit-0.3.0/setup.py
-drwxr-xr-x   0 ericfrey   (501) staff       (20)        0 2024-05-08 20:48:20.269904 panelsplit-0.3.0/tests/
--rw-r--r--   0 ericfrey   (501) staff       (20)        0 2024-05-08 20:04:00.000000 panelsplit-0.3.0/tests/__init__.py
--rw-r--r--   0 ericfrey   (501) staff       (20)     1649 2024-05-08 20:30:49.000000 panelsplit-0.3.0/tests/test_PanelSplit.py
+drwxr-xr-x   0 ericfrey   (501) staff       (20)        0 2024-05-14 18:38:08.623797 panelsplit-0.4.0/
+-rw-r--r--   0 ericfrey   (501) staff       (20)      411 2024-05-14 18:31:39.000000 panelsplit-0.4.0/CITATION.cff
+-rw-r--r--   0 ericfrey   (501) staff       (20)     1081 2024-03-26 16:58:07.000000 panelsplit-0.4.0/LICENSE
+-rw-r--r--   0 ericfrey   (501) staff       (20)     8094 2024-05-14 18:38:08.623222 panelsplit-0.4.0/PKG-INFO
+-rw-r--r--   0 ericfrey   (501) staff       (20)     7644 2024-03-26 16:58:07.000000 panelsplit-0.4.0/README.md
+drwxr-xr-x   0 ericfrey   (501) staff       (20)        0 2024-05-14 18:38:08.611773 panelsplit-0.4.0/examples/
+-rw-r--r--   0 ericfrey   (501) staff       (20)   108532 2024-03-26 16:58:07.000000 panelsplit-0.4.0/examples/An introduction to PanelSplit.ipynb
+drwxr-xr-x   0 ericfrey   (501) staff       (20)        0 2024-05-14 18:38:08.614918 panelsplit-0.4.0/panelsplit/
+-rw-r--r--   0 ericfrey   (501) staff       (20)       35 2024-02-19 10:30:46.000000 panelsplit-0.4.0/panelsplit/__init__.py
+-rw-r--r--   0 ericfrey   (501) staff       (20)    18154 2024-05-14 18:21:17.000000 panelsplit-0.4.0/panelsplit/panelsplit.py
+drwxr-xr-x   0 ericfrey   (501) staff       (20)        0 2024-05-14 18:38:08.620047 panelsplit-0.4.0/panelsplit.egg-info/
+-rw-r--r--   0 ericfrey   (501) staff       (20)     8094 2024-05-14 18:38:08.000000 panelsplit-0.4.0/panelsplit.egg-info/PKG-INFO
+-rw-r--r--   0 ericfrey   (501) staff       (20)      344 2024-05-14 18:38:08.000000 panelsplit-0.4.0/panelsplit.egg-info/SOURCES.txt
+-rw-r--r--   0 ericfrey   (501) staff       (20)        1 2024-05-14 18:38:08.000000 panelsplit-0.4.0/panelsplit.egg-info/dependency_links.txt
+-rw-r--r--   0 ericfrey   (501) staff       (20)       49 2024-05-14 18:38:08.000000 panelsplit-0.4.0/panelsplit.egg-info/requires.txt
+-rw-r--r--   0 ericfrey   (501) staff       (20)       11 2024-05-14 18:38:08.000000 panelsplit-0.4.0/panelsplit.egg-info/top_level.txt
+-rw-r--r--   0 ericfrey   (501) staff       (20)       38 2024-05-14 18:38:08.624010 panelsplit-0.4.0/setup.cfg
+-rw-r--r--   0 ericfrey   (501) staff       (20)     1219 2024-05-14 18:31:51.000000 panelsplit-0.4.0/setup.py
+drwxr-xr-x   0 ericfrey   (501) staff       (20)        0 2024-05-14 18:38:08.621471 panelsplit-0.4.0/tests/
+-rw-r--r--   0 ericfrey   (501) staff       (20)        0 2024-05-08 20:04:00.000000 panelsplit-0.4.0/tests/__init__.py
+-rw-r--r--   0 ericfrey   (501) staff       (20)     2899 2024-05-13 21:59:15.000000 panelsplit-0.4.0/tests/test_PanelSplit.py
```

### Comparing `panelsplit-0.3.0/LICENSE` & `panelsplit-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `panelsplit-0.3.0/PKG-INFO` & `panelsplit-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: panelsplit
-Version: 0.3.0
+Version: 0.4.0
 Summary: A tool for panel data analysis.
 Home-page: https://github.com/4Freye/panelsplit
 Author: Eric Frey, Ben Seimon
 Author-email: eric.frey@bse.eu, benjamin.seimon@bse.eu
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `panelsplit-0.3.0/README.md` & `panelsplit-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `panelsplit-0.3.0/examples/An introduction to PanelSplit.ipynb` & `panelsplit-0.4.0/examples/An introduction to PanelSplit.ipynb`

 * *Files identical despite different names*

### Comparing `panelsplit-0.3.0/panelsplit/panelsplit.py` & `panelsplit-0.4.0/panelsplit/panelsplit.py`

 * *Files 1% similar despite different names*

```diff
@@ -193,21 +193,22 @@
         - sample_weight: Optional pandas Series or numpy array (default=None). Sample weights for the training data.
         - n_jobs: Optional int (default=1). The number of jobs to run in parallel.
 
         Returns:
         list of fitted models: List containing fitted models for each split.
         """
         def fit_split(train_indices):
+            local_estimator = clone(estimator)
             y_train = y.loc[train_indices].dropna()
             X_train = X.loc[y_train.index]
             if sample_weight is not None:
                 sw = sample_weight.loc[y_train.index]
             else:
                 sw = None
-            return estimator.fit(X_train, y_train, sample_weight=sw)
+            return local_estimator.fit(X_train, y_train, sample_weight=sw)
 
         fitted_estimators = Parallel(n_jobs=n_jobs)(
             delayed(fit_split)(train_indices)
             for train_indices, _ in self._split_wrapper(self.split())
         )
         return fitted_estimators
```

### Comparing `panelsplit-0.3.0/panelsplit.egg-info/PKG-INFO` & `panelsplit-0.4.0/panelsplit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: panelsplit
-Version: 0.3.0
+Version: 0.4.0
 Summary: A tool for panel data analysis.
 Home-page: https://github.com/4Freye/panelsplit
 Author: Eric Frey, Ben Seimon
 Author-email: eric.frey@bse.eu, benjamin.seimon@bse.eu
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `panelsplit-0.3.0/setup.py` & `panelsplit-0.4.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # Read the contents of the README file
 with open('README.md', 'r') as f:
     long_description = f.read()
 
 setup(
     name='panelsplit',
-    version='0.3.0',
+    version='0.4.0',
     packages=find_packages(include=['panelsplit', 'panelsplit.*']),  # Include only packages within the "panelsplit" folder
 
     # Metadata
     author='Eric Frey, Ben Seimon',
     author_email='eric.frey@bse.eu, benjamin.seimon@bse.eu',
     description='A tool for panel data analysis.',
     url='https://github.com/4Freye/panelsplit',  # URL to your GitHub repository
```

