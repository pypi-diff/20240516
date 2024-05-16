# Comparing `tmp/plsp-0.2.tar.gz` & `tmp/plsp-0.21.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plsp-0.2.tar", last modified: Thu May 16 09:52:27 2024, max compression
+gzip compressed data, was "plsp-0.21.tar", last modified: Thu May 16 13:01:51 2024, max compression
```

## Comparing `plsp-0.2.tar` & `plsp-0.21.tar`

### file list

```diff
@@ -1,27 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-05-16 09:52:27.586383 plsp-0.2/
--rw-rw-rw-   0        0        0     6318 2024-05-16 09:52:27.585356 plsp-0.2/PKG-INFO
--rw-rw-rw-   0        0        0     5929 2024-05-16 09:31:25.000000 plsp-0.2/README.md
-drwxrwxrwx   0        0        0        0 2024-05-16 09:52:27.572222 plsp-0.2/plsp/
--rw-rw-rw-   0        0        0     4630 2024-05-16 09:31:25.000000 plsp-0.2/plsp/DebugContext.py
--rw-rw-rw-   0        0        0      964 2024-05-16 09:31:25.000000 plsp-0.2/plsp/DebugMode.py
--rw-rw-rw-   0        0        0      267 2024-05-16 09:31:25.000000 plsp-0.2/plsp/Direction.py
--rw-rw-rw-   0        0        0     9084 2024-05-16 09:31:25.000000 plsp-0.2/plsp/Logger.py
--rw-rw-rw-   0        0        0     2102 2024-05-16 09:31:25.000000 plsp-0.2/plsp/SharedLogger.py
--rw-rw-rw-   0        0        0     2516 2024-05-16 09:31:25.000000 plsp-0.2/plsp/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-16 09:52:27.581320 plsp-0.2/plsp/formatters/
--rw-rw-rw-   0        0        0     1114 2024-05-16 09:31:25.000000 plsp-0.2/plsp/formatters/FinalFormatter.py
--rw-rw-rw-   0        0        0     1445 2024-05-16 09:31:25.000000 plsp-0.2/plsp/formatters/Formatter.py
--rw-rw-rw-   0        0        0      103 2024-05-16 09:31:25.000000 plsp-0.2/plsp/formatters/__init__.py
--rw-rw-rw-   0        0        0     1224 2024-05-16 09:31:25.000000 plsp-0.2/plsp/formatters/bundled.py
--rw-rw-rw-   0        0        0      243 2024-05-16 09:31:25.000000 plsp-0.2/plsp/formatters/defaults.py
-drwxrwxrwx   0        0        0        0 2024-05-16 09:52:27.583341 plsp-0.2/plsp/infoinject/
--rw-rw-rw-   0        0        0    10840 2024-05-16 09:31:25.000000 plsp-0.2/plsp/infoinject/InfoInjector.py
--rw-rw-rw-   0        0        0       38 2024-05-16 09:31:25.000000 plsp-0.2/plsp/infoinject/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-16 09:52:27.584352 plsp-0.2/plsp.egg-info/
--rw-rw-rw-   0        0        0     6318 2024-05-16 09:52:27.000000 plsp-0.2/plsp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      473 2024-05-16 09:52:27.000000 plsp-0.2/plsp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-16 09:52:27.000000 plsp-0.2/plsp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2024-05-16 09:52:27.000000 plsp-0.2/plsp.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2024-05-16 09:52:27.000000 plsp-0.2/plsp.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-16 09:52:27.586383 plsp-0.2/setup.cfg
--rw-rw-rw-   0        0        0      314 2024-05-16 09:50:49.000000 plsp-0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-16 13:01:51.715724 plsp-0.21/
+-rw-rw-rw-   0        0        0     2442 2024-05-16 13:01:51.714653 plsp-0.21/PKG-INFO
+-rw-rw-rw-   0        0        0     5929 2024-05-16 09:31:25.000000 plsp-0.21/README.md
+-rw-rw-rw-   0        0        0     7683 2024-05-16 13:01:51.000000 plsp-0.21/README.py
+-rw-rw-rw-   0        0        0     3401 2024-05-16 13:01:51.000000 plsp-0.21/pickled.py
+drwxrwxrwx   0        0        0        0 2024-05-16 13:01:51.714144 plsp-0.21/plsp.egg-info/
+-rw-rw-rw-   0        0        0     2442 2024-05-16 13:01:51.000000 plsp-0.21/plsp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      170 2024-05-16 13:01:51.000000 plsp-0.21/plsp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-16 13:01:51.000000 plsp-0.21/plsp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       31 2024-05-16 13:01:51.000000 plsp-0.21/plsp.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-16 13:01:51.715724 plsp-0.21/setup.cfg
+-rw-rw-rw-   0        0        0      287 2024-05-16 13:01:06.000000 plsp-0.21/setup.py
+-rw-rw-rw-   0        0        0    21056 2024-05-16 13:01:51.000000 plsp-0.21/templated_setup.py
```

### Comparing `plsp-0.2/PKG-INFO` & `plsp-0.21/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,7 @@
-Metadata-Version: 2.1
-Name: plsp
-Version: 0.2
-Summary: A simple, easy to use, and powerful logging library for Python.
-Author: matrikater (Joel Watson)
-Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
-Requires-Dist: templated_setup
-
 # Please Log Shit Please (or `plsp`)
 
 ## Notes
 
 ```text
 info inject is a module allowing you to compile python source code with added debug information.
 this means that the interesting parts of the code stay separate from printing and other debug code.
@@ -183,10 +175,8 @@
 def fib(n):
 	if n <= 1:
 		return n
 	else:
 		return fib(n-1) + fib(n-2)
 
 fib(5)
-```
-## V0.2 released on 16th/5/2024
-added shared state feature that allows sharing `Logger` instance between separate processes.
+```
```

