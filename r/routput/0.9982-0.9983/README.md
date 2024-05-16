# Comparing `tmp/routput-0.9982.tar.gz` & `tmp/routput-0.9983.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "routput-0.9982.tar", last modified: Thu May 16 12:57:05 2024, max compression
+gzip compressed data, was "routput-0.9983.tar", last modified: Thu May 16 13:12:19 2024, max compression
```

## Comparing `routput-0.9982.tar` & `routput-0.9983.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-16 12:57:05.848330 routput-0.9982/
--rw-rw-rw-   0        0        0    25652 2024-04-18 08:26:04.000000 routput-0.9982/LICENCE
--rw-rw-rw-   0        0        0     2595 2024-05-16 12:57:05.848330 routput-0.9982/PKG-INFO
--rw-rw-rw-   0        0        0     2083 2024-04-18 09:01:17.000000 routput-0.9982/README.md
--rw-rw-rw-   0        0        0     2687 2024-05-16 12:57:05.000000 routput-0.9982/README.py
--rw-rw-rw-   0        0        0     3505 2024-05-16 12:57:05.000000 routput-0.9982/pickled.py
-drwxrwxrwx   0        0        0        0 2024-05-16 12:57:05.847310 routput-0.9982/routput.egg-info/
--rw-rw-rw-   0        0        0     2595 2024-05-16 12:57:05.000000 routput-0.9982/routput.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      190 2024-05-16 12:57:05.000000 routput-0.9982/routput.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-16 12:57:05.000000 routput-0.9982/routput.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       31 2024-05-16 12:57:05.000000 routput-0.9982/routput.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-16 12:57:05.849347 routput-0.9982/setup.cfg
--rw-rw-rw-   0        0        0      498 2024-05-16 12:45:46.000000 routput-0.9982/setup.py
--rw-rw-rw-   0        0        0    21056 2024-05-16 12:57:05.000000 routput-0.9982/templated_setup.py
+drwxrwxrwx   0        0        0        0 2024-05-16 13:12:19.832985 routput-0.9983/
+-rw-rw-rw-   0        0        0    25652 2024-04-18 08:26:04.000000 routput-0.9983/LICENCE
+-rw-rw-rw-   0        0        0     2597 2024-05-16 13:12:19.831981 routput-0.9983/PKG-INFO
+-rw-rw-rw-   0        0        0     2083 2024-04-18 09:01:17.000000 routput-0.9983/README.md
+-rw-rw-rw-   0        0        0     2687 2024-05-16 13:12:19.000000 routput-0.9983/_README.py
+-rw-rw-rw-   0        0        0     3509 2024-05-16 13:12:19.000000 routput-0.9983/_pickled.py
+drwxrwxrwx   0        0        0        0 2024-05-16 13:12:19.830962 routput-0.9983/routput.egg-info/
+-rw-rw-rw-   0        0        0     2597 2024-05-16 13:12:19.000000 routput-0.9983/routput.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      192 2024-05-16 13:12:19.000000 routput-0.9983/routput.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-16 13:12:19.000000 routput-0.9983/routput.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       41 2024-05-16 13:12:19.000000 routput-0.9983/routput.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-16 13:12:19.832985 routput-0.9983/setup.cfg
+-rw-rw-rw-   0        0        0      498 2024-05-16 12:45:46.000000 routput-0.9983/setup.py
+-rw-rw-rw-   0        0        0    21120 2024-05-16 13:12:19.000000 routput-0.9983/templated_setup.py
```

### Comparing `routput-0.9982/LICENCE` & `routput-0.9983/LICENCE`

 * *Files identical despite different names*

### Comparing `routput-0.9982/PKG-INFO` & `routput-0.9983/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: routput
-Version: 0.9982
+Version: 0.9983
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
 
-## V0.9982 released on 16th/5/2024
-`templated_setup` is giving me hell...
+## V0.9983 released on 16th/5/2024
+hopefully `templated_setup` works now...
```

### Comparing `routput-0.9982/README.md` & `routput-0.9983/README.md`

 * *Files identical despite different names*

### Comparing `routput-0.9982/README.py` & `routput-0.9983/_README.py`

 * *Files identical despite different names*

### Comparing `routput-0.9982/routput.egg-info/PKG-INFO` & `routput-0.9983/routput.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: routput
-Version: 0.9982
+Version: 0.9983
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
 
-## V0.9982 released on 16th/5/2024
-`templated_setup` is giving me hell...
+## V0.9983 released on 16th/5/2024
+hopefully `templated_setup` works now...
```

### Comparing `routput-0.9982/templated_setup.py` & `routput-0.9983/templated_setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -761,54 +761,55 @@
 		meta = None
 		with open(__file__, "r") as f:
 			meta = f.read()
 		with open("templated_setup.py", "w") as f:
 			f.write(meta)
 		with open(cls._readme_file_path, "r") as f:
 			readme = f.read()
-		with open("README.py", "w") as f:
+		with open("_README.py", "w") as f:
 			f.write("__README__ = \"\"\"")
 			f.write(base64_x_b64encode(readme.encode()).decode())
 			f.write("\"\"\"")
 		assert cls._version is not None
 		assert cls._author is not None
 		assert cls._description is not None
 		assert cls._name is not None
 		assert cls._long_description is not None
-		with open("pickled.py", "w") as f:
+		with open("_pickled.py", "w") as f:
 			f.write("__INST__ = \"\"\"")
 			f.write(base64_x_b64encode(pickle_x_dumps({
 				"version": cls._version,
 				"author": cls._author,
 				"description": cls._description,
 				"name": cls._name,
 				"long_description": cls._long_description,
 				"kwargs_for_setup_tools": kwargs_for_setup_tools,
 			})).decode())
 			f.write("\"\"\"")
 
 		if not "py_modules" in kwargs_for_setup_tools:
 			kwargs_for_setup_tools["py_modules"] = []
 		kwargs_for_setup_tools["py_modules"].append("templated_setup")
-		kwargs_for_setup_tools["py_modules"].append("README")
-		kwargs_for_setup_tools["py_modules"].append("pickled")
+		kwargs_for_setup_tools["py_modules"].append("_README")
+		kwargs_for_setup_tools["py_modules"].append("_pickled")
+		kwargs_for_setup_tools["py_modules"].append(cls._name)
 
 		setup(
 			name=cls._name,
 			version=cls._version.version_number,
 			author=cls._author,
 			description=cls._description,
 			long_description_content_type="text/markdown; charset=UTF-8; variant=GFM",
 			long_description=long_description,
 			**kwargs_for_setup_tools,
 		)
 
-		os.remove("pickled.py")
+		os.remove("_pickled.py")
 		os.remove("templated_setup.py")
-		os.remove("README.py")
+		os.remove("_README.py")
 
 		print("\n] Setup complete.\n\n")
 
 		do_publish = _Setup_Helper.__get_y_n("Would you like to publish to PyPi?")
 		if not do_publish:
 			exit(0)
```

