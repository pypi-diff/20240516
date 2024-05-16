# Comparing `tmp/scself-0.1.0.tar.gz` & `tmp/scself-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scself-0.1.0.tar", last modified: Tue May  7 18:11:47 2024, max compression
+gzip compressed data, was "scself-0.2.0.tar", last modified: Wed May 15 16:20:52 2024, max compression
```

## Comparing `scself-0.1.0.tar` & `scself-0.2.0.tar`

### file list

```diff
@@ -1,45 +1,49 @@
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2024-05-07 18:11:47.913793 scself-0.1.0/
--rw-rw-r--   0 chris     (1000) chris     (1000)     1122 2024-05-06 19:22:25.000000 scself-0.1.0/LICENSE
--rw-r--r--   0 chris     (1000) chris     (1000)      608 2024-05-07 18:11:47.913793 scself-0.1.0/PKG-INFO
--rw-rw-r--   0 chris     (1000) chris     (1000)       64 2024-05-06 19:22:25.000000 scself-0.1.0/README.md
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2024-05-07 18:11:47.909793 scself-0.1.0/scself/
--rw-rw-r--   0 chris     (1000) chris     (1000)      247 2024-05-07 17:53:37.000000 scself-0.1.0/scself/__init__.py
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2024-05-07 18:11:47.913793 scself-0.1.0/scself/_mcv/
--rw-rw-r--   0 chris     (1000) chris     (1000)       43 2024-05-07 15:20:59.000000 scself-0.1.0/scself/_mcv/__init__.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     7010 2024-05-07 15:22:50.000000 scself-0.1.0/scself/_mcv/molecular_crossvalidation.py
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2024-05-07 18:11:47.913793 scself-0.1.0/scself/_noise2self/
--rw-rw-r--   0 chris     (1000) chris     (1000)       28 2024-05-07 15:21:13.000000 scself-0.1.0/scself/_noise2self/__init__.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     5081 2024-05-06 20:54:38.000000 scself-0.1.0/scself/_noise2self/common.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     5447 2024-05-06 20:26:41.000000 scself-0.1.0/scself/_noise2self/graph.py
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2024-05-06 20:48:33.000000 scself-0.1.0/scself/_noise2self/multimodal_n2s.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     6154 2024-05-07 15:22:58.000000 scself-0.1.0/scself/_noise2self/n2s.py
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2024-05-07 18:11:47.913793 scself-0.1.0/scself/scaling/
--rw-rw-r--   0 chris     (1000) chris     (1000)       76 2024-05-06 19:59:56.000000 scself-0.1.0/scself/scaling/__init__.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     1363 2024-05-06 19:59:29.000000 scself-0.1.0/scself/scaling/truncscaler.py
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2024-05-07 18:11:47.913793 scself-0.1.0/scself/sparse/
--rw-rw-r--   0 chris     (1000) chris     (1000)      191 2024-05-06 20:01:16.000000 scself-0.1.0/scself/sparse/__init__.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     1847 2024-05-06 20:17:13.000000 scself-0.1.0/scself/sparse/graph.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     6403 2024-05-06 20:16:52.000000 scself-0.1.0/scself/sparse/math.py
--rw-rw-r--   0 chris     (1000) chris     (1000)    10626 2024-05-06 20:56:50.000000 scself-0.1.0/scself/sparse/truncated_svd.py
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2024-05-07 18:11:47.913793 scself-0.1.0/scself/tests/
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2024-05-06 21:01:57.000000 scself-0.1.0/scself/tests/__init__.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     1509 2024-02-29 17:23:43.000000 scself-0.1.0/scself/tests/_stubs.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     6119 2024-05-07 18:00:34.000000 scself-0.1.0/scself/tests/test_math.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     3378 2024-05-07 15:21:52.000000 scself-0.1.0/scself/tests/test_mcv.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     6045 2024-05-07 15:20:08.000000 scself-0.1.0/scself/tests/test_noise2self.py
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2024-05-07 18:11:47.913793 scself-0.1.0/scself/utils/
--rw-rw-r--   0 chris     (1000) chris     (1000)      244 2024-05-07 17:58:53.000000 scself-0.1.0/scself/utils/__init__.py
--rw-rw-r--   0 chris     (1000) chris     (1000)      670 2024-05-06 19:50:42.000000 scself-0.1.0/scself/utils/dot_product.py
--rw-rw-r--   0 chris     (1000) chris     (1000)      557 2024-05-06 19:45:49.000000 scself-0.1.0/scself/utils/logging.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     4662 2024-05-06 20:08:26.000000 scself-0.1.0/scself/utils/pairwise_loss.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     1939 2024-05-06 20:02:02.000000 scself-0.1.0/scself/utils/standardization.py
--rw-rw-r--   0 chris     (1000) chris     (1000)      918 2024-05-06 20:08:18.000000 scself-0.1.0/scself/utils/sum.py
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2024-05-07 18:11:47.913793 scself-0.1.0/scself.egg-info/
--rw-r--r--   0 chris     (1000) chris     (1000)      608 2024-05-07 18:11:47.000000 scself-0.1.0/scself.egg-info/PKG-INFO
--rw-rw-r--   0 chris     (1000) chris     (1000)      888 2024-05-07 18:11:47.000000 scself-0.1.0/scself.egg-info/SOURCES.txt
--rw-rw-r--   0 chris     (1000) chris     (1000)        1 2024-05-07 18:11:47.000000 scself-0.1.0/scself.egg-info/dependency_links.txt
--rw-rw-r--   0 chris     (1000) chris     (1000)        1 2024-05-06 21:04:55.000000 scself-0.1.0/scself.egg-info/not-zip-safe
--rw-rw-r--   0 chris     (1000) chris     (1000)       78 2024-05-07 18:11:47.000000 scself-0.1.0/scself.egg-info/requires.txt
--rw-rw-r--   0 chris     (1000) chris     (1000)        7 2024-05-07 18:11:47.000000 scself-0.1.0/scself.egg-info/top_level.txt
--rw-rw-r--   0 chris     (1000) chris     (1000)       38 2024-05-07 18:11:47.913793 scself-0.1.0/setup.cfg
--rw-rw-r--   0 chris     (1000) chris     (1000)     1092 2024-05-06 21:04:29.000000 scself-0.1.0/setup.py
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2024-05-15 16:20:52.807611 scself-0.2.0/
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1122 2024-05-06 19:22:25.000000 scself-0.2.0/LICENSE
+-rw-r--r--   0 chris     (1000) chris     (1000)     1393 2024-05-15 16:20:52.807611 scself-0.2.0/PKG-INFO
+-rw-rw-r--   0 chris     (1000) chris     (1000)      848 2024-05-15 16:20:07.000000 scself-0.2.0/README.md
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2024-05-15 16:20:52.803611 scself-0.2.0/scself/
+-rw-rw-r--   0 chris     (1000) chris     (1000)      282 2024-05-10 13:44:23.000000 scself-0.2.0/scself/__init__.py
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2024-05-15 16:20:52.807611 scself-0.2.0/scself/_mcv/
+-rw-rw-r--   0 chris     (1000) chris     (1000)       85 2024-05-10 13:43:03.000000 scself-0.2.0/scself/_mcv/__init__.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     3386 2024-05-14 16:32:20.000000 scself-0.2.0/scself/_mcv/common.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     2696 2024-05-10 15:45:08.000000 scself-0.2.0/scself/_mcv/mcv_per_cell.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     3148 2024-05-14 16:22:17.000000 scself-0.2.0/scself/_mcv/molecular_crossvalidation.py
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2024-05-15 16:20:52.807611 scself-0.2.0/scself/_noise2self/
+-rw-rw-r--   0 chris     (1000) chris     (1000)       78 2024-05-10 13:43:58.000000 scself-0.2.0/scself/_noise2self/__init__.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     5495 2024-05-15 16:07:41.000000 scself-0.2.0/scself/_noise2self/common.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     6634 2024-05-15 16:07:07.000000 scself-0.2.0/scself/_noise2self/graph.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     6370 2024-05-10 13:45:29.000000 scself-0.2.0/scself/_noise2self/multimodal_n2s.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     5620 2024-05-09 21:07:51.000000 scself-0.2.0/scself/_noise2self/n2s.py
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2024-05-15 16:20:52.807611 scself-0.2.0/scself/scaling/
+-rw-rw-r--   0 chris     (1000) chris     (1000)       76 2024-05-06 19:59:56.000000 scself-0.2.0/scself/scaling/__init__.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1363 2024-05-06 19:59:29.000000 scself-0.2.0/scself/scaling/truncscaler.py
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2024-05-15 16:20:52.807611 scself-0.2.0/scself/sparse/
+-rw-rw-r--   0 chris     (1000) chris     (1000)      191 2024-05-06 20:01:16.000000 scself-0.2.0/scself/sparse/__init__.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1847 2024-05-06 20:17:13.000000 scself-0.2.0/scself/sparse/graph.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     7413 2024-05-14 16:56:55.000000 scself-0.2.0/scself/sparse/math.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)    10626 2024-05-06 20:56:50.000000 scself-0.2.0/scself/sparse/truncated_svd.py
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2024-05-15 16:20:52.807611 scself-0.2.0/scself/tests/
+-rw-rw-r--   0 chris     (1000) chris     (1000)        0 2024-05-06 21:01:57.000000 scself-0.2.0/scself/tests/__init__.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1509 2024-02-29 17:23:43.000000 scself-0.2.0/scself/tests/_stubs.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     7413 2024-05-14 16:57:15.000000 scself-0.2.0/scself/tests/test_math.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     3993 2024-05-14 16:33:35.000000 scself-0.2.0/scself/tests/test_mcv.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)      946 2024-05-07 18:20:28.000000 scself-0.2.0/scself/tests/test_mkl_hacks.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     7209 2024-05-15 16:17:23.000000 scself-0.2.0/scself/tests/test_noise2self.py
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2024-05-15 16:20:52.807611 scself-0.2.0/scself/utils/
+-rw-rw-r--   0 chris     (1000) chris     (1000)      303 2024-05-14 16:31:19.000000 scself-0.2.0/scself/utils/__init__.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1083 2024-05-09 21:07:13.000000 scself-0.2.0/scself/utils/_pca.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)      670 2024-05-06 19:50:42.000000 scself-0.2.0/scself/utils/dot_product.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)      557 2024-05-06 19:45:49.000000 scself-0.2.0/scself/utils/logging.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     4622 2024-05-14 16:43:56.000000 scself-0.2.0/scself/utils/pairwise_loss.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     2067 2024-05-10 15:11:33.000000 scself-0.2.0/scself/utils/standardization.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)      984 2024-05-15 15:38:57.000000 scself-0.2.0/scself/utils/sum.py
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2024-05-15 16:20:52.807611 scself-0.2.0/scself.egg-info/
+-rw-r--r--   0 chris     (1000) chris     (1000)     1393 2024-05-15 16:20:52.000000 scself-0.2.0/scself.egg-info/PKG-INFO
+-rw-rw-r--   0 chris     (1000) chris     (1000)      990 2024-05-15 16:20:52.000000 scself-0.2.0/scself.egg-info/SOURCES.txt
+-rw-rw-r--   0 chris     (1000) chris     (1000)        1 2024-05-15 16:20:52.000000 scself-0.2.0/scself.egg-info/dependency_links.txt
+-rw-rw-r--   0 chris     (1000) chris     (1000)        1 2024-05-06 21:04:55.000000 scself-0.2.0/scself.egg-info/not-zip-safe
+-rw-rw-r--   0 chris     (1000) chris     (1000)       78 2024-05-15 16:20:52.000000 scself-0.2.0/scself.egg-info/requires.txt
+-rw-rw-r--   0 chris     (1000) chris     (1000)        7 2024-05-15 16:20:52.000000 scself-0.2.0/scself.egg-info/top_level.txt
+-rw-rw-r--   0 chris     (1000) chris     (1000)       38 2024-05-15 16:20:52.807611 scself-0.2.0/setup.cfg
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1092 2024-05-15 16:19:07.000000 scself-0.2.0/setup.py
```

### Comparing `scself-0.1.0/LICENSE` & `scself-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `scself-0.1.0/scself/_noise2self/common.py` & `scself-0.2.0/scself/_noise2self/common.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,38 +1,37 @@
 import numpy as np
 import scipy.sparse as sps
 import anndata as ad
-import tqdm
 
 from scself.utils import (
     dot,
     standardize_data,
-    pairwise_metric
+    pairwise_metric,
+    sparse_dot_patch
 )
 from scself.sparse import is_csr
-from scself.utils.dot_product import sparse_dot_patch
 from .graph import (
     local_optimal_knn,
+    combine_row_stochastic_graphs,
     _connect_to_row_stochastic,
-    _dist_to_row_stochastic
+    _dist_to_row_stochastic,
+    _invert_distance_graph
 )
 
 N_PCS = np.arange(5, 115, 10)
 N_NEIGHBORS = np.arange(15, 115, 10)
 
 
 def _search_k(
     X,
-    graph,
+    graphs,
     k,
     by_row=False,
     loss='mse',
     loss_kwargs={},
-    X_compare=None,
-    pbar=False,
     connectivity=False,
     chunk_size=10000
 ):
     """
     Find optimal number of neighbors for a given graph
 
     :param X: Data [M x N]
@@ -50,45 +49,43 @@
         for each k and each observation [K x M]
     :rtype: np.ndarray
     """
 
     n, _ = X.shape
     n_k = len(k)
 
-    X_compare = X_compare if X_compare is not None else X
-
     mses = np.zeros(n_k) if not by_row else np.zeros((n_k, n))
 
-    rfunc = tqdm.trange if pbar is True else range
-
-    if hasattr(pbar, 'postfix'):
-        _postfix = pbar.postfix
-    else:
-        _postfix = None
-
     if connectivity:
         row_normalize = _connect_to_row_stochastic
     else:
-        row_normalize = _dist_to_row_stochastic
-
-    for i in rfunc(n_k):
+        def row_normalize(x):
+            return _dist_to_row_stochastic(
+                _invert_distance_graph(x)
+            )
 
-        if _postfix is not None:
-            pbar.postfix = _postfix + f" ({k[i]} N)"
-            pbar.update(1)
+    for i in range(n_k):
 
-        # Extract k non-zero neighbors from the graph
-        k_graph = local_optimal_knn(
-            graph.copy(),
-            np.full(n, k[i]),
-            keep='smallest'
-        )
+        k_graph = [
+            # Convert to a row stochastic graph
+            row_normalize(
+                # Extract k non-zero neighbors from the graph
+                local_optimal_knn(
+                    graph.copy(),
+                    np.full(n, k[i]),
+                    keep='smallest'
+                )
+            )
+            for graph in graphs
+        ]
 
-        # Convert to a row stochastic graph
-        k_graph = row_normalize(k_graph)
+        if len(k_graph) == 1:
+            k_graph = k_graph[0]
+        else:
+            k_graph = combine_row_stochastic_graphs(k_graph)
 
         # Calculate mean squared error
         mses[i] = _noise_to_self_error(
             X,
             k_graph,
             by_row=by_row,
             metric=loss,
@@ -122,79 +119,95 @@
             _row_mse[_start:_end] = _chunk_graph_mse(
                 X,
                 k_graph,
                 _start,
                 _end
             )
 
-        if by_row:
-            return _row_mse
-        else:
-            return np.mean(_row_mse)
-
     else:
-        return pairwise_metric(
+        _row_mse = pairwise_metric(
             X,
             dot(k_graph, X, dense=not sps.issparse(X)),
-            by_row=by_row,
             metric=metric,
             **loss_kwargs
         )
 
+    if by_row:
+        return _row_mse
+    else:
+        return np.mean(_row_mse)
+
 
 def _check_args(
     neighbors,
     npcs,
-    count_data,
-    pc_data
+    count_data=None,
+    pc_data=None
 ):
 
     # Get default search parameters and check dtypes
     if neighbors is None:
         neighbors = N_NEIGHBORS
     else:
         neighbors = np.asanyarray(neighbors).reshape(-1)
 
     if npcs is None:
         npcs = N_PCS
     else:
         npcs = np.asanyarray(npcs).reshape(-1)
 
-    _max_pcs = np.max(npcs)
-
     if not np.issubdtype(neighbors.dtype, np.integer):
         raise ValueError(
             "k-NN graph requires k to be integers; "
             f"{neighbors.dtype} provided"
         )
 
     if not np.issubdtype(npcs.dtype, np.integer):
         raise ValueError(
             "n_pcs must be integers; "
             f"{npcs.dtype} provided"
         )
 
+    _check_input_data(npcs, count_data, pc_data)
+
+    return neighbors, npcs
+
+
+def _check_input_data(
+    npcs,
+    count_data,
+    pc_data
+):
+
+    _max_pcs = np.max(npcs)
+
     # Check input data sizes
     if pc_data is not None and pc_data.shape[1] < _max_pcs:
         raise ValueError(
             f"Cannot search through {_max_pcs} PCs; only "
             f"{pc_data.shape[1]} components provided"
         )
     elif min(count_data.shape) < _max_pcs:
         raise ValueError(
             f"Cannot search through {_max_pcs} PCs for "
             f"data {count_data.shape} provided"
         )
 
-    return neighbors, npcs
+    if count_data is not None and pc_data is not None:
+        if count_data.shape[0] != pc_data.shape[0]:
+            raise ValueError(
+                f"Count data {count_data.shape} observations "
+                f"do not match PC {pc_data.shape} observations"
+            )
 
 
 def _standardize(count_data, standardization_method):
     # Standardize data if necessary and create an anndata object
     # Keep separate reference to expression data and force float32
+    # This way if the expression data is provided it isnt copied
     if standardization_method is not None:
         data_obj = standardize_data(
             ad.AnnData(count_data.astype(np.float32)),
             method=standardization_method
         )
         expr_data = data_obj.X
```

### Comparing `scself-0.1.0/scself/_noise2self/graph.py` & `scself-0.2.0/scself/_noise2self/graph.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import functools
 import numpy as np
 import scipy.sparse as sps
 
 from pynndescent import PyNNDescentTransformer
 from sklearn.neighbors import NearestNeighbors
 
 from scself.sparse import is_csr
@@ -88,14 +89,31 @@
 
         # Write the new data into the original array
         neighbor_graph[i, droppers] = 0.
 
     return neighbor_graph
 
 
+def combine_row_stochastic_graphs(graphs):
+    graph = functools.reduce(lambda x, y: x + y, graphs)
+
+    rowsum = array_sum(graph, axis=1).astype(float)
+
+    if np.all(rowsum == len(graphs)):
+        if sps.issparse(graph):
+            graph.data /= len(graphs)
+        else:
+            graph /= len(graphs)
+
+    else:
+        _row_divide(graph, rowsum)
+
+    return graph
+
+
 def set_diag(X, diag):
     """
     Set diagonal of matrix X.
     Safe for dense or sparse matrices
 
     :param X: Numeric matrix
     :type X: np.ndarray, sp.spmatrix
@@ -156,45 +174,48 @@
     adata.obsp['distances'].data = adata.obsp['distances'].data.astype(
         np.float32
     )
 
     return adata
 
 
+def _invert_distance_graph(graph):
+
+    if sps.issparse(graph):
+
+        rowmean = array_sum(graph, axis=1).astype(float) / graph.shape[1]
+        rowmean[rowmean == 0] = 1.
+
+        _row_divide(graph, rowmean)
+        graph.data *= -1
+        np.exp(graph.data, out=graph.data, where=graph.data != 0)
+
+        return graph
+
+    else:
+
+        rowmean = graph.mean(axis=1)
+        rowmean[rowmean == 0] = 1.
+
+        graph /= rowmean[:, None]
+        graph *= -1
+        np.exp(graph, out=graph, where=graph != 0)
+
+        return graph
+
+
 def _dist_to_row_stochastic(graph):
 
-    if sps.isspmatrix(graph):
+    if sps.issparse(graph):
 
         rowsum = array_sum(graph, axis=1).astype(float)
         rowsum[rowsum == 0] = 1.
 
-        # Dot product between inverse rowsum diagonalized
-        # and graph.
-        # Somehow faster then element-wise \_o_/
+        return _row_divide(graph, rowsum)
 
-        if is_csr(graph):
-            from ..sparse.math import _csr_row_divide
-
-            _csr_row_divide(
-                graph.data,
-                graph.indptr,
-                rowsum
-            )
-            return graph
-        else:
-            return dot(
-                sps.diags(
-                    (1. / rowsum),
-                    offsets=0,
-                    shape=graph.shape,
-                    format='csr',
-                    dtype=graph.dtype
-                ),
-                graph
-            )
     else:
 
         rowsum = graph.sum(axis=1)
         rowsum[rowsum == 0] = 1.
 
         return np.multiply(
             graph,
@@ -210,7 +231,43 @@
     if sps.issparse(graph):
         graph.data[:] = 1
     else:
         graph = graph != 0
         graph = graph.astype(graph_dtype)
 
     return _dist_to_row_stochastic(graph)
+
+
+def _row_divide(arr, row_divide_vector):
+
+    if sps.issparse(arr):
+
+        # Numba function for CSR
+        # more memory efficient
+        if is_csr(arr):
+            from ..sparse.math import _csr_row_divide
+
+            _csr_row_divide(
+                arr.data,
+                arr.indptr,
+                row_divide_vector
+            )
+            return arr
+
+        # Dot product between inverse rowsum diagonalized
+        # and graph.
+        # Somehow faster then element-wise \_o_/
+        else:
+            return dot(
+                sps.diags(
+                    (1. / row_divide_vector),
+                    offsets=0,
+                    shape=arr.shape,
+                    format='csr',
+                    dtype=arr.dtype
+                ),
+                arr
+            )
+
+    else:
+        arr /= row_divide_vector[:, None]
+        return arr
```

### Comparing `scself-0.1.0/scself/_noise2self/n2s.py` & `scself-0.2.0/scself/_noise2self/multimodal_n2s.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,34 +1,35 @@
 import numpy as np
-import scanpy as sc
 import tqdm
 
 
-from scself.utils import log
+from scself.utils import log, pca
 from .graph import (
     neighbor_graph,
     local_optimal_knn
 )
 from .common import (
     _check_args,
+    _check_input_data,
     _standardize,
     _search_k
 )
 
 
-def noise2self(
+def multimodal_noise2self(
     count_data,
+    target_data_index=0,
+    standardization_method=None,
     neighbors=None,
     npcs=None,
     metric='euclidean',
     loss='mse',
     loss_kwargs={},
     return_errors=False,
     connectivity=False,
-    standardization_method='log',
     pc_data=None,
     chunk_size=10000,
     verbose=None
 ):
     """
     Select an optimal set of graph parameters based on noise2self
 
@@ -71,78 +72,84 @@
         global optimal k,
         local optimal k for each observation
     :rtype: sp.sparse.csr_matrix, int, int, np.ndarray [int]
     """
 
     neighbors, npcs = _check_args(
         neighbors,
-        npcs,
-        count_data,
-        pc_data
+        npcs
     )
 
-    data_obj, expr_data = _standardize(
-        count_data,
-        standardization_method
-    )
+    if not isinstance(count_data, (list, tuple)):
+        raise ValueError(
+            f"count_data must be a list of count matrices; "
+            f"{type(count_data)} provided"
+        )
 
-    log(f"Searching {len(npcs)} PC x {len(neighbors)} Neighbors space")
+    _n_modes = len(count_data)
+
+    if pc_data is None:
+        pc_data = [None] * _n_modes
+    elif not isinstance(pc_data, (list, tuple)):
+        raise ValueError(
+            f"pc_data must be a list of PC matrices; "
+            f"{type(pc_data)} provided"
+        )
 
-    if pc_data is not None:
-        log(f"Using existing PCs {pc_data.shape}")
-        data_obj.obsm['X_pca'] = pc_data
+    for c, p in zip(count_data, pc_data):
+        _check_input_data(npcs, c, pc_data)
 
-    else:
-        log(f"Calculating {np.max(npcs)} PCs")
-        data_obj.obsm['X_pca'] = sc.pp.pca(
-            expr_data,
-            n_comps=np.max(npcs),
-            zero_center=False
+    data_obj = [None] * _n_modes
+    expr_data = [None] * _n_modes
+
+    for i in range(_n_modes):
+
+        data_obj[i], expr_data[i] = _standardize(
+            count_data[i],
+            standardization_method
         )
 
+    log(f"Searching {len(npcs)} PC x {len(neighbors)} Neighbors space")
+
+    for i in range(_n_modes):
+        if pc_data[i] is not None:
+            log(f"Using existing PCs {pc_data[i].shape}")
+            data_obj[i].obsm['X_pca'] = pc_data[i]
+
+        else:
+            pca(data_obj[i], expr_data[i], np.max(npcs))
+
     mses = np.zeros((len(npcs), len(neighbors)))
 
     if len(npcs) > 1:
-        # Create a progress bar
-        tqdm_pbar = tqdm.tqdm(
-            enumerate(npcs),
-            postfix=f"{npcs[0]} PCs",
-            bar_format='{l_bar}{bar}{r_bar}',
-            total=len(npcs) * len(neighbors)
-        )
 
         # Search for the smallest MSE for each n_pcs / k combination
         # Outer loop does PCs, because the distance graph has to be
         # recalculated when PCs changes
-        for i, pc in tqdm_pbar:
+        for i, pc in tqdm.tqdm(enumerate(npcs)):
 
             # Calculate neighbor graph with the max number of neighbors
             # Faster to select only a subset of edges than to recalculate
             # (obviously)
             neighbor_graph(
                 data_obj,
                 pc,
                 np.max(neighbors),
                 metric=metric
             )
 
-            # Update the progress bar
-            tqdm_pbar.postfix = f"{pc} PCs Neighbor Search"
-            tqdm_pbar.update(0)
-
             # Search through the neighbors space
             mses[i, :] = _search_k(
                 expr_data,
-                data_obj.obsp['distances'],
+                (data_obj.obsp['distances'], ),
                 neighbors,
                 connectivity=connectivity,
                 loss=loss,
                 loss_kwargs=loss_kwargs,
-                chunk_size=chunk_size,
-                pbar=tqdm_pbar
+                chunk_size=chunk_size
             )
 
         # Get the index of the optimal PCs and k based on
         # minimizing MSE
         op_pc = np.argmin(np.min(mses, axis=1))
         op_k = np.argmin(mses[op_pc, :])
 
@@ -173,18 +180,17 @@
     )
 
     # Search for the optimal number of k for each obs
     # For the global optimal n_pc
     local_k = local_neighbors[np.argmin(
         _search_k(
             expr_data,
-            data_obj.obsp['distances'],
+            (data_obj.obsp['distances'], ),
             local_neighbors,
             by_row=True,
-            pbar=True,
             connectivity=connectivity,
             loss=loss,
             loss_kwargs=loss_kwargs,
             chunk_size=chunk_size
         ),
         axis=0
     )]
```

### Comparing `scself-0.1.0/scself/scaling/truncscaler.py` & `scself-0.2.0/scself/scaling/truncscaler.py`

 * *Files identical despite different names*

### Comparing `scself-0.1.0/scself/sparse/graph.py` & `scself-0.2.0/scself/sparse/graph.py`

 * *Files identical despite different names*

### Comparing `scself-0.1.0/scself/sparse/math.py` & `scself-0.2.0/scself/sparse/math.py`

 * *Files 27% similar despite different names*

```diff
@@ -7,44 +7,66 @@
     return sps.isspmatrix_csr(x) or isinstance(x, sps.csr_array)
 
 
 def is_csc(x):
     return sps.isspmatrix_csc(x) or isinstance(x, sps.csc_array)
 
 
-def mcv_mse_sparse(
+def mcv_mean_error_sparse(
     x,
     pc,
     rotation,
-    by_row=False,
     axis=1,
+    squared=False,
     **metric_kwargs
 ):
+    """
+    Wrapper for numba sparse mean error that calculates projection row-wise
+    to minimize memory footprint
+
+    :param x: Sparse data
+    :type x: sp.sparse.spmatrix, sp.sparse.sparray
+    :param pc: Principal component array
+    :type pc: np.ndarray
+    :param rotation: PCA rotation array
+    :type rotation: np.ndarray
+    :param axis: Aggregation axis, defaults to 1 (row).
+        None is flattened.
+    :type axis: int, optional
+    :param squared: Calculate mean squared error.
+        False is mean absolute error, defaults to False.
+    :type squared: bool, optional
+    :raises ValueError: Incorrect axis argument
+    :return: Mean error over axis (or scaler if flattened)
+    :rtype: np.ndarray, float
+    """
 
     if axis == 1:
-        func = _mse_rowwise
+        func = _mean_error_rowwise
     elif axis == 0:
-        func = _mse_columnwise
+        func = _mean_error_columnwise
+    elif axis is None:
+        func = _mean_error_rowwise
     else:
         raise ValueError
 
     y = func(
         x.data,
         x.indices,
         x.indptr,
         np.ascontiguousarray(pc),
         np.ascontiguousarray(rotation, dtype=pc.dtype),
-        x.shape[1]
+        x.shape[1],
+        squared
     )
 
-    if by_row:
-        return y
+    if axis is None:
+        y = y.mean()
 
-    else:
-        return np.mean(y)
+    return y
 
 
 def sparse_sum(sparse_array, axis=None, squared=False):
 
     if not sps.issparse(sparse_array):
         raise ValueError("sparse_sum requires a sparse array")
 
@@ -149,21 +171,22 @@
         return arr
 
     else:
         return new_data, col_indptr
 
 
 @numba.njit(parallel=False)
-def _mse_rowwise(
+def _mean_error_rowwise(
     a_data,
     a_indices,
     a_indptr,
     b_pcs,
     b_rotation,
-    n_cols
+    n_cols,
+    squared
 ):
 
     n_row = b_pcs.shape[0]
 
     output = np.zeros(n_row, dtype=float)
 
     for i in numba.prange(n_row):
@@ -174,27 +197,31 @@
         row = b_pcs[i, :] @ b_rotation
 
         if _nnz_a == 0:
             pass
         else:
             row[_idx_a] -= a_data[a_indptr[i]:a_indptr[i + 1]]
 
-        output[i] = np.mean(row ** 2)
+        if squared:
+            output[i] = np.mean(row ** 2)
+        else:
+            output[i] = np.mean(np.abs(row))
 
     return output
 
 
 @numba.njit(parallel=False)
-def _mse_columnwise(
+def _mean_error_columnwise(
     a_data,
     a_indices,
     a_indptr,
     b_pcs,
     b_rotation,
-    n_cols
+    n_cols,
+    squared
 ):
 
     n_row = b_pcs.shape[0]
     output = np.zeros(n_cols, dtype=float)
 
     for i in numba.prange(n_row):
 
@@ -204,15 +231,18 @@
         row = b_pcs[i, :] @ b_rotation
 
         if _nnz_a == 0:
             pass
         else:
             row[_idx_a] -= a_data[a_indptr[i]:a_indptr[i + 1]]
 
-        output += row ** 2
+        if squared:
+            output += row ** 2
+        else:
+            output += np.abs(row)
 
     return output / n_row
 
 
 @numba.njit(parallel=False)
 def _sum_columns(data, indices, n_col):
```

### Comparing `scself-0.1.0/scself/sparse/truncated_svd.py` & `scself-0.2.0/scself/sparse/truncated_svd.py`

 * *Files identical despite different names*

### Comparing `scself-0.1.0/scself/tests/_stubs.py` & `scself-0.2.0/scself/tests/_stubs.py`

 * *Files identical despite different names*

### Comparing `scself-0.1.0/scself/utils/dot_product.py` & `scself-0.2.0/scself/utils/dot_product.py`

 * *Files identical despite different names*

### Comparing `scself-0.1.0/scself/utils/logging.py` & `scself-0.2.0/scself/utils/logging.py`

 * *Files identical despite different names*

### Comparing `scself-0.1.0/scself/utils/pairwise_loss.py` & `scself-0.2.0/scself/utils/pairwise_loss.py`

 * *Files 8% similar despite different names*

```diff
@@ -56,36 +56,35 @@
 def _mae(x, y, axis=1):
 
     if y is not None:
         ssr = x - y
     else:
         ssr = x
 
+    ssr = np.abs(ssr)
+
     return ssr.sum(axis=axis)
 
 
 def pairwise_metric(
     x,
     y,
     metric='mse',
-    by_row=False,
     axis=1,
     **kwargs
 ):
     """
     Pairwise metric between two arrays
 
     :param x: _description_
     :type x: _type_
     :param y: _description_
     :type y: _type_
     :param metric: _description_, defaults to 'mse'
     :type metric: str, optional
-    :param by_row: _description_, defaults to False
-    :type by_row: bool, optional
     :return: _description_
     :rtype: _type_
     """
 
     if metric == 'mse':
         metric = _mse
     elif metric == 'mae':
@@ -101,21 +100,19 @@
     )
 
     try:
         loss = loss.A1
     except AttributeError:
         pass
 
-    loss = loss / x.shape[axis]
-
-    if by_row:
-        return loss
-
+    if axis is not None:
+        return loss / x.shape[axis]
     else:
-        return loss.sum() / loss.size
+        _size = x.shape[0] * x.shape[1]
+        return loss / _size
 
 
 def variance(
     X,
     axis=None,
     ddof=0
 ):
@@ -203,39 +200,38 @@
         np.sqrt(_var),
         _mean,
         out=np.zeros_like(_var),
         where=_mean != 0
     )
 
 
-def mcv_mse(
+def mcv_mean_error(
     x,
     pc,
     rotation,
-    by_row=False,
     axis=1,
+    squared=True,
     **metric_kwargs
 ):
 
     if sps.issparse(x):
 
-        from ..sparse.math import mcv_mse_sparse
+        from ..sparse.math import mcv_mean_error_sparse
 
-        return mcv_mse_sparse(
+        return mcv_mean_error_sparse(
             x,
             pc,
             rotation,
-            by_row=by_row,
             axis=axis,
+            squared=squared,
             **metric_kwargs
         )
 
     else:
 
         return pairwise_metric(
             x,
             pc @ rotation,
-            metric='mse',
-            by_row=by_row,
+            metric='mse' if squared else 'mae',
             axis=axis,
             **metric_kwargs
         )
```

### Comparing `scself-0.1.0/scself/utils/standardization.py` & `scself-0.2.0/scself/utils/standardization.py`

 * *Files 4% similar despite different names*

```diff
@@ -75,14 +75,19 @@
     elif method == 'log_scale':
         return _normalize_for_pca(
             count_data,
             target_sum,
             log=True,
             scale=True
         )
+    elif method == 'depth':
+        return _normalize_for_pca(
+            count_data,
+            target_sum
+        )
     elif method is None:
         return count_data
     else:
         raise ValueError(
-            f'method must be None, `log`, `scale`, or `log_scale`, '
+            'method must be None, `depth`, `log`, `scale`, or `log_scale`, '
             f'{method} provided'
         )
```

### Comparing `scself-0.1.0/scself/utils/sum.py` & `scself-0.2.0/scself/utils/sum.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 import numpy as np
 import scipy.sparse as sps
 from scself.sparse import is_csr
 
 
 def array_sum(array, axis=None, squared=False):
 
+    if not sps.issparse(array):
+        return array.sum(axis)
+
     # If it's not a CSR array use builtins
-    if not is_csr(array):
+    elif not is_csr(array):
 
         if squared and not sps.issparse(array):
             _sums = (array ** 2).sum(axis=axis)
         elif squared:
             _sums = array.power(2).sum(axis=axis)
         else:
             _sums = array.sum(axis=axis)
```

### Comparing `scself-0.1.0/scself.egg-info/SOURCES.txt` & `scself-0.2.0/scself.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -5,14 +5,16 @@
 scself.egg-info/PKG-INFO
 scself.egg-info/SOURCES.txt
 scself.egg-info/dependency_links.txt
 scself.egg-info/not-zip-safe
 scself.egg-info/requires.txt
 scself.egg-info/top_level.txt
 scself/_mcv/__init__.py
+scself/_mcv/common.py
+scself/_mcv/mcv_per_cell.py
 scself/_mcv/molecular_crossvalidation.py
 scself/_noise2self/__init__.py
 scself/_noise2self/common.py
 scself/_noise2self/graph.py
 scself/_noise2self/multimodal_n2s.py
 scself/_noise2self/n2s.py
 scself/scaling/__init__.py
@@ -21,14 +23,16 @@
 scself/sparse/graph.py
 scself/sparse/math.py
 scself/sparse/truncated_svd.py
 scself/tests/__init__.py
 scself/tests/_stubs.py
 scself/tests/test_math.py
 scself/tests/test_mcv.py
+scself/tests/test_mkl_hacks.py
 scself/tests/test_noise2self.py
 scself/utils/__init__.py
+scself/utils/_pca.py
 scself/utils/dot_product.py
 scself/utils/logging.py
 scself/utils/pairwise_loss.py
 scself/utils/standardization.py
 scself/utils/sum.py
```

### Comparing `scself-0.1.0/setup.py` & `scself-0.2.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 ]
 
 tests_require = [
     "coverage",
     "pytest"
 ]
 
-version = "0.1.0"
+version = "0.2.0"
 
 # Description from README.md
 long_description = "\n\n".join(
     [open(
         os.path.join(
             os.path.dirname(os.path.abspath(__file__)),
             "README.md"
```

