# Comparing `tmp/saes6-jerry-0.0.9.tar.gz` & `tmp/saes6_jerry-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "saes6-jerry-0.0.9.tar", last modified: Tue May 14 09:34:22 2024, max compression
+gzip compressed data, was "saes6_jerry-0.1.1.tar", last modified: Wed May 15 14:52:53 2024, max compression
```

## Comparing `saes6-jerry-0.0.9.tar` & `saes6_jerry-0.1.1.tar`

### file list

```diff
@@ -1,13 +1,20 @@
-drwxr-xr-x   0 gonzales   (501) staff       (20)        0 2024-05-14 09:34:22.861887 saes6-jerry-0.0.9/
--rw-r--r--   0 gonzales   (501) staff       (20)      370 2024-05-14 09:34:22.861665 saes6-jerry-0.0.9/PKG-INFO
-drwxr-xr-x   0 gonzales   (501) staff       (20)        0 2024-05-14 09:34:22.860708 saes6-jerry-0.0.9/jerry/
--rw-r--r--   0 gonzales   (501) staff       (20)       45 2024-05-14 09:34:03.000000 saes6-jerry-0.0.9/jerry/__init__.py
--rw-r--r--   0 gonzales   (501) staff       (20)      178 2024-05-14 09:33:55.000000 saes6-jerry-0.0.9/jerry/main.py
-drwxr-xr-x   0 gonzales   (501) staff       (20)        0 2024-05-14 09:34:22.861485 saes6-jerry-0.0.9/saes6_jerry.egg-info/
--rw-r--r--   0 gonzales   (501) staff       (20)      370 2024-05-14 09:34:22.000000 saes6-jerry-0.0.9/saes6_jerry.egg-info/PKG-INFO
--rw-r--r--   0 gonzales   (501) staff       (20)      218 2024-05-14 09:34:22.000000 saes6-jerry-0.0.9/saes6_jerry.egg-info/SOURCES.txt
--rw-r--r--   0 gonzales   (501) staff       (20)        1 2024-05-14 09:34:22.000000 saes6-jerry-0.0.9/saes6_jerry.egg-info/dependency_links.txt
--rw-r--r--   0 gonzales   (501) staff       (20)       43 2024-05-14 09:34:22.000000 saes6-jerry-0.0.9/saes6_jerry.egg-info/entry_points.txt
--rw-r--r--   0 gonzales   (501) staff       (20)        6 2024-05-14 09:34:22.000000 saes6-jerry-0.0.9/saes6_jerry.egg-info/top_level.txt
--rw-r--r--   0 gonzales   (501) staff       (20)       38 2024-05-14 09:34:22.861930 saes6-jerry-0.0.9/setup.cfg
--rw-r--r--   0 gonzales   (501) staff       (20)      657 2024-05-14 09:31:35.000000 saes6-jerry-0.0.9/setup.py
+drwxr-xr-x   0 gonzales   (501) staff       (20)        0 2024-05-15 14:52:53.541391 saes6_jerry-0.1.1/
+-rw-r--r--   0 gonzales   (501) staff       (20)      370 2024-05-15 14:52:53.541188 saes6_jerry-0.1.1/PKG-INFO
+-rw-r--r--   0 gonzales   (501) staff       (20)     2521 2024-05-15 14:40:59.000000 saes6_jerry-0.1.1/README.md
+drwxr-xr-x   0 gonzales   (501) staff       (20)        0 2024-05-15 14:52:53.539359 saes6_jerry-0.1.1/jerry/
+-rw-r--r--   0 gonzales   (501) staff       (20)       45 2024-05-15 14:52:51.000000 saes6_jerry-0.1.1/jerry/__init__.py
+drwxr-xr-x   0 gonzales   (501) staff       (20)        0 2024-05-15 14:52:53.539707 saes6_jerry-0.1.1/jerry/attacks/
+-rw-r--r--   0 gonzales   (501) staff       (20)        0 2024-05-15 08:19:40.000000 saes6_jerry-0.1.1/jerry/attacks/__init__.py
+drwxr-xr-x   0 gonzales   (501) staff       (20)        0 2024-05-15 14:52:53.540036 saes6_jerry-0.1.1/jerry/attacks/bruteforce/
+-rw-r--r--   0 gonzales   (501) staff       (20)        0 2024-05-15 13:26:49.000000 saes6_jerry-0.1.1/jerry/attacks/bruteforce/__init__.py
+-rw-r--r--   0 gonzales   (501) staff       (20)     3084 2024-05-15 13:26:49.000000 saes6_jerry-0.1.1/jerry/attacks/bruteforce/bruteforce.py
+-rw-r--r--   0 gonzales   (501) staff       (20)     2855 2024-05-15 14:45:05.000000 saes6_jerry-0.1.1/jerry/attacks/sys_infos.py
+-rw-r--r--   0 gonzales   (501) staff       (20)     2243 2024-05-15 14:33:24.000000 saes6_jerry-0.1.1/jerry/main.py
+drwxr-xr-x   0 gonzales   (501) staff       (20)        0 2024-05-15 14:52:53.540980 saes6_jerry-0.1.1/saes6_jerry.egg-info/
+-rw-r--r--   0 gonzales   (501) staff       (20)      370 2024-05-15 14:52:53.000000 saes6_jerry-0.1.1/saes6_jerry.egg-info/PKG-INFO
+-rw-r--r--   0 gonzales   (501) staff       (20)      357 2024-05-15 14:52:53.000000 saes6_jerry-0.1.1/saes6_jerry.egg-info/SOURCES.txt
+-rw-r--r--   0 gonzales   (501) staff       (20)        1 2024-05-15 14:52:53.000000 saes6_jerry-0.1.1/saes6_jerry.egg-info/dependency_links.txt
+-rw-r--r--   0 gonzales   (501) staff       (20)       43 2024-05-15 14:52:53.000000 saes6_jerry-0.1.1/saes6_jerry.egg-info/entry_points.txt
+-rw-r--r--   0 gonzales   (501) staff       (20)        6 2024-05-15 14:52:53.000000 saes6_jerry-0.1.1/saes6_jerry.egg-info/top_level.txt
+-rw-r--r--   0 gonzales   (501) staff       (20)       38 2024-05-15 14:52:53.541433 saes6_jerry-0.1.1/setup.cfg
+-rw-r--r--   0 gonzales   (501) staff       (20)      657 2024-05-14 09:31:35.000000 saes6_jerry-0.1.1/setup.py
```

### Comparing `saes6-jerry-0.0.9/setup.py` & `saes6_jerry-0.1.1/setup.py`

 * *Files identical despite different names*

