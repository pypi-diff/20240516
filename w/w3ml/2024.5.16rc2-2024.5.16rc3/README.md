# Comparing `tmp/w3ml-2024.5.16rc2.tar.gz` & `tmp/w3ml-2024.5.16rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/w3ml-2024.5.16rc2.tar", last modified: Thu May 16 03:53:09 2024, max compression
+gzip compressed data, was "dist/w3ml-2024.5.16rc3.tar", last modified: Thu May 16 03:57:58 2024, max compression
```

## Comparing `w3ml-2024.5.16rc2.tar` & `w3ml-2024.5.16rc3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 03:53:09.000000 w3ml-2024.5.16rc2/
--rw-r--r--   0 runner    (1001) docker     (127)      481 2024-05-16 03:53:09.000000 w3ml-2024.5.16rc2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-05-16 03:53:01.000000 w3ml-2024.5.16rc2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 03:53:09.000000 w3ml-2024.5.16rc2/w3ml/
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-16 03:53:01.000000 w3ml-2024.5.16rc2/w3ml/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 03:53:09.000000 w3ml-2024.5.16rc2/w3ml/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-16 03:53:01.000000 w3ml-2024.5.16rc2/w3ml/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 03:53:09.000000 w3ml-2024.5.16rc2/w3ml/models/
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-16 03:53:01.000000 w3ml-2024.5.16rc2/w3ml/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 03:53:09.000000 w3ml-2024.5.16rc2/w3ml/models/contrib/
--rw-r--r--   0 runner    (1001) docker     (127)      255 2024-05-16 03:53:01.000000 w3ml-2024.5.16rc2/w3ml/models/contrib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6220 2024-05-16 03:53:01.000000 w3ml-2024.5.16rc2/w3ml/models/contrib/automl_multilabel.py
--rw-r--r--   0 runner    (1001) docker     (127)    10188 2024-05-16 03:53:01.000000 w3ml-2024.5.16rc2/w3ml/models/contrib/automl_binary.py
--rw-r--r--   0 runner    (1001) docker     (127)     9527 2024-05-16 03:53:01.000000 w3ml-2024.5.16rc2/w3ml/models/contrib/automl_multiclass.py
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-16 03:53:01.000000 w3ml-2024.5.16rc2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 03:53:09.000000 w3ml-2024.5.16rc2/w3ml.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      481 2024-05-16 03:53:09.000000 w3ml-2024.5.16rc2/w3ml.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-16 03:53:09.000000 w3ml-2024.5.16rc2/w3ml.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-16 03:53:09.000000 w3ml-2024.5.16rc2/w3ml.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)      380 2024-05-16 03:53:09.000000 w3ml-2024.5.16rc2/w3ml.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 03:53:09.000000 w3ml-2024.5.16rc2/w3ml.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 03:53:09.000000 w3ml-2024.5.16rc2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-05-16 03:53:01.000000 w3ml-2024.5.16rc2/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 03:57:58.000000 w3ml-2024.5.16rc3/
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-05-16 03:57:58.000000 w3ml-2024.5.16rc3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-05-16 03:57:49.000000 w3ml-2024.5.16rc3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 03:57:58.000000 w3ml-2024.5.16rc3/w3ml/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-16 03:57:49.000000 w3ml-2024.5.16rc3/w3ml/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 03:57:58.000000 w3ml-2024.5.16rc3/w3ml/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-16 03:57:49.000000 w3ml-2024.5.16rc3/w3ml/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 03:57:58.000000 w3ml-2024.5.16rc3/w3ml/models/
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-16 03:57:49.000000 w3ml-2024.5.16rc3/w3ml/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 03:57:58.000000 w3ml-2024.5.16rc3/w3ml/models/contrib/
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2024-05-16 03:57:49.000000 w3ml-2024.5.16rc3/w3ml/models/contrib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6220 2024-05-16 03:57:49.000000 w3ml-2024.5.16rc3/w3ml/models/contrib/automl_multilabel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10188 2024-05-16 03:57:49.000000 w3ml-2024.5.16rc3/w3ml/models/contrib/automl_binary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9527 2024-05-16 03:57:49.000000 w3ml-2024.5.16rc3/w3ml/models/contrib/automl_multiclass.py
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-16 03:57:49.000000 w3ml-2024.5.16rc3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 03:57:58.000000 w3ml-2024.5.16rc3/w3ml.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-05-16 03:57:58.000000 w3ml-2024.5.16rc3/w3ml.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-16 03:57:58.000000 w3ml-2024.5.16rc3/w3ml.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-16 03:57:58.000000 w3ml-2024.5.16rc3/w3ml.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-05-16 03:57:58.000000 w3ml-2024.5.16rc3/w3ml.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 03:57:58.000000 w3ml-2024.5.16rc3/w3ml.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 03:57:58.000000 w3ml-2024.5.16rc3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-05-16 03:57:49.000000 w3ml-2024.5.16rc3/LICENSE
```

### Comparing `w3ml-2024.5.16rc2/setup.py` & `w3ml-2024.5.16rc3/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -30,11 +30,11 @@
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     python_requires=">=3.7",
     install_requires=[
         "autogluon.tabular==0.5.0",
-        "numpy>=1.19.2,<1.20",
+        "numpy<1.23,>=1.21",
         "pandas>=1.1.1,<1.2.0",
     ],
 )
```

### Comparing `w3ml-2024.5.16rc2/w3ml/models/contrib/automl_multilabel.py` & `w3ml-2024.5.16rc3/w3ml/models/contrib/automl_multilabel.py`

 * *Files identical despite different names*

### Comparing `w3ml-2024.5.16rc2/w3ml/models/contrib/automl_binary.py` & `w3ml-2024.5.16rc3/w3ml/models/contrib/automl_binary.py`

 * *Files identical despite different names*

### Comparing `w3ml-2024.5.16rc2/w3ml/models/contrib/automl_multiclass.py` & `w3ml-2024.5.16rc3/w3ml/models/contrib/automl_multiclass.py`

 * *Files identical despite different names*

### Comparing `w3ml-2024.5.16rc2/LICENSE` & `w3ml-2024.5.16rc3/LICENSE`

 * *Files identical despite different names*

