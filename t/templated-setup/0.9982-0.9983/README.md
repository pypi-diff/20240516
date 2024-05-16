# Comparing `tmp/templated_setup-0.9982.tar.gz` & `tmp/templated_setup-0.9983.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "templated_setup-0.9982.tar", last modified: Thu May 16 12:58:39 2024, max compression
+gzip compressed data, was "templated_setup-0.9983.tar", last modified: Thu May 16 13:10:08 2024, max compression
```

## Comparing `templated_setup-0.9982.tar` & `templated_setup-0.9983.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-16 12:58:39.565130 templated_setup-0.9982/
--rw-rw-rw-   0        0        0    25652 2024-03-14 11:21:06.000000 templated_setup-0.9982/LICENCE
--rw-rw-rw-   0        0        0     2555 2024-05-16 12:58:39.564113 templated_setup-0.9982/PKG-INFO
--rw-rw-rw-   0        0        0     2172 2024-04-29 06:54:31.000000 templated_setup-0.9982/README.md
--rw-rw-rw-   0        0        0       42 2024-05-16 12:58:39.565130 templated_setup-0.9982/setup.cfg
--rw-rw-rw-   0        0        0     1272 2024-05-16 12:58:34.000000 templated_setup-0.9982/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-16 12:58:39.556479 templated_setup-0.9982/templated_setup/
--rw-rw-rw-   0        0        0    21056 2024-05-16 12:57:50.000000 templated_setup-0.9982/templated_setup/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-16 12:58:39.563099 templated_setup-0.9982/templated_setup.egg-info/
--rw-rw-rw-   0        0        0     2555 2024-05-16 12:58:39.000000 templated_setup-0.9982/templated_setup.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      248 2024-05-16 12:58:39.000000 templated_setup-0.9982/templated_setup.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-16 12:58:39.000000 templated_setup-0.9982/templated_setup.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2024-05-16 12:58:39.000000 templated_setup-0.9982/templated_setup.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2024-05-16 12:58:39.000000 templated_setup-0.9982/templated_setup.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-16 13:10:08.741820 templated_setup-0.9983/
+-rw-rw-rw-   0        0        0    25652 2024-03-14 11:21:06.000000 templated_setup-0.9983/LICENCE
+-rw-rw-rw-   0        0        0     2555 2024-05-16 13:10:08.740815 templated_setup-0.9983/PKG-INFO
+-rw-rw-rw-   0        0        0     2172 2024-04-29 06:54:31.000000 templated_setup-0.9983/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-16 13:10:08.741820 templated_setup-0.9983/setup.cfg
+-rw-rw-rw-   0        0        0     1272 2024-05-16 13:09:55.000000 templated_setup-0.9983/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-16 13:10:08.734399 templated_setup-0.9983/templated_setup/
+-rw-rw-rw-   0        0        0    21120 2024-05-16 13:09:39.000000 templated_setup-0.9983/templated_setup/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-16 13:10:08.739709 templated_setup-0.9983/templated_setup.egg-info/
+-rw-rw-rw-   0        0        0     2555 2024-05-16 13:10:08.000000 templated_setup-0.9983/templated_setup.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      248 2024-05-16 13:10:08.000000 templated_setup-0.9983/templated_setup.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-16 13:10:08.000000 templated_setup-0.9983/templated_setup.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2024-05-16 13:10:08.000000 templated_setup-0.9983/templated_setup.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2024-05-16 13:10:08.000000 templated_setup-0.9983/templated_setup.egg-info/top_level.txt
```

### Comparing `templated_setup-0.9982/LICENCE` & `templated_setup-0.9983/LICENCE`

 * *Files identical despite different names*

### Comparing `templated_setup-0.9982/PKG-INFO` & `templated_setup-0.9983/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: templated_setup
-Version: 0.9982
+Version: 0.9983
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
 
-## V0.9982
+## V0.9983
 No notes.
```

### Comparing `templated_setup-0.9982/README.md` & `templated_setup-0.9983/README.md`

 * *Files identical despite different names*

### Comparing `templated_setup-0.9982/setup.py` & `templated_setup-0.9983/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 	with open(readme_file_path_, "r") as f:
 		description = f.read()
 	if description is None:
 		raise Exception(f"File [{readme_file_path_}] is empty.")
 	return description
 
 
-version_number = "0.9982"
+version_number = "0.9983"
 notes = "No notes."
 
 long_description = __init_description("README.md")
 long_description += f"\n## V{version_number}\n"
 long_description += notes
 
 setup(
```

### Comparing `templated_setup-0.9982/templated_setup/__init__.py` & `templated_setup-0.9983/templated_setup/__init__.py`

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

### Comparing `templated_setup-0.9982/templated_setup.egg-info/PKG-INFO` & `templated_setup-0.9983/templated_setup.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: templated_setup
-Version: 0.9982
+Version: 0.9983
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
 
-## V0.9982
+## V0.9983
 No notes.
```

