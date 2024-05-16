# Comparing `tmp/nonebot_plugin_sparkapi-1.0.4.tar.gz` & `tmp/nonebot_plugin_sparkapi-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_sparkapi-1.0.4.tar", last modified: Wed May 15 13:55:26 2024, max compression
+gzip compressed data, was "nonebot_plugin_sparkapi-1.0.5.tar", last modified: Wed May 15 14:34:09 2024, max compression
```

## Comparing `nonebot_plugin_sparkapi-1.0.4.tar` & `nonebot_plugin_sparkapi-1.0.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:55:26.063082 nonebot_plugin_sparkapi-1.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-15 13:55:19.000000 nonebot_plugin_sparkapi-1.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6340 2024-05-15 13:55:26.063082 nonebot_plugin_sparkapi-1.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4623 2024-05-15 13:55:19.000000 nonebot_plugin_sparkapi-1.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:55:26.059082 nonebot_plugin_sparkapi-1.0.4/nonebot_plugin_sparkapi/
--rw-r--r--   0 runner    (1001) docker     (127)     4253 2024-05-15 13:55:19.000000 nonebot_plugin_sparkapi-1.0.4/nonebot_plugin_sparkapi/SparkApi.py
--rw-r--r--   0 runner    (1001) docker     (127)     7224 2024-05-15 13:55:19.000000 nonebot_plugin_sparkapi-1.0.4/nonebot_plugin_sparkapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-05-15 13:55:19.000000 nonebot_plugin_sparkapi-1.0.4/nonebot_plugin_sparkapi/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1946 2024-05-15 13:55:19.000000 nonebot_plugin_sparkapi-1.0.4/nonebot_plugin_sparkapi/data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1677 2024-05-15 13:55:19.000000 nonebot_plugin_sparkapi-1.0.4/nonebot_plugin_sparkapi/funcs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 13:55:26.063082 nonebot_plugin_sparkapi-1.0.4/nonebot_plugin_sparkapi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6340 2024-05-15 13:55:26.000000 nonebot_plugin_sparkapi-1.0.4/nonebot_plugin_sparkapi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      437 2024-05-15 13:55:26.000000 nonebot_plugin_sparkapi-1.0.4/nonebot_plugin_sparkapi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 13:55:26.000000 nonebot_plugin_sparkapi-1.0.4/nonebot_plugin_sparkapi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-15 13:55:26.000000 nonebot_plugin_sparkapi-1.0.4/nonebot_plugin_sparkapi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-15 13:55:26.000000 nonebot_plugin_sparkapi-1.0.4/nonebot_plugin_sparkapi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      633 2024-05-15 13:55:19.000000 nonebot_plugin_sparkapi-1.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 13:55:26.063082 nonebot_plugin_sparkapi-1.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:34:09.585964 nonebot_plugin_sparkapi-1.0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-15 14:34:05.000000 nonebot_plugin_sparkapi-1.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6340 2024-05-15 14:34:09.585964 nonebot_plugin_sparkapi-1.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4623 2024-05-15 14:34:05.000000 nonebot_plugin_sparkapi-1.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:34:09.585964 nonebot_plugin_sparkapi-1.0.5/nonebot_plugin_sparkapi/
+-rw-r--r--   0 runner    (1001) docker     (127)     4253 2024-05-15 14:34:05.000000 nonebot_plugin_sparkapi-1.0.5/nonebot_plugin_sparkapi/SparkApi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7228 2024-05-15 14:34:05.000000 nonebot_plugin_sparkapi-1.0.5/nonebot_plugin_sparkapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-05-15 14:34:05.000000 nonebot_plugin_sparkapi-1.0.5/nonebot_plugin_sparkapi/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1946 2024-05-15 14:34:05.000000 nonebot_plugin_sparkapi-1.0.5/nonebot_plugin_sparkapi/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1677 2024-05-15 14:34:05.000000 nonebot_plugin_sparkapi-1.0.5/nonebot_plugin_sparkapi/funcs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:34:09.585964 nonebot_plugin_sparkapi-1.0.5/nonebot_plugin_sparkapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6340 2024-05-15 14:34:09.000000 nonebot_plugin_sparkapi-1.0.5/nonebot_plugin_sparkapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-05-15 14:34:09.000000 nonebot_plugin_sparkapi-1.0.5/nonebot_plugin_sparkapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 14:34:09.000000 nonebot_plugin_sparkapi-1.0.5/nonebot_plugin_sparkapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-15 14:34:09.000000 nonebot_plugin_sparkapi-1.0.5/nonebot_plugin_sparkapi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-15 14:34:09.000000 nonebot_plugin_sparkapi-1.0.5/nonebot_plugin_sparkapi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-15 14:34:05.000000 nonebot_plugin_sparkapi-1.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 14:34:09.585964 nonebot_plugin_sparkapi-1.0.5/setup.cfg
```

### Comparing `nonebot_plugin_sparkapi-1.0.4/LICENSE` & `nonebot_plugin_sparkapi-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_sparkapi-1.0.4/PKG-INFO` & `nonebot_plugin_sparkapi-1.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot_plugin_sparkapi
-Version: 1.0.4
+Version: 1.0.5
 Summary: Nonebot2 ChatBot that calls the official API of the iflyrec Spark LLM for all model versions, defaulting to the current latest (v3.5)
 Author-email: CCLMSY <2502408581@qq.com>
 License: MIT License
         
         Copyright (c) 2024 CCLMSY
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -24,16 +24,16 @@
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: nonebot2<3.0.0,>=2.0.0rc3
 Requires-Dist: nonebot-adapter-onebot<3.0.0,>=2.2.1
+Requires-Dist: nonebot2<3.0.0,>=2.0.0rc3
 Requires-Dist: websocket-client<2.0.0,>=1.6.1
 
 <div align="center">
   <a href="https://v2.nonebot.dev/store"><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/nbp_logo.png" width="180" height="180" alt="NoneBotPluginLogo"></a>
   <br>
   <p><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/NoneBotPlugin.svg" width="240" alt="NoneBotPluginText"></p>
 </div>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot_plugin_sparkapi Version: 1.0.4 Summary:
+Metadata-Version: 2.1 Name: nonebot_plugin_sparkapi Version: 1.0.5 Summary:
 Nonebot2 ChatBot that calls the official API of the iflyrec Spark LLM for all
 model versions, defaulting to the current latest (v3.5) Author-email: CCLMSY
 <2502408581@qq.com> License: MIT License Copyright (c) 2024 CCLMSY Permission
 is hereby granted, free of charge, to any person obtaining a copy of this
 software and associated documentation files (the "Software"), to deal in the
 Software without restriction, including without limitation the rights to use,
 copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the
@@ -12,17 +12,17 @@
 the Software. THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
 EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
 MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO
 EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES
 OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE,
 ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 DEALINGS IN THE SOFTWARE. Requires-Python: >=3.8 Description-Content-Type:
-text/markdown License-File: LICENSE Requires-Dist: nonebot2<3.0.0,>=2.0.0rc3
-Requires-Dist: nonebot-adapter-onebot<3.0.0,>=2.2.1 Requires-Dist: websocket-
-client<2.0.0,>=1.6.1
+text/markdown License-File: LICENSE Requires-Dist: nonebot-adapter-
+onebot<3.0.0,>=2.2.1 Requires-Dist: nonebot2<3.0.0,>=2.0.0rc3 Requires-Dist:
+websocket-client<2.0.0,>=1.6.1
                               _[_N_o_n_e_B_o_t_P_l_u_g_i_n_L_o_g_o_]
                               [NoneBotPluginText]
                         # nonebot-plugin-sparkapi _â¨
  ç§å¤§è®¯é£æç«å¤§è¯­è¨æ¨¡åå®æ¹APIèå¤©æºå¨äºº â¨__[_l_i_c_e_n_s_e_]_[_p_y_p_i_]
                                    [python]
 ## ð ä»ç»
 åºäºNonebot2å¹³å°ï¼è°ç¨ç§å¤§è®¯é£æç«å¤§è¯­è¨æ¨¡åå®æ¹APIçAIèå¤©æºå¨äººæä»¶
```

### Comparing `nonebot_plugin_sparkapi-1.0.4/README.md` & `nonebot_plugin_sparkapi-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_sparkapi-1.0.4/nonebot_plugin_sparkapi/SparkApi.py` & `nonebot_plugin_sparkapi-1.0.5/nonebot_plugin_sparkapi/SparkApi.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_sparkapi-1.0.4/nonebot_plugin_sparkapi/__init__.py` & `nonebot_plugin_sparkapi-1.0.5/nonebot_plugin_sparkapi/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,32 +16,32 @@
 from .data import presets, presets_lst, help_info
 
 __plugin_meta__ = PluginMetadata(
     name="科大讯飞星火大语言模型官方API聊天机器人插件",
     description="调用科大讯飞星火大语言模型官方API的聊天机器人插件，适用于所有模型版本（默认当前最新（v3.5）），支持上下文关联、人物预设",
     usage=help_info,
     type='application',
-    homepage="https://github.com/CCLMSY/nonebot_plugin_sparkapi",
+    homepage="https://github.com/CCLMSY/nonebot-plugin-sparkapi",
     config=Config,
     supported_adapters={"~onebot.v11"},
     extra = {
         "author": "CCLMSY",
-        "version": "1.0.0"
+        "version": "1.0.5"
     }
 )
 
 # 获取插件配置（由于gocqhttp使用pydantic==1.10.13，因此沿用老方法）
 conf = Config.parse_obj(nonebot.get_driver().config.dict())
 
 appid = conf.sparkapi_app_id
 api_secret = conf.sparkapi_api_secret
 api_key = conf.sparkapi_api_key
 
-if not appid or not api_secret or not api_key:
-    raise ConfigError("请设置API信息,可前往 https://console.xfyun.cn/ 获取")
+# if not appid or not api_secret or not api_key:
+#     raise ConfigError("请设置API信息,可前往 https://console.xfyun.cn/ 获取")
 
 model_version = funcs.unify_model_version(conf.sparkapi_model_version)
 Spark_url = funcs.get_Spark_url(model_version)
 domain = funcs.get_domain(model_version)
 
 command = conf.sparkapi_command
 private_chat = conf.sparkapi_private_chat
```

### Comparing `nonebot_plugin_sparkapi-1.0.4/nonebot_plugin_sparkapi/config.py` & `nonebot_plugin_sparkapi-1.0.5/nonebot_plugin_sparkapi/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_sparkapi-1.0.4/nonebot_plugin_sparkapi/data.py` & `nonebot_plugin_sparkapi-1.0.5/nonebot_plugin_sparkapi/data.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_sparkapi-1.0.4/nonebot_plugin_sparkapi/funcs.py` & `nonebot_plugin_sparkapi-1.0.5/nonebot_plugin_sparkapi/funcs.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_sparkapi-1.0.4/nonebot_plugin_sparkapi.egg-info/PKG-INFO` & `nonebot_plugin_sparkapi-1.0.5/nonebot_plugin_sparkapi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot_plugin_sparkapi
-Version: 1.0.4
+Version: 1.0.5
 Summary: Nonebot2 ChatBot that calls the official API of the iflyrec Spark LLM for all model versions, defaulting to the current latest (v3.5)
 Author-email: CCLMSY <2502408581@qq.com>
 License: MIT License
         
         Copyright (c) 2024 CCLMSY
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -24,16 +24,16 @@
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: nonebot2<3.0.0,>=2.0.0rc3
 Requires-Dist: nonebot-adapter-onebot<3.0.0,>=2.2.1
+Requires-Dist: nonebot2<3.0.0,>=2.0.0rc3
 Requires-Dist: websocket-client<2.0.0,>=1.6.1
 
 <div align="center">
   <a href="https://v2.nonebot.dev/store"><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/nbp_logo.png" width="180" height="180" alt="NoneBotPluginLogo"></a>
   <br>
   <p><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/NoneBotPlugin.svg" width="240" alt="NoneBotPluginText"></p>
 </div>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot_plugin_sparkapi Version: 1.0.4 Summary:
+Metadata-Version: 2.1 Name: nonebot_plugin_sparkapi Version: 1.0.5 Summary:
 Nonebot2 ChatBot that calls the official API of the iflyrec Spark LLM for all
 model versions, defaulting to the current latest (v3.5) Author-email: CCLMSY
 <2502408581@qq.com> License: MIT License Copyright (c) 2024 CCLMSY Permission
 is hereby granted, free of charge, to any person obtaining a copy of this
 software and associated documentation files (the "Software"), to deal in the
 Software without restriction, including without limitation the rights to use,
 copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the
@@ -12,17 +12,17 @@
 the Software. THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
 EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
 MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO
 EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES
 OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE,
 ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 DEALINGS IN THE SOFTWARE. Requires-Python: >=3.8 Description-Content-Type:
-text/markdown License-File: LICENSE Requires-Dist: nonebot2<3.0.0,>=2.0.0rc3
-Requires-Dist: nonebot-adapter-onebot<3.0.0,>=2.2.1 Requires-Dist: websocket-
-client<2.0.0,>=1.6.1
+text/markdown License-File: LICENSE Requires-Dist: nonebot-adapter-
+onebot<3.0.0,>=2.2.1 Requires-Dist: nonebot2<3.0.0,>=2.0.0rc3 Requires-Dist:
+websocket-client<2.0.0,>=1.6.1
                               _[_N_o_n_e_B_o_t_P_l_u_g_i_n_L_o_g_o_]
                               [NoneBotPluginText]
                         # nonebot-plugin-sparkapi _â¨
  ç§å¤§è®¯é£æç«å¤§è¯­è¨æ¨¡åå®æ¹APIèå¤©æºå¨äºº â¨__[_l_i_c_e_n_s_e_]_[_p_y_p_i_]
                                    [python]
 ## ð ä»ç»
 åºäºNonebot2å¹³å°ï¼è°ç¨ç§å¤§è®¯é£æç«å¤§è¯­è¨æ¨¡åå®æ¹APIçAIèå¤©æºå¨äººæä»¶
```

### Comparing `nonebot_plugin_sparkapi-1.0.4/pyproject.toml` & `nonebot_plugin_sparkapi-1.0.5/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 [project]
 name = "nonebot_plugin_sparkapi"
-version = "1.0.4"
+version = "1.0.5"
 description = "Nonebot2 ChatBot that calls the official API of the iflyrec Spark LLM for all model versions, defaulting to the current latest (v3.5)"
 authors = [
     { name = "CCLMSY", email = "2502408581@qq.com" }
 ]
 dependencies = [
-    "nonebot2 >=2.0.0rc3, <3.0.0",
     "nonebot-adapter-onebot >=2.2.1, <3.0.0",
+    "nonebot2 >=2.0.0rc3, <3.0.0",
     "websocket-client >=1.6.1, <2.0.0"
 ]
 requires-python = ">=3.8"
 license = { file = "LICENSE" }
 readme = { file = "README.md", content-type = "text/markdown" }
 
 [build-system]
 requires = ["setuptools>=42", "wheel"]
 build-backend = "setuptools.build_meta"
+
```

