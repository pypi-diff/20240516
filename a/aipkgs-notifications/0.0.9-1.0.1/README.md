# Comparing `tmp/aipkgs_notifications-0.0.9.tar.gz` & `tmp/aipkgs_notifications-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aipkgs_notifications-0.0.9.tar", max compression
+gzip compressed data, was "aipkgs_notifications-1.0.1.tar", max compression
```

## Comparing `aipkgs_notifications-0.0.9.tar` & `aipkgs_notifications-1.0.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1058 2023-11-05 00:26:39.099971 aipkgs_notifications-0.0.9/LICENSE.md
--rw-r--r--   0        0        0     3071 2023-11-04 16:54:51.776217 aipkgs_notifications-0.0.9/README.md
--rw-r--r--   0        0        0       53 2023-11-05 00:35:11.631721 aipkgs_notifications-0.0.9/aipkgs_notifications/__init__.py
--rw-r--r--   0        0        0     7850 2023-11-25 23:02:32.927245 aipkgs_notifications-0.0.9/aipkgs_notifications/apns.py
--rw-r--r--   0        0        0      946 2023-11-25 23:01:16.403609 aipkgs_notifications-0.0.9/aipkgs_notifications/enums.py
--rw-r--r--   0        0        0     5267 2023-11-25 18:31:41.602633 aipkgs_notifications-0.0.9/aipkgs_notifications/payload.py
--rw-r--r--   0        0        0     2119 2023-11-25 19:06:29.100282 aipkgs_notifications-0.0.9/aipkgs_notifications/response.py
--rw-r--r--   0        0        0      976 2023-11-02 20:50:24.863627 aipkgs_notifications-0.0.9/aipkgs_notifications/singleton.py
--rw-r--r--   0        0        0      122 2023-11-04 15:34:02.233847 aipkgs_notifications-0.0.9/aipkgs_notifications/utils.py
--rw-r--r--   0        0        0      547 2023-11-25 23:24:03.819457 aipkgs_notifications-0.0.9/pyproject.toml
--rw-r--r--   0        0        0     3801 1970-01-01 00:00:00.000000 aipkgs_notifications-0.0.9/PKG-INFO
+-rw-r--r--   0        0        0     1058 2023-11-05 00:26:39.099971 aipkgs_notifications-1.0.1/LICENSE.md
+-rw-r--r--   0        0        0     3070 2023-12-11 22:43:30.104335 aipkgs_notifications-1.0.1/README.md
+-rw-r--r--   0        0        0       51 2023-12-11 21:30:41.390034 aipkgs_notifications-1.0.1/aipkgs_notifications/__init__.py
+-rw-r--r--   0        0        0      946 2023-11-25 23:01:16.403609 aipkgs_notifications-1.0.1/aipkgs_notifications/enums.py
+-rw-r--r--   0        0        0     9396 2024-01-11 14:01:48.030045 aipkgs_notifications-1.0.1/aipkgs_notifications/ns.py
+-rw-r--r--   0        0        0     5272 2024-01-23 17:29:09.843114 aipkgs_notifications-1.0.1/aipkgs_notifications/payload.py
+-rw-r--r--   0        0        0     2122 2023-11-25 23:31:13.326810 aipkgs_notifications-1.0.1/aipkgs_notifications/response.py
+-rw-r--r--   0        0        0      976 2023-11-02 20:50:24.863627 aipkgs_notifications-1.0.1/aipkgs_notifications/singleton.py
+-rw-r--r--   0        0        0      122 2023-11-04 15:34:02.233847 aipkgs_notifications-1.0.1/aipkgs_notifications/utils.py
+-rw-r--r--   0        0        0      662 2024-05-15 22:16:16.599556 aipkgs_notifications-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     3837 1970-01-01 00:00:00.000000 aipkgs_notifications-1.0.1/PKG-INFO
```

### Comparing `aipkgs_notifications-0.0.9/LICENSE.md` & `aipkgs_notifications-1.0.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `aipkgs_notifications-0.0.9/README.md` & `aipkgs_notifications-1.0.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -13,33 +13,33 @@
 ```python
 import apns
 ```
 
 Then, initialize the APNS with your application's details:
 
 ```python
-KEY_ID = ''  
-TEAM_ID = ''  
+KEY_ID = ''
+TEAM_ID = ''
 BUNDLE_ID = 'com.test.app'
 IS_PROD = False
-P8_KEY_PATH = 'path/to/p8/key'  
+P8_KEY_PATH = 'path/to/p8/key'
 PEM_FILE_PATH = 'path/to/pem/file'
 APNS_PRIORITY = 10
 APNS_EXPIRATION = 0
 
 apns.initialize_apns(key_id=KEY_ID,
                      team_id=TEAM_ID,
                      bundle_id=BUNDLE_ID,
                      is_prod=IS_PROD,
                      p8_key_path=P8_KEY_PATH,
                      pem_file_path=PEM_FILE_PATH,
                      apns_priority=APNS_PRIORITY,
                      apns_expiration=APNS_EXPIRATION)
 
-apns.config().verbose = True
+apns.apns_config().verbose = True
 ```
 
 Now, you can send a push notification:
 
 ```python
 device_token = ""  
 data = {}
```

### Comparing `aipkgs_notifications-0.0.9/aipkgs_notifications/apns.py` & `aipkgs_notifications-1.0.1/aipkgs_notifications/ns.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 import json
 import time
 import uuid
+from typing import Optional
+
+import firebase_admin
 import httpx
 import jwt
 import aipkgs_notifications.singleton as singleton
 import aipkgs_notifications.utils as utils
 import aipkgs_notifications.response as ai_response
 import aipkgs_notifications.payload as ai_payload
 import aipkgs_notifications.enums as enums
@@ -20,14 +23,15 @@
 
 
 @singleton.Singleton
 class APNS:
     def __init__(self, key_id: str = '', team_id: str = '', bundle_id: str = '', is_prod: bool = None, p8_key_path: str = '', pem_file_path: str = '', apns_priority: int = None,
                  apns_expiration: int = None):
         self.config = Config()
+        self.config.verbose = True
 
         self.ALGORITHM = 'ES256'
         self.KEY_ID = key_id
         self.TEAM_ID = team_id
         self.BUNDLE_ID = bundle_id
         self.IS_PROD = is_prod
         self.AUTH_P8_KEY = p8_key_path
@@ -159,25 +163,25 @@
                 headers=headers,
                 json=payload.to_dict(),
             )
 
         apns_response = ai_response.APNSResponse(httpx_response=response)
 
         if self.config.verbose:
-            print(f"is_sent: {apns_response.is_sent()}")
+            print(f"is_success: {apns_response.is_success}")
             print(f"status_code: {apns_response.status_code}")
             print(f"apns_id: {apns_response.apns_id}")
             print(f"apns_unique_id:  {apns_response.apns_unique_id}")
             print(f"timestamp: {apns_response.timestamp.time if apns_response.timestamp else None}")
 
         return apns_response
 
 
-def config() -> Config:
-    return APNS.shared.config
+# def apns_config() -> Config:
+#     return APNS.shared.apns_config
 
 
 def initialize_apns(key_id='', team_id='', bundle_id='', is_prod: bool = None, p8_key_path='', pem_file_path='', apns_priority: int = None, apns_expiration: int = None):
     APNS.shared.initialize_apns(key_id=key_id, team_id=team_id, bundle_id=bundle_id, is_prod=is_prod, p8_key_path=p8_key_path, pem_file_path=pem_file_path,
                                 apns_priority=apns_priority, apns_expiration=apns_expiration)
     return APNS.shared
 
@@ -187,7 +191,42 @@
 
 
 def push(device_token: str, title: str, body: str = None, data: dict = None, badge: int = None, push_type: enums.PushType = None, collapse_id: str = None) -> ai_response.APNSResponse:
     alert_payload = ai_payload.AlertPayload(title=title, body=body)
     payload = ai_payload.Payload(alert=alert_payload, badge=badge, data=data)
 
     return push_raw(device_token=device_token, payload=payload, collapse_id=collapse_id)
+
+
+# @singleton.Singleton
+# class FirebaseSession:
+#     def __init__(self):
+#         self.__json_credentials_path = None
+#         self.__firebase_app: Optional[firebase_admin.App] = None
+#         self.__db: Optional[firebase_admin.firestore.firestore.Client] = None
+#
+#     @property
+#     def firebase_app(self) -> Optional[firebase_admin.App]:
+#         return self.__firebase_app
+#
+#     @property
+#     def firebase_db(self) -> Optional[firebase_admin.firestore.firestore.Client]:
+#         return self.__db
+#
+#     # region client
+#     def __initialize_firebase(self, json_credentials_path: str):
+#         if (self.__firebase_app is not None) \
+#                 and (self.__json_credentials_path == json_credentials_path):
+#             return
+#
+#         self.__json_credentials_path = json_credentials_path
+#         cred = firebase_admin.credentials.Certificate(self.__json_credentials_path)
+#         self.__firebase_app = firebase_admin.initialize_app(cred, {'storageBucket': 'instant-9101b.appspot.com'})
+#         self.__db = firebase_admin.firestore.client()
+#
+#     def initialize_firebase(self, json_credentials_path: str):
+#         self.__initialize_firebase(json_credentials_path=json_credentials_path)
+
+
+def initialize_firebase(json_credentials_path: str) -> firebase_admin.App:
+    FirebaseSession.shared.initialize_firebase(json_credentials_path=json_credentials_path)
+    return FirebaseSession.shared.firebase_app
```

### Comparing `aipkgs_notifications-0.0.9/aipkgs_notifications/enums.py` & `aipkgs_notifications-1.0.1/aipkgs_notifications/enums.py`

 * *Files identical despite different names*

### Comparing `aipkgs_notifications-0.0.9/aipkgs_notifications/payload.py` & `aipkgs_notifications-1.0.1/aipkgs_notifications/payload.py`

 * *Files 1% similar despite different names*

```diff
@@ -89,15 +89,15 @@
 
     def to_dict(self) -> dict:
         data = {"aps": {"alert": self.alert.to_dict() if self.alert else None,
                         "category": self.category,
                         "sound": self.sound.to_dict() if self.sound else {"name": "default"},
                         "badge": self.badge,
                         "thread-id": self.thread_id,
-                        "content-available": 1 if self.content_available else None,
+                        "content-available": 1 if self.content_available else 0,
                         "mutable-content": 1 if self.mutable_content else None,
                         "target-content-id": self.target_content_id,
                         "target-content-type": self.target_content_type,
                         "target-content-url": self.target_content_url,
                         "interruption-level": self.interruption_level.value if self.interruption_level else None,
                         "relevance-score": self.relevance_score if (self.relevance_score and ((self.relevance_score >= 0) and (self.relevance_score <= 1))) else None,
                         "filter-criteria": self.filter_criteria,
@@ -108,15 +108,15 @@
                         "dismissal-date": self.dismissal_date
                         },
                 "data": self.data}
 
         # if self.push_type == apns.PushType.background:
         #     data["aps"]["content-available"] = 1
 
-        if self.content_available:
-            data["aps"]["alert"] = None
-            data["aps"]["sound"] = None
-            data["aps"]["badge"] = None
+        # if self.content_available:
+        #     data["aps"]["alert"] = None
+        #     data["aps"]["sound"] = None
+        #     data["aps"]["badge"] = None
 
         data = utils.remove_nulls(data)
 
         return data
```

### Comparing `aipkgs_notifications-0.0.9/aipkgs_notifications/response.py` & `aipkgs_notifications-1.0.1/aipkgs_notifications/response.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
         self.status_code = self.httpx_response.status_code
         self.apns_id = headers.get('apns-id', None)
         self.apns_unique_id = headers.get('apns-unique-id', None)
         self.timestamp = Time(int(timestamp) * 1000) if timestamp else None
 
     @property
-    def is_sent(self) -> bool:
+    def is_success(self) -> bool:
         return self.httpx_response.is_success
 
 
 class Time:
     def __init__(self, timestamp):
         self.timestamp = timestamp
```

### Comparing `aipkgs_notifications-0.0.9/aipkgs_notifications/singleton.py` & `aipkgs_notifications-1.0.1/aipkgs_notifications/singleton.py`

 * *Files identical despite different names*

### Comparing `aipkgs_notifications-0.0.9/PKG-INFO` & `aipkgs_notifications-1.0.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: aipkgs-notifications
-Version: 0.0.9
-Summary: 
+Version: 1.0.1
+Summary: A simple package to send notifications to your devices using Firebase Cloud Messaging.
 Home-page: https://github.com/AlexyIbrahim/Notifications
 License: MIT
 Keywords: ai
 Author: Alexy
 Author-email: alexy.ib@outlook.com
-Requires-Python: >=3.9,<4.0
+Requires-Python: >=3.11.4,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: cryptography (>=41.0.5,<42.0.0)
+Requires-Dist: firebase-admin (>=6.3.0,<7.0.0)
 Requires-Dist: httpx[http2] (>=0.25.0,<0.26.0)
 Requires-Dist: pyjwt (>=2.8.0,<3.0.0)
 Project-URL: Repository, https://github.com/AlexyIbrahim/Notifications
 Description-Content-Type: text/markdown
 
 # APNS Push Notification
 
@@ -34,33 +33,33 @@
 ```python
 import apns
 ```
 
 Then, initialize the APNS with your application's details:
 
 ```python
-KEY_ID = ''  
-TEAM_ID = ''  
+KEY_ID = ''
+TEAM_ID = ''
 BUNDLE_ID = 'com.test.app'
 IS_PROD = False
-P8_KEY_PATH = 'path/to/p8/key'  
+P8_KEY_PATH = 'path/to/p8/key'
 PEM_FILE_PATH = 'path/to/pem/file'
 APNS_PRIORITY = 10
 APNS_EXPIRATION = 0
 
 apns.initialize_apns(key_id=KEY_ID,
                      team_id=TEAM_ID,
                      bundle_id=BUNDLE_ID,
                      is_prod=IS_PROD,
                      p8_key_path=P8_KEY_PATH,
                      pem_file_path=PEM_FILE_PATH,
                      apns_priority=APNS_PRIORITY,
                      apns_expiration=APNS_EXPIRATION)
 
-apns.config().verbose = True
+apns.apns_config().verbose = True
 ```
 
 Now, you can send a push notification:
 
 ```python
 device_token = ""  
 data = {}
```

