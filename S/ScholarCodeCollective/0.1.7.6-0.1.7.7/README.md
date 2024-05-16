# Comparing `tmp/ScholarCodeCollective-0.1.7.6.tar.gz` & `tmp/ScholarCodeCollective-0.1.7.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ScholarCodeCollective-0.1.7.6.tar", last modified: Thu May 16 08:26:00 2024, max compression
+gzip compressed data, was "ScholarCodeCollective-0.1.7.7.tar", last modified: Thu May 16 08:41:48 2024, max compression
```

## Comparing `ScholarCodeCollective-0.1.7.6.tar` & `ScholarCodeCollective-0.1.7.7.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxrwx   0        0        0        0 2024-05-16 08:26:00.315745 ScholarCodeCollective-0.1.7.6/
-drwxrwxrwx   0        0        0        0 2024-05-16 08:26:00.279431 ScholarCodeCollective-0.1.7.6/Community_Representatives_main/
--rw-rw-rw-   0        0        0       26 2024-05-06 17:39:11.000000 ScholarCodeCollective-0.1.7.6/Community_Representatives_main/__init__.py
--rw-rw-rw-   0        0        0     2892 2024-05-07 09:26:31.000000 ScholarCodeCollective-0.1.7.6/Community_Representatives_main/functions_python.py
--rw-rw-rw-   0        0        0     1698 2024-05-16 08:26:00.315745 ScholarCodeCollective-0.1.7.6/PKG-INFO
--rw-rw-rw-   0        0        0     1312 2024-05-06 18:22:38.000000 ScholarCodeCollective-0.1.7.6/README.md
-drwxrwxrwx   0        0        0        0 2024-05-16 08:26:00.282998 ScholarCodeCollective-0.1.7.6/ScholarCodeCollective/
-drwxrwxrwx   0        0        0        0 2024-05-16 08:26:00.298110 ScholarCodeCollective-0.1.7.6/ScholarCodeCollective/MDL_network_population_clustering_main/
--rw-rw-rw-   0        0        0       40 2024-04-22 16:52:21.000000 ScholarCodeCollective-0.1.7.6/ScholarCodeCollective/MDL_network_population_clustering_main/__init__.py
--rw-rw-rw-   0        0        0    23729 2024-04-22 17:15:12.000000 ScholarCodeCollective-0.1.7.6/ScholarCodeCollective/MDL_network_population_clustering_main/functions.py
-drwxrwxrwx   0        0        0        0 2024-05-16 08:26:00.301677 ScholarCodeCollective-0.1.7.6/ScholarCodeCollective/MDL_regionalization_main/
--rw-rw-rw-   0        0        0       44 2024-04-22 17:13:59.000000 ScholarCodeCollective-0.1.7.6/ScholarCodeCollective/MDL_regionalization_main/__init__.py
--rw-rw-rw-   0        0        0     6047 2024-04-23 11:59:09.000000 ScholarCodeCollective-0.1.7.6/ScholarCodeCollective/MDL_regionalization_main/functions.py
-drwxrwxrwx   0        0        0        0 2024-05-16 08:26:00.304219 ScholarCodeCollective-0.1.7.6/ScholarCodeCollective/Network_hubs_main/
--rw-rw-rw-   0        0        0       37 2024-04-22 16:59:39.000000 ScholarCodeCollective-0.1.7.6/ScholarCodeCollective/Network_hubs_main/__init__.py
--rw-rw-rw-   0        0        0     5995 2024-04-22 17:03:04.000000 ScholarCodeCollective-0.1.7.6/ScholarCodeCollective/Network_hubs_main/functions.py
--rw-rw-rw-   0        0        0      194 2024-05-16 08:07:26.000000 ScholarCodeCollective-0.1.7.6/ScholarCodeCollective/__init__.py
--rw-rw-rw-   0        0        0       42 2024-04-21 11:17:42.000000 ScholarCodeCollective-0.1.7.6/ScholarCodeCollective/cli.py
-drwxrwxrwx   0        0        0        0 2024-05-16 08:26:00.308749 ScholarCodeCollective-0.1.7.6/ScholarCodeCollective/hypergraph_binning_main/
--rw-rw-rw-   0        0        0       43 2024-04-21 11:55:34.000000 ScholarCodeCollective-0.1.7.6/ScholarCodeCollective/hypergraph_binning_main/__init__.py
--rw-rw-rw-   0        0        0     9020 2024-04-22 17:04:56.000000 ScholarCodeCollective-0.1.7.6/ScholarCodeCollective/hypergraph_binning_main/functions.py
-drwxrwxrwx   0        0        0        0 2024-05-16 08:26:00.312207 ScholarCodeCollective-0.1.7.6/ScholarCodeCollective/urban_boundary_delineation_main/
--rw-rw-rw-   0        0        0       33 2024-05-16 08:06:37.000000 ScholarCodeCollective-0.1.7.6/ScholarCodeCollective/urban_boundary_delineation_main/__init__.py
--rw-rw-rw-   0        0        0    15444 2024-05-16 07:54:57.000000 ScholarCodeCollective-0.1.7.6/ScholarCodeCollective/urban_boundary_delineation_main/greedy_algorithm.py
-drwxrwxrwx   0        0        0        0 2024-05-16 08:26:00.294053 ScholarCodeCollective-0.1.7.6/ScholarCodeCollective.egg-info/
--rw-rw-rw-   0        0        0     1698 2024-05-16 08:26:00.000000 ScholarCodeCollective-0.1.7.6/ScholarCodeCollective.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1049 2024-05-16 08:26:00.000000 ScholarCodeCollective-0.1.7.6/ScholarCodeCollective.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-16 08:26:00.000000 ScholarCodeCollective-0.1.7.6/ScholarCodeCollective.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       41 2024-05-16 08:26:00.000000 ScholarCodeCollective-0.1.7.6/ScholarCodeCollective.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       59 2024-05-16 08:26:00.000000 ScholarCodeCollective-0.1.7.6/ScholarCodeCollective.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-16 08:26:00.316954 ScholarCodeCollective-0.1.7.6/setup.cfg
--rw-rw-rw-   0        0        0     2145 2024-05-16 08:25:52.000000 ScholarCodeCollective-0.1.7.6/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-16 08:26:00.313530 ScholarCodeCollective-0.1.7.6/tests/
--rw-rw-rw-   0        0        0     1090 2024-05-16 08:11:30.000000 ScholarCodeCollective-0.1.7.6/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-16 08:41:48.355075 ScholarCodeCollective-0.1.7.7/
+drwxrwxrwx   0        0        0        0 2024-05-16 08:41:48.289539 ScholarCodeCollective-0.1.7.7/Community_Representatives_main/
+-rw-rw-rw-   0        0        0       26 2024-05-06 17:39:11.000000 ScholarCodeCollective-0.1.7.7/Community_Representatives_main/__init__.py
+-rw-rw-rw-   0        0        0     2892 2024-05-07 09:26:31.000000 ScholarCodeCollective-0.1.7.7/Community_Representatives_main/functions_python.py
+-rw-rw-rw-   0        0        0     1698 2024-05-16 08:41:48.353342 ScholarCodeCollective-0.1.7.7/PKG-INFO
+-rw-rw-rw-   0        0        0     1312 2024-05-06 18:22:38.000000 ScholarCodeCollective-0.1.7.7/README.md
+drwxrwxrwx   0        0        0        0 2024-05-16 08:41:48.302830 ScholarCodeCollective-0.1.7.7/ScholarCodeCollective/
+drwxrwxrwx   0        0        0        0 2024-05-16 08:41:48.335934 ScholarCodeCollective-0.1.7.7/ScholarCodeCollective/MDL_network_population_clustering_main/
+-rw-rw-rw-   0        0        0       40 2024-04-22 16:52:21.000000 ScholarCodeCollective-0.1.7.7/ScholarCodeCollective/MDL_network_population_clustering_main/__init__.py
+-rw-rw-rw-   0        0        0    23729 2024-04-22 17:15:12.000000 ScholarCodeCollective-0.1.7.7/ScholarCodeCollective/MDL_network_population_clustering_main/functions.py
+drwxrwxrwx   0        0        0        0 2024-05-16 08:41:48.339178 ScholarCodeCollective-0.1.7.7/ScholarCodeCollective/MDL_regionalization_main/
+-rw-rw-rw-   0        0        0       44 2024-04-22 17:13:59.000000 ScholarCodeCollective-0.1.7.7/ScholarCodeCollective/MDL_regionalization_main/__init__.py
+-rw-rw-rw-   0        0        0     6047 2024-04-23 11:59:09.000000 ScholarCodeCollective-0.1.7.7/ScholarCodeCollective/MDL_regionalization_main/functions.py
+drwxrwxrwx   0        0        0        0 2024-05-16 08:41:48.343171 ScholarCodeCollective-0.1.7.7/ScholarCodeCollective/Network_hubs_main/
+-rw-rw-rw-   0        0        0       37 2024-04-22 16:59:39.000000 ScholarCodeCollective-0.1.7.7/ScholarCodeCollective/Network_hubs_main/__init__.py
+-rw-rw-rw-   0        0        0     5995 2024-04-22 17:03:04.000000 ScholarCodeCollective-0.1.7.7/ScholarCodeCollective/Network_hubs_main/functions.py
+-rw-rw-rw-   0        0        0      162 2024-05-16 08:41:30.000000 ScholarCodeCollective-0.1.7.7/ScholarCodeCollective/__init__.py
+-rw-rw-rw-   0        0        0       42 2024-04-21 11:17:42.000000 ScholarCodeCollective-0.1.7.7/ScholarCodeCollective/cli.py
+drwxrwxrwx   0        0        0        0 2024-05-16 08:41:48.347013 ScholarCodeCollective-0.1.7.7/ScholarCodeCollective/hypergraph_binning_main/
+-rw-rw-rw-   0        0        0       43 2024-04-21 11:55:34.000000 ScholarCodeCollective-0.1.7.7/ScholarCodeCollective/hypergraph_binning_main/__init__.py
+-rw-rw-rw-   0        0        0     9020 2024-04-22 17:04:56.000000 ScholarCodeCollective-0.1.7.7/ScholarCodeCollective/hypergraph_binning_main/functions.py
+drwxrwxrwx   0        0        0        0 2024-05-16 08:41:48.350182 ScholarCodeCollective-0.1.7.7/ScholarCodeCollective/urban_boundary_delineation_main/
+-rw-rw-rw-   0        0        0       33 2024-05-16 08:06:37.000000 ScholarCodeCollective-0.1.7.7/ScholarCodeCollective/urban_boundary_delineation_main/__init__.py
+-rw-rw-rw-   0        0        0    15444 2024-05-16 07:54:57.000000 ScholarCodeCollective-0.1.7.7/ScholarCodeCollective/urban_boundary_delineation_main/greedy_algorithm.py
+drwxrwxrwx   0        0        0        0 2024-05-16 08:41:48.329263 ScholarCodeCollective-0.1.7.7/ScholarCodeCollective.egg-info/
+-rw-rw-rw-   0        0        0     1698 2024-05-16 08:41:48.000000 ScholarCodeCollective-0.1.7.7/ScholarCodeCollective.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1049 2024-05-16 08:41:48.000000 ScholarCodeCollective-0.1.7.7/ScholarCodeCollective.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-16 08:41:48.000000 ScholarCodeCollective-0.1.7.7/ScholarCodeCollective.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       41 2024-05-16 08:41:48.000000 ScholarCodeCollective-0.1.7.7/ScholarCodeCollective.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       59 2024-05-16 08:41:48.000000 ScholarCodeCollective-0.1.7.7/ScholarCodeCollective.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-16 08:41:48.355437 ScholarCodeCollective-0.1.7.7/setup.cfg
+-rw-rw-rw-   0        0        0     2145 2024-05-16 08:41:40.000000 ScholarCodeCollective-0.1.7.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-16 08:41:48.351822 ScholarCodeCollective-0.1.7.7/tests/
+-rw-rw-rw-   0        0        0     1090 2024-05-16 08:11:30.000000 ScholarCodeCollective-0.1.7.7/tests/__init__.py
```

### Comparing `ScholarCodeCollective-0.1.7.6/Community_Representatives_main/functions_python.py` & `ScholarCodeCollective-0.1.7.7/Community_Representatives_main/functions_python.py`

 * *Files identical despite different names*

### Comparing `ScholarCodeCollective-0.1.7.6/PKG-INFO` & `ScholarCodeCollective-0.1.7.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ScholarCodeCollective
-Version: 0.1.7.6
+Version: 0.1.7.7
 Summary: A collective library for the code behind several academic papers
 Home-page: https://google.com
 Author: Author Name
 Author-email: author_email@mail.com
 License: The Unlicense
 Requires-Python: >=3.9, <3.12
 Description-Content-Type: text/markdown
```

### Comparing `ScholarCodeCollective-0.1.7.6/README.md` & `ScholarCodeCollective-0.1.7.7/README.md`

 * *Files identical despite different names*

### Comparing `ScholarCodeCollective-0.1.7.6/ScholarCodeCollective/MDL_network_population_clustering_main/functions.py` & `ScholarCodeCollective-0.1.7.7/ScholarCodeCollective/MDL_network_population_clustering_main/functions.py`

 * *Files identical despite different names*

### Comparing `ScholarCodeCollective-0.1.7.6/ScholarCodeCollective/MDL_regionalization_main/functions.py` & `ScholarCodeCollective-0.1.7.7/ScholarCodeCollective/MDL_regionalization_main/functions.py`

 * *Files identical despite different names*

### Comparing `ScholarCodeCollective-0.1.7.6/ScholarCodeCollective/Network_hubs_main/functions.py` & `ScholarCodeCollective-0.1.7.7/ScholarCodeCollective/Network_hubs_main/functions.py`

 * *Files identical despite different names*

### Comparing `ScholarCodeCollective-0.1.7.6/ScholarCodeCollective/hypergraph_binning_main/functions.py` & `ScholarCodeCollective-0.1.7.7/ScholarCodeCollective/hypergraph_binning_main/functions.py`

 * *Files identical despite different names*

### Comparing `ScholarCodeCollective-0.1.7.6/ScholarCodeCollective/urban_boundary_delineation_main/greedy_algorithm.py` & `ScholarCodeCollective-0.1.7.7/ScholarCodeCollective/urban_boundary_delineation_main/greedy_algorithm.py`

 * *Files identical despite different names*

### Comparing `ScholarCodeCollective-0.1.7.6/ScholarCodeCollective.egg-info/PKG-INFO` & `ScholarCodeCollective-0.1.7.7/ScholarCodeCollective.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ScholarCodeCollective
-Version: 0.1.7.6
+Version: 0.1.7.7
 Summary: A collective library for the code behind several academic papers
 Home-page: https://google.com
 Author: Author Name
 Author-email: author_email@mail.com
 License: The Unlicense
 Requires-Python: >=3.9, <3.12
 Description-Content-Type: text/markdown
```

### Comparing `ScholarCodeCollective-0.1.7.6/ScholarCodeCollective.egg-info/SOURCES.txt` & `ScholarCodeCollective-0.1.7.7/ScholarCodeCollective.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ScholarCodeCollective-0.1.7.6/setup.py` & `ScholarCodeCollective-0.1.7.7/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 #               ["ScholarCodeCollective/Community_Representatives_main/functions.pyx"],
 #               include_dirs=[numpy.get_include()],
 #               language='c++')  
 # ]
 
 setup(
     name='ScholarCodeCollective',
-    version='0.1.7.6',
+    version='0.1.7.7',
     description='A collective library for the code behind several academic papers',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://google.com',
     author='Author Name',
     author_email='author_email@mail.com',
     license='The Unlicense',
```

### Comparing `ScholarCodeCollective-0.1.7.6/tests/__init__.py` & `ScholarCodeCollective-0.1.7.7/tests/__init__.py`

 * *Files identical despite different names*

