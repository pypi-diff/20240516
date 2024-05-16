# Comparing `tmp/nullity-0.0.3.tar.gz` & `tmp/nullity-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nullity-0.0.3.tar", last modified: Thu May 16 08:19:46 2024, max compression
+gzip compressed data, was "nullity-0.0.4.tar", last modified: Thu May 16 08:31:03 2024, max compression
```

## Comparing `nullity-0.0.3.tar` & `nullity-0.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 08:19:46.136546 nullity-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-16 08:19:40.000000 nullity-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2608 2024-05-16 08:19:46.136546 nullity-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2135 2024-05-16 08:19:40.000000 nullity-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 08:19:46.132546 nullity-0.0.3/nullity/
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-16 08:19:40.000000 nullity-0.0.3/nullity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18903 2024-05-16 08:19:40.000000 nullity-0.0.3/nullity/matrix.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 08:19:46.132546 nullity-0.0.3/nullity.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2608 2024-05-16 08:19:46.000000 nullity-0.0.3/nullity.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      218 2024-05-16 08:19:46.000000 nullity-0.0.3/nullity.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 08:19:46.000000 nullity-0.0.3/nullity.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-16 08:19:46.000000 nullity-0.0.3/nullity.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-16 08:19:46.000000 nullity-0.0.3/nullity.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 08:19:46.136546 nullity-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      859 2024-05-16 08:19:40.000000 nullity-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 08:31:03.233960 nullity-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-16 08:30:59.000000 nullity-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2608 2024-05-16 08:31:03.233960 nullity-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2135 2024-05-16 08:30:59.000000 nullity-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 08:31:03.233960 nullity-0.0.4/nullity/
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-16 08:30:59.000000 nullity-0.0.4/nullity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18903 2024-05-16 08:30:59.000000 nullity-0.0.4/nullity/matrix.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 08:31:03.233960 nullity-0.0.4/nullity.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2608 2024-05-16 08:31:03.000000 nullity-0.0.4/nullity.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-05-16 08:31:03.000000 nullity-0.0.4/nullity.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 08:31:03.000000 nullity-0.0.4/nullity.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-16 08:31:03.000000 nullity-0.0.4/nullity.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-16 08:31:03.000000 nullity-0.0.4/nullity.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 08:31:03.233960 nullity-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      859 2024-05-16 08:30:59.000000 nullity-0.0.4/setup.py
```

### Comparing `nullity-0.0.3/LICENSE` & `nullity-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `nullity-0.0.3/PKG-INFO` & `nullity-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nullity
-Version: 0.0.3
+Version: 0.0.4
 Summary: A package for all things linear algebra
 Author: Mihir Aggarwal
 Author-email: mail@mihiraggarwal.me
 Keywords: linear,algebra,linear algebra,linalg,lin-alg,linearalgebra,eigen,eigenvalue,eigenvector,nullity,null,null space,rank nullity
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `nullity-0.0.3/README.md` & `nullity-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `nullity-0.0.3/nullity/matrix.py` & `nullity-0.0.4/nullity/matrix.py`

 * *Files identical despite different names*

### Comparing `nullity-0.0.3/nullity.egg-info/PKG-INFO` & `nullity-0.0.4/nullity.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nullity
-Version: 0.0.3
+Version: 0.0.4
 Summary: A package for all things linear algebra
 Author: Mihir Aggarwal
 Author-email: mail@mihiraggarwal.me
 Keywords: linear,algebra,linear algebra,linalg,lin-alg,linearalgebra,eigen,eigenvalue,eigenvector,nullity,null,null space,rank nullity
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `nullity-0.0.3/setup.py` & `nullity-0.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os
 from setuptools import setup, find_packages
 
-VERSION = '0.0.3'
+VERSION = '0.0.4'
 DESCRIPTION = 'A package for all things linear algebra'
 
 here = os.path.abspath(os.path.dirname(__file__))
 with open(os.path.join(here, "README.md")) as f:
     long_description = f.read()
 
 setup(
```

