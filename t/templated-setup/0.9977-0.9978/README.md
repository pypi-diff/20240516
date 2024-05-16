# Comparing `tmp/templated_setup-0.9977.tar.gz` & `tmp/templated_setup-0.9978.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "templated_setup-0.9977.tar", last modified: Thu May 16 12:42:15 2024, max compression
+gzip compressed data, was "templated_setup-0.9978.tar", last modified: Thu May 16 12:45:30 2024, max compression
```

## Comparing `templated_setup-0.9977.tar` & `templated_setup-0.9978.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-16 12:42:15.898018 templated_setup-0.9977/
--rw-rw-rw-   0        0        0    25652 2024-03-14 11:21:06.000000 templated_setup-0.9977/LICENCE
--rw-rw-rw-   0        0        0     2555 2024-05-16 12:42:15.896677 templated_setup-0.9977/PKG-INFO
--rw-rw-rw-   0        0        0     2172 2024-04-29 06:54:31.000000 templated_setup-0.9977/README.md
--rw-rw-rw-   0        0        0       42 2024-05-16 12:42:15.898018 templated_setup-0.9977/setup.cfg
--rw-rw-rw-   0        0        0     1272 2024-05-16 12:42:13.000000 templated_setup-0.9977/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-16 12:42:15.888280 templated_setup-0.9977/templated_setup/
--rw-rw-rw-   0        0        0    20947 2024-05-16 12:41:35.000000 templated_setup-0.9977/templated_setup/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-16 12:42:15.895633 templated_setup-0.9977/templated_setup.egg-info/
--rw-rw-rw-   0        0        0     2555 2024-05-16 12:42:15.000000 templated_setup-0.9977/templated_setup.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      248 2024-05-16 12:42:15.000000 templated_setup-0.9977/templated_setup.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-16 12:42:15.000000 templated_setup-0.9977/templated_setup.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2024-05-16 12:42:15.000000 templated_setup-0.9977/templated_setup.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2024-05-16 12:42:15.000000 templated_setup-0.9977/templated_setup.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-16 12:45:30.865188 templated_setup-0.9978/
+-rw-rw-rw-   0        0        0    25652 2024-03-14 11:21:06.000000 templated_setup-0.9978/LICENCE
+-rw-rw-rw-   0        0        0     2555 2024-05-16 12:45:30.864679 templated_setup-0.9978/PKG-INFO
+-rw-rw-rw-   0        0        0     2172 2024-04-29 06:54:31.000000 templated_setup-0.9978/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-16 12:45:30.865188 templated_setup-0.9978/setup.cfg
+-rw-rw-rw-   0        0        0     1272 2024-05-16 12:45:26.000000 templated_setup-0.9978/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-16 12:45:30.857290 templated_setup-0.9978/templated_setup/
+-rw-rw-rw-   0        0        0    20994 2024-05-16 12:45:23.000000 templated_setup-0.9978/templated_setup/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-16 12:45:30.863658 templated_setup-0.9978/templated_setup.egg-info/
+-rw-rw-rw-   0        0        0     2555 2024-05-16 12:45:30.000000 templated_setup-0.9978/templated_setup.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      248 2024-05-16 12:45:30.000000 templated_setup-0.9978/templated_setup.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-16 12:45:30.000000 templated_setup-0.9978/templated_setup.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2024-05-16 12:45:30.000000 templated_setup-0.9978/templated_setup.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2024-05-16 12:45:30.000000 templated_setup-0.9978/templated_setup.egg-info/top_level.txt
```

### Comparing `templated_setup-0.9977/LICENCE` & `templated_setup-0.9978/LICENCE`

 * *Files identical despite different names*

### Comparing `templated_setup-0.9977/PKG-INFO` & `templated_setup-0.9978/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: templated_setup
-Version: 0.9977
+Version: 0.9978
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
 
-## V0.9977
+## V0.9978
 No notes.
```

### Comparing `templated_setup-0.9977/README.md` & `templated_setup-0.9978/README.md`

 * *Files identical despite different names*

### Comparing `templated_setup-0.9977/setup.py` & `templated_setup-0.9978/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 	with open(readme_file_path_, "r") as f:
 		description = f.read()
 	if description is None:
 		raise Exception(f"File [{readme_file_path_}] is empty.")
 	return description
 
 
-version_number = "0.9977"
+version_number = "0.9978"
 notes = "No notes."
 
 long_description = __init_description("README.md")
 long_description += f"\n## V{version_number}\n"
 long_description += notes
 
 setup(
```

### Comparing `templated_setup-0.9977/templated_setup/__init__.py` & `templated_setup-0.9978/templated_setup/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -677,17 +677,20 @@
 		import pickled
 		c = pickle_x_loads(base64_x_b64decode(pickled.__INST__.encode()))
 		version = c["version"]
 		author = c["author"]
 		description = c["description"]
 		long_description = c["long_description"]
 		kwargs_for_setup_tools = c["kwargs_for_setup_tools"]
-		kwargs_for_setup_tools["py_modules"].pop("templated_setup")
-		kwargs_for_setup_tools["py_modules"].pop("README")
-		kwargs_for_setup_tools["py_modules"].pop("pickled")
+		if not kwargs_for_setup_tools.get("py_modules"):
+			kwargs_for_setup_tools["py_modules"] = []
+		kwargs_for_setup_tools["py_modules"].append("templated_setup")
+
+		os.remove("pickled.py")
+		os.remove("README.py")
 
 		setup(
 			name=name,
 			version=version.version_number,
 			author=author,
 			description=description,
 			long_description_content_type="text/markdown; charset=UTF-8; variant=GFM",
```

### Comparing `templated_setup-0.9977/templated_setup.egg-info/PKG-INFO` & `templated_setup-0.9978/templated_setup.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: templated_setup
-Version: 0.9977
+Version: 0.9978
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
 
-## V0.9977
+## V0.9978
 No notes.
```
