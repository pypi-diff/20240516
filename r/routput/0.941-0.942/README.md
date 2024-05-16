# Comparing `tmp/routput-0.941.tar.gz` & `tmp/routput-0.942.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "routput-0.941.tar", last modified: Thu May 16 10:43:05 2024, max compression
+gzip compressed data, was "routput-0.942.tar", last modified: Thu May 16 10:50:54 2024, max compression
```

## Comparing `routput-0.941.tar` & `routput-0.942.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-16 10:43:05.516806 routput-0.941/
--rw-rw-rw-   0        0        0    25652 2024-04-18 08:26:04.000000 routput-0.941/LICENCE
--rw-rw-rw-   0        0        0     2593 2024-05-16 10:43:05.515770 routput-0.941/PKG-INFO
--rw-rw-rw-   0        0        0     2083 2024-04-18 09:01:17.000000 routput-0.941/README.md
-drwxrwxrwx   0        0        0        0 2024-05-16 10:43:05.509330 routput-0.941/routput/
--rw-rw-rw-   0        0        0       22 2024-05-16 10:24:13.000000 routput-0.941/routput/__init__.py
--rw-rw-rw-   0        0        0       31 2024-04-18 09:05:31.000000 routput-0.941/routput/__main__.py
--rw-rw-rw-   0        0        0     8179 2024-04-18 09:10:57.000000 routput-0.941/routput/routput.py
-drwxrwxrwx   0        0        0        0 2024-05-16 10:43:05.514752 routput-0.941/routput.egg-info/
--rw-rw-rw-   0        0        0     2593 2024-05-16 10:43:05.000000 routput-0.941/routput.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      209 2024-05-16 10:43:05.000000 routput-0.941/routput.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-16 10:43:05.000000 routput-0.941/routput.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-05-16 10:43:05.000000 routput-0.941/routput.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-16 10:43:05.516806 routput-0.941/setup.cfg
--rw-rw-rw-   0        0        0      498 2024-05-16 10:41:57.000000 routput-0.941/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-16 10:50:54.591465 routput-0.942/
+-rw-rw-rw-   0        0        0    25652 2024-04-18 08:26:04.000000 routput-0.942/LICENCE
+-rw-rw-rw-   0        0        0     2593 2024-05-16 10:50:54.590458 routput-0.942/PKG-INFO
+-rw-rw-rw-   0        0        0     2083 2024-04-18 09:01:17.000000 routput-0.942/README.md
+drwxrwxrwx   0        0        0        0 2024-05-16 10:50:54.585380 routput-0.942/routput/
+-rw-rw-rw-   0        0        0       22 2024-05-16 10:24:13.000000 routput-0.942/routput/__init__.py
+-rw-rw-rw-   0        0        0       31 2024-04-18 09:05:31.000000 routput-0.942/routput/__main__.py
+-rw-rw-rw-   0        0        0     8179 2024-04-18 09:10:57.000000 routput-0.942/routput/routput.py
+drwxrwxrwx   0        0        0        0 2024-05-16 10:50:54.589449 routput-0.942/routput.egg-info/
+-rw-rw-rw-   0        0        0     2593 2024-05-16 10:50:54.000000 routput-0.942/routput.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      209 2024-05-16 10:50:54.000000 routput-0.942/routput.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-16 10:50:54.000000 routput-0.942/routput.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-05-16 10:50:54.000000 routput-0.942/routput.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-16 10:50:54.591465 routput-0.942/setup.cfg
+-rw-rw-rw-   0        0        0      498 2024-05-16 10:41:57.000000 routput-0.942/setup.py
```

### Comparing `routput-0.941/LICENCE` & `routput-0.942/LICENCE`

 * *Files identical despite different names*

### Comparing `routput-0.941/PKG-INFO` & `routput-0.942/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: routput
-Version: 0.941
+Version: 0.942
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
 
-## V0.941 released on 16th/5/2024
+## V0.942 released on 16th/5/2024
 `templated_setup` is giving me hell...
```

### Comparing `routput-0.941/README.md` & `routput-0.942/README.md`

 * *Files identical despite different names*

### Comparing `routput-0.941/routput/routput.py` & `routput-0.942/routput/routput.py`

 * *Files identical despite different names*

### Comparing `routput-0.941/routput.egg-info/PKG-INFO` & `routput-0.942/routput.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: routput
-Version: 0.941
+Version: 0.942
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
 
-## V0.941 released on 16th/5/2024
+## V0.942 released on 16th/5/2024
 `templated_setup` is giving me hell...
```

