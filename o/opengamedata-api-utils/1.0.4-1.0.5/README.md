# Comparing `tmp/opengamedata_api_utils-1.0.4.tar.gz` & `tmp/opengamedata_api_utils-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opengamedata_api_utils-1.0.4.tar", last modified: Wed May 15 21:35:51 2024, max compression
+gzip compressed data, was "opengamedata_api_utils-1.0.5.tar", last modified: Wed May 15 22:00:45 2024, max compression
```

## Comparing `opengamedata_api_utils-1.0.4.tar` & `opengamedata_api_utils-1.0.5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:35:51.473625 opengamedata_api_utils-1.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-15 21:35:38.000000 opengamedata_api_utils-1.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2264 2024-05-15 21:35:51.473625 opengamedata_api_utils-1.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-05-15 21:35:38.000000 opengamedata_api_utils-1.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      852 2024-05-15 21:35:38.000000 opengamedata_api_utils-1.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 21:35:51.473625 opengamedata_api_utils-1.0.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:35:51.469625 opengamedata_api_utils-1.0.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:35:51.469625 opengamedata_api_utils-1.0.4/src/ogd/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:35:51.469625 opengamedata_api_utils-1.0.4/src/ogd/apis/
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-15 21:35:38.000000 opengamedata_api_utils-1.0.4/src/ogd/apis/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:35:51.469625 opengamedata_api_utils-1.0.4/src/ogd/apis/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)     3197 2024-05-15 21:35:38.000000 opengamedata_api_utils-1.0.4/src/ogd/apis/schemas/ServerConfigSchema.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 21:35:38.000000 opengamedata_api_utils-1.0.4/src/ogd/apis/schemas/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:35:51.469625 opengamedata_api_utils-1.0.4/src/ogd/apis/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     4649 2024-05-15 21:35:38.000000 opengamedata_api_utils-1.0.4/src/ogd/apis/utils/APIResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)     3846 2024-05-15 21:35:38.000000 opengamedata_api_utils-1.0.4/src/ogd/apis/utils/APIUtils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2888 2024-05-15 21:35:38.000000 opengamedata_api_utils-1.0.4/src/ogd/apis/utils/HelloAPI.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 21:35:38.000000 opengamedata_api_utils-1.0.4/src/ogd/apis/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:35:51.473625 opengamedata_api_utils-1.0.4/src/opengamedata_api_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2264 2024-05-15 21:35:51.000000 opengamedata_api_utils-1.0.4/src/opengamedata_api_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      460 2024-05-15 21:35:51.000000 opengamedata_api_utils-1.0.4/src/opengamedata_api_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 21:35:51.000000 opengamedata_api_utils-1.0.4/src/opengamedata_api_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-15 21:35:51.000000 opengamedata_api_utils-1.0.4/src/opengamedata_api_utils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 22:00:45.986562 opengamedata_api_utils-1.0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-15 22:00:34.000000 opengamedata_api_utils-1.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2264 2024-05-15 22:00:45.986562 opengamedata_api_utils-1.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-05-15 22:00:34.000000 opengamedata_api_utils-1.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      852 2024-05-15 22:00:34.000000 opengamedata_api_utils-1.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 22:00:45.986562 opengamedata_api_utils-1.0.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 22:00:45.982562 opengamedata_api_utils-1.0.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 22:00:45.982562 opengamedata_api_utils-1.0.5/src/ogd/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 22:00:45.982562 opengamedata_api_utils-1.0.5/src/ogd/apis/
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-15 22:00:34.000000 opengamedata_api_utils-1.0.5/src/ogd/apis/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 22:00:45.986562 opengamedata_api_utils-1.0.5/src/ogd/apis/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)     3197 2024-05-15 22:00:34.000000 opengamedata_api_utils-1.0.5/src/ogd/apis/schemas/ServerConfigSchema.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 22:00:34.000000 opengamedata_api_utils-1.0.5/src/ogd/apis/schemas/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 22:00:45.986562 opengamedata_api_utils-1.0.5/src/ogd/apis/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     4649 2024-05-15 22:00:34.000000 opengamedata_api_utils-1.0.5/src/ogd/apis/utils/APIResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3846 2024-05-15 22:00:34.000000 opengamedata_api_utils-1.0.5/src/ogd/apis/utils/APIUtils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2890 2024-05-15 22:00:34.000000 opengamedata_api_utils-1.0.5/src/ogd/apis/utils/HelloAPI.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 22:00:34.000000 opengamedata_api_utils-1.0.5/src/ogd/apis/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 22:00:45.986562 opengamedata_api_utils-1.0.5/src/opengamedata_api_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2264 2024-05-15 22:00:45.000000 opengamedata_api_utils-1.0.5/src/opengamedata_api_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2024-05-15 22:00:45.000000 opengamedata_api_utils-1.0.5/src/opengamedata_api_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 22:00:45.000000 opengamedata_api_utils-1.0.5/src/opengamedata_api_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-15 22:00:45.000000 opengamedata_api_utils-1.0.5/src/opengamedata_api_utils.egg-info/top_level.txt
```

### Comparing `opengamedata_api_utils-1.0.4/LICENSE` & `opengamedata_api_utils-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `opengamedata_api_utils-1.0.4/PKG-INFO` & `opengamedata_api_utils-1.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opengamedata-api-utils
-Version: 1.0.4
+Version: 1.0.5
 Summary: Package of utilities for server-side scripts in OpenGameData.
 Author: Ryan Wilkinson, Glenn Palmer, Daus Husaini
 Author-email: Luke Swanson <superscription58@gmail.com>
 Project-URL: Homepage, https://github.com/opengamedata/opengamedata-api-utils
 Project-URL: Bug Tracker, https://github.com/opengamedata/opengamedata-api-utils/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `opengamedata_api_utils-1.0.4/README.md` & `opengamedata_api_utils-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `opengamedata_api_utils-1.0.4/pyproject.toml` & `opengamedata_api_utils-1.0.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `opengamedata_api_utils-1.0.4/src/ogd/apis/schemas/ServerConfigSchema.py` & `opengamedata_api_utils-1.0.5/src/ogd/apis/schemas/ServerConfigSchema.py`

 * *Files identical despite different names*

### Comparing `opengamedata_api_utils-1.0.4/src/ogd/apis/utils/APIResponse.py` & `opengamedata_api_utils-1.0.5/src/ogd/apis/utils/APIResponse.py`

 * *Files identical despite different names*

### Comparing `opengamedata_api_utils-1.0.4/src/ogd/apis/utils/APIUtils.py` & `opengamedata_api_utils-1.0.5/src/ogd/apis/utils/APIUtils.py`

 * *Files identical despite different names*

### Comparing `opengamedata_api_utils-1.0.4/src/ogd/apis/utils/HelloAPI.py` & `opengamedata_api_utils-1.0.5/src/ogd/apis/utils/HelloAPI.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 class HelloAPI:
     @staticmethod
     def register(app:Flask, server_config:ServerConfigSchema):
         api = Api(app)
         api.add_resource(HelloAPI.Hello, '/hello')
         api.add_resource(HelloAPI.ParamHello, '/p_hello/<name>')
-        api.add_resource(HelloAPI.Hello, '/version')
+        api.add_resource(HelloAPI.Version, '/version')
 
         HelloAPI.server_config = server_config
 
     class Hello(Resource):
         def get(self):
             ret_val = APIResponse(
                 req_type = RESTType.GET,
```

### Comparing `opengamedata_api_utils-1.0.4/src/opengamedata_api_utils.egg-info/PKG-INFO` & `opengamedata_api_utils-1.0.5/src/opengamedata_api_utils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opengamedata-api-utils
-Version: 1.0.4
+Version: 1.0.5
 Summary: Package of utilities for server-side scripts in OpenGameData.
 Author: Ryan Wilkinson, Glenn Palmer, Daus Husaini
 Author-email: Luke Swanson <superscription58@gmail.com>
 Project-URL: Homepage, https://github.com/opengamedata/opengamedata-api-utils
 Project-URL: Bug Tracker, https://github.com/opengamedata/opengamedata-api-utils/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

