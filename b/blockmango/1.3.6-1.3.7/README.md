# Comparing `tmp/blockmango-1.3.6.tar.gz` & `tmp/blockmango-1.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blockmango-1.3.6.tar", last modified: Thu May 16 17:23:55 2024, max compression
+gzip compressed data, was "blockmango-1.3.7.tar", last modified: Thu May 16 19:18:20 2024, max compression
```

## Comparing `blockmango-1.3.6.tar` & `blockmango-1.3.7.tar`

### file list

```diff
@@ -1,17 +1,20 @@
-drwx------   0 userland  (2000) userland  (2000)        0 2024-05-16 17:23:55.330543 blockmango-1.3.6/
--rw-------   0 userland  (2000) userland  (2000)      405 2024-05-16 17:23:55.330543 blockmango-1.3.6/PKG-INFO
-drwx------   0 userland  (2000) userland  (2000)        0 2024-05-16 17:23:55.310543 blockmango-1.3.6/blockmango/
--rw-------   0 userland  (2000) userland  (2000)      172 2024-05-16 17:13:23.000000 blockmango-1.3.6/blockmango/__init__.py
--rw-------   0 userland  (2000) userland  (2000)     7880 2024-05-16 17:15:07.000000 blockmango-1.3.6/blockmango/clan.py
--rw-------   0 userland  (2000) userland  (2000)     2009 2024-05-16 17:16:06.000000 blockmango-1.3.6/blockmango/decoration.py
--rw-------   0 userland  (2000) userland  (2000)     3697 2024-05-16 17:18:28.000000 blockmango-1.3.6/blockmango/friends.py
--rw-------   0 userland  (2000) userland  (2000)     4047 2024-05-16 17:19:20.000000 blockmango-1.3.6/blockmango/groupchat.py
--rw-------   0 userland  (2000) userland  (2000)     3295 2024-05-16 17:21:42.000000 blockmango-1.3.6/blockmango/user.py
-drwx------   0 userland  (2000) userland  (2000)        0 2024-05-16 17:23:55.326543 blockmango-1.3.6/blockmango.egg-info/
--rw-------   0 userland  (2000) userland  (2000)      405 2024-05-16 17:23:54.000000 blockmango-1.3.6/blockmango.egg-info/PKG-INFO
--rw-------   0 userland  (2000) userland  (2000)      309 2024-05-16 17:23:54.000000 blockmango-1.3.6/blockmango.egg-info/SOURCES.txt
--rw-------   0 userland  (2000) userland  (2000)        1 2024-05-16 17:23:54.000000 blockmango-1.3.6/blockmango.egg-info/dependency_links.txt
--rw-------   0 userland  (2000) userland  (2000)        9 2024-05-16 17:23:54.000000 blockmango-1.3.6/blockmango.egg-info/requires.txt
--rw-------   0 userland  (2000) userland  (2000)       11 2024-05-16 17:23:54.000000 blockmango-1.3.6/blockmango.egg-info/top_level.txt
--rw-------   0 userland  (2000) userland  (2000)       38 2024-05-16 17:23:55.330543 blockmango-1.3.6/setup.cfg
--rw-------   0 userland  (2000) userland  (2000)      503 2024-05-16 17:23:18.000000 blockmango-1.3.6/setup.py
+drwx------   0 userland  (2000) userland  (2000)        0 2024-05-16 19:18:20.905168 blockmango-1.3.7/
+-rw-------   0 userland  (2000) userland  (2000)     1061 2024-05-16 17:46:17.000000 blockmango-1.3.7/LICENSE.md
+-rw-------   0 userland  (2000) userland  (2000)      430 2024-05-16 19:18:20.905168 blockmango-1.3.7/PKG-INFO
+-rw-------   0 userland  (2000) userland  (2000)      834 2024-05-16 17:43:12.000000 blockmango-1.3.7/README.md
+drwx------   0 userland  (2000) userland  (2000)        0 2024-05-16 19:18:20.885168 blockmango-1.3.7/blockmango/
+-rw-------   0 userland  (2000) userland  (2000)      172 2024-05-16 19:13:31.000000 blockmango-1.3.7/blockmango/__init__.py
+-rw-------   0 userland  (2000) userland  (2000)     5944 2024-05-16 19:13:31.000000 blockmango-1.3.7/blockmango/clan.py
+-rw-------   0 userland  (2000) userland  (2000)      803 2024-05-16 19:13:31.000000 blockmango-1.3.7/blockmango/constants.py
+-rw-------   0 userland  (2000) userland  (2000)     1839 2024-05-16 19:13:31.000000 blockmango-1.3.7/blockmango/decoration.py
+-rw-------   0 userland  (2000) userland  (2000)     3599 2024-05-16 19:13:31.000000 blockmango-1.3.7/blockmango/friends.py
+-rw-------   0 userland  (2000) userland  (2000)     4319 2024-05-16 19:13:31.000000 blockmango-1.3.7/blockmango/groupchat.py
+-rw-------   0 userland  (2000) userland  (2000)     3374 2024-05-16 19:13:31.000000 blockmango-1.3.7/blockmango/user.py
+drwx------   0 userland  (2000) userland  (2000)        0 2024-05-16 19:18:20.901168 blockmango-1.3.7/blockmango.egg-info/
+-rw-------   0 userland  (2000) userland  (2000)      430 2024-05-16 19:18:20.000000 blockmango-1.3.7/blockmango.egg-info/PKG-INFO
+-rw-------   0 userland  (2000) userland  (2000)      354 2024-05-16 19:18:20.000000 blockmango-1.3.7/blockmango.egg-info/SOURCES.txt
+-rw-------   0 userland  (2000) userland  (2000)        1 2024-05-16 19:18:20.000000 blockmango-1.3.7/blockmango.egg-info/dependency_links.txt
+-rw-------   0 userland  (2000) userland  (2000)        9 2024-05-16 19:18:20.000000 blockmango-1.3.7/blockmango.egg-info/requires.txt
+-rw-------   0 userland  (2000) userland  (2000)       11 2024-05-16 19:18:20.000000 blockmango-1.3.7/blockmango.egg-info/top_level.txt
+-rw-------   0 userland  (2000) userland  (2000)       38 2024-05-16 19:18:20.909168 blockmango-1.3.7/setup.cfg
+-rw-------   0 userland  (2000) userland  (2000)      503 2024-05-16 19:18:13.000000 blockmango-1.3.7/setup.py
```

