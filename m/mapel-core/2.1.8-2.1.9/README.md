# Comparing `tmp/mapel-core-2.1.8.tar.gz` & `tmp/mapel_core-2.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mapel-core-2.1.8.tar", last modified: Sat Mar 23 13:42:13 2024, max compression
+gzip compressed data, was "mapel_core-2.1.9.tar", last modified: Mon Apr 15 08:50:16 2024, max compression
```

## Comparing `mapel-core-2.1.8.tar` & `mapel_core-2.1.9.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 13:42:13.761350 mapel-core-2.1.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-03-23 13:42:07.000000 mapel-core-2.1.8/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3258 2024-03-23 13:42:13.761350 mapel-core-2.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-03-23 13:42:07.000000 mapel-core-2.1.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      873 2024-03-23 13:42:07.000000 mapel-core-2.1.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-03-23 13:42:07.000000 mapel-core-2.1.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-23 13:42:13.761350 mapel-core-2.1.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 13:42:13.753350 mapel-core-2.1.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 13:42:13.753350 mapel-core-2.1.8/src/mapel/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 13:42:13.753350 mapel-core-2.1.8/src/mapel/core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-23 13:42:07.000000 mapel-core-2.1.8/src/mapel/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 13:42:13.757350 mapel-core-2.1.8/src/mapel/core/embedding/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-23 13:42:07.000000 mapel-core-2.1.8/src/mapel/core/embedding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6574 2024-03-23 13:42:07.000000 mapel-core-2.1.8/src/mapel/core/embedding/embed.py
--rw-r--r--   0 runner    (1001) docker     (127)     2202 2024-03-23 13:42:07.000000 mapel-core-2.1.8/src/mapel/core/embedding/initial_positions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 13:42:13.757350 mapel-core-2.1.8/src/mapel/core/embedding/kamada_kawai/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-23 13:42:07.000000 mapel-core-2.1.8/src/mapel/core/embedding/kamada_kawai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5266 2024-03-23 13:42:07.000000 mapel-core-2.1.8/src/mapel/core/embedding/kamada_kawai/energy_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     5767 2024-03-23 13:42:07.000000 mapel-core-2.1.8/src/mapel/core/embedding/kamada_kawai/kamada_kawai.py
--rw-r--r--   0 runner    (1001) docker     (127)     4620 2024-03-23 13:42:07.000000 mapel-core-2.1.8/src/mapel/core/embedding/kamada_kawai/optimization_algorithms.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 13:42:13.757350 mapel-core-2.1.8/src/mapel/core/embedding/simulated_annealing/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-23 13:42:07.000000 mapel-core-2.1.8/src/mapel/core/embedding/simulated_annealing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5204 2024-03-23 13:42:07.000000 mapel-core-2.1.8/src/mapel/core/embedding/simulated_annealing/simulated_annealing.py
--rw-r--r--   0 runner    (1001) docker     (127)      775 2024-03-23 13:42:07.000000 mapel-core-2.1.8/src/mapel/core/embedding/simulated_annealing/simulated_annealing_energy.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 13:42:13.757350 mapel-core-2.1.8/src/mapel/core/features/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-23 13:42:07.000000 mapel-core-2.1.8/src/mapel/core/features/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1572 2024-03-23 13:42:07.000000 mapel-core-2.1.8/src/mapel/core/features/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     4130 2024-03-23 13:42:07.000000 mapel-core-2.1.8/src/mapel/core/features/distortion.py
--rw-r--r--   0 runner    (1001) docker     (127)     3120 2024-03-23 13:42:07.000000 mapel-core-2.1.8/src/mapel/core/features/mallows.py
--rw-r--r--   0 runner    (1001) docker     (127)     4866 2024-03-23 13:42:07.000000 mapel-core-2.1.8/src/mapel/core/features/monotonicity.py
--rw-r--r--   0 runner    (1001) docker     (127)     2993 2024-03-23 13:42:07.000000 mapel-core-2.1.8/src/mapel/core/features/stability.py
--rw-r--r--   0 runner    (1001) docker     (127)      620 2024-03-23 13:42:07.000000 mapel-core-2.1.8/src/mapel/core/features_main.py
--rw-r--r--   0 runner    (1001) docker     (127)     5847 2024-03-23 13:42:07.000000 mapel-core-2.1.8/src/mapel/core/glossary.py
--rw-r--r--   0 runner    (1001) docker     (127)     5808 2024-03-23 13:42:07.000000 mapel-core-2.1.8/src/mapel/core/inner_distances.py
--rw-r--r--   0 runner    (1001) docker     (127)     3398 2024-03-23 13:42:07.000000 mapel-core-2.1.8/src/mapel/core/matchings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 13:42:13.757350 mapel-core-2.1.8/src/mapel/core/objects/
--rw-r--r--   0 runner    (1001) docker     (127)    17140 2024-03-23 13:42:07.000000 mapel-core-2.1.8/src/mapel/core/objects/Experiment.py
--rw-r--r--   0 runner    (1001) docker     (127)     1329 2024-03-23 13:42:07.000000 mapel-core-2.1.8/src/mapel/core/objects/Family.py
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-03-23 13:42:07.000000 mapel-core-2.1.8/src/mapel/core/objects/Instance.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-23 13:42:07.000000 mapel-core-2.1.8/src/mapel/core/objects/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 13:42:13.761350 mapel-core-2.1.8/src/mapel/core/persistence/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-23 13:42:07.000000 mapel-core-2.1.8/src/mapel/core/persistence/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7325 2024-03-23 13:42:07.000000 mapel-core-2.1.8/src/mapel/core/persistence/experiment_exports.py
--rw-r--r--   0 runner    (1001) docker     (127)     8460 2024-03-23 13:42:07.000000 mapel-core-2.1.8/src/mapel/core/persistence/experiment_imports.py
--rw-r--r--   0 runner    (1001) docker     (127)    67459 2024-03-23 13:42:07.000000 mapel-core-2.1.8/src/mapel/core/printing.py
--rw-r--r--   0 runner    (1001) docker     (127)      680 2024-03-23 13:42:07.000000 mapel-core-2.1.8/src/mapel/core/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 13:42:13.761350 mapel-core-2.1.8/src/mapel_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3258 2024-03-23 13:42:13.000000 mapel-core-2.1.8/src/mapel_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1482 2024-03-23 13:42:13.000000 mapel-core-2.1.8/src/mapel_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-23 13:42:13.000000 mapel-core-2.1.8/src/mapel_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-03-23 13:42:13.000000 mapel-core-2.1.8/src/mapel_core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-03-23 13:42:13.000000 mapel-core-2.1.8/src/mapel_core.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:50:16.137055 mapel_core-2.1.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-04-15 08:50:09.000000 mapel_core-2.1.9/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3259 2024-04-15 08:50:16.137055 mapel_core-2.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-04-15 08:50:09.000000 mapel_core-2.1.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      873 2024-04-15 08:50:09.000000 mapel_core-2.1.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-15 08:50:09.000000 mapel_core-2.1.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 08:50:16.137055 mapel_core-2.1.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:50:16.129055 mapel_core-2.1.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:50:16.129055 mapel_core-2.1.9/src/mapel/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:50:16.133055 mapel_core-2.1.9/src/mapel/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 08:50:09.000000 mapel_core-2.1.9/src/mapel/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:50:16.133055 mapel_core-2.1.9/src/mapel/core/embedding/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 08:50:09.000000 mapel_core-2.1.9/src/mapel/core/embedding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6574 2024-04-15 08:50:09.000000 mapel_core-2.1.9/src/mapel/core/embedding/embed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2202 2024-04-15 08:50:09.000000 mapel_core-2.1.9/src/mapel/core/embedding/initial_positions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:50:16.133055 mapel_core-2.1.9/src/mapel/core/embedding/kamada_kawai/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 08:50:09.000000 mapel_core-2.1.9/src/mapel/core/embedding/kamada_kawai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5266 2024-04-15 08:50:09.000000 mapel_core-2.1.9/src/mapel/core/embedding/kamada_kawai/energy_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5767 2024-04-15 08:50:09.000000 mapel_core-2.1.9/src/mapel/core/embedding/kamada_kawai/kamada_kawai.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4620 2024-04-15 08:50:09.000000 mapel_core-2.1.9/src/mapel/core/embedding/kamada_kawai/optimization_algorithms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:50:16.133055 mapel_core-2.1.9/src/mapel/core/embedding/simulated_annealing/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 08:50:09.000000 mapel_core-2.1.9/src/mapel/core/embedding/simulated_annealing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5204 2024-04-15 08:50:09.000000 mapel_core-2.1.9/src/mapel/core/embedding/simulated_annealing/simulated_annealing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-04-15 08:50:09.000000 mapel_core-2.1.9/src/mapel/core/embedding/simulated_annealing/simulated_annealing_energy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:50:16.133055 mapel_core-2.1.9/src/mapel/core/features/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 08:50:09.000000 mapel_core-2.1.9/src/mapel/core/features/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1572 2024-04-15 08:50:09.000000 mapel_core-2.1.9/src/mapel/core/features/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4130 2024-04-15 08:50:09.000000 mapel_core-2.1.9/src/mapel/core/features/distortion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3120 2024-04-15 08:50:09.000000 mapel_core-2.1.9/src/mapel/core/features/mallows.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4866 2024-04-15 08:50:09.000000 mapel_core-2.1.9/src/mapel/core/features/monotonicity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2993 2024-04-15 08:50:09.000000 mapel_core-2.1.9/src/mapel/core/features/stability.py
+-rw-r--r--   0 runner    (1001) docker     (127)      620 2024-04-15 08:50:09.000000 mapel_core-2.1.9/src/mapel/core/features_main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5847 2024-04-15 08:50:09.000000 mapel_core-2.1.9/src/mapel/core/glossary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5808 2024-04-15 08:50:09.000000 mapel_core-2.1.9/src/mapel/core/inner_distances.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3398 2024-04-15 08:50:09.000000 mapel_core-2.1.9/src/mapel/core/matchings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:50:16.133055 mapel_core-2.1.9/src/mapel/core/objects/
+-rw-r--r--   0 runner    (1001) docker     (127)    17140 2024-04-15 08:50:09.000000 mapel_core-2.1.9/src/mapel/core/objects/Experiment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1329 2024-04-15 08:50:09.000000 mapel_core-2.1.9/src/mapel/core/objects/Family.py
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-04-15 08:50:09.000000 mapel_core-2.1.9/src/mapel/core/objects/Instance.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 08:50:09.000000 mapel_core-2.1.9/src/mapel/core/objects/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:50:16.137055 mapel_core-2.1.9/src/mapel/core/persistence/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 08:50:09.000000 mapel_core-2.1.9/src/mapel/core/persistence/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7325 2024-04-15 08:50:09.000000 mapel_core-2.1.9/src/mapel/core/persistence/experiment_exports.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8460 2024-04-15 08:50:09.000000 mapel_core-2.1.9/src/mapel/core/persistence/experiment_imports.py
+-rw-r--r--   0 runner    (1001) docker     (127)    67459 2024-04-15 08:50:09.000000 mapel_core-2.1.9/src/mapel/core/printing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      680 2024-04-15 08:50:09.000000 mapel_core-2.1.9/src/mapel/core/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:50:16.137055 mapel_core-2.1.9/src/mapel_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3259 2024-04-15 08:50:16.000000 mapel_core-2.1.9/src/mapel_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1482 2024-04-15 08:50:16.000000 mapel_core-2.1.9/src/mapel_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 08:50:16.000000 mapel_core-2.1.9/src/mapel_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-15 08:50:16.000000 mapel_core-2.1.9/src/mapel_core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-15 08:50:16.000000 mapel_core-2.1.9/src/mapel_core.egg-info/top_level.txt
```

### Comparing `mapel-core-2.1.8/LICENSE.txt` & `mapel_core-2.1.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mapel-core-2.1.8/PKG-INFO` & `mapel_core-2.1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mapel-core
-Version: 2.1.8
+Version: 2.1.9
 Summary: Map of Elections---essential parts
 Author-email: Stanislaw Szufa <s.szufa@gmail.com>, Niclas Boehmer <niclas.boehmer@tu-berlin.de>, Andrzej Kaczmarczyk <andrzej.kaczmarczyk@agh.edu.pl>, Kasper Sapala <kasper.sapala@gmail.com>, Tomasz Was <tomasz.t.was@gmail.com>
 License: Copyright (c) 2018-2022 Stanisław Szufa and contributors
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -34,15 +34,15 @@
 Requires-Dist: pillow~=10.0.0
 Requires-Dist: scipy~=1.10.1
 Requires-Dist: networkx~=3.1
 Requires-Dist: scikit-learn~=1.3.0
 Requires-Dist: tikzplotlib~=0.10.1
 Requires-Dist: tqdm~=4.66.0
 Requires-Dist: gurobipy~=10.0.2
-Requires-Dist: prefsampling>=0.1.6
+Requires-Dist: prefsampling==0.1.15
 
 # Mapel-core
 This package contains the necessary core parts of the mapel ecosystem. Mapel can
 be used to draw maps of different kinds of computational problem instances based
 on metrices defining distances between two instances.
 
 This package provides the framework that can be further extended. Some of the
```

### Comparing `mapel-core-2.1.8/README.md` & `mapel_core-2.1.9/README.md`

 * *Files identical despite different names*

### Comparing `mapel-core-2.1.8/pyproject.toml` & `mapel_core-2.1.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=65", "wheel", "pybind11>=2.6.1"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mapel-core"
-version = "2.1.8"
+version = "2.1.9"
 authors = [
  {name = "Stanislaw Szufa", email = "s.szufa@gmail.com"},
  {name = "Niclas Boehmer", email = "niclas.boehmer@tu-berlin.de"},
  {name = "Andrzej Kaczmarczyk", email = "andrzej.kaczmarczyk@agh.edu.pl"},
  {name = "Kasper Sapala", email = "kasper.sapala@gmail.com"},
  {name = "Tomasz Was", email = "tomasz.t.was@gmail.com"},
 ]
```

### Comparing `mapel-core-2.1.8/src/mapel/core/embedding/embed.py` & `mapel_core-2.1.9/src/mapel/core/embedding/embed.py`

 * *Files identical despite different names*

### Comparing `mapel-core-2.1.8/src/mapel/core/embedding/initial_positions.py` & `mapel_core-2.1.9/src/mapel/core/embedding/initial_positions.py`

 * *Files identical despite different names*

### Comparing `mapel-core-2.1.8/src/mapel/core/embedding/kamada_kawai/energy_functions.py` & `mapel_core-2.1.9/src/mapel/core/embedding/kamada_kawai/energy_functions.py`

 * *Files identical despite different names*

### Comparing `mapel-core-2.1.8/src/mapel/core/embedding/kamada_kawai/kamada_kawai.py` & `mapel_core-2.1.9/src/mapel/core/embedding/kamada_kawai/kamada_kawai.py`

 * *Files identical despite different names*

### Comparing `mapel-core-2.1.8/src/mapel/core/embedding/kamada_kawai/optimization_algorithms.py` & `mapel_core-2.1.9/src/mapel/core/embedding/kamada_kawai/optimization_algorithms.py`

 * *Files identical despite different names*

### Comparing `mapel-core-2.1.8/src/mapel/core/embedding/simulated_annealing/simulated_annealing.py` & `mapel_core-2.1.9/src/mapel/core/embedding/simulated_annealing/simulated_annealing.py`

 * *Files identical despite different names*

### Comparing `mapel-core-2.1.8/src/mapel/core/embedding/simulated_annealing/simulated_annealing_energy.py` & `mapel_core-2.1.9/src/mapel/core/embedding/simulated_annealing/simulated_annealing_energy.py`

 * *Files identical despite different names*

### Comparing `mapel-core-2.1.8/src/mapel/core/features/common.py` & `mapel_core-2.1.9/src/mapel/core/features/common.py`

 * *Files identical despite different names*

### Comparing `mapel-core-2.1.8/src/mapel/core/features/distortion.py` & `mapel_core-2.1.9/src/mapel/core/features/distortion.py`

 * *Files identical despite different names*

### Comparing `mapel-core-2.1.8/src/mapel/core/features/mallows.py` & `mapel_core-2.1.9/src/mapel/core/features/mallows.py`

 * *Files identical despite different names*

### Comparing `mapel-core-2.1.8/src/mapel/core/features/monotonicity.py` & `mapel_core-2.1.9/src/mapel/core/features/monotonicity.py`

 * *Files identical despite different names*

### Comparing `mapel-core-2.1.8/src/mapel/core/features/stability.py` & `mapel_core-2.1.9/src/mapel/core/features/stability.py`

 * *Files identical despite different names*

### Comparing `mapel-core-2.1.8/src/mapel/core/features_main.py` & `mapel_core-2.1.9/src/mapel/core/features_main.py`

 * *Files identical despite different names*

### Comparing `mapel-core-2.1.8/src/mapel/core/glossary.py` & `mapel_core-2.1.9/src/mapel/core/glossary.py`

 * *Files identical despite different names*

### Comparing `mapel-core-2.1.8/src/mapel/core/inner_distances.py` & `mapel_core-2.1.9/src/mapel/core/inner_distances.py`

 * *Files identical despite different names*

### Comparing `mapel-core-2.1.8/src/mapel/core/matchings.py` & `mapel_core-2.1.9/src/mapel/core/matchings.py`

 * *Files identical despite different names*

### Comparing `mapel-core-2.1.8/src/mapel/core/objects/Experiment.py` & `mapel_core-2.1.9/src/mapel/core/objects/Experiment.py`

 * *Files identical despite different names*

### Comparing `mapel-core-2.1.8/src/mapel/core/objects/Family.py` & `mapel_core-2.1.9/src/mapel/core/objects/Family.py`

 * *Files identical despite different names*

### Comparing `mapel-core-2.1.8/src/mapel/core/persistence/experiment_exports.py` & `mapel_core-2.1.9/src/mapel/core/persistence/experiment_exports.py`

 * *Files identical despite different names*

### Comparing `mapel-core-2.1.8/src/mapel/core/persistence/experiment_imports.py` & `mapel_core-2.1.9/src/mapel/core/persistence/experiment_imports.py`

 * *Files identical despite different names*

### Comparing `mapel-core-2.1.8/src/mapel/core/printing.py` & `mapel_core-2.1.9/src/mapel/core/printing.py`

 * *Files identical despite different names*

### Comparing `mapel-core-2.1.8/src/mapel/core/utils.py` & `mapel_core-2.1.9/src/mapel/core/utils.py`

 * *Files identical despite different names*

### Comparing `mapel-core-2.1.8/src/mapel_core.egg-info/PKG-INFO` & `mapel_core-2.1.9/src/mapel_core.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mapel-core
-Version: 2.1.8
+Version: 2.1.9
 Summary: Map of Elections---essential parts
 Author-email: Stanislaw Szufa <s.szufa@gmail.com>, Niclas Boehmer <niclas.boehmer@tu-berlin.de>, Andrzej Kaczmarczyk <andrzej.kaczmarczyk@agh.edu.pl>, Kasper Sapala <kasper.sapala@gmail.com>, Tomasz Was <tomasz.t.was@gmail.com>
 License: Copyright (c) 2018-2022 Stanisław Szufa and contributors
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -34,15 +34,15 @@
 Requires-Dist: pillow~=10.0.0
 Requires-Dist: scipy~=1.10.1
 Requires-Dist: networkx~=3.1
 Requires-Dist: scikit-learn~=1.3.0
 Requires-Dist: tikzplotlib~=0.10.1
 Requires-Dist: tqdm~=4.66.0
 Requires-Dist: gurobipy~=10.0.2
-Requires-Dist: prefsampling>=0.1.6
+Requires-Dist: prefsampling==0.1.15
 
 # Mapel-core
 This package contains the necessary core parts of the mapel ecosystem. Mapel can
 be used to draw maps of different kinds of computational problem instances based
 on metrices defining distances between two instances.
 
 This package provides the framework that can be further extended. Some of the
```

### Comparing `mapel-core-2.1.8/src/mapel_core.egg-info/SOURCES.txt` & `mapel_core-2.1.9/src/mapel_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

