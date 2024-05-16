# Comparing `tmp/routput-0.94.tar.gz` & `tmp/routput-0.941.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "routput-0.94.tar", last modified: Thu May 16 10:26:07 2024, max compression
+gzip compressed data, was "routput-0.941.tar", last modified: Thu May 16 10:43:05 2024, max compression
```

## Comparing `routput-0.94.tar` & `routput-0.941.tar`

### file list

```diff
@@ -1,16 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-16 10:26:07.240076 routput-0.94/
--rw-rw-rw-   0        0        0    25652 2024-04-18 08:26:04.000000 routput-0.94/LICENCE
--rw-rw-rw-   0        0        0     2623 2024-05-16 10:26:07.239037 routput-0.94/PKG-INFO
--rw-rw-rw-   0        0        0     2083 2024-04-18 09:01:17.000000 routput-0.94/README.md
-drwxrwxrwx   0        0        0        0 2024-05-16 10:26:07.232678 routput-0.94/routput/
--rw-rw-rw-   0        0        0       22 2024-05-16 10:24:13.000000 routput-0.94/routput/__init__.py
--rw-rw-rw-   0        0        0       31 2024-04-18 09:05:31.000000 routput-0.94/routput/__main__.py
--rw-rw-rw-   0        0        0     8179 2024-04-18 09:10:57.000000 routput-0.94/routput/routput.py
-drwxrwxrwx   0        0        0        0 2024-05-16 10:26:07.239037 routput-0.94/routput.egg-info/
--rw-rw-rw-   0        0        0     2623 2024-05-16 10:26:07.000000 routput-0.94/routput.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      239 2024-05-16 10:26:07.000000 routput-0.94/routput.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-16 10:26:07.000000 routput-0.94/routput.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2024-05-16 10:26:07.000000 routput-0.94/routput.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-05-16 10:26:07.000000 routput-0.94/routput.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-16 10:26:07.240076 routput-0.94/setup.cfg
--rw-rw-rw-   0        0        0      539 2024-05-16 10:24:43.000000 routput-0.94/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-16 10:43:05.516806 routput-0.941/
+-rw-rw-rw-   0        0        0    25652 2024-04-18 08:26:04.000000 routput-0.941/LICENCE
+-rw-rw-rw-   0        0        0     2593 2024-05-16 10:43:05.515770 routput-0.941/PKG-INFO
+-rw-rw-rw-   0        0        0     2083 2024-04-18 09:01:17.000000 routput-0.941/README.md
+drwxrwxrwx   0        0        0        0 2024-05-16 10:43:05.509330 routput-0.941/routput/
+-rw-rw-rw-   0        0        0       22 2024-05-16 10:24:13.000000 routput-0.941/routput/__init__.py
+-rw-rw-rw-   0        0        0       31 2024-04-18 09:05:31.000000 routput-0.941/routput/__main__.py
+-rw-rw-rw-   0        0        0     8179 2024-04-18 09:10:57.000000 routput-0.941/routput/routput.py
+drwxrwxrwx   0        0        0        0 2024-05-16 10:43:05.514752 routput-0.941/routput.egg-info/
+-rw-rw-rw-   0        0        0     2593 2024-05-16 10:43:05.000000 routput-0.941/routput.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      209 2024-05-16 10:43:05.000000 routput-0.941/routput.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-16 10:43:05.000000 routput-0.941/routput.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-05-16 10:43:05.000000 routput-0.941/routput.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-16 10:43:05.516806 routput-0.941/setup.cfg
+-rw-rw-rw-   0        0        0      498 2024-05-16 10:41:57.000000 routput-0.941/setup.py
```

### Comparing `routput-0.94/LICENCE` & `routput-0.941/LICENCE`

 * *Files identical despite different names*

### Comparing `routput-0.94/PKG-INFO` & `routput-0.941/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 Metadata-Version: 2.1
 Name: routput
-Version: 0.94
+Version: 0.941
 Summary: recursively searches for files based on their extensions starting from a specified directory. It can print the directory structure, include or exclude specific files, use syntax highlighting for output, and anonymize file paths for privacy.
 Author: matrikater (Joel Watson)
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 License-File: LICENCE
-Requires-Dist: templated-setup
 
 # Recursive Output Utility
 
 ## Overview
 
 This Python script recursively searches for files based on their extensions starting from a specified directory. It can print the directory structure, include or exclude specific files, use syntax highlighting for output, and anonymize file paths for privacy.
 
@@ -87,9 +86,9 @@
 python routput.py -e [py] -b
 ```
 
 ## License
 
 Open-source software licensed under GPL-2 license.
 
-## V0.94 released on 16th/5/2024
+## V0.941 released on 16th/5/2024
 `templated_setup` is giving me hell...
```

### Comparing `routput-0.94/README.md` & `routput-0.941/README.md`

 * *Files identical despite different names*

### Comparing `routput-0.94/routput/routput.py` & `routput-0.941/routput/routput.py`

 * *Files identical despite different names*

### Comparing `routput-0.94/routput.egg-info/PKG-INFO` & `routput-0.941/routput.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 Metadata-Version: 2.1
 Name: routput
-Version: 0.94
+Version: 0.941
 Summary: recursively searches for files based on their extensions starting from a specified directory. It can print the directory structure, include or exclude specific files, use syntax highlighting for output, and anonymize file paths for privacy.
 Author: matrikater (Joel Watson)
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 License-File: LICENCE
-Requires-Dist: templated-setup
 
 # Recursive Output Utility
 
 ## Overview
 
 This Python script recursively searches for files based on their extensions starting from a specified directory. It can print the directory structure, include or exclude specific files, use syntax highlighting for output, and anonymize file paths for privacy.
 
@@ -87,9 +86,9 @@
 python routput.py -e [py] -b
 ```
 
 ## License
 
 Open-source software licensed under GPL-2 license.
 
-## V0.94 released on 16th/5/2024
+## V0.941 released on 16th/5/2024
 `templated_setup` is giving me hell...
```

