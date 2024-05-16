# Comparing `tmp/cow_transfer-0.0.5.tar.gz` & `tmp/cow_transfer-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cow_transfer-0.0.5.tar", last modified: Tue May  7 14:52:36 2024, max compression
+gzip compressed data, was "cow_transfer-0.0.6.tar", last modified: Thu May 16 14:53:12 2024, max compression
```

## Comparing `cow_transfer-0.0.5.tar` & `cow_transfer-0.0.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-05-07 14:52:36.060862 cow_transfer-0.0.5/
--rw-rw-rw-   0        0        0     2175 2024-05-07 14:52:36.060862 cow_transfer-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     1647 2024-05-06 17:44:19.000000 cow_transfer-0.0.5/README.md
-drwxrwxrwx   0        0        0        0 2024-05-07 14:52:36.045460 cow_transfer-0.0.5/cow_transfer/
--rw-rw-rw-   0        0        0        0 2023-10-06 16:40:32.000000 cow_transfer-0.0.5/cow_transfer/__init__.py
--rw-rw-rw-   0        0        0     4715 2024-05-06 17:44:19.000000 cow_transfer-0.0.5/cow_transfer/cow_download.py
--rw-rw-rw-   0        0        0    17557 2024-05-06 18:00:33.000000 cow_transfer-0.0.5/cow_transfer/cow_upload.py
--rw-rw-rw-   0        0        0     2845 2024-05-06 18:02:50.000000 cow_transfer-0.0.5/cow_transfer/main.py
--rw-rw-rw-   0        0        0      407 2024-05-06 17:44:19.000000 cow_transfer-0.0.5/cow_transfer/util.py
-drwxrwxrwx   0        0        0        0 2024-05-07 14:52:36.060862 cow_transfer-0.0.5/cow_transfer.egg-info/
--rw-rw-rw-   0        0        0     2175 2024-05-07 14:52:35.000000 cow_transfer-0.0.5/cow_transfer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      359 2024-05-07 14:52:35.000000 cow_transfer-0.0.5/cow_transfer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-07 14:52:35.000000 cow_transfer-0.0.5/cow_transfer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2024-05-07 14:52:35.000000 cow_transfer-0.0.5/cow_transfer.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       37 2024-05-07 14:52:35.000000 cow_transfer-0.0.5/cow_transfer.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-05-07 14:52:35.000000 cow_transfer-0.0.5/cow_transfer.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-07 14:52:36.060862 cow_transfer-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0      954 2024-05-06 17:17:28.000000 cow_transfer-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-16 14:53:12.504055 cow_transfer-0.0.6/
+-rw-rw-rw-   0        0        0     2190 2024-05-16 14:53:12.504055 cow_transfer-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     1662 2024-05-07 16:23:55.000000 cow_transfer-0.0.6/README.md
+drwxrwxrwx   0        0        0        0 2024-05-16 14:53:12.504055 cow_transfer-0.0.6/cow_transfer/
+-rw-rw-rw-   0        0        0        0 2023-10-06 16:40:32.000000 cow_transfer-0.0.6/cow_transfer/__init__.py
+-rw-rw-rw-   0        0        0     4647 2024-05-16 14:51:13.000000 cow_transfer-0.0.6/cow_transfer/cow_download.py
+-rw-rw-rw-   0        0        0    17489 2024-05-16 14:51:13.000000 cow_transfer-0.0.6/cow_transfer/cow_upload.py
+-rw-rw-rw-   0        0        0     2818 2024-05-16 14:53:08.000000 cow_transfer-0.0.6/cow_transfer/main.py
+-rw-rw-rw-   0        0        0      713 2024-05-16 14:50:16.000000 cow_transfer-0.0.6/cow_transfer/util.py
+drwxrwxrwx   0        0        0        0 2024-05-16 14:53:12.504055 cow_transfer-0.0.6/cow_transfer.egg-info/
+-rw-rw-rw-   0        0        0     2190 2024-05-16 14:53:12.000000 cow_transfer-0.0.6/cow_transfer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      359 2024-05-16 14:53:12.000000 cow_transfer-0.0.6/cow_transfer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-16 14:53:12.000000 cow_transfer-0.0.6/cow_transfer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2024-05-16 14:53:12.000000 cow_transfer-0.0.6/cow_transfer.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       37 2024-05-16 14:53:12.000000 cow_transfer-0.0.6/cow_transfer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-05-16 14:53:12.000000 cow_transfer-0.0.6/cow_transfer.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-16 14:53:12.504055 cow_transfer-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      956 2024-05-16 14:53:08.000000 cow_transfer-0.0.6/setup.py
```

### Comparing `cow_transfer-0.0.5/PKG-INFO` & `cow_transfer-0.0.6/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cow_transfer
-Version: 0.0.5
+Version: 0.0.6
 Summary: Easily downlaod file from CowTransfer
 Home-page: https://github.com/xiyoucloud/cow_transfer.git
 Author: txb
 Author-email: txb.sdn@gmail.com
 License: MIT
 Keywords: python,DownloadKit,cow_transfer
 Platform: UNKNOWN
@@ -55,19 +55,20 @@
   --chunk_size INTEGER  分块大小（字节）  [default: 2097152]
   --threads INTEGER     上传并发数  [default: 5]
   --help                Show this message and exit.
 ```
 
 默认情况下会开启 20 个线程对文件进行下载，这会大大加快下载速度，不过下载速度还受到网络带宽的限制，即下载速度最快不会超过网络带宽。
 
-## 打包源码
+## 打包源码发布到Pypi
 ```
 # 安装依赖
 pip install wheel
 pip install twine
 # 打包
 python setup.py bdist_wheel sdist
 
 # 上传打包后的 python 包到 https://pypi.org
 twine upload dist/*
 ```
 
+
```

### Comparing `cow_transfer-0.0.5/README.md` & `cow_transfer-0.0.6/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -39,18 +39,18 @@
   --chunk_size INTEGER  分块大小（字节）  [default: 2097152]
   --threads INTEGER     上传并发数  [default: 5]
   --help                Show this message and exit.
 ```
 
 默认情况下会开启 20 个线程对文件进行下载，这会大大加快下载速度，不过下载速度还受到网络带宽的限制，即下载速度最快不会超过网络带宽。
 
-## 打包源码
+## 打包源码发布到Pypi
 ```
 # 安装依赖
 pip install wheel
 pip install twine
 # 打包
 python setup.py bdist_wheel sdist
 
 # 上传打包后的 python 包到 https://pypi.org
 twine upload dist/*
-```
+```
```

### Comparing `cow_transfer-0.0.5/cow_transfer/cow_download.py` & `cow_transfer-0.0.6/cow_transfer/cow_download.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
-from DownloadKit import DownloadKit
 import os
 import sys
+
 import requests
+from DownloadKit import DownloadKit
 
-from cow_transfer.util import get_str_arr_split_by_new_line_from_file, build_request_header
+from cow_transfer.util import get_headers_from_curl_file
 
 dirname = os.path.dirname(__file__)
 # 创建下载器对象
 d = DownloadKit(roads=20)
 # 线程数
 # 大文件分块大小，默认 20MB
 d.block_size = '50M'
@@ -78,15 +79,15 @@
 
 def download_file(unique_url, target=None, threads=20, header_file_path=None):
     if header_file_path is None:
         header_file_path = './header.txt'
     if not os.path.exists(header_file_path):
         raise SyntaxError("请添加header.txt文件")
     global common_header
-    common_header = build_request_header(get_str_arr_split_by_new_line_from_file(header_file_path))
+    common_header = get_headers_from_curl_file(header_file_path)
     get_permission_info(unique_url)
     file_details = get_file_details(unique_url)
     download_url = get_download_url(file_details)
     if target is None:
         target = dirname
     else:
         if os.path.exists(target) and os.path.isdir(target):
```

### Comparing `cow_transfer-0.0.5/cow_transfer/cow_upload.py` & `cow_transfer-0.0.6/cow_transfer/cow_upload.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 import os
-import oss2
+import threading
 import time
+from concurrent.futures import ThreadPoolExecutor
+
+import oss2
 import requests
-import threading
-from tqdm import tqdm
 from oss2.models import PartInfo
-from concurrent.futures import ThreadPoolExecutor
+from tqdm import tqdm
 
-from cow_transfer.util import build_request_header, get_str_arr_split_by_new_line_from_file
+from cow_transfer.util import get_headers_from_curl_file
 
 requests.adapters.DEFAULT_RETRIES = 3
 
 debug = False
 
 
 def log(text: str) -> str:
@@ -59,15 +60,15 @@
         self.err = ""
         self.status = "work"
         self.file_dict = {}
         self.upload_info = {
             "complete": False
         }
         self.transfer_info = {}
-        self.auth_headers = build_request_header(get_str_arr_split_by_new_line_from_file(header_file_path))
+        self.auth_headers = get_headers_from_curl_file(header_file_path)
 
         # 对象
         self.executor = None
         self.progress_bar_curr = None
         self.progress_bar_total = None
 
     # 执行
```

### Comparing `cow_transfer-0.0.5/cow_transfer/main.py` & `cow_transfer-0.0.6/cow_transfer/main.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,15 @@
-import sys
+import click
+
 from cow_transfer.cow_download import (
     download_file
 )
 from cow_transfer.cow_upload import (
     CowUploader
 )
-import argparse
-import click
 
 
 @click.group()
 def cli():
     """upload and download - v0.1.5"""
 
 
@@ -55,10 +54,10 @@
 @click.option("-h", "--header_file_path", type=click.Path(exists=True), help="header file path",
               default="./header.txt")
 def download(urlcode, threads, path, header_file_path):
     download_file(urlcode, target=path, threads=threads, header_file_path=header_file_path)
 
 
 if __name__ == "__main__":
-    # download_file('bdae5a8fc3444b', ".", 20, "./header.txt")
+    # download_file('de210271491e4f', ".", 20, "./header.txt")
     # upload_file("./header.txt", "./DSCF0001123.jpg", "", "", "", 1, 2097152, 5)
     cli()
```

### Comparing `cow_transfer-0.0.5/cow_transfer.egg-info/PKG-INFO` & `cow_transfer-0.0.6/cow_transfer.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cow-transfer
-Version: 0.0.5
+Version: 0.0.6
 Summary: Easily downlaod file from CowTransfer
 Home-page: https://github.com/xiyoucloud/cow_transfer.git
 Author: txb
 Author-email: txb.sdn@gmail.com
 License: MIT
 Keywords: python,DownloadKit,cow_transfer
 Platform: UNKNOWN
@@ -55,19 +55,20 @@
   --chunk_size INTEGER  分块大小（字节）  [default: 2097152]
   --threads INTEGER     上传并发数  [default: 5]
   --help                Show this message and exit.
 ```
 
 默认情况下会开启 20 个线程对文件进行下载，这会大大加快下载速度，不过下载速度还受到网络带宽的限制，即下载速度最快不会超过网络带宽。
 
-## 打包源码
+## 打包源码发布到Pypi
 ```
 # 安装依赖
 pip install wheel
 pip install twine
 # 打包
 python setup.py bdist_wheel sdist
 
 # 上传打包后的 python 包到 https://pypi.org
 twine upload dist/*
 ```
 
+
```

### Comparing `cow_transfer-0.0.5/setup.py` & `cow_transfer-0.0.6/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,31 +1,30 @@
 from setuptools import setup, find_packages
-import os
 
-VERSION = '0.0.5'
+VERSION = '0.0.6'
 DESCRIPTION = 'Easily downlaod file from CowTransfer'
 
 setup(
     name="cow_transfer",
     version=VERSION,
     author="txb",
     author_email="txb.sdn@gmail.com",
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=open('README.md', encoding="UTF8").read(),
     packages=find_packages(),
     install_requires=['DownloadKit', 'requests', 'oss2', 'tqdm', 'click'],
     keywords=['python', 'DownloadKit', 'cow_transfer'],
     entry_points={
-    'console_scripts': [
-        'cow = cow_transfer.main:cli'
-    ]
+        'console_scripts': [
+            'cow = cow_transfer.main:cli'
+        ]
     },
     license="MIT",
     url="https://github.com/xiyoucloud/cow_transfer.git",
-    classifiers= [
+    classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
         "Operating System :: Microsoft :: Windows"
     ]
-)
+)
```

