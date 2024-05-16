# Comparing `tmp/EasyPage-0.0.5.tar.gz` & `tmp/EasyPage-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "EasyPage-0.0.5.tar", last modified: Sat May 11 02:36:28 2024, max compression
+gzip compressed data, was "EasyPage-0.0.6.tar", last modified: Wed May 15 06:41:51 2024, max compression
```

## Comparing `EasyPage-0.0.5.tar` & `EasyPage-0.0.6.tar`

### file list

```diff
@@ -1,46 +1,50 @@
-drwxrwxrwx   0        0        0        0 2024-05-11 02:36:28.112760 EasyPage-0.0.5/
-drwxrwxrwx   0        0        0        0 2024-05-11 02:36:27.884188 EasyPage-0.0.5/EasyPage.egg-info/
--rw-rw-rw-   0        0        0      286 2024-05-11 02:36:27.000000 EasyPage-0.0.5/EasyPage.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      980 2024-05-11 02:36:27.000000 EasyPage-0.0.5/EasyPage.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-11 02:36:27.000000 EasyPage-0.0.5/EasyPage.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       76 2024-05-11 02:36:27.000000 EasyPage-0.0.5/EasyPage.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-05-11 02:36:27.000000 EasyPage-0.0.5/EasyPage.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      286 2024-05-11 02:36:28.111759 EasyPage-0.0.5/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-11 02:36:27.943192 EasyPage-0.0.5/easypage/
--rw-rw-rw-   0        0        0      177 2024-05-09 12:16:34.000000 EasyPage-0.0.5/easypage/__init__.py
--rw-rw-rw-   0        0        0     3231 2024-05-07 14:06:28.000000 EasyPage-0.0.5/easypage/cdp.py
-drwxrwxrwx   0        0        0        0 2024-05-11 02:36:28.083759 EasyPage-0.0.5/easypage/cdp_method/
--rw-rw-rw-   0        0        0        0 2024-04-17 12:56:48.000000 EasyPage-0.0.5/easypage/cdp_method/__init__.py
--rw-rw-rw-   0        0        0     1536 2024-04-24 09:10:40.000000 EasyPage-0.0.5/easypage/cdp_method/browser.py
--rw-rw-rw-   0        0        0    12414 2024-04-24 09:08:35.000000 EasyPage-0.0.5/easypage/cdp_method/dom.py
--rw-rw-rw-   0        0        0     1049 2024-04-24 08:57:22.000000 EasyPage-0.0.5/easypage/cdp_method/emulation.py
--rw-rw-rw-   0        0        0     9545 2024-04-24 14:05:55.000000 EasyPage-0.0.5/easypage/cdp_method/fetch.py
--rw-rw-rw-   0        0        0     2654 2024-04-24 09:06:00.000000 EasyPage-0.0.5/easypage/cdp_method/input.py
--rw-rw-rw-   0        0        0     4467 2024-05-07 11:18:55.000000 EasyPage-0.0.5/easypage/cdp_method/network.py
--rw-rw-rw-   0        0        0     5659 2024-04-24 09:12:45.000000 EasyPage-0.0.5/easypage/cdp_method/page.py
--rw-rw-rw-   0        0        0     3667 2024-04-24 09:16:01.000000 EasyPage-0.0.5/easypage/cdp_method/runtime.py
--rw-rw-rw-   0        0        0     2354 2024-04-24 09:16:01.000000 EasyPage-0.0.5/easypage/cdp_method/security.py
--rw-rw-rw-   0        0        0     1322 2024-04-24 09:16:01.000000 EasyPage-0.0.5/easypage/cdp_method/storage.py
--rw-rw-rw-   0        0        0     5884 2024-04-24 13:35:04.000000 EasyPage-0.0.5/easypage/cdp_method/target.py
--rw-rw-rw-   0        0        0    17686 2024-05-10 01:15:20.000000 EasyPage-0.0.5/easypage/conn.py
--rw-rw-rw-   0        0        0      391 2024-04-25 02:28:17.000000 EasyPage-0.0.5/easypage/definition.py
-drwxrwxrwx   0        0        0        0 2024-05-11 02:36:28.100756 EasyPage-0.0.5/easypage/driver/
--rw-rw-rw-   0        0        0        0 2024-04-09 06:15:36.000000 EasyPage-0.0.5/easypage/driver/__init__.py
--rw-rw-rw-   0        0        0     7794 2024-05-11 02:20:43.000000 EasyPage-0.0.5/easypage/driver/browser.py
--rw-rw-rw-   0        0        0      928 2024-05-09 09:58:08.000000 EasyPage-0.0.5/easypage/driver/driver.py
--rw-rw-rw-   0        0        0    35291 2024-05-11 02:24:38.000000 EasyPage-0.0.5/easypage/driver/page.py
--rw-rw-rw-   0        0        0     1462 2024-04-24 08:29:43.000000 EasyPage-0.0.5/easypage/errors.py
--rw-rw-rw-   0        0        0     5762 2024-05-11 02:30:56.000000 EasyPage-0.0.5/easypage/listener.py
--rw-rw-rw-   0        0        0     2093 2024-05-09 07:29:23.000000 EasyPage-0.0.5/easypage/logger.py
--rw-rw-rw-   0        0        0     4581 2024-05-11 02:18:48.000000 EasyPage-0.0.5/easypage/main.py
--rw-rw-rw-   0        0        0     4106 2024-04-25 08:20:54.000000 EasyPage-0.0.5/easypage/operate.py
--rw-rw-rw-   0        0        0    10944 2024-04-24 08:39:28.000000 EasyPage-0.0.5/easypage/options.py
--rw-rw-rw-   0        0        0     1805 2024-05-10 01:35:17.000000 EasyPage-0.0.5/easypage/request.py
--rw-rw-rw-   0        0        0     4390 2024-05-10 01:15:20.000000 EasyPage-0.0.5/easypage/response.py
--rw-rw-rw-   0        0        0     2787 2024-04-22 08:05:28.000000 EasyPage-0.0.5/easypage/settings.py
-drwxrwxrwx   0        0        0        0 2024-05-11 02:36:28.109756 EasyPage-0.0.5/easypage/utils/
--rw-rw-rw-   0        0        0        0 2024-04-09 06:15:42.000000 EasyPage-0.0.5/easypage/utils/__init__.py
--rw-rw-rw-   0        0        0     3708 2024-04-10 01:27:44.000000 EasyPage-0.0.5/easypage/utils/browser_utils.py
--rw-rw-rw-   0        0        0     2182 2024-05-09 08:03:26.000000 EasyPage-0.0.5/easypage/utils/other_utils.py
--rw-rw-rw-   0        0        0       42 2024-05-11 02:36:28.112760 EasyPage-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0      599 2024-05-11 02:36:10.000000 EasyPage-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-15 06:41:51.862573 EasyPage-0.0.6/
+drwxrwxrwx   0        0        0        0 2024-05-15 06:41:51.552459 EasyPage-0.0.6/EasyPage.egg-info/
+-rw-rw-rw-   0        0        0      286 2024-05-15 06:41:51.000000 EasyPage-0.0.6/EasyPage.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1060 2024-05-15 06:41:51.000000 EasyPage-0.0.6/EasyPage.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-15 06:41:51.000000 EasyPage-0.0.6/EasyPage.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       76 2024-05-15 06:41:51.000000 EasyPage-0.0.6/EasyPage.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       24 2024-05-15 06:41:51.000000 EasyPage-0.0.6/EasyPage.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      286 2024-05-15 06:41:51.861574 EasyPage-0.0.6/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-15 06:41:51.677772 EasyPage-0.0.6/easypage/
+-rw-rw-rw-   0        0        0      177 2024-05-09 12:16:34.000000 EasyPage-0.0.6/easypage/__init__.py
+-rw-rw-rw-   0        0        0     3349 2024-05-13 03:04:45.000000 EasyPage-0.0.6/easypage/cdp.py
+drwxrwxrwx   0        0        0        0 2024-05-15 06:41:51.792245 EasyPage-0.0.6/easypage/cdp_method/
+-rw-rw-rw-   0        0        0        0 2024-04-17 12:56:48.000000 EasyPage-0.0.6/easypage/cdp_method/__init__.py
+-rw-rw-rw-   0        0        0     1536 2024-04-24 09:10:40.000000 EasyPage-0.0.6/easypage/cdp_method/browser.py
+-rw-rw-rw-   0        0        0     1962 2024-05-13 03:08:12.000000 EasyPage-0.0.6/easypage/cdp_method/css.py
+-rw-rw-rw-   0        0        0    12414 2024-05-13 03:01:05.000000 EasyPage-0.0.6/easypage/cdp_method/dom.py
+-rw-rw-rw-   0        0        0     1049 2024-04-24 08:57:22.000000 EasyPage-0.0.6/easypage/cdp_method/emulation.py
+-rw-rw-rw-   0        0        0     9545 2024-04-24 14:05:55.000000 EasyPage-0.0.6/easypage/cdp_method/fetch.py
+-rw-rw-rw-   0        0        0     2654 2024-04-24 09:06:00.000000 EasyPage-0.0.6/easypage/cdp_method/input.py
+-rw-rw-rw-   0        0        0     4467 2024-05-07 11:18:55.000000 EasyPage-0.0.6/easypage/cdp_method/network.py
+-rw-rw-rw-   0        0        0     5659 2024-04-24 09:12:45.000000 EasyPage-0.0.6/easypage/cdp_method/page.py
+-rw-rw-rw-   0        0        0     3667 2024-04-24 09:16:01.000000 EasyPage-0.0.6/easypage/cdp_method/runtime.py
+-rw-rw-rw-   0        0        0     2354 2024-04-24 09:16:01.000000 EasyPage-0.0.6/easypage/cdp_method/security.py
+-rw-rw-rw-   0        0        0     1322 2024-04-24 09:16:01.000000 EasyPage-0.0.6/easypage/cdp_method/storage.py
+-rw-rw-rw-   0        0        0     5884 2024-04-24 13:35:04.000000 EasyPage-0.0.6/easypage/cdp_method/target.py
+-rw-rw-rw-   0        0        0    17686 2024-05-10 01:15:20.000000 EasyPage-0.0.6/easypage/conn.py
+-rw-rw-rw-   0        0        0      391 2024-04-25 02:28:17.000000 EasyPage-0.0.6/easypage/definition.py
+drwxrwxrwx   0        0        0        0 2024-05-15 06:41:51.834280 EasyPage-0.0.6/easypage/driver/
+-rw-rw-rw-   0        0        0        0 2024-04-09 06:15:36.000000 EasyPage-0.0.6/easypage/driver/__init__.py
+-rw-rw-rw-   0        0        0     7785 2024-05-14 01:38:27.000000 EasyPage-0.0.6/easypage/driver/browser.py
+-rw-rw-rw-   0        0        0      928 2024-05-09 09:58:08.000000 EasyPage-0.0.6/easypage/driver/driver.py
+-rw-rw-rw-   0        0        0    41008 2024-05-15 02:10:31.000000 EasyPage-0.0.6/easypage/driver/page.py
+-rw-rw-rw-   0        0        0     1462 2024-04-24 08:29:43.000000 EasyPage-0.0.6/easypage/errors.py
+-rw-rw-rw-   0        0        0     2097 2024-05-14 03:49:35.000000 EasyPage-0.0.6/easypage/event_manager.py
+-rw-rw-rw-   0        0        0     5762 2024-05-11 02:30:56.000000 EasyPage-0.0.6/easypage/listener.py
+-rw-rw-rw-   0        0        0     2093 2024-05-09 07:29:23.000000 EasyPage-0.0.6/easypage/logger.py
+-rw-rw-rw-   0        0        0     4580 2024-05-14 01:35:01.000000 EasyPage-0.0.6/easypage/main.py
+-rw-rw-rw-   0        0        0     4106 2024-04-25 08:20:54.000000 EasyPage-0.0.6/easypage/operate.py
+-rw-rw-rw-   0        0        0    10944 2024-04-24 08:39:28.000000 EasyPage-0.0.6/easypage/options.py
+-rw-rw-rw-   0        0        0     1805 2024-05-10 01:35:17.000000 EasyPage-0.0.6/easypage/request.py
+-rw-rw-rw-   0        0        0     4390 2024-05-10 01:15:20.000000 EasyPage-0.0.6/easypage/response.py
+-rw-rw-rw-   0        0        0     2787 2024-05-15 02:22:54.000000 EasyPage-0.0.6/easypage/settings.py
+drwxrwxrwx   0        0        0        0 2024-05-15 06:41:51.851602 EasyPage-0.0.6/easypage/utils/
+-rw-rw-rw-   0        0        0        0 2024-04-09 06:15:42.000000 EasyPage-0.0.6/easypage/utils/__init__.py
+-rw-rw-rw-   0        0        0     3708 2024-04-10 01:27:44.000000 EasyPage-0.0.6/easypage/utils/browser_utils.py
+-rw-rw-rw-   0        0        0     2182 2024-05-09 08:03:26.000000 EasyPage-0.0.6/easypage/utils/other_utils.py
+drwxrwxrwx   0        0        0        0 2024-05-15 06:41:51.860572 EasyPage-0.0.6/easypage_async/
+-rw-rw-rw-   0        0        0       40 2024-05-14 06:22:35.000000 EasyPage-0.0.6/easypage_async/__init__.py
+-rw-rw-rw-   0        0        0       42 2024-05-15 06:41:51.862573 EasyPage-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      599 2024-05-15 06:41:48.000000 EasyPage-0.0.6/setup.py
```

### Comparing `EasyPage-0.0.5/EasyPage.egg-info/SOURCES.txt` & `EasyPage-0.0.6/EasyPage.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -5,24 +5,26 @@
 EasyPage.egg-info/requires.txt
 EasyPage.egg-info/top_level.txt
 easypage/__init__.py
 easypage/cdp.py
 easypage/conn.py
 easypage/definition.py
 easypage/errors.py
+easypage/event_manager.py
 easypage/listener.py
 easypage/logger.py
 easypage/main.py
 easypage/operate.py
 easypage/options.py
 easypage/request.py
 easypage/response.py
 easypage/settings.py
 easypage/cdp_method/__init__.py
 easypage/cdp_method/browser.py
+easypage/cdp_method/css.py
 easypage/cdp_method/dom.py
 easypage/cdp_method/emulation.py
 easypage/cdp_method/fetch.py
 easypage/cdp_method/input.py
 easypage/cdp_method/network.py
 easypage/cdp_method/page.py
 easypage/cdp_method/runtime.py
@@ -31,8 +33,9 @@
 easypage/cdp_method/target.py
 easypage/driver/__init__.py
 easypage/driver/browser.py
 easypage/driver/driver.py
 easypage/driver/page.py
 easypage/utils/__init__.py
 easypage/utils/browser_utils.py
-easypage/utils/other_utils.py
+easypage/utils/other_utils.py
+easypage_async/__init__.py
```

### Comparing `EasyPage-0.0.5/easypage/cdp.py` & `EasyPage-0.0.6/easypage/cdp.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 from easypage.cdp_method.target import Target
 from easypage.cdp_method.network import NetWork
 from easypage.cdp_method.browser import Browser
 from easypage.cdp_method.runtime import Runtime
 from easypage.cdp_method.storage import Storage
 from easypage.cdp_method.security import Security
 from easypage.cdp_method.emulation import Emulation
+from easypage.cdp_method.css import CSS
 
 
 class CDP:
     def __init__(self, conn: Conn):
         self.__conn = conn
 
     def on(self, event: str, callback: typing.Callable):
@@ -115,7 +116,11 @@
     @property
     def network(self) -> NetWork:
         return NetWork(self.__conn)
 
     @property
     def security(self) -> Security:
         return Security(self.__conn)
+
+    @property
+    def css(self) -> CSS:
+        return CSS(self.__conn)
```

### Comparing `EasyPage-0.0.5/easypage/cdp_method/browser.py` & `EasyPage-0.0.6/easypage/cdp_method/browser.py`

 * *Files identical despite different names*

### Comparing `EasyPage-0.0.5/easypage/cdp_method/dom.py` & `EasyPage-0.0.6/easypage/cdp_method/dom.py`

 * *Files identical despite different names*

### Comparing `EasyPage-0.0.5/easypage/cdp_method/emulation.py` & `EasyPage-0.0.6/easypage/cdp_method/emulation.py`

 * *Files identical despite different names*

### Comparing `EasyPage-0.0.5/easypage/cdp_method/fetch.py` & `EasyPage-0.0.6/easypage/cdp_method/fetch.py`

 * *Files identical despite different names*

### Comparing `EasyPage-0.0.5/easypage/cdp_method/input.py` & `EasyPage-0.0.6/easypage/cdp_method/input.py`

 * *Files identical despite different names*

### Comparing `EasyPage-0.0.5/easypage/cdp_method/network.py` & `EasyPage-0.0.6/easypage/cdp_method/network.py`

 * *Files identical despite different names*

### Comparing `EasyPage-0.0.5/easypage/cdp_method/page.py` & `EasyPage-0.0.6/easypage/cdp_method/page.py`

 * *Files identical despite different names*

### Comparing `EasyPage-0.0.5/easypage/cdp_method/runtime.py` & `EasyPage-0.0.6/easypage/cdp_method/runtime.py`

 * *Files identical despite different names*

### Comparing `EasyPage-0.0.5/easypage/cdp_method/security.py` & `EasyPage-0.0.6/easypage/cdp_method/security.py`

 * *Files identical despite different names*

### Comparing `EasyPage-0.0.5/easypage/cdp_method/storage.py` & `EasyPage-0.0.6/easypage/cdp_method/storage.py`

 * *Files identical despite different names*

### Comparing `EasyPage-0.0.5/easypage/cdp_method/target.py` & `EasyPage-0.0.6/easypage/cdp_method/target.py`

 * *Files identical despite different names*

### Comparing `EasyPage-0.0.5/easypage/conn.py` & `EasyPage-0.0.6/easypage/conn.py`

 * *Files identical despite different names*

### Comparing `EasyPage-0.0.5/easypage/driver/browser.py` & `EasyPage-0.0.6/easypage/driver/browser.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,19 +26,19 @@
         :param opts:
         :param driver_id:
         """
         super().__init__(opts, TYPE_BROWSER, driver_id)
 
         # 获取基本信息
         _, targets = self.cdp.target.get_targets()
-        self._context_id = targets['targetInfos'][0]['browserContextId']
+        self.context_id = targets['targetInfos'][0]['browserContextId']
         self._proxy = self._opts.proxy
-        self.__class__.CONTEXTS[self._context_id] = self
+        self.__class__.CONTEXTS[self.context_id] = self
         self.__create_page_driver(targets['targetInfos'])  # 启动时创建页面的 driver
-        self.__listener = Listener(context_id=self._context_id)
+        self.__listener = Listener(context_id=self.context_id)
 
         # 启用事件
         self.cdp.target.set_discover_targets()
 
         # 事件监听
         self.cdp.on(event="Target.targetCreated", callback=self.__on_target_target_created)
         self.cdp.on(event="Target.targetInfoChanged", callback=self.__on_target_target_info_changed)
@@ -57,15 +57,15 @@
 
             context_id = target_info["browserContextId"]
             proxy = self.__class__.CONTEXTS[context_id]._proxy if context_id in self.__class__.CONTEXTS else None
 
             # 创建 driver
             page_driver = PageDriver(
                 opts=self._opts,
-                driver_id=target_info["targetId"],  # 页面的 targetId
+                page_id=target_info["targetId"],  # 页面的 targetId
                 context_id=context_id,  # 页面的上下文 id
                 context_driver=self.__class__.CONTEXTS[context_id],
                 proxy=proxy,
             )
             self.__class__.PAGES[target_info["targetId"]] = page_driver
             self.__class__.PAGE_CONTENT_MAPS[target_info["targetId"]] = context_id
 
@@ -200,17 +200,17 @@
         """
 
         :param browser_driver:
         :param context_id:
         :param proxy: 代理
         """
         self._browser_driver = browser_driver
-        self._context_id = context_id
+        self.context_id = context_id
         self._proxy = proxy
-        self.__listener = Listener(context_id=self._context_id)
+        self.__listener = Listener(context_id=self.context_id)
 
     def new_page(
             self,
             new_window: bool = False,
             **kwargs
     ) -> "PageDriver":
         """
@@ -218,15 +218,15 @@
 
         :param new_window: 是否打开新窗口
         :param kwargs:
         :return:
         """
         return self._browser_driver.new_page(
             new_window=new_window,
-            context_id=self._context_id,
+            context_id=self.context_id,
             proxy=self._proxy,
             **kwargs
         )
 
     @property
     def listen(self) -> Listener:
         """
@@ -238,14 +238,14 @@
 
     def close(self):
         """
         关闭上下文
 
         :return:
         """
-        self._browser_driver.cdp.target.close_target(target_id=self._context_id)
+        self._browser_driver.cdp.target.close_target(target_id=self.context_id)
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         self.close()
```

### Comparing `EasyPage-0.0.5/easypage/driver/driver.py` & `EasyPage-0.0.6/easypage/driver/driver.py`

 * *Files identical despite different names*

### Comparing `EasyPage-0.0.5/easypage/driver/page.py` & `EasyPage-0.0.6/easypage/driver/page.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,30 +22,30 @@
 from easypage.utils import other_utils, browser_utils
 
 
 class PageDriver(Driver):
     def __init__(
             self,
             opts: BrowserOptions,
-            driver_id: str,
+            page_id: str,
             context_id: str,
             context_driver,
             proxy: definition.Proxy = None
     ):
         """
 
         :param opts: 配置
-        :param driver_id: driver_id
+        :param page_id: driver_id
         :param context_id: 所属上下文 id
         :param context_driver: 所属上下文 driver
         :param proxy: 代理
         """
-        super().__init__(opts, TYPE_PAGE, driver_id)
-        self._driver_id = driver_id
-        self._context_id = context_id
+        super().__init__(opts, TYPE_PAGE, page_id)
+        self.page_id = page_id
+        self.context_id = context_id
         self._proxy = proxy
         self._opts = opts
         self._context_driver = context_driver
 
         # TODO 查找一下是否有可能出现未捕获到请求，但是出现响应的情况
         # 预设参数
         self.__loading: bool = True
@@ -55,14 +55,15 @@
         # TODO 考虑根据不同的条件去设置是否启动监听避免额外的资源消耗，可以根据事件在 Listener 进行驱动
         # 启用事件
         self.cdp.dom.enable()
         self.cdp.page.enable()
         self.cdp.security.set_ignore_certificate_errors()
         self.cdp.fetch.enable(handle_auth_requests=True)
         self.cdp.network.enable()
+        self.cdp.css.enable()
 
         # 事件监听
         self.cdp.on(event='Page.lifecycleEvent', callback=self.__on_page_life_cycle_event)
         self.cdp.on(event='Page.loadEventFired', callback=self.__on_page_load_event_fired)
         self.cdp.on(event='Page.frameStartedLoading', callback=self.__on_page_frame_started_loading)
         self.cdp.on(event='Page.frameStoppedLoading', callback=self.__on_page_frame_stopped_loading)
         self.cdp.on(event='Fetch.requestPaused', callback=self.__on_fetch_request_paused)
@@ -81,15 +82,15 @@
         返回的第二个值是当请求失败的时候发送原因，比如设置的代理访问不通
 
         :param url:
         :param kwargs:
         :return:
         """
         if "frameId" not in kwargs:
-            kwargs["frameId"] = self._driver_id
+            kwargs["frameId"] = self.page_id
         status, result = self.cdp.page.navigate(url=url, **kwargs)
         if not status:
             return False, None
 
         elif "errorText" in result:
             logger.warning("url：{} errorText：{}", url, result["errorText"])
             return False, result["errorText"]
@@ -211,16 +212,16 @@
                     iframe_node_id=node_id,
                     iframe_owner_page=self
                 ))
             else:
                 try:
                     page_driver = PageDriver(
                         opts=self._opts,
-                        driver_id=frame_id,  # 页面的 targetId
-                        context_id=self._context_id,  # 页面的上下文 id
+                        page_id=frame_id,  # 页面的 targetId
+                        context_id=self.context_id,  # 页面的上下文 id
                         context_driver=self._context_driver,
                         proxy=self._proxy,
                     )
                     status, iframe_dom = page_driver.cdp.dom.get_document()
                     if not status:
                         continue
                     elements.append(Element(
@@ -262,15 +263,15 @@
         """
         获取 cookie
 
         :param only_key_val: 是否仅返回 {name:'',value:''} 形式
         :param domain: 指定域名
         :return: [{'name': '', 'value': '', 'domain': '', 'path': '', 'expires': -1, 'size': 161, 'httpOnly': True, 'secure': True, 'session': True, 'sameSite': 'Strict', 'priority': 'Medium', 'sameParty': False, 'sourceScheme': 'Secure', 'sourcePort': 443}]
         """
-        status, cookies = self.cdp.storage.get_cookies(context_id=self._context_id)
+        status, cookies = self.cdp.storage.get_cookies(context_id=self.context_id)
         if not status:
             return []
 
         cookies = cookies['cookies']
 
         if only_key_val:
             cookie_dict = {}
@@ -351,80 +352,90 @@
         """
         self.cdp.page.close()
 
     """
         等待
     """
 
-    def wait_loaded(self, timeout: int = None):
+    def wait_loaded(self, status: str = "complete", timeout: int = None):
         """
         等待页面加载完成
 
-        :param timeout:
+        :param status: 可选 interactive、complete
+        :param timeout: 没有提供会使用全局的
         :return:
         """
         timeout = timeout or self._opts.timeout
 
+        # 输入检查
+        dom_read_states = ["interactive", "complete"]
+        if status not in dom_read_states:
+            status = "complete"
+
+        # 加载等待
         start_time = time.time()
         while time.time() - start_time < timeout:
-            # if not self.__loading:
-            #     return
-            if self.eval_js(js="document.readyState")[-1] == "complete":
+            dom_status = self.eval_js(js="document.readyState")[-1]
+            if dom_status == status or dom_status == "complete":
                 self.__loading = False
                 return
             time.sleep(0.1)
 
     def wait_for_selector(
             self,
             selector: str,
+            node_id: int = None,
             timeout: int = None,
             raise_err: bool = False
     ) -> Union['Element', None, errors.ElementWaitTimeout]:
         """
         等待某个元素
 
         :param timeout:
+        :param node_id:
         :param selector:
         :param raise_err:
         :return:
         """
         timeout = timeout or self._opts.timeout
 
         start_time = time.time()
 
         while time.time() - start_time < timeout:
-            ele = self.query_selector(selector=selector)
+            ele = self.query_selector(selector=selector, node_id=node_id)
             if ele:
                 return ele
             time.sleep(0.1)
 
         if raise_err:
             raise errors.ElementWaitTimeout(selector)
 
     def wait_for_selectors(
             self,
             selectors: List[str],
+            node_id: int = None,
             timeout: int = None,
             raise_err: bool = False
     ) -> Union['Element', None, errors.ElementWaitTimeout]:
         """
         等待多个元素，谁先拿到就返回谁（所以要自己注意放入的顺序）
 
         :param timeout:
+        :param node_id:
         :param selectors: 元素列表
         :param raise_err:
         :return:
         """
         timeout = timeout or self._opts.timeout
 
         start_time = time.time()
 
         while time.time() - start_time < timeout:
             for s in selectors:
-                ele = self.query_selector(selector=s)
+                ele = self.query_selector(selector=s, node_id=node_id)
                 if ele:
                     return ele
 
                 if time.time() - start_time >= timeout:
                     break
 
             time.sleep(0.1)
@@ -773,17 +784,18 @@
     OpenBracket = 219
     BackSlash = 220
     CloseBracket = 221
     SingleQuote = 222
 
 
 class ActionChain:
-    def __init__(self, node_id: int, page: PageDriver):
+    def __init__(self, node_id: int, page: PageDriver, ele: "Element"):
         self.page = page
         self.node_id = node_id
+        self.ele = ele
 
     def focus(self):
         """
         聚焦
 
         :return:
         """
@@ -812,20 +824,21 @@
                 event_type="rawKeyDown",
                 windowsVirtualKeyCode=KeyCode.Backspace,
                 modifiers=Key.Backspace,
             )
 
         return self
 
-    def input_text(self, val: str, simulation: bool = True):
+    def input_text(self, val: str, delay: float = 0, simulation: bool = True):
         """
         输入文本（模拟输入）
 
         :param val:
         :param simulation: 模拟真实操作
+        :param delay: 延时输入（s）
         :return:
         """
         if not simulation:
             # 非模拟的话，实际的修改可能并不会生效（元素修改了，但是页面没更改）
             self.page.cdp.dom.set_attribute_value(
                 name="value",
                 value=val,
@@ -849,14 +862,16 @@
                     event_type="keyUp",
                     is_key_pad=True,
                     key=v,
                     text=v,
                     code="Key " + v.upper(),
                 )
 
+                time.sleep(delay)
+
         return self
 
     def ctrl(self, key: int):
         """
         ctrl 事件
 
         :param key: 如 ctrl+A 只要输入 a 或 A 就行了
@@ -870,23 +885,69 @@
             event_type="rawKeyDown",
             windowsVirtualKeyCode=key,
             modifiers=Key.Ctrl,
         )
 
         return self
 
-    def click(self, count: int = 1, button: str = "middle", simulation: bool = True):
+    # TODO 增加组合输入
+    # def combination_input(self, modifiers: int, value: Union[str, int] = None):
+    #     """
+    #     组合输入
+    #
+    #     :param modifiers: 比如 ctrl+shift 就是 Key.Ctrl|Key.Shift
+    #     :param value: 输入的值 比如 abc
+    #     :return:
+    #     """
+
+    def click(self, count: int = 1, button: str = "left", simulation: bool = True):
         """
         执行点击
 
         :param count: 点击次数
-        :param button: 点击位置，如：none, left, middle, right, back, forward
+        :param button: 代表鼠标的按键，如：none（不触发按键，代表光标）, left（左击）, middle（滚轮）, right（右击）, back（后退）, forward（前进）
         :param simulation: 模拟真实操作
         :return:
         """
+        if not simulation:
+            self.ele.eval_js_on_selector(js="this.click();", returnByValue=True)
+        else:
+            # 聚焦
+            self.focus()
+
+            # 获取元素坐标
+            x, y = self.ele.coordinate_center
+
+            # 移动
+            self.page.cdp.input.dispatch_mouse_event(
+                event_type="mouseMoved",
+                x=x,
+                y=y,
+                button="none"
+            )
+
+            # 点击
+            self.page.cdp.input.dispatch_mouse_event(
+                event_type="mousePressed",
+                x=x,
+                y=y,
+                button=button,
+                clickCount=count
+            )
+
+            # 释放
+            self.page.cdp.input.dispatch_mouse_event(
+                event_type="mouseReleased",
+                x=x,
+                y=y,
+                button=button,
+                clickCount=count
+            )
+
+        return self
 
 
 """
     元素
 """
 
 
@@ -907,17 +968,17 @@
         :param page PageDriver 对象（iframe 的话就是 iframe 自身的 driver）
         :param is_iframe 是不是 iframe
         :param iframe_node_id iframe 自身的 node_id
         :param iframe_owner_page iframe 所在页面
         :return:
         """
         if is_iframe:
-            super().__init__(iframe_node_id, iframe_owner_page)
+            super().__init__(iframe_node_id, iframe_owner_page, self)
         else:
-            super().__init__(node_id, page)
+            super().__init__(node_id, page, self)
 
         self._back_end_node_id = None
         self._obj_id = None
         self._is_iframe = is_iframe
         self._iframe_node_id = iframe_node_id
         self._iframe_owner_page = iframe_owner_page
         self._iframe_page = page
@@ -971,75 +1032,219 @@
             )
         return self.page.query_selector_all(
             selector=selector,
             node_id=self.node_id,
             raise_err=raise_err,
         )
 
-    def eval_js_on_selector(self, js: str, **kwargs):
+    def wait_for_selector(
+            self,
+            selector: str,
+            timeout: int = None,
+            raise_err: bool = False
+    ) -> Union['Element', None, errors.ElementWaitTimeout]:
+        """
+        等待某个元素
+
+        :param timeout:
+        :param selector:
+        :param raise_err:
+        :return:
+        """
+        if self._is_iframe:
+            return self._iframe_page.wait_for_selector(
+                selector=selector,
+                timeout=timeout,
+                node_id=self._iframe_document_node_id,
+                raise_err=raise_err
+            )
+        return self.page.wait_for_selector(
+            selector=selector,
+            timeout=timeout,
+            node_id=self.node_id,
+            raise_err=raise_err
+        )
+
+    def wait_for_selectors(
+            self,
+            selectors: List[str],
+            timeout: int = None,
+            raise_err: bool = False
+    ) -> Union['Element', None, errors.ElementWaitTimeout]:
+        """
+        等待多个元素，谁先拿到就返回谁（所以要自己注意放入的顺序）
+
+        :param timeout:
+        :param selectors: 元素列表
+        :param raise_err:
+        :return:
+        """
+        if self._is_iframe:
+            return self._iframe_page.wait_for_selectors(
+                selectors=selectors,
+                timeout=timeout,
+                node_id=self._iframe_document_node_id,
+                raise_err=raise_err
+            )
+        return self.page.wait_for_selectors(
+            selectors=selectors,
+            timeout=timeout,
+            node_id=self.node_id,
+            raise_err=raise_err
+        )
+
+    def eval_js_on_selector(self, js: str, **kwargs) -> Tuple[bool, dict]:
         """
         执行 js 脚本（会自动使用 function 包裹，不然无法执行）
 
         学习链接：https://chromedevtools.github.io/devtools-protocol/tot/Runtime/#method-evaluate
 
         :param js: 路径或者 js 字符串
         :return:
         """
         js = "function (){ %s }" % js
         return self.page.cdp.runtime.call_function_on(js=js, object_id=self.object_id, **kwargs)
 
-    def click(self, count: int = 1, button: str = "left", raise_err: bool = True, simulation: bool = True):
+    @property
+    def style(self) -> dict:
         """
-        执行点击
+        获取 style
 
-        :param count: 点击次数
-        :param button: 代表鼠标的按键，如：none（不触发按键，代表光标）, left（左击）, middle（滚轮）, right（右击）, back（后退）, forward（前进）
-        :param raise_err: 是否抛出错误
-        :param simulation: 模拟真实操作
         :return:
         """
-        if not simulation:
-            self.eval_js_on_selector(js="this.click();", returnByValue=True)
-            return
-        else:
-            # 聚焦
-            self.focus()
+        status, content = self.page.cdp.css.get_computed_style_for_node(node_id=self.node_id)
+        if not status:
+            return {}
 
-            # 获取元素坐标
-            status, content = self.page.cdp.dom.get_box_model(nodeId=self.node_id, raise_err=raise_err)
-            content = content['model']['content']
-            x, y = browser_utils.parse_box_center_coordinate(data=content)
+        return dict([[i["name"], i["value"]] for i in content["computedStyle"]])
 
-            # 移动
-            self.page.cdp.input.dispatch_mouse_event(
-                event_type="mouseMoved",
-                x=x,
-                y=y,
-                button="none"
-            )
+    @property
+    def is_visible(self) -> bool:
+        """
+        元素是否可见（全部可见）
 
-            # 点击
-            self.page.cdp.input.dispatch_mouse_event(
-                event_type="mousePressed",
-                x=x,
-                y=y,
-                button=button,
-                clickCount=count
-            )
+        :return:
+        """
+        js = """
+            return function (el) {
+                var rect = el.getBoundingClientRect();
+                var isVisible = (
+                    rect.top >= 0 &&
+                    rect.left >= 0 &&
+                    rect.bottom <= (window.innerHeight || document.documentElement.clientHeight) &&
+                    rect.right <= (window.innerWidth || document.documentElement.clientWidth)
+                );
+            
+                if (!isVisible) return false;
+            
+                var style = window.getComputedStyle(el);
+                if (style.visibility === 'hidden' || style.display === 'none') return false;
+            
+                if (rect.width === 0 || rect.height === 0) return false;
+            
+                var elementBelow = document.elementFromPoint(rect.left + rect.width / 2, rect.top + rect.height / 2);
+                if (elementBelow && elementBelow !== el && !el.contains(elementBelow)) return false;
+            
+                return true;
+            }(this)
+        """
+        status, val = self.eval_js_on_selector(js=js)
+        if not status:
+            return False
 
-            # 释放
-            self.page.cdp.input.dispatch_mouse_event(
-                event_type="mouseReleased",
-                x=x,
-                y=y,
-                button=button,
-                clickCount=count
-            )
+        return val["result"]["value"]
 
-        return self
+    @property
+    def is_displayed(self) -> bool:
+        """
+        元素是否显示
+
+        :return:
+        """
+        style = self.style
+
+        if style.get("visibility") == 'hidden':
+            return True
+
+        if style.get("display") == 'none':
+            return True
+
+        if self.attrs.get("hidden"):
+            return True
+
+        status, val = self.eval_js_on_selector(js="return this.offsetParent === null;")
+        if status and val["result"]["value"]:
+            return True
+
+        return False
+
+    @property
+    def is_enable(self) -> bool:
+        """
+        元素是否可用
+
+        :return:
+        """
+        status, val = self.eval_js_on_selector(js="return this.disabled;")
+        if not status:
+            return False
+        return val["result"]["value"]
+
+    @property
+    def is_checked(self) -> bool:
+        """
+        元素是否被选择
+
+        :return:
+        """
+        status, val = self.eval_js_on_selector(js="return this.checked;")
+        if not status:
+            return False
+        return val["result"]["value"]
+
+    @property
+    def is_selected(self) -> bool:
+        """
+        元素是否被选择
+
+        :return:
+        """
+        status, val = self.eval_js_on_selector(js="return this.selected;")
+        if not status:
+            return False
+        return val["result"]["value"]
+
+    @property
+    def coordinates(self) -> dict:
+        """
+        获取元素的坐标信息
+        返回的比如 content 有 4 个坐标，分别是
+        - 左上顶点
+        - 右上顶点
+        - 右下顶点
+        - 左下顶点
+
+        :return:
+        """
+        # 获取元素坐标
+        status, content = self.page.cdp.dom.get_box_model(nodeId=self.node_id)
+        if not status:
+            return {}
+
+        return content['model']
+
+    @property
+    def coordinate_center(self) -> tuple:
+        """
+        元素中心点坐标
+
+        :return:
+        """
+        content = self.coordinates["content"]
+        return browser_utils.parse_box_center_coordinate(data=content)
 
     @property
     def attrs(self) -> dict:
         """
         属性
 
         :return:
@@ -1143,12 +1348,7 @@
 
         return self._obj_id
 
     def __repr__(self):
         attrs = self.attrs
         attrs_text = ' '.join([f'{i}="{attrs[i]}"' for i in attrs.keys()])
         return f"<{self.__class__.__name__} {self.tag_name} {attrs_text}>"
-
-
-class IframeElement(PageDriver):
-    def __init__(self, opts: BrowserOptions, driver_id: str, context_id: str = None, proxy: definition.Proxy = None):
-        super().__init__(opts, driver_id, context_id, proxy)
```

### Comparing `EasyPage-0.0.5/easypage/errors.py` & `EasyPage-0.0.6/easypage/errors.py`

 * *Files identical despite different names*

### Comparing `EasyPage-0.0.5/easypage/listener.py` & `EasyPage-0.0.6/easypage/listener.py`

 * *Files identical despite different names*

### Comparing `EasyPage-0.0.5/easypage/logger.py` & `EasyPage-0.0.6/easypage/logger.py`

 * *Files identical despite different names*

### Comparing `EasyPage-0.0.5/easypage/main.py` & `EasyPage-0.0.6/easypage/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,15 +48,15 @@
     @property
     def page(self) -> "PageDriver":
         """
         默认页面
 
         :return:
         """
-        default_page_id = BrowserDriver.CONTENT_PAGE_MAPS[self.browser._context_id][0]
+        default_page_id = BrowserDriver.CONTENT_PAGE_MAPS[self.browser.context_id][0]
         return BrowserDriver.PAGES[default_page_id]
 
     @property
     def pages(self) -> List["PageDriver"]:
         """
         获取所有的当前页面
```

### Comparing `EasyPage-0.0.5/easypage/operate.py` & `EasyPage-0.0.6/easypage/operate.py`

 * *Files identical despite different names*

### Comparing `EasyPage-0.0.5/easypage/options.py` & `EasyPage-0.0.6/easypage/options.py`

 * *Files identical despite different names*

### Comparing `EasyPage-0.0.5/easypage/request.py` & `EasyPage-0.0.6/easypage/request.py`

 * *Files identical despite different names*

### Comparing `EasyPage-0.0.5/easypage/response.py` & `EasyPage-0.0.6/easypage/response.py`

 * *Files identical despite different names*

### Comparing `EasyPage-0.0.5/easypage/settings.py` & `EasyPage-0.0.6/easypage/settings.py`

 * *Files identical despite different names*

### Comparing `EasyPage-0.0.5/easypage/utils/browser_utils.py` & `EasyPage-0.0.6/easypage/utils/browser_utils.py`

 * *Files identical despite different names*

### Comparing `EasyPage-0.0.5/easypage/utils/other_utils.py` & `EasyPage-0.0.6/easypage/utils/other_utils.py`

 * *Files identical despite different names*

### Comparing `EasyPage-0.0.5/setup.py` & `EasyPage-0.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='EasyPage',
-    version='0.0.5',
+    version='0.0.6',
     author='leviathangk',
     author_email='1015295213@qq.com',
     description='基于 CDP 协议，简洁快速的浏览器控制 API',
     keywords=['EasyPage', 'page', 'browser'],
     packages=find_packages(),
     install_requires=[
         "lxml",
```

