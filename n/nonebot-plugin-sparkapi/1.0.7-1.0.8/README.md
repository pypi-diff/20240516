# Comparing `tmp/nonebot_plugin_sparkapi-1.0.7.tar.gz` & `tmp/nonebot_plugin_sparkapi-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_sparkapi-1.0.7.tar", last modified: Thu May 16 05:04:51 2024, max compression
+gzip compressed data, was "nonebot_plugin_sparkapi-1.0.8.tar", last modified: Thu May 16 05:50:41 2024, max compression
```

## Comparing `nonebot_plugin_sparkapi-1.0.7.tar` & `nonebot_plugin_sparkapi-1.0.8.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 05:04:51.752089 nonebot_plugin_sparkapi-1.0.7/
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-16 05:04:47.000000 nonebot_plugin_sparkapi-1.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7272 2024-05-16 05:04:51.752089 nonebot_plugin_sparkapi-1.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5555 2024-05-16 05:04:47.000000 nonebot_plugin_sparkapi-1.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 05:04:51.748089 nonebot_plugin_sparkapi-1.0.7/nonebot_plugin_sparkapi/
--rw-r--r--   0 runner    (1001) docker     (127)     4528 2024-05-16 05:04:47.000000 nonebot_plugin_sparkapi-1.0.7/nonebot_plugin_sparkapi/SparkApi.py
--rw-r--r--   0 runner    (1001) docker     (127)     8416 2024-05-16 05:04:47.000000 nonebot_plugin_sparkapi-1.0.7/nonebot_plugin_sparkapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1725 2024-05-16 05:04:47.000000 nonebot_plugin_sparkapi-1.0.7/nonebot_plugin_sparkapi/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2526 2024-05-16 05:04:47.000000 nonebot_plugin_sparkapi-1.0.7/nonebot_plugin_sparkapi/data.py
--rw-r--r--   0 runner    (1001) docker     (127)     2444 2024-05-16 05:04:47.000000 nonebot_plugin_sparkapi-1.0.7/nonebot_plugin_sparkapi/funcs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 05:04:51.752089 nonebot_plugin_sparkapi-1.0.7/nonebot_plugin_sparkapi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7272 2024-05-16 05:04:51.000000 nonebot_plugin_sparkapi-1.0.7/nonebot_plugin_sparkapi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      437 2024-05-16 05:04:51.000000 nonebot_plugin_sparkapi-1.0.7/nonebot_plugin_sparkapi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 05:04:51.000000 nonebot_plugin_sparkapi-1.0.7/nonebot_plugin_sparkapi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-16 05:04:51.000000 nonebot_plugin_sparkapi-1.0.7/nonebot_plugin_sparkapi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-16 05:04:51.000000 nonebot_plugin_sparkapi-1.0.7/nonebot_plugin_sparkapi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-16 05:04:47.000000 nonebot_plugin_sparkapi-1.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 05:04:51.752089 nonebot_plugin_sparkapi-1.0.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 05:50:41.729854 nonebot_plugin_sparkapi-1.0.8/
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-16 05:50:36.000000 nonebot_plugin_sparkapi-1.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7264 2024-05-16 05:50:41.729854 nonebot_plugin_sparkapi-1.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5555 2024-05-16 05:50:36.000000 nonebot_plugin_sparkapi-1.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 05:50:41.725854 nonebot_plugin_sparkapi-1.0.8/nonebot_plugin_sparkapi/
+-rw-r--r--   0 runner    (1001) docker     (127)     4373 2024-05-16 05:50:36.000000 nonebot_plugin_sparkapi-1.0.8/nonebot_plugin_sparkapi/SparkApi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8416 2024-05-16 05:50:36.000000 nonebot_plugin_sparkapi-1.0.8/nonebot_plugin_sparkapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1725 2024-05-16 05:50:36.000000 nonebot_plugin_sparkapi-1.0.8/nonebot_plugin_sparkapi/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2526 2024-05-16 05:50:36.000000 nonebot_plugin_sparkapi-1.0.8/nonebot_plugin_sparkapi/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2444 2024-05-16 05:50:36.000000 nonebot_plugin_sparkapi-1.0.8/nonebot_plugin_sparkapi/funcs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 05:50:41.729854 nonebot_plugin_sparkapi-1.0.8/nonebot_plugin_sparkapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7264 2024-05-16 05:50:41.000000 nonebot_plugin_sparkapi-1.0.8/nonebot_plugin_sparkapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-05-16 05:50:41.000000 nonebot_plugin_sparkapi-1.0.8/nonebot_plugin_sparkapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 05:50:41.000000 nonebot_plugin_sparkapi-1.0.8/nonebot_plugin_sparkapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-16 05:50:41.000000 nonebot_plugin_sparkapi-1.0.8/nonebot_plugin_sparkapi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-16 05:50:41.000000 nonebot_plugin_sparkapi-1.0.8/nonebot_plugin_sparkapi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      626 2024-05-16 05:50:36.000000 nonebot_plugin_sparkapi-1.0.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 05:50:41.729854 nonebot_plugin_sparkapi-1.0.8/setup.cfg
```

### Comparing `nonebot_plugin_sparkapi-1.0.7/LICENSE` & `nonebot_plugin_sparkapi-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_sparkapi-1.0.7/PKG-INFO` & `nonebot_plugin_sparkapi-1.0.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot_plugin_sparkapi
-Version: 1.0.7
+Version: 1.0.8
 Summary: Nonebot2 ChatBot that calls the official API of the iflyrec Spark LLM for all model versions, defaulting to the current latest (v3.5)
 Author-email: CCLMSY <2502408581@qq.com>
 License: MIT License
         
         Copyright (c) 2024 CCLMSY
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -26,15 +26,15 @@
         SOFTWARE.
         
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: nonebot-adapter-onebot<3.0.0,>=2.2.1
 Requires-Dist: nonebot2<3.0.0,>=2.0.0rc3
-Requires-Dist: websocket-client<2.0.0,>=1.6.1
+Requires-Dist: websockets<13.0,>=12.0
 
 <div align="center">
   <a href="https://v2.nonebot.dev/store"><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/nbp_logo.png" width="180" height="180" alt="NoneBotPluginLogo"></a>
   <br>
   <p><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/NoneBotPlugin.svg" width="240" alt="NoneBotPluginText"></p>
 </div>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot_plugin_sparkapi Version: 1.0.7 Summary:
+Metadata-Version: 2.1 Name: nonebot_plugin_sparkapi Version: 1.0.8 Summary:
 Nonebot2 ChatBot that calls the official API of the iflyrec Spark LLM for all
 model versions, defaulting to the current latest (v3.5) Author-email: CCLMSY
 <2502408581@qq.com> License: MIT License Copyright (c) 2024 CCLMSY Permission
 is hereby granted, free of charge, to any person obtaining a copy of this
 software and associated documentation files (the "Software"), to deal in the
 Software without restriction, including without limitation the rights to use,
 copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the
@@ -14,15 +14,15 @@
 MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO
 EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES
 OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE,
 ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 DEALINGS IN THE SOFTWARE. Requires-Python: >=3.8 Description-Content-Type:
 text/markdown License-File: LICENSE Requires-Dist: nonebot-adapter-
 onebot<3.0.0,>=2.2.1 Requires-Dist: nonebot2<3.0.0,>=2.0.0rc3 Requires-Dist:
-websocket-client<2.0.0,>=1.6.1
+websockets<13.0,>=12.0
                               _[_N_o_n_e_B_o_t_P_l_u_g_i_n_L_o_g_o_]
                               [NoneBotPluginText]
                         # nonebot-plugin-sparkapi _â¨
  ç§å¤§è®¯é£æç«å¤§è¯­è¨æ¨¡åå®æ¹APIèå¤©æºå¨äºº â¨__[_l_i_c_e_n_s_e_]_[_p_y_p_i_]
                                    [python]
 ## ð ä»ç»
 åºäºNonebot2å¹³å°ï¼è°ç¨ç§å¤§è®¯é£æç«å¤§è¯­è¨æ¨¡åå®æ¹APIçAIèå¤©æºå¨äººæä»¶
```

### Comparing `nonebot_plugin_sparkapi-1.0.7/README.md` & `nonebot_plugin_sparkapi-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_sparkapi-1.0.7/nonebot_plugin_sparkapi/SparkApi.py` & `nonebot_plugin_sparkapi-1.0.8/nonebot_plugin_sparkapi/SparkApi.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-# type: ignore
+#type:ignore
 from datetime import datetime
 from time import mktime
 from wsgiref.handlers import format_date_time
-from urllib.parse import urlparse
+from urllib.parse import urlparse, urlencode
 
 import hmac
 import hashlib
 import base64
-from urllib.parse import urlencode
 
-import _thread as thread
+import asyncio
 import json
-import websocket
+import websockets
 import ssl
 
 from .config import Config
 from nonebot import get_driver
+
 conf = Config.parse_obj(get_driver().config.dict())
 
 model_top_k = conf.sparkapi_model_top_k
 model_temperature = conf.sparkapi_model_temperature
 max_length = conf.sparkpai_max_length
 
 answer = ""
@@ -65,88 +65,71 @@
         # print("APIKey: " + self.APIKey)
         # print("APISecret: " + self.APISecret)
         # print("signature_origin: " + signature_origin)
         # print(url)
         # 此处打印出建立连接时候的url,参考本demo的时候可取消上方打印的注释，比对相同参数时生成的url与自己代码生成的url是否一致
         return url
 
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
+# 收到websockets消息的处理
+async def on_message(ws, message):
     # print(message)
-    # print(time.time())
     data = json.loads(message)
     code = data['header']['code']
     if code != 0:
         err = f'请求错误: {code}, {data}'
         print(err)
-        ws.close()
+        await ws.close()
     else:
         # global sid
         # sid = data["header"]["sid"]
         choices = data["payload"]["choices"]
         status = choices["status"]
         content = choices["text"][0]["content"]
         # print(content,end ="")
         global answer
         answer += content
         # print(1)
         if status == 2:
-            ws.close()
+            await ws.close()
 
+async def connect_ws(appid, api_key, api_secret, Spark_url, domain, question, sid):
+    wsParam = Ws_Param(appid, api_key, api_secret, Spark_url)
+    ws_url = wsParam.create_url()
+    ssl_context = ssl.SSLContext(ssl.PROTOCOL_TLS_CLIENT)
+    ssl_context.check_hostname = False
+    ssl_context.verify_mode = ssl.CERT_NONE
+
+    async with websockets.connect(ws_url, ssl=ssl_context) as ws:
+        ws.appid = appid
+        ws.question = question
+        ws.domain = domain
+        ws.sid = sid
+        await ws.send(json.dumps(gen_params(appid, domain, question)))
+        async for message in ws:
+            await on_message(ws, message)
 
-def gen_params(appid, domain,question):
-    """
-    通过appid和用户的提问来生成请参数
-    """
+def gen_params(appid, domain, question):
     data = {
         "header": {
             "app_id": appid,
             "uid": "1234"
         },
         "parameter": {
-
             "chat": {
                 "domain": domain,
                 "temperature": model_temperature,
-                "max_tokens": max_length//2,
+                "max_tokens": max_length // 2,
                 "top_k": model_top_k,
-
                 "auditing": "default"
             }
         },
         "payload": {
             "message": {
                 "text": question
             }
         }
     }
     return data
 
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
+def main(appid, api_key, api_secret, Spark_url, domain, question, sid):
+    asyncio.run(connect_ws(appid, api_key, api_secret, Spark_url, domain, question, sid))
+
```

### Comparing `nonebot_plugin_sparkapi-1.0.7/nonebot_plugin_sparkapi/__init__.py` & `nonebot_plugin_sparkapi-1.0.8/nonebot_plugin_sparkapi/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_sparkapi-1.0.7/nonebot_plugin_sparkapi/config.py` & `nonebot_plugin_sparkapi-1.0.8/nonebot_plugin_sparkapi/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_sparkapi-1.0.7/nonebot_plugin_sparkapi/data.py` & `nonebot_plugin_sparkapi-1.0.8/nonebot_plugin_sparkapi/data.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_sparkapi-1.0.7/nonebot_plugin_sparkapi/funcs.py` & `nonebot_plugin_sparkapi-1.0.8/nonebot_plugin_sparkapi/funcs.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_sparkapi-1.0.7/nonebot_plugin_sparkapi.egg-info/PKG-INFO` & `nonebot_plugin_sparkapi-1.0.8/nonebot_plugin_sparkapi.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot_plugin_sparkapi
-Version: 1.0.7
+Version: 1.0.8
 Summary: Nonebot2 ChatBot that calls the official API of the iflyrec Spark LLM for all model versions, defaulting to the current latest (v3.5)
 Author-email: CCLMSY <2502408581@qq.com>
 License: MIT License
         
         Copyright (c) 2024 CCLMSY
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -26,15 +26,15 @@
         SOFTWARE.
         
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: nonebot-adapter-onebot<3.0.0,>=2.2.1
 Requires-Dist: nonebot2<3.0.0,>=2.0.0rc3
-Requires-Dist: websocket-client<2.0.0,>=1.6.1
+Requires-Dist: websockets<13.0,>=12.0
 
 <div align="center">
   <a href="https://v2.nonebot.dev/store"><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/nbp_logo.png" width="180" height="180" alt="NoneBotPluginLogo"></a>
   <br>
   <p><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/NoneBotPlugin.svg" width="240" alt="NoneBotPluginText"></p>
 </div>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot_plugin_sparkapi Version: 1.0.7 Summary:
+Metadata-Version: 2.1 Name: nonebot_plugin_sparkapi Version: 1.0.8 Summary:
 Nonebot2 ChatBot that calls the official API of the iflyrec Spark LLM for all
 model versions, defaulting to the current latest (v3.5) Author-email: CCLMSY
 <2502408581@qq.com> License: MIT License Copyright (c) 2024 CCLMSY Permission
 is hereby granted, free of charge, to any person obtaining a copy of this
 software and associated documentation files (the "Software"), to deal in the
 Software without restriction, including without limitation the rights to use,
 copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the
@@ -14,15 +14,15 @@
 MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO
 EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES
 OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE,
 ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 DEALINGS IN THE SOFTWARE. Requires-Python: >=3.8 Description-Content-Type:
 text/markdown License-File: LICENSE Requires-Dist: nonebot-adapter-
 onebot<3.0.0,>=2.2.1 Requires-Dist: nonebot2<3.0.0,>=2.0.0rc3 Requires-Dist:
-websocket-client<2.0.0,>=1.6.1
+websockets<13.0,>=12.0
                               _[_N_o_n_e_B_o_t_P_l_u_g_i_n_L_o_g_o_]
                               [NoneBotPluginText]
                         # nonebot-plugin-sparkapi _â¨
  ç§å¤§è®¯é£æç«å¤§è¯­è¨æ¨¡åå®æ¹APIèå¤©æºå¨äºº â¨__[_l_i_c_e_n_s_e_]_[_p_y_p_i_]
                                    [python]
 ## ð ä»ç»
 åºäºNonebot2å¹³å°ï¼è°ç¨ç§å¤§è®¯é£æç«å¤§è¯­è¨æ¨¡åå®æ¹APIçAIèå¤©æºå¨äººæä»¶
```

### Comparing `nonebot_plugin_sparkapi-1.0.7/pyproject.toml` & `nonebot_plugin_sparkapi-1.0.8/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [project]
 name = "nonebot_plugin_sparkapi"
-version = "1.0.7"
+version = "1.0.8"
 description = "Nonebot2 ChatBot that calls the official API of the iflyrec Spark LLM for all model versions, defaulting to the current latest (v3.5)"
 authors = [
     { name = "CCLMSY", email = "2502408581@qq.com" }
 ]
 dependencies = [
     "nonebot-adapter-onebot >=2.2.1, <3.0.0",
     "nonebot2 >=2.0.0rc3, <3.0.0",
-    "websocket-client >=1.6.1, <2.0.0"
+    "websockets >=12.0, <13.0"
 ]
 requires-python = ">=3.8"
 license = { file = "LICENSE" }
 readme = { file = "README.md", content-type = "text/markdown" }
 
 [build-system]
 requires = ["setuptools>=42", "wheel"]
```

