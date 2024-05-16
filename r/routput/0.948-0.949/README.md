# Comparing `tmp/routput-0.948.tar.gz` & `tmp/routput-0.949.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "routput-0.948.tar", last modified: Thu May 16 11:37:08 2024, max compression
+gzip compressed data, was "routput-0.949.tar", last modified: Thu May 16 11:44:18 2024, max compression
```

## Comparing `routput-0.948.tar` & `routput-0.949.tar`

### file list

```diff
@@ -1,13 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-05-16 11:37:08.016534 routput-0.948/
--rw-rw-rw-   0        0        0    25652 2024-04-18 08:26:04.000000 routput-0.948/LICENCE
--rw-rw-rw-   0        0        0     2593 2024-05-16 11:37:08.016534 routput-0.948/PKG-INFO
--rw-rw-rw-   0        0        0     2083 2024-04-18 09:01:17.000000 routput-0.948/README.md
--rw-rw-rw-   0        0        0        0 2024-05-16 11:32:28.000000 routput-0.948/_hardcoded.py
-drwxrwxrwx   0        0        0        0 2024-05-16 11:37:08.015513 routput-0.948/routput.egg-info/
--rw-rw-rw-   0        0        0     2593 2024-05-16 11:37:07.000000 routput-0.948/routput.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      183 2024-05-16 11:37:07.000000 routput-0.948/routput.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-16 11:37:07.000000 routput-0.948/routput.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       27 2024-05-16 11:37:07.000000 routput-0.948/routput.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-16 11:37:08.017554 routput-0.948/setup.cfg
--rw-rw-rw-   0        0        0      517 2024-05-16 11:32:37.000000 routput-0.948/setup.py
--rw-rw-rw-   0        0        0    20728 2024-05-16 11:37:07.000000 routput-0.948/templated_setup.py
+drwxrwxrwx   0        0        0        0 2024-05-16 11:44:18.599542 routput-0.949/
+-rw-rw-rw-   0        0        0    25652 2024-04-18 08:26:04.000000 routput-0.949/LICENCE
+-rw-rw-rw-   0        0        0     2593 2024-05-16 11:44:18.598529 routput-0.949/PKG-INFO
+-rw-rw-rw-   0        0        0     2083 2024-04-18 09:01:17.000000 routput-0.949/README.md
+drwxrwxrwx   0        0        0        0 2024-05-16 11:44:18.597517 routput-0.949/routput.egg-info/
+-rw-rw-rw-   0        0        0     2593 2024-05-16 11:44:18.000000 routput-0.949/routput.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      169 2024-05-16 11:44:18.000000 routput-0.949/routput.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-16 11:44:18.000000 routput-0.949/routput.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2024-05-16 11:44:18.000000 routput-0.949/routput.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-16 11:44:18.599542 routput-0.949/setup.cfg
+-rw-rw-rw-   0        0        0      498 2024-05-16 11:38:04.000000 routput-0.949/setup.py
+-rw-rw-rw-   0        0        0    19907 2024-05-16 11:44:18.000000 routput-0.949/templated_setup.py
```

### Comparing `routput-0.948/LICENCE` & `routput-0.949/LICENCE`

 * *Files identical despite different names*

### Comparing `routput-0.948/PKG-INFO` & `routput-0.949/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: routput
-Version: 0.948
+Version: 0.949
 Summary: recursively searches for files based on their extensions starting from a specified directory. It can print the directory structure, include or exclude specific files, use syntax highlighting for output, and anonymize file paths for privacy.
 Author: matrikater (Joel Watson)
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 License-File: LICENCE
 
 # Recursive Output Utility
 
@@ -86,9 +86,9 @@
 python routput.py -e [py] -b
 ```
 
 ## License
 
 Open-source software licensed under GPL-2 license.
 
-## V0.948 released on 16th/5/2024
+## V0.949 released on 16th/5/2024
 `templated_setup` is giving me hell...
```

### Comparing `routput-0.948/README.md` & `routput-0.949/README.md`

 * *Files identical despite different names*

### Comparing `routput-0.948/routput.egg-info/PKG-INFO` & `routput-0.949/routput.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: routput
-Version: 0.948
+Version: 0.949
 Summary: recursively searches for files based on their extensions starting from a specified directory. It can print the directory structure, include or exclude specific files, use syntax highlighting for output, and anonymize file paths for privacy.
 Author: matrikater (Joel Watson)
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 License-File: LICENCE
 
 # Recursive Output Utility
 
@@ -86,9 +86,9 @@
 python routput.py -e [py] -b
 ```
 
 ## License
 
 Open-source software licensed under GPL-2 license.
 
-## V0.948 released on 16th/5/2024
+## V0.949 released on 16th/5/2024
 `templated_setup` is giving me hell...
```

### Comparing `routput-0.948/templated_setup.py` & `routput-0.949/templated_setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -738,36 +738,23 @@
 		cls._old_sys_argv = sys.argv
 		sys.argv = [sys.argv[0], "sdist"]
 		do_proceed = _Setup_Helper.__get_y_n("Would you like to proceed with the build?")
 		if not do_proceed:
 			exit(0)
 		_Setup_Helper.__clear_screen()
 
-		from . import _hardcoded # No `type:ignore` here since this file should exists.
-		s_long_description = pickle_x_dumps(long_description)
-		s_long_description = base64_x_b64encode(s_long_description).decode("utf-8")
-		s_kwargs_for_setup_tools = pickle_x_dumps(kwargs_for_setup_tools)
-		s_kwargs_for_setup_tools = base64_x_b64encode(s_kwargs_for_setup_tools).decode("utf-8")
-		with open(_hardcoded.__file__, "w") as f:
-			f.write(f"__version__ = \"{cls._version.version_number}\"\n")
-			f.write(f"__author__ = \"{cls._author}\"\n")
-			f.write(f"__description__ = \"{cls._description}\"\n")
-			f.write(f"__long_description__ = \"\"\"{s_long_description}\"\"\"\n")
-			f.write(f"__kwargs_for_setup_tools__ = \"\"\"{s_kwargs_for_setup_tools}\"\"\"\n")
-
 		meta = None
 		with open(__file__, "r") as f:
 			meta = f.read()
 		with open("templated_setup.py", "w") as f:
 			f.write(meta)
 
 		if not "py_modules" in kwargs_for_setup_tools:
 			kwargs_for_setup_tools["py_modules"] = []
 		kwargs_for_setup_tools["py_modules"].append("templated_setup")
-		kwargs_for_setup_tools["py_modules"].append("_hardcoded")
 
 		setup(
 			name=cls._name,
 			version=cls._version.version_number,
 			author=cls._author,
 			description=cls._description,
 			long_description_content_type="text/markdown; charset=UTF-8; variant=GFM",
```

