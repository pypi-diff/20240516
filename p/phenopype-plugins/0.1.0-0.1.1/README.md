# Comparing `tmp/phenopype_plugins-0.1.0.tar.gz` & `tmp/phenopype_plugins-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phenopype_plugins-0.1.0.tar", last modified: Mon Apr 15 04:21:35 2024, max compression
+gzip compressed data, was "phenopype_plugins-0.1.1.tar", last modified: Mon Apr 15 18:18:27 2024, max compression
```

## Comparing `phenopype_plugins-0.1.0.tar` & `phenopype_plugins-0.1.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-04-15 04:21:35.632015 phenopype_plugins-0.1.0/
--rw-rw-rw-   0        0        0     7815 2022-04-25 22:33:40.000000 phenopype_plugins-0.1.0/LICENSE
--rw-rw-rw-   0        0        0      558 2024-04-15 04:21:35.630014 phenopype_plugins-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0      120 2024-04-15 04:19:07.000000 phenopype_plugins-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-15 04:21:35.605716 phenopype_plugins-0.1.0/phenopype_plugins/
--rw-rw-rw-   0        0        0      191 2024-04-15 04:10:50.000000 phenopype_plugins-0.1.0/phenopype_plugins/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-15 04:21:35.627852 phenopype_plugins-0.1.0/phenopype_plugins/plugins/
--rw-rw-rw-   0        0        0     3579 2024-04-14 22:05:58.000000 phenopype_plugins-0.1.0/phenopype_plugins/plugins/measurement.py
--rw-rw-rw-   0        0        0    14595 2024-04-15 04:07:33.000000 phenopype_plugins-0.1.0/phenopype_plugins/plugins/segmentation.py
--rw-rw-rw-   0        0        0     1156 2024-04-15 00:38:38.000000 phenopype_plugins-0.1.0/phenopype_plugins/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-15 04:21:35.629005 phenopype_plugins-0.1.0/phenopype_plugins.egg-info/
--rw-rw-rw-   0        0        0      558 2024-04-15 04:21:35.000000 phenopype_plugins-0.1.0/phenopype_plugins.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      376 2024-04-15 04:21:35.000000 phenopype_plugins-0.1.0/phenopype_plugins.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-15 04:21:35.000000 phenopype_plugins-0.1.0/phenopype_plugins.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2024-04-15 04:21:35.000000 phenopype_plugins-0.1.0/phenopype_plugins.egg-info/requires.txt
--rw-rw-rw-   0        0        0       23 2024-04-15 04:21:35.000000 phenopype_plugins-0.1.0/phenopype_plugins.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      581 2024-04-14 16:40:08.000000 phenopype_plugins-0.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-15 04:21:35.632015 phenopype_plugins-0.1.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-15 18:18:27.572697 phenopype_plugins-0.1.1/
+-rw-rw-rw-   0        0        0     7815 2022-04-25 22:33:40.000000 phenopype_plugins-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0      558 2024-04-15 18:18:27.572697 phenopype_plugins-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0      120 2024-04-15 04:19:07.000000 phenopype_plugins-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2024-04-15 18:18:27.541051 phenopype_plugins-0.1.1/phenopype_plugins/
+-rw-rw-rw-   0        0        0      191 2024-04-15 04:10:50.000000 phenopype_plugins-0.1.1/phenopype_plugins/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-15 18:18:27.557065 phenopype_plugins-0.1.1/phenopype_plugins/plugins/
+-rw-rw-rw-   0        0        0     3579 2024-04-14 22:05:58.000000 phenopype_plugins-0.1.1/phenopype_plugins/plugins/measurement.py
+-rw-rw-rw-   0        0        0    14595 2024-04-15 04:07:33.000000 phenopype_plugins-0.1.1/phenopype_plugins/plugins/segmentation.py
+-rw-rw-rw-   0        0        0     1156 2024-04-15 00:38:38.000000 phenopype_plugins-0.1.1/phenopype_plugins/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-15 18:18:27.572697 phenopype_plugins-0.1.1/phenopype_plugins.egg-info/
+-rw-rw-rw-   0        0        0      558 2024-04-15 18:18:27.000000 phenopype_plugins-0.1.1/phenopype_plugins.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      376 2024-04-15 18:18:27.000000 phenopype_plugins-0.1.1/phenopype_plugins.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-15 18:18:27.000000 phenopype_plugins-0.1.1/phenopype_plugins.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2024-04-15 18:18:27.000000 phenopype_plugins-0.1.1/phenopype_plugins.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       23 2024-04-15 18:18:27.000000 phenopype_plugins-0.1.1/phenopype_plugins.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      581 2024-04-15 18:17:21.000000 phenopype_plugins-0.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-15 18:18:27.572697 phenopype_plugins-0.1.1/setup.cfg
```

### Comparing `phenopype_plugins-0.1.0/LICENSE` & `phenopype_plugins-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `phenopype_plugins-0.1.0/PKG-INFO` & `phenopype_plugins-0.1.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: phenopype-plugins
-Version: 0.1.0
+Version: 0.1.1
 Summary: Plugins for phenopype
 Author-email: Moritz Lürig <moritz.luerig@gmail.com>
 Project-URL: Homepage, https://phenopype.org
 Project-URL: Bug Tracker, https://github.com/phenopype/phenopype-plugins/issues
 Keywords: computer vision,biology
 Requires-Python: ==3.9.*
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: phenopype>=3.0
+Requires-Dist: phenopype>=5.0
 
 # phenopype-plugins
 
 AI-plugins for [phenopype](https://www.phenopype.org/) - currently under development, stay tuned!
```

### Comparing `phenopype_plugins-0.1.0/phenopype_plugins/plugins/measurement.py` & `phenopype_plugins-0.1.1/phenopype_plugins/plugins/measurement.py`

 * *Files identical despite different names*

### Comparing `phenopype_plugins-0.1.0/phenopype_plugins/plugins/segmentation.py` & `phenopype_plugins-0.1.1/phenopype_plugins/plugins/segmentation.py`

 * *Files identical despite different names*

### Comparing `phenopype_plugins-0.1.0/phenopype_plugins/utils.py` & `phenopype_plugins-0.1.1/phenopype_plugins/utils.py`

 * *Files identical despite different names*

### Comparing `phenopype_plugins-0.1.0/phenopype_plugins.egg-info/PKG-INFO` & `phenopype_plugins-0.1.1/phenopype_plugins.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: phenopype-plugins
-Version: 0.1.0
+Version: 0.1.1
 Summary: Plugins for phenopype
 Author-email: Moritz Lürig <moritz.luerig@gmail.com>
 Project-URL: Homepage, https://phenopype.org
 Project-URL: Bug Tracker, https://github.com/phenopype/phenopype-plugins/issues
 Keywords: computer vision,biology
 Requires-Python: ==3.9.*
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: phenopype>=3.0
+Requires-Dist: phenopype>=5.0
 
 # phenopype-plugins
 
 AI-plugins for [phenopype](https://www.phenopype.org/) - currently under development, stay tuned!
```

### Comparing `phenopype_plugins-0.1.0/pyproject.toml` & `phenopype_plugins-0.1.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -7,17 +7,17 @@
 authors = [
 	{name = "Moritz Lürig", email = "moritz.luerig@gmail.com"},
 	]
 description = "Plugins for phenopype"
 readme = "README.md"
 requires-python = "==3.9.*"
 keywords = ["computer vision", "biology"]
-version = "0.1.0"
+version = "0.1.1"
 dependencies = [
-    "phenopype>=3.0",
+    "phenopype>=5.0",
 ]
 
 [project.urls]
 "Homepage" = "https://phenopype.org"
 "Bug Tracker" = "https://github.com/phenopype/phenopype-plugins/issues"
 
 [tool.setuptools.packages.find]
```

