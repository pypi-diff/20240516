# Comparing `tmp/ncmlistdownloader-2.0.0.240515a1.tar.gz` & `tmp/ncmlistdownloader-2.0.0.240516a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ncmlistdownloader-2.0.0.240515a1.tar", last modified: Wed May 15 14:50:40 2024, max compression
+gzip compressed data, was "ncmlistdownloader-2.0.0.240516a1.tar", last modified: Thu May 16 15:00:08 2024, max compression
```

## Comparing `ncmlistdownloader-2.0.0.240515a1.tar` & `ncmlistdownloader-2.0.0.240516a1.tar`

### file list

```diff
@@ -1,35 +1,38 @@
-drwxrwxrwx   0        0        0        0 2024-05-15 14:50:40.986467 ncmlistdownloader-2.0.0.240515a1/
--rw-rw-rw-   0        0        0    35181 2024-04-22 14:49:08.000000 ncmlistdownloader-2.0.0.240515a1/LICENSE
--rw-rw-rw-   0        0        0     1297 2024-05-15 14:50:40.984455 ncmlistdownloader-2.0.0.240515a1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-15 14:50:40.906993 ncmlistdownloader-2.0.0.240515a1/ncmlistdownloader/
--rw-rw-rw-   0        0        0     1880 2024-05-10 14:55:05.000000 ncmlistdownloader-2.0.0.240515a1/ncmlistdownloader/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-15 14:50:40.943906 ncmlistdownloader-2.0.0.240515a1/ncmlistdownloader/cmd/
--rw-rw-rw-   0        0        0     1789 2024-04-29 10:16:10.000000 ncmlistdownloader-2.0.0.240515a1/ncmlistdownloader/cmd/__init__.py
--rw-rw-rw-   0        0        0      651 2024-04-29 10:21:56.000000 ncmlistdownloader-2.0.0.240515a1/ncmlistdownloader/cmd/common.py
--rw-rw-rw-   0        0        0     1685 2024-04-29 10:22:02.000000 ncmlistdownloader-2.0.0.240515a1/ncmlistdownloader/cmd/download.py
--rw-rw-rw-   0        0        0     2689 2024-04-29 10:22:08.000000 ncmlistdownloader-2.0.0.240515a1/ncmlistdownloader/cmd/find_from_id.py
--rw-rw-rw-   0        0        0     1664 2024-04-29 10:23:33.000000 ncmlistdownloader-2.0.0.240515a1/ncmlistdownloader/cmd/json_io.py
-drwxrwxrwx   0        0        0        0 2024-05-15 14:50:40.957703 ncmlistdownloader-2.0.0.240515a1/ncmlistdownloader/common/
--rw-rw-rw-   0        0        0     2862 2024-04-29 10:21:37.000000 ncmlistdownloader-2.0.0.240515a1/ncmlistdownloader/common/__init__.py
--rw-rw-rw-   0        0        0     2161 2024-04-29 10:21:11.000000 ncmlistdownloader-2.0.0.240515a1/ncmlistdownloader/common/encode_sec_key.py
--rw-rw-rw-   0        0        0     2376 2024-05-06 05:09:23.000000 ncmlistdownloader-2.0.0.240515a1/ncmlistdownloader/common/global_args.py
--rw-rw-rw-   0        0        0     1791 2024-04-29 10:20:35.000000 ncmlistdownloader-2.0.0.240515a1/ncmlistdownloader/common/thread_test.py
-drwxrwxrwx   0        0        0        0 2024-05-15 14:50:40.964687 ncmlistdownloader-2.0.0.240515a1/ncmlistdownloader/downloader/
--rw-rw-rw-   0        0        0     6233 2024-04-29 10:20:23.000000 ncmlistdownloader-2.0.0.240515a1/ncmlistdownloader/downloader/__init__.py
--rw-rw-rw-   0        0        0     1110 2024-04-30 04:27:30.000000 ncmlistdownloader-2.0.0.240515a1/ncmlistdownloader/downloader/json_list_io.py
-drwxrwxrwx   0        0        0        0 2024-05-15 14:50:40.968675 ncmlistdownloader-2.0.0.240515a1/ncmlistdownloader/editer/
--rw-rw-rw-   0        0        0     4034 2024-05-05 14:27:08.000000 ncmlistdownloader-2.0.0.240515a1/ncmlistdownloader/editer/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-15 14:50:40.970670 ncmlistdownloader-2.0.0.240515a1/ncmlistdownloader/playlist/
--rw-rw-rw-   0        0        0     2296 2024-04-29 10:19:56.000000 ncmlistdownloader-2.0.0.240515a1/ncmlistdownloader/playlist/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-15 14:50:40.974465 ncmlistdownloader-2.0.0.240515a1/ncmlistdownloader/song/
--rw-rw-rw-   0        0        0     9580 2024-05-05 14:27:08.000000 ncmlistdownloader-2.0.0.240515a1/ncmlistdownloader/song/__init__.py
--rw-rw-rw-   0        0        0     8233 2024-05-15 14:49:40.000000 ncmlistdownloader-2.0.0.240515a1/ncmlistdownloader/song/cleaned.py
-drwxrwxrwx   0        0        0        0 2024-05-15 14:50:40.980466 ncmlistdownloader-2.0.0.240515a1/ncmlistdownloader.egg-info/
--rw-rw-rw-   0        0        0     1297 2024-05-15 14:50:40.000000 ncmlistdownloader-2.0.0.240515a1/ncmlistdownloader.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      856 2024-05-15 14:50:40.000000 ncmlistdownloader-2.0.0.240515a1/ncmlistdownloader.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-15 14:50:40.000000 ncmlistdownloader-2.0.0.240515a1/ncmlistdownloader.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       70 2024-05-15 14:50:40.000000 ncmlistdownloader-2.0.0.240515a1/ncmlistdownloader.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       37 2024-05-15 14:50:40.000000 ncmlistdownloader-2.0.0.240515a1/ncmlistdownloader.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2024-05-15 14:50:40.000000 ncmlistdownloader-2.0.0.240515a1/ncmlistdownloader.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-15 14:50:40.986467 ncmlistdownloader-2.0.0.240515a1/setup.cfg
--rw-rw-rw-   0        0        0     1825 2024-05-15 14:50:09.000000 ncmlistdownloader-2.0.0.240515a1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-16 15:00:08.639268 ncmlistdownloader-2.0.0.240516a1/
+-rw-rw-rw-   0        0        0    35181 2024-05-16 14:27:24.000000 ncmlistdownloader-2.0.0.240516a1/LICENSE
+-rw-rw-rw-   0        0        0     1297 2024-05-16 15:00:08.637937 ncmlistdownloader-2.0.0.240516a1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-16 15:00:08.583064 ncmlistdownloader-2.0.0.240516a1/ncmlistdownloader/
+-rw-rw-rw-   0        0        0        0 2024-05-16 14:32:33.000000 ncmlistdownloader-2.0.0.240516a1/ncmlistdownloader/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-16 15:00:08.598671 ncmlistdownloader-2.0.0.240516a1/ncmlistdownloader/_old/
+-rw-rw-rw-   0        0        0     1880 2024-05-16 14:27:24.000000 ncmlistdownloader-2.0.0.240516a1/ncmlistdownloader/_old/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-16 15:00:08.607287 ncmlistdownloader-2.0.0.240516a1/ncmlistdownloader/_old/cmd/
+-rw-rw-rw-   0        0        0     1789 2024-05-16 14:27:24.000000 ncmlistdownloader-2.0.0.240516a1/ncmlistdownloader/_old/cmd/__init__.py
+-rw-rw-rw-   0        0        0      651 2024-05-16 14:27:24.000000 ncmlistdownloader-2.0.0.240516a1/ncmlistdownloader/_old/cmd/common.py
+-rw-rw-rw-   0        0        0     1685 2024-05-16 14:27:24.000000 ncmlistdownloader-2.0.0.240516a1/ncmlistdownloader/_old/cmd/download.py
+-rw-rw-rw-   0        0        0     2689 2024-05-16 14:27:24.000000 ncmlistdownloader-2.0.0.240516a1/ncmlistdownloader/_old/cmd/find_from_id.py
+-rw-rw-rw-   0        0        0     1664 2024-05-16 14:27:24.000000 ncmlistdownloader-2.0.0.240516a1/ncmlistdownloader/_old/cmd/json_io.py
+drwxrwxrwx   0        0        0        0 2024-05-16 15:00:08.617339 ncmlistdownloader-2.0.0.240516a1/ncmlistdownloader/_old/common/
+-rw-rw-rw-   0        0        0     2862 2024-04-29 10:21:37.000000 ncmlistdownloader-2.0.0.240516a1/ncmlistdownloader/_old/common/__init__.py
+-rw-rw-rw-   0        0        0     2161 2024-04-29 10:21:11.000000 ncmlistdownloader-2.0.0.240516a1/ncmlistdownloader/_old/common/encode_sec_key.py
+-rw-rw-rw-   0        0        0     1791 2024-04-29 10:20:35.000000 ncmlistdownloader-2.0.0.240516a1/ncmlistdownloader/_old/common/thread_test.py
+drwxrwxrwx   0        0        0        0 2024-05-16 15:00:08.621712 ncmlistdownloader-2.0.0.240516a1/ncmlistdownloader/_old/downloader/
+-rw-rw-rw-   0        0        0     6233 2024-04-29 10:20:23.000000 ncmlistdownloader-2.0.0.240516a1/ncmlistdownloader/_old/downloader/__init__.py
+-rw-rw-rw-   0        0        0     1110 2024-04-30 04:27:30.000000 ncmlistdownloader-2.0.0.240516a1/ncmlistdownloader/_old/downloader/json_list_io.py
+drwxrwxrwx   0        0        0        0 2024-05-16 15:00:08.621712 ncmlistdownloader-2.0.0.240516a1/ncmlistdownloader/_old/editer/
+-rw-rw-rw-   0        0        0     4034 2024-05-05 14:27:08.000000 ncmlistdownloader-2.0.0.240516a1/ncmlistdownloader/_old/editer/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-16 15:00:08.627972 ncmlistdownloader-2.0.0.240516a1/ncmlistdownloader/_old/playlist/
+-rw-rw-rw-   0        0        0     2296 2024-04-29 10:19:56.000000 ncmlistdownloader-2.0.0.240516a1/ncmlistdownloader/_old/playlist/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-16 15:00:08.630956 ncmlistdownloader-2.0.0.240516a1/ncmlistdownloader/_old/song/
+-rw-rw-rw-   0        0        0     9580 2024-05-05 14:27:08.000000 ncmlistdownloader-2.0.0.240516a1/ncmlistdownloader/_old/song/__init__.py
+-rw-rw-rw-   0        0        0     1923 2024-05-16 14:59:42.000000 ncmlistdownloader-2.0.0.240516a1/ncmlistdownloader/global_args.py
+drwxrwxrwx   0        0        0        0 2024-05-16 15:00:08.634945 ncmlistdownloader-2.0.0.240516a1/ncmlistdownloader/music/
+-rw-rw-rw-   0        0        0        0 2024-05-16 14:33:24.000000 ncmlistdownloader-2.0.0.240516a1/ncmlistdownloader/music/__init__.py
+-rw-rw-rw-   0        0        0        0 2024-05-16 14:33:48.000000 ncmlistdownloader-2.0.0.240516a1/ncmlistdownloader/music/multiple_tools.py
+drwxrwxrwx   0        0        0        0 2024-05-16 15:00:08.636940 ncmlistdownloader-2.0.0.240516a1/ncmlistdownloader.egg-info/
+-rw-rw-rw-   0        0        0     1297 2024-05-16 15:00:08.000000 ncmlistdownloader-2.0.0.240516a1/ncmlistdownloader.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      949 2024-05-16 15:00:08.000000 ncmlistdownloader-2.0.0.240516a1/ncmlistdownloader.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-16 15:00:08.000000 ncmlistdownloader-2.0.0.240516a1/ncmlistdownloader.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       37 2024-05-16 15:00:08.000000 ncmlistdownloader-2.0.0.240516a1/ncmlistdownloader.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2024-05-16 15:00:08.000000 ncmlistdownloader-2.0.0.240516a1/ncmlistdownloader.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-16 15:00:08.639268 ncmlistdownloader-2.0.0.240516a1/setup.cfg
+-rw-rw-rw-   0        0        0     1811 2024-05-16 14:32:18.000000 ncmlistdownloader-2.0.0.240516a1/setup.py
```

### Comparing `ncmlistdownloader-2.0.0.240515a1/LICENSE` & `ncmlistdownloader-2.0.0.240516a1/LICENSE`

 * *Files identical despite different names*

### Comparing `ncmlistdownloader-2.0.0.240515a1/PKG-INFO` & `ncmlistdownloader-2.0.0.240516a1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ncmlistdownloader
-Version: 2.0.0.240515a1
+Version: 2.0.0.240516a1
 Summary: 获取网易云音乐歌单数据，下载音乐，主动添加元信息。
 Home-page: https://gitee.com/Cooooldwind/163ListDownloader_NexT
 Author: CooooldWind_
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Customer Service
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: End Users/Desktop
```

### Comparing `ncmlistdownloader-2.0.0.240515a1/ncmlistdownloader/__init__.py` & `ncmlistdownloader-2.0.0.240516a1/ncmlistdownloader/_old/__init__.py`

 * *Files identical despite different names*

### Comparing `ncmlistdownloader-2.0.0.240515a1/ncmlistdownloader/cmd/__init__.py` & `ncmlistdownloader-2.0.0.240516a1/ncmlistdownloader/_old/cmd/__init__.py`

 * *Files identical despite different names*

### Comparing `ncmlistdownloader-2.0.0.240515a1/ncmlistdownloader/cmd/common.py` & `ncmlistdownloader-2.0.0.240516a1/ncmlistdownloader/_old/cmd/common.py`

 * *Files identical despite different names*

### Comparing `ncmlistdownloader-2.0.0.240515a1/ncmlistdownloader/cmd/download.py` & `ncmlistdownloader-2.0.0.240516a1/ncmlistdownloader/_old/cmd/download.py`

 * *Files identical despite different names*

### Comparing `ncmlistdownloader-2.0.0.240515a1/ncmlistdownloader/cmd/find_from_id.py` & `ncmlistdownloader-2.0.0.240516a1/ncmlistdownloader/_old/cmd/find_from_id.py`

 * *Files identical despite different names*

### Comparing `ncmlistdownloader-2.0.0.240515a1/ncmlistdownloader/cmd/json_io.py` & `ncmlistdownloader-2.0.0.240516a1/ncmlistdownloader/_old/cmd/json_io.py`

 * *Files identical despite different names*

### Comparing `ncmlistdownloader-2.0.0.240515a1/ncmlistdownloader/common/__init__.py` & `ncmlistdownloader-2.0.0.240516a1/ncmlistdownloader/_old/common/__init__.py`

 * *Files identical despite different names*

### Comparing `ncmlistdownloader-2.0.0.240515a1/ncmlistdownloader/common/encode_sec_key.py` & `ncmlistdownloader-2.0.0.240516a1/ncmlistdownloader/_old/common/encode_sec_key.py`

 * *Files identical despite different names*

### Comparing `ncmlistdownloader-2.0.0.240515a1/ncmlistdownloader/common/thread_test.py` & `ncmlistdownloader-2.0.0.240516a1/ncmlistdownloader/_old/common/thread_test.py`

 * *Files identical despite different names*

### Comparing `ncmlistdownloader-2.0.0.240515a1/ncmlistdownloader/downloader/__init__.py` & `ncmlistdownloader-2.0.0.240516a1/ncmlistdownloader/_old/downloader/__init__.py`

 * *Files identical despite different names*

### Comparing `ncmlistdownloader-2.0.0.240515a1/ncmlistdownloader/downloader/json_list_io.py` & `ncmlistdownloader-2.0.0.240516a1/ncmlistdownloader/_old/downloader/json_list_io.py`

 * *Files identical despite different names*

### Comparing `ncmlistdownloader-2.0.0.240515a1/ncmlistdownloader/editer/__init__.py` & `ncmlistdownloader-2.0.0.240516a1/ncmlistdownloader/_old/editer/__init__.py`

 * *Files identical despite different names*

### Comparing `ncmlistdownloader-2.0.0.240515a1/ncmlistdownloader/playlist/__init__.py` & `ncmlistdownloader-2.0.0.240516a1/ncmlistdownloader/_old/playlist/__init__.py`

 * *Files identical despite different names*

### Comparing `ncmlistdownloader-2.0.0.240515a1/ncmlistdownloader/song/__init__.py` & `ncmlistdownloader-2.0.0.240516a1/ncmlistdownloader/_old/song/__init__.py`

 * *Files identical despite different names*

### Comparing `ncmlistdownloader-2.0.0.240515a1/ncmlistdownloader.egg-info/PKG-INFO` & `ncmlistdownloader-2.0.0.240516a1/ncmlistdownloader.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ncmlistdownloader
-Version: 2.0.0.240515a1
+Version: 2.0.0.240516a1
 Summary: 获取网易云音乐歌单数据，下载音乐，主动添加元信息。
 Home-page: https://gitee.com/Cooooldwind/163ListDownloader_NexT
 Author: CooooldWind_
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Customer Service
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: End Users/Desktop
```

### Comparing `ncmlistdownloader-2.0.0.240515a1/ncmlistdownloader.egg-info/SOURCES.txt` & `ncmlistdownloader-2.0.0.240516a1/ncmlistdownloader.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 LICENSE
 setup.py
 ncmlistdownloader/__init__.py
+ncmlistdownloader/global_args.py
 ncmlistdownloader.egg-info/PKG-INFO
 ncmlistdownloader.egg-info/SOURCES.txt
 ncmlistdownloader.egg-info/dependency_links.txt
-ncmlistdownloader.egg-info/entry_points.txt
 ncmlistdownloader.egg-info/requires.txt
 ncmlistdownloader.egg-info/top_level.txt
-ncmlistdownloader/cmd/__init__.py
-ncmlistdownloader/cmd/common.py
-ncmlistdownloader/cmd/download.py
-ncmlistdownloader/cmd/find_from_id.py
-ncmlistdownloader/cmd/json_io.py
-ncmlistdownloader/common/__init__.py
-ncmlistdownloader/common/encode_sec_key.py
-ncmlistdownloader/common/global_args.py
-ncmlistdownloader/common/thread_test.py
-ncmlistdownloader/downloader/__init__.py
-ncmlistdownloader/downloader/json_list_io.py
-ncmlistdownloader/editer/__init__.py
-ncmlistdownloader/playlist/__init__.py
-ncmlistdownloader/song/__init__.py
-ncmlistdownloader/song/cleaned.py
+ncmlistdownloader/_old/__init__.py
+ncmlistdownloader/_old/cmd/__init__.py
+ncmlistdownloader/_old/cmd/common.py
+ncmlistdownloader/_old/cmd/download.py
+ncmlistdownloader/_old/cmd/find_from_id.py
+ncmlistdownloader/_old/cmd/json_io.py
+ncmlistdownloader/_old/common/__init__.py
+ncmlistdownloader/_old/common/encode_sec_key.py
+ncmlistdownloader/_old/common/thread_test.py
+ncmlistdownloader/_old/downloader/__init__.py
+ncmlistdownloader/_old/downloader/json_list_io.py
+ncmlistdownloader/_old/editer/__init__.py
+ncmlistdownloader/_old/playlist/__init__.py
+ncmlistdownloader/_old/song/__init__.py
+ncmlistdownloader/music/__init__.py
+ncmlistdownloader/music/multiple_tools.py
```

### Comparing `ncmlistdownloader-2.0.0.240515a1/setup.py` & `ncmlistdownloader-2.0.0.240516a1/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -26,22 +26,20 @@
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: 3.12",
     ],
     name="ncmlistdownloader",
-    version="2.0.0.240515a1",
+    version="2.0.0.240516a1",
     description="获取网易云音乐歌单数据，下载音乐，主动添加元信息。",
     author="CooooldWind_",
     url="https://gitee.com/Cooooldwind/163ListDownloader_NexT",
     packages=find_packages(),
     install_requires=[
         "pycryptodome",
         "pillow",
         "mutagen",
         "requests",
     ],
-    entry_points={
-        "console_scripts": ["ncmlistdownloader = ncmlistdownloader.__init__:main"]
-    },
+    # entry_points={"console_scripts": ["ncmlistdownloader = ncmlistdownloader.__init__:main"]},
 )
```

