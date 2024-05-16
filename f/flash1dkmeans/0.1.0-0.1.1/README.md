# Comparing `tmp/flash1dkmeans-0.1.0.tar.gz` & `tmp/flash1dkmeans-0.1.1.tar.gz`

## Comparing `flash1dkmeans-0.1.0.tar` & `flash1dkmeans-0.1.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 flash1dkmeans-0.1.0/.idea/.gitignore
--rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 flash1dkmeans-0.1.0/.idea/flash1dkmeans.iml
--rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 flash1dkmeans-0.1.0/.idea/misc.xml
--rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 flash1dkmeans-0.1.0/.idea/modules.xml
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 flash1dkmeans-0.1.0/.idea/vcs.xml
--rw-r--r--   0        0        0     9505 2020-02-02 00:00:00.000000 flash1dkmeans-0.1.0/.idea/workspace.xml
--rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 flash1dkmeans-0.1.0/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 flash1dkmeans-0.1.0/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 flash1dkmeans-0.1.0/src/flash1dkmeans/__init__.py
--rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 flash1dkmeans-0.1.0/src/flash1dkmeans/config.py
--rw-r--r--   0        0        0    19117 2020-02-02 00:00:00.000000 flash1dkmeans-0.1.0/src/flash1dkmeans/k_cluster.py
--rw-r--r--   0        0        0     6861 2020-02-02 00:00:00.000000 flash1dkmeans-0.1.0/src/flash1dkmeans/main.py
--rw-r--r--   0        0        0     9772 2020-02-02 00:00:00.000000 flash1dkmeans-0.1.0/src/flash1dkmeans/two_cluster.py
--rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 flash1dkmeans-0.1.0/src/flash1dkmeans/utils.py
--rw-r--r--   0        0        0     1345 2020-02-02 00:00:00.000000 flash1dkmeans-0.1.0/tests/complex.py
--rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 flash1dkmeans-0.1.0/tests/k_cluster.py
--rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 flash1dkmeans-0.1.0/tests/two_cluster.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 flash1dkmeans-0.1.0/.gitignore
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 flash1dkmeans-0.1.0/LICENSE
--rw-r--r--   0        0        0     3784 2020-02-02 00:00:00.000000 flash1dkmeans-0.1.0/README.md
--rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 flash1dkmeans-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     4393 2020-02-02 00:00:00.000000 flash1dkmeans-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 flash1dkmeans-0.1.1/.idea/.gitignore
+-rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 flash1dkmeans-0.1.1/.idea/flash1dkmeans.iml
+-rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 flash1dkmeans-0.1.1/.idea/misc.xml
+-rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 flash1dkmeans-0.1.1/.idea/modules.xml
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 flash1dkmeans-0.1.1/.idea/vcs.xml
+-rw-r--r--   0        0        0    10140 2020-02-02 00:00:00.000000 flash1dkmeans-0.1.1/.idea/workspace.xml
+-rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 flash1dkmeans-0.1.1/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 flash1dkmeans-0.1.1/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 flash1dkmeans-0.1.1/src/flash1dkmeans/__init__.py
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 flash1dkmeans-0.1.1/src/flash1dkmeans/config.py
+-rw-r--r--   0        0        0    19159 2020-02-02 00:00:00.000000 flash1dkmeans-0.1.1/src/flash1dkmeans/k_cluster.py
+-rw-r--r--   0        0        0     6861 2020-02-02 00:00:00.000000 flash1dkmeans-0.1.1/src/flash1dkmeans/main.py
+-rw-r--r--   0        0        0     9796 2020-02-02 00:00:00.000000 flash1dkmeans-0.1.1/src/flash1dkmeans/two_cluster.py
+-rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 flash1dkmeans-0.1.1/src/flash1dkmeans/utils.py
+-rw-r--r--   0        0        0     1345 2020-02-02 00:00:00.000000 flash1dkmeans-0.1.1/tests/complex.py
+-rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 flash1dkmeans-0.1.1/tests/k_cluster.py
+-rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 flash1dkmeans-0.1.1/tests/two_cluster.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 flash1dkmeans-0.1.1/.gitignore
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 flash1dkmeans-0.1.1/LICENSE
+-rw-r--r--   0        0        0     5049 2020-02-02 00:00:00.000000 flash1dkmeans-0.1.1/README.md
+-rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 flash1dkmeans-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     5658 2020-02-02 00:00:00.000000 flash1dkmeans-0.1.1/PKG-INFO
```

### Comparing `flash1dkmeans-0.1.0/.idea/flash1dkmeans.iml` & `flash1dkmeans-0.1.1/.idea/flash1dkmeans.iml`

 * *Files identical despite different names*

### Comparing `flash1dkmeans-0.1.0/.idea/workspace.xml` & `flash1dkmeans-0.1.1/.idea/workspace.xml`

 * *Files 14% similar despite different names*

#### Comparing `flash1dkmeans-0.1.0/.idea/workspace.xml` & `flash1dkmeans-0.1.1/.idea/workspace.xml`

```diff
@@ -1,15 +1,14 @@
 <?xml version="1.0" encoding="utf-8"?>
 <project version="4">
   <component name="AutoImportSettings">
     <option name="autoReloadType" value="SELECTIVE"/>
   </component>
   <component name="ChangeListManager">
     <list default="true" id="1ba58836-480f-43dd-9244-0130cb4b0f23" name="Changes" comment="">
-      <change beforePath="$PROJECT_DIR$/pyproject.toml" beforeDir="false" afterPath="$PROJECT_DIR$/pyproject.toml" afterDir="false"/>
       <change beforePath="$PROJECT_DIR$/src/flash1dkmeans/two_cluster.py" beforeDir="false" afterPath="$PROJECT_DIR$/src/flash1dkmeans/two_cluster.py" afterDir="false"/>
     </list>
     <option name="SHOW_DIALOG" value="false"/>
     <option name="HIGHLIGHT_CONFLICTS" value="true"/>
     <option name="HIGHLIGHT_NON_ACTIVE_CHANGELIST" value="false"/>
     <option name="LAST_RESOLUTION" value="IGNORE"/>
   </component>
@@ -18,14 +17,15 @@
       <list>
         <option value="Python Script"/>
       </list>
     </option>
   </component>
   <component name="Git.Settings">
     <option name="RECENT_GIT_ROOT_PATH" value="$PROJECT_DIR$"/>
+    <option name="UPDATE_TYPE" value="REBASE"/>
   </component>
   <component name="GitHubPullRequestSearchHistory">{
   &quot;lastFilter&quot;: {
     &quot;state&quot;: &quot;OPEN&quot;,
     &quot;assignee&quot;: &quot;SyphonArch&quot;
   }
 }</component>
@@ -39,27 +39,27 @@
   &quot;associatedIndex&quot;: 0
 }</component>
   <component name="ProjectId" id="2g0ckhIOtcRZbf0wuNcUZcsVEhk"/>
   <component name="ProjectViewState">
     <option name="hideEmptyMiddlePackages" value="true"/>
     <option name="showLibraryContents" value="true"/>
   </component>
-  <component name="PropertiesComponent"><![CDATA[{
-  "keyToString": {
-    "RunOnceActivity.ShowReadmeOnStart": "true",
-    "git-widget-placeholder": "main",
-    "node.js.detected.package.eslint": "true",
-    "node.js.detected.package.tslint": "true",
-    "node.js.selected.package.eslint": "(autodetect)",
-    "node.js.selected.package.tslint": "(autodetect)",
-    "nodejs_package_manager_path": "npm",
-    "settings.editor.selected.configurable": "preferences.keymap",
-    "vue.rearranger.settings.migration": "true"
+  <component name="PropertiesComponent">{
+  &quot;keyToString&quot;: {
+    &quot;RunOnceActivity.ShowReadmeOnStart&quot;: &quot;true&quot;,
+    &quot;git-widget-placeholder&quot;: &quot;main&quot;,
+    &quot;node.js.detected.package.eslint&quot;: &quot;true&quot;,
+    &quot;node.js.detected.package.tslint&quot;: &quot;true&quot;,
+    &quot;node.js.selected.package.eslint&quot;: &quot;(autodetect)&quot;,
+    &quot;node.js.selected.package.tslint&quot;: &quot;(autodetect)&quot;,
+    &quot;nodejs_package_manager_path&quot;: &quot;npm&quot;,
+    &quot;settings.editor.selected.configurable&quot;: &quot;preferences.keymap&quot;,
+    &quot;vue.rearranger.settings.migration&quot;: &quot;true&quot;
   }
-}]]></component>
+}</component>
   <component name="SharedIndexes">
     <attachedChunks>
       <set>
         <option value="bundled-js-predefined-1d06a55b98c1-91d5c284f522-JavaScript-PY-241.15989.155"/>
         <option value="bundled-python-sdk-babbdf50b680-7c6932dee5e4-com.jetbrains.pycharm.pro.sharedIndexes.bundled-PY-241.15989.155"/>
       </set>
     </attachedChunks>
@@ -73,15 +73,16 @@
       <option name="presentableId" value="Default"/>
       <updated>1714838079481</updated>
       <workItem from="1714838080524" duration="170000"/>
       <workItem from="1714838257640" duration="1013000"/>
       <workItem from="1714888190868" duration="167000"/>
       <workItem from="1714898221385" duration="481000"/>
       <workItem from="1714899699435" duration="2811000"/>
-      <workItem from="1714905466256" duration="33030000"/>
+      <workItem from="1714905466256" duration="33115000"/>
+      <workItem from="1715875822589" duration="829000"/>
     </task>
     <task id="LOCAL-00001" summary="Drop start_idx and stop_idx">
       <option name="closed" value="true"/>
       <created>1714905994757</created>
       <option name="number" value="00001"/>
       <option name="presentableId" value="LOCAL-00001"/>
       <option name="project" value="LOCAL"/>
@@ -187,15 +188,23 @@
       <option name="closed" value="true"/>
       <created>1714937500698</created>
       <option name="number" value="00014"/>
       <option name="presentableId" value="LOCAL-00014"/>
       <option name="project" value="LOCAL"/>
       <updated>1714937500698</updated>
     </task>
-    <option name="localTasksCounter" value="15"/>
+    <task id="LOCAL-00015" summary="First version to work with Any-Precision LLM">
+      <option name="closed" value="true"/>
+      <created>1714938973858</created>
+      <option name="number" value="00015"/>
+      <option name="presentableId" value="LOCAL-00015"/>
+      <option name="project" value="LOCAL"/>
+      <updated>1714938973858</updated>
+    </task>
+    <option name="localTasksCounter" value="16"/>
     <servers/>
   </component>
   <component name="TypeScriptGeneratedFilesManager">
     <option name="version" value="3"/>
   </component>
   <component name="VcsManagerConfiguration">
     <MESSAGE value="Drop start_idx and stop_idx"/>
@@ -207,10 +216,12 @@
     <MESSAGE value="Cleanup"/>
     <MESSAGE value="Drop numba for now"/>
     <MESSAGE value="Make Numba work"/>
     <MESSAGE value="Update README"/>
     <MESSAGE value="Refactor code"/>
     <MESSAGE value="Increment version"/>
     <MESSAGE value="Change argument ordering"/>
-    <option name="LAST_COMMIT_MESSAGE" value="Change argument ordering"/>
+    <MESSAGE value="First"/>
+    <MESSAGE value="First version to work with Any-Precision LLM"/>
+    <option name="LAST_COMMIT_MESSAGE" value="First version to work with Any-Precision LLM"/>
   </component>
 </project>
```

### Comparing `flash1dkmeans-0.1.0/.idea/inspectionProfiles/Project_Default.xml` & `flash1dkmeans-0.1.1/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `flash1dkmeans-0.1.0/src/flash1dkmeans/k_cluster.py` & `flash1dkmeans-0.1.1/src/flash1dkmeans/k_cluster.py`

 * *Files 1% similar despite different names*

```diff
@@ -388,15 +388,15 @@
 @numba.njit(cache=True)
 def _kmeans_plusplus(X, n_clusters,
                      weights_prefix_sum, weighted_X_prefix_sum, weighted_X_squared_prefix_sum,
                      start_idx, stop_idx):
     """An optimized version of the kmeans++ initialization algorithm for 1D data.
     The algorithm is optimized for 1D data and utilizes prefix sums for efficient calculations.
 
-    Time complexity: O(n_clusters * log(n_clusters) * log(len(X)) * n_clusters)
+    Time complexity: O(n_clusters * (log(n_clusters) * log(len(X)) * n_clusters + log(len(X)) * n_clusters + n_clusters))
                      = O(k ^ 2 * log(k) * log(n))
 
     Args:
         X: np.ndarray
             The input data
         n_clusters: int
             The number of clusters to choose
```

### Comparing `flash1dkmeans-0.1.0/src/flash1dkmeans/main.py` & `flash1dkmeans-0.1.1/src/flash1dkmeans/main.py`

 * *Files identical despite different names*

### Comparing `flash1dkmeans-0.1.0/src/flash1dkmeans/two_cluster.py` & `flash1dkmeans-0.1.1/src/flash1dkmeans/two_cluster.py`

 * *Files 4% similar despite different names*

```diff
@@ -100,39 +100,39 @@
     # We don't want empty clusters, so we set the floor and ceiling to start_idx + 1 and stop_idx - 1
     floor = start_idx + 1
     ceiling = stop_idx - 1
     left_centroid = None
     right_centroid = None
     division_point = None
 
-    while floor + 1 < ceiling:
+    while floor < ceiling:
         division_point = (floor + ceiling) // 2
         # If the left cluster has no weight, we need to move the floor up
         left_weight_sum = query_prefix_sum(weights_prefix_sum, start_idx, division_point)
         if left_weight_sum == 0:
-            floor = division_point
+            floor = division_point + 1
             continue
         right_weight_sum = query_prefix_sum(weights_prefix_sum, division_point, stop_idx)
         # If the right cluster has no weight, we need to move the ceiling down
         if right_weight_sum == 0:
-            ceiling = division_point
+            ceiling = division_point - 1
             continue
 
         left_centroid = query_prefix_sum(weighted_X_prefix_sum, start_idx, division_point) / left_weight_sum
         right_centroid = query_prefix_sum(weighted_X_prefix_sum, division_point, stop_idx) / right_weight_sum
 
         new_division_point_value = (left_centroid + right_centroid) / 2
         if sorted_X[division_point - 1] <= new_division_point_value:
             if new_division_point_value <= sorted_X[division_point]:
                 # The new division point matches the previous one, so we can stop
                 break
             else:
-                floor = division_point
+                floor = division_point + 1
         else:
-            ceiling = division_point
+            ceiling = division_point - 1
 
     # initialize variables in case the loop above does not run through
     if left_centroid is None:
         division_point = (floor + ceiling) // 2
         left_centroid = (query_prefix_sum(weighted_X_prefix_sum, start_idx, division_point) /
                          query_prefix_sum(weights_prefix_sum, start_idx, division_point))
     if right_centroid is None:
@@ -183,39 +183,39 @@
     # We don't want empty clusters, so we set the floor and ceiling to start_idx + 1 and stop_idx - 1
     floor = start_idx + 1
     ceiling = stop_idx - 1
     left_centroid = None
     right_centroid = None
     division_point = None
 
-    while floor + 1 < ceiling:
+    while floor < ceiling:
         division_point = (floor + ceiling) // 2
         # If the left cluster has no weight, we need to move the floor up
         left_weight_sum = division_point - start_idx
         if left_weight_sum == 0:
-            floor = division_point
+            floor = division_point + 1
             continue
         right_weight_sum = stop_idx - division_point
         # If the right cluster has no weight, we need to move the ceiling down
         if right_weight_sum == 0:
-            ceiling = division_point
+            ceiling = division_point - 1
             continue
 
         left_centroid = query_prefix_sum(X_prefix_sum, start_idx, division_point) / left_weight_sum
         right_centroid = query_prefix_sum(X_prefix_sum, division_point, stop_idx) / right_weight_sum
 
         new_division_point_value = (left_centroid + right_centroid) / 2
         if sorted_X[division_point - 1] <= new_division_point_value:
             if new_division_point_value <= sorted_X[division_point]:
                 # The new division point matches the previous one, so we can stop
                 break
             else:
-                floor = division_point
+                floor = division_point + 1
         else:
-            ceiling = division_point
+            ceiling = division_point - 1
 
     # initialize variables in case the loop above does not run through
     if left_centroid is None:
         division_point = (floor + ceiling) // 2
         left_centroid = query_prefix_sum(X_prefix_sum, start_idx, division_point) / (division_point - start_idx)
     if right_centroid is None:
         division_point = (floor + ceiling) // 2
```

### Comparing `flash1dkmeans-0.1.0/tests/complex.py` & `flash1dkmeans-0.1.1/tests/complex.py`

 * *Files identical despite different names*

### Comparing `flash1dkmeans-0.1.0/.gitignore` & `flash1dkmeans-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `flash1dkmeans-0.1.0/LICENSE` & `flash1dkmeans-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `flash1dkmeans-0.1.0/README.md` & `flash1dkmeans-0.1.1/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -2,34 +2,47 @@
 An optimized K-means implementation for the one-dimensional case
 
 Exploits the fact that one-dimensional data can be sorted.
 
 For the lower level functions prefixed with `numba_`, Numba acceleration is used,
 so callers can utilize these functions within their own Numba-accelerated functions.
 
+## Important Notice
+
+This library utilizes [Numba](https://numba.pydata.org/), a JIT compiler, for acceleration.
+As there is a compile time overhead, the first invocation may be slower than usual.
+
+Numba caches the compiled functions, so execution times should stabilize after the first invocation.
+
 ## Features
 
 ### Two clusters
 
-Guaranteed to find the optimal solution for two clusters.
+Guaranteed to find the optimal solution for two clusters by employing a clever binary search.
 
 ### K clusters
 
 Uses the K-means++ initialization algorithm to find the initial centroids.
 Then uses the Lloyd's algorithm to find the final centroids, except with optimizations for the one-dimensional case.
 
 ## Time Complexity
 
-- **2 clusters**: O(log(n))
-- (+ (O(n) for prefix sum calculation if not provided))
-- **k clusters**: O(k * 2 + log(k) * log(n) + max_iter * log(n) * k)  
-  (+ (O(n) for prefix sum calculation if not provided))
+For number of elements $n$, number of clusteres $k$, number of Lloyd's algorithm iterations $i$, and assuming one-dimensional data (which is the only case covered by this implementation):
 
-This is a significant improvement over the standard K-means algorithm, which has a time complexity of O(n * k * max_iter),
-even excluding the time complexity of the K-means++ initialization.
+- **2 clusters**: $O(\log{n})$  
+  ($+ O(n)$ for prefix sum calculation if not provided, $+ O(n \cdot \log {n})$ for sorting if not sorted)
+- **$k$ clusters**: $O(k ^ 2 \cdot \log {k} \cdot \log {n}) + O(i \cdot \log {n} \cdot k)$  
+  (The first term is for K-means++ initialization, and the latter for Lloyd's algorithm)  
+  ($+ O(n)$ for prefix sum calculation if not provided, $+ O(n \cdot \log {n})$ for sorting if not sorted)
+
+This is a significant improvement over common K-means implementations.
+For example, general implementations for $d$-dimensional data using a combination of greedy K-means++ initialization and Lloyd's algorithm for convergence,
+when given one-dimensional data, spends $O(k ^ 2 \cdot \log {k} \cdot n)$ time in initialization and $O(i \cdot n \cdot k)$ time in iterations.
+
+**Note that you must use the underlying `numba_` functions directly in order to directly supply prefix sums and skip sorting.**
 
 ## How fast is it?
 
 TODO: Comparision with sklearn's KMeans
 
 
 ## Installation
@@ -62,25 +75,27 @@
     data, k,
     sample_weights=weights,  # sample weights
     max_iter=100,  # maximum number of iterations
 )
 ```
 
 ### Even More Options
-The underlying Numba-accelerated function `_sorted_kmeans_1d` can be used directly for more control.
+The underlying Numba-accelerated function `numba_kmeans_1d_k_clusters` can be used directly for more control.
 
 This is useful when the algorithm is run multiple times on different segments of the data,
 or to use within another Numba-accelerated function.
 
 The list of available functions are as follows:
 - `numba_kmeans_1d_two_clusters`
 - `numba_kmeans_1d_two_clusters_unweighted`
 - `numba_kmeans_1d_k_cluster`
 - `numba_kmeans_1d_k_cluster_unweighted`
 
+All of these functions assume the data is sorted beforehand.
+
 ```python
 from flash1dkmeans import numba_kmeans_1d_k_cluster
 import numpy as np
 
 n, k = 1024, 4
 
 # Generate random data
@@ -96,18 +111,17 @@
 weighted_X_squared_prefix_sum = np.cumsum(data ** 2 * weights)
 
 middle_idx = n // 2
 
 # Providing prefix sums reduces redundant calculations
 # This is useful when the algorithm is run multiple times on different segments of the data
 for start_idx, stop_idx in [(0, middle_idx), (middle_idx, n)]:
-  centroids, cluster_borders = numba_kmeans_1d_k_cluster(
+  centroids, cluster_borders = numba_kmeans_1d_k_cluster(  # Note that data MUST be sorted beforehand
     data, k,  # Note how the sample weights are not provided when the prefix sums are provided
     max_iter=100,  # maximum number of iterations
-    is_sorted=True,
     weights_prefix_sum=weights_prefix_sum,  # prefix sum of the sample weights, leave empty for unwieghted data
     weighted_X_prefix_sum=weighted_X_prefix_sum,  # prefix sum of the weighted data
     weighted_X_squared_prefix_sum=weighted_X_squared_prefix_sum,  # prefix sum of the squared weighted data
     start_idx=start_idx,  # start index of the data
     stop_idx=stop_idx,  # stop index of the data
   )
 ```
@@ -117,7 +131,9 @@
 ## Notes
 
 This repository has been created to be used in [Any-Precision-LLM](https://github.com/SNU-ARC/any-precision-llm) project,
 where multiple 1D K-means instances are run in parallel for LLM quantization.
 
 However, the algorithm is general and can be used for any 1D K-means problem.
 
+I have proved the validity for the two cluster case - detailed version of the proof might be posted in the future.
+
```

### Comparing `flash1dkmeans-0.1.0/pyproject.toml` & `flash1dkmeans-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "flash1dkmeans"
-version = "0.1.0"
+version = "0.1.1"
 authors = [
   { name="Jake Hyun", email="jake.hyun@hotmail.com" },
 ]
 description = "An optimized K-means implementation for the one-dimensional case."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `flash1dkmeans-0.1.0/PKG-INFO` & `flash1dkmeans-0.1.1/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: flash1dkmeans
-Version: 0.1.0
+Version: 0.1.1
 Summary: An optimized K-means implementation for the one-dimensional case.
 Project-URL: Homepage, https://github.com/SyphonArch/flash1dkmeans
 Project-URL: Issues, https://github.com/SyphonArch/flash1dkmeans/issues
 Author-email: Jake Hyun <jake.hyun@hotmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -18,34 +18,47 @@
 An optimized K-means implementation for the one-dimensional case
 
 Exploits the fact that one-dimensional data can be sorted.
 
 For the lower level functions prefixed with `numba_`, Numba acceleration is used,
 so callers can utilize these functions within their own Numba-accelerated functions.
 
+## Important Notice
+
+This library utilizes [Numba](https://numba.pydata.org/), a JIT compiler, for acceleration.
+As there is a compile time overhead, the first invocation may be slower than usual.
+
+Numba caches the compiled functions, so execution times should stabilize after the first invocation.
+
 ## Features
 
 ### Two clusters
 
-Guaranteed to find the optimal solution for two clusters.
+Guaranteed to find the optimal solution for two clusters by employing a clever binary search.
 
 ### K clusters
 
 Uses the K-means++ initialization algorithm to find the initial centroids.
 Then uses the Lloyd's algorithm to find the final centroids, except with optimizations for the one-dimensional case.
 
 ## Time Complexity
 
-- **2 clusters**: O(log(n))
-- (+ (O(n) for prefix sum calculation if not provided))
-- **k clusters**: O(k * 2 + log(k) * log(n) + max_iter * log(n) * k)  
-  (+ (O(n) for prefix sum calculation if not provided))
+For number of elements $n$, number of clusteres $k$, number of Lloyd's algorithm iterations $i$, and assuming one-dimensional data (which is the only case covered by this implementation):
 
-This is a significant improvement over the standard K-means algorithm, which has a time complexity of O(n * k * max_iter),
-even excluding the time complexity of the K-means++ initialization.
+- **2 clusters**: $O(\log{n})$  
+  ($+ O(n)$ for prefix sum calculation if not provided, $+ O(n \cdot \log {n})$ for sorting if not sorted)
+- **$k$ clusters**: $O(k ^ 2 \cdot \log {k} \cdot \log {n}) + O(i \cdot \log {n} \cdot k)$  
+  (The first term is for K-means++ initialization, and the latter for Lloyd's algorithm)  
+  ($+ O(n)$ for prefix sum calculation if not provided, $+ O(n \cdot \log {n})$ for sorting if not sorted)
+
+This is a significant improvement over common K-means implementations.
+For example, general implementations for $d$-dimensional data using a combination of greedy K-means++ initialization and Lloyd's algorithm for convergence,
+when given one-dimensional data, spends $O(k ^ 2 \cdot \log {k} \cdot n)$ time in initialization and $O(i \cdot n \cdot k)$ time in iterations.
+
+**Note that you must use the underlying `numba_` functions directly in order to directly supply prefix sums and skip sorting.**
 
 ## How fast is it?
 
 TODO: Comparision with sklearn's KMeans
 
 
 ## Installation
@@ -78,25 +91,27 @@
     data, k,
     sample_weights=weights,  # sample weights
     max_iter=100,  # maximum number of iterations
 )
 ```
 
 ### Even More Options
-The underlying Numba-accelerated function `_sorted_kmeans_1d` can be used directly for more control.
+The underlying Numba-accelerated function `numba_kmeans_1d_k_clusters` can be used directly for more control.
 
 This is useful when the algorithm is run multiple times on different segments of the data,
 or to use within another Numba-accelerated function.
 
 The list of available functions are as follows:
 - `numba_kmeans_1d_two_clusters`
 - `numba_kmeans_1d_two_clusters_unweighted`
 - `numba_kmeans_1d_k_cluster`
 - `numba_kmeans_1d_k_cluster_unweighted`
 
+All of these functions assume the data is sorted beforehand.
+
 ```python
 from flash1dkmeans import numba_kmeans_1d_k_cluster
 import numpy as np
 
 n, k = 1024, 4
 
 # Generate random data
@@ -112,18 +127,17 @@
 weighted_X_squared_prefix_sum = np.cumsum(data ** 2 * weights)
 
 middle_idx = n // 2
 
 # Providing prefix sums reduces redundant calculations
 # This is useful when the algorithm is run multiple times on different segments of the data
 for start_idx, stop_idx in [(0, middle_idx), (middle_idx, n)]:
-  centroids, cluster_borders = numba_kmeans_1d_k_cluster(
+  centroids, cluster_borders = numba_kmeans_1d_k_cluster(  # Note that data MUST be sorted beforehand
     data, k,  # Note how the sample weights are not provided when the prefix sums are provided
     max_iter=100,  # maximum number of iterations
-    is_sorted=True,
     weights_prefix_sum=weights_prefix_sum,  # prefix sum of the sample weights, leave empty for unwieghted data
     weighted_X_prefix_sum=weighted_X_prefix_sum,  # prefix sum of the weighted data
     weighted_X_squared_prefix_sum=weighted_X_squared_prefix_sum,  # prefix sum of the squared weighted data
     start_idx=start_idx,  # start index of the data
     stop_idx=stop_idx,  # stop index of the data
   )
 ```
@@ -133,7 +147,9 @@
 ## Notes
 
 This repository has been created to be used in [Any-Precision-LLM](https://github.com/SNU-ARC/any-precision-llm) project,
 where multiple 1D K-means instances are run in parallel for LLM quantization.
 
 However, the algorithm is general and can be used for any 1D K-means problem.
 
+I have proved the validity for the two cluster case - detailed version of the proof might be posted in the future.
+
```

