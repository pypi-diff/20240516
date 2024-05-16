# Comparing `tmp/routput-0.957.tar.gz` & `tmp/routput-0.9575.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "routput-0.957.tar", last modified: Thu May 16 12:29:19 2024, max compression
+gzip compressed data, was "routput-0.9575.tar", last modified: Thu May 16 12:33:39 2024, max compression
```

## Comparing `routput-0.957.tar` & `routput-0.9575.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-16 12:29:19.482883 routput-0.957/
--rw-rw-rw-   0        0        0    25652 2024-04-18 08:26:04.000000 routput-0.957/LICENCE
--rw-rw-rw-   0        0        0     2593 2024-05-16 12:29:19.481868 routput-0.957/PKG-INFO
--rw-rw-rw-   0        0        0     2083 2024-04-18 09:01:17.000000 routput-0.957/README.md
--rw-rw-rw-   0        0        0     2687 2024-05-16 12:29:19.000000 routput-0.957/README.py
--rw-rw-rw-   0        0        0       81 2024-05-16 12:29:19.000000 routput-0.957/pickled.py
-drwxrwxrwx   0        0        0        0 2024-05-16 12:29:19.480857 routput-0.957/routput.egg-info/
--rw-rw-rw-   0        0        0     2593 2024-05-16 12:29:19.000000 routput-0.957/routput.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      190 2024-05-16 12:29:19.000000 routput-0.957/routput.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-16 12:29:19.000000 routput-0.957/routput.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       31 2024-05-16 12:29:19.000000 routput-0.957/routput.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-16 12:29:19.482883 routput-0.957/setup.cfg
--rw-rw-rw-   0        0        0      498 2024-05-16 12:21:41.000000 routput-0.957/setup.py
--rw-rw-rw-   0        0        0    20378 2024-05-16 12:29:19.000000 routput-0.957/templated_setup.py
+drwxrwxrwx   0        0        0        0 2024-05-16 12:33:39.224485 routput-0.9575/
+-rw-rw-rw-   0        0        0    25652 2024-04-18 08:26:04.000000 routput-0.9575/LICENCE
+-rw-rw-rw-   0        0        0     2595 2024-05-16 12:33:39.222956 routput-0.9575/PKG-INFO
+-rw-rw-rw-   0        0        0     2083 2024-04-18 09:01:17.000000 routput-0.9575/README.md
+-rw-rw-rw-   0        0        0     2687 2024-05-16 12:33:39.000000 routput-0.9575/README.py
+-rw-rw-rw-   0        0        0     3509 2024-05-16 12:33:39.000000 routput-0.9575/pickled.py
+drwxrwxrwx   0        0        0        0 2024-05-16 12:33:39.222956 routput-0.9575/routput.egg-info/
+-rw-rw-rw-   0        0        0     2595 2024-05-16 12:33:39.000000 routput-0.9575/routput.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      190 2024-05-16 12:33:39.000000 routput-0.9575/routput.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-16 12:33:39.000000 routput-0.9575/routput.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       31 2024-05-16 12:33:39.000000 routput-0.9575/routput.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-16 12:33:39.225034 routput-0.9575/setup.cfg
+-rw-rw-rw-   0        0        0      498 2024-05-16 12:30:36.000000 routput-0.9575/setup.py
+-rw-rw-rw-   0        0        0    20783 2024-05-16 12:33:39.000000 routput-0.9575/templated_setup.py
```

### Comparing `routput-0.957/LICENCE` & `routput-0.9575/LICENCE`

 * *Files identical despite different names*

### Comparing `routput-0.957/PKG-INFO` & `routput-0.9575/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: routput
-Version: 0.957
+Version: 0.9575
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
 
-## V0.957 released on 16th/5/2024
+## V0.9575 released on 16th/5/2024
 `templated_setup` is giving me hell...
```

### Comparing `routput-0.957/README.md` & `routput-0.9575/README.md`

 * *Files identical despite different names*

### Comparing `routput-0.957/README.py` & `routput-0.9575/README.py`

 * *Files identical despite different names*

### Comparing `routput-0.957/routput.egg-info/PKG-INFO` & `routput-0.9575/routput.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: routput
-Version: 0.957
+Version: 0.9575
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
 
-## V0.957 released on 16th/5/2024
+## V0.9575 released on 16th/5/2024
 `templated_setup` is giving me hell...
```

### Comparing `routput-0.957/templated_setup.py` & `routput-0.9575/templated_setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -672,23 +672,28 @@
 
 
 	@classmethod
 	def _handle_installation_via_pip(cls, name):
 
 		import pickled
 		c = pickle_x_loads(base64_x_b64decode(pickled.__INST__.encode()))
+		version = c["_version"]
+		author = c["_author"]
+		description = c["_description"]
+		long_description = c["long_description"]
+		kwargs_for_setup_tools = c["_kwargs_for_setup_tools"]
 
 		setup(
 			name=name,
-			version=c._version.version_number,
-			author=c._author,
-			description=c._description,
+			version=version.version_number,
+			author=author,
+			description=description,
 			long_description_content_type="text/markdown; charset=UTF-8; variant=GFM",
-			long_description=c.long_description, #type:ignore
-			**c._kwargs_for_setup_tools
+			long_description=long_description, #type:ignore
+			**kwargs_for_setup_tools
 		)
 
 		return None
 	
 		f"[ END ] {_Setup_Helper._handle_installation_via_pip}"
 
 
@@ -761,15 +766,22 @@
 		assert cls._version is not None
 		assert cls._author is not None
 		assert cls._description is not None
 		assert cls._name is not None
 		assert cls._long_description is not None
 		with open("pickled.py", "w") as f:
 			f.write("__INST__ = \"\"\"")
-			f.write(base64_x_b64encode(pickle_x_dumps(cls)).decode())
+			f.write(base64_x_b64encode(pickle_x_dumps({
+				"_version": cls._version,
+				"_author": cls._author,
+				"_description": cls._description,
+				"_name": cls._name,
+				"long_description": cls._long_description,
+				"kwargs_for_setup_tools": kwargs_for_setup_tools,
+			})).decode())
 			f.write("\"\"\"")
 
 		if not "py_modules" in kwargs_for_setup_tools:
 			kwargs_for_setup_tools["py_modules"] = []
 		kwargs_for_setup_tools["py_modules"].append("templated_setup")
 		kwargs_for_setup_tools["py_modules"].append("README")
 		kwargs_for_setup_tools["py_modules"].append("pickled")
```

