# Comparing `tmp/deafrica-tools-2.3.7.tar.gz` & `tmp/deafrica_tools-2.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deafrica-tools-2.3.7.tar", last modified: Fri Mar  1 10:12:13 2024, max compression
+gzip compressed data, was "deafrica_tools-2.3.8.tar", last modified: Wed May 15 23:20:51 2024, max compression
```

## Comparing `deafrica-tools-2.3.7.tar` & `deafrica_tools-2.3.8.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 10:12:13.417901 deafrica-tools-2.3.7/
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-03-01 10:11:54.000000 deafrica-tools-2.3.7/.flake8
--rw-r--r--   0 runner    (1001) docker     (127)     1892 2024-03-01 10:11:54.000000 deafrica-tools-2.3.7/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-03-01 10:11:54.000000 deafrica-tools-2.3.7/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-03-01 10:11:54.000000 deafrica-tools-2.3.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    18441 2024-03-01 10:12:13.417901 deafrica-tools-2.3.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3097 2024-03-01 10:11:54.000000 deafrica-tools-2.3.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 10:12:13.409901 deafrica-tools-2.3.7/conda/
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-03-01 10:11:54.000000 deafrica-tools-2.3.7/conda/environment.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      951 2024-03-01 10:11:54.000000 deafrica-tools-2.3.7/conda/requirements.in
--rw-r--r--   0 runner    (1001) docker     (127)    21310 2024-03-01 10:11:54.000000 deafrica-tools-2.3.7/conda/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 10:12:13.413901 deafrica-tools-2.3.7/deafrica_tools/
--rw-r--r--   0 runner    (1001) docker     (127)      653 2024-03-01 10:11:54.000000 deafrica-tools-2.3.7/deafrica_tools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 10:12:13.417901 deafrica-tools-2.3.7/deafrica_tools/app/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-01 10:11:54.000000 deafrica-tools-2.3.7/deafrica_tools/app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    31449 2024-03-01 10:11:54.000000 deafrica-tools-2.3.7/deafrica_tools/app/animations.py
--rw-r--r--   0 runner    (1001) docker     (127)    10984 2024-03-01 10:11:54.000000 deafrica-tools-2.3.7/deafrica_tools/app/changefilmstrips.py
--rw-r--r--   0 runner    (1001) docker     (127)    10494 2024-03-01 10:11:54.000000 deafrica-tools-2.3.7/deafrica_tools/app/crophealth.py
--rw-r--r--   0 runner    (1001) docker     (127)    20287 2024-03-01 10:11:54.000000 deafrica-tools-2.3.7/deafrica_tools/app/deacoastlines.py
--rw-r--r--   0 runner    (1001) docker     (127)    37843 2024-03-01 10:11:54.000000 deafrica-tools-2.3.7/deafrica_tools/app/forestmonitoring.py
--rw-r--r--   0 runner    (1001) docker     (127)     8673 2024-03-01 10:11:54.000000 deafrica-tools-2.3.7/deafrica_tools/app/geomedian.py
--rw-r--r--   0 runner    (1001) docker     (127)    13383 2024-03-01 10:11:54.000000 deafrica-tools-2.3.7/deafrica_tools/app/imageexport.py
--rw-r--r--   0 runner    (1001) docker     (127)    13148 2024-03-01 10:11:54.000000 deafrica-tools-2.3.7/deafrica_tools/app/wetlandsinsighttool.py
--rw-r--r--   0 runner    (1001) docker     (127)     9882 2024-03-01 10:11:54.000000 deafrica-tools-2.3.7/deafrica_tools/app/widgetconstructors.py
--rw-r--r--   0 runner    (1001) docker     (127)     2016 2024-03-01 10:11:54.000000 deafrica-tools-2.3.7/deafrica_tools/areaofinterest.py
--rw-r--r--   0 runner    (1001) docker     (127)    24548 2024-03-01 10:11:54.000000 deafrica-tools-2.3.7/deafrica_tools/bandindices.py
--rw-r--r--   0 runner    (1001) docker     (127)    61470 2024-03-01 10:11:54.000000 deafrica-tools-2.3.7/deafrica_tools/classification.py
--rw-r--r--   0 runner    (1001) docker     (127)    42791 2024-03-01 10:11:54.000000 deafrica-tools-2.3.7/deafrica_tools/coastal.py
--rw-r--r--   0 runner    (1001) docker     (127)     3575 2024-03-01 10:11:54.000000 deafrica-tools-2.3.7/deafrica_tools/dask.py
--rw-r--r--   0 runner    (1001) docker     (127)    60516 2024-03-01 10:11:54.000000 deafrica-tools-2.3.7/deafrica_tools/datahandling.py
--rw-r--r--   0 runner    (1001) docker     (127)    16152 2024-03-01 10:11:54.000000 deafrica-tools-2.3.7/deafrica_tools/load_era5.py
--rw-r--r--   0 runner    (1001) docker     (127)     2793 2024-03-01 10:11:54.000000 deafrica-tools-2.3.7/deafrica_tools/load_isda.py
--rw-r--r--   0 runner    (1001) docker     (127)     2027 2024-03-01 10:11:54.000000 deafrica-tools-2.3.7/deafrica_tools/load_soil_moisture.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 10:12:13.409901 deafrica-tools-2.3.7/deafrica_tools/locales/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 10:12:13.409901 deafrica-tools-2.3.7/deafrica_tools/locales/fr/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 10:12:13.417901 deafrica-tools-2.3.7/deafrica_tools/locales/fr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1783 2024-03-01 10:11:54.000000 deafrica-tools-2.3.7/deafrica_tools/locales/fr/LC_MESSAGES/deafrica_tools.mo
--rw-r--r--   0 runner    (1001) docker     (127)     3315 2024-03-01 10:11:54.000000 deafrica-tools-2.3.7/deafrica_tools/locales/fr/LC_MESSAGES/deafrica_tools.po
--rw-r--r--   0 runner    (1001) docker     (127)    50697 2024-03-01 10:11:54.000000 deafrica-tools-2.3.7/deafrica_tools/plotting.py
--rw-r--r--   0 runner    (1001) docker     (127)    34121 2024-03-01 10:11:54.000000 deafrica-tools-2.3.7/deafrica_tools/spatial.py
--rw-r--r--   0 runner    (1001) docker     (127)    18749 2024-03-01 10:11:54.000000 deafrica-tools-2.3.7/deafrica_tools/temporal.py
--rw-r--r--   0 runner    (1001) docker     (127)     3604 2024-03-01 10:11:54.000000 deafrica-tools-2.3.7/deafrica_tools/waterbodies.py
--rw-r--r--   0 runner    (1001) docker     (127)    25961 2024-03-01 10:11:54.000000 deafrica-tools-2.3.7/deafrica_tools/wetlands.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 10:12:13.417901 deafrica-tools-2.3.7/deafrica_tools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    18441 2024-03-01 10:12:11.000000 deafrica-tools-2.3.7/deafrica_tools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1247 2024-03-01 10:12:13.000000 deafrica-tools-2.3.7/deafrica_tools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-01 10:12:11.000000 deafrica-tools-2.3.7/deafrica_tools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-03-01 10:12:11.000000 deafrica-tools-2.3.7/deafrica_tools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-03-01 10:12:11.000000 deafrica-tools-2.3.7/deafrica_tools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2232 2024-03-01 10:11:54.000000 deafrica-tools-2.3.7/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2890 2024-03-01 10:11:54.000000 deafrica-tools-2.3.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-01 10:12:13.417901 deafrica-tools-2.3.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:20:51.768966 deafrica_tools-2.3.8/
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-15 23:20:30.000000 deafrica_tools-2.3.8/.flake8
+-rw-r--r--   0 runner    (1001) docker     (127)     1892 2024-05-15 23:20:30.000000 deafrica_tools-2.3.8/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-05-15 23:20:30.000000 deafrica_tools-2.3.8/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-15 23:20:30.000000 deafrica_tools-2.3.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    18507 2024-05-15 23:20:51.768966 deafrica_tools-2.3.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3163 2024-05-15 23:20:30.000000 deafrica_tools-2.3.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:20:51.760966 deafrica_tools-2.3.8/conda/
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-05-15 23:20:30.000000 deafrica_tools-2.3.8/conda/environment.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      951 2024-05-15 23:20:30.000000 deafrica_tools-2.3.8/conda/requirements.in
+-rw-r--r--   0 runner    (1001) docker     (127)    21310 2024-05-15 23:20:30.000000 deafrica_tools-2.3.8/conda/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:20:51.764966 deafrica_tools-2.3.8/deafrica_tools/
+-rw-r--r--   0 runner    (1001) docker     (127)      675 2024-05-15 23:20:30.000000 deafrica_tools-2.3.8/deafrica_tools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:20:51.764966 deafrica_tools-2.3.8/deafrica_tools/app/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 23:20:30.000000 deafrica_tools-2.3.8/deafrica_tools/app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31449 2024-05-15 23:20:30.000000 deafrica_tools-2.3.8/deafrica_tools/app/animations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10984 2024-05-15 23:20:30.000000 deafrica_tools-2.3.8/deafrica_tools/app/changefilmstrips.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10494 2024-05-15 23:20:30.000000 deafrica_tools-2.3.8/deafrica_tools/app/crophealth.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20287 2024-05-15 23:20:30.000000 deafrica_tools-2.3.8/deafrica_tools/app/deacoastlines.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37843 2024-05-15 23:20:30.000000 deafrica_tools-2.3.8/deafrica_tools/app/forestmonitoring.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8673 2024-05-15 23:20:30.000000 deafrica_tools-2.3.8/deafrica_tools/app/geomedian.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13383 2024-05-15 23:20:30.000000 deafrica_tools-2.3.8/deafrica_tools/app/imageexport.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13148 2024-05-15 23:20:30.000000 deafrica_tools-2.3.8/deafrica_tools/app/wetlandsinsighttool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9882 2024-05-15 23:20:30.000000 deafrica_tools-2.3.8/deafrica_tools/app/widgetconstructors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2016 2024-05-15 23:20:30.000000 deafrica_tools-2.3.8/deafrica_tools/areaofinterest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24548 2024-05-15 23:20:30.000000 deafrica_tools-2.3.8/deafrica_tools/bandindices.py
+-rw-r--r--   0 runner    (1001) docker     (127)    61470 2024-05-15 23:20:30.000000 deafrica_tools-2.3.8/deafrica_tools/classification.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42791 2024-05-15 23:20:30.000000 deafrica_tools-2.3.8/deafrica_tools/coastal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3575 2024-05-15 23:20:30.000000 deafrica_tools-2.3.8/deafrica_tools/dask.py
+-rw-r--r--   0 runner    (1001) docker     (127)    60516 2024-05-15 23:20:30.000000 deafrica_tools-2.3.8/deafrica_tools/datahandling.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16152 2024-05-15 23:20:30.000000 deafrica_tools-2.3.8/deafrica_tools/load_era5.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2793 2024-05-15 23:20:30.000000 deafrica_tools-2.3.8/deafrica_tools/load_isda.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2027 2024-05-15 23:20:30.000000 deafrica_tools-2.3.8/deafrica_tools/load_soil_moisture.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:20:51.756966 deafrica_tools-2.3.8/deafrica_tools/locales/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:20:51.756966 deafrica_tools-2.3.8/deafrica_tools/locales/fr/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:20:51.764966 deafrica_tools-2.3.8/deafrica_tools/locales/fr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1783 2024-05-15 23:20:30.000000 deafrica_tools-2.3.8/deafrica_tools/locales/fr/LC_MESSAGES/deafrica_tools.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     3315 2024-05-15 23:20:30.000000 deafrica_tools-2.3.8/deafrica_tools/locales/fr/LC_MESSAGES/deafrica_tools.po
+-rw-r--r--   0 runner    (1001) docker     (127)    50697 2024-05-15 23:20:30.000000 deafrica_tools-2.3.8/deafrica_tools/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34121 2024-05-15 23:20:30.000000 deafrica_tools-2.3.8/deafrica_tools/spatial.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18749 2024-05-15 23:20:30.000000 deafrica_tools-2.3.8/deafrica_tools/temporal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3604 2024-05-15 23:20:30.000000 deafrica_tools-2.3.8/deafrica_tools/waterbodies.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25961 2024-05-15 23:20:30.000000 deafrica_tools-2.3.8/deafrica_tools/wetlands.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:20:51.764966 deafrica_tools-2.3.8/deafrica_tools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    18507 2024-05-15 23:20:49.000000 deafrica_tools-2.3.8/deafrica_tools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1247 2024-05-15 23:20:51.000000 deafrica_tools-2.3.8/deafrica_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 23:20:49.000000 deafrica_tools-2.3.8/deafrica_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-05-15 23:20:49.000000 deafrica_tools-2.3.8/deafrica_tools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-15 23:20:49.000000 deafrica_tools-2.3.8/deafrica_tools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2232 2024-05-15 23:20:30.000000 deafrica_tools-2.3.8/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2946 2024-05-15 23:20:30.000000 deafrica_tools-2.3.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 23:20:51.768966 deafrica_tools-2.3.8/setup.cfg
```

### Comparing `deafrica-tools-2.3.7/.gitignore` & `deafrica_tools-2.3.8/.gitignore`

 * *Files identical despite different names*

### Comparing `deafrica-tools-2.3.7/.pre-commit-config.yaml` & `deafrica_tools-2.3.8/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `deafrica-tools-2.3.7/LICENSE` & `deafrica_tools-2.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `deafrica-tools-2.3.7/PKG-INFO` & `deafrica_tools-2.3.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deafrica-tools
-Version: 2.3.7
+Version: 2.3.8
 Summary: Functions and algorithms for analysing Digital Earth Africa data.
 Author-email: Digital Earth Africa <systems@digitalearthafrica.org>
 Maintainer-email: Digital Earth Africa <systems@digitalearthafrica.org>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -275,25 +275,26 @@
 
 # Digital Earth Africa Tools Package
 
 Python functions and algorithms developed to assist in analysing Digital Earth Africa data (e.g. loading data, plotting, spatial analysis, machine learning).
 
 ## Installation
 
-This module is automatically installed on the Digital Earth Africa Sandbox. If for some reason the module isn't available on the Digital Earth Africa Sandbox, you can also `pip install` the module from the terminal.
+This module is automatically installed on the Digital Earth Africa Sandbox. If for some reason the module isn't available on the Digital Earth Africa Sandbox, or to upgrade the tools, you can `pip install` the module from the terminal.
 
-You can install the `deafrica-tools` package from PyPI using:
+You can install the latest version of `deafrica-tools` from PyPI using:
 
 ```
 python -m pip install --extra-index-url="https://packages.dea.ga.gov.au" deafrica-tools 
 ```
-or install the package from the `Tools` directory:
+
+or install the package directly from the `Tools` directory to incorperate local changes:
 
 ```
-python -m pip install --extra-index-url="https://packages.dea.ga.gov.au" -e Tools/
+python -m pip install --extra-index-url="https://packages.dea.ga.gov.au" Tools/
 ```
        
 To install this module from the source on any other system with `pip`:
 
 ```
 python -m pip install --extra-index-url="https://packages.dea.ga.gov.au" git+https://github.com/digitalearthafrica/deafrica-sandbox-notebooks.git#subdirectory=Tools
 ```
```

### Comparing `deafrica-tools-2.3.7/README.md` & `deafrica_tools-2.3.8/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -2,25 +2,26 @@
 
 # Digital Earth Africa Tools Package
 
 Python functions and algorithms developed to assist in analysing Digital Earth Africa data (e.g. loading data, plotting, spatial analysis, machine learning).
 
 ## Installation
 
-This module is automatically installed on the Digital Earth Africa Sandbox. If for some reason the module isn't available on the Digital Earth Africa Sandbox, you can also `pip install` the module from the terminal.
+This module is automatically installed on the Digital Earth Africa Sandbox. If for some reason the module isn't available on the Digital Earth Africa Sandbox, or to upgrade the tools, you can `pip install` the module from the terminal.
 
-You can install the `deafrica-tools` package from PyPI using:
+You can install the latest version of `deafrica-tools` from PyPI using:
 
 ```
 python -m pip install --extra-index-url="https://packages.dea.ga.gov.au" deafrica-tools 
 ```
-or install the package from the `Tools` directory:
+
+or install the package directly from the `Tools` directory to incorperate local changes:
 
 ```
-python -m pip install --extra-index-url="https://packages.dea.ga.gov.au" -e Tools/
+python -m pip install --extra-index-url="https://packages.dea.ga.gov.au" Tools/
 ```
        
 To install this module from the source on any other system with `pip`:
 
 ```
 python -m pip install --extra-index-url="https://packages.dea.ga.gov.au" git+https://github.com/digitalearthafrica/deafrica-sandbox-notebooks.git#subdirectory=Tools
 ```
```

### Comparing `deafrica-tools-2.3.7/conda/requirements.in` & `deafrica_tools-2.3.8/conda/requirements.in`

 * *Files identical despite different names*

### Comparing `deafrica-tools-2.3.7/conda/requirements.txt` & `deafrica_tools-2.3.8/conda/requirements.txt`

 * *Files identical despite different names*

### Comparing `deafrica-tools-2.3.7/deafrica_tools/__init__.py` & `deafrica_tools-2.3.8/deafrica_tools/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 __locales__ = __path__[0] + '/locales'
 
+__version__ = '2.3.8'
 
 def set_lang(lang=None):
     if lang is None:
         import os
         os_lang = os.getenv('LANG')
         
         # Just take the first 2 letters: 'fr' not 'fr_FR.UTF-8'
```

### Comparing `deafrica-tools-2.3.7/deafrica_tools/app/animations.py` & `deafrica_tools-2.3.8/deafrica_tools/app/animations.py`

 * *Files identical despite different names*

### Comparing `deafrica-tools-2.3.7/deafrica_tools/app/changefilmstrips.py` & `deafrica_tools-2.3.8/deafrica_tools/app/changefilmstrips.py`

 * *Files identical despite different names*

### Comparing `deafrica-tools-2.3.7/deafrica_tools/app/crophealth.py` & `deafrica_tools-2.3.8/deafrica_tools/app/crophealth.py`

 * *Files identical despite different names*

### Comparing `deafrica-tools-2.3.7/deafrica_tools/app/deacoastlines.py` & `deafrica_tools-2.3.8/deafrica_tools/app/deacoastlines.py`

 * *Files identical despite different names*

### Comparing `deafrica-tools-2.3.7/deafrica_tools/app/forestmonitoring.py` & `deafrica_tools-2.3.8/deafrica_tools/app/forestmonitoring.py`

 * *Files identical despite different names*

### Comparing `deafrica-tools-2.3.7/deafrica_tools/app/geomedian.py` & `deafrica_tools-2.3.8/deafrica_tools/app/geomedian.py`

 * *Files identical despite different names*

### Comparing `deafrica-tools-2.3.7/deafrica_tools/app/imageexport.py` & `deafrica_tools-2.3.8/deafrica_tools/app/imageexport.py`

 * *Files identical despite different names*

### Comparing `deafrica-tools-2.3.7/deafrica_tools/app/wetlandsinsighttool.py` & `deafrica_tools-2.3.8/deafrica_tools/app/wetlandsinsighttool.py`

 * *Files identical despite different names*

### Comparing `deafrica-tools-2.3.7/deafrica_tools/app/widgetconstructors.py` & `deafrica_tools-2.3.8/deafrica_tools/app/widgetconstructors.py`

 * *Files identical despite different names*

### Comparing `deafrica-tools-2.3.7/deafrica_tools/areaofinterest.py` & `deafrica_tools-2.3.8/deafrica_tools/areaofinterest.py`

 * *Files identical despite different names*

### Comparing `deafrica-tools-2.3.7/deafrica_tools/bandindices.py` & `deafrica_tools-2.3.8/deafrica_tools/bandindices.py`

 * *Files identical despite different names*

### Comparing `deafrica-tools-2.3.7/deafrica_tools/classification.py` & `deafrica_tools-2.3.8/deafrica_tools/classification.py`

 * *Files identical despite different names*

### Comparing `deafrica-tools-2.3.7/deafrica_tools/coastal.py` & `deafrica_tools-2.3.8/deafrica_tools/coastal.py`

 * *Files identical despite different names*

### Comparing `deafrica-tools-2.3.7/deafrica_tools/dask.py` & `deafrica_tools-2.3.8/deafrica_tools/dask.py`

 * *Files identical despite different names*

### Comparing `deafrica-tools-2.3.7/deafrica_tools/datahandling.py` & `deafrica_tools-2.3.8/deafrica_tools/datahandling.py`

 * *Files identical despite different names*

### Comparing `deafrica-tools-2.3.7/deafrica_tools/load_era5.py` & `deafrica_tools-2.3.8/deafrica_tools/load_era5.py`

 * *Files identical despite different names*

### Comparing `deafrica-tools-2.3.7/deafrica_tools/load_isda.py` & `deafrica_tools-2.3.8/deafrica_tools/load_isda.py`

 * *Files identical despite different names*

### Comparing `deafrica-tools-2.3.7/deafrica_tools/load_soil_moisture.py` & `deafrica_tools-2.3.8/deafrica_tools/load_soil_moisture.py`

 * *Files identical despite different names*

### Comparing `deafrica-tools-2.3.7/deafrica_tools/locales/fr/LC_MESSAGES/deafrica_tools.mo` & `deafrica_tools-2.3.8/deafrica_tools/locales/fr/LC_MESSAGES/deafrica_tools.mo`

 * *Files identical despite different names*

### Comparing `deafrica-tools-2.3.7/deafrica_tools/locales/fr/LC_MESSAGES/deafrica_tools.po` & `deafrica_tools-2.3.8/deafrica_tools/locales/fr/LC_MESSAGES/deafrica_tools.po`

 * *Files identical despite different names*

### Comparing `deafrica-tools-2.3.7/deafrica_tools/plotting.py` & `deafrica_tools-2.3.8/deafrica_tools/plotting.py`

 * *Files identical despite different names*

### Comparing `deafrica-tools-2.3.7/deafrica_tools/spatial.py` & `deafrica_tools-2.3.8/deafrica_tools/spatial.py`

 * *Files identical despite different names*

### Comparing `deafrica-tools-2.3.7/deafrica_tools/temporal.py` & `deafrica_tools-2.3.8/deafrica_tools/temporal.py`

 * *Files identical despite different names*

### Comparing `deafrica-tools-2.3.7/deafrica_tools/waterbodies.py` & `deafrica_tools-2.3.8/deafrica_tools/waterbodies.py`

 * *Files identical despite different names*

### Comparing `deafrica-tools-2.3.7/deafrica_tools/wetlands.py` & `deafrica_tools-2.3.8/deafrica_tools/wetlands.py`

 * *Files identical despite different names*

### Comparing `deafrica-tools-2.3.7/deafrica_tools.egg-info/PKG-INFO` & `deafrica_tools-2.3.8/deafrica_tools.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deafrica-tools
-Version: 2.3.7
+Version: 2.3.8
 Summary: Functions and algorithms for analysing Digital Earth Africa data.
 Author-email: Digital Earth Africa <systems@digitalearthafrica.org>
 Maintainer-email: Digital Earth Africa <systems@digitalearthafrica.org>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -275,25 +275,26 @@
 
 # Digital Earth Africa Tools Package
 
 Python functions and algorithms developed to assist in analysing Digital Earth Africa data (e.g. loading data, plotting, spatial analysis, machine learning).
 
 ## Installation
 
-This module is automatically installed on the Digital Earth Africa Sandbox. If for some reason the module isn't available on the Digital Earth Africa Sandbox, you can also `pip install` the module from the terminal.
+This module is automatically installed on the Digital Earth Africa Sandbox. If for some reason the module isn't available on the Digital Earth Africa Sandbox, or to upgrade the tools, you can `pip install` the module from the terminal.
 
-You can install the `deafrica-tools` package from PyPI using:
+You can install the latest version of `deafrica-tools` from PyPI using:
 
 ```
 python -m pip install --extra-index-url="https://packages.dea.ga.gov.au" deafrica-tools 
 ```
-or install the package from the `Tools` directory:
+
+or install the package directly from the `Tools` directory to incorperate local changes:
 
 ```
-python -m pip install --extra-index-url="https://packages.dea.ga.gov.au" -e Tools/
+python -m pip install --extra-index-url="https://packages.dea.ga.gov.au" Tools/
 ```
        
 To install this module from the source on any other system with `pip`:
 
 ```
 python -m pip install --extra-index-url="https://packages.dea.ga.gov.au" git+https://github.com/digitalearthafrica/deafrica-sandbox-notebooks.git#subdirectory=Tools
 ```
```

### Comparing `deafrica-tools-2.3.7/deafrica_tools.egg-info/SOURCES.txt` & `deafrica_tools-2.3.8/deafrica_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `deafrica-tools-2.3.7/index.rst` & `deafrica_tools-2.3.8/index.rst`

 * *Files identical despite different names*

### Comparing `deafrica-tools-2.3.7/pyproject.toml` & `deafrica_tools-2.3.8/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 [build-system]
 requires = ["setuptools>=61.0", "wheel", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "deafrica-tools"
-version = "2.3.7"
+version = "2.3.8"
+# reflect version changes in deafrica_tools/__init__.py
 
 description = "Functions and algorithms for analysing Digital Earth Africa data."
 authors = [{name = "Digital Earth Africa", email = "systems@digitalearthafrica.org"}]
 maintainers = [{name = "Digital Earth Africa", email = "systems@digitalearthafrica.org"}]
 readme = {file = "README.md", content-type = "text/markdown"}
 # If you change the License, remember to change the Trove Classifier!
 license = {file = "LICENSE"}
```

