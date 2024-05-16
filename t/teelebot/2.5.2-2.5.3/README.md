# Comparing `tmp/teelebot-2.5.2-py3-none-any.whl.zip` & `tmp/teelebot-2.5.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,22 +1,22 @@
-Zip file size: 43522 bytes, number of entries: 20
+Zip file size: 44191 bytes, number of entries: 20
 -rw-rw-rw-  2.0 fat     4279 b- defN 23-Dec-26 02:00 teelebot/__init__.py
 -rw-rw-rw-  2.0 fat      165 b- defN 23-May-08 17:02 teelebot/__main__.py
--rw-rw-rw-  2.0 fat    43226 b- defN 24-May-07 00:52 teelebot/bot.py
+-rw-rw-rw-  2.0 fat    43516 b- defN 24-May-16 09:47 teelebot/bot.py
 -rw-rw-rw-  2.0 fat    20714 b- defN 24-Apr-14 01:23 teelebot/buffer.py
 -rw-rw-rw-  2.0 fat     1771 b- defN 24-Feb-29 02:04 teelebot/common.py
 -rw-rw-rw-  2.0 fat    25637 b- defN 24-Feb-28 03:52 teelebot/handler.py
 -rw-rw-rw-  2.0 fat     1869 b- defN 23-Dec-25 01:59 teelebot/logger.py
 -rw-rw-rw-  2.0 fat     7236 b- defN 24-Feb-29 01:47 teelebot/metadata.py
 -rw-rw-rw-  2.0 fat      898 b- defN 23-Dec-26 02:32 teelebot/polling.py
--rw-rw-rw-  2.0 fat     3997 b- defN 24-Feb-28 01:38 teelebot/request.py
+-rw-rw-rw-  2.0 fat     6864 b- defN 24-May-16 09:51 teelebot/request.py
 -rw-rw-rw-  2.0 fat     4408 b- defN 24-May-06 05:02 teelebot/schedule.py
--rw-rw-rw-  2.0 fat      483 b- defN 24-May-06 09:29 teelebot/version.py
+-rw-rw-rw-  2.0 fat      483 b- defN 24-May-16 06:56 teelebot/version.py
 -rw-rw-rw-  2.0 fat     2796 b- defN 24-May-06 08:42 teelebot/webhook.py
--rw-rw-rw-  2.0 fat    35823 b- defN 24-May-07 00:59 teelebot-2.5.2.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     9964 b- defN 24-May-07 00:59 teelebot-2.5.2.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-May-07 00:59 teelebot-2.5.2.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       43 b- defN 24-May-07 00:59 teelebot-2.5.2.dist-info/entry_points.txt
--rw-rw-rw-  2.0 fat        9 b- defN 24-May-07 00:59 teelebot-2.5.2.dist-info/top_level.txt
--rw-rw-rw-  2.0 fat        2 b- defN 24-May-07 00:59 teelebot-2.5.2.dist-info/zip-safe
--rw-rw-r--  2.0 fat     1559 b- defN 24-May-07 00:59 teelebot-2.5.2.dist-info/RECORD
-20 files, 164971 bytes uncompressed, 41016 bytes compressed:  75.1%
+-rw-rw-rw-  2.0 fat    35823 b- defN 24-May-16 12:01 teelebot-2.5.3.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     9964 b- defN 24-May-16 12:01 teelebot-2.5.3.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-May-16 12:01 teelebot-2.5.3.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       43 b- defN 24-May-16 12:01 teelebot-2.5.3.dist-info/entry_points.txt
+-rw-rw-rw-  2.0 fat        9 b- defN 24-May-16 12:01 teelebot-2.5.3.dist-info/top_level.txt
+-rw-rw-rw-  2.0 fat        2 b- defN 24-May-16 12:01 teelebot-2.5.3.dist-info/zip-safe
+-rw-rw-r--  2.0 fat     1559 b- defN 24-May-16 12:01 teelebot-2.5.3.dist-info/RECORD
+20 files, 168128 bytes uncompressed, 41685 bytes compressed:  75.2%
```

## zipnote {}

```diff
@@ -33,29 +33,29 @@
 
 Filename: teelebot/version.py
 Comment: 
 
 Filename: teelebot/webhook.py
 Comment: 
 
-Filename: teelebot-2.5.2.dist-info/LICENSE
+Filename: teelebot-2.5.3.dist-info/LICENSE
 Comment: 
 
-Filename: teelebot-2.5.2.dist-info/METADATA
+Filename: teelebot-2.5.3.dist-info/METADATA
 Comment: 
 
-Filename: teelebot-2.5.2.dist-info/WHEEL
+Filename: teelebot-2.5.3.dist-info/WHEEL
 Comment: 
 
-Filename: teelebot-2.5.2.dist-info/entry_points.txt
+Filename: teelebot-2.5.3.dist-info/entry_points.txt
 Comment: 
 
-Filename: teelebot-2.5.2.dist-info/top_level.txt
+Filename: teelebot-2.5.3.dist-info/top_level.txt
 Comment: 
 
-Filename: teelebot-2.5.2.dist-info/zip-safe
+Filename: teelebot-2.5.3.dist-info/zip-safe
 Comment: 
 
-Filename: teelebot-2.5.2.dist-info/RECORD
+Filename: teelebot-2.5.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## teelebot/bot.py

```diff
@@ -1,12 +1,12 @@
 # -*- coding:utf-8 -*-
 """
 @description: A Python-based Telegram Bot framework
 @creation date: 2019-08-13
-@last modification: 2024-05-06
+@last modification: 2024-05-16
 @author: Pluto (github:plutobell)
 """
 import time
 import sys
 import os
 import copy
 import types
@@ -126,15 +126,16 @@
 
         thread_pool_size = int(self._pool_size)
         if int(self._pool_size) >= 3:
             thread_pool_size = round(int(self._pool_size) * 2 / 3)
         schedule_queue_size = round(int(self._pool_size) - thread_pool_size)
         if schedule_queue_size == 0: schedule_queue_size = int(self._pool_size)
 
-        self.request = _Request(thread_pool_size, self._url, self._debug, self.__proxies)
+        self.request = _Request(
+            thread_pool_size, self._url, self.message_deletor, config["hide_info"], self._debug, self.__proxies)
         self.schedule = _Schedule(schedule_queue_size)
         self.buffer = _Buffer(int(self._buffer_size) * 1024 * 1024,
             self.__plugin_bridge.keys(), self.__plugin_dir)
         self.metadata = _Metadata(self.__plugin_dir)
 
         self.__thread_pool = ThreadPoolExecutor(
             max_workers=thread_pool_size)
@@ -627,25 +628,25 @@
                         continue
 
                     no_plugin_path = f'{self.__plugin_dir}{plugin}.py'
                     if os.path.exists(no_plugin_path):
                         _logger.warn(f"[{message['update_id']}] Skip run {plugin} plugin: there is a module named '{plugin}.py' under the plugin dir with the same name as plugin {plugin} ({no_plugin_path})")
                         continue
 
+                    if self.__thread_pool._work_queue.qsize() >= self.__thread_pool._max_workers:
+                        if not self.__hide_info:
+                            _logger.info(f"[{message['update_id']}] Delay run {plugin} plugin: until a thread pool slot is available.")
+
                     def pluginFuncWrap(bot, message, plugin):
                         module = self.__import_module(plugin)
                         pluginFunc = getattr(module, plugin)
                         self.__logging_for_pluginRun(message, plugin, message["update_id"])
                         pluginFunc(bot, message)
                     fur = self.__thread_pool.submit(pluginFuncWrap, bot, message, plugin)
                     fur.add_done_callback(self.__threadpool_exception)
-
-                    if self.__thread_pool._work_queue.qsize() >= self.__thread_pool._max_workers:
-                        if not self.__hide_info:
-                            _logger.info(f"[{message['update_id']}] Delay run {plugin} plugin: until a thread pool slot is available.")
             
                     self.__response_times += 1
 
                     if message["chat"]["type"] != "private" and \
                     message["chat"]["id"] not in self.__response_chats:
                         self.__response_chats.append(message["chat"]["id"])
                     if message["from"]["id"] not in self.__response_users:
@@ -724,46 +725,49 @@
                 chat_join_request = result.get(query_or_message)
                 chat_join_request["update_id"] = result["update_id"]
                 chat_join_request["message_id"] = result.get("update_id")
                 chat_join_request["chat_join_request_id"] = result.get("update_id")
                 messages.append(chat_join_request)
             else:
                 message_dict = result.get(query_or_message)
-                message_dict["update_id"] = result["update_id"]
+                if isinstance(message_dict, dict):
+                    message_dict["update_id"] = result["update_id"]
                 messages.append(message_dict)
 
         if len(update_ids) >= 1:
             self._offset = max(update_ids) + 1
             return messages
         else:
             return None
     
     # teelebot method
     def message_deletor(self, time_gap: int, chat_id: str, message_id: str) -> str:
         """
         Timed deletion of a message, time range: [0, 900], in seconds
         """
         if time_gap < 0 or time_gap > 900:
+            _logger.error(f"[{chat_id}:{message_id}][{time_gap}s] Message deletion error: parameter time_gap is out of range.")
             return "time_gap_error"
         else:
             def message_deletor_func(time_gap, chat_id, message_id):
                 if not self.__hide_info:
                     _logger.info(f"[{chat_id}:{message_id}][{time_gap}s] Message deleting...")
 
-                time.sleep(int(time_gap))
+                if time_gap > 0:
+                    time.sleep(int(time_gap))
                 ok = self.deleteMessage(chat_id=chat_id, message_id=message_id)
                 
                 if ok:
                     if not self.__hide_info:
                         _logger.info(f"[{chat_id}:{message_id}][{time_gap}s] Message deleted.")
                 else:
                     _logger.error(f"[{chat_id}:{message_id}][{time_gap}s] Message deletion error.")
 
             if time_gap == 0:
-                message_deletor_func(chat_id, message_id)
+                message_deletor_func(time_gap, chat_id, message_id)
             else:
                 if self.__timer_thread_pool._work_queue.qsize() >= self.__timer_thread_pool._max_workers:
                     if not self.__hide_info:
                         _logger.info(f"[{chat_id}:{message_id}][{time_gap}s] Delay delete message: until a thread pool slot is available.")
 
                 fur = self.__timer_thread_pool.submit(
                     message_deletor_func, time_gap, chat_id, message_id)
```

## teelebot/request.py

```diff
@@ -1,36 +1,43 @@
 # -*- coding:utf-8 -*-
 '''
 @creation date: 2019-11-15
-@last modification: 2024-02-26
+@last modification: 2024-05-16
 '''
 import io
 import json
 import traceback
 import requests
 
 from .logger import _logger
 from traceback import extract_stack
+from concurrent.futures import ThreadPoolExecutor, Future
 
 
 class _Request(object):
     """
     Request Class
     """
-    def __init__(self, thread_pool_size, url, debug=False, proxies={"all": None}):
+    def __init__(self, thread_pool_size, url, message_deletor, hide_info, debug=False, proxies={"all": None}):
         self.__url = url
+        self.__message_deletor = message_deletor
+        self.__hide_info = hide_info
         self.__debug = debug
         self.__proxies = proxies
+
         self.__session = self.__connection_session(
             pool_connections=thread_pool_size,
             pool_maxsize=thread_pool_size * 2
         )
+        self.__thread_pool = ThreadPoolExecutor(
+            max_workers=thread_pool_size * 2)
 
     def __del__(self):
         self.__session.close()
+        self.__thread_pool.shutdown(wait=True)
 
     def __connection_session(self, pool_connections=10, pool_maxsize=10, max_retries=5):
         """
         Connection Pool
         """
         session = requests.Session()
         session.verify = False
@@ -72,14 +79,28 @@
 
         inputmedia_methods = ["sendMediaGroup", "editMessageMedia"]
         is_inputmedia = False
         inputmedia_param_name = "files"
         if method_name in inputmedia_methods:
             is_inputmedia = True
 
+        run_in_thread = False
+        run_in_thread_param_name = "run_in_thread"
+        if run_in_thread_param_name in list(kwargs.keys()):
+            value = kwargs.get(run_in_thread_param_name, False)
+            if isinstance(value, bool):
+                run_in_thread = value
+
+        del_msg_after = -1
+        del_msg_after_param_name = "del_msg_after"
+        if del_msg_after_param_name in list(kwargs.keys()):
+            value = kwargs.get(del_msg_after_param_name, False)
+            if isinstance(value, int):
+                del_msg_after = value
+
         data, files = {}, {}
         for key, value in kwargs.items():
             if isinstance(value, io.BufferedReader):
                 value = value.read()
 
             if not is_inputmedia and key == inputmedia_param_name:
                 pass
@@ -93,20 +114,68 @@
                 data[key] = json.dumps(value)
             elif isinstance(value, list):
                 data[key] = json.dumps(value)
             else:
                 data[key] = value
 
         # print(data, "\n", files)
+        url = f'{self.__url}{method_name}'
+        if run_in_thread:
+            try:
+                if self.__thread_pool._work_queue.qsize() >= self.__thread_pool._max_workers:
+                    if not self.__hide_info:
+                        _logger.info(f"[{id(self.postEverything)}] Delay run {method_name} method: until a thread pool slot is available.")
+
+                fur = self.__thread_pool.submit(
+                    self.__requestFunc, method_name, url, data, files, del_msg_after)
+                fur.add_done_callback(self.__threadpool_exception)
+
+                return True
+            except Exception as e:
+                _logger.error(f"Error executing method {method_name}:", str(e))
+                traceback.print_exc()
+
+                return False
+        else:
+            return self.__requestFunc(
+                method_name=method_name,
+                url=url,
+                data=data,
+                files=files,
+                del_msg_after=del_msg_after
+            )
+
+    def __requestFunc(self, method_name, url, data, files, del_msg_after):
         try:
-            with self.__session.post(url=f'{self.__url}{method_name}', data=data, files=files) as req:
-                self.__debug_info(method_name, req.json())
-                if req.json().get("ok", False):
-                    return req.json().get("result")
+            with self.__session.post(url=url, data=data, files=files) as req:
+                data = req.json()
+                self.__debug_info(method_name, data)
+                if data.get("ok", False):
+                    result = data.get("result")
+
+                    if del_msg_after >= 0:
+                        if isinstance(result, dict) \
+                            and "chat" in result.keys() \
+                            and "id" in result.get("chat").keys() \
+                            and "message_id" in result.keys():
+
+                            chat_id = result.get("chat").get("id")
+                            message_id = result.get("message_id")
+                            self.__message_deletor(
+                                time_gap=del_msg_after,
+                                chat_id=chat_id,
+                                message_id=message_id
+                            )
+
+                    return result
                 else:
-                    return req.json().get("ok")
+                    return data.get("ok")
         except Exception as e:
             _logger.error(f"Error executing method {method_name}:", str(e))
             traceback.print_exc()
             return False
 
+    def __threadpool_exception(self, fur):
+        if fur.exception() is not None:
+            _logger.debug(f"EXCEPTION - {str(fur.result())}")
+
```

## teelebot/version.py

```diff
@@ -1,16 +1,16 @@
 # -*- coding:utf-8 -*-
 """
 @description: A Python-based Telegram Bot framework
 @creation date: 2019-11-15
-@last modification: 2024-05-06
+@last modification: 2024-05-16
 @author: Pluto (github:plutobell)
 """
 
-__version__ = "2.5.2"
+__version__ = "2.5.3"
 
 __author__ = "Pluto"
 __email__ = "hi@ojoll.com"
 __blog__ = "https://ojoll.com"
 __github__ = "https://github.com/plutobell/teelebot"
 __description__ = "teelebot is a Python-based Telegram Bot framework with a plugin system that supports hot reload and hot loading."
```

## Comparing `teelebot-2.5.2.dist-info/LICENSE` & `teelebot-2.5.3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `teelebot-2.5.2.dist-info/METADATA` & `teelebot-2.5.3.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: teelebot
-Version: 2.5.2
+Version: 2.5.3
 Summary: teelebot is a Python-based Telegram Bot framework with a plugin system that supports hot reload and hot loading.
 Home-page: https://ojoll.com
 Author: Pluto
 Author-email: hi@ojoll.com
 License: GPLv3
 Keywords: teelebot telegram bot telegram bot api telegram
 Classifier: Programming Language :: Python :: 3
```

### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: teelebot Version: 2.5.2 Summary: teelebot is a
+Metadata-Version: 2.1 Name: teelebot Version: 2.5.3 Summary: teelebot is a
 Python-based Telegram Bot framework with a plugin system that supports hot
 reload and hot loading. Home-page: https://ojoll.com Author: Pluto Author-
 email: hi@ojoll.com License: GPLv3 Keywords: teelebot telegram bot telegram bot
 api telegram Classifier: Programming Language :: Python :: 3 Classifier:
 Operating System :: OS Independent Classifier: License :: OSI Approved :: GNU
 General Public License v3 (GPLv3) Requires-Python: >=3.6 Description-Content-
 Type: text/markdown License-File: LICENSE Requires-Dist: requests
```

## Comparing `teelebot-2.5.2.dist-info/RECORD` & `teelebot-2.5.3.dist-info/RECORD`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 teelebot/__init__.py,sha256=kAq6jlmvcxByifHdMlapLN-el_IL9h6pIkggxzvnn8c,4279
 teelebot/__main__.py,sha256=_j6f3hj0VtlcCsabcIvuS0uBI0NVbCVwmH138tqYGFo,165
-teelebot/bot.py,sha256=-U49Apfm4YuQ7xghLxijoXXxERIscYdCYVfefS3fiJ4,43226
+teelebot/bot.py,sha256=efHkPfDG1oTsIElvKxfQVllsMthGw5OlrEMgQUb1O_w,43516
 teelebot/buffer.py,sha256=payjL7pxJRn1rszs5IFq7DHEpB261dny0fO16Ko86pE,20714
 teelebot/common.py,sha256=ltYHihcrxrYVtjvBLQ8rXjEpO-4pfqJ6w_oqrTXK1ys,1771
 teelebot/handler.py,sha256=jxrMraJz5lh5bZJ5jKZsBjMgSMfeEfV8Krc5quYdghQ,25637
 teelebot/logger.py,sha256=I7UJxLdxRz5HxzwEgBPf_gILZuDlPCLwZPxioIahS2A,1869
 teelebot/metadata.py,sha256=e1UR2Nz2eP9hoLByb_j-4byPd6vpNk1SIN52o04PmYM,7236
 teelebot/polling.py,sha256=p_JO9TOgyTifTbZEcGpPRYAHp4MyoFkJ3wY0-D7yC4Q,898
-teelebot/request.py,sha256=HenftV-3frTxNks1HjMVQCCYo8SeDA2Jhhe8T1xpjD4,3997
+teelebot/request.py,sha256=Dc5UOB6Jq2YEHRUcYTz4TU13Hrz49Dvj96PdCrMHPmU,6864
 teelebot/schedule.py,sha256=K4-PpROpldz8YnGebW8sFXILViB66KQgtopT98SseE4,4408
-teelebot/version.py,sha256=ng676aTzzHbOcMVW8OuonJUdIlVnV97FzRuqf64_8M0,483
+teelebot/version.py,sha256=T3vTsDwaE922bYoERGBFRDsccWvv2s5NZZQ3KpQLtgg,483
 teelebot/webhook.py,sha256=5cd9GPAv4_LHTxDZC9s0NsKKq5eZGx_3L1i6Bl4lbig,2796
-teelebot-2.5.2.dist-info/LICENSE,sha256=IwGE9guuL-ryRPEKi6wFPI_zOhg7zDZbTYuHbSt_SAk,35823
-teelebot-2.5.2.dist-info/METADATA,sha256=348Zpn1uJ5Ktt-T6WILFFxqEUVLb_6NS4kbbgloVNL8,9964
-teelebot-2.5.2.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-teelebot-2.5.2.dist-info/entry_points.txt,sha256=IZHSiwFVJ6BPPTW3j7I1i34AESCOPaTYiC1qoWfpj6k,43
-teelebot-2.5.2.dist-info/top_level.txt,sha256=vMgTMVZJd4P3KjMwVpgWfIUvNLYKqfyHO4Cul-YwuyQ,9
-teelebot-2.5.2.dist-info/zip-safe,sha256=frcCV1k9oG9oKj3dpUqdJg1PxRT2RSN_XKdLCPjaYaY,2
-teelebot-2.5.2.dist-info/RECORD,,
+teelebot-2.5.3.dist-info/LICENSE,sha256=IwGE9guuL-ryRPEKi6wFPI_zOhg7zDZbTYuHbSt_SAk,35823
+teelebot-2.5.3.dist-info/METADATA,sha256=46AunQ3Qo9Utn2KG1DkL42p-vTgrFlziRXlY7VtJMGE,9964
+teelebot-2.5.3.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+teelebot-2.5.3.dist-info/entry_points.txt,sha256=IZHSiwFVJ6BPPTW3j7I1i34AESCOPaTYiC1qoWfpj6k,43
+teelebot-2.5.3.dist-info/top_level.txt,sha256=vMgTMVZJd4P3KjMwVpgWfIUvNLYKqfyHO4Cul-YwuyQ,9
+teelebot-2.5.3.dist-info/zip-safe,sha256=frcCV1k9oG9oKj3dpUqdJg1PxRT2RSN_XKdLCPjaYaY,2
+teelebot-2.5.3.dist-info/RECORD,,
```

