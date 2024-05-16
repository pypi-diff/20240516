# Comparing `tmp/blockmango-1.3.8.tar.gz` & `tmp/blockmango-1.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blockmango-1.3.8.tar", last modified: Thu May 16 19:39:23 2024, max compression
+gzip compressed data, was "blockmango-1.3.9.tar", last modified: Thu May 16 19:53:00 2024, max compression
```

## Comparing `blockmango-1.3.8.tar` & `blockmango-1.3.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwx------   0 userland  (2000) userland  (2000)        0 2024-05-16 19:39:23.465167 blockmango-1.3.8/
--rw-------   0 userland  (2000) userland  (2000)     1061 2024-05-16 17:46:17.000000 blockmango-1.3.8/LICENSE.md
--rw-------   0 userland  (2000) userland  (2000)      430 2024-05-16 19:39:23.465167 blockmango-1.3.8/PKG-INFO
--rw-------   0 userland  (2000) userland  (2000)      834 2024-05-16 17:43:12.000000 blockmango-1.3.8/README.md
-drwx------   0 userland  (2000) userland  (2000)        0 2024-05-16 19:39:23.441167 blockmango-1.3.8/blockmango/
--rw-------   0 userland  (2000) userland  (2000)      172 2024-05-16 19:13:31.000000 blockmango-1.3.8/blockmango/__init__.py
--rw-------   0 userland  (2000) userland  (2000)     5944 2024-05-16 19:13:31.000000 blockmango-1.3.8/blockmango/clan.py
--rw-------   0 userland  (2000) userland  (2000)      748 2024-05-16 19:37:41.000000 blockmango-1.3.8/blockmango/constants.py
--rw-------   0 userland  (2000) userland  (2000)     1839 2024-05-16 19:13:31.000000 blockmango-1.3.8/blockmango/decoration.py
--rw-------   0 userland  (2000) userland  (2000)     3599 2024-05-16 19:13:31.000000 blockmango-1.3.8/blockmango/friends.py
--rw-------   0 userland  (2000) userland  (2000)     4319 2024-05-16 19:13:31.000000 blockmango-1.3.8/blockmango/groupchat.py
--rw-------   0 userland  (2000) userland  (2000)     3374 2024-05-16 19:13:31.000000 blockmango-1.3.8/blockmango/user.py
-drwx------   0 userland  (2000) userland  (2000)        0 2024-05-16 19:39:23.461167 blockmango-1.3.8/blockmango.egg-info/
--rw-------   0 userland  (2000) userland  (2000)      430 2024-05-16 19:39:23.000000 blockmango-1.3.8/blockmango.egg-info/PKG-INFO
--rw-------   0 userland  (2000) userland  (2000)      354 2024-05-16 19:39:23.000000 blockmango-1.3.8/blockmango.egg-info/SOURCES.txt
--rw-------   0 userland  (2000) userland  (2000)        1 2024-05-16 19:39:23.000000 blockmango-1.3.8/blockmango.egg-info/dependency_links.txt
--rw-------   0 userland  (2000) userland  (2000)        9 2024-05-16 19:39:23.000000 blockmango-1.3.8/blockmango.egg-info/requires.txt
--rw-------   0 userland  (2000) userland  (2000)       11 2024-05-16 19:39:23.000000 blockmango-1.3.8/blockmango.egg-info/top_level.txt
--rw-------   0 userland  (2000) userland  (2000)       38 2024-05-16 19:39:23.465167 blockmango-1.3.8/setup.cfg
--rw-------   0 userland  (2000) userland  (2000)      503 2024-05-16 19:39:16.000000 blockmango-1.3.8/setup.py
+drwx------   0 userland  (2000) userland  (2000)        0 2024-05-16 19:53:00.897167 blockmango-1.3.9/
+-rw-------   0 userland  (2000) userland  (2000)     1061 2024-05-16 17:46:17.000000 blockmango-1.3.9/LICENSE.md
+-rw-------   0 userland  (2000) userland  (2000)      430 2024-05-16 19:53:00.893167 blockmango-1.3.9/PKG-INFO
+-rw-------   0 userland  (2000) userland  (2000)      834 2024-05-16 17:43:12.000000 blockmango-1.3.9/README.md
+drwx------   0 userland  (2000) userland  (2000)        0 2024-05-16 19:53:00.877167 blockmango-1.3.9/blockmango/
+-rw-------   0 userland  (2000) userland  (2000)      172 2024-05-16 19:13:31.000000 blockmango-1.3.9/blockmango/__init__.py
+-rw-------   0 userland  (2000) userland  (2000)     5988 2024-05-16 19:49:32.000000 blockmango-1.3.9/blockmango/clan.py
+-rw-------   0 userland  (2000) userland  (2000)      748 2024-05-16 19:37:41.000000 blockmango-1.3.9/blockmango/constants.py
+-rw-------   0 userland  (2000) userland  (2000)     1883 2024-05-16 19:49:54.000000 blockmango-1.3.9/blockmango/decoration.py
+-rw-------   0 userland  (2000) userland  (2000)     3643 2024-05-16 19:50:26.000000 blockmango-1.3.9/blockmango/friends.py
+-rw-------   0 userland  (2000) userland  (2000)     4362 2024-05-16 19:51:37.000000 blockmango-1.3.9/blockmango/groupchat.py
+-rw-------   0 userland  (2000) userland  (2000)     3418 2024-05-16 19:52:01.000000 blockmango-1.3.9/blockmango/user.py
+drwx------   0 userland  (2000) userland  (2000)        0 2024-05-16 19:53:00.893167 blockmango-1.3.9/blockmango.egg-info/
+-rw-------   0 userland  (2000) userland  (2000)      430 2024-05-16 19:53:00.000000 blockmango-1.3.9/blockmango.egg-info/PKG-INFO
+-rw-------   0 userland  (2000) userland  (2000)      354 2024-05-16 19:53:00.000000 blockmango-1.3.9/blockmango.egg-info/SOURCES.txt
+-rw-------   0 userland  (2000) userland  (2000)        1 2024-05-16 19:53:00.000000 blockmango-1.3.9/blockmango.egg-info/dependency_links.txt
+-rw-------   0 userland  (2000) userland  (2000)        9 2024-05-16 19:53:00.000000 blockmango-1.3.9/blockmango.egg-info/requires.txt
+-rw-------   0 userland  (2000) userland  (2000)       11 2024-05-16 19:53:00.000000 blockmango-1.3.9/blockmango.egg-info/top_level.txt
+-rw-------   0 userland  (2000) userland  (2000)       38 2024-05-16 19:53:00.897167 blockmango-1.3.9/setup.cfg
+-rw-------   0 userland  (2000) userland  (2000)      503 2024-05-16 19:52:28.000000 blockmango-1.3.9/setup.py
```

### Comparing `blockmango-1.3.8/LICENSE.md` & `blockmango-1.3.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `blockmango-1.3.8/README.md` & `blockmango-1.3.9/README.md`

 * *Files identical despite different names*

### Comparing `blockmango-1.3.8/blockmango/clan.py` & `blockmango-1.3.9/blockmango/clan.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import requests
+from blockmango.blockmango import constants
 from constants import BASE_URL, BASE_URL_V2, BASE_URL_V3, HEADERS_TEMPLATE
 
 class Clan:
     def __init__(self, user_id, access_token):
         self.headers = {
             **HEADERS_TEMPLATE,
             "userId": user_id,
```

### Comparing `blockmango-1.3.8/blockmango/constants.py` & `blockmango-1.3.9/blockmango/constants.py`

 * *Files identical despite different names*

### Comparing `blockmango-1.3.8/blockmango/decoration.py` & `blockmango-1.3.9/blockmango/decoration.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import requests
+from blockmango.blockmango import constants
 from constants import BASE_URL_DECORATION, BASE_URL_SHOP, BASE_URL_USER, HEADERS_TEMPLATE
 
 class Decoration:
     def __init__(self, user_id, access_token):
         self.headers = {
             **HEADERS_TEMPLATE,
             "userId": user_id,
```

### Comparing `blockmango-1.3.8/blockmango/friends.py` & `blockmango-1.3.9/blockmango/friends.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import requests
+from blockmango.blockmango import constants
 from constants import BASE_URL_FRIEND, BASE_URL_DECORATION, HEADERS_TEMPLATE
 
 class Friends:
     def __init__(self, user_id, access_token):
         self.headers = {
             **HEADERS_TEMPLATE,
             "userId": user_id,
```

### Comparing `blockmango-1.3.8/blockmango/groupchat.py` & `blockmango-1.3.9/blockmango/groupchat.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-import requests
+import request
+from blockmango.blockmango import constants
 from constants import BASE_URL_GROUP, BASE_URL_GROUP_V2, HEADERS_TEMPLATE
 
 class Group:
     def __init__(self, user_id, access_token):
         self.headers = {
             **HEADERS_TEMPLATE,
             "userId": user_id,
```

### Comparing `blockmango-1.3.8/blockmango/user.py` & `blockmango-1.3.9/blockmango/user.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import requests
+from blockmango.blockmango import constants
 from constants import BASE_URL_USER, BASE_URL_ROUTE, HEADERS_TEMPLATE
 
 class User:
     def __init__(self, user_id, access_token):
         self.headers = {
             **HEADERS_TEMPLATE,
             "userId": user_id,
```

