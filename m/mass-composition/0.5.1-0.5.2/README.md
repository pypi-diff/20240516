# Comparing `tmp/mass_composition-0.5.1.tar.gz` & `tmp/mass_composition-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mass_composition-0.5.1.tar", max compression
+gzip compressed data, was "mass_composition-0.5.2.tar", max compression
```

## Comparing `mass_composition-0.5.1.tar` & `mass_composition-0.5.2.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-r--r--   0        0        0     1069 2024-05-15 12:38:27.334730 mass_composition-0.5.1/LICENSE
--rw-r--r--   0        0        0     3491 2024-05-15 12:38:27.334730 mass_composition-0.5.1/README.md
--rw-r--r--   0        0        0      360 2024-05-15 12:38:27.738731 mass_composition-0.5.1/elphick/mass_composition/__init__.py
--rw-r--r--   0        0        0     9816 2024-05-15 12:38:27.738731 mass_composition-0.5.1/elphick/mass_composition/balance.py
--rw-r--r--   0        0        0       35 2024-05-15 12:38:27.738731 mass_composition-0.5.1/elphick/mass_composition/config/__init__.py
--rw-r--r--   0        0        0      765 2024-05-15 12:38:27.738731 mass_composition-0.5.1/elphick/mass_composition/config/config_read.py
--rw-r--r--   0        0        0      364 2024-05-15 12:38:27.738731 mass_composition-0.5.1/elphick/mass_composition/config/flowsheet_example.yaml
--rw-r--r--   0        0        0      838 2024-05-15 12:38:27.738731 mass_composition-0.5.1/elphick/mass_composition/config/mc_config.yml
--rw-r--r--   0        0        0    13598 2024-05-15 12:38:27.738731 mass_composition-0.5.1/elphick/mass_composition/dag.py
--rw-r--r--   0        0        0       59 2024-05-15 12:38:27.738731 mass_composition-0.5.1/elphick/mass_composition/datasets/__init__.py
--rw-r--r--   0        0        0     1892 2024-05-15 12:38:27.738731 mass_composition-0.5.1/elphick/mass_composition/datasets/datasets.py
--rw-r--r--   0        0        0     1622 2024-05-15 12:38:27.738731 mass_composition-0.5.1/elphick/mass_composition/datasets/downloader.py
--rw-r--r--   0        0        0     3046 2024-05-15 12:38:27.738731 mass_composition-0.5.1/elphick/mass_composition/datasets/register.csv
--rw-r--r--   0        0        0     6565 2024-05-15 12:38:27.738731 mass_composition-0.5.1/elphick/mass_composition/datasets/sample_data.py
--rw-r--r--   0        0        0    41619 2024-05-15 12:38:27.738731 mass_composition-0.5.1/elphick/mass_composition/flowsheet.py
--rw-r--r--   0        0        0     2080 2024-05-15 12:38:27.738731 mass_composition-0.5.1/elphick/mass_composition/layout.py
--rw-r--r--   0        0        0    52834 2024-05-15 12:38:27.738731 mass_composition-0.5.1/elphick/mass_composition/mass_composition.py
--rw-r--r--   0        0        0     4350 2024-05-15 12:38:27.738731 mass_composition-0.5.1/elphick/mass_composition/mc_node.py
--rw-r--r--   0        0        0      908 2024-05-15 12:38:27.738731 mass_composition-0.5.1/elphick/mass_composition/mc_status.py
--rw-r--r--   0        0        0    19410 2024-05-15 12:38:27.738731 mass_composition-0.5.1/elphick/mass_composition/mc_xarray.py
--rw-r--r--   0        0        0     5752 2024-05-15 12:38:27.738731 mass_composition-0.5.1/elphick/mass_composition/plot.py
--rw-r--r--   0        0        0     3357 2024-05-15 12:38:27.738731 mass_composition-0.5.1/elphick/mass_composition/stream.py
--rw-r--r--   0        0        0       42 2024-05-15 12:38:27.738731 mass_composition-0.5.1/elphick/mass_composition/utils/__init__.py
--rw-r--r--   0        0        0      214 2024-05-15 12:38:27.738731 mass_composition-0.5.1/elphick/mass_composition/utils/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     3909 2024-05-15 12:38:27.738731 mass_composition-0.5.1/elphick/mass_composition/utils/__pycache__/components.cpython-39.pyc
--rw-r--r--   0        0        0     2197 2024-05-15 12:38:27.738731 mass_composition-0.5.1/elphick/mass_composition/utils/__pycache__/moisture.cpython-39.pyc
--rw-r--r--   0        0        0     1494 2024-05-15 12:38:27.738731 mass_composition-0.5.1/elphick/mass_composition/utils/__pycache__/viz.cpython-39.pyc
--rw-r--r--   0        0        0     1874 2024-05-15 12:38:27.738731 mass_composition-0.5.1/elphick/mass_composition/utils/amenability.py
--rw-r--r--   0        0        0     2914 2024-05-15 12:38:27.738731 mass_composition-0.5.1/elphick/mass_composition/utils/components.py
--rw-r--r--   0        0        0       80 2024-05-15 12:38:27.738731 mass_composition-0.5.1/elphick/mass_composition/utils/geometry.py
--rw-r--r--   0        0        0     1193 2024-05-15 12:38:27.738731 mass_composition-0.5.1/elphick/mass_composition/utils/hash_utils.py
--rw-r--r--   0        0        0     9591 2024-05-15 12:38:27.738731 mass_composition-0.5.1/elphick/mass_composition/utils/interp.py
--rw-r--r--   0        0        0     4867 2024-05-15 12:38:27.738731 mass_composition-0.5.1/elphick/mass_composition/utils/loader.py
--rw-r--r--   0        0        0     2611 2024-05-15 12:38:27.738731 mass_composition-0.5.1/elphick/mass_composition/utils/moisture.py
--rw-r--r--   0        0        0      842 2024-05-15 12:38:27.738731 mass_composition-0.5.1/elphick/mass_composition/utils/parallel.py
--rw-r--r--   0        0        0     1033 2024-05-15 12:38:27.738731 mass_composition-0.5.1/elphick/mass_composition/utils/partition.py
--rw-r--r--   0        0        0     7955 2024-05-15 12:38:27.738731 mass_composition-0.5.1/elphick/mass_composition/utils/pd_utils.py
--rw-r--r--   0        0        0       61 2024-05-15 12:38:27.738731 mass_composition-0.5.1/elphick/mass_composition/utils/sampling.py
--rw-r--r--   0        0        0     2164 2024-05-15 12:38:27.738731 mass_composition-0.5.1/elphick/mass_composition/utils/size.py
--rw-r--r--   0        0        0     2630 2024-05-15 12:38:27.738731 mass_composition-0.5.1/elphick/mass_composition/utils/size_distribution.py
--rw-r--r--   0        0        0     1717 2024-05-15 12:38:27.738731 mass_composition-0.5.1/elphick/mass_composition/utils/viz.py
--rw-r--r--   0        0        0     8865 2024-05-15 12:38:27.738731 mass_composition-0.5.1/elphick/mass_composition/variables.py
--rw-r--r--   0        0        0     2014 2024-05-15 12:38:27.742732 mass_composition-0.5.1/pyproject.toml
--rw-r--r--   0        0        0     4852 1970-01-01 00:00:00.000000 mass_composition-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-05-15 21:36:56.586194 mass_composition-0.5.2/LICENSE
+-rw-r--r--   0        0        0     3491 2024-05-15 21:36:56.586194 mass_composition-0.5.2/README.md
+-rw-r--r--   0        0        0      360 2024-05-15 21:36:56.998195 mass_composition-0.5.2/elphick/mass_composition/__init__.py
+-rw-r--r--   0        0        0     9816 2024-05-15 21:36:57.002195 mass_composition-0.5.2/elphick/mass_composition/balance.py
+-rw-r--r--   0        0        0       35 2024-05-15 21:36:57.002195 mass_composition-0.5.2/elphick/mass_composition/config/__init__.py
+-rw-r--r--   0        0        0      765 2024-05-15 21:36:57.002195 mass_composition-0.5.2/elphick/mass_composition/config/config_read.py
+-rw-r--r--   0        0        0      364 2024-05-15 21:36:57.002195 mass_composition-0.5.2/elphick/mass_composition/config/flowsheet_example.yaml
+-rw-r--r--   0        0        0      838 2024-05-15 21:36:57.002195 mass_composition-0.5.2/elphick/mass_composition/config/mc_config.yml
+-rw-r--r--   0        0        0    11761 2024-05-15 21:36:57.002195 mass_composition-0.5.2/elphick/mass_composition/dag.py
+-rw-r--r--   0        0        0       59 2024-05-15 21:36:57.002195 mass_composition-0.5.2/elphick/mass_composition/datasets/__init__.py
+-rw-r--r--   0        0        0     1892 2024-05-15 21:36:57.002195 mass_composition-0.5.2/elphick/mass_composition/datasets/datasets.py
+-rw-r--r--   0        0        0     1622 2024-05-15 21:36:57.002195 mass_composition-0.5.2/elphick/mass_composition/datasets/downloader.py
+-rw-r--r--   0        0        0     3046 2024-05-15 21:36:57.002195 mass_composition-0.5.2/elphick/mass_composition/datasets/register.csv
+-rw-r--r--   0        0        0     6565 2024-05-15 21:36:57.002195 mass_composition-0.5.2/elphick/mass_composition/datasets/sample_data.py
+-rw-r--r--   0        0        0    41619 2024-05-15 21:36:57.002195 mass_composition-0.5.2/elphick/mass_composition/flowsheet.py
+-rw-r--r--   0        0        0     2080 2024-05-15 21:36:57.002195 mass_composition-0.5.2/elphick/mass_composition/layout.py
+-rw-r--r--   0        0        0    52834 2024-05-15 21:36:57.002195 mass_composition-0.5.2/elphick/mass_composition/mass_composition.py
+-rw-r--r--   0        0        0     4350 2024-05-15 21:36:57.002195 mass_composition-0.5.2/elphick/mass_composition/mc_node.py
+-rw-r--r--   0        0        0      908 2024-05-15 21:36:57.002195 mass_composition-0.5.2/elphick/mass_composition/mc_status.py
+-rw-r--r--   0        0        0    19410 2024-05-15 21:36:57.002195 mass_composition-0.5.2/elphick/mass_composition/mc_xarray.py
+-rw-r--r--   0        0        0     5752 2024-05-15 21:36:57.002195 mass_composition-0.5.2/elphick/mass_composition/plot.py
+-rw-r--r--   0        0        0     3357 2024-05-15 21:36:57.002195 mass_composition-0.5.2/elphick/mass_composition/stream.py
+-rw-r--r--   0        0        0       42 2024-05-15 21:36:57.002195 mass_composition-0.5.2/elphick/mass_composition/utils/__init__.py
+-rw-r--r--   0        0        0      214 2024-05-15 21:36:57.002195 mass_composition-0.5.2/elphick/mass_composition/utils/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     3909 2024-05-15 21:36:57.002195 mass_composition-0.5.2/elphick/mass_composition/utils/__pycache__/components.cpython-39.pyc
+-rw-r--r--   0        0        0     2197 2024-05-15 21:36:57.002195 mass_composition-0.5.2/elphick/mass_composition/utils/__pycache__/moisture.cpython-39.pyc
+-rw-r--r--   0        0        0     1494 2024-05-15 21:36:57.002195 mass_composition-0.5.2/elphick/mass_composition/utils/__pycache__/viz.cpython-39.pyc
+-rw-r--r--   0        0        0     1874 2024-05-15 21:36:57.002195 mass_composition-0.5.2/elphick/mass_composition/utils/amenability.py
+-rw-r--r--   0        0        0     2914 2024-05-15 21:36:57.002195 mass_composition-0.5.2/elphick/mass_composition/utils/components.py
+-rw-r--r--   0        0        0       80 2024-05-15 21:36:57.002195 mass_composition-0.5.2/elphick/mass_composition/utils/geometry.py
+-rw-r--r--   0        0        0     1193 2024-05-15 21:36:57.002195 mass_composition-0.5.2/elphick/mass_composition/utils/hash_utils.py
+-rw-r--r--   0        0        0     9591 2024-05-15 21:36:57.002195 mass_composition-0.5.2/elphick/mass_composition/utils/interp.py
+-rw-r--r--   0        0        0     4867 2024-05-15 21:36:57.002195 mass_composition-0.5.2/elphick/mass_composition/utils/loader.py
+-rw-r--r--   0        0        0     2611 2024-05-15 21:36:57.002195 mass_composition-0.5.2/elphick/mass_composition/utils/moisture.py
+-rw-r--r--   0        0        0      842 2024-05-15 21:36:57.002195 mass_composition-0.5.2/elphick/mass_composition/utils/parallel.py
+-rw-r--r--   0        0        0     1033 2024-05-15 21:36:57.002195 mass_composition-0.5.2/elphick/mass_composition/utils/partition.py
+-rw-r--r--   0        0        0     7955 2024-05-15 21:36:57.002195 mass_composition-0.5.2/elphick/mass_composition/utils/pd_utils.py
+-rw-r--r--   0        0        0       61 2024-05-15 21:36:57.002195 mass_composition-0.5.2/elphick/mass_composition/utils/sampling.py
+-rw-r--r--   0        0        0     2164 2024-05-15 21:36:57.002195 mass_composition-0.5.2/elphick/mass_composition/utils/size.py
+-rw-r--r--   0        0        0     2630 2024-05-15 21:36:57.002195 mass_composition-0.5.2/elphick/mass_composition/utils/size_distribution.py
+-rw-r--r--   0        0        0     1717 2024-05-15 21:36:57.002195 mass_composition-0.5.2/elphick/mass_composition/utils/viz.py
+-rw-r--r--   0        0        0     8865 2024-05-15 21:36:57.002195 mass_composition-0.5.2/elphick/mass_composition/variables.py
+-rw-r--r--   0        0        0     2014 2024-05-15 21:36:57.006195 mass_composition-0.5.2/pyproject.toml
+-rw-r--r--   0        0        0     4852 1970-01-01 00:00:00.000000 mass_composition-0.5.2/PKG-INFO
```

### Comparing `mass_composition-0.5.1/LICENSE` & `mass_composition-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mass_composition-0.5.1/README.md` & `mass_composition-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `mass_composition-0.5.1/elphick/mass_composition/balance.py` & `mass_composition-0.5.2/elphick/mass_composition/balance.py`

 * *Files identical despite different names*

### Comparing `mass_composition-0.5.1/elphick/mass_composition/config/config_read.py` & `mass_composition-0.5.2/elphick/mass_composition/config/config_read.py`

 * *Files identical despite different names*

### Comparing `mass_composition-0.5.1/elphick/mass_composition/config/mc_config.yml` & `mass_composition-0.5.2/elphick/mass_composition/config/mc_config.yml`

 * *Files identical despite different names*

### Comparing `mass_composition-0.5.1/elphick/mass_composition/dag.py` & `mass_composition-0.5.2/elphick/mass_composition/dag.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import logging
-from typing import List, Callable, Union, Optional, Tuple
+from typing import List, Callable, Union, Tuple
 
 import matplotlib.pyplot as plt
 import networkx as nx
 from joblib import Parallel, delayed
+from tqdm import tqdm
 
 from elphick.mass_composition import Stream, MassComposition
 
 logger = logging.getLogger(__name__)
 
 
 class Node:
@@ -22,43 +23,14 @@
     def __init__(self, name: str = 'DAG', n_jobs=-1):
         self.name = name
         self.stream_parent_node = {}  # Map stream names to node names
         self.n_jobs = n_jobs  # Number of workers for parallel execution
         self.graph = nx.DiGraph()
         self.node_executed = {}  # Store the execution state of nodes
 
-    # @property
-    # def mass_compositions(self) -> dict[str, Stream]:
-    #     """
-    #     Retrieves all the Stream objects associated with the nodes in the DAG.
-    #
-    #     This property iterates over all the nodes in the DAG, checks if the node has been executed,
-    #     and if so, retrieves the result of the node execution. If the node has not been executed,
-    #     it retrieves the Stream object associated with the node in the graph.
-    #
-    #     Returns:
-    #         dict[str, Stream]: A dictionary where the keys are node names and the values
-    #         are Stream objects associated with those nodes.
-    #     """
-    #     mass_compositions = {}
-    #     for node in self.graph.nodes:
-    #         if node in self.node_executed:
-    #             result = self.node_executed[node]
-    #             if isinstance(result, Stream):
-    #                 mass_compositions[node] = result
-    #             elif isinstance(result, tuple) and all(isinstance(r, Stream) for r in result):
-    #                 for r in result:
-    #                     mass_compositions[r.name] = r
-    #         else:
-    #             # If the node is not in the results dictionary, it is a leaf node
-    #             # Retrieve its result from the Stream objects associated with the node in the graph
-    #             mc = self.graph.nodes[node]['mc']
-    #             mass_compositions[node] = mc
-    #     return mass_compositions
-
     @property
     def streams(self):
         """
         Retrieves all the Stream objects associated with the edges in the DAG.
 
         This property iterates over all the edges in the DAG and retrieves the Stream object associated with each edge.
 
@@ -89,15 +61,16 @@
     def add_input(self, name: str) -> 'DAG':
         self.graph.add_node(name, operation=DAG.input, kwargs=None, defined=True, name=name, strm=None,
                             dependencies=[])
         # Update the stream_to_node mapping
         self.stream_parent_node[name] = name
         return self
 
-    def add_step(self, name: str, operation: Callable, streams: List[str], kwargs: dict = None, defined: bool = True) -> 'DAG':
+    def add_step(self, name: str, operation: Callable, streams: List[str], kwargs: dict = None,
+                 defined: bool = True) -> 'DAG':
         # Determine dependencies from the input streams
         dependencies = [self.stream_parent_node[stream] for stream in streams]
         self.graph.add_node(name, operation=operation, dependencies=dependencies, kwargs=kwargs, defined=defined)
         for stream in streams:
             self.graph.add_edge(self.stream_parent_node[stream], name, name=stream)
         if kwargs is not None:
             for key, value in kwargs.items():
@@ -129,21 +102,25 @@
         Parameters:
         input_streams (dict): A dictionary mapping node names to Stream objects. These are the initial Stream objects
                     for the input nodes of the DAG.
 
         Returns:
         None
         """
-        logger.info("Running the DAG")  # Log the node that is being executed
+        logger.info("Preparing the DAG")
         self._finalize()
+        logger.info("Executing the DAG")
 
         # Initialize the execution state of all nodes to False
         for node in self.graph.nodes:
             self.node_executed[node] = False
 
+        # Initialise a progressbar that will count up to the number of nodes in the graph
+        pbar = tqdm(total=len(self.graph.nodes), desc="Executing nodes", unit="node")
+
         executed_nodes = set()  # Keep track of nodes that have been executed
 
         while len(executed_nodes) < len(self.graph):
             # Find nodes with no predecessors that haven't been executed yet
             ready_nodes = [node for node in self.graph.nodes if
                            all(pred in executed_nodes for pred in self.graph.predecessors(node)) and
                            node not in executed_nodes]
@@ -155,44 +132,54 @@
             if not ready_nodes:
                 unexecuted_nodes = set(self.graph.nodes) - executed_nodes
                 for node in unexecuted_nodes:
                     predecessors = list(self.graph.predecessors(node))
                     logger.debug(f"Node {node} is waiting for {predecessors}")
 
             # Create a job for each ready node
-            jobs = [delayed(self.execute_node)(node, input_streams, executed_nodes) for node in ready_nodes]
+            jobs = [delayed(self.execute_node)(node, input_streams) for node in ready_nodes]
 
             # Execute the jobs in parallel
             if jobs:
                 results = Parallel(n_jobs=self.n_jobs)(jobs)
                 # Filter out None values
                 results = [result for result in results if result is not None]
             else:
                 results = []
 
-            # Update executed_nodes with the returned value of each job
-            for i, result in enumerate(results):
-                executed_nodes.add(ready_nodes[i])
+            # Update executed_nodes and self.graph.edges with the returned values
+            for node, result, updated_edges in results:
+                executed_nodes.add(node)
+                self.node_executed[node] = True
+                for edge, strm in updated_edges.items():
+                    logger.debug(f"Updating edge {edge} with stream {strm.name}")
+                    self.graph.edges[edge]['mc'] = strm
+                # update the progress bar by one step
+                pbar.set_postfix_str(f"Processed node: {node}")
+                pbar.update()
+
+        pbar.close()  # Close the progress bar
+        logger.info(f"DAG execution complete for the nodes: {executed_nodes}")
 
-    def execute_node(self, node: str, strms: dict, executed_nodes: set) -> Optional[Union[Stream, Tuple[Stream, ...]]]:
+    def execute_node(self, node: str, strms: dict):
         """
         Executes a node in the DAG.
 
         This method takes a node and a dictionary of Stream objects. It executes the operation associated with the
         node using the Stream objects as inputs. If the node has successors and is defined, the result of the node
         execution is stored in the edges of the graph.
 
         Parameters:
         node (str): The name of the node to be executed.
         strms (dict): A dictionary mapping node names to Stream objects.
 
         Returns:
         Union[Stream, Tuple[Stream, ...]]: The result of the node execution, or None if the node is waiting for its predecessors.
         """
-        logger.info(f"Executing node {node}")  # Log the node that is being executed
+        logger.debug(f"Executing node {node}")  # Log the node that is being executed
         operation = self.graph.nodes[node]['operation']
         kwargs = self.graph.nodes[node]['kwargs']
         defined = self.graph.nodes[node]['defined']
 
         logger.debug(f"State of self.streams before executing node {node}: {self.streams}")
 
         # Log the predecessors of the node
@@ -216,58 +203,42 @@
 
             # If not an input or output, then it is a step node
             else:
                 # If the node is not in the strms dictionary, it means that it needs to be created inside the DAG
                 # In this case, execute the operation with the results of its dependencies as inputs
                 # Check if the results of the predecessors are available
 
-                if all(self.node_executed[dependency] for dependency in self.graph.predecessors(node)):
-                    inputs = [self.graph.get_edge_data(*edge)['mc'] for edge in self.graph.in_edges(node)]
-                    # If only one input stream is provided, retrieve the corresponding Stream object
-                    if len(inputs) == 1:
-                        inputs = inputs[0]
-                        # Check if kwargs is not None before passing it to the operation
-                        result = operation(inputs, **kwargs) if kwargs is not None else operation(inputs)
-                    else:
-                        # Ensure inputs is always an iterable
-                        if isinstance(inputs, Stream):
-                            inputs = [inputs]
-                        # Check if kwargs is not None before passing it to the operation
-                        result = operation(*inputs, **kwargs) if kwargs is not None else operation(*inputs)
+                inputs = [self.graph.get_edge_data(*edge)['mc'] for edge in self.graph.in_edges(node)]
+                # If only one input stream is provided, retrieve the corresponding Stream object
+                if len(inputs) == 1:
+                    inputs = inputs[0]
+                    # Check if kwargs is not None before passing it to the operation
+                    result = operation(inputs, **kwargs) if kwargs is not None else operation(inputs)
                 else:
-                    logger.debug(f"Waiting for predecessors of node {node}")
-                    return None
+                    # Ensure inputs is always an iterable
+                    if isinstance(inputs, Stream):
+                        inputs = [inputs]
+                    # Check if kwargs is not None before passing it to the operation
+                    result = operation(*inputs, **kwargs) if kwargs is not None else operation(*inputs)
 
         except AttributeError as e:
             logger.error(f"Error while executing node {node}: {e}")
             raise
 
-        # If the node has successors and is defined, store the result of the node execution in the edges of the graph
+        # Return the node, result, and the updated edges
+        updated_edges = {}
         if list(self.graph.successors(node)) and defined:
             if isinstance(result, tuple):
                 for i, strm in enumerate(result):
-                    self.graph.edges[(node, list(self.graph.successors(node))[i])]['mc'] = strm
-                    logger.debug(f"Stored results for stream {strm.name}")  # Log the node for which a result was stored
+                    updated_edges[(node, list(self.graph.successors(node))[i])] = strm
             else:
                 for successor in self.graph.successors(node):
-                    self.graph.edges[(node, successor)]['mc'] = result
-                logger.debug(f"Stored results for stream {node}")  # Log the node for which a result was stored
-
-        # After executing the operation, update the execution state of the node
-        executed_nodes.add(node)
-        self.node_executed[node] = True  # Update the execution state in the self.node_executed dictionary
-
-        # Log the state of the self.streams dictionary
-        logger.debug(f"State of self.streams after executing node {node}: {self.streams}")
-
-        # Ensure the result is always a tuple
-        if isinstance(result, Stream):
-            return (result, None)
+                    updated_edges[(node, successor)] = result
 
-        return result
+        return node, result, updated_edges
 
     def plot(self):
         plt.figure(figsize=(8, 6))
         pos = nx.spring_layout(self.graph)
         nx.draw(self.graph, pos, with_labels=True, node_color='skyblue', node_size=1500, edge_color='k', linewidths=1,
                 font_size=10, font_weight='bold', width=2)
         plt.show()
```

### Comparing `mass_composition-0.5.1/elphick/mass_composition/datasets/datasets.py` & `mass_composition-0.5.2/elphick/mass_composition/datasets/datasets.py`

 * *Files identical despite different names*

### Comparing `mass_composition-0.5.1/elphick/mass_composition/datasets/downloader.py` & `mass_composition-0.5.2/elphick/mass_composition/datasets/downloader.py`

 * *Files identical despite different names*

### Comparing `mass_composition-0.5.1/elphick/mass_composition/datasets/register.csv` & `mass_composition-0.5.2/elphick/mass_composition/datasets/register.csv`

 * *Files identical despite different names*

### Comparing `mass_composition-0.5.1/elphick/mass_composition/datasets/sample_data.py` & `mass_composition-0.5.2/elphick/mass_composition/datasets/sample_data.py`

 * *Files identical despite different names*

### Comparing `mass_composition-0.5.1/elphick/mass_composition/flowsheet.py` & `mass_composition-0.5.2/elphick/mass_composition/flowsheet.py`

 * *Files identical despite different names*

### Comparing `mass_composition-0.5.1/elphick/mass_composition/layout.py` & `mass_composition-0.5.2/elphick/mass_composition/layout.py`

 * *Files identical despite different names*

### Comparing `mass_composition-0.5.1/elphick/mass_composition/mass_composition.py` & `mass_composition-0.5.2/elphick/mass_composition/mass_composition.py`

 * *Files identical despite different names*

### Comparing `mass_composition-0.5.1/elphick/mass_composition/mc_node.py` & `mass_composition-0.5.2/elphick/mass_composition/mc_node.py`

 * *Files identical despite different names*

### Comparing `mass_composition-0.5.1/elphick/mass_composition/mc_status.py` & `mass_composition-0.5.2/elphick/mass_composition/mc_status.py`

 * *Files identical despite different names*

### Comparing `mass_composition-0.5.1/elphick/mass_composition/mc_xarray.py` & `mass_composition-0.5.2/elphick/mass_composition/mc_xarray.py`

 * *Files identical despite different names*

### Comparing `mass_composition-0.5.1/elphick/mass_composition/plot.py` & `mass_composition-0.5.2/elphick/mass_composition/plot.py`

 * *Files identical despite different names*

### Comparing `mass_composition-0.5.1/elphick/mass_composition/stream.py` & `mass_composition-0.5.2/elphick/mass_composition/stream.py`

 * *Files identical despite different names*

### Comparing `mass_composition-0.5.1/elphick/mass_composition/utils/__pycache__/components.cpython-39.pyc` & `mass_composition-0.5.2/elphick/mass_composition/utils/__pycache__/components.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `mass_composition-0.5.1/elphick/mass_composition/utils/__pycache__/moisture.cpython-39.pyc` & `mass_composition-0.5.2/elphick/mass_composition/utils/__pycache__/moisture.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `mass_composition-0.5.1/elphick/mass_composition/utils/__pycache__/viz.cpython-39.pyc` & `mass_composition-0.5.2/elphick/mass_composition/utils/__pycache__/viz.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `mass_composition-0.5.1/elphick/mass_composition/utils/amenability.py` & `mass_composition-0.5.2/elphick/mass_composition/utils/amenability.py`

 * *Files identical despite different names*

### Comparing `mass_composition-0.5.1/elphick/mass_composition/utils/components.py` & `mass_composition-0.5.2/elphick/mass_composition/utils/components.py`

 * *Files identical despite different names*

### Comparing `mass_composition-0.5.1/elphick/mass_composition/utils/hash_utils.py` & `mass_composition-0.5.2/elphick/mass_composition/utils/hash_utils.py`

 * *Files identical despite different names*

### Comparing `mass_composition-0.5.1/elphick/mass_composition/utils/interp.py` & `mass_composition-0.5.2/elphick/mass_composition/utils/interp.py`

 * *Files identical despite different names*

### Comparing `mass_composition-0.5.1/elphick/mass_composition/utils/loader.py` & `mass_composition-0.5.2/elphick/mass_composition/utils/loader.py`

 * *Files identical despite different names*

### Comparing `mass_composition-0.5.1/elphick/mass_composition/utils/moisture.py` & `mass_composition-0.5.2/elphick/mass_composition/utils/moisture.py`

 * *Files identical despite different names*

### Comparing `mass_composition-0.5.1/elphick/mass_composition/utils/parallel.py` & `mass_composition-0.5.2/elphick/mass_composition/utils/parallel.py`

 * *Files identical despite different names*

### Comparing `mass_composition-0.5.1/elphick/mass_composition/utils/partition.py` & `mass_composition-0.5.2/elphick/mass_composition/utils/partition.py`

 * *Files identical despite different names*

### Comparing `mass_composition-0.5.1/elphick/mass_composition/utils/pd_utils.py` & `mass_composition-0.5.2/elphick/mass_composition/utils/pd_utils.py`

 * *Files identical despite different names*

### Comparing `mass_composition-0.5.1/elphick/mass_composition/utils/size.py` & `mass_composition-0.5.2/elphick/mass_composition/utils/size.py`

 * *Files identical despite different names*

### Comparing `mass_composition-0.5.1/elphick/mass_composition/utils/size_distribution.py` & `mass_composition-0.5.2/elphick/mass_composition/utils/size_distribution.py`

 * *Files identical despite different names*

### Comparing `mass_composition-0.5.1/elphick/mass_composition/utils/viz.py` & `mass_composition-0.5.2/elphick/mass_composition/utils/viz.py`

 * *Files identical despite different names*

### Comparing `mass_composition-0.5.1/elphick/mass_composition/variables.py` & `mass_composition-0.5.2/elphick/mass_composition/variables.py`

 * *Files identical despite different names*

### Comparing `mass_composition-0.5.1/pyproject.toml` & `mass_composition-0.5.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mass-composition"
-version = "0.5.1"
+version = "0.5.2"
 description = "For managing multi-dimensional mass-composition datasets, supporting weighted mathematical operations and visualisation."
 authors = ["Greg <greg@elphick.com.au>"]
 packages = [{ include = "elphick/mass_composition" }]
 repository = "https://github.com/elphick/mass-composition"
 documentation = "https://elphick.github.io/mass-composition"
 readme = "README.md"
```

### Comparing `mass_composition-0.5.1/PKG-INFO` & `mass_composition-0.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mass-composition
-Version: 0.5.1
+Version: 0.5.2
 Summary: For managing multi-dimensional mass-composition datasets, supporting weighted mathematical operations and visualisation.
 Home-page: https://github.com/elphick/mass-composition
 Author: Greg
 Author-email: greg@elphick.com.au
 Requires-Python: >=3.9,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

