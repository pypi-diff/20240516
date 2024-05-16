# Comparing `tmp/templated_setup-0.9902.tar.gz` & `tmp/templated_setup-0.9903.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "templated_setup-0.9902.tar", last modified: Thu May 16 11:16:53 2024, max compression
+gzip compressed data, was "templated_setup-0.9903.tar", last modified: Thu May 16 11:21:14 2024, max compression
```

## Comparing `templated_setup-0.9902.tar` & `templated_setup-0.9903.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-16 11:16:53.061286 templated_setup-0.9902/
--rw-rw-rw-   0        0        0    25652 2024-03-14 11:21:06.000000 templated_setup-0.9902/LICENCE
--rw-rw-rw-   0        0        0     2555 2024-05-16 11:16:53.060263 templated_setup-0.9902/PKG-INFO
--rw-rw-rw-   0        0        0     2172 2024-04-29 06:54:31.000000 templated_setup-0.9902/README.md
--rw-rw-rw-   0        0        0       42 2024-05-16 11:16:53.061286 templated_setup-0.9902/setup.cfg
--rw-rw-rw-   0        0        0     1272 2024-05-16 11:16:51.000000 templated_setup-0.9902/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-16 11:16:53.050061 templated_setup-0.9902/templated_setup/
--rw-rw-rw-   0        0        0    21014 2024-05-16 11:08:44.000000 templated_setup-0.9902/templated_setup/__init__.py
--rw-rw-rw-   0        0        0     3271 2024-05-16 11:07:16.000000 templated_setup-0.9902/templated_setup/_hardcoded.py
-drwxrwxrwx   0        0        0        0 2024-05-16 11:16:53.058737 templated_setup-0.9902/templated_setup.egg-info/
--rw-rw-rw-   0        0        0     2555 2024-05-16 11:16:53.000000 templated_setup-0.9902/templated_setup.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      278 2024-05-16 11:16:53.000000 templated_setup-0.9902/templated_setup.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-16 11:16:53.000000 templated_setup-0.9902/templated_setup.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2024-05-16 11:16:53.000000 templated_setup-0.9902/templated_setup.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2024-05-16 11:16:53.000000 templated_setup-0.9902/templated_setup.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-16 11:21:14.132376 templated_setup-0.9903/
+-rw-rw-rw-   0        0        0    25652 2024-03-14 11:21:06.000000 templated_setup-0.9903/LICENCE
+-rw-rw-rw-   0        0        0     2555 2024-05-16 11:21:14.132376 templated_setup-0.9903/PKG-INFO
+-rw-rw-rw-   0        0        0     2172 2024-04-29 06:54:31.000000 templated_setup-0.9903/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-16 11:21:14.133397 templated_setup-0.9903/setup.cfg
+-rw-rw-rw-   0        0        0     1272 2024-05-16 11:21:06.000000 templated_setup-0.9903/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-16 11:21:14.124574 templated_setup-0.9903/templated_setup/
+-rw-rw-rw-   0        0        0    21071 2024-05-16 11:21:01.000000 templated_setup-0.9903/templated_setup/__init__.py
+-rw-rw-rw-   0        0        0     3271 2024-05-16 11:07:16.000000 templated_setup-0.9903/templated_setup/_hardcoded.py
+drwxrwxrwx   0        0        0        0 2024-05-16 11:21:14.131358 templated_setup-0.9903/templated_setup.egg-info/
+-rw-rw-rw-   0        0        0     2555 2024-05-16 11:21:14.000000 templated_setup-0.9903/templated_setup.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      278 2024-05-16 11:21:14.000000 templated_setup-0.9903/templated_setup.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-16 11:21:14.000000 templated_setup-0.9903/templated_setup.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2024-05-16 11:21:14.000000 templated_setup-0.9903/templated_setup.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2024-05-16 11:21:14.000000 templated_setup-0.9903/templated_setup.egg-info/top_level.txt
```

### Comparing `templated_setup-0.9902/LICENCE` & `templated_setup-0.9903/LICENCE`

 * *Files identical despite different names*

### Comparing `templated_setup-0.9902/PKG-INFO` & `templated_setup-0.9903/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: templated_setup
-Version: 0.9902
+Version: 0.9903
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
 
-## V0.9902
+## V0.9903
 No notes.
```

### Comparing `templated_setup-0.9902/README.md` & `templated_setup-0.9903/README.md`

 * *Files identical despite different names*

### Comparing `templated_setup-0.9902/setup.py` & `templated_setup-0.9903/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 	with open(readme_file_path_, "r") as f:
 		description = f.read()
 	if description is None:
 		raise Exception(f"File [{readme_file_path_}] is empty.")
 	return description
 
 
-version_number = "0.9902"
+version_number = "0.9903"
 notes = "No notes."
 
 long_description = __init_description("README.md")
 long_description += f"\n## V{version_number}\n"
 long_description += notes
 
 setup(
```

### Comparing `templated_setup-0.9902/templated_setup/__init__.py` & `templated_setup-0.9903/templated_setup/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -674,14 +674,16 @@
 		except ImportError:
 			with open("_hardcoded.py", "w") as f:
 				f.write("__version__ = \"0.0\"\n")
 				f.write("__author__ = \"\"\n")
 				f.write("__description__ = \"\"\n")
 				f.write("__long_description__ = \"\"\"\"\"\"\n")
 				f.write("__kwargs_for_setup_tools__ = \"\"\"\"\"\"\n")
+			with open("__init__.py", "w") as f:
+				f.write("")
 			from . import _hardcoded #type:ignore
 		kwargs_for_setup_tools = base64_x_b64decode(_hardcoded.__kwargs_for_setup_tools__.encode("utf-8")) #type:ignore
 		kwargs_for_setup_tools = pickle_x_loads(kwargs_for_setup_tools)
 		long_description = base64_x_b64decode(_hardcoded.__long_description__.encode("utf-8")) #type:ignore
 		long_description = pickle_x_loads(long_description)
 		setup(
 			name=name,
```

### Comparing `templated_setup-0.9902/templated_setup/_hardcoded.py` & `templated_setup-0.9903/templated_setup/_hardcoded.py`

 * *Files identical despite different names*

### Comparing `templated_setup-0.9902/templated_setup.egg-info/PKG-INFO` & `templated_setup-0.9903/templated_setup.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: templated_setup
-Version: 0.9902
+Version: 0.9903
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
 
-## V0.9902
+## V0.9903
 No notes.
```

