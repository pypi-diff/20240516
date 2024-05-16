# Comparing `tmp/templated_setup-0.985.tar.gz` & `tmp/templated_setup-0.986.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "templated_setup-0.985.tar", last modified: Thu May 16 10:48:12 2024, max compression
+gzip compressed data, was "templated_setup-0.986.tar", last modified: Thu May 16 10:55:25 2024, max compression
```

## Comparing `templated_setup-0.985.tar` & `templated_setup-0.986.tar`

### file list

```diff
@@ -1,15 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-05-16 10:48:12.282345 templated_setup-0.985/
--rw-rw-rw-   0        0        0    25652 2024-03-14 11:21:06.000000 templated_setup-0.985/LICENCE
--rw-rw-rw-   0        0        0     2588 2024-05-16 10:48:12.281327 templated_setup-0.985/PKG-INFO
--rw-rw-rw-   0        0        0     2172 2024-04-29 06:54:31.000000 templated_setup-0.985/README.md
--rw-rw-rw-   0        0        0       42 2024-05-16 10:48:12.282345 templated_setup-0.985/setup.cfg
--rw-rw-rw-   0        0        0      427 2024-05-16 10:47:19.000000 templated_setup-0.985/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-16 10:48:12.274696 templated_setup-0.985/templated_setup/
--rw-rw-rw-   0        0        0    20503 2024-05-16 10:47:17.000000 templated_setup-0.985/templated_setup/__init__.py
--rw-rw-rw-   0        0        0     3271 2024-05-16 10:48:12.000000 templated_setup-0.985/templated_setup/_hardcoded.py
-drwxrwxrwx   0        0        0        0 2024-05-16 10:48:12.280307 templated_setup-0.985/templated_setup.egg-info/
--rw-rw-rw-   0        0        0     2588 2024-05-16 10:48:12.000000 templated_setup-0.985/templated_setup.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      278 2024-05-16 10:48:12.000000 templated_setup-0.985/templated_setup.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-16 10:48:12.000000 templated_setup-0.985/templated_setup.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2024-05-16 10:48:12.000000 templated_setup-0.985/templated_setup.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2024-05-16 10:48:12.000000 templated_setup-0.985/templated_setup.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-16 10:55:25.908539 templated_setup-0.986/
+-rw-rw-rw-   0        0        0    25652 2024-03-14 11:21:06.000000 templated_setup-0.986/LICENCE
+-rw-rw-rw-   0        0        0     2588 2024-05-16 10:55:25.907033 templated_setup-0.986/PKG-INFO
+-rw-rw-rw-   0        0        0     2172 2024-04-29 06:54:31.000000 templated_setup-0.986/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-16 10:55:25.908539 templated_setup-0.986/setup.cfg
+-rw-rw-rw-   0        0        0      427 2024-05-16 10:55:07.000000 templated_setup-0.986/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-16 10:55:25.907033 templated_setup-0.986/templated_setup.egg-info/
+-rw-rw-rw-   0        0        0     2588 2024-05-16 10:55:25.000000 templated_setup-0.986/templated_setup.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      239 2024-05-16 10:55:25.000000 templated_setup-0.986/templated_setup.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-16 10:55:25.000000 templated_setup-0.986/templated_setup.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2024-05-16 10:55:25.000000 templated_setup-0.986/templated_setup.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2024-05-16 10:55:25.000000 templated_setup-0.986/templated_setup.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    20709 2024-05-16 10:55:25.000000 templated_setup-0.986/templated_setup.py
```

### Comparing `templated_setup-0.985/LICENCE` & `templated_setup-0.986/LICENCE`

 * *Files identical despite different names*

### Comparing `templated_setup-0.985/PKG-INFO` & `templated_setup-0.986/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: templated-setup
-Version: 0.985
+Version: 0.986
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
 
-## V0.985 released on 16th/5/2024
+## V0.986 released on 16th/5/2024
 this module is hell.
```

### Comparing `templated_setup-0.985/README.md` & `templated_setup-0.986/README.md`

 * *Files identical despite different names*

### Comparing `templated_setup-0.985/templated_setup/__init__.py` & `templated_setup-0.986/templated_setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -756,21 +756,26 @@
 
 		meta = None
 		with open(__file__, "r") as f:
 			meta = f.read()
 		with open("templated_setup.py", "w") as f:
 			f.write(meta)
 
+		#if not "ext_modules" in kwargs_for_setup_tools:
+		#	kwargs_for_setup_tools["ext_modules"] = []
+		#kwargs_for_setup_tools["ext_modules"].append("templated_setup")
+
 		setup(
 			name=cls._name,
 			version=cls._version.version_number,
 			author=cls._author,
 			description=cls._description,
 			long_description_content_type="text/markdown; charset=UTF-8; variant=GFM",
 			long_description=long_description,
+			py_modules=["templated_setup"],
 			**kwargs_for_setup_tools,
 		)
 
 		os.remove("templated_setup.py")
 
 		print("\n] Setup complete.\n\n")
```

### Comparing `templated_setup-0.985/templated_setup.egg-info/PKG-INFO` & `templated_setup-0.986/templated_setup.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: templated-setup
-Version: 0.985
+Version: 0.986
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
 
-## V0.985 released on 16th/5/2024
+## V0.986 released on 16th/5/2024
 this module is hell.
```

