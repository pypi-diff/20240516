# Comparing `tmp/EasyPage-0.0.6.tar.gz` & `tmp/EasyPage-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "EasyPage-0.0.6.tar", last modified: Wed May 15 06:41:51 2024, max compression
+gzip compressed data, was "EasyPage-0.0.7.tar", last modified: Thu May 16 03:42:47 2024, max compression
```

## Comparing `EasyPage-0.0.6.tar` & `EasyPage-0.0.7.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxrwxrwx   0        0        0        0 2024-05-15 06:41:51.862573 EasyPage-0.0.6/
-drwxrwxrwx   0        0        0        0 2024-05-15 06:41:51.552459 EasyPage-0.0.6/EasyPage.egg-info/
--rw-rw-rw-   0        0        0      286 2024-05-15 06:41:51.000000 EasyPage-0.0.6/EasyPage.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1060 2024-05-15 06:41:51.000000 EasyPage-0.0.6/EasyPage.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-15 06:41:51.000000 EasyPage-0.0.6/EasyPage.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       76 2024-05-15 06:41:51.000000 EasyPage-0.0.6/EasyPage.egg-info/requires.txt
--rw-rw-rw-   0        0        0       24 2024-05-15 06:41:51.000000 EasyPage-0.0.6/EasyPage.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      286 2024-05-15 06:41:51.861574 EasyPage-0.0.6/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-15 06:41:51.677772 EasyPage-0.0.6/easypage/
--rw-rw-rw-   0        0        0      177 2024-05-09 12:16:34.000000 EasyPage-0.0.6/easypage/__init__.py
--rw-rw-rw-   0        0        0     3349 2024-05-13 03:04:45.000000 EasyPage-0.0.6/easypage/cdp.py
-drwxrwxrwx   0        0        0        0 2024-05-15 06:41:51.792245 EasyPage-0.0.6/easypage/cdp_method/
--rw-rw-rw-   0        0        0        0 2024-04-17 12:56:48.000000 EasyPage-0.0.6/easypage/cdp_method/__init__.py
--rw-rw-rw-   0        0        0     1536 2024-04-24 09:10:40.000000 EasyPage-0.0.6/easypage/cdp_method/browser.py
--rw-rw-rw-   0        0        0     1962 2024-05-13 03:08:12.000000 EasyPage-0.0.6/easypage/cdp_method/css.py
--rw-rw-rw-   0        0        0    12414 2024-05-13 03:01:05.000000 EasyPage-0.0.6/easypage/cdp_method/dom.py
--rw-rw-rw-   0        0        0     1049 2024-04-24 08:57:22.000000 EasyPage-0.0.6/easypage/cdp_method/emulation.py
--rw-rw-rw-   0        0        0     9545 2024-04-24 14:05:55.000000 EasyPage-0.0.6/easypage/cdp_method/fetch.py
--rw-rw-rw-   0        0        0     2654 2024-04-24 09:06:00.000000 EasyPage-0.0.6/easypage/cdp_method/input.py
--rw-rw-rw-   0        0        0     4467 2024-05-07 11:18:55.000000 EasyPage-0.0.6/easypage/cdp_method/network.py
--rw-rw-rw-   0        0        0     5659 2024-04-24 09:12:45.000000 EasyPage-0.0.6/easypage/cdp_method/page.py
--rw-rw-rw-   0        0        0     3667 2024-04-24 09:16:01.000000 EasyPage-0.0.6/easypage/cdp_method/runtime.py
--rw-rw-rw-   0        0        0     2354 2024-04-24 09:16:01.000000 EasyPage-0.0.6/easypage/cdp_method/security.py
--rw-rw-rw-   0        0        0     1322 2024-04-24 09:16:01.000000 EasyPage-0.0.6/easypage/cdp_method/storage.py
--rw-rw-rw-   0        0        0     5884 2024-04-24 13:35:04.000000 EasyPage-0.0.6/easypage/cdp_method/target.py
--rw-rw-rw-   0        0        0    17686 2024-05-10 01:15:20.000000 EasyPage-0.0.6/easypage/conn.py
--rw-rw-rw-   0        0        0      391 2024-04-25 02:28:17.000000 EasyPage-0.0.6/easypage/definition.py
-drwxrwxrwx   0        0        0        0 2024-05-15 06:41:51.834280 EasyPage-0.0.6/easypage/driver/
--rw-rw-rw-   0        0        0        0 2024-04-09 06:15:36.000000 EasyPage-0.0.6/easypage/driver/__init__.py
--rw-rw-rw-   0        0        0     7785 2024-05-14 01:38:27.000000 EasyPage-0.0.6/easypage/driver/browser.py
--rw-rw-rw-   0        0        0      928 2024-05-09 09:58:08.000000 EasyPage-0.0.6/easypage/driver/driver.py
--rw-rw-rw-   0        0        0    41008 2024-05-15 02:10:31.000000 EasyPage-0.0.6/easypage/driver/page.py
--rw-rw-rw-   0        0        0     1462 2024-04-24 08:29:43.000000 EasyPage-0.0.6/easypage/errors.py
--rw-rw-rw-   0        0        0     2097 2024-05-14 03:49:35.000000 EasyPage-0.0.6/easypage/event_manager.py
--rw-rw-rw-   0        0        0     5762 2024-05-11 02:30:56.000000 EasyPage-0.0.6/easypage/listener.py
--rw-rw-rw-   0        0        0     2093 2024-05-09 07:29:23.000000 EasyPage-0.0.6/easypage/logger.py
--rw-rw-rw-   0        0        0     4580 2024-05-14 01:35:01.000000 EasyPage-0.0.6/easypage/main.py
--rw-rw-rw-   0        0        0     4106 2024-04-25 08:20:54.000000 EasyPage-0.0.6/easypage/operate.py
--rw-rw-rw-   0        0        0    10944 2024-04-24 08:39:28.000000 EasyPage-0.0.6/easypage/options.py
--rw-rw-rw-   0        0        0     1805 2024-05-10 01:35:17.000000 EasyPage-0.0.6/easypage/request.py
--rw-rw-rw-   0        0        0     4390 2024-05-10 01:15:20.000000 EasyPage-0.0.6/easypage/response.py
--rw-rw-rw-   0        0        0     2787 2024-05-15 02:22:54.000000 EasyPage-0.0.6/easypage/settings.py
-drwxrwxrwx   0        0        0        0 2024-05-15 06:41:51.851602 EasyPage-0.0.6/easypage/utils/
--rw-rw-rw-   0        0        0        0 2024-04-09 06:15:42.000000 EasyPage-0.0.6/easypage/utils/__init__.py
--rw-rw-rw-   0        0        0     3708 2024-04-10 01:27:44.000000 EasyPage-0.0.6/easypage/utils/browser_utils.py
--rw-rw-rw-   0        0        0     2182 2024-05-09 08:03:26.000000 EasyPage-0.0.6/easypage/utils/other_utils.py
-drwxrwxrwx   0        0        0        0 2024-05-15 06:41:51.860572 EasyPage-0.0.6/easypage_async/
--rw-rw-rw-   0        0        0       40 2024-05-14 06:22:35.000000 EasyPage-0.0.6/easypage_async/__init__.py
--rw-rw-rw-   0        0        0       42 2024-05-15 06:41:51.862573 EasyPage-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0      599 2024-05-15 06:41:48.000000 EasyPage-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-16 03:42:47.147691 EasyPage-0.0.7/
+drwxrwxrwx   0        0        0        0 2024-05-16 03:42:46.811139 EasyPage-0.0.7/EasyPage.egg-info/
+-rw-rw-rw-   0        0        0      286 2024-05-16 03:42:46.000000 EasyPage-0.0.7/EasyPage.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1060 2024-05-16 03:42:46.000000 EasyPage-0.0.7/EasyPage.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-16 03:42:46.000000 EasyPage-0.0.7/EasyPage.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       76 2024-05-16 03:42:46.000000 EasyPage-0.0.7/EasyPage.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       24 2024-05-16 03:42:46.000000 EasyPage-0.0.7/EasyPage.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      286 2024-05-16 03:42:47.147691 EasyPage-0.0.7/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-16 03:42:46.946177 EasyPage-0.0.7/easypage/
+-rw-rw-rw-   0        0        0      192 2024-05-16 02:17:32.000000 EasyPage-0.0.7/easypage/__init__.py
+-rw-rw-rw-   0        0        0     3349 2024-05-13 03:04:45.000000 EasyPage-0.0.7/easypage/cdp.py
+drwxrwxrwx   0        0        0        0 2024-05-16 03:42:47.072289 EasyPage-0.0.7/easypage/cdp_method/
+-rw-rw-rw-   0        0        0        0 2024-04-17 12:56:48.000000 EasyPage-0.0.7/easypage/cdp_method/__init__.py
+-rw-rw-rw-   0        0        0     1536 2024-04-24 09:10:40.000000 EasyPage-0.0.7/easypage/cdp_method/browser.py
+-rw-rw-rw-   0        0        0     1962 2024-05-13 03:08:12.000000 EasyPage-0.0.7/easypage/cdp_method/css.py
+-rw-rw-rw-   0        0        0    12414 2024-05-13 03:01:05.000000 EasyPage-0.0.7/easypage/cdp_method/dom.py
+-rw-rw-rw-   0        0        0     1049 2024-04-24 08:57:22.000000 EasyPage-0.0.7/easypage/cdp_method/emulation.py
+-rw-rw-rw-   0        0        0     9545 2024-04-24 14:05:55.000000 EasyPage-0.0.7/easypage/cdp_method/fetch.py
+-rw-rw-rw-   0        0        0     2654 2024-04-24 09:06:00.000000 EasyPage-0.0.7/easypage/cdp_method/input.py
+-rw-rw-rw-   0        0        0     4467 2024-05-07 11:18:55.000000 EasyPage-0.0.7/easypage/cdp_method/network.py
+-rw-rw-rw-   0        0        0     8620 2024-05-16 02:51:16.000000 EasyPage-0.0.7/easypage/cdp_method/page.py
+-rw-rw-rw-   0        0        0     3667 2024-04-24 09:16:01.000000 EasyPage-0.0.7/easypage/cdp_method/runtime.py
+-rw-rw-rw-   0        0        0     2354 2024-04-24 09:16:01.000000 EasyPage-0.0.7/easypage/cdp_method/security.py
+-rw-rw-rw-   0        0        0     1322 2024-04-24 09:16:01.000000 EasyPage-0.0.7/easypage/cdp_method/storage.py
+-rw-rw-rw-   0        0        0     5884 2024-04-24 13:35:04.000000 EasyPage-0.0.7/easypage/cdp_method/target.py
+-rw-rw-rw-   0        0        0    17770 2024-05-16 03:42:29.000000 EasyPage-0.0.7/easypage/conn.py
+-rw-rw-rw-   0        0        0      391 2024-04-25 02:28:17.000000 EasyPage-0.0.7/easypage/definition.py
+drwxrwxrwx   0        0        0        0 2024-05-16 03:42:47.128698 EasyPage-0.0.7/easypage/driver/
+-rw-rw-rw-   0        0        0        0 2024-04-09 06:15:36.000000 EasyPage-0.0.7/easypage/driver/__init__.py
+-rw-rw-rw-   0        0        0     7785 2024-05-14 01:38:27.000000 EasyPage-0.0.7/easypage/driver/browser.py
+-rw-rw-rw-   0        0        0      928 2024-05-09 09:58:08.000000 EasyPage-0.0.7/easypage/driver/driver.py
+-rw-rw-rw-   0        0        0    43065 2024-05-16 03:05:30.000000 EasyPage-0.0.7/easypage/driver/page.py
+-rw-rw-rw-   0        0        0     1462 2024-04-24 08:29:43.000000 EasyPage-0.0.7/easypage/errors.py
+-rw-rw-rw-   0        0        0     2097 2024-05-14 03:49:35.000000 EasyPage-0.0.7/easypage/event_manager.py
+-rw-rw-rw-   0        0        0     5762 2024-05-11 02:30:56.000000 EasyPage-0.0.7/easypage/listener.py
+-rw-rw-rw-   0        0        0     2093 2024-05-09 07:29:23.000000 EasyPage-0.0.7/easypage/logger.py
+-rw-rw-rw-   0        0        0     4580 2024-05-14 01:35:01.000000 EasyPage-0.0.7/easypage/main.py
+-rw-rw-rw-   0        0        0     4106 2024-04-25 08:20:54.000000 EasyPage-0.0.7/easypage/operate.py
+-rw-rw-rw-   0        0        0    10944 2024-04-24 08:39:28.000000 EasyPage-0.0.7/easypage/options.py
+-rw-rw-rw-   0        0        0     1805 2024-05-10 01:35:17.000000 EasyPage-0.0.7/easypage/request.py
+-rw-rw-rw-   0        0        0     4390 2024-05-10 01:15:20.000000 EasyPage-0.0.7/easypage/response.py
+-rw-rw-rw-   0        0        0     2787 2024-05-15 02:22:54.000000 EasyPage-0.0.7/easypage/settings.py
+drwxrwxrwx   0        0        0        0 2024-05-16 03:42:47.137690 EasyPage-0.0.7/easypage/utils/
+-rw-rw-rw-   0        0        0        0 2024-04-09 06:15:42.000000 EasyPage-0.0.7/easypage/utils/__init__.py
+-rw-rw-rw-   0        0        0     3708 2024-04-10 01:27:44.000000 EasyPage-0.0.7/easypage/utils/browser_utils.py
+-rw-rw-rw-   0        0        0     2182 2024-05-09 08:03:26.000000 EasyPage-0.0.7/easypage/utils/other_utils.py
+drwxrwxrwx   0        0        0        0 2024-05-16 03:42:47.146690 EasyPage-0.0.7/easypage_async/
+-rw-rw-rw-   0        0        0       40 2024-05-14 06:22:35.000000 EasyPage-0.0.7/easypage_async/__init__.py
+-rw-rw-rw-   0        0        0       42 2024-05-16 03:42:47.147691 EasyPage-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0      599 2024-05-16 03:42:07.000000 EasyPage-0.0.7/setup.py
```

### Comparing `EasyPage-0.0.6/EasyPage.egg-info/SOURCES.txt` & `EasyPage-0.0.7/EasyPage.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `EasyPage-0.0.6/easypage/cdp.py` & `EasyPage-0.0.7/easypage/cdp.py`

 * *Files identical despite different names*

### Comparing `EasyPage-0.0.6/easypage/cdp_method/browser.py` & `EasyPage-0.0.7/easypage/cdp_method/browser.py`

 * *Files identical despite different names*

### Comparing `EasyPage-0.0.6/easypage/cdp_method/css.py` & `EasyPage-0.0.7/easypage/cdp_method/css.py`

 * *Files identical despite different names*

### Comparing `EasyPage-0.0.6/easypage/cdp_method/dom.py` & `EasyPage-0.0.7/easypage/cdp_method/dom.py`

 * *Files identical despite different names*

### Comparing `EasyPage-0.0.6/easypage/cdp_method/emulation.py` & `EasyPage-0.0.7/easypage/cdp_method/emulation.py`

 * *Files identical despite different names*

### Comparing `EasyPage-0.0.6/easypage/cdp_method/fetch.py` & `EasyPage-0.0.7/easypage/cdp_method/fetch.py`

 * *Files identical despite different names*

### Comparing `EasyPage-0.0.6/easypage/cdp_method/input.py` & `EasyPage-0.0.7/easypage/cdp_method/input.py`

 * *Files identical despite different names*

### Comparing `EasyPage-0.0.6/easypage/cdp_method/network.py` & `EasyPage-0.0.7/easypage/cdp_method/network.py`

 * *Files identical despite different names*

### Comparing `EasyPage-0.0.6/easypage/cdp_method/page.py` & `EasyPage-0.0.7/easypage/cdp_method/page.py`

 * *Files 16% similar despite different names*

```diff
@@ -30,14 +30,93 @@
         """
         return self.__conn.send(
             method="Page.enable",
             raise_err=raise_err,
             need_callback=need_callback,
         )
 
+    def reload(
+            self,
+            ignore_cache: bool = False,
+            scrip_to_evaluate_onload: str = None,
+            raise_err: bool = False,
+            need_callback: bool = False,
+    ) -> Tuple[bool, dict]:
+        """
+        刷新页面
+
+        https://chromedevtools.github.io/devtools-protocol/tot/Page/#method-reload
+
+        :param ignore_cache: 是否忽略浏览器缓存(所有资源都会重新加载)
+        :param scrip_to_evaluate_onload：注入的脚本（origin 变了就不会注入了）
+        :param raise_err: 接收到错误消息时，是否抛出，默认为 False
+        :param need_callback: 接收到消息时，是否返回，默认为 True
+        :return:
+        """
+        return self.__conn.send(
+            method="Page.enable",
+            params={
+                "ignoreCache": ignore_cache,
+                "scriptToEvaluateOnLoad": scrip_to_evaluate_onload,
+            },
+            raise_err=raise_err,
+            need_callback=need_callback,
+        )
+
+    def stop_loading(
+            self,
+            raise_err: bool = False,
+            need_callback: bool = False,
+    ) -> Tuple[bool, dict]:
+        """
+        停止页面加载（强制页面停止所有导航和挂起的资源提取）
+
+        https://chromedevtools.github.io/devtools-protocol/tot/Page/#method-stopLoading
+
+        :param raise_err: 接收到错误消息时，是否抛出，默认为 False
+        :param need_callback: 接收到消息时，是否返回，默认为 True
+        :return:
+        """
+        return self.__conn.send(
+            method="Page.stopLoading",
+            raise_err=raise_err,
+            need_callback=need_callback,
+        )
+
+    def add_script_to_evaluate_on_new_document(
+            self,
+            source: str,
+            run_immediately: bool = False,
+            raise_err: bool = False,
+            need_callback: bool = False,
+    ) -> Tuple[bool, dict]:
+        """
+        每次加载新文档时执行脚本（在页面所有 scripts 执行之前执行，可以用作 hook 之类）
+
+        https://chromedevtools.github.io/devtools-protocol/tot/Page/#method-addScriptToEvaluateOnNewDocument
+
+        :param source: 执行的脚本
+        :param run_immediately: 是否立即执行（否的话只在新文档加载时执行）
+        :param raise_err: 接收到错误消息时，是否抛出，默认为 False
+        :param need_callback: 接收到消息时，是否返回，默认为 True
+        :return:
+        """
+        send_data = {
+            "source": source,
+        }
+        if run_immediately:
+            send_data["runImmediately"] = run_immediately
+
+        return self.__conn.send(
+            method="Page.addScriptToEvaluateOnNewDocument",
+            params=send_data,
+            raise_err=raise_err,
+            need_callback=need_callback,
+        )
+
     def navigate(
             self,
             url: str,
             frame_id: str = None,
             ignore_url_check: bool = False,
             raise_err: bool = False,
             need_callback: bool = True,
```

### Comparing `EasyPage-0.0.6/easypage/cdp_method/runtime.py` & `EasyPage-0.0.7/easypage/cdp_method/runtime.py`

 * *Files identical despite different names*

### Comparing `EasyPage-0.0.6/easypage/cdp_method/security.py` & `EasyPage-0.0.7/easypage/cdp_method/security.py`

 * *Files identical despite different names*

### Comparing `EasyPage-0.0.6/easypage/cdp_method/storage.py` & `EasyPage-0.0.7/easypage/cdp_method/storage.py`

 * *Files identical despite different names*

### Comparing `EasyPage-0.0.6/easypage/cdp_method/target.py` & `EasyPage-0.0.7/easypage/cdp_method/target.py`

 * *Files identical despite different names*

### Comparing `EasyPage-0.0.6/easypage/conn.py` & `EasyPage-0.0.7/easypage/conn.py`

 * *Files 1% similar despite different names*

```diff
@@ -412,20 +412,21 @@
         # 发送信息
         try:
             self.__ws.send(msg_json)
             return True, msg
         except (errors.CDPRecvTimeout, errors.CDPRecvErrorMsg):
             raise
         except (websocket.WebSocketConnectionClosedException, ConnectionResetError):
-            logger.warning("连接已断开：{}", self.driver_url)
+            # logger.warning("连接已断开：{}", self.driver_url)
+            raise errors.CDPConnClosed(f"连接已断开：{self.driver_url}")
         except:
             traceback.print_exc()
             raise
 
-        return False, dict()
+        # return False, dict()
 
     def __recv_result(self):
         """
         接收消息、事件处理
 
         :return:
         """
```

### Comparing `EasyPage-0.0.6/easypage/driver/browser.py` & `EasyPage-0.0.7/easypage/driver/browser.py`

 * *Files identical despite different names*

### Comparing `EasyPage-0.0.6/easypage/driver/driver.py` & `EasyPage-0.0.7/easypage/driver/driver.py`

 * *Files identical despite different names*

### Comparing `EasyPage-0.0.6/easypage/driver/page.py` & `EasyPage-0.0.7/easypage/driver/page.py`

 * *Files 2% similar despite different names*

```diff
@@ -340,14 +340,58 @@
                 save_path = save_path.with_suffix(".png")
 
             with open(save_path, "wb") as f:
                 f.write(data_bytes)
 
         return data_bytes
 
+    def reload(
+            self,
+            ignore_cache: bool = False,
+            scrip_to_evaluate_onload: str = None,
+            raise_err: bool = False,
+            need_callback: bool = False,
+    ) -> Tuple[bool, dict]:
+        """
+        刷新页面
+
+        https://chromedevtools.github.io/devtools-protocol/tot/Page/#method-reload
+
+        :param ignore_cache: 是否忽略浏览器缓存(所有资源都会重新加载)
+        :param scrip_to_evaluate_onload：注入的脚本（origin 变了就不会注入了）
+        :param raise_err: 接收到错误消息时，是否抛出，默认为 False
+        :param need_callback: 接收到消息时，是否返回，默认为 True
+        :return:
+        """
+        return self.cdp.page.reload(
+            ignore_cache=ignore_cache,
+            scrip_to_evaluate_onload=scrip_to_evaluate_onload,
+            raise_err=raise_err,
+            need_callback=need_callback
+        )
+
+    def stop_loading(
+            self,
+            raise_err: bool = False,
+            need_callback: bool = False,
+    ) -> Tuple[bool, dict]:
+        """
+        停止页面加载（强制页面停止所有导航和挂起的资源提取）
+
+        https://chromedevtools.github.io/devtools-protocol/tot/Page/#method-stopLoading
+
+        :param raise_err: 接收到错误消息时，是否抛出，默认为 False
+        :param need_callback: 接收到消息时，是否返回，默认为 True
+        :return:
+        """
+        return self.cdp.page.stop_loading(
+            raise_err=raise_err,
+            need_callback=need_callback,
+        )
+
     def close(self):
         """
         关闭当前页面
 
         :return:
         """
         self.cdp.page.close()
@@ -370,15 +414,15 @@
         dom_read_states = ["interactive", "complete"]
         if status not in dom_read_states:
             status = "complete"
 
         # 加载等待
         start_time = time.time()
         while time.time() - start_time < timeout:
-            dom_status = self.eval_js(js="document.readyState")[-1]
+            dom_status = self.ready_state
             if dom_status == status or dom_status == "complete":
                 self.__loading = False
                 return
             time.sleep(0.1)
 
     def wait_for_selector(
             self,
@@ -444,14 +488,35 @@
             raise errors.ElementWaitTimeout(selectors)
 
     """
         访问属性
     """
 
     @property
+    def user_agent(self) -> str:
+        """
+        返回 ua
+
+        :return:
+        """
+        status, data = self.cdp.browser.version()
+        if not status:
+            return ""
+        return data["userAgent"]
+
+    @property
+    def ready_state(self) -> str:
+        """
+        页面加载状态
+
+        :return:
+        """
+        return self.eval_js(js="document.readyState")[-1]
+
+    @property
     def url(self) -> str:
         """
         当前页面的 url
 
         :return:
         """
         status, root = self.cdp.dom.get_document()
```

### Comparing `EasyPage-0.0.6/easypage/errors.py` & `EasyPage-0.0.7/easypage/errors.py`

 * *Files identical despite different names*

### Comparing `EasyPage-0.0.6/easypage/event_manager.py` & `EasyPage-0.0.7/easypage/event_manager.py`

 * *Files identical despite different names*

### Comparing `EasyPage-0.0.6/easypage/listener.py` & `EasyPage-0.0.7/easypage/listener.py`

 * *Files identical despite different names*

### Comparing `EasyPage-0.0.6/easypage/logger.py` & `EasyPage-0.0.7/easypage/logger.py`

 * *Files identical despite different names*

### Comparing `EasyPage-0.0.6/easypage/main.py` & `EasyPage-0.0.7/easypage/main.py`

 * *Files identical despite different names*

### Comparing `EasyPage-0.0.6/easypage/operate.py` & `EasyPage-0.0.7/easypage/operate.py`

 * *Files identical despite different names*

### Comparing `EasyPage-0.0.6/easypage/options.py` & `EasyPage-0.0.7/easypage/options.py`

 * *Files identical despite different names*

### Comparing `EasyPage-0.0.6/easypage/request.py` & `EasyPage-0.0.7/easypage/request.py`

 * *Files identical despite different names*

### Comparing `EasyPage-0.0.6/easypage/response.py` & `EasyPage-0.0.7/easypage/response.py`

 * *Files identical despite different names*

### Comparing `EasyPage-0.0.6/easypage/settings.py` & `EasyPage-0.0.7/easypage/settings.py`

 * *Files identical despite different names*

### Comparing `EasyPage-0.0.6/easypage/utils/browser_utils.py` & `EasyPage-0.0.7/easypage/utils/browser_utils.py`

 * *Files identical despite different names*

### Comparing `EasyPage-0.0.6/easypage/utils/other_utils.py` & `EasyPage-0.0.7/easypage/utils/other_utils.py`

 * *Files identical despite different names*

### Comparing `EasyPage-0.0.6/setup.py` & `EasyPage-0.0.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='EasyPage',
-    version='0.0.6',
+    version='0.0.7',
     author='leviathangk',
     author_email='1015295213@qq.com',
     description='基于 CDP 协议，简洁快速的浏览器控制 API',
     keywords=['EasyPage', 'page', 'browser'],
     packages=find_packages(),
     install_requires=[
         "lxml",
```

