# Comparing `tmp/astro_otter-0.0.1.tar.gz` & `tmp/astro_otter-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "astro_otter-0.0.1.tar", last modified: Sat May 11 01:05:14 2024, max compression
+gzip compressed data, was "astro_otter-0.0.2.tar", last modified: Thu May 16 18:43:37 2024, max compression
```

## Comparing `astro_otter-0.0.1.tar` & `astro_otter-0.0.2.tar`

### file list

```diff
@@ -1,29 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 01:05:14.064441 astro_otter-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-11 01:05:07.000000 astro_otter-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    31845 2024-05-11 01:05:14.064441 astro_otter-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    29546 2024-05-11 01:05:07.000000 astro_otter-0.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1838 2024-05-11 01:05:07.000000 astro_otter-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-11 01:05:14.064441 astro_otter-0.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 01:05:14.060441 astro_otter-0.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 01:05:14.064441 astro_otter-0.0.1/src/astro_otter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    31845 2024-05-11 01:05:14.000000 astro_otter-0.0.1/src/astro_otter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      525 2024-05-11 01:05:14.000000 astro_otter-0.0.1/src/astro_otter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-11 01:05:14.000000 astro_otter-0.0.1/src/astro_otter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-11 01:05:14.000000 astro_otter-0.0.1/src/astro_otter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-11 01:05:14.000000 astro_otter-0.0.1/src/astro_otter.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 01:05:14.060441 astro_otter-0.0.1/src/otter/
--rw-r--r--   0 runner    (1001) docker     (127)      339 2024-05-11 01:05:07.000000 astro_otter-0.0.1/src/otter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-11 01:05:07.000000 astro_otter-0.0.1/src/otter/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)      494 2024-05-11 01:05:07.000000 astro_otter-0.0.1/src/otter/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 01:05:14.064441 astro_otter-0.0.1/src/otter/io/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 01:05:07.000000 astro_otter-0.0.1/src/otter/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17038 2024-05-11 01:05:07.000000 astro_otter-0.0.1/src/otter/io/otter.py
--rw-r--r--   0 runner    (1001) docker     (127)    31165 2024-05-11 01:05:07.000000 astro_otter-0.0.1/src/otter/io/transient.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 01:05:14.064441 astro_otter-0.0.1/src/otter/plotter/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 01:05:07.000000 astro_otter-0.0.1/src/otter/plotter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2083 2024-05-11 01:05:07.000000 astro_otter-0.0.1/src/otter/plotter/otter_plotter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2861 2024-05-11 01:05:07.000000 astro_otter-0.0.1/src/otter/plotter/plotter.py
--rw-r--r--   0 runner    (1001) docker     (127)    13600 2024-05-11 01:05:07.000000 astro_otter-0.0.1/src/otter/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 01:05:14.064441 astro_otter-0.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-05-11 01:05:07.000000 astro_otter-0.0.1/tests/test_package.py
--rw-r--r--   0 runner    (1001) docker     (127)    34081 2024-05-11 01:05:07.000000 astro_otter-0.0.1/tests/test_transient.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:43:37.699491 astro_otter-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-16 18:43:32.000000 astro_otter-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    32269 2024-05-16 18:43:37.699491 astro_otter-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    29755 2024-05-16 18:43:32.000000 astro_otter-0.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2026 2024-05-16 18:43:32.000000 astro_otter-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 18:43:37.699491 astro_otter-0.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:43:37.695491 astro_otter-0.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:43:37.699491 astro_otter-0.0.2/src/astro_otter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    32269 2024-05-16 18:43:37.000000 astro_otter-0.0.2/src/astro_otter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      589 2024-05-16 18:43:37.000000 astro_otter-0.0.2/src/astro_otter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 18:43:37.000000 astro_otter-0.0.2/src/astro_otter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-16 18:43:37.000000 astro_otter-0.0.2/src/astro_otter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-16 18:43:37.000000 astro_otter-0.0.2/src/astro_otter.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:43:37.699491 astro_otter-0.0.2/src/otter/
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-05-16 18:43:32.000000 astro_otter-0.0.2/src/otter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-16 18:43:32.000000 astro_otter-0.0.2/src/otter/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      938 2024-05-16 18:43:32.000000 astro_otter-0.0.2/src/otter/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:43:37.699491 astro_otter-0.0.2/src/otter/io/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 18:43:32.000000 astro_otter-0.0.2/src/otter/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17608 2024-05-16 18:43:32.000000 astro_otter-0.0.2/src/otter/io/otter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33621 2024-05-16 18:43:32.000000 astro_otter-0.0.2/src/otter/io/transient.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:43:37.699491 astro_otter-0.0.2/src/otter/plotter/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 18:43:32.000000 astro_otter-0.0.2/src/otter/plotter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2091 2024-05-16 18:43:32.000000 astro_otter-0.0.2/src/otter/plotter/otter_plotter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2896 2024-05-16 18:43:32.000000 astro_otter-0.0.2/src/otter/plotter/plotter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15163 2024-05-16 18:43:32.000000 astro_otter-0.0.2/src/otter/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:43:37.699491 astro_otter-0.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-05-16 18:43:32.000000 astro_otter-0.0.2/tests/test_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6472 2024-05-16 18:43:32.000000 astro_otter-0.0.2/tests/test_otter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-05-16 18:43:32.000000 astro_otter-0.0.2/tests/test_package.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38808 2024-05-16 18:43:32.000000 astro_otter-0.0.2/tests/test_transient.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-05-16 18:43:32.000000 astro_otter-0.0.2/tests/test_util.py
```

### Comparing `astro_otter-0.0.1/LICENSE` & `astro_otter-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `astro_otter-0.0.1/PKG-INFO` & `astro_otter-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astro-otter
-Version: 0.0.1
+Version: 0.0.2
 Author-email: Noah Franz <nfranz@arizona.edu>
 License: MIT License
         
         Copyright (c) 2023 Noah Franz
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -46,14 +46,21 @@
 Requires-Dist: matplotlib
 Requires-Dist: plotly
 Requires-Dist: astroquery
 Requires-Dist: synphot
 Requires-Dist: ads
 Requires-Dist: ruff
 Requires-Dist: pre-commit
+Requires-Dist: Sphinx>=3.0.0
+Requires-Dist: myst_parser>=0.13
+Requires-Dist: nbsphinx>=0.9.1
+Requires-Dist: sphinx-book-theme>=0.0.33
+Requires-Dist: sphinx_copybutton
+Requires-Dist: autodoc
+Requires-Dist: ipykernel
 
 # OTTER API
 ### **O**pen mul**T**iwavelength **T**ransient **E**vent **R**epository
 
 A Python API for the OTTER.
 
 [actions-badge]:            https://github.com/astro-otter/otter/workflows/CI/badge.svg
@@ -62,26 +69,28 @@
 [black-link]:               https://github.com/psf/black
 [conda-badge]:              https://img.shields.io/conda/vn/conda-forge/hepfile
 [conda-link]:               https://github.com/conda-forge/hepfile-feedstock
 [github-discussions-badge]: https://img.shields.io/static/v1?label=Discussions&message=Ask&color=blue&logo=github
 [github-discussions-link]:  https://github.com/mattbellis/hepfile/discussions
 [gitter-badge]:             https://badges.gitter.im/https://github.com/mattbellis/hepfile/community.svg
 [gitter-link]:              https://gitter.im/https://github.com/mattbellis/hepfile/community?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge
-[pypi-link]:                https://pypi.org/project/hepfile/
-[pypi-platforms]:           https://img.shields.io/pypi/pyversions/hepfile
-[pypi-version]:             https://badge.fury.io/py/hepfile.svg
+[pypi-link]:                https://pypi.org/project/astro-otter/
+[pypi-platforms]:           https://img.shields.io/pypi/pyversions/astro-otter
+[pypi-version]:             https://badge.fury.io/py/astro-otter.svg
 [rtd-badge]:                https://readthedocs.org/projects/otter/badge/?version=latest
 [rtd-link]:                 https://otter.readthedocs.io/en/latest/?badge=latest
 [sk-badge]:                 https://scikit-hep.org/assets/images/Scikit--HEP-Project-blue.svg
 [ruff-badge]:               https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json
 [ruff-link]:                https://github.com/astral-sh/ruff
 [codecov-badge]:            https://codecov.io/gh/astro-otter/otter/graph/badge.svg?token=BtCerOdTc0
 [codecov-link]:             https://codecov.io/gh/astro-otter/otter
 
+[![Documentation Status](https://readthedocs.org/projects/astro-otter/badge/?version=latest)](https://astro-otter.readthedocs.io/en/latest/?badge=latest)
 [![Actions Status][actions-badge]][actions-link]
+[![PyPI version][pypi-version]][pypi-link]
 [![Linting: Ruff][ruff-badge]][ruff-link]
 [![codecov][codecov-badge]][codecov-link]
 
 ## Installation
 To install the OTTER API use
 ```
 git clone https://github.com/astro-otter/otter.git
```

### Comparing `astro_otter-0.0.1/README.md` & `astro_otter-0.0.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -9,26 +9,28 @@
 [black-link]:               https://github.com/psf/black
 [conda-badge]:              https://img.shields.io/conda/vn/conda-forge/hepfile
 [conda-link]:               https://github.com/conda-forge/hepfile-feedstock
 [github-discussions-badge]: https://img.shields.io/static/v1?label=Discussions&message=Ask&color=blue&logo=github
 [github-discussions-link]:  https://github.com/mattbellis/hepfile/discussions
 [gitter-badge]:             https://badges.gitter.im/https://github.com/mattbellis/hepfile/community.svg
 [gitter-link]:              https://gitter.im/https://github.com/mattbellis/hepfile/community?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge
-[pypi-link]:                https://pypi.org/project/hepfile/
-[pypi-platforms]:           https://img.shields.io/pypi/pyversions/hepfile
-[pypi-version]:             https://badge.fury.io/py/hepfile.svg
+[pypi-link]:                https://pypi.org/project/astro-otter/
+[pypi-platforms]:           https://img.shields.io/pypi/pyversions/astro-otter
+[pypi-version]:             https://badge.fury.io/py/astro-otter.svg
 [rtd-badge]:                https://readthedocs.org/projects/otter/badge/?version=latest
 [rtd-link]:                 https://otter.readthedocs.io/en/latest/?badge=latest
 [sk-badge]:                 https://scikit-hep.org/assets/images/Scikit--HEP-Project-blue.svg
 [ruff-badge]:               https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json
 [ruff-link]:                https://github.com/astral-sh/ruff
 [codecov-badge]:            https://codecov.io/gh/astro-otter/otter/graph/badge.svg?token=BtCerOdTc0
 [codecov-link]:             https://codecov.io/gh/astro-otter/otter
 
+[![Documentation Status](https://readthedocs.org/projects/astro-otter/badge/?version=latest)](https://astro-otter.readthedocs.io/en/latest/?badge=latest)
 [![Actions Status][actions-badge]][actions-link]
+[![PyPI version][pypi-version]][pypi-link]
 [![Linting: Ruff][ruff-badge]][ruff-link]
 [![codecov][codecov-badge]][codecov-link]
 
 ## Installation
 To install the OTTER API use
 ```
 git clone https://github.com/astro-otter/otter.git
```

### Comparing `astro_otter-0.0.1/pyproject.toml` & `astro_otter-0.0.2/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -35,16 +35,25 @@
   "plotly",
   "astroquery",
   "synphot",
   "ads",
 
   # useful dev tools
   "ruff", # linter
-  "pre-commit" # enable pre-commit hooks
-  ]
+  "pre-commit", # enable pre-commit hooks
+
+  # tools for building the readthedocs page
+  "Sphinx>=3.0.0",
+  "myst_parser>=0.13",
+  "nbsphinx>=0.9.1",
+  "sphinx-book-theme>=0.0.33",
+  "sphinx_copybutton",
+  "autodoc",
+  "ipykernel"
+]
 
 [project.urls]
 Home = "https://github.com/astro-otter"
 
 [tool.setuptools.packages.find]
 where = ['src']
```

### Comparing `astro_otter-0.0.1/src/astro_otter.egg-info/PKG-INFO` & `astro_otter-0.0.2/src/astro_otter.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astro-otter
-Version: 0.0.1
+Version: 0.0.2
 Author-email: Noah Franz <nfranz@arizona.edu>
 License: MIT License
         
         Copyright (c) 2023 Noah Franz
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -46,14 +46,21 @@
 Requires-Dist: matplotlib
 Requires-Dist: plotly
 Requires-Dist: astroquery
 Requires-Dist: synphot
 Requires-Dist: ads
 Requires-Dist: ruff
 Requires-Dist: pre-commit
+Requires-Dist: Sphinx>=3.0.0
+Requires-Dist: myst_parser>=0.13
+Requires-Dist: nbsphinx>=0.9.1
+Requires-Dist: sphinx-book-theme>=0.0.33
+Requires-Dist: sphinx_copybutton
+Requires-Dist: autodoc
+Requires-Dist: ipykernel
 
 # OTTER API
 ### **O**pen mul**T**iwavelength **T**ransient **E**vent **R**epository
 
 A Python API for the OTTER.
 
 [actions-badge]:            https://github.com/astro-otter/otter/workflows/CI/badge.svg
@@ -62,26 +69,28 @@
 [black-link]:               https://github.com/psf/black
 [conda-badge]:              https://img.shields.io/conda/vn/conda-forge/hepfile
 [conda-link]:               https://github.com/conda-forge/hepfile-feedstock
 [github-discussions-badge]: https://img.shields.io/static/v1?label=Discussions&message=Ask&color=blue&logo=github
 [github-discussions-link]:  https://github.com/mattbellis/hepfile/discussions
 [gitter-badge]:             https://badges.gitter.im/https://github.com/mattbellis/hepfile/community.svg
 [gitter-link]:              https://gitter.im/https://github.com/mattbellis/hepfile/community?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge
-[pypi-link]:                https://pypi.org/project/hepfile/
-[pypi-platforms]:           https://img.shields.io/pypi/pyversions/hepfile
-[pypi-version]:             https://badge.fury.io/py/hepfile.svg
+[pypi-link]:                https://pypi.org/project/astro-otter/
+[pypi-platforms]:           https://img.shields.io/pypi/pyversions/astro-otter
+[pypi-version]:             https://badge.fury.io/py/astro-otter.svg
 [rtd-badge]:                https://readthedocs.org/projects/otter/badge/?version=latest
 [rtd-link]:                 https://otter.readthedocs.io/en/latest/?badge=latest
 [sk-badge]:                 https://scikit-hep.org/assets/images/Scikit--HEP-Project-blue.svg
 [ruff-badge]:               https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json
 [ruff-link]:                https://github.com/astral-sh/ruff
 [codecov-badge]:            https://codecov.io/gh/astro-otter/otter/graph/badge.svg?token=BtCerOdTc0
 [codecov-link]:             https://codecov.io/gh/astro-otter/otter
 
+[![Documentation Status](https://readthedocs.org/projects/astro-otter/badge/?version=latest)](https://astro-otter.readthedocs.io/en/latest/?badge=latest)
 [![Actions Status][actions-badge]][actions-link]
+[![PyPI version][pypi-version]][pypi-link]
 [![Linting: Ruff][ruff-badge]][ruff-link]
 [![codecov][codecov-badge]][codecov-link]
 
 ## Installation
 To install the OTTER API use
 ```
 git clone https://github.com/astro-otter/otter.git
```

### Comparing `astro_otter-0.0.1/src/otter/io/otter.py` & `astro_otter-0.0.2/src/otter/io/otter.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 This is the primary class for user interaction with the catalog
 """
 
+from __future__ import annotations
 import os
 import json
 import glob
 from warnings import warn
 
 import pandas as pd
 
@@ -24,22 +25,19 @@
 
 
 class Otter(object):
     """
     This is the primary class for users to access the otter backend database
 
     Args:
-        username [str]: Your connection username to the database, default is the user
-                        login which only has read permission.
-        password [str]: Your password corresponding to your username.
-        db [str]: The database name to connect to. This is default to 'otter' which is
-                  the only database so far.
-        collection [str]: The collection to read data from. Right now the only
-                          collection is 'tdes'.
-        debug [bool]: debug mode, set to true to limit reading from database.
+        datadir (str): Path to the data directory with the otter data. If not provided
+                       will default to a ".otter" directory in the CWD where you call
+                       this class from.
+        debug (bool): If we should just debug and not do anything serious.
+
     """
 
     def __init__(self, datadir: str = None, debug: bool = False) -> None:
         # save inputs
         if datadir is None:
             self.CWD = os.path.dirname(os.path.abspath("__FILE__"))
             self.DATADIR = os.path.join(self.CWD, ".otter")
@@ -83,17 +81,17 @@
     def cone_search(
         self, coords: SkyCoord, radius: float = 5, raw: bool = False
     ) -> Table:
         """
         Performs a cone search of the catalog over the given coords and radius.
 
         Args:
-            coords [SkyCoord]: An astropy SkyCoord object with coordinates to match to
-            radius [float]: The radius of the cone in arcseconds, default is 0.05"
-            raw [bool]: If False (the default) return an astropy table of the metadata
+            coords (SkyCoord): An astropy SkyCoord object with coordinates to match to
+            radius (float): The radius of the cone in arcseconds, default is 0.05"
+            raw (bool): If False (the default) return an astropy table of the metadata
                         for matching objects. Otherwise, return the raw json dicts
 
         Return:
             The metadata for the transients in coords+radius. Will return an astropy
             Table if raw is False, otherwise a dict.
         """
 
@@ -113,60 +111,74 @@
         **kwargs,
     ) -> Table:
         """
         Get the photometry of the objects matching the arguments. This will do the
         unit conversion for you!
 
         Args:
-            flux_units [astropy.unit.Unit]: Either a valid string to convert
+            flux_units (astropy.unit.Unit): Either a valid string to convert
                                             or an astropy.unit.Unit
-            date_units [astropy.unit.Unit]: Either a valid string to convert to a date
+            date_units (astropy.unit.Unit): Either a valid string to convert to a date
                                             or an astropy.unit.Unit
-            return_type [str]: Either 'astropy' or 'pandas'. If astropy, returns an
+            return_type (str): Either 'astropy' or 'pandas'. If astropy, returns an
                                astropy Table. If pandas, returns a pandas DataFrame.
                                Default is 'astropy'.
-            obs_type [str]: Either 'radio', 'uvoir', or 'xray'. Will only return that
+            obs_type (str): Either 'radio', 'uvoir', or 'xray'. Will only return that
                             type of photometry if not None. Default is None and will
                             return any type of photometry.
-            keep_raw [bool]: If True, keep the raw flux/date/freq/wave associated with
+            keep_raw (bool): If True, keep the raw flux/date/freq/wave associated with
                              the dataset. Else, just keep the converted data. Default
                              is False.
-            **kwargs : Arguments to pass to Otter.query(). Can be:
-                       names [list[str]]: A list of names to get the metadata for
-                       coords [SkyCoord]: An astropy SkyCoord object with coordinates
+            **kwargs : Arguments to pass to Otter.query(). Can be::
+
+                       names (list[str]): A list of names to get the metadata for
+                       coords (SkyCoord): An astropy SkyCoord object with coordinates
                                           to match to
-                       radius [float]: The radius in arcseconds for a cone search,
+                       radius (float): The radius in arcseconds for a cone search,
                                        default is 0.05"
-                       minZ [float]: The minimum redshift to search for
-                       maxZ [float]: The maximum redshift to search for
-                       refs [list[str]]: A list of ads bibcodes to match to. Will only
+                       minZ (float): The minimum redshift to search for
+                       maxZ (float): The maximum redshift to search for
+                       refs (list[str]): A list of ads bibcodes to match to. Will only
                                          return metadata for transients that have this
                                          as a reference.
-                       hasSpec [bool]: if True, only return events that have spectra.
+                       hasSpec (bool): if True, only return events that have spectra.
 
         Return:
-           The photometry for the requested transients that match the arguments.
-           Will be an astropy Table sorted by transient default name.
+            The photometry for the requested transients that match the arguments.
+            Will be an astropy Table sorted by transient default name.
+
+        Raises:
+            FailedQueryError: When the query returns no results
+            IOError: if one of your inputs is incorrect
         """
         queryres = self.query(hasphot=True, **kwargs)
 
         dicts = []
         for transient in queryres:
             # clean the photometry
             default_name = transient["name/default_name"]
-            phot = transient.clean_photometry(
-                flux_unit=flux_unit,
-                date_unit=date_unit,
-                wave_unit=wave_unit,
-                freq_unit=freq_unit,
-                obs_type=obs_type,
-            )
-            phot["name"] = [default_name] * len(phot)
 
-            dicts.append(phot)
+            try:
+                phot = transient.clean_photometry(
+                    flux_unit=flux_unit,
+                    date_unit=date_unit,
+                    wave_unit=wave_unit,
+                    freq_unit=freq_unit,
+                    obs_type=obs_type,
+                )
+
+                phot["name"] = [default_name] * len(phot)
+
+                dicts.append(phot)
+
+            except FailedQueryError:
+                # This is fine, it just means that there is no data associated
+                # with this one transient. We'll check and make sure there is data
+                # associated with at least one of the transients later!
+                pass
 
         if len(dicts) == 0:
             raise FailedQueryError()
         fullphot = pd.concat(dicts)
 
         # remove some possibly confusing keys
         keys_to_keep = [
@@ -199,15 +211,15 @@
             raise IOError("return_type can only be pandas or astropy")
 
     def load_file(self, filename: str) -> dict:
         """
         Loads an otter JSON file
 
         Args:
-            filename [str]: The path to the file to load
+            filename (str): The path to the OTTER JSON file to load
         """
 
         # read in files from summary
         with open(filename, "r") as f:
             to_ret = Transient(json.load(f))
 
         return to_ret
@@ -230,23 +242,23 @@
         WARNING! This does not do any conversions for you!
         This is how it differs from the `get_meta` method. Users should prefer to use
         `get_meta`, `getPhot`, and `getSpec` independently because it is a better
         workflow and can return the data in an astropy table with everything in the
         same units.
 
         Args:
-            names [list[str]]: A list of names to get the metadata for
-            coords [SkyCoord]: An astropy SkyCoord object with coordinates to match to
-            radius [float]: The radius in arcseconds for a cone search, default is 0.05"
-            minz [float]: The minimum redshift to search for
-            maxz [float]: The maximum redshift to search for
-            refs [list[str]]: A list of ads bibcodes to match to. Will only return
+            names (list[str]): A list of names to get the metadata for
+            coords (SkyCoord): An astropy SkyCoord object with coordinates to match to
+            radius (float): The radius in arcseconds for a cone search, default is 0.05"
+            minz (float): The minimum redshift to search for
+            maxz (float): The maximum redshift to search for
+            refs (list[str]): A list of ads bibcodes to match to. Will only return
                               metadata for transients that have this as a reference.
-            hasphot [bool]: if True, only returns transients which have photometry.
-            hasspec [bool]: if True, only return transients that have spectra.
+            hasphot (bool): if True, only returns transients which have photometry.
+            hasspec (bool): if True, only return transients that have spectra.
 
         Return:
            Get all of the raw (unconverted!) data for objects that match the criteria.
         """
         if (
             all(arg is None for arg in [names, coords, maxz, minz, refs])
             and not hasphot
@@ -340,32 +352,37 @@
 
             summary = summary[checkrefs]
 
         outdata = [self.load_file(path) for path in summary.json_path]
 
         return outdata
 
-    def save(self, schema: list[dict], testing=False, **kwargs) -> None:
+    def save(self, schema: list[dict], testing=False) -> None:
         """
         Upload all the data in the given list of schemas.
 
         Args:
-            schema [list[dict]]: A list of json dictionaries
+            schema (list[dict]): A list of json dictionaries
+            testing (bool): Should we just enter test mode? Default is False
+
+        Raises:
+            OtterLimitationError: If some objects in OTTER are within 5" we can't figure
+                                  out which ones to merge with which ones.
         """
 
         if not isinstance(schema, list):
             schema = [schema]
 
         for transient in schema:
-            print(transient["name/default_name"])
-
             # convert the json to a Transient
             if not isinstance(transient, Transient):
                 transient = Transient(transient)
 
+            print(transient["name/default_name"])
+
             coord = transient.get_skycoord()
             res = self.cone_search(coords=coord)
 
             if len(res) == 0:
                 # This is a new object to upload
                 print("Adding this as a new object...")
                 self._save_document(dict(transient), test_mode=testing)
@@ -401,16 +418,14 @@
 
         # now save this data
         # create a new file in self.DATADIR with this
         if len(todel) > 0:
             outfilepath = os.path.join(self.DATADIR, todel[0] + ".json")
             if test_mode:
                 print("Renaming the following file for backups: ", outfilepath)
-            else:
-                os.rename(outfilepath, outfilepath + ".backup")
         else:
             if test_mode:
                 print("Don't need to mess with the files at all!")
             fname = schema["name"]["default_name"] + ".json"
             fname = fname.replace(" ", "-")  # replace spaces in the filename
             outfilepath = os.path.join(self.DATADIR, fname)
 
@@ -425,21 +440,24 @@
         if not test_mode:
             with open(outfilepath, "w") as f:
                 f.write(out)
         else:
             print(f"Would write to {outfilepath}")
             # print(out)
 
-    def generate_summary_table(self, save=False):
+    def generate_summary_table(self, save=False) -> pd.DataFrame:
         """
         Generate a summary table for the JSON files in self.DATADIR
 
         args:
-            save [bool]: if True, save the summary file to "summary.csv"
-                         in self.DATADIR. Default is False.
+            save (bool): if True, save the summary file to "summary.csv"
+                         in self.DATADIR. Default is False and is just returned.
+
+        returns:
+            pandas.DataFrame of the summary meta information of the transients
         """
         allfiles = glob.glob(os.path.join(self.DATADIR, "*.json"))
 
         # read the data from all the json files and convert to Transients
         rows = []
         for jsonfile in allfiles:
             with open(jsonfile, "r") as j:
```

### Comparing `astro_otter-0.0.1/src/otter/io/transient.py` & `astro_otter-0.0.2/src/otter/io/transient.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 """
 Class for a transient,
 basically just inherits the dict properties with some overwriting
 """
 
+from __future__ import annotations
 import warnings
 from copy import deepcopy
 import re
 from collections.abc import MutableMapping
+from typing_extensions import Self
 
 import numpy as np
 import pandas as pd
 
 import astropy.units as u
 from astropy.time import Time
 from astropy.coordinates import SkyCoord
@@ -33,15 +35,17 @@
 
 class Transient(MutableMapping):
     def __init__(self, d={}, name=None):
         """
         Overwrite the dictionary init
 
         Args:
-            d [dict]: A transient dictionary
+            d (dict): A transient dictionary
+            name (str): The default name of the transient, default is None and it will
+                        be inferred from the input dictionary.
         """
         self.data = d
 
         if "reference_alias" in self:
             self.srcmap = {
                 ref["name"]: ref["human_readable_name"]
                 for ref in self["reference_alias"]
@@ -64,15 +68,15 @@
 
     def __getitem__(self, keys):
         """
         Override getitem to recursively access Transient elements
         """
 
         if isinstance(keys, (list, tuple)):
-            return Transient({key: self[key] for key in keys})
+            return Transient({key: (self[key] if key in self else []) for key in keys})
         elif isinstance(keys, str) and "/" in keys:  # this is for a path
             s = "']['".join(keys.split("/"))
             s = "['" + s
             s += "']"
             return eval(f"self{s}")
         elif (
             isinstance(keys, int)
@@ -81,14 +85,18 @@
         ):
             # this is for indexing a sublist
             return self[int(keys)]
         else:
             return self.data[keys]
 
     def __setitem__(self, key, value):
+        """
+        Override set item to work with the '/' syntax
+        """
+
         if isinstance(key, str) and "/" in key:  # this is for a path
             s = "']['".join(key.split("/"))
             s = "['" + s
             s += "']"
             exec(f"self{s} = value")
         else:
             self.data[key] = value
@@ -105,15 +113,15 @@
         return iter(self.data)
 
     def __len__(self):
         return len(self.data)
 
     def __repr__(self, html=False):
         if not html:
-            return str(self.data)
+            return f"Transient(\n\tName: {self.default_name},\n\tKeys: {self.keys()}\n)"
         else:
             html = ""
 
             coord = self.get_skycoord()
 
             # add the ra and dec
             # These are required so no need to check if they are there
@@ -256,22 +264,25 @@
 
         # and now combining out with the stuff only in t1 and t2
         out = out | dict(self[only_in_t1]) | dict(other[only_in_t2])
 
         # now return out as a Transient Object
         return Transient(out)
 
-    def get_meta(self, keys=None):
+    def get_meta(self, keys=None) -> Self:
         """
         Get the metadata (no photometry or spectra)
 
         This essentially just wraps on __getitem__ but with some checks
 
         Args:
-            keys [list[str]] : list of keys
+            keys (list[str]) : list of keys to get the metadata for from the transient
+
+        Returns:
+            A Transient object of just the meta data
         """
         if keys is None:
             keys = list(self.keys())
 
             # note: using the remove method is safe here because dict keys are unique
             if "photometry" in keys:
                 keys.remove("photometry")
@@ -292,43 +303,56 @@
                     keys.remove(key)
                     warnings.warn(
                         f"Not returning {key} because it is not in this transient!"
                     )
 
         return self[keys]
 
-    def get_skycoord(self, coord_format="icrs"):
+    def get_skycoord(self, coord_format="icrs") -> SkyCoord:
         """
         Convert the coordinates to an astropy SkyCoord
+
+        Args:
+            coord_format (str): Astropy coordinate format to convert the SkyCoord to
+                                defaults to icrs.
+
+        Returns:
+            Astropy.coordinates.SkyCoord of the default coordinate for the transient
         """
 
         # now we can generate the SkyCoord
         f = "df['coordinate_type'] == 'equitorial'"
         coord_dict = self._get_default("coordinate", filt=f)
         coordin = self._reformat_coordinate(coord_dict)
         coord = SkyCoord(**coordin).transform_to(coord_format)
 
         return coord
 
-    def get_discovery_date(self):
+    def get_discovery_date(self) -> Time:
         """
-        Get the default discovery date
+        Get the default discovery date for this Transient
+
+        Returns:
+            astropy.time.Time of the default discovery date
         """
         key = "date_reference"
         date = self._get_default(key, filt='df["date_type"] == "discovery"')
         if "date_format" in date:
             f = date["date_format"]
         else:
             f = "mjd"
 
         return Time(date["value"], format=f)
 
-    def get_redshift(self):
+    def get_redshift(self) -> float:
         """
-        Get the default redshift
+        Get the default redshift of this Transient
+
+        Returns:
+            Float value of the default redshift
         """
         f = "df['distance_type']=='redshift'"
         default = self._get_default("distance", filt=f)
         if default is None:
             return default
         else:
             return default["value"]
@@ -386,18 +410,40 @@
         self,
         flux_unit: u.Unit = "mag(AB)",
         date_unit: u.Unit = "MJD",
         freq_unit: u.Unit = "GHz",
         wave_unit: u.Unit = "nm",
         by: str = "raw",
         obs_type: str = None,
-    ):
+    ) -> pd.DataFrame:
         """
         Ensure the photometry associated with this transient is all in the same
         units/system/etc
+
+        Args:
+            flux_unit (astropy.unit.Unit): The astropy unit or string representation of
+                                           an astropy unit to convert and return the
+                                           flux as.
+            date_unit (str): Valid astropy date format string.
+            freq_unit (astropy.unit.Unit): The astropy unit or string representation of
+                                           an astropy unit to convert and return the
+                                           frequency as.
+            wave_unit (astropy.unit.Unit): The astropy unit or string representation of
+                                           an astropy unit to convert and return the
+                                           wavelength as.
+            by (str): Either 'raw' or 'value'. 'raw' is the default and is highly
+                      recommended! If 'value' is used it may skip some photometry.
+                      See the schema definition to understand this keyword completely
+                      before using it.
+            obs_type (str): "radio", "xray", or "uvoir". If provided, it only returns
+                            data taken within that range of wavelengths/frequencies.
+                            Default is None which will return all of the data.
+
+        Returns:
+            A pandas DataFrame of the cleaned up photometry in the requested units
         """
 
         # check inputs
         if by not in {"value", "raw"}:
             raise IOError("Please choose either value or raw!")
 
         # turn the photometry key into a pandas dataframe
@@ -425,14 +471,17 @@
         # make sure 'by' is in df
         if by not in df:
             if by == "value":
                 by = "raw"
             else:
                 by = "value"
 
+        # skip rows where 'by' is nan
+        df = df[df[by].notna()]
+
         # drop irrelevant obs_types before continuing
         if obs_type is not None:
             valid_obs_types = {"radio", "uvoir", "xray"}
             if obs_type not in valid_obs_types:
                 raise IOError("Please provide a valid obs_type")
             df = df[df.obs_type == obs_type]
```

### Comparing `astro_otter-0.0.1/src/otter/plotter/otter_plotter.py` & `astro_otter-0.0.2/src/otter/plotter/otter_plotter.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,27 +2,29 @@
 OtterPlotter Class which handles the backend of the plotting.
 
 Currently supported backends are:
 - matplotlib
 - plotly
 """
 
+from __future__ import annotations
 import importlib
 
 
 class OtterPlotter:
-    def __init__(self, backend):
-        """
-        Handles the backend for the "plotter" module
+    """
+    Handles the backend for the "plotter" module
+
+    Args:
+        backend (string): a string of the module name to import and use
+                          as the backend. Currently supported are "matplotlib",
+                          "matplotlib.pyplot", "plotly", and "plotly.graph_objects"
+    """
 
-        Args:
-            backend [string]: a string of the module name to import and use
-                              as the backend. Currently supported are "matplotlib",
-                              "matplotlib.pyplot", "plotly", and "plotly.graph_objects"
-        """
+    def __init__(self, backend):
         if backend == "matplotlib.pyplot":
             self.backend = backend
         elif backend == "pyplot.graph_objects":
             self.backend = backend
         elif "plotly" in backend and "graph_objects" not in backend:
             self.backend = "plotly.graph_objects"
         elif "matplotlib" in backend and "pyplot" not in backend:
```

### Comparing `astro_otter-0.0.1/src/otter/plotter/plotter.py` & `astro_otter-0.0.2/src/otter/plotter/plotter.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 Some utilities to create common plots for transients that use the OtterPlotter
 """
 
+from __future__ import annotations
 from .otter_plotter import OtterPlotter
 
 
 def plot_light_curve(
     date: float,
     flux: float,
     date_err: float = None,
@@ -17,23 +18,23 @@
     ylabel: str = "Flux",
     **kwargs,
 ):
     """
     Plot the light curve for the input data
 
     Args:
-        date [float]: MJD dates
-        flux [float]: Flux
-        date_err [float]: optional error on the MJD dates
-        flux_err [float]: optional error on the flux
-        fig [float]: matplotlib fig object, optional. Will be created if not provided.
-        ax [float]: matplitlib axis object, optional. Will be created if not provided.
-        backend [str]: backend for plotting. options: "matplotlib" (default) or "plotly"
-        xlabel [str]: x-axis label
-        ylabel [str]: y-axis label
+        date (float): MJD dates
+        flux (float): Flux
+        date_err (float): optional error on the MJD dates
+        flux_err (float): optional error on the flux
+        fig (float): matplotlib fig object, optional. Will be created if not provided.
+        ax (float): matplitlib axis object, optional. Will be created if not provided.
+        backend (str): backend for plotting. options: "matplotlib" (default) or "plotly"
+        xlabel (str): x-axis label
+        ylabel (str): y-axis label
         **kwargs: keyword arguments to pass to either plotly.graph_objects.add_scatter
                   or matplotlib.pyplot.errorbar
 
     Returns:
        Either a matplotlib axis or plotly figure
     """
 
@@ -62,23 +63,23 @@
     ylabel: str = "Flux",
     **kwargs,
 ):
     """
     Plot the SED for the input data
 
     Args:
-        wave_or_freq [float]: wave or frequency array
-        flux [float]: Flux
-        wave_or_freq_err [float]: optional error on the MJD dates
-        flux_err [float]: optional error on the flux
-        fig [float]: matplotlib fig object, optional. Will be created if not provided.
-        ax [float]: matplitlib axis object, optional. Will be created if not provided.
-        backend [str]: backend for plotting. Options: "matplotlib" (default) or "plotly"
-        xlabel [str]: x-axis label
-        ylabel [str]: y-axis label
+        wave_or_freq (float): wave or frequency array
+        flux (float): Flux
+        wave_or_freq_err (float): optional error on the MJD dates
+        flux_err (float): optional error on the flux
+        fig (float): matplotlib fig object, optional. Will be created if not provided.
+        ax (float): matplitlib axis object, optional. Will be created if not provided.
+        backend (str): backend for plotting. Options: "matplotlib" (default) or "plotly"
+        xlabel (str): x-axis label
+        ylabel (str): y-axis label
         **kwargs: keyword arguments to pass to either plotly.graph_objects.add_scatter
                   or matplotlib.pyplot.errorbar
 
     Returns:
        Either a matplotlib axis or plotly figure
     """
```

### Comparing `astro_otter-0.0.1/src/otter/util.py` & `astro_otter-0.0.2/src/otter/util.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 Some constants, mappings, and functions to be used across the software
 """
 
+from __future__ import annotations
 import os
 import ads
 import astropy.units as u
 
 """
 Helper functions first that just don't belong anywhere else
 """
@@ -183,14 +184,18 @@
     "F1130W": 11310.984595876938,
     "F1280W": 12831.396996921212,
     "F1500W": 15091.367399905488,
     "F1800W": 18006.083119653664,
     "F2100W": 20842.526633138932,
     "F2550W": 25408.228367890282,
 }
+"""
+Mapping for the effective wavelength in nanometers for all filters used in the dataset.
+"""
+
 
 # gives the effective frequency for all filters
 # These are all in THz
 FILTER_MAP_FREQ = {
     "FUV": 1975.086895569116,
     "NUV": 1346.3548820463916,
     "UVW2": 1531.4976984760474,
@@ -298,14 +303,18 @@
     "F1130W": 26.53952983680919,
     "F1280W": 23.59741975845449,
     "F1500W": 20.08679352819493,
     "F1800W": 16.773842151606242,
     "F2100W": 14.581938602646188,
     "F2550W": 11.919267708332558,
 }
+"""
+Mapping for the effective frequencies in THz for all the filters used in OTTER
+"""
+
 
 # x-ray telescope areas for converting
 # NOTE: these are estimates from the links provided
 # Since this is inherently instrument dependent they are not entirely reliable
 # All are for 1-2 keV
 XRAY_AREAS = {
     # https://swift.gsfc.nasa.gov/about_swift/Sci_Fact_Sheet.pdf
@@ -315,36 +324,59 @@
     # https://www.cosmos.esa.int/web/xmm-newton/technical-details-mirrors
     "xmm": 1500 * u.cm**2,
     "xmm slew": 1500 * u.cm**2,
     "xmm pointed": 1500 * u.cm**2,
     # https://cxc.harvard.edu/cdo/about_chandra
     "chandra": 600 * u.cm**2,
 }
+"""
+X-Ray telescope areas that are used for converting from counts to other units.
+
+NOTE: These are estimates from the following links
+* https://swift.gsfc.nasa.gov/about_swift/Sci_Fact_Sheet.pdf
+* https://heasarc.gsfc.nasa.gov/docs/rosat/ruh/handbook/node39.html#SECTION00634000000000000000
+* https://www.cosmos.esa.int/web/xmm-newton/technical-details-mirrors
+* https://cxc.harvard.edu/cdo/about_chandra
+"""
+
 
 # define a working base directory constant
 BASEDIR = os.path.dirname(os.path.dirname(os.path.dirname(os.path.abspath(__file__))))
+"""
+Base directory for the OTTER API software package
+"""
+
 DATADIR = os.path.join(BASEDIR, "data", "base")
+"""
+Deprecated database directory that IS NOT always constant anymore
+"""
 
 # Overarching schema that stops once we get down to a string or list
 schema = {
     "schema_version": {"value": "0", "comment": "Copied from tde.space"},
     "name": {"default_name": None, "alias": []},
     "coordinate": [],
     "distance": [],
     "classification": [],
     "reference_alias": [],
     "date_reference": [],
     "photometry": [],
     "spectra": [],
     "filter_alias": [],
 }
-
+"""
+Schema dictionary to be filled with values from the subschemas
+"""
 
 # sub schemas that get filled into lists
 name_alias_schema = {"value": None, "reference": None}
+"""
+Subschema for the name and alias dictionary
+"""
+
 coordinate_schema = {
     "ra": None,
     "dec": None,
     "l": None,
     "b": None,
     "lon": None,
     "lat": None,
@@ -363,44 +395,61 @@
     "epoch": None,
     "frame": None,
     "coord_type": None,
     "computed": None,
     "reference": None,
     "default": None,
 }
+"""
+Subschema to describe the possible attributes for the coordinate dictionary
+"""
+
 
 distance_schema = {
     "value": None,
     "unit": None,
     "error": None,
     "cosmology": None,
     "reference": None,
     "computed": None,
     "uuid": None,
     "default": None,
     "distance_type": None,
 }
+"""
+Subschema to describe the possible attributes for the distance dictionary
+"""
+
 
 classification_schema = {
     "object_class": None,
     "confidence": None,
     "class_type": None,
     "reference": None,
     "default": None,
 }
+"""
+Subschema to describe the attributes for the classification dictionary
+"""
 
 reference_alias_schema = {"name": None, "human_readable_name": None}
+"""
+Subschema to describe the attributes for the reference alias dictionary
+"""
 
 date_reference_schema = {
     "value": None,
     "date_format": None,
     "date_type": None,
     "reference": None,
     "computed": None,
 }
+"""
+Subschema to describe the date_reference dictionary attributes
+"""
 
 photometry_schema = {
     "raw": None,
     "raw_err": None,
     "raw_units": None,
     "value": None,
     "value_err": None,
@@ -432,14 +481,18 @@
     "corr_hostav": None,
     "val_k": None,
     "val_s": None,
     "val_av": None,
     "val_host": None,
     "val_hostav": None,
 }
+"""
+Subschema to describe all of the possible attributes that can be used in the photometry
+dictionary
+"""
 
 spectra_schema = {
     "wavelength": None,
     "wavelength_units": None,
     "flux": None,
     "fluxerr": None,
     "raw": None,
@@ -491,20 +544,26 @@
     "freq_max": None,
     "zp": None,
     "wave_units": None,
     "freq_units": None,
     "zp_units": None,
     "zp_system": None,
 }
+"""
+Subschema to describe the attributes in the filter_alias dictionary
+"""
 
 # package the subschemas by the key used for that location in the Transient object
 subschema = {
     "name/alias": name_alias_schema,
     "coordinate": coordinate_schema,
     "distance": distance_schema,
     "classification": classification_schema,
     "reference_alias": reference_alias_schema,
     "date_reference": date_reference_schema,
     "photometry": photometry_schema,
     "spectra": spectra_schema,
     "filter_alias": filter_alias_schema,
 }
+"""
+A useful variable to describe all of the subschemas that are available and can be used
+"""
```

