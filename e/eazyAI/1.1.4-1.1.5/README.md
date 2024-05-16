# Comparing `tmp/eazyAI-1.1.4.tar.gz` & `tmp/eazyAI-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eazyAI-1.1.4.tar", last modified: Tue May 14 17:04:15 2024, max compression
+gzip compressed data, was "eazyAI-1.1.5.tar", last modified: Wed May 15 18:30:53 2024, max compression
```

## Comparing `eazyAI-1.1.4.tar` & `eazyAI-1.1.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-14 17:04:15.556376 eazyAI-1.1.4/
--rw-rw-rw-   0        0        0    35823 2024-05-14 07:06:57.000000 eazyAI-1.1.4/LICENSE
--rw-rw-rw-   0        0        0      389 2024-05-14 17:04:15.554056 eazyAI-1.1.4/PKG-INFO
--rw-rw-rw-   0        0        0       91 2024-05-14 07:06:57.000000 eazyAI-1.1.4/README.md
-drwxrwxrwx   0        0        0        0 2024-05-14 17:04:15.532768 eazyAI-1.1.4/eazyAI/
--rw-rw-rw-   0        0        0       83 2024-05-14 10:56:49.000000 eazyAI-1.1.4/eazyAI/__init__.py
--rw-rw-rw-   0        0        0     4766 2024-05-14 17:04:10.000000 eazyAI-1.1.4/eazyAI/main.py
-drwxrwxrwx   0        0        0        0 2024-05-14 17:04:15.552676 eazyAI-1.1.4/eazyAI.egg-info/
--rw-rw-rw-   0        0        0      389 2024-05-14 17:04:15.000000 eazyAI-1.1.4/eazyAI.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      209 2024-05-14 17:04:15.000000 eazyAI-1.1.4/eazyAI.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-14 17:04:15.000000 eazyAI-1.1.4/eazyAI.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       35 2024-05-14 17:04:15.000000 eazyAI-1.1.4/eazyAI.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-05-14 17:04:15.000000 eazyAI-1.1.4/eazyAI.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-14 17:04:15.557407 eazyAI-1.1.4/setup.cfg
--rw-rw-rw-   0        0        0      494 2024-05-14 17:03:53.000000 eazyAI-1.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-15 18:30:53.517042 eazyAI-1.1.5/
+-rw-rw-rw-   0        0        0    35823 2024-05-14 07:06:57.000000 eazyAI-1.1.5/LICENSE
+-rw-rw-rw-   0        0        0      389 2024-05-15 18:30:53.516021 eazyAI-1.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0       91 2024-05-14 07:06:57.000000 eazyAI-1.1.5/README.md
+drwxrwxrwx   0        0        0        0 2024-05-15 18:30:53.488795 eazyAI-1.1.5/eazyAI/
+-rw-rw-rw-   0        0        0      124 2024-05-15 18:29:36.000000 eazyAI-1.1.5/eazyAI/__init__.py
+-rw-rw-rw-   0        0        0     7439 2024-05-15 18:30:22.000000 eazyAI-1.1.5/eazyAI/main.py
+drwxrwxrwx   0        0        0        0 2024-05-15 18:30:53.514533 eazyAI-1.1.5/eazyAI.egg-info/
+-rw-rw-rw-   0        0        0      389 2024-05-15 18:30:53.000000 eazyAI-1.1.5/eazyAI.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      209 2024-05-15 18:30:53.000000 eazyAI-1.1.5/eazyAI.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-15 18:30:53.000000 eazyAI-1.1.5/eazyAI.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       35 2024-05-15 18:30:53.000000 eazyAI-1.1.5/eazyAI.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-05-15 18:30:53.000000 eazyAI-1.1.5/eazyAI.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-15 18:30:53.518042 eazyAI-1.1.5/setup.cfg
+-rw-rw-rw-   0        0        0      494 2024-05-15 18:30:47.000000 eazyAI-1.1.5/setup.py
```

### Comparing `eazyAI-1.1.4/LICENSE` & `eazyAI-1.1.5/LICENSE`

 * *Files identical despite different names*

