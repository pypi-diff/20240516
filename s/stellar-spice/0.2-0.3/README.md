# Comparing `tmp/stellar_spice-0.2.tar.gz` & `tmp/stellar_spice-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stellar_spice-0.2.tar", last modified: Thu May 16 01:13:28 2024, max compression
+gzip compressed data, was "stellar_spice-0.3.tar", last modified: Thu May 16 01:23:49 2024, max compression
```

## Comparing `stellar_spice-0.2.tar` & `stellar_spice-0.3.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 01:13:28.889384 stellar_spice-0.2/
--rw-r--r--   0 runner    (1001) docker     (127)      863 2024-05-16 01:13:28.889384 stellar_spice-0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      331 2024-05-16 01:13:19.000000 stellar_spice-0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      774 2024-05-16 01:13:19.000000 stellar_spice-0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 01:13:28.889384 stellar_spice-0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 01:13:28.881384 stellar_spice-0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 01:13:28.881384 stellar_spice-0.2/src/spice/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 01:13:19.000000 stellar_spice-0.2/src/spice/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 01:13:28.881384 stellar_spice-0.2/src/spice/geometry/
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-16 01:13:19.000000 stellar_spice-0.2/src/spice/geometry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5615 2024-05-16 01:13:19.000000 stellar_spice-0.2/src/spice/geometry/sutherland_hodgman.py
--rw-r--r--   0 runner    (1001) docker     (127)     4984 2024-05-16 01:13:19.000000 stellar_spice-0.2/src/spice/geometry/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 01:13:28.885384 stellar_spice-0.2/src/spice/models/
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-16 01:13:19.000000 stellar_spice-0.2/src/spice/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4671 2024-05-16 01:13:19.000000 stellar_spice-0.2/src/spice/models/binary.py
--rw-r--r--   0 runner    (1001) docker     (127)     8741 2024-05-16 01:13:19.000000 stellar_spice-0.2/src/spice/models/mesh_generation.py
--rw-r--r--   0 runner    (1001) docker     (127)     4643 2024-05-16 01:13:19.000000 stellar_spice-0.2/src/spice/models/mesh_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3830 2024-05-16 01:13:19.000000 stellar_spice-0.2/src/spice/models/mesh_transform.py
--rw-r--r--   0 runner    (1001) docker     (127)     7736 2024-05-16 01:13:19.000000 stellar_spice-0.2/src/spice/models/mesh_view.py
--rw-r--r--   0 runner    (1001) docker     (127)     3198 2024-05-16 01:13:19.000000 stellar_spice-0.2/src/spice/models/orbit_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3121 2024-05-16 01:13:19.000000 stellar_spice-0.2/src/spice/models/phoebe_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3179 2024-05-16 01:13:19.000000 stellar_spice-0.2/src/spice/models/spots.py
--rw-r--r--   0 runner    (1001) docker     (127)     4193 2024-05-16 01:13:19.000000 stellar_spice-0.2/src/spice/models/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 01:13:28.885384 stellar_spice-0.2/src/spice/phoebe_model/
--rw-r--r--   0 runner    (1001) docker     (127)     6752 2024-05-16 01:13:19.000000 stellar_spice-0.2/src/spice/phoebe_model/DI-Her-meshes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 01:13:28.885384 stellar_spice-0.2/src/spice/plots/
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-16 01:13:19.000000 stellar_spice-0.2/src/spice/plots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14238 2024-05-16 01:13:19.000000 stellar_spice-0.2/src/spice/plots/plot_mesh.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 01:13:28.885384 stellar_spice-0.2/src/spice/spectrum/
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-16 01:13:19.000000 stellar_spice-0.2/src/spice/spectrum/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7209 2024-05-16 01:13:19.000000 stellar_spice-0.2/src/spice/spectrum/filter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 01:13:28.885384 stellar_spice-0.2/src/spice/spectrum/filter_data/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 01:13:19.000000 stellar_spice-0.2/src/spice/spectrum/filter_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1777 2024-05-16 01:13:19.000000 stellar_spice-0.2/src/spice/spectrum/planck_law.py
--rw-r--r--   0 runner    (1001) docker     (127)    10303 2024-05-16 01:13:19.000000 stellar_spice-0.2/src/spice/spectrum/spectrum.py
--rw-r--r--   0 runner    (1001) docker     (127)     8630 2024-05-16 01:13:19.000000 stellar_spice-0.2/src/spice/spectrum/spectrum_korg.py
--rw-r--r--   0 runner    (1001) docker     (127)     5242 2024-05-16 01:13:19.000000 stellar_spice-0.2/src/spice/spectrum/spectrum_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)      927 2024-05-16 01:13:19.000000 stellar_spice-0.2/src/spice/spectrum/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 01:13:28.885384 stellar_spice-0.2/src/spice/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-16 01:13:19.000000 stellar_spice-0.2/src/spice/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-16 01:13:19.000000 stellar_spice-0.2/src/spice/utils/warnings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 01:13:28.889384 stellar_spice-0.2/src/stellar_spice.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      863 2024-05-16 01:13:28.000000 stellar_spice-0.2/src/stellar_spice.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-05-16 01:13:28.000000 stellar_spice-0.2/src/stellar_spice.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 01:13:28.000000 stellar_spice-0.2/src/stellar_spice.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-05-16 01:13:28.000000 stellar_spice-0.2/src/stellar_spice.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-16 01:13:28.000000 stellar_spice-0.2/src/stellar_spice.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 01:23:49.145123 stellar_spice-0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)      895 2024-05-16 01:23:49.145123 stellar_spice-0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-05-16 01:23:41.000000 stellar_spice-0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      798 2024-05-16 01:23:41.000000 stellar_spice-0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 01:23:49.145123 stellar_spice-0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 01:23:49.137123 stellar_spice-0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 01:23:49.137123 stellar_spice-0.3/src/spice/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 01:23:41.000000 stellar_spice-0.3/src/spice/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 01:23:49.137123 stellar_spice-0.3/src/spice/geometry/
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-16 01:23:41.000000 stellar_spice-0.3/src/spice/geometry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5615 2024-05-16 01:23:41.000000 stellar_spice-0.3/src/spice/geometry/sutherland_hodgman.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4984 2024-05-16 01:23:41.000000 stellar_spice-0.3/src/spice/geometry/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 01:23:49.141123 stellar_spice-0.3/src/spice/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-16 01:23:41.000000 stellar_spice-0.3/src/spice/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4671 2024-05-16 01:23:41.000000 stellar_spice-0.3/src/spice/models/binary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8741 2024-05-16 01:23:41.000000 stellar_spice-0.3/src/spice/models/mesh_generation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4643 2024-05-16 01:23:41.000000 stellar_spice-0.3/src/spice/models/mesh_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3830 2024-05-16 01:23:41.000000 stellar_spice-0.3/src/spice/models/mesh_transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7736 2024-05-16 01:23:41.000000 stellar_spice-0.3/src/spice/models/mesh_view.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3198 2024-05-16 01:23:41.000000 stellar_spice-0.3/src/spice/models/orbit_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3121 2024-05-16 01:23:41.000000 stellar_spice-0.3/src/spice/models/phoebe_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3179 2024-05-16 01:23:41.000000 stellar_spice-0.3/src/spice/models/spots.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4193 2024-05-16 01:23:41.000000 stellar_spice-0.3/src/spice/models/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 01:23:49.141123 stellar_spice-0.3/src/spice/phoebe_model/
+-rw-r--r--   0 runner    (1001) docker     (127)     6752 2024-05-16 01:23:41.000000 stellar_spice-0.3/src/spice/phoebe_model/DI-Her-meshes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 01:23:49.141123 stellar_spice-0.3/src/spice/plots/
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-16 01:23:41.000000 stellar_spice-0.3/src/spice/plots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14238 2024-05-16 01:23:41.000000 stellar_spice-0.3/src/spice/plots/plot_mesh.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 01:23:49.141123 stellar_spice-0.3/src/spice/spectrum/
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-16 01:23:41.000000 stellar_spice-0.3/src/spice/spectrum/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7209 2024-05-16 01:23:41.000000 stellar_spice-0.3/src/spice/spectrum/filter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 01:23:49.141123 stellar_spice-0.3/src/spice/spectrum/filter_data/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 01:23:41.000000 stellar_spice-0.3/src/spice/spectrum/filter_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1777 2024-05-16 01:23:41.000000 stellar_spice-0.3/src/spice/spectrum/planck_law.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10303 2024-05-16 01:23:41.000000 stellar_spice-0.3/src/spice/spectrum/spectrum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8630 2024-05-16 01:23:42.000000 stellar_spice-0.3/src/spice/spectrum/spectrum_korg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5242 2024-05-16 01:23:42.000000 stellar_spice-0.3/src/spice/spectrum/spectrum_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-05-16 01:23:42.000000 stellar_spice-0.3/src/spice/spectrum/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 01:23:49.141123 stellar_spice-0.3/src/spice/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-16 01:23:42.000000 stellar_spice-0.3/src/spice/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-16 01:23:42.000000 stellar_spice-0.3/src/spice/utils/warnings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 01:23:49.145123 stellar_spice-0.3/src/stellar_spice.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      895 2024-05-16 01:23:49.000000 stellar_spice-0.3/src/stellar_spice.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-05-16 01:23:49.000000 stellar_spice-0.3/src/stellar_spice.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 01:23:49.000000 stellar_spice-0.3/src/stellar_spice.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      205 2024-05-16 01:23:49.000000 stellar_spice-0.3/src/stellar_spice.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-16 01:23:49.000000 stellar_spice-0.3/src/stellar_spice.egg-info/top_level.txt
```

### Comparing `stellar_spice-0.2/pyproject.toml` & `stellar_spice-0.3/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 [build-system]
 requires = ["setuptools >= 61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "stellar-spice"
-version = "0.2"
+version = "0.3"
 readme = "README.md"
 dependencies = [
+    "celluloid~=0.2.0",
     "jax~=0.4.24",
     "jaxlib~=0.4.24",
     "numpy~=1.26.4",
     "flax~=0.8.1",
     "joblib~=1.3.2",
     "transformer-payne~=0.5"
 ]
```

### Comparing `stellar_spice-0.2/src/spice/geometry/sutherland_hodgman.py` & `stellar_spice-0.3/src/spice/geometry/sutherland_hodgman.py`

 * *Files identical despite different names*

### Comparing `stellar_spice-0.2/src/spice/geometry/utils.py` & `stellar_spice-0.3/src/spice/geometry/utils.py`

 * *Files identical despite different names*

### Comparing `stellar_spice-0.2/src/spice/models/binary.py` & `stellar_spice-0.3/src/spice/models/binary.py`

 * *Files identical despite different names*

### Comparing `stellar_spice-0.2/src/spice/models/mesh_generation.py` & `stellar_spice-0.3/src/spice/models/mesh_generation.py`

 * *Files identical despite different names*

### Comparing `stellar_spice-0.2/src/spice/models/mesh_model.py` & `stellar_spice-0.3/src/spice/models/mesh_model.py`

 * *Files identical despite different names*

### Comparing `stellar_spice-0.2/src/spice/models/mesh_transform.py` & `stellar_spice-0.3/src/spice/models/mesh_transform.py`

 * *Files identical despite different names*

### Comparing `stellar_spice-0.2/src/spice/models/mesh_view.py` & `stellar_spice-0.3/src/spice/models/mesh_view.py`

 * *Files identical despite different names*

### Comparing `stellar_spice-0.2/src/spice/models/orbit_utils.py` & `stellar_spice-0.3/src/spice/models/orbit_utils.py`

 * *Files identical despite different names*

### Comparing `stellar_spice-0.2/src/spice/models/phoebe_utils.py` & `stellar_spice-0.3/src/spice/models/phoebe_utils.py`

 * *Files identical despite different names*

### Comparing `stellar_spice-0.2/src/spice/models/spots.py` & `stellar_spice-0.3/src/spice/models/spots.py`

 * *Files identical despite different names*

### Comparing `stellar_spice-0.2/src/spice/models/utils.py` & `stellar_spice-0.3/src/spice/models/utils.py`

 * *Files identical despite different names*

### Comparing `stellar_spice-0.2/src/spice/phoebe_model/DI-Her-meshes.py` & `stellar_spice-0.3/src/spice/phoebe_model/DI-Her-meshes.py`

 * *Files identical despite different names*

### Comparing `stellar_spice-0.2/src/spice/plots/plot_mesh.py` & `stellar_spice-0.3/src/spice/plots/plot_mesh.py`

 * *Files identical despite different names*

### Comparing `stellar_spice-0.2/src/spice/spectrum/filter.py` & `stellar_spice-0.3/src/spice/spectrum/filter.py`

 * *Files identical despite different names*

### Comparing `stellar_spice-0.2/src/spice/spectrum/planck_law.py` & `stellar_spice-0.3/src/spice/spectrum/planck_law.py`

 * *Files identical despite different names*

### Comparing `stellar_spice-0.2/src/spice/spectrum/spectrum.py` & `stellar_spice-0.3/src/spice/spectrum/spectrum.py`

 * *Files identical despite different names*

### Comparing `stellar_spice-0.2/src/spice/spectrum/spectrum_korg.py` & `stellar_spice-0.3/src/spice/spectrum/spectrum_korg.py`

 * *Files identical despite different names*

### Comparing `stellar_spice-0.2/src/spice/spectrum/spectrum_transformer.py` & `stellar_spice-0.3/src/spice/spectrum/spectrum_transformer.py`

 * *Files identical despite different names*

### Comparing `stellar_spice-0.2/src/spice/spectrum/utils.py` & `stellar_spice-0.3/src/spice/spectrum/utils.py`

 * *Files identical despite different names*

### Comparing `stellar_spice-0.2/src/stellar_spice.egg-info/SOURCES.txt` & `stellar_spice-0.3/src/stellar_spice.egg-info/SOURCES.txt`

 * *Files identical despite different names*

