# Comparing `tmp/jyhelper-1.2.2.tar.gz` & `tmp/jyhelper-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jyhelper-1.2.2.tar", last modified: Wed Apr 10 09:34:05 2024, max compression
+gzip compressed data, was "jyhelper-1.2.3.tar", last modified: Thu May 16 09:07:58 2024, max compression
```

## Comparing `jyhelper-1.2.2.tar` & `jyhelper-1.2.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-04-10 09:34:05.488783 jyhelper-1.2.2/
--rw-rw-rw-   0        0        0     1130 2024-04-10 09:34:05.486973 jyhelper-1.2.2/PKG-INFO
--rw-rw-rw-   0        0        0      820 2023-11-17 09:46:48.000000 jyhelper-1.2.2/README.md
-drwxrwxrwx   0        0        0        0 2024-04-10 09:34:05.451018 jyhelper-1.2.2/jyhelper/
--rw-rw-rw-   0        0        0      385 2023-11-17 06:00:40.000000 jyhelper-1.2.2/jyhelper/__init__.py
--rw-rw-rw-   0        0        0     4455 2024-01-30 07:23:11.000000 jyhelper-1.2.2/jyhelper/common.py
--rw-rw-rw-   0        0        0    15783 2023-12-28 09:52:26.000000 jyhelper-1.2.2/jyhelper/db.py
--rw-rw-rw-   0        0        0     5284 2024-01-05 03:38:54.000000 jyhelper-1.2.2/jyhelper/feishuRobot.py
--rw-rw-rw-   0        0        0     1709 2023-11-17 03:22:58.000000 jyhelper-1.2.2/jyhelper/file.py
--rw-rw-rw-   0        0        0     4651 2023-11-10 07:43:50.000000 jyhelper-1.2.2/jyhelper/timeHelper.py
-drwxrwxrwx   0        0        0        0 2024-04-10 09:34:05.482980 jyhelper-1.2.2/jyhelper.egg-info/
--rw-rw-rw-   0        0        0     1130 2024-04-10 09:34:04.000000 jyhelper-1.2.2/jyhelper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      296 2024-04-10 09:34:04.000000 jyhelper-1.2.2/jyhelper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-10 09:34:04.000000 jyhelper-1.2.2/jyhelper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2024-04-10 09:34:04.000000 jyhelper-1.2.2/jyhelper.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-04-10 09:34:04.000000 jyhelper-1.2.2/jyhelper.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-10 09:34:05.488783 jyhelper-1.2.2/setup.cfg
--rw-rw-rw-   0        0        0      718 2024-04-10 09:32:13.000000 jyhelper-1.2.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-16 09:07:58.837970 jyhelper-1.2.3/
+-rw-rw-rw-   0        0        0     1130 2024-05-16 09:07:58.835993 jyhelper-1.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0      820 2023-11-17 09:46:48.000000 jyhelper-1.2.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-16 09:07:58.808683 jyhelper-1.2.3/jyhelper/
+-rw-rw-rw-   0        0        0      385 2023-11-17 06:00:40.000000 jyhelper-1.2.3/jyhelper/__init__.py
+-rw-rw-rw-   0        0        0     4455 2024-01-30 07:23:11.000000 jyhelper-1.2.3/jyhelper/common.py
+-rw-rw-rw-   0        0        0    15783 2023-12-28 09:52:26.000000 jyhelper-1.2.3/jyhelper/db.py
+-rw-rw-rw-   0        0        0     5284 2024-01-05 03:38:54.000000 jyhelper-1.2.3/jyhelper/feishuRobot.py
+-rw-rw-rw-   0        0        0     1888 2024-05-16 08:55:22.000000 jyhelper-1.2.3/jyhelper/file.py
+-rw-rw-rw-   0        0        0     4651 2024-04-30 03:17:37.000000 jyhelper-1.2.3/jyhelper/timeHelper.py
+drwxrwxrwx   0        0        0        0 2024-05-16 09:07:58.832531 jyhelper-1.2.3/jyhelper.egg-info/
+-rw-rw-rw-   0        0        0     1130 2024-05-16 09:07:58.000000 jyhelper-1.2.3/jyhelper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      296 2024-05-16 09:07:58.000000 jyhelper-1.2.3/jyhelper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-16 09:07:58.000000 jyhelper-1.2.3/jyhelper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2024-05-16 09:07:58.000000 jyhelper-1.2.3/jyhelper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-05-16 09:07:58.000000 jyhelper-1.2.3/jyhelper.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-16 09:07:58.837970 jyhelper-1.2.3/setup.cfg
+-rw-rw-rw-   0        0        0      718 2024-05-16 09:05:44.000000 jyhelper-1.2.3/setup.py
```

### Comparing `jyhelper-1.2.2/PKG-INFO` & `jyhelper-1.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jyhelper
-Version: 1.2.2
+Version: 1.2.3
 Summary: 各种实用、常用的小函数、类
 Home-page: https://pypi.org/project/jyhelper/
 Author: JY
 Author-email: your-email@example.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.0
```

### Comparing `jyhelper-1.2.2/README.md` & `jyhelper-1.2.3/README.md`

 * *Files identical despite different names*

### Comparing `jyhelper-1.2.2/jyhelper/common.py` & `jyhelper-1.2.3/jyhelper/common.py`

 * *Files identical despite different names*

### Comparing `jyhelper-1.2.2/jyhelper/db.py` & `jyhelper-1.2.3/jyhelper/db.py`

 * *Files identical despite different names*

### Comparing `jyhelper-1.2.2/jyhelper/feishuRobot.py` & `jyhelper-1.2.3/jyhelper/feishuRobot.py`

 * *Files identical despite different names*

### Comparing `jyhelper-1.2.2/jyhelper/file.py` & `jyhelper-1.2.3/jyhelper/file.py`

 * *Files 15% similar despite different names*

```diff
@@ -43,11 +43,17 @@
 
     # 清空文件后写入
     @staticmethod
     def writeTxtFileNewMode(filePath, content, encoding=ENCODING_UTF8):
         with open(filePath, 'w', encoding=encoding) as f:
             f.write(content)
 
+    # 得到文件的行数
+    @staticmethod
+    def countLines(filePath, encoding=ENCODING_UTF8):
+        with open(filePath, 'r', encoding=encoding) as f:
+            line_count = sum(1 for line in f)
+        return line_count
+
 
 if __name__ == '__main__':
-    for line in file.readTxtFileByLine('D:\\downloads\\index.html'):
-        print(line)
+    print(file.countLines(''))
```

### Comparing `jyhelper-1.2.2/jyhelper/timeHelper.py` & `jyhelper-1.2.3/jyhelper/timeHelper.py`

 * *Files identical despite different names*

### Comparing `jyhelper-1.2.2/jyhelper.egg-info/PKG-INFO` & `jyhelper-1.2.3/jyhelper.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jyhelper
-Version: 1.2.2
+Version: 1.2.3
 Summary: 各种实用、常用的小函数、类
 Home-page: https://pypi.org/project/jyhelper/
 Author: JY
 Author-email: your-email@example.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.0
```

### Comparing `jyhelper-1.2.2/setup.py` & `jyhelper-1.2.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # @Time : 2023/11/08 18:38 
 # @Author : JY
 
 from setuptools import setup
 
 setup(
     name='jyhelper',
-    version='1.2.2',
+    version='1.2.3',
     packages=['jyhelper'],
     install_requires=[
         'pymysql',
         'requests'
     ],
     description='各种实用、常用的小函数、类',
     long_description=open('README.md',encoding='utf-8').read(),  # 详细描述，通常从 README.md 中读取
```

