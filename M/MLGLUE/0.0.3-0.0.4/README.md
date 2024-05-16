# Comparing `tmp/MLGLUE-0.0.3.tar.gz` & `tmp/MLGLUE-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MLGLUE-0.0.3.tar", last modified: Fri Apr 12 08:00:49 2024, max compression
+gzip compressed data, was "MLGLUE-0.0.4.tar", last modified: Thu May 16 09:22:56 2024, max compression
```

## Comparing `MLGLUE-0.0.3.tar` & `MLGLUE-0.0.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-12 08:00:49.285384 MLGLUE-0.0.3/
--rw-rw-rw-   0        0        0     1126 2023-10-18 08:35:00.000000 MLGLUE-0.0.3/LICENSE
-drwxrwxrwx   0        0        0        0 2024-04-12 08:00:49.254135 MLGLUE-0.0.3/MLGLUE/
--rw-rw-rw-   0        0        0     9156 2024-04-12 07:57:57.000000 MLGLUE-0.0.3/MLGLUE/Likelihoods.py
--rw-rw-rw-   0        0        0    37269 2024-04-12 07:54:23.000000 MLGLUE-0.0.3/MLGLUE/MLGLUE.py
--rw-rw-rw-   0        0        0      143 2023-04-18 14:23:30.000000 MLGLUE-0.0.3/MLGLUE/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-12 08:00:49.269764 MLGLUE-0.0.3/MLGLUE.egg-info/
--rw-rw-rw-   0        0        0      691 2024-04-12 08:00:48.000000 MLGLUE-0.0.3/MLGLUE.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      233 2024-04-12 08:00:49.000000 MLGLUE-0.0.3/MLGLUE.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-12 08:00:48.000000 MLGLUE-0.0.3/MLGLUE.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       43 2024-04-12 08:00:48.000000 MLGLUE-0.0.3/MLGLUE.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-04-12 08:00:48.000000 MLGLUE-0.0.3/MLGLUE.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      691 2024-04-12 08:00:49.285384 MLGLUE-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     2184 2023-10-27 08:49:15.000000 MLGLUE-0.0.3/README.md
--rw-rw-rw-   0        0        0       42 2024-04-12 08:00:49.285384 MLGLUE-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      954 2024-04-12 07:58:52.000000 MLGLUE-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-16 09:22:56.935526 MLGLUE-0.0.4/
+-rw-rw-rw-   0        0        0     1126 2023-10-18 08:35:00.000000 MLGLUE-0.0.4/LICENSE
+drwxrwxrwx   0        0        0        0 2024-05-16 09:22:56.904191 MLGLUE-0.0.4/MLGLUE/
+-rw-rw-rw-   0        0        0     9156 2024-04-12 07:57:57.000000 MLGLUE-0.0.4/MLGLUE/Likelihoods.py
+-rw-rw-rw-   0        0        0    58001 2024-05-07 20:04:39.000000 MLGLUE-0.0.4/MLGLUE/MLGLUE.py
+-rw-rw-rw-   0        0        0      143 2024-05-06 12:14:34.000000 MLGLUE-0.0.4/MLGLUE/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-16 09:22:56.935526 MLGLUE-0.0.4/MLGLUE.egg-info/
+-rw-rw-rw-   0        0        0      691 2024-05-16 09:22:56.000000 MLGLUE-0.0.4/MLGLUE.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      233 2024-05-16 09:22:56.000000 MLGLUE-0.0.4/MLGLUE.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-16 09:22:56.000000 MLGLUE-0.0.4/MLGLUE.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       43 2024-05-16 09:22:56.000000 MLGLUE-0.0.4/MLGLUE.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-05-16 09:22:56.000000 MLGLUE-0.0.4/MLGLUE.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      691 2024-05-16 09:22:56.935526 MLGLUE-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     2184 2023-10-27 08:49:15.000000 MLGLUE-0.0.4/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-16 09:22:56.935526 MLGLUE-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      954 2024-05-16 09:22:33.000000 MLGLUE-0.0.4/setup.py
```

### Comparing `MLGLUE-0.0.3/LICENSE` & `MLGLUE-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `MLGLUE-0.0.3/MLGLUE/Likelihoods.py` & `MLGLUE-0.0.4/MLGLUE/Likelihoods.py`

 * *Files identical despite different names*

### Comparing `MLGLUE-0.0.3/MLGLUE.egg-info/PKG-INFO` & `MLGLUE-0.0.4/MLGLUE.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MLGLUE
-Version: 0.0.3
+Version: 0.0.4
 Summary: a Python implementation of the (M)ulti(l)evel (G)eneralized (L)ikelihood (U)ncertainty (E)stimation (MLGLUE) algorithm and utility functions
 Home-page: https://github.com/iGW-TU-Dresden/MLGLUE
 Author: M. G. Rudolph
 Author-email: max_gustav.rudolph@tu-dresden.de
 License: MIT
 Platform: Windows
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `MLGLUE-0.0.3/PKG-INFO` & `MLGLUE-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MLGLUE
-Version: 0.0.3
+Version: 0.0.4
 Summary: a Python implementation of the (M)ulti(l)evel (G)eneralized (L)ikelihood (U)ncertainty (E)stimation (MLGLUE) algorithm and utility functions
 Home-page: https://github.com/iGW-TU-Dresden/MLGLUE
 Author: M. G. Rudolph
 Author-email: max_gustav.rudolph@tu-dresden.de
 License: MIT
 Platform: Windows
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `MLGLUE-0.0.3/README.md` & `MLGLUE-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `MLGLUE-0.0.3/setup.py` & `MLGLUE-0.0.4/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import find_packages, setup
 
 setup(
     name = "MLGLUE",
     author = "M. G. Rudolph",
-    version = "0.0.3",
+    version = "0.0.4",
     description = "a Python implementation of the (M)ulti(l)evel (G)eneralized (L)ikelihood (U)ncertainty (E)stimation (MLGLUE) algorithm and utility functions",
     url = "https://github.com/iGW-TU-Dresden/MLGLUE",
     author_email = "max_gustav.rudolph@tu-dresden.de",
     license = "MIT",
     classifiers = [
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Science/Research",
```

