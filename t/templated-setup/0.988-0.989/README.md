# Comparing `tmp/templated_setup-0.988.tar.gz` & `tmp/templated_setup-0.989.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "templated_setup-0.988.tar", last modified: Thu May 16 11:03:38 2024, max compression
+gzip compressed data, was "templated_setup-0.989.tar", last modified: Thu May 16 11:07:16 2024, max compression
```

## Comparing `templated_setup-0.988.tar` & `templated_setup-0.989.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-05-16 11:03:38.046132 templated_setup-0.988/
--rw-rw-rw-   0        0        0    25652 2024-03-14 11:21:06.000000 templated_setup-0.988/LICENCE
--rw-rw-rw-   0        0        0     2588 2024-05-16 11:03:38.045605 templated_setup-0.988/PKG-INFO
--rw-rw-rw-   0        0        0     2172 2024-04-29 06:54:31.000000 templated_setup-0.988/README.md
--rw-rw-rw-   0        0        0       42 2024-05-16 11:03:38.046648 templated_setup-0.988/setup.cfg
--rw-rw-rw-   0        0        0      427 2024-05-16 10:55:07.000000 templated_setup-0.988/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-16 11:03:38.044583 templated_setup-0.988/templated_setup.egg-info/
--rw-rw-rw-   0        0        0     2588 2024-05-16 11:03:37.000000 templated_setup-0.988/templated_setup.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      239 2024-05-16 11:03:38.000000 templated_setup-0.988/templated_setup.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-16 11:03:37.000000 templated_setup-0.988/templated_setup.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2024-05-16 11:03:37.000000 templated_setup-0.988/templated_setup.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2024-05-16 11:03:37.000000 templated_setup-0.988/templated_setup.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    21014 2024-05-16 11:03:37.000000 templated_setup-0.988/templated_setup.py
+drwxrwxrwx   0        0        0        0 2024-05-16 11:07:16.589519 templated_setup-0.989/
+-rw-rw-rw-   0        0        0    25652 2024-03-14 11:21:06.000000 templated_setup-0.989/LICENCE
+-rw-rw-rw-   0        0        0     2588 2024-05-16 11:07:16.588294 templated_setup-0.989/PKG-INFO
+-rw-rw-rw-   0        0        0     2172 2024-04-29 06:54:31.000000 templated_setup-0.989/README.md
+-rw-rw-rw-   0        0        0    21017 2024-05-16 11:07:16.000000 templated_setup-0.989/_templated_setup.py
+-rw-rw-rw-   0        0        0       42 2024-05-16 11:07:16.589519 templated_setup-0.989/setup.cfg
+-rw-rw-rw-   0        0        0      427 2024-05-16 10:55:07.000000 templated_setup-0.989/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-16 11:07:16.587266 templated_setup-0.989/templated_setup.egg-info/
+-rw-rw-rw-   0        0        0     2588 2024-05-16 11:07:16.000000 templated_setup-0.989/templated_setup.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      240 2024-05-16 11:07:16.000000 templated_setup-0.989/templated_setup.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-16 11:07:16.000000 templated_setup-0.989/templated_setup.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2024-05-16 11:07:16.000000 templated_setup-0.989/templated_setup.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2024-05-16 11:07:16.000000 templated_setup-0.989/templated_setup.egg-info/top_level.txt
```

### Comparing `templated_setup-0.988/LICENCE` & `templated_setup-0.989/LICENCE`

 * *Files identical despite different names*

### Comparing `templated_setup-0.988/PKG-INFO` & `templated_setup-0.989/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: templated-setup
-Version: 0.988
+Version: 0.989
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
 
-## V0.988 released on 16th/5/2024
+## V0.989 released on 16th/5/2024
 this module is hell.
```

### Comparing `templated_setup-0.988/README.md` & `templated_setup-0.989/README.md`

 * *Files identical despite different names*

### Comparing `templated_setup-0.988/templated_setup.egg-info/PKG-INFO` & `templated_setup-0.989/templated_setup.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: templated-setup
-Version: 0.988
+Version: 0.989
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
 
-## V0.988 released on 16th/5/2024
+## V0.989 released on 16th/5/2024
 this module is hell.
```

### Comparing `templated_setup-0.988/templated_setup.py` & `templated_setup-0.989/_templated_setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -762,32 +762,32 @@
 			f.write(f"__description__ = \"{cls._description}\"\n")
 			f.write(f"__long_description__ = \"\"\"{s_long_description}\"\"\"\n")
 			f.write(f"__kwargs_for_setup_tools__ = \"\"\"{s_kwargs_for_setup_tools}\"\"\"\n")
 
 		meta = None
 		with open(__file__, "r") as f:
 			meta = f.read()
-		with open("templated_setup.py", "w") as f:
+		with open("_templated_setup.py", "w") as f:
 			f.write(meta)
 
 		if not "py_modules" in kwargs_for_setup_tools:
 			kwargs_for_setup_tools["py_modules"] = []
-		kwargs_for_setup_tools["py_modules"].append("templated_setup")
+		kwargs_for_setup_tools["py_modules"].append("_templated_setup")
 
 		setup(
 			name=cls._name,
 			version=cls._version.version_number,
 			author=cls._author,
 			description=cls._description,
 			long_description_content_type="text/markdown; charset=UTF-8; variant=GFM",
 			long_description=long_description,
 			**kwargs_for_setup_tools,
 		)
 
-		os.remove("templated_setup.py")
+		os.remove("_templated_setup.py")
 
 		print("\n] Setup complete.\n\n")
 
 		do_publish = _Setup_Helper.__get_y_n("Would you like to publish to PyPi?")
 		if not do_publish:
 			exit(0)
```

