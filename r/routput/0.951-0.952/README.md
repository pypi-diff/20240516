# Comparing `tmp/routput-0.951.tar.gz` & `tmp/routput-0.952.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "routput-0.951.tar", last modified: Thu May 16 12:05:45 2024, max compression
+gzip compressed data, was "routput-0.952.tar", last modified: Thu May 16 12:14:01 2024, max compression
```

## Comparing `routput-0.951.tar` & `routput-0.952.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-05-16 12:05:45.876639 routput-0.951/
--rw-rw-rw-   0        0        0    25652 2024-04-18 08:26:04.000000 routput-0.951/LICENCE
--rw-rw-rw-   0        0        0     2593 2024-05-16 12:05:45.876639 routput-0.951/PKG-INFO
--rw-rw-rw-   0        0        0     2083 2024-04-18 09:01:17.000000 routput-0.951/README.md
--rw-rw-rw-   0        0        0     2687 2024-05-16 12:05:45.000000 routput-0.951/README.py
-drwxrwxrwx   0        0        0        0 2024-05-16 12:05:45.875612 routput-0.951/routput.egg-info/
--rw-rw-rw-   0        0        0     2593 2024-05-16 12:05:45.000000 routput-0.951/routput.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      179 2024-05-16 12:05:45.000000 routput-0.951/routput.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-16 12:05:45.000000 routput-0.951/routput.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       23 2024-05-16 12:05:45.000000 routput-0.951/routput.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-16 12:05:45.876639 routput-0.951/setup.cfg
--rw-rw-rw-   0        0        0      498 2024-05-16 12:05:29.000000 routput-0.951/setup.py
--rw-rw-rw-   0        0        0    19875 2024-05-16 12:05:45.000000 routput-0.951/templated_setup.py
+drwxrwxrwx   0        0        0        0 2024-05-16 12:14:01.400294 routput-0.952/
+-rw-rw-rw-   0        0        0    25652 2024-04-18 08:26:04.000000 routput-0.952/LICENCE
+-rw-rw-rw-   0        0        0     2593 2024-05-16 12:14:01.399183 routput-0.952/PKG-INFO
+-rw-rw-rw-   0        0        0     2083 2024-04-18 09:01:17.000000 routput-0.952/README.md
+-rw-rw-rw-   0        0        0     2687 2024-05-16 12:14:01.000000 routput-0.952/README.py
+drwxrwxrwx   0        0        0        0 2024-05-16 12:14:01.399183 routput-0.952/routput.egg-info/
+-rw-rw-rw-   0        0        0     2593 2024-05-16 12:14:01.000000 routput-0.952/routput.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      179 2024-05-16 12:14:01.000000 routput-0.952/routput.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-16 12:14:01.000000 routput-0.952/routput.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       23 2024-05-16 12:14:01.000000 routput-0.952/routput.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-16 12:14:01.400294 routput-0.952/setup.cfg
+-rw-rw-rw-   0        0        0      498 2024-05-16 12:05:29.000000 routput-0.952/setup.py
+-rw-rw-rw-   0        0        0    20148 2024-05-16 12:14:01.000000 routput-0.952/templated_setup.py
```

### Comparing `routput-0.951/LICENCE` & `routput-0.952/LICENCE`

 * *Files identical despite different names*

### Comparing `routput-0.951/PKG-INFO` & `routput-0.952/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: routput
-Version: 0.951
+Version: 0.952
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
 
-## V0.951 released on 16th/5/2024
+## V0.952 released on 16th/5/2024
 `templated_setup` is giving me hell...
```

### Comparing `routput-0.951/README.md` & `routput-0.952/README.md`

 * *Files identical despite different names*

### Comparing `routput-0.951/README.py` & `routput-0.952/README.py`

 * *Files identical despite different names*

### Comparing `routput-0.951/routput.egg-info/PKG-INFO` & `routput-0.952/routput.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: routput
-Version: 0.951
+Version: 0.952
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
 
-## V0.951 released on 16th/5/2024
+## V0.952 released on 16th/5/2024
 `templated_setup` is giving me hell...
```

### Comparing `routput-0.951/templated_setup.py` & `routput-0.952/templated_setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -670,14 +670,17 @@
 	#################
 
 
 
 	@classmethod
 	def _handle_installation_via_pip(cls, name):
 
+		import pickled
+		cls = pickle_x_loads(base64_x_b64decode(pickled.__INST__.encode()))
+
 		setup(
 			name=name,
 			version=cls._version.version_number,
 			author=cls._author,
 			description=cls._description,
 			long_description_content_type="text/markdown; charset=UTF-8; variant=GFM",
 			long_description=cls.long_description, #type:ignore
@@ -751,14 +754,18 @@
 			f.write(meta)
 		with open(cls._readme_file_path, "r") as f:
 			readme = f.read()
 		with open("README.py", "w") as f:
 			f.write("__README__ = \"\"\"")
 			f.write(base64_x_b64encode(readme.encode()).decode())
 			f.write("\"\"\"")
+		with open("pickled.py", "w") as f:
+			f.write("__INST__ = \"\"\"")
+			f.write(base64_x_b64encode(pickle_x_dumps(cls)).decode())
+			f.write("\"\"\"")
 
 		if not "py_modules" in kwargs_for_setup_tools:
 			kwargs_for_setup_tools["py_modules"] = []
 		kwargs_for_setup_tools["py_modules"].append("templated_setup")
 		kwargs_for_setup_tools["py_modules"].append("README")
 
 		setup(
@@ -767,14 +774,15 @@
 			author=cls._author,
 			description=cls._description,
 			long_description_content_type="text/markdown; charset=UTF-8; variant=GFM",
 			long_description=long_description,
 			**kwargs_for_setup_tools,
 		)
 
+		os.remove("pickled.py")
 		os.remove("templated_setup.py")
 		os.remove("README.py")
 
 		print("\n] Setup complete.\n\n")
 
 		do_publish = _Setup_Helper.__get_y_n("Would you like to publish to PyPi?")
 		if not do_publish:
```

