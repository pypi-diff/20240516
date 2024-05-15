# Comparing `tmp/mapel-roommates-2.1.8.tar.gz` & `tmp/mapel_roommates-2.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mapel-roommates-2.1.8.tar", last modified: Sat Mar 23 13:42:17 2024, max compression
+gzip compressed data, was "mapel_roommates-2.1.9.tar", last modified: Mon Apr 15 08:50:20 2024, max compression
```

## Comparing `mapel-roommates-2.1.8.tar` & `mapel_roommates-2.1.9.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 13:42:17.909392 mapel-roommates-2.1.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-03-23 13:42:07.000000 mapel-roommates-2.1.8/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2520 2024-03-23 13:42:17.905393 mapel-roommates-2.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      827 2024-03-23 13:42:07.000000 mapel-roommates-2.1.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      666 2024-03-23 13:42:07.000000 mapel-roommates-2.1.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-03-23 13:42:07.000000 mapel-roommates-2.1.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-23 13:42:17.909392 mapel-roommates-2.1.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 13:42:17.901393 mapel-roommates-2.1.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 13:42:17.901393 mapel-roommates-2.1.8/src/mapel/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 13:42:17.901393 mapel-roommates-2.1.8/src/mapel/roommates/
--rw-r--r--   0 runner    (1001) docker     (127)     1538 2024-03-23 13:42:07.000000 mapel-roommates-2.1.8/src/mapel/roommates/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 13:42:17.905393 mapel-roommates-2.1.8/src/mapel/roommates/cultures/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-23 13:42:07.000000 mapel-roommates-2.1.8/src/mapel/roommates/cultures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      341 2024-03-23 13:42:07.000000 mapel-roommates-2.1.8/src/mapel/roommates/cultures/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    10974 2024-03-23 13:42:07.000000 mapel-roommates-2.1.8/src/mapel/roommates/cultures/euclidean.py
--rw-r--r--   0 runner    (1001) docker     (127)    18812 2024-03-23 13:42:07.000000 mapel-roommates-2.1.8/src/mapel/roommates/cultures/group_separable.py
--rw-r--r--   0 runner    (1001) docker     (127)     3478 2024-03-23 13:42:07.000000 mapel-roommates-2.1.8/src/mapel/roommates/cultures/impartial.py
--rw-r--r--   0 runner    (1001) docker     (127)     3805 2024-03-23 13:42:07.000000 mapel-roommates-2.1.8/src/mapel/roommates/cultures/mallows.py
--rw-r--r--   0 runner    (1001) docker     (127)      676 2024-03-23 13:42:07.000000 mapel-roommates-2.1.8/src/mapel/roommates/cultures/urn.py
--rw-r--r--   0 runner    (1001) docker     (127)     1695 2024-03-23 13:42:07.000000 mapel-roommates-2.1.8/src/mapel/roommates/cultures_.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 13:42:17.905393 mapel-roommates-2.1.8/src/mapel/roommates/distances/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-23 13:42:07.000000 mapel-roommates-2.1.8/src/mapel/roommates/distances/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3401 2024-03-23 13:42:07.000000 mapel-roommates-2.1.8/src/mapel/roommates/distances/main_distances.py
--rw-r--r--   0 runner    (1001) docker     (127)     3741 2024-03-23 13:42:07.000000 mapel-roommates-2.1.8/src/mapel/roommates/distances_.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 13:42:17.905393 mapel-roommates-2.1.8/src/mapel/roommates/features/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-23 13:42:07.000000 mapel-roommates-2.1.8/src/mapel/roommates/features/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10122 2024-03-23 13:42:07.000000 mapel-roommates-2.1.8/src/mapel/roommates/features/basic_features.py
--rw-r--r--   0 runner    (1001) docker     (127)     4873 2024-03-23 13:42:07.000000 mapel-roommates-2.1.8/src/mapel/roommates/features/distance_to_stability_features.py
--rw-r--r--   0 runner    (1001) docker     (127)     4254 2024-03-23 13:42:07.000000 mapel-roommates-2.1.8/src/mapel/roommates/features_.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 13:42:17.905393 mapel-roommates-2.1.8/src/mapel/roommates/objects/
--rw-r--r--   0 runner    (1001) docker     (127)     4497 2024-03-23 13:42:07.000000 mapel-roommates-2.1.8/src/mapel/roommates/objects/Roommates.py
--rw-r--r--   0 runner    (1001) docker     (127)    18401 2024-03-23 13:42:07.000000 mapel-roommates-2.1.8/src/mapel/roommates/objects/RoommatesExperiment.py
--rw-r--r--   0 runner    (1001) docker     (127)     3140 2024-03-23 13:42:07.000000 mapel-roommates-2.1.8/src/mapel/roommates/objects/RoommatesFamily.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-23 13:42:07.000000 mapel-roommates-2.1.8/src/mapel/roommates/objects/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 13:42:17.905393 mapel-roommates-2.1.8/src/mapel/roommates/persistence/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-23 13:42:07.000000 mapel-roommates-2.1.8/src/mapel/roommates/persistence/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1474 2024-03-23 13:42:07.000000 mapel-roommates-2.1.8/src/mapel/roommates/persistence/instance_exports.py
--rw-r--r--   0 runner    (1001) docker     (127)     1833 2024-03-23 13:42:07.000000 mapel-roommates-2.1.8/src/mapel/roommates/persistence/instance_imports.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 13:42:17.905393 mapel-roommates-2.1.8/src/mapel_roommates.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2520 2024-03-23 13:42:17.000000 mapel-roommates-2.1.8/src/mapel_roommates.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1255 2024-03-23 13:42:17.000000 mapel-roommates-2.1.8/src/mapel_roommates.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-23 13:42:17.000000 mapel-roommates-2.1.8/src/mapel_roommates.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-03-23 13:42:17.000000 mapel-roommates-2.1.8/src/mapel_roommates.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-03-23 13:42:17.000000 mapel-roommates-2.1.8/src/mapel_roommates.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:50:20.117075 mapel_roommates-2.1.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-04-15 08:50:09.000000 mapel_roommates-2.1.9/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2520 2024-04-15 08:50:20.117075 mapel_roommates-2.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      827 2024-04-15 08:50:09.000000 mapel_roommates-2.1.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      666 2024-04-15 08:50:09.000000 mapel_roommates-2.1.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-15 08:50:09.000000 mapel_roommates-2.1.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 08:50:20.117075 mapel_roommates-2.1.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:50:20.109075 mapel_roommates-2.1.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:50:20.109075 mapel_roommates-2.1.9/src/mapel/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:50:20.109075 mapel_roommates-2.1.9/src/mapel/roommates/
+-rw-r--r--   0 runner    (1001) docker     (127)     1538 2024-04-15 08:50:09.000000 mapel_roommates-2.1.9/src/mapel/roommates/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:50:20.113075 mapel_roommates-2.1.9/src/mapel/roommates/cultures/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 08:50:09.000000 mapel_roommates-2.1.9/src/mapel/roommates/cultures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-04-15 08:50:09.000000 mapel_roommates-2.1.9/src/mapel/roommates/cultures/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10974 2024-04-15 08:50:09.000000 mapel_roommates-2.1.9/src/mapel/roommates/cultures/euclidean.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18812 2024-04-15 08:50:09.000000 mapel_roommates-2.1.9/src/mapel/roommates/cultures/group_separable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3478 2024-04-15 08:50:09.000000 mapel_roommates-2.1.9/src/mapel/roommates/cultures/impartial.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3805 2024-04-15 08:50:09.000000 mapel_roommates-2.1.9/src/mapel/roommates/cultures/mallows.py
+-rw-r--r--   0 runner    (1001) docker     (127)      676 2024-04-15 08:50:09.000000 mapel_roommates-2.1.9/src/mapel/roommates/cultures/urn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1695 2024-04-15 08:50:09.000000 mapel_roommates-2.1.9/src/mapel/roommates/cultures_.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:50:20.113075 mapel_roommates-2.1.9/src/mapel/roommates/distances/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 08:50:09.000000 mapel_roommates-2.1.9/src/mapel/roommates/distances/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3401 2024-04-15 08:50:09.000000 mapel_roommates-2.1.9/src/mapel/roommates/distances/main_distances.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3741 2024-04-15 08:50:09.000000 mapel_roommates-2.1.9/src/mapel/roommates/distances_.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:50:20.113075 mapel_roommates-2.1.9/src/mapel/roommates/features/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 08:50:09.000000 mapel_roommates-2.1.9/src/mapel/roommates/features/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10122 2024-04-15 08:50:09.000000 mapel_roommates-2.1.9/src/mapel/roommates/features/basic_features.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4873 2024-04-15 08:50:09.000000 mapel_roommates-2.1.9/src/mapel/roommates/features/distance_to_stability_features.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4254 2024-04-15 08:50:09.000000 mapel_roommates-2.1.9/src/mapel/roommates/features_.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:50:20.113075 mapel_roommates-2.1.9/src/mapel/roommates/objects/
+-rw-r--r--   0 runner    (1001) docker     (127)     4497 2024-04-15 08:50:09.000000 mapel_roommates-2.1.9/src/mapel/roommates/objects/Roommates.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18401 2024-04-15 08:50:09.000000 mapel_roommates-2.1.9/src/mapel/roommates/objects/RoommatesExperiment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3140 2024-04-15 08:50:09.000000 mapel_roommates-2.1.9/src/mapel/roommates/objects/RoommatesFamily.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 08:50:09.000000 mapel_roommates-2.1.9/src/mapel/roommates/objects/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:50:20.113075 mapel_roommates-2.1.9/src/mapel/roommates/persistence/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 08:50:09.000000 mapel_roommates-2.1.9/src/mapel/roommates/persistence/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1474 2024-04-15 08:50:09.000000 mapel_roommates-2.1.9/src/mapel/roommates/persistence/instance_exports.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1833 2024-04-15 08:50:09.000000 mapel_roommates-2.1.9/src/mapel/roommates/persistence/instance_imports.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:50:20.117075 mapel_roommates-2.1.9/src/mapel_roommates.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2520 2024-04-15 08:50:20.000000 mapel_roommates-2.1.9/src/mapel_roommates.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1255 2024-04-15 08:50:20.000000 mapel_roommates-2.1.9/src/mapel_roommates.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 08:50:20.000000 mapel_roommates-2.1.9/src/mapel_roommates.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-15 08:50:20.000000 mapel_roommates-2.1.9/src/mapel_roommates.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-15 08:50:20.000000 mapel_roommates-2.1.9/src/mapel_roommates.egg-info/top_level.txt
```

### Comparing `mapel-roommates-2.1.8/LICENSE.txt` & `mapel_roommates-2.1.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mapel-roommates-2.1.8/PKG-INFO` & `mapel_roommates-2.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mapel-roommates
-Version: 2.1.8
+Version: 2.1.9
 Summary: Map of Roommates
 Author-email: Stanislaw Szufa <s.szufa@gmail.com>, Niclas Boehmer <niclas.boehmer@tu-berlin.de>
 License: Copyright (c) 2018-2022 Stanislaw Szufa and contributors
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `mapel-roommates-2.1.8/README.md` & `mapel_roommates-2.1.9/README.md`

 * *Files identical despite different names*

### Comparing `mapel-roommates-2.1.8/src/mapel/roommates/__init__.py` & `mapel_roommates-2.1.9/src/mapel/roommates/__init__.py`

 * *Files identical despite different names*

### Comparing `mapel-roommates-2.1.8/src/mapel/roommates/cultures/euclidean.py` & `mapel_roommates-2.1.9/src/mapel/roommates/cultures/euclidean.py`

 * *Files identical despite different names*

### Comparing `mapel-roommates-2.1.8/src/mapel/roommates/cultures/group_separable.py` & `mapel_roommates-2.1.9/src/mapel/roommates/cultures/group_separable.py`

 * *Files identical despite different names*

### Comparing `mapel-roommates-2.1.8/src/mapel/roommates/cultures/impartial.py` & `mapel_roommates-2.1.9/src/mapel/roommates/cultures/impartial.py`

 * *Files identical despite different names*

### Comparing `mapel-roommates-2.1.8/src/mapel/roommates/cultures/mallows.py` & `mapel_roommates-2.1.9/src/mapel/roommates/cultures/mallows.py`

 * *Files identical despite different names*

### Comparing `mapel-roommates-2.1.8/src/mapel/roommates/cultures/urn.py` & `mapel_roommates-2.1.9/src/mapel/roommates/cultures/urn.py`

 * *Files identical despite different names*

### Comparing `mapel-roommates-2.1.8/src/mapel/roommates/cultures_.py` & `mapel_roommates-2.1.9/src/mapel/roommates/cultures_.py`

 * *Files identical despite different names*

### Comparing `mapel-roommates-2.1.8/src/mapel/roommates/distances/main_distances.py` & `mapel_roommates-2.1.9/src/mapel/roommates/distances/main_distances.py`

 * *Files identical despite different names*

### Comparing `mapel-roommates-2.1.8/src/mapel/roommates/distances_.py` & `mapel_roommates-2.1.9/src/mapel/roommates/distances_.py`

 * *Files identical despite different names*

### Comparing `mapel-roommates-2.1.8/src/mapel/roommates/features/basic_features.py` & `mapel_roommates-2.1.9/src/mapel/roommates/features/basic_features.py`

 * *Files identical despite different names*

### Comparing `mapel-roommates-2.1.8/src/mapel/roommates/features/distance_to_stability_features.py` & `mapel_roommates-2.1.9/src/mapel/roommates/features/distance_to_stability_features.py`

 * *Files identical despite different names*

### Comparing `mapel-roommates-2.1.8/src/mapel/roommates/features_.py` & `mapel_roommates-2.1.9/src/mapel/roommates/features_.py`

 * *Files identical despite different names*

### Comparing `mapel-roommates-2.1.8/src/mapel/roommates/objects/Roommates.py` & `mapel_roommates-2.1.9/src/mapel/roommates/objects/Roommates.py`

 * *Files identical despite different names*

### Comparing `mapel-roommates-2.1.8/src/mapel/roommates/objects/RoommatesExperiment.py` & `mapel_roommates-2.1.9/src/mapel/roommates/objects/RoommatesExperiment.py`

 * *Files identical despite different names*

### Comparing `mapel-roommates-2.1.8/src/mapel/roommates/objects/RoommatesFamily.py` & `mapel_roommates-2.1.9/src/mapel/roommates/objects/RoommatesFamily.py`

 * *Files identical despite different names*

### Comparing `mapel-roommates-2.1.8/src/mapel/roommates/persistence/instance_exports.py` & `mapel_roommates-2.1.9/src/mapel/roommates/persistence/instance_exports.py`

 * *Files identical despite different names*

### Comparing `mapel-roommates-2.1.8/src/mapel/roommates/persistence/instance_imports.py` & `mapel_roommates-2.1.9/src/mapel/roommates/persistence/instance_imports.py`

 * *Files identical despite different names*

### Comparing `mapel-roommates-2.1.8/src/mapel_roommates.egg-info/PKG-INFO` & `mapel_roommates-2.1.9/src/mapel_roommates.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mapel-roommates
-Version: 2.1.8
+Version: 2.1.9
 Summary: Map of Roommates
 Author-email: Stanislaw Szufa <s.szufa@gmail.com>, Niclas Boehmer <niclas.boehmer@tu-berlin.de>
 License: Copyright (c) 2018-2022 Stanislaw Szufa and contributors
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `mapel-roommates-2.1.8/src/mapel_roommates.egg-info/SOURCES.txt` & `mapel_roommates-2.1.9/src/mapel_roommates.egg-info/SOURCES.txt`

 * *Files identical despite different names*

