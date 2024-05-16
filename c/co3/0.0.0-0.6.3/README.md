# Comparing `tmp/co3-0.0.0.tar.gz` & `tmp/co3-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "co3-0.0.0.tar", last modified: Thu May 16 03:04:55 2024, max compression
+gzip compressed data, was "co3-0.6.3.tar", last modified: Thu May 16 03:08:48 2024, max compression
```

## Comparing `co3-0.0.0.tar` & `co3-0.6.3.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxr-xr-x   0 smgr      (1000) smgr      (1000)        0 2024-05-16 03:04:55.974601 co3-0.0.0/
--rw-r--r--   0 smgr      (1000) smgr      (1000)     1071 2024-05-16 03:01:31.000000 co3-0.0.0/LICENSE
--rw-r--r--   0 smgr      (1000) smgr      (1000)        0 2024-05-16 03:01:31.000000 co3-0.0.0/MANIFEST.in
--rw-r--r--   0 smgr      (1000) smgr      (1000)     3264 2024-05-16 03:04:55.974601 co3-0.0.0/PKG-INFO
--rw-r--r--   0 smgr      (1000) smgr      (1000)     2109 2024-05-16 03:01:31.000000 co3-0.0.0/README.md
-drwxr-xr-x   0 smgr      (1000) smgr      (1000)        0 2024-05-16 03:04:55.971268 co3-0.0.0/co3/
--rw-r--r--   0 smgr      (1000) smgr      (1000)     5147 2024-05-16 03:01:31.000000 co3-0.0.0/co3/__init__.py
--rw-r--r--   0 smgr      (1000) smgr      (1000)     1165 2024-05-16 03:01:31.000000 co3-0.0.0/co3/accessor.py
-drwxr-xr-x   0 smgr      (1000) smgr      (1000)        0 2024-05-16 03:04:55.971268 co3-0.0.0/co3/accessors/
--rw-r--r--   0 smgr      (1000) smgr      (1000)     1357 2024-05-16 03:01:31.000000 co3-0.0.0/co3/accessors/__init__.py
--rw-r--r--   0 smgr      (1000) smgr      (1000)     4388 2024-05-16 03:01:31.000000 co3-0.0.0/co3/accessors/fts.py
--rw-r--r--   0 smgr      (1000) smgr      (1000)     6328 2024-05-16 03:01:31.000000 co3-0.0.0/co3/accessors/sql.py
--rw-r--r--   0 smgr      (1000) smgr      (1000)     2547 2024-05-16 03:01:31.000000 co3-0.0.0/co3/accessors/vss.py
--rw-r--r--   0 smgr      (1000) smgr      (1000)    13954 2024-05-16 03:01:31.000000 co3-0.0.0/co3/co3.py
--rw-r--r--   0 smgr      (1000) smgr      (1000)     4725 2024-05-16 03:01:31.000000 co3-0.0.0/co3/collector.py
--rw-r--r--   0 smgr      (1000) smgr      (1000)      609 2024-05-16 03:01:31.000000 co3-0.0.0/co3/component.py
-drwxr-xr-x   0 smgr      (1000) smgr      (1000)        0 2024-05-16 03:04:55.971268 co3-0.0.0/co3/components/
--rw-r--r--   0 smgr      (1000) smgr      (1000)     4109 2024-05-16 03:01:31.000000 co3-0.0.0/co3/components/__init__.py
--rw-r--r--   0 smgr      (1000) smgr      (1000)     6895 2024-05-16 03:01:31.000000 co3-0.0.0/co3/database.py
-drwxr-xr-x   0 smgr      (1000) smgr      (1000)        0 2024-05-16 03:04:55.974601 co3-0.0.0/co3/databases/
--rw-r--r--   0 smgr      (1000) smgr      (1000)      116 2024-05-16 03:01:31.000000 co3-0.0.0/co3/databases/__init__.py
--rw-r--r--   0 smgr      (1000) smgr      (1000)      201 2024-05-16 03:01:31.000000 co3-0.0.0/co3/databases/fts.py
--rw-r--r--   0 smgr      (1000) smgr      (1000)     1123 2024-05-16 03:01:31.000000 co3-0.0.0/co3/databases/sql.py
--rw-r--r--   0 smgr      (1000) smgr      (1000)      202 2024-05-16 03:01:31.000000 co3-0.0.0/co3/databases/vss.py
--rw-r--r--   0 smgr      (1000) smgr      (1000)     1785 2024-05-16 03:01:31.000000 co3-0.0.0/co3/differ.py
--rw-r--r--   0 smgr      (1000) smgr      (1000)     4128 2024-05-16 03:01:31.000000 co3-0.0.0/co3/engine.py
-drwxr-xr-x   0 smgr      (1000) smgr      (1000)        0 2024-05-16 03:04:55.974601 co3-0.0.0/co3/engines/
--rw-r--r--   0 smgr      (1000) smgr      (1000)     1502 2024-05-16 03:01:31.000000 co3-0.0.0/co3/engines/__init__.py
--rw-r--r--   0 smgr      (1000) smgr      (1000)    16768 2024-05-16 03:01:31.000000 co3-0.0.0/co3/indexer.py
-drwxr-xr-x   0 smgr      (1000) smgr      (1000)        0 2024-05-16 03:04:55.974601 co3-0.0.0/co3/indexers/
--rw-r--r--   0 smgr      (1000) smgr      (1000)     1163 2024-05-16 03:01:31.000000 co3-0.0.0/co3/indexers/relational.py
--rw-r--r--   0 smgr      (1000) smgr      (1000)     1054 2024-05-16 03:01:31.000000 co3-0.0.0/co3/manager.py
-drwxr-xr-x   0 smgr      (1000) smgr      (1000)        0 2024-05-16 03:04:55.974601 co3-0.0.0/co3/managers/
--rw-r--r--   0 smgr      (1000) smgr      (1000)      120 2024-05-16 03:01:31.000000 co3-0.0.0/co3/managers/__init__.py
--rw-r--r--   0 smgr      (1000) smgr      (1000)     1028 2024-05-16 03:01:31.000000 co3-0.0.0/co3/managers/fts.py
--rw-r--r--   0 smgr      (1000) smgr      (1000)     6644 2024-05-16 03:01:31.000000 co3-0.0.0/co3/managers/sql.py
--rw-r--r--   0 smgr      (1000) smgr      (1000)      228 2024-05-16 03:01:31.000000 co3-0.0.0/co3/managers/vss.py
--rw-r--r--   0 smgr      (1000) smgr      (1000)    22876 2024-05-16 03:01:31.000000 co3-0.0.0/co3/mapper.py
-drwxr-xr-x   0 smgr      (1000) smgr      (1000)        0 2024-05-16 03:04:55.974601 co3-0.0.0/co3/mappers/
--rw-r--r--   0 smgr      (1000) smgr      (1000)     2606 2024-05-16 03:01:31.000000 co3-0.0.0/co3/mappers/__init__.py
--rw-r--r--   0 smgr      (1000) smgr      (1000)      176 2024-05-16 03:01:31.000000 co3-0.0.0/co3/resource.py
-drwxr-xr-x   0 smgr      (1000) smgr      (1000)        0 2024-05-16 03:04:55.974601 co3-0.0.0/co3/resources/
--rw-r--r--   0 smgr      (1000) smgr      (1000)       44 2024-05-16 03:01:31.000000 co3-0.0.0/co3/resources/__init__.py
--rw-r--r--   0 smgr      (1000) smgr      (1000)      826 2024-05-16 03:01:31.000000 co3-0.0.0/co3/resources/disk.py
--rw-r--r--   0 smgr      (1000) smgr      (1000)     1304 2024-05-16 03:01:31.000000 co3-0.0.0/co3/schema.py
-drwxr-xr-x   0 smgr      (1000) smgr      (1000)        0 2024-05-16 03:04:55.974601 co3-0.0.0/co3/schemas/
--rw-r--r--   0 smgr      (1000) smgr      (1000)      493 2024-05-16 03:01:31.000000 co3-0.0.0/co3/schemas/__init__.py
--rw-r--r--   0 smgr      (1000) smgr      (1000)    10748 2024-05-16 03:01:31.000000 co3-0.0.0/co3/syncer.py
-drwxr-xr-x   0 smgr      (1000) smgr      (1000)        0 2024-05-16 03:04:55.974601 co3-0.0.0/co3/util/
--rw-r--r--   0 smgr      (1000) smgr      (1000)      134 2024-05-16 03:01:31.000000 co3-0.0.0/co3/util/__init__.py
--rw-r--r--   0 smgr      (1000) smgr      (1000)     7321 2024-05-16 03:01:31.000000 co3-0.0.0/co3/util/db.py
--rw-r--r--   0 smgr      (1000) smgr      (1000)      241 2024-05-16 03:01:31.000000 co3-0.0.0/co3/util/generic.py
--rw-r--r--   0 smgr      (1000) smgr      (1000)     1400 2024-05-16 03:01:31.000000 co3-0.0.0/co3/util/paths.py
--rw-r--r--   0 smgr      (1000) smgr      (1000)      142 2024-05-16 03:01:31.000000 co3-0.0.0/co3/util/regex.py
--rw-r--r--   0 smgr      (1000) smgr      (1000)     1400 2024-05-16 03:01:31.000000 co3-0.0.0/co3/util/types.py
-drwxr-xr-x   0 smgr      (1000) smgr      (1000)        0 2024-05-16 03:04:55.974601 co3-0.0.0/co3.egg-info/
--rw-r--r--   0 smgr      (1000) smgr      (1000)     3264 2024-05-16 03:04:55.000000 co3-0.0.0/co3.egg-info/PKG-INFO
--rw-r--r--   0 smgr      (1000) smgr      (1000)     1039 2024-05-16 03:04:55.000000 co3-0.0.0/co3.egg-info/SOURCES.txt
--rw-r--r--   0 smgr      (1000) smgr      (1000)        1 2024-05-16 03:04:55.000000 co3-0.0.0/co3.egg-info/dependency_links.txt
--rw-r--r--   0 smgr      (1000) smgr      (1000)      132 2024-05-16 03:04:55.000000 co3-0.0.0/co3.egg-info/requires.txt
--rw-r--r--   0 smgr      (1000) smgr      (1000)        4 2024-05-16 03:04:55.000000 co3-0.0.0/co3.egg-info/top_level.txt
--rw-r--r--   0 smgr      (1000) smgr      (1000)     1198 2024-05-16 03:01:31.000000 co3-0.0.0/pyproject.toml
--rw-r--r--   0 smgr      (1000) smgr      (1000)       38 2024-05-16 03:04:55.974601 co3-0.0.0/setup.cfg
-drwxr-xr-x   0 smgr      (1000) smgr      (1000)        0 2024-05-16 03:04:55.974601 co3-0.0.0/tests/
--rw-r--r--   0 smgr      (1000) smgr      (1000)     1187 2024-05-16 03:01:31.000000 co3-0.0.0/tests/test_co3.py
--rw-r--r--   0 smgr      (1000) smgr      (1000)     1330 2024-05-16 03:01:31.000000 co3-0.0.0/tests/test_database.py
--rw-r--r--   0 smgr      (1000) smgr      (1000)      650 2024-05-16 03:01:31.000000 co3-0.0.0/tests/test_imports.py
--rw-r--r--   0 smgr      (1000) smgr      (1000)     1851 2024-05-16 03:01:31.000000 co3-0.0.0/tests/test_mapper.py
--rw-r--r--   0 smgr      (1000) smgr      (1000)      953 2024-05-16 03:01:31.000000 co3-0.0.0/tests/test_schema.py
+drwxr-xr-x   0 smgr      (1000) smgr      (1000)        0 2024-05-16 03:08:48.981302 co3-0.6.3/
+-rw-r--r--   0 smgr      (1000) smgr      (1000)     1071 2024-05-16 03:01:31.000000 co3-0.6.3/LICENSE
+-rw-r--r--   0 smgr      (1000) smgr      (1000)        0 2024-05-16 03:01:31.000000 co3-0.6.3/MANIFEST.in
+-rw-r--r--   0 smgr      (1000) smgr      (1000)     3264 2024-05-16 03:08:48.981302 co3-0.6.3/PKG-INFO
+-rw-r--r--   0 smgr      (1000) smgr      (1000)     2109 2024-05-16 03:01:31.000000 co3-0.6.3/README.md
+drwxr-xr-x   0 smgr      (1000) smgr      (1000)        0 2024-05-16 03:08:48.974635 co3-0.6.3/co3/
+-rw-r--r--   0 smgr      (1000) smgr      (1000)     5147 2024-05-16 03:01:31.000000 co3-0.6.3/co3/__init__.py
+-rw-r--r--   0 smgr      (1000) smgr      (1000)     1165 2024-05-16 03:01:31.000000 co3-0.6.3/co3/accessor.py
+drwxr-xr-x   0 smgr      (1000) smgr      (1000)        0 2024-05-16 03:08:48.977968 co3-0.6.3/co3/accessors/
+-rw-r--r--   0 smgr      (1000) smgr      (1000)     1357 2024-05-16 03:01:31.000000 co3-0.6.3/co3/accessors/__init__.py
+-rw-r--r--   0 smgr      (1000) smgr      (1000)     4388 2024-05-16 03:01:31.000000 co3-0.6.3/co3/accessors/fts.py
+-rw-r--r--   0 smgr      (1000) smgr      (1000)     6328 2024-05-16 03:01:31.000000 co3-0.6.3/co3/accessors/sql.py
+-rw-r--r--   0 smgr      (1000) smgr      (1000)     2547 2024-05-16 03:01:31.000000 co3-0.6.3/co3/accessors/vss.py
+-rw-r--r--   0 smgr      (1000) smgr      (1000)    13954 2024-05-16 03:01:31.000000 co3-0.6.3/co3/co3.py
+-rw-r--r--   0 smgr      (1000) smgr      (1000)     4725 2024-05-16 03:01:31.000000 co3-0.6.3/co3/collector.py
+-rw-r--r--   0 smgr      (1000) smgr      (1000)      609 2024-05-16 03:01:31.000000 co3-0.6.3/co3/component.py
+drwxr-xr-x   0 smgr      (1000) smgr      (1000)        0 2024-05-16 03:08:48.977968 co3-0.6.3/co3/components/
+-rw-r--r--   0 smgr      (1000) smgr      (1000)     4109 2024-05-16 03:01:31.000000 co3-0.6.3/co3/components/__init__.py
+-rw-r--r--   0 smgr      (1000) smgr      (1000)     6895 2024-05-16 03:01:31.000000 co3-0.6.3/co3/database.py
+drwxr-xr-x   0 smgr      (1000) smgr      (1000)        0 2024-05-16 03:08:48.977968 co3-0.6.3/co3/databases/
+-rw-r--r--   0 smgr      (1000) smgr      (1000)      116 2024-05-16 03:01:31.000000 co3-0.6.3/co3/databases/__init__.py
+-rw-r--r--   0 smgr      (1000) smgr      (1000)      201 2024-05-16 03:01:31.000000 co3-0.6.3/co3/databases/fts.py
+-rw-r--r--   0 smgr      (1000) smgr      (1000)     1123 2024-05-16 03:01:31.000000 co3-0.6.3/co3/databases/sql.py
+-rw-r--r--   0 smgr      (1000) smgr      (1000)      202 2024-05-16 03:01:31.000000 co3-0.6.3/co3/databases/vss.py
+-rw-r--r--   0 smgr      (1000) smgr      (1000)     1785 2024-05-16 03:01:31.000000 co3-0.6.3/co3/differ.py
+-rw-r--r--   0 smgr      (1000) smgr      (1000)     4128 2024-05-16 03:01:31.000000 co3-0.6.3/co3/engine.py
+drwxr-xr-x   0 smgr      (1000) smgr      (1000)        0 2024-05-16 03:08:48.977968 co3-0.6.3/co3/engines/
+-rw-r--r--   0 smgr      (1000) smgr      (1000)     1502 2024-05-16 03:01:31.000000 co3-0.6.3/co3/engines/__init__.py
+-rw-r--r--   0 smgr      (1000) smgr      (1000)    16768 2024-05-16 03:01:31.000000 co3-0.6.3/co3/indexer.py
+drwxr-xr-x   0 smgr      (1000) smgr      (1000)        0 2024-05-16 03:08:48.977968 co3-0.6.3/co3/indexers/
+-rw-r--r--   0 smgr      (1000) smgr      (1000)     1163 2024-05-16 03:01:31.000000 co3-0.6.3/co3/indexers/relational.py
+-rw-r--r--   0 smgr      (1000) smgr      (1000)     1054 2024-05-16 03:01:31.000000 co3-0.6.3/co3/manager.py
+drwxr-xr-x   0 smgr      (1000) smgr      (1000)        0 2024-05-16 03:08:48.977968 co3-0.6.3/co3/managers/
+-rw-r--r--   0 smgr      (1000) smgr      (1000)      120 2024-05-16 03:01:31.000000 co3-0.6.3/co3/managers/__init__.py
+-rw-r--r--   0 smgr      (1000) smgr      (1000)     1028 2024-05-16 03:01:31.000000 co3-0.6.3/co3/managers/fts.py
+-rw-r--r--   0 smgr      (1000) smgr      (1000)     6644 2024-05-16 03:01:31.000000 co3-0.6.3/co3/managers/sql.py
+-rw-r--r--   0 smgr      (1000) smgr      (1000)      228 2024-05-16 03:01:31.000000 co3-0.6.3/co3/managers/vss.py
+-rw-r--r--   0 smgr      (1000) smgr      (1000)    22876 2024-05-16 03:01:31.000000 co3-0.6.3/co3/mapper.py
+drwxr-xr-x   0 smgr      (1000) smgr      (1000)        0 2024-05-16 03:08:48.977968 co3-0.6.3/co3/mappers/
+-rw-r--r--   0 smgr      (1000) smgr      (1000)     2606 2024-05-16 03:01:31.000000 co3-0.6.3/co3/mappers/__init__.py
+-rw-r--r--   0 smgr      (1000) smgr      (1000)      176 2024-05-16 03:01:31.000000 co3-0.6.3/co3/resource.py
+drwxr-xr-x   0 smgr      (1000) smgr      (1000)        0 2024-05-16 03:08:48.977968 co3-0.6.3/co3/resources/
+-rw-r--r--   0 smgr      (1000) smgr      (1000)       44 2024-05-16 03:01:31.000000 co3-0.6.3/co3/resources/__init__.py
+-rw-r--r--   0 smgr      (1000) smgr      (1000)      826 2024-05-16 03:01:31.000000 co3-0.6.3/co3/resources/disk.py
+-rw-r--r--   0 smgr      (1000) smgr      (1000)     1304 2024-05-16 03:01:31.000000 co3-0.6.3/co3/schema.py
+drwxr-xr-x   0 smgr      (1000) smgr      (1000)        0 2024-05-16 03:08:48.977968 co3-0.6.3/co3/schemas/
+-rw-r--r--   0 smgr      (1000) smgr      (1000)      493 2024-05-16 03:01:31.000000 co3-0.6.3/co3/schemas/__init__.py
+-rw-r--r--   0 smgr      (1000) smgr      (1000)    10748 2024-05-16 03:01:31.000000 co3-0.6.3/co3/syncer.py
+drwxr-xr-x   0 smgr      (1000) smgr      (1000)        0 2024-05-16 03:08:48.977968 co3-0.6.3/co3/util/
+-rw-r--r--   0 smgr      (1000) smgr      (1000)      134 2024-05-16 03:01:31.000000 co3-0.6.3/co3/util/__init__.py
+-rw-r--r--   0 smgr      (1000) smgr      (1000)     7321 2024-05-16 03:01:31.000000 co3-0.6.3/co3/util/db.py
+-rw-r--r--   0 smgr      (1000) smgr      (1000)      241 2024-05-16 03:01:31.000000 co3-0.6.3/co3/util/generic.py
+-rw-r--r--   0 smgr      (1000) smgr      (1000)     1400 2024-05-16 03:01:31.000000 co3-0.6.3/co3/util/paths.py
+-rw-r--r--   0 smgr      (1000) smgr      (1000)      142 2024-05-16 03:01:31.000000 co3-0.6.3/co3/util/regex.py
+-rw-r--r--   0 smgr      (1000) smgr      (1000)     1400 2024-05-16 03:01:31.000000 co3-0.6.3/co3/util/types.py
+drwxr-xr-x   0 smgr      (1000) smgr      (1000)        0 2024-05-16 03:08:48.981302 co3-0.6.3/co3.egg-info/
+-rw-r--r--   0 smgr      (1000) smgr      (1000)     3264 2024-05-16 03:08:48.000000 co3-0.6.3/co3.egg-info/PKG-INFO
+-rw-r--r--   0 smgr      (1000) smgr      (1000)     1039 2024-05-16 03:08:48.000000 co3-0.6.3/co3.egg-info/SOURCES.txt
+-rw-r--r--   0 smgr      (1000) smgr      (1000)        1 2024-05-16 03:08:48.000000 co3-0.6.3/co3.egg-info/dependency_links.txt
+-rw-r--r--   0 smgr      (1000) smgr      (1000)      132 2024-05-16 03:08:48.000000 co3-0.6.3/co3.egg-info/requires.txt
+-rw-r--r--   0 smgr      (1000) smgr      (1000)        4 2024-05-16 03:08:48.000000 co3-0.6.3/co3.egg-info/top_level.txt
+-rw-r--r--   0 smgr      (1000) smgr      (1000)     1247 2024-05-16 03:06:56.000000 co3-0.6.3/pyproject.toml
+-rw-r--r--   0 smgr      (1000) smgr      (1000)       38 2024-05-16 03:08:48.981302 co3-0.6.3/setup.cfg
+drwxr-xr-x   0 smgr      (1000) smgr      (1000)        0 2024-05-16 03:08:48.981302 co3-0.6.3/tests/
+-rw-r--r--   0 smgr      (1000) smgr      (1000)     1187 2024-05-16 03:01:31.000000 co3-0.6.3/tests/test_co3.py
+-rw-r--r--   0 smgr      (1000) smgr      (1000)     1330 2024-05-16 03:01:31.000000 co3-0.6.3/tests/test_database.py
+-rw-r--r--   0 smgr      (1000) smgr      (1000)      650 2024-05-16 03:01:31.000000 co3-0.6.3/tests/test_imports.py
+-rw-r--r--   0 smgr      (1000) smgr      (1000)     1851 2024-05-16 03:01:31.000000 co3-0.6.3/tests/test_mapper.py
+-rw-r--r--   0 smgr      (1000) smgr      (1000)      953 2024-05-16 03:01:31.000000 co3-0.6.3/tests/test_schema.py
```

### Comparing `co3-0.0.0/LICENSE` & `co3-0.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `co3-0.0.0/PKG-INFO` & `co3-0.6.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: co3
-Version: 0.0.0
+Version: 0.6.3
 Summary: Lightweight Python ORM for hierarchical storage management
 Author-email: Sam Griesemer <samgriesemer+git@gmail.com>
 Project-URL: Homepage, https://doc.olog.io/co3
 Project-URL: Documentation, https://doc.olog.io/co3
 Project-URL: Repository, https://git.olog.io/olog/co3
 Project-URL: Issues, https://git.olog.io/olog/co3/issues
 Keywords: database,orm
```

### Comparing `co3-0.0.0/README.md` & `co3-0.6.3/README.md`

 * *Files identical despite different names*

### Comparing `co3-0.0.0/co3/__init__.py` & `co3-0.6.3/co3/__init__.py`

 * *Files identical despite different names*

### Comparing `co3-0.0.0/co3/accessor.py` & `co3-0.6.3/co3/accessor.py`

 * *Files identical despite different names*

### Comparing `co3-0.0.0/co3/accessors/__init__.py` & `co3-0.6.3/co3/accessors/__init__.py`

 * *Files identical despite different names*

### Comparing `co3-0.0.0/co3/accessors/fts.py` & `co3-0.6.3/co3/accessors/fts.py`

 * *Files identical despite different names*

### Comparing `co3-0.0.0/co3/accessors/sql.py` & `co3-0.6.3/co3/accessors/sql.py`

 * *Files identical despite different names*

### Comparing `co3-0.0.0/co3/accessors/vss.py` & `co3-0.6.3/co3/accessors/vss.py`

 * *Files identical despite different names*

### Comparing `co3-0.0.0/co3/co3.py` & `co3-0.6.3/co3/co3.py`

 * *Files identical despite different names*

### Comparing `co3-0.0.0/co3/collector.py` & `co3-0.6.3/co3/collector.py`

 * *Files identical despite different names*

### Comparing `co3-0.0.0/co3/component.py` & `co3-0.6.3/co3/component.py`

 * *Files identical despite different names*

### Comparing `co3-0.0.0/co3/components/__init__.py` & `co3-0.6.3/co3/components/__init__.py`

 * *Files identical despite different names*

### Comparing `co3-0.0.0/co3/database.py` & `co3-0.6.3/co3/database.py`

 * *Files identical despite different names*

### Comparing `co3-0.0.0/co3/databases/sql.py` & `co3-0.6.3/co3/databases/sql.py`

 * *Files identical despite different names*

### Comparing `co3-0.0.0/co3/differ.py` & `co3-0.6.3/co3/differ.py`

 * *Files identical despite different names*

### Comparing `co3-0.0.0/co3/engine.py` & `co3-0.6.3/co3/engine.py`

 * *Files identical despite different names*

### Comparing `co3-0.0.0/co3/engines/__init__.py` & `co3-0.6.3/co3/engines/__init__.py`

 * *Files identical despite different names*

### Comparing `co3-0.0.0/co3/indexer.py` & `co3-0.6.3/co3/indexer.py`

 * *Files identical despite different names*

### Comparing `co3-0.0.0/co3/indexers/relational.py` & `co3-0.6.3/co3/indexers/relational.py`

 * *Files identical despite different names*

### Comparing `co3-0.0.0/co3/manager.py` & `co3-0.6.3/co3/manager.py`

 * *Files identical despite different names*

### Comparing `co3-0.0.0/co3/managers/fts.py` & `co3-0.6.3/co3/managers/fts.py`

 * *Files identical despite different names*

### Comparing `co3-0.0.0/co3/managers/sql.py` & `co3-0.6.3/co3/managers/sql.py`

 * *Files identical despite different names*

### Comparing `co3-0.0.0/co3/mapper.py` & `co3-0.6.3/co3/mapper.py`

 * *Files identical despite different names*

### Comparing `co3-0.0.0/co3/mappers/__init__.py` & `co3-0.6.3/co3/mappers/__init__.py`

 * *Files identical despite different names*

### Comparing `co3-0.0.0/co3/resources/disk.py` & `co3-0.6.3/co3/resources/disk.py`

 * *Files identical despite different names*

### Comparing `co3-0.0.0/co3/schema.py` & `co3-0.6.3/co3/schema.py`

 * *Files identical despite different names*

### Comparing `co3-0.0.0/co3/syncer.py` & `co3-0.6.3/co3/syncer.py`

 * *Files identical despite different names*

### Comparing `co3-0.0.0/co3/util/db.py` & `co3-0.6.3/co3/util/db.py`

 * *Files identical despite different names*

### Comparing `co3-0.0.0/co3/util/paths.py` & `co3-0.6.3/co3/util/paths.py`

 * *Files identical despite different names*

### Comparing `co3-0.0.0/co3/util/types.py` & `co3-0.6.3/co3/util/types.py`

 * *Files identical despite different names*

### Comparing `co3-0.0.0/co3.egg-info/PKG-INFO` & `co3-0.6.3/co3.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: co3
-Version: 0.0.0
+Version: 0.6.3
 Summary: Lightweight Python ORM for hierarchical storage management
 Author-email: Sam Griesemer <samgriesemer+git@gmail.com>
 Project-URL: Homepage, https://doc.olog.io/co3
 Project-URL: Documentation, https://doc.olog.io/co3
 Project-URL: Repository, https://git.olog.io/olog/co3
 Project-URL: Issues, https://git.olog.io/olog/co3/issues
 Keywords: database,orm
```

### Comparing `co3-0.0.0/co3.egg-info/SOURCES.txt` & `co3-0.6.3/co3.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `co3-0.0.0/pyproject.toml` & `co3-0.6.3/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel", "setuptools-git-versioning>=2.0,<3"]
 build-backend = "setuptools.build_meta"
 
+[tool.setuptools-git-versioning]
+enabled = true
+
 [project]
 name = "co3"
 description = "Lightweight Python ORM for hierarchical storage management"
 readme = "README.md"
 requires-python = ">=3.12"
 dynamic = ["version"]
 #license = {file = "LICENSE"}
```

### Comparing `co3-0.0.0/tests/test_co3.py` & `co3-0.6.3/tests/test_co3.py`

 * *Files identical despite different names*

### Comparing `co3-0.0.0/tests/test_database.py` & `co3-0.6.3/tests/test_database.py`

 * *Files identical despite different names*

### Comparing `co3-0.0.0/tests/test_imports.py` & `co3-0.6.3/tests/test_imports.py`

 * *Files identical despite different names*

### Comparing `co3-0.0.0/tests/test_mapper.py` & `co3-0.6.3/tests/test_mapper.py`

 * *Files identical despite different names*

### Comparing `co3-0.0.0/tests/test_schema.py` & `co3-0.6.3/tests/test_schema.py`

 * *Files identical despite different names*

