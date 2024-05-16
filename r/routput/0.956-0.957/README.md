# Comparing `tmp/routput-0.956.tar.gz` & `tmp/routput-0.957.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "routput-0.956.tar", last modified: Thu May 16 12:23:33 2024, max compression
+gzip compressed data, was "routput-0.957.tar", last modified: Thu May 16 12:29:19 2024, max compression
```

## Comparing `routput-0.956.tar` & `routput-0.957.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-16 12:23:33.064198 routput-0.956/
--rw-rw-rw-   0        0        0    25652 2024-04-18 08:26:04.000000 routput-0.956/LICENCE
--rw-rw-rw-   0        0        0     2593 2024-05-16 12:23:33.064198 routput-0.956/PKG-INFO
--rw-rw-rw-   0        0        0     2083 2024-04-18 09:01:17.000000 routput-0.956/README.md
--rw-rw-rw-   0        0        0     2687 2024-05-16 12:23:32.000000 routput-0.956/README.py
--rw-rw-rw-   0        0        0       81 2024-05-16 12:23:32.000000 routput-0.956/pickled.py
-drwxrwxrwx   0        0        0        0 2024-05-16 12:23:33.063194 routput-0.956/routput.egg-info/
--rw-rw-rw-   0        0        0     2593 2024-05-16 12:23:32.000000 routput-0.956/routput.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      190 2024-05-16 12:23:33.000000 routput-0.956/routput.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-16 12:23:33.000000 routput-0.956/routput.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       31 2024-05-16 12:23:33.000000 routput-0.956/routput.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-16 12:23:33.064198 routput-0.956/setup.cfg
--rw-rw-rw-   0        0        0      498 2024-05-16 12:21:41.000000 routput-0.956/setup.py
--rw-rw-rw-   0        0        0    20186 2024-05-16 12:23:32.000000 routput-0.956/templated_setup.py
+drwxrwxrwx   0        0        0        0 2024-05-16 12:29:19.482883 routput-0.957/
+-rw-rw-rw-   0        0        0    25652 2024-04-18 08:26:04.000000 routput-0.957/LICENCE
+-rw-rw-rw-   0        0        0     2593 2024-05-16 12:29:19.481868 routput-0.957/PKG-INFO
+-rw-rw-rw-   0        0        0     2083 2024-04-18 09:01:17.000000 routput-0.957/README.md
+-rw-rw-rw-   0        0        0     2687 2024-05-16 12:29:19.000000 routput-0.957/README.py
+-rw-rw-rw-   0        0        0       81 2024-05-16 12:29:19.000000 routput-0.957/pickled.py
+drwxrwxrwx   0        0        0        0 2024-05-16 12:29:19.480857 routput-0.957/routput.egg-info/
+-rw-rw-rw-   0        0        0     2593 2024-05-16 12:29:19.000000 routput-0.957/routput.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      190 2024-05-16 12:29:19.000000 routput-0.957/routput.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-16 12:29:19.000000 routput-0.957/routput.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       31 2024-05-16 12:29:19.000000 routput-0.957/routput.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-16 12:29:19.482883 routput-0.957/setup.cfg
+-rw-rw-rw-   0        0        0      498 2024-05-16 12:21:41.000000 routput-0.957/setup.py
+-rw-rw-rw-   0        0        0    20378 2024-05-16 12:29:19.000000 routput-0.957/templated_setup.py
```

### Comparing `routput-0.956/LICENCE` & `routput-0.957/LICENCE`

 * *Files identical despite different names*

### Comparing `routput-0.956/PKG-INFO` & `routput-0.957/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: routput
-Version: 0.956
+Version: 0.957
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
 
-## V0.956 released on 16th/5/2024
+## V0.957 released on 16th/5/2024
 `templated_setup` is giving me hell...
```

### Comparing `routput-0.956/README.md` & `routput-0.957/README.md`

 * *Files identical despite different names*

### Comparing `routput-0.956/README.py` & `routput-0.957/README.py`

 * *Files identical despite different names*

### Comparing `routput-0.956/routput.egg-info/PKG-INFO` & `routput-0.957/routput.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: routput
-Version: 0.956
+Version: 0.957
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
 
-## V0.956 released on 16th/5/2024
+## V0.957 released on 16th/5/2024
 `templated_setup` is giving me hell...
```

### Comparing `routput-0.956/templated_setup.py` & `routput-0.957/templated_setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -675,15 +675,15 @@
 	def _handle_installation_via_pip(cls, name):
 
 		import pickled
 		c = pickle_x_loads(base64_x_b64decode(pickled.__INST__.encode()))
 
 		setup(
 			name=name,
-			version=c._version_number,
+			version=c._version.version_number,
 			author=c._author,
 			description=c._description,
 			long_description_content_type="text/markdown; charset=UTF-8; variant=GFM",
 			long_description=c.long_description, #type:ignore
 			**c._kwargs_for_setup_tools
 		)
 
@@ -754,14 +754,19 @@
 			f.write(meta)
 		with open(cls._readme_file_path, "r") as f:
 			readme = f.read()
 		with open("README.py", "w") as f:
 			f.write("__README__ = \"\"\"")
 			f.write(base64_x_b64encode(readme.encode()).decode())
 			f.write("\"\"\"")
+		assert cls._version is not None
+		assert cls._author is not None
+		assert cls._description is not None
+		assert cls._name is not None
+		assert cls._long_description is not None
 		with open("pickled.py", "w") as f:
 			f.write("__INST__ = \"\"\"")
 			f.write(base64_x_b64encode(pickle_x_dumps(cls)).decode())
 			f.write("\"\"\"")
 
 		if not "py_modules" in kwargs_for_setup_tools:
 			kwargs_for_setup_tools["py_modules"] = []
```

