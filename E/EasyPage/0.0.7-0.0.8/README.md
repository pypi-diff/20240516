# Comparing `tmp/EasyPage-0.0.7.tar.gz` & `tmp/EasyPage-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "EasyPage-0.0.7.tar", last modified: Thu May 16 03:42:47 2024, max compression
+gzip compressed data, was "EasyPage-0.0.8.tar", last modified: Thu May 16 07:10:29 2024, max compression
```

## Comparing `EasyPage-0.0.7.tar` & `EasyPage-0.0.8.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxrwxrwx   0        0        0        0 2024-05-16 03:42:47.147691 EasyPage-0.0.7/
-drwxrwxrwx   0        0        0        0 2024-05-16 03:42:46.811139 EasyPage-0.0.7/EasyPage.egg-info/
--rw-rw-rw-   0        0        0      286 2024-05-16 03:42:46.000000 EasyPage-0.0.7/EasyPage.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1060 2024-05-16 03:42:46.000000 EasyPage-0.0.7/EasyPage.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-16 03:42:46.000000 EasyPage-0.0.7/EasyPage.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       76 2024-05-16 03:42:46.000000 EasyPage-0.0.7/EasyPage.egg-info/requires.txt
--rw-rw-rw-   0        0        0       24 2024-05-16 03:42:46.000000 EasyPage-0.0.7/EasyPage.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      286 2024-05-16 03:42:47.147691 EasyPage-0.0.7/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-16 03:42:46.946177 EasyPage-0.0.7/easypage/
--rw-rw-rw-   0        0        0      192 2024-05-16 02:17:32.000000 EasyPage-0.0.7/easypage/__init__.py
--rw-rw-rw-   0        0        0     3349 2024-05-13 03:04:45.000000 EasyPage-0.0.7/easypage/cdp.py
-drwxrwxrwx   0        0        0        0 2024-05-16 03:42:47.072289 EasyPage-0.0.7/easypage/cdp_method/
--rw-rw-rw-   0        0        0        0 2024-04-17 12:56:48.000000 EasyPage-0.0.7/easypage/cdp_method/__init__.py
--rw-rw-rw-   0        0        0     1536 2024-04-24 09:10:40.000000 EasyPage-0.0.7/easypage/cdp_method/browser.py
--rw-rw-rw-   0        0        0     1962 2024-05-13 03:08:12.000000 EasyPage-0.0.7/easypage/cdp_method/css.py
--rw-rw-rw-   0        0        0    12414 2024-05-13 03:01:05.000000 EasyPage-0.0.7/easypage/cdp_method/dom.py
--rw-rw-rw-   0        0        0     1049 2024-04-24 08:57:22.000000 EasyPage-0.0.7/easypage/cdp_method/emulation.py
--rw-rw-rw-   0        0        0     9545 2024-04-24 14:05:55.000000 EasyPage-0.0.7/easypage/cdp_method/fetch.py
--rw-rw-rw-   0        0        0     2654 2024-04-24 09:06:00.000000 EasyPage-0.0.7/easypage/cdp_method/input.py
--rw-rw-rw-   0        0        0     4467 2024-05-07 11:18:55.000000 EasyPage-0.0.7/easypage/cdp_method/network.py
--rw-rw-rw-   0        0        0     8620 2024-05-16 02:51:16.000000 EasyPage-0.0.7/easypage/cdp_method/page.py
--rw-rw-rw-   0        0        0     3667 2024-04-24 09:16:01.000000 EasyPage-0.0.7/easypage/cdp_method/runtime.py
--rw-rw-rw-   0        0        0     2354 2024-04-24 09:16:01.000000 EasyPage-0.0.7/easypage/cdp_method/security.py
--rw-rw-rw-   0        0        0     1322 2024-04-24 09:16:01.000000 EasyPage-0.0.7/easypage/cdp_method/storage.py
--rw-rw-rw-   0        0        0     5884 2024-04-24 13:35:04.000000 EasyPage-0.0.7/easypage/cdp_method/target.py
--rw-rw-rw-   0        0        0    17770 2024-05-16 03:42:29.000000 EasyPage-0.0.7/easypage/conn.py
--rw-rw-rw-   0        0        0      391 2024-04-25 02:28:17.000000 EasyPage-0.0.7/easypage/definition.py
-drwxrwxrwx   0        0        0        0 2024-05-16 03:42:47.128698 EasyPage-0.0.7/easypage/driver/
--rw-rw-rw-   0        0        0        0 2024-04-09 06:15:36.000000 EasyPage-0.0.7/easypage/driver/__init__.py
--rw-rw-rw-   0        0        0     7785 2024-05-14 01:38:27.000000 EasyPage-0.0.7/easypage/driver/browser.py
--rw-rw-rw-   0        0        0      928 2024-05-09 09:58:08.000000 EasyPage-0.0.7/easypage/driver/driver.py
--rw-rw-rw-   0        0        0    43065 2024-05-16 03:05:30.000000 EasyPage-0.0.7/easypage/driver/page.py
--rw-rw-rw-   0        0        0     1462 2024-04-24 08:29:43.000000 EasyPage-0.0.7/easypage/errors.py
--rw-rw-rw-   0        0        0     2097 2024-05-14 03:49:35.000000 EasyPage-0.0.7/easypage/event_manager.py
--rw-rw-rw-   0        0        0     5762 2024-05-11 02:30:56.000000 EasyPage-0.0.7/easypage/listener.py
--rw-rw-rw-   0        0        0     2093 2024-05-09 07:29:23.000000 EasyPage-0.0.7/easypage/logger.py
--rw-rw-rw-   0        0        0     4580 2024-05-14 01:35:01.000000 EasyPage-0.0.7/easypage/main.py
--rw-rw-rw-   0        0        0     4106 2024-04-25 08:20:54.000000 EasyPage-0.0.7/easypage/operate.py
--rw-rw-rw-   0        0        0    10944 2024-04-24 08:39:28.000000 EasyPage-0.0.7/easypage/options.py
--rw-rw-rw-   0        0        0     1805 2024-05-10 01:35:17.000000 EasyPage-0.0.7/easypage/request.py
--rw-rw-rw-   0        0        0     4390 2024-05-10 01:15:20.000000 EasyPage-0.0.7/easypage/response.py
--rw-rw-rw-   0        0        0     2787 2024-05-15 02:22:54.000000 EasyPage-0.0.7/easypage/settings.py
-drwxrwxrwx   0        0        0        0 2024-05-16 03:42:47.137690 EasyPage-0.0.7/easypage/utils/
--rw-rw-rw-   0        0        0        0 2024-04-09 06:15:42.000000 EasyPage-0.0.7/easypage/utils/__init__.py
--rw-rw-rw-   0        0        0     3708 2024-04-10 01:27:44.000000 EasyPage-0.0.7/easypage/utils/browser_utils.py
--rw-rw-rw-   0        0        0     2182 2024-05-09 08:03:26.000000 EasyPage-0.0.7/easypage/utils/other_utils.py
-drwxrwxrwx   0        0        0        0 2024-05-16 03:42:47.146690 EasyPage-0.0.7/easypage_async/
--rw-rw-rw-   0        0        0       40 2024-05-14 06:22:35.000000 EasyPage-0.0.7/easypage_async/__init__.py
--rw-rw-rw-   0        0        0       42 2024-05-16 03:42:47.147691 EasyPage-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0      599 2024-05-16 03:42:07.000000 EasyPage-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-16 07:10:29.497529 EasyPage-0.0.8/
+drwxrwxrwx   0        0        0        0 2024-05-16 07:10:29.245953 EasyPage-0.0.8/EasyPage.egg-info/
+-rw-rw-rw-   0        0        0      286 2024-05-16 07:10:29.000000 EasyPage-0.0.8/EasyPage.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1060 2024-05-16 07:10:29.000000 EasyPage-0.0.8/EasyPage.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-16 07:10:29.000000 EasyPage-0.0.8/EasyPage.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       76 2024-05-16 07:10:29.000000 EasyPage-0.0.8/EasyPage.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       24 2024-05-16 07:10:29.000000 EasyPage-0.0.8/EasyPage.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      286 2024-05-16 07:10:29.497529 EasyPage-0.0.8/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-16 07:10:29.317952 EasyPage-0.0.8/easypage/
+-rw-rw-rw-   0        0        0      192 2024-05-16 02:17:32.000000 EasyPage-0.0.8/easypage/__init__.py
+-rw-rw-rw-   0        0        0     3499 2024-05-16 07:05:55.000000 EasyPage-0.0.8/easypage/cdp.py
+drwxrwxrwx   0        0        0        0 2024-05-16 07:10:29.460525 EasyPage-0.0.8/easypage/cdp_method/
+-rw-rw-rw-   0        0        0        0 2024-04-17 12:56:48.000000 EasyPage-0.0.8/easypage/cdp_method/__init__.py
+-rw-rw-rw-   0        0        0     1536 2024-04-24 09:10:40.000000 EasyPage-0.0.8/easypage/cdp_method/browser.py
+-rw-rw-rw-   0        0        0     1962 2024-05-13 03:08:12.000000 EasyPage-0.0.8/easypage/cdp_method/css.py
+-rw-rw-rw-   0        0        0    12414 2024-05-13 03:01:05.000000 EasyPage-0.0.8/easypage/cdp_method/dom.py
+-rw-rw-rw-   0        0        0     1049 2024-04-24 08:57:22.000000 EasyPage-0.0.8/easypage/cdp_method/emulation.py
+-rw-rw-rw-   0        0        0     9545 2024-04-24 14:05:55.000000 EasyPage-0.0.8/easypage/cdp_method/fetch.py
+-rw-rw-rw-   0        0        0     2654 2024-04-24 09:06:00.000000 EasyPage-0.0.8/easypage/cdp_method/input.py
+-rw-rw-rw-   0        0        0     4467 2024-05-07 11:18:55.000000 EasyPage-0.0.8/easypage/cdp_method/network.py
+-rw-rw-rw-   0        0        0     8620 2024-05-16 02:51:16.000000 EasyPage-0.0.8/easypage/cdp_method/page.py
+-rw-rw-rw-   0        0        0     3667 2024-04-24 09:16:01.000000 EasyPage-0.0.8/easypage/cdp_method/runtime.py
+-rw-rw-rw-   0        0        0     2354 2024-04-24 09:16:01.000000 EasyPage-0.0.8/easypage/cdp_method/security.py
+-rw-rw-rw-   0        0        0     1322 2024-04-24 09:16:01.000000 EasyPage-0.0.8/easypage/cdp_method/storage.py
+-rw-rw-rw-   0        0        0     5884 2024-04-24 13:35:04.000000 EasyPage-0.0.8/easypage/cdp_method/target.py
+-rw-rw-rw-   0        0        0    18116 2024-05-16 07:10:10.000000 EasyPage-0.0.8/easypage/conn.py
+-rw-rw-rw-   0        0        0      391 2024-04-25 02:28:17.000000 EasyPage-0.0.8/easypage/definition.py
+drwxrwxrwx   0        0        0        0 2024-05-16 07:10:29.484527 EasyPage-0.0.8/easypage/driver/
+-rw-rw-rw-   0        0        0        0 2024-04-09 06:15:36.000000 EasyPage-0.0.8/easypage/driver/__init__.py
+-rw-rw-rw-   0        0        0     7785 2024-05-14 01:38:27.000000 EasyPage-0.0.8/easypage/driver/browser.py
+-rw-rw-rw-   0        0        0      928 2024-05-09 09:58:08.000000 EasyPage-0.0.8/easypage/driver/driver.py
+-rw-rw-rw-   0        0        0    44997 2024-05-16 07:09:02.000000 EasyPage-0.0.8/easypage/driver/page.py
+-rw-rw-rw-   0        0        0     1598 2024-05-16 06:11:45.000000 EasyPage-0.0.8/easypage/errors.py
+-rw-rw-rw-   0        0        0     2137 2024-05-16 06:41:09.000000 EasyPage-0.0.8/easypage/event_manager.py
+-rw-rw-rw-   0        0        0     5897 2024-05-16 06:06:04.000000 EasyPage-0.0.8/easypage/listener.py
+-rw-rw-rw-   0        0        0     2093 2024-05-09 07:29:23.000000 EasyPage-0.0.8/easypage/logger.py
+-rw-rw-rw-   0        0        0     4580 2024-05-14 01:35:01.000000 EasyPage-0.0.8/easypage/main.py
+-rw-rw-rw-   0        0        0     4106 2024-04-25 08:20:54.000000 EasyPage-0.0.8/easypage/operate.py
+-rw-rw-rw-   0        0        0    10944 2024-04-24 08:39:28.000000 EasyPage-0.0.8/easypage/options.py
+-rw-rw-rw-   0        0        0     1813 2024-05-16 06:38:58.000000 EasyPage-0.0.8/easypage/request.py
+-rw-rw-rw-   0        0        0     4390 2024-05-10 01:15:20.000000 EasyPage-0.0.8/easypage/response.py
+-rw-rw-rw-   0        0        0     2787 2024-05-15 02:22:54.000000 EasyPage-0.0.8/easypage/settings.py
+drwxrwxrwx   0        0        0        0 2024-05-16 07:10:29.493525 EasyPage-0.0.8/easypage/utils/
+-rw-rw-rw-   0        0        0        0 2024-04-09 06:15:42.000000 EasyPage-0.0.8/easypage/utils/__init__.py
+-rw-rw-rw-   0        0        0     3708 2024-04-10 01:27:44.000000 EasyPage-0.0.8/easypage/utils/browser_utils.py
+-rw-rw-rw-   0        0        0     2182 2024-05-09 08:03:26.000000 EasyPage-0.0.8/easypage/utils/other_utils.py
+drwxrwxrwx   0        0        0        0 2024-05-16 07:10:29.495525 EasyPage-0.0.8/easypage_async/
+-rw-rw-rw-   0        0        0       40 2024-05-14 06:22:35.000000 EasyPage-0.0.8/easypage_async/__init__.py
+-rw-rw-rw-   0        0        0       42 2024-05-16 07:10:29.498529 EasyPage-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0      599 2024-05-16 07:10:25.000000 EasyPage-0.0.8/setup.py
```

### Comparing `EasyPage-0.0.7/EasyPage.egg-info/SOURCES.txt` & `EasyPage-0.0.8/EasyPage.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `EasyPage-0.0.7/easypage/cdp.py` & `EasyPage-0.0.8/easypage/cdp.py`

 * *Files 3% similar despite different names*

```diff
@@ -73,14 +73,22 @@
         """
         return self.__conn.send(
             method=method,
             raise_err=raise_err,
             params=params
         )
 
+    def closed(self) -> bool:
+        """
+        返回连接是否关闭
+
+        :return:
+        """
+        return self.__conn.closed()
+
     @property
     def target(self) -> Target:
         return Target(self.__conn)
 
     @property
     def page(self) -> Page:
         return Page(self.__conn)
```

### Comparing `EasyPage-0.0.7/easypage/cdp_method/browser.py` & `EasyPage-0.0.8/easypage/cdp_method/browser.py`

 * *Files identical despite different names*

### Comparing `EasyPage-0.0.7/easypage/cdp_method/css.py` & `EasyPage-0.0.8/easypage/cdp_method/css.py`

 * *Files identical despite different names*

### Comparing `EasyPage-0.0.7/easypage/cdp_method/dom.py` & `EasyPage-0.0.8/easypage/cdp_method/dom.py`

 * *Files identical despite different names*

### Comparing `EasyPage-0.0.7/easypage/cdp_method/emulation.py` & `EasyPage-0.0.8/easypage/cdp_method/emulation.py`

 * *Files identical despite different names*

### Comparing `EasyPage-0.0.7/easypage/cdp_method/fetch.py` & `EasyPage-0.0.8/easypage/cdp_method/fetch.py`

 * *Files identical despite different names*

### Comparing `EasyPage-0.0.7/easypage/cdp_method/input.py` & `EasyPage-0.0.8/easypage/cdp_method/input.py`

 * *Files identical despite different names*

### Comparing `EasyPage-0.0.7/easypage/cdp_method/network.py` & `EasyPage-0.0.8/easypage/cdp_method/network.py`

 * *Files identical despite different names*

### Comparing `EasyPage-0.0.7/easypage/cdp_method/page.py` & `EasyPage-0.0.8/easypage/cdp_method/page.py`

 * *Files identical despite different names*

### Comparing `EasyPage-0.0.7/easypage/cdp_method/runtime.py` & `EasyPage-0.0.8/easypage/cdp_method/runtime.py`

 * *Files identical despite different names*

### Comparing `EasyPage-0.0.7/easypage/cdp_method/security.py` & `EasyPage-0.0.8/easypage/cdp_method/security.py`

 * *Files identical despite different names*

### Comparing `EasyPage-0.0.7/easypage/cdp_method/storage.py` & `EasyPage-0.0.8/easypage/cdp_method/storage.py`

 * *Files identical despite different names*

### Comparing `EasyPage-0.0.7/easypage/cdp_method/target.py` & `EasyPage-0.0.8/easypage/cdp_method/target.py`

 * *Files identical despite different names*

### Comparing `EasyPage-0.0.7/easypage/conn.py` & `EasyPage-0.0.8/easypage/conn.py`

 * *Files 2% similar despite different names*

```diff
@@ -336,14 +336,18 @@
 
         :param method:
         :param params:
         :param raise_err: 接收到错误消息时，是否抛出，默认为 False
         :param need_callback: 接收到消息时，是否返回，默认为 True
         :return
         """
+        # 判断连接是否正常
+        if self.closed():
+            return False, dict()
+
         # 发送消息
         status, msg = self.__send(
             method=method,
             params=params,
             need_callback=need_callback
         )
 
@@ -363,40 +367,44 @@
                 if "result" in recv_msg:
                     return True, recv_msg["result"]
                 elif "error" in recv_msg:
                     if raise_err:
                         raise errors.CDPRecvErrorMsg(recv_msg["error"])
                     return False, recv_msg["error"]
 
-                logger.error("没有结果：{}", recv_msg)
+                logger.warning("没有结果：{}", recv_msg)
             except Empty:
                 if time.time() - start_time >= self.timeout:
                     self.__remove_result(msg_id=msg["id"])
                     if raise_err:
                         raise errors.CDPRecvTimeout(msg)
-                    logger.error("接收超时：{}", msg)
+                    logger.warning("接收超时：{}", msg)
                     break
 
+        return False, dict()
+
     def __send(
             self,
             method: str,
             params: dict = None,
+            raise_err: bool = False,
             need_callback: bool = True,
     ) -> typing.Tuple[bool, dict]:
         """
         同步发送消息
 
         使用：status, value = send(method="", raise_err=False, params={})
 
         返回的结果是有两个值：
             - status 表示当前消息是否有错误发生（raise_err 为 True 时直接抛出）
             - value 是对应浏览器返回的消息，是一个 dict
 
         :param method:
         :param params:
+        :param raise_err: 接收到错误消息时，是否抛出，默认为 False
         :param need_callback: 接收到消息时，是否返回，默认为 True
         :return
         """
         # 构建消息
         msg = {
             "id": self.__get_id,
             "method": method,  # 在此示例中启用网络事件
@@ -409,24 +417,25 @@
         msg_json = json.dumps(msg)
         logger.debug("[SEND] {}", msg_json)
 
         # 发送信息
         try:
             self.__ws.send(msg_json)
             return True, msg
-        except (errors.CDPRecvTimeout, errors.CDPRecvErrorMsg):
-            raise
         except (websocket.WebSocketConnectionClosedException, ConnectionResetError):
-            # logger.warning("连接已断开：{}", self.driver_url)
-            raise errors.CDPConnClosed(f"连接已断开：{self.driver_url}")
+            self.__stop = True
+            if raise_err:
+                raise errors.CDPConnClosed(f"连接已断开：{self.driver_url}")
+            else:
+                logger.warning("连接已断开：{}", self.driver_url)
         except:
             traceback.print_exc()
             raise
 
-        # return False, dict()
+        return False, dict()
 
     def __recv_result(self):
         """
         接收消息、事件处理
 
         :return:
         """
@@ -435,27 +444,28 @@
                 msg = self.__ws.recv()
                 logger.debug("[RECV] {}", msg)
                 msg = json.loads(msg)
             except websocket.WebSocketTimeoutException:
                 continue
             except (websocket.WebSocketConnectionClosedException, ConnectionResetError):
                 logger.warning("连接已断开：{}", self.driver_url)
+                self.__stop = True
                 return
             except Exception:
                 if self.__stop:
                     return
                 else:
                     self.__stop = True
                     raise
 
             # 消息处理
             if msg.get("id"):
                 has_error = False
                 if msg.get("error"):
-                    logger.error("[RECV] {}", msg["error"])
+                    logger.warning("[RECV] {}", msg["error"])
                     has_error = True
 
                 # 消息 id 存在的话就是需要立刻回调
                 if msg["id"] in self.__result_monitor:
                     self.__add_result(msg_id=msg["id"], result=msg)
                 else:
                     # 判断响应-body 获取事件的触发
@@ -474,14 +484,17 @@
 
     def closed(self) -> bool:
         """
         判断连接是否断开，同时做一点处理
 
         :return:
         """
+        if self.__stop:
+            return True
+
         status = self.__ws.connected
         if not status:
             self.__stop = True
 
         return not status
 
     def close(self):
```

### Comparing `EasyPage-0.0.7/easypage/driver/browser.py` & `EasyPage-0.0.8/easypage/driver/browser.py`

 * *Files identical despite different names*

### Comparing `EasyPage-0.0.7/easypage/driver/driver.py` & `EasyPage-0.0.8/easypage/driver/driver.py`

 * *Files identical despite different names*

### Comparing `EasyPage-0.0.7/easypage/driver/page.py` & `EasyPage-0.0.8/easypage/driver/page.py`

 * *Files 4% similar despite different names*

```diff
@@ -148,22 +148,23 @@
             return None
 
         elements = []
         for nn in new_nodes['nodeIds']:
             elements.append(Element(node_id=nn, page=self))
         return elements
 
-    def eval_js(self, js: str, **kwargs) -> Tuple[bool, any]:
+    def eval_js(self, js: str, raise_err: bool = False, **kwargs) -> Tuple[bool, any]:
         """
         执行 js 脚本
 
         :param js: 路径或者 js 字符串
+        :param raise_err: 接收到错误消息时，是否抛出，默认为 False
         :return: 可能是字符串、数字等
         """
-        status, result = self.cdp.runtime.evaluate(js, **kwargs)
+        status, result = self.cdp.runtime.evaluate(js=js, raise_err=raise_err, **kwargs)
         if not status:
             return status, result
 
         if 'value' in result['result']:
             return True, result['result']['value']
         else:
             return False, result['result']['description']
@@ -393,15 +394,15 @@
         关闭当前页面
 
         :return:
         """
         self.cdp.page.close()
 
     """
-        等待
+        等待 TODO 等待是否需要单独写一个类，公用等待方法
     """
 
     def wait_loaded(self, status: str = "complete", timeout: int = None):
         """
         等待页面加载完成
 
         :param status: 可选 interactive、complete
@@ -414,18 +415,26 @@
         dom_read_states = ["interactive", "complete"]
         if status not in dom_read_states:
             status = "complete"
 
         # 加载等待
         start_time = time.time()
         while time.time() - start_time < timeout:
-            dom_status = self.ready_state
+            try:
+                dom_status = self.eval_js(js="document.readyState", raise_err=True)[-1]
+            except errors.CDPConnClosed:
+                return
+
             if dom_status == status or dom_status == "complete":
                 self.__loading = False
                 return
+
+            if self.cdp.closed():
+                break
+
             time.sleep(0.1)
 
     def wait_for_selector(
             self,
             selector: str,
             node_id: int = None,
             timeout: int = None,
@@ -439,19 +448,26 @@
         :param selector:
         :param raise_err:
         :return:
         """
         timeout = timeout or self._opts.timeout
 
         start_time = time.time()
-
         while time.time() - start_time < timeout:
-            ele = self.query_selector(selector=selector, node_id=node_id)
+            try:
+                ele = self.query_selector(selector=selector, node_id=node_id, raise_err=True)
+            except errors.CDPConnClosed:
+                return
+
             if ele:
                 return ele
+
+            if self.cdp.closed():
+                break
+
             time.sleep(0.1)
 
         if raise_err:
             raise errors.ElementWaitTimeout(selector)
 
     def wait_for_selectors(
             self,
@@ -471,26 +487,74 @@
         """
         timeout = timeout or self._opts.timeout
 
         start_time = time.time()
 
         while time.time() - start_time < timeout:
             for s in selectors:
-                ele = self.query_selector(selector=s, node_id=node_id)
+                try:
+                    ele = self.query_selector(selector=s, node_id=node_id, raise_err=True)
+                except errors.CDPConnClosed:
+                    return
+
                 if ele:
                     return ele
 
-                if time.time() - start_time >= timeout:
+                if self.cdp.closed():
                     break
 
             time.sleep(0.1)
 
         if raise_err:
             raise errors.ElementWaitTimeout(selectors)
 
+    def wait_for_url(
+            self,
+            url: str,
+            is_regex: bool = True,
+            timeout: int = None,
+            raise_err: bool = False
+    ) -> Union[Request, None]:
+        """
+        等待直到某个 url 出现
+
+        :param url: 待匹配的 url
+        :param is_regex: 是否正则匹配，不是那就用包含关系（in 匹配）
+        :param timeout: 等待超时时间
+        :param raise_err: 是否报错
+        :return:
+        """
+        is_show = False
+        result_req: Request = None  # type:ignore
+
+        # 请求回调
+        def callback(req: Request):
+            nonlocal is_show, result_req
+            is_show = True
+            result_req = req
+            print("出结果啦：", req)
+
+        # 请求监听
+        self.listen.request_on_url(url=url, callback=callback, is_regex=is_regex)
+
+        timeout = timeout or self._opts.timeout
+        start_time = time.time()
+        while time.time() - start_time < timeout:
+            if is_show:
+                return result_req
+            elif self.cdp.closed():
+                break
+
+            time.sleep(0.1)
+
+        if raise_err:
+            raise errors.UrlWaitTimeout(url)
+
+        return None
+
     """
         访问属性
     """
 
     @property
     def user_agent(self) -> str:
         """
```

### Comparing `EasyPage-0.0.7/easypage/errors.py` & `EasyPage-0.0.8/easypage/errors.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,25 +33,30 @@
 
 # 接收到的消息有错误时触发
 class CDPRecvErrorMsg(Exception):
     def __init__(self, msg: str):
         super().__init__("接收到错误消息：{}".format(msg))
 
 
-class CDPRecvTimeout(Exception):
-    def __init__(self, msg: dict):
-        super().__init__("接收消息超时：{}".format(msg))
+class ElementNotFound(Exception):
+    def __init__(self, ele: str):
+        super().__init__("没有找到元素：{}".format(ele))
 
 
 """
-    Element
+    Timeout
 """
 
 
+class CDPRecvTimeout(Exception):
+    def __init__(self, msg: dict):
+        super().__init__("接收消息超时：{}".format(msg))
+
+
 class ElementWaitTimeout(Exception):
     def __init__(self, ele: Union[List[str], str]):
         super().__init__("元素等待超时：{}".format(ele))
 
 
-class ElementNotFound(Exception):
-    def __init__(self, ele: str):
-        super().__init__("没有找到元素：{}".format(ele))
+class UrlWaitTimeout(Exception):
+    def __init__(self, url: str):
+        super().__init__("url 等待超时：{}".format(url))
```

### Comparing `EasyPage-0.0.7/easypage/event_manager.py` & `EasyPage-0.0.8/easypage/event_manager.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 """
     事件管理器
 
     用来管理 enable、disable
+
+    TODO 可以试试装饰器模式
 """
 from threading import Lock
 from easypage.cdp import CDP
 from easypage.logger import logger
 
 
 class EventManager:
```

### Comparing `EasyPage-0.0.7/easypage/listener.py` & `EasyPage-0.0.8/easypage/listener.py`

 * *Files 11% similar despite different names*

```diff
@@ -43,15 +43,15 @@
         self._http_listen_on = True
 
     def request_on_url(self, url: str, callback: Callable, is_regex: bool = True):
         """
         请求监听
 
         :param url: 待匹配的 url
-        :param is_regex: 是否正则匹配
+        :param is_regex: 是否正则匹配，不是那就用包含关系（in 匹配）
         :param callback:
         :return:
         """
         self.__request_listeners[callback] = {
             "url": url,
             "func": callback,
             "is_regex": is_regex
@@ -71,15 +71,15 @@
         self._http_listen_on = True
 
     def response_on_url(self, url: str, callback: Callable, is_regex: bool = True):
         """
         响应监听
 
         :param url: 待匹配的 url
-        :param is_regex: 是否正则匹配
+        :param is_regex: 是否正则匹配，不是那就用包含关系（in 匹配）
         :param callback:
         :return:
         """
         self.__response_listeners[callback] = {
             "url": url,
             "func": callback,
             "is_regex": is_regex
@@ -87,15 +87,15 @@
         self._http_listen_on = True
 
     def response_on_mime_type(self, mime_type: str, callback: Callable, is_regex: bool = True):
         """
         响应监听（根据响应的 mime_type，如：text/html、image/png、application/json）
 
         :param mime_type: 待匹配的 mime_type
-        :param is_regex: 是否正则匹配
+        :param is_regex: 是否正则匹配，不是那就用包含关系（in 匹配）
         :param callback:
         :return:
         """
         self.__response_listeners[callback] = {
             "mime_type": mime_type,
             "func": callback,
             "is_regex": is_regex
@@ -115,15 +115,15 @@
         """
         for func, config in self.__request_listeners.items():
             if "url" in config:
                 is_regex = config["is_regex"]
                 if is_regex:
                     if re.search(config["url"], request.url):
                         func(request)
-                elif config["url"] == request.url:
+                elif config["url"] in request.url:
                     func(request)
             elif "is_regex" not in config:
                 func(request)
 
     def _on_response(self, response: Response, cdp: CDP):
         """
         响应触发
@@ -136,22 +136,22 @@
 
         for func, config in self.__response_listeners.items():
             if "url" in config:
                 is_regex = config["is_regex"]
                 if is_regex:
                     if re.search(config["url"], response.url):
                         run_functions.append(func)
-                elif config["url"] == response.url:
+                elif config["url"] in response.url:
                     run_functions.append(func)
             if "mime_type" in config:
                 is_regex = config["is_regex"]
                 if is_regex:
                     if re.search(config["mime_type"], response.mime_type):
                         run_functions.append(func)
-                elif config["mime_type"] == response.mime_type:
+                elif config["mime_type"] in response.mime_type:
                     run_functions.append(func)
             elif "is_regex" not in config:
                 run_functions.append(func)
 
         # 判断要不要处理
         if len(run_functions) == 0:
             return
```

### Comparing `EasyPage-0.0.7/easypage/logger.py` & `EasyPage-0.0.8/easypage/logger.py`

 * *Files identical despite different names*

### Comparing `EasyPage-0.0.7/easypage/main.py` & `EasyPage-0.0.8/easypage/main.py`

 * *Files identical despite different names*

### Comparing `EasyPage-0.0.7/easypage/operate.py` & `EasyPage-0.0.8/easypage/operate.py`

 * *Files identical despite different names*

### Comparing `EasyPage-0.0.7/easypage/options.py` & `EasyPage-0.0.8/easypage/options.py`

 * *Files identical despite different names*

### Comparing `EasyPage-0.0.7/easypage/request.py` & `EasyPage-0.0.8/easypage/request.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 from urllib import parse
 
 
 class Request:
     def __init__(self, data: dict):
         self.request_id = data["requestId"]
-        self.frame_id = data["frameId"]
+        self.frame_id = data.get("frameId", "")
         self.resource_type = data["resourceType"] if "resourceType" in data else data["type"]
         self._request = data["request"]
         self._url_parse = parse.urlparse(self._request["url"])
 
     @property
     def url(self) -> str:
         return self._request["url"]
```

### Comparing `EasyPage-0.0.7/easypage/response.py` & `EasyPage-0.0.8/easypage/response.py`

 * *Files identical despite different names*

### Comparing `EasyPage-0.0.7/easypage/settings.py` & `EasyPage-0.0.8/easypage/settings.py`

 * *Files identical despite different names*

### Comparing `EasyPage-0.0.7/easypage/utils/browser_utils.py` & `EasyPage-0.0.8/easypage/utils/browser_utils.py`

 * *Files identical despite different names*

### Comparing `EasyPage-0.0.7/easypage/utils/other_utils.py` & `EasyPage-0.0.8/easypage/utils/other_utils.py`

 * *Files identical despite different names*

### Comparing `EasyPage-0.0.7/setup.py` & `EasyPage-0.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='EasyPage',
-    version='0.0.7',
+    version='0.0.8',
     author='leviathangk',
     author_email='1015295213@qq.com',
     description='基于 CDP 协议，简洁快速的浏览器控制 API',
     keywords=['EasyPage', 'page', 'browser'],
     packages=find_packages(),
     install_requires=[
         "lxml",
```

