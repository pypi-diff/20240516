# Comparing `tmp/RnDNews-0.0.1.tar.gz` & `tmp/RnDNews-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RnDNews-0.0.1.tar", last modified: Wed May 15 16:57:54 2024, max compression
+gzip compressed data, was "RnDNews-0.1.0.tar", last modified: Thu May 16 09:04:53 2024, max compression
```

## Comparing `RnDNews-0.0.1.tar` & `RnDNews-0.1.0.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxrwxr-x   0 hanan     (1000) hanan     (1000)        0 2024-05-15 16:57:54.635581 RnDNews-0.0.1/
--rw-r--r--   0 hanan     (1000) hanan     (1000)      238 2024-05-15 16:57:54.635581 RnDNews-0.0.1/PKG-INFO
--rw-rw-r--   0 hanan     (1000) hanan     (1000)        0 2024-05-08 13:10:51.000000 RnDNews-0.0.1/README.md
-drwxrwxr-x   0 hanan     (1000) hanan     (1000)        0 2024-05-15 16:57:54.635581 RnDNews-0.0.1/RnDNews/
--rw-rw-r--   0 hanan     (1000) hanan     (1000)     4717 2024-05-14 15:46:53.000000 RnDNews-0.0.1/RnDNews/DuckDuckGo_Scraper.py
--rw-rw-r--   0 hanan     (1000) hanan     (1000)     4849 2024-05-14 10:46:50.000000 RnDNews-0.0.1/RnDNews/Google_Scraper.py
--rw-rw-r--   0 hanan     (1000) hanan     (1000)      404 2024-05-14 10:46:50.000000 RnDNews-0.0.1/RnDNews/Scraper.py
--rw-rw-r--   0 hanan     (1000) hanan     (1000)     4084 2024-05-14 16:33:54.000000 RnDNews-0.0.1/RnDNews/Shared_Methods.py
--rw-rw-r--   0 hanan     (1000) hanan     (1000)        0 2024-04-01 13:33:50.000000 RnDNews-0.0.1/RnDNews/__init__.py
--rw-rw-r--   0 hanan     (1000) hanan     (1000)     2276 2024-05-14 16:28:59.000000 RnDNews-0.0.1/RnDNews/config.py
--rw-rw-r--   0 hanan     (1000) hanan     (1000)      793 2024-05-08 10:09:07.000000 RnDNews-0.0.1/RnDNews/test.py
-drwxrwxr-x   0 hanan     (1000) hanan     (1000)        0 2024-05-15 16:57:54.635581 RnDNews-0.0.1/RnDNews.egg-info/
--rw-r--r--   0 hanan     (1000) hanan     (1000)      238 2024-05-15 16:57:54.000000 RnDNews-0.0.1/RnDNews.egg-info/PKG-INFO
--rw-rw-r--   0 hanan     (1000) hanan     (1000)      297 2024-05-15 16:57:54.000000 RnDNews-0.0.1/RnDNews.egg-info/SOURCES.txt
--rw-rw-r--   0 hanan     (1000) hanan     (1000)        1 2024-05-15 16:57:54.000000 RnDNews-0.0.1/RnDNews.egg-info/dependency_links.txt
--rw-rw-r--   0 hanan     (1000) hanan     (1000)        8 2024-05-15 16:57:54.000000 RnDNews-0.0.1/RnDNews.egg-info/top_level.txt
--rw-rw-r--   0 hanan     (1000) hanan     (1000)       38 2024-05-15 16:57:54.635581 RnDNews-0.0.1/setup.cfg
--rw-rw-r--   0 hanan     (1000) hanan     (1000)      394 2024-05-08 10:09:07.000000 RnDNews-0.0.1/setup.py
+drwxrwxr-x   0 hanan     (1000) hanan     (1000)        0 2024-05-16 09:04:53.679830 RnDNews-0.1.0/
+-rw-r--r--   0 hanan     (1000) hanan     (1000)     1253 2024-05-16 09:04:53.679830 RnDNews-0.1.0/PKG-INFO
+-rw-rw-r--   0 hanan     (1000) hanan     (1000)        0 2024-05-08 13:10:51.000000 RnDNews-0.1.0/README.md
+drwxrwxr-x   0 hanan     (1000) hanan     (1000)        0 2024-05-16 09:04:53.675830 RnDNews-0.1.0/RnDNews/
+-rw-rw-r--   0 hanan     (1000) hanan     (1000)     4717 2024-05-14 15:46:53.000000 RnDNews-0.1.0/RnDNews/DuckDuckGo_Scraper.py
+-rw-rw-r--   0 hanan     (1000) hanan     (1000)     4849 2024-05-14 10:46:50.000000 RnDNews-0.1.0/RnDNews/Google_Scraper.py
+-rw-rw-r--   0 hanan     (1000) hanan     (1000)      404 2024-05-14 10:46:50.000000 RnDNews-0.1.0/RnDNews/Scraper.py
+-rw-rw-r--   0 hanan     (1000) hanan     (1000)     4084 2024-05-14 16:33:54.000000 RnDNews-0.1.0/RnDNews/Shared_Methods.py
+-rw-rw-r--   0 hanan     (1000) hanan     (1000)        0 2024-04-01 13:33:50.000000 RnDNews-0.1.0/RnDNews/__init__.py
+-rw-rw-r--   0 hanan     (1000) hanan     (1000)     2276 2024-05-14 16:28:59.000000 RnDNews-0.1.0/RnDNews/config.py
+-rw-rw-r--   0 hanan     (1000) hanan     (1000)      793 2024-05-08 10:09:07.000000 RnDNews-0.1.0/RnDNews/test.py
+drwxrwxr-x   0 hanan     (1000) hanan     (1000)        0 2024-05-16 09:04:53.679830 RnDNews-0.1.0/RnDNews.egg-info/
+-rw-r--r--   0 hanan     (1000) hanan     (1000)     1253 2024-05-16 09:04:53.000000 RnDNews-0.1.0/RnDNews.egg-info/PKG-INFO
+-rw-rw-r--   0 hanan     (1000) hanan     (1000)      327 2024-05-16 09:04:53.000000 RnDNews-0.1.0/RnDNews.egg-info/SOURCES.txt
+-rw-rw-r--   0 hanan     (1000) hanan     (1000)        1 2024-05-16 09:04:53.000000 RnDNews-0.1.0/RnDNews.egg-info/dependency_links.txt
+-rw-rw-r--   0 hanan     (1000) hanan     (1000)      550 2024-05-16 09:04:53.000000 RnDNews-0.1.0/RnDNews.egg-info/requires.txt
+-rw-rw-r--   0 hanan     (1000) hanan     (1000)        8 2024-05-16 09:04:53.000000 RnDNews-0.1.0/RnDNews.egg-info/top_level.txt
+-rw-rw-r--   0 hanan     (1000) hanan     (1000)       38 2024-05-16 09:04:53.679830 RnDNews-0.1.0/setup.cfg
+-rw-rw-r--   0 hanan     (1000) hanan     (1000)     1291 2024-05-16 09:04:44.000000 RnDNews-0.1.0/setup.py
```

### Comparing `RnDNews-0.0.1/RnDNews/DuckDuckGo_Scraper.py` & `RnDNews-0.1.0/RnDNews/DuckDuckGo_Scraper.py`

 * *Files identical despite different names*

### Comparing `RnDNews-0.0.1/RnDNews/Google_Scraper.py` & `RnDNews-0.1.0/RnDNews/Google_Scraper.py`

 * *Files identical despite different names*

### Comparing `RnDNews-0.0.1/RnDNews/Shared_Methods.py` & `RnDNews-0.1.0/RnDNews/Shared_Methods.py`

 * *Files identical despite different names*

### Comparing `RnDNews-0.0.1/RnDNews/config.py` & `RnDNews-0.1.0/RnDNews/config.py`

 * *Files identical despite different names*

### Comparing `RnDNews-0.0.1/RnDNews/test.py` & `RnDNews-0.1.0/RnDNews/test.py`

 * *Files identical despite different names*

