# Comparing `tmp/mapel-marriages-2.1.8.tar.gz` & `tmp/mapel_marriages-2.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mapel-marriages-2.1.8.tar", last modified: Sat Mar 23 13:42:19 2024, max compression
+gzip compressed data, was "mapel_marriages-2.1.9.tar", last modified: Mon Apr 15 08:50:22 2024, max compression
```

## Comparing `mapel-marriages-2.1.8.tar` & `mapel_marriages-2.1.9.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 13:42:19.969414 mapel-marriages-2.1.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-03-23 13:42:07.000000 mapel-marriages-2.1.8/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2519 2024-03-23 13:42:19.969414 mapel-marriages-2.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      826 2024-03-23 13:42:07.000000 mapel-marriages-2.1.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      665 2024-03-23 13:42:07.000000 mapel-marriages-2.1.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-03-23 13:42:07.000000 mapel-marriages-2.1.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-23 13:42:19.969414 mapel-marriages-2.1.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 13:42:19.961413 mapel-marriages-2.1.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 13:42:19.961413 mapel-marriages-2.1.8/src/mapel/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 13:42:19.965413 mapel-marriages-2.1.8/src/mapel/marriages/
--rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-03-23 13:42:07.000000 mapel-marriages-2.1.8/src/mapel/marriages/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 13:42:19.965413 mapel-marriages-2.1.8/src/mapel/marriages/cultures/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-23 13:42:07.000000 mapel-marriages-2.1.8/src/mapel/marriages/cultures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      341 2024-03-23 13:42:07.000000 mapel-marriages-2.1.8/src/mapel/marriages/cultures/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    17187 2024-03-23 13:42:07.000000 mapel-marriages-2.1.8/src/mapel/marriages/cultures/euclidean.py
--rw-r--r--   0 runner    (1001) docker     (127)     2409 2024-03-23 13:42:07.000000 mapel-marriages-2.1.8/src/mapel/marriages/cultures/impartial.py
--rw-r--r--   0 runner    (1001) docker     (127)     1355 2024-03-23 13:42:07.000000 mapel-marriages-2.1.8/src/mapel/marriages/cultures/mallows.py
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-03-23 13:42:07.000000 mapel-marriages-2.1.8/src/mapel/marriages/cultures/urn.py
--rw-r--r--   0 runner    (1001) docker     (127)     1854 2024-03-23 13:42:07.000000 mapel-marriages-2.1.8/src/mapel/marriages/cultures_.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 13:42:19.965413 mapel-marriages-2.1.8/src/mapel/marriages/distances/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-23 13:42:07.000000 mapel-marriages-2.1.8/src/mapel/marriages/distances/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4475 2024-03-23 13:42:07.000000 mapel-marriages-2.1.8/src/mapel/marriages/distances/main_marriages_distances.py
--rw-r--r--   0 runner    (1001) docker     (127)     4943 2024-03-23 13:42:07.000000 mapel-marriages-2.1.8/src/mapel/marriages/distances_.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 13:42:19.965413 mapel-marriages-2.1.8/src/mapel/marriages/features/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-23 13:42:07.000000 mapel-marriages-2.1.8/src/mapel/marriages/features/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9347 2024-03-23 13:42:07.000000 mapel-marriages-2.1.8/src/mapel/marriages/features/basic_features.py
--rw-r--r--   0 runner    (1001) docker     (127)     4873 2024-03-23 13:42:07.000000 mapel-marriages-2.1.8/src/mapel/marriages/features/distance_to_stability_features.py
--rw-r--r--   0 runner    (1001) docker     (127)     6678 2024-03-23 13:42:07.000000 mapel-marriages-2.1.8/src/mapel/marriages/features/experiments_marriage.py
--rw-r--r--   0 runner    (1001) docker     (127)      582 2024-03-23 13:42:07.000000 mapel-marriages-2.1.8/src/mapel/marriages/features_.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 13:42:19.965413 mapel-marriages-2.1.8/src/mapel/marriages/objects/
--rw-r--r--   0 runner    (1001) docker     (127)     4278 2024-03-23 13:42:07.000000 mapel-marriages-2.1.8/src/mapel/marriages/objects/Marriages.py
--rw-r--r--   0 runner    (1001) docker     (127)    15466 2024-03-23 13:42:07.000000 mapel-marriages-2.1.8/src/mapel/marriages/objects/MarriagesExperiment.py
--rw-r--r--   0 runner    (1001) docker     (127)     3168 2024-03-23 13:42:07.000000 mapel-marriages-2.1.8/src/mapel/marriages/objects/MarriagesFamily.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-23 13:42:07.000000 mapel-marriages-2.1.8/src/mapel/marriages/objects/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 13:42:19.965413 mapel-marriages-2.1.8/src/mapel/marriages/persistence/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-23 13:42:07.000000 mapel-marriages-2.1.8/src/mapel/marriages/persistence/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1518 2024-03-23 13:42:07.000000 mapel-marriages-2.1.8/src/mapel/marriages/persistence/instance_exports.py
--rw-r--r--   0 runner    (1001) docker     (127)     1938 2024-03-23 13:42:07.000000 mapel-marriages-2.1.8/src/mapel/marriages/persistence/instance_imports.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 13:42:19.969414 mapel-marriages-2.1.8/src/mapel_marriages.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2519 2024-03-23 13:42:19.000000 mapel-marriages-2.1.8/src/mapel_marriages.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1270 2024-03-23 13:42:19.000000 mapel-marriages-2.1.8/src/mapel_marriages.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-23 13:42:19.000000 mapel-marriages-2.1.8/src/mapel_marriages.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-03-23 13:42:19.000000 mapel-marriages-2.1.8/src/mapel_marriages.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-03-23 13:42:19.000000 mapel-marriages-2.1.8/src/mapel_marriages.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:50:22.093085 mapel_marriages-2.1.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-04-15 08:50:09.000000 mapel_marriages-2.1.9/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2519 2024-04-15 08:50:22.093085 mapel_marriages-2.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      826 2024-04-15 08:50:09.000000 mapel_marriages-2.1.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      665 2024-04-15 08:50:09.000000 mapel_marriages-2.1.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-15 08:50:09.000000 mapel_marriages-2.1.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 08:50:22.093085 mapel_marriages-2.1.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:50:22.089084 mapel_marriages-2.1.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:50:22.089084 mapel_marriages-2.1.9/src/mapel/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:50:22.089084 mapel_marriages-2.1.9/src/mapel/marriages/
+-rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-04-15 08:50:09.000000 mapel_marriages-2.1.9/src/mapel/marriages/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:50:22.089084 mapel_marriages-2.1.9/src/mapel/marriages/cultures/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 08:50:09.000000 mapel_marriages-2.1.9/src/mapel/marriages/cultures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-04-15 08:50:09.000000 mapel_marriages-2.1.9/src/mapel/marriages/cultures/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17187 2024-04-15 08:50:09.000000 mapel_marriages-2.1.9/src/mapel/marriages/cultures/euclidean.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2409 2024-04-15 08:50:09.000000 mapel_marriages-2.1.9/src/mapel/marriages/cultures/impartial.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1355 2024-04-15 08:50:09.000000 mapel_marriages-2.1.9/src/mapel/marriages/cultures/mallows.py
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-04-15 08:50:09.000000 mapel_marriages-2.1.9/src/mapel/marriages/cultures/urn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1854 2024-04-15 08:50:09.000000 mapel_marriages-2.1.9/src/mapel/marriages/cultures_.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:50:22.093085 mapel_marriages-2.1.9/src/mapel/marriages/distances/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 08:50:09.000000 mapel_marriages-2.1.9/src/mapel/marriages/distances/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4475 2024-04-15 08:50:09.000000 mapel_marriages-2.1.9/src/mapel/marriages/distances/main_marriages_distances.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4943 2024-04-15 08:50:09.000000 mapel_marriages-2.1.9/src/mapel/marriages/distances_.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:50:22.093085 mapel_marriages-2.1.9/src/mapel/marriages/features/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 08:50:09.000000 mapel_marriages-2.1.9/src/mapel/marriages/features/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9347 2024-04-15 08:50:09.000000 mapel_marriages-2.1.9/src/mapel/marriages/features/basic_features.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4873 2024-04-15 08:50:09.000000 mapel_marriages-2.1.9/src/mapel/marriages/features/distance_to_stability_features.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6678 2024-04-15 08:50:09.000000 mapel_marriages-2.1.9/src/mapel/marriages/features/experiments_marriage.py
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-04-15 08:50:09.000000 mapel_marriages-2.1.9/src/mapel/marriages/features_.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:50:22.093085 mapel_marriages-2.1.9/src/mapel/marriages/objects/
+-rw-r--r--   0 runner    (1001) docker     (127)     4278 2024-04-15 08:50:09.000000 mapel_marriages-2.1.9/src/mapel/marriages/objects/Marriages.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15466 2024-04-15 08:50:09.000000 mapel_marriages-2.1.9/src/mapel/marriages/objects/MarriagesExperiment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3168 2024-04-15 08:50:09.000000 mapel_marriages-2.1.9/src/mapel/marriages/objects/MarriagesFamily.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 08:50:09.000000 mapel_marriages-2.1.9/src/mapel/marriages/objects/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:50:22.093085 mapel_marriages-2.1.9/src/mapel/marriages/persistence/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 08:50:09.000000 mapel_marriages-2.1.9/src/mapel/marriages/persistence/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1518 2024-04-15 08:50:09.000000 mapel_marriages-2.1.9/src/mapel/marriages/persistence/instance_exports.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1938 2024-04-15 08:50:09.000000 mapel_marriages-2.1.9/src/mapel/marriages/persistence/instance_imports.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:50:22.093085 mapel_marriages-2.1.9/src/mapel_marriages.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2519 2024-04-15 08:50:22.000000 mapel_marriages-2.1.9/src/mapel_marriages.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1270 2024-04-15 08:50:22.000000 mapel_marriages-2.1.9/src/mapel_marriages.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 08:50:22.000000 mapel_marriages-2.1.9/src/mapel_marriages.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-15 08:50:22.000000 mapel_marriages-2.1.9/src/mapel_marriages.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-15 08:50:22.000000 mapel_marriages-2.1.9/src/mapel_marriages.egg-info/top_level.txt
```

### Comparing `mapel-marriages-2.1.8/LICENSE.txt` & `mapel_marriages-2.1.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mapel-marriages-2.1.8/PKG-INFO` & `mapel_marriages-2.1.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mapel-marriages
-Version: 2.1.8
+Version: 2.1.9
 Summary: Map of Marriages
 Author-email: Stanislaw Szufa <s.szufa@gmail.com>, Niclas Boehmer <niclas.boehmer@tu-berlin.de>
 License: Copyright (c) 2018-2022 Stanislaw Szufa and contributors
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `mapel-marriages-2.1.8/README.md` & `mapel_marriages-2.1.9/README.md`

 * *Files identical despite different names*

### Comparing `mapel-marriages-2.1.8/pyproject.toml` & `mapel_marriages-2.1.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=65", "wheel", "pybind11>=2.6.1"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mapel-marriages"
-version = "2.1.8"
+version = "2.1.9"
 authors = [
  {name = "Stanislaw Szufa", email = "s.szufa@gmail.com"},
  {name = "Niclas Boehmer", email = "niclas.boehmer@tu-berlin.de"},
 ]
 description = "Map of Marriages"
 classifiers=[
     "Programming Language :: Python :: 3",
```

### Comparing `mapel-marriages-2.1.8/src/mapel/marriages/__init__.py` & `mapel_marriages-2.1.9/src/mapel/marriages/__init__.py`

 * *Files identical despite different names*

### Comparing `mapel-marriages-2.1.8/src/mapel/marriages/cultures/euclidean.py` & `mapel_marriages-2.1.9/src/mapel/marriages/cultures/euclidean.py`

 * *Files identical despite different names*

### Comparing `mapel-marriages-2.1.8/src/mapel/marriages/cultures/impartial.py` & `mapel_marriages-2.1.9/src/mapel/marriages/cultures/impartial.py`

 * *Files identical despite different names*

### Comparing `mapel-marriages-2.1.8/src/mapel/marriages/cultures/mallows.py` & `mapel_marriages-2.1.9/src/mapel/marriages/cultures/mallows.py`

 * *Files identical despite different names*

### Comparing `mapel-marriages-2.1.8/src/mapel/marriages/cultures/urn.py` & `mapel_marriages-2.1.9/src/mapel/marriages/cultures/urn.py`

 * *Files identical despite different names*

### Comparing `mapel-marriages-2.1.8/src/mapel/marriages/cultures_.py` & `mapel_marriages-2.1.9/src/mapel/marriages/cultures_.py`

 * *Files identical despite different names*

### Comparing `mapel-marriages-2.1.8/src/mapel/marriages/distances/main_marriages_distances.py` & `mapel_marriages-2.1.9/src/mapel/marriages/distances/main_marriages_distances.py`

 * *Files identical despite different names*

### Comparing `mapel-marriages-2.1.8/src/mapel/marriages/distances_.py` & `mapel_marriages-2.1.9/src/mapel/marriages/distances_.py`

 * *Files identical despite different names*

### Comparing `mapel-marriages-2.1.8/src/mapel/marriages/features/basic_features.py` & `mapel_marriages-2.1.9/src/mapel/marriages/features/basic_features.py`

 * *Files identical despite different names*

### Comparing `mapel-marriages-2.1.8/src/mapel/marriages/features/distance_to_stability_features.py` & `mapel_marriages-2.1.9/src/mapel/marriages/features/distance_to_stability_features.py`

 * *Files identical despite different names*

### Comparing `mapel-marriages-2.1.8/src/mapel/marriages/features/experiments_marriage.py` & `mapel_marriages-2.1.9/src/mapel/marriages/features/experiments_marriage.py`

 * *Files identical despite different names*

### Comparing `mapel-marriages-2.1.8/src/mapel/marriages/features_.py` & `mapel_marriages-2.1.9/src/mapel/marriages/features_.py`

 * *Files identical despite different names*

### Comparing `mapel-marriages-2.1.8/src/mapel/marriages/objects/Marriages.py` & `mapel_marriages-2.1.9/src/mapel/marriages/objects/Marriages.py`

 * *Files identical despite different names*

### Comparing `mapel-marriages-2.1.8/src/mapel/marriages/objects/MarriagesExperiment.py` & `mapel_marriages-2.1.9/src/mapel/marriages/objects/MarriagesExperiment.py`

 * *Files identical despite different names*

### Comparing `mapel-marriages-2.1.8/src/mapel/marriages/objects/MarriagesFamily.py` & `mapel_marriages-2.1.9/src/mapel/marriages/objects/MarriagesFamily.py`

 * *Files identical despite different names*

### Comparing `mapel-marriages-2.1.8/src/mapel/marriages/persistence/instance_exports.py` & `mapel_marriages-2.1.9/src/mapel/marriages/persistence/instance_exports.py`

 * *Files identical despite different names*

### Comparing `mapel-marriages-2.1.8/src/mapel/marriages/persistence/instance_imports.py` & `mapel_marriages-2.1.9/src/mapel/marriages/persistence/instance_imports.py`

 * *Files identical despite different names*

### Comparing `mapel-marriages-2.1.8/src/mapel_marriages.egg-info/PKG-INFO` & `mapel_marriages-2.1.9/src/mapel_marriages.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mapel-marriages
-Version: 2.1.8
+Version: 2.1.9
 Summary: Map of Marriages
 Author-email: Stanislaw Szufa <s.szufa@gmail.com>, Niclas Boehmer <niclas.boehmer@tu-berlin.de>
 License: Copyright (c) 2018-2022 Stanislaw Szufa and contributors
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `mapel-marriages-2.1.8/src/mapel_marriages.egg-info/SOURCES.txt` & `mapel_marriages-2.1.9/src/mapel_marriages.egg-info/SOURCES.txt`

 * *Files identical despite different names*

