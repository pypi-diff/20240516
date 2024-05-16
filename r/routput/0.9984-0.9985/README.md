# Comparing `tmp/routput-0.9984.tar.gz` & `tmp/routput-0.9985.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "routput-0.9984.tar", last modified: Thu May 16 13:14:48 2024, max compression
+gzip compressed data, was "routput-0.9985.tar", last modified: Thu May 16 13:23:15 2024, max compression
```

## Comparing `routput-0.9984.tar` & `routput-0.9985.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-16 13:14:48.460852 routput-0.9984/
--rw-rw-rw-   0        0        0    25652 2024-04-18 08:26:04.000000 routput-0.9984/LICENCE
--rw-rw-rw-   0        0        0     2597 2024-05-16 13:14:48.460852 routput-0.9984/PKG-INFO
--rw-rw-rw-   0        0        0     2083 2024-04-18 09:01:17.000000 routput-0.9984/README.md
--rw-rw-rw-   0        0        0     2687 2024-05-16 13:14:48.000000 routput-0.9984/_README.py
--rw-rw-rw-   0        0        0     3509 2024-05-16 13:14:48.000000 routput-0.9984/_pickled.py
-drwxrwxrwx   0        0        0        0 2024-05-16 13:14:48.459727 routput-0.9984/routput.egg-info/
--rw-rw-rw-   0        0        0     2597 2024-05-16 13:14:48.000000 routput-0.9984/routput.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      192 2024-05-16 13:14:48.000000 routput-0.9984/routput.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-16 13:14:48.000000 routput-0.9984/routput.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       41 2024-05-16 13:14:48.000000 routput-0.9984/routput.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-16 13:14:48.462023 routput-0.9984/setup.cfg
--rw-rw-rw-   0        0        0      498 2024-05-16 12:45:46.000000 routput-0.9984/setup.py
--rw-rw-rw-   0        0        0    21122 2024-05-16 13:14:48.000000 routput-0.9984/templated_setup.py
+drwxrwxrwx   0        0        0        0 2024-05-16 13:23:15.694417 routput-0.9985/
+-rw-rw-rw-   0        0        0    25652 2024-04-18 08:26:04.000000 routput-0.9985/LICENCE
+-rw-rw-rw-   0        0        0     6443 2024-05-16 13:23:15.694417 routput-0.9985/PKG-INFO
+-rw-rw-rw-   0        0        0     2083 2024-04-18 09:01:17.000000 routput-0.9985/README.md
+-rw-rw-rw-   0        0        0     2687 2024-05-16 13:23:15.000000 routput-0.9985/_README.py
+-rw-rw-rw-   0        0        0     8505 2024-05-16 13:23:15.000000 routput-0.9985/_pickled.py
+drwxrwxrwx   0        0        0        0 2024-05-16 13:23:15.693400 routput-0.9985/routput.egg-info/
+-rw-rw-rw-   0        0        0     6443 2024-05-16 13:23:15.000000 routput-0.9985/routput.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      192 2024-05-16 13:23:15.000000 routput-0.9985/routput.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-16 13:23:15.000000 routput-0.9985/routput.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       41 2024-05-16 13:23:15.000000 routput-0.9985/routput.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-16 13:23:15.694417 routput-0.9985/setup.cfg
+-rw-rw-rw-   0        0        0      498 2024-05-16 12:45:46.000000 routput-0.9985/setup.py
+-rw-rw-rw-   0        0        0    21175 2024-05-16 13:23:15.000000 routput-0.9985/templated_setup.py
```

### Comparing `routput-0.9984/LICENCE` & `routput-0.9985/LICENCE`

 * *Files identical despite different names*

### Comparing `routput-0.9984/PKG-INFO` & `routput-0.9985/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,7 @@
-Metadata-Version: 2.1
-Name: routput
-Version: 0.9984
-Summary: recursively searches for files based on their extensions starting from a specified directory. It can print the directory structure, include or exclude specific files, use syntax highlighting for output, and anonymize file paths for privacy.
-Author: matrikater (Joel Watson)
-Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
-License-File: LICENCE
-
 # Recursive Output Utility
 
 ## Overview
 
 This Python script recursively searches for files based on their extensions starting from a specified directory. It can print the directory structure, include or exclude specific files, use syntax highlighting for output, and anonymize file paths for privacy.
 
 ## Requirements
@@ -85,10 +77,7 @@
 ```bash
 python routput.py -e [py] -b
 ```
 
 ## License
 
 Open-source software licensed under GPL-2 license.
-
-## V0.9984 released on 16th/5/2024
-hopefully `templated_setup` works now...
```

### Comparing `routput-0.9984/_README.py` & `routput-0.9985/_README.py`

 * *Files identical despite different names*

### Comparing `routput-0.9984/templated_setup.py` & `routput-0.9985/templated_setup.py`

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

