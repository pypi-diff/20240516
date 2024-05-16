# Comparing `tmp/cloudreve-1.0.2.tar.gz` & `tmp/cloudreve-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cloudreve-1.0.2.tar", last modified: Tue May 14 23:12:52 2024, max compression
+gzip compressed data, was "cloudreve-1.0.3.tar", last modified: Thu May 16 08:38:43 2024, max compression
```

## Comparing `cloudreve-1.0.2.tar` & `cloudreve-1.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-05-14 23:12:52.052342 cloudreve-1.0.2/
--rw-rw-rw-   0        0        0    35823 2024-04-30 15:03:13.000000 cloudreve-1.0.2/LICENSE
--rw-rw-rw-   0        0        0     2023 2024-05-14 23:12:52.051834 cloudreve-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     1149 2024-05-14 23:12:25.000000 cloudreve-1.0.2/README.md
--rw-rw-rw-   0        0        0       42 2024-05-14 23:12:52.053144 cloudreve-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1353 2024-05-14 23:12:15.000000 cloudreve-1.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-14 23:12:51.996770 cloudreve-1.0.2/src/
-drwxrwxrwx   0        0        0        0 2024-05-14 23:12:52.008863 cloudreve-1.0.2/src/cloudreve/
--rw-rw-rw-   0        0        0       28 2024-04-30 17:10:56.000000 cloudreve-1.0.2/src/cloudreve/__init__.py
--rw-rw-rw-   0        0        0    11459 2024-05-01 03:39:59.000000 cloudreve-1.0.2/src/cloudreve/models.py
-drwxrwxrwx   0        0        0        0 2024-05-14 23:12:52.048601 cloudreve-1.0.2/src/cloudreve.egg-info/
--rw-rw-rw-   0        0        0     2023 2024-05-14 23:12:51.000000 cloudreve-1.0.2/src/cloudreve.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      260 2024-05-14 23:12:51.000000 cloudreve-1.0.2/src/cloudreve.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-14 23:12:51.000000 cloudreve-1.0.2/src/cloudreve.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-05-14 23:12:51.000000 cloudreve-1.0.2/src/cloudreve.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-05-14 23:12:51.000000 cloudreve-1.0.2/src/cloudreve.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-16 08:38:43.066848 cloudreve-1.0.3/
+-rw-rw-rw-   0        0        0    35823 2024-04-30 15:03:13.000000 cloudreve-1.0.3/LICENSE
+-rw-rw-rw-   0        0        0     2163 2024-05-16 08:38:43.064844 cloudreve-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1289 2024-05-14 23:14:08.000000 cloudreve-1.0.3/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-16 08:38:43.066848 cloudreve-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1353 2024-05-16 08:37:57.000000 cloudreve-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-16 08:38:43.022217 cloudreve-1.0.3/src/
+drwxrwxrwx   0        0        0        0 2024-05-16 08:38:43.030735 cloudreve-1.0.3/src/cloudreve/
+-rw-rw-rw-   0        0        0       29 2024-05-16 08:26:12.000000 cloudreve-1.0.3/src/cloudreve/__init__.py
+-rw-rw-rw-   0        0        0    11459 2024-05-01 03:39:59.000000 cloudreve-1.0.3/src/cloudreve/models.py
+drwxrwxrwx   0        0        0        0 2024-05-16 08:38:43.063842 cloudreve-1.0.3/src/cloudreve.egg-info/
+-rw-rw-rw-   0        0        0     2163 2024-05-16 08:38:42.000000 cloudreve-1.0.3/src/cloudreve.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      260 2024-05-16 08:38:42.000000 cloudreve-1.0.3/src/cloudreve.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-16 08:38:42.000000 cloudreve-1.0.3/src/cloudreve.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-05-16 08:38:42.000000 cloudreve-1.0.3/src/cloudreve.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-16 08:38:42.000000 cloudreve-1.0.3/src/cloudreve.egg-info/top_level.txt
```

### Comparing `cloudreve-1.0.2/LICENSE` & `cloudreve-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `cloudreve-1.0.2/PKG-INFO` & `cloudreve-1.0.3/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudreve
-Version: 1.0.2
+Version: 1.0.3
 Summary: SDK for Cloudreve sites
 Home-page: https://github.com/yxzlwz/cloudreve-sdk
 Author: yxzlwz
 Author-email: yxzlwz@gmail.com
 License: GPLv3
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
@@ -31,14 +31,18 @@
 
 ## 安装
 
 ```bash
 pip3 install cloudreve
 ```
 
+## 使用前说明
+
+- 本项目上传功能目前只适配了 **本机存储** 和 **OneDrive存储** ，有别的需求可以提PR。
+
 ## 示例
 
 ```python
 from cloudreve import Cloudreve
 
 # 初始化
 conn = Cloudreve('http://127.0.0.1:5212')
```

### Comparing `cloudreve-1.0.2/README.md` & `cloudreve-1.0.3/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -8,14 +8,18 @@
 
 ## 安装
 
 ```bash
 pip3 install cloudreve
 ```
 
+## 使用前说明
+
+- 本项目上传功能目前只适配了 **本机存储** 和 **OneDrive存储** ，有别的需求可以提PR。
+
 ## 示例
 
 ```python
 from cloudreve import Cloudreve
 
 # 初始化
 conn = Cloudreve('http://127.0.0.1:5212')
```

### Comparing `cloudreve-1.0.2/setup.py` & `cloudreve-1.0.3/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,15 +7,15 @@
           encoding='utf-8') as fh:
     readme = fh.read()
 
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
 
 setup(
     name='cloudreve',
-    version='1.0.2',
+    version='1.0.3',
     package_dir={'': 'src'},
     packages=find_packages(where='src'),
     include_package_data=True,
     license='GPLv3',
     description='SDK for Cloudreve sites',
     long_description=readme,
     long_description_content_type='text/markdown',
```

### Comparing `cloudreve-1.0.2/src/cloudreve/models.py` & `cloudreve-1.0.3/src/cloudreve/models.py`

 * *Files identical despite different names*

### Comparing `cloudreve-1.0.2/src/cloudreve.egg-info/PKG-INFO` & `cloudreve-1.0.3/src/cloudreve.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudreve
-Version: 1.0.2
+Version: 1.0.3
 Summary: SDK for Cloudreve sites
 Home-page: https://github.com/yxzlwz/cloudreve-sdk
 Author: yxzlwz
 Author-email: yxzlwz@gmail.com
 License: GPLv3
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
@@ -31,14 +31,18 @@
 
 ## 安装
 
 ```bash
 pip3 install cloudreve
 ```
 
+## 使用前说明
+
+- 本项目上传功能目前只适配了 **本机存储** 和 **OneDrive存储** ，有别的需求可以提PR。
+
 ## 示例
 
 ```python
 from cloudreve import Cloudreve
 
 # 初始化
 conn = Cloudreve('http://127.0.0.1:5212')
```

