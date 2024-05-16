# Comparing `tmp/inferent_deep-0.0.1.tar.gz` & `tmp/inferent_deep-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inferent_deep-0.0.1.tar", last modified: Thu May 16 12:00:08 2024, max compression
+gzip compressed data, was "inferent_deep-0.0.2.tar", last modified: Thu May 16 13:51:51 2024, max compression
```

## Comparing `inferent_deep-0.0.1.tar` & `inferent_deep-0.0.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 olives     (501) staff       (20)        0 2024-05-16 12:00:08.333067 inferent_deep-0.0.1/
--rw-r--r--   0 olives     (501) staff       (20)     1065 2024-05-16 11:42:37.000000 inferent_deep-0.0.1/LICENSE
--rw-r--r--   0 olives     (501) staff       (20)      696 2024-05-16 12:00:08.332774 inferent_deep-0.0.1/PKG-INFO
--rw-r--r--   0 olives     (501) staff       (20)      126 2024-05-16 11:43:18.000000 inferent_deep-0.0.1/README.md
--rw-r--r--   0 olives     (501) staff       (20)      635 2024-05-16 11:48:15.000000 inferent_deep-0.0.1/pyproject.toml
--rw-r--r--   0 olives     (501) staff       (20)       38 2024-05-16 12:00:08.333120 inferent_deep-0.0.1/setup.cfg
-drwxr-xr-x   0 olives     (501) staff       (20)        0 2024-05-16 12:00:08.328976 inferent_deep-0.0.1/src/
--rw-r--r--   0 olives     (501) staff       (20)        1 2024-05-16 11:42:37.000000 inferent_deep-0.0.1/src/__init__.py
-drwxr-xr-x   0 olives     (501) staff       (20)        0 2024-05-16 12:00:08.329476 inferent_deep-0.0.1/src/inferent-deep/
--rw-r--r--   0 olives     (501) staff       (20)       38 2024-05-16 11:42:37.000000 inferent_deep-0.0.1/src/inferent-deep/__init__.py
-drwxr-xr-x   0 olives     (501) staff       (20)        0 2024-05-16 12:00:08.330818 inferent_deep-0.0.1/src/inferent-deep/training/
--rw-r--r--   0 olives     (501) staff       (20)      103 2024-05-16 11:42:37.000000 inferent_deep-0.0.1/src/inferent-deep/training/__init__.py
--rw-r--r--   0 olives     (501) staff       (20)     3436 2024-05-16 11:42:37.000000 inferent_deep-0.0.1/src/inferent-deep/training/datamanager.py
--rw-r--r--   0 olives     (501) staff       (20)     1214 2024-05-16 11:42:37.000000 inferent_deep-0.0.1/src/inferent-deep/training/predictor.py
--rw-r--r--   0 olives     (501) staff       (20)     3558 2024-05-16 11:42:37.000000 inferent_deep-0.0.1/src/inferent-deep/training/preprocessor.py
--rw-r--r--   0 olives     (501) staff       (20)     8173 2024-05-16 11:42:37.000000 inferent_deep-0.0.1/src/inferent-deep/training/pytorch.py
-drwxr-xr-x   0 olives     (501) staff       (20)        0 2024-05-16 12:00:08.332489 inferent_deep-0.0.1/src/inferent_deep.egg-info/
--rw-r--r--   0 olives     (501) staff       (20)      696 2024-05-16 12:00:08.000000 inferent_deep-0.0.1/src/inferent_deep.egg-info/PKG-INFO
--rw-r--r--   0 olives     (501) staff       (20)      533 2024-05-16 12:00:08.000000 inferent_deep-0.0.1/src/inferent_deep.egg-info/SOURCES.txt
--rw-r--r--   0 olives     (501) staff       (20)        1 2024-05-16 12:00:08.000000 inferent_deep-0.0.1/src/inferent_deep.egg-info/dependency_links.txt
--rw-r--r--   0 olives     (501) staff       (20)       26 2024-05-16 12:00:08.000000 inferent_deep-0.0.1/src/inferent_deep.egg-info/requires.txt
--rw-r--r--   0 olives     (501) staff       (20)       29 2024-05-16 12:00:08.000000 inferent_deep-0.0.1/src/inferent_deep.egg-info/top_level.txt
-drwxr-xr-x   0 olives     (501) staff       (20)        0 2024-05-16 12:00:08.332165 inferent_deep-0.0.1/src/tests/
--rw-r--r--   0 olives     (501) staff       (20)        0 2024-05-16 11:42:37.000000 inferent_deep-0.0.1/src/tests/__init__.py
--rw-r--r--   0 olives     (501) staff       (20)      646 2024-05-16 11:42:37.000000 inferent_deep-0.0.1/src/tests/test_training.py
+drwxr-xr-x   0 olives     (501) staff       (20)        0 2024-05-16 13:51:51.007179 inferent_deep-0.0.2/
+-rw-r--r--   0 olives     (501) staff       (20)     1065 2024-05-16 11:42:37.000000 inferent_deep-0.0.2/LICENSE
+-rw-r--r--   0 olives     (501) staff       (20)      696 2024-05-16 13:51:51.006891 inferent_deep-0.0.2/PKG-INFO
+-rw-r--r--   0 olives     (501) staff       (20)      126 2024-05-16 11:43:18.000000 inferent_deep-0.0.2/README.md
+-rw-r--r--   0 olives     (501) staff       (20)      635 2024-05-16 13:51:45.000000 inferent_deep-0.0.2/pyproject.toml
+-rw-r--r--   0 olives     (501) staff       (20)       38 2024-05-16 13:51:51.007260 inferent_deep-0.0.2/setup.cfg
+drwxr-xr-x   0 olives     (501) staff       (20)        0 2024-05-16 13:51:51.003015 inferent_deep-0.0.2/src/
+-rw-r--r--   0 olives     (501) staff       (20)        1 2024-05-16 11:42:37.000000 inferent_deep-0.0.2/src/__init__.py
+drwxr-xr-x   0 olives     (501) staff       (20)        0 2024-05-16 13:51:51.006522 inferent_deep-0.0.2/src/inferent_deep.egg-info/
+-rw-r--r--   0 olives     (501) staff       (20)      696 2024-05-16 13:51:50.000000 inferent_deep-0.0.2/src/inferent_deep.egg-info/PKG-INFO
+-rw-r--r--   0 olives     (501) staff       (20)      527 2024-05-16 13:51:50.000000 inferent_deep-0.0.2/src/inferent_deep.egg-info/SOURCES.txt
+-rw-r--r--   0 olives     (501) staff       (20)        1 2024-05-16 13:51:50.000000 inferent_deep-0.0.2/src/inferent_deep.egg-info/dependency_links.txt
+-rw-r--r--   0 olives     (501) staff       (20)       26 2024-05-16 13:51:50.000000 inferent_deep-0.0.2/src/inferent_deep.egg-info/requires.txt
+-rw-r--r--   0 olives     (501) staff       (20)       28 2024-05-16 13:51:50.000000 inferent_deep-0.0.2/src/inferent_deep.egg-info/top_level.txt
+drwxr-xr-x   0 olives     (501) staff       (20)        0 2024-05-16 13:51:51.004405 inferent_deep-0.0.2/src/inferentdeep/
+-rw-r--r--   0 olives     (501) staff       (20)       38 2024-05-16 11:42:37.000000 inferent_deep-0.0.2/src/inferentdeep/__init__.py
+drwxr-xr-x   0 olives     (501) staff       (20)        0 2024-05-16 13:51:51.005765 inferent_deep-0.0.2/src/inferentdeep/training/
+-rw-r--r--   0 olives     (501) staff       (20)      103 2024-05-16 11:42:37.000000 inferent_deep-0.0.2/src/inferentdeep/training/__init__.py
+-rw-r--r--   0 olives     (501) staff       (20)     3436 2024-05-16 11:42:37.000000 inferent_deep-0.0.2/src/inferentdeep/training/datamanager.py
+-rw-r--r--   0 olives     (501) staff       (20)     1214 2024-05-16 11:42:37.000000 inferent_deep-0.0.2/src/inferentdeep/training/predictor.py
+-rw-r--r--   0 olives     (501) staff       (20)     3558 2024-05-16 11:42:37.000000 inferent_deep-0.0.2/src/inferentdeep/training/preprocessor.py
+-rw-r--r--   0 olives     (501) staff       (20)     8173 2024-05-16 11:42:37.000000 inferent_deep-0.0.2/src/inferentdeep/training/pytorch.py
+drwxr-xr-x   0 olives     (501) staff       (20)        0 2024-05-16 13:51:51.006216 inferent_deep-0.0.2/src/tests/
+-rw-r--r--   0 olives     (501) staff       (20)        0 2024-05-16 11:42:37.000000 inferent_deep-0.0.2/src/tests/__init__.py
+-rw-r--r--   0 olives     (501) staff       (20)      646 2024-05-16 11:42:37.000000 inferent_deep-0.0.2/src/tests/test_training.py
```

### Comparing `inferent_deep-0.0.1/LICENSE` & `inferent_deep-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `inferent_deep-0.0.1/PKG-INFO` & `inferent_deep-0.0.2/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inferent-deep
-Version: 0.0.1
+Version: 0.0.2
 Summary: Inferent Ventures - Deep Learning Tools
 Author-email: Inferent Ventures <inferentventures@gmail.com>
 Project-URL: Homepage, https://github.com/inferent
 Project-URL: Issues, https://github.com/inferent
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `inferent_deep-0.0.1/pyproject.toml` & `inferent_deep-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "inferent-deep"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Inferent Ventures", email="inferentventures@gmail.com" },
 ]
 description = "Inferent Ventures - Deep Learning Tools"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `inferent_deep-0.0.1/src/inferent-deep/training/datamanager.py` & `inferent_deep-0.0.2/src/inferentdeep/training/datamanager.py`

 * *Files identical despite different names*

### Comparing `inferent_deep-0.0.1/src/inferent-deep/training/predictor.py` & `inferent_deep-0.0.2/src/inferentdeep/training/predictor.py`

 * *Files identical despite different names*

### Comparing `inferent_deep-0.0.1/src/inferent-deep/training/preprocessor.py` & `inferent_deep-0.0.2/src/inferentdeep/training/preprocessor.py`

 * *Files identical despite different names*

### Comparing `inferent_deep-0.0.1/src/inferent-deep/training/pytorch.py` & `inferent_deep-0.0.2/src/inferentdeep/training/pytorch.py`

 * *Files identical despite different names*

### Comparing `inferent_deep-0.0.1/src/inferent_deep.egg-info/PKG-INFO` & `inferent_deep-0.0.2/src/inferent_deep.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inferent-deep
-Version: 0.0.1
+Version: 0.0.2
 Summary: Inferent Ventures - Deep Learning Tools
 Author-email: Inferent Ventures <inferentventures@gmail.com>
 Project-URL: Homepage, https://github.com/inferent
 Project-URL: Issues, https://github.com/inferent
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `inferent_deep-0.0.1/src/inferent_deep.egg-info/SOURCES.txt` & `inferent_deep-0.0.2/src/inferent_deep.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 LICENSE
 README.md
 pyproject.toml
 src/__init__.py
-src/inferent-deep/__init__.py
-src/inferent-deep/training/__init__.py
-src/inferent-deep/training/datamanager.py
-src/inferent-deep/training/predictor.py
-src/inferent-deep/training/preprocessor.py
-src/inferent-deep/training/pytorch.py
 src/inferent_deep.egg-info/PKG-INFO
 src/inferent_deep.egg-info/SOURCES.txt
 src/inferent_deep.egg-info/dependency_links.txt
 src/inferent_deep.egg-info/requires.txt
 src/inferent_deep.egg-info/top_level.txt
+src/inferentdeep/__init__.py
+src/inferentdeep/training/__init__.py
+src/inferentdeep/training/datamanager.py
+src/inferentdeep/training/predictor.py
+src/inferentdeep/training/preprocessor.py
+src/inferentdeep/training/pytorch.py
 src/tests/__init__.py
 src/tests/test_training.py
```

### Comparing `inferent_deep-0.0.1/src/tests/test_training.py` & `inferent_deep-0.0.2/src/tests/test_training.py`

 * *Files identical despite different names*

