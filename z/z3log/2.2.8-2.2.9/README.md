# Comparing `tmp/z3log-2.2.8.tar.gz` & `tmp/z3log-2.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "z3log-2.2.8.tar", last modified: Mon Dec 18 14:28:31 2023, max compression
+gzip compressed data, was "z3log-2.2.9.tar", last modified: Mon Jan  8 13:35:05 2024, max compression
```

## Comparing `z3log-2.2.8.tar` & `z3log-2.2.9.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxr-x   0 usi       (1000) usi       (1000)        0 2023-12-18 14:28:31.084581 z3log-2.2.8/
--rw-rw-r--   0 usi       (1000) usi       (1000)     1328 2023-12-18 14:28:31.084581 z3log-2.2.8/PKG-INFO
--rw-rw-r--   0 usi       (1000) usi       (1000)        8 2023-10-05 10:44:59.000000 z3log-2.2.8/README.md
-drwxrwxr-x   0 usi       (1000) usi       (1000)        0 2023-12-18 14:28:31.084581 z3log-2.2.8/Z3Log/
--rw-rw-r--   0 usi       (1000) usi       (1000)        2 2023-11-08 10:27:53.000000 z3log-2.2.8/Z3Log/__init__.py
--rw-rw-r--   0 usi       (1000) usi       (1000)     5459 2023-11-13 10:55:19.000000 z3log-2.2.8/Z3Log/argument.py
-drwxrwxr-x   0 usi       (1000) usi       (1000)        0 2023-12-18 14:28:31.084581 z3log-2.2.8/Z3Log/config/
--rw-rw-r--   0 usi       (1000) usi       (1000)        2 2023-11-08 10:27:53.000000 z3log-2.2.8/Z3Log/config/__init__.py
--rw-rw-r--   0 usi       (1000) usi       (1000)     1655 2023-11-08 10:27:53.000000 z3log-2.2.8/Z3Log/config/config.py
--rw-rw-r--   0 usi       (1000) usi       (1000)      772 2023-11-08 10:27:53.000000 z3log-2.2.8/Z3Log/config/path.py
--rw-rw-r--   0 usi       (1000) usi       (1000)    21764 2023-12-18 12:14:42.000000 z3log-2.2.8/Z3Log/graph.py
--rw-rw-r--   0 usi       (1000) usi       (1000)    15355 2023-11-08 10:27:53.000000 z3log-2.2.8/Z3Log/result.py
--rw-rw-r--   0 usi       (1000) usi       (1000)     1657 2023-11-08 10:27:53.000000 z3log-2.2.8/Z3Log/specs.py
--rw-rw-r--   0 usi       (1000) usi       (1000)     3731 2023-11-08 10:27:53.000000 z3log-2.2.8/Z3Log/stats.py
--rw-rw-r--   0 usi       (1000) usi       (1000)     4583 2023-11-08 10:27:53.000000 z3log-2.2.8/Z3Log/testbench.py
--rw-rw-r--   0 usi       (1000) usi       (1000)     2558 2023-12-18 12:15:03.000000 z3log-2.2.8/Z3Log/utils.py
--rw-rw-r--   0 usi       (1000) usi       (1000)    21285 2023-12-18 12:23:53.000000 z3log-2.2.8/Z3Log/verilog.py
--rw-rw-r--   0 usi       (1000) usi       (1000)    97801 2023-11-14 14:31:56.000000 z3log-2.2.8/Z3Log/z3solver.py
--rw-rw-r--   0 usi       (1000) usi       (1000)       38 2023-12-18 14:28:31.084581 z3log-2.2.8/setup.cfg
--rw-rw-r--   0 usi       (1000) usi       (1000)     1742 2023-12-18 14:28:09.000000 z3log-2.2.8/setup.py
-drwxrwxr-x   0 usi       (1000) usi       (1000)        0 2023-12-18 14:28:31.084581 z3log-2.2.8/z3log.egg-info/
--rw-rw-r--   0 usi       (1000) usi       (1000)     1328 2023-12-18 14:28:31.000000 z3log-2.2.8/z3log.egg-info/PKG-INFO
--rw-rw-r--   0 usi       (1000) usi       (1000)      397 2023-12-18 14:28:31.000000 z3log-2.2.8/z3log.egg-info/SOURCES.txt
--rw-rw-r--   0 usi       (1000) usi       (1000)        1 2023-12-18 14:28:31.000000 z3log-2.2.8/z3log.egg-info/dependency_links.txt
--rw-rw-r--   0 usi       (1000) usi       (1000)      352 2023-12-18 14:28:31.000000 z3log-2.2.8/z3log.egg-info/requires.txt
--rw-rw-r--   0 usi       (1000) usi       (1000)        6 2023-12-18 14:28:31.000000 z3log-2.2.8/z3log.egg-info/top_level.txt
+drwxrwxr-x   0 usi       (1000) usi       (1000)        0 2024-01-08 13:35:05.435274 z3log-2.2.9/
+-rw-rw-r--   0 usi       (1000) usi       (1000)     1328 2024-01-08 13:35:05.435274 z3log-2.2.9/PKG-INFO
+-rw-rw-r--   0 usi       (1000) usi       (1000)        8 2023-10-05 10:44:59.000000 z3log-2.2.9/README.md
+drwxrwxr-x   0 usi       (1000) usi       (1000)        0 2024-01-08 13:35:05.435274 z3log-2.2.9/Z3Log/
+-rw-rw-r--   0 usi       (1000) usi       (1000)        2 2023-11-08 10:27:53.000000 z3log-2.2.9/Z3Log/__init__.py
+-rw-rw-r--   0 usi       (1000) usi       (1000)     5459 2023-11-13 10:55:19.000000 z3log-2.2.9/Z3Log/argument.py
+drwxrwxr-x   0 usi       (1000) usi       (1000)        0 2024-01-08 13:35:05.435274 z3log-2.2.9/Z3Log/config/
+-rw-rw-r--   0 usi       (1000) usi       (1000)        2 2023-11-08 10:27:53.000000 z3log-2.2.9/Z3Log/config/__init__.py
+-rw-rw-r--   0 usi       (1000) usi       (1000)     1655 2023-11-08 10:27:53.000000 z3log-2.2.9/Z3Log/config/config.py
+-rw-rw-r--   0 usi       (1000) usi       (1000)      772 2023-11-08 10:27:53.000000 z3log-2.2.9/Z3Log/config/path.py
+-rw-rw-r--   0 usi       (1000) usi       (1000)    22743 2024-01-03 13:16:44.000000 z3log-2.2.9/Z3Log/graph.py
+-rw-rw-r--   0 usi       (1000) usi       (1000)    15355 2023-11-08 10:27:53.000000 z3log-2.2.9/Z3Log/result.py
+-rw-rw-r--   0 usi       (1000) usi       (1000)     1657 2023-11-08 10:27:53.000000 z3log-2.2.9/Z3Log/specs.py
+-rw-rw-r--   0 usi       (1000) usi       (1000)     3731 2023-11-08 10:27:53.000000 z3log-2.2.9/Z3Log/stats.py
+-rw-rw-r--   0 usi       (1000) usi       (1000)     4583 2023-11-08 10:27:53.000000 z3log-2.2.9/Z3Log/testbench.py
+-rw-rw-r--   0 usi       (1000) usi       (1000)     2598 2023-12-21 10:31:10.000000 z3log-2.2.9/Z3Log/utils.py
+-rw-rw-r--   0 usi       (1000) usi       (1000)    21285 2023-12-19 11:17:35.000000 z3log-2.2.9/Z3Log/verilog.py
+-rw-rw-r--   0 usi       (1000) usi       (1000)    98832 2024-01-08 10:50:04.000000 z3log-2.2.9/Z3Log/z3solver.py
+-rw-rw-r--   0 usi       (1000) usi       (1000)       38 2024-01-08 13:35:05.439273 z3log-2.2.9/setup.cfg
+-rw-rw-r--   0 usi       (1000) usi       (1000)     1742 2024-01-08 13:34:43.000000 z3log-2.2.9/setup.py
+drwxrwxr-x   0 usi       (1000) usi       (1000)        0 2024-01-08 13:35:05.435274 z3log-2.2.9/z3log.egg-info/
+-rw-rw-r--   0 usi       (1000) usi       (1000)     1328 2024-01-08 13:35:05.000000 z3log-2.2.9/z3log.egg-info/PKG-INFO
+-rw-rw-r--   0 usi       (1000) usi       (1000)      397 2024-01-08 13:35:05.000000 z3log-2.2.9/z3log.egg-info/SOURCES.txt
+-rw-rw-r--   0 usi       (1000) usi       (1000)        1 2024-01-08 13:35:05.000000 z3log-2.2.9/z3log.egg-info/dependency_links.txt
+-rw-rw-r--   0 usi       (1000) usi       (1000)      352 2024-01-08 13:35:05.000000 z3log-2.2.9/z3log.egg-info/requires.txt
+-rw-rw-r--   0 usi       (1000) usi       (1000)        6 2024-01-08 13:35:05.000000 z3log-2.2.9/z3log.egg-info/top_level.txt
```

### Comparing `z3log-2.2.8/PKG-INFO` & `z3log-2.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: z3log
-Version: 2.2.8
+Version: 2.2.9
 Summary: 
 Paper Title: ErrorEval: an Open-Source Worst-Case-Error Evaluation Framework for Approximate Computing
 
 Short Description: The open-source toolchain that proposes a methodology called ErrorEval which relies on 
 SMT (Satisfiability Modulo Theories) solvers.
 
 Authors:
```

### Comparing `z3log-2.2.8/Z3Log/argument.py` & `z3log-2.2.9/Z3Log/argument.py`

 * *Files identical despite different names*

### Comparing `z3log-2.2.8/Z3Log/config/config.py` & `z3log-2.2.9/Z3Log/config/config.py`

 * *Files identical despite different names*

### Comparing `z3log-2.2.8/Z3Log/config/path.py` & `z3log-2.2.9/Z3Log/config/path.py`

 * *Files identical despite different names*

### Comparing `z3log-2.2.8/Z3Log/graph.py` & `z3log-2.2.9/Z3Log/graph.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import networkx as nx
 import re
 from typing import Dict, List
 from .config.path import *
 from .config.config import *
 import os
 from .argument import Arguments
-
+import time
 
 class Graph:
     def __init__(self, benchmark_name, is_clean: bool = False, address: str = None):
         """
         takes in a circuit and creates a networkx graph out of it
         :param benchmark_name: the input benchmark in gv format
         :param is_clean: leave empty for now
@@ -31,25 +31,34 @@
         self.__verilog_in_path = f'{folder}/{benchmark_name}.{extension}'
 
         # print(f'Converting the graph into a NeworkX object')
 
 
         self.__graph = self.import_graph(address)
 
+
         self.__sorted_node_list = None
 
         self.__is_clean = is_clean
 
-
+        # s = time.time()
         if not self.is_clean:
             self.clean_graph()
+        # e = time.time()
+        # print(Fore.LIGHTBLUE_EX + f'cleaning runtime = {e - s}', Style.RESET_ALL)
+
 
 
         self.sort_graph()
+
+
+
         self.remove_output_outgoing_edges()
+
+
         self.__input_dict = self.sort_dict(self.extract_inputs())
         self.__output_dict = self.sort_dict(self.extract_outputs())
         self.__gate_dict = self.sort_dict(self.extract_gates())
         self.__constant_dict = self.sort_dict(self.extract_constants())
 
 
 
@@ -294,41 +303,65 @@
     #         """
     #     with open(f'yosys_graph.log', 'w') as y:
     #         subprocess.call([YOSYS, '-p', yosys_command], stdout=y)
     #     print(f'{self.dot_in_path = }')
     #     self.fix_direction()
 
     def fix_direction(self):
-        print(f'{self.dot_in_path = }')
+        # print(f'{self.dot_in_path = }')
         dot_command = f'{DOT} {self.dot_in_path} -Grankdir=TB -o {self.out_path}'
         subprocess.call([dot_command], shell=True)
-        print(f'{self.dot_in_path = }')
+        # print(f'{self.dot_in_path = }')
         os.remove(self.dot_in_path)
 
     def clean_graph(self):
-        # for n in self.graph.nodes:
-        #     if LABEL not in self.graph.nodes[n]:
-        #         print(f'{n}, {self.graph.nodes[n] = }')
-
-        # for n in self.graph.nodes:
-        #     if LABEL not in self.graph.nodes[n]:
-        #         print(f'{n}, {self.graph.nodes[n] = }')
-        # exit()
+        # s = time.time()
         self.merge_points_into_source()
+        # e = time.time()
+        # print(Fore.GREEN + f'merge_points_into_source runtime = {e - s}', Style.RESET_ALL)
+
+
         self.clean_input_labels()
+
+
         self.clean_output_labels()
+
         self.clean_wire_labels()
+
+
         self.clean_gate_labels()
+
+
         self.clean_constant_labels()
+
+
         self.merge_buffers_into_gates()
+
+
+        # s = time.time()
         self.merge_wires_into_gates()
+        # e = time.time()
+        # print(Fore.GREEN + f'merge_wires_into_gates runtime = {e - s}', Style.RESET_ALL)
+
+        # s = time.time()
         self.relabel_nodes()
+        # e = time.time()
+        # print(Fore.GREEN + f'relabel_nodes runtime = {e - s}', Style.RESET_ALL)
+
+
         self.delete_extra_fields()
+
+
+
         self.set_is_clean(True)
         self.count_iog()
+        e = time.time()
+
+
+        s = time.time()
         self.set_input_dict(self.extract_inputs())
         self.set_output_dict(self.extract_outputs())
         self.set_gate_dict(self.extract_gates())
         self.set_constant_dict(self.extract_constants())
 
 
     def delete_extra_fields(self):
@@ -386,77 +419,92 @@
             if self.graph.nodes[e[1]]['label'] == 'BUF':
                 src_node = e[0]
                 des_node = e[1]
                 tmp_graph = nx.contracted_nodes(tmp_graph, src_node, des_node, self_loops=False)
         self.set_graph(tmp_graph)
 
     def merge_points_into_source(self):
+        # s = time.time()
         tmp_graph = self.graph.copy(as_view=False)
+        # e = time.time()
+        # print(f'copy runtime = {e - s}')
+
+        # s = time.time()
         for e in self.graph.edges:
             if self.graph.nodes[e[1]][SHAPE] == 'point':
-                # print(f'{e[1] = }')
                 src_node = e[0]
                 des_node = e[1]
-                tmp_graph = nx.contracted_nodes(tmp_graph, src_node, des_node, self_loops=False)
+                # tmp_graph = nx.contracted_nodes(tmp_graph, src_node, des_node, self_loops=False)
+                nx.contracted_nodes(tmp_graph, src_node, des_node, self_loops=False, copy=False)
+        # e = time.time()
+        # print(f'merging (iterating over edges) runtime = {e - s}')
+
+        # s = time.time()
         self.set_graph(tmp_graph)
+        # e = time.time()
+        # print(f'set graph runtime = {e - s}')
 
     def merge_wires_into_gates(self):
         tmp_graph = self.graph.copy(as_view=False)
         for e in self.graph.edges:
-            # if (re.search(POSSIBLE_GATES, self.graph.nodes[e[0]]['label']) and
-            #         re.search('g\d+', self.graph.nodes[e[1]]['label'])):
             if re.search('g\d+', self.graph.nodes[e[1]]['label']):
                 src_node = e[0]
                 des_node = e[1]
-                tmp_graph = nx.contracted_nodes(tmp_graph, src_node, des_node, self_loops=False)
+                # tmp_graph = nx.contracted_nodes(tmp_graph, src_node, des_node, self_loops=False)
+                nx.contracted_nodes(tmp_graph, src_node, des_node, self_loops=False, copy=False)
         self.set_graph(tmp_graph)
 
 
     def relabel_nodes(self):
         tmp_graph = self.graph.copy()
         gate_idx = 0
         for n in self.graph.nodes:
             if self.is_cleaned_pi(n):
                 old_name = n
                 new_name = self.graph.nodes[n]['label']
 
                 mapping = {old_name: new_name}
-                tmp_graph = nx.relabel_nodes(tmp_graph, mapping)
+                # tmp_graph = nx.relabel_nodes(tmp_graph, mapping)
+                nx.relabel_nodes(tmp_graph, mapping, copy=False)
             elif self.is_cleaned_po(n):
                 old_name = n
                 new_name = self.graph.nodes[n]['label']
 
                 mapping = {old_name: new_name}
-                tmp_graph = nx.relabel_nodes(tmp_graph, mapping)
+                # tmp_graph = nx.relabel_nodes(tmp_graph, mapping)
+                nx.relabel_nodes(tmp_graph, mapping, copy=False)
             elif self.is_merged_gate(n):
                 old_name = n
                 new_name = f'g{gate_idx}'
                 gate_idx += 1
 
                 mapping = {old_name: new_name}
-                tmp_graph = nx.relabel_nodes(tmp_graph, mapping)
+                # tmp_graph = nx.relabel_nodes(tmp_graph, mapping)
+                nx.relabel_nodes(tmp_graph, mapping, copy=False)
             elif self.is_cleaned_gate(n):
                 old_name = n
                 new_name = f'g{gate_idx}'
                 gate_idx += 1
 
                 mapping = {old_name: new_name}
-                tmp_graph = nx.relabel_nodes(tmp_graph, mapping)
+                # tmp_graph = nx.relabel_nodes(tmp_graph, mapping)
+                nx.relabel_nodes(tmp_graph, mapping, copy=False)
             elif self.is_constant(n):
                 old_name = n
                 new_name = f'g{gate_idx}'
                 gate_idx += 1
 
                 mapping = {old_name: new_name}
-                tmp_graph = nx.relabel_nodes(tmp_graph, mapping)
+                # tmp_graph = nx.relabel_nodes(tmp_graph, mapping)
+                nx.relabel_nodes(tmp_graph, mapping, copy=False)
             else:
                 print(f'{n = }, {self.graph.nodes[n]}')
                 print('WARNING! No mapping needed!')
 
-        # exit()
+
         self.set_graph(tmp_graph)
 
 
     def is_cleaned_pi(self, node):
         if not self.is_constant(node):
             if re.search(r'in\d+', self.graph.nodes[node][LABEL]):
                 return True
```

### Comparing `z3log-2.2.8/Z3Log/result.py` & `z3log-2.2.9/Z3Log/result.py`

 * *Files identical despite different names*

### Comparing `z3log-2.2.8/Z3Log/specs.py` & `z3log-2.2.9/Z3Log/specs.py`

 * *Files identical despite different names*

### Comparing `z3log-2.2.8/Z3Log/stats.py` & `z3log-2.2.9/Z3Log/stats.py`

 * *Files identical despite different names*

### Comparing `z3log-2.2.8/Z3Log/testbench.py` & `z3log-2.2.9/Z3Log/testbench.py`

 * *Files identical despite different names*

### Comparing `z3log-2.2.8/Z3Log/utils.py` & `z3log-2.2.9/Z3Log/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import re
 import subprocess
 import os
 import shutil
 from .config.path import *
 from .config.config import *
+import time
 
 
 def get_pure_name(file_name: str) -> str:
     if file_name is None:
         return file_name
     name = file_name
     if re.search('/', file_name):
@@ -26,31 +27,35 @@
 
     dot_command = f'{DOT} {dot_in_path} -Grankdir=TB -o {gv_out_path}'
     subprocess.call([dot_command], shell=True)
     os.remove(dot_in_path)
 
 
 def convert_verilog_to_gv(file_name: str) -> None:
+
     file_name = get_pure_name(file_name)
 
     folder, extension = OUTPUT_PATH['ver']
     verilog_in_path = f'{folder}/{file_name}.{extension}'
     # print(f'{verilog_in_path = }')
     folder, extension = OUTPUT_PATH['gv']
     gv_out_path = f'{folder}/{file_name}.{extension}'
 
     yosys_command = f"""
         read_verilog {verilog_in_path}
+        opt
+        clean
         show -prefix {gv_out_path[:-3]} -format gv
         """
     with open(f'yosys_graph.log', 'w') as y:
         subprocess.call([YOSYS, '-p', yosys_command], stdout=y)
     fix_direction(file_name)
 
 
+
 def setup_folder_structure():
     # Setting up the folder structure
     directories = [OUTPUT_PATH['ver'][0], OUTPUT_PATH['aig'][0], OUTPUT_PATH['gv'][0], OUTPUT_PATH['z3'][0],
                    OUTPUT_PATH['report'][0], OUTPUT_PATH['figure'][0], TEST_PATH['tb'][0], TEST_PATH['z3'][0]]
 
     for directory in directories:
         if ~os.path.exists(directory):
```

### Comparing `z3log-2.2.8/Z3Log/verilog.py` & `z3log-2.2.9/Z3Log/verilog.py`

 * *Files identical despite different names*

### Comparing `z3log-2.2.8/Z3Log/z3solver.py` & `z3log-2.2.9/Z3Log/z3solver.py`

 * *Files 2% similar despite different names*

```diff
@@ -428,15 +428,15 @@
             # Use the number of available CPU cores
             num_workers = multiprocessing.cpu_count()
             # Initialize a Pool of worker processes
             with multiprocessing.Pool(num_workers) as pool:
                 # Create all node names to be processed
                 args = [(labler, f'app_g{i}', queue) for i in range(num_of_nodes)]
                 # Map the helper function to each node name
-                pool.map(self.labler_wrapper, args)
+                pool.map(self.labler_wrapper, args, chunksize=1)
             # Now get the results from the queue
             for _ in range(num_of_nodes):
                 node, weight = queue.get()
                 shared_list.append((node, weight))
             print(Fore.LIGHTBLUE_EX + 'Done' + Style.RESET_ALL)
         else:
             print(Fore.LIGHTBLUE_EX + f'Labeling (implicit & NOT parallel)... ', end='' + Style.RESET_ALL)
@@ -462,20 +462,23 @@
             node, weight = node_weight
             self.append_label(node, weight)
 
 
 
 
     def implicit_labeling(self, removed_node: str = None, queue = None, this_ctx=None):
-
+        st = time.time()
         if this_ctx is None:
 
             this_ctx = Context()
         s = Optimize(ctx=this_ctx)
         assert s.ctx == this_ctx
+        et = time.time()
+        # print(f'define solver time = {et - st}')
+        st = time.time()
         f_exact = Function('f_exact', IntSort( ctx=this_ctx), IntSort( ctx=this_ctx))
         f_approx = Function('f_approx', IntSort( ctx=this_ctx), IntSort( ctx=this_ctx))
         f_error = Function('f_error', IntSort( ctx=this_ctx), IntSort( ctx=this_ctx), IntSort( ctx=this_ctx))
         input_list_exact = self.BoolVector('in', self.graph.num_inputs, exact=True, ctx=this_ctx)
 
         gate_list_exact = self.BoolVector('g', self.graph.num_constants + self.graph.num_gates, exact=True, ctx=this_ctx)
         output_list_exact = self.BoolVector('out', self.graph.num_outputs, exact=True, ctx=this_ctx)
@@ -486,60 +489,85 @@
 
 
         gate_list_approx = self.BoolVector('g', self.approximate_graph.num_constants + self.approximate_graph.num_gates, exact=False, ctx=this_ctx)
         output_list_approx = self.BoolVector('out', self.approximate_graph.num_outputs, exact=False, ctx=this_ctx)
         approx_circuit = self.convert_approximate_to_implicit_z3_constraints(removed_node, ctx=this_ctx)
         approx_output = self.integer_circuit_output_to_implicit_z3_constriants(output_list_approx, exact=False, ctx=this_ctx)
 
+        et = time.time()
+        # print(f'conversion time = {et - st}')
+
+        st = time.time()
+        s.add(exact_circuit)
+        s.add(approx_circuit)
+
 
 
-        s.add((exact_circuit))
-        s.add((approx_circuit))
         if self.style == 'max':
             foundWCE = False
             wce = 0
+            st = time.time()
             while(not foundWCE):
                 s.push()
                 s.add(f_exact(exact_output) == exact_output)
                 s.add(f_approx(approx_output) == approx_output)
                 s.add(f_error(exact_output, approx_output) == Abs(exact_output - approx_output))
                 s.add(f_error(exact_output, approx_output) > wce)
                 s.maximize(f_error(exact_output, approx_output))
+
+                # print(f'adding constraints time = {et - st}')
+
                 c = s.check()
+                # print(f'{c = }')
                 if c == sat:
                     wce = abs((s.model()[f_error].else_value().as_long()))
+                    # print(f'{wce}')
                 else:
                     foundWCE = True
+
+                # print(f'check time = {et -st}')
                 s.pop()
             del s
             if queue:
+                et = time.time()
+                # print(f'{this_ctx = }')
+                # print(f'{removed_node}={wce} is done labeling! in {et - st}')
                 queue.put((removed_node, wce))
             else:
+                # print(f'{this_ctx = }')
+                et = time.time()
+                # print(f'{removed_node}={wce} is done labeling! in {et - st}')
+
                 return wce
         else:
             foundBCE = False
             bce = None
 
             s.push()
             s.add(f_exact(exact_output) == exact_output)
             s.add(f_approx(approx_output) == approx_output)
             s.add(f_error(exact_output, approx_output) == Abs(exact_output - approx_output))
             s.add(f_error(exact_output, approx_output) > 0)
             s.minimize(f_error(exact_output, approx_output))
+            et = time.time()
+            # print(f'adding constraints time = {et - st}')
             c = s.check()
+            et = time.time()
+            runtime = et  -  st
             if c == sat:
                 bce = abs((s.model()[f_error].else_value().as_long()))
-
             else:
                 foundBCE = True
             s.pop()
             del s
             if queue:
+                print(f'{removed_node} is done labeling!')
                 queue.put((removed_node, bce))
             else:
+                print(f'{removed_node} is done labeling!')
                 return bce
 
 
     def evaluate(self):
         return self.implicit_labeling()
 
     def import_results(self):
```

### Comparing `z3log-2.2.8/setup.py` & `z3log-2.2.9/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 import os
 
 
-VERSION = '2.2.8'
+VERSION = '2.2.9'
 DESCRIPTION = """
 Paper Title: ErrorEval: an Open-Source Worst-Case-Error Evaluation Framework for Approximate Computing
 
 Short Description: The open-source toolchain that proposes a methodology called ErrorEval which relies on 
 SMT (Satisfiability Modulo Theories) solvers.
 
 Authors:
```

### Comparing `z3log-2.2.8/z3log.egg-info/PKG-INFO` & `z3log-2.2.9/z3log.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: z3log
-Version: 2.2.8
+Version: 2.2.9
 Summary: 
 Paper Title: ErrorEval: an Open-Source Worst-Case-Error Evaluation Framework for Approximate Computing
 
 Short Description: The open-source toolchain that proposes a methodology called ErrorEval which relies on 
 SMT (Satisfiability Modulo Theories) solvers.
 
 Authors:
```

