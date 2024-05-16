# Comparing `tmp/blockmango-1.0.tar.gz` & `tmp/blockmango-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blockmango-1.0.tar", last modified: Thu May 16 08:32:31 2024, max compression
+gzip compressed data, was "blockmango-1.1.tar", last modified: Thu May 16 09:25:19 2024, max compression
```

## Comparing `blockmango-1.0.tar` & `blockmango-1.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwx------   0 userland  (2000) userland  (2000)        0 2024-05-16 08:32:31.935711 blockmango-1.0/
--rw-------   0 userland  (2000) userland  (2000)      405 2024-05-16 08:32:31.935711 blockmango-1.0/PKG-INFO
-drwx------   0 userland  (2000) userland  (2000)        0 2024-05-16 08:32:31.919711 blockmango-1.0/blockmango/
--rw-------   0 userland  (2000) userland  (2000)        0 2024-05-04 19:42:32.000000 blockmango-1.0/blockmango/__init__.py
--rw-------   0 userland  (2000) userland  (2000)     7939 2024-05-04 19:42:16.000000 blockmango-1.0/blockmango/clan.py
--rw-------   0 userland  (2000) userland  (2000)     1825 2024-05-16 08:32:01.000000 blockmango-1.0/blockmango/decoration.py
--rw-------   0 userland  (2000) userland  (2000)       35 2024-05-04 19:41:46.000000 blockmango-1.0/blockmango/exceptions.py
--rw-------   0 userland  (2000) userland  (2000)     3791 2024-05-11 09:51:08.000000 blockmango-1.0/blockmango/friends.py
--rw-------   0 userland  (2000) userland  (2000)     4140 2024-05-07 13:28:40.000000 blockmango-1.0/blockmango/groupchat.py
--rw-------   0 userland  (2000) userland  (2000)     3163 2024-05-16 13:21:24.000000 blockmango-1.0/blockmango/user.py
--rw-------   0 userland  (2000) userland  (2000)       87 2024-05-04 19:44:48.000000 blockmango-1.0/blockmango/util.py
-drwx------   0 userland  (2000) userland  (2000)        0 2024-05-16 08:32:31.931711 blockmango-1.0/blockmango.egg-info/
--rw-------   0 userland  (2000) userland  (2000)      405 2024-05-16 08:32:31.000000 blockmango-1.0/blockmango.egg-info/PKG-INFO
--rw-------   0 userland  (2000) userland  (2000)      353 2024-05-16 08:32:31.000000 blockmango-1.0/blockmango.egg-info/SOURCES.txt
--rw-------   0 userland  (2000) userland  (2000)        1 2024-05-16 08:32:31.000000 blockmango-1.0/blockmango.egg-info/dependency_links.txt
--rw-------   0 userland  (2000) userland  (2000)        9 2024-05-16 08:32:31.000000 blockmango-1.0/blockmango.egg-info/requires.txt
--rw-------   0 userland  (2000) userland  (2000)       11 2024-05-16 08:32:31.000000 blockmango-1.0/blockmango.egg-info/top_level.txt
--rw-------   0 userland  (2000) userland  (2000)       38 2024-05-16 08:32:31.935711 blockmango-1.0/setup.cfg
--rw-------   0 userland  (2000) userland  (2000)      503 2024-05-16 13:50:20.000000 blockmango-1.0/setup.py
+drwx------   0 userland  (2000) userland  (2000)        0 2024-05-16 09:25:19.843710 blockmango-1.1/
+-rw-------   0 userland  (2000) userland  (2000)      403 2024-05-16 09:25:19.839709 blockmango-1.1/PKG-INFO
+drwx------   0 userland  (2000) userland  (2000)        0 2024-05-16 09:25:19.819709 blockmango-1.1/blockmango/
+-rw-------   0 userland  (2000) userland  (2000)      172 2024-05-16 09:24:00.000000 blockmango-1.1/blockmango/__init__.py
+-rw-------   0 userland  (2000) userland  (2000)     7939 2024-05-04 19:42:16.000000 blockmango-1.1/blockmango/clan.py
+-rw-------   0 userland  (2000) userland  (2000)     1825 2024-05-16 09:24:50.000000 blockmango-1.1/blockmango/decoration.py
+-rw-------   0 userland  (2000) userland  (2000)       35 2024-05-04 19:41:46.000000 blockmango-1.1/blockmango/exceptions.py
+-rw-------   0 userland  (2000) userland  (2000)     3791 2024-05-11 09:51:08.000000 blockmango-1.1/blockmango/friends.py
+-rw-------   0 userland  (2000) userland  (2000)     4140 2024-05-07 13:28:40.000000 blockmango-1.1/blockmango/groupchat.py
+-rw-------   0 userland  (2000) userland  (2000)     3163 2024-05-16 13:21:24.000000 blockmango-1.1/blockmango/user.py
+-rw-------   0 userland  (2000) userland  (2000)       87 2024-05-04 19:44:48.000000 blockmango-1.1/blockmango/util.py
+drwx------   0 userland  (2000) userland  (2000)        0 2024-05-16 09:25:19.835709 blockmango-1.1/blockmango.egg-info/
+-rw-------   0 userland  (2000) userland  (2000)      403 2024-05-16 09:25:19.000000 blockmango-1.1/blockmango.egg-info/PKG-INFO
+-rw-------   0 userland  (2000) userland  (2000)      353 2024-05-16 09:25:19.000000 blockmango-1.1/blockmango.egg-info/SOURCES.txt
+-rw-------   0 userland  (2000) userland  (2000)        1 2024-05-16 09:25:19.000000 blockmango-1.1/blockmango.egg-info/dependency_links.txt
+-rw-------   0 userland  (2000) userland  (2000)        9 2024-05-16 09:25:19.000000 blockmango-1.1/blockmango.egg-info/requires.txt
+-rw-------   0 userland  (2000) userland  (2000)       11 2024-05-16 09:25:19.000000 blockmango-1.1/blockmango.egg-info/top_level.txt
+-rw-------   0 userland  (2000) userland  (2000)       38 2024-05-16 09:25:19.843710 blockmango-1.1/setup.cfg
+-rw-------   0 userland  (2000) userland  (2000)      501 2024-05-16 09:21:22.000000 blockmango-1.1/setup.py
```

### Comparing `blockmango-1.0/blockmango/clan.py` & `blockmango-1.1/blockmango/clan.py`

 * *Files identical despite different names*

### Comparing `blockmango-1.0/blockmango/decoration.py` & `blockmango-1.1/blockmango/decoration.py`

 * *Files identical despite different names*

### Comparing `blockmango-1.0/blockmango/friends.py` & `blockmango-1.1/blockmango/friends.py`

 * *Files identical despite different names*

### Comparing `blockmango-1.0/blockmango/groupchat.py` & `blockmango-1.1/blockmango/groupchat.py`

 * *Files identical despite different names*

### Comparing `blockmango-1.0/blockmango/user.py` & `blockmango-1.1/blockmango/user.py`

 * *Files identical despite different names*

