# Comparing `tmp/routput-0.953.tar.gz` & `tmp/routput-0.954.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "routput-0.953.tar", last modified: Thu May 16 12:16:42 2024, max compression
+gzip compressed data, was "routput-0.954.tar", last modified: Thu May 16 12:19:17 2024, max compression
```

## Comparing `routput-0.953.tar` & `routput-0.954.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-16 12:16:42.603886 routput-0.953/
--rw-rw-rw-   0        0        0    25652 2024-04-18 08:26:04.000000 routput-0.953/LICENCE
--rw-rw-rw-   0        0        0     2593 2024-05-16 12:16:42.603886 routput-0.953/PKG-INFO
--rw-rw-rw-   0        0        0     2083 2024-04-18 09:01:17.000000 routput-0.953/README.md
--rw-rw-rw-   0        0        0     2687 2024-05-16 12:16:42.000000 routput-0.953/README.py
--rw-rw-rw-   0        0        0       81 2024-05-16 12:16:42.000000 routput-0.953/pickled.py
-drwxrwxrwx   0        0        0        0 2024-05-16 12:16:42.602866 routput-0.953/routput.egg-info/
--rw-rw-rw-   0        0        0     2593 2024-05-16 12:16:42.000000 routput-0.953/routput.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      190 2024-05-16 12:16:42.000000 routput-0.953/routput.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-16 12:16:42.000000 routput-0.953/routput.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       31 2024-05-16 12:16:42.000000 routput-0.953/routput.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-16 12:16:42.604902 routput-0.953/setup.cfg
--rw-rw-rw-   0        0        0      498 2024-05-16 12:05:29.000000 routput-0.953/setup.py
--rw-rw-rw-   0        0        0    20206 2024-05-16 12:16:42.000000 routput-0.953/templated_setup.py
+drwxrwxrwx   0        0        0        0 2024-05-16 12:19:17.039944 routput-0.954/
+-rw-rw-rw-   0        0        0    25652 2024-04-18 08:26:04.000000 routput-0.954/LICENCE
+-rw-rw-rw-   0        0        0     2593 2024-05-16 12:19:17.038922 routput-0.954/PKG-INFO
+-rw-rw-rw-   0        0        0     2083 2024-04-18 09:01:17.000000 routput-0.954/README.md
+-rw-rw-rw-   0        0        0     2687 2024-05-16 12:19:16.000000 routput-0.954/README.py
+-rw-rw-rw-   0        0        0       81 2024-05-16 12:19:16.000000 routput-0.954/pickled.py
+drwxrwxrwx   0        0        0        0 2024-05-16 12:19:17.037816 routput-0.954/routput.egg-info/
+-rw-rw-rw-   0        0        0     2593 2024-05-16 12:19:16.000000 routput-0.954/routput.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      190 2024-05-16 12:19:17.000000 routput-0.954/routput.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-16 12:19:16.000000 routput-0.954/routput.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       31 2024-05-16 12:19:16.000000 routput-0.954/routput.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-16 12:19:17.039944 routput-0.954/setup.cfg
+-rw-rw-rw-   0        0        0      498 2024-05-16 12:05:29.000000 routput-0.954/setup.py
+-rw-rw-rw-   0        0        0    20194 2024-05-16 12:19:16.000000 routput-0.954/templated_setup.py
```

### Comparing `routput-0.953/LICENCE` & `routput-0.954/LICENCE`

 * *Files identical despite different names*

### Comparing `routput-0.953/PKG-INFO` & `routput-0.954/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: routput
-Version: 0.953
+Version: 0.954
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
 
-## V0.953 released on 16th/5/2024
+## V0.954 released on 16th/5/2024
 `templated_setup` is giving me hell...
```

### Comparing `routput-0.953/README.md` & `routput-0.954/README.md`

 * *Files identical despite different names*

### Comparing `routput-0.953/README.py` & `routput-0.954/README.py`

 * *Files identical despite different names*

### Comparing `routput-0.953/routput.egg-info/PKG-INFO` & `routput-0.954/routput.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: routput
-Version: 0.953
+Version: 0.954
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
 
-## V0.953 released on 16th/5/2024
+## V0.954 released on 16th/5/2024
 `templated_setup` is giving me hell...
```

### Comparing `routput-0.953/templated_setup.py` & `routput-0.954/templated_setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -671,24 +671,24 @@
 
 
 
 	@classmethod
 	def _handle_installation_via_pip(cls, name):
 
 		import pickled
-		cls = pickle_x_loads(base64_x_b64decode(pickled.__INST__.encode()))
+		c = pickle_x_loads(base64_x_b64decode(pickled.__INST__.encode()))
 
 		setup(
 			name=name,
-			version=cls._version.version_number,
-			author=cls._author,
-			description=cls._description,
+			version=c._version.version_number,
+			author=c._author,
+			description=c._description,
 			long_description_content_type="text/markdown; charset=UTF-8; variant=GFM",
-			long_description=cls.long_description, #type:ignore
-			**cls._kwargs_for_setup_tools
+			long_description=c.long_description, #type:ignore
+			**c._kwargs_for_setup_tools
 		)
 
 		return None
 	
 		f"[ END ] {_Setup_Helper._handle_installation_via_pip}"
```

