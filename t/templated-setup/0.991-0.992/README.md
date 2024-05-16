# Comparing `tmp/templated_setup-0.991.tar.gz` & `tmp/templated_setup-0.992.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "templated_setup-0.991.tar", last modified: Thu May 16 11:51:52 2024, max compression
+gzip compressed data, was "templated_setup-0.992.tar", last modified: Thu May 16 12:03:00 2024, max compression
```

## Comparing `templated_setup-0.991.tar` & `templated_setup-0.992.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-16 11:51:52.335076 templated_setup-0.991/
--rw-rw-rw-   0        0        0    25652 2024-03-14 11:21:06.000000 templated_setup-0.991/LICENCE
--rw-rw-rw-   0        0        0     2553 2024-05-16 11:51:52.333541 templated_setup-0.991/PKG-INFO
--rw-rw-rw-   0        0        0     2172 2024-04-29 06:54:31.000000 templated_setup-0.991/README.md
--rw-rw-rw-   0        0        0       42 2024-05-16 11:51:52.335076 templated_setup-0.991/setup.cfg
--rw-rw-rw-   0        0        0     1271 2024-05-16 11:51:49.000000 templated_setup-0.991/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-16 11:51:52.325119 templated_setup-0.991/templated_setup/
--rw-rw-rw-   0        0        0    19806 2024-05-16 11:51:40.000000 templated_setup-0.991/templated_setup/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-16 11:51:52.332524 templated_setup-0.991/templated_setup.egg-info/
--rw-rw-rw-   0        0        0     2553 2024-05-16 11:51:52.000000 templated_setup-0.991/templated_setup.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      248 2024-05-16 11:51:52.000000 templated_setup-0.991/templated_setup.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-16 11:51:52.000000 templated_setup-0.991/templated_setup.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2024-05-16 11:51:52.000000 templated_setup-0.991/templated_setup.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2024-05-16 11:51:52.000000 templated_setup-0.991/templated_setup.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-16 12:03:00.811493 templated_setup-0.992/
+-rw-rw-rw-   0        0        0    25652 2024-03-14 11:21:06.000000 templated_setup-0.992/LICENCE
+-rw-rw-rw-   0        0        0     2553 2024-05-16 12:03:00.810479 templated_setup-0.992/PKG-INFO
+-rw-rw-rw-   0        0        0     2172 2024-04-29 06:54:31.000000 templated_setup-0.992/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-16 12:03:00.812003 templated_setup-0.992/setup.cfg
+-rw-rw-rw-   0        0        0     1271 2024-05-16 12:02:55.000000 templated_setup-0.992/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-16 12:03:00.802536 templated_setup-0.992/templated_setup/
+-rw-rw-rw-   0        0        0    19875 2024-05-16 12:02:46.000000 templated_setup-0.992/templated_setup/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-16 12:03:00.809463 templated_setup-0.992/templated_setup.egg-info/
+-rw-rw-rw-   0        0        0     2553 2024-05-16 12:03:00.000000 templated_setup-0.992/templated_setup.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      248 2024-05-16 12:03:00.000000 templated_setup-0.992/templated_setup.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-16 12:03:00.000000 templated_setup-0.992/templated_setup.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2024-05-16 12:03:00.000000 templated_setup-0.992/templated_setup.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2024-05-16 12:03:00.000000 templated_setup-0.992/templated_setup.egg-info/top_level.txt
```

### Comparing `templated_setup-0.991/LICENCE` & `templated_setup-0.992/LICENCE`

 * *Files identical despite different names*

### Comparing `templated_setup-0.991/PKG-INFO` & `templated_setup-0.992/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: templated_setup
-Version: 0.991
+Version: 0.992
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
 
-## V0.991
+## V0.992
 No notes.
```

### Comparing `templated_setup-0.991/README.md` & `templated_setup-0.992/README.md`

 * *Files identical despite different names*

### Comparing `templated_setup-0.991/setup.py` & `templated_setup-0.992/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 	with open(readme_file_path_, "r") as f:
 		description = f.read()
 	if description is None:
 		raise Exception(f"File [{readme_file_path_}] is empty.")
 	return description
 
 
-version_number = "0.991"
+version_number = "0.992"
 notes = "No notes."
 
 long_description = __init_description("README.md")
 long_description += f"\n## V{version_number}\n"
 long_description += notes
 
 setup(
```

### Comparing `templated_setup-0.991/templated_setup/__init__.py` & `templated_setup-0.992/templated_setup/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -154,15 +154,15 @@
 	@staticmethod
 	def __init_description(readme_file_path_) -> "str":
 
 		description = None
 
 		try:
 			import README #type:ignore
-			return README.__README__
+			return base64_x_b64decode(README.__README__.encode()).decode()
 		except:
 			pass
 
 		if not os.path.exists(readme_file_path_):
 			raise FileNotFoundError(f"No such file or directory: [{readme_file_path_}].")
 		
 		if not os.path.isabs(readme_file_path_):
@@ -747,15 +747,15 @@
 		meta = None
 		with open(__file__, "r") as f:
 			meta = f.read()
 		with open("templated_setup.py", "w") as f:
 			f.write(meta)
 		with open(cls._readme_file_path, "r") as f:
 			readme = f.read()
-		with open("README.py") as f:
+		with open("README.py", "w") as f:
 			f.write("__README__ = \"\"\"")
 			f.write(base64_x_b64encode(readme.encode()).decode())
 			f.write("\"\"\"")
 
 		if not "py_modules" in kwargs_for_setup_tools:
 			kwargs_for_setup_tools["py_modules"] = []
 		kwargs_for_setup_tools["py_modules"].append("templated_setup")
@@ -768,14 +768,15 @@
 			description=cls._description,
 			long_description_content_type="text/markdown; charset=UTF-8; variant=GFM",
 			long_description=long_description,
 			**kwargs_for_setup_tools,
 		)
 
 		os.remove("templated_setup.py")
+		os.remove("README.py")
 
 		print("\n] Setup complete.\n\n")
 
 		do_publish = _Setup_Helper.__get_y_n("Would you like to publish to PyPi?")
 		if not do_publish:
 			exit(0)
```

### Comparing `templated_setup-0.991/templated_setup.egg-info/PKG-INFO` & `templated_setup-0.992/templated_setup.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: templated_setup
-Version: 0.991
+Version: 0.992
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
 
-## V0.991
+## V0.992
 No notes.
```

