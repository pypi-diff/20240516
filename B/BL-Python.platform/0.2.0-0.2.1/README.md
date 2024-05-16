# Comparing `tmp/bl_python_platform-0.2.0.tar.gz` & `tmp/bl_python_platform-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bl_python_platform-0.2.0.tar", last modified: Tue May 14 21:39:45 2024, max compression
+gzip compressed data, was "bl_python_platform-0.2.1.tar", last modified: Thu May 16 21:22:27 2024, max compression
```

## Comparing `bl_python_platform-0.2.0.tar` & `bl_python_platform-0.2.1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:39:45.481477 bl_python_platform-0.2.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:39:45.477477 bl_python_platform-0.2.0/BL_Python/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:39:45.481477 bl_python_platform-0.2.0/BL_Python/platform/
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-14 21:39:40.000000 bl_python_platform-0.2.0/BL_Python/platform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2538 2024-05-14 21:39:40.000000 bl_python_platform-0.2.0/BL_Python/platform/dependency_injection.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:39:45.481477 bl_python_platform-0.2.0/BL_Python/platform/feature_flag/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 21:39:40.000000 bl_python_platform-0.2.0/BL_Python/platform/feature_flag/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4605 2024-05-14 21:39:40.000000 bl_python_platform-0.2.0/BL_Python/platform/feature_flag/db_feature_flag_router.py
--rw-r--r--   0 runner    (1001) docker     (127)     2186 2024-05-14 21:39:40.000000 bl_python_platform-0.2.0/BL_Python/platform/feature_flag/feature_flag_router.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:39:45.481477 bl_python_platform-0.2.0/BL_Python/platform/identity/
--rw-r--r--   0 runner    (1001) docker     (127)     4237 2024-05-14 21:39:40.000000 bl_python_platform-0.2.0/BL_Python/platform/identity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5337 2024-05-14 21:39:40.000000 bl_python_platform-0.2.0/BL_Python/platform/identity/user_loader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:39:45.481477 bl_python_platform-0.2.0/BL_Python.platform.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1437 2024-05-14 21:39:45.000000 bl_python_platform-0.2.0/BL_Python.platform.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      668 2024-05-14 21:39:45.000000 bl_python_platform-0.2.0/BL_Python.platform.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 21:39:45.000000 bl_python_platform-0.2.0/BL_Python.platform.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-14 21:39:45.000000 bl_python_platform-0.2.0/BL_Python.platform.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-14 21:39:45.000000 bl_python_platform-0.2.0/BL_Python.platform.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)    18092 2024-05-14 21:39:40.000000 bl_python_platform-0.2.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-14 21:39:40.000000 bl_python_platform-0.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1437 2024-05-14 21:39:45.481477 bl_python_platform-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      317 2024-05-14 21:39:40.000000 bl_python_platform-0.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 21:39:40.000000 bl_python_platform-0.2.0/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     1504 2024-05-14 21:39:40.000000 bl_python_platform-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 21:39:45.481477 bl_python_platform-0.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:39:45.477477 bl_python_platform-0.2.0/test/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:39:45.477477 bl_python_platform-0.2.0/test/unit/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:39:45.481477 bl_python_platform-0.2.0/test/unit/feature_flags/
--rw-r--r--   0 runner    (1001) docker     (127)     8577 2024-05-14 21:39:40.000000 bl_python_platform-0.2.0/test/unit/feature_flags/test_db_feature_flag_router.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:39:45.481477 bl_python_platform-0.2.0/test/unit/identity/
--rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-05-14 21:39:40.000000 bl_python_platform-0.2.0/test/unit/identity/test_loader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 21:22:27.524834 bl_python_platform-0.2.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 21:22:27.516834 bl_python_platform-0.2.1/BL_Python/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 21:22:27.520834 bl_python_platform-0.2.1/BL_Python/platform/
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-16 21:22:23.000000 bl_python_platform-0.2.1/BL_Python/platform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2538 2024-05-16 21:22:23.000000 bl_python_platform-0.2.1/BL_Python/platform/dependency_injection.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 21:22:27.520834 bl_python_platform-0.2.1/BL_Python/platform/feature_flag/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 21:22:23.000000 bl_python_platform-0.2.1/BL_Python/platform/feature_flag/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4605 2024-05-16 21:22:23.000000 bl_python_platform-0.2.1/BL_Python/platform/feature_flag/db_feature_flag_router.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2186 2024-05-16 21:22:23.000000 bl_python_platform-0.2.1/BL_Python/platform/feature_flag/feature_flag_router.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 21:22:27.524834 bl_python_platform-0.2.1/BL_Python/platform/identity/
+-rw-r--r--   0 runner    (1001) docker     (127)     4237 2024-05-16 21:22:23.000000 bl_python_platform-0.2.1/BL_Python/platform/identity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6942 2024-05-16 21:22:23.000000 bl_python_platform-0.2.1/BL_Python/platform/identity/user_loader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 21:22:27.524834 bl_python_platform-0.2.1/BL_Python.platform.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1437 2024-05-16 21:22:27.000000 bl_python_platform-0.2.1/BL_Python.platform.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2024-05-16 21:22:27.000000 bl_python_platform-0.2.1/BL_Python.platform.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 21:22:27.000000 bl_python_platform-0.2.1/BL_Python.platform.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-16 21:22:27.000000 bl_python_platform-0.2.1/BL_Python.platform.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-16 21:22:27.000000 bl_python_platform-0.2.1/BL_Python.platform.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    18092 2024-05-16 21:22:23.000000 bl_python_platform-0.2.1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-16 21:22:23.000000 bl_python_platform-0.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1437 2024-05-16 21:22:27.524834 bl_python_platform-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-05-16 21:22:23.000000 bl_python_platform-0.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 21:22:23.000000 bl_python_platform-0.2.1/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     1504 2024-05-16 21:22:23.000000 bl_python_platform-0.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 21:22:27.524834 bl_python_platform-0.2.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 21:22:27.520834 bl_python_platform-0.2.1/test/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 21:22:27.520834 bl_python_platform-0.2.1/test/unit/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 21:22:27.524834 bl_python_platform-0.2.1/test/unit/feature_flags/
+-rw-r--r--   0 runner    (1001) docker     (127)     8577 2024-05-16 21:22:23.000000 bl_python_platform-0.2.1/test/unit/feature_flags/test_db_feature_flag_router.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 21:22:27.524834 bl_python_platform-0.2.1/test/unit/identity/
+-rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-05-16 21:22:23.000000 bl_python_platform-0.2.1/test/unit/identity/test_loader.py
```

### Comparing `bl_python_platform-0.2.0/BL_Python/platform/dependency_injection.py` & `bl_python_platform-0.2.1/BL_Python/platform/dependency_injection.py`

 * *Files identical despite different names*

### Comparing `bl_python_platform-0.2.0/BL_Python/platform/feature_flag/db_feature_flag_router.py` & `bl_python_platform-0.2.1/BL_Python/platform/feature_flag/db_feature_flag_router.py`

 * *Files identical despite different names*

### Comparing `bl_python_platform-0.2.0/BL_Python/platform/feature_flag/feature_flag_router.py` & `bl_python_platform-0.2.1/BL_Python/platform/feature_flag/feature_flag_router.py`

 * *Files identical despite different names*

### Comparing `bl_python_platform-0.2.0/BL_Python/platform/identity/__init__.py` & `bl_python_platform-0.2.1/BL_Python/platform/identity/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_python_platform-0.2.0/BL_Python.platform.egg-info/PKG-INFO` & `bl_python_platform-0.2.1/BL_Python.platform.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BL_Python.platform
-Version: 0.2.0
+Version: 0.2.1
 Summary: Libraries for developing PaaS software in Boutros Lab.
 Author-email: Aaron Holmes <aholmes@mednet.ucla.edu>
 Project-URL: Homepage, https://github.com/uclahs-cds/BL_Python
 Project-URL: Bug Tracker, https://github.com/uclahs-cds/BL_Python/issues
 Project-URL: Repository, https://github.com/uclahs-cds/BL_Python.git
 Project-URL: Changelog, https://github.com/uclahs-cds/BL_Python/blob/main/CHANGELOG.md
 Classifier: Programming Language :: Python :: 3
```

### Comparing `bl_python_platform-0.2.0/BL_Python.platform.egg-info/SOURCES.txt` & `bl_python_platform-0.2.1/BL_Python.platform.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bl_python_platform-0.2.0/LICENSE.md` & `bl_python_platform-0.2.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `bl_python_platform-0.2.0/PKG-INFO` & `bl_python_platform-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BL_Python.platform
-Version: 0.2.0
+Version: 0.2.1
 Summary: Libraries for developing PaaS software in Boutros Lab.
 Author-email: Aaron Holmes <aholmes@mednet.ucla.edu>
 Project-URL: Homepage, https://github.com/uclahs-cds/BL_Python
 Project-URL: Bug Tracker, https://github.com/uclahs-cds/BL_Python/issues
 Project-URL: Repository, https://github.com/uclahs-cds/BL_Python.git
 Project-URL: Changelog, https://github.com/uclahs-cds/BL_Python/blob/main/CHANGELOG.md
 Classifier: Programming Language :: Python :: 3
```

### Comparing `bl_python_platform-0.2.0/pyproject.toml` & `bl_python_platform-0.2.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `bl_python_platform-0.2.0/test/unit/feature_flags/test_db_feature_flag_router.py` & `bl_python_platform-0.2.1/test/unit/feature_flags/test_db_feature_flag_router.py`

 * *Files identical despite different names*

### Comparing `bl_python_platform-0.2.0/test/unit/identity/test_loader.py` & `bl_python_platform-0.2.1/test/unit/identity/test_loader.py`

 * *Files identical despite different names*

