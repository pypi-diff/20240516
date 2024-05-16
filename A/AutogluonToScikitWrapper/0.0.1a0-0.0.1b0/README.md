# Comparing `tmp/AutogluonToScikitWrapper-0.0.1a0.tar.gz` & `tmp/AutogluonToScikitWrapper-0.0.1b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AutogluonToScikitWrapper-0.0.1a0.tar", last modified: Thu May 16 13:02:15 2024, max compression
+gzip compressed data, was "AutogluonToScikitWrapper-0.0.1b0.tar", last modified: Thu May 16 13:08:30 2024, max compression
```

## Comparing `AutogluonToScikitWrapper-0.0.1a0.tar` & `AutogluonToScikitWrapper-0.0.1b0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-05-16 13:02:15.010303 AutogluonToScikitWrapper-0.0.1a0/
-drwxrwxrwx   0        0        0        0 2024-05-16 13:02:15.003277 AutogluonToScikitWrapper-0.0.1a0/AutogluonToScikitWrapper.egg-info/
--rw-rw-rw-   0        0        0      634 2024-05-16 13:02:14.000000 AutogluonToScikitWrapper-0.0.1a0/AutogluonToScikitWrapper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      299 2024-05-16 13:02:14.000000 AutogluonToScikitWrapper-0.0.1a0/AutogluonToScikitWrapper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-16 13:02:14.000000 AutogluonToScikitWrapper-0.0.1a0/AutogluonToScikitWrapper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2024-05-16 13:02:14.000000 AutogluonToScikitWrapper-0.0.1a0/AutogluonToScikitWrapper.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-05-16 13:02:14.000000 AutogluonToScikitWrapper-0.0.1a0/AutogluonToScikitWrapper.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      634 2024-05-16 13:02:15.010303 AutogluonToScikitWrapper-0.0.1a0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-16 13:02:15.003277 AutogluonToScikitWrapper-0.0.1a0/agksWrapper/
--rw-rw-rw-   0        0        0       51 2024-05-16 12:18:30.000000 AutogluonToScikitWrapper-0.0.1a0/agksWrapper/__init__.py
--rw-rw-rw-   0        0        0     2377 2024-05-16 11:39:53.000000 AutogluonToScikitWrapper-0.0.1a0/agksWrapper/agsk_wrapper.py
--rw-rw-rw-   0        0        0       42 2024-05-16 13:02:15.010303 AutogluonToScikitWrapper-0.0.1a0/setup.cfg
--rw-rw-rw-   0        0        0      884 2024-05-16 13:02:10.000000 AutogluonToScikitWrapper-0.0.1a0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-16 13:08:30.577667 AutogluonToScikitWrapper-0.0.1b0/
+drwxrwxrwx   0        0        0        0 2024-05-16 13:08:30.565729 AutogluonToScikitWrapper-0.0.1b0/AutogluonToScikitWrapper.egg-info/
+-rw-rw-rw-   0        0        0      634 2024-05-16 13:08:30.000000 AutogluonToScikitWrapper-0.0.1b0/AutogluonToScikitWrapper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      299 2024-05-16 13:08:30.000000 AutogluonToScikitWrapper-0.0.1b0/AutogluonToScikitWrapper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-16 13:08:30.000000 AutogluonToScikitWrapper-0.0.1b0/AutogluonToScikitWrapper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2024-05-16 13:08:30.000000 AutogluonToScikitWrapper-0.0.1b0/AutogluonToScikitWrapper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-05-16 13:08:30.000000 AutogluonToScikitWrapper-0.0.1b0/AutogluonToScikitWrapper.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      634 2024-05-16 13:08:30.577667 AutogluonToScikitWrapper-0.0.1b0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-16 13:08:30.565729 AutogluonToScikitWrapper-0.0.1b0/agksWrapper/
+-rw-rw-rw-   0        0        0       57 2024-05-16 13:08:20.000000 AutogluonToScikitWrapper-0.0.1b0/agksWrapper/__init__.py
+-rw-rw-rw-   0        0        0     2383 2024-05-16 13:08:20.000000 AutogluonToScikitWrapper-0.0.1b0/agksWrapper/agsk_wrapper.py
+-rw-rw-rw-   0        0        0       42 2024-05-16 13:08:30.578880 AutogluonToScikitWrapper-0.0.1b0/setup.cfg
+-rw-rw-rw-   0        0        0      884 2024-05-16 13:08:23.000000 AutogluonToScikitWrapper-0.0.1b0/setup.py
```

### Comparing `AutogluonToScikitWrapper-0.0.1a0/AutogluonToScikitWrapper.egg-info/PKG-INFO` & `AutogluonToScikitWrapper-0.0.1b0/AutogluonToScikitWrapper.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AutogluonToScikitWrapper
-Version: 0.0.1a0
+Version: 0.0.1b0
 Summary: Autogluon to Scikit Wrapper
 Home-page: UNKNOWN
 Author: Arijit Singh
 Author-email: arijit@easydata.ai
 License: UNKNOWN
 Keywords: Autogluon,Scikit-learn,wrapper
 Platform: UNKNOWN
```

### Comparing `AutogluonToScikitWrapper-0.0.1a0/PKG-INFO` & `AutogluonToScikitWrapper-0.0.1b0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AutogluonToScikitWrapper
-Version: 0.0.1a0
+Version: 0.0.1b0
 Summary: Autogluon to Scikit Wrapper
 Home-page: UNKNOWN
 Author: Arijit Singh
 Author-email: arijit@easydata.ai
 License: UNKNOWN
 Keywords: Autogluon,Scikit-learn,wrapper
 Platform: UNKNOWN
```

### Comparing `AutogluonToScikitWrapper-0.0.1a0/agksWrapper/agsk_wrapper.py` & `AutogluonToScikitWrapper-0.0.1b0/agksWrapper/agsk_wrapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from sklearn.base import BaseEstimator, ClassifierMixin
 from autogluon.tabular import TabularDataset
 
 
-class AutogluonToScikitWrapper(BaseEstimator, ClassifierMixin):
+class AutogluonToScikitWrapperMethod(BaseEstimator, ClassifierMixin):
 
     def __init__(self, **kwargs):
         self.init = None
         self.classes_ = []
         self._estimator_type = "classifier"
         if len(kwargs) != 0:
             self.mdl = TabularPredictor(**kwargs)
```

### Comparing `AutogluonToScikitWrapper-0.0.1a0/setup.py` & `AutogluonToScikitWrapper-0.0.1b0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.1a'
+VERSION = '0.0.1b'
 DESCRIPTION = 'Autogluon to Scikit Wrapper'
 LONG_DESCRIPTION = (
     'A wrapper which converts Autogluon models to Scikit-Learn models, '
     'thus breaking any limitation faced by user when implementing Scikit-learn methods to Autogluon Models'
 )
 
 # Setting up
```

