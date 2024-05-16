# Comparing `tmp/simplextep-0.1.2.tar.gz` & `tmp/simplextep-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simplextep-0.1.2.tar", last modified: Tue May 14 21:13:23 2024, max compression
+gzip compressed data, was "simplextep-0.1.3.tar", last modified: Thu May 16 06:25:20 2024, max compression
```

## Comparing `simplextep-0.1.2.tar` & `simplextep-0.1.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-05-14 21:13:23.456365 simplextep-0.1.2/
--rw-rw-rw-   0        0        0     1082 2024-05-14 20:05:02.000000 simplextep-0.1.2/LICENSE
--rw-rw-rw-   0        0        0      336 2024-05-14 21:13:23.456365 simplextep-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0      142 2024-05-14 20:51:03.000000 simplextep-0.1.2/README.md
-drwxrwxrwx   0        0        0        0 2024-05-14 21:13:23.440696 simplextep-0.1.2/Simplextep.egg-info/
--rw-rw-rw-   0        0        0      336 2024-05-14 21:13:23.000000 simplextep-0.1.2/Simplextep.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      195 2024-05-14 21:13:23.000000 simplextep-0.1.2/Simplextep.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-14 21:13:23.000000 simplextep-0.1.2/Simplextep.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       33 2024-05-14 21:13:23.000000 simplextep-0.1.2/Simplextep.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2024-05-14 21:13:23.000000 simplextep-0.1.2/Simplextep.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-14 21:13:23.456365 simplextep-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0      383 2024-05-14 21:13:01.000000 simplextep-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-16 06:25:20.634047 simplextep-0.1.3/
+-rw-rw-rw-   0        0        0     1082 2024-05-14 20:05:02.000000 simplextep-0.1.3/LICENSE
+-rw-rw-rw-   0        0        0      336 2024-05-16 06:25:20.634047 simplextep-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0      142 2024-05-14 20:51:03.000000 simplextep-0.1.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-16 06:25:20.634047 simplextep-0.1.3/Simplextep.egg-info/
+-rw-rw-rw-   0        0        0      336 2024-05-16 06:25:20.000000 simplextep-0.1.3/Simplextep.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      195 2024-05-16 06:25:20.000000 simplextep-0.1.3/Simplextep.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-16 06:25:20.000000 simplextep-0.1.3/Simplextep.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       33 2024-05-16 06:25:20.000000 simplextep-0.1.3/Simplextep.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2024-05-16 06:25:20.000000 simplextep-0.1.3/Simplextep.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-16 06:25:20.634047 simplextep-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      383 2024-05-16 06:25:13.000000 simplextep-0.1.3/setup.py
```

### Comparing `simplextep-0.1.2/LICENSE` & `simplextep-0.1.3/LICENSE`

 * *Files identical despite different names*

