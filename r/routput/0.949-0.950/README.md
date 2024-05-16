# Comparing `tmp/routput-0.949.tar.gz` & `tmp/routput-0.950.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "routput-0.949.tar", last modified: Thu May 16 11:44:18 2024, max compression
+gzip compressed data, was "routput-0.950.tar", last modified: Thu May 16 11:52:49 2024, max compression
```

## Comparing `routput-0.949.tar` & `routput-0.950.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-05-16 11:44:18.599542 routput-0.949/
--rw-rw-rw-   0        0        0    25652 2024-04-18 08:26:04.000000 routput-0.949/LICENCE
--rw-rw-rw-   0        0        0     2593 2024-05-16 11:44:18.598529 routput-0.949/PKG-INFO
--rw-rw-rw-   0        0        0     2083 2024-04-18 09:01:17.000000 routput-0.949/README.md
-drwxrwxrwx   0        0        0        0 2024-05-16 11:44:18.597517 routput-0.949/routput.egg-info/
--rw-rw-rw-   0        0        0     2593 2024-05-16 11:44:18.000000 routput-0.949/routput.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      169 2024-05-16 11:44:18.000000 routput-0.949/routput.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-16 11:44:18.000000 routput-0.949/routput.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2024-05-16 11:44:18.000000 routput-0.949/routput.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-16 11:44:18.599542 routput-0.949/setup.cfg
--rw-rw-rw-   0        0        0      498 2024-05-16 11:38:04.000000 routput-0.949/setup.py
--rw-rw-rw-   0        0        0    19907 2024-05-16 11:44:18.000000 routput-0.949/templated_setup.py
+drwxrwxrwx   0        0        0        0 2024-05-16 11:52:49.887101 routput-0.950/
+-rw-rw-rw-   0        0        0    25652 2024-04-18 08:26:04.000000 routput-0.950/LICENCE
+-rw-rw-rw-   0        0        0     2593 2024-05-16 11:52:49.886056 routput-0.950/PKG-INFO
+-rw-rw-rw-   0        0        0     2083 2024-04-18 09:01:17.000000 routput-0.950/README.md
+drwxrwxrwx   0        0        0        0 2024-05-16 11:52:49.885039 routput-0.950/routput.egg-info/
+-rw-rw-rw-   0        0        0     2593 2024-05-16 11:52:49.000000 routput-0.950/routput.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      169 2024-05-16 11:52:49.000000 routput-0.950/routput.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-16 11:52:49.000000 routput-0.950/routput.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2024-05-16 11:52:49.000000 routput-0.950/routput.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-16 11:52:49.887101 routput-0.950/setup.cfg
+-rw-rw-rw-   0        0        0      498 2024-05-16 11:38:04.000000 routput-0.950/setup.py
+-rw-rw-rw-   0        0        0    19907 2024-05-16 11:52:49.000000 routput-0.950/templated_setup.py
```

### Comparing `routput-0.949/LICENCE` & `routput-0.950/LICENCE`

 * *Files identical despite different names*

### Comparing `routput-0.949/PKG-INFO` & `routput-0.950/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: routput
-Version: 0.949
+Version: 0.950
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
 
-## V0.949 released on 16th/5/2024
+## V0.950 released on 16th/5/2024
 `templated_setup` is giving me hell...
```

### Comparing `routput-0.949/README.md` & `routput-0.950/README.md`

 * *Files identical despite different names*

### Comparing `routput-0.949/routput.egg-info/PKG-INFO` & `routput-0.950/routput.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: routput
-Version: 0.949
+Version: 0.950
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
 
-## V0.949 released on 16th/5/2024
+## V0.950 released on 16th/5/2024
 `templated_setup` is giving me hell...
```

### Comparing `routput-0.949/templated_setup.py` & `routput-0.950/templated_setup.py`

 * *Files identical despite different names*

