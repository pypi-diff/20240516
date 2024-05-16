# Comparing `tmp/gfagraphs-0.3.7.tar.gz` & `tmp/gfagraphs-0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gfagraphs-0.3.7.tar", last modified: Thu Apr 25 14:41:01 2024, max compression
+gzip compressed data, was "gfagraphs-0.3.8.tar", last modified: Thu May 16 14:24:37 2024, max compression
```

## Comparing `gfagraphs-0.3.7.tar` & `gfagraphs-0.3.8.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 sidubois (669136) genscale (35005)        0 2024-04-25 14:41:01.438296 gfagraphs-0.3.7/
--rw-r--r--   0 sidubois (669136) genscale (35005)    34521 2023-11-29 09:58:07.000000 gfagraphs-0.3.7/LICENSE
--rw-r--r--   0 sidubois (669136) genscale (35005)     2114 2024-04-25 14:41:01.438296 gfagraphs-0.3.7/PKG-INFO
--rw-r--r--   0 sidubois (669136) genscale (35005)     1491 2024-04-19 14:44:53.000000 gfagraphs-0.3.7/README.md
-drwxr-xr-x   0 sidubois (669136) genscale (35005)        0 2024-04-25 14:41:01.437296 gfagraphs-0.3.7/gfagraphs/
--rw-r--r--   0 sidubois (669136) genscale (35005)       58 2024-04-19 08:22:28.000000 gfagraphs-0.3.7/gfagraphs/__init__.py
--rw-r--r--   0 sidubois (669136) genscale (35005)    39616 2024-03-07 16:32:34.000000 gfagraphs-0.3.7/gfagraphs/gfagraphs.py
-drwxr-xr-x   0 sidubois (669136) genscale (35005)        0 2024-04-25 14:41:01.437296 gfagraphs-0.3.7/gfagraphs.egg-info/
--rw-r--r--   0 sidubois (669136) genscale (35005)     2114 2024-04-25 14:41:01.000000 gfagraphs-0.3.7/gfagraphs.egg-info/PKG-INFO
--rw-r--r--   0 sidubois (669136) genscale (35005)      365 2024-04-25 14:41:01.000000 gfagraphs-0.3.7/gfagraphs.egg-info/SOURCES.txt
--rw-r--r--   0 sidubois (669136) genscale (35005)        1 2024-04-25 14:41:01.000000 gfagraphs-0.3.7/gfagraphs.egg-info/dependency_links.txt
--rw-r--r--   0 sidubois (669136) genscale (35005)        1 2024-04-19 08:24:53.000000 gfagraphs-0.3.7/gfagraphs.egg-info/not-zip-safe
--rw-r--r--   0 sidubois (669136) genscale (35005)       19 2024-04-25 14:41:01.000000 gfagraphs-0.3.7/gfagraphs.egg-info/top_level.txt
-drwxr-xr-x   0 sidubois (669136) genscale (35005)        0 2024-04-25 14:41:01.437296 gfagraphs-0.3.7/pgGraphs/
--rw-r--r--   0 sidubois (669136) genscale (35005)      178 2024-04-23 16:35:16.000000 gfagraphs-0.3.7/pgGraphs/__init__.py
--rw-r--r--   0 sidubois (669136) genscale (35005)     1848 2024-04-24 12:08:52.000000 gfagraphs-0.3.7/pgGraphs/abstractions.py
--rw-r--r--   0 sidubois (669136) genscale (35005)    16812 2024-04-24 12:47:37.000000 gfagraphs-0.3.7/pgGraphs/gfaparser.py
--rw-r--r--   0 sidubois (669136) genscale (35005)    32461 2024-04-25 14:40:40.000000 gfagraphs-0.3.7/pgGraphs/graph.py
--rw-r--r--   0 sidubois (669136) genscale (35005)     6217 2024-04-19 09:42:36.000000 gfagraphs-0.3.7/pgGraphs/nx.py
--rw-r--r--   0 sidubois (669136) genscale (35005)      695 2024-04-25 14:41:01.000000 gfagraphs-0.3.7/pyproject.toml
--rw-r--r--   0 sidubois (669136) genscale (35005)       38 2024-04-25 14:41:01.438296 gfagraphs-0.3.7/setup.cfg
--rw-r--r--   0 sidubois (669136) genscale (35005)     2449 2024-04-25 14:40:51.000000 gfagraphs-0.3.7/setup.py
-drwxr-xr-x   0 sidubois (669136) genscale (35005)        0 2024-04-25 14:41:01.437296 gfagraphs-0.3.7/tests/
--rw-r--r--   0 sidubois (669136) genscale (35005)      536 2024-04-25 12:43:00.000000 gfagraphs-0.3.7/tests/test.py
+drwxr-xr-x   0 sidubois (669136) genscale (35005)        0 2024-05-16 14:24:37.079153 gfagraphs-0.3.8/
+-rw-r--r--   0 sidubois (669136) genscale (35005)    34521 2023-11-29 09:58:07.000000 gfagraphs-0.3.8/LICENSE
+-rw-r--r--   0 sidubois (669136) genscale (35005)     2114 2024-05-16 14:24:37.079153 gfagraphs-0.3.8/PKG-INFO
+-rw-r--r--   0 sidubois (669136) genscale (35005)     1491 2024-04-19 14:44:53.000000 gfagraphs-0.3.8/README.md
+drwxr-xr-x   0 sidubois (669136) genscale (35005)        0 2024-05-16 14:24:37.079153 gfagraphs-0.3.8/gfagraphs/
+-rw-r--r--   0 sidubois (669136) genscale (35005)       58 2024-04-19 08:22:28.000000 gfagraphs-0.3.8/gfagraphs/__init__.py
+-rw-r--r--   0 sidubois (669136) genscale (35005)    39616 2024-03-07 16:32:34.000000 gfagraphs-0.3.8/gfagraphs/gfagraphs.py
+drwxr-xr-x   0 sidubois (669136) genscale (35005)        0 2024-05-16 14:24:37.079153 gfagraphs-0.3.8/gfagraphs.egg-info/
+-rw-r--r--   0 sidubois (669136) genscale (35005)     2114 2024-05-16 14:24:37.000000 gfagraphs-0.3.8/gfagraphs.egg-info/PKG-INFO
+-rw-r--r--   0 sidubois (669136) genscale (35005)      365 2024-05-16 14:24:37.000000 gfagraphs-0.3.8/gfagraphs.egg-info/SOURCES.txt
+-rw-r--r--   0 sidubois (669136) genscale (35005)        1 2024-05-16 14:24:37.000000 gfagraphs-0.3.8/gfagraphs.egg-info/dependency_links.txt
+-rw-r--r--   0 sidubois (669136) genscale (35005)        1 2024-04-19 08:24:53.000000 gfagraphs-0.3.8/gfagraphs.egg-info/not-zip-safe
+-rw-r--r--   0 sidubois (669136) genscale (35005)       19 2024-05-16 14:24:37.000000 gfagraphs-0.3.8/gfagraphs.egg-info/top_level.txt
+drwxr-xr-x   0 sidubois (669136) genscale (35005)        0 2024-05-16 14:24:37.079153 gfagraphs-0.3.8/pgGraphs/
+-rw-r--r--   0 sidubois (669136) genscale (35005)      178 2024-04-23 16:35:16.000000 gfagraphs-0.3.8/pgGraphs/__init__.py
+-rw-r--r--   0 sidubois (669136) genscale (35005)     1848 2024-04-24 12:08:52.000000 gfagraphs-0.3.8/pgGraphs/abstractions.py
+-rw-r--r--   0 sidubois (669136) genscale (35005)    16812 2024-04-24 12:47:37.000000 gfagraphs-0.3.8/pgGraphs/gfaparser.py
+-rw-r--r--   0 sidubois (669136) genscale (35005)    31680 2024-05-16 14:18:06.000000 gfagraphs-0.3.8/pgGraphs/graph.py
+-rw-r--r--   0 sidubois (669136) genscale (35005)     6217 2024-04-19 09:42:36.000000 gfagraphs-0.3.8/pgGraphs/nx.py
+-rw-r--r--   0 sidubois (669136) genscale (35005)      695 2024-05-16 14:24:37.000000 gfagraphs-0.3.8/pyproject.toml
+-rw-r--r--   0 sidubois (669136) genscale (35005)       38 2024-05-16 14:24:37.079153 gfagraphs-0.3.8/setup.cfg
+-rw-r--r--   0 sidubois (669136) genscale (35005)     2449 2024-05-16 14:24:18.000000 gfagraphs-0.3.8/setup.py
+drwxr-xr-x   0 sidubois (669136) genscale (35005)        0 2024-05-16 14:24:37.079153 gfagraphs-0.3.8/tests/
+-rw-r--r--   0 sidubois (669136) genscale (35005)      536 2024-04-25 12:43:00.000000 gfagraphs-0.3.8/tests/test.py
```

### Comparing `gfagraphs-0.3.7/LICENSE` & `gfagraphs-0.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `gfagraphs-0.3.7/PKG-INFO` & `gfagraphs-0.3.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gfagraphs
-Version: 0.3.7
+Version: 0.3.8
 Summary: Library to parse, edit and handle in memory GFA graphs
 Home-page: https://github.com/Tharos-ux/gfagraphs
 Author: ('Siegfried Dubois',)
 Author-email: Siegfried Dubois <siegfried.dubois@inria.fr>
 Project-URL: Homepage, https://github.com/Tharos-ux/gfagraphs
 Project-URL: Bug Tracker, https://github.com/Tharos-ux/gfagraphs/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `gfagraphs-0.3.7/README.md` & `gfagraphs-0.3.8/README.md`

 * *Files identical despite different names*

### Comparing `gfagraphs-0.3.7/gfagraphs/gfagraphs.py` & `gfagraphs-0.3.8/gfagraphs/gfagraphs.py`

 * *Files identical despite different names*

### Comparing `gfagraphs-0.3.7/gfagraphs.egg-info/PKG-INFO` & `gfagraphs-0.3.8/gfagraphs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gfagraphs
-Version: 0.3.7
+Version: 0.3.8
 Summary: Library to parse, edit and handle in memory GFA graphs
 Home-page: https://github.com/Tharos-ux/gfagraphs
 Author: ('Siegfried Dubois',)
 Author-email: Siegfried Dubois <siegfried.dubois@inria.fr>
 Project-URL: Homepage, https://github.com/Tharos-ux/gfagraphs
 Project-URL: Bug Tracker, https://github.com/Tharos-ux/gfagraphs/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `gfagraphs-0.3.7/pgGraphs/abstractions.py` & `gfagraphs-0.3.8/pgGraphs/abstractions.py`

 * *Files identical despite different names*

### Comparing `gfagraphs-0.3.7/pgGraphs/gfaparser.py` & `gfagraphs-0.3.8/pgGraphs/gfaparser.py`

 * *Files identical despite different names*

### Comparing `gfagraphs-0.3.7/pgGraphs/graph.py` & `gfagraphs-0.3.8/pgGraphs/graph.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,34 +74,28 @@
                             self.segments[name] = datas
                         case GFALine.WALK | GFALine.PATH:
                             self.paths[name] = datas
                         case GFALine.LINE:
                             if name not in self.lines:
                                 self.lines[name] = datas
                             else:
-                                try:
-                                    self.lines[name]['orientation'] = self.lines[name].get(
-                                        'orientation',
-                                        {}
-                                    ) | datas['orientation']
-                                except TypeError:
-                                    print(name, self.lines[name].get(
-                                        'orientation', {}), datas['orientation'])
+                                [_ors,] = datas['orientation']
+                                self.lines[name]['orientation'].add(
+                                    (_ors[0], _ors[1]))
                             if with_reverse_edges:
                                 if name[::-1] not in self.lines:
                                     [_ors,] = datas['orientation']
                                     self.lines[name[::-1]] = {
                                         'orientation': set(
                                             [(reverse(_ors[1]), reverse(_ors[0]))]
                                         )
                                     }
-                                    self.lines[name[::-1]]
                                 else:
-                                    self.lines[name[::-1]]['orientation'] = self.lines[name[::-1]].get(
-                                        'orientation', set()) | set([(reverse(_ors[1]), reverse(_ors[0]))])
+                                    self.lines[name[::-1]]['orientation'].add(
+                                        (reverse(_ors[1]), reverse(_ors[0])))
 
                         case GFALine.HEADER:
                             self.headers.append(datas)
                         case _:
                             pass
 
     def __str__(self) -> str:
@@ -594,24 +588,18 @@
             }
             self.segments[node]['in'] = {
                 Orientation.FORWARD: set(),
                 Orientation.REVERSE: set(),
             }
         for (from_node, to_node), datas in self.lines.items():
             for from_orientation, to_orientation in datas['orientation']:
-                if from_orientation == Orientation.FORWARD:
-                    self.segments[from_node]['out'][Orientation.FORWARD].add(
-                        (to_node, to_orientation))
-                    self.segments[to_node]['in'][Orientation.FORWARD].add(
-                        (from_node, from_orientation))
-                else:
-                    self.segments[from_node]['out'][Orientation.REVERSE].add(
-                        (to_node, to_orientation))
-                    self.segments[to_node]['in'][Orientation.REVERSE].add(
-                        (from_node, from_orientation))
+                self.segments[from_node]['out'][from_orientation].add(
+                    (to_node, to_orientation))
+                self.segments[to_node]['in'][to_orientation].add(
+                    (from_node, from_orientation))
 
     def compute_neighbors(self) -> None:
         """
         Computes both predecessors and successors
         This function is O(n) with n being the number of edges.
         """
         for node in self.segments.keys():
```

### Comparing `gfagraphs-0.3.7/pgGraphs/nx.py` & `gfagraphs-0.3.8/pgGraphs/nx.py`

 * *Files identical despite different names*

### Comparing `gfagraphs-0.3.7/pyproject.toml` & `gfagraphs-0.3.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
     requires = ["setuptools>=61.0"]
     build-backend = "setuptools.build_meta"
 
     [project]
     name = "gfagraphs"
-    version = "0.3.7"
+    version = "0.3.8"
     authors = [
     { name="Siegfried Dubois", email="siegfried.dubois@inria.fr" },
     ]
     description = "Library to parse, edit and handle in memory GFA graphs"
     readme = "README.md"
     requires-python = ">=3.10"
     classifiers = [
```

### Comparing `gfagraphs-0.3.7/setup.py` & `gfagraphs-0.3.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 NAME: str = "gfagraphs"
 AUTHOR: str = "Siegfried Dubois",
 AUTHOR_EMAIL: str = "siegfried.dubois@inria.fr",
 LICENCE: str = "LICENCE"
 DESCRIPTION: str = "Library to parse, edit and handle in memory GFA graphs"
 REQUIRED_PYTHON: tuple = (3, 10)
 OVERRIDE_VN: bool = True
-VN: str = "0.3.7"
+VN: str = "0.3.8"
 URL: str = "https://github.com/Tharos-ux/gfagraphs"
 REQUIREMENTS: list[str] = [
     'networkx',
     'tharos-pytools',
     'matplotlib',
     'mycolorpy',
 ]
```

### Comparing `gfagraphs-0.3.7/tests/test.py` & `gfagraphs-0.3.8/tests/test.py`

 * *Files identical despite different names*

