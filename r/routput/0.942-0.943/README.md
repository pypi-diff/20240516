# Comparing `tmp/routput-0.942.tar.gz` & `tmp/routput-0.943.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "routput-0.942.tar", last modified: Thu May 16 10:50:54 2024, max compression
+gzip compressed data, was "routput-0.943.tar", last modified: Thu May 16 11:18:13 2024, max compression
```

## Comparing `routput-0.942.tar` & `routput-0.943.tar`

### file list

```diff
@@ -1,15 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-05-16 10:50:54.591465 routput-0.942/
--rw-rw-rw-   0        0        0    25652 2024-04-18 08:26:04.000000 routput-0.942/LICENCE
--rw-rw-rw-   0        0        0     2593 2024-05-16 10:50:54.590458 routput-0.942/PKG-INFO
--rw-rw-rw-   0        0        0     2083 2024-04-18 09:01:17.000000 routput-0.942/README.md
-drwxrwxrwx   0        0        0        0 2024-05-16 10:50:54.585380 routput-0.942/routput/
--rw-rw-rw-   0        0        0       22 2024-05-16 10:24:13.000000 routput-0.942/routput/__init__.py
--rw-rw-rw-   0        0        0       31 2024-04-18 09:05:31.000000 routput-0.942/routput/__main__.py
--rw-rw-rw-   0        0        0     8179 2024-04-18 09:10:57.000000 routput-0.942/routput/routput.py
-drwxrwxrwx   0        0        0        0 2024-05-16 10:50:54.589449 routput-0.942/routput.egg-info/
--rw-rw-rw-   0        0        0     2593 2024-05-16 10:50:54.000000 routput-0.942/routput.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      209 2024-05-16 10:50:54.000000 routput-0.942/routput.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-16 10:50:54.000000 routput-0.942/routput.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-05-16 10:50:54.000000 routput-0.942/routput.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-16 10:50:54.591465 routput-0.942/setup.cfg
--rw-rw-rw-   0        0        0      498 2024-05-16 10:41:57.000000 routput-0.942/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-16 11:18:13.343025 routput-0.943/
+-rw-rw-rw-   0        0        0    25652 2024-04-18 08:26:04.000000 routput-0.943/LICENCE
+-rw-rw-rw-   0        0        0     2593 2024-05-16 11:18:13.341713 routput-0.943/PKG-INFO
+-rw-rw-rw-   0        0        0     2083 2024-04-18 09:01:17.000000 routput-0.943/README.md
+drwxrwxrwx   0        0        0        0 2024-05-16 11:18:13.340701 routput-0.943/routput.egg-info/
+-rw-rw-rw-   0        0        0     2593 2024-05-16 11:18:13.000000 routput-0.943/routput.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      169 2024-05-16 11:18:13.000000 routput-0.943/routput.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-16 11:18:13.000000 routput-0.943/routput.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2024-05-16 11:18:13.000000 routput-0.943/routput.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-16 11:18:13.343025 routput-0.943/setup.cfg
+-rw-rw-rw-   0        0        0      498 2024-05-16 11:17:34.000000 routput-0.943/setup.py
+-rw-rw-rw-   0        0        0    21014 2024-05-16 11:18:13.000000 routput-0.943/templated_setup.py
```

### Comparing `routput-0.942/LICENCE` & `routput-0.943/LICENCE`

 * *Files identical despite different names*

### Comparing `routput-0.942/PKG-INFO` & `routput-0.943/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: routput
-Version: 0.942
+Version: 0.943
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
 
-## V0.942 released on 16th/5/2024
+## V0.943 released on 16th/5/2024
 `templated_setup` is giving me hell...
```

### Comparing `routput-0.942/README.md` & `routput-0.943/README.md`

 * *Files identical despite different names*

### Comparing `routput-0.942/routput.egg-info/PKG-INFO` & `routput-0.943/routput.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: routput
-Version: 0.942
+Version: 0.943
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
 
-## V0.942 released on 16th/5/2024
+## V0.943 released on 16th/5/2024
 `templated_setup` is giving me hell...
```

