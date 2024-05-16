# Comparing `tmp/nonebot_plugin_sparkapi-1.0.6.tar.gz` & `tmp/nonebot_plugin_sparkapi-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_sparkapi-1.0.6.tar", last modified: Thu May 16 02:56:54 2024, max compression
+gzip compressed data, was "nonebot_plugin_sparkapi-1.0.7.tar", last modified: Thu May 16 05:04:51 2024, max compression
```

## Comparing `nonebot_plugin_sparkapi-1.0.6.tar` & `nonebot_plugin_sparkapi-1.0.7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-05-16 02:56:54.114294 nonebot_plugin_sparkapi-1.0.6/
--rw-rw-rw-   0        0        0     1084 2024-05-15 03:42:49.000000 nonebot_plugin_sparkapi-1.0.6/LICENSE
--rw-rw-rw-   0        0        0     7216 2024-05-16 02:56:54.113405 nonebot_plugin_sparkapi-1.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     5465 2024-05-16 02:38:32.000000 nonebot_plugin_sparkapi-1.0.6/README.md
-drwxrwxrwx   0        0        0        0 2024-05-16 02:56:54.106584 nonebot_plugin_sparkapi-1.0.6/nonebot_plugin_sparkapi/
--rw-rw-rw-   0        0        0     4680 2024-05-16 02:46:33.000000 nonebot_plugin_sparkapi-1.0.6/nonebot_plugin_sparkapi/SparkApi.py
--rw-rw-rw-   0        0        0     7402 2024-05-16 02:49:46.000000 nonebot_plugin_sparkapi-1.0.6/nonebot_plugin_sparkapi/__init__.py
--rw-rw-rw-   0        0        0     1734 2024-05-16 01:17:15.000000 nonebot_plugin_sparkapi-1.0.6/nonebot_plugin_sparkapi/config.py
--rw-rw-rw-   0        0        0     2391 2024-05-16 01:28:50.000000 nonebot_plugin_sparkapi-1.0.6/nonebot_plugin_sparkapi/data.py
--rw-rw-rw-   0        0        0     1779 2024-05-16 02:50:14.000000 nonebot_plugin_sparkapi-1.0.6/nonebot_plugin_sparkapi/funcs.py
-drwxrwxrwx   0        0        0        0 2024-05-16 02:56:54.112364 nonebot_plugin_sparkapi-1.0.6/nonebot_plugin_sparkapi.egg-info/
--rw-rw-rw-   0        0        0     7216 2024-05-16 02:56:54.000000 nonebot_plugin_sparkapi-1.0.6/nonebot_plugin_sparkapi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      437 2024-05-16 02:56:54.000000 nonebot_plugin_sparkapi-1.0.6/nonebot_plugin_sparkapi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-16 02:56:54.000000 nonebot_plugin_sparkapi-1.0.6/nonebot_plugin_sparkapi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       94 2024-05-16 02:56:54.000000 nonebot_plugin_sparkapi-1.0.6/nonebot_plugin_sparkapi.egg-info/requires.txt
--rw-rw-rw-   0        0        0       24 2024-05-16 02:56:54.000000 nonebot_plugin_sparkapi-1.0.6/nonebot_plugin_sparkapi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      654 2024-05-16 02:53:36.000000 nonebot_plugin_sparkapi-1.0.6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-16 02:56:54.114533 nonebot_plugin_sparkapi-1.0.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 05:04:51.752089 nonebot_plugin_sparkapi-1.0.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-16 05:04:47.000000 nonebot_plugin_sparkapi-1.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7272 2024-05-16 05:04:51.752089 nonebot_plugin_sparkapi-1.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5555 2024-05-16 05:04:47.000000 nonebot_plugin_sparkapi-1.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 05:04:51.748089 nonebot_plugin_sparkapi-1.0.7/nonebot_plugin_sparkapi/
+-rw-r--r--   0 runner    (1001) docker     (127)     4528 2024-05-16 05:04:47.000000 nonebot_plugin_sparkapi-1.0.7/nonebot_plugin_sparkapi/SparkApi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8416 2024-05-16 05:04:47.000000 nonebot_plugin_sparkapi-1.0.7/nonebot_plugin_sparkapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1725 2024-05-16 05:04:47.000000 nonebot_plugin_sparkapi-1.0.7/nonebot_plugin_sparkapi/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2526 2024-05-16 05:04:47.000000 nonebot_plugin_sparkapi-1.0.7/nonebot_plugin_sparkapi/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2444 2024-05-16 05:04:47.000000 nonebot_plugin_sparkapi-1.0.7/nonebot_plugin_sparkapi/funcs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 05:04:51.752089 nonebot_plugin_sparkapi-1.0.7/nonebot_plugin_sparkapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7272 2024-05-16 05:04:51.000000 nonebot_plugin_sparkapi-1.0.7/nonebot_plugin_sparkapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-05-16 05:04:51.000000 nonebot_plugin_sparkapi-1.0.7/nonebot_plugin_sparkapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 05:04:51.000000 nonebot_plugin_sparkapi-1.0.7/nonebot_plugin_sparkapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-16 05:04:51.000000 nonebot_plugin_sparkapi-1.0.7/nonebot_plugin_sparkapi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-16 05:04:51.000000 nonebot_plugin_sparkapi-1.0.7/nonebot_plugin_sparkapi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-16 05:04:47.000000 nonebot_plugin_sparkapi-1.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 05:04:51.752089 nonebot_plugin_sparkapi-1.0.7/setup.cfg
```

### Comparing `nonebot_plugin_sparkapi-1.0.6/PKG-INFO` & `nonebot_plugin_sparkapi-1.0.7/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,159 +1,163 @@
-Metadata-Version: 2.1
-Name: nonebot_plugin_sparkapi
-Version: 1.0.6
-Summary: Nonebot2 ChatBot that calls the official API of the iflyrec Spark LLM for all model versions, defaulting to the current latest (v3.5)
-Author-email: CCLMSY <2502408581@qq.com>
-License: MIT License
-        
-        Copyright (c) 2024 CCLMSY
-        
-        Permission is hereby granted, free of charge, to any person obtaining a copy
-        of this software and associated documentation files (the "Software"), to deal
-        in the Software without restriction, including without limitation the rights
-        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-        copies of the Software, and to permit persons to whom the Software is
-        furnished to do so, subject to the following conditions:
-        
-        The above copyright notice and this permission notice shall be included in all
-        copies or substantial portions of the Software.
-        
-        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-        SOFTWARE.
-        
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: nonebot-adapter-onebot<3.0.0,>=2.2.1
-Requires-Dist: nonebot2<3.0.0,>=2.0.0rc3
-Requires-Dist: websocket-client<2.0.0,>=1.6.1
-
-<div align="center">
-  <a href="https://v2.nonebot.dev/store"><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/nbp_logo.png" width="180" height="180" alt="NoneBotPluginLogo"></a>
-  <br>
-  <p><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/NoneBotPlugin.svg" width="240" alt="NoneBotPluginText"></p>
-</div>
-
-<div align="center">
-
-# nonebot-plugin-sparkapi
-
-_✨ 科大讯飞星火大语言模型官方API聊天机器人 ✨_
-
-<a href="./LICENSE">
-    <img src="https://img.shields.io/github/license/CCLMSY/nonebot-plugin-sparkapi.svg" alt="license">
-</a>
-<a href="https://pypi.python.org/pypi/nonebot-plugin-sparkapi">
-    <img src="https://img.shields.io/pypi/v/nonebot-plugin-sparkapi.svg" alt="pypi">
-</a>
-<img src="https://img.shields.io/badge/python-3.8+-blue.svg" alt="python">
-
-</div>
-
-## 📖 介绍
-
-基于Nonebot2平台，调用科大讯飞星火大语言模型官方API的AI聊天机器人插件
-
-适用于所有模型版本（默认当前最新（v3.5）），支持上下文关联、人物预设等功能
-
-### 💬 功能
-- [x] 支持AI对话
-- [x] 支持上下文关联记忆（可设置记忆文本长度）
-- [x] 用户鉴别（每个用户的历史记录独立）
-- [x] 支持使用、切换人物预设（prompt）
-- [x] 人物预设菜单自动生成，更改无需重写
-- [x] 功能菜单自动生成，更改无需重写
-- [x] 完善的配置项（有其他需求请发issue）
-- [ ] 实用功能列表（查天气、查快递等）
-- [ ] 用户权限与功能区分（超级用户、普通用户）
-- [ ] 支持星火助手API
-- [ ] 支持用户自定义、更改预设
-- [ ] 基于pickle的历史记录持久化
-
-### 📦 项目地址
-- Github：https://github.com/CCLMSY/nonebot-plugin-sparkapi 
-- 觉得好用的话，请给个 Star⭐️ 谢谢喵~ 
-
-## 💿 安装
-
-<details open>
-<summary>使用 nb-cli 安装</summary>
-在 nonebot2 项目的根目录下打开命令行, 输入以下指令即可安装
-
-    nb plugin install nonebot-plugin-sparkapi
-
-</details>
-
-<details>
-<summary>使用包管理器安装</summary>
-在 nonebot2 项目的插件目录下, 打开命令行, 根据你使用的包管理器, 输入相应的安装命令
-
-<details>
-<summary>pip</summary>
-
-    pip install nonebot-plugin-sparkapi
-</details>
-<details>
-<summary>pdm</summary>
-
-    pdm add nonebot-plugin-sparkapi
-</details>
-<details>
-<summary>poetry</summary>
-
-    poetry add nonebot-plugin-sparkapi
-</details>
-<details>
-<summary>conda</summary>
-
-    conda install nonebot-plugin-sparkapi
-</details>
-
-打开 nonebot2 项目根目录下的 `pyproject.toml` 文件, 在 `[tool.nonebot]` 部分追加写入
-
-    plugins = ["nonebot_plugin_sparkapi"]
-
-</details>
-
-## ⚙️ 配置
-
-在 nonebot2 项目的`.env`文件中添加下表中的必填配置
-
-其中，服务接口认证信息 app_id, api_secret, api_key 请前往 [讯飞开放平台控制台](https://console.xfyun.cn/) 获取
-
-| 配置项 | 必填 | 默认值 | 说明 |
-|:-----:|:----:|:----:|:----:|
-| sparkapi_app_id | 是 | "" | APPID |
-| sparkapi_api_secret | 是 | "" | APISecret |
-| sparkapi_api_key | 是 | "" | APIKey |
-| sparkapi_model_version | 否 | "" | 星火大模型的版本，默认为当前最新。<br>可选值：v3.5, v3.0, v2.0, v1.5 |
-| sparkapi_model_top_k | 否 | 4 | 平衡生成文本的质量和多样性。<br>较小的 k 值会减少随机性，使得输出更加稳定；<br>而较大的 k 值会增加随机性，产生更多新颖的输出。<br>取值范围[1, 6] |
-| sparkapi_model_temperature | 否 | 0.5 | 控制结果随机性，取值越高随机性越强，即相同的问题得到的不同答案的可能性越高。<br>取值范围 (0，1] |
-| sparkapi_command_chat | 否 | "" | 机器人对话指令，默认为空可直接对话<br>（需要同时在`.env`中配置命令起始字符为空<br>COMMAND_START = [""]） |
-| sparkapi_private_chat | 否 | True | 是否允许私聊使用 |
-| sparkapi_group_public | 否 | False | 群聊启用公共会话<br>True：所有人共享同一会话<br>False：每个人的会话各自独立 |
-| sparkapi_group_at | 否 | True | 群聊回复消息时是否需要@提问者 |
-| sparkapi_fnotice | 否 | True | 收到请求时是否提示“已收到请求” |
-| sparkapi_priority | 否 | 90 | 事件响应器优先级，[1,99]，数字越小优先级越高 |
-| sparkpai_max_length | 否 | 8000 | 上下文最大长度，[1,8000]<br>单次发送和回复的消息不能超过该项的一半 |
-| sparkapi_setpreset_clear | 否 | True | 切换人物预设时是否清空对话历史记录 |
-| sparkapi_bot_name | 否 | "" | 机器人的名字 |
-
-
-## 🎉 使用
-### 指令表
-| 指令 | 需要@ | 范围 | 说明 |
-|:-----:|:----:|:----:|:----:|
-| sparkapi_command_chat（若不为空） + 对话内容 | 是 | 私聊/群聊 | 与机器人进行对话 |
-| help | 是 | 私聊/群聊 | 查看帮助信息 |
-| showpresets | 是 | 私聊/群聊 | 查看当前可选的人物预设 |
-| setpreset | 是 | 私聊/群聊 | 查看当前可选的人物预设<br>回复编号以进行切换<br> |
-| setpreset + 人物预设编号 | 是 | 私聊/群聊 | 切换到编号对应的人物预设 |
-| clear | 是 | 私聊/群聊 | 清除当前对话上下文 |
-
-### 效果图
-![demo](https://github.com/CCLMSY/nonebot-plugin-sparkapi/blob/resources/demo.jpg)
+Metadata-Version: 2.1
+Name: nonebot_plugin_sparkapi
+Version: 1.0.7
+Summary: Nonebot2 ChatBot that calls the official API of the iflyrec Spark LLM for all model versions, defaulting to the current latest (v3.5)
+Author-email: CCLMSY <2502408581@qq.com>
+License: MIT License
+        
+        Copyright (c) 2024 CCLMSY
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all
+        copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+        SOFTWARE.
+        
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: nonebot-adapter-onebot<3.0.0,>=2.2.1
+Requires-Dist: nonebot2<3.0.0,>=2.0.0rc3
+Requires-Dist: websocket-client<2.0.0,>=1.6.1
+
+<div align="center">
+  <a href="https://v2.nonebot.dev/store"><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/nbp_logo.png" width="180" height="180" alt="NoneBotPluginLogo"></a>
+  <br>
+  <p><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/NoneBotPlugin.svg" width="240" alt="NoneBotPluginText"></p>
+</div>
+
+<div align="center">
+
+# nonebot-plugin-sparkapi
+
+_✨ 科大讯飞星火大语言模型官方API聊天机器人 ✨_
+
+<a href="./LICENSE">
+    <img src="https://img.shields.io/github/license/CCLMSY/nonebot-plugin-sparkapi.svg" alt="license">
+</a>
+<a href="https://pypi.python.org/pypi/nonebot-plugin-sparkapi">
+    <img src="https://img.shields.io/pypi/v/nonebot-plugin-sparkapi.svg" alt="pypi">
+</a>
+<img src="https://img.shields.io/badge/python-3.8+-blue.svg" alt="python">
+
+</div>
+
+## 📖 介绍
+
+基于Nonebot2平台，调用科大讯飞星火大语言模型官方API的AI聊天机器人插件
+
+适用于所有模型版本（默认当前最新（v3.5）），支持上下文关联、人物预设等功能
+
+### 💬 功能
+- [x] 支持AI对话
+- [x] 支持上下文关联记忆（可设置记忆文本长度）
+- [x] 用户鉴别（每个用户的历史记录独立）
+- [x] 支持使用、切换人物预设（prompt）
+- [x] 人物预设菜单自动生成，更改无需重写
+- [x] 功能菜单自动生成，更改无需重写
+- [x] 完善的配置项（有其他需求请发issue）
+- [x] 历史记录持久化
+- [ ] 实用功能列表（查天气、查快递等）
+- [ ] 用户权限与功能区分（超级用户、普通用户）
+- [ ] 支持星火助手API
+- [ ] 支持用户自定义、更改预设
+
+### 📦 项目地址
+- Github：https://github.com/CCLMSY/nonebot-plugin-sparkapi 
+- 觉得好用的话，请给个 Star⭐️ 谢谢喵~ 
+
+## 💿 安装
+
+<details open>
+<summary>使用 nb-cli 安装</summary>
+在 nonebot2 项目的根目录下打开命令行, 输入以下指令即可安装
+
+    nb plugin install nonebot-plugin-sparkapi
+
+</details>
+
+<details>
+<summary>使用包管理器安装</summary>
+在 nonebot2 项目的插件目录下, 打开命令行, 根据你使用的包管理器, 输入相应的安装命令
+
+<details>
+<summary>pip</summary>
+
+    pip install nonebot-plugin-sparkapi
+</details>
+<details>
+<summary>pdm</summary>
+
+    pdm add nonebot-plugin-sparkapi
+</details>
+<details>
+<summary>poetry</summary>
+
+    poetry add nonebot-plugin-sparkapi
+</details>
+<details>
+<summary>conda</summary>
+
+    conda install nonebot-plugin-sparkapi
+</details>
+
+打开 nonebot2 项目根目录下的 `pyproject.toml` 文件, 在 `[tool.nonebot]` 部分追加写入
+
+    plugins = ["nonebot_plugin_sparkapi"]
+
+</details>
+
+## ⚙️ 配置
+
+在 nonebot2 项目的`.env`文件中添加下表中的必填配置
+
+其中，服务接口认证信息 app_id, api_secret, api_key 请前往 [讯飞开放平台控制台](https://console.xfyun.cn/) 获取
+
+| 配置项 | 必填 | 默认值 | 说明 |
+|:-----:|:----:|:----:|:----:|
+| sparkapi_app_id | 是 | "" | APPID |
+| sparkapi_api_secret | 是 | "" | APISecret |
+| sparkapi_api_key | 是 | "" | APIKey |
+| sparkapi_model_version | 否 | "" | 星火大模型的版本，默认为当前最新。<br>可选值：v3.5, v3.0, v2.0, v1.5 |
+| sparkapi_model_top_k | 否 | 4 | 平衡生成文本的质量和多样性。<br>较小的 k 值会减少随机性，使得输出更加稳定；<br>而较大的 k 值会增加随机性，产生更多新颖的输出。<br>取值范围[1, 6] |
+| sparkapi_model_temperature | 否 | 0.5 | 控制结果随机性，取值越高随机性越强，即相同的问题得到的不同答案的可能性越高。<br>取值范围 (0，1] |
+| sparkapi_command_chat | 否 | "" | 机器人对话指令，默认为空可直接对话<br>（需要同时在`.env`中配置命令起始字符为空<br>COMMAND_START = [""]） |
+| sparkapi_private_chat | 否 | True | 是否允许私聊使用 |
+| sparkapi_group_public | 否 | False | 群聊启用公共会话<br>True：所有人共享同一会话<br>False：每个人的会话各自独立 |
+| sparkapi_group_at | 否 | True | 群聊回复消息时是否需要@提问者 |
+| sparkapi_fnotice | 否 | True | 收到请求时是否提示“已收到请求” |
+| sparkapi_priority | 否 | 90 | 事件响应器优先级，[1,99]，数字越小优先级越高 |
+| sparkpai_max_length | 否 | 8000 | 上下文最大长度，[1,8000]<br>单次发送和回复的消息不能超过该项的一半 |
+| sparkapi_setpreset_clear | 否 | True | 切换人物预设时是否清除当前对话上下文 |
+| sparkapi_bot_name | 否 | "" | 机器人的名字 |
+
+
+## 🎉 使用
+### 指令表
+所有指令均可在data.py中修改，且无需重写菜单/指令生成函数
+
+| 指令 | 需要@ | 范围 | 说明 |
+|:-----:|:----:|:----:|:----:|
+| sparkapi_command_chat（若不为空） + 对话内容 | 是 | 私聊/群聊 | 与机器人进行对话 |
+| help | 是 | 私聊/群聊 | 查看帮助信息 |
+| showpresets | 是 | 私聊/群聊 | 查看当前可选的人物预设 |
+| setpreset | 是 | 私聊/群聊 | 查看当前可选的人物预设<br>回复编号以进行切换<br> |
+| setpreset + 人物预设编号 | 是 | 私聊/群聊 | 切换到编号对应的人物预设 |
+| savesession | 是 | 私聊/群聊 | 保存当前对话上下文 |
+| loadsession | 是 | 私聊/群聊 | 加载之前保存的对话上下文 |
+| clear | 是 | 私聊/群聊 | 清除当前对话上下文 |
+
+### 效果图
+![demo](https://github.com/CCLMSY/nonebot-plugin-sparkapi/blob/resources/demo.jpg)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot_plugin_sparkapi Version: 1.0.6 Summary:
+Metadata-Version: 2.1 Name: nonebot_plugin_sparkapi Version: 1.0.7 Summary:
 Nonebot2 ChatBot that calls the official API of the iflyrec Spark LLM for all
 model versions, defaulting to the current latest (v3.5) Author-email: CCLMSY
 <2502408581@qq.com> License: MIT License Copyright (c) 2024 CCLMSY Permission
 is hereby granted, free of charge, to any person obtaining a copy of this
 software and associated documentation files (the "Software"), to deal in the
 Software without restriction, including without limitation the rights to use,
 copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the
@@ -29,29 +29,29 @@
 éç¨äºæææ¨¡åçæ¬ï¼é»è®¤å½åææ°ï¼v3.5ï¼ï¼ï¼æ¯æä¸ä¸æå³èãäººç©é¢è®¾ç­åè½
 ### ð¬ åè½ - [x] æ¯æAIå¯¹è¯ - [x]
 æ¯æä¸ä¸æå³èè®°å¿ï¼å¯è®¾ç½®è®°å¿ææ¬é¿åº¦ï¼ - [x]
 ç¨æ·é´å«ï¼æ¯ä¸ªç¨æ·çåå²è®°å½ç¬ç«ï¼ - [x]
 æ¯æä½¿ç¨ãåæ¢äººç©é¢è®¾ï¼promptï¼ - [x]
 äººç©é¢è®¾èåèªå¨çæï¼æ´æ¹æ ééå - [x]
 åè½èåèªå¨çæï¼æ´æ¹æ ééå - [x]
-å®åçéç½®é¡¹ï¼æå¶ä»éæ±è¯·åissueï¼ - [ ]
-å®ç¨åè½åè¡¨ï¼æ¥å¤©æ°ãæ¥å¿«éç­ï¼ - [ ]
+å®åçéç½®é¡¹ï¼æå¶ä»éæ±è¯·åissueï¼ - [x] åå²è®°å½æä¹å
+- [ ] å®ç¨åè½åè¡¨ï¼æ¥å¤©æ°ãæ¥å¿«éç­ï¼ - [ ]
 ç¨æ·æéä¸åè½åºåï¼è¶çº§ç¨æ·ãæ®éç¨æ·ï¼ - [ ]
-æ¯ææç«å©æAPI - [ ] æ¯æç¨æ·èªå®ä¹ãæ´æ¹é¢è®¾ - [ ]
-åºäºpickleçåå²è®°å½æä¹å ### ð¦ é¡¹ç®å°å - Githubï¼https://
-github.com/CCLMSY/nonebot-plugin-sparkapi - è§å¾å¥½ç¨çè¯ï¼è¯·ç»ä¸ª
-Starâ­ï¸ è°¢è°¢åµ~ ## ð¿ å®è£ ä½¿ç¨ nb-cli å®è£ å¨ nonebot2
-é¡¹ç®çæ ¹ç®å½ä¸æå¼å½ä»¤è¡, è¾å¥ä»¥ä¸æä»¤å³å¯å®è£ nb plugin
-install nonebot-plugin-sparkapi ä½¿ç¨åç®¡çå¨å®è£ å¨ nonebot2
-é¡¹ç®çæä»¶ç®å½ä¸, æå¼å½ä»¤è¡, æ ¹æ®ä½ ä½¿ç¨çåç®¡çå¨,
-è¾å¥ç¸åºçå®è£å½ä»¤ pip pip install nonebot-plugin-sparkapi pdm pdm add
-nonebot-plugin-sparkapi poetry poetry add nonebot-plugin-sparkapi conda conda
-install nonebot-plugin-sparkapi æå¼ nonebot2 é¡¹ç®æ ¹ç®å½ä¸ç
-`pyproject.toml` æä»¶, å¨ `[tool.nonebot]` é¨åè¿½å åå¥ plugins =
-["nonebot_plugin_sparkapi"] ## âï¸ éç½® å¨ nonebot2
+æ¯ææç«å©æAPI - [ ] æ¯æç¨æ·èªå®ä¹ãæ´æ¹é¢è®¾ ### ð¦
+é¡¹ç®å°å - Githubï¼https://github.com/CCLMSY/nonebot-plugin-sparkapi -
+è§å¾å¥½ç¨çè¯ï¼è¯·ç»ä¸ª Starâ­ï¸ è°¢è°¢åµ~ ## ð¿ å®è£ ä½¿ç¨ nb-
+cli å®è£ å¨ nonebot2 é¡¹ç®çæ ¹ç®å½ä¸æå¼å½ä»¤è¡,
+è¾å¥ä»¥ä¸æä»¤å³å¯å®è£ nb plugin install nonebot-plugin-sparkapi
+ä½¿ç¨åç®¡çå¨å®è£ å¨ nonebot2 é¡¹ç®çæä»¶ç®å½ä¸,
+æå¼å½ä»¤è¡, æ ¹æ®ä½ ä½¿ç¨çåç®¡çå¨, è¾å¥ç¸åºçå®è£å½ä»¤
+pip pip install nonebot-plugin-sparkapi pdm pdm add nonebot-plugin-sparkapi
+poetry poetry add nonebot-plugin-sparkapi conda conda install nonebot-plugin-
+sparkapi æå¼ nonebot2 é¡¹ç®æ ¹ç®å½ä¸ç `pyproject.toml` æä»¶, å¨ `
+[tool.nonebot]` é¨åè¿½å åå¥ plugins = ["nonebot_plugin_sparkapi"] ##
+âï¸ éç½® å¨ nonebot2
 é¡¹ç®ç`.env`æä»¶ä¸­æ·»å ä¸è¡¨ä¸­çå¿å¡«éç½®
 å¶ä¸­ï¼æå¡æ¥å£è®¤è¯ä¿¡æ¯ app_id, api_secret, api_key è¯·åå¾
 [è®¯é£å¼æ¾å¹³å°æ§å¶å°](https://console.xfyun.cn/) è·å | éç½®é¡¹ |
 å¿å¡« | é»è®¤å¼ | è¯´æ | |:-----:|:----:|:----:|:----:| | sparkapi_app_id
 | æ¯ | "" | APPID | | sparkapi_api_secret | æ¯ | "" | APISecret | |
 sparkapi_api_key | æ¯ | "" | APIKey | | sparkapi_model_version | å¦ | "" |
 æç«å¤§æ¨¡åççæ¬ï¼é»è®¤ä¸ºå½åææ°ã
@@ -71,19 +71,23 @@
 Falseï¼æ¯ä¸ªäººçä¼è¯åèªç¬ç« | | sparkapi_group_at | å¦ | True |
 ç¾¤èåå¤æ¶æ¯æ¶æ¯å¦éè¦@æé®è | | sparkapi_fnotice | å¦ | True |
 æ¶å°è¯·æ±æ¶æ¯å¦æç¤ºâå·²æ¶å°è¯·æ±â | | sparkapi_priority | å¦ |
 90 | äºä»¶ååºå¨ä¼åçº§ï¼[1,99]ï¼æ°å­è¶å°ä¼åçº§è¶é« | |
 sparkpai_max_length | å¦ | 8000 | ä¸ä¸ææå¤§é¿åº¦ï¼[1,8000]
 åæ¬¡åéååå¤çæ¶æ¯ä¸è½è¶è¿è¯¥é¡¹çä¸å | |
 sparkapi_setpreset_clear | å¦ | True |
-åæ¢äººç©é¢è®¾æ¶æ¯å¦æ¸ç©ºå¯¹è¯åå²è®°å½ | | sparkapi_bot_name | å¦
-| "" | æºå¨äººçåå­ | ## ð ä½¿ç¨ ### æä»¤è¡¨ | æä»¤ | éè¦@ |
-èå´ | è¯´æ | |:-----:|:----:|:----:|:----:| |
-sparkapi_command_chatï¼è¥ä¸ä¸ºç©ºï¼ + å¯¹è¯åå®¹ | æ¯ | ç§è/ç¾¤è |
-ä¸æºå¨äººè¿è¡å¯¹è¯ | | help | æ¯ | ç§è/ç¾¤è | æ¥çå¸®å©ä¿¡æ¯ |
-| showpresets | æ¯ | ç§è/ç¾¤è | æ¥çå½åå¯éçäººç©é¢è®¾ | |
-setpreset | æ¯ | ç§è/ç¾¤è | æ¥çå½åå¯éçäººç©é¢è®¾
+åæ¢äººç©é¢è®¾æ¶æ¯å¦æ¸é¤å½åå¯¹è¯ä¸ä¸æ | | sparkapi_bot_name |
+å¦ | "" | æºå¨äººçåå­ | ## ð ä½¿ç¨ ### æä»¤è¡¨
+æææä»¤åå¯å¨data.pyä¸­ä¿®æ¹ï¼ä¸æ ééåèå/
+æä»¤çæå½æ° | æä»¤ | éè¦@ | èå´ | è¯´æ | |:-----:|:----:|:---
+-:|:----:| | sparkapi_command_chatï¼è¥ä¸ä¸ºç©ºï¼ + å¯¹è¯åå®¹ | æ¯ |
+ç§è/ç¾¤è | ä¸æºå¨äººè¿è¡å¯¹è¯ | | help | æ¯ | ç§è/ç¾¤è |
+æ¥çå¸®å©ä¿¡æ¯ | | showpresets | æ¯ | ç§è/ç¾¤è |
+æ¥çå½åå¯éçäººç©é¢è®¾ | | setpreset | æ¯ | ç§è/ç¾¤è |
+æ¥çå½åå¯éçäººç©é¢è®¾
 åå¤ç¼å·ä»¥è¿è¡åæ¢
 | | setpreset + äººç©é¢è®¾ç¼å· | æ¯ | ç§è/ç¾¤è |
-åæ¢å°ç¼å·å¯¹åºçäººç©é¢è®¾ | | clear | æ¯ | ç§è/ç¾¤è |
+åæ¢å°ç¼å·å¯¹åºçäººç©é¢è®¾ | | savesession | æ¯ | ç§è/ç¾¤è |
+ä¿å­å½åå¯¹è¯ä¸ä¸æ | | loadsession | æ¯ | ç§è/ç¾¤è |
+å è½½ä¹åä¿å­çå¯¹è¯ä¸ä¸æ | | clear | æ¯ | ç§è/ç¾¤è |
 æ¸é¤å½åå¯¹è¯ä¸ä¸æ | ### ææå¾ ![demo](https://github.com/CCLMSY/
 nonebot-plugin-sparkapi/blob/resources/demo.jpg)
```

### Comparing `nonebot_plugin_sparkapi-1.0.6/README.md` & `nonebot_plugin_sparkapi-1.0.7/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,125 +1,129 @@
-<div align="center">
-  <a href="https://v2.nonebot.dev/store"><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/nbp_logo.png" width="180" height="180" alt="NoneBotPluginLogo"></a>
-  <br>
-  <p><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/NoneBotPlugin.svg" width="240" alt="NoneBotPluginText"></p>
-</div>
-
-<div align="center">
-
-# nonebot-plugin-sparkapi
-
-_✨ 科大讯飞星火大语言模型官方API聊天机器人 ✨_
-
-<a href="./LICENSE">
-    <img src="https://img.shields.io/github/license/CCLMSY/nonebot-plugin-sparkapi.svg" alt="license">
-</a>
-<a href="https://pypi.python.org/pypi/nonebot-plugin-sparkapi">
-    <img src="https://img.shields.io/pypi/v/nonebot-plugin-sparkapi.svg" alt="pypi">
-</a>
-<img src="https://img.shields.io/badge/python-3.8+-blue.svg" alt="python">
-
-</div>
-
-## 📖 介绍
-
-基于Nonebot2平台，调用科大讯飞星火大语言模型官方API的AI聊天机器人插件
-
-适用于所有模型版本（默认当前最新（v3.5）），支持上下文关联、人物预设等功能
-
-### 💬 功能
-- [x] 支持AI对话
-- [x] 支持上下文关联记忆（可设置记忆文本长度）
-- [x] 用户鉴别（每个用户的历史记录独立）
-- [x] 支持使用、切换人物预设（prompt）
-- [x] 人物预设菜单自动生成，更改无需重写
-- [x] 功能菜单自动生成，更改无需重写
-- [x] 完善的配置项（有其他需求请发issue）
-- [ ] 实用功能列表（查天气、查快递等）
-- [ ] 用户权限与功能区分（超级用户、普通用户）
-- [ ] 支持星火助手API
-- [ ] 支持用户自定义、更改预设
-- [ ] 基于pickle的历史记录持久化
-
-### 📦 项目地址
-- Github：https://github.com/CCLMSY/nonebot-plugin-sparkapi 
-- 觉得好用的话，请给个 Star⭐️ 谢谢喵~ 
-
-## 💿 安装
-
-<details open>
-<summary>使用 nb-cli 安装</summary>
-在 nonebot2 项目的根目录下打开命令行, 输入以下指令即可安装
-
-    nb plugin install nonebot-plugin-sparkapi
-
-</details>
-
-<details>
-<summary>使用包管理器安装</summary>
-在 nonebot2 项目的插件目录下, 打开命令行, 根据你使用的包管理器, 输入相应的安装命令
-
-<details>
-<summary>pip</summary>
-
-    pip install nonebot-plugin-sparkapi
-</details>
-<details>
-<summary>pdm</summary>
-
-    pdm add nonebot-plugin-sparkapi
-</details>
-<details>
-<summary>poetry</summary>
-
-    poetry add nonebot-plugin-sparkapi
-</details>
-<details>
-<summary>conda</summary>
-
-    conda install nonebot-plugin-sparkapi
-</details>
-
-打开 nonebot2 项目根目录下的 `pyproject.toml` 文件, 在 `[tool.nonebot]` 部分追加写入
-
-    plugins = ["nonebot_plugin_sparkapi"]
-
-</details>
-
-## ⚙️ 配置
-
-在 nonebot2 项目的`.env`文件中添加下表中的必填配置
-
-其中，服务接口认证信息 app_id, api_secret, api_key 请前往 [讯飞开放平台控制台](https://console.xfyun.cn/) 获取
-
-| 配置项 | 必填 | 默认值 | 说明 |
-|:-----:|:----:|:----:|:----:|
-| sparkapi_app_id | 是 | "" | APPID |
-| sparkapi_api_secret | 是 | "" | APISecret |
-| sparkapi_api_key | 是 | "" | APIKey |
-| sparkapi_model_version | 否 | "" | 星火大模型的版本，默认为当前最新。<br>可选值：v3.5, v3.0, v2.0, v1.5 |
-| sparkapi_model_top_k | 否 | 4 | 平衡生成文本的质量和多样性。<br>较小的 k 值会减少随机性，使得输出更加稳定；<br>而较大的 k 值会增加随机性，产生更多新颖的输出。<br>取值范围[1, 6] |
-| sparkapi_model_temperature | 否 | 0.5 | 控制结果随机性，取值越高随机性越强，即相同的问题得到的不同答案的可能性越高。<br>取值范围 (0，1] |
-| sparkapi_command_chat | 否 | "" | 机器人对话指令，默认为空可直接对话<br>（需要同时在`.env`中配置命令起始字符为空<br>COMMAND_START = [""]） |
-| sparkapi_private_chat | 否 | True | 是否允许私聊使用 |
-| sparkapi_group_public | 否 | False | 群聊启用公共会话<br>True：所有人共享同一会话<br>False：每个人的会话各自独立 |
-| sparkapi_group_at | 否 | True | 群聊回复消息时是否需要@提问者 |
-| sparkapi_fnotice | 否 | True | 收到请求时是否提示“已收到请求” |
-| sparkapi_priority | 否 | 90 | 事件响应器优先级，[1,99]，数字越小优先级越高 |
-| sparkpai_max_length | 否 | 8000 | 上下文最大长度，[1,8000]<br>单次发送和回复的消息不能超过该项的一半 |
-| sparkapi_setpreset_clear | 否 | True | 切换人物预设时是否清空对话历史记录 |
-| sparkapi_bot_name | 否 | "" | 机器人的名字 |
-
-
-## 🎉 使用
-### 指令表
-| 指令 | 需要@ | 范围 | 说明 |
-|:-----:|:----:|:----:|:----:|
-| sparkapi_command_chat（若不为空） + 对话内容 | 是 | 私聊/群聊 | 与机器人进行对话 |
-| help | 是 | 私聊/群聊 | 查看帮助信息 |
-| showpresets | 是 | 私聊/群聊 | 查看当前可选的人物预设 |
-| setpreset | 是 | 私聊/群聊 | 查看当前可选的人物预设<br>回复编号以进行切换<br> |
-| setpreset + 人物预设编号 | 是 | 私聊/群聊 | 切换到编号对应的人物预设 |
-| clear | 是 | 私聊/群聊 | 清除当前对话上下文 |
-
-### 效果图
-![demo](https://github.com/CCLMSY/nonebot-plugin-sparkapi/blob/resources/demo.jpg)
+<div align="center">
+  <a href="https://v2.nonebot.dev/store"><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/nbp_logo.png" width="180" height="180" alt="NoneBotPluginLogo"></a>
+  <br>
+  <p><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/NoneBotPlugin.svg" width="240" alt="NoneBotPluginText"></p>
+</div>
+
+<div align="center">
+
+# nonebot-plugin-sparkapi
+
+_✨ 科大讯飞星火大语言模型官方API聊天机器人 ✨_
+
+<a href="./LICENSE">
+    <img src="https://img.shields.io/github/license/CCLMSY/nonebot-plugin-sparkapi.svg" alt="license">
+</a>
+<a href="https://pypi.python.org/pypi/nonebot-plugin-sparkapi">
+    <img src="https://img.shields.io/pypi/v/nonebot-plugin-sparkapi.svg" alt="pypi">
+</a>
+<img src="https://img.shields.io/badge/python-3.8+-blue.svg" alt="python">
+
+</div>
+
+## 📖 介绍
+
+基于Nonebot2平台，调用科大讯飞星火大语言模型官方API的AI聊天机器人插件
+
+适用于所有模型版本（默认当前最新（v3.5）），支持上下文关联、人物预设等功能
+
+### 💬 功能
+- [x] 支持AI对话
+- [x] 支持上下文关联记忆（可设置记忆文本长度）
+- [x] 用户鉴别（每个用户的历史记录独立）
+- [x] 支持使用、切换人物预设（prompt）
+- [x] 人物预设菜单自动生成，更改无需重写
+- [x] 功能菜单自动生成，更改无需重写
+- [x] 完善的配置项（有其他需求请发issue）
+- [x] 历史记录持久化
+- [ ] 实用功能列表（查天气、查快递等）
+- [ ] 用户权限与功能区分（超级用户、普通用户）
+- [ ] 支持星火助手API
+- [ ] 支持用户自定义、更改预设
+
+### 📦 项目地址
+- Github：https://github.com/CCLMSY/nonebot-plugin-sparkapi 
+- 觉得好用的话，请给个 Star⭐️ 谢谢喵~ 
+
+## 💿 安装
+
+<details open>
+<summary>使用 nb-cli 安装</summary>
+在 nonebot2 项目的根目录下打开命令行, 输入以下指令即可安装
+
+    nb plugin install nonebot-plugin-sparkapi
+
+</details>
+
+<details>
+<summary>使用包管理器安装</summary>
+在 nonebot2 项目的插件目录下, 打开命令行, 根据你使用的包管理器, 输入相应的安装命令
+
+<details>
+<summary>pip</summary>
+
+    pip install nonebot-plugin-sparkapi
+</details>
+<details>
+<summary>pdm</summary>
+
+    pdm add nonebot-plugin-sparkapi
+</details>
+<details>
+<summary>poetry</summary>
+
+    poetry add nonebot-plugin-sparkapi
+</details>
+<details>
+<summary>conda</summary>
+
+    conda install nonebot-plugin-sparkapi
+</details>
+
+打开 nonebot2 项目根目录下的 `pyproject.toml` 文件, 在 `[tool.nonebot]` 部分追加写入
+
+    plugins = ["nonebot_plugin_sparkapi"]
+
+</details>
+
+## ⚙️ 配置
+
+在 nonebot2 项目的`.env`文件中添加下表中的必填配置
+
+其中，服务接口认证信息 app_id, api_secret, api_key 请前往 [讯飞开放平台控制台](https://console.xfyun.cn/) 获取
+
+| 配置项 | 必填 | 默认值 | 说明 |
+|:-----:|:----:|:----:|:----:|
+| sparkapi_app_id | 是 | "" | APPID |
+| sparkapi_api_secret | 是 | "" | APISecret |
+| sparkapi_api_key | 是 | "" | APIKey |
+| sparkapi_model_version | 否 | "" | 星火大模型的版本，默认为当前最新。<br>可选值：v3.5, v3.0, v2.0, v1.5 |
+| sparkapi_model_top_k | 否 | 4 | 平衡生成文本的质量和多样性。<br>较小的 k 值会减少随机性，使得输出更加稳定；<br>而较大的 k 值会增加随机性，产生更多新颖的输出。<br>取值范围[1, 6] |
+| sparkapi_model_temperature | 否 | 0.5 | 控制结果随机性，取值越高随机性越强，即相同的问题得到的不同答案的可能性越高。<br>取值范围 (0，1] |
+| sparkapi_command_chat | 否 | "" | 机器人对话指令，默认为空可直接对话<br>（需要同时在`.env`中配置命令起始字符为空<br>COMMAND_START = [""]） |
+| sparkapi_private_chat | 否 | True | 是否允许私聊使用 |
+| sparkapi_group_public | 否 | False | 群聊启用公共会话<br>True：所有人共享同一会话<br>False：每个人的会话各自独立 |
+| sparkapi_group_at | 否 | True | 群聊回复消息时是否需要@提问者 |
+| sparkapi_fnotice | 否 | True | 收到请求时是否提示“已收到请求” |
+| sparkapi_priority | 否 | 90 | 事件响应器优先级，[1,99]，数字越小优先级越高 |
+| sparkpai_max_length | 否 | 8000 | 上下文最大长度，[1,8000]<br>单次发送和回复的消息不能超过该项的一半 |
+| sparkapi_setpreset_clear | 否 | True | 切换人物预设时是否清除当前对话上下文 |
+| sparkapi_bot_name | 否 | "" | 机器人的名字 |
+
+
+## 🎉 使用
+### 指令表
+所有指令均可在data.py中修改，且无需重写菜单/指令生成函数
+
+| 指令 | 需要@ | 范围 | 说明 |
+|:-----:|:----:|:----:|:----:|
+| sparkapi_command_chat（若不为空） + 对话内容 | 是 | 私聊/群聊 | 与机器人进行对话 |
+| help | 是 | 私聊/群聊 | 查看帮助信息 |
+| showpresets | 是 | 私聊/群聊 | 查看当前可选的人物预设 |
+| setpreset | 是 | 私聊/群聊 | 查看当前可选的人物预设<br>回复编号以进行切换<br> |
+| setpreset + 人物预设编号 | 是 | 私聊/群聊 | 切换到编号对应的人物预设 |
+| savesession | 是 | 私聊/群聊 | 保存当前对话上下文 |
+| loadsession | 是 | 私聊/群聊 | 加载之前保存的对话上下文 |
+| clear | 是 | 私聊/群聊 | 清除当前对话上下文 |
+
+### 效果图
+![demo](https://github.com/CCLMSY/nonebot-plugin-sparkapi/blob/resources/demo.jpg)
```

#### html2text {}

```diff
@@ -8,29 +8,29 @@
 éç¨äºæææ¨¡åçæ¬ï¼é»è®¤å½åææ°ï¼v3.5ï¼ï¼ï¼æ¯æä¸ä¸æå³èãäººç©é¢è®¾ç­åè½
 ### ð¬ åè½ - [x] æ¯æAIå¯¹è¯ - [x]
 æ¯æä¸ä¸æå³èè®°å¿ï¼å¯è®¾ç½®è®°å¿ææ¬é¿åº¦ï¼ - [x]
 ç¨æ·é´å«ï¼æ¯ä¸ªç¨æ·çåå²è®°å½ç¬ç«ï¼ - [x]
 æ¯æä½¿ç¨ãåæ¢äººç©é¢è®¾ï¼promptï¼ - [x]
 äººç©é¢è®¾èåèªå¨çæï¼æ´æ¹æ ééå - [x]
 åè½èåèªå¨çæï¼æ´æ¹æ ééå - [x]
-å®åçéç½®é¡¹ï¼æå¶ä»éæ±è¯·åissueï¼ - [ ]
-å®ç¨åè½åè¡¨ï¼æ¥å¤©æ°ãæ¥å¿«éç­ï¼ - [ ]
+å®åçéç½®é¡¹ï¼æå¶ä»éæ±è¯·åissueï¼ - [x] åå²è®°å½æä¹å
+- [ ] å®ç¨åè½åè¡¨ï¼æ¥å¤©æ°ãæ¥å¿«éç­ï¼ - [ ]
 ç¨æ·æéä¸åè½åºåï¼è¶çº§ç¨æ·ãæ®éç¨æ·ï¼ - [ ]
-æ¯ææç«å©æAPI - [ ] æ¯æç¨æ·èªå®ä¹ãæ´æ¹é¢è®¾ - [ ]
-åºäºpickleçåå²è®°å½æä¹å ### ð¦ é¡¹ç®å°å - Githubï¼https://
-github.com/CCLMSY/nonebot-plugin-sparkapi - è§å¾å¥½ç¨çè¯ï¼è¯·ç»ä¸ª
-Starâ­ï¸ è°¢è°¢åµ~ ## ð¿ å®è£ ä½¿ç¨ nb-cli å®è£ å¨ nonebot2
-é¡¹ç®çæ ¹ç®å½ä¸æå¼å½ä»¤è¡, è¾å¥ä»¥ä¸æä»¤å³å¯å®è£ nb plugin
-install nonebot-plugin-sparkapi ä½¿ç¨åç®¡çå¨å®è£ å¨ nonebot2
-é¡¹ç®çæä»¶ç®å½ä¸, æå¼å½ä»¤è¡, æ ¹æ®ä½ ä½¿ç¨çåç®¡çå¨,
-è¾å¥ç¸åºçå®è£å½ä»¤ pip pip install nonebot-plugin-sparkapi pdm pdm add
-nonebot-plugin-sparkapi poetry poetry add nonebot-plugin-sparkapi conda conda
-install nonebot-plugin-sparkapi æå¼ nonebot2 é¡¹ç®æ ¹ç®å½ä¸ç
-`pyproject.toml` æä»¶, å¨ `[tool.nonebot]` é¨åè¿½å åå¥ plugins =
-["nonebot_plugin_sparkapi"] ## âï¸ éç½® å¨ nonebot2
+æ¯ææç«å©æAPI - [ ] æ¯æç¨æ·èªå®ä¹ãæ´æ¹é¢è®¾ ### ð¦
+é¡¹ç®å°å - Githubï¼https://github.com/CCLMSY/nonebot-plugin-sparkapi -
+è§å¾å¥½ç¨çè¯ï¼è¯·ç»ä¸ª Starâ­ï¸ è°¢è°¢åµ~ ## ð¿ å®è£ ä½¿ç¨ nb-
+cli å®è£ å¨ nonebot2 é¡¹ç®çæ ¹ç®å½ä¸æå¼å½ä»¤è¡,
+è¾å¥ä»¥ä¸æä»¤å³å¯å®è£ nb plugin install nonebot-plugin-sparkapi
+ä½¿ç¨åç®¡çå¨å®è£ å¨ nonebot2 é¡¹ç®çæä»¶ç®å½ä¸,
+æå¼å½ä»¤è¡, æ ¹æ®ä½ ä½¿ç¨çåç®¡çå¨, è¾å¥ç¸åºçå®è£å½ä»¤
+pip pip install nonebot-plugin-sparkapi pdm pdm add nonebot-plugin-sparkapi
+poetry poetry add nonebot-plugin-sparkapi conda conda install nonebot-plugin-
+sparkapi æå¼ nonebot2 é¡¹ç®æ ¹ç®å½ä¸ç `pyproject.toml` æä»¶, å¨ `
+[tool.nonebot]` é¨åè¿½å åå¥ plugins = ["nonebot_plugin_sparkapi"] ##
+âï¸ éç½® å¨ nonebot2
 é¡¹ç®ç`.env`æä»¶ä¸­æ·»å ä¸è¡¨ä¸­çå¿å¡«éç½®
 å¶ä¸­ï¼æå¡æ¥å£è®¤è¯ä¿¡æ¯ app_id, api_secret, api_key è¯·åå¾
 [è®¯é£å¼æ¾å¹³å°æ§å¶å°](https://console.xfyun.cn/) è·å | éç½®é¡¹ |
 å¿å¡« | é»è®¤å¼ | è¯´æ | |:-----:|:----:|:----:|:----:| | sparkapi_app_id
 | æ¯ | "" | APPID | | sparkapi_api_secret | æ¯ | "" | APISecret | |
 sparkapi_api_key | æ¯ | "" | APIKey | | sparkapi_model_version | å¦ | "" |
 æç«å¤§æ¨¡åççæ¬ï¼é»è®¤ä¸ºå½åææ°ã
@@ -50,19 +50,23 @@
 Falseï¼æ¯ä¸ªäººçä¼è¯åèªç¬ç« | | sparkapi_group_at | å¦ | True |
 ç¾¤èåå¤æ¶æ¯æ¶æ¯å¦éè¦@æé®è | | sparkapi_fnotice | å¦ | True |
 æ¶å°è¯·æ±æ¶æ¯å¦æç¤ºâå·²æ¶å°è¯·æ±â | | sparkapi_priority | å¦ |
 90 | äºä»¶ååºå¨ä¼åçº§ï¼[1,99]ï¼æ°å­è¶å°ä¼åçº§è¶é« | |
 sparkpai_max_length | å¦ | 8000 | ä¸ä¸ææå¤§é¿åº¦ï¼[1,8000]
 åæ¬¡åéååå¤çæ¶æ¯ä¸è½è¶è¿è¯¥é¡¹çä¸å | |
 sparkapi_setpreset_clear | å¦ | True |
-åæ¢äººç©é¢è®¾æ¶æ¯å¦æ¸ç©ºå¯¹è¯åå²è®°å½ | | sparkapi_bot_name | å¦
-| "" | æºå¨äººçåå­ | ## ð ä½¿ç¨ ### æä»¤è¡¨ | æä»¤ | éè¦@ |
-èå´ | è¯´æ | |:-----:|:----:|:----:|:----:| |
-sparkapi_command_chatï¼è¥ä¸ä¸ºç©ºï¼ + å¯¹è¯åå®¹ | æ¯ | ç§è/ç¾¤è |
-ä¸æºå¨äººè¿è¡å¯¹è¯ | | help | æ¯ | ç§è/ç¾¤è | æ¥çå¸®å©ä¿¡æ¯ |
-| showpresets | æ¯ | ç§è/ç¾¤è | æ¥çå½åå¯éçäººç©é¢è®¾ | |
-setpreset | æ¯ | ç§è/ç¾¤è | æ¥çå½åå¯éçäººç©é¢è®¾
+åæ¢äººç©é¢è®¾æ¶æ¯å¦æ¸é¤å½åå¯¹è¯ä¸ä¸æ | | sparkapi_bot_name |
+å¦ | "" | æºå¨äººçåå­ | ## ð ä½¿ç¨ ### æä»¤è¡¨
+æææä»¤åå¯å¨data.pyä¸­ä¿®æ¹ï¼ä¸æ ééåèå/
+æä»¤çæå½æ° | æä»¤ | éè¦@ | èå´ | è¯´æ | |:-----:|:----:|:---
+-:|:----:| | sparkapi_command_chatï¼è¥ä¸ä¸ºç©ºï¼ + å¯¹è¯åå®¹ | æ¯ |
+ç§è/ç¾¤è | ä¸æºå¨äººè¿è¡å¯¹è¯ | | help | æ¯ | ç§è/ç¾¤è |
+æ¥çå¸®å©ä¿¡æ¯ | | showpresets | æ¯ | ç§è/ç¾¤è |
+æ¥çå½åå¯éçäººç©é¢è®¾ | | setpreset | æ¯ | ç§è/ç¾¤è |
+æ¥çå½åå¯éçäººç©é¢è®¾
 åå¤ç¼å·ä»¥è¿è¡åæ¢
 | | setpreset + äººç©é¢è®¾ç¼å· | æ¯ | ç§è/ç¾¤è |
-åæ¢å°ç¼å·å¯¹åºçäººç©é¢è®¾ | | clear | æ¯ | ç§è/ç¾¤è |
+åæ¢å°ç¼å·å¯¹åºçäººç©é¢è®¾ | | savesession | æ¯ | ç§è/ç¾¤è |
+ä¿å­å½åå¯¹è¯ä¸ä¸æ | | loadsession | æ¯ | ç§è/ç¾¤è |
+å è½½ä¹åä¿å­çå¯¹è¯ä¸ä¸æ | | clear | æ¯ | ç§è/ç¾¤è |
 æ¸é¤å½åå¯¹è¯ä¸ä¸æ | ### ææå¾ ![demo](https://github.com/CCLMSY/
 nonebot-plugin-sparkapi/blob/resources/demo.jpg)
```

### Comparing `nonebot_plugin_sparkapi-1.0.6/nonebot_plugin_sparkapi/SparkApi.py` & `nonebot_plugin_sparkapi-1.0.7/nonebot_plugin_sparkapi/SparkApi.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,152 +1,152 @@
-# type: ignore
-from datetime import datetime
-from time import mktime
-from wsgiref.handlers import format_date_time
-from urllib.parse import urlparse
-
-import hmac
-import hashlib
-import base64
-from urllib.parse import urlencode
-
-import _thread as thread
-import json
-import websocket
-import ssl
-
-from .config import Config
-from nonebot import get_driver
-conf = Config.parse_obj(get_driver().config.dict())
-
-model_top_k = conf.sparkapi_model_top_k
-model_temperature = conf.sparkapi_model_temperature
-max_length = conf.sparkpai_max_length
-
-answer = ""
-
-class Ws_Param(object):
-    # 初始化
-    def __init__(self, APPID, APIKey, APISecret, Spark_url):
-        self.APPID = APPID
-        self.APIKey = APIKey
-        self.APISecret = APISecret
-        self.host = urlparse(Spark_url).netloc 
-        self.path = urlparse(Spark_url).path
-        self.Spark_url = Spark_url
-        self.sid = ""
-
-    # 生成url
-    def create_url(self):
-        # 生成RFC1123格式的时间戳
-        now = datetime.now()
-        date = format_date_time(mktime(now.timetuple()))
-
-        # 拼接字符串
-        signature_origin = "host: " + self.host + "\n"
-        signature_origin += "date: " + date + "\n"
-        signature_origin += "GET " + self.path + " HTTP/1.1"
-
-        # 进行hmac-sha256进行加密
-        signature_sha = hmac.new(self.APISecret.encode('utf-8'), signature_origin.encode('utf-8'), digestmod=hashlib.sha256).digest()
-        signature_sha_base64 = base64.b64encode(signature_sha).decode(encoding='utf-8')
-        authorization_origin = f'api_key="{self.APIKey}", algorithm="hmac-sha256", headers="host date request-line", signature="{signature_sha_base64}"'
-        authorization = base64.b64encode(authorization_origin.encode('utf-8')).decode(encoding='utf-8')
-
-        # 将请求的鉴权参数组合为字典
-        v = {
-            "authorization": authorization,
-            "date": date,
-            "host": self.host
-        }
-        # 拼接鉴权参数，生成url
-        url = self.Spark_url + '?' + urlencode(v)
-
-        # print("APPID: " + self.APPID)
-        # print("APIKey: " + self.APIKey)
-        # print("APISecret: " + self.APISecret)
-        # print("signature_origin: " + signature_origin)
-        # print(url)
-        # 此处打印出建立连接时候的url,参考本demo的时候可取消上方打印的注释，比对相同参数时生成的url与自己代码生成的url是否一致
-        return url
-
-# 收到websocket错误的处理
-def on_error(ws, error):
-    print("### error:", error)
-
-
-# 收到websocket关闭的处理
-def on_close(ws, *args):
-    return
-
-# 收到websocket连接建立的处理
-def on_open(ws):
-    thread.start_new_thread(run, (ws,))
-
-
-def run(ws, *args):
-    data = json.dumps(gen_params(appid=ws.appid, domain= ws.domain,question=ws.question))
-    ws.send(data)
-
-
-# 收到websocket消息的处理
-def on_message(ws, message):
-    # print(message)
-    # print(time.time())
-    data = json.loads(message)
-    code = data['header']['code']
-    if code != 0:
-        err = f'请求错误: {code}, {data}'
-        print(err)
-        ws.close()
-    else:
-        # global sid
-        # sid = data["header"]["sid"]
-        choices = data["payload"]["choices"]
-        status = choices["status"]
-        content = choices["text"][0]["content"]
-        # print(content,end ="")
-        global answer
-        answer += content
-        # print(1)
-        if status == 2:
-            ws.close()
-
-
-def gen_params(appid, domain,question):
-    """
-    通过appid和用户的提问来生成请参数
-    """
-    data = {
-        "header": {
-            "app_id": appid,
-            "uid": "1234"
-        },
-        "parameter": {
-
-            "chat": {
-                "domain": domain,
-                "temperature": model_temperature,
-                "max_tokens": max_length//2,
-                "top_k": model_top_k,
-
-                "auditing": "default"
-            }
-        },
-        "payload": {
-            "message": {
-                "text": question
-            }
-        }
-    }
-    return data
-
-def main(appid, api_key, api_secret, Spark_url,domain, question,sid):
-    wsParam = Ws_Param(appid, api_key, api_secret, Spark_url)
-    websocket.enableTrace(False)
-    wsUrl = wsParam.create_url()
-    ws = websocket.WebSocketApp(wsUrl, on_message=on_message, on_error=on_error, on_close=on_close, on_open=on_open)
-    ws.appid = appid 
-    ws.question = question
-    ws.domain = domain
-    ws.sid = sid
-    ws.run_forever(sslopt={"cert_reqs": ssl.CERT_NONE})
+# type: ignore
+from datetime import datetime
+from time import mktime
+from wsgiref.handlers import format_date_time
+from urllib.parse import urlparse
+
+import hmac
+import hashlib
+import base64
+from urllib.parse import urlencode
+
+import _thread as thread
+import json
+import websocket
+import ssl
+
+from .config import Config
+from nonebot import get_driver
+conf = Config.parse_obj(get_driver().config.dict())
+
+model_top_k = conf.sparkapi_model_top_k
+model_temperature = conf.sparkapi_model_temperature
+max_length = conf.sparkpai_max_length
+
+answer = ""
+
+class Ws_Param(object):
+    # 初始化
+    def __init__(self, APPID, APIKey, APISecret, Spark_url):
+        self.APPID = APPID
+        self.APIKey = APIKey
+        self.APISecret = APISecret
+        self.host = urlparse(Spark_url).netloc 
+        self.path = urlparse(Spark_url).path
+        self.Spark_url = Spark_url
+        self.sid = ""
+
+    # 生成url
+    def create_url(self):
+        # 生成RFC1123格式的时间戳
+        now = datetime.now()
+        date = format_date_time(mktime(now.timetuple()))
+
+        # 拼接字符串
+        signature_origin = "host: " + self.host + "\n"
+        signature_origin += "date: " + date + "\n"
+        signature_origin += "GET " + self.path + " HTTP/1.1"
+
+        # 进行hmac-sha256进行加密
+        signature_sha = hmac.new(self.APISecret.encode('utf-8'), signature_origin.encode('utf-8'), digestmod=hashlib.sha256).digest()
+        signature_sha_base64 = base64.b64encode(signature_sha).decode(encoding='utf-8')
+        authorization_origin = f'api_key="{self.APIKey}", algorithm="hmac-sha256", headers="host date request-line", signature="{signature_sha_base64}"'
+        authorization = base64.b64encode(authorization_origin.encode('utf-8')).decode(encoding='utf-8')
+
+        # 将请求的鉴权参数组合为字典
+        v = {
+            "authorization": authorization,
+            "date": date,
+            "host": self.host
+        }
+        # 拼接鉴权参数，生成url
+        url = self.Spark_url + '?' + urlencode(v)
+
+        # print("APPID: " + self.APPID)
+        # print("APIKey: " + self.APIKey)
+        # print("APISecret: " + self.APISecret)
+        # print("signature_origin: " + signature_origin)
+        # print(url)
+        # 此处打印出建立连接时候的url,参考本demo的时候可取消上方打印的注释，比对相同参数时生成的url与自己代码生成的url是否一致
+        return url
+
+# 收到websocket错误的处理
+def on_error(ws, error):
+    print("### error:", error)
+
+
+# 收到websocket关闭的处理
+def on_close(ws, *args):
+    return
+
+# 收到websocket连接建立的处理
+def on_open(ws):
+    thread.start_new_thread(run, (ws,))
+
+
+def run(ws, *args):
+    data = json.dumps(gen_params(appid=ws.appid, domain= ws.domain,question=ws.question))
+    ws.send(data)
+
+
+# 收到websocket消息的处理
+def on_message(ws, message):
+    # print(message)
+    # print(time.time())
+    data = json.loads(message)
+    code = data['header']['code']
+    if code != 0:
+        err = f'请求错误: {code}, {data}'
+        print(err)
+        ws.close()
+    else:
+        # global sid
+        # sid = data["header"]["sid"]
+        choices = data["payload"]["choices"]
+        status = choices["status"]
+        content = choices["text"][0]["content"]
+        # print(content,end ="")
+        global answer
+        answer += content
+        # print(1)
+        if status == 2:
+            ws.close()
+
+
+def gen_params(appid, domain,question):
+    """
+    通过appid和用户的提问来生成请参数
+    """
+    data = {
+        "header": {
+            "app_id": appid,
+            "uid": "1234"
+        },
+        "parameter": {
+
+            "chat": {
+                "domain": domain,
+                "temperature": model_temperature,
+                "max_tokens": max_length//2,
+                "top_k": model_top_k,
+
+                "auditing": "default"
+            }
+        },
+        "payload": {
+            "message": {
+                "text": question
+            }
+        }
+    }
+    return data
+
+def main(appid, api_key, api_secret, Spark_url,domain, question,sid):
+    wsParam = Ws_Param(appid, api_key, api_secret, Spark_url)
+    websocket.enableTrace(False)
+    wsUrl = wsParam.create_url()
+    ws = websocket.WebSocketApp(wsUrl, on_message=on_message, on_error=on_error, on_close=on_close, on_open=on_open)
+    ws.appid = appid 
+    ws.question = question
+    ws.domain = domain
+    ws.sid = sid
+    ws.run_forever(sslopt={"cert_reqs": ssl.CERT_NONE})
```

### Comparing `nonebot_plugin_sparkapi-1.0.6/nonebot_plugin_sparkapi/__init__.py` & `nonebot_plugin_sparkapi-1.0.7/nonebot_plugin_sparkapi/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -8,16 +8,16 @@
 
 import nonebot
 import asyncio
 from copy import deepcopy
 
 from .config import Config, ConfigError
 from . import SparkApi,funcs
-from .funcs import gethash,getlength,appendText
-from .data import presets, presets_lst, help_info
+from .funcs import gethash,getlength,appendText,save_session,load_session
+from .data import presets, presets_lst, help_info, commands
 
 __plugin_meta__ = PluginMetadata(
     name="科大讯飞星火大语言模型官方API聊天机器人插件",
     description="调用科大讯飞星火大语言模型官方API的聊天机器人插件，适用于所有模型版本（默认当前最新（v3.5）），支持上下文关联、人物预设",
     usage=help_info,
     type='application',
     homepage="https://github.com/CCLMSY/nonebot-plugin-sparkapi",
@@ -39,16 +39,14 @@
 # if not appid or not api_secret or not api_key:
 #     raise ConfigError("请设置API信息,可前往 https://console.xfyun.cn/ 获取")
 
 model_version = funcs.unify_model_version(conf.sparkapi_model_version)
 Spark_url = funcs.get_Spark_url(model_version)
 domain = funcs.get_domain(model_version)
 
-print("model_version:",model_version,"Spark_url:",Spark_url,"domain:",domain)
-
 command_chat = conf.sparkapi_command_chat
 private_chat = conf.sparkapi_private_chat
 group_public = conf.sparkapi_group_public
 group_at = conf.sparkapi_group_at
 fnotice = conf.sparkapi_fnotice
 setpreset_clear = conf.sparkapi_setpreset_clear
 
@@ -58,19 +56,21 @@
 sessions = {} # 会话记录
 spname = {} # 选取的prompt
 
 # block:阻止优先级更低的事件继续处理
 # priority:数字越小优先级越高
 # 私聊功能已关闭
 
-sparkhelp = on_command("help",block=True,priority=5,rule = to_me()) # 显示帮助信息
-showpresets = on_command("showpresets",block=True,priority=5,rule = to_me()) # 显示人物预设
-setpreset = on_command("setpreset",block=True,priority=5,rule = to_me()) # 更改人物预设
-clear = on_command("clear",block=True,priority=5,rule = to_me()) # 清空对话
+sparkhelp = on_command(commands["help"],block=True,priority=5,rule = to_me()) # 显示帮助信息
+showpresets = on_command(commands["showpresets"],block=True,priority=5,rule = to_me()) # 显示人物预设
+setpreset = on_command(commands["setpreset"],block=True,priority=5,rule = to_me()) # 更改人物预设
+clear = on_command(commands["clear"],block=True,priority=5,rule = to_me()) # 清空对话
 chat = on_command(command_chat,block=True,priority=priority,rule = to_me()) # 具有上下文的对话
+savesession = on_command(commands["savesession"],block=True,priority=5,rule = to_me()) # 保存对话记录
+loadsession = on_command(commands["loadsession"],block=True,priority=5,rule = to_me()) # 加载对话记录
 
 @chat.handle()
 async def chat_handle_function(event: MessageEvent, msg: Message = CommandArg()):
     if isinstance(event, PrivateMessageEvent) and not private_chat:
         await chat.finish(MS.text("私聊功能已关闭。如有需要，请联系管理员。"))
 
     content = msg.extract_plain_text().strip() # 提取纯文本
@@ -168,14 +168,34 @@
     if session_id in sessions:
         del sessions[session_id]
         del spname[session_id]
         await clear.finish(MS.text("对话已清空"))
     else:
         await clear.finish(MS.text("无对话记录"))
 
+@savesession.handle()
+async def savesession_handle_function(event: MessageEvent):
+    session_id = get_session_id(event)
+    if session_id in sessions:
+        save_session(sessions[session_id], spname[session_id], session_id)
+        await savesession.finish(MS.text("当前对话记录已保存！"))
+    else:
+        await savesession.finish(MS.text("当前无对话记录"))
+
+@loadsession.handle()
+async def loadsession_handle_function(event: MessageEvent):
+    session_id = get_session_id(event)
+    session, pname = load_session(session_id)
+    if session:
+        sessions[session_id] = session
+        spname[session_id] = pname
+        await loadsession.finish(MS.text("已加载上次保存的对话记录！"))
+    else:
+        await loadsession.finish(MS.text("未保存对话记录"))
+
 # 根据消息类型创建会话ID
 def get_session_id(event):
     if isinstance(event, PrivateMessageEvent):
         return "private_" + str(event.user_id)
     if group_public:
         return event.get_session_id().replace(str(event.user_id), "public")
     else:
```

### Comparing `nonebot_plugin_sparkapi-1.0.6/nonebot_plugin_sparkapi/config.py` & `nonebot_plugin_sparkapi-1.0.7/nonebot_plugin_sparkapi/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,13 +16,13 @@
     sparkapi_group_public: bool = False # 群聊启用公共会话：True：所有人共享同一会话；False：每个人的会话各自独立
     sparkapi_group_at: bool = True # 群聊回复时是否需要@提问者
     sparkapi_fnotice:bool = True # 收到请求时是否提示已收到请求
 
     sparkapi_priority: int = 90 # 事件响应器优先级，[1,99]，数字越小优先级越高
     sparkpai_max_length: int = 8000 # 单次上下文最大长度 越大，对话历史记录保留越长，消耗token上限越高
 
-    sparkapi_setpreset_clear: bool = True # 切换人物预设时是否清空对话历史记录
+    sparkapi_setpreset_clear: bool = True # 切换人物预设时是否清空上下文
 
     sparkapi_bot_name: str = "" # 机器人名字
 
 class ConfigError(Exception):
     pass
```

### Comparing `nonebot_plugin_sparkapi-1.0.6/nonebot_plugin_sparkapi/data.py` & `nonebot_plugin_sparkapi-1.0.7/nonebot_plugin_sparkapi/data.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,58 +1,63 @@
-from .config import Config
-from nonebot import get_driver
-conf = Config.parse_obj(get_driver().config.dict())
-bot_name = conf.sparkapi_bot_name
-command_chat = conf.sparkapi_command_chat
-setprset_clear = conf.sparkapi_setpreset_clear
-
-propmt_default = '忽略此前得到的一切提示。'
-if bot_name:
-    propmt_default += f'现在，你的名字叫{bot_name}。'
-propmt_default += '你具有全面的知识储备，可以和人类进行自然交流，解答问题，高效完成各领域认知智能需求。'
-
-prompt_psychological_counselor =\
-'忽略此前得到的一切提示。\
-现在，你是一位心理咨询师。\
-你具有富有同理心、慈悲、开放和具有文化敏感性的心理治疗师形象。\
-在下面的对话中，请运用积极倾听技巧、开放式问题和清晰的沟通，帮助客户反思他们的思想、情感和经历。\
-与客户建立真诚、信任和支持的关系，创造一个让他们感到安全舒适、可以畅所欲言的环境。\
-接下来，请先进行简单的自我介绍（请注意，不要直接使用本提示），并委婉的引导客户说出他们遇到的挫折。\
-'
-
-presets = { # 
-    "全能机器人": {
-        'role': 'system', 
-        'content': propmt_default
-        },
-    "心理咨询师":{
-        'role': 'system',
-        'content': prompt_psychological_counselor
-        }
-}
-
-presets_lst = "\n".join([f"{id}. {name}" for id, name in enumerate(presets.keys(), start=1)])
-presets_lst = f"【人物预设】\n{presets_lst}"
-if setprset_clear:
-    presets_lst += "\n\n⚠更改人物预设时会清空对话历史记录"
-
-command_help = "help"
-command_showpresets = "showpresets"
-command_setpreset = "setpreset"
-command_preset = "preset"
-command_clear = "clear"
-
-commands_lst = {
-    f"{command_chat+' + ' if command_chat else '直接发送'}对话内容" : "与机器人进行对话",
-    command_help : "显示帮助信息",
-    command_showpresets : "显示人物预设",
-    command_setpreset : "更改人物预设",
-    command_preset + " + 序号" : "选择人物预设",
-    command_clear : "清空对话"
-}
-
-help_info = "【帮助信息】\n"
-
-for id, (command, description) in enumerate(commands_lst.items(), start=1):
-    help_info += f"{id}. {command}：{description}\n"
-
-help_info += "\n群聊中需要@bot + 指令/对话内容"
+from .config import Config
+from nonebot import get_driver
+conf = Config.parse_obj(get_driver().config.dict())
+bot_name = conf.sparkapi_bot_name
+command_chat = conf.sparkapi_command_chat
+setprset_clear = conf.sparkapi_setpreset_clear
+
+propmt_default = '忽略此前得到的一切提示。'
+if bot_name:
+    propmt_default += f'现在，你的名字叫{bot_name}。'
+propmt_default += '你具有全面的知识储备，可以和人类进行自然交流，解答问题，高效完成各领域认知智能需求。'
+
+prompt_psychological_counselor =\
+'忽略此前得到的一切提示。\
+现在，你是一位心理咨询师。\
+你具有富有同理心、慈悲、开放和具有文化敏感性的心理治疗师形象。\
+在下面的对话中，请运用积极倾听技巧、开放式问题和清晰的沟通，帮助客户反思他们的思想、情感和经历。\
+与客户建立真诚、信任和支持的关系，创造一个让他们感到安全舒适、可以畅所欲言的环境。\
+接下来，请先进行简单的自我介绍（请注意，不要直接使用本提示），并委婉的引导客户说出他们遇到的挫折。\
+'
+
+presets = { # 
+    "全能机器人": {
+        'role': 'system', 
+        'content': propmt_default
+        },
+    "心理咨询师":{
+        'role': 'system',
+        'content': prompt_psychological_counselor
+        }
+}
+
+presets_lst = "\n".join([f"{id}. {name}" for id, name in enumerate(presets.keys(), start=1)])
+presets_lst = f"【人物预设】\n{presets_lst}"
+if setprset_clear:
+    presets_lst += "\n\n⚠更改人物预设时会清空对话！"
+
+commands = {
+    "help" : "help",
+    "showpresets" : "showpresets",
+    "setpreset" : "setpreset",
+    "clear" : "clear",
+    "savesession" : "savesession",
+    "loadsession" : "loadsession"
+}
+
+commands_lst = {
+    f"{command_chat+' + ' if command_chat else '直接发送'}对话内容" : "与机器人进行对话",
+    commands["help"] : "显示帮助信息",
+    commands["showpresets"] : "显示人物预设",
+    commands["setpreset"] : "更改人物预设",
+    f"{commands['setpreset']} + 序号" : "选择人物预设",
+    commands["savesession"] : "保存当前对话记录",
+    commands["loadsession"] : "加载上次保存的对话记录",
+    commands["clear"] : "清除对话"
+}
+
+help_info = "【帮助信息】\n"
+
+for id, (command, description) in enumerate(commands_lst.items(), start=1):
+    help_info += f"{id}. {command}：{description}\n"
+
+help_info += "\n群聊中需要@bot + 指令/对话内容"
```

### Comparing `nonebot_plugin_sparkapi-1.0.6/nonebot_plugin_sparkapi.egg-info/PKG-INFO` & `nonebot_plugin_sparkapi-1.0.7/nonebot_plugin_sparkapi.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,159 +1,163 @@
-Metadata-Version: 2.1
-Name: nonebot_plugin_sparkapi
-Version: 1.0.6
-Summary: Nonebot2 ChatBot that calls the official API of the iflyrec Spark LLM for all model versions, defaulting to the current latest (v3.5)
-Author-email: CCLMSY <2502408581@qq.com>
-License: MIT License
-        
-        Copyright (c) 2024 CCLMSY
-        
-        Permission is hereby granted, free of charge, to any person obtaining a copy
-        of this software and associated documentation files (the "Software"), to deal
-        in the Software without restriction, including without limitation the rights
-        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-        copies of the Software, and to permit persons to whom the Software is
-        furnished to do so, subject to the following conditions:
-        
-        The above copyright notice and this permission notice shall be included in all
-        copies or substantial portions of the Software.
-        
-        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-        SOFTWARE.
-        
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: nonebot-adapter-onebot<3.0.0,>=2.2.1
-Requires-Dist: nonebot2<3.0.0,>=2.0.0rc3
-Requires-Dist: websocket-client<2.0.0,>=1.6.1
-
-<div align="center">
-  <a href="https://v2.nonebot.dev/store"><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/nbp_logo.png" width="180" height="180" alt="NoneBotPluginLogo"></a>
-  <br>
-  <p><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/NoneBotPlugin.svg" width="240" alt="NoneBotPluginText"></p>
-</div>
-
-<div align="center">
-
-# nonebot-plugin-sparkapi
-
-_✨ 科大讯飞星火大语言模型官方API聊天机器人 ✨_
-
-<a href="./LICENSE">
-    <img src="https://img.shields.io/github/license/CCLMSY/nonebot-plugin-sparkapi.svg" alt="license">
-</a>
-<a href="https://pypi.python.org/pypi/nonebot-plugin-sparkapi">
-    <img src="https://img.shields.io/pypi/v/nonebot-plugin-sparkapi.svg" alt="pypi">
-</a>
-<img src="https://img.shields.io/badge/python-3.8+-blue.svg" alt="python">
-
-</div>
-
-## 📖 介绍
-
-基于Nonebot2平台，调用科大讯飞星火大语言模型官方API的AI聊天机器人插件
-
-适用于所有模型版本（默认当前最新（v3.5）），支持上下文关联、人物预设等功能
-
-### 💬 功能
-- [x] 支持AI对话
-- [x] 支持上下文关联记忆（可设置记忆文本长度）
-- [x] 用户鉴别（每个用户的历史记录独立）
-- [x] 支持使用、切换人物预设（prompt）
-- [x] 人物预设菜单自动生成，更改无需重写
-- [x] 功能菜单自动生成，更改无需重写
-- [x] 完善的配置项（有其他需求请发issue）
-- [ ] 实用功能列表（查天气、查快递等）
-- [ ] 用户权限与功能区分（超级用户、普通用户）
-- [ ] 支持星火助手API
-- [ ] 支持用户自定义、更改预设
-- [ ] 基于pickle的历史记录持久化
-
-### 📦 项目地址
-- Github：https://github.com/CCLMSY/nonebot-plugin-sparkapi 
-- 觉得好用的话，请给个 Star⭐️ 谢谢喵~ 
-
-## 💿 安装
-
-<details open>
-<summary>使用 nb-cli 安装</summary>
-在 nonebot2 项目的根目录下打开命令行, 输入以下指令即可安装
-
-    nb plugin install nonebot-plugin-sparkapi
-
-</details>
-
-<details>
-<summary>使用包管理器安装</summary>
-在 nonebot2 项目的插件目录下, 打开命令行, 根据你使用的包管理器, 输入相应的安装命令
-
-<details>
-<summary>pip</summary>
-
-    pip install nonebot-plugin-sparkapi
-</details>
-<details>
-<summary>pdm</summary>
-
-    pdm add nonebot-plugin-sparkapi
-</details>
-<details>
-<summary>poetry</summary>
-
-    poetry add nonebot-plugin-sparkapi
-</details>
-<details>
-<summary>conda</summary>
-
-    conda install nonebot-plugin-sparkapi
-</details>
-
-打开 nonebot2 项目根目录下的 `pyproject.toml` 文件, 在 `[tool.nonebot]` 部分追加写入
-
-    plugins = ["nonebot_plugin_sparkapi"]
-
-</details>
-
-## ⚙️ 配置
-
-在 nonebot2 项目的`.env`文件中添加下表中的必填配置
-
-其中，服务接口认证信息 app_id, api_secret, api_key 请前往 [讯飞开放平台控制台](https://console.xfyun.cn/) 获取
-
-| 配置项 | 必填 | 默认值 | 说明 |
-|:-----:|:----:|:----:|:----:|
-| sparkapi_app_id | 是 | "" | APPID |
-| sparkapi_api_secret | 是 | "" | APISecret |
-| sparkapi_api_key | 是 | "" | APIKey |
-| sparkapi_model_version | 否 | "" | 星火大模型的版本，默认为当前最新。<br>可选值：v3.5, v3.0, v2.0, v1.5 |
-| sparkapi_model_top_k | 否 | 4 | 平衡生成文本的质量和多样性。<br>较小的 k 值会减少随机性，使得输出更加稳定；<br>而较大的 k 值会增加随机性，产生更多新颖的输出。<br>取值范围[1, 6] |
-| sparkapi_model_temperature | 否 | 0.5 | 控制结果随机性，取值越高随机性越强，即相同的问题得到的不同答案的可能性越高。<br>取值范围 (0，1] |
-| sparkapi_command_chat | 否 | "" | 机器人对话指令，默认为空可直接对话<br>（需要同时在`.env`中配置命令起始字符为空<br>COMMAND_START = [""]） |
-| sparkapi_private_chat | 否 | True | 是否允许私聊使用 |
-| sparkapi_group_public | 否 | False | 群聊启用公共会话<br>True：所有人共享同一会话<br>False：每个人的会话各自独立 |
-| sparkapi_group_at | 否 | True | 群聊回复消息时是否需要@提问者 |
-| sparkapi_fnotice | 否 | True | 收到请求时是否提示“已收到请求” |
-| sparkapi_priority | 否 | 90 | 事件响应器优先级，[1,99]，数字越小优先级越高 |
-| sparkpai_max_length | 否 | 8000 | 上下文最大长度，[1,8000]<br>单次发送和回复的消息不能超过该项的一半 |
-| sparkapi_setpreset_clear | 否 | True | 切换人物预设时是否清空对话历史记录 |
-| sparkapi_bot_name | 否 | "" | 机器人的名字 |
-
-
-## 🎉 使用
-### 指令表
-| 指令 | 需要@ | 范围 | 说明 |
-|:-----:|:----:|:----:|:----:|
-| sparkapi_command_chat（若不为空） + 对话内容 | 是 | 私聊/群聊 | 与机器人进行对话 |
-| help | 是 | 私聊/群聊 | 查看帮助信息 |
-| showpresets | 是 | 私聊/群聊 | 查看当前可选的人物预设 |
-| setpreset | 是 | 私聊/群聊 | 查看当前可选的人物预设<br>回复编号以进行切换<br> |
-| setpreset + 人物预设编号 | 是 | 私聊/群聊 | 切换到编号对应的人物预设 |
-| clear | 是 | 私聊/群聊 | 清除当前对话上下文 |
-
-### 效果图
-![demo](https://github.com/CCLMSY/nonebot-plugin-sparkapi/blob/resources/demo.jpg)
+Metadata-Version: 2.1
+Name: nonebot_plugin_sparkapi
+Version: 1.0.7
+Summary: Nonebot2 ChatBot that calls the official API of the iflyrec Spark LLM for all model versions, defaulting to the current latest (v3.5)
+Author-email: CCLMSY <2502408581@qq.com>
+License: MIT License
+        
+        Copyright (c) 2024 CCLMSY
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all
+        copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+        SOFTWARE.
+        
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: nonebot-adapter-onebot<3.0.0,>=2.2.1
+Requires-Dist: nonebot2<3.0.0,>=2.0.0rc3
+Requires-Dist: websocket-client<2.0.0,>=1.6.1
+
+<div align="center">
+  <a href="https://v2.nonebot.dev/store"><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/nbp_logo.png" width="180" height="180" alt="NoneBotPluginLogo"></a>
+  <br>
+  <p><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/NoneBotPlugin.svg" width="240" alt="NoneBotPluginText"></p>
+</div>
+
+<div align="center">
+
+# nonebot-plugin-sparkapi
+
+_✨ 科大讯飞星火大语言模型官方API聊天机器人 ✨_
+
+<a href="./LICENSE">
+    <img src="https://img.shields.io/github/license/CCLMSY/nonebot-plugin-sparkapi.svg" alt="license">
+</a>
+<a href="https://pypi.python.org/pypi/nonebot-plugin-sparkapi">
+    <img src="https://img.shields.io/pypi/v/nonebot-plugin-sparkapi.svg" alt="pypi">
+</a>
+<img src="https://img.shields.io/badge/python-3.8+-blue.svg" alt="python">
+
+</div>
+
+## 📖 介绍
+
+基于Nonebot2平台，调用科大讯飞星火大语言模型官方API的AI聊天机器人插件
+
+适用于所有模型版本（默认当前最新（v3.5）），支持上下文关联、人物预设等功能
+
+### 💬 功能
+- [x] 支持AI对话
+- [x] 支持上下文关联记忆（可设置记忆文本长度）
+- [x] 用户鉴别（每个用户的历史记录独立）
+- [x] 支持使用、切换人物预设（prompt）
+- [x] 人物预设菜单自动生成，更改无需重写
+- [x] 功能菜单自动生成，更改无需重写
+- [x] 完善的配置项（有其他需求请发issue）
+- [x] 历史记录持久化
+- [ ] 实用功能列表（查天气、查快递等）
+- [ ] 用户权限与功能区分（超级用户、普通用户）
+- [ ] 支持星火助手API
+- [ ] 支持用户自定义、更改预设
+
+### 📦 项目地址
+- Github：https://github.com/CCLMSY/nonebot-plugin-sparkapi 
+- 觉得好用的话，请给个 Star⭐️ 谢谢喵~ 
+
+## 💿 安装
+
+<details open>
+<summary>使用 nb-cli 安装</summary>
+在 nonebot2 项目的根目录下打开命令行, 输入以下指令即可安装
+
+    nb plugin install nonebot-plugin-sparkapi
+
+</details>
+
+<details>
+<summary>使用包管理器安装</summary>
+在 nonebot2 项目的插件目录下, 打开命令行, 根据你使用的包管理器, 输入相应的安装命令
+
+<details>
+<summary>pip</summary>
+
+    pip install nonebot-plugin-sparkapi
+</details>
+<details>
+<summary>pdm</summary>
+
+    pdm add nonebot-plugin-sparkapi
+</details>
+<details>
+<summary>poetry</summary>
+
+    poetry add nonebot-plugin-sparkapi
+</details>
+<details>
+<summary>conda</summary>
+
+    conda install nonebot-plugin-sparkapi
+</details>
+
+打开 nonebot2 项目根目录下的 `pyproject.toml` 文件, 在 `[tool.nonebot]` 部分追加写入
+
+    plugins = ["nonebot_plugin_sparkapi"]
+
+</details>
+
+## ⚙️ 配置
+
+在 nonebot2 项目的`.env`文件中添加下表中的必填配置
+
+其中，服务接口认证信息 app_id, api_secret, api_key 请前往 [讯飞开放平台控制台](https://console.xfyun.cn/) 获取
+
+| 配置项 | 必填 | 默认值 | 说明 |
+|:-----:|:----:|:----:|:----:|
+| sparkapi_app_id | 是 | "" | APPID |
+| sparkapi_api_secret | 是 | "" | APISecret |
+| sparkapi_api_key | 是 | "" | APIKey |
+| sparkapi_model_version | 否 | "" | 星火大模型的版本，默认为当前最新。<br>可选值：v3.5, v3.0, v2.0, v1.5 |
+| sparkapi_model_top_k | 否 | 4 | 平衡生成文本的质量和多样性。<br>较小的 k 值会减少随机性，使得输出更加稳定；<br>而较大的 k 值会增加随机性，产生更多新颖的输出。<br>取值范围[1, 6] |
+| sparkapi_model_temperature | 否 | 0.5 | 控制结果随机性，取值越高随机性越强，即相同的问题得到的不同答案的可能性越高。<br>取值范围 (0，1] |
+| sparkapi_command_chat | 否 | "" | 机器人对话指令，默认为空可直接对话<br>（需要同时在`.env`中配置命令起始字符为空<br>COMMAND_START = [""]） |
+| sparkapi_private_chat | 否 | True | 是否允许私聊使用 |
+| sparkapi_group_public | 否 | False | 群聊启用公共会话<br>True：所有人共享同一会话<br>False：每个人的会话各自独立 |
+| sparkapi_group_at | 否 | True | 群聊回复消息时是否需要@提问者 |
+| sparkapi_fnotice | 否 | True | 收到请求时是否提示“已收到请求” |
+| sparkapi_priority | 否 | 90 | 事件响应器优先级，[1,99]，数字越小优先级越高 |
+| sparkpai_max_length | 否 | 8000 | 上下文最大长度，[1,8000]<br>单次发送和回复的消息不能超过该项的一半 |
+| sparkapi_setpreset_clear | 否 | True | 切换人物预设时是否清除当前对话上下文 |
+| sparkapi_bot_name | 否 | "" | 机器人的名字 |
+
+
+## 🎉 使用
+### 指令表
+所有指令均可在data.py中修改，且无需重写菜单/指令生成函数
+
+| 指令 | 需要@ | 范围 | 说明 |
+|:-----:|:----:|:----:|:----:|
+| sparkapi_command_chat（若不为空） + 对话内容 | 是 | 私聊/群聊 | 与机器人进行对话 |
+| help | 是 | 私聊/群聊 | 查看帮助信息 |
+| showpresets | 是 | 私聊/群聊 | 查看当前可选的人物预设 |
+| setpreset | 是 | 私聊/群聊 | 查看当前可选的人物预设<br>回复编号以进行切换<br> |
+| setpreset + 人物预设编号 | 是 | 私聊/群聊 | 切换到编号对应的人物预设 |
+| savesession | 是 | 私聊/群聊 | 保存当前对话上下文 |
+| loadsession | 是 | 私聊/群聊 | 加载之前保存的对话上下文 |
+| clear | 是 | 私聊/群聊 | 清除当前对话上下文 |
+
+### 效果图
+![demo](https://github.com/CCLMSY/nonebot-plugin-sparkapi/blob/resources/demo.jpg)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot_plugin_sparkapi Version: 1.0.6 Summary:
+Metadata-Version: 2.1 Name: nonebot_plugin_sparkapi Version: 1.0.7 Summary:
 Nonebot2 ChatBot that calls the official API of the iflyrec Spark LLM for all
 model versions, defaulting to the current latest (v3.5) Author-email: CCLMSY
 <2502408581@qq.com> License: MIT License Copyright (c) 2024 CCLMSY Permission
 is hereby granted, free of charge, to any person obtaining a copy of this
 software and associated documentation files (the "Software"), to deal in the
 Software without restriction, including without limitation the rights to use,
 copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the
@@ -29,29 +29,29 @@
 éç¨äºæææ¨¡åçæ¬ï¼é»è®¤å½åææ°ï¼v3.5ï¼ï¼ï¼æ¯æä¸ä¸æå³èãäººç©é¢è®¾ç­åè½
 ### ð¬ åè½ - [x] æ¯æAIå¯¹è¯ - [x]
 æ¯æä¸ä¸æå³èè®°å¿ï¼å¯è®¾ç½®è®°å¿ææ¬é¿åº¦ï¼ - [x]
 ç¨æ·é´å«ï¼æ¯ä¸ªç¨æ·çåå²è®°å½ç¬ç«ï¼ - [x]
 æ¯æä½¿ç¨ãåæ¢äººç©é¢è®¾ï¼promptï¼ - [x]
 äººç©é¢è®¾èåèªå¨çæï¼æ´æ¹æ ééå - [x]
 åè½èåèªå¨çæï¼æ´æ¹æ ééå - [x]
-å®åçéç½®é¡¹ï¼æå¶ä»éæ±è¯·åissueï¼ - [ ]
-å®ç¨åè½åè¡¨ï¼æ¥å¤©æ°ãæ¥å¿«éç­ï¼ - [ ]
+å®åçéç½®é¡¹ï¼æå¶ä»éæ±è¯·åissueï¼ - [x] åå²è®°å½æä¹å
+- [ ] å®ç¨åè½åè¡¨ï¼æ¥å¤©æ°ãæ¥å¿«éç­ï¼ - [ ]
 ç¨æ·æéä¸åè½åºåï¼è¶çº§ç¨æ·ãæ®éç¨æ·ï¼ - [ ]
-æ¯ææç«å©æAPI - [ ] æ¯æç¨æ·èªå®ä¹ãæ´æ¹é¢è®¾ - [ ]
-åºäºpickleçåå²è®°å½æä¹å ### ð¦ é¡¹ç®å°å - Githubï¼https://
-github.com/CCLMSY/nonebot-plugin-sparkapi - è§å¾å¥½ç¨çè¯ï¼è¯·ç»ä¸ª
-Starâ­ï¸ è°¢è°¢åµ~ ## ð¿ å®è£ ä½¿ç¨ nb-cli å®è£ å¨ nonebot2
-é¡¹ç®çæ ¹ç®å½ä¸æå¼å½ä»¤è¡, è¾å¥ä»¥ä¸æä»¤å³å¯å®è£ nb plugin
-install nonebot-plugin-sparkapi ä½¿ç¨åç®¡çå¨å®è£ å¨ nonebot2
-é¡¹ç®çæä»¶ç®å½ä¸, æå¼å½ä»¤è¡, æ ¹æ®ä½ ä½¿ç¨çåç®¡çå¨,
-è¾å¥ç¸åºçå®è£å½ä»¤ pip pip install nonebot-plugin-sparkapi pdm pdm add
-nonebot-plugin-sparkapi poetry poetry add nonebot-plugin-sparkapi conda conda
-install nonebot-plugin-sparkapi æå¼ nonebot2 é¡¹ç®æ ¹ç®å½ä¸ç
-`pyproject.toml` æä»¶, å¨ `[tool.nonebot]` é¨åè¿½å åå¥ plugins =
-["nonebot_plugin_sparkapi"] ## âï¸ éç½® å¨ nonebot2
+æ¯ææç«å©æAPI - [ ] æ¯æç¨æ·èªå®ä¹ãæ´æ¹é¢è®¾ ### ð¦
+é¡¹ç®å°å - Githubï¼https://github.com/CCLMSY/nonebot-plugin-sparkapi -
+è§å¾å¥½ç¨çè¯ï¼è¯·ç»ä¸ª Starâ­ï¸ è°¢è°¢åµ~ ## ð¿ å®è£ ä½¿ç¨ nb-
+cli å®è£ å¨ nonebot2 é¡¹ç®çæ ¹ç®å½ä¸æå¼å½ä»¤è¡,
+è¾å¥ä»¥ä¸æä»¤å³å¯å®è£ nb plugin install nonebot-plugin-sparkapi
+ä½¿ç¨åç®¡çå¨å®è£ å¨ nonebot2 é¡¹ç®çæä»¶ç®å½ä¸,
+æå¼å½ä»¤è¡, æ ¹æ®ä½ ä½¿ç¨çåç®¡çå¨, è¾å¥ç¸åºçå®è£å½ä»¤
+pip pip install nonebot-plugin-sparkapi pdm pdm add nonebot-plugin-sparkapi
+poetry poetry add nonebot-plugin-sparkapi conda conda install nonebot-plugin-
+sparkapi æå¼ nonebot2 é¡¹ç®æ ¹ç®å½ä¸ç `pyproject.toml` æä»¶, å¨ `
+[tool.nonebot]` é¨åè¿½å åå¥ plugins = ["nonebot_plugin_sparkapi"] ##
+âï¸ éç½® å¨ nonebot2
 é¡¹ç®ç`.env`æä»¶ä¸­æ·»å ä¸è¡¨ä¸­çå¿å¡«éç½®
 å¶ä¸­ï¼æå¡æ¥å£è®¤è¯ä¿¡æ¯ app_id, api_secret, api_key è¯·åå¾
 [è®¯é£å¼æ¾å¹³å°æ§å¶å°](https://console.xfyun.cn/) è·å | éç½®é¡¹ |
 å¿å¡« | é»è®¤å¼ | è¯´æ | |:-----:|:----:|:----:|:----:| | sparkapi_app_id
 | æ¯ | "" | APPID | | sparkapi_api_secret | æ¯ | "" | APISecret | |
 sparkapi_api_key | æ¯ | "" | APIKey | | sparkapi_model_version | å¦ | "" |
 æç«å¤§æ¨¡åççæ¬ï¼é»è®¤ä¸ºå½åææ°ã
@@ -71,19 +71,23 @@
 Falseï¼æ¯ä¸ªäººçä¼è¯åèªç¬ç« | | sparkapi_group_at | å¦ | True |
 ç¾¤èåå¤æ¶æ¯æ¶æ¯å¦éè¦@æé®è | | sparkapi_fnotice | å¦ | True |
 æ¶å°è¯·æ±æ¶æ¯å¦æç¤ºâå·²æ¶å°è¯·æ±â | | sparkapi_priority | å¦ |
 90 | äºä»¶ååºå¨ä¼åçº§ï¼[1,99]ï¼æ°å­è¶å°ä¼åçº§è¶é« | |
 sparkpai_max_length | å¦ | 8000 | ä¸ä¸ææå¤§é¿åº¦ï¼[1,8000]
 åæ¬¡åéååå¤çæ¶æ¯ä¸è½è¶è¿è¯¥é¡¹çä¸å | |
 sparkapi_setpreset_clear | å¦ | True |
-åæ¢äººç©é¢è®¾æ¶æ¯å¦æ¸ç©ºå¯¹è¯åå²è®°å½ | | sparkapi_bot_name | å¦
-| "" | æºå¨äººçåå­ | ## ð ä½¿ç¨ ### æä»¤è¡¨ | æä»¤ | éè¦@ |
-èå´ | è¯´æ | |:-----:|:----:|:----:|:----:| |
-sparkapi_command_chatï¼è¥ä¸ä¸ºç©ºï¼ + å¯¹è¯åå®¹ | æ¯ | ç§è/ç¾¤è |
-ä¸æºå¨äººè¿è¡å¯¹è¯ | | help | æ¯ | ç§è/ç¾¤è | æ¥çå¸®å©ä¿¡æ¯ |
-| showpresets | æ¯ | ç§è/ç¾¤è | æ¥çå½åå¯éçäººç©é¢è®¾ | |
-setpreset | æ¯ | ç§è/ç¾¤è | æ¥çå½åå¯éçäººç©é¢è®¾
+åæ¢äººç©é¢è®¾æ¶æ¯å¦æ¸é¤å½åå¯¹è¯ä¸ä¸æ | | sparkapi_bot_name |
+å¦ | "" | æºå¨äººçåå­ | ## ð ä½¿ç¨ ### æä»¤è¡¨
+æææä»¤åå¯å¨data.pyä¸­ä¿®æ¹ï¼ä¸æ ééåèå/
+æä»¤çæå½æ° | æä»¤ | éè¦@ | èå´ | è¯´æ | |:-----:|:----:|:---
+-:|:----:| | sparkapi_command_chatï¼è¥ä¸ä¸ºç©ºï¼ + å¯¹è¯åå®¹ | æ¯ |
+ç§è/ç¾¤è | ä¸æºå¨äººè¿è¡å¯¹è¯ | | help | æ¯ | ç§è/ç¾¤è |
+æ¥çå¸®å©ä¿¡æ¯ | | showpresets | æ¯ | ç§è/ç¾¤è |
+æ¥çå½åå¯éçäººç©é¢è®¾ | | setpreset | æ¯ | ç§è/ç¾¤è |
+æ¥çå½åå¯éçäººç©é¢è®¾
 åå¤ç¼å·ä»¥è¿è¡åæ¢
 | | setpreset + äººç©é¢è®¾ç¼å· | æ¯ | ç§è/ç¾¤è |
-åæ¢å°ç¼å·å¯¹åºçäººç©é¢è®¾ | | clear | æ¯ | ç§è/ç¾¤è |
+åæ¢å°ç¼å·å¯¹åºçäººç©é¢è®¾ | | savesession | æ¯ | ç§è/ç¾¤è |
+ä¿å­å½åå¯¹è¯ä¸ä¸æ | | loadsession | æ¯ | ç§è/ç¾¤è |
+å è½½ä¹åä¿å­çå¯¹è¯ä¸ä¸æ | | clear | æ¯ | ç§è/ç¾¤è |
 æ¸é¤å½åå¯¹è¯ä¸ä¸æ | ### ææå¾ ![demo](https://github.com/CCLMSY/
 nonebot-plugin-sparkapi/blob/resources/demo.jpg)
```

