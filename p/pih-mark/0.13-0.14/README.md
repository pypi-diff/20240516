# Comparing `tmp/pih-mark-0.13.tar.gz` & `tmp/pih-mark-0.14.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pih-mark-0.13.tar", last modified: Mon Apr 15 06:23:30 2024, max compression
+gzip compressed data, was "pih-mark-0.14.tar", last modified: Mon Apr 15 06:25:41 2024, max compression
```

## Comparing `pih-mark-0.13.tar` & `pih-mark-0.14.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-04-15 06:23:30.737257 pih-mark-0.13/
-drwxrwxrwx   0        0        0        0 2024-04-15 06:23:30.189982 pih-mark-0.13/MarkService/
--rw-rw-rw-   0        0        0        0 2022-10-20 04:44:07.000000 pih-mark-0.13/MarkService/__init__.py
--rw-rw-rw-   0        0        0      146 2024-02-13 23:54:48.000000 pih-mark-0.13/MarkService/__main__.py
--rw-rw-rw-   0        0        0    38542 2024-02-14 00:46:43.000000 pih-mark-0.13/MarkService/api.py
--rw-rw-rw-   0        0        0     1626 2024-02-09 14:42:12.000000 pih-mark-0.13/MarkService/api_test.py
--rw-rw-rw-   0        0        0     1815 2024-04-15 06:22:30.000000 pih-mark-0.13/MarkService/const.py
--rw-rw-rw-   0        0        0     6244 2024-04-15 06:21:49.000000 pih-mark-0.13/MarkService/service.py
--rw-rw-rw-   0        0        0      315 2024-04-15 06:23:30.690375 pih-mark-0.13/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-15 06:23:30.659124 pih-mark-0.13/pih_mark.egg-info/
--rw-rw-rw-   0        0        0      315 2024-04-15 06:23:29.000000 pih-mark-0.13/pih_mark.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      328 2024-04-15 06:23:29.000000 pih-mark-0.13/pih_mark.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-15 06:23:29.000000 pih-mark-0.13/pih_mark.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       56 2024-04-15 06:23:29.000000 pih-mark-0.13/pih_mark.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       22 2024-04-15 06:23:29.000000 pih-mark-0.13/pih_mark.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-04-15 06:23:29.000000 pih-mark-0.13/pih_mark.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-15 06:23:30.737257 pih-mark-0.13/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-15 06:25:42.036622 pih-mark-0.14/
+drwxrwxrwx   0        0        0        0 2024-04-15 06:25:41.630380 pih-mark-0.14/MarkService/
+-rw-rw-rw-   0        0        0        0 2022-10-20 04:44:07.000000 pih-mark-0.14/MarkService/__init__.py
+-rw-rw-rw-   0        0        0      146 2024-02-13 23:54:48.000000 pih-mark-0.14/MarkService/__main__.py
+-rw-rw-rw-   0        0        0    38542 2024-02-14 00:46:43.000000 pih-mark-0.14/MarkService/api.py
+-rw-rw-rw-   0        0        0     1626 2024-02-09 14:42:12.000000 pih-mark-0.14/MarkService/api_test.py
+-rw-rw-rw-   0        0        0     1815 2024-04-15 06:24:48.000000 pih-mark-0.14/MarkService/const.py
+-rw-rw-rw-   0        0        0     6244 2024-04-15 06:21:49.000000 pih-mark-0.14/MarkService/service.py
+-rw-rw-rw-   0        0        0      315 2024-04-15 06:25:42.005390 pih-mark-0.14/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-15 06:25:41.958514 pih-mark-0.14/pih_mark.egg-info/
+-rw-rw-rw-   0        0        0      315 2024-04-15 06:25:41.000000 pih-mark-0.14/pih_mark.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      328 2024-04-15 06:25:41.000000 pih-mark-0.14/pih_mark.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-15 06:25:41.000000 pih-mark-0.14/pih_mark.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       56 2024-04-15 06:25:41.000000 pih-mark-0.14/pih_mark.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       22 2024-04-15 06:25:41.000000 pih-mark-0.14/pih_mark.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-04-15 06:25:41.000000 pih-mark-0.14/pih_mark.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-15 06:25:42.052240 pih-mark-0.14/setup.cfg
```

### Comparing `pih-mark-0.13/MarkService/api.py` & `pih-mark-0.14/MarkService/api.py`

 * *Files identical despite different names*

### Comparing `pih-mark-0.13/MarkService/api_test.py` & `pih-mark-0.14/MarkService/api_test.py`

 * *Files identical despite different names*

### Comparing `pih-mark-0.13/MarkService/const.py` & `pih-mark-0.14/MarkService/const.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from pih.consts.hosts import Hosts
 from pih.collections.service import ServiceDescription
 
 NAME: str = "Mark"
 
 HOST = Hosts.BACKUP_WORKER
 
-VERSION: str = "0.13"
+VERSION: str = "0.14"
 
 PACKAGES: tuple[str, ...] = ("pymssql", "schedule")
 
 SD: ServiceDescription = ServiceDescription(
     name=NAME,
     description="Orion service",
     host=HOST.NAME,
```

### Comparing `pih-mark-0.13/MarkService/service.py` & `pih-mark-0.14/MarkService/service.py`

 * *Files identical despite different names*

