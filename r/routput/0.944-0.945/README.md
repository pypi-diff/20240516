# Comparing `tmp/routput-0.944.tar.gz` & `tmp/routput-0.945.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "routput-0.944.tar", last modified: Thu May 16 11:22:21 2024, max compression
+gzip compressed data, was "routput-0.945.tar", last modified: Thu May 16 11:24:41 2024, max compression
```

## Comparing `routput-0.944.tar` & `routput-0.945.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-05-16 11:22:21.976667 routput-0.944/
--rw-rw-rw-   0        0        0    25652 2024-04-18 08:26:04.000000 routput-0.944/LICENCE
--rw-rw-rw-   0        0        0     2593 2024-05-16 11:22:21.976667 routput-0.944/PKG-INFO
--rw-rw-rw-   0        0        0     2083 2024-04-18 09:01:17.000000 routput-0.944/README.md
-drwxrwxrwx   0        0        0        0 2024-05-16 11:22:21.975617 routput-0.944/routput.egg-info/
--rw-rw-rw-   0        0        0     2593 2024-05-16 11:22:21.000000 routput-0.944/routput.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      169 2024-05-16 11:22:21.000000 routput-0.944/routput.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-16 11:22:21.000000 routput-0.944/routput.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2024-05-16 11:22:21.000000 routput-0.944/routput.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-16 11:22:21.976667 routput-0.944/setup.cfg
--rw-rw-rw-   0        0        0      498 2024-05-16 11:17:34.000000 routput-0.944/setup.py
--rw-rw-rw-   0        0        0    21071 2024-05-16 11:22:21.000000 routput-0.944/templated_setup.py
+drwxrwxrwx   0        0        0        0 2024-05-16 11:24:41.214328 routput-0.945/
+-rw-rw-rw-   0        0        0    25652 2024-04-18 08:26:04.000000 routput-0.945/LICENCE
+-rw-rw-rw-   0        0        0     2593 2024-05-16 11:24:41.213207 routput-0.945/PKG-INFO
+-rw-rw-rw-   0        0        0     2083 2024-04-18 09:01:17.000000 routput-0.945/README.md
+drwxrwxrwx   0        0        0        0 2024-05-16 11:24:41.212194 routput-0.945/routput.egg-info/
+-rw-rw-rw-   0        0        0     2593 2024-05-16 11:24:41.000000 routput-0.945/routput.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      169 2024-05-16 11:24:41.000000 routput-0.945/routput.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-16 11:24:41.000000 routput-0.945/routput.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2024-05-16 11:24:41.000000 routput-0.945/routput.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-16 11:24:41.214328 routput-0.945/setup.cfg
+-rw-rw-rw-   0        0        0      498 2024-05-16 11:17:34.000000 routput-0.945/setup.py
+-rw-rw-rw-   0        0        0    21133 2024-05-16 11:24:41.000000 routput-0.945/templated_setup.py
```

### Comparing `routput-0.944/LICENCE` & `routput-0.945/LICENCE`

 * *Files identical despite different names*

### Comparing `routput-0.944/PKG-INFO` & `routput-0.945/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: routput
-Version: 0.944
+Version: 0.945
 Summary: recursively searches for files based on their extensions starting from a specified directory. It can print the directory structure, include or exclude specific files, use syntax highlighting for output, and anonymize file paths for privacy.
 Author: matrikater (Joel Watson)
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 License-File: LICENCE
 
 # Recursive Output Utility
 
@@ -86,9 +86,9 @@
 python routput.py -e [py] -b
 ```
 
 ## License
 
 Open-source software licensed under GPL-2 license.
 
-## V0.944 released on 16th/5/2024
+## V0.945 released on 16th/5/2024
 `templated_setup` is giving me hell...
```

### Comparing `routput-0.944/README.md` & `routput-0.945/README.md`

 * *Files identical despite different names*

### Comparing `routput-0.944/routput.egg-info/PKG-INFO` & `routput-0.945/routput.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: routput
-Version: 0.944
+Version: 0.945
 Summary: recursively searches for files based on their extensions starting from a specified directory. It can print the directory structure, include or exclude specific files, use syntax highlighting for output, and anonymize file paths for privacy.
 Author: matrikater (Joel Watson)
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 License-File: LICENCE
 
 # Recursive Output Utility
 
@@ -86,9 +86,9 @@
 python routput.py -e [py] -b
 ```
 
 ## License
 
 Open-source software licensed under GPL-2 license.
 
-## V0.944 released on 16th/5/2024
+## V0.945 released on 16th/5/2024
 `templated_setup` is giving me hell...
```

### Comparing `routput-0.944/templated_setup.py` & `routput-0.945/templated_setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -676,14 +676,16 @@
 				f.write("__version__ = \"0.0\"\n")
 				f.write("__author__ = \"\"\n")
 				f.write("__description__ = \"\"\n")
 				f.write("__long_description__ = \"\"\"\"\"\"\n")
 				f.write("__kwargs_for_setup_tools__ = \"\"\"\"\"\"\n")
 			with open("__init__.py", "w") as f:
 				f.write("")
+			import sys
+			sys.path.append(os.path.dirname(__file__))
 			from . import _hardcoded #type:ignore
 		kwargs_for_setup_tools = base64_x_b64decode(_hardcoded.__kwargs_for_setup_tools__.encode("utf-8")) #type:ignore
 		kwargs_for_setup_tools = pickle_x_loads(kwargs_for_setup_tools)
 		long_description = base64_x_b64decode(_hardcoded.__long_description__.encode("utf-8")) #type:ignore
 		long_description = pickle_x_loads(long_description)
 		setup(
 			name=name,
```

