# Comparing `tmp/blockmango-1.1.tar.gz` & `tmp/blockmango-1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blockmango-1.1.tar", last modified: Thu May 16 09:25:19 2024, max compression
+gzip compressed data, was "blockmango-1.3.tar", last modified: Thu May 16 09:56:49 2024, max compression
```

## Comparing `blockmango-1.1.tar` & `blockmango-1.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwx------   0 userland  (2000) userland  (2000)        0 2024-05-16 09:25:19.843710 blockmango-1.1/
--rw-------   0 userland  (2000) userland  (2000)      403 2024-05-16 09:25:19.839709 blockmango-1.1/PKG-INFO
-drwx------   0 userland  (2000) userland  (2000)        0 2024-05-16 09:25:19.819709 blockmango-1.1/blockmango/
--rw-------   0 userland  (2000) userland  (2000)      172 2024-05-16 09:24:00.000000 blockmango-1.1/blockmango/__init__.py
--rw-------   0 userland  (2000) userland  (2000)     7939 2024-05-04 19:42:16.000000 blockmango-1.1/blockmango/clan.py
--rw-------   0 userland  (2000) userland  (2000)     1825 2024-05-16 09:24:50.000000 blockmango-1.1/blockmango/decoration.py
--rw-------   0 userland  (2000) userland  (2000)       35 2024-05-04 19:41:46.000000 blockmango-1.1/blockmango/exceptions.py
--rw-------   0 userland  (2000) userland  (2000)     3791 2024-05-11 09:51:08.000000 blockmango-1.1/blockmango/friends.py
--rw-------   0 userland  (2000) userland  (2000)     4140 2024-05-07 13:28:40.000000 blockmango-1.1/blockmango/groupchat.py
--rw-------   0 userland  (2000) userland  (2000)     3163 2024-05-16 13:21:24.000000 blockmango-1.1/blockmango/user.py
--rw-------   0 userland  (2000) userland  (2000)       87 2024-05-04 19:44:48.000000 blockmango-1.1/blockmango/util.py
-drwx------   0 userland  (2000) userland  (2000)        0 2024-05-16 09:25:19.835709 blockmango-1.1/blockmango.egg-info/
--rw-------   0 userland  (2000) userland  (2000)      403 2024-05-16 09:25:19.000000 blockmango-1.1/blockmango.egg-info/PKG-INFO
--rw-------   0 userland  (2000) userland  (2000)      353 2024-05-16 09:25:19.000000 blockmango-1.1/blockmango.egg-info/SOURCES.txt
--rw-------   0 userland  (2000) userland  (2000)        1 2024-05-16 09:25:19.000000 blockmango-1.1/blockmango.egg-info/dependency_links.txt
--rw-------   0 userland  (2000) userland  (2000)        9 2024-05-16 09:25:19.000000 blockmango-1.1/blockmango.egg-info/requires.txt
--rw-------   0 userland  (2000) userland  (2000)       11 2024-05-16 09:25:19.000000 blockmango-1.1/blockmango.egg-info/top_level.txt
--rw-------   0 userland  (2000) userland  (2000)       38 2024-05-16 09:25:19.843710 blockmango-1.1/setup.cfg
--rw-------   0 userland  (2000) userland  (2000)      501 2024-05-16 09:21:22.000000 blockmango-1.1/setup.py
+drwx------   0 userland  (2000) userland  (2000)        0 2024-05-16 09:56:49.691709 blockmango-1.3/
+-rw-------   0 userland  (2000) userland  (2000)      403 2024-05-16 09:56:49.691709 blockmango-1.3/PKG-INFO
+drwx------   0 userland  (2000) userland  (2000)        0 2024-05-16 09:56:49.679709 blockmango-1.3/blockmango/
+-rw-------   0 userland  (2000) userland  (2000)      172 2024-05-16 09:55:31.000000 blockmango-1.3/blockmango/__init__.py
+-rw-------   0 userland  (2000) userland  (2000)     7939 2024-05-04 19:42:16.000000 blockmango-1.3/blockmango/clan.py
+-rw-------   0 userland  (2000) userland  (2000)     2232 2024-05-16 09:55:55.000000 blockmango-1.3/blockmango/decoration.py
+-rw-------   0 userland  (2000) userland  (2000)       35 2024-05-04 19:41:46.000000 blockmango-1.3/blockmango/exceptions.py
+-rw-------   0 userland  (2000) userland  (2000)     3791 2024-05-11 09:51:08.000000 blockmango-1.3/blockmango/friends.py
+-rw-------   0 userland  (2000) userland  (2000)     4140 2024-05-07 13:28:40.000000 blockmango-1.3/blockmango/groupchat.py
+-rw-------   0 userland  (2000) userland  (2000)     3149 2024-05-16 09:56:25.000000 blockmango-1.3/blockmango/user.py
+-rw-------   0 userland  (2000) userland  (2000)       87 2024-05-04 19:44:48.000000 blockmango-1.3/blockmango/util.py
+drwx------   0 userland  (2000) userland  (2000)        0 2024-05-16 09:56:49.687709 blockmango-1.3/blockmango.egg-info/
+-rw-------   0 userland  (2000) userland  (2000)      403 2024-05-16 09:56:49.000000 blockmango-1.3/blockmango.egg-info/PKG-INFO
+-rw-------   0 userland  (2000) userland  (2000)      353 2024-05-16 09:56:49.000000 blockmango-1.3/blockmango.egg-info/SOURCES.txt
+-rw-------   0 userland  (2000) userland  (2000)        1 2024-05-16 09:56:49.000000 blockmango-1.3/blockmango.egg-info/dependency_links.txt
+-rw-------   0 userland  (2000) userland  (2000)        9 2024-05-16 09:56:49.000000 blockmango-1.3/blockmango.egg-info/requires.txt
+-rw-------   0 userland  (2000) userland  (2000)       11 2024-05-16 09:56:49.000000 blockmango-1.3/blockmango.egg-info/top_level.txt
+-rw-------   0 userland  (2000) userland  (2000)       38 2024-05-16 09:56:49.691709 blockmango-1.3/setup.cfg
+-rw-------   0 userland  (2000) userland  (2000)      501 2024-05-16 09:54:56.000000 blockmango-1.3/setup.py
```

### Comparing `blockmango-1.1/blockmango/clan.py` & `blockmango-1.3/blockmango/clan.py`

 * *Files identical despite different names*

### Comparing `blockmango-1.1/blockmango/decoration.py` & `blockmango-1.3/blockmango/decoration.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,49 +1,49 @@
 import requests
 import json
 
 class Decoration:
-	def __init__(self, user_id, access_token):
-		self.user_id = user_id
-		self.access_token = access_token
-		self.headers = {
-		"userId": user_id,
-		"Access-Token": access_token,
-		"User-Agent": "okhttp/3.12.1"
-		}
-		
-	def see_skins(self, uid):
-		url = f"http://modsgs.sandboxol.com/decoration/api/v1/new/decorations/users/{uid}/classify/all"
-		params = {"engineVersion": "10105",
-		"os": "android", "showVip": 1}
-		response = requests.get(url, headers=self.headers)
-		return self._handle_response(reponse)
-		
-	def current_price(self, skin_id, is_suit):
-		url = "http://modsgs.sandboxol.com/decoration/api/v1/decoration/current/price"
-		json = [{"id":skin_id,"isSuit":is_suit}]
-		response = requests.post(url, json=json, headers=self.headers)
-		return self._handle_response(response)
-		
-	def buy_skin(self, diamond, clothVoucher, paytype):
-		url = "http://modsgs.sandboxol.com/shop/api/v1/new/shop/decorations/buy"
-		params = {"diamond": diamond, "gold": 0, "clothVoucher": clothVoucher, "payType": paytype}
-		response = requests.post(url, headers=self.headers, params=params)
-		return self._handle_response(response)
-	
-	def shop_info(self):
-		url = "http://modsgs.sandboxol.com/user/api/v1/user/shop/info"
-		response = requests.get(url, headers=self.headers)
-		return self._handle_response(response)
-		
-	def equip_skin(self, skinid):
-		url = "http://modsgs.sandboxol.com/decoration/api/v1/decorations/using/new"
-		params = {"ids": skinid}
-		response = requests.post(url, params=params, header=self.headers)
-		return self._handle_response(response)
-		
-		
+        def __init__(self, user_id, access_token):
+                self.user_id = user_id
+                self.access_token = access_token
+                self.headers = {
+                "userId": user_id,
+                "Access-Token": access_token,
+                "User-Agent": "okhttp/3.12.1"
+                }
+
+        def see_skins(self, uid):
+                url = f"http://modsgs.sandboxol.com/decoration/api/v1/new/decorations/users/{uid}/classify/all"
+                params = {"engineVersion": "10105",
+                "os": "android", "showVip": 1}
+                response = requests.get(url, headers=self.headers)
+                return self._handle_response(reponse)
+
+        def current_price(self, skin_id, is_suit):
+                url = "http://modsgs.sandboxol.com/decoration/api/v1/decoration/current/price"
+                json = [{"id":skin_id,"isSuit":is_suit}]
+                response = requests.post(url, json=json, headers=self.headers)
+                return self._handle_response(response)
+
+        def buy_skin(self, diamond, clothVoucher, paytype):
+                url = "http://modsgs.sandboxol.com/shop/api/v1/new/shop/decorations/buy"
+                params = {"diamond": diamond, "gold": 0, "clothVoucher": clothVoucher, "payType": paytype}
+                response = requests.post(url, headers=self.headers, params=params)
+                return self._handle_response(response)
+
+        def shop_info(self):
+                url = "http://modsgs.sandboxol.com/user/api/v1/user/shop/info"
+                response = requests.get(url, headers=self.headers)
+                return self._handle_response(response)
+
+        def equip_skin(self, skinid):
+                url = "http://modsgs.sandboxol.com/decoration/api/v1/decorations/using/new"
+                params = {"ids": skinid}
+                response = requests.post(url, params=params, header=self.headers)
+                return self._handle_response(response)
+
+
     def _handle_response(self, response):
         if response.status_code == 200:
             return response.json()
         else:
             return {"Error": f"Failed to perform action. Status code: {response.status_code}"}
```

### Comparing `blockmango-1.1/blockmango/friends.py` & `blockmango-1.3/blockmango/friends.py`

 * *Files identical despite different names*

### Comparing `blockmango-1.1/blockmango/groupchat.py` & `blockmango-1.3/blockmango/groupchat.py`

 * *Files identical despite different names*

### Comparing `blockmango-1.1/blockmango/user.py` & `blockmango-1.3/blockmango/user.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,14 +63,12 @@
     	
     def unbind_email(self, verifyCode, email):
     	url = f"http://modsgs.sandboxol.com/user/api/v2/users/{self.user_id}/emails"
     	params = {"email": email, "verifyCode": verifyCode}
     	response = requests.delete(url, params=params, headers=self.headers)
     	return self._handle_response(response)
     	
-    def 
-    	
     def _handle_response(self, response):
         if response.status_code == 200:
             return response.json()
         else:
-            return {"Error": f"Failed to perform action. Status code: {response.status_code}"}
+            return {"Error": f"Failed to perform action. Status code: {response.status_code}"}
```

