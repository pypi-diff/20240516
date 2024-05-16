# Comparing `tmp/xtn-tools-pro-1.0.0.1.5.tar.gz` & `tmp/xtn-tools-pro-1.0.0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\xtn-tools-pro-1.0.0.1.5.tar", last modified: Wed May 15 09:20:39 2024, max compression
+gzip compressed data, was "dist\xtn-tools-pro-1.0.0.1.6.tar", last modified: Wed May 15 23:41:47 2024, max compression
```

## Comparing `xtn-tools-pro-1.0.0.1.5.tar` & `xtn-tools-pro-1.0.0.1.6.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0        0        0        0 2024-05-15 09:20:39.000000 xtn-tools-pro-1.0.0.1.5/
--rw-rw-rw-   0        0        0        0 2024-04-17 03:27:01.000000 xtn-tools-pro-1.0.0.1.5/LICENSE
--rw-rw-rw-   0        0        0      287 2024-05-15 09:20:39.000000 xtn-tools-pro-1.0.0.1.5/PKG-INFO
--rw-rw-rw-   0        0        0       11 2024-04-17 03:28:15.000000 xtn-tools-pro-1.0.0.1.5/README.md
--rw-rw-rw-   0        0        0       42 2024-05-15 09:20:39.000000 xtn-tools-pro-1.0.0.1.5/setup.cfg
--rw-rw-rw-   0        0        0     1271 2024-05-15 09:20:30.000000 xtn-tools-pro-1.0.0.1.5/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-15 09:20:39.000000 xtn-tools-pro-1.0.0.1.5/xtn_tools_pro/
--rw-rw-rw-   0        0        0      395 2024-04-18 05:24:09.000000 xtn-tools-pro-1.0.0.1.5/xtn_tools_pro/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-15 09:20:39.000000 xtn-tools-pro-1.0.0.1.5/xtn_tools_pro/db/
--rw-rw-rw-   0        0        0     5573 2024-05-12 16:30:30.000000 xtn-tools-pro-1.0.0.1.5/xtn_tools_pro/db/MongoDB.py
--rw-rw-rw-   0        0        0    13373 2024-05-12 14:20:54.000000 xtn-tools-pro-1.0.0.1.5/xtn_tools_pro/db/MysqlDB.py
--rw-rw-rw-   0        0        0     6053 2024-04-27 07:30:36.000000 xtn-tools-pro-1.0.0.1.5/xtn_tools_pro/db/RedisDB.py
--rw-rw-rw-   0        0        0      416 2024-04-18 05:40:27.000000 xtn-tools-pro-1.0.0.1.5/xtn_tools_pro/db/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-15 09:20:39.000000 xtn-tools-pro-1.0.0.1.5/xtn_tools_pro/proxy/
--rw-rw-rw-   0        0        0    10969 2024-05-15 09:20:30.000000 xtn-tools-pro-1.0.0.1.5/xtn_tools_pro/proxy/XiaoXiangProxy.py
--rw-rw-rw-   0        0        0      418 2024-04-27 04:18:50.000000 xtn-tools-pro-1.0.0.1.5/xtn_tools_pro/proxy/__init__.py
--rw-rw-rw-   0        0        0     8703 2024-05-13 14:02:38.000000 xtn-tools-pro-1.0.0.1.5/xtn_tools_pro/proxy/proxy.py
--rw-rw-rw-   0        0        0      542 2024-05-12 16:30:30.000000 xtn-tools-pro-1.0.0.1.5/xtn_tools_pro/tools.py
-drwxrwxrwx   0        0        0        0 2024-05-15 09:20:39.000000 xtn-tools-pro-1.0.0.1.5/xtn_tools_pro/utils/
--rw-rw-rw-   0        0        0      418 2024-05-12 04:02:30.000000 xtn-tools-pro-1.0.0.1.5/xtn_tools_pro/utils/__init__.py
--rw-rw-rw-   0        0        0     3190 2024-05-15 08:10:00.000000 xtn-tools-pro-1.0.0.1.5/xtn_tools_pro/utils/crypto.py
--rw-rw-rw-   0        0        0     1509 2024-05-12 16:32:12.000000 xtn-tools-pro-1.0.0.1.5/xtn_tools_pro/utils/file_utils.py
--rw-rw-rw-   0        0        0     3773 2024-05-15 07:34:46.000000 xtn-tools-pro-1.0.0.1.5/xtn_tools_pro/utils/helpers.py
--rw-rw-rw-   0        0        0     8139 2024-05-12 16:32:03.000000 xtn-tools-pro-1.0.0.1.5/xtn_tools_pro/utils/log.py
--rw-rw-rw-   0        0        0     1657 2024-05-12 12:05:16.000000 xtn-tools-pro-1.0.0.1.5/xtn_tools_pro/utils/retry.py
--rw-rw-rw-   0        0        0     6263 2024-05-12 16:30:30.000000 xtn-tools-pro-1.0.0.1.5/xtn_tools_pro/utils/sql.py
--rw-rw-rw-   0        0        0     4859 2024-05-12 16:32:03.000000 xtn-tools-pro-1.0.0.1.5/xtn_tools_pro/utils/time_utils.py
-drwxrwxrwx   0        0        0        0 2024-05-15 09:20:39.000000 xtn-tools-pro-1.0.0.1.5/xtn_tools_pro.egg-info/
--rw-rw-rw-   0        0        0      287 2024-05-15 09:20:39.000000 xtn-tools-pro-1.0.0.1.5/xtn_tools_pro.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      715 2024-05-15 09:20:39.000000 xtn-tools-pro-1.0.0.1.5/xtn_tools_pro.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-15 09:20:39.000000 xtn-tools-pro-1.0.0.1.5/xtn_tools_pro.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2024-05-15 09:20:39.000000 xtn-tools-pro-1.0.0.1.5/xtn_tools_pro.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-05-15 09:20:39.000000 xtn-tools-pro-1.0.0.1.5/xtn_tools_pro.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-15 23:41:47.000000 xtn-tools-pro-1.0.0.1.6/
+-rw-rw-rw-   0        0        0        0 2024-04-17 03:27:01.000000 xtn-tools-pro-1.0.0.1.6/LICENSE
+-rw-rw-rw-   0        0        0      287 2024-05-15 23:41:47.000000 xtn-tools-pro-1.0.0.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0       11 2024-04-17 03:28:15.000000 xtn-tools-pro-1.0.0.1.6/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-15 23:41:47.000000 xtn-tools-pro-1.0.0.1.6/setup.cfg
+-rw-rw-rw-   0        0        0     1289 2024-05-15 23:41:23.000000 xtn-tools-pro-1.0.0.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-15 23:41:47.000000 xtn-tools-pro-1.0.0.1.6/xtn_tools_pro/
+-rw-rw-rw-   0        0        0      395 2024-04-18 05:24:09.000000 xtn-tools-pro-1.0.0.1.6/xtn_tools_pro/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-15 23:41:47.000000 xtn-tools-pro-1.0.0.1.6/xtn_tools_pro/db/
+-rw-rw-rw-   0        0        0     5573 2024-05-12 16:30:30.000000 xtn-tools-pro-1.0.0.1.6/xtn_tools_pro/db/MongoDB.py
+-rw-rw-rw-   0        0        0    13373 2024-05-12 14:20:54.000000 xtn-tools-pro-1.0.0.1.6/xtn_tools_pro/db/MysqlDB.py
+-rw-rw-rw-   0        0        0     6053 2024-04-27 07:30:36.000000 xtn-tools-pro-1.0.0.1.6/xtn_tools_pro/db/RedisDB.py
+-rw-rw-rw-   0        0        0      416 2024-04-18 05:40:27.000000 xtn-tools-pro-1.0.0.1.6/xtn_tools_pro/db/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-15 23:41:47.000000 xtn-tools-pro-1.0.0.1.6/xtn_tools_pro/proxy/
+-rw-rw-rw-   0        0        0    11029 2024-05-15 23:41:23.000000 xtn-tools-pro-1.0.0.1.6/xtn_tools_pro/proxy/XiaoXiangProxy.py
+-rw-rw-rw-   0        0        0      418 2024-04-27 04:18:50.000000 xtn-tools-pro-1.0.0.1.6/xtn_tools_pro/proxy/__init__.py
+-rw-rw-rw-   0        0        0     8703 2024-05-13 14:02:38.000000 xtn-tools-pro-1.0.0.1.6/xtn_tools_pro/proxy/proxy.py
+-rw-rw-rw-   0        0        0      542 2024-05-12 16:30:30.000000 xtn-tools-pro-1.0.0.1.6/xtn_tools_pro/tools.py
+drwxrwxrwx   0        0        0        0 2024-05-15 23:41:47.000000 xtn-tools-pro-1.0.0.1.6/xtn_tools_pro/utils/
+-rw-rw-rw-   0        0        0      418 2024-05-12 04:02:30.000000 xtn-tools-pro-1.0.0.1.6/xtn_tools_pro/utils/__init__.py
+-rw-rw-rw-   0        0        0     3190 2024-05-15 08:10:00.000000 xtn-tools-pro-1.0.0.1.6/xtn_tools_pro/utils/crypto.py
+-rw-rw-rw-   0        0        0     1509 2024-05-12 16:32:12.000000 xtn-tools-pro-1.0.0.1.6/xtn_tools_pro/utils/file_utils.py
+-rw-rw-rw-   0        0        0     3812 2024-05-15 15:46:10.000000 xtn-tools-pro-1.0.0.1.6/xtn_tools_pro/utils/helpers.py
+-rw-rw-rw-   0        0        0     8139 2024-05-12 16:32:03.000000 xtn-tools-pro-1.0.0.1.6/xtn_tools_pro/utils/log.py
+-rw-rw-rw-   0        0        0     1657 2024-05-12 12:05:16.000000 xtn-tools-pro-1.0.0.1.6/xtn_tools_pro/utils/retry.py
+-rw-rw-rw-   0        0        0     6263 2024-05-12 16:30:30.000000 xtn-tools-pro-1.0.0.1.6/xtn_tools_pro/utils/sql.py
+-rw-rw-rw-   0        0        0     4859 2024-05-12 16:32:03.000000 xtn-tools-pro-1.0.0.1.6/xtn_tools_pro/utils/time_utils.py
+drwxrwxrwx   0        0        0        0 2024-05-15 23:41:47.000000 xtn-tools-pro-1.0.0.1.6/xtn_tools_pro.egg-info/
+-rw-rw-rw-   0        0        0      287 2024-05-15 23:41:47.000000 xtn-tools-pro-1.0.0.1.6/xtn_tools_pro.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      715 2024-05-15 23:41:47.000000 xtn-tools-pro-1.0.0.1.6/xtn_tools_pro.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-15 23:41:47.000000 xtn-tools-pro-1.0.0.1.6/xtn_tools_pro.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       54 2024-05-15 23:41:47.000000 xtn-tools-pro-1.0.0.1.6/xtn_tools_pro.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-05-15 23:41:47.000000 xtn-tools-pro-1.0.0.1.6/xtn_tools_pro.egg-info/top_level.txt
```

### Comparing `xtn-tools-pro-1.0.0.1.5/setup.py` & `xtn-tools-pro-1.0.0.1.6/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 import setuptools
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setuptools.setup(
     name="xtn-tools-pro",  # 模块名称
-    version="1.0.0.1.5",  # 版本
+    version="1.0.0.1.6",  # 版本
     author="xtn",  # 作者
     author_email="czw011122@163.com",  # 作者邮箱
     description="xtn 开发工具",  # 模块简介
     long_description=long_description,  # 模块详细介绍
     long_description_content_type="text/markdown",  # 模块详细介绍格式
     packages=setuptools.find_packages(),  # 自动找到项目中导入的模块
     # 模块相关的元数据(更多描述信息)
@@ -29,11 +29,12 @@
     # 依赖模块
     install_requires=[
         "pymongo",
         "redis",
         "pymysql",
         "dbutils",
         "colorlog",
-        "requests"
+        "requests",
+        "Faker"
     ],
     python_requires='>=3',
 )
```

### Comparing `xtn-tools-pro-1.0.0.1.5/xtn_tools_pro/db/MongoDB.py` & `xtn-tools-pro-1.0.0.1.6/xtn_tools_pro/db/MongoDB.py`

 * *Files identical despite different names*

### Comparing `xtn-tools-pro-1.0.0.1.5/xtn_tools_pro/db/MysqlDB.py` & `xtn-tools-pro-1.0.0.1.6/xtn_tools_pro/db/MysqlDB.py`

 * *Files identical despite different names*

### Comparing `xtn-tools-pro-1.0.0.1.5/xtn_tools_pro/db/RedisDB.py` & `xtn-tools-pro-1.0.0.1.6/xtn_tools_pro/db/RedisDB.py`

 * *Files identical despite different names*

### Comparing `xtn-tools-pro-1.0.0.1.5/xtn_tools_pro/proxy/XiaoXiangProxy.py` & `xtn-tools-pro-1.0.0.1.6/xtn_tools_pro/proxy/XiaoXiangProxy.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,14 +51,16 @@
         self.__usage_time = usage_time
 
         # if is_log:
         #     # 日志
         #     nowDate = str(datetime.datetime.now().strftime('%Y_%m_%d'))
         #     logger.add(loggerPath.format(t=nowDate))
 
+        self.bind_ip()
+
     def __log(self, text):
         """
             记录日志
         :param text:
         :return:
         """
         print(text)
@@ -146,20 +148,23 @@
                 else:
                     self.__log("获取小象代理返回响应码不为200，等待2s，{content}".format(content=response.text))
                     time.sleep(2)
                     continue
             except Exception as e:
                 self.__log("获取小象代理报错：{e}".format(e=e))
 
+    def bind_ip(self):
+        # 手动绑定终端IP
+        response = requests.get(url=self.__XiaoXiangAutoBinding, verify=False, timeout=3)
+        self.__log(response.text)
+
     def run(self):
         while True:
             try:
-                # 手动绑定终端IP
-                response = requests.get(url=self.__XiaoXiangAutoBinding, verify=False, timeout=3)
-                self.__log(response.text)
+                self.bind_ip()
                 while True:
                     # 检查代理
                     self.__check_proxy()
                     # 获取小象代理
                     self.__get_api_proxy()
                     time.sleep(1)
                     # 判断时间是否超过当前23:59分时间戳
```

### Comparing `xtn-tools-pro-1.0.0.1.5/xtn_tools_pro/proxy/proxy.py` & `xtn-tools-pro-1.0.0.1.6/xtn_tools_pro/proxy/proxy.py`

 * *Files identical despite different names*

### Comparing `xtn-tools-pro-1.0.0.1.5/xtn_tools_pro/tools.py` & `xtn-tools-pro-1.0.0.1.6/xtn_tools_pro/tools.py`

 * *Files identical despite different names*

### Comparing `xtn-tools-pro-1.0.0.1.5/xtn_tools_pro/utils/crypto.py` & `xtn-tools-pro-1.0.0.1.6/xtn_tools_pro/utils/crypto.py`

 * *Files identical despite different names*

### Comparing `xtn-tools-pro-1.0.0.1.5/xtn_tools_pro/utils/file_utils.py` & `xtn-tools-pro-1.0.0.1.6/xtn_tools_pro/utils/file_utils.py`

 * *Files identical despite different names*

### Comparing `xtn-tools-pro-1.0.0.1.5/xtn_tools_pro/utils/helpers.py` & `xtn-tools-pro-1.0.0.1.6/xtn_tools_pro/utils/helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -118,9 +118,13 @@
     :param params:
     :return:
     """
     encoded_params = urlencode(params)
     full_url = url + "?" + encoded_params
     return full_url
 
+
+
 if __name__ == '__main__':
-    print(get_uuid(4))
+    # print(get_uuid(4))
+    from faker import Faker
+
```

### Comparing `xtn-tools-pro-1.0.0.1.5/xtn_tools_pro/utils/log.py` & `xtn-tools-pro-1.0.0.1.6/xtn_tools_pro/utils/log.py`

 * *Files identical despite different names*

### Comparing `xtn-tools-pro-1.0.0.1.5/xtn_tools_pro/utils/retry.py` & `xtn-tools-pro-1.0.0.1.6/xtn_tools_pro/utils/retry.py`

 * *Files identical despite different names*

### Comparing `xtn-tools-pro-1.0.0.1.5/xtn_tools_pro/utils/sql.py` & `xtn-tools-pro-1.0.0.1.6/xtn_tools_pro/utils/sql.py`

 * *Files identical despite different names*

### Comparing `xtn-tools-pro-1.0.0.1.5/xtn_tools_pro/utils/time_utils.py` & `xtn-tools-pro-1.0.0.1.6/xtn_tools_pro/utils/time_utils.py`

 * *Files identical despite different names*

### Comparing `xtn-tools-pro-1.0.0.1.5/xtn_tools_pro.egg-info/SOURCES.txt` & `xtn-tools-pro-1.0.0.1.6/xtn_tools_pro.egg-info/SOURCES.txt`

 * *Files identical despite different names*

