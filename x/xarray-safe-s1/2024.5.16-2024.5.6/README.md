# Comparing `tmp/xarray_safe_s1-2024.5.16.tar.gz` & `tmp/xarray_safe_s1-2024.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xarray_safe_s1-2024.5.16.tar", last modified: Thu May 16 09:40:10 2024, max compression
+gzip compressed data, was "xarray_safe_s1-2024.5.6.tar", last modified: Mon May  6 12:40:39 2024, max compression
```

## Comparing `xarray_safe_s1-2024.5.16.tar` & `xarray_safe_s1-2024.5.6.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:40:10.032033 xarray_safe_s1-2024.5.16/
--rw-r--r--   0 runner    (1001) docker     (127)      349 2024-05-16 09:40:00.000000 xarray_safe_s1-2024.5.16/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:40:10.024033 xarray_safe_s1-2024.5.16/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-16 09:40:00.000000 xarray_safe_s1-2024.5.16/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:40:10.024033 xarray_safe_s1-2024.5.16/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      923 2024-05-16 09:40:00.000000 xarray_safe_s1-2024.5.16/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-05-16 09:40:00.000000 xarray_safe_s1-2024.5.16/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      958 2024-05-16 09:40:00.000000 xarray_safe_s1-2024.5.16/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      418 2024-05-16 09:40:00.000000 xarray_safe_s1-2024.5.16/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-05-16 09:40:00.000000 xarray_safe_s1-2024.5.16/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     8257 2024-05-16 09:40:10.032033 xarray_safe_s1-2024.5.16/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7750 2024-05-16 09:40:00.000000 xarray_safe_s1-2024.5.16/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:40:10.024033 xarray_safe_s1-2024.5.16/ci/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:40:10.024033 xarray_safe_s1-2024.5.16/ci/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-05-16 09:40:00.000000 xarray_safe_s1-2024.5.16/ci/requirements/docs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      534 2024-05-16 09:40:00.000000 xarray_safe_s1-2024.5.16/ci/requirements/environment.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:40:10.028033 xarray_safe_s1-2024.5.16/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-16 09:40:00.000000 xarray_safe_s1-2024.5.16/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:40:10.024033 xarray_safe_s1-2024.5.16/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:40:10.028033 xarray_safe_s1-2024.5.16/docs/_static/css/
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-16 09:40:00.000000 xarray_safe_s1-2024.5.16/docs/_static/css/xsar.css
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-16 09:40:00.000000 xarray_safe_s1-2024.5.16/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3353 2024-05-16 09:40:00.000000 xarray_safe_s1-2024.5.16/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:40:10.028033 xarray_safe_s1-2024.5.16/docs/examples/
--rw-r--r--   0 runner    (1001) docker     (127)    10471 2024-05-16 09:40:00.000000 xarray_safe_s1-2024.5.16/docs/examples/simple_tutorial.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     2292 2024-05-16 09:40:00.000000 xarray_safe_s1-2024.5.16/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-05-16 09:40:00.000000 xarray_safe_s1-2024.5.16/docs/installing.rst
--rw-r--r--   0 runner    (1001) docker     (127)      800 2024-05-16 09:40:00.000000 xarray_safe_s1-2024.5.16/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-16 09:40:00.000000 xarray_safe_s1-2024.5.16/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:40:10.028033 xarray_safe_s1-2024.5.16/highleveltests/
--rw-r--r--   0 runner    (1001) docker     (127)      374 2024-05-16 09:40:00.000000 xarray_safe_s1-2024.5.16/highleveltests/open_SLC_IW.py
--rw-r--r--   0 runner    (1001) docker     (127)     1674 2024-05-16 09:40:00.000000 xarray_safe_s1-2024.5.16/highleveltests/open_SLC_IW_S3.py
--rw-r--r--   0 runner    (1001) docker     (127)      705 2024-05-16 09:40:00.000000 xarray_safe_s1-2024.5.16/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:40:10.028033 xarray_safe_s1-2024.5.16/safe_s1/
--rw-r--r--   0 runner    (1001) docker     (127)      338 2024-05-16 09:40:00.000000 xarray_safe_s1-2024.5.16/safe_s1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-16 09:40:00.000000 xarray_safe_s1-2024.5.16/safe_s1/config.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-05-16 09:40:00.000000 xarray_safe_s1-2024.5.16/safe_s1/getconfig.py
--rw-r--r--   0 runner    (1001) docker     (127)    29355 2024-05-16 09:40:00.000000 xarray_safe_s1-2024.5.16/safe_s1/reader.py
--rw-r--r--   0 runner    (1001) docker     (127)    52508 2024-05-16 09:40:00.000000 xarray_safe_s1-2024.5.16/safe_s1/sentinel1_xml_mappings.py
--rw-r--r--   0 runner    (1001) docker     (127)     5503 2024-05-16 09:40:00.000000 xarray_safe_s1-2024.5.16/safe_s1/xml_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 09:40:10.032033 xarray_safe_s1-2024.5.16/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:40:10.028033 xarray_safe_s1-2024.5.16/test/
--rw-r--r--   0 runner    (1001) docker     (127)      891 2024-05-16 09:40:00.000000 xarray_safe_s1-2024.5.16/test/test_s1reader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:40:10.028033 xarray_safe_s1-2024.5.16/xarray_safe_s1.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8257 2024-05-16 09:40:10.000000 xarray_safe_s1-2024.5.16/xarray_safe_s1.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      785 2024-05-16 09:40:10.000000 xarray_safe_s1-2024.5.16/xarray_safe_s1.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 09:40:10.000000 xarray_safe_s1-2024.5.16/xarray_safe_s1.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-16 09:40:10.000000 xarray_safe_s1-2024.5.16/xarray_safe_s1.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-16 09:40:10.000000 xarray_safe_s1-2024.5.16/xarray_safe_s1.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 12:40:39.206913 xarray_safe_s1-2024.5.6/
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-05-06 12:40:29.000000 xarray_safe_s1-2024.5.6/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 12:40:39.202913 xarray_safe_s1-2024.5.6/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-06 12:40:29.000000 xarray_safe_s1-2024.5.6/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 12:40:39.202913 xarray_safe_s1-2024.5.6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      923 2024-05-06 12:40:29.000000 xarray_safe_s1-2024.5.6/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-05-06 12:40:29.000000 xarray_safe_s1-2024.5.6/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      958 2024-05-06 12:40:29.000000 xarray_safe_s1-2024.5.6/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-05-06 12:40:29.000000 xarray_safe_s1-2024.5.6/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-05-06 12:40:29.000000 xarray_safe_s1-2024.5.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     8256 2024-05-06 12:40:39.206913 xarray_safe_s1-2024.5.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7750 2024-05-06 12:40:29.000000 xarray_safe_s1-2024.5.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 12:40:39.198913 xarray_safe_s1-2024.5.6/ci/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 12:40:39.202913 xarray_safe_s1-2024.5.6/ci/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-05-06 12:40:29.000000 xarray_safe_s1-2024.5.6/ci/requirements/docs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      534 2024-05-06 12:40:29.000000 xarray_safe_s1-2024.5.6/ci/requirements/environment.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 12:40:39.202913 xarray_safe_s1-2024.5.6/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-06 12:40:29.000000 xarray_safe_s1-2024.5.6/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 12:40:39.198913 xarray_safe_s1-2024.5.6/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 12:40:39.202913 xarray_safe_s1-2024.5.6/docs/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-06 12:40:29.000000 xarray_safe_s1-2024.5.6/docs/_static/css/xsar.css
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-06 12:40:29.000000 xarray_safe_s1-2024.5.6/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3353 2024-05-06 12:40:29.000000 xarray_safe_s1-2024.5.6/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 12:40:39.202913 xarray_safe_s1-2024.5.6/docs/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)    10471 2024-05-06 12:40:29.000000 xarray_safe_s1-2024.5.6/docs/examples/simple_tutorial.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     2292 2024-05-06 12:40:29.000000 xarray_safe_s1-2024.5.6/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-05-06 12:40:29.000000 xarray_safe_s1-2024.5.6/docs/installing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-05-06 12:40:29.000000 xarray_safe_s1-2024.5.6/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-06 12:40:29.000000 xarray_safe_s1-2024.5.6/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 12:40:39.202913 xarray_safe_s1-2024.5.6/highleveltests/
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-05-06 12:40:29.000000 xarray_safe_s1-2024.5.6/highleveltests/open_SLC_IW.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1674 2024-05-06 12:40:29.000000 xarray_safe_s1-2024.5.6/highleveltests/open_SLC_IW_S3.py
+-rw-r--r--   0 runner    (1001) docker     (127)      705 2024-05-06 12:40:29.000000 xarray_safe_s1-2024.5.6/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 12:40:39.206913 xarray_safe_s1-2024.5.6/safe_s1/
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2024-05-06 12:40:29.000000 xarray_safe_s1-2024.5.6/safe_s1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-06 12:40:29.000000 xarray_safe_s1-2024.5.6/safe_s1/config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-05-06 12:40:29.000000 xarray_safe_s1-2024.5.6/safe_s1/getconfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29089 2024-05-06 12:40:29.000000 xarray_safe_s1-2024.5.6/safe_s1/reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52508 2024-05-06 12:40:29.000000 xarray_safe_s1-2024.5.6/safe_s1/sentinel1_xml_mappings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5503 2024-05-06 12:40:29.000000 xarray_safe_s1-2024.5.6/safe_s1/xml_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 12:40:39.206913 xarray_safe_s1-2024.5.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 12:40:39.206913 xarray_safe_s1-2024.5.6/test/
+-rw-r--r--   0 runner    (1001) docker     (127)      891 2024-05-06 12:40:29.000000 xarray_safe_s1-2024.5.6/test/test_s1reader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 12:40:39.206913 xarray_safe_s1-2024.5.6/xarray_safe_s1.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8256 2024-05-06 12:40:39.000000 xarray_safe_s1-2024.5.6/xarray_safe_s1.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      785 2024-05-06 12:40:39.000000 xarray_safe_s1-2024.5.6/xarray_safe_s1.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 12:40:39.000000 xarray_safe_s1-2024.5.6/xarray_safe_s1.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-06 12:40:39.000000 xarray_safe_s1-2024.5.6/xarray_safe_s1.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-06 12:40:39.000000 xarray_safe_s1-2024.5.6/xarray_safe_s1.egg-info/top_level.txt
```

### Comparing `xarray_safe_s1-2024.5.16/.github/workflows/publish.yml` & `xarray_safe_s1-2024.5.6/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `xarray_safe_s1-2024.5.16/.pre-commit-config.yaml` & `xarray_safe_s1-2024.5.6/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `xarray_safe_s1-2024.5.16/LICENSE` & `xarray_safe_s1-2024.5.6/LICENSE`

 * *Files identical despite different names*

### Comparing `xarray_safe_s1-2024.5.16/PKG-INFO` & `xarray_safe_s1-2024.5.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xarray-safe-s1
-Version: 2024.5.16
+Version: 2024.5.6
 License: MIT
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: geopandas
 Requires-Dist: numpy
 Requires-Dist: xarray
```

### Comparing `xarray_safe_s1-2024.5.16/README.md` & `xarray_safe_s1-2024.5.6/README.md`

 * *Files identical despite different names*

### Comparing `xarray_safe_s1-2024.5.16/ci/requirements/environment.yaml` & `xarray_safe_s1-2024.5.6/ci/requirements/environment.yaml`

 * *Files identical despite different names*

### Comparing `xarray_safe_s1-2024.5.16/docs/Makefile` & `xarray_safe_s1-2024.5.6/docs/Makefile`

 * *Files identical despite different names*

### Comparing `xarray_safe_s1-2024.5.16/docs/conf.py` & `xarray_safe_s1-2024.5.6/docs/conf.py`

 * *Files identical despite different names*

### Comparing `xarray_safe_s1-2024.5.16/docs/examples/simple_tutorial.ipynb` & `xarray_safe_s1-2024.5.6/docs/examples/simple_tutorial.ipynb`

 * *Files identical despite different names*

### Comparing `xarray_safe_s1-2024.5.16/docs/index.rst` & `xarray_safe_s1-2024.5.6/docs/index.rst`

 * *Files identical despite different names*

### Comparing `xarray_safe_s1-2024.5.16/docs/installing.rst` & `xarray_safe_s1-2024.5.6/docs/installing.rst`

 * *Files identical despite different names*

### Comparing `xarray_safe_s1-2024.5.16/docs/make.bat` & `xarray_safe_s1-2024.5.6/docs/make.bat`

 * *Files identical despite different names*

### Comparing `xarray_safe_s1-2024.5.16/highleveltests/open_SLC_IW_S3.py` & `xarray_safe_s1-2024.5.6/highleveltests/open_SLC_IW_S3.py`

 * *Files identical despite different names*

### Comparing `xarray_safe_s1-2024.5.16/pyproject.toml` & `xarray_safe_s1-2024.5.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `xarray_safe_s1-2024.5.16/safe_s1/getconfig.py` & `xarray_safe_s1-2024.5.6/safe_s1/getconfig.py`

 * *Files identical despite different names*

### Comparing `xarray_safe_s1-2024.5.16/safe_s1/reader.py` & `xarray_safe_s1-2024.5.6/safe_s1/reader.py`

 * *Files 1% similar despite different names*

```diff
@@ -108,15 +108,15 @@
                 'antenna_pattern':self.antenna_pattern,
                 'swath_merging': self.swath_merging
             }
             self.dt = datatree.DataTree.from_dict(self._dict)
             assert self.dt==self.datatree
         else:
             print('multidataset')
-            # there is no error raised here, because we want to let the user access the metadata for multidatasets
+            # raise Exception()
 
     def load_digital_number(self, resolution=None, chunks=None, resampling=rasterio.enums.Resampling.rms):
         """
         load digital_number from self.sar_meta.files['measurement'], as an `xarray.Dataset`.
 
         Parameters
         ----------
@@ -642,30 +642,27 @@
         Returns
         -------
         xarray.Dataset
             raw noise range lut
         """
         tmp = []
         pols = []
-        history = []
         for pol_code, xml_file in self.files['noise'].items():
             #pol = self.files['polarization'].cat.categories[pol_code - 1]
             pol = os.path.basename(xml_file).split('-')[4].upper()
             pols.append(pol)
             noise_lut_range_raw_ds = self.xml_parser.get_compound_var(xml_file, 'noise_lut_range_raw')
             for vari in noise_lut_range_raw_ds:
                 if 'noise_lut' in vari:
                     varitmp = 'noiseLut'
                 hihi = self.xml_parser.get_var(self.files['noise'].iloc[0], 'noise.range.%s' % varitmp,
                                                describe=True)
                 noise_lut_range_raw_ds[vari].attrs['description'] = hihi
-                history.append(self.xml_parser.get_compound_var(xml_file, 'noise_lut_range_raw', describe=True))
             tmp.append(noise_lut_range_raw_ds)
         ds = xr.concat(tmp, pd.Index(pols, name="pol"))
-        ds.attrs['history'] = '\n'.join(history)
         return ds
 
     def get_noise_azi_initial_parameters(self, pol):
         """
         Retrieve initial noise lut and lines
 
         Parameters
```

### Comparing `xarray_safe_s1-2024.5.16/safe_s1/sentinel1_xml_mappings.py` & `xarray_safe_s1-2024.5.6/safe_s1/sentinel1_xml_mappings.py`

 * *Files identical despite different names*

### Comparing `xarray_safe_s1-2024.5.16/safe_s1/xml_parser.py` & `xarray_safe_s1-2024.5.6/safe_s1/xml_parser.py`

 * *Files identical despite different names*

### Comparing `xarray_safe_s1-2024.5.16/test/test_s1reader.py` & `xarray_safe_s1-2024.5.6/test/test_s1reader.py`

 * *Files identical despite different names*

### Comparing `xarray_safe_s1-2024.5.16/xarray_safe_s1.egg-info/PKG-INFO` & `xarray_safe_s1-2024.5.6/xarray_safe_s1.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xarray-safe-s1
-Version: 2024.5.16
+Version: 2024.5.6
 License: MIT
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: geopandas
 Requires-Dist: numpy
 Requires-Dist: xarray
```

### Comparing `xarray_safe_s1-2024.5.16/xarray_safe_s1.egg-info/SOURCES.txt` & `xarray_safe_s1-2024.5.6/xarray_safe_s1.egg-info/SOURCES.txt`

 * *Files identical despite different names*

