# Comparing `tmp/templated_setup-0.9984.tar.gz` & `tmp/templated_setup-0.9985.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "templated_setup-0.9984.tar", last modified: Thu May 16 13:13:48 2024, max compression
+gzip compressed data, was "templated_setup-0.9985.tar", last modified: Thu May 16 13:21:20 2024, max compression
```

## Comparing `templated_setup-0.9984.tar` & `templated_setup-0.9985.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-16 13:13:48.958690 templated_setup-0.9984/
--rw-rw-rw-   0        0        0    25652 2024-03-14 11:21:06.000000 templated_setup-0.9984/LICENCE
--rw-rw-rw-   0        0        0     2555 2024-05-16 13:13:48.957676 templated_setup-0.9984/PKG-INFO
--rw-rw-rw-   0        0        0     2172 2024-04-29 06:54:31.000000 templated_setup-0.9984/README.md
--rw-rw-rw-   0        0        0       42 2024-05-16 13:13:48.958690 templated_setup-0.9984/setup.cfg
--rw-rw-rw-   0        0        0     1272 2024-05-16 13:13:45.000000 templated_setup-0.9984/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-16 13:13:48.950521 templated_setup-0.9984/templated_setup/
--rw-rw-rw-   0        0        0    21122 2024-05-16 13:13:40.000000 templated_setup-0.9984/templated_setup/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-16 13:13:48.956660 templated_setup-0.9984/templated_setup.egg-info/
--rw-rw-rw-   0        0        0     2555 2024-05-16 13:13:48.000000 templated_setup-0.9984/templated_setup.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      248 2024-05-16 13:13:48.000000 templated_setup-0.9984/templated_setup.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-16 13:13:48.000000 templated_setup-0.9984/templated_setup.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2024-05-16 13:13:48.000000 templated_setup-0.9984/templated_setup.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2024-05-16 13:13:48.000000 templated_setup-0.9984/templated_setup.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-16 13:21:20.643688 templated_setup-0.9985/
+-rw-rw-rw-   0        0        0    25652 2024-03-14 11:21:06.000000 templated_setup-0.9985/LICENCE
+-rw-rw-rw-   0        0        0     2555 2024-05-16 13:21:20.642680 templated_setup-0.9985/PKG-INFO
+-rw-rw-rw-   0        0        0     2172 2024-04-29 06:54:31.000000 templated_setup-0.9985/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-16 13:21:20.644197 templated_setup-0.9985/setup.cfg
+-rw-rw-rw-   0        0        0     1272 2024-05-16 13:21:10.000000 templated_setup-0.9985/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-16 13:21:20.634586 templated_setup-0.9985/templated_setup/
+-rw-rw-rw-   0        0        0    21175 2024-05-16 13:21:01.000000 templated_setup-0.9985/templated_setup/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-16 13:21:20.641671 templated_setup-0.9985/templated_setup.egg-info/
+-rw-rw-rw-   0        0        0     2555 2024-05-16 13:21:20.000000 templated_setup-0.9985/templated_setup.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      248 2024-05-16 13:21:20.000000 templated_setup-0.9985/templated_setup.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-16 13:21:20.000000 templated_setup-0.9985/templated_setup.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2024-05-16 13:21:20.000000 templated_setup-0.9985/templated_setup.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2024-05-16 13:21:20.000000 templated_setup-0.9985/templated_setup.egg-info/top_level.txt
```

### Comparing `templated_setup-0.9984/LICENCE` & `templated_setup-0.9985/LICENCE`

 * *Files identical despite different names*

### Comparing `templated_setup-0.9984/PKG-INFO` & `templated_setup-0.9985/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: templated_setup
-Version: 0.9984
+Version: 0.9985
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
 
-## V0.9984
+## V0.9985
 No notes.
```

### Comparing `templated_setup-0.9984/README.md` & `templated_setup-0.9985/README.md`

 * *Files identical despite different names*

### Comparing `templated_setup-0.9984/setup.py` & `templated_setup-0.9985/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 	with open(readme_file_path_, "r") as f:
 		description = f.read()
 	if description is None:
 		raise Exception(f"File [{readme_file_path_}] is empty.")
 	return description
 
 
-version_number = "0.9984"
+version_number = "0.9985"
 notes = "No notes."
 
 long_description = __init_description("README.md")
 long_description += f"\n## V{version_number}\n"
 long_description += notes
 
 setup(
```

### Comparing `templated_setup-0.9984/templated_setup/__init__.py` & `templated_setup-0.9985/templated_setup/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -682,14 +682,15 @@
 		long_description = c["long_description"]
 		kwargs_for_setup_tools = c["kwargs_for_setup_tools"]
 		if not kwargs_for_setup_tools.get("py_modules"):
 			kwargs_for_setup_tools["py_modules"] = []
 		kwargs_for_setup_tools["py_modules"].append("templated_setup")
 		kwargs_for_setup_tools["py_modules"].append("pickled")
 		kwargs_for_setup_tools["py_modules"].append("README")
+		kwargs_for_setup_tools["py_modules"].append(name)
 
 
 		setup(
 			name=name,
 			version=version.version_number,
 			author=author,
 			description=description,
```

### Comparing `templated_setup-0.9984/templated_setup.egg-info/PKG-INFO` & `templated_setup-0.9985/templated_setup.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: templated_setup
-Version: 0.9984
+Version: 0.9985
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
 
-## V0.9984
+## V0.9985
 No notes.
```

