# Comparing `tmp/mapel-2.1.8.tar.gz` & `tmp/mapel-2.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mapel-2.1.8.tar", last modified: Sat Mar 23 13:42:11 2024, max compression
+gzip compressed data, was "mapel-2.1.9.tar", last modified: Mon Apr 15 08:50:14 2024, max compression
```

## Comparing `mapel-2.1.8.tar` & `mapel-2.1.9.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 13:42:11.569327 mapel-2.1.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-03-23 13:42:07.000000 mapel-2.1.8/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2624 2024-03-23 13:42:11.569327 mapel-2.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      600 2024-03-23 13:42:07.000000 mapel-2.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 13:42:11.569327 mapel-2.1.8/mapel.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2624 2024-03-23 13:42:11.000000 mapel-2.1.8/mapel.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-03-23 13:42:11.000000 mapel-2.1.8/mapel.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-23 13:42:11.000000 mapel-2.1.8/mapel.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-03-23 13:42:11.000000 mapel-2.1.8/mapel.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-23 13:42:11.000000 mapel-2.1.8/mapel.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      959 2024-03-23 13:42:07.000000 mapel-2.1.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-03-23 13:42:07.000000 mapel-2.1.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-23 13:42:11.569327 mapel-2.1.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:50:14.029045 mapel-2.1.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-04-15 08:50:09.000000 mapel-2.1.9/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2624 2024-04-15 08:50:14.029045 mapel-2.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-04-15 08:50:09.000000 mapel-2.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:50:14.029045 mapel-2.1.9/mapel.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2624 2024-04-15 08:50:14.000000 mapel-2.1.9/mapel.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-15 08:50:14.000000 mapel-2.1.9/mapel.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 08:50:14.000000 mapel-2.1.9/mapel.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-15 08:50:14.000000 mapel-2.1.9/mapel.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 08:50:14.000000 mapel-2.1.9/mapel.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      959 2024-04-15 08:50:09.000000 mapel-2.1.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-15 08:50:09.000000 mapel-2.1.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 08:50:14.029045 mapel-2.1.9/setup.cfg
```

### Comparing `mapel-2.1.8/LICENSE.txt` & `mapel-2.1.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mapel-2.1.8/PKG-INFO` & `mapel-2.1.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mapel
-Version: 2.1.8
+Version: 2.1.9
 Summary: Map of Elections---all packages
 Author-email: Stanislaw Szufa <s.szufa@gmail.com>, Niclas Boehmer <niclas.boehmer@tu-berlin.de>, Piotr Faliszewski <faliszew@agh.edu.pl>, Lukasz Janeczko <lukij1997@gmail.com>, Andrzej Kaczmarczyk <andrzej.kaczmarczyk@agh.edu.pl>, Kasper Sapala <kasper.sapala@gmail.com>, Tomasz Was <tomasz.t.was@gmail.com>
 License: Copyright (c) 2018-2022 Stanislaw Szufa and contributors
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -25,18 +25,18 @@
         
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
-Requires-Dist: mapel-core==2.1.8
-Requires-Dist: mapel-elections==2.1.8
-Requires-Dist: mapel-roommates==2.1.8
-Requires-Dist: mapel-marriages==2.1.8
+Requires-Dist: mapel-core==2.1.9
+Requires-Dist: mapel-elections==2.1.9
+Requires-Dist: mapel-roommates==2.1.9
+Requires-Dist: mapel-marriages==2.1.9
 
 # Mapel
 This package's purpose is to install jointly the following (so far all) parts of
 the mapel ecosystem:  
 1. mapel-core
 1. mapel-elections
 1. mapel-roommates
```

### Comparing `mapel-2.1.8/README.md` & `mapel-2.1.9/README.md`

 * *Files identical despite different names*

### Comparing `mapel-2.1.8/mapel.egg-info/PKG-INFO` & `mapel-2.1.9/mapel.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mapel
-Version: 2.1.8
+Version: 2.1.9
 Summary: Map of Elections---all packages
 Author-email: Stanislaw Szufa <s.szufa@gmail.com>, Niclas Boehmer <niclas.boehmer@tu-berlin.de>, Piotr Faliszewski <faliszew@agh.edu.pl>, Lukasz Janeczko <lukij1997@gmail.com>, Andrzej Kaczmarczyk <andrzej.kaczmarczyk@agh.edu.pl>, Kasper Sapala <kasper.sapala@gmail.com>, Tomasz Was <tomasz.t.was@gmail.com>
 License: Copyright (c) 2018-2022 Stanislaw Szufa and contributors
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -25,18 +25,18 @@
         
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
-Requires-Dist: mapel-core==2.1.8
-Requires-Dist: mapel-elections==2.1.8
-Requires-Dist: mapel-roommates==2.1.8
-Requires-Dist: mapel-marriages==2.1.8
+Requires-Dist: mapel-core==2.1.9
+Requires-Dist: mapel-elections==2.1.9
+Requires-Dist: mapel-roommates==2.1.9
+Requires-Dist: mapel-marriages==2.1.9
 
 # Mapel
 This package's purpose is to install jointly the following (so far all) parts of
 the mapel ecosystem:  
 1. mapel-core
 1. mapel-elections
 1. mapel-roommates
```

### Comparing `mapel-2.1.8/pyproject.toml` & `mapel-2.1.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=65"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mapel"
-version = "2.1.8"
+version = "2.1.9"
 authors = [
  {name = "Stanislaw Szufa", email = "s.szufa@gmail.com"},
  {name = "Niclas Boehmer", email = "niclas.boehmer@tu-berlin.de"},
  {name = "Piotr Faliszewski", email = "faliszew@agh.edu.pl"},
  {name = "Lukasz Janeczko", email = "lukij1997@gmail.com"},
  {name = "Andrzej Kaczmarczyk", email = "andrzej.kaczmarczyk@agh.edu.pl"},
  {name = "Kasper Sapala", email = "kasper.sapala@gmail.com"},
```

