# Comparing `tmp/nonebot-plugin-hx-yinying-1.2.13.tar.gz` & `tmp/nonebot-plugin-hx-yinying-1.2.14.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot-plugin-hx-yinying-1.2.13.tar", last modified: Wed May 15 12:58:00 2024, max compression
+gzip compressed data, was "nonebot-plugin-hx-yinying-1.2.14.tar", last modified: Wed May 15 15:23:04 2024, max compression
```

## Comparing `nonebot-plugin-hx-yinying-1.2.13.tar` & `nonebot-plugin-hx-yinying-1.2.14.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-05-15 12:58:00.879761 nonebot-plugin-hx-yinying-1.2.13/
--rw-rw-rw-   0        0        0     1098 2024-04-16 15:27:11.000000 nonebot-plugin-hx-yinying-1.2.13/LICENSE
--rw-rw-rw-   0        0        0     6503 2024-05-15 12:58:00.879761 nonebot-plugin-hx-yinying-1.2.13/PKG-INFO
--rw-rw-rw-   0        0        0     6062 2024-04-28 16:24:12.000000 nonebot-plugin-hx-yinying-1.2.13/README.md
-drwxrwxrwx   0        0        0        0 2024-05-15 12:58:00.718650 nonebot-plugin-hx-yinying-1.2.13/nonebot_plugin_hx_yinying/
--rw-rw-rw-   0        0        0    54995 2024-05-12 17:17:24.000000 nonebot-plugin-hx-yinying-1.2.13/nonebot_plugin_hx_yinying/__init__.py
--rw-rw-rw-   0        0        0    75105 2024-05-15 12:50:11.000000 nonebot-plugin-hx-yinying-1.2.13/nonebot_plugin_hx_yinying/chat.py
--rw-rw-rw-   0        0        0     1533 2024-05-15 12:56:45.000000 nonebot-plugin-hx-yinying-1.2.13/nonebot_plugin_hx_yinying/config.py
--rw-rw-rw-   0        0        0     2549 2024-05-11 16:56:48.000000 nonebot-plugin-hx-yinying-1.2.13/nonebot_plugin_hx_yinying/image_check.py
--rw-rw-rw-   0        0        0     5372 2024-05-15 12:56:18.000000 nonebot-plugin-hx-yinying-1.2.13/nonebot_plugin_hx_yinying/report.py
--rw-rw-rw-   0        0        0     5032 2024-05-12 17:16:42.000000 nonebot-plugin-hx-yinying-1.2.13/nonebot_plugin_hx_yinying/smms.py
-drwxrwxrwx   0        0        0        0 2024-05-15 12:58:00.868724 nonebot-plugin-hx-yinying-1.2.13/nonebot_plugin_hx_yinying.egg-info/
--rw-rw-rw-   0        0        0     6503 2024-05-15 12:57:59.000000 nonebot-plugin-hx-yinying-1.2.13/nonebot_plugin_hx_yinying.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      499 2024-05-15 12:57:59.000000 nonebot-plugin-hx-yinying-1.2.13/nonebot_plugin_hx_yinying.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-15 12:57:59.000000 nonebot-plugin-hx-yinying-1.2.13/nonebot_plugin_hx_yinying.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      274 2024-05-15 12:57:59.000000 nonebot-plugin-hx-yinying-1.2.13/nonebot_plugin_hx_yinying.egg-info/requires.txt
--rw-rw-rw-   0        0        0       26 2024-05-15 12:57:59.000000 nonebot-plugin-hx-yinying-1.2.13/nonebot_plugin_hx_yinying.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       85 2024-05-15 12:58:00.889374 nonebot-plugin-hx-yinying-1.2.13/setup.cfg
--rw-rw-rw-   0        0        0     1003 2024-05-15 12:56:38.000000 nonebot-plugin-hx-yinying-1.2.13/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-15 15:23:03.888590 nonebot-plugin-hx-yinying-1.2.14/
+-rw-rw-rw-   0        0        0     1098 2024-04-16 15:27:11.000000 nonebot-plugin-hx-yinying-1.2.14/LICENSE
+-rw-rw-rw-   0        0        0     6503 2024-05-15 15:23:03.890615 nonebot-plugin-hx-yinying-1.2.14/PKG-INFO
+-rw-rw-rw-   0        0        0     6062 2024-04-28 16:24:12.000000 nonebot-plugin-hx-yinying-1.2.14/README.md
+drwxrwxrwx   0        0        0        0 2024-05-15 15:23:03.758363 nonebot-plugin-hx-yinying-1.2.14/nonebot_plugin_hx_yinying/
+-rw-rw-rw-   0        0        0    56210 2024-05-15 15:18:50.000000 nonebot-plugin-hx-yinying-1.2.14/nonebot_plugin_hx_yinying/__init__.py
+-rw-rw-rw-   0        0        0    75184 2024-05-15 14:51:11.000000 nonebot-plugin-hx-yinying-1.2.14/nonebot_plugin_hx_yinying/chat.py
+-rw-rw-rw-   0        0        0     1533 2024-05-15 15:19:12.000000 nonebot-plugin-hx-yinying-1.2.14/nonebot_plugin_hx_yinying/config.py
+-rw-rw-rw-   0        0        0     2549 2024-05-11 16:56:48.000000 nonebot-plugin-hx-yinying-1.2.14/nonebot_plugin_hx_yinying/image_check.py
+-rw-rw-rw-   0        0        0     5372 2024-05-15 12:55:21.000000 nonebot-plugin-hx-yinying-1.2.14/nonebot_plugin_hx_yinying/report.py
+-rw-rw-rw-   0        0        0     5032 2024-05-12 17:16:42.000000 nonebot-plugin-hx-yinying-1.2.14/nonebot_plugin_hx_yinying/smms.py
+drwxrwxrwx   0        0        0        0 2024-05-15 15:23:03.878036 nonebot-plugin-hx-yinying-1.2.14/nonebot_plugin_hx_yinying.egg-info/
+-rw-rw-rw-   0        0        0     6503 2024-05-15 15:23:02.000000 nonebot-plugin-hx-yinying-1.2.14/nonebot_plugin_hx_yinying.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      499 2024-05-15 15:23:03.000000 nonebot-plugin-hx-yinying-1.2.14/nonebot_plugin_hx_yinying.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-15 15:23:02.000000 nonebot-plugin-hx-yinying-1.2.14/nonebot_plugin_hx_yinying.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      274 2024-05-15 15:23:02.000000 nonebot-plugin-hx-yinying-1.2.14/nonebot_plugin_hx_yinying.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       26 2024-05-15 15:23:02.000000 nonebot-plugin-hx-yinying-1.2.14/nonebot_plugin_hx_yinying.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       85 2024-05-15 15:23:03.976684 nonebot-plugin-hx-yinying-1.2.14/setup.cfg
+-rw-rw-rw-   0        0        0     1003 2024-05-15 15:22:36.000000 nonebot-plugin-hx-yinying-1.2.14/setup.py
```

### Comparing `nonebot-plugin-hx-yinying-1.2.13/LICENSE` & `nonebot-plugin-hx-yinying-1.2.14/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-hx-yinying-1.2.13/PKG-INFO` & `nonebot-plugin-hx-yinying-1.2.14/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-hx-yinying
-Version: 1.2.13
+Version: 1.2.14
 Summary: chat with yinying
 Home-page: https://github.com/huanxin996/nonebot_plugin_hx-yinying
 Author: Huan Xin
 Author-email: mc.xiaolang@foxmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-hx-yinying Version: 1.2.13 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-hx-yinying Version: 1.2.14 Summary:
 chat with yinying Home-page: https://github.com/huanxin996/nonebot_plugin_hx-
 yinying Author: Huan Xin Author-email: mc.xiaolang@foxmail.com Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Description-Content-
 Type: text/markdown License-File: LICENSE [![All Contributors](https://
 img.shields.io/badge/all_contributors-2-orange.svg?style=flat-square)]
 (#contributors-) * @Author : huanxin996 * @Date : 2024-4-17 * @LastEditors :
```

### Comparing `nonebot-plugin-hx-yinying-1.2.13/README.md` & `nonebot-plugin-hx-yinying-1.2.14/README.md`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-hx-yinying-1.2.13/nonebot_plugin_hx_yinying/__init__.py` & `nonebot-plugin-hx-yinying-1.2.14/nonebot_plugin_hx_yinying/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -85,16 +85,43 @@
 model_handoff = on_command("切换模型", aliases={"qhmodel","切换chat模型","模型切换"},rule=Rule(chek_rule_base),  priority=0, block=True)
 easycyber_set = on_command("easycyber", aliases={"easycyber设置","hxworld"},rule=Rule(chek_rule_base),  priority=0, block=True)
 cyber_set = on_command("cyber", aliases={"cyber设置","Hxworld"},rule=Rule(chek_rule_base),  priority=0, block=True)
 admin_set = on_command("控制台操作", aliases={"管理控制台","setstart"},rule=Rule(chek_rule_admin),  priority=0, block=True)
 verision = on_command("确认版本", aliases={"旅行伙伴确认","版本确认"},rule=Rule(chek_rule_base),  priority=0, block=True)
 character = on_command("sd", aliases={"旅行伙伴加入","设定加入"},rule=Rule(chek_rule_base),  priority=0, block=True)
 chat_ne = on_command("加入订阅", aliases={"旅行伙伴觉醒","订阅加入"},rule=Rule(chek_rule_base),  priority=0, block=True)
+time_noend = on_command("切换时间线", aliases={"切换模式"},rule=Rule(chek_rule_base),  priority=0, block=True)
 ces = on_command("测试服务", aliases={"测试报错"},rule=Rule(chek_rule_base), priority=0, block=True)
 
+#生命模式-无限时间(仅供cyber和easycyber使用)
+@time_noend.got(
+    "msg",
+    prompt=f"请输入时间线\n当前仅支持\n无限-overworld\n普通-nether\n请输入全称：无限-overworld",
+)
+async def time_noend(matcher: Matcher,bot:Bot, event: MessageEvent):
+    text = unescape(event.get_plaintext().strip())
+    config_1 = config_in_user(get_id(event),False)
+    user_config = json_get(config_1,get_id(event))
+    lines = user_config.get("model_endless",False)
+    if text == "无限-overworld" and lines != True:
+        user_config["model_endless"] = True
+        with open(f'{log_dir}/config/config_user.json','w',encoding='utf-8') as file:
+            json.dump(config_1,file)
+        msg = ".载入成功"
+    elif text == "普通-nether" and lines != False:
+        user_config["model_endless"] = True
+        with open(f'{log_dir}/config/config_user.json','w',encoding='utf-8') as file:
+            json.dump(config_1,file)
+        msg = "..载入成功"
+    else:
+        msg = "时间线重叠..."
+    await send_msg(matcher,event,msg)
+
+
+
 #自定义自己的设定
 @character.handle()
 async def character(matcher: Matcher,bot:Bot, event: MessageEvent, msg: Message = CommandArg()):
     user = get_id(event)
     nick = await get_nick(bot,event)
     config = config_in_user(user,nick)
     config_get = json_get(config,user)
```

### Comparing `nonebot-plugin-hx-yinying-1.2.13/nonebot_plugin_hx_yinying/chat.py` & `nonebot-plugin-hx-yinying-1.2.14/nonebot_plugin_hx_yinying/chat.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -- coding: utf-8 --**
-from nonebot.adapters.onebot.v11 import Bot, GroupMessageEvent ,MessageSegment ,Message,MessageEvent,Event
+from nonebot.adapters.onebot.v11 import Bot, GroupMessageEvent ,MessageSegment ,Message,MessageEvent,Event,PrivateMessageEvent
 from html import unescape
 from typing import List
 import os,httpx, json, time, requests,platform
 from loguru import logger as lg
 from .config import Config
 import operator,nonebot,random
 from nonebot import get_plugin_config, logger, require,get_driver
@@ -187,15 +187,14 @@
             seg.data["url"]
             for seg in event.message
             if (seg.type == "image") and ("url" in seg.data)
         ]
     )
     return urls
 
-
 #创建用户文件夹
 def create_dir_usr(path):
     if not os.path.exists(path):
         os.mkdir(path)
 
 #获取json函数
 def json_get(data, *keys, default=None):
@@ -216,15 +215,14 @@
 def json_get_time(json,key) -> str:
     try:
         back = json[f"{key}"]
     except Exception as e:
         back = 1
     return back
 
-
 #json转义防止爆炸（）
 def json_replace(text) -> str:
     text = text.replace('\n','/n')
     text = text.replace('\t','/t')
     text = text.replace("'","/'")
     text = text.replace('"','/"')
     return text
@@ -272,15 +270,15 @@
         if new_verision <= hx_config.hx_version:
             logger.success(f"[Hx_YinYing]:你的Hx_YinYing已经是最新版本了！当前版本为{hx_config.hx_version},仓库版本为{new_verision}")
         else:
             logger.success("[Hx_YinYing]:检查到Hx_YinYing有新版本！")
             venv = os.getcwd()
             if os.path.exists(f"{venv}/.venv"):
                 logger.success("【Hx】正在自动更新中--找到虚拟环境![开始安装]")
-                os.system(f'f"{venv}/.venv/Scripts/python.exe" -m pip install nonebot-plugin-hx-yinying=={new_verision} -i https://pypi.Python.org/simple/')
+                os.system(f'"{venv}/.venv/Scripts/python.exe" -m pip install nonebot-plugin-hx-yinying=={new_verision} -i https://pypi.Python.org/simple/')
                 logger.success(f"[Hx_YinYing]:更新完成！最新版本为{new_verision}|当前使用版本为{hx_config.hx_version}")
                 logger.warning(f"[Hx_YinYing]:你可能需要重新启动nonebot来完成插件的重载")
             else:
                 logger.warning("【Hx】正在自动更新中--未找到虚拟环境！[安装在本地环境]")
                 os.system(f'pip install nonebot-plugin-hx-yinying=={new_verision} -i https://pypi.Python.org/simple/')
                 logger.success(f"[Hx_YinYing]:更新完成！最新版本为{new_verision}|当前使用版本为{hx_config.hx_version}")
                 logger.warning(f"[Hx_YinYing]:你可能需要重新启动nonebot来完成插件的重载")
@@ -862,27 +860,29 @@
         superuser = get_superuser()
         white_group = json_get(config, "white_group")
         white_user = json_get(config, "white_user")
         black_group = json_get(config, "blacklist_group")
         black_user = json_get(config, "blacklist_user")
         rule_mode = json_get(config, "rule_model")
         at_reply = json_get(config, "at_reply", default=False)
-        private = json_get(config, "private", default=False)
+        private = json_get(config, "private", default=True)
         def check_user_group_rules(to_me):
             is_admin = id in admin_list or id == admin_pro or id in superuser
             is_white = group_id in white_group or id in white_user
-            is_black = group_id in black_group or id in black_user
-            is_at_reply = at_reply if isinstance(eve, GroupMessageEvent) else True and to_me
-            return is_admin or is_white or (is_black and not is_at_reply)
+            is_black = group_id not in black_group or id not in black_user
+            is_private = private if isinstance(eve, GroupMessageEvent) else True
+            if to_me and isinstance(eve, GroupMessageEvent):
+                return at_reply
+            return is_admin or is_white or (is_private and is_black)
         if isinstance(eve, GroupMessageEvent):
             to_me = event.to_me
-            if rule_mode == "black":
-                return check_user_group_rules(to_me)
-            elif rule_mode == "white":
+            if rule_mode == "white":
                 return check_user_group_rules(to_me) or group_id in white_group
+            else:
+                return check_user_group_rules(to_me)
         elif not isinstance(eve, GroupMessageEvent) and not private:
             return False
         else:
             return check_user_group_rules(True)
     except Exception as e:
         logger.error(f"配置验证异常: {str(e)}")
         return True
```

### Comparing `nonebot-plugin-hx-yinying-1.2.13/nonebot_plugin_hx_yinying/config.py` & `nonebot-plugin-hx-yinying-1.2.14/nonebot_plugin_hx_yinying/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from typing import List, Optional, Union
 import nonebot
 from pydantic import BaseModel,AnyHttpUrl,Field
 
 
 class Config(BaseModel):
     # 插件版本号勿动！！！！
-    hx_version: Optional[str] = "1.2.13"
+    hx_version: Optional[str] = "1.2.14"
     # 秩乱v你的appid
     yinying_appid: Optional[str] = None
     # 秩乱给你的token
     yinying_token: Optional[str] = None
     # 插件数据文件存储路径，可不填。
     hx_path: Optional[str] = None
     # 图像检查api，爱来自阿里云
```

### Comparing `nonebot-plugin-hx-yinying-1.2.13/nonebot_plugin_hx_yinying/image_check.py` & `nonebot-plugin-hx-yinying-1.2.14/nonebot_plugin_hx_yinying/image_check.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-hx-yinying-1.2.13/nonebot_plugin_hx_yinying/report.py` & `nonebot-plugin-hx-yinying-1.2.14/nonebot_plugin_hx_yinying/report.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-hx-yinying-1.2.13/nonebot_plugin_hx_yinying/smms.py` & `nonebot-plugin-hx-yinying-1.2.14/nonebot_plugin_hx_yinying/smms.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-hx-yinying-1.2.13/nonebot_plugin_hx_yinying.egg-info/PKG-INFO` & `nonebot-plugin-hx-yinying-1.2.14/nonebot_plugin_hx_yinying.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-hx-yinying
-Version: 1.2.13
+Version: 1.2.14
 Summary: chat with yinying
 Home-page: https://github.com/huanxin996/nonebot_plugin_hx-yinying
 Author: Huan Xin
 Author-email: mc.xiaolang@foxmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-hx-yinying Version: 1.2.13 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-hx-yinying Version: 1.2.14 Summary:
 chat with yinying Home-page: https://github.com/huanxin996/nonebot_plugin_hx-
 yinying Author: Huan Xin Author-email: mc.xiaolang@foxmail.com Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Description-Content-
 Type: text/markdown License-File: LICENSE [![All Contributors](https://
 img.shields.io/badge/all_contributors-2-orange.svg?style=flat-square)]
 (#contributors-) * @Author : huanxin996 * @Date : 2024-4-17 * @LastEditors :
```

### Comparing `nonebot-plugin-hx-yinying-1.2.13/setup.py` & `nonebot-plugin-hx-yinying-1.2.14/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="nonebot-plugin-hx-yinying",
-    version="1.2.13",
+    version="1.2.14",
     author="Huan Xin",
     author_email="mc.xiaolang@foxmail.com",
     description="chat with yinying",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/huanxin996/nonebot_plugin_hx-yinying",
     packages=setuptools.find_packages(),
```

