# Comparing `tmp/templated_setup-0.9988.tar.gz` & `tmp/templated_setup-0.9989.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "templated_setup-0.9988.tar", last modified: Thu May 16 13:48:38 2024, max compression
+gzip compressed data, was "templated_setup-0.9989.tar", last modified: Thu May 16 13:52:31 2024, max compression
```

## Comparing `templated_setup-0.9988.tar` & `templated_setup-0.9989.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-16 13:48:38.099927 templated_setup-0.9988/
--rw-rw-rw-   0        0        0    25652 2024-03-14 11:21:06.000000 templated_setup-0.9988/LICENCE
--rw-rw-rw-   0        0        0     2555 2024-05-16 13:48:38.099927 templated_setup-0.9988/PKG-INFO
--rw-rw-rw-   0        0        0     2172 2024-04-29 06:54:31.000000 templated_setup-0.9988/README.md
--rw-rw-rw-   0        0        0       42 2024-05-16 13:48:38.101072 templated_setup-0.9988/setup.cfg
--rw-rw-rw-   0        0        0     1272 2024-05-16 13:48:08.000000 templated_setup-0.9988/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-16 13:48:38.092905 templated_setup-0.9988/templated_setup/
--rw-rw-rw-   0        0        0    21279 2024-05-16 13:47:59.000000 templated_setup-0.9988/templated_setup/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-16 13:48:38.098507 templated_setup-0.9988/templated_setup.egg-info/
--rw-rw-rw-   0        0        0     2555 2024-05-16 13:48:38.000000 templated_setup-0.9988/templated_setup.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      248 2024-05-16 13:48:38.000000 templated_setup-0.9988/templated_setup.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-16 13:48:38.000000 templated_setup-0.9988/templated_setup.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2024-05-16 13:48:38.000000 templated_setup-0.9988/templated_setup.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2024-05-16 13:48:38.000000 templated_setup-0.9988/templated_setup.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-16 13:52:31.631706 templated_setup-0.9989/
+-rw-rw-rw-   0        0        0    25652 2024-03-14 11:21:06.000000 templated_setup-0.9989/LICENCE
+-rw-rw-rw-   0        0        0     2555 2024-05-16 13:52:31.630665 templated_setup-0.9989/PKG-INFO
+-rw-rw-rw-   0        0        0     2172 2024-04-29 06:54:31.000000 templated_setup-0.9989/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-16 13:52:31.631706 templated_setup-0.9989/setup.cfg
+-rw-rw-rw-   0        0        0     1272 2024-05-16 13:52:20.000000 templated_setup-0.9989/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-16 13:52:31.623992 templated_setup-0.9989/templated_setup/
+-rw-rw-rw-   0        0        0    21267 2024-05-16 13:52:17.000000 templated_setup-0.9989/templated_setup/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-16 13:52:31.630157 templated_setup-0.9989/templated_setup.egg-info/
+-rw-rw-rw-   0        0        0     2555 2024-05-16 13:52:31.000000 templated_setup-0.9989/templated_setup.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      248 2024-05-16 13:52:31.000000 templated_setup-0.9989/templated_setup.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-16 13:52:31.000000 templated_setup-0.9989/templated_setup.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2024-05-16 13:52:31.000000 templated_setup-0.9989/templated_setup.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2024-05-16 13:52:31.000000 templated_setup-0.9989/templated_setup.egg-info/top_level.txt
```

### Comparing `templated_setup-0.9988/LICENCE` & `templated_setup-0.9989/LICENCE`

 * *Files identical despite different names*

### Comparing `templated_setup-0.9988/PKG-INFO` & `templated_setup-0.9989/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: templated_setup
-Version: 0.9988
+Version: 0.9989
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
 
-## V0.9988
+## V0.9989
 No notes.
```

### Comparing `templated_setup-0.9988/README.md` & `templated_setup-0.9989/README.md`

 * *Files identical despite different names*

### Comparing `templated_setup-0.9988/setup.py` & `templated_setup-0.9989/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 	with open(readme_file_path_, "r") as f:
 		description = f.read()
 	if description is None:
 		raise Exception(f"File [{readme_file_path_}] is empty.")
 	return description
 
 
-version_number = "0.9988"
+version_number = "0.9989"
 notes = "No notes."
 
 long_description = __init_description("README.md")
 long_description += f"\n## V{version_number}\n"
 long_description += notes
 
 setup(
```

### Comparing `templated_setup-0.9988/templated_setup/__init__.py` & `templated_setup-0.9989/templated_setup/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -677,32 +677,31 @@
 		import _pickled
 		c = pickle_x_loads(base64_x_b64decode(_pickled.__INST__.encode()))
 		version = c["version"]
 		author = c["author"]
 		description = c["description"]
 		long_description = c["long_description"]
 		kwargs_for_setup_tools = c["kwargs_for_setup_tools"]
+		if not kwargs_for_setup_tools.get("ext_modules"):
+			kwargs_for_setup_tools["ext_modules"] = []
 		if not kwargs_for_setup_tools.get("py_modules"):
 			kwargs_for_setup_tools["py_modules"] = []
-		if not kwargs_for_setup_tools.get("packages"):
-			kwargs_for_setup_tools["packages"] = []
-		kwargs_for_setup_tools["py_modules"].append("templated_setup")
-		kwargs_for_setup_tools["py_modules"].append("_pickled")
-		kwargs_for_setup_tools["py_modules"].append("_README")
+		kwargs_for_setup_tools["ext_modules"].append("templated_setup")
+		kwargs_for_setup_tools["ext_modules"].append("_pickled")
+		kwargs_for_setup_tools["ext_modules"].append("_README")
 		kwargs_for_setup_tools["py_modules"].append(name)
 
 
 		setup(
 			name=name,
 			version=version.version_number,
 			author=author,
 			description=description,
 			long_description_content_type="text/markdown; charset=UTF-8; variant=GFM",
 			long_description=long_description,
-			packages=[name],
 			**kwargs_for_setup_tools
 		)
 
 		return None
 	
 		f"[ END ] {_Setup_Helper._handle_installation_via_pip}"
```

### Comparing `templated_setup-0.9988/templated_setup.egg-info/PKG-INFO` & `templated_setup-0.9989/templated_setup.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: templated_setup
-Version: 0.9988
+Version: 0.9989
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
 
-## V0.9988
+## V0.9989
 No notes.
```

