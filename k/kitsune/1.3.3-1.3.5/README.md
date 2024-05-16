# Comparing `tmp/kitsune-1.3.3.tar.gz` & `tmp/kitsune-1.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kitsune-1.3.3.tar", last modified: Wed Mar 29 03:09:01 2023, max compression
+gzip compressed data, was "kitsune-1.3.5.tar", last modified: Thu May 16 15:24:12 2024, max compression
```

## Comparing `kitsune-1.3.3.tar` & `kitsune-1.3.5.tar`

### file list

```diff
@@ -1,31 +1,30 @@
-drwxr-xr-x   0 pnatapol   (501) staff       (20)        0 2023-03-29 03:09:01.031606 kitsune-1.3.3/
--rw-r--r--   0 pnatapol   (501) staff       (20)    35128 2020-04-15 21:45:03.000000 kitsune-1.3.3/LICENSE
--rw-r--r--   0 pnatapol   (501) staff       (20)       99 2020-04-15 21:45:03.000000 kitsune-1.3.3/MANIFEST.in
--rw-r--r--   0 pnatapol   (501) staff       (20)    13027 2023-03-29 03:09:01.031996 kitsune-1.3.3/PKG-INFO
--rw-r--r--   0 pnatapol   (501) staff       (20)    12156 2023-03-29 03:01:41.000000 kitsune-1.3.3/README.md
-drwxr-xr-x   0 pnatapol   (501) staff       (20)        0 2023-03-29 03:09:01.009337 kitsune-1.3.3/kitsune/
--rw-r--r--   0 pnatapol   (501) staff       (20)        0 2023-03-29 03:01:41.000000 kitsune-1.3.3/kitsune/__init__.py
--rw-r--r--   0 pnatapol   (501) staff       (20)      599 2020-04-19 05:51:05.000000 kitsune-1.3.3/kitsune/cre_a.py
--rw-r--r--   0 pnatapol   (501) staff       (20)     1986 2023-03-29 03:01:41.000000 kitsune-1.3.3/kitsune/kitsune.py
-drwxr-xr-x   0 pnatapol   (501) staff       (20)        0 2023-03-29 03:09:01.027071 kitsune-1.3.3/kitsune/modules/
--rw-r--r--   0 pnatapol   (501) staff       (20)        0 2023-03-29 03:01:41.000000 kitsune-1.3.3/kitsune/modules/__init__.py
--rw-r--r--   0 pnatapol   (501) staff       (20)     3023 2023-03-29 03:01:41.000000 kitsune-1.3.3/kitsune/modules/acf.py
--rw-r--r--   0 pnatapol   (501) staff       (20)     3512 2023-03-29 03:01:41.000000 kitsune-1.3.3/kitsune/modules/cre.py
--rw-r--r--   0 pnatapol   (501) staff       (20)     3233 2023-03-29 03:01:41.000000 kitsune-1.3.3/kitsune/modules/dmatrix.py
--rw-r--r--   0 pnatapol   (501) staff       (20)     7852 2023-03-29 03:01:41.000000 kitsune-1.3.3/kitsune/modules/kitsunejf.py
--rw-r--r--   0 pnatapol   (501) staff       (20)    20130 2023-03-29 03:01:41.000000 kitsune-1.3.3/kitsune/modules/kopt.py
--rw-r--r--   0 pnatapol   (501) staff       (20)     2146 2023-03-29 03:01:41.000000 kitsune-1.3.3/kitsune/modules/ofc.py
-drwxr-xr-x   0 pnatapol   (501) staff       (20)        0 2023-03-29 03:09:01.030489 kitsune-1.3.3/kitsune/tests/
--rw-r--r--   0 pnatapol   (501) staff       (20)        0 2020-04-15 21:45:03.000000 kitsune-1.3.3/kitsune/tests/__init__.py
--rw-r--r--   0 pnatapol   (501) staff       (20)      204 2020-04-15 21:45:03.000000 kitsune-1.3.3/kitsune/tests/test_kitsunejf.py
--rw-r--r--   0 pnatapol   (501) staff       (20)      130 2020-04-15 21:45:03.000000 kitsune-1.3.3/kitsune/tests/test_main.py
-drwxr-xr-x   0 pnatapol   (501) staff       (20)        0 2023-03-29 03:09:01.017552 kitsune-1.3.3/kitsune.egg-info/
--rw-r--r--   0 pnatapol   (501) staff       (20)    13027 2023-03-29 03:09:00.000000 kitsune-1.3.3/kitsune.egg-info/PKG-INFO
--rw-r--r--   0 pnatapol   (501) staff       (20)      584 2023-03-29 03:09:00.000000 kitsune-1.3.3/kitsune.egg-info/SOURCES.txt
--rw-r--r--   0 pnatapol   (501) staff       (20)        1 2023-03-29 03:09:00.000000 kitsune-1.3.3/kitsune.egg-info/dependency_links.txt
--rw-r--r--   0 pnatapol   (501) staff       (20)       49 2023-03-29 03:09:00.000000 kitsune-1.3.3/kitsune.egg-info/entry_points.txt
--rw-r--r--   0 pnatapol   (501) staff       (20)        1 2020-04-16 00:50:06.000000 kitsune-1.3.3/kitsune.egg-info/not-zip-safe
--rw-r--r--   0 pnatapol   (501) staff       (20)       38 2023-03-29 03:09:00.000000 kitsune-1.3.3/kitsune.egg-info/requires.txt
--rw-r--r--   0 pnatapol   (501) staff       (20)        8 2023-03-29 03:09:00.000000 kitsune-1.3.3/kitsune.egg-info/top_level.txt
--rw-r--r--   0 pnatapol   (501) staff       (20)      242 2023-03-29 03:09:01.033604 kitsune-1.3.3/setup.cfg
--rw-r--r--   0 pnatapol   (501) staff       (20)     1725 2023-03-29 03:01:41.000000 kitsune-1.3.3/setup.py
+drwxr-xr-x   0 natapolpornputtapong   (501) staff       (20)        0 2024-05-16 15:24:12.071582 kitsune-1.3.5/
+-rw-r--r--   0 natapolpornputtapong   (501) staff       (20)    35128 2023-02-22 16:53:08.000000 kitsune-1.3.5/LICENSE
+-rw-r--r--   0 natapolpornputtapong   (501) staff       (20)       99 2023-02-22 16:53:08.000000 kitsune-1.3.5/MANIFEST.in
+-rw-r--r--   0 natapolpornputtapong   (501) staff       (20)    13110 2024-05-16 15:24:12.071281 kitsune-1.3.5/PKG-INFO
+-rw-r--r--   0 natapolpornputtapong   (501) staff       (20)    12156 2024-05-16 15:13:10.000000 kitsune-1.3.5/README.md
+drwxr-xr-x   0 natapolpornputtapong   (501) staff       (20)        0 2024-05-16 15:24:12.060258 kitsune-1.3.5/kitsune/
+-rw-r--r--   0 natapolpornputtapong   (501) staff       (20)        0 2023-02-22 16:53:08.000000 kitsune-1.3.5/kitsune/__init__.py
+-rw-r--r--   0 natapolpornputtapong   (501) staff       (20)     1986 2024-05-16 15:19:08.000000 kitsune-1.3.5/kitsune/kitsune.py
+drwxr-xr-x   0 natapolpornputtapong   (501) staff       (20)        0 2024-05-16 15:24:12.069595 kitsune-1.3.5/kitsune/modules/
+-rw-r--r--   0 natapolpornputtapong   (501) staff       (20)        0 2023-02-22 16:53:08.000000 kitsune-1.3.5/kitsune/modules/__init__.py
+-rw-r--r--   0 natapolpornputtapong   (501) staff       (20)     3023 2024-05-16 15:13:10.000000 kitsune-1.3.5/kitsune/modules/acf.py
+-rw-r--r--   0 natapolpornputtapong   (501) staff       (20)     3512 2024-05-16 15:13:10.000000 kitsune-1.3.5/kitsune/modules/cre.py
+-rw-r--r--   0 natapolpornputtapong   (501) staff       (20)     3233 2024-05-16 15:13:10.000000 kitsune-1.3.5/kitsune/modules/dmatrix.py
+-rw-r--r--   0 natapolpornputtapong   (501) staff       (20)     8094 2024-05-16 15:17:03.000000 kitsune-1.3.5/kitsune/modules/kitsunejf.py
+-rw-r--r--   0 natapolpornputtapong   (501) staff       (20)    20130 2024-05-16 15:13:10.000000 kitsune-1.3.5/kitsune/modules/kopt.py
+-rw-r--r--   0 natapolpornputtapong   (501) staff       (20)     2146 2024-05-16 15:13:10.000000 kitsune-1.3.5/kitsune/modules/ofc.py
+drwxr-xr-x   0 natapolpornputtapong   (501) staff       (20)        0 2024-05-16 15:24:12.070505 kitsune-1.3.5/kitsune/tests/
+-rw-r--r--   0 natapolpornputtapong   (501) staff       (20)        0 2023-02-22 16:53:08.000000 kitsune-1.3.5/kitsune/tests/__init__.py
+-rw-r--r--   0 natapolpornputtapong   (501) staff       (20)      204 2023-02-22 16:53:08.000000 kitsune-1.3.5/kitsune/tests/test_kitsunejf.py
+-rw-r--r--   0 natapolpornputtapong   (501) staff       (20)      130 2023-02-22 16:53:08.000000 kitsune-1.3.5/kitsune/tests/test_main.py
+drwxr-xr-x   0 natapolpornputtapong   (501) staff       (20)        0 2024-05-16 15:24:12.070919 kitsune-1.3.5/kitsune.egg-info/
+-rw-r--r--   0 natapolpornputtapong   (501) staff       (20)    13110 2024-05-16 15:24:12.000000 kitsune-1.3.5/kitsune.egg-info/PKG-INFO
+-rw-r--r--   0 natapolpornputtapong   (501) staff       (20)      567 2024-05-16 15:24:12.000000 kitsune-1.3.5/kitsune.egg-info/SOURCES.txt
+-rw-r--r--   0 natapolpornputtapong   (501) staff       (20)        1 2024-05-16 15:24:12.000000 kitsune-1.3.5/kitsune.egg-info/dependency_links.txt
+-rw-r--r--   0 natapolpornputtapong   (501) staff       (20)       49 2024-05-16 15:24:12.000000 kitsune-1.3.5/kitsune.egg-info/entry_points.txt
+-rw-r--r--   0 natapolpornputtapong   (501) staff       (20)        1 2023-02-22 17:02:50.000000 kitsune-1.3.5/kitsune.egg-info/not-zip-safe
+-rw-r--r--   0 natapolpornputtapong   (501) staff       (20)       38 2024-05-16 15:24:12.000000 kitsune-1.3.5/kitsune.egg-info/requires.txt
+-rw-r--r--   0 natapolpornputtapong   (501) staff       (20)        8 2024-05-16 15:24:12.000000 kitsune-1.3.5/kitsune.egg-info/top_level.txt
+-rw-r--r--   0 natapolpornputtapong   (501) staff       (20)      242 2024-05-16 15:24:12.072726 kitsune-1.3.5/setup.cfg
+-rw-r--r--   0 natapolpornputtapong   (501) staff       (20)     1725 2023-02-22 16:53:08.000000 kitsune-1.3.5/setup.py
```

### Comparing `kitsune-1.3.3/LICENSE` & `kitsune-1.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `kitsune-1.3.3/PKG-INFO` & `kitsune-1.3.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kitsune
-Version: 1.3.3
+Version: 1.3.5
 Summary: A toolkit for evaluation of the lenght of k-mer in a given genome dataset for alignment-free phylogenimic analysis
 Home-page: https://github.com/natapol/kitsune
 Download-URL: https://pypi.org/project/kitsune/
 Author: Natapol Pornputtapong
 Author-email: natapol.por@gmail.com
 License: GPL-3.0 License
 Keywords: bioinformatics,kitsune
@@ -14,14 +14,17 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS :: MacOS X
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: numpy>=1.1.0
+Requires-Dist: scipy>=0.18.1
+Requires-Dist: tqdm>=4.32
 
 # KITSUNE: K-mer-length Iterative Selection for UNbiased Ecophylogenomics
 
 <img src="https://github.com/natapol/kitsune/blob/master/logoKITSUNE.png" width="40%">
 
 [![PyPI version](https://badge.fury.io/py/kitsune.svg)](https://badge.fury.io/py/kitsune)
 ![Upload Python Package](https://github.com/natapol/kitsune/workflows/Upload%20Python%20Package/badge.svg)
```

### Comparing `kitsune-1.3.3/README.md` & `kitsune-1.3.5/README.md`

 * *Files identical despite different names*

### Comparing `kitsune-1.3.3/kitsune/kitsune.py` & `kitsune-1.3.5/kitsune/kitsune.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 KITSUNE: K-mer-length Iterative Selection for UNbiased Ecophylogenomics
 """
 
 import importlib
 import sys
 
 __author__ = "Natapol Pornputtapong (natapol.p@chula.ac.th)"
-__version__ = "1.3.3"
-__date__ = "Mar 15, 2023"
+__version__ = "1.3.5"
+__date__ = "May 16, 2024"
 
 # Define the set of commands with help messages
 COMMANDS = {
     "acf": "Compute average number of common features between signatures",
     "cre": "Compute cumulative relative entropy",
     "dmatrix": "Compute distance matrix",
     "kopt": ("Compute recommended choice (optimal) of kmer within a given "
```

### Comparing `kitsune-1.3.3/kitsune/modules/acf.py` & `kitsune-1.3.5/kitsune/modules/acf.py`

 * *Files identical despite different names*

### Comparing `kitsune-1.3.3/kitsune/modules/cre.py` & `kitsune-1.3.5/kitsune/modules/cre.py`

 * *Files identical despite different names*

### Comparing `kitsune-1.3.3/kitsune/modules/dmatrix.py` & `kitsune-1.3.5/kitsune/modules/dmatrix.py`

 * *Files identical despite different names*

### Comparing `kitsune-1.3.3/kitsune/modules/kitsunejf.py` & `kitsune-1.3.5/kitsune/modules/kitsunejf.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,18 +2,21 @@
 import math
 import os
 import platform
 import subprocess
 import tempfile
 import warnings
 
+from pkg_resources import packaging
+
 from shutil import which
 
 import numpy as np
 
+import scipy
 from scipy.stats import chi2
 from scipy.spatial import distance
 from scipy.special import loggamma
 
 if platform.system() not in ['Darwin', 'Linux']:
     raise Exception("{} OS is not supported.".format(platform.system()))
 
@@ -145,22 +148,27 @@
 ]
 
 BOOLEAN_DISTANCE = [
     distance.dice,
     distance.hamming,
     distance.jaccard,
     jaccarddistp,
-    distance.kulsinski,
+    distance.kulczynski1,
     distance.rogerstanimoto,
     distance.russellrao,
     distance.sokalmichener,
     distance.sokalsneath,
     distance.yule
 ]
 
+if  packaging.version.parse(scipy.__version__) >= packaging.version.parse("1.8.0"):
+    BOOLEAN_DISTANCE.append(distance.kulczynski1)
+else:
+    BOOLEAN_DISTANCE.append(distance.kulsinski)
+
 PROB_DISTANCE = [
     distance.jensenshannon,
     euclidean_of_frequency
 ]
 
 
 class Kmercount(dict):
@@ -227,15 +235,15 @@
                         canonical
                     )
                 )
 
         datadict = dict()
 
         try:
-            for line in dumpdata.split('\n'):
+            for line in dumpdata.splitlines():
                 dat = line.rstrip().split(' ')
                 datadict[dat[0]] = int(dat[1])
 
         except ValueError:
             raise JellyFishError("Bloom filter file is truncated.")
 
         super(Kmercount, self).__init__(datadict)
```

### Comparing `kitsune-1.3.3/kitsune/modules/kopt.py` & `kitsune-1.3.5/kitsune/modules/kopt.py`

 * *Files identical despite different names*

### Comparing `kitsune-1.3.3/kitsune/modules/ofc.py` & `kitsune-1.3.5/kitsune/modules/ofc.py`

 * *Files identical despite different names*

### Comparing `kitsune-1.3.3/kitsune.egg-info/PKG-INFO` & `kitsune-1.3.5/kitsune.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kitsune
-Version: 1.3.3
+Version: 1.3.5
 Summary: A toolkit for evaluation of the lenght of k-mer in a given genome dataset for alignment-free phylogenimic analysis
 Home-page: https://github.com/natapol/kitsune
 Download-URL: https://pypi.org/project/kitsune/
 Author: Natapol Pornputtapong
 Author-email: natapol.por@gmail.com
 License: GPL-3.0 License
 Keywords: bioinformatics,kitsune
@@ -14,14 +14,17 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS :: MacOS X
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: numpy>=1.1.0
+Requires-Dist: scipy>=0.18.1
+Requires-Dist: tqdm>=4.32
 
 # KITSUNE: K-mer-length Iterative Selection for UNbiased Ecophylogenomics
 
 <img src="https://github.com/natapol/kitsune/blob/master/logoKITSUNE.png" width="40%">
 
 [![PyPI version](https://badge.fury.io/py/kitsune.svg)](https://badge.fury.io/py/kitsune)
 ![Upload Python Package](https://github.com/natapol/kitsune/workflows/Upload%20Python%20Package/badge.svg)
```

### Comparing `kitsune-1.3.3/kitsune.egg-info/SOURCES.txt` & `kitsune-1.3.5/kitsune.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 LICENSE
 MANIFEST.in
 README.md
 setup.cfg
 setup.py
 kitsune/__init__.py
-kitsune/cre_a.py
 kitsune/kitsune.py
 kitsune.egg-info/PKG-INFO
 kitsune.egg-info/SOURCES.txt
 kitsune.egg-info/dependency_links.txt
 kitsune.egg-info/entry_points.txt
 kitsune.egg-info/not-zip-safe
 kitsune.egg-info/requires.txt
```

### Comparing `kitsune-1.3.3/setup.py` & `kitsune-1.3.5/setup.py`

 * *Files identical despite different names*

