# Comparing `tmp/xtn-tools-pro-1.0.0.1.4.tar.gz` & `tmp/xtn-tools-pro-1.0.0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\xtn-tools-pro-1.0.0.1.4.tar", last modified: Wed May 15 09:14:45 2024, max compression
+gzip compressed data, was "dist\xtn-tools-pro-1.0.0.1.5.tar", last modified: Wed May 15 09:20:39 2024, max compression
```

## Comparing `xtn-tools-pro-1.0.0.1.4.tar` & `xtn-tools-pro-1.0.0.1.5.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0        0        0        0 2024-05-15 09:14:45.000000 xtn-tools-pro-1.0.0.1.4/
--rw-rw-rw-   0        0        0        0 2024-04-17 03:27:01.000000 xtn-tools-pro-1.0.0.1.4/LICENSE
--rw-rw-rw-   0        0        0      287 2024-05-15 09:14:45.000000 xtn-tools-pro-1.0.0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0       11 2024-04-17 03:28:15.000000 xtn-tools-pro-1.0.0.1.4/README.md
--rw-rw-rw-   0        0        0       42 2024-05-15 09:14:45.000000 xtn-tools-pro-1.0.0.1.4/setup.cfg
--rw-rw-rw-   0        0        0     1271 2024-05-15 09:14:37.000000 xtn-tools-pro-1.0.0.1.4/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-15 09:14:45.000000 xtn-tools-pro-1.0.0.1.4/xtn_tools_pro/
--rw-rw-rw-   0        0        0      395 2024-04-18 05:24:09.000000 xtn-tools-pro-1.0.0.1.4/xtn_tools_pro/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-15 09:14:45.000000 xtn-tools-pro-1.0.0.1.4/xtn_tools_pro/db/
--rw-rw-rw-   0        0        0     5573 2024-05-12 16:30:30.000000 xtn-tools-pro-1.0.0.1.4/xtn_tools_pro/db/MongoDB.py
--rw-rw-rw-   0        0        0    13373 2024-05-12 14:20:54.000000 xtn-tools-pro-1.0.0.1.4/xtn_tools_pro/db/MysqlDB.py
--rw-rw-rw-   0        0        0     6053 2024-04-27 07:30:36.000000 xtn-tools-pro-1.0.0.1.4/xtn_tools_pro/db/RedisDB.py
--rw-rw-rw-   0        0        0      416 2024-04-18 05:40:27.000000 xtn-tools-pro-1.0.0.1.4/xtn_tools_pro/db/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-15 09:14:45.000000 xtn-tools-pro-1.0.0.1.4/xtn_tools_pro/proxy/
--rw-rw-rw-   0        0        0    10964 2024-05-15 09:14:14.000000 xtn-tools-pro-1.0.0.1.4/xtn_tools_pro/proxy/XiaoXiangProxy.py
--rw-rw-rw-   0        0        0      418 2024-04-27 04:18:50.000000 xtn-tools-pro-1.0.0.1.4/xtn_tools_pro/proxy/__init__.py
--rw-rw-rw-   0        0        0     8703 2024-05-13 14:02:38.000000 xtn-tools-pro-1.0.0.1.4/xtn_tools_pro/proxy/proxy.py
--rw-rw-rw-   0        0        0      542 2024-05-12 16:30:30.000000 xtn-tools-pro-1.0.0.1.4/xtn_tools_pro/tools.py
-drwxrwxrwx   0        0        0        0 2024-05-15 09:14:45.000000 xtn-tools-pro-1.0.0.1.4/xtn_tools_pro/utils/
--rw-rw-rw-   0        0        0      418 2024-05-12 04:02:30.000000 xtn-tools-pro-1.0.0.1.4/xtn_tools_pro/utils/__init__.py
--rw-rw-rw-   0        0        0     3190 2024-05-15 08:10:00.000000 xtn-tools-pro-1.0.0.1.4/xtn_tools_pro/utils/crypto.py
--rw-rw-rw-   0        0        0     1509 2024-05-12 16:32:12.000000 xtn-tools-pro-1.0.0.1.4/xtn_tools_pro/utils/file_utils.py
--rw-rw-rw-   0        0        0     3773 2024-05-15 07:34:46.000000 xtn-tools-pro-1.0.0.1.4/xtn_tools_pro/utils/helpers.py
--rw-rw-rw-   0        0        0     8139 2024-05-12 16:32:03.000000 xtn-tools-pro-1.0.0.1.4/xtn_tools_pro/utils/log.py
--rw-rw-rw-   0        0        0     1657 2024-05-12 12:05:16.000000 xtn-tools-pro-1.0.0.1.4/xtn_tools_pro/utils/retry.py
--rw-rw-rw-   0        0        0     6263 2024-05-12 16:30:30.000000 xtn-tools-pro-1.0.0.1.4/xtn_tools_pro/utils/sql.py
--rw-rw-rw-   0        0        0     4859 2024-05-12 16:32:03.000000 xtn-tools-pro-1.0.0.1.4/xtn_tools_pro/utils/time_utils.py
-drwxrwxrwx   0        0        0        0 2024-05-15 09:14:45.000000 xtn-tools-pro-1.0.0.1.4/xtn_tools_pro.egg-info/
--rw-rw-rw-   0        0        0      287 2024-05-15 09:14:45.000000 xtn-tools-pro-1.0.0.1.4/xtn_tools_pro.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      715 2024-05-15 09:14:45.000000 xtn-tools-pro-1.0.0.1.4/xtn_tools_pro.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-15 09:14:45.000000 xtn-tools-pro-1.0.0.1.4/xtn_tools_pro.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2024-05-15 09:14:45.000000 xtn-tools-pro-1.0.0.1.4/xtn_tools_pro.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-05-15 09:14:45.000000 xtn-tools-pro-1.0.0.1.4/xtn_tools_pro.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-15 09:20:39.000000 xtn-tools-pro-1.0.0.1.5/
+-rw-rw-rw-   0        0        0        0 2024-04-17 03:27:01.000000 xtn-tools-pro-1.0.0.1.5/LICENSE
+-rw-rw-rw-   0        0        0      287 2024-05-15 09:20:39.000000 xtn-tools-pro-1.0.0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0       11 2024-04-17 03:28:15.000000 xtn-tools-pro-1.0.0.1.5/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-15 09:20:39.000000 xtn-tools-pro-1.0.0.1.5/setup.cfg
+-rw-rw-rw-   0        0        0     1271 2024-05-15 09:20:30.000000 xtn-tools-pro-1.0.0.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-15 09:20:39.000000 xtn-tools-pro-1.0.0.1.5/xtn_tools_pro/
+-rw-rw-rw-   0        0        0      395 2024-04-18 05:24:09.000000 xtn-tools-pro-1.0.0.1.5/xtn_tools_pro/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-15 09:20:39.000000 xtn-tools-pro-1.0.0.1.5/xtn_tools_pro/db/
+-rw-rw-rw-   0        0        0     5573 2024-05-12 16:30:30.000000 xtn-tools-pro-1.0.0.1.5/xtn_tools_pro/db/MongoDB.py
+-rw-rw-rw-   0        0        0    13373 2024-05-12 14:20:54.000000 xtn-tools-pro-1.0.0.1.5/xtn_tools_pro/db/MysqlDB.py
+-rw-rw-rw-   0        0        0     6053 2024-04-27 07:30:36.000000 xtn-tools-pro-1.0.0.1.5/xtn_tools_pro/db/RedisDB.py
+-rw-rw-rw-   0        0        0      416 2024-04-18 05:40:27.000000 xtn-tools-pro-1.0.0.1.5/xtn_tools_pro/db/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-15 09:20:39.000000 xtn-tools-pro-1.0.0.1.5/xtn_tools_pro/proxy/
+-rw-rw-rw-   0        0        0    10969 2024-05-15 09:20:30.000000 xtn-tools-pro-1.0.0.1.5/xtn_tools_pro/proxy/XiaoXiangProxy.py
+-rw-rw-rw-   0        0        0      418 2024-04-27 04:18:50.000000 xtn-tools-pro-1.0.0.1.5/xtn_tools_pro/proxy/__init__.py
+-rw-rw-rw-   0        0        0     8703 2024-05-13 14:02:38.000000 xtn-tools-pro-1.0.0.1.5/xtn_tools_pro/proxy/proxy.py
+-rw-rw-rw-   0        0        0      542 2024-05-12 16:30:30.000000 xtn-tools-pro-1.0.0.1.5/xtn_tools_pro/tools.py
+drwxrwxrwx   0        0        0        0 2024-05-15 09:20:39.000000 xtn-tools-pro-1.0.0.1.5/xtn_tools_pro/utils/
+-rw-rw-rw-   0        0        0      418 2024-05-12 04:02:30.000000 xtn-tools-pro-1.0.0.1.5/xtn_tools_pro/utils/__init__.py
+-rw-rw-rw-   0        0        0     3190 2024-05-15 08:10:00.000000 xtn-tools-pro-1.0.0.1.5/xtn_tools_pro/utils/crypto.py
+-rw-rw-rw-   0        0        0     1509 2024-05-12 16:32:12.000000 xtn-tools-pro-1.0.0.1.5/xtn_tools_pro/utils/file_utils.py
+-rw-rw-rw-   0        0        0     3773 2024-05-15 07:34:46.000000 xtn-tools-pro-1.0.0.1.5/xtn_tools_pro/utils/helpers.py
+-rw-rw-rw-   0        0        0     8139 2024-05-12 16:32:03.000000 xtn-tools-pro-1.0.0.1.5/xtn_tools_pro/utils/log.py
+-rw-rw-rw-   0        0        0     1657 2024-05-12 12:05:16.000000 xtn-tools-pro-1.0.0.1.5/xtn_tools_pro/utils/retry.py
+-rw-rw-rw-   0        0        0     6263 2024-05-12 16:30:30.000000 xtn-tools-pro-1.0.0.1.5/xtn_tools_pro/utils/sql.py
+-rw-rw-rw-   0        0        0     4859 2024-05-12 16:32:03.000000 xtn-tools-pro-1.0.0.1.5/xtn_tools_pro/utils/time_utils.py
+drwxrwxrwx   0        0        0        0 2024-05-15 09:20:39.000000 xtn-tools-pro-1.0.0.1.5/xtn_tools_pro.egg-info/
+-rw-rw-rw-   0        0        0      287 2024-05-15 09:20:39.000000 xtn-tools-pro-1.0.0.1.5/xtn_tools_pro.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      715 2024-05-15 09:20:39.000000 xtn-tools-pro-1.0.0.1.5/xtn_tools_pro.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-15 09:20:39.000000 xtn-tools-pro-1.0.0.1.5/xtn_tools_pro.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2024-05-15 09:20:39.000000 xtn-tools-pro-1.0.0.1.5/xtn_tools_pro.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-05-15 09:20:39.000000 xtn-tools-pro-1.0.0.1.5/xtn_tools_pro.egg-info/top_level.txt
```

### Comparing `xtn-tools-pro-1.0.0.1.4/setup.py` & `xtn-tools-pro-1.0.0.1.5/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 import setuptools
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setuptools.setup(
     name="xtn-tools-pro",  # 模块名称
-    version="1.0.0.1.4",  # 版本
+    version="1.0.0.1.5",  # 版本
     author="xtn",  # 作者
     author_email="czw011122@163.com",  # 作者邮箱
     description="xtn 开发工具",  # 模块简介
     long_description=long_description,  # 模块详细介绍
     long_description_content_type="text/markdown",  # 模块详细介绍格式
     packages=setuptools.find_packages(),  # 自动找到项目中导入的模块
     # 模块相关的元数据(更多描述信息)
```

### Comparing `xtn-tools-pro-1.0.0.1.4/xtn_tools_pro/db/MongoDB.py` & `xtn-tools-pro-1.0.0.1.5/xtn_tools_pro/db/MongoDB.py`

 * *Files identical despite different names*

### Comparing `xtn-tools-pro-1.0.0.1.4/xtn_tools_pro/db/MysqlDB.py` & `xtn-tools-pro-1.0.0.1.5/xtn_tools_pro/db/MysqlDB.py`

 * *Files identical despite different names*

### Comparing `xtn-tools-pro-1.0.0.1.4/xtn_tools_pro/db/RedisDB.py` & `xtn-tools-pro-1.0.0.1.5/xtn_tools_pro/db/RedisDB.py`

 * *Files identical despite different names*

### Comparing `xtn-tools-pro-1.0.0.1.4/xtn_tools_pro/proxy/XiaoXiangProxy.py` & `xtn-tools-pro-1.0.0.1.5/xtn_tools_pro/proxy/XiaoXiangProxy.py`

 * *Files 0% similar despite different names*

```diff
@@ -70,15 +70,15 @@
         :return:
         """
         proxy_val_list = list(self.__redis_pool.get_all_key("{}*".format(self.__redisProxyName)))
         for proxy_val in proxy_val_list:
             # 获取时间
             time_out = proxy_val.split(":")[-1]
             # 获取使用次数
-            proxy_val_count = self.__redis_pool.get(proxy_val)
+            proxy_val_count = int(self.__redis_pool.get(proxy_val))
             if int(time_out) + self.__usage_time < get_time_now_timestamp(is_time_10=True):
                 del_state = self.__redis_pool.delete(proxy_val)
                 self.__log(
                     "当前代理状态:{proxy_val},{time_out}_{py_time}当前代理已超过使用时间,删除状态为：{del_state}".
                         format(proxy_val=proxy_val, del_state=del_state,
                                time_out=time_out, py_time=get_time_now_timestamp(is_time_10=True)))
             elif int(proxy_val_count) >= self.__usage_cnt:
```

### Comparing `xtn-tools-pro-1.0.0.1.4/xtn_tools_pro/proxy/proxy.py` & `xtn-tools-pro-1.0.0.1.5/xtn_tools_pro/proxy/proxy.py`

 * *Files identical despite different names*

### Comparing `xtn-tools-pro-1.0.0.1.4/xtn_tools_pro/tools.py` & `xtn-tools-pro-1.0.0.1.5/xtn_tools_pro/tools.py`

 * *Files identical despite different names*

### Comparing `xtn-tools-pro-1.0.0.1.4/xtn_tools_pro/utils/crypto.py` & `xtn-tools-pro-1.0.0.1.5/xtn_tools_pro/utils/crypto.py`

 * *Files identical despite different names*

### Comparing `xtn-tools-pro-1.0.0.1.4/xtn_tools_pro/utils/file_utils.py` & `xtn-tools-pro-1.0.0.1.5/xtn_tools_pro/utils/file_utils.py`

 * *Files identical despite different names*

### Comparing `xtn-tools-pro-1.0.0.1.4/xtn_tools_pro/utils/helpers.py` & `xtn-tools-pro-1.0.0.1.5/xtn_tools_pro/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `xtn-tools-pro-1.0.0.1.4/xtn_tools_pro/utils/log.py` & `xtn-tools-pro-1.0.0.1.5/xtn_tools_pro/utils/log.py`

 * *Files identical despite different names*

### Comparing `xtn-tools-pro-1.0.0.1.4/xtn_tools_pro/utils/retry.py` & `xtn-tools-pro-1.0.0.1.5/xtn_tools_pro/utils/retry.py`

 * *Files identical despite different names*

### Comparing `xtn-tools-pro-1.0.0.1.4/xtn_tools_pro/utils/sql.py` & `xtn-tools-pro-1.0.0.1.5/xtn_tools_pro/utils/sql.py`

 * *Files identical despite different names*

### Comparing `xtn-tools-pro-1.0.0.1.4/xtn_tools_pro/utils/time_utils.py` & `xtn-tools-pro-1.0.0.1.5/xtn_tools_pro/utils/time_utils.py`

 * *Files identical despite different names*

### Comparing `xtn-tools-pro-1.0.0.1.4/xtn_tools_pro.egg-info/SOURCES.txt` & `xtn-tools-pro-1.0.0.1.5/xtn_tools_pro.egg-info/SOURCES.txt`

 * *Files identical despite different names*

