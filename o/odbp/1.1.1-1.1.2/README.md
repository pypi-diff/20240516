# Comparing `tmp/odbp-1.1.1.tar.gz` & `tmp/odbp-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "odbp-1.1.1.tar", last modified: Mon Apr 29 22:12:51 2024, max compression
+gzip compressed data, was "odbp-1.1.2.tar", last modified: Tue May  7 18:05:53 2024, max compression
```

## Comparing `odbp-1.1.1.tar` & `odbp-1.1.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 clark     (1000) clark     (1000)        0 2024-04-29 22:12:51.943334 odbp-1.1.1/
--rw-r--r--   0 clark     (1000) clark     (1000)     1074 2024-04-29 21:57:07.000000 odbp-1.1.1/LICENSE
--rw-r--r--   0 clark     (1000) clark     (1000)     2908 2024-04-29 22:12:51.943334 odbp-1.1.1/PKG-INFO
--rw-r--r--   0 clark     (1000) clark     (1000)      668 2024-04-29 22:12:32.000000 odbp-1.1.1/README.md
--rw-r--r--   0 clark     (1000) clark     (1000)     1213 2024-04-29 22:12:32.000000 odbp-1.1.1/pyproject.toml
--rw-r--r--   0 clark     (1000) clark     (1000)       38 2024-04-29 22:12:51.943334 odbp-1.1.1/setup.cfg
-drwxr-xr-x   0 clark     (1000) clark     (1000)        0 2024-04-29 22:12:51.940000 odbp-1.1.1/src/
-drwxr-xr-x   0 clark     (1000) clark     (1000)        0 2024-04-29 22:12:51.943334 odbp-1.1.1/src/odbp/
--rw-r--r--   0 clark     (1000) clark     (1000)       80 2024-04-29 22:12:32.000000 odbp-1.1.1/src/odbp/__init__.py
-drwxr-xr-x   0 clark     (1000) clark     (1000)        0 2024-04-29 22:12:51.943334 odbp-1.1.1/src/odbp/data/
--rw-r--r--   0 clark     (1000) clark     (1000)     4808 2024-04-29 22:12:32.000000 odbp-1.1.1/src/odbp/data/config.toml
--rw-r--r--   0 clark     (1000) clark     (1000)    49418 2024-04-29 21:57:07.000000 odbp-1.1.1/src/odbp/data/odbp_views.toml
--rw-r--r--   0 clark     (1000) clark     (1000)      586 2024-04-29 21:57:07.000000 odbp-1.1.1/src/odbp/data_model.py
--rw-r--r--   0 clark     (1000) clark     (1000)      381 2024-04-29 21:57:07.000000 odbp-1.1.1/src/odbp/magic.py
--rw-r--r--   0 clark     (1000) clark     (1000)    38719 2024-04-29 22:12:32.000000 odbp-1.1.1/src/odbp/odbp.py
--rw-r--r--   0 clark     (1000) clark     (1000)    27454 2024-04-29 21:57:07.000000 odbp-1.1.1/src/odbp/odbp_settings.py
-drwxr-xr-x   0 clark     (1000) clark     (1000)        0 2024-04-29 22:12:51.943334 odbp-1.1.1/src/odbp/py2_scripts/
--rw-r--r--   0 clark     (1000) clark     (1000)    24893 2024-04-29 22:12:32.000000 odbp-1.1.1/src/odbp/py2_scripts/converter.py
--rw-r--r--   0 clark     (1000) clark     (1000)     5011 2024-04-29 22:12:32.000000 odbp-1.1.1/src/odbp/py2_scripts/odb_info_getter.py
--rw-r--r--   0 clark     (1000) clark     (1000)     6389 2024-04-29 22:12:32.000000 odbp-1.1.1/src/odbp/reader.py
--rw-r--r--   0 clark     (1000) clark     (1000)    14979 2024-04-29 22:12:32.000000 odbp-1.1.1/src/odbp/writer.py
-drwxr-xr-x   0 clark     (1000) clark     (1000)        0 2024-04-29 22:12:51.943334 odbp-1.1.1/src/odbp.egg-info/
--rw-r--r--   0 clark     (1000) clark     (1000)     2908 2024-04-29 22:12:51.000000 odbp-1.1.1/src/odbp.egg-info/PKG-INFO
--rw-r--r--   0 clark     (1000) clark     (1000)      464 2024-04-29 22:12:51.000000 odbp-1.1.1/src/odbp.egg-info/SOURCES.txt
--rw-r--r--   0 clark     (1000) clark     (1000)        1 2024-04-29 22:12:51.000000 odbp-1.1.1/src/odbp.egg-info/dependency_links.txt
--rw-r--r--   0 clark     (1000) clark     (1000)      157 2024-04-29 22:12:51.000000 odbp-1.1.1/src/odbp.egg-info/requires.txt
--rw-r--r--   0 clark     (1000) clark     (1000)        5 2024-04-29 22:12:51.000000 odbp-1.1.1/src/odbp.egg-info/top_level.txt
+drwxr-xr-x   0 clark     (1000) clark     (1000)        0 2024-05-07 18:05:53.780002 odbp-1.1.2/
+-rw-r--r--   0 clark     (1000) clark     (1000)     1074 2024-04-29 21:57:07.000000 odbp-1.1.2/LICENSE
+-rw-r--r--   0 clark     (1000) clark     (1000)     2914 2024-05-07 18:05:53.776668 odbp-1.1.2/PKG-INFO
+-rw-r--r--   0 clark     (1000) clark     (1000)      668 2024-04-29 22:12:32.000000 odbp-1.1.2/README.md
+-rw-r--r--   0 clark     (1000) clark     (1000)     1212 2024-05-07 18:02:55.000000 odbp-1.1.2/pyproject.toml
+-rw-r--r--   0 clark     (1000) clark     (1000)       38 2024-05-07 18:05:53.780002 odbp-1.1.2/setup.cfg
+drwxr-xr-x   0 clark     (1000) clark     (1000)        0 2024-05-07 18:05:53.773335 odbp-1.1.2/src/
+drwxr-xr-x   0 clark     (1000) clark     (1000)        0 2024-05-07 18:05:53.776668 odbp-1.1.2/src/odbp/
+-rw-r--r--   0 clark     (1000) clark     (1000)       80 2024-05-07 18:02:55.000000 odbp-1.1.2/src/odbp/__init__.py
+drwxr-xr-x   0 clark     (1000) clark     (1000)        0 2024-05-07 18:05:53.776668 odbp-1.1.2/src/odbp/data/
+-rw-r--r--   0 clark     (1000) clark     (1000)     4808 2024-04-29 22:12:32.000000 odbp-1.1.2/src/odbp/data/config.toml
+-rw-r--r--   0 clark     (1000) clark     (1000)    49418 2024-04-29 21:57:07.000000 odbp-1.1.2/src/odbp/data/odbp_views.toml
+-rw-r--r--   0 clark     (1000) clark     (1000)      586 2024-04-29 21:57:07.000000 odbp-1.1.2/src/odbp/data_model.py
+-rw-r--r--   0 clark     (1000) clark     (1000)      381 2024-04-29 21:57:07.000000 odbp-1.1.2/src/odbp/magic.py
+-rw-r--r--   0 clark     (1000) clark     (1000)    38719 2024-04-29 22:12:32.000000 odbp-1.1.2/src/odbp/odbp.py
+-rw-r--r--   0 clark     (1000) clark     (1000)    27454 2024-04-29 21:57:07.000000 odbp-1.1.2/src/odbp/odbp_settings.py
+drwxr-xr-x   0 clark     (1000) clark     (1000)        0 2024-05-07 18:05:53.776668 odbp-1.1.2/src/odbp/py2_scripts/
+-rw-r--r--   0 clark     (1000) clark     (1000)    24893 2024-04-29 22:12:32.000000 odbp-1.1.2/src/odbp/py2_scripts/converter.py
+-rw-r--r--   0 clark     (1000) clark     (1000)     5011 2024-04-29 22:12:32.000000 odbp-1.1.2/src/odbp/py2_scripts/odb_info_getter.py
+-rw-r--r--   0 clark     (1000) clark     (1000)     6389 2024-04-29 22:12:32.000000 odbp-1.1.2/src/odbp/reader.py
+-rw-r--r--   0 clark     (1000) clark     (1000)    14457 2024-05-07 18:02:55.000000 odbp-1.1.2/src/odbp/writer.py
+drwxr-xr-x   0 clark     (1000) clark     (1000)        0 2024-05-07 18:05:53.776668 odbp-1.1.2/src/odbp.egg-info/
+-rw-r--r--   0 clark     (1000) clark     (1000)     2914 2024-05-07 18:05:53.000000 odbp-1.1.2/src/odbp.egg-info/PKG-INFO
+-rw-r--r--   0 clark     (1000) clark     (1000)      464 2024-05-07 18:05:53.000000 odbp-1.1.2/src/odbp.egg-info/SOURCES.txt
+-rw-r--r--   0 clark     (1000) clark     (1000)        1 2024-05-07 18:05:53.000000 odbp-1.1.2/src/odbp.egg-info/dependency_links.txt
+-rw-r--r--   0 clark     (1000) clark     (1000)      163 2024-05-07 18:05:53.000000 odbp-1.1.2/src/odbp.egg-info/requires.txt
+-rw-r--r--   0 clark     (1000) clark     (1000)        5 2024-05-07 18:05:53.000000 odbp-1.1.2/src/odbp.egg-info/top_level.txt
```

### Comparing `odbp-1.1.1/LICENSE` & `odbp-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `odbp-1.1.1/PKG-INFO` & `odbp-1.1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odbp
-Version: 1.1.1
+Version: 1.1.2
 Summary: Python3 API for Abaqus .odb files. Focused on Additive Manufacturing Thermal Transfer
 Author-email: Clark Hensley <clarkhensley@duck.com>
 Maintainer-email: Clark Hensley <clarkhensley@duck.com>
 License: MIT License
         
         Copyright (c) 2024 Matthew W. Priddy
         
@@ -34,15 +34,15 @@
 License-File: LICENSE
 Requires-Dist: platformdirs
 Requires-Dist: h5py
 Requires-Dist: numpy
 Requires-Dist: pandas
 Requires-Dist: pyreadline3; platform_system == "Windows"
 Provides-Extra: all
-Requires-Dist: plot; extra == "all"
+Requires-Dist: odbp[plot]; extra == "all"
 Provides-Extra: plot
 Requires-Dist: polyscope; extra == "plot"
 Requires-Dist: scipy; extra == "plot"
 Requires-Dist: tomli>=1.1.0; python_version < "3.11" and extra == "plot"
 
 # ODBP
```

### Comparing `odbp-1.1.1/README.md` & `odbp-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `odbp-1.1.1/pyproject.toml` & `odbp-1.1.2/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -12,17 +12,15 @@
 "numpy",
 "pandas",
 "pyreadline3; platform_system == 'Windows'",
 ]
 dynamic = ["version",]
 
 [project.optional-dependencies]
-all = [
-    "plot",
-]
+all = ["odbp[plot]"]
 plot = [
     "polyscope",
     "scipy",
     "tomli>=1.1.0; python_version < '3.11'",
 ]
 
 [project.urls]
```

### Comparing `odbp-1.1.1/src/odbp/data/config.toml` & `odbp-1.1.2/src/odbp/data/config.toml`

 * *Files identical despite different names*

### Comparing `odbp-1.1.1/src/odbp/data/odbp_views.toml` & `odbp-1.1.2/src/odbp/data/odbp_views.toml`

 * *Files identical despite different names*

### Comparing `odbp-1.1.1/src/odbp/data_model.py` & `odbp-1.1.2/src/odbp/data_model.py`

 * *Files identical despite different names*

### Comparing `odbp-1.1.1/src/odbp/odbp.py` & `odbp-1.1.2/src/odbp/odbp.py`

 * *Files identical despite different names*

### Comparing `odbp-1.1.1/src/odbp/odbp_settings.py` & `odbp-1.1.2/src/odbp/odbp_settings.py`

 * *Files identical despite different names*

### Comparing `odbp-1.1.1/src/odbp/py2_scripts/converter.py` & `odbp-1.1.2/src/odbp/py2_scripts/converter.py`

 * *Files identical despite different names*

### Comparing `odbp-1.1.1/src/odbp/py2_scripts/odb_info_getter.py` & `odbp-1.1.2/src/odbp/py2_scripts/odb_info_getter.py`

 * *Files identical despite different names*

### Comparing `odbp-1.1.1/src/odbp/reader.py` & `odbp-1.1.2/src/odbp/reader.py`

 * *Files identical despite different names*

### Comparing `odbp-1.1.1/src/odbp/writer.py` & `odbp-1.1.2/src/odbp/writer.py`

 * *Files 2% similar despite different names*

```diff
@@ -126,25 +126,14 @@
                         with open(input_pickle, "rb") as pf:
                             part_to_elementsets_mapping = pickle.load(pf)
 
                     case "part_to_nodesets_mapping":
                         with open(input_pickle, "rb") as pf:
                             part_to_nodesets_mapping = pickle.load(pf)
 
-                    case "element_connectivity":
-                        with open(input_pickle, "rb") as pf:
-                            element_connectivity_dict: dict[int, npt.NDArray] = pickle.load(pf)
-                            k: int
-                            v: npt.NDArray
-                            temp_element_connectivity: list[tuple[int, npt.NDArray]] = [(k, v) for k, v in element_connectivity_dict.items()]
-                            # Sort by label
-                            e: tuple[int, npt.NDArray]
-                            temp_element_connectivity = sorted(temp_element_connectivity, key=lambda e: e[0])
-                            element_connectivity = np.array([e[1] for e in temp_element_connectivity])
-
                     case _:
                         raise Exception(f"Unknown pickle file: {input_pickle}")
 
             elif input_pickle_or_npz.suffix == ".npz":
                 npz_file: pathlib.Path = input_pickle_or_npz
                 with warnings.catch_warnings():
                     warnings.filterwarnings("ignore", category=UserWarning, append=True)
@@ -157,14 +146,18 @@
                                 data_len: int = node_coords_data.shape[0]
                                 node_coords = {
                                     "X": node_coords_data[:, 0].reshape((data_len, 1)),
                                     "Y": node_coords_data[:, 1].reshape((data_len, 1)),
                                     "Z": node_coords_data[:, 2].reshape((data_len, 1)),
                                 }
 
+                        case "element_connectivity":
+                            with np.load(npz_file) as data_file:
+                                element_connectivity: npt.NDArray = data_file[data_file.files[0]]
+
                         case _:
                             raise Exception(f"Unknown npz file: {npz_file}")
 
             else:
                 raise ValueError(f"Unexpected file: {input_pickle_or_npz}")
 
     step_dict: dict[str, dict[int, dict[str, npt.NDArray | dict[str, npt.NDArray]]]]
```

### Comparing `odbp-1.1.1/src/odbp.egg-info/PKG-INFO` & `odbp-1.1.2/src/odbp.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odbp
-Version: 1.1.1
+Version: 1.1.2
 Summary: Python3 API for Abaqus .odb files. Focused on Additive Manufacturing Thermal Transfer
 Author-email: Clark Hensley <clarkhensley@duck.com>
 Maintainer-email: Clark Hensley <clarkhensley@duck.com>
 License: MIT License
         
         Copyright (c) 2024 Matthew W. Priddy
         
@@ -34,15 +34,15 @@
 License-File: LICENSE
 Requires-Dist: platformdirs
 Requires-Dist: h5py
 Requires-Dist: numpy
 Requires-Dist: pandas
 Requires-Dist: pyreadline3; platform_system == "Windows"
 Provides-Extra: all
-Requires-Dist: plot; extra == "all"
+Requires-Dist: odbp[plot]; extra == "all"
 Provides-Extra: plot
 Requires-Dist: polyscope; extra == "plot"
 Requires-Dist: scipy; extra == "plot"
 Requires-Dist: tomli>=1.1.0; python_version < "3.11" and extra == "plot"
 
 # ODBP
```

