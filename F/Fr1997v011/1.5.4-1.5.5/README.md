# Comparing `tmp/Fr1997v011-1.5.4.tar.gz` & `tmp/Fr1997v011-1.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Fr1997v011-1.5.4.tar", last modified: Wed May 15 09:56:29 2024, max compression
+gzip compressed data, was "Fr1997v011-1.5.5.tar", last modified: Wed May 15 10:48:25 2024, max compression
```

## Comparing `Fr1997v011-1.5.4.tar` & `Fr1997v011-1.5.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-05-15 09:56:29.424118 Fr1997v011-1.5.4/
-drwxrwxrwx   0        0        0        0 2024-05-15 09:56:29.404499 Fr1997v011-1.5.4/Fr1997v011.egg-info/
--rw-rw-rw-   0        0        0      182 2024-05-15 09:56:29.000000 Fr1997v011-1.5.4/Fr1997v011.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      323 2024-05-15 09:56:29.000000 Fr1997v011-1.5.4/Fr1997v011.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-15 09:56:29.000000 Fr1997v011-1.5.4/Fr1997v011.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-05-14 11:04:08.000000 Fr1997v011-1.5.4/Fr1997v011.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       12 2024-05-15 09:56:29.000000 Fr1997v011-1.5.4/Fr1997v011.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1091 2023-10-08 06:35:50.000000 Fr1997v011-1.5.4/LICENSE
--rw-rw-rw-   0        0        0      182 2024-05-15 09:56:29.421110 Fr1997v011-1.5.4/PKG-INFO
--rw-rw-rw-   0        0        0      773 2024-05-14 11:04:15.000000 Fr1997v011-1.5.4/README.md
-drwxrwxrwx   0        0        0        0 2024-05-15 09:56:29.409019 Fr1997v011-1.5.4/fr1997_mode/
--rw-rw-rw-   0        0        0       56 2023-10-11 07:25:55.000000 Fr1997v011-1.5.4/fr1997_mode/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-15 09:56:29.413535 Fr1997v011-1.5.4/fr1997_mode/mode_func/
--rw-rw-rw-   0        0        0       29 2024-04-25 01:03:20.000000 Fr1997v011-1.5.4/fr1997_mode/mode_func/__init__.py
--rw-rw-rw-   0        0        0   181260 2024-05-15 09:56:27.000000 Fr1997v011-1.5.4/fr1997_mode/mode_func/all_func.py
-drwxrwxrwx   0        0        0        0 2024-05-15 09:56:29.418049 Fr1997v011-1.5.4/fr1997_mode/mode_static/
--rw-rw-rw-   0        0        0        0 2023-10-13 07:18:36.000000 Fr1997v011-1.5.4/fr1997_mode/mode_static/__init__.py
--rw-rw-rw-   0        0        0       42 2024-05-15 09:56:29.424118 Fr1997v011-1.5.4/setup.cfg
--rw-rw-rw-   0        0        0      322 2024-05-14 11:04:05.000000 Fr1997v011-1.5.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-15 10:48:25.557351 Fr1997v011-1.5.5/
+drwxrwxrwx   0        0        0        0 2024-05-15 10:48:25.545771 Fr1997v011-1.5.5/Fr1997v011.egg-info/
+-rw-rw-rw-   0        0        0      182 2024-05-15 10:48:25.000000 Fr1997v011-1.5.5/Fr1997v011.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      323 2024-05-15 10:48:25.000000 Fr1997v011-1.5.5/Fr1997v011.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-15 10:48:25.000000 Fr1997v011-1.5.5/Fr1997v011.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-05-15 10:48:25.000000 Fr1997v011-1.5.5/Fr1997v011.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       12 2024-05-15 10:48:25.000000 Fr1997v011-1.5.5/Fr1997v011.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1091 2023-10-08 06:35:50.000000 Fr1997v011-1.5.5/LICENSE
+-rw-rw-rw-   0        0        0      182 2024-05-15 10:48:25.555343 Fr1997v011-1.5.5/PKG-INFO
+-rw-rw-rw-   0        0        0      773 2024-05-14 11:04:15.000000 Fr1997v011-1.5.5/README.md
+drwxrwxrwx   0        0        0        0 2024-05-15 10:48:25.546777 Fr1997v011-1.5.5/fr1997_mode/
+-rw-rw-rw-   0        0        0       56 2023-10-11 07:25:55.000000 Fr1997v011-1.5.5/fr1997_mode/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-15 10:48:25.551779 Fr1997v011-1.5.5/fr1997_mode/mode_func/
+-rw-rw-rw-   0        0        0       29 2024-04-25 01:03:20.000000 Fr1997v011-1.5.5/fr1997_mode/mode_func/__init__.py
+-rw-rw-rw-   0        0        0   181260 2024-05-15 09:56:27.000000 Fr1997v011-1.5.5/fr1997_mode/mode_func/all_func.py
+drwxrwxrwx   0        0        0        0 2024-05-15 10:48:25.554292 Fr1997v011-1.5.5/fr1997_mode/mode_static/
+-rw-rw-rw-   0        0        0        0 2023-10-13 07:18:36.000000 Fr1997v011-1.5.5/fr1997_mode/mode_static/__init__.py
+-rw-rw-rw-   0        0        0       42 2024-05-15 10:48:25.557351 Fr1997v011-1.5.5/setup.cfg
+-rw-rw-rw-   0        0        0      322 2024-05-15 10:48:23.000000 Fr1997v011-1.5.5/setup.py
```

### Comparing `Fr1997v011-1.5.4/LICENSE` & `Fr1997v011-1.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `Fr1997v011-1.5.4/README.md` & `Fr1997v011-1.5.5/README.md`

 * *Files identical despite different names*

### Comparing `Fr1997v011-1.5.4/fr1997_mode/mode_func/all_func.py` & `Fr1997v011-1.5.5/fr1997_mode/mode_func/all_func.py`

 * *Files identical despite different names*

