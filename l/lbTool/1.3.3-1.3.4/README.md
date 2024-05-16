# Comparing `tmp/lbTool-1.3.3.tar.gz` & `tmp/lbtool-1.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lbTool-1.3.3.tar", last modified: Wed Jan 17 07:02:46 2024, max compression
+gzip compressed data, was "lbtool-1.3.4.tar", last modified: Thu May 16 11:14:04 2024, max compression
```

## Comparing `lbTool-1.3.3.tar` & `lbtool-1.3.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2024-01-17 07:02:46.188553 lbTool-1.3.3/
--rw-rw-rw-   0        0        0     5915 2024-01-17 07:02:46.187555 lbTool-1.3.3/PKG-INFO
--rw-rw-rw-   0        0        0     5402 2024-01-17 07:02:08.000000 lbTool-1.3.3/README.md
-drwxrwxrwx   0        0        0        0 2024-01-17 07:02:46.179576 lbTool-1.3.3/lbTool/
--rw-rw-rw-   0        0        0     4492 2023-12-04 07:29:53.000000 lbTool-1.3.3/lbTool/Common.py
--rw-rw-rw-   0        0        0     1075 2023-11-08 02:54:21.000000 lbTool-1.3.3/lbTool/ConfigManager.py
--rw-rw-rw-   0        0        0    10452 2024-01-17 05:40:57.000000 lbTool-1.3.3/lbTool/Db.py
--rw-rw-rw-   0        0        0    18185 2024-01-17 06:47:24.000000 lbTool-1.3.3/lbTool/DmDb.py
--rw-rw-rw-   0        0        0     4063 2023-07-14 07:59:22.000000 lbTool-1.3.3/lbTool/EnCipher.py
--rw-rw-rw-   0        0        0     2280 2023-08-22 15:07:22.000000 lbTool-1.3.3/lbTool/FileUtil.py
--rw-rw-rw-   0        0        0     2937 2023-12-11 07:24:18.000000 lbTool-1.3.3/lbTool/Logging.py
--rw-rw-rw-   0        0        0        0 2023-07-25 07:51:14.000000 lbTool-1.3.3/lbTool/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-17 07:02:46.186558 lbTool-1.3.3/lbTool.egg-info/
--rw-rw-rw-   0        0        0     5915 2024-01-17 07:02:46.000000 lbTool-1.3.3/lbTool.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      311 2024-01-17 07:02:46.000000 lbTool-1.3.3/lbTool.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-01-17 07:02:46.000000 lbTool-1.3.3/lbTool.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      148 2024-01-17 07:02:46.000000 lbTool-1.3.3/lbTool.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-01-17 07:02:46.000000 lbTool-1.3.3/lbTool.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-01-17 07:02:46.188553 lbTool-1.3.3/setup.cfg
--rw-rw-rw-   0        0        0     1064 2024-01-17 07:02:08.000000 lbTool-1.3.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-16 11:14:04.351777 lbtool-1.3.4/
+-rw-rw-rw-   0        0        0     5915 2024-05-16 11:14:04.350780 lbtool-1.3.4/PKG-INFO
+-rw-rw-rw-   0        0        0     5402 2024-01-17 07:02:08.000000 lbtool-1.3.4/README.md
+drwxrwxrwx   0        0        0        0 2024-05-16 11:14:04.343798 lbtool-1.3.4/lbTool/
+-rw-rw-rw-   0        0        0     4492 2023-12-04 07:29:53.000000 lbtool-1.3.4/lbTool/Common.py
+-rw-rw-rw-   0        0        0     1075 2023-11-08 02:54:21.000000 lbtool-1.3.4/lbTool/ConfigManager.py
+-rw-rw-rw-   0        0        0    10446 2024-05-16 08:08:55.000000 lbtool-1.3.4/lbTool/Db.py
+-rw-rw-rw-   0        0        0    18181 2024-05-15 16:26:28.000000 lbtool-1.3.4/lbTool/DmDb.py
+-rw-rw-rw-   0        0        0     4063 2023-07-14 07:59:22.000000 lbtool-1.3.4/lbTool/EnCipher.py
+-rw-rw-rw-   0        0        0     2280 2023-08-22 15:07:22.000000 lbtool-1.3.4/lbTool/FileUtil.py
+-rw-rw-rw-   0        0        0     3140 2024-05-16 11:06:24.000000 lbtool-1.3.4/lbTool/Logging.py
+-rw-rw-rw-   0        0        0        0 2023-07-25 07:51:14.000000 lbtool-1.3.4/lbTool/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-16 11:14:04.349782 lbtool-1.3.4/lbTool.egg-info/
+-rw-rw-rw-   0        0        0     5915 2024-05-16 11:14:04.000000 lbtool-1.3.4/lbTool.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      311 2024-05-16 11:14:04.000000 lbtool-1.3.4/lbTool.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-16 11:14:04.000000 lbtool-1.3.4/lbTool.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      148 2024-05-16 11:14:04.000000 lbtool-1.3.4/lbTool.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-05-16 11:14:04.000000 lbtool-1.3.4/lbTool.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-16 11:14:04.351777 lbtool-1.3.4/setup.cfg
+-rw-rw-rw-   0        0        0     1064 2024-05-16 11:11:01.000000 lbtool-1.3.4/setup.py
```

### Comparing `lbTool-1.3.3/PKG-INFO` & `lbtool-1.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lbTool
-Version: 1.3.3
+Version: 1.3.4
 Summary: Multifunctional Toolset
 Author: lb
 Author-email: lcoolb@163.com
 Requires-Python: >=3.6, <3.11
 Description-Content-Type: text/markdown
 Requires-Dist: requests
 Requires-Dist: gmSsl==3.2.2
```

### Comparing `lbTool-1.3.3/README.md` & `lbtool-1.3.4/README.md`

 * *Files identical despite different names*

### Comparing `lbTool-1.3.3/lbTool/Common.py` & `lbtool-1.3.4/lbTool/Common.py`

 * *Files identical despite different names*

### Comparing `lbTool-1.3.3/lbTool/ConfigManager.py` & `lbtool-1.3.4/lbTool/ConfigManager.py`

 * *Files identical despite different names*

### Comparing `lbTool-1.3.3/lbTool/Db.py` & `lbtool-1.3.4/lbTool/Db.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import datetime
 
+from lbTool.ConfigManager import ConfigManager
 from pony.orm import *
 from pony.orm.core import EntityMeta
 
-from lib.lbTool.ConfigManager import ConfigManager
-
 
 def get_orm_con():
     """
     获取数据库连接
     :return:
     """
     db_config = ConfigManager.get_value("database")
@@ -20,20 +19,20 @@
                           password=f"{db_config['password']}",
                           db=f"{db_config['db_name']}")
     else:
         raise RuntimeError("不支持的数据库连接！")
     return db_con
 
 
-def init_db(db_con, is_create_table=False, show_sql=True):
+def init_db(db_con, show_sql=True, is_create_table=False):
     """
     初始化db
     :param db_con: db对象
-    :param is_create_table: 是否创建表
     :param show_sql: 是否在控制台显示语句
+    :param is_create_table: 是否创建表
     :return:
     """
     if show_sql:
         # 控制台显示语句
         sql_debug(True)
     create_table = True if is_create_table is True else False
     # 根据实体关联表
```

### Comparing `lbTool-1.3.3/lbTool/DmDb.py` & `lbtool-1.3.4/lbTool/DmDb.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import dmPython
 
-from lib.lbTool.ConfigManager import ConfigManager
+from lbTool.ConfigManager import ConfigManager
 
 
 def get_dm_con(contextmanager=False):
     """
     获取数据库连接
     :param contextmanager: 是否使用上下文管理器 默认False
     :return:
```

### Comparing `lbTool-1.3.3/lbTool/EnCipher.py` & `lbtool-1.3.4/lbTool/EnCipher.py`

 * *Files identical despite different names*

### Comparing `lbTool-1.3.3/lbTool/FileUtil.py` & `lbtool-1.3.4/lbTool/FileUtil.py`

 * *Files identical despite different names*

### Comparing `lbTool-1.3.3/lbTool/Logging.py` & `lbtool-1.3.4/lbTool/Logging.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,19 +2,28 @@
 import logging
 from logging import config
 import os
 
 import yaml
 
 
-class Logger:
-    def __init__(self, init_logger="fileLogger"):
+def get_logger(init_logger="root"):
+    """
+    获取日志操作对象
+    :param init_logger: 默认root，可单独指定
+    """
+    logger_base = __Logger(init_logger)
+    return logger_base.logger
+
+
+class __Logger:
+    def __init__(self, init_logger="root"):
         """
         初始化日志管理类
-        :param init_logger: 日志处理器 默认fileLogger 为空则使用root
+        :param init_logger: 日志处理器 默认root，可单独指定
         """
         # 配置日志记录 日志级别从低到高 DEBUG->INFO->WARNING->ERROR->CRITICAL
         # 1.基本配置
         # logging.basicConfig(level=logging.DEBUG,  # 设置日志级别为 DEBUG（最低级别）
         #                     filename=f'Log/Logs_{datetime.now().strftime("%Y%m%d")}.log',  # 指定日志文件名
         #                     filemode='a',  # 设置文件模式为追加写入
         #                     format='%(asctime)s - %(levelname)s - %(message)s')
```

### Comparing `lbTool-1.3.3/lbTool.egg-info/PKG-INFO` & `lbtool-1.3.4/lbTool.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lbTool
-Version: 1.3.3
+Version: 1.3.4
 Summary: Multifunctional Toolset
 Author: lb
 Author-email: lcoolb@163.com
 Requires-Python: >=3.6, <3.11
 Description-Content-Type: text/markdown
 Requires-Dist: requests
 Requires-Dist: gmSsl==3.2.2
```

### Comparing `lbTool-1.3.3/setup.py` & `lbtool-1.3.4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='lbTool',  # 包的名称
-    version='1.3.3',  # 版本号
+    version='1.3.4',  # 版本号
     author='lb',  # 作者名
     author_email='lcoolb@163.com',
     description='Multifunctional Toolset',  # 包的描述信息
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=find_packages(),  # 包含的所有包
     install_requires=[  # 依赖的其他包
```

