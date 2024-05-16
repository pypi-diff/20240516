# Comparing `tmp/EasyPage-0.0.8.tar.gz` & `tmp/EasyPage-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "EasyPage-0.0.8.tar", last modified: Thu May 16 07:10:29 2024, max compression
+gzip compressed data, was "EasyPage-0.0.9.tar", last modified: Thu May 16 07:14:13 2024, max compression
```

## Comparing `EasyPage-0.0.8.tar` & `EasyPage-0.0.9.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxrwxrwx   0        0        0        0 2024-05-16 07:10:29.497529 EasyPage-0.0.8/
-drwxrwxrwx   0        0        0        0 2024-05-16 07:10:29.245953 EasyPage-0.0.8/EasyPage.egg-info/
--rw-rw-rw-   0        0        0      286 2024-05-16 07:10:29.000000 EasyPage-0.0.8/EasyPage.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1060 2024-05-16 07:10:29.000000 EasyPage-0.0.8/EasyPage.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-16 07:10:29.000000 EasyPage-0.0.8/EasyPage.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       76 2024-05-16 07:10:29.000000 EasyPage-0.0.8/EasyPage.egg-info/requires.txt
--rw-rw-rw-   0        0        0       24 2024-05-16 07:10:29.000000 EasyPage-0.0.8/EasyPage.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      286 2024-05-16 07:10:29.497529 EasyPage-0.0.8/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-16 07:10:29.317952 EasyPage-0.0.8/easypage/
--rw-rw-rw-   0        0        0      192 2024-05-16 02:17:32.000000 EasyPage-0.0.8/easypage/__init__.py
--rw-rw-rw-   0        0        0     3499 2024-05-16 07:05:55.000000 EasyPage-0.0.8/easypage/cdp.py
-drwxrwxrwx   0        0        0        0 2024-05-16 07:10:29.460525 EasyPage-0.0.8/easypage/cdp_method/
--rw-rw-rw-   0        0        0        0 2024-04-17 12:56:48.000000 EasyPage-0.0.8/easypage/cdp_method/__init__.py
--rw-rw-rw-   0        0        0     1536 2024-04-24 09:10:40.000000 EasyPage-0.0.8/easypage/cdp_method/browser.py
--rw-rw-rw-   0        0        0     1962 2024-05-13 03:08:12.000000 EasyPage-0.0.8/easypage/cdp_method/css.py
--rw-rw-rw-   0        0        0    12414 2024-05-13 03:01:05.000000 EasyPage-0.0.8/easypage/cdp_method/dom.py
--rw-rw-rw-   0        0        0     1049 2024-04-24 08:57:22.000000 EasyPage-0.0.8/easypage/cdp_method/emulation.py
--rw-rw-rw-   0        0        0     9545 2024-04-24 14:05:55.000000 EasyPage-0.0.8/easypage/cdp_method/fetch.py
--rw-rw-rw-   0        0        0     2654 2024-04-24 09:06:00.000000 EasyPage-0.0.8/easypage/cdp_method/input.py
--rw-rw-rw-   0        0        0     4467 2024-05-07 11:18:55.000000 EasyPage-0.0.8/easypage/cdp_method/network.py
--rw-rw-rw-   0        0        0     8620 2024-05-16 02:51:16.000000 EasyPage-0.0.8/easypage/cdp_method/page.py
--rw-rw-rw-   0        0        0     3667 2024-04-24 09:16:01.000000 EasyPage-0.0.8/easypage/cdp_method/runtime.py
--rw-rw-rw-   0        0        0     2354 2024-04-24 09:16:01.000000 EasyPage-0.0.8/easypage/cdp_method/security.py
--rw-rw-rw-   0        0        0     1322 2024-04-24 09:16:01.000000 EasyPage-0.0.8/easypage/cdp_method/storage.py
--rw-rw-rw-   0        0        0     5884 2024-04-24 13:35:04.000000 EasyPage-0.0.8/easypage/cdp_method/target.py
--rw-rw-rw-   0        0        0    18116 2024-05-16 07:10:10.000000 EasyPage-0.0.8/easypage/conn.py
--rw-rw-rw-   0        0        0      391 2024-04-25 02:28:17.000000 EasyPage-0.0.8/easypage/definition.py
-drwxrwxrwx   0        0        0        0 2024-05-16 07:10:29.484527 EasyPage-0.0.8/easypage/driver/
--rw-rw-rw-   0        0        0        0 2024-04-09 06:15:36.000000 EasyPage-0.0.8/easypage/driver/__init__.py
--rw-rw-rw-   0        0        0     7785 2024-05-14 01:38:27.000000 EasyPage-0.0.8/easypage/driver/browser.py
--rw-rw-rw-   0        0        0      928 2024-05-09 09:58:08.000000 EasyPage-0.0.8/easypage/driver/driver.py
--rw-rw-rw-   0        0        0    44997 2024-05-16 07:09:02.000000 EasyPage-0.0.8/easypage/driver/page.py
--rw-rw-rw-   0        0        0     1598 2024-05-16 06:11:45.000000 EasyPage-0.0.8/easypage/errors.py
--rw-rw-rw-   0        0        0     2137 2024-05-16 06:41:09.000000 EasyPage-0.0.8/easypage/event_manager.py
--rw-rw-rw-   0        0        0     5897 2024-05-16 06:06:04.000000 EasyPage-0.0.8/easypage/listener.py
--rw-rw-rw-   0        0        0     2093 2024-05-09 07:29:23.000000 EasyPage-0.0.8/easypage/logger.py
--rw-rw-rw-   0        0        0     4580 2024-05-14 01:35:01.000000 EasyPage-0.0.8/easypage/main.py
--rw-rw-rw-   0        0        0     4106 2024-04-25 08:20:54.000000 EasyPage-0.0.8/easypage/operate.py
--rw-rw-rw-   0        0        0    10944 2024-04-24 08:39:28.000000 EasyPage-0.0.8/easypage/options.py
--rw-rw-rw-   0        0        0     1813 2024-05-16 06:38:58.000000 EasyPage-0.0.8/easypage/request.py
--rw-rw-rw-   0        0        0     4390 2024-05-10 01:15:20.000000 EasyPage-0.0.8/easypage/response.py
--rw-rw-rw-   0        0        0     2787 2024-05-15 02:22:54.000000 EasyPage-0.0.8/easypage/settings.py
-drwxrwxrwx   0        0        0        0 2024-05-16 07:10:29.493525 EasyPage-0.0.8/easypage/utils/
--rw-rw-rw-   0        0        0        0 2024-04-09 06:15:42.000000 EasyPage-0.0.8/easypage/utils/__init__.py
--rw-rw-rw-   0        0        0     3708 2024-04-10 01:27:44.000000 EasyPage-0.0.8/easypage/utils/browser_utils.py
--rw-rw-rw-   0        0        0     2182 2024-05-09 08:03:26.000000 EasyPage-0.0.8/easypage/utils/other_utils.py
-drwxrwxrwx   0        0        0        0 2024-05-16 07:10:29.495525 EasyPage-0.0.8/easypage_async/
--rw-rw-rw-   0        0        0       40 2024-05-14 06:22:35.000000 EasyPage-0.0.8/easypage_async/__init__.py
--rw-rw-rw-   0        0        0       42 2024-05-16 07:10:29.498529 EasyPage-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0      599 2024-05-16 07:10:25.000000 EasyPage-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-16 07:14:13.195865 EasyPage-0.0.9/
+drwxrwxrwx   0        0        0        0 2024-05-16 07:14:04.567462 EasyPage-0.0.9/EasyPage.egg-info/
+-rw-rw-rw-   0        0        0      286 2024-05-16 07:14:04.000000 EasyPage-0.0.9/EasyPage.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1060 2024-05-16 07:14:04.000000 EasyPage-0.0.9/EasyPage.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-16 07:14:04.000000 EasyPage-0.0.9/EasyPage.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       76 2024-05-16 07:14:04.000000 EasyPage-0.0.9/EasyPage.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       24 2024-05-16 07:14:04.000000 EasyPage-0.0.9/EasyPage.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      286 2024-05-16 07:14:13.194866 EasyPage-0.0.9/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-16 07:14:08.427179 EasyPage-0.0.9/easypage/
+-rw-rw-rw-   0        0        0      192 2024-05-16 02:17:32.000000 EasyPage-0.0.9/easypage/__init__.py
+-rw-rw-rw-   0        0        0     3499 2024-05-16 07:05:55.000000 EasyPage-0.0.9/easypage/cdp.py
+drwxrwxrwx   0        0        0        0 2024-05-16 07:14:11.644024 EasyPage-0.0.9/easypage/cdp_method/
+-rw-rw-rw-   0        0        0        0 2024-04-17 12:56:48.000000 EasyPage-0.0.9/easypage/cdp_method/__init__.py
+-rw-rw-rw-   0        0        0     1536 2024-04-24 09:10:40.000000 EasyPage-0.0.9/easypage/cdp_method/browser.py
+-rw-rw-rw-   0        0        0     1962 2024-05-13 03:08:12.000000 EasyPage-0.0.9/easypage/cdp_method/css.py
+-rw-rw-rw-   0        0        0    12414 2024-05-13 03:01:05.000000 EasyPage-0.0.9/easypage/cdp_method/dom.py
+-rw-rw-rw-   0        0        0     1049 2024-04-24 08:57:22.000000 EasyPage-0.0.9/easypage/cdp_method/emulation.py
+-rw-rw-rw-   0        0        0     9545 2024-04-24 14:05:55.000000 EasyPage-0.0.9/easypage/cdp_method/fetch.py
+-rw-rw-rw-   0        0        0     2654 2024-04-24 09:06:00.000000 EasyPage-0.0.9/easypage/cdp_method/input.py
+-rw-rw-rw-   0        0        0     4467 2024-05-07 11:18:55.000000 EasyPage-0.0.9/easypage/cdp_method/network.py
+-rw-rw-rw-   0        0        0     8620 2024-05-16 02:51:16.000000 EasyPage-0.0.9/easypage/cdp_method/page.py
+-rw-rw-rw-   0        0        0     3667 2024-04-24 09:16:01.000000 EasyPage-0.0.9/easypage/cdp_method/runtime.py
+-rw-rw-rw-   0        0        0     2354 2024-04-24 09:16:01.000000 EasyPage-0.0.9/easypage/cdp_method/security.py
+-rw-rw-rw-   0        0        0     1322 2024-04-24 09:16:01.000000 EasyPage-0.0.9/easypage/cdp_method/storage.py
+-rw-rw-rw-   0        0        0     5884 2024-04-24 13:35:04.000000 EasyPage-0.0.9/easypage/cdp_method/target.py
+-rw-rw-rw-   0        0        0    18116 2024-05-16 07:10:10.000000 EasyPage-0.0.9/easypage/conn.py
+-rw-rw-rw-   0        0        0      391 2024-04-25 02:28:17.000000 EasyPage-0.0.9/easypage/definition.py
+drwxrwxrwx   0        0        0        0 2024-05-16 07:14:12.556410 EasyPage-0.0.9/easypage/driver/
+-rw-rw-rw-   0        0        0        0 2024-04-09 06:15:36.000000 EasyPage-0.0.9/easypage/driver/__init__.py
+-rw-rw-rw-   0        0        0     7785 2024-05-14 01:38:27.000000 EasyPage-0.0.9/easypage/driver/browser.py
+-rw-rw-rw-   0        0        0      928 2024-05-09 09:58:08.000000 EasyPage-0.0.9/easypage/driver/driver.py
+-rw-rw-rw-   0        0        0    44934 2024-05-16 07:13:51.000000 EasyPage-0.0.9/easypage/driver/page.py
+-rw-rw-rw-   0        0        0     1598 2024-05-16 06:11:45.000000 EasyPage-0.0.9/easypage/errors.py
+-rw-rw-rw-   0        0        0     2137 2024-05-16 06:41:09.000000 EasyPage-0.0.9/easypage/event_manager.py
+-rw-rw-rw-   0        0        0     5897 2024-05-16 06:06:04.000000 EasyPage-0.0.9/easypage/listener.py
+-rw-rw-rw-   0        0        0     2093 2024-05-09 07:29:23.000000 EasyPage-0.0.9/easypage/logger.py
+-rw-rw-rw-   0        0        0     4580 2024-05-14 01:35:01.000000 EasyPage-0.0.9/easypage/main.py
+-rw-rw-rw-   0        0        0     4106 2024-04-25 08:20:54.000000 EasyPage-0.0.9/easypage/operate.py
+-rw-rw-rw-   0        0        0    10944 2024-04-24 08:39:28.000000 EasyPage-0.0.9/easypage/options.py
+-rw-rw-rw-   0        0        0     1813 2024-05-16 06:38:58.000000 EasyPage-0.0.9/easypage/request.py
+-rw-rw-rw-   0        0        0     4390 2024-05-10 01:15:20.000000 EasyPage-0.0.9/easypage/response.py
+-rw-rw-rw-   0        0        0     2787 2024-05-15 02:22:54.000000 EasyPage-0.0.9/easypage/settings.py
+drwxrwxrwx   0        0        0        0 2024-05-16 07:14:13.101865 EasyPage-0.0.9/easypage/utils/
+-rw-rw-rw-   0        0        0        0 2024-04-09 06:15:42.000000 EasyPage-0.0.9/easypage/utils/__init__.py
+-rw-rw-rw-   0        0        0     3708 2024-04-10 01:27:44.000000 EasyPage-0.0.9/easypage/utils/browser_utils.py
+-rw-rw-rw-   0        0        0     2182 2024-05-09 08:03:26.000000 EasyPage-0.0.9/easypage/utils/other_utils.py
+drwxrwxrwx   0        0        0        0 2024-05-16 07:14:13.193864 EasyPage-0.0.9/easypage_async/
+-rw-rw-rw-   0        0        0       40 2024-05-14 06:22:35.000000 EasyPage-0.0.9/easypage_async/__init__.py
+-rw-rw-rw-   0        0        0       42 2024-05-16 07:14:13.195865 EasyPage-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      599 2024-05-16 07:13:51.000000 EasyPage-0.0.9/setup.py
```

### Comparing `EasyPage-0.0.8/EasyPage.egg-info/SOURCES.txt` & `EasyPage-0.0.9/EasyPage.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `EasyPage-0.0.8/easypage/cdp.py` & `EasyPage-0.0.9/easypage/cdp.py`

 * *Files identical despite different names*

### Comparing `EasyPage-0.0.8/easypage/cdp_method/browser.py` & `EasyPage-0.0.9/easypage/cdp_method/browser.py`

 * *Files identical despite different names*

### Comparing `EasyPage-0.0.8/easypage/cdp_method/css.py` & `EasyPage-0.0.9/easypage/cdp_method/css.py`

 * *Files identical despite different names*

### Comparing `EasyPage-0.0.8/easypage/cdp_method/dom.py` & `EasyPage-0.0.9/easypage/cdp_method/dom.py`

 * *Files identical despite different names*

### Comparing `EasyPage-0.0.8/easypage/cdp_method/emulation.py` & `EasyPage-0.0.9/easypage/cdp_method/emulation.py`

 * *Files identical despite different names*

### Comparing `EasyPage-0.0.8/easypage/cdp_method/fetch.py` & `EasyPage-0.0.9/easypage/cdp_method/fetch.py`

 * *Files identical despite different names*

### Comparing `EasyPage-0.0.8/easypage/cdp_method/input.py` & `EasyPage-0.0.9/easypage/cdp_method/input.py`

 * *Files identical despite different names*

### Comparing `EasyPage-0.0.8/easypage/cdp_method/network.py` & `EasyPage-0.0.9/easypage/cdp_method/network.py`

 * *Files identical despite different names*

### Comparing `EasyPage-0.0.8/easypage/cdp_method/page.py` & `EasyPage-0.0.9/easypage/cdp_method/page.py`

 * *Files identical despite different names*

### Comparing `EasyPage-0.0.8/easypage/cdp_method/runtime.py` & `EasyPage-0.0.9/easypage/cdp_method/runtime.py`

 * *Files identical despite different names*

### Comparing `EasyPage-0.0.8/easypage/cdp_method/security.py` & `EasyPage-0.0.9/easypage/cdp_method/security.py`

 * *Files identical despite different names*

### Comparing `EasyPage-0.0.8/easypage/cdp_method/storage.py` & `EasyPage-0.0.9/easypage/cdp_method/storage.py`

 * *Files identical despite different names*

### Comparing `EasyPage-0.0.8/easypage/cdp_method/target.py` & `EasyPage-0.0.9/easypage/cdp_method/target.py`

 * *Files identical despite different names*

### Comparing `EasyPage-0.0.8/easypage/conn.py` & `EasyPage-0.0.9/easypage/conn.py`

 * *Files identical despite different names*

### Comparing `EasyPage-0.0.8/easypage/driver/browser.py` & `EasyPage-0.0.9/easypage/driver/browser.py`

 * *Files identical despite different names*

### Comparing `EasyPage-0.0.8/easypage/driver/driver.py` & `EasyPage-0.0.9/easypage/driver/driver.py`

 * *Files identical despite different names*

### Comparing `EasyPage-0.0.8/easypage/driver/page.py` & `EasyPage-0.0.9/easypage/driver/page.py`

 * *Files 0% similar despite different names*

```diff
@@ -417,15 +417,15 @@
             status = "complete"
 
         # 加载等待
         start_time = time.time()
         while time.time() - start_time < timeout:
             try:
                 dom_status = self.eval_js(js="document.readyState", raise_err=True)[-1]
-            except errors.CDPConnClosed:
+            except:
                 return
 
             if dom_status == status or dom_status == "complete":
                 self.__loading = False
                 return
 
             if self.cdp.closed():
@@ -451,15 +451,15 @@
         """
         timeout = timeout or self._opts.timeout
 
         start_time = time.time()
         while time.time() - start_time < timeout:
             try:
                 ele = self.query_selector(selector=selector, node_id=node_id, raise_err=True)
-            except errors.CDPConnClosed:
+            except:
                 return
 
             if ele:
                 return ele
 
             if self.cdp.closed():
                 break
@@ -489,15 +489,15 @@
 
         start_time = time.time()
 
         while time.time() - start_time < timeout:
             for s in selectors:
                 try:
                     ele = self.query_selector(selector=s, node_id=node_id, raise_err=True)
-                except errors.CDPConnClosed:
+                except:
                     return
 
                 if ele:
                     return ele
 
                 if self.cdp.closed():
                     break
```

### Comparing `EasyPage-0.0.8/easypage/errors.py` & `EasyPage-0.0.9/easypage/errors.py`

 * *Files identical despite different names*

### Comparing `EasyPage-0.0.8/easypage/event_manager.py` & `EasyPage-0.0.9/easypage/event_manager.py`

 * *Files identical despite different names*

### Comparing `EasyPage-0.0.8/easypage/listener.py` & `EasyPage-0.0.9/easypage/listener.py`

 * *Files identical despite different names*

### Comparing `EasyPage-0.0.8/easypage/logger.py` & `EasyPage-0.0.9/easypage/logger.py`

 * *Files identical despite different names*

### Comparing `EasyPage-0.0.8/easypage/main.py` & `EasyPage-0.0.9/easypage/main.py`

 * *Files identical despite different names*

### Comparing `EasyPage-0.0.8/easypage/operate.py` & `EasyPage-0.0.9/easypage/operate.py`

 * *Files identical despite different names*

### Comparing `EasyPage-0.0.8/easypage/options.py` & `EasyPage-0.0.9/easypage/options.py`

 * *Files identical despite different names*

### Comparing `EasyPage-0.0.8/easypage/request.py` & `EasyPage-0.0.9/easypage/request.py`

 * *Files identical despite different names*

### Comparing `EasyPage-0.0.8/easypage/response.py` & `EasyPage-0.0.9/easypage/response.py`

 * *Files identical despite different names*

### Comparing `EasyPage-0.0.8/easypage/settings.py` & `EasyPage-0.0.9/easypage/settings.py`

 * *Files identical despite different names*

### Comparing `EasyPage-0.0.8/easypage/utils/browser_utils.py` & `EasyPage-0.0.9/easypage/utils/browser_utils.py`

 * *Files identical despite different names*

### Comparing `EasyPage-0.0.8/easypage/utils/other_utils.py` & `EasyPage-0.0.9/easypage/utils/other_utils.py`

 * *Files identical despite different names*

### Comparing `EasyPage-0.0.8/setup.py` & `EasyPage-0.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='EasyPage',
-    version='0.0.8',
+    version='0.0.9',
     author='leviathangk',
     author_email='1015295213@qq.com',
     description='基于 CDP 协议，简洁快速的浏览器控制 API',
     keywords=['EasyPage', 'page', 'browser'],
     packages=find_packages(),
     install_requires=[
         "lxml",
```

