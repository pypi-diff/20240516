# Comparing `tmp/yuanfen-2024.4.25.1.tar.gz` & `tmp/yuanfen-2024.5.16.1.tar.gz`

## Comparing `yuanfen-2024.4.25.1.tar` & `yuanfen-2024.5.16.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 yuanfen-2024.4.25.1/src/yuanfen/__init__.py
--rw-r--r--   0        0        0     2125 2020-02-02 00:00:00.000000 yuanfen-2024.4.25.1/src/yuanfen/config.py
--rw-r--r--   0        0        0     3608 2020-02-02 00:00:00.000000 yuanfen-2024.4.25.1/src/yuanfen/email.py
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 yuanfen-2024.4.25.1/src/yuanfen/env.py
--rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 yuanfen-2024.4.25.1/src/yuanfen/group_robot.py
--rw-r--r--   0        0        0     1021 2020-02-02 00:00:00.000000 yuanfen-2024.4.25.1/src/yuanfen/ip.py
--rw-r--r--   0        0        0     1321 2020-02-02 00:00:00.000000 yuanfen-2024.4.25.1/src/yuanfen/logger.py
--rw-r--r--   0        0        0     1775 2020-02-02 00:00:00.000000 yuanfen-2024.4.25.1/src/yuanfen/redis.py
--rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 yuanfen-2024.4.25.1/src/yuanfen/response.py
--rw-r--r--   0        0        0     1323 2020-02-02 00:00:00.000000 yuanfen-2024.4.25.1/src/yuanfen/time.py
--rw-r--r--   0        0        0     2633 2020-02-02 00:00:00.000000 yuanfen-2024.4.25.1/src/yuanfen/version.py
--rw-r--r--   0        0        0     3501 2020-02-02 00:00:00.000000 yuanfen-2024.4.25.1/.gitignore
--rw-r--r--   0        0        0     1364 2020-02-02 00:00:00.000000 yuanfen-2024.4.25.1/README.md
--rw-r--r--   0        0        0      846 2020-02-02 00:00:00.000000 yuanfen-2024.4.25.1/pyproject.toml
--rw-r--r--   0        0        0     1994 2020-02-02 00:00:00.000000 yuanfen-2024.4.25.1/PKG-INFO
+-rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 yuanfen-2024.5.16.1/src/yuanfen/__init__.py
+-rw-r--r--   0        0        0     2125 2020-02-02 00:00:00.000000 yuanfen-2024.5.16.1/src/yuanfen/config.py
+-rw-r--r--   0        0        0     3723 2020-02-02 00:00:00.000000 yuanfen-2024.5.16.1/src/yuanfen/email.py
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 yuanfen-2024.5.16.1/src/yuanfen/env.py
+-rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 yuanfen-2024.5.16.1/src/yuanfen/group_robot.py
+-rw-r--r--   0        0        0     1021 2020-02-02 00:00:00.000000 yuanfen-2024.5.16.1/src/yuanfen/ip.py
+-rw-r--r--   0        0        0     1321 2020-02-02 00:00:00.000000 yuanfen-2024.5.16.1/src/yuanfen/logger.py
+-rw-r--r--   0        0        0     1775 2020-02-02 00:00:00.000000 yuanfen-2024.5.16.1/src/yuanfen/redis.py
+-rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 yuanfen-2024.5.16.1/src/yuanfen/response.py
+-rw-r--r--   0        0        0     1323 2020-02-02 00:00:00.000000 yuanfen-2024.5.16.1/src/yuanfen/time.py
+-rw-r--r--   0        0        0     2633 2020-02-02 00:00:00.000000 yuanfen-2024.5.16.1/src/yuanfen/version.py
+-rw-r--r--   0        0        0     3501 2020-02-02 00:00:00.000000 yuanfen-2024.5.16.1/.gitignore
+-rw-r--r--   0        0        0     1364 2020-02-02 00:00:00.000000 yuanfen-2024.5.16.1/README.md
+-rw-r--r--   0        0        0      846 2020-02-02 00:00:00.000000 yuanfen-2024.5.16.1/pyproject.toml
+-rw-r--r--   0        0        0     1994 2020-02-02 00:00:00.000000 yuanfen-2024.5.16.1/PKG-INFO
```

### Comparing `yuanfen-2024.4.25.1/src/yuanfen/__init__.py` & `yuanfen-2024.5.16.1/src/yuanfen/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from .env import APP_ENV
 from .group_robot import GroupRobot
 from .logger import Logger
 from .redis import Redis, RedisLock
 from .response import BaseResponse, ErrorResponse, SuccessResponse
 from .version import Version
 
-__version__ = "2024.4.25.1"
+__version__ = "2024.5.16.1"
 
 __all__ = [
     "APP_ENV",
     "BaseResponse",
     "Config",
     "Email",
     "ErrorResponse",
```

### Comparing `yuanfen-2024.4.25.1/src/yuanfen/config.py` & `yuanfen-2024.5.16.1/src/yuanfen/config.py`

 * *Files identical despite different names*

### Comparing `yuanfen-2024.4.25.1/src/yuanfen/email.py` & `yuanfen-2024.5.16.1/src/yuanfen/email.py`

 * *Files 6% similar despite different names*

```diff
@@ -49,14 +49,16 @@
             return ids.decode("utf-8").split()[-count:]
 
     def fetch(self, message_id: str, content_type: str = None):
         with imaplib.IMAP4_SSL(self.imap_server, self.imap_port, timeout=self.timeout) as connection:
             connection.login(self.address, self.password)
             connection.select()
             _, msg_data = connection.uid("fetch", message_id, "(RFC822)")
+            if not msg_data:
+                return None
             raw = email.message_from_bytes(msg_data[0][1])
             mail_info = {}
             mail_info["subject"] = get_header_content(raw, "Subject")
             mail_info["from"] = get_header_content(raw, "From")
             mail_info["to"] = get_header_content(raw, "To")
             date = get_header_content(raw, "Date")
             if date:
@@ -78,9 +80,11 @@
                 mail_info["content"] = payload.decode(charset)
                 break
             return mail_info
 
     def search(self, count: int, content_type: str, *criteria: str):
         messages = []
         for message_id in self.search_ids(count, *criteria):
-            messages.append(self.fetch(message_id, content_type))
+            message = self.fetch(message_id, content_type)
+            if message:
+                messages.append(message)
         return messages
```

### Comparing `yuanfen-2024.4.25.1/src/yuanfen/ip.py` & `yuanfen-2024.5.16.1/src/yuanfen/ip.py`

 * *Files identical despite different names*

### Comparing `yuanfen-2024.4.25.1/src/yuanfen/logger.py` & `yuanfen-2024.5.16.1/src/yuanfen/logger.py`

 * *Files identical despite different names*

### Comparing `yuanfen-2024.4.25.1/src/yuanfen/redis.py` & `yuanfen-2024.5.16.1/src/yuanfen/redis.py`

 * *Files identical despite different names*

### Comparing `yuanfen-2024.4.25.1/src/yuanfen/time.py` & `yuanfen-2024.5.16.1/src/yuanfen/time.py`

 * *Files identical despite different names*

### Comparing `yuanfen-2024.4.25.1/src/yuanfen/version.py` & `yuanfen-2024.5.16.1/src/yuanfen/version.py`

 * *Files identical despite different names*

### Comparing `yuanfen-2024.4.25.1/.gitignore` & `yuanfen-2024.5.16.1/.gitignore`

 * *Files identical despite different names*

### Comparing `yuanfen-2024.4.25.1/README.md` & `yuanfen-2024.5.16.1/README.md`

 * *Files identical despite different names*

### Comparing `yuanfen-2024.4.25.1/pyproject.toml` & `yuanfen-2024.5.16.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `yuanfen-2024.4.25.1/PKG-INFO` & `yuanfen-2024.5.16.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: yuanfen
-Version: 2024.4.25.1
+Version: 2024.5.16.1
 Summary: Yuanfen Python Library
 Project-URL: Homepage, https://github.com/YuanfenNet/yf-lib-py
 Author-email: Bean <bean@yuanfen.net>
 License-Expression: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
```

