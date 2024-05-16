# Comparing `tmp/coscine-0.9.4.tar.gz` & `tmp/coscine-0.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/coscine-0.9.4.tar", last modified: Mon Jul 10 19:03:18 2023, max compression
+gzip compressed data, was "dist/coscine-0.9.5.tar", last modified: Fri Sep  1 14:19:26 2023, max compression
```

## Comparing `coscine-0.9.4.tar` & `coscine-0.9.5.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 19:03:18.000000 coscine-0.9.4/
--rw-rw-rw-   0 root         (0) root         (0)     1084 2023-04-11 13:11:08.000000 coscine-0.9.4/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)     7001 2023-07-10 19:03:18.000000 coscine-0.9.4/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     5471 2023-07-10 19:00:16.000000 coscine-0.9.4/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-10 19:03:18.000000 coscine-0.9.4/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     3905 2023-04-11 13:11:08.000000 coscine-0.9.4/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 19:03:18.000000 coscine-0.9.4/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 19:03:18.000000 coscine-0.9.4/src/coscine/
--rw-rw-rw-   0 root         (0) root         (0)     2954 2023-07-10 19:00:16.000000 coscine-0.9.4/src/coscine/__about__.py
--rw-rw-rw-   0 root         (0) root         (0)     2231 2023-04-11 13:11:08.000000 coscine-0.9.4/src/coscine/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6267 2023-04-11 13:11:08.000000 coscine-0.9.4/src/coscine/cache.py
--rw-rw-rw-   0 root         (0) root         (0)    24288 2023-04-11 13:11:08.000000 coscine-0.9.4/src/coscine/client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 19:03:18.000000 coscine-0.9.4/src/coscine/data/
--rw-rw-rw-   0 root         (0) root         (0)     1991 2023-04-11 13:11:08.000000 coscine-0.9.4/src/coscine/data/project.json
--rw-rw-rw-   0 root         (0) root         (0)     2029 2023-04-11 13:11:08.000000 coscine-0.9.4/src/coscine/data/resource.json
--rw-rw-rw-   0 root         (0) root         (0)     2276 2023-04-11 13:11:08.000000 coscine-0.9.4/src/coscine/defaults.py
--rw-rw-rw-   0 root         (0) root         (0)    28689 2023-07-10 19:00:16.000000 coscine-0.9.4/src/coscine/form.py
--rw-rw-rw-   0 root         (0) root         (0)     6907 2023-06-22 14:06:09.000000 coscine-0.9.4/src/coscine/graph.py
--rw-rw-rw-   0 root         (0) root         (0)    19265 2023-06-22 14:06:09.000000 coscine-0.9.4/src/coscine/object.py
--rw-rw-rw-   0 root         (0) root         (0)    21761 2023-04-11 13:11:08.000000 coscine-0.9.4/src/coscine/project.py
--rw-rw-rw-   0 root         (0) root         (0)    26362 2023-04-11 13:46:13.000000 coscine-0.9.4/src/coscine/resource.py
--rw-rw-rw-   0 root         (0) root         (0)     7402 2023-04-11 13:11:08.000000 coscine-0.9.4/src/coscine/s3.py
--rw-rw-rw-   0 root         (0) root         (0)    11884 2023-04-11 13:11:08.000000 coscine-0.9.4/src/coscine/utils.py
--rw-rw-rw-   0 root         (0) root         (0)    14870 2023-04-11 13:11:08.000000 coscine-0.9.4/src/coscine/vocabulary.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 19:03:18.000000 coscine-0.9.4/src/coscine.egg-info/
--rw-r--r--   0 root         (0) root         (0)     7001 2023-07-10 19:03:18.000000 coscine-0.9.4/src/coscine.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      556 2023-07-10 19:03:18.000000 coscine-0.9.4/src/coscine.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-10 19:03:18.000000 coscine-0.9.4/src/coscine.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       84 2023-07-10 19:03:18.000000 coscine-0.9.4/src/coscine.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-07-10 19:03:18.000000 coscine-0.9.4/src/coscine.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-01 14:19:26.000000 coscine-0.9.5/
+-rw-rw-rw-   0 root         (0) root         (0)     1084 2023-04-11 13:11:08.000000 coscine-0.9.5/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)     7001 2023-09-01 14:19:26.000000 coscine-0.9.5/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     5471 2023-07-10 19:00:16.000000 coscine-0.9.5/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-09-01 14:19:26.000000 coscine-0.9.5/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     3905 2023-04-11 13:11:08.000000 coscine-0.9.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-01 14:19:26.000000 coscine-0.9.5/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-01 14:19:26.000000 coscine-0.9.5/src/coscine/
+-rw-rw-rw-   0 root         (0) root         (0)     2868 2023-09-01 14:17:25.000000 coscine-0.9.5/src/coscine/__about__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2231 2023-04-11 13:11:08.000000 coscine-0.9.5/src/coscine/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6267 2023-04-11 13:11:08.000000 coscine-0.9.5/src/coscine/cache.py
+-rw-rw-rw-   0 root         (0) root         (0)    24288 2023-04-11 13:11:08.000000 coscine-0.9.5/src/coscine/client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-01 14:19:26.000000 coscine-0.9.5/src/coscine/data/
+-rw-rw-rw-   0 root         (0) root         (0)     1991 2023-04-11 13:11:08.000000 coscine-0.9.5/src/coscine/data/project.json
+-rw-rw-rw-   0 root         (0) root         (0)     2029 2023-04-11 13:11:08.000000 coscine-0.9.5/src/coscine/data/resource.json
+-rw-rw-rw-   0 root         (0) root         (0)     2276 2023-04-11 13:11:08.000000 coscine-0.9.5/src/coscine/defaults.py
+-rw-rw-rw-   0 root         (0) root         (0)    28752 2023-09-01 14:17:25.000000 coscine-0.9.5/src/coscine/form.py
+-rw-rw-rw-   0 root         (0) root         (0)     7747 2023-09-01 14:17:25.000000 coscine-0.9.5/src/coscine/graph.py
+-rw-rw-rw-   0 root         (0) root         (0)    19265 2023-06-22 14:06:09.000000 coscine-0.9.5/src/coscine/object.py
+-rw-rw-rw-   0 root         (0) root         (0)    21761 2023-04-11 13:11:08.000000 coscine-0.9.5/src/coscine/project.py
+-rw-rw-rw-   0 root         (0) root         (0)    26362 2023-04-11 13:46:13.000000 coscine-0.9.5/src/coscine/resource.py
+-rw-rw-rw-   0 root         (0) root         (0)     7402 2023-04-11 13:11:08.000000 coscine-0.9.5/src/coscine/s3.py
+-rw-rw-rw-   0 root         (0) root         (0)    11884 2023-04-11 13:11:08.000000 coscine-0.9.5/src/coscine/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)    14883 2023-09-01 14:17:25.000000 coscine-0.9.5/src/coscine/vocabulary.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-01 14:19:26.000000 coscine-0.9.5/src/coscine.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     7001 2023-09-01 14:19:26.000000 coscine-0.9.5/src/coscine.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      556 2023-09-01 14:19:26.000000 coscine-0.9.5/src/coscine.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-09-01 14:19:26.000000 coscine-0.9.5/src/coscine.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       84 2023-09-01 14:19:26.000000 coscine-0.9.5/src/coscine.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-09-01 14:19:26.000000 coscine-0.9.5/src/coscine.egg-info/top_level.txt
```

### Comparing `coscine-0.9.4/LICENSE.txt` & `coscine-0.9.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `coscine-0.9.4/PKG-INFO` & `coscine-0.9.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coscine
-Version: 0.9.4
+Version: 0.9.5
 Summary: The Coscine Python SDK provides a pythonic interface to the Coscine REST API.
 Home-page: https://git.rwth-aachen.de/coscine/community-features/coscine-python-sdk/
 Author: RWTH Aachen University
 Author-email: coscine@itc.rwth-aachen.de
 License: MIT License
 Project-URL: Issues, https://git.rwth-aachen.de/coscine/community-features/coscine-python-sdk/-/issues
 Project-URL: Documentation, https://coscine.pages.rwth-aachen.de/community-features/coscine-python-sdk/
```

### Comparing `coscine-0.9.4/README.md` & `coscine-0.9.5/README.md`

 * *Files identical despite different names*

### Comparing `coscine-0.9.4/setup.py` & `coscine-0.9.5/setup.py`

 * *Files identical despite different names*

### Comparing `coscine-0.9.4/src/coscine/__about__.py` & `coscine-0.9.5/src/coscine/__about__.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,86 +1,86 @@
-###############################################################################
-# Coscine Python SDK
-# Copyright (c) 2018-2023 RWTH Aachen University
-# Licensed under the terms of the MIT License
-###############################################################################
-# Coscine, short for Collaborative Scientific Integration Environment, is
-# a platform for research data management (RDM).
-# For more information on Coscine visit https://www.coscine.de/.
-#
-# Please note that this python module is open source software primarily
-# developed and maintained by the scientific community. It is not
-# an official service that RWTH Aachen provides support for.
-###############################################################################
-
-###############################################################################
-# File description
-###############################################################################
-
-"""
-This file contains package metadata primarily intended for setup.py but
-also accessed by various source files in src/.
-"""
-
-###############################################################################
-# Module globals / Constants
-###############################################################################
-
-# Package title/name as it would appear in PyPi
-__title__ = "coscine"
-
-# Current package version
-# Do not set version to 1.0.0 before update to Coscine API version 2
-__version__ = "0.9.4"
-
-# Short package description
-__summary__ = (
-    "The Coscine Python SDK provides a pythonic interface to "
-    "the Coscine REST API."
-)
-
-# Package copyright owner
-__author__ = "RWTH Aachen University"
-
-# Coscine contact (Note: This is the official Coscine contact email!)
-# Only for copyright claims, licensing issues or sourcecode hosting!
-# Please do not direct bug reports or feature requests to that address!
-# They are not responsible for the development, they "just" represent Coscine!
-__contact__ = "coscine@itc.rwth-aachen.de"
-
-# Package license
-__license__ = "MIT License"
-
-# Package keywords/tags (must be given as a list!)
-__keywords__ = ["Coscine", "RWTH Aachen", "Research Data Management"]
-
-# Package dependencies (must be given as a list!)
-__dependencies__ = [
-    "rdflib",
-    "requests",
-    "requests-toolbelt",
-    "tqdm",
-    "colorama",
-    "prettytable",
-    "appdirs",
-    "python-dateutil"
-]
-
-# Python version required
-__pyver__ = ">=3.7"
-
-# Project url (official sourcecode hosting)
-__url__ = (
-    "https://git.rwth-aachen.de/coscine/community-features/"
-    "coscine-python-sdk/"
-)
-
-# Additional urls for e.g. bug reports and documentation
-__project_urls__ = {
-    "Issues": __url__ + "-/issues",
-    "Documentation": (
-        "https://coscine.pages.rwth-aachen.de/"
-        "community-features/coscine-python-sdk/"
-    )
-}
-
-###############################################################################
+###############################################################################
+# Coscine Python SDK
+# Copyright (c) 2018-2023 RWTH Aachen University
+# Licensed under the terms of the MIT License
+###############################################################################
+# Coscine, short for Collaborative Scientific Integration Environment, is
+# a platform for research data management (RDM).
+# For more information on Coscine visit https://www.coscine.de/.
+#
+# Please note that this python module is open source software primarily
+# developed and maintained by the scientific community. It is not
+# an official service that RWTH Aachen provides support for.
+###############################################################################
+
+###############################################################################
+# File description
+###############################################################################
+
+"""
+This file contains package metadata primarily intended for setup.py but
+also accessed by various source files in src/.
+"""
+
+###############################################################################
+# Module globals / Constants
+###############################################################################
+
+# Package title/name as it would appear in PyPi
+__title__ = "coscine"
+
+# Current package version
+# Do not set version to 1.0.0 before update to Coscine API version 2
+__version__ = "0.9.5"
+
+# Short package description
+__summary__ = (
+    "The Coscine Python SDK provides a pythonic interface to "
+    "the Coscine REST API."
+)
+
+# Package copyright owner
+__author__ = "RWTH Aachen University"
+
+# Coscine contact (Note: This is the official Coscine contact email!)
+# Only for copyright claims, licensing issues or sourcecode hosting!
+# Please do not direct bug reports or feature requests to that address!
+# They are not responsible for the development, they "just" represent Coscine!
+__contact__ = "coscine@itc.rwth-aachen.de"
+
+# Package license
+__license__ = "MIT License"
+
+# Package keywords/tags (must be given as a list!)
+__keywords__ = ["Coscine", "RWTH Aachen", "Research Data Management"]
+
+# Package dependencies (must be given as a list!)
+__dependencies__ = [
+    "rdflib",
+    "requests",
+    "requests-toolbelt",
+    "tqdm",
+    "colorama",
+    "prettytable",
+    "appdirs",
+    "python-dateutil"
+]
+
+# Python version required
+__pyver__ = ">=3.7"
+
+# Project url (official sourcecode hosting)
+__url__ = (
+    "https://git.rwth-aachen.de/coscine/community-features/"
+    "coscine-python-sdk/"
+)
+
+# Additional urls for e.g. bug reports and documentation
+__project_urls__ = {
+    "Issues": __url__ + "-/issues",
+    "Documentation": (
+        "https://coscine.pages.rwth-aachen.de/"
+        "community-features/coscine-python-sdk/"
+    )
+}
+
+###############################################################################
```

### Comparing `coscine-0.9.4/src/coscine/__init__.py` & `coscine-0.9.5/src/coscine/__init__.py`

 * *Files identical despite different names*

### Comparing `coscine-0.9.4/src/coscine/cache.py` & `coscine-0.9.5/src/coscine/cache.py`

 * *Files identical despite different names*

### Comparing `coscine-0.9.4/src/coscine/client.py` & `coscine-0.9.5/src/coscine/client.py`

 * *Files identical despite different names*

### Comparing `coscine-0.9.4/src/coscine/data/project.json` & `coscine-0.9.5/src/coscine/data/project.json`

 * *Files identical despite different names*

### Comparing `coscine-0.9.4/src/coscine/data/resource.json` & `coscine-0.9.5/src/coscine/data/resource.json`

 * *Files identical despite different names*

### Comparing `coscine-0.9.4/src/coscine/defaults.py` & `coscine-0.9.5/src/coscine/defaults.py`

 * *Files identical despite different names*

### Comparing `coscine-0.9.4/src/coscine/form.py` & `coscine-0.9.5/src/coscine/form.py`

 * *Files 0% similar despite different names*

```diff
@@ -567,14 +567,15 @@
         """
         return list(zip(self.keys(), self.values()))
 
 ###############################################################################
 
     @staticmethod
     def _xsd_typeof(xsd_type: str) -> type:
+        if xsd_type is None: return str  # Be more permissive
         if xsd_type.startswith("xsd:"):
             xsd_type = xsd_type[4:]
         for item in XSD_TYPES.values():
             if xsd_type in item["values"]:
                 return item["type"]
         return str
```

### Comparing `coscine-0.9.4/src/coscine/graph.py` & `coscine-0.9.5/src/coscine/graph.py`

 * *Files 10% similar despite different names*

```diff
@@ -23,16 +23,18 @@
 """
 
 ###############################################################################
 # Dependencies
 ###############################################################################
 
 from __future__ import annotations
-from typing import Dict, List
+from typing import TYPE_CHECKING, Dict, List
 import rdflib
+if TYPE_CHECKING:
+    from coscine.client import Client
 
 ###############################################################################
 # Classes / Functions / Scripts
 ###############################################################################
 
 class ApplicationProfile:
     """
@@ -46,35 +48,54 @@
     ----------
     graph : rdflib.Graph
         An rdf graph parsed with the help of rdflib
     RDFTYPE : str
         A variable frequently used by methods of this class.
     """
 
+    client: Client
     graph: rdflib.Graph
     RDFTYPE: str = "http://www.w3.org/1999/02/22-rdf-syntax-ns#type"
 
 ###############################################################################
 
-    def __init__(self, graph: str, format: str = "json-ld") -> None:
+    def __init__(self, client: Client, graph: str, format: str = "json-ld") -> None:
         """
         Initializes an instance of the ApplicationProfile wrapper class.
 
         Parameters
         ----------
         graph : str
             A Coscine application profile rdf graph in json-ld text format.
         format : str (optional), default: "json-ld"
             The format of the graph
         """
 
+        self.client = client
         self.graph = rdflib.Graph()
         self.graph.bind("sh", "http://www.w3.org/ns/shacl#")
         self.graph.bind("dcterms", "http://purl.org/dc/terms/")
         self.graph.parse(data=graph, format=format)
+        self._recursive_import()
+
+###############################################################################
+
+    def _recursive_import(self):
+        """
+        Imports parent application profiles
+        TODO: Import after importing (actually recurse)
+        Currently we just iterate over owl:imports once,
+        but after importing new profiles, new owl:imports
+        may have appeared in the graph...
+        """
+        query = "SELECT ?url WHERE { ?_ owl:imports ?url . }"
+        for result in self.graph.query(query):
+            url = str(result[0])
+            profile = self.client.vocabularies.application_profile(url)
+            self.graph.parse(data=str(profile), format="ttl")
 
 ###############################################################################
 
     def __str__(self) -> str:
         """
         Serializes the application profile rdf graph used internally
         for easy output to stdout.
```

### Comparing `coscine-0.9.4/src/coscine/object.py` & `coscine-0.9.5/src/coscine/object.py`

 * *Files identical despite different names*

### Comparing `coscine-0.9.4/src/coscine/project.py` & `coscine-0.9.5/src/coscine/project.py`

 * *Files identical despite different names*

### Comparing `coscine-0.9.4/src/coscine/resource.py` & `coscine-0.9.5/src/coscine/resource.py`

 * *Files identical despite different names*

### Comparing `coscine-0.9.4/src/coscine/s3.py` & `coscine-0.9.5/src/coscine/s3.py`

 * *Files identical despite different names*

### Comparing `coscine-0.9.4/src/coscine/utils.py` & `coscine-0.9.5/src/coscine/utils.py`

 * *Files identical despite different names*

### Comparing `coscine-0.9.4/src/coscine/vocabulary.py` & `coscine-0.9.5/src/coscine/vocabulary.py`

 * *Files 1% similar despite different names*

```diff
@@ -324,15 +324,15 @@
         ApplicationProfile
             A parsed application profile.
         """
 
         uri = self.client.uri("Metadata", "Metadata", "profiles", path)
         data = self.client.static_request(uri)
         graph = json.dumps(data[0]["@graph"])
-        return ApplicationProfile(graph)
+        return ApplicationProfile(self.client, graph)
 
 ###############################################################################
 
     def instance(self, link: str) -> Vocabulary:
         """
         Retrieves a data instance. Instances are always normalized.
```

### Comparing `coscine-0.9.4/src/coscine.egg-info/PKG-INFO` & `coscine-0.9.5/src/coscine.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coscine
-Version: 0.9.4
+Version: 0.9.5
 Summary: The Coscine Python SDK provides a pythonic interface to the Coscine REST API.
 Home-page: https://git.rwth-aachen.de/coscine/community-features/coscine-python-sdk/
 Author: RWTH Aachen University
 Author-email: coscine@itc.rwth-aachen.de
 License: MIT License
 Project-URL: Issues, https://git.rwth-aachen.de/coscine/community-features/coscine-python-sdk/-/issues
 Project-URL: Documentation, https://coscine.pages.rwth-aachen.de/community-features/coscine-python-sdk/
```

### Comparing `coscine-0.9.4/src/coscine.egg-info/SOURCES.txt` & `coscine-0.9.5/src/coscine.egg-info/SOURCES.txt`

 * *Files identical despite different names*

