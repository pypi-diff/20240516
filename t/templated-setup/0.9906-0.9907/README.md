# Comparing `tmp/templated_setup-0.9906.tar.gz` & `tmp/templated_setup-0.9907.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "templated_setup-0.9906.tar", last modified: Thu May 16 11:30:29 2024, max compression
+gzip compressed data, was "templated_setup-0.9907.tar", last modified: Thu May 16 11:36:10 2024, max compression
```

## Comparing `templated_setup-0.9906.tar` & `templated_setup-0.9907.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-16 11:30:29.493188 templated_setup-0.9906/
--rw-rw-rw-   0        0        0    25652 2024-03-14 11:21:06.000000 templated_setup-0.9906/LICENCE
--rw-rw-rw-   0        0        0     2555 2024-05-16 11:30:29.492170 templated_setup-0.9906/PKG-INFO
--rw-rw-rw-   0        0        0     2172 2024-04-29 06:54:31.000000 templated_setup-0.9906/README.md
--rw-rw-rw-   0        0        0       42 2024-05-16 11:30:29.493188 templated_setup-0.9906/setup.cfg
--rw-rw-rw-   0        0        0     1272 2024-05-16 11:30:25.000000 templated_setup-0.9906/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-16 11:30:29.484399 templated_setup-0.9906/templated_setup/
--rw-rw-rw-   0        0        0    21007 2024-05-16 11:30:19.000000 templated_setup-0.9906/templated_setup/__init__.py
--rw-rw-rw-   0        0        0     3271 2024-05-16 11:07:16.000000 templated_setup-0.9906/templated_setup/_hardcoded.py
-drwxrwxrwx   0        0        0        0 2024-05-16 11:30:29.491047 templated_setup-0.9906/templated_setup.egg-info/
--rw-rw-rw-   0        0        0     2555 2024-05-16 11:30:29.000000 templated_setup-0.9906/templated_setup.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      278 2024-05-16 11:30:29.000000 templated_setup-0.9906/templated_setup.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-16 11:30:29.000000 templated_setup-0.9906/templated_setup.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2024-05-16 11:30:29.000000 templated_setup-0.9906/templated_setup.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2024-05-16 11:30:29.000000 templated_setup-0.9906/templated_setup.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-16 11:36:10.827906 templated_setup-0.9907/
+-rw-rw-rw-   0        0        0    25652 2024-03-14 11:21:06.000000 templated_setup-0.9907/LICENCE
+-rw-rw-rw-   0        0        0     2555 2024-05-16 11:36:10.826902 templated_setup-0.9907/PKG-INFO
+-rw-rw-rw-   0        0        0     2172 2024-04-29 06:54:31.000000 templated_setup-0.9907/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-16 11:36:10.828410 templated_setup-0.9907/setup.cfg
+-rw-rw-rw-   0        0        0     1272 2024-05-16 11:35:57.000000 templated_setup-0.9907/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-16 11:36:10.819298 templated_setup-0.9907/templated_setup/
+-rw-rw-rw-   0        0        0    20728 2024-05-16 11:35:42.000000 templated_setup-0.9907/templated_setup/__init__.py
+-rw-rw-rw-   0        0        0     3271 2024-05-16 11:07:16.000000 templated_setup-0.9907/templated_setup/_hardcoded.py
+drwxrwxrwx   0        0        0        0 2024-05-16 11:36:10.825871 templated_setup-0.9907/templated_setup.egg-info/
+-rw-rw-rw-   0        0        0     2555 2024-05-16 11:36:10.000000 templated_setup-0.9907/templated_setup.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      278 2024-05-16 11:36:10.000000 templated_setup-0.9907/templated_setup.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-16 11:36:10.000000 templated_setup-0.9907/templated_setup.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2024-05-16 11:36:10.000000 templated_setup-0.9907/templated_setup.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2024-05-16 11:36:10.000000 templated_setup-0.9907/templated_setup.egg-info/top_level.txt
```

### Comparing `templated_setup-0.9906/LICENCE` & `templated_setup-0.9907/LICENCE`

 * *Files identical despite different names*

### Comparing `templated_setup-0.9906/PKG-INFO` & `templated_setup-0.9907/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: templated_setup
-Version: 0.9906
+Version: 0.9907
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
 
-## V0.9906
+## V0.9907
 No notes.
```

### Comparing `templated_setup-0.9906/README.md` & `templated_setup-0.9907/README.md`

 * *Files identical despite different names*

### Comparing `templated_setup-0.9906/setup.py` & `templated_setup-0.9907/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 	with open(readme_file_path_, "r") as f:
 		description = f.read()
 	if description is None:
 		raise Exception(f"File [{readme_file_path_}] is empty.")
 	return description
 
 
-version_number = "0.9906"
+version_number = "0.9907"
 notes = "No notes."
 
 long_description = __init_description("README.md")
 long_description += f"\n## V{version_number}\n"
 long_description += notes
 
 setup(
```

### Comparing `templated_setup-0.9906/templated_setup/__init__.py` & `templated_setup-0.9907/templated_setup/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -665,24 +665,15 @@
 
 
 	@classmethod
 	def _handle_installation_via_pip(cls, name):
 
 		# NOTE: If we do not hardcode the version, then pip will throw a fit when trying to install the 
 		# NOTE:   `templated-setup` package.
-		try:
-			from . import _hardcoded #type:ignore
-		except ImportError:
-			with open("_hardcoded.py", "w") as f:
-				f.write("__version__ = \"0.0\"\n")
-				f.write("__author__ = \"\"\n")
-				f.write("__description__ = \"\"\n")
-				f.write("__long_description__ = \"\"\"\"\"\"\n")
-				f.write("__kwargs_for_setup_tools__ = \"\"\"\"\"\"\n")
-			import _hardcoded #type:ignore
+		from . import _hardcoded #type:ignore
 		kwargs_for_setup_tools = base64_x_b64decode(_hardcoded.__kwargs_for_setup_tools__.encode("utf-8")) #type:ignore
 		kwargs_for_setup_tools = pickle_x_loads(kwargs_for_setup_tools)
 		long_description = base64_x_b64decode(_hardcoded.__long_description__.encode("utf-8")) #type:ignore
 		long_description = pickle_x_loads(long_description)
 		setup(
 			name=name,
 			version=_hardcoded.__version__, #type:ignore
@@ -768,14 +759,15 @@
 			meta = f.read()
 		with open("templated_setup.py", "w") as f:
 			f.write(meta)
 
 		if not "py_modules" in kwargs_for_setup_tools:
 			kwargs_for_setup_tools["py_modules"] = []
 		kwargs_for_setup_tools["py_modules"].append("templated_setup")
+		kwargs_for_setup_tools["py_modules"].append("_hardcoded")
 
 		setup(
 			name=cls._name,
 			version=cls._version.version_number,
 			author=cls._author,
 			description=cls._description,
 			long_description_content_type="text/markdown; charset=UTF-8; variant=GFM",
```

### Comparing `templated_setup-0.9906/templated_setup/_hardcoded.py` & `templated_setup-0.9907/templated_setup/_hardcoded.py`

 * *Files identical despite different names*

### Comparing `templated_setup-0.9906/templated_setup.egg-info/PKG-INFO` & `templated_setup-0.9907/templated_setup.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: templated_setup
-Version: 0.9906
+Version: 0.9907
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
 
-## V0.9906
+## V0.9907
 No notes.
```

