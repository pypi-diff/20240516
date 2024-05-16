# Comparing `tmp/SDKPythonTestingPanda-1.0.5.tar.gz` & `tmp/SDKPythonTestingPanda-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\SDKPythonTestingPanda-1.0.5.tar", last modified: Thu May 16 15:06:41 2024, max compression
+gzip compressed data, was "dist\SDKPythonTestingPanda-1.0.6.tar", last modified: Thu May 16 15:09:24 2024, max compression
```

## Comparing `SDKPythonTestingPanda-1.0.5.tar` & `SDKPythonTestingPanda-1.0.6.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2024-05-16 15:06:41.000000 SDKPythonTestingPanda-1.0.5/
--rw-rw-rw-   0        0        0      225 2024-05-16 15:06:41.000000 SDKPythonTestingPanda-1.0.5/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-16 15:06:41.000000 SDKPythonTestingPanda-1.0.5/SDKPythonTestingPanda/
--rw-rw-rw-   0        0        0        0 2024-05-16 15:06:31.000000 SDKPythonTestingPanda-1.0.5/SDKPythonTestingPanda/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-16 15:06:41.000000 SDKPythonTestingPanda-1.0.5/SDKPythonTestingPanda.egg-info/
--rw-rw-rw-   0        0        0      225 2024-05-16 15:06:41.000000 SDKPythonTestingPanda-1.0.5/SDKPythonTestingPanda.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      222 2024-05-16 15:06:41.000000 SDKPythonTestingPanda-1.0.5/SDKPythonTestingPanda.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-16 15:06:41.000000 SDKPythonTestingPanda-1.0.5/SDKPythonTestingPanda.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       22 2024-05-16 15:06:41.000000 SDKPythonTestingPanda-1.0.5/SDKPythonTestingPanda.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-16 15:06:41.000000 SDKPythonTestingPanda-1.0.5/setup.cfg
--rw-rw-rw-   0        0        0      248 2024-05-16 15:03:46.000000 SDKPythonTestingPanda-1.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-16 15:09:24.000000 SDKPythonTestingPanda-1.0.6/
+-rw-rw-rw-   0        0        0      225 2024-05-16 15:09:24.000000 SDKPythonTestingPanda-1.0.6/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-16 15:09:24.000000 SDKPythonTestingPanda-1.0.6/SDKPythonTestingPanda/
+-rw-rw-rw-   0        0        0        0 2024-05-16 15:06:31.000000 SDKPythonTestingPanda-1.0.6/SDKPythonTestingPanda/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-16 15:09:24.000000 SDKPythonTestingPanda-1.0.6/SDKPythonTestingPanda.egg-info/
+-rw-rw-rw-   0        0        0      225 2024-05-16 15:09:24.000000 SDKPythonTestingPanda-1.0.6/SDKPythonTestingPanda.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      222 2024-05-16 15:09:24.000000 SDKPythonTestingPanda-1.0.6/SDKPythonTestingPanda.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-16 15:09:24.000000 SDKPythonTestingPanda-1.0.6/SDKPythonTestingPanda.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       22 2024-05-16 15:09:24.000000 SDKPythonTestingPanda-1.0.6/SDKPythonTestingPanda.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-16 15:09:24.000000 SDKPythonTestingPanda-1.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      248 2024-05-16 15:08:29.000000 SDKPythonTestingPanda-1.0.6/setup.py
```

