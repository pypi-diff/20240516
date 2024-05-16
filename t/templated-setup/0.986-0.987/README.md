# Comparing `tmp/templated_setup-0.986.tar.gz` & `tmp/templated_setup-0.987.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "templated_setup-0.986.tar", last modified: Thu May 16 10:55:25 2024, max compression
+gzip compressed data, was "templated_setup-0.987.tar", last modified: Thu May 16 11:02:04 2024, max compression
```

## Comparing `templated_setup-0.986.tar` & `templated_setup-0.987.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-05-16 10:55:25.908539 templated_setup-0.986/
--rw-rw-rw-   0        0        0    25652 2024-03-14 11:21:06.000000 templated_setup-0.986/LICENCE
--rw-rw-rw-   0        0        0     2588 2024-05-16 10:55:25.907033 templated_setup-0.986/PKG-INFO
--rw-rw-rw-   0        0        0     2172 2024-04-29 06:54:31.000000 templated_setup-0.986/README.md
--rw-rw-rw-   0        0        0       42 2024-05-16 10:55:25.908539 templated_setup-0.986/setup.cfg
--rw-rw-rw-   0        0        0      427 2024-05-16 10:55:07.000000 templated_setup-0.986/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-16 10:55:25.907033 templated_setup-0.986/templated_setup.egg-info/
--rw-rw-rw-   0        0        0     2588 2024-05-16 10:55:25.000000 templated_setup-0.986/templated_setup.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      239 2024-05-16 10:55:25.000000 templated_setup-0.986/templated_setup.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-16 10:55:25.000000 templated_setup-0.986/templated_setup.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2024-05-16 10:55:25.000000 templated_setup-0.986/templated_setup.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2024-05-16 10:55:25.000000 templated_setup-0.986/templated_setup.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    20709 2024-05-16 10:55:25.000000 templated_setup-0.986/templated_setup.py
+drwxrwxrwx   0        0        0        0 2024-05-16 11:02:04.454402 templated_setup-0.987/
+-rw-rw-rw-   0        0        0    25652 2024-03-14 11:21:06.000000 templated_setup-0.987/LICENCE
+-rw-rw-rw-   0        0        0     2588 2024-05-16 11:02:04.453379 templated_setup-0.987/PKG-INFO
+-rw-rw-rw-   0        0        0     2172 2024-04-29 06:54:31.000000 templated_setup-0.987/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-16 11:02:04.454402 templated_setup-0.987/setup.cfg
+-rw-rw-rw-   0        0        0      427 2024-05-16 10:55:07.000000 templated_setup-0.987/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-16 11:02:04.452362 templated_setup-0.987/templated_setup.egg-info/
+-rw-rw-rw-   0        0        0     2588 2024-05-16 11:02:04.000000 templated_setup-0.987/templated_setup.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      239 2024-05-16 11:02:04.000000 templated_setup-0.987/templated_setup.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-16 11:02:04.000000 templated_setup-0.987/templated_setup.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2024-05-16 11:02:04.000000 templated_setup-0.987/templated_setup.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2024-05-16 11:02:04.000000 templated_setup-0.987/templated_setup.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    20972 2024-05-16 11:02:04.000000 templated_setup-0.987/templated_setup.py
```

### Comparing `templated_setup-0.986/LICENCE` & `templated_setup-0.987/LICENCE`

 * *Files identical despite different names*

### Comparing `templated_setup-0.986/PKG-INFO` & `templated_setup-0.987/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: templated-setup
-Version: 0.986
+Version: 0.987
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
 
-## V0.986 released on 16th/5/2024
+## V0.987 released on 16th/5/2024
 this module is hell.
```

### Comparing `templated_setup-0.986/README.md` & `templated_setup-0.987/README.md`

 * *Files identical despite different names*

### Comparing `templated_setup-0.986/templated_setup.egg-info/PKG-INFO` & `templated_setup-0.987/templated_setup.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: templated-setup
-Version: 0.986
+Version: 0.987
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
 
-## V0.986 released on 16th/5/2024
+## V0.987 released on 16th/5/2024
 this module is hell.
```

### Comparing `templated_setup-0.986/templated_setup.py` & `templated_setup-0.987/templated_setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -665,15 +665,23 @@
 
 
 	@classmethod
 	def _handle_installation_via_pip(cls, name):
 
 		# NOTE: If we do not hardcode the version, then pip will throw a fit when trying to install the 
 		# NOTE:   `templated-setup` package.
-		from . import _hardcoded #type:ignore
+		try:
+			from . import _hardcoded #type:ignore
+		except ImportError:
+			with open("_hardcoded.py", "w") as f:
+				f.write("__version__ = \"0.0\"\n")
+				f.write("__author__ = \"\"\n")
+				f.write("__description__ = \"\"\n")
+				f.write("__long_description__ = \"\"\"\"\"\"\n")
+				f.write("__kwargs_for_setup_tools__ = \"\"\"\"\"\"\n")
 		kwargs_for_setup_tools = base64_x_b64decode(_hardcoded.__kwargs_for_setup_tools__.encode("utf-8")) #type:ignore
 		kwargs_for_setup_tools = pickle_x_loads(kwargs_for_setup_tools)
 		long_description = base64_x_b64decode(_hardcoded.__long_description__.encode("utf-8")) #type:ignore
 		long_description = pickle_x_loads(long_description)
 		setup(
 			name=name,
 			version=_hardcoded.__version__, #type:ignore
@@ -756,26 +764,25 @@
 
 		meta = None
 		with open(__file__, "r") as f:
 			meta = f.read()
 		with open("templated_setup.py", "w") as f:
 			f.write(meta)
 
-		#if not "ext_modules" in kwargs_for_setup_tools:
-		#	kwargs_for_setup_tools["ext_modules"] = []
-		#kwargs_for_setup_tools["ext_modules"].append("templated_setup")
+		if not "py_modules" in kwargs_for_setup_tools:
+			kwargs_for_setup_tools["py_modules"] = []
+		kwargs_for_setup_tools["py_modules"].append("templated_setup")
 
 		setup(
 			name=cls._name,
 			version=cls._version.version_number,
 			author=cls._author,
 			description=cls._description,
 			long_description_content_type="text/markdown; charset=UTF-8; variant=GFM",
 			long_description=long_description,
-			py_modules=["templated_setup"],
 			**kwargs_for_setup_tools,
 		)
 
 		os.remove("templated_setup.py")
 
 		print("\n] Setup complete.\n\n")
```

