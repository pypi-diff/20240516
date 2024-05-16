# Comparing `tmp/jsepp-0.1.7.tar.gz` & `tmp/jsepp-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jsepp-0.1.7.tar", last modified: Fri Jan 12 05:39:43 2024, max compression
+gzip compressed data, was "jsepp-0.1.8.tar", last modified: Thu May 16 01:10:48 2024, max compression
```

## Comparing `jsepp-0.1.7.tar` & `jsepp-0.1.8.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-01-12 05:39:43.551847 jsepp-0.1.7/
--rw-rw-rw-   0        0        0      610 2024-01-12 05:39:43.551847 jsepp-0.1.7/PKG-INFO
--rw-rw-rw-   0        0        0      439 2023-04-12 02:46:41.000000 jsepp-0.1.7/README.md
-drwxrwxrwx   0        0        0        0 2024-01-12 05:39:43.549854 jsepp-0.1.7/jsepp/
--rw-rw-rw-   0        0        0       14 2023-04-12 06:01:14.000000 jsepp-0.1.7/jsepp/__init__.py
--rw-rw-rw-   0        0        0     1016 2024-01-12 05:38:56.000000 jsepp-0.1.7/jsepp/config.py
--rw-rw-rw-   0        0        0     3082 2023-05-06 06:46:53.000000 jsepp-0.1.7/jsepp/data.py
--rw-rw-rw-   0        0        0     2475 2023-08-28 06:19:09.000000 jsepp-0.1.7/jsepp/dbutils.py
--rw-rw-rw-   0        0        0      571 2023-05-06 04:45:51.000000 jsepp-0.1.7/jsepp/ml.py
--rw-rw-rw-   0        0        0     4102 2023-11-23 02:02:32.000000 jsepp-0.1.7/jsepp/visualize.py
-drwxrwxrwx   0        0        0        0 2024-01-12 05:39:43.551847 jsepp-0.1.7/jsepp.egg-info/
--rw-rw-rw-   0        0        0      610 2024-01-12 05:39:43.000000 jsepp-0.1.7/jsepp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      258 2024-01-12 05:39:43.000000 jsepp-0.1.7/jsepp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-01-12 05:39:43.000000 jsepp-0.1.7/jsepp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       66 2024-01-12 05:39:43.000000 jsepp-0.1.7/jsepp.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-01-12 05:39:43.000000 jsepp-0.1.7/jsepp.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-01-12 05:39:43.551847 jsepp-0.1.7/setup.cfg
--rw-rw-rw-   0        0        0      551 2024-01-12 05:39:21.000000 jsepp-0.1.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-16 01:10:48.409563 jsepp-0.1.8/
+-rw-rw-rw-   0        0        0      610 2024-05-16 01:10:48.409563 jsepp-0.1.8/PKG-INFO
+-rw-rw-rw-   0        0        0      439 2023-04-12 02:46:41.000000 jsepp-0.1.8/README.md
+drwxrwxrwx   0        0        0        0 2024-05-16 01:10:48.406573 jsepp-0.1.8/jsepp/
+-rw-rw-rw-   0        0        0       14 2023-04-12 06:01:14.000000 jsepp-0.1.8/jsepp/__init__.py
+-rw-rw-rw-   0        0        0     1016 2024-01-12 05:38:56.000000 jsepp-0.1.8/jsepp/config.py
+-rw-rw-rw-   0        0        0     3082 2023-05-06 06:46:53.000000 jsepp-0.1.8/jsepp/data.py
+-rw-rw-rw-   0        0        0     2475 2023-08-28 06:19:09.000000 jsepp-0.1.8/jsepp/dbutils.py
+-rw-rw-rw-   0        0        0      571 2023-05-06 04:45:51.000000 jsepp-0.1.8/jsepp/ml.py
+-rw-rw-rw-   0        0        0     4102 2023-11-23 02:02:32.000000 jsepp-0.1.8/jsepp/visualize.py
+-rw-rw-rw-   0        0        0     2248 2024-05-16 01:06:11.000000 jsepp-0.1.8/jsepp/water.py
+drwxrwxrwx   0        0        0        0 2024-05-16 01:10:48.408566 jsepp-0.1.8/jsepp.egg-info/
+-rw-rw-rw-   0        0        0      610 2024-05-16 01:10:48.000000 jsepp-0.1.8/jsepp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      273 2024-05-16 01:10:48.000000 jsepp-0.1.8/jsepp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-16 01:10:48.000000 jsepp-0.1.8/jsepp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       66 2024-05-16 01:10:48.000000 jsepp-0.1.8/jsepp.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-05-16 01:10:48.000000 jsepp-0.1.8/jsepp.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-16 01:10:48.409563 jsepp-0.1.8/setup.cfg
+-rw-rw-rw-   0        0        0      551 2024-05-16 01:10:45.000000 jsepp-0.1.8/setup.py
```

### Comparing `jsepp-0.1.7/PKG-INFO` & `jsepp-0.1.8/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jsepp
-Version: 0.1.7
+Version: 0.1.8
 Summary: a package for general environmental data processing
 Author: Hansen Zhao
 Author-email: zhaohs12@163.com
 
 ## JSEPP
 ### dbutils
 #### MySQLConn
```

### Comparing `jsepp-0.1.7/jsepp/config.py` & `jsepp-0.1.8/jsepp/config.py`

 * *Files identical despite different names*

### Comparing `jsepp-0.1.7/jsepp/data.py` & `jsepp-0.1.8/jsepp/data.py`

 * *Files identical despite different names*

### Comparing `jsepp-0.1.7/jsepp/dbutils.py` & `jsepp-0.1.8/jsepp/dbutils.py`

 * *Files identical despite different names*

### Comparing `jsepp-0.1.7/jsepp/ml.py` & `jsepp-0.1.8/jsepp/ml.py`

 * *Files identical despite different names*

### Comparing `jsepp-0.1.7/jsepp/visualize.py` & `jsepp-0.1.8/jsepp/visualize.py`

 * *Files identical despite different names*

### Comparing `jsepp-0.1.7/jsepp.egg-info/PKG-INFO` & `jsepp-0.1.8/jsepp.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jsepp
-Version: 0.1.7
+Version: 0.1.8
 Summary: a package for general environmental data processing
 Author: Hansen Zhao
 Author-email: zhaohs12@163.com
 
 ## JSEPP
 ### dbutils
 #### MySQLConn
```

### Comparing `jsepp-0.1.7/setup.py` & `jsepp-0.1.8/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r') as f:
     long_des = f.read()
 
 setup(
     name='jsepp',
-    version='0.1.7',
+    version='0.1.8',
     packages=find_packages(),
     install_requires=[
         'pymysql',
         'pymongo',
         'numpy',
         'pandas',
         'openpyxl',
```

