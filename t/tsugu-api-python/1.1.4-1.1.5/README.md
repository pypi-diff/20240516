# Comparing `tmp/tsugu-api-python-1.1.4.tar.gz` & `tmp/tsugu-api-python-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tsugu-api-python-1.1.4.tar", last modified: Thu May 16 00:36:43 2024, max compression
+gzip compressed data, was "tsugu-api-python-1.1.5.tar", last modified: Thu May 16 00:55:15 2024, max compression
```

## Comparing `tsugu-api-python-1.1.4.tar` & `tsugu-api-python-1.1.5.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 00:36:43.002552 tsugu-api-python-1.1.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-16 00:36:34.000000 tsugu-api-python-1.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6199 2024-05-16 00:36:43.002552 tsugu-api-python-1.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4593 2024-05-16 00:36:34.000000 tsugu-api-python-1.1.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 00:36:43.002552 tsugu-api-python-1.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      846 2024-05-16 00:36:34.000000 tsugu-api-python-1.1.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 00:36:43.002552 tsugu-api-python-1.1.4/tsugu_api/
--rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-05-16 00:36:34.000000 tsugu-api-python-1.1.4/tsugu_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1557 2024-05-16 00:36:34.000000 tsugu-api-python-1.1.4/tsugu_api/_bandoristation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2835 2024-05-16 00:36:34.000000 tsugu-api-python-1.1.4/tsugu_api/_network.py
--rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-05-16 00:36:34.000000 tsugu-api-python-1.1.4/tsugu_api/_station.py
--rw-r--r--   0 runner    (1001) docker     (127)     9389 2024-05-16 00:36:34.000000 tsugu-api-python-1.1.4/tsugu_api/_tsugu.py
--rw-r--r--   0 runner    (1001) docker     (127)     3114 2024-05-16 00:36:34.000000 tsugu-api-python-1.1.4/tsugu_api/_typing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3344 2024-05-16 00:36:34.000000 tsugu-api-python-1.1.4/tsugu_api/_user.py
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-16 00:36:34.000000 tsugu-api-python-1.1.4/tsugu_api/exception.py
--rw-r--r--   0 runner    (1001) docker     (127)     1908 2024-05-16 00:36:34.000000 tsugu-api-python-1.1.4/tsugu_api/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-05-16 00:36:34.000000 tsugu-api-python-1.1.4/tsugu_api/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 00:36:43.002552 tsugu-api-python-1.1.4/tsugu_api_async/
--rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-05-16 00:36:34.000000 tsugu-api-python-1.1.4/tsugu_api_async/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1845 2024-05-16 00:36:34.000000 tsugu-api-python-1.1.4/tsugu_api_async/_bandoristation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3769 2024-05-16 00:36:34.000000 tsugu-api-python-1.1.4/tsugu_api_async/_network.py
--rw-r--r--   0 runner    (1001) docker     (127)     1882 2024-05-16 00:36:34.000000 tsugu-api-python-1.1.4/tsugu_api_async/_station.py
--rw-r--r--   0 runner    (1001) docker     (127)    10995 2024-05-16 00:36:34.000000 tsugu-api-python-1.1.4/tsugu_api_async/_tsugu.py
--rw-r--r--   0 runner    (1001) docker     (127)     3236 2024-05-16 00:36:34.000000 tsugu-api-python-1.1.4/tsugu_api_async/_typing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3805 2024-05-16 00:36:34.000000 tsugu-api-python-1.1.4/tsugu_api_async/_user.py
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-16 00:36:34.000000 tsugu-api-python-1.1.4/tsugu_api_async/exception.py
--rw-r--r--   0 runner    (1001) docker     (127)     2115 2024-05-16 00:36:34.000000 tsugu-api-python-1.1.4/tsugu_api_async/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     1263 2024-05-16 00:36:34.000000 tsugu-api-python-1.1.4/tsugu_api_async/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 00:36:43.002552 tsugu-api-python-1.1.4/tsugu_api_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6199 2024-05-16 00:36:42.000000 tsugu-api-python-1.1.4/tsugu_api_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      723 2024-05-16 00:36:42.000000 tsugu-api-python-1.1.4/tsugu_api_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 00:36:42.000000 tsugu-api-python-1.1.4/tsugu_api_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-16 00:36:42.000000 tsugu-api-python-1.1.4/tsugu_api_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-16 00:36:42.000000 tsugu-api-python-1.1.4/tsugu_api_python.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 00:55:15.089806 tsugu-api-python-1.1.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-16 00:55:04.000000 tsugu-api-python-1.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6199 2024-05-16 00:55:15.089806 tsugu-api-python-1.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4593 2024-05-16 00:55:04.000000 tsugu-api-python-1.1.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 00:55:15.089806 tsugu-api-python-1.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      846 2024-05-16 00:55:04.000000 tsugu-api-python-1.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 00:55:15.085806 tsugu-api-python-1.1.5/tsugu_api/
+-rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-05-16 00:55:04.000000 tsugu-api-python-1.1.5/tsugu_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1582 2024-05-16 00:55:04.000000 tsugu-api-python-1.1.5/tsugu_api/_bandoristation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2835 2024-05-16 00:55:04.000000 tsugu-api-python-1.1.5/tsugu_api/_network.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-05-16 00:55:04.000000 tsugu-api-python-1.1.5/tsugu_api/_station.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9395 2024-05-16 00:55:04.000000 tsugu-api-python-1.1.5/tsugu_api/_tsugu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3124 2024-05-16 00:55:04.000000 tsugu-api-python-1.1.5/tsugu_api/_typing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3344 2024-05-16 00:55:04.000000 tsugu-api-python-1.1.5/tsugu_api/_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-16 00:55:04.000000 tsugu-api-python-1.1.5/tsugu_api/exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1908 2024-05-16 00:55:04.000000 tsugu-api-python-1.1.5/tsugu_api/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-05-16 00:55:04.000000 tsugu-api-python-1.1.5/tsugu_api/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 00:55:15.089806 tsugu-api-python-1.1.5/tsugu_api_async/
+-rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-05-16 00:55:04.000000 tsugu-api-python-1.1.5/tsugu_api_async/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1870 2024-05-16 00:55:04.000000 tsugu-api-python-1.1.5/tsugu_api_async/_bandoristation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3769 2024-05-16 00:55:04.000000 tsugu-api-python-1.1.5/tsugu_api_async/_network.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1882 2024-05-16 00:55:04.000000 tsugu-api-python-1.1.5/tsugu_api_async/_station.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11001 2024-05-16 00:55:04.000000 tsugu-api-python-1.1.5/tsugu_api_async/_tsugu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3246 2024-05-16 00:55:04.000000 tsugu-api-python-1.1.5/tsugu_api_async/_typing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3805 2024-05-16 00:55:04.000000 tsugu-api-python-1.1.5/tsugu_api_async/_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-16 00:55:04.000000 tsugu-api-python-1.1.5/tsugu_api_async/exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2115 2024-05-16 00:55:04.000000 tsugu-api-python-1.1.5/tsugu_api_async/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1263 2024-05-16 00:55:04.000000 tsugu-api-python-1.1.5/tsugu_api_async/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 00:55:15.089806 tsugu-api-python-1.1.5/tsugu_api_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6199 2024-05-16 00:55:14.000000 tsugu-api-python-1.1.5/tsugu_api_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      723 2024-05-16 00:55:15.000000 tsugu-api-python-1.1.5/tsugu_api_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 00:55:14.000000 tsugu-api-python-1.1.5/tsugu_api_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-16 00:55:14.000000 tsugu-api-python-1.1.5/tsugu_api_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-16 00:55:14.000000 tsugu-api-python-1.1.5/tsugu_api_python.egg-info/top_level.txt
```

### Comparing `tsugu-api-python-1.1.4/LICENSE` & `tsugu-api-python-1.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `tsugu-api-python-1.1.4/PKG-INFO` & `tsugu-api-python-1.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tsugu-api-python
-Version: 1.1.4
+Version: 1.1.5
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
-Metadata-Version: 2.1 Name: tsugu-api-python Version: 1.1.4 Summary: Tsugu
+Metadata-Version: 2.1 Name: tsugu-api-python Version: 1.1.5 Summary: Tsugu
 BanGDream Bot çåè½ API ç»åå Home-page: https://github.com/
 WindowsSov8forUs/tsugu-api-python Author: WindowsSov8 Author-email:
 qwertyuiop2333@hotmail.com License: MIT Description:
  ![tsugu-api-ython logo](https://github.com/WindowsSov8forUs/tsugu-api-python/
          blob/main/logo.png) # tsugu-api-python _â¨ Python ç¼åç
       [TsuguBanGDreamBot](https://github.com/Yamamoto-2/tsugu-bangdream-
          bot?tab=readme-ov-file) ç¸å³åç§åè½ API è°ç¨åº â¨_
```

### Comparing `tsugu-api-python-1.1.4/README.md` & `tsugu-api-python-1.1.5/README.md`

 * *Files identical despite different names*

### Comparing `tsugu-api-python-1.1.4/setup.py` & `tsugu-api-python-1.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open('README.md', 'r', encoding='utf-8') as readme:
     long_description = readme.read()
 
 setup(
     name='tsugu-api-python',
-    version='1.1.4',
+    version='1.1.5',
     author='WindowsSov8',
     author_email='qwertyuiop2333@hotmail.com',
     description='Tsugu BanGDream Bot 的功能 API 统合包',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/WindowsSov8forUs/tsugu-api-python',
     include_package_data=False,
```

### Comparing `tsugu-api-python-1.1.4/tsugu_api/__init__.py` & `tsugu-api-python-1.1.5/tsugu_api/__init__.py`

 * *Files identical despite different names*

### Comparing `tsugu-api-python-1.1.4/tsugu_api/_bandoristation.py` & `tsugu-api-python-1.1.5/tsugu_api/_bandoristation.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from typing import List
+
 from tsugu_api import settings
 from tsugu_api._network import Api
 from tsugu_api._typing import _StationRoom
 from tsugu_api.exception import RoomQueryFailure, RoomSubmitFailure
 
 BANDORI_STATION_URL = 'https://api.bandoristation.com/index.php'
 
@@ -30,19 +32,19 @@
     response = Api(
         BANDORI_STATION_URL,
         proxy=settings.backend_proxy
     ).get(params).json()
     if response['status'] == 'failure':
         raise RoomSubmitFailure(response['response'])
 
-def query_room_number() -> list[_StationRoom]:
+def query_room_number() -> List[_StationRoom]:
     '''获取房间号
 
     返回:
-        list[_StationRoom]: 房间信息列表
+        List[_StationRoom]: 房间信息列表
     '''
     
     # 构建参数
     params = {
         'function': 'query_room_number'
     }
```

### Comparing `tsugu-api-python-1.1.4/tsugu_api/_network.py` & `tsugu-api-python-1.1.5/tsugu_api/_network.py`

 * *Files identical despite different names*

### Comparing `tsugu-api-python-1.1.4/tsugu_api/_station.py` & `tsugu-api-python-1.1.5/tsugu_api/_station.py`

 * *Files identical despite different names*

### Comparing `tsugu-api-python-1.1.4/tsugu_api/_tsugu.py` & `tsugu-api-python-1.1.5/tsugu_api/_tsugu.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Optional
+from typing import List, Optional
 
 from tsugu_api import settings
 from tsugu_api._network import Api
 from tsugu_api._typing import (
     _Room,
     _Server,
     _Response,
@@ -120,15 +120,15 @@
     
     # 发送请求
     return Api(
         url,
         proxy=settings.backend_proxy
     ).post(data).json()
 
-def room_list(room_list: list[_Room]) -> _Response:
+def room_list(room_list: List[_Room]) -> _Response:
     '''绘制车牌绘图
 
     参数:
         room_list (list[_CarData]): 车牌信息列表
 
     返回:
         _Response: 响应信息
@@ -145,15 +145,15 @@
     
     # 发送请求
     return Api(
         url,
         proxy=settings.backend_proxy
     ).post(data).json()
 
-def search_card(default_servers: list[_Server], text: str) -> _Response:
+def search_card(default_servers: List[_Server], text: str) -> _Response:
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
 
-def search_character(default_servers: list[_Server], text: str) -> _Response:
+def search_character(default_servers: List[_Server], text: str) -> _Response:
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
 
-def search_event(default_servers: list[_Server], text: str) -> _Response:
+def search_event(default_servers: List[_Server], text: str) -> _Response:
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
 
-def search_gacha(default_servers: list[_Server], gacha_id: int) -> _Response:
+def search_gacha(default_servers: List[_Server], gacha_id: int) -> _Response:
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
 
-def search_song(default_servers: list[_Server], text: str) -> _Response:
+def search_song(default_servers: List[_Server], text: str) -> _Response:
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
 
-def song_chart(default_servers: list[_Server], song_id: int, difficulty_text: _DifficultyText) -> _Response:
+def song_chart(default_servers: List[_Server], song_id: int, difficulty_text: _DifficultyText) -> _Response:
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
 
-def song_meta(default_servers: list[_Server], server: _Server) -> _Response:
+def song_meta(default_servers: List[_Server], server: _Server) -> _Response:
     '''查询歌曲分数表
 
     参数:
         default_servers (list[_Server]): 默认服务器
         server (_Server): 主服务器
 
     返回:
```

### Comparing `tsugu-api-python-1.1.4/tsugu_api/_typing.py` & `tsugu-api-python-1.1.5/tsugu_api/_typing.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 `tsugu_api._typing`
 
 定义了一些类型别名
 '''
 
 from typing import (
     Any,
+    List,
     Union,
     Literal,
     TypeAlias,
     TypedDict
 )
 from typing_extensions import NotRequired
 
@@ -39,15 +40,15 @@
 '''服务器'''
 
 class _Data(TypedDict):
     '''API 单个响应数据'''
     type: Literal['string', 'base64']
     string: str
 
-_Response: TypeAlias = list[_Data]
+_Response: TypeAlias = List[_Data]
 
 _DifficultyText: TypeAlias = Literal['easy', 'normal', 'hard', 'expert', 'special']
 '''难度名'''
 
 class _Player(TypedDict):
     id: int
     server: _Server
@@ -70,44 +71,44 @@
     player: _Player
     avanter: NotRequired[str]
     userName: NotRequired[str]
 
 class _QueryResponse(TypedDict):
     '''`/station/queryAllRoom` 响应结果'''
     status: _Status
-    data: Union[str, list[_Room]]
+    data: Union[str, List[_Room]]
 
 class _TsuguUserServer(TypedDict):
     '''服务器数据'''
     playerId: int
     bindingStatus: Literal[0, 1, 2]
     verifyCode: NotRequired[int]
 
 class _TsuguUser(TypedDict):
     '''用户数据'''
     user_id: str
     platform: str
     server_mode: _ServerId
-    default_server: list[_ServerId]
+    default_server: List[_ServerId]
     car: bool
-    server_list: list[_TsuguUserServer]
+    server_list: List[_TsuguUserServer]
 
 class _GetUserDataResponse(TypedDict):
     '''`/user/getUserData` 响应结果'''
     status: _Status
     data: Union[str, _TsuguUser]
 
 class _Update(TypedDict):
     '''更新数据'''
     user_id: NotRequired[str]
     platform: NotRequired[str]
     server_mode: NotRequired[_ServerId]
-    default_server: NotRequired[list[_ServerId]]
+    default_server: NotRequired[List[_ServerId]]
     car: NotRequired[bool]
-    server_list: NotRequired[list[_TsuguUserServer]]
+    server_list: NotRequired[List[_TsuguUserServer]]
 
 class _ChangeUserDataResponse(TypedDict):
     '''`/user/changeUserData` 响应结果'''
     status: _Status
     data: NotRequired[str]
 
 class _VerifyCode(TypedDict):
```

### Comparing `tsugu-api-python-1.1.4/tsugu_api/_user.py` & `tsugu-api-python-1.1.5/tsugu_api/_user.py`

 * *Files identical despite different names*

### Comparing `tsugu-api-python-1.1.4/tsugu_api/settings.py` & `tsugu-api-python-1.1.5/tsugu_api/settings.py`

 * *Files identical despite different names*

### Comparing `tsugu-api-python-1.1.4/tsugu_api/utils.py` & `tsugu-api-python-1.1.5/tsugu_api/utils.py`

 * *Files identical despite different names*

### Comparing `tsugu-api-python-1.1.4/tsugu_api_async/__init__.py` & `tsugu-api-python-1.1.5/tsugu_api_async/__init__.py`

 * *Files identical despite different names*

### Comparing `tsugu-api-python-1.1.4/tsugu_api_async/_bandoristation.py` & `tsugu-api-python-1.1.5/tsugu_api_async/_bandoristation.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from typing import List
+
 from httpx import Response
 
 from tsugu_api_async import settings
 from tsugu_api_async._network import Api
 from tsugu_api_async._typing import _StationRoom
 from tsugu_api_async.exception import RoomQueryFailure, RoomSubmitFailure
 
@@ -34,19 +36,19 @@
             proxy=settings.backend_proxy
     ).get(params)
     if isinstance(response, Response): response = response.json()
     else: response = await response.json()
     if response['status'] == 'failure':
         raise RoomSubmitFailure(response['response'])
 
-async def query_room_number() -> list[_StationRoom]:
+async def query_room_number() -> List[_StationRoom]:
     '''获取房间号
 
     返回:
-        list[_StationRoom]: 房间信息列表
+        List[_StationRoom]: 房间信息列表
     '''
     
     # 构建参数
     params = {
         'function': 'query_room_number'
     }
```

### Comparing `tsugu-api-python-1.1.4/tsugu_api_async/_network.py` & `tsugu-api-python-1.1.5/tsugu_api_async/_network.py`

 * *Files identical despite different names*

### Comparing `tsugu-api-python-1.1.4/tsugu_api_async/_station.py` & `tsugu-api-python-1.1.5/tsugu_api_async/_station.py`

 * *Files identical despite different names*

### Comparing `tsugu-api-python-1.1.4/tsugu_api_async/_tsugu.py` & `tsugu-api-python-1.1.5/tsugu_api_async/_tsugu.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Optional
+from typing import List, Optional
 
 from httpx import Response
 
 from tsugu_api_async import settings
 from tsugu_api_async._network import Api
 from tsugu_api_async._typing import (
     _Room,
@@ -130,15 +130,15 @@
     response = await Api(
         url,
         proxy=settings.backend_proxy
     ).post(data)
     if isinstance(response, Response): return response.json()
     return await response.json()
 
-async def room_list(room_list: list[_Room]) -> _Response:
+async def room_list(room_list: List[_Room]) -> _Response:
     '''绘制车牌绘图
 
     参数:
         room_list (list[_CarData]): 车牌信息列表
 
     返回:
         _Response: 响应信息
@@ -157,15 +157,15 @@
     response = await Api(
         url,
         proxy=settings.backend_proxy
     ).post(data)
     if isinstance(response, Response): return response.json()
     return await response.json()
 
-async def search_card(default_servers: list[_Server], text: str) -> _Response:
+async def search_card(default_servers: List[_Server], text: str) -> _Response:
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
 
-async def search_character(default_servers: list[_Server], text: str) -> _Response:
+async def search_character(default_servers: List[_Server], text: str) -> _Response:
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
 
-async def search_event(default_servers: list[_Server], text: str) -> _Response:
+async def search_event(default_servers: List[_Server], text: str) -> _Response:
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
 
-async def search_gacha(default_servers: list[_Server], gacha_id: int) -> _Response:
+async def search_gacha(default_servers: List[_Server], gacha_id: int) -> _Response:
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
 
-async def search_song(default_servers: list[_Server], text: str) -> _Response:
+async def search_song(default_servers: List[_Server], text: str) -> _Response:
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
 
-async def song_chart(default_servers: list[_Server], song_id: int, difficulty_text: _DifficultyText) -> _Response:
+async def song_chart(default_servers: List[_Server], song_id: int, difficulty_text: _DifficultyText) -> _Response:
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
 
-async def song_meta(default_servers: list[_Server], server: _Server) -> _Response:
+async def song_meta(default_servers: List[_Server], server: _Server) -> _Response:
     '''查询歌曲分数表
 
     参数:
         default_servers (list[_Server]): 默认服务器
         server (_Server): 主服务器
 
     返回:
```

### Comparing `tsugu-api-python-1.1.4/tsugu_api_async/_typing.py` & `tsugu-api-python-1.1.5/tsugu_api_async/_typing.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 `tsugu_api._typing`
 
 定义了一些类型别名
 '''
 
 from typing import (
     Any,
+    List,
     Union,
     Literal,
     TypeAlias,
     TypedDict
 )
 from typing_extensions import NotRequired
 
@@ -44,15 +45,15 @@
 '''服务器'''
 
 class _Data(TypedDict):
     '''API 单个响应数据'''
     type: Literal['string', 'base64']
     string: str
 
-_Response: TypeAlias = list[_Data]
+_Response: TypeAlias = List[_Data]
 
 _DifficultyText: TypeAlias = Literal['easy', 'normal', 'hard', 'expert', 'special']
 '''难度名'''
 
 class _Player(TypedDict):
     id: int
     server: _Server
@@ -75,44 +76,44 @@
     player: _Player
     avanter: NotRequired[str]
     userName: NotRequired[str]
 
 class _QueryResponse(TypedDict):
     '''`/station/queryAllRoom` 响应结果'''
     status: _Status
-    data: Union[str, list[_Room]]
+    data: Union[str, List[_Room]]
 
 class _TsuguUserServer(TypedDict):
     '''服务器数据'''
     playerId: int
     bindingStatus: Literal[0, 1, 2]
     verifyCode: NotRequired[int]
 
 class _TsuguUser(TypedDict):
     '''用户数据'''
     user_id: str
     platform: str
     server_mode: _ServerId
-    default_server: list[_ServerId]
+    default_server: List[_ServerId]
     car: bool
-    server_list: list[_TsuguUserServer]
+    server_list: List[_TsuguUserServer]
 
 class _GetUserDataResponse(TypedDict):
     '''`/user/getUserData` 响应结果'''
     status: _Status
     data: Union[str, _TsuguUser]
 
 class _Update(TypedDict):
     '''更新数据'''
     user_id: NotRequired[str]
     platform: NotRequired[str]
     server_mode: NotRequired[_ServerId]
-    default_server: NotRequired[list[_ServerId]]
+    default_server: NotRequired[List[_ServerId]]
     car: NotRequired[bool]
-    server_list: NotRequired[list[_TsuguUserServer]]
+    server_list: NotRequired[List[_TsuguUserServer]]
 
 class _ChangeUserDataResponse(TypedDict):
     '''`/user/changeUserData` 响应结果'''
     status: _Status
     data: NotRequired[str]
 
 class _VerifyCode(TypedDict):
```

### Comparing `tsugu-api-python-1.1.4/tsugu_api_async/_user.py` & `tsugu-api-python-1.1.5/tsugu_api_async/_user.py`

 * *Files identical despite different names*

### Comparing `tsugu-api-python-1.1.4/tsugu_api_async/settings.py` & `tsugu-api-python-1.1.5/tsugu_api_async/settings.py`

 * *Files identical despite different names*

### Comparing `tsugu-api-python-1.1.4/tsugu_api_async/utils.py` & `tsugu-api-python-1.1.5/tsugu_api_async/utils.py`

 * *Files identical despite different names*

### Comparing `tsugu-api-python-1.1.4/tsugu_api_python.egg-info/PKG-INFO` & `tsugu-api-python-1.1.5/tsugu_api_python.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tsugu-api-python
-Version: 1.1.4
+Version: 1.1.5
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
-Metadata-Version: 2.1 Name: tsugu-api-python Version: 1.1.4 Summary: Tsugu
+Metadata-Version: 2.1 Name: tsugu-api-python Version: 1.1.5 Summary: Tsugu
 BanGDream Bot çåè½ API ç»åå Home-page: https://github.com/
 WindowsSov8forUs/tsugu-api-python Author: WindowsSov8 Author-email:
 qwertyuiop2333@hotmail.com License: MIT Description:
  ![tsugu-api-ython logo](https://github.com/WindowsSov8forUs/tsugu-api-python/
          blob/main/logo.png) # tsugu-api-python _â¨ Python ç¼åç
       [TsuguBanGDreamBot](https://github.com/Yamamoto-2/tsugu-bangdream-
          bot?tab=readme-ov-file) ç¸å³åç§åè½ API è°ç¨åº â¨_
```

### Comparing `tsugu-api-python-1.1.4/tsugu_api_python.egg-info/SOURCES.txt` & `tsugu-api-python-1.1.5/tsugu_api_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

