# Comparing `tmp/SDKPythonTestingPanda-1.0.8.tar.gz` & `tmp/SDKPythonTestingPanda-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\SDKPythonTestingPanda-1.0.8.tar", last modified: Thu May 16 15:17:03 2024, max compression
+gzip compressed data, was "dist\SDKPythonTestingPanda-1.1.0.tar", last modified: Thu May 16 15:22:28 2024, max compression
```

## Comparing `SDKPythonTestingPanda-1.0.8.tar` & `SDKPythonTestingPanda-1.1.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2024-05-16 15:17:03.000000 SDKPythonTestingPanda-1.0.8/
--rw-rw-rw-   0        0        0      225 2024-05-16 15:17:03.000000 SDKPythonTestingPanda-1.0.8/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-16 15:17:03.000000 SDKPythonTestingPanda-1.0.8/SDKPythonTestingPanda/
--rw-rw-rw-   0        0        0        0 2024-05-16 15:16:53.000000 SDKPythonTestingPanda-1.0.8/SDKPythonTestingPanda/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-16 15:17:03.000000 SDKPythonTestingPanda-1.0.8/SDKPythonTestingPanda.egg-info/
--rw-rw-rw-   0        0        0      225 2024-05-16 15:17:03.000000 SDKPythonTestingPanda-1.0.8/SDKPythonTestingPanda.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      222 2024-05-16 15:17:03.000000 SDKPythonTestingPanda-1.0.8/SDKPythonTestingPanda.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-16 15:17:03.000000 SDKPythonTestingPanda-1.0.8/SDKPythonTestingPanda.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       22 2024-05-16 15:17:03.000000 SDKPythonTestingPanda-1.0.8/SDKPythonTestingPanda.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-16 15:17:03.000000 SDKPythonTestingPanda-1.0.8/setup.cfg
--rw-rw-rw-   0        0        0      248 2024-05-16 15:16:56.000000 SDKPythonTestingPanda-1.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-16 15:22:28.000000 SDKPythonTestingPanda-1.1.0/
+-rw-rw-rw-   0        0        0      225 2024-05-16 15:22:28.000000 SDKPythonTestingPanda-1.1.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-16 15:22:28.000000 SDKPythonTestingPanda-1.1.0/SDKPythonTestingPanda/
+-rw-rw-rw-   0        0        0        0 2024-05-16 15:22:25.000000 SDKPythonTestingPanda-1.1.0/SDKPythonTestingPanda/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-16 15:22:28.000000 SDKPythonTestingPanda-1.1.0/SDKPythonTestingPanda.egg-info/
+-rw-rw-rw-   0        0        0      225 2024-05-16 15:22:28.000000 SDKPythonTestingPanda-1.1.0/SDKPythonTestingPanda.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      222 2024-05-16 15:22:28.000000 SDKPythonTestingPanda-1.1.0/SDKPythonTestingPanda.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-16 15:22:28.000000 SDKPythonTestingPanda-1.1.0/SDKPythonTestingPanda.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       22 2024-05-16 15:22:28.000000 SDKPythonTestingPanda-1.1.0/SDKPythonTestingPanda.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-16 15:22:28.000000 SDKPythonTestingPanda-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      248 2024-05-16 15:21:16.000000 SDKPythonTestingPanda-1.1.0/setup.py
```

