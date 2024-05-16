# Comparing `tmp/tsugu-api-python-1.1.5.tar.gz` & `tmp/tsugu-api-python-1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tsugu-api-python-1.1.5.tar", last modified: Thu May 16 00:55:15 2024, max compression
+gzip compressed data, was "tsugu-api-python-1.1.6.tar", last modified: Thu May 16 01:11:04 2024, max compression
```

## Comparing `tsugu-api-python-1.1.5.tar` & `tsugu-api-python-1.1.6.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 00:55:15.089806 tsugu-api-python-1.1.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-16 00:55:04.000000 tsugu-api-python-1.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6199 2024-05-16 00:55:15.089806 tsugu-api-python-1.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4593 2024-05-16 00:55:04.000000 tsugu-api-python-1.1.5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 00:55:15.089806 tsugu-api-python-1.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      846 2024-05-16 00:55:04.000000 tsugu-api-python-1.1.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 00:55:15.085806 tsugu-api-python-1.1.5/tsugu_api/
--rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-05-16 00:55:04.000000 tsugu-api-python-1.1.5/tsugu_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1582 2024-05-16 00:55:04.000000 tsugu-api-python-1.1.5/tsugu_api/_bandoristation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2835 2024-05-16 00:55:04.000000 tsugu-api-python-1.1.5/tsugu_api/_network.py
--rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-05-16 00:55:04.000000 tsugu-api-python-1.1.5/tsugu_api/_station.py
--rw-r--r--   0 runner    (1001) docker     (127)     9395 2024-05-16 00:55:04.000000 tsugu-api-python-1.1.5/tsugu_api/_tsugu.py
--rw-r--r--   0 runner    (1001) docker     (127)     3124 2024-05-16 00:55:04.000000 tsugu-api-python-1.1.5/tsugu_api/_typing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3344 2024-05-16 00:55:04.000000 tsugu-api-python-1.1.5/tsugu_api/_user.py
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-16 00:55:04.000000 tsugu-api-python-1.1.5/tsugu_api/exception.py
--rw-r--r--   0 runner    (1001) docker     (127)     1908 2024-05-16 00:55:04.000000 tsugu-api-python-1.1.5/tsugu_api/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-05-16 00:55:04.000000 tsugu-api-python-1.1.5/tsugu_api/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 00:55:15.089806 tsugu-api-python-1.1.5/tsugu_api_async/
--rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-05-16 00:55:04.000000 tsugu-api-python-1.1.5/tsugu_api_async/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1870 2024-05-16 00:55:04.000000 tsugu-api-python-1.1.5/tsugu_api_async/_bandoristation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3769 2024-05-16 00:55:04.000000 tsugu-api-python-1.1.5/tsugu_api_async/_network.py
--rw-r--r--   0 runner    (1001) docker     (127)     1882 2024-05-16 00:55:04.000000 tsugu-api-python-1.1.5/tsugu_api_async/_station.py
--rw-r--r--   0 runner    (1001) docker     (127)    11001 2024-05-16 00:55:04.000000 tsugu-api-python-1.1.5/tsugu_api_async/_tsugu.py
--rw-r--r--   0 runner    (1001) docker     (127)     3246 2024-05-16 00:55:04.000000 tsugu-api-python-1.1.5/tsugu_api_async/_typing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3805 2024-05-16 00:55:04.000000 tsugu-api-python-1.1.5/tsugu_api_async/_user.py
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-16 00:55:04.000000 tsugu-api-python-1.1.5/tsugu_api_async/exception.py
--rw-r--r--   0 runner    (1001) docker     (127)     2115 2024-05-16 00:55:04.000000 tsugu-api-python-1.1.5/tsugu_api_async/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     1263 2024-05-16 00:55:04.000000 tsugu-api-python-1.1.5/tsugu_api_async/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 00:55:15.089806 tsugu-api-python-1.1.5/tsugu_api_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6199 2024-05-16 00:55:14.000000 tsugu-api-python-1.1.5/tsugu_api_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      723 2024-05-16 00:55:15.000000 tsugu-api-python-1.1.5/tsugu_api_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 00:55:14.000000 tsugu-api-python-1.1.5/tsugu_api_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-16 00:55:14.000000 tsugu-api-python-1.1.5/tsugu_api_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-16 00:55:14.000000 tsugu-api-python-1.1.5/tsugu_api_python.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 01:11:04.701051 tsugu-api-python-1.1.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-16 01:10:53.000000 tsugu-api-python-1.1.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6199 2024-05-16 01:11:04.701051 tsugu-api-python-1.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4593 2024-05-16 01:10:53.000000 tsugu-api-python-1.1.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 01:11:04.701051 tsugu-api-python-1.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      846 2024-05-16 01:10:53.000000 tsugu-api-python-1.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 01:11:04.697051 tsugu-api-python-1.1.6/tsugu_api/
+-rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-05-16 01:10:53.000000 tsugu-api-python-1.1.6/tsugu_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1582 2024-05-16 01:10:53.000000 tsugu-api-python-1.1.6/tsugu_api/_bandoristation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2835 2024-05-16 01:10:53.000000 tsugu-api-python-1.1.6/tsugu_api/_network.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-05-16 01:10:53.000000 tsugu-api-python-1.1.6/tsugu_api/_station.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9433 2024-05-16 01:10:53.000000 tsugu-api-python-1.1.6/tsugu_api/_tsugu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3124 2024-05-16 01:10:53.000000 tsugu-api-python-1.1.6/tsugu_api/_typing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3344 2024-05-16 01:10:53.000000 tsugu-api-python-1.1.6/tsugu_api/_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-16 01:10:53.000000 tsugu-api-python-1.1.6/tsugu_api/exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1908 2024-05-16 01:10:53.000000 tsugu-api-python-1.1.6/tsugu_api/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-05-16 01:10:53.000000 tsugu-api-python-1.1.6/tsugu_api/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 01:11:04.701051 tsugu-api-python-1.1.6/tsugu_api_async/
+-rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-05-16 01:10:53.000000 tsugu-api-python-1.1.6/tsugu_api_async/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1870 2024-05-16 01:10:53.000000 tsugu-api-python-1.1.6/tsugu_api_async/_bandoristation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3769 2024-05-16 01:10:53.000000 tsugu-api-python-1.1.6/tsugu_api_async/_network.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1882 2024-05-16 01:10:53.000000 tsugu-api-python-1.1.6/tsugu_api_async/_station.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11039 2024-05-16 01:10:53.000000 tsugu-api-python-1.1.6/tsugu_api_async/_tsugu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3246 2024-05-16 01:10:53.000000 tsugu-api-python-1.1.6/tsugu_api_async/_typing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3805 2024-05-16 01:10:53.000000 tsugu-api-python-1.1.6/tsugu_api_async/_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-16 01:10:53.000000 tsugu-api-python-1.1.6/tsugu_api_async/exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2115 2024-05-16 01:10:53.000000 tsugu-api-python-1.1.6/tsugu_api_async/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1263 2024-05-16 01:10:53.000000 tsugu-api-python-1.1.6/tsugu_api_async/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 01:11:04.701051 tsugu-api-python-1.1.6/tsugu_api_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6199 2024-05-16 01:11:04.000000 tsugu-api-python-1.1.6/tsugu_api_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      723 2024-05-16 01:11:04.000000 tsugu-api-python-1.1.6/tsugu_api_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 01:11:04.000000 tsugu-api-python-1.1.6/tsugu_api_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-16 01:11:04.000000 tsugu-api-python-1.1.6/tsugu_api_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-16 01:11:04.000000 tsugu-api-python-1.1.6/tsugu_api_python.egg-info/top_level.txt
```

### Comparing `tsugu-api-python-1.1.5/LICENSE` & `tsugu-api-python-1.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `tsugu-api-python-1.1.5/PKG-INFO` & `tsugu-api-python-1.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tsugu-api-python
-Version: 1.1.5
+Version: 1.1.6
 Summary: Tsugu BanGDream Bot 的功能 API 统合包
 Home-page: https://github.com/WindowsSov8forUs/tsugu-api-python
 Author: WindowsSov8
 Author-email: qwertyuiop2333@hotmail.com
 License: MIT
 Description: <div align="center">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: tsugu-api-python Version: 1.1.5 Summary: Tsugu
+Metadata-Version: 2.1 Name: tsugu-api-python Version: 1.1.6 Summary: Tsugu
 BanGDream Bot çåè½ API ç»åå Home-page: https://github.com/
 WindowsSov8forUs/tsugu-api-python Author: WindowsSov8 Author-email:
 qwertyuiop2333@hotmail.com License: MIT Description:
  ![tsugu-api-ython logo](https://github.com/WindowsSov8forUs/tsugu-api-python/
          blob/main/logo.png) # tsugu-api-python _â¨ Python ç¼åç
       [TsuguBanGDreamBot](https://github.com/Yamamoto-2/tsugu-bangdream-
          bot?tab=readme-ov-file) ç¸å³åç§åè½ API è°ç¨åº â¨_
```

### Comparing `tsugu-api-python-1.1.5/README.md` & `tsugu-api-python-1.1.6/README.md`

 * *Files identical despite different names*

### Comparing `tsugu-api-python-1.1.5/setup.py` & `tsugu-api-python-1.1.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open('README.md', 'r', encoding='utf-8') as readme:
     long_description = readme.read()
 
 setup(
     name='tsugu-api-python',
-    version='1.1.5',
+    version='1.1.6',
     author='WindowsSov8',
     author_email='qwertyuiop2333@hotmail.com',
     description='Tsugu BanGDream Bot 的功能 API 统合包',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/WindowsSov8forUs/tsugu-api-python',
     include_package_data=False,
```

### Comparing `tsugu-api-python-1.1.5/tsugu_api/__init__.py` & `tsugu-api-python-1.1.6/tsugu_api/__init__.py`

 * *Files identical despite different names*

### Comparing `tsugu-api-python-1.1.5/tsugu_api/_bandoristation.py` & `tsugu-api-python-1.1.6/tsugu_api/_bandoristation.py`

 * *Files identical despite different names*

### Comparing `tsugu-api-python-1.1.5/tsugu_api/_network.py` & `tsugu-api-python-1.1.6/tsugu_api/_network.py`

 * *Files identical despite different names*

### Comparing `tsugu-api-python-1.1.5/tsugu_api/_station.py` & `tsugu-api-python-1.1.6/tsugu_api/_station.py`

 * *Files identical despite different names*

### Comparing `tsugu-api-python-1.1.5/tsugu_api/_tsugu.py` & `tsugu-api-python-1.1.6/tsugu_api/_tsugu.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import List, Optional
+from typing import List, Optional, Sequence
 
 from tsugu_api import settings
 from tsugu_api._network import Api
 from tsugu_api._typing import (
     _Room,
     _Server,
     _Response,
@@ -145,15 +145,15 @@
     
     # 发送请求
     return Api(
         url,
         proxy=settings.backend_proxy
     ).post(data).json()
 
-def search_card(default_servers: List[_Server], text: str) -> _Response:
+def search_card(default_servers: Sequence[_Server], text: str) -> _Response:
     '''查询卡片
 
     参数:
         default_servers (list[_Server]): 默认服务器
         text (str): 查询参数
 
     返回:
@@ -173,15 +173,15 @@
     
     # 发送请求
     return Api(
         url,
         proxy=settings.backend_proxy
     ).post(data).json()
 
-def search_character(default_servers: List[_Server], text: str) -> _Response:
+def search_character(default_servers: Sequence[_Server], text: str) -> _Response:
     '''查询角色
 
     参数:
         default_servers (list[_Server]): 默认服务器
         text (str): 查询参数
 
     返回:
@@ -200,15 +200,15 @@
     
     # 发送请求
     return Api(
         url,
         proxy=settings.backend_proxy
     ).post(data).json()
 
-def search_event(default_servers: List[_Server], text: str) -> _Response:
+def search_event(default_servers: Sequence[_Server], text: str) -> _Response:
     '''查询活动
 
     参数:
         default_servers (list[_Server]): 默认服务器
         text (str): 查询参数
 
     返回:
@@ -228,15 +228,15 @@
     
     # 发送请求
     return Api(
         url,
         proxy=settings.backend_proxy
     ).post(data).json()
 
-def search_gacha(default_servers: List[_Server], gacha_id: int) -> _Response:
+def search_gacha(default_servers: Sequence[_Server], gacha_id: int) -> _Response:
     '''查询卡池
 
     参数:
         default_servers (list[_Server]): 默认服务器
         gacha_id (int): 卡池 ID
 
     返回:
@@ -284,15 +284,15 @@
     
     # 发送请求
     return Api(
         url,
         proxy=settings.backend_proxy
     ).post(data).json()
 
-def search_song(default_servers: List[_Server], text: str) -> _Response:
+def search_song(default_servers: Sequence[_Server], text: str) -> _Response:
     '''查询歌曲
 
     参数:
         default_servers (list[_Server]): 默认服务器
         text (str): 查询参数
 
     返回:
@@ -311,15 +311,15 @@
     
     # 发送请求
     return Api(
         url,
         proxy=settings.backend_proxy
     ).post(data).json()
 
-def song_chart(default_servers: List[_Server], song_id: int, difficulty_text: _DifficultyText) -> _Response:
+def song_chart(default_servers: Sequence[_Server], song_id: int, difficulty_text: _DifficultyText) -> _Response:
     '''查询歌曲谱面
 
     参数:
         default_servers (list[_Server]): 默认服务器
         song_id (int): 歌曲 ID
         difficulty_text (_Difficulty): 谱面难度
 
@@ -340,15 +340,15 @@
     
     # 发送请求
     return Api(
         url,
         proxy=settings.backend_proxy
     ).post(data).json()
 
-def song_meta(default_servers: List[_Server], server: _Server) -> _Response:
+def song_meta(default_servers: Sequence[_Server], server: _Server) -> _Response:
     '''查询歌曲分数表
 
     参数:
         default_servers (list[_Server]): 默认服务器
         server (_Server): 主服务器
 
     返回:
```

### Comparing `tsugu-api-python-1.1.5/tsugu_api/_typing.py` & `tsugu-api-python-1.1.6/tsugu_api/_typing.py`

 * *Files identical despite different names*

### Comparing `tsugu-api-python-1.1.5/tsugu_api/_user.py` & `tsugu-api-python-1.1.6/tsugu_api/_user.py`

 * *Files identical despite different names*

### Comparing `tsugu-api-python-1.1.5/tsugu_api/settings.py` & `tsugu-api-python-1.1.6/tsugu_api/settings.py`

 * *Files identical despite different names*

### Comparing `tsugu-api-python-1.1.5/tsugu_api/utils.py` & `tsugu-api-python-1.1.6/tsugu_api/utils.py`

 * *Files identical despite different names*

### Comparing `tsugu-api-python-1.1.5/tsugu_api_async/__init__.py` & `tsugu-api-python-1.1.6/tsugu_api_async/__init__.py`

 * *Files identical despite different names*

### Comparing `tsugu-api-python-1.1.5/tsugu_api_async/_bandoristation.py` & `tsugu-api-python-1.1.6/tsugu_api_async/_bandoristation.py`

 * *Files identical despite different names*

### Comparing `tsugu-api-python-1.1.5/tsugu_api_async/_network.py` & `tsugu-api-python-1.1.6/tsugu_api_async/_network.py`

 * *Files identical despite different names*

### Comparing `tsugu-api-python-1.1.5/tsugu_api_async/_station.py` & `tsugu-api-python-1.1.6/tsugu_api_async/_station.py`

 * *Files identical despite different names*

### Comparing `tsugu-api-python-1.1.5/tsugu_api_async/_tsugu.py` & `tsugu-api-python-1.1.6/tsugu_api_async/_tsugu.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import List, Optional
+from typing import List, Optional, Sequence
 
 from httpx import Response
 
 from tsugu_api_async import settings
 from tsugu_api_async._network import Api
 from tsugu_api_async._typing import (
     _Room,
@@ -157,15 +157,15 @@
     response = await Api(
         url,
         proxy=settings.backend_proxy
     ).post(data)
     if isinstance(response, Response): return response.json()
     return await response.json()
 
-async def search_card(default_servers: List[_Server], text: str) -> _Response:
+async def search_card(default_servers: Sequence[_Server], text: str) -> _Response:
     '''查询卡片
 
     参数:
         default_servers (list[_Server]): 默认服务器
         text (str): 查询参数
 
     返回:
@@ -187,15 +187,15 @@
     response = await Api(
         url,
         proxy=settings.backend_proxy
     ).post(data)
     if isinstance(response, Response): return response.json()
     return await response.json()
 
-async def search_character(default_servers: List[_Server], text: str) -> _Response:
+async def search_character(default_servers: Sequence[_Server], text: str) -> _Response:
     '''查询角色
 
     参数:
         default_servers (list[_Server]): 默认服务器
         text (str): 查询参数
 
     返回:
@@ -216,15 +216,15 @@
     response = await Api(
         url,
         proxy=settings.backend_proxy
     ).post(data)
     if isinstance(response, Response): return response.json()
     return await response.json()
 
-async def search_event(default_servers: List[_Server], text: str) -> _Response:
+async def search_event(default_servers: Sequence[_Server], text: str) -> _Response:
     '''查询活动
 
     参数:
         default_servers (list[_Server]): 默认服务器
         text (str): 查询参数
 
     返回:
@@ -246,15 +246,15 @@
     response = await Api(
         url,
         proxy=settings.backend_proxy
     ).post(data)
     if isinstance(response, Response): return response.json()
     return await response.json()
 
-async def search_gacha(default_servers: List[_Server], gacha_id: int) -> _Response:
+async def search_gacha(default_servers: Sequence[_Server], gacha_id: int) -> _Response:
     '''查询卡池
 
     参数:
         default_servers (list[_Server]): 默认服务器
         gacha_id (int): 卡池 ID
 
     返回:
@@ -306,15 +306,15 @@
     response = await Api(
         url,
         proxy=settings.backend_proxy
     ).post(data)
     if isinstance(response, Response): return response.json()
     return await response.json()
 
-async def search_song(default_servers: List[_Server], text: str) -> _Response:
+async def search_song(default_servers: Sequence[_Server], text: str) -> _Response:
     '''查询歌曲
 
     参数:
         default_servers (list[_Server]): 默认服务器
         text (str): 查询参数
 
     返回:
@@ -335,15 +335,15 @@
     response = await Api(
         url,
         proxy=settings.backend_proxy
     ).post(data)
     if isinstance(response, Response): return response.json()
     return await response.json()
 
-async def song_chart(default_servers: List[_Server], song_id: int, difficulty_text: _DifficultyText) -> _Response:
+async def song_chart(default_servers: Sequence[_Server], song_id: int, difficulty_text: _DifficultyText) -> _Response:
     '''查询歌曲谱面
 
     参数:
         default_servers (list[_Server]): 默认服务器
         song_id (int): 歌曲 ID
         difficulty_text (_Difficulty): 谱面难度
 
@@ -366,15 +366,15 @@
     response = await Api(
         url,
         proxy=settings.backend_proxy
     ).post(data)
     if isinstance(response, Response): return response.json()
     return await response.json()
 
-async def song_meta(default_servers: List[_Server], server: _Server) -> _Response:
+async def song_meta(default_servers: Sequence[_Server], server: _Server) -> _Response:
     '''查询歌曲分数表
 
     参数:
         default_servers (list[_Server]): 默认服务器
         server (_Server): 主服务器
 
     返回:
```

### Comparing `tsugu-api-python-1.1.5/tsugu_api_async/_typing.py` & `tsugu-api-python-1.1.6/tsugu_api_async/_typing.py`

 * *Files identical despite different names*

### Comparing `tsugu-api-python-1.1.5/tsugu_api_async/_user.py` & `tsugu-api-python-1.1.6/tsugu_api_async/_user.py`

 * *Files identical despite different names*

### Comparing `tsugu-api-python-1.1.5/tsugu_api_async/settings.py` & `tsugu-api-python-1.1.6/tsugu_api_async/settings.py`

 * *Files identical despite different names*

### Comparing `tsugu-api-python-1.1.5/tsugu_api_async/utils.py` & `tsugu-api-python-1.1.6/tsugu_api_async/utils.py`

 * *Files identical despite different names*

### Comparing `tsugu-api-python-1.1.5/tsugu_api_python.egg-info/PKG-INFO` & `tsugu-api-python-1.1.6/tsugu_api_python.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tsugu-api-python
-Version: 1.1.5
+Version: 1.1.6
 Summary: Tsugu BanGDream Bot 的功能 API 统合包
 Home-page: https://github.com/WindowsSov8forUs/tsugu-api-python
 Author: WindowsSov8
 Author-email: qwertyuiop2333@hotmail.com
 License: MIT
 Description: <div align="center">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: tsugu-api-python Version: 1.1.5 Summary: Tsugu
+Metadata-Version: 2.1 Name: tsugu-api-python Version: 1.1.6 Summary: Tsugu
 BanGDream Bot çåè½ API ç»åå Home-page: https://github.com/
 WindowsSov8forUs/tsugu-api-python Author: WindowsSov8 Author-email:
 qwertyuiop2333@hotmail.com License: MIT Description:
  ![tsugu-api-ython logo](https://github.com/WindowsSov8forUs/tsugu-api-python/
          blob/main/logo.png) # tsugu-api-python _â¨ Python ç¼åç
       [TsuguBanGDreamBot](https://github.com/Yamamoto-2/tsugu-bangdream-
          bot?tab=readme-ov-file) ç¸å³åç§åè½ API è°ç¨åº â¨_
```

### Comparing `tsugu-api-python-1.1.5/tsugu_api_python.egg-info/SOURCES.txt` & `tsugu-api-python-1.1.6/tsugu_api_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

