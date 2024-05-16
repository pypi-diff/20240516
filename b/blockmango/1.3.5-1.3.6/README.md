# Comparing `tmp/blockmango-1.3.5.tar.gz` & `tmp/blockmango-1.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blockmango-1.3.5.tar", last modified: Thu May 16 14:21:47 2024, max compression
+gzip compressed data, was "blockmango-1.3.6.tar", last modified: Thu May 16 17:23:55 2024, max compression
```

## Comparing `blockmango-1.3.5.tar` & `blockmango-1.3.6.tar`

### file list

```diff
@@ -1,19 +1,17 @@
-drwx------   0 userland  (2000) userland  (2000)        0 2024-05-16 14:21:47.430547 blockmango-1.3.5/
--rw-------   0 userland  (2000) userland  (2000)      405 2024-05-16 14:21:47.426547 blockmango-1.3.5/PKG-INFO
-drwx------   0 userland  (2000) userland  (2000)        0 2024-05-16 14:21:47.390547 blockmango-1.3.5/blockmango/
--rw-------   0 userland  (2000) userland  (2000)      172 2024-05-16 14:19:38.000000 blockmango-1.3.5/blockmango/__init__.py
--rw-------   0 userland  (2000) userland  (2000)     7939 2024-05-16 14:19:38.000000 blockmango-1.3.5/blockmango/clan.py
--rw-------   0 userland  (2000) userland  (2000)     2096 2024-05-16 14:19:38.000000 blockmango-1.3.5/blockmango/decoration.py
--rw-------   0 userland  (2000) userland  (2000)       35 2024-05-16 14:19:38.000000 blockmango-1.3.5/blockmango/exceptions.py
--rw-------   0 userland  (2000) userland  (2000)     3791 2024-05-16 14:19:38.000000 blockmango-1.3.5/blockmango/friends.py
--rw-------   0 userland  (2000) userland  (2000)     4140 2024-05-16 14:19:38.000000 blockmango-1.3.5/blockmango/groupchat.py
--rw-------   0 userland  (2000) userland  (2000)     3194 2024-05-16 14:20:28.000000 blockmango-1.3.5/blockmango/user.py
--rw-------   0 userland  (2000) userland  (2000)       87 2024-05-16 14:19:38.000000 blockmango-1.3.5/blockmango/util.py
-drwx------   0 userland  (2000) userland  (2000)        0 2024-05-16 14:21:47.422547 blockmango-1.3.5/blockmango.egg-info/
--rw-------   0 userland  (2000) userland  (2000)      405 2024-05-16 14:21:45.000000 blockmango-1.3.5/blockmango.egg-info/PKG-INFO
--rw-------   0 userland  (2000) userland  (2000)      353 2024-05-16 14:21:46.000000 blockmango-1.3.5/blockmango.egg-info/SOURCES.txt
--rw-------   0 userland  (2000) userland  (2000)        1 2024-05-16 14:21:45.000000 blockmango-1.3.5/blockmango.egg-info/dependency_links.txt
--rw-------   0 userland  (2000) userland  (2000)        9 2024-05-16 14:21:45.000000 blockmango-1.3.5/blockmango.egg-info/requires.txt
--rw-------   0 userland  (2000) userland  (2000)       11 2024-05-16 14:21:45.000000 blockmango-1.3.5/blockmango.egg-info/top_level.txt
--rw-------   0 userland  (2000) userland  (2000)       38 2024-05-16 14:21:47.430547 blockmango-1.3.5/setup.cfg
--rw-------   0 userland  (2000) userland  (2000)      503 2024-05-16 14:21:29.000000 blockmango-1.3.5/setup.py
+drwx------   0 userland  (2000) userland  (2000)        0 2024-05-16 17:23:55.330543 blockmango-1.3.6/
+-rw-------   0 userland  (2000) userland  (2000)      405 2024-05-16 17:23:55.330543 blockmango-1.3.6/PKG-INFO
+drwx------   0 userland  (2000) userland  (2000)        0 2024-05-16 17:23:55.310543 blockmango-1.3.6/blockmango/
+-rw-------   0 userland  (2000) userland  (2000)      172 2024-05-16 17:13:23.000000 blockmango-1.3.6/blockmango/__init__.py
+-rw-------   0 userland  (2000) userland  (2000)     7880 2024-05-16 17:15:07.000000 blockmango-1.3.6/blockmango/clan.py
+-rw-------   0 userland  (2000) userland  (2000)     2009 2024-05-16 17:16:06.000000 blockmango-1.3.6/blockmango/decoration.py
+-rw-------   0 userland  (2000) userland  (2000)     3697 2024-05-16 17:18:28.000000 blockmango-1.3.6/blockmango/friends.py
+-rw-------   0 userland  (2000) userland  (2000)     4047 2024-05-16 17:19:20.000000 blockmango-1.3.6/blockmango/groupchat.py
+-rw-------   0 userland  (2000) userland  (2000)     3295 2024-05-16 17:21:42.000000 blockmango-1.3.6/blockmango/user.py
+drwx------   0 userland  (2000) userland  (2000)        0 2024-05-16 17:23:55.326543 blockmango-1.3.6/blockmango.egg-info/
+-rw-------   0 userland  (2000) userland  (2000)      405 2024-05-16 17:23:54.000000 blockmango-1.3.6/blockmango.egg-info/PKG-INFO
+-rw-------   0 userland  (2000) userland  (2000)      309 2024-05-16 17:23:54.000000 blockmango-1.3.6/blockmango.egg-info/SOURCES.txt
+-rw-------   0 userland  (2000) userland  (2000)        1 2024-05-16 17:23:54.000000 blockmango-1.3.6/blockmango.egg-info/dependency_links.txt
+-rw-------   0 userland  (2000) userland  (2000)        9 2024-05-16 17:23:54.000000 blockmango-1.3.6/blockmango.egg-info/requires.txt
+-rw-------   0 userland  (2000) userland  (2000)       11 2024-05-16 17:23:54.000000 blockmango-1.3.6/blockmango.egg-info/top_level.txt
+-rw-------   0 userland  (2000) userland  (2000)       38 2024-05-16 17:23:55.330543 blockmango-1.3.6/setup.cfg
+-rw-------   0 userland  (2000) userland  (2000)      503 2024-05-16 17:23:18.000000 blockmango-1.3.6/setup.py
```

### Comparing `blockmango-1.3.5/blockmango/clan.py` & `blockmango-1.3.6/blockmango/clan.py`

 * *Files 1% similar despite different names*

```diff
@@ -171,8 +171,8 @@
         response = requests.delete(url, headers=self.headers)
         return self._handle_response(response)
 
     def _handle_response(self, response):
         if response.status_code == 200:
             return response.json()
         else:
-            return {"Error": f"Failed to perform action. Status code: {response.status_code}"}
+            return response.json()
```

### Comparing `blockmango-1.3.5/blockmango/decoration.py` & `blockmango-1.3.6/blockmango/decoration.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,8 +40,8 @@
         response = requests.post(url, headers=self.headers, params=params)
         return self._handle_response(response)
         
     def _handle_response(self, response):
         if response.status_code == 200:
             return response.json()
         else:
-            return {"Error": f"Failed to perform action. Status code: {response.status_code}. Response: {response.text}"}
+            return response.json()
```

### Comparing `blockmango-1.3.5/blockmango/friends.py` & `blockmango-1.3.6/blockmango/friends.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,8 +82,8 @@
 
     def friend_reject(self, friend_id):
     	url = "http://modsgs.sandboxol.com/friend/api/v1/friends/{friend_id}/rejection"
     	response = requests.put(url, headers=self.headers)
     	return self._handle_response(response)
     	
     def _handle_response(self, response):
-        return response.json() if response.status_code == 200 else {"Error": f"Failed. Status code: {response.status_code}"}
+        return response.json()
```

### Comparing `blockmango-1.3.5/blockmango/groupchat.py` & `blockmango-1.3.6/blockmango/groupchat.py`

 * *Files 8% similar despite different names*

```diff
@@ -59,8 +59,8 @@
         
     def group_owner(self, group_id, new_owner):
         url = "http://modsgs.sandboxol.com/msg/api/v1/msg/group/chat/transfer"
         response = requests.put(url, headers=self.headers, json={"groupId": group_id, "inviterId": self.user_id, "userId": new_owner})
         return self._handle_response(response)
 
     def _handle_response(self, response):
-        return response.json() if response.status_code == 200 else {"Error": f"Failed. Status code: {response.status_code}"}
+        return response.json()
```

### Comparing `blockmango-1.3.5/blockmango/user.py` & `blockmango-1.3.6/blockmango/user.py`

 * *Files 9% similar despite different names*

```diff
@@ -66,9 +66,9 @@
     	response = requests.delete(url, params=params, headers=self.headers)
     	return self._handle_response(response)
     	
     	
     def _handle_response(self, response):
         if response.status_code == 200:
             return response.json()
-        else:
-            return {"Error": f"Failed to perform action. Status code: {response.status_code}"}
+        else: #i am programming in terminal right now, this if-else statement might be useless, but my terminal doesn't gives me indentations so its hard to fix it. im sorry
+            return response.json()
```

