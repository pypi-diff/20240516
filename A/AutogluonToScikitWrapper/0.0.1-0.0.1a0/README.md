# Comparing `tmp/AutogluonToScikitWrapper-0.0.1.tar.gz` & `tmp/AutogluonToScikitWrapper-0.0.1a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AutogluonToScikitWrapper-0.0.1.tar", last modified: Thu May 16 11:59:32 2024, max compression
+gzip compressed data, was "AutogluonToScikitWrapper-0.0.1a0.tar", last modified: Thu May 16 13:02:15 2024, max compression
```

## Comparing `AutogluonToScikitWrapper-0.0.1.tar` & `AutogluonToScikitWrapper-0.0.1a0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-05-16 11:59:32.015195 AutogluonToScikitWrapper-0.0.1/
-drwxrwxrwx   0        0        0        0 2024-05-16 11:59:32.004321 AutogluonToScikitWrapper-0.0.1/AutogluonToScikitWrapper.egg-info/
--rw-rw-rw-   0        0        0      632 2024-05-16 11:59:31.000000 AutogluonToScikitWrapper-0.0.1/AutogluonToScikitWrapper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      299 2024-05-16 11:59:31.000000 AutogluonToScikitWrapper-0.0.1/AutogluonToScikitWrapper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-16 11:59:31.000000 AutogluonToScikitWrapper-0.0.1/AutogluonToScikitWrapper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2024-05-16 11:59:31.000000 AutogluonToScikitWrapper-0.0.1/AutogluonToScikitWrapper.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-05-16 11:59:31.000000 AutogluonToScikitWrapper-0.0.1/AutogluonToScikitWrapper.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      632 2024-05-16 11:59:32.015195 AutogluonToScikitWrapper-0.0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-16 11:59:32.015195 AutogluonToScikitWrapper-0.0.1/agksWrapper/
--rw-rw-rw-   0        0        0       51 2024-05-16 11:39:53.000000 AutogluonToScikitWrapper-0.0.1/agksWrapper/__init__.py
--rw-rw-rw-   0        0        0     2377 2024-05-16 11:39:53.000000 AutogluonToScikitWrapper-0.0.1/agksWrapper/agsk_warpper.py
--rw-rw-rw-   0        0        0       42 2024-05-16 11:59:32.015195 AutogluonToScikitWrapper-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      883 2024-05-16 11:59:18.000000 AutogluonToScikitWrapper-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-16 13:02:15.010303 AutogluonToScikitWrapper-0.0.1a0/
+drwxrwxrwx   0        0        0        0 2024-05-16 13:02:15.003277 AutogluonToScikitWrapper-0.0.1a0/AutogluonToScikitWrapper.egg-info/
+-rw-rw-rw-   0        0        0      634 2024-05-16 13:02:14.000000 AutogluonToScikitWrapper-0.0.1a0/AutogluonToScikitWrapper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      299 2024-05-16 13:02:14.000000 AutogluonToScikitWrapper-0.0.1a0/AutogluonToScikitWrapper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-16 13:02:14.000000 AutogluonToScikitWrapper-0.0.1a0/AutogluonToScikitWrapper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2024-05-16 13:02:14.000000 AutogluonToScikitWrapper-0.0.1a0/AutogluonToScikitWrapper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-05-16 13:02:14.000000 AutogluonToScikitWrapper-0.0.1a0/AutogluonToScikitWrapper.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      634 2024-05-16 13:02:15.010303 AutogluonToScikitWrapper-0.0.1a0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-16 13:02:15.003277 AutogluonToScikitWrapper-0.0.1a0/agksWrapper/
+-rw-rw-rw-   0        0        0       51 2024-05-16 12:18:30.000000 AutogluonToScikitWrapper-0.0.1a0/agksWrapper/__init__.py
+-rw-rw-rw-   0        0        0     2377 2024-05-16 11:39:53.000000 AutogluonToScikitWrapper-0.0.1a0/agksWrapper/agsk_wrapper.py
+-rw-rw-rw-   0        0        0       42 2024-05-16 13:02:15.010303 AutogluonToScikitWrapper-0.0.1a0/setup.cfg
+-rw-rw-rw-   0        0        0      884 2024-05-16 13:02:10.000000 AutogluonToScikitWrapper-0.0.1a0/setup.py
```

### Comparing `AutogluonToScikitWrapper-0.0.1/AutogluonToScikitWrapper.egg-info/PKG-INFO` & `AutogluonToScikitWrapper-0.0.1a0/AutogluonToScikitWrapper.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AutogluonToScikitWrapper
-Version: 0.0.1
+Version: 0.0.1a0
 Summary: Autogluon to Scikit Wrapper
 Home-page: UNKNOWN
 Author: Arijit Singh
 Author-email: arijit@easydata.ai
 License: UNKNOWN
 Keywords: Autogluon,Scikit-learn,wrapper
 Platform: UNKNOWN
```

### Comparing `AutogluonToScikitWrapper-0.0.1/PKG-INFO` & `AutogluonToScikitWrapper-0.0.1a0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AutogluonToScikitWrapper
-Version: 0.0.1
+Version: 0.0.1a0
 Summary: Autogluon to Scikit Wrapper
 Home-page: UNKNOWN
 Author: Arijit Singh
 Author-email: arijit@easydata.ai
 License: UNKNOWN
 Keywords: Autogluon,Scikit-learn,wrapper
 Platform: UNKNOWN
```

### Comparing `AutogluonToScikitWrapper-0.0.1/agksWrapper/agsk_warpper.py` & `AutogluonToScikitWrapper-0.0.1a0/agksWrapper/agsk_wrapper.py`

 * *Files identical despite different names*

### Comparing `AutogluonToScikitWrapper-0.0.1/setup.py` & `AutogluonToScikitWrapper-0.0.1a0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.1'
+VERSION = '0.0.1a'
 DESCRIPTION = 'Autogluon to Scikit Wrapper'
 LONG_DESCRIPTION = (
     'A wrapper which converts Autogluon models to Scikit-Learn models, '
     'thus breaking any limitation faced by user when implementing Scikit-learn methods to Autogluon Models'
 )
 
 # Setting up
```

