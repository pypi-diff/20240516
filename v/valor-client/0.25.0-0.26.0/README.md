# Comparing `tmp/valor_client-0.25.0.tar.gz` & `tmp/valor_client-0.26.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "valor_client-0.25.0.tar", last modified: Mon May 13 19:10:08 2024, max compression
+gzip compressed data, was "valor_client-0.26.0.tar", last modified: Thu May 16 19:27:17 2024, max compression
```

## Comparing `valor_client-0.25.0.tar` & `valor_client-0.26.0.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:10:08.094879 valor_client-0.25.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-13 19:10:03.000000 valor_client-0.25.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-05-13 19:10:08.094879 valor_client-0.25.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-05-13 19:10:03.000000 valor_client-0.25.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 19:10:08.094879 valor_client-0.25.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-05-13 19:10:03.000000 valor_client-0.25.0/tox.ini
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:10:08.086878 valor_client-0.25.0/unit-tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-05-13 19:10:03.000000 valor_client-0.25.0/unit-tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:10:08.086878 valor_client-0.25.0/unit-tests/coretypes/
--rw-r--r--   0 runner    (1001) docker     (127)     8020 2024-05-13 19:10:03.000000 valor_client-0.25.0/unit-tests/coretypes/test_core.py
--rw-r--r--   0 runner    (1001) docker     (127)     2214 2024-05-13 19:10:03.000000 valor_client-0.25.0/unit-tests/coretypes/test_evaluation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3871 2024-05-13 19:10:03.000000 valor_client-0.25.0/unit-tests/coretypes/test_filtering.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:10:08.086878 valor_client-0.25.0/unit-tests/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)      426 2024-05-13 19:10:03.000000 valor_client-0.25.0/unit-tests/schemas/test_evaluation_schemas.py
--rw-r--r--   0 runner    (1001) docker     (127)     3342 2024-05-13 19:10:03.000000 valor_client-0.25.0/unit-tests/schemas/test_filters.py
--rw-r--r--   0 runner    (1001) docker     (127)     4045 2024-05-13 19:10:03.000000 valor_client-0.25.0/unit-tests/schemas/test_geojson.py
--rw-r--r--   0 runner    (1001) docker     (127)     2746 2024-05-13 19:10:03.000000 valor_client-0.25.0/unit-tests/schemas/test_label.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:10:08.086878 valor_client-0.25.0/unit-tests/symbolic/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:10:08.086878 valor_client-0.25.0/unit-tests/symbolic/collections/
--rw-r--r--   0 runner    (1001) docker     (127)     2658 2024-05-13 19:10:03.000000 valor_client-0.25.0/unit-tests/symbolic/collections/test_dictionary.py
--rw-r--r--   0 runner    (1001) docker     (127)     3694 2024-05-13 19:10:03.000000 valor_client-0.25.0/unit-tests/symbolic/collections/test_static_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)    12927 2024-05-13 19:10:03.000000 valor_client-0.25.0/unit-tests/symbolic/collections/test_structures.py
--rw-r--r--   0 runner    (1001) docker     (127)     5707 2024-05-13 19:10:03.000000 valor_client-0.25.0/unit-tests/symbolic/test_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:10:08.086878 valor_client-0.25.0/unit-tests/symbolic/types/
--rw-r--r--   0 runner    (1001) docker     (127)    13912 2024-05-13 19:10:03.000000 valor_client-0.25.0/unit-tests/symbolic/types/test_schemas.py
--rw-r--r--   0 runner    (1001) docker     (127)    38078 2024-05-13 19:10:03.000000 valor_client-0.25.0/unit-tests/symbolic/types/test_symbolic_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     2001 2024-05-13 19:10:03.000000 valor_client-0.25.0/unit-tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      465 2024-05-13 19:10:03.000000 valor_client-0.25.0/unit-tests/test_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     3791 2024-05-13 19:10:03.000000 valor_client-0.25.0/unit-tests/test_typing.py
--rw-r--r--   0 runner    (1001) docker     (127)     5639 2024-05-13 19:10:03.000000 valor_client-0.25.0/unit-tests/test_viz.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:10:08.090878 valor_client-0.25.0/valor/
--rw-r--r--   0 runner    (1001) docker     (127)      706 2024-05-13 19:10:03.000000 valor_client-0.25.0/valor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    29488 2024-05-13 19:10:03.000000 valor_client-0.25.0/valor/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    54799 2024-05-13 19:10:03.000000 valor_client-0.25.0/valor/coretypes.py
--rw-r--r--   0 runner    (1001) docker     (127)      661 2024-05-13 19:10:03.000000 valor_client-0.25.0/valor/enums.py
--rw-r--r--   0 runner    (1001) docker     (127)     3384 2024-05-13 19:10:03.000000 valor_client-0.25.0/valor/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     5599 2024-05-13 19:10:03.000000 valor_client-0.25.0/valor/metatypes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:10:08.090878 valor_client-0.25.0/valor/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-05-13 19:10:03.000000 valor_client-0.25.0/valor/schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2803 2024-05-13 19:10:03.000000 valor_client-0.25.0/valor/schemas/evaluation.py
--rw-r--r--   0 runner    (1001) docker     (127)    14601 2024-05-13 19:10:03.000000 valor_client-0.25.0/valor/schemas/filters.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:10:08.090878 valor_client-0.25.0/valor/schemas/symbolic/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 19:10:03.000000 valor_client-0.25.0/valor/schemas/symbolic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12908 2024-05-13 19:10:03.000000 valor_client-0.25.0/valor/schemas/symbolic/collections.py
--rw-r--r--   0 runner    (1001) docker     (127)     5099 2024-05-13 19:10:03.000000 valor_client-0.25.0/valor/schemas/symbolic/operators.py
--rw-r--r--   0 runner    (1001) docker     (127)    59078 2024-05-13 19:10:03.000000 valor_client-0.25.0/valor/schemas/symbolic/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-05-13 19:10:03.000000 valor_client-0.25.0/valor/type_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)    10702 2024-05-13 19:10:03.000000 valor_client-0.25.0/valor/viz.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:10:08.090878 valor_client-0.25.0/valor_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-05-13 19:10:08.000000 valor_client-0.25.0/valor_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-05-13 19:10:08.000000 valor_client-0.25.0/valor_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 19:10:08.000000 valor_client-0.25.0/valor_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-13 19:10:08.000000 valor_client-0.25.0/valor_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-13 19:10:08.000000 valor_client-0.25.0/valor_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:27:17.750795 valor_client-0.26.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-16 19:27:13.000000 valor_client-0.26.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-05-16 19:27:17.750795 valor_client-0.26.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-05-16 19:27:13.000000 valor_client-0.26.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 19:27:17.750795 valor_client-0.26.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-05-16 19:27:13.000000 valor_client-0.26.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:27:17.742796 valor_client-0.26.0/unit-tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-05-16 19:27:13.000000 valor_client-0.26.0/unit-tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:27:17.742796 valor_client-0.26.0/unit-tests/coretypes/
+-rw-r--r--   0 runner    (1001) docker     (127)     8020 2024-05-16 19:27:13.000000 valor_client-0.26.0/unit-tests/coretypes/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2214 2024-05-16 19:27:13.000000 valor_client-0.26.0/unit-tests/coretypes/test_evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3871 2024-05-16 19:27:13.000000 valor_client-0.26.0/unit-tests/coretypes/test_filtering.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:27:17.746796 valor_client-0.26.0/unit-tests/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2024-05-16 19:27:13.000000 valor_client-0.26.0/unit-tests/schemas/test_evaluation_schemas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3342 2024-05-16 19:27:13.000000 valor_client-0.26.0/unit-tests/schemas/test_filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4045 2024-05-16 19:27:13.000000 valor_client-0.26.0/unit-tests/schemas/test_geojson.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2746 2024-05-16 19:27:13.000000 valor_client-0.26.0/unit-tests/schemas/test_label.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:27:17.746796 valor_client-0.26.0/unit-tests/symbolic/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:27:17.746796 valor_client-0.26.0/unit-tests/symbolic/collections/
+-rw-r--r--   0 runner    (1001) docker     (127)     2658 2024-05-16 19:27:13.000000 valor_client-0.26.0/unit-tests/symbolic/collections/test_dictionary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3694 2024-05-16 19:27:13.000000 valor_client-0.26.0/unit-tests/symbolic/collections/test_static_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12927 2024-05-16 19:27:13.000000 valor_client-0.26.0/unit-tests/symbolic/collections/test_structures.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5707 2024-05-16 19:27:13.000000 valor_client-0.26.0/unit-tests/symbolic/test_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:27:17.746796 valor_client-0.26.0/unit-tests/symbolic/types/
+-rw-r--r--   0 runner    (1001) docker     (127)    13912 2024-05-16 19:27:13.000000 valor_client-0.26.0/unit-tests/symbolic/types/test_schemas.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38078 2024-05-16 19:27:13.000000 valor_client-0.26.0/unit-tests/symbolic/types/test_symbolic_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1320 2024-05-16 19:27:13.000000 valor_client-0.26.0/unit-tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2024-05-16 19:27:13.000000 valor_client-0.26.0/unit-tests/test_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3791 2024-05-16 19:27:13.000000 valor_client-0.26.0/unit-tests/test_typing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5639 2024-05-16 19:27:13.000000 valor_client-0.26.0/unit-tests/test_viz.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:27:17.746796 valor_client-0.26.0/valor/
+-rw-r--r--   0 runner    (1001) docker     (127)      706 2024-05-16 19:27:13.000000 valor_client-0.26.0/valor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27176 2024-05-16 19:27:13.000000 valor_client-0.26.0/valor/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    55477 2024-05-16 19:27:13.000000 valor_client-0.26.0/valor/coretypes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      661 2024-05-16 19:27:13.000000 valor_client-0.26.0/valor/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3542 2024-05-16 19:27:13.000000 valor_client-0.26.0/valor/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5599 2024-05-16 19:27:13.000000 valor_client-0.26.0/valor/metatypes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:27:17.746796 valor_client-0.26.0/valor/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-05-16 19:27:13.000000 valor_client-0.26.0/valor/schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2803 2024-05-16 19:27:13.000000 valor_client-0.26.0/valor/schemas/evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14601 2024-05-16 19:27:13.000000 valor_client-0.26.0/valor/schemas/filters.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:27:17.746796 valor_client-0.26.0/valor/schemas/symbolic/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 19:27:13.000000 valor_client-0.26.0/valor/schemas/symbolic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12908 2024-05-16 19:27:13.000000 valor_client-0.26.0/valor/schemas/symbolic/collections.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5099 2024-05-16 19:27:13.000000 valor_client-0.26.0/valor/schemas/symbolic/operators.py
+-rw-r--r--   0 runner    (1001) docker     (127)    59078 2024-05-16 19:27:13.000000 valor_client-0.26.0/valor/schemas/symbolic/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-05-16 19:27:13.000000 valor_client-0.26.0/valor/type_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10702 2024-05-16 19:27:13.000000 valor_client-0.26.0/valor/viz.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:27:17.750795 valor_client-0.26.0/valor_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-05-16 19:27:17.000000 valor_client-0.26.0/valor_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-05-16 19:27:17.000000 valor_client-0.26.0/valor_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 19:27:17.000000 valor_client-0.26.0/valor_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-16 19:27:17.000000 valor_client-0.26.0/valor_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-16 19:27:17.000000 valor_client-0.26.0/valor_client.egg-info/top_level.txt
```

### Comparing `valor_client-0.25.0/LICENSE` & `valor_client-0.26.0/LICENSE`

 * *Files identical despite different names*

### Comparing `valor_client-0.25.0/PKG-INFO` & `valor_client-0.26.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: valor-client
-Version: 0.25.0
+Version: 0.26.0
 Summary: Python client for the Valor evaluation store
 License: MIT License
         
         Copyright (c) 2023 Striveworks
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `valor_client-0.25.0/pyproject.toml` & `valor_client-0.26.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `valor_client-0.25.0/unit-tests/conftest.py` & `valor_client-0.26.0/unit-tests/conftest.py`

 * *Files identical despite different names*

### Comparing `valor_client-0.25.0/unit-tests/coretypes/test_core.py` & `valor_client-0.26.0/unit-tests/coretypes/test_core.py`

 * *Files identical despite different names*

### Comparing `valor_client-0.25.0/unit-tests/coretypes/test_evaluation.py` & `valor_client-0.26.0/unit-tests/coretypes/test_evaluation.py`

 * *Files identical despite different names*

### Comparing `valor_client-0.25.0/unit-tests/coretypes/test_filtering.py` & `valor_client-0.26.0/unit-tests/coretypes/test_filtering.py`

 * *Files identical despite different names*

### Comparing `valor_client-0.25.0/unit-tests/schemas/test_filters.py` & `valor_client-0.26.0/unit-tests/schemas/test_filters.py`

 * *Files identical despite different names*

### Comparing `valor_client-0.25.0/unit-tests/schemas/test_geojson.py` & `valor_client-0.26.0/unit-tests/schemas/test_geojson.py`

 * *Files identical despite different names*

### Comparing `valor_client-0.25.0/unit-tests/schemas/test_label.py` & `valor_client-0.26.0/unit-tests/schemas/test_label.py`

 * *Files identical despite different names*

### Comparing `valor_client-0.25.0/unit-tests/symbolic/collections/test_dictionary.py` & `valor_client-0.26.0/unit-tests/symbolic/collections/test_dictionary.py`

 * *Files identical despite different names*

### Comparing `valor_client-0.25.0/unit-tests/symbolic/collections/test_static_collection.py` & `valor_client-0.26.0/unit-tests/symbolic/collections/test_static_collection.py`

 * *Files identical despite different names*

### Comparing `valor_client-0.25.0/unit-tests/symbolic/collections/test_structures.py` & `valor_client-0.26.0/unit-tests/symbolic/collections/test_structures.py`

 * *Files identical despite different names*

### Comparing `valor_client-0.25.0/unit-tests/symbolic/test_operators.py` & `valor_client-0.26.0/unit-tests/symbolic/test_operators.py`

 * *Files identical despite different names*

### Comparing `valor_client-0.25.0/unit-tests/symbolic/types/test_schemas.py` & `valor_client-0.26.0/unit-tests/symbolic/types/test_schemas.py`

 * *Files identical despite different names*

### Comparing `valor_client-0.25.0/unit-tests/symbolic/types/test_symbolic_types.py` & `valor_client-0.26.0/unit-tests/symbolic/types/test_symbolic_types.py`

 * *Files identical despite different names*

### Comparing `valor_client-0.25.0/unit-tests/test_typing.py` & `valor_client-0.26.0/unit-tests/test_typing.py`

 * *Files identical despite different names*

### Comparing `valor_client-0.25.0/unit-tests/test_viz.py` & `valor_client-0.26.0/unit-tests/test_viz.py`

 * *Files identical despite different names*

### Comparing `valor_client-0.25.0/valor/__init__.py` & `valor_client-0.26.0/valor/__init__.py`

 * *Files identical despite different names*

### Comparing `valor_client-0.25.0/valor/client.py` & `valor_client-0.26.0/valor/client.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import json
 import logging
-import math
 import os
 import time
 from dataclasses import asdict, dataclass
 from typing import Callable, Dict, List, Optional, TypeVar, Union
 from urllib.parse import urlencode, urljoin
 
 import requests
@@ -87,74 +86,14 @@
     return len(
         json.dumps(json_obj, ensure_ascii=False).encode(
             encoding
         )  # this outputs bytes
     )
 
 
-def _chunk_list(
-    json_list: list, chunk_size_bytes: int, encoding: str = "utf-8"
-) -> List[list]:
-    """
-    Chunks a list into smaller lists.
-
-    Parameters
-    ----------
-    json_list : list
-        A list of JSON-compatible objects.
-    chunk_size_bytes : int
-        The maximum number of bytes that a multi-element array can use.
-    encoding : str, default='utf-8'
-        The method used to encode the string object into a bytes format.
-
-    Returns
-    -------
-    List[list]
-        A list of lists containing JSON-compatible objects.
-    """
-    # edge case
-    if len(json_list) == 1:
-        if get_json_size(json_list, encoding) > chunk_size_bytes:
-            logging.warning(
-                f"Attempting to POST an object that is larger than {chunk_size_bytes} bytes."
-            )
-        return [json_list]
-
-    n_elements = len(json_list)
-    avg_element_size = get_json_size(json_list) / n_elements
-    n_elements_per_chunk = int(chunk_size_bytes / avg_element_size)
-
-    # return a list of individual elements if n_elements_per_chunk is zero
-    if n_elements_per_chunk == 0:
-        return [[element] for element in json_list]
-
-    n_chunks = math.ceil(n_elements / n_elements_per_chunk)
-
-    chunks = []
-    for i in range(n_chunks):
-        lhi = i * n_elements_per_chunk
-        rhi = (i + 1) * n_elements_per_chunk
-        new_chunk_size = get_json_size(
-            json_obj=json_list[lhi:rhi], encoding=encoding
-        )
-        if (
-            new_chunk_size > chunk_size_bytes
-        ):  # Recursively chunk if still too large.
-            chunks.extend(
-                _chunk_list(
-                    json_list=json_list[lhi:rhi],
-                    chunk_size_bytes=chunk_size_bytes,
-                    encoding=encoding,
-                )
-            )
-        else:
-            chunks.append(json_list[lhi:rhi])
-    return chunks
-
-
 @dataclass
 class ClientConnection:
     """
     Valor client object for interacting with the api.
 
     Parameters
     ----------
@@ -339,39 +278,35 @@
         Helper for handling DELETE requests.
         """
         return self._requests_wrapper(
             method_name="delete", endpoint=endpoint, *args, **kwargs
         )
 
     def create_groundtruths(
-        self,
-        groundtruths: List[dict],
-        chunk_size_bytes: int = int(1e7),
+        self, groundtruths: List[dict], ignore_existing_datums: bool = False
     ) -> None:
         """
         Creates ground truths.
 
         `CREATE` endpoint.
 
         Parameters
         ----------
         groundtruths : List[dict]
             The ground truths to be created.
-        chunk_size_bytes : int, default=1e7
-            Maximum size of a POST'ed json in bytes. Defaults to 10MB.
-        """
-        chunked_groundtruths = _chunk_list(
-            json_list=groundtruths,
-            chunk_size_bytes=chunk_size_bytes,
+        ignore_existing_datums : bool, default=False
+            If True, will ignore datums that already exist in the backend.
+            If False, will raise an error if any datums already exist.
+            Default is False.
+        """
+        self._requests_post_rel_host(
+            "groundtruths",
+            json=groundtruths,
+            params={"ignore_existing_datums": ignore_existing_datums},
         )
-        for chunk in chunked_groundtruths:
-            self._requests_post_rel_host(
-                "groundtruths",
-                json=chunk,
-            )
 
     def get_groundtruth(
         self,
         dataset_name: str,
         datum_uid: str,
     ) -> dict:
         """
@@ -391,40 +326,26 @@
         dict
             The requested ground truth.
         """
         return self._requests_get_rel_host(
             f"groundtruths/dataset/{dataset_name}/datum/{datum_uid}"
         ).json()
 
-    def create_predictions(
-        self,
-        predictions: List[dict],
-        chunk_size_bytes: int = int(1e7),
-    ) -> None:
+    def create_predictions(self, predictions: List[dict]) -> None:
         """
         Creates predictions.
 
         `CREATE` endpoint.
 
         Parameters
         ----------
         predictions : List[dict]
             The predictions to be created.
-        chunk_size_bytes : int, default=1e7
-            Maximum size of a POST'ed json in bytes. Defaults to 10MB.
         """
-        chunked_predictions = _chunk_list(
-            json_list=predictions,
-            chunk_size_bytes=chunk_size_bytes,
-        )
-        for chunk in chunked_predictions:
-            self._requests_post_rel_host(
-                "predictions",
-                json=chunk,
-            )
+        self._requests_post_rel_host("predictions", json=predictions)
 
     def get_prediction(
         self,
         dataset_name: str,
         model_name: str,
         datum_uid: str,
     ) -> dict:
```

### Comparing `valor_client-0.25.0/valor/coretypes.py` & `valor_client-0.26.0/valor/coretypes.py`

 * *Files 1% similar despite different names*

```diff
@@ -514,26 +514,32 @@
             dataset=self,
             groundtruths=[groundtruth],
         )
 
     def add_groundtruths(
         self,
         groundtruths: List[GroundTruth],
+        ignore_existing_datums: bool = False,
     ) -> None:
         """
         Add multiple ground truths to the dataset.
 
         Parameters
         ----------
         groundtruths : List[GroundTruth]
             The ground truths to create.
+        ignore_existing_datums : bool, default=False
+            If True, will ignore datums that already exist in the backend.
+            If False, will raise an error if any datums already exist.
+            Default is False.
         """
         Client(self.conn).create_groundtruths(
             dataset=self,
             groundtruths=groundtruths,
+            ignore_existing_datums=ignore_existing_datums,
         )
 
     def get_groundtruth(
         self,
         datum: Union[Datum, str],
     ) -> Union[GroundTruth, None]:
         """
@@ -1242,38 +1248,45 @@
             dataset = dataset.encode_value()
         self.conn.create_dataset(dataset)
 
     def create_groundtruths(
         self,
         dataset: Dataset,
         groundtruths: List[GroundTruth],
+        ignore_existing_datums: bool = False,
     ):
         """
         Creates ground truths.
 
         Parameters
         ----------
 
         dataset : valor.Dataset
             The dataset to create the ground truth for.
         groundtruths : List[valor.GroundTruth]
             The ground truths to create.
+        ignore_existing_datums : bool, default=False
+            If True, will ignore datums that already exist in the backend.
+            If False, will raise an error if any datums already exist.
+            Default is False.
         """
         groundtruths_json = []
         for groundtruth in groundtruths:
             if not isinstance(groundtruth, GroundTruth):
                 raise TypeError(
                     f"Expected ground truth to be of type 'valor.GroundTruth' not '{type(groundtruth)}'."
                 )
             if not isinstance(groundtruth.annotations._value, list):
                 raise TypeError
             groundtruth_dict = groundtruth.encode_value()
             groundtruth_dict["dataset_name"] = dataset.name
             groundtruths_json.append(groundtruth_dict)
-        self.conn.create_groundtruths(groundtruths_json)
+        self.conn.create_groundtruths(
+            groundtruths_json, ignore_existing_datums=ignore_existing_datums
+        )
 
     def get_groundtruth(
         self,
         dataset: Union[Dataset, str],
         datum: Union[Datum, str],
     ) -> Union[GroundTruth, None]:
         """
```

### Comparing `valor_client-0.25.0/valor/enums.py` & `valor_client-0.26.0/valor/enums.py`

 * *Files identical despite different names*

### Comparing `valor_client-0.25.0/valor/exceptions.py` & `valor_client-0.26.0/valor/exceptions.py`

 * *Files 5% similar despite different names*

```diff
@@ -110,14 +110,23 @@
     Raises an exception if the user tries to create a datum that already exists.
 
     """
 
     pass
 
 
+class DatumsAlreadyExistError(ClientException):
+    """
+    Raises an exception if the user tries to create a datum that already exists.
+
+    """
+
+    pass
+
+
 class AnnotationAlreadyExistsError(ClientException):
     """
     Raises an exception if the user tries to create a annotation for a datum that already has annotation(s).
     """
 
     pass
```

### Comparing `valor_client-0.25.0/valor/metatypes.py` & `valor_client-0.26.0/valor/metatypes.py`

 * *Files identical despite different names*

### Comparing `valor_client-0.25.0/valor/schemas/__init__.py` & `valor_client-0.26.0/valor/schemas/__init__.py`

 * *Files identical despite different names*

### Comparing `valor_client-0.25.0/valor/schemas/evaluation.py` & `valor_client-0.26.0/valor/schemas/evaluation.py`

 * *Files identical despite different names*

### Comparing `valor_client-0.25.0/valor/schemas/filters.py` & `valor_client-0.26.0/valor/schemas/filters.py`

 * *Files identical despite different names*

### Comparing `valor_client-0.25.0/valor/schemas/symbolic/collections.py` & `valor_client-0.26.0/valor/schemas/symbolic/collections.py`

 * *Files identical despite different names*

### Comparing `valor_client-0.25.0/valor/schemas/symbolic/operators.py` & `valor_client-0.26.0/valor/schemas/symbolic/operators.py`

 * *Files identical despite different names*

### Comparing `valor_client-0.25.0/valor/schemas/symbolic/types.py` & `valor_client-0.26.0/valor/schemas/symbolic/types.py`

 * *Files identical despite different names*

### Comparing `valor_client-0.25.0/valor/type_checks.py` & `valor_client-0.26.0/valor/type_checks.py`

 * *Files identical despite different names*

### Comparing `valor_client-0.25.0/valor/viz.py` & `valor_client-0.26.0/valor/viz.py`

 * *Files identical despite different names*

### Comparing `valor_client-0.25.0/valor_client.egg-info/PKG-INFO` & `valor_client-0.26.0/valor_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: valor-client
-Version: 0.25.0
+Version: 0.26.0
 Summary: Python client for the Valor evaluation store
 License: MIT License
         
         Copyright (c) 2023 Striveworks
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `valor_client-0.25.0/valor_client.egg-info/SOURCES.txt` & `valor_client-0.26.0/valor_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

