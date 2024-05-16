# Comparing `tmp/SDKPythonTestingPanda-1.2.0.tar.gz` & `tmp/SDKPythonTestingPanda-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\SDKPythonTestingPanda-1.2.0.tar", last modified: Thu May 16 15:28:56 2024, max compression
+gzip compressed data, was "dist\SDKPythonTestingPanda-1.3.0.tar", last modified: Thu May 16 15:30:10 2024, max compression
```

## Comparing `SDKPythonTestingPanda-1.2.0.tar` & `SDKPythonTestingPanda-1.3.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-05-16 15:28:56.000000 SDKPythonTestingPanda-1.2.0/
--rw-rw-rw-   0        0        0      225 2024-05-16 15:28:56.000000 SDKPythonTestingPanda-1.2.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-16 15:28:56.000000 SDKPythonTestingPanda-1.2.0/SDKPythonTestingPanda/
--rw-rw-rw-   0        0        0       90 2024-05-16 14:45:21.000000 SDKPythonTestingPanda-1.2.0/SDKPythonTestingPanda/SDKPythonTestingPanda.py
--rw-rw-rw-   0        0        0        0 2024-05-16 15:22:25.000000 SDKPythonTestingPanda-1.2.0/SDKPythonTestingPanda/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-16 15:28:56.000000 SDKPythonTestingPanda-1.2.0/SDKPythonTestingPanda.egg-info/
--rw-rw-rw-   0        0        0      225 2024-05-16 15:28:56.000000 SDKPythonTestingPanda-1.2.0/SDKPythonTestingPanda.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      269 2024-05-16 15:28:56.000000 SDKPythonTestingPanda-1.2.0/SDKPythonTestingPanda.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-16 15:28:56.000000 SDKPythonTestingPanda-1.2.0/SDKPythonTestingPanda.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       22 2024-05-16 15:28:56.000000 SDKPythonTestingPanda-1.2.0/SDKPythonTestingPanda.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-16 15:28:56.000000 SDKPythonTestingPanda-1.2.0/setup.cfg
--rw-rw-rw-   0        0        0      248 2024-05-16 15:28:00.000000 SDKPythonTestingPanda-1.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-16 15:30:10.000000 SDKPythonTestingPanda-1.3.0/
+-rw-rw-rw-   0        0        0      225 2024-05-16 15:30:10.000000 SDKPythonTestingPanda-1.3.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-16 15:30:10.000000 SDKPythonTestingPanda-1.3.0/SDKPythonTestingPanda/
+-rw-rw-rw-   0        0        0       90 2024-05-16 14:45:21.000000 SDKPythonTestingPanda-1.3.0/SDKPythonTestingPanda/SDKPythonTestingPanda.py
+-rw-rw-rw-   0        0        0        0 2024-05-16 15:22:25.000000 SDKPythonTestingPanda-1.3.0/SDKPythonTestingPanda/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-16 15:30:10.000000 SDKPythonTestingPanda-1.3.0/SDKPythonTestingPanda.egg-info/
+-rw-rw-rw-   0        0        0      225 2024-05-16 15:30:10.000000 SDKPythonTestingPanda-1.3.0/SDKPythonTestingPanda.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      269 2024-05-16 15:30:10.000000 SDKPythonTestingPanda-1.3.0/SDKPythonTestingPanda.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-16 15:30:10.000000 SDKPythonTestingPanda-1.3.0/SDKPythonTestingPanda.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       22 2024-05-16 15:30:10.000000 SDKPythonTestingPanda-1.3.0/SDKPythonTestingPanda.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-16 15:30:10.000000 SDKPythonTestingPanda-1.3.0/setup.cfg
+-rw-rw-rw-   0        0        0      248 2024-05-16 15:30:07.000000 SDKPythonTestingPanda-1.3.0/setup.py
```

