# Comparing `tmp/templated_setup-0.989.tar.gz` & `tmp/templated_setup-0.9901.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "templated_setup-0.989.tar", last modified: Thu May 16 11:07:16 2024, max compression
+gzip compressed data, was "templated_setup-0.9901.tar", last modified: Thu May 16 11:14:00 2024, max compression
```

## Comparing `templated_setup-0.989.tar` & `templated_setup-0.9901.tar`

### file list

```diff
@@ -1,13 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-05-16 11:07:16.589519 templated_setup-0.989/
--rw-rw-rw-   0        0        0    25652 2024-03-14 11:21:06.000000 templated_setup-0.989/LICENCE
--rw-rw-rw-   0        0        0     2588 2024-05-16 11:07:16.588294 templated_setup-0.989/PKG-INFO
--rw-rw-rw-   0        0        0     2172 2024-04-29 06:54:31.000000 templated_setup-0.989/README.md
--rw-rw-rw-   0        0        0    21017 2024-05-16 11:07:16.000000 templated_setup-0.989/_templated_setup.py
--rw-rw-rw-   0        0        0       42 2024-05-16 11:07:16.589519 templated_setup-0.989/setup.cfg
--rw-rw-rw-   0        0        0      427 2024-05-16 10:55:07.000000 templated_setup-0.989/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-16 11:07:16.587266 templated_setup-0.989/templated_setup.egg-info/
--rw-rw-rw-   0        0        0     2588 2024-05-16 11:07:16.000000 templated_setup-0.989/templated_setup.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      240 2024-05-16 11:07:16.000000 templated_setup-0.989/templated_setup.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-16 11:07:16.000000 templated_setup-0.989/templated_setup.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2024-05-16 11:07:16.000000 templated_setup-0.989/templated_setup.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2024-05-16 11:07:16.000000 templated_setup-0.989/templated_setup.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-16 11:14:00.737527 templated_setup-0.9901/
+-rw-rw-rw-   0        0        0    25652 2024-03-14 11:21:06.000000 templated_setup-0.9901/LICENCE
+-rw-rw-rw-   0        0        0     2555 2024-05-16 11:14:00.737016 templated_setup-0.9901/PKG-INFO
+-rw-rw-rw-   0        0        0     2172 2024-04-29 06:54:31.000000 templated_setup-0.9901/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-16 11:14:00.738540 templated_setup-0.9901/setup.cfg
+-rw-rw-rw-   0        0        0     1300 2024-05-16 11:12:38.000000 templated_setup-0.9901/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-16 11:14:00.735309 templated_setup-0.9901/templated_setup.egg-info/
+-rw-rw-rw-   0        0        0     2555 2024-05-16 11:14:00.000000 templated_setup-0.9901/templated_setup.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      220 2024-05-16 11:14:00.000000 templated_setup-0.9901/templated_setup.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-16 11:14:00.000000 templated_setup-0.9901/templated_setup.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2024-05-16 11:14:00.000000 templated_setup-0.9901/templated_setup.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2024-05-16 11:14:00.000000 templated_setup-0.9901/templated_setup.egg-info/top_level.txt
```

### Comparing `templated_setup-0.989/LICENCE` & `templated_setup-0.9901/LICENCE`

 * *Files identical despite different names*

### Comparing `templated_setup-0.989/PKG-INFO` & `templated_setup-0.9901/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: templated-setup
-Version: 0.989
+Version: 0.9901
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
 
-## V0.989 released on 16th/5/2024
-this module is hell.
+## V0.9901
+No notes.
```

### Comparing `templated_setup-0.989/README.md` & `templated_setup-0.9901/README.md`

 * *Files identical despite different names*

### Comparing `templated_setup-0.989/templated_setup.egg-info/PKG-INFO` & `templated_setup-0.9901/templated_setup.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: templated-setup
-Version: 0.989
+Version: 0.9901
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
 
-## V0.989 released on 16th/5/2024
-this module is hell.
+## V0.9901
+No notes.
```

