# Comparing `tmp/blockmango-1.3.tar.gz` & `tmp/blockmango-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blockmango-1.3.tar", last modified: Thu May 16 09:56:49 2024, max compression
+gzip compressed data, was "blockmango-1.3.1.tar", last modified: Thu May 16 10:13:01 2024, max compression
```

## Comparing `blockmango-1.3.tar` & `blockmango-1.3.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwx------   0 userland  (2000) userland  (2000)        0 2024-05-16 09:56:49.691709 blockmango-1.3/
--rw-------   0 userland  (2000) userland  (2000)      403 2024-05-16 09:56:49.691709 blockmango-1.3/PKG-INFO
-drwx------   0 userland  (2000) userland  (2000)        0 2024-05-16 09:56:49.679709 blockmango-1.3/blockmango/
--rw-------   0 userland  (2000) userland  (2000)      172 2024-05-16 09:55:31.000000 blockmango-1.3/blockmango/__init__.py
--rw-------   0 userland  (2000) userland  (2000)     7939 2024-05-04 19:42:16.000000 blockmango-1.3/blockmango/clan.py
--rw-------   0 userland  (2000) userland  (2000)     2232 2024-05-16 09:55:55.000000 blockmango-1.3/blockmango/decoration.py
--rw-------   0 userland  (2000) userland  (2000)       35 2024-05-04 19:41:46.000000 blockmango-1.3/blockmango/exceptions.py
--rw-------   0 userland  (2000) userland  (2000)     3791 2024-05-11 09:51:08.000000 blockmango-1.3/blockmango/friends.py
--rw-------   0 userland  (2000) userland  (2000)     4140 2024-05-07 13:28:40.000000 blockmango-1.3/blockmango/groupchat.py
--rw-------   0 userland  (2000) userland  (2000)     3149 2024-05-16 09:56:25.000000 blockmango-1.3/blockmango/user.py
--rw-------   0 userland  (2000) userland  (2000)       87 2024-05-04 19:44:48.000000 blockmango-1.3/blockmango/util.py
-drwx------   0 userland  (2000) userland  (2000)        0 2024-05-16 09:56:49.687709 blockmango-1.3/blockmango.egg-info/
--rw-------   0 userland  (2000) userland  (2000)      403 2024-05-16 09:56:49.000000 blockmango-1.3/blockmango.egg-info/PKG-INFO
--rw-------   0 userland  (2000) userland  (2000)      353 2024-05-16 09:56:49.000000 blockmango-1.3/blockmango.egg-info/SOURCES.txt
--rw-------   0 userland  (2000) userland  (2000)        1 2024-05-16 09:56:49.000000 blockmango-1.3/blockmango.egg-info/dependency_links.txt
--rw-------   0 userland  (2000) userland  (2000)        9 2024-05-16 09:56:49.000000 blockmango-1.3/blockmango.egg-info/requires.txt
--rw-------   0 userland  (2000) userland  (2000)       11 2024-05-16 09:56:49.000000 blockmango-1.3/blockmango.egg-info/top_level.txt
--rw-------   0 userland  (2000) userland  (2000)       38 2024-05-16 09:56:49.691709 blockmango-1.3/setup.cfg
--rw-------   0 userland  (2000) userland  (2000)      501 2024-05-16 09:54:56.000000 blockmango-1.3/setup.py
+drwx------   0 userland  (2000) userland  (2000)        0 2024-05-16 10:13:01.095708 blockmango-1.3.1/
+-rw-------   0 userland  (2000) userland  (2000)      405 2024-05-16 10:13:01.091708 blockmango-1.3.1/PKG-INFO
+drwx------   0 userland  (2000) userland  (2000)        0 2024-05-16 10:13:01.071708 blockmango-1.3.1/blockmango/
+-rw-------   0 userland  (2000) userland  (2000)      172 2024-05-16 10:11:34.000000 blockmango-1.3.1/blockmango/__init__.py
+-rw-------   0 userland  (2000) userland  (2000)     7939 2024-05-04 19:42:16.000000 blockmango-1.3.1/blockmango/clan.py
+-rw-------   0 userland  (2000) userland  (2000)      550 2024-05-12 10:44:16.000000 blockmango-1.3.1/blockmango/decoration.py
+-rw-------   0 userland  (2000) userland  (2000)       35 2024-05-04 19:41:46.000000 blockmango-1.3.1/blockmango/exceptions.py
+-rw-------   0 userland  (2000) userland  (2000)     3791 2024-05-11 09:51:08.000000 blockmango-1.3.1/blockmango/friends.py
+-rw-------   0 userland  (2000) userland  (2000)     4140 2024-05-07 13:28:40.000000 blockmango-1.3.1/blockmango/groupchat.py
+-rw-------   0 userland  (2000) userland  (2000)     3155 2024-05-16 10:11:53.000000 blockmango-1.3.1/blockmango/user.py
+-rw-------   0 userland  (2000) userland  (2000)       87 2024-05-04 19:44:48.000000 blockmango-1.3.1/blockmango/util.py
+drwx------   0 userland  (2000) userland  (2000)        0 2024-05-16 10:13:01.087708 blockmango-1.3.1/blockmango.egg-info/
+-rw-------   0 userland  (2000) userland  (2000)      405 2024-05-16 10:13:00.000000 blockmango-1.3.1/blockmango.egg-info/PKG-INFO
+-rw-------   0 userland  (2000) userland  (2000)      353 2024-05-16 10:13:00.000000 blockmango-1.3.1/blockmango.egg-info/SOURCES.txt
+-rw-------   0 userland  (2000) userland  (2000)        1 2024-05-16 10:13:00.000000 blockmango-1.3.1/blockmango.egg-info/dependency_links.txt
+-rw-------   0 userland  (2000) userland  (2000)        9 2024-05-16 10:13:00.000000 blockmango-1.3.1/blockmango.egg-info/requires.txt
+-rw-------   0 userland  (2000) userland  (2000)       11 2024-05-16 10:13:00.000000 blockmango-1.3.1/blockmango.egg-info/top_level.txt
+-rw-------   0 userland  (2000) userland  (2000)       38 2024-05-16 10:13:01.095708 blockmango-1.3.1/setup.cfg
+-rw-------   0 userland  (2000) userland  (2000)      503 2024-05-16 10:11:01.000000 blockmango-1.3.1/setup.py
```

### Comparing `blockmango-1.3/blockmango/clan.py` & `blockmango-1.3.1/blockmango/clan.py`

 * *Files identical despite different names*

### Comparing `blockmango-1.3/blockmango/friends.py` & `blockmango-1.3.1/blockmango/friends.py`

 * *Files identical despite different names*

### Comparing `blockmango-1.3/blockmango/groupchat.py` & `blockmango-1.3.1/blockmango/groupchat.py`

 * *Files identical despite different names*

### Comparing `blockmango-1.3/blockmango/user.py` & `blockmango-1.3.1/blockmango/user.py`

 * *Files 0% similar despite different names*

```diff
@@ -63,12 +63,13 @@
     	
     def unbind_email(self, verifyCode, email):
     	url = f"http://modsgs.sandboxol.com/user/api/v2/users/{self.user_id}/emails"
     	params = {"email": email, "verifyCode": verifyCode}
     	response = requests.delete(url, params=params, headers=self.headers)
     	return self._handle_response(response)
     	
+    	
     def _handle_response(self, response):
         if response.status_code == 200:
             return response.json()
         else:
             return {"Error": f"Failed to perform action. Status code: {response.status_code}"}
```

