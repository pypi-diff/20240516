# Comparing `tmp/bl_python_platform-0.2.1.tar.gz` & `tmp/bl_python_platform-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bl_python_platform-0.2.1.tar", last modified: Thu May 16 21:22:27 2024, max compression
+gzip compressed data, was "bl_python_platform-0.2.2.tar", last modified: Thu May 16 21:52:11 2024, max compression
```

## Comparing `bl_python_platform-0.2.1.tar` & `bl_python_platform-0.2.2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 21:22:27.524834 bl_python_platform-0.2.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 21:22:27.516834 bl_python_platform-0.2.1/BL_Python/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 21:22:27.520834 bl_python_platform-0.2.1/BL_Python/platform/
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-16 21:22:23.000000 bl_python_platform-0.2.1/BL_Python/platform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2538 2024-05-16 21:22:23.000000 bl_python_platform-0.2.1/BL_Python/platform/dependency_injection.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 21:22:27.520834 bl_python_platform-0.2.1/BL_Python/platform/feature_flag/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 21:22:23.000000 bl_python_platform-0.2.1/BL_Python/platform/feature_flag/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4605 2024-05-16 21:22:23.000000 bl_python_platform-0.2.1/BL_Python/platform/feature_flag/db_feature_flag_router.py
--rw-r--r--   0 runner    (1001) docker     (127)     2186 2024-05-16 21:22:23.000000 bl_python_platform-0.2.1/BL_Python/platform/feature_flag/feature_flag_router.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 21:22:27.524834 bl_python_platform-0.2.1/BL_Python/platform/identity/
--rw-r--r--   0 runner    (1001) docker     (127)     4237 2024-05-16 21:22:23.000000 bl_python_platform-0.2.1/BL_Python/platform/identity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6942 2024-05-16 21:22:23.000000 bl_python_platform-0.2.1/BL_Python/platform/identity/user_loader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 21:22:27.524834 bl_python_platform-0.2.1/BL_Python.platform.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1437 2024-05-16 21:22:27.000000 bl_python_platform-0.2.1/BL_Python.platform.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      668 2024-05-16 21:22:27.000000 bl_python_platform-0.2.1/BL_Python.platform.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 21:22:27.000000 bl_python_platform-0.2.1/BL_Python.platform.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-16 21:22:27.000000 bl_python_platform-0.2.1/BL_Python.platform.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-16 21:22:27.000000 bl_python_platform-0.2.1/BL_Python.platform.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)    18092 2024-05-16 21:22:23.000000 bl_python_platform-0.2.1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-16 21:22:23.000000 bl_python_platform-0.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1437 2024-05-16 21:22:27.524834 bl_python_platform-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      317 2024-05-16 21:22:23.000000 bl_python_platform-0.2.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 21:22:23.000000 bl_python_platform-0.2.1/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     1504 2024-05-16 21:22:23.000000 bl_python_platform-0.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 21:22:27.524834 bl_python_platform-0.2.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 21:22:27.520834 bl_python_platform-0.2.1/test/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 21:22:27.520834 bl_python_platform-0.2.1/test/unit/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 21:22:27.524834 bl_python_platform-0.2.1/test/unit/feature_flags/
--rw-r--r--   0 runner    (1001) docker     (127)     8577 2024-05-16 21:22:23.000000 bl_python_platform-0.2.1/test/unit/feature_flags/test_db_feature_flag_router.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 21:22:27.524834 bl_python_platform-0.2.1/test/unit/identity/
--rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-05-16 21:22:23.000000 bl_python_platform-0.2.1/test/unit/identity/test_loader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 21:52:11.832151 bl_python_platform-0.2.2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 21:52:11.828151 bl_python_platform-0.2.2/BL_Python/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 21:52:11.832151 bl_python_platform-0.2.2/BL_Python/platform/
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-16 21:52:08.000000 bl_python_platform-0.2.2/BL_Python/platform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2538 2024-05-16 21:52:08.000000 bl_python_platform-0.2.2/BL_Python/platform/dependency_injection.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 21:52:11.832151 bl_python_platform-0.2.2/BL_Python/platform/feature_flag/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 21:52:08.000000 bl_python_platform-0.2.2/BL_Python/platform/feature_flag/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4605 2024-05-16 21:52:08.000000 bl_python_platform-0.2.2/BL_Python/platform/feature_flag/db_feature_flag_router.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2186 2024-05-16 21:52:08.000000 bl_python_platform-0.2.2/BL_Python/platform/feature_flag/feature_flag_router.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 21:52:11.832151 bl_python_platform-0.2.2/BL_Python/platform/identity/
+-rw-r--r--   0 runner    (1001) docker     (127)     4237 2024-05-16 21:52:08.000000 bl_python_platform-0.2.2/BL_Python/platform/identity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6944 2024-05-16 21:52:08.000000 bl_python_platform-0.2.2/BL_Python/platform/identity/user_loader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 21:52:11.832151 bl_python_platform-0.2.2/BL_Python.platform.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1437 2024-05-16 21:52:11.000000 bl_python_platform-0.2.2/BL_Python.platform.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2024-05-16 21:52:11.000000 bl_python_platform-0.2.2/BL_Python.platform.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 21:52:11.000000 bl_python_platform-0.2.2/BL_Python.platform.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-16 21:52:11.000000 bl_python_platform-0.2.2/BL_Python.platform.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-16 21:52:11.000000 bl_python_platform-0.2.2/BL_Python.platform.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    18092 2024-05-16 21:52:08.000000 bl_python_platform-0.2.2/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-16 21:52:08.000000 bl_python_platform-0.2.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1437 2024-05-16 21:52:11.832151 bl_python_platform-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-05-16 21:52:08.000000 bl_python_platform-0.2.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 21:52:08.000000 bl_python_platform-0.2.2/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     1504 2024-05-16 21:52:08.000000 bl_python_platform-0.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 21:52:11.832151 bl_python_platform-0.2.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 21:52:11.828151 bl_python_platform-0.2.2/test/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 21:52:11.828151 bl_python_platform-0.2.2/test/unit/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 21:52:11.832151 bl_python_platform-0.2.2/test/unit/feature_flags/
+-rw-r--r--   0 runner    (1001) docker     (127)     8577 2024-05-16 21:52:08.000000 bl_python_platform-0.2.2/test/unit/feature_flags/test_db_feature_flag_router.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 21:52:11.832151 bl_python_platform-0.2.2/test/unit/identity/
+-rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-05-16 21:52:08.000000 bl_python_platform-0.2.2/test/unit/identity/test_loader.py
```

### Comparing `bl_python_platform-0.2.1/BL_Python/platform/dependency_injection.py` & `bl_python_platform-0.2.2/BL_Python/platform/dependency_injection.py`

 * *Files identical despite different names*

### Comparing `bl_python_platform-0.2.1/BL_Python/platform/feature_flag/db_feature_flag_router.py` & `bl_python_platform-0.2.2/BL_Python/platform/feature_flag/db_feature_flag_router.py`

 * *Files identical despite different names*

### Comparing `bl_python_platform-0.2.1/BL_Python/platform/feature_flag/feature_flag_router.py` & `bl_python_platform-0.2.2/BL_Python/platform/feature_flag/feature_flag_router.py`

 * *Files identical despite different names*

### Comparing `bl_python_platform-0.2.1/BL_Python/platform/identity/__init__.py` & `bl_python_platform-0.2.2/BL_Python/platform/identity/__init__.py`

 * *Files identical despite different names*

### Comparing `bl_python_platform-0.2.1/BL_Python/platform/identity/user_loader.py` & `bl_python_platform-0.2.2/BL_Python/platform/identity/user_loader.py`

 * *Files 0% similar despite different names*

```diff
@@ -100,15 +100,15 @@
         try:
             # SQLAlchemy generates invalid SQL when attempting an implicit
             # LEFT JOIN between user -> user_role and user_role -> role.
             # As such, we handle the join explicitly by extracting the property
             # relationships and referencing the relevant columns.
             user_table_property_mapper = cast(Mapper, class_mapper(self._user_table))
             user_table_properties = cast(
-                list[RelationshipProperty[DbRole] | ColumnProperty],
+                "list[RelationshipProperty[DbRole] | ColumnProperty]",
                 user_table_property_mapper.iterate_properties,  # pyright: ignore[reportUnknownMemberType]
             )
             # Only extract the secondary join table (user_role).
             # We find this by matching on the `role` table relationship
             # from the `user` table.
             user_role_table = next(
                 relationship.secondary
```

### Comparing `bl_python_platform-0.2.1/BL_Python.platform.egg-info/PKG-INFO` & `bl_python_platform-0.2.2/BL_Python.platform.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BL_Python.platform
-Version: 0.2.1
+Version: 0.2.2
 Summary: Libraries for developing PaaS software in Boutros Lab.
 Author-email: Aaron Holmes <aholmes@mednet.ucla.edu>
 Project-URL: Homepage, https://github.com/uclahs-cds/BL_Python
 Project-URL: Bug Tracker, https://github.com/uclahs-cds/BL_Python/issues
 Project-URL: Repository, https://github.com/uclahs-cds/BL_Python.git
 Project-URL: Changelog, https://github.com/uclahs-cds/BL_Python/blob/main/CHANGELOG.md
 Classifier: Programming Language :: Python :: 3
```

### Comparing `bl_python_platform-0.2.1/BL_Python.platform.egg-info/SOURCES.txt` & `bl_python_platform-0.2.2/BL_Python.platform.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bl_python_platform-0.2.1/LICENSE.md` & `bl_python_platform-0.2.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `bl_python_platform-0.2.1/PKG-INFO` & `bl_python_platform-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BL_Python.platform
-Version: 0.2.1
+Version: 0.2.2
 Summary: Libraries for developing PaaS software in Boutros Lab.
 Author-email: Aaron Holmes <aholmes@mednet.ucla.edu>
 Project-URL: Homepage, https://github.com/uclahs-cds/BL_Python
 Project-URL: Bug Tracker, https://github.com/uclahs-cds/BL_Python/issues
 Project-URL: Repository, https://github.com/uclahs-cds/BL_Python.git
 Project-URL: Changelog, https://github.com/uclahs-cds/BL_Python/blob/main/CHANGELOG.md
 Classifier: Programming Language :: Python :: 3
```

### Comparing `bl_python_platform-0.2.1/pyproject.toml` & `bl_python_platform-0.2.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `bl_python_platform-0.2.1/test/unit/feature_flags/test_db_feature_flag_router.py` & `bl_python_platform-0.2.2/test/unit/feature_flags/test_db_feature_flag_router.py`

 * *Files identical despite different names*

### Comparing `bl_python_platform-0.2.1/test/unit/identity/test_loader.py` & `bl_python_platform-0.2.2/test/unit/identity/test_loader.py`

 * *Files identical despite different names*

