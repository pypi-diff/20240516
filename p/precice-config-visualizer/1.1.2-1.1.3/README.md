# Comparing `tmp/precice_config_visualizer-1.1.2.tar.gz` & `tmp/precice_config_visualizer-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "precice_config_visualizer-1.1.2.tar", last modified: Wed Apr 17 08:25:13 2024, max compression
+gzip compressed data, was "precice_config_visualizer-1.1.3.tar", last modified: Wed Apr 17 08:44:56 2024, max compression
```

## Comparing `precice_config_visualizer-1.1.2.tar` & `precice_config_visualizer-1.1.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 08:25:13.175918 precice_config_visualizer-1.1.2/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-17 08:25:01.000000 precice_config_visualizer-1.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3388 2024-04-17 08:25:13.175918 precice_config_visualizer-1.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2195 2024-04-17 08:25:01.000000 precice_config_visualizer-1.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 08:25:13.175918 precice_config_visualizer-1.1.2/precice_config_visualizer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3388 2024-04-17 08:25:13.000000 precice_config_visualizer-1.1.2/precice_config_visualizer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      402 2024-04-17 08:25:13.000000 precice_config_visualizer-1.1.2/precice_config_visualizer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 08:25:13.000000 precice_config_visualizer-1.1.2/precice_config_visualizer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-17 08:25:13.000000 precice_config_visualizer-1.1.2/precice_config_visualizer.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-17 08:25:13.000000 precice_config_visualizer-1.1.2/precice_config_visualizer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-17 08:25:13.000000 precice_config_visualizer-1.1.2/precice_config_visualizer.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 08:25:13.175918 precice_config_visualizer-1.1.2/preciceconfigvisualizer/
--rwxr-xr-x   0 runner    (1001) docker     (127)     2452 2024-04-17 08:25:01.000000 precice_config_visualizer-1.1.2/preciceconfigvisualizer/cli.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    15627 2024-04-17 08:25:01.000000 precice_config_visualizer-1.1.2/preciceconfigvisualizer/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-04-17 08:25:01.000000 precice_config_visualizer-1.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 08:25:13.175918 precice_config_visualizer-1.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 08:25:01.000000 precice_config_visualizer-1.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 08:44:56.195321 precice_config_visualizer-1.1.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-17 08:44:47.000000 precice_config_visualizer-1.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3388 2024-04-17 08:44:56.195321 precice_config_visualizer-1.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2195 2024-04-17 08:44:47.000000 precice_config_visualizer-1.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 08:44:56.195321 precice_config_visualizer-1.1.3/precice_config_visualizer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3388 2024-04-17 08:44:56.000000 precice_config_visualizer-1.1.3/precice_config_visualizer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-04-17 08:44:56.000000 precice_config_visualizer-1.1.3/precice_config_visualizer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 08:44:56.000000 precice_config_visualizer-1.1.3/precice_config_visualizer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-17 08:44:56.000000 precice_config_visualizer-1.1.3/precice_config_visualizer.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-17 08:44:56.000000 precice_config_visualizer-1.1.3/precice_config_visualizer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-17 08:44:56.000000 precice_config_visualizer-1.1.3/precice_config_visualizer.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 08:44:56.195321 precice_config_visualizer-1.1.3/preciceconfigvisualizer/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2532 2024-04-17 08:44:47.000000 precice_config_visualizer-1.1.3/preciceconfigvisualizer/cli.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    15652 2024-04-17 08:44:47.000000 precice_config_visualizer-1.1.3/preciceconfigvisualizer/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-04-17 08:44:47.000000 precice_config_visualizer-1.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 08:44:56.195321 precice_config_visualizer-1.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 08:44:47.000000 precice_config_visualizer-1.1.3/setup.py
```

### Comparing `precice_config_visualizer-1.1.2/LICENSE` & `precice_config_visualizer-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `precice_config_visualizer-1.1.2/PKG-INFO` & `precice_config_visualizer-1.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: precice-config-visualizer
-Version: 1.1.2
+Version: 1.1.3
 Summary: A tool for visualizing a preCICE configuration file as a dot file.
 Author-email: The preCICE Developers <info@precice.org>
 Maintainer-email: Frédéric Simonis <frederic.simonis@ipvs.uni-stuttgart.de>
 License: GPLv3
 Project-URL: Homepage, https://precice.org
 Project-URL: Documentation, https://precice.org/tooling-config-visualization.html
 Project-URL: Repository, https://github.com/precice/config-visualizer.git
```

### Comparing `precice_config_visualizer-1.1.2/README.md` & `precice_config_visualizer-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `precice_config_visualizer-1.1.2/precice_config_visualizer.egg-info/PKG-INFO` & `precice_config_visualizer-1.1.3/precice_config_visualizer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: precice-config-visualizer
-Version: 1.1.2
+Version: 1.1.3
 Summary: A tool for visualizing a preCICE configuration file as a dot file.
 Author-email: The preCICE Developers <info@precice.org>
 Maintainer-email: Frédéric Simonis <frederic.simonis@ipvs.uni-stuttgart.de>
 License: GPLv3
 Project-URL: Homepage, https://precice.org
 Project-URL: Documentation, https://precice.org/tooling-config-visualization.html
 Project-URL: Repository, https://github.com/precice/config-visualizer.git
```

### Comparing `precice_config_visualizer-1.1.2/preciceconfigvisualizer/cli.py` & `precice_config_visualizer-1.1.3/preciceconfigvisualizer/cli.py`

 * *Files 8% similar despite different names*

```diff
@@ -82,12 +82,13 @@
     dot = configFileToDotCode(args.infile, **vars(args))
 
     ext = os.path.splitext(args.outfile.name)[1].lower().lstrip(".")
     if ext in SUPPORTED_FORMATS:
         g = pydot.graph_from_dot_data(dot)[0]
         args.outfile.write(g.create(format=ext))
     else:
+        # sys.stdout is always in utf-8 mode, so we do the same for the outfile
         args.outfile.write(dot)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `precice_config_visualizer-1.1.2/preciceconfigvisualizer/common.py` & `precice_config_visualizer-1.1.3/preciceconfigvisualizer/common.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from collections import defaultdict
 from itertools import cycle
 
 import pydot
 from lxml import etree
 
 
-from typing import Literal, TypedDict
+from typing import Literal, TypedDict, Union, List, Dict
 
 if sys.version_info < (3, 11):
     from typing_extensions import Unpack
 else:
     from typing import Unpack
 
 
@@ -69,29 +69,29 @@
         if es == src and ed == dst:
             return e
     e = pydot.Edge(quote(src), quote(dst), **attrs)
     g.add_edge(e)
     return e
 
 
-def getEdge(g: pydot.Graph, src: str, dst: str) -> pydot.Edge | None:
+def getEdge(g: pydot.Graph, src: str, dst: str) -> Union[pydot.Edge, None]:
     for e in g.get_edge_list():
         es, ed = e.get_source().strip('"'), e.get_destination().strip('"')
         if es == src and ed == dst:
             return e
     return None
 
 
-def getParticipantNames(solverinterface: etree._Element) -> list[str]:
+def getParticipantNames(solverinterface: etree._Element) -> List[str]:
     return [p.attrib["name"] for p in solverinterface.findall("participant")]
 
 
 def getParticipantColor(
     solverinterface: str, use_colors: bool = False
-) -> dict[str, str]:
+) -> Dict[str, str]:
     names = getParticipantNames(solverinterface)
     colors = None
     if not use_colors:
         colors = cycle(["black"])
     else:
         colorblind = [
             "#0173B2",
```

### Comparing `precice_config_visualizer-1.1.2/pyproject.toml` & `precice_config_visualizer-1.1.3/pyproject.toml`

 * *Files identical despite different names*

