# Comparing `tmp/sqlman-0.3.1.tar.gz` & `tmp/sqlman-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlman-0.3.1.tar", last modified: Fri May 10 06:16:35 2024, max compression
+gzip compressed data, was "sqlman-0.3.2.tar", last modified: Thu May 16 11:47:57 2024, max compression
```

## Comparing `sqlman-0.3.1.tar` & `sqlman-0.3.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 wangtuo    (501) staff       (20)        0 2024-05-10 06:16:35.759545 sqlman-0.3.1/
--rw-r--r--   0 wangtuo    (501) staff       (20)     3990 2024-05-10 06:16:35.759327 sqlman-0.3.1/PKG-INFO
--rw-r--r--   0 wangtuo    (501) staff       (20)     3702 2024-05-10 06:15:07.000000 sqlman-0.3.1/README.md
--rw-r--r--   0 wangtuo    (501) staff       (20)       38 2024-05-10 06:16:35.759581 sqlman-0.3.1/setup.cfg
--rw-r--r--   0 wangtuo    (501) staff       (20)      645 2024-05-10 06:16:31.000000 sqlman-0.3.1/setup.py
-drwxr-xr-x   0 wangtuo    (501) staff       (20)        0 2024-05-10 06:16:35.758040 sqlman-0.3.1/sqlman/
--rw-r--r--   0 wangtuo    (501) staff       (20)       60 2024-04-17 16:06:46.000000 sqlman-0.3.1/sqlman/__init__.py
--rw-r--r--   0 wangtuo    (501) staff       (20)     6497 2024-05-10 05:04:46.000000 sqlman-0.3.1/sqlman/handler.py
--rw-r--r--   0 wangtuo    (501) staff       (20)     9510 2024-05-10 05:43:51.000000 sqlman-0.3.1/sqlman/table_controller.py
--rw-r--r--   0 wangtuo    (501) staff       (20)     1362 2024-04-21 12:47:57.000000 sqlman-0.3.1/sqlman/tools.py
-drwxr-xr-x   0 wangtuo    (501) staff       (20)        0 2024-05-10 06:16:35.758893 sqlman-0.3.1/sqlman.egg-info/
--rw-r--r--   0 wangtuo    (501) staff       (20)     3990 2024-05-10 06:16:35.000000 sqlman-0.3.1/sqlman.egg-info/PKG-INFO
--rw-r--r--   0 wangtuo    (501) staff       (20)      292 2024-05-10 06:16:35.000000 sqlman-0.3.1/sqlman.egg-info/SOURCES.txt
--rw-r--r--   0 wangtuo    (501) staff       (20)        1 2024-05-10 06:16:35.000000 sqlman-0.3.1/sqlman.egg-info/dependency_links.txt
--rw-r--r--   0 wangtuo    (501) staff       (20)        1 2024-05-10 06:16:35.000000 sqlman-0.3.1/sqlman.egg-info/not-zip-safe
--rw-r--r--   0 wangtuo    (501) staff       (20)       29 2024-05-10 06:16:35.000000 sqlman-0.3.1/sqlman.egg-info/requires.txt
--rw-r--r--   0 wangtuo    (501) staff       (20)        7 2024-05-10 06:16:35.000000 sqlman-0.3.1/sqlman.egg-info/top_level.txt
-drwxr-xr-x   0 wangtuo    (501) staff       (20)        0 2024-05-10 06:16:35.758998 sqlman-0.3.1/tests/
--rw-r--r--   0 wangtuo    (501) staff       (20)      279 2024-05-10 05:38:51.000000 sqlman-0.3.1/tests/test-0.py
+drwxr-xr-x   0 wangtuo    (501) staff       (20)        0 2024-05-16 11:47:57.022647 sqlman-0.3.2/
+-rw-r--r--   0 wangtuo    (501) staff       (20)     3990 2024-05-16 11:47:57.022430 sqlman-0.3.2/PKG-INFO
+-rw-r--r--   0 wangtuo    (501) staff       (20)     3702 2024-05-10 06:15:07.000000 sqlman-0.3.2/README.md
+-rw-r--r--   0 wangtuo    (501) staff       (20)       38 2024-05-16 11:47:57.022686 sqlman-0.3.2/setup.cfg
+-rw-r--r--   0 wangtuo    (501) staff       (20)      645 2024-05-16 11:47:03.000000 sqlman-0.3.2/setup.py
+drwxr-xr-x   0 wangtuo    (501) staff       (20)        0 2024-05-16 11:47:57.021258 sqlman-0.3.2/sqlman/
+-rw-r--r--   0 wangtuo    (501) staff       (20)       60 2024-04-17 16:06:46.000000 sqlman-0.3.2/sqlman/__init__.py
+-rw-r--r--   0 wangtuo    (501) staff       (20)     6497 2024-05-10 05:04:46.000000 sqlman-0.3.2/sqlman/handler.py
+-rw-r--r--   0 wangtuo    (501) staff       (20)     9514 2024-05-16 11:47:03.000000 sqlman-0.3.2/sqlman/table_controller.py
+-rw-r--r--   0 wangtuo    (501) staff       (20)     1362 2024-04-21 12:47:57.000000 sqlman-0.3.2/sqlman/tools.py
+drwxr-xr-x   0 wangtuo    (501) staff       (20)        0 2024-05-16 11:47:57.021993 sqlman-0.3.2/sqlman.egg-info/
+-rw-r--r--   0 wangtuo    (501) staff       (20)     3990 2024-05-16 11:47:56.000000 sqlman-0.3.2/sqlman.egg-info/PKG-INFO
+-rw-r--r--   0 wangtuo    (501) staff       (20)      292 2024-05-16 11:47:56.000000 sqlman-0.3.2/sqlman.egg-info/SOURCES.txt
+-rw-r--r--   0 wangtuo    (501) staff       (20)        1 2024-05-16 11:47:56.000000 sqlman-0.3.2/sqlman.egg-info/dependency_links.txt
+-rw-r--r--   0 wangtuo    (501) staff       (20)        1 2024-05-16 11:47:56.000000 sqlman-0.3.2/sqlman.egg-info/not-zip-safe
+-rw-r--r--   0 wangtuo    (501) staff       (20)       29 2024-05-16 11:47:56.000000 sqlman-0.3.2/sqlman.egg-info/requires.txt
+-rw-r--r--   0 wangtuo    (501) staff       (20)        7 2024-05-16 11:47:56.000000 sqlman-0.3.2/sqlman.egg-info/top_level.txt
+drwxr-xr-x   0 wangtuo    (501) staff       (20)        0 2024-05-16 11:47:57.022160 sqlman-0.3.2/tests/
+-rw-r--r--   0 wangtuo    (501) staff       (20)      279 2024-05-10 05:38:51.000000 sqlman-0.3.2/tests/test-0.py
```

### Comparing `sqlman-0.3.1/PKG-INFO` & `sqlman-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlman
-Version: 0.3.1
+Version: 0.3.2
 Summary: 告别SQL语句，python操作mysql的贴心助手
 Home-page: https://github.com/markadc/sqlman
 Author: WangTuo
 Author-email: markadc@126.com
 License: MIT
 Keywords: Python,MySQL,Database
 Description-Content-Type: text/markdown
```

### Comparing `sqlman-0.3.1/README.md` & `sqlman-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `sqlman-0.3.1/setup.py` & `sqlman-0.3.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name='sqlman',
-    version='0.3.1',
+    version='0.3.2',
     description='告别SQL语句，python操作mysql的贴心助手',
     url='https://github.com/markadc/sqlman',
     author='WangTuo',
     author_email='markadc@126.com',
     packages=find_packages(),
     license='MIT',
     zip_safe=False,
```

### Comparing `sqlman-0.3.1/sqlman/handler.py` & `sqlman-0.3.2/sqlman/handler.py`

 * *Files identical despite different names*

### Comparing `sqlman-0.3.1/sqlman/table_controller.py` & `sqlman-0.3.2/sqlman/table_controller.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,16 +12,16 @@
     def __init__(self, cfg: dict, table: str):
         super().__init__(cfg)
         self.table = table
 
     def get_tables(self) -> list:
         """获取当前数据库的所有表"""
         sql = 'show tables'
-        data = self.exe_sql(sql, mode=2)['query']
-        tables = [this['Tables_in_test'] for this in data]
+        data = self.exe_sql(sql, dict_cursor=False, mode=2)['query']
+        tables = [this[0] for this in data]
         return tables
 
     def kill(self) -> bool:
         """删除这张表"""
         sql = 'DROP TABLE {}'.format(self.table)
         return self.exe_sql(sql)['status'] == 1
```

### Comparing `sqlman-0.3.1/sqlman/tools.py` & `sqlman-0.3.2/sqlman/tools.py`

 * *Files identical despite different names*

### Comparing `sqlman-0.3.1/sqlman.egg-info/PKG-INFO` & `sqlman-0.3.2/sqlman.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlman
-Version: 0.3.1
+Version: 0.3.2
 Summary: 告别SQL语句，python操作mysql的贴心助手
 Home-page: https://github.com/markadc/sqlman
 Author: WangTuo
 Author-email: markadc@126.com
 License: MIT
 Keywords: Python,MySQL,Database
 Description-Content-Type: text/markdown
```

