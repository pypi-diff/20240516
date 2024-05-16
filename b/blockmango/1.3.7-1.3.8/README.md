# Comparing `tmp/blockmango-1.3.7.tar.gz` & `tmp/blockmango-1.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blockmango-1.3.7.tar", last modified: Thu May 16 19:18:20 2024, max compression
+gzip compressed data, was "blockmango-1.3.8.tar", last modified: Thu May 16 19:39:23 2024, max compression
```

## Comparing `blockmango-1.3.7.tar` & `blockmango-1.3.8.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwx------   0 userland  (2000) userland  (2000)        0 2024-05-16 19:18:20.905168 blockmango-1.3.7/
--rw-------   0 userland  (2000) userland  (2000)     1061 2024-05-16 17:46:17.000000 blockmango-1.3.7/LICENSE.md
--rw-------   0 userland  (2000) userland  (2000)      430 2024-05-16 19:18:20.905168 blockmango-1.3.7/PKG-INFO
--rw-------   0 userland  (2000) userland  (2000)      834 2024-05-16 17:43:12.000000 blockmango-1.3.7/README.md
-drwx------   0 userland  (2000) userland  (2000)        0 2024-05-16 19:18:20.885168 blockmango-1.3.7/blockmango/
--rw-------   0 userland  (2000) userland  (2000)      172 2024-05-16 19:13:31.000000 blockmango-1.3.7/blockmango/__init__.py
--rw-------   0 userland  (2000) userland  (2000)     5944 2024-05-16 19:13:31.000000 blockmango-1.3.7/blockmango/clan.py
--rw-------   0 userland  (2000) userland  (2000)      803 2024-05-16 19:13:31.000000 blockmango-1.3.7/blockmango/constants.py
--rw-------   0 userland  (2000) userland  (2000)     1839 2024-05-16 19:13:31.000000 blockmango-1.3.7/blockmango/decoration.py
--rw-------   0 userland  (2000) userland  (2000)     3599 2024-05-16 19:13:31.000000 blockmango-1.3.7/blockmango/friends.py
--rw-------   0 userland  (2000) userland  (2000)     4319 2024-05-16 19:13:31.000000 blockmango-1.3.7/blockmango/groupchat.py
--rw-------   0 userland  (2000) userland  (2000)     3374 2024-05-16 19:13:31.000000 blockmango-1.3.7/blockmango/user.py
-drwx------   0 userland  (2000) userland  (2000)        0 2024-05-16 19:18:20.901168 blockmango-1.3.7/blockmango.egg-info/
--rw-------   0 userland  (2000) userland  (2000)      430 2024-05-16 19:18:20.000000 blockmango-1.3.7/blockmango.egg-info/PKG-INFO
--rw-------   0 userland  (2000) userland  (2000)      354 2024-05-16 19:18:20.000000 blockmango-1.3.7/blockmango.egg-info/SOURCES.txt
--rw-------   0 userland  (2000) userland  (2000)        1 2024-05-16 19:18:20.000000 blockmango-1.3.7/blockmango.egg-info/dependency_links.txt
--rw-------   0 userland  (2000) userland  (2000)        9 2024-05-16 19:18:20.000000 blockmango-1.3.7/blockmango.egg-info/requires.txt
--rw-------   0 userland  (2000) userland  (2000)       11 2024-05-16 19:18:20.000000 blockmango-1.3.7/blockmango.egg-info/top_level.txt
--rw-------   0 userland  (2000) userland  (2000)       38 2024-05-16 19:18:20.909168 blockmango-1.3.7/setup.cfg
--rw-------   0 userland  (2000) userland  (2000)      503 2024-05-16 19:18:13.000000 blockmango-1.3.7/setup.py
+drwx------   0 userland  (2000) userland  (2000)        0 2024-05-16 19:39:23.465167 blockmango-1.3.8/
+-rw-------   0 userland  (2000) userland  (2000)     1061 2024-05-16 17:46:17.000000 blockmango-1.3.8/LICENSE.md
+-rw-------   0 userland  (2000) userland  (2000)      430 2024-05-16 19:39:23.465167 blockmango-1.3.8/PKG-INFO
+-rw-------   0 userland  (2000) userland  (2000)      834 2024-05-16 17:43:12.000000 blockmango-1.3.8/README.md
+drwx------   0 userland  (2000) userland  (2000)        0 2024-05-16 19:39:23.441167 blockmango-1.3.8/blockmango/
+-rw-------   0 userland  (2000) userland  (2000)      172 2024-05-16 19:13:31.000000 blockmango-1.3.8/blockmango/__init__.py
+-rw-------   0 userland  (2000) userland  (2000)     5944 2024-05-16 19:13:31.000000 blockmango-1.3.8/blockmango/clan.py
+-rw-------   0 userland  (2000) userland  (2000)      748 2024-05-16 19:37:41.000000 blockmango-1.3.8/blockmango/constants.py
+-rw-------   0 userland  (2000) userland  (2000)     1839 2024-05-16 19:13:31.000000 blockmango-1.3.8/blockmango/decoration.py
+-rw-------   0 userland  (2000) userland  (2000)     3599 2024-05-16 19:13:31.000000 blockmango-1.3.8/blockmango/friends.py
+-rw-------   0 userland  (2000) userland  (2000)     4319 2024-05-16 19:13:31.000000 blockmango-1.3.8/blockmango/groupchat.py
+-rw-------   0 userland  (2000) userland  (2000)     3374 2024-05-16 19:13:31.000000 blockmango-1.3.8/blockmango/user.py
+drwx------   0 userland  (2000) userland  (2000)        0 2024-05-16 19:39:23.461167 blockmango-1.3.8/blockmango.egg-info/
+-rw-------   0 userland  (2000) userland  (2000)      430 2024-05-16 19:39:23.000000 blockmango-1.3.8/blockmango.egg-info/PKG-INFO
+-rw-------   0 userland  (2000) userland  (2000)      354 2024-05-16 19:39:23.000000 blockmango-1.3.8/blockmango.egg-info/SOURCES.txt
+-rw-------   0 userland  (2000) userland  (2000)        1 2024-05-16 19:39:23.000000 blockmango-1.3.8/blockmango.egg-info/dependency_links.txt
+-rw-------   0 userland  (2000) userland  (2000)        9 2024-05-16 19:39:23.000000 blockmango-1.3.8/blockmango.egg-info/requires.txt
+-rw-------   0 userland  (2000) userland  (2000)       11 2024-05-16 19:39:23.000000 blockmango-1.3.8/blockmango.egg-info/top_level.txt
+-rw-------   0 userland  (2000) userland  (2000)       38 2024-05-16 19:39:23.465167 blockmango-1.3.8/setup.cfg
+-rw-------   0 userland  (2000) userland  (2000)      503 2024-05-16 19:39:16.000000 blockmango-1.3.8/setup.py
```

### Comparing `blockmango-1.3.7/LICENSE.md` & `blockmango-1.3.8/LICENSE.md`

 * *Files identical despite different names*

### Comparing `blockmango-1.3.7/README.md` & `blockmango-1.3.8/README.md`

 * *Files identical despite different names*

### Comparing `blockmango-1.3.7/blockmango/clan.py` & `blockmango-1.3.8/blockmango/clan.py`

 * *Files identical despite different names*

### Comparing `blockmango-1.3.7/blockmango/constants.py` & `blockmango-1.3.8/blockmango/constants.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,13 +10,12 @@
 BASE_URL_GROUP_V2 = "http://modsgs.sandboxol.com/msg/api/v2"
 
 BASE_URL_DECORATION = "http://modsgs.sandboxol.com/decoration/api/v1"
 BASE_URL_SHOP = "http://modsgs.sandboxol.com/shop/api/v1"
 BASE_URL_USER = "http://modsgs.sandboxol.com/user/api/v1"
 BASE_URL_FRIEND = "http://modsgs.sandboxol.com/friend/api/v1"
 
-BASE_URL_USER = "http://modsgs.sandboxol.com/user/api"
 BASE_URL_ROUTE = "http://route.sandboxol.com/user/api"
 
 HEADERS_TEMPLATE = {
     "User-Agent": "okhttp/3.12.1"
 }
```

### Comparing `blockmango-1.3.7/blockmango/decoration.py` & `blockmango-1.3.8/blockmango/decoration.py`

 * *Files identical despite different names*

### Comparing `blockmango-1.3.7/blockmango/friends.py` & `blockmango-1.3.8/blockmango/friends.py`

 * *Files identical despite different names*

### Comparing `blockmango-1.3.7/blockmango/groupchat.py` & `blockmango-1.3.8/blockmango/groupchat.py`

 * *Files identical despite different names*

### Comparing `blockmango-1.3.7/blockmango/user.py` & `blockmango-1.3.8/blockmango/user.py`

 * *Files identical despite different names*

