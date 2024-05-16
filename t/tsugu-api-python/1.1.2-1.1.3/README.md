# Comparing `tmp/tsugu-api-python-1.1.2.tar.gz` & `tmp/tsugu-api-python-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tsugu-api-python-1.1.2.tar", last modified: Wed May 15 04:46:31 2024, max compression
+gzip compressed data, was "tsugu-api-python-1.1.3.tar", last modified: Wed May 15 16:09:12 2024, max compression
```

## Comparing `tsugu-api-python-1.1.2.tar` & `tsugu-api-python-1.1.3.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 04:46:31.990208 tsugu-api-python-1.1.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-15 04:46:22.000000 tsugu-api-python-1.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5878 2024-05-15 04:46:31.990208 tsugu-api-python-1.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4336 2024-05-15 04:46:22.000000 tsugu-api-python-1.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 04:46:31.990208 tsugu-api-python-1.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      846 2024-05-15 04:46:22.000000 tsugu-api-python-1.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 04:46:31.986208 tsugu-api-python-1.1.2/tsugu_api/
--rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-05-15 04:46:22.000000 tsugu-api-python-1.1.2/tsugu_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1557 2024-05-15 04:46:22.000000 tsugu-api-python-1.1.2/tsugu_api/_bandoristation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2835 2024-05-15 04:46:22.000000 tsugu-api-python-1.1.2/tsugu_api/_network.py
--rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-05-15 04:46:22.000000 tsugu-api-python-1.1.2/tsugu_api/_station.py
--rw-r--r--   0 runner    (1001) docker     (127)     9389 2024-05-15 04:46:22.000000 tsugu-api-python-1.1.2/tsugu_api/_tsugu.py
--rw-r--r--   0 runner    (1001) docker     (127)     3085 2024-05-15 04:46:22.000000 tsugu-api-python-1.1.2/tsugu_api/_typing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3344 2024-05-15 04:46:22.000000 tsugu-api-python-1.1.2/tsugu_api/_user.py
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-15 04:46:22.000000 tsugu-api-python-1.1.2/tsugu_api/exception.py
--rw-r--r--   0 runner    (1001) docker     (127)     1908 2024-05-15 04:46:22.000000 tsugu-api-python-1.1.2/tsugu_api/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-05-15 04:46:22.000000 tsugu-api-python-1.1.2/tsugu_api/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 04:46:31.986208 tsugu-api-python-1.1.2/tsugu_api_async/
--rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-05-15 04:46:22.000000 tsugu-api-python-1.1.2/tsugu_api_async/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1845 2024-05-15 04:46:22.000000 tsugu-api-python-1.1.2/tsugu_api_async/_bandoristation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3769 2024-05-15 04:46:22.000000 tsugu-api-python-1.1.2/tsugu_api_async/_network.py
--rw-r--r--   0 runner    (1001) docker     (127)     1882 2024-05-15 04:46:22.000000 tsugu-api-python-1.1.2/tsugu_api_async/_station.py
--rw-r--r--   0 runner    (1001) docker     (127)    10995 2024-05-15 04:46:22.000000 tsugu-api-python-1.1.2/tsugu_api_async/_tsugu.py
--rw-r--r--   0 runner    (1001) docker     (127)     3207 2024-05-15 04:46:22.000000 tsugu-api-python-1.1.2/tsugu_api_async/_typing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3805 2024-05-15 04:46:22.000000 tsugu-api-python-1.1.2/tsugu_api_async/_user.py
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-15 04:46:22.000000 tsugu-api-python-1.1.2/tsugu_api_async/exception.py
--rw-r--r--   0 runner    (1001) docker     (127)     2116 2024-05-15 04:46:22.000000 tsugu-api-python-1.1.2/tsugu_api_async/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     1263 2024-05-15 04:46:22.000000 tsugu-api-python-1.1.2/tsugu_api_async/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 04:46:31.990208 tsugu-api-python-1.1.2/tsugu_api_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5878 2024-05-15 04:46:31.000000 tsugu-api-python-1.1.2/tsugu_api_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      723 2024-05-15 04:46:31.000000 tsugu-api-python-1.1.2/tsugu_api_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 04:46:31.000000 tsugu-api-python-1.1.2/tsugu_api_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-15 04:46:31.000000 tsugu-api-python-1.1.2/tsugu_api_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-15 04:46:31.000000 tsugu-api-python-1.1.2/tsugu_api_python.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:09:12.107467 tsugu-api-python-1.1.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-15 16:09:02.000000 tsugu-api-python-1.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6199 2024-05-15 16:09:12.107467 tsugu-api-python-1.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4593 2024-05-15 16:09:02.000000 tsugu-api-python-1.1.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 16:09:12.107467 tsugu-api-python-1.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      846 2024-05-15 16:09:02.000000 tsugu-api-python-1.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:09:12.103467 tsugu-api-python-1.1.3/tsugu_api/
+-rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-05-15 16:09:02.000000 tsugu-api-python-1.1.3/tsugu_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1557 2024-05-15 16:09:02.000000 tsugu-api-python-1.1.3/tsugu_api/_bandoristation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2835 2024-05-15 16:09:02.000000 tsugu-api-python-1.1.3/tsugu_api/_network.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-05-15 16:09:02.000000 tsugu-api-python-1.1.3/tsugu_api/_station.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9389 2024-05-15 16:09:02.000000 tsugu-api-python-1.1.3/tsugu_api/_tsugu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3110 2024-05-15 16:09:02.000000 tsugu-api-python-1.1.3/tsugu_api/_typing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3344 2024-05-15 16:09:02.000000 tsugu-api-python-1.1.3/tsugu_api/_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-15 16:09:02.000000 tsugu-api-python-1.1.3/tsugu_api/exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1908 2024-05-15 16:09:02.000000 tsugu-api-python-1.1.3/tsugu_api/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-05-15 16:09:02.000000 tsugu-api-python-1.1.3/tsugu_api/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:09:12.103467 tsugu-api-python-1.1.3/tsugu_api_async/
+-rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-05-15 16:09:02.000000 tsugu-api-python-1.1.3/tsugu_api_async/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1845 2024-05-15 16:09:02.000000 tsugu-api-python-1.1.3/tsugu_api_async/_bandoristation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3769 2024-05-15 16:09:02.000000 tsugu-api-python-1.1.3/tsugu_api_async/_network.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1882 2024-05-15 16:09:02.000000 tsugu-api-python-1.1.3/tsugu_api_async/_station.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10995 2024-05-15 16:09:02.000000 tsugu-api-python-1.1.3/tsugu_api_async/_tsugu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3232 2024-05-15 16:09:02.000000 tsugu-api-python-1.1.3/tsugu_api_async/_typing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3805 2024-05-15 16:09:02.000000 tsugu-api-python-1.1.3/tsugu_api_async/_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-15 16:09:02.000000 tsugu-api-python-1.1.3/tsugu_api_async/exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2115 2024-05-15 16:09:02.000000 tsugu-api-python-1.1.3/tsugu_api_async/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1263 2024-05-15 16:09:02.000000 tsugu-api-python-1.1.3/tsugu_api_async/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:09:12.107467 tsugu-api-python-1.1.3/tsugu_api_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6199 2024-05-15 16:09:11.000000 tsugu-api-python-1.1.3/tsugu_api_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      723 2024-05-15 16:09:12.000000 tsugu-api-python-1.1.3/tsugu_api_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 16:09:11.000000 tsugu-api-python-1.1.3/tsugu_api_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-15 16:09:11.000000 tsugu-api-python-1.1.3/tsugu_api_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-15 16:09:11.000000 tsugu-api-python-1.1.3/tsugu_api_python.egg-info/top_level.txt
```

### Comparing `tsugu-api-python-1.1.2/LICENSE` & `tsugu-api-python-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `tsugu-api-python-1.1.2/PKG-INFO` & `tsugu-api-python-1.1.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tsugu-api-python
-Version: 1.1.2
+Version: 1.1.3
 Summary: Tsugu BanGDream Bot 的功能 API 统合包
 Home-page: https://github.com/WindowsSov8forUs/tsugu-api-python
 Author: WindowsSov8
 Author-email: qwertyuiop2333@hotmail.com
 License: MIT
 Description: <div align="center">
         
@@ -67,16 +67,23 @@
         |查询指定卡池信息|`search_gacha`|
         |获取玩家状态信息|`search_player`|
         |查询符合条件的歌曲信息|`search_song`|
         |查询指定歌曲指定难度的谱面|`song_chart`|
         |查询歌曲分数表|`song_meta`|
         |查询指定活动的指定档位预测线|`ycx`|
         |查询指定活动的全部档位预测线|`ycx_all`|
-        |提交车牌信息到后端|`station_submit_room_number`|
-        |从后端获取最近的车牌信息列表|`station_query_all_room`|
+        
+        #### 车站数据后端功能
+        
+        |功能描述|方法名称|
+        |:------|:----------|
+        |提交房间信息到后端|`station_submit_room_number`|
+        |从后端获取最近的房间信息列表|`station_query_all_room`|
+        
+        > 若后端不支持用户数据库，以上功能可能无法使用，请以 **车站功能** API 代替。
         
         #### 用户数据后端功能
         
         |功能描述|方法名称|
         |:------|:----------|
         |获取用户数据|`get_user_data`|
         |修改用户数据|`change_user_data`|
@@ -85,15 +92,16 @@
         
         > 以上功能都可使用本地用户数据库代替，本 API 不提供相关的配置方法。
         
         #### 车站功能
         
         |功能描述|方法名称|
         |:------|:----------|
-        |提交车牌信息到车站|`submit_room_number`|
+        |从车站获取最近的房间信息列表|`query_room_number`|
+        |提交房间信息到车站|`submit_room_number`|
         
         
         ## 快速使用
         
         以下将以获取歌曲 **EXIST** (id=325) 的信息为例。
         
         使用以下指令安装本模块：
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: tsugu-api-python Version: 1.1.2 Summary: Tsugu
+Metadata-Version: 2.1 Name: tsugu-api-python Version: 1.1.3 Summary: Tsugu
 BanGDream Bot çåè½ API ç»åå Home-page: https://github.com/
 WindowsSov8forUs/tsugu-api-python Author: WindowsSov8 Author-email:
 qwertyuiop2333@hotmail.com License: MIT Description:
  ![tsugu-api-ython logo](https://github.com/WindowsSov8forUs/tsugu-api-python/
          blob/main/logo.png) # tsugu-api-python _â¨ Python ç¼åç
       [TsuguBanGDreamBot](https://github.com/Yamamoto-2/tsugu-bangdream-
          bot?tab=readme-ov-file) ç¸å³åç§åè½ API è°ç¨åº â¨_
@@ -29,25 +29,30 @@
 |æ¥è¯¢ç¬¦åæ¡ä»¶çæ´»å¨ä¿¡æ¯|`search_event`|
 |æ¥è¯¢æå®å¡æ± ä¿¡æ¯|`search_gacha`|
 |è·åç©å®¶ç¶æä¿¡æ¯|`search_player`|
 |æ¥è¯¢ç¬¦åæ¡ä»¶çæ­æ²ä¿¡æ¯|`search_song`|
 |æ¥è¯¢æå®æ­æ²æå®é¾åº¦çè°±é¢|`song_chart`|
 |æ¥è¯¢æ­æ²åæ°è¡¨|`song_meta`|
 |æ¥è¯¢æå®æ´»å¨çæå®æ¡£ä½é¢æµçº¿|`ycx`|
-|æ¥è¯¢æå®æ´»å¨çå¨é¨æ¡£ä½é¢æµçº¿|`ycx_all`|
-|æäº¤è½¦çä¿¡æ¯å°åç«¯|`station_submit_room_number`|
-|ä»åç«¯è·åæè¿çè½¦çä¿¡æ¯åè¡¨|`station_query_all_room`| ####
-ç¨æ·æ°æ®åç«¯åè½ |åè½æè¿°|æ¹æ³åç§°| |:------|:----------
+|æ¥è¯¢æå®æ´»å¨çå¨é¨æ¡£ä½é¢æµçº¿|`ycx_all`| ####
+è½¦ç«æ°æ®åç«¯åè½ |åè½æè¿°|æ¹æ³åç§°| |:------|:----------
+| |æäº¤æ¿é´ä¿¡æ¯å°åç«¯|`station_submit_room_number`|
+|ä»åç«¯è·åæè¿çæ¿é´ä¿¡æ¯åè¡¨|`station_query_all_room`| >
+è¥åç«¯ä¸æ¯æç¨æ·æ°æ®åºï¼ä»¥ä¸åè½å¯è½æ æ³ä½¿ç¨ï¼è¯·ä»¥
+**è½¦ç«åè½** API ä»£æ¿ã #### ç¨æ·æ°æ®åç«¯åè½
+|åè½æè¿°|æ¹æ³åç§°| |:------|:----------
 | |è·åç¨æ·æ°æ®|`get_user_data`| |ä¿®æ¹ç¨æ·æ°æ®|`change_user_data`|
 |åéç»å®ç¨æ·è¯·æ±|`bind_player_request`|
 |éªè¯ç»å®ç¨æ·è¯·æ±|`bind_player_verification`| >
 ä»¥ä¸åè½é½å¯ä½¿ç¨æ¬å°ç¨æ·æ°æ®åºä»£æ¿ï¼æ¬ API
 ä¸æä¾ç¸å³çéç½®æ¹æ³ã #### è½¦ç«åè½ |åè½æè¿°|æ¹æ³åç§°|
-|:------|:----------| |æäº¤è½¦çä¿¡æ¯å°è½¦ç«|`submit_room_number`| ##
-å¿«éä½¿ç¨ ä»¥ä¸å°ä»¥è·åæ­æ² **EXIST** (id=325) çä¿¡æ¯ä¸ºä¾ã
+|:------|:----------
+| |ä»è½¦ç«è·åæè¿çæ¿é´ä¿¡æ¯åè¡¨|`query_room_number`|
+|æäº¤æ¿é´ä¿¡æ¯å°è½¦ç«|`submit_room_number`| ## å¿«éä½¿ç¨
+ä»¥ä¸å°ä»¥è·åæ­æ² **EXIST** (id=325) çä¿¡æ¯ä¸ºä¾ã
 ä½¿ç¨ä»¥ä¸æä»¤å®è£æ¬æ¨¡åï¼ ```bash $ pip3 install tsugu-api-python
 ``` ä½¿ç¨å¦ä¸ä»£ç ï¼è·åæå®æ­æ²ä¿¡æ¯å¾çï¼ ```python from
 tsugu_api import search_song def main() -> None: result = search_song([3, 0],
 "EXIST") # è¿éä¹å¯ä»¥ä¼ å¥ "325" ï¼å·ä½åå³äºç¨æ·è¾å¥ä¿¡æ¯
 main() ``` > `[3, 0]` æä»£ç¨æ·çé»è®¤æå¡å¨åè¡¨ï¼å¯ä»éè¿
 `get_user_data()` æ¹æ³è·åçè¿åå¼ä¸­è·åã è·åå°ç `result`
 å°æ¯ä¸ä¸ª `_Response` å¯¹è±¡ï¼å½è·åå°åç¡®çä¿¡æ¯æ¶ï¼ `result`
```

### Comparing `tsugu-api-python-1.1.2/README.md` & `tsugu-api-python-1.1.3/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -59,16 +59,23 @@
 |查询指定卡池信息|`search_gacha`|
 |获取玩家状态信息|`search_player`|
 |查询符合条件的歌曲信息|`search_song`|
 |查询指定歌曲指定难度的谱面|`song_chart`|
 |查询歌曲分数表|`song_meta`|
 |查询指定活动的指定档位预测线|`ycx`|
 |查询指定活动的全部档位预测线|`ycx_all`|
-|提交车牌信息到后端|`station_submit_room_number`|
-|从后端获取最近的车牌信息列表|`station_query_all_room`|
+
+#### 车站数据后端功能
+
+|功能描述|方法名称|
+|:------|:----------|
+|提交房间信息到后端|`station_submit_room_number`|
+|从后端获取最近的房间信息列表|`station_query_all_room`|
+
+> 若后端不支持用户数据库，以上功能可能无法使用，请以 **车站功能** API 代替。
 
 #### 用户数据后端功能
 
 |功能描述|方法名称|
 |:------|:----------|
 |获取用户数据|`get_user_data`|
 |修改用户数据|`change_user_data`|
@@ -77,15 +84,16 @@
 
 > 以上功能都可使用本地用户数据库代替，本 API 不提供相关的配置方法。
 
 #### 车站功能
 
 |功能描述|方法名称|
 |:------|:----------|
-|提交车牌信息到车站|`submit_room_number`|
+|从车站获取最近的房间信息列表|`query_room_number`|
+|提交房间信息到车站|`submit_room_number`|
 
 
 ## 快速使用
 
 以下将以获取歌曲 **EXIST** (id=325) 的信息为例。
 
 使用以下指令安装本模块：
```

#### html2text {}

```diff
@@ -25,25 +25,30 @@
 |æ¥è¯¢ç¬¦åæ¡ä»¶çæ´»å¨ä¿¡æ¯|`search_event`|
 |æ¥è¯¢æå®å¡æ± ä¿¡æ¯|`search_gacha`|
 |è·åç©å®¶ç¶æä¿¡æ¯|`search_player`|
 |æ¥è¯¢ç¬¦åæ¡ä»¶çæ­æ²ä¿¡æ¯|`search_song`|
 |æ¥è¯¢æå®æ­æ²æå®é¾åº¦çè°±é¢|`song_chart`|
 |æ¥è¯¢æ­æ²åæ°è¡¨|`song_meta`|
 |æ¥è¯¢æå®æ´»å¨çæå®æ¡£ä½é¢æµçº¿|`ycx`|
-|æ¥è¯¢æå®æ´»å¨çå¨é¨æ¡£ä½é¢æµçº¿|`ycx_all`|
-|æäº¤è½¦çä¿¡æ¯å°åç«¯|`station_submit_room_number`|
-|ä»åç«¯è·åæè¿çè½¦çä¿¡æ¯åè¡¨|`station_query_all_room`| ####
-ç¨æ·æ°æ®åç«¯åè½ |åè½æè¿°|æ¹æ³åç§°| |:------|:----------
+|æ¥è¯¢æå®æ´»å¨çå¨é¨æ¡£ä½é¢æµçº¿|`ycx_all`| ####
+è½¦ç«æ°æ®åç«¯åè½ |åè½æè¿°|æ¹æ³åç§°| |:------|:----------
+| |æäº¤æ¿é´ä¿¡æ¯å°åç«¯|`station_submit_room_number`|
+|ä»åç«¯è·åæè¿çæ¿é´ä¿¡æ¯åè¡¨|`station_query_all_room`| >
+è¥åç«¯ä¸æ¯æç¨æ·æ°æ®åºï¼ä»¥ä¸åè½å¯è½æ æ³ä½¿ç¨ï¼è¯·ä»¥
+**è½¦ç«åè½** API ä»£æ¿ã #### ç¨æ·æ°æ®åç«¯åè½
+|åè½æè¿°|æ¹æ³åç§°| |:------|:----------
 | |è·åç¨æ·æ°æ®|`get_user_data`| |ä¿®æ¹ç¨æ·æ°æ®|`change_user_data`|
 |åéç»å®ç¨æ·è¯·æ±|`bind_player_request`|
 |éªè¯ç»å®ç¨æ·è¯·æ±|`bind_player_verification`| >
 ä»¥ä¸åè½é½å¯ä½¿ç¨æ¬å°ç¨æ·æ°æ®åºä»£æ¿ï¼æ¬ API
 ä¸æä¾ç¸å³çéç½®æ¹æ³ã #### è½¦ç«åè½ |åè½æè¿°|æ¹æ³åç§°|
-|:------|:----------| |æäº¤è½¦çä¿¡æ¯å°è½¦ç«|`submit_room_number`| ##
-å¿«éä½¿ç¨ ä»¥ä¸å°ä»¥è·åæ­æ² **EXIST** (id=325) çä¿¡æ¯ä¸ºä¾ã
+|:------|:----------
+| |ä»è½¦ç«è·åæè¿çæ¿é´ä¿¡æ¯åè¡¨|`query_room_number`|
+|æäº¤æ¿é´ä¿¡æ¯å°è½¦ç«|`submit_room_number`| ## å¿«éä½¿ç¨
+ä»¥ä¸å°ä»¥è·åæ­æ² **EXIST** (id=325) çä¿¡æ¯ä¸ºä¾ã
 ä½¿ç¨ä»¥ä¸æä»¤å®è£æ¬æ¨¡åï¼ ```bash $ pip3 install tsugu-api-python
 ``` ä½¿ç¨å¦ä¸ä»£ç ï¼è·åæå®æ­æ²ä¿¡æ¯å¾çï¼ ```python from
 tsugu_api import search_song def main() -> None: result = search_song([3, 0],
 "EXIST") # è¿éä¹å¯ä»¥ä¼ å¥ "325" ï¼å·ä½åå³äºç¨æ·è¾å¥ä¿¡æ¯
 main() ``` > `[3, 0]` æä»£ç¨æ·çé»è®¤æå¡å¨åè¡¨ï¼å¯ä»éè¿
 `get_user_data()` æ¹æ³è·åçè¿åå¼ä¸­è·åã è·åå°ç `result`
 å°æ¯ä¸ä¸ª `_Response` å¯¹è±¡ï¼å½è·åå°åç¡®çä¿¡æ¯æ¶ï¼ `result`
```

### Comparing `tsugu-api-python-1.1.2/setup.py` & `tsugu-api-python-1.1.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open('README.md', 'r', encoding='utf-8') as readme:
     long_description = readme.read()
 
 setup(
     name='tsugu-api-python',
-    version='1.1.2',
+    version='1.1.3',
     author='WindowsSov8',
     author_email='qwertyuiop2333@hotmail.com',
     description='Tsugu BanGDream Bot 的功能 API 统合包',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/WindowsSov8forUs/tsugu-api-python',
     include_package_data=False,
```

### Comparing `tsugu-api-python-1.1.2/tsugu_api/__init__.py` & `tsugu-api-python-1.1.3/tsugu_api/__init__.py`

 * *Files identical despite different names*

### Comparing `tsugu-api-python-1.1.2/tsugu_api/_bandoristation.py` & `tsugu-api-python-1.1.3/tsugu_api/_bandoristation.py`

 * *Files identical despite different names*

### Comparing `tsugu-api-python-1.1.2/tsugu_api/_network.py` & `tsugu-api-python-1.1.3/tsugu_api/_network.py`

 * *Files identical despite different names*

### Comparing `tsugu-api-python-1.1.2/tsugu_api/_station.py` & `tsugu-api-python-1.1.3/tsugu_api/_station.py`

 * *Files identical despite different names*

### Comparing `tsugu-api-python-1.1.2/tsugu_api/_tsugu.py` & `tsugu-api-python-1.1.3/tsugu_api/_tsugu.py`

 * *Files identical despite different names*

### Comparing `tsugu-api-python-1.1.2/tsugu_api/_typing.py` & `tsugu-api-python-1.1.3/tsugu_api/_typing.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 '''
 
 from typing import (
     Any,
     Union,
     Literal,
     TypeAlias,
-    TypedDict,
-    NotRequired
+    TypedDict
 )
+from typing_extensions import NotRequired
 
 _ServerId: TypeAlias = Literal[0, 1, 2, 3, 4]
 '''
 服务器 ID
 
 值:
     0: 日服
```

### Comparing `tsugu-api-python-1.1.2/tsugu_api/_user.py` & `tsugu-api-python-1.1.3/tsugu_api/_user.py`

 * *Files identical despite different names*

### Comparing `tsugu-api-python-1.1.2/tsugu_api/settings.py` & `tsugu-api-python-1.1.3/tsugu_api/settings.py`

 * *Files identical despite different names*

### Comparing `tsugu-api-python-1.1.2/tsugu_api/utils.py` & `tsugu-api-python-1.1.3/tsugu_api/utils.py`

 * *Files identical despite different names*

### Comparing `tsugu-api-python-1.1.2/tsugu_api_async/__init__.py` & `tsugu-api-python-1.1.3/tsugu_api_async/__init__.py`

 * *Files identical despite different names*

### Comparing `tsugu-api-python-1.1.2/tsugu_api_async/_bandoristation.py` & `tsugu-api-python-1.1.3/tsugu_api_async/_bandoristation.py`

 * *Files identical despite different names*

### Comparing `tsugu-api-python-1.1.2/tsugu_api_async/_network.py` & `tsugu-api-python-1.1.3/tsugu_api_async/_network.py`

 * *Files identical despite different names*

### Comparing `tsugu-api-python-1.1.2/tsugu_api_async/_station.py` & `tsugu-api-python-1.1.3/tsugu_api_async/_station.py`

 * *Files identical despite different names*

### Comparing `tsugu-api-python-1.1.2/tsugu_api_async/_tsugu.py` & `tsugu-api-python-1.1.3/tsugu_api_async/_tsugu.py`

 * *Files identical despite different names*

### Comparing `tsugu-api-python-1.1.2/tsugu_api_async/_typing.py` & `tsugu-api-python-1.1.3/tsugu_api_async/_typing.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 '''
 
 from typing import (
     Any,
     Union,
     Literal,
     TypeAlias,
-    TypedDict,
-    NotRequired
+    TypedDict
 )
+from typing_extensions import NotRequired
 
 from httpx import Response
 from aiohttp import ClientResponse
 
 _ApiResponse: TypeAlias = Union[Response, ClientResponse]
 
 _ServerId: TypeAlias = Literal[0, 1, 2, 3, 4]
```

### Comparing `tsugu-api-python-1.1.2/tsugu_api_async/_user.py` & `tsugu-api-python-1.1.3/tsugu_api_async/_user.py`

 * *Files identical despite different names*

### Comparing `tsugu-api-python-1.1.2/tsugu_api_async/settings.py` & `tsugu-api-python-1.1.3/tsugu_api_async/settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 '''对 tsugu_api 进行配置'''
 
-from enum import StrEnum
+from enum import Enum
 from typing import Optional
 
-class Client(StrEnum):
+class Client(str, Enum):
     HTTPX = 'httpx'
     '''使用 `httpx`'''
     AIO_HTTP = 'aiohttp'
     '''使用 `aiohttp`'''
 
 client: Client = Client.HTTPX
 '''使用的 HTTP 客户端'''
```

### Comparing `tsugu-api-python-1.1.2/tsugu_api_async/utils.py` & `tsugu-api-python-1.1.3/tsugu_api_async/utils.py`

 * *Files identical despite different names*

### Comparing `tsugu-api-python-1.1.2/tsugu_api_python.egg-info/PKG-INFO` & `tsugu-api-python-1.1.3/tsugu_api_python.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tsugu-api-python
-Version: 1.1.2
+Version: 1.1.3
 Summary: Tsugu BanGDream Bot 的功能 API 统合包
 Home-page: https://github.com/WindowsSov8forUs/tsugu-api-python
 Author: WindowsSov8
 Author-email: qwertyuiop2333@hotmail.com
 License: MIT
 Description: <div align="center">
         
@@ -67,16 +67,23 @@
         |查询指定卡池信息|`search_gacha`|
         |获取玩家状态信息|`search_player`|
         |查询符合条件的歌曲信息|`search_song`|
         |查询指定歌曲指定难度的谱面|`song_chart`|
         |查询歌曲分数表|`song_meta`|
         |查询指定活动的指定档位预测线|`ycx`|
         |查询指定活动的全部档位预测线|`ycx_all`|
-        |提交车牌信息到后端|`station_submit_room_number`|
-        |从后端获取最近的车牌信息列表|`station_query_all_room`|
+        
+        #### 车站数据后端功能
+        
+        |功能描述|方法名称|
+        |:------|:----------|
+        |提交房间信息到后端|`station_submit_room_number`|
+        |从后端获取最近的房间信息列表|`station_query_all_room`|
+        
+        > 若后端不支持用户数据库，以上功能可能无法使用，请以 **车站功能** API 代替。
         
         #### 用户数据后端功能
         
         |功能描述|方法名称|
         |:------|:----------|
         |获取用户数据|`get_user_data`|
         |修改用户数据|`change_user_data`|
@@ -85,15 +92,16 @@
         
         > 以上功能都可使用本地用户数据库代替，本 API 不提供相关的配置方法。
         
         #### 车站功能
         
         |功能描述|方法名称|
         |:------|:----------|
-        |提交车牌信息到车站|`submit_room_number`|
+        |从车站获取最近的房间信息列表|`query_room_number`|
+        |提交房间信息到车站|`submit_room_number`|
         
         
         ## 快速使用
         
         以下将以获取歌曲 **EXIST** (id=325) 的信息为例。
         
         使用以下指令安装本模块：
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: tsugu-api-python Version: 1.1.2 Summary: Tsugu
+Metadata-Version: 2.1 Name: tsugu-api-python Version: 1.1.3 Summary: Tsugu
 BanGDream Bot çåè½ API ç»åå Home-page: https://github.com/
 WindowsSov8forUs/tsugu-api-python Author: WindowsSov8 Author-email:
 qwertyuiop2333@hotmail.com License: MIT Description:
  ![tsugu-api-ython logo](https://github.com/WindowsSov8forUs/tsugu-api-python/
          blob/main/logo.png) # tsugu-api-python _â¨ Python ç¼åç
       [TsuguBanGDreamBot](https://github.com/Yamamoto-2/tsugu-bangdream-
          bot?tab=readme-ov-file) ç¸å³åç§åè½ API è°ç¨åº â¨_
@@ -29,25 +29,30 @@
 |æ¥è¯¢ç¬¦åæ¡ä»¶çæ´»å¨ä¿¡æ¯|`search_event`|
 |æ¥è¯¢æå®å¡æ± ä¿¡æ¯|`search_gacha`|
 |è·åç©å®¶ç¶æä¿¡æ¯|`search_player`|
 |æ¥è¯¢ç¬¦åæ¡ä»¶çæ­æ²ä¿¡æ¯|`search_song`|
 |æ¥è¯¢æå®æ­æ²æå®é¾åº¦çè°±é¢|`song_chart`|
 |æ¥è¯¢æ­æ²åæ°è¡¨|`song_meta`|
 |æ¥è¯¢æå®æ´»å¨çæå®æ¡£ä½é¢æµçº¿|`ycx`|
-|æ¥è¯¢æå®æ´»å¨çå¨é¨æ¡£ä½é¢æµçº¿|`ycx_all`|
-|æäº¤è½¦çä¿¡æ¯å°åç«¯|`station_submit_room_number`|
-|ä»åç«¯è·åæè¿çè½¦çä¿¡æ¯åè¡¨|`station_query_all_room`| ####
-ç¨æ·æ°æ®åç«¯åè½ |åè½æè¿°|æ¹æ³åç§°| |:------|:----------
+|æ¥è¯¢æå®æ´»å¨çå¨é¨æ¡£ä½é¢æµçº¿|`ycx_all`| ####
+è½¦ç«æ°æ®åç«¯åè½ |åè½æè¿°|æ¹æ³åç§°| |:------|:----------
+| |æäº¤æ¿é´ä¿¡æ¯å°åç«¯|`station_submit_room_number`|
+|ä»åç«¯è·åæè¿çæ¿é´ä¿¡æ¯åè¡¨|`station_query_all_room`| >
+è¥åç«¯ä¸æ¯æç¨æ·æ°æ®åºï¼ä»¥ä¸åè½å¯è½æ æ³ä½¿ç¨ï¼è¯·ä»¥
+**è½¦ç«åè½** API ä»£æ¿ã #### ç¨æ·æ°æ®åç«¯åè½
+|åè½æè¿°|æ¹æ³åç§°| |:------|:----------
 | |è·åç¨æ·æ°æ®|`get_user_data`| |ä¿®æ¹ç¨æ·æ°æ®|`change_user_data`|
 |åéç»å®ç¨æ·è¯·æ±|`bind_player_request`|
 |éªè¯ç»å®ç¨æ·è¯·æ±|`bind_player_verification`| >
 ä»¥ä¸åè½é½å¯ä½¿ç¨æ¬å°ç¨æ·æ°æ®åºä»£æ¿ï¼æ¬ API
 ä¸æä¾ç¸å³çéç½®æ¹æ³ã #### è½¦ç«åè½ |åè½æè¿°|æ¹æ³åç§°|
-|:------|:----------| |æäº¤è½¦çä¿¡æ¯å°è½¦ç«|`submit_room_number`| ##
-å¿«éä½¿ç¨ ä»¥ä¸å°ä»¥è·åæ­æ² **EXIST** (id=325) çä¿¡æ¯ä¸ºä¾ã
+|:------|:----------
+| |ä»è½¦ç«è·åæè¿çæ¿é´ä¿¡æ¯åè¡¨|`query_room_number`|
+|æäº¤æ¿é´ä¿¡æ¯å°è½¦ç«|`submit_room_number`| ## å¿«éä½¿ç¨
+ä»¥ä¸å°ä»¥è·åæ­æ² **EXIST** (id=325) çä¿¡æ¯ä¸ºä¾ã
 ä½¿ç¨ä»¥ä¸æä»¤å®è£æ¬æ¨¡åï¼ ```bash $ pip3 install tsugu-api-python
 ``` ä½¿ç¨å¦ä¸ä»£ç ï¼è·åæå®æ­æ²ä¿¡æ¯å¾çï¼ ```python from
 tsugu_api import search_song def main() -> None: result = search_song([3, 0],
 "EXIST") # è¿éä¹å¯ä»¥ä¼ å¥ "325" ï¼å·ä½åå³äºç¨æ·è¾å¥ä¿¡æ¯
 main() ``` > `[3, 0]` æä»£ç¨æ·çé»è®¤æå¡å¨åè¡¨ï¼å¯ä»éè¿
 `get_user_data()` æ¹æ³è·åçè¿åå¼ä¸­è·åã è·åå°ç `result`
 å°æ¯ä¸ä¸ª `_Response` å¯¹è±¡ï¼å½è·åå°åç¡®çä¿¡æ¯æ¶ï¼ `result`
```

### Comparing `tsugu-api-python-1.1.2/tsugu_api_python.egg-info/SOURCES.txt` & `tsugu-api-python-1.1.3/tsugu_api_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

