# Comparing `tmp/wayfarer-0.9.5.tar.gz` & `tmp/wayfarer-0.9.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wayfarer-0.9.5.tar", last modified: Tue Sep 19 13:24:30 2023, max compression
+gzip compressed data, was "wayfarer-0.9.6.tar", last modified: Tue Dec 12 13:54:17 2023, max compression
```

## Comparing `wayfarer-0.9.5.tar` & `wayfarer-0.9.6.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-19 13:24:30.295931 wayfarer-0.9.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2023-09-19 13:22:38.000000 wayfarer-0.9.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5663 2023-09-19 13:24:30.291931 wayfarer-0.9.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5165 2023-09-19 13:22:38.000000 wayfarer-0.9.5/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-09-19 13:24:30.295931 wayfarer-0.9.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1012 2023-09-19 13:22:39.000000 wayfarer-0.9.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-19 13:24:30.287931 wayfarer-0.9.5/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    14527 2023-09-19 13:22:39.000000 wayfarer-0.9.5/tests/test_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)    14248 2023-09-19 13:22:39.000000 wayfarer-0.9.5/tests/test_linearref.py
--rw-r--r--   0 runner    (1001) docker     (127)     6449 2023-09-19 13:22:39.000000 wayfarer-0.9.5/tests/test_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)     1440 2023-09-19 13:22:39.000000 wayfarer-0.9.5/tests/test_loops.py
--rw-r--r--   0 runner    (1001) docker     (127)     1347 2023-09-19 13:22:39.000000 wayfarer-0.9.5/tests/test_osmnx_compat.py
--rw-r--r--   0 runner    (1001) docker     (127)     3607 2023-09-19 13:22:39.000000 wayfarer-0.9.5/tests/test_routing.py
--rw-r--r--   0 runner    (1001) docker     (127)    13542 2023-09-19 13:22:39.000000 wayfarer-0.9.5/tests/test_routing_ordered_path.py
--rw-r--r--   0 runner    (1001) docker     (127)     8836 2023-09-19 13:22:39.000000 wayfarer-0.9.5/tests/test_splitting.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-19 13:24:30.291931 wayfarer-0.9.5/wayfarer/
--rw-r--r--   0 runner    (1001) docker     (127)     2006 2023-09-19 13:22:39.000000 wayfarer-0.9.5/wayfarer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18851 2023-09-19 13:22:39.000000 wayfarer-0.9.5/wayfarer/functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3038 2023-09-19 13:22:39.000000 wayfarer-0.9.5/wayfarer/io.py
--rw-r--r--   0 runner    (1001) docker     (127)    16368 2023-09-19 13:22:39.000000 wayfarer-0.9.5/wayfarer/linearref.py
--rw-r--r--   0 runner    (1001) docker     (127)    10519 2023-09-19 13:22:39.000000 wayfarer-0.9.5/wayfarer/loader.py
--rw-r--r--   0 runner    (1001) docker     (127)     3086 2023-09-19 13:22:39.000000 wayfarer-0.9.5/wayfarer/loops.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-19 13:22:39.000000 wayfarer-0.9.5/wayfarer/merger.py
--rw-r--r--   0 runner    (1001) docker     (127)     2632 2023-09-19 13:22:39.000000 wayfarer-0.9.5/wayfarer/osmnx_compat.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-19 13:22:39.000000 wayfarer-0.9.5/wayfarer/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    13790 2023-09-19 13:22:39.000000 wayfarer-0.9.5/wayfarer/routing.py
--rw-r--r--   0 runner    (1001) docker     (127)    11765 2023-09-19 13:22:39.000000 wayfarer-0.9.5/wayfarer/splitter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1718 2023-09-19 13:22:39.000000 wayfarer-0.9.5/wayfarer/validator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-19 13:24:30.291931 wayfarer-0.9.5/wayfarer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5663 2023-09-19 13:24:30.000000 wayfarer-0.9.5/wayfarer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      656 2023-09-19 13:24:30.000000 wayfarer-0.9.5/wayfarer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-19 13:24:30.000000 wayfarer-0.9.5/wayfarer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-19 13:23:09.000000 wayfarer-0.9.5/wayfarer.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       22 2023-09-19 13:24:30.000000 wayfarer-0.9.5/wayfarer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2023-09-19 13:24:30.000000 wayfarer-0.9.5/wayfarer.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-12 13:54:17.831032 wayfarer-0.9.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2023-12-12 13:53:13.000000 wayfarer-0.9.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5663 2023-12-12 13:54:17.831032 wayfarer-0.9.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5165 2023-12-12 13:53:13.000000 wayfarer-0.9.6/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-12 13:54:17.831032 wayfarer-0.9.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1012 2023-12-12 13:53:13.000000 wayfarer-0.9.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-12 13:54:17.827032 wayfarer-0.9.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    15071 2023-12-12 13:53:13.000000 wayfarer-0.9.6/tests/test_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14248 2023-12-12 13:53:13.000000 wayfarer-0.9.6/tests/test_linearref.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6449 2023-12-12 13:53:13.000000 wayfarer-0.9.6/tests/test_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1440 2023-12-12 13:53:13.000000 wayfarer-0.9.6/tests/test_loops.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1347 2023-12-12 13:53:13.000000 wayfarer-0.9.6/tests/test_osmnx_compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3607 2023-12-12 13:53:13.000000 wayfarer-0.9.6/tests/test_routing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13542 2023-12-12 13:53:13.000000 wayfarer-0.9.6/tests/test_routing_ordered_path.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8836 2023-12-12 13:53:13.000000 wayfarer-0.9.6/tests/test_splitting.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-12 13:54:17.827032 wayfarer-0.9.6/wayfarer/
+-rw-r--r--   0 runner    (1001) docker     (127)     2006 2023-12-12 13:53:13.000000 wayfarer-0.9.6/wayfarer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19715 2023-12-12 13:53:13.000000 wayfarer-0.9.6/wayfarer/functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3038 2023-12-12 13:53:13.000000 wayfarer-0.9.6/wayfarer/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16368 2023-12-12 13:53:13.000000 wayfarer-0.9.6/wayfarer/linearref.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10519 2023-12-12 13:53:13.000000 wayfarer-0.9.6/wayfarer/loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3086 2023-12-12 13:53:13.000000 wayfarer-0.9.6/wayfarer/loops.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-12 13:53:13.000000 wayfarer-0.9.6/wayfarer/merger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2632 2023-12-12 13:53:13.000000 wayfarer-0.9.6/wayfarer/osmnx_compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-12 13:53:13.000000 wayfarer-0.9.6/wayfarer/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    13790 2023-12-12 13:53:13.000000 wayfarer-0.9.6/wayfarer/routing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11765 2023-12-12 13:53:13.000000 wayfarer-0.9.6/wayfarer/splitter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1718 2023-12-12 13:53:13.000000 wayfarer-0.9.6/wayfarer/validator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-12 13:54:17.831032 wayfarer-0.9.6/wayfarer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5663 2023-12-12 13:54:17.000000 wayfarer-0.9.6/wayfarer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      656 2023-12-12 13:54:17.000000 wayfarer-0.9.6/wayfarer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-12 13:54:17.000000 wayfarer-0.9.6/wayfarer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-12 13:53:30.000000 wayfarer-0.9.6/wayfarer.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2023-12-12 13:54:17.000000 wayfarer-0.9.6/wayfarer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2023-12-12 13:54:17.000000 wayfarer-0.9.6/wayfarer.egg-info/top_level.txt
```

### Comparing `wayfarer-0.9.5/LICENSE` & `wayfarer-0.9.6/LICENSE`

 * *Files identical despite different names*

### Comparing `wayfarer-0.9.5/PKG-INFO` & `wayfarer-0.9.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wayfarer
-Version: 0.9.5
+Version: 0.9.6
 Summary: A library to add spatial functions to networkx
 Home-page: https://github.com/compassinformatics/wayfarer/
 Author: Seth Girvin
 Author-email: sgirvin@compass.ie
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `wayfarer-0.9.5/README.rst` & `wayfarer-0.9.6/README.rst`

 * *Files identical despite different names*

### Comparing `wayfarer-0.9.5/setup.py` & `wayfarer-0.9.6/setup.py`

 * *Files identical despite different names*

### Comparing `wayfarer-0.9.5/tests/test_functions.py` & `wayfarer-0.9.6/tests/test_functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -311,37 +311,51 @@
         1, 2, key="B", **{"EDGE_ID": "B", "LEN_": 100, "NODEID_FROM": 1, "NODEID_TO": 2}
     )
     net.add_edge(2, 3, key="C", **{"EDGE_ID": "C", "LEN_": 100})
 
     node_list = [1, 2]
     edges = functions.get_edges_from_nodes(net, node_list)
     assert len(edges) == 1
-    edges[0].key == "B"
+    assert edges[0].key == "B"
 
     edges = functions.get_edges_from_nodes(net, [2, 1], with_direction_flag=True)
     assert len(edges) == 1
     assert edges[0].key == "B"
     assert edges[0].attributes[WITH_DIRECTION_FIELD] is False
 
 
 def test_get_edges_from_nodes_non_unique():
     net = networkx.MultiGraph()
 
     net.add_edge(1, 2, key="A", **{"EDGE_ID": "A", "LEN_": 100})
     net.add_edge(1, 2, key="B", **{"EDGE_ID": "B", "LEN_": 100})
 
-    node_list = [1, 2, 1]
+    node_list = [1, 2, 1]  # a loop
     edges = functions.get_edges_from_nodes(net, node_list, return_unique=True)
     assert len(edges) == 1
-    edges[0].key == "B"
+    # as edge A is the "first" key it will be returned
+    assert edges[0].key == "A"
 
     edges = functions.get_edges_from_nodes(net, node_list, return_unique=False)
     assert len(edges) == 2
-    edges[0].key == "B"
-    edges[1].key == "B"
+    assert edges[0].key == "A"
+    assert edges[1].key == "A"
+
+
+def test_get_edges_from_nodes_all_lengths():
+    net = networkx.MultiGraph()
+
+    net.add_edge(1, 2, key="A", **{"EDGE_ID": "A", "LEN_": 50})
+    net.add_edge(1, 2, key="B", **{"EDGE_ID": "B", "LEN_": 100})
+
+    node_list = [1, 2]
+    edges = functions.get_edges_from_nodes(net, node_list, shortest_path_only=False)
+    assert len(edges) == 2
+    assert edges[0].key == "A"
+    assert edges[1].key == "B"
 
 
 def test_edges_to_graph():
     edges = []
     net = functions.edges_to_graph(edges)
     assert len(net.edges()) == 0
 
@@ -475,13 +489,14 @@
     # test_to_edge()
     # test_to_edge_no_attributes()
     # test_edges_to_graph_no_keys()
     # test_get_edge_by_key_missing()
     # test_get_all_paths_from_nodes_with_direction()
     # test_get_path_length()
     # test_doctest()
-    # test_get_edges_from_nodes_non_unique()
+    test_get_edges_from_nodes_non_unique()
     # test_has_no_overlaps()
     # test_has_no_overlaps_loop()
     # test_has_overlaps()
-    test_has_no_overlaps_loop_with_split()
+    # test_has_no_overlaps_loop_with_split()
+    test_get_edges_from_nodes_all_lengths()
     print("Done!")
```

### Comparing `wayfarer-0.9.5/tests/test_linearref.py` & `wayfarer-0.9.6/tests/test_linearref.py`

 * *Files identical despite different names*

### Comparing `wayfarer-0.9.5/tests/test_loader.py` & `wayfarer-0.9.6/tests/test_loader.py`

 * *Files identical despite different names*

### Comparing `wayfarer-0.9.5/tests/test_loops.py` & `wayfarer-0.9.6/tests/test_loops.py`

 * *Files identical despite different names*

### Comparing `wayfarer-0.9.5/tests/test_osmnx_compat.py` & `wayfarer-0.9.6/tests/test_osmnx_compat.py`

 * *Files identical despite different names*

### Comparing `wayfarer-0.9.5/tests/test_routing.py` & `wayfarer-0.9.6/tests/test_routing.py`

 * *Files identical despite different names*

### Comparing `wayfarer-0.9.5/tests/test_routing_ordered_path.py` & `wayfarer-0.9.6/tests/test_routing_ordered_path.py`

 * *Files identical despite different names*

### Comparing `wayfarer-0.9.5/tests/test_splitting.py` & `wayfarer-0.9.6/tests/test_splitting.py`

 * *Files identical despite different names*

### Comparing `wayfarer-0.9.5/wayfarer/__init__.py` & `wayfarer-0.9.6/wayfarer/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import NamedTuple
 
 
-__version__ = "0.9.5"
+__version__ = "0.9.6"
 
 LENGTH_FIELD = "LEN_"
 EDGE_ID_FIELD = "EDGE_ID"
 OFFSET_FIELD = "OFFSET"
 
 NODEID_FROM_FIELD = "NODEID_FROM"
 NODEID_TO_FIELD = "NODEID_TO"
```

### Comparing `wayfarer-0.9.5/wayfarer/functions.py` & `wayfarer-0.9.6/wayfarer/functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -326,35 +326,52 @@
 
 def get_edges_from_nodes(
     net: (networkx.MultiGraph | networkx.MultiDiGraph),
     node_list: list[int | str],
     with_direction_flag: bool = False,
     length_field: str = LENGTH_FIELD,
     return_unique: bool = True,
+    shortest_path_only: bool = True,
 ) -> list[Edge]:
     """
-    From a list of nodes, create pairs and then get the shortest edge between the two nodes
-    Set with_direction_flag to add a new attribute to the edge to show if it is matching the
-    direction of the path
+    From a list of nodes, create pairs and then get all the edges between the two nodes.
+    By default only the shortest edges between the edges will be returned, but setting
+    ``shortest_path_only`` to ``False`` will return all edges ignoring the ``length_field``.
+    Set ``with_direction_flag`` to add a new attribute to the edge to show if it is matching the
+    direction of the path.
+    ``return_unique`` ensures only one copy of each edge is returned in the case of loops
     """
     edge_list = []
 
     node_pairs = pairwise(node_list)
 
     for u, v in node_pairs:
         edges = get_edges_from_node_pair(net, u, v)
+        node_edges = []
         if edges:
-            key, attributes = get_shortest_edge(edges, length_field)
-            atts_copy = copy.deepcopy(attributes)
-            edge = Edge(start_node=u, end_node=v, key=key, attributes=atts_copy)
+            if shortest_path_only:
+                key, attributes = get_shortest_edge(edges, length_field)
+                atts_copy = copy.deepcopy(attributes)
+                edge = Edge(start_node=u, end_node=v, key=key, attributes=atts_copy)
+                node_edges.append(edge)
+            else:
+                # get all edges between the nodes, ignoring the length_field
+                for key, attributes in edges.items():
+                    atts_copy = copy.deepcopy(attributes)
+                    node_edges.append(
+                        Edge(start_node=u, end_node=v, key=key, attributes=atts_copy)
+                    )
 
             if with_direction_flag:
-                add_direction_flag(**edge._asdict())  # unpack namedtuple to **kwargs
+                for edge in node_edges:
+                    add_direction_flag(
+                        **edge._asdict()
+                    )  # unpack namedtuple to **kwargs
 
-            edge_list.append(edge)
+            edge_list += node_edges
 
     if return_unique:
         return list({v.key: v for v in edge_list}.values())
     else:
         return edge_list
 
 
@@ -628,15 +645,14 @@
     sorted_edges = sorted(edges, key=lambda e: e.attributes[EDGE_ID_FIELD])
     grouped_edges = itertools.groupby(
         sorted_edges, key=lambda e: e.attributes[EDGE_ID_FIELD]
     )
 
     for _, edge_group in grouped_edges:
         for edge1, edge2 in itertools.combinations(edge_group, 2):
-
             from_m1 = edge1.attributes.get(OFFSET_FIELD, 0)
             to_m1 = from_m1 + edge1.attributes.get(LENGTH_FIELD, 0)
 
             from_m2 = edge2.attributes.get(OFFSET_FIELD, 0)
             to_m2 = from_m2 + edge2.attributes.get(LENGTH_FIELD, 0)
 
             if max(from_m1, from_m2) < min(to_m1, to_m2):
```

### Comparing `wayfarer-0.9.5/wayfarer/io.py` & `wayfarer-0.9.6/wayfarer/io.py`

 * *Files identical despite different names*

### Comparing `wayfarer-0.9.5/wayfarer/linearref.py` & `wayfarer-0.9.6/wayfarer/linearref.py`

 * *Files identical despite different names*

### Comparing `wayfarer-0.9.5/wayfarer/loader.py` & `wayfarer-0.9.6/wayfarer/loader.py`

 * *Files identical despite different names*

### Comparing `wayfarer-0.9.5/wayfarer/loops.py` & `wayfarer-0.9.6/wayfarer/loops.py`

 * *Files identical despite different names*

### Comparing `wayfarer-0.9.5/wayfarer/osmnx_compat.py` & `wayfarer-0.9.6/wayfarer/osmnx_compat.py`

 * *Files identical despite different names*

### Comparing `wayfarer-0.9.5/wayfarer/routing.py` & `wayfarer-0.9.6/wayfarer/routing.py`

 * *Files identical despite different names*

### Comparing `wayfarer-0.9.5/wayfarer/splitter.py` & `wayfarer-0.9.6/wayfarer/splitter.py`

 * *Files identical despite different names*

### Comparing `wayfarer-0.9.5/wayfarer/validator.py` & `wayfarer-0.9.6/wayfarer/validator.py`

 * *Files identical despite different names*

### Comparing `wayfarer-0.9.5/wayfarer.egg-info/PKG-INFO` & `wayfarer-0.9.6/wayfarer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wayfarer
-Version: 0.9.5
+Version: 0.9.6
 Summary: A library to add spatial functions to networkx
 Home-page: https://github.com/compassinformatics/wayfarer/
 Author: Seth Girvin
 Author-email: sgirvin@compass.ie
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `wayfarer-0.9.5/wayfarer.egg-info/SOURCES.txt` & `wayfarer-0.9.6/wayfarer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

