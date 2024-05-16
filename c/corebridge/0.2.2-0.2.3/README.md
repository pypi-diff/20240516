# Comparing `tmp/corebridge-0.2.2.tar.gz` & `tmp/corebridge-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "corebridge-0.2.2.tar", last modified: Thu May 16 17:52:05 2024, max compression
+gzip compressed data, was "corebridge-0.2.3.tar", last modified: Thu May 16 17:55:05 2024, max compression
```

## Comparing `corebridge-0.2.2.tar` & `corebridge-0.2.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 fenke     (1000) users      (100)        0 2024-05-16 17:52:05.875648 corebridge-0.2.2/
--rw-r--r--   0 fenke     (1000) users      (100)    11337 2024-01-31 12:54:47.000000 corebridge-0.2.2/LICENSE
--rw-r--r--   0 fenke     (1000) users      (100)      111 2024-01-31 12:54:47.000000 corebridge-0.2.2/MANIFEST.in
--rw-r--r--   0 fenke     (1000) users      (100)     2655 2024-05-16 17:52:05.875648 corebridge-0.2.2/PKG-INFO
--rw-r--r--   0 fenke     (1000) users      (100)     1887 2024-05-03 10:28:01.000000 corebridge-0.2.2/README.md
-drwxr-xr-x   0 fenke     (1000) users      (100)        0 2024-05-16 17:52:05.875648 corebridge-0.2.2/corebridge/
--rw-r--r--   0 fenke     (1000) users      (100)     4615 2024-05-16 17:50:44.000000 corebridge-0.2.2/corebridge/__init__.py
--rw-r--r--   0 fenke     (1000) users      (100)     2865 2024-05-16 17:50:44.000000 corebridge-0.2.2/corebridge/_modidx.py
--rw-r--r--   0 fenke     (1000) users      (100)     4612 2024-05-16 17:50:44.000000 corebridge-0.2.2/corebridge/aicorebridge.py
--rw-r--r--   0 fenke     (1000) users      (100)     4464 2024-05-16 17:50:44.000000 corebridge-0.2.2/corebridge/core.py
-drwxr-xr-x   0 fenke     (1000) users      (100)        0 2024-05-16 17:52:05.875648 corebridge-0.2.2/corebridge.egg-info/
--rw-r--r--   0 fenke     (1000) users      (100)     2655 2024-05-16 17:52:05.000000 corebridge-0.2.2/corebridge.egg-info/PKG-INFO
--rw-r--r--   0 fenke     (1000) users      (100)      381 2024-05-16 17:52:05.000000 corebridge-0.2.2/corebridge.egg-info/SOURCES.txt
--rw-r--r--   0 fenke     (1000) users      (100)        1 2024-05-16 17:52:05.000000 corebridge-0.2.2/corebridge.egg-info/dependency_links.txt
--rw-r--r--   0 fenke     (1000) users      (100)       42 2024-05-16 17:52:05.000000 corebridge-0.2.2/corebridge.egg-info/entry_points.txt
--rw-r--r--   0 fenke     (1000) users      (100)        1 2024-01-31 15:42:47.000000 corebridge-0.2.2/corebridge.egg-info/not-zip-safe
--rw-r--r--   0 fenke     (1000) users      (100)      273 2024-05-16 17:52:05.000000 corebridge-0.2.2/corebridge.egg-info/requires.txt
--rw-r--r--   0 fenke     (1000) users      (100)       11 2024-05-16 17:52:05.000000 corebridge-0.2.2/corebridge.egg-info/top_level.txt
--rw-r--r--   0 fenke     (1000) users      (100)     1194 2024-05-16 17:50:53.000000 corebridge-0.2.2/settings.ini
--rw-r--r--   0 fenke     (1000) users      (100)       38 2024-05-16 17:52:05.875648 corebridge-0.2.2/setup.cfg
--rw-r--r--   0 fenke     (1000) users      (100)     2596 2024-01-31 12:54:47.000000 corebridge-0.2.2/setup.py
+drwxr-xr-x   0 fenke     (1000) users      (100)        0 2024-05-16 17:55:05.797267 corebridge-0.2.3/
+-rw-r--r--   0 fenke     (1000) users      (100)    11337 2024-01-31 12:54:47.000000 corebridge-0.2.3/LICENSE
+-rw-r--r--   0 fenke     (1000) users      (100)      111 2024-01-31 12:54:47.000000 corebridge-0.2.3/MANIFEST.in
+-rw-r--r--   0 fenke     (1000) users      (100)     2655 2024-05-16 17:55:05.797267 corebridge-0.2.3/PKG-INFO
+-rw-r--r--   0 fenke     (1000) users      (100)     1887 2024-05-03 10:28:01.000000 corebridge-0.2.3/README.md
+drwxr-xr-x   0 fenke     (1000) users      (100)        0 2024-05-16 17:55:05.797267 corebridge-0.2.3/corebridge/
+-rw-r--r--   0 fenke     (1000) users      (100)       22 2024-05-16 17:54:56.000000 corebridge-0.2.3/corebridge/__init__.py
+-rw-r--r--   0 fenke     (1000) users      (100)     2865 2024-05-16 17:54:56.000000 corebridge-0.2.3/corebridge/_modidx.py
+-rw-r--r--   0 fenke     (1000) users      (100)     4612 2024-05-16 17:54:56.000000 corebridge-0.2.3/corebridge/aicorebridge.py
+-rw-r--r--   0 fenke     (1000) users      (100)     4464 2024-05-16 17:54:56.000000 corebridge-0.2.3/corebridge/core.py
+drwxr-xr-x   0 fenke     (1000) users      (100)        0 2024-05-16 17:55:05.797267 corebridge-0.2.3/corebridge.egg-info/
+-rw-r--r--   0 fenke     (1000) users      (100)     2655 2024-05-16 17:55:05.000000 corebridge-0.2.3/corebridge.egg-info/PKG-INFO
+-rw-r--r--   0 fenke     (1000) users      (100)      381 2024-05-16 17:55:05.000000 corebridge-0.2.3/corebridge.egg-info/SOURCES.txt
+-rw-r--r--   0 fenke     (1000) users      (100)        1 2024-05-16 17:55:05.000000 corebridge-0.2.3/corebridge.egg-info/dependency_links.txt
+-rw-r--r--   0 fenke     (1000) users      (100)       42 2024-05-16 17:55:05.000000 corebridge-0.2.3/corebridge.egg-info/entry_points.txt
+-rw-r--r--   0 fenke     (1000) users      (100)        1 2024-01-31 15:42:47.000000 corebridge-0.2.3/corebridge.egg-info/not-zip-safe
+-rw-r--r--   0 fenke     (1000) users      (100)      279 2024-05-16 17:55:05.000000 corebridge-0.2.3/corebridge.egg-info/requires.txt
+-rw-r--r--   0 fenke     (1000) users      (100)       11 2024-05-16 17:55:05.000000 corebridge-0.2.3/corebridge.egg-info/top_level.txt
+-rw-r--r--   0 fenke     (1000) users      (100)     1200 2024-05-16 17:54:41.000000 corebridge-0.2.3/settings.ini
+-rw-r--r--   0 fenke     (1000) users      (100)       38 2024-05-16 17:55:05.797267 corebridge-0.2.3/setup.cfg
+-rw-r--r--   0 fenke     (1000) users      (100)     2596 2024-01-31 12:54:47.000000 corebridge-0.2.3/setup.py
```

### Comparing `corebridge-0.2.2/LICENSE` & `corebridge-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `corebridge-0.2.2/PKG-INFO` & `corebridge-0.2.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: corebridge
-Version: 0.2.2
+Version: 0.2.3
 Summary: Bridge for Stactics AICore
 Home-page: https://github.com/fenke/corebridge
 Author: Fenke Meijer
 Author-email: fenkemeijer@gmail.com
 License: Apache Software License 2.0
-Keywords: nbdev jupyter notebook python
+Keywords: python aicore stactics whysor
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `corebridge-0.2.2/README.md` & `corebridge-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `corebridge-0.2.2/corebridge/__init__.py` & `corebridge-0.2.3/corebridge/aicorebridge.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-__version__ = "0.2.1"
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../nbs/01_aicorebridge.ipynb.
 
 # %% auto 0
 __all__ = ['syslog', 'AICoreModule']
 
 # %% ../nbs/01_aicorebridge.ipynb 4
 import typing
@@ -10,14 +9,15 @@
 import inspect
 import datetime
 import json
 import pandas as pd
 import numpy as np
 
 from fastcore.basics import patch_to, patch
+from core import *
 
 
 # %% ../nbs/01_aicorebridge.ipynb 5
 syslog = logging.getLogger(__name__)
 
 # %% ../nbs/01_aicorebridge.ipynb 6
 try:
```

### Comparing `corebridge-0.2.2/corebridge/_modidx.py` & `corebridge-0.2.3/corebridge/_modidx.py`

 * *Files identical despite different names*

### Comparing `corebridge-0.2.2/corebridge/core.py` & `corebridge-0.2.3/corebridge/core.py`

 * *Files identical despite different names*

### Comparing `corebridge-0.2.2/corebridge.egg-info/PKG-INFO` & `corebridge-0.2.3/corebridge.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: corebridge
-Version: 0.2.2
+Version: 0.2.3
 Summary: Bridge for Stactics AICore
 Home-page: https://github.com/fenke/corebridge
 Author: Fenke Meijer
 Author-email: fenkemeijer@gmail.com
 License: Apache Software License 2.0
-Keywords: nbdev jupyter notebook python
+Keywords: python aicore stactics whysor
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `corebridge-0.2.2/settings.ini` & `corebridge-0.2.3/settings.ini`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [DEFAULT]
 # All sections below are required unless otherwise specified.
 # See https://github.com/fastai/nbdev/blob/master/settings.ini for examples.
 
 ### Python library ###
 repo = corebridge
 lib_name = %(repo)s
-version = 0.2.2
+version = 0.2.3
 min_python = 3.7
 license = apache2
 black_formatting = False
 
 ### nbdev ###
 doc_path = _docs
 lib_path = corebridge
@@ -28,16 +28,16 @@
 
 ### PyPI ###
 audience = Developers
 author = Fenke Meijer
 author_email = fenkemeijer@gmail.com
 copyright = 2023 onwards, %(author)s
 description = Bridge for Stactics AICore
-keywords = nbdev jupyter notebook python
+keywords = python aicore stactics whysor
 language = English
 status = 3
 user = fenke
 
 ### Optional ###
 requirements = python-dateutil pytz numpy pandas scipy scikit-learn fastcore twine
-dev_requirements = python-dateutil pytz numpy pyarrow pandas scipy scikit-learn fastcore jupyter ipywidgets jupyterlab>4 jupyter_contrib_nbextensions jupyterlab-git jupyterlab-quarto nbdev aiohttp asyncpg apscheduler
+dev_requirements = python-dateutil pytz numpy pyarrow pandas scipy scikit-learn fastcore jupyter ipywidgets jupyterlab>4 jupyter_contrib_nbextensions jupyterlab-git jupyterlab-quarto nbdev aiohttp asyncpg apscheduler twine
 # console_scripts =
```

### Comparing `corebridge-0.2.2/setup.py` & `corebridge-0.2.3/setup.py`

 * *Files identical despite different names*

