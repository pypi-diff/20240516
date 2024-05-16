# Comparing `tmp/wherobots_python_dbapi-0.5.2.tar.gz` & `tmp/wherobots_python_dbapi-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wherobots_python_dbapi-0.5.2.tar", max compression
+gzip compressed data, was "wherobots_python_dbapi-0.5.3.tar", max compression
```

## Comparing `wherobots_python_dbapi-0.5.2.tar` & `wherobots_python_dbapi-0.5.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0    11357 2024-05-14 22:03:59.455281 wherobots_python_dbapi-0.5.2/LICENSE
--rw-r--r--   0        0        0     2651 2024-05-14 22:03:59.455281 wherobots_python_dbapi-0.5.2/README.md
--rw-r--r--   0        0        0      944 2024-05-14 22:03:59.455281 wherobots_python_dbapi-0.5.2/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-14 22:03:59.455281 wherobots_python_dbapi-0.5.2/wherobots/__init__.py
--rw-r--r--   0        0        0      184 2024-05-14 22:03:59.455281 wherobots_python_dbapi-0.5.2/wherobots/db/__init__.py
--rw-r--r--   0        0        0     8317 2024-05-14 22:03:59.455281 wherobots_python_dbapi-0.5.2/wherobots/db/connection.py
--rw-r--r--   0        0        0     1767 2024-05-14 22:03:59.455281 wherobots_python_dbapi-0.5.2/wherobots/db/constants.py
--rw-r--r--   0        0        0     2774 2024-05-14 22:03:59.455281 wherobots_python_dbapi-0.5.2/wherobots/db/cursor.py
--rw-r--r--   0        0        0     5928 2024-05-14 22:03:59.455281 wherobots_python_dbapi-0.5.2/wherobots/db/driver.py
--rw-r--r--   0        0        0      310 2024-05-14 22:03:59.459281 wherobots_python_dbapi-0.5.2/wherobots/db/errors.py
--rw-r--r--   0        0        0       80 2024-05-14 22:03:59.459281 wherobots_python_dbapi-0.5.2/wherobots/db/region.py
--rw-r--r--   0        0        0      491 2024-05-14 22:03:59.459281 wherobots_python_dbapi-0.5.2/wherobots/db/runtime.py
--rw-r--r--   0        0        0     3495 1970-01-01 00:00:00.000000 wherobots_python_dbapi-0.5.2/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-16 05:29:16.307048 wherobots_python_dbapi-0.5.3/LICENSE
+-rw-r--r--   0        0        0     2651 2024-05-16 05:29:16.307048 wherobots_python_dbapi-0.5.3/README.md
+-rw-r--r--   0        0        0      944 2024-05-16 05:29:16.311048 wherobots_python_dbapi-0.5.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-16 05:29:16.311048 wherobots_python_dbapi-0.5.3/wherobots/__init__.py
+-rw-r--r--   0        0        0      184 2024-05-16 05:29:16.311048 wherobots_python_dbapi-0.5.3/wherobots/db/__init__.py
+-rw-r--r--   0        0        0     8317 2024-05-16 05:29:16.311048 wherobots_python_dbapi-0.5.3/wherobots/db/connection.py
+-rw-r--r--   0        0        0     1767 2024-05-16 05:29:16.311048 wherobots_python_dbapi-0.5.3/wherobots/db/constants.py
+-rw-r--r--   0        0        0     2774 2024-05-16 05:29:16.311048 wherobots_python_dbapi-0.5.3/wherobots/db/cursor.py
+-rw-r--r--   0        0        0     5928 2024-05-16 05:29:16.311048 wherobots_python_dbapi-0.5.3/wherobots/db/driver.py
+-rw-r--r--   0        0        0      310 2024-05-16 05:29:16.311048 wherobots_python_dbapi-0.5.3/wherobots/db/errors.py
+-rw-r--r--   0        0        0       80 2024-05-16 05:29:16.311048 wherobots_python_dbapi-0.5.3/wherobots/db/region.py
+-rw-r--r--   0        0        0      491 2024-05-16 05:29:16.311048 wherobots_python_dbapi-0.5.3/wherobots/db/runtime.py
+-rw-r--r--   0        0        0     3495 1970-01-01 00:00:00.000000 wherobots_python_dbapi-0.5.3/PKG-INFO
```

### Comparing `wherobots_python_dbapi-0.5.2/LICENSE` & `wherobots_python_dbapi-0.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `wherobots_python_dbapi-0.5.2/README.md` & `wherobots_python_dbapi-0.5.3/README.md`

 * *Files identical despite different names*

### Comparing `wherobots_python_dbapi-0.5.2/pyproject.toml` & `wherobots_python_dbapi-0.5.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "wherobots-python-dbapi"
-version = "0.5.2"
+version = "0.5.3"
 description = "Python DB-API driver for Wherobots DB"
 authors = ["Maxime Petazzoni <max@wherobots.com>"]
 license = "Apache 2.0"
 readme = "README.md"
 packages = [{ include = "wherobots" }]
 
 [project.urls]
```

### Comparing `wherobots_python_dbapi-0.5.2/wherobots/db/connection.py` & `wherobots_python_dbapi-0.5.3/wherobots/db/connection.py`

 * *Files identical despite different names*

### Comparing `wherobots_python_dbapi-0.5.2/wherobots/db/constants.py` & `wherobots_python_dbapi-0.5.3/wherobots/db/constants.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 
 DEFAULT_ENDPOINT: str = "api.cloud.wherobots.com"  # "api.cloud.wherobots.com"
 STAGING_ENDPOINT: str = "api.staging.wherobots.com"  # "api.staging.wherobots.com"
 DEFAULT_RUNTIME: Runtime = Runtime.SEDONA
 DEFAULT_REGION: Region = Region.AWS_US_WEST_2
 DEFAULT_READ_TIMEOUT_SECONDS: float = 0.25
-DEFAULT_SESSION_WAIT_TIMEOUT_SECONDS: float = 300
+DEFAULT_SESSION_WAIT_TIMEOUT_SECONDS: float = 900
 MAX_MESSAGE_SIZE: int = 100 * 2**20  # 100MiB
 PROTOCOL_VERSION: str = "1.0.0"
 
 
 class ExecutionState(LowercaseStrEnum):
     IDLE = auto()
     "Not executing any operation."
```

### Comparing `wherobots_python_dbapi-0.5.2/wherobots/db/cursor.py` & `wherobots_python_dbapi-0.5.3/wherobots/db/cursor.py`

 * *Files identical despite different names*

### Comparing `wherobots_python_dbapi-0.5.2/wherobots/db/driver.py` & `wherobots_python_dbapi-0.5.3/wherobots/db/driver.py`

 * *Files identical despite different names*

### Comparing `wherobots_python_dbapi-0.5.2/PKG-INFO` & `wherobots_python_dbapi-0.5.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wherobots-python-dbapi
-Version: 0.5.2
+Version: 0.5.3
 Summary: Python DB-API driver for Wherobots DB
 License: Apache 2.0
 Author: Maxime Petazzoni
 Author-email: max@wherobots.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

