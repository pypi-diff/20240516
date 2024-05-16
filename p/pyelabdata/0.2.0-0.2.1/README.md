# Comparing `tmp/pyelabdata-0.2.0.tar.gz` & `tmp/pyelabdata-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyelabdata-0.2.0.tar", last modified: Thu May 16 10:43:33 2024, max compression
+gzip compressed data, was "pyelabdata-0.2.1.tar", last modified: Thu May 16 10:51:50 2024, max compression
```

## Comparing `pyelabdata-0.2.0.tar` & `pyelabdata-0.2.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-16 10:43:33.732818 pyelabdata-0.2.0/
--rw-rw-rw-   0        0        0     1097 2024-01-25 17:49:20.000000 pyelabdata-0.2.0/LICENSE
--rw-rw-rw-   0        0        0    10904 2024-05-16 10:43:33.730818 pyelabdata-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     9934 2024-05-16 10:06:32.000000 pyelabdata-0.2.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-16 10:43:33.704819 pyelabdata-0.2.0/pyelabdata/
--rw-rw-rw-   0        0        0       27 2024-02-23 10:39:15.000000 pyelabdata-0.2.0/pyelabdata/__init__.py
--rw-rw-rw-   0        0        0    27062 2024-05-16 10:03:05.000000 pyelabdata-0.2.0/pyelabdata/pyelabdata.py
-drwxrwxrwx   0        0        0        0 2024-05-16 10:43:33.729820 pyelabdata-0.2.0/pyelabdata.egg-info/
--rw-rw-rw-   0        0        0    10904 2024-05-16 10:43:33.000000 pyelabdata-0.2.0/pyelabdata.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      249 2024-05-16 10:43:33.000000 pyelabdata-0.2.0/pyelabdata.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-16 10:43:33.000000 pyelabdata-0.2.0/pyelabdata.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       84 2024-05-16 10:43:33.000000 pyelabdata-0.2.0/pyelabdata.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-05-16 10:43:33.000000 pyelabdata-0.2.0/pyelabdata.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1167 2024-05-10 15:45:32.000000 pyelabdata-0.2.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-16 10:43:33.732818 pyelabdata-0.2.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-16 10:51:50.060470 pyelabdata-0.2.1/
+-rw-rw-rw-   0        0        0     1097 2024-01-25 17:49:20.000000 pyelabdata-0.2.1/LICENSE
+-rw-rw-rw-   0        0        0    10883 2024-05-16 10:51:50.058483 pyelabdata-0.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     9934 2024-05-16 10:06:32.000000 pyelabdata-0.2.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-16 10:51:50.030466 pyelabdata-0.2.1/pyelabdata/
+-rw-rw-rw-   0        0        0       27 2024-02-23 10:39:15.000000 pyelabdata-0.2.1/pyelabdata/__init__.py
+-rw-rw-rw-   0        0        0    27062 2024-05-16 10:03:05.000000 pyelabdata-0.2.1/pyelabdata/pyelabdata.py
+drwxrwxrwx   0        0        0        0 2024-05-16 10:51:50.057472 pyelabdata-0.2.1/pyelabdata.egg-info/
+-rw-rw-rw-   0        0        0    10883 2024-05-16 10:51:50.000000 pyelabdata-0.2.1/pyelabdata.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      249 2024-05-16 10:51:50.000000 pyelabdata-0.2.1/pyelabdata.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-16 10:51:50.000000 pyelabdata-0.2.1/pyelabdata.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       79 2024-05-16 10:51:50.000000 pyelabdata-0.2.1/pyelabdata.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-16 10:51:50.000000 pyelabdata-0.2.1/pyelabdata.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1154 2024-05-16 10:51:21.000000 pyelabdata-0.2.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-16 10:51:50.060470 pyelabdata-0.2.1/setup.cfg
```

### Comparing `pyelabdata-0.2.0/LICENSE` & `pyelabdata-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyelabdata-0.2.0/PKG-INFO` & `pyelabdata-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: pyelabdata
-Version: 0.2.0
+Version: 0.2.1
 Summary: pyelabdata provides functions for simple one-line access to data in eLabFTW
 Author-email: "Elektronikpraktikum, Department Physik, FAU Erlangen-Nürnberg" <physik-ep@fau.de>, "Michael Krieger, Lehrstuhl für Angewandte Physik, FAU Erlangen-Nürnberg" <michael.krieger@fau.de>
 Project-URL: Repository, https://github.com/FAU-PHYSIK-EP/pyelabdata
 Project-URL: Issues, https://github.com/FAU-PHYSIK-EP/pyelabdata/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: elabapi_python
 Requires-Dist: pandas
-Requires-Dist: json
 Requires-Dist: h5py
 Requires-Dist: ipyparams
 Requires-Dist: matplotlib
 Requires-Dist: pathlib
 Requires-Dist: datetime
 Requires-Dist: IPython
```

### Comparing `pyelabdata-0.2.0/README.md` & `pyelabdata-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `pyelabdata-0.2.0/pyelabdata/pyelabdata.py` & `pyelabdata-0.2.1/pyelabdata/pyelabdata.py`

 * *Files identical despite different names*

### Comparing `pyelabdata-0.2.0/pyelabdata.egg-info/PKG-INFO` & `pyelabdata-0.2.1/pyelabdata.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: pyelabdata
-Version: 0.2.0
+Version: 0.2.1
 Summary: pyelabdata provides functions for simple one-line access to data in eLabFTW
 Author-email: "Elektronikpraktikum, Department Physik, FAU Erlangen-Nürnberg" <physik-ep@fau.de>, "Michael Krieger, Lehrstuhl für Angewandte Physik, FAU Erlangen-Nürnberg" <michael.krieger@fau.de>
 Project-URL: Repository, https://github.com/FAU-PHYSIK-EP/pyelabdata
 Project-URL: Issues, https://github.com/FAU-PHYSIK-EP/pyelabdata/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: elabapi_python
 Requires-Dist: pandas
-Requires-Dist: json
 Requires-Dist: h5py
 Requires-Dist: ipyparams
 Requires-Dist: matplotlib
 Requires-Dist: pathlib
 Requires-Dist: datetime
 Requires-Dist: IPython
```

### Comparing `pyelabdata-0.2.0/pyproject.toml` & `pyelabdata-0.2.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pyelabdata"
-version = "0.2.0"
+version = "0.2.1"
 authors = [
     { name="Elektronikpraktikum, Department Physik, FAU Erlangen-Nürnberg", email="physik-ep@fau.de" },
     { name="Michael Krieger, Lehrstuhl für Angewandte Physik, FAU Erlangen-Nürnberg", email="michael.krieger@fau.de"}
 ]
 description = "pyelabdata provides functions for simple one-line access to data in eLabFTW"
 readme = "README.md"
 requires-python = ">=3.8"
@@ -23,15 +23,14 @@
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent"
 ]
 dependencies = [
     "numpy",
     "elabapi_python",
     "pandas",
-    "json",
     "h5py",
     "ipyparams",
     "matplotlib",
     "pathlib",
     "datetime",
     "IPython"
 ]
```

