# Comparing `tmp/w3ml-2024.3.21rc0.tar.gz` & `tmp/w3ml-2024.5.16rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/w3ml-2024.3.21rc0.tar", last modified: Thu Mar 21 09:16:40 2024, max compression
+gzip compressed data, was "dist/w3ml-2024.5.16rc1.tar", last modified: Thu May 16 02:41:17 2024, max compression
```

## Comparing `w3ml-2024.3.21rc0.tar` & `w3ml-2024.5.16rc1.tar`

### file list

```diff
@@ -1,21 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 09:16:40.000000 w3ml-2024.3.21rc0/
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-03-21 09:16:30.000000 w3ml-2024.3.21rc0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 09:16:40.000000 w3ml-2024.3.21rc0/w3ml.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      291 2024-03-21 09:16:40.000000 w3ml-2024.3.21rc0/w3ml.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-03-21 09:16:40.000000 w3ml-2024.3.21rc0/w3ml.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-21 09:16:40.000000 w3ml-2024.3.21rc0/w3ml.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      481 2024-03-21 09:16:40.000000 w3ml-2024.3.21rc0/w3ml.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-03-21 09:16:40.000000 w3ml-2024.3.21rc0/w3ml.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      481 2024-03-21 09:16:40.000000 w3ml-2024.3.21rc0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-21 09:16:40.000000 w3ml-2024.3.21rc0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 09:16:40.000000 w3ml-2024.3.21rc0/w3ml/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 09:16:40.000000 w3ml-2024.3.21rc0/w3ml/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-03-21 09:16:30.000000 w3ml-2024.3.21rc0/w3ml/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 09:16:40.000000 w3ml-2024.3.21rc0/w3ml/models/
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-03-21 09:16:30.000000 w3ml-2024.3.21rc0/w3ml/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 09:16:40.000000 w3ml-2024.3.21rc0/w3ml/models/contrib/
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-03-21 09:16:30.000000 w3ml-2024.3.21rc0/w3ml/models/contrib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7444 2024-03-21 09:16:30.000000 w3ml-2024.3.21rc0/w3ml/models/contrib/automl.py
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-03-21 09:16:30.000000 w3ml-2024.3.21rc0/w3ml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-03-21 09:16:30.000000 w3ml-2024.3.21rc0/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-03-21 09:16:30.000000 w3ml-2024.3.21rc0/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 02:41:17.000000 w3ml-2024.5.16rc1/
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-05-16 02:41:17.000000 w3ml-2024.5.16rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-05-16 02:41:08.000000 w3ml-2024.5.16rc1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 02:41:17.000000 w3ml-2024.5.16rc1/w3ml/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-16 02:41:08.000000 w3ml-2024.5.16rc1/w3ml/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 02:41:17.000000 w3ml-2024.5.16rc1/w3ml/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-16 02:41:08.000000 w3ml-2024.5.16rc1/w3ml/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 02:41:17.000000 w3ml-2024.5.16rc1/w3ml/models/
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-16 02:41:08.000000 w3ml-2024.5.16rc1/w3ml/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 02:41:17.000000 w3ml-2024.5.16rc1/w3ml/models/contrib/
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2024-05-16 02:41:08.000000 w3ml-2024.5.16rc1/w3ml/models/contrib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6220 2024-05-16 02:41:08.000000 w3ml-2024.5.16rc1/w3ml/models/contrib/automl_multilabel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10188 2024-05-16 02:41:08.000000 w3ml-2024.5.16rc1/w3ml/models/contrib/automl_binary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9527 2024-05-16 02:41:08.000000 w3ml-2024.5.16rc1/w3ml/models/contrib/automl_multiclass.py
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-16 02:41:08.000000 w3ml-2024.5.16rc1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 02:41:17.000000 w3ml-2024.5.16rc1/w3ml.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-05-16 02:41:17.000000 w3ml-2024.5.16rc1/w3ml.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-16 02:41:17.000000 w3ml-2024.5.16rc1/w3ml.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-16 02:41:17.000000 w3ml-2024.5.16rc1/w3ml.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-05-16 02:41:17.000000 w3ml-2024.5.16rc1/w3ml.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 02:41:17.000000 w3ml-2024.5.16rc1/w3ml.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 02:41:17.000000 w3ml-2024.5.16rc1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-05-16 02:41:08.000000 w3ml-2024.5.16rc1/LICENSE
```

### Comparing `w3ml-2024.3.21rc0/setup.py` & `w3ml-2024.5.16rc1/setup.py`

 * *Files identical despite different names*

### Comparing `w3ml-2024.3.21rc0/LICENSE` & `w3ml-2024.5.16rc1/LICENSE`

 * *Files identical despite different names*

