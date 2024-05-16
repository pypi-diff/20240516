# Comparing `tmp/l2ss_py-2.8.0.tar.gz` & `tmp/l2ss_py-2.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "l2ss_py-2.8.0.tar", max compression
+gzip compressed data, was "l2ss_py-2.9.0.tar", max compression
```

## Comparing `l2ss_py-2.8.0.tar` & `l2ss_py-2.9.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0    11357 2024-01-31 19:31:57.464155 l2ss_py-2.8.0/LICENSE
--rw-r--r--   0        0        0     4830 2024-01-31 19:31:57.468155 l2ss_py-2.8.0/README.md
--rw-r--r--   0        0        0      634 2024-01-31 19:31:57.468155 l2ss_py-2.8.0/podaac/subsetter/__init__.py
--rw-r--r--   0        0        0     6282 2024-01-31 19:31:57.468155 l2ss_py-2.8.0/podaac/subsetter/dimension_cleanup.py
--rw-r--r--   0        0        0     3228 2024-01-31 19:31:57.468155 l2ss_py-2.8.0/podaac/subsetter/gpm_cleanup.py
--rw-r--r--   0        0        0    10368 2024-01-31 19:31:57.468155 l2ss_py-2.8.0/podaac/subsetter/group_handling.py
--rw-r--r--   0        0        0     3118 2024-01-31 19:31:57.468155 l2ss_py-2.8.0/podaac/subsetter/run_subsetter.py
--rw-r--r--   0        0        0    49675 2024-01-31 19:31:57.468155 l2ss_py-2.8.0/podaac/subsetter/subset.py
--rw-r--r--   0        0        0     8667 2024-01-31 19:31:57.468155 l2ss_py-2.8.0/podaac/subsetter/subset_harmony.py
--rw-r--r--   0        0        0     2035 2024-01-31 19:31:57.468155 l2ss_py-2.8.0/podaac/subsetter/time_converting.py
--rw-r--r--   0        0        0    10191 2024-01-31 19:31:57.468155 l2ss_py-2.8.0/podaac/subsetter/xarray_enhancements.py
--rw-r--r--   0        0        0     1950 2024-01-31 19:32:13.868145 l2ss_py-2.8.0/pyproject.toml
--rw-r--r--   0        0        0     6138 1970-01-01 00:00:00.000000 l2ss_py-2.8.0/setup.py
--rw-r--r--   0        0        0     5948 1970-01-01 00:00:00.000000 l2ss_py-2.8.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-03-11 20:01:42.360409 l2ss_py-2.9.0/LICENSE
+-rw-r--r--   0        0        0     4830 2024-03-11 20:01:42.360409 l2ss_py-2.9.0/README.md
+-rw-r--r--   0        0        0      634 2024-03-11 20:01:42.360409 l2ss_py-2.9.0/podaac/subsetter/__init__.py
+-rw-r--r--   0        0        0     6282 2024-03-11 20:01:42.360409 l2ss_py-2.9.0/podaac/subsetter/dimension_cleanup.py
+-rw-r--r--   0        0        0     3228 2024-03-11 20:01:42.360409 l2ss_py-2.9.0/podaac/subsetter/gpm_cleanup.py
+-rw-r--r--   0        0        0    10368 2024-03-11 20:01:42.360409 l2ss_py-2.9.0/podaac/subsetter/group_handling.py
+-rw-r--r--   0        0        0     3118 2024-03-11 20:01:42.360409 l2ss_py-2.9.0/podaac/subsetter/run_subsetter.py
+-rw-r--r--   0        0        0    49675 2024-03-11 20:01:42.360409 l2ss_py-2.9.0/podaac/subsetter/subset.py
+-rw-r--r--   0        0        0     8667 2024-03-11 20:01:42.360409 l2ss_py-2.9.0/podaac/subsetter/subset_harmony.py
+-rw-r--r--   0        0        0     2294 2024-03-11 20:01:42.360409 l2ss_py-2.9.0/podaac/subsetter/time_converting.py
+-rw-r--r--   0        0        0    10732 2024-03-11 20:01:42.360409 l2ss_py-2.9.0/podaac/subsetter/xarray_enhancements.py
+-rw-r--r--   0        0        0     1953 2024-03-11 20:01:57.904482 l2ss_py-2.9.0/pyproject.toml
+-rw-r--r--   0        0        0     6138 1970-01-01 00:00:00.000000 l2ss_py-2.9.0/setup.py
+-rw-r--r--   0        0        0     5948 1970-01-01 00:00:00.000000 l2ss_py-2.9.0/PKG-INFO
```

### Comparing `l2ss_py-2.8.0/LICENSE` & `l2ss_py-2.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `l2ss_py-2.8.0/README.md` & `l2ss_py-2.9.0/README.md`

 * *Files identical despite different names*

### Comparing `l2ss_py-2.8.0/podaac/subsetter/__init__.py` & `l2ss_py-2.9.0/podaac/subsetter/__init__.py`

 * *Files identical despite different names*

### Comparing `l2ss_py-2.8.0/podaac/subsetter/dimension_cleanup.py` & `l2ss_py-2.9.0/podaac/subsetter/dimension_cleanup.py`

 * *Files identical despite different names*

### Comparing `l2ss_py-2.8.0/podaac/subsetter/gpm_cleanup.py` & `l2ss_py-2.9.0/podaac/subsetter/gpm_cleanup.py`

 * *Files identical despite different names*

### Comparing `l2ss_py-2.8.0/podaac/subsetter/group_handling.py` & `l2ss_py-2.9.0/podaac/subsetter/group_handling.py`

 * *Files identical despite different names*

### Comparing `l2ss_py-2.8.0/podaac/subsetter/run_subsetter.py` & `l2ss_py-2.9.0/podaac/subsetter/run_subsetter.py`

 * *Files identical despite different names*

### Comparing `l2ss_py-2.8.0/podaac/subsetter/subset.py` & `l2ss_py-2.9.0/podaac/subsetter/subset.py`

 * *Files identical despite different names*

### Comparing `l2ss_py-2.8.0/podaac/subsetter/subset_harmony.py` & `l2ss_py-2.9.0/podaac/subsetter/subset_harmony.py`

 * *Files identical despite different names*

### Comparing `l2ss_py-2.8.0/podaac/subsetter/time_converting.py` & `l2ss_py-2.9.0/podaac/subsetter/time_converting.py`

 * *Files 8% similar despite different names*

```diff
@@ -41,15 +41,18 @@
     """
     start_date = get_start_date(instrument_type)
 
     for var in time_vars:
         if np.issubdtype(dataset[var].dtype, np.dtype(float)) or np.issubdtype(dataset[var].dtype, np.float32):
             # adjust the time values from the start date
             if start_date:
-                dataset[var].values = [start_date + datetime.timedelta(seconds=i) for i in dataset[var].values]
+                # create array of the start time in datetime format
+                date_time_array = np.full(dataset[var].shape, start_date)
+                # add seconds since the start time to the start time to get the time at the data point
+                dataset[var].values = date_time_array.astype("datetime64[ns]") + dataset[var].astype('timedelta64[s]').values
                 continue
             # if there isn't a start_date, get it from the UTC variable
             utc_var_name = subset.compute_utc_name(dataset)
             if utc_var_name:
                 start_seconds = dataset[var].values[0]
                 dataset[var].values = [datetime.datetime(i[0], i[1], i[2], hour=i[3], minute=i[4], second=i[5]) for i in dataset[utc_var_name].values]
                 start_date = dataset[var].values[0] - np.timedelta64(int(start_seconds), 's')
```

### Comparing `l2ss_py-2.8.0/podaac/subsetter/xarray_enhancements.py` & `l2ss_py-2.9.0/podaac/subsetter/xarray_enhancements.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,18 +64,24 @@
         True if the scanline should be cut.
 
     Returns
     -------
     dict
         Indexer dictionary for the provided condition.
     """
-
-    rows = np.any(cond.values.squeeze(), axis=1)
+    # check if the lat/lon coordinate numpy array has 2 or more dimensions
+    if cond.values.squeeze().ndim == 2:
+        x_axis = 1
+        y_axis = 0
+    else:
+        x_axis = 2
+        y_axis = 1
+    rows = np.any(cond.values.squeeze(), axis=x_axis)
     if cut:
-        cols = np.any(cond.values.squeeze(), axis=0)
+        cols = np.any(cond.values.squeeze(), axis=y_axis)
     else:
         cols = np.ones(len(cond.values[0]))
 
     # If the subsetted area is equal to the original area
     if np.all(rows) & np.all(cols):
         logging.info("Subsetted area equal to the original granule.")
 
@@ -85,18 +91,27 @@
 
     cond_shape_list = list(cond.shape)
     cond_list = list(cond.dims)
     output = [idx for idx, element in enumerate(cond_shape_list) if element == 1]
     for i in output:
         cond_list.pop(i)
 
-    indexers = {
-        cond_list[0]: np.where(rows)[0],
-        cond_list[1]: np.where(cols)[0]
-    }
+    if rows.ndim == 1:
+        indexers = {
+            cond_list[0]: np.where(rows)[0],
+            cond_list[1]: np.where(cols)[0]
+        }
+    else:
+        # if the lat/lon had 3 dimensions the conditional array was identical in the z direction - taking the first
+        rows = rows[0]
+        cols = cols[0]
+        indexers = {
+            cond_list[1]: np.where(rows)[0],
+            cond_list[2]: np.where(cols)[0]
+        }
 
     return indexers
 
 
 def copy_empty_dataset(dataset: xr.Dataset) -> xr.Dataset:
     """
     Copy a dataset into a new, empty dataset. This dataset should:
```

### Comparing `l2ss_py-2.8.0/pyproject.toml` & `l2ss_py-2.9.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 # laws and regulations. User has the responsibility to obtain export
 # licenses, or other export authority as may be required before exporting
 # such information to foreign countries or providing access to foreign
 # persons.
 
 [tool.poetry]
 name = "l2ss-py"
-version = "2.8.0"
+version = "2.9.0"
 description = "L2 Subsetter Service"
 authors = ["podaac-tva <podaac-tva@jpl.nasa.gov>"]
 license = "Apache-2.0"
 readme = "README.md"
 repository = "https://github.com/podaac/l2ss-py"
 classifiers = [
     "Topic :: Software Development :: Libraries :: Python Modules"
@@ -37,21 +37,21 @@
 julian = "^0.14"
 importlib-metadata = "^7.0.1"
 h5py = "^3.6.0"
 cf-xarray = "*"
 numpy = "^1.26.3"
 
 [tool.poetry.dev-dependencies]
-pytest = "~7"
+pytest = "^8.0.2"
 flake8 = "^7.0.0"
 pytest-cov = "~4"
 pylint = "^3.0.2"
 sphinx = "^7.2.6"
 pytest-benchmark = "~4"
-moto = "4.2.13"
+moto = "5.0.2"
 jsonschema = "^4.20.0"
 m2r2 = "^0.3.2"
 sphinx-rtd-theme = "^2.0.0"
 
 [tool.pytest.ini_options]
 junit_family = "xunit2"
```

### Comparing `l2ss_py-2.8.0/setup.py` & `l2ss_py-2.9.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
 entry_points = \
 {'console_scripts': ['l2ss-py = podaac.subsetter.run_subsetter:main',
                      'l2ss_harmony = podaac.subsetter.subset_harmony:main']}
 
 setup_kwargs = {
     'name': 'l2ss-py',
-    'version': '2.8.0',
+    'version': '2.9.0',
     'description': 'L2 Subsetter Service',
     'long_description': '\n# l2ss-py\n\n[![Coverage](https://sonarcloud.io/api/project_badges/measure?project=podaac_l2ss-py&metric=coverage)](https://sonarcloud.io/dashboard?id=podaac_l2ss-py)  \ndevelop: [![Develop Build](https://github.com/podaac/l2ss-py/actions/workflows/build-pipeline.yml/badge.svg?branch=develop&event=push)](https://github.com/podaac/l2ss-py/actions/workflows/build-pipeline.yml)  \nmain: [![Main Build](https://github.com/podaac/l2ss-py/actions/workflows/build-pipeline.yml/badge.svg?branch=main&event=push)](https://github.com/podaac/l2ss-py/actions/workflows/build-pipeline.yml)\n\nHarmony service for subsetting L2 data. l2ss-py supports:\n\n- Spatial subsetting\n    - Bounding box\n    - Shapefile subsetting\n    - GeoJSON subsetting\n- Temporal subsetting\n- Variable subsetting\n\nIf you would like to contribute to l2ss-py, refer to the [contribution document](CONTRIBUTING.md).\n\n## Initial setup, with poetry\n\n1. Follow the instructions for installing `poetry` [here](https://python-poetry.org/docs/).\n2. Install l2ss-py, with its dependencies, by running the following from the repository directory:\n\n```\npoetry install\n```\n\n***Note:*** l2ss-py can be installed as above and run without any dependency on `harmony`. \nHowever, to additionally test the harmony adapter layer, \nextra dependencies can be installed with `poetry install -E harmony`.\n\n## How to test l2ss-py locally\n\n### Unit tests\n\nThere are comprehensive unit tests for l2ss-py. The tests can be run as follows:\n\n```\npoetry run pytest -m "not aws and not integration" tests/\n```\n\nYou can generate coverage reports as follows:\n\n```\npoetry run pytest --junitxml=build/reports/pytest.xml --cov=podaac/ --cov-report=html -m "not aws and not integration" tests/\n```\n\n***Note:*** The majority of the tests execute core functionality of l2ss-py without ever interacting with the harmony python modules. \nThe `test_subset_harmony` tests, however, are explicitly for testing the harmony adapter layer \nand do require the harmony optional dependencies be installed, \nas described above with the `-E harmony` argument.\n\n### l2ss-py script\n\nYou can run l2ss-py on a single granule without using Harmony. In order \nto run this, the l2ss-py package must be installed in your current \nPython interpreter\n\n```\n$ l2ss-py --help                                                                                                                    \nusage: run_subsetter.py [-h] [--bbox BBOX BBOX BBOX BBOX]\n                        [--variables VARIABLES [VARIABLES ...]]\n                        [--min-time MIN_TIME] [--max-time MAX_TIME] [--cut]\n                        input_file output_file\n\nRun l2ss-py\n\npositional arguments:\n  input_file            File to subset\n  output_file           Output file\n\noptional arguments:\n  -h, --help            show this help message and exit\n  --bbox BBOX BBOX BBOX BBOX\n                        Bounding box in the form min_lon min_lat max_lon\n                        max_lat\n  --variables VARIABLES [VARIABLES ...]\n                        Variables, only include if variable subset is desired.\n                        Should be a space separated list of variable names\n                        e.g. sst wind_dir sst_error ...\n  --min-time MIN_TIME   Min time. Should be ISO-8601 format. Only include if\n                        temporal subset is desired.\n  --max-time MAX_TIME   Max time. Should be ISO-8601 format. Only include if\n                        temporal subset is desired.\n  --cut                 If provided, scanline will be cut\n  --shapefile SHAPEFILE\n                        Path to either shapefile or geojson file used to subset the provided input granule\n```\n\nFor example:\n\n```\nl2ss-py /path/to/input.nc /path/to/output.nc --bbox -50 -10 50 10 --variables wind_speed wind_dir ice_age time --min-time \'2015-07-02T09:00:00\' --max-time \'2015-07-02T10:00:00\' --cut\n```\n\nAn addition to providing a bounding box, spatial subsetting can be achieved by passing in a shapefile or a geojson file. \n\n```shell script\npoetry run l2ss-py /path/to/input.nc /path/to/output.nc --shapefile /path/to/test.shp\n```\n\nor \n\n```shell script\npoetry run l2ss-py /path/to/input.nc /path/to/output.nc --shapefile /path/to/test.geojson\n```\n\n### Running Harmony locally\n\nIn order to fully test l2ss-py with Harmony, you can run Harmony locally. This requires the data exists in UAT Earthdata Cloud.\n\n1. Set up local Harmony instance. Instructions [here](https://github.com/nasa/harmony#Quick-Start)\n2. Add concept ID for your data to [services.yml](https://github.com/nasa/harmony/blob/main/config/services.yml)\n3. Execute a local Harmony l2ss-py request. For example:\n    ```\n   localhost:3000/YOUR_COLLECTION_ID/ogc-api-coverages/1.0.0/collections/all/coverage/rangeset?format=application%2Fx-netcdf4&subset=lat(-10%3A10)&subset=lon(-10%3A10)&maxResults=2\n   ```\n',
     'author': 'podaac-tva',
     'author_email': 'podaac-tva@jpl.nasa.gov',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/podaac/l2ss-py',
```

### Comparing `l2ss_py-2.8.0/PKG-INFO` & `l2ss_py-2.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: l2ss-py
-Version: 2.8.0
+Version: 2.9.0
 Summary: L2 Subsetter Service
 Home-page: https://github.com/podaac/l2ss-py
 License: Apache-2.0
 Author: podaac-tva
 Author-email: podaac-tva@jpl.nasa.gov
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
```

