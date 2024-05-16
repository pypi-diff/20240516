# Comparing `tmp/sopel_amputator-0.1.tar.gz` & `tmp/sopel_amputator-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sopel_amputator-0.1.tar", last modified: Fri Apr 12 18:16:07 2024, max compression
+gzip compressed data, was "sopel_amputator-0.2.0.tar", last modified: Sat Apr 13 18:48:43 2024, max compression
```

## Comparing `sopel_amputator-0.1.tar` & `sopel_amputator-0.2.0.tar`

### file list

```diff
@@ -1,18 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:16:07.817806 sopel_amputator-0.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-04-12 18:15:56.000000 sopel_amputator-0.1/COPYING
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-12 18:15:56.000000 sopel_amputator-0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-04-12 18:15:56.000000 sopel_amputator-0.1/NEWS
--rw-r--r--   0 runner    (1001) docker     (127)     1963 2024-04-12 18:16:07.817806 sopel_amputator-0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      880 2024-04-12 18:15:56.000000 sopel_amputator-0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      745 2024-04-12 18:16:07.817806 sopel_amputator-0.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)      692 2024-04-12 18:15:56.000000 sopel_amputator-0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:16:07.817806 sopel_amputator-0.1/sopel_amputator/
--rw-r--r--   0 runner    (1001) docker     (127)     2688 2024-04-12 18:15:56.000000 sopel_amputator-0.1/sopel_amputator/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:16:07.817806 sopel_amputator-0.1/sopel_amputator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1963 2024-04-12 18:16:07.000000 sopel_amputator-0.1/sopel_amputator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      355 2024-04-12 18:16:07.000000 sopel_amputator-0.1/sopel_amputator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 18:16:07.000000 sopel_amputator-0.1/sopel_amputator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-12 18:16:07.000000 sopel_amputator-0.1/sopel_amputator.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 18:16:07.000000 sopel_amputator-0.1/sopel_amputator.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-12 18:16:07.000000 sopel_amputator-0.1/sopel_amputator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-12 18:16:07.000000 sopel_amputator-0.1/sopel_amputator.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 18:48:43.178231 sopel_amputator-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-04-13 18:48:34.000000 sopel_amputator-0.2.0/COPYING
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-13 18:48:34.000000 sopel_amputator-0.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      713 2024-04-13 18:48:34.000000 sopel_amputator-0.2.0/NEWS
+-rw-r--r--   0 runner    (1001) docker     (127)     2396 2024-04-13 18:48:43.178231 sopel_amputator-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      880 2024-04-13 18:48:34.000000 sopel_amputator-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1225 2024-04-13 18:48:34.000000 sopel_amputator-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-13 18:48:43.178231 sopel_amputator-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 18:48:43.178231 sopel_amputator-0.2.0/sopel_amputator/
+-rw-r--r--   0 runner    (1001) docker     (127)     4311 2024-04-13 18:48:34.000000 sopel_amputator-0.2.0/sopel_amputator/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 18:48:43.178231 sopel_amputator-0.2.0/sopel_amputator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2396 2024-04-13 18:48:43.000000 sopel_amputator-0.2.0/sopel_amputator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-13 18:48:43.000000 sopel_amputator-0.2.0/sopel_amputator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 18:48:43.000000 sopel_amputator-0.2.0/sopel_amputator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-13 18:48:43.000000 sopel_amputator-0.2.0/sopel_amputator.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-13 18:48:43.000000 sopel_amputator-0.2.0/sopel_amputator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-13 18:48:43.000000 sopel_amputator-0.2.0/sopel_amputator.egg-info/top_level.txt
```

### Comparing `sopel_amputator-0.1/COPYING` & `sopel_amputator-0.2.0/COPYING`

 * *Files identical despite different names*

### Comparing `sopel_amputator-0.1/PKG-INFO` & `sopel_amputator-0.2.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 Metadata-Version: 2.1
 Name: sopel-amputator
-Version: 0.1.0
+Version: 0.2.0
 Summary: Sopel plugin that detects AMP links and finds their canonical forms using AmputatorBot
-Home-page: https://github.com/dgw/sopel-amputator
-Author: dgw
-Author-email: dgw@technobabbl.es
-License: Eiffel Forum License, version 2
+Author-email: dgw <dgw@technobabbl.es>
+License: EFL-2.0
+Project-URL: Homepage, https://github.com/dgw/sopel-amputator
+Project-URL: Bug Tracker, https://github.com/dgw/sopel-amputator/issues
+Keywords: sopel,plugin,bot,irc
+Platform: Linux x86, x86-64
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: Eiffel Forum License (EFL)
 Classifier: License :: OSI Approved :: Eiffel Forum License
 Classifier: Topic :: Communications :: Chat :: Internet Relay Chat
+Requires-Python: <4,>=3.8
 Description-Content-Type: text/markdown
 License-File: COPYING
-Requires-Dist: sopel<9,>=8.0.0.dev0
+Requires-Dist: sopel>=8.0.0.dev0
 
 # sopel-amputator
 
 Sopel plugin that detects AMP links and finds their canonical forms using
 [AmputatorBot](https://www.amputatorbot.com/)
 
 ## Installing
@@ -41,17 +44,27 @@
 This is a list of hostnames which `sopel-amputator` will ignore, even if they
 match one of the common AMP substrings it looks for. By default it contains a
 set of ignored domains from the AmputatorBot project.
 
 The default list is _overridden_ when setting this value, so make sure to also
 enter any of the default entries you want to keep.
 
-
 ## Changelog
 
+### 0.2.0
+
+Under-the-hood improvements:
+
+* More robust domain matching against ignore list
+  * Includes distinct log messages for exact matches vs. subdomain matches
+* More granular error handling
+* Better error logging
+* Migrated package metadata from `setup.py`+`setup.cfg` to `pyproject.toml`
+
+
 ### 0.1.0
 
 Initial release.
 
 Pending conversion from `setup.py`+`setup.cfg` template to newer style package
 using `pyproject.toml`—plus some other features on the todo list—but the basics
 are here:
```

### Comparing `sopel_amputator-0.1/README.md` & `sopel_amputator-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `sopel_amputator-0.1/sopel_amputator.egg-info/PKG-INFO` & `sopel_amputator-0.2.0/sopel_amputator.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 Metadata-Version: 2.1
 Name: sopel-amputator
-Version: 0.1.0
+Version: 0.2.0
 Summary: Sopel plugin that detects AMP links and finds their canonical forms using AmputatorBot
-Home-page: https://github.com/dgw/sopel-amputator
-Author: dgw
-Author-email: dgw@technobabbl.es
-License: Eiffel Forum License, version 2
+Author-email: dgw <dgw@technobabbl.es>
+License: EFL-2.0
+Project-URL: Homepage, https://github.com/dgw/sopel-amputator
+Project-URL: Bug Tracker, https://github.com/dgw/sopel-amputator/issues
+Keywords: sopel,plugin,bot,irc
+Platform: Linux x86, x86-64
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: Eiffel Forum License (EFL)
 Classifier: License :: OSI Approved :: Eiffel Forum License
 Classifier: Topic :: Communications :: Chat :: Internet Relay Chat
+Requires-Python: <4,>=3.8
 Description-Content-Type: text/markdown
 License-File: COPYING
-Requires-Dist: sopel<9,>=8.0.0.dev0
+Requires-Dist: sopel>=8.0.0.dev0
 
 # sopel-amputator
 
 Sopel plugin that detects AMP links and finds their canonical forms using
 [AmputatorBot](https://www.amputatorbot.com/)
 
 ## Installing
@@ -41,17 +44,27 @@
 This is a list of hostnames which `sopel-amputator` will ignore, even if they
 match one of the common AMP substrings it looks for. By default it contains a
 set of ignored domains from the AmputatorBot project.
 
 The default list is _overridden_ when setting this value, so make sure to also
 enter any of the default entries you want to keep.
 
-
 ## Changelog
 
+### 0.2.0
+
+Under-the-hood improvements:
+
+* More robust domain matching against ignore list
+  * Includes distinct log messages for exact matches vs. subdomain matches
+* More granular error handling
+* Better error logging
+* Migrated package metadata from `setup.py`+`setup.cfg` to `pyproject.toml`
+
+
 ### 0.1.0
 
 Initial release.
 
 Pending conversion from `setup.py`+`setup.cfg` template to newer style package
 using `pyproject.toml`—plus some other features on the todo list—but the basics
 are here:
```

