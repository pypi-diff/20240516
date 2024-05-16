# Comparing `tmp/miservice_fork-2.4.3.tar.gz` & `tmp/miservice_fork-2.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "miservice_fork-2.4.3.tar", last modified: Mon Apr 15 03:45:06 2024, max compression
+gzip compressed data, was "miservice_fork-2.4.4.tar", last modified: Thu May 16 00:06:45 2024, max compression
```

## Comparing `miservice_fork-2.4.3.tar` & `miservice_fork-2.4.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 yihong    (1000) yihong    (1000)        0 2024-04-15 03:45:06.059708 miservice_fork-2.4.3/
--rw-rw-r--   0 yihong    (1000) yihong    (1000)     1067 2024-04-15 03:38:01.000000 miservice_fork-2.4.3/LICENSE
--rw-r--r--   0 yihong    (1000) yihong    (1000)      529 2024-04-15 03:45:06.059708 miservice_fork-2.4.3/PKG-INFO
--rw-rw-r--   0 yihong    (1000) yihong    (1000)     4587 2024-04-15 03:44:37.000000 miservice_fork-2.4.3/README.md
--rwxrwxr-x   0 yihong    (1000) yihong    (1000)       96 2024-04-15 03:38:01.000000 miservice_fork-2.4.3/micli.py
-drwxrwxr-x   0 yihong    (1000) yihong    (1000)        0 2024-04-15 03:45:06.055708 miservice_fork-2.4.3/miservice/
--rwxrwxr-x   0 yihong    (1000) yihong    (1000)      178 2024-04-15 03:38:01.000000 miservice_fork-2.4.3/miservice/__init__.py
--rw-rw-r--   0 yihong    (1000) yihong    (1000)       95 2024-04-15 03:38:01.000000 miservice_fork-2.4.3/miservice/__main__.py
--rw-rw-r--   0 yihong    (1000) yihong    (1000)     7911 2024-04-15 03:44:37.000000 miservice_fork-2.4.3/miservice/cli.py
--rwxrwxr-x   0 yihong    (1000) yihong    (1000)     5647 2024-04-15 03:38:01.000000 miservice_fork-2.4.3/miservice/miaccount.py
--rwxrwxr-x   0 yihong    (1000) yihong    (1000)     3818 2024-04-15 03:38:01.000000 miservice_fork-2.4.3/miservice/miiocommand.py
--rwxrwxr-x   0 yihong    (1000) yihong    (1000)    10620 2024-04-15 03:38:01.000000 miservice_fork-2.4.3/miservice/miioservice.py
--rw-rw-r--   0 yihong    (1000) yihong    (1000)     4251 2024-04-15 03:38:01.000000 miservice_fork-2.4.3/miservice/minaservice.py
-drwxrwxr-x   0 yihong    (1000) yihong    (1000)        0 2024-04-15 03:45:06.059708 miservice_fork-2.4.3/miservice_fork.egg-info/
--rw-r--r--   0 yihong    (1000) yihong    (1000)      529 2024-04-15 03:45:06.000000 miservice_fork-2.4.3/miservice_fork.egg-info/PKG-INFO
--rw-rw-r--   0 yihong    (1000) yihong    (1000)      424 2024-04-15 03:45:06.000000 miservice_fork-2.4.3/miservice_fork.egg-info/SOURCES.txt
--rw-rw-r--   0 yihong    (1000) yihong    (1000)        1 2024-04-15 03:45:06.000000 miservice_fork-2.4.3/miservice_fork.egg-info/dependency_links.txt
--rw-rw-r--   0 yihong    (1000) yihong    (1000)       46 2024-04-15 03:45:06.000000 miservice_fork-2.4.3/miservice_fork.egg-info/entry_points.txt
--rw-rw-r--   0 yihong    (1000) yihong    (1000)       21 2024-04-15 03:45:06.000000 miservice_fork-2.4.3/miservice_fork.egg-info/requires.txt
--rw-rw-r--   0 yihong    (1000) yihong    (1000)       10 2024-04-15 03:45:06.000000 miservice_fork-2.4.3/miservice_fork.egg-info/top_level.txt
--rw-rw-r--   0 yihong    (1000) yihong    (1000)       38 2024-04-15 03:45:06.059708 miservice_fork-2.4.3/setup.cfg
--rwxrwxr-x   0 yihong    (1000) yihong    (1000)      919 2024-04-15 03:44:53.000000 miservice_fork-2.4.3/setup.py
+drwxr-xr-x   0 hyi        (502) staff       (20)        0 2024-05-16 00:06:45.508926 miservice_fork-2.4.4/
+-rw-r--r--   0 hyi        (502) staff       (20)     1067 2023-03-11 14:21:43.000000 miservice_fork-2.4.4/LICENSE
+-rw-r--r--   0 hyi        (502) staff       (20)      529 2024-05-16 00:06:45.508471 miservice_fork-2.4.4/PKG-INFO
+-rw-r--r--   0 hyi        (502) staff       (20)     4587 2024-05-16 00:06:29.000000 miservice_fork-2.4.4/README.md
+-rwxr-xr-x   0 hyi        (502) staff       (20)       96 2023-07-31 09:48:54.000000 miservice_fork-2.4.4/micli.py
+drwxr-xr-x   0 hyi        (502) staff       (20)        0 2024-05-16 00:06:45.503200 miservice_fork-2.4.4/miservice/
+-rwxr-xr-x   0 hyi        (502) staff       (20)      178 2023-03-12 07:11:31.000000 miservice_fork-2.4.4/miservice/__init__.py
+-rw-r--r--   0 hyi        (502) staff       (20)       95 2023-03-11 14:21:43.000000 miservice_fork-2.4.4/miservice/__main__.py
+-rw-r--r--   0 hyi        (502) staff       (20)     7911 2024-05-16 00:06:29.000000 miservice_fork-2.4.4/miservice/cli.py
+-rwxr-xr-x   0 hyi        (502) staff       (20)     5647 2023-10-23 08:06:30.000000 miservice_fork-2.4.4/miservice/miaccount.py
+-rwxr-xr-x   0 hyi        (502) staff       (20)     3818 2024-01-07 08:08:03.000000 miservice_fork-2.4.4/miservice/miiocommand.py
+-rwxr-xr-x   0 hyi        (502) staff       (20)    10620 2024-01-29 05:33:41.000000 miservice_fork-2.4.4/miservice/miioservice.py
+-rw-r--r--   0 hyi        (502) staff       (20)     4264 2024-05-16 00:06:29.000000 miservice_fork-2.4.4/miservice/minaservice.py
+drwxr-xr-x   0 hyi        (502) staff       (20)        0 2024-05-16 00:06:45.507814 miservice_fork-2.4.4/miservice_fork.egg-info/
+-rw-r--r--   0 hyi        (502) staff       (20)      529 2024-05-16 00:06:45.000000 miservice_fork-2.4.4/miservice_fork.egg-info/PKG-INFO
+-rw-r--r--   0 hyi        (502) staff       (20)      424 2024-05-16 00:06:45.000000 miservice_fork-2.4.4/miservice_fork.egg-info/SOURCES.txt
+-rw-r--r--   0 hyi        (502) staff       (20)        1 2024-05-16 00:06:45.000000 miservice_fork-2.4.4/miservice_fork.egg-info/dependency_links.txt
+-rw-r--r--   0 hyi        (502) staff       (20)       46 2024-05-16 00:06:45.000000 miservice_fork-2.4.4/miservice_fork.egg-info/entry_points.txt
+-rw-r--r--   0 hyi        (502) staff       (20)       21 2024-05-16 00:06:45.000000 miservice_fork-2.4.4/miservice_fork.egg-info/requires.txt
+-rw-r--r--   0 hyi        (502) staff       (20)       10 2024-05-16 00:06:45.000000 miservice_fork-2.4.4/miservice_fork.egg-info/top_level.txt
+-rw-r--r--   0 hyi        (502) staff       (20)       38 2024-05-16 00:06:45.508976 miservice_fork-2.4.4/setup.cfg
+-rwxr-xr-x   0 hyi        (502) staff       (20)      919 2024-05-16 00:06:38.000000 miservice_fork-2.4.4/setup.py
```

### Comparing `miservice_fork-2.4.3/LICENSE` & `miservice_fork-2.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `miservice_fork-2.4.3/PKG-INFO` & `miservice_fork-2.4.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: miservice_fork
-Version: 2.4.3
+Version: 2.4.4
 Summary: XiaoMi Cloud Service fork from https://github.com/Yonsm/MiService
 Home-page: https://github.com/yihong0618/MiService
 Author: Yonsm, yihong0618
 Author-email: Yonsm@qq.com, zouzou0208@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `miservice_fork-2.4.3/README.md` & `miservice_fork-2.4.4/README.md`

 * *Files identical despite different names*

### Comparing `miservice_fork-2.4.3/miservice/cli.py` & `miservice_fork-2.4.4/miservice/cli.py`

 * *Files identical despite different names*

### Comparing `miservice_fork-2.4.3/miservice/miaccount.py` & `miservice_fork-2.4.4/miservice/miaccount.py`

 * *Files identical despite different names*

### Comparing `miservice_fork-2.4.3/miservice/miiocommand.py` & `miservice_fork-2.4.4/miservice/miiocommand.py`

 * *Files identical despite different names*

### Comparing `miservice_fork-2.4.3/miservice/miioservice.py` & `miservice_fork-2.4.4/miservice/miioservice.py`

 * *Files identical despite different names*

### Comparing `miservice_fork-2.4.3/miservice/minaservice.py` & `miservice_fork-2.4.4/miservice/minaservice.py`

 * *Files 1% similar despite different names*

```diff
@@ -92,20 +92,20 @@
         return await self.ubus_request(
             deviceId,
             "player_set_loop",
             "mediaplayer",
             {"media": "common", "type": type},
         )
 
-    async def play_by_url(self, deviceId, url):
+    async def play_by_url(self, deviceId, url, _type=2):
         return await self.ubus_request(
             deviceId,
             "player_play_url",
             "mediaplayer",
-            {"url": url, "type": 1, "media": "app_ios"},
+            {"url": url, "type": _type, "media": "app_ios"},
         )
 
     async def send_message(self, devices, devno, message, volume=None):  # -1/0/1...
         result = False
         for i in range(0, len(devices)):
             if (
                 devno == -1
```

### Comparing `miservice_fork-2.4.3/miservice_fork.egg-info/PKG-INFO` & `miservice_fork-2.4.4/miservice_fork.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: miservice_fork
-Version: 2.4.3
+Version: 2.4.4
 Summary: XiaoMi Cloud Service fork from https://github.com/Yonsm/MiService
 Home-page: https://github.com/yihong0618/MiService
 Author: Yonsm, yihong0618
 Author-email: Yonsm@qq.com, zouzou0208@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `miservice_fork-2.4.3/setup.py` & `miservice_fork-2.4.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 
 from setuptools import setup
 
 setup(
     name="miservice_fork",
     description="XiaoMi Cloud Service fork from https://github.com/Yonsm/MiService",
-    version="2.4.3",
+    version="2.4.4",
     license="MIT",
     author="Yonsm, yihong0618",
     author_email="Yonsm@qq.com, zouzou0208@gmail.com",
     url="https://github.com/yihong0618/MiService",
     packages=["miservice"],
     scripts=["micli.py"],
     python_requires=">=3.7",
```

