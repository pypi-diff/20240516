# Comparing `tmp/hsclient-1.0.0.tar.gz` & `tmp/hsclient-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hsclient-1.0.0.tar", last modified: Mon Feb 19 20:03:41 2024, max compression
+gzip compressed data, was "hsclient-1.0.1.tar", last modified: Thu May 16 15:11:04 2024, max compression
```

## Comparing `hsclient-1.0.0.tar` & `hsclient-1.0.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 20:03:41.099192 hsclient-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1499 2024-02-19 20:03:33.000000 hsclient-1.0.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4685 2024-02-19 20:03:41.099192 hsclient-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3518 2024-02-19 20:03:33.000000 hsclient-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 20:03:41.099192 hsclient-1.0.0/hsclient/
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-02-19 20:03:33.000000 hsclient-1.0.0/hsclient/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    67150 2024-02-19 20:03:33.000000 hsclient-1.0.0/hsclient/hydroshare.py
--rw-r--r--   0 runner    (1001) docker     (127)     1618 2024-02-19 20:03:33.000000 hsclient-1.0.0/hsclient/json_models.py
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-02-19 20:03:33.000000 hsclient-1.0.0/hsclient/oauth2_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1881 2024-02-19 20:03:33.000000 hsclient-1.0.0/hsclient/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 20:03:41.099192 hsclient-1.0.0/hsclient.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4685 2024-02-19 20:03:41.000000 hsclient-1.0.0/hsclient.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      388 2024-02-19 20:03:41.000000 hsclient-1.0.0/hsclient.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-19 20:03:41.000000 hsclient-1.0.0/hsclient.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-02-19 20:03:41.000000 hsclient-1.0.0/hsclient.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-02-19 20:03:41.000000 hsclient-1.0.0/hsclient.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      908 2024-02-19 20:03:41.103191 hsclient-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-02-19 20:03:33.000000 hsclient-1.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 20:03:41.099192 hsclient-1.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    14519 2024-02-19 20:03:33.000000 hsclient-1.0.0/tests/test_data_objects.py
--rw-r--r--   0 runner    (1001) docker     (127)    22744 2024-02-19 20:03:33.000000 hsclient-1.0.0/tests/test_functional.py
--rw-r--r--   0 runner    (1001) docker     (127)     3593 2024-02-19 20:03:33.000000 hsclient-1.0.0/tests/test_json_models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 15:11:04.536164 hsclient-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1499 2024-05-16 15:11:01.000000 hsclient-1.0.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4685 2024-05-16 15:11:04.536164 hsclient-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3518 2024-05-16 15:11:01.000000 hsclient-1.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 15:11:04.536164 hsclient-1.0.1/hsclient/
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-16 15:11:01.000000 hsclient-1.0.1/hsclient/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    67150 2024-05-16 15:11:01.000000 hsclient-1.0.1/hsclient/hydroshare.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1709 2024-05-16 15:11:01.000000 hsclient-1.0.1/hsclient/json_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-05-16 15:11:01.000000 hsclient-1.0.1/hsclient/oauth2_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1881 2024-05-16 15:11:01.000000 hsclient-1.0.1/hsclient/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 15:11:04.536164 hsclient-1.0.1/hsclient.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4685 2024-05-16 15:11:04.000000 hsclient-1.0.1/hsclient.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-05-16 15:11:04.000000 hsclient-1.0.1/hsclient.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 15:11:04.000000 hsclient-1.0.1/hsclient.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-05-16 15:11:04.000000 hsclient-1.0.1/hsclient.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-16 15:11:04.000000 hsclient-1.0.1/hsclient.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      908 2024-05-16 15:11:04.536164 hsclient-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-05-16 15:11:01.000000 hsclient-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 15:11:04.536164 hsclient-1.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    14519 2024-05-16 15:11:01.000000 hsclient-1.0.1/tests/test_data_objects.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22744 2024-05-16 15:11:01.000000 hsclient-1.0.1/tests/test_functional.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3593 2024-05-16 15:11:01.000000 hsclient-1.0.1/tests/test_json_models.py
```

### Comparing `hsclient-1.0.0/LICENSE.txt` & `hsclient-1.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `hsclient-1.0.0/PKG-INFO` & `hsclient-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: hsclient
-Version: 1.0.0
+Version: 1.0.1
 Summary: A python client for managing HydroShare resources
 Home-page: https://github.com/hydroshare/hsclient
 Author: Scott Black
 Author-email: scott.black@usu.edu
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
-Requires-Dist: hsmodels>=1.0.0
+Requires-Dist: hsmodels>=1.0.3
 Requires-Dist: requests
 Requires-Dist: requests_oauthlib
 Provides-Extra: pandas
 Requires-Dist: pandas; extra == "pandas"
 Provides-Extra: xarray
 Requires-Dist: netCDF4; extra == "xarray"
 Requires-Dist: xarray; extra == "xarray"
```

### Comparing `hsclient-1.0.0/README.md` & `hsclient-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `hsclient-1.0.0/hsclient/hydroshare.py` & `hsclient-1.0.1/hsclient/hydroshare.py`

 * *Files identical despite different names*

### Comparing `hsclient-1.0.0/hsclient/json_models.py` & `hsclient-1.0.1/hsclient/json_models.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,15 +16,19 @@
     identifiers: Dict[UserIdentifierType, AnyUrl] = {}
     type: str = None
     subject_areas: List[str] = []
     date_joined: datetime = None
 
     @field_validator("subject_areas", mode='before')
     def split_subject_areas(cls, value):
-        return value.split(", ") if value else []
+        if isinstance(value, str):
+            return value.split(", ")
+        if value is None:
+            return []
+        return value
 
 
 class ResourcePreview(BaseModel):
     resource_type: str = None
     resource_title: str = None
     resource_id: str = None
     abstract: str = None
```

### Comparing `hsclient-1.0.0/hsclient/utils.py` & `hsclient-1.0.1/hsclient/utils.py`

 * *Files identical despite different names*

### Comparing `hsclient-1.0.0/hsclient.egg-info/PKG-INFO` & `hsclient-1.0.1/hsclient.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: hsclient
-Version: 1.0.0
+Version: 1.0.1
 Summary: A python client for managing HydroShare resources
 Home-page: https://github.com/hydroshare/hsclient
 Author: Scott Black
 Author-email: scott.black@usu.edu
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
-Requires-Dist: hsmodels>=1.0.0
+Requires-Dist: hsmodels>=1.0.3
 Requires-Dist: requests
 Requires-Dist: requests_oauthlib
 Provides-Extra: pandas
 Requires-Dist: pandas; extra == "pandas"
 Provides-Extra: xarray
 Requires-Dist: netCDF4; extra == "xarray"
 Requires-Dist: xarray; extra == "xarray"
```

### Comparing `hsclient-1.0.0/setup.cfg` & `hsclient-1.0.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `hsclient-1.0.0/setup.py` & `hsclient-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import pathlib
 from setuptools import setup, find_packages
 
 README = (pathlib.Path(__file__).parent / "README.md").read_text()
 
 setup(
     name='hsclient',
-    version='1.0.0',
+    version='1.0.1',
     packages=find_packages(include=['hsclient', 'hsclient.*'],
                            exclude=("tests",)),
     install_requires=[
-        'hsmodels>=1.0.0',
+        'hsmodels>=1.0.3',
         'requests',
         'requests_oauthlib',
     ],
     extras_require={
         "pandas": ["pandas"],
         "xarray": ["netCDF4", "xarray"],
         "rasterio": ["rasterio"],
```

### Comparing `hsclient-1.0.0/tests/test_data_objects.py` & `hsclient-1.0.1/tests/test_data_objects.py`

 * *Files identical despite different names*

### Comparing `hsclient-1.0.0/tests/test_functional.py` & `hsclient-1.0.1/tests/test_functional.py`

 * *Files identical despite different names*

### Comparing `hsclient-1.0.0/tests/test_json_models.py` & `hsclient-1.0.1/tests/test_json_models.py`

 * *Files identical despite different names*

