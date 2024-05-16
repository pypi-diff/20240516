# Comparing `tmp/ScholarCodeCollective-0.1.7.5.tar.gz` & `tmp/ScholarCodeCollective-0.1.7.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ScholarCodeCollective-0.1.7.5.tar", last modified: Tue May  7 08:21:26 2024, max compression
+gzip compressed data, was "ScholarCodeCollective-0.1.7.6.tar", last modified: Thu May 16 08:26:00 2024, max compression
```

## Comparing `ScholarCodeCollective-0.1.7.5.tar` & `ScholarCodeCollective-0.1.7.6.tar`

### file list

```diff
@@ -1,31 +1,34 @@
-drwxrwxrwx   0        0        0        0 2024-05-07 08:21:26.890458 ScholarCodeCollective-0.1.7.5/
--rw-rw-rw-   0        0        0     1698 2024-05-07 08:21:26.889456 ScholarCodeCollective-0.1.7.5/PKG-INFO
--rw-rw-rw-   0        0        0     1312 2024-05-06 18:22:38.000000 ScholarCodeCollective-0.1.7.5/README.md
-drwxrwxrwx   0        0        0        0 2024-05-07 08:21:26.714372 ScholarCodeCollective-0.1.7.5/ScholarCodeCollective/
-drwxrwxrwx   0        0        0        0 2024-05-07 08:21:26.760913 ScholarCodeCollective-0.1.7.5/ScholarCodeCollective/Community_Representatives_main/
--rw-rw-rw-   0        0        0       26 2024-05-06 17:39:11.000000 ScholarCodeCollective-0.1.7.5/ScholarCodeCollective/Community_Representatives_main/__init__.py
--rw-rw-rw-   0        0        0  1889097 2024-05-07 08:21:26.000000 ScholarCodeCollective-0.1.7.5/ScholarCodeCollective/Community_Representatives_main/functions.c
-drwxrwxrwx   0        0        0        0 2024-05-07 08:21:26.784378 ScholarCodeCollective-0.1.7.5/ScholarCodeCollective/MDL_network_population_clustering_main/
--rw-rw-rw-   0        0        0       40 2024-04-22 16:52:21.000000 ScholarCodeCollective-0.1.7.5/ScholarCodeCollective/MDL_network_population_clustering_main/__init__.py
--rw-rw-rw-   0        0        0    23729 2024-04-22 17:15:12.000000 ScholarCodeCollective-0.1.7.5/ScholarCodeCollective/MDL_network_population_clustering_main/functions.py
-drwxrwxrwx   0        0        0        0 2024-05-07 08:21:26.813260 ScholarCodeCollective-0.1.7.5/ScholarCodeCollective/MDL_regionalization_main/
--rw-rw-rw-   0        0        0       44 2024-04-22 17:13:59.000000 ScholarCodeCollective-0.1.7.5/ScholarCodeCollective/MDL_regionalization_main/__init__.py
--rw-rw-rw-   0        0        0     6047 2024-04-23 11:59:09.000000 ScholarCodeCollective-0.1.7.5/ScholarCodeCollective/MDL_regionalization_main/functions.py
-drwxrwxrwx   0        0        0        0 2024-05-07 08:21:26.854306 ScholarCodeCollective-0.1.7.5/ScholarCodeCollective/Network_hubs_main/
--rw-rw-rw-   0        0        0       37 2024-04-22 16:59:39.000000 ScholarCodeCollective-0.1.7.5/ScholarCodeCollective/Network_hubs_main/__init__.py
--rw-rw-rw-   0        0        0     5995 2024-04-22 17:03:04.000000 ScholarCodeCollective-0.1.7.5/ScholarCodeCollective/Network_hubs_main/functions.py
--rw-rw-rw-   0        0        0      161 2024-05-06 18:22:48.000000 ScholarCodeCollective-0.1.7.5/ScholarCodeCollective/__init__.py
--rw-rw-rw-   0        0        0       42 2024-04-21 11:17:42.000000 ScholarCodeCollective-0.1.7.5/ScholarCodeCollective/cli.py
-drwxrwxrwx   0        0        0        0 2024-05-07 08:21:26.876660 ScholarCodeCollective-0.1.7.5/ScholarCodeCollective/hypergraph_binning_main/
--rw-rw-rw-   0        0        0       43 2024-04-21 11:55:34.000000 ScholarCodeCollective-0.1.7.5/ScholarCodeCollective/hypergraph_binning_main/__init__.py
--rw-rw-rw-   0        0        0     9020 2024-04-22 17:04:56.000000 ScholarCodeCollective-0.1.7.5/ScholarCodeCollective/hypergraph_binning_main/functions.py
-drwxrwxrwx   0        0        0        0 2024-05-07 08:21:26.739578 ScholarCodeCollective-0.1.7.5/ScholarCodeCollective.egg-info/
--rw-rw-rw-   0        0        0     1698 2024-05-07 08:21:26.000000 ScholarCodeCollective-0.1.7.5/ScholarCodeCollective.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      945 2024-05-07 08:21:26.000000 ScholarCodeCollective-0.1.7.5/ScholarCodeCollective.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-07 08:21:26.000000 ScholarCodeCollective-0.1.7.5/ScholarCodeCollective.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       41 2024-05-07 08:21:26.000000 ScholarCodeCollective-0.1.7.5/ScholarCodeCollective.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       28 2024-05-07 08:21:26.000000 ScholarCodeCollective-0.1.7.5/ScholarCodeCollective.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-07 08:21:26.890458 ScholarCodeCollective-0.1.7.5/setup.cfg
--rw-rw-rw-   0        0        0     2128 2024-05-07 08:20:44.000000 ScholarCodeCollective-0.1.7.5/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-07 08:21:26.886942 ScholarCodeCollective-0.1.7.5/tests/
--rw-rw-rw-   0        0        0     1010 2024-04-22 17:16:16.000000 ScholarCodeCollective-0.1.7.5/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-16 08:26:00.315745 ScholarCodeCollective-0.1.7.6/
+drwxrwxrwx   0        0        0        0 2024-05-16 08:26:00.279431 ScholarCodeCollective-0.1.7.6/Community_Representatives_main/
+-rw-rw-rw-   0        0        0       26 2024-05-06 17:39:11.000000 ScholarCodeCollective-0.1.7.6/Community_Representatives_main/__init__.py
+-rw-rw-rw-   0        0        0     2892 2024-05-07 09:26:31.000000 ScholarCodeCollective-0.1.7.6/Community_Representatives_main/functions_python.py
+-rw-rw-rw-   0        0        0     1698 2024-05-16 08:26:00.315745 ScholarCodeCollective-0.1.7.6/PKG-INFO
+-rw-rw-rw-   0        0        0     1312 2024-05-06 18:22:38.000000 ScholarCodeCollective-0.1.7.6/README.md
+drwxrwxrwx   0        0        0        0 2024-05-16 08:26:00.282998 ScholarCodeCollective-0.1.7.6/ScholarCodeCollective/
+drwxrwxrwx   0        0        0        0 2024-05-16 08:26:00.298110 ScholarCodeCollective-0.1.7.6/ScholarCodeCollective/MDL_network_population_clustering_main/
+-rw-rw-rw-   0        0        0       40 2024-04-22 16:52:21.000000 ScholarCodeCollective-0.1.7.6/ScholarCodeCollective/MDL_network_population_clustering_main/__init__.py
+-rw-rw-rw-   0        0        0    23729 2024-04-22 17:15:12.000000 ScholarCodeCollective-0.1.7.6/ScholarCodeCollective/MDL_network_population_clustering_main/functions.py
+drwxrwxrwx   0        0        0        0 2024-05-16 08:26:00.301677 ScholarCodeCollective-0.1.7.6/ScholarCodeCollective/MDL_regionalization_main/
+-rw-rw-rw-   0        0        0       44 2024-04-22 17:13:59.000000 ScholarCodeCollective-0.1.7.6/ScholarCodeCollective/MDL_regionalization_main/__init__.py
+-rw-rw-rw-   0        0        0     6047 2024-04-23 11:59:09.000000 ScholarCodeCollective-0.1.7.6/ScholarCodeCollective/MDL_regionalization_main/functions.py
+drwxrwxrwx   0        0        0        0 2024-05-16 08:26:00.304219 ScholarCodeCollective-0.1.7.6/ScholarCodeCollective/Network_hubs_main/
+-rw-rw-rw-   0        0        0       37 2024-04-22 16:59:39.000000 ScholarCodeCollective-0.1.7.6/ScholarCodeCollective/Network_hubs_main/__init__.py
+-rw-rw-rw-   0        0        0     5995 2024-04-22 17:03:04.000000 ScholarCodeCollective-0.1.7.6/ScholarCodeCollective/Network_hubs_main/functions.py
+-rw-rw-rw-   0        0        0      194 2024-05-16 08:07:26.000000 ScholarCodeCollective-0.1.7.6/ScholarCodeCollective/__init__.py
+-rw-rw-rw-   0        0        0       42 2024-04-21 11:17:42.000000 ScholarCodeCollective-0.1.7.6/ScholarCodeCollective/cli.py
+drwxrwxrwx   0        0        0        0 2024-05-16 08:26:00.308749 ScholarCodeCollective-0.1.7.6/ScholarCodeCollective/hypergraph_binning_main/
+-rw-rw-rw-   0        0        0       43 2024-04-21 11:55:34.000000 ScholarCodeCollective-0.1.7.6/ScholarCodeCollective/hypergraph_binning_main/__init__.py
+-rw-rw-rw-   0        0        0     9020 2024-04-22 17:04:56.000000 ScholarCodeCollective-0.1.7.6/ScholarCodeCollective/hypergraph_binning_main/functions.py
+drwxrwxrwx   0        0        0        0 2024-05-16 08:26:00.312207 ScholarCodeCollective-0.1.7.6/ScholarCodeCollective/urban_boundary_delineation_main/
+-rw-rw-rw-   0        0        0       33 2024-05-16 08:06:37.000000 ScholarCodeCollective-0.1.7.6/ScholarCodeCollective/urban_boundary_delineation_main/__init__.py
+-rw-rw-rw-   0        0        0    15444 2024-05-16 07:54:57.000000 ScholarCodeCollective-0.1.7.6/ScholarCodeCollective/urban_boundary_delineation_main/greedy_algorithm.py
+drwxrwxrwx   0        0        0        0 2024-05-16 08:26:00.294053 ScholarCodeCollective-0.1.7.6/ScholarCodeCollective.egg-info/
+-rw-rw-rw-   0        0        0     1698 2024-05-16 08:26:00.000000 ScholarCodeCollective-0.1.7.6/ScholarCodeCollective.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1049 2024-05-16 08:26:00.000000 ScholarCodeCollective-0.1.7.6/ScholarCodeCollective.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-16 08:26:00.000000 ScholarCodeCollective-0.1.7.6/ScholarCodeCollective.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       41 2024-05-16 08:26:00.000000 ScholarCodeCollective-0.1.7.6/ScholarCodeCollective.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       59 2024-05-16 08:26:00.000000 ScholarCodeCollective-0.1.7.6/ScholarCodeCollective.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-16 08:26:00.316954 ScholarCodeCollective-0.1.7.6/setup.cfg
+-rw-rw-rw-   0        0        0     2145 2024-05-16 08:25:52.000000 ScholarCodeCollective-0.1.7.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-16 08:26:00.313530 ScholarCodeCollective-0.1.7.6/tests/
+-rw-rw-rw-   0        0        0     1090 2024-05-16 08:11:30.000000 ScholarCodeCollective-0.1.7.6/tests/__init__.py
```

### Comparing `ScholarCodeCollective-0.1.7.5/PKG-INFO` & `ScholarCodeCollective-0.1.7.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ScholarCodeCollective
-Version: 0.1.7.5
+Version: 0.1.7.6
 Summary: A collective library for the code behind several academic papers
 Home-page: https://google.com
 Author: Author Name
 Author-email: author_email@mail.com
 License: The Unlicense
 Requires-Python: >=3.9, <3.12
 Description-Content-Type: text/markdown
```

### Comparing `ScholarCodeCollective-0.1.7.5/README.md` & `ScholarCodeCollective-0.1.7.6/README.md`

 * *Files identical despite different names*

### Comparing `ScholarCodeCollective-0.1.7.5/ScholarCodeCollective/MDL_network_population_clustering_main/functions.py` & `ScholarCodeCollective-0.1.7.6/ScholarCodeCollective/MDL_network_population_clustering_main/functions.py`

 * *Files identical despite different names*

### Comparing `ScholarCodeCollective-0.1.7.5/ScholarCodeCollective/MDL_regionalization_main/functions.py` & `ScholarCodeCollective-0.1.7.6/ScholarCodeCollective/MDL_regionalization_main/functions.py`

 * *Files identical despite different names*

### Comparing `ScholarCodeCollective-0.1.7.5/ScholarCodeCollective/Network_hubs_main/functions.py` & `ScholarCodeCollective-0.1.7.6/ScholarCodeCollective/Network_hubs_main/functions.py`

 * *Files identical despite different names*

### Comparing `ScholarCodeCollective-0.1.7.5/ScholarCodeCollective/hypergraph_binning_main/functions.py` & `ScholarCodeCollective-0.1.7.6/ScholarCodeCollective/hypergraph_binning_main/functions.py`

 * *Files identical despite different names*

### Comparing `ScholarCodeCollective-0.1.7.5/ScholarCodeCollective.egg-info/PKG-INFO` & `ScholarCodeCollective-0.1.7.6/ScholarCodeCollective.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ScholarCodeCollective
-Version: 0.1.7.5
+Version: 0.1.7.6
 Summary: A collective library for the code behind several academic papers
 Home-page: https://google.com
 Author: Author Name
 Author-email: author_email@mail.com
 License: The Unlicense
 Requires-Python: >=3.9, <3.12
 Description-Content-Type: text/markdown
```

### Comparing `ScholarCodeCollective-0.1.7.5/ScholarCodeCollective.egg-info/SOURCES.txt` & `ScholarCodeCollective-0.1.7.6/ScholarCodeCollective.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 README.md
 setup.py
+Community_Representatives_main/__init__.py
+Community_Representatives_main/functions_python.py
 ScholarCodeCollective/__init__.py
 ScholarCodeCollective/cli.py
 ScholarCodeCollective.egg-info/PKG-INFO
 ScholarCodeCollective.egg-info/SOURCES.txt
 ScholarCodeCollective.egg-info/dependency_links.txt
 ScholarCodeCollective.egg-info/entry_points.txt
 ScholarCodeCollective.egg-info/top_level.txt
-ScholarCodeCollective/Community_Representatives_main/functions.c
-ScholarCodeCollective/Community_Representatives_main/__init__.py
 ScholarCodeCollective/MDL_network_population_clustering_main/__init__.py
 ScholarCodeCollective/MDL_network_population_clustering_main/functions.py
 ScholarCodeCollective/MDL_regionalization_main/__init__.py
 ScholarCodeCollective/MDL_regionalization_main/functions.py
 ScholarCodeCollective/Network_hubs_main/__init__.py
 ScholarCodeCollective/Network_hubs_main/functions.py
 ScholarCodeCollective/hypergraph_binning_main/__init__.py
 ScholarCodeCollective/hypergraph_binning_main/functions.py
+ScholarCodeCollective/urban_boundary_delineation_main/__init__.py
+ScholarCodeCollective/urban_boundary_delineation_main/greedy_algorithm.py
 tests/__init__.py
```

### Comparing `ScholarCodeCollective-0.1.7.5/setup.py` & `ScholarCodeCollective-0.1.7.6/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,10 @@
 # from distutils.core import setup
 # import pathlib
 # import setuptools
-from setuptools import setup, find_packages, Extension
-from Cython.Build import cythonize
-import numpy  # If your Cython modules use NumPy
 
 
 # setuptools.setup(
 #     name='ScholarCodeCollective',
 #     version='0.1.4',
 #     description='A collective library for the code behind several academic papers',
 #     long_description=open('README.md').read(),
@@ -26,26 +23,30 @@
 #     entry_points={"console_scripts": ["paper = paper.cli:main"]},
 
 # )
 
 # extensions = [
 #     Extension("ScholarCodeCollective.Community_Representatives_main.functions",
 #               ["ScholarCodeCollective/Community_Representatives_main/functions.pyx"],
-#               language='c++')  # use 'c' if not using C++ features
+#               language='c++')  
+# ]
+from setuptools import setup, find_packages, Extension
+from Cython.Build import cythonize
+import numpy
+
+# extensions = [
+#     Extension("ScholarCodeCollective.Community_Representatives_main.functions",
+#               ["ScholarCodeCollective/Community_Representatives_main/functions.pyx"],
+#               include_dirs=[numpy.get_include()],
+#               language='c++')  
 # ]
-extensions = [
-    Extension(
-        "ScholarCodeCollective.Community_Representatives_main.functions",
-        ["ScholarCodeCollective/Community_Representatives_main/functions.pyx"]
-    )
-]
 
 setup(
     name='ScholarCodeCollective',
-    version='0.1.7.5',
+    version='0.1.7.6',
     description='A collective library for the code behind several academic papers',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://google.com',
     author='Author Name',
     author_email='author_email@mail.com',
     license='The Unlicense',
@@ -53,9 +54,9 @@
         "Documentation": "x",
         "Source": "file:///D:/Research%20HKU/PYPI_lib/Documentation/_build/html/index.html"
     },
     python_requires=">=3.9, <3.12",
     packages=find_packages(),
     include_package_data=True,
     entry_points={"console_scripts": ["paper = paper.cli:main"]},
-    ext_modules=cythonize(extensions, compiler_directives={'language_level': "3"})
+    #ext_modules=cythonize(extensions, compiler_directives={'language_level': "3"})
 )
```

### Comparing `ScholarCodeCollective-0.1.7.5/tests/__init__.py` & `ScholarCodeCollective-0.1.7.6/tests/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import time
 import sys
 import ScholarCodeCollective
 from ScholarCodeCollective.hypergraph_binning_main import Hypergraph_binning
 from ScholarCodeCollective.MDL_regionalization_main import MDL_regionalization
 from ScholarCodeCollective.Network_hubs_main import Network_hubs
 from ScholarCodeCollective.MDL_network_population_clustering_main import MDL_populations
+from ScholarCodeCollective.urban_boundary_delineation_main import greedy_opt
+
 
 
 
 hypergraph_instance = ScholarCodeCollective.hypergraph_binning_main.Hypergraph_binning()
 
 # Example call to a method that uses logchoose
 hypergraph_instance.logOmega([5], [2])
```

