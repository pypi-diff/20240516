# Comparing `tmp/templated_setup-0.993.tar.gz` & `tmp/templated_setup-0.994.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "templated_setup-0.993.tar", last modified: Thu May 16 12:11:56 2024, max compression
+gzip compressed data, was "templated_setup-0.994.tar", last modified: Thu May 16 12:14:58 2024, max compression
```

## Comparing `templated_setup-0.993.tar` & `templated_setup-0.994.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-16 12:11:56.185773 templated_setup-0.993/
--rw-rw-rw-   0        0        0    25652 2024-03-14 11:21:06.000000 templated_setup-0.993/LICENCE
--rw-rw-rw-   0        0        0     2553 2024-05-16 12:11:56.184266 templated_setup-0.993/PKG-INFO
--rw-rw-rw-   0        0        0     2172 2024-04-29 06:54:31.000000 templated_setup-0.993/README.md
--rw-rw-rw-   0        0        0       42 2024-05-16 12:11:56.185773 templated_setup-0.993/setup.cfg
--rw-rw-rw-   0        0        0     1271 2024-05-16 12:11:51.000000 templated_setup-0.993/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-16 12:11:56.178119 templated_setup-0.993/templated_setup/
--rw-rw-rw-   0        0        0    20148 2024-05-16 12:11:36.000000 templated_setup-0.993/templated_setup/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-16 12:11:56.184266 templated_setup-0.993/templated_setup.egg-info/
--rw-rw-rw-   0        0        0     2553 2024-05-16 12:11:56.000000 templated_setup-0.993/templated_setup.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      248 2024-05-16 12:11:56.000000 templated_setup-0.993/templated_setup.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-16 12:11:56.000000 templated_setup-0.993/templated_setup.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2024-05-16 12:11:56.000000 templated_setup-0.993/templated_setup.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2024-05-16 12:11:56.000000 templated_setup-0.993/templated_setup.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-16 12:14:58.128693 templated_setup-0.994/
+-rw-rw-rw-   0        0        0    25652 2024-03-14 11:21:06.000000 templated_setup-0.994/LICENCE
+-rw-rw-rw-   0        0        0     2553 2024-05-16 12:14:58.127281 templated_setup-0.994/PKG-INFO
+-rw-rw-rw-   0        0        0     2172 2024-04-29 06:54:31.000000 templated_setup-0.994/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-16 12:14:58.128693 templated_setup-0.994/setup.cfg
+-rw-rw-rw-   0        0        0     1271 2024-05-16 12:14:55.000000 templated_setup-0.994/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-16 12:14:58.119602 templated_setup-0.994/templated_setup/
+-rw-rw-rw-   0        0        0    20206 2024-05-16 12:14:49.000000 templated_setup-0.994/templated_setup/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-16 12:14:58.126255 templated_setup-0.994/templated_setup.egg-info/
+-rw-rw-rw-   0        0        0     2553 2024-05-16 12:14:58.000000 templated_setup-0.994/templated_setup.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      248 2024-05-16 12:14:58.000000 templated_setup-0.994/templated_setup.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-16 12:14:58.000000 templated_setup-0.994/templated_setup.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2024-05-16 12:14:58.000000 templated_setup-0.994/templated_setup.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2024-05-16 12:14:58.000000 templated_setup-0.994/templated_setup.egg-info/top_level.txt
```

### Comparing `templated_setup-0.993/LICENCE` & `templated_setup-0.994/LICENCE`

 * *Files identical despite different names*

### Comparing `templated_setup-0.993/PKG-INFO` & `templated_setup-0.994/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: templated_setup
-Version: 0.993
+Version: 0.994
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
 
-## V0.993
+## V0.994
 No notes.
```

### Comparing `templated_setup-0.993/README.md` & `templated_setup-0.994/README.md`

 * *Files identical despite different names*

### Comparing `templated_setup-0.993/setup.py` & `templated_setup-0.994/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 	with open(readme_file_path_, "r") as f:
 		description = f.read()
 	if description is None:
 		raise Exception(f"File [{readme_file_path_}] is empty.")
 	return description
 
 
-version_number = "0.993"
+version_number = "0.994"
 notes = "No notes."
 
 long_description = __init_description("README.md")
 long_description += f"\n## V{version_number}\n"
 long_description += notes
 
 setup(
```

### Comparing `templated_setup-0.993/templated_setup/__init__.py` & `templated_setup-0.994/templated_setup/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -763,14 +763,15 @@
 			f.write(base64_x_b64encode(pickle_x_dumps(cls)).decode())
 			f.write("\"\"\"")
 
 		if not "py_modules" in kwargs_for_setup_tools:
 			kwargs_for_setup_tools["py_modules"] = []
 		kwargs_for_setup_tools["py_modules"].append("templated_setup")
 		kwargs_for_setup_tools["py_modules"].append("README")
+		kwargs_for_setup_tools["py_modules"].append("pickled")
 
 		setup(
 			name=cls._name,
 			version=cls._version.version_number,
 			author=cls._author,
 			description=cls._description,
 			long_description_content_type="text/markdown; charset=UTF-8; variant=GFM",
```

### Comparing `templated_setup-0.993/templated_setup.egg-info/PKG-INFO` & `templated_setup-0.994/templated_setup.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: templated_setup
-Version: 0.993
+Version: 0.994
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
 
-## V0.993
+## V0.994
 No notes.
```

