# Comparing `tmp/templated_setup-0.9901.tar.gz` & `tmp/templated_setup-0.9902.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "templated_setup-0.9901.tar", last modified: Thu May 16 11:14:00 2024, max compression
+gzip compressed data, was "templated_setup-0.9902.tar", last modified: Thu May 16 11:16:53 2024, max compression
```

## Comparing `templated_setup-0.9901.tar` & `templated_setup-0.9902.tar`

### file list

```diff
@@ -1,12 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-16 11:14:00.737527 templated_setup-0.9901/
--rw-rw-rw-   0        0        0    25652 2024-03-14 11:21:06.000000 templated_setup-0.9901/LICENCE
--rw-rw-rw-   0        0        0     2555 2024-05-16 11:14:00.737016 templated_setup-0.9901/PKG-INFO
--rw-rw-rw-   0        0        0     2172 2024-04-29 06:54:31.000000 templated_setup-0.9901/README.md
--rw-rw-rw-   0        0        0       42 2024-05-16 11:14:00.738540 templated_setup-0.9901/setup.cfg
--rw-rw-rw-   0        0        0     1300 2024-05-16 11:12:38.000000 templated_setup-0.9901/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-16 11:14:00.735309 templated_setup-0.9901/templated_setup.egg-info/
--rw-rw-rw-   0        0        0     2555 2024-05-16 11:14:00.000000 templated_setup-0.9901/templated_setup.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      220 2024-05-16 11:14:00.000000 templated_setup-0.9901/templated_setup.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-16 11:14:00.000000 templated_setup-0.9901/templated_setup.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2024-05-16 11:14:00.000000 templated_setup-0.9901/templated_setup.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2024-05-16 11:14:00.000000 templated_setup-0.9901/templated_setup.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-16 11:16:53.061286 templated_setup-0.9902/
+-rw-rw-rw-   0        0        0    25652 2024-03-14 11:21:06.000000 templated_setup-0.9902/LICENCE
+-rw-rw-rw-   0        0        0     2555 2024-05-16 11:16:53.060263 templated_setup-0.9902/PKG-INFO
+-rw-rw-rw-   0        0        0     2172 2024-04-29 06:54:31.000000 templated_setup-0.9902/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-16 11:16:53.061286 templated_setup-0.9902/setup.cfg
+-rw-rw-rw-   0        0        0     1272 2024-05-16 11:16:51.000000 templated_setup-0.9902/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-16 11:16:53.050061 templated_setup-0.9902/templated_setup/
+-rw-rw-rw-   0        0        0    21014 2024-05-16 11:08:44.000000 templated_setup-0.9902/templated_setup/__init__.py
+-rw-rw-rw-   0        0        0     3271 2024-05-16 11:07:16.000000 templated_setup-0.9902/templated_setup/_hardcoded.py
+drwxrwxrwx   0        0        0        0 2024-05-16 11:16:53.058737 templated_setup-0.9902/templated_setup.egg-info/
+-rw-rw-rw-   0        0        0     2555 2024-05-16 11:16:53.000000 templated_setup-0.9902/templated_setup.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      278 2024-05-16 11:16:53.000000 templated_setup-0.9902/templated_setup.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-16 11:16:53.000000 templated_setup-0.9902/templated_setup.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2024-05-16 11:16:53.000000 templated_setup-0.9902/templated_setup.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2024-05-16 11:16:53.000000 templated_setup-0.9902/templated_setup.egg-info/top_level.txt
```

### Comparing `templated_setup-0.9901/LICENCE` & `templated_setup-0.9902/LICENCE`

 * *Files identical despite different names*

### Comparing `templated_setup-0.9901/PKG-INFO` & `templated_setup-0.9902/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: templated-setup
-Version: 0.9901
+Name: templated_setup
+Version: 0.9902
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
 
-## V0.9901
+## V0.9902
 No notes.
```

### Comparing `templated_setup-0.9901/README.md` & `templated_setup-0.9902/README.md`

 * *Files identical despite different names*

### Comparing `templated_setup-0.9901/setup.py` & `templated_setup-0.9902/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -14,28 +14,27 @@
 	with open(readme_file_path_, "r") as f:
 		description = f.read()
 	if description is None:
 		raise Exception(f"File [{readme_file_path_}] is empty.")
 	return description
 
 
-version_number = "0.9901"
+version_number = "0.9902"
 notes = "No notes."
 
 long_description = __init_description("README.md")
 long_description += f"\n## V{version_number}\n"
 long_description += notes
 
 setup(
-	name="templated-setup",
-	version="0.9901",
+	name="templated_setup",
+	version=version_number,
 	author="matrikater (Joel Watson)",
 	description=DESCRIPTION,
 	author_email="administraitor@matriko.xyz",
 	install_requires=[
 		"setuptools",
 		"twine"
 	],
 	long_description_content_type="text/markdown; charset=UTF-8; variant=GFM",
 	long_description=long_description,
-	py_modules=["templated_setup"],
 )
```

### Comparing `templated_setup-0.9901/templated_setup.egg-info/PKG-INFO` & `templated_setup-0.9902/templated_setup.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: templated-setup
-Version: 0.9901
+Name: templated_setup
+Version: 0.9902
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
 
-## V0.9901
+## V0.9902
 No notes.
```

