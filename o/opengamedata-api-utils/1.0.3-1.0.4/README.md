# Comparing `tmp/opengamedata_api_utils-1.0.3.tar.gz` & `tmp/opengamedata_api_utils-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opengamedata_api_utils-1.0.3.tar", last modified: Wed May 15 00:13:03 2024, max compression
+gzip compressed data, was "opengamedata_api_utils-1.0.4.tar", last modified: Wed May 15 21:35:51 2024, max compression
```

## Comparing `opengamedata_api_utils-1.0.3.tar` & `opengamedata_api_utils-1.0.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 00:13:03.746476 opengamedata_api_utils-1.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-15 00:12:48.000000 opengamedata_api_utils-1.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2264 2024-05-15 00:13:03.746476 opengamedata_api_utils-1.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-05-15 00:12:48.000000 opengamedata_api_utils-1.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      852 2024-05-15 00:12:48.000000 opengamedata_api_utils-1.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 00:13:03.746476 opengamedata_api_utils-1.0.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 00:13:03.742476 opengamedata_api_utils-1.0.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 00:13:03.742476 opengamedata_api_utils-1.0.3/src/ogd/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 00:13:03.742476 opengamedata_api_utils-1.0.3/src/ogd/apis/
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-15 00:12:48.000000 opengamedata_api_utils-1.0.3/src/ogd/apis/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 00:13:03.742476 opengamedata_api_utils-1.0.3/src/ogd/apis/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)     3006 2024-05-15 00:12:48.000000 opengamedata_api_utils-1.0.3/src/ogd/apis/schemas/ServerConfigSchema.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 00:12:48.000000 opengamedata_api_utils-1.0.3/src/ogd/apis/schemas/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 00:13:03.746476 opengamedata_api_utils-1.0.3/src/ogd/apis/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     4649 2024-05-15 00:12:48.000000 opengamedata_api_utils-1.0.3/src/ogd/apis/utils/APIResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)     3846 2024-05-15 00:12:48.000000 opengamedata_api_utils-1.0.3/src/ogd/apis/utils/APIUtils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2888 2024-05-15 00:12:48.000000 opengamedata_api_utils-1.0.3/src/ogd/apis/utils/HelloAPI.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 00:12:48.000000 opengamedata_api_utils-1.0.3/src/ogd/apis/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 00:13:03.746476 opengamedata_api_utils-1.0.3/src/opengamedata_api_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2264 2024-05-15 00:13:03.000000 opengamedata_api_utils-1.0.3/src/opengamedata_api_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      460 2024-05-15 00:13:03.000000 opengamedata_api_utils-1.0.3/src/opengamedata_api_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 00:13:03.000000 opengamedata_api_utils-1.0.3/src/opengamedata_api_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-15 00:13:03.000000 opengamedata_api_utils-1.0.3/src/opengamedata_api_utils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:35:51.473625 opengamedata_api_utils-1.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-15 21:35:38.000000 opengamedata_api_utils-1.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2264 2024-05-15 21:35:51.473625 opengamedata_api_utils-1.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-05-15 21:35:38.000000 opengamedata_api_utils-1.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      852 2024-05-15 21:35:38.000000 opengamedata_api_utils-1.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 21:35:51.473625 opengamedata_api_utils-1.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:35:51.469625 opengamedata_api_utils-1.0.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:35:51.469625 opengamedata_api_utils-1.0.4/src/ogd/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:35:51.469625 opengamedata_api_utils-1.0.4/src/ogd/apis/
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-15 21:35:38.000000 opengamedata_api_utils-1.0.4/src/ogd/apis/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:35:51.469625 opengamedata_api_utils-1.0.4/src/ogd/apis/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)     3197 2024-05-15 21:35:38.000000 opengamedata_api_utils-1.0.4/src/ogd/apis/schemas/ServerConfigSchema.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 21:35:38.000000 opengamedata_api_utils-1.0.4/src/ogd/apis/schemas/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:35:51.469625 opengamedata_api_utils-1.0.4/src/ogd/apis/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     4649 2024-05-15 21:35:38.000000 opengamedata_api_utils-1.0.4/src/ogd/apis/utils/APIResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3846 2024-05-15 21:35:38.000000 opengamedata_api_utils-1.0.4/src/ogd/apis/utils/APIUtils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2888 2024-05-15 21:35:38.000000 opengamedata_api_utils-1.0.4/src/ogd/apis/utils/HelloAPI.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 21:35:38.000000 opengamedata_api_utils-1.0.4/src/ogd/apis/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:35:51.473625 opengamedata_api_utils-1.0.4/src/opengamedata_api_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2264 2024-05-15 21:35:51.000000 opengamedata_api_utils-1.0.4/src/opengamedata_api_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2024-05-15 21:35:51.000000 opengamedata_api_utils-1.0.4/src/opengamedata_api_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 21:35:51.000000 opengamedata_api_utils-1.0.4/src/opengamedata_api_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-15 21:35:51.000000 opengamedata_api_utils-1.0.4/src/opengamedata_api_utils.egg-info/top_level.txt
```

### Comparing `opengamedata_api_utils-1.0.3/LICENSE` & `opengamedata_api_utils-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `opengamedata_api_utils-1.0.3/PKG-INFO` & `opengamedata_api_utils-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opengamedata-api-utils
-Version: 1.0.3
+Version: 1.0.4
 Summary: Package of utilities for server-side scripts in OpenGameData.
 Author: Ryan Wilkinson, Glenn Palmer, Daus Husaini
 Author-email: Luke Swanson <superscription58@gmail.com>
 Project-URL: Homepage, https://github.com/opengamedata/opengamedata-api-utils
 Project-URL: Bug Tracker, https://github.com/opengamedata/opengamedata-api-utils/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `opengamedata_api_utils-1.0.3/README.md` & `opengamedata_api_utils-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `opengamedata_api_utils-1.0.3/pyproject.toml` & `opengamedata_api_utils-1.0.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `opengamedata_api_utils-1.0.3/src/ogd/apis/schemas/ServerConfigSchema.py` & `opengamedata_api_utils-1.0.4/src/ogd/apis/schemas/ServerConfigSchema.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,21 +8,22 @@
 import logging
 from typing import Any, Dict
 
 # import 3rd-party libraries
 
 # import OGD libraries
 from ogd.core.schemas.Schema import Schema
+from ogd.core.utils.SemanticVersion import SemanticVersion
 
 # import local files
 
 class ServerConfigSchema(Schema):
     def __init__(self, name:str, all_elements:Dict[str, Any], logger:logging.Logger):
-        self._dbg_level        : int
-        self._version          : str
+        self._dbg_level : int
+        self._version   : SemanticVersion
 
         if "DEBUG_LEVEL" in all_elements.keys():
             self._dbg_level = ServerConfigSchema._parseDebugLevel(all_elements["DEBUG_LEVEL"], logger=logger)
         else:
             self._dbg_level = logging.INFO
             logger.warn(f"{name} config does not have a 'DEBUG_LEVEL' element; defaulting to dbg_level={self._dbg_level}", logging.WARN)
         if "VER" in all_elements.keys():
@@ -36,15 +37,15 @@
         super().__init__(name=name, other_elements=_leftovers)
 
     @property
     def DebugLevel(self) -> int:
         return self._dbg_level
 
     @property
-    def Version(self) -> str:
+    def Version(self) -> SemanticVersion:
         return self._version
 
     @property
     def AsMarkdown(self) -> str:
         ret_val : str
 
         ret_val = f"{self.Name}"
@@ -68,17 +69,17 @@
                     logger.warn(f"Config debug level had unexpected value {level}, defaulting to logging.INFO.", logging.WARN)
         else:
             ret_val = logging.INFO
             logger.warn(f"Config debug level was unexpected type {type(level)}, defaulting to logging.INFO.", logging.WARN)
         return ret_val
 
     @staticmethod
-    def _parseVersion(version, logger:logging.Logger) -> str:
-        ret_val : str
+    def _parseVersion(version, logger:logging.Logger) -> SemanticVersion:
+        ret_val : SemanticVersion
         if isinstance(version, int):
-            ret_val = str(version)
+            ret_val = SemanticVersion(major=version)
         elif isinstance(version, str):
-            ret_val = version
+            ret_val = SemanticVersion.FromString(semver=version)
         else:
-            ret_val = str(version)
-            logger.warn(f"Config version was unexpected type {type(version)}, defaulting to str(version)={ret_val}.", logging.WARN)
+            ret_val = SemanticVersion.FromString(str(version))
+            logger.warn(f"Config version was unexpected type {type(version)}, defaulting to SemanticVersion(str(version))={ret_val}.", logging.WARN)
         return ret_val
```

### Comparing `opengamedata_api_utils-1.0.3/src/ogd/apis/utils/APIResponse.py` & `opengamedata_api_utils-1.0.4/src/ogd/apis/utils/APIResponse.py`

 * *Files identical despite different names*

### Comparing `opengamedata_api_utils-1.0.3/src/ogd/apis/utils/APIUtils.py` & `opengamedata_api_utils-1.0.4/src/ogd/apis/utils/APIUtils.py`

 * *Files identical despite different names*

### Comparing `opengamedata_api_utils-1.0.3/src/ogd/apis/utils/HelloAPI.py` & `opengamedata_api_utils-1.0.4/src/ogd/apis/utils/HelloAPI.py`

 * *Files identical despite different names*

### Comparing `opengamedata_api_utils-1.0.3/src/opengamedata_api_utils.egg-info/PKG-INFO` & `opengamedata_api_utils-1.0.4/src/opengamedata_api_utils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opengamedata-api-utils
-Version: 1.0.3
+Version: 1.0.4
 Summary: Package of utilities for server-side scripts in OpenGameData.
 Author: Ryan Wilkinson, Glenn Palmer, Daus Husaini
 Author-email: Luke Swanson <superscription58@gmail.com>
 Project-URL: Homepage, https://github.com/opengamedata/opengamedata-api-utils
 Project-URL: Bug Tracker, https://github.com/opengamedata/opengamedata-api-utils/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

