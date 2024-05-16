# Comparing `tmp/templated_setup-0.995.tar.gz` & `tmp/templated_setup-0.9975.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "templated_setup-0.995.tar", last modified: Thu May 16 12:32:40 2024, max compression
+gzip compressed data, was "templated_setup-0.9975.tar", last modified: Thu May 16 12:34:46 2024, max compression
```

## Comparing `templated_setup-0.995.tar` & `templated_setup-0.9975.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-16 12:32:40.382702 templated_setup-0.995/
--rw-rw-rw-   0        0        0    25652 2024-03-14 11:21:06.000000 templated_setup-0.995/LICENCE
--rw-rw-rw-   0        0        0     2553 2024-05-16 12:32:40.381689 templated_setup-0.995/PKG-INFO
--rw-rw-rw-   0        0        0     2172 2024-04-29 06:54:31.000000 templated_setup-0.995/README.md
--rw-rw-rw-   0        0        0       42 2024-05-16 12:32:40.383769 templated_setup-0.995/setup.cfg
--rw-rw-rw-   0        0        0     1271 2024-05-16 12:32:37.000000 templated_setup-0.995/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-16 12:32:40.375106 templated_setup-0.995/templated_setup/
--rw-rw-rw-   0        0        0    20783 2024-05-16 12:32:29.000000 templated_setup-0.995/templated_setup/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-16 12:32:40.381689 templated_setup-0.995/templated_setup.egg-info/
--rw-rw-rw-   0        0        0     2553 2024-05-16 12:32:40.000000 templated_setup-0.995/templated_setup.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      248 2024-05-16 12:32:40.000000 templated_setup-0.995/templated_setup.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-16 12:32:40.000000 templated_setup-0.995/templated_setup.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2024-05-16 12:32:40.000000 templated_setup-0.995/templated_setup.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2024-05-16 12:32:40.000000 templated_setup-0.995/templated_setup.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-16 12:34:46.564164 templated_setup-0.9975/
+-rw-rw-rw-   0        0        0    25652 2024-03-14 11:21:06.000000 templated_setup-0.9975/LICENCE
+-rw-rw-rw-   0        0        0     2555 2024-05-16 12:34:46.563156 templated_setup-0.9975/PKG-INFO
+-rw-rw-rw-   0        0        0     2172 2024-04-29 06:54:31.000000 templated_setup-0.9975/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-16 12:34:46.565172 templated_setup-0.9975/setup.cfg
+-rw-rw-rw-   0        0        0     1272 2024-05-16 12:34:38.000000 templated_setup-0.9975/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-16 12:34:46.556584 templated_setup-0.9975/templated_setup/
+-rw-rw-rw-   0        0        0    20775 2024-05-16 12:34:27.000000 templated_setup-0.9975/templated_setup/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-16 12:34:46.563156 templated_setup-0.9975/templated_setup.egg-info/
+-rw-rw-rw-   0        0        0     2555 2024-05-16 12:34:46.000000 templated_setup-0.9975/templated_setup.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      248 2024-05-16 12:34:46.000000 templated_setup-0.9975/templated_setup.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-16 12:34:46.000000 templated_setup-0.9975/templated_setup.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2024-05-16 12:34:46.000000 templated_setup-0.9975/templated_setup.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2024-05-16 12:34:46.000000 templated_setup-0.9975/templated_setup.egg-info/top_level.txt
```

### Comparing `templated_setup-0.995/LICENCE` & `templated_setup-0.9975/LICENCE`

 * *Files identical despite different names*

### Comparing `templated_setup-0.995/PKG-INFO` & `templated_setup-0.9975/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: templated_setup
-Version: 0.995
+Version: 0.9975
 Summary: A quick and easy replacement for some `setup.py` implementations.
 Author: matrikater (Joel Watson)
 Author-email: administraitor@matriko.xyz
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 License-File: LICENCE
 Requires-Dist: setuptools
 Requires-Dist: twine
@@ -67,9 +67,9 @@
 
 > Actually I would be happy to have some help with this project as making a `setup.py` every time is a bit boring.
 
 ## License
 
 This project is licensed under the GPLv2 License - see the [LICENSE](LICENSE) file for details.
 
-## V0.995
+## V0.9975
 No notes.
```

### Comparing `templated_setup-0.995/README.md` & `templated_setup-0.9975/README.md`

 * *Files identical despite different names*

### Comparing `templated_setup-0.995/setup.py` & `templated_setup-0.9975/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 	with open(readme_file_path_, "r") as f:
 		description = f.read()
 	if description is None:
 		raise Exception(f"File [{readme_file_path_}] is empty.")
 	return description
 
 
-version_number = "0.995"
+version_number = "0.9975"
 notes = "No notes."
 
 long_description = __init_description("README.md")
 long_description += f"\n## V{version_number}\n"
 long_description += notes
 
 setup(
```

### Comparing `templated_setup-0.995/templated_setup/__init__.py` & `templated_setup-0.9975/templated_setup/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -672,19 +672,19 @@
 
 
 	@classmethod
 	def _handle_installation_via_pip(cls, name):
 
 		import pickled
 		c = pickle_x_loads(base64_x_b64decode(pickled.__INST__.encode()))
-		version = c["_version"]
-		author = c["_author"]
-		description = c["_description"]
+		version = c["version"]
+		author = c["author"]
+		description = c["description"]
 		long_description = c["long_description"]
-		kwargs_for_setup_tools = c["_kwargs_for_setup_tools"]
+		kwargs_for_setup_tools = c["kwargs_for_setup_tools"]
 
 		setup(
 			name=name,
 			version=version.version_number,
 			author=author,
 			description=description,
 			long_description_content_type="text/markdown; charset=UTF-8; variant=GFM",
@@ -767,18 +767,18 @@
 		assert cls._author is not None
 		assert cls._description is not None
 		assert cls._name is not None
 		assert cls._long_description is not None
 		with open("pickled.py", "w") as f:
 			f.write("__INST__ = \"\"\"")
 			f.write(base64_x_b64encode(pickle_x_dumps({
-				"_version": cls._version,
-				"_author": cls._author,
-				"_description": cls._description,
-				"_name": cls._name,
+				"version": cls._version,
+				"author": cls._author,
+				"description": cls._description,
+				"name": cls._name,
 				"long_description": cls._long_description,
 				"kwargs_for_setup_tools": kwargs_for_setup_tools,
 			})).decode())
 			f.write("\"\"\"")
 
 		if not "py_modules" in kwargs_for_setup_tools:
 			kwargs_for_setup_tools["py_modules"] = []
```

### Comparing `templated_setup-0.995/templated_setup.egg-info/PKG-INFO` & `templated_setup-0.9975/templated_setup.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: templated_setup
-Version: 0.995
+Version: 0.9975
 Summary: A quick and easy replacement for some `setup.py` implementations.
 Author: matrikater (Joel Watson)
 Author-email: administraitor@matriko.xyz
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 License-File: LICENCE
 Requires-Dist: setuptools
 Requires-Dist: twine
@@ -67,9 +67,9 @@
 
 > Actually I would be happy to have some help with this project as making a `setup.py` every time is a bit boring.
 
 ## License
 
 This project is licensed under the GPLv2 License - see the [LICENSE](LICENSE) file for details.
 
-## V0.995
+## V0.9975
 No notes.
```

