# Comparing `tmp/routput-0.955.tar.gz` & `tmp/routput-0.956.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "routput-0.955.tar", last modified: Thu May 16 12:22:05 2024, max compression
+gzip compressed data, was "routput-0.956.tar", last modified: Thu May 16 12:23:33 2024, max compression
```

## Comparing `routput-0.955.tar` & `routput-0.956.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-16 12:22:05.688639 routput-0.955/
--rw-rw-rw-   0        0        0    25652 2024-04-18 08:26:04.000000 routput-0.955/LICENCE
--rw-rw-rw-   0        0        0     2593 2024-05-16 12:22:05.687629 routput-0.955/PKG-INFO
--rw-rw-rw-   0        0        0     2083 2024-04-18 09:01:17.000000 routput-0.955/README.md
--rw-rw-rw-   0        0        0     2687 2024-05-16 12:22:05.000000 routput-0.955/README.py
--rw-rw-rw-   0        0        0       81 2024-05-16 12:22:05.000000 routput-0.955/pickled.py
-drwxrwxrwx   0        0        0        0 2024-05-16 12:22:05.687122 routput-0.955/routput.egg-info/
--rw-rw-rw-   0        0        0     2593 2024-05-16 12:22:05.000000 routput-0.955/routput.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      190 2024-05-16 12:22:05.000000 routput-0.955/routput.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-16 12:22:05.000000 routput-0.955/routput.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       31 2024-05-16 12:22:05.000000 routput-0.955/routput.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-16 12:22:05.688639 routput-0.955/setup.cfg
--rw-rw-rw-   0        0        0      498 2024-05-16 12:21:41.000000 routput-0.955/setup.py
--rw-rw-rw-   0        0        0    20185 2024-05-16 12:22:05.000000 routput-0.955/templated_setup.py
+drwxrwxrwx   0        0        0        0 2024-05-16 12:23:33.064198 routput-0.956/
+-rw-rw-rw-   0        0        0    25652 2024-04-18 08:26:04.000000 routput-0.956/LICENCE
+-rw-rw-rw-   0        0        0     2593 2024-05-16 12:23:33.064198 routput-0.956/PKG-INFO
+-rw-rw-rw-   0        0        0     2083 2024-04-18 09:01:17.000000 routput-0.956/README.md
+-rw-rw-rw-   0        0        0     2687 2024-05-16 12:23:32.000000 routput-0.956/README.py
+-rw-rw-rw-   0        0        0       81 2024-05-16 12:23:32.000000 routput-0.956/pickled.py
+drwxrwxrwx   0        0        0        0 2024-05-16 12:23:33.063194 routput-0.956/routput.egg-info/
+-rw-rw-rw-   0        0        0     2593 2024-05-16 12:23:32.000000 routput-0.956/routput.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      190 2024-05-16 12:23:33.000000 routput-0.956/routput.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-16 12:23:33.000000 routput-0.956/routput.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       31 2024-05-16 12:23:33.000000 routput-0.956/routput.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-16 12:23:33.064198 routput-0.956/setup.cfg
+-rw-rw-rw-   0        0        0      498 2024-05-16 12:21:41.000000 routput-0.956/setup.py
+-rw-rw-rw-   0        0        0    20186 2024-05-16 12:23:32.000000 routput-0.956/templated_setup.py
```

### Comparing `routput-0.955/LICENCE` & `routput-0.956/LICENCE`

 * *Files identical despite different names*

### Comparing `routput-0.955/PKG-INFO` & `routput-0.956/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: routput
-Version: 0.955
+Version: 0.956
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
 
-## V0.955 released on 16th/5/2024
+## V0.956 released on 16th/5/2024
 `templated_setup` is giving me hell...
```

### Comparing `routput-0.955/README.md` & `routput-0.956/README.md`

 * *Files identical despite different names*

### Comparing `routput-0.955/README.py` & `routput-0.956/README.py`

 * *Files identical despite different names*

### Comparing `routput-0.955/routput.egg-info/PKG-INFO` & `routput-0.956/routput.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: routput
-Version: 0.955
+Version: 0.956
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
 
-## V0.955 released on 16th/5/2024
+## V0.956 released on 16th/5/2024
 `templated_setup` is giving me hell...
```

### Comparing `routput-0.955/templated_setup.py` & `routput-0.956/templated_setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -675,15 +675,15 @@
 	def _handle_installation_via_pip(cls, name):
 
 		import pickled
 		c = pickle_x_loads(base64_x_b64decode(pickled.__INST__.encode()))
 
 		setup(
 			name=name,
-			version=c.version_number,
+			version=c._version_number,
 			author=c._author,
 			description=c._description,
 			long_description_content_type="text/markdown; charset=UTF-8; variant=GFM",
 			long_description=c.long_description, #type:ignore
 			**c._kwargs_for_setup_tools
 		)
```

