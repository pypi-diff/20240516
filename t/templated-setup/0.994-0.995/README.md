# Comparing `tmp/templated_setup-0.994.tar.gz` & `tmp/templated_setup-0.995.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "templated_setup-0.994.tar", last modified: Thu May 16 12:14:58 2024, max compression
+gzip compressed data, was "templated_setup-0.995.tar", last modified: Thu May 16 12:32:40 2024, max compression
```

## Comparing `templated_setup-0.994.tar` & `templated_setup-0.995.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-16 12:14:58.128693 templated_setup-0.994/
--rw-rw-rw-   0        0        0    25652 2024-03-14 11:21:06.000000 templated_setup-0.994/LICENCE
--rw-rw-rw-   0        0        0     2553 2024-05-16 12:14:58.127281 templated_setup-0.994/PKG-INFO
--rw-rw-rw-   0        0        0     2172 2024-04-29 06:54:31.000000 templated_setup-0.994/README.md
--rw-rw-rw-   0        0        0       42 2024-05-16 12:14:58.128693 templated_setup-0.994/setup.cfg
--rw-rw-rw-   0        0        0     1271 2024-05-16 12:14:55.000000 templated_setup-0.994/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-16 12:14:58.119602 templated_setup-0.994/templated_setup/
--rw-rw-rw-   0        0        0    20206 2024-05-16 12:14:49.000000 templated_setup-0.994/templated_setup/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-16 12:14:58.126255 templated_setup-0.994/templated_setup.egg-info/
--rw-rw-rw-   0        0        0     2553 2024-05-16 12:14:58.000000 templated_setup-0.994/templated_setup.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      248 2024-05-16 12:14:58.000000 templated_setup-0.994/templated_setup.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-16 12:14:58.000000 templated_setup-0.994/templated_setup.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2024-05-16 12:14:58.000000 templated_setup-0.994/templated_setup.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2024-05-16 12:14:58.000000 templated_setup-0.994/templated_setup.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-16 12:32:40.382702 templated_setup-0.995/
+-rw-rw-rw-   0        0        0    25652 2024-03-14 11:21:06.000000 templated_setup-0.995/LICENCE
+-rw-rw-rw-   0        0        0     2553 2024-05-16 12:32:40.381689 templated_setup-0.995/PKG-INFO
+-rw-rw-rw-   0        0        0     2172 2024-04-29 06:54:31.000000 templated_setup-0.995/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-16 12:32:40.383769 templated_setup-0.995/setup.cfg
+-rw-rw-rw-   0        0        0     1271 2024-05-16 12:32:37.000000 templated_setup-0.995/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-16 12:32:40.375106 templated_setup-0.995/templated_setup/
+-rw-rw-rw-   0        0        0    20783 2024-05-16 12:32:29.000000 templated_setup-0.995/templated_setup/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-16 12:32:40.381689 templated_setup-0.995/templated_setup.egg-info/
+-rw-rw-rw-   0        0        0     2553 2024-05-16 12:32:40.000000 templated_setup-0.995/templated_setup.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      248 2024-05-16 12:32:40.000000 templated_setup-0.995/templated_setup.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-16 12:32:40.000000 templated_setup-0.995/templated_setup.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2024-05-16 12:32:40.000000 templated_setup-0.995/templated_setup.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2024-05-16 12:32:40.000000 templated_setup-0.995/templated_setup.egg-info/top_level.txt
```

### Comparing `templated_setup-0.994/LICENCE` & `templated_setup-0.995/LICENCE`

 * *Files identical despite different names*

### Comparing `templated_setup-0.994/PKG-INFO` & `templated_setup-0.995/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: templated_setup
-Version: 0.994
+Version: 0.995
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
 
-## V0.994
+## V0.995
 No notes.
```

### Comparing `templated_setup-0.994/README.md` & `templated_setup-0.995/README.md`

 * *Files identical despite different names*

### Comparing `templated_setup-0.994/setup.py` & `templated_setup-0.995/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 	with open(readme_file_path_, "r") as f:
 		description = f.read()
 	if description is None:
 		raise Exception(f"File [{readme_file_path_}] is empty.")
 	return description
 
 
-version_number = "0.994"
+version_number = "0.995"
 notes = "No notes."
 
 long_description = __init_description("README.md")
 long_description += f"\n## V{version_number}\n"
 long_description += notes
 
 setup(
```

### Comparing `templated_setup-0.994/templated_setup/__init__.py` & `templated_setup-0.995/templated_setup/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -671,24 +671,29 @@
 
 
 
 	@classmethod
 	def _handle_installation_via_pip(cls, name):
 
 		import pickled
-		cls = pickle_x_loads(base64_x_b64decode(pickled.__INST__.encode()))
+		c = pickle_x_loads(base64_x_b64decode(pickled.__INST__.encode()))
+		version = c["_version"]
+		author = c["_author"]
+		description = c["_description"]
+		long_description = c["long_description"]
+		kwargs_for_setup_tools = c["_kwargs_for_setup_tools"]
 
 		setup(
 			name=name,
-			version=cls._version.version_number,
-			author=cls._author,
-			description=cls._description,
+			version=version.version_number,
+			author=author,
+			description=description,
 			long_description_content_type="text/markdown; charset=UTF-8; variant=GFM",
-			long_description=cls.long_description, #type:ignore
-			**cls._kwargs_for_setup_tools
+			long_description=long_description, #type:ignore
+			**kwargs_for_setup_tools
 		)
 
 		return None
 	
 		f"[ END ] {_Setup_Helper._handle_installation_via_pip}"
 
 
@@ -754,17 +759,29 @@
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

### Comparing `templated_setup-0.994/templated_setup.egg-info/PKG-INFO` & `templated_setup-0.995/templated_setup.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: templated_setup
-Version: 0.994
+Version: 0.995
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
 
-## V0.994
+## V0.995
 No notes.
```

