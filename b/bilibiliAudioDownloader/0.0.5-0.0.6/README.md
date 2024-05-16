# Comparing `tmp/bilibiliaudiodownloader-0.0.5.tar.gz` & `tmp/bilibiliaudiodownloader-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bilibiliaudiodownloader-0.0.5.tar", last modified: Thu May 16 15:53:58 2024, max compression
+gzip compressed data, was "bilibiliaudiodownloader-0.0.6.tar", last modified: Thu May 16 16:10:57 2024, max compression
```

## Comparing `bilibiliaudiodownloader-0.0.5.tar` & `bilibiliaudiodownloader-0.0.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-05-16 15:53:58.897836 bilibiliaudiodownloader-0.0.5/
-drwxrwxrwx   0        0        0        0 2024-05-16 15:53:58.854828 bilibiliaudiodownloader-0.0.5/BilibiliAudioDownloader/
--rw-rw-rw-   0        0        0       83 2024-05-16 15:48:42.000000 bilibiliaudiodownloader-0.0.5/BilibiliAudioDownloader/__init__.py
--rw-rw-rw-   0        0        0     1493 2024-05-09 12:09:38.000000 bilibiliaudiodownloader-0.0.5/BilibiliAudioDownloader/audio_downloader.py
--rw-rw-rw-   0        0        0     2621 2024-05-07 02:09:50.000000 bilibiliaudiodownloader-0.0.5/BilibiliAudioDownloader/bvid_search.py
--rw-rw-rw-   0        0        0     1584 2024-05-07 01:58:18.000000 bilibiliaudiodownloader-0.0.5/BilibiliAudioDownloader/up_uid_search.py
--rw-rw-rw-   0        0        0     1873 2024-05-16 15:53:58.892830 bilibiliaudiodownloader-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     1162 2024-05-13 12:21:06.000000 bilibiliaudiodownloader-0.0.5/README.md
-drwxrwxrwx   0        0        0        0 2024-05-16 15:53:58.889830 bilibiliaudiodownloader-0.0.5/bilibiliAudioDownloader.egg-info/
--rw-rw-rw-   0        0        0     1873 2024-05-16 15:53:57.000000 bilibiliaudiodownloader-0.0.5/bilibiliAudioDownloader.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      462 2024-05-16 15:53:58.000000 bilibiliaudiodownloader-0.0.5/bilibiliAudioDownloader.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-16 15:53:57.000000 bilibiliaudiodownloader-0.0.5/bilibiliAudioDownloader.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      107 2024-05-16 15:53:57.000000 bilibiliaudiodownloader-0.0.5/bilibiliAudioDownloader.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       23 2024-05-16 15:53:57.000000 bilibiliaudiodownloader-0.0.5/bilibiliAudioDownloader.egg-info/requires.txt
--rw-rw-rw-   0        0        0       24 2024-05-16 15:53:57.000000 bilibiliaudiodownloader-0.0.5/bilibiliAudioDownloader.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-16 15:53:58.898833 bilibiliaudiodownloader-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0     1278 2024-05-16 15:49:18.000000 bilibiliaudiodownloader-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-16 16:10:57.939523 bilibiliaudiodownloader-0.0.6/
+drwxrwxrwx   0        0        0        0 2024-05-16 16:10:57.892524 bilibiliaudiodownloader-0.0.6/BilibiliAudioDownloader/
+-rw-rw-rw-   0        0        0       83 2024-05-16 15:48:42.000000 bilibiliaudiodownloader-0.0.6/BilibiliAudioDownloader/__init__.py
+-rw-rw-rw-   0        0        0     1764 2024-05-16 16:01:12.000000 bilibiliaudiodownloader-0.0.6/BilibiliAudioDownloader/audio_downloader.py
+-rw-rw-rw-   0        0        0     2621 2024-05-07 02:09:50.000000 bilibiliaudiodownloader-0.0.6/BilibiliAudioDownloader/bvid_search.py
+-rw-rw-rw-   0        0        0     1584 2024-05-07 01:58:18.000000 bilibiliaudiodownloader-0.0.6/BilibiliAudioDownloader/up_uid_search.py
+-rw-rw-rw-   0        0        0     1873 2024-05-16 16:10:57.936523 bilibiliaudiodownloader-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     1162 2024-05-13 12:21:06.000000 bilibiliaudiodownloader-0.0.6/README.md
+drwxrwxrwx   0        0        0        0 2024-05-16 16:10:57.915525 bilibiliaudiodownloader-0.0.6/bilibiliAudioDownloader.egg-info/
+-rw-rw-rw-   0        0        0     1873 2024-05-16 16:10:57.000000 bilibiliaudiodownloader-0.0.6/bilibiliAudioDownloader.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      462 2024-05-16 16:10:57.000000 bilibiliaudiodownloader-0.0.6/bilibiliAudioDownloader.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-16 16:10:57.000000 bilibiliaudiodownloader-0.0.6/bilibiliAudioDownloader.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      107 2024-05-16 16:10:57.000000 bilibiliaudiodownloader-0.0.6/bilibiliAudioDownloader.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       23 2024-05-16 16:10:57.000000 bilibiliaudiodownloader-0.0.6/bilibiliAudioDownloader.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       24 2024-05-16 16:10:57.000000 bilibiliaudiodownloader-0.0.6/bilibiliAudioDownloader.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-16 16:10:57.939523 bilibiliaudiodownloader-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0     1278 2024-05-16 16:10:49.000000 bilibiliaudiodownloader-0.0.6/setup.py
```

### Comparing `bilibiliaudiodownloader-0.0.5/BilibiliAudioDownloader/audio_downloader.py` & `bilibiliaudiodownloader-0.0.6/BilibiliAudioDownloader/audio_downloader.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,23 @@
 import requests
 import re
 import os
 import time
 import random
 import json
+
+import os
+import sys
+
+# 将当前文件所在的目录添加到 Python 解释器的搜索路径中
+current_dir = os.path.dirname(os.path.abspath(__file__))
+parent_dir = os.path.dirname(current_dir)
+sys.path.append(parent_dir)
+
+# 现在可以进行相对导入
 import up_uid_search
 import bvid_search
 
 def download_audio(bvid):
     header = {
         'user-agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/124.0.0.0 Safari/537.36 Edg/124.0.0.0'
     }
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `bilibiliaudiodownloader-0.0.5/BilibiliAudioDownloader/bvid_search.py` & `bilibiliaudiodownloader-0.0.6/BilibiliAudioDownloader/bvid_search.py`

 * *Files identical despite different names*

### Comparing `bilibiliaudiodownloader-0.0.5/BilibiliAudioDownloader/up_uid_search.py` & `bilibiliaudiodownloader-0.0.6/BilibiliAudioDownloader/up_uid_search.py`

 * *Files identical despite different names*

### Comparing `bilibiliaudiodownloader-0.0.5/PKG-INFO` & `bilibiliaudiodownloader-0.0.6/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bilibiliAudioDownloader
-Version: 0.0.5
+Version: 0.0.6
 Summary: A tool for downloading audio files from Bilibili videos
 Home-page: https://github.com/legal-intelligence/legal-intelligence/tree/Legal_Video/BilibiliAudioDownloader
 Author: YoMi__token__.21
 Author-email: wanglong67890@outlook.com
 License: MIT
 Keywords: python,audio downloader,Bilibili
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `bilibiliaudiodownloader-0.0.5/README.md` & `bilibiliaudiodownloader-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `bilibiliaudiodownloader-0.0.5/bilibiliAudioDownloader.egg-info/PKG-INFO` & `bilibiliaudiodownloader-0.0.6/bilibiliAudioDownloader.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bilibiliAudioDownloader
-Version: 0.0.5
+Version: 0.0.6
 Summary: A tool for downloading audio files from Bilibili videos
 Home-page: https://github.com/legal-intelligence/legal-intelligence/tree/Legal_Video/BilibiliAudioDownloader
 Author: YoMi__token__.21
 Author-email: wanglong67890@outlook.com
 License: MIT
 Keywords: python,audio downloader,Bilibili
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `bilibiliaudiodownloader-0.0.5/setup.py` & `bilibiliaudiodownloader-0.0.6/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.5'
+VERSION = '0.0.6'
 DESCRIPTION = 'A tool for downloading audio files from Bilibili videos'
 
 setup(
     name="bilibiliAudioDownloader",
     version=VERSION,
     author="YoMi__token__.21",
     author_email="wanglong67890@outlook.com",
```

