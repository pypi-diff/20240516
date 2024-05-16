# Comparing `tmp/nonebot_plugin_sparkapi-1.0.8.tar.gz` & `tmp/nonebot_plugin_sparkapi-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_sparkapi-1.0.8.tar", last modified: Thu May 16 05:50:41 2024, max compression
+gzip compressed data, was "nonebot_plugin_sparkapi-1.0.9.tar", last modified: Thu May 16 06:14:45 2024, max compression
```

## Comparing `nonebot_plugin_sparkapi-1.0.8.tar` & `nonebot_plugin_sparkapi-1.0.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 05:50:41.729854 nonebot_plugin_sparkapi-1.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-16 05:50:36.000000 nonebot_plugin_sparkapi-1.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7264 2024-05-16 05:50:41.729854 nonebot_plugin_sparkapi-1.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5555 2024-05-16 05:50:36.000000 nonebot_plugin_sparkapi-1.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 05:50:41.725854 nonebot_plugin_sparkapi-1.0.8/nonebot_plugin_sparkapi/
--rw-r--r--   0 runner    (1001) docker     (127)     4373 2024-05-16 05:50:36.000000 nonebot_plugin_sparkapi-1.0.8/nonebot_plugin_sparkapi/SparkApi.py
--rw-r--r--   0 runner    (1001) docker     (127)     8416 2024-05-16 05:50:36.000000 nonebot_plugin_sparkapi-1.0.8/nonebot_plugin_sparkapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1725 2024-05-16 05:50:36.000000 nonebot_plugin_sparkapi-1.0.8/nonebot_plugin_sparkapi/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2526 2024-05-16 05:50:36.000000 nonebot_plugin_sparkapi-1.0.8/nonebot_plugin_sparkapi/data.py
--rw-r--r--   0 runner    (1001) docker     (127)     2444 2024-05-16 05:50:36.000000 nonebot_plugin_sparkapi-1.0.8/nonebot_plugin_sparkapi/funcs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 05:50:41.729854 nonebot_plugin_sparkapi-1.0.8/nonebot_plugin_sparkapi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7264 2024-05-16 05:50:41.000000 nonebot_plugin_sparkapi-1.0.8/nonebot_plugin_sparkapi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      437 2024-05-16 05:50:41.000000 nonebot_plugin_sparkapi-1.0.8/nonebot_plugin_sparkapi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 05:50:41.000000 nonebot_plugin_sparkapi-1.0.8/nonebot_plugin_sparkapi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-16 05:50:41.000000 nonebot_plugin_sparkapi-1.0.8/nonebot_plugin_sparkapi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-16 05:50:41.000000 nonebot_plugin_sparkapi-1.0.8/nonebot_plugin_sparkapi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      626 2024-05-16 05:50:36.000000 nonebot_plugin_sparkapi-1.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 05:50:41.729854 nonebot_plugin_sparkapi-1.0.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 06:14:45.123940 nonebot_plugin_sparkapi-1.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-16 06:14:34.000000 nonebot_plugin_sparkapi-1.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7264 2024-05-16 06:14:45.123940 nonebot_plugin_sparkapi-1.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5555 2024-05-16 06:14:34.000000 nonebot_plugin_sparkapi-1.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 06:14:45.119940 nonebot_plugin_sparkapi-1.0.9/nonebot_plugin_sparkapi/
+-rw-r--r--   0 runner    (1001) docker     (127)     4373 2024-05-16 06:14:34.000000 nonebot_plugin_sparkapi-1.0.9/nonebot_plugin_sparkapi/SparkApi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8423 2024-05-16 06:14:34.000000 nonebot_plugin_sparkapi-1.0.9/nonebot_plugin_sparkapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1725 2024-05-16 06:14:34.000000 nonebot_plugin_sparkapi-1.0.9/nonebot_plugin_sparkapi/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2526 2024-05-16 06:14:34.000000 nonebot_plugin_sparkapi-1.0.9/nonebot_plugin_sparkapi/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2444 2024-05-16 06:14:34.000000 nonebot_plugin_sparkapi-1.0.9/nonebot_plugin_sparkapi/funcs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 06:14:45.123940 nonebot_plugin_sparkapi-1.0.9/nonebot_plugin_sparkapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7264 2024-05-16 06:14:45.000000 nonebot_plugin_sparkapi-1.0.9/nonebot_plugin_sparkapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-05-16 06:14:45.000000 nonebot_plugin_sparkapi-1.0.9/nonebot_plugin_sparkapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 06:14:45.000000 nonebot_plugin_sparkapi-1.0.9/nonebot_plugin_sparkapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-16 06:14:45.000000 nonebot_plugin_sparkapi-1.0.9/nonebot_plugin_sparkapi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-16 06:14:45.000000 nonebot_plugin_sparkapi-1.0.9/nonebot_plugin_sparkapi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      626 2024-05-16 06:14:34.000000 nonebot_plugin_sparkapi-1.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 06:14:45.123940 nonebot_plugin_sparkapi-1.0.9/setup.cfg
```

### Comparing `nonebot_plugin_sparkapi-1.0.8/LICENSE` & `nonebot_plugin_sparkapi-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_sparkapi-1.0.8/PKG-INFO` & `nonebot_plugin_sparkapi-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot_plugin_sparkapi
-Version: 1.0.8
+Version: 1.0.9
 Summary: Nonebot2 ChatBot that calls the official API of the iflyrec Spark LLM for all model versions, defaulting to the current latest (v3.5)
 Author-email: CCLMSY <2502408581@qq.com>
 License: MIT License
         
         Copyright (c) 2024 CCLMSY
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot_plugin_sparkapi Version: 1.0.8 Summary:
+Metadata-Version: 2.1 Name: nonebot_plugin_sparkapi Version: 1.0.9 Summary:
 Nonebot2 ChatBot that calls the official API of the iflyrec Spark LLM for all
 model versions, defaulting to the current latest (v3.5) Author-email: CCLMSY
 <2502408581@qq.com> License: MIT License Copyright (c) 2024 CCLMSY Permission
 is hereby granted, free of charge, to any person obtaining a copy of this
 software and associated documentation files (the "Software"), to deal in the
 Software without restriction, including without limitation the rights to use,
 copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the
```

### Comparing `nonebot_plugin_sparkapi-1.0.8/README.md` & `nonebot_plugin_sparkapi-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_sparkapi-1.0.8/nonebot_plugin_sparkapi/SparkApi.py` & `nonebot_plugin_sparkapi-1.0.9/nonebot_plugin_sparkapi/SparkApi.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_sparkapi-1.0.8/nonebot_plugin_sparkapi/__init__.py` & `nonebot_plugin_sparkapi-1.0.9/nonebot_plugin_sparkapi/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -188,30 +188,31 @@
     if session:
         sessions[session_id] = session
         spname[session_id] = pname
         await loadsession.finish(MS.text("已加载上次保存的对话记录！"))
     else:
         await loadsession.finish(MS.text("未保存对话记录"))
 
-# 根据消息类型创建会话ID
-def get_session_id(event):
-    if isinstance(event, PrivateMessageEvent):
-        return "private_" + str(event.user_id)
-    if group_public:
-        return event.get_session_id().replace(str(event.user_id), "public")
-    else:
-        return event.get_session_id()
 
-def request(history, sid, pname):
+async def request(history, sid, pname):
     history = deepcopy(history)
     history.insert(0, presets[pname])
     history = checklen(history)
     print(history)
     SparkApi.answer = ""
     SparkApi.main(appid,api_key,api_secret,Spark_url,domain,history,sid)
     ans = SparkApi.answer
     return ans
 
+# 根据消息类型创建会话ID
+def get_session_id(event):
+    if isinstance(event, PrivateMessageEvent):
+        return "private_" + str(event.user_id)
+    if group_public:
+        return event.get_session_id().replace(str(event.user_id), "public")
+    else:
+        return event.get_session_id()
+
 def checklen(text): # 检查对话长度
     while (getlength(text) > max_length):
         del text[0]
     return text
```

### Comparing `nonebot_plugin_sparkapi-1.0.8/nonebot_plugin_sparkapi/config.py` & `nonebot_plugin_sparkapi-1.0.9/nonebot_plugin_sparkapi/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_sparkapi-1.0.8/nonebot_plugin_sparkapi/data.py` & `nonebot_plugin_sparkapi-1.0.9/nonebot_plugin_sparkapi/data.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_sparkapi-1.0.8/nonebot_plugin_sparkapi/funcs.py` & `nonebot_plugin_sparkapi-1.0.9/nonebot_plugin_sparkapi/funcs.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_sparkapi-1.0.8/nonebot_plugin_sparkapi.egg-info/PKG-INFO` & `nonebot_plugin_sparkapi-1.0.9/nonebot_plugin_sparkapi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot_plugin_sparkapi
-Version: 1.0.8
+Version: 1.0.9
 Summary: Nonebot2 ChatBot that calls the official API of the iflyrec Spark LLM for all model versions, defaulting to the current latest (v3.5)
 Author-email: CCLMSY <2502408581@qq.com>
 License: MIT License
         
         Copyright (c) 2024 CCLMSY
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot_plugin_sparkapi Version: 1.0.8 Summary:
+Metadata-Version: 2.1 Name: nonebot_plugin_sparkapi Version: 1.0.9 Summary:
 Nonebot2 ChatBot that calls the official API of the iflyrec Spark LLM for all
 model versions, defaulting to the current latest (v3.5) Author-email: CCLMSY
 <2502408581@qq.com> License: MIT License Copyright (c) 2024 CCLMSY Permission
 is hereby granted, free of charge, to any person obtaining a copy of this
 software and associated documentation files (the "Software"), to deal in the
 Software without restriction, including without limitation the rights to use,
 copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the
```

### Comparing `nonebot_plugin_sparkapi-1.0.8/pyproject.toml` & `nonebot_plugin_sparkapi-1.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "nonebot_plugin_sparkapi"
-version = "1.0.8"
+version = "1.0.9"
 description = "Nonebot2 ChatBot that calls the official API of the iflyrec Spark LLM for all model versions, defaulting to the current latest (v3.5)"
 authors = [
     { name = "CCLMSY", email = "2502408581@qq.com" }
 ]
 dependencies = [
     "nonebot-adapter-onebot >=2.2.1, <3.0.0",
     "nonebot2 >=2.0.0rc3, <3.0.0",
```

