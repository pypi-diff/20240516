# Comparing `tmp/blockmango-1.3.4.tar.gz` & `tmp/blockmango-1.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blockmango-1.3.4.tar", last modified: Thu May 16 12:17:25 2024, max compression
+gzip compressed data, was "blockmango-1.3.5.tar", last modified: Thu May 16 14:21:47 2024, max compression
```

## Comparing `blockmango-1.3.4.tar` & `blockmango-1.3.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwx------   0 userland  (2000) userland  (2000)        0 2024-05-16 12:17:25.632010 blockmango-1.3.4/
--rw-------   0 userland  (2000) userland  (2000)      405 2024-05-16 12:17:25.632010 blockmango-1.3.4/PKG-INFO
-drwx------   0 userland  (2000) userland  (2000)        0 2024-05-16 12:17:25.616010 blockmango-1.3.4/blockmango/
--rw-------   0 userland  (2000) userland  (2000)      172 2024-05-16 12:14:22.000000 blockmango-1.3.4/blockmango/__init__.py
--rw-------   0 userland  (2000) userland  (2000)     7939 2024-05-16 12:14:22.000000 blockmango-1.3.4/blockmango/clan.py
--rw-------   0 userland  (2000) userland  (2000)     2096 2024-05-16 12:14:22.000000 blockmango-1.3.4/blockmango/decoration.py
--rw-------   0 userland  (2000) userland  (2000)       35 2024-05-16 12:14:22.000000 blockmango-1.3.4/blockmango/exceptions.py
--rw-------   0 userland  (2000) userland  (2000)     3791 2024-05-16 12:14:22.000000 blockmango-1.3.4/blockmango/friends.py
--rw-------   0 userland  (2000) userland  (2000)     4140 2024-05-16 12:14:22.000000 blockmango-1.3.4/blockmango/groupchat.py
--rw-------   0 userland  (2000) userland  (2000)     3342 2024-05-16 12:16:29.000000 blockmango-1.3.4/blockmango/user.py
--rw-------   0 userland  (2000) userland  (2000)       87 2024-05-16 12:14:22.000000 blockmango-1.3.4/blockmango/util.py
-drwx------   0 userland  (2000) userland  (2000)        0 2024-05-16 12:17:25.628010 blockmango-1.3.4/blockmango.egg-info/
--rw-------   0 userland  (2000) userland  (2000)      405 2024-05-16 12:17:25.000000 blockmango-1.3.4/blockmango.egg-info/PKG-INFO
--rw-------   0 userland  (2000) userland  (2000)      353 2024-05-16 12:17:25.000000 blockmango-1.3.4/blockmango.egg-info/SOURCES.txt
--rw-------   0 userland  (2000) userland  (2000)        1 2024-05-16 12:17:25.000000 blockmango-1.3.4/blockmango.egg-info/dependency_links.txt
--rw-------   0 userland  (2000) userland  (2000)        9 2024-05-16 12:17:25.000000 blockmango-1.3.4/blockmango.egg-info/requires.txt
--rw-------   0 userland  (2000) userland  (2000)       11 2024-05-16 12:17:25.000000 blockmango-1.3.4/blockmango.egg-info/top_level.txt
--rw-------   0 userland  (2000) userland  (2000)       38 2024-05-16 12:17:25.632010 blockmango-1.3.4/setup.cfg
--rw-------   0 userland  (2000) userland  (2000)      503 2024-05-16 12:17:11.000000 blockmango-1.3.4/setup.py
+drwx------   0 userland  (2000) userland  (2000)        0 2024-05-16 14:21:47.430547 blockmango-1.3.5/
+-rw-------   0 userland  (2000) userland  (2000)      405 2024-05-16 14:21:47.426547 blockmango-1.3.5/PKG-INFO
+drwx------   0 userland  (2000) userland  (2000)        0 2024-05-16 14:21:47.390547 blockmango-1.3.5/blockmango/
+-rw-------   0 userland  (2000) userland  (2000)      172 2024-05-16 14:19:38.000000 blockmango-1.3.5/blockmango/__init__.py
+-rw-------   0 userland  (2000) userland  (2000)     7939 2024-05-16 14:19:38.000000 blockmango-1.3.5/blockmango/clan.py
+-rw-------   0 userland  (2000) userland  (2000)     2096 2024-05-16 14:19:38.000000 blockmango-1.3.5/blockmango/decoration.py
+-rw-------   0 userland  (2000) userland  (2000)       35 2024-05-16 14:19:38.000000 blockmango-1.3.5/blockmango/exceptions.py
+-rw-------   0 userland  (2000) userland  (2000)     3791 2024-05-16 14:19:38.000000 blockmango-1.3.5/blockmango/friends.py
+-rw-------   0 userland  (2000) userland  (2000)     4140 2024-05-16 14:19:38.000000 blockmango-1.3.5/blockmango/groupchat.py
+-rw-------   0 userland  (2000) userland  (2000)     3194 2024-05-16 14:20:28.000000 blockmango-1.3.5/blockmango/user.py
+-rw-------   0 userland  (2000) userland  (2000)       87 2024-05-16 14:19:38.000000 blockmango-1.3.5/blockmango/util.py
+drwx------   0 userland  (2000) userland  (2000)        0 2024-05-16 14:21:47.422547 blockmango-1.3.5/blockmango.egg-info/
+-rw-------   0 userland  (2000) userland  (2000)      405 2024-05-16 14:21:45.000000 blockmango-1.3.5/blockmango.egg-info/PKG-INFO
+-rw-------   0 userland  (2000) userland  (2000)      353 2024-05-16 14:21:46.000000 blockmango-1.3.5/blockmango.egg-info/SOURCES.txt
+-rw-------   0 userland  (2000) userland  (2000)        1 2024-05-16 14:21:45.000000 blockmango-1.3.5/blockmango.egg-info/dependency_links.txt
+-rw-------   0 userland  (2000) userland  (2000)        9 2024-05-16 14:21:45.000000 blockmango-1.3.5/blockmango.egg-info/requires.txt
+-rw-------   0 userland  (2000) userland  (2000)       11 2024-05-16 14:21:45.000000 blockmango-1.3.5/blockmango.egg-info/top_level.txt
+-rw-------   0 userland  (2000) userland  (2000)       38 2024-05-16 14:21:47.430547 blockmango-1.3.5/setup.cfg
+-rw-------   0 userland  (2000) userland  (2000)      503 2024-05-16 14:21:29.000000 blockmango-1.3.5/setup.py
```

### Comparing `blockmango-1.3.4/blockmango/clan.py` & `blockmango-1.3.5/blockmango/clan.py`

 * *Files identical despite different names*

### Comparing `blockmango-1.3.4/blockmango/decoration.py` & `blockmango-1.3.5/blockmango/decoration.py`

 * *Files identical despite different names*

### Comparing `blockmango-1.3.4/blockmango/friends.py` & `blockmango-1.3.5/blockmango/friends.py`

 * *Files identical despite different names*

### Comparing `blockmango-1.3.4/blockmango/groupchat.py` & `blockmango-1.3.5/blockmango/groupchat.py`

 * *Files identical despite different names*

### Comparing `blockmango-1.3.4/blockmango/user.py` & `blockmango-1.3.5/blockmango/user.py`

 * *Files 18% similar despite different names*

```diff
@@ -12,65 +12,63 @@
         }
 
     def get_user_info(self):
         url = "http://modsgs.sandboxol.com/user/api/v2/user/details/info"
         response = requests.get(url, headers=self.headers)
         return self._handle_response(response)
         
-    def set_birthday(self, birthday):
-        url = "http://modsgs.sandboxol.com/user/api/v1/user/info"
-        payload = {"birthday": birthday}
-        response = requests.put(url, json=payload, headers=self.headers)
-        return self._handle_response(response)
-        
-    def login(self, device_id, device_sign, password, user_id):
-        url = "http://route.sandboxol.com/user/api/v1/app/login"
-        headers = self.headers.copy()
-        headers["bmg-device-id"] = device_id
-        headers["bmg-sign"] = device_sign
-        payload = {"password": password, "uid": user_id}
-        response = requests.post(url, headers=headers, json=payload)
-        return self._handle_response(response)
-        
+    def birthday(self, birthday):
+    	url = "http://modsgs.sandboxol.com/user/api/v1/user/info"
+    	json = {"birthday": birthday}
+    	response = requests.put(url, json=json, headers = self.headers)
+    	return self._handle_response(response)
+    	
+    def login(self, device_id, device_sign, password, userId):
+    	url = "http://route.sandboxol.com/user/api/v1/app/login"
+    	headers = {"userId": self.user_id, "Access-Token": self.access_token, "User-Agent": "okhttp/3.12.1", "bmg-sign": device_sign, "bmg-device-id": device_id}
+    	
+    	json = {"password": password, "uid": userId}
+    	response = requests.post(url, headers=headers, json=json)
+    	return self._handle_response(response)
+    	
     def change_name(self, new_name):
-        url = "http://modsgs.sandboxol.com/user/api/v3/user/nickName"
-        params = {"newName": new_name, "oldName": "darkk.py"}
-        response = requests.put(url, headers=self.headers, params=params)
-        return self._handle_response(response)
-        
+    	url = "http://modsgs.sandboxol.com/user/api/v3/user/nickName"
+    	params = {"newName": new_name, "oldName": "darkk.py"}
+    	response = requests.put(url, headers=self.headers, params=params)
+    	return self._handle_response(response)
+    	
     def change_details(self, new_details):
-        url = "http://modsgs.sandboxol.com/user/api/v1/user/info"
-        payload = {"details": new_details}
-        response = requests.put(url, headers=self.headers, json=payload)
-        return self._handle_response(response)
-        
+    	url = "http://modsgs.sandboxol.com/user/api/v1/user/info"
+    	json = {"details": new_details}
+    	response = requests.put(url, headers=self.headers, json=json)
+    	return self._handle_response(response)
+    	
     def change_pfp(self, pfp_url):
-        url = "http://modsgs.sandboxol.com/user/api/v1/user/info"
-        payload = {"picUrl": pfp_url}
-        response = requests.put(url, json=payload, headers=self.headers)
-        return self._handle_response(response)
+    	url = "http://modsgs.sandboxol.com/user/api/v1/user/info"
+    	json = {"picUrl": pfp_url}
+    	response = requests.put(url, json=json, headers=self.headers)
+    	return self._handle_response(response)
     
-    def modify_password(self, old_password, new_password):
-        url = "http://modsgs.sandboxol.com/user/api/v1/user/password/modify"
-        payload = {"confirmPassword": "", "newPassword": new_password, "oldPassword": old_password}
-        response = requests.post(url, json=payload, headers=self.headers)
-        return self._handle_response(response)
-        
-    def bind_email(self, email, verify_code):
-        url = "http://modsgs.sandboxol.com/user/api/v1/users/bind/email"
-        payload = {"email": email, "verifyCode": verify_code}
-        response = requests.post(url, json=payload, headers=self.headers)
-        return self._handle_response(response)
-        
-    def unbind_email(self, verify_code, email):
-        url = f"http://modsgs.sandboxol.com/user/api/v2/users/{self.user_id}/emails"
-        params = {"email": email, "verifyCode": verify_code}
-        response = requests.delete(url, params=params, headers=self.headers)
-        return self._handle_response(response)
-        
+    def modify_password(self, oldPassword, newPassword):
+    	url = "http://modsgs.sandboxol.com/user/api/v1/user/password/modify"
+    	json = {"confirmPassword": "", "newPassword": newPassword, "oldPassword": oldPassword}
+    	response = requests.post(url, json=json, headers=self.headers)
+    	return self._handle_response(response)
+    	
+    def bind_email(self, email, verifyCode):
+    	url = "http://modsgs.sandboxol.com/user/api/v1/users/bind/email"
+    	json = {"email": email, "verifyCode": verifyCode}
+    	response = requests.post(url, json=json, headers=self.headers)
+    	return self._handle_response(response)
+    	
+    def unbind_email(self, verifyCode, email):
+    	url = f"http://modsgs.sandboxol.com/user/api/v2/users/{self.user_id}/emails"
+    	params = {"email": email, "verifyCode": verifyCode}
+    	response = requests.delete(url, params=params, headers=self.headers)
+    	return self._handle_response(response)
+    	
+    	
     def _handle_response(self, response):
         if response.status_code == 200:
             return response.json()
         else:
-            return {"Error": f"Failed to perform action. Status code: {response.status_code}, Response: {response.text}"}
-
-
+            return {"Error": f"Failed to perform action. Status code: {response.status_code}"}
```

