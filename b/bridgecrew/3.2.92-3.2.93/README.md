# Comparing `tmp/bridgecrew-3.2.92.tar.gz` & `tmp/bridgecrew-3.2.93.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/bridgecrew-3.2.92.tar", last modified: Wed May 15 08:49:27 2024, max compression
+gzip compressed data, was "dist/bridgecrew-3.2.93.tar", last modified: Thu May 16 16:10:45 2024, max compression
```

## Comparing `bridgecrew-3.2.92.tar` & `bridgecrew-3.2.93.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 08:49:27.000000 bridgecrew-3.2.92/
--rw-r--r--   0 root         (0) root         (0)     1375 2024-05-15 08:49:27.000000 bridgecrew-3.2.92/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      505 2024-05-02 11:35:32.000000 bridgecrew-3.2.92/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 08:49:27.000000 bridgecrew-3.2.92/bin/
--rwxr-xr-x   0 root         (0) root         (0)       93 2024-05-02 11:35:32.000000 bridgecrew-3.2.92/bin/bridgecrew
--rw-r--r--   0 root         (0) root         (0)     1368 2024-05-02 11:35:32.000000 bridgecrew-3.2.92/bin/bridgecrew.cmd
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 08:49:27.000000 bridgecrew-3.2.92/bridgecrew/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-02 11:35:32.000000 bridgecrew-3.2.92/bridgecrew/__init__.py
--rw-r--r--   0 root         (0) root         (0)      481 2024-05-02 11:35:32.000000 bridgecrew-3.2.92/bridgecrew/banner.py
--rw-r--r--   0 root         (0) root         (0)      416 2024-05-02 11:35:32.000000 bridgecrew-3.2.92/bridgecrew/main.py
--rw-r--r--   0 root         (0) root         (0)       19 2024-05-15 08:49:23.000000 bridgecrew-3.2.92/bridgecrew/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 08:49:27.000000 bridgecrew-3.2.92/bridgecrew.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1375 2024-05-15 08:49:27.000000 bridgecrew-3.2.92/bridgecrew.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      306 2024-05-15 08:49:27.000000 bridgecrew-3.2.92/bridgecrew.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-15 08:49:27.000000 bridgecrew-3.2.92/bridgecrew.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       16 2024-05-15 08:49:27.000000 bridgecrew-3.2.92/bridgecrew.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2024-05-15 08:49:27.000000 bridgecrew-3.2.92/bridgecrew.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-15 08:49:27.000000 bridgecrew-3.2.92/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1773 2024-05-02 11:35:32.000000 bridgecrew-3.2.92/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 16:10:45.000000 bridgecrew-3.2.93/
+-rw-r--r--   0 root         (0) root         (0)     1375 2024-05-16 16:10:45.000000 bridgecrew-3.2.93/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      505 2024-01-22 12:20:37.000000 bridgecrew-3.2.93/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 16:10:45.000000 bridgecrew-3.2.93/bin/
+-rwxr-xr-x   0 root         (0) root         (0)       93 2024-01-22 12:20:37.000000 bridgecrew-3.2.93/bin/bridgecrew
+-rw-r--r--   0 root         (0) root         (0)     1368 2024-01-22 12:20:37.000000 bridgecrew-3.2.93/bin/bridgecrew.cmd
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 16:10:45.000000 bridgecrew-3.2.93/bridgecrew/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-01-22 12:20:37.000000 bridgecrew-3.2.93/bridgecrew/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      481 2024-01-22 12:20:37.000000 bridgecrew-3.2.93/bridgecrew/banner.py
+-rw-r--r--   0 root         (0) root         (0)      416 2024-01-22 12:20:37.000000 bridgecrew-3.2.93/bridgecrew/main.py
+-rw-r--r--   0 root         (0) root         (0)       19 2024-05-16 16:10:41.000000 bridgecrew-3.2.93/bridgecrew/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 16:10:45.000000 bridgecrew-3.2.93/bridgecrew.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1375 2024-05-16 16:10:45.000000 bridgecrew-3.2.93/bridgecrew.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      306 2024-05-16 16:10:45.000000 bridgecrew-3.2.93/bridgecrew.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-16 16:10:45.000000 bridgecrew-3.2.93/bridgecrew.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2024-05-16 16:10:45.000000 bridgecrew-3.2.93/bridgecrew.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2024-05-16 16:10:45.000000 bridgecrew-3.2.93/bridgecrew.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-16 16:10:45.000000 bridgecrew-3.2.93/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1773 2024-01-22 12:20:37.000000 bridgecrew-3.2.93/setup.py
```

### Comparing `bridgecrew-3.2.92/PKG-INFO` & `bridgecrew-3.2.93/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bridgecrew
-Version: 3.2.92
+Version: 3.2.93
 Summary: Infrastructure as code static analysis
 Home-page: https://github.com/bridgecrewio/bridgecrew
 Author: bridgecrew
 Author-email: meet@bridgecrew.io
 License: Apache License 2.0
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
```

### Comparing `bridgecrew-3.2.92/bin/bridgecrew.cmd` & `bridgecrew-3.2.93/bin/bridgecrew.cmd`

 * *Files identical despite different names*

### Comparing `bridgecrew-3.2.92/bridgecrew.egg-info/PKG-INFO` & `bridgecrew-3.2.93/bridgecrew.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bridgecrew
-Version: 3.2.92
+Version: 3.2.93
 Summary: Infrastructure as code static analysis
 Home-page: https://github.com/bridgecrewio/bridgecrew
 Author: bridgecrew
 Author-email: meet@bridgecrew.io
 License: Apache License 2.0
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
```

### Comparing `bridgecrew-3.2.92/setup.py` & `bridgecrew-3.2.93/setup.py`

 * *Files identical despite different names*

