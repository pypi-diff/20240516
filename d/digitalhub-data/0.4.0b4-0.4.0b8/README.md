# Comparing `tmp/digitalhub_data-0.4.0b4.tar.gz` & `tmp/digitalhub_data-0.4.0b8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "digitalhub_data-0.4.0b4.tar", last modified: Fri May  3 12:54:43 2024, max compression
+gzip compressed data, was "digitalhub_data-0.4.0b8.tar", last modified: Tue May 14 10:52:48 2024, max compression
```

## Comparing `digitalhub_data-0.4.0b4.tar` & `digitalhub_data-0.4.0b8.tar`

### file list

```diff
@@ -1,43 +1,44 @@
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-03 12:54:43.518972 digitalhub_data-0.4.0b4/
--rw-r--r--   0 mmartini  (1000) mmartini  (1000)      946 2024-05-03 12:54:43.518972 digitalhub_data-0.4.0b4/PKG-INFO
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      468 2024-04-23 09:36:04.000000 digitalhub_data-0.4.0b4/README.md
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-03 12:54:43.498972 digitalhub_data-0.4.0b4/digitalhub_data/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      329 2024-05-03 12:46:15.000000 digitalhub_data-0.4.0b4/digitalhub_data/__init__.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-03 12:54:43.502972 digitalhub_data-0.4.0b4/digitalhub_data/entities/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-01-30 10:40:56.000000 digitalhub_data-0.4.0b4/digitalhub_data/entities/__init__.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-03 12:54:43.510971 digitalhub_data-0.4.0b4/digitalhub_data/entities/dataitems/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-01-30 10:40:45.000000 digitalhub_data-0.4.0b4/digitalhub_data/entities/dataitems/__init__.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     3322 2024-05-03 12:46:16.000000 digitalhub_data-0.4.0b4/digitalhub_data/entities/dataitems/builder.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     6406 2024-05-03 12:46:16.000000 digitalhub_data-0.4.0b4/digitalhub_data/entities/dataitems/crud.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-03 12:54:43.514972 digitalhub_data-0.4.0b4/digitalhub_data/entities/dataitems/entity/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-03-04 14:42:21.000000 digitalhub_data-0.4.0b4/digitalhub_data/entities/dataitems/entity/__init__.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     6857 2024-05-03 12:46:16.000000 digitalhub_data-0.4.0b4/digitalhub_data/entities/dataitems/entity/_base.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      180 2024-03-15 13:13:54.000000 digitalhub_data-0.4.0b4/digitalhub_data/entities/dataitems/entity/dataitem.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      142 2024-03-04 15:16:25.000000 digitalhub_data-0.4.0b4/digitalhub_data/entities/dataitems/entity/iceberg.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     2985 2024-04-24 13:01:27.000000 digitalhub_data-0.4.0b4/digitalhub_data/entities/dataitems/entity/table.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      582 2024-04-23 09:36:04.000000 digitalhub_data-0.4.0b4/digitalhub_data/entities/dataitems/metadata.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1093 2024-04-08 13:12:06.000000 digitalhub_data-0.4.0b4/digitalhub_data/entities/dataitems/models.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1418 2024-04-08 13:12:04.000000 digitalhub_data-0.4.0b4/digitalhub_data/entities/dataitems/spec.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      863 2024-03-15 12:04:24.000000 digitalhub_data-0.4.0b4/digitalhub_data/entities/dataitems/status.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-03 12:54:43.514972 digitalhub_data-0.4.0b4/digitalhub_data/entities/projects/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-01-31 10:03:33.000000 digitalhub_data-0.4.0b4/digitalhub_data/entities/projects/__init__.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     6053 2024-05-03 12:46:16.000000 digitalhub_data-0.4.0b4/digitalhub_data/entities/projects/crud.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     5909 2024-05-03 12:46:16.000000 digitalhub_data-0.4.0b4/digitalhub_data/entities/projects/entity.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      950 2024-02-15 10:15:41.000000 digitalhub_data-0.4.0b4/digitalhub_data/entities/projects/spec.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1050 2024-04-23 09:36:04.000000 digitalhub_data-0.4.0b4/digitalhub_data/entities/registries.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-03 12:54:43.514972 digitalhub_data-0.4.0b4/digitalhub_data/entities/runs/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-01-22 14:51:32.000000 digitalhub_data-0.4.0b4/digitalhub_data/entities/runs/__init__.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      300 2024-03-07 13:39:55.000000 digitalhub_data-0.4.0b4/digitalhub_data/entities/runs/models.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      407 2024-03-08 13:54:39.000000 digitalhub_data-0.4.0b4/digitalhub_data/entities/runs/spec.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      351 2024-03-14 13:46:16.000000 digitalhub_data-0.4.0b4/digitalhub_data/entities/runs/status.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-03 12:54:43.518972 digitalhub_data-0.4.0b4/digitalhub_data/utils/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-01-29 10:07:05.000000 digitalhub_data-0.4.0b4/digitalhub_data/utils/__init__.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     2440 2024-02-05 09:25:21.000000 digitalhub_data-0.4.0b4/digitalhub_data/utils/data_utils.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-03 12:54:43.518972 digitalhub_data-0.4.0b4/digitalhub_data.egg-info/
--rw-r--r--   0 mmartini  (1000) mmartini  (1000)      946 2024-05-03 12:54:43.000000 digitalhub_data-0.4.0b4/digitalhub_data.egg-info/PKG-INFO
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1305 2024-05-03 12:54:43.000000 digitalhub_data-0.4.0b4/digitalhub_data.egg-info/SOURCES.txt
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        1 2024-05-03 12:54:43.000000 digitalhub_data-0.4.0b4/digitalhub_data.egg-info/dependency_links.txt
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)       21 2024-05-03 12:54:43.000000 digitalhub_data-0.4.0b4/digitalhub_data.egg-info/requires.txt
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)       21 2024-05-03 12:54:43.000000 digitalhub_data-0.4.0b4/digitalhub_data.egg-info/top_level.txt
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1056 2024-05-03 12:31:18.000000 digitalhub_data-0.4.0b4/pyproject.toml
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)       38 2024-05-03 12:54:43.518972 digitalhub_data-0.4.0b4/setup.cfg
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-14 10:52:48.187830 digitalhub_data-0.4.0b8/
+-rw-r--r--   0 mmartini  (1000) mmartini  (1000)      946 2024-05-14 10:52:48.187830 digitalhub_data-0.4.0b8/PKG-INFO
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      468 2024-04-23 09:36:04.000000 digitalhub_data-0.4.0b8/README.md
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-14 10:52:48.183830 digitalhub_data-0.4.0b8/digitalhub_data/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      329 2024-05-14 10:46:36.000000 digitalhub_data-0.4.0b8/digitalhub_data/__init__.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-14 10:52:48.183830 digitalhub_data-0.4.0b8/digitalhub_data/entities/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-01-30 10:40:56.000000 digitalhub_data-0.4.0b8/digitalhub_data/entities/__init__.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-14 10:52:48.187830 digitalhub_data-0.4.0b8/digitalhub_data/entities/dataitems/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-01-30 10:40:45.000000 digitalhub_data-0.4.0b8/digitalhub_data/entities/dataitems/__init__.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     3322 2024-05-14 10:46:36.000000 digitalhub_data-0.4.0b8/digitalhub_data/entities/dataitems/builder.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     6484 2024-05-14 10:46:36.000000 digitalhub_data-0.4.0b8/digitalhub_data/entities/dataitems/crud.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-14 10:52:48.187830 digitalhub_data-0.4.0b8/digitalhub_data/entities/dataitems/entity/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-03-04 14:42:21.000000 digitalhub_data-0.4.0b8/digitalhub_data/entities/dataitems/entity/__init__.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     6975 2024-05-14 10:46:36.000000 digitalhub_data-0.4.0b8/digitalhub_data/entities/dataitems/entity/_base.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      180 2024-03-15 13:13:54.000000 digitalhub_data-0.4.0b8/digitalhub_data/entities/dataitems/entity/dataitem.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      142 2024-03-04 15:16:25.000000 digitalhub_data-0.4.0b8/digitalhub_data/entities/dataitems/entity/iceberg.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     2994 2024-05-06 09:59:04.000000 digitalhub_data-0.4.0b8/digitalhub_data/entities/dataitems/entity/table.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      582 2024-04-23 09:36:04.000000 digitalhub_data-0.4.0b8/digitalhub_data/entities/dataitems/metadata.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1093 2024-04-08 13:12:06.000000 digitalhub_data-0.4.0b8/digitalhub_data/entities/dataitems/models.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1418 2024-04-08 13:12:04.000000 digitalhub_data-0.4.0b8/digitalhub_data/entities/dataitems/spec.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      863 2024-03-15 12:04:24.000000 digitalhub_data-0.4.0b8/digitalhub_data/entities/dataitems/status.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      415 2024-05-06 11:22:14.000000 digitalhub_data-0.4.0b8/digitalhub_data/entities/entity_types.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-14 10:52:48.187830 digitalhub_data-0.4.0b8/digitalhub_data/entities/projects/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-01-31 10:03:33.000000 digitalhub_data-0.4.0b8/digitalhub_data/entities/projects/__init__.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     6053 2024-05-14 10:46:36.000000 digitalhub_data-0.4.0b8/digitalhub_data/entities/projects/crud.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     6000 2024-05-14 10:46:36.000000 digitalhub_data-0.4.0b8/digitalhub_data/entities/projects/entity.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      950 2024-02-15 10:15:41.000000 digitalhub_data-0.4.0b8/digitalhub_data/entities/projects/spec.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      773 2024-05-06 11:19:40.000000 digitalhub_data-0.4.0b8/digitalhub_data/entities/registries.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-14 10:52:48.187830 digitalhub_data-0.4.0b8/digitalhub_data/entities/runs/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-01-22 14:51:32.000000 digitalhub_data-0.4.0b8/digitalhub_data/entities/runs/__init__.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      300 2024-03-07 13:39:55.000000 digitalhub_data-0.4.0b8/digitalhub_data/entities/runs/models.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      407 2024-03-08 13:54:39.000000 digitalhub_data-0.4.0b8/digitalhub_data/entities/runs/spec.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      351 2024-03-14 13:46:16.000000 digitalhub_data-0.4.0b8/digitalhub_data/entities/runs/status.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-14 10:52:48.187830 digitalhub_data-0.4.0b8/digitalhub_data/utils/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-01-29 10:07:05.000000 digitalhub_data-0.4.0b8/digitalhub_data/utils/__init__.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     2440 2024-02-05 09:25:21.000000 digitalhub_data-0.4.0b8/digitalhub_data/utils/data_utils.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-14 10:52:48.187830 digitalhub_data-0.4.0b8/digitalhub_data.egg-info/
+-rw-r--r--   0 mmartini  (1000) mmartini  (1000)      946 2024-05-14 10:52:48.000000 digitalhub_data-0.4.0b8/digitalhub_data.egg-info/PKG-INFO
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1346 2024-05-14 10:52:48.000000 digitalhub_data-0.4.0b8/digitalhub_data.egg-info/SOURCES.txt
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        1 2024-05-14 10:52:48.000000 digitalhub_data-0.4.0b8/digitalhub_data.egg-info/dependency_links.txt
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)       21 2024-05-14 10:52:48.000000 digitalhub_data-0.4.0b8/digitalhub_data.egg-info/requires.txt
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)       21 2024-05-14 10:52:48.000000 digitalhub_data-0.4.0b8/digitalhub_data.egg-info/top_level.txt
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1056 2024-05-13 12:41:00.000000 digitalhub_data-0.4.0b8/pyproject.toml
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)       38 2024-05-14 10:52:48.187830 digitalhub_data-0.4.0b8/setup.cfg
```

### Comparing `digitalhub_data-0.4.0b4/PKG-INFO` & `digitalhub_data-0.4.0b8/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: digitalhub-data
-Version: 0.4.0b4
+Version: 0.4.0b8
 Summary: Python SDK for DHCore
 Author-email: Fondazione Bruno Kessler <dslab@fbk.eu>, Matteo Martini <mmartini@fbk.eu>
 Keywords: data,dataops,kubernetes
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.9
```

### Comparing `digitalhub_data-0.4.0b4/digitalhub_data/entities/dataitems/builder.py` & `digitalhub_data-0.4.0b8/digitalhub_data/entities/dataitems/builder.py`

 * *Files identical despite different names*

### Comparing `digitalhub_data-0.4.0b4/digitalhub_data/entities/dataitems/crud.py` & `digitalhub_data-0.4.0b8/digitalhub_data/entities/dataitems/crud.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,20 +6,21 @@
 import typing
 
 from digitalhub_core.context.builder import check_context, get_context
 from digitalhub_core.utils.api import api_ctx_delete, api_ctx_list, api_ctx_read, api_ctx_update
 from digitalhub_core.utils.generic_utils import parse_entity_key
 from digitalhub_core.utils.io_utils import read_yaml
 from digitalhub_data.entities.dataitems.builder import dataitem_from_dict, dataitem_from_parameters
+from digitalhub_data.entities.entity_types import EntityTypes
 
 if typing.TYPE_CHECKING:
     from digitalhub_data.entities.dataitems.entity._base import Dataitem
 
 
-ENTITY_TYPE = "dataitems"
+ENTITY_TYPE = EntityTypes.DATAITEMS.value
 
 
 def create_dataitem(**kwargs) -> Dataitem:
     """
     Create a new data item with the provided parameters.
 
     Parameters
```

### Comparing `digitalhub_data-0.4.0b4/digitalhub_data/entities/dataitems/entity/_base.py` & `digitalhub_data-0.4.0b8/digitalhub_data/entities/dataitems/entity/_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,27 +12,30 @@
 from digitalhub_core.entities._builders.spec import build_spec
 from digitalhub_core.entities._builders.status import build_status
 from digitalhub_core.utils.api import api_ctx_create, api_ctx_read, api_ctx_update
 from digitalhub_core.utils.exceptions import EntityError
 from digitalhub_core.utils.generic_utils import build_uuid, get_timestamp
 from digitalhub_core.utils.io_utils import write_yaml
 from digitalhub_core.utils.uri_utils import map_uri_scheme
+from digitalhub_data.entities.entity_types import EntityTypes
 
 if typing.TYPE_CHECKING:
     from digitalhub_core.context.context import Context
     from digitalhub_data.entities.dataitems.metadata import DataitemMetadata
     from digitalhub_data.entities.dataitems.spec import DataitemSpec
     from digitalhub_data.entities.dataitems.status import DataitemStatus
 
 
 class Dataitem(Entity):
     """
     A class representing a dataitem.
     """
 
+    ENTITY_TYPE = EntityTypes.DATAITEMS.value
+
     def __init__(
         self,
         project: str,
         name: str,
         uuid: str,
         kind: str,
         metadata: DataitemMetadata,
@@ -63,15 +66,15 @@
             Owner of the object.
         """
         super().__init__()
         self.project = project
         self.name = name
         self.id = uuid
         self.kind = kind
-        self.key = f"store://{project}/dataitems/{kind}/{name}:{uuid}"
+        self.key = f"store://{project}/{self.ENTITY_TYPE}/{kind}/{name}:{uuid}"
         self.metadata = metadata
         self.spec = spec
         self.status = status
         self.user = user
 
         # Add attributes to be used in the to_dict method
         self._obj_attr.extend(["project", "name", "id", "key"])
```

### Comparing `digitalhub_data-0.4.0b4/digitalhub_data/entities/dataitems/entity/table.py` & `digitalhub_data-0.4.0b8/digitalhub_data/entities/dataitems/entity/table.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,14 +79,14 @@
 
         Returns
         -------
         str
             Path to the written dataframe.
         """
         if target_path is None:
-            target_path = f"{self.project}/dataitems/{self.kind}/{self.name}.parquet"
+            target_path = f"{self.project}/{self.ENTITY_TYPE}/{self.kind}/{self.name}.parquet"
             store = get_default_store()
         else:
             store = get_store(target_path)
         if df is None:
             df = self.as_df()
         return store.write_df(df, target_path, **kwargs)
```

### Comparing `digitalhub_data-0.4.0b4/digitalhub_data/entities/dataitems/metadata.py` & `digitalhub_data-0.4.0b8/digitalhub_data/entities/dataitems/metadata.py`

 * *Files identical despite different names*

### Comparing `digitalhub_data-0.4.0b4/digitalhub_data/entities/dataitems/models.py` & `digitalhub_data-0.4.0b8/digitalhub_data/entities/dataitems/models.py`

 * *Files identical despite different names*

### Comparing `digitalhub_data-0.4.0b4/digitalhub_data/entities/dataitems/spec.py` & `digitalhub_data-0.4.0b8/digitalhub_data/entities/dataitems/spec.py`

 * *Files identical despite different names*

### Comparing `digitalhub_data-0.4.0b4/digitalhub_data/entities/dataitems/status.py` & `digitalhub_data-0.4.0b8/digitalhub_data/entities/dataitems/status.py`

 * *Files identical despite different names*

### Comparing `digitalhub_data-0.4.0b4/digitalhub_data/entities/projects/crud.py` & `digitalhub_data-0.4.0b8/digitalhub_data/entities/projects/crud.py`

 * *Files identical despite different names*

### Comparing `digitalhub_data-0.4.0b4/digitalhub_data/entities/projects/entity.py` & `digitalhub_data-0.4.0b8/digitalhub_data/entities/projects/entity.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,21 +10,24 @@
 from digitalhub_data.entities.dataitems.crud import (
     create_dataitem_from_dict,
     delete_dataitem,
     get_dataitem,
     list_dataitems,
     new_dataitem,
 )
+from digitalhub_data.entities.entity_types import EntityTypes
 
 if typing.TYPE_CHECKING:
     from digitalhub_data.entities.dataitems.entity._base import Dataitem
 
 
-CTX_ENTITIES.append("dataitems")
-FUNC_MAP["dataitems"] = create_dataitem_from_dict
+DATAITEMS = EntityTypes.DATAITEMS.value
+
+CTX_ENTITIES.append(DATAITEMS)
+FUNC_MAP[DATAITEMS] = create_dataitem_from_dict
 
 
 class ProjectData(Project):
 
     """
     ProjectData class.
     """
@@ -45,15 +48,15 @@
         Returns
         -------
         Dataitem
            Object instance.
         """
         kwargs["project"] = self.name
         obj = new_dataitem(**kwargs)
-        self._add_object(obj, "dataitems")
+        self._add_object(obj, DATAITEMS)
         return obj
 
     def get_dataitem(self, entity_name: str | None = None, entity_id: str | None = None, **kwargs) -> Dataitem:
         """
         Get object from backend.
 
         Parameters
@@ -67,15 +70,15 @@
 
         Returns
         -------
         Dataitem
             Instance of Dataitem class.
         """
         obj = get_dataitem(self.name, entity_name=entity_name, entity_id=entity_id, **kwargs)
-        self._add_object(obj, "dataitems")
+        self._add_object(obj, DATAITEMS)
         return obj
 
     def delete_dataitem(self, entity_name: str | None = None, entity_id: str | None = None, **kwargs) -> None:
         """
         Delete a Dataitem from project.
 
         Parameters
@@ -88,30 +91,30 @@
             Parameters to pass to the API call.
 
         Returns
         -------
         None
         """
         delete_dataitem(self.name, entity_name=entity_name, entity_id=entity_id, **kwargs)
-        self._delete_object("dataitems", entity_name, entity_id)
+        self._delete_object(DATAITEMS, entity_name, entity_id)
 
     def set_dataitem(self, dataitem: Dataitem) -> None:
         """
         Set a Dataitem.
 
         Parameters
         ----------
         dataitem : Dataitem
             Dataitem to set.
 
         Returns
         -------
         None
         """
-        self._add_object(dataitem, "dataitems")
+        self._add_object(dataitem, DATAITEMS)
 
     def list_dataitems(self, **kwargs) -> list[dict]:
         """
         List dataitems associated with the project.
 
         Parameters
         ----------
```

### Comparing `digitalhub_data-0.4.0b4/digitalhub_data/entities/projects/spec.py` & `digitalhub_data-0.4.0b8/digitalhub_data/entities/projects/spec.py`

 * *Files identical despite different names*

### Comparing `digitalhub_data-0.4.0b4/digitalhub_data/utils/data_utils.py` & `digitalhub_data-0.4.0b8/digitalhub_data/utils/data_utils.py`

 * *Files identical despite different names*

### Comparing `digitalhub_data-0.4.0b4/digitalhub_data.egg-info/PKG-INFO` & `digitalhub_data-0.4.0b8/digitalhub_data.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: digitalhub-data
-Version: 0.4.0b4
+Version: 0.4.0b8
 Summary: Python SDK for DHCore
 Author-email: Fondazione Bruno Kessler <dslab@fbk.eu>, Matteo Martini <mmartini@fbk.eu>
 Keywords: data,dataops,kubernetes
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.9
```

### Comparing `digitalhub_data-0.4.0b4/digitalhub_data.egg-info/SOURCES.txt` & `digitalhub_data-0.4.0b8/digitalhub_data.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 digitalhub_data/__init__.py
 digitalhub_data.egg-info/PKG-INFO
 digitalhub_data.egg-info/SOURCES.txt
 digitalhub_data.egg-info/dependency_links.txt
 digitalhub_data.egg-info/requires.txt
 digitalhub_data.egg-info/top_level.txt
 digitalhub_data/entities/__init__.py
+digitalhub_data/entities/entity_types.py
 digitalhub_data/entities/registries.py
 digitalhub_data/entities/dataitems/__init__.py
 digitalhub_data/entities/dataitems/builder.py
 digitalhub_data/entities/dataitems/crud.py
 digitalhub_data/entities/dataitems/metadata.py
 digitalhub_data/entities/dataitems/models.py
 digitalhub_data/entities/dataitems/spec.py
```

### Comparing `digitalhub_data-0.4.0b4/pyproject.toml` & `digitalhub_data-0.4.0b8/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "digitalhub-data"
-version = "0.4.0b4"
+version = "0.4.0b8"
 description = "Python SDK for DHCore"
 readme = "README.md"
 authors = [
     { name = "Fondazione Bruno Kessler", email = "dslab@fbk.eu" },
     { name = "Matteo Martini", email = "mmartini@fbk.eu" }
 ]
 license = { file = "LICENSE.txt" }
@@ -23,15 +23,15 @@
     "digitalhub-core~=0.3",
 ]
 
 [tool.setuptools.packages.find]
 exclude = ["modules*"]
 
 [tool.bumpver]
-current_version = "0.4.0b4"
+current_version = "0.4.0b8"
 version_pattern = "MAJOR.MINOR.PATCH[PYTAGNUM]"
 commit_message  = "Bump version {old_version} -> {new_version}"
 commit          = false
 tag             = false
 push            = false
 
 [tool.bumpver.file_patterns]
```

