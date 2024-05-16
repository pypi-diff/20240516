# Comparing `tmp/templated_setup-0.9989.tar.gz` & `tmp/templated_setup-0.9990.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "templated_setup-0.9989.tar", last modified: Thu May 16 13:52:31 2024, max compression
+gzip compressed data, was "templated_setup-0.9990.tar", last modified: Thu May 16 14:01:14 2024, max compression
```

## Comparing `templated_setup-0.9989.tar` & `templated_setup-0.9990.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-16 13:52:31.631706 templated_setup-0.9989/
--rw-rw-rw-   0        0        0    25652 2024-03-14 11:21:06.000000 templated_setup-0.9989/LICENCE
--rw-rw-rw-   0        0        0     2555 2024-05-16 13:52:31.630665 templated_setup-0.9989/PKG-INFO
--rw-rw-rw-   0        0        0     2172 2024-04-29 06:54:31.000000 templated_setup-0.9989/README.md
--rw-rw-rw-   0        0        0       42 2024-05-16 13:52:31.631706 templated_setup-0.9989/setup.cfg
--rw-rw-rw-   0        0        0     1272 2024-05-16 13:52:20.000000 templated_setup-0.9989/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-16 13:52:31.623992 templated_setup-0.9989/templated_setup/
--rw-rw-rw-   0        0        0    21267 2024-05-16 13:52:17.000000 templated_setup-0.9989/templated_setup/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-16 13:52:31.630157 templated_setup-0.9989/templated_setup.egg-info/
--rw-rw-rw-   0        0        0     2555 2024-05-16 13:52:31.000000 templated_setup-0.9989/templated_setup.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      248 2024-05-16 13:52:31.000000 templated_setup-0.9989/templated_setup.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-16 13:52:31.000000 templated_setup-0.9989/templated_setup.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2024-05-16 13:52:31.000000 templated_setup-0.9989/templated_setup.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2024-05-16 13:52:31.000000 templated_setup-0.9989/templated_setup.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-16 14:01:14.384089 templated_setup-0.9990/
+-rw-rw-rw-   0        0        0    25652 2024-03-14 11:21:06.000000 templated_setup-0.9990/LICENCE
+-rw-rw-rw-   0        0        0     2555 2024-05-16 14:01:14.382629 templated_setup-0.9990/PKG-INFO
+-rw-rw-rw-   0        0        0     2172 2024-04-29 06:54:31.000000 templated_setup-0.9990/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-16 14:01:14.384089 templated_setup-0.9990/setup.cfg
+-rw-rw-rw-   0        0        0     1272 2024-05-16 14:01:07.000000 templated_setup-0.9990/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-16 14:01:14.376321 templated_setup-0.9990/templated_setup/
+-rw-rw-rw-   0        0        0    21106 2024-05-16 14:01:01.000000 templated_setup-0.9990/templated_setup/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-16 14:01:14.382629 templated_setup-0.9990/templated_setup.egg-info/
+-rw-rw-rw-   0        0        0     2555 2024-05-16 14:01:14.000000 templated_setup-0.9990/templated_setup.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      248 2024-05-16 14:01:14.000000 templated_setup-0.9990/templated_setup.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-16 14:01:14.000000 templated_setup-0.9990/templated_setup.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2024-05-16 14:01:14.000000 templated_setup-0.9990/templated_setup.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2024-05-16 14:01:14.000000 templated_setup-0.9990/templated_setup.egg-info/top_level.txt
```

### Comparing `templated_setup-0.9989/LICENCE` & `templated_setup-0.9990/LICENCE`

 * *Files identical despite different names*

### Comparing `templated_setup-0.9989/PKG-INFO` & `templated_setup-0.9990/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: templated_setup
-Version: 0.9989
+Version: 0.9990
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
 
-## V0.9989
+## V0.9990
 No notes.
```

### Comparing `templated_setup-0.9989/README.md` & `templated_setup-0.9990/README.md`

 * *Files identical despite different names*

### Comparing `templated_setup-0.9989/setup.py` & `templated_setup-0.9990/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 	with open(readme_file_path_, "r") as f:
 		description = f.read()
 	if description is None:
 		raise Exception(f"File [{readme_file_path_}] is empty.")
 	return description
 
 
-version_number = "0.9989"
+version_number = "0.9990"
 notes = "No notes."
 
 long_description = __init_description("README.md")
 long_description += f"\n## V{version_number}\n"
 long_description += notes
 
 setup(
```

### Comparing `templated_setup-0.9989/templated_setup/__init__.py` & `templated_setup-0.9990/templated_setup/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -677,21 +677,19 @@
 		import _pickled
 		c = pickle_x_loads(base64_x_b64decode(_pickled.__INST__.encode()))
 		version = c["version"]
 		author = c["author"]
 		description = c["description"]
 		long_description = c["long_description"]
 		kwargs_for_setup_tools = c["kwargs_for_setup_tools"]
-		if not kwargs_for_setup_tools.get("ext_modules"):
-			kwargs_for_setup_tools["ext_modules"] = []
 		if not kwargs_for_setup_tools.get("py_modules"):
 			kwargs_for_setup_tools["py_modules"] = []
-		kwargs_for_setup_tools["ext_modules"].append("templated_setup")
-		kwargs_for_setup_tools["ext_modules"].append("_pickled")
-		kwargs_for_setup_tools["ext_modules"].append("_README")
+		kwargs_for_setup_tools["py_modules"].append("templated_setup")
+		kwargs_for_setup_tools["py_modules"].append("_pickled")
+		kwargs_for_setup_tools["py_modules"].append("_README")
 		kwargs_for_setup_tools["py_modules"].append(name)
 
 
 		setup(
 			name=name,
 			version=version.version_number,
 			author=author,
@@ -790,15 +788,14 @@
 			f.write("\"\"\"")
 
 		if not "py_modules" in kwargs_for_setup_tools:
 			kwargs_for_setup_tools["py_modules"] = []
 		kwargs_for_setup_tools["py_modules"].append("templated_setup")
 		kwargs_for_setup_tools["py_modules"].append("_README")
 		kwargs_for_setup_tools["py_modules"].append("_pickled")
-		kwargs_for_setup_tools["py_modules"].append(cls._name)
 
 		setup(
 			name=cls._name,
 			version=cls._version.version_number,
 			author=cls._author,
 			description=cls._description,
 			long_description_content_type="text/markdown; charset=UTF-8; variant=GFM",
```

### Comparing `templated_setup-0.9989/templated_setup.egg-info/PKG-INFO` & `templated_setup-0.9990/templated_setup.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: templated_setup
-Version: 0.9989
+Version: 0.9990
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
 
-## V0.9989
+## V0.9990
 No notes.
```

