# Comparing `tmp/mass_composition-0.6.1.tar.gz` & `tmp/mass_composition-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mass_composition-0.6.1.tar", max compression
+gzip compressed data, was "mass_composition-0.6.2.tar", max compression
```

## Comparing `mass_composition-0.6.1.tar` & `mass_composition-0.6.2.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-r--r--   0        0        0     1069 2024-05-16 04:33:46.335871 mass_composition-0.6.1/LICENSE
--rw-r--r--   0        0        0     3491 2024-05-16 04:33:46.335871 mass_composition-0.6.1/README.md
--rw-r--r--   0        0        0      360 2024-05-16 04:33:46.743866 mass_composition-0.6.1/elphick/mass_composition/__init__.py
--rw-r--r--   0        0        0     9816 2024-05-16 04:33:46.743866 mass_composition-0.6.1/elphick/mass_composition/balance.py
--rw-r--r--   0        0        0       35 2024-05-16 04:33:46.743866 mass_composition-0.6.1/elphick/mass_composition/config/__init__.py
--rw-r--r--   0        0        0      765 2024-05-16 04:33:46.743866 mass_composition-0.6.1/elphick/mass_composition/config/config_read.py
--rw-r--r--   0        0        0      364 2024-05-16 04:33:46.743866 mass_composition-0.6.1/elphick/mass_composition/config/flowsheet_example.yaml
--rw-r--r--   0        0        0      838 2024-05-16 04:33:46.743866 mass_composition-0.6.1/elphick/mass_composition/config/mc_config.yml
--rw-r--r--   0        0        0    11999 2024-05-16 04:33:46.743866 mass_composition-0.6.1/elphick/mass_composition/dag.py
--rw-r--r--   0        0        0       59 2024-05-16 04:33:46.743866 mass_composition-0.6.1/elphick/mass_composition/datasets/__init__.py
--rw-r--r--   0        0        0     1892 2024-05-16 04:33:46.743866 mass_composition-0.6.1/elphick/mass_composition/datasets/datasets.py
--rw-r--r--   0        0        0     1622 2024-05-16 04:33:46.743866 mass_composition-0.6.1/elphick/mass_composition/datasets/downloader.py
--rw-r--r--   0        0        0     3046 2024-05-16 04:33:46.743866 mass_composition-0.6.1/elphick/mass_composition/datasets/register.csv
--rw-r--r--   0        0        0     6604 2024-05-16 04:33:46.743866 mass_composition-0.6.1/elphick/mass_composition/datasets/sample_data.py
--rw-r--r--   0        0        0    41619 2024-05-16 04:33:46.743866 mass_composition-0.6.1/elphick/mass_composition/flowsheet.py
--rw-r--r--   0        0        0     2080 2024-05-16 04:33:46.747866 mass_composition-0.6.1/elphick/mass_composition/layout.py
--rw-r--r--   0        0        0    56291 2024-05-16 04:33:46.747866 mass_composition-0.6.1/elphick/mass_composition/mass_composition.py
--rw-r--r--   0        0        0     4350 2024-05-16 04:33:46.747866 mass_composition-0.6.1/elphick/mass_composition/mc_node.py
--rw-r--r--   0        0        0      908 2024-05-16 04:33:46.747866 mass_composition-0.6.1/elphick/mass_composition/mc_status.py
--rw-r--r--   0        0        0    19483 2024-05-16 04:33:46.747866 mass_composition-0.6.1/elphick/mass_composition/mc_xarray.py
--rw-r--r--   0        0        0     5752 2024-05-16 04:33:46.747866 mass_composition-0.6.1/elphick/mass_composition/plot.py
--rw-r--r--   0        0        0     6010 2024-05-16 04:33:46.747866 mass_composition-0.6.1/elphick/mass_composition/stream.py
--rw-r--r--   0        0        0       42 2024-05-16 04:33:46.747866 mass_composition-0.6.1/elphick/mass_composition/utils/__init__.py
--rw-r--r--   0        0        0      214 2024-05-16 04:33:46.747866 mass_composition-0.6.1/elphick/mass_composition/utils/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     3909 2024-05-16 04:33:46.747866 mass_composition-0.6.1/elphick/mass_composition/utils/__pycache__/components.cpython-39.pyc
--rw-r--r--   0        0        0     2197 2024-05-16 04:33:46.747866 mass_composition-0.6.1/elphick/mass_composition/utils/__pycache__/moisture.cpython-39.pyc
--rw-r--r--   0        0        0     1494 2024-05-16 04:33:46.747866 mass_composition-0.6.1/elphick/mass_composition/utils/__pycache__/viz.cpython-39.pyc
--rw-r--r--   0        0        0     1874 2024-05-16 04:33:46.747866 mass_composition-0.6.1/elphick/mass_composition/utils/amenability.py
--rw-r--r--   0        0        0     2914 2024-05-16 04:33:46.747866 mass_composition-0.6.1/elphick/mass_composition/utils/components.py
--rw-r--r--   0        0        0       80 2024-05-16 04:33:46.747866 mass_composition-0.6.1/elphick/mass_composition/utils/geometry.py
--rw-r--r--   0        0        0     1193 2024-05-16 04:33:46.747866 mass_composition-0.6.1/elphick/mass_composition/utils/hash_utils.py
--rw-r--r--   0        0        0     9591 2024-05-16 04:33:46.747866 mass_composition-0.6.1/elphick/mass_composition/utils/interp.py
--rw-r--r--   0        0        0     4867 2024-05-16 04:33:46.747866 mass_composition-0.6.1/elphick/mass_composition/utils/loader.py
--rw-r--r--   0        0        0     2611 2024-05-16 04:33:46.747866 mass_composition-0.6.1/elphick/mass_composition/utils/moisture.py
--rw-r--r--   0        0        0      842 2024-05-16 04:33:46.747866 mass_composition-0.6.1/elphick/mass_composition/utils/parallel.py
--rw-r--r--   0        0        0     1033 2024-05-16 04:33:46.747866 mass_composition-0.6.1/elphick/mass_composition/utils/partition.py
--rw-r--r--   0        0        0     7955 2024-05-16 04:33:46.747866 mass_composition-0.6.1/elphick/mass_composition/utils/pd_utils.py
--rw-r--r--   0        0        0       61 2024-05-16 04:33:46.747866 mass_composition-0.6.1/elphick/mass_composition/utils/sampling.py
--rw-r--r--   0        0        0     2164 2024-05-16 04:33:46.747866 mass_composition-0.6.1/elphick/mass_composition/utils/size.py
--rw-r--r--   0        0        0     2630 2024-05-16 04:33:46.747866 mass_composition-0.6.1/elphick/mass_composition/utils/size_distribution.py
--rw-r--r--   0        0        0     1717 2024-05-16 04:33:46.747866 mass_composition-0.6.1/elphick/mass_composition/utils/viz.py
--rw-r--r--   0        0        0     8865 2024-05-16 04:33:46.747866 mass_composition-0.6.1/elphick/mass_composition/variables.py
--rw-r--r--   0        0        0     2040 2024-05-16 04:33:46.751865 mass_composition-0.6.1/pyproject.toml
--rw-r--r--   0        0        0     4852 1970-01-01 00:00:00.000000 mass_composition-0.6.1/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-05-16 05:07:06.997629 mass_composition-0.6.2/LICENSE
+-rw-r--r--   0        0        0     3491 2024-05-16 05:07:06.997629 mass_composition-0.6.2/README.md
+-rw-r--r--   0        0        0      360 2024-05-16 05:07:07.401633 mass_composition-0.6.2/elphick/mass_composition/__init__.py
+-rw-r--r--   0        0        0     9816 2024-05-16 05:07:07.401633 mass_composition-0.6.2/elphick/mass_composition/balance.py
+-rw-r--r--   0        0        0       35 2024-05-16 05:07:07.401633 mass_composition-0.6.2/elphick/mass_composition/config/__init__.py
+-rw-r--r--   0        0        0      765 2024-05-16 05:07:07.401633 mass_composition-0.6.2/elphick/mass_composition/config/config_read.py
+-rw-r--r--   0        0        0      364 2024-05-16 05:07:07.401633 mass_composition-0.6.2/elphick/mass_composition/config/flowsheet_example.yaml
+-rw-r--r--   0        0        0      838 2024-05-16 05:07:07.401633 mass_composition-0.6.2/elphick/mass_composition/config/mc_config.yml
+-rw-r--r--   0        0        0    12309 2024-05-16 05:07:07.401633 mass_composition-0.6.2/elphick/mass_composition/dag.py
+-rw-r--r--   0        0        0       59 2024-05-16 05:07:07.401633 mass_composition-0.6.2/elphick/mass_composition/datasets/__init__.py
+-rw-r--r--   0        0        0     1892 2024-05-16 05:07:07.401633 mass_composition-0.6.2/elphick/mass_composition/datasets/datasets.py
+-rw-r--r--   0        0        0     1622 2024-05-16 05:07:07.401633 mass_composition-0.6.2/elphick/mass_composition/datasets/downloader.py
+-rw-r--r--   0        0        0     3046 2024-05-16 05:07:07.405633 mass_composition-0.6.2/elphick/mass_composition/datasets/register.csv
+-rw-r--r--   0        0        0     6604 2024-05-16 05:07:07.405633 mass_composition-0.6.2/elphick/mass_composition/datasets/sample_data.py
+-rw-r--r--   0        0        0    41619 2024-05-16 05:07:07.405633 mass_composition-0.6.2/elphick/mass_composition/flowsheet.py
+-rw-r--r--   0        0        0     2080 2024-05-16 05:07:07.405633 mass_composition-0.6.2/elphick/mass_composition/layout.py
+-rw-r--r--   0        0        0    56291 2024-05-16 05:07:07.405633 mass_composition-0.6.2/elphick/mass_composition/mass_composition.py
+-rw-r--r--   0        0        0     4350 2024-05-16 05:07:07.405633 mass_composition-0.6.2/elphick/mass_composition/mc_node.py
+-rw-r--r--   0        0        0      908 2024-05-16 05:07:07.405633 mass_composition-0.6.2/elphick/mass_composition/mc_status.py
+-rw-r--r--   0        0        0    19483 2024-05-16 05:07:07.405633 mass_composition-0.6.2/elphick/mass_composition/mc_xarray.py
+-rw-r--r--   0        0        0     5752 2024-05-16 05:07:07.405633 mass_composition-0.6.2/elphick/mass_composition/plot.py
+-rw-r--r--   0        0        0     6010 2024-05-16 05:07:07.405633 mass_composition-0.6.2/elphick/mass_composition/stream.py
+-rw-r--r--   0        0        0       42 2024-05-16 05:07:07.405633 mass_composition-0.6.2/elphick/mass_composition/utils/__init__.py
+-rw-r--r--   0        0        0      214 2024-05-16 05:07:07.405633 mass_composition-0.6.2/elphick/mass_composition/utils/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     3909 2024-05-16 05:07:07.405633 mass_composition-0.6.2/elphick/mass_composition/utils/__pycache__/components.cpython-39.pyc
+-rw-r--r--   0        0        0     2197 2024-05-16 05:07:07.405633 mass_composition-0.6.2/elphick/mass_composition/utils/__pycache__/moisture.cpython-39.pyc
+-rw-r--r--   0        0        0     1494 2024-05-16 05:07:07.405633 mass_composition-0.6.2/elphick/mass_composition/utils/__pycache__/viz.cpython-39.pyc
+-rw-r--r--   0        0        0     1874 2024-05-16 05:07:07.405633 mass_composition-0.6.2/elphick/mass_composition/utils/amenability.py
+-rw-r--r--   0        0        0     2914 2024-05-16 05:07:07.405633 mass_composition-0.6.2/elphick/mass_composition/utils/components.py
+-rw-r--r--   0        0        0       80 2024-05-16 05:07:07.405633 mass_composition-0.6.2/elphick/mass_composition/utils/geometry.py
+-rw-r--r--   0        0        0     1193 2024-05-16 05:07:07.405633 mass_composition-0.6.2/elphick/mass_composition/utils/hash_utils.py
+-rw-r--r--   0        0        0     9591 2024-05-16 05:07:07.405633 mass_composition-0.6.2/elphick/mass_composition/utils/interp.py
+-rw-r--r--   0        0        0     4867 2024-05-16 05:07:07.405633 mass_composition-0.6.2/elphick/mass_composition/utils/loader.py
+-rw-r--r--   0        0        0     2611 2024-05-16 05:07:07.405633 mass_composition-0.6.2/elphick/mass_composition/utils/moisture.py
+-rw-r--r--   0        0        0      842 2024-05-16 05:07:07.405633 mass_composition-0.6.2/elphick/mass_composition/utils/parallel.py
+-rw-r--r--   0        0        0     1033 2024-05-16 05:07:07.405633 mass_composition-0.6.2/elphick/mass_composition/utils/partition.py
+-rw-r--r--   0        0        0     7955 2024-05-16 05:07:07.405633 mass_composition-0.6.2/elphick/mass_composition/utils/pd_utils.py
+-rw-r--r--   0        0        0       61 2024-05-16 05:07:07.405633 mass_composition-0.6.2/elphick/mass_composition/utils/sampling.py
+-rw-r--r--   0        0        0     2164 2024-05-16 05:07:07.405633 mass_composition-0.6.2/elphick/mass_composition/utils/size.py
+-rw-r--r--   0        0        0     2630 2024-05-16 05:07:07.405633 mass_composition-0.6.2/elphick/mass_composition/utils/size_distribution.py
+-rw-r--r--   0        0        0     1717 2024-05-16 05:07:07.405633 mass_composition-0.6.2/elphick/mass_composition/utils/viz.py
+-rw-r--r--   0        0        0     8865 2024-05-16 05:07:07.405633 mass_composition-0.6.2/elphick/mass_composition/variables.py
+-rw-r--r--   0        0        0     2040 2024-05-16 05:07:07.409633 mass_composition-0.6.2/pyproject.toml
+-rw-r--r--   0        0        0     4852 1970-01-01 00:00:00.000000 mass_composition-0.6.2/PKG-INFO
```

### Comparing `mass_composition-0.6.1/LICENSE` & `mass_composition-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mass_composition-0.6.1/README.md` & `mass_composition-0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `mass_composition-0.6.1/elphick/mass_composition/balance.py` & `mass_composition-0.6.2/elphick/mass_composition/balance.py`

 * *Files identical despite different names*

### Comparing `mass_composition-0.6.1/elphick/mass_composition/config/config_read.py` & `mass_composition-0.6.2/elphick/mass_composition/config/config_read.py`

 * *Files identical despite different names*

### Comparing `mass_composition-0.6.1/elphick/mass_composition/config/mc_config.yml` & `mass_composition-0.6.2/elphick/mass_composition/config/mc_config.yml`

 * *Files identical despite different names*

### Comparing `mass_composition-0.6.1/elphick/mass_composition/dag.py` & `mass_composition-0.6.2/elphick/mass_composition/dag.py`

 * *Files 2% similar despite different names*

```diff
@@ -233,15 +233,21 @@
             if isinstance(result, tuple):
                 for i, strm in enumerate(result):
                     updated_edges[(node, list(self.graph.successors(node))[i])] = strm
             else:
                 for successor in self.graph.successors(node):
                     updated_edges[(node, successor)] = result
 
-        return node, list(result), updated_edges
+        # Check the type of the result
+        if isinstance(result, MassComposition):
+            # If the result is a Stream object, return it as is
+            return node, result, updated_edges
+        else:
+            # If the result is a generator or a tuple of Stream objects, convert it to a list
+            return node, list(result), updated_edges
 
     def plot(self):
         plt.figure(figsize=(8, 6))
         pos = nx.spring_layout(self.graph)
         nx.draw(self.graph, pos, with_labels=True, node_color='skyblue', node_size=1500, edge_color='k', linewidths=1,
                 font_size=10, font_weight='bold', width=2)
         plt.show()
```

### Comparing `mass_composition-0.6.1/elphick/mass_composition/datasets/datasets.py` & `mass_composition-0.6.2/elphick/mass_composition/datasets/datasets.py`

 * *Files identical despite different names*

### Comparing `mass_composition-0.6.1/elphick/mass_composition/datasets/downloader.py` & `mass_composition-0.6.2/elphick/mass_composition/datasets/downloader.py`

 * *Files identical despite different names*

### Comparing `mass_composition-0.6.1/elphick/mass_composition/datasets/register.csv` & `mass_composition-0.6.2/elphick/mass_composition/datasets/register.csv`

 * *Files identical despite different names*

### Comparing `mass_composition-0.6.1/elphick/mass_composition/datasets/sample_data.py` & `mass_composition-0.6.2/elphick/mass_composition/datasets/sample_data.py`

 * *Files identical despite different names*

### Comparing `mass_composition-0.6.1/elphick/mass_composition/flowsheet.py` & `mass_composition-0.6.2/elphick/mass_composition/flowsheet.py`

 * *Files identical despite different names*

### Comparing `mass_composition-0.6.1/elphick/mass_composition/layout.py` & `mass_composition-0.6.2/elphick/mass_composition/layout.py`

 * *Files identical despite different names*

### Comparing `mass_composition-0.6.1/elphick/mass_composition/mass_composition.py` & `mass_composition-0.6.2/elphick/mass_composition/mass_composition.py`

 * *Files identical despite different names*

### Comparing `mass_composition-0.6.1/elphick/mass_composition/mc_node.py` & `mass_composition-0.6.2/elphick/mass_composition/mc_node.py`

 * *Files identical despite different names*

### Comparing `mass_composition-0.6.1/elphick/mass_composition/mc_status.py` & `mass_composition-0.6.2/elphick/mass_composition/mc_status.py`

 * *Files identical despite different names*

### Comparing `mass_composition-0.6.1/elphick/mass_composition/mc_xarray.py` & `mass_composition-0.6.2/elphick/mass_composition/mc_xarray.py`

 * *Files identical despite different names*

### Comparing `mass_composition-0.6.1/elphick/mass_composition/plot.py` & `mass_composition-0.6.2/elphick/mass_composition/plot.py`

 * *Files identical despite different names*

### Comparing `mass_composition-0.6.1/elphick/mass_composition/stream.py` & `mass_composition-0.6.2/elphick/mass_composition/stream.py`

 * *Files identical despite different names*

### Comparing `mass_composition-0.6.1/elphick/mass_composition/utils/__pycache__/components.cpython-39.pyc` & `mass_composition-0.6.2/elphick/mass_composition/utils/__pycache__/components.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `mass_composition-0.6.1/elphick/mass_composition/utils/__pycache__/moisture.cpython-39.pyc` & `mass_composition-0.6.2/elphick/mass_composition/utils/__pycache__/moisture.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `mass_composition-0.6.1/elphick/mass_composition/utils/__pycache__/viz.cpython-39.pyc` & `mass_composition-0.6.2/elphick/mass_composition/utils/__pycache__/viz.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `mass_composition-0.6.1/elphick/mass_composition/utils/amenability.py` & `mass_composition-0.6.2/elphick/mass_composition/utils/amenability.py`

 * *Files identical despite different names*

### Comparing `mass_composition-0.6.1/elphick/mass_composition/utils/components.py` & `mass_composition-0.6.2/elphick/mass_composition/utils/components.py`

 * *Files identical despite different names*

### Comparing `mass_composition-0.6.1/elphick/mass_composition/utils/hash_utils.py` & `mass_composition-0.6.2/elphick/mass_composition/utils/hash_utils.py`

 * *Files identical despite different names*

### Comparing `mass_composition-0.6.1/elphick/mass_composition/utils/interp.py` & `mass_composition-0.6.2/elphick/mass_composition/utils/interp.py`

 * *Files identical despite different names*

### Comparing `mass_composition-0.6.1/elphick/mass_composition/utils/loader.py` & `mass_composition-0.6.2/elphick/mass_composition/utils/loader.py`

 * *Files identical despite different names*

### Comparing `mass_composition-0.6.1/elphick/mass_composition/utils/moisture.py` & `mass_composition-0.6.2/elphick/mass_composition/utils/moisture.py`

 * *Files identical despite different names*

### Comparing `mass_composition-0.6.1/elphick/mass_composition/utils/parallel.py` & `mass_composition-0.6.2/elphick/mass_composition/utils/parallel.py`

 * *Files identical despite different names*

### Comparing `mass_composition-0.6.1/elphick/mass_composition/utils/partition.py` & `mass_composition-0.6.2/elphick/mass_composition/utils/partition.py`

 * *Files identical despite different names*

### Comparing `mass_composition-0.6.1/elphick/mass_composition/utils/pd_utils.py` & `mass_composition-0.6.2/elphick/mass_composition/utils/pd_utils.py`

 * *Files identical despite different names*

### Comparing `mass_composition-0.6.1/elphick/mass_composition/utils/size.py` & `mass_composition-0.6.2/elphick/mass_composition/utils/size.py`

 * *Files identical despite different names*

### Comparing `mass_composition-0.6.1/elphick/mass_composition/utils/size_distribution.py` & `mass_composition-0.6.2/elphick/mass_composition/utils/size_distribution.py`

 * *Files identical despite different names*

### Comparing `mass_composition-0.6.1/elphick/mass_composition/utils/viz.py` & `mass_composition-0.6.2/elphick/mass_composition/utils/viz.py`

 * *Files identical despite different names*

### Comparing `mass_composition-0.6.1/elphick/mass_composition/variables.py` & `mass_composition-0.6.2/elphick/mass_composition/variables.py`

 * *Files identical despite different names*

### Comparing `mass_composition-0.6.1/pyproject.toml` & `mass_composition-0.6.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mass-composition"
-version = "0.6.1"
+version = "0.6.2"
 description = "For managing multi-dimensional mass-composition datasets, supporting weighted mathematical operations and visualisation."
 authors = ["Greg <greg@elphick.com.au>"]
 packages = [{ include = "elphick/mass_composition" }]
 repository = "https://github.com/elphick/mass-composition"
 documentation = "https://elphick.github.io/mass-composition"
 readme = "README.md"
```

### Comparing `mass_composition-0.6.1/PKG-INFO` & `mass_composition-0.6.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mass-composition
-Version: 0.6.1
+Version: 0.6.2
 Summary: For managing multi-dimensional mass-composition datasets, supporting weighted mathematical operations and visualisation.
 Home-page: https://github.com/elphick/mass-composition
 Author: Greg
 Author-email: greg@elphick.com.au
 Requires-Python: >=3.9,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

