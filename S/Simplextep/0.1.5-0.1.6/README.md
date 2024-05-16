# Comparing `tmp/simplextep-0.1.5.tar.gz` & `tmp/simplextep-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simplextep-0.1.5.tar", last modified: Thu May 16 07:13:50 2024, max compression
+gzip compressed data, was "simplextep-0.1.6.tar", last modified: Thu May 16 07:33:55 2024, max compression
```

## Comparing `simplextep-0.1.5.tar` & `simplextep-0.1.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-16 07:13:50.641596 simplextep-0.1.5/
--rw-rw-rw-   0        0        0     1082 2024-05-14 20:05:02.000000 simplextep-0.1.5/LICENSE
--rw-rw-rw-   0        0        0       21 2024-05-16 07:13:12.000000 simplextep-0.1.5/MANIFEST.in
--rw-rw-rw-   0        0        0      350 2024-05-16 07:13:50.547030 simplextep-0.1.5/PKG-INFO
--rw-rw-rw-   0        0        0      142 2024-05-14 20:51:03.000000 simplextep-0.1.5/README.md
-drwxrwxrwx   0        0        0        0 2024-05-16 07:13:50.547030 simplextep-0.1.5/Simplextep.egg-info/
--rw-rw-rw-   0        0        0      350 2024-05-16 07:13:50.000000 simplextep-0.1.5/Simplextep.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      221 2024-05-16 07:13:50.000000 simplextep-0.1.5/Simplextep.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-16 07:13:50.000000 simplextep-0.1.5/Simplextep.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       33 2024-05-16 07:13:50.000000 simplextep-0.1.5/Simplextep.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2024-05-16 07:13:50.000000 simplextep-0.1.5/Simplextep.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    40462 2024-05-16 06:22:52.000000 simplextep-0.1.5/Simplextep.py
--rw-rw-rw-   0        0        0       42 2024-05-16 07:13:50.641596 simplextep-0.1.5/setup.cfg
--rw-rw-rw-   0        0        0      402 2024-05-16 07:13:46.000000 simplextep-0.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-16 07:33:55.177585 simplextep-0.1.6/
+-rw-rw-rw-   0        0        0     1082 2024-05-14 20:05:02.000000 simplextep-0.1.6/LICENSE
+-rw-rw-rw-   0        0        0       21 2024-05-16 07:13:12.000000 simplextep-0.1.6/MANIFEST.in
+-rw-rw-rw-   0        0        0      350 2024-05-16 07:33:55.177585 simplextep-0.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0      142 2024-05-14 20:51:03.000000 simplextep-0.1.6/README.md
+drwxrwxrwx   0        0        0        0 2024-05-16 07:33:55.177585 simplextep-0.1.6/Simplextep.egg-info/
+-rw-rw-rw-   0        0        0      350 2024-05-16 07:33:54.000000 simplextep-0.1.6/Simplextep.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      221 2024-05-16 07:33:55.000000 simplextep-0.1.6/Simplextep.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-16 07:33:54.000000 simplextep-0.1.6/Simplextep.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       33 2024-05-16 07:33:54.000000 simplextep-0.1.6/Simplextep.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2024-05-16 07:33:54.000000 simplextep-0.1.6/Simplextep.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    40462 2024-05-16 06:22:52.000000 simplextep-0.1.6/Simplextep.py
+-rw-rw-rw-   0        0        0       42 2024-05-16 07:33:55.177585 simplextep-0.1.6/setup.cfg
+-rw-rw-rw-   0        0        0      402 2024-05-16 07:33:22.000000 simplextep-0.1.6/setup.py
```

### Comparing `simplextep-0.1.5/LICENSE` & `simplextep-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `simplextep-0.1.5/Simplextep.py` & `simplextep-0.1.6/Simplextep.py`

 * *Files identical despite different names*

