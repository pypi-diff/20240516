# Comparing `tmp/templated_setup-0.992.tar.gz` & `tmp/templated_setup-0.993.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "templated_setup-0.992.tar", last modified: Thu May 16 12:03:00 2024, max compression
+gzip compressed data, was "templated_setup-0.993.tar", last modified: Thu May 16 12:11:56 2024, max compression
```

## Comparing `templated_setup-0.992.tar` & `templated_setup-0.993.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-16 12:03:00.811493 templated_setup-0.992/
--rw-rw-rw-   0        0        0    25652 2024-03-14 11:21:06.000000 templated_setup-0.992/LICENCE
--rw-rw-rw-   0        0        0     2553 2024-05-16 12:03:00.810479 templated_setup-0.992/PKG-INFO
--rw-rw-rw-   0        0        0     2172 2024-04-29 06:54:31.000000 templated_setup-0.992/README.md
--rw-rw-rw-   0        0        0       42 2024-05-16 12:03:00.812003 templated_setup-0.992/setup.cfg
--rw-rw-rw-   0        0        0     1271 2024-05-16 12:02:55.000000 templated_setup-0.992/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-16 12:03:00.802536 templated_setup-0.992/templated_setup/
--rw-rw-rw-   0        0        0    19875 2024-05-16 12:02:46.000000 templated_setup-0.992/templated_setup/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-16 12:03:00.809463 templated_setup-0.992/templated_setup.egg-info/
--rw-rw-rw-   0        0        0     2553 2024-05-16 12:03:00.000000 templated_setup-0.992/templated_setup.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      248 2024-05-16 12:03:00.000000 templated_setup-0.992/templated_setup.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-16 12:03:00.000000 templated_setup-0.992/templated_setup.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2024-05-16 12:03:00.000000 templated_setup-0.992/templated_setup.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2024-05-16 12:03:00.000000 templated_setup-0.992/templated_setup.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-16 12:11:56.185773 templated_setup-0.993/
+-rw-rw-rw-   0        0        0    25652 2024-03-14 11:21:06.000000 templated_setup-0.993/LICENCE
+-rw-rw-rw-   0        0        0     2553 2024-05-16 12:11:56.184266 templated_setup-0.993/PKG-INFO
+-rw-rw-rw-   0        0        0     2172 2024-04-29 06:54:31.000000 templated_setup-0.993/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-16 12:11:56.185773 templated_setup-0.993/setup.cfg
+-rw-rw-rw-   0        0        0     1271 2024-05-16 12:11:51.000000 templated_setup-0.993/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-16 12:11:56.178119 templated_setup-0.993/templated_setup/
+-rw-rw-rw-   0        0        0    20148 2024-05-16 12:11:36.000000 templated_setup-0.993/templated_setup/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-16 12:11:56.184266 templated_setup-0.993/templated_setup.egg-info/
+-rw-rw-rw-   0        0        0     2553 2024-05-16 12:11:56.000000 templated_setup-0.993/templated_setup.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      248 2024-05-16 12:11:56.000000 templated_setup-0.993/templated_setup.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-16 12:11:56.000000 templated_setup-0.993/templated_setup.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2024-05-16 12:11:56.000000 templated_setup-0.993/templated_setup.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2024-05-16 12:11:56.000000 templated_setup-0.993/templated_setup.egg-info/top_level.txt
```

### Comparing `templated_setup-0.992/LICENCE` & `templated_setup-0.993/LICENCE`

 * *Files identical despite different names*

### Comparing `templated_setup-0.992/PKG-INFO` & `templated_setup-0.993/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: templated_setup
-Version: 0.992
+Version: 0.993
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
 
-## V0.992
+## V0.993
 No notes.
```

### Comparing `templated_setup-0.992/README.md` & `templated_setup-0.993/README.md`

 * *Files identical despite different names*

### Comparing `templated_setup-0.992/setup.py` & `templated_setup-0.993/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 	with open(readme_file_path_, "r") as f:
 		description = f.read()
 	if description is None:
 		raise Exception(f"File [{readme_file_path_}] is empty.")
 	return description
 
 
-version_number = "0.992"
+version_number = "0.993"
 notes = "No notes."
 
 long_description = __init_description("README.md")
 long_description += f"\n## V{version_number}\n"
 long_description += notes
 
 setup(
```

### Comparing `templated_setup-0.992/templated_setup/__init__.py` & `templated_setup-0.993/templated_setup/__init__.py`

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

### Comparing `templated_setup-0.992/templated_setup.egg-info/PKG-INFO` & `templated_setup-0.993/templated_setup.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: templated_setup
-Version: 0.992
+Version: 0.993
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
 
-## V0.992
+## V0.993
 No notes.
```

