# Comparing `tmp/digitalhub_ml-0.4.0b4.tar.gz` & `tmp/digitalhub_ml-0.4.0b8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "digitalhub_ml-0.4.0b4.tar", last modified: Fri May  3 13:06:42 2024, max compression
+gzip compressed data, was "digitalhub_ml-0.4.0b8.tar", last modified: Tue May 14 11:02:36 2024, max compression
```

## Comparing `digitalhub_ml-0.4.0b4.tar` & `digitalhub_ml-0.4.0b8.tar`

### file list

```diff
@@ -1,33 +1,34 @@
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-03 13:06:42.175145 digitalhub_ml-0.4.0b4/
--rw-r--r--   0 mmartini  (1000) mmartini  (1000)      938 2024-05-03 13:06:42.175145 digitalhub_ml-0.4.0b4/PKG-INFO
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      462 2024-04-23 09:36:04.000000 digitalhub_ml-0.4.0b4/README.md
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-03 13:06:42.171145 digitalhub_ml-0.4.0b4/digitalhub_ml/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      304 2024-05-03 12:46:16.000000 digitalhub_ml-0.4.0b4/digitalhub_ml/__init__.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-03 13:06:42.171145 digitalhub_ml-0.4.0b4/digitalhub_ml/entities/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-02-01 11:38:37.000000 digitalhub_ml-0.4.0b4/digitalhub_ml/entities/__init__.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-03 13:06:42.171145 digitalhub_ml-0.4.0b4/digitalhub_ml/entities/models/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-02-01 11:40:22.000000 digitalhub_ml-0.4.0b4/digitalhub_ml/entities/models/__init__.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     6252 2024-05-03 12:46:17.000000 digitalhub_ml-0.4.0b4/digitalhub_ml/entities/models/crud.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     7145 2024-05-03 12:46:17.000000 digitalhub_ml-0.4.0b4/digitalhub_ml/entities/models/entity.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      318 2024-04-23 09:36:04.000000 digitalhub_ml-0.4.0b4/digitalhub_ml/entities/models/metadata.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      557 2024-04-23 09:36:04.000000 digitalhub_ml-0.4.0b4/digitalhub_ml/entities/models/spec.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      209 2024-02-15 10:15:41.000000 digitalhub_ml-0.4.0b4/digitalhub_ml/entities/models/status.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-03 13:06:42.175145 digitalhub_ml-0.4.0b4/digitalhub_ml/entities/projects/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-02-01 11:33:48.000000 digitalhub_ml-0.4.0b4/digitalhub_ml/entities/projects/__init__.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     6049 2024-05-03 12:46:16.000000 digitalhub_ml-0.4.0b4/digitalhub_ml/entities/projects/crud.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     5788 2024-05-03 12:46:17.000000 digitalhub_ml-0.4.0b4/digitalhub_ml/entities/projects/entity.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      988 2024-05-03 12:46:16.000000 digitalhub_ml-0.4.0b4/digitalhub_ml/entities/projects/spec.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      991 2024-04-23 09:36:04.000000 digitalhub_ml-0.4.0b4/digitalhub_ml/entities/registries.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-03 13:06:42.175145 digitalhub_ml-0.4.0b4/digitalhub_ml/entities/runs/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-01-23 14:34:03.000000 digitalhub_ml-0.4.0b4/digitalhub_ml/entities/runs/__init__.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      300 2024-03-07 13:39:55.000000 digitalhub_ml-0.4.0b4/digitalhub_ml/entities/runs/models.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      405 2024-05-03 12:46:16.000000 digitalhub_ml-0.4.0b4/digitalhub_ml/entities/runs/spec.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      313 2024-03-14 13:46:16.000000 digitalhub_ml-0.4.0b4/digitalhub_ml/entities/runs/status.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-03 13:06:42.175145 digitalhub_ml-0.4.0b4/digitalhub_ml.egg-info/
--rw-r--r--   0 mmartini  (1000) mmartini  (1000)      938 2024-05-03 13:06:42.000000 digitalhub_ml-0.4.0b4/digitalhub_ml.egg-info/PKG-INFO
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      864 2024-05-03 13:06:42.000000 digitalhub_ml-0.4.0b4/digitalhub_ml.egg-info/SOURCES.txt
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        1 2024-05-03 13:06:42.000000 digitalhub_ml-0.4.0b4/digitalhub_ml.egg-info/dependency_links.txt
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)       21 2024-05-03 13:06:42.000000 digitalhub_ml-0.4.0b4/digitalhub_ml.egg-info/requires.txt
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)       19 2024-05-03 13:06:42.000000 digitalhub_ml-0.4.0b4/digitalhub_ml.egg-info/top_level.txt
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1054 2024-05-03 12:31:18.000000 digitalhub_ml-0.4.0b4/pyproject.toml
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)       38 2024-05-03 13:06:42.175145 digitalhub_ml-0.4.0b4/setup.cfg
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-14 11:02:36.945569 digitalhub_ml-0.4.0b8/
+-rw-r--r--   0 mmartini  (1000) mmartini  (1000)      938 2024-05-14 11:02:36.945569 digitalhub_ml-0.4.0b8/PKG-INFO
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      462 2024-04-23 09:36:04.000000 digitalhub_ml-0.4.0b8/README.md
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-14 11:02:36.941569 digitalhub_ml-0.4.0b8/digitalhub_ml/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      304 2024-05-14 10:46:36.000000 digitalhub_ml-0.4.0b8/digitalhub_ml/__init__.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-14 11:02:36.941569 digitalhub_ml-0.4.0b8/digitalhub_ml/entities/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-02-01 11:38:37.000000 digitalhub_ml-0.4.0b8/digitalhub_ml/entities/__init__.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      436 2024-05-06 11:22:14.000000 digitalhub_ml-0.4.0b8/digitalhub_ml/entities/entity_types.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-14 11:02:36.945569 digitalhub_ml-0.4.0b8/digitalhub_ml/entities/models/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-02-01 11:40:22.000000 digitalhub_ml-0.4.0b8/digitalhub_ml/entities/models/__init__.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     6328 2024-05-14 10:46:36.000000 digitalhub_ml-0.4.0b8/digitalhub_ml/entities/models/crud.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     7285 2024-05-14 10:46:36.000000 digitalhub_ml-0.4.0b8/digitalhub_ml/entities/models/entity.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      318 2024-04-23 09:36:04.000000 digitalhub_ml-0.4.0b8/digitalhub_ml/entities/models/metadata.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      557 2024-05-06 10:38:24.000000 digitalhub_ml-0.4.0b8/digitalhub_ml/entities/models/spec.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      209 2024-02-15 10:15:41.000000 digitalhub_ml-0.4.0b8/digitalhub_ml/entities/models/status.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-14 11:02:36.945569 digitalhub_ml-0.4.0b8/digitalhub_ml/entities/projects/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-02-01 11:33:48.000000 digitalhub_ml-0.4.0b8/digitalhub_ml/entities/projects/__init__.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     6049 2024-05-14 10:46:36.000000 digitalhub_ml-0.4.0b8/digitalhub_ml/entities/projects/crud.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     5869 2024-05-14 10:46:36.000000 digitalhub_ml-0.4.0b8/digitalhub_ml/entities/projects/entity.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      988 2024-05-14 10:46:36.000000 digitalhub_ml-0.4.0b8/digitalhub_ml/entities/projects/spec.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      730 2024-05-06 11:19:46.000000 digitalhub_ml-0.4.0b8/digitalhub_ml/entities/registries.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-14 11:02:36.945569 digitalhub_ml-0.4.0b8/digitalhub_ml/entities/runs/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-01-23 14:34:03.000000 digitalhub_ml-0.4.0b8/digitalhub_ml/entities/runs/__init__.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      300 2024-03-07 13:39:55.000000 digitalhub_ml-0.4.0b8/digitalhub_ml/entities/runs/models.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      405 2024-05-14 10:46:36.000000 digitalhub_ml-0.4.0b8/digitalhub_ml/entities/runs/spec.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      313 2024-03-14 13:46:16.000000 digitalhub_ml-0.4.0b8/digitalhub_ml/entities/runs/status.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-14 11:02:36.945569 digitalhub_ml-0.4.0b8/digitalhub_ml.egg-info/
+-rw-r--r--   0 mmartini  (1000) mmartini  (1000)      938 2024-05-14 11:02:36.000000 digitalhub_ml-0.4.0b8/digitalhub_ml.egg-info/PKG-INFO
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      903 2024-05-14 11:02:36.000000 digitalhub_ml-0.4.0b8/digitalhub_ml.egg-info/SOURCES.txt
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        1 2024-05-14 11:02:36.000000 digitalhub_ml-0.4.0b8/digitalhub_ml.egg-info/dependency_links.txt
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)       21 2024-05-14 11:02:36.000000 digitalhub_ml-0.4.0b8/digitalhub_ml.egg-info/requires.txt
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)       19 2024-05-14 11:02:36.000000 digitalhub_ml-0.4.0b8/digitalhub_ml.egg-info/top_level.txt
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1054 2024-05-13 12:41:00.000000 digitalhub_ml-0.4.0b8/pyproject.toml
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)       38 2024-05-14 11:02:36.945569 digitalhub_ml-0.4.0b8/setup.cfg
```

### Comparing `digitalhub_ml-0.4.0b4/PKG-INFO` & `digitalhub_ml-0.4.0b8/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: digitalhub-ml
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

### Comparing `digitalhub_ml-0.4.0b4/digitalhub_ml/entities/models/crud.py` & `digitalhub_ml-0.4.0b8/digitalhub_ml/entities/models/crud.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,21 +5,22 @@
 
 import typing
 
 from digitalhub_core.context.builder import check_context, get_context
 from digitalhub_core.utils.api import api_ctx_delete, api_ctx_list, api_ctx_read, api_ctx_update
 from digitalhub_core.utils.generic_utils import parse_entity_key
 from digitalhub_core.utils.io_utils import read_yaml
+from digitalhub_ml.entities.entity_types import EntityTypes
 from digitalhub_ml.entities.models.entity import model_from_dict, model_from_parameters
 
 if typing.TYPE_CHECKING:
     from digitalhub_ml.entities.models.entity import Model
 
 
-ENTITY_TYPE = "models"
+ENTITY_TYPE = EntityTypes.MODELS.value
 
 
 def create_model(**kwargs) -> Model:
     """
     Create a new Model instance with the specified parameters.
 
     Parameters
```

### Comparing `digitalhub_ml-0.4.0b4/digitalhub_ml/entities/models/entity.py` & `digitalhub_ml-0.4.0b8/digitalhub_ml/entities/models/entity.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,27 +10,30 @@
 from digitalhub_core.entities._base.entity import Entity
 from digitalhub_core.entities._builders.metadata import build_metadata
 from digitalhub_core.entities._builders.spec import build_spec
 from digitalhub_core.entities._builders.status import build_status
 from digitalhub_core.utils.api import api_ctx_create, api_ctx_read, api_ctx_update
 from digitalhub_core.utils.generic_utils import build_uuid, get_timestamp
 from digitalhub_core.utils.io_utils import write_yaml
+from digitalhub_ml.entities.entity_types import EntityTypes
 
 if typing.TYPE_CHECKING:
     from digitalhub_core.context.context import Context
     from digitalhub_ml.entities.models.metadata import ModelMetadata
     from digitalhub_ml.entities.models.spec import ModelSpec
     from digitalhub_ml.entities.models.status import ModelStatus
 
 
 class Model(Entity):
     """
     A class representing a model.
     """
 
+    ENTITY_TYPE = EntityTypes.MODELS.value
+
     def __init__(
         self,
         project: str,
         name: str,
         uuid: str,
         kind: str,
         metadata: ModelMetadata,
@@ -61,15 +64,15 @@
             Owner of the object.
         """
         super().__init__()
         self.project = project
         self.name = name
         self.id = uuid
         self.kind = kind
-        self.key = f"store://{project}/models/{kind}/{name}:{uuid}"
+        self.key = f"store://{project}/{self.ENTITY_TYPE}/{kind}/{name}:{uuid}"
         self.metadata = metadata
         self.spec = spec
         self.status = status
         self.user = user
 
         # Add attributes to be used in the to_dict method
         self._obj_attr.extend(["project", "name", "id", "key"])
@@ -91,35 +94,35 @@
         -------
         Model
             Entity saved.
         """
         obj = self.to_dict()
 
         if not update:
-            api = api_ctx_create(self.project, "models")
+            api = api_ctx_create(self.project, self.ENTITY_TYPE)
             new_obj = self._context().create_object(api, obj)
             self._update_attributes(new_obj)
             return self
 
         self.metadata.updated = obj["metadata"]["updated"] = get_timestamp()
-        api = api_ctx_update(self.project, "models", self.id)
+        api = api_ctx_update(self.project, self.ENTITY_TYPE, self.id)
         new_obj = self._context().update_object(api, obj)
         self._update_attributes(new_obj)
         return self
 
     def refresh(self) -> Model:
         """
         Refresh object from backend.
 
         Returns
         -------
         Model
             Entity refreshed.
         """
-        api = api_ctx_read(self.project, "models", self.id)
+        api = api_ctx_read(self.project, self.ENTITY_TYPE, self.id)
         obj = self._context().read_object(api)
         self._update_attributes(obj)
         return self
 
     def export(self, filename: str | None = None) -> None:
         """
         Export object as a YAML file.
```

### Comparing `digitalhub_ml-0.4.0b4/digitalhub_ml/entities/models/spec.py` & `digitalhub_ml-0.4.0b8/digitalhub_ml/entities/models/spec.py`

 * *Files identical despite different names*

### Comparing `digitalhub_ml-0.4.0b4/digitalhub_ml/entities/projects/crud.py` & `digitalhub_ml-0.4.0b8/digitalhub_ml/entities/projects/crud.py`

 * *Files identical despite different names*

### Comparing `digitalhub_ml-0.4.0b4/digitalhub_ml/entities/projects/entity.py` & `digitalhub_ml-0.4.0b8/digitalhub_ml/entities/projects/entity.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,22 +3,23 @@
 import typing
 
 from digitalhub_core.entities._builders.metadata import build_metadata
 from digitalhub_core.entities._builders.spec import build_spec
 from digitalhub_core.entities._builders.status import build_status
 from digitalhub_core.utils.generic_utils import build_uuid
 from digitalhub_data.entities.projects.entity import CTX_ENTITIES, FUNC_MAP, ProjectData
+from digitalhub_ml.entities.entity_types import EntityTypes
 from digitalhub_ml.entities.models.crud import create_model_from_dict, delete_model, get_model, list_models, new_model
 
 if typing.TYPE_CHECKING:
     from digitalhub_ml.entities.models.entity import Model
 
-
-CTX_ENTITIES.append("models")
-FUNC_MAP["models"] = create_model_from_dict
+MODELS = EntityTypes.MODELS.value
+CTX_ENTITIES.append(MODELS)
+FUNC_MAP[MODELS] = create_model_from_dict
 
 
 class ProjectMl(ProjectData):
     """
     ProjectMl class.
     """
 
@@ -39,15 +40,15 @@
         -------
         Model
            Object instance.
         """
         kwargs["project"] = self.name
         kwargs["kind"] = "model"
         obj = new_model(**kwargs)
-        self._add_object(obj, "models")
+        self._add_object(obj, MODELS)
         return obj
 
     def get_model(self, entity_name: str | None = None, entity_id: str | None = None, **kwargs) -> Model:
         """
         Get object from backend.
 
         Parameters
@@ -61,15 +62,15 @@
 
         Returns
         -------
         Model
             Instance of Model class.
         """
         obj = get_model(self.name, entity_name=entity_name, entity_id=entity_id, **kwargs)
-        self._add_object(obj, "models")
+        self._add_object(obj, MODELS)
         return obj
 
     def delete_model(self, entity_name: str | None = None, entity_id: str | None = None, **kwargs) -> None:
         """
         Delete a Model from project.
 
         Parameters
@@ -82,30 +83,30 @@
             Parameters to pass to the API call.
 
         Returns
         -------
         None
         """
         delete_model(self.name, entity_name=entity_name, entity_id=entity_id, **kwargs)
-        self._delete_object("models", entity_name, entity_id)
+        self._delete_object(MODELS, entity_name, entity_id)
 
     def set_model(self, model: Model) -> None:
         """
         Set a Model.
 
         Parameters
         ----------
         model : Model
             Model to set.
 
         Returns
         -------
         None
         """
-        self._add_object(model, "models")
+        self._add_object(model, MODELS)
 
     def list_models(self, **kwargs) -> list[dict]:
         """
         List models associated with the project.
 
         Parameters
         ----------
```

### Comparing `digitalhub_ml-0.4.0b4/digitalhub_ml/entities/projects/spec.py` & `digitalhub_ml-0.4.0b8/digitalhub_ml/entities/projects/spec.py`

 * *Files identical despite different names*

### Comparing `digitalhub_ml-0.4.0b4/digitalhub_ml.egg-info/PKG-INFO` & `digitalhub_ml-0.4.0b8/digitalhub_ml.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: digitalhub-ml
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

### Comparing `digitalhub_ml-0.4.0b4/digitalhub_ml.egg-info/SOURCES.txt` & `digitalhub_ml-0.4.0b8/digitalhub_ml.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 digitalhub_ml/__init__.py
 digitalhub_ml.egg-info/PKG-INFO
 digitalhub_ml.egg-info/SOURCES.txt
 digitalhub_ml.egg-info/dependency_links.txt
 digitalhub_ml.egg-info/requires.txt
 digitalhub_ml.egg-info/top_level.txt
 digitalhub_ml/entities/__init__.py
+digitalhub_ml/entities/entity_types.py
 digitalhub_ml/entities/registries.py
 digitalhub_ml/entities/models/__init__.py
 digitalhub_ml/entities/models/crud.py
 digitalhub_ml/entities/models/entity.py
 digitalhub_ml/entities/models/metadata.py
 digitalhub_ml/entities/models/spec.py
 digitalhub_ml/entities/models/status.py
```

### Comparing `digitalhub_ml-0.4.0b4/pyproject.toml` & `digitalhub_ml-0.4.0b8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "digitalhub-ml"
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
     "digitalhub-data~=0.3",
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

