# Comparing `tmp/opengamedata_api_utils-1.0.6.tar.gz` & `tmp/opengamedata_api_utils-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opengamedata_api_utils-1.0.6.tar", last modified: Wed May 15 22:36:13 2024, max compression
+gzip compressed data, was "opengamedata_api_utils-1.0.7.tar", last modified: Thu May 16 03:58:45 2024, max compression
```

## Comparing `opengamedata_api_utils-1.0.6.tar` & `opengamedata_api_utils-1.0.7.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 22:36:13.300227 opengamedata_api_utils-1.0.6/
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-15 22:35:55.000000 opengamedata_api_utils-1.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2264 2024-05-15 22:36:13.300227 opengamedata_api_utils-1.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-05-15 22:35:55.000000 opengamedata_api_utils-1.0.6/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      852 2024-05-15 22:35:55.000000 opengamedata_api_utils-1.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 22:36:13.300227 opengamedata_api_utils-1.0.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 22:36:13.296227 opengamedata_api_utils-1.0.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 22:36:13.296227 opengamedata_api_utils-1.0.6/src/ogd/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 22:36:13.300227 opengamedata_api_utils-1.0.6/src/ogd/apis/
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-15 22:35:55.000000 opengamedata_api_utils-1.0.6/src/ogd/apis/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 22:36:13.300227 opengamedata_api_utils-1.0.6/src/ogd/apis/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)     3197 2024-05-15 22:35:55.000000 opengamedata_api_utils-1.0.6/src/ogd/apis/schemas/ServerConfigSchema.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 22:35:55.000000 opengamedata_api_utils-1.0.6/src/ogd/apis/schemas/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 22:36:13.300227 opengamedata_api_utils-1.0.6/src/ogd/apis/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     4649 2024-05-15 22:35:55.000000 opengamedata_api_utils-1.0.6/src/ogd/apis/utils/APIResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)     3846 2024-05-15 22:35:55.000000 opengamedata_api_utils-1.0.6/src/ogd/apis/utils/APIUtils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2895 2024-05-15 22:35:55.000000 opengamedata_api_utils-1.0.6/src/ogd/apis/utils/HelloAPI.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 22:35:55.000000 opengamedata_api_utils-1.0.6/src/ogd/apis/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 22:36:13.300227 opengamedata_api_utils-1.0.6/src/opengamedata_api_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2264 2024-05-15 22:36:13.000000 opengamedata_api_utils-1.0.6/src/opengamedata_api_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      460 2024-05-15 22:36:13.000000 opengamedata_api_utils-1.0.6/src/opengamedata_api_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 22:36:13.000000 opengamedata_api_utils-1.0.6/src/opengamedata_api_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-15 22:36:13.000000 opengamedata_api_utils-1.0.6/src/opengamedata_api_utils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 03:58:45.901426 opengamedata_api_utils-1.0.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-16 03:58:34.000000 opengamedata_api_utils-1.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2264 2024-05-16 03:58:45.901426 opengamedata_api_utils-1.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-05-16 03:58:34.000000 opengamedata_api_utils-1.0.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      852 2024-05-16 03:58:34.000000 opengamedata_api_utils-1.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 03:58:45.901426 opengamedata_api_utils-1.0.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 03:58:45.901426 opengamedata_api_utils-1.0.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 03:58:45.897426 opengamedata_api_utils-1.0.7/src/ogd/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 03:58:45.901426 opengamedata_api_utils-1.0.7/src/ogd/apis/
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-16 03:58:34.000000 opengamedata_api_utils-1.0.7/src/ogd/apis/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 03:58:45.901426 opengamedata_api_utils-1.0.7/src/ogd/apis/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)     3225 2024-05-16 03:58:34.000000 opengamedata_api_utils-1.0.7/src/ogd/apis/schemas/ServerConfigSchema.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 03:58:34.000000 opengamedata_api_utils-1.0.7/src/ogd/apis/schemas/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 03:58:45.901426 opengamedata_api_utils-1.0.7/src/ogd/apis/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     4649 2024-05-16 03:58:34.000000 opengamedata_api_utils-1.0.7/src/ogd/apis/utils/APIResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3846 2024-05-16 03:58:34.000000 opengamedata_api_utils-1.0.7/src/ogd/apis/utils/APIUtils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2902 2024-05-16 03:58:34.000000 opengamedata_api_utils-1.0.7/src/ogd/apis/utils/HelloAPI.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 03:58:34.000000 opengamedata_api_utils-1.0.7/src/ogd/apis/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 03:58:45.901426 opengamedata_api_utils-1.0.7/src/opengamedata_api_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2264 2024-05-16 03:58:45.000000 opengamedata_api_utils-1.0.7/src/opengamedata_api_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2024-05-16 03:58:45.000000 opengamedata_api_utils-1.0.7/src/opengamedata_api_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 03:58:45.000000 opengamedata_api_utils-1.0.7/src/opengamedata_api_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-16 03:58:45.000000 opengamedata_api_utils-1.0.7/src/opengamedata_api_utils.egg-info/top_level.txt
```

### Comparing `opengamedata_api_utils-1.0.6/LICENSE` & `opengamedata_api_utils-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `opengamedata_api_utils-1.0.6/PKG-INFO` & `opengamedata_api_utils-1.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opengamedata-api-utils
-Version: 1.0.6
+Version: 1.0.7
 Summary: Package of utilities for server-side scripts in OpenGameData.
 Author: Ryan Wilkinson, Glenn Palmer, Daus Husaini
 Author-email: Luke Swanson <superscription58@gmail.com>
 Project-URL: Homepage, https://github.com/opengamedata/opengamedata-api-utils
 Project-URL: Bug Tracker, https://github.com/opengamedata/opengamedata-api-utils/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `opengamedata_api_utils-1.0.6/README.md` & `opengamedata_api_utils-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `opengamedata_api_utils-1.0.6/pyproject.toml` & `opengamedata_api_utils-1.0.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `opengamedata_api_utils-1.0.6/src/ogd/apis/schemas/ServerConfigSchema.py` & `opengamedata_api_utils-1.0.7/src/ogd/apis/schemas/ServerConfigSchema.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,15 @@
             self._dbg_level = ServerConfigSchema._parseDebugLevel(all_elements["DEBUG_LEVEL"], logger=logger)
         else:
             self._dbg_level = logging.INFO
             logger.warn(f"{name} config does not have a 'DEBUG_LEVEL' element; defaulting to dbg_level={self._dbg_level}", logging.WARN)
         if "VER" in all_elements.keys():
             self._version = ServerConfigSchema._parseVersion(all_elements["VER"], logger=logger)
         else:
-            self._version = "UNKNOWN VERSION"
+            self._version = SemanticVersion.FromString("UNKNOWN VERSION")
             logger.warn(f"{name} config does not have a 'VER' element; defaulting to version={self._version}", logging.WARN)
 
         _used = {"DB_CONFIG", "OGD_CORE_PATH", "GOOGLE_CLIENT_ID", "DEBUG_LEVEL", "VER"}
         _leftovers = { key : val for key,val in all_elements.items() if key not in _used }
         super().__init__(name=name, other_elements=_leftovers)
 
     @property
```

### Comparing `opengamedata_api_utils-1.0.6/src/ogd/apis/utils/APIResponse.py` & `opengamedata_api_utils-1.0.7/src/ogd/apis/utils/APIResponse.py`

 * *Files identical despite different names*

### Comparing `opengamedata_api_utils-1.0.6/src/ogd/apis/utils/APIUtils.py` & `opengamedata_api_utils-1.0.7/src/ogd/apis/utils/APIUtils.py`

 * *Files identical despite different names*

### Comparing `opengamedata_api_utils-1.0.6/src/ogd/apis/utils/HelloAPI.py` & `opengamedata_api_utils-1.0.7/src/ogd/apis/utils/HelloAPI.py`

 * *Files 4% similar despite different names*

```diff
@@ -76,11 +76,11 @@
                 status   = ResponseStatus.SUCCESS)
             return ret_val.AsDict
     
     class Version(Resource):
         def get(self):
             ret_val = APIResponse(
                 req_type = RESTType.GET,
-                val      = str(HelloAPI.server_config.Version),
+                val      = {"version":HelloAPI.server_config.Version},
                 msg      = f"Successfully retrieved API version.",
                 status   = ResponseStatus.SUCCESS)
             return ret_val.AsDict
```

### Comparing `opengamedata_api_utils-1.0.6/src/opengamedata_api_utils.egg-info/PKG-INFO` & `opengamedata_api_utils-1.0.7/src/opengamedata_api_utils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opengamedata-api-utils
-Version: 1.0.6
+Version: 1.0.7
 Summary: Package of utilities for server-side scripts in OpenGameData.
 Author: Ryan Wilkinson, Glenn Palmer, Daus Husaini
 Author-email: Luke Swanson <superscription58@gmail.com>
 Project-URL: Homepage, https://github.com/opengamedata/opengamedata-api-utils
 Project-URL: Bug Tracker, https://github.com/opengamedata/opengamedata-api-utils/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

