# Comparing `tmp/cartoGRAPHs-2.0.0.tar.gz` & `tmp/cartographs-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cartoGRAPHs-2.0.0.tar", last modified: Fri Oct 20 19:11:23 2023, max compression
+gzip compressed data, was "/Users/chris/Desktop/Github/CartoGRAPHs/cartoGRAPHs/dist/.tmp-iam441nv/cartographs-2.0.1.tar", last modified: Thu May 16 09:02:10 2024, max compression
```

## Comparing `cartoGRAPHs-2.0.0.tar` & `cartographs-2.0.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-10-20 19:11:23.858487 cartoGRAPHs-2.0.0/
--rw-r--r--   0 chris      (501) staff       (20)     1090 2021-05-27 18:40:24.000000 cartoGRAPHs-2.0.0/LICENSE.md
--rw-r--r--   0 chris      (501) staff       (20)     6749 2023-10-20 19:11:23.858203 cartoGRAPHs-2.0.0/PKG-INFO
--rw-r--r--   0 chris      (501) staff       (20)     6432 2022-03-18 17:36:43.000000 cartoGRAPHs-2.0.0/README.md
-drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-10-20 19:11:23.855148 cartoGRAPHs-2.0.0/cartoGRAPHs/
--rwx------   0 chris      (501) staff       (20)      228 2023-10-20 08:15:44.000000 cartoGRAPHs-2.0.0/cartoGRAPHs/__init__.py
--rw-r--r--   0 chris      (501) staff       (20)    13885 2023-10-20 09:18:34.000000 cartoGRAPHs-2.0.0/cartoGRAPHs/cartoGRAPHs.py
--rw-r--r--   0 chris      (501) staff       (20)     6081 2023-10-20 09:17:30.000000 cartoGRAPHs-2.0.0/cartoGRAPHs/func_calculations.py
--rw-r--r--   0 chris      (501) staff       (20)    62716 2023-10-20 17:38:58.000000 cartoGRAPHs-2.0.0/cartoGRAPHs/func_embed_plot.py
--rw-r--r--   0 chris      (501) staff       (20)    10043 2023-10-20 09:18:06.000000 cartoGRAPHs-2.0.0/cartoGRAPHs/func_exportVR.py
--rw-r--r--   0 chris      (501) staff       (20)    10608 2023-10-20 09:18:14.000000 cartoGRAPHs-2.0.0/cartoGRAPHs/func_load_data.py
--rw-r--r--   0 chris      (501) staff       (20)    21711 2023-10-20 17:13:05.000000 cartoGRAPHs-2.0.0/cartoGRAPHs/func_visual_properties.py
-drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-10-20 19:11:23.857842 cartoGRAPHs-2.0.0/cartoGRAPHs.egg-info/
--rw-r--r--   0 chris      (501) staff       (20)     6749 2023-10-20 19:11:23.000000 cartoGRAPHs-2.0.0/cartoGRAPHs.egg-info/PKG-INFO
--rw-r--r--   0 chris      (501) staff       (20)      415 2023-10-20 19:11:23.000000 cartoGRAPHs-2.0.0/cartoGRAPHs.egg-info/SOURCES.txt
--rw-r--r--   0 chris      (501) staff       (20)        1 2023-10-20 19:11:23.000000 cartoGRAPHs-2.0.0/cartoGRAPHs.egg-info/dependency_links.txt
--rw-r--r--   0 chris      (501) staff       (20)      123 2023-10-20 19:11:23.000000 cartoGRAPHs-2.0.0/cartoGRAPHs.egg-info/requires.txt
--rw-r--r--   0 chris      (501) staff       (20)       12 2023-10-20 19:11:23.000000 cartoGRAPHs-2.0.0/cartoGRAPHs.egg-info/top_level.txt
--rw-r--r--   0 chris      (501) staff       (20)       38 2023-10-20 19:11:23.858595 cartoGRAPHs-2.0.0/setup.cfg
--rwx------   0 chris      (501) staff       (20)     1064 2023-10-20 19:11:13.000000 cartoGRAPHs-2.0.0/setup.py
+drwxr-xr-x   0 chris      (501) staff       (20)        0 2024-05-16 09:02:10.253977 cartographs-2.0.1/
+-rw-r--r--   0 chris      (501) staff       (20)     1090 2024-05-16 08:47:00.000000 cartographs-2.0.1/LICENSE.md
+-rw-r--r--   0 chris      (501) staff       (20)     7070 2024-05-16 09:02:10.253275 cartographs-2.0.1/PKG-INFO
+-rw-r--r--   0 chris      (501) staff       (20)     6432 2024-05-16 08:47:00.000000 cartographs-2.0.1/README.md
+drwxr-xr-x   0 chris      (501) staff       (20)        0 2024-05-16 09:02:10.248945 cartographs-2.0.1/cartoGRAPHs/
+-rwxr-xr-x   0 chris      (501) staff       (20)      229 2024-05-16 08:47:00.000000 cartographs-2.0.1/cartoGRAPHs/__init__.py
+-rw-r--r--   0 chris      (501) staff       (20)    13885 2024-05-16 08:47:00.000000 cartographs-2.0.1/cartoGRAPHs/cartoGRAPHs.py
+-rw-r--r--   0 chris      (501) staff       (20)     6081 2024-05-16 08:47:00.000000 cartographs-2.0.1/cartoGRAPHs/func_calculations.py
+-rw-r--r--   0 chris      (501) staff       (20)    62738 2024-05-16 08:58:42.000000 cartographs-2.0.1/cartoGRAPHs/func_embed_plot.py
+-rw-r--r--   0 chris      (501) staff       (20)    10043 2024-05-16 08:47:00.000000 cartographs-2.0.1/cartoGRAPHs/func_exportVR.py
+-rw-r--r--   0 chris      (501) staff       (20)    10608 2024-05-16 08:47:00.000000 cartographs-2.0.1/cartoGRAPHs/func_load_data.py
+-rw-r--r--   0 chris      (501) staff       (20)    21711 2024-05-16 08:47:00.000000 cartographs-2.0.1/cartoGRAPHs/func_visual_properties.py
+drwxr-xr-x   0 chris      (501) staff       (20)        0 2024-05-16 09:02:10.252721 cartographs-2.0.1/cartoGRAPHs.egg-info/
+-rw-r--r--   0 chris      (501) staff       (20)     7070 2024-05-16 09:02:10.000000 cartographs-2.0.1/cartoGRAPHs.egg-info/PKG-INFO
+-rw-r--r--   0 chris      (501) staff       (20)      415 2024-05-16 09:02:10.000000 cartographs-2.0.1/cartoGRAPHs.egg-info/SOURCES.txt
+-rw-r--r--   0 chris      (501) staff       (20)        1 2024-05-16 09:02:10.000000 cartographs-2.0.1/cartoGRAPHs.egg-info/dependency_links.txt
+-rw-r--r--   0 chris      (501) staff       (20)      131 2024-05-16 09:02:10.000000 cartographs-2.0.1/cartoGRAPHs.egg-info/requires.txt
+-rw-r--r--   0 chris      (501) staff       (20)       12 2024-05-16 09:02:10.000000 cartographs-2.0.1/cartoGRAPHs.egg-info/top_level.txt
+-rw-r--r--   0 chris      (501) staff       (20)       38 2024-05-16 09:02:10.254106 cartographs-2.0.1/setup.cfg
+-rwxr-xr-x   0 chris      (501) staff       (20)     1073 2024-05-16 08:58:22.000000 cartographs-2.0.1/setup.py
```

### Comparing `cartoGRAPHs-2.0.0/LICENSE.md` & `cartographs-2.0.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `cartoGRAPHs-2.0.0/PKG-INFO` & `cartographs-2.0.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,7 @@
-Metadata-Version: 2.1
-Name: cartoGRAPHs
-Version: 2.0.0
-Summary: A Network Layout and Visualization Package
-Home-page: https://github.com/menchelab/cartoGRAPHs
-Author: Chris H.
-Author-email: chris@menchelab.com
-License: MIT License
-Platform: UNKNOWN
-Description-Content-Type: text/markdown
-License-File: LICENSE.md
-
 # CARTOGRAPHS 
 Visual Network Exploration in two and three dimensions
 
 
 ![cartographs](img/cartographs_img02.png)
 
 ---
@@ -166,9 +154,7 @@
 
 ### SYSTEM REQUIREMENTS
 All Visualizations with networks up to 20,000 nodes and ~300,000 links in the main jupyter notebook were carried out on a machine with a 2 GHz Quad-Core Intel Core i5 and 16GB or Memory. 
 Heavier computation, such as performed during layout benchmarking, was calculated on a cluster and stored in the benchmark/netdist_precalc folder. 
 
 *Please note : This project is work in progress and will be updated/improved frequently.*
 
-
-
```

### Comparing `cartoGRAPHs-2.0.0/README.md` & `cartographs-2.0.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,32 @@
+Metadata-Version: 2.1
+Name: cartoGRAPHs
+Version: 2.0.1
+Summary: A Network Layout and Visualization Package
+Home-page: https://github.com/menchelab/cartoGRAPHs
+Author: Chris H.
+Author-email: chris@menchelab.com
+License: MIT License
+Description-Content-Type: text/markdown
+License-File: LICENSE.md
+Requires-Dist: numpy
+Requires-Dist: pandas
+Requires-Dist: matplotlib
+Requires-Dist: seaborn
+Requires-Dist: scipy
+Requires-Dist: networkx
+Requires-Dist: plotly
+Requires-Dist: colormath
+Requires-Dist: umap-learn
+Requires-Dist: scikit_learn
+Requires-Dist: shapely
+Requires-Dist: colormath
+Requires-Dist: numba
+Requires-Dist: pynndescent==0.5.8
+
 # CARTOGRAPHS 
 Visual Network Exploration in two and three dimensions
 
 
 ![cartographs](img/cartographs_img02.png)
 
 ---
```

### Comparing `cartoGRAPHs-2.0.0/cartoGRAPHs/cartoGRAPHs.py` & `cartographs-2.0.1/cartoGRAPHs/cartoGRAPHs.py`

 * *Files identical despite different names*

### Comparing `cartoGRAPHs-2.0.0/cartoGRAPHs/func_calculations.py` & `cartographs-2.0.1/cartoGRAPHs/func_calculations.py`

 * *Files identical despite different names*

### Comparing `cartoGRAPHs-2.0.0/cartoGRAPHs/func_embed_plot.py` & `cartographs-2.0.1/cartoGRAPHs/func_embed_plot.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,16 @@
 # This python file is part of the Project "cartoGRAPHs"
 # for  E M B E D D I N G & P L O T T I N G  2D + 3D 
 #
 ########################################################################################
 
 import plotly
 import plotly.graph_objs as pgo
-import umap.parametric_umap as umap
+import umap as umap 
+#import umap.parametric_umap as umap
 from sklearn.manifold import TSNE
 from sklearn import preprocessing
 from numpy import pi, cos, sin, arccos, arange
 import math 
 import networkx as nx
 from shapely import geometry
```

### Comparing `cartoGRAPHs-2.0.0/cartoGRAPHs/func_exportVR.py` & `cartographs-2.0.1/cartoGRAPHs/func_exportVR.py`

 * *Files identical despite different names*

### Comparing `cartoGRAPHs-2.0.0/cartoGRAPHs/func_load_data.py` & `cartographs-2.0.1/cartoGRAPHs/func_load_data.py`

 * *Files identical despite different names*

### Comparing `cartoGRAPHs-2.0.0/cartoGRAPHs/func_visual_properties.py` & `cartographs-2.0.1/cartoGRAPHs/func_visual_properties.py`

 * *Files identical despite different names*

### Comparing `cartoGRAPHs-2.0.0/cartoGRAPHs.egg-info/PKG-INFO` & `cartographs-2.0.1/cartoGRAPHs.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,31 @@
 Metadata-Version: 2.1
 Name: cartoGRAPHs
-Version: 2.0.0
+Version: 2.0.1
 Summary: A Network Layout and Visualization Package
 Home-page: https://github.com/menchelab/cartoGRAPHs
 Author: Chris H.
 Author-email: chris@menchelab.com
 License: MIT License
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
+Requires-Dist: numpy
+Requires-Dist: pandas
+Requires-Dist: matplotlib
+Requires-Dist: seaborn
+Requires-Dist: scipy
+Requires-Dist: networkx
+Requires-Dist: plotly
+Requires-Dist: colormath
+Requires-Dist: umap-learn
+Requires-Dist: scikit_learn
+Requires-Dist: shapely
+Requires-Dist: colormath
+Requires-Dist: numba
+Requires-Dist: pynndescent==0.5.8
 
 # CARTOGRAPHS 
 Visual Network Exploration in two and three dimensions
 
 
 ![cartographs](img/cartographs_img02.png)
 
@@ -166,9 +179,7 @@
 
 ### SYSTEM REQUIREMENTS
 All Visualizations with networks up to 20,000 nodes and ~300,000 links in the main jupyter notebook were carried out on a machine with a 2 GHz Quad-Core Intel Core i5 and 16GB or Memory. 
 Heavier computation, such as performed during layout benchmarking, was calculated on a cluster and stored in the benchmark/netdist_precalc folder. 
 
 *Please note : This project is work in progress and will be updated/improved frequently.*
 
-
-
```

### Comparing `cartoGRAPHs-2.0.0/setup.py` & `cartographs-2.0.1/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import pathlib
 from setuptools import setup, find_packages
 
 HERE = pathlib.Path(__file__).parent
 
-VERSION = '2.0.0'
+VERSION = '2.0.1'
 PACKAGE_NAME = 'cartoGRAPHs'
 AUTHOR = 'Chris H.'
 AUTHOR_EMAIL = 'chris@menchelab.com'
 URL = 'https://github.com/menchelab/cartoGRAPHs'
 
 LICENSE = 'MIT License'
 DESCRIPTION = 'A Network Layout and Visualization Package'
@@ -24,22 +24,22 @@
         'plotly',
         'colormath',
         'umap-learn',
         'scikit_learn',
         'shapely',
         'colormath',
         'numba',
-        'tensorflow'
+        'pynndescent==0.5.8'
 ]
 
 setup(name=PACKAGE_NAME,
       version=VERSION,
       description=DESCRIPTION,
       long_description=LONG_DESCRIPTION,
       long_description_content_type=LONG_DESC_TYPE,
       author=AUTHOR,
       license=LICENSE,
       author_email=AUTHOR_EMAIL,
       url=URL,
       install_requires=INSTALL_REQUIRES,
       packages=find_packages()
-      )
+      )
```

