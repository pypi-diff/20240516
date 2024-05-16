# Comparing `tmp/pyrisco-0.6.1.tar.gz` & `tmp/pyrisco-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrisco-0.6.1.tar", last modified: Thu Apr 25 15:59:24 2024, max compression
+gzip compressed data, was "pyrisco-0.6.2.tar", last modified: Thu May 16 05:05:53 2024, max compression
```

## Comparing `pyrisco-0.6.1.tar` & `pyrisco-0.6.2.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 onfreund   (501) staff       (20)        0 2024-04-25 15:59:24.626548 pyrisco-0.6.1/
--rw-r--r--   0 onfreund   (501) staff       (20)     1065 2021-08-21 12:09:24.000000 pyrisco-0.6.1/LICENSE
--rw-r--r--   0 onfreund   (501) staff       (20)       25 2021-08-21 12:09:24.000000 pyrisco-0.6.1/MANIFEST.in
--rw-r--r--   0 onfreund   (501) staff       (20)     3030 2024-04-25 15:59:24.625155 pyrisco-0.6.1/PKG-INFO
--rw-r--r--   0 onfreund   (501) staff       (20)     2363 2022-07-23 14:50:37.000000 pyrisco-0.6.1/README.md
-drwxr-xr-x   0 onfreund   (501) staff       (20)        0 2024-04-25 15:59:24.599570 pyrisco-0.6.1/pyrisco/
--rw-r--r--   0 onfreund   (501) staff       (20)      148 2022-07-23 14:51:59.000000 pyrisco-0.6.1/pyrisco/__init__.py
-drwxr-xr-x   0 onfreund   (501) staff       (20)        0 2024-04-25 15:59:24.610879 pyrisco-0.6.1/pyrisco/cloud/
--rw-r--r--   0 onfreund   (501) staff       (20)       36 2022-07-23 14:51:32.000000 pyrisco-0.6.1/pyrisco/cloud/__init__.py
--rw-r--r--   0 onfreund   (501) staff       (20)      687 2022-07-23 08:48:17.000000 pyrisco-0.6.1/pyrisco/cloud/alarm.py
--rw-r--r--   0 onfreund   (501) staff       (20)     1860 2022-07-23 08:48:17.000000 pyrisco-0.6.1/pyrisco/cloud/event.py
--rw-r--r--   0 onfreund   (501) staff       (20)     1532 2022-07-23 08:48:17.000000 pyrisco-0.6.1/pyrisco/cloud/partition.py
--rw-r--r--   0 onfreund   (501) staff       (20)     6109 2022-08-03 19:38:59.000000 pyrisco-0.6.1/pyrisco/cloud/risco_cloud.py
--rw-r--r--   0 onfreund   (501) staff       (20)      790 2022-07-23 08:48:17.000000 pyrisco-0.6.1/pyrisco/cloud/zone.py
--rw-r--r--   0 onfreund   (501) staff       (20)     2891 2024-03-23 09:28:16.000000 pyrisco-0.6.1/pyrisco/common.py
-drwxr-xr-x   0 onfreund   (501) staff       (20)        0 2024-04-25 15:59:24.623398 pyrisco-0.6.1/pyrisco/local/
--rw-r--r--   0 onfreund   (501) staff       (20)       36 2022-07-23 14:52:55.000000 pyrisco-0.6.1/pyrisco/local/__init__.py
--rw-r--r--   0 onfreund   (501) staff       (20)      161 2022-07-23 08:48:17.000000 pyrisco-0.6.1/pyrisco/local/const.py
--rw-r--r--   0 onfreund   (501) staff       (20)     1969 2024-02-14 09:05:38.000000 pyrisco-0.6.1/pyrisco/local/panels.py
--rw-r--r--   0 onfreund   (501) staff       (20)     1849 2022-07-27 14:11:25.000000 pyrisco-0.6.1/pyrisco/local/partition.py
--rw-r--r--   0 onfreund   (501) staff       (20)     5365 2022-09-15 12:11:59.000000 pyrisco-0.6.1/pyrisco/local/risco_crypt.py
--rw-r--r--   0 onfreund   (501) staff       (20)     7272 2024-04-25 15:56:30.000000 pyrisco-0.6.1/pyrisco/local/risco_local.py
--rw-r--r--   0 onfreund   (501) staff       (20)     5161 2024-04-25 15:57:15.000000 pyrisco-0.6.1/pyrisco/local/risco_socket.py
--rw-r--r--   0 onfreund   (501) staff       (20)     1097 2024-03-23 09:28:48.000000 pyrisco-0.6.1/pyrisco/local/system.py
--rw-r--r--   0 onfreund   (501) staff       (20)     1647 2022-11-04 12:33:58.000000 pyrisco-0.6.1/pyrisco/local/zone.py
-drwxr-xr-x   0 onfreund   (501) staff       (20)        0 2024-04-25 15:59:24.624192 pyrisco-0.6.1/pyrisco.egg-info/
--rw-r--r--   0 onfreund   (501) staff       (20)     3030 2024-04-25 15:59:24.000000 pyrisco-0.6.1/pyrisco.egg-info/PKG-INFO
--rw-r--r--   0 onfreund   (501) staff       (20)      614 2024-04-25 15:59:24.000000 pyrisco-0.6.1/pyrisco.egg-info/SOURCES.txt
--rw-r--r--   0 onfreund   (501) staff       (20)        1 2024-04-25 15:59:24.000000 pyrisco-0.6.1/pyrisco.egg-info/dependency_links.txt
--rw-r--r--   0 onfreund   (501) staff       (20)        8 2024-04-25 15:59:24.000000 pyrisco-0.6.1/pyrisco.egg-info/requires.txt
--rw-r--r--   0 onfreund   (501) staff       (20)        8 2024-04-25 15:59:24.000000 pyrisco-0.6.1/pyrisco.egg-info/top_level.txt
--rw-r--r--   0 onfreund   (501) staff       (20)       38 2024-04-25 15:59:24.626712 pyrisco-0.6.1/setup.cfg
--rw-r--r--   0 onfreund   (501) staff       (20)     3379 2024-04-25 15:57:47.000000 pyrisco-0.6.1/setup.py
+drwxr-xr-x   0 onfreund   (501) staff       (20)        0 2024-05-16 05:05:53.268073 pyrisco-0.6.2/
+-rw-r--r--   0 onfreund   (501) staff       (20)     1065 2021-08-21 12:09:24.000000 pyrisco-0.6.2/LICENSE
+-rw-r--r--   0 onfreund   (501) staff       (20)       25 2021-08-21 12:09:24.000000 pyrisco-0.6.2/MANIFEST.in
+-rw-r--r--   0 onfreund   (501) staff       (20)     3030 2024-05-16 05:05:53.267344 pyrisco-0.6.2/PKG-INFO
+-rw-r--r--   0 onfreund   (501) staff       (20)     2363 2022-07-23 14:50:37.000000 pyrisco-0.6.2/README.md
+drwxr-xr-x   0 onfreund   (501) staff       (20)        0 2024-05-16 05:05:53.246632 pyrisco-0.6.2/pyrisco/
+-rw-r--r--   0 onfreund   (501) staff       (20)      148 2022-07-23 14:51:59.000000 pyrisco-0.6.2/pyrisco/__init__.py
+drwxr-xr-x   0 onfreund   (501) staff       (20)        0 2024-05-16 05:05:53.255103 pyrisco-0.6.2/pyrisco/cloud/
+-rw-r--r--   0 onfreund   (501) staff       (20)       36 2022-07-23 14:51:32.000000 pyrisco-0.6.2/pyrisco/cloud/__init__.py
+-rw-r--r--   0 onfreund   (501) staff       (20)      687 2022-07-23 08:48:17.000000 pyrisco-0.6.2/pyrisco/cloud/alarm.py
+-rw-r--r--   0 onfreund   (501) staff       (20)     1860 2022-07-23 08:48:17.000000 pyrisco-0.6.2/pyrisco/cloud/event.py
+-rw-r--r--   0 onfreund   (501) staff       (20)     1532 2022-07-23 08:48:17.000000 pyrisco-0.6.2/pyrisco/cloud/partition.py
+-rw-r--r--   0 onfreund   (501) staff       (20)     6109 2022-08-03 19:38:59.000000 pyrisco-0.6.2/pyrisco/cloud/risco_cloud.py
+-rw-r--r--   0 onfreund   (501) staff       (20)      790 2022-07-23 08:48:17.000000 pyrisco-0.6.2/pyrisco/cloud/zone.py
+-rw-r--r--   0 onfreund   (501) staff       (20)     2891 2024-03-23 09:28:16.000000 pyrisco-0.6.2/pyrisco/common.py
+drwxr-xr-x   0 onfreund   (501) staff       (20)        0 2024-05-16 05:05:53.265435 pyrisco-0.6.2/pyrisco/local/
+-rw-r--r--   0 onfreund   (501) staff       (20)       36 2022-07-23 14:52:55.000000 pyrisco-0.6.2/pyrisco/local/__init__.py
+-rw-r--r--   0 onfreund   (501) staff       (20)      161 2022-07-23 08:48:17.000000 pyrisco-0.6.2/pyrisco/local/const.py
+-rw-r--r--   0 onfreund   (501) staff       (20)     1969 2024-02-14 09:05:38.000000 pyrisco-0.6.2/pyrisco/local/panels.py
+-rw-r--r--   0 onfreund   (501) staff       (20)     1849 2022-07-27 14:11:25.000000 pyrisco-0.6.2/pyrisco/local/partition.py
+-rw-r--r--   0 onfreund   (501) staff       (20)     5365 2022-09-15 12:11:59.000000 pyrisco-0.6.2/pyrisco/local/risco_crypt.py
+-rw-r--r--   0 onfreund   (501) staff       (20)     7272 2024-05-16 05:03:20.000000 pyrisco-0.6.2/pyrisco/local/risco_local.py
+-rw-r--r--   0 onfreund   (501) staff       (20)     5161 2024-04-25 15:57:15.000000 pyrisco-0.6.2/pyrisco/local/risco_socket.py
+-rw-r--r--   0 onfreund   (501) staff       (20)     1097 2024-03-23 09:28:48.000000 pyrisco-0.6.2/pyrisco/local/system.py
+-rw-r--r--   0 onfreund   (501) staff       (20)     1647 2022-11-04 12:33:58.000000 pyrisco-0.6.2/pyrisco/local/zone.py
+drwxr-xr-x   0 onfreund   (501) staff       (20)        0 2024-05-16 05:05:53.266484 pyrisco-0.6.2/pyrisco.egg-info/
+-rw-r--r--   0 onfreund   (501) staff       (20)     3030 2024-05-16 05:05:53.000000 pyrisco-0.6.2/pyrisco.egg-info/PKG-INFO
+-rw-r--r--   0 onfreund   (501) staff       (20)      614 2024-05-16 05:05:53.000000 pyrisco-0.6.2/pyrisco.egg-info/SOURCES.txt
+-rw-r--r--   0 onfreund   (501) staff       (20)        1 2024-05-16 05:05:53.000000 pyrisco-0.6.2/pyrisco.egg-info/dependency_links.txt
+-rw-r--r--   0 onfreund   (501) staff       (20)        8 2024-05-16 05:05:53.000000 pyrisco-0.6.2/pyrisco.egg-info/requires.txt
+-rw-r--r--   0 onfreund   (501) staff       (20)        8 2024-05-16 05:05:53.000000 pyrisco-0.6.2/pyrisco.egg-info/top_level.txt
+-rw-r--r--   0 onfreund   (501) staff       (20)       38 2024-05-16 05:05:53.268222 pyrisco-0.6.2/setup.cfg
+-rw-r--r--   0 onfreund   (501) staff       (20)     3379 2024-05-16 05:03:47.000000 pyrisco-0.6.2/setup.py
```

### Comparing `pyrisco-0.6.1/LICENSE` & `pyrisco-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyrisco-0.6.1/PKG-INFO` & `pyrisco-0.6.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrisco
-Version: 0.6.1
+Version: 0.6.2
 Summary: A python library to communicate with Risco Cloud.
 Home-page: https://github.com/OnFreund/PyRisco
 Author: On Freund
 Author-email: onfreund@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `pyrisco-0.6.1/README.md` & `pyrisco-0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `pyrisco-0.6.1/pyrisco/cloud/alarm.py` & `pyrisco-0.6.2/pyrisco/cloud/alarm.py`

 * *Files identical despite different names*

### Comparing `pyrisco-0.6.1/pyrisco/cloud/event.py` & `pyrisco-0.6.2/pyrisco/cloud/event.py`

 * *Files identical despite different names*

### Comparing `pyrisco-0.6.1/pyrisco/cloud/partition.py` & `pyrisco-0.6.2/pyrisco/cloud/partition.py`

 * *Files identical despite different names*

### Comparing `pyrisco-0.6.1/pyrisco/cloud/risco_cloud.py` & `pyrisco-0.6.2/pyrisco/cloud/risco_cloud.py`

 * *Files identical despite different names*

### Comparing `pyrisco-0.6.1/pyrisco/cloud/zone.py` & `pyrisco-0.6.2/pyrisco/cloud/zone.py`

 * *Files identical despite different names*

### Comparing `pyrisco-0.6.1/pyrisco/common.py` & `pyrisco-0.6.2/pyrisco/common.py`

 * *Files identical despite different names*

### Comparing `pyrisco-0.6.1/pyrisco/local/panels.py` & `pyrisco-0.6.2/pyrisco/local/panels.py`

 * *Files identical despite different names*

### Comparing `pyrisco-0.6.1/pyrisco/local/partition.py` & `pyrisco-0.6.2/pyrisco/local/partition.py`

 * *Files identical despite different names*

### Comparing `pyrisco-0.6.1/pyrisco/local/risco_crypt.py` & `pyrisco-0.6.2/pyrisco/local/risco_crypt.py`

 * *Files identical despite different names*

### Comparing `pyrisco-0.6.1/pyrisco/local/risco_local.py` & `pyrisco-0.6.2/pyrisco/local/risco_local.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -32,17 +32,17 @@
     self._legacy_panel = not panel_type.startswith("RP")
     if self._legacy_panel:
       firmware = ""
     else:
       firmware = await self._rs.send_result_command("FSVER?")
     self._panel_capabilities = panel_capabilities(panel_type, firmware)
     self._id = await self._rs.send_result_command("PNLSERD")
-    self._system = await self._init_system()
     self._zones = await self._init_zones()
     self._partitions = await self._init_partitions()
+    self._system = await self._init_system()
     self._listen_task = asyncio.create_task(self._listen(self._rs.queue))
 
   async def disconnect(self):
     await self._rs.disconnect()
     self._listen_task.cancel()
     self._listen_task = None
```

### Comparing `pyrisco-0.6.1/pyrisco/local/risco_socket.py` & `pyrisco-0.6.2/pyrisco/local/risco_socket.py`

 * *Files identical despite different names*

### Comparing `pyrisco-0.6.1/pyrisco/local/system.py` & `pyrisco-0.6.2/pyrisco/local/system.py`

 * *Files identical despite different names*

### Comparing `pyrisco-0.6.1/pyrisco/local/zone.py` & `pyrisco-0.6.2/pyrisco/local/zone.py`

 * *Files identical despite different names*

### Comparing `pyrisco-0.6.1/pyrisco.egg-info/PKG-INFO` & `pyrisco-0.6.2/pyrisco.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrisco
-Version: 0.6.1
+Version: 0.6.2
 Summary: A python library to communicate with Risco Cloud.
 Home-page: https://github.com/OnFreund/PyRisco
 Author: On Freund
 Author-email: onfreund@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `pyrisco-0.6.1/pyrisco.egg-info/SOURCES.txt` & `pyrisco-0.6.2/pyrisco.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyrisco-0.6.1/setup.py` & `pyrisco-0.6.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # Package meta-data.
 NAME = 'pyrisco'
 DESCRIPTION = 'A python library to communicate with Risco Cloud.'
 URL = 'https://github.com/OnFreund/PyRisco'
 EMAIL = 'onfreund@gmail.com'
 AUTHOR = 'On Freund'
 REQUIRES_PYTHON = '>=3.7.0'
-VERSION = '0.6.1'
+VERSION = '0.6.2'
 
 REQUIRED = ['aiohttp']
 
 EXTRAS = {}
 
 
 here = os.path.abspath(os.path.dirname(__file__))
```

