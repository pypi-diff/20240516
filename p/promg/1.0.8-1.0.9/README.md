# Comparing `tmp/promg-1.0.8.tar.gz` & `tmp/promg-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "promg-1.0.8.tar", last modified: Thu Feb 29 10:13:11 2024, max compression
+gzip compressed data, was "promg-1.0.9.tar", last modified: Mon Mar  4 09:04:17 2024, max compression
```

## Comparing `promg-1.0.8.tar` & `promg-1.0.9.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:13:11.357951 promg-1.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)     7652 2024-02-29 10:13:04.000000 promg-1.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-02-29 10:13:11.357951 promg-1.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      955 2024-02-29 10:13:04.000000 promg-1.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-29 10:13:11.357951 promg-1.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-02-29 10:13:04.000000 promg-1.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:13:11.349951 promg-1.0.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:13:11.349951 promg-1.0.8/src/promg/
--rw-r--r--   0 runner    (1001) docker     (127)      630 2024-02-29 10:13:04.000000 promg-1.0.8/src/promg/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:13:11.353951 promg-1.0.8/src/promg/cypher_queries/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-29 10:13:04.000000 promg-1.0.8/src/promg/cypher_queries/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11395 2024-02-29 10:13:04.000000 promg-1.0.8/src/promg/cypher_queries/data_importer_ql.py
--rw-r--r--   0 runner    (1001) docker     (127)     7218 2024-02-29 10:13:04.000000 promg-1.0.8/src/promg/cypher_queries/db_managment_ql.py
--rw-r--r--   0 runner    (1001) docker     (127)      922 2024-02-29 10:13:04.000000 promg-1.0.8/src/promg/cypher_queries/exporter_ql.py
--rw-r--r--   0 runner    (1001) docker     (127)     5722 2024-02-29 10:13:04.000000 promg-1.0.8/src/promg/cypher_queries/inference_engine_ql.py
--rw-r--r--   0 runner    (1001) docker     (127)     3660 2024-02-29 10:13:04.000000 promg-1.0.8/src/promg/cypher_queries/process_discovery_ql.py
--rw-r--r--   0 runner    (1001) docker     (127)    22790 2024-02-29 10:13:04.000000 promg-1.0.8/src/promg/cypher_queries/semantic_header_ql.py
--rw-r--r--   0 runner    (1001) docker     (127)     9542 2024-02-29 10:13:04.000000 promg-1.0.8/src/promg/cypher_queries/task_identification_ql.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:13:11.353951 promg-1.0.8/src/promg/data_managers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-29 10:13:04.000000 promg-1.0.8/src/promg/data_managers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    31712 2024-02-29 10:13:04.000000 promg-1.0.8/src/promg/data_managers/datastructures.py
--rw-r--r--   0 runner    (1001) docker     (127)    41411 2024-02-29 10:13:04.000000 promg-1.0.8/src/promg/data_managers/semantic_header.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:13:11.353951 promg-1.0.8/src/promg/database_managers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-29 10:13:04.000000 promg-1.0.8/src/promg/database_managers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      555 2024-02-29 10:13:04.000000 promg-1.0.8/src/promg/database_managers/authentication.py
--rw-r--r--   0 runner    (1001) docker     (127)     4602 2024-02-29 10:13:04.000000 promg-1.0.8/src/promg/database_managers/db_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)      228 2024-02-29 10:13:04.000000 promg-1.0.8/src/promg/database_managers/remote_authentication.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:13:11.353951 promg-1.0.8/src/promg/facades/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-29 10:13:04.000000 promg-1.0.8/src/promg/facades/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6160 2024-02-29 10:13:04.000000 promg-1.0.8/src/promg/facades/oced_pg.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:13:11.357951 promg-1.0.8/src/promg/modules/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-29 10:13:04.000000 promg-1.0.8/src/promg/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9007 2024-02-29 10:13:04.000000 promg-1.0.8/src/promg/modules/data_importer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4413 2024-02-29 10:13:04.000000 promg-1.0.8/src/promg/modules/db_management.py
--rw-r--r--   0 runner    (1001) docker     (127)     8229 2024-02-29 10:13:04.000000 promg-1.0.8/src/promg/modules/ekg_builder_semantic_header.py
--rw-r--r--   0 runner    (1001) docker     (127)     3227 2024-02-29 10:13:04.000000 promg-1.0.8/src/promg/modules/exporter.py
--rw-r--r--   0 runner    (1001) docker     (127)     4718 2024-02-29 10:13:04.000000 promg-1.0.8/src/promg/modules/inference_engine.py
--rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-02-29 10:13:04.000000 promg-1.0.8/src/promg/modules/process_discovery.py
--rw-r--r--   0 runner    (1001) docker     (127)     2409 2024-02-29 10:13:04.000000 promg-1.0.8/src/promg/modules/task_identification.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:13:11.357951 promg-1.0.8/src/promg/utilities/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-29 10:13:04.000000 promg-1.0.8/src/promg/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-02-29 10:13:04.000000 promg-1.0.8/src/promg/utilities/auxiliary_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2088 2024-02-29 10:13:04.000000 promg-1.0.8/src/promg/utilities/configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1039 2024-02-29 10:13:04.000000 promg-1.0.8/src/promg/utilities/context_manager_tqdm.py
--rw-r--r--   0 runner    (1001) docker     (127)     1823 2024-02-29 10:13:04.000000 promg-1.0.8/src/promg/utilities/get_db_size.py
--rw-r--r--   0 runner    (1001) docker     (127)     4036 2024-02-29 10:13:04.000000 promg-1.0.8/src/promg/utilities/performance_handling.py
--rw-r--r--   0 runner    (1001) docker     (127)      387 2024-02-29 10:13:04.000000 promg-1.0.8/src/promg/utilities/singleton.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:13:11.357951 promg-1.0.8/src/promg.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-02-29 10:13:11.000000 promg-1.0.8/src/promg.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-02-29 10:13:11.000000 promg-1.0.8/src/promg.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-29 10:13:11.000000 promg-1.0.8/src/promg.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-02-29 10:13:11.000000 promg-1.0.8/src/promg.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-02-29 10:13:11.000000 promg-1.0.8/src/promg.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 09:04:17.008238 promg-1.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     7652 2024-03-04 09:04:11.000000 promg-1.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-03-04 09:04:17.008238 promg-1.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      955 2024-03-04 09:04:11.000000 promg-1.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-04 09:04:17.008238 promg-1.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-03-04 09:04:11.000000 promg-1.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 09:04:17.000238 promg-1.0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 09:04:17.000238 promg-1.0.9/src/promg/
+-rw-r--r--   0 runner    (1001) docker     (127)      630 2024-03-04 09:04:11.000000 promg-1.0.9/src/promg/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 09:04:17.004238 promg-1.0.9/src/promg/cypher_queries/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-04 09:04:11.000000 promg-1.0.9/src/promg/cypher_queries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11395 2024-03-04 09:04:11.000000 promg-1.0.9/src/promg/cypher_queries/data_importer_ql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7218 2024-03-04 09:04:11.000000 promg-1.0.9/src/promg/cypher_queries/db_managment_ql.py
+-rw-r--r--   0 runner    (1001) docker     (127)      922 2024-03-04 09:04:11.000000 promg-1.0.9/src/promg/cypher_queries/exporter_ql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5722 2024-03-04 09:04:11.000000 promg-1.0.9/src/promg/cypher_queries/inference_engine_ql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3660 2024-03-04 09:04:11.000000 promg-1.0.9/src/promg/cypher_queries/process_discovery_ql.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22790 2024-03-04 09:04:11.000000 promg-1.0.9/src/promg/cypher_queries/semantic_header_ql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9542 2024-03-04 09:04:11.000000 promg-1.0.9/src/promg/cypher_queries/task_identification_ql.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 09:04:17.004238 promg-1.0.9/src/promg/data_managers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-04 09:04:11.000000 promg-1.0.9/src/promg/data_managers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31712 2024-03-04 09:04:11.000000 promg-1.0.9/src/promg/data_managers/datastructures.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46016 2024-03-04 09:04:11.000000 promg-1.0.9/src/promg/data_managers/semantic_header.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 09:04:17.004238 promg-1.0.9/src/promg/database_managers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-04 09:04:11.000000 promg-1.0.9/src/promg/database_managers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      555 2024-03-04 09:04:11.000000 promg-1.0.9/src/promg/database_managers/authentication.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4602 2024-03-04 09:04:11.000000 promg-1.0.9/src/promg/database_managers/db_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-03-04 09:04:11.000000 promg-1.0.9/src/promg/database_managers/remote_authentication.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 09:04:17.004238 promg-1.0.9/src/promg/facades/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-04 09:04:11.000000 promg-1.0.9/src/promg/facades/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6160 2024-03-04 09:04:11.000000 promg-1.0.9/src/promg/facades/oced_pg.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 09:04:17.004238 promg-1.0.9/src/promg/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-04 09:04:11.000000 promg-1.0.9/src/promg/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9007 2024-03-04 09:04:11.000000 promg-1.0.9/src/promg/modules/data_importer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4413 2024-03-04 09:04:11.000000 promg-1.0.9/src/promg/modules/db_management.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8229 2024-03-04 09:04:11.000000 promg-1.0.9/src/promg/modules/ekg_builder_semantic_header.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3227 2024-03-04 09:04:11.000000 promg-1.0.9/src/promg/modules/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4718 2024-03-04 09:04:11.000000 promg-1.0.9/src/promg/modules/inference_engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-03-04 09:04:11.000000 promg-1.0.9/src/promg/modules/process_discovery.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2409 2024-03-04 09:04:11.000000 promg-1.0.9/src/promg/modules/task_identification.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 09:04:17.008238 promg-1.0.9/src/promg/utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-04 09:04:11.000000 promg-1.0.9/src/promg/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-03-04 09:04:11.000000 promg-1.0.9/src/promg/utilities/auxiliary_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2088 2024-03-04 09:04:11.000000 promg-1.0.9/src/promg/utilities/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1039 2024-03-04 09:04:11.000000 promg-1.0.9/src/promg/utilities/context_manager_tqdm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1823 2024-03-04 09:04:11.000000 promg-1.0.9/src/promg/utilities/get_db_size.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4036 2024-03-04 09:04:11.000000 promg-1.0.9/src/promg/utilities/performance_handling.py
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-03-04 09:04:11.000000 promg-1.0.9/src/promg/utilities/singleton.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 09:04:17.008238 promg-1.0.9/src/promg.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-03-04 09:04:16.000000 promg-1.0.9/src/promg.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-03-04 09:04:16.000000 promg-1.0.9/src/promg.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-04 09:04:16.000000 promg-1.0.9/src/promg.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-03-04 09:04:16.000000 promg-1.0.9/src/promg.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-03-04 09:04:16.000000 promg-1.0.9/src/promg.egg-info/top_level.txt
```

### Comparing `promg-1.0.8/LICENSE` & `promg-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `promg-1.0.8/PKG-INFO` & `promg-1.0.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: promg
-Version: 1.0.8
+Version: 1.0.9
 Summary: Pyhton library to build Event Knowledge Graphs
 Author: A. Swevels, D.Fahland
 License: GPL 3.0
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: neo4j
```

### Comparing `promg-1.0.8/README.md` & `promg-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `promg-1.0.8/setup.py` & `promg-1.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `promg-1.0.8/src/promg/__init__.py` & `promg-1.0.9/src/promg/__init__.py`

 * *Files identical despite different names*

### Comparing `promg-1.0.8/src/promg/cypher_queries/data_importer_ql.py` & `promg-1.0.9/src/promg/cypher_queries/data_importer_ql.py`

 * *Files identical despite different names*

### Comparing `promg-1.0.8/src/promg/cypher_queries/db_managment_ql.py` & `promg-1.0.9/src/promg/cypher_queries/db_managment_ql.py`

 * *Files identical despite different names*

### Comparing `promg-1.0.8/src/promg/cypher_queries/exporter_ql.py` & `promg-1.0.9/src/promg/cypher_queries/exporter_ql.py`

 * *Files identical despite different names*

### Comparing `promg-1.0.8/src/promg/cypher_queries/inference_engine_ql.py` & `promg-1.0.9/src/promg/cypher_queries/inference_engine_ql.py`

 * *Files identical despite different names*

### Comparing `promg-1.0.8/src/promg/cypher_queries/process_discovery_ql.py` & `promg-1.0.9/src/promg/cypher_queries/process_discovery_ql.py`

 * *Files identical despite different names*

### Comparing `promg-1.0.8/src/promg/cypher_queries/semantic_header_ql.py` & `promg-1.0.9/src/promg/cypher_queries/semantic_header_ql.py`

 * *Files identical despite different names*

### Comparing `promg-1.0.8/src/promg/cypher_queries/task_identification_ql.py` & `promg-1.0.9/src/promg/cypher_queries/task_identification_ql.py`

 * *Files identical despite different names*

### Comparing `promg-1.0.8/src/promg/data_managers/datastructures.py` & `promg-1.0.9/src/promg/data_managers/datastructures.py`

 * *Files identical despite different names*

### Comparing `promg-1.0.8/src/promg/data_managers/semantic_header.py` & `promg-1.0.9/src/promg/data_managers/semantic_header.py`

 * *Files 10% similar despite different names*

```diff
@@ -251,38 +251,41 @@
                             from_node=_from_node, to_node=_to_node, properties=[], where_condition="",
                             has_direction=_has_direction)
 
     @staticmethod
     def from_dict(obj: Any) -> Optional["Relationship"]:
         return Relationship.from_string(obj)
 
-    def get_pattern(self, name: Optional[str] = None, exclude_nodes=True, with_brackets=False):
+    def get_pattern(self, name: Optional[str] = None, exclude_nodes=True, with_properties=True, with_brackets=False):
+        # First, make pattern consisting of rel_name:rel_type (if defined)
         rel_pattern_str = "$rel_name"
         if self.get_relation_type() != "":
             rel_pattern_str = "$rel_name:$rel_type"
 
         name = name if name is not None else self.relation_name
         rel_pattern = Template(rel_pattern_str).substitute(rel_name=name,
                                                            rel_type=self.get_relation_type())
 
-        if len(self.properties) > 0:
+        # add properties if requested and there are properties defined
+        if with_properties and len(self.properties) > 0:
             properties_string = ",".join([prop.get_pattern() for prop in self.properties])
             rel_pattern_str = "$rel_pattern {$properties}"
             rel_pattern = Template(rel_pattern_str).substitute(rel_pattern=rel_pattern,
                                                                properties=properties_string)
-        elif self.where_condition != "":
+        # add where condition if requested and where condition is defined
+        elif with_properties and self.where_condition != "":
             rel_pattern_str = "$rel_pattern WHERE $where_condition"
             rel_pattern = Template(rel_pattern_str).substitute(rel_pattern=rel_pattern,
                                                                where_condition=self.where_condition)
-
+        # don't add from and to nodes if they should be excluded
         if exclude_nodes:
-            if with_brackets:
+            if with_brackets: # add brackets
                 rel_pattern_str = "[$rel_pattern]"
                 rel_pattern = Template(rel_pattern_str).substitute(rel_pattern=rel_pattern)
-        else:
+        else: # add from and to nodes (brackets are always added)
             from_node_pattern = self.from_node.get_pattern()
             to_node_pattern = self.to_node.get_pattern()
             rel_pattern_str = "($from_node) - [$rel_pattern] -> ($to_node)" if self.has_direction \
                 else "($from_node) - [$rel_pattern] - ($to_node)"
             rel_pattern = Template(rel_pattern_str).substitute(from_node=from_node_pattern,
                                                                to_node=to_node_pattern,
                                                                rel_pattern=rel_pattern)
@@ -423,27 +426,34 @@
         return ":".join(self.record_labels)
 
 
 class NodeConstructor:
     def __init__(self, prevalent_record: Optional[Union["Relationship", "Node"]],
                  node: Optional["Node"],
                  relation: Optional["Relationship"],
+                 use_inference: bool,
                  result: "Node",
                  set_labels: str,
                  infer_observed: bool = False,
                  infer_corr_from_event_record: bool = False,
                  infer_corr_from_entity_record: bool = False,
                  infer_corr_from_reified_parents: bool = False,
                  inferred_relationships: List[InferredRelationship] = None,
                  event_label: str = "Event",
                  corr_type: str = "CORR",
                  infer_reified_relation: bool = False):
+        # node can be constructed using several methods
+        # 1) via a prevalent record
         self.prevalent_record = prevalent_record
+        # 2) via a relation
         self.relation = relation
+        # 3) via a node
         self.node = node
+        # 4) via inference, custom code provided by user
+        self.use_inference = use_inference
         self.result = result
         self.set_labels = set_labels
         self.infer_prevalence_record = prevalent_record is not None
         self.infer_observed = infer_observed
         self.infer_corr_from_event_record = infer_corr_from_event_record
         self.infer_corr_from_entity_record = infer_corr_from_entity_record
         self.infer_corr_from_reified_parents = infer_corr_from_reified_parents
@@ -453,14 +463,15 @@
         self.infer_reified_relation = infer_reified_relation
 
     @staticmethod
     def from_dict(obj: Any) -> "NodeConstructor":
         _prevalent_record = RelationshipOrNode.from_string(obj.get("prevalent_record"))
         _node = Relationship.from_string(obj.get("node"))
         _relation = Relationship.from_string(obj.get("relation"))
+        _use_inference = replace_undefined_value(obj.get("use_inference"), False)
         _result = Node.from_string(obj.get("result"))
         _set_labels = obj.get("set_labels")
         _infer_observed = replace_undefined_value(obj.get("infer_observed"), False)
         _infer_corr_from_event_record = replace_undefined_value(obj.get("infer_corr_from_event_record"), False)
         _infer_corr_from_entity_record = replace_undefined_value(obj.get("infer_corr_from_entity_record"), False)
         _infer_corr_from_reified_parents = replace_undefined_value(obj.get("infer_corr_from_reified_parents"), False)
         _corr_type = replace_undefined_value(obj.get("corr_type"), "CORR")
@@ -468,14 +479,15 @@
         _infer_reified_relation = replace_undefined_value(obj.get("infer_reified_relation"), False)
 
         _inferred_relations = create_list(InferredRelationship, obj.get("inferred_relationships"))
 
         return NodeConstructor(prevalent_record=_prevalent_record,
                                relation=_relation,
                                node=_node,
+                               use_inference=_use_inference,
                                result=_result,
                                infer_observed=_infer_observed,
                                infer_corr_from_event_record=_infer_corr_from_event_record,
                                infer_corr_from_entity_record=_infer_corr_from_entity_record,
                                infer_corr_from_reified_parents=_infer_corr_from_reified_parents,
                                inferred_relationships=_inferred_relations,
                                corr_type=_corr_type,
@@ -486,14 +498,16 @@
     def __name__(self):
         if self.prevalent_record is not None:
             return "constructed_by_record"
         elif self.node is not None:
             return "constructed_by_node"
         elif self.relation is not None:
             return "constructed_by_relation"
+        elif self.use_inference:
+            return "constructed_by_inference"
 
     def get_label_string(self):
         return self.result.get_label_str()
 
     def get_labels(self, as_str=True):
         if as_str:
             return ",".join([f'"{label}"' for label in self.result.labels])
@@ -519,15 +533,15 @@
             if include_start_and:
                 return f"AND {condition_str}"
             else:
                 return condition_str
         return condition_str
 
     def get_pattern(self, name: Optional[str] = None, with_brackets=False, with_properties=True):
-        return self.result.get_pattern(name, with_brackets, with_properties)
+        return self.result.get_pattern(name, with_brackets=with_brackets, with_properties=with_properties)
 
     def __repr__(self):
         return self.result.get_pattern(with_brackets=True)
 
     def constructed_by_record(self):
         return self.prevalent_record is not None
 
@@ -622,51 +636,62 @@
             return f'DF_A'
 
 
 class RelationConstructor:
     def __init__(self, prevalent_record: Optional[Union["Relationship", "Node"]],
                  nodes: List["Node"],
                  relations: List["Relationship"],
+                 use_inference: bool,
                  from_node: "Node",
                  to_node: "Node",
                  result: "Relationship",
                  optional_properties: List[Property],
                  model_as_node: bool,
                  infer_corr_from_reified_parents: bool,
                  corr_type: str):
+        # relations can be constructed using several methods
+        # 1) via a prevalent record
         self.prevalent_record = prevalent_record
-        self.from_node = from_node
-        self.to_node = to_node
+        # 2) via another relations
         self.relations = relations
+        # 3) via other nodes
         self.nodes = nodes
+        # 4) via inference, custom code provided by user
+        self.use_inference = use_inference
+
+        self.from_node = from_node
+        self.to_node = to_node
         self.result = result
         self.optional_properties = optional_properties
         self.model_as_node = model_as_node
         self.infer_corr_from_reified_parents = infer_corr_from_reified_parents
         self.corr_type = corr_type
 
     @staticmethod
     def from_dict(obj: Any, model_as_node: bool) -> "RelationConstructor":
         _prevalent_record = RelationshipOrNode.from_string(obj.get("prevalent_record"))
         _nodes = create_list(Node, obj.get("nodes"))
         _relations = create_list(Relationship, obj.get("relations"))
+        _use_inference = replace_undefined_value(obj.get("use_inference"), False)
+
         _from_node = Node.from_string(obj.get("from_node"))
         _to_node = Node.from_string(obj.get("to_node"))
         _result = Relationship.from_string(obj.get("result"))
         _optional_properties = obj.get("set_optional_properties")
         if _optional_properties is not None:
             _optional_properties = _optional_properties.split(",")
             _optional_properties = [Property.from_string(prop) for prop in _optional_properties]
 
         _infer_corr_from_reified_parents = replace_undefined_value(obj.get("infer_corr_from_reified_parents"), False)
         _corr_type = replace_undefined_value(obj.get("corr_type"), "CORR")
 
         return RelationConstructor(prevalent_record=_prevalent_record,
                                    relations=_relations,
                                    nodes=_nodes,
+                                   use_inference=_use_inference,
                                    from_node=_from_node,
                                    to_node=_to_node,
                                    result=_result,
                                    optional_properties=_optional_properties,
                                    model_as_node=model_as_node,
                                    infer_corr_from_reified_parents=_infer_corr_from_reified_parents,
                                    corr_type=_corr_type)
@@ -674,14 +699,16 @@
     def __name__(self):
         if self.prevalent_record is not None:
             return "constructed_by_record"
         elif self.nodes is not None:
             return "constructed_by_nodes"
         elif self.relations is not None:
             return "constructed_by_relations"
+        elif self.use_inference:
+            return "constructed_by_inference"
 
     def get_type(self):
         return self.result.get_relation_type()
 
     def get_prevalent_record_pattern(self, node_name: str):
         return self.prevalent_record.get_pattern(node_name)
 
@@ -693,28 +720,44 @@
         return keys
 
     def get_where_condition(self, node_name: str = "record"):
         return " AND ".join(
             [f'''{node_name}.{key} IS NOT NULL AND {node_name}.{key} <> "Unknown"''' for key
              in self.get_keys()])
 
-    def get_pattern(self, name: Optional[str] = None, with_brackets=False, with_properties=True):
-        return self.result.get_pattern(name, with_brackets, with_properties)
+    def get_pattern(self, name: Optional[str] = None, with_brackets=False, with_properties=True, exclude_nodes=False):
+        return self.result.get_pattern(name=name, with_brackets=with_brackets, with_properties=with_properties,
+                                       exclude_nodes=exclude_nodes)
 
     def __repr__(self):
         return self.result.get_pattern(with_brackets=False, exclude_nodes=False)
 
-    def constructed_by_record(self):
-        return self.prevalent_record is not None
-
-    def constructed_by_nodes(self):
-        return len(self.nodes) > 0
-
-    def constructed_by_relations(self):
-        return len(self.relations) > 0
+    def constructed_by_record(self, modeled_as_nodes):
+        # A = self.prevalent_record is not None
+        # B = modeled_as_node -> self.model_as_node == not modeled_as_node OR self.model_as_node
+        # C = A AND B == len(self.relations) > 0 AND (not modeled_as_node OR self.model_as_node)
+        return (self.prevalent_record is not None) and (not modeled_as_nodes or self.model_as_node)
+
+    def constructed_by_nodes(self, modeled_as_nodes):
+        # A = len(self.nodes) > 0
+        # B = modeled_as_node -> self.model_as_node == not modeled_as_node OR self.model_as_node
+        # C = A AND B == len(self.relations) > 0 AND (not modeled_as_node OR self.model_as_node)
+        return (len(self.nodes) > 0) and (not modeled_as_nodes or self.model_as_node)
+
+    def constructed_by_relations(self, modeled_as_nodes):
+        # A = len(self.relations) > 0
+        # B = modeled_as_node -> self.model_as_node == not modeled_as_node OR self.model_as_node
+        # C = A AND B == len(self.relations) > 0 AND (not modeled_as_node OR self.model_as_node)
+        return (len(self.relations) > 0) and (not modeled_as_nodes or self.model_as_node)
+
+    def constructed_by_inference(self, modeled_as_nodes):
+        # A = self.use_inference
+        # B = modeled_as_node -> self.model_as_node == not modeled_as_node OR self.model_as_node
+        # C = A AND B == self.use_inference AND (not modeled_as_node OR self.model_as_node)
+        return self.use_inference and (not modeled_as_nodes or self.model_as_node)
 
     def get_set_result_properties_query(self):
         if self.optional_properties is None:
             return None
         return ",".join([prop.get_pattern(is_set=True) for prop in self.optional_properties])
 
     def get_relations_query(self):
@@ -934,39 +977,60 @@
                         node_constructors[node.type].append(node_constructor)
         return node_constructors
 
     def get_entities_constructed_by_query(self):
         return [entity for entity in self.nodes if
                 entity.constructor_type == "EntityConstructorByQuery"]
 
-    def get_relations_constructed_by_nodes(self, rel_types: Optional[List[str]]):
-        return self._get_relations_constructed_by_specific_constructor(rel_types, constructor="nodes")
-
-    def get_relations_constructed_by_relations(self, rel_types: Optional[List[str]]):
-        return self._get_relations_constructed_by_specific_constructor(rel_types, constructor="relations")
+    def get_node_relation_constructors(self, rel_types: Optional[List[str]] = None):
+        # get relations that are modeled as nodes
+        rel_constructors = []
+        # check for all diferent methods
+        rel_constructors.extend(self.get_relations_constructed_by_nodes(rel_types, modeled_as_nodes=True))
+        rel_constructors.extend(self.get_relations_constructed_by_relations(rel_types, modeled_as_nodes=True))
+        rel_constructors.extend(self.get_relations_constructed_by_record(rel_types, modeled_as_nodes=True))
+        rel_constructors.extend(self.get_relations_constructed_by_inference(rel_types, modeled_as_nodes=True))
+        return rel_constructors
 
-    def get_relations_constructed_by_record(self, rel_types: Optional[List[str]]):
-        return self._get_relations_constructed_by_specific_constructor(rel_types, constructor="record")
+    def get_relations_constructed_by_nodes(self, rel_types: Optional[List[str]], modeled_as_nodes=False):
+        return self._get_relations_constructed_by_specific_constructor(rel_types, constructor="nodes",
+                                                                       modeled_as_nodes=modeled_as_nodes)
+
+    def get_relations_constructed_by_relations(self, rel_types: Optional[List[str]], modeled_as_nodes=False):
+        return self._get_relations_constructed_by_specific_constructor(rel_types, constructor="relations",
+                                                                       modeled_as_nodes=modeled_as_nodes)
+
+    def get_relations_constructed_by_record(self, rel_types: Optional[List[str]], modeled_as_nodes=False):
+        return self._get_relations_constructed_by_specific_constructor(rel_types, constructor="record",
+                                                                       modeled_as_nodes=modeled_as_nodes)
+
+    def get_relations_constructed_by_inference(self, rel_types: Optional[List[str]], modeled_as_nodes=False):
+        return self._get_relations_constructed_by_specific_constructor(rel_types, constructor="inference",
+                                                                       modeled_as_nodes=modeled_as_nodes)
 
-    def _get_relations_constructed_by_specific_constructor(self, rel_types, constructor):
+    def _get_relations_constructed_by_specific_constructor(self, rel_types, constructor, modeled_as_nodes):
         rel_constructors = []
         for relation in self.relations:
             if rel_types is None or relation.type in rel_types:
                 if constructor == "nodes":
                     rel_constructors.extend(
                         [rel_constructor for rel_constructor in relation.relation_constructors if
-                         rel_constructor.constructed_by_nodes()])
+                         rel_constructor.constructed_by_nodes(modeled_as_nodes)])
                 elif constructor == "relations":
                     rel_constructors.extend(
                         [rel_constructor for rel_constructor in relation.relation_constructors if
-                         rel_constructor.constructed_by_relations()])
+                         rel_constructor.constructed_by_relations(modeled_as_nodes)])
                 elif constructor == "record":
                     rel_constructors.extend(
                         [rel_constructor for rel_constructor in relation.relation_constructors if
-                         rel_constructor.constructed_by_record()])
+                         rel_constructor.constructed_by_record(modeled_as_nodes)])
+                elif constructor == "inference":
+                    rel_constructors.extend(
+                        [rel_constructor for rel_constructor in relation.relation_constructors if
+                         rel_constructor.constructed_by_inference(modeled_as_nodes)])
         return rel_constructors
 
     def get_relations_derived_from_relations(self):
         return [relation for relation in self.relations if
                 "RelationConstructorByRelations" in relation.constructor_type]
 
     def get_relations_derived_from_query(self):
```

### Comparing `promg-1.0.8/src/promg/database_managers/authentication.py` & `promg-1.0.9/src/promg/database_managers/authentication.py`

 * *Files identical despite different names*

### Comparing `promg-1.0.8/src/promg/database_managers/db_connection.py` & `promg-1.0.9/src/promg/database_managers/db_connection.py`

 * *Files identical despite different names*

### Comparing `promg-1.0.8/src/promg/facades/oced_pg.py` & `promg-1.0.9/src/promg/facades/oced_pg.py`

 * *Files identical despite different names*

### Comparing `promg-1.0.8/src/promg/modules/data_importer.py` & `promg-1.0.9/src/promg/modules/data_importer.py`

 * *Files identical despite different names*

### Comparing `promg-1.0.8/src/promg/modules/db_management.py` & `promg-1.0.9/src/promg/modules/db_management.py`

 * *Files identical despite different names*

### Comparing `promg-1.0.8/src/promg/modules/ekg_builder_semantic_header.py` & `promg-1.0.9/src/promg/modules/ekg_builder_semantic_header.py`

 * *Files identical despite different names*

### Comparing `promg-1.0.8/src/promg/modules/exporter.py` & `promg-1.0.9/src/promg/modules/exporter.py`

 * *Files identical despite different names*

### Comparing `promg-1.0.8/src/promg/modules/inference_engine.py` & `promg-1.0.9/src/promg/modules/inference_engine.py`

 * *Files identical despite different names*

### Comparing `promg-1.0.8/src/promg/modules/process_discovery.py` & `promg-1.0.9/src/promg/modules/process_discovery.py`

 * *Files identical despite different names*

### Comparing `promg-1.0.8/src/promg/modules/task_identification.py` & `promg-1.0.9/src/promg/modules/task_identification.py`

 * *Files identical despite different names*

### Comparing `promg-1.0.8/src/promg/utilities/auxiliary_functions.py` & `promg-1.0.9/src/promg/utilities/auxiliary_functions.py`

 * *Files identical despite different names*

### Comparing `promg-1.0.8/src/promg/utilities/configuration.py` & `promg-1.0.9/src/promg/utilities/configuration.py`

 * *Files identical despite different names*

### Comparing `promg-1.0.8/src/promg/utilities/context_manager_tqdm.py` & `promg-1.0.9/src/promg/utilities/context_manager_tqdm.py`

 * *Files identical despite different names*

### Comparing `promg-1.0.8/src/promg/utilities/get_db_size.py` & `promg-1.0.9/src/promg/utilities/get_db_size.py`

 * *Files identical despite different names*

### Comparing `promg-1.0.8/src/promg/utilities/performance_handling.py` & `promg-1.0.9/src/promg/utilities/performance_handling.py`

 * *Files identical despite different names*

### Comparing `promg-1.0.8/src/promg.egg-info/PKG-INFO` & `promg-1.0.9/src/promg.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: promg
-Version: 1.0.8
+Version: 1.0.9
 Summary: Pyhton library to build Event Knowledge Graphs
 Author: A. Swevels, D.Fahland
 License: GPL 3.0
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: neo4j
```

### Comparing `promg-1.0.8/src/promg.egg-info/SOURCES.txt` & `promg-1.0.9/src/promg.egg-info/SOURCES.txt`

 * *Files identical despite different names*

